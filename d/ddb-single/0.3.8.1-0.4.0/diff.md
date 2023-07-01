# Comparing `tmp/ddb_single-0.3.8.1.zip` & `tmp/ddb_single-0.4.0.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 22596 bytes, number of entries: 21
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 07:10 ddb_single-0.3.8.1/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 07:10 ddb_single-0.3.8.1/ddb_single/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 07:10 ddb_single-0.3.8.1/ddb_single.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-27 07:10 ddb_single-0.3.8.1/tests/
--rw-r--r--  2.0 unx     8806 b- defN 23-Jun-27 07:10 ddb_single-0.3.8.1/PKG-INFO
--rw-r--r--  2.0 unx       38 b- defN 23-Jun-27 07:10 ddb_single-0.3.8.1/setup.cfg
--rw-r--r--  2.0 unx      774 b- defN 23-Jun-27 07:10 ddb_single-0.3.8.1/setup.py
--rw-r--r--  2.0 unx      284 b- defN 23-Jun-27 07:10 ddb_single-0.3.8.1/ddb_single/__init__.py
--rw-r--r--  2.0 unx     6118 b- defN 23-Jun-27 07:10 ddb_single-0.3.8.1/ddb_single/utils_botos.py
--rw-r--r--  2.0 unx     9770 b- defN 23-Jun-27 07:10 ddb_single-0.3.8.1/ddb_single/query.py
--rw-r--r--  2.0 unx    13659 b- defN 23-Jun-27 07:10 ddb_single-0.3.8.1/ddb_single/model.py
--rw-r--r--  2.0 unx    22402 b- defN 23-Jun-27 07:10 ddb_single-0.3.8.1/ddb_single/table.py
--rw-r--r--  2.0 unx     8806 b- defN 23-Jun-27 07:10 ddb_single-0.3.8.1/ddb_single.egg-info/PKG-INFO
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-27 07:10 ddb_single-0.3.8.1/ddb_single.egg-info/requires.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-27 07:10 ddb_single-0.3.8.1/ddb_single.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx      370 b- defN 23-Jun-27 07:10 ddb_single-0.3.8.1/ddb_single.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-27 07:10 ddb_single-0.3.8.1/ddb_single.egg-info/top_level.txt
--rw-r--r--  2.0 unx     2929 b- defN 23-Jun-27 07:10 ddb_single-0.3.8.1/tests/test_batch.py
--rw-r--r--  2.0 unx     2759 b- defN 23-Jun-27 07:10 ddb_single-0.3.8.1/tests/test_query.py
--rw-r--r--  2.0 unx     2072 b- defN 23-Jun-27 07:10 ddb_single-0.3.8.1/tests/test_search.py
--rw-r--r--  2.0 unx     3594 b- defN 23-Jun-27 07:10 ddb_single-0.3.8.1/tests/test_relation.py
-21 files, 82399 bytes uncompressed, 19360 bytes compressed:  76.5%
+Zip file size: 23449 bytes, number of entries: 21
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 10:21 ddb_single-0.4.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 10:21 ddb_single-0.4.0/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 10:21 ddb_single-0.4.0/ddb_single/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 10:21 ddb_single-0.4.0/ddb_single.egg-info/
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-01 10:21 ddb_single-0.4.0/setup.cfg
+-rw-r--r--  2.0 unx      774 b- defN 23-Jul-01 10:20 ddb_single-0.4.0/setup.py
+-rw-r--r--  2.0 unx     8804 b- defN 23-Jul-01 10:21 ddb_single-0.4.0/PKG-INFO
+-rw-r--r--  2.0 unx     6403 b- defN 23-Jul-01 10:20 ddb_single-0.4.0/tests/test_query.py
+-rw-r--r--  2.0 unx     2123 b- defN 23-Jul-01 10:20 ddb_single-0.4.0/tests/test_search.py
+-rw-r--r--  2.0 unx     3706 b- defN 23-Jul-01 10:20 ddb_single-0.4.0/tests/test_relation.py
+-rw-r--r--  2.0 unx     3036 b- defN 23-Jul-01 10:20 ddb_single-0.4.0/tests/test_batch.py
+-rw-r--r--  2.0 unx      284 b- defN 23-Jul-01 10:20 ddb_single-0.4.0/ddb_single/__init__.py
+-rw-r--r--  2.0 unx    22402 b- defN 23-Jul-01 10:20 ddb_single-0.4.0/ddb_single/table.py
+-rw-r--r--  2.0 unx     6118 b- defN 23-Jul-01 10:20 ddb_single-0.4.0/ddb_single/utils_botos.py
+-rw-r--r--  2.0 unx    13992 b- defN 23-Jul-01 10:20 ddb_single-0.4.0/ddb_single/model.py
+-rw-r--r--  2.0 unx    10375 b- defN 23-Jul-01 10:20 ddb_single-0.4.0/ddb_single/query.py
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-01 10:21 ddb_single-0.4.0/ddb_single.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-01 10:21 ddb_single-0.4.0/ddb_single.egg-info/requires.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-01 10:21 ddb_single-0.4.0/ddb_single.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     8804 b- defN 23-Jul-01 10:21 ddb_single-0.4.0/ddb_single.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx      370 b- defN 23-Jul-01 10:21 ddb_single-0.4.0/ddb_single.egg-info/SOURCES.txt
+21 files, 87247 bytes uncompressed, 20297 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -1,64 +1,64 @@
-Filename: ddb_single-0.3.8.1/
+Filename: ddb_single-0.4.0/
 Comment: 
 
