# Comparing `tmp/bose-2.0.1.tar.gz` & `tmp/bose-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bose-2.0.1.tar", last modified: Sat Jul  1 12:34:18 2023, max compression
+gzip compressed data, was "bose-2.0.2.tar", last modified: Sat Jul  1 15:55:11 2023, max compression
```

## Comparing `bose-2.0.1.tar` & `bose-2.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 12:34:18.549460 bose-2.0.1/
--rw-rw-rw-   0        0        0    14240 2023-07-01 12:34:18.550453 bose-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    10461 2023-05-24 16:36:27.405231 bose-2.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-01 12:34:18.548459 bose-2.0.1/bose/
--rw-rw-rw-   0        0        0      452 2023-06-30 14:14:28.791702 bose-2.0.1/bose/__init__.py
--rw-rw-rw-   0        0        0     4160 2023-07-01 09:12:23.121716 bose-2.0.1/bose/account_generator.py
--rw-rw-rw-   0        0        0      707 2023-06-30 05:04:43.924597 bose-2.0.1/bose/analytics.py
--rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-2.0.1/bose/base_data.py
--rw-rw-rw-   0        0        0     8287 2023-07-01 12:32:35.823549 bose-2.0.1/bose/base_task.py
--rw-rw-rw-   0        0        0      317 2023-06-29 11:53:16.211079 bose-2.0.1/bose/beep_utils.py
--rw-rw-rw-   0        0        0     9954 2023-07-01 09:15:52.186941 bose-2.0.1/bose/bose_driver.py
--rw-rw-rw-   0        0        0     9966 2023-07-01 09:15:52.186941 bose-2.0.1/bose/bose_undetected_driver.py
--rw-rw-rw-   0        0        0     7700 2023-06-29 13:46:50.340921 bose-2.0.1/bose/create_driver.py
--rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-2.0.1/bose/download_driver.py
--rw-rw-rw-   0        0        0      948 2023-06-30 07:55:50.167685 bose-2.0.1/bose/ip_utils.py
--rw-rw-rw-   0        0        0     2953 2023-06-30 15:33:26.223178 bose-2.0.1/bose/launch_tasks.py
--rw-rw-rw-   0        0        0     3185 2023-06-29 08:54:46.918966 bose-2.0.1/bose/local_storage.py
--rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-2.0.1/bose/local_storage_driver.py
--rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-2.0.1/bose/opponent.py
--rw-rw-rw-   0        0        0     2510 2023-07-01 09:16:40.175639 bose-2.0.1/bose/output.py
--rw-rw-rw-   0        0        0     4600 2023-07-01 06:42:54.180748 bose-2.0.1/bose/profile.py
--rw-rw-rw-   0        0        0      853 2023-06-29 11:00:24.518432 bose-2.0.1/bose/schedule_utils.py
--rw-rw-rw-   0        0        0      460 2023-06-29 10:04:53.656427 bose-2.0.1/bose/task_config.py
--rw-rw-rw-   0        0        0     1375 2023-07-01 09:14:29.721606 bose-2.0.1/bose/task_info.py
--rw-rw-rw-   0        0        0     5429 2023-06-26 10:10:30.768354 bose-2.0.1/bose/temp_mail.py
--rw-rw-rw-   0        0        0     7361 2023-05-10 09:24:37.900794 bose-2.0.1/bose/user_agent.py
--rw-rw-rw-   0        0        0     6210 2023-07-01 09:18:35.128413 bose-2.0.1/bose/utils.py
--rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-2.0.1/bose/wait.py
--rw-rw-rw-   0        0        0     1203 2023-05-09 07:09:28.075948 bose-2.0.1/bose/window_size.py
--rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2312 2023-07-01 12:34:06.665361 bose-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:55:11.822726 bose-2.0.2/
+-rw-rw-rw-   0        0        0    14240 2023-07-01 15:55:11.822726 bose-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10461 2023-05-24 16:36:27.405231 bose-2.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-01 15:55:11.822726 bose-2.0.2/bose/
+-rw-rw-rw-   0        0        0      452 2023-06-30 14:14:28.791702 bose-2.0.2/bose/__init__.py
+-rw-rw-rw-   0        0        0     4160 2023-07-01 09:12:23.121716 bose-2.0.2/bose/account_generator.py
+-rw-rw-rw-   0        0        0      707 2023-06-30 05:04:43.924597 bose-2.0.2/bose/analytics.py
+-rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-2.0.2/bose/base_data.py
+-rw-rw-rw-   0        0        0     8287 2023-07-01 12:32:35.823549 bose-2.0.2/bose/base_task.py
+-rw-rw-rw-   0        0        0      317 2023-06-29 11:53:16.211079 bose-2.0.2/bose/beep_utils.py
+-rw-rw-rw-   0        0        0    10014 2023-07-01 15:53:31.955272 bose-2.0.2/bose/bose_driver.py
+-rw-rw-rw-   0        0        0    10026 2023-07-01 15:54:08.464721 bose-2.0.2/bose/bose_undetected_driver.py
+-rw-rw-rw-   0        0        0     7700 2023-06-29 13:46:50.340921 bose-2.0.2/bose/create_driver.py
+-rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-2.0.2/bose/download_driver.py
+-rw-rw-rw-   0        0        0      948 2023-06-30 07:55:50.167685 bose-2.0.2/bose/ip_utils.py
+-rw-rw-rw-   0        0        0     2953 2023-06-30 15:33:26.223178 bose-2.0.2/bose/launch_tasks.py
+-rw-rw-rw-   0        0        0     3185 2023-06-29 08:54:46.918966 bose-2.0.2/bose/local_storage.py
+-rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-2.0.2/bose/local_storage_driver.py
+-rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-2.0.2/bose/opponent.py
+-rw-rw-rw-   0        0        0     2510 2023-07-01 09:16:40.175639 bose-2.0.2/bose/output.py
+-rw-rw-rw-   0        0        0     4600 2023-07-01 06:42:54.180748 bose-2.0.2/bose/profile.py
+-rw-rw-rw-   0        0        0      853 2023-06-29 11:00:24.518432 bose-2.0.2/bose/schedule_utils.py
+-rw-rw-rw-   0        0        0      460 2023-06-29 10:04:53.656427 bose-2.0.2/bose/task_config.py
+-rw-rw-rw-   0        0        0     1375 2023-07-01 09:14:29.721606 bose-2.0.2/bose/task_info.py
+-rw-rw-rw-   0        0        0     5429 2023-06-26 10:10:30.768354 bose-2.0.2/bose/temp_mail.py
+-rw-rw-rw-   0        0        0     7361 2023-05-10 09:24:37.900794 bose-2.0.2/bose/user_agent.py
+-rw-rw-rw-   0        0        0     6210 2023-07-01 09:18:35.128413 bose-2.0.2/bose/utils.py
+-rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-2.0.2/bose/wait.py
+-rw-rw-rw-   0        0        0     1203 2023-05-09 07:09:28.075948 bose-2.0.2/bose/window_size.py
+-rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2312 2023-07-01 15:54:52.364280 bose-2.0.2/setup.py
```

### Comparing `bose-2.0.1/PKG-INFO` & `bose-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bose
-Version: 2.0.1
+Version: 2.0.2
 Summary: The Ultimate Web Scraping Framework
 Home-page: UNKNOWN
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Description: 🚀 Introducing ✨ Bose Framework - The Swiss Army Knife for Bot Developers 🤖
         =============================================================================
