# Comparing `tmp/atksh-utils-0.2.0.tar.gz` & `tmp/atksh-utils-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atksh-utils-0.2.0.tar", last modified: Mon Jun 19 02:21:51 2023, max compression
+gzip compressed data, was "atksh-utils-0.2.1.tar", last modified: Sat Jul  1 05:54:42 2023, max compression
```

## Comparing `atksh-utils-0.2.0.tar` & `atksh-utils-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:21:51.911514 atksh-utils-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:21:51.907514 atksh-utils-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:21:51.907514 atksh-utils-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-19 02:21:51.911514 atksh-utils-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-19 02:21:51.911514 atksh-utils-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:21:51.907514 atksh-utils-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:21:51.907514 atksh-utils-0.2.0/src/atksh_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/src/atksh_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:21:51.911514 atksh-utils-0.2.0/src/atksh_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/src/atksh_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10340 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/src/atksh_utils/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/src/atksh_utils/openai/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/src/atksh_utils/openai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/src/atksh_utils/openai/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 02:21:51.000000 atksh-utils-0.2.0/src/atksh_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:21:51.907514 atksh-utils-0.2.0/src/atksh_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-19 02:21:51.000000 atksh-utils-0.2.0/src/atksh_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-19 02:21:51.000000 atksh-utils-0.2.0/src/atksh_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 02:21:51.000000 atksh-utils-0.2.0/src/atksh_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-19 02:21:51.000000 atksh-utils-0.2.0/src/atksh_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 02:21:51.000000 atksh-utils-0.2.0/src/atksh_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:21:51.907514 atksh-utils-0.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:21:51.911514 atksh-utils-0.2.0/tests/openai/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/tests/openai/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-19 02:21:36.000000 atksh-utils-0.2.0/tests/openai/test_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:54:42.876316 atksh-utils-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:54:42.872316 atksh-utils-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:54:42.872316 atksh-utils-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-01 05:54:42.876316 atksh-utils-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-01 05:54:42.876316 atksh-utils-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:54:42.872316 atksh-utils-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:54:42.872316 atksh-utils-0.2.1/src/atksh_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/src/atksh_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:54:42.876316 atksh-utils-0.2.1/src/atksh_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/src/atksh_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10340 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/src/atksh_utils/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/src/atksh_utils/openai/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/src/atksh_utils/openai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/src/atksh_utils/openai/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-01 05:54:42.000000 atksh-utils-0.2.1/src/atksh_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:54:42.872316 atksh-utils-0.2.1/src/atksh_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-01 05:54:42.000000 atksh-utils-0.2.1/src/atksh_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-01 05:54:42.000000 atksh-utils-0.2.1/src/atksh_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 05:54:42.000000 atksh-utils-0.2.1/src/atksh_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-01 05:54:42.000000 atksh-utils-0.2.1/src/atksh_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-01 05:54:42.000000 atksh-utils-0.2.1/src/atksh_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:54:42.872316 atksh-utils-0.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:54:42.876316 atksh-utils-0.2.1/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/tests/openai/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/tests/openai/test_functional.py
```

### Comparing `atksh-utils-0.2.0/.github/workflows/publish_to_pypi.yaml` & `atksh-utils-0.2.1/.github/workflows/publish_to_pypi.yaml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.2.0/.gitignore` & `atksh-utils-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.2.0/LICENSE` & `atksh-utils-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.2.0/PKG-INFO` & `atksh-utils-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.2.0
+Version: 0.2.1
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
         
@@ -101,36 +101,21 @@
     :param b: An integer.
     :type b: int
     :return: The sum of a and b.
     :rtype: int
     """
     return a // b
 
-
-def exec_python_code(code: str) -> str:
-    """This is a function that executes Python code and returns the stdout. Don't forget to print the result.
-
-    :param code: A string of Python code.
-    :type code: str
-    :return: The result of the execution of the Python code (stdout by print)
-    :rtype: str
-    """
-    import tempfile
-    import subprocess
-    with tempfile.NamedTemporaryFile(mode="w", suffix=".py") as f:
-        f.write(code)
-        f.flush()
-        result = subprocess.check_output(["python", f.name])
-    result = result.decode("utf-8").strip()
-    if result == "":
-        result = "NotPrintedError('The result is not printed.')"
-    return result
-
 ai.set_function(mul)
 ai.set_function(add)
 ai.set_function(sub)
 ai.set_function(div)
-ai.set_function(exec_python_code)
 
-print(ai("Just answer the value of (5243 + 642) x (5314 - 4231) // 100"))
+print(ai("Just answer the value of (5243 + 642) x (5314 - 4231) // 100")[1])
 # The value of (5243 + 642) x (5314 - 4231) // 100 is 63734.
+
+
+ai = OpenAI(key, "gpt-3.5-turbo-0613")
+ai.set_browser_functions()
+print(ai("How the weather in Tokyo?")[1])
+# The current weather in Tokyo varies depending on the source. According to AccuWeather, it is partly sunny with a temperature of 89°F. BBC Weather predicts thundery showers tonight with a low temperature of 22°C. Timeanddate.com reports an overcast sky with a temperature of 82°F. The Weather Network and The Weather Channel provide forecasts for the next 7 and 13 days respectively. Weather Underground also offers weather conditions for Tokyo and other cities.
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `atksh-utils-0.2.0/README.md` & `atksh-utils-0.2.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -68,36 +68,21 @@
     :param b: An integer.
     :type b: int
     :return: The sum of a and b.
     :rtype: int
     """
     return a // b
 
