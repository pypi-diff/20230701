# Comparing `tmp/dww_test-0.0.1-py3-none-any.whl.zip` & `tmp/dww_test-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3046 bytes, number of entries: 8
+Zip file size: 3073 bytes, number of entries: 8
 -rw-r--r--  2.0 unx      122 b- defN 20-Feb-02 00:00 dww_test/__about__.py
 -rw-r--r--  2.0 unx      100 b- defN 20-Feb-02 00:00 dww_test/__init__.py
--rwxr-xr-x  2.0 unx       72 b- defN 20-Feb-02 00:00 dww_test/dww_test.py
+-rwxr-xr-x  2.0 unx      118 b- defN 20-Feb-02 00:00 dww_test/dww_test.py
 -rw-r--r--  2.0 unx       23 b- defN 20-Feb-02 00:00 dww_test/dww_test.py~
-?rw-r--r--  2.0 unx     1387 b- defN 20-Feb-02 00:00 dww_test-0.0.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dww_test-0.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1092 b- defN 20-Feb-02 00:00 dww_test-0.0.1.dist-info/licenses/LICENSE.txt
-?rw-r--r--  2.0 unx      615 b- defN 20-Feb-02 00:00 dww_test-0.0.1.dist-info/RECORD
-8 files, 3498 bytes uncompressed, 1974 bytes compressed:  43.6%
+?rw-r--r--  2.0 unx     1387 b- defN 20-Feb-02 00:00 dww_test-0.0.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dww_test-0.0.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1092 b- defN 20-Feb-02 00:00 dww_test-0.0.2.dist-info/licenses/LICENSE.txt
+?rw-r--r--  2.0 unx      616 b- defN 20-Feb-02 00:00 dww_test-0.0.2.dist-info/RECORD
+8 files, 3545 bytes uncompressed, 2001 bytes compressed:  43.6%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: dww_test/dww_test.py
 Comment: 
 
 Filename: dww_test/dww_test.py~
 Comment: 
 
-Filename: dww_test-0.0.1.dist-info/METADATA
+Filename: dww_test-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: dww_test-0.0.1.dist-info/WHEEL
+Filename: dww_test-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: dww_test-0.0.1.dist-info/licenses/LICENSE.txt
+Filename: dww_test-0.0.2.dist-info/licenses/LICENSE.txt
 Comment: 
 
-Filename: dww_test-0.0.1.dist-info/RECORD
+Filename: dww_test-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dww_test/__about__.py

```diff
@@ -1,4 +1,4 @@
 # SPDX-FileCopyrightText: 2023-present U.N. Owen <void@some.where>
 #
 # SPDX-License-Identifier: MIT
-__version__ = "0.0.1"
+__version__ = "0.0.2"
```

## dww_test/dww_test.py

```diff
@@ -1,4 +1,7 @@
 #!/usr/bin/env python
 
+def dwwfunc():
+    print("My python module")
+
 if __name__ == "__main__":
     print("dww test")
```

## Comparing `dww_test-0.0.1.dist-info/METADATA` & `dww_test-0.0.2.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dww-test
-Version: 0.0.1
+Version: 0.0.2
 Summary: Hatch test project
 Project-URL: Documentation, https://github.com/unknown/dww-test#readme
 Project-URL: Issues, https://github.com/unknown/dww-test/issues
 Project-URL: Source, https://github.com/unknown/dww-test
 Author-email: "U.N. Owen" <void@some.where>
 License-Expression: MIT
 License-File: LICENSE.txt
```

## Comparing `dww_test-0.0.1.dist-info/licenses/LICENSE.txt` & `dww_test-0.0.2.dist-info/licenses/LICENSE.txt`

 * *Files identical despite different names*

