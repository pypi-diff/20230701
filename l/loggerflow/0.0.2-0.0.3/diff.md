# Comparing `tmp/loggerflow-0.0.2.tar.gz` & `tmp/loggerflow-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggerflow-0.0.2.tar", last modified: Mon Jun 19 13:15:42 2023, max compression
+gzip compressed data, was "loggerflow-0.0.3.tar", last modified: Sat Jul  1 12:59:14 2023, max compression
```

## Comparing `loggerflow-0.0.2.tar` & `loggerflow-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 13:15:42.958906 loggerflow-0.0.2/
--rw-rw-rw-   0        0        0     1114 2023-06-10 20:34:53.000000 loggerflow-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2575 2023-06-19 13:15:42.957901 loggerflow-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1830 2023-06-19 12:51:14.000000 loggerflow-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 13:15:42.940364 loggerflow-0.0.2/loggerflow/
--rw-rw-rw-   0        0        0      242 2023-06-10 20:56:46.000000 loggerflow-0.0.2/loggerflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:15:42.954897 loggerflow-0.0.2/loggerflow/backends/
--rw-rw-rw-   0        0        0        0 2023-06-10 20:36:08.000000 loggerflow-0.0.2/loggerflow/backends/__init__.py
--rw-rw-rw-   0        0        0      164 2023-06-11 09:55:09.000000 loggerflow-0.0.2/loggerflow/backends/abstract_backend.py
--rw-rw-rw-   0        0        0      893 2023-06-11 09:55:09.000000 loggerflow-0.0.2/loggerflow/backends/discord.py
--rw-rw-rw-   0        0        0      156 2023-06-11 08:26:33.000000 loggerflow-0.0.2/loggerflow/backends/filters.py
--rw-rw-rw-   0        0        0     1093 2023-06-19 09:45:46.000000 loggerflow-0.0.2/loggerflow/backends/telegram.py
--rw-rw-rw-   0        0        0     2712 2023-06-19 12:21:45.000000 loggerflow-0.0.2/loggerflow/loggerflow.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:15:42.956900 loggerflow-0.0.2/loggerflow/utils/
--rw-rw-rw-   0        0        0        0 2023-06-10 20:35:33.000000 loggerflow-0.0.2/loggerflow/utils/__init__.py
--rw-rw-rw-   0        0        0      241 2023-06-19 12:19:59.000000 loggerflow-0.0.2/loggerflow/utils/handler.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:15:42.948374 loggerflow-0.0.2/loggerflow.egg-info/
--rw-rw-rw-   0        0        0     2575 2023-06-19 13:15:42.000000 loggerflow-0.0.2/loggerflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      466 2023-06-19 13:15:42.000000 loggerflow-0.0.2/loggerflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 13:15:42.000000 loggerflow-0.0.2/loggerflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-19 13:15:42.000000 loggerflow-0.0.2/loggerflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 13:15:42.000000 loggerflow-0.0.2/loggerflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 13:15:42.958906 loggerflow-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1076 2023-06-19 13:11:18.000000 loggerflow-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 12:59:14.195413 loggerflow-0.0.3/
+-rw-rw-rw-   0        0        0     1529 2023-07-01 12:41:46.000000 loggerflow-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3165 2023-07-01 12:59:14.194411 loggerflow-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2427 2023-07-01 12:57:40.000000 loggerflow-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 12:59:14.158571 loggerflow-0.0.3/loggerflow/
+-rw-rw-rw-   0        0        0      242 2023-06-10 20:56:46.000000 loggerflow-0.0.3/loggerflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 12:59:14.184878 loggerflow-0.0.3/loggerflow/backends/
+-rw-rw-rw-   0        0        0      156 2023-06-22 18:07:06.000000 loggerflow-0.0.3/loggerflow/backends/__init__.py
+-rw-rw-rw-   0        0        0      164 2023-06-11 09:55:09.000000 loggerflow-0.0.3/loggerflow/backends/abstract_backend.py
+-rw-rw-rw-   0        0        0      767 2023-06-22 16:52:02.000000 loggerflow-0.0.3/loggerflow/backends/discord.py
+-rw-rw-rw-   0        0        0      112 2023-06-22 16:42:10.000000 loggerflow-0.0.3/loggerflow/backends/filters.py
+-rw-rw-rw-   0        0        0      952 2023-07-01 12:30:53.000000 loggerflow-0.0.3/loggerflow/backends/telegram.py
+-rw-rw-rw-   0        0        0     4716 2023-07-01 12:35:54.000000 loggerflow-0.0.3/loggerflow/loggerflow.py
+drwxrwxrwx   0        0        0        0 2023-07-01 12:59:14.191879 loggerflow-0.0.3/loggerflow/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-10 20:35:33.000000 loggerflow-0.0.3/loggerflow/utils/__init__.py
+-rw-rw-rw-   0        0        0      241 2023-06-19 12:19:59.000000 loggerflow-0.0.3/loggerflow/utils/handler.py
+-rw-rw-rw-   0        0        0     1385 2023-07-01 12:17:35.000000 loggerflow-0.0.3/loggerflow/utils/stack_cleaner.py
+drwxrwxrwx   0        0        0        0 2023-07-01 12:59:14.171125 loggerflow-0.0.3/loggerflow.egg-info/
+-rw-rw-rw-   0        0        0     3165 2023-07-01 12:59:14.000000 loggerflow-0.0.3/loggerflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-07-01 12:59:14.000000 loggerflow-0.0.3/loggerflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 12:59:14.000000 loggerflow-0.0.3/loggerflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-01 12:59:14.000000 loggerflow-0.0.3/loggerflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-01 12:59:14.000000 loggerflow-0.0.3/loggerflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 12:59:14.195413 loggerflow-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1069 2023-07-01 12:30:53.000000 loggerflow-0.0.3/setup.py
```

### Comparing `loggerflow-0.0.2/PKG-INFO` & `loggerflow-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: loggerflow
-Version: 0.0.2
+Version: 0.0.3
 Summary: A new level of bug tracking for your Python projects
 Home-page: https://github.com/DeNRuDi/loggerflow
