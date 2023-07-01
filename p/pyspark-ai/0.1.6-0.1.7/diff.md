# Comparing `tmp/pyspark_ai-0.1.6.tar.gz` & `tmp/pyspark_ai-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspark_ai-0.1.6.tar", max compression
+gzip compressed data, was "pyspark_ai-0.1.7.tar", max compression
```

## Comparing `pyspark_ai-0.1.6.tar` & `pyspark_ai-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 pyspark_ai-0.1.6/LICENSE
--rw-r--r--   0        0        0     4428 2023-06-29 20:50:57.072138 pyspark_ai-0.1.6/README.md
--rw-r--r--   0        0        0      998 2023-06-29 20:57:35.998349 pyspark_ai-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-23 22:14:14.484356 pyspark_ai-0.1.6/pyspark_ai/__init__.py
--rw-r--r--   0        0        0     3945 2023-06-23 22:14:14.484674 pyspark_ai-0.1.6/pyspark_ai/ai_utils.py
--rw-r--r--   0        0        0     2718 2023-06-23 22:14:14.484982 pyspark_ai-0.1.6/pyspark_ai/cache.py
--rw-r--r--   0        0        0     1905 2023-06-23 22:14:14.485144 pyspark_ai-0.1.6/pyspark_ai/code_logger.py
--rw-r--r--   0        0        0     5224 2023-06-23 22:14:14.485334 pyspark_ai-0.1.6/pyspark_ai/file_cache.py
--rw-r--r--   0        0        0     1233 2023-06-23 22:14:14.485716 pyspark_ai-0.1.6/pyspark_ai/llm_chain_with_cache.py
--rw-r--r--   0        0        0     9288 2023-06-28 23:32:33.674290 pyspark_ai-0.1.6/pyspark_ai/prompt.py
--rw-r--r--   0        0        0    17555 2023-06-29 00:12:04.660577 pyspark_ai-0.1.6/pyspark_ai/pyspark_ai.py
--rw-r--r--   0        0        0      713 2023-06-23 22:14:14.486408 pyspark_ai-0.1.6/pyspark_ai/search_tool_with_cache.py
--rw-r--r--   0        0        0     5552 1970-01-01 00:00:00.000000 pyspark_ai-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 pyspark_ai-0.1.7/LICENSE
+-rw-r--r--   0        0        0     5215 2023-07-01 05:38:10.252689 pyspark_ai-0.1.7/README.md
+-rw-r--r--   0        0        0      998 2023-07-01 05:40:38.891598 pyspark_ai-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-23 22:14:14.484356 pyspark_ai-0.1.7/pyspark_ai/__init__.py
+-rw-r--r--   0        0        0     3945 2023-06-23 22:14:14.484674 pyspark_ai-0.1.7/pyspark_ai/ai_utils.py
+-rw-r--r--   0        0        0     2718 2023-06-23 22:14:14.484982 pyspark_ai-0.1.7/pyspark_ai/cache.py
+-rw-r--r--   0        0        0     1954 2023-07-01 04:48:49.616610 pyspark_ai-0.1.7/pyspark_ai/code_logger.py
+-rw-r--r--   0        0        0     5224 2023-06-23 22:14:14.485334 pyspark_ai-0.1.7/pyspark_ai/file_cache.py
+-rw-r--r--   0        0        0     1233 2023-06-23 22:14:14.485716 pyspark_ai-0.1.7/pyspark_ai/llm_chain_with_cache.py
+-rw-r--r--   0        0        0     9288 2023-06-28 23:32:33.674290 pyspark_ai-0.1.7/pyspark_ai/prompt.py
+-rw-r--r--   0        0        0    17555 2023-06-29 00:12:04.660577 pyspark_ai-0.1.7/pyspark_ai/pyspark_ai.py
+-rw-r--r--   0        0        0      713 2023-06-23 22:14:14.486408 pyspark_ai-0.1.7/pyspark_ai/search_tool_with_cache.py
+-rw-r--r--   0        0        0     6339 1970-01-01 00:00:00.000000 pyspark_ai-0.1.7/PKG-INFO
```

### Comparing `pyspark_ai-0.1.6/LICENSE` & `pyspark_ai-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.6/README.md` & `pyspark_ai-0.1.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 <div align="center">
 
 ![English SDK for Apache Spark](./docs/_static/english-sdk-spark.svg)
-<h2>
-English is the new programming language;<br />
-Generative AI is the new compiler;<br />
-Python is ... the new byte code.
-</h2>
 </div>
 
