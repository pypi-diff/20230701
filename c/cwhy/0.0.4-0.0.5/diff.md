# Comparing `tmp/cwhy-0.0.4.tar.gz` & `tmp/cwhy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwhy-0.0.4.tar", last modified: Wed Apr 12 18:34:07 2023, max compression
+gzip compressed data, was "cwhy-0.0.5.tar", last modified: Fri Jun 30 22:24:03 2023, max compression
```

## Comparing `cwhy-0.0.4.tar` & `cwhy-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-12 18:34:07.473870 cwhy-0.0.4/
--rw-r--r--   0 emery      (504) staff       (20)    11357 2023-04-04 16:20:04.000000 cwhy-0.0.4/LICENSE
--rw-r--r--   0 emery      (504) staff       (20)    11083 2023-04-12 18:34:07.473717 cwhy-0.0.4/PKG-INFO
--rw-r--r--   0 emery      (504) staff       (20)    10468 2023-04-11 21:33:44.000000 cwhy-0.0.4/README.md
--rw-r--r--   0 emery      (504) staff       (20)      904 2023-04-12 18:33:53.000000 cwhy-0.0.4/pyproject.toml
--rw-r--r--   0 emery      (504) staff       (20)       38 2023-04-12 18:34:07.473901 cwhy-0.0.4/setup.cfg
-drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-12 18:34:07.472376 cwhy-0.0.4/src/
-drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-12 18:34:07.472967 cwhy-0.0.4/src/cwhy/
--rw-r--r--   0 emery      (504) staff       (20)        0 2023-04-12 18:32:27.000000 cwhy-0.0.4/src/cwhy/__init__.py
--rwxr-xr-x   0 emery      (504) staff       (20)     1954 2023-04-12 18:33:36.000000 cwhy-0.0.4/src/cwhy/__main__.py
--rwxr-xr-x   0 emery      (504) staff       (20)     7774 2023-04-12 18:20:17.000000 cwhy-0.0.4/src/cwhy/cwhy.py
-drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-04-12 18:34:07.473586 cwhy-0.0.4/src/cwhy.egg-info/
--rw-r--r--   0 emery      (504) staff       (20)    11083 2023-04-12 18:34:07.000000 cwhy-0.0.4/src/cwhy.egg-info/PKG-INFO
--rw-r--r--   0 emery      (504) staff       (20)      285 2023-04-12 18:34:07.000000 cwhy-0.0.4/src/cwhy.egg-info/SOURCES.txt
--rw-r--r--   0 emery      (504) staff       (20)        1 2023-04-12 18:34:07.000000 cwhy-0.0.4/src/cwhy.egg-info/dependency_links.txt
--rw-r--r--   0 emery      (504) staff       (20)       44 2023-04-12 18:34:07.000000 cwhy-0.0.4/src/cwhy.egg-info/entry_points.txt
--rw-r--r--   0 emery      (504) staff       (20)       95 2023-04-12 18:34:07.000000 cwhy-0.0.4/src/cwhy.egg-info/requires.txt
--rw-r--r--   0 emery      (504) staff       (20)        5 2023-04-12 18:34:07.000000 cwhy-0.0.4/src/cwhy.egg-info/top_level.txt
+drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-06-30 22:24:03.442305 cwhy-0.0.5/
+-rw-r--r--   0 emery      (504) staff       (20)    11357 2023-04-04 16:20:04.000000 cwhy-0.0.5/LICENSE
+-rw-r--r--   0 emery      (504) staff       (20)    11707 2023-06-30 22:24:03.442118 cwhy-0.0.5/PKG-INFO
+-rw-r--r--   0 emery      (504) staff       (20)    11085 2023-06-30 22:21:42.000000 cwhy-0.0.5/README.md
+-rw-r--r--   0 emery      (504) staff       (20)      817 2023-06-30 22:23:29.000000 cwhy-0.0.5/pyproject.toml
+-rw-r--r--   0 emery      (504) staff       (20)       38 2023-06-30 22:24:03.442335 cwhy-0.0.5/setup.cfg
+drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-06-30 22:24:03.440759 cwhy-0.0.5/src/
+drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-06-30 22:24:03.441362 cwhy-0.0.5/src/cwhy/
+-rw-r--r--   0 emery      (504) staff       (20)        0 2023-04-12 18:32:27.000000 cwhy-0.0.5/src/cwhy/__init__.py
+-rwxr-xr-x   0 emery      (504) staff       (20)     2826 2023-06-30 22:21:42.000000 cwhy-0.0.5/src/cwhy/__main__.py
+-rwxr-xr-x   0 emery      (504) staff       (20)     7804 2023-06-30 22:21:42.000000 cwhy-0.0.5/src/cwhy/cwhy.py
+drwxr-xr-x   0 emery      (504) staff       (20)        0 2023-06-30 22:24:03.441983 cwhy-0.0.5/src/cwhy.egg-info/
+-rw-r--r--   0 emery      (504) staff       (20)    11707 2023-06-30 22:24:03.000000 cwhy-0.0.5/src/cwhy.egg-info/PKG-INFO
+-rw-r--r--   0 emery      (504) staff       (20)      285 2023-06-30 22:24:03.000000 cwhy-0.0.5/src/cwhy.egg-info/SOURCES.txt
+-rw-r--r--   0 emery      (504) staff       (20)        1 2023-06-30 22:24:03.000000 cwhy-0.0.5/src/cwhy.egg-info/dependency_links.txt
+-rw-r--r--   0 emery      (504) staff       (20)       44 2023-06-30 22:24:03.000000 cwhy-0.0.5/src/cwhy.egg-info/entry_points.txt
+-rw-r--r--   0 emery      (504) staff       (20)       15 2023-06-30 22:24:03.000000 cwhy-0.0.5/src/cwhy.egg-info/requires.txt
+-rw-r--r--   0 emery      (504) staff       (20)        5 2023-06-30 22:24:03.000000 cwhy-0.0.5/src/cwhy.egg-info/top_level.txt
```

### Comparing `cwhy-0.0.4/LICENSE` & `cwhy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cwhy-0.0.4/PKG-INFO` & `cwhy-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,62 +1,90 @@
 Metadata-Version: 2.1
 Name: cwhy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Explains and proposes fixes for C/C++/Rust compiler errors.
 Author-email: Emery Berger <emery.berger@gmail.com>, Nicolas van Kempen <nvankemp@gmail.com>, Bryce Adelstein Lelbach <brycelelbach@gmail.com>
 Project-URL: Homepage, https://github.com/plasma-umass/cwhy
