# Comparing `tmp/bose-1.8.1.tar.gz` & `tmp/bose-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bose-1.8.1.tar", last modified: Wed Jun 14 13:00:11 2023, max compression
+gzip compressed data, was "bose-2.0.0.tar", last modified: Sat Jul  1 12:04:34 2023, max compression
```

## Comparing `bose-1.8.1.tar` & `bose-2.0.0.tar`

### file list

```diff
@@ -1,25 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 13:00:11.015886 bose-1.8.1/
--rw-rw-rw-   0        0        0    14240 2023-06-14 13:00:11.015886 bose-1.8.1/PKG-INFO
--rw-rw-rw-   0        0        0    10461 2023-05-24 16:36:27.405231 bose-1.8.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-14 13:00:11.015886 bose-1.8.1/bose/
--rw-rw-rw-   0        0        0      342 2023-06-14 07:55:53.180015 bose-1.8.1/bose/__init__.py
--rw-rw-rw-   0        0        0     3200 2023-06-14 12:56:17.167308 bose-1.8.1/bose/account_generator.py
--rw-rw-rw-   0        0        0      652 2023-05-25 17:01:27.624054 bose-1.8.1/bose/analytics.py
--rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-1.8.1/bose/base_data.py
--rw-rw-rw-   0        0        0     5070 2023-06-13 16:14:19.186655 bose-1.8.1/bose/base_task.py
--rw-rw-rw-   0        0        0     9039 2023-06-13 16:14:04.846297 bose-1.8.1/bose/bose_driver.py
--rw-rw-rw-   0        0        0     9051 2023-06-13 16:14:04.846297 bose-1.8.1/bose/bose_undetected_driver.py
--rw-rw-rw-   0        0        0     7295 2023-06-13 16:14:19.186655 bose-1.8.1/bose/create_driver.py
--rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-1.8.1/bose/download_driver.py
--rw-rw-rw-   0        0        0     3185 2023-05-18 07:50:25.651854 bose-1.8.1/bose/local_storage.py
--rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-1.8.1/bose/local_storage_driver.py
--rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-1.8.1/bose/opponent.py
--rw-rw-rw-   0        0        0     3187 2023-05-15 09:11:34.318135 bose-1.8.1/bose/output.py
--rw-rw-rw-   0        0        0     1650 2023-05-13 11:28:17.687091 bose-1.8.1/bose/task_info.py
--rw-rw-rw-   0        0        0     5433 2023-06-14 07:47:40.744829 bose-1.8.1/bose/temp_mail.py
--rw-rw-rw-   0        0        0     7361 2023-05-10 09:24:37.900794 bose-1.8.1/bose/user_agent.py
--rw-rw-rw-   0        0        0     6050 2023-05-10 10:34:20.625623 bose-1.8.1/bose/utils.py
--rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-1.8.1/bose/wait.py
--rw-rw-rw-   0        0        0     1203 2023-05-09 07:09:28.075948 bose-1.8.1/bose/window_size.py
--rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-1.8.1/setup.cfg
--rw-rw-rw-   0        0        0     2336 2023-06-14 12:59:51.493882 bose-1.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 12:04:34.322560 bose-2.0.0/
+-rw-rw-rw-   0        0        0    14240 2023-07-01 12:04:34.323560 bose-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10461 2023-05-24 16:36:27.405231 bose-2.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-01 12:04:34.322560 bose-2.0.0/bose/
+-rw-rw-rw-   0        0        0      452 2023-06-30 14:14:28.791702 bose-2.0.0/bose/__init__.py
+-rw-rw-rw-   0        0        0     4160 2023-07-01 09:12:23.121716 bose-2.0.0/bose/account_generator.py
+-rw-rw-rw-   0        0        0      707 2023-06-30 05:04:43.924597 bose-2.0.0/bose/analytics.py
+-rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-2.0.0/bose/base_data.py
+-rw-rw-rw-   0        0        0     8291 2023-07-01 09:14:35.292128 bose-2.0.0/bose/base_task.py
+-rw-rw-rw-   0        0        0      317 2023-06-29 11:53:16.211079 bose-2.0.0/bose/beep_utils.py
+-rw-rw-rw-   0        0        0     9954 2023-07-01 09:15:52.186941 bose-2.0.0/bose/bose_driver.py
+-rw-rw-rw-   0        0        0     9966 2023-07-01 09:15:52.186941 bose-2.0.0/bose/bose_undetected_driver.py
+-rw-rw-rw-   0        0        0     7700 2023-06-29 13:46:50.340921 bose-2.0.0/bose/create_driver.py
+-rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-2.0.0/bose/download_driver.py
+-rw-rw-rw-   0        0        0      948 2023-06-30 07:55:50.167685 bose-2.0.0/bose/ip_utils.py
+-rw-rw-rw-   0        0        0     2953 2023-06-30 15:33:26.223178 bose-2.0.0/bose/launch_tasks.py
+-rw-rw-rw-   0        0        0     3185 2023-06-29 08:54:46.918966 bose-2.0.0/bose/local_storage.py
+-rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-2.0.0/bose/local_storage_driver.py
+-rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-2.0.0/bose/opponent.py
+-rw-rw-rw-   0        0        0     2510 2023-07-01 09:16:40.175639 bose-2.0.0/bose/output.py
+-rw-rw-rw-   0        0        0     4600 2023-07-01 06:42:54.180748 bose-2.0.0/bose/profile.py
+-rw-rw-rw-   0        0        0      853 2023-06-29 11:00:24.518432 bose-2.0.0/bose/schedule_utils.py
+-rw-rw-rw-   0        0        0      460 2023-06-29 10:04:53.656427 bose-2.0.0/bose/task_config.py
+-rw-rw-rw-   0        0        0     1375 2023-07-01 09:14:29.721606 bose-2.0.0/bose/task_info.py
+-rw-rw-rw-   0        0        0     5429 2023-06-26 10:10:30.768354 bose-2.0.0/bose/temp_mail.py
+-rw-rw-rw-   0        0        0     7361 2023-05-10 09:24:37.900794 bose-2.0.0/bose/user_agent.py
+-rw-rw-rw-   0        0        0     6210 2023-07-01 09:18:35.128413 bose-2.0.0/bose/utils.py
+-rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-2.0.0/bose/wait.py
+-rw-rw-rw-   0        0        0     1203 2023-05-09 07:09:28.075948 bose-2.0.0/bose/window_size.py
+-rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     2312 2023-07-01 09:18:35.128413 bose-2.0.0/setup.py
```

### Comparing `bose-1.8.1/PKG-INFO` & `bose-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bose
-Version: 1.8.1
+Version: 2.0.0
 Summary: The Ultimate Web Scraping Framework
 Home-page: UNKNOWN
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Description: 🚀 Introducing ✨ Bose Framework - The Swiss Army Knife for Bot Developers 🤖
         =============================================================================
