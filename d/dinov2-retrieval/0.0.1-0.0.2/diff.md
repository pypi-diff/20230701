# Comparing `tmp/dinov2_retrieval-0.0.1.tar.gz` & `tmp/dinov2_retrieval-0.0.2.tar.gz`

## Comparing `dinov2_retrieval-0.0.1.tar` & `dinov2_retrieval-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 dinov2_retrieval-0.0.1/src/dinov2_retrieval/__init__.py
--rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 dinov2_retrieval-0.0.1/src/dinov2_retrieval/image_retriever.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 dinov2_retrieval-0.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 dinov2_retrieval-0.0.1/LICENSE
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 dinov2_retrieval-0.0.1/README.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 dinov2_retrieval-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 dinov2_retrieval-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 dinov2_retrieval-0.0.2/src/dinov2_retrieval/__init__.py
+-rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 dinov2_retrieval-0.0.2/src/dinov2_retrieval/image_retriever.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 dinov2_retrieval-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 dinov2_retrieval-0.0.2/LICENSE
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 dinov2_retrieval-0.0.2/README.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 dinov2_retrieval-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 dinov2_retrieval-0.0.2/PKG-INFO
```

### Comparing `dinov2_retrieval-0.0.1/src/dinov2_retrieval/__init__.py` & `dinov2_retrieval-0.0.2/src/dinov2_retrieval/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,20 +27,22 @@
         default="output",
         help="root folder to save output results",
     )
     parser.add_argument(
         "-q",
         "--query",
         type=str,
+        required=True,
         help="path to a query image file or image folder",
     )
     parser.add_argument(
         "-d",
         "--database",
         type=str,
+        required=True,
         help="path to the database image file or image folder",
     )
     parser.add_argument(
         "-n",
         "--num",
         type=int,
         default=1,
@@ -53,15 +55,15 @@
         help="image output size",
     )
     parser.add_argument(
         "-m",
         "--margin",
         type=int,
         default=10,
-        choices=range(0, 100),
+        choices=range(0, 105, 5),
         help="margin size (in pixel) between concatenated images",
     )
     parser.add_argument(
         "--disable-cache",
         action="store_true",
         help="don't cache database features, will extract features each time, quite time-consuming for large database",
     )
```

### Comparing `dinov2_retrieval-0.0.1/src/dinov2_retrieval/image_retriever.py` & `dinov2_retrieval-0.0.2/src/dinov2_retrieval/image_retriever.py`

 * *Files identical despite different names*

### Comparing `dinov2_retrieval-0.0.1/.gitignore` & `dinov2_retrieval-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dinov2_retrieval-0.0.1/LICENSE` & `dinov2_retrieval-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dinov2_retrieval-0.0.1/pyproject.toml` & `dinov2_retrieval-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dinov2-retrieval"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Yunfeng Wang", email="wyf.brz@gmail.com" },
 ]
 description = "A cli program of image retrieval using dinov2"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dinov2_retrieval-0.0.1/PKG-INFO` & `dinov2_retrieval-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dinov2-retrieval
-Version: 0.0.1
+Version: 0.0.2
 Summary: A cli program of image retrieval using dinov2
 Project-URL: Homepage, https://github.com/vra/dinov2-retrieval
 Project-URL: Bug Tracker, https://github.com/vra/dinov2-retrieval/issues
 Author-email: Yunfeng Wang <wyf.brz@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

