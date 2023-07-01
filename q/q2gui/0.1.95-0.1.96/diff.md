# Comparing `tmp/q2gui-0.1.95.tar.gz` & `tmp/q2gui-0.1.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2gui-0.1.95.tar", max compression
+gzip compressed data, was "q2gui-0.1.96.tar", max compression
```

## Comparing `q2gui-0.1.95.tar` & `q2gui-0.1.96.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    10347 2023-06-21 10:29:20.277459 q2gui-0.1.95/LICENSE
--rw-r--r--   0        0        0      576 2023-06-30 13:41:35.102853 q2gui-0.1.95/pyproject.toml
--rw-r--r--   0        0        0       39 2022-12-11 17:39:14.961644 q2gui-0.1.95/q2gui/__init__.py
--rw-r--r--   0        0        0      892 2022-12-11 17:39:14.961644 q2gui-0.1.95/q2gui/__main__.py
--rw-r--r--   0        0        0        0 2022-12-11 17:39:14.961644 q2gui-0.1.95/q2gui/pyqt6/__init__.py
--rw-r--r--   0        0        0    18395 2023-06-25 14:11:05.710673 q2gui-0.1.95/q2gui/pyqt6/q2app.py
--rw-r--r--   0        0        0    10075 2023-06-25 14:11:17.663886 q2gui-0.1.95/q2gui/pyqt6/q2form.py
--rw-r--r--   0        0        0      934 2023-06-25 14:11:34.825464 q2gui-0.1.95/q2gui/pyqt6/q2model.py
--rw-r--r--   0        0        0    10507 2023-06-28 19:48:59.612135 q2gui-0.1.95/q2gui/pyqt6/q2style.py
--rw-r--r--   0        0        0     8704 2023-06-30 09:15:23.522377 q2gui-0.1.95/q2gui/pyqt6/q2widget.py
--rw-r--r--   0        0        0     4982 2023-06-29 15:09:52.465129 q2gui-0.1.95/q2gui/pyqt6/q2window.py
--rw-r--r--   0        0        0      754 2023-02-06 11:50:26.449600 q2gui-0.1.95/q2gui/pyqt6/widgets/__init__.py
--rw-r--r--   0        0        0     1945 2023-06-25 14:12:17.787215 q2gui-0.1.95/q2gui/pyqt6/widgets/q2button.py
--rw-r--r--   0        0        0     2604 2023-06-25 14:12:24.675295 q2gui-0.1.95/q2gui/pyqt6/widgets/q2check.py
--rw-r--r--   0        0        0    16742 2023-06-28 20:23:31.010565 q2gui-0.1.95/q2gui/pyqt6/widgets/q2code.py
--rw-r--r--   0        0        0     1997 2023-06-25 14:14:55.047159 q2gui-0.1.95/q2gui/pyqt6/widgets/q2combo.py
--rw-r--r--   0        0        0     7052 2023-06-30 09:30:48.477542 q2gui-0.1.95/q2gui/pyqt6/widgets/q2date.py
--rw-r--r--   0        0        0     1423 2023-06-30 09:29:17.097202 q2gui-0.1.95/q2gui/pyqt6/widgets/q2doublespin.py
--rw-r--r--   0        0        0     3996 2023-06-25 14:14:16.859234 q2gui-0.1.95/q2gui/pyqt6/widgets/q2frame.py
--rw-r--r--   0        0        0     9350 2023-06-28 18:27:25.949985 q2gui-0.1.95/q2gui/pyqt6/widgets/q2grid.py
--rw-r--r--   0        0        0     4910 2023-06-25 14:15:06.706273 q2gui-0.1.95/q2gui/pyqt6/widgets/q2image.py
--rw-r--r--   0        0        0     2326 2023-06-30 09:16:34.186384 q2gui-0.1.95/q2gui/pyqt6/widgets/q2label.py
--rw-r--r--   0        0        0     4990 2023-06-25 14:13:01.287625 q2gui-0.1.95/q2gui/pyqt6/widgets/q2line.py
--rw-r--r--   0        0        0     1832 2023-06-25 14:13:04.950023 q2gui-0.1.95/q2gui/pyqt6/widgets/q2list.py
--rw-r--r--   0        0        0     3400 2023-06-25 14:13:08.964479 q2gui-0.1.95/q2gui/pyqt6/widgets/q2lookup.py
--rw-r--r--   0        0        0     1288 2023-06-25 14:13:12.427853 q2gui-0.1.95/q2gui/pyqt6/widgets/q2progressbar.py
--rw-r--r--   0        0        0     3002 2023-06-25 14:14:45.832847 q2gui-0.1.95/q2gui/pyqt6/widgets/q2radio.py
--rw-r--r--   0        0        0     7206 2023-06-25 14:13:35.252403 q2gui-0.1.95/q2gui/pyqt6/widgets/q2relation.py
--rw-r--r--   0        0        0      998 2023-06-25 14:15:42.427890 q2gui-0.1.95/q2gui/pyqt6/widgets/q2scroller.py
--rw-r--r--   0        0        0    17399 2023-06-25 14:15:37.873742 q2gui-0.1.95/q2gui/pyqt6/widgets/q2sheet.py
--rw-r--r--   0        0        0     1115 2023-06-25 14:15:33.781067 q2gui-0.1.95/q2gui/pyqt6/widgets/q2space.py
--rw-r--r--   0        0        0     1232 2023-06-30 09:29:03.480058 q2gui-0.1.95/q2gui/pyqt6/widgets/q2spin.py
--rw-r--r--   0        0        0     3397 2023-06-25 14:15:24.948690 q2gui-0.1.95/q2gui/pyqt6/widgets/q2tab.py
--rw-r--r--   0        0        0     1545 2023-06-25 14:15:20.976634 q2gui-0.1.95/q2gui/pyqt6/widgets/q2text.py
--rw-r--r--   0        0        0     7538 2023-06-25 14:15:16.690766 q2gui-0.1.95/q2gui/pyqt6/widgets/q2toolbar.py
--rw-r--r--   0        0        0     1168 2023-06-30 09:23:45.362000 q2gui-0.1.95/q2gui/pyqt6/widgets/q2toolbutton.py
--rw-r--r--   0        0        0    21326 2023-06-30 13:00:29.804624 q2gui-0.1.95/q2gui/q2app.py
--rw-r--r--   0        0        0    12944 2023-06-29 20:34:11.352834 q2gui-0.1.95/q2gui/q2dialogs.py
--rw-r--r--   0        0        0    69603 2023-06-30 13:24:00.325657 q2gui-0.1.95/q2gui/q2form.py
--rw-r--r--   0        0        0    15709 2023-06-25 14:10:22.631445 q2gui-0.1.95/q2gui/q2model.py
--rw-r--r--   0        0        0     5909 2023-06-25 14:10:31.421051 q2gui-0.1.95/q2gui/q2style.py
--rw-r--r--   0        0        0     1513 2023-06-25 14:11:23.976312 q2gui-0.1.95/q2gui/q2utils.py
--rw-r--r--   0        0        0     5073 2023-06-25 14:10:45.942186 q2gui-0.1.95/q2gui/q2widget.py
--rw-r--r--   0        0        0     3814 2023-06-25 14:10:50.574661 q2gui-0.1.95/q2gui/q2window.py
--rw-r--r--   0        0        0       22 2023-06-30 13:41:37.311287 q2gui-0.1.95/q2gui/version.py
--rw-r--r--   0        0        0     1533 2022-12-11 17:39:14.929664 q2gui-0.1.95/README.md
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 q2gui-0.1.95/PKG-INFO
+-rw-r--r--   0        0        0    10347 2023-06-21 10:29:20.277459 q2gui-0.1.96/LICENSE
+-rw-r--r--   0        0        0      576 2023-07-01 16:40:21.538590 q2gui-0.1.96/pyproject.toml
+-rw-r--r--   0        0        0       39 2022-12-11 17:39:14.961644 q2gui-0.1.96/q2gui/__init__.py
+-rw-r--r--   0        0        0      892 2022-12-11 17:39:14.961644 q2gui-0.1.96/q2gui/__main__.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:14.961644 q2gui-0.1.96/q2gui/pyqt6/__init__.py
+-rw-r--r--   0        0        0    18937 2023-07-01 11:48:44.092567 q2gui-0.1.96/q2gui/pyqt6/q2app.py
+-rw-r--r--   0        0        0    10075 2023-06-25 14:11:17.663886 q2gui-0.1.96/q2gui/pyqt6/q2form.py
+-rw-r--r--   0        0        0      934 2023-06-25 14:11:34.825464 q2gui-0.1.96/q2gui/pyqt6/q2model.py
+-rw-r--r--   0        0        0    10507 2023-06-28 19:48:59.612135 q2gui-0.1.96/q2gui/pyqt6/q2style.py
+-rw-r--r--   0        0        0     8704 2023-06-30 09:15:23.522377 q2gui-0.1.96/q2gui/pyqt6/q2widget.py
+-rw-r--r--   0        0        0     4982 2023-06-29 15:09:52.465129 q2gui-0.1.96/q2gui/pyqt6/q2window.py
+-rw-r--r--   0        0        0      754 2023-02-06 11:50:26.449600 q2gui-0.1.96/q2gui/pyqt6/widgets/__init__.py
+-rw-r--r--   0        0        0     1945 2023-06-25 14:12:17.787215 q2gui-0.1.96/q2gui/pyqt6/widgets/q2button.py
+-rw-r--r--   0        0        0     2604 2023-06-25 14:12:24.675295 q2gui-0.1.96/q2gui/pyqt6/widgets/q2check.py
+-rw-r--r--   0        0        0    16742 2023-06-28 20:23:31.010565 q2gui-0.1.96/q2gui/pyqt6/widgets/q2code.py
+-rw-r--r--   0        0        0     1997 2023-06-25 14:14:55.047159 q2gui-0.1.96/q2gui/pyqt6/widgets/q2combo.py
+-rw-r--r--   0        0        0     7052 2023-06-30 09:30:48.477542 q2gui-0.1.96/q2gui/pyqt6/widgets/q2date.py
+-rw-r--r--   0        0        0     1423 2023-06-30 09:29:17.097202 q2gui-0.1.96/q2gui/pyqt6/widgets/q2doublespin.py
+-rw-r--r--   0        0        0     3996 2023-06-25 14:14:16.859234 q2gui-0.1.96/q2gui/pyqt6/widgets/q2frame.py
+-rw-r--r--   0        0        0     9350 2023-06-28 18:27:25.949985 q2gui-0.1.96/q2gui/pyqt6/widgets/q2grid.py
+-rw-r--r--   0        0        0     4910 2023-06-25 14:15:06.706273 q2gui-0.1.96/q2gui/pyqt6/widgets/q2image.py
+-rw-r--r--   0        0        0     2326 2023-06-30 09:16:34.186384 q2gui-0.1.96/q2gui/pyqt6/widgets/q2label.py
+-rw-r--r--   0        0        0     4990 2023-06-25 14:13:01.287625 q2gui-0.1.96/q2gui/pyqt6/widgets/q2line.py
+-rw-r--r--   0        0        0     1832 2023-06-25 14:13:04.950023 q2gui-0.1.96/q2gui/pyqt6/widgets/q2list.py
+-rw-r--r--   0        0        0     3400 2023-06-25 14:13:08.964479 q2gui-0.1.96/q2gui/pyqt6/widgets/q2lookup.py
+-rw-r--r--   0        0        0     1288 2023-06-25 14:13:12.427853 q2gui-0.1.96/q2gui/pyqt6/widgets/q2progressbar.py
+-rw-r--r--   0        0        0     3002 2023-06-25 14:14:45.832847 q2gui-0.1.96/q2gui/pyqt6/widgets/q2radio.py
+-rw-r--r--   0        0        0     7206 2023-06-25 14:13:35.252403 q2gui-0.1.96/q2gui/pyqt6/widgets/q2relation.py
+-rw-r--r--   0        0        0      998 2023-06-25 14:15:42.427890 q2gui-0.1.96/q2gui/pyqt6/widgets/q2scroller.py
+-rw-r--r--   0        0        0    17399 2023-06-25 14:15:37.873742 q2gui-0.1.96/q2gui/pyqt6/widgets/q2sheet.py
+-rw-r--r--   0        0        0     1118 2023-07-01 10:11:15.099025 q2gui-0.1.96/q2gui/pyqt6/widgets/q2space.py
+-rw-r--r--   0        0        0     1232 2023-06-30 09:29:03.480058 q2gui-0.1.96/q2gui/pyqt6/widgets/q2spin.py
+-rw-r--r--   0        0        0     3934 2023-07-01 14:42:37.242752 q2gui-0.1.96/q2gui/pyqt6/widgets/q2tab.py
+-rw-r--r--   0        0        0     1545 2023-06-25 14:15:20.976634 q2gui-0.1.96/q2gui/pyqt6/widgets/q2text.py
+-rw-r--r--   0        0        0     7538 2023-06-25 14:15:16.690766 q2gui-0.1.96/q2gui/pyqt6/widgets/q2toolbar.py
+-rw-r--r--   0        0        0     1168 2023-06-30 09:23:45.362000 q2gui-0.1.96/q2gui/pyqt6/widgets/q2toolbutton.py
+-rw-r--r--   0        0        0    21326 2023-06-30 13:00:29.804624 q2gui-0.1.96/q2gui/q2app.py
+-rw-r--r--   0        0        0    12944 2023-06-29 20:34:11.352834 q2gui-0.1.96/q2gui/q2dialogs.py
+-rw-r--r--   0        0        0    69652 2023-07-01 09:42:25.792695 q2gui-0.1.96/q2gui/q2form.py
+-rw-r--r--   0        0        0    15709 2023-06-25 14:10:22.631445 q2gui-0.1.96/q2gui/q2model.py
+-rw-r--r--   0        0        0     5909 2023-06-25 14:10:31.421051 q2gui-0.1.96/q2gui/q2style.py
+-rw-r--r--   0        0        0     1513 2023-06-25 14:11:23.976312 q2gui-0.1.96/q2gui/q2utils.py
+-rw-r--r--   0        0        0     5945 2023-07-01 10:59:16.641839 q2gui-0.1.96/q2gui/q2widget.py
+-rw-r--r--   0        0        0     3814 2023-06-25 14:10:50.574661 q2gui-0.1.96/q2gui/q2window.py
+-rw-r--r--   0        0        0       22 2023-07-01 16:40:24.733400 q2gui-0.1.96/q2gui/version.py
+-rw-r--r--   0        0        0     1533 2022-12-11 17:39:14.929664 q2gui-0.1.96/README.md
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 q2gui-0.1.96/PKG-INFO
```

### Comparing `q2gui-0.1.95/LICENSE` & `q2gui-0.1.96/LICENSE`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/pyproject.toml` & `q2gui-0.1.96/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "q2gui"
-version = "0.1.95"
+version = "0.1.96"
 description = "Python GUI toolkit"
 authors = ["Andrei Puchko <andrei.puchko@gmx.de>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1"
```

