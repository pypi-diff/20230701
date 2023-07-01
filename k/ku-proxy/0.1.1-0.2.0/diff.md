# Comparing `tmp/ku_proxy-0.1.1-py3-none-any.whl.zip` & `tmp/ku_proxy-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,12 @@
-Zip file size: 4750 bytes, number of entries: 7
--rw-r--r--  2.0 unx       42 b- defN 23-Feb-01 10:29 ku/__init__.py
--rw-r--r--  2.0 unx     5427 b- defN 23-Feb-01 10:29 ku/ku.py
--rw-rw-rw-  2.0 unx     1064 b- defN 23-Feb-01 10:29 ku_proxy-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3261 b- defN 23-Feb-01 10:29 ku_proxy-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-01 10:29 ku_proxy-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        3 b- defN 23-Feb-01 10:29 ku_proxy-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      524 b- defN 23-Feb-01 10:29 ku_proxy-0.1.1.dist-info/RECORD
-7 files, 10413 bytes uncompressed, 3824 bytes compressed:  63.3%
+Zip file size: 10546 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       42 b- defN 23-Jul-01 19:41 ku/__init__.py
+-rw-r--r--  2.0 unx    11923 b- defN 23-Jul-01 19:41 ku/ku.py
+-rw-r--r--  2.0 unx     9453 b- defN 23-Jul-01 19:41 ku/kun.py
+-rw-r--r--  2.0 unx      943 b- defN 23-Jul-01 19:41 ku/util.py
+-rw-rw-rw-  2.0 unx     1064 b- defN 23-Jul-01 19:41 ku_proxy-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3462 b- defN 23-Jul-01 19:41 ku_proxy-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-01 19:41 ku_proxy-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 23-Jul-01 19:41 ku_proxy-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        3 b- defN 23-Jul-01 19:41 ku_proxy-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      753 b- defN 23-Jul-01 19:41 ku_proxy-0.2.0.dist-info/RECORD
+10 files, 27779 bytes uncompressed, 9272 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -1,22 +1,31 @@
 Filename: ku/__init__.py
 Comment: 
 
 Filename: ku/ku.py
 Comment: 
 
-Filename: ku_proxy-0.1.1.dist-info/LICENSE
+Filename: ku/kun.py
 Comment: 
 
-Filename: ku_proxy-0.1.1.dist-info/METADATA
+Filename: ku/util.py
 Comment: 
 
-Filename: ku_proxy-0.1.1.dist-info/WHEEL
+Filename: ku_proxy-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: ku_proxy-0.1.1.dist-info/top_level.txt
+Filename: ku_proxy-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: ku_proxy-0.1.1.dist-info/RECORD
+Filename: ku_proxy-0.2.0.dist-info/WHEEL
+Comment: 
+
+Filename: ku_proxy-0.2.0.dist-info/entry_points.txt
+Comment: 
+
+Filename: ku_proxy-0.2.0.dist-info/top_level.txt
+Comment: 
+
+Filename: ku_proxy-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ku/__init__.py

```diff
@@ -1,2 +1,2 @@
 from .ku import * # NOQA
-version = '0.1.1'
+version = '0.2.0'
```

## ku/ku.py

