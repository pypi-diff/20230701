# Comparing `tmp/hostb_client-7.tar.gz` & `tmp/hostb_client-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hostb_client-7.tar", last modified: Thu Jan 11 20:17:18 2018, max compression
+gzip compressed data, was "dist/hostb_client-9.tar", last modified: Sat Feb 10 12:54:41 2018, max compression
```

## Comparing `hostb_client-7.tar` & `hostb_client-9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2018-01-11 20:17:18.000000 hostb_client-7/
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2018-01-11 20:17:18.000000 hostb_client-7/bin/
--rwxr-xr-x   0 j         (1000) j         (1000)     1083 2014-03-01 15:20:57.000000 hostb_client-7/bin/hostb_client
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2018-01-11 20:17:18.000000 hostb_client-7/hostb_client/
--rw-r--r--   0 j         (1000) j         (1000)     7974 2016-08-24 15:08:09.000000 hostb_client-7/hostb_client/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)     2703 2014-03-01 12:38:46.000000 hostb_client-7/hostb_client/form.py
--rw-r--r--   0 j         (1000) j         (1000)     4126 2014-03-01 12:43:30.000000 hostb_client-7/hostb_client/utils.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2018-01-11 20:17:18.000000 hostb_client-7/hostb_client.egg-info/
--rw-r--r--   0 j         (1000) j         (1000)      460 2018-01-11 20:17:18.000000 hostb_client-7/hostb_client.egg-info/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)      244 2018-01-11 20:17:18.000000 hostb_client-7/hostb_client.egg-info/SOURCES.txt
--rw-r--r--   0 j         (1000) j         (1000)        1 2018-01-11 20:17:18.000000 hostb_client-7/hostb_client.egg-info/dependency_links.txt
--rw-r--r--   0 j         (1000) j         (1000)       13 2018-01-11 20:17:18.000000 hostb_client-7/hostb_client.egg-info/top_level.txt
--rw-r--r--   0 j         (1000) j         (1000)      159 2014-03-03 14:24:19.000000 hostb_client-7/README
--rw-r--r--   0 j         (1000) j         (1000)      942 2018-01-11 20:17:17.000000 hostb_client-7/setup.py
--rw-r--r--   0 j         (1000) j         (1000)      460 2018-01-11 20:17:18.000000 hostb_client-7/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)       59 2018-01-11 20:17:18.000000 hostb_client-7/setup.cfg
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2018-02-10 12:54:41.000000 hostb_client-9/
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2018-02-10 12:54:41.000000 hostb_client-9/bin/
+-rwxr-xr-x   0 j         (1000) j         (1000)     1089 2018-01-11 20:21:35.000000 hostb_client-9/bin/hostb_client
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2018-02-10 12:54:41.000000 hostb_client-9/hostb_client/
+-rw-r--r--   0 j         (1000) j         (1000)     8089 2018-02-10 12:16:14.000000 hostb_client-9/hostb_client/__init__.py
+-rw-r--r--   0 j         (1000) j         (1000)     3184 2018-01-11 20:41:44.000000 hostb_client-9/hostb_client/form.py
+-rw-r--r--   0 j         (1000) j         (1000)     4076 2018-01-11 20:22:40.000000 hostb_client-9/hostb_client/utils.py
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2018-02-10 12:54:41.000000 hostb_client-9/hostb_client.egg-info/
+-rw-r--r--   0 j         (1000) j         (1000)      454 2018-02-10 12:54:40.000000 hostb_client-9/hostb_client.egg-info/PKG-INFO
+-rw-r--r--   0 j         (1000) j         (1000)      247 2018-02-10 12:54:40.000000 hostb_client-9/hostb_client.egg-info/SOURCES.txt
+-rw-r--r--   0 j         (1000) j         (1000)        1 2018-02-10 12:54:40.000000 hostb_client-9/hostb_client.egg-info/dependency_links.txt
+-rw-r--r--   0 j         (1000) j         (1000)       13 2018-02-10 12:54:40.000000 hostb_client-9/hostb_client.egg-info/top_level.txt
+-rw-r--r--   0 j         (1000) j         (1000)      167 2018-01-11 20:46:05.000000 hostb_client-9/README.md
+-rw-r--r--   0 j         (1000) j         (1000)      938 2018-02-10 12:54:40.000000 hostb_client-9/setup.py
+-rw-r--r--   0 j         (1000) j         (1000)      454 2018-02-10 12:54:41.000000 hostb_client-9/PKG-INFO
+-rw-r--r--   0 j         (1000) j         (1000)       59 2018-02-10 12:54:41.000000 hostb_client-9/setup.cfg
```

### Comparing `hostb_client-7/bin/hostb_client` & `hostb_client-9/bin/hostb_client`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-#!/usr/bin/python
+#!/usr/bin/python3
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
-# GPL 2012
+# GPL 2012-2018
 
 import os
 import sys
 from optparse import OptionParser
 
 root = os.path.join(os.path.abspath(os.path.dirname(__file__)), '..')
 if os.path.exists(os.path.join(root, 'hostb_client')):
```

