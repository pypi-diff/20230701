# Comparing `tmp/spectree-1.1.3.tar.gz` & `tmp/spectree-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectree-1.1.3.tar", last modified: Tue May 30 09:31:32 2023, max compression
+gzip compressed data, was "spectree-1.1.4.tar", last modified: Sat Jul  1 07:34:41 2023, max compression
```

## Comparing `spectree-1.1.3.tar` & `spectree-1.1.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:31:32.521828 spectree-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-30 09:31:18.000000 spectree-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-30 09:31:18.000000 spectree-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18665 2023-05-30 09:31:32.521828 spectree-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17412 2023-05-30 09:31:18.000000 spectree-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-30 09:31:18.000000 spectree-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 09:31:32.521828 spectree-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-30 09:31:18.000000 spectree-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:31:32.517828 spectree-1.1.3/spectree/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:31:32.517828 spectree-1.1.3/spectree/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/plugins/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/plugins/falcon_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/plugins/flask_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/plugins/quart_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/plugins/starlette_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13804 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-05-30 09:31:18.000000 spectree-1.1.3/spectree/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:31:32.517828 spectree-1.1.3/spectree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18665 2023-05-30 09:31:32.000000 spectree-1.1.3/spectree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-30 09:31:32.000000 spectree-1.1.3/spectree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:31:32.000000 spectree-1.1.3/spectree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-30 09:31:32.000000 spectree-1.1.3/spectree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 09:31:32.000000 spectree-1.1.3/spectree.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:31:32.521828 spectree-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_plugin_falcon.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_plugin_falcon_asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_plugin_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_plugin_flask_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_plugin_flask_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_plugin_quart.py
--rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_plugin_starlette.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-05-30 09:31:18.000000 spectree-1.1.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:34:41.414464 spectree-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-07-01 07:34:30.000000 spectree-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-01 07:34:30.000000 spectree-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-07-01 07:34:41.414464 spectree-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17910 2023-07-01 07:34:30.000000 spectree-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-01 07:34:30.000000 spectree-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 07:34:41.414464 spectree-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-01 07:34:30.000000 spectree-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:34:41.414464 spectree-1.1.4/spectree/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:34:41.414464 spectree-1.1.4/spectree/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/plugins/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/plugins/falcon_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/plugins/flask_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/plugins/quart_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/plugins/starlette_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:34:41.414464 spectree-1.1.4/spectree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-07-01 07:34:41.000000 spectree-1.1.4/spectree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-01 07:34:41.000000 spectree-1.1.4/spectree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 07:34:41.000000 spectree-1.1.4/spectree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-01 07:34:41.000000 spectree-1.1.4/spectree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-01 07:34:41.000000 spectree-1.1.4/spectree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:34:41.414464 spectree-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_plugin_falcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_plugin_falcon_asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_plugin_flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_plugin_flask_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_plugin_flask_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_plugin_quart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_plugin_starlette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_utils.py
```

### Comparing `spectree-1.1.3/LICENSE` & `spectree-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spectree-1.1.3/PKG-INFO` & `spectree-1.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectree
-Version: 1.1.3
+Version: 1.1.4
 Summary: generate OpenAPI document and validate request&response with Python annotations.
 Author-email: Keming Yang <kemingy94@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/0b01001001/spectree
 Project-URL: documentation, https://0b01001001.github.io/spectree/
 Project-URL: repository, https://github.com/0b01001001/spectree
 Project-URL: changelog, https://github.com/0b01001001/spectree/releases
