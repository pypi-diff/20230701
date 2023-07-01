# Comparing `tmp/unbelievaboat-1.0.3.tar.gz` & `tmp/unbelievaboat-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unbelievaboat-1.0.3.tar", last modified: Sat Jul  1 16:03:11 2023, max compression
+gzip compressed data, was "unbelievaboat-1.0.4.tar", last modified: Sat Jul  1 17:01:40 2023, max compression
```

## Comparing `unbelievaboat-1.0.3.tar` & `unbelievaboat-1.0.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 16:03:11.475788 unbelievaboat-1.0.3/
--rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     3159 2023-07-01 16:03:11.474783 unbelievaboat-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2432 2023-07-01 16:02:14.000000 unbelievaboat-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-01 16:03:11.475788 unbelievaboat-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1064 2023-07-01 16:02:47.000000 unbelievaboat-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 16:03:11.410235 unbelievaboat-1.0.3/unbelievaboat/
--rw-rw-rw-   0        0        0     5396 2023-07-01 14:59:44.000000 unbelievaboat-1.0.3/unbelievaboat/Client.py
--rw-rw-rw-   0        0        0     3133 2023-07-01 14:59:51.000000 unbelievaboat-1.0.3/unbelievaboat/RequestHandler.py
--rw-rw-rw-   0        0        0      336 2023-07-01 14:55:29.000000 unbelievaboat-1.0.3/unbelievaboat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 16:03:11.452526 unbelievaboat-1.0.3/unbelievaboat/errors/
--rw-rw-rw-   0        0        0      572 2023-07-01 11:55:22.000000 unbelievaboat-1.0.3/unbelievaboat/errors/APIError.py
--rw-rw-rw-   0        0        0      551 2023-07-01 13:35:00.000000 unbelievaboat-1.0.3/unbelievaboat/errors/HTTPError.py
--rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.0.3/unbelievaboat/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 16:03:11.460034 unbelievaboat-1.0.3/unbelievaboat/structures/
--rw-rw-rw-   0        0        0      944 2023-07-01 14:37:58.000000 unbelievaboat-1.0.3/unbelievaboat/structures/Guild.py
--rw-rw-rw-   0        0        0      694 2023-07-01 14:56:59.000000 unbelievaboat-1.0.3/unbelievaboat/structures/Leaderboard.py
--rw-rw-rw-   0        0        0      929 2023-07-01 14:38:30.000000 unbelievaboat-1.0.3/unbelievaboat/structures/Permission.py
--rw-rw-rw-   0        0        0      650 2023-07-01 15:01:25.000000 unbelievaboat-1.0.3/unbelievaboat/structures/Store.py
--rw-rw-rw-   0        0        0      601 2023-07-01 14:12:42.000000 unbelievaboat-1.0.3/unbelievaboat/structures/User.py
--rw-rw-rw-   0        0        0      362 2023-07-01 14:56:55.000000 unbelievaboat-1.0.3/unbelievaboat/structures/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 16:03:11.468279 unbelievaboat-1.0.3/unbelievaboat/structures/items/
--rw-rw-rw-   0        0        0     1272 2023-07-01 14:50:40.000000 unbelievaboat-1.0.3/unbelievaboat/structures/items/BaseItem.py
--rw-rw-rw-   0        0        0      387 2023-07-01 14:50:40.000000 unbelievaboat-1.0.3/unbelievaboat/structures/items/InventoryItem.py
--rw-rw-rw-   0        0        0      966 2023-07-01 14:50:40.000000 unbelievaboat-1.0.3/unbelievaboat/structures/items/StoreItem.py
--rw-rw-rw-   0        0        0     1009 2023-07-01 14:50:40.000000 unbelievaboat-1.0.3/unbelievaboat/structures/items/StoreItemAction.py
--rw-rw-rw-   0        0        0     1275 2023-07-01 14:50:40.000000 unbelievaboat-1.0.3/unbelievaboat/structures/items/StoreItemRequirement.py
--rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.0.3/unbelievaboat/structures/items/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 16:03:11.473280 unbelievaboat-1.0.3/unbelievaboat/util/
--rw-rw-rw-   0        0        0     1143 2023-07-01 11:45:16.000000 unbelievaboat-1.0.3/unbelievaboat/util/Bucket.py
--rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.0.3/unbelievaboat/util/Constants.py
--rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.0.3/unbelievaboat/util/SnakeCaseConventer.py
--rw-rw-rw-   0        0        0      250 2023-07-01 13:41:07.000000 unbelievaboat-1.0.3/unbelievaboat/util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 16:03:11.448720 unbelievaboat-1.0.3/unbelievaboat.egg-info/
--rw-rw-rw-   0        0        0     3159 2023-07-01 16:03:11.000000 unbelievaboat-1.0.3/unbelievaboat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2023-07-01 16:03:11.000000 unbelievaboat-1.0.3/unbelievaboat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 16:03:11.000000 unbelievaboat-1.0.3/unbelievaboat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-01 16:03:11.000000 unbelievaboat-1.0.3/unbelievaboat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-01 16:03:11.000000 unbelievaboat-1.0.3/unbelievaboat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 17:01:40.137675 unbelievaboat-1.0.4/
+-rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3173 2023-07-01 17:01:40.136665 unbelievaboat-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2432 2023-07-01 16:02:14.000000 unbelievaboat-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-01 17:01:40.137675 unbelievaboat-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1084 2023-07-01 17:01:18.000000 unbelievaboat-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 17:01:40.087628 unbelievaboat-1.0.4/unbelievaboat/
+-rw-rw-rw-   0        0        0     5584 2023-07-01 16:55:18.000000 unbelievaboat-1.0.4/unbelievaboat/Client.py
+-rw-rw-rw-   0        0        0     3133 2023-07-01 14:59:51.000000 unbelievaboat-1.0.4/unbelievaboat/RequestHandler.py
+-rw-rw-rw-   0        0        0      336 2023-07-01 14:55:29.000000 unbelievaboat-1.0.4/unbelievaboat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 17:01:40.113710 unbelievaboat-1.0.4/unbelievaboat/errors/
+-rw-rw-rw-   0        0        0      572 2023-07-01 11:55:22.000000 unbelievaboat-1.0.4/unbelievaboat/errors/APIError.py
+-rw-rw-rw-   0        0        0      551 2023-07-01 13:35:00.000000 unbelievaboat-1.0.4/unbelievaboat/errors/HTTPError.py
+-rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.0.4/unbelievaboat/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 17:01:40.120417 unbelievaboat-1.0.4/unbelievaboat/structures/
+-rw-rw-rw-   0        0        0      925 2023-07-01 16:58:46.000000 unbelievaboat-1.0.4/unbelievaboat/structures/Guild.py
+-rw-rw-rw-   0        0        0      728 2023-07-01 16:59:19.000000 unbelievaboat-1.0.4/unbelievaboat/structures/Leaderboard.py
+-rw-rw-rw-   0        0        0      929 2023-07-01 16:45:44.000000 unbelievaboat-1.0.4/unbelievaboat/structures/Permission.py
+-rw-rw-rw-   0        0        0      704 2023-07-01 16:45:44.000000 unbelievaboat-1.0.4/unbelievaboat/structures/Store.py
+-rw-rw-rw-   0        0        0     1240 2023-07-01 17:00:44.000000 unbelievaboat-1.0.4/unbelievaboat/structures/User.py
+-rw-rw-rw-   0        0        0      362 2023-07-01 14:56:55.000000 unbelievaboat-1.0.4/unbelievaboat/structures/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 17:01:40.129288 unbelievaboat-1.0.4/unbelievaboat/structures/items/
+-rw-rw-rw-   0        0        0     1293 2023-07-01 16:54:27.000000 unbelievaboat-1.0.4/unbelievaboat/structures/items/BaseItem.py
+-rw-rw-rw-   0        0        0      429 2023-07-01 16:54:36.000000 unbelievaboat-1.0.4/unbelievaboat/structures/items/InventoryItem.py
+-rw-rw-rw-   0        0        0     1353 2023-07-01 16:57:10.000000 unbelievaboat-1.0.4/unbelievaboat/structures/items/StoreItem.py
+-rw-rw-rw-   0        0        0     1030 2023-07-01 16:54:52.000000 unbelievaboat-1.0.4/unbelievaboat/structures/items/StoreItemAction.py
+-rw-rw-rw-   0        0        0     1296 2023-07-01 16:55:37.000000 unbelievaboat-1.0.4/unbelievaboat/structures/items/StoreItemRequirement.py
+-rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.0.4/unbelievaboat/structures/items/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 17:01:40.134537 unbelievaboat-1.0.4/unbelievaboat/util/
+-rw-rw-rw-   0        0        0     1143 2023-07-01 11:45:16.000000 unbelievaboat-1.0.4/unbelievaboat/util/Bucket.py
+-rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.0.4/unbelievaboat/util/Constants.py
+-rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.0.4/unbelievaboat/util/SnakeCaseConventer.py
+-rw-rw-rw-   0        0        0      250 2023-07-01 13:41:07.000000 unbelievaboat-1.0.4/unbelievaboat/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 17:01:40.109640 unbelievaboat-1.0.4/unbelievaboat.egg-info/
+-rw-rw-rw-   0        0        0     3173 2023-07-01 17:01:39.000000 unbelievaboat-1.0.4/unbelievaboat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1025 2023-07-01 17:01:40.000000 unbelievaboat-1.0.4/unbelievaboat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 17:01:39.000000 unbelievaboat-1.0.4/unbelievaboat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-01 17:01:39.000000 unbelievaboat-1.0.4/unbelievaboat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-01 17:01:39.000000 unbelievaboat-1.0.4/unbelievaboat.egg-info/top_level.txt
```

### Comparing `unbelievaboat-1.0.3/LICENSE` & `unbelievaboat-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.3/PKG-INFO` & `unbelievaboat-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: unbelievaboat
-Version: 1.0.3
+Version: 1.0.4
 Summary: Wrapper for UnbelievaBoat API.
 Home-page: https://github.com/yoggys/unbelievaboat
 Author: yoggys
 Author-email: yoggies@yoggies.ovh
