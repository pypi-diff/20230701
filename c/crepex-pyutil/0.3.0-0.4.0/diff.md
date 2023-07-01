# Comparing `tmp/crepex_pyutil-0.3.0.tar.gz` & `tmp/crepex_pyutil-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crepex_pyutil-0.3.0.tar", max compression
+gzip compressed data, was "crepex_pyutil-0.4.0.tar", max compression
```

## Comparing `crepex_pyutil-0.3.0.tar` & `crepex_pyutil-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      791 2023-04-12 09:41:55.227358 crepex_pyutil-0.3.0/README.md
--rw-r--r--   0        0        0      413 2023-05-15 08:46:56.394050 crepex_pyutil-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-12 06:42:39.752853 crepex_pyutil-0.3.0/src/crepex_pyutil/__init__.py
--rwxr-xr-x   0        0        0     2826 2023-04-13 11:48:15.785079 crepex_pyutil-0.3.0/src/crepex_pyutil/dates.py
--rw-r--r--   0        0        0      664 2023-04-12 05:49:04.763845 crepex_pyutil-0.3.0/src/crepex_pyutil/exceptions.py
--rw-r--r--   0        0        0       81 2023-05-15 08:44:18.527777 crepex_pyutil-0.3.0/src/crepex_pyutil/requests/__init__.py
--rw-r--r--   0        0        0     2107 2023-04-12 06:02:06.720570 crepex_pyutil-0.3.0/src/crepex_pyutil/requests/helper.py
--rw-r--r--   0        0        0     2197 2023-05-15 08:45:17.992026 crepex_pyutil-0.3.0/src/crepex_pyutil/requests/slack.py
--rwxr-xr-x   0        0        0     1726 2023-04-27 01:58:48.842662 crepex_pyutil-0.3.0/src/crepex_pyutil/string.py
--rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 crepex_pyutil-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      791 2023-04-12 09:41:55.227358 crepex_pyutil-0.4.0/README.md
+-rw-r--r--   0        0        0      413 2023-07-01 09:14:15.088437 crepex_pyutil-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 06:42:39.752853 crepex_pyutil-0.4.0/src/crepex_pyutil/__init__.py
+-rwxr-xr-x   0        0        0     3246 2023-07-01 09:13:24.096916 crepex_pyutil-0.4.0/src/crepex_pyutil/dates.py
+-rw-r--r--   0        0        0      712 2023-07-01 09:08:24.771723 crepex_pyutil-0.4.0/src/crepex_pyutil/exceptions.py
+-rw-r--r--   0        0        0       81 2023-05-15 08:44:18.527777 crepex_pyutil-0.4.0/src/crepex_pyutil/requests/__init__.py
+-rw-r--r--   0        0        0     2107 2023-04-12 06:02:06.720570 crepex_pyutil-0.4.0/src/crepex_pyutil/requests/helper.py
+-rw-r--r--   0        0        0     2197 2023-05-15 08:45:17.992026 crepex_pyutil-0.4.0/src/crepex_pyutil/requests/slack.py
+-rwxr-xr-x   0        0        0     1726 2023-04-27 01:58:48.842662 crepex_pyutil-0.4.0/src/crepex_pyutil/string.py
+-rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 crepex_pyutil-0.4.0/PKG-INFO
```

### Comparing `crepex_pyutil-0.3.0/README.md` & `crepex_pyutil-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `crepex_pyutil-0.3.0/src/crepex_pyutil/dates.py` & `crepex_pyutil-0.4.0/src/crepex_pyutil/dates.py`

 * *Files 13% similar despite different names*

```diff
@@ -91,7 +91,20 @@
     주어진 날짜의 주간 시작일과 종료일을 반환
     :param dt: 기준일
     :return: 시작일, 종료일 tuple
     """
     start = (dt - timedelta(days=dt.weekday())).replace(hour=0, minute=0, second=0)
     end = (start + timedelta(days=6)).replace(hour=23, minute=59, second=59)
     return start, end
+
+
+def time_string_to_milliseconds(time_string):
+    """
+    "시:분:초" 형식의 문자열을 millisecond 단위의 정수로 변경하여 반환
+    :param time_string: 시간 문자열
+    :return: millisecond 정수
+    """
+    hours, minutes, seconds = time_string.split(":")
+    total_milliseconds = (
+        int(hours) * 3600000 + int(minutes) * 60000 + int(seconds) * 1000
+    )
+    return total_milliseconds
```

### Comparing `crepex_pyutil-0.3.0/src/crepex_pyutil/exceptions.py` & `crepex_pyutil-0.4.0/src/crepex_pyutil/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 class CodeMessageException(Exception):
     """
     내부 모듈에 사용
     """
 
     def __init__(self, code, msg):
+        self.code = code
+        self.msg = msg
         message = f"code{code}.{msg}"
         super().__init__(message)
 
 
 class LoginException(CodeMessageException):
     def __init__(self, code: int):
         super().__init__(code, msg="로그인 실패")
```

### Comparing `crepex_pyutil-0.3.0/src/crepex_pyutil/requests/helper.py` & `crepex_pyutil-0.4.0/src/crepex_pyutil/requests/helper.py`

 * *Files identical despite different names*

### Comparing `crepex_pyutil-0.3.0/src/crepex_pyutil/requests/slack.py` & `crepex_pyutil-0.4.0/src/crepex_pyutil/requests/slack.py`

 * *Files identical despite different names*

### Comparing `crepex_pyutil-0.3.0/src/crepex_pyutil/string.py` & `crepex_pyutil-0.4.0/src/crepex_pyutil/string.py`

 * *Files identical despite different names*

### Comparing `crepex_pyutil-0.3.0/PKG-INFO` & `crepex_pyutil-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crepex-pyutil
-Version: 0.3.0
+Version: 0.4.0
 Summary: CrepeX python utilities
 Author: Hyunwoo Shim
 Author-email: hyunwoo.shim@crepe-x.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

