# Comparing `tmp/cv2filters-0.1.1.tar.gz` & `tmp/cv2filters-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cv2filters-0.1.1.tar", last modified: Sat Jul  1 14:45:13 2023, max compression
+gzip compressed data, was "cv2filters-0.1.2.tar", last modified: Sat Jul  1 15:26:53 2023, max compression
```

## Comparing `cv2filters-0.1.1.tar` & `cv2filters-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:45:13.689154 cv2filters-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-07-01 14:45:13.689154 cv2filters-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-07-01 14:44:54.000000 cv2filters-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:45:13.689154 cv2filters-0.1.1/cv2filters/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-01 14:44:54.000000 cv2filters-0.1.1/cv2filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16204 2023-07-01 14:44:54.000000 cv2filters-0.1.1/cv2filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:45:13.689154 cv2filters-0.1.1/cv2filters.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-07-01 14:45:13.000000 cv2filters-0.1.1/cv2filters.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-01 14:45:13.000000 cv2filters-0.1.1/cv2filters.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 14:45:13.000000 cv2filters-0.1.1/cv2filters.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-01 14:45:13.000000 cv2filters-0.1.1/cv2filters.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-01 14:45:13.000000 cv2filters-0.1.1/cv2filters.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 14:45:13.689154 cv2filters-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-01 14:44:54.000000 cv2filters-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:26:53.965485 cv2filters-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-01 15:26:34.000000 cv2filters-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-07-01 15:26:53.965485 cv2filters-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-07-01 15:26:34.000000 cv2filters-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:26:53.965485 cv2filters-0.1.2/cv2filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-01 15:26:34.000000 cv2filters-0.1.2/cv2filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16204 2023-07-01 15:26:34.000000 cv2filters-0.1.2/cv2filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:26:53.965485 cv2filters-0.1.2/cv2filters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-07-01 15:26:53.000000 cv2filters-0.1.2/cv2filters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-01 15:26:53.000000 cv2filters-0.1.2/cv2filters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 15:26:53.000000 cv2filters-0.1.2/cv2filters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-01 15:26:53.000000 cv2filters-0.1.2/cv2filters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-01 15:26:53.000000 cv2filters-0.1.2/cv2filters.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 15:26:53.965485 cv2filters-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-01 15:26:34.000000 cv2filters-0.1.2/setup.py
```

### Comparing `cv2filters-0.1.1/PKG-INFO` & `cv2filters-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,26 @@
-Metadata-Version: 2.1
-Name: cv2filters
-Version: 0.1.1
-Summary:  OpenCv Wrapper that simplifies image processing with OpenCV, making it accessible to users of all skill levels
-Home-page: https://github.com/nuhmanpk/cv2filters
-Author: Nuhman Pk
-Author-email: nuhmanpk7@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # CV2Filters
 
 CV2Filters a powerful Python package designed as a wrapper around OpenCV, the popular open-source computer vision library. cv2Filters simplifies image processing tasks by providing a higher-level abstraction of the underlying OpenCV functionality. This package aims to make image processing more accessible to both beginner and advanced users, enabling them to efficiently perform a wide range of image manipulation and analysis tasks
 
 CV2Filters empowers users to harness the power of OpenCV in a simplified and intuitive manner. By abstracting away the complexities, the package enables a broader audience to explore image processing, drive innovation, and unlock new possibilities in the field of computer vision.
 
