# Comparing `tmp/unbelievaboat-1.0.2.tar.gz` & `tmp/unbelievaboat-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unbelievaboat-1.0.2.tar", last modified: Sat Jul  1 15:42:43 2023, max compression
+gzip compressed data, was "unbelievaboat-1.0.3.tar", last modified: Sat Jul  1 16:03:11 2023, max compression
```

## Comparing `unbelievaboat-1.0.2.tar` & `unbelievaboat-1.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 15:42:43.167580 unbelievaboat-1.0.2/
--rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     2778 2023-07-01 15:42:43.167580 unbelievaboat-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1994 2023-07-01 15:42:11.000000 unbelievaboat-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-01 15:42:43.168518 unbelievaboat-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1064 2023-07-01 15:42:40.000000 unbelievaboat-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 15:42:43.101649 unbelievaboat-1.0.2/unbelievaboat/
--rw-rw-rw-   0        0        0     5396 2023-07-01 14:59:44.000000 unbelievaboat-1.0.2/unbelievaboat/Client.py
--rw-rw-rw-   0        0        0     3133 2023-07-01 14:59:51.000000 unbelievaboat-1.0.2/unbelievaboat/RequestHandler.py
--rw-rw-rw-   0        0        0      336 2023-07-01 14:55:29.000000 unbelievaboat-1.0.2/unbelievaboat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 15:42:43.144415 unbelievaboat-1.0.2/unbelievaboat/errors/
--rw-rw-rw-   0        0        0      572 2023-07-01 11:55:22.000000 unbelievaboat-1.0.2/unbelievaboat/errors/APIError.py
--rw-rw-rw-   0        0        0      551 2023-07-01 13:35:00.000000 unbelievaboat-1.0.2/unbelievaboat/errors/HTTPError.py
--rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.0.2/unbelievaboat/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 15:42:43.152218 unbelievaboat-1.0.2/unbelievaboat/structures/
--rw-rw-rw-   0        0        0      944 2023-07-01 14:37:58.000000 unbelievaboat-1.0.2/unbelievaboat/structures/Guild.py
--rw-rw-rw-   0        0        0      694 2023-07-01 14:56:59.000000 unbelievaboat-1.0.2/unbelievaboat/structures/Leaderboard.py
--rw-rw-rw-   0        0        0      929 2023-07-01 14:38:30.000000 unbelievaboat-1.0.2/unbelievaboat/structures/Permission.py
--rw-rw-rw-   0        0        0      650 2023-07-01 15:01:25.000000 unbelievaboat-1.0.2/unbelievaboat/structures/Store.py
--rw-rw-rw-   0        0        0      601 2023-07-01 14:12:42.000000 unbelievaboat-1.0.2/unbelievaboat/structures/User.py
--rw-rw-rw-   0        0        0      362 2023-07-01 14:56:55.000000 unbelievaboat-1.0.2/unbelievaboat/structures/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 15:42:43.160488 unbelievaboat-1.0.2/unbelievaboat/structures/items/
--rw-rw-rw-   0        0        0     1272 2023-07-01 14:50:40.000000 unbelievaboat-1.0.2/unbelievaboat/structures/items/BaseItem.py
--rw-rw-rw-   0        0        0      387 2023-07-01 14:50:40.000000 unbelievaboat-1.0.2/unbelievaboat/structures/items/InventoryItem.py
--rw-rw-rw-   0        0        0      966 2023-07-01 14:50:40.000000 unbelievaboat-1.0.2/unbelievaboat/structures/items/StoreItem.py
--rw-rw-rw-   0        0        0     1009 2023-07-01 14:50:40.000000 unbelievaboat-1.0.2/unbelievaboat/structures/items/StoreItemAction.py
--rw-rw-rw-   0        0        0     1275 2023-07-01 14:50:40.000000 unbelievaboat-1.0.2/unbelievaboat/structures/items/StoreItemRequirement.py
--rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.0.2/unbelievaboat/structures/items/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 15:42:43.166004 unbelievaboat-1.0.2/unbelievaboat/util/
--rw-rw-rw-   0        0        0     1143 2023-07-01 11:45:16.000000 unbelievaboat-1.0.2/unbelievaboat/util/Bucket.py
--rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.0.2/unbelievaboat/util/Constants.py
--rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.0.2/unbelievaboat/util/SnakeCaseConventer.py
--rw-rw-rw-   0        0        0      250 2023-07-01 13:41:07.000000 unbelievaboat-1.0.2/unbelievaboat/util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 15:42:43.138941 unbelievaboat-1.0.2/unbelievaboat.egg-info/
--rw-rw-rw-   0        0        0     2778 2023-07-01 15:42:42.000000 unbelievaboat-1.0.2/unbelievaboat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2023-07-01 15:42:43.000000 unbelievaboat-1.0.2/unbelievaboat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 15:42:42.000000 unbelievaboat-1.0.2/unbelievaboat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-01 15:42:42.000000 unbelievaboat-1.0.2/unbelievaboat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-01 15:42:42.000000 unbelievaboat-1.0.2/unbelievaboat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 16:03:11.475788 unbelievaboat-1.0.3/
+-rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3159 2023-07-01 16:03:11.474783 unbelievaboat-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2432 2023-07-01 16:02:14.000000 unbelievaboat-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-01 16:03:11.475788 unbelievaboat-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2023-07-01 16:02:47.000000 unbelievaboat-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 16:03:11.410235 unbelievaboat-1.0.3/unbelievaboat/
+-rw-rw-rw-   0        0        0     5396 2023-07-01 14:59:44.000000 unbelievaboat-1.0.3/unbelievaboat/Client.py
+-rw-rw-rw-   0        0        0     3133 2023-07-01 14:59:51.000000 unbelievaboat-1.0.3/unbelievaboat/RequestHandler.py
+-rw-rw-rw-   0        0        0      336 2023-07-01 14:55:29.000000 unbelievaboat-1.0.3/unbelievaboat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 16:03:11.452526 unbelievaboat-1.0.3/unbelievaboat/errors/
+-rw-rw-rw-   0        0        0      572 2023-07-01 11:55:22.000000 unbelievaboat-1.0.3/unbelievaboat/errors/APIError.py
+-rw-rw-rw-   0        0        0      551 2023-07-01 13:35:00.000000 unbelievaboat-1.0.3/unbelievaboat/errors/HTTPError.py
+-rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.0.3/unbelievaboat/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 16:03:11.460034 unbelievaboat-1.0.3/unbelievaboat/structures/
+-rw-rw-rw-   0        0        0      944 2023-07-01 14:37:58.000000 unbelievaboat-1.0.3/unbelievaboat/structures/Guild.py
+-rw-rw-rw-   0        0        0      694 2023-07-01 14:56:59.000000 unbelievaboat-1.0.3/unbelievaboat/structures/Leaderboard.py
+-rw-rw-rw-   0        0        0      929 2023-07-01 14:38:30.000000 unbelievaboat-1.0.3/unbelievaboat/structures/Permission.py
+-rw-rw-rw-   0        0        0      650 2023-07-01 15:01:25.000000 unbelievaboat-1.0.3/unbelievaboat/structures/Store.py
+-rw-rw-rw-   0        0        0      601 2023-07-01 14:12:42.000000 unbelievaboat-1.0.3/unbelievaboat/structures/User.py
+-rw-rw-rw-   0        0        0      362 2023-07-01 14:56:55.000000 unbelievaboat-1.0.3/unbelievaboat/structures/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 16:03:11.468279 unbelievaboat-1.0.3/unbelievaboat/structures/items/
+-rw-rw-rw-   0        0        0     1272 2023-07-01 14:50:40.000000 unbelievaboat-1.0.3/unbelievaboat/structures/items/BaseItem.py
+-rw-rw-rw-   0        0        0      387 2023-07-01 14:50:40.000000 unbelievaboat-1.0.3/unbelievaboat/structures/items/InventoryItem.py
+-rw-rw-rw-   0        0        0      966 2023-07-01 14:50:40.000000 unbelievaboat-1.0.3/unbelievaboat/structures/items/StoreItem.py
+-rw-rw-rw-   0        0        0     1009 2023-07-01 14:50:40.000000 unbelievaboat-1.0.3/unbelievaboat/structures/items/StoreItemAction.py
+-rw-rw-rw-   0        0        0     1275 2023-07-01 14:50:40.000000 unbelievaboat-1.0.3/unbelievaboat/structures/items/StoreItemRequirement.py
+-rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.0.3/unbelievaboat/structures/items/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 16:03:11.473280 unbelievaboat-1.0.3/unbelievaboat/util/
+-rw-rw-rw-   0        0        0     1143 2023-07-01 11:45:16.000000 unbelievaboat-1.0.3/unbelievaboat/util/Bucket.py
+-rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.0.3/unbelievaboat/util/Constants.py
+-rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.0.3/unbelievaboat/util/SnakeCaseConventer.py
+-rw-rw-rw-   0        0        0      250 2023-07-01 13:41:07.000000 unbelievaboat-1.0.3/unbelievaboat/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 16:03:11.448720 unbelievaboat-1.0.3/unbelievaboat.egg-info/
+-rw-rw-rw-   0        0        0     3159 2023-07-01 16:03:11.000000 unbelievaboat-1.0.3/unbelievaboat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1025 2023-07-01 16:03:11.000000 unbelievaboat-1.0.3/unbelievaboat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 16:03:11.000000 unbelievaboat-1.0.3/unbelievaboat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-01 16:03:11.000000 unbelievaboat-1.0.3/unbelievaboat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-01 16:03:11.000000 unbelievaboat-1.0.3/unbelievaboat.egg-info/top_level.txt
```

### Comparing `unbelievaboat-1.0.2/LICENSE` & `unbelievaboat-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.2/PKG-INFO` & `unbelievaboat-1.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbelievaboat
-Version: 1.0.2
+Version: 1.0.3
 Summary: Wrapper for UnbelievaBoat API.
 Home-page: https://github.com/yoggys/unbelievaboat
 Author: yoggys
 Author-email: yoggies@yoggies.ovh
 Keywords: python,unb,unbelievaboat,api,wrapper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -15,15 +15,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # UnbelievaBoat API Python Wrapper
 
