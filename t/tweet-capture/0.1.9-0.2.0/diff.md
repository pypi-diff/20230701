# Comparing `tmp/tweet-capture-0.1.9.tar.gz` & `tmp/tweet-capture-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweet-capture-0.1.9.tar", last modified: Wed Apr 12 20:01:41 2023, max compression
+gzip compressed data, was "tweet-capture-0.2.0.tar", last modified: Sat Jul  1 21:44:15 2023, max compression
```

## Comparing `tweet-capture-0.1.9.tar` & `tweet-capture-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 20:01:41.669123 tweet-capture-0.1.9/
--rw-rw-rw-   0        0        0     1085 2021-05-31 19:56:28.000000 tweet-capture-0.1.9/LICENSE
--rw-rw-rw-   0        0        0     3238 2023-04-12 20:01:41.669826 tweet-capture-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     2656 2023-04-06 14:53:44.000000 tweet-capture-0.1.9/README.md
--rw-rw-rw-   0        0        0       67 2023-04-06 14:53:44.000000 tweet-capture-0.1.9/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-04-12 20:01:41.670576 tweet-capture-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1180 2023-04-12 19:53:24.000000 tweet-capture-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 20:01:41.660557 tweet-capture-0.1.9/tweet_capture.egg-info/
--rw-rw-rw-   0        0        0     3238 2023-04-12 20:01:41.000000 tweet-capture-0.1.9/tweet_capture.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2023-04-12 20:01:41.000000 tweet-capture-0.1.9/tweet_capture.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 20:01:41.000000 tweet-capture-0.1.9/tweet_capture.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-12 20:01:41.000000 tweet-capture-0.1.9/tweet_capture.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       65 2023-04-12 20:01:41.000000 tweet-capture-0.1.9/tweet_capture.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-12 20:01:41.000000 tweet-capture-0.1.9/tweet_capture.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 20:01:41.664305 tweet-capture-0.1.9/tweetcapture/
--rw-rw-rw-   0        0        0       60 2021-05-31 18:34:46.000000 tweet-capture-0.1.9/tweetcapture/__init__.py
--rw-rw-rw-   0        0        0     3502 2023-04-06 14:53:44.000000 tweet-capture-0.1.9/tweetcapture/cli.py
--rw-rw-rw-   0        0        0    13816 2023-04-06 14:53:44.000000 tweet-capture-0.1.9/tweetcapture/screenshot.py
-drwxrwxrwx   0        0        0        0 2023-04-12 20:01:41.668054 tweet-capture-0.1.9/tweetcapture/utils/
--rw-rw-rw-   0        0        0        0 2021-05-31 19:53:06.000000 tweet-capture-0.1.9/tweetcapture/utils/__init__.py
--rw-rw-rw-   0        0        0     1831 2023-04-06 13:06:19.000000 tweet-capture-0.1.9/tweetcapture/utils/utils.py
--rw-rw-rw-   0        0        0     2302 2023-04-06 14:53:44.000000 tweet-capture-0.1.9/tweetcapture/utils/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:44:15.883343 tweet-capture-0.2.0/
+-rw-rw-rw-   0        0        0     1085 2021-05-31 19:56:28.000000 tweet-capture-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3238 2023-07-01 21:44:15.883343 tweet-capture-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2656 2023-04-06 14:53:44.000000 tweet-capture-0.2.0/README.md
+-rw-rw-rw-   0        0        0       67 2023-04-06 14:53:44.000000 tweet-capture-0.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-07-01 21:44:15.885334 tweet-capture-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1180 2023-07-01 21:00:35.000000 tweet-capture-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:44:15.870208 tweet-capture-0.2.0/tweet_capture.egg-info/
+-rw-rw-rw-   0        0        0     3238 2023-07-01 21:44:15.000000 tweet-capture-0.2.0/tweet_capture.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-07-01 21:44:15.000000 tweet-capture-0.2.0/tweet_capture.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 21:44:15.000000 tweet-capture-0.2.0/tweet_capture.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-01 21:44:15.000000 tweet-capture-0.2.0/tweet_capture.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       65 2023-07-01 21:44:15.000000 tweet-capture-0.2.0/tweet_capture.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-01 21:44:15.000000 tweet-capture-0.2.0/tweet_capture.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 21:44:15.876206 tweet-capture-0.2.0/tweetcapture/
+-rw-rw-rw-   0        0        0       60 2021-05-31 18:34:46.000000 tweet-capture-0.2.0/tweetcapture/__init__.py
+-rw-rw-rw-   0        0        0     4019 2023-07-01 20:57:26.000000 tweet-capture-0.2.0/tweetcapture/cli.py
+-rw-rw-rw-   0        0        0    14403 2023-07-01 21:12:57.000000 tweet-capture-0.2.0/tweetcapture/screenshot.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:44:15.882341 tweet-capture-0.2.0/tweetcapture/utils/
+-rw-rw-rw-   0        0        0        0 2021-05-31 19:53:06.000000 tweet-capture-0.2.0/tweetcapture/utils/__init__.py
+-rw-rw-rw-   0        0        0     1831 2023-04-06 13:06:19.000000 tweet-capture-0.2.0/tweetcapture/utils/utils.py
+-rw-rw-rw-   0        0        0     2302 2023-07-01 20:41:47.000000 tweet-capture-0.2.0/tweetcapture/utils/webdriver.py
```

### Comparing `tweet-capture-0.1.9/LICENSE` & `tweet-capture-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tweet-capture-0.1.9/PKG-INFO` & `tweet-capture-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweet-capture
-Version: 0.1.9
+Version: 0.2.0
 Summary: Take a tweet screenshot
 Home-page: https://github.com/Xacnio/tweetcapture
 Author: Alperen Çetin
 Author-email: xacnio@pm.me
 License: MIT
 Keywords: tweet screenshot
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `tweet-capture-0.1.9/README.md` & `tweet-capture-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tweet-capture-0.1.9/setup.py` & `tweet-capture-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     with open('requirements.txt', 'r') as f:
         requirements = f.read().splitlines()
         return requirements
 
 
 setuptools.setup(
     name="tweet-capture",
-    version="0.1.9",
+    version="0.2.0",
     author="Alperen Çetin",
     author_email="xacnio@pm.me",
     description="Take a tweet screenshot",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Xacnio/tweetcapture",
     packages=setuptools.find_packages(),
```

