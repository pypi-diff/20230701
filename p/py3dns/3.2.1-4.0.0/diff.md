# Comparing `tmp/py3dns-3.2.1.tar.gz` & `tmp/py3dns-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py3dns-3.2.1.tar", last modified: Wed Sep  4 12:15:49 2019, max compression
+gzip compressed data, was "py3dns-4.0.0.tar", last modified: Sat Jul  1 21:13:47 2023, max compression
```

## Comparing `py3dns-3.2.1.tar` & `py3dns-4.0.0.tar`

### file list

```diff
@@ -1,42 +1,29 @@
-drwxr-xr-x   0 kitterma  (1000) kitterma  (1000)        0 2019-09-04 12:15:49.000000 py3dns-3.2.1/
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)     3507 2019-09-04 12:14:51.000000 py3dns-3.2.1/CHANGES
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)      499 2018-07-23 16:27:50.000000 py3dns-3.2.1/CREDITS.txt
-drwxr-xr-x   0 kitterma  (1000) kitterma  (1000)        0 2019-09-04 12:15:49.000000 py3dns-3.2.1/DNS/
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)    17703 2019-09-04 10:19:11.000000 py3dns-3.2.1/DNS/Base.py
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)      845 2018-07-23 16:27:50.000000 py3dns-3.2.1/DNS/Class.py
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)    25495 2018-07-23 16:27:50.000000 py3dns-3.2.1/DNS/Lib.py
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)      546 2018-07-23 16:27:50.000000 py3dns-3.2.1/DNS/Opcode.py
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)     1619 2018-07-23 16:27:50.000000 py3dns-3.2.1/DNS/Status.py
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)     1739 2018-07-23 16:27:50.000000 py3dns-3.2.1/DNS/Type.py
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)      862 2019-09-04 09:43:56.000000 py3dns-3.2.1/DNS/__init__.py
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)     2678 2019-09-04 12:11:10.000000 py3dns-3.2.1/DNS/lazy.py
-drwxr-xr-x   0 kitterma  (1000) kitterma  (1000)        0 2019-09-04 12:15:49.000000 py3dns-3.2.1/DNS/tests/
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)      305 2018-07-23 16:27:50.000000 py3dns-3.2.1/DNS/tests/__init__.py
--rwxr-xr-x   0 kitterma  (1000) kitterma  (1000)    18712 2018-07-23 16:27:50.000000 py3dns-3.2.1/DNS/tests/testPackers.py
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)    10690 2019-09-04 12:13:10.000000 py3dns-3.2.1/DNS/tests/test_base.py
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)     3848 2018-07-23 16:27:50.000000 py3dns-3.2.1/DNS/win32dns.py
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)     4062 2018-07-23 16:27:50.000000 py3dns-3.2.1/LICENSE
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)      183 2018-07-23 17:26:38.000000 py3dns-3.2.1/MANIFEST.in
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)      858 2019-09-04 12:15:49.000000 py3dns-3.2.1/PKG-INFO
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)      524 2018-07-23 16:27:50.000000 py3dns-3.2.1/README-guido.txt
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)     6055 2018-07-23 17:06:46.000000 py3dns-3.2.1/README.txt
-drwxr-xr-x   0 kitterma  (1000) kitterma  (1000)        0 2019-09-04 12:15:49.000000 py3dns-3.2.1/py3dns.egg-info/
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)      858 2019-09-04 12:15:48.000000 py3dns-3.2.1/py3dns.egg-info/PKG-INFO
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)      566 2019-09-04 12:15:48.000000 py3dns-3.2.1/py3dns.egg-info/SOURCES.txt
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)        1 2019-09-04 12:15:48.000000 py3dns-3.2.1/py3dns.egg-info/dependency_links.txt
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)        1 2018-07-23 17:07:56.000000 py3dns-3.2.1/py3dns.egg-info/not-zip-safe
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)        4 2019-09-04 12:15:48.000000 py3dns-3.2.1/py3dns.egg-info/top_level.txt
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)       38 2019-09-04 12:15:49.000000 py3dns-3.2.1/setup.cfg
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)     1143 2018-07-23 17:04:32.000000 py3dns-3.2.1/setup.py
--rwxr-xr-x   0 kitterma  (1000) kitterma  (1000)      141 2018-07-23 16:27:50.000000 py3dns-3.2.1/test.py
-drwxr-xr-x   0 kitterma  (1000) kitterma  (1000)        0 2019-09-04 12:15:49.000000 py3dns-3.2.1/tests/
--rwxr-xr-x   0 kitterma  (1000) kitterma  (1000)     1126 2018-07-23 16:27:50.000000 py3dns-3.2.1/tests/test.py
--rwxr-xr-x   0 kitterma  (1000) kitterma  (1000)      360 2018-07-23 16:27:50.000000 py3dns-3.2.1/tests/test2.py
--rwxr-xr-x   0 kitterma  (1000) kitterma  (1000)      167 2018-07-23 16:27:50.000000 py3dns-3.2.1/tests/test4.py
--rwxr-xr-x   0 kitterma  (1000) kitterma  (1000)     2164 2018-07-23 16:27:50.000000 py3dns-3.2.1/tests/test5.py
--rwxr-xr-x   0 kitterma  (1000) kitterma  (1000)     1120 2018-07-23 16:27:50.000000 py3dns-3.2.1/tests/test6.py
--rwxr-xr-x   0 kitterma  (1000) kitterma  (1000)     1579 2018-07-23 16:27:50.000000 py3dns-3.2.1/tests/test7.py
--rwxr-xr-x   0 kitterma  (1000) kitterma  (1000)      282 2018-07-23 16:27:50.000000 py3dns-3.2.1/tests/testsrv.py
-drwxr-xr-x   0 kitterma  (1000) kitterma  (1000)        0 2019-09-04 12:15:49.000000 py3dns-3.2.1/tools/
--rw-r--r--   0 kitterma  (1000) kitterma  (1000)     1628 2018-07-23 16:27:50.000000 py3dns-3.2.1/tools/caching.py
--rwxr-xr-x   0 kitterma  (1000) kitterma  (1000)     1987 2018-07-23 16:27:50.000000 py3dns-3.2.1/tools/named-perf.py
+-rw-r--r--   0        0        0     3975 2023-07-01 21:05:20.511201 py3dns-4.0.0/CHANGES
+-rw-r--r--   0        0        0      499 2020-04-17 19:29:51.000000 py3dns-4.0.0/CREDITS.txt
+-rw-r--r--   0        0        0    16252 2023-07-01 20:39:28.319523 py3dns-4.0.0/DNS/Base.py
+-rw-r--r--   0        0        0      845 2020-04-17 19:29:51.000000 py3dns-4.0.0/DNS/Class.py
+-rw-r--r--   0        0        0    25495 2020-04-17 19:29:51.000000 py3dns-4.0.0/DNS/Lib.py
+-rw-r--r--   0        0        0      546 2020-04-17 19:29:51.000000 py3dns-4.0.0/DNS/Opcode.py
+-rw-r--r--   0        0        0     1619 2020-04-17 19:29:51.000000 py3dns-4.0.0/DNS/Status.py
+-rw-r--r--   0        0        0     1739 2020-04-17 19:29:51.000000 py3dns-4.0.0/DNS/Type.py
+-rw-r--r--   0        0        0      862 2023-07-01 19:23:56.276977 py3dns-4.0.0/DNS/__init__.py
+-rw-r--r--   0        0        0     2678 2020-04-17 19:29:51.000000 py3dns-4.0.0/DNS/lazy.py
+-rw-r--r--   0        0        0      305 2020-04-17 19:29:51.000000 py3dns-4.0.0/DNS/tests/__init__.py
+-rwxr-xr-x   0        0        0    18712 2020-04-17 19:29:51.000000 py3dns-4.0.0/DNS/tests/testPackers.py
+-rw-r--r--   0        0        0    10704 2020-04-17 19:29:51.000000 py3dns-4.0.0/DNS/tests/test_base.py
+-rw-r--r--   0        0        0     3848 2020-04-17 19:29:51.000000 py3dns-4.0.0/DNS/win32dns.py
+-rw-r--r--   0        0        0     4062 2020-04-17 19:29:51.000000 py3dns-4.0.0/LICENSE
+-rw-r--r--   0        0        0      524 2020-04-17 19:29:51.000000 py3dns-4.0.0/README-guido.txt
+-rw-r--r--   0        0        0     6364 2023-07-01 20:43:41.852065 py3dns-4.0.0/README.txt
+-rw-r--r--   0        0        0     1042 2023-07-01 20:13:25.842207 py3dns-4.0.0/pyproject.toml
+-rwxr-xr-x   0        0        0      310 2020-04-17 19:29:51.000000 py3dns-4.0.0/test.py
+-rwxr-xr-x   0        0        0     1126 2020-04-17 19:29:51.000000 py3dns-4.0.0/tests/test.py
+-rwxr-xr-x   0        0        0      360 2020-04-17 19:29:51.000000 py3dns-4.0.0/tests/test2.py
+-rwxr-xr-x   0        0        0      167 2020-04-17 19:29:51.000000 py3dns-4.0.0/tests/test4.py
+-rwxr-xr-x   0        0        0     2164 2020-04-17 19:29:51.000000 py3dns-4.0.0/tests/test5.py
+-rwxr-xr-x   0        0        0     1120 2020-04-17 19:29:51.000000 py3dns-4.0.0/tests/test6.py
+-rwxr-xr-x   0        0        0     1579 2020-04-17 19:29:51.000000 py3dns-4.0.0/tests/test7.py
+-rwxr-xr-x   0        0        0      282 2020-04-17 19:29:51.000000 py3dns-4.0.0/tests/testsrv.py
+-rw-r--r--   0        0        0     1628 2020-04-17 19:29:51.000000 py3dns-4.0.0/tools/caching.py
+-rwxr-xr-x   0        0        0     1987 2020-04-17 19:29:51.000000 py3dns-4.0.0/tools/named-perf.py
+-rw-r--r--   0        0        0     7141 1970-01-01 00:00:00.000000 py3dns-4.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `py3dns-3.2.1/CHANGES` & `py3dns-4.0.0/CHANGES`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+4.0.0 Sat, Jul 1, 2023
+ * Bump major version due to incompatible change
+ * Remove class DnsAsyncRequest, asyncore is removed from Python 3.12 and it
+   would require a substial rewrite - If you need async DNS, use aiodns
+   instead. (LP: #2003329)
+ * Switch build system from setuptools with setup.py to flit
+ * If /etc/resolv.conf, assume DNS server is '127.0.0.1', this changes the
+   existing behavior - in previous releases there would be a
+   FileNotFoundError.
+
 3.2.1 Wed, Sep  4, 2019
  * Add support for setting timeout for convenience methods in DNS.lazy
  * Fixed DNS.req resulttype error format (LP: #1842423)
  * Use errno.EADDRINUSE instead of the hard coded Linux value for improved
    portability (LP: #1793540)
  * Update test suite to correct for use of no longer existing DNS records
  * Set timeout=1 for tests so testing with a non-responsive nameserver will
```

### Comparing `py3dns-3.2.1/DNS/Base.py` & `py3dns-4.0.0/DNS/Base.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
     Base functionality. Request and Response classes, that sort of thing.
 """
 
 import socket, string, types, time, select
 import errno
 from . import Type,Class,Opcode
-import asyncore
 #
 # This random generator is used for transaction ids and port selection.  This
 # is important to prevent spurious results from lost packets, and malicious
 # cache poisoning.  This doesn't matter if you are behind a caching nameserver
 # or your app is a primary DNS server only. To install your own generator,
 # replace DNS.Base.random.  SystemRandom uses /dev/urandom or similar source.  
 #
@@ -46,16 +45,20 @@
 
 defaults= { 'protocol':'udp', 'port':53, 'opcode':Opcode.QUERY,
             'qtype':Type.A, 'rd':1, 'timing':1, 'timeout': 30, 'server_rotate': 0,
             'server': [] }
 
 def ParseResolvConf(resolv_path="/etc/resolv.conf"):
     "parses the /etc/resolv.conf file and sets defaults for name servers"
-    with open(resolv_path, 'r') as stream:
-        return ParseResolvConfFromIterable(stream)
+    try:
+        with open(resolv_path, 'r') as stream:
+            return ParseResolvConfFromIterable(stream)
+    except FileNotFoundError:
+        return(defaults['server'].append('127.0.0.1'))
+
 
 def ParseResolvConfFromIterable(lines):
     "parses a resolv.conf formatted stream and sets defaults for name servers"
     global defaults
     for line in lines:
         line = line.strip()
         if not line or line[0]==';' or line[0]=='#':
@@ -90,15 +93,14 @@
     """
     pass
 
 class DnsRequest:
     """ high level Request object """
     def __init__(self,*name,**args):
         self.donefunc=None
-        self.py3async=None
         self.defaults = {}
         self.argparse(name,args)
         self.defaults = self.args
         self.tid = 0
         self.resulttype = ''
         if len(self.defaults['server']) == 0:
             raise DNSError('No working name servers discovered')
@@ -270,18 +272,15 @@
         try:
             if protocol == 'udp':
                 self.sendUDPRequest(server)
             else:
                 self.sendTCPRequest(server)
         except socket.error as reason:
             raise SocketError(reason)
-        if self.py3async:
-            return None
-        else:
-            return self.response
+        return self.response
 
     def req(self,*name,**args):
         " needs a refactoring "
         self.argparse(name,args)
         #if not self.args:
         #    raise ArgumentError, 'reinitialize request before reuse'
         try:
@@ -322,18 +321,15 @@
         try:
             if protocol == 'udp':
                 self.sendUDPRequest(server)
             else:
                 self.sendTCPRequest(server)
         except socket.error as reason:
             raise SocketError(reason)
-        if self.py3async:
-            return None
-        else:
-            return self.response
+        return self.response
 
     def sendUDPRequest(self, server):
         "refactor me"
         first_socket_error = None
         self.response=None
         for self.ns in server:
             try:
@@ -343,29 +339,26 @@
                     else: continue
                 else:
                     self.socketInit(socket.AF_INET, socket.SOCK_DGRAM)
                 try:
                     # TODO. Handle timeouts &c correctly (RFC)
                     self.time_start=time.time()
                     self.conn()
-                    if not self.py3async:
-                        self.s.send(self.request)
+                    self.s.send(self.request)
+                    r=self.processUDPReply()
+                    # Since we bind to the source port and connect to the
+                    # destination port, we don't need to check that here,
+                    # but do make sure it's actually a DNS request that the
+                    # packet is in reply to.
+                    while (r.header['id'] != self.tid or
+                            self.from_address[1] != self.port):
                         r=self.processUDPReply()
-                        # Since we bind to the source port and connect to the
-                        # destination port, we don't need to check that here,
-                        # but do make sure it's actually a DNS request that the
-                        # packet is in reply to.
-                        while r.header['id'] != self.tid        \
-                                or self.from_address[1] != self.port:
-                            r=self.processUDPReply()
-                        self.response = r
-                        # FIXME: check waiting async queries
+                    self.response = r
                 finally:
-                    if not self.py3async:
-                        self.s.close()
+                    self.s.close()
             except socket.error as e:
                 # Keep trying more nameservers, but preserve the first error
                 # that occurred so it can be reraised in case none of the
                 # servers worked:
                 first_socket_error = first_socket_error or e
                 continue
             except TimeoutError as t:
@@ -414,48 +407,14 @@
                 first_socket_error = first_socket_error or t
                 continue
             if self.response:
                 break
         if not self.response and first_socket_error:
             raise first_socket_error
 
-#class DnsAsyncRequest(DnsRequest):
-class DnsAsyncRequest(DnsRequest,asyncore.dispatcher_with_send):
-    " an asynchronous request object. out of date, probably broken "
-    def __init__(self,*name,**args):
-        DnsRequest.__init__(self, *name, **args)
-        # XXX todo
-        if 'done' in args and args['done']:
-            self.donefunc=args['done']
-        else:
-            self.donefunc=self.showResult
-        #self.realinit(name,args) # XXX todo
-        self.py3async=1
-    def conn(self):
-        self.getSource()
-        self.connect((self.ns,self.port))
-        self.time_start=time.time()
-        if 'start' in self.args and self.args['start']:
-            asyncore.dispatcher.go(self)
-    def socketInit(self,a,b):
-        self.create_socket(a,b)
-        asyncore.dispatcher.__init__(self)
-        self.s=self
-    def handle_read(self):
-        if self.args['protocol'] == 'udp':
-            self.response=self.processUDPReply()
-            if self.donefunc:
-                self.donefunc(*(self,))
-    def handle_connect(self):
-        self.send(self.request)
-    def handle_write(self):
-        pass
-    def showResult(self,*s):
-        self.response.show()
-
 def ParseOSXSysConfig():
     "Retrieves the current Mac OS X resolver settings using the scutil(8) command."
     import os, re
     scutil = os.popen('/usr/sbin/scutil --dns', 'r')
     res_re = re.compile('^\s+nameserver[]0-9[]*\s*\:\s*(\S+)$')
     sets = [ ]
     currentset = None
```

### Comparing `py3dns-3.2.1/DNS/Class.py` & `py3dns-4.0.0/DNS/Class.py`

 * *Files identical despite different names*

### Comparing `py3dns-3.2.1/DNS/Lib.py` & `py3dns-4.0.0/DNS/Lib.py`

 * *Files identical despite different names*

### Comparing `py3dns-3.2.1/DNS/Opcode.py` & `py3dns-4.0.0/DNS/Opcode.py`

 * *Files identical despite different names*

### Comparing `py3dns-3.2.1/DNS/Status.py` & `py3dns-4.0.0/DNS/Status.py`

 * *Files identical despite different names*

### Comparing `py3dns-3.2.1/DNS/Type.py` & `py3dns-4.0.0/DNS/Type.py`

 * *Files identical despite different names*

### Comparing `py3dns-3.2.1/DNS/__init__.py` & `py3dns-4.0.0/DNS/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # Changes for Python3 port © 2011 Scott Kitterman <scott@kitterman.com>
 #
 # This code is covered by the standard Python License. See LICENSE for details.
 
 # __init__.py for DNS class.
 
-__version__ = '3.2.1'
+__version__ = '4.0.0'
 
 try:
     import ipaddress
 except ImportError:
     try:
         import ipaddr as ipaddress
     except ImportError:
```

### Comparing `py3dns-3.2.1/DNS/lazy.py` & `py3dns-4.0.0/DNS/lazy.py`

 * *Files identical despite different names*

### Comparing `py3dns-3.2.1/DNS/tests/testPackers.py` & `py3dns-4.0.0/DNS/tests/testPackers.py`

 * *Files identical despite different names*

### Comparing `py3dns-3.2.1/DNS/tests/test_base.py` & `py3dns-4.0.0/DNS/tests/test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         self.assertEqual(aaaab_response.answers[0]['data'],b'&\x06(\x00\x02 \x00\x01\x02H\x18\x93%\xc8\x19F')
         # IPv6 decimal
         aaaai_response = dnsobj.qry(qtype='AAAA', resulttype='integer', timeout=1)
         self.assertTrue(aaaai_response.answers)
         self.assertEqual(aaaai_response.answers[0]['data'], 50542628918019813867414319910101719366)
 
     def testDnsRequestEmptyMX(self):
-        dnsobj = DNS.DnsRequest('example.org')
+        dnsobj = DNS.DnsRequest('mail.kitterman.org')
 
         mx_empty_response = dnsobj.qry(qtype='MX', timeout=1)
         self.assertFalse(mx_empty_response.answers)
 
     def testDnsRequestMX(self):
         dnsobj = DNS.DnsRequest('ietf.org')
         mx_response = dnsobj.qry(qtype='MX', timeout=1)
@@ -181,15 +181,15 @@
         # does the result look like a binary ipv6 address?
         self.assertEqual(len(aaaad_response.answers[0]['data']) , 16)
         for b in aaaad_response.answers[0]['data']:
             assertIsByte(b)
         self.assertEqual(aaaad_response.answers[0]['data'],b'&\x06(\x00\x02 \x00\x01\x02H\x18\x93%\xc8\x19F')
         
     def testDnsRequestEmptyMXD(self):
-        dnsob = DNS.DnsRequest('example.org')
+        dnsob = DNS.DnsRequest('mail.kitterman.org')
 
         mx_empty_response = dnsob.req(qtype='MX', timeout=1)
         self.assertFalse(mx_empty_response.answers)
 
     def testDnsRequestMXD(self):
         dnsob = DNS.DnsRequest('ietf.org')
         mx_response = dnsob.req(qtype='MX', timeout=1)
```

### Comparing `py3dns-3.2.1/DNS/win32dns.py` & `py3dns-4.0.0/DNS/win32dns.py`

 * *Files identical despite different names*

### Comparing `py3dns-3.2.1/LICENSE` & `py3dns-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py3dns-3.2.1/README-guido.txt` & `py3dns-4.0.0/README-guido.txt`

 * *Files identical despite different names*

### Comparing `py3dns-3.2.1/README.txt` & `py3dns-4.0.0/README.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Release 4.0.0 UNRELEASED
+Removed class DnsAsyncRequest since Python 3.12 dropped asyncore.  Bumping
+major version since this is a breaking change.  If you need async DNS, use
+aiodns instead.
+
+Changed behavior when /etc/resolv.conf is missing.  Instead of
+FileNotFoundError, assume DNS server is '127.0.0.1'.
+
 Release 3.2.0 Mon Jul 23 2018
 
 Switched from distutils to setuptools because "it's the future".  It is
 unlikely to have end user impact.  For python3.3+ no additional dependencies
 are required.
 
 Release 3.1.0 Thu Apr 24 23:52:00 EDT 2014
```

### Comparing `py3dns-3.2.1/tests/test.py` & `py3dns-4.0.0/tests/test.py`

 * *Files identical despite different names*

### Comparing `py3dns-3.2.1/tests/test5.py` & `py3dns-4.0.0/tests/test5.py`

 * *Files identical despite different names*

### Comparing `py3dns-3.2.1/tests/test6.py` & `py3dns-4.0.0/tests/test6.py`

 * *Files identical despite different names*

### Comparing `py3dns-3.2.1/tests/test7.py` & `py3dns-4.0.0/tests/test7.py`

 * *Files identical despite different names*

### Comparing `py3dns-3.2.1/tools/caching.py` & `py3dns-4.0.0/tools/caching.py`

 * *Files identical despite different names*

### Comparing `py3dns-3.2.1/tools/named-perf.py` & `py3dns-4.0.0/tools/named-perf.py`

 * *Files identical despite different names*

