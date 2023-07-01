# Comparing `tmp/freeGPT-1.2.1.tar.gz` & `tmp/freeGPT-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeGPT-1.2.1.tar", last modified: Fri Jun 30 21:36:33 2023, max compression
+gzip compressed data, was "freeGPT-1.2.2.tar", last modified: Sat Jul  1 09:45:48 2023, max compression
```

## Comparing `freeGPT-1.2.1.tar` & `freeGPT-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 21:36:33.056357 freeGPT-1.2.1/
--rw-rw-rw-   0        0        0    35149 2023-06-30 21:35:53.000000 freeGPT-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     3561 2023-06-30 21:36:33.054357 freeGPT-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2273 2023-06-30 21:35:53.000000 freeGPT-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 21:36:33.038357 freeGPT-1.2.1/freeGPT/
--rw-rw-rw-   0        0        0      120 2023-06-30 21:35:53.000000 freeGPT-1.2.1/freeGPT/__init__.py
--rw-rw-rw-   0        0        0     1880 2023-06-30 21:35:53.000000 freeGPT-1.2.1/freeGPT/alpaca_7b.py
--rw-rw-rw-   0        0        0     1955 2023-06-30 21:35:53.000000 freeGPT-1.2.1/freeGPT/gpt3.py
--rw-rw-rw-   0        0        0     4667 2023-06-30 21:35:53.000000 freeGPT-1.2.1/freeGPT/gpt4.py
-drwxrwxrwx   0        0        0        0 2023-06-30 21:36:33.053357 freeGPT-1.2.1/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     3561 2023-06-30 21:36:32.000000 freeGPT-1.2.1/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-06-30 21:36:33.000000 freeGPT-1.2.1/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 21:36:32.000000 freeGPT-1.2.1/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-30 21:36:32.000000 freeGPT-1.2.1/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-30 21:36:32.000000 freeGPT-1.2.1/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 21:36:33.056357 freeGPT-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1676 2023-06-30 21:35:53.000000 freeGPT-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:45:48.898915 freeGPT-1.2.2/
+-rw-rw-rw-   0        0        0    35149 2023-07-01 09:45:08.000000 freeGPT-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0     3648 2023-07-01 09:45:48.897917 freeGPT-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2355 2023-07-01 09:45:08.000000 freeGPT-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 09:45:48.870911 freeGPT-1.2.2/freeGPT/
+-rw-rw-rw-   0        0        0      120 2023-07-01 09:45:08.000000 freeGPT-1.2.2/freeGPT/__init__.py
+-rw-rw-rw-   0        0        0     1868 2023-07-01 09:45:08.000000 freeGPT-1.2.2/freeGPT/alpaca_7b.py
+-rw-rw-rw-   0        0        0     1955 2023-07-01 09:45:08.000000 freeGPT-1.2.2/freeGPT/gpt3.py
+-rw-rw-rw-   0        0        0     4647 2023-07-01 09:45:08.000000 freeGPT-1.2.2/freeGPT/gpt4.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:45:48.896912 freeGPT-1.2.2/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     3648 2023-07-01 09:45:48.000000 freeGPT-1.2.2/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-07-01 09:45:48.000000 freeGPT-1.2.2/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 09:45:48.000000 freeGPT-1.2.2/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-01 09:45:48.000000 freeGPT-1.2.2/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-01 09:45:48.000000 freeGPT-1.2.2/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 09:45:48.899912 freeGPT-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1676 2023-07-01 09:45:08.000000 freeGPT-1.2.2/setup.py
```

### Comparing `freeGPT-1.2.1/LICENSE` & `freeGPT-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.2.1/PKG-INFO` & `freeGPT-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.2.1
+Version: 1.2.2
 Summary: freeGPT provides free access to GPT3, GPT4 and more models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Project-URL: Discord, https://discord.gg/XH6pUGkwRr
