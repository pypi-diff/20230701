# Comparing `tmp/findlike-1.3.0.tar.gz` & `tmp/findlike-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findlike-1.3.0.tar", last modified: Thu Jun 29 15:13:17 2023, max compression
+gzip compressed data, was "findlike-1.3.1.tar", last modified: Sat Jul  1 01:05:21 2023, max compression
```

## Comparing `findlike-1.3.0.tar` & `findlike-1.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-06-29 15:13:17.277779 findlike-1.3.0/
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1067 2023-06-27 14:06:31.000000 findlike-1.3.0/LICENSE
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     7877 2023-06-29 15:13:17.274445 findlike-1.3.0/PKG-INFO
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     7252 2023-06-29 15:08:05.000000 findlike-1.3.0/README.md
-drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-06-29 15:13:17.274445 findlike-1.3.0/findlike/
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)        0 2022-12-31 23:26:30.000000 findlike-1.3.0/findlike/__init__.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)       59 2023-06-23 20:53:39.000000 findlike-1.3.0/findlike/__main__.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     5049 2023-06-29 14:33:51.000000 findlike-1.3.0/findlike/cli.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     3300 2023-06-29 14:20:03.000000 findlike-1.3.0/findlike/constants.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     4330 2023-06-28 17:12:04.000000 findlike-1.3.0/findlike/format.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     3234 2023-06-28 17:48:12.000000 findlike-1.3.0/findlike/preprocessing.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1218 2023-06-29 14:30:47.000000 findlike-1.3.0/findlike/utils.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1706 2023-06-28 17:51:37.000000 findlike-1.3.0/findlike/wrappers.py
-drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-06-29 15:13:17.274445 findlike-1.3.0/findlike.egg-info/
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     7877 2023-06-29 15:13:17.000000 findlike-1.3.0/findlike.egg-info/PKG-INFO
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)      474 2023-06-29 15:13:17.000000 findlike-1.3.0/findlike.egg-info/SOURCES.txt
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)        1 2023-06-29 15:13:17.000000 findlike-1.3.0/findlike.egg-info/dependency_links.txt
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)       46 2023-06-29 15:13:17.000000 findlike-1.3.0/findlike.egg-info/entry_points.txt
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)      186 2023-06-29 15:13:17.000000 findlike-1.3.0/findlike.egg-info/requires.txt
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)        9 2023-06-29 15:13:17.000000 findlike-1.3.0/findlike.egg-info/top_level.txt
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1095 2023-06-29 15:11:29.000000 findlike-1.3.0/pyproject.toml
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)       38 2023-06-29 15:13:17.277779 findlike-1.3.0/setup.cfg
-drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-06-29 15:13:17.274445 findlike-1.3.0/tests/
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     8276 2023-06-28 14:38:17.000000 findlike-1.3.0/tests/test_cli.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1898 2023-06-28 13:14:54.000000 findlike-1.3.0/tests/test_corpus.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     2937 2023-06-27 19:22:45.000000 findlike-1.3.0/tests/test_format.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1967 2023-06-28 17:48:50.000000 findlike-1.3.0/tests/test_processor.py
+drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-07-01 01:05:21.616878 findlike-1.3.1/
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1067 2023-06-27 14:06:31.000000 findlike-1.3.1/LICENSE
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)    11535 2023-07-01 01:05:21.616878 findlike-1.3.1/PKG-INFO
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)    10911 2023-06-29 21:00:15.000000 findlike-1.3.1/README.md
+drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-07-01 01:05:21.616878 findlike-1.3.1/findlike/
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)        0 2022-12-31 23:26:30.000000 findlike-1.3.1/findlike/__init__.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)       59 2023-06-23 20:53:39.000000 findlike-1.3.1/findlike/__main__.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     5151 2023-07-01 00:35:57.000000 findlike-1.3.1/findlike/cli.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     3952 2023-07-01 00:02:10.000000 findlike-1.3.1/findlike/constants.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     4330 2023-06-28 17:12:04.000000 findlike-1.3.1/findlike/format.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     3586 2023-07-01 01:01:42.000000 findlike-1.3.1/findlike/preprocessing.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1211 2023-07-01 00:00:21.000000 findlike-1.3.1/findlike/utils.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     2111 2023-07-01 00:49:44.000000 findlike-1.3.1/findlike/wrappers.py
+drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-07-01 01:05:21.616878 findlike-1.3.1/findlike.egg-info/
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)    11535 2023-07-01 01:05:21.000000 findlike-1.3.1/findlike.egg-info/PKG-INFO
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)      474 2023-07-01 01:05:21.000000 findlike-1.3.1/findlike.egg-info/SOURCES.txt
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)        1 2023-07-01 01:05:21.000000 findlike-1.3.1/findlike.egg-info/dependency_links.txt
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)       46 2023-07-01 01:05:21.000000 findlike-1.3.1/findlike.egg-info/entry_points.txt
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)      186 2023-07-01 01:05:21.000000 findlike-1.3.1/findlike.egg-info/requires.txt
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)        9 2023-07-01 01:05:21.000000 findlike-1.3.1/findlike.egg-info/top_level.txt
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1095 2023-07-01 01:04:44.000000 findlike-1.3.1/pyproject.toml
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)       38 2023-07-01 01:05:21.616878 findlike-1.3.1/setup.cfg
+drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-07-01 01:05:21.616878 findlike-1.3.1/tests/
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     8759 2023-07-01 00:11:26.000000 findlike-1.3.1/tests/test_cli.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1897 2023-07-01 00:24:14.000000 findlike-1.3.1/tests/test_corpus.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     2937 2023-06-27 19:22:45.000000 findlike-1.3.1/tests/test_format.py
+-rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1967 2023-06-28 17:48:50.000000 findlike-1.3.1/tests/test_processor.py
```

### Comparing `findlike-1.3.0/LICENSE` & `findlike-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `findlike-1.3.0/findlike/cli.py` & `findlike-1.3.1/findlike/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     help="directory to scan for similar files",
     required=False,
 )
 @click.option(
     "--filename-pattern",
     "-f",
     type=str,
-    default="*.*",
+    default=None,
     help="filename pattern matching",
     show_default="plain-text file extensions",
     required=False,
 )
 @click.option(
     "--recursive",
     "-R",
@@ -180,33 +180,33 @@
     else:
         raise click.UsageError(
             "Neither REFERENCE_FILE nor --query QUERY was provided."
         )
 
     # Put together the list of documents to be analyzed.
     directory_path = Path(directory)
+    extensions: list[str] = [filename_pattern] if filename_pattern else TEXT_FILE_EXT
     document_paths = collect_paths(
-        directory=directory_path, extensions=TEXT_FILE_EXT, recursive=recursive
+        directory=directory_path, extensions=extensions, recursive=recursive
     )
 
     # Create a corpus with the collected documents.
     corpus = Corpus(paths=document_paths, min_chars=min_chars)
+    corpus.add_document(document=reference_content)
 
     # Set up the documents pre-processor.
     stemmer = SnowballStemmer(language).stem
     processor = Processor(
         stopwords=get_stop_words(language=language),
         stemmer=stemmer,
     )
-
+    
     # Set up the similarity model.
     model = ALGORITHM_CLASSES[algorithm](processor=processor)
-    model.fit(
-        corpus.documents_ + [reference_content]
-    )  # Add reference to avoid zero division
+    model.fit(corpus.documents_)  # Add reference to avoid zero division
     scores = model.get_scores(source=reference_content)
 
     # Format and print results.
     formatter = FORMATTER_CLASSES[format](
         targets=corpus.paths_,
         scores=scores,
         max_results=max_results,
```

