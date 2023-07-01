# Comparing `tmp/bk-iam-1.3.3.tar.gz` & `tmp/bk-iam-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bk-iam-1.3.3.tar", last modified: Wed Jun 21 09:42:43 2023, max compression
+gzip compressed data, was "dist/bk-iam-1.3.4.tar", last modified: Sat Jul  1 07:56:52 2023, max compression
```

## Comparing `bk-iam-1.3.3.tar` & `bk-iam-1.3.4.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/
--rw-r--r--   0 root         (0) root         (0)       47 2023-06-21 09:42:03.000000 bk-iam-1.3.3/iam/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/api/
--rw-r--r--   0 root         (0) root         (0)    16124 2023-03-07 08:22:34.000000 bk-iam-1.3.3/iam/api/client.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5536 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/api/http.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/meta.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/objects.py
--rw-r--r--   0 root         (0) root         (0)    10156 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/dummy_iam.py
--rw-r--r--   0 root         (0) root         (0)    23130 2023-03-07 08:59:27.000000 bk-iam-1.3.3/iam/iam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/apply/
--rw-r--r--   0 root         (0) root         (0)     7594 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/apply/models.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/apply/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5087 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/eval/
--rw-r--r--   0 root         (0) root         (0)     1803 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/eval/constants.py
--rw-r--r--   0 root         (0) root         (0)     2079 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/eval/object.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/eval/expression.py
--rw-r--r--   0 root         (0) root         (0)    11845 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/eval/operators.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/eval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/model/
--rw-r--r--   0 root         (0) root         (0)     3470 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/model/models.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1286 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/collection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/iam_migration/
--rw-r--r--   0 root         (0) root         (0)      951 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/apps.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/iam_migration/templates/
--rw-r--r--   0 root         (0) root         (0)      570 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/templates/migration.tmpl
--rw-r--r--   0 root         (0) root         (0)      845 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1343 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/iam_migration/utils/
--rw-r--r--   0 root         (0) root         (0)    25878 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/utils/do_migrate.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2757 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/migrator.py
--rw-r--r--   0 root         (0) root         (0)      818 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/iam_migration/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/iam_migration/management/commands/
--rw-r--r--   0 root         (0) root         (0)     3756 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/management/commands/iam_makemigrations.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/iam_migration/migrations/
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/iam_migration/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/django/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/django/dispatcher/
--rw-r--r--   0 root         (0) root         (0)      923 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/django/dispatcher/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     9942 2023-06-21 09:42:03.000000 bk-iam-1.3.3/iam/contrib/django/dispatcher/dispatchers.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/django/dispatcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1347 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/django/middlewares.py
--rw-r--r--   0 root         (0) root         (0)     1308 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/django/response.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/django/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/converter/
--rw-r--r--   0 root         (0) root         (0)     2226 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/converter/base.py
--rw-r--r--   0 root         (0) root         (0)     5859 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/converter/queryset.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/converter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5814 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/converter/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/contrib/tastypie/
--rw-r--r--   0 root         (0) root         (0)     4177 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/tastypie/resource.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/tastypie/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8012 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/tastypie/authorization.py
--rw-r--r--   0 root         (0) root         (0)     2090 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/tastypie/shortcuts.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/__init__.py
--rw-r--r--   0 root         (0) root         (0)      781 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/contrib/http.py
--rw-r--r--   0 root         (0) root         (0)     1911 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/resource/
--rw-r--r--   0 root         (0) root         (0)     3430 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/resource/provider.py
--rw-r--r--   0 root         (0) root         (0)      982 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/resource/constants.py
--rw-r--r--   0 root         (0) root         (0)      948 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/resource/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)     1439 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/resource/utils.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/resource/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1179 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/shortcuts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/iam/auth/
--rw-r--r--   0 root         (0) root         (0)    14884 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/auth/models.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-03-07 02:07:52.000000 bk-iam-1.3.3/iam/cache.py
--rw-r--r--   0 root         (0) root         (0)       59 2023-06-21 09:42:43.000000 bk-iam-1.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      194 2023-03-07 02:07:52.000000 bk-iam-1.3.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     3109 2023-06-14 09:22:24.000000 bk-iam-1.3.3/readme_en.md
--rw-r--r--   0 root         (0) root         (0)      220 2023-03-07 02:07:52.000000 bk-iam-1.3.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      565 2023-06-21 09:42:43.000000 bk-iam-1.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1244 2023-03-07 02:07:52.000000 bk-iam-1.3.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:42:43.000000 bk-iam-1.3.3/bk_iam.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1948 2023-06-21 09:42:43.000000 bk-iam-1.3.3/bk_iam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 09:42:43.000000 bk-iam-1.3.3/bk_iam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-21 09:42:43.000000 bk-iam-1.3.3/bk_iam.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-21 09:42:43.000000 bk-iam-1.3.3/bk_iam.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      565 2023-06-21 09:42:43.000000 bk-iam-1.3.3/bk_iam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3752 2023-06-14 09:22:24.000000 bk-iam-1.3.3/readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:52.000000 bk-iam-1.3.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:52.000000 bk-iam-1.3.4/iam/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-07-01 07:56:46.000000 bk-iam-1.3.4/iam/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:52.000000 bk-iam-1.3.4/iam/api/
+-rw-r--r--   0 root         (0) root         (0)    16124 2023-03-07 08:22:34.000000 bk-iam-1.3.4/iam/api/client.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5536 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/api/http.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/meta.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/objects.py
+-rw-r--r--   0 root         (0) root         (0)    10156 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/dummy_iam.py
+-rw-r--r--   0 root         (0) root         (0)    23130 2023-03-07 08:59:27.000000 bk-iam-1.3.4/iam/iam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:52.000000 bk-iam-1.3.4/iam/apply/
+-rw-r--r--   0 root         (0) root         (0)     7594 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/apply/models.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/apply/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5087 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:52.000000 bk-iam-1.3.4/iam/eval/
+-rw-r--r--   0 root         (0) root         (0)     1803 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/eval/constants.py
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/eval/object.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/eval/expression.py
+-rw-r--r--   0 root         (0) root         (0)    11845 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/eval/operators.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/eval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:52.000000 bk-iam-1.3.4/iam/model/
+-rw-r--r--   0 root         (0) root         (0)     3470 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/model/models.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/collection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:52.000000 bk-iam-1.3.4/iam/contrib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:52.000000 bk-iam-1.3.4/iam/contrib/iam_migration/
+-rw-r--r--   0 root         (0) root         (0)      951 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/iam_migration/apps.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/iam_migration/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:52.000000 bk-iam-1.3.4/iam/contrib/iam_migration/templates/
+-rw-r--r--   0 root         (0) root         (0)      570 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/iam_migration/templates/migration.tmpl
+-rw-r--r--   0 root         (0) root         (0)      845 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/iam_migration/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1343 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/iam_migration/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:52.000000 bk-iam-1.3.4/iam/contrib/iam_migration/utils/
+-rw-r--r--   0 root         (0) root         (0)    25878 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/iam_migration/utils/do_migrate.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/iam_migration/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2805 2023-07-01 07:56:46.000000 bk-iam-1.3.4/iam/contrib/iam_migration/migrator.py
+-rw-r--r--   0 root         (0) root         (0)      818 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/iam_migration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:52.000000 bk-iam-1.3.4/iam/contrib/iam_migration/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:52.000000 bk-iam-1.3.4/iam/contrib/iam_migration/management/commands/
+-rw-r--r--   0 root         (0) root         (0)     3756 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/iam_migration/management/commands/iam_makemigrations.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/iam_migration/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/iam_migration/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:52.000000 bk-iam-1.3.4/iam/contrib/iam_migration/migrations/
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/iam_migration/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/iam_migration/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:52.000000 bk-iam-1.3.4/iam/contrib/django/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:52.000000 bk-iam-1.3.4/iam/contrib/django/dispatcher/
+-rw-r--r--   0 root         (0) root         (0)      923 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/django/dispatcher/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     9942 2023-07-01 07:56:46.000000 bk-iam-1.3.4/iam/contrib/django/dispatcher/dispatchers.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/django/dispatcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/django/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/django/response.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/django/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:52.000000 bk-iam-1.3.4/iam/contrib/converter/
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/converter/base.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/converter/queryset.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/converter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5814 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/converter/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:52.000000 bk-iam-1.3.4/iam/contrib/tastypie/
+-rw-r--r--   0 root         (0) root         (0)     4177 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/tastypie/resource.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/tastypie/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8012 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/tastypie/authorization.py
+-rw-r--r--   0 root         (0) root         (0)     2090 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/tastypie/shortcuts.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      781 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/contrib/http.py
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:52.000000 bk-iam-1.3.4/iam/resource/
+-rw-r--r--   0 root         (0) root         (0)     3430 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/resource/provider.py
+-rw-r--r--   0 root         (0) root         (0)      982 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/resource/constants.py
+-rw-r--r--   0 root         (0) root         (0)      948 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/resource/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/resource/utils.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/resource/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1179 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/shortcuts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:52.000000 bk-iam-1.3.4/iam/auth/
+-rw-r--r--   0 root         (0) root         (0)    14884 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/auth/models.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-03-07 02:07:52.000000 bk-iam-1.3.4/iam/cache.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-01 07:56:52.000000 bk-iam-1.3.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      194 2023-03-07 02:07:52.000000 bk-iam-1.3.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-07-01 07:56:46.000000 bk-iam-1.3.4/readme_en.md
+-rw-r--r--   0 root         (0) root         (0)      220 2023-03-07 02:07:52.000000 bk-iam-1.3.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      565 2023-07-01 07:56:52.000000 bk-iam-1.3.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-07-01 07:56:46.000000 bk-iam-1.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:52.000000 bk-iam-1.3.4/bk_iam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-07-01 07:56:52.000000 bk-iam-1.3.4/bk_iam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-01 07:56:52.000000 bk-iam-1.3.4/bk_iam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-07-01 07:56:52.000000 bk-iam-1.3.4/bk_iam.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-01 07:56:52.000000 bk-iam-1.3.4/bk_iam.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      565 2023-07-01 07:56:52.000000 bk-iam-1.3.4/bk_iam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3752 2023-07-01 07:56:46.000000 bk-iam-1.3.4/readme.md
```

### Comparing `bk-iam-1.3.3/iam/api/client.py` & `bk-iam-1.3.4/iam/api/client.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/api/__init__.py` & `bk-iam-1.3.4/iam/api/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/api/http.py` & `bk-iam-1.3.4/iam/api/http.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/meta.py` & `bk-iam-1.3.4/iam/meta.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/exceptions.py` & `bk-iam-1.3.4/iam/exceptions.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/objects.py` & `bk-iam-1.3.4/iam/objects.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/dummy_iam.py` & `bk-iam-1.3.4/iam/dummy_iam.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/iam.py` & `bk-iam-1.3.4/iam/iam.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/apply/models.py` & `bk-iam-1.3.4/iam/apply/models.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/apply/__init__.py` & `bk-iam-1.3.4/iam/apply/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/utils.py` & `bk-iam-1.3.4/iam/utils.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/eval/constants.py` & `bk-iam-1.3.4/iam/eval/constants.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/eval/object.py` & `bk-iam-1.3.4/iam/eval/object.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/eval/expression.py` & `bk-iam-1.3.4/iam/eval/expression.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/eval/operators.py` & `bk-iam-1.3.4/iam/eval/operators.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/eval/__init__.py` & `bk-iam-1.3.4/iam/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/model/models.py` & `bk-iam-1.3.4/iam/model/models.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/model/__init__.py` & `bk-iam-1.3.4/iam/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/collection.py` & `bk-iam-1.3.4/iam/collection.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/iam_migration/apps.py` & `bk-iam-1.3.4/iam/contrib/iam_migration/apps.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/iam_migration/constants.py` & `bk-iam-1.3.4/iam/contrib/iam_migration/constants.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/iam_migration/templates/migration.tmpl` & `bk-iam-1.3.4/iam/contrib/iam_migration/templates/migration.tmpl`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/iam_migration/exceptions.py` & `bk-iam-1.3.4/iam/contrib/iam_migration/exceptions.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/iam_migration/template.py` & `bk-iam-1.3.4/iam/contrib/iam_migration/template.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/iam_migration/utils/do_migrate.py` & `bk-iam-1.3.4/iam/contrib/iam_migration/utils/do_migrate.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/iam_migration/utils/__init__.py` & `bk-iam-1.3.4/iam/contrib/iam_migration/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/iam_migration/migrator.py` & `bk-iam-1.3.4/iam/contrib/iam_migration/migrator.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,26 +30,25 @@
 
 renders = {"upsert_system": upsert_system_render}
 
 
 class IAMMigrator(object):
     def __init__(self, migration_json):
         self.migration_json = migration_json
+        self._bk_app_code = getattr(settings, "APP_CODE", "")
+        self._bk_app_secret = settings.SECRET_KEY
 
     def migrate(self):
-        app_code = settings.APP_CODE
-        app_secret = settings.SECRET_KEY
-
         iam_host = ""
         USE_APIGATEWAY = getattr(settings, "BK_IAM_USE_APIGATEWAY", False)
         if USE_APIGATEWAY:
             do_migrate.enable_use_apigateway()
             iam_host = getattr(settings, "BK_IAM_APIGATEWAY_URL", "")
             if iam_host == "":
-                raise exceptions.MigrationFailError("settings.BK_IAM_APIGATEWAY_URL should be setted")
+                raise exceptions.MigrationFailError("settings.BK_IAM_APIGATEWAY_URL should be set")
         else:
             iam_host = settings.BK_IAM_INNER_HOST
 
         # only trigger migrator at db migrate
         if "migrate" not in sys.argv:
             return
 
@@ -67,10 +66,10 @@
             if op["operation"] in renders:
                 renders[op["operation"]](op["data"])
 
         ok, _ = do_migrate.api_ping(iam_host)
         if not ok:
             raise exceptions.NetworkUnreachableError("bk iam ping error")
 
-        ok = do_migrate.do_migrate(data, iam_host, app_code, app_secret)
+        ok = do_migrate.do_migrate(data, iam_host, self._bk_app_code, self._bk_app_secret)
         if not ok:
             raise exceptions.MigrationFailError("iam migrate fail")
```