### Comparing `q2gui-0.1.95/q2gui/__main__.py` & `q2gui-0.1.96/q2gui/__main__.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/q2app.py` & `q2gui-0.1.96/q2gui/pyqt6/q2app.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,37 +42,48 @@
 
 from PyQt6.QtCore import QEvent, Qt, QCoreApplication, QTimer
 from PyQt6.QtGui import QFontMetrics, QIcon, QFont, QBrush, QColor, QShortcut, QKeySequence
 
 from q2gui.pyqt6.q2window import Q2QtWindow
 from q2gui.pyqt6.q2style import Q2Style
 from q2gui.pyqt6.widgets.q2frame import q2frame
+from q2gui.pyqt6.widgets.q2space import q2space
+from q2gui.pyqt6.widgets.q2toolbutton import q2toolbutton
 
 
 import q2gui.q2app as q2app
 
 
 class stdout_widget(q2frame):
     def __init__(self, mode="h"):
         super().__init__({"column": "/h", "label": "Output"})
         self.stdout_widget = QTextEdit(self)
-        self.closeButton = QToolButton(self)
-        self.closeButton.setText("❌")
-        self.closeButton.setFixedSize(1, 1)
+
+        self.toolbar_frame = q2frame({"column": "/v"})
+        self.closeButton = q2toolbutton(self.make_meta(column="hide", label="❌", mess="Hide output"))
         self.closeButton.clicked.connect(lambda: self.hide())
