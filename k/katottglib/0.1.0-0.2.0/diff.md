# Comparing `tmp/katottglib-0.1.0.tar.gz` & `tmp/katottglib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katottglib-0.1.0.tar", last modified: Sat Jun 10 09:58:17 2023, max compression
+gzip compressed data, was "katottglib-0.2.0.tar", last modified: Sat Jul  1 13:39:57 2023, max compression
```

## Comparing `katottglib-0.1.0.tar` & `katottglib-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-06-10 09:58:17.612125 katottglib-0.1.0/
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1073 2023-06-06 21:02:05.000000 katottglib-0.1.0/LICENSE
--rw-r--r--   0 dsenchishen   (502) staff       (20)      834 2023-06-10 09:58:17.612245 katottglib-0.1.0/PKG-INFO
--rw-r--r--   0 dsenchishen   (502) staff       (20)      263 2023-06-10 09:47:34.000000 katottglib-0.1.0/README.rst
-drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-06-10 09:58:17.610174 katottglib-0.1.0/data/
--rw-r--r--   0 dsenchishen   (502) staff       (20)       53 2023-06-06 21:02:05.000000 katottglib-0.1.0/data/__init__.py
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1242 2023-06-09 20:30:49.000000 katottglib-0.1.0/data/data.py
--rw-r--r--   0 dsenchishen   (502) staff       (20)      586 2023-06-06 21:02:05.000000 katottglib-0.1.0/data/entity.py
-drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-06-10 09:58:17.611423 katottglib-0.1.0/katottglib.egg-info/
--rw-r--r--   0 dsenchishen   (502) staff       (20)      834 2023-06-10 09:58:17.000000 katottglib-0.1.0/katottglib.egg-info/PKG-INFO
--rw-r--r--   0 dsenchishen   (502) staff       (20)      250 2023-06-10 09:58:17.000000 katottglib-0.1.0/katottglib.egg-info/SOURCES.txt
--rw-r--r--   0 dsenchishen   (502) staff       (20)        1 2023-06-10 09:58:17.000000 katottglib-0.1.0/katottglib.egg-info/dependency_links.txt
--rw-r--r--   0 dsenchishen   (502) staff       (20)       10 2023-06-10 09:58:17.000000 katottglib-0.1.0/katottglib.egg-info/top_level.txt
--rw-r--r--   0 dsenchishen   (502) staff       (20)      406 2023-06-06 21:02:05.000000 katottglib-0.1.0/pyproject.toml
--rw-r--r--   0 dsenchishen   (502) staff       (20)      639 2023-06-10 09:58:17.612663 katottglib-0.1.0/setup.cfg
--rw-r--r--   0 dsenchishen   (502) staff       (20)       38 2021-03-15 19:22:38.000000 katottglib-0.1.0/setup.py
-drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-06-10 09:58:17.611679 katottglib-0.1.0/test/
--rw-r--r--   0 dsenchishen   (502) staff       (20)     1878 2023-06-09 20:22:51.000000 katottglib-0.1.0/test/__init__.py
+drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-01 13:39:57.242864 katottglib-0.2.0/
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1073 2023-06-06 21:02:05.000000 katottglib-0.2.0/LICENSE
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1094 2023-07-01 13:39:57.243000 katottglib-0.2.0/PKG-INFO
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      523 2023-07-01 13:21:46.000000 katottglib-0.2.0/README.rst
+drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-01 13:39:57.240577 katottglib-0.2.0/data/
+-rw-r--r--   0 dsenchishen   (502) staff       (20)       53 2023-06-06 21:02:05.000000 katottglib-0.2.0/data/__init__.py
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1534 2023-07-01 12:09:31.000000 katottglib-0.2.0/data/data.py
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      586 2023-06-06 21:02:05.000000 katottglib-0.2.0/data/entity.py
+drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-01 13:39:57.242109 katottglib-0.2.0/katottglib.egg-info/
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1094 2023-07-01 13:39:57.000000 katottglib-0.2.0/katottglib.egg-info/PKG-INFO
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      250 2023-07-01 13:39:57.000000 katottglib-0.2.0/katottglib.egg-info/SOURCES.txt
+-rw-r--r--   0 dsenchishen   (502) staff       (20)        1 2023-07-01 13:39:57.000000 katottglib-0.2.0/katottglib.egg-info/dependency_links.txt
+-rw-r--r--   0 dsenchishen   (502) staff       (20)       10 2023-07-01 13:39:57.000000 katottglib-0.2.0/katottglib.egg-info/top_level.txt
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      406 2023-06-06 21:02:05.000000 katottglib-0.2.0/pyproject.toml
+-rw-r--r--   0 dsenchishen   (502) staff       (20)      639 2023-07-01 13:39:57.243519 katottglib-0.2.0/setup.cfg
+-rw-r--r--   0 dsenchishen   (502) staff       (20)       38 2021-03-15 19:22:38.000000 katottglib-0.2.0/setup.py
+drwxr-xr-x   0 dsenchishen   (502) staff       (20)        0 2023-07-01 13:39:57.242421 katottglib-0.2.0/test/
+-rw-r--r--   0 dsenchishen   (502) staff       (20)     1878 2023-06-09 20:22:51.000000 katottglib-0.2.0/test/__init__.py
```

### Comparing `katottglib-0.1.0/LICENSE` & `katottglib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `katottglib-0.1.0/PKG-INFO` & `katottglib-0.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katottglib
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python lib to operate KATOTTG addresses (classified administrative division of Ukraine).
 Home-page: https://github.com/sen-den/katottglib
 Author: Denis Senchishen
 Author-email: dsenchishen@icloud.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,19 +17,28 @@
 ===========
 KATOTTG lib
 ===========
 
 Quick start
 -----------
 
-To be done...
+- Install with `pip install katottglib`
+- Import `import katottglib`
+- Search for entities with `find_by_name` `katottglib.find_by_name(name="Lviv")`
 
 Release notes
 -------------
 
+v0.2.0 (2023-07-01)
+...................
+
+Fixes and improvements to performance.
+
+- Dataframe is now persisted with Pickle.
+
 v0.1.0 (2023-06-10)
 ...................
 
 Initial release.
 
 - Search by name with filter by level (``find_by_name``).
 - Search by identifier (``find_by_id``)
```