```

### Comparing `bose-1.8.1/README.rst` & `bose-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `bose-1.8.1/bose/account_generator.py` & `bose-2.0.0/bose/account_generator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,29 @@
+import string
 import requests
-import enum
 import random
-
 from .temp_mail import TempMail
+from .utils import merge_list_of_dicts, merge_dicts_in_one_dict
+
+from datetime import datetime
+
+def convert_timestamp(timestamp):
+    dt = datetime.strptime(timestamp, "%Y-%m-%dT%H:%M:%S.%fZ")
+    year = dt.year
+    month = dt.month
+    day = dt.day
+    return {"year": year, "month": month, "day": day}
 
-# from greatawesomeutils.lang import *
 
-class Gender(enum.Enum):
+class Gender():
     MEN = 'male'
     BOTH = ''
     WOMEN = 'female'
 
-class Country(enum.Enum):
+class Country():
     AU = 'AU'
     BR = 'BR'
     CA = 'CA'
     CH = 'CH'
     DE = 'DE'
     DK = 'DK'
     ES = 'ES'
@@ -33,18 +41,34 @@
     TR = 'TR'
     UA = 'UA'
     US = 'US'
 class ProblemWithGetPersonData(Exception):
     """Problem with obtaining personal data"""
 
 
-def process_password(word):
+def get_missing_chars(word:str):
+    missing_chars = []
+    
+    if not any(char.isupper() for char in word):
+        missing_chars.append(random.choice(string.ascii_uppercase))
+    
+    if not any(char.islower() for char in word):
+        missing_chars.append(random.choice(string.ascii_lowercase))
+    
     if not any(char.isdigit() for char in word):
-        # Append '1' to the word if no number is found
-        word += str(random.randint(10 ** (1 - 1), (10 ** 1) - 1))
+        missing_chars.append(random.choice(string.digits))
+    
+    if not any(char in string.punctuation for char in word):
+        missing_chars.append(random.choice(string.punctuation))
+    
+    random.shuffle(missing_chars)
+    return ''.join(missing_chars)
+
+def process_password(word):
+    word = word + get_missing_chars(word)
 
     if len(word) < 8:
         digits_needed = 8 - len(word)
         
         # Generate a random number with the required number of digits
         random_number = random.randint(10 ** (digits_needed - 1), (10 ** digits_needed) - 1)
         
@@ -53,58 +77,66 @@
 
 
     return word
 
 def __get_person(user_data: dict):
     email = user_data["email"]
     
+    dob = convert_timestamp(user_data["dob"]["date"])
+
+    username = user_data["email"].replace("@example.com" , "").replace(".", "") + str(dob['year'])
     
-    username = user_data["email"].replace("@example.com" , "").replace(".", "")
-    
-    email_username = user_data["email"].replace("@example.com" , "")
-    email = TempMail.generate_email(email_username)
+    email = TempMail.generate_email(username)
 
     address = str(user_data["location"]["street"]["number"]) + ", " + user_data["location"]["street"]["name"] + ", " + user_data["location"]["city"] + ", " +user_data["location"]["state"] +  ", " + user_data["location"]["country"] 
 
+    
     return {
      "name": user_data["name"]["first"] + " " + user_data["name"]["last"], 
+     "first_name": user_data["name"]["first"],
+     "last_name": user_data["name"]["last"],
      "username": username, 
      "email": email,
      "password":process_password(user_data["login"]["password"]),
+     "uuid": user_data["login"]["uuid"], 
      "profile_picture" : user_data["picture"]["large"], 
      "phone" : user_data["phone"],
      "address" : address,
      "gender":user_data["gender"],    
      "country": user_data["nat"],
-     "dob" : user_data["dob"]
+     "dob" : merge_dicts_in_one_dict(dob, user_data["dob"]) , 
+    #  "created_at" : datetime_to_str(datetime.now())
     }
 
 
 
 def generate_persons(count: int, gender: Gender = Gender.BOTH, country: Country = None):
 
     if not isinstance(count, int) or count < 1:
         count = 1
 
-    params = {'gender': gender.value, 'results': count}
+    params = {'gender': gender, 'results': count}
     if country is not None:
-         params['nat'] = country.value
+         params['nat'] = country
     
     r = requests.get('https://randomuser.me/api', params=params)
     if r.status_code != 200:
         raise ProblemWithGetPersonData()
 
-    return [__get_person(data) for data in r.json()['results']]
+    results = r.json()['results']
+
+    final = [__get_person(data) for data in results]
+
+    ids =  [{"id":  1 + i } for i in range(len(results))]
+    
+    datas = merge_list_of_dicts(  ids, final)
+    
+    return datas
 
 
 
 class AccountGenerator:
     def generate_account(gender: Gender = Gender.BOTH, country: Country = None):
             return generate_persons(1, gender, country)[0]
 
     def generate_accounts(n, gender: Gender = Gender.BOTH, country: Country = None):
             return generate_persons(n, gender, country)
-
-if __name__ == '__main__':
-    account = AccountGenerator.generate_accounts(3, gender = Gender.WOMEN, country=Country.IN)
-    # write_temp_json(account)
-    # print(account)
```

