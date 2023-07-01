# Comparing `tmp/shioajicaller-0.4.1.2.tar.gz` & `tmp/shioajicaller-0.4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shioajicaller-0.4.1.2.tar", max compression
+gzip compressed data, was "shioajicaller-0.4.1.3.tar", max compression
```

## Comparing `shioajicaller-0.4.1.2.tar` & `shioajicaller-0.4.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1074 2021-07-18 10:36:07.309953 shioajicaller-0.4.1.2/LICENSE
--rw-r--r--   0        0        0    21151 2023-04-23 03:55:56.545221 shioajicaller-0.4.1.2/README.md
--rw-r--r--   0        0        0      671 2023-04-23 04:50:16.051088 shioajicaller-0.4.1.2/pyproject.toml
--rw-r--r--   0        0        0       64 2023-01-07 06:34:39.824248 shioajicaller-0.4.1.2/shioajicaller/__init__.py
--rw-r--r--   0        0        0    20163 2023-01-07 06:34:39.824583 shioajicaller-0.4.1.2/shioajicaller/caller.py
--rw-r--r--   0        0        0     5631 2023-04-23 03:50:23.401077 shioajicaller-0.4.1.2/shioajicaller/cli/__init__.py
--rw-r--r--   0        0        0       56 2021-07-22 10:56:11.854486 shioajicaller-0.4.1.2/shioajicaller/codes/__init__.py
--rw-r--r--   0        0        0     7573 2022-10-17 17:45:53.550806 shioajicaller-0.4.1.2/shioajicaller/codes/update.py
--rw-r--r--   0        0        0      636 2023-01-07 06:34:39.825269 shioajicaller-0.4.1.2/shioajicaller/config.py
--rw-r--r--   0        0        0       41 2021-10-04 14:25:31.896900 shioajicaller-0.4.1.2/shioajicaller/server/__init__.py
--rw-r--r--   0        0        0    32589 2023-04-23 04:47:27.727156 shioajicaller-0.4.1.2/shioajicaller/server/websocket.py
--rw-r--r--   0        0        0    23180 1970-01-01 00:00:00.000000 shioajicaller-0.4.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2021-07-18 10:36:07.309953 shioajicaller-0.4.1.3/LICENSE
+-rw-r--r--   0        0        0    21203 2023-07-01 06:40:54.731776 shioajicaller-0.4.1.3/README.md
+-rw-r--r--   0        0        0      671 2023-07-01 06:42:44.180383 shioajicaller-0.4.1.3/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-01-07 06:34:39.824248 shioajicaller-0.4.1.3/shioajicaller/__init__.py
+-rw-r--r--   0        0        0    20163 2023-01-07 06:34:39.824583 shioajicaller-0.4.1.3/shioajicaller/caller.py
+-rw-r--r--   0        0        0     5675 2023-07-01 06:40:54.732245 shioajicaller-0.4.1.3/shioajicaller/cli/__init__.py
+-rw-r--r--   0        0        0       56 2021-07-22 10:56:11.854486 shioajicaller-0.4.1.3/shioajicaller/codes/__init__.py
+-rw-r--r--   0        0        0     7573 2022-10-17 17:45:53.550806 shioajicaller-0.4.1.3/shioajicaller/codes/update.py
+-rw-r--r--   0        0        0      636 2023-01-07 06:34:39.825269 shioajicaller-0.4.1.3/shioajicaller/config.py
+-rw-r--r--   0        0        0       41 2021-10-04 14:25:31.896900 shioajicaller-0.4.1.3/shioajicaller/server/__init__.py
+-rw-r--r--   0        0        0    32589 2023-04-23 04:47:27.727156 shioajicaller-0.4.1.3/shioajicaller/server/websocket.py
+-rw-r--r--   0        0        0    23232 1970-01-01 00:00:00.000000 shioajicaller-0.4.1.3/PKG-INFO
```

### Comparing `shioajicaller-0.4.1.2/LICENSE` & `shioajicaller-0.4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.1.2/README.md` & `shioajicaller-0.4.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -173,31 +173,31 @@
   sdpower/shioaji_caller websockets -wm -ps 250
 ```
 
 ## 範例Example
 這裡說明範例，參數避免暴露請自行建立.env檔案就可以不用給帳號密碼參數。
 
 ```
