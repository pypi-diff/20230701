# Comparing `tmp/wpdetect-1.3.9.tar.gz` & `tmp/wpdetect-1.4.0.tar.gz`

## Comparing `wpdetect-1.3.9.tar` & `wpdetect-1.4.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 wpdetect-1.3.9/requirements.txt
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 wpdetect-1.3.9/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 wpdetect-1.3.9/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wpdetect-1.3.9/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.3.9/wpdetect/__init__.py
--rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 wpdetect-1.3.9/wpdetect/__main__.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 wpdetect-1.3.9/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wpdetect-1.3.9/LICENSE.txt
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 wpdetect-1.3.9/README.md
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 wpdetect-1.3.9/pyproject.toml
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 wpdetect-1.3.9/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 wpdetect-1.4.0/requirements.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wpdetect-1.4.0/sample_urls.txt
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 wpdetect-1.4.0/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 wpdetect-1.4.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wpdetect-1.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.4.0/wpdetect/__init__.py
+-rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 wpdetect-1.4.0/wpdetect/__main__.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 wpdetect-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wpdetect-1.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 wpdetect-1.4.0/README.md
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 wpdetect-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 wpdetect-1.4.0/PKG-INFO
```

### Comparing `wpdetect-1.3.9/.github/workflows/pylint.yml` & `wpdetect-1.4.0/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `wpdetect-1.3.9/.github/workflows/pypi-publish.yml` & `wpdetect-1.4.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `wpdetect-1.3.9/wpdetect/__main__.py` & `wpdetect-1.4.0/wpdetect/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 name: wpdetect
 description: A simple script to detect if a website is running WordPress.
 '''
 
 import sys
 import urllib.request
 import requests
+import click
 from pyfiglet import figlet_format
 
 HEADER = "'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_3) AppleWebKit/537.75.14" + \
     " (KHTML, like Gecko) Version/7.0.3 Safari/7046A194A'"
-VERSION = "1.3.9"
+VERSION = "1.4.0"
 
 # Error messages
 ERROR_UNABLE_TO_OPEN_URL = "Couldn't open url," + \
     " please make sure to type a valid and publicly accessible url.\n"
 
 # List to store the found WordPress installations
 wp_domains = []
@@ -162,48 +163,31 @@
                 url = domain.strip()
                 url_check(url, is_batch=True)
 
     except FileNotFoundError:
         print("Please enter the file name correctly, file not found!\n")
 
 
-arguments = {
-    '-h': usage,
-    '--help': usage,
-    '-v': lambda: print(VERSION),
-    '--version': lambda: print(VERSION),
-    '-f':  handle_file,
-    '--file': handle_file
-}
-
-
-def main():
-    """Main function."""
+@click.command()
+@click.argument('url', required=False)
+@click.option('-f', '--file', type=click.Path(exists=True), help="File with list of URLs to check.")
+@click.option('-v', '--version', is_flag=True, help="Print version.")
+def main(url, file, version):
+    """Detects if a website is running WordPress."""
 
     print_logo(VERSION)
 
-    try:
-        if len(sys.argv) > 1:
-            argument = sys.argv[1]
+    if url:
+        url_check(url)
 
-            # Check if the argument exists in the dictionary
-            if argument in arguments:
-                # Execute the corresponding action
-                arguments[argument](*sys.argv[2:])
-
-            else:
-                # Assume it's a URL and pass it to url_check
-                url_check(argument)
-        else:
-            usage()
+    if file:
+        handle_file(file)
 
-    except IndexError:
-        print(
-            "You didn't enter anything! Please try again, make sure to enter a valid url.")
-        usage()
+    if version:
+        print(VERSION)
 
-    except KeyboardInterrupt:
-        print("\nAborted by user.")
+    if len(sys.argv) == 1:
+        usage()
 
 
 if __name__ == '__main__':
-    main()
+    main(None, None, None)
```

### Comparing `wpdetect-1.3.9/.gitignore` & `wpdetect-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `wpdetect-1.3.9/LICENSE.txt` & `wpdetect-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wpdetect-1.3.9/README.md` & `wpdetect-1.4.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -38,14 +38,20 @@
 http://www.techcrunch.com/
 ```
 
 Please note that, it is not always possible to detect the presence of WordPress, website admins can take extra measures to remove sign of WordPress.
 
 ## Changelog
 
+#### What's new in version 1.4.0
+
+-   Removed manual argument parsing.
+-   Introduced [click](https://click.palletsprojects.com/en/8.1.x/) and parsing arguments with it.
+-   Added a sample URL in the repo for ease of testing.
+
 #### What's new in version 1.3.9
 
 -   Minor bug fixes
 -   Added workflow for linting on code push
 -   Added workflow for publishing to PyPi on release
 
 #### What's new in version 1.3.8
```

### Comparing `wpdetect-1.3.9/pyproject.toml` & `wpdetect-1.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wpdetect"
-version = "1.3.9"
+version = "1.4.0"
 dependencies = [
-    "pyfiglet", "requests"
+    "pyfiglet", "requests", "click"
 ]
 authors = [
   { name="S M Mahmudul Hasan", email="he@smmahmudulhasan.com" },
 ]
 description = "A WordPress detection tool, detects if a website is running WordPress"
 readme = "README.md"
 requires-python = ">=3.4"
```

### Comparing `wpdetect-1.3.9/PKG-INFO` & `wpdetect-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: wpdetect
-Version: 1.3.9
+Version: 1.4.0
 Summary: A WordPress detection tool, detects if a website is running WordPress
 Project-URL: Homepage, https://github.com/IamLizu/wpdetect
 Project-URL: Bug Tracker, https://github.com/IamLizu/wpdetect/issues
 Author-email: S M Mahmudul Hasan <he@smmahmudulhasan.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.4
+Requires-Dist: click
 Requires-Dist: pyfiglet
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # WP DETECT
 
 A WordPress detection tool, detects if a website is running WordPress. wpdetect is a great tool when you just want to check WordPress' presence but do not want to scan the site for vulnerabilities or issues.
@@ -57,14 +58,20 @@
 http://www.techcrunch.com/
 ```
 
 Please note that, it is not always possible to detect the presence of WordPress, website admins can take extra measures to remove sign of WordPress.
 
 ## Changelog
 
+#### What's new in version 1.4.0
+
+-   Removed manual argument parsing.
+-   Introduced [click](https://click.palletsprojects.com/en/8.1.x/) and parsing arguments with it.
+-   Added a sample URL in the repo for ease of testing.
+
 #### What's new in version 1.3.9
 
 -   Minor bug fixes
 -   Added workflow for linting on code push
 -   Added workflow for publishing to PyPi on release
 
 #### What's new in version 1.3.8
```

