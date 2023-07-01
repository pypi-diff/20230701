# Comparing `tmp/unbelievaboat-1.0.1.tar.gz` & `tmp/unbelievaboat-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unbelievaboat-1.0.1.tar", last modified: Sat Jul  1 15:40:59 2023, max compression
+gzip compressed data, was "unbelievaboat-1.0.2.tar", last modified: Sat Jul  1 15:42:43 2023, max compression
```

## Comparing `unbelievaboat-1.0.1.tar` & `unbelievaboat-1.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 15:40:59.344047 unbelievaboat-1.0.1/
--rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2780 2023-07-01 15:40:59.342998 unbelievaboat-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1996 2023-07-01 15:23:34.000000 unbelievaboat-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-01 15:40:59.344047 unbelievaboat-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1064 2023-07-01 15:40:51.000000 unbelievaboat-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 15:40:59.293868 unbelievaboat-1.0.1/unbelievaboat/
--rw-rw-rw-   0        0        0     5396 2023-07-01 14:59:44.000000 unbelievaboat-1.0.1/unbelievaboat/Client.py
--rw-rw-rw-   0        0        0     3133 2023-07-01 14:59:51.000000 unbelievaboat-1.0.1/unbelievaboat/RequestHandler.py
--rw-rw-rw-   0        0        0      336 2023-07-01 14:55:29.000000 unbelievaboat-1.0.1/unbelievaboat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 15:40:59.322193 unbelievaboat-1.0.1/unbelievaboat/errors/
--rw-rw-rw-   0        0        0      572 2023-07-01 11:55:22.000000 unbelievaboat-1.0.1/unbelievaboat/errors/APIError.py
--rw-rw-rw-   0        0        0      551 2023-07-01 13:35:00.000000 unbelievaboat-1.0.1/unbelievaboat/errors/HTTPError.py
--rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.0.1/unbelievaboat/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 15:40:59.329815 unbelievaboat-1.0.1/unbelievaboat/structures/
--rw-rw-rw-   0        0        0      944 2023-07-01 14:37:58.000000 unbelievaboat-1.0.1/unbelievaboat/structures/Guild.py
--rw-rw-rw-   0        0        0      694 2023-07-01 14:56:59.000000 unbelievaboat-1.0.1/unbelievaboat/structures/Leaderboard.py
--rw-rw-rw-   0        0        0      929 2023-07-01 14:38:30.000000 unbelievaboat-1.0.1/unbelievaboat/structures/Permission.py
--rw-rw-rw-   0        0        0      650 2023-07-01 15:01:25.000000 unbelievaboat-1.0.1/unbelievaboat/structures/Store.py
--rw-rw-rw-   0        0        0      601 2023-07-01 14:12:42.000000 unbelievaboat-1.0.1/unbelievaboat/structures/User.py
--rw-rw-rw-   0        0        0      362 2023-07-01 14:56:55.000000 unbelievaboat-1.0.1/unbelievaboat/structures/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 15:40:59.336565 unbelievaboat-1.0.1/unbelievaboat/structures/items/
--rw-rw-rw-   0        0        0     1272 2023-07-01 14:50:40.000000 unbelievaboat-1.0.1/unbelievaboat/structures/items/BaseItem.py
--rw-rw-rw-   0        0        0      387 2023-07-01 14:50:40.000000 unbelievaboat-1.0.1/unbelievaboat/structures/items/InventoryItem.py
--rw-rw-rw-   0        0        0      966 2023-07-01 14:50:40.000000 unbelievaboat-1.0.1/unbelievaboat/structures/items/StoreItem.py
--rw-rw-rw-   0        0        0     1009 2023-07-01 14:50:40.000000 unbelievaboat-1.0.1/unbelievaboat/structures/items/StoreItemAction.py
--rw-rw-rw-   0        0        0     1275 2023-07-01 14:50:40.000000 unbelievaboat-1.0.1/unbelievaboat/structures/items/StoreItemRequirement.py
--rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.0.1/unbelievaboat/structures/items/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 15:40:59.341492 unbelievaboat-1.0.1/unbelievaboat/util/
--rw-rw-rw-   0        0        0     1143 2023-07-01 11:45:16.000000 unbelievaboat-1.0.1/unbelievaboat/util/Bucket.py
--rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.0.1/unbelievaboat/util/Constants.py
--rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.0.1/unbelievaboat/util/SnakeCaseConventer.py
--rw-rw-rw-   0        0        0      250 2023-07-01 13:41:07.000000 unbelievaboat-1.0.1/unbelievaboat/util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 15:40:59.317720 unbelievaboat-1.0.1/unbelievaboat.egg-info/
--rw-rw-rw-   0        0        0     2780 2023-07-01 15:40:59.000000 unbelievaboat-1.0.1/unbelievaboat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2023-07-01 15:40:59.000000 unbelievaboat-1.0.1/unbelievaboat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 15:40:59.000000 unbelievaboat-1.0.1/unbelievaboat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-01 15:40:59.000000 unbelievaboat-1.0.1/unbelievaboat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-01 15:40:59.000000 unbelievaboat-1.0.1/unbelievaboat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 15:42:43.167580 unbelievaboat-1.0.2/
+-rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2778 2023-07-01 15:42:43.167580 unbelievaboat-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1994 2023-07-01 15:42:11.000000 unbelievaboat-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-01 15:42:43.168518 unbelievaboat-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2023-07-01 15:42:40.000000 unbelievaboat-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:42:43.101649 unbelievaboat-1.0.2/unbelievaboat/
+-rw-rw-rw-   0        0        0     5396 2023-07-01 14:59:44.000000 unbelievaboat-1.0.2/unbelievaboat/Client.py
+-rw-rw-rw-   0        0        0     3133 2023-07-01 14:59:51.000000 unbelievaboat-1.0.2/unbelievaboat/RequestHandler.py
+-rw-rw-rw-   0        0        0      336 2023-07-01 14:55:29.000000 unbelievaboat-1.0.2/unbelievaboat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:42:43.144415 unbelievaboat-1.0.2/unbelievaboat/errors/
+-rw-rw-rw-   0        0        0      572 2023-07-01 11:55:22.000000 unbelievaboat-1.0.2/unbelievaboat/errors/APIError.py
+-rw-rw-rw-   0        0        0      551 2023-07-01 13:35:00.000000 unbelievaboat-1.0.2/unbelievaboat/errors/HTTPError.py
+-rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.0.2/unbelievaboat/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:42:43.152218 unbelievaboat-1.0.2/unbelievaboat/structures/
+-rw-rw-rw-   0        0        0      944 2023-07-01 14:37:58.000000 unbelievaboat-1.0.2/unbelievaboat/structures/Guild.py
+-rw-rw-rw-   0        0        0      694 2023-07-01 14:56:59.000000 unbelievaboat-1.0.2/unbelievaboat/structures/Leaderboard.py
+-rw-rw-rw-   0        0        0      929 2023-07-01 14:38:30.000000 unbelievaboat-1.0.2/unbelievaboat/structures/Permission.py
+-rw-rw-rw-   0        0        0      650 2023-07-01 15:01:25.000000 unbelievaboat-1.0.2/unbelievaboat/structures/Store.py
+-rw-rw-rw-   0        0        0      601 2023-07-01 14:12:42.000000 unbelievaboat-1.0.2/unbelievaboat/structures/User.py
+-rw-rw-rw-   0        0        0      362 2023-07-01 14:56:55.000000 unbelievaboat-1.0.2/unbelievaboat/structures/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:42:43.160488 unbelievaboat-1.0.2/unbelievaboat/structures/items/
+-rw-rw-rw-   0        0        0     1272 2023-07-01 14:50:40.000000 unbelievaboat-1.0.2/unbelievaboat/structures/items/BaseItem.py
+-rw-rw-rw-   0        0        0      387 2023-07-01 14:50:40.000000 unbelievaboat-1.0.2/unbelievaboat/structures/items/InventoryItem.py
+-rw-rw-rw-   0        0        0      966 2023-07-01 14:50:40.000000 unbelievaboat-1.0.2/unbelievaboat/structures/items/StoreItem.py
+-rw-rw-rw-   0        0        0     1009 2023-07-01 14:50:40.000000 unbelievaboat-1.0.2/unbelievaboat/structures/items/StoreItemAction.py
+-rw-rw-rw-   0        0        0     1275 2023-07-01 14:50:40.000000 unbelievaboat-1.0.2/unbelievaboat/structures/items/StoreItemRequirement.py
+-rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.0.2/unbelievaboat/structures/items/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:42:43.166004 unbelievaboat-1.0.2/unbelievaboat/util/
+-rw-rw-rw-   0        0        0     1143 2023-07-01 11:45:16.000000 unbelievaboat-1.0.2/unbelievaboat/util/Bucket.py
+-rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.0.2/unbelievaboat/util/Constants.py
+-rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.0.2/unbelievaboat/util/SnakeCaseConventer.py
+-rw-rw-rw-   0        0        0      250 2023-07-01 13:41:07.000000 unbelievaboat-1.0.2/unbelievaboat/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:42:43.138941 unbelievaboat-1.0.2/unbelievaboat.egg-info/
+-rw-rw-rw-   0        0        0     2778 2023-07-01 15:42:42.000000 unbelievaboat-1.0.2/unbelievaboat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1025 2023-07-01 15:42:43.000000 unbelievaboat-1.0.2/unbelievaboat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 15:42:42.000000 unbelievaboat-1.0.2/unbelievaboat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-01 15:42:42.000000 unbelievaboat-1.0.2/unbelievaboat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-01 15:42:42.000000 unbelievaboat-1.0.2/unbelievaboat.egg-info/top_level.txt
```

### Comparing `unbelievaboat-1.0.1/LICENSE` & `unbelievaboat-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.1/PKG-INFO` & `unbelievaboat-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbelievaboat
-Version: 1.0.1
+Version: 1.0.2
 Summary: Wrapper for UnbelievaBoat API.
 Home-page: https://github.com/yoggys/unbelievaboat
 Author: yoggys
 Author-email: yoggies@yoggies.ovh
 Keywords: python,unb,unbelievaboat,api,wrapper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -61,15 +61,15 @@
 
 
 asyncio.run(main())
 ```
 
 Replace `"your-api-token"` with your actual API token. You can obtain an API token by logging into the UnbelievaBoat dashboard and generating a token for your bot.
 
-Please note that the above example demonstrates a basic usage scenario. You can explore other available methods in the `Client` class to interact with different API endpoints. You can also find more examples in the [examples](https://github.com/yoggys/unbelievaboat/tree/master/examples) directory.
+Please note that the above example demonstrates a basic usage scenario. You can explore other available methods in the `Client` class to interact with different API endpoints. You can also find more examples in the [examples](https://github.com/yoggys/unbelievaboat/tree/main/examples) directory.
 
 ## Contributing
 
 Contributions are welcome! If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/yoggys/unbelievaboat).
 
 ## License
```