-Filename: ddb_single-0.3.8.1/ddb_single/
+Filename: ddb_single-0.4.0/tests/
 Comment: 
 
-Filename: ddb_single-0.3.8.1/ddb_single.egg-info/
+Filename: ddb_single-0.4.0/ddb_single/
 Comment: 
 
-Filename: ddb_single-0.3.8.1/tests/
+Filename: ddb_single-0.4.0/ddb_single.egg-info/
 Comment: 
 
-Filename: ddb_single-0.3.8.1/PKG-INFO
+Filename: ddb_single-0.4.0/setup.cfg
 Comment: 
 
-Filename: ddb_single-0.3.8.1/setup.cfg
+Filename: ddb_single-0.4.0/setup.py
 Comment: 
 
-Filename: ddb_single-0.3.8.1/setup.py
+Filename: ddb_single-0.4.0/PKG-INFO
 Comment: 
 
-Filename: ddb_single-0.3.8.1/ddb_single/__init__.py
+Filename: ddb_single-0.4.0/tests/test_query.py
 Comment: 
 
-Filename: ddb_single-0.3.8.1/ddb_single/utils_botos.py
+Filename: ddb_single-0.4.0/tests/test_search.py
 Comment: 
 
-Filename: ddb_single-0.3.8.1/ddb_single/query.py
+Filename: ddb_single-0.4.0/tests/test_relation.py
 Comment: 
 
-Filename: ddb_single-0.3.8.1/ddb_single/model.py
+Filename: ddb_single-0.4.0/tests/test_batch.py
 Comment: 
 
-Filename: ddb_single-0.3.8.1/ddb_single/table.py
+Filename: ddb_single-0.4.0/ddb_single/__init__.py
 Comment: 
 
-Filename: ddb_single-0.3.8.1/ddb_single.egg-info/PKG-INFO
+Filename: ddb_single-0.4.0/ddb_single/table.py
 Comment: 
 
-Filename: ddb_single-0.3.8.1/ddb_single.egg-info/requires.txt
+Filename: ddb_single-0.4.0/ddb_single/utils_botos.py
 Comment: 
 
-Filename: ddb_single-0.3.8.1/ddb_single.egg-info/dependency_links.txt
+Filename: ddb_single-0.4.0/ddb_single/model.py
 Comment: 
 
-Filename: ddb_single-0.3.8.1/ddb_single.egg-info/SOURCES.txt
+Filename: ddb_single-0.4.0/ddb_single/query.py
 Comment: 
 
-Filename: ddb_single-0.3.8.1/ddb_single.egg-info/top_level.txt
+Filename: ddb_single-0.4.0/ddb_single.egg-info/dependency_links.txt
 Comment: 
 
-Filename: ddb_single-0.3.8.1/tests/test_batch.py
+Filename: ddb_single-0.4.0/ddb_single.egg-info/requires.txt
 Comment: 
 
-Filename: ddb_single-0.3.8.1/tests/test_query.py
+Filename: ddb_single-0.4.0/ddb_single.egg-info/top_level.txt
 Comment: 
 
-Filename: ddb_single-0.3.8.1/tests/test_search.py
+Filename: ddb_single-0.4.0/ddb_single.egg-info/PKG-INFO
 Comment: 
 
-Filename: ddb_single-0.3.8.1/tests/test_relation.py
+Filename: ddb_single-0.4.0/ddb_single.egg-info/SOURCES.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `ddb_single-0.3.8.1/PKG-INFO` & `ddb_single-0.4.0/ddb_single.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ddb_single
-Version: 0.3.8.1
+Name: ddb-single
+Version: 0.4.0
 Summary: Python DynamoDB interface, specialized in single-table design.
 Home-page: https://github.com/medaka0213/DynamoDB-SingleTable
 Author: medaka
 License: MIT
 Keywords: aws dynamodb serverless
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
```

