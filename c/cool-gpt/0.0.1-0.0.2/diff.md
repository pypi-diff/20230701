# Comparing `tmp/cool_gpt-0.0.1.tar.gz` & `tmp/cool_gpt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cool_gpt-0.0.1.tar", last modified: Sat Jul  1 04:25:52 2023, max compression
+gzip compressed data, was "cool_gpt-0.0.2.tar", last modified: Sat Jul  1 05:09:46 2023, max compression
```

## Comparing `cool_gpt-0.0.1.tar` & `cool_gpt-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 04:25:52.941962 cool_gpt-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-06-28 21:07:39.000000 cool_gpt-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2937 2023-07-01 04:25:52.941962 cool_gpt-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2294 2023-07-01 04:09:22.000000 cool_gpt-0.0.1/README.md
--rw-rw-rw-   0        0        0      693 2023-07-01 04:25:35.000000 cool_gpt-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-01 04:25:52.941962 cool_gpt-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-01 04:25:52.927013 cool_gpt-0.0.1/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 20:45:04.000000 cool_gpt-0.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 04:25:52.928008 cool_gpt-0.0.1/src/cool_gpt/
--rw-rw-rw-   0        0        0        0 2023-06-28 20:41:41.000000 cool_gpt-0.0.1/src/cool_gpt/__init__.py
--rw-rw-rw-   0        0        0     2703 2023-07-01 04:04:26.000000 cool_gpt-0.0.1/src/cool_gpt/bot.py
-drwxrwxrwx   0        0        0        0 2023-07-01 04:25:52.940971 cool_gpt-0.0.1/src/cool_gpt.egg-info/
--rw-rw-rw-   0        0        0     2937 2023-07-01 04:25:52.000000 cool_gpt-0.0.1/src/cool_gpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-01 04:25:52.000000 cool_gpt-0.0.1/src/cool_gpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 04:25:52.000000 cool_gpt-0.0.1/src/cool_gpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-01 04:25:52.000000 cool_gpt-0.0.1/src/cool_gpt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 05:09:46.515486 cool_gpt-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2023-06-28 21:07:39.000000 cool_gpt-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4141 2023-07-01 05:09:46.515486 cool_gpt-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3468 2023-07-01 05:08:33.000000 cool_gpt-0.0.2/README.md
+-rw-rw-rw-   0        0        0      816 2023-07-01 05:05:32.000000 cool_gpt-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-01 05:09:46.515486 cool_gpt-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-01 05:09:46.515486 cool_gpt-0.0.2/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 20:45:04.000000 cool_gpt-0.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 05:09:46.515486 cool_gpt-0.0.2/src/cool_gpt/
+-rw-rw-rw-   0        0        0        0 2023-06-28 20:41:41.000000 cool_gpt-0.0.2/src/cool_gpt/__init__.py
+-rw-rw-rw-   0        0        0     2737 2023-07-01 05:03:25.000000 cool_gpt-0.0.2/src/cool_gpt/bot.py
+drwxrwxrwx   0        0        0        0 2023-07-01 05:09:46.515486 cool_gpt-0.0.2/src/cool_gpt/speech_to_text/
+-rw-rw-rw-   0        0        0        0 2023-04-03 21:49:40.000000 cool_gpt-0.0.2/src/cool_gpt/speech_to_text/__init__.py
+-rw-rw-rw-   0        0        0     2277 2023-04-03 21:49:40.000000 cool_gpt-0.0.2/src/cool_gpt/speech_to_text/speech_to_text.py
+-rw-rw-rw-   0        0        0      715 2023-04-03 21:49:40.000000 cool_gpt-0.0.2/src/cool_gpt/speech_to_text/speech_to_text_whisper.py
+drwxrwxrwx   0        0        0        0 2023-07-01 05:09:46.515486 cool_gpt-0.0.2/src/cool_gpt/text_to_speech/
+-rw-rw-rw-   0        0        0        0 2023-04-03 21:49:40.000000 cool_gpt-0.0.2/src/cool_gpt/text_to_speech/__init__.py
+-rw-rw-rw-   0        0        0     3268 2023-04-03 21:49:40.000000 cool_gpt-0.0.2/src/cool_gpt/text_to_speech/text_to_speech.py
+drwxrwxrwx   0        0        0        0 2023-07-01 05:09:46.515486 cool_gpt-0.0.2/src/cool_gpt.egg-info/
+-rw-rw-rw-   0        0        0     4141 2023-07-01 05:09:46.000000 cool_gpt-0.0.2/src/cool_gpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-07-01 05:09:46.000000 cool_gpt-0.0.2/src/cool_gpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 05:09:46.000000 cool_gpt-0.0.2/src/cool_gpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-01 05:09:46.000000 cool_gpt-0.0.2/src/cool_gpt.egg-info/top_level.txt
```

### Comparing `cool_gpt-0.0.1/LICENSE` & `cool_gpt-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cool_gpt-0.0.1/PKG-INFO` & `cool_gpt-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cool_gpt
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package that can help you to generate text using ChatGPT via scraping.
 Author-email: dipeshpal <dipeshpal17@gmail.com>
 Project-URL: Homepage, https://github.com/Dipeshpal/cool-gpt
 Project-URL: Bug Tracker, https://github.com/Dipeshpal/cool-gpt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,28 +39,58 @@
 pip install cool_gpt
 ```
 
 ## Getting Started
 
 To get started, follow these steps:
 
-Here's a basic example of how to use cool_gpt:
+### [Basic Usage] Here's a basic example of how to use cool_gpt:
+
+Install: `pip install cool-gpt==0.0.1` or `pip install cool-gpt`
+
+**NOTE: cool-gpt==0.0.1 doesn't support text to speech and speech to text**
+
 
 ```
 from cool_gpt import bot
 
 driver = bot.setup_driver()
 print('Enter 'q' to quit')
 while True:
     message = input('You: ')
     if message == 'q':
         break
     print('Bot:', bot.ask(message, driver))
 ```
 
+### [Advance Usage] It also supports text to speech and speech to text:
+
+Install: `pip install cool-gpt`
+
+```
+from cool_gpt import bot
+from cool_gpt.speech_to_text.speech_to_text import speech_to_text_google
+from cool_gpt.speech_to_text.speech_to_text_whisper import speech_to_text_whisper
+from cool_gpt.text_to_speech.text_to_speech import text_to_speech
+
+driver = bot.setup_driver(debug=False)
+while True:
+    # message = input('You: ') # for text input
+    message, status = speech_to_text_whisper()  # for speech input via whisper
+    # message, status = speech_to_text_google()  # for speech input via gtts
+    if status:
+        print('You:', message)
+        ans = bot.ask(message, driver)
+        print('Bot:', ans)
+        text_to_speech(ans, backend_tts_api='pyttsx3')  # for speech output via pyttsx3 its free and unlimited
+        # _ = text_to_speech(ans, backend_tts_api='gtts')  # for speech output via gtts its free but limited in a day
+    else:
+        print('Speak again louder please.')
+```
+
 
 ## Limitations
 
 Please note the following limitations of cool_gpt:
 
 cool_gpt is dependent on the availability and reliability of the toolbot.ai interface.
```

