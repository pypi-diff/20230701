# Comparing `tmp/termuxgui-0.1.5.tar.gz` & `tmp/termuxgui-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termuxgui-0.1.5.tar", last modified: Mon Sep 26 16:56:03 2022, max compression
+gzip compressed data, was "termuxgui-0.1.6.tar", last modified: Sat Jul  1 14:02:56 2023, max compression
```

## Comparing `termuxgui-0.1.5.tar` & `termuxgui-0.1.6.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 16:56:03.782666 termuxgui-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (121)    16725 2022-09-26 16:55:53.000000 termuxgui-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-09-26 16:56:03.782666 termuxgui-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      882 2022-09-26 16:55:53.000000 termuxgui-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-26 16:55:53.000000 termuxgui-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-09-26 16:56:03.782666 termuxgui-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 16:56:03.774665 termuxgui-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 16:56:03.778666 termuxgui-0.1.5/src/termuxgui/
--rw-r--r--   0 runner    (1001) docker     (121)     1982 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5799 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/activity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1667 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/buffer.py
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/button.py
--rw-r--r--   0 runner    (1001) docker     (121)      716 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/compoundbutton.py
--rw-r--r--   0 runner    (1001) docker     (121)     6376 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/edittext.py
--rw-r--r--   0 runner    (1001) docker     (121)     2000 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/event.py
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/framelayout.py
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/gridlayout.py
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/horizontalscrollview.py
--rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/imageview.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/linearlayout.py
--rw-r--r--   0 runner    (1001) docker     (121)     1449 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/msg.py
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/nestedscrollview.py
--rw-r--r--   0 runner    (1001) docker     (121)     6096 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/notification.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 16:56:03.782666 termuxgui-0.1.5/src/termuxgui/oo/
--rw-r--r--   0 runner    (1001) docker     (121)     1495 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1623 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/activity.py
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/button.py
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     3165 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/edittext.py
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/framelayout.py
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/gridlayout.py
--rw-r--r--   0 runner    (1001) docker     (121)      717 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/horizontalscrollview.py
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/imageview.py
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/linearlayout.py
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/nestedscrollview.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/radiobutton.py
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/radiogroup.py
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/space.py
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/spinner.py
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/swiperefreshlayout.py
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/switch.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/tablayout.py
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/textview.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/togglebutton.py
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/view.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/viewgroup.py
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/oo/webview.py
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (121)      735 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/radiobutton.py
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/radiogroup.py
--rw-r--r--   0 runner    (1001) docker     (121)     6211 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/remoteviews.py
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/space.py
--rw-r--r--   0 runner    (1001) docker     (121)      974 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/spinner.py
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/swiperefreshlayout.py
--rw-r--r--   0 runner    (1001) docker     (121)      720 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/switch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/tablayout.py
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/task.py
--rw-r--r--   0 runner    (1001) docker     (121)     2279 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/textview.py
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/togglebutton.py
--rw-r--r--   0 runner    (1001) docker     (121)     6527 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/view.py
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/viewgroup.py
--rw-r--r--   0 runner    (1001) docker     (121)     2378 2022-09-26 16:55:53.000000 termuxgui-0.1.5/src/termuxgui/webview.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 16:56:03.778666 termuxgui-0.1.5/src/termuxgui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-09-26 16:56:03.000000 termuxgui-0.1.5/src/termuxgui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1832 2022-09-26 16:56:03.000000 termuxgui-0.1.5/src/termuxgui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-26 16:56:03.000000 termuxgui-0.1.5/src/termuxgui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-26 16:56:03.000000 termuxgui-0.1.5/src/termuxgui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:02:56.291728 termuxgui-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-01 14:02:46.000000 termuxgui-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-01 14:02:56.291728 termuxgui-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-01 14:02:46.000000 termuxgui-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-01 14:02:46.000000 termuxgui-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-01 14:02:56.291728 termuxgui-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:02:56.283728 termuxgui-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:02:56.287728 termuxgui-0.1.6/src/termuxgui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/compoundbutton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/edittext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/framelayout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/gridlayout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/horizontalscrollview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/linearlayout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/nestedscrollview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:02:56.291728 termuxgui-0.1.6/src/termuxgui/oo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/edittext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/framelayout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/gridlayout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/horizontalscrollview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/linearlayout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/nestedscrollview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/radiobutton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/radiogroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/swiperefreshlayout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/tablayout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/textview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/togglebutton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/viewgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/oo/webview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/radiobutton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/radiogroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/remoteviews.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/swiperefreshlayout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/tablayout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/textview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/togglebutton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/viewgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-01 14:02:46.000000 termuxgui-0.1.6/src/termuxgui/webview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:02:56.287728 termuxgui-0.1.6/src/termuxgui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-01 14:02:56.000000 termuxgui-0.1.6/src/termuxgui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-01 14:02:56.000000 termuxgui-0.1.6/src/termuxgui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 14:02:56.000000 termuxgui-0.1.6/src/termuxgui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 14:02:56.000000 termuxgui-0.1.6/src/termuxgui.egg-info/top_level.txt
```

### Comparing `termuxgui-0.1.5/LICENSE` & `termuxgui-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/PKG-INFO` & `termuxgui-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termuxgui
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python bindings for the Termux:GUI plugin.
 Home-page: https://github.com/tareksander/termux-gui-python-bindings
 Author: Tarek Sander
 Project-URL: Bug Tracker, https://github.com/tareksander/termux-gui-python-bindings/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: Other OS