+
+        self.cleanButton = q2toolbutton(self.make_meta(label="🧹", mess="Clean output"))
+        self.cleanButton.clicked.connect(self.stdout_widget.clear)
+
+        self.toolbar_frame.insert_widget(widget=self.closeButton)
+        # self.toolbar_frame.insert_widget(widget=q2space())
+        self.toolbar_frame.insert_widget(widget=self.cleanButton)
+
         self.insert_widget(widget=self.stdout_widget)
-        self.insert_widget(widget=self.closeButton)
+        self.insert_widget(widget=self.toolbar_frame)
         self.setVisible(False)
 
     def write(self, text):
         if not self.isVisible():
             self.setVisible(True)
         from PyQt6.QtGui import QTextCursor
 
         self.stdout_widget.moveCursor(QTextCursor.MoveOperation.End)
+        q2app.q2_app.process_events()
         self.stdout_widget.insertPlainText(text)
 
 
 class Q2App(QMainWindow, q2app.Q2App, Q2QtWindow):
     class Q2TabWidget(QTabWidget):
         def __init__(self, parent):
             super().__init__(parent)
```

### Comparing `q2gui-0.1.95/q2gui/pyqt6/q2form.py` & `q2gui-0.1.96/q2gui/pyqt6/q2form.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/q2model.py` & `q2gui-0.1.96/q2gui/pyqt6/q2model.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/q2style.py` & `q2gui-0.1.96/q2gui/pyqt6/q2style.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/q2widget.py` & `q2gui-0.1.96/q2gui/pyqt6/q2widget.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/q2window.py` & `q2gui-0.1.96/q2gui/pyqt6/q2window.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/__init__.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2button.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2button.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2check.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2check.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2code.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2code.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2combo.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2combo.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2date.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2date.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2doublespin.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2doublespin.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2frame.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2frame.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2grid.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2grid.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2image.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2image.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2label.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2label.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2line.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2line.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2list.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2list.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2lookup.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2lookup.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2progressbar.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2progressbar.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2radio.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2radio.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2relation.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2relation.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2scroller.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2scroller.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2sheet.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2sheet.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2space.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2space.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,12 +24,12 @@
 
 from PyQt6.QtWidgets import QFrame, QHBoxLayout, QSizePolicy
 
 from q2gui.pyqt6.q2widget import Q2Widget
 
 
 class q2space(QFrame, Q2Widget):