### Comparing `bk-iam-1.3.3/iam/contrib/iam_migration/__init__.py` & `bk-iam-1.3.4/iam/contrib/iam_migration/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/iam_migration/management/commands/iam_makemigrations.py` & `bk-iam-1.3.4/iam/contrib/iam_migration/management/commands/iam_makemigrations.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/iam_migration/management/commands/__init__.py` & `bk-iam-1.3.4/iam/contrib/iam_migration/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/iam_migration/management/__init__.py` & `bk-iam-1.3.4/iam/contrib/iam_migration/management/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/iam_migration/migrations/__init__.py` & `bk-iam-1.3.4/iam/contrib/iam_migration/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/iam_migration/conf.py` & `bk-iam-1.3.4/iam/contrib/iam_migration/conf.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/django/dispatcher/exceptions.py` & `bk-iam-1.3.4/iam/contrib/django/dispatcher/exceptions.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/django/dispatcher/dispatchers.py` & `bk-iam-1.3.4/iam/contrib/django/dispatcher/dispatchers.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             return fail_response(401, "basic auth failed", request_id)
 
         # load json data
         try:
             data = json.loads(request.body)
         except Exception:
             logger.error("resource request(%s) failed with invalid body: %s", request_id, request.body)
-            return fail_response(400, "reqeust body is not a valid json", request_id)
+            return fail_response(400, "request body is not a valid json", request_id)
 
         # check basic params
         method = data.get("method")
         resource_type = data.get("type")
         if not (method and resource_type):
             logger.error("resource request(%s) failed with invalid data: %s. method and type required",
                          request_id, data)
