# Comparing `tmp/id_translation-0.5.0.tar.gz` & `tmp/id_translation-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "id_translation-0.5.0.tar", max compression
+gzip compressed data, was "id_translation-0.5.1.tar", max compression
```

## Comparing `id_translation-0.5.0.tar` & `id_translation-0.5.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1077 2023-06-29 19:58:15.847356 id_translation-0.5.0/LICENSE.md
--rw-r--r--   0        0        0     5488 2023-06-29 19:58:15.847356 id_translation-0.5.0/README.md
--rw-r--r--   0        0        0     5642 2023-06-29 19:58:15.855356 id_translation-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      962 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/__init__.py
--rw-r--r--   0        0        0      203 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/__version__.py
--rw-r--r--   0        0        0     4652 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/_base_metadata.py
--rw-r--r--   0        0        0     4208 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/_config_utils.py
--rw-r--r--   0        0        0     1467 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/_load_toml.py
--rw-r--r--   0        0        0    50044 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/_translator.py
--rw-r--r--   0        0        0      947 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/_uuid_utils.py
--rw-r--r--   0        0        0      235 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/dio/__init__.py
--rw-r--r--   0        0        0     2036 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/dio/_data_structure_io.py
--rw-r--r--   0        0        0     1346 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/dio/_dict.py
--rw-r--r--   0        0        0     4141 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/dio/_pandas.py
--rw-r--r--   0        0        0      771 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/dio/_resolve.py
--rw-r--r--   0        0        0     2572 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/dio/_sequence.py
--rw-r--r--   0        0        0     1094 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/dio/_set.py
--rw-r--r--   0        0        0     1022 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/dio/_single_value.py
--rw-r--r--   0        0        0      760 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/dio/exceptions.py
--rw-r--r--   0        0        0      898 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/exceptions.py
--rw-r--r--   0        0        0    11744 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/factory.py
--rw-r--r--   0        0        0     1264 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/fetching/__init__.py
--rw-r--r--   0        0        0    23102 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/fetching/_abstract_fetcher.py
--rw-r--r--   0        0        0     7573 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/fetching/_cache.py
--rw-r--r--   0        0        0     3249 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/fetching/_fetcher.py
--rw-r--r--   0        0        0     1441 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/fetching/_memory_fetcher.py
--rw-r--r--   0        0        0    13706 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/fetching/_multi_fetcher.py
--rw-r--r--   0        0        0     5431 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/fetching/_pandas_fetcher.py
--rw-r--r--   0        0        0    17244 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/fetching/_sql_fetcher.py
--rw-r--r--   0        0        0     2165 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/fetching/exceptions.py
--rw-r--r--   0        0        0     1154 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/fetching/types.py
--rw-r--r--   0        0        0      601 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/mapping/__init__.py
--rw-r--r--   0        0        0     5710 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/mapping/_cardinality.py
--rw-r--r--   0        0        0     8043 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/mapping/_directional_mapping.py
--rw-r--r--   0        0        0     8004 2023-06-29 19:58:15.855356 id_translation-0.5.0/src/id_translation/mapping/_heuristic_score.py
--rw-r--r--   0        0        0    21999 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/mapping/_mapper.py
--rw-r--r--   0        0        0     2371 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/mapping/exceptions.py
--rw-r--r--   0        0        0     6171 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/mapping/filter_functions.py
--rw-r--r--   0        0        0     6250 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/mapping/heuristic_functions.py
--rw-r--r--   0        0        0     3051 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/mapping/score_functions.py
--rw-r--r--   0        0        0    13582 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/mapping/support.py
--rw-r--r--   0        0        0     2854 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/mapping/types.py
--rw-r--r--   0        0        0      287 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/offline/__init__.py
--rw-r--r--   0        0        0     5323 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/offline/_format.py
--rw-r--r--   0        0        0     3723 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/offline/_format_applier.py
--rw-r--r--   0        0        0     2628 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/offline/_magic_dict.py
--rw-r--r--   0        0        0     7603 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/offline/_translation_map.py
--rw-r--r--   0        0        0     6114 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/offline/parse_format_string.py
--rw-r--r--   0        0        0     3276 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/offline/types.py
--rw-r--r--   0        0        0        0 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/py.typed
--rw-r--r--   0        0        0     3362 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/testing.py
--rw-r--r--   0        0        0     2741 2023-06-29 19:58:15.859356 id_translation-0.5.0/src/id_translation/types.py
--rw-r--r--   0        0        0     6884 1970-01-01 00:00:00.000000 id_translation-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-01 08:54:13.109397 id_translation-0.5.1/LICENSE.md
+-rw-r--r--   0        0        0     5488 2023-07-01 08:54:13.109397 id_translation-0.5.1/README.md
+-rw-r--r--   0        0        0     5642 2023-07-01 08:54:13.117397 id_translation-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      962 2023-07-01 08:54:13.117397 id_translation-0.5.1/src/id_translation/__init__.py
+-rw-r--r--   0        0        0      203 2023-07-01 08:54:13.117397 id_translation-0.5.1/src/id_translation/__version__.py
+-rw-r--r--   0        0        0     4652 2023-07-01 08:54:13.117397 id_translation-0.5.1/src/id_translation/_base_metadata.py
+-rw-r--r--   0        0        0     4208 2023-07-01 08:54:13.117397 id_translation-0.5.1/src/id_translation/_config_utils.py
+-rw-r--r--   0        0        0     1467 2023-07-01 08:54:13.117397 id_translation-0.5.1/src/id_translation/_load_toml.py
+-rw-r--r--   0        0        0    50044 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/_translator.py
+-rw-r--r--   0        0        0      947 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/_uuid_utils.py
+-rw-r--r--   0        0        0      235 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/dio/__init__.py
+-rw-r--r--   0        0        0     2036 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/dio/_data_structure_io.py
+-rw-r--r--   0        0        0     1346 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/dio/_dict.py
+-rw-r--r--   0        0        0     4141 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/dio/_pandas.py
+-rw-r--r--   0        0        0      771 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/dio/_resolve.py
+-rw-r--r--   0        0        0     2572 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/dio/_sequence.py
+-rw-r--r--   0        0        0     1094 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/dio/_set.py
+-rw-r--r--   0        0        0     1022 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/dio/_single_value.py
+-rw-r--r--   0        0        0      760 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/dio/exceptions.py
+-rw-r--r--   0        0        0      898 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/exceptions.py
+-rw-r--r--   0        0        0    11744 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/factory.py
+-rw-r--r--   0        0        0     1264 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/fetching/__init__.py
+-rw-r--r--   0        0        0    23102 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/fetching/_abstract_fetcher.py
+-rw-r--r--   0        0        0     7573 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/fetching/_cache.py
+-rw-r--r--   0        0        0     3249 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/fetching/_fetcher.py
+-rw-r--r--   0        0        0     1441 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/fetching/_memory_fetcher.py
+-rw-r--r--   0        0        0    14412 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/fetching/_multi_fetcher.py
+-rw-r--r--   0        0        0     5431 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/fetching/_pandas_fetcher.py
+-rw-r--r--   0        0        0    17348 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/fetching/_sql_fetcher.py
+-rw-r--r--   0        0        0     2165 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/fetching/exceptions.py
+-rw-r--r--   0        0        0     1154 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/fetching/types.py
+-rw-r--r--   0        0        0      601 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/mapping/__init__.py
+-rw-r--r--   0        0        0     5710 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/mapping/_cardinality.py
+-rw-r--r--   0        0        0     8043 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/mapping/_directional_mapping.py
+-rw-r--r--   0        0        0     8004 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/mapping/_heuristic_score.py
+-rw-r--r--   0        0        0    21999 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/mapping/_mapper.py
+-rw-r--r--   0        0        0     2371 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/mapping/exceptions.py
+-rw-r--r--   0        0        0     6171 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/mapping/filter_functions.py
+-rw-r--r--   0        0        0     6250 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/mapping/heuristic_functions.py
+-rw-r--r--   0        0        0     3051 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/mapping/score_functions.py
+-rw-r--r--   0        0        0    13582 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/mapping/support.py
+-rw-r--r--   0        0        0     2854 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/mapping/types.py
+-rw-r--r--   0        0        0      287 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/offline/__init__.py
+-rw-r--r--   0        0        0     5323 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/offline/_format.py
+-rw-r--r--   0        0        0     3723 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/offline/_format_applier.py
+-rw-r--r--   0        0        0     2628 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/offline/_magic_dict.py
+-rw-r--r--   0        0        0     7603 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/offline/_translation_map.py
+-rw-r--r--   0        0        0     6114 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/offline/parse_format_string.py
+-rw-r--r--   0        0        0     3276 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/offline/types.py
+-rw-r--r--   0        0        0        0 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/py.typed
+-rw-r--r--   0        0        0     3362 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/testing.py
+-rw-r--r--   0        0        0     2741 2023-07-01 08:54:13.121397 id_translation-0.5.1/src/id_translation/types.py
+-rw-r--r--   0        0        0     6884 1970-01-01 00:00:00.000000 id_translation-0.5.1/PKG-INFO
```

### Comparing `id_translation-0.5.0/LICENSE.md` & `id_translation-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/README.md` & `id_translation-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/pyproject.toml` & `id_translation-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "id-translation"
-version = "0.5.0"
+version = "0.5.1"
 description = "Convert IDs into human-readable labels."
 authors = ["Richard Sundqvist <richard.sundqvist@live.se>"]
 
 readme = "README.md"
 homepage = "https://github.com/rsundqvist/id-translation"
 repository = "https://github.com/rsundqvist/id-translation"
 documentation = "https://id-translation.readthedocs.io"
