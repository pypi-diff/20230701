# Comparing `tmp/spark_quality_rules_tools-0.3.5.tar.gz` & `tmp/spark_quality_rules_tools-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.3.5.tar", last modified: Sat Jul  1 20:59:26 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.3.6.tar", last modified: Sat Jul  1 21:41:31 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.3.5.tar` & `spark_quality_rules_tools-0.3.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 20:59:26.380630 spark_quality_rules_tools-0.3.5/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.5/LICENSE
--rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4041 2023-07-01 20:59:26.380630 spark_quality_rules_tools-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.3.5/README.md
--rw-rw-rw-   0        0        0      643 2023-06-14 13:22:39.000000 spark_quality_rules_tools-0.3.5/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-01 20:59:26.380630 spark_quality_rules_tools-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-07-01 20:59:06.000000 spark_quality_rules_tools-0.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 20:59:26.366580 spark_quality_rules_tools-0.3.5/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     2235 2023-07-01 20:58:29.000000 spark_quality_rules_tools-0.3.5/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 20:59:26.378582 spark_quality_rules_tools-0.3.5/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.5/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    43061 2023-07-01 20:58:29.000000 spark_quality_rules_tools-0.3.5/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-07-01 20:59:26.380630 spark_quality_rules_tools-0.3.5/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.5/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.5/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.5/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-07-01 20:59:26.380630 spark_quality_rules_tools-0.3.5/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.5/spark_quality_rules_tools/utils/resource/resolve_edge.conf
--rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.5/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
--rw-rw-rw-   0        0        0    25817 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.5/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     3742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.5/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-07-01 20:59:26.377582 spark_quality_rules_tools-0.3.5/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     4041 2023-07-01 20:59:26.000000 spark_quality_rules_tools-0.3.5/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      784 2023-07-01 20:59:26.000000 spark_quality_rules_tools-0.3.5/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 20:59:26.000000 spark_quality_rules_tools-0.3.5/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2023-07-01 20:59:26.000000 spark_quality_rules_tools-0.3.5/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-07-01 20:59:26.000000 spark_quality_rules_tools-0.3.5/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 21:41:31.686282 spark_quality_rules_tools-0.3.6/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4041 2023-07-01 21:41:31.686282 spark_quality_rules_tools-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.3.6/README.md
+-rw-rw-rw-   0        0        0      661 2023-07-01 21:30:21.000000 spark_quality_rules_tools-0.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-01 21:41:31.687282 spark_quality_rules_tools-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-07-01 21:41:18.000000 spark_quality_rules_tools-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:41:31.663278 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     2342 2023-07-01 21:41:18.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:41:31.682282 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    45106 2023-07-01 21:41:18.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:41:31.684282 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:41:31.686282 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/resource/resolve_edge.conf
+-rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
+-rw-rw-rw-   0        0        0    25817 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     3742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:41:31.680281 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     4041 2023-07-01 21:41:31.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      784 2023-07-01 21:41:31.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 21:41:31.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      186 2023-07-01 21:41:31.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-07-01 21:41:31.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.3.5/LICENSE` & `spark_quality_rules_tools-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.5/PKG-INFO` & `spark_quality_rules_tools-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_quality_rules_tools
-Version: 0.3.5
+Version: 0.3.6
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.3.5/README.md` & `spark_quality_rules_tools-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.5/pyproject.toml` & `spark_quality_rules_tools-0.3.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 numpy = "1.24.3"
 pyarrow = "12.0.0"
 setuptools = "58.2.0"
 wheel = "0.40.0"
 spark-dataframe-tools = "^0.2.0"
 color-tools = "^0.0.2"
 pyhocon = "^0.3.60"
+tqdm = "^4.65.0"
 
 
 [tool.poetry.group.dev.dependencies]
 jupyterlab = "^4.0.0"
 twine = "^4.0.2"
 
 [build-system]
