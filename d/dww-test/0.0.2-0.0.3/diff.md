# Comparing `tmp/dww_test-0.0.2-py3-none-any.whl.zip` & `tmp/dww_test-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3073 bytes, number of entries: 8
+Zip file size: 3070 bytes, number of entries: 8
 -rw-r--r--  2.0 unx      122 b- defN 20-Feb-02 00:00 dww_test/__about__.py
 -rw-r--r--  2.0 unx      100 b- defN 20-Feb-02 00:00 dww_test/__init__.py
--rwxr-xr-x  2.0 unx      118 b- defN 20-Feb-02 00:00 dww_test/dww_test.py
+-rwxr-xr-x  2.0 unx      111 b- defN 20-Feb-02 00:00 dww_test/dww_test.py
 -rw-r--r--  2.0 unx       23 b- defN 20-Feb-02 00:00 dww_test/dww_test.py~
-?rw-r--r--  2.0 unx     1387 b- defN 20-Feb-02 00:00 dww_test-0.0.2.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dww_test-0.0.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1092 b- defN 20-Feb-02 00:00 dww_test-0.0.2.dist-info/licenses/LICENSE.txt
-?rw-r--r--  2.0 unx      616 b- defN 20-Feb-02 00:00 dww_test-0.0.2.dist-info/RECORD
-8 files, 3545 bytes uncompressed, 2001 bytes compressed:  43.6%
+?rw-r--r--  2.0 unx     1387 b- defN 20-Feb-02 00:00 dww_test-0.0.3.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dww_test-0.0.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1092 b- defN 20-Feb-02 00:00 dww_test-0.0.3.dist-info/licenses/LICENSE.txt
+?rw-r--r--  2.0 unx      616 b- defN 20-Feb-02 00:00 dww_test-0.0.3.dist-info/RECORD
+8 files, 3538 bytes uncompressed, 1998 bytes compressed:  43.5%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: dww_test/dww_test.py
 Comment: 
 
 Filename: dww_test/dww_test.py~
 Comment: 
 
-Filename: dww_test-0.0.2.dist-info/METADATA
+Filename: dww_test-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: dww_test-0.0.2.dist-info/WHEEL
+Filename: dww_test-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: dww_test-0.0.2.dist-info/licenses/LICENSE.txt
+Filename: dww_test-0.0.3.dist-info/licenses/LICENSE.txt
 Comment: 
 
-Filename: dww_test-0.0.2.dist-info/RECORD
+Filename: dww_test-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dww_test/__about__.py

```diff
@@ -1,4 +1,4 @@
 # SPDX-FileCopyrightText: 2023-present U.N. Owen <void@some.where>
 #
 # SPDX-License-Identifier: MIT
-__version__ = "0.0.2"
+__version__ = "0.0.3"
```

## dww_test/dww_test.py

```diff
@@ -1,7 +1,7 @@
 #!/usr/bin/env python
 
 def dwwfunc():
     print("My python module")
 
 if __name__ == "__main__":
-    print("dww test")
+    dww_func()
```

## Comparing `dww_test-0.0.2.dist-info/METADATA` & `dww_test-0.0.3.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dww-test
-Version: 0.0.2
+Version: 0.0.3
 Summary: Hatch test project
 Project-URL: Documentation, https://github.com/unknown/dww-test#readme
 Project-URL: Issues, https://github.com/unknown/dww-test/issues
 Project-URL: Source, https://github.com/unknown/dww-test
 Author-email: "U.N. Owen" <void@some.where>
 License-Expression: MIT
 License-File: LICENSE.txt
```

## Comparing `dww_test-0.0.2.dist-info/licenses/LICENSE.txt` & `dww_test-0.0.3.dist-info/licenses/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `dww_test-0.0.2.dist-info/RECORD` & `dww_test-0.0.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-dww_test/__about__.py,sha256=pczFFwSCJ9Co8bn4nAJreepA92Ohs104CxAeN3sEezA,122
+dww_test/__about__.py,sha256=FIXUSBa-8xqohw6pJjWnzlbevt-Gby9N0mcvNCt3vKA,122
 dww_test/__init__.py,sha256=xbJugSkmU6lnNoLqurj8x3psMLrTzuCVr0f7oG7WvjY,100
-dww_test/dww_test.py,sha256=C8hkXNPkSKLY8A9myXvwMwBXZgIL5Y87uThHqD9c_Z0,118
+dww_test/dww_test.py,sha256=l0Mho8d_b2jkw5IxAggrZAVBNkNqZBYLdTjaxoqnorA,111
 dww_test/dww_test.py~,sha256=bFcNM5_jMqYwiuqwRIoF1UvQnS_-p-mPlK66oujFKVQ,23
-dww_test-0.0.2.dist-info/METADATA,sha256=nTkptkwdapuNBYcsBwrl74o-KnscNV6IQbpeK8PqgHs,1387
-dww_test-0.0.2.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
-dww_test-0.0.2.dist-info/licenses/LICENSE.txt,sha256=jriEt3irvhUMo7cyrB4n2sAgngMzhDTG7n8lhCt-kH4,1092
-dww_test-0.0.2.dist-info/RECORD,,
+dww_test-0.0.3.dist-info/METADATA,sha256=-XIR8bYj4b8lcbUjshL9zq5eTGD42O7n6BL2W32AeHw,1387
+dww_test-0.0.3.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
+dww_test-0.0.3.dist-info/licenses/LICENSE.txt,sha256=jriEt3irvhUMo7cyrB4n2sAgngMzhDTG7n8lhCt-kH4,1092
+dww_test-0.0.3.dist-info/RECORD,,
```