+## Introduction
+The English SDK for Apache Spark is an extremely simple yet powerful tool. It takes English instructions and compile them into PySpark objects like DataFrames.
+Its goal is to make Spark more user-friendly and accessible, allowing you to focus your efforts on extracting insights from your data.
+
+For a more comprehensive introduction and background to our project, we have the following resources:
+- [Blog Post](https://www.databricks.com/blog/introducing-english-new-programming-language-apache-spark): A detailed walkthrough of our project.
+- [Demo Video](https://www.youtube.com/watch?v=yj7XlTB1Jvc&t=511s): DATA+AI summit announcement video with demo.
+
 ## Installation
 
 ```bash
 pip install pyspark-ai
 ```
 
 ## Configuring OpenAI LLMs
@@ -23,18 +26,25 @@
 ```
 By default, the `SparkAI` instances will use the GPT-4 model. However, you're encouraged to experiment with creating and implementing other LLMs, which can be passed during the initialization of `SparkAI` instances for various use-cases.
 
 ## Usage
 ### Initialization
 
 ```python
+from langchain.chat_models import ChatOpenAI
 from pyspark_ai import SparkAI
 
-spark_ai = SparkAI()
-spark_ai.activate()  # active partial functions for Spark DataFrame
+# If 'gpt-4' is unavailable, use 'gpt-3.5-turbo' (might lower output quality)
+llm = ChatOpenAI(model_name='gpt-4', temperature=0)
+
+# Initialize SparkAI with the ChatOpenAI model
+spark_ai = SparkAI(llm=llm, verbose=True)
+
+# Activate partial functions for Spark DataFrame
+spark_ai.activate()
 ```
 
 ### Data Ingestion
 If you have [set up the Google Python client](https://developers.google.com/docs/api/quickstart/python), you can ingest data via search engine:
 ```python
 auto_df = spark_ai.create_df("2022 USA national auto sales by brand")
 ```
```

### Comparing `pyspark_ai-0.1.6/pyproject.toml` & `pyspark_ai-0.1.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyspark-ai"
-version = "0.1.6"
+version = "0.1.7"
 description = "English SDK for Apache Spark"
 authors = ["Gengliang Wang <gengliang@apache.org>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/databrickslabs/pyspark-ai"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `pyspark_ai-0.1.6/pyspark_ai/ai_utils.py` & `pyspark_ai-0.1.7/pyspark_ai/ai_utils.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.6/pyspark_ai/cache.py` & `pyspark_ai-0.1.7/pyspark_ai/cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.6/pyspark_ai/code_logger.py` & `pyspark_ai-0.1.7/pyspark_ai/code_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,18 @@
         return GREEN + "INFO: " + RESET + super().format(record)
 
 
 class CodeLogger:
     def __init__(self, name):
         self.logger = logging.getLogger(name)
         self.logger.setLevel(logging.INFO)
-        handler = logging.StreamHandler(sys.stdout)
-        handler.setFormatter(CustomFormatter("%(message)s"))  # output only the message
-        self.logger.addHandler(handler)
+        if not self.logger.handlers:
+            handler = logging.StreamHandler(sys.stdout)
+            handler.setFormatter(CustomFormatter("%(message)s"))  # output only the message
+            self.logger.addHandler(handler)
 
     @staticmethod
     def colorize_code(code, language):
         if not language or language.lower() == "python":
             lexer = PythonLexer()
         elif language.lower() == "sql":
             lexer = SqlLexer()
```

### Comparing `pyspark_ai-0.1.6/pyspark_ai/file_cache.py` & `pyspark_ai-0.1.7/pyspark_ai/file_cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.6/pyspark_ai/llm_chain_with_cache.py` & `pyspark_ai-0.1.7/pyspark_ai/llm_chain_with_cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.6/pyspark_ai/prompt.py` & `pyspark_ai-0.1.7/pyspark_ai/prompt.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.6/pyspark_ai/pyspark_ai.py` & `pyspark_ai-0.1.7/pyspark_ai/pyspark_ai.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.6/pyspark_ai/search_tool_with_cache.py` & `pyspark_ai-0.1.7/pyspark_ai/search_tool_with_cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.6/PKG-INFO` & `pyspark_ai-0.1.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspark-ai
-Version: 0.1.6
+Version: 0.1.7
 Summary: English SDK for Apache Spark
 Home-page: https://github.com/databrickslabs/pyspark-ai
 License: Apache-2.0
 Author: Gengliang Wang
 Author-email: gengliang@apache.org
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
@@ -26,21 +26,24 @@
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tiktoken (==0.4.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 ![English SDK for Apache Spark](./docs/_static/english-sdk-spark.svg)
-<h2>
-English is the new programming language;<br />
-Generative AI is the new compiler;<br />
-Python is ... the new byte code.
-</h2>
 </div>
 
+## Introduction
+The English SDK for Apache Spark is an extremely simple yet powerful tool. It takes English instructions and compile them into PySpark objects like DataFrames.
+Its goal is to make Spark more user-friendly and accessible, allowing you to focus your efforts on extracting insights from your data.
+
+For a more comprehensive introduction and background to our project, we have the following resources:
+- [Blog Post](https://www.databricks.com/blog/introducing-english-new-programming-language-apache-spark): A detailed walkthrough of our project.
+- [Demo Video](https://www.youtube.com/watch?v=yj7XlTB1Jvc&t=511s): DATA+AI summit announcement video with demo.
+
 ## Installation
 
 ```bash
 pip install pyspark-ai
 ```
 
 ## Configuring OpenAI LLMs
@@ -52,18 +55,25 @@
 ```
 By default, the `SparkAI` instances will use the GPT-4 model. However, you're encouraged to experiment with creating and implementing other LLMs, which can be passed during the initialization of `SparkAI` instances for various use-cases.
 
 ## Usage
 ### Initialization
 
 ```python
+from langchain.chat_models import ChatOpenAI
 from pyspark_ai import SparkAI
 
-spark_ai = SparkAI()
-spark_ai.activate()  # active partial functions for Spark DataFrame
+# If 'gpt-4' is unavailable, use 'gpt-3.5-turbo' (might lower output quality)
+llm = ChatOpenAI(model_name='gpt-4', temperature=0)
+
+# Initialize SparkAI with the ChatOpenAI model
+spark_ai = SparkAI(llm=llm, verbose=True)
+
+# Activate partial functions for Spark DataFrame
+spark_ai.activate()
 ```
 
 ### Data Ingestion
 If you have [set up the Google Python client](https://developers.google.com/docs/api/quickstart/python), you can ingest data via search engine:
 ```python
 auto_df = spark_ai.create_df("2022 USA national auto sales by brand")
 ```
```

