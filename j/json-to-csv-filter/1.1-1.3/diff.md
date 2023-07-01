# Comparing `tmp/json_to_csv_filter-1.1.tar.gz` & `tmp/json_to_csv_filter-1.3.tar.gz`

## Comparing `json_to_csv_filter-1.1.tar` & `json_to_csv_filter-1.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 json_to_csv_filter-1.1/requirements.txt
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 json_to_csv_filter-1.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 json_to_csv_filter-1.1/.idea/.gitignore
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 json_to_csv_filter-1.1/.idea/json_to_csv.iml
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 json_to_csv_filter-1.1/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 json_to_csv_filter-1.1/.idea/vcs.xml
--rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 json_to_csv_filter-1.1/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 json_to_csv_filter-1.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 json_to_csv_filter-1.1/src/json_to_csv_filter/__init__.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 json_to_csv_filter-1.1/src/json_to_csv_filter/json_to_csv.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 json_to_csv_filter-1.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 json_to_csv_filter-1.1/LICENSE
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 json_to_csv_filter-1.1/README.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 json_to_csv_filter-1.1/pyproject.toml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 json_to_csv_filter-1.1/PKG-INFO
+-rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/deploy.sh
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/requirements.txt
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/.idea/.gitignore
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/.idea/json_to_csv.iml
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/src/json_to_csv_filter/__init__.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/src/json_to_csv_filter/json_to_csv.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/LICENSE
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/README.md
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/pyproject.toml
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3/PKG-INFO
```

### Comparing `json_to_csv_filter-1.1/.github/workflows/python-package.yml` & `json_to_csv_filter-1.3/.github/workflows/python-package.yml`

 * *Files 11% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 on:
   push:
     branches: [ "main" ]
   pull_request:
     branches: [ "main" ]
 
 jobs:
-  build:
-
+  pypi-publish:
+    name: Upload release to PyPI
     runs-on: ubuntu-latest
-    strategy:
-      fail-fast: false
-      matrix:
-        python-version: ["3.8", "3.9", "3.10"]
-
+    environment:
+      name: pypi
+      url: https://pypi.org/p/json_to_csv_filter
+    permissions:
+      id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
@@ -33,12 +33,9 @@
       run: |
         # stop the build if there are Python syntax errors or undefined names
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
         # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
         flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
     - name: Build package
       run: python -m build
-    - name: Publish package
-      uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
-      with:
-        user: __token__
-        password: ${{ secrets.PYPI_API_TOKEN }}        
+    - name: Publish package distributions to PyPI
+      uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `json_to_csv_filter-1.1/.idea/workspace.xml` & `json_to_csv_filter-1.3/.idea/workspace.xml`

 * *Files 3% similar despite different names*

#### Comparing `json_to_csv_filter-1.1/.idea/workspace.xml` & `json_to_csv_filter-1.3/.idea/workspace.xml`

```diff
@@ -1,17 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="3ce160a4-54f9-4e48-b828-419d5587133a" name="Changes" comment="">
+    <list default="true" id="3ce160a4-54f9-4e48-b828-419d5587133a" name="Changes" comment="renamed package">
+      <change afterPath="$PROJECT_DIR$/deploy.sh" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/json_to_csv/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/json_to_csv_filter/__init__.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/json_to_csv/json_to_csv.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/json_to_csv_filter/json_to_csv.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/json_to_csv_filter/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/json_to_csv_filter/__init__.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -31,21 +31,21 @@
     <option name="stateVersion" value="1"/>
   </component>
   <component name="ProjectId" id="2QeGovvmF8FXOEDFaqt7BcvSr6V"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent"><![CDATA[{
-  "keyToString": {
-    "RunOnceActivity.ShowReadmeOnStart": "true",
-    "last_opened_file_path": "/Users/hylke/Projects/json_to_csv",
-    "settings.editor.selected.configurable": "org.jetbrains.plugins.github.ui.GithubSettingsConfigurable"
+  <component name="PropertiesComponent">{
+  &quot;keyToString&quot;: {
+    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
+    &quot;last_opened_file_path&quot;: &quot;/Users/hylke/Projects/json_to_csv&quot;,
+    &quot;settings.editor.selected.configurable&quot;: &quot;org.jetbrains.plugins.github.ui.GithubSettingsConfigurable&quot;
   }
-}]]></component>
+}</component>
   <component name="RecentsManager">
     <key name="MoveFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/src"/>
       <recent name="$PROJECT_DIR$/json_to_csv"/>
     </key>
   </component>
   <component name="RunManager" selected="Python.json_to_csv_file_output">
@@ -101,21 +101,33 @@
     <task active="true" id="Default" summary="Default task">
       <changelist id="3ce160a4-54f9-4e48-b828-419d5587133a" name="Changes" comment=""/>
       <created>1685706811532</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1685706811532</updated>
     </task>
+    <task id="LOCAL-00001" summary="renamed package">
+      <created>1687901189154</created>
+      <option name="number" value="00001"/>
+      <option name="presentableId" value="LOCAL-00001"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1687901189154</updated>
+    </task>
+    <option name="localTasksCounter" value="2"/>
     <servers/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
       <map>
         <entry key="MAIN">
           <value>
             <State/>
           </value>
         </entry>
       </map>
     </option>
   </component>
+  <component name="VcsManagerConfiguration">
+    <MESSAGE value="renamed package"/>
+    <option name="LAST_COMMIT_MESSAGE" value="renamed package"/>
+  </component>
 </project>
```

### Comparing `json_to_csv_filter-1.1/src/json_to_csv_filter/json_to_csv.py` & `json_to_csv_filter-1.3/src/json_to_csv_filter/json_to_csv.py`

 * *Files identical despite different names*

### Comparing `json_to_csv_filter-1.1/.gitignore` & `json_to_csv_filter-1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `json_to_csv_filter-1.1/LICENSE` & `json_to_csv_filter-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `json_to_csv_filter-1.1/pyproject.toml` & `json_to_csv_filter-1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "json_to_csv_filter"
-version = "1.1"
+dynamic = ["version"]
 requires-python = ">=3.7"
 description = "Convert list of json objects to csv with optional filters"
 authors = [
     { name="Hylke Foeken", email="h.foeken@gmail.com" },
 ]
 readme = "README.md"
 classifiers = [
@@ -18,8 +18,11 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/hylkefoeken/json-to-csv"
 "Bug Tracker" = "https://github.com/hylkefoeken/json-to-csv/issues"
 
 [project.scripts]
-json2csv = "json_to_csv.json_to_csv:main"
+json2csv = "json_to_csv_filter.json_to_csv:main"
+
+[tool.hatch.version]
+path = "src/json_to_csv_filter/__init__.py"
```