```

### Comparing `spark_quality_rules_tools-0.3.5/setup.py` & `spark_quality_rules_tools-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.3.5',
+    version='0.3.6',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.3.5/spark_quality_rules_tools/__init__.py` & `spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,38 +3,51 @@
 from spark_quality_rules_tools.functions.generator import dq_extract_parameters_artifactory
 from spark_quality_rules_tools.functions.generator import dq_extract_parameters_file
 from spark_quality_rules_tools.functions.generator import dq_path_workspace
 from spark_quality_rules_tools.functions.generator import dq_run_sandbox_artifactory
 from spark_quality_rules_tools.functions.generator import dq_run_sandbox_file
 from spark_quality_rules_tools.functions.generator import dq_run_sandbox_file_with_rules
 from spark_quality_rules_tools.functions.generator import dq_spark_session
+from spark_quality_rules_tools.functions.generator import dq_validate_artifactory
+from spark_quality_rules_tools.functions.generator import dq_validate_artifactory_with_rules
 from spark_quality_rules_tools.functions.generator import dq_validate_conf_artifactory
 from spark_quality_rules_tools.functions.generator import dq_validate_conf_file
-from spark_quality_rules_tools.functions.generator import dq_validate_rules_artifactory
-from spark_quality_rules_tools.functions.generator import dq_validate_rules_file
+from spark_quality_rules_tools.functions.generator import dq_validate_file
+from spark_quality_rules_tools.functions.generator import dq_validate_file_with_rules
 from spark_quality_rules_tools.utils import BASE_DIR
 from spark_quality_rules_tools.utils.color import get_color
 from spark_quality_rules_tools.utils.color import get_color_b
 from spark_quality_rules_tools.utils.resolve import get_replace_resolve_parameter
 from spark_quality_rules_tools.utils.rules import get_validate_rules
 
-generator_all = ["dq_creating_directory",
-                 "dq_spark_session",
-                 "dq_path_workspace",
-                 "dq_download_jar",
-                 "dq_extract_parameters_artifactory",
-                 "dq_run_sandbox_artifactory",
-                 "dq_validate_rules_artifactory",
-                 "dq_validate_conf_artifactory",
-                 "dq_extract_parameters_file",
-                 "dq_run_sandbox_file",
-                 "dq_run_sandbox_file_with_rules"
-                 "dq_validate_conf_file",
-                 "dq_validate_rules_file"
-                 ]
-utils_all = ["BASE_DIR",
-             "get_color",
-             "get_color_b",
-             "get_replace_resolve_parameter",
-             "get_validate_rules"]
+generator_all = [
+    "dq_creating_directory",
+    "dq_spark_session",
+    "dq_path_workspace",
+    "dq_download_jar"
+]
+generator_artifactory = [
+    "dq_validate_conf_artifactory",
+    "dq_extract_parameters_artifactory",
+    "dq_run_sandbox_artifactory",
+    "dq_validate_rules_artifactory",
+    "dq_validate_artifactory",
+    "dq_validate_artifactory_with_rules"
+]
+
+generator_file = [
+    "dq_validate_conf_file",
+    "dq_extract_parameters_file",
+    "dq_run_sandbox_file",
+    "dq_run_sandbox_file_with_rules"
+    "dq_validate_file",
+    "dq_validate_file_with_rules"
+]
+
+utils_all = [
+    "BASE_DIR",
+    "get_color",
+    "get_color_b",
+    "get_replace_resolve_parameter"
+]
 
 __all__ = generator_all + utils_all
```

### Comparing `spark_quality_rules_tools-0.3.5/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/functions/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -833,15 +833,15 @@
     print(f"{get_color('table name:')} {get_color_b(table_name)}")
     print(f"{get_color('conf name :')} {get_color_b(url_conf_name)}")
     print(f"{get_color('cutoff date:')} {get_color_b(cutoff_date)}")
     print(f"{get_color('Generating a file csv:')} {get_color_b(dir_reports_name_filename)}")
     print(f"{get_color('=================================')} ")
 
 
-def dq_validate_rules_artifactory(url_conf=None):
+def dq_validate_artifactory(url_conf=None):
     import sys
     import os
     from spark_quality_rules_tools import get_validate_rules
 
     is_windows = sys.platform.startswith('win')
     dir_hocons_name = os.getenv('pj_dq_dir_hocons_name')
 
