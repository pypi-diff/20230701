# Comparing `tmp/frequenz-repo-config-0.2.0.tar.gz` & `tmp/frequenz-repo-config-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-repo-config-0.2.0.tar", last modified: Fri May 26 09:41:45 2023, max compression
+gzip compressed data, was "frequenz-repo-config-0.3.0.tar", last modified: Sat Jul  1 07:04:01 2023, max compression
```

## Comparing `frequenz-repo-config-0.2.0.tar` & `frequenz-repo-config-0.3.0.tar`

### file list

```diff
@@ -1,68 +1,127 @@
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.131061 frequenz-repo-config-0.2.0/
--rw-r--r--   0 luca      (1000) luca      (1000)       34 2023-04-03 13:31:43.000000 frequenz-repo-config-0.2.0/.darglint
--rw-r--r--   0 luca      (1000) luca      (1000)     2134 2023-03-10 15:07:55.000000 frequenz-repo-config-0.2.0/.gitignore
--rw-r--r--   0 luca      (1000) luca      (1000)     1090 2023-03-31 14:27:27.000000 frequenz-repo-config-0.2.0/LICENSE
--rw-r--r--   0 luca      (1000) luca      (1000)     2907 2023-05-26 09:41:45.131061 frequenz-repo-config-0.2.0/PKG-INFO
--rw-r--r--   0 luca      (1000) luca      (1000)     1488 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/README.md
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.123061 frequenz-repo-config-0.2.0/cookiecutter/
--rw-r--r--   0 luca      (1000) luca      (1000)      740 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.123061 frequenz-repo-config-0.2.0/cookiecutter/hooks/
--rw-r--r--   0 luca      (1000) luca      (1000)    13771 2023-05-26 09:40:07.000000 frequenz-repo-config-0.2.0/cookiecutter/hooks/post_gen_project.py
--rw-r--r--   0 luca      (1000) luca      (1000)     3001 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/cookiecutter/local_extensions.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.127061 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/
--rw-r--r--   0 luca      (1000) luca      (1000)     2134 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/.gitignore
--rw-r--r--   0 luca      (1000) luca      (1000)      316 2023-05-26 09:40:07.000000 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/.gitmodules
--rw-r--r--   0 luca      (1000) luca      (1000)     1090 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/LICENSE
--rw-r--r--   0 luca      (1000) luca      (1000)      130 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/README.md
--rw-r--r--   0 luca      (1000) luca      (1000)      216 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/noxfile.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.123061 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.123061 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/frequenz/
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.123061 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/frequenz/api/
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.127061 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/frequenz/api/{{cookiecutter.name}}/
--rw-r--r--   0 luca      (1000) luca      (1000)      433 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/frequenz/api/{{cookiecutter.name}}/{{cookiecutter.name}}.proto
--rw-r--r--   0 luca      (1000) luca      (1000)     4317 2023-05-26 09:40:07.000000 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/pyproject.toml
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.123061 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.123061 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.123061 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.127061 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name}}/
--rw-r--r--   0 luca      (1000) luca      (1000)      646 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name}}/__init__.py
--rw-r--r--   0 luca      (1000) luca      (1000)        0 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name}}/py.typed
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.127061 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/tests/
--rw-r--r--   0 luca      (1000) luca      (1000)     1361 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/tests/test_{{cookiecutter.name}}.py
--rw-r--r--   0 luca      (1000) luca      (1000)      335 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/noxfile.py
--rw-r--r--   0 luca      (1000) luca      (1000)     3184 2023-05-24 13:58:13.000000 frequenz-repo-config-0.2.0/pyproject.toml
--rw-r--r--   0 luca      (1000) luca      (1000)       38 2023-05-26 09:41:45.131061 frequenz-repo-config-0.2.0/setup.cfg
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.123061 frequenz-repo-config-0.2.0/src/
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.127061 frequenz-repo-config-0.2.0/src/frequenz/
--rw-r--r--   0 luca      (1000) luca      (1000)        0 2023-04-13 14:08:23.000000 frequenz-repo-config-0.2.0/src/frequenz/py.typed
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.123061 frequenz-repo-config-0.2.0/src/frequenz/repo/
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.127061 frequenz-repo-config-0.2.0/src/frequenz/repo/config/
--rw-r--r--   0 luca      (1000) luca      (1000)     8427 2023-05-26 09:40:07.000000 frequenz-repo-config-0.2.0/src/frequenz/repo/config/__init__.py
--rw-r--r--   0 luca      (1000) luca      (1000)      501 2023-05-17 11:36:59.000000 frequenz-repo-config-0.2.0/src/frequenz/repo/config/_core.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.127061 frequenz-repo-config-0.2.0/src/frequenz/repo/config/nox/
--rw-r--r--   0 luca      (1000) luca      (1000)     1478 2023-03-31 14:27:27.000000 frequenz-repo-config-0.2.0/src/frequenz/repo/config/nox/__init__.py
--rw-r--r--   0 luca      (1000) luca      (1000)     6257 2023-05-25 10:46:13.000000 frequenz-repo-config-0.2.0/src/frequenz/repo/config/nox/config.py
--rw-r--r--   0 luca      (1000) luca      (1000)     3708 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/src/frequenz/repo/config/nox/default.py
--rw-r--r--   0 luca      (1000) luca      (1000)     4996 2023-05-17 11:36:59.000000 frequenz-repo-config-0.2.0/src/frequenz/repo/config/nox/session.py
--rw-r--r--   0 luca      (1000) luca      (1000)     6943 2023-05-24 13:01:23.000000 frequenz-repo-config-0.2.0/src/frequenz/repo/config/nox/util.py
--rw-r--r--   0 luca      (1000) luca      (1000)        0 2023-05-08 13:51:55.000000 frequenz-repo-config-0.2.0/src/frequenz/repo/config/py.typed
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.131061 frequenz-repo-config-0.2.0/src/frequenz/repo/config/setuptools/
--rw-r--r--   0 luca      (1000) luca      (1000)      157 2023-03-30 12:38:00.000000 frequenz-repo-config-0.2.0/src/frequenz/repo/config/setuptools/__init__.py
--rw-r--r--   0 luca      (1000) luca      (1000)     5305 2023-05-26 09:40:07.000000 frequenz-repo-config-0.2.0/src/frequenz/repo/config/setuptools/grpc_tools.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.131061 frequenz-repo-config-0.2.0/src/frequenz_repo_config.egg-info/
--rw-r--r--   0 luca      (1000) luca      (1000)     2907 2023-05-26 09:41:45.000000 frequenz-repo-config-0.2.0/src/frequenz_repo_config.egg-info/PKG-INFO
--rw-r--r--   0 luca      (1000) luca      (1000)     1830 2023-05-26 09:41:45.000000 frequenz-repo-config-0.2.0/src/frequenz_repo_config.egg-info/SOURCES.txt
--rw-r--r--   0 luca      (1000) luca      (1000)        1 2023-05-26 09:41:45.000000 frequenz-repo-config-0.2.0/src/frequenz_repo_config.egg-info/dependency_links.txt
--rw-r--r--   0 luca      (1000) luca      (1000)       93 2023-05-26 09:41:45.000000 frequenz-repo-config-0.2.0/src/frequenz_repo_config.egg-info/entry_points.txt
--rw-r--r--   0 luca      (1000) luca      (1000)      759 2023-05-26 09:41:45.000000 frequenz-repo-config-0.2.0/src/frequenz_repo_config.egg-info/requires.txt
--rw-r--r--   0 luca      (1000) luca      (1000)        9 2023-05-26 09:41:45.000000 frequenz-repo-config-0.2.0/src/frequenz_repo_config.egg-info/top_level.txt
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.131061 frequenz-repo-config-0.2.0/tests/
--rw-r--r--   0 luca      (1000) luca      (1000)      102 2023-05-17 11:36:44.000000 frequenz-repo-config-0.2.0/tests/__init__.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.131061 frequenz-repo-config-0.2.0/tests/integration/
--rw-r--r--   0 luca      (1000) luca      (1000)     1208 2023-05-26 09:40:07.000000 frequenz-repo-config-0.2.0/tests/integration/test_cookiecutter_generation.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2023-05-26 09:41:45.131061 frequenz-repo-config-0.2.0/tests/nox/
--rw-r--r--   0 luca      (1000) luca      (1000)      103 2023-05-17 11:36:44.000000 frequenz-repo-config-0.2.0/tests/nox/__init__.py
--rw-r--r--   0 luca      (1000) luca      (1000)      831 2023-05-17 11:36:44.000000 frequenz-repo-config-0.2.0/tests/nox/test_default.py
--rw-r--r--   0 luca      (1000) luca      (1000)      508 2023-05-17 11:36:58.000000 frequenz-repo-config-0.2.0/tests/test_core.py
--rw-r--r--   0 luca      (1000) luca      (1000)      710 2023-05-17 11:36:57.000000 frequenz-repo-config-0.2.0/tests/test_pyproject.py
--rw-r--r--   0 luca      (1000) luca      (1000)      322 2023-05-17 11:36:44.000000 frequenz-repo-config-0.2.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.459284 frequenz-repo-config-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.cookiecutter-replay.json
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.darglint
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.451284 frequenz-repo-config-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.451284 frequenz-repo-config-0.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)     2737 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      512 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2169 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.github/ISSUE_TEMPLATE/feature.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      481 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.github/RELEASE_NOTES.template.md
+-rw-r--r--   0 runner    (1001) docker     (122)      727 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      945 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.github/keylabeler.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      912 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.451284 frequenz-repo-config-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     8141 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.github/workflows/dco-merge-queue.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      932 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      288 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     4344 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3929 2023-07-01 07:04:01.459284 frequenz-repo-config-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2477 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.451284 frequenz-repo-config-0.3.0/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (122)      974 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.451284 frequenz-repo-config-0.3.0/cookiecutter/hooks/
+-rw-r--r--   0 runner    (1001) docker     (122)    15982 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/hooks/post_gen_project.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5762 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/local_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.451284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.451284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.451284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      705 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2169 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/ISSUE_TEMPLATE/feature.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/RELEASE_NOTES.template.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1608 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/keylabeler.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     8243 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/workflows/dco-merge-queue.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      338 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)      381 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     5645 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)      372 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/mkdocstrings_autoapi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3193 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      231 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.443284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.443284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.443284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/frequenz/api/{{cookiecutter.name}}/
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/proto/frequenz/api/{{cookiecutter.name}}/{{cookiecutter.name}}.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     4637 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.447284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.447284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.447284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name}}/
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name}}/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name}}/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1356 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/tests/test_{{cookiecutter.name}}.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/docs/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (122)     8118 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/docs/mkdocstrings_autoapi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2997 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3539 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-01 07:04:01.459284 frequenz-repo-config-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.447284 frequenz-repo-config-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.455284 frequenz-repo-config-0.3.0/src/frequenz/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.447284 frequenz-repo-config-0.3.0/src/frequenz/repo/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.459284 frequenz-repo-config-0.3.0/src/frequenz/repo/config/
+-rw-r--r--   0 runner    (1001) docker     (122)    10857 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5255 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/mkdocs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.459284 frequenz-repo-config-0.3.0/src/frequenz/repo/config/nox/
+-rw-r--r--   0 runner    (1001) docker     (122)     1815 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/nox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8792 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/nox/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3726 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/nox/default.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4996 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/nox/session.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6943 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/nox/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2878 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.459284 frequenz-repo-config-0.3.0/src/frequenz/repo/config/setuptools/
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/setuptools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3516 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/src/frequenz/repo/config/setuptools/grpc_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.459284 frequenz-repo-config-0.3.0/src/frequenz_repo_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3929 2023-07-01 07:04:01.000000 frequenz-repo-config-0.3.0/src/frequenz_repo_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-07-01 07:04:01.000000 frequenz-repo-config-0.3.0/src/frequenz_repo_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-01 07:04:01.000000 frequenz-repo-config-0.3.0/src/frequenz_repo_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-07-01 07:04:01.000000 frequenz-repo-config-0.3.0/src/frequenz_repo_config.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-07-01 07:04:01.000000 frequenz-repo-config-0.3.0/src/frequenz_repo_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-01 07:04:01.000000 frequenz-repo-config-0.3.0/src/frequenz_repo_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.459284 frequenz-repo-config-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.459284 frequenz-repo-config-0.3.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)     2454 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/tests/integration/test_cookiecutter_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-01 07:04:01.459284 frequenz-repo-config-0.3.0/tests/nox/
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/tests/nox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/tests/nox/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)      710 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/tests/test_pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-07-01 07:03:51.000000 frequenz-repo-config-0.3.0/tests/utils.py
```

### Comparing `frequenz-repo-config-0.2.0/.gitignore` & `frequenz-repo-config-0.3.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -110,14 +110,17 @@
 .env
 .venv
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
+# direnv https://github.com/direnv/direnv
+.envrc
+.direnv/
 
 # Spyder project settings
 .spyderproject
 .spyproject
 
 # Rope project settings
 .ropeproject