-Keywords: python,unb,unbelievaboat,api,wrapper
+Keywords: python,unb,unbelievaboat,api,wrapper,async,asyncio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `unbelievaboat-1.0.3/README.md` & `unbelievaboat-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.3/setup.py` & `unbelievaboat-1.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 cwd = Path(__file__).parent
 long_description = (cwd / "README.md").read_text()
 
 setup(
     name="unbelievaboat",
-    version="1.0.3",
+    version="1.0.4",
     author="yoggys",
     author_email="yoggies@yoggies.ovh",
     description="Wrapper for UnbelievaBoat API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yoggys/unbelievaboat",
     packages=find_packages(),
@@ -24,9 +24,9 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
-    keywords=["python", "unb", "unbelievaboat", "api", "wrapper"],
+    keywords=["python", "unb", "unbelievaboat", "api", "wrapper", "async", "asyncio"],
 )
```

### Comparing `unbelievaboat-1.0.3/unbelievaboat/Client.py` & `unbelievaboat-1.0.4/unbelievaboat/Client.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,43 +45,46 @@
         ) as response:
             response.raise_for_status()
             return await response.json()
 
     async def get_user_balance(self, guild_id: int, user_id: int) -> User:
         endpoint: str = f"guilds/{guild_id}/users/{user_id}"
         data: Dict[str, Any] = await self._request_handler.request("GET", endpoint)