-[![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
+[![Discord Server](https://img.shields.io/discord/746360067632136222?label=discord&style=for-the-badge&logo=discord&color=5865F2&logoColor=white)](https://discord.gg/yoggies)
+[![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/downloads/release/python-380/)
+[![PyPI Version](https://img.shields.io/pypi/v/unbelievaboat.svg?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/unbelievaboat/)
+
 
 This is a Python wrapper for the UnbelievaBoat API, which provides access to the UnbelievaBoat Discord bot functionality. It allows you to interact with the API endpoints to retrieve guild information, user balances, leaderboard data, and more.
 
 ## Requirements
 
 - Python 3.8 or higher
```

### Comparing `unbelievaboat-1.0.2/README.md` & `unbelievaboat-1.0.3/unbelievaboat.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,79 @@
-# UnbelievaBoat API Python Wrapper
-
-[![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
-
-This is a Python wrapper for the UnbelievaBoat API, which provides access to the UnbelievaBoat Discord bot functionality. It allows you to interact with the API endpoints to retrieve guild information, user balances, leaderboard data, and more.
-
-## Requirements
-
-- Python 3.8 or higher
-
-## Installation
-
-You can install the UnbelievaBoat API Python wrapper using pip. Open your terminal and run the following command:
-
-```shell
-pip install unbelievaboat
-```
-
-## Usage
-
-Here's an example of how to use the UnbelievaBoat API Python wrapper to interact with the UnbelievaBoat API:
-
-```python
-from unbelievaboat import Client
-import asyncio
-
-
-async def main():
-    # Initialize the client with your API token
-    client = Client("your-api-token")
-
-    # Retrieve guild information
-    guild = await client.get_guild(guild_id)
-    print(guild)
-
-    # Retrieve user balance
-    user_balance = await client.get_user_balance(guild_id, user_id)
-    print(user_balance)
-
-    # Close the client session
-    await client.close()
-
-
-asyncio.run(main())
-```
-
-Replace `"your-api-token"` with your actual API token. You can obtain an API token by logging into the UnbelievaBoat dashboard and generating a token for your bot.
-
-Please note that the above example demonstrates a basic usage scenario. You can explore other available methods in the `Client` class to interact with different API endpoints. You can also find more examples in the [examples](https://github.com/yoggys/unbelievaboat/tree/main/examples) directory.
-
-## Contributing
-
-Contributions are welcome! If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/yoggys/unbelievaboat).
-
-## License
-
-This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
+Metadata-Version: 2.1
+Name: unbelievaboat
+Version: 1.0.3
+Summary: Wrapper for UnbelievaBoat API.
+Home-page: https://github.com/yoggys/unbelievaboat
+Author: yoggys
+Author-email: yoggies@yoggies.ovh
+Keywords: python,unb,unbelievaboat,api,wrapper
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# UnbelievaBoat API Python Wrapper
+
+[![Discord Server](https://img.shields.io/discord/746360067632136222?label=discord&style=for-the-badge&logo=discord&color=5865F2&logoColor=white)](https://discord.gg/yoggies)
+[![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/downloads/release/python-380/)
+[![PyPI Version](https://img.shields.io/pypi/v/unbelievaboat.svg?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/unbelievaboat/)
+
+
+This is a Python wrapper for the UnbelievaBoat API, which provides access to the UnbelievaBoat Discord bot functionality. It allows you to interact with the API endpoints to retrieve guild information, user balances, leaderboard data, and more.
+
+## Requirements
+
+- Python 3.8 or higher
+
+## Installation
+
+You can install the UnbelievaBoat API Python wrapper using pip. Open your terminal and run the following command:
+
+```shell
+pip install unbelievaboat
+```
+
+## Usage
+
+Here's an example of how to use the UnbelievaBoat API Python wrapper to interact with the UnbelievaBoat API:
+
+```python
+from unbelievaboat import Client
+import asyncio
+
+
+async def main():
+    # Initialize the client with your API token
+    client = Client("your-api-token")
+
+    # Retrieve guild information
+    guild = await client.get_guild(guild_id)
+    print(guild)
+
+    # Retrieve user balance
+    user_balance = await client.get_user_balance(guild_id, user_id)
+    print(user_balance)
+
+    # Close the client session
+    await client.close()
+
+
+asyncio.run(main())
+```
+
+Replace `"your-api-token"` with your actual API token. You can obtain an API token by logging into the UnbelievaBoat dashboard and generating a token for your bot.
+
+Please note that the above example demonstrates a basic usage scenario. You can explore other available methods in the `Client` class to interact with different API endpoints. You can also find more examples in the [examples](https://github.com/yoggys/unbelievaboat/tree/main/examples) directory.
+
+## Contributing
+
+Contributions are welcome! If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/yoggys/unbelievaboat).
+
+## License
+
+This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `unbelievaboat-1.0.2/setup.py` & `unbelievaboat-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 cwd = Path(__file__).parent
 long_description = (cwd / "README.md").read_text()
 
 setup(
     name="unbelievaboat",
-    version="1.0.2",
+    version="1.0.3",
     author="yoggys",
     author_email="yoggies@yoggies.ovh",
     description="Wrapper for UnbelievaBoat API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yoggys/unbelievaboat",
     packages=find_packages(),
```

### Comparing `unbelievaboat-1.0.2/unbelievaboat/Client.py` & `unbelievaboat-1.0.3/unbelievaboat/Client.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.2/unbelievaboat/RequestHandler.py` & `unbelievaboat-1.0.3/unbelievaboat/RequestHandler.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.2/unbelievaboat/errors/APIError.py` & `unbelievaboat-1.0.3/unbelievaboat/errors/APIError.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.2/unbelievaboat/errors/HTTPError.py` & `unbelievaboat-1.0.3/unbelievaboat/errors/HTTPError.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.2/unbelievaboat/structures/Guild.py` & `unbelievaboat-1.0.3/unbelievaboat/structures/Guild.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.2/unbelievaboat/structures/Leaderboard.py` & `unbelievaboat-1.0.3/unbelievaboat/structures/Leaderboard.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.2/unbelievaboat/structures/Permission.py` & `unbelievaboat-1.0.3/unbelievaboat/structures/Permission.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.2/unbelievaboat/structures/Store.py` & `unbelievaboat-1.0.3/unbelievaboat/structures/Store.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.2/unbelievaboat/structures/User.py` & `unbelievaboat-1.0.3/unbelievaboat/structures/User.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.2/unbelievaboat/structures/items/BaseItem.py` & `unbelievaboat-1.0.3/unbelievaboat/structures/items/BaseItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.2/unbelievaboat/structures/items/StoreItem.py` & `unbelievaboat-1.0.3/unbelievaboat/structures/items/StoreItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.2/unbelievaboat/structures/items/StoreItemAction.py` & `unbelievaboat-1.0.3/unbelievaboat/structures/items/StoreItemAction.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.2/unbelievaboat/structures/items/StoreItemRequirement.py` & `unbelievaboat-1.0.3/unbelievaboat/structures/items/StoreItemRequirement.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.2/unbelievaboat/util/Bucket.py` & `unbelievaboat-1.0.3/unbelievaboat/util/Bucket.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.2/unbelievaboat/util/SnakeCaseConventer.py` & `unbelievaboat-1.0.3/unbelievaboat/util/SnakeCaseConventer.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.2/unbelievaboat.egg-info/PKG-INFO` & `unbelievaboat-1.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,13 @@
-Metadata-Version: 2.1
-Name: unbelievaboat
-Version: 1.0.2
-Summary: Wrapper for UnbelievaBoat API.
-Home-page: https://github.com/yoggys/unbelievaboat
-Author: yoggys
-Author-email: yoggies@yoggies.ovh
-Keywords: python,unb,unbelievaboat,api,wrapper
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # UnbelievaBoat API Python Wrapper
 
-[![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
+[![Discord Server](https://img.shields.io/discord/746360067632136222?label=discord&style=for-the-badge&logo=discord&color=5865F2&logoColor=white)](https://discord.gg/yoggies)
+[![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/downloads/release/python-380/)
+[![PyPI Version](https://img.shields.io/pypi/v/unbelievaboat.svg?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/unbelievaboat/)
+
 
 This is a Python wrapper for the UnbelievaBoat API, which provides access to the UnbelievaBoat Discord bot functionality. It allows you to interact with the API endpoints to retrieve guild information, user balances, leaderboard data, and more.
 
 ## Requirements
 
 - Python 3.8 or higher
```

### Comparing `unbelievaboat-1.0.2/unbelievaboat.egg-info/SOURCES.txt` & `unbelievaboat-1.0.3/unbelievaboat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

