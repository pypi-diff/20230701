# Comparing `tmp/combidata-0.2.1.tar.gz` & `tmp/combidata-0.2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "combidata-0.2.1.tar", last modified: Fri Jun 30 14:19:17 2023, max compression
+gzip compressed data, was "combidata-0.2.1.1.tar", last modified: Sat Jul  1 12:23:55 2023, max compression
```

## Comparing `combidata-0.2.1.tar` & `combidata-0.2.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 14:19:17.850964 combidata-0.2.1/
--rw-rw-rw-   0        0        0     1083 2022-11-07 15:57:18.000000 combidata-0.2.1/LICENSE
--rw-rw-rw-   0        0        0    10465 2023-06-30 14:19:17.849966 combidata-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     9684 2023-06-30 14:16:48.000000 combidata-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 14:19:17.793961 combidata-0.2.1/combidata/
--rw-rw-rw-   0        0        0      395 2023-02-10 13:56:29.000000 combidata-0.2.1/combidata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 14:19:17.829962 combidata-0.2.1/combidata/classes/
--rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.1/combidata/classes/__init__.py
--rw-rw-rw-   0        0        0     2831 2023-04-01 06:03:08.000000 combidata-0.2.1/combidata/classes/case.py
--rw-rw-rw-   0        0        0     2161 2023-06-30 13:44:01.000000 combidata-0.2.1/combidata/classes/combination.py
--rw-rw-rw-   0        0        0     6255 2023-06-30 14:01:33.000000 combidata-0.2.1/combidata/classes/data_generator.py
--rw-rw-rw-   0        0        0      351 2023-03-02 16:58:22.000000 combidata-0.2.1/combidata/classes/process.py
-drwxrwxrwx   0        0        0        0 2023-06-30 14:19:17.844967 combidata-0.2.1/combidata/processes/
--rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.1/combidata/processes/__init__.py
--rw-rw-rw-   0        0        0     5249 2023-04-01 05:47:28.000000 combidata-0.2.1/combidata/processes/combine.py
--rw-rw-rw-   0        0        0      655 2023-02-16 18:09:16.000000 combidata-0.2.1/combidata/processes/form.py
--rw-rw-rw-   0        0        0     1924 2023-04-01 06:30:40.000000 combidata-0.2.1/combidata/processes/genetate.py
-drwxrwxrwx   0        0        0        0 2023-06-30 14:19:17.820967 combidata-0.2.1/combidata.egg-info/
--rw-rw-rw-   0        0        0    10465 2023-06-30 14:19:17.000000 combidata-0.2.1/combidata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-06-30 14:19:17.000000 combidata-0.2.1/combidata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 14:19:17.000000 combidata-0.2.1/combidata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-30 14:19:17.000000 combidata-0.2.1/combidata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      553 2023-06-30 14:16:48.000000 combidata-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 14:19:17.850964 combidata-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1073 2023-06-30 14:16:48.000000 combidata-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 14:19:17.846969 combidata-0.2.1/tests/
--rw-rw-rw-   0        0        0     3511 2023-06-30 13:59:13.000000 combidata-0.2.1/tests/test_generator.py
+drwxrwxrwx   0        0        0        0 2023-07-01 12:23:55.497819 combidata-0.2.1.1/
+-rw-rw-rw-   0        0        0     1083 2022-11-07 15:57:18.000000 combidata-0.2.1.1/LICENSE
+-rw-rw-rw-   0        0        0    10467 2023-07-01 12:23:55.496775 combidata-0.2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9684 2023-06-30 14:16:48.000000 combidata-0.2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 12:23:55.456770 combidata-0.2.1.1/combidata/
+-rw-rw-rw-   0        0        0      395 2023-02-10 13:56:29.000000 combidata-0.2.1.1/combidata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 12:23:55.486770 combidata-0.2.1.1/combidata/classes/
+-rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.1.1/combidata/classes/__init__.py
+-rw-rw-rw-   0        0        0     2831 2023-04-01 06:03:08.000000 combidata-0.2.1.1/combidata/classes/case.py
+-rw-rw-rw-   0        0        0     2463 2023-07-01 12:20:32.000000 combidata-0.2.1.1/combidata/classes/combination.py
+-rw-rw-rw-   0        0        0     6255 2023-06-30 14:01:33.000000 combidata-0.2.1.1/combidata/classes/data_generator.py
+-rw-rw-rw-   0        0        0      351 2023-03-02 16:58:22.000000 combidata-0.2.1.1/combidata/classes/process.py
+drwxrwxrwx   0        0        0        0 2023-07-01 12:23:55.492773 combidata-0.2.1.1/combidata/processes/
+-rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.1.1/combidata/processes/__init__.py
+-rw-rw-rw-   0        0        0     5249 2023-04-01 05:47:28.000000 combidata-0.2.1.1/combidata/processes/combine.py
+-rw-rw-rw-   0        0        0      655 2023-02-16 18:09:16.000000 combidata-0.2.1.1/combidata/processes/form.py
+-rw-rw-rw-   0        0        0     1924 2023-04-01 06:30:40.000000 combidata-0.2.1.1/combidata/processes/genetate.py
+drwxrwxrwx   0        0        0        0 2023-07-01 12:23:55.479769 combidata-0.2.1.1/combidata.egg-info/
+-rw-rw-rw-   0        0        0    10467 2023-07-01 12:23:55.000000 combidata-0.2.1.1/combidata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-07-01 12:23:55.000000 combidata-0.2.1.1/combidata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 12:23:55.000000 combidata-0.2.1.1/combidata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-01 12:23:55.000000 combidata-0.2.1.1/combidata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      555 2023-07-01 12:23:28.000000 combidata-0.2.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-01 12:23:55.497819 combidata-0.2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-07-01 12:23:28.000000 combidata-0.2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 12:23:55.494775 combidata-0.2.1.1/tests/
+-rw-rw-rw-   0        0        0     3511 2023-06-30 13:59:13.000000 combidata-0.2.1.1/tests/test_generator.py
```

### Comparing `combidata-0.2.1/LICENSE` & `combidata-0.2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `combidata-0.2.1/PKG-INFO` & `combidata-0.2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combidata
-Version: 0.2.1
+Version: 0.2.1.1
 Summary: Package for random data generation, combination and data prepare for tests
 Home-page: https://github.com/Warrfie/combidata
 Author: Kuklikov Maxim (Warrfie)
 Author-email: "MaximKuklikov(Warrfie)" <warrfie@gmail.com>
 Project-URL: Homepage, https://github.com/Warrfie/combidata
 Keywords: QA,SET,random data generation,testing API,testing,autotesting
 Classifier: Development Status :: 4 - Beta
```

