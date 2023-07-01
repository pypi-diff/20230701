# Comparing `tmp/vspreview-0.7.0.tar.gz` & `tmp/vspreview-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vspreview-0.7.0.tar", last modified: Tue Jun 20 14:27:17 2023, max compression
+gzip compressed data, was "vspreview-0.7.1.tar", last modified: Sat Jul  1 19:27:04 2023, max compression
```

## Comparing `vspreview-0.7.0.tar` & `vspreview-0.7.1.tar`

### file list

```diff
@@ -1,107 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.439163 vspreview-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 14:26:50.000000 vspreview-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-20 14:27:17.439163 vspreview-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-20 14:26:50.000000 vspreview-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-20 14:27:17.439163 vspreview-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-20 14:26:50.000000 vspreview-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.427162 vspreview-0.7.0/vspreview/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.427162 vspreview-0.7.0/vspreview/api/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/api/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/api/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/api/other.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/api/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.427162 vspreview-0.7.0/vspreview/core/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16444 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/abstracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/bases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.431163 vspreview-0.7.0/vspreview/core/custom/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/custom/combobox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/custom/dragnavigator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/custom/edits.py
--rw-r--r--   0 runner    (1001) docker     (123)    11634 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/custom/graphicsview.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/custom/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/custom/notch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/custom/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.431163 vspreview-0.7.0/vspreview/core/types/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/types/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/types/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/types/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/types/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    22099 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/types/video.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/types/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/vsenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.431163 vspreview-0.7.0/vspreview/main/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/main/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/main/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12902 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/main/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    31241 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/main/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.431163 vspreview-0.7.0/vspreview/models/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/models/generalmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/models/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/models/scening.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.431163 vspreview-0.7.0/vspreview/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/plugins/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/plugins/frame_props.ppy
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/plugins/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/plugins/split_view.ppy
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/plugins/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.431163 vspreview-0.7.0/vspreview/toolbars/
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.435163 vspreview-0.7.0/vspreview/toolbars/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/benchmark/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/benchmark/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.435163 vspreview-0.7.0/vspreview/toolbars/comp/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/comp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/comp/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    30482 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/comp/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.435163 vspreview-0.7.0/vspreview/toolbars/debug/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/debug/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/debug/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.435163 vspreview-0.7.0/vspreview/toolbars/main/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/main/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.435163 vspreview-0.7.0/vspreview/toolbars/misc/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/misc/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16070 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/misc/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.435163 vspreview-0.7.0/vspreview/toolbars/pipette/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/pipette/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/pipette/colorview.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/pipette/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/pipette/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.435163 vspreview-0.7.0/vspreview/toolbars/playback/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/playback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/playback/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    25044 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/playback/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.435163 vspreview-0.7.0/vspreview/toolbars/scening/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/scening/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/scening/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/scening/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    35867 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/scening/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.435163 vspreview-0.7.0/vspreview/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.427162 vspreview-0.7.0/vspreview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-20 14:27:17.000000 vspreview-0.7.0/vspreview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-20 14:27:17.000000 vspreview-0.7.0/vspreview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:27:17.000000 vspreview-0.7.0/vspreview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-20 14:27:17.000000 vspreview-0.7.0/vspreview.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:27:08.000000 vspreview-0.7.0/vspreview.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-20 14:27:17.000000 vspreview-0.7.0/vspreview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 14:27:17.000000 vspreview-0.7.0/vspreview.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:27:04.984718 vspreview-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-01 19:26:43.000000 vspreview-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-01 19:27:04.984718 vspreview-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-01 19:26:43.000000 vspreview-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-01 19:27:04.984718 vspreview-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-01 19:26:43.000000 vspreview-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:27:04.972718 vspreview-0.7.1/vspreview/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:27:04.976719 vspreview-0.7.1/vspreview/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/api/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/api/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/api/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:27:04.976719 vspreview-0.7.1/vspreview/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16444 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/core/abstracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/core/bases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:27:04.976719 vspreview-0.7.1/vspreview/core/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/core/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/core/custom/combobox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/core/custom/dragnavigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/core/custom/edits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11634 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/core/custom/graphicsview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/core/custom/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/core/custom/notch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/core/custom/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:27:04.976719 vspreview-0.7.1/vspreview/core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/core/types/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/core/types/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/core/types/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/core/types/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22170 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/core/types/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/core/types/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/core/vsenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:27:04.980718 vspreview-0.7.1/vspreview/main/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/main/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/main/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12902 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/main/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31241 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/main/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:27:04.980718 vspreview-0.7.1/vspreview/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/models/generalmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/models/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/models/scening.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:27:04.980718 vspreview-0.7.1/vspreview/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/plugins/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/plugins/frame_props.ppy
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/plugins/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/plugins/split_view.ppy
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/plugins/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/qt_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:27:04.980718 vspreview-0.7.1/vspreview/toolbars/
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:27:04.980718 vspreview-0.7.1/vspreview/toolbars/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/benchmark/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/benchmark/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:27:04.980718 vspreview-0.7.1/vspreview/toolbars/comp/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/comp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/comp/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30482 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/comp/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:27:04.980718 vspreview-0.7.1/vspreview/toolbars/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/debug/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/debug/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:27:04.980718 vspreview-0.7.1/vspreview/toolbars/main/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/main/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:27:04.980718 vspreview-0.7.1/vspreview/toolbars/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/misc/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16070 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/misc/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:27:04.980718 vspreview-0.7.1/vspreview/toolbars/pipette/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/pipette/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/pipette/colorview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/pipette/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/pipette/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:27:04.984718 vspreview-0.7.1/vspreview/toolbars/playback/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/playback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/playback/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25044 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/playback/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:27:04.984718 vspreview-0.7.1/vspreview/toolbars/scening/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/scening/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/scening/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/scening/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35867 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/toolbars/scening/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:27:04.984718 vspreview-0.7.1/vspreview/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17989 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-01 19:26:43.000000 vspreview-0.7.1/vspreview/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:27:04.976719 vspreview-0.7.1/vspreview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-01 19:27:04.000000 vspreview-0.7.1/vspreview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-01 19:27:04.000000 vspreview-0.7.1/vspreview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 19:27:04.000000 vspreview-0.7.1/vspreview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-01 19:27:04.000000 vspreview-0.7.1/vspreview.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 19:26:57.000000 vspreview-0.7.1/vspreview.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-01 19:27:04.000000 vspreview-0.7.1/vspreview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 19:27:04.000000 vspreview-0.7.1/vspreview.egg-info/top_level.txt
```

### Comparing `vspreview-0.7.0/LICENSE` & `vspreview-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/PKG-INFO` & `vspreview-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vspreview
-Version: 0.7.0
+Version: 0.7.1
 Summary: Previewer for VapourSynth scripts
 Author: Endilll
 Author-email: 
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-preview
 Project-URL: Documentation, https://vspreview.encode.moe/en/latest/