### Comparing `katottglib-0.1.0/data/data.py` & `katottglib-0.2.0/data/data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,43 @@
+import pandas as pd
 import os
 
-import pandas as pd
+DATA_FILE_PATH = "kodifikator_data.pkl"
 
 
 def load_xlsx() -> pd.DataFrame:
     script_dir = os.path.dirname(os.path.abspath(__file__))
     file_path = os.path.join(script_dir, "kodifikator.xlsx")
     df = pd.read_excel(file_path, skiprows=2, skipfooter=3)
     return df
 
 
 def load_data() -> pd.DataFrame:
-    df = load_xlsx()
-    df["id"] = df["Додатковий рівень"].fillna(
-        df["Четвертий рівень"].fillna(
-            df["Третій рівень"].fillna(
-                df["Другий рівень"].fillna(df["Перший рівень"])
+    if os.path.exists(DATA_FILE_PATH):
+        df = pd.read_pickle(DATA_FILE_PATH)
+    else:
+        df = load_xlsx()
+        df["id"] = df["Додатковий рівень"].fillna(
+            df["Четвертий рівень"].fillna(
+                df["Третій рівень"].fillna(
+                    df["Другий рівень"].fillna(df["Перший рівень"])
+                )
             )
         )
-    )
-    category_mapping = {
-        "O": "Області та АРК",
-        "K": "Міста зі спеціальним статусом (Київ та Севастополь)",
-        "P": "Райони в областях та в АРК",
-        "H": "Територіальні громади",
-        "M": "Міста",
-        "T": "Селища міського типу",
-        "C": "Села",
-        "X": "Селища",
-        "B": "Райони в містах",
-    }
-
-    df["Назва категорії об’єкта"] = df["Категорія об’єкта"].map(
-        category_mapping
-    )
+        category_mapping = {
+            "O": "Області та АРК",
+            "K": "Міста зі спеціальним статусом (Київ та Севастополь)",
+            "P": "Райони в областях та в АРК",
+            "H": "Територіальні громади",
+            "M": "Міста",
+            "T": "Селища міського типу",
+            "C": "Села",
+            "X": "Селища",
+            "B": "Райони в містах",
+        }
+
+        df["Назва категорії об’єкта"] = df["Категорія об’єкта"].map(
+            category_mapping
+        )
+        df.to_pickle(DATA_FILE_PATH)  # Persist the DataFrame to disk
+
     return df
```

### Comparing `katottglib-0.1.0/data/entity.py` & `katottglib-0.2.0/data/entity.py`

 * *Files identical despite different names*

### Comparing `katottglib-0.1.0/katottglib.egg-info/PKG-INFO` & `katottglib-0.2.0/katottglib.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katottglib
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python lib to operate KATOTTG addresses (classified administrative division of Ukraine).
 Home-page: https://github.com/sen-den/katottglib
 Author: Denis Senchishen
 Author-email: dsenchishen@icloud.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,19 +17,28 @@
 ===========
 KATOTTG lib
 ===========
 
 Quick start
 -----------
 
-To be done...
+- Install with `pip install katottglib`
+- Import `import katottglib`
+- Search for entities with `find_by_name` `katottglib.find_by_name(name="Lviv")`
 
 Release notes
 -------------
 
+v0.2.0 (2023-07-01)
+...................
+
+Fixes and improvements to performance.
+
+- Dataframe is now persisted with Pickle.
+
 v0.1.0 (2023-06-10)
 ...................
 
 Initial release.
 
 - Search by name with filter by level (``find_by_name``).
 - Search by identifier (``find_by_id``)
```

### Comparing `katottglib-0.1.0/setup.cfg` & `katottglib-0.2.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = katottglib
-version = 0.1.0
+version = 0.2.0
 description = A Python lib to operate KATOTTG addresses (classified administrative division of Ukraine).
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/sen-den/katottglib
 author = Denis Senchishen
 author_email = dsenchishen@icloud.com
 license = MIT
```

### Comparing `katottglib-0.1.0/test/__init__.py` & `katottglib-0.2.0/test/__init__.py`

 * *Files identical despite different names*

