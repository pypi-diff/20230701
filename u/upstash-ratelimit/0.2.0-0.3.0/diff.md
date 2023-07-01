# Comparing `tmp/upstash_ratelimit-0.2.0.tar.gz` & `tmp/upstash_ratelimit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_ratelimit-0.2.0.tar", max compression
+gzip compressed data, was "upstash_ratelimit-0.3.0.tar", max compression
```

## Comparing `upstash_ratelimit-0.2.0.tar` & `upstash_ratelimit-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,24 @@
--rw-r--r--   0        0        0     1072 2023-05-24 13:49:29.501847 upstash_ratelimit-0.2.0/LICENSE
--rw-r--r--   0        0        0    11067 2023-06-21 06:26:04.086481 upstash_ratelimit-0.2.0/README.md
--rw-r--r--   0        0        0      398 2023-06-30 21:29:45.489466 upstash_ratelimit-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 13:49:29.503800 upstash_ratelimit-0.2.0/upstash_ratelimit/__init__.py
--rw-r--r--   0        0        0    18972 2023-06-21 06:26:04.089379 upstash_ratelimit-0.2.0/upstash_ratelimit/algorithm.py
--rw-r--r--   0        0        0      167 2023-05-24 13:49:29.504075 upstash_ratelimit-0.2.0/upstash_ratelimit/config.py
--rw-r--r--   0        0        0     2997 2023-06-21 04:18:16.326585 upstash_ratelimit-0.2.0/upstash_ratelimit/limiter.py
--rw-r--r--   0        0        0        0 2023-05-24 13:49:29.504232 upstash_ratelimit-0.2.0/upstash_ratelimit/py.typed
--rw-r--r--   0        0        0      475 2023-06-21 04:18:16.326882 upstash_ratelimit-0.2.0/upstash_ratelimit/schema/response.py
--rw-r--r--   0        0        0      392 2023-06-21 04:18:16.327167 upstash_ratelimit-0.2.0/upstash_ratelimit/utils/time.py
--rw-r--r--   0        0        0    11656 1970-01-01 00:00:00.000000 upstash_ratelimit-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-24 13:49:29.501847 upstash_ratelimit-0.3.0/LICENSE
+-rw-r--r--   0        0        0    11067 2023-06-21 06:26:04.086481 upstash_ratelimit-0.3.0/README.md
+-rw-r--r--   0        0        0      398 2023-07-01 01:38:59.014707 upstash_ratelimit-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-06-30 22:13:44.524574 upstash_ratelimit-0.3.0/upstash_ratelimit/__init__.py
+-rw-r--r--   0        0        0     1828 2023-07-01 00:54:30.139483 upstash_ratelimit-0.3.0/upstash_ratelimit/algorithms/algorithm.py
+-rw-r--r--   0        0        0     3243 2023-07-01 00:40:41.395386 upstash_ratelimit-0.3.0/upstash_ratelimit/algorithms/fixed_window_core.py
+-rw-r--r--   0        0        0     5777 2023-07-01 00:17:49.801642 upstash_ratelimit-0.3.0/upstash_ratelimit/algorithms/sliding_window_core.py
+-rw-r--r--   0        0        0     5231 2023-07-01 00:17:45.426985 upstash_ratelimit-0.3.0/upstash_ratelimit/algorithms/token_bucket_core.py
+-rw-r--r--   0        0        0       86 2023-07-01 00:19:13.681310 upstash_ratelimit-0.3.0/upstash_ratelimit/asyncio/__init__.py
+-rw-r--r--   0        0        0     1161 2023-07-01 01:02:11.086857 upstash_ratelimit-0.3.0/upstash_ratelimit/asyncio/async_blocker.py
+-rw-r--r--   0        0        0     2981 2023-07-01 01:17:19.839016 upstash_ratelimit-0.3.0/upstash_ratelimit/asyncio/fixed_window.py
+-rw-r--r--   0        0        0     3506 2023-07-01 01:06:06.660882 upstash_ratelimit-0.3.0/upstash_ratelimit/asyncio/limiter.py
+-rw-r--r--   0        0        0     3788 2023-07-01 01:03:13.817815 upstash_ratelimit-0.3.0/upstash_ratelimit/asyncio/sliding_window.py
+-rw-r--r--   0        0        0     3399 2023-07-01 01:06:25.788183 upstash_ratelimit-0.3.0/upstash_ratelimit/asyncio/token_bucket.py
+-rw-r--r--   0        0        0      167 2023-05-24 13:49:29.504075 upstash_ratelimit-0.3.0/upstash_ratelimit/config.py
+-rw-r--r--   0        0        0     3489 2023-07-01 01:05:05.419552 upstash_ratelimit-0.3.0/upstash_ratelimit/limiter.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:49:29.504232 upstash_ratelimit-0.3.0/upstash_ratelimit/py.typed
+-rw-r--r--   0        0        0      475 2023-06-21 04:18:16.326882 upstash_ratelimit-0.3.0/upstash_ratelimit/schema/response.py
+-rw-r--r--   0        0        0     2824 2023-07-01 01:01:07.547407 upstash_ratelimit-0.3.0/upstash_ratelimit/sync/fixed_window.py
+-rw-r--r--   0        0        0     3477 2023-07-01 01:01:01.211066 upstash_ratelimit-0.3.0/upstash_ratelimit/sync/sliding_window.py
+-rw-r--r--   0        0        0     1111 2023-07-01 01:00:30.604276 upstash_ratelimit-0.3.0/upstash_ratelimit/sync/sync_blocker.py
+-rw-r--r--   0        0        0     3185 2023-07-01 01:01:11.877570 upstash_ratelimit-0.3.0/upstash_ratelimit/sync/token_bucket.py
+-rw-r--r--   0        0        0      392 2023-06-21 04:18:16.327167 upstash_ratelimit-0.3.0/upstash_ratelimit/utils/time.py
+-rw-r--r--   0        0        0    11656 1970-01-01 00:00:00.000000 upstash_ratelimit-0.3.0/PKG-INFO
```

### Comparing `upstash_ratelimit-0.2.0/LICENSE` & `upstash_ratelimit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.2.0/README.md` & `upstash_ratelimit-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.2.0/PKG-INFO` & `upstash_ratelimit-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upstash-ratelimit
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: Zgîmbău Tudor
 Author-email: tudor.zgimbau@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

