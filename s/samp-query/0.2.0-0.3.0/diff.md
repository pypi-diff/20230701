# Comparing `tmp/samp_query-0.2.0.tar.gz` & `tmp/samp_query-0.3.0.tar.gz`

## Comparing `samp_query-0.2.0.tar` & `samp_query-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,8 @@
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 samp_query-0.2.0/.coverage
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 samp_query-0.2.0/main.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 samp_query-0.2.0/requirements-test.txt
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 samp_query-0.2.0/requirements.txt
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 samp_query-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 samp_query-0.2.0/samp_query/__init__.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 samp_query-0.2.0/samp_query/rcon.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.2.0/test/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.2.0/test/conftest.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 samp_query-0.2.0/test/test_client.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 samp_query-0.2.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 samp_query-0.2.0/LICENSE
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 samp_query-0.2.0/README.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 samp_query-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 samp_query-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    12337 2020-02-02 00:00:00.000000 samp_query-0.3.0/samp_query/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.3.0/samp_query/py.typed
+-rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 samp_query-0.3.0/samp_query/rcon.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 samp_query-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 samp_query-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 samp_query-0.3.0/README.md
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 samp_query-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 samp_query-0.3.0/PKG-INFO
```

### Comparing `samp_query-0.2.0/samp_query/rcon.py` & `samp_query-0.3.0/samp_query/rcon.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+import os
 import sys
 
 import trio
 
 from samp_query import (
     Client,
     InvalidRCONPassword,
     RCONDisabled,
 )
 
+if sys.platform not in ('win32', 'cygwin', 'msys'):
+    import readline  # noqa: F401
+
 TIMEOUT = 5
 
 
 def prompt(text: str, default: bool = False) -> bool:
     choices = ['y', 'n']
     default_index = 0 if default is True else 1
     choices[default_index] = choices[default_index].upper()
@@ -26,29 +30,30 @@
             return False
 
         if not response:
             return default
 
         if response not in valid_choices:
             print(
-                f'Invalid response {response}. Valid choices are:',
+                f'Invalid response: {response!r}. Valid choices are:',
                 ', '.join(repr(choice) for choice in valid_choices)
             )
             continue
 
         return response.startswith('y')
 
 
 async def main(*args: str) -> str | None:
     header = 'samp-query RCON client'
     print(header)
     print('=' * len(header), end='\n\n')
 
     if len(args) != 4:
-        return f'Usage: {args[0]} host port rcon_password'
+        samp_rcon = os.path.basename(args[0])
+        return f'Usage: {samp_rcon} host port rcon_password'
 
     host, port, rcon_password = args[1:]
     client = Client(host, int(port), rcon_password)
 
     print(f'Connecting to {host}:{port}...')
 
     try:
@@ -81,28 +86,34 @@
 
     except InvalidRCONPassword:
         return f'Invalid RCON password for {host}:{port}.'
 
     while True:
         try:
             command = input(f'rcon@{host}:{port} # ')
-        except EOFError:
+        except (EOFError, KeyboardInterrupt):
             print()
             break
 
         if not command:
             continue
 
         if command == 'quit':
             break
 
         if command == 'exit':
-            if not prompt(
-                'Are you sure you want to shut your server down?'
-            ):
+            try:
+                really_exit = prompt(
+                    'Are you sure you want to shut your server down?'
+                )
+            except KeyboardInterrupt:
+                print()
+                break
+
+            if not really_exit:
                 continue
 
             try:
                 await client.rcon(command)
             except RCONDisabled:
                 pass  # Yes, it's very much disabled the hard way now.
```

### Comparing `samp_query-0.2.0/LICENSE` & `samp_query-0.3.0/LICENSE`

 * *Files identical despite different names*

