# Comparing `tmp/aa-standingssync-1.8.1.tar.gz` & `tmp/aa_standingssync-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-standingssync-1.8.1.tar", last modified: Thu Feb 16 18:38:43 2023, max compression
+gzip compressed data, was "aa_standingssync-1.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa-standingssync-1.8.1.tar` & `aa_standingssync-1.9.0.tar`

### file list

```diff
@@ -1,71 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 18:38:43.839253 aa-standingssync-1.8.1/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2021-01-09 22:56:20.000000 aa-standingssync-1.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      312 2022-06-18 17:46:09.000000 aa-standingssync-1.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8921 2023-02-16 18:38:43.839253 aa-standingssync-1.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7986 2023-02-12 17:44:30.000000 aa-standingssync-1.8.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 18:38:43.819253 aa-standingssync-1.8.1/aa_standingssync.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8921 2023-02-16 18:38:43.000000 aa-standingssync-1.8.1/aa_standingssync.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1801 2023-02-16 18:38:43.000000 aa-standingssync-1.8.1/aa_standingssync.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-16 18:38:43.000000 aa-standingssync-1.8.1/aa_standingssync.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2023-02-16 18:38:43.000000 aa-standingssync-1.8.1/aa_standingssync.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-02-16 18:38:43.000000 aa-standingssync-1.8.1/aa_standingssync.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-16 18:38:43.839253 aa-standingssync-1.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1634 2023-02-15 12:07:48.000000 aa-standingssync-1.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 18:38:43.827253 aa-standingssync-1.8.1/standingssync/
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-02-16 17:26:02.000000 aa-standingssync-1.8.1/standingssync/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7598 2023-02-16 17:26:02.000000 aa-standingssync-1.8.1/standingssync/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     1981 2023-02-10 11:25:58.000000 aa-standingssync-1.8.1/standingssync/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      218 2021-08-05 18:01:47.000000 aa-standingssync-1.8.1/standingssync/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-02-13 14:31:15.000000 aa-standingssync-1.8.1/standingssync/auth_hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 18:38:43.831253 aa-standingssync-1.8.1/standingssync/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-06 16:53:27.000000 aa-standingssync-1.8.1/standingssync/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6458 2023-02-15 12:07:48.000000 aa-standingssync-1.8.1/standingssync/core/esi_api.py
--rw-rw-rw-   0 root         (0) root         (0)    10307 2023-02-15 12:07:48.000000 aa-standingssync-1.8.1/standingssync/core/esi_contacts.py
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-02-09 09:33:51.000000 aa-standingssync-1.8.1/standingssync/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 18:38:43.815253 aa-standingssync-1.8.1/standingssync/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 18:38:43.831253 aa-standingssync-1.8.1/standingssync/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)     1331 2022-08-02 17:14:17.000000 aa-standingssync-1.8.1/standingssync/management/commands/standingssync_calc_war_ids.py
--rw-rw-rw-   0 root         (0) root         (0)     7701 2023-02-14 18:56:39.000000 aa-standingssync-1.8.1/standingssync/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 18:38:43.831253 aa-standingssync-1.8.1/standingssync/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     6919 2022-08-08 16:33:54.000000 aa-standingssync-1.8.1/standingssync/migrations/0001_initial_new_2.py
--rw-rw-rw-   0 root         (0) root         (0)     3426 2023-02-10 13:31:27.000000 aa-standingssync-1.8.1/standingssync/migrations/0002_improve_sync_logic.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-09 22:56:20.000000 aa-standingssync-1.8.1/standingssync/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17643 2023-02-15 12:07:48.000000 aa-standingssync-1.8.1/standingssync/models.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2022-06-18 17:46:09.000000 aa-standingssync-1.8.1/standingssync/providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 18:38:43.815253 aa-standingssync-1.8.1/standingssync/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 18:38:43.831253 aa-standingssync-1.8.1/standingssync/static/standingssync/
--rw-rw-rw-   0 root         (0) root         (0)     1217 2023-02-13 14:31:15.000000 aa-standingssync-1.8.1/standingssync/static/standingssync/base.css
--rw-rw-rw-   0 root         (0) root         (0)   887006 2022-06-18 17:46:09.000000 aa-standingssync-1.8.1/standingssync/swagger.json
--rw-rw-rw-   0 root         (0) root         (0)     2892 2023-02-15 12:07:48.000000 aa-standingssync-1.8.1/standingssync/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 18:38:43.819253 aa-standingssync-1.8.1/standingssync/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 18:38:43.815253 aa-standingssync-1.8.1/standingssync/templates/admin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 18:38:43.819253 aa-standingssync-1.8.1/standingssync/templates/admin/standingssync/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 18:38:43.831253 aa-standingssync-1.8.1/standingssync/templates/admin/standingssync/evewar/
--rw-rw-rw-   0 root         (0) root         (0)      281 2023-02-10 12:48:03.000000 aa-standingssync-1.8.1/standingssync/templates/admin/standingssync/evewar/change_list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 18:38:43.831253 aa-standingssync-1.8.1/standingssync/templates/standingssync/
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-02-13 21:46:35.000000 aa-standingssync-1.8.1/standingssync/templates/standingssync/_base.html
--rw-rw-rw-   0 root         (0) root         (0)     5546 2023-02-15 12:07:48.000000 aa-standingssync-1.8.1/standingssync/templates/standingssync/characters.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 18:38:43.835253 aa-standingssync-1.8.1/standingssync/templates/standingssync/partial/
--rw-rw-rw-   0 root         (0) root         (0)     1702 2023-02-13 21:46:35.000000 aa-standingssync-1.8.1/standingssync/templates/standingssync/partial/menu.html
--rw-rw-rw-   0 root         (0) root         (0)      204 2023-02-16 17:26:02.000000 aa-standingssync-1.8.1/standingssync/templates/standingssync/partial/war_participant.html
--rw-rw-rw-   0 root         (0) root         (0)     4939 2023-02-15 21:09:12.000000 aa-standingssync-1.8.1/standingssync/templates/standingssync/wars.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 18:38:43.835253 aa-standingssync-1.8.1/standingssync/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-13 21:46:35.000000 aa-standingssync-1.8.1/standingssync/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      972 2023-02-16 17:26:02.000000 aa-standingssync-1.8.1/standingssync/templatetags/standingssync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 18:38:43.839253 aa-standingssync-1.8.1/standingssync/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-04 14:13:04.000000 aa-standingssync-1.8.1/standingssync/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 18:38:43.839253 aa-standingssync-1.8.1/standingssync/tests/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-06 16:53:27.000000 aa-standingssync-1.8.1/standingssync/tests/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7050 2023-02-15 12:07:48.000000 aa-standingssync-1.8.1/standingssync/tests/core/test_esi_api.py
--rw-rw-rw-   0 root         (0) root         (0)    15744 2023-02-15 12:07:49.000000 aa-standingssync-1.8.1/standingssync/tests/core/test_esi_contacts.py
--rw-rw-rw-   0 root         (0) root         (0)     5220 2023-02-14 13:34:04.000000 aa-standingssync-1.8.1/standingssync/tests/factories.py
--rw-rw-rw-   0 root         (0) root         (0)      856 2023-02-16 17:26:02.000000 aa-standingssync-1.8.1/standingssync/tests/test_admin.py
--rw-rw-rw-   0 root         (0) root         (0)    10210 2023-02-15 20:59:45.000000 aa-standingssync-1.8.1/standingssync/tests/test_integration.py
--rw-rw-rw-   0 root         (0) root         (0)    20716 2023-02-14 13:34:04.000000 aa-standingssync-1.8.1/standingssync/tests/test_managers.py
--rw-rw-rw-   0 root         (0) root         (0)    35053 2023-02-15 12:12:44.000000 aa-standingssync-1.8.1/standingssync/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     8531 2023-02-12 17:44:30.000000 aa-standingssync-1.8.1/standingssync/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1412 2023-02-16 17:26:02.000000 aa-standingssync-1.8.1/standingssync/tests/test_templatetags.py
--rw-rw-rw-   0 root         (0) root         (0)    11783 2023-02-13 14:31:15.000000 aa-standingssync-1.8.1/standingssync/tests/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)    11894 2023-02-15 12:07:49.000000 aa-standingssync-1.8.1/standingssync/tests/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      605 2023-02-13 21:46:35.000000 aa-standingssync-1.8.1/standingssync/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     9924 2023-02-15 20:59:45.000000 aa-standingssync-1.8.1/standingssync/views.py
+-rw-r--r--   0        0        0     1070 2023-07-01 13:11:08.839238 aa_standingssync-1.9.0/LICENSE
+-rw-r--r--   0        0        0     7854 2023-07-01 13:11:08.839238 aa_standingssync-1.9.0/README.md
+-rw-r--r--   0        0        0     1725 2023-07-01 13:11:08.839238 aa_standingssync-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      197 2023-07-01 13:11:08.839238 aa_standingssync-1.9.0/standingssync/__init__.py
+-rw-r--r--   0        0        0     7697 2023-07-01 15:08:56.087378 aa_standingssync-1.9.0/standingssync/admin.py
+-rw-r--r--   0        0        0     2022 2023-07-01 14:34:00.250443 aa_standingssync-1.9.0/standingssync/app_settings.py
+-rw-r--r--   0        0        0      218 2023-07-01 13:11:08.839238 aa_standingssync-1.9.0/standingssync/apps.py
+-rw-r--r--   0        0        0      952 2023-07-01 13:11:08.839238 aa_standingssync-1.9.0/standingssync/auth_hooks.py
+-rw-r--r--   0        0        0        0 2023-07-01 18:16:48.926772 aa_standingssync-1.9.0/standingssync/core/__init__.py
+-rw-r--r--   0        0        0     6481 2023-07-01 14:34:00.250443 aa_standingssync-1.9.0/standingssync/core/esi_api.py
+-rw-r--r--   0        0        0    10868 2023-07-01 14:34:00.250443 aa_standingssync-1.9.0/standingssync/core/esi_contacts.py
+-rw-r--r--   0        0        0      292 2023-07-01 14:34:00.250443 aa_standingssync-1.9.0/standingssync/helpers.py
+-rw-r--r--   0        0        0     1331 2023-07-01 13:11:08.843238 aa_standingssync-1.9.0/standingssync/management/commands/standingssync_calc_war_ids.py
+-rw-r--r--   0        0        0     7700 2023-07-01 14:34:00.250443 aa_standingssync-1.9.0/standingssync/managers.py
+-rw-r--r--   0        0        0     6918 2023-07-01 13:11:08.843238 aa_standingssync-1.9.0/standingssync/migrations/0001_initial_new_2.py
+-rw-r--r--   0        0        0     3426 2023-07-01 13:11:08.843238 aa_standingssync-1.9.0/standingssync/migrations/0002_improve_sync_logic.py
+-rw-r--r--   0        0        0        0 2023-07-01 18:16:48.926772 aa_standingssync-1.9.0/standingssync/migrations/__init__.py
+-rw-r--r--   0        0        0    18056 2023-07-01 18:03:46.630191 aa_standingssync-1.9.0/standingssync/models.py
+-rw-r--r--   0        0        0      181 2023-07-01 14:34:00.250443 aa_standingssync-1.9.0/standingssync/providers.py
+-rw-r--r--   0        0        0     1217 2023-07-01 13:11:08.843238 aa_standingssync-1.9.0/standingssync/static/standingssync/base.css
+-rw-r--r--   0        0        0     2924 2023-07-01 14:34:00.254443 aa_standingssync-1.9.0/standingssync/tasks.py
+-rw-r--r--   0        0        0      281 2023-07-01 13:11:08.843238 aa_standingssync-1.9.0/standingssync/templates/admin/standingssync/evewar/change_list.html
+-rw-r--r--   0        0        0      429 2023-07-01 13:11:08.843238 aa_standingssync-1.9.0/standingssync/templates/standingssync/_base.html
+-rw-r--r--   0        0        0     5546 2023-07-01 13:11:08.843238 aa_standingssync-1.9.0/standingssync/templates/standingssync/characters.html
+-rw-r--r--   0        0        0     1702 2023-07-01 13:11:08.843238 aa_standingssync-1.9.0/standingssync/templates/standingssync/partial/menu.html
+-rw-r--r--   0        0        0      204 2023-07-01 13:11:08.843238 aa_standingssync-1.9.0/standingssync/templates/standingssync/partial/war_participant.html
+-rw-r--r--   0        0        0     4939 2023-07-01 13:11:08.843238 aa_standingssync-1.9.0/standingssync/templates/standingssync/wars.html
+-rw-r--r--   0        0        0        0 2023-07-01 18:16:48.926772 aa_standingssync-1.9.0/standingssync/templatetags/__init__.py
+-rw-r--r--   0        0        0      986 2023-07-01 18:03:46.630191 aa_standingssync-1.9.0/standingssync/templatetags/standingssync.py
+-rw-r--r--   0        0        0        0 2023-07-01 18:16:48.926772 aa_standingssync-1.9.0/standingssync/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 18:16:48.926772 aa_standingssync-1.9.0/standingssync/tests/core/__init__.py
+-rw-r--r--   0        0        0     7050 2023-07-01 13:11:08.843238 aa_standingssync-1.9.0/standingssync/tests/core/test_esi_api.py
+-rw-r--r--   0        0        0    17823 2023-07-01 14:34:00.254443 aa_standingssync-1.9.0/standingssync/tests/core/test_esi_contacts.py
+-rw-r--r--   0        0        0     6253 2023-07-01 14:34:00.254443 aa_standingssync-1.9.0/standingssync/tests/factories.py
+-rw-r--r--   0        0        0      856 2023-07-01 13:11:08.843238 aa_standingssync-1.9.0/standingssync/tests/test_admin.py
+-rw-r--r--   0        0        0    10222 2023-07-01 18:03:46.630191 aa_standingssync-1.9.0/standingssync/tests/test_integration.py
+-rw-r--r--   0        0        0    20729 2023-07-01 18:03:46.630191 aa_standingssync-1.9.0/standingssync/tests/test_managers.py
+-rw-r--r--   0        0        0    35633 2023-07-01 18:03:46.630191 aa_standingssync-1.9.0/standingssync/tests/test_models.py
+-rw-r--r--   0        0        0     8561 2023-07-01 18:03:46.630191 aa_standingssync-1.9.0/standingssync/tests/test_tasks.py
+-rw-r--r--   0        0        0     1822 2023-07-01 18:03:46.630191 aa_standingssync-1.9.0/standingssync/tests/test_templatetags.py
+-rw-r--r--   0        0        0    12054 2023-07-01 18:03:46.630191 aa_standingssync-1.9.0/standingssync/tests/test_views.py
+-rw-r--r--   0        0        0    11894 2023-07-01 13:11:08.843238 aa_standingssync-1.9.0/standingssync/tests/utils.py
+-rw-r--r--   0        0        0      638 2023-07-01 14:34:00.254443 aa_standingssync-1.9.0/standingssync/urls.py
+-rw-r--r--   0        0        0     9927 2023-07-01 18:03:46.630191 aa_standingssync-1.9.0/standingssync/views.py
+-rw-r--r--   0        0        0     8910 1970-01-01 00:00:00.000000 aa_standingssync-1.9.0/PKG-INFO
```