### Comparing `combidata-0.2.1/README.md` & `combidata-0.2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `combidata-0.2.1/combidata/classes/case.py` & `combidata-0.2.1.1/combidata/classes/case.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.1/combidata/classes/combination.py` & `combidata-0.2.1.1/combidata/classes/combination.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,16 +49,21 @@
 
     def run(self):
         self.workflow = list(self.workflow) if isinstance(self.workflow, list) else self.workflow  # todo beautify
         workflow = self.workflow.pop(0) if isinstance(self.workflow, list) else self.workflow
         for current_step in workflow:
             while step_not_done(current_step.name, self):
                 if self.step_done != current_step.name:
+                    if logger := self.tools.get("logger"):
+                        logger.start_step(self.tools.get("id"), current_step.name)
                     try:
                         current_step.activate(self)
                     except Exception as e:
                         self.step_done = "STOP"
                         if logger := self.tools.get("logger"):
-                            logger.end_test(self.tools.get("id"), str(e))
+                            logger.end_step(self.tools.get("id"), str(e))
                         else:
                             raise e
+                    else:
+                        if logger := self.tools.get("logger"):
+                            logger.end_step(self.tools.get("id"))
```

### Comparing `combidata-0.2.1/combidata/classes/data_generator.py` & `combidata-0.2.1.1/combidata/classes/data_generator.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.1/combidata/processes/combine.py` & `combidata-0.2.1.1/combidata/processes/combine.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.1/combidata/processes/form.py` & `combidata-0.2.1.1/combidata/processes/form.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.1/combidata/processes/genetate.py` & `combidata-0.2.1.1/combidata/processes/genetate.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.1/combidata.egg-info/PKG-INFO` & `combidata-0.2.1.1/combidata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combidata
-Version: 0.2.1
+Version: 0.2.1.1
 Summary: Package for random data generation, combination and data prepare for tests
 Home-page: https://github.com/Warrfie/combidata
 Author: Kuklikov Maxim (Warrfie)
 Author-email: "MaximKuklikov(Warrfie)" <warrfie@gmail.com>
 Project-URL: Homepage, https://github.com/Warrfie/combidata
 Keywords: QA,SET,random data generation,testing API,testing,autotesting
 Classifier: Development Status :: 4 - Beta
```

### Comparing `combidata-0.2.1/pyproject.toml` & `combidata-0.2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
     "testing API",
     "testing",
     "autotesting"
 ]
 urls = {Homepage = "https://github.com/Warrfie/combidata"}
 authors = [{name = "MaximKuklikov(Warrfie)", email = "warrfie@gmail.com"}]
 requires-python = ">=3.10"
-version="0.2.1"
+version="0.2.1.1"
```

### Comparing `combidata-0.2.1/setup.py` & `combidata-0.2.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name="combidata",
-    version="0.2.1",
+    version="0.2.1.1",
     description="Package for random data generation and combination different cases",
     long_description=long_description,
     url="https://github.com/Warrfie/combidata",
     author="Kuklikov Maxim (Warrfie)",
     author_email="warrfie@gmail.com",
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `combidata-0.2.1/tests/test_generator.py` & `combidata-0.2.1.1/tests/test_generator.py`

 * *Files identical despite different names*

