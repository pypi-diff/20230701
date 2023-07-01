# Comparing `tmp/Google Ads Transparency Scraper-1.5.tar.gz` & `tmp/Google-Ads-Transparency-Scraper-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Google Ads Transparency Scraper-1.5.tar", last modified: Wed Jun 28 12:33:39 2023, max compression
+gzip compressed data, was "Google-Ads-Transparency-Scraper-1.5.1.tar", last modified: Sat Jul  1 10:52:06 2023, max compression
```

## Comparing `Google Ads Transparency Scraper-1.5.tar` & `Google-Ads-Transparency-Scraper-1.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 12:33:39.057946 Google Ads Transparency Scraper-1.5/
-drwxrwxrwx   0        0        0        0 2023-06-28 12:33:39.041947 Google Ads Transparency Scraper-1.5/GoogleAdsTransparency/
--rw-rw-rw-   0        0        0      106 2023-06-28 05:20:16.000000 Google Ads Transparency Scraper-1.5/GoogleAdsTransparency/__init__.py
--rw-rw-rw-   0        0        0    10314 2023-06-28 07:22:06.000000 Google Ads Transparency Scraper-1.5/GoogleAdsTransparency/main.py
--rw-rw-rw-   0        0        0    11448 2023-06-28 06:06:26.000000 Google Ads Transparency Scraper-1.5/GoogleAdsTransparency/regions.py
-drwxrwxrwx   0        0        0        0 2023-06-28 12:33:39.057946 Google Ads Transparency Scraper-1.5/Google_Ads_Transparency_Scraper.egg-info/
--rw-rw-rw-   0        0        0      868 2023-06-28 12:33:38.000000 Google Ads Transparency Scraper-1.5/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      399 2023-06-28 12:33:38.000000 Google Ads Transparency Scraper-1.5/Google_Ads_Transparency_Scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 12:33:38.000000 Google Ads Transparency Scraper-1.5/Google_Ads_Transparency_Scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-06-28 12:33:38.000000 Google Ads Transparency Scraper-1.5/Google_Ads_Transparency_Scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-28 12:33:38.000000 Google Ads Transparency Scraper-1.5/Google_Ads_Transparency_Scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      868 2023-06-28 12:33:39.057946 Google Ads Transparency Scraper-1.5/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-06-26 11:23:38.000000 Google Ads Transparency Scraper-1.5/README.md
--rw-rw-rw-   0        0        0       86 2023-06-28 12:33:39.057946 Google Ads Transparency Scraper-1.5/setup.cfg
--rw-rw-rw-   0        0        0     1267 2023-06-28 12:33:15.000000 Google Ads Transparency Scraper-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 10:52:06.842738 Google-Ads-Transparency-Scraper-1.5.1/
+drwxrwxrwx   0        0        0        0 2023-07-01 10:52:06.813738 Google-Ads-Transparency-Scraper-1.5.1/GoogleAdsTransparency/
+-rw-rw-rw-   0        0        0      106 2023-06-28 05:20:16.000000 Google-Ads-Transparency-Scraper-1.5.1/GoogleAdsTransparency/__init__.py
+-rw-rw-rw-   0        0        0    10314 2023-06-28 07:22:06.000000 Google-Ads-Transparency-Scraper-1.5.1/GoogleAdsTransparency/main.py
+-rw-rw-rw-   0        0        0    11448 2023-06-28 06:06:26.000000 Google-Ads-Transparency-Scraper-1.5.1/GoogleAdsTransparency/regions.py
+drwxrwxrwx   0        0        0        0 2023-07-01 10:52:06.841744 Google-Ads-Transparency-Scraper-1.5.1/Google_Ads_Transparency_Scraper.egg-info/
+-rw-rw-rw-   0        0        0      876 2023-07-01 10:52:06.000000 Google-Ads-Transparency-Scraper-1.5.1/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-07-01 10:52:06.000000 Google-Ads-Transparency-Scraper-1.5.1/Google_Ads_Transparency_Scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 10:52:06.000000 Google-Ads-Transparency-Scraper-1.5.1/Google_Ads_Transparency_Scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-07-01 10:52:06.000000 Google-Ads-Transparency-Scraper-1.5.1/Google_Ads_Transparency_Scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-01 10:52:06.000000 Google-Ads-Transparency-Scraper-1.5.1/Google_Ads_Transparency_Scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      876 2023-07-01 10:52:06.842738 Google-Ads-Transparency-Scraper-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-06-26 11:23:38.000000 Google-Ads-Transparency-Scraper-1.5.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-01 10:52:06.845738 Google-Ads-Transparency-Scraper-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1275 2023-07-01 10:51:48.000000 Google-Ads-Transparency-Scraper-1.5.1/setup.py
```

### Comparing `Google Ads Transparency Scraper-1.5/GoogleAdsTransparency/main.py` & `Google-Ads-Transparency-Scraper-1.5.1/GoogleAdsTransparency/main.py`

 * *Files identical despite different names*

### Comparing `Google Ads Transparency Scraper-1.5/GoogleAdsTransparency/regions.py` & `Google-Ads-Transparency-Scraper-1.5.1/GoogleAdsTransparency/regions.py`

 * *Files identical despite different names*

### Comparing `Google Ads Transparency Scraper-1.5/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO` & `Google-Ads-Transparency-Scraper-1.5.1/Google_Ads_Transparency_Scraper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Google-Ads-Transparency-Scraper
-Version: 1.5
-Summary: A scraper for getting Ads from Google Transparency
+Version: 1.5.1
+Summary: A scraper for getting Ads from Google Ads Transparency
 Home-page: https://github.com/faniAhmed/GoogleAdsTransparencyScraper
-Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.2.tar.gz
+Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.1.tar.gz
 Author: Farhan Ahmed
 Author-email: jattfarhan10@gmail.com
 License: Securely Incorporation
 Keywords: Google,Transparency,Scraper,API,Google Ads,Ads,Google Transparency,Google Transparency Scraper,Google Ads Scrapre
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `Google Ads Transparency Scraper-1.5/PKG-INFO` & `Google-Ads-Transparency-Scraper-1.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: Google Ads Transparency Scraper
-Version: 1.5
-Summary: A scraper for getting Ads from Google Transparency
+Name: Google-Ads-Transparency-Scraper
+Version: 1.5.1
+Summary: A scraper for getting Ads from Google Ads Transparency
 Home-page: https://github.com/faniAhmed/GoogleAdsTransparencyScraper
-Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.2.tar.gz
+Download-URL: https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.1.tar.gz
 Author: Farhan Ahmed
 Author-email: jattfarhan10@gmail.com
 License: Securely Incorporation
 Keywords: Google,Transparency,Scraper,API,Google Ads,Ads,Google Transparency,Google Transparency Scraper,Google Ads Scrapre
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `Google Ads Transparency Scraper-1.5/setup.py` & `Google-Ads-Transparency-Scraper-1.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Install packages as defined in this file into the Python environment."""
 from setuptools import setup, find_packages
 
 setup(
-    name="Google Ads Transparency Scraper",
+    name="Google-Ads-Transparency-Scraper",
     author="Farhan Ahmed",
     author_email="jattfarhan10@gmail.com",
     url="https://github.com/faniAhmed/GoogleAdsTransparencyScraper",
-    description="A scraper for getting Ads from Google Transparency",
-    version="1.5",
+    description="A scraper for getting Ads from Google Ads Transparency",
+    version="1.5.1",
     packages=find_packages(),
-    download_url= 'https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.2.tar.gz',
+    download_url= 'https://github.com/faniAhmed/GoogleAdsTransparencyScraper/archive/refs/tags/v1.5.1.tar.gz',
     keywords= ['Google', 'Transparency', 'Scraper', 'API', 'Google Ads', 'Ads', 'Google Transparency', 'Google Transparency Scraper', 'Google Ads Scrapre'],
     license='Securely Incorporation',
     install_requires=[
         "setuptools>=45.0",
         "beautifulsoup4>=4.12.2",
         "Requests>=2.31.0",
         "lxml>=4.6.3",
```