-USER_ID=YOUID
-USER_PASSWORD=YOU_PASSWORD
+API_KEY= YOU_API_KEY
+SECRET_KEY= YOU_SECRET_KEY
 ```
 ### 執行範例
 ```
 $ python main.py update --help
-$ python main.py update -u YOUID -p YOU_PASSWORD
+$ python main.py update -api YOU_API_KEY -secret YOU_SECRET_KEY
 ```
 ### 直接執行cli
 ```
 $ shioajicaller update
-$ shioajicaller -u YOUID -p YOU_PASSWORD
+$ shioajicaller -api YOU_API_KEY -secret YOU_SECRET_KEY
 ```
 ### 新增 redis
 ```
 $ shioajicaller update -rh 127.0.0.1 -rp 6379 -rdb 0 -t redis
-$ shioajicaller -t redis -u YOUID -p YOU_PASSWORD
+$ shioajicaller -t redis -api YOU_API_KEY -secret YOU_SECRET_KEY
 ```
 ### ENV範例
 
 可使用環境變數與.env擋案
 
 ```
 API_KEY=YOU_API_KEY
```

### Comparing `shioajicaller-0.4.1.2/pyproject.toml` & `shioajicaller-0.4.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "shioajicaller"
-version = "0.4.1.2"
+version = "0.4.1.3"
 description = "shioaj warp caller"
 authors = ["Steve Lo <info@sd.idv.tw>"]
 license = "MIT"
 repository = "https://github.com/SDpower/shioajicaller"
 readme = ["README.md", "LICENSE"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-shioaji = {extras = ["speed"], version = "^1.1.0"}
+shioaji = {extras = ["speed"], version = "^1.1.6"}
 python-dotenv = "^0.19.0"
 redis = "^4.5.4"
 websockets = "^10.0"
 gmqtt = "^0.6.10"
 orjson = "^3.8.0"
 uvloop = {version = "^0.17.0", platform = "linux"}
```

### Comparing `shioajicaller-0.4.1.2/shioajicaller/caller.py` & `shioajicaller-0.4.1.3/shioajicaller/caller.py`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.1.2/shioajicaller/cli/__init__.py` & `shioajicaller-0.4.1.3/shioajicaller/cli/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     level=logging.WARNING,
     format="%(asctime)s %(levelname)s %(message)s",
 )
 
 def update():
     parser = argparse.ArgumentParser(
         description='Update Code List')
-    parser.add_argument('-api', '--api-key', nargs='+', help='Shioaji API_KEY')
-    parser.add_argument('-secret', '--secret-key', nargs='+' , help='Shioaji SECRET_KEY')
+    parser.add_argument('-api', '--api-key', type=str, default='', help='Shioaji API_KEY')
+    parser.add_argument('-secret', '--secret-key', type=str, default='' , help='Shioaji SECRET_KEY')
     parser.add_argument('-t', '--type', default='csv', help='output type csv or redis')
     parser.add_argument('-rh', '--redis-host', default='127.0.0.1', help='redis host')
     parser.add_argument('-rp', '--redis-port',type=int, default=6379, help='redis port')
     parser.add_argument('-rdb', '--redis-db',type=int, default=0, help='reis db')
     args = parser.parse_args(sys.argv[2:])
     callers = Caller()
     callers.SetAccount(apiKey= args.api_key ,secretKey= args.secret_key)
@@ -46,16 +46,16 @@
 
         __update_codes_redis(callers,host,port,db)
     print('Done!')
 
 def websockets():
     parser = argparse.ArgumentParser(
         description='Websockets Server')
-    parser.add_argument('-api', '--api-key', nargs='+', help='Shioaji API_KEY')
-    parser.add_argument('-secret', '--secret-key', nargs='+' , help='Shioaji SECRET_KEY')
+    parser.add_argument('-api', '--api-key', type=str, default='', help='Shioaji API_KEY')
+    parser.add_argument('-secret', '--secret-key', type=str, default='' , help='Shioaji SECRET_KEY')
     parser.add_argument('-wp', '--websockets-port',type=int, default=6789, help='Websockets port')
     parser.add_argument('-ps', '--pool-size', type=int, default=50, help='pool size')
     parser.add_argument('-wr', '--with-redis', action="store_true", help='with redis publish.')
     parser.add_argument('-rh', '--redis-host', default='127.0.0.1', help='redis host')
     parser.add_argument('-rp', '--redis-port',type=int, default=6379, help='redis port')
     parser.add_argument('-rdb', '--redis-db',type=int, default=0, help='reis db')
     parser.add_argument('-wm', '--with-mqtt', action="store_true", help='with mqtt publish.')
```

### Comparing `shioajicaller-0.4.1.2/shioajicaller/codes/update.py` & `shioajicaller-0.4.1.3/shioajicaller/codes/update.py`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.1.2/shioajicaller/config.py` & `shioajicaller-0.4.1.3/shioajicaller/config.py`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.1.2/shioajicaller/server/websocket.py` & `shioajicaller-0.4.1.3/shioajicaller/server/websocket.py`

 * *Files identical despite different names*

### Comparing `shioajicaller-0.4.1.2/PKG-INFO` & `shioajicaller-0.4.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shioajicaller
-Version: 0.4.1.2
+Version: 0.4.1.3
 Summary: shioaj warp caller
 Home-page: https://github.com/SDpower/shioajicaller
 License: MIT
 Author: Steve Lo
 Author-email: info@sd.idv.tw
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: gmqtt (>=0.6.10,<0.7.0)
 Requires-Dist: orjson (>=3.8.0,<4.0.0)
 Requires-Dist: python-dotenv (>=0.19.0,<0.20.0)
 Requires-Dist: redis (>=4.5.4,<5.0.0)
-Requires-Dist: shioaji[speed] (>=1.1.0,<2.0.0)
+Requires-Dist: shioaji[speed] (>=1.1.6,<2.0.0)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0) ; sys_platform == "linux"
 Requires-Dist: websockets (>=10.0,<11.0)
 Project-URL: Repository, https://github.com/SDpower/shioajicaller
 Description-Content-Type: text/markdown
 
 Shioaji Warp Caller P.O.C project.
 
