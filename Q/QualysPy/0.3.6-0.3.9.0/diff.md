# Comparing `tmp/qualyspy-0.3.6.tar.gz` & `tmp/qualyspy-0.3.9.0.tar.gz`

## Comparing `qualyspy-0.3.6.tar` & `qualyspy-0.3.9.0.tar`

### file list

```diff
@@ -1,44 +1,65 @@
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 qualyspy-0.3.6/.vscode/launch.json
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 qualyspy-0.3.6/.vscode/settings.json
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 qualyspy-0.3.6/.vscode/tasks.json
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 qualyspy-0.3.6/debug/build.sh
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.3.6/debug/dtd.txt
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.3.6/debug/output.txt
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.3.6/debug/parse_dtd.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.3.6/debug/quickscan.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.3.6/debug/remove_cookies.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 qualyspy-0.3.6/debug/test.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/make.bat
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/source/conf.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/source/index.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/source/modules.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/source/qualyspy.assets.host_list.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/source/qualyspy.assets.host_list_detection.rst
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/source/qualyspy.qualysapi.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/source/qualyspy.qutils.rst
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/source/qualyspy.rst
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/source/qualyspy.scan_configuration.knowledgebase.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/__init__.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/exceptions.py
--rw-r--r--   0        0        0    16827 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/qualysapi.py
--rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/qutils.py
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/urls.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/asset_mgmt_tagging/__init__.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/asset_mgmt_tagging/api_input.py
--rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/asset_mgmt_tagging/asset.py
--rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/asset_mgmt_tagging/tag.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/assets/__init__.py
--rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/assets/host_list.py
--rw-r--r--   0        0        0    40811 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/assets/host_list_detection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/certview/__init__.py
--rw-r--r--   0        0        0    14938 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/certview/certificate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/scan_configuration/__init__.py
--rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/scan_configuration/knowledgebase.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.3.6/requirements/deploy.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qualyspy-0.3.6/requirements/dev.txt
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 qualyspy-0.3.6/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.3.6/LICENSE
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 qualyspy-0.3.6/README.md
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 qualyspy-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 qualyspy-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/config-example.ini
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/.vscode/launch.json
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/.vscode/settings.json
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/.vscode/tasks.json
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/debug/build.sh
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/debug/dtd.txt
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/debug/output.txt
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/debug/parse_dtd.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/debug/quickscan.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/debug/remove_cookies.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/debug/test.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/docs/Makefile
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/docs/conf.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/docs/make.bat
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/docs/modules.rst
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/docs/qualyspy.models.rst
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/docs/qualyspy.models.vmdr.rst
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/docs/qualyspy.rst
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy/URLS.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy/__init__.py
+-rw-r--r--   0        0        0    14970 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy/base.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy/exceptions.py
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy/gav.py
+-rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy/qutils.py
+-rw-r--r--   0        0        0     9613 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy/vmdr.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy/models/__init__.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy/models/sa_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy/models/gav/__init__.py
+-rw-r--r--   0        0        0    22850 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy/models/gav/asset_details_orm.py
+-rw-r--r--   0        0        0     7776 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy/models/gav/asset_details_output.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy/models/vmdr/__init__.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy/models/vmdr/converters.py
+-rw-r--r--   0        0        0    12712 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy/models/vmdr/host_list_orm.py
+-rw-r--r--   0        0        0    20174 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy/models/vmdr/host_list_output.py
+-rw-r--r--   0        0        0     9915 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy/models/vmdr/host_list_vm_detection_orm.py
+-rw-r--r--   0        0        0    20975 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy/models/vmdr/host_list_vm_detection_output.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy-legacy/__init__.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy-legacy/exceptions.py
+-rw-r--r--   0        0        0    15305 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy-legacy/qualysapi.py
+-rw-r--r--   0        0        0    16537 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy-legacy/qutils.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy-legacy/urls.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy-legacy/asset_mgmt_tagging/__init__.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy-legacy/asset_mgmt_tagging/api_input.py
+-rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy-legacy/asset_mgmt_tagging/asset.py
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy-legacy/asset_mgmt_tagging/tag.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy-legacy/assets/__init__.py
+-rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy-legacy/assets/host_list.py
+-rw-r--r--   0        0        0    40850 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy-legacy/assets/host_list_detection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy-legacy/certview/__init__.py
+-rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy-legacy/certview/certificate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy-legacy/scan_configuration/__init__.py
+-rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/qualyspy-legacy/scan_configuration/knowledgebase.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/requirements/deploy.txt
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/requirements/dev.txt
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/requirements/docs.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/tests/gav_test.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/tests/vmdr_test.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/LICENSE
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/README.md
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 qualyspy-0.3.9.0/PKG-INFO
```

