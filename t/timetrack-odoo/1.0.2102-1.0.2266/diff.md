# Comparing `tmp/timetrack-odoo-1.0.2102.tar.gz` & `tmp/timetrack-odoo-1.0.2266.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/timetrack-odoo-1.0.2102.tar", last modified: Tue Mar  7 22:28:04 2023, max compression
+gzip compressed data, was "dist/timetrack-odoo-1.0.2266.tar", last modified: Sat Jul  1 10:03:02 2023, max compression
```

## Comparing `timetrack-odoo-1.0.2102.tar` & `timetrack-odoo-1.0.2266.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 guidod    (1001) root         (0)        0 2023-03-07 22:28:04.000000 timetrack-odoo-1.0.2102/
--rw-r--r--   0 guidod    (1001) root         (0)    11357 2023-03-05 10:17:39.000000 timetrack-odoo-1.0.2102/LICENSE
--rw-r--r--   0 guidod    (1001) root         (0)     2206 2023-03-07 22:28:04.000000 timetrack-odoo-1.0.2102/PKG-INFO
--rw-r--r--   0 guidod    (1001) root         (0)     1598 2023-03-07 22:28:04.000000 timetrack-odoo-1.0.2102/README
--rw-r--r--   0 guidod    (1001) root         (0)     3145 2023-03-05 22:04:59.000000 timetrack-odoo-1.0.2102/README.md
--rwxr-xr-x   0 guidod    (1001) root         (0)     5557 2023-03-07 22:26:16.000000 timetrack-odoo-1.0.2102/dotgitconfig.py
--rwxr-xr-x   0 guidod    (1001) root         (0)    19806 2023-03-07 01:38:46.000000 timetrack-odoo-1.0.2102/dotnetrc.py
--rwxr-xr-x   0 guidod    (1001) root         (0)    25395 2023-03-07 22:26:16.000000 timetrack-odoo-1.0.2102/jira2data.py
--rwxr-xr-x   0 guidod    (1001) root         (0)     9711 2023-03-07 22:26:16.000000 timetrack-odoo-1.0.2102/jira2data_api.py
--rwxr-xr-x   0 guidod    (1001) root         (0)    29646 2023-03-07 22:26:16.000000 timetrack-odoo-1.0.2102/odoo2data.py
--rwxr-xr-x   0 guidod    (1001) root         (0)    27065 2023-03-07 22:26:16.000000 timetrack-odoo-1.0.2102/odoo2data_api.py
--rwxr-xr-x   0 guidod    (1001) root         (0)    11479 2023-03-07 22:26:16.000000 timetrack-odoo-1.0.2102/odootopic.py
--rw-r--r--   0 guidod    (1001) root         (0)     1303 2023-03-07 22:28:04.000000 timetrack-odoo-1.0.2102/setup.cfg
--rwxr-xr-x   0 guidod    (1001) root         (0)       60 2023-03-07 22:28:04.000000 timetrack-odoo-1.0.2102/setup.py
--rwxr-xr-x   0 guidod    (1001) root         (0)    11073 2023-03-07 22:26:16.000000 timetrack-odoo-1.0.2102/tabtools.py
--rwxr-xr-x   0 guidod    (1001) root         (0)    59013 2023-03-07 22:26:16.000000 timetrack-odoo-1.0.2102/tabtotext.py
--rwxr-xr-x   0 guidod    (1001) root         (0)     9235 2023-03-07 22:26:16.000000 timetrack-odoo-1.0.2102/tabtoxlsx.py
--rwxr-xr-x   0 guidod    (1001) root         (0)    15192 2023-03-07 22:26:16.000000 timetrack-odoo-1.0.2102/timerange.py
--rwxr-xr-x   0 guidod    (1001) root         (0)    22488 2023-03-07 22:26:16.000000 timetrack-odoo-1.0.2102/timetrack.py
-drwxr-xr-x   0 guidod    (1001) root         (0)        0 2023-03-07 22:28:04.000000 timetrack-odoo-1.0.2102/timetrack_odoo.egg-info/
--rw-r--r--   0 guidod    (1001) root         (0)     2206 2023-03-07 22:28:04.000000 timetrack-odoo-1.0.2102/timetrack_odoo.egg-info/PKG-INFO
--rw-r--r--   0 guidod    (1001) root         (0)      436 2023-03-07 22:28:04.000000 timetrack-odoo-1.0.2102/timetrack_odoo.egg-info/SOURCES.txt
--rw-r--r--   0 guidod    (1001) root         (0)        1 2023-03-07 22:28:04.000000 timetrack-odoo-1.0.2102/timetrack_odoo.egg-info/dependency_links.txt
--rw-r--r--   0 guidod    (1001) root         (0)       18 2023-03-07 22:28:04.000000 timetrack-odoo-1.0.2102/timetrack_odoo.egg-info/requires.txt
--rw-r--r--   0 guidod    (1001) root         (0)        1 2023-03-07 22:28:04.000000 timetrack-odoo-1.0.2102/timetrack_odoo.egg-info/top_level.txt
--rwxr-xr-x   0 guidod    (1001) root         (0)    19738 2023-03-07 22:26:16.000000 timetrack-odoo-1.0.2102/zeit2jira.py
--rwxr-xr-x   0 guidod    (1001) root         (0)    24697 2023-03-07 22:26:16.000000 timetrack-odoo-1.0.2102/zeit2json.py
--rwxr-xr-x   0 guidod    (1001) root         (0)    30794 2023-03-07 22:26:16.000000 timetrack-odoo-1.0.2102/zeit2odoo.py
+drwxr-xr-x   0 guidod    (1001) root         (0)        0 2023-07-01 10:03:02.000000 timetrack-odoo-1.0.2266/
+-rw-r--r--   0 guidod    (1001) root         (0)    11357 2023-03-05 10:17:39.000000 timetrack-odoo-1.0.2266/LICENSE
+-rw-r--r--   0 guidod    (1001) root         (0)     2197 2023-07-01 10:03:02.000000 timetrack-odoo-1.0.2266/PKG-INFO
+-rw-r--r--   0 guidod    (1001) root         (0)     1597 2023-07-01 10:03:01.000000 timetrack-odoo-1.0.2266/README
+-rw-r--r--   0 guidod    (1001) root         (0)     3249 2023-03-07 22:31:20.000000 timetrack-odoo-1.0.2266/README.md
+-rwxr-xr-x   0 guidod    (1001) root         (0)     5701 2023-07-01 09:52:00.000000 timetrack-odoo-1.0.2266/dotgitconfig.py
+-rwxr-xr-x   0 guidod    (1001) root         (0)    25726 2023-07-01 09:52:00.000000 timetrack-odoo-1.0.2266/dotnetrc.py
+-rwxr-xr-x   0 guidod    (1001) root         (0)    25483 2023-07-01 09:52:00.000000 timetrack-odoo-1.0.2266/jira2data.py
+-rwxr-xr-x   0 guidod    (1001) root         (0)     9711 2023-07-01 09:52:00.000000 timetrack-odoo-1.0.2266/jira2data_api.py
+-rwxr-xr-x   0 guidod    (1001) root         (0)    37800 2023-07-01 09:52:00.000000 timetrack-odoo-1.0.2266/odoo2data.py
+-rwxr-xr-x   0 guidod    (1001) root         (0)    27751 2023-07-01 09:52:00.000000 timetrack-odoo-1.0.2266/odoo2data_api.py
+-rwxr-xr-x   0 guidod    (1001) root         (0)    11684 2023-07-01 09:52:00.000000 timetrack-odoo-1.0.2266/odootopic.py
+-rw-r--r--   0 guidod    (1001) root         (0)     1303 2023-07-01 10:03:02.000000 timetrack-odoo-1.0.2266/setup.cfg
+-rwxr-xr-x   0 guidod    (1001) root         (0)       60 2023-07-01 10:03:01.000000 timetrack-odoo-1.0.2266/setup.py
+-rwxr-xr-x   0 guidod    (1001) root         (0)    11842 2023-07-01 09:52:00.000000 timetrack-odoo-1.0.2266/tabtools.py
+-rwxr-xr-x   0 guidod    (1001) root         (0)    60527 2023-07-01 09:52:00.000000 timetrack-odoo-1.0.2266/tabtotext.py
+-rwxr-xr-x   0 guidod    (1001) root         (0)     9919 2023-07-01 09:52:00.000000 timetrack-odoo-1.0.2266/tabtoxlsx.py
+-rwxr-xr-x   0 guidod    (1001) root         (0)    15891 2023-07-01 09:52:00.000000 timetrack-odoo-1.0.2266/timerange.py
+-rwxr-xr-x   0 guidod    (1001) root         (0)    22523 2023-07-01 09:52:00.000000 timetrack-odoo-1.0.2266/timetrack.py
+drwxr-xr-x   0 guidod    (1001) root         (0)        0 2023-07-01 10:03:02.000000 timetrack-odoo-1.0.2266/timetrack_odoo.egg-info/
+-rw-r--r--   0 guidod    (1001) root         (0)     2197 2023-07-01 10:03:02.000000 timetrack-odoo-1.0.2266/timetrack_odoo.egg-info/PKG-INFO
+-rw-r--r--   0 guidod    (1001) root         (0)      436 2023-07-01 10:03:02.000000 timetrack-odoo-1.0.2266/timetrack_odoo.egg-info/SOURCES.txt
+-rw-r--r--   0 guidod    (1001) root         (0)        1 2023-07-01 10:03:02.000000 timetrack-odoo-1.0.2266/timetrack_odoo.egg-info/dependency_links.txt
+-rw-r--r--   0 guidod    (1001) root         (0)       18 2023-07-01 10:03:02.000000 timetrack-odoo-1.0.2266/timetrack_odoo.egg-info/requires.txt
+-rw-r--r--   0 guidod    (1001) root         (0)        1 2023-07-01 10:03:02.000000 timetrack-odoo-1.0.2266/timetrack_odoo.egg-info/top_level.txt
+-rwxr-xr-x   0 guidod    (1001) root         (0)    19826 2023-07-01 09:52:00.000000 timetrack-odoo-1.0.2266/zeit2jira.py
+-rwxr-xr-x   0 guidod    (1001) root         (0)    24832 2023-07-01 09:52:00.000000 timetrack-odoo-1.0.2266/zeit2json.py
+-rwxr-xr-x   0 guidod    (1001) root         (0)    30884 2023-07-01 09:52:00.000000 timetrack-odoo-1.0.2266/zeit2odoo.py
```

### Comparing `timetrack-odoo-1.0.2102/LICENSE` & `timetrack-odoo-1.0.2266/LICENSE`

 * *Files identical despite different names*

### Comparing `timetrack-odoo-1.0.2102/PKG-INFO` & `timetrack-odoo-1.0.2266/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: timetrack-odoo
-Version: 1.0.2102
+Version: 1.0.2266
 Summary: Synchronize odoo-import data with Odoo Timesheet and Jira Worklogs
 Home-page: https://github.com/gdraheim/timetrack-odoo
 Author: Guido U. Draheim
 Author-email: Guido.Draheim@gmx.de
 License: APL
 Description: 