-    def __init__(self, meta):
+    def __init__(self, meta={}):
         super().__init__(meta)
         self.setSizePolicy(QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Minimum)
         self.setLayout(QHBoxLayout())
         self.layout().addStretch()
```

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2spin.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2spin.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2tab.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2tab.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 from PyQt6.QtWidgets import QTabBar, QTabWidget
 from PyQt6.QtGui import QKeySequence, QShortcut
 from PyQt6.QtCore import Qt
 
 from q2gui.pyqt6.q2window import Q2Frame
 from q2gui.pyqt6.q2widget import Q2Widget
-
+from q2gui.q2utils import int_
 
 class Q2TabBar(QTabBar, Q2Widget):
     def get_text(self):
         return self.tabText(self.currentIndex())
 
 
 class q2tab(QTabWidget, Q2Widget, Q2Frame):
@@ -86,14 +86,29 @@
 
     def next_tab(self):
         self.setCurrentIndex(self.currentIndex() + 1)
 
     def prev_tab(self):
         self.setCurrentIndex(self.currentIndex() - 1)
 
+    def set_tab(self, index=0):
+        if isinstance(index, str):
+            for x in range(self.tabBar().count()):
+                print(self.tabBar().tabText(x))
+                if self.tabBar().tabText(x) == index:
+                    index = x
+                    break
+        else:
+            index = int_(index)
+            if index >= self.count():
+                index = self.count() - 1
+            elif index < 0:
+                index = 0
+        self.setCurrentIndex(index)
+
     def minimumSizeHint(self):
         self.setMinimumHeight(super().minimumSizeHint().height())
         return super().minimumSizeHint()
 
     def set_shortcuts_local(self):
         self.next_tab_hotkey.setContext(Qt.ShortcutContext.WidgetWithChildrenShortcut)
         self.prev_tab_hotkey.setContext(Qt.ShortcutContext.WidgetWithChildrenShortcut)
```

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2text.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2text.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2toolbar.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2toolbar.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/pyqt6/widgets/q2toolbutton.py` & `q2gui-0.1.96/q2gui/pyqt6/widgets/q2toolbutton.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/q2app.py` & `q2gui-0.1.96/q2gui/q2app.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/q2dialogs.py` & `q2gui-0.1.96/q2gui/q2dialogs.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/q2form.py` & `q2gui-0.1.96/q2gui/q2form.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,16 +136,15 @@
 
     def set_model(self, model):
         self.model: Q2Model = model
         self.model.q2_form = self
         return self.model
 
     def refresh(self):
