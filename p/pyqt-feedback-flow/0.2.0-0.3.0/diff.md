# Comparing `tmp/pyqt-feedback-flow-0.2.0.tar.gz` & `tmp/pyqt-feedback-flow-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt-feedback-flow-0.2.0.tar", max compression
+gzip compressed data, was "pyqt-feedback-flow-0.3.0.tar", max compression
```

## Comparing `pyqt-feedback-flow-0.2.0.tar` & `pyqt-feedback-flow-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-03-25 18:32:48.740993 pyqt-feedback-flow-0.2.0/LICENSE
--rw-r--r--   0        0        0     3082 2023-03-25 18:32:48.741993 pyqt-feedback-flow-0.2.0/README.md
--rw-r--r--   0        0        0      586 2023-03-25 18:32:48.745993 pyqt-feedback-flow-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-03-25 18:32:48.745993 pyqt-feedback-flow-0.2.0/pyqt_feedback_flow/__init__.py
--rw-r--r--   0        0        0     9078 2023-03-25 18:32:48.745993 pyqt-feedback-flow-0.2.0/pyqt_feedback_flow/feedback.py
--rw-r--r--   0        0        0     3874 2023-03-25 18:35:43.283371 pyqt-feedback-flow-0.2.0/setup.py
--rw-r--r--   0        0        0     3691 2023-03-25 18:35:43.283556 pyqt-feedback-flow-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-01 18:47:06.198295 pyqt-feedback-flow-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3082 2023-07-01 18:47:06.198295 pyqt-feedback-flow-0.3.0/README.md
+-rw-r--r--   0        0        0      585 2023-07-01 18:47:06.202295 pyqt-feedback-flow-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-01 18:47:06.202295 pyqt-feedback-flow-0.3.0/pyqt_feedback_flow/__init__.py
+-rw-r--r--   0        0        0     9203 2023-07-01 18:47:06.202295 pyqt-feedback-flow-0.3.0/pyqt_feedback_flow/feedback.py
+-rw-r--r--   0        0        0     3873 2023-07-01 18:47:12.232478 pyqt-feedback-flow-0.3.0/setup.py
+-rw-r--r--   0        0        0     3690 2023-07-01 18:47:12.232677 pyqt-feedback-flow-0.3.0/PKG-INFO
```

### Comparing `pyqt-feedback-flow-0.2.0/LICENSE` & `pyqt-feedback-flow-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqt-feedback-flow-0.2.0/README.md` & `pyqt-feedback-flow-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyqt-feedback-flow-0.2.0/pyproject.toml` & `pyqt-feedback-flow-0.3.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "pyqt-feedback-flow"
-version = "0.2.0"
+version = "0.3.0"
 description = "Show feedback in toast-like notifications"
 authors = ["Iztok Fister Jr. <iztok@iztok-jr-fister.eu>", "Luka Lukač <luka.lukac@student.um.si>"]
 homepage = "https://github.com/firefly-cpp/pyqt-feedback-flow"
 repository = "https://github.com/firefly-cpp/pyqt-feedback-flow"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-PyQt5 = "^5.15.6"
-emoji = "^2.2.0"
+PyQt6 = "^6.4.2"
+emoji = "^2.6.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyqt-feedback-flow-0.2.0/pyqt_feedback_flow/feedback.py` & `pyqt-feedback-flow-0.3.0/pyqt_feedback_flow/feedback.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from enum import Enum
-from PyQt5.QtCore import QEasingCurve, QPoint, QPropertyAnimation, Qt
-from PyQt5.QtGui import QPixmap
-from PyQt5.QtSvg import QSvgWidget
-from PyQt5.QtWidgets import QApplication, QLabel, QVBoxLayout, QWidget
+from PyQt6 import QtGui
+from PyQt6.QtCore import QEasingCurve, QPoint, QPropertyAnimation, Qt
+from PyQt6.QtGui import QPixmap
+from PyQt6.QtSvgWidgets import QSvgWidget
+from PyQt6.QtWidgets import QApplication, QLabel, QVBoxLayout, QWidget
 
 
 class AnimationType(Enum):
     """
     Enumeration class for the type of the animation.
     """
     VERTICAL = 0
