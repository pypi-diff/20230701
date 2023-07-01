# Comparing `tmp/json_to_csv_filter-1.3.tar.gz` & `tmp/json_to_csv_filter-1.3.1.tar.gz`

## Comparing `json_to_csv_filter-1.3.tar` & `json_to_csv_filter-1.3.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/deploy.sh
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/requirements.txt
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/.idea/.gitignore
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/.idea/json_to_csv.iml
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/.idea/vcs.xml
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/src/json_to_csv_filter/__init__.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/src/json_to_csv_filter/json_to_csv.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/LICENSE
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/README.md
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/pyproject.toml
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/PKG-INFO
+-rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/deploy.sh
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/.idea/.gitignore
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/.idea/json_to_csv.iml
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/src/json_to_csv_filter/__init__.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/src/json_to_csv_filter/json_to_csv.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/LICENSE
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/README.md
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/PKG-INFO
```

### Comparing `json_to_csv_filter-1.3/.github/workflows/python-package.yml` & `json_to_csv_filter-1.3.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `json_to_csv_filter-1.3/.idea/workspace.xml` & `json_to_csv_filter-1.3.1/.idea/workspace.xml`

 * *Files 10% similar despite different names*

#### Comparing `json_to_csv_filter-1.3/.idea/workspace.xml` & `json_to_csv_filter-1.3.1/.idea/workspace.xml`

```diff
@@ -1,18 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="3ce160a4-54f9-4e48-b828-419d5587133a" name="Changes" comment="renamed package">
-      <change afterPath="$PROJECT_DIR$/deploy.sh" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/json_to_csv_filter/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/json_to_csv_filter/__init__.py" afterDir="false"/>
-    </list>
+    <list default="true" id="3ce160a4-54f9-4e48-b828-419d5587133a" name="Changes" comment="renamed package"/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
```

### Comparing `json_to_csv_filter-1.3/src/json_to_csv_filter/json_to_csv.py` & `json_to_csv_filter-1.3.1/src/json_to_csv_filter/json_to_csv.py`

 * *Files identical despite different names*

### Comparing `json_to_csv_filter-1.3/.gitignore` & `json_to_csv_filter-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `json_to_csv_filter-1.3/LICENSE` & `json_to_csv_filter-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `json_to_csv_filter-1.3/README.md` & `json_to_csv_filter-1.3.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-# json-to-csv
+# Description
+Converts a list of json objects to a csv with optional filtering, sorting and date formatting.
+
+# Usage
+```bash
 usage: json_to_csv.py [-h] [-i [INCLUDE ...]] [-e [EXCLUDE ...]] [-o [ORDER ...]] [-n [NUMBER]] [-d [DATE_FIELDS ...]] [-df [DATE_FORMAT]]
                       [infile] [outfile]
 
 Convert list of json objects to csv
 
 positional arguments:
   infile                Input file, defaults to STDIN
@@ -17,8 +21,9 @@
   -o [ORDER ...], --order [ORDER ...]
                         Order fields, defaults to none
   -n [NUMBER], --number [NUMBER]
                         Number of records to process, defaults to all
   -d [DATE_FIELDS ...], --date-fields [DATE_FIELDS ...]
                         Date fields, defaults to none
   -df [DATE_FORMAT], --date-format [DATE_FORMAT]
-                        Datetime format, defaults to none
+                        Datetime format, defaults to none
+```
```

### Comparing `json_to_csv_filter-1.3/pyproject.toml` & `json_to_csv_filter-1.3.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    'python-dateutil ~= 2.8.2'
+]
 
 [project.urls]
 "Homepage" = "https://github.com/hylkefoeken/json-to-csv"
 "Bug Tracker" = "https://github.com/hylkefoeken/json-to-csv/issues"
 
 [project.scripts]
 json2csv = "json_to_csv_filter.json_to_csv:main"
```

### Comparing `json_to_csv_filter-1.3/PKG-INFO` & `json_to_csv_filter-1.3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: json_to_csv_filter
-Version: 1.3
+Version: 1.3.1
 Summary: Convert list of json objects to csv with optional filters
 Project-URL: Homepage, https://github.com/hylkefoeken/json-to-csv
 Project-URL: Bug Tracker, https://github.com/hylkefoeken/json-to-csv/issues
 Author-email: Hylke Foeken <h.foeken@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: python-dateutil~=2.8.2
 Description-Content-Type: text/markdown
 
-# json-to-csv
+# Description
+Converts a list of json objects to a csv with optional filtering, sorting and date formatting.
+
+# Usage
+```bash
 usage: json_to_csv.py [-h] [-i [INCLUDE ...]] [-e [EXCLUDE ...]] [-o [ORDER ...]] [-n [NUMBER]] [-d [DATE_FIELDS ...]] [-df [DATE_FORMAT]]
                       [infile] [outfile]
 
 Convert list of json objects to csv
 
 positional arguments:
   infile                Input file, defaults to STDIN
@@ -31,8 +36,9 @@
   -o [ORDER ...], --order [ORDER ...]
                         Order fields, defaults to none
   -n [NUMBER], --number [NUMBER]
                         Number of records to process, defaults to all
   -d [DATE_FIELDS ...], --date-fields [DATE_FIELDS ...]
                         Date fields, defaults to none
   -df [DATE_FORMAT], --date-format [DATE_FORMAT]
-                        Datetime format, defaults to none
+                        Datetime format, defaults to none
+```
```

