# Comparing `tmp/xia_user-0.1.31-cp39-none-win_amd64.whl.zip` & `tmp/xia_user-0.1.32-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9664 bytes, number of entries: 9
--rw-r--r--  2.0 unx      363 b- defN 23-Jun-30 11:41 xia_user/__init__.py
+Zip file size: 9665 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      363 b- defN 23-Jul-01 18:11 xia_user/__init__.py
 -rw-r--r--  2.0 unx      887 b- defN 23-Jun-29 20:17 xia_user/messages.py
 -rw-r--r--  2.0 unx     9660 b- defN 23-Jun-29 20:17 xia_user/role_matrix.py
 -rw-r--r--  2.0 unx    19323 b- defN 23-Jun-29 20:17 xia_user/user.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:46 xia_user-0.1.31.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      734 b- defN 23-Jun-30 11:46 xia_user-0.1.31.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:46 xia_user-0.1.31.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-30 11:46 xia_user-0.1.31.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      703 b- defN 23-Jun-30 11:46 xia_user-0.1.31.dist-info/RECORD
-9 files, 31929 bytes uncompressed, 8454 bytes compressed:  73.5%
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 18:14 xia_user-0.1.32.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      734 b- defN 23-Jul-01 18:14 xia_user-0.1.32.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 18:14 xia_user-0.1.32.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-01 18:14 xia_user-0.1.32.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      703 b- defN 23-Jul-01 18:14 xia_user-0.1.32.dist-info/RECORD
+9 files, 31929 bytes uncompressed, 8455 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: xia_user/role_matrix.py
 Comment: 
 
 Filename: xia_user/user.py
 Comment: 
 
-Filename: xia_user-0.1.31.dist-info/LICENSE.txt
+Filename: xia_user-0.1.32.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_user-0.1.31.dist-info/METADATA
+Filename: xia_user-0.1.32.dist-info/METADATA
 Comment: 
 
-Filename: xia_user-0.1.31.dist-info/WHEEL
+Filename: xia_user-0.1.32.dist-info/WHEEL
 Comment: 
 
-Filename: xia_user-0.1.31.dist-info/top_level.txt
+Filename: xia_user-0.1.32.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_user-0.1.31.dist-info/RECORD
+Filename: xia_user-0.1.32.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_user/__init__.py

```diff
@@ -6,8 +6,8 @@
 __all__ = [
     "UserBasicInfo", "AppNameField",
     "User", "UserRoles", "ApiInfo", "ApiKey",
     "RoleMatrix", "RoleContent", "Policy", "Group"
 ]
 
 
-__version__ = "0.1.31"
+__version__ = "0.1.32"
```

## Comparing `xia_user-0.1.31.dist-info/METADATA` & `xia_user-0.1.32.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-user
-Version: 0.1.31
+Version: 0.1.32
 Summary: xia-user
-Home-page: https://develop.x-i-a.com/docs/xia-user/0.1.31/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-user/0.1.32/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_user-0.1.31.dist-info/RECORD` & `xia_user-0.1.32.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-xia_user/__init__.py,sha256=G5FpK4TBC-g_q_cSGFZ7ScJWArxkjo7kUHuNXNBLJCc,363
+xia_user/__init__.py,sha256=QYTacvBENES63iP47sf9msP3-LM_K9OOy4pqFIN8Xsg,363
 xia_user/messages.py,sha256=f0naN8nMvBbXnhZZn71myynbYdqT4DaXp3EzkEPqT0o,887
 xia_user/role_matrix.py,sha256=F8g5jVg1f9FeKoPpBFFFcS_mvrl54MaspY1EXN-Jn1Y,9660
 xia_user/user.py,sha256=h3xEjz2cOqK0ikd4ZgIKu-NSyjay4VhtXU0bSkly7VI,19323
-xia_user-0.1.31.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
-xia_user-0.1.31.dist-info/METADATA,sha256=-IiFGIwY1VPQHEMT-1xjWQsPiE9zJ27V8qQ-n2C8GN4,734
-xia_user-0.1.31.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_user-0.1.31.dist-info/top_level.txt,sha256=83bMsRCwFtrpI8U1LNGqnyMAROolkm0ssQ1MveXgEBo,9
-xia_user-0.1.31.dist-info/RECORD,,
+xia_user-0.1.32.dist-info/LICENSE.txt,sha256=VI2DRhUdOX7ADnFkyNfO3YiExtoLHTFKKd8XFlFAbWw,151
+xia_user-0.1.32.dist-info/METADATA,sha256=_kNU3S3oePC3bd6iV8pAZTm8rsg3otgrdCI64KMmsrE,734
+xia_user-0.1.32.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_user-0.1.32.dist-info/top_level.txt,sha256=83bMsRCwFtrpI8U1LNGqnyMAROolkm0ssQ1MveXgEBo,9
+xia_user-0.1.32.dist-info/RECORD,,
```

