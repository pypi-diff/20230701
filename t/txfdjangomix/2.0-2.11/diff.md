# Comparing `tmp/txfdjangomix-2.0.tar.gz` & `tmp/txfdjangomix-2.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txfdjangomix-2.0.tar", last modified: Mon Jun 26 09:59:04 2023, max compression
+gzip compressed data, was "txfdjangomix-2.11.tar", last modified: Sat Jul  1 06:31:34 2023, max compression
```

## Comparing `txfdjangomix-2.0.tar` & `txfdjangomix-2.11.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 09:59:04.707639 txfdjangomix-2.0/
--rw-rw-rw-   0        0        0    11558 2022-06-17 08:26:46.000000 txfdjangomix-2.0/LICENSE
--rw-rw-rw-   0        0        0      425 2023-06-26 09:59:04.706642 txfdjangomix-2.0/PKG-INFO
--rw-rw-rw-   0        0        0       31 2022-06-17 09:05:06.000000 txfdjangomix-2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-26 09:59:04.707639 txfdjangomix-2.0/setup.cfg
--rw-rw-rw-   0        0        0      875 2023-06-26 09:58:38.000000 txfdjangomix-2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:59:04.580814 txfdjangomix-2.0/txfdjangomix/
--rw-rw-rw-   0        0        0     1205 2022-06-17 02:10:26.000000 txfdjangomix-2.0/txfdjangomix/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:59:04.605891 txfdjangomix-2.0/txfdjangomix/django_log/
--rw-rw-rw-   0        0        0     1205 2022-06-13 09:56:48.000000 txfdjangomix-2.0/txfdjangomix/django_log/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:59:04.651061 txfdjangomix-2.0/txfdjangomix/django_log/sql_log/
--rw-rw-rw-   0        0        0        0 2022-06-13 09:59:01.000000 txfdjangomix-2.0/txfdjangomix/django_log/sql_log/__init__.py
--rw-rw-rw-   0        0        0       66 2022-06-13 09:59:01.000000 txfdjangomix-2.0/txfdjangomix/django_log/sql_log/admin.py
--rw-rw-rw-   0        0        0      151 2022-06-13 09:59:01.000000 txfdjangomix-2.0/txfdjangomix/django_log/sql_log/apps.py
--rw-rw-rw-   0        0        0     2279 2022-06-16 09:45:23.000000 txfdjangomix-2.0/txfdjangomix/django_log/sql_log/insert_django_sql.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:59:04.652059 txfdjangomix-2.0/txfdjangomix/django_log/sql_log/migrations/
--rw-rw-rw-   0        0        0        0 2022-06-13 09:59:01.000000 txfdjangomix-2.0/txfdjangomix/django_log/sql_log/migrations/__init__.py
--rw-rw-rw-   0        0        0      936 2022-06-16 09:32:42.000000 txfdjangomix-2.0/txfdjangomix/django_log/sql_log/models.py
--rw-rw-rw-   0        0        0       63 2022-06-13 09:59:01.000000 txfdjangomix-2.0/txfdjangomix/django_log/sql_log/tests.py
--rw-rw-rw-   0        0        0       66 2022-06-13 09:59:01.000000 txfdjangomix-2.0/txfdjangomix/django_log/sql_log/views.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:59:04.678986 txfdjangomix-2.0/txfdjangomix/django_response_middleware/
--rw-rw-rw-   0        0        0      734 2021-12-06 02:22:57.000000 txfdjangomix-2.0/txfdjangomix/django_response_middleware/__init__.py
--rw-rw-rw-   0        0        0     2313 2023-06-26 09:58:18.000000 txfdjangomix-2.0/txfdjangomix/django_response_middleware/django_response_middleware.py
--rw-rw-rw-   0        0        0     3496 2021-12-06 02:22:57.000000 txfdjangomix-2.0/txfdjangomix/django_response_middleware/response_codes.py
--rw-rw-rw-   0        0        0     3500 2023-05-25 06:38:18.000000 txfdjangomix-2.0/txfdjangomix/django_response_middleware/response_data.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:59:04.695671 txfdjangomix-2.0/txfdjangomix/django_response_middleware/utils/
--rw-rw-rw-   0        0        0        0 2021-12-06 03:12:37.000000 txfdjangomix-2.0/txfdjangomix/django_response_middleware/utils/__init__.py
--rw-rw-rw-   0        0        0     1388 2022-06-06 01:56:29.000000 txfdjangomix-2.0/txfdjangomix/django_response_middleware/utils/json_cls.py
--rw-rw-rw-   0        0        0      755 2023-05-25 06:38:18.000000 txfdjangomix-2.0/txfdjangomix/django_response_middleware/utils/type_conversion.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:59:04.706642 txfdjangomix-2.0/txfdjangomix/utils/
--rw-rw-rw-   0        0        0        0 2022-07-05 11:50:18.000000 txfdjangomix-2.0/txfdjangomix/utils/__init__.py
--rw-rw-rw-   0        0        0     6381 2022-12-16 03:10:31.000000 txfdjangomix-2.0/txfdjangomix/utils/models.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:59:04.602899 txfdjangomix-2.0/txfdjangomix.egg-info/
--rw-rw-rw-   0        0        0      425 2023-06-26 09:59:04.000000 txfdjangomix-2.0/txfdjangomix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1132 2023-06-26 09:59:04.000000 txfdjangomix-2.0/txfdjangomix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 09:59:04.000000 txfdjangomix-2.0/txfdjangomix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-26 09:59:04.000000 txfdjangomix-2.0/txfdjangomix.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-26 09:59:04.000000 txfdjangomix-2.0/txfdjangomix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-07-05 11:52:46.000000 txfdjangomix-2.0/txfdjangomix.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-07-01 06:31:34.559569 txfdjangomix-2.11/
+-rw-rw-rw-   0        0        0    11558 2022-06-17 08:26:46.000000 txfdjangomix-2.11/LICENSE
+-rw-rw-rw-   0        0        0      426 2023-07-01 06:31:34.558572 txfdjangomix-2.11/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2022-06-17 09:05:06.000000 txfdjangomix-2.11/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-01 06:31:34.559569 txfdjangomix-2.11/setup.cfg
+-rw-rw-rw-   0        0        0      876 2023-07-01 06:29:49.000000 txfdjangomix-2.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 06:31:34.457720 txfdjangomix-2.11/txfdjangomix/
+-rw-rw-rw-   0        0        0     1205 2022-06-17 02:10:26.000000 txfdjangomix-2.11/txfdjangomix/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 06:31:34.478209 txfdjangomix-2.11/txfdjangomix/django_log/
+-rw-rw-rw-   0        0        0     1205 2022-06-13 09:56:48.000000 txfdjangomix-2.11/txfdjangomix/django_log/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 06:31:34.517105 txfdjangomix-2.11/txfdjangomix/django_log/sql_log/
+-rw-rw-rw-   0        0        0        0 2022-06-13 09:59:01.000000 txfdjangomix-2.11/txfdjangomix/django_log/sql_log/__init__.py
+-rw-rw-rw-   0        0        0       66 2022-06-13 09:59:01.000000 txfdjangomix-2.11/txfdjangomix/django_log/sql_log/admin.py
+-rw-rw-rw-   0        0        0      151 2022-06-13 09:59:01.000000 txfdjangomix-2.11/txfdjangomix/django_log/sql_log/apps.py
+-rw-rw-rw-   0        0        0     2279 2022-06-16 09:45:23.000000 txfdjangomix-2.11/txfdjangomix/django_log/sql_log/insert_django_sql.py
+drwxrwxrwx   0        0        0        0 2023-07-01 06:31:34.518102 txfdjangomix-2.11/txfdjangomix/django_log/sql_log/migrations/
+-rw-rw-rw-   0        0        0        0 2022-06-13 09:59:01.000000 txfdjangomix-2.11/txfdjangomix/django_log/sql_log/migrations/__init__.py
+-rw-rw-rw-   0        0        0      936 2022-06-16 09:32:42.000000 txfdjangomix-2.11/txfdjangomix/django_log/sql_log/models.py
+-rw-rw-rw-   0        0        0       63 2022-06-13 09:59:01.000000 txfdjangomix-2.11/txfdjangomix/django_log/sql_log/tests.py
+-rw-rw-rw-   0        0        0       66 2022-06-13 09:59:01.000000 txfdjangomix-2.11/txfdjangomix/django_log/sql_log/views.py
+drwxrwxrwx   0        0        0        0 2023-07-01 06:31:34.539623 txfdjangomix-2.11/txfdjangomix/django_response_middleware/
+-rw-rw-rw-   0        0        0      734 2021-12-06 02:22:57.000000 txfdjangomix-2.11/txfdjangomix/django_response_middleware/__init__.py
+-rw-rw-rw-   0        0        0     2303 2023-07-01 06:28:54.000000 txfdjangomix-2.11/txfdjangomix/django_response_middleware/django_response_middleware.py
+-rw-rw-rw-   0        0        0     3496 2021-12-06 02:22:57.000000 txfdjangomix-2.11/txfdjangomix/django_response_middleware/response_codes.py
+-rw-rw-rw-   0        0        0     3500 2023-05-25 06:38:18.000000 txfdjangomix-2.11/txfdjangomix/django_response_middleware/response_data.py
+drwxrwxrwx   0        0        0        0 2023-07-01 06:31:34.549595 txfdjangomix-2.11/txfdjangomix/django_response_middleware/utils/
+-rw-rw-rw-   0        0        0        0 2021-12-06 03:12:37.000000 txfdjangomix-2.11/txfdjangomix/django_response_middleware/utils/__init__.py
+-rw-rw-rw-   0        0        0     1540 2023-07-01 06:29:33.000000 txfdjangomix-2.11/txfdjangomix/django_response_middleware/utils/json_cls.py
+-rw-rw-rw-   0        0        0      755 2023-05-25 06:38:18.000000 txfdjangomix-2.11/txfdjangomix/django_response_middleware/utils/type_conversion.py
+drwxrwxrwx   0        0        0        0 2023-07-01 06:31:34.557574 txfdjangomix-2.11/txfdjangomix/utils/
+-rw-rw-rw-   0        0        0        0 2022-07-05 11:50:18.000000 txfdjangomix-2.11/txfdjangomix/utils/__init__.py
+-rw-rw-rw-   0        0        0     6381 2022-12-16 03:10:31.000000 txfdjangomix-2.11/txfdjangomix/utils/models.py
+drwxrwxrwx   0        0        0        0 2023-07-01 06:31:34.475708 txfdjangomix-2.11/txfdjangomix.egg-info/
+-rw-rw-rw-   0        0        0      426 2023-07-01 06:31:34.000000 txfdjangomix-2.11/txfdjangomix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1132 2023-07-01 06:31:34.000000 txfdjangomix-2.11/txfdjangomix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 06:31:34.000000 txfdjangomix-2.11/txfdjangomix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-01 06:31:34.000000 txfdjangomix-2.11/txfdjangomix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-01 06:31:34.000000 txfdjangomix-2.11/txfdjangomix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-07-05 11:52:46.000000 txfdjangomix-2.11/txfdjangomix.egg-info/zip-safe
```

### Comparing `txfdjangomix-2.0/LICENSE` & `txfdjangomix-2.11/LICENSE`

 * *Files identical despite different names*

### Comparing `txfdjangomix-2.0/setup.py` & `txfdjangomix-2.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='txfdjangomix',  # 名字
-      version='2.0',  # 版本
+      version='2.11',  # 版本
       description='django response middleware',  # 简介一般我们放在readme.md
       classifiers=[
           'Programming Language :: Python',  # python
           'Intended Audience :: Developers',  # 受众人
           'Operating System :: OS Independent',  # 系统
       ],
       long_description_content_type="text/markdown",  # 类型
