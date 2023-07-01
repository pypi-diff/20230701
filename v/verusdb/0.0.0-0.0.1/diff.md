# Comparing `tmp/verusdb-0.0.0.tar.gz` & `tmp/verusdb-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verusdb-0.0.0.tar", max compression
+gzip compressed data, was "verusdb-0.0.1.tar", max compression
```

## Comparing `verusdb-0.0.0.tar` & `verusdb-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1070 2023-06-17 06:40:55.359565 verusdb-0.0.0/LICENSE
--rw-r--r--   0        0        0     3329 2023-06-19 06:57:13.788015 verusdb-0.0.0/README.md
--rw-r--r--   0        0        0      590 2023-06-20 17:58:35.928188 verusdb-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      135 2023-06-20 17:56:50.228219 verusdb-0.0.0/verusdb/__init__.py
--rw-r--r--   0        0        0     2215 2023-06-18 19:24:41.462883 verusdb-0.0.0/verusdb/client.py
--rw-r--r--   0        0        0      361 2023-06-18 07:26:49.191853 verusdb-0.0.0/verusdb/embeddings/__init__.py
--rw-r--r--   0        0        0     1106 2023-06-18 06:14:06.648099 verusdb-0.0.0/verusdb/embeddings/openai.py
--rw-r--r--   0        0        0      620 2023-06-18 06:36:00.194796 verusdb-0.0.0/verusdb/engines/__init__.py
--rw-r--r--   0        0        0     6143 2023-06-18 19:13:02.225802 verusdb-0.0.0/verusdb/engines/polars.py
--rw-r--r--   0        0        0     6469 2023-06-19 19:15:18.677570 verusdb-0.0.0/verusdb/engines/redis.py
--rw-r--r--   0        0        0     1396 2023-06-18 19:22:05.381266 verusdb-0.0.0/verusdb/settings.py
--rw-r--r--   0        0        0        0 2023-06-15 19:35:29.018878 verusdb-0.0.0/verusdb/utils.py
--rw-r--r--   0        0        0     3928 1970-01-01 00:00:00.000000 verusdb-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-17 06:40:55.359565 verusdb-0.0.1/LICENSE
+-rw-r--r--   0        0        0     3782 2023-07-01 05:12:22.862028 verusdb-0.0.1/README.md
+-rw-r--r--   0        0        0      610 2023-07-01 06:39:02.599491 verusdb-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      135 2023-07-01 06:39:16.259482 verusdb-0.0.1/verusdb/__init__.py
+-rw-r--r--   0        0        0     2975 2023-07-01 06:37:36.379495 verusdb-0.0.1/verusdb/client.py
+-rw-r--r--   0        0        0      361 2023-06-18 07:26:49.191853 verusdb-0.0.1/verusdb/embeddings/__init__.py
+-rw-r--r--   0        0        0     1106 2023-07-01 06:38:17.569499 verusdb-0.0.1/verusdb/embeddings/openai.py
+-rw-r--r--   0        0        0      552 2023-06-21 20:45:07.559810 verusdb-0.0.1/verusdb/engines/__init__.py
+-rw-r--r--   0        0        0     7987 2023-07-01 06:38:07.369500 verusdb-0.0.1/verusdb/engines/polars.py
+-rw-r--r--   0        0        0     6157 2023-07-01 06:38:00.979499 verusdb-0.0.1/verusdb/engines/postgresql.py
+-rw-r--r--   0        0        0     8177 2023-06-29 17:48:39.971488 verusdb-0.0.1/verusdb/engines/redis.py
+-rw-r--r--   0        0        0     1924 2023-07-01 06:37:47.009497 verusdb-0.0.1/verusdb/settings.py
+-rw-r--r--   0        0        0      297 2023-07-01 06:38:27.809496 verusdb-0.0.1/verusdb/utils.py
+-rw-r--r--   0        0        0     4422 1970-01-01 00:00:00.000000 verusdb-0.0.1/PKG-INFO
```

### Comparing `verusdb-0.0.0/LICENSE` & `verusdb-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `verusdb-0.0.0/README.md` & `verusdb-0.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,13 @@
 # Verus
 
 Verus is a powerful, lightweight and flexible vector store that is designed to work seamlessly with multiple databases. It is built with LLM in mind, making it an ideal choice for natural language processing, information retrieval, and recommendation systems.
 
 One of the key benefits of Verus is its agnostic design, which allows it to integrate with a wide range of databases. This means that you can use Verus with your existing database infrastructure, without having to worry about compatibility issues.
 
-## TODOs
-- [ ] Redis Integration
-- [ ] PostgreSQL Integration
-- [ ] DuckDB Integration
-- [ ] CosmosDB Intergration
-- [ ] Benchmarking
-
-
 ## Installation
 
 You can install VerusDB using pip:
 
 `pip install verusdb`
 
 ## Usage
@@ -37,41 +29,40 @@
 
 # Search for documents
 response = client.search(text='what is my first document?')
 ```
 
 This will output a list of documents that match the search query, along with their metadata and a cosine similarity score. You can adjust the the number of results you obtain by relevance
 