### Comparing `bose-1.8.1/bose/analytics.py` & `bose-2.0.0/bose/analytics.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from .local_storage import LocalStorage
 import requests
 
 class Analytics:
-    def send_tracking_data():
+    def send_tracking_data(task_name):
         try:
             cookies = {}
             headers = {}
             json_data = {
                 'type': 'bose_usage',
                 'data': {
+                    'task_name': task_name, 
                     "count": LocalStorage.get_item('count', 0)
                 },
             }
 
             response = requests.post('https://www.omkar.cloud/backend/actions/', 
                                     #  cookies=cookies, headers=headers, 
                                      json=json_data)
```

### Comparing `bose-1.8.1/bose/base_data.py` & `bose-2.0.0/bose/base_data.py`

 * *Files identical despite different names*

### Comparing `bose-1.8.1/bose/bose_driver.py` & `bose-2.0.0/bose/bose_undetected_driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import traceback
-from datetime import datetime
-from selenium import webdriver
+from undetected_chromedriver import Chrome
 
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 import random
 from time import sleep
+from .beep_utils import beep_input
 from .local_storage_driver import LocalStorage
 from .opponent import Opponent
 from .utils import relative_path, sleep_for_n_seconds, sleep_forever
+from datetime import datetime
 
 
-class BoseDriver(webdriver.Chrome):
+class BoseUndetectedDriver(Chrome):
 
     def get_by_current_page_referrer(self, link, wait=None):
 
         # selenium.common.exceptions.WebDriverException
         self.execute_script(f"""
                 window.location.href = "{link}";
             """)