### Comparing `cool_gpt-0.0.1/pyproject.toml` & `cool_gpt-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 [build-system]
-requires = ["setuptools>=61.0", "selenium==4.10.0", "element-manager==1.0.4"]
+requires = ["setuptools>=61.0", "selenium==4.10.0", "element-manager==1.0.4",
+    'gtts', 'playsound', 'SpeechRecognition', "pyttsx3", 'sounddevice',
+    'openai-whisper', 'pyaudio', 'shutup']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cool_gpt"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
-  { name="dipeshpal", email="dipeshpal17@gmail.com" },
+    { name = "dipeshpal", email = "dipeshpal17@gmail.com" },
 ]
 description = "A Python package that can help you to generate text using ChatGPT via scraping."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `cool_gpt-0.0.1/src/cool_gpt/bot.py` & `cool_gpt-0.0.2/src/cool_gpt/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.chrome.options import Options
 from element_manager import *
 import time
+import shutup
+
+shutup.please()
 
 
 def setup_driver(debug=True):
     """
     This sets up the driver in headless mode
     :return: selenium driver
     """
```

### Comparing `cool_gpt-0.0.1/src/cool_gpt.egg-info/PKG-INFO` & `cool_gpt-0.0.2/src/cool_gpt.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cool-gpt
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package that can help you to generate text using ChatGPT via scraping.
 Author-email: dipeshpal <dipeshpal17@gmail.com>
 Project-URL: Homepage, https://github.com/Dipeshpal/cool-gpt
 Project-URL: Bug Tracker, https://github.com/Dipeshpal/cool-gpt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,28 +39,58 @@
 pip install cool_gpt
 ```
 
 ## Getting Started
 
 To get started, follow these steps:
 
-Here's a basic example of how to use cool_gpt:
+### [Basic Usage] Here's a basic example of how to use cool_gpt:
+
+Install: `pip install cool-gpt==0.0.1` or `pip install cool-gpt`
+
+**NOTE: cool-gpt==0.0.1 doesn't support text to speech and speech to text**
+
 
 ```
 from cool_gpt import bot
 
 driver = bot.setup_driver()
 print('Enter 'q' to quit')
 while True:
     message = input('You: ')
     if message == 'q':
         break
     print('Bot:', bot.ask(message, driver))
 ```
 
+### [Advance Usage] It also supports text to speech and speech to text:
+
+Install: `pip install cool-gpt`
+
+```
+from cool_gpt import bot
+from cool_gpt.speech_to_text.speech_to_text import speech_to_text_google
+from cool_gpt.speech_to_text.speech_to_text_whisper import speech_to_text_whisper
+from cool_gpt.text_to_speech.text_to_speech import text_to_speech
+
+driver = bot.setup_driver(debug=False)
+while True:
+    # message = input('You: ') # for text input
+    message, status = speech_to_text_whisper()  # for speech input via whisper
+    # message, status = speech_to_text_google()  # for speech input via gtts
+    if status:
+        print('You:', message)
+        ans = bot.ask(message, driver)
+        print('Bot:', ans)
+        text_to_speech(ans, backend_tts_api='pyttsx3')  # for speech output via pyttsx3 its free and unlimited
+        # _ = text_to_speech(ans, backend_tts_api='gtts')  # for speech output via gtts its free but limited in a day
+    else:
+        print('Speak again louder please.')
+```
+
 
 ## Limitations
 
 Please note the following limitations of cool_gpt:
 
 cool_gpt is dependent on the availability and reliability of the toolbot.ai interface.
```