-
 ```json
 [
   {
     "collection": "MyCollection",
     "text": "This is my first document",
     "metadata": {
       "source": "input",
-      "pages": "5"}
-    ,
+      "pages": "5"
+    },
     "score": 0.937450967393278
   },
   {
     "collection": "MyCollection",
     "text": "This is my second document",
     "metadata": {
       "source": "input",
-      "pages": "5"}
-    ,
+      "pages": "5"
+    },
     "score": 0.8927016698439493
   }
 ]
 ```
 
 # Configuration
 
-You can configure VerusDB by passing a Settings object to the VerusClient constructor. The Settings object allows you to specify the folder where the database files will be stored, the storage engine to use (currently Polars and Redis are supported), 
+You can configure VerusDB by passing a Settings object to the VerusClient constructor. The Settings object allows you to specify the folder where the database files will be stored, the storage engine to use (currently Polars and Redis are supported),
 
 ## Polars
 
 ```python
 from verusdb.settings import Settings
 from verusdb.client import VerusClient
 from verusdb.embeddings.openai import OpenAIEmbeddingsEngine
@@ -80,14 +71,15 @@
 settings = Settings(
     folder='data',
     engine='polars',
     embeddings=OpenAIEmbeddingsEngine(key='my-openai-api-key')
 )
 client = VerusClient(settings)
 ```
+
 ## Redis
 
 ```python
 from verusdb.settings import Settings
 from verusdb.client import VerusClient
 from verusdb.embeddings.openai import OpenAIEmbeddingsEngine
 
@@ -97,18 +89,47 @@
     redis = {
                 'host': 'localhost',
                 'port': 6379,
                 'db': 0,
                 'password': None,
                 'prefix': 'doc:',
                 'index': 'verusdb'
-    },     
+    },
+    embeddings=OpenAIEmbeddingsEngine(key='my-openai-api-key')
+)
+client = VerusClient(settings)
+```
+
+## PostgreSQL
+
+```python
+from verusdb.settings import Settings
+from verusdb.client import VerusClient
+from verusdb.embeddings.openai import OpenAIEmbeddingsEngine
+
+# Create a new VerusDB client with custom settings
+settings = Settings(
+    engine='redis',
+    postgres = {
+                "host": "localhost",
+                "port": 5432,
+                "db": "verus",
+                "username": "verus",
+                "password": "verus",
+                "table": "verusdb"
+    },
     embeddings=OpenAIEmbeddingsEngine(key='my-openai-api-key')
 )
+
+
 client = VerusClient(settings)
+
+
 ```
 
 # Contributing