@@ -27,16 +28,16 @@
 
     def js_click(self, element):
         self.execute_script("arguments[0].click();",  element)
 
     def sleep(self, n):
         sleep_for_n_seconds(n)
 
-    def wait_for_enter(self, text="Press Enter To Continue..."):
-        input(text)
+    def prompt(self, text="Press Enter To Continue..."):
+        return beep_input(text, self.beep)
 
     def short_random_sleep(self):
         sleep_for_n_seconds(random.uniform(2, 4))
 
     def long_random_sleep(self):
         sleep_for_n_seconds(random.uniform(6, 9))
 
@@ -261,16 +262,31 @@
                 time += sleep_time
                 sleep(sleep_time)
 
         if raise_exception:
             raise Exception(f"Page {target} not found")
         return False
 
+
     def save_screenshot(self, filename=datetime.now().strftime('%Y-%m-%d_%H-%M-%S') + ".png"):
         try:
             saving_screenshot_at = relative_path(
                 f'{self.task_path}/{filename}', 0)
             self.get_screenshot_as_file(
                 saving_screenshot_at)
         except:
             traceback.print_exc()
             print('Failed to save screenshot')
+
+    def prompt_to_solve_captcha(self):
+        print('')
+        print('   __ _ _ _    _                          _       _           ')
+        print('  / _(_) | |  (_)                        | |     | |          ')
+        print(' | |_ _| | |   _ _ __      ___ __ _ _ __ | |_ ___| |__   __ _ ')
+        print(' |  _| | | |  | | `_ \    / __/ _` | `_ \| __/ __| `_ \ / _` |') 
+        print(' | | | | | |  | | | | |  | (_| (_| | |_) | || (__| | | | (_| |')   # Tells user to solve captcha
+        print(' |_| |_|_|_|  |_|_| |_|   \___\__,_| .__/ \__\___|_| |_|\__,_|')
+        print('                                   | |                        ')
+        print('                                   |_|                        ')
+        print('')
+
+        return beep_input('Press fill in the captcha and press enter to continue ...', self.beep)
```

### Comparing `bose-1.8.1/bose/bose_undetected_driver.py` & `bose-2.0.0/bose/bose_driver.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import traceback
-from undetected_chromedriver import Chrome
+from datetime import datetime
+from selenium import webdriver
 
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 import random
 from time import sleep
+from .beep_utils import beep_input
 from .local_storage_driver import LocalStorage
 from .opponent import Opponent
 from .utils import relative_path, sleep_for_n_seconds, sleep_forever
-from datetime import datetime
 
 
-class BoseUndetectedDriver(Chrome):
+class BoseDriver(webdriver.Chrome):
 
     def get_by_current_page_referrer(self, link, wait=None):
 
         # selenium.common.exceptions.WebDriverException
         self.execute_script(f"""
                 window.location.href = "{link}";
             """)
@@ -27,16 +28,16 @@
 
     def js_click(self, element):
         self.execute_script("arguments[0].click();",  element)
 
     def sleep(self, n):
         sleep_for_n_seconds(n)
 
-    def wait_for_enter(self, text="Press Enter To Continue..."):
-        input(text)
+    def prompt(self, text="Press Enter To Continue..."):
+        return beep_input(text, self.beep)
 
     def short_random_sleep(self):
         sleep_for_n_seconds(random.uniform(2, 4))
 
     def long_random_sleep(self):
         sleep_for_n_seconds(random.uniform(6, 9))
 
