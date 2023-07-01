# Comparing `tmp/sashimi_domains-0.9.2.tar.gz` & `tmp/sashimi_domains-0.9.3.tar.gz`

## Comparing `sashimi_domains-0.9.2.tar` & `sashimi_domains-0.9.3.tar`

### file list

```diff
@@ -1,47 +1,50 @@
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/TODO
--rw-r--r--   0        0        0    26080 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/limbo/blockology.py
--rw-r--r--   0        0        0     4308 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/limbo/corporalogy.py
--rw-r--r--   0        0        0    15646 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/limbo/graphology.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/__init__.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/config.py
--rw-r--r--   0        0        0     9608 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/ioio.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/misc.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/naming.py
--rw-r--r--   0        0        0    18282 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/scorology.py
--rw-r--r--   0        0        0     9237 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/vectorology.py
--rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/w2v_score.py
--rw-r--r--   0        0        0    12895 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/blocks/__init__.py
--rw-r--r--   0        0        0    17181 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/blocks/annotations.py
--rw-r--r--   0        0        0     8885 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/blocks/area_rank_chart.py
--rw-r--r--   0        0        0    11261 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/blocks/block_ext_map.py
--rw-r--r--   0        0        0    44082 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/blocks/hierarchical_block_map.py
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/blocks/hierarchical_block_map_help.html
--rw-r--r--   0        0        0     8002 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/blocks/link_maps.py
--rw-r--r--   0        0        0    11432 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/blocks/network_map.py
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/blocks/util.py
--rw-r--r--   0        0        0     8939 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/blocks/zmethods.py
--rw-r--r--   0        0        0     8602 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/blocks/tables/__init__.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/blocks/tables/tables.css
--rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/blocks/tables/tables_html.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/blocks/tables/tables_plots.py
--rw-r--r--   0        0        0    37117 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/corpus/__init__.py
--rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/corpus/nlp.py
--rw-r--r--   0        0        0     8886 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/corpus/parsers.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/corpus/wos.py
--rw-r--r--   0        0        0    19814 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/graph_models/__init__.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/graph_models/domain_chained_model.py
--rw-r--r--   0        0        0     6588 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/graph_models/domain_topic_model.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/graph_models/util.py
--rwxr-xr-x   0        0        0     1746 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/util/asco_clean.py
--rwxr-xr-x   0        0        0      451 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/util/pubmed_clean.py
--rwxr-xr-x   0        0        0      612 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/util/pubmed_get.sh
--rwxr-xr-x   0        0        0     6667 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/util/scan_bugtrap.py
--rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/util/wos_lam/__init__.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/src/sashimi/util/wos_lam/wos_api_request.tpl
--rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/tests/test_basic_usage.py
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/tests/test_pclabel_bfield.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/.gitignore
--rw-r--r--   0        0        0    35061 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/LICENSE
--rw-r--r--   0        0        0     7445 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/README.md
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 sashimi_domains-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/TODO
+-rw-r--r--   0        0        0   441328 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/doc/domain topic map.png
+-rw-r--r--   0        0        0    26080 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/limbo/blockology.py
+-rw-r--r--   0        0        0     4308 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/limbo/corporalogy.py
+-rw-r--r--   0        0        0    15646 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/limbo/graphology.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/__init__.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/config.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/entropies.py
+-rw-r--r--   0        0        0     9758 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/ioio.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/misc.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/naming.py
+-rw-r--r--   0        0        0    18265 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/scorology.py
+-rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/vectorology.py
+-rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/w2v_score.py
+-rw-r--r--   0        0        0    16237 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/#annotations.py#
+-rw-r--r--   0        0        0    13901 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/__init__.py
+-rw-r--r--   0        0        0    16246 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/annotations.py
+-rw-r--r--   0        0        0     8885 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/area_rank_chart.py
+-rw-r--r--   0        0        0    11244 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/block_ext_map.py
+-rw-r--r--   0        0        0    44214 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/hierarchical_block_map.py
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/hierarchical_block_map_help.html
+-rw-r--r--   0        0        0     8002 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/link_maps.py
+-rw-r--r--   0        0        0    11670 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/network_map.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/util.py
+-rw-r--r--   0        0        0     8937 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/zmethods.py
+-rw-r--r--   0        0        0    10540 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/tables/__init__.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/tables/tables.css
+-rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/tables/tables_html.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/tables/tables_plots.py
+-rw-r--r--   0        0        0    37282 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/corpus/__init__.py
+-rw-r--r--   0        0        0     6200 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/corpus/nlp.py
+-rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/corpus/parsers.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/corpus/wos.py
+-rw-r--r--   0        0        0    20413 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/graph_models/__init__.py
+-rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/graph_models/domain_chained_model.py
+-rw-r--r--   0        0        0     6602 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/graph_models/domain_topic_model.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/graph_models/util.py
+-rwxr-xr-x   0        0        0     1746 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/util/asco_clean.py
+-rwxr-xr-x   0        0        0      451 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/util/pubmed_clean.py
+-rwxr-xr-x   0        0        0      612 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/util/pubmed_get.sh
+-rwxr-xr-x   0        0        0     6667 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/util/scan_bugtrap.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/util/wos_lam/__init__.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/util/wos_lam/wos_api_request.tpl
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/tests/test_basic_usage.py
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/tests/test_pclabel_bfield.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/.gitignore
+-rw-r--r--   0        0        0    35061 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/LICENSE
+-rw-r--r--   0        0        0     8175 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/README.md
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     9516 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/PKG-INFO
```

### Comparing `sashimi_domains-0.9.2/src/limbo/blockology.py` & `sashimi_domains-0.9.3/src/limbo/blockology.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.2/src/limbo/corporalogy.py` & `sashimi_domains-0.9.3/src/limbo/corporalogy.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.2/src/limbo/graphology.py` & `sashimi_domains-0.9.3/src/limbo/graphology.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.2/src/sashimi/__init__.py` & `sashimi_domains-0.9.3/src/sashimi/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding: utf-8
-
 # Sashimi - Study of the organisation and evolution of a corpus
 #
 # Author(s):
 # * Ale Abdo <abdo@member.fsf.org>
 #
 # License:
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
@@ -22,15 +20,15 @@
 """
 
 __author__ = "Alexandre Hannud Abdo <abdo@member.fsf.org>"
 __copyright__ = "Copyright 2016-2023 Alexandre Hannud Abdo"
 __license__ = "GNU GPL version 3 or above"
 __URL__ = "https://gitlab.com/solstag/sashimi/"
 
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 __all__ = ["Corpus", "GraphModels", "Vectorology"]
 
 import graph_tool  # to avoid import order issues with pandas # noqa
 
 #######################
 # Expose main classes #
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/config.py` & `sashimi_domains-0.9.3/src/sashimi/config.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.2/src/sashimi/ioio.py` & `sashimi_domains-0.9.3/src/sashimi/ioio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding: utf-8
-
 # Sashimi - Study of the organisation and evolution of a corpus
 #
 # Author(s):
 # * Ale Abdo <abdo@member.fsf.org>
 #
 # License:
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
@@ -185,35 +183,37 @@
 
         fopen = compressor.open if compressor else open
         fpath.parent.mkdir(parents=True, exist_ok=True)
         with fopen(fpath, mode) as f:
             formatter.dump(obj, f, **formatter_args)
 
     @classmethod
-    def load_pandas(cls, fpath, fmt=None, formatter_args={}):
+    def load_pandas(cls, fpath, fmt=None, formatter_args={}, doc_as_tuple=False):
         """
         Reads a pandas object from the disk, decompressing if needed.
 
         Parameters
         ----------
         fpath: string
             Path to load from.
         fmt: string
             One of 'pickle' or 'json'.
             If `None`, tries to guess from extension, defaulting to 'json'.
         formatter_args: dict
             Parameters passed to reading function.