### Comparing `tweet-capture-0.1.9/tweet_capture.egg-info/PKG-INFO` & `tweet-capture-0.2.0/tweet_capture.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweet-capture
-Version: 0.1.9
+Version: 0.2.0
 Summary: Take a tweet screenshot
 Home-page: https://github.com/Xacnio/tweetcapture
 Author: Alperen Çetin
 Author-email: xacnio@pm.me
 License: MIT
 Keywords: tweet screenshot
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `tweet-capture-0.1.9/tweetcapture/cli.py` & `tweet-capture-0.2.0/tweetcapture/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     parser.add_argument('-hq', '--hide-quotes', dest='hide_tweet_quotes', action='store_true', help="Hide tweet quotes")
     parser.add_argument('-hlp', '--hide-link-previews', dest='hide_tweet_link_previews', action='store_true', help="Hide tweet link previews")
     parser.add_argument('-ha', '--hide-all', dest='hide_all_tweet_medias', action='store_true', help="Hide all tweet medias")
     
     parser.add_argument('--overwrite', dest='overwrite', action='store_true', help="Overwrite output file if exists")
     parser.add_argument('-d', '--debug', dest='debug', action='store_true', help="Debug mode")
     parser.add_argument('--gui', dest='gui', action='store_true', help="GUI mode, open browser window")
+    parser.add_argument('--cookies', type=str, help="Set cookies cookie1=value1;cookie2=value2", default="")
     parser.set_defaults(show_parent_tweets=False, overwrite=False, debug=False, gui=False, hide_tweet_photos=False, hide_tweet_videos=False, hide_tweet_gifs=False, hide_tweet_quotes=False, hide_tweet_link_previews=False, hide_all_tweet_medias=False)
 
     args = parser.parse_args()
     return args
 
 
 def main():
@@ -40,14 +41,26 @@
     if args.hide_all_tweet_medias is True: 
         tweet.hide_all_media()
     else: 
         tweet.hide_media(args.hide_tweet_link_previews, args.hide_tweet_photos, args.hide_tweet_videos, args.hide_tweet_gifs, args.hide_tweet_quotes)
     tweet.set_gui(args.gui)
     if len(args.chromedriver) > 0:
         tweet.set_chromedriver_path(args.chromedriver)
+
+    if len(args.cookies) > 0:
+        cookies = []
+        splitted = args.cookies.split(";")
+        if len(splitted) >= 1:
+            for cookie in splitted:
+                cookie = cookie.split("=")
+                if len(cookie) == 2:
+                    cookies.append({'name': cookie[0], 'value': cookie[1]})
+            if len(cookies) > 0:
+                tweet.set_cookies(cookies)
+
     try:
         filename = run(tweet.screenshot(args.url, args.output))
         print(f"Screenshot is saved: {filename}")
     except Exception as error:
         if args.debug:
             traceback.print_exc()
         else:
```

