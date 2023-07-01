# Comparing `tmp/speech_engine-0.0.1.tar.gz` & `tmp/speech_engine-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\speech_engine-0.0.1.tar", last modified: Fri Jun 30 15:03:26 2023, max compression
+gzip compressed data, was "dist\speech_engine-0.0.2.tar", last modified: Sat Jul  1 03:27:37 2023, max compression
```

## Comparing `speech_engine-0.0.1.tar` & `speech_engine-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 15:03:26.991435 speech_engine-0.0.1/
--rw-rw-rw-   0        0        0     2876 2023-06-30 15:03:26.990450 speech_engine-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1605 2023-06-30 15:01:39.000000 speech_engine-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 15:03:26.991435 speech_engine-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1130 2023-06-30 15:01:22.000000 speech_engine-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:03:26.942425 speech_engine-0.0.1/speech_engine/
--rw-rw-rw-   0        0        0       47 2023-06-30 05:39:37.000000 speech_engine-0.0.1/speech_engine/__init__.py
--rw-rw-rw-   0        0        0     2071 2023-06-30 15:01:56.000000 speech_engine-0.0.1/speech_engine/tts.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:03:26.987547 speech_engine-0.0.1/speech_engine.egg-info/
--rw-rw-rw-   0        0        0     2876 2023-06-30 15:03:26.000000 speech_engine-0.0.1/speech_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-06-30 15:03:26.000000 speech_engine-0.0.1/speech_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 15:03:26.000000 speech_engine-0.0.1/speech_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-30 15:03:26.000000 speech_engine-0.0.1/speech_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-30 15:03:26.000000 speech_engine-0.0.1/speech_engine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 03:27:37.232620 speech_engine-0.0.2/
+-rw-rw-rw-   0        0        0     2985 2023-07-01 03:27:37.231653 speech_engine-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1722 2023-07-01 03:19:52.000000 speech_engine-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-01 03:27:37.233622 speech_engine-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1130 2023-07-01 03:24:41.000000 speech_engine-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 03:27:37.176032 speech_engine-0.0.2/speech_engine/
+-rw-rw-rw-   0        0        0      128 2023-06-30 15:26:28.000000 speech_engine-0.0.2/speech_engine/__init__.py
+-rw-rw-rw-   0        0        0     5108 2023-07-01 03:11:57.000000 speech_engine-0.0.2/speech_engine/tts.py
+drwxrwxrwx   0        0        0        0 2023-07-01 03:27:37.228621 speech_engine-0.0.2/speech_engine.egg-info/
+-rw-rw-rw-   0        0        0     2985 2023-07-01 03:27:37.000000 speech_engine-0.0.2/speech_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-07-01 03:27:37.000000 speech_engine-0.0.2/speech_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 03:27:37.000000 speech_engine-0.0.2/speech_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-01 03:27:37.000000 speech_engine-0.0.2/speech_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-01 03:27:37.000000 speech_engine-0.0.2/speech_engine.egg-info/top_level.txt
```

### Comparing `speech_engine-0.0.1/PKG-INFO` & `speech_engine-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: speech_engine
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package for synthesizing text into speech
 Home-page: https://github.com/PraaneshSelvaraj/speech_engine
 Author: Praanesh
 Author-email: praaneshselvaraj2003@gmail.com
 License: UNKNOWN
-Description: # speech_engine
+Description: # Speech Engine
         
-        speech_engine is a Python package that provides a simple interface for synthesizing text into speech using multiple .
+        Speech Engine is a Python package that provides a simple interface for synthesizing text into speech using different TTS engines, including Google Text-to-Speech (gTTS) and Wit.ai Text-to-Speech (Wit TTS).
         
         ## Installation
         
-        You can install `speech_engine` using pip:
+        You can install `speech-engine` using pip:
         
-        ```python
-        pip install speech_engine
+        ```bash
+        pip install speech-engine
         ```
         
         ## Usage
-        
-        ### Basic Usage
-        
+        ### TTS_GOOGLE
         ```python
         from speech_engine import TTS_Google, FileExtensionError
         
         # Instantiate TTS_Google
         tts = TTS_Google()
         
         # Set the language and other options
@@ -38,40 +36,41 @@
         # Synthesize and save speech as an audio file
         try:
             tts.save("Hello, world!", "output.mp3")
         except FileExtensionError as e:
             print(e.message)
         ```
         
-        
-        ### Customizing Options
-        You can customize various options of the TTS_Google class:
-        
-        
+        ### TTS_Witai
         ```python
-        # Set the language
-        tts.lang = 'en'
+        from speech_engine import TTS_Witai, InvalidTokenError, FileExtensionError
         
-        # Set the top-level domain (optional)
-        tts.tld = 'com'
+        # Instantiate TTS_Witai with the Wit.ai auth token
+        tts = TTS_Witai(authToken)
         