@@ -261,16 +262,31 @@
                 time += sleep_time
                 sleep(sleep_time)
 
         if raise_exception:
             raise Exception(f"Page {target} not found")
         return False
 
+
     def save_screenshot(self, filename=datetime.now().strftime('%Y-%m-%d_%H-%M-%S') + ".png"):
         try:
             saving_screenshot_at = relative_path(
                 f'{self.task_path}/{filename}', 0)
             self.get_screenshot_as_file(
                 saving_screenshot_at)
         except:
             traceback.print_exc()
             print('Failed to save screenshot')
+
+    def prompt_to_solve_captcha(self):
+        print('')
+        print('   __ _ _ _    _                          _       _           ')
+        print('  / _(_) | |  (_)                        | |     | |          ')
+        print(' | |_ _| | |   _ _ __      ___ __ _ _ __ | |_ ___| |__   __ _ ')
+        print(' |  _| | | |  | | `_ \    / __/ _` | `_ \| __/ __| `_ \ / _` |') 
+        print(' | | | | | |  | | | | |  | (_| (_| | |_) | || (__| | | | (_| |')   # Tells user to solve captcha
+        print(' |_| |_|_|_|  |_|_| |_|   \___\__,_| .__/ \__\___|_| |_|\__,_|')
+        print('                                   | |                        ')
+        print('                                   |_|                        ')
+        print('')
+
+        return beep_input('Press fill in the captcha and press enter to continue ...', self.beep)
```

### Comparing `bose-1.8.1/bose/create_driver.py` & `bose-2.0.0/bose/create_driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,36 +10,46 @@
 from .bose_undetected_driver import BoseUndetectedDriver
 import shutil
 import os
 
 class RetryException(Exception):
     pass
 
-
 class BrowserConfig:
-    def __init__(self, user_agent=None, window_size=WindowSize.window_size_1920_1080, profile=None, is_eager=False, use_undetected_driver=False, close_on_crash = False):
+    def __init__(self, user_agent=None, headless= False,  window_size=WindowSize.window_size_1920_1080, profile=None, is_eager=False, use_undetected_driver=False, is_tiny_profile=False):
         self.user_agent = user_agent
+        self.headless = headless    
         self.window_size = window_size
-        self.profile = profile
+        
+        if profile is not None:
+            self.profile = str(profile)
+        else: 
+            self.profile = None
         self.is_eager = is_eager
         self.use_undetected_driver = use_undetected_driver
-        self.close_on_crash = close_on_crash
+        
+        self.is_tiny_profile = is_tiny_profile
+
+        if self.is_tiny_profile and self.profile is None:
+            raise Exception('Profile must be given when using tiny profile')
+
 
 def delete_cache(driver):
     print('Deleting Cache')
     driver.command_executor._commands['SEND_COMMAND'] = (
         'POST', '/session/$sessionId/chromium/send_command'
     )
     driver.execute('SEND_COMMAND', dict(
         cmd='Network.clearBrowserCache', params={}))
 
 
 def add_useragent(options, user_agent):
     options.add_argument(f'--user-agent={user_agent}')
 
+
 def create_profile_path(user_id):
     PROFILES_PATH = 'profiles'
     PATH = f'{PROFILES_PATH}/{user_id}'
     path = relative_path(PATH, 0)
     return path
 
 
@@ -58,66 +68,67 @@
 def delete_profile_path(user_id):
     path = create_profile_path(user_id)
     shutil.rmtree(path, ignore_errors=True)
 
 
 def add_essential_options(options, profile, window_size, user_agent):
     options.add_argument("--start-maximized")
-    
+
     if window_size == None:
         if profile == None:
             window_size = WindowSizeInstance.get_random()
         else:
             window_size = WindowSizeInstance.get_hashed(profile)
-    else: 
+    else:
         if window_size == WindowSize.RANDOM:
             window_size = WindowSizeInstance.get_random()
         elif window_size == WindowSize.HASHED:
             window_size = WindowSizeInstance.get_hashed(profile)
-        else: 
+        else:
             window_size = window_size
