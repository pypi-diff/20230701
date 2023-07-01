# Comparing `tmp/f1_telemetry-2022.1.7.tar.gz` & `tmp/f1_telemetry-2023.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f1_telemetry-2022.1.7.tar", max compression
+gzip compressed data, was "f1_telemetry-2023.1.0.tar", max compression
```

## Comparing `f1_telemetry-2022.1.7.tar` & `f1_telemetry-2023.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1791 2023-04-25 16:25:48.881459 f1_telemetry-2022.1.7/README.md
--rw-r--r--   0        0        0        0 2023-04-25 16:25:48.897459 f1_telemetry-2022.1.7/f1_telemetry/__init__.py
--rw-r--r--   0        0        0     2307 2023-04-25 16:25:48.897459 f1_telemetry-2022.1.7/f1_telemetry/__main__.py
--rw-r--r--   0        0        0    16287 2023-04-25 16:25:48.897459 f1_telemetry-2022.1.7/f1_telemetry/collector.py
--rw-r--r--   0        0        0     1155 2023-04-25 16:25:48.897459 f1_telemetry-2022.1.7/f1_telemetry/live.py
--rw-r--r--   0        0        0     6082 2023-04-25 16:25:48.897459 f1_telemetry-2022.1.7/f1_telemetry/model.py
--rw-r--r--   0        0        0     2833 2023-04-25 16:25:48.897459 f1_telemetry-2022.1.7/f1_telemetry/report.py
--rw-r--r--   0        0        0      467 2023-04-25 16:25:48.897459 f1_telemetry-2022.1.7/f1_telemetry/server.py
--rw-r--r--   0        0        0     1393 2023-04-25 16:25:48.897459 f1_telemetry-2022.1.7/f1_telemetry/storage.py
--rw-r--r--   0        0        0     2742 2023-04-25 16:25:48.897459 f1_telemetry-2022.1.7/f1_telemetry/view.py
--rw-r--r--   0        0        0    73384 2023-04-25 16:25:48.901459 f1_telemetry-2022.1.7/f1_telemetry/webapp/art/Formula1-Regular.ttf
--rw-r--r--   0        0        0   203029 2023-04-25 16:25:48.901459 f1_telemetry-2022.1.7/f1_telemetry/webapp/art/bg.jpg
--rw-r--r--   0        0        0    33104 2023-04-25 16:25:48.901459 f1_telemetry-2022.1.7/f1_telemetry/webapp/art/car.svg
--rw-r--r--   0        0        0     5266 2023-04-25 16:25:48.901459 f1_telemetry-2022.1.7/f1_telemetry/webapp/index.html
--rw-r--r--   0        0        0    35177 2023-04-25 16:25:48.901459 f1_telemetry-2022.1.7/f1_telemetry/webapp/live.html
--rw-r--r--   0        0        0     6497 2023-04-25 16:25:48.901459 f1_telemetry-2022.1.7/f1_telemetry/webapp/live.js
--rw-r--r--   0        0        0     9991 2023-04-25 16:25:48.901459 f1_telemetry-2022.1.7/f1_telemetry/webapp/plots.js
--rw-r--r--   0        0        0     4647 2023-04-25 16:25:48.901459 f1_telemetry-2022.1.7/f1_telemetry/webapp/queries.js
--rw-r--r--   0        0        0     1321 2023-04-25 16:25:48.901459 f1_telemetry-2022.1.7/f1_telemetry/webapp/style.css
--rw-r--r--   0        0        0     3189 2023-04-25 16:25:48.901459 f1_telemetry-2022.1.7/f1_telemetry/webapp/trace.js
--rw-r--r--   0        0        0      787 2023-04-25 16:25:48.901459 f1_telemetry-2022.1.7/f1_telemetry/webapp/utils.js
--rw-r--r--   0        0        0     6089 2023-04-25 16:25:48.901459 f1_telemetry-2022.1.7/f1_telemetry/webapp/view.js
--rw-r--r--   0        0        0     1078 2023-04-25 16:25:59.061478 f1_telemetry-2022.1.7/pyproject.toml
--rw-r--r--   0        0        0     2911 1970-01-01 00:00:00.000000 f1_telemetry-2022.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1791 2023-07-01 18:43:26.339050 f1_telemetry-2023.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-01 18:43:26.359050 f1_telemetry-2023.1.0/f1_telemetry/__init__.py
+-rw-r--r--   0        0        0     2307 2023-07-01 18:43:26.359050 f1_telemetry-2023.1.0/f1_telemetry/__main__.py
+-rw-r--r--   0        0        0    16287 2023-07-01 18:43:26.359050 f1_telemetry-2023.1.0/f1_telemetry/collector.py
+-rw-r--r--   0        0        0     1155 2023-07-01 18:43:26.359050 f1_telemetry-2023.1.0/f1_telemetry/live.py
+-rw-r--r--   0        0        0     6082 2023-07-01 18:43:26.359050 f1_telemetry-2023.1.0/f1_telemetry/model.py
+-rw-r--r--   0        0        0     2833 2023-07-01 18:43:26.359050 f1_telemetry-2023.1.0/f1_telemetry/report.py
+-rw-r--r--   0        0        0      467 2023-07-01 18:43:26.359050 f1_telemetry-2023.1.0/f1_telemetry/server.py
+-rw-r--r--   0        0        0     1393 2023-07-01 18:43:26.359050 f1_telemetry-2023.1.0/f1_telemetry/storage.py
+-rw-r--r--   0        0        0     2742 2023-07-01 18:43:26.359050 f1_telemetry-2023.1.0/f1_telemetry/view.py
+-rw-r--r--   0        0        0    73384 2023-07-01 18:43:26.363050 f1_telemetry-2023.1.0/f1_telemetry/webapp/art/Formula1-Regular.ttf
+-rw-r--r--   0        0        0   203029 2023-07-01 18:43:26.363050 f1_telemetry-2023.1.0/f1_telemetry/webapp/art/bg.jpg
+-rw-r--r--   0        0        0    33104 2023-07-01 18:43:26.363050 f1_telemetry-2023.1.0/f1_telemetry/webapp/art/car.svg
+-rw-r--r--   0        0        0     5266 2023-07-01 18:43:26.363050 f1_telemetry-2023.1.0/f1_telemetry/webapp/index.html
+-rw-r--r--   0        0        0    35177 2023-07-01 18:43:26.363050 f1_telemetry-2023.1.0/f1_telemetry/webapp/live.html
+-rw-r--r--   0        0        0     6497 2023-07-01 18:43:26.363050 f1_telemetry-2023.1.0/f1_telemetry/webapp/live.js
+-rw-r--r--   0        0        0     9991 2023-07-01 18:43:26.363050 f1_telemetry-2023.1.0/f1_telemetry/webapp/plots.js
+-rw-r--r--   0        0        0     4647 2023-07-01 18:43:26.363050 f1_telemetry-2023.1.0/f1_telemetry/webapp/queries.js
+-rw-r--r--   0        0        0     1321 2023-07-01 18:43:26.363050 f1_telemetry-2023.1.0/f1_telemetry/webapp/style.css
+-rw-r--r--   0        0        0     3189 2023-07-01 18:43:26.363050 f1_telemetry-2023.1.0/f1_telemetry/webapp/trace.js
+-rw-r--r--   0        0        0      787 2023-07-01 18:43:26.363050 f1_telemetry-2023.1.0/f1_telemetry/webapp/utils.js
+-rw-r--r--   0        0        0     6089 2023-07-01 18:43:26.363050 f1_telemetry-2023.1.0/f1_telemetry/webapp/view.js
+-rw-r--r--   0        0        0     1078 2023-07-01 18:43:41.279284 f1_telemetry-2023.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2760 1970-01-01 00:00:00.000000 f1_telemetry-2023.1.0/PKG-INFO
```

### Comparing `f1_telemetry-2022.1.7/README.md` & `f1_telemetry-2023.1.0/README.md`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2022.1.7/f1_telemetry/__main__.py` & `f1_telemetry-2023.1.0/f1_telemetry/__main__.py`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2022.1.7/f1_telemetry/collector.py` & `f1_telemetry-2023.1.0/f1_telemetry/collector.py`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2022.1.7/f1_telemetry/live.py` & `f1_telemetry-2023.1.0/f1_telemetry/live.py`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2022.1.7/f1_telemetry/model.py` & `f1_telemetry-2023.1.0/f1_telemetry/model.py`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2022.1.7/f1_telemetry/report.py` & `f1_telemetry-2023.1.0/f1_telemetry/report.py`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2022.1.7/f1_telemetry/storage.py` & `f1_telemetry-2023.1.0/f1_telemetry/storage.py`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2022.1.7/f1_telemetry/view.py` & `f1_telemetry-2023.1.0/f1_telemetry/view.py`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2022.1.7/f1_telemetry/webapp/art/Formula1-Regular.ttf` & `f1_telemetry-2023.1.0/f1_telemetry/webapp/art/Formula1-Regular.ttf`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2022.1.7/f1_telemetry/webapp/art/bg.jpg` & `f1_telemetry-2023.1.0/f1_telemetry/webapp/art/bg.jpg`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2022.1.7/f1_telemetry/webapp/art/car.svg` & `f1_telemetry-2023.1.0/f1_telemetry/webapp/art/car.svg`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2022.1.7/f1_telemetry/webapp/index.html` & `f1_telemetry-2023.1.0/f1_telemetry/webapp/index.html`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2022.1.7/f1_telemetry/webapp/live.html` & `f1_telemetry-2023.1.0/f1_telemetry/webapp/live.html`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2022.1.7/f1_telemetry/webapp/live.js` & `f1_telemetry-2023.1.0/f1_telemetry/webapp/live.js`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2022.1.7/f1_telemetry/webapp/plots.js` & `f1_telemetry-2023.1.0/f1_telemetry/webapp/plots.js`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2022.1.7/f1_telemetry/webapp/queries.js` & `f1_telemetry-2023.1.0/f1_telemetry/webapp/queries.js`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2022.1.7/f1_telemetry/webapp/style.css` & `f1_telemetry-2023.1.0/f1_telemetry/webapp/style.css`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2022.1.7/f1_telemetry/webapp/trace.js` & `f1_telemetry-2023.1.0/f1_telemetry/webapp/trace.js`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2022.1.7/f1_telemetry/webapp/utils.js` & `f1_telemetry-2023.1.0/f1_telemetry/webapp/utils.js`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2022.1.7/f1_telemetry/webapp/view.js` & `f1_telemetry-2023.1.0/f1_telemetry/webapp/view.js`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2022.1.7/pyproject.toml` & `f1_telemetry-2023.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 authors = ["Gabriele N. Tornetta <phoenix1987@gmail.com>"]
 license = "MIT"
 packages = [
   {include = "f1_telemetry"},
 ]
 readme = "README.md"
 repository = "https://github.com/P403n1x87/f1-telemetry"
