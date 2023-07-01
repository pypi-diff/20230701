# Comparing `tmp/heimdallm-0.1.1.tar.gz` & `tmp/heimdallm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heimdallm-0.1.1.tar", max compression
+gzip compressed data, was "heimdallm-0.1.2.tar", max compression
```

## Comparing `heimdallm-0.1.1.tar` & `heimdallm-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      750 2023-07-01 07:36:38.986297 heimdallm-0.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    34523 2023-07-01 07:36:38.986297 heimdallm-0.1.1/LICENSE
--rw-r--r--   0        0        0     6452 2023-07-01 07:36:38.986297 heimdallm-0.1.1/README.md
--rw-r--r--   0        0        0       81 2023-07-01 07:36:38.990296 heimdallm-0.1.1/heimdallm/__init__.py
--rw-r--r--   0        0        0     6301 2023-07-01 07:36:38.990296 heimdallm-0.1.1/heimdallm/bifrost.py
--rw-r--r--   0        0        0        0 2023-07-01 07:36:38.990296 heimdallm-0.1.1/heimdallm/bifrosts/sql/__init__.py
--rw-r--r--   0        0        0     4341 2023-07-01 07:36:38.990296 heimdallm-0.1.1/heimdallm/bifrosts/sql/exc.py
--rw-r--r--   0        0        0        0 2023-07-01 07:36:38.990296 heimdallm-0.1.1/heimdallm/bifrosts/sql/mysql/__init__.py
--rw-r--r--   0        0        0     3441 2023-07-01 07:36:38.990296 heimdallm-0.1.1/heimdallm/bifrosts/sql/mysql/presets.py
--rw-r--r--   0        0        0        0 2023-07-01 07:36:38.990296 heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/__init__.py
--rw-r--r--   0        0        0     3707 2023-07-01 07:36:38.990296 heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/presets.py
--rw-r--r--   0        0        0        0 2023-07-01 07:36:38.990296 heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/select/__init__.py
--rw-r--r--   0        0        0     4539 2023-07-01 07:36:38.990296 heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/select/bifrost.py
--rw-r--r--   0        0        0     4740 2023-07-01 07:36:38.990296 heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/select/envelope.py
--rw-r--r--   0        0        0     1331 2023-07-01 07:36:38.990296 heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/select/envelopes/base.j2
--rw-r--r--   0        0        0     4756 2023-07-01 07:36:38.990296 heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/select/reconstruct.py
--rw-r--r--   0        0        0     6704 2023-07-01 07:36:38.990296 heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/select/sqlite.lark
--rw-r--r--   0        0        0     8817 2023-07-01 07:36:38.990296 heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/select/validator.py
--rw-r--r--   0        0        0    16115 2023-07-01 07:36:38.990296 heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/select/visitors.py
--rw-r--r--   0        0        0        0 2023-07-01 07:36:38.990296 heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/utils/__init__.py
--rw-r--r--   0        0        0      993 2023-07-01 07:36:38.990296 heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/utils/identifier.py
--rw-r--r--   0        0        0     2716 2023-07-01 07:36:38.994297 heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/utils/visitors.py
--rw-r--r--   0        0        0     4369 2023-07-01 07:36:38.994297 heimdallm-0.1.1/heimdallm/bifrosts/sql/utils.py
--rw-r--r--   0        0        0      711 2023-07-01 07:36:38.994297 heimdallm-0.1.1/heimdallm/constraints.py
--rw-r--r--   0        0        0     1854 2023-07-01 07:36:38.994297 heimdallm-0.1.1/heimdallm/envelope.py
--rw-r--r--   0        0        0      156 2023-07-01 07:36:38.994297 heimdallm-0.1.1/heimdallm/llm.py
--rw-r--r--   0        0        0        0 2023-07-01 07:36:38.994297 heimdallm-0.1.1/heimdallm/llm_providers/__init__.py
--rw-r--r--   0        0        0      753 2023-07-01 07:36:38.994297 heimdallm-0.1.1/heimdallm/llm_providers/mock.py
--rw-r--r--   0        0        0     2388 2023-07-01 07:36:38.994297 heimdallm-0.1.1/heimdallm/llm_providers/openai.py
--rw-r--r--   0        0        0        0 2023-07-01 07:36:38.994297 heimdallm-0.1.1/heimdallm/support/__init__.py
--rw-r--r--   0        0        0     1182 2023-07-01 07:36:38.994297 heimdallm-0.1.1/heimdallm/support/github.py
--rw-r--r--   0        0        0     1547 2023-07-01 07:36:39.026298 heimdallm-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7762 1970-01-01 00:00:00.000000 heimdallm-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      750 2023-07-01 13:58:32.237701 heimdallm-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0    34523 2023-07-01 13:58:32.237701 heimdallm-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6498 2023-07-01 13:58:32.237701 heimdallm-0.1.2/README.md
+-rw-r--r--   0        0        0       81 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/__init__.py
+-rw-r--r--   0        0        0     6301 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrost.py
+-rw-r--r--   0        0        0        0 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/__init__.py
+-rw-r--r--   0        0        0     4341 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/exc.py
+-rw-r--r--   0        0        0        0 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/mysql/__init__.py
+-rw-r--r--   0        0        0     3441 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/mysql/presets.py
+-rw-r--r--   0        0        0        0 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/__init__.py
+-rw-r--r--   0        0        0     3707 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/presets.py
+-rw-r--r--   0        0        0        0 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/__init__.py
+-rw-r--r--   0        0        0     4539 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/bifrost.py
+-rw-r--r--   0        0        0     4740 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/envelope.py
+-rw-r--r--   0        0        0     1331 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/envelopes/base.j2
+-rw-r--r--   0        0        0     4756 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/reconstruct.py
+-rw-r--r--   0        0        0     6704 2023-07-01 13:58:32.237701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/sqlite.lark
+-rw-r--r--   0        0        0     8817 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/validator.py
+-rw-r--r--   0        0        0    16115 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/visitors.py
+-rw-r--r--   0        0        0        0 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/utils/__init__.py
+-rw-r--r--   0        0        0      993 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/utils/identifier.py
+-rw-r--r--   0        0        0     2716 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/utils/visitors.py
+-rw-r--r--   0        0        0     4369 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/bifrosts/sql/utils.py
+-rw-r--r--   0        0        0      711 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/constraints.py
+-rw-r--r--   0        0        0     1854 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/envelope.py
+-rw-r--r--   0        0        0      156 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/llm.py
+-rw-r--r--   0        0        0        0 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/llm_providers/__init__.py
+-rw-r--r--   0        0        0      753 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/llm_providers/mock.py
+-rw-r--r--   0        0        0     2388 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/llm_providers/openai.py
+-rw-r--r--   0        0        0        0 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/support/__init__.py
+-rw-r--r--   0        0        0     1182 2023-07-01 13:58:32.241701 heimdallm-0.1.2/heimdallm/support/github.py
+-rw-r--r--   0        0        0     1547 2023-07-01 13:58:32.273700 heimdallm-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7808 1970-01-01 00:00:00.000000 heimdallm-0.1.2/PKG-INFO
```

### Comparing `heimdallm-0.1.1/CONTRIBUTING.md` & `heimdallm-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.1/LICENSE` & `heimdallm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.1/README.md` & `heimdallm-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # HeimdaLLM
 
 > Heimdall, the watchman of the gods, dwelt at its entrance, where he guarded Bifrost,
 > the shimmering path connecting the realms.
 