-        return User(data)
+        data["guild_id"] = guild_id
+        return User(self, data)
 
     async def set_user_balance(
         self, guild_id: int, user_id: int, data: Dict[str, Any] = {}, reason: str = None
     ) -> User:
         endpoint: str = f"guilds/{guild_id}/users/{user_id}"
         payload: Dict[str, Any] = {
             "cash": data.get("cash"),
             "bank": data.get("bank"),
             "reason": reason,
         }
         data: Dict[str, Any] = await self._request_handler.request(
             "PUT", endpoint, data=payload
         )
-        return User(data)
+        data["guild_id"] = guild_id
+        return User(self, data)
 
     async def edit_user_balance(
         self, guild_id: int, user_id: int, data: Dict[str, Any] = {}, reason: str = None
     ) -> User:
         endpoint: str = f"guilds/{guild_id}/users/{user_id}"
         payload: Dict[str, Any] = {
             "cash": data.get("cash"),
             "bank": data.get("bank"),
             "reason": reason,
         }
         data: Dict[str, Any] = await self._request_handler.request(
             "PATCH", endpoint, data=payload
         )
-        return User(data)
+        data["guild_id"] = guild_id
+        return User(self, data)
 
     async def get_guild_leaderboard(
         self, guild_id: int, params: Dict[str, Any] = {}
     ) -> Dict[str, Union[List[User], int]]:
         endpoint: str = f"guilds/{guild_id}/users"
         data: Dict[str, Any] = await self._request_handler.request(
             "GET", endpoint, params=params
@@ -104,43 +107,43 @@
         return Guild(data)
 
     async def get_application_permission(self, guild_id: int) -> Permission:
         endpoint: str = f"applications/@me/guilds/{guild_id}"
         data: Dict[str, Any] = await self._request_handler.request("GET", endpoint)
         return Permission(data["permissions"])
 
-    async def get_items(
-        self, guild_id: int, params: Dict[str, Any] = None
-    ) -> Dict[str, Union[int, List[StoreItem]]]:
+    async def get_items(self, guild_id: int, params: Dict[str, Any] = None) -> Store:
         endpoint: str = f"guilds/{guild_id}/items"
         data: Dict[str, Any] = await self._request_handler.request(
             "GET", endpoint, params=params
         )
 
         return Store(
+            self,
             {
                 "guild_id": guild_id,
                 "page": data["page"],
                 "totalPages": data["total_pages"],
                 "items": data["items"],
-            }
+            },
         )
 
     async def get_item(self, guild_id: int, item_id: int) -> StoreItem:
         endpoint: str = f"guilds/{guild_id}/items/{item_id}"
         data: Dict[str, Any] = await self._request_handler.request("GET", endpoint)
