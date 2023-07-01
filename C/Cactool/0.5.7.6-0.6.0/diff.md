# Comparing `tmp/Cactool-0.5.7.6.tar.gz` & `tmp/Cactool-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Cactool-0.5.7.6.tar", last modified: Mon Apr  4 21:32:18 2022, max compression
+gzip compressed data, was "Cactool-0.6.0.tar", last modified: Sat Jul  1 00:15:11 2023, max compression
```

## Comparing `Cactool-0.5.7.6.tar` & `Cactool-0.6.0.tar`

### file list

```diff
@@ -1,72 +1,137 @@
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2022-04-04 21:32:18.480841 Cactool-0.5.7.6/
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2022-04-04 21:32:18.474174 Cactool-0.5.7.6/Cactool.egg-info/
--rw-r--r--   0 sam       (1000) sam       (1000)     4481 2022-04-04 21:32:18.000000 Cactool-0.5.7.6/Cactool.egg-info/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)     1700 2022-04-04 21:32:18.000000 Cactool-0.5.7.6/Cactool.egg-info/SOURCES.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        1 2022-04-04 21:32:18.000000 Cactool-0.5.7.6/Cactool.egg-info/dependency_links.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       44 2022-04-04 21:32:18.000000 Cactool-0.5.7.6/Cactool.egg-info/entry_points.txt
--rw-r--r--   0 sam       (1000) sam       (1000)      114 2022-04-04 21:32:18.000000 Cactool-0.5.7.6/Cactool.egg-info/requires.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        8 2022-04-04 21:32:18.000000 Cactool-0.5.7.6/Cactool.egg-info/top_level.txt
--rw-r--r--   0 sam       (1000) sam       (1000)     1093 2022-01-13 19:23:36.000000 Cactool-0.5.7.6/LICENSE
--rw-r--r--   0 sam       (1000) sam       (1000)     4481 2022-04-04 21:32:18.480841 Cactool-0.5.7.6/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)     3896 2022-04-04 21:31:56.000000 Cactool-0.5.7.6/README.md
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2022-04-04 21:32:18.474174 Cactool-0.5.7.6/cactool/
--rw-r--r--   0 sam       (1000) sam       (1000)     4598 2022-04-04 05:23:52.000000 Cactool-0.5.7.6/cactool/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)       89 2022-04-04 05:16:56.000000 Cactool-0.5.7.6/cactool/__main__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7999 2022-04-04 21:28:48.000000 Cactool-0.5.7.6/cactool/database.py
--rw-r--r--   0 sam       (1000) sam       (1000)      101 2022-02-12 20:05:29.000000 Cactool-0.5.7.6/cactool/dates.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2022-04-04 21:32:18.474174 Cactool-0.5.7.6/cactool/defaults/
--rw-r--r--   0 sam       (1000) sam       (1000)      111 2022-03-31 02:02:28.000000 Cactool-0.5.7.6/cactool/defaults/config.json
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2022-04-04 21:32:18.477508 Cactool-0.5.7.6/cactool/migrations/
--rw-r--r--   0 sam       (1000) sam       (1000)       41 2022-02-27 15:56:50.000000 Cactool-0.5.7.6/cactool/migrations/README
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2022-04-04 21:32:18.477508 Cactool-0.5.7.6/cactool/migrations/__pycache__/
--rw-r--r--   0 sam       (1000) sam       (1000)     2254 2022-02-27 16:24:04.000000 Cactool-0.5.7.6/cactool/migrations/__pycache__/env.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)      857 2022-02-27 15:56:50.000000 Cactool-0.5.7.6/cactool/migrations/alembic.ini
--rw-r--r--   0 sam       (1000) sam       (1000)     2767 2022-02-27 15:56:50.000000 Cactool-0.5.7.6/cactool/migrations/env.py
--rw-r--r--   0 sam       (1000) sam       (1000)      494 2022-02-27 15:56:50.000000 Cactool-0.5.7.6/cactool/migrations/script.py.mako
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2022-04-04 21:32:18.477508 Cactool-0.5.7.6/cactool/migrations/versions/
--rw-r--r--   0 sam       (1000) sam       (1000)      907 2022-02-27 16:35:30.000000 Cactool-0.5.7.6/cactool/migrations/versions/7226d855d8ec_add_more_ordinal_data_types.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5025 2022-02-27 15:56:53.000000 Cactool-0.5.7.6/cactool/migrations/versions/d1b66364eeb3_initial_migration.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2022-04-04 21:32:18.477508 Cactool-0.5.7.6/cactool/scripts/
--rwxr-xr-x   0 sam       (1000) sam       (1000)       50 2022-03-09 00:03:52.000000 Cactool-0.5.7.6/cactool/scripts/debug.sh
--rwxr-xr-x   0 sam       (1000) sam       (1000)       92 2022-02-12 20:18:15.000000 Cactool-0.5.7.6/cactool/scripts/delete-database.sh
--rw-r--r--   0 sam       (1000) sam       (1000)      209 2022-03-10 01:16:43.000000 Cactool-0.5.7.6/cactool/scripts/get-port.py
--rwxr-xr-x   0 sam       (1000) sam       (1000)      323 2022-03-07 04:34:30.000000 Cactool-0.5.7.6/cactool/scripts/update.sh
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2022-04-04 21:32:18.474174 Cactool-0.5.7.6/cactool/static/
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2022-04-04 21:32:18.477508 Cactool-0.5.7.6/cactool/static/assets/
--rw-r--r--   0 sam       (1000) sam       (1000)    96984 2022-01-22 19:00:56.000000 Cactool-0.5.7.6/cactool/static/assets/cactool-large.png
--rw-r--r--   0 sam       (1000) sam       (1000)    15406 2022-01-24 00:38:04.000000 Cactool-0.5.7.6/cactool/static/assets/favicon.ico
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2022-04-04 21:32:18.477508 Cactool-0.5.7.6/cactool/static/bin/
--rw-r--r--   0 sam       (1000) sam       (1000)    46730 2022-02-22 22:12:25.000000 Cactool-0.5.7.6/cactool/static/bin/tiktok_embed.js
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2022-04-04 21:32:18.480841 Cactool-0.5.7.6/cactool/static/css/
--rw-r--r--   0 sam       (1000) sam       (1000)      184 2022-03-08 20:13:14.000000 Cactool-0.5.7.6/cactool/static/css/cactool.css
--rw-r--r--   0 sam       (1000) sam       (1000)   206899 2021-10-18 22:57:34.000000 Cactool-0.5.7.6/cactool/static/css/styles.css
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2022-04-04 21:32:18.480841 Cactool-0.5.7.6/cactool/static/js/
--rw-r--r--   0 sam       (1000) sam       (1000)     9760 2022-03-14 17:10:39.000000 Cactool-0.5.7.6/cactool/static/js/code.js
--rw-r--r--   0 sam       (1000) sam       (1000)      428 2022-01-23 17:31:12.000000 Cactool-0.5.7.6/cactool/static/js/twitter.js
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2022-04-04 21:32:18.480841 Cactool-0.5.7.6/cactool/templates/
--rw-r--r--   0 sam       (1000) sam       (1000)     3296 2022-01-24 00:48:56.000000 Cactool-0.5.7.6/cactool/templates/add_dataset.html
--rw-r--r--   0 sam       (1000) sam       (1000)      445 2022-01-24 19:29:20.000000 Cactool-0.5.7.6/cactool/templates/card.html
--rw-r--r--   0 sam       (1000) sam       (1000)     2960 2022-03-14 17:04:07.000000 Cactool-0.5.7.6/cactool/templates/code_dataset.html
--rw-r--r--   0 sam       (1000) sam       (1000)     2527 2022-01-25 21:17:29.000000 Cactool-0.5.7.6/cactool/templates/create_project.html
--rw-r--r--   0 sam       (1000) sam       (1000)     2940 2022-03-10 08:33:18.000000 Cactool-0.5.7.6/cactool/templates/dashboard.html
--rw-r--r--   0 sam       (1000) sam       (1000)     1761 2022-04-04 21:15:31.000000 Cactool-0.5.7.6/cactool/templates/delete_dataset.html
--rw-r--r--   0 sam       (1000) sam       (1000)     1697 2022-02-10 11:21:44.000000 Cactool-0.5.7.6/cactool/templates/delete_project.html
--rw-r--r--   0 sam       (1000) sam       (1000)      615 2022-01-15 16:58:57.000000 Cactool-0.5.7.6/cactool/templates/flash.html
--rw-r--r--   0 sam       (1000) sam       (1000)     1998 2022-02-12 14:20:07.000000 Cactool-0.5.7.6/cactool/templates/import_dataset.html
--rw-r--r--   0 sam       (1000) sam       (1000)     2569 2022-02-14 04:17:36.000000 Cactool-0.5.7.6/cactool/templates/index.html
--rw-r--r--   0 sam       (1000) sam       (1000)     2491 2022-01-24 00:51:32.000000 Cactool-0.5.7.6/cactool/templates/login.html
--rw-r--r--   0 sam       (1000) sam       (1000)     1666 2022-03-10 08:33:18.000000 Cactool-0.5.7.6/cactool/templates/macros.html
--rw-r--r--   0 sam       (1000) sam       (1000)     1492 2022-01-25 21:10:17.000000 Cactool-0.5.7.6/cactool/templates/navigation.html
--rw-r--r--   0 sam       (1000) sam       (1000)     1783 2022-02-13 22:01:26.000000 Cactool-0.5.7.6/cactool/templates/show_datasets.html
--rw-r--r--   0 sam       (1000) sam       (1000)     3742 2022-02-27 15:27:57.000000 Cactool-0.5.7.6/cactool/templates/signup.html
--rw-r--r--   0 sam       (1000) sam       (1000)     4951 2022-04-04 21:15:01.000000 Cactool-0.5.7.6/cactool/templates/view_dataset.html
--rw-r--r--   0 sam       (1000) sam       (1000)     2585 2022-02-13 22:01:06.000000 Cactool-0.5.7.6/cactool/templates/view_project.html
--rw-r--r--   0 sam       (1000) sam       (1000)      702 2022-02-27 15:57:01.000000 Cactool-0.5.7.6/cactool/types.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2022-04-04 21:32:18.480841 Cactool-0.5.7.6/cactool/views/
--rw-r--r--   0 sam       (1000) sam       (1000)        0 2022-03-09 00:26:38.000000 Cactool-0.5.7.6/cactool/views/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3040 2022-04-04 05:13:05.000000 Cactool-0.5.7.6/cactool/views/authentication.py
--rw-r--r--   0 sam       (1000) sam       (1000)    11744 2022-04-04 21:23:34.000000 Cactool-0.5.7.6/cactool/views/datasets.py
--rw-r--r--   0 sam       (1000) sam       (1000)      560 2022-02-14 02:06:22.000000 Cactool-0.5.7.6/cactool/views/home.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3181 2022-04-04 05:13:05.000000 Cactool-0.5.7.6/cactool/views/projects.py
--rw-r--r--   0 sam       (1000) sam       (1000)       81 2022-03-08 19:19:39.000000 Cactool-0.5.7.6/pyproject.toml
--rw-r--r--   0 sam       (1000) sam       (1000)      999 2022-04-04 21:32:18.480841 Cactool-0.5.7.6/setup.cfg
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.785363 Cactool-0.6.0/
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.745362 Cactool-0.6.0/Cactool.egg-info/
+-rw-r--r--   0 sam       (1000) sam       (1000)     7367 2023-07-01 00:15:11.000000 Cactool-0.6.0/Cactool.egg-info/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)     6047 2023-07-01 00:15:11.000000 Cactool-0.6.0/Cactool.egg-info/SOURCES.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-07-01 00:15:11.000000 Cactool-0.6.0/Cactool.egg-info/dependency_links.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       44 2023-07-01 00:15:11.000000 Cactool-0.6.0/Cactool.egg-info/entry_points.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)      142 2023-07-01 00:15:11.000000 Cactool-0.6.0/Cactool.egg-info/requires.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        8 2023-07-01 00:15:11.000000 Cactool-0.6.0/Cactool.egg-info/top_level.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)     1093 2022-05-11 16:09:13.000000 Cactool-0.6.0/LICENSE
+-rw-r--r--   0 sam       (1000) sam       (1000)     7367 2023-07-01 00:15:11.785363 Cactool-0.6.0/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)     6821 2023-06-30 00:04:08.000000 Cactool-0.6.0/README.md
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.748696 Cactool-0.6.0/cactool/
+-rw-r--r--   0 sam       (1000) sam       (1000)     4631 2023-06-30 00:04:08.000000 Cactool-0.6.0/cactool/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)       91 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/__main__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    11482 2023-01-13 15:13:46.000000 Cactool-0.6.0/cactool/database.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      102 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/dates.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.748696 Cactool-0.6.0/cactool/defaults/
+-rw-r--r--   0 sam       (1000) sam       (1000)      365 2023-03-01 20:55:20.000000 Cactool-0.6.0/cactool/defaults/config.json
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.752029 Cactool-0.6.0/cactool/migrations/
+-rw-r--r--   0 sam       (1000) sam       (1000)       41 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/migrations/README
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.752029 Cactool-0.6.0/cactool/migrations/__pycache__/
+-rw-r--r--   0 sam       (1000) sam       (1000)     2254 2022-11-13 17:39:31.000000 Cactool-0.6.0/cactool/migrations/__pycache__/env.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     4001 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/__pycache__/env.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      832 2022-11-17 22:51:58.000000 Cactool-0.6.0/cactool/migrations/alembic.ini
+-rw-r--r--   0 sam       (1000) sam       (1000)     2745 2022-11-13 17:39:27.000000 Cactool-0.6.0/cactool/migrations/env.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      494 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/migrations/script.py.mako
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.755362 Cactool-0.6.0/cactool/migrations/versions/
+-rw-r--r--   0 sam       (1000) sam       (1000)      592 2022-11-13 17:39:27.000000 Cactool-0.6.0/cactool/migrations/versions/07c0c9849f18_store_user_otp_secret.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      952 2022-11-17 22:51:58.000000 Cactool-0.6.0/cactool/migrations/versions/07d73859b99c_add_show_data_type.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      822 2022-12-19 20:19:53.000000 Cactool-0.6.0/cactool/migrations/versions/16942fdb0f18_add_relative_column_priorities.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      709 2023-01-13 15:21:55.000000 Cactool-0.6.0/cactool/migrations/versions/19d06323ddd6_store_dataset_access_ranes.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      763 2023-01-12 00:42:42.000000 Cactool-0.6.0/cactool/migrations/versions/28e8811a530d_support_dataset_file_storage.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1269 2023-01-02 05:22:05.000000 Cactool-0.6.0/cactool/migrations/versions/51ed49d3ed75_support_user_email_verification.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      938 2022-12-19 20:19:53.000000 Cactool-0.6.0/cactool/migrations/versions/5e7f3be664d5_rename_priority_column_to_order.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      380 2022-11-17 22:51:58.000000 Cactool-0.6.0/cactool/migrations/versions/6286ef6698f9_merge_heads.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      885 2022-11-13 17:39:27.000000 Cactool-0.6.0/cactool/migrations/versions/7226d855d8ec_add_more_ordinal_data_types.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.768696 Cactool-0.6.0/cactool/migrations/versions/__pycache__/
+-rw-r--r--   0 sam       (1000) sam       (1000)     1064 2022-11-12 14:02:05.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/072331977abf_store_user_emails.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      966 2022-11-13 17:39:31.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/07c0c9849f18_store_user_otp_secret.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1615 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/07c0c9849f18_store_user_otp_secret.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1133 2022-11-17 22:52:32.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/07d73859b99c_add_show_data_type.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1592 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/07d73859b99c_add_show_data_type.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1026 2023-01-10 17:45:24.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/0f3a32ab3b24_support_dataset_files.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      946 2022-12-11 16:39:27.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/16942fdb0f18_.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      993 2023-01-01 23:29:37.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/16942fdb0f18_add_relative_column_priorities.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1644 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/16942fdb0f18_add_relative_column_priorities.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1005 2023-01-13 14:54:14.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/19d06323ddd6_.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1051 2023-01-22 14:51:47.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/19d06323ddd6_store_dataset_access_ranes.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1888 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/19d06323ddd6_store_dataset_access_ranes.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1092 2023-01-10 17:39:40.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/25345a0b177f_make_datasetfile_file_names_part_of_the_.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1032 2023-01-13 14:54:14.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/28e8811a530d_support_dataset_file_storage.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1594 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/28e8811a530d_support_dataset_file_storage.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1299 2023-01-07 09:30:57.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/51ed49d3ed75_support_user_email_verification.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     2396 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/51ed49d3ed75_support_user_email_verification.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      922 2022-11-12 13:57:50.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/5ab489444dcc_store_user_emails.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      986 2023-01-01 23:29:37.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/5e7f3be664d5_rename_priority_column_to_order.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1882 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/5e7f3be664d5_rename_priority_column_to_order.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      686 2022-11-13 17:44:58.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/6286ef6698f9_.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      695 2022-11-17 22:52:32.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/6286ef6698f9_merge_heads.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      790 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/6286ef6698f9_merge_heads.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1124 2022-11-13 17:39:31.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/7226d855d8ec_add_more_ordinal_data_types.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1579 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/7226d855d8ec_add_more_ordinal_data_types.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      937 2022-11-12 15:14:52.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/727b95af4b5f_.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1242 2023-01-02 05:07:03.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/c0ed5c0ee030_.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      972 2022-11-13 17:39:31.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/c12d86b089b8_store_user_emails.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1628 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/c12d86b089b8_store_user_emails.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1154 2023-01-10 10:50:03.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/ce5fc447a2e8_add_image_display_type.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1615 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/ce5fc447a2e8_add_image_display_type.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     3000 2022-11-13 17:39:31.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/d1b66364eeb3_initial_migration.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     8379 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/d1b66364eeb3_initial_migration.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      587 2022-11-13 17:39:27.000000 Cactool-0.6.0/cactool/migrations/versions/c12d86b089b8_store_user_emails.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      982 2023-01-07 10:01:34.000000 Cactool-0.6.0/cactool/migrations/versions/ce5fc447a2e8_add_image_display_type.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5807 2022-11-13 17:39:27.000000 Cactool-0.6.0/cactool/migrations/versions/d1b66364eeb3_initial_migration.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.768696 Cactool-0.6.0/cactool/scripts/
+-rwxr-xr-x   0 sam       (1000) sam       (1000)       50 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/scripts/debug.sh
+-rwxr-xr-x   0 sam       (1000) sam       (1000)       92 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/scripts/delete-database.sh
+-rw-r--r--   0 sam       (1000) sam       (1000)      209 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/scripts/get-port.py
+-rwxr-xr-x   0 sam       (1000) sam       (1000)      323 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/scripts/update.sh
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.745362 Cactool-0.6.0/cactool/static/
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.772029 Cactool-0.6.0/cactool/static/assets/
+-rw-r--r--   0 sam       (1000) sam       (1000)   162190 2023-06-30 00:04:08.000000 Cactool-0.6.0/cactool/static/assets/404Error.png
+-rw-r--r--   0 sam       (1000) sam       (1000)   161280 2023-06-30 00:04:08.000000 Cactool-0.6.0/cactool/static/assets/StrangeError.png
+-rw-r--r--   0 sam       (1000) sam       (1000)    96984 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/static/assets/cactool-large.png
+-rw-r--r--   0 sam       (1000) sam       (1000)    15406 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/static/assets/favicon.ico
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.772029 Cactool-0.6.0/cactool/static/bin/
+-rw-r--r--   0 sam       (1000) sam       (1000)    15593 2022-05-14 10:36:35.000000 Cactool-0.6.0/cactool/static/bin/instagram_embed.js
+-rw-r--r--   0 sam       (1000) sam       (1000)    47547 2023-01-07 09:19:40.000000 Cactool-0.6.0/cactool/static/bin/tiktok_embed.js
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.775363 Cactool-0.6.0/cactool/static/css/
+-rw-r--r--   0 sam       (1000) sam       (1000)    95609 2022-11-17 22:51:58.000000 Cactool-0.6.0/cactool/static/css/bootstrap-icons.css
+-rw-r--r--   0 sam       (1000) sam       (1000)   194901 2022-11-17 22:51:58.000000 Cactool-0.6.0/cactool/static/css/bootstrap.css
+-rw-r--r--   0 sam       (1000) sam       (1000)      790 2023-02-28 15:07:32.000000 Cactool-0.6.0/cactool/static/css/cactool.css
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.775363 Cactool-0.6.0/cactool/static/css/fonts/
+-rw-r--r--   0 sam       (1000) sam       (1000)   121296 2022-11-17 22:51:58.000000 Cactool-0.6.0/cactool/static/css/fonts/bootstrap-icons.woff2
+-rw-r--r--   0 sam       (1000) sam       (1000)     1508 2022-12-20 02:32:09.000000 Cactool-0.6.0/cactool/static/css/login.css
+-rw-r--r--   0 sam       (1000) sam       (1000)      130 2022-12-20 02:57:30.000000 Cactool-0.6.0/cactool/static/css/projects.css
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.778696 Cactool-0.6.0/cactool/static/js/
+-rw-r--r--   0 sam       (1000) sam       (1000)    80496 2022-11-17 22:51:58.000000 Cactool-0.6.0/cactool/static/js/bootstrap.js
+-rw-r--r--   0 sam       (1000) sam       (1000)    10545 2023-01-17 13:21:52.000000 Cactool-0.6.0/cactool/static/js/code.js
+-rw-r--r--   0 sam       (1000) sam       (1000)      428 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/static/js/twitter.js
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.785363 Cactool-0.6.0/cactool/templates/
+-rw-r--r--   0 sam       (1000) sam       (1000)      838 2023-06-30 00:04:08.000000 Cactool-0.6.0/cactool/templates/404.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     3113 2022-12-20 03:07:40.000000 Cactool-0.6.0/cactool/templates/add_dataset.html
+-rw-r--r--   0 sam       (1000) sam       (1000)      445 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/templates/card.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     4581 2023-02-28 15:09:22.000000 Cactool-0.6.0/cactool/templates/code_dataset.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     2121 2023-01-02 14:21:53.000000 Cactool-0.6.0/cactool/templates/coding_interface.html
+-rw-r--r--   0 sam       (1000) sam       (1000)        0 2022-12-19 20:19:56.000000 Cactool-0.6.0/cactool/templates/contact.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     1491 2022-12-20 02:57:47.000000 Cactool-0.6.0/cactool/templates/create_project.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     2727 2022-12-20 02:38:15.000000 Cactool-0.6.0/cactool/templates/dashboard.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     1583 2022-12-20 02:42:07.000000 Cactool-0.6.0/cactool/templates/delete_dataset.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     1463 2022-12-20 03:06:04.000000 Cactool-0.6.0/cactool/templates/delete_project.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     1268 2023-06-30 00:04:08.000000 Cactool-0.6.0/cactool/templates/error.html
+-rw-r--r--   0 sam       (1000) sam       (1000)        0 2022-12-19 20:19:56.000000 Cactool-0.6.0/cactool/templates/faq.html
+-rw-r--r--   0 sam       (1000) sam       (1000)      615 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/templates/flash.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     2067 2022-12-20 02:39:33.000000 Cactool-0.6.0/cactool/templates/import_dataset.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     2349 2022-12-20 03:04:09.000000 Cactool-0.6.0/cactool/templates/index.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     6812 2022-05-28 12:15:27.000000 Cactool-0.6.0/cactool/templates/instagram_embed.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     1947 2022-12-19 20:19:56.000000 Cactool-0.6.0/cactool/templates/login.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     1847 2023-01-10 12:22:56.000000 Cactool-0.6.0/cactool/templates/macros.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     2046 2022-12-19 20:19:56.000000 Cactool-0.6.0/cactool/templates/navigation.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     1541 2022-12-20 02:59:07.000000 Cactool-0.6.0/cactool/templates/setup_2fa.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     1634 2022-12-20 03:07:12.000000 Cactool-0.6.0/cactool/templates/show_datasets.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     4580 2022-12-20 02:59:18.000000 Cactool-0.6.0/cactool/templates/signup.html
+-rw-r--r--   0 sam       (1000) sam       (1000)      209 2023-01-07 09:19:00.000000 Cactool-0.6.0/cactool/templates/tiktok_embed.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     1545 2023-01-12 01:15:17.000000 Cactool-0.6.0/cactool/templates/upload_images.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     1488 2022-12-20 03:08:13.000000 Cactool-0.6.0/cactool/templates/verify_2fa.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     6815 2023-02-28 15:19:51.000000 Cactool-0.6.0/cactool/templates/view_dataset.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     2401 2022-12-20 03:07:59.000000 Cactool-0.6.0/cactool/templates/view_project.html
+-rw-r--r--   0 sam       (1000) sam       (1000)      847 2023-01-07 09:58:35.000000 Cactool-0.6.0/cactool/types.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.785363 Cactool-0.6.0/cactool/views/
+-rw-r--r--   0 sam       (1000) sam       (1000)        0 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/views/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     8334 2023-01-22 15:00:13.000000 Cactool-0.6.0/cactool/views/authentication.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    19277 2023-01-22 15:00:13.000000 Cactool-0.6.0/cactool/views/datasets.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      558 2022-05-28 11:37:55.000000 Cactool-0.6.0/cactool/views/home.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3152 2022-05-28 11:37:55.000000 Cactool-0.6.0/cactool/views/projects.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      425 2023-01-22 14:59:50.000000 Cactool-0.6.0/cactool/views/site.py
+-rw-r--r--   0 sam       (1000) sam       (1000)       81 2022-07-06 17:45:09.000000 Cactool-0.6.0/pyproject.toml
+-rw-r--r--   0 sam       (1000) sam       (1000)     1028 2023-07-01 00:15:11.785363 Cactool-0.6.0/setup.cfg
```

### Comparing `Cactool-0.5.7.6/LICENSE` & `Cactool-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Cactool-0.5.7.6/cactool/__init__.py` & `Cactool-0.6.0/cactool/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,153 +1,158 @@
-import sys
+import base64
+import json
 import os
 import os.path
-import subprocess
 import pathlib
-import base64
-import json
 import secrets
+import subprocess
+import sys
 
 import appdirs
-
-from flask import Flask
-from flask_login import LoginManager
-from flask_migrate import Migrate, upgrade
+import waitress
 from cryptography.hazmat.primitives.hashes import SHA256
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
+from flask import Flask, g
+from flask_login import LoginManager
+from flask_migrate import Migrate, upgrade
+from werkzeug.exceptions import HTTPException
 
-from .database import db, AnonymousUser, User
+from .database import AnonymousUser, User, db
 from .views.authentication import authentication
+from .views.datasets import datasets
 from .views.home import home
 from .views.projects import projects
-from .views.datasets import datasets
-
-import waitress
+from .views.site import page_not_found, server_error, site
 
 ROOT = pathlib.Path(__file__).parents[1]
 CONFIG_DIR = appdirs.user_config_dir("cactool")
 MIGRATIONS_DIR = os.path.join(ROOT, "cactool/migrations")
 DEFAULT_CONFIG_FILE_NAME = os.path.join(ROOT, "cactool/defaults/config.json")
 CONFIG_FILE_NAME = os.path.join(CONFIG_DIR, "config.json")
 STARTUP_SCRIPT_LOCATION = os.path.join(ROOT, "cactool/bin/cactool")
 STATIC_FOLDER_PATH = os.path.join(ROOT, "cactool/static")
 DATABASE_FILE_NAME = "db.sqlite3"
 
+
+def get_value(key):
+    return config[key]
+
+
+def write_config(config):
+    with open(CONFIG_FILE_NAME, "w") as file:
+        json.dump(config, file, indent=2, sort_keys=True)
+
+
+def set_value(config, key, value):
+    config[key] = value
+    write_config(config)
+
+
+def unset_value(config, key):
+    del config[key]
+    write_config(config)
+
+
+def upgrade_database():
+    with app.app_context():
+        upgrade(MIGRATIONS_DIR)
+
+
 if not os.path.exists(CONFIG_DIR):
     os.makedirs(CONFIG_DIR)
 
+with open(DEFAULT_CONFIG_FILE_NAME) as file:
+    default_config = json.load(file)
+
 if not os.path.exists(CONFIG_FILE_NAME):
     secret_key = secrets.token_urlsafe(64)
-    with open(DEFAULT_CONFIG_FILE_NAME) as file:
-        config = json.load(file)
-        config["secret-key"] = secret_key
-    with open(CONFIG_FILE_NAME, "w") as file:
-        json.dump(config, file, indent=2, sort_keys=True)
-else:
-    with open(CONFIG_FILE_NAME) as file:
-        config = json.load(file)
-
-if not "upload-limit" in config:
-    config["upload-limit"] = 1024
-if not "max-rows" in config:
-    config["max-rows"] = -1
-if not "signup-code" in config or config["signup-code"] == "":
-    config["signup-code"] = None
+    config = default_config.copy()
+    config["secret-key"] = secret_key
+    write_config(config)
+
+with open(CONFIG_FILE_NAME) as file:
+    config = json.load(file)
+
+config = {**default_config, **config}
+write_config(config)
 
 app = Flask(__name__, static_folder=STATIC_FOLDER_PATH)
 
 app.register_blueprint(home)
 app.register_blueprint(authentication)
 app.register_blueprint(projects)
 app.register_blueprint(datasets)
+app.register_blueprint(site)
+app.register_error_handler(404, page_not_found)
+app.register_error_handler(500, server_error)
+
+
+@app.errorhandler(Exception)
+def handle_exception(exception):
+    if isinstance(exception, HTTPException):
+        return exception
+
+    return server_error(exception)
+
 
 if not os.path.isdir(app.instance_path):
     try:
         os.makedirs(app.instance_path)
     except FileExistsError:
         pass
 
 DATABASE_LOCATION = os.path.join(app.instance_path, DATABASE_FILE_NAME)
 DATABASE_URI = "sqlite:///" + DATABASE_LOCATION
 
 app.config["SQLALCHEMY_DATABASE_URI"] = DATABASE_URI
 app.config["DATABASE_LOCATION"] = DATABASE_LOCATION
 app.config["SQLALCHEMY_TRACK_MODIFICATIONS"] = False
-app.config["MAX_CONTENT_LENGTH"] = int(config["upload-limit"]) * 1024**2
-app.config["max_rows_in_memory"] = int(config["max-rows"])
-app.config["signup-code"] = config["signup-code"]
+app.config["MAX_CONTENT_LENGTH"] = config["upload-limit"] * 1024**2
+
+app.config.update(config)
+
 app.secret_key = config["secret-key"]
 
-kdf = PBKDF2HMAC(
-    algorithm=SHA256,
-    length=32,
-    salt=b"",
-    iterations=390000
-)
+kdf = PBKDF2HMAC(algorithm=SHA256(), length=32, salt=os.urandom(32), iterations=390000)
 
 app.encryption_key = base64.urlsafe_b64encode(kdf.derive(app.secret_key.encode()))
 
 login_manager = LoginManager()
 login_manager.anonymous_user = AnonymousUser
 login_manager.login_view = "authentication.login"
 login_manager.init_app(app)
 
 db.init_app(app)
-migrate = Migrate(app, db, compare_type=True)
+migrate = Migrate(app, db, compare_type=True, render_as_batch=True)
+
 
 @login_manager.user_loader
 def load_user(user_id):
     return User.query.get(user_id)
 
-def get_value(key):
-    if key == "port":
-        if "port" in config:
-            return config["port"]
-        else:
-            return 8080
-    else:
-        return config[key]
-
-def write_config():
-    with open(CONFIG_FILE_NAME, "w") as file:
-        json.dump(config, file)
-
-def set_value(key, value):
-    config[key] = value
-    write_config()
-
-def unset_value(key):
-    del config[key]
-    write_config()
-
-def upgrade_database():
-    with app.app_context():
-        upgrade(MIGRATIONS_DIR)
 
 USAGE_STRING = """\
 usage: cactool COMMAND [ARGS...]
 Commands:
   cactool                   Starts the server
   cactool get NAME          Gets a configuration parameter
   cactool unset NAME        Unsets a configuration parameter
   cactool set NAME VALUE    Sets a configuration parameter\
 """
 
+
 def cactool():
     if len(sys.argv) == 1:
         upgrade_database()
-        bind = f"localhost:{get_value('port')}"
+        bind = f"0.0.0.0:{get_value('port')}"
         print(f"Starting Cactool server instance at http://{bind}")
-        waitress.serve(
-            app,
-            listen = bind
-        ) # Start application
+        waitress.serve(app, listen=bind)  # Start application
     elif len(sys.argv) == 2 and sys.argv[1] == "update":
-        upgrade_database() # Upgrade the database
+        upgrade_database()  # Upgrade the database
     elif len(sys.argv) == 3 and sys.argv[1] == "get":
-        print(get_value(sys.argv[2])) # Get a configuration parameter
+        print(get_value(config, sys.argv[2]))  # Get a configuration parameter
     elif len(sys.argv) == 3 and sys.argv[1] == "unset":
-        unset_value(sys.argv[2]) # Unsets a configuration parameter
+        unset_value(config, sys.argv[2])  # Unsets a configuration parameter
     elif len(sys.argv) == 4 and sys.argv[1] == "set":
-        set_value(sys.argv[2], sys.argv[3]) # Sets a configuration parameter
+        set_value(config, sys.argv[2], sys.argv[3])  # Sets a configuration parameter
     else:
         print(USAGE_STRING)
```

### Comparing `Cactool-0.5.7.6/cactool/database.py` & `Cactool-0.6.0/cactool/database.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,96 @@
-from flask_sqlalchemy import SQLAlchemy
-from flask_login import UserMixin, AnonymousUserMixin
+import base64
 import csv
-from .types import Type, AccessLevel
+import operator
+import os
+import secrets
+
 import cryptography.fernet
- 
+from flask_login import AnonymousUserMixin, UserMixin
+from flask_sqlalchemy import SQLAlchemy
+
+from .types import AccessLevel, Type
+
 db = SQLAlchemy()
 
 
 class AccessContainer:
     def grants(self, access_type, thing=False):
-        return (not thing or self.container_id == thing.id) and access_type <= self.access_level
+        return (
+            not thing or self.container_id == thing.id
+        ) and access_type <= self.access_level
 
     def grant_condition(self, access_type):
         def condition(thing):
             return self.grants(access_type, thing)
+
         return condition
-    
+
     @property
     def access_level(self):
         raise NotImplementedError()
 
     @property
     def container_id(self):
         raise NotImplementedError()
 
+
+class UserEmailVerification(db.Model):
+    verification_code = db.Column(db.String(16), primary_key=True)
+    user_id = db.Column(db.ForeignKey("user.id"))
+    timestamp = db.Column(db.Integer())
+
+    user = db.relationship("User")
+
+
 class DatasetAccess(db.Model, AccessContainer):
     user_id = db.Column(db.ForeignKey("user.id"), primary_key=True)
     dataset_id = db.Column(db.ForeignKey("dataset.id"), primary_key=True)
     access_level = db.Column(db.Enum(AccessLevel))
-    
+
+    start_index = db.Column(db.Integer, default=None)
+    end_index = db.Column(db.Integer, default=None)
+
+    user = db.relationship("User")
+    dataset = db.relationship("Dataset")
+
     @property
     def container_id(self):
         return self.dataset_id
 
+    @property
+    def start(self):
+        if self.start_index:
+            return self.start_index
+        return 0
+
+    @property
+    def end(self):
+        if self.end_index:
+            return self.end_index
+        return self.dataset.num_rows - 1
+
+
 class ProjectAccess(db.Model, AccessContainer):
     user_id = db.Column(db.ForeignKey("user.id"), primary_key=True)
     project_id = db.Column(db.ForeignKey("project.id"), primary_key=True)
     access_level = db.Column(db.Enum(AccessLevel))
-    
+
     @property
     def container_id(self):
         return self.project_id
-    
+
+
 project_datasets = db.Table(
     "project_datasets",
     db.Column("project_id", db.ForeignKey("project.id")),
-    db.Column("dataset_id", db.ForeignKey("dataset.id"))
+    db.Column("dataset_id", db.ForeignKey("dataset.id")),
 )
 
+
 class AnonymousUser(AnonymousUserMixin):
     def viewable_datasets(self):
         return []
 
     def editable_projects(self):
         return []
 
@@ -69,100 +108,126 @@
 
     def can_code(self, thing):
         return False
 
     def can_export(self, thing):
         return False
 
+    @property
     def initials(self):
         return "??"
 
+
 class User(UserMixin, db.Model):
     id = db.Column(db.String(512), unique=True, primary_key=True)
     admin = db.Column(db.Boolean)
     username = db.Column(db.String(20), unique=True)
+    otp_secret = db.Column(db.String())
+    email = db.Column(db.String(50))
     password = db.Column(db.String(1024))
     firstname = db.Column(db.String(50))
     surname = db.Column(db.String(50))
+    unverified = db.Column(db.Boolean(), default=False)
 
     dataset_rights = db.relationship(DatasetAccess)
     project_rights = db.relationship(ProjectAccess)
