# Comparing `tmp/wpdetect-1.4.2.tar.gz` & `tmp/wpdetect-1.4.3.tar.gz`

## Comparing `wpdetect-1.4.2.tar` & `wpdetect-1.4.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 wpdetect-1.4.2/requirements.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wpdetect-1.4.2/sample_urls.txt
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 wpdetect-1.4.2/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 wpdetect-1.4.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wpdetect-1.4.2/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.4.2/wpdetect/__init__.py
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 wpdetect-1.4.2/wpdetect/__main__.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 wpdetect-1.4.2/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wpdetect-1.4.2/LICENSE.txt
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 wpdetect-1.4.2/README.md
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 wpdetect-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 wpdetect-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 wpdetect-1.4.3/requirements.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wpdetect-1.4.3/sample_urls.txt
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 wpdetect-1.4.3/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 wpdetect-1.4.3/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wpdetect-1.4.3/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.4.3/wpdetect/__init__.py
+-rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 wpdetect-1.4.3/wpdetect/__main__.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 wpdetect-1.4.3/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wpdetect-1.4.3/LICENSE.txt
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 wpdetect-1.4.3/README.md
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 wpdetect-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 wpdetect-1.4.3/PKG-INFO
```

### Comparing `wpdetect-1.4.2/.github/workflows/pylint.yml` & `wpdetect-1.4.3/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.2/.github/workflows/pypi-publish.yml` & `wpdetect-1.4.3/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.2/wpdetect/__main__.py` & `wpdetect-1.4.3/wpdetect/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,32 +7,47 @@
 import urllib.request
 import requests
 import click
 from pyfiglet import figlet_format
 
 HEADER = "'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_3) AppleWebKit/537.75.14" + \
     " (KHTML, like Gecko) Version/7.0.3 Safari/7046A194A'"
-VERSION = "1.4.2"
+VERSION = "1.4.3"
 
 # Error messages
 ERROR_UNABLE_TO_OPEN_URL = "Couldn't open url," + \
     " please make sure to type a valid and publicly accessible url.\n"
 
 # List to store the found WordPress installations
 wp_domains = []
 
 
+# cli options store
+cli_options = {
+    'verbose': True,  # default value
+    'show_signature': False,  # default value
+}
+
+
+def print_verbose(message):
+    """Prints the message if verbose is true."""
+
+    if cli_options['verbose']:
+        print(message)
+
+
 def print_logo(version):
     """
         print_logo(version)
         Prints the logo with version number.
     """
 
-    print(figlet_format('     wpdetect     '))
-    print("=================== VERSION: " + version + " ===================\n")
+    print_verbose(figlet_format('     wpdetect     '))
+    print_verbose("=================== VERSION: " +
+                  version + " ===================\n")
 
 
 def wp_check(url):
     """Checks if the given url is a WordPress installation."""
 
     wp_signature = urllib.request.Request(url, headers={'User-Agent': HEADER})
 
@@ -45,56 +60,56 @@
 
     return False
 
 
 def check_protocol(url):
     """Checks if the url has a protocol specified, if not, it adds HTTP."""
 
-    print("[!] No protocol specified.")
+    print_verbose("[!] No protocol specified.")
     url = "http://" + url
-    print("[+] Going with HTTP.\n")
-    print("Checking: " + str(url))
+    print_verbose("[+] Going with HTTP.\n")
+    print_verbose("Checking: " + str(url))
 
     return url
 
 
 def check_redirect(url):
     """Checks if the url redirects to another url, if so, it follows the redirect."""
 
     headers = {'User-Agent': 'Mozilla/5.0'}
     response = requests.head(url, allow_redirects=True,
                              headers=headers, timeout=5)
     redirected_url = response.url
 
     if url != redirected_url:
-        print(f"[!] {url} redirected to {redirected_url}")
+        print_verbose(f"[!] {url} redirected to {redirected_url}")
         # Recursively follow the redirect
         return check_redirect(redirected_url)
 
     return redirected_url
 
 
 def check_http(url):
     """Instead of HTTPS, it tries to connect over HTTP."""
 
-    print("[!] Couldn't connect over HTTPS.")
-    print("[+] Trying with HTTP.\n")
+    print_verbose("[!] Couldn't connect over HTTPS.")
+    print_verbose("[+] Trying with HTTP.\n")
     url = "http://" + url[8:]
-    print("Checking: " + str(url))
+    print_verbose("Checking: " + str(url))
 
     return url
 
 
-def url_check(url, show_signature=False):
+def url_check(url):
     """
         Checks if the url is valid and publicly accessible.
         If so, it runs wp_check on it.
     """
 
-    print("\nChecking: " + str(url))
+    print_verbose("\nChecking: " + str(url))
     try:
         if url[:4] != "http":
             url = check_protocol(url)
 
         url = check_redirect(url)
 
         wp_signatures = {
@@ -108,81 +123,99 @@
         }
 
         # run wp_check for each url in wp_signatures
         for wp_signature in wp_signatures.values():
             result = wp_check(wp_signature)
 
             if result:
-                url_to_print = wp_signature if show_signature else url
+                url_to_print = wp_signature if cli_options["show_signature"] else url
 