## Comparing `ddb_single-0.3.8.1/setup.py` & `ddb_single-0.4.0/setup.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.3.8.1/ddb_single/utils_botos.py` & `ddb_single-0.4.0/ddb_single/utils_botos.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.3.8.1/ddb_single/query.py` & `ddb_single-0.4.0/ddb_single/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,30 +114,31 @@
         old_item = self.get_by_unique(
             self.__model__.data[self.__model__.__unique_keys__[0]]
         )
         if old_item:
             if raise_if_exists:
                 raise Exception("Item Already exists")
             else:
-                self._update(old_item, batch=batch)
+                self._update(old_item, new_item={}, batch=batch)
         else:
             self._create(batch)
 
     # 更新
-    def update(self, batch=None):
+    def update(self, target: dict = None, batch=None):
         """
         Update an item.
         Args:
+            target: Target item
             batch: BatchWriteItem
         """
-        old_item = self.get_by_unique(
+        payload = self.get_by_unique(
             self.__model__.data[self.__model__.__unique_keys__[0]]
         )
-        if old_item:
-            self._update(old_item, batch=batch)
+        if payload:
+            self._update(payload, target or {}, batch=batch)
         else:
             self._create(batch=batch)
 
     def _create(self, batch=None, remove_ex_search_items=False):
         self.validate()
         search_items_add, search_items_rm = self._search_items()
         rel_items_add, rel_items_rm = self._relation_items()
@@ -148,16 +149,16 @@
         self.__table__.create(self.__model__.data, batch=batch)
         if remove_ex_search_items:
             self.__table__.batch_update(items_add, batch=batch)
             self.__table__.batch_delete_items(items_remove, batch=batch)
         else:
             self.__table__.batch_create(items_add, batch=batch)
 
-    def _update(self, old_item, batch=None):
-        self.__model__.data = {**old_item, **self.__model__.data}
+    def _update(self, old_item, new_item, batch=None):
+        self.__model__.data = {**old_item, **self.__model__.data, **new_item}
         self.__model__.data[self.__model__.__primary_key__] = old_item[
             self.__model__.__primary_key__
         ]
         self.__model__.data[self.__model__.__secondary_key__] = old_item[
             self.__model__.__secondary_key__
         ]
         if not util_b.is_same_json(old_item, self.__model__.data):
@@ -176,25 +177,35 @@
     def delete(self, target: dict = None, batch=None):
         """
         Delete an item.
         Args:
             batch: BatchWriteItem
         """
         target = target or self.__model__.data
-        self.delete_by_pk(target[self.__model__.__primary_key__], batch=batch)
+        if target.get(self.__model__.__unique_keys__[0]):
+            # unique があれば unique で削除
+            self.delete_by_unique(
+                target[self.__model__.__unique_keys__[0]], batch=batch
+            )
+        elif target.get(self.__model__.__primary_key__):
+            # pk があれば pk で削除
+            self.delete_by_pk(target[self.__model__.__primary_key__], batch=batch)
+        else:
+            # 両方とも無ければエラー
+            raise Exception("Primary key or Unique key is required.")
 
     def delete_by_unique(self, value, batch=None):
         """
         Delete an item by unique key.
         Args:
             batch: BatchWriteItem
         """
-        item = self.get_by_unique(value)
-        if item:
-            self.delete(item, batch=batch)
+        target = self.get_by_unique(value)
+        pk = target.get(self.__model__.__primary_key__)
+        self.delete_by_pk(pk, batch=batch)
 
     # 関連付け
     def _relation_item(self, pk, field: DBField):
         return {
             self.__model__.__primary_key__: self.__model__.data[
                 self.__model__.__primary_key__
             ],
```

## Comparing `ddb_single-0.3.8.1/ddb_single/model.py` & `ddb_single-0.4.0/ddb_single/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         required=False,
         primary_key=False,
         secondary_key=False,
         unique_key=False,
         search_key=False,
         reletion=None,
         reletion_by_unique=True,
+        ignore_case=False,
         **kwargs,
     ):
         """
         Args:
             type (FieldType): The type of the field.
             default: The default value of the field.
             default_factory: The default factory of the field.
@@ -54,14 +55,15 @@
         self.required = required
         self.primary_key = primary_key
         self.secondary_key = secondary_key
         self.unique_key = unique_key
         self.search_key = search_key or unique_key
         self.relation = reletion
         self.reletion_by_unique = reletion_by_unique
+        self.ignore_case = ignore_case
         self.value = None
 
     def setup(self, name, model_cls):
         self.__model_cls__ = model_cls
         self.__table__: Table = model_cls.__table__
         self.name = name
         if self.primary_key:
@@ -187,28 +189,34 @@
     def search_item(self, pk):
         """
         Args:
             pk: The primary key of the item.
         Returns:
             dict: The search item.
         """
+        _value = self.value
+        if self.ignore_case and isinstance(_value, str):
+            # lower case if self.ignore_case = True
+            _value = _value.lower()
         return {
             self.__table__.__primary_key__: pk,
             self.__table__.__secondary_key__: self.search_key_factory(),
-            self.search_data_key(): self.value,
+            self.search_data_key(): _value,
         }
 
     def key_ex(self, value, mode):
         """
         Args:
             value: The value to be compared.
             mode: The mode of the comparison.
         Returns:
             dict: The key expression.
         """
+        if self.ignore_case and isinstance(value, str):
+            value = value.lower()
         if self.secondary_key:
             raise ValueError(f"Secondary key can not be used as a key: {self.name}")
         res = {
             "FilterMethod": util_b.attr_method(self.name, value, mode),
         }
         if util_b.is_key(mode):
             if self.primary_key:
```

## Comparing `ddb_single-0.3.8.1/ddb_single/table.py` & `ddb_single-0.4.0/ddb_single/table.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.3.8.1/ddb_single.egg-info/PKG-INFO` & `ddb_single-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ddb-single
-Version: 0.3.8.1
+Name: ddb_single
+Version: 0.4.0
 Summary: Python DynamoDB interface, specialized in single-table design.
 Home-page: https://github.com/medaka0213/DynamoDB-SingleTable
 Author: medaka
 License: MIT
 Keywords: aws dynamodb serverless
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
```

## Comparing `ddb_single-0.3.8.1/tests/test_batch.py` & `ddb_single-0.4.0/tests/test_batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 
 from ddb_single.table import FieldType, Table
 from ddb_single.model import BaseModel, DBField
 from ddb_single.query import Query
 
 import datetime
 
+
+import logging
+
+logging.basicConfig(level=logging.INFO)
+
 table = Table(
     table_name="batch_test_" + datetime.datetime.now().strftime("%Y%m%d%H%M%S"),
     endpoint_url="http://localhost:8000",
     region_name="us-west-2",
     aws_access_key_id="ACCESS_ID",
     aws_secret_access_key="ACCESS_KEY",
 )
@@ -79,7 +84,11 @@
         pks = query.model(User).search(User.name.begins_with("test"), pk_only=True)
         with table.batch_writer() as batch:
             for pk in pks[:3]:
                 query.model(User).delete_by_pk(pk, batch=batch)
         # 効果確認
         res = query.model(User).search(User.name.begins_with("test"))
         self.assertEqual(len(res), 1)
+
+
+if __name__ == "__main__":
+    unittest.main()
```

## Comparing `ddb_single-0.3.8.1/tests/test_search.py` & `ddb_single-0.4.0/tests/test_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import unittest
 
 from ddb_single.table import FieldType, Table
 from ddb_single.model import BaseModel, DBField
 from ddb_single.query import Query
 
 import datetime
-
 import logging
 
-logging.basicConfig(level=logging.DEBUG)
+logging.basicConfig(level=logging.INFO)
 
 table = Table(
-    table_name="query_test_" + datetime.datetime.now().strftime("%Y%m%d%H%M%S"),
+    table_name="search_test_" + datetime.datetime.now().strftime("%Y%m%d%H%M%S"),
     endpoint_url="http://localhost:8000",
     region_name="us-west-2",
     aws_access_key_id="ACCESS_ID",
     aws_secret_access_key="ACCESS_KEY",
 )
 table.init()
 
@@ -65,7 +64,11 @@
     def test_not_equal(self):
         res = query.model(User).search(User.name.ne("test1"))
         self.assertEqual(len(res), 2)
 
     def test_begins(self):
         res = query.model(User).search(User.name.begins_with("test"))
         self.assertEqual(len(res), 3)
+
+
+if __name__ == "__main__":
+    unittest.main()
```

## Comparing `ddb_single-0.3.8.1/tests/test_relation.py` & `ddb_single-0.4.0/tests/test_relation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import unittest
 
 from ddb_single.table import FieldType, Table
 from ddb_single.model import BaseModel, DBField
 from ddb_single.query import Query
 
 import datetime
+import logging
+
+logging.basicConfig(level=logging.INFO)
 
 table = Table(
     table_name="rel_test_" + datetime.datetime.now().strftime("%Y%m%d%H%M%S"),
     endpoint_url="http://localhost:8000",
     region_name="us-west-2",
     aws_access_key_id="ACCESS_ID",
     aws_secret_access_key="ACCESS_KEY",
@@ -97,7 +100,11 @@
         res = query.model(BlogPost).get(blogpost.data["pk"])
         self.assertIsNotNone(res)
         self.assertEqual(res["author"], "test2")
         # 効果確認 (関連)
         rel_user = query.model(blogpost).get_relation(model=User)
         self.assertEqual(len(rel_user), 1)
         self.assertEqual(rel_user[0]["name"], "test2")
+
+
+if __name__ == "__main__":
+    unittest.main()
```

