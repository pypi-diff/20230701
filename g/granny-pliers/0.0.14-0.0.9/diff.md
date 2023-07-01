# Comparing `tmp/granny-pliers-0.0.14.tar.gz` & `tmp/granny-pliers-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "granny-pliers-0.0.14.tar", last modified: Sat Jul  1 19:06:25 2023, max compression
+gzip compressed data, was "granny-pliers-0.0.9.tar", last modified: Wed Jun 14 21:02:38 2023, max compression
```

## Comparing `granny-pliers-0.0.14.tar` & `granny-pliers-0.0.9.tar`

### file list

```diff
@@ -1,75 +1,70 @@
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 19:06:25.076838 granny-pliers-0.0.14/
--rw-r--r--   0 pd         (501) staff       (20)    11357 2023-06-03 18:43:25.000000 granny-pliers-0.0.14/LICENSE
--rw-r--r--   0 pd         (501) staff       (20)    13701 2023-07-01 19:06:25.076273 granny-pliers-0.0.14/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)       16 2023-06-10 17:39:54.000000 granny-pliers-0.0.14/README.md
--rw-r--r--   0 pd         (501) staff       (20)     1620 2023-07-01 19:05:30.000000 granny-pliers-0.0.14/pyproject.toml
--rw-r--r--   0 pd         (501) staff       (20)       38 2023-07-01 19:06:25.076968 granny-pliers-0.0.14/setup.cfg
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 19:06:25.032495 granny-pliers-0.0.14/src/
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 19:06:25.036909 granny-pliers-0.0.14/src/granny_pliers/
--rw-r--r--   0 pd         (501) staff       (20)      988 2023-07-01 19:05:36.000000 granny-pliers-0.0.14/src/granny_pliers/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 19:06:25.047320 granny-pliers-0.0.14/src/granny_pliers/auth/
--rw-r--r--   0 pd         (501) staff       (20)     1228 2023-06-10 13:12:31.000000 granny-pliers-0.0.14/src/granny_pliers/auth/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     1683 2023-06-10 11:50:56.000000 granny-pliers-0.0.14/src/granny_pliers/auth/auth_config.py
--rw-r--r--   0 pd         (501) staff       (20)      986 2023-06-10 13:13:15.000000 granny-pliers-0.0.14/src/granny_pliers/auth/auth_error.py
--rw-r--r--   0 pd         (501) staff       (20)     1308 2023-06-10 13:13:08.000000 granny-pliers-0.0.14/src/granny_pliers/auth/auth_request.py
--rw-r--r--   0 pd         (501) staff       (20)     1016 2023-06-10 13:11:55.000000 granny-pliers-0.0.14/src/granny_pliers/auth/auth_response.py
--rw-r--r--   0 pd         (501) staff       (20)     6158 2023-06-10 13:18:46.000000 granny-pliers-0.0.14/src/granny_pliers/auth/jwt.py
--rw-r--r--   0 pd         (501) staff       (20)      882 2023-06-10 11:26:21.000000 granny-pliers-0.0.14/src/granny_pliers/auth/permissions.py
--rw-r--r--   0 pd         (501) staff       (20)      828 2023-06-10 11:26:59.000000 granny-pliers-0.0.14/src/granny_pliers/auth/roles.py
--rw-r--r--   0 pd         (501) staff       (20)     9678 2023-06-10 13:14:07.000000 granny-pliers-0.0.14/src/granny_pliers/auth/rsa_codec.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 19:06:25.052590 granny-pliers-0.0.14/src/granny_pliers/config/
--rw-r--r--   0 pd         (501) staff       (20)      985 2023-06-04 16:29:44.000000 granny-pliers-0.0.14/src/granny_pliers/config/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     3198 2023-06-09 21:43:11.000000 granny-pliers-0.0.14/src/granny_pliers/config/abstract_config.py
--rw-r--r--   0 pd         (501) staff       (20)     1614 2023-06-03 23:39:30.000000 granny-pliers-0.0.14/src/granny_pliers/config/autowired_config.py
--rw-r--r--   0 pd         (501) staff       (20)     6694 2023-06-14 20:55:52.000000 granny-pliers-0.0.14/src/granny_pliers/config/logger_config.py
--rw-r--r--   0 pd         (501) staff       (20)      860 2023-06-03 18:43:25.000000 granny-pliers-0.0.14/src/granny_pliers/config/project_environment.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 19:06:25.055430 granny-pliers-0.0.14/src/granny_pliers/logger/
--rw-r--r--   0 pd         (501) staff       (20)      884 2023-06-04 16:29:44.000000 granny-pliers-0.0.14/src/granny_pliers/logger/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     1292 2023-06-03 18:43:25.000000 granny-pliers-0.0.14/src/granny_pliers/logger/abstract_logger.py
--rw-r--r--   0 pd         (501) staff       (20)     1253 2023-06-03 18:43:25.000000 granny-pliers-0.0.14/src/granny_pliers/logger/log_processors.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 19:06:25.056283 granny-pliers-0.0.14/src/granny_pliers/models/
--rw-r--r--   0 pd         (501) staff       (20)      620 2023-06-10 11:58:05.000000 granny-pliers-0.0.14/src/granny_pliers/models/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 19:06:25.057767 granny-pliers-0.0.14/src/granny_pliers/models/auth/
--rw-r--r--   0 pd         (501) staff       (20)      688 2023-06-10 13:33:22.000000 granny-pliers-0.0.14/src/granny_pliers/models/auth/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     2061 2023-06-10 13:36:39.000000 granny-pliers-0.0.14/src/granny_pliers/models/auth/user.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 19:06:25.059419 granny-pliers-0.0.14/src/granny_pliers/models/metrics/
--rw-r--r--   0 pd         (501) staff       (20)      715 2023-06-10 13:32:44.000000 granny-pliers-0.0.14/src/granny_pliers/models/metrics/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     2766 2023-06-10 13:33:13.000000 granny-pliers-0.0.14/src/granny_pliers/models/metrics/confusion_matrix.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 19:06:25.060975 granny-pliers-0.0.14/src/granny_pliers/models/web/
--rw-r--r--   0 pd         (501) staff       (20)      729 2023-06-10 13:36:51.000000 granny-pliers-0.0.14/src/granny_pliers/models/web/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     1645 2023-06-10 11:59:08.000000 granny-pliers-0.0.14/src/granny_pliers/models/web/web_service_health_status.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 19:06:25.065236 granny-pliers-0.0.14/src/granny_pliers/orm/
--rw-r--r--   0 pd         (501) staff       (20)     1222 2023-06-10 13:29:12.000000 granny-pliers-0.0.14/src/granny_pliers/orm/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     5494 2023-06-10 13:26:46.000000 granny-pliers-0.0.14/src/granny_pliers/orm/abstract_http_client.py
--rw-r--r--   0 pd         (501) staff       (20)     5956 2023-06-10 13:25:56.000000 granny-pliers-0.0.14/src/granny_pliers/orm/abstract_http_repository.py
--rw-r--r--   0 pd         (501) staff       (20)     3287 2023-07-01 17:54:45.000000 granny-pliers-0.0.14/src/granny_pliers/orm/abstract_model.py
--rw-r--r--   0 pd         (501) staff       (20)    19825 2023-07-01 18:02:54.000000 granny-pliers-0.0.14/src/granny_pliers/orm/abstract_mongo_repository.py
--rw-r--r--   0 pd         (501) staff       (20)     7523 2023-06-09 21:46:56.000000 granny-pliers-0.0.14/src/granny_pliers/orm/abstract_repository.py
--rw-r--r--   0 pd         (501) staff       (20)    14519 2023-06-10 17:09:48.000000 granny-pliers-0.0.14/src/granny_pliers/orm/restful_http_client.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 19:06:25.067215 granny-pliers-0.0.14/src/granny_pliers/scheduler/
--rw-r--r--   0 pd         (501) staff       (20)      194 2023-06-25 17:48:19.000000 granny-pliers-0.0.14/src/granny_pliers/scheduler/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     1154 2023-06-25 17:47:45.000000 granny-pliers-0.0.14/src/granny_pliers/scheduler/abstract_schedule_object.py
--rw-r--r--   0 pd         (501) staff       (20)     7068 2023-06-25 17:47:10.000000 granny-pliers-0.0.14/src/granny_pliers/scheduler/abstract_scheduler.py
--rw-r--r--   0 pd         (501) staff       (20)     4916 2023-06-25 17:44:42.000000 granny-pliers-0.0.14/src/granny_pliers/scheduler/time_table.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 19:06:25.069296 granny-pliers-0.0.14/src/granny_pliers/testing/
--rw-r--r--   0 pd         (501) staff       (20)      806 2023-06-04 16:29:44.000000 granny-pliers-0.0.14/src/granny_pliers/testing/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     1998 2023-06-10 12:35:19.000000 granny-pliers-0.0.14/src/granny_pliers/testing/abstract_test_case.py
--rw-r--r--   0 pd         (501) staff       (20)      914 2023-06-10 12:35:55.000000 granny-pliers-0.0.14/src/granny_pliers/testing/async_abstract_test_case.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 19:06:25.070986 granny-pliers-0.0.14/src/granny_pliers/tools/
--rw-r--r--   0 pd         (501) staff       (20)      711 2023-06-10 13:15:39.000000 granny-pliers-0.0.14/src/granny_pliers/tools/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     2271 2023-06-10 17:09:40.000000 granny-pliers-0.0.14/src/granny_pliers/tools/datetime_helper.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 19:06:25.073810 granny-pliers-0.0.14/src/granny_pliers/web/
--rw-r--r--   0 pd         (501) staff       (20)     1041 2023-06-10 13:18:21.000000 granny-pliers-0.0.14/src/granny_pliers/web/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     2135 2023-06-10 17:09:00.000000 granny-pliers-0.0.14/src/granny_pliers/web/abstract_status_web_service.py
--rw-r--r--   0 pd         (501) staff       (20)     4235 2023-06-10 13:21:16.000000 granny-pliers-0.0.14/src/granny_pliers/web/abstract_web_application.py
--rw-r--r--   0 pd         (501) staff       (20)    11869 2023-06-10 13:32:23.000000 granny-pliers-0.0.14/src/granny_pliers/web/abstract_web_service.py
--rw-r--r--   0 pd         (501) staff       (20)     1575 2023-06-15 19:06:25.000000 granny-pliers-0.0.14/src/granny_pliers/web/web_application_config.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 19:06:25.075431 granny-pliers-0.0.14/src/granny_pliers/worker/
--rw-r--r--   0 pd         (501) staff       (20)      713 2023-06-04 16:29:44.000000 granny-pliers-0.0.14/src/granny_pliers/worker/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     5086 2023-06-04 16:29:44.000000 granny-pliers-0.0.14/src/granny_pliers/worker/abstract_worker.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 19:06:25.039034 granny-pliers-0.0.14/src/granny_pliers.egg-info/
--rw-r--r--   0 pd         (501) staff       (20)    13701 2023-07-01 19:06:25.000000 granny-pliers-0.0.14/src/granny_pliers.egg-info/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)     2275 2023-07-01 19:06:25.000000 granny-pliers-0.0.14/src/granny_pliers.egg-info/SOURCES.txt
--rw-r--r--   0 pd         (501) staff       (20)        1 2023-07-01 19:06:25.000000 granny-pliers-0.0.14/src/granny_pliers.egg-info/dependency_links.txt
--rw-r--r--   0 pd         (501) staff       (20)      230 2023-07-01 19:06:25.000000 granny-pliers-0.0.14/src/granny_pliers.egg-info/requires.txt
--rw-r--r--   0 pd         (501) staff       (20)       14 2023-07-01 19:06:25.000000 granny-pliers-0.0.14/src/granny_pliers.egg-info/top_level.txt
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.471133 granny-pliers-0.0.9/
+-rw-r--r--   0 pd         (501) staff       (20)    11357 2023-06-03 18:43:25.000000 granny-pliers-0.0.9/LICENSE
+-rw-r--r--   0 pd         (501) staff       (20)    13700 2023-06-14 21:02:38.470754 granny-pliers-0.0.9/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)       16 2023-06-10 17:39:54.000000 granny-pliers-0.0.9/README.md
+-rw-r--r--   0 pd         (501) staff       (20)     1619 2023-06-14 20:50:52.000000 granny-pliers-0.0.9/pyproject.toml
+-rw-r--r--   0 pd         (501) staff       (20)       38 2023-06-14 21:02:38.471227 granny-pliers-0.0.9/setup.cfg
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.437214 granny-pliers-0.0.9/src/
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.440162 granny-pliers-0.0.9/src/granny_pliers/
+-rw-r--r--   0 pd         (501) staff       (20)      987 2023-06-14 20:51:00.000000 granny-pliers-0.0.9/src/granny_pliers/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.448122 granny-pliers-0.0.9/src/granny_pliers/auth/
+-rw-r--r--   0 pd         (501) staff       (20)     1228 2023-06-10 13:12:31.000000 granny-pliers-0.0.9/src/granny_pliers/auth/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     1683 2023-06-10 11:50:56.000000 granny-pliers-0.0.9/src/granny_pliers/auth/auth_config.py
+-rw-r--r--   0 pd         (501) staff       (20)      986 2023-06-10 13:13:15.000000 granny-pliers-0.0.9/src/granny_pliers/auth/auth_error.py
+-rw-r--r--   0 pd         (501) staff       (20)     1308 2023-06-10 13:13:08.000000 granny-pliers-0.0.9/src/granny_pliers/auth/auth_request.py
+-rw-r--r--   0 pd         (501) staff       (20)     1016 2023-06-10 13:11:55.000000 granny-pliers-0.0.9/src/granny_pliers/auth/auth_response.py
+-rw-r--r--   0 pd         (501) staff       (20)     6158 2023-06-10 13:18:46.000000 granny-pliers-0.0.9/src/granny_pliers/auth/jwt.py
+-rw-r--r--   0 pd         (501) staff       (20)      882 2023-06-10 11:26:21.000000 granny-pliers-0.0.9/src/granny_pliers/auth/permissions.py
+-rw-r--r--   0 pd         (501) staff       (20)      828 2023-06-10 11:26:59.000000 granny-pliers-0.0.9/src/granny_pliers/auth/roles.py
+-rw-r--r--   0 pd         (501) staff       (20)     9678 2023-06-10 13:14:07.000000 granny-pliers-0.0.9/src/granny_pliers/auth/rsa_codec.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.450537 granny-pliers-0.0.9/src/granny_pliers/config/
+-rw-r--r--   0 pd         (501) staff       (20)      985 2023-06-04 16:29:44.000000 granny-pliers-0.0.9/src/granny_pliers/config/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     3198 2023-06-09 21:43:11.000000 granny-pliers-0.0.9/src/granny_pliers/config/abstract_config.py
+-rw-r--r--   0 pd         (501) staff       (20)     1614 2023-06-03 23:39:30.000000 granny-pliers-0.0.9/src/granny_pliers/config/autowired_config.py
+-rw-r--r--   0 pd         (501) staff       (20)     6694 2023-06-14 20:55:52.000000 granny-pliers-0.0.9/src/granny_pliers/config/logger_config.py
+-rw-r--r--   0 pd         (501) staff       (20)      860 2023-06-03 18:43:25.000000 granny-pliers-0.0.9/src/granny_pliers/config/project_environment.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.452701 granny-pliers-0.0.9/src/granny_pliers/logger/
+-rw-r--r--   0 pd         (501) staff       (20)      884 2023-06-04 16:29:44.000000 granny-pliers-0.0.9/src/granny_pliers/logger/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     1292 2023-06-03 18:43:25.000000 granny-pliers-0.0.9/src/granny_pliers/logger/abstract_logger.py
+-rw-r--r--   0 pd         (501) staff       (20)     1253 2023-06-03 18:43:25.000000 granny-pliers-0.0.9/src/granny_pliers/logger/log_processors.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.453438 granny-pliers-0.0.9/src/granny_pliers/models/
+-rw-r--r--   0 pd         (501) staff       (20)      620 2023-06-10 11:58:05.000000 granny-pliers-0.0.9/src/granny_pliers/models/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.454935 granny-pliers-0.0.9/src/granny_pliers/models/auth/
+-rw-r--r--   0 pd         (501) staff       (20)      688 2023-06-10 13:33:22.000000 granny-pliers-0.0.9/src/granny_pliers/models/auth/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     2061 2023-06-10 13:36:39.000000 granny-pliers-0.0.9/src/granny_pliers/models/auth/user.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.456903 granny-pliers-0.0.9/src/granny_pliers/models/metrics/
+-rw-r--r--   0 pd         (501) staff       (20)      715 2023-06-10 13:32:44.000000 granny-pliers-0.0.9/src/granny_pliers/models/metrics/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     2766 2023-06-10 13:33:13.000000 granny-pliers-0.0.9/src/granny_pliers/models/metrics/confusion_matrix.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.458526 granny-pliers-0.0.9/src/granny_pliers/models/web/
+-rw-r--r--   0 pd         (501) staff       (20)      729 2023-06-10 13:36:51.000000 granny-pliers-0.0.9/src/granny_pliers/models/web/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     1645 2023-06-10 11:59:08.000000 granny-pliers-0.0.9/src/granny_pliers/models/web/web_service_health_status.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.462837 granny-pliers-0.0.9/src/granny_pliers/orm/
+-rw-r--r--   0 pd         (501) staff       (20)     1222 2023-06-10 13:29:12.000000 granny-pliers-0.0.9/src/granny_pliers/orm/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     5494 2023-06-10 13:26:46.000000 granny-pliers-0.0.9/src/granny_pliers/orm/abstract_http_client.py
+-rw-r--r--   0 pd         (501) staff       (20)     5956 2023-06-10 13:25:56.000000 granny-pliers-0.0.9/src/granny_pliers/orm/abstract_http_repository.py
+-rw-r--r--   0 pd         (501) staff       (20)     2990 2023-06-10 13:38:35.000000 granny-pliers-0.0.9/src/granny_pliers/orm/abstract_model.py
+-rw-r--r--   0 pd         (501) staff       (20)    19833 2023-06-10 13:36:11.000000 granny-pliers-0.0.9/src/granny_pliers/orm/abstract_mongo_repository.py
+-rw-r--r--   0 pd         (501) staff       (20)     7523 2023-06-09 21:46:56.000000 granny-pliers-0.0.9/src/granny_pliers/orm/abstract_repository.py
+-rw-r--r--   0 pd         (501) staff       (20)    14519 2023-06-10 17:09:48.000000 granny-pliers-0.0.9/src/granny_pliers/orm/restful_http_client.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.464681 granny-pliers-0.0.9/src/granny_pliers/testing/
+-rw-r--r--   0 pd         (501) staff       (20)      806 2023-06-04 16:29:44.000000 granny-pliers-0.0.9/src/granny_pliers/testing/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     1998 2023-06-10 12:35:19.000000 granny-pliers-0.0.9/src/granny_pliers/testing/abstract_test_case.py
+-rw-r--r--   0 pd         (501) staff       (20)      914 2023-06-10 12:35:55.000000 granny-pliers-0.0.9/src/granny_pliers/testing/async_abstract_test_case.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.466108 granny-pliers-0.0.9/src/granny_pliers/tools/
+-rw-r--r--   0 pd         (501) staff       (20)      711 2023-06-10 13:15:39.000000 granny-pliers-0.0.9/src/granny_pliers/tools/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     2271 2023-06-10 17:09:40.000000 granny-pliers-0.0.9/src/granny_pliers/tools/datetime_helper.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.468181 granny-pliers-0.0.9/src/granny_pliers/web/
+-rw-r--r--   0 pd         (501) staff       (20)     1041 2023-06-10 13:18:21.000000 granny-pliers-0.0.9/src/granny_pliers/web/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     2135 2023-06-10 17:09:00.000000 granny-pliers-0.0.9/src/granny_pliers/web/abstract_status_web_service.py
+-rw-r--r--   0 pd         (501) staff       (20)     4235 2023-06-10 13:21:16.000000 granny-pliers-0.0.9/src/granny_pliers/web/abstract_web_application.py
+-rw-r--r--   0 pd         (501) staff       (20)    11869 2023-06-10 13:32:23.000000 granny-pliers-0.0.9/src/granny_pliers/web/abstract_web_service.py
+-rw-r--r--   0 pd         (501) staff       (20)     1499 2023-06-10 12:04:19.000000 granny-pliers-0.0.9/src/granny_pliers/web/web_application_config.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.469771 granny-pliers-0.0.9/src/granny_pliers/worker/
+-rw-r--r--   0 pd         (501) staff       (20)      713 2023-06-04 16:29:44.000000 granny-pliers-0.0.9/src/granny_pliers/worker/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     5086 2023-06-04 16:29:44.000000 granny-pliers-0.0.9/src/granny_pliers/worker/abstract_worker.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.441760 granny-pliers-0.0.9/src/granny_pliers.egg-info/
+-rw-r--r--   0 pd         (501) staff       (20)    13700 2023-06-14 21:02:38.000000 granny-pliers-0.0.9/src/granny_pliers.egg-info/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)     2087 2023-06-14 21:02:38.000000 granny-pliers-0.0.9/src/granny_pliers.egg-info/SOURCES.txt
+-rw-r--r--   0 pd         (501) staff       (20)        1 2023-06-14 21:02:38.000000 granny-pliers-0.0.9/src/granny_pliers.egg-info/dependency_links.txt
+-rw-r--r--   0 pd         (501) staff       (20)      230 2023-06-14 21:02:38.000000 granny-pliers-0.0.9/src/granny_pliers.egg-info/requires.txt
+-rw-r--r--   0 pd         (501) staff       (20)       14 2023-06-14 21:02:38.000000 granny-pliers-0.0.9/src/granny_pliers.egg-info/top_level.txt
```

### Comparing `granny-pliers-0.0.14/LICENSE` & `granny-pliers-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/PKG-INFO` & `granny-pliers-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granny-pliers
-Version: 0.0.14
+Version: 0.0.9
 Summary: Set of tools
 Author-email: Dmytro Stepanenko <dmitrijstepanenko@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `granny-pliers-0.0.14/pyproject.toml` & `granny-pliers-0.0.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "granny-pliers"
-version = "0.0.14"
+version = "0.0.9"
 
 authors = [
     { name = "Dmytro Stepanenko", email = "dmitrijstepanenko@gmail.com" },
 ]
 
 license = { file = "LICENSE" }
 
@@ -37,24 +37,24 @@
     "colorama>=0.4.6",
     "jsonplus>=0.8.0",
     "cryptography>=41.0.1",
     "aiohttp>=3.8.4",
     "aiofiles>=23.1.0",
     "dateparser>=1.1.8",
     "PyYAML>=6.0",
-    "motor==3.2.0",
+    "motor==3.1.2",
 ]
 
 [project.optional-dependencies]
 # Dev dependencies.
 dev = [
     "black>=22.3.0",
     "pylint>=2.17.4",
     "coverage>=7.2.7",
-    "pytest>=7.4.0",
+    "pytest>=7.3.1",
     "pytest-cov==4.1.0"
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/stepanenko-family/shared/granny-pliers.git"
 
 [tool.black]
```

