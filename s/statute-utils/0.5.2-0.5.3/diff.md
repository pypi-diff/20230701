# Comparing `tmp/statute_utils-0.5.2.tar.gz` & `tmp/statute_utils-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statute_utils-0.5.2.tar", max compression
+gzip compressed data, was "statute_utils-0.5.3.tar", max compression
```

## Comparing `statute_utils-0.5.2.tar` & `statute_utils-0.5.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.5.2/LICENSE
--rw-r--r--   0        0        0      898 2023-07-01 01:29:45.722010 statute_utils-0.5.2/README.md
--rw-r--r--   0        0        0     1380 2023-07-01 07:27:19.364605 statute_utils-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      457 2023-07-01 06:23:31.949055 statute_utils-0.5.2/statute_utils/__init__.py
--rw-r--r--   0        0        0      275 2023-07-01 05:31:15.495445 statute_utils-0.5.2/statute_utils/components/__init__.py
--rw-r--r--   0        0        0     8971 2023-07-01 07:26:53.216138 statute_utils-0.5.2/statute_utils/components/category.py
--rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.5.2/statute_utils/components/short.py
--rw-r--r--   0        0        0     4683 2023-07-01 04:37:03.665122 statute_utils-0.5.2/statute_utils/components/utils.py
--rw-r--r--   0        0        0     9658 2023-07-01 06:55:45.539814 statute_utils-0.5.2/statute_utils/main.py
--rw-r--r--   0        0        0     5022 2023-07-01 06:44:19.410593 statute_utils-0.5.2/statute_utils/models.py
--rw-r--r--   0        0        0     9880 2023-07-01 07:26:41.687325 statute_utils-0.5.2/statute_utils/models_names.py
--rw-r--r--   0        0        0     6682 2023-07-01 06:21:01.765608 statute_utils-0.5.2/statute_utils/models_serials.py
--rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.5.2/statute_utils/recipes/__init__.py
--rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.5.2/statute_utils/recipes/const.py
--rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.5.2/statute_utils/recipes/digits.py
--rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.5.2/statute_utils/recipes/roc.py
--rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.5.2/statute_utils/recipes/spain.py
--rw-r--r--   0        0        0     4709 2023-07-01 06:20:32.418706 statute_utils-0.5.2/statute_utils/tree.py
--rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 statute_utils-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.5.3/LICENSE
+-rw-r--r--   0        0        0      898 2023-07-01 01:29:45.722010 statute_utils-0.5.3/README.md
+-rw-r--r--   0        0        0     1380 2023-07-01 12:33:52.669248 statute_utils-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      457 2023-07-01 06:23:31.949055 statute_utils-0.5.3/statute_utils/__init__.py
+-rw-r--r--   0        0        0      275 2023-07-01 05:31:15.495445 statute_utils-0.5.3/statute_utils/components/__init__.py
+-rw-r--r--   0        0        0     8971 2023-07-01 07:26:53.216138 statute_utils-0.5.3/statute_utils/components/category.py
+-rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.5.3/statute_utils/components/short.py
+-rw-r--r--   0        0        0     4683 2023-07-01 04:37:03.665122 statute_utils-0.5.3/statute_utils/components/utils.py
+-rw-r--r--   0        0        0    10136 2023-07-01 12:36:21.497674 statute_utils-0.5.3/statute_utils/main.py
+-rw-r--r--   0        0        0     5022 2023-07-01 06:44:19.410593 statute_utils-0.5.3/statute_utils/models.py
+-rw-r--r--   0        0        0     9880 2023-07-01 07:26:41.687325 statute_utils-0.5.3/statute_utils/models_names.py
+-rw-r--r--   0        0        0     6682 2023-07-01 06:21:01.765608 statute_utils-0.5.3/statute_utils/models_serials.py
+-rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.5.3/statute_utils/recipes/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.5.3/statute_utils/recipes/const.py
+-rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.5.3/statute_utils/recipes/digits.py
+-rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.5.3/statute_utils/recipes/roc.py
+-rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.5.3/statute_utils/recipes/spain.py
+-rw-r--r--   0        0        0     4709 2023-07-01 06:20:32.418706 statute_utils-0.5.3/statute_utils/tree.py
+-rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 statute_utils-0.5.3/PKG-INFO
```

### Comparing `statute_utils-0.5.2/LICENSE` & `statute_utils-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.2/README.md` & `statute_utils-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.2/pyproject.toml` & `statute_utils-0.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "statute-utils"
-version = "0.5.2"
+version = "0.5.3"
 description = "Philippine statutory law pattern matching and unit retrieval."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/statute-utils"
 documentation = "https://justmars.github.io/statute-utils"
 classifiers = [
```

### Comparing `statute_utils-0.5.2/statute_utils/components/category.py` & `statute_utils-0.5.3/statute_utils/components/category.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.2/statute_utils/components/short.py` & `statute_utils-0.5.3/statute_utils/components/short.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.2/statute_utils/components/utils.py` & `statute_utils-0.5.3/statute_utils/components/utils.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.2/statute_utils/main.py` & `statute_utils-0.5.3/statute_utils/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         logging.warning(err)
         return True
 
     if rule.date < document_date:
         return True
     else:
         err = (
-            f"{context or ''} {document_date=} likely erroneous for"
+            f"Date mismatch > {context or ''} | {document_date=} likely erroneous for"
             f" {rule=} {rule.date=}".strip()
         )
         logging.error(err)
         return False
 
 
 def extract_rules(
@@ -146,31 +146,34 @@
             yield rule
 
     for rule in extract_named_rules(text, document_date):
         if is_rule_ok(rule, document_date, context):
             yield rule
 
 
-def extract_rule(text: str, document_date: datetime.date | None = None) -> Rule | None:
+def extract_rule(
+    text: str, document_date: datetime.date | None = None, context: str | None = None
+) -> Rule | None:
     """Thin wrapper over `extract_rules()`. Get the first matching Rule found.
 
     Examples:
         >>> text = "The Civil Code of the Philippines, the old Spanish Civil Code; Rep Act No. 386"
         >>> extract_rule(text)  # get the first matching rule
         <Rule: ra 386>
 
     Args:
         text (str): Text to search for statute patterns.
         document_date (datetime.date | None, optional): When present, makes a naive dated extraction of _named_ ambiguous rules. Defaults to None.
+        context (str | None, optional): Helps provide error message, if provided. Defaults to None.
 
     Returns:
         Rule | None: The first Rule found, if it exists
     """  # noqa: E501
     try:
-        return next(extract_rules(text, document_date))
+        return next(extract_rules(text, document_date, context))
     except StopIteration:
         return None
 
 
 class CountedStatute(NamedTuple):
     """Based on results from `extract_rules()`, get count of each
     unique rule found."""
@@ -180,15 +183,18 @@
     mentions: int = 1
 
     def __repr__(self) -> str:
         return f"{self.cat} {self.num}: {self.mentions}"
 
     @classmethod
     def from_source(
-        cls, text: str, document_date: datetime.date | None = None
+        cls,
+        text: str,
+        document_date: datetime.date | None = None,
+        context: str | None = None,
     ) -> Iterator[Self]:
         """Detect counted rules from source `text`.
 
         Examples:
             >>> text = "The Civil Code of the Philippines, the old Spanish Civil Code; Rep Act No. 386"
             >>> results = list(CountedStatute.from_source(text))
             >>> results
@@ -196,19 +202,21 @@
             >>> results[0] == CountedStatute(cat=StatuteSerialCategory('ra'),num='386', mentions=2)
             True
             >>> results[1] == CountedStatute(cat=StatuteSerialCategory('spain'),num='civil', mentions=1)
             True
 
         Args:
             text (str): Legalese containing statutory rules in various formats.
+            document_date (datetime.date | None, optional): When present, makes a naive dated extraction of _named_ ambiguous rules. Defaults to None.
+            context (str | None, optional): Helps provide error message, if provided. Defaults to None.
 
         Yields:
             Iterator[Self]: Each counted rule found.
         """  # noqa: E501
-        rules = extract_rules(text, document_date)
+        rules = extract_rules(text, document_date, context)
         unique_rules = Counter(rules)
         for rule, mention_count in unique_rules.items():
             yield CountedStatute(cat=rule.cat, num=rule.num, mentions=mention_count)
 
     @classmethod
     def from_repr_format(cls, repr_texts: list[str]) -> Iterator[Self]:
         """Generate pythonic counterparts from `<cat> <id>: <mentions>` format.
```

### Comparing `statute_utils-0.5.2/statute_utils/models.py` & `statute_utils-0.5.3/statute_utils/models.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.2/statute_utils/models_names.py` & `statute_utils-0.5.3/statute_utils/models_names.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.2/statute_utils/models_serials.py` & `statute_utils-0.5.3/statute_utils/models_serials.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.2/statute_utils/recipes/digits.py` & `statute_utils-0.5.3/statute_utils/recipes/digits.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.2/statute_utils/recipes/spain.py` & `statute_utils-0.5.3/statute_utils/recipes/spain.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.2/statute_utils/tree.py` & `statute_utils-0.5.3/statute_utils/tree.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.2/PKG-INFO` & `statute_utils-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statute-utils
-Version: 0.5.2
+Version: 0.5.3
 Summary: Philippine statutory law pattern matching and unit retrieval.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
```