-version = "2022.1.7"
+version = "2023.1.0"
 
 [tool.isort]
 force_single_line = true
 lines_after_imports = 2
 profile = "black"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-f1-packets = "^2022.1.2"
+f1-packets = "^2023.1.0"
 influxdb-client = "^1.30.0"
 websockets = "^10.3"
 pyttsx3 = "2.71"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
```

### Comparing `f1_telemetry-2022.1.7/PKG-INFO` & `f1_telemetry-2023.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: f1-telemetry
-Version: 2022.1.7
+Version: 2023.1.0
 Summary: F1 telemetry data collection and visualisation
 Home-page: https://github.com/P403n1x87/f1-telemetry
 License: MIT
 Author: Gabriele N. Tornetta
 Author-email: phoenix1987@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: f1-packets (>=2022.1.2,<2023.0.0)
+Requires-Dist: f1-packets (>=2023.1.0,<2024.0.0)
 Requires-Dist: influxdb-client (>=1.30.0,<2.0.0)
 Requires-Dist: pyttsx3 (==2.71)
 Requires-Dist: websockets (>=10.3,<11.0)
 Project-URL: Repository, https://github.com/P403n1x87/f1-telemetry
 Project-URL: issues, https://github.com/P403n1x87/f1-telemetry/issues
 Description-Content-Type: text/markdown
```

