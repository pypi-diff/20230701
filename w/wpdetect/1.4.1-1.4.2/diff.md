# Comparing `tmp/wpdetect-1.4.1.tar.gz` & `tmp/wpdetect-1.4.2.tar.gz`

## Comparing `wpdetect-1.4.1.tar` & `wpdetect-1.4.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 wpdetect-1.4.1/requirements.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wpdetect-1.4.1/sample_urls.txt
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 wpdetect-1.4.1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 wpdetect-1.4.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wpdetect-1.4.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.4.1/wpdetect/__init__.py
--rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 wpdetect-1.4.1/wpdetect/__main__.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 wpdetect-1.4.1/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wpdetect-1.4.1/LICENSE.txt
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 wpdetect-1.4.1/README.md
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 wpdetect-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 wpdetect-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 wpdetect-1.4.2/requirements.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wpdetect-1.4.2/sample_urls.txt
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 wpdetect-1.4.2/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 wpdetect-1.4.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wpdetect-1.4.2/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.4.2/wpdetect/__init__.py
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 wpdetect-1.4.2/wpdetect/__main__.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 wpdetect-1.4.2/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wpdetect-1.4.2/LICENSE.txt
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 wpdetect-1.4.2/README.md
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 wpdetect-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 wpdetect-1.4.2/PKG-INFO
```

### Comparing `wpdetect-1.4.1/.github/workflows/pylint.yml` & `wpdetect-1.4.2/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.1/.github/workflows/pypi-publish.yml` & `wpdetect-1.4.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.1/wpdetect/__main__.py` & `wpdetect-1.4.2/wpdetect/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import urllib.request
 import requests
 import click
 from pyfiglet import figlet_format
 
 HEADER = "'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_3) AppleWebKit/537.75.14" + \
     " (KHTML, like Gecko) Version/7.0.3 Safari/7046A194A'"
-VERSION = "1.4.1"
+VERSION = "1.4.2"
 
 # Error messages
 ERROR_UNABLE_TO_OPEN_URL = "Couldn't open url," + \
     " please make sure to type a valid and publicly accessible url.\n"
 
 # List to store the found WordPress installations
 wp_domains = []
@@ -80,21 +80,21 @@
     print("[+] Trying with HTTP.\n")
     url = "http://" + url[8:]
     print("Checking: " + str(url))
 
     return url
 
 
-def url_check(url, is_batch=False, show_signature=False):
+def url_check(url, show_signature=False):
     """
         Checks if the url is valid and publicly accessible.
         If so, it runs wp_check on it.
     """
 
-    print("Checking: " + str(url))
+    print("\nChecking: " + str(url))
     try:
         if url[:4] != "http":
             url = check_protocol(url)
 
         url = check_redirect(url)
 
         wp_signatures = {
@@ -113,18 +113,17 @@
 
             if result:
                 url_to_print = wp_signature if show_signature else url
 
                 print(f"[✓] WordPress found at: {url_to_print}")
 
                 wp_domains.append(url)
-                break
-
-        if len(wp_domains) == 0 and is_batch is False:
-            print("[X] No WordPress installation found!")
+            else:
+                print(f"[✗] WordPress not found at: {url}")
+            break
 
     except urllib.error.HTTPError as error:
         if error.code == 403:
             print("Got 403! Website seems to be behind a WAF.")
 
     except urllib.error.URLError:
         if url[:5] == "https":
@@ -147,19 +146,18 @@
         with open(filename, 'r', encoding='utf-8') as file:
             domains = file.readlines()
 
             print("Targets,\n")
 
             for domain in domains:
                 print(domain.strip())
-            print("\n")
 
             for domain in domains:
                 url = domain.strip()
-                url_check(url, True, show_signature)
+                url_check(url, show_signature)
 
     except FileNotFoundError:
         print("Please enter the file name correctly, file not found!\n")
 
 
 @click.command(context_settings={"help_option_names": ['-h', '--help']})
 @click.argument('url', required=False)
@@ -170,15 +168,15 @@
 def main(url, file, version, show_signature):
     """Detects if a website is running WordPress."""
 
     if version is False:
         print_logo(VERSION)
 
     if url:
-        url_check(url, False, show_signature)
+        url_check(url, show_signature)
 
     if file:
         handle_file(file, show_signature)
 
     if version:
         print(f"Version: {VERSION}")
```

### Comparing `wpdetect-1.4.1/.gitignore` & `wpdetect-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.1/LICENSE.txt` & `wpdetect-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.1/README.md` & `wpdetect-1.4.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,18 @@
 http://www.techcrunch.com/
 ```
 
 Please note that, it is not always possible to detect the presence of WordPress, website admins can take extra measures to remove sign of WordPress.
 
 ## Changelog
 
+#### What's new in version 1.4.2
+
+-   Fixed [#18](https://github.com/IamLizu/wpdetect/issues/18)
+
 #### What's new in version 1.4.1
 
 -   Fixed [#10](https://github.com/IamLizu/wpdetect/issues/10)
 -   Added `-h` in `click` help options
 
 #### What's new in version 1.4.0
```

### Comparing `wpdetect-1.4.1/pyproject.toml` & `wpdetect-1.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wpdetect"
-version = "1.4.1"
+version = "1.4.2"
 dependencies = [
     "pyfiglet", "requests", "click"
 ]
 authors = [
   { name="S M Mahmudul Hasan", email="he@smmahmudulhasan.com" },
 ]
 description = "A WordPress detection tool, detects if a website is running WordPress"
```

### Comparing `wpdetect-1.4.1/PKG-INFO` & `wpdetect-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpdetect
-Version: 1.4.1
+Version: 1.4.2
 Summary: A WordPress detection tool, detects if a website is running WordPress
 Project-URL: Homepage, https://github.com/IamLizu/wpdetect
 Project-URL: Bug Tracker, https://github.com/IamLizu/wpdetect/issues
 Author-email: S M Mahmudul Hasan <he@smmahmudulhasan.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -58,14 +58,18 @@
 http://www.techcrunch.com/
 ```
 
 Please note that, it is not always possible to detect the presence of WordPress, website admins can take extra measures to remove sign of WordPress.
 
 ## Changelog
 
+#### What's new in version 1.4.2
+
+-   Fixed [#18](https://github.com/IamLizu/wpdetect/issues/18)
+
 #### What's new in version 1.4.1
 
 -   Fixed [#10](https://github.com/IamLizu/wpdetect/issues/10)
 -   Added `-h` in `click` help options
 
 #### What's new in version 1.4.0
```