-        self.model.refresh()
-        self.refresh_children()
+        self._q2dialogs.q2working(lambda: (self.model.refresh(), self.refresh_children()), _("Refreshing..."))
         self.set_grid_index()
 
     def widget(self):
         if self.form_stack:
             return self.form_stack[-1]
 
     def widgets(self):
```

### Comparing `q2gui-0.1.95/q2gui/q2model.py` & `q2gui-0.1.96/q2gui/q2model.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/q2style.py` & `q2gui-0.1.96/q2gui/q2style.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/q2utils.py` & `q2gui-0.1.96/q2gui/q2utils.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/q2gui/q2widget.py` & `q2gui-0.1.96/q2gui/q2widget.py`

 * *Files 27% similar despite different names*

```diff
@@ -200,7 +200,51 @@
         pass
 
     def action_set_visible(self, text, mode):
         pass
 
     def action_set_enabled(self, text, mode):
         pass
+
+    @staticmethod
+    def make_meta(
+        column="",
+        label="",
+        gridlabel="",
+        control="",
+        pic="",
+        data="",
+        datatype="char",
+        datalen=0,
+        datadec=0,
+        pk="",
+        ai="",
+        migrate="*",
+        actions=[],
+        alignment=-1,
+        to_table="",
+        to_column="",
+        to_form=None,
+        related="",
+        db=None,
+        mask="",
+        opts="",
+        when=None,
+        show=None,
+        valid=None,
+        dblclick=None,
+        readonly=None,
+        disabled=None,
+        check=None,
+        noform=None,
+        nogrid=None,
+        widget=None,
+        margins=None,
+        stretch=0,
+        mess="",
+        tag="",
+        eat_enter=None,
+        hotkey="",
+    ):
+        meta = locals().copy()
+        return meta
+
```

### Comparing `q2gui-0.1.95/q2gui/q2window.py` & `q2gui-0.1.96/q2gui/q2window.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/README.md` & `q2gui-0.1.96/README.md`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.95/PKG-INFO` & `q2gui-0.1.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q2gui
-Version: 0.1.95
+Version: 0.1.96
 Summary: Python GUI toolkit
 License: Apache 2.0
 Author: Andrei Puchko
 Author-email: andrei.puchko@gmx.de
 Requires-Python: >=3.8.1
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