```

### Comparing `vspreview-0.7.0/README.md` & `vspreview-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/setup.cfg` & `vspreview-0.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/setup.py` & `vspreview-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/api/nodes.py` & `vspreview-0.7.1/vspreview/api/nodes.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/api/other.py` & `vspreview-0.7.1/vspreview/api/other.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/api/output.py` & `vspreview-0.7.1/vspreview/api/output.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/core/abstracts.py` & `vspreview-0.7.1/vspreview/core/abstracts.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/core/bases.py` & `vspreview-0.7.1/vspreview/core/bases.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/core/custom/combobox.py` & `vspreview-0.7.1/vspreview/core/custom/combobox.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/core/custom/dragnavigator.py` & `vspreview-0.7.1/vspreview/core/custom/dragnavigator.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/core/custom/edits.py` & `vspreview-0.7.1/vspreview/core/custom/edits.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/core/custom/graphicsview.py` & `vspreview-0.7.1/vspreview/core/custom/graphicsview.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/core/custom/misc.py` & `vspreview-0.7.1/vspreview/core/custom/misc.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/core/custom/notch.py` & `vspreview-0.7.1/vspreview/core/custom/notch.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/core/custom/plotting.py` & `vspreview-0.7.1/vspreview/core/custom/plotting.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/core/logger.py` & `vspreview-0.7.1/vspreview/core/logger.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/core/types/audio.py` & `vspreview-0.7.1/vspreview/core/types/audio.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/core/types/scene.py` & `vspreview-0.7.1/vspreview/core/types/scene.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/core/types/units.py` & `vspreview-0.7.1/vspreview/core/types/units.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/core/types/video.py` & `vspreview-0.7.1/vspreview/core/types/video.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,35 +99,36 @@
 
         self.main = main_window()
 
         assert self.main.env
 
         self.set_fmt_values()
 