-        # Set the speech speed
-        tts.slow = False
-        ```
+        # Check if the provided token is valid
+        if not tts.is_valid_token:
+            raise InvalidTokenError()
         
-        ### Handling File Extension Errors
-        When using the save() method, if the provided filename does not have a .mp3 extension, a FileExtensionError will be raised. You can handle this exception as follows:
+        # Set the voice
+        tts.voice = 'Colin'
         
-        ```python
+        # Synthesize and play speech
+        tts.speak("Hello, world!")
+        
+        # Synthesize and save speech as an audio file
         try:
-            tts.save("Hello, world!", "output.wav")
+            tts.save("Hello, world!", "output.mp3")
         except FileExtensionError as e:
             print(e.message)
-        ```
         
+        # Get available voices
+        voices = tts.get_voices()
+        print(voices)
+        ```
         ## License
         This project is licensed under the MIT License - see the [LICENSE](https://github.com/PraaneshSelvaraj/speech_engine/blob/main/LICENSE) file for details.
         
         ## Contributions
         Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on GitHub.
         
 Keywords: speech_engine,text2speech,text-to-speech,TTS,speech synthesis,audio generation,natural language processing,language processing,voice synthesis,speech output,speech generation,language synthesis,voice output,audio synthesis,voice generation
```

### Comparing `speech_engine-0.0.1/setup.py` & `speech_engine-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='speech_engine',
-    version='0.0.1',
+    version='0.0.2',
     author='Praanesh',
     author_email='praaneshselvaraj2003@gmail.com',
     description='Python package for synthesizing text into speech',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/PraaneshSelvaraj/speech_engine',
     packages=find_packages(),
```

### Comparing `speech_engine-0.0.1/speech_engine.egg-info/PKG-INFO` & `speech_engine-0.0.2/speech_engine.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: speech-engine
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package for synthesizing text into speech
 Home-page: https://github.com/PraaneshSelvaraj/speech_engine
 Author: Praanesh
 Author-email: praaneshselvaraj2003@gmail.com
 License: UNKNOWN
-Description: # speech_engine
+Description: # Speech Engine
         
-        speech_engine is a Python package that provides a simple interface for synthesizing text into speech using multiple .
+        Speech Engine is a Python package that provides a simple interface for synthesizing text into speech using different TTS engines, including Google Text-to-Speech (gTTS) and Wit.ai Text-to-Speech (Wit TTS).
         
         ## Installation
         
-        You can install `speech_engine` using pip:
+        You can install `speech-engine` using pip:
         
-        ```python
-        pip install speech_engine
+        ```bash
+        pip install speech-engine
         ```
         
         ## Usage
-        
-        ### Basic Usage
-        
+        ### TTS_GOOGLE
         ```python
         from speech_engine import TTS_Google, FileExtensionError
         
         # Instantiate TTS_Google
         tts = TTS_Google()
         
         # Set the language and other options
@@ -38,40 +36,41 @@
         # Synthesize and save speech as an audio file
         try:
             tts.save("Hello, world!", "output.mp3")
         except FileExtensionError as e:
             print(e.message)
         ```
         
-        
-        ### Customizing Options
-        You can customize various options of the TTS_Google class:
-        
-        
+        ### TTS_Witai
         ```python
-        # Set the language
-        tts.lang = 'en'
+        from speech_engine import TTS_Witai, InvalidTokenError, FileExtensionError
         
-        # Set the top-level domain (optional)
-        tts.tld = 'com'
+        # Instantiate TTS_Witai with the Wit.ai auth token
+        tts = TTS_Witai(authToken)
         
-        # Set the speech speed
-        tts.slow = False
-        ```
+        # Check if the provided token is valid
+        if not tts.is_valid_token:
+            raise InvalidTokenError()
         
-        ### Handling File Extension Errors
-        When using the save() method, if the provided filename does not have a .mp3 extension, a FileExtensionError will be raised. You can handle this exception as follows:
+        # Set the voice
+        tts.voice = 'Colin'
         
-        ```python
+        # Synthesize and play speech
+        tts.speak("Hello, world!")
+        
+        # Synthesize and save speech as an audio file
         try:
-            tts.save("Hello, world!", "output.wav")
+            tts.save("Hello, world!", "output.mp3")
         except FileExtensionError as e:
             print(e.message)
-        ```
         
+        # Get available voices
+        voices = tts.get_voices()
+        print(voices)
+        ```
         ## License
         This project is licensed under the MIT License - see the [LICENSE](https://github.com/PraaneshSelvaraj/speech_engine/blob/main/LICENSE) file for details.
         
         ## Contributions
         Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on GitHub.
         
 Keywords: speech_engine,text2speech,text-to-speech,TTS,speech synthesis,audio generation,natural language processing,language processing,voice synthesis,speech output,speech generation,language synthesis,voice output,audio synthesis,voice generation
```