```

### Comparing `bk-iam-1.3.3/iam/contrib/django/dispatcher/__init__.py` & `bk-iam-1.3.4/iam/contrib/django/dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/django/middlewares.py` & `bk-iam-1.3.4/iam/contrib/django/middlewares.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/django/response.py` & `bk-iam-1.3.4/iam/contrib/django/response.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/django/__init__.py` & `bk-iam-1.3.4/iam/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/converter/base.py` & `bk-iam-1.3.4/iam/contrib/converter/base.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/converter/queryset.py` & `bk-iam-1.3.4/iam/contrib/converter/queryset.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/converter/__init__.py` & `bk-iam-1.3.4/iam/contrib/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/converter/sql.py` & `bk-iam-1.3.4/iam/contrib/converter/sql.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/tastypie/resource.py` & `bk-iam-1.3.4/iam/contrib/tastypie/resource.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/tastypie/__init__.py` & `bk-iam-1.3.4/iam/contrib/tastypie/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/tastypie/authorization.py` & `bk-iam-1.3.4/iam/contrib/tastypie/authorization.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/tastypie/shortcuts.py` & `bk-iam-1.3.4/iam/contrib/tastypie/shortcuts.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/__init__.py` & `bk-iam-1.3.4/iam/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/contrib/http.py` & `bk-iam-1.3.4/iam/contrib/http.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/__init__.py` & `bk-iam-1.3.4/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/resource/provider.py` & `bk-iam-1.3.4/iam/resource/provider.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/resource/constants.py` & `bk-iam-1.3.4/iam/resource/constants.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/resource/dispatcher.py` & `bk-iam-1.3.4/iam/resource/dispatcher.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/resource/utils.py` & `bk-iam-1.3.4/iam/resource/utils.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/resource/__init__.py` & `bk-iam-1.3.4/iam/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/shortcuts.py` & `bk-iam-1.3.4/iam/shortcuts.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/auth/models.py` & `bk-iam-1.3.4/iam/auth/models.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/auth/__init__.py` & `bk-iam-1.3.4/iam/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/iam/cache.py` & `bk-iam-1.3.4/iam/cache.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/readme_en.md` & `bk-iam-1.3.4/readme_en.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ![](docs/resource/img/bk_iam_en.png)
 ---
 