```

### Comparing `termuxgui-0.1.5/README.md` & `termuxgui-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/setup.cfg` & `termuxgui-0.1.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = termuxgui
-version = 0.1.5
+version = 0.1.6
 author = Tarek Sander
 description = Python bindings for the Termux:GUI plugin.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tareksander/termux-gui-python-bindings
 project_urls = 
 	Bug Tracker = https://github.com/tareksander/termux-gui-python-bindings/issues
```

### Comparing `termuxgui-0.1.5/src/termuxgui/__init__.py` & `termuxgui-0.1.6/src/termuxgui/__init__.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/activity.py` & `termuxgui-0.1.6/src/termuxgui/activity.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,10 +102,13 @@
     def hidesoftkeyboard(self):
         """Hides the soft keyboard if this Activity has the soft keyboard focus."""
         self.c.send_msg({"method": "hideSoftKeyboard", "params": {"aid": self.aid}})
     
     def interceptbackbutton(self, intercept: bool):
         """Sets whether to intercept a back button press and send an event instead."""
         self.c.send_msg({"method": "interceptBackButton", "params": {"aid": self.aid, "intercept": intercept}})
-    
-    
+
+    def setsecure(self, secure: bool):
+        """Sets the secure flag for the Activity, making screenshots impossible and showing a blank screen in the
+        task switcher."""
+        self.c.send_msg({"method": "setSecure", "params": {"aid": self.aid, "secure": secure}})
```

### Comparing `termuxgui-0.1.5/src/termuxgui/buffer.py` & `termuxgui-0.1.6/src/termuxgui/buffer.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/button.py` & `termuxgui-0.1.6/src/termuxgui/button.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/checkbox.py` & `termuxgui-0.1.6/src/termuxgui/checkbox.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/compoundbutton.py` & `termuxgui-0.1.6/src/termuxgui/compoundbutton.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/connection.py` & `termuxgui-0.1.6/src/termuxgui/connection.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         with mainss, eventss:
             mainss.bind('\0' + adrMain)
             eventss.bind('\0' + adrEvent)
             mainss.listen(1)
             eventss.listen(1)
             mainss.settimeout(5)
             eventss.settimeout(5)