-Author: DeNRuDi, kad1m
+Author: DeNRuDi
 Author-email: denisrudnitskiy0@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -28,20 +28,28 @@
 ```
 
 A new level of bug tracking for your Python projects.
 
 
 <h5> Simple start (with Telegram backend): </h5>
 <details>
-  <summary>Changes (0.0.2 - actual)</summary>
+  <summary>Changes (0.0.3 - actual)</summary>
 
+  - v.0.0.3
+    - added the `traceback='full'` attribute to the LoggerFlow constructor, which allows you to send full, clean or minimal traceback to the backend (depending on your preferences).
+    You can pass 3 parameters:
+        - `full` -  Sending full traceback on your backend/backends;
+        - `clean` - Sending your program's stacktrace (clearing lines that were are called from libraries);
+        - `minimal` - Sending a 1 line with name file, number line and last line of your traceback;
+    - minor fixes in project architecture;
+    - writing documentation for project.
   - v.0.0.2
-    - add logging in threads (to disable logging in threads - pass the parameter thread_logging=False to the LoggerFlow constructor);
+    - added logging in threads (to disable logging in threads - pass the parameter thread_logging=False to the LoggerFlow constructor);
     - minor fixes;
-  - v0.0.1 
+  - v.0.0.1 
     - create project LoggerFlow;
 </details>
 
 ```
 from loggerflow.backends.telegram import TelegramBackend
 from loggerflow import LoggerFlow
```

### Comparing `loggerflow-0.0.2/README.md` & `loggerflow-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -9,20 +9,28 @@
 ```
 
 A new level of bug tracking for your Python projects.
 
 
 <h5> Simple start (with Telegram backend): </h5>
 <details>
-  <summary>Changes (0.0.2 - actual)</summary>
+  <summary>Changes (0.0.3 - actual)</summary>
 
+  - v.0.0.3
+    - added the `traceback='full'` attribute to the LoggerFlow constructor, which allows you to send full, clean or minimal traceback to the backend (depending on your preferences).
+    You can pass 3 parameters:
+        - `full` -  Sending full traceback on your backend/backends;
+        - `clean` - Sending your program's stacktrace (clearing lines that were are called from libraries);
+        - `minimal` - Sending a 1 line with name file, number line and last line of your traceback;
+    - minor fixes in project architecture;
+    - writing documentation for project.
   - v.0.0.2
-    - add logging in threads (to disable logging in threads - pass the parameter thread_logging=False to the LoggerFlow constructor);
+    - added logging in threads (to disable logging in threads - pass the parameter thread_logging=False to the LoggerFlow constructor);
     - minor fixes;
-  - v0.0.1 
+  - v.0.0.1 
     - create project LoggerFlow;
 </details>
 
 ```
 from loggerflow.backends.telegram import TelegramBackend
 from loggerflow import LoggerFlow
```

### Comparing `loggerflow-0.0.2/loggerflow/backends/discord.py` & `loggerflow-0.0.3/loggerflow/backends/discord.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 from loggerflow.backends.abstract_backend import AbstractBackend
 from loggerflow.backends.filters import Filter
 
 from discordwebhook import Discord
 
 
 class DiscordBackend(AbstractBackend, Filter):