@@ -33,27 +34,27 @@
         """
         Initialisation method for Feedback class.\n
         Args:
             width (int): width of the notification
             height (int): height of the notification
         """
         super(_Feedback, self).__init__()
-        self.setWindowFlags(Qt.FramelessWindowHint |
-                            Qt.WindowStaysOnTopHint |
-                            Qt.X11BypassWindowManagerHint)
-        self.setAttribute(Qt.WA_TranslucentBackground)
+        self.setWindowFlags(Qt.WindowType.FramelessWindowHint |
+                            Qt.WindowType.WindowStaysOnTopHint |
+                            Qt.WindowType.X11BypassWindowManagerHint)
+        self.setAttribute(Qt.WidgetAttribute.WA_TranslucentBackground)
         self.layout = QVBoxLayout(self)
         self.notification_width = width
         self.notification_height = height
 
     def show(self,
              type_of_animation: int,
              animation_direction: int,
              time: int = 3000,
-             curve: int = QEasingCurve.OutInQuart) -> None:
+             curve: int = QEasingCurve(QEasingCurve.Type.OutInQuart)) -> None:
         """
         Method for displaying a toast notification.\n
         Args:
             type_of_animation (int): one of the preset types of animations
                                      in AnimationType enum class
             animation_direction (int): one of the preset directions of
                                        animations in AnimationDirection
@@ -105,15 +106,15 @@
                   animation_direction == AnimationDirection.DOWN):
                 start = QPoint(0, 0)
                 end = QPoint(width - self.notification_width,
                              height - self.notification_height)
             else:
                 raise Exception("""Incorrect combination of animation
                                    type and direction.""")
-        # Antidiagonal animation.
+        # Anti diagonal animation.
         elif type_of_animation == AnimationType.ANTI_DIAGONAL:
             if animation_direction == AnimationDirection.RIGHT or \
                animation_direction == AnimationDirection.UP:
                 start = QPoint(0, height - self.notification_height)
                 end = QPoint(width - self.notification_width, 0)
             elif (animation_direction == AnimationDirection.LEFT or
                   animation_direction == AnimationDirection.DOWN):
@@ -144,15 +145,15 @@
         self.start_flow.setDuration(time)
         self.start_flow.finished.connect(self.close)
 
         # Animation of the opacity of the notification.
         self.start_opacity = QPropertyAnimation(self, b'windowOpacity')
         self.start_opacity.setStartValue(1)
         self.start_opacity.setEndValue(0)
-        self.start_opacity.setEasingCurve(QEasingCurve.InQuint)
+        self.start_opacity.setEasingCurve(QEasingCurve.Type.InQuint)
         self.start_opacity.setDuration(time)
 
         self.start_flow.start()
         self.start_opacity.start()
 
 
 class ImageFeedback(_Feedback):
@@ -183,15 +184,15 @@
             self.vector.setFixedSize(width, height)
             self.layout.addWidget(self.vector)
         # If the image is raster, it is opened with QPixmap.
         else:
             pixmap = QPixmap(self.img).scaled(
                 width,
                 height,
-                transformMode=Qt.SmoothTransformation)
+                transformMode=Qt.ImageConversionFlag.SmoothTransformation)
             self.label = QLabel(self)
             self.layout.addWidget(self.label)
             self.label.setPixmap(pixmap)
 
 
 class TextFeedback(_Feedback):
     """