### Comparing `hostb_client-7/hostb_client/__init__.py` & `hostb_client-9/hostb_client/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-#!/usr/bin/python
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
-# GPL 2014
-from __future__ import division, print_function
+# GPL 2014-2018
 
-import cookielib
+
+import http.cookiejar
 import gzip
-import StringIO
-import urllib2
-from urlparse import urlparse
+import io
+import urllib.request, urllib.error, urllib.parse
+from urllib.parse import urlparse
 
 import json
 import math
 import os
 import socket
 import sys
 import time
 
-from form import MultiPartForm
-from utils import format_duration, format_bytes
+from .form import MultiPartForm
+from .utils import format_duration, format_bytes
 
 DEBUG = False
 
 __version__ = '0.1'
 
 socket.setdefaulttimeout(300)
 CHUNK_SIZE = 1024*1024
@@ -45,17 +44,17 @@
         self.base_url = url
         self.url = os.path.join(self.base_url, 'add')
         self._resume_file = '/tmp/hostb_client.%s.json' % os.environ.get('USER')
         #super(Client, self).__init__(url, cj)
         if cj:
             self._cj = cj
         else:
-            self._cj = cookielib.CookieJar()
-        self._opener = urllib2.build_opener(urllib2.HTTPCookieProcessor(self._cj),
-                                            urllib2.HTTPHandler(debuglevel=self.debuglevel))
+            self._cj = http.cookiejar.CookieJar()
+        self._opener = urllib.request.build_opener(urllib.request.HTTPCookieProcessor(self._cj),
+                                            urllib.request.HTTPHandler(debuglevel=self.debuglevel))
         self._opener.addheaders = [
             ('User-Agent', '%s/%s' % (self.__name__, self.__version__))
         ]
 
     def upload(self, filename, password=''):
         return self.upload_chunks(self.url, filename, {
             'firefogg': '1',
@@ -80,35 +79,37 @@
             for key in data:
                 form.add_field(key, data[key])
             data = self._json_request(url, form)
 
         print(filename)
         hide_cursor()
         result_url = data.get('url')
+        print_result_url = result_url
         upload_token = data.get('token')
         if 'uploadUrl' in data:
-            if 'url' in data:
+            if result_url:
                 print(data['url'])
+                print_result_url = False
             uploadUrl = data['uploadUrl']
             if uploadUrl.startswith('/'):
                 u = urlparse(url)
                 uploadUrl = '%s://%s%s' % (u.scheme, u.netloc, uploadUrl)
-            f = open(filename)
+            f = open(filename, 'rb')
             fsize = os.stat(filename).st_size
             done = 0
             start = time.mktime(time.localtime())
             if 'offset' in data and data['offset'] < fsize:
                 done = data['offset']
                 f.seek(done)
                 resume_offset = done
             else:
                 resume_offset = 0
             chunk = f.read(CHUNK_SIZE)
             fname = os.path.basename(filename)
-            if isinstance(fname, unicode):
+            if isinstance(fname, str):
                 fname = fname.encode('utf-8')
             while chunk:
                 elapsed = time.mktime(time.localtime()) - start
                 remaining = ""
                 if done:
                     r = math.ceil((elapsed / (done/(fsize-resume_offset)) - elapsed)/60) * 60
                     r = format_duration(r, milliseconds=False, verbosity=2)
@@ -154,16 +155,17 @@
                             'url': result_url,
                             'offset': done
                         }, r, indent=2)
                     chunk = f.read(CHUNK_SIZE)
             if os.path.exists(self._resume_file):
                 os.unlink(self._resume_file)
                 resume = None