### Comparing `granny-pliers-0.0.14/src/granny_pliers/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """Granny Pliers is a Python library that contains a collection of useful
 and helpful tools, designed to simplify developers' lives."""
 
-__version__ = "0.0.14"
+__version__ = "0.0.9"
 __author__ = "Dmytro Stepanenko"
 __copyright__ = "Copyright 2022, Dmytro Stepanenko, Granny Pliers"
 __credits__ = ["Dmytro Stepanenko"]
 __license__ = "Apache License Version 2.0"
 __email__ = "dmitrijstepanenko@gmail.com"
```

### Comparing `granny-pliers-0.0.14/src/granny_pliers/auth/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/auth/auth_config.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/auth_config.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/auth/auth_error.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/auth_error.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/auth/auth_request.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/auth_request.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/auth/auth_response.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/auth_response.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/auth/jwt.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/auth/permissions.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/auth/roles.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/roles.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/auth/rsa_codec.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/rsa_codec.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/config/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/config/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/config/abstract_config.py` & `granny-pliers-0.0.9/src/granny_pliers/config/abstract_config.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/config/autowired_config.py` & `granny-pliers-0.0.9/src/granny_pliers/config/autowired_config.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/config/logger_config.py` & `granny-pliers-0.0.9/src/granny_pliers/config/logger_config.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/config/project_environment.py` & `granny-pliers-0.0.9/src/granny_pliers/config/project_environment.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/logger/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/logger/abstract_logger.py` & `granny-pliers-0.0.9/src/granny_pliers/logger/abstract_logger.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/logger/log_processors.py` & `granny-pliers-0.0.9/src/granny_pliers/logger/log_processors.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/models/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/models/auth/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/models/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/models/auth/user.py` & `granny-pliers-0.0.9/src/granny_pliers/models/auth/user.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/models/metrics/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/models/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/models/metrics/confusion_matrix.py` & `granny-pliers-0.0.9/src/granny_pliers/models/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/models/web/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/models/web/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/models/web/web_service_health_status.py` & `granny-pliers-0.0.9/src/granny_pliers/models/web/web_service_health_status.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/orm/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/orm/abstract_http_client.py` & `granny-pliers-0.0.9/src/granny_pliers/orm/abstract_http_client.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/orm/abstract_http_repository.py` & `granny-pliers-0.0.9/src/granny_pliers/orm/abstract_http_repository.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/orm/abstract_model.py` & `granny-pliers-0.0.9/src/granny_pliers/orm/abstract_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """BaseModel"""
 
 from dataclasses import dataclass, fields, field
 from datetime import datetime