+        doc_as_tuple: bool
+            If fmt="json", convert anything doc-like (list[list[str]]) to tuples.
 
         Returns
         -------
         A pandas object, usually a Series or Dataframe
         """
         fpath = Path(fpath)
         if not fpath.exists():
-            raise FileNotFoundError
+            raise FileNotFoundError(fpath)
         fmt, cmp = cls.get_format(fpath)
         compression = cls.compressors[cmp]["pandas_arg"]
         method = cls.formatters[fmt]["rmethod"]
         extra_args = cls.formatters[fmt]["r_extra_args"]
 
         # compression in `to_hdf` seems useless, we might have used lzma on top
         if fmt == "hdf5":
@@ -252,25 +252,24 @@
                         ),
                     )
                     break
                 except (lzma.LZMAError, gzip.BadGzipFile):
                     pass
 
         # json doesn't handle tuples, so we must find and convert our tokens
-        if fmt != "json":
-            return df
-        df = df.transform(
-            lambda x: x.map(lambda y: tuple(map(tuple, y)), na_action="ignore")
-            if all(
-                type(y) is list
-                and all(type(z) is list and all(type(w) is str for w in z) for z in y)
-                for y in x.loc[x.notna()]
+        if fmt == "json" and doc_as_tuple:
+            df = df.transform(
+                lambda x: x.map(lambda y: tuple(map(tuple, y)), na_action="ignore")
+                if all(
+                    type(y) is list
+                    and all(type(z) is list and all(type(w) is str for w in z) for z in y)
+                    for y in x.loc[x.notna()]
+                )
+                else x
             )
-            else x
-        )
         return df
 
     @classmethod
     def store_pandas(cls, obj, fpath, fmt=None, formatter_args={}):
         """
         Stores a pandas object to the disk.
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/misc.py` & `sashimi_domains-0.9.3/src/sashimi/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding: utf-8
-
 # Sashimi - Study of the organisation and evolution of a corpus
 #
 # Author(s):
 # * Ale Abdo <abdo@member.fsf.org>
 #
 # License:
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/naming.py` & `sashimi_domains-0.9.3/src/sashimi/naming.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding: utf-8
-
 # Sashimi - Study of the organisation and evolution of a corpus
 #
 # Author(s):
 # * Ale Abdo <abdo@member.fsf.org>
 #
 # License:
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/scorology.py` & `sashimi_domains-0.9.3/src/sashimi/scorology.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding: utf-8
-
 # Sashimi - Study of the organisation and evolution of a corpus
 #
 # Author(s):
 # * Ale Abdo <abdo@member.fsf.org>
 #
 # License:
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/vectorology.py` & `sashimi_domains-0.9.3/src/sashimi/vectorology.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding: utf-8
-
 # Corporalogister
 #
 # Author(s):
 # * Ale Abdo <abdo@member.fsf.org>
 #
 # License:
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/w2v_score.py` & `sashimi_domains-0.9.3/src/sashimi/w2v_score.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding: utf-8
-
 # Originally LGPL licensed code from gensim
 # See https://github.com/RaRe-Technologies/gensim
 
 from numpy import (
     exp,
     log,
     dot,
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/blocks/__init__.py` & `sashimi_domains-0.9.3/src/sashimi/blocks/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding: utf-8
-
 # Sashimi - Study of the organisation and evolution of a corpus
 #
 # Author(s):
 # * Ale Abdo <abdo@member.fsf.org>
 #
 # License:
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
@@ -16,15 +14,14 @@
 # <https://gitlab.com/solstag/abstractology>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 from collections import Counter
 from functools import cache
 
-import numpy as np
 import pandas as pd
 
 from ..corpus import Corpus
 from .hierarchical_block_map import composite_hierarchical_block_map
 from . import zmethods
 from .tables import subxblocks_report, xblocks_report
 from .network_map import network_map
@@ -123,14 +120,15 @@
         if hasattr(self, "dblocks"):
             if not hasattr(self, "_orig_dblocks"):
                 self._orig_dblocks = self.dblocks
             if keep:
                 self.dblocks = self.dblocks.loc[self.data.index]
             else:
                 self.dblocks = self._orig_dblocks.loc[self.data.index]
+            self.gen_mapindex()
 
     def find_blocks(self, lscape, finder):
         """
         Returns the blocks that correspond to features defined in finder.
         For example, blocks with the highest or lowest values, or with
         the highest or lowest differences in values across the landscape.
 
@@ -255,42 +253,68 @@
         """
         topic_terms = set(self.tblocks[self.tblocks[tlevel].eq(tblock)].index)
         return self.filter_terms(lambda term: term not in topic_terms, column)
 
     @cache
     def get_xelement_yelements(self, xbtype, ybtype):
         if (xbtype, ybtype) == ("doc", "ter"):
-            return self.get_doc_terms()
+            series = pd.Series(self.get_doc_terms(), index=self.dblocks.index)
         if (xbtype, ybtype) == ("doc", "ext"):
-            return self.get_doc_exts()
+            series = pd.Series(self.get_doc_exts(), index=self.dblocks.index)
         if (xbtype, ybtype) == ("ter", "doc"):
-            return pd.Series(self.ter_documents, index=self.tblocks.index).map(
-                lambda x: Counter() if x is np.nan else x
-            )
+            series = pd.Series(self.ter_documents, index=self.tblocks.index)
         if (xbtype, ybtype) == ("ext", "doc"):
-            return pd.Series(self.ext_documents, index=self.eblocks.index).map(
-                lambda x: Counter() if x is np.nan else x
-            )
+            series = pd.Series(self.ext_documents, index=self.eblocks.index)
+        return series.map(
+            lambda x: x
+            if isinstance(x, Counter)
+            else Counter()
+            if (isinstance(isna := pd.isna(x), bool) and isna)
+            else Counter(x)
+        )
 
-    @cache
-    def get_xblock_yblocks_counts(self, xbtype, xlevel, xb, ybtype, ylevel):
+    def get_xsel_yblocks_counts(self, xbtype, xsel, ybtype, ylevel):
         xelement_yelements = self.get_xelement_yelements(xbtype, ybtype)
         xblocks, _ = self.get_blocks_levels(xbtype)
         yblocks, _ = self.get_blocks_levels(ybtype)
-        sel = xb if xlevel is None else xblocks[xlevel].eq(xb)
         yelement2yblock = (lambda x: x) if ylevel is None else yblocks[ylevel].get
         xblock_yblocks_c = Counter()
-        if hasattr(xelement_yelements.iloc[0], "elements"):  # e.g. Counter()
-            for val in xelement_yelements.loc[sel]:
-                xblock_yblocks_c.update(yelement2yblock(el) for el in val.elements())
-        else:
-            for val in xelement_yelements.loc[sel]:
-                xblock_yblocks_c.update(yelement2yblock(el) for el in val)
+        for val in xelement_yelements.loc[xsel]:
+            xblock_yblocks_c.update(yelement2yblock(el) for el in val.elements())
         return xblock_yblocks_c
 
+    @cache
+    def get_xblock_yblocks_counts(self, xbtype, xlevel, xb, ybtype, ylevel):
+        xblocks, _ = self.get_blocks_levels(xbtype)
+        xsel = (xblocks.index == xb) if xlevel is None else xblocks[xlevel].eq(xb)
+        return self.get_xsel_yblocks_counts(xbtype, xsel, ybtype, ylevel)
+
+    def get_antixblock_sel(self, xbtype, xlevel, xb, antixlevel=None):
+        """
+        Selects the complement of a block `xb` of level `xlevel` and type `xbtype`.
+        (antixlevel): restrict selection to this parent (higher) xlevel
+        """
+        xblocks, _ = self.get_blocks_levels(xbtype)
+        xsel = (xblocks.index == xb) if xlevel is None else xblocks[xlevel].eq(xb)
+        xsel = ~xsel
+        if antixlevel is not None:
+            if antixlevel <= xlevel:
+                raise ValueError("`antixlevel` must be higher than `xlevel`")
+            antixlevel_xblock_containing_xb = xblocks.loc[~xsel, antixlevel].iloc[0]
+            antixsel = xblocks[antixlevel].eq(antixlevel_xblock_containing_xb)
+            xsel = xsel & antixsel
+        return xsel
+
+    @cache
+    def get_antixblock_yblocks_counts(
+            self, xbtype, xlevel, xb, antixlevel=None, ybtype="ter", ylevel=1,
+    ):
+        xsel = self.get_antixblock_sel(xbtype, xlevel, xb, antixlevel)
+        return self.get_xsel_yblocks_counts(xbtype, xsel, ybtype, ylevel)
+
     def get_xblock_yblocks_stat(
         self, stat, xbtype, xlevel, xb, ybtype, ylevel, ybs=None
     ):
         """
         Gets the `stat` = "count" or "frac_presence" of yblocks in xblocks.
         """
         ybs = None if ybs is None else set(ybs)
@@ -298,35 +322,33 @@
             raise ValueError(f"Unkown statistics: {stat}")
         xelements_yelements = self.get_xelement_yelements(xbtype, ybtype)
         xblocks, _ = self.get_blocks_levels(xbtype)
         yblocks, _ = self.get_blocks_levels(ybtype)
 
         # functions to abstract different cases
         yelement2yblock = (lambda x: x) if ylevel is None else yblocks[ylevel].get
-        yels_is_counter = hasattr(xelements_yelements.iloc[0], "elements")
-        yelements2yblocks = (
-            (lambda xel_yels: (yelement2yblock(el) for el in xel_yels.elements()))
-            if yels_is_counter
-            else (lambda xel_yels: (yelement2yblock(el) for el in xel_yels))
-        )
+
+        def yelements2yblocks(xel_yels):
+            return (yelement2yblock(el) for el in xel_yels.elements())
+
         yelements2yblocks4stat = (
             yelements2yblocks
             if (stat == "count")
             else (lambda xel_yels: set(yelements2yblocks(xel_yels)))
         )
-        any_func = len if stat == "count" else bool
+        any_cum_func = len if stat == "count" else bool
 
         # calculations
         xblock_yblocks_c = Counter()
         xblock_yblocks_any = 0
         sel = (xblocks.index == xb) if xlevel is None else xblocks[xlevel].eq(xb)
         for xel_yels in xelements_yelements.loc[sel]:
             yblocks4stat = [*yelements2yblocks4stat(xel_yels)]
             xblock_yblocks_c.update(yblocks4stat)
-            xblock_yblocks_any += any_func(
+            xblock_yblocks_any += any_cum_func(
                 [yb for yb in yblocks4stat if (ybs is None) or (yb in ybs)]
             )
 
         stat_s = pd.Series(xblock_yblocks_c).sort_values()
         stat_s.name = self.lblock_to_label[xlevel, xb]
         stat_s["any"] = xblock_yblocks_any
         stat_s = stat_s.div(sel.sum()) if stat == "frac_presence" else stat_s
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/blocks/annotations.py` & `sashimi_domains-0.9.3/src/sashimi/blocks/#annotations.py#`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding: utf-8
-
 # Sashimi - Study of the organisation and evolution of a corpus
 #
 # Author(s):
 # * Ale Abdo <abdo@member.fsf.org>
 #
 # License:
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
@@ -13,123 +11,55 @@
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
 # <https://gitlab.com/solstag/abstractology>
 #
 # Contributions are welcome, get in touch with the author(s).
 
-from heapq import nsmallest
+from heapq import nsmallest as heapq_nsmallest
 import html
 import random
 
-import numpy
-from numpy import mean
 import pandas
 from tqdm import tqdm
 
 from ..naming import naming
 from ..ioio import ioio
-
-#############
-# entropies #
-#############
-
-
-def pt_entropy(p, q=None):
-    """pointwise [relative] entropy"""
-    if q is None:
-        return -numpy.log2(p)
-    if q > 0 and p == 0:
-        return -numpy.inf
-    return numpy.log2(p / q)
-
-
-def ept_entropy(p, q=None, pe=None):
-    """expectation-weighted pointwise [relative] entropy"""
-    pe = p if pe is None else pe
-    return 0.0 if pe == 0 else pe * pt_entropy(p, q)
-
-
-def entropy(p, q=None, pe=None):
-    """total expectation-weighted [relative] entropy"""
-    pe = p if pe is None else pe
-    q = [None] * len(p) if q is None else q
-    return sum(ept_entropy(p, q, pe) for p, q, pe in zip(p, q, pe))
-
-
-def hier_pt_entropy(p, qs=None):
-    """mean of pointwise relative entropies"""
-    # qs = qs[:1] # TODO
-    return mean([pt_entropy(p, q) for q in qs])
-
-
-def hier_ept_entropy(p, qs=None, pe=None):
-    """expectation-weighted mean of pointwise relative entropies"""
-    pe = p if pe is None else pe
-    return 0.0 if pe == 0 else pe * hier_pt_entropy(p, qs)
-
-
-def make_subentropy(sub_counts, up_counts):
-    """nested commonality"""
-
-    def subentropy(x):
-        pe = mean([sc_tot and sc[x] / sc_tot for sc, sc_tot in sub_counts])
-        return mean(
-            [
-                hier_ept_entropy(
-                    sc_tot and sc[x] / sc_tot,
-                    [uc[x] / uc_tot for uc, uc_tot in up_counts] or [1 / len(sc)],
-                    pe=pe,
-                )
-                for sc, sc_tot in sub_counts
-            ]
-        )
-
-    return subentropy
+from ..entropies import make_nested_specificity, make_nested_commonality
 
 
 ##############################
 # xblock yblocks annotations #
 ##############################
 
 
-def get_xblock_yblocks(corpus, xbtype, xlevel, xb, ybtype, ylevel, n=None):
+def get_xblock_yblocks(
+    corpus, xbtype, xlevel, xb, ybtype, ylevel, num=None, anti=False
+):
     """
     Returns
     =======
     [(yblock, yblock_entropy), ...]
     """
-
-    def get_counts(hxb):
-        xlevel_, xb_ = corpus.hblock_to_level_block(hxb, xbtype)
-        xyc = corpus.get_xblock_yblocks_counts(xbtype, xlevel_, xb_, ybtype, ylevel)
-        return xyc, sum(xyc.values())
-
     hxb = corpus.level_block_to_hblock(xlevel, xb, xbtype)
-    ybc, ybct = get_counts(hxb)
-    upybcs = [get_counts(hxb[:i]) for i in range(1, len(hxb))]
+    get_counts = make_get_counts(corpus, xbtype, ybtype, ylevel)
+    ybcs = get_counts(hxb, anti=anti)
+    ybs = ybcs[-1][0] if anti else ybcs[0]
+    upybcs = [get_counts(hxb[:i]) for i in reversed(range(1, len(hxb)))]
 
-    def keyf(x):
-        """nested specificity (for topics)"""
-        return hier_ept_entropy(
-            ybc[x] / ybct,
-            [upybc[x] / upybct for upybc, upybct in upybcs] or [1 / len(ybc)],
-        )
+    nested_specificity = make_nested_specificity(ybcs, upybcs)
 
     def sortkeyf(x):
         return -x[1]
 
-    if n is None:
-        return sorted(((x, keyf(x)) for x in ybc), key=sortkeyf)
-    else:
-        return nsmallest(n, ((x, keyf(x)) for x in ybc), key=sortkeyf)
+    return nsmallest(num, ((x, nested_specificity(x)) for x in ybs), key=sortkeyf)
 
 
 def get_xblock_yblocks_elements(
-    corpus, xbtype, xlevel, xb, ybtype, ylevel, num=10, ent_frac=1 / 2
+    corpus, xbtype, xlevel, xb, ybtype, ylevel, num=10, ent_frac=0.5, anti=False
 ):
     """
     Given a domain block, returns a list containing, for each pertinent level 1 topic,
     a list of pertinent terms.
 
     After ordering topics by pointwise topic-level relative entropy, takes enough topics
     to account for half of the positive part of the topic-level relative entropy between
@@ -150,44 +80,37 @@
             ...
         ),
         'btypes': (xbtype, ybtype),
         'levels': (xlevel, ylevel),
     }
     """
     yblocks, _ = corpus.get_blocks_levels(ybtype)
-    xblock_yblocks = get_xblock_yblocks(corpus, xbtype, xlevel, xb, ybtype, ylevel)
-
-    def get_counts(hxb):
-        xlevel_, xb_ = corpus.hblock_to_level_block(hxb, xbtype)
-        xyc = corpus.get_xblock_yblocks_counts(xbtype, xlevel_, xb_, ybtype, None)
-        return xyc, sum(xyc.values())
+    xblock_yblocks = get_xblock_yblocks(
+        corpus, xbtype, xlevel, xb, ybtype, ylevel, anti=anti
+    )
 
+    get_counts = make_get_counts(corpus, xbtype, ybtype, None)
     hxb = corpus.level_block_to_hblock(xlevel, xb, xbtype)
-    yc, yct = get_counts(hxb)
-    upycs = [get_counts(hxb[:i]) for i in range(1, len(hxb))]
+    ycs = get_counts(hxb, anti=anti)
+    upycs = [get_counts(hxb[:i]) for i in reversed(range(1, len(hxb)))]
 
     yblocks_elements = {}
     for yb, yb_ent in yield_values_fraction(xblock_yblocks, ent_frac):
         yblocks_elements[yb] = {"ent": yb_ent, "elements": []}
     total_ent = sum(v for _, v in xblock_yblocks if v > 0)
     cum_ent = sum(x["ent"] for x in yblocks_elements.values())
 
     # TODO: we could consider the mutual information with previous terms and
     # skip the term if it's too high.
 
-    def keyf(x):
-        """nested specificity (for terms)"""
-        return hier_ept_entropy(
-            yc[x] / yct,
-            [upyc[x] / upyct for upyc, upyct in upycs] or [1 / len(yc)],
-        )
+    nested_specificity = make_nested_specificity(ycs, upycs)
 
     for yb, ybinfo in yblocks_elements.items():
         elements = yblocks[yblocks[ylevel].eq(yb)].index
-        elements = ((x, keyf(x)) for x in elements)
+        elements = ((x, nested_specificity(x)) for x in elements)
         elements = filter(lambda x: x[1] > 0, elements)
         elements = list(elements)
         ybinfo["ent_el"] = sum(x[1] for x in elements)
         elements = nsmallest(num, elements, key=lambda x: -x[1])
         if not elements:
             continue
         e_list = [elements.pop(0)]
@@ -216,15 +139,15 @@
 
 ###############################
 # xblocks yblocks annotations #
 ###############################
 
 
 def get_xblocks_yblocks(
-    corpus, xbtype, xlevelblocks, ybtype, ylevel, n=None, ent_frac=1 / 2
+    corpus, xbtype, xlevelblocks, ybtype, ylevel, n=None, ent_frac=0.5
 ):
     yblocks = {}
     for xlevel, xb in xlevelblocks:
         xblock_yblocks = get_xblock_yblocks(corpus, xbtype, xlevel, xb, ybtype, ylevel)
         for k, v in xblock_yblocks:
             yblocks[k] = yblocks.setdefault(k, 0.0) + v
     return list(yield_values_fraction(yblocks.items(), ent_frac))
@@ -235,15 +158,15 @@
         xblock_yblocks = get_xblock_yblocks(corpus, xbtype, xlevel, xb, ybtype, ylevel)
         for k, v in yield_values_fraction(xblock_yblocks, ent_frac):
             yblocks[k] = yblocks.setdefault(k, 0.0) + v
     return list(yblocks.items())
 
 
 def get_yblocks_xblocks(
-    corpus, xbtype, xlevel, ybtype, ylevel, ybs, n=None, ent_frac=1 / 2
+    corpus, xbtype, xlevel, ybtype, ylevel, ybs, n=None, ent_frac=0.5
 ):
     ybs = set(ybs)
     xblocks = []
 
     for xb in tqdm(corpus.get_blocks_levels(xbtype)[0][xlevel].unique()):
         xb_yblocks = get_xblock_yblocks(corpus, xbtype, xlevel, xb, ybtype, ylevel)
         for _, ent_low in yield_values_fraction(xb_yblocks, ent_frac):
@@ -255,20 +178,18 @@
 
 
 #################################
 # subxblock yblocks annotations #
 #################################
 
 
-def get_subxblocks_yblocks(corpus, xbtype, xlevel, xb, ybtype, ylevel, n=None):
-    def get_counts(hxb):
-        xlevel_, xb_ = corpus.hblock_to_level_block(hxb, xbtype)
-        xyc = corpus.get_xblock_yblocks_counts(xbtype, xlevel_, xb_, ybtype, ylevel)
-        return xyc, sum(xyc.values())
-
+def get_subxblocks_yblocks(
+    corpus, xbtype, xlevel, xb, ybtype, ylevel, num=None, anti=False
+):
+    get_counts = make_get_counts(corpus, xbtype, ybtype, ylevel)
     hxb = corpus.level_block_to_hblock(xlevel, xb, xbtype)
     yb_counts, _ = get_counts(hxb)
     upx_yb_counts = [get_counts(hxb[:i]) for i in range(1, len(hxb))]
 
     if xlevel == 1:
         sxlevel = "v"
     else:
@@ -277,39 +198,32 @@
     xblocks, _ = corpus.get_blocks_levels(xbtype)
     subxblocks = xblocks[xblocks[xlevel].eq(xb)].groupby(sxlevel)
     subx_yb_counts = []
     for subxb, group in subxblocks:
         hsubxb = corpus.level_block_to_hblock(sxlevel, subxb, xbtype)
         subx_yb_counts.append(get_counts(hsubxb))
 
-    keyf = make_subentropy(subx_yb_counts, upx_yb_counts)
+    keyf = make_nested_commonality(subx_yb_counts, upx_yb_counts)
 
     yblocks = ((x, keyf(x)) for x in yb_counts)
     yblocks = filter(lambda x: x[1] > 0, yblocks)
 
     def sortkeyf(x):
         return -x[1]
 
-    if n is None:
-        return sorted(yblocks, key=sortkeyf)
-    else:
-        return nsmallest(n, yblocks, key=sortkeyf)
+    return nsmallest(num, yblocks, key=sortkeyf)
 
 
 def get_subxblocks_yblocks_elements(
-    corpus, xbtype, xlevel, xb, ybtype, ylevel, num=5, ent_frac=1 / 2
+    corpus, xbtype, xlevel, xb, ybtype, ylevel, num=5, ent_frac=0.5, anti=False
 ):
     xblocks, xlevels = corpus.get_blocks_levels(xbtype)
     yblocks, ylevels = corpus.get_blocks_levels(ybtype)
 
-    def get_counts(hxb):
-        xlevel_, xb_ = corpus.hblock_to_level_block(hxb, xbtype)
-        xyc = corpus.get_xblock_yblocks_counts(xbtype, xlevel_, xb_, ybtype, None)
-        return xyc, sum(xyc.values())
-
+    get_counts = make_get_counts(corpus, xbtype, ybtype, None)
     hxb = corpus.level_block_to_hblock(xlevel, xb, xbtype)
     upx_y_counts = [get_counts(hxb[:i]) for i in range(1, len(hxb))]
 
     subxblocks_yblocks = get_subxblocks_yblocks(
         corpus, xbtype, xlevel, xb, ybtype, ylevel
     )
 
@@ -325,15 +239,15 @@
 
     yblocks_elements = {}
     for yb, yb_ent in yield_values_fraction(subxblocks_yblocks, ent_frac):
         yblocks_elements[yb] = {"ent": yb_ent, "elements": []}
     total_ent = sum(v for _, v in subxblocks_yblocks if v > 0)
     cum_ent = sum(x["ent"] for x in yblocks_elements.values())
 
-    keyf = make_subentropy(subx_y_counts, upx_y_counts)
+    keyf = make_nested_commonality(subx_y_counts, upx_y_counts)
 
     for yb, ybinfo in yblocks_elements.items():
         elements = yblocks[yblocks[ylevel].eq(yb)].index
         elements = ((x, keyf(x)) for x in elements)
         elements = filter(lambda x: x[1] > 0, elements)
         elements = list(elements)
         ybinfo["ent_el"] = sum(x[1] for x in elements)
@@ -357,28 +271,28 @@
 
 ######################
 # xblock annotations #
 ######################
 
 
 def get_xblock_xelements(
-    corpus, xbtype, xlevel, xb, order, ybtype=None, n=None, sxblocks=None
+    corpus, xbtype, xlevel, xb, order, ybtype=None, num=None, sxblocks=None
 ):
     xblocks, _ = (
         corpus.get_blocks_levels(xbtype) if sxblocks is None else (sxblocks, None)
     )
     if ybtype:
         xelement_yelements = corpus.get_xelement_yelements(xbtype, ybtype)
     xelements = xblocks[xblocks[xlevel].eq(xb)]
-    n = min(n, len(xelements)) if n is not None else len(xelements)
+    num = min(num, len(xelements)) if num is not None else len(xelements)
     if order == "time":
         assert xbtype == "doc"
         return corpus.data.loc[xelements.index].sort_values(corpus.col_time).index
     if order == "sample":
-        xs = xelements.sample(n).index
+        xs = xelements.sample(num).index
         if xbtype == "doc":
             return corpus.data.loc[xs, corpus.col_title].astype(str).to_list()
         if ybtype:
 
             def keyf(x):
                 return -sum(xelement_yelements[x].values())
 
@@ -387,22 +301,22 @@
             return list(xs)
     if xbtype == "term" and order == "concentration":
         grade, _, _ = corpus.get_graded_vocab_cached(corpus.column, sampled=True)
 
         def keyf(x):
             return -grade[x]
 
-        return sorted(xelements.index, key=keyf)[:n]
+        return sorted(xelements.index, key=keyf)[:num]
     if order == "frequency":
 
         def keyf(x):
             return -sum(xelement_yelements[x].values())
 
-        xs = [x for x in nsmallest(n, xelements.index, key=keyf)]
-        # xs_freq = [-keyf(x) for x in nsmallest(n, xelements.index, key=keyf)]
+        xs = [x for x in nsmallest(num, xelements.index, key=keyf)]
+        # xs_freq = [-keyf(x) for x in nsmallest(num, xelements.index, key=keyf)]
         # xs_cumfreq = [sum(xs_freq[: i + 1]) for i in range(len(xs))]
         # total_freq = sum(-keyf(x) for x in xelements.index)
         return [
             # f"{x} <small>({-keyf(x)}, "
             # + f"{xs_freq[i]/total_freq:.0%}/{xs_cumfreq[i]/total_freq:.0%})</small>"
             (x, -keyf(x))
             for i, x in enumerate(xs)
@@ -410,14 +324,47 @@
 
 
 ########
 # misc #
 ########
 
 
+def make_get_counts(corpus, xbtype, ybtype, ylevel):
+    _, xlevels = corpus.get_blocks_levels(xbtype)
+
+    def get_regular_counts(hxb):
+        xlevel_, xb_ = corpus.hblock_to_level_block(hxb, xbtype)
+        xyc = corpus.get_xblock_yblocks_counts(xbtype, xlevel_, xb_, ybtype, ylevel)
+        return xyc, sum(xyc.values())
+
+    def get_anti_counts(hxb):
+        xlevel_, xb_ = corpus.hblock_to_level_block(hxb, xbtype)
+        counts = []
+        for axlevel in [xl for xl in xlevels if xl > xlevel_]:
+            xyc = corpus.get_antixblock_yblocks_counts(
+                xbtype, xlevel_, xb_, axlevel, ybtype, ylevel
+            )
+            counts.append((xyc, sum(xyc.values())))
+        return counts
+
+    def get_counts(hxb, anti=False):
+        if anti:
+            return get_anti_counts(hxb)
+        return get_regular_counts(hxb)
+
+    return get_counts
+
+
+def nsmallest(n, iterable, key):
+    if n is None:
+        return sorted(iterable, key=key)
+    else:
+        return heapq_nsmallest(n, iterable, key=key)
+
+
 def yield_values_fraction(keys_values, frac):
     total = sum(v for _, v in keys_values if v > 0)
     cum = 0.0
     for k, v in keys_values:
         cum += v
         yield (k, v)
         if cum > total * frac:
@@ -492,40 +439,52 @@
             for url in urls:
                 title += f'<a target="_blank" href="{html.escape(str(url))}">🗎</a>'
         return title
 
     return get_title
 
 
+#########
+# cache #
+#########
+
+
 def load_annotations(
-    corpus, annotation_function, xbtype, ybtype, ylevel=1, num=5, ent_frac=1 / 2
+    corpus, annotation_function, xbtype, ybtype, ylevel=1, num=5, ent_frac=0.5
 ):
-    use_cache = getattr(corpus, "cached_annotations", True)
+    use_cache = corpus.use_cached_annotations
+    use_cache_sample = corpus.use_cached_annotations_sampled
     if use_cache:
         if all(t in ("doc", "ter") for t in (xbtype, ybtype)):
             fdir = corpus.blocks_dir
         else:
             fdir = corpus.chained_dir
+        fname_params = (
+            ("xbtype", xbtype),
+            ("ybtype", ybtype),
+            ("ylevel", ylevel),
+            ("num", num),
+            ("ent_frac", ent_frac),
+        )
+        sample_hash = corpus.get_sample_hash(
+                **{x: x in {xbtype, ybtype} for x in ["doc", "ter", "ext"]}
+        ) if use_cache_sample else None
+        if sample_hash := :
+                fname_params = [("sample", sample_hash), *fname_params]
         fpath = (
             fdir
             / "cache"
             / naming.gen(
                 annotation_function.__name__,
-                (
-                    ("xbtype", xbtype),
-                    ("ybtype", ybtype),
-                    ("ylevel", ylevel),
-                    ("num", num),
-                    ("ent_frac", ent_frac),
-                ),
+                fname_params,
                 ".pickle.xz",
             )
         )
         if fpath.exists():
-            print("Loading cached annotations!")
+            print(f"Loading cached {'sampled' if sample_hash else ''} annotations!")
             return ioio.load(fpath)
 
     annotations = {}
     xblocks, xlevels = corpus.get_blocks_levels(xbtype)
     for xlevel in tqdm(xlevels):
         annotations[xlevel] = {}
         for xb in tqdm(xblocks[xlevel].unique()):
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/blocks/area_rank_chart.py` & `sashimi_domains-0.9.3/src/sashimi/blocks/area_rank_chart.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.2/src/sashimi/blocks/block_ext_map.py` & `sashimi_domains-0.9.3/src/sashimi/blocks/block_ext_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding: utf-8
-
 # Sashimi - Study of the organisation and evolution of a corpus
 #
 # Author(s):
 # * Ale Abdo <abdo@member.fsf.org>
 #
 # License:
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/blocks/hierarchical_block_map.py` & `sashimi_domains-0.9.3/src/sashimi/blocks/hierarchical_block_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding: utf-8
-
 # Sashimi - Study of the organisation and evolution of a corpus
 #
 # Author(s):
 # * Ale Abdo <abdo@member.fsf.org>
 #
 # License:
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
@@ -101,17 +99,22 @@
     ]
     zname = [map_args["zmethod"].__name__ for map_args in maps_args]
 
     if page_title is None:
         page_title = f'{"|".join(corpus.loaded["data"])}: {len(corpus.data)} documents'
 
     name_args = "norm", "scale", "bheight"
+    fname_params = [
+        (key, [maps_args[i][key] for i in range(len(btype))]) for key in name_args
+    ]
+    if sample_hash := corpus.get_sample_hash(**{x: True for x in btype}):
+        fname_params = [("sample", sample_hash), *fname_params]
     fname = naming.gen(
         f"domain_map_{btype}_{zname}",
-        [(key, [maps_args[i][key] for i in range(len(btype))]) for key in name_args],
+        fname_params,
         "html",
     )
 
     # Object shared by all maps
     document_data = bkm.ColumnDataSource(
         {
             "title": corpus.data.reset_index().agg(
@@ -182,20 +185,18 @@
 
     if len(btype) in (1, 2):
         # link figures
         if btype in (["doc", "ter"], ["doc", "ext"]):
             map_d = ["doc", figs[0], corpus.dblocks, corpus.dblocks_levels]
             if btype[1] == "ter":
                 map_x = ["ter", figs[1], corpus.tblocks, corpus.tblocks_levels]
-                # values_x = corpus.values_ter_doc_count_all
-                values_x = corpus.values_ter_link_count_all
+                values_x = zmethods.get_cross_counts(corpus, "ter", "link")
             if btype[1] == "ext":
                 map_x = ["ext", figs[1], corpus.eblocks, corpus.eblocks_levels]
-                # values_x = corpus.values_ext_doc_count_all
-                values_x = corpus.values_ext_link_count_all
+                values_x = zmethods.get_cross_counts(corpus, "ext", "link")
             for map_s, map_t in ([map_d, map_x], [map_x, map_d]):
                 link_maps(
                     corpus,
                     *map_s,
                     *map_t,
                     values=values_x,
                     selection_mode=selection_mode,
@@ -495,15 +496,15 @@
         args=dict(source=source, fig=fig),
         v_func=process_items_js
         + """
         function preprocess_items (_items, i) {
             const items = [..._items]
             const [btype, ent] = items[0]
             const level_is_1 = source.data["x"][i] == 1
-            const title = `${level_is_1 ? "≏" : "⋂"} ${ent.toPrecision(2)}`
+            const title = `${level_is_1 ? "≏" : "⋂"} ${Math.pow(2, ent).toPrecision(2)}`
             if (items.length > 1) {
                 items.shift()
                 items[0] = [`${title}　⁄　${items[0][0]}`, ...items[0].slice(1)]
             } else {
                 items[0] = [`${title}`, ...items[0].slice(1)]
             }
             return items
@@ -888,15 +889,15 @@
                 return source.data[key][index]
             }
         )
         texts.push(infobox_text)
     }
     if (texts.length){
         infobox.text = (
-            '<div style="width:49.5lvw; max-height:95lvh; overflow:auto">'
+            '<div style="width:49.25lvw; max-height:95lvh; overflow:auto">'
             + texts.join("<hr>")
             + "</div>"
         )
     }
     else {
         infobox.text = "<big>I suggest you try clicking on a block. 😉</big>"
     }
@@ -1031,16 +1032,18 @@
         for _btype in (xbtype, "doc")
         for _blocks, _levels in [corpus.get_blocks_levels(_btype)]
         for _level in _levels
         for _block in _blocks[_level].unique()
     )
 
     searchbox = bkm.AutocompleteInput(
-        placeholder="🔍 Enter a term, or /b followed by a block label, or /d followed by a document title (ESC to unselect all)",
+        placeholder="🔍 Enter a term, or /b followed by a block label,"
+        " or /d followed by a document title (ESC to unselect all)",
         completions=sorted(completions),
+        max_completions=1024,
         case_sensitive=False,
         sizing_mode="stretch_width",
         align="center",
     )
     searchbox_cb = CustomJS(
         args=dict(
             xsource=xsource,
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/blocks/hierarchical_block_map_help.html` & `sashimi_domains-0.9.3/src/sashimi/blocks/hierarchical_block_map_help.html`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.2/src/sashimi/blocks/link_maps.py` & `sashimi_domains-0.9.3/src/sashimi/blocks/link_maps.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.2/src/sashimi/blocks/network_map.py` & `sashimi_domains-0.9.3/src/sashimi/blocks/network_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding: utf-8
-
 # Sashimi - Study of the organisation and evolution of a corpus
 #
 # Author(s):
 # * Ale Abdo <abdo@member.fsf.org>
 #
 # License:
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
@@ -36,27 +34,33 @@
     corpus,
     xbtype,
     doc_level,
     ter_level,
     ext_level,
     *,
     xb_selection=None,
-    force_specific=False,
+    edges="specific",
 ):
     def first_element(yb_info_elements):
         return yb_info_elements[0][0] if yb_info_elements else ""
 
     xlevel = {"doc": doc_level, "ter": ter_level, "ext": ext_level}[xbtype]
-    xb_selection = set(xb_selection)
+    if edges == "specific":
+        annotation_function = get_xblock_yblocks_elements
+    elif edges == "common":
+        if xlevel == 1:
+            raise ValueError(
+                f"`edges=common` requires xbtype (here `{xbtype}`) level > 1 (here `{xlevel}`)."
+            )
+        annotation_function = get_subxblocks_yblocks_elements
+    else:
+        raise ValueError("`edges` must be one of ['specific', 'common']")
+
     annotations_ylevel = []
-    annotation_function = (
-        get_xblock_yblocks_elements
-        if force_specific or xlevel == 1
-        else get_subxblocks_yblocks_elements
-    )
+    xb_selection = set(xb_selection)
 
     if xbtype == "doc":
         if ter_level is not None:
             ter_annotations = load_annotations(
                 corpus, annotation_function, "doc", "ter", ter_level
             )
             annotations_ylevel.append((ter_annotations, ter_level))
@@ -110,29 +114,32 @@
     doc_level,
     ter_level=1,
     ext_level=None,
     *,
     xb_selection=None,
     split_on=None,
     split_list=None,
-    force_specific=False,
+    edges="specific",
 ):
     """
     (corpus)
+    (xbtype)
     (doc_level) display document nodes from this level
     (ter_level) display term nodes from this level
     (ext_level) display chained nodes from this level
 
+    (xb_selection) list of int
+        Restrict the network to a list of domains from `doc_level`
+
     Show a halo on domain nodes for the difference in relative volume
     between those in and out of a set of values such as years:
     (split_on) series of values based on which to split
     (split_list) values from split series to consider positive
 
-    (dblocks) list of int
-        Restrict the network to a list of domains from `doc_level`
+    (edges): measure determining edges ("specific" or "common")
     """
     xblocks, xblocks_levels = corpus.get_blocks_levels(xbtype)
     xlevel = {"doc": doc_level, "ter": ter_level, "ext": ext_level}[xbtype]
     arg_xb_selection = xb_selection
     if xb_selection is None:
         xb_selection = xblocks[xlevel]
     xb_selection = np.unique(xb_selection)
@@ -140,15 +147,15 @@
     g = dblock_terext_graph(
         corpus,
         xbtype,
         doc_level,
         ter_level,
         ext_level,
         xb_selection=xb_selection,
-        force_specific=force_specific,
+        edges=edges,
     )
     vp_label = g.vp["label"]
 
     vp_block = g.new_vertex_property("int")
     for v in g.vertices():
         vp_block[v] = corpus.label_to_hblock[vp_label[v]][-1]
 
@@ -205,30 +212,29 @@
 
     g.vp["position"] = gt.sfdp_layout(
         g, eweight=gt.prop_to_size(g.ep["specificity"], mi=0.01, power=1)
     )
 
     fname_params = [
         ("xbtype", xbtype),
+        ("edges", edges),
         ("doc_level", doc_level),
         ("ter_level", ter_level),
         ("ext_level", ext_level),
         (
             "xblocks",
             None
             if arg_xb_selection is None
             else get_hash(tuple(xb_selection.tolist())),
         ),
         ("split_on", getattr(split_on, "name", None)),
         ("split_list", None if split_list is None else get_hash(tuple(split_list))),
     ]
     if sample_hash := corpus.get_sample_hash(doc=True, ter=ter_level, ext=ext_level):
         fname_params = [("sample", sample_hash), *fname_params]
-    if force_specific:
-        fname_params = [*fname_params, ("force_specific", force_specific)]
 
     target_dir = corpus.blocks_adir if ext_level is None else corpus.chained_adir
     fpath_graphml = target_dir / naming.gen("network_map", fname_params, "graphml")
     fpath_pdf = target_dir / naming.gen("network_map", fname_params, "pdf")
     fpath_svg = target_dir / naming.gen("network_map", fname_params, "svg")
     g.save(str(fpath_graphml))
     draw(g, str(fpath_pdf))
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/blocks/util.py` & `sashimi_domains-0.9.3/src/sashimi/blocks/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding: utf-8
-
 # Sashimi - Study of the organisation and evolution of a corpus
 #
 # Author(s):
 # * Ale Abdo <abdo@member.fsf.org>
 #
 # License:
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/blocks/zmethods.py` & `sashimi_domains-0.9.3/src/sashimi/blocks/zmethods.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding: utf-8
-
 # Sashimi - Study of the organisation and evolution of a corpus
 #
 # Author(s):
 # * Ale Abdo <abdo@member.fsf.org>
 #
 # License:
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
@@ -14,20 +12,19 @@
 #
 # Reference repository for this file:
 # <https://gitlab.com/solstag/abstractology>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 import pandas
-from pathlib import Path
 from collections import Counter
 from tqdm import tqdm
 
 from ..ioio import ioio
-
+from ..naming import naming
 
 """
 Methods to be used with hierarchical_block_map.
 
 'zmethods' should be defined as:
 
 def example(corpus, blocks, level, index)
@@ -169,57 +166,56 @@
 
     x_doc_density_pair.__name__ = "{}_doc_density_{}_{}_{}".format(
         btype, func.__name__, idx0.name, idx1.name
     )
     return x_doc_density_pair
 
 
-def load_cross_count_all(corpus, ybtype, ltype):
+def get_cross_counts(corpus, ybtype, ltype):
     """
     Pairs every domain from every level with every cross block from every
     level (topics or extended blocks) and counts the number of links or documents
     connected to each cross block.
 
     (corpus)
-    (btype): str
+    (ybtype): str
         The block type to cross. Either 'ter' or 'ext'.
     (ltype) str
         Either 'link' or 'doc'. Whether to count links or documents.
-    (store) bool
-        Store the result to a file.
-    (from_file) bool
-        Attempt to read from a stored result.
 
     Result
     ------
-    Sets corpus.'values_{btype}_{ltype}_count_all', to a pandas.Series with MultiIndex
-
+    A pandas.Series with MultiIndex:
     (domain level, domain, cross level, cross block)
     """
-    use_cache = getattr(corpus, "cached_cross_count", True)
+    use_cache = corpus.use_cached_cross_counts
     dblocks = corpus.dblocks
     yblocks, yblocks_levels, _ = corpus.get_blocks_levels_sample(ybtype)
     y_documents = corpus.get_xelement_yelements(ybtype, "doc")
-    attr_name = f"values_{ybtype}_{ltype}_count_all"
+    fname_params = [("ybtype", ybtype), ("ltype", ltype)]
+    if sample_hash := corpus.get_sample_hash(
+        **{x: x in {"doc", ybtype} for x in ["doc", "ter", "ext"]}
+    ):
+        fname_params = [("sample", sample_hash), *fname_params]
     if ybtype == "ter":
         fdir = corpus.blocks_dir
     elif ybtype == "ext":
         fdir = corpus.chained_dir
-    fpath = Path(fdir, f"{attr_name}{corpus.data_file_extension}")
-    if use_cache:
+    fpath = fdir / "cache" / naming.gen("cross_counts", fname_params, corpus.ext_data)
 
+    if use_cache:
         try:
             values = ioio.load(fpath)
-            values = pandas.Series(
-                index=pandas.MultiIndex.from_tuples(values["index"]),
-                data=(x for x in values["data"]),
-            )
-            setattr(corpus, attr_name, values)
-            print("Loaded cached cross count")
-            return
+            if isinstance(values, dict):
+                values = pandas.Series(
+                    index=pandas.MultiIndex.from_tuples(values["index"]),
+                    data=(x for x in values["data"]),
+                )
+            print("Loaded cached cross counts")
+            return values
         except FileNotFoundError:
             pass
 
     keys, vals = [], []
     for ylevel in tqdm(yblocks_levels, desc="Cross level"):
         y_groups = yblocks[ylevel].groupby(yblocks[ylevel])
         for yb, yg in tqdm(y_groups, desc=f"  {ybtype.capitalize()} block"):
@@ -234,18 +230,18 @@
                         g_index = set(g.index)
                         vals.append(sum(v for k, v in yb_docs.items() if k in g_index))
                     else:  # ltype == 'doc'
                         vals.append(len(g.index.intersection(yb_docs)))
 
     values = pandas.Series(vals, index=pandas.MultiIndex.from_tuples(keys))
 
-    setattr(corpus, attr_name, values)
     if use_cache:
-        print("Storing cross count values")
+        print("Storing cross counts")
         ioio.store_pandas(values, fpath)
+    return values
 
 
 def p_diff(a, b):
     return a - b
 
 
 def p_rel(a, b):
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/blocks/tables/__init__.py` & `sashimi_domains-0.9.3/src/sashimi/blocks/tables/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 #
 # Reference repository for this file:
 # <https://gitlab.com/solstag/abstractology>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 import re
+import logging
+from pathlib import Path
 
 import pandas as pd
 
 from ..util import sorted_hierarchical_block_index
 from ..annotations import (
     get_xblock_yblocks_elements,
     get_subxblocks_yblocks_elements,
@@ -31,14 +33,16 @@
     html_output,
     html_multi_xblocks_yblocks_table,
     html_domain_documents_table,
     html_xblock_yblocks_table,
 )
 from .tables_plots import get_time_plot
 
+logger = logging.getLogger(__name__)
+
 
 def subxblocks_report(
     corpus, xbtype, xlevel, xb, ybtype, ylevel=1, *, outfile=None, plots=False
 ):
     """
     Produces a table reporting on the topic assemblages for each subxblock
     of `xb`.
@@ -96,20 +100,19 @@
         for sxlevel, sxb in get_subxblocks(corpus, xbtype, xlevel, xb, 1):
             sxdata = data[xlevel, xb][l1_label][sxb] = get_xblock_data(
                 corpus,
                 xbtype,
                 sxlevel,
                 sxb,
                 ybtype,
-                ylevel,
                 annotations[sxlevel][sxb],
                 plots=plots,
             )
             if xbtype == "doc":
-                sxdata["examples"] = sxdata["examples"].agg(get_title, axis=1)
+                sxdata["elements"] = sxdata["examples"].agg(get_title, axis=1)
 
     report = html_multi_xblocks_yblocks_table(data, xbtype, labels, plots=plots)
     if outfile is None:
         return report
     else:
         return html_output(report, outfile)
 
@@ -120,14 +123,15 @@
     ybtype,
     ylevel=1,
     *,
     outfile=None,
     plots=False,
     docs=slice(None),
     code_terms_map=None,
+    code_terms_restrict=None,
 ):
     """
     Produces a table reporting on a single domain's yblock assemblages and documents.
     """
     labels = make_labels(corpus.lblock_to_label, get_labels(corpus))
     get_title = make_get_title(corpus.col_title, corpus.col_url, corpus.col_time)
     annotations = load_annotations(
@@ -135,95 +139,147 @@
     )
     data = get_xblock_data(
         corpus,
         "doc",
         1,
         dblock,
         ybtype,
-        ylevel,
         annotations[1][dblock],
         plots=plots,
     )
-    data["abstracts"] = data["examples"].loc[docs, corpus.text_sources]
-    if corpus.col_venue:
-        data["venues"] = data["examples"].loc[docs, corpus.col_venue]
+    sample = data["examples"].loc[docs]
     if code_terms_map:
-        get_code_terms = make_get_code_terms(
+        get_code_terms = make_match_code_terms(
             corpus.col_title, corpus.text_sources, code_terms_map
         )
-        data["code_terms"] = data["examples"].loc[docs].agg(get_code_terms, axis=1)
-    data["examples"] = (
-        data["examples"].loc[docs].agg(get_title, axis=1)
-    )  # must come last
+        code_terms = sample.agg(get_code_terms, axis=1)
+        if code_terms_restrict:
+            sel_code_terms = code_terms.map(code_terms_restrict.intersection)
+            sample = sample.loc[sel_code_terms.astype(bool)]
+            code_terms = code_terms.reindex_like(sample)
+        data["code_terms"] = code_terms
+    data["examples"] = sample
+    data["abstracts"] = sample[corpus.text_sources]
+    if corpus.col_venue:
+        data["venues"] = sample[corpus.col_venue]
+    data["titles"] = sample.agg(get_title, axis=1)
     report_domain = html_xblock_yblocks_table(data, "doc", labels)
     report_contents = html_domain_documents_table(data, labels, code_terms_map)
     report = [report_domain, report_contents]
     if outfile is None:
         return report
     else:
         return html_output(report, outfile)
 
 
-def get_xblock_data(
-    corpus, xbtype, xlevel, xb, ybtype, ylevel, annotated, *, plots=False
+def l1domains_code_terms_report(
+    corpus,
+    doc_levels_blocks,
+    ybtype,
+    ylevel=1,
+    *,
+    outdir=None,
+    plots=False,
+    docs=slice(None),
+    code_terms_map=None,
 ):
+    if any(dlevel != 1 for dlevel, _ in doc_levels_blocks):
+        raise ValueError("`doc_level_blocks` must only contain level 1 domains")
+    outdir = Path(outdir)
+    outdir.mkdir(exist_ok=True)
+    for code_term in code_terms_map:
+        code_term_dir = outdir / code_term
+        code_term_dir.mkdir(exist_ok=True)
+        for dlevel, dblock in doc_levels_blocks:
+            outfile = code_term_dir / f"{corpus.lblock_to_label[dlevel, dblock]}.html"
+            l1domain_full_report(
+                corpus,
+                dblock,
+                ybtype,
+                ylevel,
+                outfile=outfile,
+                plots=plots,
+                docs=docs,
+                code_terms_map=code_terms_map,
+                code_terms_restrict={code_term},
+            )
+
+
+def get_xblock_data(corpus, xbtype, xlevel, xb, ybtype, annotated, *, plots=False):
     """
     Get the report data for the given domain.
     """
     order = "frequency" if ybtype == "doc" else "time"
     xblocks_elements = get_xblock_xelements(
-        corpus, xbtype, xlevel, xb, order, ybtype=ybtype, n=None
+        corpus, xbtype, xlevel, xb, order, ybtype=ybtype, num=None
     )
     data = {
         "id": corpus.lblock_to_label[xlevel, xb],
         "specific": annotated,
     }
     if xbtype == "doc":
         data["examples"] = corpus.data.loc[xblocks_elements]
     else:
-        data["examples"] = data["examples"].map(
+        data["examples"] = corpus.data.loc[xblocks_elements].map(
             lambda x: f"{x[0]} <small>({x[1]})</small>"
         )
     if plots:
         data["plot"] = get_time_plot(corpus, xbtype, xlevel, xb)
 
     return data
 
 
-def get_codes_frequencies(corpus, dlevel, dblock, code_terms_map):
-    get_code_terms = make_get_code_terms(
+##########
+# Coding #
+##########
+
+
+def code_frequency_tables(corpus, domain_labels, code_terms_map, fname_prefix=None):
+    if fname_prefix is None:
+        fname_prefix = ",".join(domain_labels) + "_×_" + ",".join(code_terms_map)
+    match_code_terms = make_match_code_terms(
         corpus.col_title, corpus.text_sources, code_terms_map
     )
-    domain = corpus.data.loc[corpus.dblocks[dlevel].eq(dblock)]
-    domain_codes = domain.agg(get_code_terms, axis=1)
-    domain_codes_cooc = domain_codes.map(tuple).value_counts()
-    domain_codes_count = domain_codes.explode().value_counts()
-    domain_codes_cooc.name = corpus.lblock_to_label[dlevel, dblock]
-    domain_codes_count.name = corpus.lblock_to_label[dlevel, dblock]
-    return domain_codes_cooc, domain_codes_count
+    code_coocs, code_frequencies = get_codes_frequencies(
+        corpus,
+        [corpus.label_to_tlblock[dl][1:] for dl in domain_labels],
+        match_code_terms,
+    )
+    code_frequencies.to_csv(
+        corpus.blocks_adir / f"{fname_prefix}-code_domain_frequencies.csv"
+    )
+    code_coocs.to_csv(corpus.blocks_adir / f"{fname_prefix}-code_colocations.csv")
 
 
-def code_frequency_tables(corpus, domain_labels, code_terms_map):
-    code_coocs_d = {}
-    code_frequencies_d = {}
-    for dl in domain_labels:
-        cc, cf = get_codes_frequencies(
-            corpus, *corpus.label_to_tlblock[dl][-2:], code_terms_map
-        )
-        code_coocs_d[cc.name] = cc
-        code_frequencies_d[cf.name] = cf
-    code_frequencies = pd.DataFrame(code_frequencies_d, dtype="Int64").fillna(0)
-    code_frequencies.loc["Total"] = code_frequencies.sum().astype("Int64")
-    code_frequencies["Total"] = code_frequencies.sum(axis=1).astype("Int64")
-    code_coocs = pd.concat(code_coocs_d.values())
-    code_coocs = code_coocs.groupby(code_coocs.index).sum()
-    code_coocs.name = "Colocations"
-    code_frequencies.to_csv(corpus.blocks_adir / "code_domain_frequencies.csv")
-    code_coocs.to_csv(corpus.blocks_adir / "code_colocations.csv")
-    
+def get_codes_frequencies(corpus, doc_levels_blocks, match_code_terms):
+    col_any, col_size, col_sum = ["#Any", "#Size", "#Sum"]
+    domains_codes_count_d = {}
+    codes_coocs_count_d = {}
+    for dlevel, dblock in doc_levels_blocks:
+        dlabel = corpus.lblock_to_label[dlevel, dblock]
+        domain = corpus.data.loc[corpus.dblocks[dlevel].eq(dblock)]
+        domain_codes = domain.agg(match_code_terms, axis=1)
+        codes_coocs_count_d[dlabel] = domain_codes.map(tuple).value_counts()
+        codes_coocs_count_d[dlabel][col_any] = domain_codes.astype(bool).sum()
+        codes_coocs_count_d[dlabel][col_size] = len(domain_codes)
+        domains_codes_count_d[dlabel] = domain_codes.explode().value_counts()
+        domains_codes_count_d[dlabel][col_any] = domain_codes.astype(bool).sum()
+        domains_codes_count_d[dlabel][col_size] = len(domain_codes)
+
+    codes_coocs_count = pd.concat(codes_coocs_count_d.values())
+    codes_coocs_count = codes_coocs_count.groupby(codes_coocs_count.index).sum()
+    codes_coocs_count = codes_coocs_count.sort_values(ascending=False)
+    codes_coocs_count.name = "Colocations"
+
+    domains_codes_count = pd.DataFrame(domains_codes_count_d, dtype="Int64").fillna(0)
+    domains_codes_count[col_sum] = domains_codes_count.sum(axis=1).astype("Int64")
+    domains_codes_count = domains_codes_count.sort_values(col_sum, ascending=False)
+
+    return codes_coocs_count, domains_codes_count
+
 
 ####################
 # Helper functions #
 ####################
 
 
 def get_subxblocks(corpus, xbtype, xlevel, xb, sxlevel=None):
@@ -248,20 +304,20 @@
 
 def get_labels(corpus, fpath=None):
     if (fpath is not None) and fpath.exists():
         return pd.read_csv(fpath).set_index("Domain")["Label"]
     return pd.Series(dtype=object)
 
 
-def make_get_code_terms(col_title, text_sources, code_terms_map):
+def make_match_code_terms(col_title, text_sources, code_terms_map):
     code_terms_rx = {k: re.compile(rf"(?i)\b{v}\b") for k, v in code_terms_map.items()}
     text_columns = sorted(set([col_title, *text_sources]))
 
-    def get_code_terms(row):
+    def match_code_terms(row):
         code_terms = set()
         for key, rex in code_terms_rx.items():
             for text in row[text_columns]:
                 if rex.search(text):
                     code_terms.add(key)
         return sorted(code_terms)
 
-    return get_code_terms
+    return match_code_terms
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/blocks/tables/tables.css` & `sashimi_domains-0.9.3/src/sashimi/blocks/tables/tables.css`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 th {
     background-color: #4CAF50;
     color: white;
 }
 .tstats {
     opacity:.5;
 }
-.examples > ul {
+.elements > ul {
     max-height: 300px;
     overflow-y: auto;
     padding-left: 15px;
 }
 .code_terms > ul {
     padding-left: 15px;
 }
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/blocks/tables/tables_html.py` & `sashimi_domains-0.9.3/src/sashimi/blocks/tables/tables_html.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,19 +41,21 @@
     tr.append(E.TH("Abstract"))
     if "code_terms" in data:
         tr.append(E.TH("Code terms"))
     table = E.TABLE(
         E.THEAD(tr),
         tbody := E.TBODY(),
     )
-    for idx, example in data["examples"].items():
+    for idx in data["examples"].index:
         tr = E.TR()
         if "venues" in data:
             tr.append(E.TD(data["venues"].loc[idx]))
-        tr.append(E.TD(html.fragment_fromstring(example, create_parent="p")))
+        tr.append(
+            E.TD(html.fragment_fromstring(data["titles"].loc[idx], create_parent="p"))
+        )
         tr.append(
             E.TD(
                 *[
                     y
                     for x in data["abstracts"].loc[idx]
                     for y in (*format_marks(x), E.HR)
                 ][:-1],
@@ -110,21 +112,21 @@
 
 def html_multi_xblocks_yblocks_table(data, xbtype, labels, plots=False):
     levels = sorted(set(x[0] for x in data))
     deep = levels != [1]
     ln_label = f"L{levels[-1]}{xbtype[0].upper()}" if len(levels) == 1 else "ID"
     l1_label = f"L1{xbtype[0].upper()}"
     columns = (
-        ["Plot", ln_label, "Common", "Plot", l1_label, "Specific", "Examples"]
+        ["Plot", ln_label, "Common", "Plot", l1_label, "Specific", "Elements"]
         if deep and plots
-        else [ln_label, "Common", l1_label, "Specific", "Examples"]
+        else [ln_label, "Common", l1_label, "Specific", "Elements"]
         if deep and not plots
-        else ["Plot", l1_label, "Specific", "Examples"]
+        else ["Plot", l1_label, "Specific", "Elements"]
         if not deep and plots
-        else [l1_label, "Specific", "Examples"]
+        else [l1_label, "Specific", "Elements"]
     )
     table = E.TABLE(E.THEAD(E.TR(*(E.TH(str(key)) for key in columns))))
     tbody = E.TBODY()
     table.append(tbody)
     for _, d_data in data.items():
         drow = E.TR()
         if deep:
@@ -165,15 +167,15 @@
                         ),
                         CLASS="label",
                     ),
                     E.TD(
                         *format_xblock_yblocks_elements(sd_data["specific"], labels),
                         CLASS="yblocks",
                     ),
-                    E.TD(format_examples(sd_data["examples"]), CLASS="examples"),
+                    E.TD(format_elements(sd_data["elements"]), CLASS="elements"),
                 )
             )
             drow = E.TR()
     return E.DIV(table)
 
 
 def format_xblock_yblocks_elements(xblock_yblocks_elements, labels):
@@ -203,26 +205,26 @@
         formatted.append(E.BR())
     if formatted:
         formatted.pop()
 
     return formatted
 
 
-def format_examples(examples):
-    return E.UL(*(html.fragment_fromstring(x, create_parent="li") for x in examples))
+def format_elements(elements):
+    return E.UL(*(html.fragment_fromstring(x, create_parent="li") for x in elements))
 
 
-def format_code_terms(examples):
+def format_code_terms(code_terms):
     return E.UL(
         *(
             html.fragment_fromstring(
                 f'<span style="font-size:0;opacity:0">code:</span>{x}',
                 create_parent="li",
             )
-            for x in examples
+            for x in code_terms
         )
     )
 
 
 def make_format_marks(code_terms_map):
     if code_terms_map is None:
         return lambda x: x
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/blocks/tables/tables_plots.py` & `sashimi_domains-0.9.3/src/sashimi/blocks/tables/tables_plots.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.2/src/sashimi/corpus/__init__.py` & `sashimi_domains-0.9.3/src/sashimi/corpus/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,28 +100,28 @@
         if config_path is not None:
             self.config_path = config_path
         to_load = load_config(get_config_path(config_path, analysis_dir, storage_dir))
 
         # Load properties
         prop_defaults = {
             STORAGE_DIR_KEY: STORAGE_DIR_DEFAULT,
-            "data_file_extension": ".json.xz",
+            "ext_data": ".json.xz",
             "column": None,
             "token_sources": [],
             "text_sources": [],
         }
         self._load_properties(wargs, to_load, prop_defaults)
 
         # Load directory structure
         def get_dir(dir_path, load_key, default_name):
             return Path(
                 dir_path
                 if dir_path is not None
-                else to_load.pop(load_key)
-                if load_key in to_load
+                else to_load["properties"].pop(load_key)
+                if load_key in to_load["properties"]
                 else self.storage_dir / default_name
             )
 
         self.analysis_dir = get_dir(
             analysis_dir, ANALYSIS_DIR_KEY, ANALYSIS_DIR_DEFAULT
         )
         self.resources_dir = get_dir(
@@ -146,15 +146,15 @@
     def _load_properties(self, wargs, to_load, prop_defaults):
         """
         Loads properties with keys in `prop_defaults`, prefering in order:
         - values passed in wargs
         - values passed in to_load
         - values from prop_defaults
         """
-        prop_to_load = to_load.get("properties", {})
+        prop_to_load = to_load["properties"]
         for prop in prop_defaults:
             if wargs.get(prop, None) is not None:
                 setattr(self, prop, wargs[prop])
             elif prop in prop_to_load:
                 setattr(self, prop, prop_to_load.pop(prop))
             else:
                 setattr(self, prop, prop_defaults[prop])
@@ -204,15 +204,15 @@
             self._column = column
         else:
             raise KeyError("`column` must be a valid key in the data.")
 
     column = makep("column", True, _set_column, None)
     token_sources = makep("token_sources")
     text_sources = makep("text_sources")
-    data_file_extension = makep("ext_data")
+    ext_data = makep("ext_data")
     _column_label_keys = {
         "affiliations",
         "authors",
         "id",
         "time",
         "title",
         "url",
@@ -225,15 +225,15 @@
 
     storage_dir = makep(STORAGE_DIR_KEY, True, _fset_dir(STORAGE_DIR_KEY), None)
     analysis_dir = makep(ANALYSIS_DIR_KEY, True, _fset_dir(ANALYSIS_DIR_KEY), None)
     resources_dir = makep(RESOURCES_DIR_KEY, True, _fset_dir(RESOURCES_DIR_KEY), None)
     data_store = property_getfuncdir(lambda self: self.storage_dir / "data")
 
     def _gen_data_name(self, names):
-        return naming.gen("|".join(names), [], self.data_file_extension)
+        return naming.gen("|".join(names), [], self.ext_data)
 
     data_name = property(
         lambda self: self._gen_data_name(self.loaded["data"])
         if self.loaded["data"]
         else None
     )
     data_dir = property_getfuncdir(lambda self: self.data_store / self.data_name)
@@ -279,14 +279,15 @@
         """
         Data is stored under `self.data_store` inside a directory carrying the
         same name as the file to be saved. The file name itelf is derived from
         the value of `self.loaded["data"]`.
 
         If you want to store it somewhere else, use `ioio.store_pandas` instead.
         """
+        columns = [columns] if isinstance(columns, str) else columns
         data = self.data if columns is None else self.data[columns]
         fpath = self.data_dir / self.data_name
         if not overwrite and fpath.exists():
             raise ValueError(
                 f"File {self.data_name} already exists in {self.data_dir}. "
                 f"If you are sure, pass `overwrite=True`"
             )
@@ -307,18 +308,18 @@
         data = ioio.load_pandas(self.data_store / name_in_store / name_in_store)
         if return_not_load:
             return data
         self.load_data(data, name=name)
 
     def list_datasets(self):
         return [
-            fpath.name[: -len(self.data_file_extension)]
+            fpath.name[: -len(self.ext_data)]
             for fpath in self.data_store.iterdir()
             if ioio.uncompressed_suffix(fpath)
-            == ioio.uncompressed_suffix(Path(f"_{self.data_file_extension}"))
+            == ioio.uncompressed_suffix(Path(f"_{self.ext_data}"))
         ]
 
     ################
     # Data methods #
     ################
 
     def check_column(self, default_name="_tokens"):
@@ -326,19 +327,25 @@
         if column is None:
             column = default_name
             if column in self.data:
                 raise ValueError(f"Key `{column}` already present in data.")
             self.data[column] = [[] for _ in range(len(self.data))]
         else:
             if column not in self.data:
-                raise ValueError("Attribute `.column` is set but is not a key in data.")
-            logger.warning(
-                f'Attribute `.column` already set to "{column}": '
-                "loaded tokens will be appended to existing ones."
-            )
+                # raise ValueError("Attribute `.column` is set but is not a key in data.")
+                logger.warning(
+                    f'Attribute `.column` is set to "{column}", which is not a key in data. '
+                    "Processed tokens will be added to a new column."
+                )
+                self.data[column] = [[] for _ in range(len(self.data))]
+            else:
+                logger.warning(
+                    f'Attribute `.column` already set to "{column}". '
+                    "Processed tokens will be appended to existing ones."
+                )
         return column
 
     def process_sources(
         self, ngrams=1, language=None, stop_words=False, tokens_to_doc=None
     ):
         """
         Normalize token data from columns in `self.token_sources` and tokenize and process textual
@@ -565,25 +572,21 @@
 
     def cache_clear(self, clear_static=False):
         if clear_static and clear_static != "ext":
             clearattrs(
                 self,
                 [
                     "ter_documents",
-                    "values_ter_link_count_all",
-                    "values_ter_doc_count_all",
                 ],
             )
         if clear_static and clear_static != "ter":
             clearattrs(
                 self,
                 [
                     "ext_documents",
-                    "values_ext_link_count_all",
-                    "values_ext_doc_count_all",
                 ],
             )
         for m in dir(type(self)):
             m = getattr(type(self), m)
             if hasattr(m, "cache_clear"):
                 m.cache_clear()
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/corpus/nlp.py` & `sashimi_domains-0.9.3/src/sashimi/corpus/nlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,28 +177,24 @@
     if isinstance(obj, class_or_tuple):
         for ob in obj:
             yield from flatten_nested_containers(ob, class_or_tuple, dropna)
     elif not dropna or not strict_na(obj):
         yield obj
 
 
-def wordsentence(docs, in_class_or_tuple=(list, tuple), out_class=list):
+def wordsentence(doc, in_class_or_tuple=(list, tuple), out_class=list):
     """
-    Convert elements to Document[Sentence[Word...]...] form
+    Convert element to Document[Sentence[Word...]...] form
     """
-
-    def wordsentence_doc(d):
-        if strict_na(d):
-            return d
-        if isinstance(d, in_class_or_tuple):
-            return out_class(
-                out_class(flatten_nested_containers(s, in_class_or_tuple, True))
-                for s in d
-                if not strict_na(s)
-            )
-        return out_class([out_class([d])])
-
-    return docs.map(wordsentence_doc)
+    if strict_na(doc):
+        return doc
+    if isinstance(doc, in_class_or_tuple):
+        return out_class(
+            out_class(flatten_nested_containers(sen, in_class_or_tuple, True))
+            for sen in doc
+            if not strict_na(sen)
+        )
+    return out_class([out_class([doc])])
 
 
 def tokens_to_doc(tokens):
     return [[x] if isinstance(x, str) else [*x] for x in tokens]
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/corpus/parsers.py` & `sashimi_domains-0.9.3/src/sashimi/corpus/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding: utf-8
-
 # Sashimi - Study of the organisation and evolution of a corpus
 #
 # Author(s):
 # * Ale Abdo <abdo@member.fsf.org>
 #
 # License:
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/corpus/wos.py` & `sashimi_domains-0.9.3/src/sashimi/corpus/wos.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding: utf-8
-
 # Sashimi - Study of the organisation and evolution of a corpus
 #
 # Author(s):
 # * Ale Abdo <abdo@member.fsf.org>
 #
 # License:
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
@@ -19,15 +17,15 @@
 
 from ..util.wos_lam import WosLam
 
 
 def load_wos_citations(self, user=None, password=None, pmids=None):
     if pmids is None:
         pmids = self.data.pmid
-    fpath = Path(self.data_dir, f"wos_citations{self.data_file_extension}")
+    fpath = Path(self.data_dir, f"wos_citations{self.ext_data}")
     try:
         wos_citations = ioio.load_pandas(fpath)
     except FileNotFoundError:
         wos_citations = pandas.Series()
     new_pmids = pmids[~pmids.isin(wos_citations.index)]
     print(
         "Found {} stored, downloading {} new citation counts".format(
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/graph_models/__init__.py` & `sashimi_domains-0.9.3/src/sashimi/graph_models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding: utf-8
-
 # Sashimi - Study of the organisation and evolution of a corpus
 #
 # Author(s):
 # * Ale Abdo <abdo@member.fsf.org>
 #
 # License:
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
@@ -53,14 +51,17 @@
         self.set_graph(self._to_load.pop("graph", None), strict=False)
         self.set_blockstate(self._to_load.pop("blockstate", None))
         self.loaded["chainedbstates"] = self._to_load.pop("chainedbstates", {})
         if graph_extend := self._to_load.pop("graph_extend", None):
             self.set_chain(**graph_extend, strict=False)
         else:
             self.unset_chain()
+        self.use_cached_annotations = True
+        self.use_cached_annotations_sampled = False
+        self.use_cached_cross_counts = True
 
     ext_g = ".gt.xz"
     ext_nbs = ".json.xz"
 
     graph_name = makep_fromdict("loaded", "graph", True, None, None)
     graph_dir = property_getfuncdir(lambda self: self.data_dir / self.graph_name)
     graph_adir = property_getfuncdir(lambda self: self.data_adir / self.graph_name)
@@ -73,67 +74,60 @@
         lambda self: self.loaded["chainedbstates"].get(self.graph_extend_name, None)
     )
     chained_dir = property_getfuncdir(lambda self: self.blocks_dir / self.chained_name)
     chained_adir = property_getfuncdir(
         lambda self: self.blocks_adir / self.chained_name
     )
 
-    def load_domain_topic_model(self, ltype="link", load=True):
+    def load_domain_topic_model(self, load=True):
         """"""
         self.cache_clear(clear_static=True)
         if not self.column:
             raise ValueError
         if not self.blocks_name or not load:
             if not self.graph_name:
                 create_docter_graph(self)
             self.load_graph()
             calc_nested_blockstate(self)
         self.load_blockstate()
         self.blockstate_to_dataframes()
         self.load_ter_documents()
-        zmethods.load_cross_count_all(self, "ter", "link")
 
-    def load_domain_chained_model(
-        self, ltype="link", load=True, bext="max", anneal=False
-    ):
+    def load_domain_chained_model(self, load=True, bext="max", anneal=False):
         """"""
         self.cache_clear(clear_static=True)
         if not (self.graph_extend and (load or self.blocks_name)):
             raise ValueError
         self.load_blockstate()
         self.blockstate_to_dataframes()
         if not self.chained_name or not load:
             calc_chained_nested_blockstate(self, bext=bext, anneal=anneal)
         self.load_blockstate(chained=True, keep_blocks=True)
         self.blockstate_to_dataframes()
         self.load_ter_documents()
         self.load_ext_documents()
-        zmethods.load_cross_count_all(self, "ter", "link")
-        zmethods.load_cross_count_all(self, "ext", "link")
 
     def trim_to_sample(self):
         self.cache_clear(clear_static=True)
-        self.cached_annotations = False
-        self.cached_cross_count = False
+        self.use_cached_annotations = False
         if not self.tblocks.empty:
             self.load_ter_documents()
             if not hasattr(self, "_orig_tblocks"):
                 self._orig_tblocks = self.tblocks.copy()
             self.tblocks = self._orig_tblocks[
                 self._orig_tblocks.index.isin(self.ter_documents)
             ]
-            zmethods.load_cross_count_all(self, "ter", "link")
         if not self.eblocks.empty:
             self.load_ext_documents()
             if not hasattr(self, "_orig_eblocks"):
                 self._orig_eblocks = self.eblocks.copy()
             self.eblocks = self._orig_eblocks[
                 self._orig_eblocks.index.isin(self.ext_documents)
             ]
-            zmethods.load_cross_count_all(self, "ext", "link")
+        self.gen_mapindex()
 
     ################################################
     # Graph and blockstate methods (TODO move out) #
     ################################################
 
     def from_corpus_to_convoc(self):
         """
@@ -243,15 +237,15 @@
 
     def clear_graph(self):
         clearattrs(self, ["graph"])
 
     def clear_extended(self):
         clearattrs(
             self,
-            ["ext_documents", "values_ext_link_count_all", "values_ext_doc_count_all"],
+            ["ext_documents"],
         )
 
     def unset_chain(self):
         self.loaded["graph_extend"] = None
 
     def set_chain(self, prop, matcher=None, strict=True):
         """
@@ -265,26 +259,33 @@
                 if not (self.resources_dir / matcher).is_file():
                     raise ValueError
         self.loaded["graph_extend"] = {"prop": prop, "matcher": matcher}
 
     # Blockstate
 
     def list_blockstates(self):
-        return [
+        blockstate_list = [
             str(fpath.name)
             for fpath in self.graph_dir.iterdir()
             if fpath.name.startswith("blockstate; ") and fpath.is_dir()
         ]
+        return sorted(blockstate_list)
 
     def list_chainedbstates(self):
-        return [
+        params_string = (
+            f"prop={self.graph_extend['prop']}; matcher={self.graph_extend['matcher']};"
+        )
+        chainedbstates_list = [
             str(fpath.name)
             for fpath in self.blocks_dir.iterdir()
-            if fpath.name.startswith("chainedbstate; ") and fpath.is_dir()
+            if fpath.name.startswith("chainedbstate; ")
+            and fpath.is_dir()
+            and params_string in str(fpath)
         ]
+        return sorted(chainedbstates_list)
 
     def load_blockstate(self, chained=False, keep_blocks=False):
         """
         Loads a previously stored blockstate from a json or pickle file.
 
         The loaded state is found at `self.state`.
 
@@ -410,15 +411,16 @@
                 self.list_chainedbstates() if chained else self.list_blockstates()
             )
         state_ent = {}
         for state in state_list:
             self.set_blockstate(state, chained)
             self.load_blockstate(chained=chained)
             state_ent[state] = self.state.entropy()
-        chosen_state = sorted(state_ent.items(), key=lambda x: x[1])[index][0]
+        state_ent = dict(sorted(state_ent.items(), key=lambda x: x[1]))
+        chosen_state = [*state_ent][index]
         self.set_blockstate(chosen_state, chained)
         self.clear_blockstate()
         if delete_non_best:
             for state in [state for state in state_list if state != chosen_state]:
                 self.delete_blockstate(state)
         return state_ent
 
@@ -493,35 +495,49 @@
             # assign remaining blocks and block_levels
             self.tblocks, self.eblocks = (tblocks, eblocks)
             self.dblocks_levels, self.tblocks_levels, self.eblocks_levels = (
                 [x for x in blocks if isinstance(x, int)]
                 for blocks in (dblocks, tblocks, eblocks)
             )
         self.gen_block_label_correspondence()
+        self.gen_mapindex()
 
     def gen_block_label_correspondence(self):
         self.hblock_to_label = {}
         self.label_to_hblock = {}
-        self.label_to_mapindex = {}
         self.label_to_tlblock = {}
         self.lblock_to_label = {}
-        self.lblock_to_mapindex = {}
         self_dblocks = getattr(self, "_orig_dblocks", self.dblocks)
         for blocks, levels, btype in [
             (self_dblocks, self.dblocks_levels, "doc"),
             (self.tblocks, self.tblocks_levels, "ter"),
             (self.eblocks, self.eblocks_levels, "ext"),
         ]:
-            mapindex = 0
             for level in reversed(levels):
                 for i, hblock in enumerate(
                     sorted_hierarchical_block_index(blocks, levels, level)
                 ):
                     lblock = (level, hblock[-1])
                     label = "L{}{}{}".format(level, btype[0].upper(), i)
                     self.hblock_to_label[hblock] = label
                     self.label_to_hblock[label] = hblock
-                    self.label_to_mapindex[label] = mapindex
                     self.label_to_tlblock[label] = (btype, *lblock)
                     self.lblock_to_label[(level, hblock[-1])] = label
+
+    def gen_mapindex(self):
+        self.label_to_mapindex = {}
+        self.lblock_to_mapindex = {}
+        for blocks, levels, btype in [
+            (self.dblocks, self.dblocks_levels, "doc"),
+            (self.tblocks, self.tblocks_levels, "ter"),
+            (self.eblocks, self.eblocks_levels, "ext"),
+        ]:
+            mapindex = 0
+            for level in reversed(levels):
+                for i, hblock in enumerate(
+                    sorted_hierarchical_block_index(blocks, levels, level)
+                ):
+                    lblock = (level, hblock[-1])
+                    label = self.lblock_to_label[lblock]
+                    self.label_to_mapindex[label] = mapindex
                     self.lblock_to_mapindex[lblock] = mapindex
                     mapindex += 1
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/graph_models/domain_chained_model.py` & `sashimi_domains-0.9.3/src/sashimi/graph_models/domain_chained_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding: utf-8
-
 # Sashimi - Study of the organisation and evolution of a corpus
 #
 # Author(s):
 # * Ale Abdo <abdo@member.fsf.org>
 #
 # License:
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
@@ -27,15 +25,15 @@
 
 def calc_chained_nested_blockstate(corpus, bext="max", niter=10, anneal=False):
     """
     Calculates a chained nested blockstate for vertices derived from
     values of some property of the documents.
     Only works for NestedBlockState without layers or overlapping.
     (corpus)
-    (runs) number of times the optimization procedure is runs
+    (niter) number of times the optimization procedure is run
     (anneal) use annealing for optimization
     :str: file name of stored state
     """
     name_args = []
     if sample := corpus.get_sample_hash(doc=True, ext=True):
         name_args += [("sample", sample)]
 
@@ -53,27 +51,26 @@
         try:
             (corpus.blocks_dir / fname).mkdir(exist_ok=False)
             print(f"Reserved name: {fname}\n")
             break
         except OSError:
             pass
 
-    print("Generating blockstate\n")
+    print("Generating initial block state\n")
     g = gen_doc_graph(corpus)
     extend_graph(corpus, g)
     doc_bs = gen_doc_blocks(corpus)
     pclabel = "type"
     nbstate = gen_chained_nested_blockstate(g, doc_bs, pclabel=pclabel, bext=bext)
 
+    # WARNING: nbstate copies lose hbfields, do not optimize or get entropy on them
+
     print("Starting minimization from initial state:\n", nbstate)
     ent = nbstate.entropy()
-    best_nbstate = (
-        nbstate.copy()
-    )  # WARNING: copies lose hbfields, do not optimize on them
-
+    best_nbstate = nbstate.copy()
     for _ in range(niter):
         if not anneal:
             for i in range(1000):  # this should be sufficiently large
                 nbstate.multiflip_mcmc_sweep(
                     beta=numpy.inf,
                     niter=10,
                     ls=[*range(len(nbstate.levels) - 1)],
@@ -85,14 +82,15 @@
                 niter=1000,
                 mcmc_equilibrate_args=dict(
                     force_niter=10,
                     mcmc_args=dict(ls=[*range(len(nbstate.levels) - 1)]),
                 ),
             )
         if nbstate.entropy() < ent:
+            ent = nbstate.entropy()
             best_nbstate = nbstate.copy()
     nbstate = contiguous_map_nested_blockstate(best_nbstate)
 
     fpath = corpus.blocks_dir / fname / fname
     corpus.store_blockstate(fpath, state=nbstate, pclabel=pclabel)
     print("Saved chained state: {}".format(fname))
     corpus.set_blockstate(str(fname), chained=True)
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/graph_models/domain_topic_model.py` & `sashimi_domains-0.9.3/src/sashimi/graph_models/domain_topic_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding: utf-8
-
 # Sashimi - Study of the organisation and evolution of a corpus
 #
 # Author(s):
 # * Ale Abdo <abdo@member.fsf.org>
 #
 # License:
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
@@ -185,14 +183,15 @@
     corpus.store_blockstate(state=state, **store_blockstate_args)
     print("Saved state: {}".format(fname))
     corpus.loaded["blockstate"] = str(fname)
     return fname
 
 
 def refine_state(state, strategy="sweep"):
+    print("Refining state...")
     if isinstance(strategy, str):
         strategy = [strategy]
     for method in strategy:
         if method == "sweep":
             for i in range(1000):
                 state.multiflip_mcmc_sweep(beta=np.inf, niter=10)
         if method == "anneal":
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/graph_models/util.py` & `sashimi_domains-0.9.3/src/sashimi/graph_models/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding: utf-8
-
 # Sashimi - Study of the organisation and evolution of a corpus
 #
 # Author(s):
 # * Ale Abdo <abdo@member.fsf.org>
 #
 # License:
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
@@ -18,19 +16,19 @@
 # Contributions are welcome, get in touch with the author(s).
 
 
 def contiguous_map_nested_blockstate(ns, io_is_bs=False):
     bs = ns if io_is_bs else ns.get_bs()
     bs = [b.copy() for b in bs]
     for lvl, b in enumerate(bs):
-        m = dict()
+        old_b_to_new_b = dict()
         for i, b_i in enumerate(b):
-            b[i] = m.setdefault(b_i, len(m))
+            b[i] = old_b_to_new_b.setdefault(b_i, len(old_b_to_new_b))
         if lvl + 1 < len(bs):
             up_b = bs[lvl + 1]
-            up_bc = up_b[: len(m)].copy()
-            for i, j in m.items():
-                up_bc[j] = up_b[i]
-            bs[lvl + 1] = up_bc
+            new_up_b = up_b[: len(old_b_to_new_b)].copy()
+            for i, j in old_b_to_new_b.items():
+                new_up_b[j] = up_b[i]
+            bs[lvl + 1] = new_up_b
     while len(bs) > 2 and list(bs[-1]) == list(bs[-2]):
         bs.pop()
     return bs if io_is_bs else ns.copy(bs=bs)
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/util/asco_clean.py` & `sashimi_domains-0.9.3/src/sashimi/util/asco_clean.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.2/src/sashimi/util/pubmed_get.sh` & `sashimi_domains-0.9.3/src/sashimi/util/pubmed_get.sh`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.2/src/sashimi/util/scan_bugtrap.py` & `sashimi_domains-0.9.3/src/sashimi/util/scan_bugtrap.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.2/src/sashimi/util/wos_lam/__init__.py` & `sashimi_domains-0.9.3/src/sashimi/util/wos_lam/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/python3
-# coding: utf-8
-
 # WosLam, a tiny library for the WOS Links Article Match API
 #
 # Author(s):
 # * Ale Abdo <abdo@member.fsf.org>
 #
 # License:
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
```

### Comparing `sashimi_domains-0.9.2/src/sashimi/util/wos_lam/wos_api_request.tpl` & `sashimi_domains-0.9.3/src/sashimi/util/wos_lam/wos_api_request.tpl`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.2/tests/test_basic_usage.py` & `sashimi_domains-0.9.3/tests/test_basic_usage.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,15 +108,14 @@
     corpus.register_config(f"{corpus.data_name}-dtm.json")
     return corpus
 
 
 @cache
 def example_corpus_dcm():
     corpus = example_corpus_dtm()
-    assert hasattr(corpus, "values_ter_link_count_all")
     corpus.set_chain("meta")
     corpus.load_domain_chained_model()
     corpus.state.entropy()
     corpus.register_config(f"{corpus.data_name}-dcm.json")
     return corpus
 
 
@@ -125,24 +124,30 @@
     data = corpus.load_from_store(corpus.loaded["data"], return_not_load=True)
     return corpus.data.compare(data)
 
 
 def test_corpus_dtm_maps():
     corpus = example_corpus_dtm()
     dm = corpus.domain_map()
-    dn = corpus.domain_network(doc_level=1)
-    return dm, dn
+    dns = corpus.domain_network(doc_level=1, edges="specific")
+    dnc = None
+    if 2 in corpus.dblocks_levels:
+        dnc = corpus.domain_network(doc_level=2, edges="common")
+    return dm, dns, dnc
 
 
 def test_corpus_dcm_maps():
     corpus = example_corpus_dcm()
     dm = corpus.domain_map()
     dm = corpus.domain_map(chained=True)
-    dn = corpus.domain_network(doc_level=1, ext_level=1)
-    return dm, dn
+    dns = corpus.domain_network(doc_level=1, ext_level=1, edges="specific")
+    dnc = None
+    if 2 in corpus.dblocks_levels:
+        dnc = corpus.domain_network(doc_level=2, ext_level=1, edges="common")
+    return dm, dns, dnc
 
 
 def load_test_corpus(name):
     return sashimi.GraphModels(name)
 
 
 def cache_clear():
```

### Comparing `sashimi_domains-0.9.2/tests/test_pclabel_bfield.py` & `sashimi_domains-0.9.3/tests/test_pclabel_bfield.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.2/LICENSE` & `sashimi_domains-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.2/README.md` & `sashimi_domains-0.9.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Model-based data interfaces (visualisations):
 - Interactive domain-topic maps and domain-chained maps
 - Domain-topic tables and domain-chained tables
 - Domain-topic, domain-chained and domain-topic-chained networks
 - Area rank charts (bump charts) of the evolution of domain sizes
 
-<img alt="Domain-topic network" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2022-11-19-17-42-28.png" width="50%"><img alt="Domain-topic map" src="https://docs.cortext.net/wp-content/uploads/dtm-example-chloroquine.png" width="50%">
+<img alt="Domain-topic network" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2022-11-19-17-42-28.png" width="50%"><img alt="Domain-topic map" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2023-06-28-10-56-41.png" width="50%">
 
 ## Using Sashimi without programming (no code)
 
 Sashimi is available as a suite of methods in the [Cortext Manager](https://docs.cortext.net/) web service. See [SASHIMI](https://docs.cortext.net/sashimi/).
 
 ## Savoring Sashimi
 Also for users of this library, the [documentation](https://docs.cortext.net/sashimi/) at Cortext serves as a good introduction to the methodology.
@@ -35,17 +35,17 @@
 ### Dependencies
 
 This project builds mainly on the following others:
 - [graph-tool](graph-tool.skewed.de/) (for Stochastic Block Model inference)
 - [pandas](https://pandas.pydata.org/)
 - [spacy](https://spacy.io/) (for tokenization)
 - [gensim](https://radimrehurek.com/gensim/) (for ngram detection)
-- [bokeh](https://bokeh.org/) (for hierarchical block maps and other plots)
-- [lxml](https://lxml.de/) (for domain tables)
-- [matplotlib](https://matplotlib.org/) (for simple corpus statistics)
+- [bokeh](https://bokeh.org/) (for building hierarchical block maps and other plots)
+- [lxml](https://lxml.de/) (for building domain tables)
+- [matplotlib](https://matplotlib.org/) (for plotting simple corpus statistics)
 
 With the exception of graph-tool, they'll be automatically handled by `pip`.
 
 ## Basic usage
 
 ```python
 from sashimi import GraphModels
@@ -107,16 +107,21 @@
 print(corpus.dblocks)
 print(corpus.tblocks)
 
 # Create an interactive hierarchical map
 # Output is a self-contained html+css+js+data document
 corpus.domain_map()
 
-# Create network representation for the first domain and topic levels, as pdf and graphml documents
+# Create network representations for the first domain and topic levels, as pdf, svg and graphml documents
 corpus.domain_network(doc_level=1, ter_level=1)
+corpus.domain_network(doc_level=2, ter_level=1)
+# The default representation shows edges from a domain to its "specific" topics, with the previous call being equivalent to the following
+corpus.domain_network(doc_level=2, ter_level=1, edges="specific")
+# For domains of level higher than 1, setting `edges="common"` will show edges towards topics that are common to all of its subdomains
+corpus.domain_network(doc_level=2, ter_level=1, edges="common")
 
 # Create domain-topic tables for all domains at level 3
 if 3 in corpus.dblocks:
     corpus.subxblocks_tables(xbtype="doc", xlevel=3, xb=None, ybtype="ter")
 
 # Store the current choices of corpus and model
 corpus.register_config("my_config.json")
@@ -133,19 +138,22 @@
 corpus.load_domain_chained_model()
 print(corpus.list_chainedbstates())
 
 # Create interactive instruments for the chained dimension
 corpus.domain_map(chained=True)
 corpus.domain_network(doc_level=1, ter_level=None, ext_level=1)
 corpus.domain_network(doc_level=1, ter_level=1, ext_level=1)
+# The `edges` parameter applies to both topics and the chained dimension
+corpus.domain_network(doc_level=2, ter_level=None, ext_level=1, edges="specific")
+corpus.domain_network(doc_level=2, ter_level=1, ext_level=1, edges="common")
 if 3 in corpus.dblocks:
     corpus.subxblocks_tables(xbtype="doc", xlevel=3, xb=None, ybtype="ext")
 ```
 
-<img alt="Domain-chained map" src="https://docs.cortext.net/wp-content/uploads/dcm-example-journals-chloroquine-.png" width="50%"><img alt="Domain-topic-chained network" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2022-11-19-17-45-15.png" width="50%">
+<img alt="Domain-chained map" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2023-06-28-11-02-16.png" width="50%"><img alt="Domain-topic-chained network" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2022-11-19-17-45-15.png" width="50%">
 
 ## Advanced usages
 
 - The domain map document provides a "Help" tab explaining how to navigate and read it, which is also useful to understand the other interfaces.
 
 - Create filtered visualisations to show only a selected group of domains in maps and networks.
```

### Comparing `sashimi_domains-0.9.2/pyproject.toml` & `sashimi_domains-0.9.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -31,17 +31,17 @@
   "scipy",
   "spacy",
   "tqdm",
 ]
 dynamic = ["version"]
 
 [project.urls]
-Documentation = "https://gitlab.com/solstag/abstractology/"
-Issues = "https://gitlab.com/solstag/abstractology/-/issues"
-Source = "https://gitlab.com/solstag/abstractology/"
+Documentation = "https://gitlab.com/solstag/sashimi/"
+Issues = "https://gitlab.com/solstag/sashimi/-/issues"
+Source = "https://gitlab.com/solstag/sashimi/"
 
 [tool.hatch.version]
 path = "src/sashimi/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 [tool.hatch.build.targets.wheel]
 packages = ["src/sashimi"]
```

### Comparing `sashimi_domains-0.9.2/PKG-INFO` & `sashimi_domains-0.9.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: sashimi-domains
-Version: 0.9.2
+Version: 0.9.3
 Summary: Sashimi is a Python module that provides tailored mathematical models and corresponding interactive visualisations for exploratory and confirmatory mixed-methods analysis of large textual or token corpora. It can detect textual and metadata structures and shifts, by employing stochastic block modeling (SBM) from graph-tool or [currently deprecated] word embedding from Gensim.
-Project-URL: Documentation, https://gitlab.com/solstag/abstractology/
-Project-URL: Issues, https://gitlab.com/solstag/abstractology/-/issues
-Project-URL: Source, https://gitlab.com/solstag/abstractology/
+Project-URL: Documentation, https://gitlab.com/solstag/sashimi/
+Project-URL: Issues, https://gitlab.com/solstag/sashimi/-/issues
+Project-URL: Source, https://gitlab.com/solstag/sashimi/
 Author-email: Ale Abdo <abdo@member.fsf.org>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -39,15 +39,15 @@
 
 Model-based data interfaces (visualisations):
 - Interactive domain-topic maps and domain-chained maps
 - Domain-topic tables and domain-chained tables
 - Domain-topic, domain-chained and domain-topic-chained networks
 - Area rank charts (bump charts) of the evolution of domain sizes
 
-<img alt="Domain-topic network" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2022-11-19-17-42-28.png" width="50%"><img alt="Domain-topic map" src="https://docs.cortext.net/wp-content/uploads/dtm-example-chloroquine.png" width="50%">
+<img alt="Domain-topic network" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2022-11-19-17-42-28.png" width="50%"><img alt="Domain-topic map" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2023-06-28-10-56-41.png" width="50%">
 
 ## Using Sashimi without programming (no code)
 
 Sashimi is available as a suite of methods in the [Cortext Manager](https://docs.cortext.net/) web service. See [SASHIMI](https://docs.cortext.net/sashimi/).
 
 ## Savoring Sashimi
 Also for users of this library, the [documentation](https://docs.cortext.net/sashimi/) at Cortext serves as a good introduction to the methodology.
@@ -63,17 +63,17 @@
 ### Dependencies
 
 This project builds mainly on the following others:
 - [graph-tool](graph-tool.skewed.de/) (for Stochastic Block Model inference)
 - [pandas](https://pandas.pydata.org/)
 - [spacy](https://spacy.io/) (for tokenization)
 - [gensim](https://radimrehurek.com/gensim/) (for ngram detection)
-- [bokeh](https://bokeh.org/) (for hierarchical block maps and other plots)
-- [lxml](https://lxml.de/) (for domain tables)
-- [matplotlib](https://matplotlib.org/) (for simple corpus statistics)
+- [bokeh](https://bokeh.org/) (for building hierarchical block maps and other plots)
+- [lxml](https://lxml.de/) (for building domain tables)
+- [matplotlib](https://matplotlib.org/) (for plotting simple corpus statistics)
 
 With the exception of graph-tool, they'll be automatically handled by `pip`.
 
 ## Basic usage
 
 ```python
 from sashimi import GraphModels
@@ -135,16 +135,21 @@
 print(corpus.dblocks)
 print(corpus.tblocks)
 
 # Create an interactive hierarchical map
 # Output is a self-contained html+css+js+data document
 corpus.domain_map()
 
-# Create network representation for the first domain and topic levels, as pdf and graphml documents
+# Create network representations for the first domain and topic levels, as pdf, svg and graphml documents
 corpus.domain_network(doc_level=1, ter_level=1)
+corpus.domain_network(doc_level=2, ter_level=1)
+# The default representation shows edges from a domain to its "specific" topics, with the previous call being equivalent to the following
+corpus.domain_network(doc_level=2, ter_level=1, edges="specific")
+# For domains of level higher than 1, setting `edges="common"` will show edges towards topics that are common to all of its subdomains
+corpus.domain_network(doc_level=2, ter_level=1, edges="common")
 
 # Create domain-topic tables for all domains at level 3
 if 3 in corpus.dblocks:
     corpus.subxblocks_tables(xbtype="doc", xlevel=3, xb=None, ybtype="ter")
 
 # Store the current choices of corpus and model
 corpus.register_config("my_config.json")
@@ -161,19 +166,22 @@
 corpus.load_domain_chained_model()
 print(corpus.list_chainedbstates())
 
 # Create interactive instruments for the chained dimension
 corpus.domain_map(chained=True)
 corpus.domain_network(doc_level=1, ter_level=None, ext_level=1)
 corpus.domain_network(doc_level=1, ter_level=1, ext_level=1)
+# The `edges` parameter applies to both topics and the chained dimension
+corpus.domain_network(doc_level=2, ter_level=None, ext_level=1, edges="specific")
+corpus.domain_network(doc_level=2, ter_level=1, ext_level=1, edges="common")
 if 3 in corpus.dblocks:
     corpus.subxblocks_tables(xbtype="doc", xlevel=3, xb=None, ybtype="ext")
 ```
 
-<img alt="Domain-chained map" src="https://docs.cortext.net/wp-content/uploads/dcm-example-journals-chloroquine-.png" width="50%"><img alt="Domain-topic-chained network" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2022-11-19-17-45-15.png" width="50%">
+<img alt="Domain-chained map" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2023-06-28-11-02-16.png" width="50%"><img alt="Domain-topic-chained network" src="https://docs.cortext.net/wp-content/uploads/Screenshot-from-2022-11-19-17-45-15.png" width="50%">
 
 ## Advanced usages
 
 - The domain map document provides a "Help" tab explaining how to navigate and read it, which is also useful to understand the other interfaces.
 
 - Create filtered visualisations to show only a selected group of domains in maps and networks.
```