```

### Comparing `txfdjangomix-2.0/txfdjangomix/__init__.py` & `txfdjangomix-2.11/txfdjangomix/__init__.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-2.0/txfdjangomix/django_log/__init__.py` & `txfdjangomix-2.11/txfdjangomix/django_log/__init__.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-2.0/txfdjangomix/django_log/sql_log/insert_django_sql.py` & `txfdjangomix-2.11/txfdjangomix/django_log/sql_log/insert_django_sql.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-2.0/txfdjangomix/django_log/sql_log/models.py` & `txfdjangomix-2.11/txfdjangomix/django_log/sql_log/models.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-2.0/txfdjangomix/django_response_middleware/__init__.py` & `txfdjangomix-2.11/txfdjangomix/django_response_middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-2.0/txfdjangomix/django_response_middleware/django_response_middleware.py` & `txfdjangomix-2.11/txfdjangomix/django_response_middleware/django_response_middleware.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,23 +16,23 @@
         response = self.get_response(request)
         return response
 
 
 class ResponseMiddleware(MyBaseMiddleware):
     """自定义返回结果"""
 
-    def process_template_response(self, request, response):
+    def error_message(self, response):
+        try:
+            return ';'.join(list(response.data.values()))
+        except:
+            return str(response.data).replace('[[', '').replace(']]', '')
 