-    
+
     window_size = WindowSize.window_size_to_string(window_size)
     options.add_argument(f"--window-size={window_size}")
 
     if profile is not None:
         profile = str(profile)
 
     if user_agent == None:
         if profile == None:
             user_agent = UserAgentInstance.get_random()
         else:
             user_agent = UserAgentInstance.get_hashed(profile)
-    else: 
+    else:
         if user_agent == UserAgent.RANDOM:
             user_agent = UserAgentInstance.get_random()
         elif user_agent == UserAgent.HASHED:
             user_agent = UserAgentInstance.get_hashed(profile)
-        else: 
+        else:
             user_agent = user_agent
-    
+
     add_useragent(options, user_agent)
 
     has_user = profile is not None
+
     if has_user:
         path = create_profile_path(profile)
         user_data_path = f"--user-data-dir={path}"
         options.add_argument(user_data_path)
 
-    return {"window_size":window_size, "user_agent":user_agent, "profile": profile}
+    return {"window_size": window_size, "user_agent": user_agent, "profile": profile}
+
 
 def get_eager_startegy():
 
     caps = DesiredCapabilities().CHROME
     # caps["pageLoadStrategy"] = "normal"  #  Waits for full page load
     caps["pageLoadStrategy"] = "none"   # Do not wait for full page load
     return caps
 
 
-
 def hide_automation_flags(options):
     options.add_argument('--disable-blink-features=AutomationControlled')
     options.add_argument("--disable-blink-features")
 
     options.add_experimental_option(
         "excludeSwitches", ["enable-automation"])
     options.add_experimental_option('useAutomationExtension', False)
@@ -133,52 +144,60 @@
 
     return (
         os.path.exists('/.dockerenv') or
         os.path.isfile(path) and any('docker' in line for line in open(path))
         or os.environ.get('KUBERNETES_SERVICE_HOST') is not None
     )
 
+
 def get_driver_path():
     executable_name = "chromedriver.exe" if is_windows() else "chromedriver"
     dest_path = f"build/{executable_name}"
     return dest_path
 
+
 def create_driver(config: BrowserConfig):
     def run():
         is_undetected = config.use_undetected_driver
         options = ChromeOptions() if is_undetected else GoogleChromeOptions()
 
+        if config.headless:
+            options.add_argument('--headless=new')
+
         if is_docker():
             print("Running in Docker, So adding sandbox arguments")
             options.arguments.extend(
                 ["--no-sandbox", "--disable-setuid-sandbox"])
 
-        driver_attributes = add_essential_options(options, config.profile, config.window_size, config.user_agent)
+        driver_attributes = add_essential_options(
+            options, None if config.is_tiny_profile else config.profile, config.window_size, config.user_agent)
 
         if driver_attributes["profile"] is not None:
-            driver_string = "Creating Driver with profile {}, window_size={}, and user_agent={}".format(driver_attributes["profile"], driver_attributes["window_size"], driver_attributes["user_agent"])
+            driver_string = "Creating Driver with profile {}, window_size={}, and user_agent={}".format(
+                driver_attributes["profile"], driver_attributes["window_size"], driver_attributes["user_agent"])
         else:
-            driver_string = "Creating Driver with window_size={} and user_agent={}".format(driver_attributes["window_size"], driver_attributes["user_agent"])
-      
+            driver_string = "Creating Driver with window_size={} and user_agent={}".format(
+                driver_attributes["window_size"], driver_attributes["user_agent"])
+
         if config.is_eager:
             desired_capabilities = get_eager_startegy()
         else:
             desired_capabilities = None
-        
+
         print(driver_string)
 
         if is_undetected:
             driver = BoseUndetectedDriver(
                 desired_capabilities=desired_capabilities,
-                              options=options
-                            )
+                options=options
+            )
         else:
             # options.add_experimental_option("prefs",  {"profile.managed_default_content_settings.images": 2})
             hide_automation_flags(options)
