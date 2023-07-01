# Comparing `tmp/sphinx_c_autodoc-1.2.1.tar.gz` & `tmp/sphinx_c_autodoc-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_c_autodoc-1.2.1.tar", max compression
+gzip compressed data, was "sphinx_c_autodoc-1.2.2.tar", max compression
```

## Comparing `sphinx_c_autodoc-1.2.1.tar` & `sphinx_c_autodoc-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1071 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/LICENSE-MIT
--rw-r--r--   0        0        0     2669 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/README.rst
--rw-r--r--   0        0        0     1187 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/pyproject.toml
--rw-r--r--   0        0        0    26897 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/__init__.py
--rw-r--r--   0        0        0     7095 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/apidoc/__init__.py
--rw-r--r--   0        0        0       72 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/apidoc/templates/header.rst.jinja2
--rw-r--r--   0        0        0       57 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/apidoc/templates/source.rst.jinja2
--rw-r--r--   0        0        0      131 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/apidoc/templates/toc.rst.jinja2
--rw-r--r--   0        0        0        0 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/clang/__init__.py
--rw-r--r--   0        0        0      514 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/clang/comments.py
--rw-r--r--   0        0        0     5875 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/clang/patches.py
--rw-r--r--   0        0        0        0 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/domains/__init__.py
--rw-r--r--   0        0        0     1393 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/domains/c.py
--rw-r--r--   0        0        0    35949 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/loader.py
--rw-r--r--   0        0        0     6275 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/napoleon/__init__.py
--rw-r--r--   0        0        0    15732 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/viewcode/__init__.py
--rw-r--r--   0        0        0     3869 1970-01-01 00:00:00.000000 sphinx_c_autodoc-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-03-04 02:31:47.051291 sphinx_c_autodoc-1.2.2/LICENSE-MIT
+-rw-r--r--   0        0        0     2669 2023-06-12 01:58:47.515854 sphinx_c_autodoc-1.2.2/README.rst
+-rw-r--r--   0        0        0     1187 2023-06-29 01:30:43.148011 sphinx_c_autodoc-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0    26897 2023-04-07 20:52:17.681827 sphinx_c_autodoc-1.2.2/src/sphinx_c_autodoc/__init__.py
+-rw-r--r--   0        0        0     7095 2023-03-04 02:31:47.054586 sphinx_c_autodoc-1.2.2/src/sphinx_c_autodoc/apidoc/__init__.py
+-rw-r--r--   0        0        0       72 2023-03-04 02:31:47.054718 sphinx_c_autodoc-1.2.2/src/sphinx_c_autodoc/apidoc/templates/header.rst.jinja2
+-rw-r--r--   0        0        0       57 2023-03-04 02:31:47.054799 sphinx_c_autodoc-1.2.2/src/sphinx_c_autodoc/apidoc/templates/source.rst.jinja2
+-rw-r--r--   0        0        0      131 2023-03-04 02:31:47.054894 sphinx_c_autodoc-1.2.2/src/sphinx_c_autodoc/apidoc/templates/toc.rst.jinja2
+-rw-r--r--   0        0        0        0 2023-03-04 02:31:47.054966 sphinx_c_autodoc-1.2.2/src/sphinx_c_autodoc/clang/__init__.py
+-rw-r--r--   0        0        0      514 2023-03-04 02:31:47.055087 sphinx_c_autodoc-1.2.2/src/sphinx_c_autodoc/clang/comments.py
+-rw-r--r--   0        0        0     5875 2023-03-04 02:31:47.055199 sphinx_c_autodoc-1.2.2/src/sphinx_c_autodoc/clang/patches.py
+-rw-r--r--   0        0        0        0 2023-03-04 02:31:47.055275 sphinx_c_autodoc-1.2.2/src/sphinx_c_autodoc/domains/__init__.py
+-rw-r--r--   0        0        0     1393 2023-03-04 02:31:47.055370 sphinx_c_autodoc-1.2.2/src/sphinx_c_autodoc/domains/c.py
+-rw-r--r--   0        0        0    36147 2023-06-29 01:13:22.420822 sphinx_c_autodoc-1.2.2/src/sphinx_c_autodoc/loader.py
+-rw-r--r--   0        0        0     6275 2023-03-04 02:31:47.055801 sphinx_c_autodoc-1.2.2/src/sphinx_c_autodoc/napoleon/__init__.py
+-rw-r--r--   0        0        0    15732 2023-03-04 02:31:47.055986 sphinx_c_autodoc-1.2.2/src/sphinx_c_autodoc/viewcode/__init__.py
+-rw-r--r--   0        0        0     3869 1970-01-01 00:00:00.000000 sphinx_c_autodoc-1.2.2/PKG-INFO
```

### Comparing `sphinx_c_autodoc-1.2.1/LICENSE-MIT` & `sphinx_c_autodoc-1.2.2/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `sphinx_c_autodoc-1.2.1/README.rst` & `sphinx_c_autodoc-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_c_autodoc-1.2.1/pyproject.toml` & `sphinx_c_autodoc-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinx-c-autodoc"
-version = "1.2.1"
+version = "1.2.2"
 description = "A sphinx autodoc extension for c modules"
 authors = ["Nick <speedyleion@users.noreply.github.com>"]
 license = "MIT License, The Unlicense (Unlicense)"
 readme = "README.rst"
 packages = [{include = "sphinx_c_autodoc", from = "src"}]
 repository = "https://github.com/speedyleion/sphinx-c-autodoc"
 documentation = "https://sphinx-c-autodoc.readthedocs.io/en/latest/"
@@ -25,16 +25,16 @@
 [tool.poetry.scripts]
 sphinx-c-apidoc = 'sphinx_c_autodoc.apidoc:main'
 
 [tool.poetry.group.dev.dependencies]
 pylint = "2.13.9"
 black = "23.3.0"
 pycodestyle = "2.10.0"
-mypy =  "1.3.0"
-pytest = "7.3.2"
+mypy =  "1.4.1"
+pytest = "7.4.0"
 pytest-cov = "4.1.0"
 sphinx_rtd_theme = "1.2.2"
 sphinxcontrib-autoprogram = "0.1.8"
 types-docutils = "0.20.0.1"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/__init__.py` & `sphinx_c_autodoc-1.2.2/src/sphinx_c_autodoc/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/apidoc/__init__.py` & `sphinx_c_autodoc-1.2.2/src/sphinx_c_autodoc/apidoc/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/clang/comments.py` & `sphinx_c_autodoc-1.2.2/src/sphinx_c_autodoc/clang/comments.py`

 * *Files identical despite different names*