+    def process_template_response(self, request, response):
         if hasattr(response, 'data'):
-            # ============  返回详情  ============
-            # {
-            #     "code": "200",
-            #     "message": "ok",
-            #     "datas": { ... }
-            # ============
+
             if response.status_code == 200:
                 data = response.data
                 if data:
                     if 'datas' not in response.data and 'code' not in response.data:
                         del response.data
                         response.data = {
                             'code': '{}'.format(response.status_code),
@@ -43,20 +43,20 @@
                     response.data = {
                         'code': '{}'.format(response.status_code),
                         'message': 'ok',
                         'datas': data
                     }
 
             else:
-
                 code = response.status_code
                 response.status_code = 200
+
                 response.data = {
                     'code': code,
-                    'message': ';'.join(list(response.data.values())),
+                    'message': self.error_message(response),
                     'datas': response.data,
                 }
 
         return response
 
 
 class CustomizeExceptionMiddleware(MyBaseMiddleware):
```

### Comparing `txfdjangomix-2.0/txfdjangomix/django_response_middleware/response_codes.py` & `txfdjangomix-2.11/txfdjangomix/django_response_middleware/response_codes.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-2.0/txfdjangomix/django_response_middleware/response_data.py` & `txfdjangomix-2.11/txfdjangomix/django_response_middleware/response_data.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-2.0/txfdjangomix/django_response_middleware/utils/json_cls.py` & `txfdjangomix-2.11/txfdjangomix/django_response_middleware/utils/json_cls.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,23 +22,27 @@
                 r = r[:23] + r[26:]
             if r.endswith('+00:00'):
                 r = r[:-6] + 'Z'
             return r
         elif isinstance(o, datetime.date):
             return o.isoformat()
         elif isinstance(o, datetime.time):
-
             r = o.isoformat()
             if o.microsecond:
                 r = r[:12]
             return r
         elif isinstance(o, datetime.timedelta):
             return duration_iso_string(o)
         elif isinstance(o, (decimal.Decimal, uuid.UUID, Promise)):
             return str(o)
         elif isinstance(o, (numpy.float64, numpy.float32, numpy.float16)):
             return float(o)
         elif isinstance(o, (numpy.int0, numpy.int8, numpy.int16, numpy.int32)):
             return int(o)
+        try:
+            return str(o)
+        except:
+            pass
         else:
+            print('json解析失败 数据:{} 类型:{}'.format(o), type(o))
             return super().default(o)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `txfdjangomix-2.0/txfdjangomix/django_response_middleware/utils/type_conversion.py` & `txfdjangomix-2.11/txfdjangomix/django_response_middleware/utils/type_conversion.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-2.0/txfdjangomix/utils/models.py` & `txfdjangomix-2.11/txfdjangomix/utils/models.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-2.0/txfdjangomix.egg-info/SOURCES.txt` & `txfdjangomix-2.11/txfdjangomix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