-        return StoreItem(data)
+        data["guild_id"] = guild_id
+        return StoreItem(self, data)
 
     async def edit_item(
         self,
         guild_id: int,
         item_id: int,
         data: Dict[str, Any],
         params: Dict[str, Any] = None,
     ) -> StoreItem:
         endpoint: str = f"guilds/{guild_id}/items/{item_id}"
         payload: Dict[str, Any] = to_snake_case_deep(data)
         response: Dict[str, Any] = await self._request_handler.request(
             "PATCH", endpoint, data=payload, params=params
         )
-
-        return StoreItem(response)
+        response["guild_id"] = guild_id
+        return StoreItem(self, response)
```

### Comparing `unbelievaboat-1.0.3/unbelievaboat/RequestHandler.py` & `unbelievaboat-1.0.4/unbelievaboat/RequestHandler.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.3/unbelievaboat/errors/APIError.py` & `unbelievaboat-1.0.4/unbelievaboat/errors/APIError.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.3/unbelievaboat/errors/HTTPError.py` & `unbelievaboat-1.0.4/unbelievaboat/errors/HTTPError.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.3/unbelievaboat/structures/Guild.py` & `unbelievaboat-1.0.4/unbelievaboat/structures/Guild.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from typing import Optional
+from typing import Any, Dict, Optional
 
 
 class Guild:
-    def __init__(self, data: dict = {}) -> None:
-        self.id: Optional[str] = data.get("id")
-        self.name: Optional[str] = data.get("name")
+    def __init__(self, data: Dict[str, Any] = {}) -> None:
+        self.id: str = data.get("id")
+        self.name: str = data.get("name")
         self.icon: Optional[str] = data.get("icon")
-        self.owner_id: Optional[str] = data.get("owner_id")
-        self.member_count: Optional[int] = data.get("member_count")
-        self.currency_symbol: Optional[str] = data.get("symbol")
-        self._raw_data: dict = data
+        self.owner_id: str = data.get("owner_id")
+        self.member_count: int = data.get("member_count")
+        self.currency_symbol: str = data.get("symbol")
+        self._raw_data: Dict[str, Any] = data
+
+    def __str__(self) -> str:
+        return "<Guild id={} name='{}' owner_id={} member_count={}>".format(
+            self.owner_id, self.name, self.owner_id, self.member_count
+        )
 
     @property
     def icon_url(self) -> Optional[str]:
         if self.icon:
             extension = "gif" if self.icon.startswith("a_") else "png"
             return f"https://cdn.discordapp.com/icons/{self.id}/{self.icon}.{extension}"
         return None