-            if result_url:
+            if print_result_url:
                 print(result_url + (' ' * (80-len(result_url))))
+            if result_url:
                 if upload_token:
                     print('To remove this file later, you need this token: %s' % upload_token)
             else:
                 print(' ' * 80)
             print('')
             show_cursor()
             return data and 'result' in data and data.get('result') == 1
@@ -175,27 +177,26 @@
                     print("failed to upload file to", url)
                     print(data)
         return False
 
     def _json_request(self, url, form):
         result = {}
         try:
-            body = str(form)
-            request = urllib2.Request(str(url))
+            body = form.body()
+            request = urllib.request.Request(str(url), data=body, method='POST')
             request.add_header('Content-type', form.get_content_type())
             request.add_header('Content-Length', str(len(body)))
             request.add_header('Accept-Encoding', 'gzip, deflate')
-            request.add_data(body)
             f = self._opener.open(request)
             result = f.read()
             if f.headers.get('content-encoding', None) == 'gzip':
-                result = gzip.GzipFile(fileobj=StringIO.StringIO(result)).read()
+                result = gzip.GzipFile(fileobj=io.BytesIO(result)).read()
             result = result.decode('utf-8')
             return json.loads(result)
-        except urllib2.HTTPError as e:
+        except urllib.error.HTTPError as e:
             if self.DEBUG:
                 import webbrowser
                 if e.code >= 500:
                     with open('/tmp/error.html', 'w') as f:
                         f.write(e.read())
                     webbrowser.open_new_tab('/tmp/error.html')
```

### Comparing `hostb_client-7/hostb_client/form.py` & `hostb_client-9/hostb_client/form.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,100 @@
 import itertools
-import mimetools
 import mimetypes
+import os
+import hashlib
+import sys
 
 
 __all__ = ['MultiPartForm']
 
+# from /usr/lib/python3.4/email/generator.py
+# Helper used by Generator._make_boundary
+_width = len(repr(sys.maxsize-1))
+_fmt = '%%0%dd' % _width
+
+def _make_boundary():
+    # Craft a random boundary.
+    boundary = ('=' * 15) + hashlib.sha1(os.urandom(32)).hexdigest() + '=='
+    return boundary
+
 class MultiPartForm(object):
     """Accumulate the data to be used when posting a form."""
 
     def __init__(self):
         self.form_fields = []
         self.files = []
-        self.boundary = mimetools.choose_boundary()
+        self.boundary = _make_boundary()
         return
     
     def get_content_type(self):
         return 'multipart/form-data; boundary=%s' % self.boundary
 
     def add_field(self, name, value):
         """Add a simple field to the form data."""
-        if isinstance(name, unicode):
-            name = name.encode('utf-8')
-        if isinstance(value, unicode):
-            value = value.encode('utf-8')
+        if isinstance(name, bytes):
+            name = name.decode('utf-8')
+        if isinstance(value, bytes):
+            value = value.decode('utf-8')
         self.form_fields.append((name, value))
         return
 
     def add_file(self, fieldname, filename, fileHandle, mimetype=None):
         """Add a file to be uploaded."""
-        if isinstance(fieldname, unicode):
-            fieldname = fieldname.encode('utf-8')
-        if isinstance(filename, unicode):
-            filename = filename.encode('utf-8')
+        if isinstance(fieldname, bytes):
+            fieldname = fieldname.decode('utf-8')
+        if isinstance(filename, bytes):
+            filename = filename.decode('utf-8')
 
         if hasattr(fileHandle, 'read'):
             body = fileHandle.read()
         else:
             body = fileHandle
         if mimetype is None:
             mimetype = mimetypes.guess_type(filename)[0] or 'application/octet-stream'
         self.files.append((fieldname, filename, mimetype, body))
         return
