# Comparing `tmp/heaven-0.0.9.tar.gz` & `tmp/heaven-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaven-0.0.9.tar", max compression
+gzip compressed data, was "heaven-0.1.0.tar", max compression
```

## Comparing `heaven-0.0.9.tar` & `heaven-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1073 2023-04-04 16:11:34.728189 heaven-0.0.9/LICENSE
--rw-r--r--   0        0        0     1300 2023-06-16 18:27:00.893443 heaven-0.0.9/README.md
--rw-r--r--   0        0        0      216 2023-06-25 10:40:34.424329 heaven-0.0.9/heaven/__init__.py
--rw-r--r--   0        0        0      743 2023-06-10 13:10:30.157056 heaven-0.0.9/heaven/constants.py
--rw-r--r--   0        0        0      261 2023-06-10 13:10:30.157160 heaven-0.0.9/heaven/context.py
--rw-r--r--   0        0        0      141 2023-06-10 13:10:30.157248 heaven-0.0.9/heaven/errors.py
--rw-r--r--   0        0        0      977 2023-06-10 13:10:30.157442 heaven-0.0.9/heaven/form.py
--rw-r--r--   0        0        0     2946 2023-06-10 13:10:30.157649 heaven-0.0.9/heaven/mocks.py
--rw-r--r--   0        0        0     3734 2023-06-25 10:40:10.409284 heaven-0.0.9/heaven/request.py
--rw-r--r--   0        0        0     4390 2023-06-10 23:36:48.661427 heaven-0.0.9/heaven/response.py
--rw-r--r--   0        0        0    22029 2023-06-16 18:25:20.409409 heaven-0.0.9/heaven/router.py
--rw-r--r--   0        0        0        0 2023-06-10 13:10:30.158385 heaven-0.0.9/heaven/server.py
--rw-r--r--   0        0        0     1116 2023-06-10 13:10:30.158553 heaven-0.0.9/heaven/tutorials.py
--rw-r--r--   0        0        0      926 2023-06-10 13:10:30.158643 heaven-0.0.9/heaven/utils.py
--rw-r--r--   0        0        0      485 2023-06-25 10:40:43.222347 heaven-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     2106 1970-01-01 00:00:00.000000 heaven-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-04 16:11:34.728189 heaven-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1300 2023-06-16 18:27:00.893443 heaven-0.1.0/README.md
+-rw-r--r--   0        0        0      216 2023-06-26 23:31:15.815957 heaven-0.1.0/heaven/__init__.py
+-rw-r--r--   0        0        0      743 2023-06-10 13:10:30.157056 heaven-0.1.0/heaven/constants.py
+-rw-r--r--   0        0        0      261 2023-06-10 13:10:30.157160 heaven-0.1.0/heaven/context.py
+-rw-r--r--   0        0        0      141 2023-06-10 13:10:30.157248 heaven-0.1.0/heaven/errors.py
+-rw-r--r--   0        0        0      977 2023-06-10 13:10:30.157442 heaven-0.1.0/heaven/form.py
+-rw-r--r--   0        0        0     2946 2023-06-10 13:10:30.157649 heaven-0.1.0/heaven/mocks.py
+-rw-r--r--   0        0        0     3751 2023-06-26 22:30:38.568524 heaven-0.1.0/heaven/request.py
+-rw-r--r--   0        0        0     4916 2023-06-29 08:27:55.804469 heaven-0.1.0/heaven/response.py
+-rw-r--r--   0        0        0    22051 2023-06-26 23:23:06.970388 heaven-0.1.0/heaven/router.py
+-rw-r--r--   0        0        0        0 2023-06-10 13:10:30.158385 heaven-0.1.0/heaven/server.py
+-rw-r--r--   0        0        0     1484 2023-06-26 22:09:03.202081 heaven-0.1.0/heaven/tutorials.py
+-rw-r--r--   0        0        0      926 2023-06-10 13:10:30.158643 heaven-0.1.0/heaven/utils.py
+-rw-r--r--   0        0        0      505 2023-07-01 09:00:36.636947 heaven-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2149 1970-01-01 00:00:00.000000 heaven-0.1.0/PKG-INFO
```

### Comparing `heaven-0.0.9/LICENSE` & `heaven-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaven-0.0.9/README.md` & `heaven-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `heaven-0.0.9/heaven/constants.py` & `heaven-0.1.0/heaven/constants.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.9/heaven/form.py` & `heaven-0.1.0/heaven/form.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.9/heaven/mocks.py` & `heaven-0.1.0/heaven/mocks.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.9/heaven/request.py` & `heaven-0.1.0/heaven/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,17 +55,17 @@
             csd = {}
             cookiestring = self.headers.get("cookie")
             if not cookiestring:
                 self._cookies = csd
                 return self._cookies
             cookies = cookiestring.split("; ")
             for cookie in cookies:
-                try: k, v = cookie.split("=")
+                try: k, v = cookie.split("=", 1)
                 except: pass
-                else: csd[k] = v
+                else: csd[k.lower()] = v
             self._cookies = csd
         return self._cookies
 
     @property
     def form(self) -> "Form":
         if not "multipart/form-data" in self.headers.get("content-type"):
             return None  # currently none
@@ -102,15 +102,15 @@
 
     @property
     def params(self):
         if not self._dirty:
             if not self._params: self._params = {}
             self._params = {**self._params, **self._parse_qs()}
             self._dirty = True
-        return self._params
+        return self._params or {}
 
     @params.setter
     def params(self, pair):
         if not self._params:
             self._params = {}
         self._params[pair[0]] = pair[1]
```