```diff
@@ -1,172 +1,379 @@
 """
     Ku
     ==
-    single-thread async tcp proxy
+    single-threaded async mitm tcp proxy
 """
 
-from threading import Thread
+from threading import Thread, currentThread
 from select import select
-from socket import socket
-from typing import Union
+from socket import socket, SOL_SOCKET, AF_INET, AF_INET6
+import logging
+
+from typing import Union, Tuple, List
+
+from enum import Enum
+from time import time, sleep
+from re import match
+
+from platform import system
+
+# https://learn.microsoft.com/en-us/windows/win32/winsock/so-conditional-accept
+SO_CONDITIONAL_ACCEPT = 0x3002
 
 class Reject(object):
     pass
 
 class Pass(object):
     pass
 
+class state(Enum):
+    DISCONNECTED = 0
+    CLIENT_W_U = 1 # client waiting for upstream
+    CONNECTED = 2
+
 class tcpsession(object):
 
-    def __init__(self, client: socket, server: socket, proxy):
+    state: state = state.DISCONNECTED
+
+    client: socket
+    server: socket
+
+    client_total: int
+    server_total: int
+
+    estab_time: int
+
+    def __init__(self, client: socket, server: socket, proxy, *args) -> None:
         pass
 
     def clientbound(self, data: bytes) -> Union[bytes, Reject, Pass]:
         pass
 
     def serverbound(self, data) -> Union[bytes, Reject, Pass]:
         pass
 
-    def connection_made(self) -> None:
-        pass
-
     def connection_lost(self, side: Union[socket, None], err: Union[Exception, None]) -> None:
         pass
+    
+    def shutdown(self) -> None:
+        pass
+
+    def _change_state(self, new_state: state) -> None:
+        self.proxy.logger.debug(f"#{id(self)} {self.state} -> {new_state}")
+        self.state = new_state
+
+    def terminate(self) -> None:
+        self.proxy.terminate(self)
+
+    def __repr__(self):        
+        if self.state != state.CONNECTED:
+            return super().__repr__()
+        return f"<#{id(self)}[{round((time() - self.estab_time), 2)}] {self.client.getpeername()}->{self.client.getsockname()}::{self.server.getsockname()}->{self.server.getpeername()}>"
 
 class ku(object):
 
-    fd: list  # tracked file descriptors
-    ss: list  # [[<socket Client>, <socket Upstream>, <tcpsession Session>], ...]
+    fd: List[socket]  # tracked file descriptors
+    wai: List[socket] # wa
+    ss: List[tcpsession]
 
-    socket: socket  # listening socket
+    sockets: Tuple[socket]  # listening socket
     thread: Thread  # polling thread
     upstream: tuple  # upstream proto, host, port
 
     alive: bool = True  # alive marker
-    dead: bool = False # loop dead marker
+    pause: bool = False # you can temporarily stop polling
+    PSM = 0.00001 # power Save Mode, reduces cpu cycles count
 
     @staticmethod
-    def htphp(host: tuple):
-        """
-            convert host tuple to proto, host, port
-        """
-        x = host[0].split(']')
-        if len(x) == 2:
-            return 23, x[0][1:], host[1]
-        return 2, host[0], host[1]
+    def _resolve_proto(host: str):
 
-    def __init__(self, listen: tuple, upstream: tuple, session: tcpsession = tcpsession, maxcon: int = -1):
+        IPv6 = r"^(\[[\d\D]{1,}\])$"
+        IP6 = r"^([a-f0-9:]{1,})$"
+        IPv4 = r"^([0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3})$"
+        TLD = r"^([A-z0-9._-]{1,})$"
+
+        PATTERNS = [IPv6, IPv4, TLD, IP6]
+
+        for pattern in PATTERNS:
+            i = match(pattern, host)
+            if i:
+                if pattern is IPv6:
+                    return AF_INET6
+                
+                elif pattern is IP6:
+                    return AF_INET6
+
+                elif pattern is IPv4:
+                    return AF_INET
+
+                elif pattern is TLD:
+                    return -1
+
+    def __init__(self, listen: tuple, upstream: tuple, session: tcpsession = tcpsession, session_args: tuple = (), maxcon: int = -1, upstream_6: bool = False):
 
         self.fd: list = []
+        self.wai: list = []
         self.ss: list = []
 
-        self.upstream = self.htphp(upstream)
+        self.logger = logging.getLogger("ku.devel")
+
+        proto = self._resolve_proto(upstream[0])
+        self.upstream = (AF_INET6 if upstream_6 else AF_INET if proto == -1 else proto, upstream[0], upstream[1])
+        self.logger.debug(f"Upstreaming to - {'v6' if self.upstream[0] is AF_INET6 else 'v4'} {upstream[0]}:{upstream[1]}")
+
         self.session = session
         self.maxcon = maxcon
+        self.session_args = session_args
 
-        proto, host, port = self.htphp(listen)
-        self.socket = socket(proto, 1)
-        self.socket.bind((host, port))
-        self.socket.listen()
-        self.fd.append(self.socket)
+        self.sockets = ()
+        for i in range(0, len(listen), 2):
+            proto, host, port = self._resolve_proto(listen[i]), *listen[i:i+2]
+
+            sock = socket(proto, 1)
+            self.logger.debug(f"Listening at - {'v6' if proto is AF_INET6 else 'v4'} {host}:{port}")
+            sock.bind((host, port))
+            if system() == "Windows":
+                sock.setsockopt(SOL_SOCKET, SO_CONDITIONAL_ACCEPT, 1)
+            sock.listen()
+            self.fd.append(sock)
+            self.sockets = (*self.sockets, sock)
 
-        self.thread = Thread(target=self.poll)
+        self.thread = Thread(target=self.poll, name=f"Ku poller #{currentThread().ident}", daemon=True)
         self.thread.start()
 
     def shutdown(self):
+        # can't be called from handler!)
+        if currentThread() is self.thread:
+            raise RuntimeError(f"People stuck at {currentThread()}")
+
         self.alive = False
-        while not self.dead:
+        while self.thread.is_alive():
             pass
+
+        for s in self.ss:
+            if s.state == state.CONNECTED:
+                s.shutdown()
+
+            s.client.shutdown(1)
+            s.server.shutdown(1)
+            s._change_state(state.DISCONNECTED)
+
         del self.fd
         del self.ss        
-        self.socket.close()
-        del self.socket
+        for sock in self.sockets:
+            sock.close()
+        del self.sockets
         del self.thread
 
     def terminate(self, session: tcpsession):
-        for s in self.ss.copy():
-            if s[2] == session:
-                session.connection_lost(None, RuntimeError("Internal terminate request"))
-                self.ss.remove(s)
-                self.fd.remove(s[0])
-                self.fd.remove(s[1])
-                s[1].close()
-                s[0].close()
-
-    def _handle_socket_disconnect(self, fd, err):        
-        for s in self.ss.copy():
-            if s[0] == fd or s[1] == fd:
-                # found session
-                s[2].connection_lost(fd, err)
-                self.ss.remove(s)
-                self.fd.remove(s[0])
-                self.fd.remove(s[1])
-                s[1].close()
-                s[0].close()
+        session._change_state(state.DISCONNECTED)
+        # Call handlers
+        session.connection_lost(None, RuntimeError("Internal terminate request"))
+        # Remove descriptors from polling
+        self.fd.remove(session.client)
+        self.fd.remove(session.server)
+        # Shutdown sockets
+        session.client.shutdown(2)
+        session.server.shutdown(2)
+        # Delete session
+        self.ss.remove(session)
+        self.logger.debug(f"#{id(session)} terminated [ITR]")
+
+    def _handle_socket_disconnect(self, fd, err):            
+        s = self.lookup_session(fd)        
+        if not s:
+            # ITR
+            return
+
+        # Remove descriptors from wathcing list
+        self.fd.remove(s.client)
+        self.fd.remove(s.server)
+
+        # Close associated descripors
+        s.server.close()
+        s.client.close()
+
+        # Destroy session instance
+        self.ss.remove(s)
+
+        s._change_state(state.DISCONNECTED)
+        s.connection_lost(fd, err)
+
+        self.logger.debug(f"#{id(s)} terminated")
+
+    def lookup_session(self, fd: socket):
+        for s in self.ss:
+            if s.client == fd or s.server == fd:
+                return s
+
+    def send(self, fd: socket, data: bytes) -> None:
+        try:
+            fd.sendall(data)
+        except Exception as e:
+            self.logger.debug(f"Failed to send data to the fd, initiating session termination...")
+            self._handle_socket_disconnect(fd)
+
+    def _accept(self, fd: socket):
+        # check limitations
+        if len(self.ss) == self.maxcon:
+            try:
+                c, addr = fd.accept()
+                c.close()
+            except:
+                pass
+            return
+        
+        # create new instance of tcpsession class
+        s = object.__new__(self.session)
+        s.proxy = self
+        self.logger.debug(f"#{id(s)} Begin new connection request processing")
+
+        # new client
+        try:
+            c, addr = fd.accept()
+        except Exception as e:
+            self.logger.warning(f"Failed to accept new client: {e}")
+            self.logger.debug(f"#{id(s)} terminated")
+            return
+            
+        self.logger.debug(f"#{id(s)} client: {addr}")
+        s.client = c
+
+        s._change_state(state.CLIENT_W_U)
+
+        # new upstream
+        u = socket(self.upstream[0], 1)
+        u.settimeout(0)
+        s.server = u
+
+        try:                        
+            u.connect(self.upstream[1:])
+        except BlockingIOError:
+            pass
+
+        self.logger.debug(f"#{id(s)} upstreaming initiated, waiting...")        
+
+        self.ss.append(s)                    
+        self.wai.append(u)
 
     def poll(self):
+        self.logger.debug("Begin polling")
+
         while self.alive:
             # select()
-            fds = select(self.fd, [], [], 0)[0]
+            fds, puo, puf = select(self.fd, self.wai, self.wai, 0)
+            if not (fds or puo or puf) or self.pause:
+                if self.PSM:
+                    sleep(self.PSM)
+                continue
 
-            if self.socket in fds:
-                # check limitations
-                if len(self.ss) != self.maxcon:
-                    # new client
-                    c, addr = self.socket.accept()
+            for fd in puo:                
+                s = self.lookup_session(fd)
+                self.logger.debug(f"#{id(s)} upstreamed, initiating trasmisson")
+
+                # Remove upstream from waiting list
+                self.wai.remove(fd)
+
+                # Add client & upstream to watging list
+                self.fd.append(fd)
+                self.fd.append(s.client)
+
+                # Change session state
+                s._change_state(state.CONNECTED)
+
+                s.estab_time = time()
+
+                # Init session
+                s.__init__(s.client, fd, self, *self.session_args)
+
+            for fd in puf:
+                s = self.lookup_session(fd)
+                self.logger.debug(f"#{id(s)} Failed to upstream")
+
+                # Remove upstream from waiting list
+                self.wai.remove(fd)
+
+                # Close associated client & upstream descriptors
+                s.client.close()
+                fd.close()
+
+                # Change session state
+                s._change_state(state.DISCONNECTED)
+
+                self.ss.remove(s)
+
+                self.logger.debug(f"#{id(s)} terminated")
+
+            for sock in self.sockets:
+                if sock in fds:
+                    self._accept(sock)
+                    fds.remove(sock)
+
+            for fd in fds:
+                if fd not in self.fd:
+                    continue
+
+                s = self.lookup_session(fd)
+                bname = 'client' if fd is s.client else 'upstream'
 
-                    # new upstream
-                    u = socket(self.upstream[0], 1)
-                    try:
-                        u.connect(self.upstream[1:])
-                    except Exception as e:
-                        print(F"Failed to connect to the server due to an error: {e}")
-                        c.close()
-                        continue
-
-                    # create new instance of tcpsession class
-                    s = self.session(c, u, self)
-                    s.connection_made()
-
-                    self.ss.append([c, u, s])
-                    self.fd.append(c)
-                    self.fd.append(u)
-                fds.remove(self.socket)
-            print(fds) if self.socket in fds else None
-            for f in fds:
                 try:
-                    data = f.recv(65535)
+                    data = fd.recv(65535)
                 except Exception as e:
-                    self._handle_socket_disconnect(f, e)
+                    self.logger.debug(f"#{id(s)}, {bname} lost connection: {e}")
+                    self._handle_socket_disconnect(fd, e)
                     continue
 
                 if len(data) < 1:
-                    self._handle_socket_disconnect(f, None)
+                    self.logger.debug(f"#{id(s)}, {bname} disconnected")
+                    self._handle_socket_disconnect(fd, None)
                     continue
 
-                for s in self.ss:
-                    if f == s[0]:
-                        hr = s[2].serverbound(data)
-                        if isinstance(hr, bytes):
-                            data = hr
-                        elif hr is Reject:
+                if fd is s.client:
+                    self.logger.debug(f"#{id(s)} client -> server {round(len(data) / 1000, 2)}Kb")
+                    hr = None
+
+                    try:
+                        hr = s.serverbound(data)
+                    except Exception as e:
+                        self.logger.error(f"Exception in {s.serverbound}: {e}")
+
+                    if isinstance(hr, bytes):
+                        data = hr
+
+                    elif hr is Reject:
                             continue
-                        elif hr is not Pass and hr is not None:
-                            raise RuntimeError(F"Handler returned undefined type! {hr.__class__}")
-                        try:
-                            s[1].sendall(data)
-                        except Exception as e:
-                            self._handle_socket_disconnect(f, e)
-
-                    elif f == s[1]:
-                        hr = s[2].clientbound(data)
-                        if isinstance(hr, bytes):
-                            data = hr
-                        elif hr is Reject:
+
+                    elif hr is not Pass and hr is not None:
+                        self.logger.error(F"#{id(s)} ServerBound handler returned unidentified type! {hr.__class__}")
+
+                    try:
+                        s.server.sendall(data)
+                    except Exception as e:
+                        self.logger.debug(f"#{id(s)} Upstream dropped connection in the middle of data transmission process")
+                        self._handle_socket_disconnect(s.server, e)
+
+                else:
+                    self.logger.debug(f"#{id(s)} server -> client {round(len(data) / 1000, 2)}Kb")
+                    hr = None
+
+                    try:
+                        hr = s.clientbound(data)
+                    except Exception as e:
+                        self.logger.error(f"Exception in {s.clientbound}: {e}")                        
+
+                    if isinstance(hr, bytes):
+                        data = hr
+
+                    elif hr is Reject:
                             continue
-                        elif hr is not Pass and hr is not None:
-                            raise RuntimeError(F"Handler returned undefined type! {hr.__class__}")
-                        try:
-                            s[0].sendall(data)
-                        except Exception as e:
-                            self._handle_socket_disconnect(f, e)
-        self.dead = True
+
+                    elif hr is not Pass and hr is not None:
+                        self.logger.error(F"#{id(s)} ClientBound handler returned unidentified type! {hr.__class__}")
+
+                    try:
+                        s.client.sendall(data)
+                    except Exception as e:
+                        self.logger.debug(f"#{id(s)} Client dropped connection in the middle of data transmission process")
+                        self._handle_socket_disconnect(s.client, e)
+
+        self.logger.debug(f"Stop polling")
```