```

### Comparing `id_translation-0.5.0/src/id_translation/__init__.py` & `id_translation-0.5.1/src/id_translation/__init__.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/_base_metadata.py` & `id_translation-0.5.1/src/id_translation/_base_metadata.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/_config_utils.py` & `id_translation-0.5.1/src/id_translation/_config_utils.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/_load_toml.py` & `id_translation-0.5.1/src/id_translation/_load_toml.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/_translator.py` & `id_translation-0.5.1/src/id_translation/_translator.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/_uuid_utils.py` & `id_translation-0.5.1/src/id_translation/_uuid_utils.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/dio/_data_structure_io.py` & `id_translation-0.5.1/src/id_translation/dio/_data_structure_io.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/dio/_dict.py` & `id_translation-0.5.1/src/id_translation/dio/_dict.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/dio/_pandas.py` & `id_translation-0.5.1/src/id_translation/dio/_pandas.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/dio/_resolve.py` & `id_translation-0.5.1/src/id_translation/dio/_resolve.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/dio/_sequence.py` & `id_translation-0.5.1/src/id_translation/dio/_sequence.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/dio/_set.py` & `id_translation-0.5.1/src/id_translation/dio/_set.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/dio/_single_value.py` & `id_translation-0.5.1/src/id_translation/dio/_single_value.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/dio/exceptions.py` & `id_translation-0.5.1/src/id_translation/dio/exceptions.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/exceptions.py` & `id_translation-0.5.1/src/id_translation/exceptions.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/factory.py` & `id_translation-0.5.1/src/id_translation/factory.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/fetching/__init__.py` & `id_translation-0.5.1/src/id_translation/fetching/__init__.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/fetching/_abstract_fetcher.py` & `id_translation-0.5.1/src/id_translation/fetching/_abstract_fetcher.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/fetching/_cache.py` & `id_translation-0.5.1/src/id_translation/fetching/_cache.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/fetching/_fetcher.py` & `id_translation-0.5.1/src/id_translation/fetching/_fetcher.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/fetching/_memory_fetcher.py` & `id_translation-0.5.1/src/id_translation/fetching/_memory_fetcher.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/fetching/_multi_fetcher.py` & `id_translation-0.5.1/src/id_translation/fetching/_multi_fetcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import logging
 import warnings
 from concurrent.futures import Future, ThreadPoolExecutor, as_completed
 from time import perf_counter
