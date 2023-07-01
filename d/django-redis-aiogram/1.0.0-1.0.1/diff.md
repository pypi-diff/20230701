# Comparing `tmp/django-redis-aiogram-1.0.0.tar.gz` & `tmp/django-redis-aiogram-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-redis-aiogram-1.0.0.tar", last modified: Sat Jul  1 13:02:17 2023, max compression
+gzip compressed data, was "django-redis-aiogram-1.0.1.tar", last modified: Sat Jul  1 20:03:14 2023, max compression
```

## Comparing `django-redis-aiogram-1.0.0.tar` & `django-redis-aiogram-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 corneizer  (1000) corneizer  (1001)        0 2023-07-01 13:02:17.125528 django-redis-aiogram-1.0.0/
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)       52 2023-07-01 12:57:46.000000 django-redis-aiogram-1.0.0/CHANGELOG.md
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)       87 2023-06-30 00:14:25.000000 django-redis-aiogram-1.0.0/MANIFEST.in
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)     3145 2023-07-01 13:02:17.125528 django-redis-aiogram-1.0.0/PKG-INFO
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)     2375 2023-07-01 12:52:07.000000 django-redis-aiogram-1.0.0/README.md
-drwxr-xr-x   0 corneizer  (1000) corneizer  (1001)        0 2023-07-01 13:02:17.125528 django-redis-aiogram-1.0.0/django_redis_aiogram.egg-info/
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)     3145 2023-07-01 13:02:17.000000 django-redis-aiogram-1.0.0/django_redis_aiogram.egg-info/PKG-INFO
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)      628 2023-07-01 13:02:17.000000 django-redis-aiogram-1.0.0/django_redis_aiogram.egg-info/SOURCES.txt
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)        1 2023-07-01 13:02:17.000000 django-redis-aiogram-1.0.0/django_redis_aiogram.egg-info/dependency_links.txt
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)        1 2023-07-01 12:56:03.000000 django-redis-aiogram-1.0.0/django_redis_aiogram.egg-info/not-zip-safe
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)       38 2023-07-01 13:02:17.000000 django-redis-aiogram-1.0.0/django_redis_aiogram.egg-info/requires.txt
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)       13 2023-07-01 13:02:17.000000 django-redis-aiogram-1.0.0/django_redis_aiogram.egg-info/top_level.txt
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)       38 2023-07-01 13:02:17.125528 django-redis-aiogram-1.0.0/setup.cfg
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)     1261 2023-06-30 00:16:40.000000 django-redis-aiogram-1.0.0/setup.py
-drwxr-xr-x   0 corneizer  (1000) corneizer  (1001)        0 2023-07-01 13:02:17.125528 django-redis-aiogram-1.0.0/telegram_bot/
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)      193 2023-07-01 12:12:40.000000 django-redis-aiogram-1.0.0/telegram_bot/__init__.py
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)      414 2023-07-01 12:19:34.000000 django-redis-aiogram-1.0.0/telegram_bot/apps.py
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)     1471 2023-07-01 11:10:16.000000 django-redis-aiogram-1.0.0/telegram_bot/checks.py
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)      409 2023-07-01 11:10:08.000000 django-redis-aiogram-1.0.0/telegram_bot/defaults.py
-drwxr-xr-x   0 corneizer  (1000) corneizer  (1001)        0 2023-07-01 13:02:17.125528 django-redis-aiogram-1.0.0/telegram_bot/management/
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)        0 2023-04-18 14:18:56.000000 django-redis-aiogram-1.0.0/telegram_bot/management/__init__.py
-drwxr-xr-x   0 corneizer  (1000) corneizer  (1001)        0 2023-07-01 13:02:17.125528 django-redis-aiogram-1.0.0/telegram_bot/management/commands/
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)        0 2023-04-18 14:18:56.000000 django-redis-aiogram-1.0.0/telegram_bot/management/commands/__init__.py
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)     1413 2023-06-30 13:33:45.000000 django-redis-aiogram-1.0.0/telegram_bot/management/commands/start_tgbot.py
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)      109 2023-06-30 12:41:08.000000 django-redis-aiogram-1.0.0/telegram_bot/redis.py
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)      939 2023-07-01 11:10:08.000000 django-redis-aiogram-1.0.0/telegram_bot/settings.py
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)      556 2023-07-01 12:55:16.000000 django-redis-aiogram-1.0.0/telegram_bot/signals.py
--rw-r--r--   0 corneizer  (1000) corneizer  (1001)     5434 2023-07-01 12:28:01.000000 django-redis-aiogram-1.0.0/telegram_bot/telegram_bot.py
+drwxr-xr-x   0 corneizer  (1000) corneizer  (1001)        0 2023-07-01 20:03:14.014064 django-redis-aiogram-1.0.1/
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)       52 2023-07-01 13:13:16.000000 django-redis-aiogram-1.0.1/CHANGELOG.md
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)     1064 2023-07-01 13:13:16.000000 django-redis-aiogram-1.0.1/LICENSE
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)       87 2023-07-01 13:13:16.000000 django-redis-aiogram-1.0.1/MANIFEST.in
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)     3169 2023-07-01 20:03:14.014064 django-redis-aiogram-1.0.1/PKG-INFO
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)     2377 2023-07-01 19:58:58.000000 django-redis-aiogram-1.0.1/README.md
+drwxr-xr-x   0 corneizer  (1000) corneizer  (1001)        0 2023-07-01 20:03:14.014064 django-redis-aiogram-1.0.1/django_redis_aiogram.egg-info/
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)     3169 2023-07-01 20:03:14.000000 django-redis-aiogram-1.0.1/django_redis_aiogram.egg-info/PKG-INFO
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)      636 2023-07-01 20:03:14.000000 django-redis-aiogram-1.0.1/django_redis_aiogram.egg-info/SOURCES.txt
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)        1 2023-07-01 20:03:14.000000 django-redis-aiogram-1.0.1/django_redis_aiogram.egg-info/dependency_links.txt
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)        1 2023-07-01 12:56:03.000000 django-redis-aiogram-1.0.1/django_redis_aiogram.egg-info/not-zip-safe
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)       38 2023-07-01 20:03:14.000000 django-redis-aiogram-1.0.1/django_redis_aiogram.egg-info/requires.txt
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)       13 2023-07-01 20:03:14.000000 django-redis-aiogram-1.0.1/django_redis_aiogram.egg-info/top_level.txt
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)       38 2023-07-01 20:03:14.014064 django-redis-aiogram-1.0.1/setup.cfg
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)     1261 2023-07-01 20:03:07.000000 django-redis-aiogram-1.0.1/setup.py
+drwxr-xr-x   0 corneizer  (1000) corneizer  (1001)        0 2023-07-01 20:03:14.014064 django-redis-aiogram-1.0.1/telegram_bot/
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)      193 2023-07-01 13:13:16.000000 django-redis-aiogram-1.0.1/telegram_bot/__init__.py
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)      414 2023-07-01 13:13:16.000000 django-redis-aiogram-1.0.1/telegram_bot/apps.py
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)     1471 2023-07-01 13:13:16.000000 django-redis-aiogram-1.0.1/telegram_bot/checks.py
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)      409 2023-07-01 13:13:16.000000 django-redis-aiogram-1.0.1/telegram_bot/defaults.py
+drwxr-xr-x   0 corneizer  (1000) corneizer  (1001)        0 2023-07-01 20:03:14.014064 django-redis-aiogram-1.0.1/telegram_bot/management/
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)        0 2023-07-01 13:13:16.000000 django-redis-aiogram-1.0.1/telegram_bot/management/__init__.py
+drwxr-xr-x   0 corneizer  (1000) corneizer  (1001)        0 2023-07-01 20:03:14.014064 django-redis-aiogram-1.0.1/telegram_bot/management/commands/
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)        0 2023-07-01 13:13:16.000000 django-redis-aiogram-1.0.1/telegram_bot/management/commands/__init__.py
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)     1413 2023-07-01 13:13:16.000000 django-redis-aiogram-1.0.1/telegram_bot/management/commands/start_tgbot.py
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)      109 2023-07-01 13:13:16.000000 django-redis-aiogram-1.0.1/telegram_bot/redis.py
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)      939 2023-07-01 13:13:16.000000 django-redis-aiogram-1.0.1/telegram_bot/settings.py
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)      556 2023-07-01 13:13:16.000000 django-redis-aiogram-1.0.1/telegram_bot/signals.py
+-rw-r--r--   0 corneizer  (1000) corneizer  (1001)     5434 2023-07-01 13:13:16.000000 django-redis-aiogram-1.0.1/telegram_bot/telegram_bot.py
```

### Comparing `django-redis-aiogram-1.0.0/PKG-INFO` & `django-redis-aiogram-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-redis-aiogram
-Version: 1.0.0
+Version: 1.0.1
 Summary: Running aiogram in neighbor container, sending messages to telegram via redis
 Home-page: https://github.com/CorneiZeR/django-redis-aiogram
 Author: Oleksii Kolosiuk
 Author-email: kolosyuk1@gmail.com
 License: MIT
 Keywords: django redis aiogram docker
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,26 +13,27 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # django-redis-aiogram
 
 `django-redis-aiogram` provides a quick way to install `aiogram` in a container adjacent to `django`, allowing you to use your own router and loop. Also Allows you to send messages through `redis`.
 
 ### Supported Python and Django releases
 
 Current release of `django-redis-aiogram` is **1.0.0**, and it supports Python 3.8+ and Django 4.2+.
 
 ## Installation
 