### Comparing `aa-standingssync-1.8.1/LICENSE` & `aa_standingssync-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-standingssync-1.8.1/PKG-INFO` & `aa_standingssync-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: aa-standingssync
-Version: 1.8.1
-Summary: Standing sync for non-alliance characters - app for for Alliance Auth
-Home-page: https://gitlab.com/ErikKalkoken/aa-standingssync
-Author: Erik Kalkoken
-Author-email: kalkoken87@gmail.com
-License: MIT
-Platform: UNKNOWN
+Version: 1.9.0
+Summary: Alliance Auth app for cloning alliance standings and war targets to alts.
+Author-email: Erik Kalkoken <kalkoken87@gmail.com>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Requires-Dist: allianceauth-app-utils>=1.19
+Requires-Dist: allianceauth>=3
+Requires-Dist: django-eveuniverse>=1.2
+Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-standingssync
 
 # Standings Sync
 
-This is a plugin app for [Alliance Auth](https://gitlab.com/allianceauth/allianceauth), which enables non-alliance characters like scout alts to have the same standings view in game as their alliance main.
+Alliance Auth app for cloning alliance standings and war targets to alts.
 
 [![release](https://img.shields.io/pypi/v/aa-standingssync?label=release)](https://pypi.org/project/aa-standingssync/)
 [![python](https://img.shields.io/pypi/pyversions/aa-standingssync)](https://pypi.org/project/aa-standingssync/)
 [![django](https://img.shields.io/pypi/djversions/aa-standingssync?label=django)](https://pypi.org/project/aa-standingssync/)
 [![pipeline](https://gitlab.com/ErikKalkoken/aa-standingssync/badges/master/pipeline.svg)](https://gitlab.com/ErikKalkoken/aa-standingssync/-/pipelines)
 [![codecov](https://codecov.io/gl/ErikKalkoken/aa-standingssync/branch/master/graph/badge.svg?token=gHBi42fbSs)](https://codecov.io/gl/ErikKalkoken/aa-standingssync)
 [![license](https://img.shields.io/badge/license-MIT-green)](https://gitlab.com/ErikKalkoken/aa-standingssync/-/blob/master/LICENSE)
@@ -195,8 +195,7 @@
 
 - Manually start the sync process for characters / alliances
 
 ## Feedback
 
 If you encounter any bugs or would like to request a new feature please open an issue in this gitlab repo.
 
-
```

### Comparing `aa-standingssync-1.8.1/README.md` & `aa_standingssync-1.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Standings Sync
 
-This is a plugin app for [Alliance Auth](https://gitlab.com/allianceauth/allianceauth), which enables non-alliance characters like scout alts to have the same standings view in game as their alliance main.
+Alliance Auth app for cloning alliance standings and war targets to alts.
 
 [![release](https://img.shields.io/pypi/v/aa-standingssync?label=release)](https://pypi.org/project/aa-standingssync/)
 [![python](https://img.shields.io/pypi/pyversions/aa-standingssync)](https://pypi.org/project/aa-standingssync/)
 [![django](https://img.shields.io/pypi/djversions/aa-standingssync?label=django)](https://pypi.org/project/aa-standingssync/)
 [![pipeline](https://gitlab.com/ErikKalkoken/aa-standingssync/badges/master/pipeline.svg)](https://gitlab.com/ErikKalkoken/aa-standingssync/-/pipelines)
 [![codecov](https://codecov.io/gl/ErikKalkoken/aa-standingssync/branch/master/graph/badge.svg?token=gHBi42fbSs)](https://codecov.io/gl/ErikKalkoken/aa-standingssync)
 [![license](https://img.shields.io/badge/license-MIT-green)](https://gitlab.com/ErikKalkoken/aa-standingssync/-/blob/master/LICENSE)
```

### Comparing `aa-standingssync-1.8.1/standingssync/admin.py` & `aa_standingssync-1.9.0/standingssync/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Admin site for standingssync."""
+
 from django.contrib import admin
 from django.db.models import Prefetch
 from eveuniverse.models import EveEntity
 
 from . import tasks
 from .models import EveContact, EveWar, SyncedCharacter, SyncManager
 
@@ -100,15 +102,15 @@
     def has_add_permission(self, *args, **kwargs):
         return False
 
     def has_change_permission(self, *args, **kwargs) -> bool:
         return False
 
     def get_queryset(self, request):
-        qs = super().get_queryset(request).annotate_state().annotate_is_active()
+        qs = super().get_queryset(request).annotate_state().annotate_is_active()  # type: ignore
         return qs.prefetch_related(
             Prefetch("allies", queryset=EveEntity.objects.select_related())
         ).annotate_state()
 
     def _state(self, obj) -> str:
         return EveWar.State(obj.state).label
 
@@ -209,15 +211,18 @@
 
     @admin.display(ordering="character_ownership__user__username")
     def _user(self, obj):
         return obj.character_ownership.user if obj.character_ownership else None
 
     @admin.display(ordering="character_ownership__character__character_name")
     def _character_name(self, obj):
-        return obj.character_ownership.character.character_name
+        try:
+            return obj.character.character_name
+        except ValueError:
+            return ""
 
     @admin.display(ordering="alliance__alliance_name")
     def _alliance_name(self, obj):
         return obj.alliance.alliance_name
 
     @admin.display(description="Alliance contacts")
     def _alliance_contacts_count(self, obj):
```

### Comparing `aa-standingssync-1.8.1/standingssync/app_settings.py` & `aa_standingssync-1.9.0/standingssync/app_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from app_utils.django import clean_setting
+"""Settings for standingssync."""
+
+from app_utils.app_settings import clean_setting
 
 STANDINGSSYNC_ADD_WAR_TARGETS = clean_setting("STANDINGSSYNC_ADD_WAR_TARGETS", False)
 """When enabled will automatically add or set war targets
  with standing = -10 to synced characters.
 """
 
 STANDINGSSYNC_CHAR_MIN_STANDING = clean_setting(
```

### Comparing `aa-standingssync-1.8.1/standingssync/auth_hooks.py` & `aa_standingssync-1.9.0/standingssync/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-standingssync-1.8.1/standingssync/core/esi_api.py` & `aa_standingssync-1.9.0/standingssync/core/esi_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Wrapper for handling all access to the ESI API."""
 
 from collections import defaultdict
-from typing import Callable, Dict, FrozenSet, Iterable, List, Set
+from typing import Callable, Dict, FrozenSet, Iterable, Optional, Set
 
 from esi.models import Token
 
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.helpers import chunks
 from app_utils.logging import LoggerAddTag
 
@@ -110,15 +110,15 @@
         )
 
 
 def _update_character_contacts_esi(
     token: Token,
     contacts_by_standing: Dict[float, Iterable[int]],
     esi_method: Callable,
-    label_ids: list = None,
+    label_ids: Optional[list] = None,
 ) -> None:
     """Add new or update existing character contacts on ESI."""
     max_items = 100
     for standing in contacts_by_standing:
         contact_ids = sorted(list(contacts_by_standing[standing]))
         for contact_ids_chunk in chunks(contact_ids, max_items):
             params = {
@@ -129,16 +129,16 @@
             }
             if label_ids is not None:
                 params["label_ids"] = sorted(list(label_ids))
             esi_method(**params).results()
 
 
 def _group_for_esi_update(
-    contacts: List["EsiContact"],
-) -> Dict[FrozenSet, Dict[float, Set[int]]]:
+    contacts: Iterable["EsiContact"],
+) -> Dict[FrozenSet, Dict[float, Iterable[int]]]:
     """Group contacts for ESI update."""
     contacts_grouped = dict()
     for contact in contacts:
         if contact.label_ids not in contacts_grouped:
             contacts_grouped[contact.label_ids] = defaultdict(set)
         contacts_grouped[contact.label_ids][contact.standing].add(contact.contact_id)
     return contacts_grouped
```

### Comparing `aa-standingssync-1.8.1/standingssync/core/esi_contacts.py` & `aa_standingssync-1.9.0/standingssync/core/esi_contacts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+"""Core logic for handling ESI contacts."""
+
 import hashlib
 import json
 from copy import deepcopy
 from dataclasses import dataclass, field, fields
 from enum import Enum
-from typing import Dict, FrozenSet, Iterable, List, Optional, Set, Tuple
+from typing import Any, Dict, FrozenSet, Iterable, List, Optional, Set, Tuple
 
 from eveuniverse.models import EveEntity
 
 from standingssync.app_settings import STANDINGSSYNC_WAR_TARGETS_LABEL_NAME
 
 
 @dataclass(frozen=True)
@@ -33,24 +35,28 @@
 
 
 @dataclass(frozen=True)
 class EsiContact:
     """An ESI contact. Immutable."""
 
     class ContactType(str, Enum):
+        """A contact type."""
+
+        ALLIANCE = "alliance"
         CHARACTER = "character"
         CORPORATION = "corporation"
-        ALLIANCE = "alliance"
+        FACTION = "faction"
 
         @classmethod
         def from_esi_contact_type(cls, contact_type) -> "EsiContact.ContactType":
             mapper = {
+                "alliance": cls.ALLIANCE,
                 "character": cls.CHARACTER,
                 "corporation": cls.CORPORATION,
-                "alliance": cls.ALLIANCE,
+                "faction": cls.FACTION,
             }
             return mapper[contact_type]
 
     contact_id: int
     contact_type: ContactType
     standing: float
     label_ids: FrozenSet[int] = field(default_factory=frozenset)
@@ -77,53 +83,59 @@
         }
         if self.label_ids:
             obj["label_ids"] = sorted(list(self.label_ids))
         return obj
 
     @classmethod
     def from_esi_dict(cls, esi_dict: dict) -> "EsiContact":
+        """Create new objects from an ESI contact."""
         return cls(
             contact_id=esi_dict["contact_id"],
             contact_type=EsiContact.ContactType.from_esi_contact_type(
                 esi_dict["contact_type"]
             ),
             standing=esi_dict["standing"],
-            label_ids=esi_dict.get("label_ids") or [],
+            label_ids=esi_dict.get("label_ids") or frozenset(),
         )
 
     @classmethod
     def from_eve_entity(
         cls, eve_entity: EveEntity, standing: float, label_ids=None
     ) -> "EsiContact":
         """Create new instance from an EveEntity object."""
         contact_type_map = {
             EveEntity.CATEGORY_ALLIANCE: cls.ContactType.ALLIANCE,
             EveEntity.CATEGORY_CHARACTER: cls.ContactType.CHARACTER,
             EveEntity.CATEGORY_CORPORATION: cls.ContactType.CORPORATION,
+            EveEntity.CATEGORY_FACTION: cls.ContactType.FACTION,
         }
+        if eve_entity.category not in contact_type_map:
+            raise ValueError(
+                f"{eve_entity}: Can not create from eve entity without category"
+            )
         return cls(
             contact_id=eve_entity.id,
             contact_type=contact_type_map[eve_entity.category],
             standing=standing,
-            label_ids=label_ids if label_ids else [],
+            label_ids=label_ids if label_ids else frozenset(),
         )
 
     @classmethod
-    def from_eve_contact(cls, eve_contact: object, label_ids=None) -> "EsiContact":
+    def from_eve_contact(cls, eve_contact: Any, label_ids=None) -> "EsiContact":
         """Create new instance from an EveContact object."""
         contact_type_map = {
             EveEntity.CATEGORY_ALLIANCE: cls.ContactType.ALLIANCE,
             EveEntity.CATEGORY_CHARACTER: cls.ContactType.CHARACTER,
             EveEntity.CATEGORY_CORPORATION: cls.ContactType.CORPORATION,
         }
         return cls(
             contact_id=eve_contact.eve_entity.id,
             contact_type=contact_type_map[eve_contact.eve_entity.category],
             standing=eve_contact.standing,
-            label_ids=label_ids if label_ids else [],
+            label_ids=label_ids if label_ids else frozenset(),
         )
 
 
 @dataclass
 class EsiContactsContainer:
     """Container of ESI contacts with their labels."""
 
@@ -144,15 +156,17 @@
             label_ids = {
                 label_id for label_id in contact.label_ids if label_id in self._labels
             }
         else:
             label_ids = []
         self._contacts[contact.contact_id] = contact.clone(label_ids=label_ids)
 
-    def add_eve_contacts(self, contacts: List[object], label_ids: List[int] = None):
+    def add_eve_contacts(
+        self, contacts: Iterable[object], label_ids: Optional[List[int]] = None
+    ):
         for contact in contacts:
             self.add_contact(EsiContact.from_eve_contact(contact, label_ids=label_ids))
 
     def remove_contact(self, contact: EsiContact):
         """Remove contact."""
         try:
             del self._contacts[contact.contact_id]
@@ -170,29 +184,29 @@
         """Returns contact by it's ID.
 
         Raises ValueError when contact is not found.
         """
         try:
             return self._contacts[contact_id]
         except KeyError:
-            raise ValueError(f"Contact with ID {contact_id} not found.")
+            raise ValueError(f"Contact with ID {contact_id} not found.") from None
 
     def contacts(self) -> Set[EsiContact]:
         """Fetch all contacts."""
         return set(self._contacts.values())
 
     def label_by_id(self, label_id) -> EsiContactLabel:
         """Returns label by it's ID.
 
         Raises ValueError when label is not found.
         """
         try:
             return self._labels[label_id]
         except KeyError:
-            raise ValueError(f"Label with ID {label_id} not found.")
+            raise ValueError(f"Label with ID {label_id} not found.") from None
 
     def labels(self) -> Set[EsiContactLabel]:
         """Fetch all labels."""
         return set(self._labels.values())
 
     def war_target_label_id(self) -> Optional[int]:
         """Fetch the ID of the configured war target label."""
@@ -263,32 +277,32 @@
         """Calculate hash for current contacts & label in order to identify changes."""
         data = self._to_dict()
         return hashlib.md5(json.dumps(data).encode("utf-8")).hexdigest()
 
     @classmethod
     def from_esi_contacts(
         cls,
-        contacts: Iterable[EsiContact] = None,
-        labels: Iterable[EsiContactLabel] = None,
+        contacts: Optional[Iterable[EsiContact]] = None,
+        labels: Optional[Iterable[EsiContactLabel]] = None,
     ) -> "EsiContactsContainer":
         """Create new object from Esi contacts."""
         obj = cls()
         if labels:
             for label in labels:
                 obj.add_label(label)
         if contacts:
             for contact in contacts:
                 obj.add_contact(contact)
         return obj
 
     @classmethod
     def from_esi_dicts(
         cls,
-        contacts: Iterable[dict] = None,
-        labels: Iterable[dict] = None,
+        contacts: Optional[Iterable[dict]] = None,
+        labels: Optional[Iterable[dict]] = None,
     ) -> "EsiContactsContainer":
         """Create new object from ESI contacts and labels."""
         obj = cls()
         if labels:
             for label in labels:
                 obj.add_label(EsiContactLabel.from_esi_dict(label))
         if contacts:
```

### Comparing `aa-standingssync-1.8.1/standingssync/management/commands/standingssync_calc_war_ids.py` & `aa_standingssync-1.9.0/standingssync/management/commands/standingssync_calc_war_ids.py`

 * *Files identical despite different names*

### Comparing `aa-standingssync-1.8.1/standingssync/managers.py` & `aa_standingssync-1.9.0/standingssync/managers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+"""Managers for standingssync."""
+
 import datetime as dt
 from collections import defaultdict
-from typing import Dict, Optional, Set, Tuple
+from typing import Any, Dict, Set, Tuple
 
 from django.contrib.auth.models import User
 from django.db import models, transaction
 from django.db.models import Case, Value, When
 from django.utils.timezone import now
 from eveuniverse.models import EveEntity
 
@@ -15,15 +17,15 @@
 from . import __title__
 from .core import esi_api
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 class EveContactQuerySet(models.QuerySet):
-    def grouped_by_standing(self) -> Dict[int, models.Model]:
+    def grouped_by_standing(self) -> Dict[int, Any]:
         """Group alliance contacts by standing and convert into sorted dict."""
         contacts_by_standing = defaultdict(set)
         for contact in self.all():
             contacts_by_standing[contact.standing].add(contact)
         return dict(sorted(contacts_by_standing.items()))
 
 
@@ -62,15 +64,15 @@
             )
         )
 
     def annotate_is_active(self) -> models.QuerySet:
         """Add is_active field to queryset. Requires prior annotation of state."""
         return self.annotate(
             is_active=Case(
-                When(state__in=self.model.State.active_states, then=Value(True)),
+                When(state__in=self.model.State.active_states(), then=Value(True)),
                 default=Value(False),
             )
         )
 
     def current_wars(self) -> models.QuerySet:
         """Filter for current wars.
 
@@ -120,15 +122,15 @@
 
             # case 3 alliance is ally
             if war.allies.filter(id=alliance.alliance_id).exists():
                 war_target_ids.add(war.aggressor_id)
 
         return EveEntity.objects.filter(id__in=war_target_ids)
 
-    def update_or_create_from_esi(self, id: int) -> Tuple[models.Model, bool]:
+    def update_or_create_from_esi(self, id: int) -> Tuple[Any, bool]:
         """Updates existing or creates new objects from ESI with given ID."""
 
         logger.info("Retrieving war details for ID %s", id)
         entity_ids = set()
         war_info = esi_api.fetch_war(war_id=id)
         aggressor = self._get_or_create_eve_entity_from_participant(
             war_info["aggressor"]
@@ -148,15 +150,15 @@
                     "retracted": war_info.get("retracted"),
                     "started": war_info.get("started"),
                     "finished": war_info.get("finished"),
                 },
             )
             war.allies.clear()
             if war_info.get("allies"):
-                for ally_info in war_info.get("allies"):
+                for ally_info in war_info.get("allies", []):
                     try:
                         ally = self._get_or_create_eve_entity_from_participant(
                             ally_info
                         )
                     except ValueError:
                         logger.warning("%s: Could not identify ally: ", id, ally_info)
                         continue
@@ -183,15 +185,15 @@
         return war_ids.difference(finished_war_ids)
 
 
 EveWarManager = EveWarManagerBase.from_queryset(EveWarQuerySet)
 
 
 class SyncManagerManager(models.Manager):
-    def fetch_for_user(self, user: User) -> Optional[models.Model]:
+    def fetch_for_user(self, user: User) -> Any:
         """Fetch sync manager for given user. Return None if no match is found."""
         if not user.profile.main_character:
             return None
         try:
             alliance = EveAllianceInfo.objects.get(
                 alliance_id=user.profile.main_character.alliance_id
             )
```

### Comparing `aa-standingssync-1.8.1/standingssync/migrations/0001_initial_new_2.py` & `aa_standingssync-1.9.0/standingssync/migrations/0001_initial_new_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 4.0.7 on 2022-08-08 16:09
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     replaces = [
         ("standingssync", "0001_initial-new"),
         ("standingssync", "0002_add_war_targets"),
         ("standingssync", "0003_war_target_labels"),
         ("standingssync", "0004_remove_old_eve_entity"),
         ("standingssync", "0005_add_new_eve_entity"),
     ]
```

### Comparing `aa-standingssync-1.8.1/standingssync/migrations/0002_improve_sync_logic.py` & `aa_standingssync-1.9.0/standingssync/migrations/0002_improve_sync_logic.py`

 * *Files identical despite different names*

### Comparing `aa-standingssync-1.8.1/standingssync/models.py` & `aa_standingssync-1.9.0/standingssync/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+"""Models for standingssync."""
+
 import datetime as dt
 from typing import Optional, Set
 
 from django.conf import settings
 from django.contrib.auth.models import User
-from django.core.exceptions import ObjectDoesNotExist
 from django.db import models, transaction
-from django.utils.functional import classproperty
 from django.utils.timezone import now
 from esi.errors import TokenExpiredError, TokenInvalidError
 from esi.models import Token
 from eveuniverse.models import EveEntity
 
 from allianceauth.authentication.models import CharacterOwnership
 from allianceauth.eveonline.models import EveAllianceInfo, EveCharacter
@@ -81,14 +81,21 @@
     )
 
     objects = SyncManagerManager()
 
     def __str__(self):
         return str(self.alliance)
 
+    @property
+    def character(self) -> EveCharacter:
+        """Return character linked to this manager or raises exception of none exists."""
+        if not self.character_ownership:
+            raise ValueError("No character ownership")
+        return self.character_ownership.character
+
     def contacts_for_sync(self, synced_character: "SyncedCharacter") -> models.QuerySet:
         """Relevant contacts for sync, which excludes the sync character."""
         return self.contacts.exclude(eve_entity_id=synced_character.character_id)
 
     def effective_standing_with_character(self, character: EveCharacter) -> float:
         """Effective standing of the alliance with a character."""
         try:
@@ -120,33 +127,36 @@
         """
         if self.character_ownership is None:
             raise RuntimeError(f"{self}: Can not sync. No character configured.")
         if not self.character_ownership.user.has_perm("standingssync.add_syncmanager"):
             raise RuntimeError(
                 f"{self}: Can not sync. Character does not have sufficient permission."
             )
-        token = self._fetch_token()
+        token = self.fetch_token()
         if not token:
             raise RuntimeError(f"{self}: Can not sync. No valid token found.")
         contacts = esi_api.fetch_alliance_contacts(self.alliance.alliance_id, token)
         current_contacts = EsiContactsContainer.from_esi_contacts(contacts)
         war_target_ids = self._add_war_targets(current_contacts)
         new_version_hash = current_contacts.version_hash()
         if force_update or new_version_hash != self.version_hash:
             self._save_new_contacts(current_contacts, war_target_ids, new_version_hash)
         else:
             logger.info("%s: Alliance contacts are unchanged.", self)
         self.record_successful_sync()
 
-    def _fetch_token(self) -> Token:
+    def fetch_token(self) -> Optional[Token]:
         """Fetch valid token with required scopes."""
+        if not self.character_ownership:
+            return None
+
         token = (
             Token.objects.filter(
                 user=self.character_ownership.user,
-                character_id=self.character_ownership.character.character_id,
+                character_id=self.character.character_id,
             )
             .require_scopes(self.get_esi_scopes())
             .require_valid()
             .first()
         )
         return token
 
@@ -158,15 +168,15 @@
         if not STANDINGSSYNC_ADD_WAR_TARGETS:
             return set()
         war_targets = EveWar.objects.alliance_war_targets(self.alliance)
         war_target_ids = set()
         for war_target in war_targets:
             try:
                 contacts.add_contact(EsiContact.from_eve_entity(war_target, -10.0))
-            except KeyError:  # eve_entity has no category
+            except ValueError:  # eve_entity has no category
                 logger.warning("Skipping unresolved war target: %s", war_target)
             else:
                 war_target_ids.add(war_target.id)
         return war_target_ids
 
     def _save_new_contacts(
         self,
@@ -214,29 +224,26 @@
         help_text="Whether this character has the war target label.",
     )
     manager = models.ForeignKey(
         SyncManager, on_delete=models.CASCADE, related_name="synced_characters"
     )
 
     def __str__(self):
-        try:
-            character_name = self.character_ownership.character.character_name
-        except ObjectDoesNotExist:
-            character_name = f"[{self.pk}]"
+        character_name = self.character_ownership.character.character_name
         return f"{character_name} - {self.manager}"
 
     @property
     def character(self) -> EveCharacter:
         return self.character_ownership.character
 
     @property
-    def character_id(self) -> int:
-        return self.character.character_id
+    def character_id(self) -> Optional[int]:
+        return self.character.character_id if self.character else None
 
-    def run_sync(self) -> bool:
+    def run_sync(self) -> Optional[bool]:
         """Sync in-game contacts for given character with alliance contacts
         and/or war targets.
 
         Will delete this sync character if necessary,
         e.g. if token is no longer valid or character is no longer blue
 
         Returns:
@@ -245,15 +252,15 @@
         - True when update was done successfully
         """
         logger.info("%s: Updating character", self)
         if not self._has_owner_permissions():
             return False
         if not self._has_standing_with_alliance():
             return False
-        token = self._fetch_token()
+        token = self.fetch_token()
         if not token:
             logger.error("%s: Can not sync. No valid token found.", self)
             return False
         if not self.manager.contacts_for_sync(self).exists():
             logger.info("%s: No contacts to sync", self)
             return None
 
@@ -318,33 +325,37 @@
             logger.info(
                 "%s: sync deactivated due to insufficient user permissions", self
             )
             self._deactivate_sync("you no longer have permission for this service")
             return False
         return True
 
-    def _fetch_token(self) -> Optional[Token]:
+    def fetch_token(self) -> Optional[Token]:
         """Fetch valid token with required scopes.
 
         Will deactivate this character if any severe issues are encountered.
         """
         try:
             token = self._valid_token()
+
         except TokenInvalidError:
             logger.info("%s: sync deactivated due to invalid token", self)
             self._deactivate_sync("your token is no longer valid")
             return None
+
         except TokenExpiredError:
             logger.info("%s: sync deactivated due to expired token", self)
             self._deactivate_sync("your token has expired")
             return None
+
         if token is None:
             logger.info("%s: can not find suitable token for synced char", self)
             self._deactivate_sync("you do not have a token anymore")
             return None
+
         return token
 
     def _valid_token(self) -> Optional[Token]:
         return (
             Token.objects.filter(
                 user=self.character_ownership.user,
                 character_id=self.character_ownership.character.character_id,
@@ -402,14 +413,21 @@
                 "%s: new version hash: %s", self, current_contacts.version_hash()
             )
         return current_contacts
 
     def delete_all_contacts(self):
         """Delete all contacts of this character."""
         token = self._valid_token()
+        if not token:
+            logger.warning(
+                "%s: Can not delete contacts, because no valid token found.",
+                self,
+            )
+            return
+
         contacts_clone = self._fetch_current_contacts(token)
         contacts = contacts_clone.contacts()
         logger.info("%s: Deleting all %d contacts", self, len(contacts))
         esi_api.delete_character_contacts(token, contacts)
 
     @staticmethod
     def get_esi_scopes() -> list:
@@ -447,15 +465,15 @@
     class State(models.TextChoices):
         PENDING = "pending"  # declared, but not started yet
         ONGOING = "ongoing"  # active and without finish date
         CONCLUDING = "concluding"  # active and about to finish normally
         RETRACTED = "retracted"  # activate and about to finish after retraction
         FINISHED = "finished"  # finished war
 
-        @classproperty
+        @classmethod
         def active_states(cls) -> Set["EveWar.State"]:
             return {cls.ONGOING, cls.CONCLUDING, cls.RETRACTED}
 
     id = models.PositiveIntegerField(primary_key=True)
     aggressor = models.ForeignKey(EveEntity, on_delete=models.CASCADE, related_name="+")
     allies = models.ManyToManyField(EveEntity, related_name="+")
     declared = models.DateTimeField()
```

### Comparing `aa-standingssync-1.8.1/standingssync/static/standingssync/base.css` & `aa_standingssync-1.9.0/standingssync/static/standingssync/base.css`

 * *Files identical despite different names*

### Comparing `aa-standingssync-1.8.1/standingssync/tasks.py` & `aa_standingssync-1.9.0/standingssync/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Tasks for standingssync."""
+
 from celery import shared_task
 
 from eveuniverse.core.esitools import is_esi_online
 from eveuniverse.models import EveEntity
 from eveuniverse.tasks import update_unresolved_eve_entities
 
 from allianceauth.services.hooks import get_extension_logger
```

### Comparing `aa-standingssync-1.8.1/standingssync/templates/standingssync/characters.html` & `aa_standingssync-1.9.0/standingssync/templates/standingssync/characters.html`

 * *Files identical despite different names*

### Comparing `aa-standingssync-1.8.1/standingssync/templates/standingssync/partial/menu.html` & `aa_standingssync-1.9.0/standingssync/templates/standingssync/partial/menu.html`

 * *Files identical despite different names*

### Comparing `aa-standingssync-1.8.1/standingssync/templates/standingssync/wars.html` & `aa_standingssync-1.9.0/standingssync/templates/standingssync/wars.html`

 * *Files identical despite different names*

### Comparing `aa-standingssync-1.8.1/standingssync/templatetags/standingssync.py` & `aa_standingssync-1.9.0/standingssync/templatetags/standingssync.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,36 @@
+"""Template tags for standingssync."""
+
 from django import template
 from eveuniverse.core import zkillboard
 from eveuniverse.models import EveEntity
 
 register = template.Library()
 
 
 @register.inclusion_tag("standingssync/partial/war_participant.html")
-def war_participant(obj: EveEntity, icon_size=None) -> str:
+def war_participant(obj: EveEntity, icon_size=None) -> dict:
     """Render war participant with icon, name and link to ZKB."""
     context = {"has_data": False, "icon_size": icon_size or 20}
     try:
         category = obj.category
     except AttributeError:
         return context
-    if category:
-        if obj.is_alliance:
-            profile_url = zkillboard.alliance_url(obj.id)
-        elif obj.is_corporation:
-            profile_url = zkillboard.corporation_url(obj.id)
-        else:
-            profile_url = ""
-        context.update(
-            {
-                "has_data": True,
-                "name": obj.name,
-                "profile_url": profile_url,
-                "icon_url": obj.icon_url(32),
-            }
-        )
+
+    if not category:
+        return context
+
+    if obj.is_alliance:
+        profile_url = zkillboard.alliance_url(obj.id)
+    elif obj.is_corporation:
+        profile_url = zkillboard.corporation_url(obj.id)
+    else:
+        profile_url = ""
+    context.update(
+        {
+            "has_data": True,
+            "name": obj.name,
+            "profile_url": profile_url,
+            "icon_url": obj.icon_url(32),
+        }
+    )
     return context
```

### Comparing `aa-standingssync-1.8.1/standingssync/tests/core/test_esi_api.py` & `aa_standingssync-1.9.0/standingssync/tests/core/test_esi_api.py`

 * *Files identical despite different names*

### Comparing `aa-standingssync-1.8.1/standingssync/tests/core/test_esi_contacts.py` & `aa_standingssync-1.9.0/standingssync/tests/core/test_esi_contacts.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,23 @@
 
 from standingssync.core.esi_contacts import (
     EsiContact,
     EsiContactLabel,
     EsiContactsContainer,
 )
 
-from ..factories import EsiContactFactory, EsiContactLabelFactory, EveContactFactory
+from ..factories import (
+    EsiContactFactory,
+    EsiContactLabelFactory,
+    EveContactFactory,
+    EveEntityAllianceFactory,
+    EveEntityCharacterFactory,
+    EveEntityCorporationFactory,
+    EveEntityFactionFactory,
+)
 
 MODULE_PATH = "standingssync.core.esi_contacts"
 WAR_TARGET_LABEL = "WAR TARGETS"
 
 
 class TestEsiContact(NoSocketsTestCase):
     def test_should_create_new_1(self):
@@ -21,80 +29,120 @@
         # then
         self.assertEqual(obj.contact_id, 1001)
         self.assertEqual(obj.contact_type, EsiContact.ContactType.CHARACTER)
         self.assertEqual(obj.standing, 5.0)
 
     def test_should_create_new_2(self):
         # when
-        obj = EsiContact(1001, "character", 5.0)
+        obj = EsiContact(1001, "character", 5.0)  # type: ignore
         # then
         self.assertEqual(obj.contact_id, 1001)
         self.assertEqual(obj.contact_type, EsiContact.ContactType.CHARACTER)
         self.assertEqual(obj.standing, 5.0)
 
     def test_should_create_new_3(self):
         # when/then
         with self.assertRaises(ValueError):
-            EsiContact(1001, "xyz", 5.0)
+            EsiContact(1001, "xyz", 5.0)  # type: ignore
+
+    def test_should_create_all_types(self):
+        # given
+        params = [
+            ("character", EsiContact.ContactType.CHARACTER),
+            ("corporation", EsiContact.ContactType.CORPORATION),
+            ("alliance", EsiContact.ContactType.ALLIANCE),
+            ("faction", EsiContact.ContactType.FACTION),
+        ]
+        for input, expected in params:
+            with self.subTest(input=input):
+                # when
+                obj = EsiContact(1001, input, 5.0)
+                # then
+                self.assertEqual(obj.contact_id, 1001)
+                self.assertEqual(obj.contact_type, expected)
+                self.assertEqual(obj.standing, 5.0)
 
     def test_should_clone_contact_1(self):
         # given
-        a = EsiContact(1, "character", 5.0, [1, 2])
+        a = EsiContact(1, EsiContact.ContactType.CHARACTER, 5.0, frozenset([1, 2]))
         # when
         b = a.clone()
         # then
         self.assertEqual(a, b)
 
     def test_should_clone_contact_2(self):
         # given
-        a = EsiContact(1, "character", 5.0, [1, 2])
+        a = EsiContact(1, EsiContact.ContactType.CHARACTER, 5.0, frozenset([1, 2]))
         # when
         b = a.clone(standing=-10)
         # then
         self.assertEqual(b.contact_id, a.contact_id)
         self.assertEqual(b.contact_type, a.contact_type)
         self.assertEqual(b.label_ids, a.label_ids)
         self.assertEqual(b.standing, -10)
 
-    def test_should_create_from_dict_1(self):
+    def test_should_create_from_esi_character(self):
         # given
         esi_dict = {"contact_id": 1, "contact_type": "character", "standing": 5.0}
         # when
         obj = EsiContact.from_esi_dict(esi_dict)
         # then
-        self.assertEqual(obj, EsiContact(1, "character", 5.0))
+        self.assertEqual(obj, EsiContact(1, EsiContact.ContactType.CHARACTER, 5.0))
 
-    def test_should_create_from_dict_2(self):
+    def test_should_create_from_esi_corporation(self):
         # given
         esi_dict = {"contact_id": 1, "contact_type": "corporation", "standing": 5.0}
         # when
         obj = EsiContact.from_esi_dict(esi_dict)
         # then
-        self.assertEqual(obj, EsiContact(1, "corporation", 5.0))
+        self.assertEqual(obj, EsiContact(1, EsiContact.ContactType.CORPORATION, 5.0))
 
-    def test_should_create_from_dict_3(self):
+    def test_should_create_from_esi_alliance(self):
         # given
         esi_dict = {"contact_id": 1, "contact_type": "alliance", "standing": 5.0}
         # when
         obj = EsiContact.from_esi_dict(esi_dict)
         # then
-        self.assertEqual(obj, EsiContact(1, "alliance", 5.0))
+        self.assertEqual(obj, EsiContact(1, EsiContact.ContactType.ALLIANCE, 5.0))
 
-    def test_should_create_from_dict_4(self):
+    def test_should_create_from_esi_contact_when_labels_are_none(self):
         # given
         esi_dict = {
             "contact_id": 1,
             "contact_type": "alliance",
             "standing": 5.0,
             "label_ids": None,
         }
         # when
         obj = EsiContact.from_esi_dict(esi_dict)
         # then
-        self.assertEqual(obj, EsiContact(1, "alliance", 5.0))
+        self.assertEqual(obj, EsiContact(1, EsiContact.ContactType.ALLIANCE, 5.0))
+
+    def test_should_create_from_esi_faction(self):
+        # given
+        esi_dict = {"contact_id": 1, "contact_type": "faction", "standing": 5.0}
+        # when
+        obj = EsiContact.from_esi_dict(esi_dict)
+        # then
+        self.assertEqual(obj, EsiContact(1, EsiContact.ContactType.FACTION, 5.0))
+
+    def test_should_create_from_eve_entities(self):
+        # given
+        params = [
+            (EveEntityCharacterFactory(), EsiContact.ContactType.CHARACTER),
+            (EveEntityCorporationFactory(), EsiContact.ContactType.CORPORATION),
+            (EveEntityAllianceFactory(), EsiContact.ContactType.ALLIANCE),
+            (EveEntityFactionFactory(), EsiContact.ContactType.FACTION),
+        ]
+        for eve_entity, expected in params:
+            with self.subTest(category=eve_entity.category):
+                # when
+                obj = EsiContact.from_eve_entity(eve_entity=eve_entity, standing=5.0)
+                # then
+                self.assertEqual(obj, EsiContact(eve_entity.id, expected, 5.0))
 
 
 class TestEsiContactLabel(NoSocketsTestCase):
     def test_should_create_from_esi_dict(self):
         # given
         esi_dict = {"label_id": 42, "label_name": "alpha"}
         # when
```

### Comparing `aa-standingssync-1.8.1/standingssync/tests/factories.py` & `aa_standingssync-1.9.0/standingssync/tests/factories.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,12 @@
+"""Model test factories."""
+
+
 import datetime as dt
+from typing import Generic, TypeVar
 
 import factory
 import factory.fuzzy
 
 from django.utils.timezone import now
 from eveuniverse.models import EveEntity
 
@@ -12,16 +16,25 @@
     EveCorporationInfoFactory,
     UserMainFactory,
 )
 
 from standingssync.core.esi_contacts import EsiContact, EsiContactLabel
 from standingssync.models import EveContact, EveWar, SyncedCharacter, SyncManager
 
+T = TypeVar("T")
+
 
-class EveEntityFactory(factory.django.DjangoModelFactory):
+class BaseMetaFactory(Generic[T], factory.base.FactoryMetaClass):
+    def __call__(cls, *args, **kwargs) -> T:
+        return super().__call__(*args, **kwargs)
+
+
+class EveEntityFactory(
+    factory.django.DjangoModelFactory, metaclass=BaseMetaFactory[EveEntity]
+):
     class Meta:
         model = EveEntity
         django_get_or_create = ("id", "name")
 
     category = EveEntity.CATEGORY_CHARACTER
 
     @factory.lazy_attribute
@@ -49,15 +62,29 @@
 
 
 class EveEntityAllianceFactory(EveEntityFactory):
     name = factory.Faker("company")
     category = EveEntity.CATEGORY_ALLIANCE
 
 
-class EveWarFactory(factory.django.DjangoModelFactory):
+class EveEntityFactionFactory(
+    factory.django.DjangoModelFactory, metaclass=BaseMetaFactory[EveEntity]
+):
+    class Meta:
+        model = EveEntity
+        django_get_or_create = ("id", "name")
+
+    id = factory.Sequence(lambda n: 500001 + n)
+    name = factory.Faker("color_name")
+    category = EveEntity.CATEGORY_FACTION
+
+
+class EveWarFactory(
+    factory.django.DjangoModelFactory, metaclass=BaseMetaFactory[EveWar]
+):
     class Meta:
         model = EveWar
 
     id = factory.Sequence(lambda n: 1 + n)
     aggressor = factory.SubFactory(EveEntityAllianceFactory)
     declared = factory.fuzzy.FuzzyDateTime(
         now() - dt.timedelta(days=3), end_dt=now() - dt.timedelta(days=2)
@@ -75,15 +102,15 @@
     @factory.post_generation
     def allies(self, create, extracted, **kwargs):
         if not create:
             return
 
         if extracted:
             for ally in extracted:
-                self.allies.add(ally)
+                self.allies.add(ally)  # type: ignore
 
 
 class UserMainManagerFactory(UserMainFactory):
     main_character__scopes = ["esi-alliances.read_contacts.v1"]
     permissions__ = ["standingssync.add_syncmanager"]
 
 
@@ -91,88 +118,96 @@
     main_character__scopes = [
         "esi-characters.read_contacts.v1",
         "esi-characters.write_contacts.v1",
     ]
     permissions__ = ["standingssync.add_syncedcharacter"]
 
 
-class SyncManagerFactory(factory.django.DjangoModelFactory):
+class SyncManagerFactory(
+    factory.django.DjangoModelFactory, metaclass=BaseMetaFactory[SyncManager]
+):
     class Meta:
         model = SyncManager
 
     class Params:
         user = factory.SubFactory(UserMainManagerFactory)
 
     @factory.lazy_attribute
     def alliance(self):
         return EveAllianceInfoFactory(
-            alliance_id=self.user.profile.main_character.alliance_id
+            alliance_id=self.user.profile.main_character.alliance_id  # type: ignore
         )
 
     @factory.lazy_attribute
     def character_ownership(self):
-        return self.user.profile.main_character.character_ownership
+        return self.user.profile.main_character.character_ownership  # type: ignore
 
     @factory.post_generation
     def create_eve_entities(self, create, extracted, **kwargs):
         if not create:
             return
         EveEntityAllianceFactory(
-            id=self.alliance.alliance_id, name=self.alliance.alliance_name
+            id=self.alliance.alliance_id, name=self.alliance.alliance_name  # type: ignore
         )
 
 
-class SyncedCharacterFactory(factory.django.DjangoModelFactory):
+class SyncedCharacterFactory(
+    factory.django.DjangoModelFactory, metaclass=BaseMetaFactory[SyncedCharacter]
+):
     class Meta:
         model = SyncedCharacter
 
     class Params:
         user = factory.SubFactory(UserMainSyncerFactory)
 
     manager = factory.SubFactory(SyncManagerFactory)
 
     @factory.lazy_attribute
     def character_ownership(self):
-        return self.user.profile.main_character.character_ownership
+        return self.user.profile.main_character.character_ownership  # type: ignore
 
 
-class EveContactFactory(factory.django.DjangoModelFactory):
+class EveContactFactory(
+    factory.django.DjangoModelFactory, metaclass=BaseMetaFactory[EveContact]
+):
     class Meta:
         model = EveContact
 
     manager = factory.SubFactory(SyncManagerFactory)
     eve_entity = factory.SubFactory(EveEntityCharacterFactory)
     standing = 5
     is_war_target = False
 
 
 class EveContactWarTargetFactory(EveContactFactory):
     standing = -10
     is_war_target = True
 
 
-class EsiContactDictFactory(factory.base.DictFactory):
+class EsiContactDictFactory(factory.base.DictFactory, metaclass=BaseMetaFactory[dict]):
     contact_id = factory.fuzzy.FuzzyInteger(90_000, 99_999)
     contact_type = factory.fuzzy.FuzzyChoice(["character", "corporation", "alliance"])
     standing = factory.fuzzy.FuzzyFloat(-10.0, 10.0)
 
 
-class EsiLabelDictFactory(factory.base.DictFactory):
+class EsiLabelDictFactory(factory.base.DictFactory, metaclass=BaseMetaFactory[dict]):
     label_id = factory.fuzzy.FuzzyInteger(1, 9_999)
     label_name = factory.Faker("word")
 
 
-class EsiContactFactory(factory.base.Factory):
+class EsiContactFactory(factory.base.Factory, metaclass=BaseMetaFactory[EsiContact]):
     class Meta:
         model = EsiContact
 
     contact_id = factory.fuzzy.FuzzyInteger(90_000, 99_999)
     contact_type = factory.fuzzy.FuzzyChoice(list(EsiContact.ContactType))
     standing = factory.fuzzy.FuzzyFloat(-10.0, 10.0)
 
 
-class EsiContactLabelFactory(factory.base.DictFactory):
+class EsiContactLabelFactory(
+    factory.base.Factory, metaclass=BaseMetaFactory[EsiContactLabel]
+):
     class Meta:
         model = EsiContactLabel
 
     id = factory.fuzzy.FuzzyInteger(1, 9_999)
     name = factory.Faker("word")
```

### Comparing `aa-standingssync-1.8.1/standingssync/tests/test_admin.py` & `aa_standingssync-1.9.0/standingssync/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa-standingssync-1.8.1/standingssync/tests/test_integration.py` & `aa_standingssync-1.9.0/standingssync/tests/test_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from eveuniverse.models import EveEntity
 
 from allianceauth.eveonline.models import EveAllianceInfo
 from app_utils.esi_testing import BravadoOperationStub
 from app_utils.testing import NoSocketsTestCase
 
 from standingssync.core.esi_contacts import EsiContact, EsiContactLabel
+from standingssync.tasks import run_manager_sync
 
-from ..tasks import run_manager_sync
 from .factories import (
     EveEntityAllianceFactory,
     EveEntityCharacterFactory,
     EveWarFactory,
     SyncedCharacterFactory,
     SyncManagerFactory,
     UserMainSyncerFactory,
```

### Comparing `aa-standingssync-1.8.1/standingssync/tests/test_managers.py` & `aa_standingssync-1.9.0/standingssync/tests/test_managers.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 from allianceauth.authentication.models import CharacterOwnership
 from allianceauth.eveonline.models import EveAllianceInfo
 from app_utils.esi_testing import BravadoOperationStub
 from app_utils.testdata_factories import UserFactory
 from app_utils.testing import NoSocketsTestCase, create_user_from_evecharacter
 
-from ..models import EveWar, SyncManager
+from standingssync.models import EveWar, SyncManager
+
 from .factories import (
     EveContactFactory,
     EveEntityAllianceFactory,
     EveEntityCorporationFactory,
     EveWarFactory,
     SyncedCharacterFactory,
     SyncManagerFactory,
```

### Comparing `aa-standingssync-1.8.1/standingssync/tests/test_models.py` & `aa_standingssync-1.9.0/standingssync/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import datetime as dt
 from typing import Set
 from unittest.mock import patch
 
 from django.utils.timezone import now
 from esi.errors import TokenExpiredError, TokenInvalidError
+from esi.models import Token
 from eveuniverse.models import EveEntity
 
 from allianceauth.eveonline.models import EveCharacter
 from app_utils.esi_testing import BravadoOperationStub
 from app_utils.testing import (
     NoSocketsTestCase,
     add_character_to_user,
     create_user_from_evecharacter,
 )
 
 from standingssync.core.esi_contacts import EsiContact, EsiContactsContainer
+from standingssync.models import EveContact, EveWar, SyncedCharacter, SyncManager
 
-from ..models import EveContact, EveWar, SyncedCharacter, SyncManager
 from .factories import (
     EsiContactFactory,
     EsiContactLabelFactory,
     EveContactFactory,
     EveContactWarTargetFactory,
     EveEntityAllianceFactory,
     EveEntityCharacterFactory,
@@ -187,15 +188,27 @@
         )
         self.assertSetEqual(expected_contact_ids, result_contact_ids)
         contact = sync_manager.contacts.get(eve_entity_id=3015)
         self.assertEqual(contact.standing, -10.0)
         self.assertTrue(contact.is_war_target)
 
 
-class TestSyncManagerErrorCases(LoadTestDataMixin, NoSocketsTestCase):
+class TestSyncManager(LoadTestDataMixin, NoSocketsTestCase):
+    def test_should_return_token(self):
+        # given
+        obj = SyncManagerFactory()
+        # when/then
+        self.assertIsInstance(obj.fetch_token(), Token)
+
+    def test_should_none_when_no_character_ownership(self):
+        # given
+        obj = SyncManagerFactory(character_ownership=None)
+        # when/then
+        self.assertIsNone(obj.fetch_token())
+
     def test_should_abort_when_no_char(self):
         # given
         sync_manager = SyncManagerFactory(
             alliance=self.alliance_1, character_ownership=None
         )
         # when/then
         with self.assertRaises(RuntimeError):
@@ -221,14 +234,27 @@
             user, self.character_1  # Token without valid scope will not be found
         )
         sync_manager = SyncManagerFactory(user=user)
         # when/then
         with self.assertRaises(RuntimeError):
             sync_manager.run_sync()
 
+    def test_should_return_character(self):
+        # given
+        obj = SyncManagerFactory()
+        # when/then
+        self.assertEqual(obj.character, obj.character_ownership.character)  # type: ignore
+
+    def test_should_raise_error_when_no_character(self):
+        # given
+        obj = SyncManagerFactory(character_ownership=None)
+        # when
+        with self.assertRaises(ValueError):
+            _ = obj.character
+
 
 @patch(MODELS_PATH + ".STANDINGSSYNC_ADD_WAR_TARGETS", True)
 @patch(ESI_API_PATH + ".esi")
 class TestSyncManager2(NoSocketsTestCase):
     @staticmethod
     def _war_target_contact_ids() -> Set[int]:
         return set(
@@ -403,14 +429,65 @@
         with patch(MODELS_PATH + ".STANDINGSSYNC_ADD_WAR_TARGETS", True):
             result = sync_manager._add_war_targets(alliance_contacts)
         # then
         self.assertSetEqual(alliance_contacts.contacts(), {defender})
         self.assertSetEqual(result, {defender.contact_id})
 
 
+class TestSyncCharacter(NoSocketsTestCase):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+        cls.sync_manager = SyncManagerFactory()
+
+    def test_should_return_token(self):
+        # given
+        obj = SyncedCharacterFactory(manager=self.sync_manager)
+        # when
+        result = obj.fetch_token()
+        # then
+        self.assertIsInstance(result, Token)
+
+    def test_should_return_none_and_delete_when_token_invalid(self):
+        # given
+        obj = SyncedCharacterFactory(manager=self.sync_manager)
+        with patch(MODELS_PATH + ".SyncedCharacter._valid_token") as m:
+            m.side_effect = TokenInvalidError
+            # when
+            result = obj.fetch_token()
+        # then
+        self.assertIsNone(result)
+        self.assertFalse(SyncedCharacter.objects.filter(pk=obj.pk).exists())
+
+    def test_should_return_none_and_delete_when_token_has_issues(self):
+        params = [TokenInvalidError, TokenExpiredError]
+        for exception in params:
+            with self.subTest(exception=exception):
+                # given
+                obj = SyncedCharacterFactory(manager=self.sync_manager)
+                # when
+                with patch(MODELS_PATH + ".SyncedCharacter._valid_token") as m:
+                    m.side_effect = exception
+                    result = obj.fetch_token()
+                # then
+                self.assertIsNone(result)
+                self.assertFalse(SyncedCharacter.objects.filter(pk=obj.pk).exists())
+
+    def test_should_return_none_and_delete_when_token_not_found(self):
+        # given
+        obj = SyncedCharacterFactory(manager=self.sync_manager)
+        # when
+        with patch(MODELS_PATH + ".SyncedCharacter._valid_token") as m:
+            m.return_value = None
+            result = obj.fetch_token()
+        # then
+        self.assertIsNone(result)
+        self.assertFalse(SyncedCharacter.objects.filter(pk=obj.pk).exists())
+
+
 @patch(ESI_CONTACTS_PATH + ".STANDINGSSYNC_WAR_TARGETS_LABEL_NAME", WAR_TARGET_LABEL)
 @patch(ESI_API_PATH + ".esi")
 class TestSyncCharacterEsi(NoSocketsTestCase):
     @patch(MODELS_PATH + ".STANDINGSSYNC_ADD_WAR_TARGETS", False)
     @patch(MODELS_PATH + ".STANDINGSSYNC_REPLACE_CONTACTS", True)
     @patch(MODELS_PATH + ".STANDINGSSYNC_CHAR_MIN_STANDING", 0.01)
     def test_should_replace_contacts_no_wt(self, mock_esi):
@@ -703,87 +780,36 @@
             contacts=[character_contact_1],
         )
         # when
         synced_character.delete_all_contacts()
         # then
         self.assertSetEqual(esi_character_contacts.contacts(), set())
 
+    def test_should_do_nothing_when_no_token(self, mock_esi):
+        # given
+        obj = SyncedCharacterFactory()
+        obj.character_ownership.user.token_set.all().delete()
+        with patch(MODELS_PATH + ".esi_api.delete_character_contacts") as esi_api:
+            # when
+            obj.delete_all_contacts()
+            # then
+            self.assertFalse(esi_api.called)
+
 
 class TestSyncCharacterErrorCases(LoadTestDataMixin, NoSocketsTestCase):
     def test_should_delete_when_insufficient_permission(self):
         # given
         user, _ = create_user_from_evecharacter(self.character_1.character_id)
         alt_ownership = add_character_to_user(
             user, character=self.character_2, scopes=SyncedCharacter.get_esi_scopes()
         )
         sync_manager = SyncManagerFactory(user=user, version_hash="new")
         sync_character = SyncedCharacterFactory(
             character_ownership=alt_ownership, manager=sync_manager
         )
-        # when
-        result = sync_character.run_sync()
-        # then
-        self.assertFalse(result)
-        self.assertFalse(SyncedCharacter.objects.filter(pk=sync_character.pk).exists())
-
-    def test_should_delete_when_no_valid_token_found(self):
-        # given
-        user, _ = create_user_from_evecharacter(
-            self.character_1.character_id,
-            permissions=["standingssync.add_syncedcharacter"],
-        )
-        alt_ownership = add_character_to_user(
-            user, character=self.character_2
-        )  # token has wrong scope and will therefore not be found
-        sync_manager = SyncManagerFactory(user=user, version_hash="new")
-        sync_character = SyncedCharacterFactory(
-            character_ownership=alt_ownership, manager=sync_manager
-        )
-        # when
-        result = sync_character.run_sync()
-        # then
-        self.assertFalse(result)
-        self.assertFalse(SyncedCharacter.objects.filter(pk=sync_character.pk).exists())
-
-    @patch(MODELS_PATH + ".Token")
-    def test_should_delete_when_token_is_invalid(self, mock_Token):
-        # given
-        mock_Token.objects.filter.side_effect = TokenInvalidError()
-        user, _ = create_user_from_evecharacter(
-            self.character_1.character_id,
-            permissions=["standingssync.add_syncedcharacter"],
-        )
-        alt_ownership = add_character_to_user(
-            user, character=self.character_2, scopes=SyncedCharacter.get_esi_scopes()
-        )
-        sync_manager = SyncManagerFactory(user=user, version_hash="new")
-        sync_character = SyncedCharacterFactory(
-            character_ownership=alt_ownership, manager=sync_manager
-        )
-        # when
-        result = sync_character.run_sync()
-        # then
-        self.assertFalse(result)
-        self.assertFalse(SyncedCharacter.objects.filter(pk=sync_character.pk).exists())
-
-    @patch(MODELS_PATH + ".Token")
-    def test_should_delete_when_token_is_expired(self, mock_Token):
-        # given
-        mock_Token.objects.filter.side_effect = TokenExpiredError()
-        user, _ = create_user_from_evecharacter(
-            self.character_1.character_id,
-            permissions=["standingssync.add_syncedcharacter"],
-        )
-        alt_ownership = add_character_to_user(
-            user, character=self.character_2, scopes=SyncedCharacter.get_esi_scopes()
-        )
-        sync_manager = SyncManagerFactory(user=user, version_hash="new")
-        sync_character = SyncedCharacterFactory(
-            character_ownership=alt_ownership, manager=sync_manager
-        )
         # when
         result = sync_character.run_sync()
         # then
         self.assertFalse(result)
         self.assertFalse(SyncedCharacter.objects.filter(pk=sync_character.pk).exists())
 
     @patch(MODELS_PATH + ".STANDINGSSYNC_CHAR_MIN_STANDING", 0.1)
```

### Comparing `aa-standingssync-1.8.1/standingssync/tests/test_tasks.py` & `aa_standingssync-1.9.0/standingssync/tests/test_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 from allianceauth.authentication.models import CharacterOwnership
 from app_utils.testing import (
     NoSocketsTestCase,
     create_user_from_evecharacter,
     generate_invalid_pk,
 )
 
-from .. import tasks
-from ..models import SyncedCharacter, SyncManager
+from standingssync import tasks
+from standingssync.models import SyncedCharacter, SyncManager
+
 from .factories import EveContactFactory, SyncedCharacterFactory, SyncManagerFactory
 from .utils import ALLIANCE_CONTACTS, LoadTestDataMixin
 
 MANAGERS_PATH = "standingssync.managers"
 MODELS_PATH = "standingssync.models"
 TASKS_PATH = "standingssync.tasks"
 
@@ -101,25 +102,25 @@
             tasks.run_character_sync(generate_invalid_pk(SyncedCharacter))
 
     @patch(TASKS_PATH + ".SyncedCharacter.run_sync")
     def test_should_call_update(self, mock_update):
         # given
         mock_update.return_value = True
         # when
-        tasks.run_character_sync(self.synced_character_2)
+        tasks.run_character_sync(self.synced_character_2.pk)
         # then
         self.assertTrue(mock_update.called)
 
     @patch(TASKS_PATH + ".SyncedCharacter.run_sync")
     def test_should_raise_exception(self, mock_update):
         # given
         mock_update.side_effect = RuntimeError
         # when
         with self.assertRaises(RuntimeError):
-            tasks.run_character_sync(self.synced_character_2)
+            tasks.run_character_sync(self.synced_character_2.pk)
 
 
 @patch(TASKS_PATH + ".run_character_sync")
 class TestManagerSync(LoadTestDataMixin, TestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
```

### Comparing `aa-standingssync-1.8.1/standingssync/tests/test_views.py` & `aa_standingssync-1.9.0/standingssync/tests/test_views.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 from django.test import RequestFactory, TestCase
 from django.urls import reverse
 from esi.models import Token
 
 from allianceauth.authentication.models import CharacterOwnership
 from app_utils.testing import NoSocketsTestCase, create_user_from_evecharacter
 
-from .. import views
-from ..models import EveEntity, SyncedCharacter, SyncManager
+from standingssync import views
+from standingssync.models import EveEntity, SyncedCharacter, SyncManager
+
 from .factories import EveContactFactory, SyncedCharacterFactory, SyncManagerFactory
 from .utils import ALLIANCE_CONTACTS, LoadTestDataMixin
 
 MODULE_PATH = "standingssync.views"
 
 
 class TestMainScreen(LoadTestDataMixin, TestCase):
@@ -46,14 +47,24 @@
             manager=cls.sync_manager, character_ownership=cls.alt_ownership_1
         )
 
         # user 3 has no permission
         cls.user_3, _ = create_user_from_evecharacter(cls.character_3.character_id)
         cls.factory = RequestFactory()
 
+    def test_should_redirect_to_main_page(self):
+        # given
+        request = self.factory.get(reverse("standingssync:characters"))
+        request.user = self.user_2
+        # when
+        response = views.index(request)
+        # then
+        self.assertEqual(response.status_code, 302)
+        self.assertEqual(response.url, reverse("standingssync:characters"))
+
     def test_user_with_permission_can_open_app(self):
         request = self.factory.get(reverse("standingssync:characters"))
         request.user = self.user_2
         response = views.characters(request)
         self.assertEqual(response.status_code, 200)
 
     def test_user_wo_permission_can_not_open_app(self):
@@ -69,20 +80,14 @@
         )
         request.user = self.user_2
         response = views.remove_character(request, self.sync_char.pk)
         self.assertEqual(response.status_code, 302)
         self.assertTrue(mock_messages.success.called)
         self.assertFalse(SyncedCharacter.objects.filter(pk=self.sync_char.pk).exists())
 
-    def test_user_with_permission_can_set_alliance_char(self):
-        pass
-
-    def test_user_wo_permission_can_not_set_alliance_char(self):
-        pass
-
 
 @patch(MODULE_PATH + ".tasks.run_character_sync")
 @patch(MODULE_PATH + ".messages")
 class TestAddSyncChar(LoadTestDataMixin, NoSocketsTestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
@@ -117,15 +122,15 @@
         cls.factory = RequestFactory()
 
     def make_request(self, user, character):
         token = Mock(spec=Token)
         token.character_id = character.character_id
         request = self.factory.get(reverse("standingssync:add_character"))
         request.user = user
-        request.token = token
+        request.token = token  # type: ignore
         middleware = SessionMiddleware(Mock())
         middleware.process_request(request)
         orig_view = views.add_character.__wrapped__.__wrapped__.__wrapped__
         return orig_view(request, token)
 
     def test_users_can_not_add_alliance_members(
         self, mock_messages, mock_run_character_sync
@@ -214,15 +219,15 @@
         cls.factory = RequestFactory()
 
     def make_request(self, user, character):
         token = Mock(spec=Token)
         token.character_id = character.character_id
         request = self.factory.get(reverse("standingssync:add_alliance_manager"))
         request.user = user
-        request.token = token
+        request.token = token  # type: ignore
         middleware = SessionMiddleware(Mock())
         middleware.process_request(request)
         orig_view = views.add_alliance_manager.__wrapped__.__wrapped__.__wrapped__
         return orig_view(request, token)
 
     def test_user_with_permission_can_add_alliance_manager(
         self, mock_messages, mock_tasks
```

### Comparing `aa-standingssync-1.8.1/standingssync/tests/utils.py` & `aa_standingssync-1.9.0/standingssync/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa-standingssync-1.8.1/standingssync/urls.py` & `aa_standingssync-1.9.0/standingssync/urls.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Routes for standingssync."""
+
 from django.urls import path
 
 from . import views
 
 app_name = "standingssync"
 
 urlpatterns = [
```

### Comparing `aa-standingssync-1.8.1/standingssync/views.py` & `aa_standingssync-1.9.0/standingssync/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Views for standingssync."""
+
 from django.contrib import messages
 from django.contrib.admin.views.decorators import staff_member_required
 from django.contrib.auth.decorators import login_required, permission_required
 from django.db.models import Prefetch
 from django.shortcuts import get_object_or_404, redirect, render
 from esi.decorators import token_required
 
@@ -41,23 +43,23 @@
     return redirect("standingssync:characters")
 
 
 @login_required
 @permission_required("standingssync.add_syncedcharacter")
 def characters(request):
     """main page"""
-    sync_manager = SyncManager.objects.fetch_for_user(request.user)
+    sync_manager: SyncManager = SyncManager.objects.fetch_for_user(request.user)
     synced_characters = []
     if sync_manager:
         qs = sync_manager.synced_characters_for_user(request.user).select_related(
             "character_ownership", "character_ownership__character"
         )
         for synced_character in qs:
             character = synced_character.character
-            organization = character.corporation_name
+            organization = str(character.corporation_name)
             if character.alliance_ticker:
                 organization += f" [{character.alliance_ticker}]"
 
             errors = []
             if not synced_character.is_sync_fresh:
                 errors.append("Sync is outdated.")
             if (
@@ -74,47 +76,49 @@
                     "name": character.character_name,
                     "portrait_url": character.portrait_url,
                     "organization": organization,
                     "errors": errors,
                     "pk": synced_character.pk,
                 }
             )
+
+    if sync_manager:
+        alliance = sync_manager.alliance
+        alliance_contacts_count = (
+            sync_manager.contacts.filter(is_war_target=False).count()  # type: ignore
+            if STANDINGSSYNC_REPLACE_CONTACTS
+            else None
+        )
+        alliance_war_targets_count = (
+            sync_manager.contacts.filter(is_war_target=True).count()  # type: ignore
+            if STANDINGSSYNC_ADD_WAR_TARGETS
+            else None
+        )
+
+    else:
+        alliance = None
+        alliance_contacts_count = None
+        alliance_war_targets_count = None
+
     context = {
         "page_title": "My Characters",
         "synced_characters": synced_characters,
+        "alliance": alliance,
         "has_synced_chars": len(synced_characters) > 0,
+        "alliance_contacts_count": alliance_contacts_count,
+        "alliance_war_targets_count": alliance_war_targets_count,
+        "war_targets_label_name": STANDINGSSYNC_WAR_TARGETS_LABEL_NAME,
     }
-    if sync_manager:
-        context["alliance"] = sync_manager.alliance
-        if STANDINGSSYNC_REPLACE_CONTACTS:
-            alliance_contacts_count = sync_manager.contacts.filter(
-                is_war_target=False
-            ).count()
-        else:
-            alliance_contacts_count = None
-        if STANDINGSSYNC_ADD_WAR_TARGETS:
-            alliance_war_targets_count = sync_manager.contacts.filter(
-                is_war_target=True
-            ).count()
-        else:
-            alliance_war_targets_count = None
-    else:
-        context["alliance"] = None
-        alliance_contacts_count = None
-        alliance_war_targets_count = None
 
-    context["alliance_contacts_count"] = alliance_contacts_count
-    context["alliance_war_targets_count"] = alliance_war_targets_count
-    context["war_targets_label_name"] = STANDINGSSYNC_WAR_TARGETS_LABEL_NAME
     return render(request, "standingssync/characters.html", common_context(context))
 
 
 @login_required
 @permission_required("standingssync.add_syncmanager")
-@token_required(SyncManager.get_esi_scopes())
+@token_required(SyncManager.get_esi_scopes())  # type: ignore
 def add_alliance_manager(request, token):
     """Add or update sync manager for an alliance."""
     token_char = get_object_or_404(EveCharacter, character_id=token.character_id)
     if not token_char.alliance_id:
         messages.warning(
             request,
             f"Can not add {token_char}, because it is not a member of any alliance.",
@@ -132,32 +136,32 @@
             alliance=alliance, defaults={"character_ownership": character_ownership}
         )
         tasks.run_manager_sync.delay(sync_manager.pk)
         if STANDINGSSYNC_ADD_WAR_TARGETS:
             tasks.sync_all_wars.delay()
         messages.success(
             request,
-            f"{sync_manager.character_ownership.character.character_name} "
+            f"{sync_manager.character.character_name} "
             f"set as alliance character for {alliance.alliance_name}. "
             "Started syncing of alliance contacts. ",
         )
     return redirect("standingssync:index")
 
 
 @login_required
 @permission_required("standingssync.add_syncedcharacter")
-@token_required(scopes=SyncedCharacter.get_esi_scopes())
+@token_required(scopes=SyncedCharacter.get_esi_scopes())  # type: ignore
 def add_character(request, token):
     """add character to receive alliance contacts"""
     alliance = get_object_or_404(
         EveAllianceInfo, alliance_id=request.user.profile.main_character.alliance_id
     )
     sync_manager = get_object_or_404(SyncManager, alliance=alliance)
     token_char = get_object_or_404(EveCharacter, character_id=token.character_id)
-    if token_char.alliance_id == sync_manager.character_ownership.character.alliance_id:
+    if token_char.alliance_id == sync_manager.character.alliance_id:
         messages.warning(
             request,
             "Adding alliance members does not make much sense, "
             "since they already have access to alliance contacts.",
         )
 
     else:
@@ -201,52 +205,52 @@
     return redirect("standingssync:characters")
 
 
 @login_required
 @permission_required("standingssync.add_syncedcharacter")
 def wars(request):
     sync_manager = SyncManager.objects.fetch_for_user(request.user)
-    wars = []
+    all_wars = []
     if sync_manager:
         for war in (
             EveWar.objects.current_wars()
             .alliance_wars(alliance=sync_manager.alliance)
             .prefetch_related(Prefetch("allies", to_attr="allies_sorted"))
             .select_related("aggressor", "defender")
             .annotate_state()
             .annotate_is_active()
             .order_by("-started")
         ):
             allies = sorted(list(war.allies_sorted), key=lambda o: o.name)
-            wars.append(
+            all_wars.append(
                 {
                     "declared": war.declared,
                     "started": war.started,
                     "finished": war.finished,
                     "aggressor": war.aggressor,
                     "defender": war.defender,
                     "allies": allies,
                     "state": war.state,
                     "is_active": war.is_active,
                 }
             )
     context = {
         "page_title": "Current Wars",
         "alliance": "Not configured",
-        "wars": wars,
+        "wars": all_wars,
         "war_count": "?",
         "active_wars_count": "?",
         "State": EveWar.State,
     }
     if sync_manager:
         context.update(
             {
                 "alliance": sync_manager.alliance,
-                "war_count": len(wars),
-                "active_wars_count": sum([1 for obj in wars if obj["is_active"]]),
+                "war_count": len(all_wars),
+                "active_wars_count": sum([1 for obj in all_wars if obj["is_active"]]),
             }
         )
     return render(request, "standingssync/wars.html", common_context(context))
 
 
 @login_required
 @staff_member_required
```