-        
         ## TIMETRACK ODOO (and JIRA Worklogs and more)
         
         Timetrack is a synchronisation tool for work hours. It can read, write and
         update different data bases.
         
         * [Odoo Timesheet](https://www.odoo.com/app/timesheet-features) via REST API
         * [Jira Issue Worklogs](https://confluence.atlassian.com/jirasoftwareserver/logging-work-on-issues-939938944.html) via REST API
```

### Comparing `timetrack-odoo-1.0.2102/README` & `timetrack-odoo-1.0.2266/README`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 
-
 ## TIMETRACK ODOO (and JIRA Worklogs and more)
 
 Timetrack is a synchronisation tool for work hours. It can read, write and
 update different data bases.
 
 * [Odoo Timesheet](https://www.odoo.com/app/timesheet-features) via REST API
 * [Jira Issue Worklogs](https://confluence.atlassian.com/jirasoftwareserver/logging-work-on-issues-939938944.html) via REST API
```

### Comparing `timetrack-odoo-1.0.2102/README.md` & `timetrack-odoo-1.0.2266/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![Style Check](https://github.com/gdraheim/timetrack-odoo/actions/workflows/stylecheck.yml/badge.svg?event=push&branch=main)](https://github.com/gdraheim/timetrack-odoo/actions/workflows/stylecheck.yml)
 [![Type Check](https://github.com/gdraheim/timetrack-odoo/actions/workflows/typecheck.yml/badge.svg?event=push&branch=main)](https://github.com/gdraheim/timetrack-odoo/actions/workflows/typecheck.yml)
 [![Unit Tests](https://img.shields.io/badge/basic%20unit%20tests-578%20tests-brightgreen)](https://github.com/gdraheim/timetrack-odoo/actions/workflows/unittests.yml)
-
+[![PyPI version](https://badge.fury.io/py/timetrack-odoo.svg)](https://pypi.org/project/timetrack-odoo/)
 
 ## TIMETRACK ODOO (and JIRA Worklogs and more)
 
 Timetrack is a synchronisation tool for work hours. It can read, write and
 update different data bases.
 
 * [Odoo Timesheet](https://www.odoo.com/app/timesheet-features) via REST API
```

### Comparing `timetrack-odoo-1.0.2102/dotgitconfig.py` & `timetrack-odoo-1.0.2266/dotgitconfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python3
 import dotnetrc
 """ This is a wrapper around dotnetrc.py which can read the git-credentials store,
     adding functions to read the the gitconfig settings alternativly. """
 
 __copyright__ = "(C) 2021-2023 Guido Draheim, licensed under the Apache License 2.0"""
-__version__ = "1.1.2102"
+__version__ = "1.1.2266"
 
 from typing import List, Dict, Tuple, Optional
 
 import logging
 import sys
 import os
 import os.path as _path
@@ -96,24 +96,25 @@
     git_config_overrides[section][key] = value
     gitconfig_logg.debug("[%s][%s] = '%s' # %s", section, key, value, line.strip())
 
 if __name__ == "__main__":
     from optparse import OptionParser
     o = OptionParser("%prog [-u username] [-p password] url...")
     o.formatter.max_help_position = 30
-    o.add_option("-v", "--verbose", action="count", default=0)
+    o.add_option("-v", "--verbose", action="count", default=0, help="more verbose logging")
+    o.add_option("-^", "--quiet", action="count", default=0, help="less verbose logging")
     o.add_option("-u", "--username", metavar="NAME", default=GITRC_USERNAME)
     o.add_option("-p", "--password", metavar="PASS", default=GITRC_PASSWORD)
     o.add_option("-g", "--gitcredentials", metavar="FILE", default=GIT_CREDENTIALS)
     o.add_option("-G", "--extracredentials", metavar="FILE", default=NETRC_FILENAME)
     o.add_option("-C", "--gitconfig", metavar="FILE", default=GIT_CONFIG)
     o.add_option("-c", "--config", metavar="NAME=VALUE", action="append", default=[])
     o.add_option("-y", "--cleartext", action="store_true", default=False)
     opt, args = o.parse_args()
-    logging.basicConfig(level=logging.WARNING - 10 * opt.verbose)
+    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose + 10 * opt.quiet))
     GIT_CONFIG = opt.gitconfig
     for value in opt.config:
         git_config_override(value)
     dotnetrc.GIT_CREDENTIALS = opt.gitcredentials
     add_password_filename(opt.extracredentials)
     dotnetrc.NETRC_USERNAME = opt.username
     dotnetrc.NETRC_PASSWORD = opt.password
```

### Comparing `timetrack-odoo-1.0.2102/dotnetrc.py` & `timetrack-odoo-1.0.2266/dotnetrc.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 """ This function can store username/password tuples either as default or specific
 for a root url. It follows in style the dot-netc model from BSD and actually the
 code does inspect ~/.netrc for matching entries if a url is specified. The script
 can also read the ~/.git-credentials format. Even a mix of entries is possible
 where extensions should only be used in a ~/.net-credentials filename. ////
 Use command './dotnetrc.py set <url> <name> <pass>' to write entries."""
 
+__version__ = "0.4.2266"
+
 # dot git-credentials format:
 #   https://<username>:<password>@<hostname>
 #
 # dot netrc format:
 #   machine <hostname> login <username> password <password> protocol <http>
 #   machine <hostname> login <username> password <password>
 #   machine <hostname> password <password>
@@ -54,14 +56,16 @@
 
 NETRC_OVERRIDE: Dict[str, Tuple[str, str]] = OrderedDict()
 NET_CREDENTIALS = "~/.net-credentials"
 GIT_CREDENTIALS = "~/.git-credentials"
 NETRC_FILENAME = "~/.netrc"
 NETRC_FILENAMES = [GIT_CREDENTIALS, NETRC_FILENAME]
 
+NETRC_CRYPT = "46"
+
 def _target(url: str) -> str:
     if "://" not in url:
         url = f"https://{url}"
     machine = _urlparse(url)
     port = ""
     if machine.port and machine.port not in [80, 443]:
         port = f":{machine.port}"
@@ -86,20 +90,98 @@
     return codecs.decode(codecs.decode(text.encode('ascii')[::-1], 'base64'), 'utf-8')
 def _encode36(text: str) -> str:
     """ echo -n pw | base64 | rev | tr A-Za-z M-ZA-Nm-za-n """
     # return codecs.decode(codecs.encode(codecs.encode(text.encode('utf-8'), 'base64'), 'rot13')[::-1], 'ascii').strip()
     return codecs.encode(codecs.decode(codecs.encode(text.encode('utf-8'), 'base64'), 'ascii')[::-1], 'rot13').strip()
 def _decode36(text: str) -> str:
     return codecs.decode(codecs.decode(codecs.decode(text, 'rot13').encode('ascii')[::-1], 'base64'), 'utf-8')
-def _decode(text: str, encoding: str) -> str:
+def _encode32(text: str) -> str:
+    return codecs.decode(codecs.encode(cryptData(text.encode('utf-8')), 'base64').replace(b"\n", b""), 'ascii')
+def _decode32(text: str) -> str:
+    return codecs.decode(decryptData(codecs.decode(text.encode('ascii'), 'base64')), 'utf-8')
+
+def _decode(text: str, encoding: Optional[str] = None) -> str:
+    encoding = encoding if encoding is not None else NETRC_CRYPT
     if encoding.endswith("64"): return _decode64(text).strip()
     if encoding.endswith("63"): return _decode63(text).strip()
     if encoding.endswith("46"): return _decode46(text).strip()
     if encoding.endswith("36"): return _decode36(text).strip()
+    if encoding.endswith("32"): return _decode32(text).strip()
     return text
+def _encode(text: str, encoding: Optional[str] = None) -> str:
+    encoding = encoding if encoding is not None else NETRC_CRYPT
+    if encoding.endswith("64"): return _encode64(text).strip()
+    if encoding.endswith("63"): return _encode63(text).strip()
+    if encoding.endswith("46"): return _encode46(text).strip()
+    if encoding.endswith("36"): return _encode36(text).strip()
+    if encoding.endswith("32"): return _encode32(text).strip()
+    return text
+
+# ...............................................................................................................
+if os.name in ['nt']:
+    # https://stackoverflow.com/questions/463832/using-dpapi-with-python
+    # DPAPI access library
+    # This file uses code originally created by Crusher Joe:
+    # http://article.gmane.org/gmane.comp.python.ctypes/420
+    #
+
+    from ctypes import *
+    from ctypes.wintypes import DWORD
+
+    LocalFree = windll.kernel32.LocalFree  # type: ignore[name-defined]
+    memcpy = cdll.msvcrt.memcpy  # type: ignore[name-defined]
+    CryptProtectData = windll.crypt32.CryptProtectData  # type: ignore[name-defined]
+    CryptUnprotectData = windll.crypt32.CryptUnprotectData  # type: ignore[name-defined]
+    CRYPTPROTECT_UI_FORBIDDEN = 0x01
+    extraEntropy = b"cl;ad13 \0al;323kjd #(adl;k$#ajsd"
+
+    class DATA_BLOB(Structure):
+        _fields_ = [("cbData", DWORD), ("pbData", POINTER(c_char))]
+
+    def getData(blobOut: DATA_BLOB) -> bytes:
+        cbData = int(blobOut.cbData)
+        pbData = blobOut.pbData
+        buffer = c_buffer(cbData)
+        memcpy(buffer, pbData, cbData)
+        LocalFree(pbData)
+        return buffer.raw
+
+    def Win32CryptProtectData(plainText: bytes, entropy: bytes) -> bytes:
+        bufferIn = c_buffer(plainText, len(plainText))
+        blobIn = DATA_BLOB(len(plainText), bufferIn)
+        bufferEntropy = c_buffer(entropy, len(entropy))
+        blobEntropy = DATA_BLOB(len(entropy), bufferEntropy)
+        blobOut = DATA_BLOB()
+
+        if CryptProtectData(byref(blobIn), u"python_data", byref(blobEntropy),
+                            None, None, CRYPTPROTECT_UI_FORBIDDEN, byref(blobOut)):
+            return getData(blobOut)
+        else:
+            return b""
+
+    def Win32CryptUnprotectData(cipherText: bytes, entropy: bytes) -> bytes:
+        bufferIn = c_buffer(cipherText, len(cipherText))
+        blobIn = DATA_BLOB(len(cipherText), bufferIn)
+        bufferEntropy = c_buffer(entropy, len(entropy))
+        blobEntropy = DATA_BLOB(len(entropy), bufferEntropy)
+        blobOut = DATA_BLOB()
+        if CryptUnprotectData(byref(blobIn), None, byref(blobEntropy), None, None,
+                              CRYPTPROTECT_UI_FORBIDDEN, byref(blobOut)):
+            return getData(blobOut)
+        else:
+            return b""
+
+    def cryptData(text: bytes) -> bytes:
+        return Win32CryptProtectData(text, extraEntropy)
+
+    def decryptData(cipher_text: bytes) -> bytes:
+        return Win32CryptUnprotectData(cipher_text, extraEntropy)
+
+    NETRC_CRYPT = '32'
+# ...............................................................................................................
 
 def set_username_password(username: str, password: str) -> Tuple[str, str]:
     global NETRC_USERNAME, NETRC_PASSWORD
     if ":" in username:
         NETRC_PASSWORD = username.split(':', 1)[1]
         NETRC_USERNAME = username.split(':', 1)[0]
     else:
@@ -204,15 +286,15 @@
         return self.search(_target(url))
     def search(self, target: str) -> Optional[Tuple[str, str]]:
         return self._search(target, self.FILENAME)
     def _search(self, target: str, filename: str) -> Optional[Tuple[str, str]]:
         netrc = _path.expanduser(filename)
         block = ""
         if _path.isfile(netrc):
-            if os.stat(netrc).st_mode & 0o77:
+            if os.stat(netrc).st_mode & 0o77 and os.name not in ['nt']:
                 netrc_logg.warning(" !! netrc file should be private - chmod 600 %s", netrc)
             netrc_logg.debug("looking for 'machine %s' in %s", target, netrc)
             with open(netrc) as f:
                 netrc_text = f.read()
             matches: Dict[str, Tuple[str, str, str]] = {}
             for line in (netrc_text + "\ndefault").splitlines():
                 if not line.strip() or line.strip().startswith("#"):
@@ -346,16 +428,17 @@
     if os.path.isfile(filename):
         with open(filename) as f:
             for line in f:
                 if _fnmatch(line, matching0) or _fnmatch(line, matching1):
                     continue  # delete
                 lines.append(line.rstrip())
     with open(filename, "w") as f:
-        password46 = _encode46(password)
-        f.write(f"machine {machine} login {username} password46 {password46}\n")
+        crypt: str = NETRC_CRYPT
+        cryptpassword = _encode(password, crypt)
+        f.write(f"machine {machine} login {username} password{crypt} {cryptpassword}\n")
         for line in lines:
             if line.strip():
                 f.write(line + "\n")
     os.chmod(filename, 0o600)
     return filename
 
 def erase_username_password(url: str) -> str:
@@ -375,57 +458,94 @@
             if line.strip():
                 f.write(line + "\n")
     os.chmod(filename, 0o600)
     return filename
 
 if __name__ == "__main__":
     from optparse import OptionParser
-    o = OptionParser("%prog [-u username] [-p password] url | SET url name pass", epilog=__doc__)
-    o.formatter.max_help_position = 36
-    o.add_option("-v", "--verbose", action="count", default=0)
-    o.add_option("-u", "--username", metavar="NAME", default=NETRC_USERNAME, help="fallback to default user")
-    o.add_option("-p", "--password", metavar="PASS", default=NETRC_PASSWORD, help="fallback to default pass")
-    o.add_option("-f", "--fromcredentials", metavar="FILE", default="", help="scan this instead of:")
-    o.add_option("-N", "--netcredentials", metavar="FILE", default=NET_CREDENTIALS, help="[%default]")
-    o.add_option("-g", "--gitcredentials", metavar="FILE", default=GIT_CREDENTIALS, help="[%default]")
-    o.add_option("-G", "--extracredentials", metavar="FILE", default=NETRC_FILENAME, help="[%default]")
-    o.add_option("-e", "--extrafile", metavar="NAME", default="")
-    o.add_option("-y", "--cleartext", action="store_true", default=NETRC_CLEARTEXT)
-    o.add_option("--as-ac", action="store_true", help="show as '-a user -c pass'")
-    o.add_option("--as-up", action="store_true", help="show as '-u user -p pass'")
-    opt, args = o.parse_args()
-    logging.basicConfig(level=logging.WARNING - 10 * opt.verbose)
+    cmdline = OptionParser("%prog [-u username] [-p password] url | HELP | DEL url | SET url name pass", epilog=__doc__, version=__version__)
+    cmdline.formatter.max_help_position = 36
+    cmdline.add_option("-v", "--verbose", action="count", default=0, help="more verbose logging")
+    cmdline.add_option("-^", "--quiet", action="count", default=0, help="less verbose logging")
+    cmdline.add_option("-u", "--username", metavar="NAME", default=NETRC_USERNAME, help="fallback to default user")
+    cmdline.add_option("-p", "--password", metavar="PASS", default=NETRC_PASSWORD, help="fallback to default pass")
+    cmdline.add_option("-f", "--fromcredentials", metavar="FILE", default="", help="scan this instead of:")
+    cmdline.add_option("-N", "--netcredentials", metavar="FILE", default=NET_CREDENTIALS, help="[%default]")
+    cmdline.add_option("-g", "--gitcredentials", metavar="FILE", default=GIT_CREDENTIALS, help="[%default]")
+    cmdline.add_option("-G", "--extracredentials", metavar="FILE", default=NETRC_FILENAME, help="[%default]")
+    cmdline.add_option("-e", "--extrafile", metavar="NAME", default="")
+    cmdline.add_option("-y", "--cleartext", action="store_true", default=NETRC_CLEARTEXT)
+    cmdline.add_option("-2", "--crypt32", action="store_true", default=False, help="use win32crypt (default if available)")
+    cmdline.add_option("-3", "--crypt36", action="store_true", default=False, help="use triple obfuscation with rot13")
+    cmdline.add_option("-4", "--crypt46", action="store_true", default=False, help="use double obfuscation with rev")
+    cmdline.add_option("-6", "--crypt64", action="store_true", default=False, help="use single obfuscation with base64")
+    cmdline.add_option("-9", "--nocrypt", action="store_true", default=False, help="use no obfusction for passwords")
+    cmdline.add_option("-a", "--as-username", action="store_true", help="as  '--username user --password pass'")
+    cmdline.add_option("--as-user", action="store_true", help="show as '--user user --password pass'")
+    cmdline.add_option("--as-ac", action="store_true", help="show as '-a user -c pass'")
+    cmdline.add_option("--as-up", action="store_true", help="show as '-u user -p pass'")
+    cmdline.add_option("--as-u", action="store_true", help="show as '-u user:pass'")
+    opt, args = cmdline.parse_args()
+    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose + 10 * opt.quiet))
     if opt.fromcredentials:
         NET_CREDENTIALS = opt.fromcredentials
         net_password_filename(opt.fromcredentials)
     else:
         GIT_CREDENTIALS = opt.gitcredentials
         NET_CREDENTIALS = opt.netcredentials
         net_password_filename(opt.netcredentials)
         set_password_filename(opt.gitcredentials)
     add_password_filename(opt.extracredentials)
     NETRC_USERNAME = opt.username
     NETRC_PASSWORD = opt.password
     NETRC_CLEARTEXT = opt.cleartext
-    NET_AS_AC = opt.as_ac
-    NET_AS_UP = opt.as_up
+    if opt.nocrypt:
+        NETRC_CRYPT = ""
+    if opt.crypt46:
+        NETRC_CRYPT = "64"
+    if opt.crypt46:
+        NETRC_CRYPT = "46"
+    if opt.crypt36:
+        NETRC_CRYPT = "36"
+    if opt.crypt32:
+        NETRC_CRYPT = "32"
     if not args:
         args = ["help"]
+    elif len(args) == 1 and "." in args[0]:
+        args = ["GET"] + args
+    elif len(args) >= 3 and "." in args[0]:
+        args = ["SET"] + args
     cmd = args[0]
-    if cmd in ["help"]:
-        print(__doc__)
+    if cmd in ["help", "HELP"]:
+        cmdline.print_help()
+        print("\nCommands:")
+        previous = ""
+        for line in open(__file__):
+            if previous.strip().replace("elif cmd", "if cmd").startswith("if cmd in"):
+                if "#" in line:
+                    print(previous.strip().split(" cmd in")[1], line.strip().split("#")[1])
+                else:
+                    print(previous.strip().split(" cmd in")[1], line.strip())
+            previous = line
+        raise SystemExit()
     elif cmd in ["get", "find", "for", "GET"]:
         uselogin = get_username_password(args[1])
         if not uselogin: sys.exit(1)
         hostpath = _target(args[1]).split("/", 1) + [""]
         # printing in the style of https://git-scm.com/docs/git-credential
-        if opt.as_ac:
+        if opt.as_username:
+            print(" --username " + uselogin[0] + " --password " + uselogin[1])
+        elif opt.as_user:
+            print(" --user " + uselogin[0] + " --password " + uselogin[1])
+        elif opt.as_ac:
             print(" -a " + uselogin[0] + " -c " + uselogin[1])
         elif opt.as_up:
             print(" -u " + uselogin[0] + " -p " + uselogin[1])
+        elif opt.as_u:
+            print(" -u " + uselogin[0] + ":" + uselogin[1])
         else:
             if hostpath[0]: print("host=" + hostpath[0])
             if hostpath[1]: print("path=" + hostpath[1])
             if uselogin[0]: print("username=" + uselogin[0])
             if uselogin[1]: print("password=" + uselogin[1])
         print("")
     elif cmd in ["store", "write", "set", "SET"]:
```

### Comparing `timetrack-odoo-1.0.2102/jira2data.py` & `timetrack-odoo-1.0.2266/jira2data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python3
 """
 Read and format Jira worklog entries. Provides additional reports.
 """
 
 __copyright__ = "(C) 2022-2023 Guido Draheim, licensed under the Apache License 2.0"""
-__version__ = "0.4.2102"
+__version__ = "0.4.2266"
 
 from typing import Union, Dict, List, Any, Optional, Tuple, Iterable, Iterator, cast
 from requests import Session, Response, HTTPError
 from requests.packages.urllib3.exceptions import InsecureRequestWarning   # type: ignore[import]
 import warnings
 import logging
 import json
@@ -502,18 +502,18 @@
             import tabtoxlsx
             tabtoxlsx.saveToXLSX(XLSXFILE, result, sorts=sortby)
             logg.log(DONE, " %s written  %s %s", FMT, viewFMT(FMT), XLSXFILE)
     return 0
 
 if __name__ == "__main__":
     from optparse import OptionParser
-    cmdline = OptionParser("%prog [options] [help|zeit|odoo|summary|projects|tickets]", epilog=__doc__)
+    cmdline = OptionParser("%prog [-options] [help|commands..]", epilog=__doc__, version=__version__)
     cmdline.formatter.max_help_position = 30
-    cmdline.add_option("-v", "--verbose", action="count", default=0,
-                       help="more verbose logging")
+    cmdline.add_option("-v", "--verbose", action="count", default=0, help="more verbose logging")
+    cmdline.add_option("-^", "--quiet", action="count", default=0, help="less verbose logging")
     cmdline.add_option("-r", "--remote", metavar="URL", default="",
                        help="url to Jira API endpoint (or gitconfig jira.url)")
     cmdline.add_option("-a", "--after", metavar="DATE", default=None,
                        help="only evaluate entrys on and after [first of month]")
     cmdline.add_option("-b", "--before", metavar="DATE", default=None,
                        help="only evaluate entrys on and before [last of month]")
     cmdline.add_option("-j", "--project", metavar="JIRA", action="append", default=PROJECTS,
@@ -527,15 +527,15 @@
     cmdline.add_option("-m", "--taskdata", metavar="PATH", default=TASKDATA, help="use odootopic mapping file")
     cmdline.add_option("-q", "--dryrun", action="count", default=0)
     cmdline.add_option("-Q", "--shortdesc", action="count", default=SHORTDESC,
                        help="present short lines for description [%default]")
     cmdline.add_option("-U", "--user", metavar="NAME", default=NIX,
                        help="filter for user [%default]")
     opt, args = cmdline.parse_args()
-    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose))
+    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose + 10 * opt.quiet))
     warnings.simplefilter("once", InsecureRequestWarning)
     SHORTDESC = opt.shortdesc
     DRYRUN = opt.dryrun
     DAYS = dayrange(opt.after, opt.before)
     PROJECTS = opt.project
     LABELS = ",".join(opt.labels)
     FORMAT = opt.format
```

### Comparing `timetrack-odoo-1.0.2102/jira2data_api.py` & `timetrack-odoo-1.0.2266/jira2data_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python3
 """
 Interface to Jira as a method to read and store worklog entries
 """
 
 __copyright__ = "(C) 2022-2023 Guido Draheim, licensed under the Apache License 2.0"""
-__version__ = "0.4.2102"
+__version__ = "0.4.2266"
 
 from typing import Union, Dict, List, Any, Optional, Tuple, Iterable, Iterator, cast
 from requests import Session, Response, HTTPError
 import warnings
 import logging
 import json
 import os
```

### Comparing `timetrack-odoo-1.0.2102/odoo2data.py` & `timetrack-odoo-1.0.2266/odoo2data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python3
 """
 Read and format Odoo timesheet entries. Provides extra reports.
 """
 
 __copyright__ = "(C) 2021-2023 Guido Draheim, licensed under the Apache License 2.0"""
-__version__ = "1.0.2102"
+__version__ = "1.0.2266"
 
 from typing import Optional, Union, Dict, List, Tuple, cast, Iterable, Iterator
 
 import logging
 import re
 import os
 import csv
@@ -52,34 +52,49 @@
 LABELS = ""
 FORMAT = ""
 OUTPUT = ""
 JSONFILE = ""
 XLSXFILE = ""
 
 EURO = "euro"
+NIX = ""
 
 def strName(value: JSONItem) -> str:
     if value is None:
         return "~"
     val = str(value)
     if SHORTNAME:
         if len(val) > 27:
             return val[:17] + "..." + val[-7:]
     return val
 
-def get_proj_price_rate(proj: str) -> int:
+def get_proj_price_rate(proj: str, task: str = NIX) -> int:
     rate = 0
-    for price in PRICES:
-        if ":" in price:
-            proj_name, proj_rate = price.split(":", 1)
-            proj_pattern = (proj_name if "*" in proj_name else proj_name + "*")
-            if fnmatches(proj, proj_pattern):
-                rate = int(proj_rate)
-        else:
-            rate = int(price)
+    if task:
+        for price in PRICES:
+            if ":" in price:
+                proj_task, proj_rate = price.split(":", 1)
+                if "@" not in proj_task: continue
+                proj_name, task_name = proj_task.split("@", 1)
+                proj_pattern = (proj_name if "*" in proj_name else proj_name + "*")
+                task_pattern = (task_name if "*" in task_name else "*" + task_name + "*")
+                if fnmatches(proj, proj_pattern) and fnmatches(task, task_pattern):
+                    rate = int(proj_rate)
+            else:
+                rate = int(price)
+    if not rate:
+        for price in PRICES:
+            if ":" in price:
+                proj_name, proj_rate = price.split(":", 1)
+                if "@" in proj_name: continue
+                proj_pattern = (proj_name if "*" in proj_name else proj_name + "*")
+                if fnmatches(proj, proj_pattern):
+                    rate = int(proj_rate)
+            else:
+                rate = int(price)
     if not rate:
         gitrc_price = git_config_value("zeit.price")
         if gitrc_price:
             rate = int(gitrc_price)
     if not rate:
         rate = PRICE10  # ensure that price is not a copy of hours
     return rate
@@ -286,20 +301,67 @@
     return _summary_per_day(odoodata)
 def _summary_per_day(odoodata: JSONList) -> JSONList:
     daydata: Dict[Day, JSONDict] = {}
     for item in odoodata:
         odoo_date: Day = get_date(cast(str, item["entry_date"]))
         odoo_size: Num = cast(Num, item["entry_size"])
         weekday = odoo_date.isoweekday()
-        weekday_name = ["so", "mo", "di", "mi", "do", "fr", "sa", "so", "mo"][weekday + 1]
+        weekday_name = WEEKDAYS[weekday]
         if odoo_date not in daydata:
             daydata[odoo_date] = {"date": odoo_date, "day": weekday_name, "odoo": 0}
         daydata[odoo_date]["odoo"] += odoo_size  # type: ignore
     return list(daydata.values())
 
+def user2(name: str, m: int) -> str:
+    if " " in name:
+        n = name.split(" ")
+        return n[0][0] + n[-1][0]
+    else:
+        return str(m) + n[0]
+def reports_per_day(odoodata: Optional[JSONList] = None) -> JSONList:
+    if odoodata:
+        m = 0
+        logg.info("%s: zeit", m)
+        result = _report_per_day(odoodata, user=user2(".", m))
+        users = FOR_USER
+    else:
+        result = []
+        users = FOR_USER if FOR_USER else [""]
+    for m, user in enumerate(users):
+        logg.info("%i: %s", m + 1, user)
+        odoo = odoo_api.Odoo().for_user(user)
+        odoodata = odoo.timesheet(DAYS.after, DAYS.before)
+        result += _report_per_day(odoodata, user=user2(user, m + 1))
+    return sorted(result, key=lambda r: (r["date"], r["at proj"], r["user"]))
+def _report_per_day(odoodata: JSONList, user: str = ":") -> JSONList:
+    work_sep = " / "
+    daydata: Dict[Tuple[Day, str], JSONDict] = {}
+    for item in odoodata:
+        odoo_date: Day = get_date(cast(str, item["entry_date"]))
+        odoo_size: Num = cast(Num, item["entry_size"])
+        odoo_work: str = cast(str, item["entry_desc"])
+        odoo_proj: str = cast(str, item["proj_name"])
+        odoo_task: str = cast(str, item["task_name"])
+        if ODOO_PROJONLY:
+            if not fnmatches(odoo_proj, ODOO_PROJONLY): continue
+        if ODOO_PROJSKIP:
+            if fnmatches(odoo_proj, ODOO_PROJSKIP): continue
+        weekday = odoo_date.isoweekday()
+        weekday_name = WEEKDAYS[weekday]
+        key = (odoo_date, odoo_proj)
+        if key not in daydata:
+            daydata[key] = {"date": odoo_date, "day": weekday_name,
+                            "at proj": odoo_proj,
+                            "odoo": 0, "user": user, "work": ""}
+        daydata[key]["odoo"] += odoo_size  # type: ignore
+        if daydata[key]["work"]:
+            daydata[key]["work"] += work_sep  # type: ignore
+        daydata[key]["work"] += odoo_work  # type: ignore
+    return list(daydata.values())
+
 def summary_per_project_task(odoodata: Optional[JSONList] = None) -> JSONList:
     if not odoodata:
         odoo = odoo_api.Odoo().for_user(FOR_USER[0] if FOR_USER else "")
         odoodata = odoo.timesheet(DAYS.after, DAYS.before)
     return _summary_per_project_task(odoodata)
 def _summary_per_project_task(odoodata: JSONList) -> JSONList:
     sumdata: Dict[Tuple[str, str], JSONDict] = {}
@@ -363,14 +425,82 @@
         odoo_size = cast(float, item["odoo"])
         price_rate = get_proj_price_rate(proj_name)
         elem: JSONDict = {"am": new_month, "at proj": proj_name, "odoo": odoo_size, "m": focus,
                           "satz": int(price_rate), "summe": round(price_rate * odoo_size, 2)}
         sumvals.append(elem)
     return sumvals
 
+def reports_per_project_task(odoodata: Optional[JSONList] = None) -> JSONList:
+    if odoodata:
+        m = 0
+        logg.info("%s: zeit", m)
+        result = _report_per_project_task(odoodata, focus=m)
+        users = FOR_USER
+    else:
+        result = []
+        users = FOR_USER if FOR_USER else [""]
+    for m, user in enumerate(users):
+        logg.info("%i: %s", m + 1, user)
+        odoo = odoo_api.Odoo().for_user(user)
+        odoodata = odoo.timesheet(DAYS.after, DAYS.before)
+        result += _report_per_project_task(odoodata, focus=m + 1)
+    return sorted(result, key=lambda r: (r["am"], r["at proj"], r["m"]))
+def report_per_project_task(odoodata: Optional[JSONList] = None) -> JSONList:
+    if not odoodata:
+        odoo = odoo_api.Odoo().for_user(FOR_USER[0] if FOR_USER else "")
+        odoodata = odoo.timesheet(DAYS.after, DAYS.before)
+    return _report_per_project_task(odoodata)
+def _report_per_project_task(odoodata: JSONList, focus: int = 0) -> JSONList:
+    sumdata = _monthly_per_project_task(odoodata)
+    sumvals: JSONList = []
+    for item in sumdata:
+        new_month = cast(str, item["am"])
+        proj_name = cast(str, item["at proj"])
+        task_name = cast(str, item["at task"])
+        odoo_size = cast(float, item["odoo"])
+        price_rate = get_proj_price_rate(proj_name, task_name)
+        elem: JSONDict = {"am": new_month, "at proj": proj_name, "at task": task_name, "odoo": odoo_size, "m": focus,
+                          "satz": int(price_rate), "summe": round(price_rate * odoo_size, 2)}
+        sumvals.append(elem)
+    return sumvals
+
+def reports_per_project_topic(odoodata: Optional[JSONList] = None) -> JSONList:
+    if odoodata:
+        m = 0
+        logg.info("%s: zeit", m)
+        result = _report_per_project_topic(odoodata, focus=m)
+        users = FOR_USER
+    else:
+        result = []
+        users = FOR_USER if FOR_USER else [""]
+    for m, user in enumerate(users):
+        logg.info("%i: %s", m + 1, user)
+        odoo = odoo_api.Odoo().for_user(user)
+        odoodata = odoo.timesheet(DAYS.after, DAYS.before)
+        result += _report_per_project_topic(odoodata, focus=m + 1)
+    return sorted(result, key=lambda r: (r["am"], r["at proj"], r["m"]))
+def report_per_project_topic(odoodata: Optional[JSONList] = None) -> JSONList:
+    if not odoodata:
+        odoo = odoo_api.Odoo().for_user(FOR_USER[0] if FOR_USER else "")
+        odoodata = odoo.timesheet(DAYS.after, DAYS.before)
+    return _report_per_project_topic(odoodata)
+def _report_per_project_topic(odoodata: JSONList, focus: int = 0) -> JSONList:
+    sumdata = _monthly_per_project_topic(odoodata)
+    sumvals: JSONList = []
+    for item in sumdata:
+        new_month = cast(str, item["am"])
+        proj_name = cast(str, item["at proj"])
+        task_pref = cast(str, item["at topic"])
+        odoo_size = cast(float, item["odoo"])
+        price_rate = get_proj_price_rate(proj_name, task_pref)
+        elem: JSONDict = {"am": new_month, "at proj": proj_name, "at topic": task_pref, "odoo": odoo_size, "m": focus,
+                          "satz": int(price_rate), "summe": round(price_rate * odoo_size, 2)}
+        sumvals.append(elem)
+    return sumvals
+
 def monthly_per_project(odoodata: Optional[JSONList] = None) -> JSONList:
     if not odoodata:
         odoo = odoo_api.Odoo().for_user(FOR_USER[0] if FOR_USER else "")
         odoodata = odoo.timesheet(DAYS.after, DAYS.before)
     return _monthly_per_project(odoodata)
 def _monthly_per_project(odoodata: JSONList) -> JSONList:
     sumdata = _monthly_per_project_task(odoodata)
@@ -407,14 +537,41 @@
         if ODOO_PROJSKIP:
             if fnmatches(proj_name, ODOO_PROJSKIP): continue
         if odoo_key not in sumdata:
             sumdata[odoo_key] = {"am": odoo_month, "at proj": proj_name, "at task": task_name, "odoo": 0, "zeit": 0}
         sumdata[odoo_key]["odoo"] += odoo_size  # type: ignore
     return list(sumdata.values())
 
+def monthly_per_project_topic(odoodata: Optional[JSONList] = None) -> JSONList:
+    if not odoodata:
+        odoo = odoo_api.Odoo().for_user(FOR_USER[0] if FOR_USER else "")
+        odoodata = odoo.timesheet(DAYS.after, DAYS.before)
+    return _monthly_per_project_topic(odoodata)
+def _monthly_per_project_topic(odoodata: JSONList) -> JSONList:
+    sumdata: Dict[Tuple[str, str, str], JSONDict] = {}
+    for item in odoodata:
+        proj_name: str = cast(str, item["proj_name"])
+        odoo_desc: str = cast(str, item["entry_desc"])
+        odoo_date: Day = get_date(cast(str, item["entry_date"]))
+        odoo_size: Num = cast(Num, item["entry_size"])
+        task_pref: str = pref_desc(odoo_desc)
+        if ADDFOOTER > 1:
+            odoo_month = "M%02i.%04i" % (odoo_date.month, odoo_date.year)
+        else:
+            odoo_month = "M%02i" % odoo_date.month
+        odoo_key = (odoo_month, proj_name, task_pref)
+        if ODOO_PROJONLY:
+            if not fnmatches(proj_name, ODOO_PROJONLY): continue
+        if ODOO_PROJSKIP:
+            if fnmatches(proj_name, ODOO_PROJSKIP): continue
+        if odoo_key not in sumdata:
+            sumdata[odoo_key] = {"am": odoo_month, "at proj": proj_name, "at topic": task_pref, "odoo": 0, "zeit": 0}
+        sumdata[odoo_key]["odoo"] += odoo_size  # type: ignore
+    return list(sumdata.values())
+
 def fnmatches(text: str, pattern: str) -> bool:
     for pat in pattern.split("|"):
         if pat.isalnum() and pat.islower():
             if fnmatch(text.lower(), f"*{pat}*"):
                 return True
         else:
             if fnmatch(text, pat + "*"):
@@ -519,14 +676,22 @@
             with open(filename, "w") as f:
                 f.write(tabtotext.tabToFMT("wide", results))
             summary += ["zeit.txt data written to %s" % filename]
         else:
             summary += ["file did already exist: %s" % filename]
     elif arg in ["dd", "dsummary", "days"]:
         results = summary_per_day(data)
+    elif arg in ["tx", "taskreport"]:
+        results = report_per_project_task(data)  # group by Odoo project, per month and add price column
+    elif arg in ["pxx", "topicreports"]:
+        results = reports_per_project_topic(data)  # group by Odoo project, per month and add price column
+    elif arg in ["px", "topicreport"]:
+        results = report_per_project_topic(data)  # group by Odoo project, per month and add price column
+    elif arg in ["txx", "taskreports"]:
+        results = reports_per_project_task(data)  # group by Odoo project, per month and add price column
     elif arg in ["xx", "report"]:
         results = report_per_project(data)  # group by Odoo project, per month and add price column
         sum_euro = sum([float(cast(JSONBase, item["summe"])) for item in results if item["summe"]])
         sum_odoo = sum([float(cast(JSONBase, item["odoo"])) for item in results if item["odoo"]])
         summary = [f"{sum_euro:11.2f} {EURO} summe", f"{sum_odoo:11.2f} hours odoo"]
         if results and not ADDFOOTER:
             summary += [" ### use -Z to add a VAT footer !!"]
@@ -537,14 +702,18 @@
         sum_euro = sum([float(cast(JSONBase, item["summe"])) for item in results if item["summe"]])
         sum_odoo = sum([float(cast(JSONBase, item["odoo"])) for item in results if item["odoo"]])
         summary = [f"{sum_euro:11.2f} {EURO} summe", f"{sum_odoo:11.2f} hours odoo"]
         if results and not ADDFOOTER:
             summary += [" ### use -Z to add a VAT footer !!"]
         formats["summe"] = "{:$}"
         formats["satz"] = "{:4.2f}"
+    elif arg in ["dx", "dayreports"]:
+        results = reports_per_day(data)  # group by Odoo project, per month, add price and m column
+    elif arg in ["mt", "mtopic", "mtopics"]:
+        results = monthly_per_project_topic(data)  # group by Odoo project-and-task, seperate per month
     elif arg in ["mm", "msummarize", "mtasks", "monthlys"]:
         results = monthly_per_project_task(data)  # group by Odoo project-and-task, seperate per month
     elif arg in ["sx", "msummary", "monthly"]:
         results = monthly_per_project(data)  # group by Odoo project but keep sums seperate per month
         sum_odoo = sum([float(cast(JSONBase, item["odoo"])) for item in results if item["odoo"]])
         summary = [f"{sum_odoo:11.2f} hours odoo"]
     elif arg in ["ee", "summarize", "tasks"]:
@@ -603,18 +772,18 @@
             FMT = "xlsx"
             import tabtoxlsx
             tabtoxlsx.saveToXLSX(XLSXFILE, results, formats=formats, reorder=reorder)
             logg.log(DONE, " %s written   %s '%s'", FMT, viewFMT(FMT), XLSXFILE)
 
 if __name__ == "__main__":
     from optparse import OptionParser
-    cmdline = OptionParser("%prog [help|zeit|odoo|work|days|summarize|summary|topics|users|projects|tasks]", epilog=__doc__)
+    cmdline = OptionParser("%prog [-options] [help|commands...]", epilog=__doc__, version=__version__)
     cmdline.formatter.max_help_position = 30
-    cmdline.add_option("-v", "--verbose", action="count", default=0,
-                       help="more verbose logging")
+    cmdline.add_option("-v", "--verbose", action="count", default=0, help="more verbose logging")
+    cmdline.add_option("-^", "--quiet", action="count", default=0, help="less verbose logging")
     cmdline.add_option("-a", "--after", metavar="DATE", default=None,
                        help="only evaluate entrys on and after date")
     cmdline.add_option("-b", "--before", metavar="DATE", default=None,
                        help="only evaluate entrys on and before date")
     cmdline.add_option("-p", "--price", metavar="TEXT", action="append", default=PRICES,
                        help="pattern:price per hour [%default]")
     cmdline.add_option("--projskip", metavar="TEXT", default=ODOO_PROJSKIP,
@@ -637,16 +806,16 @@
     cmdline.add_option("-g", "--gitcredentials", metavar="FILE", default=dotnetrc.GIT_CREDENTIALS)
     cmdline.add_option("-G", "--netcredentials", metavar="FILE", default=dotnetrc.NET_CREDENTIALS)
     cmdline.add_option("-E", "--extracredentials", metavar="FILE", default=dotnetrc.NETRC_FILENAME)
     cmdline.add_option("-c", "--config", metavar="NAME=VALUE", action="append", default=[])
     cmdline.add_option("-u", "--user", metavar="NAME", action="append", default=[],
                        help="show data for other users than the login user (use full name or email)")
     opt, args = cmdline.parse_args()
-    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose))
-    logg.setLevel(level=max(0, logging.WARNING - 10 * opt.verbose))
+    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose + 10 * opt.quiet))
+    logg.setLevel(level=max(0, logging.WARNING - 10 * opt.verbose + 10 * opt.quiet))
     # logg.addHandler(logging.StreamHandler())
     for value in opt.config:
         git_config_override(value)
     dotnetrc.set_password_filename(opt.gitcredentials)
     dotnetrc.add_password_filename(opt.netcredentials, opt.extracredentials)
     FOR_USER = opt.user
     LABELS = ",".join(opt.labels)
