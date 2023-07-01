# Comparing `tmp/cy_account-0.1.6.tar.gz` & `tmp/cy_account-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cy_account-0.1.6.tar", last modified: Sat Jul  1 03:33:02 2023, max compression
+gzip compressed data, was "cy_account-0.1.7.tar", last modified: Sat Jul  1 15:15:25 2023, max compression
```

## Comparing `cy_account-0.1.6.tar` & `cy_account-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 03:33:02.989967 cy_account-0.1.6/
--rw-rw-rw-   0        0        0      303 2023-07-01 03:33:02.987958 cy_account-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-26 16:03:11.000000 cy_account-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 03:33:02.945964 cy_account-0.1.6/cy_account/
--rw-rw-rw-   0        0        0     7191 2023-07-01 03:32:04.000000 cy_account-0.1.6/cy_account/__init__.py
--rw-rw-rw-   0        0        0      389 2023-06-26 16:40:06.000000 cy_account-0.1.6/cy_account/test.py
-drwxrwxrwx   0        0        0        0 2023-07-01 03:33:02.985964 cy_account-0.1.6/cy_account.egg-info/
--rw-rw-rw-   0        0        0      303 2023-07-01 03:33:02.000000 cy_account-0.1.6/cy_account.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-07-01 03:33:02.000000 cy_account-0.1.6/cy_account.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 03:33:02.000000 cy_account-0.1.6/cy_account.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-01 03:33:02.000000 cy_account-0.1.6/cy_account.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-01 03:33:02.000000 cy_account-0.1.6/cy_account.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 03:33:02.989967 cy_account-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      581 2023-07-01 03:32:47.000000 cy_account-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:15:25.777150 cy_account-0.1.7/
+-rw-rw-rw-   0        0        0      303 2023-07-01 15:15:25.776149 cy_account-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-07-01 03:33:37.000000 cy_account-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 15:15:25.749147 cy_account-0.1.7/cy_account/
+-rw-rw-rw-   0        0        0     7359 2023-07-01 15:14:49.000000 cy_account-0.1.7/cy_account/__init__.py
+-rw-rw-rw-   0        0        0      389 2023-06-26 16:40:06.000000 cy_account-0.1.7/cy_account/test.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:15:25.774148 cy_account-0.1.7/cy_account.egg-info/
+-rw-rw-rw-   0        0        0      303 2023-07-01 15:15:25.000000 cy_account-0.1.7/cy_account.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-07-01 15:15:25.000000 cy_account-0.1.7/cy_account.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 15:15:25.000000 cy_account-0.1.7/cy_account.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-01 15:15:25.000000 cy_account-0.1.7/cy_account.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-01 15:15:25.000000 cy_account-0.1.7/cy_account.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 15:15:25.777150 cy_account-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-07-01 15:15:14.000000 cy_account-0.1.7/setup.py
```

### Comparing `cy_account-0.1.6/cy_account/__init__.py` & `cy_account-0.1.7/cy_account/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 __all__ = ["UserInfo", "AccountAPI", "ServerForRequest"]
 
+import traceback
 from typing import Optional
 from pydantic import BaseModel, ValidationError
 
 import json
 import requests
 import redis as redis
 from fastapi import HTTPException
@@ -43,34 +44,42 @@
         self.app_id = app_id
         self.serverForRequest = ServerForRequest(app_id=app_id)
 
     def get_user(self, token, auto_error=True):
         """
         通过token获取用户信息得到的数据是自己的数据，比较详细
         """
-        user = self.__get_user_by_token(token)
+        try:
+            user = self.__get_user_by_token(token)
 
-        # if not uid and auto_error:
-        #     raise HTTPException(status_code=401, detail="请登录")
-        #
-        # user = self.__get_user_for_cache(user_id=uid)
-
-        if not user and auto_error:
-            raise HTTPException(status_code=401, detail="无效的用户")
+            if not user and auto_error:
+                raise HTTPException(status_code=401, detail="无效的用户")
 
-        return user
+            return user
+        except:
+            traceback.print_exc()
+            return None
 
     def get_user_by_id(self, user_id, auto_error=True, has_detail=False):
         """
        通过user_id获取用户信息得到的数据是别人的数据，要去除一部分数据
        """
-        user = self.__get_user_for_cache(user_id=user_id)
+        try:
+            user = self.__get_user_for_cache(user_id=user_id)
+        except:
+            if not auto_error:
+                return None
+            else:
+                user = None
 
-        if not user and auto_error:
-            raise HTTPException(status_code=400, detail="用户不存在")
+        if not user:
+            if auto_error:
+                raise HTTPException(status_code=400, detail="用户不存在")
+            else:
+                return None
 
         if not has_detail:
             user.is_vip = None
             user.vip_level = None
             user.vip_end_time = None
             user.points = None
             user.phone = None
@@ -88,15 +97,15 @@
     def get_user_no_error(self, user_id=0, token=None):
         """
         不抛出异常的情况下返回用户信息
         """
         if user_id:
             return self.get_user_by_id(user_id, auto_error=False)
         if token:
-            return self.get_user(token=token)
+            return self.get_user(token=token, auto_error=False)
         return None
 
     def send_phone_code(self, phone):
         r = self.serverForRequest.post(self.account_api_server, path='/api/v1/users/code', query={'phone': phone})
         return r
 
     def login_by_code(self, phone, code):
@@ -133,16 +142,14 @@
             # 接口获取
             user = self.__get_user_info(user_id)
         #
         # if user.status == 2:
         #     raise HTTPException(status_code=402, detail="账号已被冻结")
         return user
 
-
-
     def __get_user_by_token(self, token) -> UserInfo | None:
         if not token:
             return None
         user = self.serverForRequest.get(self.account_api_server, f"api/v1/users/token/{token}")
         if not user:
             return None
         return UserInfo(**user)
```

### Comparing `cy_account-0.1.6/setup.py` & `cy_account-0.1.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="cy_account",
-    version="0.1.6",
+    version="0.1.7",
     author="luyuan",
     author_email="136735431@qq.com",
     description="edited by myself",
     py_modules=["cy_account"],
     classifiers=["Programming Language :: Python :: 3",
                  "License :: OSI Approved :: MIT License",
                  "Operating System :: OS Independent"],
```

