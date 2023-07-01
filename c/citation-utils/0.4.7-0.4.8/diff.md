# Comparing `tmp/citation_utils-0.4.7.tar.gz` & `tmp/citation_utils-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_utils-0.4.7.tar", max compression
+gzip compressed data, was "citation_utils-0.4.8.tar", max compression
```

## Comparing `citation_utils-0.4.7.tar` & `citation_utils-0.4.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1491 2023-06-23 10:27:21.228309 citation_utils-0.4.7/LICENSE
--rw-r--r--   0        0        0      653 2023-06-25 09:54:14.887730 citation_utils-0.4.7/citation_utils/__init__.py
--rw-r--r--   0        0        0    18085 2023-06-30 03:42:19.085667 citation_utils-0.4.7/citation_utils/citation.py
--rw-r--r--   0        0        0     1179 2023-06-25 09:54:14.891749 citation_utils-0.4.7/citation_utils/dockets/__init__.py
--rw-r--r--   0        0        0     3125 2023-06-29 03:28:48.048714 citation_utils-0.4.7/citation_utils/dockets/constructed_ac.py
--rw-r--r--   0        0        0     3164 2023-06-29 03:28:29.361313 citation_utils-0.4.7/citation_utils/dockets/constructed_am.py
--rw-r--r--   0        0        0     2457 2023-06-25 09:54:14.895608 citation_utils-0.4.7/citation_utils/dockets/constructed_bm.py
--rw-r--r--   0        0        0     2866 2023-06-29 03:27:47.112900 citation_utils-0.4.7/citation_utils/dockets/constructed_gr.py
--rw-r--r--   0        0        0     2094 2023-06-25 09:54:14.896184 citation_utils-0.4.7/citation_utils/dockets/constructed_jib.py
--rw-r--r--   0        0        0     2692 2023-06-28 10:55:51.445938 citation_utils-0.4.7/citation_utils/dockets/constructed_oca.py
--rw-r--r--   0        0        0     1597 2023-06-25 09:54:14.896710 citation_utils-0.4.7/citation_utils/dockets/constructed_pet.py
--rw-r--r--   0        0        0     2055 2023-06-28 10:33:49.974829 citation_utils-0.4.7/citation_utils/dockets/constructed_udk.py
--rw-r--r--   0        0        0      364 2023-06-25 10:00:40.543092 citation_utils-0.4.7/citation_utils/dockets/models/__init__.py
--rw-r--r--   0        0        0     4834 2023-06-25 09:54:14.900031 citation_utils-0.4.7/citation_utils/dockets/models/constructor.py
--rw-r--r--   0        0        0     1373 2023-06-25 09:54:14.900293 citation_utils-0.4.7/citation_utils/dockets/models/docket_category.py
--rw-r--r--   0        0        0     1696 2023-06-29 03:24:53.524673 citation_utils-0.4.7/citation_utils/dockets/models/docket_citation.py
--rw-r--r--   0        0        0     5873 2023-06-29 02:04:16.817476 citation_utils-0.4.7/citation_utils/dockets/models/docket_model.py
--rw-r--r--   0        0        0     3404 2023-06-28 02:34:55.066065 citation_utils-0.4.7/citation_utils/dockets/models/docket_rules.py
--rw-r--r--   0        0        0     2911 2023-06-25 09:54:14.901368 citation_utils-0.4.7/citation_utils/dockets/models/gr_clean.py
--rw-r--r--   0        0        0       81 2023-06-25 09:54:14.902014 citation_utils-0.4.7/citation_utils/dockets/models/misc/__init__.py
--rw-r--r--   0        0        0      746 2023-06-25 09:54:14.903593 citation_utils-0.4.7/citation_utils/dockets/models/misc/extra.py
--rw-r--r--   0        0        0     1514 2023-06-25 09:54:14.903861 citation_utils-0.4.7/citation_utils/dockets/models/misc/num.py
--rw-r--r--   0        0        0      242 2023-06-25 09:54:14.904129 citation_utils-0.4.7/citation_utils/dockets/models/misc/x.py
--rw-r--r--   0        0        0     5861 2023-06-29 03:34:11.063815 citation_utils-0.4.7/citation_utils/document.py
--rw-r--r--   0        0        0     2531 2023-06-25 09:54:14.904670 citation_utils-0.4.7/citation_utils/special.py
--rw-r--r--   0        0        0     1312 2023-06-30 03:42:55.806152 citation_utils-0.4.7/pyproject.toml
--rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 citation_utils-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-23 10:27:21.228309 citation_utils-0.4.8/LICENSE
+-rw-r--r--   0        0        0      653 2023-06-25 09:54:14.887730 citation_utils-0.4.8/citation_utils/__init__.py
+-rw-r--r--   0        0        0    18063 2023-07-01 03:42:49.795835 citation_utils-0.4.8/citation_utils/citation.py
+-rw-r--r--   0        0        0     1179 2023-06-25 09:54:14.891749 citation_utils-0.4.8/citation_utils/dockets/__init__.py
+-rw-r--r--   0        0        0     3125 2023-06-29 03:28:48.048714 citation_utils-0.4.8/citation_utils/dockets/constructed_ac.py
+-rw-r--r--   0        0        0     3164 2023-06-29 03:28:29.361313 citation_utils-0.4.8/citation_utils/dockets/constructed_am.py
+-rw-r--r--   0        0        0     2457 2023-06-25 09:54:14.895608 citation_utils-0.4.8/citation_utils/dockets/constructed_bm.py
+-rw-r--r--   0        0        0     2866 2023-06-29 03:27:47.112900 citation_utils-0.4.8/citation_utils/dockets/constructed_gr.py
+-rw-r--r--   0        0        0     2094 2023-06-25 09:54:14.896184 citation_utils-0.4.8/citation_utils/dockets/constructed_jib.py
+-rw-r--r--   0        0        0     2692 2023-06-28 10:55:51.445938 citation_utils-0.4.8/citation_utils/dockets/constructed_oca.py
+-rw-r--r--   0        0        0     1597 2023-06-25 09:54:14.896710 citation_utils-0.4.8/citation_utils/dockets/constructed_pet.py
+-rw-r--r--   0        0        0     2055 2023-06-28 10:33:49.974829 citation_utils-0.4.8/citation_utils/dockets/constructed_udk.py
+-rw-r--r--   0        0        0      364 2023-06-25 10:00:40.543092 citation_utils-0.4.8/citation_utils/dockets/models/__init__.py
+-rw-r--r--   0        0        0     4834 2023-06-25 09:54:14.900031 citation_utils-0.4.8/citation_utils/dockets/models/constructor.py
+-rw-r--r--   0        0        0     1373 2023-06-25 09:54:14.900293 citation_utils-0.4.8/citation_utils/dockets/models/docket_category.py
+-rw-r--r--   0        0        0     1778 2023-07-01 03:41:01.932253 citation_utils-0.4.8/citation_utils/dockets/models/docket_citation.py
+-rw-r--r--   0        0        0     5839 2023-07-01 03:42:14.972022 citation_utils-0.4.8/citation_utils/dockets/models/docket_model.py
+-rw-r--r--   0        0        0     3404 2023-06-28 02:34:55.066065 citation_utils-0.4.8/citation_utils/dockets/models/docket_rules.py
+-rw-r--r--   0        0        0     2911 2023-06-25 09:54:14.901368 citation_utils-0.4.8/citation_utils/dockets/models/gr_clean.py
+-rw-r--r--   0        0        0       81 2023-06-25 09:54:14.902014 citation_utils-0.4.8/citation_utils/dockets/models/misc/__init__.py
+-rw-r--r--   0        0        0      746 2023-06-25 09:54:14.903593 citation_utils-0.4.8/citation_utils/dockets/models/misc/extra.py
+-rw-r--r--   0        0        0     1514 2023-06-25 09:54:14.903861 citation_utils-0.4.8/citation_utils/dockets/models/misc/num.py
+-rw-r--r--   0        0        0      242 2023-06-25 09:54:14.904129 citation_utils-0.4.8/citation_utils/dockets/models/misc/x.py
+-rw-r--r--   0        0        0     5861 2023-06-29 03:34:11.063815 citation_utils-0.4.8/citation_utils/document.py
+-rw-r--r--   0        0        0     2531 2023-06-25 09:54:14.904670 citation_utils-0.4.8/citation_utils/special.py
+-rw-r--r--   0        0        0     1312 2023-07-01 03:47:11.964121 citation_utils-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 citation_utils-0.4.8/PKG-INFO
```

### Comparing `citation_utils-0.4.7/LICENSE` & `citation_utils-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.7/citation_utils/__init__.py` & `citation_utils-0.4.8/citation_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.7/citation_utils/citation.py` & `citation_utils-0.4.8/citation_utils/citation.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     datetime.date(2000, 10, 10) | `docket_date` | optional (date) | When docket serial issued
     GR 138570, Oct. 10, 2000 | `docket` | optional (str) | Combined `docket_category` `docket_serial` `docket_date`
     None | `phil` | optional (str) | combined `volume` Phil. `page`
     342 SCRA 449 | `scra` | optional (str) | combined `volume` SCRA `page`
     None | `offg` | optional (str) | combined `volume` O.G. `page`
     """  # noqa: E501
 
-    model_config = ConfigDict(use_enum_values=True, str_strip_whitespace=True)
+    model_config = ConfigDict(str_strip_whitespace=True)
     docket_category: DocketCategory | None = Field(default=None, alias="cat")
     docket_serial: str | None = Field(default=None, alias="num")
     docket_date: datetime.date | None = Field(default=None, alias="date")
     phil: str | None = Field(default=None)
     scra: str | None = Field(default=None)
     offg: str | None = Field(default=None)
```

### Comparing `citation_utils-0.4.7/citation_utils/dockets/__init__.py` & `citation_utils-0.4.8/citation_utils/dockets/__init__.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.7/citation_utils/dockets/constructed_ac.py` & `citation_utils-0.4.8/citation_utils/dockets/constructed_ac.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.7/citation_utils/dockets/constructed_am.py` & `citation_utils-0.4.8/citation_utils/dockets/constructed_am.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.7/citation_utils/dockets/constructed_bm.py` & `citation_utils-0.4.8/citation_utils/dockets/constructed_bm.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.7/citation_utils/dockets/constructed_gr.py` & `citation_utils-0.4.8/citation_utils/dockets/constructed_gr.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.7/citation_utils/dockets/constructed_jib.py` & `citation_utils-0.4.8/citation_utils/dockets/constructed_jib.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.7/citation_utils/dockets/constructed_oca.py` & `citation_utils-0.4.8/citation_utils/dockets/constructed_oca.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.7/citation_utils/dockets/constructed_pet.py` & `citation_utils-0.4.8/citation_utils/dockets/constructed_pet.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.7/citation_utils/dockets/constructed_udk.py` & `citation_utils-0.4.8/citation_utils/dockets/constructed_udk.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.7/citation_utils/dockets/models/constructor.py` & `citation_utils-0.4.8/citation_utils/dockets/models/constructor.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.7/citation_utils/dockets/models/docket_category.py` & `citation_utils-0.4.8/citation_utils/dockets/models/docket_category.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.7/citation_utils/dockets/models/docket_citation.py` & `citation_utils-0.4.8/citation_utils/dockets/models/docket_citation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import abc
 from collections.abc import Iterator
 from typing import Self
 
 from citation_report import Report
+from pydantic import field_serializer
 
+from .docket_category import DocketCategory
 from .docket_model import Docket
 
 
 class DocketReportCitation(Docket, Report, abc.ABC):
     """Note `Report` is defined in a separate library `citation-report`.
 
     The `DocketReportCitation` abstract class makes sure that all of the
