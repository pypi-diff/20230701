# Comparing `tmp/translucenttb-0.0.2.tar.gz` & `tmp/translucenttb-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translucenttb-0.0.2.tar", last modified: Sat Jul  1 02:55:29 2023, max compression
+gzip compressed data, was "translucenttb-0.0.3.tar", last modified: Sat Jul  1 04:46:19 2023, max compression
```

## Comparing `translucenttb-0.0.2.tar` & `translucenttb-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:55:29.314081 translucenttb-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-01 02:55:29.310081 translucenttb-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-01 02:55:10.000000 translucenttb-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-01 02:55:10.000000 translucenttb-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 02:55:29.314081 translucenttb-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-01 02:55:10.000000 translucenttb-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:55:29.310081 translucenttb-0.0.2/translucenttb/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-01 02:55:10.000000 translucenttb-0.0.2/translucenttb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-01 02:55:10.000000 translucenttb-0.0.2/translucenttb/blur.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-01 02:55:10.000000 translucenttb-0.0.2/translucenttb/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:55:29.310081 translucenttb-0.0.2/translucenttb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-01 02:55:29.000000 translucenttb-0.0.2/translucenttb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-01 02:55:29.000000 translucenttb-0.0.2/translucenttb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 02:55:29.000000 translucenttb-0.0.2/translucenttb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-01 02:55:29.000000 translucenttb-0.0.2/translucenttb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 04:46:19.934819 translucenttb-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-01 04:46:19.934819 translucenttb-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-01 04:45:56.000000 translucenttb-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-01 04:45:56.000000 translucenttb-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 04:46:19.934819 translucenttb-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-01 04:45:56.000000 translucenttb-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 04:46:19.934819 translucenttb-0.0.3/translucenttb/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-01 04:45:56.000000 translucenttb-0.0.3/translucenttb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-01 04:45:56.000000 translucenttb-0.0.3/translucenttb/blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-01 04:45:56.000000 translucenttb-0.0.3/translucenttb/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 04:46:19.934819 translucenttb-0.0.3/translucenttb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-01 04:46:19.000000 translucenttb-0.0.3/translucenttb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-01 04:46:19.000000 translucenttb-0.0.3/translucenttb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 04:46:19.000000 translucenttb-0.0.3/translucenttb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-01 04:46:19.000000 translucenttb-0.0.3/translucenttb.egg-info/top_level.txt
```

### Comparing `translucenttb-0.0.2/translucenttb/blur.py` & `translucenttb-0.0.3/translucenttb/blur.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     blue = HEX[5:7]
     green = HEX[3:5]
     red = HEX[1:3]
     gradientColor = alpha + blue + green + red
     return int(gradientColor, base=16)
 
 
-def blur(blurtype: str = "acrylic", hexColor: bool = False):
+def blur(blurtype: str = "acrylic", hexColor: str = ""):
     hwnd = windll.user32.FindWindowW("Shell_TrayWnd", None)
     accent = ACCENTPOLICY()
     accent.AccentState = 3
 
     gradientColor = 0
 
     accent.AccentFlags = 2
@@ -82,16 +82,15 @@
         DWM_BB_ENABLE = 0x01
         bb = DWM_BLURBEHIND()
         bb.dwFlags = DWM_BB_ENABLE
         bb.fEnable = 1
         bb.hRgnBlur = 1
         windll.dwmapi.DwmEnableBlurBehindWindow(hwnd, byref(bb))
     elif blurtype == "acrylic":
-        accent.AccentState = 4
-
+        accent.AccentState = 3
     accent.GradientColor = gradientColor
 
     data = WINDOWCOMPOSITIONATTRIBDATA()
     data.Attribute = 19
     data.SizeOfData = sizeof(accent)
     data.Data = cast(pointer(accent), POINTER(c_int))
```