@@ -22,14 +22,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: email
 Provides-Extra: flask
 Provides-Extra: quart
 Provides-Extra: falcon
 Provides-Extra: starlette
 Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE
 
 # SpecTree
 
 
 [![GitHub Actions](https://github.com/0b01001001/spectree/workflows/Python%20package/badge.svg)](https://github.com/0b01001001/spectree/actions)
 [![pypi](https://img.shields.io/pypi/v/spectree.svg)](https://pypi.python.org/pypi/spectree)
@@ -62,22 +63,23 @@
 * [falcon example with logging when validation failed](/examples/falcon_demo.py)
 * [starlette example](examples/starlette_demo.py)
 
 ### Step by Step
 
 1. Define your data structure used in (query, json, headers, cookies, resp) with `pydantic.BaseModel`
 2. create `spectree.SpecTree` instance with the web framework name you are using, like `api = SpecTree('flask')`
-3. `api.validate` decorate the route with
+3. `api.validate` decorate the route with (the default value is given in parentheses):
    * `query`
    * `json`
    * `headers`
    * `cookies`
    * `resp`
-   * `tags`
-   * `security`
+   * `tags` *(no tags on endpoint)*
+   * `security` *(`None` - endpoint is not secured)*
+   * `deprecated` *(`False` - endpoint is not marked as deprecated)*
 4. access these data with `context(query, json, headers, cookies)` (of course, you can access these from the original place where the framework offered)
    * flask: `request.context`
    * falcon: `req.context`
    * starlette: `request.context`
 5. register to the web application `api.register(app)`
 6. check the document at URL location `/apidoc/redoc` or `/apidoc/swagger`
 
@@ -241,14 +243,28 @@
 def foobar():
     ...
 ```
 
 </p>
 </details>
 
+> How to mark deprecated endpoint?
+
+Use `deprecated` attribute with value `True` in `api.validate()` decorator. This way, an endpoint will be marked as
+ deprecated and will be marked with a strikethrough in API documentation.
+
+Code example:
+```
+@api.validate(
+    deprecated=True,
+)
+def deprecated_endpoint():
+    ...
+```
+
 > What should I return when I'm using the library?
 
 No need to change anything. Just return what the framework required.
 
 > How to log when the validation failed?
 
 Validation errors are logged with the INFO level. Details are passed into `extra`. Check the [falcon example](examples/falcon_demo.py) for details.
```

### Comparing `spectree-1.1.3/README.md` & `spectree-1.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -32,22 +32,23 @@
 * [falcon example with logging when validation failed](/examples/falcon_demo.py)
 * [starlette example](examples/starlette_demo.py)
 
 ### Step by Step
 
 1. Define your data structure used in (query, json, headers, cookies, resp) with `pydantic.BaseModel`
 2. create `spectree.SpecTree` instance with the web framework name you are using, like `api = SpecTree('flask')`
-3. `api.validate` decorate the route with
+3. `api.validate` decorate the route with (the default value is given in parentheses):
    * `query`
    * `json`
    * `headers`
    * `cookies`
    * `resp`
-   * `tags`
-   * `security`
+   * `tags` *(no tags on endpoint)*
+   * `security` *(`None` - endpoint is not secured)*
+   * `deprecated` *(`False` - endpoint is not marked as deprecated)*
 4. access these data with `context(query, json, headers, cookies)` (of course, you can access these from the original place where the framework offered)
    * flask: `request.context`
    * falcon: `req.context`
    * starlette: `request.context`
 5. register to the web application `api.register(app)`
 6. check the document at URL location `/apidoc/redoc` or `/apidoc/swagger`
 
@@ -211,14 +212,28 @@
 def foobar():
     ...
 ```
 
 </p>
 </details>
 
+> How to mark deprecated endpoint?
+
+Use `deprecated` attribute with value `True` in `api.validate()` decorator. This way, an endpoint will be marked as
+ deprecated and will be marked with a strikethrough in API documentation.
+
+Code example:
+```
+@api.validate(
+    deprecated=True,
+)
+def deprecated_endpoint():
+    ...
+```
+
 > What should I return when I'm using the library?
 
 No need to change anything. Just return what the framework required.
 
 > How to log when the validation failed?
 
 Validation errors are logged with the INFO level. Details are passed into `extra`. Check the [falcon example](examples/falcon_demo.py) for details.
```

### Comparing `spectree-1.1.3/pyproject.toml` & `spectree-1.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spectree"
-version = "1.1.3"
+version = "1.1.4"
 dynamic = []
 description = "generate OpenAPI document and validate request&response with Python annotations."
 readme = "README.md"
 license = {text = "Apache-2.0"}
 requires-python = ">=3.8"
 authors = [
     { name = "Keming Yang", email = "kemingy94@gmail.com" },
@@ -30,27 +30,32 @@
     "autoflake>=1.4,<3.0",
     "black>=22.3,<24.0",
     "flake8>=4,<7",
     "isort~=5.10",
     "mypy>=0.971",
     "pre-commit",
     "pytest~=7.1",
+    "syrupy>=4.0",
 ]
 email = [
-    "pydantic[email]>=1.2",
+    "pydantic[email]>=1.2,<2",
 ]
 falcon = [
     "falcon>=3.0.0",
 ]
 flask = [
     "flask",
 ]
 starlette = [
     "starlette[full]",
 ]
+docs = [
+    "Sphinx",
+    "furo",
+]
 
 [project.urls]
 Homepage = "https://github.com/0b01001001/spectree"
 documentation = "https://0b01001001.github.io/spectree/"
 repository = "https://github.com/0b01001001/spectree"
 changelog = "https://github.com/0b01001001/spectree/releases"
 
@@ -58,15 +63,15 @@
 profile = "black"
 
 [tool.mypy]
 plugins = ["pydantic.mypy"]
 follow_imports = "silent"
 ignore_missing_imports = true
 show_error_codes = true
-warn_unused_ignores = true
+warn_unused_ignores = false
 warn_redundant_casts = true
 no_implicit_reexport = true
 disable_error_code = ["attr-defined"]
 
 [tool.pydantic-mypy]
 init_typed = true
 init_forbid_extra = true
```

### Comparing `spectree-1.1.3/setup.py` & `spectree-1.1.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,23 +5,27 @@
 
 setup(
     name="spectree",
     install_requires=[
         "pydantic>=1.2",
     ],
     extras_require={
-        "email": ["pydantic[email]>=1.2"],
+        "email": ["pydantic[email]>=1.2,<2"],
         "flask": ["flask"],
         "quart": ["quart"],
         "falcon": ["falcon>=3.0.0"],
         "starlette": ["starlette[full]"],
         "dev": [
             "pytest~=7.1",
             "flake8>=4,<7",
             "black>=22.3,<24.0",
             "isort~=5.10",
             "autoflake>=1.4,<3.0",
             "mypy>=0.971",
             "syrupy>=4.0.0",
         ],
+        "docs": [
+            "Sphinx",
+            "furo",
+        ],
     },
 )
```

### Comparing `spectree-1.1.3/spectree/_types.py` & `spectree-1.1.4/spectree/_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 OptionalModelType = Optional[ModelType]
 NamingStrategy = Callable[[ModelType], str]
 NestedNamingStrategy = Callable[[str, str], str]
 
 
 class MultiDict(Protocol):
     def get(self, key: str) -> Optional[str]:
-        ...
+        pass
 
     def getlist(self, key: str) -> List[str]:
-        ...
+        pass
 
     def __iter__(self) -> Iterator[str]:
-        ...
+        pass
 
 
 class FunctionDecorator(Protocol):
     resp: Any
     tags: Sequence[Any]
     security: Union[None, Dict, List[Any]]
     deprecated: bool
```

### Comparing `spectree-1.1.3/spectree/config.py` & `spectree-1.1.4/spectree/config.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.3/spectree/models.py` & `spectree-1.1.4/spectree/models.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.3/spectree/page.py` & `spectree-1.1.4/spectree/page.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.3/spectree/plugins/__init__.py` & `spectree-1.1.4/spectree/plugins/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from collections import namedtuple
 
 from .base import BasePlugin
 
-__all__ = ["BasePlugin"]
-
 Plugin = namedtuple("Plugin", ("name", "package", "class_name"))
 
 PLUGINS = {
     "base": Plugin(".base", __name__, "BasePlugin"),
     "flask": Plugin(".flask_plugin", __name__, "FlaskPlugin"),
     "quart": Plugin(".quart_plugin", __name__, "QuartPlugin"),
     "falcon": Plugin(".falcon_plugin", __name__, "FalconPlugin"),
     "falcon-asgi": Plugin(".falcon_plugin", __name__, "FalconAsgiPlugin"),
     "starlette": Plugin(".starlette_plugin", __name__, "StarlettePlugin"),
 }
+
+__all__ = ["BasePlugin", "PLUGINS", "Plugin"]
```

### Comparing `spectree-1.1.3/spectree/plugins/base.py` & `spectree-1.1.4/spectree/plugins/base.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.3/spectree/plugins/falcon_plugin.py` & `spectree-1.1.4/spectree/plugins/falcon_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.3/spectree/plugins/flask_plugin.py` & `spectree-1.1.4/spectree/plugins/flask_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.3/spectree/plugins/quart_plugin.py` & `spectree-1.1.4/spectree/plugins/quart_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.3/spectree/plugins/starlette_plugin.py` & `spectree-1.1.4/spectree/plugins/starlette_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,16 +153,18 @@
                 if route.path.startswith(f"/{self.config.path}"):
                     continue
 
                 func = route.app
                 if isinstance(func, partial):
                     try:
                         func = func.__wrapped__
-                    except AttributeError:
-                        pass
+                    except AttributeError as err:
+                        self.logger.warning(
+                            "failed to get the wrapped func %s: %s", func, err
+                        )
 
                 if inspect.isclass(func):
                     for method in METHODS:
                         if getattr(func, method, None):
                             routes.append(
                                 Route(
                                     f"{prefix}{route.path}",
```

### Comparing `spectree-1.1.3/spectree/response.py` & `spectree-1.1.4/spectree/response.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.3/spectree/spec.py` & `spectree-1.1.4/spectree/spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         :param json: `pydantic.BaseModel`, JSON format request body
         :param form: `pydantic.BaseModel`, form-data request body
         :param headers: `pydantic.BaseModel`, if you have specific headers
         :param cookies: `pydantic.BaseModel`, if you have cookies for this route
         :param resp: `spectree.Response`
         :param tags: a tuple of strings or :class:`spectree.models.Tag`
         :param security: dict with security config for current route and method
-        :param deprecated: bool if endpoint is marked as deprecated
+        :param deprecated: bool, if endpoint is marked as deprecated
         :param before: :meth:`spectree.utils.default_before_handler` for
             specific endpoint
         :param after: :meth:`spectree.utils.default_after_handler` for
             specific endpoint
         :param validation_error_status: The response status code to use for the
             specific endpoint, in the event of a validation error. If not specified,
             the global `validation_error_status` is used instead, defined
```

### Comparing `spectree-1.1.3/spectree/utils.py` & `spectree-1.1.4/spectree/utils.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.3/spectree.egg-info/PKG-INFO` & `spectree-1.1.4/spectree.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectree
-Version: 1.1.3
+Version: 1.1.4
 Summary: generate OpenAPI document and validate request&response with Python annotations.
 Author-email: Keming Yang <kemingy94@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/0b01001001/spectree
 Project-URL: documentation, https://0b01001001.github.io/spectree/
 Project-URL: repository, https://github.com/0b01001001/spectree
 Project-URL: changelog, https://github.com/0b01001001/spectree/releases
@@ -22,14 +22,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: email
 Provides-Extra: flask
 Provides-Extra: quart
 Provides-Extra: falcon
 Provides-Extra: starlette
 Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE
 
 # SpecTree
 
 
 [![GitHub Actions](https://github.com/0b01001001/spectree/workflows/Python%20package/badge.svg)](https://github.com/0b01001001/spectree/actions)
 [![pypi](https://img.shields.io/pypi/v/spectree.svg)](https://pypi.python.org/pypi/spectree)
@@ -62,22 +63,23 @@
 * [falcon example with logging when validation failed](/examples/falcon_demo.py)
 * [starlette example](examples/starlette_demo.py)
 
 ### Step by Step
 
 1. Define your data structure used in (query, json, headers, cookies, resp) with `pydantic.BaseModel`
 2. create `spectree.SpecTree` instance with the web framework name you are using, like `api = SpecTree('flask')`
-3. `api.validate` decorate the route with
+3. `api.validate` decorate the route with (the default value is given in parentheses):
    * `query`
    * `json`
    * `headers`
    * `cookies`
    * `resp`
-   * `tags`
-   * `security`
+   * `tags` *(no tags on endpoint)*
+   * `security` *(`None` - endpoint is not secured)*
+   * `deprecated` *(`False` - endpoint is not marked as deprecated)*
 4. access these data with `context(query, json, headers, cookies)` (of course, you can access these from the original place where the framework offered)
    * flask: `request.context`
    * falcon: `req.context`
    * starlette: `request.context`
 5. register to the web application `api.register(app)`
 6. check the document at URL location `/apidoc/redoc` or `/apidoc/swagger`
 
@@ -241,14 +243,28 @@
 def foobar():
     ...
 ```
 
 </p>
 </details>
 
+> How to mark deprecated endpoint?
+
+Use `deprecated` attribute with value `True` in `api.validate()` decorator. This way, an endpoint will be marked as
+ deprecated and will be marked with a strikethrough in API documentation.
+
+Code example:
+```
+@api.validate(
+    deprecated=True,
+)
+def deprecated_endpoint():
+    ...
+```
+
 > What should I return when I'm using the library?
 
 No need to change anything. Just return what the framework required.
 
 > How to log when the validation failed?
 
 Validation errors are logged with the INFO level. Details are passed into `extra`. Check the [falcon example](examples/falcon_demo.py) for details.
```

### Comparing `spectree-1.1.3/spectree.egg-info/SOURCES.txt` & `spectree-1.1.4/spectree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spectree-1.1.3/tests/test_config.py` & `spectree-1.1.4/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     config = Configuration(
         license={"name": "MIT", "url": "https://opensource.org/licenses/MIT"}
     )
     assert config.license.name == "MIT"
     assert config.license.url == "https://opensource.org/licenses/MIT"
 
     with pytest.raises(ValidationError):
-        config = Configuration(license={"name": "MIT", "url": "url"})
+        Configuration(license={"name": "MIT", "url": "url"})
 
 
 def test_config_contact():
     config = Configuration(contact={"name": "John"})
     assert config.contact.name == "John"
 
     config = Configuration(contact={"name": "John", "url": "https://example.com"})
@@ -33,15 +33,15 @@
     assert config.contact.url == "https://example.com"
 
     config = Configuration(contact={"name": "John", "email": "hello@github.com"})
     assert config.contact.name == "John"
     assert config.contact.email == "hello@github.com"
 
     with pytest.raises(ValidationError):
-        config = Configuration(contact={"name": "John", "url": "url"})
+        Configuration(contact={"name": "John", "url": "url"})
 
 
 @pytest.mark.skipif(EmailFieldType == str, reason="email-validator is not installled")
 def test_config_contact_invalid_email():
     with pytest.raises(ValidationError):
         Configuration(contact={"name": "John", "email": "hello"})
```

### Comparing `spectree-1.1.3/tests/test_plugin.py` & `spectree-1.1.4/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.3/tests/test_plugin_falcon.py` & `spectree-1.1.4/tests/test_plugin_falcon.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.3/tests/test_plugin_falcon_asgi.py` & `spectree-1.1.4/tests/test_plugin_falcon_asgi.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.3/tests/test_plugin_flask.py` & `spectree-1.1.4/tests/test_plugin_flask.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.3/tests/test_plugin_flask_blueprint.py` & `spectree-1.1.4/tests/test_plugin_flask_blueprint.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.3/tests/test_plugin_flask_view.py` & `spectree-1.1.4/tests/test_plugin_flask_view.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.3/tests/test_plugin_quart.py` & `spectree-1.1.4/tests/test_plugin_quart.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,15 @@
 async def list_json():
     return {}
 
 
 # INFO: ensures that spec is calculated and cached _after_ registering
 # view functions for validations. This enables tests to access `api.spec`
 # without app_context.
+# TODO: this is commented out because it requires async context
 # with app.app_context():
 #     api.spec
 api.register(app)
 
 
 @pytest.fixture
 def client():
@@ -258,14 +259,15 @@
 async def oauth_two_ping():
     """
     oauth2 auth type with flow
     """
     return jsonify(msg="pong")
 
 
+# TODO: this is commented out because it requires async context
 # with app_secure.app_context():
 #     api_secure.spec
 
 api_secure.register(app_secure)
 
 
 """
@@ -328,11 +330,12 @@
 async def global_security_or():
     """
     global auth OR
     """
     return jsonify(msg="pong")
 
 
+# TODO: this is commented out because it requires async context
 # with app_global_secure.app_context():
 #     api_global_secure.spec
 
 api_global_secure.register(app_global_secure)
```

### Comparing `spectree-1.1.3/tests/test_plugin_starlette.py` & `spectree-1.1.4/tests/test_plugin_starlette.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.3/tests/test_response.py` & `spectree-1.1.4/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.3/tests/test_spec.py` & `spectree-1.1.4/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.3/tests/test_utils.py` & `spectree-1.1.4/tests/test_utils.py`

 * *Files identical despite different names*