+[![Downloads](https://static.pepy.tech/personalized-badge/cv2filters?period=total&units=international_system&left_color=grey&right_color=yellow&left_text=Total-Downloads)](https://pepy.tech/project/cv2filters)
+![PyPI - Format](https://img.shields.io/pypi/format/cv2filters)
+[![GitHub license](https://img.shields.io/github/license/nuhmanpk/cv2filters.svg)](https://github.com/nuhmanpk/cv2filters/blob/main/LICENSE)
+[![Upload Python Package](https://github.com/nuhmanpk/cv2filters/actions/workflows/publish.yml/badge.svg)](https://github.com/nuhmanpk/cv2filters/actions/workflows/publish.yml)
+[![Supported Versions](https://img.shields.io/pypi/pyversions/cv2filters.svg)](https://pypi.org/project/cv2filters)
+![PyPI](https://img.shields.io/pypi/v/cv2filters)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/cv2filters)
+[![Downloads](https://static.pepy.tech/personalized-badge/cv2filters?period=week&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads/Week)](https://pepy.tech/project/cv2filters)
+
 ## Installation
 
+[Refer Example](https://github.com/nuhmanpk/cv2filters/wiki) 
+
 To install the library, you can use pip:
 
 ```shell
 pip install cv2filters
 ```
 
 ## Usage
@@ -39,14 +35,15 @@
 
 or
 
 ```python
 from cv2filters.filters import <function-to-be-used>
 ```
 
+
 Now you can use the various filtering functions available in the library. For example, let's show how to use the increase_brightness and apply_blur functions:
 
 ```python
 from cv2filters.filters import increase_brightness, apply_blur
 import cv2
 
 image = cv2.imread('image.jpg')
@@ -185,9 +182,7 @@
 
 If you'd like to contribute to this library, please follow these steps:
 
 * Fork the repository.
 * Create a new branch.
 * Make your changes and test them.
 * Submit a pull request.
-
-
```

### Comparing `cv2filters-0.1.1/README.md` & `cv2filters-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,42 @@
+Metadata-Version: 2.1
+Name: cv2filters
+Version: 0.1.2
+Summary:  Unleash the power of OpenCV with CV2Filters, the ultimate image processing wrapper for all skill levels, revolutionizing computer vision with seamless exploration, manipulation, and groundbreaking research
+Home-page: https://github.com/nuhmanpk/cv2filters
+Author: Nuhman Pk
+Author-email: nuhmanpk7@gmail.com
+License: MIT
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # CV2Filters
 
 CV2Filters a powerful Python package designed as a wrapper around OpenCV, the popular open-source computer vision library. cv2Filters simplifies image processing tasks by providing a higher-level abstraction of the underlying OpenCV functionality. This package aims to make image processing more accessible to both beginner and advanced users, enabling them to efficiently perform a wide range of image manipulation and analysis tasks
 
 CV2Filters empowers users to harness the power of OpenCV in a simplified and intuitive manner. By abstracting away the complexities, the package enables a broader audience to explore image processing, drive innovation, and unlock new possibilities in the field of computer vision.
 
+[![Downloads](https://static.pepy.tech/personalized-badge/cv2filters?period=total&units=international_system&left_color=grey&right_color=yellow&left_text=Total-Downloads)](https://pepy.tech/project/cv2filters)
+![PyPI - Format](https://img.shields.io/pypi/format/cv2filters)
+[![GitHub license](https://img.shields.io/github/license/nuhmanpk/cv2filters.svg)](https://github.com/nuhmanpk/cv2filters/blob/main/LICENSE)
+[![Upload Python Package](https://github.com/nuhmanpk/cv2filters/actions/workflows/publish.yml/badge.svg)](https://github.com/nuhmanpk/cv2filters/actions/workflows/publish.yml)
+[![Supported Versions](https://img.shields.io/pypi/pyversions/cv2filters.svg)](https://pypi.org/project/cv2filters)
+![PyPI](https://img.shields.io/pypi/v/cv2filters)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/cv2filters)
+[![Downloads](https://static.pepy.tech/personalized-badge/cv2filters?period=week&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads/Week)](https://pepy.tech/project/cv2filters)
+
 ## Installation
 
+[Refer Example](https://github.com/nuhmanpk/cv2filters/wiki) 
+
 To install the library, you can use pip:
 
 ```shell
 pip install cv2filters
 ```
 
 ## Usage
@@ -24,14 +51,15 @@
 
 or
 
 ```python
 from cv2filters.filters import <function-to-be-used>
 ```
 
+
 Now you can use the various filtering functions available in the library. For example, let's show how to use the increase_brightness and apply_blur functions:
 
 ```python
 from cv2filters.filters import increase_brightness, apply_blur
 import cv2
 
 image = cv2.imread('image.jpg')
@@ -170,7 +198,9 @@
 
 If you'd like to contribute to this library, please follow these steps:
 
 * Fork the repository.
 * Create a new branch.
 * Make your changes and test them.
 * Submit a pull request.
+
+
```

### Comparing `cv2filters-0.1.1/cv2filters/filters.py` & `cv2filters-0.1.2/cv2filters/filters.py`

 * *Files identical despite different names*

### Comparing `cv2filters-0.1.1/cv2filters.egg-info/PKG-INFO` & `cv2filters-0.1.2/cv2filters.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,42 @@
 Metadata-Version: 2.1
 Name: cv2filters
-Version: 0.1.1
-Summary:  OpenCv Wrapper that simplifies image processing with OpenCV, making it accessible to users of all skill levels
+Version: 0.1.2
+Summary:  Unleash the power of OpenCV with CV2Filters, the ultimate image processing wrapper for all skill levels, revolutionizing computer vision with seamless exploration, manipulation, and groundbreaking research
 Home-page: https://github.com/nuhmanpk/cv2filters
 Author: Nuhman Pk
 Author-email: nuhmanpk7@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # CV2Filters
 
 CV2Filters a powerful Python package designed as a wrapper around OpenCV, the popular open-source computer vision library. cv2Filters simplifies image processing tasks by providing a higher-level abstraction of the underlying OpenCV functionality. This package aims to make image processing more accessible to both beginner and advanced users, enabling them to efficiently perform a wide range of image manipulation and analysis tasks
 
 CV2Filters empowers users to harness the power of OpenCV in a simplified and intuitive manner. By abstracting away the complexities, the package enables a broader audience to explore image processing, drive innovation, and unlock new possibilities in the field of computer vision.
 
+[![Downloads](https://static.pepy.tech/personalized-badge/cv2filters?period=total&units=international_system&left_color=grey&right_color=yellow&left_text=Total-Downloads)](https://pepy.tech/project/cv2filters)
+![PyPI - Format](https://img.shields.io/pypi/format/cv2filters)
+[![GitHub license](https://img.shields.io/github/license/nuhmanpk/cv2filters.svg)](https://github.com/nuhmanpk/cv2filters/blob/main/LICENSE)
+[![Upload Python Package](https://github.com/nuhmanpk/cv2filters/actions/workflows/publish.yml/badge.svg)](https://github.com/nuhmanpk/cv2filters/actions/workflows/publish.yml)
+[![Supported Versions](https://img.shields.io/pypi/pyversions/cv2filters.svg)](https://pypi.org/project/cv2filters)
+![PyPI](https://img.shields.io/pypi/v/cv2filters)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/cv2filters)
+[![Downloads](https://static.pepy.tech/personalized-badge/cv2filters?period=week&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads/Week)](https://pepy.tech/project/cv2filters)
+
 ## Installation
 
+[Refer Example](https://github.com/nuhmanpk/cv2filters/wiki) 
+
 To install the library, you can use pip:
 
 ```shell
 pip install cv2filters
 ```
 
 ## Usage
@@ -39,14 +51,15 @@
 
 or
 
 ```python
 from cv2filters.filters import <function-to-be-used>
 ```
 
+
 Now you can use the various filtering functions available in the library. For example, let's show how to use the increase_brightness and apply_blur functions:
 
 ```python
 from cv2filters.filters import increase_brightness, apply_blur
 import cv2
 
 image = cv2.imread('image.jpg')
```

### Comparing `cv2filters-0.1.1/setup.py` & `cv2filters-0.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 
 file = pathlib.Path(__file__).parent
 
 README = (file / "README.md").read_text()
 
 setuptools.setup(
     name="cv2filters",
-    version="0.1.1",
+    version="0.1.2",
     author="Nuhman Pk",
     author_email="nuhmanpk7@gmail.com",
     long_description = README,
     long_description_content_type = "text/markdown",
-    description=" OpenCv Wrapper that simplifies image processing with OpenCV, making it accessible to users of all skill levels",
+    description=" Unleash the power of OpenCV with CV2Filters, the ultimate image processing wrapper for all skill levels, revolutionizing computer vision with seamless exploration, manipulation, and groundbreaking research",
     license="MIT",
     url="https://github.com/nuhmanpk/cv2filters",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(include=['cv2filters']),  
     install_requires=[
         'opencv_python'
     ],
     
     python_requires=">=3.6",
     
-)
+)
```

