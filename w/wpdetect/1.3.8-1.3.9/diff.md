# Comparing `tmp/wpdetect-1.3.8.tar.gz` & `tmp/wpdetect-1.3.9.tar.gz`

## Comparing `wpdetect-1.3.8.tar` & `wpdetect-1.3.9.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 wpdetect-1.3.8/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.3.8/wpdetect/__init__.py
--rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 wpdetect-1.3.8/wpdetect/__main__.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 wpdetect-1.3.8/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 wpdetect-1.3.8/LICENSE.txt
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 wpdetect-1.3.8/README.md
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 wpdetect-1.3.8/pyproject.toml
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 wpdetect-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 wpdetect-1.3.9/requirements.txt
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 wpdetect-1.3.9/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 wpdetect-1.3.9/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wpdetect-1.3.9/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.3.9/wpdetect/__init__.py
+-rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 wpdetect-1.3.9/wpdetect/__main__.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 wpdetect-1.3.9/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wpdetect-1.3.9/LICENSE.txt
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 wpdetect-1.3.9/README.md
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 wpdetect-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 wpdetect-1.3.9/PKG-INFO
```

### Comparing `wpdetect-1.3.8/LICENSE.txt` & `wpdetect-1.3.9/LICENSE.txt`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2020 S M Mahmudul Hasan
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright 2020 S M Mahmudul Hasan
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `wpdetect-1.3.8/README.md` & `wpdetect-1.3.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,62 @@
-# WP DETECT
-
-A WordPress detection tool, detects if a website is running WordPress. wpdetect is a great tool when you just want to check WordPress' presence but do not want to scan the site for vulnerabilities or issues.
-
-## Installation
-
-You can install wpdetect using pip,
-
-```sh
-pip install wpdetect
-```
-
-wpdetect requires Python 3 or above to run. If you have Python 2 installed too, make sure to use the right pip.
-
-## Usage
-
-```sh
-wpdetect <website_url>
-```
-
-Example
-
-```sh
-wpdetect https://wordpress.org
-```
-
-Or feed a text file with a list of domains, each domain should be separated with new lines.
-
-```sh
-wpdetect -f sites.txt
-```
-
-Where `sites.txt` will contain domains like this,
-
-```sh
-https://wordpress.org
-https://www.newyorker.com/
-http://www.techcrunch.com/
-```
-
-Please note that, it is not always possible to detect the presence of WordPress, website admins can take extra measures to remove sign of WordPress.
-
-## Changelog
-
-#### What's new in version 1.3.8
-
--   Fixed [#8](https://github.com/IamLizu/wpdetect/issues)
-
-#### What's new in version 1.3.7
-
--   Migrated to Hatchling build system
--   Updated README
-
-#### What's new in version 1.3.6
-
--   Fixed minor bugs
+# WP DETECT
+
+A WordPress detection tool, detects if a website is running WordPress. wpdetect is a great tool when you just want to check WordPress' presence but do not want to scan the site for vulnerabilities or issues.
+
+## Installation
+
+You can install wpdetect using pip,
+
+```sh
+pip install wpdetect
+```
+
+wpdetect requires Python 3 or above to run. If you have Python 2 installed too, make sure to use the right pip.
+
+## Usage
+
+```sh
+wpdetect <website_url>
+```
+
+Example
+
+```sh
+wpdetect https://wordpress.org
+```
+
+Or feed a text file with a list of domains, each domain should be separated with new lines.
+
+```sh
+wpdetect -f sites.txt
+```
+
+Where `sites.txt` will contain domains like this,
+
+```sh
+https://wordpress.org
+https://www.newyorker.com/
+http://www.techcrunch.com/
+```
+
+Please note that, it is not always possible to detect the presence of WordPress, website admins can take extra measures to remove sign of WordPress.
+
+## Changelog
+
+#### What's new in version 1.3.9
+
+-   Minor bug fixes
+-   Added workflow for linting on code push
+-   Added workflow for publishing to PyPi on release
+
+#### What's new in version 1.3.8
+
+-   Fixed [#8](https://github.com/IamLizu/wpdetect/issues/8)
+
+#### What's new in version 1.3.7
+
+-   Migrated to Hatchling build system
+-   Updated README
+
+#### What's new in version 1.3.6
+
+-   Fixed minor bugs
```

### Comparing `wpdetect-1.3.8/pyproject.toml` & `wpdetect-1.3.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "wpdetect"
-version = "1.3.8"
-dependencies = [
-    "pyfiglet", "requests"
-]
-authors = [
-  { name="S M Mahmudul Hasan", email="thegeek@iamlizu.com" },
-]
-description = "A WordPress detection tool, detects if a website is running WordPress"
-readme = "README.md"
-requires-python = ">=3.4"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    'Development Status :: 5 - Production/Stable',
-    'Topic :: Software Development :: Build Tools',
-    'Intended Audience :: Developers',
-]
-
-[project.urls]
-"Homepage" = "https://github.com/IamLizu/wpdetect"
-"Bug Tracker" = "https://github.com/IamLizu/wpdetect/issues"
-
-[project.scripts]
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "wpdetect"
+version = "1.3.9"
+dependencies = [
+    "pyfiglet", "requests"
+]
+authors = [
+  { name="S M Mahmudul Hasan", email="he@smmahmudulhasan.com" },
+]
+description = "A WordPress detection tool, detects if a website is running WordPress"
+readme = "README.md"
+requires-python = ">=3.4"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    'Development Status :: 5 - Production/Stable',
+    'Topic :: Software Development :: Build Tools',
+    'Intended Audience :: Developers',
+]
+
+[project.urls]
+"Homepage" = "https://github.com/IamLizu/wpdetect"
+"Bug Tracker" = "https://github.com/IamLizu/wpdetect/issues"
+
+[project.scripts]
 wpdetect = "wpdetect.__main__:main"
```

### Comparing `wpdetect-1.3.8/PKG-INFO` & `wpdetect-1.3.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: wpdetect
-Version: 1.3.8
+Version: 1.3.9
 Summary: A WordPress detection tool, detects if a website is running WordPress
 Project-URL: Homepage, https://github.com/IamLizu/wpdetect
 Project-URL: Bug Tracker, https://github.com/IamLizu/wpdetect/issues
-Author-email: S M Mahmudul Hasan <thegeek@iamlizu.com>
+Author-email: S M Mahmudul Hasan <he@smmahmudulhasan.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Build Tools
@@ -57,17 +57,23 @@
 http://www.techcrunch.com/
 ```
 
 Please note that, it is not always possible to detect the presence of WordPress, website admins can take extra measures to remove sign of WordPress.
 
 ## Changelog
 
+#### What's new in version 1.3.9
+
+-   Minor bug fixes
+-   Added workflow for linting on code push
+-   Added workflow for publishing to PyPi on release
+
 #### What's new in version 1.3.8
 
--   Fixed [#8](https://github.com/IamLizu/wpdetect/issues)
+-   Fixed [#8](https://github.com/IamLizu/wpdetect/issues/8)
 
 #### What's new in version 1.3.7
 
 -   Migrated to Hatchling build system
 -   Updated README
 
 #### What's new in version 1.3.6
```