@@ -43,15 +43,15 @@
 Join my [Discord server](https://discord.gg/XH6pUGkwRr) for live chat, support, or if you have any issues with this package.
 
 ## Source:
 
 | Models   | Websites                                                |
 | -------- | ------------------------------------------------------- |
 | gpt3     | [<ava-ai-ef611.web.app>](https://ava-ai-ef611.web.app/) |
-| gpt4     | [<you.com>](https://you.com/)       |
+| gpt4     | [<you.com>](https://you.com/)                           |
 | alpaca_7b| [<chatllama.baseten.co>](https://chatllama.baseten.co/) |
 
 ## Support this repository:
 
 - Star this repository :D
 - Add the [freeGPT Discord bot](https://dsc.gg/freeGPT).
 - Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
@@ -74,21 +74,26 @@
 - It's interactive, overall fast, and easy to use.
 - And lastly, it's [open-sourced](https://github.com/Ruu3f/freeGPT/tree/main/discord-bot).
 
 ## Example:
 
 ```python
 import freeGPT
+import asyncio
 
-while True:
-    prompt = input("👦: ")
-    try:
-        model = getattr(freeGPT, "Model Name here.")
-        resp = model.Completion.create(prompt)
-        print(f"🤖: {resp}")
-    except Exception as e:
-        print(f"🤖: {e}")
+
+async def main():
+    while True:
+        prompt = input("👦: ")
+        try:
+            resp = await getattr(freeGPT, "MODEL NAME").Completion.create(prompt)
+            print(f"🤖: {resp}")
+        except Exception as e:
+            print(f"🤖: {e}")
+
+
+asyncio.run(main())
 ```
 
 ## Star History Chart:
 
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.2.1/README.md` & `freeGPT-1.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 Join my [Discord server](https://discord.gg/XH6pUGkwRr) for live chat, support, or if you have any issues with this package.
 
 ## Source:
 
 | Models   | Websites                                                |
 | -------- | ------------------------------------------------------- |
 | gpt3     | [<ava-ai-ef611.web.app>](https://ava-ai-ef611.web.app/) |
-| gpt4     | [<you.com>](https://you.com/)       |
+| gpt4     | [<you.com>](https://you.com/)                           |
 | alpaca_7b| [<chatllama.baseten.co>](https://chatllama.baseten.co/) |
 
 ## Support this repository:
 
 - Star this repository :D
 - Add the [freeGPT Discord bot](https://dsc.gg/freeGPT).
 - Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
@@ -48,21 +48,26 @@
 - It's interactive, overall fast, and easy to use.
 - And lastly, it's [open-sourced](https://github.com/Ruu3f/freeGPT/tree/main/discord-bot).
 
 ## Example:
 
 ```python
 import freeGPT
+import asyncio
 
-while True:
-    prompt = input("👦: ")
-    try:
-        model = getattr(freeGPT, "Model Name here.")
-        resp = model.Completion.create(prompt)
-        print(f"🤖: {resp}")
-    except Exception as e:
-        print(f"🤖: {e}")
+
+async def main():
+    while True:
+        prompt = input("👦: ")
+        try:
+            resp = await getattr(freeGPT, "MODEL NAME").Completion.create(prompt)
+            print(f"🤖: {resp}")
+        except Exception as e:
+            print(f"🤖: {e}")
+
+
+asyncio.run(main())
 ```
 
 ## Star History Chart:
 
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.2.1/freeGPT/alpaca_7b.py` & `freeGPT-1.2.2/freeGPT/alpaca_7b.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,15 @@
     Attributes:
         None
 
     Methods:
         create(prompt): Generates a text completion for the given prompt using an API.
     """
 
-    @staticmethod
-    def create(prompt):
+    async def create(prompt):
         """
         Generates a text completion for the given prompt using an API.
 
         Args:
             prompt (str): The prompt for which to generate a text completion.
 
         Returns:
```

### Comparing `freeGPT-1.2.1/freeGPT/gpt3.py` & `freeGPT-1.2.2/freeGPT/gpt3.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 import requests
 
 
 class Completion:
-    @staticmethod
-    def create(prompt):
+    async def create(prompt):
         """
         Create a new completion based on the given prompt.
 
         Args:
             prompt (str): The prompt to generate a completion for.
 
         Returns:
@@ -28,21 +27,21 @@
                     "stream": True,
                     "messages": [
                         {"role": "system", "content": "You are Ava, an AI assistant."},
                         {"role": "user", "content": prompt},
                     ],
                 },
             )
-        except:
+        except Exception:
             raise Exception("Unable to fetch the response.")
         resp = ""
         for line in resp_obj.iter_lines():
             line_text = line.decode("utf-8").strip()
             if line_text.startswith("data:"):
-                data = line_text[len("data:") :]
+                data = line_text.split("data:")[1]
                 try:
                     data_json = json.loads(data)
                     if "choices" in data_json:
                         choices = data_json["choices"]
                         for choice in choices:
                             if (
                                 "finish_reason" in choice
```

### Comparing `freeGPT-1.2.1/freeGPT/gpt4.py` & `freeGPT-1.2.2/freeGPT/gpt4.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 try:
     import tls_client
 except Exception:
     subprocess.run(["pip", "install", "tls_client", "--no-cache-dir"])
 
 
 class Completion:
-    @staticmethod
-    def create(
+    async def create(
         prompt,
         page: int = 1,
         count: int = 10,
         safe_search: str = "Off",
         on_shopping_page: bool = False,
         mkt: str = "",
         response_filter: str = "WebPages, Translations, Computation, RelatedSearches",
@@ -105,20 +104,20 @@
 
         text = "".join(re.findall(r'{"youChatToken": "(.*?)"}', response.text))
 
         extra = {
             "youChatSerpResults": json.loads(you_chat_serp_results),
         }
 
-        result = {
+        resp = {
             "text": text.replace("\\n", "\n").replace("\\\\", "\\").replace('\\"', '"')
         }
 
         if include_links:
-            result["links"] = json.loads(third_party_search_results)["search"][
+            resp["links"] = json.loads(third_party_search_results)["search"][
                 "third_party_search_results"
             ]
 
         if detailed:
-            result["extra"] = extra
+            resp["extra"] = extra
 
-        return result["text"]
+        return resp["text"]
```

### Comparing `freeGPT-1.2.1/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.2.2/freeGPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.2.1
+Version: 1.2.2
 Summary: freeGPT provides free access to GPT3, GPT4 and more models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Project-URL: Discord, https://discord.gg/XH6pUGkwRr
@@ -43,15 +43,15 @@
 Join my [Discord server](https://discord.gg/XH6pUGkwRr) for live chat, support, or if you have any issues with this package.
 
 ## Source:
 
 | Models   | Websites                                                |
 | -------- | ------------------------------------------------------- |
 | gpt3     | [<ava-ai-ef611.web.app>](https://ava-ai-ef611.web.app/) |
-| gpt4     | [<you.com>](https://you.com/)       |
+| gpt4     | [<you.com>](https://you.com/)                           |
 | alpaca_7b| [<chatllama.baseten.co>](https://chatllama.baseten.co/) |
 
 ## Support this repository:
 
 - Star this repository :D
 - Add the [freeGPT Discord bot](https://dsc.gg/freeGPT).
 - Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
@@ -74,21 +74,26 @@
 - It's interactive, overall fast, and easy to use.
 - And lastly, it's [open-sourced](https://github.com/Ruu3f/freeGPT/tree/main/discord-bot).
 
 ## Example:
 
 ```python
 import freeGPT
+import asyncio
 
-while True:
-    prompt = input("👦: ")
-    try:
-        model = getattr(freeGPT, "Model Name here.")
-        resp = model.Completion.create(prompt)
-        print(f"🤖: {resp}")
-    except Exception as e:
-        print(f"🤖: {e}")
+
+async def main():
+    while True:
+        prompt = input("👦: ")
+        try:
+            resp = await getattr(freeGPT, "MODEL NAME").Completion.create(prompt)
+            print(f"🤖: {resp}")
+        except Exception as e:
+            print(f"🤖: {e}")
+
+
+asyncio.run(main())
 ```
 
 ## Star History Chart:
 
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.2.1/setup.py` & `freeGPT-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.2.1",
+    version="1.2.2",
     description="freeGPT provides free access to GPT3, GPT4 and more models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv3",
     keywords=[
```

