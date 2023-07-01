# Comparing `tmp/count_tokens-0.3.0.tar.gz` & `tmp/count_tokens-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "count_tokens-0.3.0.tar", max compression
+gzip compressed data, was "count_tokens-0.4.0.tar", max compression
```

## Comparing `count_tokens-0.3.0.tar` & `count_tokens-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1184 2023-06-28 10:33:37.741280 count_tokens-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-06-28 06:49:18.286368 count_tokens-0.3.0/count_tokens/__init__.py
--rwxr-xr-x   0        0        0     1829 2023-06-28 08:38:37.683411 count_tokens-0.3.0/count_tokens/count.py
--rw-r--r--   0        0        0     1214 2023-06-28 10:33:47.690258 count_tokens-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 count_tokens-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2015 2023-07-01 04:28:49.570016 count_tokens-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-28 06:49:18.286368 count_tokens-0.4.0/count_tokens/__init__.py
+-rwxr-xr-x   0        0        0     1829 2023-06-28 08:38:37.683411 count_tokens-0.4.0/count_tokens/count.py
+-rw-r--r--   0        0        0     1214 2023-07-01 04:28:59.682369 count_tokens-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3099 1970-01-01 00:00:00.000000 count_tokens-0.4.0/PKG-INFO
```

### Comparing `count_tokens-0.3.0/count_tokens/count.py` & `count_tokens-0.4.0/count_tokens/count.py`

 * *Files identical despite different names*

### Comparing `count_tokens-0.3.0/pyproject.toml` & `count_tokens-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "count-tokens"
-version = "0.3.0"
+version = "0.4.0"
 description = "Count number of tokens in the text file using toktoken tokenizer from OpenAI."
 authors = ["Krystian Safjan <ksafjan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "count_tokens"}]
 
 keywords = ["count", "tokens", "toktoken", "openai", "tokenizer"]
```