```

### Comparing `timetrack-odoo-1.0.2102/odoo2data_api.py` & `timetrack-odoo-1.0.2266/odoo2data_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/env python3
 
 __copyright__ = "(C) 2021-2023 Guido Draheim, licensed under the Apache License 2.0"""
-__version__ = "0.7.2102"
+__version__ = "0.7.2266"
 
 import logging
 from typing import List, Dict, Union, Optional, Tuple, Any, cast
 
 import sys
 import re
 import os.path as path
@@ -638,14 +638,26 @@
             if ondate == before:
                 break
             ondate += datetime.timedelta(days=1)
         return records
 
 ###########################################################################################
 def run(arg: str) -> None:
+    if arg in ["help"]:
+        cmdline.print_help()
+        print("\nCommands:")
+        previous = ""
+        for line in open(__file__):
+            if previous.strip().replace("elif arg", "if arg").startswith("if arg in"):
+                if "#" in line:
+                    print(previous.strip().split(" arg in")[1], line.strip().split("#")[1])
+                else:
+                    print(previous.strip().split(" arg in")[1], line.strip())
+            previous = line
+        raise SystemExit()
     if arg in ["dbs", "databases"]:
         odoo = Odoo()
         logg.info(" ODOO URL %s DB %s", odoo.url, odoo.db)
         print(", ".join(odoo.databases()))
     if arg in ["pjs", "projects"]:
         odoo = Odoo()
         logg.info(" ODOO URL %s DB %s", odoo.url, odoo.db)