-            
+
             # CAPTCHA
             options.arguments.extend(
                 ["--disable-web-security", "--disable-site-isolation-trials", "--disable-application-cache"])
 
             path = relative_path(get_driver_path(), 0)
 
             driver = BoseDriver(
@@ -189,11 +208,11 @@
 
         if driver_attributes["profile"] is None:
             del driver_attributes["profile"]
 
         driver._init_data = driver_attributes
         return driver
     driver = retry_if_is_error(
-                run, NETWORK_ERRORS + [(WebDriverException, lambda: delete_corrupted_files(config.profile) if config.profile else None )], 5)
+        run, NETWORK_ERRORS + [(WebDriverException, lambda: delete_corrupted_files(config.profile) if config.profile else None)], 5)
     print("Launched Browser")
 
     return driver
```

### Comparing `bose-1.8.1/bose/download_driver.py` & `bose-2.0.0/bose/download_driver.py`

 * *Files identical despite different names*

### Comparing `bose-1.8.1/bose/local_storage.py` & `bose-2.0.0/bose/local_storage.py`

 * *Files identical despite different names*

### Comparing `bose-1.8.1/bose/local_storage_driver.py` & `bose-2.0.0/bose/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `bose-1.8.1/bose/output.py` & `bose-2.0.0/bose/output.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import requests
 import csv
-import openpyxl
-from .utils import write_json, read_json
+from .utils import relative_path, write_json, read_json
 
 class Output:
 
     def read_json(filename):
         if not filename.startswith("output/"):
             filename = "output/" +  filename
 
@@ -47,53 +47,35 @@
             filename = filename + ".csv"
 
         with open(filename, 'w', newline='', encoding='utf-8') as csvfile:
             fieldnames = data[0].keys()  # get the fieldnames from the first dictionary
             writer = csv.DictWriter(csvfile, fieldnames=fieldnames)
             writer.writeheader()  # write the header row
             writer.writerows(data)  # write each row of data
-        print(f"View written CSV file at {filename}")        
-    def write_xlsx(data, filename):
-        """
-        Saves a list of dictionaries as an Excel file with the given filename.
-        Each dictionary in the list corresponds to a row in the Excel file.
-        The keys of each dictionary correspond to column names in the Excel file.
-        """
-        if len(data) == 0:
-            print("Data is empty.")
-            return
+        print(f"View written CSV file at {filename}")     
 
-        if not filename.startswith("output/"):
-            filename = "output/" +  filename
 
-        if not filename.endswith(".xlsx"):
-            filename = filename + ".xlsx"
-
-        wb = openpyxl.Workbook()
-        ws = wb.active
-
-        # write headers
-        headers = list(data[0].keys())
-        for col_num, header in enumerate(headers, start=1):
-            ws.cell(row=1, column=col_num).value = header
-
-        # write data
-        if data:
-            for row_num, data in enumerate(data, start=2):
-                for col_num, key in enumerate(headers, start=1):
-                    ws.cell(row=row_num, column=col_num).value = data.get(key)
-
-        # save file
-        wb.save(filename)
-        print(f"View written Excel file at {filename}")        
+    def read_finished_json():
+        return Output.read_json("finished.json")
 
-    def read_pending():
-        return Output.read_json("pending.json")
+    def write_finished_json(data):
+        return Output.write_json(data, 'finished.json')
 
-    def write_pending(data):
-        return Output.write_json(data, "pending.json")
 
-    def read_finished():
-        return Output.read_json("finished.json")
+    def write_finished_csv(data):
+        return Output.write_csv(data, 'finished.csv')
 
-    def write_finished(data):
-        return Output.write_json(data, 'finished.json')
+    def save_image(url, filename = None):
+        if filename is None:
+            filename = url.split("/")[-1]
+    
+        response = requests.get(url)
+        if response.status_code == 200:
+            # Extract the filename from the URL
+            output_dir = "output"
+
+            # Save the image in the output directory
+            with open(relative_path(
+                f'{output_dir}/{filename}', 0), "wb") as f:
+                f.write(response.content)
+        else:
+            print("Failed to download the image.")
```

### Comparing `bose-1.8.1/bose/task_info.py` & `bose-2.0.0/bose/task_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,15 @@
 import requests
 from datetime import datetime
-from requests.exceptions import ReadTimeout
 import traceback
 
+from .ip_utils import find_ip_details
+
 from .utils import pretty_format_time
 