### Comparing `tweet-capture-0.1.9/tweetcapture/screenshot.py` & `tweet-capture-0.2.0/tweetcapture/screenshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from asyncio import sleep
 from tweetcapture.utils.webdriver import get_driver
 from tweetcapture.utils.utils import is_valid_tweet_url, get_tweet_file_name, add_corners
 from selenium.webdriver.common.by import By
 from PIL import Image
-from os import remove
+from os import remove, environ
 from os.path import exists
 
 class TweetCapture:
     driver = None
     driver_path = None
     gui = False
     mode = 3
@@ -16,14 +16,15 @@
     chrome_opts = []
     lang = None
     test = False
     show_parent_tweets = False
     show_mentions_count = 0
     overwrite = False
     radius = 15
+    cookies = None
 
     hide_link_previews = False
     hide_photos = False
     hide_videos = False
     hide_gifs = False
     hide_quotes = False
 
@@ -33,38 +34,45 @@
         self.set_night_mode(night_mode)
         self.set_mode(mode)
         self.test = test
         self.show_parent_tweets = show_parent_tweets
         self.show_mentions_count = show_mentions_count
         self.overwrite = overwrite
         self.radius = radius
+        if environ.get('AUTH_TOKEN') != None:
+            self.cookies = [{'name': 'auth_token', 'value': environ.get('AUTH_TOKEN')}]
 
     async def screenshot(self, url, path=None, mode=None, night_mode=None, show_parent_tweets=None, show_mentions_count=None, overwrite=None, radius=None):
         if is_valid_tweet_url(url) is False:
             raise Exception("Invalid tweet url")
 
         if not isinstance(path, str) or len(path) == 0:
             path = get_tweet_file_name(url)
 
-        if exists(path) and (self.overwrite if overwrite is None else overwrite) is False:
-            raise Exception("File already exists")
+        if exists(path):
+            if (self.overwrite if overwrite is None else overwrite) is False:
+                raise Exception("File already exists")
+            else:
+                remove(path)
 
         url = is_valid_tweet_url(url)
         if self.lang:
             url += "?lang=" + self.lang
 
-            
         radius = self.radius if radius is None else radius
         driver = await get_driver(self.chrome_opts, self.driver_path, self.gui)
         if driver is None:
             raise Exception("webdriver cannot be initialized")
         try:
             driver.get(url)
             driver.add_cookie(
                 {"name": "night_mode", "value": str(self.night_mode if night_mode is None else night_mode)})
+            if self.cookies:
+                for cookie in self.cookies:
+                    driver.add_cookie(cookie)
             driver.get(url)
             await sleep(self.wait_time)
            
             self.__hide_global_items(driver)
             driver.execute_script("!!document.activeElement ? document.activeElement.blur() : 0")
 
             if self.test is True: 
@@ -153,18 +161,25 @@
         self.chrome_opts.append(option)
 
     def set_lang(self, lang):
         self.lang = lang
 
     def set_chromedriver_path(self, path):
         self.driver_path = path
+    
+    def set_cookies(self, cookies):
+        if isinstance(cookies, list):
+            self.cookies = cookies
 
     def __hide_global_items(self, driver):
-        HIDE_ITEMS_XPATH = ['/html/body/div/div/div/div[1]',
-        '/html/body/div/div/div/div[2]/header', '/html/body/div/div/div/div[2]/main/div/div/div/div/div/div[1]']
+        HIDE_ITEMS_XPATH = [
+            '/html/body/div/div/div/div[1]',
+            '/html/body/div/div/div/div[2]/header', '/html/body/div/div/div/div[2]/main/div/div/div/div/div/div[1]',
+            ".//ancestor::div[@data-testid = 'tweetButtonInline']/../../../../../../../../../../.."
+        ]
         for item in HIDE_ITEMS_XPATH:
             try:
                 element = driver.find_element(By.XPATH, item)
                 driver.execute_script("""
                 arguments[0].style.display="none";
                 """, element)
             except:
```

### Comparing `tweet-capture-0.1.9/tweetcapture/utils/utils.py` & `tweet-capture-0.2.0/tweetcapture/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tweet-capture-0.1.9/tweetcapture/utils/webdriver.py` & `tweet-capture-0.2.0/tweetcapture/utils/webdriver.py`

 * *Files identical despite different names*