-    
+    email_verification = db.relationship(UserEmailVerification)
 
     def viewable_datasets(self):
         datasets = []
         for access in self.dataset_rights:
             if access.grants(AccessLevel.CODE):
                 datasets.append(access.dataset)
-        
+
         return datasets
-    
+
     def editable_projects(self):
         projects = []
         for access in self.project_rights:
             project = Project.query.get(access.project_id)
             if project and self.can_edit(project):
                 projects.append(project)
 
-        return projects      
-    
+        return projects
+
     def can(self, access_type, thing):
         if isinstance(thing, Dataset):
             return self.can_dataset(thing, access_type)
- 
+
         if isinstance(thing, Project):
             return self.can_project(thing, access_type)
-        
+
         raise TypeError("User.can expects an instance of Project or Dataset")
 
     def can_dataset(self, dataset, access_type):
         rights = DatasetAccess.query.get((self.id, dataset.id))
         return rights and rights.grants(access_type, dataset)
-    
+
     def can_project(self, project, access_type):
         rights = ProjectAccess.query.get((self.id, project.id))
         return rights and rights.grants(access_type, project)
 
     def can_edit(self, thing):
-       return self.can(
-           AccessLevel.ADMIN,
-           thing 
-       )
+        return self.can(AccessLevel.ADMIN, thing)
 
     def can_export(self, thing):
-        return self.can(
-            AccessLevel.EXPORT,
-            thing 
-        )
-        
-    def can_code(self, thing):
-        return self.can(
-            AccessLevel.CODE,
-            thing
-        )
+        return self.can(AccessLevel.EXPORT, thing)
 
+    def can_code(self, thing):
+        return self.can(AccessLevel.CODE, thing)
 
     def get_id(self):
         return self.id
-    
+
+    @property
     def initials(self):
         return self.firstname[0].upper() + self.surname[0].upper()
-    
+
+    def regenerate_otp_secret(self):
+        self.otp_secret = User.random_otp_secret()
+
+    @staticmethod
+    def random_otp_secret():
+        byte_sequence = secrets.token_bytes(40)
+        return base64.b32encode(byte_sequence).decode()
+
+    @staticmethod
+    def otp_secret_to_url(secret, username=None):
+        if username:
+            return f"otpauth://totp/Cactool:{username}?secret={secret}&issuer=Cactool"
+        return f"otpauth://totp/Cactool?secret={secret}"
+
+    @property
+    def has_2fa(self):
+        return self.otp_secret is not None
+
+    def disable_2fa(self):
+        self.otp_secret = None
+
+    @property
+    def otp_secret_url(self):
+        if not self.otp_secret:
+            return None
+        return User.otp_secret_to_url(self.otp_secret, username=self.username)
+
+
 class Dataset(db.Model):
     id = db.Column(db.String(512), unique=True, primary_key=True)
     name = db.Column(db.String(50))
     description = db.Column(db.String(1024))
-    
+
     columns = db.relationship("DatasetColumn", cascade="all, delete-orphan")
     rows = db.relationship("DatasetRow", cascade="all, delete-orphan")
 
     projects = db.relationship("Project", secondary=project_datasets)
 
     granted_access = db.relationship("DatasetAccess", cascade="all, delete-orphan")
-    
+
+    files = db.relationship("DatasetFile", cascade="all, delete-orphan")
+
     def emit_csv(self) -> str:
         writer = csv.DictWriter()
         pass
 
     def confirm(self, code, ekey):
         fernet = cryptography.fernet.Fernet(ekey)
         return fernet.decrypt(code) == self.id.encode()
@@ -172,99 +237,153 @@
         return fernet.encrypt(self.id.encode()).hex()
 
     def generate_invite_link(self, base_url, ekey):
         return base_url + f"dataset/invite/{self.id}/{self.code(ekey)}"
 
     @property
     def num_rows(self):
+        return DatasetRow.query.filter_by(dataset_id=self.id).count()
+
+    @property
+    def num_coded(self):
         return DatasetRow.query.filter_by(
-            dataset_id=self.id
+            dataset_id=self.id, coded=True, skip=False
         ).count()
-    
+
+    @property
+    def num_skipped(self):
+        return DatasetRow.query.filter_by(dataset_id=self.id, skip=True).count()
+
+    @property
+    def num_unavailable(self):
+        return DatasetRow.query.filter_by(
+            dataset_id=self.id, post_unavailable=True
+        ).count()
+
+    @property
+    def code_status_description(self):
+        messages = [f"{self.num_coded} coded"]
+
+        num_skipped = self.num_skipped
+        num_unavailable = self.num_unavailable
+        if num_skipped:
+            messages.append(f"{num_skipped} skipped")
+        if num_unavailable:
+            messages.append(f"{num_unavailable} unavailable")
+
+        return ", ".join(messages)
+
+    @property
+    def has_social_media(self):
+        return any(
+            column.type in [Type.SOCIAL_MEDIA, Type.IMAGE] for column in self.columns
+        )
+
     @property
     def ordered_columns(self):
-        return sorted(self.columns, key=lambda column: column.type != Type.SOCIAL_MEDIA)
+        return sorted(self.columns, key=lambda column: column.order or 999)
+
+    @property
+    def coder_access(self):
+        result = []
+        for access in self.granted_access:
+            if access.grants(AccessLevel.CODE):
+                result.append(access)
+        return result
+
+    @property
+    def coders(self):
+        coders = []
+        for access in self.coder_access:
+            coders.append(access.user)
+        return coders
 
 
 class DatasetColumn(db.Model):
     id = db.Column(db.String(512), primary_key=True, unique=True)
     name = db.Column(db.String(50))
     type = db.Column(db.Enum(Type))
     dataset_id = db.Column(db.ForeignKey(Dataset.id))
     prompt = db.Column(db.String(512))
+    order = db.Column(db.Integer, default=999)
 
     dataset = db.relationship(Dataset, foreign_keys="DatasetColumn.dataset_id")
-    
-    
-    __table_args__ = (
-        db.UniqueConstraint(dataset_id, name),
-    )
 
-class DatasetRow(db.Model):   
+    __table_args__ = (db.UniqueConstraint(dataset_id, name),)
+
+
+class DatasetRow(db.Model):
     dataset_id = db.Column(db.String(512), db.ForeignKey(Dataset.id), primary_key=True)
     row_number = db.Column(db.Integer, primary_key=True)
 
-    coded = db.Column(db.Boolean())
+    coded = db.Column(db.Boolean(), default=False)
     coder_id = db.Column(db.ForeignKey(User.id), nullable=True)
-    
-    skip = db.Column(db.Boolean())
-    post_unavailable = db.Column(db.Boolean())
+
+    skip = db.Column(db.Boolean(), default=False)
+    post_unavailable = db.Column(db.Boolean(), default=False)
 
     values = db.relationship("DatasetRowValue", lazy=True, cascade="all, delete-orphan")
     dataset = db.relationship(Dataset, foreign_keys="DatasetRow.dataset_id")
-    
+
     coder = db.relationship("User", foreign_keys="DatasetRow.coder_id")
-    
-    __table_args__ = (
-        db.UniqueConstraint(dataset_id, row_number),
-    )
-    
+
+    __table_args__ = (db.UniqueConstraint(dataset_id, row_number),)
+
     def serialise(self):
         return {
             "is_empty": False,
             "dataset_id": self.dataset_id,
             "row_number": self.row_number,
             "columns": {
                 entry.column.id: {
-                     "name": entry.column.name,
-                     "prompt": entry.column.prompt,
-                     "value": entry.value,
-                     "type": entry.column.type.serialise()
-                }   for entry in self.values
-            }
+                    "name": entry.column.name,
+                    "prompt": entry.column.prompt,
+                    "value": entry.value,
+                    "type": entry.column.type.serialise(),
+                }
+                for entry in sorted(
+                    self.values, key=lambda value: value.column.order or 0
+                )
+            },
         }
-    
+
     @staticmethod
     def empty(dataset_id, row_number):
-        return {
-            {
-                
-            }
-        }
+        return {{}}
 
 
 class DatasetRowValue(db.Model):
     dataset_id = db.Column(db.String(512), primary_key=True)
     dataset_row_number = db.Column(db.Integer, primary_key=True)
     column_id = db.Column(db.ForeignKey(DatasetColumn.id), primary_key=True)
 
     value = db.Column(db.String(65535))
-    
+
     column = db.relationship("DatasetColumn")
-    
+
     __table_args__ = (
         db.ForeignKeyConstraint(
             [dataset_id, dataset_row_number],
-            [DatasetRow.dataset_id, DatasetRow.row_number]
+            [DatasetRow.dataset_id, DatasetRow.row_number],
         ),
-        db.UniqueConstraint(
-            dataset_id, dataset_row_number, column_id
-        )
+        db.UniqueConstraint(dataset_id, dataset_row_number, column_id),
     )
-    
+
+
+class DatasetFile(db.Model):
+    dataset_id = db.Column(db.ForeignKey(Dataset.id), primary_key=True)
+    file_name = db.Column(db.String(255), primary_key=True)
+    mime_type = db.Column(db.String(32))
+
+    def content(self, instance_directory):
+        location = os.path.join(instance_directory, self.dataset_id, self.file_name)
+        with open(location, "rb") as file:
+            content = file.read()
+        return content
+
 
 class Project(db.Model):
     id = db.Column(db.String(512), primary_key=True, unique=True)
     name = db.Column(db.String(50))
     description = db.Column(db.String(1024))
 
     datasets = db.relationship("Dataset", secondary=project_datasets)
```

### Comparing `Cactool-0.5.7.6/cactool/migrations/__pycache__/env.cpython-310.pyc` & `Cactool-0.6.0/cactool/migrations/__pycache__/env.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Feb 27 15:56:50 2022 UTC, .py size: 2767 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-00000000: 6f0d 0d0a 0000 0000 429f 1b62 cf0a 0000  o.......B..b....
+00000000: 6f0d 0d0a 0000 0000 cf2b 7163 b90a 0000  o........+qc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 b200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
-00000060: 6d08 5a08 0100 6508 6a09 5a09 6504 6509  m.Z...e.j.Z.e.e.
+00000060: 6d08 5a08 0100 6506 6a09 5a09 6504 6509  m.Z...e.j.Z.e.e.
 00000070: 6a0a 8301 0100 6502 a00b 6406 a101 5a0c  j.....e...d...Z.
-00000080: 6509 a00d 6407 650e 6506 6a0f 6408 1900  e...d.e.e.j.d...
+00000080: 6509 a00d 6407 650e 6508 6a0f 6408 1900  e...d.e.e.j.d...
 00000090: 6a10 a011 a100 6a12 8301 a013 6409 640a  j.....j.....d.d.
-000000a0: a102 a102 0100 6506 6a0f 6408 1900 6a10  ......e.j.d...j.
+000000a0: a102 a102 0100 6508 6a0f 6408 1900 6a10  ......e.j.d...j.
 000000b0: 6a14 5a15 640b 640c 8400 5a16 640d 640e  j.Z.d.d...Z.d.d.
-000000c0: 8400 5a17 6508 a018 a100 7254 6516 8300  ..Z.e.....rTe...
+000000c0: 8400 5a17 6506 a018 a100 7254 6516 8300  ..Z.e.....rTe...
 000000d0: 0100 6402 5300 6517 8300 0100 6402 5300  ..d.S.e.....d.S.
 000000e0: 290f e900 0000 0029 01da 0e77 6974 685f  )......)...with_
 000000f0: 7374 6174 656d 656e 744e 2901 da0a 6669  statementN)...fi
-00000100: 6c65 436f 6e66 6967 2901 da0b 6375 7272  leConfig)...curr
-00000110: 656e 745f 6170 7029 01da 0763 6f6e 7465  ent_app)...conte
-00000120: 7874 7a0b 616c 656d 6269 632e 656e 76fa  xtz.alembic.env.
+00000100: 6c65 436f 6e66 6967 2901 da07 636f 6e74  leConfig)...cont
+00000110: 6578 7429 01da 0b63 7572 7265 6e74 5f61  ext)...current_a
+00000120: 7070 7a0b 616c 656d 6269 632e 656e 76fa  ppz.alembic.env.
 00000130: 0e73 716c 616c 6368 656d 792e 7572 6cda  .sqlalchemy.url.
 00000140: 076d 6967 7261 7465 fa01 257a 0225 2563  .migrate..%z.%%c
 00000150: 0000 0000 0000 0000 0000 0000 0100 0000  ................
 00000160: 0800 0000 4300 0000 7350 0000 0074 00a0  ....C...sP...t..
 00000170: 0164 01a1 017d 0074 026a 037c 0074 0464  .d...}.t.j.|.t.d
 00000180: 0264 038d 0301 0074 02a0 05a1 008f 0d01  .d.....t........
 00000190: 0074 02a0 06a1 0001 0057 0064 0404 0004  .t.......W.d....
@@ -47,95 +47,95 @@
 000002e0: 7665 6e20 7374 7269 6e67 2074 6f20 7468  ven string to th
 000002f0: 650a 2020 2020 7363 7269 7074 206f 7574  e.    script out
 00000300: 7075 742e 0a0a 2020 2020 7206 0000 0054  put...    r....T
 00000310: 2903 da03 7572 6cda 0f74 6172 6765 745f  )...url..target_
 00000320: 6d65 7461 6461 7461 da0d 6c69 7465 7261  metadata..litera
 00000330: 6c5f 6269 6e64 734e 2907 da06 636f 6e66  l_bindsN)...conf
 00000340: 6967 da0f 6765 745f 6d61 696e 5f6f 7074  ig..get_main_opt
-00000350: 696f 6e72 0500 0000 da09 636f 6e66 6967  ionr......config
+00000350: 696f 6e72 0400 0000 da09 636f 6e66 6967  ionr......config
 00000360: 7572 6572 0a00 0000 da11 6265 6769 6e5f  urer......begin_
 00000370: 7472 616e 7361 6374 696f 6eda 0e72 756e  transaction..run
 00000380: 5f6d 6967 7261 7469 6f6e 7329 0172 0900  _migrations).r..
-00000390: 0000 a900 7211 0000 00fa 312f 686f 6d65  ....r.....1/home
+00000390: 0000 a900 7211 0000 00fa 392f 686f 6d65  ....r.....9/home
 000003a0: 2f73 616d 2f44 6f63 756d 656e 7473 2f67  /sam/Documents/g
-000003b0: 6974 2f63 6163 746f 6f6c 2f6d 6967 7261  it/cactool/migra
-000003c0: 7469 6f6e 732f 656e 762e 7079 da16 7275  tions/env.py..ru
-000003d0: 6e5f 6d69 6772 6174 696f 6e73 5f6f 6666  n_migrations_off
-000003e0: 6c69 6e65 2300 0000 730e 0000 000a 0c04  line#...s.......
-000003f0: 0106 0106 ff0a 040a 0122 ff72 1300 0000  .........".r....
-00000400: 6300 0000 0000 0000 0000 0000 0003 0000  c...............
-00000410: 0009 0000 0043 0000 0073 a600 0000 6401  .....C...s....d.
-00000420: 6402 8400 7d00 7400 6a01 6403 1900 6a02  d...}.t.j.d...j.
-00000430: a003 a100 7d01 7c01 a004 a100 8f39 7d02  ....}.|......9}.
-00000440: 7405 6a06 6406 7c02 7407 7c00 6404 9c03  t.j.d.|.t.|.d...
-00000450: 7400 6a01 6403 1900 6a08 a401 8e01 0100  t.j.d...j.......
-00000460: 7405 a009 a100 8f0c 0100 7405 a00a a100  t.........t.....
-00000470: 0100 5700 6405 0400 0400 8303 0100 6e10  ..W.d.........n.
-00000480: 3100 7334 7701 0100 0100 0100 5900 0100  1.s4w.......Y...
-00000490: 5700 6405 0400 0400 8303 0100 6405 5300  W.d.........d.S.
-000004a0: 5700 6405 0400 0400 8303 0100 6405 5300  W.d.........d.S.
-000004b0: 3100 734c 7701 0100 0100 0100 5900 0100  1.sLw.......Y...
-000004c0: 6405 5300 2907 7a89 5275 6e20 6d69 6772  d.S.).z.Run migr
-000004d0: 6174 696f 6e73 2069 6e20 276f 6e6c 696e  ations in 'onlin
-000004e0: 6527 206d 6f64 652e 0a0a 2020 2020 496e  e' mode...    In
-000004f0: 2074 6869 7320 7363 656e 6172 696f 2077   this scenario w
-00000500: 6520 6e65 6564 2074 6f20 6372 6561 7465  e need to create
-00000510: 2061 6e20 456e 6769 6e65 0a20 2020 2061   an Engine.    a
-00000520: 6e64 2061 7373 6f63 6961 7465 2061 2063  nd associate a c
-00000530: 6f6e 6e65 6374 696f 6e20 7769 7468 2074  onnection with t
-00000540: 6865 2063 6f6e 7465 7874 2e0a 0a20 2020  he context...   
-00000550: 2063 0300 0000 0000 0000 0000 0000 0400   c..............
-00000560: 0000 0400 0000 5300 0000 7342 0000 0074  ......S...sB...t
-00000570: 0074 016a 0264 0164 0283 0372 1d7c 0264  .t.j.d.d...r.|.d
-00000580: 0319 007d 037c 036a 03a0 04a1 0072 1f67  ...}.|.j.....r.g
-00000590: 007c 0264 0064 0085 023c 0074 05a0 0664  .|.d.d...<.t...d
-000005a0: 04a1 0101 0064 0053 0064 0053 0064 0053  .....d.S.d.S.d.S
-000005b0: 0029 054e da0c 6175 746f 6765 6e65 7261  .).N..autogenera
-000005c0: 7465 4672 0100 0000 7a1e 4e6f 2063 6861  teFr....z.No cha
-000005d0: 6e67 6573 2069 6e20 7363 6865 6d61 2064  nges in schema d
-000005e0: 6574 6563 7465 642e 2907 da07 6765 7461  etected.)...geta
-000005f0: 7474 7272 0c00 0000 da08 636d 645f 6f70  ttrr......cmd_op
-00000600: 7473 da0b 7570 6772 6164 655f 6f70 73da  ts..upgrade_ops.
-00000610: 0869 735f 656d 7074 79da 066c 6f67 6765  .is_empty..logge
-00000620: 72da 0469 6e66 6f29 0472 0500 0000 da08  r..info).r......
-00000630: 7265 7669 7369 6f6e da0a 6469 7265 6374  revision..direct
-00000640: 6976 6573 da06 7363 7269 7074 7211 0000  ives..scriptr...
-00000650: 0072 1100 0000 7212 0000 00da 1b70 726f  .r....r......pro
-00000660: 6365 7373 5f72 6576 6973 696f 6e5f 6469  cess_revision_di
-00000670: 7265 6374 6976 6573 4300 0000 730e 0000  rectivesC...s...
-00000680: 000e 0108 010a 010c 010e 0104 fc04 027a  ...............z
-00000690: 3a72 756e 5f6d 6967 7261 7469 6f6e 735f  :run_migrations_
-000006a0: 6f6e 6c69 6e65 2e3c 6c6f 6361 6c73 3e2e  online.<locals>.
-000006b0: 7072 6f63 6573 735f 7265 7669 7369 6f6e  process_revision
-000006c0: 5f64 6972 6563 7469 7665 7372 0700 0000  _directivesr....
-000006d0: 2903 da0a 636f 6e6e 6563 7469 6f6e 720a  )...connectionr.
-000006e0: 0000 0072 1e00 0000 4e72 1100 0000 290b  ...r....Nr....).
-000006f0: 7204 0000 00da 0a65 7874 656e 7369 6f6e  r......extension
-00000700: 73da 0264 62da 0a67 6574 5f65 6e67 696e  s..db..get_engin
-00000710: 65da 0763 6f6e 6e65 6374 7205 0000 0072  e..connectr....r
-00000720: 0e00 0000 720a 0000 00da 0e63 6f6e 6669  ....r......confi
-00000730: 6775 7265 5f61 7267 7372 0f00 0000 7210  gure_argsr....r.
-00000740: 0000 0029 0372 1e00 0000 da0b 636f 6e6e  ...).r......conn
-00000750: 6563 7461 626c 6572 1f00 0000 7211 0000  ectabler....r...
-00000760: 0072 1100 0000 7212 0000 00da 1572 756e  .r....r......run
-00000770: 5f6d 6967 7261 7469 6f6e 735f 6f6e 6c69  _migrations_onli
-00000780: 6e65 3800 0000 7320 0000 0008 0b10 070a  ne8...s ........
-00000790: 0206 0102 0102 0102 0104 fd0a 0406 fc0a  ................
-000007a0: 070a 011e ff0e f802 0822 f872 2600 0000  .........".r&...
-000007b0: 2919 da0a 5f5f 6675 7475 7265 5f5f 7202  )...__future__r.
-000007c0: 0000 00da 076c 6f67 6769 6e67 5a0e 6c6f  .....loggingZ.lo
-000007d0: 6767 696e 672e 636f 6e66 6967 7203 0000  gging.configr...
-000007e0: 00da 0566 6c61 736b 7204 0000 00da 0761  ...flaskr......a
-000007f0: 6c65 6d62 6963 7205 0000 0072 0c00 0000  lembicr....r....
-00000800: da10 636f 6e66 6967 5f66 696c 655f 6e61  ..config_file_na
-00000810: 6d65 da09 6765 744c 6f67 6765 7272 1900  me..getLoggerr..
-00000820: 0000 da0f 7365 745f 6d61 696e 5f6f 7074  ....set_main_opt
-00000830: 696f 6eda 0373 7472 7220 0000 0072 2100  ion..strr ...r!.
-00000840: 0000 7222 0000 0072 0900 0000 da07 7265  ..r"...r......re
-00000850: 706c 6163 65da 086d 6574 6164 6174 6172  place..metadatar
-00000860: 0a00 0000 7213 0000 0072 2600 0000 da0f  ....r....r&.....
-00000870: 6973 5f6f 6666 6c69 6e65 5f6d 6f64 6572  is_offline_moder
-00000880: 1100 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
-00000890: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000008a0: 0073 2800 0000 0c00 0802 0c01 0c02 0c02  .s(.............
-000008b0: 0604 0a04 0a01 0406 0201 1601 0401 02ff  ................
-000008c0: 04fe 0e04 0808 0815 0820 0a01 0a02       ......... ....
+000003b0: 6974 2f63 6163 746f 6f6c 2f63 6163 746f  it/cactool/cacto
+000003c0: 6f6c 2f6d 6967 7261 7469 6f6e 732f 656e  ol/migrations/en
+000003d0: 762e 7079 da16 7275 6e5f 6d69 6772 6174  v.py..run_migrat
+000003e0: 696f 6e73 5f6f 6666 6c69 6e65 2200 0000  ions_offline"...
+000003f0: 730a 0000 000a 0c10 010a 020a 0122 ff72  s............".r
+00000400: 1300 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000410: 0003 0000 0009 0000 0043 0000 0073 a600  .........C...s..
+00000420: 0000 6401 6402 8400 7d00 7400 6a01 6403  ..d.d...}.t.j.d.
+00000430: 1900 6a02 a003 a100 7d01 7c01 a004 a100  ..j.....}.|.....
+00000440: 8f39 7d02 7405 6a06 6406 7c02 7407 7c00  .9}.t.j.d.|.t.|.
+00000450: 6404 9c03 7400 6a01 6403 1900 6a08 a401  d...t.j.d...j...
+00000460: 8e01 0100 7405 a009 a100 8f0c 0100 7405  ....t.........t.
+00000470: a00a a100 0100 5700 6405 0400 0400 8303  ......W.d.......
+00000480: 0100 6e10 3100 7334 7701 0100 0100 0100  ..n.1.s4w.......
+00000490: 5900 0100 5700 6405 0400 0400 8303 0100  Y...W.d.........
+000004a0: 6405 5300 5700 6405 0400 0400 8303 0100  d.S.W.d.........
+000004b0: 6405 5300 3100 734c 7701 0100 0100 0100  d.S.1.sLw.......
+000004c0: 5900 0100 6405 5300 2907 7a89 5275 6e20  Y...d.S.).z.Run 
+000004d0: 6d69 6772 6174 696f 6e73 2069 6e20 276f  migrations in 'o
+000004e0: 6e6c 696e 6527 206d 6f64 652e 0a0a 2020  nline' mode...  
+000004f0: 2020 496e 2074 6869 7320 7363 656e 6172    In this scenar
+00000500: 696f 2077 6520 6e65 6564 2074 6f20 6372  io we need to cr
+00000510: 6561 7465 2061 6e20 456e 6769 6e65 0a20  eate an Engine. 
+00000520: 2020 2061 6e64 2061 7373 6f63 6961 7465     and associate
+00000530: 2061 2063 6f6e 6e65 6374 696f 6e20 7769   a connection wi
+00000540: 7468 2074 6865 2063 6f6e 7465 7874 2e0a  th the context..
+00000550: 0a20 2020 2063 0300 0000 0000 0000 0000  .    c..........
+00000560: 0000 0400 0000 0400 0000 5300 0000 7342  ..........S...sB
+00000570: 0000 0074 0074 016a 0264 0164 0283 0372  ...t.t.j.d.d...r
+00000580: 1d7c 0264 0319 007d 037c 036a 03a0 04a1  .|.d...}.|.j....
+00000590: 0072 1f67 007c 0264 0064 0085 023c 0074  .r.g.|.d.d...<.t
+000005a0: 05a0 0664 04a1 0101 0064 0053 0064 0053  ...d.....d.S.d.S
+000005b0: 0064 0053 0029 054e da0c 6175 746f 6765  .d.S.).N..autoge
+000005c0: 6e65 7261 7465 4672 0100 0000 7a1e 4e6f  nerateFr....z.No
+000005d0: 2063 6861 6e67 6573 2069 6e20 7363 6865   changes in sche
+000005e0: 6d61 2064 6574 6563 7465 642e 2907 da07  ma detected.)...
+000005f0: 6765 7461 7474 7272 0c00 0000 da08 636d  getattrr......cm
+00000600: 645f 6f70 7473 da0b 7570 6772 6164 655f  d_opts..upgrade_
+00000610: 6f70 73da 0869 735f 656d 7074 79da 066c  ops..is_empty..l
+00000620: 6f67 6765 72da 0469 6e66 6f29 0472 0400  ogger..info).r..
+00000630: 0000 da08 7265 7669 7369 6f6e da0a 6469  ....revision..di
+00000640: 7265 6374 6976 6573 da06 7363 7269 7074  rectives..script
+00000650: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
+00000660: 1b70 726f 6365 7373 5f72 6576 6973 696f  .process_revisio
+00000670: 6e5f 6469 7265 6374 6976 6573 4000 0000  n_directives@...
+00000680: 730e 0000 000e 0108 010a 010c 010e 0104  s...............
+00000690: fc04 027a 3a72 756e 5f6d 6967 7261 7469  ...z:run_migrati
+000006a0: 6f6e 735f 6f6e 6c69 6e65 2e3c 6c6f 6361  ons_online.<loca
+000006b0: 6c73 3e2e 7072 6f63 6573 735f 7265 7669  ls>.process_revi
+000006c0: 7369 6f6e 5f64 6972 6563 7469 7665 7372  sion_directivesr
+000006d0: 0700 0000 2903 da0a 636f 6e6e 6563 7469  ....)...connecti
+000006e0: 6f6e 720a 0000 0072 1e00 0000 4e72 1100  onr....r....Nr..
+000006f0: 0000 290b 7205 0000 00da 0a65 7874 656e  ..).r......exten
+00000700: 7369 6f6e 73da 0264 62da 0a67 6574 5f65  sions..db..get_e
+00000710: 6e67 696e 65da 0763 6f6e 6e65 6374 7204  ngine..connectr.
+00000720: 0000 0072 0e00 0000 720a 0000 00da 0e63  ...r....r......c
+00000730: 6f6e 6669 6775 7265 5f61 7267 7372 0f00  onfigure_argsr..
+00000740: 0000 7210 0000 0029 0372 1e00 0000 da0b  ..r....).r......
+00000750: 636f 6e6e 6563 7461 626c 6572 1f00 0000  connectabler....
+00000760: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
+00000770: 1572 756e 5f6d 6967 7261 7469 6f6e 735f  .run_migrations_
+00000780: 6f6e 6c69 6e65 3500 0000 7320 0000 0008  online5...s ....
+00000790: 0b10 070a 0206 0102 0102 0102 0104 fd0a  ................
+000007a0: 0406 fc0a 070a 011e ff0e f802 0822 f872  .............".r
+000007b0: 2600 0000 2919 da0a 5f5f 6675 7475 7265  &...)...__future
+000007c0: 5f5f 7202 0000 00da 076c 6f67 6769 6e67  __r......logging
+000007d0: 5a0e 6c6f 6767 696e 672e 636f 6e66 6967  Z.logging.config
+000007e0: 7203 0000 00da 0761 6c65 6d62 6963 7204  r......alembicr.
+000007f0: 0000 00da 0566 6c61 736b 7205 0000 0072  .....flaskr....r
+00000800: 0c00 0000 da10 636f 6e66 6967 5f66 696c  ......config_fil
+00000810: 655f 6e61 6d65 da09 6765 744c 6f67 6765  e_name..getLogge
+00000820: 7272 1900 0000 da0f 7365 745f 6d61 696e  rr......set_main
+00000830: 5f6f 7074 696f 6eda 0373 7472 7220 0000  _option..strr ..
+00000840: 0072 2100 0000 7222 0000 0072 0900 0000  .r!...r"...r....
+00000850: da07 7265 706c 6163 65da 086d 6574 6164  ..replace..metad
+00000860: 6174 6172 0a00 0000 7213 0000 0072 2600  atar....r....r&.
+00000870: 0000 da0f 6973 5f6f 6666 6c69 6e65 5f6d  ....is_offline_m
+00000880: 6f64 6572 1100 0000 7211 0000 0072 1100  oder....r....r..
+00000890: 0000 7212 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+000008a0: 3e01 0000 0073 2400 0000 0c00 0802 0c01  >....s$.........
+000008b0: 0c02 0c01 0604 0a04 0a01 0406 0201 1c01  ................
+000008c0: 04fe 0e04 0808 0813 0820 0a01 0a02       ......... ....
```

### Comparing `Cactool-0.5.7.6/cactool/migrations/alembic.ini` & `Cactool-0.6.0/cactool/migrations/alembic.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# A generic, single database configuration.
-
 [alembic]
 # template used to generate migration files
 # file_template = %%(rev)s_%%(slug)s
 
 # set to 'true' to run the environment during
 # the 'revision' command, regardless of autogenerate
 # revision_environment = false
+script_location = .
 
 
 # Logging configuration
 [loggers]
 keys = root,sqlalchemy,alembic,flask_migrate
 
 [handlers]
```

### Comparing `Cactool-0.5.7.6/cactool/migrations/env.py` & `Cactool-0.6.0/cactool/migrations/env.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 from __future__ import with_statement
 
 import logging
 from logging.config import fileConfig
 
-from flask import current_app
-
 from alembic import context
+from flask import current_app
 
 # this is the Alembic Config object, which provides
 # access to the values within the .ini file in use.
 config = context.config
 
 # Interpret the config file for Python logging.
 # This line sets up loggers basically.
 fileConfig(config.config_file_name)
-logger = logging.getLogger('alembic.env')
+logger = logging.getLogger("alembic.env")
 
 # add your model's MetaData object here
 # for 'autogenerate' support
 # from myapp import mymodel
 # target_metadata = mymodel.Base.metadata
 config.set_main_option(
-    'sqlalchemy.url',
-    str(current_app.extensions['migrate'].db.get_engine().url).replace(
-        '%', '%%'))
-target_metadata = current_app.extensions['migrate'].db.metadata
+    "sqlalchemy.url",
+    str(current_app.extensions["migrate"].db.get_engine().url).replace("%", "%%"),
+)
+target_metadata = current_app.extensions["migrate"].db.metadata
 
 # other values from the config, defined by the needs of env.py,
 # can be acquired:
 # my_important_option = config.get_main_option("my_important_option")
 # ... etc.
 
 
@@ -41,17 +40,15 @@
     we don't even need a DBAPI to be available.
 
     Calls to context.execute() here emit the given string to the
     script output.
 
     """
     url = config.get_main_option("sqlalchemy.url")
-    context.configure(
-        url=url, target_metadata=target_metadata, literal_binds=True
-    )
+    context.configure(url=url, target_metadata=target_metadata, literal_binds=True)
 
     with context.begin_transaction():
         context.run_migrations()
 
 
 def run_migrations_online():
     """Run migrations in 'online' mode.