```

### Comparing `citation_utils-0.4.7/citation_utils/dockets/models/docket_model.py` & `citation_utils-0.4.8/citation_utils/dockets/models/docket_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from datetime import date
 from typing import Self
 
 from citation_date import DOCKET_DATE_FORMAT
 from citation_report.main import is_eq
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import BaseModel, ConfigDict, Field, field_serializer
 
 from .docket_category import DocketCategory
 from .gr_clean import gr_prefix_clean
 
 DB_SERIAL_NUM = re.compile(r"^(?P<serial>[a-z0-9-]+).*$")
 """Ideally, the docket id for the database should only be alpha-numeric, lowercase with dashes."""  # noqa: E501
 
@@ -45,15 +45,14 @@
     Sample Citation | Category | Serial | Date
     :-- |:--:|:--:|:--:
     _G.R. Nos. 138570, October 10, 2000_ | GR | 74910 | October 10, 2000
     _A.M. RTJ-12-2317 (Formerly OCA I.P.I. No. 10-3378-RTJ), Jan 1, 2000_ | AM | RTJ-12-2317 |Jan 1, 2000
     _A.C. No. 10179 (Formerly CBD 11-2985), March 04, 2014_ | AC | 10179 | Mar. 4, 2014
     """  # noqa: E501
 
-    model_config = ConfigDict(use_enum_values=True)
     context: str = Field(..., description="Full text matched by regex pattern.")
     category: DocketCategory = Field(..., description="e.g. General Register, etc.")
     ids: str = Field(
         ..., description="This may be comma-separated, e.g. '12, 32, and 41'"
     )
     docket_date: date = Field(...)
```

### Comparing `citation_utils-0.4.7/citation_utils/dockets/models/docket_rules.py` & `citation_utils-0.4.8/citation_utils/dockets/models/docket_rules.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.7/citation_utils/dockets/models/gr_clean.py` & `citation_utils-0.4.8/citation_utils/dockets/models/gr_clean.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.7/citation_utils/dockets/models/misc/extra.py` & `citation_utils-0.4.8/citation_utils/dockets/models/misc/extra.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.7/citation_utils/dockets/models/misc/num.py` & `citation_utils-0.4.8/citation_utils/dockets/models/misc/num.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.7/citation_utils/document.py` & `citation_utils-0.4.8/citation_utils/document.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.7/citation_utils/special.py` & `citation_utils-0.4.8/citation_utils/special.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.7/pyproject.toml` & `citation_utils-0.4.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citation_utils"
-version = "0.4.7"
+version = "0.4.8"
 description = "Pattern matching Philippine Supreme Court citations."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/citation-utils"
 documentation = "https://justmars.github.io/citation-utils"
 classifiers = [
   "Topic :: Text Processing :: General",
@@ -14,15 +14,15 @@
   "Intended Audience :: Legal Industry",
   "Framework :: Pydantic",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-citation_report = "^0.1.6"
+citation_report = "^0.1.7"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3"
 pytest-cov = "^2.12.1"
 pre-commit = "^3.3"
 mkdocs = "^1.4.3"
 mkdocstrings = {extras = ["python"], version = "^0.22.0"}
```

### Comparing `citation_utils-0.4.7/PKG-INFO` & `citation_utils-0.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: citation-utils
-Version: 0.4.7
+Version: 0.4.8
 Summary: Pattern matching Philippine Supreme Court citations.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Legal Industry
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: General
 Classifier: Typing :: Typed
-Requires-Dist: citation_report (>=0.1.6,<0.2.0)
+Requires-Dist: citation_report (>=0.1.7,<0.2.0)
 Project-URL: Documentation, https://justmars.github.io/citation-utils
 Project-URL: Repository, https://github.com/justmars/citation-utils
```