-[![Heimdall](./docs/source/images/heimdall.png)](https://docs.heimdallm.ai)
+[![Heimdall](https://raw.githubusercontent.com/amoffat/HeimdaLLM/main/docs/source/images/heimdall.png)](https://docs.heimdallm.ai)
 [![Build status](https://github.com/amoffat/HeimdaLLM/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/amoffat/HeimdaLLM/actions)
-[![Docs](https://img.shields.io/badge/Documentation-purple.svg)](https://docs.heimdallm.ai)
+[![Docs](https://img.shields.io/badge/Docs-purple.svg)](https://docs.heimdallm.ai)
 [![GitHub Sponsors](https://img.shields.io/github/sponsors/amoffat)](https://github.com/sponsors/amoffat)
 [![PyPI](https://img.shields.io/pypi/v/heimdallm)](https://pypi.org/project/heimdallm/)
 [![License: Commercial](https://img.shields.io/badge/License-Commercial-blue.svg)](https://forms.gle/frEPeeJx81Cmwva78)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![Coverage Status](https://coveralls.io/repos/github/amoffat/HeimdaLLM/badge.svg?branch=dev)](https://coveralls.io/github/amoffat/HeimdaLLM?branch=dev)
 
 HeimdaLLM safely bridges the gap between untrusted human input and trusted
```

### Comparing `heimdallm-0.1.1/heimdallm/bifrost.py` & `heimdallm-0.1.2/heimdallm/bifrost.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.1/heimdallm/bifrosts/sql/exc.py` & `heimdallm-0.1.2/heimdallm/bifrosts/sql/exc.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.1/heimdallm/bifrosts/sql/mysql/presets.py` & `heimdallm-0.1.2/heimdallm/bifrosts/sql/mysql/presets.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/presets.py` & `heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/presets.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/select/bifrost.py` & `heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/bifrost.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/select/envelope.py` & `heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/envelope.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/select/envelopes/base.j2` & `heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/envelopes/base.j2`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/select/reconstruct.py` & `heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/reconstruct.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/select/sqlite.lark` & `heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/sqlite.lark`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/select/validator.py` & `heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/validator.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/select/visitors.py` & `heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/select/visitors.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/utils/identifier.py` & `heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/utils/identifier.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.1/heimdallm/bifrosts/sql/sqlite/utils/visitors.py` & `heimdallm-0.1.2/heimdallm/bifrosts/sql/sqlite/utils/visitors.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.1/heimdallm/bifrosts/sql/utils.py` & `heimdallm-0.1.2/heimdallm/bifrosts/sql/utils.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.1/heimdallm/constraints.py` & `heimdallm-0.1.2/heimdallm/constraints.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.1/heimdallm/envelope.py` & `heimdallm-0.1.2/heimdallm/envelope.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.1/heimdallm/llm_providers/mock.py` & `heimdallm-0.1.2/heimdallm/llm_providers/mock.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.1/heimdallm/llm_providers/openai.py` & `heimdallm-0.1.2/heimdallm/llm_providers/openai.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.1/heimdallm/support/github.py` & `heimdallm-0.1.2/heimdallm/support/github.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.1/pyproject.toml` & `heimdallm-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "heimdallm"
-version = "0.1.1"
+version = "0.1.2"
 description = "Construct trusted SQL queries from untrusted input"
 homepage = "https://github.com/amoffat/HeimdaLLM"
 repository = "https://github.com/amoffat/HeimdaLLM"
 documentation = "https://heimdallm.readthedocs.io/en/latest/"
 authors = ["Andrew Moffat <arwmoffat@gmail.com>"]
 maintainers = ["Andrew Moffat <arwmoffat@gmail.com>"]
 keywords = ["sql", "llm", "ai"]
```

### Comparing `heimdallm-0.1.1/PKG-INFO` & `heimdallm-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heimdallm
-Version: 0.1.1
+Version: 0.1.2
 Summary: Construct trusted SQL queries from untrusted input
 Home-page: https://github.com/amoffat/HeimdaLLM
 License: AGPL-3.0
 Keywords: sql,llm,ai
 Author: Andrew Moffat
 Author-email: arwmoffat@gmail.com
 Maintainer: Andrew Moffat
@@ -30,17 +30,17 @@
 Description-Content-Type: text/markdown
 
 # HeimdaLLM
 
 > Heimdall, the watchman of the gods, dwelt at its entrance, where he guarded Bifrost,
 > the shimmering path connecting the realms.
 
-[![Heimdall](./docs/source/images/heimdall.png)](https://docs.heimdallm.ai)
+[![Heimdall](https://raw.githubusercontent.com/amoffat/HeimdaLLM/main/docs/source/images/heimdall.png)](https://docs.heimdallm.ai)
 [![Build status](https://github.com/amoffat/HeimdaLLM/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/amoffat/HeimdaLLM/actions)
-[![Docs](https://img.shields.io/badge/Documentation-purple.svg)](https://docs.heimdallm.ai)
+[![Docs](https://img.shields.io/badge/Docs-purple.svg)](https://docs.heimdallm.ai)
 [![GitHub Sponsors](https://img.shields.io/github/sponsors/amoffat)](https://github.com/sponsors/amoffat)
 [![PyPI](https://img.shields.io/pypi/v/heimdallm)](https://pypi.org/project/heimdallm/)
 [![License: Commercial](https://img.shields.io/badge/License-Commercial-blue.svg)](https://forms.gle/frEPeeJx81Cmwva78)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![Coverage Status](https://coveralls.io/repos/github/amoffat/HeimdaLLM/badge.svg?branch=dev)](https://coveralls.io/github/amoffat/HeimdaLLM?branch=dev)
 
 HeimdaLLM safely bridges the gap between untrusted human input and trusted
```