```

### Comparing `bose-2.0.1/README.rst` & `bose-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `bose-2.0.1/bose/account_generator.py` & `bose-2.0.2/bose/account_generator.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.1/bose/analytics.py` & `bose-2.0.2/bose/analytics.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.1/bose/base_data.py` & `bose-2.0.2/bose/base_data.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.1/bose/base_task.py` & `bose-2.0.2/bose/base_task.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.1/bose/bose_driver.py` & `bose-2.0.2/bose/bose_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,18 +127,18 @@
     def scroll_site(self):
         self.execute_script(""" 
 window.scrollBy(0, 10000);
 """)
 
     def scroll_element(self, element):
 
-        is_till_end = self.execute_script(
-            "return arguments[0].scrollTop === (arguments[0].scrollHeight - arguments[0].offsetHeight)", element)
+        did_element_scroll = self.execute_script(
+            "return Math.round(arguments[0].scrollTop) === Math.round(Math.round(arguments[0].scrollHeight) - Math.round(arguments[0].offsetHeight))", element)
 
-        if is_till_end:
+        if did_element_scroll:
             return False
         else:
             self.execute_script("arguments[0].scrollBy(0, 10000)", element)
             return True
 
     def get_cookies_dict(self):
         all_cookies = self.get_cookies()
```

### Comparing `bose-2.0.1/bose/bose_undetected_driver.py` & `bose-2.0.2/bose/bose_undetected_driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,18 +127,18 @@
     def scroll_site(self):
         self.execute_script(""" 
 window.scrollBy(0, 10000);
 """)
 
     def scroll_element(self, element):
 
-        is_till_end = self.execute_script(
-            "return arguments[0].scrollTop === (arguments[0].scrollHeight - arguments[0].offsetHeight)", element)
+        did_element_scroll = self.execute_script(
+            "return Math.round(arguments[0].scrollTop) === Math.round(Math.round(arguments[0].scrollHeight) - Math.round(arguments[0].offsetHeight))", element)
 
-        if is_till_end:
+        if did_element_scroll:
             return False
         else:
             self.execute_script("arguments[0].scrollBy(0, 10000)", element)
             return True
 
     def get_cookies_dict(self):
         all_cookies = self.get_cookies()
```

### Comparing `bose-2.0.1/bose/create_driver.py` & `bose-2.0.2/bose/create_driver.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.1/bose/download_driver.py` & `bose-2.0.2/bose/download_driver.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.1/bose/ip_utils.py` & `bose-2.0.2/bose/ip_utils.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.1/bose/launch_tasks.py` & `bose-2.0.2/bose/launch_tasks.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.1/bose/local_storage.py` & `bose-2.0.2/bose/local_storage.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.1/bose/local_storage_driver.py` & `bose-2.0.2/bose/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.1/bose/output.py` & `bose-2.0.2/bose/output.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.1/bose/profile.py` & `bose-2.0.2/bose/profile.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.1/bose/schedule_utils.py` & `bose-2.0.2/bose/schedule_utils.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.1/bose/task_info.py` & `bose-2.0.2/bose/task_info.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.1/bose/temp_mail.py` & `bose-2.0.2/bose/temp_mail.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.1/bose/user_agent.py` & `bose-2.0.2/bose/user_agent.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.1/bose/utils.py` & `bose-2.0.2/bose/utils.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.1/bose/window_size.py` & `bose-2.0.2/bose/window_size.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.1/setup.py` & `bose-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     except:
       return None
     
             
 setup(
     name='bose',
     packages=['bose'],
-    version='2.0.1',
+    version='2.0.2',
     license='MIT',
     project_urls={
         "Documentation": "https://omkar.cloud/bose/",
         "Source": "https://github.com/omkarcloud/bose",
         "Tracker": "https://github.com/omkarcloud/bose/issues",
     },
```