-
-def exec_python_code(code: str) -> str:
-    """This is a function that executes Python code and returns the stdout. Don't forget to print the result.
-
-    :param code: A string of Python code.
-    :type code: str
-    :return: The result of the execution of the Python code (stdout by print)
-    :rtype: str
-    """
-    import tempfile
-    import subprocess
-    with tempfile.NamedTemporaryFile(mode="w", suffix=".py") as f:
-        f.write(code)
-        f.flush()
-        result = subprocess.check_output(["python", f.name])
-    result = result.decode("utf-8").strip()
-    if result == "":
-        result = "NotPrintedError('The result is not printed.')"
-    return result
-
 ai.set_function(mul)
 ai.set_function(add)
 ai.set_function(sub)
 ai.set_function(div)
-ai.set_function(exec_python_code)
 
-print(ai("Just answer the value of (5243 + 642) x (5314 - 4231) // 100"))
+print(ai("Just answer the value of (5243 + 642) x (5314 - 4231) // 100")[1])
 # The value of (5243 + 642) x (5314 - 4231) // 100 is 63734.
+
+
+ai = OpenAI(key, "gpt-3.5-turbo-0613")
+ai.set_browser_functions()
+print(ai("How the weather in Tokyo?")[1])
+# The current weather in Tokyo varies depending on the source. According to AccuWeather, it is partly sunny with a temperature of 89°F. BBC Weather predicts thundery showers tonight with a low temperature of 22°C. Timeanddate.com reports an overcast sky with a temperature of 82°F. The Weather Network and The Weather Channel provide forecasts for the next 7 and 13 days respectively. Weather Underground also offers weather conditions for Tokyo and other cities.
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `atksh-utils-0.2.0/pyproject.toml` & `atksh-utils-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 requires = ["setuptools>=62.6", "setuptools_scm[toml]>=6.2", "wheel"]
 
 [project]
 dependencies = [
   "openai>=0.27.8",
   "beautifulsoup4>=4.12.2,<5.0.0",
   "requests>=2.26.0,<3.0.0",
+  "duckduckgo_search>=3.8.3,<4.0.0",
 ]
 description = "atksh's utils"
 dynamic = ["version"]
 license = {file = "LICENSE"}
 name = "atksh-utils"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `atksh-utils-0.2.0/src/atksh_utils/openai/api.py` & `atksh-utils-0.2.1/src/atksh_utils/openai/api.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.2.0/src/atksh_utils/openai/functional.py` & `atksh-utils-0.2.1/src/atksh_utils/openai/functional.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.2.0/src/atksh_utils/openai/prompt.py` & `atksh-utils-0.2.1/src/atksh_utils/openai/prompt.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 - When writing some examples, you must clearly indicate that it is giving examples, rather than speaking as if it's generality.
 - The language of your response must match the language of the input.
 - The temperature is set to 0 so you will generate the precise response.
 {more}
 
 Let’s work this out in a step-by-step way to be sure we have the right answer!
 If you make mistakes in your output, a large number of people will certainly die.
+
+Now, let's answer the following questions.
 """
 
 
 def generate_react_prompt(turn: str) -> str:
     turn = turn.lower()
     assert turn in {"analyze", "plan", "act"}
     return f"""
@@ -38,14 +40,16 @@
     - Input: The current state, the action to be performed and the summary.
     - Output: The new state and the report of the action.
 
 Note that your simulation will be needed to perform actions since you have no physical body but know widely about the world.
 
 Now, you will do the {turn} task.
 Let’s work this out in a step-by-step way to be sure we have the right answer! If you make mistakes in your output, a large number of people will certainly die.