-        # runtime attributes
-        self.source = VideoOutputNode(vs_output.clip, vs_output.alpha)
-        self.prepared = VideoOutputNode(vs_output.clip, vs_output.alpha)
-
-        if self.source.alpha is not None:
-            self.prepared.alpha = self.prepare_vs_output(self.source.alpha, True).std.CopyFrameProps(self.source.alpha)
-
         with self.main.env:
             vs_outputs = list(vs.get_outputs().values())
 
         self.vs_index = index
         self.index = vs_outputs.index(vs_output) if vs_output in vs_outputs else index
 
+        self.info = self.main.user_output_info[vs.VideoNode].get(self.vs_index, {})  # type: ignore
+
+        self.cached = not not self.info.get('cache', False)
+        self.source = VideoOutputNode(vs_output.clip, vs_output.alpha, self.cached)
+        self.prepared = VideoOutputNode(vs_output.clip, vs_output.alpha, self.cached)
+
+        if self.source.alpha is not None:
+            self.prepared.alpha = self.prepare_vs_output(self.source.alpha, True).std.CopyFrameProps(self.source.alpha)
+
         self.prepared.clip = self.prepare_vs_output(self.source.clip).std.CopyFrameProps(self.source.clip)
         self.width = self.prepared.clip.width
         self.height = self.prepared.clip.height
         self.fps_num = self.prepared.clip.fps.numerator
         self.fps_den = self.prepared.clip.fps.denominator
         self.fps = self.fps_num / self.fps_den
         self.total_frames = Frame(self.prepared.clip.num_frames)
-        self.info = self.main.user_output_info[vs.VideoNode].get(self.vs_index, {})  # type: ignore
 
         self.name = self.info.get('name', 'Video Node %d' % self.vs_index)
 
         if self.main.outputs is not None:
             self.main.outputs.setData(self.main.outputs.index(self.vs_index), self.name)
 
         self.props = cast(vs.FrameProps, {})
@@ -548,15 +549,15 @@
         return Frame(self._calculate_frame(float(time)))
 
     def to_time(self, frame: Frame) -> Time:
         return Time(seconds=self._calculate_seconds(int(frame)))
 
     def with_node(self, new_node: vs.VideoNode | VideoOutputNode) -> VideoOutput:
         if isinstance(new_node, vs.VideoNode):
-            new_node = VideoOutputNode(new_node, None)
+            new_node = VideoOutputNode(new_node, None, self.cached)
 
         new_output = VideoOutput(new_node, self.vs_index, False)
         new_output.index = self.index
 
         new_output.last_showed_frame = self.last_showed_frame
         new_output.name = self.name
```

### Comparing `vspreview-0.7.0/vspreview/core/types/yaml.py` & `vspreview-0.7.1/vspreview/core/types/yaml.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/core/vsenv.py` & `vspreview-0.7.1/vspreview/core/vsenv.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/init.py` & `vspreview-0.7.1/vspreview/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from . import qt_patch  # noqa: F401
+
 import logging
 import os
 import signal
 import sys
 from argparse import ArgumentParser
 from pathlib import Path
 from typing import Sequence
```

### Comparing `vspreview-0.7.0/vspreview/main/dialog.py` & `vspreview-0.7.1/vspreview/main/dialog.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/main/settings.py` & `vspreview-0.7.1/vspreview/main/settings.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/main/timeline.py` & `vspreview-0.7.1/vspreview/main/timeline.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/main/window.py` & `vspreview-0.7.1/vspreview/main/window.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/models/generalmodel.py` & `vspreview-0.7.1/vspreview/models/generalmodel.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/models/outputs.py` & `vspreview-0.7.1/vspreview/models/outputs.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/models/scening.py` & `vspreview-0.7.1/vspreview/models/scening.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/plugins/__init__.py` & `vspreview-0.7.1/vspreview/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/plugins/abstract.py` & `vspreview-0.7.1/vspreview/plugins/abstract.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/plugins/frame_props.ppy` & `vspreview-0.7.1/vspreview/plugins/frame_props.ppy`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/plugins/install.py` & `vspreview-0.7.1/vspreview/plugins/install.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/plugins/split_view.ppy` & `vspreview-0.7.1/vspreview/plugins/split_view.ppy`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/plugins/utils.py` & `vspreview-0.7.1/vspreview/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/toolbars/__init__.py` & `vspreview-0.7.1/vspreview/toolbars/__init__.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/toolbars/benchmark/settings.py` & `vspreview-0.7.1/vspreview/toolbars/benchmark/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,80 @@
 from __future__ import annotations
 
 from typing import Any, Mapping
 
 from PyQt6.QtWidgets import QLabel
 