@@ -198,31 +198,31 @@
   sdpower/shioaji_caller websockets -wm -ps 250
 ```
 
 ## 範例Example
 這裡說明範例，參數避免暴露請自行建立.env檔案就可以不用給帳號密碼參數。
 
 ```
-USER_ID=YOUID
-USER_PASSWORD=YOU_PASSWORD
+API_KEY= YOU_API_KEY
+SECRET_KEY= YOU_SECRET_KEY
 ```
 ### 執行範例
 ```
 $ python main.py update --help
-$ python main.py update -u YOUID -p YOU_PASSWORD
+$ python main.py update -api YOU_API_KEY -secret YOU_SECRET_KEY
 ```
 ### 直接執行cli
 ```
 $ shioajicaller update
-$ shioajicaller -u YOUID -p YOU_PASSWORD
+$ shioajicaller -api YOU_API_KEY -secret YOU_SECRET_KEY
 ```
 ### 新增 redis
 ```
 $ shioajicaller update -rh 127.0.0.1 -rp 6379 -rdb 0 -t redis
-$ shioajicaller -t redis -u YOUID -p YOU_PASSWORD
+$ shioajicaller -t redis -api YOU_API_KEY -secret YOU_SECRET_KEY
 ```
 ### ENV範例
 
 可使用環境變數與.env擋案
 
 ```
 API_KEY=YOU_API_KEY
```