@@ -666,21 +678,22 @@
         print(text)
 
 def reset() -> None:
     pass  # only defined in the mockup
 
 if __name__ == "__main__":
     from optparse import OptionParser
-    cmdline = OptionParser("%prog [options] command...")
+    cmdline = OptionParser("%prog [-options] [help|commands...]", version=__version__)
+    cmdline.add_option("-v", "--verbose", action="count", default=0, help="more verbose logging")
+    cmdline.add_option("-^", "--quiet", action="count", default=0, help="less verbose logging")
     cmdline.add_option("-g", "--gitcredentials", metavar="FILE", default="~/.netrc")
-    cmdline.add_option("-v", "--verbose", action="count", default=0)
     cmdline.add_option("-d", "--db", metavar="name", default=ODOO_DB)
     cmdline.add_option("-e", "--url", metavar="url", default=ODOO_URL)
     opt, args = cmdline.parse_args()
-    logging.basicConfig(level=logging.WARNING - 10 * opt.verbose)
+    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose + 10 * opt.quiet))
     dotnetrc.set_password_filename(opt.gitcredentials)
     ODOO_URL = opt.url
     ODOO_DB = opt.db
     if not args:
         args = ["projects"]
     for arg in args:
         run(arg)
```

### Comparing `timetrack-odoo-1.0.2102/odootopic.py` & `timetrack-odoo-1.0.2266/odootopic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #! /usr/bin/env python3
+""" associates topics with Odoo project+task coordinates """
 
 __copyright__ = "(C) 2022-2023 Guido Draheim, licensed under the Apache License 2.0"""