```

### Comparing `frequenz-repo-config-0.2.0/LICENSE` & `frequenz-repo-config-0.3.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Frequenz Energy-as-a-Service GmbH
+Copyright © 2023 Frequenz Energy-as-a-Service GmbH
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `frequenz-repo-config-0.2.0/README.md` & `frequenz-repo-config-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,64 @@
-# Frequenz repository common configuration for Python
+# Frequenz Repository Configuration
 
-This is very opinionated set of tools and configurations to setup a Python
-repository for Frequenz projects.
+[![Build Status](https://github.com/frequenz-floss/frequenz-repo-config-python/actions/workflows/ci.yaml/badge.svg)](https://github.com/frequenz-floss/frequenz-repo-config-python/actions/workflows/ci.yaml)
+[![PyPI Package](https://img.shields.io/pypi/v/frequenz-repo-config)](https://pypi.org/project/frequenz-repo-config/)
+[![Docs](https://img.shields.io/badge/docs-latest-informational)](https://frequenz-floss.github.io/frequenz-repo-config-python/)
 
-If offers:
+## Introduction
 
-* [Cookiecutter] templates for scaffolding new projects
-* Trivial build of `noxfile.py` with some predefined sessions with all common
-  checks.
-* Tools to build protobuf/grpc files as Python, including type information.
+This is a highly opinionated set of tools and configurations to set up a Python
+repository for [Frequenz](https://frequenz.com) projects.
 
+It offers:
 
-[Cookiecutter]: https://cookiecutter.readthedocs.io/en/stable
+* [Cookiecutter] templates for scaffolding new projects
+* Trivial build of `noxfile.py` with some predefined sessions that include all
+  common checks.
+* Tools to build protobuf/grpc files as Python, including type information.
 
-## Start a new projects
+## Quick Example
 
-To start a new project you should first [install
+To start a new project, you should first [install
 Cookiecutter](https://cookiecutter.readthedocs.io/en/stable/installation.html).
 It is normally available in any Linux distribution, but some have a very old
-version (for example, Ubuntu/Debian).  You can [check which version your distro
-has in Repology](https://repology.org/project/cookiecutter/versions). You need
-**at least version 2.1.0**.  To make sure to get an up to date version you can
-always uses `pip` and install in a `venv`:
+version (for example, Ubuntu/Debian). You can [check which version your distro
+has on Repology](https://repology.org/project/cookiecutter/versions). You need
+**at least version 2.1.0**. To ensure you get an up-to-date version, you can
+always use `pip` and install it in a `venv`:
 
 ```console
 $ python -m venv cookiecutter
 $ cd cookiecutter
 $ . bin/activate
