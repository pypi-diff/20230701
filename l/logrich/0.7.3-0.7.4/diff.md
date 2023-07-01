# Comparing `tmp/logrich-0.7.3.tar.gz` & `tmp/logrich-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logrich-0.7.3.tar", max compression
+gzip compressed data, was "logrich-0.7.4.tar", max compression
```

## Comparing `logrich-0.7.3.tar` & `logrich-0.7.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1184 2023-03-25 11:37:39.185788 logrich-0.7.3/README.md
--rw-r--r--   0        0        0       64 2023-05-26 12:26:29.779505 logrich-0.7.3/logrich/__init__.py
--rw-r--r--   0        0        0     2924 2023-03-25 11:37:39.181788 logrich-0.7.3/logrich/app.py
--rw-r--r--   0        0        0     1222 2023-05-30 09:32:35.174252 logrich-0.7.3/logrich/config.py
--rw-r--r--   0        0        0     4819 2023-05-26 11:25:52.964148 logrich-0.7.3/logrich/logger_assets.py
--rw-r--r--   0        0        0      904 2023-05-30 09:35:12.566071 logrich-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     2031 1970-01-01 00:00:00.000000 logrich-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1184 2023-03-25 11:37:39.185788 logrich-0.7.4/README.md
+-rw-r--r--   0        0        0       64 2023-05-26 12:26:29.779505 logrich-0.7.4/logrich/__init__.py
+-rw-r--r--   0        0        0     2924 2023-07-01 04:45:32.044283 logrich-0.7.4/logrich/app.py
+-rw-r--r--   0        0        0     1223 2023-07-01 02:47:20.971119 logrich-0.7.4/logrich/config.py
+-rw-r--r--   0        0        0     5143 2023-07-01 04:47:09.438028 logrich-0.7.4/logrich/logger_assets.py
+-rw-r--r--   0        0        0      904 2023-07-01 04:53:33.844638 logrich-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     2031 1970-01-01 00:00:00.000000 logrich-0.7.4/PKG-INFO
```

### Comparing `logrich-0.7.3/README.md` & `logrich-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `logrich-0.7.3/logrich/app.py` & `logrich-0.7.4/logrich/app.py`

 * *Files identical despite different names*

### Comparing `logrich-0.7.3/logrich/config.py` & `logrich-0.7.4/logrich/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class Settings(BaseSettings):
     """
     Server config settings
     """
 
-    LOG_LEVEL: Union[int,str] = 5
+    LOG_LEVEL: Union[int, str] = 5
     # макисмальная длина текста чтобы разместить его на одной линии с уровнем лога
     MAX_WITH_LOG_OF_OBJ: int = 120
     # https://loguru.readthedocs.io/en/stable/resources/recipes.html#adapting-colors-and-format-of-logged-messages-dynamically
     # https://docs-python.ru/standart-library/modul-string-python/klass-template-modulja-string/
     # https://loguru.readthedocs.io/en/stable/api/logger.html#color
     # https://rich.readthedocs.io/en/stable/style.html
```

### Comparing `logrich-0.7.3/logrich/logger_assets.py` & `logrich-0.7.4/logrich/logger_assets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
 import datetime
+import re
 from typing import Any
 
 import loguru
 
 from rich.highlighter import ReprHighlighter, _combine_regex as combine_regex
+from rich.pretty import pprint  # noqa
 from rich.theme import Theme
 from rich.table import Table
 from rich.console import Console
 from logrich.config import config
 
 
 console = Console()
@@ -125,35 +127,41 @@
         collapse_padding=True,
         show_edge=False,
         show_lines=False,
         show_footer=False,
         expand=True,
         box=None,
     )
+    record_time = ""
+    if config.LOGURU_DATETIME_SHOW:
+        time_ = datetime.datetime.now()
+        record_time = f"\n[#00FA9A r not b] {time_.strftime(config.LOGURU_DATETIME_FORMAT)} [/]"
+    if level.name.lower() in theme_fmt.keys():
+        theme_lvl = theme_fmt.get(style, "")
+        stamp = f"[{theme_lvl}] {level:<9}[/]{record_time}"
+        style = f"{level.name.lower()}_msg"
+    else:
+        style = re.match(r"^\[(.*)\].", level.name).groups()[0].replace("reverse", "")
+        stamp = f"{level:<9}{record_time}"
     # LEVEL
     table.add_column(
         justify="left",
         min_width=config.MIN_WIDTH_COMPUTED,
         max_width=config.MAX_WIDTH,
     )
     # MESSAGE
-    table.add_column(ratio=config.RATIO_MAIN, overflow="fold", style=f"{level.name.lower()}_msg")
+    table.add_column(ratio=config.RATIO_MAIN, overflow="fold", style=style)
     # FILE
     table.add_column(justify="right", ratio=config.RATIO_FROM, overflow="fold")
     # LINE
     table.add_column(ratio=2, overflow="crop")  # для паддинга справа
-    record_time = ""
-    if config.LOGURU_DATETIME_SHOW:
-        time_ = datetime.datetime.now()
-        record_time = f"\n[#00FA9A r not b] {time_.strftime(config.LOGURU_DATETIME_FORMAT)} [/]"
-    table.add_row(
-        f"[{theme_fmt.get(style)}] {level:<9}[/]{record_time}",
-        f"{message}",
-        f"[#858585]{file}...[/][#eb4034]{line}[/]",
-    )
+    msg = f"{message}"
+    file_info = f"[#858585]{file}...[/][#eb4034]{line}[/]"
+
+    table.add_row(stamp, msg, file_info)
     with console.capture() as capture:
         console_dict.print(table, markup=True)
     return capture.get()
 
 
 def format_extra_obj(message: Any) -> str:
     """форматирует вывод исключений в цвете и в заданной ширине, исп-ся rich"""
```

### Comparing `logrich-0.7.3/pyproject.toml` & `logrich-0.7.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "logrich"
-version = "0.7.3"
+version = "0.7.4"
 description = "loguru + rich = logrich"
 authors = ["Dmitry Mavlin <mavlind@list.ru>"]
 license = "GPL"
 readme = "README.md"
 keywords = ["logger", "loguru", "rich"]
 
 [project.urls]
```

### Comparing `logrich-0.7.3/PKG-INFO` & `logrich-0.7.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logrich
-Version: 0.7.3
+Version: 0.7.4
 Summary: loguru + rich = logrich
 License: GPL
 Keywords: logger,loguru,rich
 Author: Dmitry Mavlin
 Author-email: mavlind@list.ru
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