-__version__ = "0.8.2102"
+__version__ = "0.8.2266"
 
 from typing import List, Dict, Union, Optional, Tuple, Iterator, Iterable, cast
 
 import logging
 import re
 import csv
 import datetime
@@ -242,27 +243,27 @@
 
 def run(filename: str) -> None:
     results = mapping(open(filename))
     print(tabtotext.tabToGFM(list(results)))
 
 if __name__ == "__main__":
     from optparse import OptionParser
-    cmdline = OptionParser("%prog files...")
+    cmdline = OptionParser("%prog files...", epilog=__doc__, version=__version__)
     cmdline.formatter.max_help_position = 30
-    cmdline.add_option("-v", "--verbose", action="count", default=0,
-                       help="more verbose logging")
+    cmdline.add_option("-v", "--verbose", action="count", default=0, help="more verbose logging")
+    cmdline.add_option("-^", "--quiet", action="count", default=0, help="less verbose logging")
     cmdline.add_option("-a", "--after", metavar="DATE", default="",
                        help="only evaluate entrys on and after [first of year]")
     cmdline.add_option("-b", "--before", metavar="DATE", default="",
                        help="only evaluate entrys on and before [last of year]")
     cmdline.add_option("-f", "--filename", metavar="TEXT", default="",
                        help="choose input filename [may be path/zeit{YEAR}.txt]")
     opt, args = cmdline.parse_args()
-    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose))
-    logg.setLevel(level=max(0, logging.WARNING - 10 * opt.verbose))
+    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose + 10 * opt.quiet))
+    logg.setLevel(level=max(0, logging.WARNING - 10 * opt.verbose + 10 * opt.quiet))
     #
     import zeit2json
     zeit2json.ZEIT_FILENAME = opt.filename
     zeit2json.ZEIT_AFTER = opt.after
     zeit2json.ZEIT_BEFORE = opt.before
     if not args:
         args = [zeit2json.get_zeit_filename()]
```

### Comparing `timetrack-odoo-1.0.2102/setup.cfg` & `timetrack-odoo-1.0.2266/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = timetrack-odoo
-version = 1.0.2102
+version = 1.0.2266
 license = APL
 license_files = 
 	LICENSE
 author = Guido U. Draheim
 author-email = Guido.Draheim@gmx.de
 home-page = https://github.com/gdraheim/timetrack-odoo
 description = Synchronize odoo-import data with Odoo Timesheet and Jira Worklogs
```

### Comparing `timetrack-odoo-1.0.2102/tabtools.py` & `timetrack-odoo-1.0.2266/tabtools.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Implements frac formatting, for example three-quarter of an hour.
 It can also read time-like number like 12:30 into simple floats.
 And it has support for some Mi-byte input and output, so that
 arge numbers an be presented nicely and parsed back.
 """
 
 __copyright__ = "(C) 2022-2023 Guido Draheim, licensed under the Apache License 2.0"""
-__version__ = "1.5.2102"
+__version__ = "1.5.2266"
 
 from typing import Any, cast, Union
 import string
 import re
 import logging
 
 logg = logging.getLogger("fracfloat")
@@ -309,12 +309,24 @@
     line = line.replace("JP$", chr(currency_yen))
     line = line.replace("CN$", chr(currency_yen))
     line = line.replace("BP$", chr(currency_pound))
     line = line.replace("PD$", chr(currency_pound))
     return line
 
 if __name__ == "__main__":
