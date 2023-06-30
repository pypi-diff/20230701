# Comparing `tmp/pycsgogpt-0.1.0.tar.gz` & `tmp/pycsgogpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycsgogpt-0.1.0.tar", max compression
+gzip compressed data, was "pycsgogpt-0.1.1.tar", max compression
```

## Comparing `pycsgogpt-0.1.0.tar` & `pycsgogpt-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1023 2023-06-30 22:36:04.906488 pycsgogpt-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-30 22:36:04.906488 pycsgogpt-0.1.0/pycsgogpt/__init__.py
--rw-r--r--   0        0        0      667 2023-06-30 22:36:04.906488 pycsgogpt-0.1.0/pycsgogpt/__main__.py
--rw-r--r--   0        0        0     2218 2023-06-30 22:36:04.906488 pycsgogpt-0.1.0/pycsgogpt/csgo_chatbot.py
--rw-r--r--   0        0        0      756 2023-06-30 22:36:04.906488 pycsgogpt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 pycsgogpt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1024 2023-06-30 22:42:41.828118 pycsgogpt-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 22:42:41.832118 pycsgogpt-0.1.1/pycsgogpt/__init__.py
+-rw-r--r--   0        0        0      667 2023-06-30 22:42:41.832118 pycsgogpt-0.1.1/pycsgogpt/__main__.py
+-rw-r--r--   0        0        0     2218 2023-06-30 22:42:41.832118 pycsgogpt-0.1.1/pycsgogpt/csgo_chatbot.py
+-rw-r--r--   0        0        0      756 2023-06-30 22:42:41.832118 pycsgogpt-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1789 1970-01-01 00:00:00.000000 pycsgogpt-0.1.1/PKG-INFO
```

### Comparing `pycsgogpt-0.1.0/README.md` & `pycsgogpt-0.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pycsgogpt
 
-**pycsgogpt** is a CSGO chatbot powered by OpenAI GPT-3.5 Turbo. It connects to a CSGO server via Telnet and uses the GPT-3.5 Turbo model to generate responses based on incoming messages from other players. The chatbot provides an interactive and fun experience by simulating human-like conversations in the game.
+**pycsgogpt** is a CSGO chatbot powered by OpenAI GPT-3.5 Turbo. It connects to a CSGO client via Telnet and uses the GPT-3.5 Turbo model to generate responses based on incoming messages from other players. The chatbot provides an interactive and fun experience by simulating human-like conversations in the game.
 
 ## Installation
 
 ```bash
 pip install pycsgogpt
 ```
 
@@ -20,8 +20,8 @@
 * openapi-key: Your OpenAI API key.
 * telnet-port (optional): The telnet port for the CSGO server (default: 21234).
 
 ## Contributing
 Contributions are welcome! If you have any bug reports, feature requests, or suggestions, please open an issue or submit a pull request.
 
 ## License
-This project is licensed under the MIT License. See [LICENSE](LICENSE) for more details.
+This project is licensed under the MIT License. See [LICENSE](LICENSE) for more details.
```

### Comparing `pycsgogpt-0.1.0/pycsgogpt/__main__.py` & `pycsgogpt-0.1.1/pycsgogpt/__main__.py`

 * *Files identical despite different names*

### Comparing `pycsgogpt-0.1.0/pycsgogpt/csgo_chatbot.py` & `pycsgogpt-0.1.1/pycsgogpt/csgo_chatbot.py`

 * *Files identical despite different names*

### Comparing `pycsgogpt-0.1.0/pyproject.toml` & `pycsgogpt-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "pycsgogpt"
-version = "0.1.0"
+version = "0.1.1"
 description = "CSGO Chatbot using OpenAI GPT-3.5 Turbo."
 authors = ["Aviv <4440524+nikeix@users.noreply.github.com>"]
 license = "MIT"
 keywords = ["csgo", "chatbot", "openai", "gpt"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `pycsgogpt-0.1.0/PKG-INFO` & `pycsgogpt-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycsgogpt
-Version: 0.1.0
+Version: 0.1.1
 Summary: CSGO Chatbot using OpenAI GPT-3.5 Turbo.
 License: MIT
 Keywords: csgo,chatbot,openai,gpt
 Author: Aviv
 Author-email: 4440524+nikeix@users.noreply.github.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,15 @@
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: telnetlib3 (>=2.0.2,<3.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # pycsgogpt
 
-**pycsgogpt** is a CSGO chatbot powered by OpenAI GPT-3.5 Turbo. It connects to a CSGO server via Telnet and uses the GPT-3.5 Turbo model to generate responses based on incoming messages from other players. The chatbot provides an interactive and fun experience by simulating human-like conversations in the game.
+**pycsgogpt** is a CSGO chatbot powered by OpenAI GPT-3.5 Turbo. It connects to a CSGO client via Telnet and uses the GPT-3.5 Turbo model to generate responses based on incoming messages from other players. The chatbot provides an interactive and fun experience by simulating human-like conversations in the game.
 
 ## Installation
 
 ```bash
 pip install pycsgogpt
 ```
 
@@ -42,7 +42,8 @@
 * telnet-port (optional): The telnet port for the CSGO server (default: 21234).
 
 ## Contributing
 Contributions are welcome! If you have any bug reports, feature requests, or suggestions, please open an issue or submit a pull request.
 
 ## License
 This project is licensed under the MIT License. See [LICENSE](LICENSE) for more details.
+
```

