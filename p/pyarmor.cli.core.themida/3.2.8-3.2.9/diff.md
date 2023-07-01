# Comparing `tmp/pyarmor.cli.core.themida-3.2.8-cp39-none-any.whl.zip` & `tmp/pyarmor.cli.core.themida-3.2.9-cp39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7727798 bytes, number of entries: 7
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-23 10:06 pyarmor/cli/core/themida/__init__.py
--rwxr-xr-x  2.0 unx  3844126 b- defN 23-Jun-23 10:06 pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd
--rwxr-xr-x  2.0 unx  4827152 b- defN 23-Jun-23 10:06 pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd
--rw-r--r--  2.0 unx      809 b- defN 23-Jun-23 10:06 pyarmor.cli.core.themida-3.2.8.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-23 10:06 pyarmor.cli.core.themida-3.2.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-23 10:06 pyarmor.cli.core.themida-3.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      690 b- defN 23-Jun-23 10:06 pyarmor.cli.core.themida-3.2.8.dist-info/RECORD
-7 files, 8672900 bytes uncompressed, 7726550 bytes compressed:  10.9%
+Zip file size: 8245848 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-01 01:14 pyarmor/cli/core/themida/__init__.py
+-rwxr-xr-x  2.0 unx  4075038 b- defN 23-Jul-01 01:14 pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd
+-rwxr-xr-x  2.0 unx  5125136 b- defN 23-Jul-01 01:14 pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd
+-rw-r--r--  2.0 unx      809 b- defN 23-Jul-01 01:14 pyarmor.cli.core.themida-3.2.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       93 b- defN 23-Jul-01 01:14 pyarmor.cli.core.themida-3.2.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-01 01:14 pyarmor.cli.core.themida-3.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      690 b- defN 23-Jul-01 01:14 pyarmor.cli.core.themida-3.2.9.dist-info/RECORD
+7 files, 9201796 bytes uncompressed, 8244600 bytes compressed:  10.4%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd
 Comment: 
 
 Filename: pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd
 Comment: 
 
-Filename: pyarmor.cli.core.themida-3.2.8.dist-info/METADATA
+Filename: pyarmor.cli.core.themida-3.2.9.dist-info/METADATA
 Comment: 
 
-Filename: pyarmor.cli.core.themida-3.2.8.dist-info/WHEEL
+Filename: pyarmor.cli.core.themida-3.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: pyarmor.cli.core.themida-3.2.8.dist-info/top_level.txt
+Filename: pyarmor.cli.core.themida-3.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pyarmor.cli.core.themida-3.2.8.dist-info/RECORD
+Filename: pyarmor.cli.core.themida-3.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyarmor/cli/core/themida/__init__.py

```diff
@@ -1 +1 @@
-__VERSION__ = '3.2.8'
+__VERSION__ = '3.2.9'
```

## Comparing `pyarmor.cli.core.themida-3.2.8.dist-info/METADATA` & `pyarmor.cli.core.themida-3.2.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarmor.cli.core.themida
-Version: 3.2.8
+Version: 3.2.9
 Summary: Provide pre-built extension module `pyarmor_runtime` protected by Themida for Pyarmor
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pyarmor.cli.core.themida-3.2.8.dist-info/RECORD` & `pyarmor.cli.core.themida-3.2.9.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-pyarmor/cli/core/themida/__init__.py,sha256=PG51kpFg0wVpa349hmCcuGnAthuwDOr30Fft4rWT9MI,22
-pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd,sha256=mOjCebhUKOvXeU6bFtvoo3fzHJ7s7f1s1cx8BGAX-BQ,3844126
-pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd,sha256=IGgP6ZcqHMrfN5Mcho1wpJ9_ZYjnKqq3YfdkvErbw2g,4827152
-pyarmor.cli.core.themida-3.2.8.dist-info/METADATA,sha256=GtYJfVpgdQJzhq9ASXok_caaUdEkxRsPAh1qndDcqDo,809
-pyarmor.cli.core.themida-3.2.8.dist-info/WHEEL,sha256=QbbyyBnlPXzoGKd-349G69XkCwSd1NFnt4kuAN58gNs,93
-pyarmor.cli.core.themida-3.2.8.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
-pyarmor.cli.core.themida-3.2.8.dist-info/RECORD,,
+pyarmor/cli/core/themida/__init__.py,sha256=vbtJ2fWzIv5Bzsv7yVH47Dtk4RGUCTWnE2pl091zBUY,22
+pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd,sha256=T5d7xmkSyaMcJdSpxT6XMtqK--UyYkWe33qtyNL_enA,4075038
+pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd,sha256=RYrmd-7DvkMi8Gv2Abl6GB8V3IJaXZXa6VDSeCPp6Sc,5125136
+pyarmor.cli.core.themida-3.2.9.dist-info/METADATA,sha256=b9SDClkhCPXrSf704brS2rDKbbLPlZ-axYqeygaJ44w,809
+pyarmor.cli.core.themida-3.2.9.dist-info/WHEEL,sha256=QbbyyBnlPXzoGKd-349G69XkCwSd1NFnt4kuAN58gNs,93
+pyarmor.cli.core.themida-3.2.9.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
+pyarmor.cli.core.themida-3.2.9.dist-info/RECORD,,
```

