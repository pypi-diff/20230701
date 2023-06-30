# Comparing `tmp/refuel-autolabel-0.0.5.tar.gz` & `tmp/refuel-autolabel-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refuel-autolabel-0.0.5.tar", last modified: Fri Jun 23 23:32:07 2023, max compression
+gzip compressed data, was "refuel-autolabel-0.0.6.tar", last modified: Fri Jun 30 23:17:00 2023, max compression
```

## Comparing `refuel-autolabel-0.0.5.tar` & `refuel-autolabel-0.0.6.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.793369 refuel-autolabel-0.0.5/
--rw-r--r--   0 nihit      (501) staff       (20)     1066 2023-05-11 06:24:46.000000 refuel-autolabel-0.0.5/LICENSE
--rw-r--r--   0 nihit      (501) staff       (20)    10926 2023-06-23 23:32:07.793181 refuel-autolabel-0.0.5/PKG-INFO
--rw-r--r--   0 nihit      (501) staff       (20)     8902 2023-06-23 16:52:52.000000 refuel-autolabel-0.0.5/README.md
--rw-r--r--   0 nihit      (501) staff       (20)     2134 2023-06-23 23:30:09.000000 refuel-autolabel-0.0.5/pyproject.toml
--rw-r--r--   0 nihit      (501) staff       (20)       38 2023-06-23 23:32:07.793418 refuel-autolabel-0.0.5/setup.cfg
-drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.782307 refuel-autolabel-0.0.5/src/
-drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.784280 refuel-autolabel-0.0.5/src/autolabel/
--rw-r--r--   0 nihit      (501) staff       (20)       63 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.5/src/autolabel/__init__.py
-drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.785045 refuel-autolabel-0.0.5/src/autolabel/cache/
--rw-r--r--   0 nihit      (501) staff       (20)       74 2023-05-16 00:22:56.000000 refuel-autolabel-0.0.5/src/autolabel/cache/__init__.py
--rw-r--r--   0 nihit      (501) staff       (20)      924 2023-06-08 20:27:49.000000 refuel-autolabel-0.0.5/src/autolabel/cache/base.py
--rw-r--r--   0 nihit      (501) staff       (20)     1817 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.5/src/autolabel/cache/sqlalchemy_cache.py
--rw-r--r--   0 nihit      (501) staff       (20)     9137 2023-06-15 00:40:46.000000 refuel-autolabel-0.0.5/src/autolabel/confidence.py
-drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.785708 refuel-autolabel-0.0.5/src/autolabel/configs/
--rw-r--r--   0 nihit      (501) staff       (20)       65 2023-05-29 00:22:31.000000 refuel-autolabel-0.0.5/src/autolabel/configs/__init__.py
--rw-r--r--   0 nihit      (501) staff       (20)     1515 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.5/src/autolabel/configs/base.py
--rw-r--r--   0 nihit      (501) staff       (20)     5886 2023-06-20 23:17:06.000000 refuel-autolabel-0.0.5/src/autolabel/configs/config.py
-drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.787277 refuel-autolabel-0.0.5/src/autolabel/data_models/
--rw-r--r--   0 nihit      (501) staff       (20)      195 2023-05-16 00:22:56.000000 refuel-autolabel-0.0.5/src/autolabel/data_models/__init__.py
--rw-r--r--   0 nihit      (501) staff       (20)     2001 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.5/src/autolabel/data_models/annotation.py
--rw-r--r--   0 nihit      (501) staff       (20)       71 2023-05-14 02:11:15.000000 refuel-autolabel-0.0.5/src/autolabel/data_models/base.py
--rw-r--r--   0 nihit      (501) staff       (20)     2036 2023-06-10 22:44:42.000000 refuel-autolabel-0.0.5/src/autolabel/data_models/cache.py
--rw-r--r--   0 nihit      (501) staff       (20)     1071 2023-05-14 02:11:15.000000 refuel-autolabel-0.0.5/src/autolabel/data_models/dataset.py
--rw-r--r--   0 nihit      (501) staff       (20)      928 2023-05-14 02:11:15.000000 refuel-autolabel-0.0.5/src/autolabel/data_models/task.py
--rw-r--r--   0 nihit      (501) staff       (20)     2625 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.5/src/autolabel/data_models/task_run.py
-drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.787851 refuel-autolabel-0.0.5/src/autolabel/database/
--rw-r--r--   0 nihit      (501) staff       (20)       77 2023-05-14 02:11:15.000000 refuel-autolabel-0.0.5/src/autolabel/database/__init__.py
--rw-r--r--   0 nihit      (501) staff       (20)      410 2023-06-10 22:44:42.000000 refuel-autolabel-0.0.5/src/autolabel/database/engine.py
--rw-r--r--   0 nihit      (501) staff       (20)     2788 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.5/src/autolabel/database/state_manager.py
--rw-r--r--   0 nihit      (501) staff       (20)     8085 2023-06-23 23:23:54.000000 refuel-autolabel-0.0.5/src/autolabel/dataset_loader.py
-drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.788486 refuel-autolabel-0.0.5/src/autolabel/few_shot/
--rw-r--r--   0 nihit      (501) staff       (20)     2429 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.5/src/autolabel/few_shot/__init__.py
--rw-r--r--   0 nihit      (501) staff       (20)     1295 2023-05-14 02:11:15.000000 refuel-autolabel-0.0.5/src/autolabel/few_shot/fixed_example_selector.py
--rw-r--r--   0 nihit      (501) staff       (20)    11031 2023-06-09 05:14:40.000000 refuel-autolabel-0.0.5/src/autolabel/few_shot/vector_store.py
--rw-r--r--   0 nihit      (501) staff       (20)    19406 2023-06-23 23:23:54.000000 refuel-autolabel-0.0.5/src/autolabel/labeler.py
-drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.790398 refuel-autolabel-0.0.5/src/autolabel/models/
--rw-r--r--   0 nihit      (501) staff       (20)     1965 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.5/src/autolabel/models/__init__.py
--rw-r--r--   0 nihit      (501) staff       (20)     2496 2023-05-29 00:22:31.000000 refuel-autolabel-0.0.5/src/autolabel/models/anthropic.py
--rw-r--r--   0 nihit      (501) staff       (20)     4150 2023-05-29 00:22:31.000000 refuel-autolabel-0.0.5/src/autolabel/models/base.py
--rw-r--r--   0 nihit      (501) staff       (20)     3132 2023-06-23 04:22:30.000000 refuel-autolabel-0.0.5/src/autolabel/models/hf_pipeline.py
--rw-r--r--   0 nihit      (501) staff       (20)     4404 2023-06-20 23:17:06.000000 refuel-autolabel-0.0.5/src/autolabel/models/openai.py
--rw-r--r--   0 nihit      (501) staff       (20)     3920 2023-06-20 23:17:06.000000 refuel-autolabel-0.0.5/src/autolabel/models/palm.py
--rw-r--r--   0 nihit      (501) staff       (20)     3575 2023-06-20 23:17:06.000000 refuel-autolabel-0.0.5/src/autolabel/models/refuel.py
--rw-r--r--   0 nihit      (501) staff       (20)     4625 2023-06-14 21:52:44.000000 refuel-autolabel-0.0.5/src/autolabel/schema.py
-drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.791922 refuel-autolabel-0.0.5/src/autolabel/tasks/
--rw-r--r--   0 nihit      (501) staff       (20)     1160 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.5/src/autolabel/tasks/__init__.py
--rw-r--r--   0 nihit      (501) staff       (20)     4319 2023-06-20 23:17:06.000000 refuel-autolabel-0.0.5/src/autolabel/tasks/base.py
--rw-r--r--   0 nihit      (501) staff       (20)     7409 2023-06-19 23:05:19.000000 refuel-autolabel-0.0.5/src/autolabel/tasks/classification.py
--rw-r--r--   0 nihit      (501) staff       (20)     7419 2023-06-19 23:05:19.000000 refuel-autolabel-0.0.5/src/autolabel/tasks/entity_matching.py
--rw-r--r--   0 nihit      (501) staff       (20)    12627 2023-06-19 23:05:19.000000 refuel-autolabel-0.0.5/src/autolabel/tasks/named_entity_recognition.py
--rw-r--r--   0 nihit      (501) staff       (20)     7508 2023-06-19 23:05:19.000000 refuel-autolabel-0.0.5/src/autolabel/tasks/question_answering.py
--rw-r--r--   0 nihit      (501) staff       (20)     1574 2023-06-08 20:27:49.000000 refuel-autolabel-0.0.5/src/autolabel/tasks/utils.py
--rw-r--r--   0 nihit      (501) staff       (20)     9773 2023-06-22 21:37:13.000000 refuel-autolabel-0.0.5/src/autolabel/utils.py
-drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.792946 refuel-autolabel-0.0.5/src/refuel_autolabel.egg-info/
--rw-r--r--   0 nihit      (501) staff       (20)    10926 2023-06-23 23:32:07.000000 refuel-autolabel-0.0.5/src/refuel_autolabel.egg-info/PKG-INFO
--rw-r--r--   0 nihit      (501) staff       (20)     1571 2023-06-23 23:32:07.000000 refuel-autolabel-0.0.5/src/refuel_autolabel.egg-info/SOURCES.txt
--rw-r--r--   0 nihit      (501) staff       (20)        1 2023-06-23 23:32:07.000000 refuel-autolabel-0.0.5/src/refuel_autolabel.egg-info/dependency_links.txt
--rw-r--r--   0 nihit      (501) staff       (20)      782 2023-06-23 23:32:07.000000 refuel-autolabel-0.0.5/src/refuel_autolabel.egg-info/requires.txt
--rw-r--r--   0 nihit      (501) staff       (20)       10 2023-06-23 23:32:07.000000 refuel-autolabel-0.0.5/src/refuel_autolabel.egg-info/top_level.txt
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.617916 refuel-autolabel-0.0.6/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1066 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/LICENSE
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    10361 2023-06-30 23:17:00.617696 refuel-autolabel-0.0.6/PKG-INFO
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8337 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/README.md
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2247 2023-06-30 23:16:32.000000 refuel-autolabel-0.0.6/pyproject.toml
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       38 2023-06-30 23:17:00.617963 refuel-autolabel-0.0.6/setup.cfg
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.602635 refuel-autolabel-0.0.6/src/
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.604749 refuel-autolabel-0.0.6/src/autolabel/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       63 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.6/src/autolabel/__init__.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.605527 refuel-autolabel-0.0.6/src/autolabel/cache/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       74 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/src/autolabel/cache/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      924 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.6/src/autolabel/cache/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1817 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.6/src/autolabel/cache/sqlalchemy_cache.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     9137 2023-06-15 00:37:32.000000 refuel-autolabel-0.0.6/src/autolabel/confidence.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.606230 refuel-autolabel-0.0.6/src/autolabel/configs/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       65 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/src/autolabel/configs/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1401 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/configs/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7569 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/configs/config.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4114 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/configs/schema.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.607915 refuel-autolabel-0.0.6/src/autolabel/data_models/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      195 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/src/autolabel/data_models/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2001 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.6/src/autolabel/data_models/annotation.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       71 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/src/autolabel/data_models/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2036 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.6/src/autolabel/data_models/cache.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1071 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/src/autolabel/data_models/dataset.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      928 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/src/autolabel/data_models/task.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2625 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.6/src/autolabel/data_models/task_run.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.608439 refuel-autolabel-0.0.6/src/autolabel/database/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       77 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/src/autolabel/database/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      679 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/database/engine.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2788 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.6/src/autolabel/database/state_manager.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8085 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/dataset_loader.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.609102 refuel-autolabel-0.0.6/src/autolabel/few_shot/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3233 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/few_shot/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1295 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/src/autolabel/few_shot/fixed_example_selector.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    11031 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.6/src/autolabel/few_shot/vector_store.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    19705 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/labeler.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.610564 refuel-autolabel-0.0.6/src/autolabel/models/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1965 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.6/src/autolabel/models/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2496 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/src/autolabel/models/anthropic.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4150 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.6/src/autolabel/models/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3132 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/models/hf_pipeline.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     5682 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/models/openai.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3920 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.6/src/autolabel/models/palm.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3575 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.6/src/autolabel/models/refuel.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4685 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/schema.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.612509 refuel-autolabel-0.0.6/src/autolabel/tasks/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1298 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/tasks/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4319 2023-06-22 05:07:53.000000 refuel-autolabel-0.0.6/src/autolabel/tasks/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7409 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.6/src/autolabel/tasks/classification.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7419 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.6/src/autolabel/tasks/entity_matching.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8221 2023-06-30 23:04:22.000000 refuel-autolabel-0.0.6/src/autolabel/tasks/multilabel_classification.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    12627 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.6/src/autolabel/tasks/named_entity_recognition.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7508 2023-06-20 21:44:37.000000 refuel-autolabel-0.0.6/src/autolabel/tasks/question_answering.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1574 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.6/src/autolabel/tasks/utils.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     9773 2023-06-22 21:40:05.000000 refuel-autolabel-0.0.6/src/autolabel/utils.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-30 23:17:00.617432 refuel-autolabel-0.0.6/src/refuel_autolabel.egg-info/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    10361 2023-06-30 23:17:00.000000 refuel-autolabel-0.0.6/src/refuel_autolabel.egg-info/PKG-INFO
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1652 2023-06-30 23:17:00.000000 refuel-autolabel-0.0.6/src/refuel_autolabel.egg-info/SOURCES.txt
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)        1 2023-06-30 23:17:00.000000 refuel-autolabel-0.0.6/src/refuel_autolabel.egg-info/dependency_links.txt
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      863 2023-06-30 23:17:00.000000 refuel-autolabel-0.0.6/src/refuel_autolabel.egg-info/requires.txt
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       10 2023-06-30 23:17:00.000000 refuel-autolabel-0.0.6/src/refuel_autolabel.egg-info/top_level.txt
```

### Comparing `refuel-autolabel-0.0.5/LICENSE` & `refuel-autolabel-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/PKG-INFO` & `refuel-autolabel-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refuel-autolabel
-Version: 0.0.5
+Version: 0.0.6
 Summary: Label, clean and enrich text datasets with LLMs
 Author-email: "Refuel.ai" <support@refuel.ai>
 License: MIT License
         
         Copyright (c) 2023 refuel-ai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,29 +42,33 @@
 Provides-Extra: all
 License-File: LICENSE
 
 <img alt="Refuel logo" src="https://raw.githubusercontent.com/refuel-ai/autolabel/main/docs/assets/Autolabel_blk_w_background.png">
 
 
 <h4 align="center">