### Comparing `qualyspy-0.3.6/debug/dtd.txt` & `qualyspy-0.3.9.0/debug/dtd.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.6/debug/output.txt` & `qualyspy-0.3.9.0/debug/output.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.6/debug/parse_dtd.py` & `qualyspy-0.3.9.0/debug/parse_dtd.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.6/debug/quickscan.py` & `qualyspy-0.3.9.0/debug/quickscan.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.6/debug/remove_cookies.py` & `qualyspy-0.3.9.0/debug/remove_cookies.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.6/docs/Makefile` & `qualyspy-0.3.9.0/docs/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Minimal makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line, and also
 # from the environment for the first two.
 SPHINXOPTS    ?=
 SPHINXBUILD   ?= sphinx-build
-SOURCEDIR     = source
-BUILDDIR      = build
+SOURCEDIR     = .
+BUILDDIR      = _build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
```

### Comparing `qualyspy-0.3.6/docs/make.bat` & `qualyspy-0.3.9.0/docs/make.bat`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 pushd %~dp0
 
 REM Command file for Sphinx documentation
 
 if "%SPHINXBUILD%" == "" (
 	set SPHINXBUILD=sphinx-build
 )
-set SOURCEDIR=source
-set BUILDDIR=build
+set SOURCEDIR=.
+set BUILDDIR=_build
 
 %SPHINXBUILD% >NUL 2>NUL
 if errorlevel 9009 (
 	echo.
 	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
 	echo.installed, then set the SPHINXBUILD environment variable to point
 	echo.to the full path of the 'sphinx-build' executable. Alternatively you
```

### Comparing `qualyspy-0.3.6/docs/source/conf.py` & `qualyspy-0.3.9.0/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import os
-import sys
-sys.path.insert(0, os.path.abspath('../../'))
-
 # Configuration file for the Sphinx documentation builder.
 #
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
+import os
+import sys
+sys.path.insert(0, os.path.abspath('..'))
+
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'QualysPy'
-copyright = '2022, Jordan Barnartt'
+copyright = '2023, Jordan Barnartt'
 author = 'Jordan Barnartt'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.coverage', 'sphinx.ext.napoleon']
+extensions = ['sphinx.ext.napoleon']
 
 templates_path = ['_templates']
-exclude_patterns = []
+exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = 'sphinx_rtd_theme'
-#html_static_path = ['_static']
+html_static_path = ['_static']
```

### Comparing `qualyspy-0.3.6/qualyspy/qualysapi.py` & `qualyspy-0.3.9.0/qualyspy-legacy/qualysapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,39 +28,14 @@
 }
 JSON_IN_XML_OUT_HEADERS = {
     "Accept": "application/json",
     "Content-Type": "application/xml",
 }
 
 
-class CustomHttpAdapter(requests.adapters.HTTPAdapter):
-    """Transport adapter" that allows us to use custom ssl_context.
-
-    Workaround because Qualys API Gateway URL does not support Secure Renegotation, which is
-    enforced in OpenSSL 3.X.  Reference:
-    https://stackoverflow.com/questions/71603314/ssl-error-unsafe-legacy-renegotiation-disabled
-    """
-
-    def __init__(
-        self, ssl_context: Optional[ssl.SSLContext] = None, **kwargs: Any
-    ) -> None:
-        self.ssl_context = ssl_context
-        super().__init__(**kwargs)
-
-    def init_poolmanager(
-        self, connections: Any, maxsize: Any, block: bool = False, **kwargs: Any
-    ) -> None:
-        self.poolmanager = urllib3.poolmanager.PoolManager(
-            num_pools=connections,
-            maxsize=maxsize,
-            block=block,
-            ssl_context=self.ssl_context,
-        )
-
-
 API_ROOT = qutils.config["AUTHENTICATION"]["api_root"]
 API_GATEWAY_ROOT = qutils.config["AUTHENTICATION"]["api_gateway_root"]
 CREDENTIALS = {
     "username": qutils.config["AUTHENTICATION"]["username"],
     "password": qutils.config["AUTHENTICATION"]["password"],
 }
 