-Project-URL: Bug Tracker, https://github.com/plasma-umass/cwhy
+Project-URL: Bug Tracker, https://github.com/plasma-umass/cwhy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cwhy
 
-by [Emery Berger](https://emeryberger.com), [Bryce Adelstein Lelbach](https://twitter.com/blelbach?lang=en), and [Nicolas van Kempen](https://nvankempen.com/)
+by [Emery Berger](https://emeryberger.com), [Bryce Adelstein Lelbach](https://twitter.com/blelbach?lang=en), and
+[Nicolas van Kempen](https://nvankempen.com/).
 
-[![PyPI Latest Release](https://img.shields.io/pypi/v/cwhy.svg)](https://pypi.org/project/cwhy/)[![Downloads](https://pepy.tech/badge/cwhy)](https://pepy.tech/project/cwhy) [![Downloads](https://pepy.tech/badge/cwhy/month)](https://pepy.tech/project/cwhy) ![Python versions](https://img.shields.io/pypi/pyversions/cwhy.svg?style=flat-square)
+[![PyPI](https://img.shields.io/pypi/v/cwhy.svg)](https://pypi.org/project/cwhy/)
+[![downloads](https://pepy.tech/badge/cwhy)](https://pepy.tech/project/cwhy)
+[![downloads/month](https://pepy.tech/badge/cwhy/month)](https://pepy.tech/project/cwhy)
 
 ("See why")
 
-Explains and suggest fixes for C/C++/Rust compiler error messages.
+Explains and suggests fixes for C/C++/Rust compiler error messages.
 
 ## Installation
 
 ```
 python3 -m pip install cwhy
 ```
 
-*NOTE*: To use cwhy, you must first set up an OpenAI API key. If you
-already have an API key, you can set it as an environment variable
-called `OPENAI_API_KEY`. If you do not have one yet,
-you can get a key here: https://platform.openai.com/account/api-keys
+To use cwhy, you must first set up an OpenAI API key. If you already have an API key, you can set it as an environment
+variable called `OPENAI_API_KEY`. If you do not have one yet, you can
+[get a key here](https://platform.openai.com/account/api-keys).
 
-```
-export OPENAI_API_KEY=<your-api-key>
+```bash
+% export OPENAI_API_KEY=<your-api-key>
 ```
 
 ## Usage
 
-Just pipe your compiler's output to `cwhy`. `cwhy` will by default provide an explanation. If you'd like a suggested fix, add `fix`.
+### Compiler wrapper mode
+
+This new mode is recommended as CWhy will then operate in the same context as the compiler, and will do a better job
+finding the right source files.
+
+```bash
+# Invoking the compiler directly.
+% `cwhy wrapper` mycode.cpp
 
-e.g.,
+# Invoking with GNU make, using GPT-4.
+% CXX=`cwhy --llm=gpt-4 wrapper` make
 
+# Invoking with CMake, using GPT-4 and clang++.
+% cmake -DCMAKE_CXX_COMPILER=`cwhy --llm=gpt-4 wrapper --compiler=clang++` ...
 ```
-% clang++ -g mycode.cpp |& cwhy     # explanation only
-% clang++ -g mycode.cpp |& cwhy fix # to see a suggested fix
+
+### Original mode
+
+Just pipe your compiler's output to `cwhy`.
+
+```bash
+% clang++ -g mycode.cpp |& cwhy
 ```
 
+### Options
+
+These options can be displayed with `cwhy --help`.
+
+ -  `--llm`: pick a specific OpenAI LLM. CWhy has been tested with `gpt-3.5-turbo` and `gpt-4`.
+ -  `--timeout`: pick a different timeout than the default for API calls.
+ -  `--show-prompt` (debug): print prompts before calling the API.
+
+The wrapper mode specifically also has a `--compiler` option to select the underlying compiler to use.
+
 ## Examples
 
 ### C++
 
-This highlighted example is [missing-hash.cpp](test/c++/missing-hash.cpp), which is one of the first cases we experimented with.
+This highlighted example is [missing-hash.cpp](test/c++/missing-hash.cpp), which is one of the first cases we
+experimented with.
 
 <details>
 <summary>
 Expand to see the original (pretty obscure) error message:
 </summary>
 
 ```
```

### Comparing `cwhy-0.0.4/README.md` & `cwhy-0.0.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,76 @@
 # cwhy
 
-by [Emery Berger](https://emeryberger.com), [Bryce Adelstein Lelbach](https://twitter.com/blelbach?lang=en), and [Nicolas van Kempen](https://nvankempen.com/)
+by [Emery Berger](https://emeryberger.com), [Bryce Adelstein Lelbach](https://twitter.com/blelbach?lang=en), and
+[Nicolas van Kempen](https://nvankempen.com/).
 
-[![PyPI Latest Release](https://img.shields.io/pypi/v/cwhy.svg)](https://pypi.org/project/cwhy/)[![Downloads](https://pepy.tech/badge/cwhy)](https://pepy.tech/project/cwhy) [![Downloads](https://pepy.tech/badge/cwhy/month)](https://pepy.tech/project/cwhy) ![Python versions](https://img.shields.io/pypi/pyversions/cwhy.svg?style=flat-square)
+[![PyPI](https://img.shields.io/pypi/v/cwhy.svg)](https://pypi.org/project/cwhy/)
+[![downloads](https://pepy.tech/badge/cwhy)](https://pepy.tech/project/cwhy)
+[![downloads/month](https://pepy.tech/badge/cwhy/month)](https://pepy.tech/project/cwhy)
 
 ("See why")
 
-Explains and suggest fixes for C/C++/Rust compiler error messages.
+Explains and suggests fixes for C/C++/Rust compiler error messages.
 
 ## Installation
 
 ```
 python3 -m pip install cwhy
 ```
 
-*NOTE*: To use cwhy, you must first set up an OpenAI API key. If you
-already have an API key, you can set it as an environment variable
-called `OPENAI_API_KEY`. If you do not have one yet,
-you can get a key here: https://platform.openai.com/account/api-keys
+To use cwhy, you must first set up an OpenAI API key. If you already have an API key, you can set it as an environment
+variable called `OPENAI_API_KEY`. If you do not have one yet, you can
+[get a key here](https://platform.openai.com/account/api-keys).
 
-```
-export OPENAI_API_KEY=<your-api-key>
+```bash
+% export OPENAI_API_KEY=<your-api-key>
 ```
 
 ## Usage
 
-Just pipe your compiler's output to `cwhy`. `cwhy` will by default provide an explanation. If you'd like a suggested fix, add `fix`.
+### Compiler wrapper mode
+
+This new mode is recommended as CWhy will then operate in the same context as the compiler, and will do a better job
+finding the right source files.
+
+```bash
+# Invoking the compiler directly.
+% `cwhy wrapper` mycode.cpp
 
-e.g.,
+# Invoking with GNU make, using GPT-4.
+% CXX=`cwhy --llm=gpt-4 wrapper` make
 
+# Invoking with CMake, using GPT-4 and clang++.
+% cmake -DCMAKE_CXX_COMPILER=`cwhy --llm=gpt-4 wrapper --compiler=clang++` ...
 ```
-% clang++ -g mycode.cpp |& cwhy     # explanation only
-% clang++ -g mycode.cpp |& cwhy fix # to see a suggested fix
+
+### Original mode
+
+Just pipe your compiler's output to `cwhy`.
+
+```bash
+% clang++ -g mycode.cpp |& cwhy
 ```
 
+### Options
+
+These options can be displayed with `cwhy --help`.
+
+ -  `--llm`: pick a specific OpenAI LLM. CWhy has been tested with `gpt-3.5-turbo` and `gpt-4`.
+ -  `--timeout`: pick a different timeout than the default for API calls.
+ -  `--show-prompt` (debug): print prompts before calling the API.
+
+The wrapper mode specifically also has a `--compiler` option to select the underlying compiler to use.
+
 ## Examples
 
 ### C++
 
-This highlighted example is [missing-hash.cpp](test/c++/missing-hash.cpp), which is one of the first cases we experimented with.
+This highlighted example is [missing-hash.cpp](test/c++/missing-hash.cpp), which is one of the first cases we
+experimented with.
 
 <details>
 <summary>
 Expand to see the original (pretty obscure) error message:
 </summary>
 
 ```
```

### Comparing `cwhy-0.0.4/pyproject.toml` & `cwhy-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cwhy"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Emery Berger", email="emery.berger@gmail.com" },
   { name="Nicolas van Kempen", email="nvankemp@gmail.com" },
   { name="Bryce Adelstein Lelbach", email="brycelelbach@gmail.com" }
 ]
-dependencies = ["openai>=0.27.0", "openai_async>=0.0.3", "rich>=12.4.4", "ast-comments>=1.0.0", "click>=8.1.3", "httpx>=0.23.3"]
+dependencies = ["openai>=0.27.0"]
 description = "Explains and proposes fixes for C/C++/Rust compiler errors."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -22,8 +22,8 @@
 
 [project.scripts]
 cwhy = "cwhy.__main__:main"
 
 
 [project.urls]
 "Homepage" = "https://github.com/plasma-umass/cwhy"
-"Bug Tracker" = "https://github.com/plasma-umass/cwhy"
+"Bug Tracker" = "https://github.com/plasma-umass/cwhy/issues"
```

### Comparing `cwhy-0.0.4/src/cwhy/cwhy.py` & `cwhy-0.0.5/src/cwhy/cwhy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,206 +1,226 @@
-#! /usr/bin/env python3
-import asyncio
-import httpx
-import io
-import openai
-import openai_async
 import re
 import sys
-import traceback
 import textwrap
 
+import openai
+
+
 def word_wrap_except_code_blocks(text: str) -> str:
     """Wraps text except for code blocks.
 
     Splits the text into paragraphs and wraps each paragraph,
     except for paragraphs that are inside of code blocks denoted
     by ` ``` `. Returns the updated text.
 
     Args:
         text: The text to wrap.
 
     Returns:
         The wrapped text.
     """
     # Split text into paragraphs
-    paragraphs = text.split('\n\n')
+    paragraphs = text.split("\n\n")
     wrapped_paragraphs = []
     # Check if currently in a code block.
     in_code_block = False
     # Loop through each paragraph and apply appropriate wrapping.
     for paragraph in paragraphs:
         # If this paragraph starts and ends with a code block, add it as is.
-        if paragraph.startswith('```') and paragraph.endswith('```'):
+        if paragraph.startswith("```") and paragraph.endswith("```"):
             wrapped_paragraphs.append(paragraph)
             continue
         # If this is the beginning of a code block add it as is.
-        if paragraph.startswith('```'):
+        if paragraph.startswith("```"):
             in_code_block = True
             wrapped_paragraphs.append(paragraph)
             continue
         # If this is the end of a code block stop skipping text.
-        if paragraph.endswith('```'):
+        if paragraph.endswith("```"):
             in_code_block = False
             wrapped_paragraphs.append(paragraph)
             continue
         # If we are currently in a code block add the paragraph as is.
         if in_code_block:
             wrapped_paragraphs.append(paragraph)
         else:
             # Otherwise, apply text wrapping to the paragraph.
             wrapped_paragraph = textwrap.fill(paragraph)
             wrapped_paragraphs.append(wrapped_paragraph)
     # Join all paragraphs into a single string
-    wrapped_text = '\n\n'.join(wrapped_paragraphs)
+    wrapped_text = "\n\n".join(wrapped_paragraphs)
     return wrapped_text
 
+
 def read_lines(file_path: str, start_line: int, end_line: int) -> (str, int):
     """
     Read lines from a file.
 
     Args:
         file_path (str): The path of the file to read.
         start_line (int): The line number of the first line to include (1-indexed).
         end_line (int): The line number of the last line to include.
 
     Returns:
         (str, end_line): The content read and the last line included.
 
     """
     # open the file for reading
-    with open(file_path, 'r') as f:
-        # read all the lines from the file
-        lines = f.readlines()
-        # remove trailing newline characters
-        lines = [line.rstrip() for line in lines]
-    # convert start_line to 0-based indexing and ensure it's in range
-    start_line = max(0, start_line - 1)
-    # ensure end_line is within range
-    end_line = min(len(lines), end_line)
-    # return the requested lines as a list
-    return ('\n'.join(lines[start_line:end_line]) + '\n', start_line, end_line)
+    try:
+        with open(file_path.lstrip(), "r") as f:
+            # read all the lines from the file
+            lines = f.readlines()
+            # remove trailing newline characters
+            lines = [line.rstrip() for line in lines]
+        # convert start_line to 0-based indexing and ensure it's in range
+        start_line = max(0, start_line - 1)
+        # ensure end_line is within range
+        end_line = min(len(lines), end_line)
+        # return the requested lines as a list
+        return ("\n".join(lines[start_line:end_line]) + "\n", start_line, end_line)
+    except FileNotFoundError:
+        print(f"Cwhy warning: file not found: {file_path.lstrip()}")
+        return ("\n", start_line, end_line)
 
-async def complete(ctx, user_prompt):
+
+def complete(args, user_prompt):
     try:
-        completion = await openai_async.chat_complete(openai.api_key, timeout=ctx.obj['timeout'], payload={'model': ctx.obj['llm'], 'messages': [{'role': 'user', 'content': user_prompt}]})
-        completion.raise_for_status()
-        text = completion.json()['choices'][0]['message']['content']
-    except httpx.ReadTimeout:
-        print('The OpenAI API timed out. You can try increasing the timeout with the --timeout option.')
-        sys.exit(1)
-    except (openai.error.AuthenticationError, httpx.LocalProtocolError, httpx.HTTPStatusError):
-        print(traceback.format_exc())
-        print('You need an OpenAI key to use this tool.')
-        print('You can get a key here: https://platform.openai.com/account/api-keys')
-        print('Set the environment variable OPENAI_API_KEY to your key value.')
-        print('If OPENAI_API_KEY is already correctly set, you may have exceeded your usage or rate limit.')
-        sys.exit(1)
-    return text
+        completion = openai.ChatCompletion.create(
+            model=args["llm"],
+            request_timeout=args["timeout"],
+            messages=[{"role": "user", "content": user_prompt}],
+        )
+        return completion.choices[0].message.content
+    except openai.error.AuthenticationError:
+        print("You need an OpenAI key to use this tool.")
+        print("You can get a key here: https://platform.openai.com/account/api-keys")
+        print("Set the environment variable OPENAI_API_KEY to your key value.")
+        print(
+            "If OPENAI_API_KEY is already correctly set, you may have exceeded your usage or rate limit."
+        )
+    except openai.error.Timeout:
+        print(
+            "The OpenAI API timed out. You can try increasing the timeout with the --timeout option."
+        )
+
+    sys.exit(1)
+
+
+def evaluate_prompt(args, prompt, wrap=True):
+    if args["show_prompt"]:
+        print("===================== Prompt =====================")
+        print(prompt)
+        print("==================================================")
+    text = complete(args, prompt)
+    if wrap:
+        text = word_wrap_except_code_blocks(text)
+    print(text)
+
 
-class explain_context(object):
+class explain_context:
     def __init__(self, diagnostic):
-        diagnostic_lines = diagnostic.readlines()
-        diagnostic_lines = [line.decode() for line in diagnostic_lines]
+        diagnostic_lines = diagnostic.splitlines()
 
         self.code_locations = {}
 
         # Magic number - don't send more than this many code locations.
         # This is just to prevent overwhelming OpenAI.
         max_code_locations = 10
 
         # Go through the diagnostic and build up a list of code locations.
         line = 0
         while line < len(diagnostic_lines):
             # This pattern works for some C++ compilers (GCC, Clang) and Rust.
-            match = re.search(r'^([^:->]+):([0-9]+):([0-9]+)', diagnostic_lines[line])
+            match = re.search(r"^([^:->]+):([0-9]+):([0-9]+)", diagnostic_lines[line])
 
             line += 1
 
             if not match:
                 continue
 
             if max_code_locations == 0:
                 # We've found the end of the last "frame", and we don't have room
                 # for anymore, so we're done.
                 break
 
             file_name = match.group(1)
             line_number = int(match.group(2))
 
-            (abridged_code, line_start, line_end) = read_lines(file_name, line_number - 7, line_number + 2)
+            (abridged_code, line_start, line_end) = read_lines(
+                file_name, line_number - 7, line_number + 2
+            )
 
             # Avoid duplicates.
             if (file_name, line_start, line_end) not in self.code_locations:
-              self.code_locations[(file_name, line_start, line_end)] = abridged_code
-              max_code_locations -= 1
+                self.code_locations[(file_name, line_start, line_end)] = abridged_code
+                max_code_locations -= 1
 
         # If the diagnostic didn't come from a context that we know about and
         # handle in the above loop, we should make sure it's not too long.
         if not self.code_locations and line == len(diagnostic_lines) - 1:
             line = min(line, 50)
 
-        self.unabridged_diagnostic = ''.join(diagnostic_lines) + '\n'
-        self.abridged_diagnostic = '```\n' + ''.join(diagnostic_lines[:line]) + '```\n'
+        self.unabridged_diagnostic = "\n".join(diagnostic_lines) + "\n"
+        self.abridged_diagnostic = (
+            "```\n" + "\n".join(diagnostic_lines[:line]) + "```\n"
+        )
 
         def format_code_location(code_location):
             ((file_name, line_start, line_end), abridged_code) = code_location
-            s = 'File `{}` line {} to {}:\n'.format(file_name, line_start, line_end)
-            s += '\n'
-            s += '```\n'
+            s = "File `{}` line {} to {}:\n".format(file_name, line_start, line_end)
+            s += "\n"
+            s += "```\n"
             s += abridged_code
-            s += '```\n'
+            s += "```\n"
             return s
 
-        self.code = '\n'.join([format_code_location(cl) for cl in self.code_locations.items()]) + '\n'
+        self.code = (
+            "\n".join([format_code_location(cl) for cl in self.code_locations.items()])
+            + "\n"
+        )
 
-def base_prompt():
-    with io.open(sys.stdin.fileno(), "rb", closefd=False) as stdin:
-        ctx = explain_context(stdin)
-
-    if not ctx.unabridged_diagnostic.strip():
-        # Fail silently if stdin was empty
-        return ""
+
+def base_prompt(diagnostic):
+    ctx = explain_context(diagnostic)
 
     user_prompt = ""
     if ctx.code:
         user_prompt += "This is my code:\n\n"
         user_prompt += ctx.code
         user_prompt += "\n"
     user_prompt += "This is my error:\n\n"
     user_prompt += ctx.abridged_diagnostic
     user_prompt += "\n\n"
 
     return user_prompt
 
-def explain_prompt():
-    return base_prompt() + "What's the problem?"
 
-def fix_prompt():
-    return base_prompt() + "Suggest code to fix the problem. Surround the code in backticks (```)."
+def explain_prompt(diagnostic):
+    return base_prompt(diagnostic) + "What's the problem?"
 
-class extract_sources_context(object):
-    def __init__(self, diagnostic):
-        diagnostic_lines = diagnostic.readlines()
-        diagnostic_lines = [line.decode() for line in diagnostic_lines]
 
-        line = min(len(diagnostic_lines) - 1, 50)
+def fix_prompt(diagnostic):
+    return (
+        base_prompt(diagnostic)
+        + "Suggest code to fix the problem. Surround the code in backticks (```)."
+    )
 
-        self.unabridged_diagnostic = '\n'.join(diagnostic_lines) + '\n'
-        self.abridged_diagnostic = '```\n' + '\n'.join(diagnostic_lines[:line]) + '\n```\n'
 
-def extract_sources_prompt():
-    with io.open(sys.stdin.fileno(), "rb", closefd=False) as stdin:
-        ctx = extract_sources_context(stdin)
-
-    if not ctx.unabridged_diagnostic.strip():
-        # Fail silently if stdin was empty
-        return ""
+class extract_sources_context:
+    def __init__(self, diagnostic):
+        diagnostic_lines = diagnostic.splitlines()
+        line = min(len(diagnostic_lines) - 1, 50)
+        self.unabridged_diagnostic = "\n".join(diagnostic_lines) + "\n"
+        self.abridged_diagnostic = (
+            "```\n" + "\n".join(diagnostic_lines[:line]) + "\n```\n"
+        )
+
 
+def extract_sources_prompt(diagnostic):
+    ctx = extract_sources_context(diagnostic)
     user_prompt = "Respond only in the CSV format with no header row.\n"
     user_prompt += "Identify all of the file paths and associated line numbers.\n"
     user_prompt += "Output each file path and associated line number.\n"
     user_prompt += "\n"
     user_prompt += ctx.abridged_diagnostic
 
     return user_prompt
-
```

### Comparing `cwhy-0.0.4/src/cwhy.egg-info/PKG-INFO` & `cwhy-0.0.5/src/cwhy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,62 +1,90 @@
 Metadata-Version: 2.1
 Name: cwhy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Explains and proposes fixes for C/C++/Rust compiler errors.
 Author-email: Emery Berger <emery.berger@gmail.com>, Nicolas van Kempen <nvankemp@gmail.com>, Bryce Adelstein Lelbach <brycelelbach@gmail.com>
 Project-URL: Homepage, https://github.com/plasma-umass/cwhy
-Project-URL: Bug Tracker, https://github.com/plasma-umass/cwhy
+Project-URL: Bug Tracker, https://github.com/plasma-umass/cwhy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cwhy
 
-by [Emery Berger](https://emeryberger.com), [Bryce Adelstein Lelbach](https://twitter.com/blelbach?lang=en), and [Nicolas van Kempen](https://nvankempen.com/)
+by [Emery Berger](https://emeryberger.com), [Bryce Adelstein Lelbach](https://twitter.com/blelbach?lang=en), and
+[Nicolas van Kempen](https://nvankempen.com/).
 
-[![PyPI Latest Release](https://img.shields.io/pypi/v/cwhy.svg)](https://pypi.org/project/cwhy/)[![Downloads](https://pepy.tech/badge/cwhy)](https://pepy.tech/project/cwhy) [![Downloads](https://pepy.tech/badge/cwhy/month)](https://pepy.tech/project/cwhy) ![Python versions](https://img.shields.io/pypi/pyversions/cwhy.svg?style=flat-square)
+[![PyPI](https://img.shields.io/pypi/v/cwhy.svg)](https://pypi.org/project/cwhy/)
+[![downloads](https://pepy.tech/badge/cwhy)](https://pepy.tech/project/cwhy)
+[![downloads/month](https://pepy.tech/badge/cwhy/month)](https://pepy.tech/project/cwhy)
 
 ("See why")
 
-Explains and suggest fixes for C/C++/Rust compiler error messages.
+Explains and suggests fixes for C/C++/Rust compiler error messages.
 
 ## Installation
 
 ```
 python3 -m pip install cwhy
 ```
 
-*NOTE*: To use cwhy, you must first set up an OpenAI API key. If you
-already have an API key, you can set it as an environment variable
-called `OPENAI_API_KEY`. If you do not have one yet,
-you can get a key here: https://platform.openai.com/account/api-keys
+To use cwhy, you must first set up an OpenAI API key. If you already have an API key, you can set it as an environment
+variable called `OPENAI_API_KEY`. If you do not have one yet, you can
+[get a key here](https://platform.openai.com/account/api-keys).
 
-```
-export OPENAI_API_KEY=<your-api-key>
+```bash
+% export OPENAI_API_KEY=<your-api-key>
 ```
 
 ## Usage
 
-Just pipe your compiler's output to `cwhy`. `cwhy` will by default provide an explanation. If you'd like a suggested fix, add `fix`.
+### Compiler wrapper mode
+
+This new mode is recommended as CWhy will then operate in the same context as the compiler, and will do a better job
+finding the right source files.
+
+```bash
+# Invoking the compiler directly.
+% `cwhy wrapper` mycode.cpp
 
-e.g.,
+# Invoking with GNU make, using GPT-4.
+% CXX=`cwhy --llm=gpt-4 wrapper` make
 
+# Invoking with CMake, using GPT-4 and clang++.
+% cmake -DCMAKE_CXX_COMPILER=`cwhy --llm=gpt-4 wrapper --compiler=clang++` ...
 ```
-% clang++ -g mycode.cpp |& cwhy     # explanation only
-% clang++ -g mycode.cpp |& cwhy fix # to see a suggested fix
+
+### Original mode
+
+Just pipe your compiler's output to `cwhy`.
+
+```bash
+% clang++ -g mycode.cpp |& cwhy
 ```
 
+### Options
+
+These options can be displayed with `cwhy --help`.
+
+ -  `--llm`: pick a specific OpenAI LLM. CWhy has been tested with `gpt-3.5-turbo` and `gpt-4`.
+ -  `--timeout`: pick a different timeout than the default for API calls.
+ -  `--show-prompt` (debug): print prompts before calling the API.
+
+The wrapper mode specifically also has a `--compiler` option to select the underlying compiler to use.
+
 ## Examples
 
 ### C++
 
-This highlighted example is [missing-hash.cpp](test/c++/missing-hash.cpp), which is one of the first cases we experimented with.
+This highlighted example is [missing-hash.cpp](test/c++/missing-hash.cpp), which is one of the first cases we
+experimented with.
 
 <details>
 <summary>
 Expand to see the original (pretty obscure) error message:
 </summary>
 
 ```
```