@@ -857,15 +857,15 @@
 
     dir_hocons_filename = os.path.join(dir_hocons_name, uuaa_name, f"{url_conf_name}.conf")
     if is_windows:
         dir_hocons_filename = dir_hocons_filename.replace("\\", "/")
     get_validate_rules(hocons_dir=dir_hocons_filename)
 
 
-def dq_validate_rules_file(file_conf=None, uuaa=None):
+def dq_validate_file(file_conf=None, uuaa=None):
     import sys
     import os
     from spark_quality_rules_tools import get_validate_rules
 
     is_windows = sys.platform.startswith('win')
     dir_hocons_name = os.getenv('pj_dq_dir_hocons_name')
 
@@ -875,7 +875,63 @@
     if file_conf in ("", None):
         raise Exception(f'required variable file_conf')
 
     dir_hocons_filename = os.path.join(dir_hocons_name, uuaa_name, f"{url_conf_name}.conf")
     if is_windows:
         dir_hocons_filename = dir_hocons_filename.replace("\\", "/")
     get_validate_rules(hocons_dir=dir_hocons_filename)
+
+
+def dq_validate_artifactory_with_rules(file_conf=None,
+                                       rules_id=None,
+                                       uuaa=None):
+    import sys
+    import os
+    from spark_quality_rules_tools import get_validate_rules
+
+    is_windows = sys.platform.startswith('win')
+    dir_hocons_name = os.getenv('pj_dq_dir_hocons_name')
+
+    url_conf_name = str(str(file_conf).split(".")[0])
+    uuaa_name = str(uuaa).upper()
+
+    if file_conf in ("", None):
+        raise Exception(f'required variable file_conf')
+
+    id_split = str(rules_id).split("_")
+    rule_country = str(id_split[0])
+    rule_type = str(id_split[1])
+    rule_id = str(id_split[-2])
+    rule_correlative = str(id_split[-1])
+
+    dir_hocons_filename = os.path.join(dir_hocons_name, uuaa_name, f"{url_conf_name}_{rule_country}_{rule_type}_{rule_id}_{rule_correlative}.conf")
+    if is_windows:
+        dir_hocons_filename = dir_hocons_filename.replace("\\", "/")
+    get_validate_rules(hocons_dir=dir_hocons_filename)
+
+
+def dq_validate_file_with_rules(file_conf=None,
+                                rules_id=None,
+                                uuaa=None):
+    import sys
+    import os
+    from spark_quality_rules_tools import get_validate_rules
+
+    is_windows = sys.platform.startswith('win')
+    dir_hocons_name = os.getenv('pj_dq_dir_hocons_name')
+
+    url_conf_name = str(str(file_conf).split(".")[0])
+    uuaa_name = str(uuaa).upper()
+
+    if file_conf in ("", None):
+        raise Exception(f'required variable file_conf')
+
+    id_split = str(rules_id).split("_")
+    rule_country = str(id_split[0])
+    rule_type = str(id_split[1])
+    rule_id = str(id_split[-2])
+    rule_correlative = str(id_split[-1])
+
+    dir_hocons_filename = os.path.join(dir_hocons_name, uuaa_name, f"{url_conf_name}_{rule_country}_{rule_type}_{rule_id}_{rule_correlative}.conf")
+    if is_windows:
+        dir_hocons_filename = dir_hocons_filename.replace("\\", "/")
+    get_validate_rules(hocons_dir=dir_hocons_filename)
```

### Comparing `spark_quality_rules_tools-0.3.5/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.5/spark_quality_rules_tools/utils/resource/resolve_edge.conf` & `spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/resource/resolve_edge.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.5/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf` & `spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.5/spark_quality_rules_tools/utils/resource/rules.json` & `spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/resource/rules.json`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.5/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/rules.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.5/spark_quality_rules_tools.egg-info/PKG-INFO` & `spark_quality_rules_tools-0.3.6/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-quality-rules-tools
-Version: 0.3.5
+Version: 0.3.6
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.3.5/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.3.6/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

