# Comparing `tmp/cy_account-0.1.5.tar.gz` & `tmp/cy_account-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cy_account-0.1.5.tar", last modified: Mon Jun 26 16:40:28 2023, max compression
+gzip compressed data, was "cy_account-0.1.6.tar", last modified: Sat Jul  1 03:33:02 2023, max compression
```

## Comparing `cy_account-0.1.5.tar` & `cy_account-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 16:40:28.805476 cy_account-0.1.5/
--rw-rw-rw-   0        0        0      303 2023-06-26 16:40:28.804485 cy_account-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-26 16:03:11.000000 cy_account-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 16:40:28.780488 cy_account-0.1.5/cy_account/
--rw-rw-rw-   0        0        0     7707 2023-06-26 16:38:41.000000 cy_account-0.1.5/cy_account/__init__.py
--rw-rw-rw-   0        0        0      389 2023-06-26 16:40:06.000000 cy_account-0.1.5/cy_account/test.py
-drwxrwxrwx   0        0        0        0 2023-06-26 16:40:28.803486 cy_account-0.1.5/cy_account.egg-info/
--rw-rw-rw-   0        0        0      303 2023-06-26 16:40:28.000000 cy_account-0.1.5/cy_account.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-06-26 16:40:28.000000 cy_account-0.1.5/cy_account.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 16:40:28.000000 cy_account-0.1.5/cy_account.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-26 16:40:28.000000 cy_account-0.1.5/cy_account.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-26 16:40:28.000000 cy_account-0.1.5/cy_account.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 16:40:28.806484 cy_account-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      581 2023-06-26 16:40:24.000000 cy_account-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 03:33:02.989967 cy_account-0.1.6/
+-rw-rw-rw-   0        0        0      303 2023-07-01 03:33:02.987958 cy_account-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-26 16:03:11.000000 cy_account-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 03:33:02.945964 cy_account-0.1.6/cy_account/
+-rw-rw-rw-   0        0        0     7191 2023-07-01 03:32:04.000000 cy_account-0.1.6/cy_account/__init__.py
+-rw-rw-rw-   0        0        0      389 2023-06-26 16:40:06.000000 cy_account-0.1.6/cy_account/test.py
+drwxrwxrwx   0        0        0        0 2023-07-01 03:33:02.985964 cy_account-0.1.6/cy_account.egg-info/
+-rw-rw-rw-   0        0        0      303 2023-07-01 03:33:02.000000 cy_account-0.1.6/cy_account.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-07-01 03:33:02.000000 cy_account-0.1.6/cy_account.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 03:33:02.000000 cy_account-0.1.6/cy_account.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-01 03:33:02.000000 cy_account-0.1.6/cy_account.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-01 03:33:02.000000 cy_account-0.1.6/cy_account.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 03:33:02.989967 cy_account-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-07-01 03:32:47.000000 cy_account-0.1.6/setup.py
```

### Comparing `cy_account-0.1.5/cy_account/__init__.py` & `cy_account-0.1.6/cy_account/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
         # if not uid and auto_error:
         #     raise HTTPException(status_code=401, detail="请登录")
         #
         # user = self.__get_user_for_cache(user_id=uid)
 
         if not user and auto_error:
-            raise HTTPException(status_code=400, detail="用户不存在")
+            raise HTTPException(status_code=401, detail="无效的用户")
 
         return user
 
     def get_user_by_id(self, user_id, auto_error=True, has_detail=False):
         """
        通过user_id获取用户信息得到的数据是别人的数据，要去除一部分数据
        """
@@ -133,28 +133,15 @@
             # 接口获取
             user = self.__get_user_info(user_id)
         #
         # if user.status == 2:
         #     raise HTTPException(status_code=402, detail="账号已被冻结")
         return user
 
-    #
-    # def __get_user_by_token(self, token):
-    #     if not token:
-    #         return 0
-    #     try:
-    #         # todo 判断 token 是否有效，如无效则调用account账号验证
-    #         payload = jwt.decode(
-    #             token, self.__get_secret_key(settings.APP_ID), algorithms="HS256"
-    #         )
-    #     except (jwt.JWTError, ValidationError):
-    #         traceback.print_exc()
-    #         return 0
-    #     user_id = payload['sub']
-    #     return user_id
+
 
     def __get_user_by_token(self, token) -> UserInfo | None:
         if not token:
             return None
         user = self.serverForRequest.get(self.account_api_server, f"api/v1/users/token/{token}")
         if not user:
             return None
```

### Comparing `cy_account-0.1.5/setup.py` & `cy_account-0.1.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="cy_account",
-    version="0.1.5",
+    version="0.1.6",
     author="luyuan",
     author_email="136735431@qq.com",
     description="edited by myself",
     py_modules=["cy_account"],
     classifiers=["Programming Language :: Python :: 3",
                  "License :: OSI Approved :: MIT License",
                  "Operating System :: OS Independent"],
```