+
 If you find a bug or have a feature request, please open an issue on the [GitHub repository](https://github.com/verusdb/verusdb). Pull requests are also welcome!
 
 # License
-VerusDB is licensed under the [MIT License](https://opensource.org/licenses/MIT).
+
+VerusDB is licensed under the [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `verusdb-0.0.0/pyproject.toml` & `verusdb-0.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "verusdb"
-version = "0.0.0"
+version = "0.0.1"
 description = ""
 authors = ["Roger Naranjo <rogernaranjo@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 polars = "^0.18.2"
 numpy = "^1.24.3"
 openai = "^0.27.8"
 redis = "^4.5.5"
+psycopg2 = "^2.9.6"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.2"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `verusdb-0.0.0/verusdb/client.py` & `verusdb-0.0.1/verusdb/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 from __future__ import annotations
-import polars as pl
 from verusdb.settings import Settings
-import numpy as np
 from verusdb.engines.polars import PolarsEngine
 from verusdb.engines.redis import RedisEngine
+from verusdb.engines.postgresql import PostgreSQLEngine
 
 
 class VerusClient:
 
     def __init__(self, settings: Settings):
         self.settings = settings
         self.collection = 'verusdb'
         
         if self.settings.engine == 'redis':
             self.engine = RedisEngine(settings)
             
         if self.settings.engine == 'polars':
             self.engine = PolarsEngine(settings)
             
+        if self.settings.engine == 'postgres':
+            self.engine = PostgreSQLEngine(settings)
+            
             
         self.engine.load()
         
-        
-    def get_store(self):
-        return self.engine.store
+
     
     def get_engine(self):
         return self.engine
         
 
     def add(self, texts: list[str],  collection: str | None = None, embeddings: list[list[float]] | None = None, metadata: list[dict[str, str]] | None = None):
         """
         Add a document to the dataframe
         """
         if collection is None:
             collection = self.collection
             
-        self.engine.add(texts, collection, embeddings, metadata)
+        self.engine.add(texts=texts, collection=collection, embeddings=embeddings, metadata=metadata)
 
     def search(self, text: str| None = None, collection:str | None =  None, embedding: list[float] | None = None, filters: dict[str, str] | None = None, top_k: int = 10):
         """
         Search for similar documents
         """
         
         if text is None and embedding is None:
@@ -56,20 +56,34 @@
             raise ValueError('Embedding must be provided for the search')        
     
         return self.engine.search(embedding, collection, filters, top_k)
     
     def clear(self):
         self.engine.clear()
     
+    def update(self, uuid: str, metadata: dict[str, str]):
+        return self.engine.update(uuid, metadata)
+        
+
+    def get_documents(self, collection: str | None = None):
+        if collection is None:
+            collection = self.collection
+        return self.engine.get_documents(collection=collection)
+    
+    def get_document(self, uuid: str):
+        return self.engine.get_document(uuid)
 
     def save(self):
         """
         Save the dataframe to disk
         """
-        self.engine.save()
+        if self.settings.engine == 'polars':
+            self.engine.save()
+        else:
+            raise NotImplementedError('Save is not implemented for this engine')
 
-    def delete(self, filters: dict[str, str]):
+    def delete(self, uuid: str| None = None, collection: str | None = None ,filters: dict[str, str]| None = None):
         """
         Delete documents from the dataframe
         """
-        self.engine.delete(filters)
+        self.engine.delete(uuid=uuid, collection=collection, filters=filters)
```

### Comparing `verusdb-0.0.0/verusdb/embeddings/openai.py` & `verusdb-0.0.1/verusdb/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `verusdb-0.0.0/verusdb/engines/__init__.py` & `verusdb-0.0.1/verusdb/engines/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,12 +16,8 @@
     def load(self):
         pass
     
     @abstractmethod
     def search(self, collection, query, filters, num_results=10) -> list[dict[str, str]]:
         pass
 
-    @abstractmethod
-    def save(self, path) -> bool:
-        pass
-
```

### Comparing `verusdb-0.0.0/verusdb/engines/polars.py` & `verusdb-0.0.1/verusdb/engines/polars.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,194 +1,254 @@
 from __future__ import annotations
+import os
 import numpy as np
 import polars as pl
 from verusdb.engines import BaseEngine
 from verusdb.settings import Settings
-import os
+from verusdb.utils import generate_uuid
 
 
 class PolarsEngine(BaseEngine):
     """
     PolarsEngine class
 
     """
 
     def __init__(self, settings: Settings):
         """
         Create a new PolarsEngine instance
         """
         self.store = pl.DataFrame()
         self.settings = settings
-        self.embeddings_engine = settings.embeddings 
+        self.embeddings_engine = settings.embeddings
 
-        
     def __get_blank_store(self):
         """
         Get a blank dataframe
         """
-        return pl.DataFrame(schema=
-            [
-                ('collection', pl.Utf8),
-                ('text', pl.Utf8),
-                ('embeddings', pl.List(pl.Float64)),
+        return pl.DataFrame(
+            schema=[
+                ("uuid", str),
+                ("collection", pl.Utf8),
+                ("text", pl.Utf8),
+                ("embeddings", pl.List(pl.Float64)),
             ]
         )
 
     def load(self):
         """
         Load the dataframe from disk
         """
         if not self.settings.persist:
             self.store = self.__get_blank_store()
             return
-        
-        if self.settings.folder and os.path.exists(self.settings.folder+'/verusdb.parquet'):
-            self.store = pl.read_parquet(self.settings.folder+'/verusdb.parquet')
+
+        if self.settings.folder and os.path.exists(
+            self.settings.folder + "/verusdb.parquet"
+        ):
+            self.store = pl.read_parquet(self.settings.folder + "/verusdb.parquet")
         else:
             self.store = self.__get_blank_store()
 
-            
     def clear(self):
         self.store = self.__get_blank_store()
-        
-
-        
-
 
-    def add(self, texts: list[str],  collection: str | None = None, embeddings: list[list[float]] | None = None, metadata: list[dict[str, str]] | None = None):
+    def add(
+        self,
+        texts: list[str],
+        collection: str | None = None,
+        embeddings: list[list[float]] | None = None,
+        metadata: list[dict[str, str]] | None = None,
+    ):
         """
         Add a document to the dataframe
         """
         metadata_df = pl.DataFrame(metadata)
-        
+
         if embeddings is None:
-            
             if self.embeddings_engine is None:
-                raise ValueError('Embeddings engine not set')
-            
+                raise ValueError("Embeddings engine not set")
+
             embeddings = [self.embeddings_engine.encode(text) for text in texts]
-            
 
         data = {
-            'collection': collection,
-            'text': texts,
-            'embeddings': embeddings,
+            "uuid": generate_uuid(dimension=len(texts)),
+            "collection": collection,
+            "text": texts,
+            "embeddings": embeddings,
         }
 
-        #add the metadata to the dataframe
+        # Add the metadata to the dataframe
         for key in metadata_df.columns:
-            data['metadata__'+key] = metadata_df[key]
+            data["metadata__" + key] = metadata_df[key]
 
-        # add the columns starting with metadata__ from store to the data dict
+        # Add the columns starting with metadata__ from store to the data dict
         for key in self.store.columns:
-            if key.startswith('metadata__') and key not in data.keys():
-                data[key] = ''
-
+            if key.startswith("metadata__") and key not in data.keys():
+                data[key] = ""
 
-        # add to self.store the new columns with '' as the value
+        # Add to self.store the new columns with '' as the value
         self.store = self.store.with_columns(
-            (pl.lit('')).alias('metadata__'+key) for key in metadata_df.columns
+            (pl.lit("")).alias("metadata__" + key) for key in metadata_df.columns
         )
 
-        # add the new dataframe to the existing dataframe
+        # Add the new dataframe to the existing dataframe
         self.store = self.store.vstack(pl.DataFrame(data))
 
-    def delete(self, filters: dict[str, str] | None = None):
+    def delete(self, uuid: str | None = None, collection: str | None = None, filters: dict[str, str] | None = None):
         """
         Delete documents from the store
         """
-        if filters is None:
-            self.store = pl.DataFrame(schema=
-            [
-                ('collection', pl.Utf8),
-                ('text', pl.Utf8),
-                ('embeddings', pl.List(pl.Float64)),
-            ])
-        else:
-            for key, value in filters.items():
-                self.store = self.store.filter(pl.col(f'metadata__{key}') != value)
+        if uuid is None and filters is None and collection is None:
+            ValueError("uuid, collection or filters must be provided")
+            
+        if collection is not None:
+            self.store = self.store.filter(pl.col("collection") != collection)
 
+        if uuid is not None:
+            self.store = self.store.filter(pl.col("uuid") != uuid)
 
-    def _cosine_similarity(self, embedding: list[float], collection: str | None = None,  filters: dict[str, str] | None = None) -> pl.DataFrame:
+        if filters is not None:
+            for key, value in filters.items():
+                self.store = self.store.filter(pl.col(f"metadata__{key}") != value)
 
-        #expand the metadata column
+    def _cosine_similarity(
+        self,
+        embedding: list[float],
+        collection: str | None = None,
+        filters: dict[str, str] | None = None,
+    ) -> pl.DataFrame:
+        """
+        Calculate the cosine similarity
+        """
         temp = self.store
 
         if collection is not None:
-            temp = temp.filter(pl.col('collection') == collection)
+            temp = temp.filter(pl.col("collection") == collection)
 
-        #filter the dataframe
+        # filter the dataframe
         if filters is not None:
             for key, value in filters.items():
-                temp = temp.filter(pl.col('metadata__'+key) == value)
+                temp = temp.filter(pl.col("metadata__" + key) == value)
 
-        norm =  np.linalg.norm(embedding)
+        norm = np.linalg.norm(embedding)
 
         if norm == 0:
-            raise ValueError('The embedding cannot be a zero vector')
-        
+            raise ValueError("The embedding cannot be a zero vector")
+
         # Calculate the cosine similarity
         # TODO: This is not the most efficient way to do this, there is a pylint warning
         temp = temp.with_columns(
-            pl.col('embeddings').apply(lambda x: (x.dot(embedding))/ (norm * np.linalg.norm(x))).alias('score') # type: ignore
+            pl.col("embeddings").apply(lambda x: (x.dot(embedding)) / (norm * np.linalg.norm(x))).alias("score")  # type: ignore
         )
-        
-        # Return the dataframe sorted by cosine similarity
-        return temp.sort('score', descending=True)
 
-    
+        # Return the dataframe sorted by cosine similarity
+        return temp.sort("score", descending=True)
 
-    def search(self,  embedding: list[float], collection: str | None = None, filters: dict[str, str] | None = None, top_k: int = 10) -> list[dict[str, str]]:
+    def search(
+        self,
+        embedding: list[float],
+        collection: str | None = None,
+        filters: dict[str, str] | None = None,
+        top_k: int = 10,
+    ) -> list[dict[str, str]]:
         """
         Search the dataframe
         """
-        
+
         # Calculate the cosine similarity
-        results = self._cosine_similarity(embedding, collection, filters).drop('embeddings')
+        results = self._cosine_similarity(embedding, collection, filters).drop(
+            "embeddings"
+        )
 
         # Return the top k results
-        return self._serialize(results.head(top_k))
-    
+        return self._serialize(results.head(top_k), include_score=True)
 
-    def search_text(self, text: str, collection: str | None = None,  filters: dict[str, str] | None = None, top_k: int = 10, return_object: bool = False):
+    def search_text(
+        self,
+        text: str,
+        collection: str | None = None,
+        filters: dict[str, str] | None = None,
+        top_k: int = 10,
+        return_object: bool = False,
+    ):
         """
         Search the dataframe
         """
-        # calulate the embedding
-        
+
         if self.embeddings_engine is None:
-            raise ValueError('Embeddings Engine is not set')
-        
-        embedding : list[float] = self.embeddings_engine.encode(text)
+            raise ValueError("Embeddings Engine is not set")
+
+        # calulate the embedding
+        embedding: list[float] = self.embeddings_engine.encode(text)
 
-        #perform the search
-        results = self._cosine_similarity(embedding=embedding, collection=collection,  filters=filters).drop('embeddings')
+        # perform the search
+        results = self._cosine_similarity(
+            embedding=embedding, collection=collection, filters=filters
+        ).drop("embeddings")
 
         # Return the top k results
         if return_object:
             return results.head(top_k)
-        
-        return self._serialize(results.head(top_k))
 
-    def _serialize(self, documents: pl.DataFrame) -> list[dict[str, str]]:
+        return self._serialize(results.head(top_k), include_score=True)
+
+    def _serialize(
+        self, documents: pl.DataFrame, include_score: bool = False
+    ) -> list[dict[str, str]]:
+        if not include_score and "score" in documents.columns:
+            documents = documents.drop("score")
+
         serialized_data = documents.to_dicts()
-        
+
         for data in serialized_data:
             metadata = {}
             keys_to_remove = []
             for key, value in data.items():
-                if key.startswith('metadata__'):
+                if key.startswith("metadata__"):
                     metadata[key.split("__")[1]] = value
                     keys_to_remove.append(key)
             for key in keys_to_remove:
                 data.pop(key)
-            data['metadata'] = metadata
-                    
+            data["metadata"] = metadata
+
         return serialized_data
-    
+
+    def get_documents(self, collection: str | None = None):
+        if collection is None:
+            return self._serialize(self.store)
+
+        return self._serialize(self.store.filter(pl.col("collection") == collection))
+
+    def get_document(self, uuid: str):
+        document = self._serialize(
+            self.store.filter(pl.col("uuid") == uuid).drop("embeddings")
+        )
+        return document[0] if len(document) > 0 else None
+
+    def update(self, uuid: str, metadata: dict[str, str]):
+        """
+        Update the metadata of a document
+        """
+
+        removed_uuid = self.store.filter(pl.col("uuid") != uuid)
+        uuid_df = self.store.filter(pl.col("uuid") == uuid)
+
+        # replace all metadata columns with empty strings from the uuid_df
+        for key in uuid_df.columns:
+            if key.startswith("metadata__"):
+                uuid_df = uuid_df.with_columns(pl.lit("").alias(key))
+
+        # add the metadata to the uuid_df
+        for key, value in metadata.items():
+            uuid_df = uuid_df.with_columns(pl.lit(value).alias("metadata__" + key))
+
+        # combine the two dataframes
+        self.store = removed_uuid.vstack(uuid_df)
+
+        return self.get_document(uuid)
+
     def save(self):
         """
         Save the dataframe
         """
         self.store.write_parquet(self.settings.file)
-
-
```

### Comparing `verusdb-0.0.0/verusdb/engines/redis.py` & `verusdb-0.0.1/verusdb/engines/redis.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 import redis
 import numpy as np
 from redis.commands.search.field import TagField, VectorField, NumericField, TextField
 from redis.commands.search.indexDefinition import IndexDefinition, IndexType
 from redis.commands.search.query import Query
 from verusdb.engines import BaseEngine
 from verusdb.settings import Settings
+from verusdb.utils import generate_uuid
 
 class RedisEngine(BaseEngine):
     """
-    PolarsEngine class
+    Regis endigne class
 
     """
 
     def __init__(self, settings: Settings):
         """
-        Create a new PolarsEngine instance
+        Create a new Redis Engine instance
         """
         self.settings = settings
         self.embeddings_engine = settings.embeddings
         self.redis_host = settings.redis_host
         self.redis_port = settings.redis_port
         self.redis_db = settings.redis_db
         self.redis_index = settings.redis_index
@@ -37,14 +38,15 @@
         try:
             # check to see if index exists
             self.store.ft(self.redis_index).info()
 
         except:
             # schema
             schema = (
+                TextField("uuid"),                     # UUID Field Name
                 TextField("collection"),                # Tag Field Name
                 TextField("text"),                     # Text Field Name
                 TagField("metadata"),                # Tag Field Name
                 VectorField("embeddings",               # Vector Field Name
                     "HNSW", {                          # Vector Index Type: FLAT or HNSW
                         "TYPE": "FLOAT32",             # FLOAT32 or FLOAT64
                         "DIM": self.dimensions,        # Number of Vector Dimensions
@@ -71,63 +73,99 @@
         
              
         if embeddings is None:
             embeddings = [self.embeddings_engine.encode(text) for text in texts] # type: ignore
         
         if metadata is None:
             metadata = [{}] * len(texts)
-
+            
+        uuids = generate_uuid(len(texts))
         
-        for text, embedding, meta in zip(texts, embeddings, metadata):
+        for uuid, text, embedding, meta in zip(uuids, texts, embeddings, metadata):
             data.append({
+                'uuid': uuid,
                 'collection': collection,
                 'text': text,
                 'embeddings': np.array(embedding).astype(np.float32).tobytes(),
                 'metadata': ','.join([f'{key}:{value}' for key, value in meta.items()])
             })
 
         # expand the metadata and add it to the data
      
         
         # add the data to the redis index
         pipe = self.store.pipeline()
         
         for i, item in enumerate(data):
-            
-            pipe.hset(f"doc:{i}", mapping=item)
+            uuid = item['uuid']
+            pipe.hset(f"{self.redis_doc_prefix}:{uuid}", mapping=item)
         
 
         pipe.execute()
             
             
         
     def clear(self):
         self.store.flushdb()            
+   
+    def get_documents(self, collection : str | None = None):
+        """
+        Get all documents from the index
+        """
+        query_string = f"@collection:{collection}"
+        query = (Query(f"({query_string})"))
         
-
+        
+        results = self.store.ft(self.redis_index).search(query)
+        print(query_string, self.redis_index,results.docs)
+        
+        return self._serialize(results.docs)
+             
+    def get_document(self, uuid: str):
+        
+        return self._serialize(self.store.hgetall(f"{self.redis_doc_prefix}:{uuid}"))
       
 
-    def delete(self, filters: dict[str, str] | None = None):
+    def delete(self, uuid: str | None = None,  collection: str | None = None, filters: dict[str, str] | None = None):
         """
         Delete documents from the index based on filters
         """
+        if collection is None and filters is None and uuid is None:
+            ValueError("Must provide either a collection, filters or uuid")
+                   
+        if uuid:
+            self.store.delete(f"{self.redis_doc_prefix}:{uuid}")
+            return True   
+            
         
-        
-        pass
+                       
+        query_string = f"@collection:{collection}"
 
+        
+        if filters:
+            for key, value in filters.items():
+                query_string += f" @metadata:{key}:{value}"
+                
+        query = (Query(f"({query_string})=>[DEL]"))
+        
+        self.store.ft(self.redis_index).search(query)
+        
+        return True
+        
+        
     
 
     def search(self,  embedding: list[float], collection: str | None = None, filters: dict[str, str] | None = None, top_k: int = 10, return_objects: bool = False):
         
         # build the query
         query_string = f"@collection:{collection}"
         # query_string = '*'
         
         
-        return_fields = ['collection', 'text', 'metadata', 'score']
+        return_fields = ['uuid','collection', 'text', 'metadata', 'score']
         
         if filters:
             for key, value in filters.items():
                 query_string += f" @metadata:{key}:{value}"
         
             
         # create the query for the embedding, filters and collection
@@ -169,30 +207,36 @@
         if return_object:
             return results
         
         return self._serialize(results.docs) # type: ignore
         
         # Return the top k results
 
-    def _serialize(self, documents) -> list[dict[str,str] | dict[str,dict[str,str]]]:
+    def _serialize(self, documents, include_score : bool = False) -> list[dict[str,str] | dict[str,dict[str,str]]]:
         """
         Serialize the redis output, merging the metadata
         
         """
         
         data: list[dict[str,str] | dict[str,dict[str,str]]] = []
-        
+
         for doc in documents:
             
-            data.append({
+            
+            data_dict = {
+                'uuid': doc['uuid'],
                 'collection': doc['collection'],
                 'text': doc['text'],
                 'metadata': {key: value for key, value in [item.split(':') for item in doc['metadata'].split(',')]} if doc['metadata'] else {},
-                'score': doc['score']
-            })
+            }
+            
+            if include_score:
+                data_dict['score'] = doc['score']
+                
+            data.append(data_dict)
             
             
         return data
```

### Comparing `verusdb-0.0.0/PKG-INFO` & `verusdb-0.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 Metadata-Version: 2.1
 Name: verusdb
-Version: 0.0.0
+Version: 0.0.1
 Summary: 
 Author: Roger Naranjo
 Author-email: rogernaranjo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: polars (>=0.18.2,<0.19.0)
+Requires-Dist: psycopg2 (>=2.9.6,<3.0.0)
 Requires-Dist: redis (>=4.5.5,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Verus
 
 Verus is a powerful, lightweight and flexible vector store that is designed to work seamlessly with multiple databases. It is built with LLM in mind, making it an ideal choice for natural language processing, information retrieval, and recommendation systems.
 
 One of the key benefits of Verus is its agnostic design, which allows it to integrate with a wide range of databases. This means that you can use Verus with your existing database infrastructure, without having to worry about compatibility issues.
 
-## TODOs
-- [ ] Redis Integration
-- [ ] PostgreSQL Integration
-- [ ] DuckDB Integration
-- [ ] CosmosDB Intergration
-- [ ] Benchmarking
-
-
 ## Installation
 
 You can install VerusDB using pip:
 
 `pip install verusdb`
 
 ## Usage
@@ -55,41 +48,40 @@
 
 # Search for documents
 response = client.search(text='what is my first document?')
 ```
 
 This will output a list of documents that match the search query, along with their metadata and a cosine similarity score. You can adjust the the number of results you obtain by relevance
 
-
 ```json
 [
   {
     "collection": "MyCollection",
     "text": "This is my first document",
     "metadata": {
       "source": "input",
-      "pages": "5"}
-    ,
+      "pages": "5"
+    },
     "score": 0.937450967393278
   },
   {
     "collection": "MyCollection",
     "text": "This is my second document",
     "metadata": {
       "source": "input",
-      "pages": "5"}
-    ,
+      "pages": "5"
+    },
     "score": 0.8927016698439493
   }
 ]
 ```
 
 # Configuration
 
-You can configure VerusDB by passing a Settings object to the VerusClient constructor. The Settings object allows you to specify the folder where the database files will be stored, the storage engine to use (currently Polars and Redis are supported), 
+You can configure VerusDB by passing a Settings object to the VerusClient constructor. The Settings object allows you to specify the folder where the database files will be stored, the storage engine to use (currently Polars and Redis are supported),
 
 ## Polars
 
 ```python
 from verusdb.settings import Settings
 from verusdb.client import VerusClient
 from verusdb.embeddings.openai import OpenAIEmbeddingsEngine
@@ -98,14 +90,15 @@
 settings = Settings(
     folder='data',
     engine='polars',
     embeddings=OpenAIEmbeddingsEngine(key='my-openai-api-key')
 )
 client = VerusClient(settings)
 ```
+
 ## Redis
 
 ```python
 from verusdb.settings import Settings
 from verusdb.client import VerusClient
 from verusdb.embeddings.openai import OpenAIEmbeddingsEngine
 
@@ -115,18 +108,48 @@
     redis = {
                 'host': 'localhost',
                 'port': 6379,
                 'db': 0,
                 'password': None,
                 'prefix': 'doc:',
                 'index': 'verusdb'
-    },     
+    },
     embeddings=OpenAIEmbeddingsEngine(key='my-openai-api-key')
 )
 client = VerusClient(settings)
 ```
 
+## PostgreSQL
+
+```python
+from verusdb.settings import Settings
+from verusdb.client import VerusClient
+from verusdb.embeddings.openai import OpenAIEmbeddingsEngine
+
+# Create a new VerusDB client with custom settings
+settings = Settings(
+    engine='redis',
+    postgres = {
+                "host": "localhost",
+                "port": 5432,
+                "db": "verus",
+                "username": "verus",
+                "password": "verus",
+                "table": "verusdb"
+    },
+    embeddings=OpenAIEmbeddingsEngine(key='my-openai-api-key')
+)
+
+
+client = VerusClient(settings)
+
+
+```
+
 # Contributing
+
 If you find a bug or have a feature request, please open an issue on the [GitHub repository](https://github.com/verusdb/verusdb). Pull requests are also welcome!
 
 # License
+
 VerusDB is licensed under the [MIT License](https://opensource.org/licenses/MIT).
+
```