-from typing import Dict, Iterable, List, Tuple
+from typing import Dict, Iterable, List, Tuple, Union
 
 from rics.action_level import ActionLevel, ActionLevelHelper
 from rics.collections.dicts import reverse_dict
 from rics.misc import tname
 from rics.performance import format_seconds
 
 from ..offline.types import SourcePlaceholderTranslations
@@ -32,22 +32,24 @@
     Args:
         *fetchers: Fetchers to wrap.
         max_workers: Number of threads to use for fetching. Fetch instructions will be dispatched using a
              :py:class:`~concurrent.futures.ThreadPoolExecutor`. Individual fetchers will be called at most once per
              ``fetch()`` or ``fetch_all()`` call made with the ``MultiFetcher``.
         duplicate_translation_action: Action to take when multiple fetchers return translations for the same source.
         duplicate_source_discovered_action: Action to take when multiple fetchers claim the same source.
+        optional_fetcher_discarded_log_level: If ``True``, log a warning
     """
 
     def __init__(
         self,
         *fetchers: Fetcher[SourceType, IdType],
         max_workers: int = 1,
         duplicate_translation_action: ActionLevel.ParseType = ActionLevel.WARN,
         duplicate_source_discovered_action: ActionLevel.ParseType = ActionLevel.WARN,
+        optional_fetcher_discarded_log_level: Union[int, str] = "DEBUG",
     ) -> None:
         for pos, f in enumerate(fetchers):
             if not isinstance(f, Fetcher):  # pragma: no cover
                 raise TypeError(f"Argument {pos} is of type {type(f)}, expected Fetcher subtype.")
 
         self._id_to_rank: Dict[int, int] = {id(f): rank for rank, f in enumerate(fetchers)}
         self._id_to_fetcher: Dict[int, Fetcher[SourceType, IdType]] = {id(f): f for f in fetchers}
@@ -55,14 +57,22 @@
         self.max_workers: int = max_workers
         self._duplicate_translation_action = _ACTION_LEVEL_HELPER.verify(
             duplicate_translation_action, "duplicate_translation_action"
         )
         self._duplicate_source_discovered_action = _ACTION_LEVEL_HELPER.verify(
             duplicate_source_discovered_action, "duplicate_source_discovered_action"
         )
+        if isinstance(optional_fetcher_discarded_log_level, str):
+            as_int = logging.getLevelName(optional_fetcher_discarded_log_level.upper())
+            if not isinstance(as_int, int):
+                raise ValueError(
+                    f"Bad {optional_fetcher_discarded_log_level=}. Use an integer or a valid log level name."
+                )
+            optional_fetcher_discarded_log_level = as_int
+        self._optional_discard_level = optional_fetcher_discarded_log_level
 
         if len(self.fetchers) != len(fetchers):
             raise ValueError("Repeat fetcher instance(s)!")  # pragma: no cover
 
     @property
     def allow_fetch_all(self) -> bool:
         return all(f.allow_fetch_all for f in self._id_to_fetcher.values())  # pragma: no cover
@@ -223,22 +233,23 @@
                     except Exception as e:  # noqa: B902
                         sources = None
                         exception_info = f"{type(e).__name__}: {e}"
                 else:
                     sources = fetcher.sources
 
                 if not sources:
+                    fetcher.close()
                     if sources is None:
-                        LOGGER.warning(
+                        LOGGER.log(
+                            self._optional_discard_level,
                             f"Discarding optional {self._fmt_fetcher(fetcher)}: "
-                            f"Raised {exception_info!r} when getting sources."
+                            f"Raised\n    {exception_info}\nwhen getting sources.",
                         )
                     else:
                         LOGGER.warning(f"Discarding {self._fmt_fetcher(fetcher)}: No sources.")
-                    fetcher.close()
                     del self._id_to_rank[fid]
                     del self._id_to_fetcher[fid]
                     continue
 
                 rank = self._id_to_rank[fid]
                 for source in sources:
                     if source in source_to_fetcher_id:
```

### Comparing `id_translation-0.5.0/src/id_translation/fetching/_pandas_fetcher.py` & `id_translation-0.5.1/src/id_translation/fetching/_pandas_fetcher.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/fetching/_sql_fetcher.py` & `id_translation-0.5.1/src/id_translation/fetching/_sql_fetcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,19 @@
     @property
     def allow_fetch_all(self) -> bool:
         return super().allow_fetch_all and all(s.fetch_all_permitted for s in self._summaries.values())
 
     def __str__(self) -> str:
         disconnected = "<disconnected>: " if not self.online else ""
         schema = f"[schema={self._schema!r}]" if self._schema else ""
-        return f"{tname(self)}({disconnected}{self._estr}, tables{schema}={repr(self.sources or '<no tables>')})"
+        try:
+            sources = self.sources
+        except Exception:  # noqa: B902
+            sources = None
+        return f"{tname(self)}({disconnected}{self._estr}, tables{schema}={sources or '<no tables>'})"
 
     @property
     def engine(self) -> sqlalchemy.engine.Engine:
         """Engine used by this fetcher.
 
         Returns:
             The ``Engine`` used for fetching.