-    import sys
+    import sys, os
+    from optparse import OptionParser
+    cmdline = OptionParser("%prog [--longoptions] text...", add_help_option=False, epilog=__doc__, version=__version__)
+    cmdline.add_option("--help", action="count", default=0, help="show this help message and exit")
+    cmdline.add_option("--verbose", action="count", default=0, help="more verbose logging")
+    cmdline.add_option("--quiet", action="count", default=0, help="less verbose logging")
+    opts = [arg for arg in sys.argv[1:] if arg.startswith("--")]
+    args = [arg for arg in sys.argv[1:] if arg not in opts]
+    opt, noargs = cmdline.parse_args(opts)
+    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose + 10 * opt.quiet))
+    if opt.help: 
+        cmdline.print_help()
+        raise SystemExit()
     out = []
-    for arg in sys.argv[1:]:
+    for arg in args:
         out.append(encodeFrac(arg))
     print(" ".join(out))
```

### Comparing `timetrack-odoo-1.0.2102/tabtotext.py` & `timetrack-odoo-1.0.2266/tabtotext.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python3
 """
 This script allows to format table-like data (list of dicts).
 The various output formats can be read back.
 """
 
 __copyright__ = "(C) 2017-2023 Guido Draheim, licensed under the Apache License 2.0"""
-__version__ = "1.6.2102"
+__version__ = "1.6.2266"
 
 from typing import Optional, Union, Dict, List, Any, Sequence, Callable, Collection, Sized, Type, cast, Iterable, Iterator
 from collections import OrderedDict
 from html import escape
 from datetime import date as Date
 from datetime import datetime as Time
 from datetime import timezone
@@ -53,16 +53,19 @@
 JSONDictList = Dict[str, JSONList]
 JSONDictDict = Dict[str, JSONDict]
 
 # dataclass support
 
 class DataItem:
     """ Use this as the base class for dataclass types """
-    def __index__(self, name: str) -> JSONItem:
+    def __getitem__(self, name: str) -> JSONItem:
         return cast(JSONItem, getattr(self, name))
+    def replace(self, **values:  str) -> JSONDict:
+        return _dataitem_replace(self, values)  # type: ignore[arg-type]
+
 DataList = List[DataItem]
 
 def _is_dataitem(obj: Any) -> bool:
     if isinstance(obj, DataItem):
         return True
     if hasattr(obj, '__dataclass_fields__'):
         return True
@@ -71,14 +74,23 @@
     if hasattr(obj, "keys"):
         return cast(JSONDict, obj)
     result: JSONDict = dict_factory()
     annotations: Dict[str, str] = obj.__class__.__dict__.get('__annotations__', {})
     for name in annotations:
         result[name] = cast(JSONItem, getattr(obj, name))
     return result
+def _dataitem_replace(obj: DataItem, values: JSONDict, dict_factory: Type[Dict[str, Any]] = dict) -> JSONDict:
+    result: JSONDict = dict_factory()
+    annotations: Dict[str, str] = obj.__class__.__dict__.get('__annotations__', {})
+    for name in annotations:
+        if name in values:
+            result[name] = values[name]
+        else:
+            result[name] = cast(JSONItem, getattr(obj, name))
+    return result
 
 # helper functions
 
 _None_String = "~"
 _False_String = "(no)"
 _True_String = "(yes)"
 
@@ -321,31 +333,23 @@
                     except Exception as e:
                         logg.debug("format <%s> does not apply: %s", fmt, e)
             # only a few percent-formatting variants are supported
             if isinstance(val, float):
                 m = re.search(r"%\d(?:[.]\d)f", fmt)
                 if m:
                     try:
-                        return fmt.format(val4)
+                        return fmt % val
                     except Exception as e:
-                        logg.debug("format <%s> does not apply: %s", fmt, e)
-                # only a few percent-formatting variants are supported
-                if isinstance(val, float):
-                    m = re.search(r"%\d(?:[.]\d)f", fmt)
-                    if m:
-                        try:
-                            return fmt % val
-                        except Exception as e:
-                            logg.debug("format <%s> does not apply: %e", fmt, e)
-                if "%s" in fmt:
-                    try:
-                        return fmt % self.item(val)
-                    except Exception as e:
-                        logg.debug("format <%s> does not apply: %s", fmt, e)
-            logg.debug("bad format '%s' in col '%s'", self.formats[col], col)
+                        logg.debug("format <%s> does not apply: %e", fmt, e)
+            if "%s" in fmt:
+                try:
+                    return fmt % self.item(val)
+                except Exception as e:
+                    logg.debug("format <%s> does not apply: %s", fmt, e)
+            logg.debug("unknown format '%s' for col '%s'", fmt, col)
         if isinstance(val, float):
             return self.floatfmt % val
         return self.item(val)
 class FormatGFM(NumFormatJSONItem):
     def __init__(self, formats: Dict[str, str] = {}, tab: str = '|'):
         NumFormatJSONItem.__init__(self, formats)
         self.tab = tab
@@ -596,41 +600,56 @@
         class MyHTMLParser(html.parser.HTMLParser):
             def __init__(self, *, convert_charrefs: bool = True) -> None:
                 html.parser.HTMLParser.__init__(self, convert_charrefs=convert_charrefs)
                 self.found: List[JSONDict] = []
                 self.th: List[str] = []
                 self.td: List[JSONItem] = []
                 self.val: Optional[str] = None
+                self.th2: List[str] = []
+                self.td2: List[JSONItem] = []
+                self.val2: Optional[str] = None
             def tr(self) -> Iterator[JSONDict]:
                 found = self.found.copy()
                 self.found = []
                 for record in found:
                     yield record
             def handle_data(self, data: str) -> None:
                 tagged = self.get_starttag_text() or ""
                 if tagged.startswith("<th"):
                     self.val = data
                 if tagged.startswith("<td"):
                     self.val = data
+                if tagged.startswith("<br"):
+                    self.val2 = data
             def handle_endtag(self, tag: str) -> None:
                 if tag == "th":
                     self.th += [self.val or str(len(self.th) + 1)]
                     self.val = None
+                    if self.val2:
+                        self.th2 += [self.val2 or str(len(self.th2) + 1)]
+                        self.val2 = None
                 if tag == "td":
                     tagged = self.get_starttag_text() or ""
                     val = self.val
                     if "right" in tagged and val and val.startswith(" "):
                         val = val[1:]
                     self.td += [val]
                     self.val = None
+                    if self.val2:
+                        self.td2 += [self.val2 or str(len(self.td2) + 1)]
+                        self.val2 = None
                 if tag == "tr" and self.td:
                     made = zip(self.th, self.td)
                     item = dict(made)
+                    if self.th2:
+                        made2 = zip(self.th2, self.td2)
+                        item.update(dict(made2))
                     self.found += [item]
                     self.td = []
+                    self.td2 = []
         parser = MyHTMLParser(convert_charrefs=self.convert_charrefs)
         for row in rows:
             parser.feed(row)
             for record in parser.tr():
                 for key, val in record.items():
                     if isinstance(val, str):
                         record[key] = self.convert.toJSONItem(val)
@@ -1050,47 +1069,46 @@
         results = list(_dataitem_asdict(cast(DataItem, item)) for item in cast(List[Any], result))
     else:
         results = cast(JSONList, result)  # type: ignore[redundant-cast]
     return tabToFMT(output, results, sorts, formats, datedelim=datedelim, legend=legend)
 def tabToFMT(fmt: str, result: JSONList, sorts: RowSortList = [], formats: FormatsDict = {}, *,  #
              datedelim: str = '-', legend: LegendList = [],  #
              reorder: ColSortList = []) -> str:
-    if fmt:
-        f = fmt.lower()
-        if f in ["md", "markdown"]:
-            return tabToGFM(result=result, sorts=sorts, formats=formats, reorder=reorder)
-        if f in ["html"]:
-            return tabToHTML(result=result, sorts=sorts, formats=formats, reorder=reorder)
-        if f in ["json"]:
-            return tabToJSON(result=result, sorts=sorts, formats=formats, reorder=reorder, datedelim=datedelim)
-        if f in ["yaml"]:
-            return tabToYAML(result=result, sorts=sorts, formats=formats, reorder=reorder, datedelim=datedelim)
-        if f in ["toml"]:
-            return tabToTOML(result=result, sorts=sorts, formats=formats, reorder=reorder, datedelim=datedelim)
-        if f in ["wide"]:
-            return tabToGFM(result=result, sorts=sorts, formats=formats, reorder=reorder, tab='')
-        if f in ["text"]:
-            return tabToGFM(result=result, sorts=sorts, formats=formats, reorder=reorder, tab='', noheaders=True)
-        if f in ["tabs"]:
-            return tabToGFM(result=result, sorts=sorts, formats=formats, reorder=reorder, tab='\t')
-        if f in ["tab"]:
-            return tabToCSV(result=result, sorts=sorts, formats=formats, reorder=reorder, datedelim=datedelim, tab='\t')
-        if f in ["dat"]:
-            return tabToCSV(result=result, sorts=sorts, formats=formats, reorder=reorder, datedelim=datedelim, tab='\t', noheaders=True)
-        if f in ["ifs", "data"]:
-            return tabToCSV(result=result, sorts=sorts, formats=formats, reorder=reorder, datedelim=datedelim, tab=os.environ.get("IFS", "\t"), noheaders=True)
-        if f in ["csv"]:
-            return tabToCSV(result=result, sorts=sorts, formats=formats, reorder=reorder, datedelim=datedelim, tab=';')
-        if f in ["list"]:
-            return tabToCSV(result=result, sorts=sorts, formats=formats, reorder=reorder, datedelim=datedelim, tab=';', noheaders=True)
-        if f in ["xlsx"]:
-            return tabToCSV(result=result, sorts=sorts, formats=formats, reorder=reorder, datedelim=datedelim, tab=',')
-        if f in ["htm"]:
-            # including the legend
-            return tabToHTML(result=result, sorts=sorts, formats=formats, reorder=reorder, legend=legend)
+    fmt = fmt or ""
+    if fmt.lower() in ["md", "markdown"]:
+        return tabToGFM(result=result, sorts=sorts, formats=formats, reorder=reorder)
+    if fmt.lower() in ["html"]:
+        return tabToHTML(result=result, sorts=sorts, formats=formats, reorder=reorder)
+    if fmt.lower() in ["json"]:
+        return tabToJSON(result=result, sorts=sorts, formats=formats, reorder=reorder, datedelim=datedelim)
+    if fmt.lower() in ["yaml"]:
+        return tabToYAML(result=result, sorts=sorts, formats=formats, reorder=reorder, datedelim=datedelim)
+    if fmt.lower() in ["toml"]:
+        return tabToTOML(result=result, sorts=sorts, formats=formats, reorder=reorder, datedelim=datedelim)
+    if fmt.lower() in ["wide"]:
+        return tabToGFM(result=result, sorts=sorts, formats=formats, reorder=reorder, tab='')
+    if fmt.lower() in ["text"]:
+        return tabToGFM(result=result, sorts=sorts, formats=formats, reorder=reorder, tab='', noheaders=True)
+    if fmt.lower() in ["tabs"]:
+        return tabToGFM(result=result, sorts=sorts, formats=formats, reorder=reorder, tab='\t')
+    if fmt.lower() in ["tab"]:
+        return tabToCSV(result=result, sorts=sorts, formats=formats, reorder=reorder, datedelim=datedelim, tab='\t')
+    if fmt.lower() in ["dat"]:
+        return tabToCSV(result=result, sorts=sorts, formats=formats, reorder=reorder, datedelim=datedelim, tab='\t', noheaders=True)
+    if fmt.lower() in ["ifs", "data"]:
+        return tabToCSV(result=result, sorts=sorts, formats=formats, reorder=reorder, datedelim=datedelim, tab=os.environ.get("IFS", "\t"), noheaders=True)
+    if fmt.lower() in ["csv"]:
+        return tabToCSV(result=result, sorts=sorts, formats=formats, reorder=reorder, datedelim=datedelim, tab=';')
+    if fmt.lower() in ["list"]:
+        return tabToCSV(result=result, sorts=sorts, formats=formats, reorder=reorder, datedelim=datedelim, tab=';', noheaders=True)
+    if fmt.lower() in ["xlsx"]:
+        return tabToCSV(result=result, sorts=sorts, formats=formats, reorder=reorder, datedelim=datedelim, tab=',')
+    if fmt.lower() in ["htm"]:
+        # including the legend
+        return tabToHTML(result=result, sorts=sorts, formats=formats, reorder=reorder, legend=legend)
     return tabToGFM(result=result, sorts=sorts, formats=formats, reorder=reorder, legend=legend)
 
 def editprog() -> str:
     return os.environ.get("EDIT", "mcedit")
 def htmlprog() -> str:
     return os.environ.get("BROWSER", "chrome")
 def xlsxprog() -> str:
@@ -1324,30 +1342,43 @@
     result = readFromFMT(fileformat, filename)
     return tabToPrintWith(result, output, fmt, selects=selects, sorts=sorts, formats=formats, reorder=reorder, datedelim=datedelim, legend=legend)
 
 if __name__ == "__main__":
     DONE = (logging.WARNING + logging.ERROR) // 2
     logging.addLevelName(DONE, "DONE")
     from optparse import OptionParser
-    cmdline = OptionParser("%prog [help|data|check|valid|update|compare|summarize|summary|topics]", epilog=__doc__)
+    cmdline = OptionParser("%prog [help|filename.json|filename.html]...", epilog=__doc__, version=__version__)
     cmdline.formatter.max_help_position = 30
-    cmdline.add_option("-v", "--verbose", action="count", default=0,
-                       help="more verbose logging")
+    cmdline.add_option("-v", "--verbose", action="count", default=0, help="more verbose logging")
+    cmdline.add_option("-^", "--quiet", action="count", default=0, help="less verbose logging")
     cmdline.add_option("-S", "--sort-by", "--sort-columns", metavar="LIST", action="append",  # ..
                        help="reorder columns for sorting (a,x)", default=[])
     cmdline.add_option("-L", "--labels", "--label-columns", metavar="LIST", action="append",  # ..
                        help="select columns to show (a,x=b)", default=[])
     cmdline.add_option("-F", "--formats", "--format-columns", metavar="LIST", action="append",  # ..
                        help="apply formatting to columns (a:.2f,b:_d)", default=[])
     cmdline.add_option("-i", "--inputformat", metavar="FMT", help="fix input format (instead of autodetection)", default="")
     cmdline.add_option("-o", "--format", metavar="FMT", help="json|yaml|html|wide|md|htm|tab|csv", default="")
     cmdline.add_option("-O", "--output", metavar="CON", default="-", help="redirect output to filename")
     opt, args = cmdline.parse_args()
-    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose))
+    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose + 10 * opt.quiet))
     if not args:
         cmdline.print_help()
     else:
         for arg in args:
+            if arg in ["help"]:
+                cmdline.print_help()
+                print("\nCommands:")
+                previous = ""
+                for line in open(__file__):
+                    if previous.strip().replace("elif arg", "if arg").startswith("if arg in"):
+                        if "#" in line:
+                            print(previous.strip().split(" arg in")[1], line.strip().split("#")[1])
+                        else:
+                            print(previous.strip().split(" arg in")[1], line.strip())
+                previous = line
+                raise SystemExit()
+            # ....
             done = tabFileToPrintWith(arg, opt.inputformat, opt.output, opt.format, selects=",".join(opt.labels),  # ..
                                       sorts=",".join(opt.sort_by), formats=",".join(opt.formats))
             if done:
                 logg.log(DONE, " %s", done)
```

### Comparing `timetrack-odoo-1.0.2102/tabtoxlsx.py` & `timetrack-odoo-1.0.2266/tabtoxlsx.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """
 This script allows to format table-like data (list of dicts).
 It is sister program for tabtotext implenting excel input and output.
 """
 
 __copyright__ = "(C) 2017-2023 Guido Draheim, licensed under the Apache License 2.0"""
-__version__ = "1.6.2102"
+__version__ = "1.6.2266"
 
 import logging
 from typing import Optional, Union, Dict, List, Any, Sequence, Callable
 from tabtotext import JSONList, JSONDict, tabToGFM, strNone, strJSONItem
 from tabtotext import ColSortList, RowSortList, LegendList, FormatsDict, RowSortCallable, ColSortCallable
 
 from openpyxl import Workbook, load_workbook  # type: ignore
@@ -192,28 +192,41 @@
             data = result
         saveToXLSX(filename + ".xlsx", result, sorts=sorts, formats=formats, reorder=reorder)
         return [filename + ".xlsx", "{:3d} rows".format(len(result))]
 
     DONE = (logging.WARNING + logging.ERROR) // 2
     logging.addLevelName(DONE, "DONE")
     from optparse import OptionParser
-    cmdline = OptionParser("%prog [help|data|check|valid|update|compare|summarize|summary|topics]", epilog=__doc__)
+    cmdline = OptionParser("%prog [help|files...]", epilog=__doc__, version=__version__)
     cmdline.formatter.max_help_position = 30
-    cmdline.add_option("-v", "--verbose", action="count", default=0,
-                       help="more verbose logging")
+    cmdline.add_option("-v", "--verbose", action="count", default=0, help="more verbose logging")
+    cmdline.add_option("-^", "--quiet", action="count", default=0, help="less verbose logging")
     cmdline.add_option("-S", "--sort-by", "--sort-columns", metavar="LIST", action="append",  # ..
                        help="reorder columns for sorting (a,x)", default=[])
     cmdline.add_option("-L", "--labels", "--label-columns", metavar="LIST", action="append",  # ..
                        help="select columns to show (a,x=b)", default=[])
     cmdline.add_option("-F", "--formats", "--format-columns", metavar="LIST", action="append",  # ..
                        help="apply formatting to columns (a:.2f,b:_d)", default=[])
     cmdline.add_option("-i", "--inputformat", metavar="FMT", help="fix input format (instead of autodetection)", default="")
     opt, args = cmdline.parse_args()
-    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose))
+    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose + 10 * opt.quiet))
     if not args:
         cmdline.print_help()
     else:
         for arg in args:
+            if arg in ["help"]:
+                cmdline.print_help()
+                print("\nCommands:")
+                previous = ""
+                for line in open(__file__):
+                    if previous.strip().replace("elif arg", "if arg").startswith("if arg in"):
+                        if "#" in line:
+                            print(previous.strip().split(" arg in")[1], line.strip().split("#")[1])
+                        else:
+                            print(previous.strip().split(" arg in")[1], line.strip())
+                    previous = line
+                raise SystemExit()
+            # ....
             done = saveFileToFileXLSX(arg, opt.inputformat,  # ..
                                       selects=",".join(opt.labels), sorting=",".join(opt.sort_by), formatting=",".join(opt.formats))
             if done:
                 logg.log(DONE, " %s", " ".join(done))
```

### Comparing `timetrack-odoo-1.0.2102/timerange.py` & `timetrack-odoo-1.0.2266/timerange.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python3
 """
 Cut out from zeit2excel for after/before time ranges in days.
 Added a number of symbolic names for nearby months and weeks.
 """
 
 __copyright__ = "(C) 2022-2023 Guido Draheim, licensed under the Apache License 2.0"""
-__version__ = "0.8.2102"
+__version__ = "0.8.2266"
 
 from typing import Union, Optional, Tuple
 
 import logging
 import re
 import datetime
 
@@ -337,30 +337,42 @@
     logg.log(DONE, f"                     {ref} = after {days.after} ... {days.before} before")
     amount = len(days)
     logg.log(DONE, f"                     {dis} are {amount} days")
     return f"-a {days.after} -b {days.before}"
 
 if __name__ == "__main__":
     from optparse import OptionParser
-    cmdline = OptionParser("%prog files...", epilog=__doc__)
+    cmdline = OptionParser("%prog [-opt] [help|commands...]", epilog=__doc__, version=__version__)
     cmdline.formatter.max_help_position = 30
-    cmdline.add_option("-v", "--verbose", action="count", default=0,
-                       help="more verbose logging")
+    cmdline.add_option("-v", "--verbose", action="count", default=0, help="more verbose logging")
+    cmdline.add_option("-^", "--quiet", action="count", default=0, help="less verbose logging")
     cmdline.add_option("-a", "--after", metavar="DATE", default=None,
                        help="only evaluate on and after [first of month]")
     cmdline.add_option("-b", "--before", metavar="DATE", default=None,
                        help="only evaluate on and before [last of month]")
     opt, args = cmdline.parse_args()
-    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose))
-    logg.setLevel(level=max(0, logging.WARNING - 10 * opt.verbose))
+    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose + 10 * opt.quiet))
+    logg.setLevel(level=max(0, logging.WARNING - 10 * opt.verbose + 10 * opt.quiet))
     # logg.addHandler(logging.StreamHandler())
     ref = None
     days = dayrange(opt.after, opt.before)
     if args and is_dayrange(args[0]):
         ref = args[0]
         args = args[1:]
         days = dayrange(ref)
     if not args:
         args = ["check"]
     for arg in args:
+        if arg in ["help"]:
+            cmdline.print_help()
+            print("\nCommands:")
+            previous = ""
+            for line in open(__file__):
+                if previous.strip().replace("elif arg", "if arg").startswith("if arg in"):
+                    if "#" in line:
+                        print(previous.strip().split(" arg in")[1], line.strip().split("#")[1])
+                    else:
+                        print(previous.strip().split(" arg in")[1], line.strip())
+                previous = line
+            raise SystemExit()
         if arg in ["check"]:
             print(check_days(days, ref))
```

### Comparing `timetrack-odoo-1.0.2102/timetrack.py` & `timetrack-odoo-1.0.2266/timetrack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #! /usr/bin/env python3
+""" frontend to run other modules in the system """
 
 __copyright__ = "(C) 2019-2023 Guido Draheim, licensed under the Apache License 2.0"""
-__version__ = "0.2.2102"
+__version__ = "0.2.2266"
 
 from typing import Optional, Union, Dict, List, Tuple, Iterable, cast
 
 import logging
 import re
 import os
 import csv
@@ -473,20 +474,18 @@
             import tabtoxlsx
             tabtoxlsx.saveToXLSX(XLSXFILE, results, headers)
             logg.log(DONE, " %s written   %s '%s'", FMT, viewFMT(FMT), XLSXFILE)
     return results
 
 if __name__ == "__main__":
     from optparse import OptionParser
-    cmdline = OptionParser("%prog [help|data|check|valid|update|compare|summarize|summary|topics] files...")
+    cmdline = OptionParser("%prog [-opt] [help|command...]", epilog=__doc__, version=__version__)
     cmdline.formatter.max_help_position = 30