### Comparing `findlike-1.3.0/findlike/format.py` & `findlike-1.3.1/findlike/format.py`

 * *Files identical despite different names*

### Comparing `findlike-1.3.0/findlike/preprocessing.py` & `findlike-1.3.1/findlike/preprocessing.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,16 +41,16 @@
         return text
 
     def tokenizer(self, text: str) -> list[str]:
         """Run the tokenization and post-processing.
         This method should be called by the similarity algorithms.
         """
         tokens = self._tokenize(text)
-        tokens = self._stemmize(tokens)
-        return tokens
+        stemmized_tokens = self._stemmize(tokens)
+        return stemmized_tokens
 
     def _tokenize(self, text: str) -> list[str]:
         """Preprocess a text and returns a list of tokens.
         This method should be called by the similarity algorithms.
         """
         words = WORD_RE.findall(text)
         return words
@@ -88,14 +88,26 @@
 
         self._load_documents()
         if min_chars:
             self._apply_min_chars_filter()
         self._prune_documents()
         self._prune_paths()
 
+    def add_document(self, document: str|None):
+        """Add a document to the current corpus.
+
+        Args:
+            document (str): Document to be added.
+
+        Returns:
+            list[str]: The new corpus after the document has been added.
+        """
+        if document:
+            self.documents_.append(document)
+
     def _load_documents(self):
         self._loaded_documents = [try_read_file(p) for p in self.paths]
 
     def _prune_paths(self):
         self.paths_ = compress(self.paths, self.documents_)
 
     def _prune_documents(self):