-from ...core import AbstractToolbarSettings, CheckBox, HBoxLayout, Time, TimeEdit, try_load
+from ...core import AbstractToolbarSettings, CheckBox, HBoxLayout, Time, TimeEdit, try_load, SpinBox
 
 __all__ = [
     'BenchmarkSettings'
 ]
 
 
 class BenchmarkSettings(AbstractToolbarSettings):
     __slots__ = (
         'clear_cache_checkbox',
         'refresh_interval_control', 'frame_data_sharing_fix_checkbox',
     )
 
     def setup_ui(self) -> None:
+        from ...main import MainSettings
+
         super().setup_ui()
 
         self.clear_cache_checkbox = CheckBox('Clear VS frame caches before each run', self)
 
         self.frame_data_sharing_fix_checkbox = CheckBox('(Debug) Enable frame data sharing fix', self)
 
         self.refresh_interval_control = TimeEdit(self)
 
+        self.default_usable_cpus_spinbox = SpinBox(self, 1, MainSettings.get_usable_cpus_count())
+
         self.vlayout.addWidgets([
             self.clear_cache_checkbox,
             self.frame_data_sharing_fix_checkbox
         ])
         self.vlayout.addLayout(
             HBoxLayout([
-                QLabel('Refresh interval', self),
+                QLabel('Refresh interval'),
                 self.refresh_interval_control
             ])
         )
+        self.vlayout.addLayout(
+            HBoxLayout([
+                QLabel('Default usable CPUs count'),
+                self.default_usable_cpus_spinbox
+            ])
+        )
 
     def set_defaults(self) -> None:
+        from ...main import MainSettings
+
         self.clear_cache_checkbox.setChecked(False)
         self.refresh_interval_control.setValue(Time(milliseconds=150))
         self.frame_data_sharing_fix_checkbox.setChecked(True)
