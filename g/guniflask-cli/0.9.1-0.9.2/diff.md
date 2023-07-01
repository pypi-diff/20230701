# Comparing `tmp/guniflask-cli-0.9.1.tar.gz` & `tmp/guniflask-cli-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/guniflask-cli-0.9.1.tar", last modified: Wed Sep 16 07:55:15 2020, max compression
+gzip compressed data, was "dist/guniflask-cli-0.9.2.tar", last modified: Thu Sep 17 13:07:19 2020, max compression
```

## Comparing `guniflask-cli-0.9.1.tar` & `guniflask-cli-0.9.2.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/
--rw-r--r--   0 jadbin     (501) staff       (20)     1063 2020-08-06 02:10:40.000000 guniflask-cli-0.9.1/LICENSE
--rw-r--r--   0 jadbin     (501) staff       (20)      128 2020-08-06 02:10:40.000000 guniflask-cli-0.9.1/MANIFEST.in
--rw-r--r--   0 jadbin     (501) staff       (20)     1457 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/PKG-INFO
--rw-r--r--   0 jadbin     (501) staff       (20)      666 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/README.rst
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/guniflask_cli/
--rw-r--r--   0 jadbin     (501) staff       (20)       38 2020-09-16 07:47:45.000000 guniflask-cli-0.9.1/guniflask_cli/__init__.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/guniflask_cli/commands/
--rw-r--r--   0 jadbin     (501) staff       (20)       15 2020-08-06 02:10:40.000000 guniflask-cli-0.9.1/guniflask_cli/commands/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)      483 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/commands/base.py
--rw-r--r--   0 jadbin     (501) staff       (20)      998 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/commands/debug.py
--rw-r--r--   0 jadbin     (501) staff       (20)    12618 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/commands/init.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1426 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/commands/restart.py
--rw-r--r--   0 jadbin     (501) staff       (20)      965 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/commands/start.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1624 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/commands/stop.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2833 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/commands/table2model.py
--rw-r--r--   0 jadbin     (501) staff       (20)      485 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/commands/version.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2455 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/config.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2654 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/env.py
--rw-r--r--   0 jadbin     (501) staff       (20)      352 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/errors.py
--rw-r--r--   0 jadbin     (501) staff       (20)     4976 2020-09-16 07:43:10.000000 guniflask-cli-0.9.1/guniflask_cli/gunicorn.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1864 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/main.py
--rw-r--r--   0 jadbin     (501) staff       (20)    12861 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/sqlgen.py
--rw-r--r--   0 jadbin     (501) staff       (20)     5754 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/step.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/guniflask_cli/templates/
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/
--rw-r--r--   0 jadbin     (501) staff       (20)      117 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/.dockerignore
--rw-r--r--   0 jadbin     (501) staff       (20)      112 2020-08-06 02:10:40.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/.gitignore
--rw-r--r--   0 jadbin     (501) staff       (20)      196 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/Dockerfile.jinja2
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/_project_name/
--rw-r--r--   0 jadbin     (501) staff       (20)       52 2020-08-06 02:10:40.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/_project_name/__init__.py.jinja2
--rw-r--r--   0 jadbin     (501) staff       (20)      481 2020-08-06 02:10:40.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/_project_name/app.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/_project_name/config/
--rw-r--r--   0 jadbin     (501) staff       (20)       15 2020-08-06 02:10:40.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/_project_name/config/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1228 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/_project_name/config/jwt_config.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1444 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/_project_name/config/microservice_config.py
--rw-r--r--   0 jadbin     (501) staff       (20)      701 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/_project_name/config/security_config.py.jinja2
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/bin/
--rw-r--r--   0 jadbin     (501) staff       (20)       90 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/bin/manage
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/conf/
--rw-r--r--   0 jadbin     (501) staff       (20)      475 2020-08-06 02:10:40.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/conf/_project_name.py.jinja2
--rw-r--r--   0 jadbin     (501) staff       (20)       40 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/conf/app.env.jinja2
--rw-r--r--   0 jadbin     (501) staff       (20)       42 2020-08-06 02:10:40.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/conf/gunicorn.py.jinja2
--rw-r--r--   0 jadbin     (501) staff       (20)       93 2020-08-06 02:10:40.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/docker-compose.yml.jinja2
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/requirements/
--rw-r--r--   0 jadbin     (501) staff       (20)      107 2020-08-06 02:10:40.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/requirements/app.txt.jinja2
--rw-r--r--   0 jadbin     (501) staff       (20)       18 2020-08-06 02:10:40.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/requirements/test.txt
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/tests/
--rw-r--r--   0 jadbin     (501) staff       (20)       15 2020-08-06 02:10:40.000000 guniflask-cli-0.9.1/guniflask_cli/templates/project/tests/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2491 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/guniflask_cli/utils.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/guniflask_cli.egg-info/
--rw-r--r--   0 jadbin     (501) staff       (20)     1457 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/guniflask_cli.egg-info/PKG-INFO
--rw-r--r--   0 jadbin     (501) staff       (20)     1854 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/guniflask_cli.egg-info/SOURCES.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        1 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/guniflask_cli.egg-info/dependency_links.txt
--rw-r--r--   0 jadbin     (501) staff       (20)       55 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/guniflask_cli.egg-info/entry_points.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        1 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/guniflask_cli.egg-info/not-zip-safe
--rw-r--r--   0 jadbin     (501) staff       (20)      140 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/guniflask_cli.egg-info/requires.txt
--rw-r--r--   0 jadbin     (501) staff       (20)       14 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/guniflask_cli.egg-info/top_level.txt
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/requirements/
--rw-r--r--   0 jadbin     (501) staff       (20)       18 2020-08-06 02:10:40.000000 guniflask-cli-0.9.1/requirements/test.txt
--rw-r--r--   0 jadbin     (501) staff       (20)       38 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/setup.cfg
--rw-r--r--   0 jadbin     (501) staff       (20)     2343 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/setup.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:55:15.000000 guniflask-cli-0.9.1/tests/
--rw-r--r--   0 jadbin     (501) staff       (20)       15 2020-08-06 02:10:40.000000 guniflask-cli-0.9.1/tests/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)      767 2020-09-15 17:23:47.000000 guniflask-cli-0.9.1/tests/test_init_project.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/
+-rw-r--r--   0 jadbin     (501) staff       (20)     1063 2020-08-06 02:10:40.000000 guniflask-cli-0.9.2/LICENSE
+-rw-r--r--   0 jadbin     (501) staff       (20)      128 2020-08-06 02:10:40.000000 guniflask-cli-0.9.2/MANIFEST.in
+-rw-r--r--   0 jadbin     (501) staff       (20)     1457 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/PKG-INFO
+-rw-r--r--   0 jadbin     (501) staff       (20)      666 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/README.rst
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/guniflask_cli/
+-rw-r--r--   0 jadbin     (501) staff       (20)       38 2020-09-17 13:05:19.000000 guniflask-cli-0.9.2/guniflask_cli/__init__.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/guniflask_cli/commands/
+-rw-r--r--   0 jadbin     (501) staff       (20)       15 2020-08-06 02:10:40.000000 guniflask-cli-0.9.2/guniflask_cli/commands/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      483 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/guniflask_cli/commands/base.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      998 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/guniflask_cli/commands/debug.py
+-rw-r--r--   0 jadbin     (501) staff       (20)    12618 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/guniflask_cli/commands/init.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1426 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/guniflask_cli/commands/restart.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      965 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/guniflask_cli/commands/start.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1624 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/guniflask_cli/commands/stop.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2833 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/guniflask_cli/commands/table2model.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      485 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/guniflask_cli/commands/version.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2455 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/guniflask_cli/config.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2654 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/guniflask_cli/env.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      352 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/guniflask_cli/errors.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     4982 2020-09-17 10:33:49.000000 guniflask-cli-0.9.2/guniflask_cli/gunicorn.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1864 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/guniflask_cli/main.py
+-rw-r--r--   0 jadbin     (501) staff       (20)    12851 2020-09-17 06:08:04.000000 guniflask-cli-0.9.2/guniflask_cli/sqlgen.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     5754 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/guniflask_cli/step.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/guniflask_cli/templates/
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/
+-rw-r--r--   0 jadbin     (501) staff       (20)      117 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/.dockerignore
+-rw-r--r--   0 jadbin     (501) staff       (20)      112 2020-08-06 02:10:40.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/.gitignore
+-rw-r--r--   0 jadbin     (501) staff       (20)      196 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/Dockerfile.jinja2
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/_project_name/
+-rw-r--r--   0 jadbin     (501) staff       (20)       52 2020-08-06 02:10:40.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/_project_name/__init__.py.jinja2
+-rw-r--r--   0 jadbin     (501) staff       (20)      481 2020-08-06 02:10:40.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/_project_name/app.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/_project_name/config/
+-rw-r--r--   0 jadbin     (501) staff       (20)       15 2020-08-06 02:10:40.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/_project_name/config/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1228 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/_project_name/config/jwt_config.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1444 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/_project_name/config/microservice_config.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      701 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/_project_name/config/security_config.py.jinja2
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/bin/
+-rw-r--r--   0 jadbin     (501) staff       (20)       90 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/bin/manage
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/conf/
+-rw-r--r--   0 jadbin     (501) staff       (20)      475 2020-08-06 02:10:40.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/conf/_project_name.py.jinja2
+-rw-r--r--   0 jadbin     (501) staff       (20)       40 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/conf/app.env.jinja2
+-rw-r--r--   0 jadbin     (501) staff       (20)       42 2020-08-06 02:10:40.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/conf/gunicorn.py.jinja2
+-rw-r--r--   0 jadbin     (501) staff       (20)       93 2020-08-06 02:10:40.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/docker-compose.yml.jinja2
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/requirements/
+-rw-r--r--   0 jadbin     (501) staff       (20)      107 2020-08-06 02:10:40.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/requirements/app.txt.jinja2
+-rw-r--r--   0 jadbin     (501) staff       (20)       18 2020-08-06 02:10:40.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/requirements/test.txt
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/tests/
+-rw-r--r--   0 jadbin     (501) staff       (20)       15 2020-08-06 02:10:40.000000 guniflask-cli-0.9.2/guniflask_cli/templates/project/tests/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2491 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/guniflask_cli/utils.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2752 2020-09-17 12:59:49.000000 guniflask-cli-0.9.2/guniflask_cli/workers.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/guniflask_cli.egg-info/
+-rw-r--r--   0 jadbin     (501) staff       (20)     1457 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/guniflask_cli.egg-info/PKG-INFO
+-rw-r--r--   0 jadbin     (501) staff       (20)     1879 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/guniflask_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)        1 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/guniflask_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)       55 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/guniflask_cli.egg-info/entry_points.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)        1 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/guniflask_cli.egg-info/not-zip-safe
+-rw-r--r--   0 jadbin     (501) staff       (20)      140 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/guniflask_cli.egg-info/requires.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)       14 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/guniflask_cli.egg-info/top_level.txt
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/requirements/
+-rw-r--r--   0 jadbin     (501) staff       (20)       18 2020-08-06 02:10:40.000000 guniflask-cli-0.9.2/requirements/test.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)       38 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/setup.cfg
+-rw-r--r--   0 jadbin     (501) staff       (20)     2343 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/setup.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:07:19.000000 guniflask-cli-0.9.2/tests/
+-rw-r--r--   0 jadbin     (501) staff       (20)       15 2020-08-06 02:10:40.000000 guniflask-cli-0.9.2/tests/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      767 2020-09-15 17:23:47.000000 guniflask-cli-0.9.2/tests/test_init_project.py
```

### Comparing `guniflask-cli-0.9.1/LICENSE` & `guniflask-cli-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `guniflask-cli-0.9.1/PKG-INFO` & `guniflask-cli-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: guniflask-cli
-Version: 0.9.1
+Version: 0.9.2
 Summary: Standard tooling for Flask development with guniflask
 Home-page: https://github.com/jadbin/guniflask-cli
 Author: jadbin
 Author-email: jadbin.com@hotmail.com
 License: MIT
 Description: =============
         guniflask-cli
```

