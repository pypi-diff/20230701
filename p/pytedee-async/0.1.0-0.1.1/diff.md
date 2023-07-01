# Comparing `tmp/pytedee_async-0.1.0.tar.gz` & `tmp/pytedee_async-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytedee_async-0.1.0.tar", last modified: Fri Jun 30 20:11:57 2023, max compression
+gzip compressed data, was "pytedee_async-0.1.1.tar", last modified: Sat Jul  1 06:38:49 2023, max compression
```

## Comparing `pytedee_async-0.1.0.tar` & `pytedee_async-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:11:57.388900 pytedee_async-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-30 20:11:43.000000 pytedee_async-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-30 20:11:57.388900 pytedee_async-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-30 20:11:43.000000 pytedee_async-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:11:57.388900 pytedee_async-0.1.0/pytedee_async/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-30 20:11:43.000000 pytedee_async-0.1.0/pytedee_async/Lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-06-30 20:11:43.000000 pytedee_async-0.1.0/pytedee_async/TedeeClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-30 20:11:43.000000 pytedee_async-0.1.0/pytedee_async/TedeeClientException.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 20:11:43.000000 pytedee_async-0.1.0/pytedee_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-30 20:11:43.000000 pytedee_async-0.1.0/pytedee_async/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-30 20:11:43.000000 pytedee_async-0.1.0/pytedee_async/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:11:57.388900 pytedee_async-0.1.0/pytedee_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-30 20:11:57.000000 pytedee_async-0.1.0/pytedee_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-30 20:11:57.000000 pytedee_async-0.1.0/pytedee_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 20:11:57.000000 pytedee_async-0.1.0/pytedee_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 20:11:57.000000 pytedee_async-0.1.0/pytedee_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 20:11:57.000000 pytedee_async-0.1.0/pytedee_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 20:11:57.388900 pytedee_async-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-30 20:11:43.000000 pytedee_async-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:38:49.458268 pytedee_async-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-01 06:38:35.000000 pytedee_async-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-01 06:38:49.458268 pytedee_async-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-01 06:38:35.000000 pytedee_async-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:38:49.458268 pytedee_async-0.1.1/pytedee_async/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-01 06:38:35.000000 pytedee_async-0.1.1/pytedee_async/Lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-07-01 06:38:35.000000 pytedee_async-0.1.1/pytedee_async/TedeeClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-01 06:38:35.000000 pytedee_async-0.1.1/pytedee_async/TedeeClientException.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-01 06:38:35.000000 pytedee_async-0.1.1/pytedee_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-01 06:38:35.000000 pytedee_async-0.1.1/pytedee_async/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-01 06:38:35.000000 pytedee_async-0.1.1/pytedee_async/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:38:49.458268 pytedee_async-0.1.1/pytedee_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-01 06:38:49.000000 pytedee_async-0.1.1/pytedee_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-01 06:38:49.000000 pytedee_async-0.1.1/pytedee_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 06:38:49.000000 pytedee_async-0.1.1/pytedee_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-01 06:38:49.000000 pytedee_async-0.1.1/pytedee_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-01 06:38:49.000000 pytedee_async-0.1.1/pytedee_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 06:38:49.458268 pytedee_async-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-01 06:38:35.000000 pytedee_async-0.1.1/setup.py
```

### Comparing `pytedee_async-0.1.0/LICENSE` & `pytedee_async-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.1.0/PKG-INFO` & `pytedee_async-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytedee_async
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Tedee Lock Client package
 Home-page: https://github.com/zweckj/pytedee_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pytedee_async-0.1.0/README.md` & `pytedee_async-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.1.0/pytedee_async/Lock.py` & `pytedee_async-0.1.1/pytedee_async/Lock.py`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.1.0/pytedee_async/TedeeClient.py` & `pytedee_async-0.1.1/pytedee_async/TedeeClient.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,18 +73,18 @@
                 elif response.status == 401:
                     raise TedeeAuthException()
                 elif response.status == 429:
                     raise TedeeRateLimitException()
                 else:
                     raise TedeeClientException(f"Error during listing of devices. Status code {response.status}")
                     
-    # unlocking
+
     async def unlock(self, lock_id) -> None:
         '''Unlock method'''
-        url = API_URL_LOCK + str(lock_id) + API_PATH_UNLOCK
+        url = API_URL_LOCK + str(lock_id) + API_PATH_UNLOCK + "?mode=3"
         
         async with aiohttp.ClientSession(
                 headers=self._api_header, 
                 timeout=aiohttp.ClientTimeout(total=self._timeout)
             ) as session:
             async with session.post(url) as response:
                 if response.status == 202:
@@ -98,15 +98,15 @@
                 elif response.status == 401:
                     raise TedeeAuthException()
                 elif response.status == 429:
                     raise TedeeRateLimitException()
                 else:
                     raise TedeeClientException(f"Error during unlocking of lock {lock_id}. Status code {response.status}")
             
-    # locking
+
     async def lock(self, lock_id) -> None:
         ''''Lock method'''
 
         url = API_URL_LOCK + str(lock_id) + API_PATH_LOCK
         async with aiohttp.ClientSession(
                 headers=self._api_header, 
                 timeout=aiohttp.ClientTimeout(total=self._timeout)
@@ -123,15 +123,41 @@
                 elif response.status == 429:
                     raise TedeeRateLimitException()
                 else:
                     raise TedeeClientException(f"Error during locking of lock {lock_id}. Status code {response.status}")
 
     # pulling  
     async def open(self, lock_id) -> None:
-        '''Open the door latch'''
+        '''Unlock the door and pull the door latch'''
+
+        url = API_URL_LOCK + str(lock_id) + API_PATH_UNLOCK + "?mode=4"
+        self._locks_dict[lock_id].state = 4
+        
+        async with aiohttp.ClientSession(
+                headers=self._api_header, 
+                timeout=aiohttp.ClientTimeout(total=self._timeout)
+            ) as session:
+            async with session.post(url) as response:
+                
+                if response.status == 202:
+                    self._locks_dict[lock_id].state = 2
+                    _LOGGER.debug(f"open command successful, id: {lock_id}")
+
+                    await asyncio.sleep(self._locks_dict[lock_id].duration_pullspring + 1)
+                    await self.get_locks()
+                elif response.status == 401:
+                    raise TedeeAuthException()
+                elif response.status == 429:
+                    raise TedeeRateLimitException()
+                else: 
+                    raise TedeeClientException(f"Error during unlatching of lock {lock_id}. Status code {response.status}")
+                
+
+    async def pull(self, lock_id) -> None:
+        '''Only pull the door latch'''
 
         url = API_URL_LOCK + str(lock_id) + API_PATH_PULL
         self._locks_dict[lock_id].state = 8
         
         async with aiohttp.ClientSession(
                 headers=self._api_header, 
                 timeout=aiohttp.ClientTimeout(total=self._timeout)
```

### Comparing `pytedee_async-0.1.0/pytedee_async/helpers.py` & `pytedee_async-0.1.1/pytedee_async/helpers.py`

 * *Files identical despite different names*

### Comparing `pytedee_async-0.1.0/pytedee_async.egg-info/PKG-INFO` & `pytedee_async-0.1.1/pytedee_async.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytedee-async
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Tedee Lock Client package
 Home-page: https://github.com/zweckj/pytedee_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pytedee_async-0.1.0/setup.py` & `pytedee_async-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytedee_async", 
-    version="0.1.0",
+    version="0.1.1",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     description="A Tedee Lock Client package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/pytedee_async",
     packages=setuptools.find_packages(),
```