### Comparing `sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/clang/patches.py` & `sphinx_c_autodoc-1.2.2/src/sphinx_c_autodoc/clang/patches.py`

 * *Files identical despite different names*

### Comparing `sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/domains/c.py` & `sphinx_c_autodoc-1.2.2/src/sphinx_c_autodoc/domains/c.py`

 * *Files identical despite different names*

### Comparing `sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/loader.py` & `sphinx_c_autodoc-1.2.2/src/sphinx_c_autodoc/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,21 +344,29 @@
         tokens = [
             i.spelling for i in ident_iter if i.kind == cindex.TokenKind.IDENTIFIER
         ]
 
         return f"{self.name}({', '.join(tokens)})"
 
 
-class DocumentedEnumerator(DocumentedMacro):
+class DocumentedEnumerator(DocumentedObject):
     """
     An enumerator, the constant values in an enum
     """
 
     type_ = "enumerator"
 
+    def format_name(self) -> str:
+        """
+        The name of the object.
+
+        For things like functions and others this will include the return type.
+        """
+        return self.name
+
 
 class DocumentedMember(DocumentedObject):
     """
     A documented member of a struct or union.
     """
 
     type_ = "member"
```

### Comparing `sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/napoleon/__init__.py` & `sphinx_c_autodoc-1.2.2/src/sphinx_c_autodoc/napoleon/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/viewcode/__init__.py` & `sphinx_c_autodoc-1.2.2/src/sphinx_c_autodoc/viewcode/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_c_autodoc-1.2.1/PKG-INFO` & `sphinx_c_autodoc-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-c-autodoc
-Version: 1.2.1
+Version: 1.2.2
 Summary: A sphinx autodoc extension for c modules
 Home-page: https://github.com/speedyleion/sphinx-c-autodoc
 License: MIT License, The Unlicense (Unlicense)
 Author: Nick
 Author-email: speedyleion@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