+        self.default_usable_cpus_spinbox.setValue(max(1, MainSettings.get_usable_cpus_count() // 2))
 
     @property
     def clear_cache_enabled(self) -> bool:
         return self.clear_cache_checkbox.isChecked()
 
     @property
     def refresh_interval(self) -> Time:
         return self.refresh_interval_control.value()
 
     @property
     def frame_data_sharing_fix_enabled(self) -> bool:
         return self.frame_data_sharing_fix_checkbox.isChecked()
 
+    @property
+    def default_usable_cpus_count(self) -> int:
+        return self.default_usable_cpus_spinbox.value()
+
     def __getstate__(self) -> Mapping[str, Any]:
         return {
             'clear_cache_enabled': self.clear_cache_enabled,
             'refresh_interval': self.refresh_interval,
             'frame_data_sharing_fix_enabled': self.frame_data_sharing_fix_enabled,
         }
```

### Comparing `vspreview-0.7.0/vspreview/toolbars/benchmark/toolbar.py` & `vspreview-0.7.1/vspreview/toolbars/benchmark/toolbar.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from time import perf_counter
 from typing import TYPE_CHECKING
 
 import vapoursynth as vs
 from PyQt6.QtCore import QMetaObject, Qt
 from PyQt6.QtWidgets import QLabel
 
-from ...core import AbstractToolbar, CheckBox, Frame, PushButton, Time, Timer
+from ...core import AbstractToolbar, CheckBox, Frame, PushButton, Time, Timer, SpinBox
 from ...core.custom import FrameEdit
 from ...utils import qt_silent_call, strfdelta
 from .settings import BenchmarkSettings
 
 
 if TYPE_CHECKING:
     from ...main import MainWindow
@@ -61,19 +61,24 @@
         self.update_info_timer = Timer(timeout=self.update_info, timerType=Qt.TimerType.PreciseTimer)
 
         self.set_qobject_names()
 
     def setup_ui(self) -> None:
         super().setup_ui()
 
-        self.start_frame_control = FrameEdit(self, valueChanged=lambda value: self.update_controls(start=value))
-
-        self.end_frame_control = FrameEdit(self, valueChanged=lambda value: self.update_controls(end=value))
-
-        self.total_frames_control = FrameEdit(self, 1, valueChanged=lambda value: self.update_controls(total=value))
+        self.start_frame_control = FrameEdit(
+            self, 0, maximum=10000, valueChanged=lambda value: self.update_controls(start=value)
+        )
+        self.end_frame_control = FrameEdit(
+            self, maximum=10000, valueChanged=lambda value: self.update_controls(end=value)
+        )
+        self.total_frames_control = FrameEdit(
+            self, 1, maximum=10000, valueChanged=lambda value: self.update_controls(total=value)
+        )
+        self.total_frames_control.setValue(1000)
 
         self.unsequenced_checkbox = CheckBox(
             'Unsequenced', self, checked=True, tooltip=(
                 "If enabled, next frame will be requested each time frameserver returns completed frame.\n"
                 "If disabled, first frame that's currently processing will be waited before requesting the next one."
             )
         )
@@ -83,65 +88,75 @@
             stateChanged=self.on_prefetch_changed
         )
 
         self.run_abort_button = PushButton('Run', self, checkable=True, clicked=self.on_run_abort_pressed)
 
         self.info_label = QLabel(self)
 
+        self.usable_cpus_spinbox = SpinBox(self, 1, self.settings.default_usable_cpus_spinbox.maximum())
+        self.usable_cpus_spinbox.setValue(self.settings.default_usable_cpus_count)
+
         self.hlayout.addWidgets([
             QLabel('Start:'), self.start_frame_control,
             QLabel('End:'), self.end_frame_control,
             QLabel('Total:'), self.total_frames_control,
+            QLabel('Usable CPUs Count:'), self.usable_cpus_spinbox,
             self.prefetch_checkbox,
             self.unsequenced_checkbox,
             self.run_abort_button,
-            self.info_label,
+            self.info_label
         ])
         self.hlayout.addStretch()
 
     def on_current_output_changed(self, index: int, prev_index: int) -> None:
-        self.start_frame_control.setMaximum(self.main.current_output.total_frames - 1)
-        self.end_frame_control.setMaximum(self.main.current_output.total_frames - 1)
-        self.total_frames_control.setMaximum(self.main.current_output.total_frames - Frame(1))
+        max_frames = 1000 if self.main.current_output is None else self.main.current_output.total_frames
+        self.start_frame_control.setMaximum(max_frames - 1)
+        self.end_frame_control.setMaximum(max_frames - 1)
+        self.total_frames_control.setMaximum(max_frames - Frame(1))
+        self.total_frames_control.setValue(min(self.total_frames_control.value() or 1000, max_frames))
 
     def run(self) -> None:
         if self.settings.clear_cache_enabled:
             from vstools.utils.vs_proxy import clear_cache
             clear_cache()
 
         if self.settings.frame_data_sharing_fix_enabled:
             self.main.current_output.update_graphic_item(
                 self.main.current_scene.pixmap().copy(),
                 graphics_scene_item=self.main.current_output.graphics_scene_item
             )
 
+        self.frames_done = 0
+
         self.start_frame = self.start_frame_control.value()
         self.end_frame = self.end_frame_control.value()
         self.total_frames = self.total_frames_control.value()
         self.frames_left = deepcopy(self.total_frames)
+
         if self.prefetch_checkbox.isChecked():
-            concurrent_requests_count = self.main.settings.usable_cpus_count
+            concurrent_requests_count = self.usable_cpus_spinbox.value()
         else:
             concurrent_requests_count = 1
 
         self.unsequenced = self.unsequenced_checkbox.isChecked()
         if not self.unsequenced:
             self.buffer = deque([], concurrent_requests_count)
             self.sequenced_timer.start()
 
         self.running = True
         self.run_start_time = perf_counter()
+        self.update_info()
 
         for offset in range(min(int(self.frames_left), concurrent_requests_count)):
             if self.unsequenced:
                 self._request_next_frame_unsequenced()
             else:
-                frame = self.start_frame + Frame(offset)
-                future = self.main.current_output.prepared.clip.get_frame_async(int(frame))
-                self.buffer.appendleft(future)
+                self.buffer.appendleft(
+                    self.main.current_output.source.original_clip.get_frame_async(self.start_frame + offset)
+                )
 
         self.update_info_timer.setInterval(round(float(self.settings.refresh_interval) * 1000))
         self.update_info_timer.start()
 
     def abort(self) -> None:
         if self.running:
             self.update_info()
@@ -153,64 +168,76 @@
             self.run_abort_button.click()
 
     def _request_next_frame_sequenced(self) -> None:
         if self.frames_left <= Frame(0):
             self.abort()
             return
 
+        self.frames_done += 1
         self.buffer.pop().result()
 
-        next_frame = self.end_frame + Frame(1) - self.frames_left
-        if next_frame <= self.end_frame:
-            new_future = self.main.current_output.prepared.clip.get_frame_async(int(next_frame))
-            self.buffer.appendleft(new_future)
+        if (next_frame := self.end_frame + 1 - self.frames_left) <= self.end_frame:
+            self.buffer.appendleft(
+                self.main.current_output.source.original_clip.get_frame_async(next_frame)
+            )
 
         self.frames_left -= Frame(1)
 
     def _request_next_frame_unsequenced(self, future: Future[vs.VideoFrame] | None = None) -> None:
-        if self.frames_left <= Frame(0):
+        if self.frames_done >= self.total_frames:
             self.abort()
             return
 
         if self.running:
-            next_frame = self.end_frame + Frame(1) - self.frames_left
-            new_future = self.main.current_output.prepared.clip.get_frame_async(int(next_frame))
-            new_future.add_done_callback(self._request_next_frame_unsequenced)  # type: ignore
+            self.main.current_output.source.original_clip.get_frame_async(
+                self.end_frame + 1 - self.frames_left
+            ).add_done_callback(
+                self._request_next_frame_unsequenced
+            )
 
         if future is not None:
             future.result()
+            self.frames_done += 1
+
         self.frames_left -= Frame(1)
 
     def on_run_abort_pressed(self, checked: bool) -> None:
         self.set_ui_editable(not checked)
         if checked:
             self.run()
         else:
             self.abort()
 
     def on_prefetch_changed(self, new_state: Qt.CheckState) -> None:
         if new_state == Qt.CheckState.Checked:
             self.unsequenced_checkbox.setEnabled(True)
+            self.usable_cpus_spinbox.setEnabled(True)
         elif new_state == Qt.CheckState.Unchecked:
             self.unsequenced_checkbox.setChecked(False)
             self.unsequenced_checkbox.setEnabled(False)
+            self.usable_cpus_spinbox.setEnabled(False)
 
     def set_ui_editable(self, new_state: bool) -> None:
         self. start_frame_control.setEnabled(new_state)
         self.end_frame_control.setEnabled(new_state)
         self.total_frames_control.setEnabled(new_state)
         self.prefetch_checkbox.setEnabled(new_state)
         self. unsequenced_checkbox.setEnabled(new_state)
 
     def update_controls(
         self, start: Frame | None = None, end: Frame | None = None, total: Frame | None = None
     ) -> None:
         if not hasattr(self.main, 'current_output'):
             return
 
+        if self.main.current_output is None:
+            max_frames = 1000
+        else:
+            max_frames = self.main.current_output.total_frames
+
         if start is not None:
             end = self.end_frame_control.value()
             total = self.total_frames_control.value()
 
             if start > end:
                 end = start
             total = end - start + Frame(1)
@@ -224,24 +251,24 @@
         elif total is not None:
             start = self.start_frame_control.value()
             end = self.end_frame_control.value()
             old_total = end - start + Frame(1)
             delta = total - old_total
 
             end += delta
-            if end > (e := self.main.current_output.total_frames - 1):
+            if end > (e := max_frames - 1):
                 start -= end - e
                 end = e
         else:
             return
 
         qt_silent_call(self.start_frame_control.setValue, start)
         qt_silent_call(self.end_frame_control.setValue, end)
         qt_silent_call(self.total_frames_control.setValue, total)
 
     def update_info(self) -> None:
         run_time = Time(seconds=(perf_counter() - self.run_start_time))
-        frames_done = self.total_frames - self.frames_left
-        fps = int(frames_done) / float(run_time)
+        fps = int(self.frames_done) / float(run_time)
 
-        info_str = (f"{frames_done}/{self.total_frames} frames in {strfdelta(run_time, '%M:%S.%Z')}, {fps:.4f} fps")
-        self.info_label.setText(info_str)
+        self.info_label.setText(
+            f"{self.frames_done}/{self.total_frames} frames in {strfdelta(run_time, '%M:%S.%Z')}, {fps:.4f} fps"
+        )
```

### Comparing `vspreview-0.7.0/vspreview/toolbars/comp/settings.py` & `vspreview-0.7.1/vspreview/toolbars/comp/settings.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/toolbars/comp/toolbar.py` & `vspreview-0.7.1/vspreview/toolbars/comp/toolbar.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/toolbars/debug/toolbar.py` & `vspreview-0.7.1/vspreview/toolbars/debug/toolbar.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/toolbars/main/toolbar.py` & `vspreview-0.7.1/vspreview/toolbars/main/toolbar.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/toolbars/misc/toolbar.py` & `vspreview-0.7.1/vspreview/toolbars/misc/toolbar.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/toolbars/pipette/colorview.py` & `vspreview-0.7.1/vspreview/toolbars/pipette/colorview.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/toolbars/pipette/toolbar.py` & `vspreview-0.7.1/vspreview/toolbars/pipette/toolbar.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/toolbars/playback/settings.py` & `vspreview-0.7.1/vspreview/toolbars/playback/settings.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/toolbars/playback/toolbar.py` & `vspreview-0.7.1/vspreview/toolbars/playback/toolbar.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/toolbars/scening/dialog.py` & `vspreview-0.7.1/vspreview/toolbars/scening/dialog.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/toolbars/scening/settings.py` & `vspreview-0.7.1/vspreview/toolbars/scening/settings.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/toolbars/scening/toolbar.py` & `vspreview-0.7.1/vspreview/toolbars/scening/toolbar.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview/utils/debug.py` & `vspreview-0.7.1/vspreview/utils/debug.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,27 +85,27 @@
     def run_get_frame_test(self) -> None:
         N = 10
 
         start_frame_async = 1000
         total_async = 0
         for i in range(start_frame_async, start_frame_async + N):
             s1 = perf_counter_ns()
-            f1 = self.main.current_output.prepared.clip.get_frame_async(i)
+            f1 = self.main.current_output.source.original_clip.get_frame_async(i)
             f1.result()
             s2 = perf_counter_ns()
             logging.debug(f'async test time: {s2 - s1} ns')
             if i != start_frame_async:
                 total_async += s2 - s1
 
         start_frame_sync = 2000
         total_sync = 0
 
         for i in range(start_frame_sync, start_frame_sync + N):
             s1 = perf_counter_ns()
-            self.main.current_output.prepared.clip.get_frame(i)
+            self.main.current_output.source.original_clip.get_frame(i)
             s2 = perf_counter_ns()
             if i != start_frame_sync:
                 total_sync += s2 - s1
 
         logging.debug('')
         logging.debug(f'Async average: {total_async / N - 1} ns, {1_000_000_000 / (total_async / N - 1)} fps')
         logging.debug(f'Sync average:  {total_sync  / N - 1} ns, {1_000_000_000 / (total_sync  / N - 1)} fps')
```

### Comparing `vspreview-0.7.0/vspreview/utils/utils.py` & `vspreview-0.7.1/vspreview/utils/utils.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.7.0/vspreview.egg-info/PKG-INFO` & `vspreview-0.7.1/vspreview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vspreview
-Version: 0.7.0
+Version: 0.7.1
 Summary: Previewer for VapourSynth scripts
 Author: Endilll
 Author-email: 
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-preview
 Project-URL: Documentation, https://vspreview.encode.moe/en/latest/
```

### Comparing `vspreview-0.7.0/vspreview.egg-info/SOURCES.txt` & `vspreview-0.7.1/vspreview.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.cfg
 setup.py
 vspreview/__init__.py
 vspreview/__main__.py
 vspreview/_metadata.py
 vspreview/init.py
 vspreview/py.typed
+vspreview/qt_patch.py
 vspreview.egg-info/PKG-INFO
 vspreview.egg-info/SOURCES.txt
 vspreview.egg-info/dependency_links.txt
 vspreview.egg-info/entry_points.txt
 vspreview.egg-info/not-zip-safe
 vspreview.egg-info/requires.txt
 vspreview.egg-info/top_level.txt
```