+
+Don't forget to use another function like web_search, visit_page, and so on for analyze, plan, and act tasks.
 """
 
 
 SUMMARIZE_PROMPT = """
 You are SummarizeGPT, an expert summarizer of information with respect to the given query.
 You will organize the information in a mutually exclusive and collectively exhaustive manner.
 You will write in markdown format, and nest items for simplicity.
```

### Comparing `atksh-utils-0.2.0/src/atksh_utils/openai/tool.py` & `atksh-utils-0.2.1/src/atksh_utils/openai/tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 
 MAX_ATTEMPTS = 3
 MAX_SEARCH_RESULTS = 8
 
 
 def get_browser_functions(ai: "OpenAI"):
     child = ai.make_child(model_name="gpt-3.5-turbo-16k")
-    child.set_system_prompt(SUMMARIZE_PROMPT + "\nPlease include url links.")
+    child.set_system_prompt(
+        SUMMARIZE_PROMPT + "\nPlease include URL links; otherwise, the following will fail."
+    )
 
     def _summarize(query_text: str, results: str) -> str:
         """Summarizes the query text and results."""
         return child(f"Query: {query_text}\nResults: {results}\nSummary: ")[1]
 
     def web_search(query_text: str) -> str:
         """Searches the web for the query text.
@@ -49,14 +51,17 @@
         :param query_text: The text to query for summarization.
         :type query_text: str
         :param url: The url to visit (must be a valid url like `https://commerce-flow.com/request_brochure/`)
         :type url: str
         :return: The summarized text of the page.
         :rtype: str
         """
-        response = requests.get(url)
-        soup = bs4(response.text, "html.parser")
-        body = soup.find("body").text.strip()
-        ret = _summarize(query_text, body[:10000])
+        try:
+            response = requests.get(url)
+            soup = bs4(response.text, "html.parser")
+            body = soup.find("body").text.strip()
+            ret = _summarize(query_text, body[:10000])
+        except Exception as e:
+            ret = f"Error: {e}.\nPlease try again or try another url."
         return ret
 
     return web_search, visit_page
```

### Comparing `atksh-utils-0.2.0/src/atksh_utils.egg-info/PKG-INFO` & `atksh-utils-0.2.1/src/atksh_utils.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.2.0
+Version: 0.2.1
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
         
@@ -101,36 +101,21 @@
     :param b: An integer.
     :type b: int
     :return: The sum of a and b.
     :rtype: int
     """
     return a // b
 
-
-def exec_python_code(code: str) -> str:
-    """This is a function that executes Python code and returns the stdout. Don't forget to print the result.
-
-    :param code: A string of Python code.
-    :type code: str
-    :return: The result of the execution of the Python code (stdout by print)
-    :rtype: str
-    """
-    import tempfile
-    import subprocess
-    with tempfile.NamedTemporaryFile(mode="w", suffix=".py") as f:
-        f.write(code)
-        f.flush()
-        result = subprocess.check_output(["python", f.name])
-    result = result.decode("utf-8").strip()
-    if result == "":
-        result = "NotPrintedError('The result is not printed.')"
-    return result
-
 ai.set_function(mul)
 ai.set_function(add)
 ai.set_function(sub)
 ai.set_function(div)
-ai.set_function(exec_python_code)
 
-print(ai("Just answer the value of (5243 + 642) x (5314 - 4231) // 100"))
+print(ai("Just answer the value of (5243 + 642) x (5314 - 4231) // 100")[1])
 # The value of (5243 + 642) x (5314 - 4231) // 100 is 63734.
+
+
+ai = OpenAI(key, "gpt-3.5-turbo-0613")
+ai.set_browser_functions()
+print(ai("How the weather in Tokyo?")[1])
+# The current weather in Tokyo varies depending on the source. According to AccuWeather, it is partly sunny with a temperature of 89°F. BBC Weather predicts thundery showers tonight with a low temperature of 22°C. Timeanddate.com reports an overcast sky with a temperature of 82°F. The Weather Network and The Weather Channel provide forecasts for the next 7 and 13 days respectively. Weather Underground also offers weather conditions for Tokyo and other cities.
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `atksh-utils-0.2.0/src/atksh_utils.egg-info/SOURCES.txt` & `atksh-utils-0.2.1/src/atksh_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.2.0/tests/openai/test_api.py` & `atksh-utils-0.2.1/tests/openai/test_api.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.2.0/tests/openai/test_functional.py` & `atksh-utils-0.2.1/tests/openai/test_functional.py`

 * *Files identical despite different names*