-[cookiecutter] $ pip install cookiecutter
+(venv) $ pip install cookiecutter
 Collecting cookiecutter
 ...
 ```
 
-Then just run cookiecutter where you want to create the new project. A new
+Then simply run [Cookiecutter] where you want to create the new project. A new
 directory will be created with the generated project name. For example:
 
 ```sh
 cd ~/devel
 cookiecutter gh:frequenz-floss/frequenz-repo-config-python --directory=cookiecutter
 ```
 
-This will prompt for the project type, name and other configuration and
-generate the whole project for you.
+This command will prompt you for the project type, name, and other
+configuration options, and it will generate the entire project for you.
+
+After completing the project and fixing the `TODO`s, you can either amend the
+previous commit using `git commit --amend` or create a new commit for the
+changes using `git commit`.
+
+## Documentation
+
+For more detailed documentation, please check the [project's
+website](https://frequenz-floss.github.io/frequenz-repo-config-python/).
+
+## Contributing
+
+If you want to know how to build this project and contribute to it, please
+refer to the [Contributing Guide](CONTRIBUTING.md).
+
+
+[Cookiecutter]: https://cookiecutter.readthedocs.io/en/stable
```

### Comparing `frequenz-repo-config-0.2.0/cookiecutter/hooks/post_gen_project.py` & `frequenz-repo-config-0.3.0/cookiecutter/hooks/post_gen_project.py`

 * *Files 20% similar despite different names*

```diff
@@ -43,53 +43,79 @@
 
     print()
     print("-" * 80)
     print()
     success(f"Your 🍪 {cookiecutter.github_repo_name} has been cut!")
     print()
     print_generated_tree()
-    print("Here is a list of things that should be reviewed and fixed:")
+    print("Here is a list of things that should be reviewed and FIXED:")
     print_todos()
     print()
     print(
         "After completing it you can amend the previous commit using `git commit "
         "--amend` or create a new commit for the changes using `git commit`."
     )
     print()
     print(
         "You can make sure linting and tests pass by creating a virtual "
         "environment, installing the development dependencies and running `nox`:"
     )
     print()
     print(f"cd {cookiecutter.github_repo_name}")
+    print("# Requires at least python version 3.11")
     print("python3 -m venv .venv")
     print(". .venv/bin/activate")
     print("pip install .[dev-noxfile]")
     print("nox")
     print()
+    print("To generate and serve the documentation:")
+    print("pip install .[dev-mkdocs]")
+    if cookiecutter.type == "api":
+        print("# Requires docker")
+    print("mkdocs serve")
+    print()
+    print("To initialize the GitHub pages website:")
+    print("mike deploy --update-aliases next latest")
+    print("mike set-default latest")
+    print("git push upstream gh-pages  # or origin if you haven't forked the repo")
+    print()
+    print("Make sure that GitHub pages is enabled in your repository settings:")
+    print(
+        f"https://github.com/{cookiecutter.github_org}/{cookiecutter.github_repo_name}"
+        "/settings/pages"
+    )
+    print("If all went well, your new website should be available soon at:")
+    print(
+        f"https://{cookiecutter.github_org}.github.io/{cookiecutter.github_repo_name}/"
+    )
+    print()
     if warnings := do_sanity_checks():
         for warning in warnings:
             warn(warning)
         print()
     note(
         "If you had any issues or find any errors in the generated files, "
         "please report them!"
     )