-def find_safe_ip():
-    url = 'https://ipinfo.io/'
-    try:
-        response = requests.get(url, timeout=10)
-        data =  (response.json())
-
-        if "readme" in data:
-           del data["readme"]
-        return data
-    except ReadTimeout:
-        return None
-    except Exception:
-        traceback.print_exc()
-        return None
-    
 
 def format_time_diff(start_time, end_time):
     time_diff = end_time - start_time
     total_seconds = int(time_diff.total_seconds())
 
     minutes, seconds = divmod(total_seconds, 60)
 
@@ -42,25 +28,29 @@
 class TaskInfo():
   data = {}
   
   def start(self):
     self.data["start_time"] = datetime.now()
     pass
   
+  
   def end(self):
     self.data["end_time"] = datetime.now()
     self.data["duration"] = format_time_diff(self.data["start_time"],self.data["end_time"])
     
 
     self.data["start_time"] = pretty_format_time(self.data["start_time"])
     self.data["end_time"] = pretty_format_time(self.data["end_time"])
 
 
   def set_ip(self):
-    self.data["ip_details"] = find_safe_ip()
+    self.data["ip_details"] = find_ip_details()
+
+  def set_task_name(self, task_name):
+    self.data["task_name"] = task_name
 
 
 if __name__ == "__main__":
     t = TaskInfo()
     t.start()
     t.end()
     t.set_ip()
```

### Comparing `bose-1.8.1/bose/temp_mail.py` & `bose-2.0.0/bose/temp_mail.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,19 +7,17 @@
 from urllib.error import ContentTooShortError
 from http.client import RemoteDisconnected
 from urllib.error import ContentTooShortError, URLError
 
 NETWORK_ERRORS = [RemoteDisconnected, URLError,
                   ConnectionAbortedError, ContentTooShortError,  BlockingIOError]
 
-
 def istuple(el):
     return type(el) is tuple
 
-
 def is_errors_instance(instances, error):
     for i in range(len(instances)):
         ins = instances[i]
         if isinstance(error, ins):
             return True, i
     return False, -1
```

### Comparing `bose-1.8.1/bose/user_agent.py` & `bose-2.0.0/bose/user_agent.py`

 * *Files identical despite different names*

### Comparing `bose-1.8.1/bose/utils.py` & `bose-2.0.0/bose/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime
 import errno
 import json
 import sys
 from time import sleep
 import traceback
 from urllib.error import ContentTooShortError
 from http.client import RemoteDisconnected
@@ -132,17 +133,14 @@
 
 
 def remove_nones(list):
     return [element for element in list if element is not None]
 
 
 
-def wait_for_enter(message="Press Enter To Continue..."):
-    return input(message)
-
 
 
 def exit_with_failed_status():
     print('Exiting with status 1')
     sys.exit(1)
 
 
@@ -259,8 +257,21 @@
     with open(path, 'w') as fp:
         json.dump(data, fp, indent=indent)
 
 
 def get_driver_path():
     executable_name = "chromedriver.exe" if is_windows() else "chromedriver"
     dest_path = f"build/{executable_name}"
-    return dest_path
+    return dest_path
+
+
+datetime_format = '%Y-%m-%d %H:%M:%S'
+
+def str_to_datetime(when):
+    return datetime.strptime(
+        when, datetime_format)
+
+
+def datetime_to_str(when):
+    return when.strftime(datetime_format)
+
+
```

### Comparing `bose-1.8.1/bose/window_size.py` & `bose-2.0.0/bose/window_size.py`

 * *Files identical despite different names*

### Comparing `bose-1.8.1/setup.py` & `bose-2.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 
 install_requires = [
     "requests",
     "chromedriver-autoinstaller==0.4.0",
     "selenium==4.5.0",
     "undetected_chromedriver>=3.4.6",
-    "openpyxl>=3.0.3",
     "beautifulsoup4>=4.11.2",
 
 ]
 extras_require = {}
 cpython_dependencies = [
     "PyDispatcher>=2.0.5",
 ]
@@ -21,15 +20,15 @@
     except:
       return None
     
             
 setup(
     name='bose',
     packages=['bose'],
-    version='1.8.1',
+    version='2.0.0',
     license='MIT',
     project_urls={
         "Documentation": "https://omkar.cloud/bose/",
         "Source": "https://github.com/omkarcloud/bose",
         "Tracker": "https://github.com/omkarcloud/bose/issues",
     },
```