@@ -98,16 +73,20 @@
             "password": CREDENTIALS["password"],
         }
         conn = requests.post(
             API_ROOT + qutils.URLS["Session Login"], headers=self._headers, data=data
         )
         if conn.status_code == requests.codes.ok:
             self._cookies["QualysSession"] = conn.cookies["QualysSession"]
-            with open("debug/cookies.txt", "a") as f:
-                f.write(str(conn.cookies["QualysSession"]) + "\n")
+            try:
+                # Write the cookie to a file in order to quickly clear them when debugging.
+                with open("debug/cookies.txt", "a") as f:
+                    f.write(str(conn.cookies["QualysSession"]) + "\n")
+            except FileNotFoundError:
+                pass
         else:
             print(conn.headers)
             conn.raise_for_status()
 
     def _connect_CertView(self) -> None:
         """Connects to the CertView API.  Adds a bearer token attribute to the class to be
         automatically used with any CertView API calls.
@@ -116,24 +95,19 @@
         data = {
             "username": CREDENTIALS["username"],
             "password": CREDENTIALS["password"],
             "token": "true",
             "permissions": "true",
         }
         headers = {"ContentType": "application/x-www-form-urlencoded"}
-
-        with requests.Session() as s:
-            ctx = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)
-            ctx.options |= 0x4
-            s.mount("https://", CustomHttpAdapter(ctx))
-            conn = s.post(
-                API_GATEWAY_ROOT + qutils.URLS["CertView Authentication"],
-                headers=headers,
-                data=data,
-            )
+        conn = requests.post(
+            API_GATEWAY_ROOT + qutils.URLS["CertView Authentication"],
+            headers=headers,
+            data=data,
+        )
         self._bearer_token = conn.text
 
     def register_in_out_headers(
         self, api_match: str, in_header: str, out_header: str
     ) -> None:
         """Registers the 'Accept' and 'Content-Type' headers for a given API path.
 
@@ -228,34 +202,21 @@
                     root + path,
                     headers=headers,
                     cookies=self._cookies,
                     params=params,
                     auth=auth,
                 )
             case "post":
-                if "/certview/" in path:
-                    with requests.Session() as s:
-                        ctx = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)
-                        ctx.options |= 0x4
-                        s.mount("https://", CustomHttpAdapter(ctx))
-                        response = s.post(
-                            root + path,
-                            headers=headers,
-                            cookies=self._cookies,
-                            data=data,
-                            auth=auth,
-                        )
-                else:
-                    response = requests.post(
-                        root + path,
-                        headers=headers,
-                        cookies=self._cookies,
-                        data=data,
-                        auth=auth,
-                    )
+                response = requests.post(
+                    root + path,
+                    headers=headers,
+                    cookies=self._cookies,
+                    data=data,
+                    auth=auth,
+                )
             case _:
                 raise ValueError(f"{method} is not a supported")
 
         if response.status_code != requests.codes.ok:
             status_code = response.status_code
             reason = response.reason
             url = response.url
```

### Comparing `qualyspy-0.3.6/qualyspy/qutils.py` & `qualyspy-0.3.9.0/qualyspy-legacy/qutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
     if not isinstance(input, MutableSequence):
         return str(input)
 
     output = ""
     for item in input:
         output += str(item) + ","
 
-    output.rstrip(",")  # Remove final comma
+    output = output.rstrip(",")  # Remove final comma
     return output
 
 
 def datetime_to_qualys_format(dt: Optional[datetime.datetime]) -> Optional[str]:
     """Converts a Python datetime object to the string format used by the Qualys API."""
 
     if dt is None:
```

### Comparing `qualyspy-0.3.6/qualyspy/urls.json` & `qualyspy-0.3.9.0/qualyspy-legacy/urls.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.6/qualyspy/asset_mgmt_tagging/api_input.py` & `qualyspy-0.3.9.0/qualyspy-legacy/asset_mgmt_tagging/api_input.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.6/qualyspy/asset_mgmt_tagging/asset.py` & `qualyspy-0.3.9.0/qualyspy-legacy/asset_mgmt_tagging/asset.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.6/qualyspy/asset_mgmt_tagging/tag.py` & `qualyspy-0.3.9.0/qualyspy-legacy/asset_mgmt_tagging/tag.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.6/qualyspy/assets/host_list.py` & `qualyspy-0.3.9.0/qualyspy-legacy/assets/host_list.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.6/qualyspy/assets/host_list_detection.py` & `qualyspy-0.3.9.0/qualyspy-legacy/assets/host_list_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import datetime
 import ipaddress
 from collections.abc import MutableSequence
 from typing import Optional, TextIO, Union
 
 import qualyspy.qualysapi as qualysapi
 import qualyspy.qutils as qutils
+from qualyspy.exceptions import Qualys_API_Error
 
 
 @dataclasses.dataclass
 class Warning:
     """A warning which appears when the API request reaches the truncation limit."""
 
     text: str
@@ -800,15 +801,15 @@
 
     if output_format == "python":
         if post:
             raw = conn.post(qutils.URLS["Host List Detection"], data=params_filtered)
         else:
             raw = conn.get(qutils.URLS["Host List Detection"], params=params_filtered)
         if raw.tag == "SIMPLE_RETURN":
-            raise qualysapi.Qualys_API_Error(
+            raise Qualys_API_Error(
                 f"Error {str(raw.RESPONSE.CODE)}: {str(raw.RESPONSE.TEXT)}"
             )
         host_list: list[Host] = []
         try:
             for host in raw.RESPONSE.HOST_LIST.HOST:
                 h = qutils.elements_to_class(
                     host,
```

### Comparing `qualyspy-0.3.6/qualyspy/certview/certificate.py` & `qualyspy-0.3.9.0/qualyspy-legacy/certview/certificate.py`

 * *Files 6% similar despite different names*

```diff
@@ -423,14 +423,24 @@
 
         raw = self.conn.post(qutils.URLS["List CertView Certificates"], input_data)
 
         if len(raw) > 0:
             certificates: list[Certificate] = []
             for cert in raw:
                 c = Certificate.parse_obj(cert)
+
+                # subject.name somtimes includes null characters "\x00", even though the GUI doesn't
+                # show these.  I've opened a ticket with Qualys about it.  In the meanwhile, this
+                # will replace them with something PostgreSQL is happy with.
+                # Also other fields, apparently...
+                #
+                c.subject.name = c.subject.name.replace("\x00", "\uFFFD")
+                c.subject.locality = c.subject.locality.replace("\x00", "\uFFFD")
+                c.subject.state = c.subject.state.replace("\x00", "\uFFFD")
+
                 certificates.append(c)
             return certificates
         else:
             return None
 
     def __call__(
         self,
```

### Comparing `qualyspy-0.3.6/qualyspy/scan_configuration/knowledgebase.py` & `qualyspy-0.3.9.0/qualyspy-legacy/scan_configuration/knowledgebase.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.6/.gitignore` & `qualyspy-0.3.9.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Debugging
 debug/cookies.txt
 debug/qualysapi.conf
 debug/db/*
+tests/test_data.py
 
 # qualysapi config file
 qualysapi.conf
 
 # Visual Studio Code
 #.vscode/
```

### Comparing `qualyspy-0.3.6/LICENSE` & `qualyspy-0.3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.6/pyproject.toml` & `qualyspy-0.3.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "QualysPy"
-version = "0.3.6"
+version = "0.3.9.0"
 authors = [
   { name="Jordan Barnartt", email="jbarnart@uwaterloo.ca" },
 ]
 description = "A Python wrapper for the Qualys API."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -23,15 +23,16 @@
 ]
 dependencies = [
   "lxml",
   "requests",
   "python-dateutil",
   "pydantic",
   "SQLAlchemy",
-  "psycopg2"
+  "psycopg2",
+  "xsdata",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/JordanBarnartt/qualyspy"
 "Bug Tracker" = "https://github.com/JordanBarnartt/qualyspy/issues"
 
 [tool.pyright]
```