-    cmdline.add_option("--quiet", action="count", default=0,
-                       help="less verbose logging")
-    cmdline.add_option("-v", "--verbose", action="count", default=0,
-                       help="more verbose logging")
+    cmdline.add_option("-v", "--verbose", action="count", default=0, help="more verbose logging")
+    cmdline.add_option("-^", "--quiet", action="count", default=0, help="less verbose logging")
     cmdline.add_option("-a", "--after", metavar="DATE", default=None,
                        help="only evaluate entrys on and after data")
     cmdline.add_option("-b", "--before", metavar="DATE", default=None,
                        help="only evaluate entrys on and before date")
     cmdline.add_option("-p", "--price", metavar="TEXT", action="append", default=PRICES,
                        help="pattern:price per hour [%default]")
     cmdline.add_option("--projskip", metavar="TEXT", default=PROJSKIP,
@@ -511,16 +510,16 @@
     cmdline.add_option("-g", "--gitcredentials", metavar="FILE", default=dotnetrc.GIT_CREDENTIALS)
     cmdline.add_option("-G", "--netcredentials", metavar="FILE", default=dotnetrc.NET_CREDENTIALS)
     cmdline.add_option("-E", "--extracredentials", metavar="FILE", default=dotnetrc.NETRC_FILENAME)
     cmdline.add_option("-c", "--config", metavar="NAME=VALUE", action="append", default=[])
     cmdline.add_option("-y", "--update", action="store_true", default=UPDATE,
                        help="actually update odoo")
     opt, args = cmdline.parse_args()
-    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose))
-    logg.setLevel(level=max(0, logging.WARNING - 10 * opt.verbose))
+    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose + 10 * opt.quiet))
+    logg.setLevel(level=max(0, logging.WARNING - 10 * opt.verbose + 10 * opt.quiet))
     # logg.addHandler(logging.StreamHandler())
     for value in opt.config:
         git_config_override(value)
     dotnetrc.set_password_filename(opt.gitcredentials)
     dotnetrc.add_password_filename(opt.netcredentials, opt.extracredentials)
     config = ConfigParser()
     config.read_string(default_config(False))
```

### Comparing `timetrack-odoo-1.0.2102/timetrack_odoo.egg-info/PKG-INFO` & `timetrack-odoo-1.0.2266/timetrack_odoo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: timetrack-odoo
-Version: 1.0.2102
+Version: 1.0.2266
 Summary: Synchronize odoo-import data with Odoo Timesheet and Jira Worklogs
 Home-page: https://github.com/gdraheim/timetrack-odoo
 Author: Guido U. Draheim
 Author-email: Guido.Draheim@gmx.de
 License: APL
 Description: 
-        
         ## TIMETRACK ODOO (and JIRA Worklogs and more)
         
         Timetrack is a synchronisation tool for work hours. It can read, write and
         update different data bases.
         
         * [Odoo Timesheet](https://www.odoo.com/app/timesheet-features) via REST API
         * [Jira Issue Worklogs](https://confluence.atlassian.com/jirasoftwareserver/logging-work-on-issues-939938944.html) via REST API
```

### Comparing `timetrack-odoo-1.0.2102/zeit2jira.py` & `timetrack-odoo-1.0.2266/zeit2jira.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python3
 """
 Synchronize odoo-import data (from zeit.txt) with Jira worklog entries.
 """
 
 __copyright__ = "(C) 2022-2023 Guido Draheim, licensed under the Apache License 2.0"""
-__version__ = "0.4.2102"
+__version__ = "0.4.2266"
 
 from typing import Optional, Union, Dict, List, Tuple, Iterable, Iterator, cast
 
 import logging
 import re
 import os
 import csv
@@ -360,18 +360,18 @@
             FMT = "xlsx"
             import tabtoxlsx
             tabtoxlsx.saveToXLSX(XLSXFILE, results)
             logg.log(DONE, " %s written   %s '%s'", FMT, viewFMT(FMT), XLSXFILE)
 
 if __name__ == "__main__":
     from optparse import OptionParser
-    cmdline = OptionParser("%prog [help|data|check|valid|update|compare|summarize|summary|topics]", epilog=__doc__)
+    cmdline = OptionParser("%prog [-opt] [help|comand...]", epilog=__doc__, version=__version__)
     cmdline.formatter.max_help_position = 30
-    cmdline.add_option("-v", "--verbose", action="count", default=0,
-                       help="more verbose logging")
+    cmdline.add_option("-v", "--verbose", action="count", default=0, help="more verbose logging")
+    cmdline.add_option("-^", "--quiet", action="count", default=0, help="less verbose logging")
     cmdline.add_option("-r", "--remote", metavar="URL", default="",
                        help="url to Jira API endpoint (or gitconfig jira.url)")
     cmdline.add_option("-a", "--after", metavar="DATE", default=None,
                        help="only evaluate entrys on and after date")
     cmdline.add_option("-b", "--before", metavar="DATE", default=None,
                        help="only evaluate entrys on and before date")
     cmdline.add_option("-s", "--summary", metavar="TEXT", default=ZEIT_SUMMARY,
@@ -398,16 +398,16 @@
     cmdline.add_option("-g", "--gitcredentials", metavar="FILE", default=dotnetrc.GIT_CREDENTIALS)
     cmdline.add_option("-G", "--netcredentials", metavar="FILE", default=dotnetrc.NET_CREDENTIALS)
     cmdline.add_option("-E", "--extracredentials", metavar="FILE", default=dotnetrc.NETRC_FILENAME)
     cmdline.add_option("-c", "--config", metavar="NAME=VALUE", action="append", default=[])
     cmdline.add_option("-y", "--update", action="store_true", default=UPDATE,
                        help="actually update odoo")
     opt, args = cmdline.parse_args()
-    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose))
-    logg.setLevel(level=max(0, logging.WARNING - 10 * opt.verbose))
+    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose + 10 * opt.quiet))
+    logg.setLevel(level=max(0, logging.WARNING - 10 * opt.verbose + 10 * opt.quiet))
     # logg.addHandler(logging.StreamHandler())
     for value in opt.config:
         git_config_override(value)
     dotnetrc.set_password_filename(opt.gitcredentials)
     dotnetrc.add_password_filename(opt.netcredentials, opt.extracredentials)
     REMOTE = opt.remote
     UPDATE = opt.update
```

### Comparing `timetrack-odoo-1.0.2102/zeit2json.py` & `timetrack-odoo-1.0.2266/zeit2json.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 or Jira via their Rest APIs. See zeit2odoo.py and zeit2jira.py.
 
 (this module was initially developed as zeit2excel.py and retains some of the
 older optins)
 """
 
 __copyright__ = "(C) 2017-2023 Guido Draheim, licensed under the Apache License 2.0"""
-__version__ = "0.6.2102"
+__version__ = "0.6.2266"
 
 from typing import List, Dict, Union, Optional, Sequence, TextIO, Iterator, cast
 
 import logging
 import re
 import os
 import csv
@@ -508,18 +508,18 @@
         xlsx_file = XLSXFILE or f"{filename}.{FMT}"
         import tabtoxlsx
         tabtoxlsx.saveToXLSX(xlsx_file, data, reorder=order)
         logg.log(DONE, " %s written   %s '%s'  (%s entries)", FMT, viewFMT(FMT), xlsx_file, len(data))
 
 if __name__ == "__main__":
     from optparse import OptionParser
-    cmdline = OptionParser("%prog files...", epilog=__doc__)
+    cmdline = OptionParser("%prog [-opt] files...", epilog=__doc__, version=__version__)
     cmdline.formatter.max_help_position = 30
-    cmdline.add_option("-v", "--verbose", action="count", default=0,
-                       help="more verbose logging")
+    cmdline.add_option("-v", "--verbose", action="count", default=0, help="more verbose logging")
+    cmdline.add_option("-^", "--quiet", action="count", default=0, help="less verbose logging")
     cmdline.add_option("-1", "--oldformat", action="store_true", default=False,
                        help="generate ID column (was used as foreignkey in old odoo)")
     cmdline.add_option("-2", "--newformat", action="store_true", default=False,
                        help="generate Ticket column (can be used to import to jira)")
     cmdline.add_option("-a", "--after", metavar="DATE", default=ZEIT_AFTER,
                        help="only evaluate entrys on and after [first of year]")
     cmdline.add_option("-b", "--before", metavar="DATE", default=ZEIT_BEFORE,
@@ -544,16 +544,16 @@
     cmdline.add_option("-x", "--extra", action="store_true", default=ZEIT_EXTRATIME,
                        help="allow for the extra times [%default]")
     cmdline.add_option("-z", "--short", action="store_true", default=ZEIT_SHORT,
                        help="present the shorthand names for projects and tasks [%default]")
     cmdline.add_option("-U", "--user-name", metavar="TEXT", default=ZEIT_USER_NAME,
                        help="user name for the output report (not for login)")
     opt, args = cmdline.parse_args()
-    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose))
-    logg.setLevel(level=max(0, logging.WARNING - 10 * opt.verbose))
+    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose + 10 * opt.quiet))
+    logg.setLevel(level=max(0, logging.WARNING - 10 * opt.verbose + 10 * opt.quiet))
     # logg.addHandler(logging.StreamHandler())
     FORMAT = opt.format
     OUTPUT = opt.output
     JSONFILE = opt.jsonfile
     XLSXFILE = opt.xlsxfile
     CSVFILE = opt.csvfile
     if opt.newformat:
```

### Comparing `timetrack-odoo-1.0.2102/zeit2odoo.py` & `timetrack-odoo-1.0.2266/zeit2odoo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python3
 """
 Synchronize odoo-import data (from zeit.txt) with Odoo timesheet records.
 """
 
 __copyright__ = "(C) 2021-2023 Guido Draheim, licensed under the Apache License 2.0"""
-__version__ = "1.0.2102"
+__version__ = "1.0.2266"
 
 from typing import Optional, Union, Dict, List, Tuple, cast
 
 import logging
 import re
 import os
 import csv
@@ -564,18 +564,18 @@
             FMT = "xlsx"
             import tabtoxlsx
             tabtoxlsx.saveToXLSX(XLSXFILE, results)
             logg.log(DONE, " %s written   %s '%s'", FMT, viewFMT(FMT), XLSXFILE)
 
 if __name__ == "__main__":
     from optparse import OptionParser
-    cmdline = OptionParser("%prog [help|data|check|valid|update|compare|summarize|summary|topics]", epilog=__doc__)
+    cmdline = OptionParser("%prog [-opt] [help|commmand...]", epilog=__doc__, version=__version__)
     cmdline.formatter.max_help_position = 30
-    cmdline.add_option("-v", "--verbose", action="count", default=0,
-                       help="more verbose logging")
+    cmdline.add_option("-v", "--verbose", action="count", default=0, help="more verbose logging")
+    cmdline.add_option("-^", "--quiet", action="count", default=0, help="less verbose logging")
     cmdline.add_option("-a", "--after", metavar="DATE", default=None,
                        help="only evaluate entrys on and after date")
     cmdline.add_option("-b", "--before", metavar="DATE", default=None,
                        help="only evaluate entrys on and before date")
     cmdline.add_option("-s", "--summary", metavar="TEXT", default=ZEIT_SUMMARY,
                        help="suffix for summary report [%default]")
     cmdline.add_option("-p", "--price", metavar="TEXT", action="append", default=PRICES,
@@ -606,16 +606,16 @@
     cmdline.add_option("-g", "--gitcredentials", metavar="FILE", default=dotnetrc.GIT_CREDENTIALS)
     cmdline.add_option("-G", "--netcredentials", metavar="FILE", default=dotnetrc.NET_CREDENTIALS)
     cmdline.add_option("-E", "--extracredentials", metavar="FILE", default=dotnetrc.NETRC_FILENAME)
     cmdline.add_option("-c", "--config", metavar="NAME=VALUE", action="append", default=[])
     cmdline.add_option("-y", "--update", action="store_true", default=UPDATE,
                        help="actually update odoo")
     opt, args = cmdline.parse_args()
-    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose))
-    logg.setLevel(level=max(0, logging.WARNING - 10 * opt.verbose))
+    logging.basicConfig(level=max(0, logging.WARNING - 10 * opt.verbose + 10 * opt.quiet))
+    logg.setLevel(level=max(0, logging.WARNING - 10 * opt.verbose + 10 * opt.quiet))
     # logg.addHandler(logging.StreamHandler())
     for value in opt.config:
         git_config_override(value)
     dotnetrc.set_password_filename(opt.gitcredentials)
     dotnetrc.add_password_filename(opt.netcredentials, opt.extracredentials)
     if opt.mockup:
         import odoo2data_api_mockup as odoo_api  # type: ignore[no-redef]
```

