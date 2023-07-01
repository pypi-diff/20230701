# Comparing `tmp/betabageldb-0.1.0.tar.gz` & `tmp/betabageldb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betabageldb-0.1.0.tar", last modified: Thu Jun 29 05:53:26 2023, max compression
+gzip compressed data, was "betabageldb-0.1.1.tar", last modified: Sat Jul  1 11:34:05 2023, max compression
```

## Comparing `betabageldb-0.1.0.tar` & `betabageldb-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-06-29 05:53:26.353785 betabageldb-0.1.0/
--rw-r--r--   0 bidhan     (501) staff       (20)     4246 2023-06-27 19:16:56.000000 betabageldb-0.1.0/BagelDB.py
--rw-r--r--   0 bidhan     (501) staff       (20)       82 2023-06-27 19:31:31.000000 betabageldb-0.1.0/LICENSE.txt
--rw-r--r--   0 bidhan     (501) staff       (20)     2795 2023-06-29 05:53:26.353557 betabageldb-0.1.0/PKG-INFO
--rw-r--r--   0 bidhan     (501) staff       (20)     2164 2023-06-27 19:30:12.000000 betabageldb-0.1.0/README.md
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-06-29 05:53:26.353104 betabageldb-0.1.0/betabageldb.egg-info/
--rw-r--r--   0 bidhan     (501) staff       (20)     2795 2023-06-29 05:53:26.000000 betabageldb-0.1.0/betabageldb.egg-info/PKG-INFO
--rw-r--r--   0 bidhan     (501) staff       (20)      215 2023-06-29 05:53:26.000000 betabageldb-0.1.0/betabageldb.egg-info/SOURCES.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        1 2023-06-29 05:53:26.000000 betabageldb-0.1.0/betabageldb.egg-info/dependency_links.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        9 2023-06-29 05:53:26.000000 betabageldb-0.1.0/betabageldb.egg-info/requires.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        8 2023-06-29 05:53:26.000000 betabageldb-0.1.0/betabageldb.egg-info/top_level.txt
--rw-r--r--   0 bidhan     (501) staff       (20)       38 2023-06-29 05:53:26.353823 betabageldb-0.1.0/setup.cfg
--rw-r--r--   0 bidhan     (501) staff       (20)      795 2023-06-29 05:52:39.000000 betabageldb-0.1.0/setup.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-01 11:34:05.271417 betabageldb-0.1.1/
+-rw-r--r--   0 bidhan     (501) staff       (20)     5921 2023-07-01 11:14:26.000000 betabageldb-0.1.1/BagelDB.py
+-rw-r--r--   0 bidhan     (501) staff       (20)       82 2023-06-27 19:31:31.000000 betabageldb-0.1.1/LICENSE.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)     4384 2023-07-01 11:34:05.270875 betabageldb-0.1.1/PKG-INFO
+-rw-r--r--   0 bidhan     (501) staff       (20)     3753 2023-07-01 11:28:45.000000 betabageldb-0.1.1/README.md
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-01 11:34:05.270414 betabageldb-0.1.1/betabageldb.egg-info/
+-rw-r--r--   0 bidhan     (501) staff       (20)     4384 2023-07-01 11:34:05.000000 betabageldb-0.1.1/betabageldb.egg-info/PKG-INFO
+-rw-r--r--   0 bidhan     (501) staff       (20)      215 2023-07-01 11:34:05.000000 betabageldb-0.1.1/betabageldb.egg-info/SOURCES.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        1 2023-07-01 11:34:05.000000 betabageldb-0.1.1/betabageldb.egg-info/dependency_links.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        9 2023-07-01 11:34:05.000000 betabageldb-0.1.1/betabageldb.egg-info/requires.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        8 2023-07-01 11:34:05.000000 betabageldb-0.1.1/betabageldb.egg-info/top_level.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)       38 2023-07-01 11:34:05.271474 betabageldb-0.1.1/setup.cfg
+-rw-r--r--   0 bidhan     (501) staff       (20)      795 2023-07-01 11:33:50.000000 betabageldb-0.1.1/setup.py
```

### Comparing `betabageldb-0.1.0/PKG-INFO` & `betabageldb-0.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,83 @@
-Metadata-Version: 2.1
-Name: betabageldb
-Version: 0.1.0
-Summary: BagelDB is a Python library for interacting with the BagelDB API.
-Home-page: https://github.com/Bagel-DB/Client
-Author: Bidhan Roy
-Author-email: bidhan@bageldb.ai
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-Sure, here's a step-by-step guide on how to use the `BagelDB` Python client:
+Here's a step by step guide on how to use BagelDB python client.
 
 1. **Import the `BagelDB` client**
 
    Start by importing the `BagelDB` client into your Python script.
 
    ```python
-   from BagelDB import BagelDB
+   from betabageldb import BagelDB
    ```
 
 2. **Initialize the BagelDB client**
 