```

### Comparing `pyqt-feedback-flow-0.2.0/setup.py` & `pyqt-feedback-flow-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['pyqt_feedback_flow']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['PyQt5>=5.15.6,<6.0.0', 'emoji>=2.2.0,<3.0.0']
+['PyQt6>=6.4.2,<7.0.0', 'emoji>=2.6.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'pyqt-feedback-flow',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Show feedback in toast-like notifications',
     'long_description': '# pyqt-feedback-flow --- Show feedback in toast-like notifications\n\n---\n\n[![PyPI Version](https://img.shields.io/pypi/v/pyqt-feedback-flow.svg)](https://pypi.python.org/pypi/pyqt-feedback-flow)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyqt-feedback-flow.svg)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/pyqt-feedback-flow.svg)\n[![Downloads](https://pepy.tech/badge/pyqt-feedback-flow)](https://pepy.tech/project/pyqt-feedback-flow)\n[![GitHub license](https://img.shields.io/github/license/firefly-cpp/pyqt-feedback-flow.svg)](https://github.com/firefly-cpp/pyqt-feedback-flow/blob/master/LICENSE)\n![GitHub commit activity](https://img.shields.io/github/commit-activity/w/firefly-cpp/pyqt-feedback-flow.svg)\n[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/firefly-cpp/pyqt-feedback-flow.svg)](http://isitmaintained.com/project/firefly-cpp/pyqt-feedback-flow "Average time to resolve an issue")\n[![Percentage of issues still open](http://isitmaintained.com/badge/open/firefly-cpp/pyqt-feedback-flow.svg)](http://isitmaintained.com/project/firefly-cpp/pyqt-feedback-flow "Percentage of issues still open")\n[![Fedora package](https://img.shields.io/fedora/v/python3-pyqt-feedback-flow?color=blue&label=Fedora%20Linux&logo=fedora)](https://src.fedoraproject.org/rpms/python-pyqt-feedback-flow)\n\n![Pyqt](https://user-images.githubusercontent.com/73126820/167383927-6fe17311-4e80-42fc-a0ef-1494b4c58762.png)\n\n## Description\nOn many occasions, notifications can be a valuable tool to inform a user about specific events. Sometimes, static notifications or pop-up windows may provide adequate feedback; however, there are some cases where flowing notifications can be more appropriate.\n\nThis software allows us to show flowing notifications in the realm of a text or a picture. Both text and pictures (raster and vector) can be customized according to users\' wishes, which offers a wide variety of possibilities for providing flowing feedback.\n\n## Text notification example\nhttps://user-images.githubusercontent.com/73126820/167379237-7c85467d-133e-42c9-91fd-7e85f2481267.mp4\n\n## Image notification example\nhttps://user-images.githubusercontent.com/73126820/167380818-814cc1ce-d137-4906-b5a4-84af94c46d4a.mp4\n\n## Installation\n\n### pip\n\nInstall this software with pip:\n\n```sh\npip install pyqt-feedback-flow\n```\n\n### Alpine Linux\n\nTo install pyqt-feedback-flow on Alpine Linux, use:\n\n```sh\n$ apk add py3-pyqt-feedback-flow\n```\n\n### Arch Linux\n\nTo install pyqt-feedback-flow on Arch Linux, please use an [AUR helper](https://wiki.archlinux.org/title/AUR_helpers):\n\n```sh\n$ yay -Syyu python-pyqt-feedback-flow\n```\n\n### Fedora Linux\n\nTo install pyqt-feedback-flow on Fedora Linux, use:\n\n```sh\n$ dnf install python3-pyqt-feedback-flow\n```\n\n## License\n\nThis package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.\n\n## Disclaimer\n\nThis framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!\n',
     'author': 'Iztok Fister Jr.',
     'author_email': 'iztok@iztok-jr-fister.eu',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/firefly-cpp/pyqt-feedback-flow',
```

### Comparing `pyqt-feedback-flow-0.2.0/PKG-INFO` & `pyqt-feedback-flow-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pyqt-feedback-flow
-Version: 0.2.0
+Version: 0.3.0
 Summary: Show feedback in toast-like notifications
 Home-page: https://github.com/firefly-cpp/pyqt-feedback-flow
 Author: Iztok Fister Jr.
 Author-email: iztok@iztok-jr-fister.eu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: PyQt5 (>=5.15.6,<6.0.0)
-Requires-Dist: emoji (>=2.2.0,<3.0.0)
+Requires-Dist: PyQt6 (>=6.4.2,<7.0.0)
+Requires-Dist: emoji (>=2.6.0,<3.0.0)
 Project-URL: Repository, https://github.com/firefly-cpp/pyqt-feedback-flow
 Description-Content-Type: text/markdown
 
 # pyqt-feedback-flow --- Show feedback in toast-like notifications
 
 ---
```

