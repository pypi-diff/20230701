# Comparing `tmp/spinneroo-1.0.1.tar.gz` & `tmp/spinneroo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spinneroo-1.0.1.tar", last modified: Sat Jul  1 08:28:32 2023, max compression
+gzip compressed data, was "spinneroo-1.1.0.tar", last modified: Sat Jul  1 08:41:42 2023, max compression
```

## Comparing `spinneroo-1.0.1.tar` & `spinneroo-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 08:28:32.906203 spinneroo-1.0.1/
--rw-rw-rw-   0        0        0       98 2023-07-01 08:28:32.000000 spinneroo-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2032 2023-07-01 08:28:32.906203 spinneroo-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1240 2023-06-15 21:54:41.000000 spinneroo-1.0.1/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 spinneroo-1.0.1/build.py
--rw-rw-rw-   0        0        0      630 2023-07-01 08:28:32.000000 spinneroo-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-06-29 13:55:15.000000 spinneroo-1.0.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       21 2023-06-15 21:50:48.000000 spinneroo-1.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 08:28:32.906203 spinneroo-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1546 2023-07-01 08:28:27.000000 spinneroo-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 08:28:32.889625 spinneroo-1.0.1/spinneroo/
--rw-rw-rw-   0        0        0       83 2023-06-15 21:53:50.000000 spinneroo-1.0.1/spinneroo/__init__.py
--rw-rw-rw-   0        0        0       85 2023-06-15 21:52:57.000000 spinneroo-1.0.1/spinneroo/elements.py
--rw-rw-rw-   0        0        0     9908 2023-06-29 13:54:53.000000 spinneroo-1.0.1/spinneroo/progress.py
-drwxrwxrwx   0        0        0        0 2023-07-01 08:28:32.905237 spinneroo-1.0.1/spinneroo.egg-info/
--rw-rw-rw-   0        0        0     2032 2023-07-01 08:28:32.000000 spinneroo-1.0.1/spinneroo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-07-01 08:28:32.000000 spinneroo-1.0.1/spinneroo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 08:28:32.000000 spinneroo-1.0.1/spinneroo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-01 08:28:32.000000 spinneroo-1.0.1/spinneroo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-01 08:28:32.000000 spinneroo-1.0.1/spinneroo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 08:41:42.223305 spinneroo-1.1.0/
+-rw-rw-rw-   0        0        0       98 2023-07-01 08:41:41.000000 spinneroo-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2032 2023-07-01 08:41:42.223305 spinneroo-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1240 2023-06-15 21:54:41.000000 spinneroo-1.1.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 spinneroo-1.1.0/build.py
+-rw-rw-rw-   0        0        0      630 2023-07-01 08:41:41.000000 spinneroo-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-06-29 13:55:15.000000 spinneroo-1.1.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       21 2023-06-15 21:50:48.000000 spinneroo-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 08:41:42.223305 spinneroo-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1546 2023-07-01 08:41:38.000000 spinneroo-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 08:41:42.212465 spinneroo-1.1.0/spinneroo/
+-rw-rw-rw-   0        0        0       83 2023-06-15 21:53:50.000000 spinneroo-1.1.0/spinneroo/__init__.py
+-rw-rw-rw-   0        0        0       85 2023-06-15 21:52:57.000000 spinneroo-1.1.0/spinneroo/elements.py
+-rw-rw-rw-   0        0        0    10265 2023-07-01 08:41:05.000000 spinneroo-1.1.0/spinneroo/progress.py
+drwxrwxrwx   0        0        0        0 2023-07-01 08:41:42.222335 spinneroo-1.1.0/spinneroo.egg-info/
+-rw-rw-rw-   0        0        0     2032 2023-07-01 08:41:42.000000 spinneroo-1.1.0/spinneroo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-07-01 08:41:42.000000 spinneroo-1.1.0/spinneroo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 08:41:42.000000 spinneroo-1.1.0/spinneroo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-01 08:41:42.000000 spinneroo-1.1.0/spinneroo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-01 08:41:42.000000 spinneroo-1.1.0/spinneroo.egg-info/top_level.txt
```

### Comparing `spinneroo-1.0.1/PKG-INFO` & `spinneroo-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spinneroo
-Version: 1.0.1
+Version: 1.1.0
 Summary: A module for displaying progress messages and timers with spinners in the command line.
 Home-page: https://github.com/Shahaf-F-S/spinneroo
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `spinneroo-1.0.1/README.md` & `spinneroo-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `spinneroo-1.0.1/build.py` & `spinneroo-1.1.0/build.py`

 * *Files identical despite different names*

### Comparing `spinneroo-1.0.1/pyproject.toml` & `spinneroo-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'spinneroo'
-version = '1.0.1'
+version = '1.1.0'
 description = 'A module for displaying progress messages and timers with spinners in the command line.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `spinneroo-1.0.1/setup.py` & `spinneroo-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='spinneroo',
-        version='1.0.1',
+        version='1.1.0',
         description=(
             "A module for displaying progress messages and "
             "timers with spinners in the command line."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

### Comparing `spinneroo-1.0.1/spinneroo/progress.py` & `spinneroo-1.1.0/spinneroo/progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,14 +144,15 @@
         self.stay = stay
         self.counter = counter
         self.clean = clean
         self.elements = elements
 
         self.title = title or ""
         self.delay = delay or self.DELAY
+        self.cursor = elements[0]
 
         self._paused = False
 
         self._spinner_generator = self._spinning_cursor()
 
         self._running = False
 
@@ -218,14 +219,24 @@
             warnings.warn(
                 f"Attempting to pause {self} "
                 f"when the process is paused."
             )
         # end if
 
         self._paused = True
+
+        next_output = self.create_message(text="Paused")
+
+        sys.stdout.write(
+            ('\b' * len(self.output)) +
+            (' ' * len(self.output)) +
+            ('\b' * len(self.output)) +
+            next_output + "\n"
+        )
+        sys.stdout.flush()
     # end pause
 
     def unpause(self) -> None:
         """Unpauses the process."""
 
         if not self.paused:
             warnings.warn(
@@ -347,14 +358,16 @@
         :return: The current state of the cursor.
         """
 
         while True:
             for cursor in self.elements:
                 self.time = time.time()
 
+                self.cursor = cursor
+
                 if self.silence:
                     yield ""
                 # end if
 
                 self.output = self.create_message(
                     cursor=cursor, text=self.message
                 )
```

### Comparing `spinneroo-1.0.1/spinneroo.egg-info/PKG-INFO` & `spinneroo-1.1.0/spinneroo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spinneroo
-Version: 1.0.1
+Version: 1.1.0
 Summary: A module for displaying progress messages and timers with spinners in the command line.
 Home-page: https://github.com/Shahaf-F-S/spinneroo
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

