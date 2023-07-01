# Comparing `tmp/SiteScraper-2.1.2.tar.gz` & `tmp/SiteScraper-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SiteScraper-2.1.2.tar", last modified: Fri Jun 30 18:15:02 2023, max compression
+gzip compressed data, was "SiteScraper-2.2.1.tar", last modified: Sat Jul  1 08:13:38 2023, max compression
```

## Comparing `SiteScraper-2.1.2.tar` & `SiteScraper-2.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 18:15:02.576250 SiteScraper-2.1.2/
--rw-rw-rw-   0        0        0     3989 2023-06-30 18:15:02.576250 SiteScraper-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3760 2023-05-25 09:12:48.000000 SiteScraper-2.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 18:15:02.568222 SiteScraper-2.1.2/SiteScraper/
--rw-rw-rw-   0        0        0    10726 2023-06-30 18:11:27.000000 SiteScraper-2.1.2/SiteScraper/SiteScraper.py
--rw-rw-rw-   0        0        0       46 2023-05-25 10:05:57.000000 SiteScraper-2.1.2/SiteScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 18:15:02.576250 SiteScraper-2.1.2/SiteScraper.egg-info/
--rw-rw-rw-   0        0        0     3989 2023-06-30 18:15:02.000000 SiteScraper-2.1.2/SiteScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-30 18:15:02.000000 SiteScraper-2.1.2/SiteScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 18:15:02.000000 SiteScraper-2.1.2/SiteScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-30 18:15:02.000000 SiteScraper-2.1.2/SiteScraper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-06-30 18:15:02.000000 SiteScraper-2.1.2/SiteScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-30 18:15:02.000000 SiteScraper-2.1.2/SiteScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      626 2023-05-25 07:53:45.000000 SiteScraper-2.1.2/licence.txt
--rw-rw-rw-   0        0        0      158 2023-06-30 18:15:02.576250 SiteScraper-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0      497 2023-06-30 18:14:28.000000 SiteScraper-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 08:13:38.787536 SiteScraper-2.2.1/
+-rw-rw-rw-   0        0        0     3989 2023-07-01 08:13:38.788869 SiteScraper-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3760 2023-05-25 09:12:48.000000 SiteScraper-2.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 08:13:38.778249 SiteScraper-2.2.1/SiteScraper/
+-rw-rw-rw-   0        0        0    10879 2023-07-01 08:12:45.000000 SiteScraper-2.2.1/SiteScraper/SiteScraper.py
+-rw-rw-rw-   0        0        0       46 2023-05-25 10:05:57.000000 SiteScraper-2.2.1/SiteScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 08:13:38.787536 SiteScraper-2.2.1/SiteScraper.egg-info/
+-rw-rw-rw-   0        0        0     3989 2023-07-01 08:13:38.000000 SiteScraper-2.2.1/SiteScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-01 08:13:38.000000 SiteScraper-2.2.1/SiteScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 08:13:38.000000 SiteScraper-2.2.1/SiteScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-01 08:13:38.000000 SiteScraper-2.2.1/SiteScraper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-01 08:13:38.000000 SiteScraper-2.2.1/SiteScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-01 08:13:38.000000 SiteScraper-2.2.1/SiteScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      626 2023-05-25 07:53:45.000000 SiteScraper-2.2.1/licence.txt
+-rw-rw-rw-   0        0        0      158 2023-07-01 08:13:38.789963 SiteScraper-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      497 2023-07-01 08:13:13.000000 SiteScraper-2.2.1/setup.py
```

### Comparing `SiteScraper-2.1.2/PKG-INFO` & `SiteScraper-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiteScraper
-Version: 2.1.2
+Version: 2.2.1
 Summary: Scraping high intensity content sites
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # SiteScraper
```

### Comparing `SiteScraper-2.1.2/README.md` & `SiteScraper-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `SiteScraper-2.1.2/SiteScraper/SiteScraper.py` & `SiteScraper-2.2.1/SiteScraper/SiteScraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,32 +195,36 @@
                 
                 driver.quit()
                 return dic
 
             except:
                 driver.quit()
                 logging.error('Invalid url')
-    def yt_vedio_links(self,url):
+    def yt_vedio_links(self,url,abort=bool):
         try:
             driver =self.web_driver_chrome()
             self.url = url
             driver.get(url)
             time.sleep(5)
             prev_h = 0
             prev_h = driver.execute_script("return document.documentElement.scrollHeight;")
+            counter=0
             while True:
                 # Scrolling to the bottom
                 driver.execute_script("window.scrollTo(0, document.documentElement.scrollHeight);")
                 time.sleep(3)
 
-               
+                counter=counter+1
                 new_height = driver.execute_script("return document.documentElement.scrollHeight;")
                 if new_height == prev_h:
                     break
                 prev_h = new_height
+                if abort==True:
+                    if counter>135:
+                        break
 
             
             links = driver.find_elements(By.XPATH, '//*[@id="video-title-link"]')
             vedio_links = [link.get_attribute('href') for link in links]
             return vedio_links
         except:
                 driver.quit()
```

### Comparing `SiteScraper-2.1.2/SiteScraper.egg-info/PKG-INFO` & `SiteScraper-2.2.1/SiteScraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiteScraper
-Version: 2.1.2
+Version: 2.2.1
 Summary: Scraping high intensity content sites
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # SiteScraper
```

### Comparing `SiteScraper-2.1.2/licence.txt` & `SiteScraper-2.2.1/licence.txt`

 * *Files identical despite different names*