### Comparing `guniflask-cli-0.9.1/README.rst` & `guniflask-cli-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `guniflask-cli-0.9.1/guniflask_cli/commands/debug.py` & `guniflask-cli-0.9.2/guniflask_cli/commands/debug.py`

 * *Files identical despite different names*

### Comparing `guniflask-cli-0.9.1/guniflask_cli/commands/init.py` & `guniflask-cli-0.9.2/guniflask_cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `guniflask-cli-0.9.1/guniflask_cli/commands/restart.py` & `guniflask-cli-0.9.2/guniflask_cli/commands/restart.py`

 * *Files identical despite different names*

### Comparing `guniflask-cli-0.9.1/guniflask_cli/commands/start.py` & `guniflask-cli-0.9.2/guniflask_cli/commands/start.py`

 * *Files identical despite different names*

### Comparing `guniflask-cli-0.9.1/guniflask_cli/commands/stop.py` & `guniflask-cli-0.9.2/guniflask_cli/commands/stop.py`

 * *Files identical despite different names*

### Comparing `guniflask-cli-0.9.1/guniflask_cli/commands/table2model.py` & `guniflask-cli-0.9.2/guniflask_cli/commands/table2model.py`

 * *Files identical despite different names*

### Comparing `guniflask-cli-0.9.1/guniflask_cli/config.py` & `guniflask-cli-0.9.2/guniflask_cli/config.py`

 * *Files identical despite different names*