-            run(["am", "broadcast", "-n", "com.termux.gui/.GUIReceiver", "--es", "mainSocket", adrMain, "--es",
+            run(["termux-am", "broadcast", "-n", "com.termux.gui/.GUIReceiver", "--es", "mainSocket", adrMain, "--es",
                  "eventSocket", adrEvent], stdout=DEVNULL, stderr=DEVNULL)
             try:
                 main = mainss.accept()[0]
                 try:
                     event = eventss.accept()[0]
                     try:
                         # check for the termux uid to see if it is really the plugin that has connected
@@ -79,15 +79,44 @@
                     except Exception as e:
                         event.close()
                         raise e
                 except Exception as e:
                     main.close()
                     raise e
             except timeout:
-                raise RuntimeError("Could not connect to Termux:GUI. Is the plugin installed?")
+                run(["am", "broadcast", "-n", "com.termux.gui/.GUIReceiver", "--es", "mainSocket", adrMain, "--es",
+                     "eventSocket", adrEvent], stdout=DEVNULL, stderr=DEVNULL)
+                try:
+                    main = mainss.accept()[0]
+                    try:
+                        event = eventss.accept()[0]
+                        try:
+                            # check for the termux uid to see if it is really the plugin that has connected
+                            if not _check_user(main) or not _check_user(event):
+                                main.close()
+                                event.close()
+                                raise RuntimeError("Plugin doesn't have the same UID")
+                            main.sendall(b'\x01')
+                            ret = b''
+                            while len(ret) == 0:
+                                ret = ret + main.recv(1)
+                            if ret[0] != 0:
+                                main.close()
+                                event.close()
+                                raise RuntimeError("Invalid Protocol version response")
+                            self._main = main
+                            self._event = event
+                        except Exception as e:
+                            event.close()
+                            raise e
+                    except Exception as e:
+                        main.close()
+                        raise e
+                except timeout:
+                    raise RuntimeError("Could not connect to Termux:GUI. Is the plugin installed?")
 
     def events(self) -> Iterator[Event]:
         """Waits for events. Use this with "for in" to iterate over incoming events and block while waiting."""
         with self.__event_lock:
             while True:
                 yield Event(tgmsg.read_msg(self._event))
```

### Comparing `termuxgui-0.1.5/src/termuxgui/edittext.py` & `termuxgui-0.1.6/src/termuxgui/edittext.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/event.py` & `termuxgui-0.1.6/src/termuxgui/event.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/framelayout.py` & `termuxgui-0.1.6/src/termuxgui/framelayout.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/gridlayout.py` & `termuxgui-0.1.6/src/termuxgui/gridlayout.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/horizontalscrollview.py` & `termuxgui-0.1.6/src/termuxgui/horizontalscrollview.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/imageview.py` & `termuxgui-0.1.6/src/termuxgui/imageview.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/linearlayout.py` & `termuxgui-0.1.6/src/termuxgui/linearlayout.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/msg.py` & `termuxgui-0.1.6/src/termuxgui/msg.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/nestedscrollview.py` & `termuxgui-0.1.6/src/termuxgui/nestedscrollview.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/notification.py` & `termuxgui-0.1.6/src/termuxgui/notification.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/oo/__init__.py` & `termuxgui-0.1.6/src/termuxgui/oo/__init__.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/oo/activity.py` & `termuxgui-0.1.6/src/termuxgui/oo/activity.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/oo/button.py` & `termuxgui-0.1.6/src/termuxgui/oo/button.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/oo/connection.py` & `termuxgui-0.1.6/src/termuxgui/oo/connection.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/oo/edittext.py` & `termuxgui-0.1.6/src/termuxgui/oo/edittext.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/oo/gridlayout.py` & `termuxgui-0.1.6/src/termuxgui/oo/gridlayout.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/oo/horizontalscrollview.py` & `termuxgui-0.1.6/src/termuxgui/oo/horizontalscrollview.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/oo/linearlayout.py` & `termuxgui-0.1.6/src/termuxgui/oo/linearlayout.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/oo/nestedscrollview.py` & `termuxgui-0.1.6/src/termuxgui/oo/nestedscrollview.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/oo/radiogroup.py` & `termuxgui-0.1.6/src/termuxgui/oo/radiogroup.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/oo/swiperefreshlayout.py` & `termuxgui-0.1.6/src/termuxgui/oo/swiperefreshlayout.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/oo/textview.py` & `termuxgui-0.1.6/src/termuxgui/oo/textview.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/oo/view.py` & `termuxgui-0.1.6/src/termuxgui/oo/view.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/progressbar.py` & `termuxgui-0.1.6/src/termuxgui/progressbar.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/radiobutton.py` & `termuxgui-0.1.6/src/termuxgui/radiobutton.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/radiogroup.py` & `termuxgui-0.1.6/src/termuxgui/radiogroup.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/remoteviews.py` & `termuxgui-0.1.6/src/termuxgui/remoteviews.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/space.py` & `termuxgui-0.1.6/src/termuxgui/space.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/spinner.py` & `termuxgui-0.1.6/src/termuxgui/spinner.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/swiperefreshlayout.py` & `termuxgui-0.1.6/src/termuxgui/swiperefreshlayout.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/switch.py` & `termuxgui-0.1.6/src/termuxgui/switch.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/tablayout.py` & `termuxgui-0.1.6/src/termuxgui/tablayout.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/task.py` & `termuxgui-0.1.6/src/termuxgui/task.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/textview.py` & `termuxgui-0.1.6/src/termuxgui/textview.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/togglebutton.py` & `termuxgui-0.1.6/src/termuxgui/togglebutton.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/view.py` & `termuxgui-0.1.6/src/termuxgui/view.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui/webview.py` & `termuxgui-0.1.6/src/termuxgui/webview.py`

 * *Files identical despite different names*

### Comparing `termuxgui-0.1.5/src/termuxgui.egg-info/PKG-INFO` & `termuxgui-0.1.6/src/termuxgui.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termuxgui
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python bindings for the Termux:GUI plugin.
 Home-page: https://github.com/tareksander/termux-gui-python-bindings
 Author: Tarek Sander
 Project-URL: Bug Tracker, https://github.com/tareksander/termux-gui-python-bindings/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: Other OS
```

### Comparing `termuxgui-0.1.5/src/termuxgui.egg-info/SOURCES.txt` & `termuxgui-0.1.6/src/termuxgui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

