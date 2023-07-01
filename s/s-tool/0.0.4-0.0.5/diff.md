# Comparing `tmp/s_tool-0.0.4.tar.gz` & `tmp/s_tool-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s_tool-0.0.4.tar", max compression
+gzip compressed data, was "s_tool-0.0.5.tar", max compression
```

## Comparing `s_tool-0.0.4.tar` & `s_tool-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-06-04 18:38:21.227674 s_tool-0.0.4/LICENSE
--rw-r--r--   0        0        0     3682 2023-06-04 18:38:21.227674 s_tool-0.0.4/README.rst
--rw-r--r--   0        0        0     1488 2023-06-04 18:38:21.227674 s_tool-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      187 2023-06-04 18:38:21.227674 s_tool-0.0.4/s_tool/__init__.py
--rw-r--r--   0        0        0    28280 2023-06-04 18:38:21.227674 s_tool-0.0.4/s_tool/core.py
--rw-r--r--   0        0        0     2407 2023-06-04 18:38:21.227674 s_tool-0.0.4/s_tool/driver.py
--rw-r--r--   0        0        0      537 2023-06-04 18:38:21.227674 s_tool-0.0.4/s_tool/exceptions.py
--rw-r--r--   0        0        0       95 2023-06-04 18:38:21.227674 s_tool-0.0.4/s_tool/logger.py
--rw-r--r--   0        0        0     1334 2023-06-04 18:38:21.227674 s_tool-0.0.4/s_tool/parser.py
--rw-r--r--   0        0        0     4655 1970-01-01 00:00:00.000000 s_tool-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-01 19:59:08.136328 s_tool-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3679 2023-07-01 19:59:08.136328 s_tool-0.0.5/README.rst
+-rw-r--r--   0        0        0     1488 2023-07-01 19:59:08.136328 s_tool-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      187 2023-07-01 19:59:08.136328 s_tool-0.0.5/s_tool/__init__.py
+-rw-r--r--   0        0        0    28406 2023-07-01 19:59:08.136328 s_tool-0.0.5/s_tool/core.py
+-rw-r--r--   0        0        0     2407 2023-07-01 19:59:08.136328 s_tool-0.0.5/s_tool/driver.py
+-rw-r--r--   0        0        0      537 2023-07-01 19:59:08.136328 s_tool-0.0.5/s_tool/exceptions.py
+-rw-r--r--   0        0        0       95 2023-07-01 19:59:08.136328 s_tool-0.0.5/s_tool/logger.py
+-rw-r--r--   0        0        0     1334 2023-07-01 19:59:08.136328 s_tool-0.0.5/s_tool/parser.py
+-rw-r--r--   0        0        0     4652 1970-01-01 00:00:00.000000 s_tool-0.0.5/PKG-INFO
```

### Comparing `s_tool-0.0.4/LICENSE` & `s_tool-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `s_tool-0.0.4/README.rst` & `s_tool-0.0.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -40,27 +40,27 @@
 Usage
 ^^^^^
 
 * Example Using Context Manager
 
 .. code-block:: python
 
-      """Example code with context manager"""
+    """Example code with context manager"""
 
-      from s_tool.core import SeleniumDriver as SBot
-
-      with SBot("firefox", headless=True) as self:
-          self.get("https://google.com")
-          sessionid = self.session()
-          url = self.url()
-          cookies = self.cookies()
-
-          # print sessionid,url,cookies
-          print(f"\nurl     :   {url} \nsession :   {sessionid}\ncookies :   {cookies}\n")
+    from s_tool.core import SeleniumTools as SBot
 
+    with SBot(browser="firefox", headless=True) as self:
+        self.get("https://example.com")
+        sessionid = self.sessionid()
+        url = self.url()
+        cookies = self.cookies()
+
+        # print sessionid,url,cookies
+        print(f"\nurl     :   {url} \nsession :   {sessionid}\ncookies :   {cookies}\n")
+     
 
 * Example Using class
 
 .. code-block:: python 
 
     from s_tool.core import SeleniumTools
 
@@ -80,16 +80,15 @@
 
             # print sessionid,url,cookies
             print(f"\nurl     :   {url} \nsession :   {sessionid}\ncookies :   {cookies}\n")
 
 
     bot = SBot(browser ="firefox", headless=True)  # change headless=False to run with gui mode
     bot.run()
-    bot.close()
-
+    bot._close()
 
 Methods
 ^^^^^^^
 
 Here are the public methods available in the SeleniumTools class:
     - get(): Loads a web page with the specified URL or local file or Html Content.
     - url(): Returns the current URL of the page.
```