### Comparing `guniflask-cli-0.9.1/guniflask_cli/env.py` & `guniflask-cli-0.9.2/guniflask_cli/env.py`

 * *Files identical despite different names*

### Comparing `guniflask-cli-0.9.1/guniflask_cli/gunicorn.py` & `guniflask-cli-0.9.2/guniflask_cli/gunicorn.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         pid_dir = os.environ['GUNIFLASK_PID_DIR']
         log_dir = os.environ['GUNIFLASK_LOG_DIR']
         project_name = get_project_name_from_env()
         username = getpass.getuser()
         options = {
             'daemon': True,
             'workers': os.cpu_count(),
-            'worker_class': 'uvicorn.workers.UvicornWorker',
+            'worker_class': 'guniflask_cli.workers.UvicornWorker',
             'accesslog': join(log_dir, f'{project_name}-{username}.access.log'),
             'errorlog': join(log_dir, f'{project_name}-{username}.error.log'),
             'proc_name': project_name
         }
         profile_options = self._make_profile_options(os.environ.get('GUNIFLASK_ACTIVE_PROFILES'))
         if 'worker_class' in profile_options and profile_options['worker_class'] != options['worker_class']:
             raise ValueError(f'worker_class cannot be set to: {profile_options["worker_class"]}')
```

### Comparing `guniflask-cli-0.9.1/guniflask_cli/main.py` & `guniflask-cli-0.9.2/guniflask_cli/main.py`

 * *Files identical despite different names*

### Comparing `guniflask-cli-0.9.1/guniflask_cli/sqlgen.py` & `guniflask-cli-0.9.2/guniflask_cli/sqlgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # coding=utf-8
 
 import os
 from os.path import join, exists
 from collections import defaultdict
 from keyword import iskeyword