-  <a href="https://docs.refuel.ai/">Docs</a> |
   <a href="https://discord.gg/fweVnRx6CU">Discord</a> |
   <a href="https://twitter.com/RefuelAI">Twitter</a> |
-  <a href="https://www.refuel.ai/">Website</a>
+  <a href="https://www.refuel.ai/">Website</a> |
+  <a href="https://www.refuel.ai/blog-posts/llm-labeling-technical-report">Benchmark</a>
 </h4>
 
 <div align="center" style="width:800px">
 
 [![lint](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/badge.svg)](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/badge.svg) ![Tests](https://github.com/refuel-ai/autolabel/actions/workflows/test.yaml/badge.svg) ![Commit Activity](https://img.shields.io/github/commit-activity/m/refuel-ai/autolabel) [![Discord](https://img.shields.io/discord/1098746693152931901)](https://discord.gg/fweVnRx6CU) [![open in colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1t-9vNLkyoyySAG_0w3eR98biBOXlMO-E?usp=sharing)
 </div>
 
 ## ⚡ Quick Install
 
 `pip install refuel-autolabel`
 
+## 📖 Documentation
+
+[https://docs.refuel.ai/](https://docs.refuel.ai/)
+
 ## 🏷 What is Autolabel
 
 Access to [large, clean and diverse](https://twitter.com/karpathy/status/1528443124577513472?lang=en) labeled datasets is a critical component for any machine learning effort to be successful. State-of-the-art LLMs like GPT-4 are able to [automatically label data](https://arxiv.org/abs/2303.15056) with [high accuracy](https://arxiv.org/abs/2303.16854), and at a fraction of the cost and time compared to manual labeling.
 
 Autolabel is a Python library to label, clean and enrich text datasets with any Large Language Models (LLM) of your choice.
 
 ## 🚀 Getting started
@@ -198,24 +202,19 @@
 In order to use Refuel hosted LLMs, you can [request access here](https://refuel-ai.typeform.com/llm-access).
 
 ## Benchmark
 
 Check out our [technical report](https://www.refuel.ai/blog-posts/llm-labeling-technical-report) to learn more about the performance of various LLMs, and human annoators, on label quality, turnaround time and cost.
 
 ## 🛠️ Roadmap
-Our goal is to allow users to label, create or enrich any dataset, with any LLM - easily and quickly.
 
-There are four focus areas for Autolabel for 2023:
+Check out our [public roadmap](https://github.com/orgs/refuel-ai/projects/15) to learn more about ongoing and planned improvements to the Autolabel library.
 
-* **Tasks**: Add support for tasks such as retrieval, attribute enrichment and text generation/writing.
-* **LLMs**: Add support for more LLMs, especially open source models like Falcon, MPT and Dolly and the ability to plug in your own LLMs. 
-* Workflows for **experimenting with your datasets** more easily: Add support for richer data types (such as PDFs and HTML documents) and the ability to run benchmarking on your data sources.
-* Techniques to **improve labeling accuracy**: Add support for automatic prompt improvement and tools for better error analysis to iteratively improve LLM performance on different tasks 
+We are always looking for suggestions and contributions from the community. Join the discussion on [Discord](https://discord.gg/fweVnRx6CU) or open a [Github issue](https://github.com/refuel-ai/autolabel/issues) to report bugs and request features.
 
-We will be releasing a more detailed roadmap soon, but we love suggestions and contributions from the community. Chat with the Refuel team and Autolabel community on [Discord](https://discord.gg/fweVnRx6CU) or open [Github issues](https://github.com/refuel-ai/autolabel/issues) to report bugs and request features.
 
 ## 🙌 Contributing
 
 Autolabel is a rapidly developing project. We welcome contributions in all forms - bug reports, pull requests and ideas for improving the library.
 
 1. Join the conversation on [Discord](https://discord.gg/fweVnRx6CU)
 2. Open an [issue](https://github.com/refuel-ai/autolabel/issues) on Github for bugs and request features.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.5 Summary: Label,
+Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.6 Summary: Label,
 clean and enrich text datasets with LLMs Author-email: "Refuel.ai"
 refuel.ai> License: MIT License Copyright (c) 2023 refuel-ai Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -19,25 +19,26 @@
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Software Development
 :: Libraries :: Python Modules Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.6 Description-Content-Type: text/
 markdown Provides-Extra: dev Provides-Extra: openai Provides-Extra: anthropic
 Provides-Extra: huggingface Provides-Extra: google Provides-Extra: all License-
 File: LICENSE [Refuel logo]
-                  *** Docs | Discord | Twitter | Website ***
+                *** Discord | Twitter | Website | Benchmark ***
  [![lint](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/
      badge.svg)](https://github.com/refuel-ai/autolabel/actions/workflows/
 black.yaml/badge.svg) ![Tests](https://github.com/refuel-ai/autolabel/actions/
    workflows/test.yaml/badge.svg) ![Commit Activity](https://img.shields.io/
       github/commit-activity/m/refuel-ai/autolabel) [![Discord](https://
 img.shields.io/discord/1098746693152931901)](https://discord.gg/fweVnRx6CU) [!
   [open in colab](https://colab.research.google.com/assets/colab-badge.svg)]
    (https://colab.research.google.com/drive/1t-9vNLkyoyySAG_0w3eR98biBOXlMO-
                                 E?usp=sharing)
-## â¡ Quick Install `pip install refuel-autolabel` ## ð· What is Autolabel
+## â¡ Quick Install `pip install refuel-autolabel` ## ð Documentation
+[https://docs.refuel.ai/](https://docs.refuel.ai/) ## ð· What is Autolabel
 Access to [large, clean and diverse](https://twitter.com/karpathy/status/
 1528443124577513472?lang=en) labeled datasets is a critical component for any
 machine learning effort to be successful. State-of-the-art LLMs like GPT-4 are
 able to [automatically label data](https://arxiv.org/abs/2303.15056) with [high
 accuracy](https://arxiv.org/abs/2303.16854), and at a fraction of the cost and
 time compared to manual labeling. Autolabel is a Python library to label, clean
 and enrich text datasets with any Large Language Models (LLM) of your choice.
@@ -102,28 +103,19 @@
 calibrate a confidence threshold for your labeling task, and then route less
 confident labels to humans, while you still get the benefits of auto-labeling
 for the confident examples. In order to use Refuel hosted LLMs, you can
 [request access here](https://refuel-ai.typeform.com/llm-access). ## Benchmark
 Check out our [technical report](https://www.refuel.ai/blog-posts/llm-labeling-
 technical-report) to learn more about the performance of various LLMs, and
 human annoators, on label quality, turnaround time and cost. ## ð ï¸ Roadmap
-Our goal is to allow users to label, create or enrich any dataset, with any LLM
-- easily and quickly. There are four focus areas for Autolabel for 2023: *
-**Tasks**: Add support for tasks such as retrieval, attribute enrichment and
-text generation/writing. * **LLMs**: Add support for more LLMs, especially open
-source models like Falcon, MPT and Dolly and the ability to plug in your own
-LLMs. * Workflows for **experimenting with your datasets** more easily: Add
-support for richer data types (such as PDFs and HTML documents) and the ability
-to run benchmarking on your data sources. * Techniques to **improve labeling
-accuracy**: Add support for automatic prompt improvement and tools for better
-error analysis to iteratively improve LLM performance on different tasks We
-will be releasing a more detailed roadmap soon, but we love suggestions and
-contributions from the community. Chat with the Refuel team and Autolabel
-community on [Discord](https://discord.gg/fweVnRx6CU) or open [Github issues]
-(https://github.com/refuel-ai/autolabel/issues) to report bugs and request
-features. ## ð Contributing Autolabel is a rapidly developing project. We
-welcome contributions in all forms - bug reports, pull requests and ideas for
-improving the library. 1. Join the conversation on [Discord](https://
+Check out our [public roadmap](https://github.com/orgs/refuel-ai/projects/15)
+to learn more about ongoing and planned improvements to the Autolabel library.
+We are always looking for suggestions and contributions from the community.
+Join the discussion on [Discord](https://discord.gg/fweVnRx6CU) or open a
+[Github issue](https://github.com/refuel-ai/autolabel/issues) to report bugs
+and request features. ## ð Contributing Autolabel is a rapidly developing
+project. We welcome contributions in all forms - bug reports, pull requests and
+ideas for improving the library. 1. Join the conversation on [Discord](https://
 discord.gg/fweVnRx6CU) 2. Open an [issue](https://github.com/refuel-ai/
 autolabel/issues) on Github for bugs and request features. 3. Grab an open
 issue, and submit a [pull request](https://github.com/refuel-ai/autolabel/blob/
 main/CONTRIBUTING.md).
```

### Comparing `refuel-autolabel-0.0.5/README.md` & `refuel-autolabel-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 <img alt="Refuel logo" src="https://raw.githubusercontent.com/refuel-ai/autolabel/main/docs/assets/Autolabel_blk_w_background.png">
 
 
 <h4 align="center">
-  <a href="https://docs.refuel.ai/">Docs</a> |
   <a href="https://discord.gg/fweVnRx6CU">Discord</a> |
   <a href="https://twitter.com/RefuelAI">Twitter</a> |
-  <a href="https://www.refuel.ai/">Website</a>
+  <a href="https://www.refuel.ai/">Website</a> |
+  <a href="https://www.refuel.ai/blog-posts/llm-labeling-technical-report">Benchmark</a>
 </h4>
 
 <div align="center" style="width:800px">
 
 [![lint](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/badge.svg)](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/badge.svg) ![Tests](https://github.com/refuel-ai/autolabel/actions/workflows/test.yaml/badge.svg) ![Commit Activity](https://img.shields.io/github/commit-activity/m/refuel-ai/autolabel) [![Discord](https://img.shields.io/discord/1098746693152931901)](https://discord.gg/fweVnRx6CU) [![open in colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1t-9vNLkyoyySAG_0w3eR98biBOXlMO-E?usp=sharing)
 </div>
 
 ## ⚡ Quick Install
 
 `pip install refuel-autolabel`
 
+## 📖 Documentation
+
+[https://docs.refuel.ai/](https://docs.refuel.ai/)
+
 ## 🏷 What is Autolabel
 
 Access to [large, clean and diverse](https://twitter.com/karpathy/status/1528443124577513472?lang=en) labeled datasets is a critical component for any machine learning effort to be successful. State-of-the-art LLMs like GPT-4 are able to [automatically label data](https://arxiv.org/abs/2303.15056) with [high accuracy](https://arxiv.org/abs/2303.16854), and at a fraction of the cost and time compared to manual labeling.
 
 Autolabel is a Python library to label, clean and enrich text datasets with any Large Language Models (LLM) of your choice.
 
 ## 🚀 Getting started
@@ -154,24 +158,19 @@
 In order to use Refuel hosted LLMs, you can [request access here](https://refuel-ai.typeform.com/llm-access).
 
 ## Benchmark
 
 Check out our [technical report](https://www.refuel.ai/blog-posts/llm-labeling-technical-report) to learn more about the performance of various LLMs, and human annoators, on label quality, turnaround time and cost.
 
 ## 🛠️ Roadmap
-Our goal is to allow users to label, create or enrich any dataset, with any LLM - easily and quickly.
 
-There are four focus areas for Autolabel for 2023:
+Check out our [public roadmap](https://github.com/orgs/refuel-ai/projects/15) to learn more about ongoing and planned improvements to the Autolabel library.
 
-* **Tasks**: Add support for tasks such as retrieval, attribute enrichment and text generation/writing.
-* **LLMs**: Add support for more LLMs, especially open source models like Falcon, MPT and Dolly and the ability to plug in your own LLMs. 
-* Workflows for **experimenting with your datasets** more easily: Add support for richer data types (such as PDFs and HTML documents) and the ability to run benchmarking on your data sources.
-* Techniques to **improve labeling accuracy**: Add support for automatic prompt improvement and tools for better error analysis to iteratively improve LLM performance on different tasks 
+We are always looking for suggestions and contributions from the community. Join the discussion on [Discord](https://discord.gg/fweVnRx6CU) or open a [Github issue](https://github.com/refuel-ai/autolabel/issues) to report bugs and request features.
 
-We will be releasing a more detailed roadmap soon, but we love suggestions and contributions from the community. Chat with the Refuel team and Autolabel community on [Discord](https://discord.gg/fweVnRx6CU) or open [Github issues](https://github.com/refuel-ai/autolabel/issues) to report bugs and request features.
 
 ## 🙌 Contributing
 
 Autolabel is a rapidly developing project. We welcome contributions in all forms - bug reports, pull requests and ideas for improving the library.
 
 1. Join the conversation on [Discord](https://discord.gg/fweVnRx6CU)
 2. Open an [issue](https://github.com/refuel-ai/autolabel/issues) on Github for bugs and request features.
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
 [Refuel logo]
-                  *** Docs | Discord | Twitter | Website ***
+                *** Discord | Twitter | Website | Benchmark ***
  [![lint](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/
      badge.svg)](https://github.com/refuel-ai/autolabel/actions/workflows/
 black.yaml/badge.svg) ![Tests](https://github.com/refuel-ai/autolabel/actions/
    workflows/test.yaml/badge.svg) ![Commit Activity](https://img.shields.io/
       github/commit-activity/m/refuel-ai/autolabel) [![Discord](https://
 img.shields.io/discord/1098746693152931901)](https://discord.gg/fweVnRx6CU) [!
   [open in colab](https://colab.research.google.com/assets/colab-badge.svg)]
    (https://colab.research.google.com/drive/1t-9vNLkyoyySAG_0w3eR98biBOXlMO-
                                 E?usp=sharing)
-## â¡ Quick Install `pip install refuel-autolabel` ## ð· What is Autolabel
+## â¡ Quick Install `pip install refuel-autolabel` ## ð Documentation
+[https://docs.refuel.ai/](https://docs.refuel.ai/) ## ð· What is Autolabel
 Access to [large, clean and diverse](https://twitter.com/karpathy/status/
 1528443124577513472?lang=en) labeled datasets is a critical component for any
 machine learning effort to be successful. State-of-the-art LLMs like GPT-4 are
 able to [automatically label data](https://arxiv.org/abs/2303.15056) with [high
 accuracy](https://arxiv.org/abs/2303.16854), and at a fraction of the cost and
 time compared to manual labeling. Autolabel is a Python library to label, clean
 and enrich text datasets with any Large Language Models (LLM) of your choice.
@@ -78,28 +79,19 @@
 calibrate a confidence threshold for your labeling task, and then route less
 confident labels to humans, while you still get the benefits of auto-labeling
 for the confident examples. In order to use Refuel hosted LLMs, you can
 [request access here](https://refuel-ai.typeform.com/llm-access). ## Benchmark
 Check out our [technical report](https://www.refuel.ai/blog-posts/llm-labeling-
 technical-report) to learn more about the performance of various LLMs, and
 human annoators, on label quality, turnaround time and cost. ## ð ï¸ Roadmap
-Our goal is to allow users to label, create or enrich any dataset, with any LLM
-- easily and quickly. There are four focus areas for Autolabel for 2023: *
-**Tasks**: Add support for tasks such as retrieval, attribute enrichment and
-text generation/writing. * **LLMs**: Add support for more LLMs, especially open
-source models like Falcon, MPT and Dolly and the ability to plug in your own
-LLMs. * Workflows for **experimenting with your datasets** more easily: Add
-support for richer data types (such as PDFs and HTML documents) and the ability
-to run benchmarking on your data sources. * Techniques to **improve labeling
-accuracy**: Add support for automatic prompt improvement and tools for better
-error analysis to iteratively improve LLM performance on different tasks We
-will be releasing a more detailed roadmap soon, but we love suggestions and
-contributions from the community. Chat with the Refuel team and Autolabel
-community on [Discord](https://discord.gg/fweVnRx6CU) or open [Github issues]
-(https://github.com/refuel-ai/autolabel/issues) to report bugs and request
-features. ## ð Contributing Autolabel is a rapidly developing project. We
-welcome contributions in all forms - bug reports, pull requests and ideas for
-improving the library. 1. Join the conversation on [Discord](https://
+Check out our [public roadmap](https://github.com/orgs/refuel-ai/projects/15)
+to learn more about ongoing and planned improvements to the Autolabel library.
+We are always looking for suggestions and contributions from the community.
+Join the discussion on [Discord](https://discord.gg/fweVnRx6CU) or open a
+[Github issue](https://github.com/refuel-ai/autolabel/issues) to report bugs
+and request features. ## ð Contributing Autolabel is a rapidly developing
+project. We welcome contributions in all forms - bug reports, pull requests and
+ideas for improving the library. 1. Join the conversation on [Discord](https://
 discord.gg/fweVnRx6CU) 2. Open an [issue](https://github.com/refuel-ai/
 autolabel/issues) on Github for bugs and request features. 3. Grab an open
 issue, and submit a [pull request](https://github.com/refuel-ai/autolabel/blob/
 main/CONTRIBUTING.md).
```

### Comparing `refuel-autolabel-0.0.5/pyproject.toml` & `refuel-autolabel-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0.0", "wheel >= 0.38"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "refuel-autolabel"
-version = "0.0.5"
+version = "0.0.6"
 description = "Label, clean and enrich text datasets with LLMs"
 readme = "README.md"
 authors = [{ name = "Refuel.ai", email = "support@refuel.ai" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
@@ -30,15 +30,17 @@
     "SQLAlchemy == 1.4.47",
     "regex >= 2023.6.3",
     "rich >= 13.3.5",
     "scipy >= 1.10.1",
     "pydantic >= 1.10.9",
     "torch >= 1.10.0",
     "matplotlib >= 3.5.0",
-    "wget >= 3.2"
+    "wget >= 3.2",
+    "ipywidgets == 8.0.6",
+    "jsonschema >= 4.17.3"
 ]
 requires-python = ">=3.6"
 
 [project.optional-dependencies]
 dev = [
     "black",
     "bumpver",
@@ -56,34 +58,36 @@
     "pre-commit"
 ]
 openai = [
     "openai >= 0.27.4",
     "tiktoken >= 0.3.3"
 ]
 anthropic = [
-    "anthropic >= 0.2.6"
+    "anthropic == 0.2.6"
 ]
 huggingface = [
-    "transformers >= 4.25.0"
+    "transformers >= 4.25.0",
+    "sentence_transformers"
 ]
 google = [
     "google-cloud-aiplatform>=1.25.0"
 ]
 all = [
     "black",
     "bumpver",
     "pip-tools",
     "pytest",
     "pytest-mock",
     "pre-commit",
     "openai >= 0.27.4",
     "tiktoken >= 0.3.3",
-    "anthropic >= 0.2.6",
+    "anthropic == 0.2.6",
     "transformers >= 4.25.0",
-    "google-cloud-aiplatform>=1.25.0"
+    "google-cloud-aiplatform>=1.25.0",
+    "sentence_transformers"
 ]
 
 [project.urls]
 Homepage = "https://github.com/refuel-ai/autolabel"
 
 [tool.black]
 include = '\.pyi?$'
```

### Comparing `refuel-autolabel-0.0.5/src/autolabel/cache/base.py` & `refuel-autolabel-0.0.6/src/autolabel/cache/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/cache/sqlalchemy_cache.py` & `refuel-autolabel-0.0.6/src/autolabel/cache/sqlalchemy_cache.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/confidence.py` & `refuel-autolabel-0.0.6/src/autolabel/confidence.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/configs/base.py` & `refuel-autolabel-0.0.6/src/autolabel/configs/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,18 +23,14 @@
                 return json.load(config_file)
         except ValueError as e:
             logger.error(
                 f"JSON file: {json_file_path} not loaded successfully. Error: {repr(e)}"
             )
             return {}
 
-    def _validate(self) -> bool:
-        """Returns true if the config settings are valid"""
-        return True
-
     def get(self, key: str, default_value: Any = None) -> Any:
         return self.config.get(key, default_value)
 
     def keys(self) -> List:
         return list(self.config.keys())
 
     def __getitem__(self, key):
```

### Comparing `refuel-autolabel-0.0.5/src/autolabel/configs/config.py` & `refuel-autolabel-0.0.6/src/autolabel/configs/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 from functools import cached_property
 from typing import Dict, List, Union
 
+from jsonschema import validate
+
 from .base import BaseConfig
 
 
 class AutolabelConfig(BaseConfig):
     """Class to parse and store configs passed to Autolabel agent."""
 
     # Top-level config keys
     TASK_NAME_KEY = "task_name"
     TASK_TYPE_KEY = "task_type"
     DATASET_CONFIG_KEY = "dataset"
     MODEL_CONFIG_KEY = "model"
+    EMBEDDING_CONFIG_KEY = "embedding"
     PROMPT_CONFIG_KEY = "prompt"
 
     # Dataset config keys (config["dataset"][<key>])
     LABEL_COLUMN_KEY = "label_column"
+    LABEL_SEPARATOR_KEY = "label_separator"
     EXPLANATION_COLUMN_KEY = "explanation_column"
     TEXT_COLUMN_KEY = "text_column"
     DELIMITER_KEY = "delimiter"
 
     # Model config keys (config["model"][<key>])
     PROVIDER_KEY = "provider"
     MODEL_NAME_KEY = "name"
     MODEL_PARAMS_KEY = "params"
     COMPUTE_CONFIDENCE_KEY = "compute_confidence"
+    LOGIT_BIAS_KEY = "logit_bias"
+
+    # Embedding config keys (config["embedding"][<key>])
+    EMBEDDING_PROVIDER_KEY = "provider"
+    EMBEDDING_MODEL_NAME_KEY = "model"
 
     # Prompt config keys (config["prompt"][<key>])
     TASK_GUIDELINE_KEY = "task_guidelines"
     VALID_LABELS_KEY = "labels"
     FEW_SHOT_EXAMPLE_SET_KEY = "few_shot_examples"
     FEW_SHOT_SELECTION_ALGORITHM_KEY = "few_shot_selection"
     FEW_SHOT_NUM_KEY = "few_shot_num"
@@ -36,25 +45,40 @@
     OUTPUT_GUIDELINE_KEY = "output_guidelines"
     OUTPUT_FORMAT_KEY = "output_format"
     CHAIN_OF_THOUGHT_KEY = "chain_of_thought"
 
     def __init__(self, config: Union[str, Dict]) -> None:
         super().__init__(config)
 
+    def _validate(self) -> bool:
+        """Returns true if the config settings are valid"""
+        from autolabel.configs.schema import schema
+
+        validate(
+            instance=self.config,
+            schema=schema,
+        )
+        return True
+
     @cached_property
     def _dataset_config(self) -> Dict:
         """Returns information about the dataset being used for labeling (e.g. label_column, text_column, delimiter)"""
         return self.config.get(self.DATASET_CONFIG_KEY, {})
 
     @cached_property
     def _model_config(self) -> Dict:
         """Returns information about the model being used for labeling (e.g. provider name, model name, parameters)"""
         return self.config[self.MODEL_CONFIG_KEY]
 
     @cached_property
+    def _embedding_config(self) -> Dict:
+        """Returns information about the model being used for computing embeddings (e.g. provider name, model name)"""
+        return self.config.get(self.EMBEDDING_CONFIG_KEY, {})
+
+    @cached_property
     def _prompt_config(self) -> Dict:
         """Returns information about the prompt we are passing to the model (e.g. task guidelines, examples, output formatting)"""
         return self.config[self.PROMPT_CONFIG_KEY]
 
     # project and task definition config
     def task_name(self) -> str:
         return self.config[self.TASK_NAME_KEY]
@@ -64,14 +88,18 @@
         return self.config[self.TASK_TYPE_KEY]
 
     # Dataset config
     def label_column(self) -> str:
         """Returns the name of the column containing labels for the dataset. Used for comparing accuracy of autolabel results vs ground truth"""
         return self._dataset_config.get(self.LABEL_COLUMN_KEY, None)
 
+    def label_separator(self) -> str:
+        """Returns the token used to seperate multiple labels in the dataset. Defaults to a semicolon ';'"""
+        return self._dataset_config.get(self.LABEL_SEPARATOR_KEY, ";")
+
     def text_column(self) -> str:
         """Returns the name of the column containing text data we intend to label"""
         return self._dataset_config.get(self.TEXT_COLUMN_KEY, None)
 
     def explanation_column(self) -> str:
         """Returns the name of the column containing an explanation as to why the data is labeled a certain way"""
         return self._dataset_config.get(self.EXPLANATION_COLUMN_KEY, None)
@@ -93,14 +121,27 @@
         """Returns a dict of configured settings for the model (e.g. hyperparameters)"""
         return self._model_config.get(self.MODEL_PARAMS_KEY, {})
 
     def confidence(self) -> bool:
         """Returns true if the model is able to return a confidence score along with its predictions"""
         return self._model_config.get(self.COMPUTE_CONFIDENCE_KEY, False)
 
+    def logit_bias(self) -> bool:
+        """Returns true if the model is configured to use a logit bias"""
+        return self._model_config.get(self.LOGIT_BIAS_KEY, False)
+
+    # Embedding config
+    def embedding_provider(self) -> str:
+        """Returns the name of the entity that provides the model used for computing embeddings"""
+        return self._embedding_config.get(self.EMBEDDING_PROVIDER_KEY, self.provider())
+
+    def embedding_model_name(self) -> str:
+        """Returns the name of the model being used for computing embeddings (e.g. sentence-transformers/all-mpnet-base-v2)"""
+        return self._embedding_config.get(self.EMBEDDING_MODEL_NAME_KEY, None)
+
     # Prompt config
     def task_guidelines(self) -> str:
         return self._prompt_config.get(self.TASK_GUIDELINE_KEY, "")
 
     def labels_list(self) -> List[str]:
         """Returns a list of valid labels"""
         return self._prompt_config.get(self.VALID_LABELS_KEY, [])
```

### Comparing `refuel-autolabel-0.0.5/src/autolabel/data_models/annotation.py` & `refuel-autolabel-0.0.6/src/autolabel/data_models/annotation.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/data_models/cache.py` & `refuel-autolabel-0.0.6/src/autolabel/data_models/cache.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/data_models/dataset.py` & `refuel-autolabel-0.0.6/src/autolabel/data_models/dataset.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/data_models/task.py` & `refuel-autolabel-0.0.6/src/autolabel/data_models/task.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/data_models/task_run.py` & `refuel-autolabel-0.0.6/src/autolabel/data_models/task_run.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/database/state_manager.py` & `refuel-autolabel-0.0.6/src/autolabel/database/state_manager.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/dataset_loader.py` & `refuel-autolabel-0.0.6/src/autolabel/dataset_loader.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/few_shot/fixed_example_selector.py` & `refuel-autolabel-0.0.6/src/autolabel/few_shot/fixed_example_selector.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/few_shot/vector_store.py` & `refuel-autolabel-0.0.6/src/autolabel/few_shot/vector_store.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/labeler.py` & `refuel-autolabel-0.0.6/src/autolabel/labeler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import sys
 from typing import Dict, List, Optional, Tuple, Union
 import logging
 
 import numpy as np
 import pandas as pd
 from rich import print as pprint
@@ -296,14 +297,18 @@
         start_index: int = 0,
     ) -> None:
         """Calculates and prints the cost of calling autolabel.run() on a given dataset
 
         Args:
             dataset: path to a CSV dataset
         """
+        if self.config.confidence() and "REFUEL_API_KEY" not in os.environ:
+            raise ValueError(
+                "REFUEL_API_KEY environment variable must be set to compute confidence scores. You can request an API key at https://refuel-ai.typeform.com/llm-access."
+            )
 
         dataset_loader = DatasetLoader(dataset, self.config, max_items, start_index)
 
         prompt_list = []
         total_cost = 0
 
         # Get the seed examples from the dataset config
```

### Comparing `refuel-autolabel-0.0.5/src/autolabel/models/__init__.py` & `refuel-autolabel-0.0.6/src/autolabel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/models/anthropic.py` & `refuel-autolabel-0.0.6/src/autolabel/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/models/base.py` & `refuel-autolabel-0.0.6/src/autolabel/models/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/models/hf_pipeline.py` & `refuel-autolabel-0.0.6/src/autolabel/models/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/models/openai.py` & `refuel-autolabel-0.0.6/src/autolabel/models/palm.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,41 @@
 from functools import cached_property
 from typing import List, Optional
+import logging
 
-from langchain.chat_models import ChatOpenAI
-from langchain.llms import OpenAI
+from langchain.chat_models import ChatVertexAI
+from langchain.llms import VertexAI
 from langchain.schema import LLMResult, HumanMessage, Generation
-import tiktoken
 
 from autolabel.models import BaseModel
 from autolabel.configs import AutolabelConfig
 from autolabel.cache import BaseCache
 
-
-class OpenAILLM(BaseModel):
-    CHAT_ENGINE_MODELS = [
-        "gpt-3.5-turbo",
-        "gpt-3.5-turbo-0613",
-        "gpt-3.5-turbo-16k",
-        "gpt-3.5-turbo-16k-0613",
-        "gpt-4",
-        "gpt-4-0613",
-        "gpt-4-32k",
-        "gpt-4-32k-0613",
-    ]
-    MODELS_WITH_TOKEN_PROBS = ["text-curie-001", "text-davinci-003"]
-
-    # Default parameters for OpenAILLM
-    DEFAULT_MODEL = "gpt-3.5-turbo"
-    DEFAULT_PARAMS_COMPLETION_ENGINE = {
-        "max_tokens": 1000,
-        "temperature": 0.0,
-        "model_kwargs": {"logprobs": 1},
-    }
-    DEFAULT_PARAMS_CHAT_ENGINE = {
-        "max_tokens": 1000,
-        "temperature": 0.0,
-    }
-
-    # Reference: https://openai.com/pricing
-    COST_PER_PROMPT_TOKEN = {
-        "text-davinci-003": 0.02 / 1000,
-        "text-curie-001": 0.002 / 1000,
-        "gpt-3.5-turbo": 0.0015 / 1000,
-        "gpt-3.5-turbo-0613": 0.0015 / 1000,
-        "gpt-3.5-turbo-16k": 0.003 / 1000,
-        "gpt-3.5-turbo-16k-0613": 0.003 / 1000,
-        "gpt-4": 0.03 / 1000,
-        "gpt-4-0613": 0.03 / 1000,
-        "gpt-4-32k": 0.06 / 1000,
-        "gpt-4-32k-0613": 0.06 / 1000,
-    }
-    COST_PER_COMPLETION_TOKEN = {
-        "text-davinci-003": 0.02 / 1000,
-        "text-curie-001": 0.002 / 1000,
-        "gpt-3.5-turbo": 0.002 / 1000,
-        "gpt-3.5-turbo-0613": 0.002 / 1000,
-        "gpt-3.5-turbo-16k": 0.004 / 1000,
-        "gpt-3.5-turbo-16k-0613": 0.004 / 1000,
-        "gpt-4": 0.06 / 1000,
-        "gpt-4-0613": 0.06 / 1000,
-        "gpt-4-32k": 0.12 / 1000,
-        "gpt-4-32k-0613": 0.12 / 1000,
+from tenacity import (
+    before_sleep_log,
+    retry,
+    stop_after_attempt,
+    wait_exponential,
+)
+
+logger = logging.getLogger(__name__)
+
+
+class PaLMLLM(BaseModel):
+    SEP_REPLACEMENT_TOKEN = "@@"
+    CHAT_ENGINE_MODELS = ["chat-bison@001"]
+
+    DEFAULT_MODEL = "text-bison@001"
+    DEFAULT_PARAMS = {"temperature": 0}
+
+    # Reference: https://cloud.google.com/vertex-ai/pricing
+    COST_PER_CHARACTER = {
+        "text-bison@001": 0.001 / 1000,
+        "chat-bison@001": 0.0005 / 1000,
+        "textembedding-gecko@001": 0.0001 / 1000,
     }
 
     @cached_property
     def _engine(self) -> str:
         if self.model_name is not None and self.model_name in self.CHAT_ENGINE_MODELS:
             return "chat"
         else:
@@ -72,50 +44,65 @@
     def __init__(self, config: AutolabelConfig, cache: BaseCache = None) -> None:
         super().__init__(config, cache)
         # populate model name
         self.model_name = config.model_name() or self.DEFAULT_MODEL
 
         # populate model params and initialize the LLM
         model_params = config.model_params()
+        self.model_params = {
+            **self.DEFAULT_PARAMS,
+            **model_params,
+        }
         if self._engine == "chat":
-            self.model_params = {**self.DEFAULT_PARAMS_CHAT_ENGINE, **model_params}
-            self.llm = ChatOpenAI(model_name=self.model_name, **self.model_params)
+            self.llm = ChatVertexAI(model_name=self.model_name, **self.model_params)
         else:
-            self.model_params = {
-                **self.DEFAULT_PARAMS_COMPLETION_ENGINE,
-                **model_params,
-            }
-            self.llm = OpenAI(model_name=self.model_name, **self.model_params)
+            self.llm = VertexAI(model_name=self.model_name, **self.model_params)
+
+    @retry(
+        reraise=True,
+        stop=stop_after_attempt(5),
+        wait=wait_exponential(multiplier=1, min=2, max=10),
+        before_sleep=before_sleep_log(logger, logging.WARNING),
+    )
+    def _label_with_retry(self, prompts: List[str]) -> LLMResult:
+        return self.llm.generate(prompts)
 
     def _label(self, prompts: List[str]) -> LLMResult:
+        for prompt in prompts:
+            if self.SEP_REPLACEMENT_TOKEN in prompt:
+                logger.warning(
+                    f"""Current prompt contains {self.SEP_REPLACEMENT_TOKEN} 
+                                which is currently used as a separator token by refuel
+                                llm. It is highly recommended to avoid having any
+                                occurences of this substring in the prompt.
+                            """
+                )
+        prompts = [
+            prompt.replace("\n", self.SEP_REPLACEMENT_TOKEN) for prompt in prompts
+        ]
         if self._engine == "chat":
             # Need to convert list[prompts] -> list[messages]
             # Currently the entire prompt is stuck into the "human message"
             # We might consider breaking this up into human vs system message in future
             prompts = [[HumanMessage(content=prompt)] for prompt in prompts]
+
         try:
-            return self.llm.generate(prompts)
+            result = self._label_with_retry(prompts)
+            for generations in result.generations:
+                for generation in generations:
+                    generation.text = generation.text.replace(
+                        self.SEP_REPLACEMENT_TOKEN, "\n"
+                    )
+            return result
         except Exception as e:
-            print(f"Error generating from LLM: {e}, returning empty result")
-            generations = [[Generation(text="")] for _ in prompts]
-            return LLMResult(generations=generations)
+            logger.error(f"Error generating from LLM: {e}.")
+        generations = [[Generation(text="")] for _ in prompts]
+        return LLMResult(generations=generations)
 
     def get_cost(self, prompt: str, label: Optional[str] = "") -> float:
-        encoding = tiktoken.encoding_for_model(self.model_name)
-        num_prompt_toks = len(encoding.encode(prompt))
-        if label:
-            num_label_toks = len(encoding.encode(label))
-        else:
-            # get an upper bound
-            num_label_toks = self.model_params["max_tokens"]
-
-        cost_per_prompt_token = self.COST_PER_PROMPT_TOKEN[self.model_name]
-        cost_per_completion_token = self.COST_PER_COMPLETION_TOKEN[self.model_name]
-        return (num_prompt_toks * cost_per_prompt_token) + (
-            num_label_toks * cost_per_completion_token
-        )
+        if self.model_name is None:
+            return 0.0
+        cost_per_char = self.COST_PER_CHARACTER.get(self.model_name, 0.0)
+        return cost_per_char * len(prompt)
 
     def returns_token_probs(self) -> bool:
-        return (
-            self.model_name is not None
-            and self.model_name in self.MODELS_WITH_TOKEN_PROBS
-        )
+        return False
```

### Comparing `refuel-autolabel-0.0.5/src/autolabel/models/refuel.py` & `refuel-autolabel-0.0.6/src/autolabel/models/refuel.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/schema.py` & `refuel-autolabel-0.0.6/src/autolabel/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 class TaskType(str, Enum):
     """Enum containing all the types of tasks that autolabeler currently supports"""
 
     CLASSIFICATION = "classification"
     NAMED_ENTITY_RECOGNITION = "named_entity_recognition"
     QUESTION_ANSWERING = "question_answering"
     ENTITY_MATCHING = "entity_matching"
+    MULTILABEL_CLASSIFICATION = "multilabel_classification"
 
 
 class FewShotAlgorithm(str, Enum):
     """Enum of supported algorithms for choosing which examples to provide the LLM in its instruction prompt"""
 
     FIXED = "fixed"
     SEMANTIC_SIMILARITY = "semantic_similarity"
```

### Comparing `refuel-autolabel-0.0.5/src/autolabel/tasks/__init__.py` & `refuel-autolabel-0.0.6/src/autolabel/tasks/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 import logging
 
 from .base import BaseTask
 from .classification import ClassificationTask
 from .entity_matching import EntityMatchingTask
 from .question_answering import QuestionAnsweringTask
 from .named_entity_recognition import NamedEntityRecognitionTask
+from .multilabel_classification import MultilabelClassificationTask
 
 from autolabel.configs import AutolabelConfig
 from autolabel.schema import TaskType
 
 TASK_TYPE_TO_IMPLEMENTATION: Dict[TaskType, BaseTask] = {
     TaskType.CLASSIFICATION: ClassificationTask,
     TaskType.NAMED_ENTITY_RECOGNITION: NamedEntityRecognitionTask,
     TaskType.QUESTION_ANSWERING: QuestionAnsweringTask,
     TaskType.ENTITY_MATCHING: EntityMatchingTask,
+    TaskType.MULTILABEL_CLASSIFICATION: MultilabelClassificationTask,
 }
 
 logger = logging.getLogger(__name__)
 
 
 class TaskFactory:
     @staticmethod
```

### Comparing `refuel-autolabel-0.0.5/src/autolabel/tasks/base.py` & `refuel-autolabel-0.0.6/src/autolabel/tasks/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/tasks/classification.py` & `refuel-autolabel-0.0.6/src/autolabel/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/tasks/entity_matching.py` & `refuel-autolabel-0.0.6/src/autolabel/tasks/entity_matching.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/tasks/named_entity_recognition.py` & `refuel-autolabel-0.0.6/src/autolabel/tasks/named_entity_recognition.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/tasks/question_answering.py` & `refuel-autolabel-0.0.6/src/autolabel/tasks/question_answering.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/tasks/utils.py` & `refuel-autolabel-0.0.6/src/autolabel/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/autolabel/utils.py` & `refuel-autolabel-0.0.6/src/autolabel/utils.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.5/src/refuel_autolabel.egg-info/PKG-INFO` & `refuel-autolabel-0.0.6/src/refuel_autolabel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refuel-autolabel
-Version: 0.0.5
+Version: 0.0.6
 Summary: Label, clean and enrich text datasets with LLMs
 Author-email: "Refuel.ai" <support@refuel.ai>
 License: MIT License
         
         Copyright (c) 2023 refuel-ai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,29 +42,33 @@
 Provides-Extra: all
 License-File: LICENSE
 
 <img alt="Refuel logo" src="https://raw.githubusercontent.com/refuel-ai/autolabel/main/docs/assets/Autolabel_blk_w_background.png">
 
 
 <h4 align="center">
-  <a href="https://docs.refuel.ai/">Docs</a> |
   <a href="https://discord.gg/fweVnRx6CU">Discord</a> |
   <a href="https://twitter.com/RefuelAI">Twitter</a> |
-  <a href="https://www.refuel.ai/">Website</a>
+  <a href="https://www.refuel.ai/">Website</a> |
+  <a href="https://www.refuel.ai/blog-posts/llm-labeling-technical-report">Benchmark</a>
 </h4>
 
 <div align="center" style="width:800px">
 
 [![lint](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/badge.svg)](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/badge.svg) ![Tests](https://github.com/refuel-ai/autolabel/actions/workflows/test.yaml/badge.svg) ![Commit Activity](https://img.shields.io/github/commit-activity/m/refuel-ai/autolabel) [![Discord](https://img.shields.io/discord/1098746693152931901)](https://discord.gg/fweVnRx6CU) [![open in colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1t-9vNLkyoyySAG_0w3eR98biBOXlMO-E?usp=sharing)
 </div>
 
 ## ⚡ Quick Install
 
 `pip install refuel-autolabel`
 
+## 📖 Documentation
+
+[https://docs.refuel.ai/](https://docs.refuel.ai/)
+
 ## 🏷 What is Autolabel
 
 Access to [large, clean and diverse](https://twitter.com/karpathy/status/1528443124577513472?lang=en) labeled datasets is a critical component for any machine learning effort to be successful. State-of-the-art LLMs like GPT-4 are able to [automatically label data](https://arxiv.org/abs/2303.15056) with [high accuracy](https://arxiv.org/abs/2303.16854), and at a fraction of the cost and time compared to manual labeling.
 
 Autolabel is a Python library to label, clean and enrich text datasets with any Large Language Models (LLM) of your choice.
 
 ## 🚀 Getting started
@@ -198,24 +202,19 @@
 In order to use Refuel hosted LLMs, you can [request access here](https://refuel-ai.typeform.com/llm-access).
 
 ## Benchmark
 
 Check out our [technical report](https://www.refuel.ai/blog-posts/llm-labeling-technical-report) to learn more about the performance of various LLMs, and human annoators, on label quality, turnaround time and cost.
 
 ## 🛠️ Roadmap
-Our goal is to allow users to label, create or enrich any dataset, with any LLM - easily and quickly.
 
-There are four focus areas for Autolabel for 2023:
+Check out our [public roadmap](https://github.com/orgs/refuel-ai/projects/15) to learn more about ongoing and planned improvements to the Autolabel library.
 
-* **Tasks**: Add support for tasks such as retrieval, attribute enrichment and text generation/writing.
-* **LLMs**: Add support for more LLMs, especially open source models like Falcon, MPT and Dolly and the ability to plug in your own LLMs. 
-* Workflows for **experimenting with your datasets** more easily: Add support for richer data types (such as PDFs and HTML documents) and the ability to run benchmarking on your data sources.
-* Techniques to **improve labeling accuracy**: Add support for automatic prompt improvement and tools for better error analysis to iteratively improve LLM performance on different tasks 
+We are always looking for suggestions and contributions from the community. Join the discussion on [Discord](https://discord.gg/fweVnRx6CU) or open a [Github issue](https://github.com/refuel-ai/autolabel/issues) to report bugs and request features.
 
-We will be releasing a more detailed roadmap soon, but we love suggestions and contributions from the community. Chat with the Refuel team and Autolabel community on [Discord](https://discord.gg/fweVnRx6CU) or open [Github issues](https://github.com/refuel-ai/autolabel/issues) to report bugs and request features.
 
 ## 🙌 Contributing
 
 Autolabel is a rapidly developing project. We welcome contributions in all forms - bug reports, pull requests and ideas for improving the library.
 
 1. Join the conversation on [Discord](https://discord.gg/fweVnRx6CU)
 2. Open an [issue](https://github.com/refuel-ai/autolabel/issues) on Github for bugs and request features.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.5 Summary: Label,
+Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.6 Summary: Label,
 clean and enrich text datasets with LLMs Author-email: "Refuel.ai"
 refuel.ai> License: MIT License Copyright (c) 2023 refuel-ai Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -19,25 +19,26 @@
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Software Development
 :: Libraries :: Python Modules Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.6 Description-Content-Type: text/
 markdown Provides-Extra: dev Provides-Extra: openai Provides-Extra: anthropic
 Provides-Extra: huggingface Provides-Extra: google Provides-Extra: all License-
 File: LICENSE [Refuel logo]
-                  *** Docs | Discord | Twitter | Website ***
+                *** Discord | Twitter | Website | Benchmark ***
  [![lint](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/
      badge.svg)](https://github.com/refuel-ai/autolabel/actions/workflows/
 black.yaml/badge.svg) ![Tests](https://github.com/refuel-ai/autolabel/actions/
    workflows/test.yaml/badge.svg) ![Commit Activity](https://img.shields.io/
       github/commit-activity/m/refuel-ai/autolabel) [![Discord](https://
 img.shields.io/discord/1098746693152931901)](https://discord.gg/fweVnRx6CU) [!
   [open in colab](https://colab.research.google.com/assets/colab-badge.svg)]
    (https://colab.research.google.com/drive/1t-9vNLkyoyySAG_0w3eR98biBOXlMO-
                                 E?usp=sharing)
-## â¡ Quick Install `pip install refuel-autolabel` ## ð· What is Autolabel
+## â¡ Quick Install `pip install refuel-autolabel` ## ð Documentation
+[https://docs.refuel.ai/](https://docs.refuel.ai/) ## ð· What is Autolabel
 Access to [large, clean and diverse](https://twitter.com/karpathy/status/
 1528443124577513472?lang=en) labeled datasets is a critical component for any
 machine learning effort to be successful. State-of-the-art LLMs like GPT-4 are
 able to [automatically label data](https://arxiv.org/abs/2303.15056) with [high
 accuracy](https://arxiv.org/abs/2303.16854), and at a fraction of the cost and
 time compared to manual labeling. Autolabel is a Python library to label, clean
 and enrich text datasets with any Large Language Models (LLM) of your choice.
@@ -102,28 +103,19 @@
 calibrate a confidence threshold for your labeling task, and then route less
 confident labels to humans, while you still get the benefits of auto-labeling
 for the confident examples. In order to use Refuel hosted LLMs, you can
 [request access here](https://refuel-ai.typeform.com/llm-access). ## Benchmark
 Check out our [technical report](https://www.refuel.ai/blog-posts/llm-labeling-
 technical-report) to learn more about the performance of various LLMs, and
 human annoators, on label quality, turnaround time and cost. ## ð ï¸ Roadmap
-Our goal is to allow users to label, create or enrich any dataset, with any LLM
-- easily and quickly. There are four focus areas for Autolabel for 2023: *
-**Tasks**: Add support for tasks such as retrieval, attribute enrichment and
-text generation/writing. * **LLMs**: Add support for more LLMs, especially open
-source models like Falcon, MPT and Dolly and the ability to plug in your own
-LLMs. * Workflows for **experimenting with your datasets** more easily: Add
-support for richer data types (such as PDFs and HTML documents) and the ability
-to run benchmarking on your data sources. * Techniques to **improve labeling
-accuracy**: Add support for automatic prompt improvement and tools for better
-error analysis to iteratively improve LLM performance on different tasks We
-will be releasing a more detailed roadmap soon, but we love suggestions and
-contributions from the community. Chat with the Refuel team and Autolabel
-community on [Discord](https://discord.gg/fweVnRx6CU) or open [Github issues]
-(https://github.com/refuel-ai/autolabel/issues) to report bugs and request
-features. ## ð Contributing Autolabel is a rapidly developing project. We
-welcome contributions in all forms - bug reports, pull requests and ideas for
-improving the library. 1. Join the conversation on [Discord](https://
+Check out our [public roadmap](https://github.com/orgs/refuel-ai/projects/15)
+to learn more about ongoing and planned improvements to the Autolabel library.
+We are always looking for suggestions and contributions from the community.
+Join the discussion on [Discord](https://discord.gg/fweVnRx6CU) or open a
+[Github issue](https://github.com/refuel-ai/autolabel/issues) to report bugs
+and request features. ## ð Contributing Autolabel is a rapidly developing
+project. We welcome contributions in all forms - bug reports, pull requests and
+ideas for improving the library. 1. Join the conversation on [Discord](https://
 discord.gg/fweVnRx6CU) 2. Open an [issue](https://github.com/refuel-ai/
 autolabel/issues) on Github for bugs and request features. 3. Grab an open
 issue, and submit a [pull request](https://github.com/refuel-ai/autolabel/blob/
 main/CONTRIBUTING.md).
```

### Comparing `refuel-autolabel-0.0.5/src/refuel_autolabel.egg-info/SOURCES.txt` & `refuel-autolabel-0.0.6/src/refuel_autolabel.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/autolabel/utils.py
 src/autolabel/cache/__init__.py
 src/autolabel/cache/base.py
 src/autolabel/cache/sqlalchemy_cache.py
 src/autolabel/configs/__init__.py
 src/autolabel/configs/base.py
 src/autolabel/configs/config.py
+src/autolabel/configs/schema.py
 src/autolabel/data_models/__init__.py
 src/autolabel/data_models/annotation.py
 src/autolabel/data_models/base.py
 src/autolabel/data_models/cache.py
 src/autolabel/data_models/dataset.py
 src/autolabel/data_models/task.py
 src/autolabel/data_models/task_run.py
@@ -33,14 +34,15 @@
 src/autolabel/models/openai.py
 src/autolabel/models/palm.py
 src/autolabel/models/refuel.py
 src/autolabel/tasks/__init__.py
 src/autolabel/tasks/base.py
 src/autolabel/tasks/classification.py
 src/autolabel/tasks/entity_matching.py
+src/autolabel/tasks/multilabel_classification.py
 src/autolabel/tasks/named_entity_recognition.py
 src/autolabel/tasks/question_answering.py
 src/autolabel/tasks/utils.py
 src/refuel_autolabel.egg-info/PKG-INFO
 src/refuel_autolabel.egg-info/SOURCES.txt
 src/refuel_autolabel.egg-info/dependency_links.txt
 src/refuel_autolabel.egg-info/requires.txt
```

### Comparing `refuel-autolabel-0.0.5/src/refuel_autolabel.egg-info/requires.txt` & `refuel-autolabel-0.0.6/src/refuel_autolabel.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -11,30 +11,33 @@
 regex>=2023.6.3
 rich>=13.3.5
 scipy>=1.10.1
 pydantic>=1.10.9
 torch>=1.10.0
 matplotlib>=3.5.0
 wget>=3.2
+ipywidgets==8.0.6
+jsonschema>=4.17.3
 
 [all]
 black
 bumpver
 pip-tools
 pytest
 pytest-mock
 pre-commit
 openai>=0.27.4
 tiktoken>=0.3.3
-anthropic>=0.2.6
+anthropic==0.2.6
 transformers>=4.25.0
 google-cloud-aiplatform>=1.25.0
+sentence_transformers
 
 [anthropic]
-anthropic>=0.2.6
+anthropic==0.2.6
 
 [dev]
 black
 bumpver
 mkdocs
 mkdocs-autorefs
 mkdocs-jupyter
@@ -49,11 +52,12 @@
 pre-commit
 
 [google]
 google-cloud-aiplatform>=1.25.0
 
 [huggingface]
 transformers>=4.25.0
+sentence_transformers
 
 [openai]
 openai>=0.27.4
 tiktoken>=0.3.3
```