-
-    def __str__(self) -> str:
-        return "<Guild id={} name='{}' owner_id={} member_count={}>".format(
-            self.owner_id, self.name, self.owner_id, self.member_count
-        )
```

### Comparing `unbelievaboat-1.0.3/unbelievaboat/structures/Leaderboard.py` & `unbelievaboat-1.0.4/unbelievaboat/structures/Leaderboard.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from typing import List, Optional
+from typing import Any, Dict, List
 
 from .User import User
 
 
 class Leaderboard:
-    def __init__(self, data: dict = {}) -> None:
-        self.guild_id: Optional[str] = data.get("guild_id")
-        self.users: Optional[List[User]] = [
-            User(user) for user in data.get("users", [])
+    def __init__(self, client, data: Dict[str, Any] = {}) -> None:
+        self.guild_id: str = data.get("guild_id")
+        self.users: List[User] = [
+            User(client, {**user, "guild_id": self.guild_id})
+            for user in data.get("users", [])
         ]
-        self.total_pages: Optional[int] = data.get("total_pages")
-        self.page: Optional[int] = data.get("page", 1)
+        self.total_pages: int = data.get("total_pages", 1)
+        self.page: int = data.get("page", 1)
 
     def __str__(self) -> str:
         return "<Leaderboard guild_id={} users={} total_pages={} page={}>".format(
             self.guild_id,
             [str(user) for user in self.users],
             self.total_pages,
             self.page,
```

### Comparing `unbelievaboat-1.0.3/unbelievaboat/structures/Permission.py` & `unbelievaboat-1.0.4/unbelievaboat/structures/Permission.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 
 class Permission:
     economy: int = 1
 
     def __init__(self, allow: int) -> None:
         self.allow: int = allow
 
+    def __str__(self) -> str:
+        return "<Permission allow={}>".format(self.allow)
+
     @property
     def json(self) -> Dict[str, bool]:
         json: Dict[str, bool] = {}
         for permission in vars(self.__class__).keys():
             if not permission.startswith("__"):
                 json[permission] = bool(
                     self.allow & getattr(self.__class__, permission)
@@ -20,10 +23,7 @@
     def has(self, permissions: Union[str, list[str]]) -> bool:
         if isinstance(permissions, list):
             return all(
                 bool(self.allow & getattr(self.__class__, perm)) for perm in permissions
             )
         else:
             return bool(self.allow & getattr(self.__class__, permissions))
-
-    def __str__(self) -> str:
-        return "<Permission allow={}>".format(self.allow)
```

### Comparing `unbelievaboat-1.0.3/unbelievaboat/structures/Store.py` & `unbelievaboat-1.0.4/unbelievaboat/structures/Store.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from typing import List, Optional
 
 from .items import StoreItem
 
 
 class Store:
-    def __init__(self, data: dict = {}) -> None:
-        self.guild_id: Optional[str] = data.get("guild_id")
-        self.items = [StoreItem(item) for item in data.get("items", [])]
-        self.total_pages: Optional[int] = data.get("total_pages", 1)
-        self.page: Optional[int] = data.get("page", 1)
+    def __init__(self, client, data: dict = {}) -> None:
+        self.guild_id: str = data.get("guild_id")
+        self.items = [
+            StoreItem(client, {**item, "guild_id": self.guild_id})
+            for item in data.get("items", [])
+        ]
+        self.total_pages: int = data.get("total_pages", 1)
+        self.page: int = data.get("page", 1)
 
     def __str__(self) -> str:
         return "<Store guild_id={} items={} total_pages={} page={}>".format(
             self.guild_id,
             [str(item) for item in self.items],
             self.total_pages,
             self.page,
```

### Comparing `unbelievaboat-1.0.3/unbelievaboat/structures/items/BaseItem.py` & `unbelievaboat-1.0.4/unbelievaboat/structures/items/BaseItem.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import List, Optional
+from typing import Any, Dict, List, Optional
 
 from .StoreItemAction import StoreItemAction
 from .StoreItemRequirement import StoreItemRequirement
 
 
 class BaseItem:
-    def __init__(self, data: dict) -> None:
+    def __init__(self, data: Dict[str, Any]) -> None:
         self.name: str = data["name"]
         self.description: Optional[str] = data.get("description", None)
         self.is_usable: bool = data["is_usable"]
         self.is_sellable: bool = data["is_sellable"]
         self.requirements: List[StoreItemRequirement] = [
             StoreItemRequirement(requirement) for requirement in data["requirements"]
         ]
```

### Comparing `unbelievaboat-1.0.3/unbelievaboat/structures/items/StoreItem.py` & `unbelievaboat-1.0.4/unbelievaboat/structures/items/StoreItem.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 from datetime import datetime
+from typing import Any, Dict, Self
 
 from .BaseItem import BaseItem
 
 
 class StoreItem(BaseItem):
-    def __init__(self, data: dict) -> None:
+    def __init__(self, client, data: Dict[str, Any]) -> None:
         super().__init__(data)
+        self.guild_id: str = data["guild_id"]
         self.id: str = data["id"]
         self.price: int = int(data["price"])
         self.is_inventory: bool = data["is_inventory"]
         self.stock_remaining: int = data["stock_remaining"]
         self.unlimited_stock: bool = data["unlimited_stock"]
         self.expires_at: datetime = (
             datetime.strptime(data["expires_at"], "%Y-%m-%dT%H:%M:%S.%fZ")
             if data.get("expires_at")
             else None
         )
 
+        self._client = client
+
     def __str__(self) -> str:
-        return "<StoreItem id={} price={} is_inventory={} stock_remaining={} unlimited_stock={} expires_at={}>".format(
+        return "<StoreItem id={} guild_id={} price={} is_inventory={} stock_remaining={} unlimited_stock={} expires_at={}>".format(
             self.id,
+            self.guild_id,
             self.price,
             self.is_inventory,
             self.stock_remaining,
             self.unlimited_stock,
             self.expires_at,
         )
+
+    async def edit(
+        self, data: Dict[str, Any] = {}, params: Dict[str, Any] = {}
+    ) -> Self:
+        self = await self._client.edit_item(self.guild_id, self.id, data, params)
+        return self
```

### Comparing `unbelievaboat-1.0.3/unbelievaboat/structures/items/StoreItemAction.py` & `unbelievaboat-1.0.4/unbelievaboat/structures/items/StoreItemAction.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import List, Optional
+from typing import Any, Dict, List, Optional
 
 from ...util.Constants import ItemActionType
 
 
 class StoreItemAction:
-    def __init__(self, data: dict) -> None:
+    def __init__(self, data: Dict[str, Any]) -> None:
         self.type: ItemActionType = ItemActionType(data["type"])
 
         if self.type == ItemActionType.RESPOND:
             self.message: str = data["message"]
         elif self.type in [
             ItemActionType.ADD_ROLES,
             ItemActionType.ADD_ITEMS,
```

### Comparing `unbelievaboat-1.0.3/unbelievaboat/structures/items/StoreItemRequirement.py` & `unbelievaboat-1.0.4/unbelievaboat/structures/items/StoreItemRequirement.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import List, Optional
+from typing import Any, Dict, List, Optional
 
 from ...util.Constants import ItemRequirementMatchType, ItemRequirementType
 
 
 class StoreItemRequirement:
-    def __init__(self, data: dict) -> None:
+    def __init__(self, data: Dict[str, Any]) -> None:
         self.type: ItemRequirementType = ItemRequirementType(data["type"])
 
         if self.type in [ItemRequirementType.ROLE, ItemRequirementType.ITEM]:
             self.matchType: ItemRequirementMatchType = ItemRequirementMatchType(
                 data["match_type"]
             )
             self.ids: List[str] = data.get("ids", [])
```

### Comparing `unbelievaboat-1.0.3/unbelievaboat/util/Bucket.py` & `unbelievaboat-1.0.4/unbelievaboat/util/Bucket.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.3/unbelievaboat/util/SnakeCaseConventer.py` & `unbelievaboat-1.0.4/unbelievaboat/util/SnakeCaseConventer.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.3/unbelievaboat.egg-info/PKG-INFO` & `unbelievaboat-1.0.4/unbelievaboat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: unbelievaboat
-Version: 1.0.3
+Version: 1.0.4
 Summary: Wrapper for UnbelievaBoat API.
 Home-page: https://github.com/yoggys/unbelievaboat
 Author: yoggys
 Author-email: yoggies@yoggies.ovh
-Keywords: python,unb,unbelievaboat,api,wrapper
+Keywords: python,unb,unbelievaboat,api,wrapper,async,asyncio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `unbelievaboat-1.0.3/unbelievaboat.egg-info/SOURCES.txt` & `unbelievaboat-1.0.4/unbelievaboat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