```

### Comparing `id_translation-0.5.0/src/id_translation/fetching/exceptions.py` & `id_translation-0.5.1/src/id_translation/fetching/exceptions.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/fetching/types.py` & `id_translation-0.5.1/src/id_translation/fetching/types.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/mapping/__init__.py` & `id_translation-0.5.1/src/id_translation/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/mapping/_cardinality.py` & `id_translation-0.5.1/src/id_translation/mapping/_cardinality.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/mapping/_directional_mapping.py` & `id_translation-0.5.1/src/id_translation/mapping/_directional_mapping.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/mapping/_heuristic_score.py` & `id_translation-0.5.1/src/id_translation/mapping/_heuristic_score.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/mapping/_mapper.py` & `id_translation-0.5.1/src/id_translation/mapping/_mapper.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/mapping/exceptions.py` & `id_translation-0.5.1/src/id_translation/mapping/exceptions.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/mapping/filter_functions.py` & `id_translation-0.5.1/src/id_translation/mapping/filter_functions.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/mapping/heuristic_functions.py` & `id_translation-0.5.1/src/id_translation/mapping/heuristic_functions.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/mapping/score_functions.py` & `id_translation-0.5.1/src/id_translation/mapping/score_functions.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/mapping/support.py` & `id_translation-0.5.1/src/id_translation/mapping/support.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/mapping/types.py` & `id_translation-0.5.1/src/id_translation/mapping/types.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/offline/_format.py` & `id_translation-0.5.1/src/id_translation/offline/_format.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/offline/_format_applier.py` & `id_translation-0.5.1/src/id_translation/offline/_format_applier.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/offline/_magic_dict.py` & `id_translation-0.5.1/src/id_translation/offline/_magic_dict.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/offline/_translation_map.py` & `id_translation-0.5.1/src/id_translation/offline/_translation_map.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/offline/parse_format_string.py` & `id_translation-0.5.1/src/id_translation/offline/parse_format_string.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/offline/types.py` & `id_translation-0.5.1/src/id_translation/offline/types.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/testing.py` & `id_translation-0.5.1/src/id_translation/testing.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/src/id_translation/types.py` & `id_translation-0.5.1/src/id_translation/types.py`

 * *Files identical despite different names*

### Comparing `id_translation-0.5.0/PKG-INFO` & `id_translation-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: id-translation
-Version: 0.5.0
+Version: 0.5.1
 Summary: Convert IDs into human-readable labels.
 Home-page: https://github.com/rsundqvist/id-translation
 Keywords: id-translation
 Author: Richard Sundqvist
 Author-email: richard.sundqvist@live.se
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 4 - Beta
```