-The easiest and recommended way to install `django-redis-aiogram` is from [PyPI](https://pypi.python.org/pypi/django-subadmin)
+The easiest and recommended way to install `django-redis-aiogram` is from [PyPI](https://pypi.org/project/django-redis-aiogram/)
 
 ``` shell
 pip install django-redis-aiogram
 ```
 
 You need to add `telegram_bot` to `INSTALLED_APPS` in your projects `settings.py`.
```

### Comparing `django-redis-aiogram-1.0.0/README.md` & `django-redis-aiogram-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ### Supported Python and Django releases
 
 Current release of `django-redis-aiogram` is **1.0.0**, and it supports Python 3.8+ and Django 4.2+.
 
 ## Installation
 
-The easiest and recommended way to install `django-redis-aiogram` is from [PyPI](https://pypi.python.org/pypi/django-subadmin)
+The easiest and recommended way to install `django-redis-aiogram` is from [PyPI](https://pypi.org/project/django-redis-aiogram/)
 
 ``` shell
 pip install django-redis-aiogram
 ```
 
 You need to add `telegram_bot` to `INSTALLED_APPS` in your projects `settings.py`.
```

### Comparing `django-redis-aiogram-1.0.0/django_redis_aiogram.egg-info/PKG-INFO` & `django-redis-aiogram-1.0.1/django_redis_aiogram.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-redis-aiogram
-Version: 1.0.0
+Version: 1.0.1
 Summary: Running aiogram in neighbor container, sending messages to telegram via redis
 Home-page: https://github.com/CorneiZeR/django-redis-aiogram
 Author: Oleksii Kolosiuk
 Author-email: kolosyuk1@gmail.com
 License: MIT
 Keywords: django redis aiogram docker
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,26 +13,27 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # django-redis-aiogram
 
 `django-redis-aiogram` provides a quick way to install `aiogram` in a container adjacent to `django`, allowing you to use your own router and loop. Also Allows you to send messages through `redis`.
 
 ### Supported Python and Django releases
 
 Current release of `django-redis-aiogram` is **1.0.0**, and it supports Python 3.8+ and Django 4.2+.
 
 ## Installation
 
-The easiest and recommended way to install `django-redis-aiogram` is from [PyPI](https://pypi.python.org/pypi/django-subadmin)
+The easiest and recommended way to install `django-redis-aiogram` is from [PyPI](https://pypi.org/project/django-redis-aiogram/)
 
 ``` shell
 pip install django-redis-aiogram
 ```
 
 You need to add `telegram_bot` to `INSTALLED_APPS` in your projects `settings.py`.
```

### Comparing `django-redis-aiogram-1.0.0/django_redis_aiogram.egg-info/SOURCES.txt` & `django-redis-aiogram-1.0.1/django_redis_aiogram.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CHANGELOG.md
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 django_redis_aiogram.egg-info/PKG-INFO
 django_redis_aiogram.egg-info/SOURCES.txt
 django_redis_aiogram.egg-info/dependency_links.txt
 django_redis_aiogram.egg-info/not-zip-safe
```

### Comparing `django-redis-aiogram-1.0.0/setup.py` & `django-redis-aiogram-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from io import open
 from setuptools import setup, find_packages
 
 NAME = 'django-redis-aiogram'
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 
 
 def read_md(file_path):
     with open(file_path) as fp:
         return fp.read()
```

### Comparing `django-redis-aiogram-1.0.0/telegram_bot/checks.py` & `django-redis-aiogram-1.0.1/telegram_bot/checks.py`

 * *Files identical despite different names*

### Comparing `django-redis-aiogram-1.0.0/telegram_bot/management/commands/start_tgbot.py` & `django-redis-aiogram-1.0.1/telegram_bot/management/commands/start_tgbot.py`

 * *Files identical despite different names*

### Comparing `django-redis-aiogram-1.0.0/telegram_bot/settings.py` & `django-redis-aiogram-1.0.1/telegram_bot/settings.py`

 * *Files identical despite different names*

### Comparing `django-redis-aiogram-1.0.0/telegram_bot/signals.py` & `django-redis-aiogram-1.0.1/telegram_bot/signals.py`

 * *Files identical despite different names*

### Comparing `django-redis-aiogram-1.0.0/telegram_bot/telegram_bot.py` & `django-redis-aiogram-1.0.1/telegram_bot/telegram_bot.py`

 * *Files identical despite different names*

