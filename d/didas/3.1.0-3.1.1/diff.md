# Comparing `tmp/didas-3.1.0.tar.gz` & `tmp/didas-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/didas/didas/dist/.tmp-r058pheb/didas-3.1.0.tar", last modified: Fri Jun  2 11:32:51 2023, max compression
+gzip compressed data, was "/home/runner/work/didas/didas/dist/.tmp-5rshabku/didas-3.1.1.tar", last modified: Sat Jul  1 06:09:50 2023, max compression
```

## Comparing `didas-3.1.0.tar` & `didas-3.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:32:51.000000 didas-3.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:32:51.000000 didas-3.1.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-02 11:32:37.000000 didas-3.1.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:32:51.000000 didas-3.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:32:51.000000 didas-3.1.0/.github/linters/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-02 11:32:37.000000 didas-3.1.0/.github/linters/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-02 11:32:37.000000 didas-3.1.0/.github/linters/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-02 11:32:37.000000 didas-3.1.0/.github/linters/.python-black
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:32:51.000000 didas-3.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-02 11:32:37.000000 didas-3.1.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-02 11:32:37.000000 didas-3.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-02 11:32:51.000000 didas-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-02 11:32:37.000000 didas-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:32:51.000000 didas-3.1.0/didas/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-02 11:32:37.000000 didas-3.1.0/didas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 11:32:50.000000 didas-3.1.0/didas/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-02 11:32:37.000000 didas-3.1.0/didas/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-06-02 11:32:37.000000 didas-3.1.0/didas/oracle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:32:51.000000 didas-3.1.0/didas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-02 11:32:50.000000 didas-3.1.0/didas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-02 11:32:51.000000 didas-3.1.0/didas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:32:50.000000 didas-3.1.0/didas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-02 11:32:50.000000 didas-3.1.0/didas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 11:32:50.000000 didas-3.1.0/didas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-02 11:32:37.000000 didas-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-02 11:32:37.000000 didas-3.1.0/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 11:32:51.000000 didas-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:09:50.000000 didas-3.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:09:50.000000 didas-3.1.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-01 06:09:36.000000 didas-3.1.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:09:50.000000 didas-3.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:09:50.000000 didas-3.1.1/.github/linters/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-01 06:09:36.000000 didas-3.1.1/.github/linters/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-01 06:09:36.000000 didas-3.1.1/.github/linters/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-01 06:09:36.000000 didas-3.1.1/.github/linters/.python-black
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:09:50.000000 didas-3.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-01 06:09:36.000000 didas-3.1.1/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-01 06:09:36.000000 didas-3.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-01 06:09:50.000000 didas-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-01 06:09:36.000000 didas-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:09:50.000000 didas-3.1.1/didas/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-01 06:09:36.000000 didas-3.1.1/didas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-01 06:09:50.000000 didas-3.1.1/didas/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-01 06:09:36.000000 didas-3.1.1/didas/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-07-01 06:09:36.000000 didas-3.1.1/didas/oracle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:09:50.000000 didas-3.1.1/didas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-01 06:09:50.000000 didas-3.1.1/didas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-01 06:09:50.000000 didas-3.1.1/didas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 06:09:50.000000 didas-3.1.1/didas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-01 06:09:50.000000 didas-3.1.1/didas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 06:09:50.000000 didas-3.1.1/didas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-01 06:09:36.000000 didas-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 06:09:36.000000 didas-3.1.1/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 06:09:50.000000 didas-3.1.1/setup.cfg
```

### Comparing `didas-3.1.0/.devcontainer/devcontainer.json` & `didas-3.1.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `didas-3.1.0/.github/workflows/pypi.yml` & `didas-3.1.1/.github/workflows/pypi.yml`

 * *Files 8% similar despite different names*

```diff
@@ -41,12 +41,16 @@
         run: >-
           python -m
           build
           --sdist
           --wheel
           --outdir dist/
           .
+      - uses: softprops/action-gh-release@v1
+        if: github.event_name == 'release'
+        with:
+          files: dist/*
       - name: Publish distribution 📦 to PyPI
         if: github.event_name == 'release'
         uses: pypa/gh-action-pypi-publish@master
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `didas-3.1.0/.gitignore` & `didas-3.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `didas-3.1.0/PKG-INFO` & `didas-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: didas
-Version: 3.1.0
+Version: 3.1.1
 Summary: Python Commons for Didas
 Author-email: Georg Wendorf <georgfriedrich.wendorf@freenet.ag>
 Maintainer-email: Georg Wendorf <georgfriedrich.wendorf@freenet.ag>
 Project-URL: Homepage, https://github.com/freenet-group/didas
 Project-URL: Documentation, https://github.com/freenet-group/didas/blob/main/README.md
 Project-URL: Repository, https://github.com/freenet-group/didas
 Project-URL: Changelog, https://github.com/freenet-group/didas/releases
```

### Comparing `didas-3.1.0/didas/mlflow.py` & `didas-3.1.1/didas/mlflow.py`

 * *Files identical despite different names*

### Comparing `didas-3.1.0/didas/oracle.py` & `didas-3.1.1/didas/oracle.py`

 * *Files identical despite different names*

### Comparing `didas-3.1.0/didas.egg-info/PKG-INFO` & `didas-3.1.1/didas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: didas
-Version: 3.1.0
+Version: 3.1.1
 Summary: Python Commons for Didas
 Author-email: Georg Wendorf <georgfriedrich.wendorf@freenet.ag>
 Maintainer-email: Georg Wendorf <georgfriedrich.wendorf@freenet.ag>
 Project-URL: Homepage, https://github.com/freenet-group/didas
 Project-URL: Documentation, https://github.com/freenet-group/didas/blob/main/README.md
 Project-URL: Repository, https://github.com/freenet-group/didas
 Project-URL: Changelog, https://github.com/freenet-group/didas/releases
```

### Comparing `didas-3.1.0/pyproject.toml` & `didas-3.1.1/pyproject.toml`

 * *Files identical despite different names*