```

### Comparing `findlike-1.3.0/findlike/utils.py` & `findlike-1.3.1/findlike/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,11 +30,11 @@
             subdirectories as well. Defaults to False.
 
     Returns:
         list[Path]: A list of paths to the matching files.
     """
     glob_func = directory.rglob if recursive else directory.glob
     paths = [
-        x for ext in extensions for x in glob_func("*." + ext) if x.is_file()
+        x for ext in extensions for x in glob_func(ext) if x.is_file()
     ]
     return paths
```

### Comparing `findlike-1.3.0/pyproject.toml` & `findlike-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "findlike"
-version = "1.3.0"
+version = "1.3.1"
 authors = [{ name = "Bruno Arine", email = "bruno.arine@runbox.com" }]
 description = "findlike is a package to retrieve similar documents"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `findlike-1.3.0/tests/test_cli.py` & `findlike-1.3.1/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,23 +32,45 @@
 @pytest.fixture
 def create_directory(tmp_path):
     for i, candidate in enumerate(candidates):
         file = tmp_path / f"file_{i:02d}.txt"
         file.write_text(candidate)
     return str(tmp_path)
 
+
+@pytest.fixture
+def create_directory_with_non_text(tmp_path):
+    for i, candidate in enumerate(candidates):
+        file = tmp_path / f"file_{i:02d}.000"
+        file.write_text(candidate)
+    return str(tmp_path)
+
+
 @pytest.mark.parametrize("format", cli.FORMATTER_CLASSES.keys())
 def test_formats(runner, create_directory, format):
-    result = runner.invoke(cli.cli, ["-d", create_directory, "-F", format, *std_args])
+    result = runner.invoke(
+        cli.cli, ["-d", create_directory, "-F", format, *std_args]
+    )
     assert result.exit_code == 0
 
     json_data = json.loads(result.output.strip())
     assert len(json_data) == len(scores)
 
 
 @pytest.mark.parametrize("algorithm", cli.ALGORITHM_CLASSES.keys())
 def test_algorithms(runner, create_directory, algorithm):
-    result = runner.invoke(cli.cli, ["-d", create_directory, "-a", algorithm, *std_args])
+    result = runner.invoke(
+        cli.cli, ["-d", create_directory, "-a", algorithm, *std_args]
+    )
     json_data = json.loads(result.output.strip())
 
     output_scores = [float(x["score"]) for x in json_data]
     assert spearmanr(output_scores, scores)[0] > 0.99
+
+
+def test_other_extensions(runner, create_directory_with_non_text):
+    result = runner.invoke(
+        cli.cli,
+        ["-d", create_directory_with_non_text, "-f", "*.000", *std_args],
+    )
+    assert "000" in result.output.strip()
+
```

### Comparing `findlike-1.3.0/tests/test_corpus.py` & `findlike-1.3.1/tests/test_corpus.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,8 +66,7 @@
         try_read_file(invalid_path)
 
 
 def test_empty_paths_list():
     corpus = Corpus([], min_chars=0)
     assert len(corpus.documents_) == 0
     assert len(corpus.paths_) == 0
-
```

### Comparing `findlike-1.3.0/tests/test_format.py` & `findlike-1.3.1/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `findlike-1.3.0/tests/test_processor.py` & `findlike-1.3.1/tests/test_processor.py`

 * *Files identical despite different names*