@@ -61,28 +58,28 @@
 
     """
 
     # this callback is used to prevent an auto-migration from being generated
     # when there are no changes to the schema
     # reference: http://alembic.zzzcomputing.com/en/latest/cookbook.html
     def process_revision_directives(context, revision, directives):
-        if getattr(config.cmd_opts, 'autogenerate', False):
+        if getattr(config.cmd_opts, "autogenerate", False):
             script = directives[0]
             if script.upgrade_ops.is_empty():
                 directives[:] = []
-                logger.info('No changes in schema detected.')
+                logger.info("No changes in schema detected.")
 
-    connectable = current_app.extensions['migrate'].db.get_engine()
+    connectable = current_app.extensions["migrate"].db.get_engine()
 
     with connectable.connect() as connection:
         context.configure(
             connection=connection,
             target_metadata=target_metadata,
             process_revision_directives=process_revision_directives,
-            **current_app.extensions['migrate'].configure_args
+            **current_app.extensions["migrate"].configure_args
         )
 
         with context.begin_transaction():
             context.run_migrations()
 
 
 if context.is_offline_mode():
```

### Comparing `Cactool-0.5.7.6/cactool/migrations/versions/7226d855d8ec_add_more_ordinal_data_types.py` & `Cactool-0.6.0/cactool/migrations/versions/7226d855d8ec_add_more_ordinal_data_types.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,51 @@
 """Add more ordinal data types
 
 Revision ID: 7226d855d8ec
 Revises: d1b66364eeb3
 Create Date: 2022-02-27 16:24:17.410544
 
 """
-from alembic import op
 import sqlalchemy as sa
-
+from alembic import op
 
 # revision identifiers, used by Alembic.
-revision = '7226d855d8ec'
-down_revision = 'd1b66364eeb3'
+revision = "7226d855d8ec"
+down_revision = "d1b66364eeb3"
 branch_labels = None
 depends_on = None
 
 old_data_types = sa.Enum(
-    'STRING',
-    'NUMBER',
-    'LIST',
-    'BOOLEAN',
-    'SOCIAL_MEDIA',
-    'HIDDEN',
-    'LIKERT',
-    name='type'
+    "STRING",
+    "NUMBER",
+    "LIST",
+    "BOOLEAN",
+    "SOCIAL_MEDIA",
+    "HIDDEN",
+    "LIKERT",
+    name="type",
 )
 
 new_data_types = sa.Enum(
-    'STRING',
-    'NUMBER',
-    'LIST',
-    'BOOLEAN',
-    'SOCIAL_MEDIA',
-    'HIDDEN',
-    'LIKERT',
-    'ONE_TO_THREE',
-    'ONE_TO_FIVE',
-    'ONE_TO_SEVEN',
-    name='type'
+    "STRING",
+    "NUMBER",
+    "LIST",
+    "BOOLEAN",
+    "SOCIAL_MEDIA",
+    "HIDDEN",
+    "LIKERT",
+    "ONE_TO_THREE",
+    "ONE_TO_FIVE",
+    "ONE_TO_SEVEN",
+    name="type",
 )
 
+
 def upgrade():
     with op.batch_alter_table("dataset_column") as batch_op:
         batch_op.alter_column(
-            "type",
-            existing_type=old_data_types,
-            type_=new_data_types
+            "type", existing_type=old_data_types, type_=new_data_types
         )
 
 
 def downgrade():
     pass
```

### Comparing `Cactool-0.5.7.6/cactool/static/assets/cactool-large.png` & `Cactool-0.6.0/cactool/static/assets/cactool-large.png`

 * *Files identical despite different names*

### Comparing `Cactool-0.5.7.6/cactool/static/assets/favicon.ico` & `Cactool-0.6.0/cactool/static/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `Cactool-0.5.7.6/cactool/static/bin/tiktok_embed.js` & `Cactool-0.6.0/cactool/static/bin/tiktok_embed.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,2667 +1,2696 @@
-(function(e) {
-    var t = {};
-
-    function r(n) {
-        if (t[n]) return t[n].exports;
-        var a = t[n] = {
-            i: n,
-            l: false,
-            exports: {}
-        };
-        e[n].call(a.exports, a, a.exports, r);
-        a.l = true;
-        return a.exports
-    }
-    r.m = e;
-    r.c = t;
-    r.d = function(e, t, n) {
-        if (!r.o(e, t)) Object.defineProperty(e, t, {
-            enumerable: true,
-            get: n
-        })
-    };
-    r.r = function(e) {
-        if ("undefined" !== typeof Symbol && Symbol.toStringTag) Object.defineProperty(e, Symbol.toStringTag, {
-            value: "Module"
-        });
-        Object.defineProperty(e, "__esModule", {
-            value: true
-        })
-    };
-    r.t = function(e, t) {
-        if (1 & t) e = r(e);
-        if (8 & t) return e;
-        if (4 & t && "object" === typeof e && e && e.__esModule) return e;
-        var n = Object.create(null);
-        r.r(n);
-        Object.defineProperty(n, "default", {
-            enumerable: true,
-            value: e
-        });
-        if (2 & t && "string" != typeof e)
-            for (var a in e) r.d(n, a, function(t) {
-                return e[t]
-            }.bind(null, a));
-        return n
-    };
-    r.n = function(e) {
-        var t = e && e.__esModule ? function t() {
-            return e["default"]
-        } : function t() {
-            return e
-        };
-        r.d(t, "a", t);
-        return t
-    };
-    r.o = function(e, t) {
-        return Object.prototype.hasOwnProperty.call(e, t)
-    };
-    r.p = "/";
-    return r(r.s = 0)
-})({
-    0: function(e, t, r) {
-        r("3fe06cb9615786e0ea67");
-        e.exports = r("3177845424933048caec")
-    },
-    "0116c75136b233002fb9": function(e, t) {
-        var r = {}.toString;
-        e.exports = function(e) {
-            return r.call(e).slice(8, -1)
-        }
-    },
-    "03192b087bb464f059c0": function(e, t, r) {
-        "use strict";
-        var n = r("d394d0a4c1838202489d");
-        var a = r("23d432718b3e8ce32362");
-        var c = r("ca19e32ab6ee3b3692aa");
-        e.exports = function e(t) {
-            var r = n(this);
-            var i = c(r.length);
-            var o = arguments.length;
-            var f = a(o > 1 ? arguments[1] : void 0, i);
-            var u = o > 2 ? arguments[2] : void 0;
-            var d = void 0 === u ? i : a(u, i);
-            while (d > f) r[f++] = t;
-            return r
-        }
-    },
-    "0565be87d109f51269ca": function(e, t, r) {
-        "use strict";
-        var n = r("2d13d93c336705cd8ff9");
-        var a = r("ecd0e0fb36455021f082")(2);
-        n(n.P + n.F * !r("40b064d4eb439c0c1c2b")([].filter, true), "Array", {
-            filter: function e(t) {
-                return a(this, t, arguments[1])
-            }
-        })
-    },
-    "0594430ce9777a0767aa": function(e, t, r) {
-        var n = r("6ae9955278ddcf01bbfd");
-        e.exports = function(e, t) {
-            return new(n(e))(t)
-        }
-    },
-    "06b2b473e53cc019ca74": function(e, t, r) {
-        "use strict";
-        var n = r("d394d0a4c1838202489d");
-        var a = r("23d432718b3e8ce32362");
-        var c = r("ca19e32ab6ee3b3692aa");
-        e.exports = [].copyWithin || function e(t, r) {
-            var i = n(this);
-            var o = c(i.length);
-            var f = a(t, o);
-            var u = a(r, o);
-            var d = arguments.length > 2 ? arguments[2] : void 0;
-            var s = Math.min((void 0 === d ? o : a(d, o)) - u, o - f);
-            var v = 1;
-            if (u < f && f < u + s) {
-                v = -1;
-                u += s - 1;
-                f += s - 1
-            }
-            while (s-- > 0) {
-                if (u in i) i[f] = i[u];
-                else delete i[f];
-                f += v;
-                u += v
-            }
-            return i
-        }
-    },
-    "0a5193b0534d54dbcda1": function(e, t, r) {
-        "use strict";
-        var n = r("0e717e1f47872428608d");
-        var a = r("2d13d93c336705cd8ff9");
-        var c = r("d394d0a4c1838202489d");
-        var i = r("4357234160788ed77205");
-        var o = r("71d3ec5bd65418e28ebc");
-        var f = r("ca19e32ab6ee3b3692aa");
-        var u = r("8de492c765fbfb624515");
-        var d = r("f88518adc3004bf8d923");
-        a(a.S + a.F * !r("574ea81f94fc0b2f332a")((function(e) {
-            Array.from(e)
-        })), "Array", {
-            from: function e(t) {
-                var r = c(t);
-                var a = "function" == typeof this ? this : Array;
-                var s = arguments.length;
-                var v = s > 1 ? arguments[1] : void 0;
-                var l = void 0 !== v;
-                var b = 0;
-                var h = d(r);
-                var p, y, m, g;
-                if (l) v = n(v, s > 2 ? arguments[2] : void 0, 2);
-                if (void 0 != h && !(a == Array && o(h)))
-                    for (g = h.call(r), y = new a; !(m = g.next()).done; b++) u(y, b, l ? i(g, v, [m.value, b], true) : m.value);
-                else {
-                    p = f(r.length);
-                    for (y = new a(p); p > b; b++) u(y, b, l ? v(r[b], b) : r[b])
-                }
-                y.length = b;
-                return y
-            }
-        })
-    },
-    "0e717e1f47872428608d": function(e, t, r) {
-        var n = r("4d073e2fededcdd3f3d3");
-        e.exports = function(e, t, r) {
-            n(e);
-            if (void 0 === t) return e;
-            switch (r) {
-                case 1:
-                    return function(r) {
-                        return e.call(t, r)
-                    };
-                case 2:
-                    return function(r, n) {
-                        return e.call(t, r, n)
-                    };
-                case 3:
-                    return function(r, n, a) {
-                        return e.call(t, r, n, a)
-                    }
-            }
-            return function() {
-                return e.apply(t, arguments)
-            }
-        }
-    },
-    "0f025c284bc567debf3d": function(e, t, r) {
-        "use strict";
-        var n = r("2d13d93c336705cd8ff9");
-        var a = r("ecd0e0fb36455021f082")(0);
-        var c = r("40b064d4eb439c0c1c2b")([].forEach, true);
-        n(n.P + n.F * !c, "Array", {
-            forEach: function e(t) {
-                return a(this, t, arguments[1])
-            }
-        })
-    },
-    "1139de1233fd67f45bd7": function(e, t) {
-        var r = e.exports = "undefined" != typeof window && window.Math == Math ? window : "undefined" != typeof self && self.Math == Math ? self : Function("return this")();
-        if ("number" == typeof __g) __g = r
-    },
-    "12323e1413cbffdabe02": function(e, t, r) {
-        var n = r("d34390b928ecadc11dc8");
-        var a = r("d394d0a4c1838202489d");
-        var c = r("5f6eded14a8ed86276fc")("IE_PROTO");
-        var i = Object.prototype;
-        e.exports = Object.getPrototypeOf || function(e) {
-            e = a(e);
-            if (n(e, c)) return e[c];
-            if ("function" == typeof e.constructor && e instanceof e.constructor) return e.constructor.prototype;
-            return e instanceof Object ? i : null
-        }
-    },
-    "145c4f2bdc487b2578df": function(e, t, r) {
-        var n = r("e3136eea77d23f8d97ec");
-        var a = r("380c0734c088ca78ccda");
-        e.exports = Object.keys || function e(t) {
-            return n(t, a)
-        }
-    },
-    "1468f5d37f30f63d76ea": function(e, t, r) {
-        "use strict";
-        var n = r("2d13d93c336705cd8ff9");
-        var a = r("efae14a3f8cd9a616256");
-        var c = r("1f3157d073736826d4fa");
-        var i = r("ca19e32ab6ee3b3692aa");
-        var o = [].lastIndexOf;
-        var f = !!o && 1 / [1].lastIndexOf(1, -0) < 0;
-        n(n.P + n.F * (f || !r("40b064d4eb439c0c1c2b")(o)), "Array", {
-            lastIndexOf: function e(t) {
-                if (f) return o.apply(this, arguments) || 0;
-                var r = a(this);
-                var n = i(r.length);
-                var u = n - 1;
-                if (arguments.length > 1) u = Math.min(u, c(arguments[1]));
-                if (u < 0) u = n + u;
-                for (; u >= 0; u--)
-                    if (u in r)
-                        if (r[u] === t) return u || 0;
-                return -1
-            }
-        })
-    },
-    "1591b90b4327c94245ad": function(e, t, r) {
-        "use strict";
-        var n = r("2d13d93c336705cd8ff9");
-        var a = r("ecd0e0fb36455021f082")(1);
-        n(n.P + n.F * !r("40b064d4eb439c0c1c2b")([].map, true), "Array", {
-            map: function e(t) {
-                return a(this, t, arguments[1])
-            }
-        })
-    },
-    "1b01d0e59d3af79760a0": function(e, t, r) {
-        var n = r("79c91dcd8cd554c59c7b");
-        var a = r("bc1a333d2b6eceac22e3");
-        var c = r("4ef7a75a1d1957a7c5c0");
-        var i = Object.defineProperty;
-        t.f = r("5975c7ea3ecd56e534e3") ? Object.defineProperty : function e(t, r, o) {
-            n(t);
-            r = c(r, true);
-            n(o);
-            if (a) try {
-                return i(t, r, o)
-            } catch (f) {}
-            if ("get" in o || "set" in o) throw TypeError("Accessors not supported!");
-            if ("value" in o) t[r] = o.value;
-            return t
-        }
-    },
-    "1b24b031f63a74d1f57f": function(e, t, r) {
-        "use strict";
-        var n = r("f8f08bdd917755ac017a");
-
-        function a() {}
-        var c = null;
-        var i = {};
-
-        function o(e) {
-            try {
-                return e.then
-            } catch (t) {
-                c = t;
-                return i
-            }
-        }
-
-        function f(e, t) {
-            try {
-                return e(t)
-            } catch (r) {
-                c = r;
-                return i
-            }
-        }
-
-        function u(e, t, r) {
-            try {
-                e(t, r)
-            } catch (n) {
-                c = n;
-                return i
-            }
-        }
-        e.exports = d;
-
-        function d(e) {
-            if ("object" !== typeof this) throw new TypeError("Promises must be constructed via new");
-            if ("function" !== typeof e) throw new TypeError("Promise constructor's argument is not a function");
-            this._U = 0;
-            this._V = 0;
-            this._W = null;
-            this._X = null;
-            if (e === a) return;
-            m(e, this)
-        }
-        d._Y = null;
-        d._Z = null;
-        d._0 = a;
-        d.prototype.then = function(e, t) {
-            if (this.constructor !== d) return s(this, e, t);
-            var r = new d(a);
-            v(this, new y(e, t, r));
-            return r
-        };
-
-        function s(e, t, r) {
-            return new e.constructor((function(n, c) {
-                var i = new d(a);
-                i.then(n, c);
-                v(e, new y(t, r, i))
-            }))
-        }
-
-        function v(e, t) {
-            while (3 === e._V) e = e._W;
-            if (d._Y) d._Y(e);
-            if (0 === e._V) {
-                if (0 === e._U) {
-                    e._U = 1;
-                    e._X = t;
-                    return
-                }
-                if (1 === e._U) {
-                    e._U = 2;
-                    e._X = [e._X, t];
-                    return
-                }
-                e._X.push(t);
-                return
-            }
-            l(e, t)
-        }
-
-        function l(e, t) {
-            n((function() {
-                var r = 1 === e._V ? t.onFulfilled : t.onRejected;
-                if (null === r) {
-                    if (1 === e._V) b(t.promise, e._W);
-                    else h(t.promise, e._W);
-                    return
-                }
-                var n = f(r, e._W);
-                if (n === i) h(t.promise, c);
-                else b(t.promise, n)
-            }))
-        }
-
-        function b(e, t) {
-            if (t === e) return h(e, new TypeError("A promise cannot be resolved with itself."));
-            if (t && ("object" === typeof t || "function" === typeof t)) {
-                var r = o(t);
-                if (r === i) return h(e, c);
-                if (r === e.then && t instanceof d) {
-                    e._V = 3;
-                    e._W = t;
-                    p(e);
-                    return
-                } else if ("function" === typeof r) {
-                    m(r.bind(t), e);
-                    return
-                }
-            }
-            e._V = 1;
-            e._W = t;
-            p(e)
-        }
-
-        function h(e, t) {
-            e._V = 2;
-            e._W = t;
-            if (d._Z) d._Z(e, t);
-            p(e)
-        }
-
-        function p(e) {
-            if (1 === e._U) {
-                v(e, e._X);
-                e._X = null
-            }
-            if (2 === e._U) {
-                for (var t = 0; t < e._X.length; t++) v(e, e._X[t]);
-                e._X = null
-            }
-        }
-
-        function y(e, t, r) {
-            this.onFulfilled = "function" === typeof e ? e : null;
-            this.onRejected = "function" === typeof t ? t : null;
-            this.promise = r
-        }
-
-        function m(e, t) {
-            var r = false;
-            var n = u(e, (function(e) {
-                if (r) return;
-                r = true;
-                b(t, e)
-            }), (function(e) {
-                if (r) return;
-                r = true;
-                h(t, e)
-            }));
-            if (!r && n === i) {
-                r = true;
-                h(t, c)
-            }
-        }
-    },
-    "1b71f5e96f29a92413b6": function(e, t, r) {
-        "use strict";
-        var n = r("2d13d93c336705cd8ff9");
-        var a = r("5b9dc0e027f5c68eff1a");
-        var c = r("0116c75136b233002fb9");
-        var i = r("23d432718b3e8ce32362");
-        var o = r("ca19e32ab6ee3b3692aa");
-        var f = [].slice;
-        n(n.P + n.F * r("7a7739dd8a198a2cfcb5")((function() {
-            if (a) f.call(a)
-        })), "Array", {
-            slice: function e(t, r) {
-                var n = o(this.length);
-                var a = c(this);
-                r = void 0 === r ? n : r;
-                if ("Array" == a) return f.call(this, t, r);
-                var u = i(t, n);
-                var d = i(r, n);
-                var s = o(d - u);
-                var v = new Array(s);
-                var l = 0;
-                for (; l < s; l++) v[l] = "String" == a ? this.charAt(u + l) : this[u + l];
-                return v
-            }
-        })
-    },
-    "1e0f00d296712713afe6": function(e, t, r) {
-        var n = r("4d073e2fededcdd3f3d3");
-        var a = r("d394d0a4c1838202489d");
-        var c = r("a537d0accb907bf9d41f");
-        var i = r("ca19e32ab6ee3b3692aa");
-        e.exports = function(e, t, r, o, f) {
-            n(t);
-            var u = a(e);
-            var d = c(u);
-            var s = i(u.length);
-            var v = f ? s - 1 : 0;
-            var l = f ? -1 : 1;
-            if (r < 2)
-                for (;;) {
-                    if (v in d) {
-                        o = d[v];
-                        v += l;
-                        break
-                    }
-                    v += l;
-                    if (f ? v < 0 : s <= v) throw TypeError("Reduce of empty array with no initial value")
-                }
-            for (; f ? v >= 0 : s > v; v += l)
-                if (v in d) o = t(o, d[v], v, u);
-            return o
-        }
-    },
-    "1f3157d073736826d4fa": function(e, t) {
-        var r = Math.ceil;
-        var n = Math.floor;
-        e.exports = function(e) {
-            return isNaN(e = +e) ? 0 : (e > 0 ? n : r)(e)
-        }
-    },
-    "2076e982c14c41925fb4": function(e, t, r) {
-        var n = r("efae14a3f8cd9a616256");
-        var a = r("ca19e32ab6ee3b3692aa");
-        var c = r("23d432718b3e8ce32362");
-        e.exports = function(e) {
-            return function(t, r, i) {
-                var o = n(t);
-                var f = a(o.length);
-                var u = c(i, f);
-                var d;
-                if (e && r != r)
-                    while (f > u) {
-                        d = o[u++];
-                        if (d != d) return true
-                    } else
-                        for (; f > u; u++)
-                            if (e || u in o)
-                                if (o[u] === r) return e || u || 0;
-                return !e && -1
-            }
-        }
-    },
-    "224ae09e536c09e69a0a": function(e, t) {
-        e.exports = {}
-    },
-    "23617503340803072f22": function(e, t, r) {
-        "use strict";
-        r.d(t, "b", (function() {
-            return i
-        }));
-        r.d(t, "d", (function() {
-            return o
-        }));
-        r.d(t, "a", (function() {
-            return v
-        }));
-        r.d(t, "c", (function() {
-            return l
-        }));
-
-        function n(e, t, r, n, a, c, i) {
-            try {
-                var o = e[c](i);
-                var f = o.value
-            } catch (u) {
-                r(u);
-                return
-            }
-            if (o.done) t(f);
-            else Promise.resolve(f).then(n, a)
-        }
-
-        function a(e) {
-            return function() {
-                var t = this,
-                    r = arguments;
-                return new Promise((function(a, c) {
-                    var i = e.apply(t, r);
-
-                    function o(e) {
-                        n(i, a, c, o, f, "next", e)
-                    }
-
-                    function f(e) {
-                        n(i, a, c, o, f, "throw", e)
-                    }
-                    o(void 0)
-                }))
-            }
-        }
-
-        function c(e) {
-            "@babel/helpers - typeof";
-            return c = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
-                return typeof e
-            } : function(e) {
-                return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-            }, c(e)
-        }
-
-        function i() {
-            return Math.round(1e17 * Math.random())
-        }
-
-        function o() {
-            var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : [];
-            var t = arguments.length > 1 ? arguments[1] : void 0;
-            var r = arguments.length > 2 ? arguments[2] : void 0;
-            if (!e.length || !t) return [];
-            return e.reduce((function() {
-                var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : [];
-                var n = arguments.length > 1 ? arguments[1] : void 0;
-                var a = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : 0;
-                var c = Math.floor(a / t);
-                if (!e[c]) e[c] = [];
-                if (r) e[c].push(n[r]);
-                else e[c].push(n);
-                return e
-            }), [])
-        }
-
-        function f(e, t) {
-            var r = t.type || "GET";
-            var n = t.data;
-            var a = t.success,
-                i = void 0 === a ? function e(t, r) {
-                    void 0
-                } : a,
-                o = t.fail,
-                f = void 0 === o ? function e(t, r) {
-                    void 0
-                } : o;
-            var u = new XMLHttpRequest;
-            u.onreadystatechange = function() {
-                if (4 === Number(u.readyState))
-                    if (u.status >= 200 && u.status < 300 || 304 === u.status) i(u.responseText, u);
-                    else f(u.responseText, u)
-            };
-
-            function d(e) {
-                var t = e;
-                var r = [];
-                if ("string" === typeof t) t = encodeURI(t);
-                else if ("object" === c(t)) {
-                    Object.keys(t).forEach((function(e) {
-                        r.push("".concat(e, "=").concat(encodeURIComponent(t[e].toString())))
-                    }));
-                    t = r.join("&")
-                }
-                return t
-            }
-            if ("GET" === r.toUpperCase()) {
-                var s = "".concat(e, "?").concat(d(n || ""));
-                u.open("get", s, true);
-                u.send(null)
-            } else if ("POST" === r.toUpperCase()) {
-                u.open("post", e, true);
-                u.setRequestHeader("Content-Type", "application/x-www-form-urlencoded");
-                u.send(d(n || ""))
-            }
-        }
-
-        function u(e, t) {
-            return d.apply(this, arguments)
-        }
-
-        function d() {
-            d = a(regeneratorRuntime.mark((function e(t, r) {
-                return regeneratorRuntime.wrap((function e(n) {
-                    while (1) switch (n.prev = n.next) {
-                        case 0:
-                            return n.abrupt("return", new Promise((function(e, n) {
-                                var a = {
-                                    data: r,
-                                    success: e,
-                                    fail: n
-                                };
-                                f(t, a)
-                            })).then((function() {
-                                var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "{}";
-                                var t = {};
-                                try {
-                                    t = JSON.parse(e)
-                                } catch (r) {
-                                    t = {}
-                                }
-                                return t
-                            })));
-                        case 1:
-                        case "end":
-                            return n.stop()
-                    }
-                }), e)
-            })));
-            return d.apply(this, arguments)
-        }
-
-        function s() {
-            var e = "TikTok";
-            var t = {};
-            var r = function t(r) {
-                return "[".concat(e, "] ").concat(r.toString())
-            };
-            ["error", "log", "info"].forEach((function(e) {
-                t[e] = function(t) {
-                    if ("info" === e) void 0;
-                    else void 0
-                }
-            }));
-            return t
-        }
-        var v = s();
-
-        function l(e) {
-            var t = e.replace(/[\[]/, "\\[").replace(/[\]]/, "\\]");
-            var r = new RegExp("[\\?&]".concat(t, "=([^&#]*)"));
-            var n = r.exec(location.search);
-            return null === n ? "" : decodeURIComponent(n[1].replace(/\+/g, " "))
-        }
-
-        function b() {
-            return false || "production" === "dev"
-        }
-    },
-    "23d432718b3e8ce32362": function(e, t, r) {
-        var n = r("1f3157d073736826d4fa");
-        var a = Math.max;
-        var c = Math.min;
-        e.exports = function(e, t) {
-            e = n(e);
-            return e < 0 ? a(e + t, 0) : c(e, t)
-        }
-    },
-    "273d2eedcd369c189e70": function(e, t) {
-        var r = 0;
-        var n = Math.random();
-        e.exports = function(e) {
-            return "Symbol(".concat(void 0 === e ? "" : e, ")_", (++r + n).toString(36))
-        }
-    },
-    "2c09af3fb5c4ba3698b3": function(e, t, r) {
-        var n = function(e) {
-            "use strict";
-            var t = Object.prototype;
-            var r = t.hasOwnProperty;
-            var n;
-            var a = "function" === typeof Symbol ? Symbol : {};
-            var c = a.iterator || "@@iterator";
-            var i = a.asyncIterator || "@@asyncIterator";
-            var o = a.toStringTag || "@@toStringTag";
-
-            function f(e, t, r, n) {
-                var a = t && t.prototype instanceof h ? t : h;
-                var c = Object.create(a.prototype);
-                var i = new A(n || []);
-                c._invoke = j(e, r, i);
-                return c
-            }
-            e.wrap = f;
-
-            function u(e, t, r) {
-                try {
-                    return {
-                        type: "normal",
-                        arg: e.call(t, r)
-                    }
-                } catch (n) {
-                    return {
-                        type: "throw",
-                        arg: n
-                    }
-                }
-            }
-            var d = "suspendedStart";
-            var s = "suspendedYield";
-            var v = "executing";
-            var l = "completed";
-            var b = {};
-
-            function h() {}
-
-            function p() {}
-
-            function y() {}
-            var m = {};
-            m[c] = function() {
-                return this
-            };
-            var g = Object.getPrototypeOf;
-            var w = g && g(g(P([])));
-            if (w && w !== t && r.call(w, c)) m = w;
-            var x = y.prototype = h.prototype = Object.create(m);
-            p.prototype = x.constructor = y;
-            y.constructor = p;
-            y[o] = p.displayName = "GeneratorFunction";
-
-            function _(e) {
-                ["next", "throw", "return"].forEach((function(t) {
-                    e[t] = function(e) {
-                        return this._invoke(t, e)
-                    }
-                }))
-            }
-            e.isGeneratorFunction = function(e) {
-                var t = "function" === typeof e && e.constructor;
-                return t ? t === p || "GeneratorFunction" === (t.displayName || t.name) : false
-            };
-            e.mark = function(e) {
-                if (Object.setPrototypeOf) Object.setPrototypeOf(e, y);
-                else {
-                    e.__proto__ = y;
-                    if (!(o in e)) e[o] = "GeneratorFunction"
-                }
-                e.prototype = Object.create(x);
-                return e
-            };
-            e.awrap = function(e) {
-                return {
-                    __await: e
-                }
-            };
-
-            function k(e, t) {
-                function n(a, c, i, o) {
-                    var f = u(e[a], e, c);
-                    if ("throw" === f.type) o(f.arg);
-                    else {
-                        var d = f.arg;
-                        var s = d.value;
-                        if (s && "object" === typeof s && r.call(s, "__await")) return t.resolve(s.__await).then((function(e) {
-                            n("next", e, i, o)
-                        }), (function(e) {
-                            n("throw", e, i, o)
-                        }));
-                        return t.resolve(s).then((function(e) {
-                            d.value = e;
-                            i(d)
-                        }), (function(e) {
-                            return n("throw", e, i, o)
-                        }))
-                    }
-                }
-                var a;
-
-                function c(e, r) {
-                    function c() {
-                        return new t((function(t, a) {
-                            n(e, r, t, a)
-                        }))
-                    }
-                    return a = a ? a.then(c, c) : c()
-                }
-                this._invoke = c
-            }
-            _(k.prototype);
-            k.prototype[i] = function() {
-                return this
-            };
-            e.AsyncIterator = k;
-            e.async = function(t, r, n, a, c) {
-                if (void 0 === c) c = Promise;
-                var i = new k(f(t, r, n, a), c);
-                return e.isGeneratorFunction(r) ? i : i.next().then((function(e) {
-                    return e.done ? e.value : i.next()
-                }))
-            };
-
-            function j(e, t, r) {
-                var n = d;
-                return function a(c, i) {
-                    if (n === v) throw new Error("Generator is already running");
-                    if (n === l) {
-                        if ("throw" === c) throw i;
-                        return I()
-                    }
-                    r.method = c;
-                    r.arg = i;
-                    while (true) {
-                        var o = r.delegate;
-                        if (o) {
-                            var f = E(o, r);
-                            if (f) {
-                                if (f === b) continue;
-                                return f
-                            }
-                        }
-                        if ("next" === r.method) r.sent = r._sent = r.arg;
-                        else if ("throw" === r.method) {
-                            if (n === d) {
-                                n = l;
-                                throw r.arg
-                            }
-                            r.dispatchException(r.arg)
-                        } else if ("return" === r.method) r.abrupt("return", r.arg);
-                        n = v;
-                        var h = u(e, t, r);
-                        if ("normal" === h.type) {
-                            n = r.done ? l : s;
-                            if (h.arg === b) continue;
-                            return {
-                                value: h.arg,
-                                done: r.done
-                            }
-                        } else if ("throw" === h.type) {
-                            n = l;
-                            r.method = "throw";
-                            r.arg = h.arg
-                        }
-                    }
-                }
-            }
-
-            function E(e, t) {
-                var r = e.iterator[t.method];
-                if (r === n) {
-                    t.delegate = null;
-                    if ("throw" === t.method) {
-                        if (e.iterator["return"]) {
-                            t.method = "return";
-                            t.arg = n;
-                            E(e, t);
-                            if ("throw" === t.method) return b
-                        }
-                        t.method = "throw";
-                        t.arg = new TypeError("The iterator does not provide a 'throw' method")
-                    }
-                    return b
-                }
-                var a = u(r, e.iterator, t.arg);
-                if ("throw" === a.type) {
-                    t.method = "throw";
-                    t.arg = a.arg;
-                    t.delegate = null;
-                    return b
-                }
-                var c = a.arg;
-                if (!c) {
-                    t.method = "throw";
-                    t.arg = new TypeError("iterator result is not an object");
-                    t.delegate = null;
-                    return b
-                }
-                if (c.done) {
-                    t[e.resultName] = c.value;
-                    t.next = e.nextLoc;
-                    if ("return" !== t.method) {
-                        t.method = "next";
-                        t.arg = n
-                    }
-                } else return c;
-                t.delegate = null;
-                return b
-            }
-            _(x);
-            x[o] = "Generator";
-            x[c] = function() {
-                return this
-            };
-            x.toString = function() {
-                return "[object Generator]"
-            };
-
-            function S(e) {
-                var t = {
-                    tryLoc: e[0]
-                };
-                if (1 in e) t.catchLoc = e[1];
-                if (2 in e) {
-                    t.finallyLoc = e[2];
-                    t.afterLoc = e[3]
-                }
-                this.tryEntries.push(t)
-            }
-
-            function O(e) {
-                var t = e.completion || {};
-                t.type = "normal";
-                delete t.arg;
-                e.completion = t
-            }
-
-            function A(e) {
-                this.tryEntries = [{
-                    tryLoc: "root"
-                }];
-                e.forEach(S, this);
-                this.reset(true)
-            }
-            e.keys = function(e) {
-                var t = [];
-                for (var r in e) t.push(r);
-                t.reverse();
-                return function r() {
-                    while (t.length) {
-                        var n = t.pop();
-                        if (n in e) {
-                            r.value = n;
-                            r.done = false;
-                            return r
-                        }
-                    }
-                    r.done = true;
-                    return r
-                }
-            };
-
-            function P(e) {
-                if (e) {
-                    var t = e[c];
-                    if (t) return t.call(e);
-                    if ("function" === typeof e.next) return e;
-                    if (!isNaN(e.length)) {
-                        var a = -1,
-                            i = function t() {
-                                while (++a < e.length)
-                                    if (r.call(e, a)) {
-                                        t.value = e[a];
-                                        t.done = false;
-                                        return t
-                                    } t.value = n;
-                                t.done = true;
-                                return t
-                            };
-                        return i.next = i
-                    }
-                }
-                return {
-                    next: I
-                }
-            }
-            e.values = P;
-
-            function I() {
-                return {
-                    value: n,
-                    done: true
-                }
-            }
-            A.prototype = {
-                constructor: A,
-                reset: function(e) {
-                    this.prev = 0;
-                    this.next = 0;
-                    this.sent = this._sent = n;
-                    this.done = false;
-                    this.delegate = null;
-                    this.method = "next";
-                    this.arg = n;
-                    this.tryEntries.forEach(O);
-                    if (!e)
-                        for (var t in this)
-                            if ("t" === t.charAt(0) && r.call(this, t) && !isNaN(+t.slice(1))) this[t] = n
-                },
-                stop: function() {
-                    this.done = true;
-                    var e = this.tryEntries[0];
-                    var t = e.completion;
-                    if ("throw" === t.type) throw t.arg;
-                    return this.rval
-                },
-                dispatchException: function(e) {
-                    if (this.done) throw e;
-                    var t = this;
-
-                    function a(r, a) {
-                        o.type = "throw";
-                        o.arg = e;
-                        t.next = r;
-                        if (a) {
-                            t.method = "next";
-                            t.arg = n
-                        }
-                        return !!a
-                    }
-                    for (var c = this.tryEntries.length - 1; c >= 0; --c) {
-                        var i = this.tryEntries[c];
-                        var o = i.completion;
-                        if ("root" === i.tryLoc) return a("end");
-                        if (i.tryLoc <= this.prev) {
-                            var f = r.call(i, "catchLoc");
-                            var u = r.call(i, "finallyLoc");
-                            if (f && u) {
-                                if (this.prev < i.catchLoc) return a(i.catchLoc, true);
-                                else if (this.prev < i.finallyLoc) return a(i.finallyLoc)
-                            } else if (f) {
-                                if (this.prev < i.catchLoc) return a(i.catchLoc, true)
-                            } else if (u) {
-                                if (this.prev < i.finallyLoc) return a(i.finallyLoc)
-                            } else throw new Error("try statement without catch or finally")
-                        }
-                    }
-                },
-                abrupt: function(e, t) {
-                    for (var n = this.tryEntries.length - 1; n >= 0; --n) {
-                        var a = this.tryEntries[n];
-                        if (a.tryLoc <= this.prev && r.call(a, "finallyLoc") && this.prev < a.finallyLoc) {
-                            var c = a;
-                            break
-                        }
-                    }
-                    if (c && ("break" === e || "continue" === e) && c.tryLoc <= t && t <= c.finallyLoc) c = null;
-                    var i = c ? c.completion : {};
-                    i.type = e;
-                    i.arg = t;
-                    if (c) {
-                        this.method = "next";
-                        this.next = c.finallyLoc;
-                        return b
-                    }
-                    return this.complete(i)
-                },
-                complete: function(e, t) {
-                    if ("throw" === e.type) throw e.arg;
-                    if ("break" === e.type || "continue" === e.type) this.next = e.arg;
-                    else if ("return" === e.type) {
-                        this.rval = this.arg = e.arg;
-                        this.method = "return";
-                        this.next = "end"
-                    } else if ("normal" === e.type && t) this.next = t;
-                    return b
-                },
-                finish: function(e) {
-                    for (var t = this.tryEntries.length - 1; t >= 0; --t) {
-                        var r = this.tryEntries[t];
-                        if (r.finallyLoc === e) {
-                            this.complete(r.completion, r.afterLoc);
-                            O(r);
-                            return b
-                        }
-                    }
-                },
-                catch: function(e) {
-                    for (var t = this.tryEntries.length - 1; t >= 0; --t) {
-                        var r = this.tryEntries[t];
-                        if (r.tryLoc === e) {
-                            var n = r.completion;
-                            if ("throw" === n.type) {
-                                var a = n.arg;
-                                O(r)
-                            }
-                            return a
-                        }
-                    }
-                    throw new Error("illegal catch attempt")
-                },
-                delegateYield: function(e, t, r) {
-                    this.delegate = {
-                        iterator: P(e),
-                        resultName: t,
-                        nextLoc: r
-                    };
-                    if ("next" === this.method) this.arg = n;
-                    return b
-                }
-            };
-            return e
-        }(true ? e.exports : void 0);
-        try {
-            regeneratorRuntime = n
-        } catch (a) {
-            Function("r", "regeneratorRuntime = r")(n)
-        }
-    },
-    "2d13d93c336705cd8ff9": function(e, t, r) {
-        var n = r("1139de1233fd67f45bd7");
-        var a = r("5925dad3c5243ffee3db");
-        var c = r("5f25c015bbbf9d42c661");
-        var i = r("88db22626e6c88b175cf");
-        var o = r("0e717e1f47872428608d");
-        var f = "prototype";
-        var u = function(e, t, r) {
-            var d = e & u.F;
-            var s = e & u.G;
-            var v = e & u.S;
-            var l = e & u.P;
-            var b = e & u.B;
-            var h = s ? n : v ? n[t] || (n[t] = {}) : (n[t] || {})[f];
-            var p = s ? a : a[t] || (a[t] = {});
-            var y = p[f] || (p[f] = {});
-            var m, g, w, x;
-            if (s) r = t;
-            for (m in r) {
-                g = !d && h && void 0 !== h[m];
-                w = (g ? h : r)[m];
-                x = b && g ? o(w, n) : l && "function" == typeof w ? o(Function.call, w) : w;
-                if (h) i(h, m, w, e & u.U);
-                if (p[m] != w) c(p, m, x);
-                if (l && y[m] != w) y[m] = w
-            }
-        };
-        n.core = a;
-        u.F = 1;
-        u.G = 2;
-        u.S = 4;
-        u.P = 8;
-        u.B = 16;
-        u.W = 32;
-        u.U = 64;
-        u.R = 128;
-        e.exports = u
-    },
-    "307014e72ed12da69e15": function(e, t, r) {
-        "use strict";
-        var n = r("a5e6f0092ff0290e0bcf");
-        var a = r("dabaabbe8ba08d59975f");
-        var c = r("224ae09e536c09e69a0a");
-        var i = r("efae14a3f8cd9a616256");
-        e.exports = r("429cfc8e3ed333e40618")(Array, "Array", (function(e, t) {
-            this._t = i(e);
-            this._i = 0;
-            this._k = t
-        }), (function() {
-            var e = this._t;
-            var t = this._k;
-            var r = this._i++;
-            if (!e || r >= e.length) {
-                this._t = void 0;
-                return a(1)
-            }
-            if ("keys" == t) return a(0, r);
-            if ("values" == t) return a(0, e[r]);
-            return a(0, [r, e[r]])
-        }), "values");
-        c.Arguments = c.Array;
-        n("keys");
-        n("values");
-        n("entries")
-    },
-    "3177845424933048caec": function(e, t, r) {
-        "use strict";
-        r.r(t);
-        var n = r("3fe06cb9615786e0ea67");
-        var a = r("e0b8897ffbf48a102fbb");
-        var c = window.localStorage;
-        var i = window.sessionStorage;
-
-        function o(e) {
-            function t() {
-                var e = "".concat(a["j"], "storage_test");
-                var t = "";
-                try {
-                    t = i.getItem(e);
-                    if (!t) i.setItem(e, true)
-                } catch (r) {
-                    i.setItem(e, "")
-                }
-                return Boolean(t)
-            }
-            this.getItem = function(r) {
-                var n = "";
-                if (t()) n = e.getItem("".concat(a["j"]).concat(r));
-                return n
-            };
-            this.setItem = function(r, n) {
-                if (t()) e.setItem("".concat(a["j"]).concat(r), n)
-            };
-            this.removeItem = function(r) {
-                if (t()) e.removeItem("".concat(a["j"]).concat(r))
-            }
-        }
-        var f = new o(c);
-        var u = new o(i);
-        var d = r("23617503340803072f22");
-
-        function s(e, t) {
-            if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-        }
-
-        function v(e, t) {
-            for (var r = 0; r < t.length; r++) {
-                var n = t[r];
-                n.enumerable = n.enumerable || false;
-                n.configurable = true;
-                if ("value" in n) n.writable = true;
-                Object.defineProperty(e, n.key, n)
-            }
-        }
-
-        function l(e, t, r) {
-            if (t) v(e.prototype, t);
-            if (r) v(e, r);
-            Object.defineProperty(e, "prototype", {
-                writable: false
-            });
-            return e
-        }
-
-        function b(e, t, r, n, a, c, i) {
-            try {
-                var o = e[c](i);
-                var f = o.value
-            } catch (u) {
-                r(u);
-                return
-            }
-            if (o.done) t(f);
-            else Promise.resolve(f).then(n, a)
-        }
-
-        function h(e) {
-            return function() {
-                var t = this,
-                    r = arguments;
-                return new Promise((function(n, a) {
-                    var c = e.apply(t, r);
-
-                    function i(e) {
-                        b(c, n, a, i, o, "next", e)
-                    }
-
-                    function o(e) {
-                        b(c, n, a, i, o, "throw", e)
-                    }
-                    i(void 0)
-                }))
-            }
-        }(function() {
-            var e = h(regeneratorRuntime.mark((function e(t) {
-                var r, n, c, i;
-                return regeneratorRuntime.wrap((function e(o) {
-                    while (1) switch (o.prev = o.next) {
-                        case 0:
-                            r = t;
-                            n = "true";
-                            c = function() {
-                                function e() {
-                                    s(this, e);
-                                    this.mountStatus = false
-                                }
-                                l(e, [{
-                                    key: "mount",
-                                    value: function() {
-                                        var e = h(regeneratorRuntime.mark((function e() {
-                                            var t, r;
-                                            return regeneratorRuntime.wrap((function e(a) {
-                                                while (1) switch (a.prev = a.next) {
-                                                    case 0:
-                                                        t = this.mountStatus === n;
-                                                        if (!t) {
-                                                            a.next = 5;
-                                                            break
-                                                        }
-                                                        this.setNewMount(true);
-                                                        a.next = 14;
-                                                        break;
-                                                    case 5:
-                                                        this.mountStatus = true;
-                                                        a.next = 8;
-                                                        return this.checkLib();
-                                                    case 8:
-                                                        r = a.sent;
-                                                        if (!r) {
-                                                            a.next = 14;
-                                                            break
-                                                        }
-                                                        a.next = 12;
-                                                        return this.libHandle();
-                                                    case 12:
-                                                        this.checkNewMount();
-                                                        this.mountStatus = false;
-                                                    case 14:
-                                                    case "end":
-                                                        return a.stop()
-                                                }
-                                            }), e, this)
-                                        })));
-                                        return function t() {
-                                            return e.apply(this, arguments)
-                                        }
-                                    }()
-                                }, {
-                                    key: "checkLib",
-                                    value: function() {
-                                        var e = h(regeneratorRuntime.mark((function e() {
-                                            var t, n;
-                                            return regeneratorRuntime.wrap((function e(c) {
-                                                while (1) switch (c.prev = c.next) {
-                                                    case 0:
-                                                        t = false;
-                                                        if (!r[a["i"]]) r[a["i"]] = {};
-                                                        n = r[a["i"]].version;
-                                                        if (!n) {
-                                                            n = this.getLibVersion();
-                                                            r[a["i"]].version = n
-                                                        }
-                                                        c.prev = 4;
-                                                        c.next = 7;
-                                                        return Promise.all([this.checkCSS(n), this.checkScript(n)]);
-                                                    case 7:
-                                                        t = c.sent;
-                                                        c.next = 14;
-                                                        break;
-                                                    case 10:
-                                                        c.prev = 10;
-                                                        c.t0 = c["catch"](4);
-                                                        t = false;
-                                                        d["a"].error(c.t0);
-                                                    case 14:
-                                                        return c.abrupt("return", t);
-                                                    case 15:
-                                                    case "end":
-                                                        return c.stop()
-                                                }
-                                            }), e, this, [
-                                                [4, 10]
-                                            ])
-                                        })));
-                                        return function t() {
-                                            return e.apply(this, arguments)
-                                        }
-                                    }()
-                                }, {
-                                    key: "libHandle",
-                                    value: function() {
-                                        var e = h(regeneratorRuntime.mark((function e() {
-                                            var t, n, c, i, o;
-                                            return regeneratorRuntime.wrap((function e(f) {
-                                                while (1) switch (f.prev = f.next) {
-                                                    case 0:
-                                                        t = r[a["i"]] || {}, n = t.lib, c = t.isEventsInit, i = void 0 === c ? false : c;
-                                                        if (i) {
-                                                            f.next = 6;
-                                                            break
-                                                        }
-                                                        f.t0 = n;
-                                                        if (!f.t0) {
-                                                            f.next = 6;
-                                                            break
-                                                        }
-                                                        f.next = 6;
-                                                        return n.init();
-                                                    case 6:
-                                                        o = this.collectNodes();
-                                                        f.t1 = n;
-                                                        if (!f.t1) {
-                                                            f.next = 11;
-                                                            break
-                                                        }
-                                                        f.next = 11;
-                                                        return n.render(o);
-                                                    case 11:
-                                                    case "end":
-                                                        return f.stop()
-                                                }
-                                            }), e, this)
-                                        })));
-                                        return function t() {
-                                            return e.apply(this, arguments)
-                                        }
-                                    }()
-                                }, {
-                                    key: "collectNodes",
-                                    value: function e() {
-                                        var t = document.getElementsByClassName(a["h"]);
-                                        var r = [];
-                                        if (t.length) r = Array.prototype.filter.call(t, (function(e) {
-                                            var t = e.nodeName.toLowerCase() === a["k"];
-                                            var r = !e.id;
-                                            return t && r
-                                        }));
-                                        return r
-                                    }
-                                }, {
-                                    key: "getLibVersion",
-                                    value: function e() {
-                                        return a["d"]
-                                    }
-                                }, {
-                                    key: "checkCSS",
-                                    value: function e(t) {
-                                        return new Promise((function(e) {
-                                            var r = document.getElementById(a["b"]);
-                                            if (r) e(true);
-                                            else {
-                                                var n = document.createElement("link");
-                                                n.rel = "stylesheet";
-                                                n.type = "text/css";
-                                                n.id = a["b"];
-                                                n.href = "".concat(a["a"], "/").concat(a["e"]).concat(t, ".css");
-                                                document.head.appendChild(n);
-                                                n.onload = function() {
-                                                    e(true)
-                                                };
-                                                n.onerror = function(t) {
-                                                    d["a"].error(t);
-                                                    e(false)
-                                                }
-                                            }
-                                        }))
-                                    }
-                                }, {
-                                    key: "checkScript",
-                                    value: function e(t) {
-                                        return new Promise((function(e) {
-                                            var r = document.getElementById(a["c"]);
-                                            if (r) e(true);
-                                            else {
-                                                var n = document.createElement("script");
-                                                n.type = "text/javascript";
-                                                n.id = a["c"];
-                                                n.src = "".concat(a["a"], "/").concat(a["e"]).concat(t, ".js");
-                                                document.body.appendChild(n);
-                                                n.onload = function() {
-                                                    e(true)
-                                                };
-                                                n.onerror = function(t) {
-                                                    d["a"].error(t);
-                                                    e(false)
-                                                }
-                                            }
-                                        }))
-                                    }
-                                }, {
-                                    key: "checkNewMount",
-                                    value: function e() {
-                                        var t = u.getItem(a["g"]) || "";
-                                        var r = t === n;
-                                        if (r) {
-                                            this.mount();
-                                            this.setNewMount(false)
-                                        }
-                                    }
-                                }, {
-                                    key: "setNewMount",
-                                    value: function e() {
-                                        var t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "";
-                                        u.setItem(a["g"], t)
-                                    }
-                                }, {
-                                    key: "mountStatus",
-                                    set: function e() {
-                                        var t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "";
-                                        u.setItem(a["f"], t)
-                                    },
-                                    get: function e() {
-                                        return u.getItem(a["f"]) || ""
-                                    }
-                                }]);
-                                return e
-                            }();
-                            i = function() {
-                                var e = h(regeneratorRuntime.mark((function e() {
-                                    var t;
-                                    return regeneratorRuntime.wrap((function e(r) {
-                                        while (1) switch (r.prev = r.next) {
-                                            case 0:
-                                                t = new c;
-                                                r.next = 3;
-                                                return t.mount();
-                                            case 3:
-                                            case "end":
-                                                return r.stop()
-                                        }
-                                    }), e)
-                                })));
-                                return function t() {
-                                    return e.apply(this, arguments)
-                                }
-                            }();
-                            setTimeout(i, 0);
-                        case 5:
-                        case "end":
-                            return o.stop()
-                    }
-                }), e)
-            })));
-            return function t(r) {
-                return e.apply(this, arguments)
-            }
-        })()(window)
-    },
-    "32b716d95af2fd3c5c23": function(e, t, r) {
-        var n = r("0116c75136b233002fb9");
-        var a = r("621a65702ee1a566fd32")("toStringTag");
-        var c = "Arguments" == n(function() {
-            return arguments
-        }());
-        var i = function(e, t) {
-            try {
-                return e[t]
-            } catch (r) {}
-        };
-        e.exports = function(e) {
-            var t, r, o;
-            return void 0 === e ? "Undefined" : null === e ? "Null" : "string" == typeof(r = i(t = Object(e), a)) ? r : c ? n(t) : "Object" == (o = n(t)) && "function" == typeof t.callee ? "Arguments" : o
-        }
-    },
-    "340dbda6fe6f17098a91": function(e, t, r) {
-        "use strict";
-        var n = r("770f76c876afc046e4e0")(true);
-        r("429cfc8e3ed333e40618")(String, "String", (function(e) {
-            this._t = String(e);
-            this._i = 0
-        }), (function() {
-            var e = this._t;
-            var t = this._i;
-            var r;
-            if (t >= e.length) return {
-                value: void 0,
-                done: true
-            };
-            r = n(e, t);
-            this._i += r.length;
-            return {
-                value: r,
-                done: false
-            }
-        }))
-    },
-    "380c0734c088ca78ccda": function(e, t) {
-        e.exports = "constructor,hasOwnProperty,isPrototypeOf,propertyIsEnumerable,toLocaleString,toString,valueOf".split(",")
-    },
-    "3932316ffef991f5d157": function(e, t, r) {
-        "use strict";
-        var n = r("2d13d93c336705cd8ff9");
-        var a = r("ecd0e0fb36455021f082")(5);
-        var c = "find";
-        var i = true;
-        if (c in []) Array(1)[c]((function() {
-            i = false
-        }));
-        n(n.P + n.F * i, "Array", {
-            find: function e(t) {
-                return a(this, t, arguments.length > 1 ? arguments[1] : void 0)
-            }
-        });
-        r("a5e6f0092ff0290e0bcf")(c)
-    },
-    "3f2012daa60f226e86ec": function(e, t, r) {
-        "use strict";
-        var n = r("2d13d93c336705cd8ff9");
-        var a = r("8de492c765fbfb624515");
-        n(n.S + n.F * r("7a7739dd8a198a2cfcb5")((function() {
-            function e() {}
-            return !(Array.of.call(e) instanceof e)
-        })), "Array", {
-            of: function e() {
-                var t = 0;
-                var r = arguments.length;
-                var n = new("function" == typeof this ? this : Array)(r);
-                while (r > t) a(n, t, arguments[t++]);
-                n.length = r;
-                return n
-            }
-        })
-    },
-    "3fc8b4ca32b0aebd9ff3": function(e, t, r) {
-        "use strict";
-        var n = r("2d13d93c336705cd8ff9");
-        var a = r("ecd0e0fb36455021f082")(6);
-        var c = "findIndex";
-        var i = true;
-        if (c in []) Array(1)[c]((function() {
-            i = false
-        }));
-        n(n.P + n.F * i, "Array", {
-            findIndex: function e(t) {
-                return a(this, t, arguments.length > 1 ? arguments[1] : void 0)
-            }
-        });
-        r("a5e6f0092ff0290e0bcf")(c)
-    },
-    "3fe06cb9615786e0ea67": function(e, t, r) {
-        window.regeneratorRuntime = r("2c09af3fb5c4ba3698b3");
-        r("a6444c69152f1487917b");
-        if ("undefined" === typeof Promise) {
-            r("9fbadcf2c98d054f245e").enable();
-            window.Promise = r("e6615fafe8e11b81e37a")
-        }
-    },
-    "40b064d4eb439c0c1c2b": function(e, t, r) {
-        "use strict";
-        var n = r("7a7739dd8a198a2cfcb5");
-        e.exports = function(e, t) {
-            return !!e && n((function() {
-                t ? e.call(null, (function() {}), 1) : e.call(null)
-            }))
-        }
-    },
-    "40b8419e3e2132ef0a63": function(e) {
-        e.exports = {
-            name: "tiktok_embed",
-            version: "1.0.0",
-            embedVersion: "1.0.0",
-            description: "TikTok Embed SDK",
-            main: "index.js",
-            scripts: {
-                test: 'echo "Error: no test specified" && exit 1',
-                dev: "eden start",
-                build: "eden build",
-                "build:gcp": "NODE_REGION=GCP eden build",
-                "build:dev": "eden build -a",
-                commit: "eden push",
-                feature: "eden feature",
-                mr: "eden release -m",
-                lint: "eden-lint ./src --fix"
-            },
-            keywords: ["tiktok", "embed"],
-            author: "yangminghui.jasmine, chloe.chao",
-            license: "ISC",
-            devDependencies: {
-                "@ies/create-eden-config": "^1.0.2",
-                "@ies/eden-lint": "^2.15.4"
-            },
-            dependencies: {
-                "core-js": "2.5.7",
-                promise: "^8.0.3",
-                "regenerator-runtime": "^0.13.3"
-            },
-            husky: {
-                hooks: {
-                    "commit-msg": "commitlint .commitlintrc.js -E HUSKY_GIT_PARAMS",
-                    "pre-commit": "lint-staged"
-                }
-            },
-            "lint-staged": {
-                "*": ["eden lint format", "git add"]
-            }
-        }
-    },
-    "429cfc8e3ed333e40618": function(e, t, r) {
-        "use strict";
-        var n = r("46a1a30d151cac60057c");
-        var a = r("2d13d93c336705cd8ff9");
-        var c = r("88db22626e6c88b175cf");
-        var i = r("5f25c015bbbf9d42c661");
-        var o = r("224ae09e536c09e69a0a");
-        var f = r("5c5d334c57135891e397");
-        var u = r("62828dc3ffa96c06b7c9");
-        var d = r("12323e1413cbffdabe02");
-        var s = r("621a65702ee1a566fd32")("iterator");
-        var v = !([].keys && "next" in [].keys());
-        var l = "@@iterator";
-        var b = "keys";
-        var h = "values";
-        var p = function() {
-            return this
-        };
-        e.exports = function(e, t, r, y, m, g, w) {
-            f(r, t, y);
-            var x = function(e) {
-                if (!v && e in E) return E[e];
-                switch (e) {
-                    case b:
-                        return function t() {
-                            return new r(this, e)
-                        };
-                    case h:
-                        return function t() {
-                            return new r(this, e)
-                        }
-                }
-                return function t() {
-                    return new r(this, e)
-                }
-            };
-            var _ = t + " Iterator";
-            var k = m == h;
-            var j = false;
-            var E = e.prototype;
-            var S = E[s] || E[l] || m && E[m];
-            var O = S || x(m);
-            var A = m ? !k ? O : x("entries") : void 0;
-            var P = "Array" == t ? E.entries || S : S;
-            var I, T, L;
-            if (P) {
-                L = d(P.call(new e));
-                if (L !== Object.prototype && L.next) {
-                    u(L, _, true);
-                    if (!n && "function" != typeof L[s]) i(L, s, p)
-                }
-            }
-            if (k && S && S.name !== h) {
-                j = true;
-                O = function e() {
-                    return S.call(this)
-                }
-            }
-            if ((!n || w) && (v || j || !E[s])) i(E, s, O);
-            o[t] = O;
-            o[_] = p;
-            if (m) {
-                I = {
-                    values: k ? O : x(h),
-                    keys: g ? O : x(b),
-                    entries: A
-                };
-                if (w) {
-                    for (T in I)
-                        if (!(T in E)) c(E, T, I[T])
-                } else a(a.P + a.F * (v || j), t, I)
-            }
-            return I
-        }
-    },
-    "43382cd620aa5a0df057": function(e, t) {
-        var r;
-        r = function() {
-            return this
-        }();
-        try {
-            r = r || Function("return this")() || (1, eval)("this")
-        } catch (n) {
-            if ("object" === typeof window) r = window
-        }
-        e.exports = r
-    },
-    "4357234160788ed77205": function(e, t, r) {
-        var n = r("79c91dcd8cd554c59c7b");
-        e.exports = function(e, t, r, a) {
-            try {
-                return a ? t(n(r)[0], r[1]) : t(r)
-            } catch (i) {
-                var c = e["return"];
-                if (void 0 !== c) n(c.call(e));
-                throw i
-            }
-        }
-    },
-    "43a62b7f9a94dda95bf8": function(e, t, r) {
-        var n = r("5925dad3c5243ffee3db");
-        var a = r("1139de1233fd67f45bd7");
-        var c = "__core-js_shared__";
-        var i = a[c] || (a[c] = {});
-        (e.exports = function(e, t) {
-            return i[e] || (i[e] = void 0 !== t ? t : {})
-        })("versions", []).push({
-            version: n.version,
-            mode: r("46a1a30d151cac60057c") ? "pure" : "global",
-            copyright: "\xa9 2018 Denis Pushkarev (zloirock.ru)"
-        })
-    },
-    "46a1a30d151cac60057c": function(e, t) {
-        e.exports = false
-    },
-    "481c1f0e850b0c8d0f7d": function(e, t, r) {
-        "use strict";
-        var n = r("2d13d93c336705cd8ff9");
-        var a = r("1e0f00d296712713afe6");
-        n(n.P + n.F * !r("40b064d4eb439c0c1c2b")([].reduce, true), "Array", {
-            reduce: function e(t) {
-                return a(this, t, arguments.length, arguments[1], false)
-            }
-        })
-    },
-    "4cc77e026250beeef142": function(e, t, r) {
-        "use strict";
-        var n = r("2d13d93c336705cd8ff9");
-        var a = r("efae14a3f8cd9a616256");
-        var c = [].join;
-        n(n.P + n.F * (r("a537d0accb907bf9d41f") != Object || !r("40b064d4eb439c0c1c2b")(c)), "Array", {
-            join: function e(t) {
-                return c.call(a(this), void 0 === t ? "," : t)
-            }
-        })
-    },
-    "4d073e2fededcdd3f3d3": function(e, t) {
-        e.exports = function(e) {
-            if ("function" != typeof e) throw TypeError(e + " is not a function!");
-            return e
-        }
-    },
-    "4ef7a75a1d1957a7c5c0": function(e, t, r) {
-        var n = r("a459ab805827640a27e8");
-        e.exports = function(e, t) {
-            if (!n(e)) return e;
-            var r, a;
-            if (t && "function" == typeof(r = e.toString) && !n(a = r.call(e))) return a;
-            if ("function" == typeof(r = e.valueOf) && !n(a = r.call(e))) return a;
-            if (!t && "function" == typeof(r = e.toString) && !n(a = r.call(e))) return a;
-            throw TypeError("Can't convert object to primitive value")
-        }
-    },
-    "574ea81f94fc0b2f332a": function(e, t, r) {
-        var n = r("621a65702ee1a566fd32")("iterator");
-        var a = false;
-        try {
-            var c = [7][n]();
-            c["return"] = function() {
-                a = true
-            };
-            Array.from(c, (function() {
-                throw 2
-            }))
-        } catch (i) {}
-        e.exports = function(e, t) {
-            if (!t && !a) return false;
-            var r = false;
-            try {
-                var c = [7];
-                var o = c[n]();
-                o.next = function() {
-                    return {
-                        done: r = true
-                    }
-                };
-                c[n] = function() {
-                    return o
-                };
-                e(c)
-            } catch (i) {}
-            return r
-        }
-    },
-    "5925dad3c5243ffee3db": function(e, t) {
-        var r = e.exports = {
-            version: "2.5.7"
-        };
-        if ("number" == typeof __e) __e = r
-    },
-    "5975c7ea3ecd56e534e3": function(e, t, r) {
-        e.exports = !r("7a7739dd8a198a2cfcb5")((function() {
-            return 7 != Object.defineProperty({}, "a", {
-                get: function() {
-                    return 7
-                }
-            }).a
-        }))
-    },
-    "5b9dc0e027f5c68eff1a": function(e, t, r) {
-        var n = r("1139de1233fd67f45bd7").document;
-        e.exports = n && n.documentElement
-    },
-    "5baa1143f58e62614ca0": function(e, t, r) {
-        "use strict";
-        var n = r("2d13d93c336705cd8ff9");
-        var a = r("4d073e2fededcdd3f3d3");
-        var c = r("d394d0a4c1838202489d");
-        var i = r("7a7739dd8a198a2cfcb5");
-        var o = [].sort;
-        var f = [1, 2, 3];
-        n(n.P + n.F * (i((function() {
-            f.sort(void 0)
-        })) || !i((function() {
-            f.sort(null)
-        })) || !r("40b064d4eb439c0c1c2b")(o)), "Array", {
-            sort: function e(t) {
-                return void 0 === t ? o.call(c(this)) : o.call(c(this), a(t))
-            }
-        })
-    },
-    "5c5d334c57135891e397": function(e, t, r) {
-        "use strict";
-        var n = r("ef09ce044ac3210bc947");
-        var a = r("9d5592e83ab7f3d08974");
-        var c = r("62828dc3ffa96c06b7c9");
-        var i = {};
-        r("5f25c015bbbf9d42c661")(i, r("621a65702ee1a566fd32")("iterator"), (function() {
-            return this
-        }));
-        e.exports = function(e, t, r) {
-            e.prototype = n(i, {
-                next: a(1, r)
-            });
-            c(e, t + " Iterator")
-        }
-    },
-    "5f25c015bbbf9d42c661": function(e, t, r) {
-        var n = r("1b01d0e59d3af79760a0");
-        var a = r("9d5592e83ab7f3d08974");
-        e.exports = r("5975c7ea3ecd56e534e3") ? function(e, t, r) {
-            return n.f(e, t, a(1, r))
-        } : function(e, t, r) {
-            e[t] = r;
-            return e
-        }
-    },
-    "5f6eded14a8ed86276fc": function(e, t, r) {
-        var n = r("43a62b7f9a94dda95bf8")("keys");
-        var a = r("273d2eedcd369c189e70");
-        e.exports = function(e) {
-            return n[e] || (n[e] = a(e))
-        }
-    },
-    "621a65702ee1a566fd32": function(e, t, r) {
-        var n = r("43a62b7f9a94dda95bf8")("wks");
-        var a = r("273d2eedcd369c189e70");
-        var c = r("1139de1233fd67f45bd7").Symbol;
-        var i = "function" == typeof c;
-        var o = e.exports = function(e) {
-            return n[e] || (n[e] = i && c[e] || (i ? c : a)("Symbol." + e))
-        };
-        o.store = n
-    },
-    "62828dc3ffa96c06b7c9": function(e, t, r) {
-        var n = r("1b01d0e59d3af79760a0").f;
-        var a = r("d34390b928ecadc11dc8");
-        var c = r("621a65702ee1a566fd32")("toStringTag");
-        e.exports = function(e, t, r) {
-            if (e && !a(e = r ? e : e.prototype, c)) n(e, c, {
-                configurable: true,
-                value: t
-            })
-        }
-    },
-    "68a989d6f90923909f2a": function(e, t, r) {
-        var n = r("a459ab805827640a27e8");
-        var a = r("1139de1233fd67f45bd7").document;
-        var c = n(a) && n(a.createElement);
-        e.exports = function(e) {
-            return c ? a.createElement(e) : {}
-        }
-    },
-    "6ae9955278ddcf01bbfd": function(e, t, r) {
-        var n = r("a459ab805827640a27e8");
-        var a = r("8f648b1026e01323935b");
-        var c = r("621a65702ee1a566fd32")("species");
-        e.exports = function(e) {
-            var t;
-            if (a(e)) {
-                t = e.constructor;
-                if ("function" == typeof t && (t === Array || a(t.prototype))) t = void 0;
-                if (n(t)) {
-                    t = t[c];
-                    if (null === t) t = void 0
-                }
-            }
-            return void 0 === t ? Array : t
-        }
-    },
-    "71d3ec5bd65418e28ebc": function(e, t, r) {
-        var n = r("224ae09e536c09e69a0a");
-        var a = r("621a65702ee1a566fd32")("iterator");
-        var c = Array.prototype;
-        e.exports = function(e) {
-            return void 0 !== e && (n.Array === e || c[a] === e)
-        }
-    },
-    "74be682203e7c82cb4c9": function(e, t, r) {
-        r("89a21af31babcdc56725")("Array")
-    },
-    "770f76c876afc046e4e0": function(e, t, r) {
-        var n = r("1f3157d073736826d4fa");
-        var a = r("7ad2c0eb9a8edcc472a4");
-        e.exports = function(e) {
-            return function(t, r) {
-                var c = String(a(t));
-                var i = n(r);
-                var o = c.length;
-                var f, u;
-                if (i < 0 || i >= o) return e ? "" : void 0;
-                f = c.charCodeAt(i);
-                return f < 55296 || f > 56319 || i + 1 === o || (u = c.charCodeAt(i + 1)) < 56320 || u > 57343 ? e ? c.charAt(i) : f : e ? c.slice(i, i + 2) : (f - 55296 << 10) + (u - 56320) + 65536
-            }
-        }
-    },
-    "79c91dcd8cd554c59c7b": function(e, t, r) {
-        var n = r("a459ab805827640a27e8");
-        e.exports = function(e) {
-            if (!n(e)) throw TypeError(e + " is not an object!");
-            return e
-        }
-    },
-    "7a7739dd8a198a2cfcb5": function(e, t) {
-        e.exports = function(e) {
-            try {
-                return !!e()
-            } catch (t) {
-                return true
-            }
-        }
-    },
-    "7ad2c0eb9a8edcc472a4": function(e, t) {
-        e.exports = function(e) {
-            if (void 0 == e) throw TypeError("Can't call method on  " + e);
-            return e
-        }
-    },
-    "88db22626e6c88b175cf": function(e, t, r) {
-        var n = r("1139de1233fd67f45bd7");
-        var a = r("5f25c015bbbf9d42c661");
-        var c = r("d34390b928ecadc11dc8");
-        var i = r("273d2eedcd369c189e70")("src");
-        var o = "toString";
-        var f = Function[o];
-        var u = ("" + f).split(o);
-        r("5925dad3c5243ffee3db").inspectSource = function(e) {
-            return f.call(e)
-        };
-        (e.exports = function(e, t, r, o) {
-            var f = "function" == typeof r;
-            if (f) c(r, "name") || a(r, "name", t);
-            if (e[t] === r) return;
-            if (f) c(r, i) || a(r, i, e[t] ? "" + e[t] : u.join(String(t)));
-            if (e === n) e[t] = r;
-            else if (!o) {
-                delete e[t];
-                a(e, t, r)
-            } else if (e[t]) e[t] = r;
-            else a(e, t, r)
-        })(Function.prototype, o, (function e() {
-            return "function" == typeof this && this[i] || f.call(this)
-        }))
-    },
-    "896f33738142bf70015e": function(e, t, r) {
-        "use strict";
-        var n = r("2d13d93c336705cd8ff9");
-        var a = r("1e0f00d296712713afe6");
-        n(n.P + n.F * !r("40b064d4eb439c0c1c2b")([].reduceRight, true), "Array", {
-            reduceRight: function e(t) {
-                return a(this, t, arguments.length, arguments[1], true)
-            }
-        })
-    },
-    "89a21af31babcdc56725": function(e, t, r) {
-        "use strict";
-        var n = r("1139de1233fd67f45bd7");
-        var a = r("1b01d0e59d3af79760a0");
-        var c = r("5975c7ea3ecd56e534e3");
-        var i = r("621a65702ee1a566fd32")("species");
-        e.exports = function(e) {
-            var t = n[e];
-            if (c && t && !t[i]) a.f(t, i, {
-                configurable: true,
-                get: function() {
-                    return this
-                }
-            })
-        }
-    },
-    "8de492c765fbfb624515": function(e, t, r) {
-        "use strict";
-        var n = r("1b01d0e59d3af79760a0");
-        var a = r("9d5592e83ab7f3d08974");
-        e.exports = function(e, t, r) {
-            if (t in e) n.f(e, t, a(0, r));
-            else e[t] = r
-        }
-    },
-    "8f648b1026e01323935b": function(e, t, r) {
-        var n = r("0116c75136b233002fb9");
-        e.exports = Array.isArray || function e(t) {
-            return "Array" == n(t)
-        }
-    },
-    "9125d51ebaa93f49cfd5": function(e, t, r) {
-        "use strict";
-        var n = r("2d13d93c336705cd8ff9");
-        var a = r("ecd0e0fb36455021f082")(3);
-        n(n.P + n.F * !r("40b064d4eb439c0c1c2b")([].some, true), "Array", {
-            some: function e(t) {
-                return a(this, t, arguments[1])
-            }
-        })
-    },
-    "9d5592e83ab7f3d08974": function(e, t) {
-        e.exports = function(e, t) {
-            return {
-                enumerable: !(1 & e),
-                configurable: !(2 & e),
-                writable: !(4 & e),
-                value: t
-            }
-        }
-    },
-    "9fbadcf2c98d054f245e": function(e, t, r) {
-        "use strict";
-        var n = r("1b24b031f63a74d1f57f");
-        var a = [ReferenceError, TypeError, RangeError];
-        var c = false;
-        t.disable = i;
-
-        function i() {
-            c = false;
-            n._Y = null;
-            n._Z = null
-        }
-        t.enable = o;
-
-        function o(e) {
-            e = e || {};
-            if (c) i();
-            c = true;
-            var t = 0;
-            var r = 0;
-            var o = {};
-            n._Y = function(e) {
-                if (2 === e._V && o[e._1]) {
-                    if (o[e._1].logged) s(e._1);
-                    else clearTimeout(o[e._1].timeout);
-                    delete o[e._1]
-                }
-            };
-            n._Z = function(e, r) {
-                if (0 === e._U) {
-                    e._1 = t++;
-                    o[e._1] = {
-                        displayId: null,
-                        error: r,
-                        timeout: setTimeout(d.bind(null, e._1), u(r, a) ? 100 : 2e3),
-                        logged: false
-                    }
-                }
-            };
-
-            function d(t) {
-                if (e.allRejections || u(o[t].error, e.whitelist || a)) {
-                    o[t].displayId = r++;
-                    if (e.onUnhandled) {
-                        o[t].logged = true;
-                        e.onUnhandled(o[t].displayId, o[t].error)
-                    } else {
-                        o[t].logged = true;
-                        f(o[t].displayId, o[t].error)
-                    }
-                }
-            }
-
-            function s(t) {
-                if (o[t].logged)
-                    if (e.onHandled) e.onHandled(o[t].displayId, o[t].error);
-                    else if (!o[t].onUnhandled) {
-                    void 0;
-                    void 0
-                }
-            }
-        }
-
-        function f(e, t) {
-            void 0;
-            var r = (t && (t.stack || t)) + "";
-            r.split("\n").forEach((function(e) {
-                void 0
-            }))
-        }
-
-        function u(e, t) {
-            return t.some((function(t) {
-                return e instanceof t
-            }))
-        }
-    },
-    a459ab805827640a27e8: function(e, t) {
-        e.exports = function(e) {
-            return "object" === typeof e ? null !== e : "function" === typeof e
-        }
-    },
-    a537d0accb907bf9d41f: function(e, t, r) {
-        var n = r("0116c75136b233002fb9");
-        e.exports = Object("z").propertyIsEnumerable(0) ? Object : function(e) {
-            return "String" == n(e) ? e.split("") : Object(e)
-        }
-    },
-    a5e6f0092ff0290e0bcf: function(e, t, r) {
-        var n = r("621a65702ee1a566fd32")("unscopables");
-        var a = Array.prototype;
-        if (void 0 == a[n]) r("5f25c015bbbf9d42c661")(a, n, {});
-        e.exports = function(e) {
-            a[n][e] = true
-        }
-    },
-    a6444c69152f1487917b: function(e, t, r) {
-        r("340dbda6fe6f17098a91");
-        r("cff317ca62d09454b2d3");
-        r("0a5193b0534d54dbcda1");
-        r("3f2012daa60f226e86ec");
-        r("4cc77e026250beeef142");
-        r("1b71f5e96f29a92413b6");
-        r("5baa1143f58e62614ca0");
-        r("0f025c284bc567debf3d");
-        r("1591b90b4327c94245ad");
-        r("0565be87d109f51269ca");
-        r("9125d51ebaa93f49cfd5");
-        r("cf802dc5a6982c8247e6");
-        r("481c1f0e850b0c8d0f7d");
-        r("896f33738142bf70015e");
-        r("c9be824f185f52a1979a");
-        r("1468f5d37f30f63d76ea");
-        r("bc0f72eb2321587e4779");
-        r("fa5cd10f53a62f249502");
-        r("3932316ffef991f5d157");
-        r("3fc8b4ca32b0aebd9ff3");
-        r("74be682203e7c82cb4c9");
-        r("307014e72ed12da69e15");
-        e.exports = r("5925dad3c5243ffee3db").Array
-    },
-    a6d645856102faf17328: function(e, t, r) {
-        var n = r("1b01d0e59d3af79760a0");
-        var a = r("79c91dcd8cd554c59c7b");
-        var c = r("145c4f2bdc487b2578df");
-        e.exports = r("5975c7ea3ecd56e534e3") ? Object.defineProperties : function e(t, r) {
-            a(t);
-            var i = c(r);
-            var o = i.length;
-            var f = 0;
-            var u;
-            while (o > f) n.f(t, u = i[f++], r[u]);
-            return t
-        }
-    },
-    bc0f72eb2321587e4779: function(e, t, r) {
-        var n = r("2d13d93c336705cd8ff9");
-        n(n.P, "Array", {
-            copyWithin: r("06b2b473e53cc019ca74")
-        });
-        r("a5e6f0092ff0290e0bcf")("copyWithin")
-    },
-    bc1a333d2b6eceac22e3: function(e, t, r) {
-        e.exports = !r("5975c7ea3ecd56e534e3") && !r("7a7739dd8a198a2cfcb5")((function() {
-            return 7 != Object.defineProperty(r("68a989d6f90923909f2a")("div"), "a", {
-                get: function() {
-                    return 7
-                }
-            }).a
-        }))
-    },
-    c9be824f185f52a1979a: function(e, t, r) {
-        "use strict";
-        var n = r("2d13d93c336705cd8ff9");
-        var a = r("2076e982c14c41925fb4")(false);
-        var c = [].indexOf;
-        var i = !!c && 1 / [1].indexOf(1, -0) < 0;
-        n(n.P + n.F * (i || !r("40b064d4eb439c0c1c2b")(c)), "Array", {
-            indexOf: function e(t) {
-                return i ? c.apply(this, arguments) || 0 : a(this, t, arguments[1])
-            }
-        })
-    },
-    ca19e32ab6ee3b3692aa: function(e, t, r) {
-        var n = r("1f3157d073736826d4fa");
-        var a = Math.min;
-        e.exports = function(e) {
-            return e > 0 ? a(n(e), 9007199254740991) : 0
-        }
-    },
-    cf802dc5a6982c8247e6: function(e, t, r) {
-        "use strict";
-        var n = r("2d13d93c336705cd8ff9");
-        var a = r("ecd0e0fb36455021f082")(4);
-        n(n.P + n.F * !r("40b064d4eb439c0c1c2b")([].every, true), "Array", {
-            every: function e(t) {
-                return a(this, t, arguments[1])
-            }
-        })
-    },
-    cff317ca62d09454b2d3: function(e, t, r) {
-        var n = r("2d13d93c336705cd8ff9");
-        n(n.S, "Array", {
-            isArray: r("8f648b1026e01323935b")
-        })
-    },
-    d34390b928ecadc11dc8: function(e, t) {
-        var r = {}.hasOwnProperty;
-        e.exports = function(e, t) {
-            return r.call(e, t)
-        }
-    },
-    d394d0a4c1838202489d: function(e, t, r) {
-        var n = r("7ad2c0eb9a8edcc472a4");
-        e.exports = function(e) {
-            return Object(n(e))
-        }
-    },
-    dabaabbe8ba08d59975f: function(e, t) {
-        e.exports = function(e, t) {
-            return {
-                value: t,
-                done: !!e
-            }
-        }
-    },
-    e0b8897ffbf48a102fbb: function(e, t, r) {
-        "use strict";
-        r.d(t, "a", (function() {
-            return o
-        }));
-        r.d(t, "b", (function() {
-            return f
-        }));
-        r.d(t, "c", (function() {
-            return u
-        }));
-        r.d(t, "e", (function() {
-            return d
-        }));
-        r.d(t, "d", (function() {
-            return s
-        }));
-        r.d(t, "m", (function() {
-            return v
-        }));
-        r.d(t, "k", (function() {
-            return l
-        }));
-        r.d(t, "i", (function() {
-            return b
-        }));
-        r.d(t, "h", (function() {
-            return h
-        }));
-        r.d(t, "l", (function() {
-            return p
-        }));
-        r.d(t, "j", (function() {
-            return y
-        }));
-        r.d(t, "f", (function() {
-            return m
-        }));
-        r.d(t, "g", (function() {
-            return g
-        }));
-        var n = "production" !== "production";
-        var a = void 0 === "GCP";
-        var c = "https://lf16-tiktok-web.ttwstatic.com";
-        var i = a ? "/obj/tiktok-web-aiso/tiktok/falcon/embed" : "/obj/tiktok-web/tiktok/falcon/embed";
-        var o = n ? "http://127.0.0.1:4000" : "".concat(c).concat(i);
-        var f = "ttEmbedLibCSS";
-        var u = "ttEmbedLibScript";
-        var d = "embed_lib_v";
-        var s = r("40b8419e3e2132ef0a63").version;
-        var v = n ? "http://127.0.0.1:3000" : "https://www.tiktok.com";
-        var l = "blockquote";
-        var b = "tiktokEmbed";
-        var h = "tiktok-embed";
-        var p = "message";
-        var y = "__tt_embed__";
-        var m = "mounting";
-        var g = "newmount"
-    },
-    e3136eea77d23f8d97ec: function(e, t, r) {
-        var n = r("d34390b928ecadc11dc8");
-        var a = r("efae14a3f8cd9a616256");
-        var c = r("2076e982c14c41925fb4")(false);
-        var i = r("5f6eded14a8ed86276fc")("IE_PROTO");
-        e.exports = function(e, t) {
-            var r = a(e);
-            var o = 0;
-            var f = [];
-            var u;
-            for (u in r)
-                if (u != i) n(r, u) && f.push(u);
-            while (t.length > o)
-                if (n(r, u = t[o++])) ~c(f, u) || f.push(u);
-            return f
-        }
-    },
-    e6615fafe8e11b81e37a: function(e, t, r) {
-        "use strict";
-        var n = r("1b24b031f63a74d1f57f");
-        e.exports = n;
-        var a = d(true);
-        var c = d(false);
-        var i = d(null);
-        var o = d(void 0);
-        var f = d(0);
-        var u = d("");
-
-        function d(e) {
-            var t = new n(n._0);
-            t._V = 1;
-            t._W = e;
-            return t
-        }
-        n.resolve = function(e) {
-            if (e instanceof n) return e;
-            if (null === e) return i;
-            if (void 0 === e) return o;
-            if (true === e) return a;
-            if (false === e) return c;
-            if (0 === e) return f;
-            if ("" === e) return u;
-            if ("object" === typeof e || "function" === typeof e) try {
-                var t = e.then;
-                if ("function" === typeof t) return new n(t.bind(e))
-            } catch (r) {
-                return new n((function(e, t) {
-                    t(r)
-                }))
-            }
-            return d(e)
-        };
-        var s = function(e) {
-            if ("function" === typeof Array.from) {
-                s = Array.from;
-                return Array.from(e)
-            }
-            s = function(e) {
-                return Array.prototype.slice.call(e)
-            };
-            return Array.prototype.slice.call(e)
-        };
-        n.all = function(e) {
-            var t = s(e);
-            return new n((function(e, r) {
-                if (0 === t.length) return e([]);
-                var a = t.length;
-
-                function c(i, o) {
-                    if (o && ("object" === typeof o || "function" === typeof o))
-                        if (o instanceof n && o.then === n.prototype.then) {
-                            while (3 === o._V) o = o._W;
-                            if (1 === o._V) return c(i, o._W);
-                            if (2 === o._V) r(o._W);
-                            o.then((function(e) {
-                                c(i, e)
-                            }), r);
-                            return
-                        } else {
-                            var f = o.then;
-                            if ("function" === typeof f) {
-                                var u = new n(f.bind(o));
-                                u.then((function(e) {
-                                    c(i, e)
-                                }), r);
-                                return
-                            }
-                        } t[i] = o;
-                    if (0 === --a) e(t)
-                }
-                for (var i = 0; i < t.length; i++) c(i, t[i])
-            }))
-        };
-        n.reject = function(e) {
-            return new n((function(t, r) {
-                r(e)
-            }))
-        };
-        n.race = function(e) {
-            return new n((function(t, r) {
-                s(e).forEach((function(e) {
-                    n.resolve(e).then(t, r)
-                }))
-            }))
-        };
-        n.prototype["catch"] = function(e) {
-            return this.then(null, e)
-        }
-    },
-    ecd0e0fb36455021f082: function(e, t, r) {
-        var n = r("0e717e1f47872428608d");
-        var a = r("a537d0accb907bf9d41f");
-        var c = r("d394d0a4c1838202489d");
-        var i = r("ca19e32ab6ee3b3692aa");
-        var o = r("0594430ce9777a0767aa");
-        e.exports = function(e, t) {
-            var r = 1 == e;
-            var f = 2 == e;
-            var u = 3 == e;
-            var d = 4 == e;
-            var s = 6 == e;
-            var v = 5 == e || s;
-            var l = t || o;
-            return function(t, o, b) {
-                var h = c(t);
-                var p = a(h);
-                var y = n(o, b, 3);
-                var m = i(p.length);
-                var g = 0;
-                var w = r ? l(t, m) : f ? l(t, 0) : void 0;
-                var x, _;
-                for (; m > g; g++)
-                    if (v || g in p) {
-                        x = p[g];
-                        _ = y(x, g, h);
-                        if (e)
-                            if (r) w[g] = _;
-                            else if (_) switch (e) {
-                            case 3:
-                                return true;
-                            case 5:
-                                return x;
-                            case 6:
-                                return g;
-                            case 2:
-                                w.push(x)
-                        } else if (d) return false
-                    } return s ? -1 : u || d ? d : w
-            }
-        }
-    },
-    ef09ce044ac3210bc947: function(e, t, r) {
-        var n = r("79c91dcd8cd554c59c7b");
-        var a = r("a6d645856102faf17328");
-        var c = r("380c0734c088ca78ccda");
-        var i = r("5f6eded14a8ed86276fc")("IE_PROTO");
-        var o = function() {};
-        var f = "prototype";
-        var u = function() {
-            var e = r("68a989d6f90923909f2a")("iframe");
-            var t = c.length;
-            var n = "<";
-            var a = ">";
-            var i;
-            e.style.display = "none";
-            r("5b9dc0e027f5c68eff1a").appendChild(e);
-            e.src = "javascript:";
-            i = e.contentWindow.document;
-            i.open();
-            i.write(n + "script" + a + "document.F=Object" + n + "/script" + a);
-            i.close();
-            u = i.F;
-            while (t--) delete u[f][c[t]];
-            return u()
-        };
-        e.exports = Object.create || function e(t, r) {
-            var c;
-            if (null !== t) {
-                o[f] = n(t);
-                c = new o;
-                o[f] = null;
-                c[i] = t
-            } else c = u();
-            return void 0 === r ? c : a(c, r)
-        }
-    },
-    efae14a3f8cd9a616256: function(e, t, r) {
-        var n = r("a537d0accb907bf9d41f");
-        var a = r("7ad2c0eb9a8edcc472a4");
-        e.exports = function(e) {
-            return n(a(e))
-        }
-    },
-    f88518adc3004bf8d923: function(e, t, r) {
-        var n = r("32b716d95af2fd3c5c23");
-        var a = r("621a65702ee1a566fd32")("iterator");
-        var c = r("224ae09e536c09e69a0a");
-        e.exports = r("5925dad3c5243ffee3db").getIteratorMethod = function(e) {
-            if (void 0 != e) return e[a] || e["@@iterator"] || c[n(e)]
-        }
-    },
-    f8f08bdd917755ac017a: function(e, t, r) {
-        "use strict";
-        (function(t) {
-            e.exports = r;
-
-            function r(e) {
-                if (!n.length) {
-                    c();
-                    a = true
-                }
-                n[n.length] = e
-            }
-            var n = [];
-            var a = false;
-            var c;
-            var i = 0;
-            var o = 1024;
-
-            function f() {
-                while (i < n.length) {
-                    var e = i;
-                    i += 1;
-                    n[e].call();
-                    if (i > o) {
-                        for (var t = 0, r = n.length - i; t < r; t++) n[t] = n[t + i];
-                        n.length -= i;
-                        i = 0
-                    }
-                }
-                n.length = 0;
-                i = 0;
-                a = false
-            }
-            var u = "undefined" !== typeof t ? t : self;
-            var d = u.MutationObserver || u.WebKitMutationObserver;
-            if ("function" === typeof d) c = s(f);
-            else c = v(f);
-            r.requestFlush = c;
-
-            function s(e) {
-                var t = 1;
-                var r = new d(e);
-                var n = document.createTextNode("");
-                r.observe(n, {
-                    characterData: true
-                });
-                return function e() {
-                    t = -t;
-                    n.data = t
-                }
-            }
-
-            function v(e) {
-                return function t() {
-                    var r = setTimeout(a, 0);
-                    var n = setInterval(a, 50);
-
-                    function a() {
-                        clearTimeout(r);
-                        clearInterval(n);
-                        e()
-                    }
-                }
-            }
-            r.makeRequestCallFromTimer = v
-        }).call(this, r("43382cd620aa5a0df057"))
-    },
-    fa5cd10f53a62f249502: function(e, t, r) {
-        var n = r("2d13d93c336705cd8ff9");
-        n(n.P, "Array", {
-            fill: r("03192b087bb464f059c0")
-        });
-        r("a5e6f0092ff0290e0bcf")("fill")
-    }
+(function(e) {
+    var t = {};
+
+    function r(n) {
+        if (t[n]) return t[n].exports;
+        var a = t[n] = {
+            i: n,
+            l: false,
+            exports: {}
+        };
+        e[n].call(a.exports, a, a.exports, r);
+        a.l = true;
+        return a.exports
+    }
+    r.m = e;
+    r.c = t;
+    r.d = function(e, t, n) {
+        if (!r.o(e, t)) Object.defineProperty(e, t, {
+            enumerable: true,
+            get: n
+        })
+    };
+    r.r = function(e) {
+        if ("undefined" !== typeof Symbol && Symbol.toStringTag) Object.defineProperty(e, Symbol.toStringTag, {
+            value: "Module"
+        });
+        Object.defineProperty(e, "__esModule", {
+            value: true
+        })
+    };
+    r.t = function(e, t) {
+        if (1 & t) e = r(e);
+        if (8 & t) return e;
+        if (4 & t && "object" === typeof e && e && e.__esModule) return e;
+        var n = Object.create(null);
+        r.r(n);
+        Object.defineProperty(n, "default", {
+            enumerable: true,
+            value: e
+        });
+        if (2 & t && "string" != typeof e)
+            for (var a in e) r.d(n, a, function(t) {
+                return e[t]
+            }.bind(null, a));
+        return n
+    };
+    r.n = function(e) {
+        var t = e && e.__esModule ? function t() {
+            return e["default"]
+        } : function t() {
+            return e
+        };
+        r.d(t, "a", t);
+        return t
+    };
+    r.o = function(e, t) {
+        return Object.prototype.hasOwnProperty.call(e, t)
+    };
+    r.p = "/";
+    return r(r.s = 0)
+})({
+    0: function(e, t, r) {
+        r("3fe06cb9615786e0ea67");
+        e.exports = r("3177845424933048caec")
+    },
+    "0116c75136b233002fb9": function(e, t) {
+        var r = {}.toString;
+        e.exports = function(e) {
+            return r.call(e).slice(8, -1)
+        }
+    },
+    "03192b087bb464f059c0": function(e, t, r) {
+        "use strict";
+        var n = r("d394d0a4c1838202489d");
+        var a = r("23d432718b3e8ce32362");
+        var c = r("ca19e32ab6ee3b3692aa");
+        e.exports = function e(t) {
+            var r = n(this);
+            var o = c(r.length);
+            var i = arguments.length;
+            var f = a(i > 1 ? arguments[1] : void 0, o);
+            var u = i > 2 ? arguments[2] : void 0;
+            var d = void 0 === u ? o : a(u, o);
+            while (d > f) r[f++] = t;
+            return r
+        }
+    },
+    "0565be87d109f51269ca": function(e, t, r) {
+        "use strict";
+        var n = r("2d13d93c336705cd8ff9");
+        var a = r("ecd0e0fb36455021f082")(2);
+        n(n.P + n.F * !r("40b064d4eb439c0c1c2b")([].filter, true), "Array", {
+            filter: function e(t) {
+                return a(this, t, arguments[1])
+            }
+        })
+    },
+    "0594430ce9777a0767aa": function(e, t, r) {
+        var n = r("6ae9955278ddcf01bbfd");
+        e.exports = function(e, t) {
+            return new(n(e))(t)
+        }
+    },
+    "06b2b473e53cc019ca74": function(e, t, r) {
+        "use strict";
+        var n = r("d394d0a4c1838202489d");
+        var a = r("23d432718b3e8ce32362");
+        var c = r("ca19e32ab6ee3b3692aa");
+        e.exports = [].copyWithin || function e(t, r) {
+            var o = n(this);
+            var i = c(o.length);
+            var f = a(t, i);
+            var u = a(r, i);
+            var d = arguments.length > 2 ? arguments[2] : void 0;
+            var s = Math.min((void 0 === d ? i : a(d, i)) - u, i - f);
+            var v = 1;
+            if (u < f && f < u + s) {
+                v = -1;
+                u += s - 1;
+                f += s - 1
+            }
+            while (s-- > 0) {
+                if (u in o) o[f] = o[u];
+                else delete o[f];
+                f += v;
+                u += v
+            }
+            return o
+        }
+    },
+    "0a5193b0534d54dbcda1": function(e, t, r) {
+        "use strict";
+        var n = r("0e717e1f47872428608d");
+        var a = r("2d13d93c336705cd8ff9");
+        var c = r("d394d0a4c1838202489d");
+        var o = r("4357234160788ed77205");
+        var i = r("71d3ec5bd65418e28ebc");
+        var f = r("ca19e32ab6ee3b3692aa");
+        var u = r("8de492c765fbfb624515");
+        var d = r("f88518adc3004bf8d923");
+        a(a.S + a.F * !r("574ea81f94fc0b2f332a")((function(e) {
+            Array.from(e)
+        })), "Array", {
+            from: function e(t) {
+                var r = c(t);
+                var a = "function" == typeof this ? this : Array;
+                var s = arguments.length;
+                var v = s > 1 ? arguments[1] : void 0;
+                var l = void 0 !== v;
+                var b = 0;
+                var h = d(r);
+                var p, y, m, g;
+                if (l) v = n(v, s > 2 ? arguments[2] : void 0, 2);
+                if (void 0 != h && !(a == Array && i(h)))
+                    for (g = h.call(r), y = new a; !(m = g.next()).done; b++) u(y, b, l ? o(g, v, [m.value, b], true) : m.value);
+                else {
+                    p = f(r.length);
+                    for (y = new a(p); p > b; b++) u(y, b, l ? v(r[b], b) : r[b])
+                }
+                y.length = b;
+                return y
+            }
+        })
+    },
+    "0e717e1f47872428608d": function(e, t, r) {
+        var n = r("4d073e2fededcdd3f3d3");
+        e.exports = function(e, t, r) {
+            n(e);
+            if (void 0 === t) return e;
+            switch (r) {
+                case 1:
+                    return function(r) {
+                        return e.call(t, r)
+                    };
+                case 2:
+                    return function(r, n) {
+                        return e.call(t, r, n)
+                    };
+                case 3:
+                    return function(r, n, a) {
+                        return e.call(t, r, n, a)
+                    }
+            }
+            return function() {
+                return e.apply(t, arguments)
+            }
+        }
+    },
+    "0f025c284bc567debf3d": function(e, t, r) {
+        "use strict";
+        var n = r("2d13d93c336705cd8ff9");
+        var a = r("ecd0e0fb36455021f082")(0);
+        var c = r("40b064d4eb439c0c1c2b")([].forEach, true);
+        n(n.P + n.F * !c, "Array", {
+            forEach: function e(t) {
+                return a(this, t, arguments[1])
+            }
+        })
+    },
+    "1139de1233fd67f45bd7": function(e, t) {
+        var r = e.exports = "undefined" != typeof window && window.Math == Math ? window : "undefined" != typeof self && self.Math == Math ? self : Function("return this")();
+        if ("number" == typeof __g) __g = r
+    },
+    "12323e1413cbffdabe02": function(e, t, r) {
+        var n = r("d34390b928ecadc11dc8");
+        var a = r("d394d0a4c1838202489d");
+        var c = r("5f6eded14a8ed86276fc")("IE_PROTO");
+        var o = Object.prototype;
+        e.exports = Object.getPrototypeOf || function(e) {
+            e = a(e);
+            if (n(e, c)) return e[c];
+            if ("function" == typeof e.constructor && e instanceof e.constructor) return e.constructor.prototype;
+            return e instanceof Object ? o : null
+        }
+    },
+    "145c4f2bdc487b2578df": function(e, t, r) {
+        var n = r("e3136eea77d23f8d97ec");
+        var a = r("380c0734c088ca78ccda");
+        e.exports = Object.keys || function e(t) {
+            return n(t, a)
+        }
+    },
+    "1468f5d37f30f63d76ea": function(e, t, r) {
+        "use strict";
+        var n = r("2d13d93c336705cd8ff9");
+        var a = r("efae14a3f8cd9a616256");
+        var c = r("1f3157d073736826d4fa");
+        var o = r("ca19e32ab6ee3b3692aa");
+        var i = [].lastIndexOf;
+        var f = !!i && 1 / [1].lastIndexOf(1, -0) < 0;
+        n(n.P + n.F * (f || !r("40b064d4eb439c0c1c2b")(i)), "Array", {
+            lastIndexOf: function e(t) {
+                if (f) return i.apply(this, arguments) || 0;
+                var r = a(this);
+                var n = o(r.length);
+                var u = n - 1;
+                if (arguments.length > 1) u = Math.min(u, c(arguments[1]));
+                if (u < 0) u = n + u;
+                for (; u >= 0; u--)
+                    if (u in r)
+                        if (r[u] === t) return u || 0;
+                return -1
+            }
+        })
+    },
+    "1591b90b4327c94245ad": function(e, t, r) {
+        "use strict";
+        var n = r("2d13d93c336705cd8ff9");
+        var a = r("ecd0e0fb36455021f082")(1);
+        n(n.P + n.F * !r("40b064d4eb439c0c1c2b")([].map, true), "Array", {
+            map: function e(t) {
+                return a(this, t, arguments[1])
+            }
+        })
+    },
+    "1b01d0e59d3af79760a0": function(e, t, r) {
+        var n = r("79c91dcd8cd554c59c7b");
+        var a = r("bc1a333d2b6eceac22e3");
+        var c = r("4ef7a75a1d1957a7c5c0");
+        var o = Object.defineProperty;
+        t.f = r("5975c7ea3ecd56e534e3") ? Object.defineProperty : function e(t, r, i) {
+            n(t);
+            r = c(r, true);
+            n(i);
+            if (a) try {
+                return o(t, r, i)
+            } catch (f) {}
+            if ("get" in i || "set" in i) throw TypeError("Accessors not supported!");
+            if ("value" in i) t[r] = i.value;
+            return t
+        }
+    },
+    "1b24b031f63a74d1f57f": function(e, t, r) {
+        "use strict";
+        var n = r("f8f08bdd917755ac017a");
+
+        function a() {}
+        var c = null;
+        var o = {};
+
+        function i(e) {
+            try {
+                return e.then
+            } catch (t) {
+                c = t;
+                return o
+            }
+        }
+
+        function f(e, t) {
+            try {
+                return e(t)
+            } catch (r) {
+                c = r;
+                return o
+            }
+        }
+
+        function u(e, t, r) {
+            try {
+                e(t, r)
+            } catch (n) {
+                c = n;
+                return o
+            }
+        }
+        e.exports = d;
+
+        function d(e) {
+            if ("object" !== typeof this) throw new TypeError("Promises must be constructed via new");
+            if ("function" !== typeof e) throw new TypeError("Promise constructor's argument is not a function");
+            this._U = 0;
+            this._V = 0;
+            this._W = null;
+            this._X = null;
+            if (e === a) return;
+            m(e, this)
+        }
+        d._Y = null;
+        d._Z = null;
+        d._0 = a;
+        d.prototype.then = function(e, t) {
+            if (this.constructor !== d) return s(this, e, t);
+            var r = new d(a);
+            v(this, new y(e, t, r));
+            return r
+        };
+
+        function s(e, t, r) {
+            return new e.constructor((function(n, c) {
+                var o = new d(a);
+                o.then(n, c);
+                v(e, new y(t, r, o))
+            }))
+        }
+
+        function v(e, t) {
+            while (3 === e._V) e = e._W;
+            if (d._Y) d._Y(e);
+            if (0 === e._V) {
+                if (0 === e._U) {
+                    e._U = 1;
+                    e._X = t;
+                    return
+                }
+                if (1 === e._U) {
+                    e._U = 2;
+                    e._X = [e._X, t];
+                    return
+                }
+                e._X.push(t);
+                return
+            }
+            l(e, t)
+        }
+
+        function l(e, t) {
+            n((function() {
+                var r = 1 === e._V ? t.onFulfilled : t.onRejected;
+                if (null === r) {
+                    if (1 === e._V) b(t.promise, e._W);
+                    else h(t.promise, e._W);
+                    return
+                }
+                var n = f(r, e._W);
+                if (n === o) h(t.promise, c);
+                else b(t.promise, n)
+            }))
+        }
+
+        function b(e, t) {
+            if (t === e) return h(e, new TypeError("A promise cannot be resolved with itself."));
+            if (t && ("object" === typeof t || "function" === typeof t)) {
+                var r = i(t);
+                if (r === o) return h(e, c);
+                if (r === e.then && t instanceof d) {
+                    e._V = 3;
+                    e._W = t;
+                    p(e);
+                    return
+                } else if ("function" === typeof r) {
+                    m(r.bind(t), e);
+                    return
+                }
+            }
+            e._V = 1;
+            e._W = t;
+            p(e)
+        }
+
+        function h(e, t) {
+            e._V = 2;
+            e._W = t;
+            if (d._Z) d._Z(e, t);
+            p(e)
+        }
+
+        function p(e) {
+            if (1 === e._U) {
+                v(e, e._X);
+                e._X = null
+            }
+            if (2 === e._U) {
+                for (var t = 0; t < e._X.length; t++) v(e, e._X[t]);
+                e._X = null
+            }
+        }
+
+        function y(e, t, r) {
+            this.onFulfilled = "function" === typeof e ? e : null;
+            this.onRejected = "function" === typeof t ? t : null;
+            this.promise = r
+        }
+
+        function m(e, t) {
+            var r = false;
+            var n = u(e, (function(e) {
+                if (r) return;
+                r = true;
+                b(t, e)
+            }), (function(e) {
+                if (r) return;
+                r = true;
+                h(t, e)
+            }));
+            if (!r && n === o) {
+                r = true;
+                h(t, c)
+            }
+        }
+    },
+    "1b71f5e96f29a92413b6": function(e, t, r) {
+        "use strict";
+        var n = r("2d13d93c336705cd8ff9");
+        var a = r("5b9dc0e027f5c68eff1a");
+        var c = r("0116c75136b233002fb9");
+        var o = r("23d432718b3e8ce32362");
+        var i = r("ca19e32ab6ee3b3692aa");
+        var f = [].slice;
+        n(n.P + n.F * r("7a7739dd8a198a2cfcb5")((function() {
+            if (a) f.call(a)
+        })), "Array", {
+            slice: function e(t, r) {
+                var n = i(this.length);
+                var a = c(this);
+                r = void 0 === r ? n : r;
+                if ("Array" == a) return f.call(this, t, r);
+                var u = o(t, n);
+                var d = o(r, n);
+                var s = i(d - u);
+                var v = new Array(s);
+                var l = 0;
+                for (; l < s; l++) v[l] = "String" == a ? this.charAt(u + l) : this[u + l];
+                return v
+            }
+        })
+    },
+    "1e0f00d296712713afe6": function(e, t, r) {
+        var n = r("4d073e2fededcdd3f3d3");
+        var a = r("d394d0a4c1838202489d");
+        var c = r("a537d0accb907bf9d41f");
+        var o = r("ca19e32ab6ee3b3692aa");
+        e.exports = function(e, t, r, i, f) {
+            n(t);
+            var u = a(e);
+            var d = c(u);
+            var s = o(u.length);
+            var v = f ? s - 1 : 0;
+            var l = f ? -1 : 1;
+            if (r < 2)
+                for (;;) {
+                    if (v in d) {
+                        i = d[v];
+                        v += l;
+                        break
+                    }
+                    v += l;
+                    if (f ? v < 0 : s <= v) throw TypeError("Reduce of empty array with no initial value")
+                }
+            for (; f ? v >= 0 : s > v; v += l)
+                if (v in d) i = t(i, d[v], v, u);
+            return i
+        }
+    },
+    "1f3157d073736826d4fa": function(e, t) {
+        var r = Math.ceil;
+        var n = Math.floor;
+        e.exports = function(e) {
+            return isNaN(e = +e) ? 0 : (e > 0 ? n : r)(e)
+        }
+    },
+    "2076e982c14c41925fb4": function(e, t, r) {
+        var n = r("efae14a3f8cd9a616256");
+        var a = r("ca19e32ab6ee3b3692aa");
+        var c = r("23d432718b3e8ce32362");
+        e.exports = function(e) {
+            return function(t, r, o) {
+                var i = n(t);
+                var f = a(i.length);
+                var u = c(o, f);
+                var d;
+                if (e && r != r)
+                    while (f > u) {
+                        d = i[u++];
+                        if (d != d) return true
+                    } else
+                        for (; f > u; u++)
+                            if (e || u in i)
+                                if (i[u] === r) return e || u || 0;
+                return !e && -1
+            }
+        }
+    },
+    "224ae09e536c09e69a0a": function(e, t) {
+        e.exports = {}
+    },
+    "23617503340803072f22": function(e, t, r) {
+        "use strict";
+        r.d(t, "b", (function() {
+            return o
+        }));
+        r.d(t, "d", (function() {
+            return i
+        }));
+        r.d(t, "a", (function() {
+            return v
+        }));
+        r.d(t, "c", (function() {
+            return l
+        }));
+
+        function n(e, t, r, n, a, c, o) {
+            try {
+                var i = e[c](o);
+                var f = i.value
+            } catch (u) {
+                r(u);
+                return
+            }
+            if (i.done) t(f);
+            else Promise.resolve(f).then(n, a)
+        }
+
+        function a(e) {
+            return function() {
+                var t = this,
+                    r = arguments;
+                return new Promise((function(a, c) {
+                    var o = e.apply(t, r);
+
+                    function i(e) {
+                        n(o, a, c, i, f, "next", e)
+                    }
+
+                    function f(e) {
+                        n(o, a, c, i, f, "throw", e)
+                    }
+                    i(void 0)
+                }))
+            }
+        }
+
+        function c(e) {
+            "@babel/helpers - typeof";
+            return c = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+                return typeof e
+            } : function(e) {
+                return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
+            }, c(e)
+        }
+
+        function o() {
+            return Math.round(1e17 * Math.random())
+        }
+
+        function i() {
+            var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : [];
+            var t = arguments.length > 1 ? arguments[1] : void 0;
+            var r = arguments.length > 2 ? arguments[2] : void 0;
+            if (!e.length || !t) return [];
+            return e.reduce((function() {
+                var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : [];
+                var n = arguments.length > 1 ? arguments[1] : void 0;
+                var a = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : 0;
+                var c = Math.floor(a / t);
+                if (!e[c]) e[c] = [];
+                if (r) e[c].push(n[r]);
+                else e[c].push(n);
+                return e
+            }), [])
+        }
+
+        function f(e, t) {
+            var r = t.type || "GET";
+            var n = t.data;
+            var a = t.success,
+                o = void 0 === a ? function e(t, r) {
+                    void 0
+                } : a,
+                i = t.fail,
+                f = void 0 === i ? function e(t, r) {
+                    void 0
+                } : i;
+            var u = new XMLHttpRequest;
+            u.onreadystatechange = function() {
+                if (4 === Number(u.readyState))
+                    if (u.status >= 200 && u.status < 300 || 304 === u.status) o(u.responseText, u);
+                    else f(u.responseText, u)
+            };
+
+            function d(e) {
+                var t = e;
+                var r = [];
+                if ("string" === typeof t) t = encodeURI(t);
+                else if ("object" === c(t)) {
+                    Object.keys(t).forEach((function(e) {
+                        r.push("".concat(e, "=").concat(encodeURIComponent(t[e].toString())))
+                    }));
+                    t = r.join("&")
+                }
+                return t
+            }
+            if ("GET" === r.toUpperCase()) {
+                var s = "".concat(e, "?").concat(d(n || ""));
+                u.open("get", s, true);
+                u.send(null)
+            } else if ("POST" === r.toUpperCase()) {
+                u.open("post", e, true);
+                u.setRequestHeader("Content-Type", "application/x-www-form-urlencoded");
+                u.send(d(n || ""))
+            }
+        }
+
+        function u(e, t) {
+            return d.apply(this, arguments)
+        }
+
+        function d() {
+            d = a(regeneratorRuntime.mark((function e(t, r) {
+                return regeneratorRuntime.wrap((function e(n) {
+                    while (1) switch (n.prev = n.next) {
+                        case 0:
+                            return n.abrupt("return", new Promise((function(e, n) {
+                                var a = {
+                                    data: r,
+                                    success: e,
+                                    fail: n
+                                };
+                                f(t, a)
+                            })).then((function() {
+                                var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "{}";
+                                var t = {};
+                                try {
+                                    t = JSON.parse(e)
+                                } catch (r) {
+                                    t = {}
+                                }
+                                return t
+                            })));
+                        case 1:
+                        case "end":
+                            return n.stop()
+                    }
+                }), e)
+            })));
+            return d.apply(this, arguments)
+        }
+
+        function s() {
+            var e = "TikTok";
+            var t = {};
+            var r = function t(r) {
+                return "[".concat(e, "] ").concat(r.toString())
+            };
+            ["error", "log", "info"].forEach((function(e) {
+                t[e] = function(t) {
+                    if ("info" === e) void 0;
+                    else void 0
+                }
+            }));
+            return t
+        }
+        var v = s();
+
+        function l(e) {
+            var t = e.replace(/[\[]/, "\\[").replace(/[\]]/, "\\]");
+            var r = new RegExp("[\\?&]".concat(t, "=([^&#]*)"));
+            var n = r.exec(location.search);
+            return null === n ? "" : decodeURIComponent(n[1].replace(/\+/g, " "))
+        }
+
+        function b() {
+            return false || "production" === "dev"
+        }
+    },
+    "23d432718b3e8ce32362": function(e, t, r) {
+        var n = r("1f3157d073736826d4fa");
+        var a = Math.max;
+        var c = Math.min;
+        e.exports = function(e, t) {
+            e = n(e);
+            return e < 0 ? a(e + t, 0) : c(e, t)
+        }
+    },
+    "273d2eedcd369c189e70": function(e, t) {
+        var r = 0;
+        var n = Math.random();
+        e.exports = function(e) {
+            return "Symbol(".concat(void 0 === e ? "" : e, ")_", (++r + n).toString(36))
+        }
+    },
+    "2c09af3fb5c4ba3698b3": function(e, t, r) {
+        var n = function(e) {
+            "use strict";
+            var t = Object.prototype;
+            var r = t.hasOwnProperty;
+            var n;
+            var a = "function" === typeof Symbol ? Symbol : {};
+            var c = a.iterator || "@@iterator";
+            var o = a.asyncIterator || "@@asyncIterator";
+            var i = a.toStringTag || "@@toStringTag";
+
+            function f(e, t, r, n) {
+                var a = t && t.prototype instanceof h ? t : h;
+                var c = Object.create(a.prototype);
+                var o = new O(n || []);
+                c._invoke = j(e, r, o);
+                return c
+            }
+            e.wrap = f;
+
+            function u(e, t, r) {
+                try {
+                    return {
+                        type: "normal",
+                        arg: e.call(t, r)
+                    }
+                } catch (n) {
+                    return {
+                        type: "throw",
+                        arg: n
+                    }
+                }
+            }
+            var d = "suspendedStart";
+            var s = "suspendedYield";
+            var v = "executing";
+            var l = "completed";
+            var b = {};
+
+            function h() {}
+
+            function p() {}
+
+            function y() {}
+            var m = {};
+            m[c] = function() {
+                return this
+            };
+            var g = Object.getPrototypeOf;
+            var w = g && g(g(P([])));
+            if (w && w !== t && r.call(w, c)) m = w;
+            var x = y.prototype = h.prototype = Object.create(m);
+            p.prototype = x.constructor = y;
+            y.constructor = p;
+            y[i] = p.displayName = "GeneratorFunction";
+
+            function _(e) {
+                ["next", "throw", "return"].forEach((function(t) {
+                    e[t] = function(e) {
+                        return this._invoke(t, e)
+                    }
+                }))
+            }
+            e.isGeneratorFunction = function(e) {
+                var t = "function" === typeof e && e.constructor;
+                return t ? t === p || "GeneratorFunction" === (t.displayName || t.name) : false
+            };
+            e.mark = function(e) {
+                if (Object.setPrototypeOf) Object.setPrototypeOf(e, y);
+                else {
+                    e.__proto__ = y;
+                    if (!(i in e)) e[i] = "GeneratorFunction"
+                }
+                e.prototype = Object.create(x);
+                return e
+            };
+            e.awrap = function(e) {
+                return {
+                    __await: e
+                }
+            };
+
+            function k(e, t) {
+                function n(a, c, o, i) {
+                    var f = u(e[a], e, c);
+                    if ("throw" === f.type) i(f.arg);
+                    else {
+                        var d = f.arg;
+                        var s = d.value;
+                        if (s && "object" === typeof s && r.call(s, "__await")) return t.resolve(s.__await).then((function(e) {
+                            n("next", e, o, i)
+                        }), (function(e) {
+                            n("throw", e, o, i)
+                        }));
+                        return t.resolve(s).then((function(e) {
+                            d.value = e;
+                            o(d)
+                        }), (function(e) {
+                            return n("throw", e, o, i)
+                        }))
+                    }
+                }
+                var a;
+
+                function c(e, r) {
+                    function c() {
+                        return new t((function(t, a) {
+                            n(e, r, t, a)
+                        }))
+                    }
+                    return a = a ? a.then(c, c) : c()
+                }
+                this._invoke = c
+            }
+            _(k.prototype);
+            k.prototype[o] = function() {
+                return this
+            };
+            e.AsyncIterator = k;
+            e.async = function(t, r, n, a, c) {
+                if (void 0 === c) c = Promise;
+                var o = new k(f(t, r, n, a), c);
+                return e.isGeneratorFunction(r) ? o : o.next().then((function(e) {
+                    return e.done ? e.value : o.next()
+                }))
+            };
+
+            function j(e, t, r) {
+                var n = d;
+                return function a(c, o) {
+                    if (n === v) throw new Error("Generator is already running");
+                    if (n === l) {
+                        if ("throw" === c) throw o;
+                        return T()
+                    }
+                    r.method = c;
+                    r.arg = o;
+                    while (true) {
+                        var i = r.delegate;
+                        if (i) {
+                            var f = A(i, r);
+                            if (f) {
+                                if (f === b) continue;
+                                return f
+                            }
+                        }
+                        if ("next" === r.method) r.sent = r._sent = r.arg;
+                        else if ("throw" === r.method) {
+                            if (n === d) {
+                                n = l;
+                                throw r.arg
+                            }
+                            r.dispatchException(r.arg)
+                        } else if ("return" === r.method) r.abrupt("return", r.arg);
+                        n = v;
+                        var h = u(e, t, r);
+                        if ("normal" === h.type) {
+                            n = r.done ? l : s;
+                            if (h.arg === b) continue;
+                            return {
+                                value: h.arg,
+                                done: r.done
+                            }
+                        } else if ("throw" === h.type) {
+                            n = l;
+                            r.method = "throw";
+                            r.arg = h.arg
+                        }
+                    }
+                }
+            }
+
+            function A(e, t) {
+                var r = e.iterator[t.method];
+                if (r === n) {
+                    t.delegate = null;
+                    if ("throw" === t.method) {
+                        if (e.iterator["return"]) {
+                            t.method = "return";
+                            t.arg = n;
+                            A(e, t);
+                            if ("throw" === t.method) return b
+                        }
+                        t.method = "throw";
+                        t.arg = new TypeError("The iterator does not provide a 'throw' method")
+                    }
+                    return b
+                }
+                var a = u(r, e.iterator, t.arg);
+                if ("throw" === a.type) {
+                    t.method = "throw";
+                    t.arg = a.arg;
+                    t.delegate = null;
+                    return b
+                }
+                var c = a.arg;
+                if (!c) {
+                    t.method = "throw";
+                    t.arg = new TypeError("iterator result is not an object");
+                    t.delegate = null;
+                    return b
+                }
+                if (c.done) {
+                    t[e.resultName] = c.value;
+                    t.next = e.nextLoc;
+                    if ("return" !== t.method) {
+                        t.method = "next";
+                        t.arg = n
+                    }
+                } else return c;
+                t.delegate = null;
+                return b
+            }
+            _(x);
+            x[i] = "Generator";
+            x[c] = function() {
+                return this
+            };
+            x.toString = function() {
+                return "[object Generator]"
+            };
+
+            function E(e) {
+                var t = {
+                    tryLoc: e[0]
+                };
+                if (1 in e) t.catchLoc = e[1];
+                if (2 in e) {
+                    t.finallyLoc = e[2];
+                    t.afterLoc = e[3]
+                }
+                this.tryEntries.push(t)
+            }
+
+            function S(e) {
+                var t = e.completion || {};
+                t.type = "normal";
+                delete t.arg;
+                e.completion = t
+            }
+
+            function O(e) {
+                this.tryEntries = [{
+                    tryLoc: "root"
+                }];
+                e.forEach(E, this);
+                this.reset(true)
+            }
+            e.keys = function(e) {
+                var t = [];
+                for (var r in e) t.push(r);
+                t.reverse();
+                return function r() {
+                    while (t.length) {
+                        var n = t.pop();
+                        if (n in e) {
+                            r.value = n;
+                            r.done = false;
+                            return r
+                        }
+                    }
+                    r.done = true;
+                    return r
+                }
+            };
+
+            function P(e) {
+                if (e) {
+                    var t = e[c];
+                    if (t) return t.call(e);
+                    if ("function" === typeof e.next) return e;
+                    if (!isNaN(e.length)) {
+                        var a = -1,
+                            o = function t() {
+                                while (++a < e.length)
+                                    if (r.call(e, a)) {
+                                        t.value = e[a];
+                                        t.done = false;
+                                        return t
+                                    } t.value = n;
+                                t.done = true;
+                                return t
+                            };
+                        return o.next = o
+                    }
+                }
+                return {
+                    next: T
+                }
+            }
+            e.values = P;
+
+            function T() {
+                return {
+                    value: n,
+                    done: true
+                }
+            }
+            O.prototype = {
+                constructor: O,
+                reset: function(e) {
+                    this.prev = 0;
+                    this.next = 0;
+                    this.sent = this._sent = n;
+                    this.done = false;
+                    this.delegate = null;
+                    this.method = "next";
+                    this.arg = n;
+                    this.tryEntries.forEach(S);
+                    if (!e)
+                        for (var t in this)
+                            if ("t" === t.charAt(0) && r.call(this, t) && !isNaN(+t.slice(1))) this[t] = n
+                },
+                stop: function() {
+                    this.done = true;
+                    var e = this.tryEntries[0];
+                    var t = e.completion;
+                    if ("throw" === t.type) throw t.arg;
+                    return this.rval
+                },
+                dispatchException: function(e) {
+                    if (this.done) throw e;
+                    var t = this;
+
+                    function a(r, a) {
+                        i.type = "throw";
+                        i.arg = e;
+                        t.next = r;
+                        if (a) {
+                            t.method = "next";
+                            t.arg = n
+                        }
+                        return !!a
+                    }
+                    for (var c = this.tryEntries.length - 1; c >= 0; --c) {
+                        var o = this.tryEntries[c];
+                        var i = o.completion;
+                        if ("root" === o.tryLoc) return a("end");
+                        if (o.tryLoc <= this.prev) {
+                            var f = r.call(o, "catchLoc");
+                            var u = r.call(o, "finallyLoc");
+                            if (f && u) {
+                                if (this.prev < o.catchLoc) return a(o.catchLoc, true);
+                                else if (this.prev < o.finallyLoc) return a(o.finallyLoc)
+                            } else if (f) {
+                                if (this.prev < o.catchLoc) return a(o.catchLoc, true)
+                            } else if (u) {
+                                if (this.prev < o.finallyLoc) return a(o.finallyLoc)
+                            } else throw new Error("try statement without catch or finally")
+                        }
+                    }
+                },
+                abrupt: function(e, t) {
+                    for (var n = this.tryEntries.length - 1; n >= 0; --n) {
+                        var a = this.tryEntries[n];
+                        if (a.tryLoc <= this.prev && r.call(a, "finallyLoc") && this.prev < a.finallyLoc) {
+                            var c = a;
+                            break
+                        }
+                    }
+                    if (c && ("break" === e || "continue" === e) && c.tryLoc <= t && t <= c.finallyLoc) c = null;
+                    var o = c ? c.completion : {};
+                    o.type = e;
+                    o.arg = t;
+                    if (c) {
+                        this.method = "next";
+                        this.next = c.finallyLoc;
+                        return b
+                    }
+                    return this.complete(o)
+                },
+                complete: function(e, t) {
+                    if ("throw" === e.type) throw e.arg;
+                    if ("break" === e.type || "continue" === e.type) this.next = e.arg;
+                    else if ("return" === e.type) {
+                        this.rval = this.arg = e.arg;
+                        this.method = "return";
+                        this.next = "end"
+                    } else if ("normal" === e.type && t) this.next = t;
+                    return b
+                },
+                finish: function(e) {
+                    for (var t = this.tryEntries.length - 1; t >= 0; --t) {
+                        var r = this.tryEntries[t];
+                        if (r.finallyLoc === e) {
+                            this.complete(r.completion, r.afterLoc);
+                            S(r);
+                            return b
+                        }
+                    }
+                },
+                catch: function(e) {
+                    for (var t = this.tryEntries.length - 1; t >= 0; --t) {
+                        var r = this.tryEntries[t];
+                        if (r.tryLoc === e) {
+                            var n = r.completion;
+                            if ("throw" === n.type) {
+                                var a = n.arg;
+                                S(r)
+                            }
+                            return a
+                        }
+                    }
+                    throw new Error("illegal catch attempt")
+                },
+                delegateYield: function(e, t, r) {
+                    this.delegate = {
+                        iterator: P(e),
+                        resultName: t,
+                        nextLoc: r
+                    };
+                    if ("next" === this.method) this.arg = n;
+                    return b
+                }
+            };
+            return e
+        }(true ? e.exports : void 0);
+        try {
+            regeneratorRuntime = n
+        } catch (a) {
+            Function("r", "regeneratorRuntime = r")(n)
+        }
+    },
+    "2d13d93c336705cd8ff9": function(e, t, r) {
+        var n = r("1139de1233fd67f45bd7");
+        var a = r("5925dad3c5243ffee3db");
+        var c = r("5f25c015bbbf9d42c661");
+        var o = r("88db22626e6c88b175cf");
+        var i = r("0e717e1f47872428608d");
+        var f = "prototype";
+        var u = function(e, t, r) {
+            var d = e & u.F;
+            var s = e & u.G;
+            var v = e & u.S;
+            var l = e & u.P;
+            var b = e & u.B;
+            var h = s ? n : v ? n[t] || (n[t] = {}) : (n[t] || {})[f];
+            var p = s ? a : a[t] || (a[t] = {});
+            var y = p[f] || (p[f] = {});
+            var m, g, w, x;
+            if (s) r = t;
+            for (m in r) {
+                g = !d && h && void 0 !== h[m];
+                w = (g ? h : r)[m];
+                x = b && g ? i(w, n) : l && "function" == typeof w ? i(Function.call, w) : w;
+                if (h) o(h, m, w, e & u.U);
+                if (p[m] != w) c(p, m, x);
+                if (l && y[m] != w) y[m] = w
+            }
+        };
+        n.core = a;
+        u.F = 1;
+        u.G = 2;
+        u.S = 4;
+        u.P = 8;
+        u.B = 16;
+        u.W = 32;
+        u.U = 64;
+        u.R = 128;
+        e.exports = u
+    },
+    "307014e72ed12da69e15": function(e, t, r) {
+        "use strict";
+        var n = r("a5e6f0092ff0290e0bcf");
+        var a = r("dabaabbe8ba08d59975f");
+        var c = r("224ae09e536c09e69a0a");
+        var o = r("efae14a3f8cd9a616256");
+        e.exports = r("429cfc8e3ed333e40618")(Array, "Array", (function(e, t) {
+            this._t = o(e);
+            this._i = 0;
+            this._k = t
+        }), (function() {
+            var e = this._t;
+            var t = this._k;
+            var r = this._i++;
+            if (!e || r >= e.length) {
+                this._t = void 0;
+                return a(1)
+            }
+            if ("keys" == t) return a(0, r);
+            if ("values" == t) return a(0, e[r]);
+            return a(0, [r, e[r]])
+        }), "values");
+        c.Arguments = c.Array;
+        n("keys");
+        n("values");
+        n("entries")
+    },
+    "3177845424933048caec": function(e, t, r) {
+        "use strict";
+        r.r(t);
+        var n = r("3fe06cb9615786e0ea67");
+        var a = r("e0b8897ffbf48a102fbb");
+        var c, o;
+        try {
+            c = window.localStorage;
+            o = window.sessionStorage
+        } catch (p) {}
+
+        function i(e) {
+            function t() {
+                if (!o) return false;
+                var e = "".concat(a["k"], "storage_test");
+                var t = "";
+                try {
+                    t = o.getItem(e);
+                    if (!t) o.setItem(e, true)
+                } catch (r) {
+                    o.setItem(e, "")
+                }
+                return Boolean(t)
+            }
+            this.getItem = function(r) {
+                var n = "";
+                if (t()) n = e.getItem("".concat(a["k"]).concat(r));
+                return n
+            };
+            this.setItem = function(r, n) {
+                if (t()) e.setItem("".concat(a["k"]).concat(r), n)
+            };
+            this.removeItem = function(r) {
+                if (t()) e.removeItem("".concat(a["k"]).concat(r))
+            }
+        }
+        var f = new i(c);
+        var u = new i(o);
+        var d = r("23617503340803072f22");
+
+        function s(e, t) {
+            if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
+        }
+
+        function v(e, t) {
+            for (var r = 0; r < t.length; r++) {
+                var n = t[r];
+                n.enumerable = n.enumerable || false;
+                n.configurable = true;
+                if ("value" in n) n.writable = true;
+                Object.defineProperty(e, n.key, n)
+            }
+        }
+
+        function l(e, t, r) {
+            if (t) v(e.prototype, t);
+            if (r) v(e, r);
+            Object.defineProperty(e, "prototype", {
+                writable: false
+            });
+            return e
+        }
+
+        function b(e, t, r, n, a, c, o) {
+            try {
+                var i = e[c](o);
+                var f = i.value
+            } catch (u) {
+                r(u);
+                return
+            }
+            if (i.done) t(f);
+            else Promise.resolve(f).then(n, a)
+        }
+
+        function h(e) {
+            return function() {
+                var t = this,
+                    r = arguments;
+                return new Promise((function(n, a) {
+                    var c = e.apply(t, r);
+
+                    function o(e) {
+                        b(c, n, a, o, i, "next", e)
+                    }
+
+                    function i(e) {
+                        b(c, n, a, o, i, "throw", e)
+                    }
+                    o(void 0)
+                }))
+            }
+        }(function() {
+            var e = h(regeneratorRuntime.mark((function e(t) {
+                var r, n, c, o;
+                return regeneratorRuntime.wrap((function e(i) {
+                    while (1) switch (i.prev = i.next) {
+                        case 0:
+                            r = t;
+                            n = "true";
+                            c = function() {
+                                function e() {
+                                    s(this, e);
+                                    this.mountStatus = false
+                                }
+                                l(e, [{
+                                    key: "mount",
+                                    value: function() {
+                                        var e = h(regeneratorRuntime.mark((function e() {
+                                            var t, r;
+                                            return regeneratorRuntime.wrap((function e(a) {
+                                                while (1) switch (a.prev = a.next) {
+                                                    case 0:
+                                                        t = this.mountStatus === n;
+                                                        if (!t) {
+                                                            a.next = 5;
+                                                            break
+                                                        }
+                                                        this.setNewMount(true);
+                                                        a.next = 14;
+                                                        break;
+                                                    case 5:
+                                                        this.mountStatus = true;
+                                                        a.next = 8;
+                                                        return this.checkLib();
+                                                    case 8:
+                                                        r = a.sent;
+                                                        if (!r) {
+                                                            a.next = 14;
+                                                            break
+                                                        }
+                                                        a.next = 12;
+                                                        return this.libHandle();
+                                                    case 12:
+                                                        this.checkNewMount();
+                                                        this.mountStatus = false;
+                                                    case 14:
+                                                    case "end":
+                                                        return a.stop()
+                                                }
+                                            }), e, this)
+                                        })));
+                                        return function t() {
+                                            return e.apply(this, arguments)
+                                        }
+                                    }()
+                                }, {
+                                    key: "checkLib",
+                                    value: function() {
+                                        var e = h(regeneratorRuntime.mark((function e() {
+                                            var t, n;
+                                            return regeneratorRuntime.wrap((function e(c) {
+                                                while (1) switch (c.prev = c.next) {
+                                                    case 0:
+                                                        t = false;
+                                                        if (!r[a["j"]]) r[a["j"]] = {};
+                                                        n = r[a["j"]].version;
+                                                        if (!n) {
+                                                            n = this.getLibVersion();
+                                                            r[a["j"]].version = n
+                                                        }
+                                                        c.prev = 4;
+                                                        c.next = 7;
+                                                        return Promise.all([this.checkCSS(n), this.checkScript(n)]);
+                                                    case 7:
+                                                        t = c.sent;
+                                                        c.next = 14;
+                                                        break;
+                                                    case 10:
+                                                        c.prev = 10;
+                                                        c.t0 = c["catch"](4);
+                                                        t = false;
+                                                        d["a"].error(c.t0);
+                                                    case 14:
+                                                        return c.abrupt("return", t);
+                                                    case 15:
+                                                    case "end":
+                                                        return c.stop()
+                                                }
+                                            }), e, this, [
+                                                [4, 10]
+                                            ])
+                                        })));
+                                        return function t() {
+                                            return e.apply(this, arguments)
+                                        }
+                                    }()
+                                }, {
+                                    key: "libHandle",
+                                    value: function() {
+                                        var e = h(regeneratorRuntime.mark((function e() {
+                                            var t, n, c, o, i;
+                                            return regeneratorRuntime.wrap((function e(f) {
+                                                while (1) switch (f.prev = f.next) {
+                                                    case 0:
+                                                        t = r[a["j"]] || {}, n = t.lib, c = t.isEventsInit, o = void 0 === c ? false : c;
+                                                        if (o) {
+                                                            f.next = 6;
+                                                            break
+                                                        }
+                                                        f.t0 = n;
+                                                        if (!f.t0) {
+                                                            f.next = 6;
+                                                            break
+                                                        }
+                                                        f.next = 6;
+                                                        return n.init();
+                                                    case 6:
+                                                        i = this.collectNodes();
+                                                        f.t1 = n;
+                                                        if (!f.t1) {
+                                                            f.next = 11;
+                                                            break
+                                                        }
+                                                        f.next = 11;
+                                                        return n.render(i);
+                                                    case 11:
+                                                    case "end":
+                                                        return f.stop()
+                                                }
+                                            }), e, this)
+                                        })));
+                                        return function t() {
+                                            return e.apply(this, arguments)
+                                        }
+                                    }()
+                                }, {
+                                    key: "collectNodes",
+                                    value: function e() {
+                                        var t = document.getElementsByClassName(a["i"]);
+                                        var r = [];
+                                        if (t.length) r = Array.prototype.filter.call(t, (function(e) {
+                                            var t = e.nodeName.toLowerCase() === a["l"];
+                                            var r = !e.id;
+                                            return t && r
+                                        }));
+                                        return r
+                                    }
+                                }, {
+                                    key: "getLibVersion",
+                                    value: function e() {
+                                        return a["e"]
+                                    }
+                                }, {
+                                    key: "checkCSS",
+                                    value: function e(t) {
+                                        return new Promise((function(e) {
+                                            var r = document.getElementById(a["c"]);
+                                            if (r) e(true);
+                                            else {
+                                                var n = document.createElement("link");
+                                                n.rel = "stylesheet";
+                                                n.type = "text/css";
+                                                n.id = a["c"];
+                                                n.href = "".concat(a["b"], "/").concat(a["f"]).concat(t, ".css");
+                                                document.head.appendChild(n);
+                                                n.onload = function() {
+                                                    e(true)
+                                                };
+                                                n.onerror = function(t) {
+                                                    d["a"].error(t);
+                                                    e(false)
+                                                }
+                                            }
+                                        }))
+                                    }
+                                }, {
+                                    key: "checkScript",
+                                    value: function e(t) {
+                                        return new Promise((function(e) {
+                                            var r = document.getElementById(a["d"]);
+                                            if (r) e(true);
+                                            else {
+                                                var n = document.createElement("script");
+                                                n.type = "text/javascript";
+                                                n.id = a["d"];
+                                                n.src = "".concat(a["b"], "/").concat(a["f"]).concat(t, ".js");
+                                                document.body.appendChild(n);
+                                                n.onload = function() {
+                                                    e(true)
+                                                };
+                                                n.onerror = function(t) {
+                                                    d["a"].error(t);
+                                                    e(false)
+                                                }
+                                            }
+                                        }))
+                                    }
+                                }, {
+                                    key: "checkNewMount",
+                                    value: function e() {
+                                        var t = u.getItem(a["h"]) || "";
+                                        var r = t === n;
+                                        if (r) {
+                                            this.mount();
+                                            this.setNewMount(false)
+                                        }
+                                    }
+                                }, {
+                                    key: "setNewMount",
+                                    value: function e() {
+                                        var t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "";
+                                        u.setItem(a["h"], t)
+                                    }
+                                }, {
+                                    key: "mountStatus",
+                                    set: function e() {
+                                        var t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "";
+                                        u.setItem(a["g"], t)
+                                    },
+                                    get: function e() {
+                                        return u.getItem(a["g"]) || ""
+                                    }
+                                }]);
+                                return e
+                            }();
+                            o = function() {
+                                var e = h(regeneratorRuntime.mark((function e() {
+                                    var t;
+                                    return regeneratorRuntime.wrap((function e(r) {
+                                        while (1) switch (r.prev = r.next) {
+                                            case 0:
+                                                t = new c;
+                                                r.next = 3;
+                                                return t.mount();
+                                            case 3:
+                                            case "end":
+                                                return r.stop()
+                                        }
+                                    }), e)
+                                })));
+                                return function t() {
+                                    return e.apply(this, arguments)
+                                }
+                            }();
+                            setTimeout(o, 0);
+                        case 5:
+                        case "end":
+                            return i.stop()
+                    }
+                }), e)
+            })));
+            return function t(r) {
+                return e.apply(this, arguments)
+            }
+        })()(window)
+    },
+    "32b716d95af2fd3c5c23": function(e, t, r) {
+        var n = r("0116c75136b233002fb9");
+        var a = r("621a65702ee1a566fd32")("toStringTag");
+        var c = "Arguments" == n(function() {
+            return arguments
+        }());
+        var o = function(e, t) {
+            try {
+                return e[t]
+            } catch (r) {}
+        };
+        e.exports = function(e) {
+            var t, r, i;
+            return void 0 === e ? "Undefined" : null === e ? "Null" : "string" == typeof(r = o(t = Object(e), a)) ? r : c ? n(t) : "Object" == (i = n(t)) && "function" == typeof t.callee ? "Arguments" : i
+        }
+    },
+    "340dbda6fe6f17098a91": function(e, t, r) {
+        "use strict";
+        var n = r("770f76c876afc046e4e0")(true);
+        r("429cfc8e3ed333e40618")(String, "String", (function(e) {
+            this._t = String(e);
+            this._i = 0
+        }), (function() {
+            var e = this._t;
+            var t = this._i;
+            var r;
+            if (t >= e.length) return {
+                value: void 0,
+                done: true
+            };
+            r = n(e, t);
+            this._i += r.length;
+            return {
+                value: r,
+                done: false
+            }
+        }))
+    },
+    "380c0734c088ca78ccda": function(e, t) {
+        e.exports = "constructor,hasOwnProperty,isPrototypeOf,propertyIsEnumerable,toLocaleString,toString,valueOf".split(",")
+    },
+    "3932316ffef991f5d157": function(e, t, r) {
+        "use strict";
+        var n = r("2d13d93c336705cd8ff9");
+        var a = r("ecd0e0fb36455021f082")(5);
+        var c = "find";
+        var o = true;
+        if (c in []) Array(1)[c]((function() {
+            o = false
+        }));
+        n(n.P + n.F * o, "Array", {
+            find: function e(t) {
+                return a(this, t, arguments.length > 1 ? arguments[1] : void 0)
+            }
+        });
+        r("a5e6f0092ff0290e0bcf")(c)
+    },
+    "3f2012daa60f226e86ec": function(e, t, r) {
+        "use strict";
+        var n = r("2d13d93c336705cd8ff9");
+        var a = r("8de492c765fbfb624515");
+        n(n.S + n.F * r("7a7739dd8a198a2cfcb5")((function() {
+            function e() {}
+            return !(Array.of.call(e) instanceof e)
+        })), "Array", {
+            of: function e() {
+                var t = 0;
+                var r = arguments.length;
+                var n = new("function" == typeof this ? this : Array)(r);
+                while (r > t) a(n, t, arguments[t++]);
+                n.length = r;
+                return n
+            }
+        })
+    },
+    "3fc8b4ca32b0aebd9ff3": function(e, t, r) {
+        "use strict";
+        var n = r("2d13d93c336705cd8ff9");
+        var a = r("ecd0e0fb36455021f082")(6);
+        var c = "findIndex";
+        var o = true;
+        if (c in []) Array(1)[c]((function() {
+            o = false
+        }));
+        n(n.P + n.F * o, "Array", {
+            findIndex: function e(t) {
+                return a(this, t, arguments.length > 1 ? arguments[1] : void 0)
+            }
+        });
+        r("a5e6f0092ff0290e0bcf")(c)
+    },
+    "3fe06cb9615786e0ea67": function(e, t, r) {
+        window.regeneratorRuntime = r("2c09af3fb5c4ba3698b3");
+        r("a6444c69152f1487917b");
+        if ("undefined" === typeof Promise) {
+            r("9fbadcf2c98d054f245e").enable();
+            window.Promise = r("e6615fafe8e11b81e37a")
+        }
+    },
+    "40b064d4eb439c0c1c2b": function(e, t, r) {
+        "use strict";
+        var n = r("7a7739dd8a198a2cfcb5");
+        e.exports = function(e, t) {
+            return !!e && n((function() {
+                t ? e.call(null, (function() {}), 1) : e.call(null)
+            }))
+        }
+    },
+    "40b8419e3e2132ef0a63": function(e) {
+        e.exports = {
+            name: "tiktok_embed",
+            version: "1.0.11",
+            embedVersion: "1.0.11",
+            description: "TikTok Embed SDK",
+            main: "index.js",
+            scripts: {
+                test: "jest --forceExit",
+                dev: "eden start",
+                build: "eden build",
+                "build:gcp": "NODE_REGION=GCP eden build",
+                "build:dev": "eden build -a",
+                commit: "eden push",
+                feature: "eden feature",
+                mr: "eden release -m",
+                lint: "eden-lint ./src --fix"
+            },
+            keywords: ["tiktok", "embed"],
+            author: "yangminghui.jasmine, chloe.chao",
+            license: "ISC",
+            devDependencies: {
+                "@ies/create-eden-config": "^1.0.2",
+                "@ies/eden-lint": "^2.15.4",
+                "@testing-library/dom": "^8.17.1",
+                "@testing-library/jest-dom": "^5.16.5",
+                jest: "^28.1.3",
+                jsdom: "^20.0.0"
+            },
+            dependencies: {
+                "core-js": "2.5.7",
+                promise: "^8.0.3",
+                "regenerator-runtime": "^0.13.3"
+            },
+            husky: {
+                hooks: {
+                    "commit-msg": "commitlint .commitlintrc.js -E HUSKY_GIT_PARAMS",
+                    "pre-commit": "lint-staged"
+                }
+            },
+            "lint-staged": {
+                "*": ["eden lint format", "git add"]
+            }
+        }
+    },
+    "429cfc8e3ed333e40618": function(e, t, r) {
+        "use strict";
+        var n = r("46a1a30d151cac60057c");
+        var a = r("2d13d93c336705cd8ff9");
+        var c = r("88db22626e6c88b175cf");
+        var o = r("5f25c015bbbf9d42c661");
+        var i = r("224ae09e536c09e69a0a");
+        var f = r("5c5d334c57135891e397");
+        var u = r("62828dc3ffa96c06b7c9");
+        var d = r("12323e1413cbffdabe02");
+        var s = r("621a65702ee1a566fd32")("iterator");
+        var v = !([].keys && "next" in [].keys());
+        var l = "@@iterator";
+        var b = "keys";
+        var h = "values";
+        var p = function() {
+            return this
+        };
+        e.exports = function(e, t, r, y, m, g, w) {
+            f(r, t, y);
+            var x = function(e) {
+                if (!v && e in A) return A[e];
+                switch (e) {
+                    case b:
+                        return function t() {
+                            return new r(this, e)
+                        };
+                    case h:
+                        return function t() {
+                            return new r(this, e)
+                        }
+                }
+                return function t() {
+                    return new r(this, e)
+                }
+            };
+            var _ = t + " Iterator";
+            var k = m == h;
+            var j = false;
+            var A = e.prototype;
+            var E = A[s] || A[l] || m && A[m];
+            var S = E || x(m);
+            var O = m ? !k ? S : x("entries") : void 0;
+            var P = "Array" == t ? A.entries || E : E;
+            var T, I, R;
+            if (P) {
+                R = d(P.call(new e));
+                if (R !== Object.prototype && R.next) {
+                    u(R, _, true);
+                    if (!n && "function" != typeof R[s]) o(R, s, p)
+                }
+            }
+            if (k && E && E.name !== h) {
+                j = true;
+                S = function e() {
+                    return E.call(this)
+                }
+            }
+            if ((!n || w) && (v || j || !A[s])) o(A, s, S);
+            i[t] = S;
+            i[_] = p;
+            if (m) {
+                T = {
+                    values: k ? S : x(h),
+                    keys: g ? S : x(b),
+                    entries: O
+                };
+                if (w) {
+                    for (I in T)
+                        if (!(I in A)) c(A, I, T[I])
+                } else a(a.P + a.F * (v || j), t, T)
+            }
+            return T
+        }
+    },
+    "43382cd620aa5a0df057": function(e, t) {
+        var r;
+        r = function() {
+            return this
+        }();
+        try {
+            r = r || Function("return this")() || (1, eval)("this")
+        } catch (n) {
+            if ("object" === typeof window) r = window
+        }
+        e.exports = r
+    },
+    "4357234160788ed77205": function(e, t, r) {
+        var n = r("79c91dcd8cd554c59c7b");
+        e.exports = function(e, t, r, a) {
+            try {
+                return a ? t(n(r)[0], r[1]) : t(r)
+            } catch (o) {
+                var c = e["return"];
+                if (void 0 !== c) n(c.call(e));
+                throw o
+            }
+        }
+    },
+    "43a62b7f9a94dda95bf8": function(e, t, r) {
+        var n = r("5925dad3c5243ffee3db");
+        var a = r("1139de1233fd67f45bd7");
+        var c = "__core-js_shared__";
+        var o = a[c] || (a[c] = {});
+        (e.exports = function(e, t) {
+            return o[e] || (o[e] = void 0 !== t ? t : {})
+        })("versions", []).push({
+            version: n.version,
+            mode: r("46a1a30d151cac60057c") ? "pure" : "global",
+            copyright: "\xa9 2018 Denis Pushkarev (zloirock.ru)"
+        })
+    },
+    "46a1a30d151cac60057c": function(e, t) {
+        e.exports = false
+    },
+    "481c1f0e850b0c8d0f7d": function(e, t, r) {
+        "use strict";
+        var n = r("2d13d93c336705cd8ff9");
+        var a = r("1e0f00d296712713afe6");
+        n(n.P + n.F * !r("40b064d4eb439c0c1c2b")([].reduce, true), "Array", {
+            reduce: function e(t) {
+                return a(this, t, arguments.length, arguments[1], false)
+            }
+        })
+    },
+    "4cc77e026250beeef142": function(e, t, r) {
+        "use strict";
+        var n = r("2d13d93c336705cd8ff9");
+        var a = r("efae14a3f8cd9a616256");
+        var c = [].join;
+        n(n.P + n.F * (r("a537d0accb907bf9d41f") != Object || !r("40b064d4eb439c0c1c2b")(c)), "Array", {
+            join: function e(t) {
+                return c.call(a(this), void 0 === t ? "," : t)
+            }
+        })
+    },
+    "4d073e2fededcdd3f3d3": function(e, t) {
+        e.exports = function(e) {
+            if ("function" != typeof e) throw TypeError(e + " is not a function!");
+            return e
+        }
+    },
+    "4ef7a75a1d1957a7c5c0": function(e, t, r) {
+        var n = r("a459ab805827640a27e8");
+        e.exports = function(e, t) {
+            if (!n(e)) return e;
+            var r, a;
+            if (t && "function" == typeof(r = e.toString) && !n(a = r.call(e))) return a;
+            if ("function" == typeof(r = e.valueOf) && !n(a = r.call(e))) return a;
+            if (!t && "function" == typeof(r = e.toString) && !n(a = r.call(e))) return a;
+            throw TypeError("Can't convert object to primitive value")
+        }
+    },
+    "574ea81f94fc0b2f332a": function(e, t, r) {
+        var n = r("621a65702ee1a566fd32")("iterator");
+        var a = false;
+        try {
+            var c = [7][n]();
+            c["return"] = function() {
+                a = true
+            };
+            Array.from(c, (function() {
+                throw 2
+            }))
+        } catch (o) {}
+        e.exports = function(e, t) {
+            if (!t && !a) return false;
+            var r = false;
+            try {
+                var c = [7];
+                var i = c[n]();
+                i.next = function() {
+                    return {
+                        done: r = true
+                    }
+                };
+                c[n] = function() {
+                    return i
+                };
+                e(c)
+            } catch (o) {}
+            return r
+        }
+    },
+    "5925dad3c5243ffee3db": function(e, t) {
+        var r = e.exports = {
+            version: "2.5.7"
+        };
+        if ("number" == typeof __e) __e = r
+    },
+    "5975c7ea3ecd56e534e3": function(e, t, r) {
+        e.exports = !r("7a7739dd8a198a2cfcb5")((function() {
+            return 7 != Object.defineProperty({}, "a", {
+                get: function() {
+                    return 7
+                }
+            }).a
+        }))
+    },
+    "5b9dc0e027f5c68eff1a": function(e, t, r) {
+        var n = r("1139de1233fd67f45bd7").document;
+        e.exports = n && n.documentElement
+    },
+    "5baa1143f58e62614ca0": function(e, t, r) {
+        "use strict";
+        var n = r("2d13d93c336705cd8ff9");
+        var a = r("4d073e2fededcdd3f3d3");
+        var c = r("d394d0a4c1838202489d");
+        var o = r("7a7739dd8a198a2cfcb5");
+        var i = [].sort;
+        var f = [1, 2, 3];
+        n(n.P + n.F * (o((function() {
+            f.sort(void 0)
+        })) || !o((function() {
+            f.sort(null)
+        })) || !r("40b064d4eb439c0c1c2b")(i)), "Array", {
+            sort: function e(t) {
+                return void 0 === t ? i.call(c(this)) : i.call(c(this), a(t))
+            }
+        })
+    },
+    "5c5d334c57135891e397": function(e, t, r) {
+        "use strict";
+        var n = r("ef09ce044ac3210bc947");
+        var a = r("9d5592e83ab7f3d08974");
+        var c = r("62828dc3ffa96c06b7c9");
+        var o = {};
+        r("5f25c015bbbf9d42c661")(o, r("621a65702ee1a566fd32")("iterator"), (function() {
+            return this
+        }));
+        e.exports = function(e, t, r) {
+            e.prototype = n(o, {
+                next: a(1, r)
+            });
+            c(e, t + " Iterator")
+        }
+    },
+    "5f25c015bbbf9d42c661": function(e, t, r) {
+        var n = r("1b01d0e59d3af79760a0");
+        var a = r("9d5592e83ab7f3d08974");
+        e.exports = r("5975c7ea3ecd56e534e3") ? function(e, t, r) {
+            return n.f(e, t, a(1, r))
+        } : function(e, t, r) {
+            e[t] = r;
+            return e
+        }
+    },
+    "5f6eded14a8ed86276fc": function(e, t, r) {
+        var n = r("43a62b7f9a94dda95bf8")("keys");
+        var a = r("273d2eedcd369c189e70");
+        e.exports = function(e) {
+            return n[e] || (n[e] = a(e))
+        }
+    },
+    "621a65702ee1a566fd32": function(e, t, r) {
+        var n = r("43a62b7f9a94dda95bf8")("wks");
+        var a = r("273d2eedcd369c189e70");
+        var c = r("1139de1233fd67f45bd7").Symbol;
+        var o = "function" == typeof c;
+        var i = e.exports = function(e) {
+            return n[e] || (n[e] = o && c[e] || (o ? c : a)("Symbol." + e))
+        };
+        i.store = n
+    },
+    "62828dc3ffa96c06b7c9": function(e, t, r) {
+        var n = r("1b01d0e59d3af79760a0").f;
+        var a = r("d34390b928ecadc11dc8");
+        var c = r("621a65702ee1a566fd32")("toStringTag");
+        e.exports = function(e, t, r) {
+            if (e && !a(e = r ? e : e.prototype, c)) n(e, c, {
+                configurable: true,
+                value: t
+            })
+        }
+    },
+    "68a989d6f90923909f2a": function(e, t, r) {
+        var n = r("a459ab805827640a27e8");
+        var a = r("1139de1233fd67f45bd7").document;
+        var c = n(a) && n(a.createElement);
+        e.exports = function(e) {
+            return c ? a.createElement(e) : {}
+        }
+    },
+    "6ae9955278ddcf01bbfd": function(e, t, r) {
+        var n = r("a459ab805827640a27e8");
+        var a = r("8f648b1026e01323935b");
+        var c = r("621a65702ee1a566fd32")("species");
+        e.exports = function(e) {
+            var t;
+            if (a(e)) {
+                t = e.constructor;
+                if ("function" == typeof t && (t === Array || a(t.prototype))) t = void 0;
+                if (n(t)) {
+                    t = t[c];
+                    if (null === t) t = void 0
+                }
+            }
+            return void 0 === t ? Array : t
+        }
+    },
+    "71d3ec5bd65418e28ebc": function(e, t, r) {
+        var n = r("224ae09e536c09e69a0a");
+        var a = r("621a65702ee1a566fd32")("iterator");
+        var c = Array.prototype;
+        e.exports = function(e) {
+            return void 0 !== e && (n.Array === e || c[a] === e)
+        }
+    },
+    "74be682203e7c82cb4c9": function(e, t, r) {
+        r("89a21af31babcdc56725")("Array")
+    },
+    "770f76c876afc046e4e0": function(e, t, r) {
+        var n = r("1f3157d073736826d4fa");
+        var a = r("7ad2c0eb9a8edcc472a4");
+        e.exports = function(e) {
+            return function(t, r) {
+                var c = String(a(t));
+                var o = n(r);
+                var i = c.length;
+                var f, u;
+                if (o < 0 || o >= i) return e ? "" : void 0;
+                f = c.charCodeAt(o);
+                return f < 55296 || f > 56319 || o + 1 === i || (u = c.charCodeAt(o + 1)) < 56320 || u > 57343 ? e ? c.charAt(o) : f : e ? c.slice(o, o + 2) : (f - 55296 << 10) + (u - 56320) + 65536
+            }
+        }
+    },
+    "79c91dcd8cd554c59c7b": function(e, t, r) {
+        var n = r("a459ab805827640a27e8");
+        e.exports = function(e) {
+            if (!n(e)) throw TypeError(e + " is not an object!");
+            return e
+        }
+    },
+    "7a7739dd8a198a2cfcb5": function(e, t) {
+        e.exports = function(e) {
+            try {
+                return !!e()
+            } catch (t) {
+                return true
+            }
+        }
+    },
+    "7ad2c0eb9a8edcc472a4": function(e, t) {
+        e.exports = function(e) {
+            if (void 0 == e) throw TypeError("Can't call method on  " + e);
+            return e
+        }
+    },
+    "88db22626e6c88b175cf": function(e, t, r) {
+        var n = r("1139de1233fd67f45bd7");
+        var a = r("5f25c015bbbf9d42c661");
+        var c = r("d34390b928ecadc11dc8");
+        var o = r("273d2eedcd369c189e70")("src");
+        var i = "toString";
+        var f = Function[i];
+        var u = ("" + f).split(i);
+        r("5925dad3c5243ffee3db").inspectSource = function(e) {
+            return f.call(e)
+        };
+        (e.exports = function(e, t, r, i) {
+            var f = "function" == typeof r;
+            if (f) c(r, "name") || a(r, "name", t);
+            if (e[t] === r) return;
+            if (f) c(r, o) || a(r, o, e[t] ? "" + e[t] : u.join(String(t)));
+            if (e === n) e[t] = r;
+            else if (!i) {
+                delete e[t];
+                a(e, t, r)
+            } else if (e[t]) e[t] = r;
+            else a(e, t, r)
+        })(Function.prototype, i, (function e() {
+            return "function" == typeof this && this[o] || f.call(this)
+        }))
+    },
+    "896f33738142bf70015e": function(e, t, r) {
+        "use strict";
+        var n = r("2d13d93c336705cd8ff9");
+        var a = r("1e0f00d296712713afe6");
+        n(n.P + n.F * !r("40b064d4eb439c0c1c2b")([].reduceRight, true), "Array", {
+            reduceRight: function e(t) {
+                return a(this, t, arguments.length, arguments[1], true)
+            }
+        })
+    },
+    "89a21af31babcdc56725": function(e, t, r) {
+        "use strict";
+        var n = r("1139de1233fd67f45bd7");
+        var a = r("1b01d0e59d3af79760a0");
+        var c = r("5975c7ea3ecd56e534e3");
+        var o = r("621a65702ee1a566fd32")("species");
+        e.exports = function(e) {
+            var t = n[e];
+            if (c && t && !t[o]) a.f(t, o, {
+                configurable: true,
+                get: function() {
+                    return this
+                }
+            })
+        }
+    },
+    "8de492c765fbfb624515": function(e, t, r) {
+        "use strict";
+        var n = r("1b01d0e59d3af79760a0");
+        var a = r("9d5592e83ab7f3d08974");
+        e.exports = function(e, t, r) {
+            if (t in e) n.f(e, t, a(0, r));
+            else e[t] = r
+        }
+    },
+    "8f648b1026e01323935b": function(e, t, r) {
+        var n = r("0116c75136b233002fb9");
+        e.exports = Array.isArray || function e(t) {
+            return "Array" == n(t)
+        }
+    },
+    "9125d51ebaa93f49cfd5": function(e, t, r) {
+        "use strict";
+        var n = r("2d13d93c336705cd8ff9");
+        var a = r("ecd0e0fb36455021f082")(3);
+        n(n.P + n.F * !r("40b064d4eb439c0c1c2b")([].some, true), "Array", {
+            some: function e(t) {
+                return a(this, t, arguments[1])
+            }
+        })
+    },
+    "9d5592e83ab7f3d08974": function(e, t) {
+        e.exports = function(e, t) {
+            return {
+                enumerable: !(1 & e),
+                configurable: !(2 & e),
+                writable: !(4 & e),
+                value: t
+            }
+        }
+    },
+    "9fbadcf2c98d054f245e": function(e, t, r) {
+        "use strict";
+        var n = r("1b24b031f63a74d1f57f");
+        var a = [ReferenceError, TypeError, RangeError];
+        var c = false;
+        t.disable = o;
+
+        function o() {
+            c = false;
+            n._Y = null;
+            n._Z = null
+        }
+        t.enable = i;
+
+        function i(e) {
+            e = e || {};
+            if (c) o();
+            c = true;
+            var t = 0;
+            var r = 0;
+            var i = {};
+            n._Y = function(e) {
+                if (2 === e._V && i[e._1]) {
+                    if (i[e._1].logged) s(e._1);
+                    else clearTimeout(i[e._1].timeout);
+                    delete i[e._1]
+                }
+            };
+            n._Z = function(e, r) {
+                if (0 === e._U) {
+                    e._1 = t++;
+                    i[e._1] = {
+                        displayId: null,
+                        error: r,
+                        timeout: setTimeout(d.bind(null, e._1), u(r, a) ? 100 : 2e3),
+                        logged: false
+                    }
+                }
+            };
+
+            function d(t) {
+                if (e.allRejections || u(i[t].error, e.whitelist || a)) {
+                    i[t].displayId = r++;
+                    if (e.onUnhandled) {
+                        i[t].logged = true;
+                        e.onUnhandled(i[t].displayId, i[t].error)
+                    } else {
+                        i[t].logged = true;
+                        f(i[t].displayId, i[t].error)
+                    }
+                }
+            }
+
+            function s(t) {
+                if (i[t].logged)
+                    if (e.onHandled) e.onHandled(i[t].displayId, i[t].error);
+                    else if (!i[t].onUnhandled) {
+                    void 0;
+                    void 0
+                }
+            }
+        }
+
+        function f(e, t) {
+            void 0;
+            var r = (t && (t.stack || t)) + "";
+            r.split("\n").forEach((function(e) {
+                void 0
+            }))
+        }
+
+        function u(e, t) {
+            return t.some((function(t) {
+                return e instanceof t
+            }))
+        }
+    },
+    a459ab805827640a27e8: function(e, t) {
+        e.exports = function(e) {
+            return "object" === typeof e ? null !== e : "function" === typeof e
+        }
+    },
+    a537d0accb907bf9d41f: function(e, t, r) {
+        var n = r("0116c75136b233002fb9");
+        e.exports = Object("z").propertyIsEnumerable(0) ? Object : function(e) {
+            return "String" == n(e) ? e.split("") : Object(e)
+        }
+    },
+    a5e6f0092ff0290e0bcf: function(e, t, r) {
+        var n = r("621a65702ee1a566fd32")("unscopables");
+        var a = Array.prototype;
+        if (void 0 == a[n]) r("5f25c015bbbf9d42c661")(a, n, {});
+        e.exports = function(e) {
+            a[n][e] = true
+        }
+    },
+    a6444c69152f1487917b: function(e, t, r) {
+        r("340dbda6fe6f17098a91");
+        r("cff317ca62d09454b2d3");
+        r("0a5193b0534d54dbcda1");
+        r("3f2012daa60f226e86ec");
+        r("4cc77e026250beeef142");
+        r("1b71f5e96f29a92413b6");
+        r("5baa1143f58e62614ca0");
+        r("0f025c284bc567debf3d");
+        r("1591b90b4327c94245ad");
+        r("0565be87d109f51269ca");
+        r("9125d51ebaa93f49cfd5");
+        r("cf802dc5a6982c8247e6");
+        r("481c1f0e850b0c8d0f7d");
+        r("896f33738142bf70015e");
+        r("c9be824f185f52a1979a");
+        r("1468f5d37f30f63d76ea");
+        r("bc0f72eb2321587e4779");
+        r("fa5cd10f53a62f249502");
+        r("3932316ffef991f5d157");
+        r("3fc8b4ca32b0aebd9ff3");
+        r("74be682203e7c82cb4c9");
+        r("307014e72ed12da69e15");
+        e.exports = r("5925dad3c5243ffee3db").Array
+    },
+    a6d645856102faf17328: function(e, t, r) {
+        var n = r("1b01d0e59d3af79760a0");
+        var a = r("79c91dcd8cd554c59c7b");
+        var c = r("145c4f2bdc487b2578df");
+        e.exports = r("5975c7ea3ecd56e534e3") ? Object.defineProperties : function e(t, r) {
+            a(t);
+            var o = c(r);
+            var i = o.length;
+            var f = 0;
+            var u;
+            while (i > f) n.f(t, u = o[f++], r[u]);
+            return t
+        }
+    },
+    bc0f72eb2321587e4779: function(e, t, r) {
+        var n = r("2d13d93c336705cd8ff9");
+        n(n.P, "Array", {
+            copyWithin: r("06b2b473e53cc019ca74")
+        });
+        r("a5e6f0092ff0290e0bcf")("copyWithin")
+    },
+    bc1a333d2b6eceac22e3: function(e, t, r) {
+        e.exports = !r("5975c7ea3ecd56e534e3") && !r("7a7739dd8a198a2cfcb5")((function() {
+            return 7 != Object.defineProperty(r("68a989d6f90923909f2a")("div"), "a", {
+                get: function() {
+                    return 7
+                }
+            }).a
+        }))
+    },
+    c9be824f185f52a1979a: function(e, t, r) {
+        "use strict";
+        var n = r("2d13d93c336705cd8ff9");
+        var a = r("2076e982c14c41925fb4")(false);
+        var c = [].indexOf;
+        var o = !!c && 1 / [1].indexOf(1, -0) < 0;
+        n(n.P + n.F * (o || !r("40b064d4eb439c0c1c2b")(c)), "Array", {
+            indexOf: function e(t) {
+                return o ? c.apply(this, arguments) || 0 : a(this, t, arguments[1])
+            }
+        })
+    },
+    ca19e32ab6ee3b3692aa: function(e, t, r) {
+        var n = r("1f3157d073736826d4fa");
+        var a = Math.min;
+        e.exports = function(e) {
+            return e > 0 ? a(n(e), 9007199254740991) : 0
+        }
+    },
+    cf802dc5a6982c8247e6: function(e, t, r) {
+        "use strict";
+        var n = r("2d13d93c336705cd8ff9");
+        var a = r("ecd0e0fb36455021f082")(4);
+        n(n.P + n.F * !r("40b064d4eb439c0c1c2b")([].every, true), "Array", {
+            every: function e(t) {
+                return a(this, t, arguments[1])
+            }
+        })
+    },
+    cff317ca62d09454b2d3: function(e, t, r) {
+        var n = r("2d13d93c336705cd8ff9");
+        n(n.S, "Array", {
+            isArray: r("8f648b1026e01323935b")
+        })
+    },
+    d34390b928ecadc11dc8: function(e, t) {
+        var r = {}.hasOwnProperty;
+        e.exports = function(e, t) {
+            return r.call(e, t)
+        }
+    },
+    d394d0a4c1838202489d: function(e, t, r) {
+        var n = r("7ad2c0eb9a8edcc472a4");
+        e.exports = function(e) {
+            return Object(n(e))
+        }
+    },
+    dabaabbe8ba08d59975f: function(e, t) {
+        e.exports = function(e, t) {
+            return {
+                value: t,
+                done: !!e
+            }
+        }
+    },
+    e0b8897ffbf48a102fbb: function(e, t, r) {
+        "use strict";
+        r.d(t, "b", (function() {
+            return f
+        }));
+        r.d(t, "c", (function() {
+            return u
+        }));
+        r.d(t, "d", (function() {
+            return d
+        }));
+        r.d(t, "f", (function() {
+            return s
+        }));
+        r.d(t, "e", (function() {
+            return v
+        }));
+        r.d(t, "o", (function() {
+            return l
+        }));
+        r.d(t, "l", (function() {
+            return b
+        }));
+        r.d(t, "j", (function() {
+            return h
+        }));
+        r.d(t, "i", (function() {
+            return p
+        }));
+        r.d(t, "m", (function() {
+            return y
+        }));
+        r.d(t, "k", (function() {
+            return m
+        }));
+        r.d(t, "g", (function() {
+            return g
+        }));
+        r.d(t, "h", (function() {
+            return w
+        }));
+        r.d(t, "a", (function() {
+            return x
+        }));
+        r.d(t, "n", (function() {
+            return _
+        }));
+        var n = "production" !== "production";
+        var a = "VA" === "TTP";
+        var c = "VA" === "VA";
+        var o = a ? "https://lf16-tiktok-web.tiktokcdn-us.com" : "https://lf16-tiktok-web.ttwstatic.com";
+        var i = a ? "/obj/tiktok-web-tx/tiktok/falcon/embed" : c ? "/obj/tiktok-web-us/tiktok/falcon/embed" : "/obj/tiktok-web/tiktok/falcon/embed";
+        var f = n ? "http://127.0.0.1:4000" : "".concat(o).concat(i);
+        var u = "ttEmbedLibCSS";
+        var d = "ttEmbedLibScript";
+        var s = "embed_lib_v";
+        var v = r("40b8419e3e2132ef0a63").version;
+        var l = "https://www.tiktok.com";
+        var b = "blockquote";
+        var h = "tiktokEmbed";
+        var p = "tiktok-embed";
+        var y = "message";
+        var m = "__tt_embed__";
+        var g = "mounting";
+        var w = "newmount";
+        var x = Object.freeze({
+            CREATOR: "creator",
+            VIDEO: "video",
+            TAG: "tag",
+            MUSIC: "music",
+            TRENDING: "trending",
+            CURATED: "curated"
+        });
+        var _ = {
+            TTP: ["https://www.tiktok.com", "https://lf16-tiktok-common.tiktokcdn-us.com", "https://vmweb.us.tiktok.com"],
+            VA: ["https://www.tiktok.com", "https://lf16-tiktok-common.ttwstatic.com", "https://vmweb-va.byteoversea.com"],
+            SG: ["https://www.tiktok.com", "https://lf16-tiktok-common.ttwstatic.com", "https://vmweb-sg.byteoversea.com"],
+            Default: ["https://www.tiktok.com", "https://lf16-tiktok-common.tiktokcdn-us.com", "https://vmweb.us.tiktok.com"]
+        }
+    },
+    e3136eea77d23f8d97ec: function(e, t, r) {
+        var n = r("d34390b928ecadc11dc8");
+        var a = r("efae14a3f8cd9a616256");
+        var c = r("2076e982c14c41925fb4")(false);
+        var o = r("5f6eded14a8ed86276fc")("IE_PROTO");
+        e.exports = function(e, t) {
+            var r = a(e);
+            var i = 0;
+            var f = [];
+            var u;
+            for (u in r)
+                if (u != o) n(r, u) && f.push(u);
+            while (t.length > i)
+                if (n(r, u = t[i++])) ~c(f, u) || f.push(u);
+            return f
+        }
+    },
+    e6615fafe8e11b81e37a: function(e, t, r) {
+        "use strict";
+        var n = r("1b24b031f63a74d1f57f");
+        e.exports = n;
+        var a = d(true);
+        var c = d(false);
+        var o = d(null);
+        var i = d(void 0);
+        var f = d(0);
+        var u = d("");
+
+        function d(e) {
+            var t = new n(n._0);
+            t._V = 1;
+            t._W = e;
+            return t
+        }
+        n.resolve = function(e) {
+            if (e instanceof n) return e;
+            if (null === e) return o;
+            if (void 0 === e) return i;
+            if (true === e) return a;
+            if (false === e) return c;
+            if (0 === e) return f;
+            if ("" === e) return u;
+            if ("object" === typeof e || "function" === typeof e) try {
+                var t = e.then;
+                if ("function" === typeof t) return new n(t.bind(e))
+            } catch (r) {
+                return new n((function(e, t) {
+                    t(r)
+                }))
+            }
+            return d(e)
+        };
+        var s = function(e) {
+            if ("function" === typeof Array.from) {
+                s = Array.from;
+                return Array.from(e)
+            }
+            s = function(e) {
+                return Array.prototype.slice.call(e)
+            };
+            return Array.prototype.slice.call(e)
+        };
+        n.all = function(e) {
+            var t = s(e);
+            return new n((function(e, r) {
+                if (0 === t.length) return e([]);
+                var a = t.length;
+
+                function c(o, i) {
+                    if (i && ("object" === typeof i || "function" === typeof i))
+                        if (i instanceof n && i.then === n.prototype.then) {
+                            while (3 === i._V) i = i._W;
+                            if (1 === i._V) return c(o, i._W);
+                            if (2 === i._V) r(i._W);
+                            i.then((function(e) {
+                                c(o, e)
+                            }), r);
+                            return
+                        } else {
+                            var f = i.then;
+                            if ("function" === typeof f) {
+                                var u = new n(f.bind(i));
+                                u.then((function(e) {
+                                    c(o, e)
+                                }), r);
+                                return
+                            }
+                        } t[o] = i;
+                    if (0 === --a) e(t)
+                }
+                for (var o = 0; o < t.length; o++) c(o, t[o])
+            }))
+        };
+        n.reject = function(e) {
+            return new n((function(t, r) {
+                r(e)
+            }))
+        };
+        n.race = function(e) {
+            return new n((function(t, r) {
+                s(e).forEach((function(e) {
+                    n.resolve(e).then(t, r)
+                }))
+            }))
+        };
+        n.prototype["catch"] = function(e) {
+            return this.then(null, e)
+        }
+    },
+    ecd0e0fb36455021f082: function(e, t, r) {
+        var n = r("0e717e1f47872428608d");
+        var a = r("a537d0accb907bf9d41f");
+        var c = r("d394d0a4c1838202489d");
+        var o = r("ca19e32ab6ee3b3692aa");
+        var i = r("0594430ce9777a0767aa");
+        e.exports = function(e, t) {
+            var r = 1 == e;
+            var f = 2 == e;
+            var u = 3 == e;
+            var d = 4 == e;
+            var s = 6 == e;
+            var v = 5 == e || s;
+            var l = t || i;
+            return function(t, i, b) {
+                var h = c(t);
+                var p = a(h);
+                var y = n(i, b, 3);
+                var m = o(p.length);
+                var g = 0;
+                var w = r ? l(t, m) : f ? l(t, 0) : void 0;
+                var x, _;
+                for (; m > g; g++)
+                    if (v || g in p) {
+                        x = p[g];
+                        _ = y(x, g, h);
+                        if (e)
+                            if (r) w[g] = _;
+                            else if (_) switch (e) {
+                            case 3:
+                                return true;
+                            case 5:
+                                return x;
+                            case 6:
+                                return g;
+                            case 2:
+                                w.push(x)
+                        } else if (d) return false
+                    } return s ? -1 : u || d ? d : w
+            }
+        }
+    },
+    ef09ce044ac3210bc947: function(e, t, r) {
+        var n = r("79c91dcd8cd554c59c7b");
+        var a = r("a6d645856102faf17328");
+        var c = r("380c0734c088ca78ccda");
+        var o = r("5f6eded14a8ed86276fc")("IE_PROTO");
+        var i = function() {};
+        var f = "prototype";
+        var u = function() {
+            var e = r("68a989d6f90923909f2a")("iframe");
+            var t = c.length;
+            var n = "<";
+            var a = ">";
+            var o;
+            e.style.display = "none";
+            r("5b9dc0e027f5c68eff1a").appendChild(e);
+            e.src = "javascript:";
+            o = e.contentWindow.document;
+            o.open();
+            o.write(n + "script" + a + "document.F=Object" + n + "/script" + a);
+            o.close();
+            u = o.F;
+            while (t--) delete u[f][c[t]];
+            return u()
+        };
+        e.exports = Object.create || function e(t, r) {
+            var c;
+            if (null !== t) {
+                i[f] = n(t);
+                c = new i;
+                i[f] = null;
+                c[o] = t
+            } else c = u();
+            return void 0 === r ? c : a(c, r)
+        }
+    },
+    efae14a3f8cd9a616256: function(e, t, r) {
+        var n = r("a537d0accb907bf9d41f");
+        var a = r("7ad2c0eb9a8edcc472a4");
+        e.exports = function(e) {
+            return n(a(e))
+        }
+    },
+    f88518adc3004bf8d923: function(e, t, r) {
+        var n = r("32b716d95af2fd3c5c23");
+        var a = r("621a65702ee1a566fd32")("iterator");
+        var c = r("224ae09e536c09e69a0a");
+        e.exports = r("5925dad3c5243ffee3db").getIteratorMethod = function(e) {
+            if (void 0 != e) return e[a] || e["@@iterator"] || c[n(e)]
+        }
+    },
+    f8f08bdd917755ac017a: function(e, t, r) {
+        "use strict";
+        (function(t) {
+            e.exports = r;
+
+            function r(e) {
+                if (!n.length) {
+                    c();
+                    a = true
+                }
+                n[n.length] = e
+            }
+            var n = [];
+            var a = false;
+            var c;
+            var o = 0;
+            var i = 1024;
+
+            function f() {
+                while (o < n.length) {
+                    var e = o;
+                    o += 1;
+                    n[e].call();
+                    if (o > i) {
+                        for (var t = 0, r = n.length - o; t < r; t++) n[t] = n[t + o];
+                        n.length -= o;
+                        o = 0
+                    }
+                }
+                n.length = 0;
+                o = 0;
+                a = false
+            }
+            var u = "undefined" !== typeof t ? t : self;
+            var d = u.MutationObserver || u.WebKitMutationObserver;
+            if ("function" === typeof d) c = s(f);
+            else c = v(f);
+            r.requestFlush = c;
+
+            function s(e) {
+                var t = 1;
+                var r = new d(e);
+                var n = document.createTextNode("");
+                r.observe(n, {
+                    characterData: true
+                });
+                return function e() {
+                    t = -t;
+                    n.data = t
+                }
+            }
+
+            function v(e) {
+                return function t() {
+                    var r = setTimeout(a, 0);
+                    var n = setInterval(a, 50);
+
+                    function a() {
+                        clearTimeout(r);
+                        clearInterval(n);
+                        e()
+                    }
+                }
+            }
+            r.makeRequestCallFromTimer = v
+        }).call(this, r("43382cd620aa5a0df057"))
+    },
+    fa5cd10f53a62f249502: function(e, t, r) {
+        var n = r("2d13d93c336705cd8ff9");
+        n(n.P, "Array", {
+            fill: r("03192b087bb464f059c0")
+        });
+        r("a5e6f0092ff0290e0bcf")("fill")
+    }
 });
```

### Comparing `Cactool-0.5.7.6/cactool/static/js/code.js` & `Cactool-0.6.0/cactool/static/js/code.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,16 @@
 const SOCIAL_MEDIA = "SOCIAL_MEDIA"
 const BOOLEAN = "BOOLEAN"
 const HIDDEN = "HIDDEN"
 const LIKERT = "LIKERT"
 const ONE_TO_SEVEN = "ONE_TO_SEVEN"
 const ONE_TO_FIVE = "ONE_TO_FIVE"
 const ONE_TO_THREE = "ONE_TO_THREE"
+const DISPLAY = "DISPLAY"
+const IMAGE = "IMAGE"
 
 const ORDINAL_LOOKUP = {
     [ONE_TO_THREE]: 3,
     [ONE_TO_FIVE]: 5,
     [ONE_TO_SEVEN]: 7
 }
 
@@ -19,97 +21,108 @@
 
 const INSTAGRAM_HOSTS = [
     "instagram.com",
     "www.instagram.com"
 ]
 
 const TIKTOK_HOSTS = [
-    "tiktok.com",
     "www.tiktok.com",
-    "vm.tiktok.com"
+    "tiktok.com"
 ]
 
-function fetch_next_row(dataset_id, callback) {
+function next_row() {
     fetch(
         "/dataset/nextrow", {
             method: "POST",
             headers: {
                 "Content-Type": "application/json"
             },
             body: JSON.stringify({
-                dataset_id: dataset_id,
+                dataset_id: window.dataset_id,
             })
         }
-    ).then(response => response.json()).then(callback)
+    ).then(response => response.json()).then(update_row)
+}
+
+function fetch_row(row_number) {
+    fetch(
+        `/dataset/row`, {
+            method: "POST",
+            headers: {
+                "Content-Type": "application/json"
+            },
+            body: JSON.stringify({
+                dataset_id: window.dataset_id,
+                row_number: row_number,
+            })
+        }
+    ).then(response => response.json()).then(update_row)
 }
 
 function update_row(row) {
     if (row.is_empty) {
         window.location.replace(`/dataset/${window.dataset_id}/nomore`)
         return;
     }
     window.row_number = row.row_number
+    document.getElementById("row-name").innerText = row.row_number + 1;
     var columns = row.columns
     for (const [column_id, data] of Object.entries(columns)) {
         id = "column-" + column_id
         if (data.type === SOCIAL_MEDIA) {
             social_media_embed(data.value, id, column_id)
         } else if (data.type == BOOLEAN) {
-            checkbox(data.prompt, data.value === "true", id)
+            checkbox(data.prompt, data.value, id)
         } else if (data.type == HIDDEN) {
             hidden(data.prompt, data.value, id)
         } else if (data.type == LIKERT) {
             likert(data.prompt, data.value, id)
         } else if (
             data.type == ONE_TO_THREE ||
             data.type == ONE_TO_FIVE ||
             data.type == ONE_TO_SEVEN
         ) {
-            numerical_ordinal(data.prompt, data.value, id, ORDINAL_LOOKUP[data.type])
+            numerical_ordinal(column_id, data.value, id, ORDINAL_LOOKUP[data.type])
+        } else if (data.type == DISPLAY) {
+            display(data.prompt, data.value, id)
+        } else if (data.type == IMAGE) {
+            display_image(id, column_id)
         } else {
             input(data.prompt, data.value, id)
         }
     }
 }
 
 function get_value(column_name) {
     id = "column-" + column_name
     return document.getElementById(id).getElementsByTagName("input")[0].value
 }
 
 function get_boolean(column_name) {
-    id = "column-" + column_name
-    return document.getElementById(id).getElementsByTagName("input")[0].checked
+    const field = document.getElementById("column-" + column_name).querySelector("input:checked");
+    return field ? field.value : "";
 }
 
 function submit() {
     data = {
         dataset_id: window.dataset_id,
         row_number: window.row_number,
         values: {}
     }
 
     for (column of window.columns) {
-        console.log(column.type)
-        if (column.type === SOCIAL_MEDIA || column.type === HIDDEN) {
+        if (column.type === SOCIAL_MEDIA || column.type === HIDDEN || column.type === IMAGE) {
             continue
         } else if (
             column.type == LIKERT ||
             column.type == ONE_TO_THREE ||
             column.type == ONE_TO_FIVE ||
             column.type == ONE_TO_SEVEN) {
-            try {
-                data.values[column.name] = document.querySelector(`input[name="options-column-${column.name}"]:checked`).value;
-            } catch (exception) {
-                if (exception instanceof TypeError) {
-                    data.values[column.name] = ""
-                } else {
-                    console.log(exception)
-                }
-            }
+            const selected = document.querySelector(`input[name="options-${column.name}"]:checked`);
+            data.values[column.name] = selected ? selected.value : "";
         } else if (column.type == BOOLEAN) {
             data.values[column.name] = get_boolean(column.name);
         } else {
             data.values[column.name] = get_value(column.name)
         }
 
     }
@@ -121,14 +134,19 @@
                 "Content-Type": "application/json"
             },
             body: JSON.stringify(data)
         }
     ).then(next_row)
 }
 
+function go_to_row() {
+    const input_field = document.getElementById("row-number");
+    fetch_row(input_field.value)
+}
+
 function skip() {
     data = {
         dataset_id: window.dataset_id,
         row_number: window.row_number,
         skip: true,
     }
 
@@ -157,195 +175,174 @@
                 "Content-Type": "application/json"
             },
             body: JSON.stringify(data)
         }
     ).then(next_row)
 }
 
-function sanitise(string) {
-    const map = {
-        '&': '&amp;',
-        '<': '&lt;',
-        '>': '&gt;',
-        '"': '&quot;',
-        "'": '&#x27;',
-        "/": '&#x2F;',
-    };
-    const regex = /[&<>"'/]/ig;
-    return string.replace(
-        regex,
-        match => map[match]
-    );
-}
 
-function es(string) {
-    const map = {
-        '\\': '\\\\',
-        '"': '\\"',
-        "'": '\\\';',
-        '\n': '',
-        '\r': ''
-    };
-    const regex = /[\\"'\n\r]/ig;
-    return string.replace(
-        regex,
-        match => map[match]
-    );
+function input(column_name, value, id) {
+    const template = document.getElementById("text-input");
+    const field = template.content.cloneNode(true);
+    field.querySelector("input").value = value;
+    document.getElementById(id).replaceChildren(field);
 }
 
-function input(column_name, value, id) {
-    document.getElementById(id).innerHTML = `
-                <div class="input-group">
-                    <input class="form-control" value='${sanitise(value)}'>
-                </div>
-            `
+function display(column_name, value, id) {
+    const template = document.getElementById("display");
+    const field = template.content.cloneNode(true);
+    field.querySelector("p").innerText = value;
+    document.getElementById(id).replaceChildren(field);
 }
 
 function checkbox(column_name, value, id) {
-    document.getElementById(id).innerHTML = `
-                <div class="input-group">
-                    <input id=check-${id} class="btn-check" type=checkbox ${value? 'checked' : ''}>
-                    <label for=check-${id} class="btn btn-outline-primary"> Yes </label>
-                </div>
-            `
+    const template = document.getElementById("yes-no");
+    const field = template.content.cloneNode(true);
+    [...field.querySelectorAll("input")].forEach(responseField => {
+        responseField.name = id;
+        if (responseField.value == value) {
+            updateRadio(responseField);
+        }
+    });
+    document.getElementById(id).replaceChildren(field);
 }
 
 function likert(column_name, value, id) {
-    document.getElementById(id).innerHTML = `
-        <div class="input-group multi-choice">
-            <label for="option1-${id}" class="l15">
-                Didn't like
-                <br>
-                <input type="radio" name="options-${id}" id="$option1-${id}" autocomplete="off" value="1">
-            </label>
-
-            <label class="l15" for="option2-${id}">
-                Tolerable
-                <br>
-                <input type="radio" name="options-${id}" id="option2-${id}" autocomplete="off" value="2">
-            </label>
-
-            <label for="option3-${id}" class="l15">
-                Liked
-                <br>
-                <input type="radio" name="options-${id}" id="option3-${id}" autocomplete="off" value="3">
-            </label>
-
-            <label for="option4-${id}" class="l15">
-                Liked a lot
-                <br>
-                <input type="radio" name="options-${id}" id="option4-${id}" autocomplete="off" value="4">
-            </label>
-        
-            <label for="option5-${id}" class="l15">
-                Loved
-                <br>
-                <input type="radio" name="options-${id}" id="option5-${id}" autocomplete="off" value="5">
-            </label>
-        </div>
-    `
-    try {
-        document.querySelector(`input[name="options-${id}"][value="${es(value)}"]`).checked = true;
-    } catch (exception) {
-        if (exception instanceof TypeError) {
-
-        } else {
-            console.log(exception)
+    const template = document.getElement("likert");
+    const field = template.content.cloneNode(true);
+    [...field.querySelectorAll("input")].map(element => {
+        element.name = "options-" + id;
+        element.id = "option" + element.value + "-" + id;
+        if (element.value == value) {
+            element.checked = true;
         }
-    }
-
+    });
+    document.getElementById(id).replaceChildren(field);
 }
 
 function numerical_ordinal(column_name, value, id, number) {
-    html = `
-        <div class="input-group multi-choice">
-    `
-
-    for (i = 0; i < number; i++) {
-        html += `
-            <label for="option${i + 1}-${id}" class="l15">
-                ${i + 1} 
-                <br>
-                <input type="radio" name="options-${id}" id="option${i + 1}-${id}" autocomplete="off" value="${i + 1}">
-            </label>
-    `
-    }
-    html += "</div>"
-    document.getElementById(id).innerHTML = html
-    try {
-        document.querySelector(`input[name="options-${id}"][value="${es(value)}"]`).checked = true;
-    } catch (exception) {
-        if (exception instanceof TypeError) {
+    const fieldTemplate = document.getElementById("numerical-ordinal");
+    const selectTemplate = document.getElementById("ordinal-select");
 
-        } else {
-            console.log(exception)
+    const field = fieldTemplate.content.cloneNode(true);
+    for (let index = 0; index < number; index++) {
+        const select = selectTemplate.content.cloneNode(true);
+        const label = select.querySelector("span");
+        const radio = select.querySelector("input");
+
+        label.innerText = index + 1;
+        radio.name = "options-" + column_name;
+        radio.id = "option" + (index + 1) + "-" + column_name;
+        radio.value = index + 1;
+        if (radio.value == value) {
+            radio.checked = true;
         }
+        field.appendChild(select);
     }
 
+    document.getElementById(id).replaceChildren(field);
 }
 
 function hidden(_column_name, _value, id) {}
 
-function clear(id) {
-    document.getElementById(id).innerHTML = "";
+function social_media_embed(url, id, column_id) {
+    try {
+        host = new URL(url).host;
+    } catch {
+        display_error(id, `Unable to parse URL: ${url}`);
+        return;
+    }
+    if (TWITTER_HOSTS.includes(host)) {
+        twitter_embed(url, id);
+    } else if (INSTAGRAM_HOSTS.includes(host)) {
+        instagram_embed(id, column_id);
+    } else if (TIKTOK_HOSTS.includes(host)) {
+        tiktok_embed(id, column_id);
+    } else {
+        oembed(id, column_id);
+    }
 }
 
-function social_media_embed(url, id, column_id) {
-    host = new URL(url).host
-    if (TWITTER_HOSTS.includes(host))
-        twitter_embed(url, id)
-    else if (TIKTOK_HOSTS.includes(host))
-        tiktok_embed(url, id, column_id)
-    else if (INSTAGRAM_HOSTS.includes(host))
-        instagram_embed(url, id)
-    else if (YOUTUBE_HOSTS.includes(host))
-        youtube_embed(url, id, column_id)
+function instagram_embed(id, column_id) {
+    iframe = document.createElement("iframe")
+    iframe.setAttribute("src", `/dataset/code/instagram/${window.dataset_id}/${window.row_number}/${column_id}`)
+    iframe.style.width = "70vw"
+    iframe.style.height = "100vh"
+    document.getElementById(id).replaceChildren(iframe)
+}
+
+function tiktok_embed(id, column_id) {
+    iframe = document.createElement("iframe")
+    iframe.setAttribute("src", `/dataset/code/tiktok/${window.dataset_id}/${window.row_number}/${column_id}`)
+    iframe.style.width = "70vw"
+    iframe.style.height = "100vh"
+    document.getElementById(id).replaceChildren(iframe)
+}
+
+function display_image(id, column_id) {
+    image = document.createElement("img")
+    image.setAttribute("src", `/dataset/code/image/${window.dataset_id}/${window.row_number}/${column_id}.svg`)
+    image.style.maxWidth = "70%";
+    document.getElementById(id).replaceChildren(image)
 }
 
-function tiktok_embed(_url, id, column_id) {
+function display_error(id, error_message) {
+    span = document.createElement("pre");
+    span.innerText = error_message;
+    document.getElementById(id).replaceChildren(span);
+}
+
+function oembed(id, column_id) {
     fetch(
-            `/dataset/code/tiktok/${window.dataset_id}/${window.row_number}/${column_id}`, {
+            `/dataset/code/oembed/${window.dataset_id}/${window.row_number}/${column_id}`, {
                 method: "GET"
             }
         )
         .then(response => response.json())
         .then(
             function(data) {
                 div = document.createElement("div")
                 div.innerHTML = data["html"]
-                document.getElementById(id).appendChild(div)
+                document.getElementById(id).replaceChildren(div)
             }
         )
 }
 
 function twitter_embed(url, id) {
-    clear(id)
+    document.getElementById(id).replaceChildren();
     twttr.widgets.createTweet(
         url.split("/").at(-1),
         document.getElementById(id), {
             align: "center"
         }
     )
 }
 
-function update_next_row(dataset_id) {
-    fetch_next_row(dataset_id, update_row)
-}
-
-function next_row() {
-    update_next_row(window.dataset_id)
-}
-
 function initialise(dataset_id, columns, types) {
-    update_next_row(dataset_id)
-    window.dataset_id = dataset_id
-    window.column_names = columns
-    window.column_types = types
+    document.getElementById("row-number").addEventListener("keydown", (event) => {
+        if (event.key === "Enter") {
+            if (event.target.value === "") return;
+            event.preventDefault();
+            go_to_row();
+            event.target.value = "";
+        }
+    });
+    window.addEventListener("keydown", (event) => {
+        if (event.key === "Enter" && event.ctrlKey) {
+            event.preventDefault();
+            submit();
+            next_row();
+        }
+    });
+    window.dataset_id = dataset_id;
+    window.column_names = columns;
+    window.column_types = types;
     window.columns = window.column_names.map(
         function(column_name, index) {
             return {
                 name: column_name,
                 type: window.column_types[index]
-            }
+            };
         }
-    )
+    );
+    next_row();
 }
```

### Comparing `Cactool-0.5.7.6/cactool/templates/add_dataset.html` & `Cactool-0.6.0/cactool/templates/add_dataset.html`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,17 @@
 <html lang="en">
     <head>
         <meta charset="utf-8" />
         <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no" />
         <meta name="description" content="" />
         <meta name="author" content="" />
         <title>Cactoo - Add Dataset</title>
-        <!-- Favicon-->
         <link rel="icon" type="image/x-icon" href="/static/assets/favicon.ico" />
-        <!-- Bootstrap icons-->
-        <link href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.5.0/font/bootstrap-icons.css" rel="stylesheet" />
-        <!-- Core theme CSS (includes Bootstrap)-->
-        <link href="/static/css/styles.css" rel="stylesheet" />
+        <link href="/static/css/bootstrap-icons.css" rel="stylesheet" />
+        <link href="/static/css/bootstrap.css" rel="stylesheet" />
     </head>
     <body class="d-flex flex-column h-100">
         <main class="flex-shrink-0">
             <!-- Navigation-->
             {% include 'navigation.html' %}
             {% include 'flash.html' %}
             <!-- Page Content-->
@@ -47,11 +44,10 @@
                                 {% endfor %}
                             </div>
                         <a href="/dataset/import" class="btn btn-outline-dark">Create new dataset</a>
                     </div>
                 </div>
             </section>
         </main>
-        <!-- Bootstrap core JS-->
         <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
     </body>
 </html>
```

#### html2text {}

```diff
@@ -1,13 +1,12 @@
 
 
 
 
 
-
   {% include 'navigation.html' %} {% include 'flash.html' %}
 ****** Your datasets ******
 {% for dataset in current_user.datasets %}
 **** {{ dataset.name }} ****
 Contains {{ dataset.rows | length }} rows
 {{ dataset.description }}
```

### Comparing `Cactool-0.5.7.6/cactool/templates/code_dataset.html` & `Cactool-0.6.0/cactool/templates/import_dataset.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,42 @@
 <!DOCTYPE html>
 <html lang="en">
-  <head>
-    <meta charset="utf-8" />
-    <meta
-      name="viewport"
-      content="width=device-width, initial-scale=1, shrink-to-fit=no"
-    />
-    <meta name="description" content="" />
-    <meta name="author" content="" />
-    <title>Code dataset {{ dataset.name }}</title>
-    <!-- Favicon-->
-    <link rel="icon" type="image/x-icon" href="/static/assets/favicon.ico" />
-    <!-- Bootstrap icons-->
-    <link
-      href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.5.0/font/bootstrap-icons.css"
-      rel="stylesheet"
-    />
-    <!-- Core theme CSS (includes Bootstrap)-->
-    <link href="/static/css/styles.css" rel="stylesheet" />
-    <link href="/static/css/cactool.css" rel="stylesheet" />
-    <script src="/static/js/twitter.js"></script>
-    <script src="/static/js/code.js"></script>
-    <script src="/static/bin/tiktok_embed.js"></script>
-  </head>
-  <body
-    class="d-flex flex-column h-100"
-    onload="initialise('{{ dataset.id }}', {{  dataset.columns | map(attribute='id')  | list | safe }}, {{ dataset.columns | map(attribute='type.value') | list | safe }})">
-    <main class="flex-shrink-0">
-      <!-- Navigation-->
-      {% include 'navigation.html' %} {% include 'flash.html' %}
-      <!-- Page Content-->
-      <section class="py-5">
-        <div class="container px-5 my-5">
-          <div class="text-center mb-5">
-            <h1 class="fw-bolder">{{ dataset.name }}</h1>
-            <p class="lead fw-normal text-muted mb-0">Coding dataset</p>
-          </div>
-          <div>
-          <table class="table">
-            <thead>
-              <tr>
-                <th scope="col">Prompt</th>
-                <th style="width: 10px;"></th>
-                <th scope="col" style="text-align: center;">Data</th>
-              </tr>
-            </thead>
-            <tbody>
-            {% for column in dataset.ordered_columns %}
-                {% if column.type.value != "HIDDEN" %}
-                    <tr>
-                    <th scope="row" style="width: 0; whitespace: no-wrap">{{ column.prompt }}</th>
-                    <th style="width: 10px;"></th>
-                    <th scope="row" class="text-centre;">
-                      <div
-                      id="column-{{ column.id }}"
-                      class="text-centre"></div>
-                    </th>
-                    </tr> 
-                {% endif %}
-            {% endfor %}
-            </tbody>
-            </table>
-          </div>
-          <br>
-          <div class="row gy-1">
-            <a onclick="submit()" class="btn btn-primary">Submit</a>
-            <a onclick="skip()" class="btn btn-warning">Skip</a>
-            <a onclick="post_unavailable()" class="btn btn-danger">The post doesn't show</a>
-          </div>
-        </div>
-      </section>
-    </main>
-    <!-- Bootstrap core JS-->
-    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
-  </body>
+    <head>
+        <meta charset="utf-8" />
+        <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no" />
+        <meta name="description" content="" />
+        <meta name="author" content="" />
+        <title>Cactool - Import Dataset</title>
+        <link href="/static/css/bootstrap-icons.css" rel="stylesheet" />
+        <link href="/static/css/bootstrap.css" rel="stylesheet" />
+        <link rel="icon" type="image/x-icon" href="/static/assets/favicon.ico" />
+    </head>
+    <body class="d-flex flex-column h-100">
+        <main class="flex-shrink-0">
+            <!-- Navigation-->
+            {% include 'navigation.html' %}
+            {% include 'flash.html' %}
+            <!-- Page Content-->
+            <section class="py-5">
+                <div class="container px-5 my-5">
+                    <div class="text-center mb-5">
+                        <h1 class="fw-bolder">Import dataset</h1>
+                    </div>
+                    <div class="row gx-5">
+                        <div>
+                            <form id="form" onsubmit="document.getElementById('load').hidden = false;" action="/dataset/import/{{ project_id }}" method="POST" enctype="multipart/form-data">
+                                <input type="file" name="file" accept=".csv" class="form-control"/>
+                                <input name="description" placeholder="Dataset description" class="form-control" />
+                            </form>
+                        </div>
+                        <input type=submit class="btn btn-outline-dark" value="Import dataset" form="form">
+                    </div>
+                </div>
+                <div id="load" class="spinner-border" hidden role="status">
+                  <span class="sr-only"></span>
+                </div>
+            </section>
+                    </main>
+        <!-- Bootstrap core JS-->
+        <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
+    </body>
 </html>
```

#### html2text {}

```diff
@@ -1,15 +1,10 @@
 
 
 
 
 
-
-
   {% include 'navigation.html' %} {% include 'flash.html' %}
-****** {{ dataset.name }} ******
-Coding dataset
-Prompt               Data
-{{ column.prompt }}
-
-Submit Skip The post doesn't show
+****** Import dataset ******
+[File] [description         ]
+[Import dataset]
```

### Comparing `Cactool-0.5.7.6/cactool/templates/create_project.html` & `Cactool-0.6.0/cactool/templates/index.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 <!DOCTYPE html>
 <html lang="en">
     <head>
         <meta charset="utf-8" />
         <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no" />
         <meta name="description" content="" />
         <meta name="author" content="" />
-        <title>Cactool - Create Project</title>
-        <!-- Favicon-->
-        <link rel="icon" type="image/x-icon" href="/static/assets/favicon.ico"/>
-        <!-- Bootstrap icons-->
-        <link href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.5.0/font/bootstrap-icons.css" rel="stylesheet" />
-        <!-- Core theme CSS (includes Bootstrap)-->
-        <link href="/static/css/styles.css" rel="stylesheet" />
+        <title>Cactool</title>
+        <link href="/static/css/bootstrap-icons.css" rel="stylesheet" />
+        <link href="/static/css/bootstrap.css" rel="stylesheet" />
+        <link rel="icon" type="image/x-icon" href="/static/assets/favicon.ico" />
+        
+        {% include 'card.html' %}
     </head>
     <body class="d-flex flex-column h-100">
         <main class="flex-shrink-0">
-            {% include 'navigation.html' %}
-            {% include 'flash.html' %}
-            <form action="/project/create" method="post">
-            <section class="py-5" id="features">
-                <div class="container px-5 my-5">
-                    <div class="row gx-5">
-                        <div class="col-lg-4 mb-5 mb-lg-0"><h2 class="fw-bolder mb-0">Create project</h2></div>
-                        <div class="col-lg-8">
-                            <div class="row gx-5 row-cols-1 row-cols-md-2">
-                                <div class="col mb-5 h-100">
-                                    <div class="feature bg-primary bg-gradient text-white rounded-3 mb-3"><i class="bi bi-collection"></i></div>
-                                    <h2 class="h5">Project name</h2>
-                                    <input name=name class="mb-0"/>
+          {% include 'navigation.html' %}
+            <!-- Header-->
+            <header class="bg-dark py-5">
+                <div class="container px-5">
+                    <div class="row gx-5 align-items-center justify-content-center">
+                        <div class="col-lg-8 col-xl-7 col-xxl-6">
+                            <div class="my-5 text-center text-xl-start">
+                              <h1 class="display-5 fw-bolder text-white mb-2">Begin coding with Cactool</h1>
+                                <div class="d-grid gap-3 d-sm-flex justify-content-sm-center justify-content-xl-start">
+                                    <a class="btn btn-primary btn-lg px-4 me-sm-3" href="/signup">Sign up</a>
+                                    <a class="btn btn-outline-light btn-lg px-4" href="/login">Log in</a>
                                 </div>
-                                <div class="col mb-5 h-100">
-                                    <div class="feature bg-primary bg-gradient text-white rounded-3 mb-3"><i class="bi bi-collection"></i></div>
-                                    <h2 class="h5">Project description</h2>
-                                    <input name=description class="mb-0"/>
-                                </div>
-
                             </div>
-                            <input type="submit" class="btn btn-primary btn-lg px-4 me-sm-3" value="Create Project"/>
                         </div>
+                        <div class="col-xl-5 col-xxl-6 d-none d-xl-block text-center"><img class="img-fluid rounded-3 my-5" src="/static/assets/cactool-large.png" alt="..." /></div>
+                    </div>
+                </div>
+            </header>
+            <section class="py-5" id="features">
+                <div class="container px-5 my-5">
+                    <div class="row gx-5">
+                        <div class="col-lg-4 mb-5 mb-lg-0"><h2 class="fw-bolder mb-0">The quick and easy way to human-code social media posts</h2></div>
                     </div>
                 </div>
             </section>
-            </form>
         </main>
-        <!-- Bootstrap core JS-->
         <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
     </body>
 </html>
```

#### html2text {}

```diff
@@ -1,14 +1,13 @@
 
 
 
 
 
+ {% include 'card.html' %}
+ {% include 'navigation.html' %}
+****** Begin coding with Cactool ******
+Sign_up Log_in
+[...]
 
- {% include 'navigation.html' %} {% include 'flash.html' %}
-***** Create project *****
-***** Project name *****
-[name                ]
-***** Project description *****
-[description         ]
-[Create Project]
+***** The quick and easy way to human-code social media posts *****
```

### Comparing `Cactool-0.5.7.6/cactool/templates/dashboard.html` & `Cactool-0.6.0/cactool/templates/dashboard.html`

 * *Files 7% similar despite different names*

```diff
@@ -2,27 +2,22 @@
 <html lang="en">
     <head>
         <meta charset="utf-8" />
         <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no" />
         <meta name="description" content="" />
         <meta name="author" content="" />
         <title>Cactool - Projects</title>
-        <!-- Favicon-->
+        <link href="/static/css/bootstrap-icons.css" rel="stylesheet" />
+        <link href="/static/css/bootstrap.css" rel="stylesheet" />
         <link rel="icon" type="image/x-icon" href="/static/assets/favicon.ico" />
-        <!-- Bootstrap icons-->
-        <link href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.5.0/font/bootstrap-icons.css" rel="stylesheet" />
-        <!-- Core theme CSS (includes Bootstrap)-->
-        <link href="/static/css/styles.css" rel="stylesheet" />
     </head>
     <body class="d-flex flex-column h-100">
         <main class="flex-shrink-0">
-            <!-- Navigation-->
             {% include 'navigation.html' %}
             {% include 'flash.html' %}
-            <!-- Page Content-->
             <section class="py-5">
                 <div class="container px-5 my-5">
                     <div class="text-center mb-5">
                         <h1 class="fw-bolder">Projects</h1>
                     </div>
                     <div class="row gx-5">
                             <div class="accordion mb-5" id="accordionExample">
```

#### html2text {}

```diff
@@ -1,14 +1,13 @@
 
 
 
 
 
-
-  {% include 'navigation.html' %} {% include 'flash.html' %}
+ {% include 'navigation.html' %} {% include 'flash.html' %}
 ****** Projects ******
 {% for project in projects %}
 **** {{ project.name }} ****
 Contains {{ project.datasets | length }} datasets
 {{ project.description }}
 
 Open
```

### Comparing `Cactool-0.5.7.6/cactool/templates/delete_dataset.html` & `Cactool-0.6.0/cactool/templates/delete_dataset.html`

 * *Files 19% similar despite different names*

```diff
@@ -5,29 +5,22 @@
     <meta
       name="viewport"
       content="width=device-width, initial-scale=1, shrink-to-fit=no"
     />
     <meta name="description" content="" />
     <meta name="author" content="" />
     <title>Confirm dataset deletion</title>
-    <!-- Favicon-->
     <link rel="icon" type="image/x-icon" href="/satic/assets/favicon.ico" />
-    <!-- Bootstrap icons-->
-    <link
-      href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.5.0/font/bootstrap-icons.css"
-      rel="stylesheet"
-    />
-    <!-- Core theme CSS (includes Bootstrap)-->
-    <link href="/static/css/styles.css" rel="stylesheet" />
+    <link href="/static/css/bootstrap-icons.css" rel="stylesheet" />
+    <link href="/static/css/bootstrap.css" rel="stylesheet" />
+    <link href="/static/css/login.css" rel=stylesheet />
   </head>
   <body class="d-flex flex-column h-100">
     <main class="flex-shrink-0">
-      <!-- Navigation-->
       {% include 'navigation.html' %} {% include 'flash.html' %}
-      <!-- Page Content-->
       <form method="POST" action="/dataset/delete" id="confirm" hidden>
         <input hidden value="{{dataset.id}}" name="dataset_id">
         <input hidden value="true" name="confirm">
       </form>
       <section class="py-5">
         <div class="container px-5 my-5">
           <div class="text-center mb-5">
@@ -36,11 +29,10 @@
           </div>
           <div class="row gx-5">
             <input type="submit" form="confirm" href="/dataset/delete/{{ dataset.id }}" class="btn btn-outline-danger" value="Confirm deletion"></input>
           </div>
         </div>
       </section>
     </main>
-    <!-- Bootstrap core JS-->
     <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 
 
 
 
 
 
-  {% include 'navigation.html' %} {% include 'flash.html' %}
+ {% include 'navigation.html' %} {% include 'flash.html' %}
 [{{dataset.id}}      ] [true                ]
 ****** {{ dataset.name }} ******
 Are you sure you want to delete this dataset?
 [Confirm deletion]
```

### Comparing `Cactool-0.5.7.6/cactool/templates/delete_project.html` & `Cactool-0.6.0/cactool/templates/delete_project.html`

 * *Files 18% similar despite different names*

```diff
@@ -5,29 +5,22 @@
     <meta
       name="viewport"
       content="width=device-width, initial-scale=1, shrink-to-fit=no"
     />
     <meta name="description" content="" />
     <meta name="author" content="" />
     <title>Confirm project deletion</title>
-    <!-- Favicon-->
     <link rel="icon" type="image/x-icon" href="/satic/assets/favicon.ico" />
-    <!-- Bootstrap icons-->
-    <link
-      href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.5.0/font/bootstrap-icons.css"
-      rel="stylesheet"
-    />
-    <!-- Core theme CSS (includes Bootstrap)-->
-    <link href="/static/css/styles.css" rel="stylesheet" />
+    <link href="/static/css/bootstrap-icons.css" rel="stylesheet" />
+    <link href="/static/css/bootstrap.css" rel="stylesheet" />
+
   </head>
   <body class="d-flex flex-column h-100">
     <main class="flex-shrink-0">
-      <!-- Navigation-->
       {% include 'navigation.html' %} {% include 'flash.html' %}
-      <!-- Page Content-->
       <form method="POST" id="confirm" hidden>
         <input hidden value="{{project.id}}" name="project_id">
         <input hidden value="true" name="confirm">
       </form>
       <section class="py-5">
         <div class="container px-5 my-5">
           <div class="text-center mb-5">
@@ -36,11 +29,10 @@
           </div>
           <div class="row gx-5">
             <input type="submit" form="confirm"  class="btn btn-outline-danger" value="Confirm deletion"></input>
           </div>
         </div>
       </section>
     </main>
-    <!-- Bootstrap core JS-->
     <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
 
 
 
 
 
-
-  {% include 'navigation.html' %} {% include 'flash.html' %}
+ {% include 'navigation.html' %} {% include 'flash.html' %}
 [{{project.id}}      ] [true                ]
 ****** {{ project.name }} ******
 Are you sure you want to delete this project?
 [Confirm deletion]
```

### Comparing `Cactool-0.5.7.6/cactool/templates/flash.html` & `Cactool-0.6.0/cactool/templates/flash.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.5.7.6/cactool/templates/import_dataset.html` & `Cactool-0.6.0/cactool/templates/view_project.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,51 @@
+{% from "macros.html" import show_dataset %}
 <!DOCTYPE html>
 <html lang="en">
     <head>
         <meta charset="utf-8" />
         <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no" />
         <meta name="description" content="" />
         <meta name="author" content="" />
-        <title>Cactool - Import Dataset</title>
-        <!-- Favicon-->
+        <title>{{ project.name }}</title>
         <link rel="icon" type="image/x-icon" href="/static/assets/favicon.ico" />
-        <!-- Bootstrap icons-->
-        <link href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.5.0/font/bootstrap-icons.css" rel="stylesheet" />
-        <!-- Core theme CSS (includes Bootstrap)-->
-        <link href="/static/css/styles.css" rel="stylesheet" />
-    </head>
+        <link href="/static/css/bootstrap-icons.css" rel="stylesheet" />
+        <link href="/static/css/bootstrap.css" rel="stylesheet" />
+   </head>
     <body class="d-flex flex-column h-100">
         <main class="flex-shrink-0">
             <!-- Navigation-->
             {% include 'navigation.html' %}
             {% include 'flash.html' %}
             <!-- Page Content-->
             <section class="py-5">
                 <div class="container px-5 my-5">
                     <div class="text-center mb-5">
-                        <h1 class="fw-bolder">Import dataset</h1>
+                        <h1 class="fw-bolder">{{ project.name }}</h1>
+                        <p class="lead fw-normal text-muted mb-0">Datasets</p>
                     </div>
                     <div class="row gx-5">
-                        <div>
-                            <form id="form" action="/dataset/import/{{ project_id }}" method="POST" enctype="multipart/form-data">
-                                <input type="file" name="file" accept=".csv" class="form-control"/>
-                                <input name="description" placeholder="Dataset description" class="form-control" />
-                            </form>
-                        </div>
-                        <input type=submit class="btn btn-outline-dark" value="Import dataset" form="form">
+                            <!-- FAQ Accordion 1-->
+                            <!-- <h2 class="fw-bolder mb-3">Account &amp; Billing</h2> -->
+                            <div class="accordion mb-5" id="accordionExample">
+                                {% for dataset in project.datasets %}
+                                   {{ show_dataset(dataset, current_user) }} 
+                                {% endfor %}
+                            </div>
+                        <a href="/dataset/import/{{ project.id }}" class="btn btn-outline-success">Add dataset</a>
+
+                    </div>
+                    <br>
+
+                    <div class="row gx-5">
+                        <form action="/project/delete" method="POST" id="delete" hidden>
+                            <input name="project_id" value="{{ project.id }}" hidden/>
+                        </form>
+                        <input type="submit" form="delete" class="btn btn-outline-danger" value="Delete project"></input>
+                        
                     </div>
                 </div>
             </section>
         </main>
-        <!-- Bootstrap core JS-->
         <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
     </body>
 </html>
```

#### html2text {}

```diff
@@ -1,11 +1,17 @@
-
+{% from "macros.html" import show_dataset %}
 
 
 
 
 
   {% include 'navigation.html' %} {% include 'flash.html' %}
-****** Import dataset ******
-[File] [description         ]
-[Import dataset]
+****** {{ project.name }} ******
+Datasets
+
+{% for dataset in project.datasets %} {{ show_dataset(dataset, current_user) }}
+{% endfor %}
+Add_dataset
+
+[{{ project.id }}    ]
+[Delete project]
```

### Comparing `Cactool-0.5.7.6/cactool/templates/macros.html` & `Cactool-0.6.0/cactool/templates/macros.html`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     <div
       class="accordion-collapse collapse show"
       id="collapseOne"
       aria-labelledby="headingOne"
       data-bs-parent="#accordionExample"
     >
       <div class="accordion-body">
-        <strong>Contains {{ dataset.num_rows }} rows</strong>
+          <strong>Contains {{ dataset.num_rows }} rows ({{ dataset.code_status_description }})</strong>
         <br />
         {{ dataset.description }}
         <br />
         <br />
         {% if user.can_code(dataset) %}
         <a
           href="/dataset/code/{{ dataset.id }}"
@@ -34,14 +34,19 @@
         {% endif %}
         {% if user.can_edit(dataset) %}
         <a
           href="/dataset/{{ dataset.id }}"
           class="btn btn-outline-dark"
           >Edit</a
         >
+        <a
+          href="/dataset/{{ dataset.id }}/images/upload"
+          class="btn btn-outline-dark"
+          >Images</a
+        >
         {% endif %}
         {% if user.can_export(dataset) %}
         <input
           href="/dataset/export/{{ dataset.id }}"
           class="btn btn-outline-dark"
           type="submit"
           value="Export"
@@ -59,8 +64,8 @@
             type="hidden"
           />
         </form>
         {% endif %}
       </div>
     </div>
 </div>
-{% endmacro %}
+{% endmacro %}
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% macro show_dataset(dataset, user)%}
 ****  {{ dataset.name }}  ****
-Contains {{ dataset.num_rows }} rows
+Contains {{ dataset.num_rows }} rows ({{ dataset.code_status_description }})
 {{ dataset.description }}
 
 {% if user.can_code(dataset) %} Code {% endif %} {% if user.can_edit(dataset)
-%} Edit {% endif %} {% if user.can_export(dataset) %} [Export]
+%} Edit Images {% endif %} {% if user.can_export(dataset) %} [Export]
 {% endif %}
 {% endmacro %}
```

### Comparing `Cactool-0.5.7.6/cactool/templates/show_datasets.html` & `Cactool-0.6.0/cactool/templates/show_datasets.html`

 * *Files 16% similar despite different names*

```diff
@@ -3,20 +3,17 @@
 <html lang="en">
     <head>
         <meta charset="utf-8" />
         <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no" />
         <meta name="description" content="" />
         <meta name="author" content="" />
         <title>Cactool - Datasets</title>
-        <!-- Favicon-->
         <link rel="icon" type="image/x-icon" href="/static/assets/favicon.ico" />
-        <!-- Bootstrap icons-->
-        <link href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.5.0/font/bootstrap-icons.css" rel="stylesheet" />
-        <!-- Core theme CSS (includes Bootstrap)-->
-        <link href="/static/css/styles.css" rel="stylesheet" />
+        <link href="/static/css/bootstrap-icons.css" rel="stylesheet" />
+        <link href="/static/css/bootstrap.css" rel="stylesheet" />
     </head>
     <body class="d-flex flex-column h-100">
         <main class="flex-shrink-0">
             <!-- Navigation-->
             {% include 'navigation.html' %}
             {% include 'flash.html' %}
             <!-- Page Content-->
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
 {% from "macros.html" import show_dataset %}
 
 
 
 
 
-
   {% include 'navigation.html' %} {% include 'flash.html' %}
 ****** Your datasets ******
 {% for dataset in datasets %} {{ show_dataset(dataset, current_user) }} {%
 endfor %}
```

### Comparing `Cactool-0.5.7.6/cactool/templates/view_dataset.html` & `Cactool-0.6.0/cactool/templates/code_dataset.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,107 +1,105 @@
-{% from "macros.html" import show_dataset %}
 <!DOCTYPE html>
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta
       name="viewport"
       content="width=device-width, initial-scale=1, shrink-to-fit=no"
     />
     <meta name="description" content="" />
     <meta name="author" content="" />
-    <title>{{ dataset.name }}</title>
-    <!-- Favicon-->
-    <link rel="icon" type="image/x-icon" href="/satic/assets/favicon.ico" />
-    <!-- Bootstrap icons-->
-    <link
-      href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.5.0/font/bootstrap-icons.css"
-      rel="stylesheet"
-    />
-    <!-- Core theme CSS (includes Bootstrap)-->
-    <link href="/static/css/styles.css" rel="stylesheet" />
+    <title>Code dataset {{ dataset.name }}</title>
+    <link rel="icon" type="image/x-icon" href="/static/assets/favicon.ico" />
+    <link href="/static/css/bootstrap-icons.css" rel="stylesheet" />
+    <link href="/static/css/bootstrap.css" rel="stylesheet" /> 
+    <link href="/static/css/cactool.css" rel="stylesheet" />
+    <script src="/static/js/twitter.js"></script>
+    <script src="/static/js/code.js"></script>
+    <script src="/static/bin/tiktok_embed.js"></script>
   </head>
-  <body class="d-flex flex-column h-100">
+  <body
+    class="d-flex flex-column h-100"
+    onload="initialise('{{ dataset.id }}', {{  dataset.columns | map(attribute='id')  | list | safe }}, {{ dataset.columns | map(attribute='type.value') | list | safe }})">
     <main class="flex-shrink-0">
-      <!-- Navigation-->
       {% include 'navigation.html' %} {% include 'flash.html' %}
-      <!-- Page Content-->
-      <section class="py-5">
-        <div class="container px-5 my-5">
+      <section class="py-5" style="display: flex; justify-content: center;">
+        <div class="code-container">
           <div class="text-center mb-5">
             <h1 class="fw-bolder">{{ dataset.name }}</h1>
-            <p class="lead fw-normal text-muted mb-0">Viewing dataset</p>
-          </div>
-          <div class="row gx-5">
-            <!-- FAQ Accordion 1-->
-            <!-- <h2 class="fw-bolder mb-3">Account &amp; Billing</h2> -->
-            <div class="accordion mb-5" id="accordionExample">
-              {{ show_dataset(dataset, current_user) }}
-            </div>
-          </div>
-          
-          <div class="text-center mb-5">
-            <h1 class="fw-bolder h4">Coder Invite Link</h1>
-          </div>
-          <div class="input-group">
-            <input class="form-control" value="{{ invite_link }}" readonly style="background-color: transparent; font-family: monospace;">
-          </div>
-          
-          <br/>
-
-          <div class="text-center mb-5">
-            <h1 class="fw-bolder h4">Data Types</h1>
+            <p class="lead fw-normal text-muted mb-0">Row <span id="row-name"></span></p>
           </div>
-          <div>
-            <form id="types" action="/dataset/update" method="post">
-                <input type="hidden" name="dataset_id" value="{{ dataset.id }}">
+          <div class="text-center">
+              <div class="fw-bolder">Go to row</div>
+              <div class="input-group centered-flex">
+                <input id=row-number class="form-control small-number" inputmode=numeric min=0>
+                <a onclick="go_to_row()" class="btn btn-outline-dark">Go</a>
+              </div>
+              <div class="
+                  code-window
+                  {% if dataset.has_social_media %}
+                    with-social-media
+                  {% else %}
+                    without-social-media
+                  {% endif %}
+              ">
+              <div class="social-window">
+                  {% for column in dataset.ordered_columns %}
+                      {% if column.type.is_social_media %}
+                         <table class="table">
+                            <thead>
+                              <tr>
+                                  <th class="no-border" scope="col" style="text-align: center;">{{ column.prompt }}</th>
+                              </tr>
+                            </thead>
+                            <tbody>
+                                <tr>
+                                    <th class="no-border" scope="row" class="text-centre;">
+                                      <div id="column-{{ column.id }}" class="text-centre"></div>
+                                    </th>
+                                </tr>
+                            </tbody>
+                        </table>
+                      {% endif %}
+                  {% endfor %}
+              </div>
+              <div class="response-window">
                 <table class="table">
-                  <thead>
-                    <tr>
-                      <th scope="col">Column Name</th>
-                      <th scope="col">Question Type</th>
-                      <th scope="col">Prompt</th>
-                    </tr>
-                  </thead>
-                  <tbody>
-                    {% for column in dataset.columns %}
-                    <tr>
-                    <th scope="row">{{ column.name }}</th>
-                    <th scope="row">
-                      <select name="{{ column.name }}-type" class="form-select" aria-label="Default select example">
-                        <option>Select Data Type</option>
-                        <option {{ 'selected' if column.type.value == SOCIAL_MEDIA else '' }} value="SOCIAL_MEDIA">Social Media URL</option>
-                        <option {{ 'selected' if column.type.value == STRING else '' }} value="STRING">Text</option>
-                        <option {{ 'selected' if column.type.value == NUMBER else ''}} value="NUMBER">Number</option>
-                        <option {{ 'selected' if column.type.value == BOOLEAN else ''}} value="BOOLEAN">True / False</option>
-                        <option {{ 'selected' if column.type.value == HIDDEN else ''}} value="HIDDEN">Hidden</option>
-                        <option {{ 'selected' if column.type.value == ONE_TO_THREE else ''}} value="ONE_TO_THREE">Scale from 1 to 3</option>
-                        <option {{ 'selected' if column.type.value == ONE_TO_FIVE else ''}} value="ONE_TO_FIVE">Scale from 1 to 5</option>
-                        <option {{ 'selected' if column.type.value == ONE_TO_SEVEN else ''}} value="ONE_TO_SEVEN">Scale from 1 to 7</option>
-                      </select>
-                    </th>
-                    <th scope="row"><input value="{{ column.prompt }}" class="form-control" name="{{ column.name }}-prompt"/></th>
-                    </tr> 
-                    {% endfor %}
-                  </tbody>
+                <colgroup>
+                    <col style="width: 30%;">
+                    <col style="width: 70%;">
+                </colgroup>
+                <thead>
+                  <tr>
+                    <th scope="col">Prompt</th>
+                    <th scope="col" style="text-align: center;">Response</th>
+                  </tr>
+                </thead>
+                <tbody>
+                {% for column in dataset.ordered_columns %}
+                    {% if column.type.value not in ["HIDDEN", "SOCIAL_MEDIA", "IMAGE"] %}
+                        <tr>
+                        <th scope="row" style="width: 0; whitespace: no-wrap">{{ column.prompt }}</th>
+                        <th scope="row" class="text-centre;">
+                          <div
+                          id="column-{{ column.id }}"
+                          class="text-centre"></div>
+                        </th>
+                        </tr> 
+                    {% endif %}
+                {% endfor %}
+                </tbody>
                 </table>
-            </form>
-          </div>
-
-          <div class="row gx-5">
-            <input type=submit form="types" href="/dataset/update" class="btn btn-outline-dark" value="Update dataset"/>
-          </div>
-          <br>
-          <form hidden id="delete" method="POST" action="/dataset/delete">
-            <input name="dataset_id" value="{{dataset.id}}" hidden/>
-            <input name="confirm" value="false" hidden/>
-          </form>
-          <div class="row gx-5">
-            <input type="submit" form="delete" href="/dataset/delete/{{ dataset.id }}" class="btn btn-outline-danger" value="Delete dataset"/>
-          </div>
+              </div>
+        </div>
+        <div>
+          <a onclick="submit()" class="btn btn-dark">Submit</a>
+          <a onclick="skip()" class="btn btn-outline-dark">Skip</a>
+          <a onclick="post_unavailable()" class="btn btn-outline-secondary">The post doesn't show</a>
         </div>
+
       </section>
     </main>
-    <!-- Bootstrap core JS-->
+    {% include 'coding_interface.html' %}
     <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,43 +1,19 @@
-{% from "macros.html" import show_dataset %}
 
 
 
 
 
 
-  {% include 'navigation.html' %} {% include 'flash.html' %}
+ {% include 'navigation.html' %} {% include 'flash.html' %}
 ****** {{ dataset.name }} ******
-Viewing dataset
-
-{{ show_dataset(dataset, current_user) }}
-****** Coder Invite Link ******
-[{{ invite_link }}   ]
-
-****** Data Types ******
-Column Name       Question Type                          Prompt
-                  { 'selected' if column.type.value ==
-                  SOCIAL_MEDIA else '' }}
-                  value="SOCIAL_MEDIA">Social Media URL
-                  { 'selected' if column.type.value ==
-                  STRING else '' }} value="STRING">Text
-                  { 'selected' if column.type.value ==
-                  NUMBER else ''}} value="NUMBER">Number
-                  { 'selected' if column.type.value ==
-                  BOOLEAN else ''}} value="BOOLEAN">True
-                  / False
-{{ column.name }} { 'selected' if column.type.value ==   [{{ column.prompt }} ]
-                  HIDDEN else ''}} value="HIDDEN">Hidden
-                  { 'selected' if column.type.value ==
-                  ONE_TO_THREE else ''}}
-                  value="ONE_TO_THREE">Scale from 1 to 3
-                  { 'selected' if column.type.value ==
-                  ONE_TO_FIVE else ''}}
-                  value="ONE_TO_FIVE">Scale from 1 to 5
-                  { 'selected' if column.type.value ==
-                  ONE_TO_SEVEN else ''}}
-                  value="ONE_TO_SEVEN">Scale from 1 to 7
-[Update dataset]
-
-[{{dataset.id}}      ] [false               ]
-[Delete dataset]
-
+Row
+Go to row
+[                    ] Go
+{% for column in dataset.ordered_columns %} {% if column.type.is_social_media
+%}
+{{ column.prompt }}
+{% endif %} {% endfor %}
+Prompt              Response
+{{ column.prompt }}
+Submit Skip The post doesn't show
+  {% include 'coding_interface.html' %}
```

### Comparing `Cactool-0.5.7.6/cactool/views/home.py` & `Cactool-0.6.0/cactool/views/home.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from flask import Blueprint, url_for, redirect, render_template
+from flask import Blueprint, redirect, render_template, url_for
 from flask_login import current_user
 
 home = Blueprint("home", __name__)
 
+
 @home.route("/")
 def index():
     if current_user.is_authenticated:
         return redirect(url_for("home.dashboard"))
 
     return render_template("index.html")
 
 
 @home.route("/dashboard")
 def dashboard():
     if not current_user.is_authenticated:
         return redirect(url_for("authentication.login"))
 
     projects = current_user.editable_projects()
-    
-    return render_template("dashboard.html", projects=projects)
+
+    return render_template("dashboard.html", projects=projects)
```

### Comparing `Cactool-0.5.7.6/cactool/views/projects.py` & `Cactool-0.6.0/cactool/views/projects.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-from flask import Blueprint, render_template, flash, redirect, url_for, request
+import uuid
+
+from flask import Blueprint, flash, redirect, render_template, request, url_for
 from flask_login import current_user
-from ..database import db, Project, Dataset, ProjectAccess
+
+from ..database import Dataset, Project, ProjectAccess, db
 from ..dates import date_string
 from ..types import AccessLevel
-import uuid
 
 projects = Blueprint("projects", __name__)
 
+
 @projects.route("/project/<project_id>")
 def view_project(project_id):
     project = Project.query.get(project_id)
     if project and current_user.can_edit(project):
         return render_template("view_project.html", project=project)
     else:
         flash("The selected project doesn't exist")
         return redirect(url_for("home.dashboard"))
 
+
 @projects.route("/dataset/add/<project_id>", methods=["POST", "GET"])
 def add_dataset(project_id):
     if request.method == "GET":
         return render_template("add_dataset.html")
 
     dataset_id = request.form.get("dataset_id")
     project = Project.query.get(project_id)
@@ -27,24 +31,25 @@
     if not dataset:
         flash("The selected dataset doesn't exist")
         return render_template("add_dataset.html")
 
     if not project:
         flash("The selected project doesn't exist")
         return render_template("add_dataset.html")
-    
+
     if not current_user.can_edit(project) or not current_user.can_edit(dataset):
         flash("Deprecated endpoint")
         return "Deprecated endpoint"
 
     project.datasets.append(dataset)
     db.session.commit()
 
     return redirect(url_for("projects.view_project", project_id=project_id))
 
+
 @projects.route("/project/create", methods=["POST", "GET"])
 def create_project():
     if request.method == "GET":
         return render_template("create_project.html")
 
     name = request.form.get("name")
     if not name:
@@ -58,26 +63,23 @@
     user = current_user
 
     description = request.form.get("description")
 
     project = Project(
         id=uuid.uuid4().hex,
         name=name,
-        description=description if description else f"Uploaded {date_string()}"
+        description=description if description else f"Uploaded {date_string()}",
     )
 
     user.project_rights.append(
         ProjectAccess(
-            user_id = user.id,
-            project_id = project.id,
-            access_level = AccessLevel.ADMIN
+            user_id=user.id, project_id=project.id, access_level=AccessLevel.ADMIN
         )
     )
 
-
     db.session.add(project)
     db.session.commit()
 
     flash("Successfully created project")
     return redirect(url_for("home.dashboard"))
```

### Comparing `Cactool-0.5.7.6/setup.cfg` & `Cactool-0.6.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Cactool
-version = 0.5.7.6
+version = 0.6.0
 description = An easy way to collaboratively code social media posts for manual content and discourse analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Sam Ezeh
 author_email = sam.z.ezeh@gmail.com
 url = https://cactool.github.io
 project_urls = 
@@ -25,14 +25,17 @@
 	Flask_SQLAlchemy
 	passlib >= 1.7
 	Werkzeug
 	waitress
 	Flask-Migrate
 	cryptography >= 36
 	appdirs
+	pyotp
+	qrcode
+	beautifulsoup4
 
 [options.package_data]
 cactool = defaults/config.json, scripts/*, migrations/*, migrations/**/*, templates/*, templates/**/*, static/**/*
 
 [options.entry_points]
 console_scripts = 
 	cactool = cactool:cactool
```