### Comparing `s_tool-0.0.4/pyproject.toml` & `s_tool-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "s-tool"
-version = "0.0.4"
+version = "0.0.5"
 description = "Selenium wrapper to make your life easy."
 authors = ["Ravishankar Chavare <chavare.ravi123@gmail.com>", "Aahnik Daw <daw@aahnik.dev>"]
 packages = [{include = "s_tool"}]
 
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/Python-World/s-tool"
```

### Comparing `s_tool-0.0.4/s_tool/core.py` & `s_tool-0.0.5/s_tool/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,17 @@
             self.driver = self._load_driver()
             logger.info('selenium driver object created')
 
         return self
 
     def _load_driver(self):
         """Create Selenium webdriver object"""
+        if self.browser is None:
+            self.browser='chrome'
+
         obj = SeleniumDriver(browser=self.browser,
                              headless=self.headless,
                              executable_path=self.executable_path)
         self.driver = obj.load_driver()
 
         return self.driver
 
@@ -200,14 +203,17 @@
 
             # Validate the driver
             selenium_tools._validate_driver()
         """
         err = "Selenium WebDriver validation failed."
         supported_browsers = self._get_supported_browsers()
 
+        if self.driver is None:
+            return False
+
         if hasattr(
                 self.driver,
                 'name') and self.driver.name not in supported_browsers:
 
             return False
 
         try:
```

### Comparing `s_tool-0.0.4/s_tool/driver.py` & `s_tool-0.0.5/s_tool/driver.py`

 * *Files identical despite different names*

### Comparing `s_tool-0.0.4/s_tool/exceptions.py` & `s_tool-0.0.5/s_tool/exceptions.py`

 * *Files identical despite different names*

### Comparing `s_tool-0.0.4/s_tool/parser.py` & `s_tool-0.0.5/s_tool/parser.py`

 * *Files identical despite different names*

### Comparing `s_tool-0.0.4/PKG-INFO` & `s_tool-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s-tool
-Version: 0.0.4
+Version: 0.0.5
 Summary: Selenium wrapper to make your life easy.
 Home-page: https://github.com/Python-World/s-tool
 License: MIT
 Keywords: Python,Selenium,wrapper,Webdriver,Tools,Utilities
 Author: Ravishankar Chavare
 Author-email: chavare.ravi123@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -65,27 +65,27 @@
 Usage
 ^^^^^
 
 * Example Using Context Manager
 
 .. code-block:: python
 
-      """Example code with context manager"""
+    """Example code with context manager"""
 
-      from s_tool.core import SeleniumDriver as SBot
-
-      with SBot("firefox", headless=True) as self:
-          self.get("https://google.com")
-          sessionid = self.session()
-          url = self.url()
-          cookies = self.cookies()
-
-          # print sessionid,url,cookies
-          print(f"\nurl     :   {url} \nsession :   {sessionid}\ncookies :   {cookies}\n")
+    from s_tool.core import SeleniumTools as SBot
 
+    with SBot(browser="firefox", headless=True) as self:
+        self.get("https://example.com")
+        sessionid = self.sessionid()
+        url = self.url()
+        cookies = self.cookies()
+
+        # print sessionid,url,cookies
+        print(f"\nurl     :   {url} \nsession :   {sessionid}\ncookies :   {cookies}\n")
+     
 
 * Example Using class
 
 .. code-block:: python 
 
     from s_tool.core import SeleniumTools
 
@@ -105,16 +105,15 @@
 
             # print sessionid,url,cookies
             print(f"\nurl     :   {url} \nsession :   {sessionid}\ncookies :   {cookies}\n")
 
 
     bot = SBot(browser ="firefox", headless=True)  # change headless=False to run with gui mode
     bot.run()
-    bot.close()
-
+    bot._close()
 
 Methods
 ^^^^^^^
 
 Here are the public methods available in the SeleniumTools class:
     - get(): Loads a web page with the specified URL or local file or Html Content.
     - url(): Returns the current URL of the page.
```