-   Next, initialize a new instance of the `BagelDB` client. Make sure you have your OpenAI API key set in your environment variables as `OPENAI_API_KEY`. 
+   Initialize a new instance of the `BagelDB` client. You need to specify the index you want to work with at this stage. This index will be used for all subsequent insertions and searches. Make sure you have your OpenAI API key set in your environment variables as `OPENAI_API_KEY`.
 
    ```python
-   db = BagelDB()
+   index = "myIndex"
+   db = BagelDB(index)
    ```
 
 3. **Ping the BagelDB server**
 
-   To check the connection to the BagelDB server, you can use the `ping()` method. This method will return a response from the BagelDB API in JSON format. 
+   To check the connection to the BagelDB server, you can use the `ping()` method. This method will return a response from the BagelDB API in JSON format.
 
    ```python
    response = db.ping()
    print(response)
    ```
 
 4. **Get OpenAI embeddings**
 
-   Use the `getOpenAIEmbedding(inputText, model='text-embedding-ada-002')` method to get embeddings from OpenAI. The `inputText` is the text for which embeddings are required. `model` is optional and defaults to 'text-embedding-ada-002'. 
+   Use the `getOpenAIEmbedding(inputText, model='text-embedding-ada-002')` method to get embeddings from OpenAI. The `inputText` is the text for which embeddings are required. `model` is optional and defaults to 'text-embedding-ada-002'.
 
    ```python
    input_text = "Some text"
    embeddings = db.getOpenAIEmbedding(input_text)
    print(embeddings)
    ```
 
 5. **Insert vectors into BagelDB**
 
-   To insert vectors into a given index in BagelDB, use the `insert(index, vectors)` method. `index` is the index in which vectors are to be inserted, and `vectors` is a list of vectors to be inserted.
+   To insert vectors into BagelDB, use the `insert(vectors)` method. `vectors` is a list of vectors to be inserted. The index is already set during the initialization of the BagelDB client and is not required here.
 
    ```python
-   index = "myIndex"
    vectors = [{'id': 'vec1', 'values': [0.1, 0.2, 0.3], 'metadata': {'key': 'value'}}]
-   insert_response = db.insert(index, vectors)
+   insert_response = db.insert(vectors)
    print(insert_response)
    ```
 
 6. **Search for a vector in BagelDB**
 
-   To search for a vector in a given index in BagelDB, use the `search(index, vector)` method. `index` is the index in which the search is to be performed, and `vector` is the vector for which the search is to be performed.
+   To search for a vector in BagelDB, use the `search(vector)` method. `vector` is the vector for which the search is to be performed. The index is already set during the initialization of the BagelDB client and is not required here.
 
    ```python
-   index = "myIndex"
    vector = [0.1, 0.2, 0.3]
-   search_response = db.search(index, vector)
+   search_response = db.search(vector)
    print(search_response)
    ```
 
 Remember to handle exceptions in your application. The methods in the `BagelDB` client can raise exceptions if a network error occurs or if the response from the server indicates a failed HTTP status code.
+
+7. **Insert vectors from texts**
+
+   The `insertFromTexts(texts, model='text-embedding-ada-002')` method can be used to convert a list of texts to their respective embeddings and insert these as vectors into BagelDB. The `texts` parameter is a list of strings for which embeddings are required, and `model` is optional and defaults to 'text-embedding-ada-002'. Each vector will be assigned an id incrementally starting from 0 and metadata will contain original text.
+
+   ```python
+   texts = ["Some text 1", "Some text 2"]
+   insert_response = db.insertFromTexts(texts)
+   print(insert_response)
+   ```
+
+8. **Search for a vector from text**
+
+   To search for a vector derived from a given text in BagelDB, you can use the `searchFromText(text, model='text-embedding-ada-002')` method. `text` is the string for which the corresponding embedding is to be found and searched, and `model` is optional and defaults to 'text-embedding-ada-002'. 
+
+   ```python
+   text = "Some text"
+   search_response = db.searchFromText(text)
+   print(search_response)
+   ```
+
+These new methods, `insertFromTexts` and `searchFromText`, simplify the process of converting text to embeddings and performing operations on BagelDB, providing a higher level of abstraction for users to work with.
+
+Remember to handle exceptions in your application. The methods in the `BagelDB` client can raise exceptions if a network error occurs or if the response from the server indicates a failed HTTP status code.
```

### Comparing `betabageldb-0.1.0/betabageldb.egg-info/PKG-INFO` & `betabageldb-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,77 +1,100 @@
 Metadata-Version: 2.1
 Name: betabageldb
-Version: 0.1.0
+Version: 0.1.1
 Summary: BagelDB is a Python library for interacting with the BagelDB API.
 Home-page: https://github.com/Bagel-DB/Client
 Author: Bidhan Roy
 Author-email: bidhan@bageldb.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-Sure, here's a step-by-step guide on how to use the `BagelDB` Python client:
+Here's a step by step guide on how to use BagelDB python client.
 
 1. **Import the `BagelDB` client**
 
    Start by importing the `BagelDB` client into your Python script.
 
    ```python
-   from BagelDB import BagelDB
+   from betabageldb import BagelDB
    ```
 
 2. **Initialize the BagelDB client**
 
-   Next, initialize a new instance of the `BagelDB` client. Make sure you have your OpenAI API key set in your environment variables as `OPENAI_API_KEY`. 
+   Initialize a new instance of the `BagelDB` client. You need to specify the index you want to work with at this stage. This index will be used for all subsequent insertions and searches. Make sure you have your OpenAI API key set in your environment variables as `OPENAI_API_KEY`.
 
    ```python
-   db = BagelDB()
+   index = "myIndex"
+   db = BagelDB(index)
    ```
 
 3. **Ping the BagelDB server**
 
-   To check the connection to the BagelDB server, you can use the `ping()` method. This method will return a response from the BagelDB API in JSON format. 
+   To check the connection to the BagelDB server, you can use the `ping()` method. This method will return a response from the BagelDB API in JSON format.
 
    ```python
    response = db.ping()
    print(response)
    ```
 
 4. **Get OpenAI embeddings**
 
-   Use the `getOpenAIEmbedding(inputText, model='text-embedding-ada-002')` method to get embeddings from OpenAI. The `inputText` is the text for which embeddings are required. `model` is optional and defaults to 'text-embedding-ada-002'. 
+   Use the `getOpenAIEmbedding(inputText, model='text-embedding-ada-002')` method to get embeddings from OpenAI. The `inputText` is the text for which embeddings are required. `model` is optional and defaults to 'text-embedding-ada-002'.
 
    ```python
    input_text = "Some text"
    embeddings = db.getOpenAIEmbedding(input_text)
    print(embeddings)
    ```
 
 5. **Insert vectors into BagelDB**
 
-   To insert vectors into a given index in BagelDB, use the `insert(index, vectors)` method. `index` is the index in which vectors are to be inserted, and `vectors` is a list of vectors to be inserted.
+   To insert vectors into BagelDB, use the `insert(vectors)` method. `vectors` is a list of vectors to be inserted. The index is already set during the initialization of the BagelDB client and is not required here.
 
    ```python
-   index = "myIndex"
    vectors = [{'id': 'vec1', 'values': [0.1, 0.2, 0.3], 'metadata': {'key': 'value'}}]
-   insert_response = db.insert(index, vectors)
+   insert_response = db.insert(vectors)
    print(insert_response)
    ```
 
 6. **Search for a vector in BagelDB**
 
-   To search for a vector in a given index in BagelDB, use the `search(index, vector)` method. `index` is the index in which the search is to be performed, and `vector` is the vector for which the search is to be performed.
+   To search for a vector in BagelDB, use the `search(vector)` method. `vector` is the vector for which the search is to be performed. The index is already set during the initialization of the BagelDB client and is not required here.
 
    ```python
-   index = "myIndex"
    vector = [0.1, 0.2, 0.3]
-   search_response = db.search(index, vector)
+   search_response = db.search(vector)
+   print(search_response)
+   ```
+
+Remember to handle exceptions in your application. The methods in the `BagelDB` client can raise exceptions if a network error occurs or if the response from the server indicates a failed HTTP status code.
+
+7. **Insert vectors from texts**
+
+   The `insertFromTexts(texts, model='text-embedding-ada-002')` method can be used to convert a list of texts to their respective embeddings and insert these as vectors into BagelDB. The `texts` parameter is a list of strings for which embeddings are required, and `model` is optional and defaults to 'text-embedding-ada-002'. Each vector will be assigned an id incrementally starting from 0 and metadata will contain original text.
+
+   ```python
+   texts = ["Some text 1", "Some text 2"]
+   insert_response = db.insertFromTexts(texts)
+   print(insert_response)
+   ```
+
+8. **Search for a vector from text**
+
+   To search for a vector derived from a given text in BagelDB, you can use the `searchFromText(text, model='text-embedding-ada-002')` method. `text` is the string for which the corresponding embedding is to be found and searched, and `model` is optional and defaults to 'text-embedding-ada-002'. 
+
+   ```python
+   text = "Some text"
+   search_response = db.searchFromText(text)
    print(search_response)
    ```
 
+These new methods, `insertFromTexts` and `searchFromText`, simplify the process of converting text to embeddings and performing operations on BagelDB, providing a higher level of abstraction for users to work with.
+
 Remember to handle exceptions in your application. The methods in the `BagelDB` client can raise exceptions if a network error occurs or if the response from the server indicates a failed HTTP status code.
```

### Comparing `betabageldb-0.1.0/setup.py` & `betabageldb-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="betabageldb",
-    version="0.1.0",
+    version="0.1.1",
     description="BagelDB is a Python library for interacting with the BagelDB API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Bidhan Roy",
     author_email="bidhan@bageldb.ai",
     url="https://github.com/Bagel-DB/Client",
     py_modules=["BagelDB"],
```