-import re
 import inspect
 from typing import Any, Union
 
 import sqlalchemy
 from sqlalchemy import ForeignKeyConstraint, UniqueConstraint, PrimaryKeyConstraint, CheckConstraint, ForeignKey
 import inflect
 from sqlalchemy.util import OrderedDict
```

### Comparing `guniflask-cli-0.9.1/guniflask_cli/step.py` & `guniflask-cli-0.9.2/guniflask_cli/step.py`

 * *Files identical despite different names*

### Comparing `guniflask-cli-0.9.1/guniflask_cli/templates/project/_project_name/config/jwt_config.py` & `guniflask-cli-0.9.2/guniflask_cli/templates/project/_project_name/config/jwt_config.py`

 * *Files identical despite different names*

### Comparing `guniflask-cli-0.9.1/guniflask_cli/templates/project/_project_name/config/microservice_config.py` & `guniflask-cli-0.9.2/guniflask_cli/templates/project/_project_name/config/microservice_config.py`

 * *Files identical despite different names*

### Comparing `guniflask-cli-0.9.1/guniflask_cli/templates/project/_project_name/config/security_config.py.jinja2` & `guniflask-cli-0.9.2/guniflask_cli/templates/project/_project_name/config/security_config.py.jinja2`

 * *Files identical despite different names*

### Comparing `guniflask-cli-0.9.1/guniflask_cli/utils.py` & `guniflask-cli-0.9.2/guniflask_cli/utils.py`

 * *Files identical despite different names*

### Comparing `guniflask-cli-0.9.1/guniflask_cli.egg-info/PKG-INFO` & `guniflask-cli-0.9.2/guniflask_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: guniflask-cli
-Version: 0.9.1
+Version: 0.9.2
 Summary: Standard tooling for Flask development with guniflask
 Home-page: https://github.com/jadbin/guniflask-cli
 Author: jadbin
 Author-email: jadbin.com@hotmail.com
 License: MIT
 Description: =============
         guniflask-cli
```

### Comparing `guniflask-cli-0.9.1/guniflask_cli.egg-info/SOURCES.txt` & `guniflask-cli-0.9.2/guniflask_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 guniflask_cli/env.py
 guniflask_cli/errors.py
 guniflask_cli/gunicorn.py
 guniflask_cli/main.py
 guniflask_cli/sqlgen.py
 guniflask_cli/step.py
 guniflask_cli/utils.py
+guniflask_cli/workers.py
 guniflask_cli.egg-info/PKG-INFO
 guniflask_cli.egg-info/SOURCES.txt
 guniflask_cli.egg-info/dependency_links.txt
 guniflask_cli.egg-info/entry_points.txt
 guniflask_cli.egg-info/not-zip-safe
 guniflask_cli.egg-info/requires.txt
 guniflask_cli.egg-info/top_level.txt
```

### Comparing `guniflask-cli-0.9.1/setup.py` & `guniflask-cli-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `guniflask-cli-0.9.1/tests/test_init_project.py` & `guniflask-cli-0.9.2/tests/test_init_project.py`

 * *Files identical despite different names*