-    
+
     def __str__(self):
-        """Return a string representing the form data, including attached files."""
+        body = self.body()
+        body = body.decode('utf-8')
+        return body
+
+    def body(self):
+        """Return a byte string representing the form data, including attached files."""
         # Build a list of lists, each containing "lines" of the
         # request.  Each part is separated by a boundary string.
         # Once the list is built, return a string where each
         # line is separated by '\r\n'.  
         parts = []
         part_boundary = '--' + self.boundary
-        
+
         # Add the form fields
         parts.extend(
             [ part_boundary,
               'Content-Disposition: form-data; name="%s"' % name,
               '',
               value,
             ]
             for name, value in self.form_fields
             )
-        
+
         # Add the files to upload
         parts.extend(
             [ part_boundary,
               'Content-Disposition: file; name="%s"; filename="%s"' % \
                  (field_name, filename),
               'Content-Type: %s' % content_type,
               '',
               body,
             ]
             for field_name, filename, content_type, body in self.files
             )
-        
+
         # Flatten the list and add closing boundary marker,
         # then return CR+LF separated data
         flattened = list(itertools.chain(*parts))
         flattened.append('--' + self.boundary + '--')
         flattened.append('')
-        return '\r\n'.join(flattened)
+        flattened = [part if isinstance(part, bytes) else part.encode('utf-8') for part in flattened]
+        return b'\r\n'.join(flattened)
```

### Comparing `hostb_client-7/hostb_client/utils.py` & `hostb_client-9/hostb_client/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 # GPL 2014
-from __future__ import division, with_statement
+
 
 import math
 
 def format_thousands(number, separator = ','):
     """
     Return the number with separators (1,000,000)
     
@@ -96,15 +96,15 @@
         else:
             durations = [plural(d, 'day'), plural(h,'hour'),
                 plural(m, 'minute'), plural(s, 'second')]
             if years:
                 durations.insert(0, plural(y, 'year'))
             if milliseconds:
                 durations.append(plural(ms, 'millisecond'))
-        durations = filter(lambda x: not x.startswith('0'), durations)
+        durations = [x for x in durations if not x.startswith('0')]
         duration = ' '.join(durations)
     return duration
 
 def format_bytes(number):
     return format_number(number, 'byte', 'B')
 
 def format_number(number, longName, shortName):
```

### Comparing `hostb_client-7/setup.py` & `hostb_client-9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 # vi:si:et:sw=4:sts=4:ts=4
 # encoding: utf-8
 try:
     from setuptools import setup
 except:
     from distutils.core import setup
 
 def get_version():
-    return 7 #import subprocess
-    version = subprocess.check_output(['git', 'rev-list', 'HEAD', '--count'])
+    return 9 #import subprocess
+    version = subprocess.check_output(['git', 'rev-list', 'HEAD', '--count']).decode()
     return version.strip()
 
+
 setup(
     name="hostb_client",
-    version=get_version() ,
+    version=get_version(),
     description='''hostb_client is a command line client for hostb.''',
     author="j",
     author_email="j@mailb.org",
-    url="http://r-w-x.org/?p=hostb_client.git;a=summary",
-    download_url="https://hostb.org/client/",
+    url="https://r-w-x.org/r/hostb_client",
     license="GPLv3",
-    scripts = [
+    scripts=[
         'bin/hostb_client',
     ],
     packages=[
         'hostb_client'
     ],
     install_requires=[
     ],
-    keywords = [
-],
-    classifiers = [
-      'Operating System :: OS Independent',
-      'Programming Language :: Python',
-      'License :: OSI Approved :: GNU General Public License (GPL)',
+    keywords=[],
+    classifiers=[
+        'Operating System :: OS Independent',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'License :: OSI Approved :: GNU General Public License (GPL)',
     ],
 )
```

