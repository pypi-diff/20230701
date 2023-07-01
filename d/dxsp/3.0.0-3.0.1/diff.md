# Comparing `tmp/dxsp-3.0.0.tar.gz` & `tmp/dxsp-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-3.0.0.tar", max compression
+gzip compressed data, was "dxsp-3.0.1.tar", max compression
```

## Comparing `dxsp-3.0.0.tar` & `dxsp-3.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-07-01 17:42:01.895242 dxsp-3.0.0/LICENSE
--rw-r--r--   0        0        0     2339 2023-07-01 17:42:01.895242 dxsp-3.0.0/README.md
--rw-r--r--   0        0        0      114 2023-07-01 17:42:02.795255 dxsp-3.0.0/dxsp/__init__.py
--rw-r--r--   0        0        0      418 2023-07-01 17:42:01.895242 dxsp-3.0.0/dxsp/config.py
--rw-r--r--   0        0        0     8027 2023-07-01 17:42:01.895242 dxsp-3.0.0/dxsp/default_settings.toml
--rw-r--r--   0        0        0    14882 2023-07-01 17:42:01.895242 dxsp-3.0.0/dxsp/main.py
--rw-r--r--   0        0        0      103 2023-07-01 17:42:01.895242 dxsp-3.0.0/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3598 2023-07-01 17:42:01.895242 dxsp-3.0.0/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     2189 2023-07-01 17:42:01.895242 dxsp-3.0.0/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0      941 2023-07-01 17:42:01.895242 dxsp-3.0.0/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0     2118 2023-07-01 17:42:02.795255 dxsp-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     3141 1970-01-01 00:00:00.000000 dxsp-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-01 18:09:46.447126 dxsp-3.0.1/LICENSE
+-rw-r--r--   0        0        0     2249 2023-07-01 18:09:46.447126 dxsp-3.0.1/README.md
+-rw-r--r--   0        0        0      114 2023-07-01 18:09:47.347126 dxsp-3.0.1/dxsp/__init__.py
+-rw-r--r--   0        0        0      418 2023-07-01 18:09:46.447126 dxsp-3.0.1/dxsp/config.py
+-rw-r--r--   0        0        0     8027 2023-07-01 18:09:46.447126 dxsp-3.0.1/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    14882 2023-07-01 18:09:46.447126 dxsp-3.0.1/dxsp/main.py
+-rw-r--r--   0        0        0      103 2023-07-01 18:09:46.447126 dxsp-3.0.1/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3598 2023-07-01 18:09:46.447126 dxsp-3.0.1/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     2189 2023-07-01 18:09:46.447126 dxsp-3.0.1/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0      941 2023-07-01 18:09:46.447126 dxsp-3.0.1/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0     2118 2023-07-01 18:09:47.343126 dxsp-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3051 1970-01-01 00:00:00.000000 dxsp-3.0.1/PKG-INFO
```

### Comparing `dxsp-3.0.0/LICENSE` & `dxsp-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-3.0.0/README.md` & `dxsp-3.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -36,13 +36,13 @@
 ### Example
 
 [example](https://github.com/mraniki/dxsp/blob/main/examples/example.py)
 
 
 ### Real use case
 
-[TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
+[TalkyTrader](https://github.com/mraniki/tt)
 
 ## Documentation
 
 [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/)
```

### Comparing `dxsp-3.0.0/dxsp/default_settings.toml` & `dxsp-3.0.1/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-3.0.0/dxsp/main.py` & `dxsp-3.0.1/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.0.0/dxsp/protocols/oneinch.py` & `dxsp-3.0.1/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.0.0/dxsp/protocols/uniswap.py` & `dxsp-3.0.1/dxsp/protocols/uniswap.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.0.0/dxsp/protocols/zerox.py` & `dxsp-3.0.1/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.0.0/pyproject.toml` & `dxsp-3.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "3.0.0"
+version = "3.0.1"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
```

### Comparing `dxsp-3.0.0/PKG-INFO` & `dxsp-3.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 3.0.0
+Version: 3.0.1
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -56,14 +56,14 @@
 ### Example
 
 [example](https://github.com/mraniki/dxsp/blob/main/examples/example.py)
 
 
 ### Real use case
 
-[TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
+[TalkyTrader](https://github.com/mraniki/tt)
 
 ## Documentation
 
 [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/)
```