-    """
-    TODO write docstring
-    """
     def __init__(self, webhook_url: str, authors: list = None):
         self.webhook_url = webhook_url
         self.authors = authors
         self.discord = Discord(url=self.webhook_url)
 
     def write_flow(self, text: str, project_name: str):
-        if 'Traceback (most recent call last):' in text:
-            if not any(note in text for note in self.filters):
-                try:
-                    authors = '\nAuthors: ' + ', '.join(self.authors) if self.authors else ''
-                    self.discord.post(content=f'Project: {project_name}{authors}\n\n' + text)
-                except Exception:
-                    pass
+        if not any(note in text for note in self.filters):
+            try:
+                authors = '\nAuthors: ' + ', '.join(self.authors) if self.authors else ''
+                self.discord.post(content=f'Project: {project_name}{authors}\n\n' + text)
+            except Exception:
+                pass
```

### Comparing `loggerflow-0.0.2/loggerflow/backends/telegram.py` & `loggerflow-0.0.3/loggerflow/backends/telegram.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 from loggerflow.backends.abstract_backend import AbstractBackend
 from loggerflow.backends.filters import Filter
 import requests
 
 
 class TelegramBackend(AbstractBackend, Filter):
-    """
-    TODO write docstring
-    """
     def __init__(self, token: str, chat_id: int,  authors: list = None):
         self.token = token
         self.chat_id = chat_id
         self.authors = authors
         self.traceback_filters.append('A request to the Telegram API was unsuccessful')
 
-    def write_flow(self, text: str, project_name: str = None):
-        if 'Traceback (most recent call last):' in text:
-            if not any(note in text for note in self.filters):
-                try:
-                    authors = '\nAuthors: ' + ', '.join(self.authors) if self.authors else ''
-                    url = f"https://api.telegram.org/bot{self.token}/sendMessage"
-                    data = {"chat_id": self.chat_id, "text": f'Project: {project_name}{authors}\n\n' + text}
-                    requests.post(url, data=data)
-                except Exception:
-                    pass
+    def write_flow(self, text: str, project_name: str):
+        if not any(note in text for note in self.filters):
+            try:
+                authors = '\nAuthors: ' + ', '.join(self.authors) if self.authors else ''
+                url = f"https://api.telegram.org/bot{self.token}/sendMessage"
+                data = {"chat_id": self.chat_id, "text": f'Project: {project_name}{authors}\n\n' + text}
+                requests.post(url, data=data)
+            except Exception:
+                pass
```

### Comparing `loggerflow-0.0.2/loggerflow.egg-info/PKG-INFO` & `loggerflow-0.0.3/loggerflow.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: loggerflow
-Version: 0.0.2
+Version: 0.0.3
 Summary: A new level of bug tracking for your Python projects
 Home-page: https://github.com/DeNRuDi/loggerflow
-Author: DeNRuDi, kad1m
+Author: DeNRuDi
 Author-email: denisrudnitskiy0@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -28,20 +28,28 @@
 ```
 
 A new level of bug tracking for your Python projects.
 
 
 <h5> Simple start (with Telegram backend): </h5>
 <details>
-  <summary>Changes (0.0.2 - actual)</summary>
+  <summary>Changes (0.0.3 - actual)</summary>
 
+  - v.0.0.3
+    - added the `traceback='full'` attribute to the LoggerFlow constructor, which allows you to send full, clean or minimal traceback to the backend (depending on your preferences).
+    You can pass 3 parameters:
+        - `full` -  Sending full traceback on your backend/backends;
+        - `clean` - Sending your program's stacktrace (clearing lines that were are called from libraries);
+        - `minimal` - Sending a 1 line with name file, number line and last line of your traceback;
+    - minor fixes in project architecture;
+    - writing documentation for project.
   - v.0.0.2
-    - add logging in threads (to disable logging in threads - pass the parameter thread_logging=False to the LoggerFlow constructor);
+    - added logging in threads (to disable logging in threads - pass the parameter thread_logging=False to the LoggerFlow constructor);
     - minor fixes;
-  - v0.0.1 
+  - v.0.0.1 
     - create project LoggerFlow;
 </details>
 
 ```
 from loggerflow.backends.telegram import TelegramBackend
 from loggerflow import LoggerFlow
```

### Comparing `loggerflow-0.0.2/setup.py` & `loggerflow-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 
-version = '0.0.2'
+version = '0.0.3'
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='loggerflow',
     version=version,
     packages=find_packages(),
     url='https://github.com/DeNRuDi/loggerflow',
-    author='DeNRuDi, kad1m',
+    author='DeNRuDi',
     author_email='denisrudnitskiy0@gmail.com',
     description='A new level of bug tracking for your Python projects',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'requests',
         'discordwebhook',
```