### Comparing `unbelievaboat-1.0.1/README.md` & `unbelievaboat-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 
 asyncio.run(main())
 ```
 
 Replace `"your-api-token"` with your actual API token. You can obtain an API token by logging into the UnbelievaBoat dashboard and generating a token for your bot.
 
-Please note that the above example demonstrates a basic usage scenario. You can explore other available methods in the `Client` class to interact with different API endpoints. You can also find more examples in the [examples](https://github.com/yoggys/unbelievaboat/tree/master/examples) directory.
+Please note that the above example demonstrates a basic usage scenario. You can explore other available methods in the `Client` class to interact with different API endpoints. You can also find more examples in the [examples](https://github.com/yoggys/unbelievaboat/tree/main/examples) directory.
 
 ## Contributing
 
 Contributions are welcome! If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/yoggys/unbelievaboat).
 
 ## License
```

### Comparing `unbelievaboat-1.0.1/setup.py` & `unbelievaboat-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 cwd = Path(__file__).parent
 long_description = (cwd / "README.md").read_text()
 
 setup(
     name="unbelievaboat",
-    version="1.0.1",
+    version="1.0.2",
     author="yoggys",
     author_email="yoggies@yoggies.ovh",
     description="Wrapper for UnbelievaBoat API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yoggys/unbelievaboat",
     packages=find_packages(),
```

### Comparing `unbelievaboat-1.0.1/unbelievaboat/Client.py` & `unbelievaboat-1.0.2/unbelievaboat/Client.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.1/unbelievaboat/RequestHandler.py` & `unbelievaboat-1.0.2/unbelievaboat/RequestHandler.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.1/unbelievaboat/errors/APIError.py` & `unbelievaboat-1.0.2/unbelievaboat/errors/APIError.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.1/unbelievaboat/errors/HTTPError.py` & `unbelievaboat-1.0.2/unbelievaboat/errors/HTTPError.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.1/unbelievaboat/structures/Guild.py` & `unbelievaboat-1.0.2/unbelievaboat/structures/Guild.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.1/unbelievaboat/structures/Leaderboard.py` & `unbelievaboat-1.0.2/unbelievaboat/structures/Leaderboard.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.1/unbelievaboat/structures/Permission.py` & `unbelievaboat-1.0.2/unbelievaboat/structures/Permission.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.1/unbelievaboat/structures/Store.py` & `unbelievaboat-1.0.2/unbelievaboat/structures/Store.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.1/unbelievaboat/structures/User.py` & `unbelievaboat-1.0.2/unbelievaboat/structures/User.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.1/unbelievaboat/structures/items/BaseItem.py` & `unbelievaboat-1.0.2/unbelievaboat/structures/items/BaseItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.1/unbelievaboat/structures/items/StoreItem.py` & `unbelievaboat-1.0.2/unbelievaboat/structures/items/StoreItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.1/unbelievaboat/structures/items/StoreItemAction.py` & `unbelievaboat-1.0.2/unbelievaboat/structures/items/StoreItemAction.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.1/unbelievaboat/structures/items/StoreItemRequirement.py` & `unbelievaboat-1.0.2/unbelievaboat/structures/items/StoreItemRequirement.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.1/unbelievaboat/util/Bucket.py` & `unbelievaboat-1.0.2/unbelievaboat/util/Bucket.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.1/unbelievaboat/util/SnakeCaseConventer.py` & `unbelievaboat-1.0.2/unbelievaboat/util/SnakeCaseConventer.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.1/unbelievaboat.egg-info/PKG-INFO` & `unbelievaboat-1.0.2/unbelievaboat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbelievaboat
-Version: 1.0.1
+Version: 1.0.2
 Summary: Wrapper for UnbelievaBoat API.
 Home-page: https://github.com/yoggys/unbelievaboat
 Author: yoggys
 Author-email: yoggies@yoggies.ovh
 Keywords: python,unb,unbelievaboat,api,wrapper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -61,15 +61,15 @@
 
 
 asyncio.run(main())
 ```
 
 Replace `"your-api-token"` with your actual API token. You can obtain an API token by logging into the UnbelievaBoat dashboard and generating a token for your bot.
 
-Please note that the above example demonstrates a basic usage scenario. You can explore other available methods in the `Client` class to interact with different API endpoints. You can also find more examples in the [examples](https://github.com/yoggys/unbelievaboat/tree/master/examples) directory.
+Please note that the above example demonstrates a basic usage scenario. You can explore other available methods in the `Client` class to interact with different API endpoints. You can also find more examples in the [examples](https://github.com/yoggys/unbelievaboat/tree/main/examples) directory.
 
 ## Contributing
 
 Contributions are welcome! If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/yoggys/unbelievaboat).
 
 ## License
```

### Comparing `unbelievaboat-1.0.1/unbelievaboat.egg-info/SOURCES.txt` & `unbelievaboat-1.0.2/unbelievaboat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