-                print(f"[✓] WordPress found at: {url_to_print}")
+                print_verbose(f"[✓] WordPress found at: {url_to_print}")
 
-                wp_domains.append(url)
+                wp_domains.append(url_to_print)
             else:
-                print(f"[✗] WordPress not found at: {url}")
+                print_verbose(f"[✗] WordPress not found at: {url}")
             break
 
     except urllib.error.HTTPError as error:
         if error.code == 403:
-            print("Got 403! Website seems to be behind a WAF.")
+            print_verbose("Got 403! Website seems to be behind a WAF.")
 
     except urllib.error.URLError:
         if url[:5] == "https":
             url = check_http(url)
 
             try:
                 url_check(url)
             except urllib.error.URLError:
-                print(ERROR_UNABLE_TO_OPEN_URL)
+                print_verbose(ERROR_UNABLE_TO_OPEN_URL)
         else:
-            print(ERROR_UNABLE_TO_OPEN_URL)
+            print_verbose(ERROR_UNABLE_TO_OPEN_URL)
     except ValueError:
-        print("Invalid url! Please type in correct url.\n")
+        print_verbose("Invalid url! Please type in correct url.\n")
 
 
-def handle_file(filename, show_signature=False):
+def handle_file(filename):
     """Opens the file and runs url_check for each line."""
 
     try:
         with open(filename, 'r', encoding='utf-8') as file:
             domains = file.readlines()
 
-            print("Targets,\n")
+            print_verbose("Targets,\n")
 
             for domain in domains:
-                print(domain.strip())
+                print_verbose(domain.strip())
 
             for domain in domains:
                 url = domain.strip()
-                url_check(url, show_signature)
+                url_check(url)
 
     except FileNotFoundError:
         print("Please enter the file name correctly, file not found!\n")
 
 
+def print_domains():
+    """Prints the found WordPress installations."""
+
+    if cli_options['verbose'] is False:
+        for wp_domain in wp_domains:
+            print(wp_domain)
+
+
 @click.command(context_settings={"help_option_names": ['-h', '--help']})
 @click.argument('url', required=False)
 @click.option('-f', '--file', type=click.Path(exists=True), help="File with list of URLs to check.")
 @click.option('-v', '--version', is_flag=True, help="Print version.")
 @click.option('-ss', '--show-signature', is_flag=True,
               help="Show by which signature WordPress is detected in a domain.")
-def main(url, file, version, show_signature):
+@click.option('-q', '--quiet', is_flag=True, help="Only print the detected domains.")
+def main(url, file, version, show_signature, quiet):
     """Detects if a website is running WordPress."""
 
+    if quiet:
+        cli_options['verbose'] = False
+
+    if show_signature:
+        cli_options['show_signature'] = True
+
     if version is False:
         print_logo(VERSION)
 
     if url:
-        url_check(url, show_signature)
+        url_check(url)
 
     if file:
-        handle_file(file, show_signature)
+        handle_file(file)
 
     if version:
         print(f"Version: {VERSION}")
 
     if len(sys.argv) == 1:
         click.echo(click.get_current_context().get_help())
 
+    # print wp_domains if verbose is true
+    print_domains()
+
 
 if __name__ == '__main__':
-    main(None, None, None, None)
+    main(None, None, None, None, None)
```

### Comparing `wpdetect-1.4.2/.gitignore` & `wpdetect-1.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.2/LICENSE.txt` & `wpdetect-1.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.2/README.md` & `wpdetect-1.4.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -38,14 +38,18 @@
 http://www.techcrunch.com/
 ```
 
 Please note that, it is not always possible to detect the presence of WordPress, website admins can take extra measures to remove sign of WordPress.
 
 ## Changelog
 
+#### What's new in version 1.4.3
+
+-   Fixed [#20](https://github.com/IamLizu/wpdetect/issues/20)
+
 #### What's new in version 1.4.2
 
 -   Fixed [#18](https://github.com/IamLizu/wpdetect/issues/18)
 
 #### What's new in version 1.4.1
 
 -   Fixed [#10](https://github.com/IamLizu/wpdetect/issues/10)
```

### Comparing `wpdetect-1.4.2/pyproject.toml` & `wpdetect-1.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wpdetect"
-version = "1.4.2"
+version = "1.4.3"
 dependencies = [
     "pyfiglet", "requests", "click"
 ]
 authors = [
   { name="S M Mahmudul Hasan", email="he@smmahmudulhasan.com" },
 ]
 description = "A WordPress detection tool, detects if a website is running WordPress"
```

### Comparing `wpdetect-1.4.2/PKG-INFO` & `wpdetect-1.4.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpdetect
-Version: 1.4.2
+Version: 1.4.3
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
 
+#### What's new in version 1.4.3
+
+-   Fixed [#20](https://github.com/IamLizu/wpdetect/issues/20)
+
 #### What's new in version 1.4.2
 
 -   Fixed [#18](https://github.com/IamLizu/wpdetect/issues/18)
 
 #### What's new in version 1.4.1
 
 -   Fixed [#10](https://github.com/IamLizu/wpdetect/issues/10)
```