## Comparing `ku_proxy-0.1.1.dist-info/LICENSE` & `ku_proxy-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ku_proxy-0.1.1.dist-info/METADATA` & `ku_proxy-0.2.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ku-proxy
-Version: 0.1.1
+Version: 0.2.0
 Summary: ku is fast, async, modern, little tcp man-in-the-middle proxy library, written in pure Python 3
 Home-page: https://gitlab.com/seeklay/ku
 Author: seeklay
 Author-email: rudeboy@seeklay.icu
 License: MIT
 Download-URL: https://gitlab.com/seeklay/ku
 Platform: OS Independent
@@ -19,22 +19,23 @@
 
 ![](https://img.shields.io/badge/Made%20with-Python-1f425f.svg) ![](https://img.shields.io/gitlab/license/seeklay/ku.svg) ![](https://tokei.rs/b1/gitlab/seeklay/ku) ![](https://badgen.net/pypi/v/ku-proxy) ![](https://img.shields.io/pypi/dw/ku-proxy?style=flat&logo=pypi) ![](https://gitlab.com/seeklay/ku/badges/main/pipeline.svg) ![](https://gitlab.com/seeklay/ku/badges/main/coverage.svg)
 
 ### Features
  - Dump data between clients and server
  - Spoof data in both directions
  - Drop data selectively
+ - IPv6 Ready (pass upstream_6 for upstreaming ipv6 or enclose ipv6 addr in brackets like [::1] for listening addrs
 
 ### Is this proxy fast?
 [Proxy speed comparison results](speedtest.md)
 
 ### TODO
 
  - [x] Tcp mitm proxy library
- - [ ] Proxy executable script
+ - [x] Proxy executable script (kun (alpha))
 
 ### Installation
 ```bash
 pip install -U ku-proxy
 ```
 ### Author
 [seeklay](https://gitlab.com/seeklay/)
@@ -45,16 +46,15 @@
 ### Simple proxy usage:
 **Try to run this script and open http://localhost:80 in you browser**
 
 ```python
 from ku import ku, tcpsession
 from time import sleep
 
-proxy = ku(("localhost", 80), ("api.ipify.com", 80))
-# now the proxy is already running
+proxy = ku(("localhost", 80, "[::1]", 80), ("g.co", 80))
 
 while 7:
     try:
         sleep(0.07)
     except KeyboardInterrupt:
         proxy.shutdown() #proxy creates a thread to async poll for socket events
         break            #we need to call shutdown() to break the thread loop
@@ -74,18 +74,21 @@
         self.proxy = proxy
         self.id = id(self)        
         print(F"#{self.id} new conn {client.getpeername()}->{client.getsockname()}::{server.getsockname()}->{server.getpeername()}")
 
     def clientbound(self, data):        
         print(F"#{self.id} server->client  {len(data)}")
         print(data)
+        return Pass
 
     def serverbound(self, data):        
         print(F"#{self.id} client->server  {len(data)}")
         print(data)
+        #return None
+        #in python None is returned by default, None == Pass
 
     def connection_made(self):
         print(F"#{self.id} connection_made")
 
     def connection_lost(self, side, err):
         side = 'client' if side is self.client else 'server' if side is not None else 'proxy'
         print(F"#{self.id} connection_lost by {side} due to {err}")
```