-    note("https://github.com/frequenz-floss/frequenz-repo-config-python/issues/new")
+    note(
+        "https://github.com/frequenz-floss/frequenz-repo-config-python/issues/new/choose"
+    )
     print()
 
 
 def finish_setup() -> None:
     """Finish the setup.
 
     This function is called after the project has been generated and can be used
     to perform any additional setup steps that are required for the project.
     """
     was_repo_initialized = initialize_git_repo()
 
+    copy_replay_file()
+
     remove_unneeded_files()
 
     match cookiecutter.type:
         case "actor":
             finish_actor_setup()
         case "api":
             finish_api_setup()
@@ -100,14 +126,35 @@
         case "model":
             finish_model_setup()
 
     initialize_git_submodules()
     commit_git_changes(first_commit=was_repo_initialized)
 
 
+def copy_replay_file() -> None:
+    """Copy the replay file to the project root."""
+    src = _pathlib.Path("~/.cookiecutter_replay/cookiecutter.json").expanduser()
+    dst = _pathlib.Path(".cookiecutter-replay.json")
+
+    if dst.exists():
+        print(f"Replay file {dst} already exists. Skipping...")
+        return
+
+    if not src.exists():
+        print(f"WARNING: No replay file found in {src}. Skipping...")
+
+    try:
+        _shutil.copyfile(src, dst)
+    except (OSError, IOError) as error:
+        print(
+            f"WARNING: Error copying the replay file {src} -> {dst} ({error}). "
+            "Skipping..."
+        )
+
+
 def initialize_git_submodules() -> bool:
     """Initialize git submodules.
 
     If a `.gitmodules` file exists and it is not empty, it will be used to initialize
     the git submodules using `git submodule update --init --recursive`.
 
     If an empty `.gitmodules` file exists, it will be deleted.
@@ -305,14 +352,20 @@
     cmd = ["grep", "-r", "--color", rf"\<{todo_str}.*", "."]
     try_run(
         cmd,
         warn_on_error=True,
         warn_on_bad_status=f"No `{todo_str}` found using `{' '.join(cmd)}`",
         note_on_failure=f"Please search for `{todo_str}` in `{repo}/` manually.",
     )
+    print()
+    note(
+        "Make sure to (create and) configure your GitHub repository too: "
+        "https://github.com/frequenz-floss/frequenz-repo-config-python/"
+        "wiki/Configuring-a-new-GitHub-repository"
+    )
 
 
 def do_sanity_checks() -> list[str]:
     """Perform sanity checks on the generated project.
 
     Returns:
         List of warnings.
@@ -341,20 +394,17 @@
     This function is called after the project has been generated and can be used
     to perform any additional setup steps that are required for an API.
 
     Operations performed by this function:
 
     * Rename `src` to `py`
     * Rename `tests` to `pytests`
-    * Create `submodules` folder
-    * Create `.gitmodules` file
-    * Initialize submodules
     """
-    _pathlib.Path("src").rename("py")
-    _pathlib.Path("tests").rename("pytests")
+    recursive_overwrite_move(_pathlib.Path("src"), _pathlib.Path("py"))
+    recursive_overwrite_move(_pathlib.Path("tests"), _pathlib.Path("pytests"))
 
 
 def finish_app_setup() -> None:
     """Finish the setup for an app.
 
     This function is called after the project has been generated and can be used
     to perform any additional setup steps that are required for an app.
@@ -370,16 +420,17 @@
     Operations performed by this function:
 
     * Avoid having a subfolder for the type
 
       - `lib`: `src/frequenz/{name}`
       - `rest`: `src/frequenz/{type}/{name}`
     """
-    _pathlib.Path(f"src/frequenz/{cookiecutter.type}/{cookiecutter.name}").rename(
-        f"src/frequenz/{cookiecutter.name}"
+    recursive_overwrite_move(
+        _pathlib.Path(f"src/frequenz/{cookiecutter.type}/{cookiecutter.name}"),
+        _pathlib.Path(f"src/frequenz/{cookiecutter.name}"),
     )
     _pathlib.Path(f"src/frequenz/{cookiecutter.type}").rmdir()
 
 
 def finish_model_setup() -> None:
     """Finish the setup for a model.
 
@@ -431,14 +482,27 @@
             failed = True
     if failed and note_on_failure is not None:
         note(note_on_failure)
 
     return result
 
 
+def recursive_overwrite_move(src: _pathlib.Path, dst: _pathlib.Path) -> None:
+    """Recursively move a directory overwriting the target files if they exist.
+
+    Useful when overwriting an existing project to update it.
+
+    Args:
+        src: The source directory.
+        dst: The target directory.
+    """
+    _shutil.copytree(src, dst, dirs_exist_ok=True)
+    _shutil.rmtree(src)
+
+
 def success(message: str) -> None:
     """Print a success message.
 
     Args:
         message: The message to print.
     """
     print(f"\033[32m{message}\033[0m")
```

### Comparing `frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/.gitignore` & `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -110,14 +110,17 @@
 .env
 .venv
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
+# direnv https://github.com/direnv/direnv
+.envrc
+.direnv/
 
 # Spyder project settings
 .spyderproject
 .spyproject
 
 # Rope project settings
 .ropeproject
```

### Comparing `frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/LICENSE` & `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Frequenz Energy-as-a-Service GmbH
+Copyright © {% now 'utc', '%Y' %} {{cookiecutter.author_name}}
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/pyproject.toml` & `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # License: MIT
-# Copyright © {% now 'utc', '%Y' %} Frequenz Energy-as-a-Service GmbH
+# Copyright © {% now 'utc', '%Y' %} {{cookiecutter.author_name}}
 
 [build-system]
 requires = [
   "setuptools == 67.7.2",
   "setuptools_scm[toml] == 7.1.0",
   "frequenz-repo-config[{{cookiecutter.type}}] == 0.2.0",
 ]
@@ -56,40 +56,48 @@
 [project.optional-dependencies] # TODO(cookiecutter): Remove and add more if appropriate
 dev-docstrings = [
   "pydocstyle == 6.3.0",
   "darglint == 1.8.1",
   "tomli == 2.0.1",      # Needed by pydocstyle to read pyproject.toml
 ]
 dev-formatting = ["black == 23.3.0", "isort == 5.12.0"]
