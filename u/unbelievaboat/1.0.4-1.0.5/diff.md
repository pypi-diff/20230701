# Comparing `tmp/unbelievaboat-1.0.4.tar.gz` & `tmp/unbelievaboat-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unbelievaboat-1.0.4.tar", last modified: Sat Jul  1 17:01:40 2023, max compression
+gzip compressed data, was "unbelievaboat-1.0.5.tar", last modified: Sat Jul  1 18:54:31 2023, max compression
```

## Comparing `unbelievaboat-1.0.4.tar` & `unbelievaboat-1.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 17:01:40.137675 unbelievaboat-1.0.4/
--rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     3173 2023-07-01 17:01:40.136665 unbelievaboat-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2432 2023-07-01 16:02:14.000000 unbelievaboat-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-01 17:01:40.137675 unbelievaboat-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1084 2023-07-01 17:01:18.000000 unbelievaboat-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 17:01:40.087628 unbelievaboat-1.0.4/unbelievaboat/
--rw-rw-rw-   0        0        0     5584 2023-07-01 16:55:18.000000 unbelievaboat-1.0.4/unbelievaboat/Client.py
--rw-rw-rw-   0        0        0     3133 2023-07-01 14:59:51.000000 unbelievaboat-1.0.4/unbelievaboat/RequestHandler.py
--rw-rw-rw-   0        0        0      336 2023-07-01 14:55:29.000000 unbelievaboat-1.0.4/unbelievaboat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 17:01:40.113710 unbelievaboat-1.0.4/unbelievaboat/errors/
--rw-rw-rw-   0        0        0      572 2023-07-01 11:55:22.000000 unbelievaboat-1.0.4/unbelievaboat/errors/APIError.py
--rw-rw-rw-   0        0        0      551 2023-07-01 13:35:00.000000 unbelievaboat-1.0.4/unbelievaboat/errors/HTTPError.py
--rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.0.4/unbelievaboat/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 17:01:40.120417 unbelievaboat-1.0.4/unbelievaboat/structures/
--rw-rw-rw-   0        0        0      925 2023-07-01 16:58:46.000000 unbelievaboat-1.0.4/unbelievaboat/structures/Guild.py
--rw-rw-rw-   0        0        0      728 2023-07-01 16:59:19.000000 unbelievaboat-1.0.4/unbelievaboat/structures/Leaderboard.py
--rw-rw-rw-   0        0        0      929 2023-07-01 16:45:44.000000 unbelievaboat-1.0.4/unbelievaboat/structures/Permission.py
--rw-rw-rw-   0        0        0      704 2023-07-01 16:45:44.000000 unbelievaboat-1.0.4/unbelievaboat/structures/Store.py
--rw-rw-rw-   0        0        0     1240 2023-07-01 17:00:44.000000 unbelievaboat-1.0.4/unbelievaboat/structures/User.py
--rw-rw-rw-   0        0        0      362 2023-07-01 14:56:55.000000 unbelievaboat-1.0.4/unbelievaboat/structures/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 17:01:40.129288 unbelievaboat-1.0.4/unbelievaboat/structures/items/
--rw-rw-rw-   0        0        0     1293 2023-07-01 16:54:27.000000 unbelievaboat-1.0.4/unbelievaboat/structures/items/BaseItem.py
--rw-rw-rw-   0        0        0      429 2023-07-01 16:54:36.000000 unbelievaboat-1.0.4/unbelievaboat/structures/items/InventoryItem.py
--rw-rw-rw-   0        0        0     1353 2023-07-01 16:57:10.000000 unbelievaboat-1.0.4/unbelievaboat/structures/items/StoreItem.py
--rw-rw-rw-   0        0        0     1030 2023-07-01 16:54:52.000000 unbelievaboat-1.0.4/unbelievaboat/structures/items/StoreItemAction.py
--rw-rw-rw-   0        0        0     1296 2023-07-01 16:55:37.000000 unbelievaboat-1.0.4/unbelievaboat/structures/items/StoreItemRequirement.py
--rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.0.4/unbelievaboat/structures/items/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 17:01:40.134537 unbelievaboat-1.0.4/unbelievaboat/util/
--rw-rw-rw-   0        0        0     1143 2023-07-01 11:45:16.000000 unbelievaboat-1.0.4/unbelievaboat/util/Bucket.py
--rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.0.4/unbelievaboat/util/Constants.py
--rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.0.4/unbelievaboat/util/SnakeCaseConventer.py
--rw-rw-rw-   0        0        0      250 2023-07-01 13:41:07.000000 unbelievaboat-1.0.4/unbelievaboat/util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 17:01:40.109640 unbelievaboat-1.0.4/unbelievaboat.egg-info/
--rw-rw-rw-   0        0        0     3173 2023-07-01 17:01:39.000000 unbelievaboat-1.0.4/unbelievaboat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2023-07-01 17:01:40.000000 unbelievaboat-1.0.4/unbelievaboat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 17:01:39.000000 unbelievaboat-1.0.4/unbelievaboat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-01 17:01:39.000000 unbelievaboat-1.0.4/unbelievaboat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-01 17:01:39.000000 unbelievaboat-1.0.4/unbelievaboat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 18:54:31.540339 unbelievaboat-1.0.5/
+-rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3749 2023-07-01 18:54:31.538342 unbelievaboat-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3008 2023-07-01 18:53:47.000000 unbelievaboat-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-01 18:54:31.541690 unbelievaboat-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1084 2023-07-01 18:54:13.000000 unbelievaboat-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 18:54:31.331824 unbelievaboat-1.0.5/unbelievaboat/
+-rw-rw-rw-   0        0        0     5584 2023-07-01 16:55:18.000000 unbelievaboat-1.0.5/unbelievaboat/Client.py
+-rw-rw-rw-   0        0        0     3133 2023-07-01 14:59:51.000000 unbelievaboat-1.0.5/unbelievaboat/RequestHandler.py
+-rw-rw-rw-   0        0        0      336 2023-07-01 14:55:29.000000 unbelievaboat-1.0.5/unbelievaboat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 18:54:31.433503 unbelievaboat-1.0.5/unbelievaboat/errors/
+-rw-rw-rw-   0        0        0      572 2023-07-01 11:55:22.000000 unbelievaboat-1.0.5/unbelievaboat/errors/APIError.py
+-rw-rw-rw-   0        0        0      551 2023-07-01 13:35:00.000000 unbelievaboat-1.0.5/unbelievaboat/errors/HTTPError.py
+-rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.0.5/unbelievaboat/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 18:54:31.490214 unbelievaboat-1.0.5/unbelievaboat/structures/
+-rw-rw-rw-   0        0        0      925 2023-07-01 16:58:46.000000 unbelievaboat-1.0.5/unbelievaboat/structures/Guild.py
+-rw-rw-rw-   0        0        0      728 2023-07-01 16:59:19.000000 unbelievaboat-1.0.5/unbelievaboat/structures/Leaderboard.py
+-rw-rw-rw-   0        0        0      929 2023-07-01 16:45:44.000000 unbelievaboat-1.0.5/unbelievaboat/structures/Permission.py
+-rw-rw-rw-   0        0        0      704 2023-07-01 16:45:44.000000 unbelievaboat-1.0.5/unbelievaboat/structures/Store.py
+-rw-rw-rw-   0        0        0     1258 2023-07-01 18:53:50.000000 unbelievaboat-1.0.5/unbelievaboat/structures/User.py
+-rw-rw-rw-   0        0        0      362 2023-07-01 14:56:55.000000 unbelievaboat-1.0.5/unbelievaboat/structures/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 18:54:31.519812 unbelievaboat-1.0.5/unbelievaboat/structures/items/
+-rw-rw-rw-   0        0        0     1293 2023-07-01 16:54:27.000000 unbelievaboat-1.0.5/unbelievaboat/structures/items/BaseItem.py
+-rw-rw-rw-   0        0        0      429 2023-07-01 16:54:36.000000 unbelievaboat-1.0.5/unbelievaboat/structures/items/InventoryItem.py
+-rw-rw-rw-   0        0        0     1353 2023-07-01 16:57:10.000000 unbelievaboat-1.0.5/unbelievaboat/structures/items/StoreItem.py
+-rw-rw-rw-   0        0        0     1030 2023-07-01 16:54:52.000000 unbelievaboat-1.0.5/unbelievaboat/structures/items/StoreItemAction.py
+-rw-rw-rw-   0        0        0     1296 2023-07-01 16:55:37.000000 unbelievaboat-1.0.5/unbelievaboat/structures/items/StoreItemRequirement.py
+-rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.0.5/unbelievaboat/structures/items/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 18:54:31.534342 unbelievaboat-1.0.5/unbelievaboat/util/
+-rw-rw-rw-   0        0        0     1143 2023-07-01 11:45:16.000000 unbelievaboat-1.0.5/unbelievaboat/util/Bucket.py
+-rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.0.5/unbelievaboat/util/Constants.py
+-rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.0.5/unbelievaboat/util/SnakeCaseConventer.py
+-rw-rw-rw-   0        0        0      250 2023-07-01 13:41:07.000000 unbelievaboat-1.0.5/unbelievaboat/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 18:54:31.417418 unbelievaboat-1.0.5/unbelievaboat.egg-info/
+-rw-rw-rw-   0        0        0     3749 2023-07-01 18:54:31.000000 unbelievaboat-1.0.5/unbelievaboat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1025 2023-07-01 18:54:31.000000 unbelievaboat-1.0.5/unbelievaboat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 18:54:31.000000 unbelievaboat-1.0.5/unbelievaboat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-01 18:54:31.000000 unbelievaboat-1.0.5/unbelievaboat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-01 18:54:31.000000 unbelievaboat-1.0.5/unbelievaboat.egg-info/top_level.txt
```

### Comparing `unbelievaboat-1.0.4/LICENSE` & `unbelievaboat-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.4/PKG-INFO` & `unbelievaboat-1.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbelievaboat
-Version: 1.0.4
+Version: 1.0.5
 Summary: Wrapper for UnbelievaBoat API.
 Home-page: https://github.com/yoggys/unbelievaboat
 Author: yoggys
 Author-email: yoggies@yoggies.ovh
 Keywords: python,unb,unbelievaboat,api,wrapper,async,asyncio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -19,15 +19,14 @@
 
 # UnbelievaBoat API Python Wrapper
 
 [![Discord Server](https://img.shields.io/discord/746360067632136222?label=discord&style=for-the-badge&logo=discord&color=5865F2&logoColor=white)](https://discord.gg/yoggies)
 [![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/downloads/release/python-380/)
 [![PyPI Version](https://img.shields.io/pypi/v/unbelievaboat.svg?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/unbelievaboat/)
 
-
 This is a Python wrapper for the UnbelievaBoat API, which provides access to the UnbelievaBoat Discord bot functionality. It allows you to interact with the API endpoints to retrieve guild information, user balances, leaderboard data, and more.
 
 ## Requirements
 
 - Python 3.8 or higher
 
 ## Installation
@@ -52,16 +51,32 @@
     client = Client("your-api-token")
 
     # Retrieve guild information
     guild = await client.get_guild(guild_id)
     print(guild)
 
     # Retrieve user balance
-    user_balance = await client.get_user_balance(guild_id, user_id)
-    print(user_balance)
+    user = await client.get_user_balance(guild_id, user_id)
+    print(user.total)
+
+    # Set or update user balance
+    user = await client.set_user_balance(guild_id, user_id, {"bank": 100})
+    user = await client.update_user_balance(guild_id, user_id, {"bank": 100})
+    # or
+    user = await client.get_user_balance(guild_id, user_id)
+    user = await user.set_balance({"bank": 100})
+    user = await user.update_balance({"bank": 100})
+
+    # Retrieve leaderboard data
+    leaderboard = await client.get_leaderboard(guild_id)
+    print(leaderboard.users)
+
+    # Retrieve item shop data
+    shop = await client.get_shop(guild_id)
+    print(shop.items)
 
     # Close the client session
     await client.close()
 
 
 asyncio.run(main())
 ```
```

### Comparing `unbelievaboat-1.0.4/README.md` & `unbelievaboat-1.0.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # UnbelievaBoat API Python Wrapper
 
 [![Discord Server](https://img.shields.io/discord/746360067632136222?label=discord&style=for-the-badge&logo=discord&color=5865F2&logoColor=white)](https://discord.gg/yoggies)
 [![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/downloads/release/python-380/)
 [![PyPI Version](https://img.shields.io/pypi/v/unbelievaboat.svg?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/unbelievaboat/)
 
-
 This is a Python wrapper for the UnbelievaBoat API, which provides access to the UnbelievaBoat Discord bot functionality. It allows you to interact with the API endpoints to retrieve guild information, user balances, leaderboard data, and more.
 
 ## Requirements
 
 - Python 3.8 or higher
 
 ## Installation
@@ -33,16 +32,32 @@
     client = Client("your-api-token")
 
     # Retrieve guild information
     guild = await client.get_guild(guild_id)
     print(guild)
 
     # Retrieve user balance
-    user_balance = await client.get_user_balance(guild_id, user_id)
-    print(user_balance)
+    user = await client.get_user_balance(guild_id, user_id)
+    print(user.total)
+
+    # Set or update user balance
+    user = await client.set_user_balance(guild_id, user_id, {"bank": 100})
+    user = await client.update_user_balance(guild_id, user_id, {"bank": 100})
+    # or
+    user = await client.get_user_balance(guild_id, user_id)
+    user = await user.set_balance({"bank": 100})
+    user = await user.update_balance({"bank": 100})
+
+    # Retrieve leaderboard data
+    leaderboard = await client.get_leaderboard(guild_id)
+    print(leaderboard.users)
+
+    # Retrieve item shop data
+    shop = await client.get_shop(guild_id)
+    print(shop.items)
 
     # Close the client session
     await client.close()
 
 
 asyncio.run(main())
 ```
```

### Comparing `unbelievaboat-1.0.4/setup.py` & `unbelievaboat-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 cwd = Path(__file__).parent
 long_description = (cwd / "README.md").read_text()
 
 setup(
     name="unbelievaboat",
-    version="1.0.4",
+    version="1.0.5",
     author="yoggys",
     author_email="yoggies@yoggies.ovh",
     description="Wrapper for UnbelievaBoat API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yoggys/unbelievaboat",
     packages=find_packages(),
```

### Comparing `unbelievaboat-1.0.4/unbelievaboat/Client.py` & `unbelievaboat-1.0.5/unbelievaboat/Client.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.4/unbelievaboat/RequestHandler.py` & `unbelievaboat-1.0.5/unbelievaboat/RequestHandler.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.4/unbelievaboat/errors/APIError.py` & `unbelievaboat-1.0.5/unbelievaboat/errors/APIError.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.4/unbelievaboat/errors/HTTPError.py` & `unbelievaboat-1.0.5/unbelievaboat/errors/HTTPError.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.4/unbelievaboat/structures/Guild.py` & `unbelievaboat-1.0.5/unbelievaboat/structures/Guild.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.4/unbelievaboat/structures/Leaderboard.py` & `unbelievaboat-1.0.5/unbelievaboat/structures/Leaderboard.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.4/unbelievaboat/structures/Permission.py` & `unbelievaboat-1.0.5/unbelievaboat/structures/Permission.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.4/unbelievaboat/structures/Store.py` & `unbelievaboat-1.0.5/unbelievaboat/structures/Store.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.4/unbelievaboat/structures/User.py` & `unbelievaboat-1.0.5/unbelievaboat/structures/User.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,12 +24,14 @@
 
     async def set_balance(self, data: Dict[str, Any] = {}, reason: str = None) -> Self:
         self = await self._client.set_user_balance(
             self.guild_id, self.user_id, data, reason
         )
         return self
 
-    async def edit_balance(self, data: Dict[str, Any] = {}, reason: str = None) -> Self:
+    async def update_balance(
+        self, data: Dict[str, Any] = {}, reason: str = None
+    ) -> Self:
         self = await self._client.edit_user_balance(
             self.guild_id, self.user_id, data, reason
         )
         return self
```

### Comparing `unbelievaboat-1.0.4/unbelievaboat/structures/items/BaseItem.py` & `unbelievaboat-1.0.5/unbelievaboat/structures/items/BaseItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.4/unbelievaboat/structures/items/StoreItem.py` & `unbelievaboat-1.0.5/unbelievaboat/structures/items/StoreItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.4/unbelievaboat/structures/items/StoreItemAction.py` & `unbelievaboat-1.0.5/unbelievaboat/structures/items/StoreItemAction.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.4/unbelievaboat/structures/items/StoreItemRequirement.py` & `unbelievaboat-1.0.5/unbelievaboat/structures/items/StoreItemRequirement.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.4/unbelievaboat/util/Bucket.py` & `unbelievaboat-1.0.5/unbelievaboat/util/Bucket.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.4/unbelievaboat/util/SnakeCaseConventer.py` & `unbelievaboat-1.0.5/unbelievaboat/util/SnakeCaseConventer.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.4/unbelievaboat.egg-info/PKG-INFO` & `unbelievaboat-1.0.5/unbelievaboat.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbelievaboat
-Version: 1.0.4
+Version: 1.0.5
 Summary: Wrapper for UnbelievaBoat API.
 Home-page: https://github.com/yoggys/unbelievaboat
 Author: yoggys
 Author-email: yoggies@yoggies.ovh
 Keywords: python,unb,unbelievaboat,api,wrapper,async,asyncio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -19,15 +19,14 @@
 
 # UnbelievaBoat API Python Wrapper
 
 [![Discord Server](https://img.shields.io/discord/746360067632136222?label=discord&style=for-the-badge&logo=discord&color=5865F2&logoColor=white)](https://discord.gg/yoggies)
 [![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/downloads/release/python-380/)
 [![PyPI Version](https://img.shields.io/pypi/v/unbelievaboat.svg?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/unbelievaboat/)
 
-
 This is a Python wrapper for the UnbelievaBoat API, which provides access to the UnbelievaBoat Discord bot functionality. It allows you to interact with the API endpoints to retrieve guild information, user balances, leaderboard data, and more.
 
 ## Requirements
 
 - Python 3.8 or higher
 
 ## Installation
@@ -52,16 +51,32 @@
     client = Client("your-api-token")
 
     # Retrieve guild information
     guild = await client.get_guild(guild_id)
     print(guild)
 
     # Retrieve user balance
-    user_balance = await client.get_user_balance(guild_id, user_id)
-    print(user_balance)
+    user = await client.get_user_balance(guild_id, user_id)
+    print(user.total)
+
+    # Set or update user balance
+    user = await client.set_user_balance(guild_id, user_id, {"bank": 100})
+    user = await client.update_user_balance(guild_id, user_id, {"bank": 100})
+    # or
+    user = await client.get_user_balance(guild_id, user_id)
+    user = await user.set_balance({"bank": 100})
+    user = await user.update_balance({"bank": 100})
+
+    # Retrieve leaderboard data
+    leaderboard = await client.get_leaderboard(guild_id)
+    print(leaderboard.users)
+
+    # Retrieve item shop data
+    shop = await client.get_shop(guild_id)
+    print(shop.items)
 
     # Close the client session
     await client.close()
 
 
 asyncio.run(main())
 ```
```

### Comparing `unbelievaboat-1.0.4/unbelievaboat.egg-info/SOURCES.txt` & `unbelievaboat-1.0.5/unbelievaboat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