### Comparing `heaven-0.0.9/heaven/response.py` & `heaven-0.1.0/heaven/response.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from functools import singledispatch, update_wrapper
 from http import HTTPStatus
 from typing import TYPE_CHECKING
 
 from .constants import MESSAGE_NOT_FOUND, STATUS_NOT_FOUND
 from .context import Context
-from .tutorials import get_guardian_angel_html, NO_TEMPLATING
+from .tutorials import get_guardian_angel_html, ASYNC_RENDER, NO_TEMPLATING, SYNC_RENDER
 if TYPE_CHECKING:
     from router import App
 
 
 # For compatibility with older versions of python3 using this
 # otherwise would use singledispatchmethod available from ^3.8
 def MethodDispatch(method):
@@ -32,14 +32,19 @@
     return payload.encode()
 
 @_body.register(int)
 @_body.register(float)
 def _(payload):
     return f'{payload}'.encode()
 
+def _get_guardian_angel(res: 'Response', error, snippet: str):
+    res.headers = 'Content-Type', 'text/html'
+    res.status = HTTPStatus.INTERNAL_SERVER_ERROR
+    res.body = get_guardian_angel_html(error, snippet)
+
 
 class Response():
     def __init__(self, app: 'App', context: 'Context'):
         self._app = app
         self._ctx = context
         self._abort = False
         self._body = MESSAGE_NOT_FOUND.encode()
@@ -87,51 +92,52 @@
 
     @headers.setter
     def headers(self, value):
         key, val = value
         _encode = lambda k: k.encode('utf-8') if isinstance(k, str) else k
         value = _encode(key), _encode(val)
         self._headers.append(value)
-    
-    def file(self, name: str, folder='public'):
-        """Serve file from assets/public folder with correct file type from known_file_types"""
-        pass
 
     @property
     def metadata(self):
         return self._metadata
 
     @metadata.setter
     def metadata(self, value):
         if not isinstance(value, dict): raise ValueError
         self._metadata = value
 
-    @property
-    def mounted(self):
-        return self._mounted_from_application
-
-    @mounted.setter
-    def mounted(self, value: 'App'):
-        self._mounted_from_application = value
-
     async def render(self, name: str, **contexts):
         """Serve html file walking up parent router/app tree until base parent if necessary"""
-        # TODO: add support to customize order in **contexts later when you think of the api and make an atomic commit
-        templater = self.mounted._templater or self._app._templater
+        templater = self._app._templater
+        self.headers = 'content-type', 'text/html'
+        if self._mounted_from_application and not templater:
+            templater = self.mounted._templater
         if not templater:
-            self.headers = 'Content-Type', 'text/html'
-            self.status = HTTPStatus.INTERNAL_SERVER_ERROR
-            self.body = get_guardian_angel_html('You did not enable templating', NO_TEMPLATING)
-            return
+            return _get_guardian_angel(self, 'You did not enable templating', NO_TEMPLATING)
+        
+        if not templater.is_async:
+            return _get_guardian_angel(self, 'Trying to use Sync HTML Renderer to render HTML Async', ASYNC_RENDER)
+
         template = templater.get_template(name)
         self.body = await template.render_async({'ctx': self._ctx, **contexts})
 
-    def renders(self, name: str):
+    def renders(self, name: str, **contexts):
         """Synchronous version of render method above"""
-        pass
+        templater = self._app._templater
+        self.headers = 'content-type', 'text/html'
+        if self._mounted_from_application and not templater:
+            templater = self.mounted._templater
+        if not templater:
+            return _get_guardian_angel(self, 'You did not enable templating', NO_TEMPLATING)
+        
+        if templater.is_async:
+            return _get_guardian_angel(self, 'Trying to use Async HTML Renderer to render Sync HTML', SYNC_RENDER)
+        template = templater.get_template(name)
+        self.body = template.render({'ctx': self._ctx, **contexts})
 
     def redirect(self, location, permanent=False):
         if permanent: self.status = HTTPStatus.PERMANENT_REDIRECT
         else: self.status = HTTPStatus.TEMPORARY_REDIRECT
         self.headers = 'Location', location
 
     @property
```

### Comparing `heaven-0.0.9/heaven/router.py` & `heaven-0.1.0/heaven/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 SEPARATOR = INDEX = "/"
 
 
 def _closure_mounted_application(handler: Handler, mounted: 'Router'):
     async def delegate(req: Request, res: Response, ctx: Context):
         req.mounted = mounted
-        res.mounted = mounted
+        res._mounted_from_application = mounted
         if iscoroutinefunction(handler): await handler(req, res, ctx)
         else: handler(req, res, ctx)
     return delegate
 
 
 def _get_configuration(configurator=None):
     if not configurator: return {}
@@ -368,15 +368,15 @@
 
         response = await engine.handle(scope, receive, send, metadata, self)
         await send({'type': 'http.response.start', 'headers': response.headers, 'status': response.status})
         await send({'type': 'http.response.body', 'body': response.body, **response.metadata})
 
         # add background tasks
         if response.deferred:
-            await gather(*[func() for func in response._deferred])
+            await gather(*[func(self) for func in response._deferred])
 
     def abettor(self, method: str, route: str, handler: Handler, subdomain=DEFAULT, router = None):
         if not route.startswith('/'): raise UrlError
         engine = self.subdomains.get(subdomain)
         if not isinstance(engine, Routes):
             raise SubdomainError
         engine.add(method, route, handler, router or self)
```

### Comparing `heaven-0.0.9/heaven/utils.py` & `heaven-0.1.0/heaven/utils.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.9/PKG-INFO` & `heaven-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: heaven
-Version: 0.0.9
+Version: 0.1.0
 Summary: Extremely Stupid Simple, Blazing Fast, Get Out of your way immediately Microframework for building Python Web Applications.
 License: MIT
 Author: Raymond Ortserga
 Author-email: ortserga@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiofiles (>=23.0.0,<24.0.0)
 Requires-Dist: jinja2 (>=3.1.0,<4.0.0)
 Requires-Dist: uvicorn (>=0.14.0,<0.15.0)
 Description-Content-Type: text/markdown
 
 # Heaven : <img src="https://img.shields.io/badge/coverage-95%25-green" />
 
 Heaven is a very very small, extremely tiny, and insanely fast [ASGI](https://asgi.readthedocs.io) web application framework. It was designed to facilitate productivity by allowing for complete mastery in 7 minutes or less.
```