+dev-mkdocs = [
+  "mike == 1.1.2",
+  "mkdocs-gen-files == 0.5.0",
+  "mkdocs-literate-nav == 0.6.0",
+  "mkdocs-material == 9.1.16",
+  "mkdocs-section-index == 0.3.5",
+  "mkdocstrings[python] == 0.22.0",
+]
 dev-mypy = [
   "mypy == 1.2.0",
   # For checking the noxfile, docs/ script, and tests
-  "{{cookiecutter.pypi_package_name}}[dev-noxfile,dev-pytest]",
+  "{{cookiecutter.pypi_package_name}}[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
 dev-noxfile = [
   "nox == 2023.4.22",
   "frequenz-repo-config[{{cookiecutter.type}}] == 0.2.0",
 ]
 dev-pylint = [
   "pylint == 2.17.3",
   # For checking the noxfile, docs/ script, and tests
-  "{{cookiecutter.pypi_package_name}}[dev-noxfile,dev-pytest]",
+  "{{cookiecutter.pypi_package_name}}[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
 {%- if cookiecutter.type == "api" %}
 dev-pytest = ["pytest == 7.3.1"]
 {%- else %}
 dev-pytest = [
   "pytest == 7.3.1",
   "pytest-mock == 3.10.0",
   "pytest-asyncio == 0.21.0",
   "async-solipsism == 0.5",
 ]
 {%- endif %}
 dev = [
-  "{{cookiecutter.pypi_package_name}}[dev-docstrings,dev-formatting,dev-gen-docs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]",
+  "{{cookiecutter.pypi_package_name}}[dev-mkdocs,dev-docstrings,dev-formatting,dev-gen-docs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]",
 ]
 
 [project.urls]
 Changelog = "https://github.com/{{cookiecutter.github_org}}/{{cookiecutter.github_repo_name}}/releases"
 Issues = "https://github.com/{{cookiecutter.github_org}}/{{cookiecutter.github_repo_name}}/issues"
 Repository = "https://github.com/{{cookiecutter.github_org}}/{{cookiecutter.github_repo_name}}"
 Support = "https://github.com/{{cookiecutter.github_org}}/{{cookiecutter.github_repo_name}}/discussions/categories/support"
@@ -100,14 +108,15 @@
 {%- if cookiecutter.type != "api" %}
 include = '\.pyi?$'
 {%- endif %}
 
 [tool.isort]
 profile = "black"
 line_length = 88
+{#- We don't include "py" here for API because we don't want to check generated files #}
 src_paths = ["src", "examples", "tests"]
 
 [tool.pylint.similarities]
 ignore-comments = ['yes']
 ignore-docstrings = ['yes']
 ignore-imports = ['no']
 min-similarity-lines = 40
```

### Comparing `frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name}}/__init__.py` & `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/src/frequenz/{{cookiecutter.type}}/{{cookiecutter.name}}/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # License: MIT
-# Copyright © {% now 'utc', '%Y' %} Frequenz Energy-as-a-Service GmbH
+# Copyright © {% now 'utc', '%Y' %} {{cookiecutter.author_name}}
 
 """{{cookiecutter.description}}.
 
 TODO(cookiecutter): Add a more descriptive module description.
 """
 {%- if cookiecutter.type != "api" %}
```

### Comparing `frequenz-repo-config-0.2.0/cookiecutter/{{cookiecutter.github_repo_name}}/tests/test_{{cookiecutter.name}}.py` & `frequenz-repo-config-0.3.0/cookiecutter/{{cookiecutter.github_repo_name}}/tests/test_{{cookiecutter.name}}.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # License: MIT
-# Copyright © {% now 'utc', '%Y' %} Frequenz Energy-as-a-Service GmbH
+# Copyright © {% now 'utc', '%Y' %} {{cookiecutter.author_name}}
 
 """Tests for the {{cookiecutter.name}} package."""
 
 {%- if cookiecutter.type == "api" %}
 
 
 def test_package_import() -> None:
```

### Comparing `frequenz-repo-config-0.2.0/pyproject.toml` & `frequenz-repo-config-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,46 @@
+# License: MIT
+# Copyright © 2023 Frequenz Energy-as-a-Service GmbH
+
 [build-system]
-requires = ["setuptools == 67.6.0", "setuptools_scm[toml] == 7.1.0"]
+requires = ["setuptools == 67.7.2", "setuptools_scm[toml] == 7.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frequenz-repo-config"
 description = "Frequenz repository setup tools and common configuration"
 readme = "README.md"
 license = { text = "MIT" }
 keywords = [
+  "config",
   "frequenz",
-  "package",
+  "grpc",
+  "lib",
+  "library",
+  "mkdocs",
+  "nox",
   "project",
-  "config",
-  "tool",
+  "protobuf",
+  "python",
+  "repo-config",
   "repository",
   "setuptools",
-  "nox",
-  "grpc",
-  "protobuf",
+  "tool",
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.11",
   "Topic :: Software Development :: Libraries",
+  "Typing :: Typed",
 ]
 requires-python = ">= 3.11, < 4"
-dependencies = ["nox >= 2022.11.21"]
+dependencies = ["nox >= 2022.11.21", "mkdocs-gen-files >= 0.4.0, < 0.6.0"]
 dynamic = ["version"]
 
 [[project.authors]]
 name = "Frequenz Energy-as-a-Service GmbH"
 email = "floss@frequenz.com"
 
 [project.entry-points."distutils.commands"]
@@ -45,76 +52,82 @@
   "grpcio-tools >= 1.47.0, < 2",
   "mypy-protobuf >= 3.0.0, < 4",
   "setuptools >= 67.6.0, < 68",
 ]
 app = []
 lib = []
 model = []
-dev-docs-gen = [
+dev-docstrings = [
+  "pydocstyle == 6.3.0",
+  "darglint == 1.8.1",
+  "tomli == 2.0.1",      # Needed by pydocstyle to read pyproject.toml
+]
+dev-formatting = ["black == 23.3.0", "isort == 5.12.0"]
+dev-mkdocs = [
   "mike == 1.1.2",
-  "mkdocs-gen-files == 0.4.0",
-  "mkdocs-literate-nav == 0.4.0",
-  "mkdocs-material == 9.1.4",
+  "mkdocs-gen-files == 0.5.0",
+  "mkdocs-literate-nav == 0.6.0",
+  "mkdocs-material == 9.1.16",
   "mkdocs-section-index == 0.3.5",
-  "mkdocstrings[python] == 0.20.0",
+  "mkdocstrings[python] == 0.22.0",
 ]
-dev-docstrings = ["pydocstyle == 6.3.0", "darglint == 1.8.1"]
-dev-formatting = ["black == 23.3.0", "isort == 5.12.0"]
 dev-mypy = [
-  "mypy == 1.1.1",
+  "mypy == 1.2.0",
   "types-setuptools >= 67.6.0, < 68", # Should match the global dependency
-  # For checking the docs/ script, and tests
-  "frequenz-repo-config[dev-docs-gen,dev-pytest]",
+  # For checking the noxfile, docs/ script, and tests
+  "frequenz-repo-config[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
+dev-noxfile = ["nox == 2023.4.22"]
 dev-pylint = [
-  "pylint == 2.17.1",
-  "pylint-google-style-guide-imports-enforcing == 1.3.0",
-  # For checking the docs/ script, and tests
-  "frequenz-repo-config[dev-docs-gen,dev-pytest]",
+  "pylint == 2.17.3",
+  # For checking the noxfile, docs/ script, and tests
+  "frequenz-repo-config[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
 dev-pytest = [
-  "pytest == 7.2.2",
+  "pytest == 7.3.1",
   "cookiecutter == 2.1.1", # For checking the cookiecutter scripts
 ]
 dev = [
-  "frequenz-repo-config[dev-docs-gen,dev-docstrings,dev-formatting,dev-pytest,dev-mypy,dev-pylint]",
+  "frequenz-repo-config[dev-mkdocs,dev-docstrings,dev-formatting,dev-gen-docs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]",
 ]
 
 [project.urls]
 Changelog = "https://github.com/frequenz-floss/frequenz-repo-config-python/releases"
-Repository = "https://github.com/frequenz-floss/frequenz-repo-config-python"
 Issues = "https://github.com/frequenz-floss/frequenz-repo-config-python/issues"
+Repository = "https://github.com/frequenz-floss/frequenz-repo-config-python"
 Support = "https://github.com/frequenz-floss/frequenz-repo-config-python/discussions/categories/support"
 
-[tool.setuptools]
-include-package-data = true
-
-[tool.setuptools_scm]
-version_scheme = "post-release"
-
 [tool.black]
 line-length = 88
 target-version = ['py311']
 include = '\.pyi?$'
 
+[tool.isort]
+profile = "black"
+line_length = 88
+src_paths = ["src", "examples", "tests"]
+
+[tool.pylint.similarities]
+ignore-comments = ['yes']
+ignore-docstrings = ['yes']
+ignore-imports = ['no']
+min-similarity-lines = 40
+
 [tool.pylint.messages_control]
 disable = [
   "too-few-public-methods",
   # disabled because it conflicts with isort
   "wrong-import-order",
   "ungrouped-imports",
 ]
 
-[tool.isort]
-profile = "black"
-line_length = 88
-src_paths = ["src"]
-
 [[tool.mypy.overrides]]
 module = ["cookiecutter", "cookiecutter.*"]
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 markers = [
   "integration: integration tests (deselect with '-m \"not integration\"')",
 ]
+[tool.setuptools_scm]
+version_scheme = "post-release"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `frequenz-repo-config-0.2.0/src/frequenz/repo/config/__init__.py` & `frequenz-repo-config-0.3.0/src/frequenz/repo/config/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 # License: MIT
 # Copyright © 2023 Frequenz Energy-as-a-Service GmbH
 
 r"""Frequenz project setup tools and common configuration.
 
 The tools are provided to configure the main types of repositories most commonly used at
 Frequenz, defined in
-[`freq.repo.config.RepositoryType`][freq.repo.config.RepositoryType].
+[`frequenz.repo.config.RepositoryType`][].
 
 - actor: SDK actors
 - api: gRPC APIs
 - app: SDK applications
 - lib: General purpose Python libraries
 - model: SDK machine learning models
 
 # Common
 
-## `nox`
+## `nox` (running tests and linters)
 
 ### Writing the `noxfile.py`
 
 Projects wanting to use `nox` to run lint checkers and other utilities can use
 the [`frequenz.repo.config.nox`][] package.
 
 When writing the `noxfile.py` you should import the `nox` module from this
 package and use the [`frequenz.repo.config.nox.configure`][] function,
 which will configure all nox sessions.
 
-You should call `configure()` using one of the default configurations provided
-in the [`frequenz.repo.config.nox.default`][] module. For example:
+To use the default options, you should call `configure()` using one of the [repository
+types][frequenz.repo.config.RepositoryType].  For example:
 
 ```python
-from frequenz.repo.config import nox
+from frequenz.repo.config import RepositoryType, nox
 
-nox.configure(nox.default.lib_config)
+nox.configure(RepositoryType.LIB)
 ```
 
-Again, make sure to pick the correct default configuration based on the type of your
+Again, make sure to pick the correct project typedefault configuration based on the type of your
 project (`actor_config`, `api_config`, `app_config`, `lib_config`, `model_config`).
 
-If you need to modify the configuration, you can copy one of the default
-configurations by using the
-[`copy()`][frequenz.repo.config.nox.config.Config.copy] method:
+If you need to use some custom configuration, you can start from the default settings in
+the [`frequenz.repo.config.nox.default`][] module,
+[copying][frequenz.repo.config.nox.config.Config.copy] it and changing whatever you
+need to customize.  For example:
 
 ```python
 from frequenz.repo.config import nox
+from frequenz.repo.config.nox import default
 
-config = nox.default.lib_config.copy()
+config = default.lib_config.copy()
 config.opts.black.append("--diff")
 nox.configure(config)
 ```
 
 If you need further customization or to define new sessions, you can use the
 following modules:
 
@@ -126,51 +128,145 @@
 [project]
 name = "my-package"
 # ...
 
 [project.optional-dependencies]
 dev-docstrings = ["pydocstyle == 6.3.0", "darglint == 1.8.1"]
 dev-formatting = ["black == 23.3.0", "isort == 5.12.0"]
+dev-mkdocs = [
+  "mike == 1.1.2",
+  "mkdocs-gen-files == 0.5.0",
+  "mkdocs-literate-nav == 0.6.0",
+  "mkdocs-material == 9.1.16",
+  "mkdocs-section-index == 0.3.5",
+  "mkdocstrings[python] == 0.22.0",
+]
 dev-mypy = [
   "mypy == 1.1.1",
   # For checking tests
-  "my-package[dev-pytest]",
+  "my-package[dev-mkdocs,dev-pytest]",
 ]
 dev-pylint = [
   "pylint == 2.17.1",
   "pylint-google-style-guide-imports-enforcing == 1.3.0",
   # For checking tests
-  "my-package[dev-pytest]",
+  "my-package[dev-mkdocs,dev-pytest]",
 ]
 dev-pytest = [
   "pytest == 7.2.2",
   "pytest-asyncio == 0.21.0",
   "pytest-mock == 3.10.0",
 ]
 dev = [
-  "my-package[dev-docstrings,dev-formatting,dev-mypy,dev-nox,dev-pylint,dev-pytest]",
+  "my-package[dev-mkdocs,dev-docstrings,dev-formatting,dev-mypy,dev-nox,dev-pylint,dev-pytest]",
 ]
 ```
 
+## `mkdocs` (generating documentation)
+
+### API reference generation
+
+The API documnentation can be automatically generated from the source files using the
+[`frequenz.repo.config.mkdocs`][] package as when run as a
+[`mkdocs-gen-files`](https://oprypin.github.io/mkdocs-gen-files/) plugin script.
+
+To enable it you just need to make sure the `mkdocs-gen-files`, `mkdocs-literate-nav`
+and `mkdocstrings[python]` packages are installed (look at the `pyproject.toml`
+configuration in the `nox` section) and add the following configuration to the
+`mkdocs.yml` file:
+
+```yaml
+plugins:
+  - gen-files:
+      scripts:
+        - path/to/my/custom/script.py
+```
+
+By default this script will look for files in the `src/` directory and generate the
+documentation files in the `python-reference/` directory inside `mkdocs` output directory
+(`site` by defaul).
+
+If you need to customize the above paths, you can create a new script to use with the
+`mkdocs-gen-files` plugin as follows:
+
+```python
+from frequenz.repo.config import mkdocs
+
+mkdocs.generate_python_api_pages("my_sources", "API")
+```
+
+Where `my_sources` is the directory containing the source files and `API` is the
+directory where to generate the documentation files (relative to `mkdocs` output
+directory).
+
+And then replace this configuration in the `mkdocs.yml` file:
+
+```yaml
+plugins:
+  - gen-files:
+      scripts:
+        - path/to/my/custom/script.py
+```
+
 # APIs
 
-## `setuptools` gRPC support
+## Protobuf configuation
+
+Support is provided to generate files from *protobuf* files.  To do this, it is possible
+to configure the options to use while generating the files for different purposes
+(language bindings, documentation, etc.).
+
+The configuration can be done in the `pyproject.toml` file as follows:
+
+```toml
+[tool.frequenz_repo_config.protobuf]
+# Location of the proto files relative to the root of the repository (default: "proto")
+proto_path = "proto_files"
+# Glob pattern to use to find the proto files in the proto_path (default: "*.proto")
+proto_glob = "*.prt"  # Default: "*.proto"
+# List of paths to pass to the protoc compiler as include paths (default:
+# ["submodules/api-common-protos", "submodules/frequenz-api-common/proto"])
+include_paths = ["submodules/api-common-protos"]
+# Path where to generate the Python files (default: "py")
+py_path = "generated"
+# Path where to generate the documentation files (default: "protobuf-reference")
+docs_path = "API"
+```
+
+If the defaults are not suitable for you (for example you need to use more or less
+submodules or your proto files are located somewhere else), please adjust the
+configuration to match your project structure.
+
+### `mkdocs` API reference generation
+
+If your project provides *protobuf* files, you can also generate the API
+documentation for them adding one more line to the script provided in the common
+section:
+
+```python
+from frequenz.repo.config import mkdocs
+
+mkdocs.generate_python_api_pages("my_sources", "API-py")
+mkdocs.generate_protobuf_api_pages()
+```
+
+This will use the configuration in the `pyproject.toml` file and requires `docker` to
+run (it uses the `pseudomuto/protoc-gen-doc` docker image.
+
+### `setuptools` gRPC support
 
 When configuring APIs it is assumed that they have a gRPC interface.
 
-The project structure is assumed to be as follows:
+The project structure is assumed to be as described in the *Protobuf configuration*
+section plus the following:
 
-- `proto/`: Directory containing the `.proto` files.
-- `py/`: Directory containing the Python code. It should only provide
-  a `py.typed` file and a `__init__.py` file. API repositories should not
-  contain any other Python code.
 - `pytests/`: Directory containing the tests for the Python code.
-- `submodules/api-common-protos`: Directory containing the submodule with the
+- `submodules/api-common-protos`: Directory containing the Git submodule with the
   `google/api-common-protos` repository.
-- `submodules/frequenz-api-common`: Directory containing the submodule with the
+- `submodules/frequenz-api-common`: Directory containing the Git submodule with the
   `frequenz-floss/frequenz-api-common` repository.
 
 Normally Frequenz APIs use basic types from
 [`google/api-common-protos`](https://github.com/googleapis/api-common-protos) and
 [`frequenz-floss/frequenz-api-common`](https://github.com/frequenz-floss/frequenz-api-common),
 so you need to make sure the proper submodules are added to your project:
 
@@ -228,37 +324,16 @@
 Make sure to include these lines in the `MANIFEST.in` file:
 
 ```
 recursive-include submodules/api-common-protos/google *.proto
 recursive-include submodules/frequenz-api-common/proto *.proto
 ```
 
-If the defaults are not suitable for you (for example you need to use more or less
-submodules or your proto files are located somewhere else, you can customize how
-the protocol files are generated by adding the following section to your
-`pyproject.toml` file:
-
-```toml
-[tool.frequenz_repo_config.setuptools.grpc_tools]
-# Location of the proto files relative to the root of the repository (default: "proto")
-proto_path = "proto_files"
-# Glob pattern to use to find the proto files in the proto_path (default: "*.proto")
-proto_glob = "*.prt"  # Default: "*.proto"
-# List of paths to pass to the protoc compiler as include paths (default:
-# ["submodules/api-common-protos", "submodules/frequenz-api-common/proto"])
-include_paths = ["submodules/api-common-protos"]
-# Path where to generate the Python files (default: "py")
-py_path = "generated"
-```
-
 Please adapt the instructions above to your project structure if you need to change the
 defaults.
 """
 
-from . import nox, setuptools
 from ._core import RepositoryType
 
 __all__ = [
     "RepositoryType",
-    "nox",
-    "setuptools",
 ]
```

### Comparing `frequenz-repo-config-0.2.0/src/frequenz/repo/config/nox/config.py` & `frequenz-repo-config-0.3.0/src/frequenz/repo/config/nox/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 so it can be used when implementing custom nox sessions.
 
 The `configure()` function must be called before `get()` is used.
 """
 
 import dataclasses as _dataclasses
 import itertools as _itertools
-from typing import Self
+from typing import Self, assert_never, overload
 
 import nox as _nox
 
+from .._core import RepositoryType
 from . import util as _util
 
 
 @_dataclasses.dataclass(kw_only=True, slots=True)
 class CommandsOptions:
     """Command-line options for each command."""
 
@@ -173,16 +174,77 @@
     Returns:
         The global configuration object.
     """
     assert _config is not None, "You must call configure() before using this function"
     return _config
 
 
-def configure(conf: Config, /) -> None:
+@overload
+def configure(conf: Config, /, *, import_default_sessions: bool = True) -> None:
     """Configure nox using the provided configuration.
 
     Args:
         conf: The configuration to use to configure nox.
+        import_default_sessions: Whether to import the default sessions or not.
+            This is only necessary if you want to avoid using the default provided
+            sessions and use your own.
+    """
+
+
+@overload
+def configure(
+    repo_type: RepositoryType, /, *, import_default_sessions: bool = True
+) -> None:
+    """Configure nox using the provided repository type.
+
+    Args:
+        repo_type: The repository type to use to configure nox.  This will use the
+            default configuration in [`frequenz.repo.config.nox.default`][] for that
+            type of repository.
+        import_default_sessions: Whether to import the default sessions or not.
+            This is only necessary if you want to avoid using the default provided
+            sessions and use your own.
+    """
+
+
+def configure(
+    conf: Config | RepositoryType, /, *, import_default_sessions: bool = True
+) -> None:
+    """Configure nox using the provided configuration or repository type.
+
+    Args:
+        conf: The configuration to use to configure nox, or the repository type to use
+            to configure nox.  The later will use the default configuration in
+            [`frequenz.repo.config.nox.default`][] for that type of repository.
+        import_default_sessions: Whether to import the default sessions or not.
+            This is only necessary if you want to avoid using the default provided
+            sessions and use your own.
     """
     global _config  # pylint: disable=global-statement
-    _config = conf
+
+    # We need to make sure sessions are imported, otherwise they won't be visible to nox.
+    if import_default_sessions:
+        # pylint: disable=import-outside-toplevel,cyclic-import
+        from . import session as _
+
+    match conf:
+        case Config():
+            _config = conf
+        case RepositoryType() as repo_type:
+            # pylint: disable=import-outside-toplevel,cyclic-import
+            from . import default
+
+            match repo_type:
+                case RepositoryType.ACTOR:
+                    _config = default.actor_config
+                case RepositoryType.API:
+                    _config = default.api_config
+                case RepositoryType.APP:
+                    _config = default.app_config
+                case RepositoryType.LIB:
+                    _config = default.lib_config
+                case RepositoryType.MODEL:
+                    _config = default.model_config
+                case _ as unhandled:
+                    assert_never(unhandled)
+
     _nox.options.sessions = _config.sessions
```

### Comparing `frequenz-repo-config-0.2.0/src/frequenz/repo/config/nox/default.py` & `frequenz-repo-config-0.3.0/src/frequenz/repo/config/nox/default.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     black=[
         "--check",
     ],
     darglint=[
         "-v2",  # for verbose error messages.
     ],
     isort=[
+        "--diff",
         "--check",
     ],
     mypy=[
         "--install-types",
         "--namespace-packages",
         "--non-interactive",
         "--explicit-package-bases",
```

### Comparing `frequenz-repo-config-0.2.0/src/frequenz/repo/config/nox/session.py` & `frequenz-repo-config-0.3.0/src/frequenz/repo/config/nox/session.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.2.0/src/frequenz/repo/config/nox/util.py` & `frequenz-repo-config-0.3.0/src/frequenz/repo/config/nox/util.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.2.0/src/frequenz_repo_config.egg-info/requires.txt` & `frequenz-repo-config-0.3.0/src/frequenz_repo_config.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 nox>=2022.11.21
+mkdocs-gen-files<0.6.0,>=0.4.0
 
 [actor]
 
 [api]
 grpcio-tools<2,>=1.47.0
 mypy-protobuf<4,>=3.0.0
 setuptools<68,>=67.6.0
 
 [app]
 
 [dev]
-frequenz-repo-config[dev-docs-gen,dev-docstrings,dev-formatting,dev-mypy,dev-pylint,dev-pytest]
-
-[dev-docs-gen]
-mike==1.1.2
-mkdocs-gen-files==0.4.0
-mkdocs-literate-nav==0.4.0
-mkdocs-material==9.1.4
-mkdocs-section-index==0.3.5
-mkdocstrings[python]==0.20.0
+frequenz-repo-config[dev-docstrings,dev-formatting,dev-gen-docs,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]
 
 [dev-docstrings]
 pydocstyle==6.3.0
 darglint==1.8.1
+tomli==2.0.1
 
 [dev-formatting]
 black==23.3.0
 isort==5.12.0
 
+[dev-mkdocs]
+mike==1.1.2
+mkdocs-gen-files==0.5.0
+mkdocs-literate-nav==0.6.0
+mkdocs-material==9.1.16
+mkdocs-section-index==0.3.5
+mkdocstrings[python]==0.22.0
+
 [dev-mypy]
-mypy==1.1.1
+mypy==1.2.0
 types-setuptools<68,>=67.6.0
-frequenz-repo-config[dev-docs-gen,dev-pytest]
+frequenz-repo-config[dev-mkdocs,dev-noxfile,dev-pytest]
+
+[dev-noxfile]
+nox==2023.4.22
 
 [dev-pylint]
-pylint==2.17.1
-pylint-google-style-guide-imports-enforcing==1.3.0
-frequenz-repo-config[dev-docs-gen,dev-pytest]
+pylint==2.17.3
+frequenz-repo-config[dev-mkdocs,dev-noxfile,dev-pytest]
 
 [dev-pytest]
-pytest==7.2.2
+pytest==7.3.1
 cookiecutter==2.1.1
 
 [lib]
 
 [model]
```

### Comparing `frequenz-repo-config-0.2.0/tests/nox/test_default.py` & `frequenz-repo-config-0.3.0/tests/nox/test_default.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.2.0/tests/test_pyproject.py` & `frequenz-repo-config-0.3.0/tests/test_pyproject.py`

 * *Files identical despite different names*