-from enum import Enum
 from typing import TypeVar, Generic
 
 import jsonplus
 
 __all__ = ["BaseModel", "base_model_encoder", "AbstractModel", "ModelsPage", "ModelsCount"]
 
 from bson import ObjectId
@@ -105,19 +104,13 @@
 
     :param obj:
     :return: dict
     """
     obj_dict = {}
     for cls_field in fields(obj):
         if cls_field.type is ObjectId:
-            value = str(getattr(obj, cls_field.name))
-            if value is None:
-                obj_dict[cls_field.name] = None
-            else:
-                obj_dict[cls_field.name] = str(getattr(obj, cls_field.name))
+            obj_dict[cls_field.name] = str(getattr(obj, cls_field.name))
         elif cls_field.type is tuple:
             obj_dict[cls_field.name] = str(getattr(obj, cls_field.name))
-        elif issubclass(cls_field.type, Enum):
-            obj_dict[cls_field.name] = getattr(obj, cls_field.name).value
         else:
             obj_dict[cls_field.name] = getattr(obj, cls_field.name)
     return obj_dict
```

### Comparing `granny-pliers-0.0.14/src/granny_pliers/orm/abstract_mongo_repository.py` & `granny-pliers-0.0.9/src/granny_pliers/orm/abstract_mongo_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         if self.__client is not None:
             self.__client.close()
             self.__client = None
 
     def _fallback_encoder(self, value):
         try:
             if isinstance(value, Enum):
-                return value.value
+                return asdict(value.value)
             else:
                 # Python datetime to BSON DateTime encoder
                 return setup_datetime(value)
         except TypeError as error:
             self.log.error("_fallback_encoder", error=error)
 
     @staticmethod
```

### Comparing `granny-pliers-0.0.14/src/granny_pliers/orm/abstract_repository.py` & `granny-pliers-0.0.9/src/granny_pliers/orm/abstract_repository.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/orm/restful_http_client.py` & `granny-pliers-0.0.9/src/granny_pliers/orm/restful_http_client.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/testing/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/testing/abstract_test_case.py` & `granny-pliers-0.0.9/src/granny_pliers/testing/abstract_test_case.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/testing/async_abstract_test_case.py` & `granny-pliers-0.0.9/src/granny_pliers/testing/async_abstract_test_case.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/tools/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/tools/datetime_helper.py` & `granny-pliers-0.0.9/src/granny_pliers/tools/datetime_helper.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/web/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/web/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/web/abstract_status_web_service.py` & `granny-pliers-0.0.9/src/granny_pliers/web/abstract_status_web_service.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/web/abstract_web_application.py` & `granny-pliers-0.0.9/src/granny_pliers/web/abstract_web_application.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/web/abstract_web_service.py` & `granny-pliers-0.0.9/src/granny_pliers/web/abstract_web_service.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/web/web_application_config.py` & `granny-pliers-0.0.9/src/granny_pliers/web/web_application_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,18 +22,15 @@
 __all__ = ["WebApplicationConfig"]
 
 
 @dataclass()
 class WebApplicationConfig(AbstractConfig):
     """WebApplicationConfig"""
 
-    auth: AuthConfig = field(
-        default="localhost",
-        metadata={"type": AuthConfig},
-    )
+    auth: AuthConfig = None
 
     host: str = field(
         default="localhost",
         metadata={"env_var_name": "WEB_HOST", "type": str},
     )
     port: int = field(
         default=8080,
```

### Comparing `granny-pliers-0.0.14/src/granny_pliers/worker/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers/worker/abstract_worker.py` & `granny-pliers-0.0.9/src/granny_pliers/worker/abstract_worker.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.14/src/granny_pliers.egg-info/PKG-INFO` & `granny-pliers-0.0.9/src/granny_pliers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granny-pliers
-Version: 0.0.14
+Version: 0.0.9
 Summary: Set of tools
 Author-email: Dmytro Stepanenko <dmitrijstepanenko@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `granny-pliers-0.0.14/src/granny_pliers.egg-info/SOURCES.txt` & `granny-pliers-0.0.9/src/granny_pliers.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,18 +34,14 @@
 src/granny_pliers/orm/__init__.py
 src/granny_pliers/orm/abstract_http_client.py
 src/granny_pliers/orm/abstract_http_repository.py
 src/granny_pliers/orm/abstract_model.py
 src/granny_pliers/orm/abstract_mongo_repository.py
 src/granny_pliers/orm/abstract_repository.py
 src/granny_pliers/orm/restful_http_client.py
-src/granny_pliers/scheduler/__init__.py
-src/granny_pliers/scheduler/abstract_schedule_object.py
-src/granny_pliers/scheduler/abstract_scheduler.py
-src/granny_pliers/scheduler/time_table.py
 src/granny_pliers/testing/__init__.py
 src/granny_pliers/testing/abstract_test_case.py
 src/granny_pliers/testing/async_abstract_test_case.py
 src/granny_pliers/tools/__init__.py
 src/granny_pliers/tools/datetime_helper.py
 src/granny_pliers/web/__init__.py
 src/granny_pliers/web/abstract_status_web_service.py
```