-[![license](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/TencentBlueKing/iam-python-sdk/blob/master/LICENSE.txt) [![Release Version](https://img.shields.io/badge/release-1.3.2-brightgreen.svg)](https://github.com/TencentBlueKing/iam-python-sdk/releases) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/iam-python-sdk/pulls) [![BK Pipelines Status](https://api.bkdevops.qq.com/process/api/external/pipelines/projects/iam/p-5c359e750bb9457984ab84656651d843/badge?X-DEVOPS-PROJECT-ID=iam)](http://devops.oa.com/process/api-html/user/builds/projects/iam/pipelines/p-5c359e750bb9457984ab84656651d843/latestFinished?X-DEVOPS-PROJECT-ID=iam)
+[![license](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/TencentBlueKing/iam-python-sdk/blob/master/LICENSE.txt) [![Release Version](https://img.shields.io/badge/release-1.3.4-brightgreen.svg)](https://github.com/TencentBlueKing/iam-python-sdk/releases) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/iam-python-sdk/pulls) [![BK Pipelines Status](https://api.bkdevops.qq.com/process/api/external/pipelines/projects/iam/p-5c359e750bb9457984ab84656651d843/badge?X-DEVOPS-PROJECT-ID=iam)](http://devops.oa.com/process/api-html/user/builds/projects/iam/pipelines/p-5c359e750bb9457984ab84656651d843/latestFinished?X-DEVOPS-PROJECT-ID=iam)
 
 ## Overview
 
 iam-python-sdk is the SDK of blueking IAM(BK-IAM), your system can use BK-IAM easily via SDK.
 
 ## Features
```

### Comparing `bk-iam-1.3.3/PKG-INFO` & `bk-iam-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bk-iam
-Version: 1.3.3
+Version: 1.3.4
 Summary: bk-iam python sdk
 Home-page: https://github.com/TencentBlueKing/iam-python-sdk
 Author: TencentBlueKing
 Author-email: contactus_bk@tencent.com
 License: UNKNOWN
 Description: bk-iam python sdk
 Platform: UNKNOWN
```

### Comparing `bk-iam-1.3.3/setup.py` & `bk-iam-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 long_description = "bk-iam python sdk"
 
 requires = [
     "six>=1.11.0",
-    "cachetools==3.1.1",
+    "cachetools>=3.1.1,<6.0",
     "requests",
     "curlify==2.2.1",
 ]
 
 about = {}
 with open(os.path.join(here, "iam", "__version__.py"), "r") as f:
     exec(f.read(), about)
```

### Comparing `bk-iam-1.3.3/bk_iam.egg-info/SOURCES.txt` & `bk-iam-1.3.4/bk_iam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.3/bk_iam.egg-info/PKG-INFO` & `bk-iam-1.3.4/bk_iam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bk-iam
-Version: 1.3.3
+Version: 1.3.4
 Summary: bk-iam python sdk
 Home-page: https://github.com/TencentBlueKing/iam-python-sdk
 Author: TencentBlueKing
 Author-email: contactus_bk@tencent.com
 License: UNKNOWN
 Description: bk-iam python sdk
 Platform: UNKNOWN
```

### Comparing `bk-iam-1.3.3/readme.md` & `bk-iam-1.3.4/readme.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ![](docs/resource/img/bk_iam_zh.png)
 ---
 
-[![license](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/TencentBlueKing/iam-python-sdk/blob/master/LICENSE.txt) [![Release Version](https://img.shields.io/badge/release-1.3.2-brightgreen.svg)](https://github.com/TencentBlueKing/iam-python-sdk/releases) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/iam-python-sdk/pulls) [![BK Pipelines Status](https://api.bkdevops.qq.com/process/api/external/pipelines/projects/iam/p-5c359e750bb9457984ab84656651d843/badge?X-DEVOPS-PROJECT-ID=iam)](http://devops.oa.com/process/api-html/user/builds/projects/iam/pipelines/p-5c359e750bb9457984ab84656651d843/latestFinished?X-DEVOPS-PROJECT-ID=iam)
+[![license](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/TencentBlueKing/iam-python-sdk/blob/master/LICENSE.txt) [![Release Version](https://img.shields.io/badge/release-1.3.4-brightgreen.svg)](https://github.com/TencentBlueKing/iam-python-sdk/releases) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/iam-python-sdk/pulls) [![BK Pipelines Status](https://api.bkdevops.qq.com/process/api/external/pipelines/projects/iam/p-5c359e750bb9457984ab84656651d843/badge?X-DEVOPS-PROJECT-ID=iam)](http://devops.oa.com/process/api-html/user/builds/projects/iam/pipelines/p-5c359e750bb9457984ab84656651d843/latestFinished?X-DEVOPS-PROJECT-ID=iam)
 
 [(English Documents Available)](readme_en.md)
 
 ## Overview
 
 iam-python-sdk 是蓝鲸权限中心(BK-IAM)提供的用于快速接入权限体系的python SDK
```

