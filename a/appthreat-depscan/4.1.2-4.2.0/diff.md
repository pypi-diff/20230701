# Comparing `tmp/appthreat-depscan-4.1.2.tar.gz` & `tmp/appthreat-depscan-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appthreat-depscan-4.1.2.tar", last modified: Mon May  1 19:05:58 2023, max compression
+gzip compressed data, was "appthreat-depscan-4.2.0.tar", last modified: Fri Jun 30 23:12:31 2023, max compression
```

## Comparing `appthreat-depscan-4.1.2.tar` & `appthreat-depscan-4.2.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:05:58.645895 appthreat-depscan-4.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-05-01 19:05:58.641895 appthreat-depscan-4.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21215 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:05:58.637894 appthreat-depscan-4.1.2/appthreat_depscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-05-01 19:05:58.000000 appthreat-depscan-4.1.2/appthreat_depscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-01 19:05:58.000000 appthreat-depscan-4.1.2/appthreat_depscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:05:58.000000 appthreat-depscan-4.1.2/appthreat_depscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-01 19:05:58.000000 appthreat-depscan-4.1.2/appthreat_depscan.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-01 19:05:58.000000 appthreat-depscan-4.1.2/appthreat_depscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 19:05:58.000000 appthreat-depscan-4.1.2/appthreat_depscan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:05:58.637894 appthreat-depscan-4.1.2/depscan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/depscan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25919 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/depscan/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:05:58.637894 appthreat-depscan-4.1.2/depscan/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/depscan/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30587 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/depscan/lib/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/depscan/lib/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/depscan/lib/bom.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/depscan/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/depscan/lib/license.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/depscan/lib/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/depscan/lib/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18022 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/depscan/lib/pkg_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/depscan/lib/privado.py
--rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/depscan/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 19:05:58.645895 appthreat-depscan-4.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:05:58.637894 appthreat-depscan-4.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/test/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/test/test_bom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/test/test_license.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/test/test_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/test/test_pkg_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/test/test_privado.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/test/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:05:58.637894 appthreat-depscan-4.1.2/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:05:58.633895 appthreat-depscan-4.1.2/vendor/choosealicense.com/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:05:58.637894 appthreat-depscan-4.1.2/vendor/choosealicense.com/_data/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_data/fields.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_data/meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_data/rules.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:05:58.641895 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/0bsd.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/afl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35944 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/agpl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/artistic-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/bsd-2-clause.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/bsd-3-clause.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/bsd-4-clause.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/bsl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19759 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/cc-by-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    21474 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/cc0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23872 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/cecill-2.1.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/ecl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/epl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/epl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14163 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/eupl-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14871 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/eupl-1.2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23969 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/gfdl-1.3.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/gpl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    36394 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/gpl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/isc.txt
--rw-r--r--   0 runner    (1001) docker     (123)    27491 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/lgpl-2.1.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/lgpl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19902 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/lppl-1.3c.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/mit-0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/mit.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18103 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/mpl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/ms-pl.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/ms-rl.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/ncsa.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26174 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/odbl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/ofl-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/osl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/postgresql.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/upl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/vim.txt
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/wtfpl.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/zlib.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:05:58.633895 appthreat-depscan-4.1.2/vendor/spdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:05:58.641895 appthreat-depscan-4.1.2/vendor/spdx/json/
--rw-r--r--   0 runner    (1001) docker     (123)   224002 2023-05-01 19:05:42.000000 appthreat-depscan-4.1.2/vendor/spdx/json/licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:12:31.933931 appthreat-depscan-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    22457 2023-06-30 23:12:31.929931 appthreat-depscan-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21535 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:12:31.921930 appthreat-depscan-4.2.0/appthreat_depscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22457 2023-06-30 23:12:31.000000 appthreat-depscan-4.2.0/appthreat_depscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-30 23:12:31.000000 appthreat-depscan-4.2.0/appthreat_depscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 23:12:31.000000 appthreat-depscan-4.2.0/appthreat_depscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 23:12:31.000000 appthreat-depscan-4.2.0/appthreat_depscan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-30 23:12:31.000000 appthreat-depscan-4.2.0/appthreat_depscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-30 23:12:31.000000 appthreat-depscan-4.2.0/appthreat_depscan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:12:31.921930 appthreat-depscan-4.2.0/depscan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/depscan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25423 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/depscan/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:12:31.921930 appthreat-depscan-4.2.0/depscan/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/depscan/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34715 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/depscan/lib/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/depscan/lib/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13131 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/depscan/lib/bom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/depscan/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/depscan/lib/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/depscan/lib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/depscan/lib/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/depscan/lib/pkg_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/depscan/lib/privado.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/depscan/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 23:12:31.933931 appthreat-depscan-4.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:12:31.921930 appthreat-depscan-4.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    29112 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/test/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/test/test_bom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/test/test_license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/test/test_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/test/test_pkg_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/test/test_privado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:12:31.921930 appthreat-depscan-4.2.0/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:12:31.917930 appthreat-depscan-4.2.0/vendor/choosealicense.com/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:12:31.925930 appthreat-depscan-4.2.0/vendor/choosealicense.com/_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_data/fields.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_data/meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_data/rules.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:12:31.929931 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/0bsd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/afl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35944 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/agpl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/artistic-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/bsd-2-clause.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/bsd-3-clause.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/bsd-4-clause.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/bsl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19759 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/cc-by-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    21474 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/cc0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23872 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/cecill-2.1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/ecl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/epl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/epl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14163 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/eupl-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14871 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/eupl-1.2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23969 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/gfdl-1.3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/gpl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    36394 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/gpl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/isc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    27491 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/lgpl-2.1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/lgpl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19902 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/lppl-1.3c.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/mit-0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/mit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18103 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/mpl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/ms-pl.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/ms-rl.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/ncsa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26179 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/odbl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/ofl-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/osl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/postgresql.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/upl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/vim.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/wtfpl.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/zlib.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:12:31.917930 appthreat-depscan-4.2.0/vendor/spdx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:12:31.929931 appthreat-depscan-4.2.0/vendor/spdx/json/
+-rw-r--r--   0 runner    (1001) docker     (123)   251610 2023-06-30 23:12:12.000000 appthreat-depscan-4.2.0/vendor/spdx/json/licenses.json
```

### Comparing `appthreat-depscan-4.1.2/LICENSE` & `appthreat-depscan-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/PKG-INFO` & `appthreat-depscan-4.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: appthreat-depscan
-Version: 4.1.2
+Version: 4.2.0
 Summary: Fully open-source security audit for project dependencies based on known vulnerabilities and advisories.
-Home-page: https://github.com/appthreat/dep-scan
-Author: Team AppThreat
-Author-email: cloud@appthreat.com
+Author-email: Team AppThreat <cloud@appthreat.com>
 License: MIT
+Project-URL: Homepage, https://github.com/appthreat/dep-scan
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
-Classifier: Topic :: Utilities
-Classifier: Topic :: Security
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Topic :: Security
+Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Introduction
 
 dep-scan is a fully open-source security audit tool based on known vulnerabilities, advisories, and license limitations for project dependencies. Both local repositories and container images are supported as the input, and the tool is ideal for CI environments with built-in build-breaker logic.
 
 ![Depscan logo](dep-scan.png)
 
+[![release](https://github.com/appthreat/dep-scan/actions/workflows/pythonpublish.yml/badge.svg)](https://github.com/appthreat/dep-scan/actions/workflows/pythonpublish.yml)
+[![Downloads](https://static.pepy.tech/badge/appthreat-depscan)](https://pepy.tech/project/appthreat-depscan)
+[![Discord](https://img.shields.io/badge/-Discord-lime?style=for-the-badge&logo=discord&logoColor=white&color=black)](https://discord.gg/pF4BYWEJcS)
+
 ## Features
 
 - Scan most application code - local repos, Linux container images, Kubernetes manifests, and OS - to identify known CVEs with prioritization
 - Package vulnerability scanning is performed locally and is quite fast. No server is used!
 - Generate Software Bill-of-Materials (SBoM) with Vulnerability Exploitability Exchange (VEX) information
 - Perform deep packages risk audit for dependency confusion attacks and maintenance risks (See risk audit)
 
@@ -52,14 +56,16 @@
 - Amazon Linux
 - Arch Linux
 - RHEL/CentOS
 - Rocky Linux
 - Ubuntu
 - OpenSUSE/SLES
 - Photon
+- Chainguard
+- Wolfi OS
 
 Application vulnerabilities would be reported for all Linux distros and Windows. To download the full vulnerability database suitable for scanning OS, invoke dep-scan with `--cache-os` for the first time. dep-scan would also download the appropriate database based on project type automatically.
 
 ## Usage
 
 dep-scan is ideal for use during continuous integration (CI) and as a local development tool.
 
@@ -79,23 +85,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/depscan-bin/releases). These binary bundle the following:
 
 - dep-scan with Python 3.10
 - cdxgen with Node.js 18
 - cdxgen binary plugins
 
 ```bash
-curl -LO https://github.com/appthreat/depscan-bin/releases/download/v4.1.1/depscan-linux-amd64
+curl -LO https://github.com/appthreat/depscan-bin/releases/latest/download/depscan-linux-amd64
 chmod +x depscan-linux-amd64
 ./depscan-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/depscan-bin/releases/download/v4.1.1/depscan.exe
+curl -LO https://github.com/appthreat/depscan-bin/releases/latest/download/depscan.exe
 .\depscan.exe --help
 ```
 
 ### Server mode
 
 dep-scan and cdxgen could be run in server mode. Use the included docker compose file to get started.
 
@@ -188,16 +194,14 @@
                         ThreatDB server url. Eg: https://api.sbom.cx
   --threatdb-username THREATDB_USERNAME
                         ThreatDB username
   --threatdb-password THREATDB_PASSWORD
                         ThreatDB password
   --threatdb-token THREATDB_TOKEN
                         ThreatDB token for token based submission
-  --privado-json PRIVADO_JSON
-                        Enrich the VEX report with information from privado.ai json report.
 ```
 
 ### Scanning containers locally (Python version)
 
 Scan `latest` tag of the container `shiftleft/scan-slim`
 
 ```bash
@@ -229,33 +233,33 @@
 ### Scanning projects locally (Docker container)
 
 `ghcr.io/appthreat/dep-scan` or `public.ecr.aws/appthreat/dep-scan:latest` container image can be used to perform the scan.
 
 To scan with default settings
 
 ```bash
-docker run --rm -v $PWD:/app ghcr.io/appthreat/dep-scan scan --src /app --reports-dir /app/reports
+docker run --rm -v $PWD:/app ghcr.io/appthreat/dep-scan --src /app --reports-dir /app/reports
 ```
 
 Using AWS public ECR image
 
 ```bash
-docker run --rm -v $PWD:/app public.ecr.aws/appthreat/dep-scan scan --src /app --reports-dir /app/reports
+docker run --rm -v $PWD:/app public.ecr.aws/appthreat/dep-scan --src /app --reports-dir /app/reports
 ```
 
 To scan with custom environment variables based configuration
 
 ```bash
 docker run --rm \
     -e VDB_HOME=/db \
     -e NVD_START_YEAR=2010 \
     -e GITHUB_PAGE_COUNT=5 \
     -e GITHUB_TOKEN=<token> \
     -v /tmp:/db \
-    -v $PWD:/app ghcr.io/appthreat/dep-scan scan --src /app --reports-dir /app/reports
+    -v $PWD:/app ghcr.io/appthreat/dep-scan --src /app --reports-dir /app/reports
 ```
 
 In the above example, `/tmp` is mounted as `/db` into the container. This directory is then specified as `VDB_HOME` for caching the vulnerability information. This way the database can be cached and reused to improve performance.
 
 ## Supported languages and package format
 
 dep-scan uses [cdxgen](https://github.com/CycloneDX/cdxgen) command internally to create Software Bill-of-Materials (SBoM) file for the project. This is then used for performing the scans.
```

### Comparing `appthreat-depscan-4.1.2/README.md` & `appthreat-depscan-4.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Introduction
 
 dep-scan is a fully open-source security audit tool based on known vulnerabilities, advisories, and license limitations for project dependencies. Both local repositories and container images are supported as the input, and the tool is ideal for CI environments with built-in build-breaker logic.
 
 ![Depscan logo](dep-scan.png)
 
+[![release](https://github.com/appthreat/dep-scan/actions/workflows/pythonpublish.yml/badge.svg)](https://github.com/appthreat/dep-scan/actions/workflows/pythonpublish.yml)
+[![Downloads](https://static.pepy.tech/badge/appthreat-depscan)](https://pepy.tech/project/appthreat-depscan)
+[![Discord](https://img.shields.io/badge/-Discord-lime?style=for-the-badge&logo=discord&logoColor=white&color=black)](https://discord.gg/pF4BYWEJcS)
+
 ## Features
 
 - Scan most application code - local repos, Linux container images, Kubernetes manifests, and OS - to identify known CVEs with prioritization
 - Package vulnerability scanning is performed locally and is quite fast. No server is used!
 - Generate Software Bill-of-Materials (SBoM) with Vulnerability Exploitability Exchange (VEX) information
 - Perform deep packages risk audit for dependency confusion attacks and maintenance risks (See risk audit)
 
@@ -29,14 +33,16 @@
 - Amazon Linux
 - Arch Linux
 - RHEL/CentOS
 - Rocky Linux
 - Ubuntu
 - OpenSUSE/SLES
 - Photon
+- Chainguard
+- Wolfi OS
 
 Application vulnerabilities would be reported for all Linux distros and Windows. To download the full vulnerability database suitable for scanning OS, invoke dep-scan with `--cache-os` for the first time. dep-scan would also download the appropriate database based on project type automatically.
 
 ## Usage
 
 dep-scan is ideal for use during continuous integration (CI) and as a local development tool.
 
@@ -56,23 +62,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/depscan-bin/releases). These binary bundle the following:
 
 - dep-scan with Python 3.10
 - cdxgen with Node.js 18
 - cdxgen binary plugins
 
 ```bash
-curl -LO https://github.com/appthreat/depscan-bin/releases/download/v4.1.1/depscan-linux-amd64
+curl -LO https://github.com/appthreat/depscan-bin/releases/latest/download/depscan-linux-amd64
 chmod +x depscan-linux-amd64
 ./depscan-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/depscan-bin/releases/download/v4.1.1/depscan.exe
+curl -LO https://github.com/appthreat/depscan-bin/releases/latest/download/depscan.exe
 .\depscan.exe --help
 ```
 
 ### Server mode
 
 dep-scan and cdxgen could be run in server mode. Use the included docker compose file to get started.
 
@@ -165,16 +171,14 @@
                         ThreatDB server url. Eg: https://api.sbom.cx
   --threatdb-username THREATDB_USERNAME
                         ThreatDB username
   --threatdb-password THREATDB_PASSWORD
                         ThreatDB password
   --threatdb-token THREATDB_TOKEN
                         ThreatDB token for token based submission
-  --privado-json PRIVADO_JSON
-                        Enrich the VEX report with information from privado.ai json report.
 ```
 
 ### Scanning containers locally (Python version)
 
 Scan `latest` tag of the container `shiftleft/scan-slim`
 
 ```bash
@@ -206,33 +210,33 @@
 ### Scanning projects locally (Docker container)
 
 `ghcr.io/appthreat/dep-scan` or `public.ecr.aws/appthreat/dep-scan:latest` container image can be used to perform the scan.
 
 To scan with default settings
 
 ```bash
-docker run --rm -v $PWD:/app ghcr.io/appthreat/dep-scan scan --src /app --reports-dir /app/reports
+docker run --rm -v $PWD:/app ghcr.io/appthreat/dep-scan --src /app --reports-dir /app/reports
 ```
 
 Using AWS public ECR image
 
 ```bash
-docker run --rm -v $PWD:/app public.ecr.aws/appthreat/dep-scan scan --src /app --reports-dir /app/reports
+docker run --rm -v $PWD:/app public.ecr.aws/appthreat/dep-scan --src /app --reports-dir /app/reports
 ```
 
 To scan with custom environment variables based configuration
 
 ```bash
 docker run --rm \
     -e VDB_HOME=/db \
     -e NVD_START_YEAR=2010 \
     -e GITHUB_PAGE_COUNT=5 \
     -e GITHUB_TOKEN=<token> \
     -v /tmp:/db \
-    -v $PWD:/app ghcr.io/appthreat/dep-scan scan --src /app --reports-dir /app/reports
+    -v $PWD:/app ghcr.io/appthreat/dep-scan --src /app --reports-dir /app/reports
 ```
 
 In the above example, `/tmp` is mounted as `/db` into the container. This directory is then specified as `VDB_HOME` for caching the vulnerability information. This way the database can be cached and reused to improve performance.
 
 ## Supported languages and package format
 
 dep-scan uses [cdxgen](https://github.com/CycloneDX/cdxgen) command internally to create Software Bill-of-Materials (SBoM) file for the project. This is then used for performing the scans.
```

### Comparing `appthreat-depscan-4.1.2/appthreat_depscan.egg-info/PKG-INFO` & `appthreat-depscan-4.2.0/appthreat_depscan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: appthreat-depscan
-Version: 4.1.2
+Version: 4.2.0
 Summary: Fully open-source security audit for project dependencies based on known vulnerabilities and advisories.
-Home-page: https://github.com/appthreat/dep-scan
-Author: Team AppThreat
-Author-email: cloud@appthreat.com
+Author-email: Team AppThreat <cloud@appthreat.com>
 License: MIT
+Project-URL: Homepage, https://github.com/appthreat/dep-scan
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
-Classifier: Topic :: Utilities
-Classifier: Topic :: Security
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Topic :: Security
+Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Introduction
 
 dep-scan is a fully open-source security audit tool based on known vulnerabilities, advisories, and license limitations for project dependencies. Both local repositories and container images are supported as the input, and the tool is ideal for CI environments with built-in build-breaker logic.
 
 ![Depscan logo](dep-scan.png)
 
+[![release](https://github.com/appthreat/dep-scan/actions/workflows/pythonpublish.yml/badge.svg)](https://github.com/appthreat/dep-scan/actions/workflows/pythonpublish.yml)
+[![Downloads](https://static.pepy.tech/badge/appthreat-depscan)](https://pepy.tech/project/appthreat-depscan)
+[![Discord](https://img.shields.io/badge/-Discord-lime?style=for-the-badge&logo=discord&logoColor=white&color=black)](https://discord.gg/pF4BYWEJcS)
+
 ## Features
 
 - Scan most application code - local repos, Linux container images, Kubernetes manifests, and OS - to identify known CVEs with prioritization
 - Package vulnerability scanning is performed locally and is quite fast. No server is used!
 - Generate Software Bill-of-Materials (SBoM) with Vulnerability Exploitability Exchange (VEX) information
 - Perform deep packages risk audit for dependency confusion attacks and maintenance risks (See risk audit)
 
@@ -52,14 +56,16 @@
 - Amazon Linux
 - Arch Linux
 - RHEL/CentOS
 - Rocky Linux
 - Ubuntu
 - OpenSUSE/SLES
 - Photon
+- Chainguard
+- Wolfi OS
 
 Application vulnerabilities would be reported for all Linux distros and Windows. To download the full vulnerability database suitable for scanning OS, invoke dep-scan with `--cache-os` for the first time. dep-scan would also download the appropriate database based on project type automatically.
 
 ## Usage
 
 dep-scan is ideal for use during continuous integration (CI) and as a local development tool.
 
@@ -79,23 +85,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/depscan-bin/releases). These binary bundle the following:
 
 - dep-scan with Python 3.10
 - cdxgen with Node.js 18
 - cdxgen binary plugins
 
 ```bash
-curl -LO https://github.com/appthreat/depscan-bin/releases/download/v4.1.1/depscan-linux-amd64
+curl -LO https://github.com/appthreat/depscan-bin/releases/latest/download/depscan-linux-amd64
 chmod +x depscan-linux-amd64
 ./depscan-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/depscan-bin/releases/download/v4.1.1/depscan.exe
+curl -LO https://github.com/appthreat/depscan-bin/releases/latest/download/depscan.exe
 .\depscan.exe --help
 ```
 
 ### Server mode
 
 dep-scan and cdxgen could be run in server mode. Use the included docker compose file to get started.
 
@@ -188,16 +194,14 @@
                         ThreatDB server url. Eg: https://api.sbom.cx
   --threatdb-username THREATDB_USERNAME
                         ThreatDB username
   --threatdb-password THREATDB_PASSWORD
                         ThreatDB password
   --threatdb-token THREATDB_TOKEN
                         ThreatDB token for token based submission
-  --privado-json PRIVADO_JSON
-                        Enrich the VEX report with information from privado.ai json report.
 ```
 
 ### Scanning containers locally (Python version)
 
 Scan `latest` tag of the container `shiftleft/scan-slim`
 
 ```bash
@@ -229,33 +233,33 @@
 ### Scanning projects locally (Docker container)
 
 `ghcr.io/appthreat/dep-scan` or `public.ecr.aws/appthreat/dep-scan:latest` container image can be used to perform the scan.
 
 To scan with default settings
 
 ```bash
-docker run --rm -v $PWD:/app ghcr.io/appthreat/dep-scan scan --src /app --reports-dir /app/reports
+docker run --rm -v $PWD:/app ghcr.io/appthreat/dep-scan --src /app --reports-dir /app/reports
 ```
 
 Using AWS public ECR image
 
 ```bash
-docker run --rm -v $PWD:/app public.ecr.aws/appthreat/dep-scan scan --src /app --reports-dir /app/reports
+docker run --rm -v $PWD:/app public.ecr.aws/appthreat/dep-scan --src /app --reports-dir /app/reports
 ```
 
 To scan with custom environment variables based configuration
 
 ```bash
 docker run --rm \
     -e VDB_HOME=/db \
     -e NVD_START_YEAR=2010 \
     -e GITHUB_PAGE_COUNT=5 \
     -e GITHUB_TOKEN=<token> \
     -v /tmp:/db \
-    -v $PWD:/app ghcr.io/appthreat/dep-scan scan --src /app --reports-dir /app/reports
+    -v $PWD:/app ghcr.io/appthreat/dep-scan --src /app --reports-dir /app/reports
 ```
 
 In the above example, `/tmp` is mounted as `/db` into the container. This directory is then specified as `VDB_HOME` for caching the vulnerability information. This way the database can be cached and reused to improve performance.
 
 ## Supported languages and package format
 
 dep-scan uses [cdxgen](https://github.com/CycloneDX/cdxgen) command internally to create Software Bill-of-Materials (SBoM) file for the project. This is then used for performing the scans.
```

### Comparing `appthreat-depscan-4.1.2/appthreat_depscan.egg-info/SOURCES.txt` & `appthreat-depscan-4.2.0/appthreat_depscan.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
-setup.py
+pyproject.toml
 appthreat_depscan.egg-info/PKG-INFO
 appthreat_depscan.egg-info/SOURCES.txt
 appthreat_depscan.egg-info/dependency_links.txt
 appthreat_depscan.egg-info/entry_points.txt
 appthreat_depscan.egg-info/requires.txt
 appthreat_depscan.egg-info/top_level.txt
 depscan/__init__.py
```

### Comparing `appthreat-depscan-4.1.2/depscan/cli.py` & `appthreat-depscan-4.2.0/depscan/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 import json
 import os
 import tempfile
 
 from quart import Quart, request
 from rich.panel import Panel
 from rich.terminal_theme import MONOKAI
-from vdb.lib import config as config
+from vdb.lib import config
 from vdb.lib import db as dbLib
 from vdb.lib.aqua import AquaSource
 from vdb.lib.gha import GitHubSource
 from vdb.lib.nvd import NvdSource
 from vdb.lib.osv import OSVSource
 
 from depscan.lib import privado
-from depscan.lib import utils as utils
+from depscan.lib import utils
 from depscan.lib.analysis import (
-    analyse,
+    summary_stats,
     analyse_licenses,
     analyse_pkg_risks,
     jsonl_report,
     prepare_vex,
     suggest_version,
 )
 from depscan.lib.audit import audit, risk_audit, risk_audit_map, type_audit_map
@@ -239,28 +239,27 @@
     :param project_type: Project Type
     :param pkg_list: List of packages
     :param suggest_mode: True if package fix version should be normalized across findings
     """
     if not pkg_list:
         LOG.debug("Empty package search attempted!")
     else:
-        LOG.info("Scanning {} oss dependencies for issues".format(len(pkg_list)))
+        LOG.debug("Scanning %d oss dependencies for issues", len(pkg_list))
     results, pkg_aliases, purl_aliases = utils.search_pkgs(db, project_type, pkg_list)
     # pkg_aliases is a dict that can be used to find the original vendor and package name
     # This way we consistently use the same names used by the caller irrespective of how
     # the result was obtained
     sug_version_dict = {}
     if suggest_mode:
         # From the results identify optimal max version
         sug_version_dict = suggest_version(results, pkg_aliases)
         if sug_version_dict:
             LOG.debug(
-                "Adjusting fix version based on the initial suggestion {}".format(
-                    sug_version_dict
-                )
+                "Adjusting fix version based on the initial suggestion %s",
+                sug_version_dict,
             )
             # Recheck packages
             sug_pkg_list = []
             for k, v in sug_version_dict.items():
                 if not v:
                     continue
                 vendor = ""
@@ -269,27 +268,27 @@
                 tmpA = k.split(":")
                 if len(tmpA) == 2:
                     vendor = tmpA[0]
                     name = tmpA[1]
                 else:
                     name = tmpA[0]
                 # De-alias the vendor and package name
-                full_pkg = "{}:{}".format(vendor, name)
+                full_pkg = f"{vendor}:{name}"
                 full_pkg = pkg_aliases.get(full_pkg, full_pkg)
                 vendor, name = full_pkg.split(":")
                 sug_pkg_list.append(
                     {"vendor": vendor, "name": name, "version": version}
                 )
             LOG.debug(
                 "Re-checking our suggestion to ensure there are no further vulnerabilities"
             )
             override_results, _, _ = utils.search_pkgs(db, project_type, sug_pkg_list)
             if override_results:
                 new_sug_dict = suggest_version(override_results)
-                LOG.debug("Received override results: {}".format(new_sug_dict))
+                LOG.debug("Received override results: %s", new_sug_dict)
                 for nk, nv in new_sug_dict.items():
                     sug_version_dict[nk] = nv
     return results, pkg_aliases, sug_version_dict, purl_aliases
 
 
 def summarise(
     project_type,
@@ -314,15 +313,15 @@
     :param report_file: Output report file
     :param bom_file: SBoM file
     :param privado_json_file Privado json file
     :param no_vuln_table: Boolean to indicate if the results should get printed to the console
     :return: Summary of the results
     """
     if not results:
-        LOG.info(f"No oss vulnerabilities detected for type {project_type} ✅")
+        LOG.info("No oss vulnerabilities detected for type %s ✅", project_type)
         return None
     if report_file:
         jsonl_report(
             project_type,
             results,
             pkg_aliases,
             purl_aliases,
@@ -332,41 +331,43 @@
         )
     pkg_vulnerabilities = prepare_vex(
         project_type,
         results,
         pkg_aliases,
         purl_aliases,
         sug_version_dict,
-        scoped_pkgs,
-        no_vuln_table,
+        scoped_pkgs=scoped_pkgs,
+        no_vuln_table=no_vuln_table,
+        bom_file=bom_file,
     )
 
     if pkg_vulnerabilities and bom_file:
         vex_file = bom_file.replace(".json", ".vex.json")
         try:
-            with open(bom_file) as fp:
+            with open(bom_file, encoding="utf-8") as fp:
                 bom_data = json.load(fp)
                 if bom_data:
                     bom_data["vulnerabilities"] = pkg_vulnerabilities
                     # Look for any privado json file
                     if os.path.exists(privado_json_file):
                         pservice = privado.process_report(privado_json_file)
                         if pservice:
                             LOG.info(
-                                f"Including the service identified by privado from {privado_json_file}"
+                                "Including the service identified by privado from %s",
+                                privado_json_file,
                             )
                             if not bom_data.get("services"):
                                 bom_data["services"] = []
                             bom_data["services"].insert(0, pservice)
-                    with open(vex_file, mode="w") as vexfp:
+                    with open(vex_file, mode="w", encoding="utf-8") as vexfp:
                         json.dump(bom_data, vexfp)
-                        LOG.info(f"VEX file {vex_file} generated successfully")
+                        LOG.info("VEX file %s generated successfully", vex_file)
         except Exception:
             LOG.warning("Unable to generate VEX file for this scan")
-    summary = analyse(project_type, results)
+    summary = summary_stats(project_type, results)
     return summary
 
 
 @app.get("/")
 async def index():
     return {}
 
@@ -379,15 +380,15 @@
         sources_list = [OSVSource(), NvdSource()]
         if os.environ.get("GITHUB_TOKEN"):
             sources_list.insert(0, GitHubSource())
         # Include aqua source when ?os=true query string is passed
         if q.get("os", "").lower() in ("true", "1"):
             sources_list.insert(0, AquaSource())
         for s in sources_list:
-            LOG.debug("Refreshing {}".format(s.__class__.__name__))
+            LOG.debug("Refreshing %s", s.__class__.__name__)
             s.refresh()
         return {
             "error": "false",
             "message": "vulnerability database cached successfully",
         }
     return {"error": "false", "message": "vulnerability database already exists"}
 
@@ -437,19 +438,19 @@
                 "path": path,
                 "type": project_type,
                 "multiProject": multiProject,
                 "cdxgen_server": cdxgen_server,
             },
         )
         if bom_status:
-            LOG.debug(f"BOM file was generated successfully at {bfp.name}")
+            LOG.debug("BOM file was generated successfully at %s", bfp.name)
             pkg_list = get_pkg_list(bfp.name)
             if not pkg_list:
                 return {}
-            if project_type in type_audit_map.keys():
+            if project_type in type_audit_map:
                 audit_results = audit(project_type, pkg_list, None)
                 if audit_results:
                     results = results + audit_results
             vdb_results, pkg_aliases, sug_version_dict, purl_aliases = scan(
                 db, project_type, pkg_list, True
             )
             if vdb_results:
@@ -457,41 +458,44 @@
             bom_data = json.load(bfp)
             pkg_vulnerabilities = prepare_vex(
                 project_type,
                 results,
                 pkg_aliases,
                 purl_aliases,
                 sug_version_dict,
-                {},
-                True,
+                scoped_pkgs={},
+                no_vuln_table=True,
+                bom_file=bfp.name,
             )
             if pkg_vulnerabilities:
                 bom_data["vulnerabilities"] = pkg_vulnerabilities
             return json.dumps(bom_data)
         else:
             return {
                 "error": "true",
                 "message": "Unable to generate SBoM. Check your input path or url.",
             }, 500
     return {}
 
 
 def run_server(args):
+    """Run depscan as server"""
     print(at_logo)
     console.print(f"Depscan server running on {args.server_host}:{args.server_port}")
     app.config["CDXGEN_SERVER_URL"] = args.cdxgen_server
     app.run(
         host=args.server_host,
         port=args.server_port,
         debug=True if os.getenv("SCAN_DEBUG_MODE") == "debug" else False,
         use_reloader=False,
     )
 
 
 def main():
+    """Main function"""
     args = build_args()
     if args.server_mode:
         return run_server(args)
     if not args.no_banner:
         print(at_logo)
     src_dir = args.src_dir_image
     if not src_dir:
@@ -514,15 +518,15 @@
         else os.path.join(reports_dir, "depscan.json")
     )
     html_file = areport_file.replace(".json", ".html")
     # Create reports directory
     if reports_dir and not os.path.exists(reports_dir):
         os.makedirs(reports_dir, exist_ok=True)
     if len(project_types_list) > 1:
-        LOG.debug("Multiple project types found: {}".format(project_types_list))
+        LOG.debug("Multiple project types found: %s", project_types_list)
     # Enable license scanning
     if "license" in project_types_list:
         os.environ["FETCH_LICENSE"] = "true"
         project_types_list.remove("license")
         console.print(
             Panel(
                 "License audit is enabled for this scan. This would increase the time by up to 10 minutes.",
@@ -530,18 +534,16 @@
                 expand=False,
             )
         )
     for project_type in project_types_list:
         sug_version_dict = {}
         pkg_aliases = {}
         results = []
-        report_file = areport_file.replace(".json", "-{}.json".format(project_type))
-        risk_report_file = areport_file.replace(
-            ".json", "-risk.{}.json".format(project_type)
-        )
+        report_file = areport_file.replace(".json", f"-{project_type}.json")
+        risk_report_file = areport_file.replace(".json", f"-risk.{project_type}.json")
         LOG.info("=" * 80)
         creation_status = False
         if args.bom and os.path.exists(args.bom):
             bom_file = args.bom
             creation_status = True
         else:
             bom_file = report_file.replace("depscan-", "sbom-")
@@ -549,46 +551,37 @@
                 project_type,
                 bom_file,
                 src_dir,
                 args.deep_scan,
                 {"cdxgen_server": args.cdxgen_server},
             )
         if not creation_status:
-            LOG.debug("Bom file {} was not created successfully".format(bom_file))
+            LOG.debug("Bom file %s was not created successfully", bom_file)
             continue
-        LOG.info("Scanning using the bom file {}".format(bom_file))
+        LOG.debug("Scanning using the bom file %s", bom_file)
         if not args.bom:
             LOG.info(
-                "To improve performance, cache this bom file and invoke depscan with --bom {} instead of -i".format(
-                    bom_file
-                )
+                "To improve performance, cache this bom file and invoke depscan with --bom %s instead of -i",
+                bom_file,
             )
         pkg_list = get_pkg_list(bom_file)
         if not pkg_list:
             LOG.debug("No packages found in the project!")
             continue
-        scoped_pkgs = {}
-        if project_type in ["python"]:
-            all_imports = utils.get_all_imports(src_dir)
-            LOG.debug(f"Identified {len(all_imports)} imports in your project")
-            scoped_pkgs = utils.get_scope_from_imports(
-                project_type, pkg_list, all_imports
-            )
-        else:
-            scoped_pkgs = utils.get_pkgs_by_scope(project_type, pkg_list)
+        scoped_pkgs = utils.get_pkgs_by_scope(project_type, pkg_list)
         if os.getenv("FETCH_LICENSE", "") in (True, "1", "true"):
             licenses_results = bulk_lookup(
                 build_license_data(license_data_dir, spdx_license_list),
                 pkg_list=pkg_list,
             )
             license_report_file = os.path.join(
                 reports_dir, "license-" + project_type + ".json"
             )
             analyse_licenses(project_type, licenses_results, license_report_file)
-        if project_type in risk_audit_map.keys():
+        if project_type in risk_audit_map:
             if args.risk_audit:
                 console.print(
                     Panel(
                         f"Performing OSS Risk Audit for packages from {src_dir}\nNo of packages [bold]{len(pkg_list)}[/bold]. This will take a while ...",
                         title="OSS Risk Audit",
                         expand=False,
                     )
@@ -615,80 +608,67 @@
                 console.print(
                     Panel(
                         "Depscan supports OSS Risk audit for this project.\nTo enable set the environment variable [bold]ENABLE_OSS_RISK=true[/bold]",
                         title="New Feature",
                         expand=False,
                     )
                 )
-        if project_type in type_audit_map.keys():
-            LOG.info(
-                "Performing remote audit for {} of type {}".format(
-                    src_dir, project_type
-                )
-            )
-            LOG.debug(f"No of packages {len(pkg_list)}")
+        if project_type in type_audit_map:
+            LOG.info("Performing remote audit for %s of type %s", src_dir, project_type)
+            LOG.debug("No of packages %d", len(pkg_list))
             try:
                 audit_results = audit(project_type, pkg_list, report_file)
                 if audit_results:
-                    LOG.debug(f"Remote audit yielded {len(audit_results)} results")
+                    LOG.debug("Remote audit yielded %d results", len(audit_results))
                     results = results + audit_results
             except Exception as e:
                 LOG.error("Remote audit was not successful")
                 LOG.error(e)
                 results = []
         # In case of docker, check if there are any npm packages that can be audited remotely
         if project_type in ("podman", "docker", "oci"):
             npm_pkg_list = get_pkg_by_type(pkg_list, "npm")
             if npm_pkg_list:
-                LOG.debug(f"No of npm packages {len(npm_pkg_list)}")
+                LOG.debug("No of npm packages %d", len(npm_pkg_list))
                 try:
                     audit_results = audit("nodejs", npm_pkg_list, report_file)
                     if audit_results:
-                        LOG.debug(f"Remote audit yielded {len(audit_results)} results")
+                        LOG.debug("Remote audit yielded %d results", len(audit_results))
                         results = results + audit_results
                 except Exception as e:
                     LOG.error("Remote audit was not successful")
                     LOG.error(e)
         if not dbLib.index_count(db["index_file"]):
             run_cacher = True
         else:
-            LOG.debug(
-                "Vulnerability database loaded from {}".format(config.vdb_bin_file)
-            )
+            LOG.debug("Vulnerability database loaded from %s", config.vdb_bin_file)
         sources_list = [OSVSource(), NvdSource()]
         if os.environ.get("GITHUB_TOKEN"):
             sources_list.insert(0, GitHubSource())
         if run_cacher:
             if (
                 args.cache_os
                 or args.deep_scan
                 or project_type in ("docker", "podman", "yaml-manifest", "os")
             ):
                 sources_list.insert(0, AquaSource())
                 LOG.info(
-                    "OS Vulnerability database would be downloaded for the first time. This would take a few minutes ..."
+                    "OS Vulnerability database would be downloaded for the first time. To avoid this step, manually download the vulnerability database using the ORAS cli and set the environment variable VDB_HOME."
                 )
             for s in sources_list:
-                LOG.debug("Refreshing {}".format(s.__class__.__name__))
+                LOG.debug("Refreshing %s", s.__class__.__name__)
                 s.refresh()
                 run_cacher = False
         elif args.sync:
             for s in sources_list:
-                LOG.debug("Syncing {}".format(s.__class__.__name__))
+                LOG.debug("Syncing %s", s.__class__.__name__)
                 s.download_recent()
                 run_cacher = False
-        LOG.debug(
-            "Vulnerability database contains {} records".format(
-                dbLib.index_count(db["index_file"])
-            )
-        )
         LOG.info(
-            "Performing regular scan for {} using plugin {}".format(
-                src_dir, project_type
-            )
+            "Performing regular scan for %s using plugin %s", src_dir, project_type
         )
         vdb_results, pkg_aliases, sug_version_dict, purl_aliases = scan(
             db, project_type, pkg_list, args.suggest
         )
         if vdb_results:
             results = results + vdb_results
         # Summarise and print results
```

### Comparing `appthreat-depscan-4.1.2/depscan/lib/analysis.py` & `appthreat-depscan-4.2.0/depscan/lib/analysis.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,25 +2,29 @@
 
 import json
 from collections import defaultdict
 
 from rich import box
 from rich.panel import Panel
 from rich.table import Table
+from rich.tree import Tree
+from rich.style import Style
 from vdb.lib import CPE_FULL_REGEX
 from vdb.lib.config import placeholder_fix_version
 from vdb.lib.utils import parse_purl
 
-from depscan.lib import config as config
+from depscan.lib import config
 from depscan.lib.logger import LOG, console
 from depscan.lib.utils import max_version
 
+NEWLINE = "\\n"
+
 
 def best_fixed_location(version_used, sug_version, orig_fixed_location):
-    # Compare the major versions before suggesting an override
+    """Compare the major versions before suggesting an override"""
     # See: https://github.com/AppThreat/dep-scan/issues/72
     if (
         not orig_fixed_location
         and sug_version
         and sug_version != placeholder_fix_version
     ):
         return sug_version
@@ -34,35 +38,134 @@
     # Handle the placeholder version used by OS distros
     if orig_fixed_location == placeholder_fix_version:
         return ""
     return orig_fixed_location
 
 
 def distro_package(package_issue):
+    """Method to determine if the given CPE belongs to a OS distro"""
     if package_issue:
         all_parts = CPE_FULL_REGEX.match(package_issue.affected_location.cpe_uri)
         if (
             all_parts
             and all_parts.group("vendor")
             and all_parts.group("vendor") in config.LINUX_DISTRO_WITH_EDITIONS
             and all_parts.group("edition")
             and all_parts.group("edition") != "*"
         ):
             return True
     return False
 
 
+def retrieve_bom_dependency_tree(bom_file):
+    """Method to retrieve the dependency tree from a CycloneDX SBoM"""
+    if not bom_file:
+        return []
+    try:
+        with open(bom_file, encoding="utf-8") as bfp:
+            bom_data = json.load(bfp)
+            if bom_data:
+                return bom_data.get("dependencies", [])
+    except Exception:
+        pass
+    return []
+
+
+def get_pkg_display(tree_pkg, current_pkg, pkg_severity=None, extra_text=None):
+    """Construct a string that could be used for display"""
+    full_pkg_display = current_pkg
+    highlightable = tree_pkg and (tree_pkg == current_pkg or tree_pkg in current_pkg)
+    if tree_pkg:
+        try:
+            purl_obj = parse_purl(current_pkg)
+            if purl_obj:
+                version_used = purl_obj.get("version")
+                full_pkg_display = f"""{purl_obj.get("name")}@{version_used}"""
+        except Exception:
+            pass
+    if extra_text and highlightable:
+        full_pkg_display = f"{full_pkg_display} {extra_text}"
+    return full_pkg_display
+
+
+def get_tree_style(purl, p):
+    """Return a rich style to be used in a tree"""
+    if purl and (purl == p or purl in p):
+        return Style(color="#FF753D", bold=True, italic=False)
+    return Style(color="#7C8082", bold=False, italic=True)
+
+
+def pkg_sub_tree(
+    purl,
+    full_pkg,
+    bom_dependency_tree,
+    pkg_severity=None,
+    as_tree=False,
+    extra_text=None,
+):
+    """Method to locate and return a package tree from a dependency tree"""
+    pkg_tree = []
+    if full_pkg and not purl:
+        purl = full_pkg
+    if not bom_dependency_tree:
+        return [purl], Tree(
+            get_pkg_display(
+                purl, purl, pkg_severity=pkg_severity, extra_text=extra_text
+            ),
+            style=Style(color="bright_red" if pkg_severity == "CRITICAL" else None),
+        )
+    if len(bom_dependency_tree) > 1:
+        for dep in bom_dependency_tree[1:]:
+            ref = dep.get("ref")
+            depends_on = dep.get("dependsOn", [])
+            if purl in ref:
+                if not pkg_tree or (pkg_tree and ref != pkg_tree[-1]):
+                    pkg_tree.append(ref)
+            elif purl in depends_on and purl not in pkg_tree:
+                pkg_tree.append(ref)
+                pkg_tree.append(purl)
+                break
+    # We need to iterate again to identify any parent for the parent
+    if pkg_tree and len(bom_dependency_tree) > 1:
+        for dep in bom_dependency_tree[1:]:
+            if pkg_tree[0] in dep.get("dependsOn", []):
+                if dep.get("ref") not in pkg_tree:
+                    pkg_tree.insert(0, dep.get("ref"))
+                break
+        if as_tree and pkg_tree:
+            tree = Tree(
+                get_pkg_display(
+                    purl, pkg_tree[0], pkg_severity=pkg_severity, extra_text=extra_text
+                ),
+                style=get_tree_style(purl, pkg_tree[0]),
+            )
+            if len(pkg_tree) > 1:
+                for p in pkg_tree[1:]:
+                    tree.add(
+                        get_pkg_display(
+                            purl, p, pkg_severity=pkg_severity, extra_text=extra_text
+                        ),
+                        style=get_tree_style(purl, p),
+                    )
+            return pkg_tree, tree
+    return pkg_tree, Tree(
+        get_pkg_display(purl, purl, pkg_severity=pkg_severity, extra_text=extra_text),
+        style=Style(color="bright_red" if pkg_severity == "CRITICAL" else None),
+    )
+
+
 def prepare_vex(
     project_type,
     results,
     pkg_aliases,
     purl_aliases,
     sug_version_dict,
     scoped_pkgs,
-    no_vuln_table,
+    no_vuln_table=False,
+    bom_file=None,
 ):
     """Pretty print report summary"""
     if not results:
         return []
     table = Table(
         title=f"Dependency Scan Results ({project_type})",
         box=box.DOUBLE_EDGE,
@@ -80,41 +183,36 @@
     wont_fix_version_count = 0
     has_os_packages = False
     has_redhat_packages = False
     has_ubuntu_packages = False
     distro_packages_count = 0
     pkg_group_rows = defaultdict(list)
     pkg_vulnerabilities = []
+    # Retrieve any dependency tree from the SBoM
+    bom_dependency_tree = retrieve_bom_dependency_tree(bom_file)
     for h in [
-        "CVE",
-        "Package",
+        "Dependency Tree" if len(bom_dependency_tree) > 0 else "CVE",
         "Insights",
-        "Version",
         "Fix Version",
         "Severity",
         "Score",
     ]:
         justify = "left"
         if h == "Score":
             justify = "right"
         table.add_column(header=h, justify=justify, no_wrap=False)
     for res in results:
         vuln_occ_dict = res.to_dict()
-        id = vuln_occ_dict.get("id")
+        vid = vuln_occ_dict.get("id")
         problem_type = vuln_occ_dict.get("problem_type")
         package_issue = res.package_issue
         full_pkg = package_issue.affected_location.package
-        project_type_pkg = "{}:{}".format(
-            project_type, package_issue.affected_location.package
-        )
+        project_type_pkg = f"{project_type}:{package_issue.affected_location.package}"
         if package_issue.affected_location.vendor:
-            full_pkg = "{}:{}".format(
-                package_issue.affected_location.vendor,
-                package_issue.affected_location.package,
-            )
+            full_pkg = f"{package_issue.affected_location.vendor}:{package_issue.affected_location.package}"
         # De-alias package names
         full_pkg = pkg_aliases.get(full_pkg, full_pkg)
         full_pkg_display = full_pkg
         version_used = package_issue.affected_location.version
         purl = purl_aliases.get(full_pkg, full_pkg)
         package_type = None
         if purl:
@@ -134,68 +232,76 @@
                         full_pkg_display = (
                             f"""{purl_obj.get("namespace")}/{purl_obj.get("name")}"""
                         )
                     else:
                         full_pkg_display = f"""{purl_obj.get("name")}"""
             except Exception:
                 pass
-        if ids_seen.get(id + full_pkg):
+        if ids_seen.get(vid + full_pkg):
             continue
-        ids_seen[id + full_pkg] = True
+        # Mark this CVE + pkg as seen to avoid duplicates
+        ids_seen[vid + full_pkg] = True
+        # Find the best fix version
         fixed_location = best_fixed_location(
             version_used, sug_version_dict.get(full_pkg), package_issue.fixed_location
         )
         if (
             sug_version_dict.get(full_pkg) == placeholder_fix_version
             or package_issue.fixed_location == placeholder_fix_version
         ):
             wont_fix_version_count = wont_fix_version_count + 1
         package_usage = "N/A"
         insights = []
         plain_insights = []
-        package_name_style = ""
-        id_style = ""
         pkg_severity = vuln_occ_dict.get("severity")
         is_required = False
         pkg_requires_attn = False
         related_urls = vuln_occ_dict.get("related_urls")
         clinks = classify_links(
-            id,
+            vid,
             full_pkg_display,
             vuln_occ_dict.get("type"),
             package_issue.affected_location.version,
             related_urls,
         )
         if full_pkg in required_pkgs or project_type_pkg in required_pkgs:
             is_required = True
         if pkg_severity in ("CRITICAL", "HIGH"):
             if is_required:
-                id_style = ":point_right: "
                 pkg_requires_attn = True
                 pkg_attention_count = pkg_attention_count + 1
             if fixed_location:
                 fix_version_count = fix_version_count + 1
             if (
                 clinks.get("vendor") or package_type in config.OS_PKG_TYPES
             ) and pkg_severity == "CRITICAL":
                 critical_count += 1
+        # Locate this package in the tree
+        pkg_tree_list, p_rich_tree = pkg_sub_tree(
+            purl,
+            full_pkg.replace(":", "/"),
+            bom_dependency_tree,
+            pkg_severity=pkg_severity,
+            as_tree=True,
+            extra_text=f":left_arrow: {vid}",
+        )
         if is_required and package_type not in config.OS_PKG_TYPES:
             package_usage = ":direct_hit: Direct usage"
-            package_name_style = "[bold]"
-        elif full_pkg in optional_pkgs or project_type_pkg in optional_pkgs:
+        elif (not optional_pkgs and pkg_tree_list and len(pkg_tree_list) > 1) or (
+            full_pkg in optional_pkgs or project_type_pkg in optional_pkgs
+        ):
             if package_type in config.OS_PKG_TYPES:
                 package_usage = (
                     "[spring_green4]:notebook: Local install[/spring_green4]"
                 )
                 has_os_packages = True
             else:
                 package_usage = (
                     "[spring_green4]:notebook: Indirect dependency[/spring_green4]"
                 )
-            package_name_style = "[italic]"
         if package_usage != "N/A":
             insights.append(package_usage)
             plain_insights.append(package_usage)
         if clinks.get("poc") or clinks.get("Bug Bounty"):
             insights.append("[yellow]:notebook_with_decorative_cover: Has PoC[/yellow]")
             plain_insights.append("Has PoC")
             has_poc_count = has_poc_count + 1
@@ -213,47 +319,40 @@
             insights.append(
                 "[spring_green4]:direct_hit: Distro specific[/spring_green4]"
             )
             plain_insights.append("Distro specific")
             distro_packages_count = distro_packages_count + 1
             has_os_packages = True
         if pkg_requires_attn and fixed_location and purl:
-            pkg_group_rows[purl].append({"id": id, "fixed_location": fixed_location})
+            pkg_group_rows[purl].append(
+                {
+                    "id": vid,
+                    "fixed_location": fixed_location,
+                    "p_rich_tree": p_rich_tree,
+                }
+            )
         if not no_vuln_table:
             table.add_row(
-                "{}{}{}{}".format(
-                    id_style,
-                    package_name_style,
-                    "[bright_red]" if pkg_severity == "CRITICAL" else "",
-                    id,
-                ),
-                "{}{}".format(package_name_style, full_pkg_display),
+                p_rich_tree,
                 "\n".join(insights),
-                version_used,
                 fixed_location,
-                "{}{}".format(
-                    "[bright_red]" if pkg_severity == "CRITICAL" else "",
-                    vuln_occ_dict.get("severity"),
-                ),
-                "{}{}".format(
-                    "[bright_red]" if pkg_severity == "CRITICAL" else "",
-                    vuln_occ_dict.get("cvss_score"),
-                ),
+                f"""{"[bright_red]" if pkg_severity == "CRITICAL" else ""}{vuln_occ_dict.get("severity")}""",
+                f"""{"[bright_red]" if pkg_severity == "CRITICAL" else ""}{vuln_occ_dict.get("cvss_score")}""",
             )
         if purl:
             source = {}
-            if id.startswith("CVE"):
+            if vid.startswith("CVE"):
                 source = {
                     "name": "NVD",
-                    "url": f"https://nvd.nist.gov/vuln/detail/{id}",
+                    "url": f"https://nvd.nist.gov/vuln/detail/{vid}",
                 }
-            elif id.startswith("GHSA") or id.startswith("npm"):
+            elif vid.startswith("GHSA") or vid.startswith("npm"):
                 source = {
                     "name": "GitHub",
-                    "url": f"https://github.com/advisories/{id}",
+                    "url": f"https://github.com/advisories/{vid}",
                 }
             versions = [{"version": version_used, "status": "affected"}]
             recommendation = ""
             if fixed_location:
                 versions.append({"version": fixed_location, "status": "unaffected"})
                 recommendation = f"Update to {fixed_location} or later"
             affects = [{"ref": purl, "versions": versions}]
@@ -261,14 +360,19 @@
             if clinks.get("exploit"):
                 analysis = {
                     "state": "exploitable",
                     "detail": f'See {clinks.get("exploit")}',
                 }
             elif clinks.get("poc"):
                 analysis = {"state": "in_triage", "detail": f'See {clinks.get("poc")}'}
+            elif pkg_tree_list and len(pkg_tree_list) > 1:
+                analysis = {
+                    "state": "in_triage",
+                    "detail": f"Dependency Tree: {json.dumps(pkg_tree_list)}",
+                }
             score = 2.0
             try:
                 score = float(vuln_occ_dict.get("cvss_score"))
             except Exception:
                 pass
             sev_to_use = pkg_severity.lower()
             if sev_to_use not in ("critical", "high", "medium", "low", "info", "none"):
@@ -288,16 +392,16 @@
                 try:
                     acwe = int(problem_type.lower().replace("cwe-", ""))
                     cwes = [acwe]
                 except Exception:
                     pass
             pkg_vulnerabilities.append(
                 {
-                    "bom-ref": f"{id}/{purl}",
-                    "id": id,
+                    "bom-ref": f"{vid}/{purl}",
+                    "id": vid,
                     "source": source,
                     "ratings": ratings,
                     "cwes": cwes,
                     "description": vuln_occ_dict.get("short_description"),
                     "recommendation": recommendation,
                     "advisories": advisories,
                     "analysis": analysis,
@@ -330,15 +434,15 @@
             cve_list = []
             fv = None
             for c in v:
                 cve_list.append(c.get("id"))
                 if not fv:
                     fv = c.get("fixed_location")
             utable.add_row(
-                k.split("#")[0].split("?")[0],
+                v[0].get("p_rich_tree"),
                 "\n".join(sorted(cve_list, reverse=True)),
                 f"[bright_green]{fv}[/bright_green]",
             )
         console.print(utable)
     if scoped_pkgs or has_exploit_count:
         if not pkg_attention_count and has_exploit_count:
             rmessage = f":point_right: [magenta]{has_exploit_count}[/magenta] out of {len(results)} vulnerabilities have known exploits and requires your [magenta]immediate[/magenta] attention."
@@ -423,15 +527,16 @@
                 title="Recommendation",
                 expand=False,
             )
         )
     return pkg_vulnerabilities
 
 
-def analyse(project_type, results):
+def summary_stats(project_type, results):
+    """Generate summary stats"""
     if not results:
         LOG.info("No oss vulnerabilities detected ✅")
         return None
     summary = {"UNSPECIFIED": 0, "LOW": 0, "MEDIUM": 0, "HIGH": 0, "CRITICAL": 0}
     for res in results:
         summary[res.severity] += 1
     return summary
@@ -453,25 +558,22 @@
     :param pkg_aliases: Package alias
     :param out_file_name: Output filename
     """
     ids_seen = {}
     required_pkgs = scoped_pkgs.get("required", [])
     optional_pkgs = scoped_pkgs.get("optional", [])
     excluded_pkgs = scoped_pkgs.get("excluded", [])
-    with open(out_file_name, "w") as outfile:
+    with open(out_file_name, "w", encoding="utf-8") as outfile:
         for data in results:
             vuln_occ_dict = data.to_dict()
-            id = vuln_occ_dict.get("id")
+            vid = vuln_occ_dict.get("id")
             package_issue = data.package_issue
             full_pkg = package_issue.affected_location.package
             if package_issue.affected_location.vendor:
-                full_pkg = "{}:{}".format(
-                    package_issue.affected_location.vendor,
-                    package_issue.affected_location.package,
-                )
+                full_pkg = f"{package_issue.affected_location.vendor}:{package_issue.affected_location.package}"
             # De-alias package names
             full_pkg = pkg_aliases.get(full_pkg, full_pkg)
             full_pkg_display = full_pkg
             version_used = package_issue.affected_location.version
             purl = purl_aliases.get(full_pkg, full_pkg)
             if purl:
                 try:
@@ -482,18 +584,18 @@
                             full_pkg = f"""{purl_obj.get("namespace")}/{purl_obj.get("name")}@{purl_obj.get("version")}"""
                         else:
                             full_pkg = (
                                 f"""{purl_obj.get("name")}@{purl_obj.get("version")}"""
                             )
                 except Exception:
                     pass
-            if ids_seen.get(id + full_pkg):
+            if ids_seen.get(vid + full_pkg):
                 continue
             # On occasions, this could still result in duplicates if the package exists with and without a purl
-            ids_seen[id + full_pkg] = True
+            ids_seen[vid + full_pkg] = True
             project_type_pkg = "{}:{}".format(
                 project_type, package_issue.affected_location.package
             )
             fixed_location = best_fixed_location(
                 version_used,
                 sug_version_dict.get(full_pkg),
                 package_issue.fixed_location,
@@ -502,15 +604,15 @@
             if full_pkg in required_pkgs or project_type_pkg in required_pkgs:
                 package_usage = "required"
             elif full_pkg in optional_pkgs or project_type_pkg in optional_pkgs:
                 package_usage = "optional"
             elif full_pkg in excluded_pkgs or project_type_pkg in excluded_pkgs:
                 package_usage = "excluded"
             data_obj = {
-                "id": id,
+                "id": vid,
                 "package": full_pkg_display,
                 "purl": purl,
                 "package_type": vuln_occ_dict.get("type"),
                 "package_usage": package_usage,
                 "version": version_used,
                 "fix_version": fixed_location,
                 "severity": vuln_occ_dict.get("severity"),
@@ -521,14 +623,15 @@
             json.dump(data_obj, outfile)
             outfile.write("\n")
 
 
 def analyse_pkg_risks(
     project_type, scoped_pkgs, private_ns, risk_results, risk_report_file=None
 ):
+    """Identify package risk and write to a json file"""
     if not risk_results:
         return
     table = Table(
         title=f"Risk Audit Summary ({project_type})",
         box=box.DOUBLE_EDGE,
         header_style="bold magenta",
     )
@@ -543,15 +646,15 @@
             justify = "right"
         table.add_column(header=h, justify=justify)
     for pkg, risk_obj in risk_results.items():
         if not risk_obj:
             continue
         risk_metrics = risk_obj.get("risk_metrics")
         scope = risk_obj.get("scope")
-        project_type_pkg = "{}:{}".format(project_type, pkg).lower()
+        project_type_pkg = f"{project_type}:{pkg}".lower()
         if project_type_pkg in required_pkgs:
             scope = "required"
         elif project_type_pkg in optional_pkgs:
             scope = "optional"
         elif project_type_pkg in excluded_pkgs:
             scope = "excluded"
         package_usage = "N/A"
@@ -596,23 +699,24 @@
             edata.append(", ".join(risk_categories_simple))
             table.add_row(*data)
             report_data.append(dict(zip(headers, edata)))
     if report_data:
         console.print(table)
         # Store the risk audit findings in jsonl format
         if risk_report_file:
-            with open(risk_report_file, "w") as outfile:
+            with open(risk_report_file, "w", encoding="utf-8") as outfile:
                 for row in report_data:
                     json.dump(row, outfile)
                     outfile.write("\n")
     else:
         LOG.info("No package risks detected ✅")
 
 
 def analyse_licenses(project_type, licenses_results, license_report_file=None):
+    """Analyze package licenses"""
     if not licenses_results:
         return
     table = Table(
         title=f"License Scan Summary ({project_type})",
         box=box.DOUBLE_EDGE,
         header_style="bold magenta",
     )
@@ -648,15 +752,15 @@
                 ]
                 table.add_row(*data)
                 report_data.append(dict(zip(headers, data)))
     if report_data:
         console.print(table)
         # Store the license scan findings in jsonl format
         if license_report_file:
-            with open(license_report_file, "w") as outfile:
+            with open(license_report_file, "w", encoding="utf-8") as outfile:
                 for row in report_data:
                     json.dump(row, outfile)
                     outfile.write("\n")
     else:
         LOG.info("No license violation detected ✅")
 
 
@@ -671,18 +775,15 @@
             full_pkg = res.get("package")
             fixed_location = res.get("fix_version")
         else:
             package_issue = res.package_issue
             full_pkg = package_issue.affected_location.package
             fixed_location = package_issue.fixed_location
             if package_issue.affected_location.vendor:
-                full_pkg = "{}:{}".format(
-                    package_issue.affected_location.vendor,
-                    package_issue.affected_location.package,
-                )
+                full_pkg = f"{package_issue.affected_location.vendor}:{package_issue.affected_location.package}"
         # De-alias package names
         full_pkg = pkg_aliases.get(full_pkg, full_pkg)
         version_upgrades = pkg_fix_map.get(full_pkg, set())
         version_upgrades.add(fixed_location)
         pkg_fix_map[full_pkg] = version_upgrades
     for k, v in pkg_fix_map.items():
         if v:
@@ -741,12 +842,18 @@
             or "seebug.org" in rurl
             or "seclists.org" in rurl
             or "nu11secur1ty" in rurl
         ):
             clinks["exploit"] = rurl
         elif "github.com/advisories" in rurl:
             clinks["GitHub Advisory"] = rurl
-        elif "hackerone" in rurl or "bugcrowd" in rurl or "bug-bounty" in rurl:
+        elif (
+            "hackerone" in rurl
+            or "bugcrowd" in rurl
+            or "bug-bounty" in rurl
+            or "huntr.dev" in rurl
+            or "bounties" in rurl
+        ):
             clinks["Bug Bounty"] = rurl
         elif "cwe.mitre.org" in rurl:
             clinks["cwe"] = rurl
     return clinks
```

### Comparing `appthreat-depscan-4.1.2/depscan/lib/audit.py` & `appthreat-depscan-4.2.0/depscan/lib/audit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from vdb.lib.npm import NpmSource
 
-from depscan.lib import config as config
+from depscan.lib import config
 from depscan.lib.pkg_query import npm_metadata, pypi_metadata
 
 # Dict mapping project type to the audit source
 type_audit_map = {"nodejs": NpmSource(), "js": NpmSource()}
 
 # Dict mapping project type to risk audit
 risk_audit_map = {
```

### Comparing `appthreat-depscan-4.1.2/depscan/lib/bom.py` & `appthreat-depscan-4.2.0/depscan/lib/bom.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     """
     Convenience method to invoke cli tools
 
     Args:
       args cli command and args
     """
     try:
-        LOG.debug('⚡︎ Executing "{}"'.format(" ".join(args)))
+        LOG.debug('⚡︎ Executing "%s"', " ".join(args))
         if os.environ.get("FETCH_LICENSE"):
             LOG.debug(
                 "License information would be fetched from the registry. This would take several minutes ..."
             )
         cp = subprocess.run(
             args,
             stdout=stdout,
@@ -84,17 +84,17 @@
         "name": name,
         "version": version,
         "licenses": licenses,
     }
 
 
 def get_licenses(ele):
-    """ """
+    """Retrieve licenses from xml"""
     license_list = []
-    namespace = "{http://cyclonedx.org/schema/bom/1.2}"
+    namespace = "{http://cyclonedx.org/schema/bom/1.5}"
     for data in ele.findall("{0}licenses/{0}license/{0}id".format(namespace)):
         license_list.append(data.text)
     if not license_list:
         for data in ele.findall("{0}licenses/{0}license/{0}name".format(namespace)):
             if data and data.text:
                 ld_list = [data.text]
                 if "http" in data.text:
@@ -107,15 +107,15 @@
                     ld_list = [cleanup_license_string(data.text)]
                 for ld in ld_list:
                     license_list.append(ld.strip().upper())
     return license_list
 
 
 def get_package(componentEle, licenses):
-    """ """
+    """Retrieve package from xml"""
     bom_ref = componentEle.attrib.get("bom-ref")
     pkg = {"licenses": licenses, "vendor": "", "name": "", "version": "", "scope": ""}
     if bom_ref and "/" in bom_ref:
         pkg = parse_bom_ref(bom_ref, licenses)
     for ele in componentEle.iter():
         if ele.tag.endswith("group") and ele.text:
             pkg["vendor"] = ele.text
@@ -132,15 +132,15 @@
             pkg["vendor"] = namespace
     return pkg
 
 
 def get_pkg_list_json(jsonfile):
     """Method to extract packages from a bom json file"""
     pkgs = []
-    with open(jsonfile) as fp:
+    with open(jsonfile, encoding="utf-8") as fp:
         try:
             bom_data = json.load(fp)
             if bom_data and bom_data.get("components"):
                 for comp in bom_data.get("components"):
                     licenses = []
                     vendor = comp.get("group")
                     if not vendor:
@@ -180,15 +180,15 @@
         for child in root:
             if child.tag.endswith("components"):
                 for ele in child.iter():
                     if ele.tag.endswith("component"):
                         licenses = get_licenses(ele)
                         pkgs.append(get_package(ele, licenses))
     except Exception as pe:
-        LOG.debug("Unable to parse {} {}".format(xmlfile, pe))
+        LOG.debug("Unable to parse %s %s", xmlfile, pe)
         LOG.warning(
             "Unable to produce Software Bill-of-Materials for this project. Execute the scan after installing the dependencies!"
         )
     return pkgs
 
 
 def get_pkg_by_type(pkg_list, pkg_type):
@@ -227,15 +227,15 @@
         # Fallback to universal if no project type was provided
         if not project_type:
             project_type = "universal"
         if not src_dir and options.get("path"):
             src_dir = options.get("path")
         with httpx.Client(http2=True, base_url=cdxgen_server, timeout=180) as client:
             sbom_url = f"{cdxgen_server}/sbom"
-            LOG.debug(f"Invoking cdxgen server at {sbom_url}")
+            LOG.debug("Invoking cdxgen server at %s", sbom_url)
             try:
                 r = client.post(
                     sbom_url,
                     json={
                         "url": options.get("url", ""),
                         "path": options.get("path", src_dir),
                         "type": options.get("type", project_type),
@@ -243,25 +243,26 @@
                     },
                     headers=headers,
                 )
                 if r.status_code == httpx.codes.OK:
                     try:
                         json_response = r.json()
                         if json_response:
-                            with open(bom_file, mode="w") as fp:
+                            with open(bom_file, mode="w", encoding="utf-8") as fp:
                                 json.dump(json_response, fp)
                             return os.path.exists(bom_file)
                     except Exception as je:
                         LOG.error(je)
                         LOG.info(
                             "Unable to generate SBoM with cdxgen server. Trying to generate one locally."
                         )
                 else:
-                    LOG.warn(
-                        f"Unable to generate SBoM via cdxgen server due to {r.status_code}"
+                    LOG.warning(
+                        "Unable to generate SBoM via cdxgen server due to %s",
+                        r.status_code,
                     )
             except Exception as e:
                 LOG.error(e)
                 LOG.info(
                     "Unable to generate SBoM with cdxgen server. Trying to generate one locally."
                 )
     cdxgen_cmd = os.environ.get("CDXGEN_CMD", "cdxgen")
@@ -269,80 +270,86 @@
         local_bin = resource_path(
             os.path.join(
                 "local_bin", "cdxgen.exe" if sys.platform == "win32" else "cdxgen"
             )
         )
         if not os.path.exists(local_bin):
             LOG.warning(
-                "{} command not found. Please install using npm install @cyclonedx/cdxgen or set PATH variable".format(
-                    cdxgen_cmd
-                )
+                "%s command not found. Please install using npm install @cyclonedx/cdxgen or set PATH variable",
+                cdxgen_cmd,
             )
             return False
         try:
             cdxgen_cmd = local_bin
             # Set the plugins directory as an environment variable
             os.environ["CDXGEN_PLUGINS_DIR"] = resource_path("local_bin")
         except Exception:
             pass
-    if project_type in ("docker"):
+    if project_type in ("docker",):
         LOG.info(
-            f"Generating Software Bill-of-Materials for container image {src_dir}. This might take a few mins ..."
+            "Generating Software Bill-of-Materials for container image %s. This might take a few mins ...",
+            src_dir,
         )
     args = [cdxgen_cmd, "-r", "-t", project_type, "-o", bom_file]
     if deep or project_type in ("jar", "jenkins"):
         args.append("--deep")
         LOG.info("About to perform deep scan. This would take a while ...")
     args.append(src_dir)
     exec_tool(args)
     return os.path.exists(bom_file)
 
 
 def submit_bom(reports_dir, threatdb_params):
+    """Method to submit the SBoM to threatdb for analysis"""
     vex_files = find_files(reports_dir, ".vex.json", quick=False, filter=True)
     if vex_files:
         threatdb_server = threatdb_params["threatdb_server"]
         if not threatdb_server.endswith("/import"):
             threatdb_server = f"{threatdb_server}/import"
         login_url = threatdb_server.replace("/import", "/login")
         with httpx.Client(http2=True, base_url=threatdb_server, timeout=180) as client:
             token = threatdb_params.get("threatdb_token")
             if not token:
-                LOG.debug(f"Attempting to retrieve access token from {login_url}")
+                LOG.debug("Attempting to retrieve access token from %s", login_url)
                 r = client.post(
                     login_url,
                     json={
                         "username": threatdb_params["threatdb_username"],
                         "password": threatdb_params["threatdb_password"],
                     },
                     headers=headers,
                 )
                 if r.status_code == httpx.codes.OK:
                     json_response = r.json()
                     if json_response and json_response.get("access_token"):
                         token = json_response.get("access_token")
                 else:
-                    LOG.warn(
-                        f"Unable to retrieve access token from {login_url} due to {r.status_code}"
+                    LOG.warning(
+                        "Unable to retrieve access token from %s due to %s",
+                        login_url,
+                        r.status_code,
                     )
             if token:
                 for vf in vex_files:
                     files = {"file": open(vf, "rb")}
                     r = client.post(
                         threatdb_server,
                         files=files,
                         headers={"Authorization": f"Bearer {token}"},
                     )
                     if r.status_code == httpx.codes.OK:
                         json_response = r.json()
                         if not json_response.get("success"):
                             LOG.debug(
-                                f"Uploaded file {vf} was not processed successfully"
+                                "Uploaded file %s was not processed successfully", vf
                             )
                         else:
                             LOG.debug(
-                                f"Vex file {vf} was submitted successfully to the threatdb server"
+                                "Vex file %s was submitted successfully to the threatdb server",
+                                vf,
                             )
                     else:
-                        LOG.warn(
-                            f"Unable to submit vex file to {threatdb_server} due to {r.status_code}"
+                        LOG.warning(
+                            "Unable to submit vex file to %s due to %s",
+                            threatdb_server,
+                            r.status_code,
                         )
```

### Comparing `appthreat-depscan-4.1.2/depscan/lib/config.py` & `appthreat-depscan-4.2.0/depscan/lib/config.py`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/depscan/lib/license.py` & `appthreat-depscan-4.2.0/depscan/lib/license.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 
 from depscan.lib.utils import find_files
 
 
 def build_license_data(license_dir, spdx_license_list):
     """Build license data based on the txt files"""
     licenses_dict = {}
-    with open(spdx_license_list) as fp:
+    with open(spdx_license_list, encoding="utf-8") as fp:
         spdx_license_data = json.load(fp)
         for slic in spdx_license_data.get("licenses"):
             licenses_dict[slic["licenseId"]] = {
                 "title": slic["name"],
                 "spdx-id": slic["licenseId"],
                 "osi_approved": slic.get("isOsiApproved"),
                 "fsf_libre": slic.get("isFsfLibre"),
                 "conditions": [f"See {slic['detailsUrl']}"],
                 "condition_flag": not slic.get("isOsiApproved"),
             }
     license_files = find_files(license_dir, "txt")
     for lfile in license_files:
-        with open(lfile) as fp:
+        with open(lfile, encoding="utf-8") as fp:
             raw_data = fp.read().split("---")[1]
             ldata = yaml.safe_load(raw_data)
             ldata["condition_flag"] = False
             for cond in ldata["conditions"]:
                 if cond in [
                     "document-changes",
                     "network-use-disclose",
```

### Comparing `appthreat-depscan-4.1.2/depscan/lib/logger.py` & `appthreat-depscan-4.2.0/depscan/lib/logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 import logging
 import os
 
 from rich.console import Console
 from rich.logging import RichHandler
 from rich.theme import Theme
 
-custom_theme = Theme({"info": "cyan", "warning": "purple4", "danger": "bold red"})
+custom_theme = Theme({"info": "#5A7C90", "warning": "#FF753D", "danger": "bold red"})
 console = Console(
     log_time=False,
     log_path=False,
     theme=custom_theme,
-    width=int(os.getenv("COLUMNS", 270)),
+    width=int(os.getenv("COLUMNS", "270")),
     color_system="256",
     force_terminal=True,
     record=True,
 )
 
 logging.basicConfig(
     level=logging.INFO,
```

### Comparing `appthreat-depscan-4.1.2/depscan/lib/normalize.py` & `appthreat-depscan-4.2.0/depscan/lib/normalize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from vdb.lib import KNOWN_PKG_TYPES
 from vdb.lib.config import placeholder_exclude_version
 from vdb.lib.utils import parse_purl
 
-from depscan.lib import config as config
+from depscan.lib import config
 
 # Common package suffixes
 COMMON_SUFFIXES = [
     "-core",
     ".core",
     "-client-core",
     "-classic",
@@ -154,15 +154,15 @@
     if pkg_type in config.OS_PKG_TYPES:
         if "lib" in name:
             name_aliases.add(name.replace("lib", ""))
         elif "lib" not in name:
             name_aliases.add("lib" + name)
         if "-bin" not in name:
             name_aliases.add(name + "-bin")
-    if len(vendor_aliases):
+    if len(vendor_aliases) > 0:
         for vvar in list(vendor_aliases):
             for nvar in list(name_aliases):
                 pkg_list.append({**pkg_dict, "vendor": vvar, "name": nvar})
     else:
         for nvar in list(name_aliases):
             pkg_list.append({**pkg_dict, "name": nvar})
     return pkg_list
@@ -180,18 +180,15 @@
     if not pkg_aliases:
         return {}
     dealias_dict = {}
     for res in pkg_list:
         package_issue = res.package_issue
         full_pkg = package_issue.affected_location.package
         if package_issue.affected_location.vendor:
-            full_pkg = "{}:{}".format(
-                package_issue.affected_location.vendor,
-                package_issue.affected_location.package,
-            )
+            full_pkg = f"{package_issue.affected_location.vendor}:{package_issue.affected_location.package}"
         if purl_aliases.get(full_pkg.lower()):
             dealias_dict[full_pkg] = purl_aliases.get(full_pkg.lower())
         else:
             for k, v in pkg_aliases.items():
                 if (
                     full_pkg in v
                     or (":" + package_issue.affected_location.package) in v
```

### Comparing `appthreat-depscan-4.1.2/depscan/lib/pkg_query.py` & `appthreat-depscan-4.2.0/depscan/lib/pkg_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math
 from datetime import datetime
 
 import httpx
 from rich.progress import Progress
 
-from depscan.lib import config as config
+from depscan.lib import config
 from depscan.lib.logger import LOG, console
 
 
 def get_lookup_url(registry_type, pkg):
     vendor = None
     if isinstance(pkg, dict):
         vendor = pkg.get("vendor")
@@ -92,15 +92,15 @@
                         ):
                             is_private_pkg = True
                             break
                 risk_metrics = {}
                 if registry_type == "npm":
                     risk_metrics = npm_pkg_risk(json_data, is_private_pkg, scope)
                 elif registry_type == "pypi":
-                    project_type_pkg = "{}:{}".format("python", key).lower()
+                    project_type_pkg = f"python:{key}".lower()
                     required_pkgs = scoped_pkgs.get("required", [])
                     optional_pkgs = scoped_pkgs.get("optional", [])
                     excluded_pkgs = scoped_pkgs.get("excluded", [])
                     if project_type_pkg in required_pkgs:
                         scope = "required"
                     elif project_type_pkg in optional_pkgs:
                         scope = "optional"
@@ -117,15 +117,18 @@
                 LOG.debug(e)
                 failure_count = failure_count + 1
             progress.advance(task)
             done_count = done_count + 1
             if failure_count >= config.max_request_failures:
                 circuit_breaker = True
     LOG.debug(
-        f"Retrieved package metadata for {done_count}/{len(pkg_list)} packages. Failures count {failure_count}"
+        "Retrieved package metadata for %d/%d packages. Failures count %d",
+        done_count,
+        len(pkg_list),
+        failure_count,
     )
     return metadata_dict
 
 
 def npm_metadata(scoped_pkgs, pkg_list, private_ns=None):
     """
     Method to query npm for the package metadata
```

### Comparing `appthreat-depscan-4.1.2/depscan/lib/privado.py` & `appthreat-depscan-4.2.0/depscan/lib/privado.py`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/depscan/lib/utils.py` & `appthreat-depscan-4.2.0/depscan/lib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import os
 import re
 from collections import defaultdict
 
 from vdb.lib import db as dbLib
 from vdb.lib.utils import version_compare
 
-from depscan.lib import config as config
-from depscan.lib import normalize as normalize
+from depscan.lib import config
+from depscan.lib import normalize
 
 lic_symbol_regex = re.compile(r"[\(\)\,]")
 
 
 def filter_ignored_dirs(dirs):
     """
     Method to filter directory list to remove ignored directories
@@ -38,14 +38,15 @@
     result = []
     req_files = [
         "requirements.txt",
         "Pipfile",
         "poetry.lock",
         "Pipfile.lock",
         "conda.yml",
+        "pyproject.toml",
     ]
     for root, dirs, files in os.walk(path):
         filter_ignored_dirs(dirs)
         for name in req_files:
             if name in files:
                 result.append(os.path.join(root, name))
     return result
@@ -105,15 +106,15 @@
         or src_dir.endswith(".tar.gz")
     ):
         return ["docker"]
     # Check if the source is an exe file. Assume go for all binaries for now
     if is_exe(src_dir):
         return ["go", "binary"]
     project_types = []
-    if find_python_reqfiles(src_dir):
+    if find_python_reqfiles(src_dir) or find_files(src_dir, ".py", quick=True):
         project_types.append("python")
     if find_files(src_dir, "pom.xml", quick=True) or find_files(
         src_dir, ".gradle", quick=True
     ):
         project_types.append("java")
     if find_files(src_dir, ".gradle.kts", quick=True):
         project_types.append("kotlin")
@@ -209,15 +210,15 @@
             expanded_list += variations
         vendor, name = get_pkg_vendor_name(pkg)
         version = pkg.get("version")
         purl_aliases[f"{vendor.lower()}:{name.lower()}"] = pkg.get("purl")
         purl_aliases[f"{vendor.lower()}:{name.lower()}:{version}"] = pkg.get("purl")
         if variations:
             for vari in variations:
-                vari_full_pkg = "{}:{}".format(vari.get("vendor"), vari.get("name"))
+                vari_full_pkg = f"""{vari.get("vendor")}:{vari.get("name")}"""
                 pkg_aliases[vendor.lower() + ":" + name.lower()].append(vari_full_pkg)
                 purl_aliases[f"{vari_full_pkg.lower()}"] = pkg.get("purl")
                 purl_aliases[f"{vari_full_pkg.lower()}:{version}"] = pkg.get("purl")
     quick_res = dbLib.bulk_index_search(expanded_list)
     raw_results = dbLib.pkg_bulk_search(db, quick_res)
     raw_results = normalize.dedup(project_type, raw_results, pkg_aliases=pkg_aliases)
     pkg_aliases = normalize.dealias_packages(
@@ -291,30 +292,32 @@
         return version_list
     if isinstance(version_list, set):
         version_list = list(version_list)
     if len(version_list) == 1:
         return version_list[0]
     min_ver = "0"
     max_ver = version_list[0]
-    for i in range(len(version_list)):
-        if not version_list[i]:
+    for i, vl in enumerate(version_list):
+        if not vl:
             continue
-        if not version_compare(version_list[i], min_ver, max_ver):
-            max_ver = version_list[i]
+        if not version_compare(vl, min_ver, max_ver):
+            max_ver = vl
     return max_ver
 
 
 def get_all_imports(src_dir):
-    """Method to collect all package imports from a python file"""
+    """Method to collect all package imports from a python file
+    No longer required since cdxgen does python analysis already
+    """
     import_list = set()
     py_files = find_files(src_dir, ".py", quick=False)
     if not py_files:
         return import_list
     for afile in py_files:
-        with open(os.path.join(afile), "rb") as f:
+        with open(os.path.join(afile), "rb", encoding="utf-8") as f:
             content = f.read()
         parsed = ast.parse(content)
         for node in ast.walk(parsed):
             if isinstance(node, ast.Import):
                 for name in node.names:
                     pkg = name.name.split(".")[0]
                     import_list.add(pkg)
```

### Comparing `appthreat-depscan-4.1.2/setup.py` & `appthreat-depscan-4.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,56 @@
-import setuptools
+[project]
+name = "appthreat-depscan"
+version = "4.2.0"
+description = "Fully open-source security audit for project dependencies based on known vulnerabilities and advisories."
+authors = [
+    {name = "Team AppThreat", email = "cloud@appthreat.com"},
+]
+dependencies = [
+    "appthreat-vulnerability-db>=5.2.0",
+    "defusedxml",
+    "PyYAML",
+    "rich",
+    "quart",
+]
 
-with open("README.md", "r") as fh:
-    long_description = fh.read()
+requires-python = ">=3.8"
+readme = "README.md"
+license = {text = "MIT"}
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "Intended Audience :: System Administrators",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Security",
+    "Topic :: Utilities",
+]
 
-setuptools.setup(
-    name="appthreat-depscan",
-    version="4.1.2",
-    author="Team AppThreat",
-    author_email="cloud@appthreat.com",
-    description="Fully open-source security audit for project dependencies based on known vulnerabilities and advisories.",
-    entry_points={
-        "console_scripts": ["scan=depscan.cli:main", "depscan=depscan.cli:main"]
-    },
-    license="MIT",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/appthreat/dep-scan",
-    packages=["depscan", "depscan.lib", "vendor"],
-    include_package_data=True,
-    install_requires=[
-        "appthreat-vulnerability-db>=5.1.3",
-        "defusedxml",
-        "PyYAML",
-        "rich",
-        "quart",
-    ],
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "Intended Audience :: System Administrators",
-        "Topic :: Utilities",
-        "Topic :: Security",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    python_requires=">=3.8",
-)
+[project.urls]
+Homepage = "https://github.com/appthreat/dep-scan"
+
+[project.scripts]
+depscan = "depscan.cli:main"
+scan = "depscan.cli:main"
+
+[project.optional-dependencies]
+dev = ["black",
+"flake8",
+"pytest",
+"pytest-cov"
+]
+
+[build-system]
+requires = ["setuptools>=61", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools]
+include-package-data = true
+packages = ["depscan", "depscan.lib", "vendor"]
+
+[tool.pytest.ini_options]
+addopts = "--verbose --cov-append --cov-report term --cov depscan"
```

### Comparing `appthreat-depscan-4.1.2/test/test_bom.py` & `appthreat-depscan-4.2.0/test/test_bom.py`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/test/test_license.py` & `appthreat-depscan-4.2.0/test/test_license.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 import pytest
 
 from depscan.lib.bom import get_pkg_list
 from depscan.lib.license import build_license_data, bulk_lookup
-from depscan.lib import analysis as analysis
+from depscan.lib import analysis
 
 
 @pytest.fixture
 def test_license_data():
     licenses_dir = os.path.join(
         os.path.dirname(os.path.realpath(__file__)),
         "..",
```

### Comparing `appthreat-depscan-4.1.2/test/test_norm.py` & `appthreat-depscan-4.2.0/test/test_norm.py`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/test/test_pkg_query.py` & `appthreat-depscan-4.2.0/test/test_pkg_query.py`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/test/test_utils.py` & `appthreat-depscan-4.2.0/test/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from depscan.lib import utils as utils
+from depscan.lib import utils
 
 
 def test_cleanup_license_string():
     data = utils.cleanup_license_string("MIT")
     assert data == "MIT"
     data = utils.cleanup_license_string("MIT/GPL-3.0")
     assert data == "MIT OR GPL-3.0"
```

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_data/fields.yml` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_data/fields.yml`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_data/meta.yml` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_data/meta.yml`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_data/rules.yml` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_data/rules.yml`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/0bsd.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/0bsd.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/afl-3.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/afl-3.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/agpl-3.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/apache-2.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/artistic-2.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/artistic-2.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/bsd-2-clause.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/bsd-2-clause.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/bsd-3-clause.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/bsd-3-clause.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ---
 title: BSD 3-Clause "New" or "Revised" License
 spdx-id: BSD-3-Clause
+nickname: Modified BSD License
 hidden: false
 
 description: A permissive license similar to the <a href="/licenses/bsd-2-clause/">BSD 2-Clause License</a>, but with a 3rd clause that prohibits others from using the name of the copyright holder or its contributors to promote derived products without written consent.
 
 how: Create a text file (typically named LICENSE or LICENSE.txt) in the root of your source code and copy the text of the license into the file. Replace [year] with the current year and [fullname] with the name (or names) of the copyright holders.
 
 using:
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
 --- title: BSD 3-Clause "New" or "Revised" License spdx-id: BSD-3-Clause
-hidden: false description: A permissive license similar to the BSD_2-Clause
-License, but with a 3rd clause that prohibits others from using the name of the
-copyright holder or its contributors to promote derived products without
-written consent. how: Create a text file (typically named LICENSE or
-LICENSE.txt) in the root of your source code and copy the text of the license
-into the file. Replace [year] with the current year and [fullname] with the
-name (or names) of the copyright holders. using: Flutter: https://github.com/
-flutter/flutter/blob/master/LICENSE LevelDB: https://github.com/google/leveldb/
-blob/master/LICENSE Quill: https://github.com/quilljs/quill/blob/develop/
-LICENSE permissions: - commercial-use - modifications - distribution - private-
-use conditions: - include-copyright limitations: - liability - warranty --- BSD
-3-Clause License Copyright (c) [year], [fullname] Redistribution and use in
-source and binary forms, with or without modification, are permitted provided
-that the following conditions are met: 1. Redistributions of source code must
-retain the above copyright notice, this list of conditions and the following
-disclaimer. 2. Redistributions in binary form must reproduce the above
-copyright notice, this list of conditions and the following disclaimer in the
-documentation and/or other materials provided with the distribution. 3. Neither
-the name of the copyright holder nor the names of its contributors may be used
-to endorse or promote products derived from this software without specific
-prior written permission. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS
-AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT
-NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
-PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
-CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
-EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT
-OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
-INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
-CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING
-IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY
-OF SUCH DAMAGE.
+nickname: Modified BSD License hidden: false description: A permissive license
+similar to the BSD_2-Clause_License, but with a 3rd clause that prohibits
+others from using the name of the copyright holder or its contributors to
+promote derived products without written consent. how: Create a text file
+(typically named LICENSE or LICENSE.txt) in the root of your source code and
+copy the text of the license into the file. Replace [year] with the current
+year and [fullname] with the name (or names) of the copyright holders. using:
+Flutter: https://github.com/flutter/flutter/blob/master/LICENSE LevelDB: https:
+//github.com/google/leveldb/blob/master/LICENSE Quill: https://github.com/
+quilljs/quill/blob/develop/LICENSE permissions: - commercial-use -
+modifications - distribution - private-use conditions: - include-copyright
+limitations: - liability - warranty --- BSD 3-Clause License Copyright (c)
+[year], [fullname] Redistribution and use in source and binary forms, with or
+without modification, are permitted provided that the following conditions are
+met: 1. Redistributions of source code must retain the above copyright notice,
+this list of conditions and the following disclaimer. 2. Redistributions in
+binary form must reproduce the above copyright notice, this list of conditions
+and the following disclaimer in the documentation and/or other materials
+provided with the distribution. 3. Neither the name of the copyright holder nor
+the names of its contributors may be used to endorse or promote products
+derived from this software without specific prior written permission. THIS
+SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY
+EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/bsd-4-clause.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/bsd-4-clause.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/bsl-1.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/bsl-1.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/cc-by-4.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/cc-by-4.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/cc0-1.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/cc0-1.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/cecill-2.1.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/cecill-2.1.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/ecl-2.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/ecl-2.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/epl-1.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/epl-1.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/epl-2.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/epl-2.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/eupl-1.1.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/eupl-1.1.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/eupl-1.2.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/eupl-1.2.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/gfdl-1.3.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/gfdl-1.3.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/gpl-2.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/gpl-3.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/gpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/isc.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/isc.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/lgpl-2.1.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/lgpl-2.1.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/lgpl-3.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/lgpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/lppl-1.3c.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/lppl-1.3c.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/mit-0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/mit-0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/mit.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/mit.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/mpl-2.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/mpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/ms-pl.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/ms-pl.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/ms-rl.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/ms-rl.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/ncsa.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/ncsa.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/odbl-1.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/odbl-1.0.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 description: The Open Database License (ODbL) is a license agreement intended to allow users to freely share, modify, and use a database while maintaining this same freedom for others.
 
 how: Create a text file (typically named LICENSE or LICENSE.txt) in the root of your source code and copy the text of the license into the file.
 
 using:
   World Countries: https://github.com/mledoze/countries/blob/master/LICENSE
   OpenFlights: https://github.com/jpatokal/openflights/blob/master/data/LICENSE
-  Public Zone Database: https://github.com/zonedb/zonedb/blob/main/LICENSE.md
+  Public Zone Database: https://github.com/zonedb/zonedb/blob/main/LICENSE-DATA.md
 
 permissions:
   - commercial-use
   - distribution
   - modifications
   - private-use
```

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/ofl-1.1.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/ofl-1.1.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/osl-3.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/osl-3.0.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/postgresql.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/postgresql.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/unlicense.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/unlicense.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/upl-1.0.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/upl-1.0.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 description: A permissive, OSI and FSF approved, GPL compatible license, expressly allowing attribution with just a copyright notice and a short form link rather than the full text of the license.  Includes an express grant of patent rights.  Licensed works and modifications may be distributed under different terms and without source code, and the patent grant may also optionally be expanded to larger works to permit use as a contributor license agreement.
 
 how: Insert the license or a link to it along with a copyright notice into your source file(s), and/or create a text file (typically named LICENSE or LICENSE.txt) in the root of your source code and copy the text of the license into the file, replacing [year] with the current year and [fullname] with the name (or names) of the copyright holders.
 
 note: It is recommended to add a link to the license and copyright notice at the top of each source file, example text can be found at https://oss.oracle.com/licenses/upl/.
 
 using:
-  Oracle Product Images for Docker: https://github.com/oracle/docker-images/blob/main/LICENSE.txt
-  Skater: https://github.com/oracle/Skater/blob/master/LICENSE
+  Roc: https://github.com/roc-lang/roc/blob/main/LICENSE
+  Skater: https://github.com/oracle/skater/blob/main/LICENSE.txt
   Soufflé: https://github.com/souffle-lang/souffle/blob/master/LICENSE
 
 permissions:
   - commercial-use
   - modifications
   - distribution
   - patent-use
@@ -39,15 +39,15 @@
 rights in the Software, and any and all patent rights owned or freely
 licensable by each licensor hereunder covering either (i) the unmodified
 Software as contributed to or provided by such licensor, or (ii) the Larger
 Works (as defined below), to deal in both
 
 (a) the Software, and
 (b) any piece of software and/or hardware listed in the lrgrwrks.txt file if
-one is included with the Software (each a “Larger Work” to which the Software
+one is included with the Software (each a "Larger Work" to which the Software
 is contributed by such licensors),
 
 without restriction, including without limitation the rights to copy, create
 derivative works of, display, perform, and distribute the Software and make,
 use, sell, offer for sale, import, export, have made, and have sold the
 Software and the Larger Work(s), and to sublicense the foregoing rights on
 either these or other terms.
```

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/vim.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/vim.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/wtfpl.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/wtfpl.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/choosealicense.com/_licenses/zlib.txt` & `appthreat-depscan-4.2.0/vendor/choosealicense.com/_licenses/zlib.txt`

 * *Files identical despite different names*

### Comparing `appthreat-depscan-4.1.2/vendor/spdx/json/licenses.json` & `appthreat-depscan-4.2.0/vendor/spdx/json/licenses.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6404805838154136%*

 * *Differences: {"'licenseListVersion'": "'84728b7'",*

 * * "'licenses'": "{0: {'referenceNumber': 534}, 1: {'referenceNumber': 152}, 2: {'referenceNumber': "*

 * *               "149}, 4: {'referenceNumber': 106}, 5: {'referenceNumber': 83}, 6: "*

 * *               "{'referenceNumber': 70}, 7: {'referenceNumber': 465}, 8: {'referenceNumber': 310}, "*

 * *               "9: {'referenceNumber': 154}, 10: {'referenceNumber': 309}, 11: {'referenceNumber': "*

 * *               "502}, 12: {'referenceNumber': 111}, 13: {'referenceNumber': 257}, 14: "*

 * * […]*

```diff
@@ -1,2063 +1,2263 @@
 {
-    "licenseListVersion": "ce34329",
+    "licenseListVersion": "84728b7",
     "licenses": [
         {
             "detailsUrl": "https://spdx.org/licenses/0BSD.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "0BSD",
             "name": "BSD Zero Clause License",
             "reference": "https://spdx.org/licenses/0BSD.html",
-            "referenceNumber": 432,
+            "referenceNumber": 534,
             "seeAlso": [
                 "http://landley.net/toybox/license.html",
                 "https://opensource.org/licenses/0BSD"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AAL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "AAL",
             "name": "Attribution Assurance License",
             "reference": "https://spdx.org/licenses/AAL.html",
-            "referenceNumber": 246,
+            "referenceNumber": 152,
             "seeAlso": [
                 "https://opensource.org/licenses/attribution"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Abstyles.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Abstyles",
             "name": "Abstyles License",
             "reference": "https://spdx.org/licenses/Abstyles.html",
-            "referenceNumber": 341,
+            "referenceNumber": 149,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Abstyles"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/AdaCore-doc.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "AdaCore-doc",
+            "name": "AdaCore Doc License",
+            "reference": "https://spdx.org/licenses/AdaCore-doc.html",
+            "referenceNumber": 397,
+            "seeAlso": [
+                "https://github.com/AdaCore/xmlada/blob/master/docs/index.rst",
+                "https://github.com/AdaCore/gnatcoll-core/blob/master/docs/index.rst",
+                "https://github.com/AdaCore/gnatcoll-db/blob/master/docs/index.rst"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Adobe-2006.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Adobe-2006",
             "name": "Adobe Systems Incorporated Source Code License Agreement",
             "reference": "https://spdx.org/licenses/Adobe-2006.html",
-            "referenceNumber": 48,
+            "referenceNumber": 106,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/AdobeLicense"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Adobe-Glyph.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Adobe-Glyph",
             "name": "Adobe Glyph List License",
             "reference": "https://spdx.org/licenses/Adobe-Glyph.html",
-            "referenceNumber": 283,
+            "referenceNumber": 83,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/MIT#AdobeGlyph"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ADSL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "ADSL",
             "name": "Amazon Digital Services License",
             "reference": "https://spdx.org/licenses/ADSL.html",
-            "referenceNumber": 117,
+            "referenceNumber": 70,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/AmazonDigitalServicesLicense"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AFL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "AFL-1.1",
             "name": "Academic Free License v1.1",
             "reference": "https://spdx.org/licenses/AFL-1.1.html",
-            "referenceNumber": 390,
+            "referenceNumber": 465,
             "seeAlso": [
                 "http://opensource.linux-mirror.org/licenses/afl-1.1.txt",
                 "http://wayback.archive.org/web/20021004124254/http://www.opensource.org/licenses/academic.php"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AFL-1.2.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "AFL-1.2",
             "name": "Academic Free License v1.2",
             "reference": "https://spdx.org/licenses/AFL-1.2.html",
-            "referenceNumber": 471,
+            "referenceNumber": 310,
             "seeAlso": [
                 "http://opensource.linux-mirror.org/licenses/afl-1.2.txt",
                 "http://wayback.archive.org/web/20021204204652/http://www.opensource.org/licenses/academic.php"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AFL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "AFL-2.0",
             "name": "Academic Free License v2.0",
             "reference": "https://spdx.org/licenses/AFL-2.0.html",
-            "referenceNumber": 282,
+            "referenceNumber": 154,
             "seeAlso": [
                 "http://wayback.archive.org/web/20060924134533/http://www.opensource.org/licenses/afl-2.0.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AFL-2.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "AFL-2.1",
             "name": "Academic Free License v2.1",
             "reference": "https://spdx.org/licenses/AFL-2.1.html",
-            "referenceNumber": 46,
+            "referenceNumber": 309,
             "seeAlso": [
                 "http://opensource.linux-mirror.org/licenses/afl-2.1.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AFL-3.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "AFL-3.0",
             "name": "Academic Free License v3.0",
             "reference": "https://spdx.org/licenses/AFL-3.0.html",
-            "referenceNumber": 181,
+            "referenceNumber": 502,
             "seeAlso": [
                 "http://www.rosenlaw.com/AFL3.0.htm",
                 "https://opensource.org/licenses/afl-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Afmparse.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Afmparse",
             "name": "Afmparse License",
             "reference": "https://spdx.org/licenses/Afmparse.html",
-            "referenceNumber": 155,
+            "referenceNumber": 111,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Afmparse"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AGPL-1.0.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "AGPL-1.0",
             "name": "Affero General Public License v1.0",
             "reference": "https://spdx.org/licenses/AGPL-1.0.html",
-            "referenceNumber": 299,
+            "referenceNumber": 257,
             "seeAlso": [
                 "http://www.affero.org/oagpl.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AGPL-1.0-only.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "AGPL-1.0-only",
             "name": "Affero General Public License v1.0 only",
             "reference": "https://spdx.org/licenses/AGPL-1.0-only.html",
-            "referenceNumber": 411,
+            "referenceNumber": 389,
             "seeAlso": [
                 "http://www.affero.org/oagpl.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AGPL-1.0-or-later.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "AGPL-1.0-or-later",
             "name": "Affero General Public License v1.0 or later",
             "reference": "https://spdx.org/licenses/AGPL-1.0-or-later.html",
-            "referenceNumber": 225,
+            "referenceNumber": 34,
             "seeAlso": [
                 "http://www.affero.org/oagpl.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AGPL-3.0.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "AGPL-3.0",
             "name": "GNU Affero General Public License v3.0",
             "reference": "https://spdx.org/licenses/AGPL-3.0.html",
-            "referenceNumber": 136,
+            "referenceNumber": 292,
             "seeAlso": [
                 "https://www.gnu.org/licenses/agpl.txt",
                 "https://opensource.org/licenses/AGPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AGPL-3.0-only.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "AGPL-3.0-only",
             "name": "GNU Affero General Public License v3.0 only",
             "reference": "https://spdx.org/licenses/AGPL-3.0-only.html",
-            "referenceNumber": 113,
+            "referenceNumber": 33,
             "seeAlso": [
                 "https://www.gnu.org/licenses/agpl.txt",
                 "https://opensource.org/licenses/AGPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AGPL-3.0-or-later.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "AGPL-3.0-or-later",
             "name": "GNU Affero General Public License v3.0 or later",
             "reference": "https://spdx.org/licenses/AGPL-3.0-or-later.html",
-            "referenceNumber": 383,
+            "referenceNumber": 217,
             "seeAlso": [
                 "https://www.gnu.org/licenses/agpl.txt",
                 "https://opensource.org/licenses/AGPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Aladdin.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "Aladdin",
             "name": "Aladdin Free Public License",
             "reference": "https://spdx.org/licenses/Aladdin.html",
-            "referenceNumber": 68,
+            "referenceNumber": 63,
             "seeAlso": [
                 "http://pages.cs.wisc.edu/~ghost/doc/AFPL/6.01/Public.htm"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AMDPLPA.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "AMDPLPA",
             "name": "AMD's plpa_map.c License",
             "reference": "https://spdx.org/licenses/AMDPLPA.html",
-            "referenceNumber": 51,
+            "referenceNumber": 386,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/AMD_plpa_map_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AML.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "AML",
             "name": "Apple MIT License",
             "reference": "https://spdx.org/licenses/AML.html",
-            "referenceNumber": 489,
+            "referenceNumber": 147,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Apple_MIT_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AMPAS.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "AMPAS",
             "name": "Academy of Motion Picture Arts and Sciences BSD",
             "reference": "https://spdx.org/licenses/AMPAS.html",
-            "referenceNumber": 114,
+            "referenceNumber": 90,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/BSD#AMPASBSD"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ANTLR-PD.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "ANTLR-PD",
             "name": "ANTLR Software Rights Notice",
             "reference": "https://spdx.org/licenses/ANTLR-PD.html",
-            "referenceNumber": 236,
+            "referenceNumber": 448,
             "seeAlso": [
                 "http://www.antlr2.org/license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ANTLR-PD-fallback.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "ANTLR-PD-fallback",
             "name": "ANTLR Software Rights Notice with license fallback",
             "reference": "https://spdx.org/licenses/ANTLR-PD-fallback.html",
-            "referenceNumber": 329,
+            "referenceNumber": 207,
             "seeAlso": [
                 "http://www.antlr2.org/license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Apache-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "Apache-1.0",
             "name": "Apache License 1.0",
             "reference": "https://spdx.org/licenses/Apache-1.0.html",
-            "referenceNumber": 313,
+            "referenceNumber": 434,
             "seeAlso": [
                 "http://www.apache.org/licenses/LICENSE-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Apache-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "Apache-1.1",
             "name": "Apache License 1.1",
             "reference": "https://spdx.org/licenses/Apache-1.1.html",
-            "referenceNumber": 310,
+            "referenceNumber": 524,
             "seeAlso": [
                 "http://apache.org/licenses/LICENSE-1.1",
                 "https://opensource.org/licenses/Apache-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Apache-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "Apache-2.0",
             "name": "Apache License 2.0",
             "reference": "https://spdx.org/licenses/Apache-2.0.html",
-            "referenceNumber": 119,
+            "referenceNumber": 263,
             "seeAlso": [
                 "https://www.apache.org/licenses/LICENSE-2.0",
                 "https://opensource.org/licenses/Apache-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/APAFML.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "APAFML",
             "name": "Adobe Postscript AFM License",
             "reference": "https://spdx.org/licenses/APAFML.html",
-            "referenceNumber": 337,
+            "referenceNumber": 189,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/AdobePostscriptAFM"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/APL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "APL-1.0",
             "name": "Adaptive Public License 1.0",
             "reference": "https://spdx.org/licenses/APL-1.0.html",
-            "referenceNumber": 365,
+            "referenceNumber": 410,
             "seeAlso": [
                 "https://opensource.org/licenses/APL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/App-s2p.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "App-s2p",
             "name": "App::s2p License",
             "reference": "https://spdx.org/licenses/App-s2p.html",
-            "referenceNumber": 245,
+            "referenceNumber": 148,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/App-s2p"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/APSL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": true,
             "licenseId": "APSL-1.0",
             "name": "Apple Public Source License 1.0",
             "reference": "https://spdx.org/licenses/APSL-1.0.html",
-            "referenceNumber": 124,
+            "referenceNumber": 177,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Apple_Public_Source_License_1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/APSL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "APSL-1.1",
             "name": "Apple Public Source License 1.1",
             "reference": "https://spdx.org/licenses/APSL-1.1.html",
-            "referenceNumber": 259,
+            "referenceNumber": 537,
             "seeAlso": [
                 "http://www.opensource.apple.com/source/IOSerialFamily/IOSerialFamily-7/APPLE_LICENSE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/APSL-1.2.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "APSL-1.2",
             "name": "Apple Public Source License 1.2",
             "reference": "https://spdx.org/licenses/APSL-1.2.html",
-            "referenceNumber": 120,
+            "referenceNumber": 479,
             "seeAlso": [
                 "http://www.samurajdata.se/opensource/mirror/licenses/apsl.php"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/APSL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "APSL-2.0",
             "name": "Apple Public Source License 2.0",
             "reference": "https://spdx.org/licenses/APSL-2.0.html",
-            "referenceNumber": 391,
+            "referenceNumber": 183,
             "seeAlso": [
                 "http://www.opensource.apple.com/license/apsl/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Arphic-1999.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Arphic-1999",
             "name": "Arphic Public License",
             "reference": "https://spdx.org/licenses/Arphic-1999.html",
-            "referenceNumber": 445,
+            "referenceNumber": 78,
             "seeAlso": [
                 "http://ftp.gnu.org/gnu/non-gnu/chinese-fonts-truetype/LICENSE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Artistic-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": true,
             "licenseId": "Artistic-1.0",
             "name": "Artistic License 1.0",
             "reference": "https://spdx.org/licenses/Artistic-1.0.html",
-            "referenceNumber": 266,
+            "referenceNumber": 282,
             "seeAlso": [
                 "https://opensource.org/licenses/Artistic-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Artistic-1.0-cl8.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Artistic-1.0-cl8",
             "name": "Artistic License 1.0 w/clause 8",
             "reference": "https://spdx.org/licenses/Artistic-1.0-cl8.html",
-            "referenceNumber": 89,
+            "referenceNumber": 209,
             "seeAlso": [
                 "https://opensource.org/licenses/Artistic-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Artistic-1.0-Perl.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Artistic-1.0-Perl",
             "name": "Artistic License 1.0 (Perl)",
             "reference": "https://spdx.org/licenses/Artistic-1.0-Perl.html",
-            "referenceNumber": 301,
+            "referenceNumber": 552,
             "seeAlso": [
                 "http://dev.perl.org/licenses/artistic.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Artistic-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "Artistic-2.0",
             "name": "Artistic License 2.0",
             "reference": "https://spdx.org/licenses/Artistic-2.0.html",
-            "referenceNumber": 350,
+            "referenceNumber": 151,
             "seeAlso": [
                 "http://www.perlfoundation.org/artistic_license_2_0",
                 "https://www.perlfoundation.org/artistic-license-20.html",
                 "https://opensource.org/licenses/artistic-license-2.0"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/ASWF-Digital-Assets-1.0.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "ASWF-Digital-Assets-1.0",
+            "name": "ASWF Digital Assets License version 1.0",
+            "reference": "https://spdx.org/licenses/ASWF-Digital-Assets-1.0.html",
+            "referenceNumber": 277,
+            "seeAlso": [
+                "https://github.com/AcademySoftwareFoundation/foundation/blob/main/digital_assets/aswf_digital_assets_license_v1.0.txt"
+            ]
+        },
+        {
+            "detailsUrl": "https://spdx.org/licenses/ASWF-Digital-Assets-1.1.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "ASWF-Digital-Assets-1.1",
+            "name": "ASWF Digital Assets License 1.1",
+            "reference": "https://spdx.org/licenses/ASWF-Digital-Assets-1.1.html",
+            "referenceNumber": 266,
+            "seeAlso": [
+                "https://github.com/AcademySoftwareFoundation/foundation/blob/main/digital_assets/aswf_digital_assets_license_v1.1.txt"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Baekmuk.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Baekmuk",
             "name": "Baekmuk License",
             "reference": "https://spdx.org/licenses/Baekmuk.html",
-            "referenceNumber": 472,
+            "referenceNumber": 77,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing:Baekmuk?rd=Licensing/Baekmuk"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Bahyph.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Bahyph",
             "name": "Bahyph License",
             "reference": "https://spdx.org/licenses/Bahyph.html",
-            "referenceNumber": 161,
+            "referenceNumber": 4,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Bahyph"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Barr.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Barr",
             "name": "Barr License",
             "reference": "https://spdx.org/licenses/Barr.html",
-            "referenceNumber": 177,
+            "referenceNumber": 401,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Barr"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Beerware.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Beerware",
             "name": "Beerware License",
             "reference": "https://spdx.org/licenses/Beerware.html",
-            "referenceNumber": 423,
+            "referenceNumber": 487,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Beerware",
                 "https://people.freebsd.org/~phk/"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Bitstream-Charter.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Bitstream-Charter",
+            "name": "Bitstream Charter Font License",
+            "reference": "https://spdx.org/licenses/Bitstream-Charter.html",
+            "referenceNumber": 174,
+            "seeAlso": [
+                "https://fedoraproject.org/wiki/Licensing/Charter#License_Text",
+                "https://raw.githubusercontent.com/blackhole89/notekit/master/data/fonts/Charter%20license.txt"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Bitstream-Vera.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Bitstream-Vera",
             "name": "Bitstream Vera Font License",
             "reference": "https://spdx.org/licenses/Bitstream-Vera.html",
-            "referenceNumber": 458,
+            "referenceNumber": 509,
             "seeAlso": [
                 "https://web.archive.org/web/20080207013128/http://www.gnome.org/fonts/",
                 "https://docubrain.com/sites/default/files/licenses/bitstream-vera.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BitTorrent-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BitTorrent-1.0",
             "name": "BitTorrent Open Source License v1.0",
             "reference": "https://spdx.org/licenses/BitTorrent-1.0.html",
-            "referenceNumber": 175,
+            "referenceNumber": 503,
             "seeAlso": [
                 "http://sources.gentoo.org/cgi-bin/viewvc.cgi/gentoo-x86/licenses/BitTorrent?r1=1.1&r2=1.1.1.1&diff_format=s"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BitTorrent-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "BitTorrent-1.1",
             "name": "BitTorrent Open Source License v1.1",
             "reference": "https://spdx.org/licenses/BitTorrent-1.1.html",
-            "referenceNumber": 441,
+            "referenceNumber": 74,
             "seeAlso": [
                 "http://directory.fsf.org/wiki/License:BitTorrentOSL1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/blessing.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "blessing",
             "name": "SQLite Blessing",
             "reference": "https://spdx.org/licenses/blessing.html",
-            "referenceNumber": 77,
+            "referenceNumber": 444,
             "seeAlso": [
                 "https://www.sqlite.org/src/artifact/e33a4df7e32d742a?ln=4-9",
                 "https://sqlite.org/src/artifact/df5091916dbb40e6"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BlueOak-1.0.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BlueOak-1.0.0",
             "name": "Blue Oak Model License 1.0.0",
             "reference": "https://spdx.org/licenses/BlueOak-1.0.0.html",
-            "referenceNumber": 276,
+            "referenceNumber": 428,
             "seeAlso": [
                 "https://blueoakcouncil.org/license/1.0.0"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Boehm-GC.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Boehm-GC",
+            "name": "Boehm-Demers-Weiser GC License",
+            "reference": "https://spdx.org/licenses/Boehm-GC.html",
+            "referenceNumber": 313,
+            "seeAlso": [
+                "https://fedoraproject.org/wiki/Licensing:MIT#Another_Minimal_variant_(found_in_libatomic_ops)",
+                "https://github.com/uim/libgcroots/blob/master/COPYING",
+                "https://github.com/ivmai/libatomic_ops/blob/master/LICENSE"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Borceux.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Borceux",
             "name": "Borceux license",
             "reference": "https://spdx.org/licenses/Borceux.html",
-            "referenceNumber": 212,
+            "referenceNumber": 329,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Borceux"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Brian-Gladman-3-Clause.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Brian-Gladman-3-Clause",
+            "name": "Brian Gladman 3-Clause License",
+            "reference": "https://spdx.org/licenses/Brian-Gladman-3-Clause.html",
+            "referenceNumber": 131,
+            "seeAlso": [
+                "https://github.com/SWI-Prolog/packages-clib/blob/master/sha1/brg_endian.h"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/BSD-1-Clause.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "BSD-1-Clause",
             "name": "BSD 1-Clause License",
             "reference": "https://spdx.org/licenses/BSD-1-Clause.html",
-            "referenceNumber": 440,
+            "referenceNumber": 203,
             "seeAlso": [
                 "https://svnweb.freebsd.org/base/head/include/ifaddrs.h?revision=326823"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-2-Clause.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "BSD-2-Clause",
             "name": "BSD 2-Clause \"Simplified\" License",
             "reference": "https://spdx.org/licenses/BSD-2-Clause.html",
-            "referenceNumber": 93,
+            "referenceNumber": 269,
             "seeAlso": [
                 "https://opensource.org/licenses/BSD-2-Clause"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-2-Clause-FreeBSD.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "BSD-2-Clause-FreeBSD",
             "name": "BSD 2-Clause FreeBSD License",
             "reference": "https://spdx.org/licenses/BSD-2-Clause-FreeBSD.html",
-            "referenceNumber": 298,
+            "referenceNumber": 23,
             "seeAlso": [
                 "http://www.freebsd.org/copyright/freebsd-license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-2-Clause-NetBSD.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "BSD-2-Clause-NetBSD",
             "name": "BSD 2-Clause NetBSD License",
             "reference": "https://spdx.org/licenses/BSD-2-Clause-NetBSD.html",
-            "referenceNumber": 382,
+            "referenceNumber": 365,
             "seeAlso": [
                 "http://www.netbsd.org/about/redistribution.html#default"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-2-Clause-Patent.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "BSD-2-Clause-Patent",
             "name": "BSD-2-Clause Plus Patent License",
             "reference": "https://spdx.org/licenses/BSD-2-Clause-Patent.html",
-            "referenceNumber": 327,
+            "referenceNumber": 494,
             "seeAlso": [
                 "https://opensource.org/licenses/BSDplusPatent"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-2-Clause-Views.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-2-Clause-Views",
             "name": "BSD 2-Clause with views sentence",
             "reference": "https://spdx.org/licenses/BSD-2-Clause-Views.html",
-            "referenceNumber": 498,
+            "referenceNumber": 555,
             "seeAlso": [
                 "http://www.freebsd.org/copyright/freebsd-license.html",
                 "https://people.freebsd.org/~ivoras/wine/patch-wine-nvidia.sh",
                 "https://github.com/protegeproject/protege/blob/master/license.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-3-Clause.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "BSD-3-Clause",
             "name": "BSD 3-Clause \"New\" or \"Revised\" License",
             "reference": "https://spdx.org/licenses/BSD-3-Clause.html",
-            "referenceNumber": 416,
+            "referenceNumber": 320,
             "seeAlso": [
                 "https://opensource.org/licenses/BSD-3-Clause",
                 "https://www.eclipse.org/org/documents/edl-v10.php"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-3-Clause-Attribution.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-3-Clause-Attribution",
             "name": "BSD with attribution",
             "reference": "https://spdx.org/licenses/BSD-3-Clause-Attribution.html",
-            "referenceNumber": 33,
+            "referenceNumber": 195,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/BSD_with_Attribution"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-3-Clause-Clear.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "BSD-3-Clause-Clear",
             "name": "BSD 3-Clause Clear License",
             "reference": "https://spdx.org/licenses/BSD-3-Clause-Clear.html",
-            "referenceNumber": 224,
+            "referenceNumber": 231,
             "seeAlso": [
                 "http://labs.metacarta.com/license-explanation.html#license"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-3-Clause-LBNL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "BSD-3-Clause-LBNL",
             "name": "Lawrence Berkeley National Labs BSD variant license",
             "reference": "https://spdx.org/licenses/BSD-3-Clause-LBNL.html",
-            "referenceNumber": 424,
+            "referenceNumber": 45,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/LBNLBSD"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-3-Clause-Modification.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-3-Clause-Modification",
             "name": "BSD 3-Clause Modification",
             "reference": "https://spdx.org/licenses/BSD-3-Clause-Modification.html",
-            "referenceNumber": 96,
+            "referenceNumber": 202,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing:BSD#Modification_Variant"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-3-Clause-No-Military-License.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-3-Clause-No-Military-License",
             "name": "BSD 3-Clause No Military License",
             "reference": "https://spdx.org/licenses/BSD-3-Clause-No-Military-License.html",
-            "referenceNumber": 321,
+            "referenceNumber": 341,
             "seeAlso": [
                 "https://gitlab.syncad.com/hive/dhive/-/blob/master/LICENSE",
                 "https://github.com/greymass/swift-eosio/blob/master/LICENSE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-3-Clause-No-Nuclear-License.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-3-Clause-No-Nuclear-License",
             "name": "BSD 3-Clause No Nuclear License",
             "reference": "https://spdx.org/licenses/BSD-3-Clause-No-Nuclear-License.html",
-            "referenceNumber": 2,
+            "referenceNumber": 333,
             "seeAlso": [
                 "http://download.oracle.com/otn-pub/java/licenses/bsd.txt?AuthParam=1467140197_43d516ce1776bd08a58235a7785be1cc"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-3-Clause-No-Nuclear-License-2014.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-3-Clause-No-Nuclear-License-2014",
             "name": "BSD 3-Clause No Nuclear License 2014",
             "reference": "https://spdx.org/licenses/BSD-3-Clause-No-Nuclear-License-2014.html",
-            "referenceNumber": 420,
+            "referenceNumber": 447,
             "seeAlso": [
                 "https://java.net/projects/javaeetutorial/pages/BerkeleyLicense"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-3-Clause-No-Nuclear-Warranty.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-3-Clause-No-Nuclear-Warranty",
             "name": "BSD 3-Clause No Nuclear Warranty",
             "reference": "https://spdx.org/licenses/BSD-3-Clause-No-Nuclear-Warranty.html",
-            "referenceNumber": 389,
+            "referenceNumber": 79,
             "seeAlso": [
                 "https://jogamp.org/git/?p=gluegen.git;a=blob_plain;f=LICENSE.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-3-Clause-Open-MPI.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-3-Clause-Open-MPI",
             "name": "BSD 3-Clause Open MPI variant",
             "reference": "https://spdx.org/licenses/BSD-3-Clause-Open-MPI.html",
-            "referenceNumber": 162,
+            "referenceNumber": 483,
             "seeAlso": [
                 "https://www.open-mpi.org/community/license.php",
                 "http://www.netlib.org/lapack/LICENSE.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-4-Clause.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "BSD-4-Clause",
             "name": "BSD 4-Clause \"Original\" or \"Old\" License",
             "reference": "https://spdx.org/licenses/BSD-4-Clause.html",
-            "referenceNumber": 497,
+            "referenceNumber": 553,
             "seeAlso": [
                 "http://directory.fsf.org/wiki/License:BSD_4Clause"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-4-Clause-Shortened.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-4-Clause-Shortened",
             "name": "BSD 4 Clause Shortened",
             "reference": "https://spdx.org/licenses/BSD-4-Clause-Shortened.html",
-            "referenceNumber": 269,
+            "referenceNumber": 41,
             "seeAlso": [
                 "https://metadata.ftp-master.debian.org/changelogs//main/a/arpwatch/arpwatch_2.1a15-7_copyright"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-4-Clause-UC.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-4-Clause-UC",
             "name": "BSD-4-Clause (University of California-Specific)",
             "reference": "https://spdx.org/licenses/BSD-4-Clause-UC.html",
-            "referenceNumber": 146,
+            "referenceNumber": 166,
             "seeAlso": [
                 "http://www.freebsd.org/copyright/license.html"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/BSD-4.3RENO.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "BSD-4.3RENO",
+            "name": "BSD 4.3 RENO License",
+            "reference": "https://spdx.org/licenses/BSD-4.3RENO.html",
+            "referenceNumber": 130,
+            "seeAlso": [
+                "https://sourceware.org/git/?p=binutils-gdb.git;a=blob;f=libiberty/strcasecmp.c;h=131d81c2ce7881fa48c363dc5bf5fb302c61ce0b;hb=HEAD"
+            ]
+        },
+        {
+            "detailsUrl": "https://spdx.org/licenses/BSD-4.3TAHOE.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "BSD-4.3TAHOE",
+            "name": "BSD 4.3 TAHOE License",
+            "reference": "https://spdx.org/licenses/BSD-4.3TAHOE.html",
+            "referenceNumber": 515,
+            "seeAlso": [
+                "https://github.com/389ds/389-ds-base/blob/main/ldap/include/sysexits-compat.h#L15",
+                "https://git.savannah.gnu.org/cgit/indent.git/tree/doc/indent.texi?id=a74c6b4ee49397cf330b333da1042bffa60ed14f#n1788"
+            ]
+        },
+        {
+            "detailsUrl": "https://spdx.org/licenses/BSD-Advertising-Acknowledgement.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "BSD-Advertising-Acknowledgement",
+            "name": "BSD Advertising Acknowledgement License",
+            "reference": "https://spdx.org/licenses/BSD-Advertising-Acknowledgement.html",
+            "referenceNumber": 367,
+            "seeAlso": [
+                "https://github.com/python-excel/xlrd/blob/master/LICENSE#L33"
+            ]
+        },
+        {
+            "detailsUrl": "https://spdx.org/licenses/BSD-Attribution-HPND-disclaimer.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "BSD-Attribution-HPND-disclaimer",
+            "name": "BSD with Attribution and HPND disclaimer",
+            "reference": "https://spdx.org/licenses/BSD-Attribution-HPND-disclaimer.html",
+            "referenceNumber": 280,
+            "seeAlso": [
+                "https://github.com/cyrusimap/cyrus-sasl/blob/master/COPYING"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/BSD-Protection.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-Protection",
             "name": "BSD Protection License",
             "reference": "https://spdx.org/licenses/BSD-Protection.html",
-            "referenceNumber": 133,
+            "referenceNumber": 126,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/BSD_Protection_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-Source-Code.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-Source-Code",
             "name": "BSD Source Code Attribution",
             "reference": "https://spdx.org/licenses/BSD-Source-Code.html",
-            "referenceNumber": 10,
+            "referenceNumber": 396,
             "seeAlso": [
                 "https://github.com/robbiehanson/CocoaHTTPServer/blob/master/LICENSE.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "BSL-1.0",
             "name": "Boost Software License 1.0",
             "reference": "https://spdx.org/licenses/BSL-1.0.html",
-            "referenceNumber": 386,
+            "referenceNumber": 467,
             "seeAlso": [
                 "http://www.boost.org/LICENSE_1_0.txt",
                 "https://opensource.org/licenses/BSL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BUSL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BUSL-1.1",
             "name": "Business Source License 1.1",
             "reference": "https://spdx.org/licenses/BUSL-1.1.html",
-            "referenceNumber": 292,
+            "referenceNumber": 256,
             "seeAlso": [
                 "https://mariadb.com/bsl11/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/bzip2-1.0.5.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": false,
             "licenseId": "bzip2-1.0.5",
             "name": "bzip2 and libbzip2 License v1.0.5",
             "reference": "https://spdx.org/licenses/bzip2-1.0.5.html",
-            "referenceNumber": 122,
+            "referenceNumber": 238,
             "seeAlso": [
                 "https://sourceware.org/bzip2/1.0.5/bzip2-manual-1.0.5.html",
                 "http://bzip.org/1.0.5/bzip2-manual-1.0.5.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/bzip2-1.0.6.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "bzip2-1.0.6",
             "name": "bzip2 and libbzip2 License v1.0.6",
             "reference": "https://spdx.org/licenses/bzip2-1.0.6.html",
-            "referenceNumber": 387,
+            "referenceNumber": 392,
             "seeAlso": [
                 "https://sourceware.org/git/?p=bzip2.git;a=blob;f=LICENSE;hb=bzip2-1.0.6",
                 "http://bzip.org/1.0.5/bzip2-manual-1.0.5.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/C-UDA-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "C-UDA-1.0",
             "name": "Computational Use of Data Agreement v1.0",
             "reference": "https://spdx.org/licenses/C-UDA-1.0.html",
-            "referenceNumber": 457,
+            "referenceNumber": 194,
             "seeAlso": [
                 "https://github.com/microsoft/Computational-Use-of-Data-Agreement/blob/master/C-UDA-1.0.md",
                 "https://cdla.dev/computational-use-of-data-agreement-v1-0/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CAL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "CAL-1.0",
             "name": "Cryptographic Autonomy License 1.0",
             "reference": "https://spdx.org/licenses/CAL-1.0.html",
-            "referenceNumber": 235,
+            "referenceNumber": 347,
             "seeAlso": [
                 "http://cryptographicautonomylicense.com/license-text.html",
                 "https://opensource.org/licenses/CAL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CAL-1.0-Combined-Work-Exception.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "CAL-1.0-Combined-Work-Exception",
             "name": "Cryptographic Autonomy License 1.0 (Combined Work Exception)",
             "reference": "https://spdx.org/licenses/CAL-1.0-Combined-Work-Exception.html",
-            "referenceNumber": 141,
+            "referenceNumber": 316,
             "seeAlso": [
                 "http://cryptographicautonomylicense.com/license-text.html",
                 "https://opensource.org/licenses/CAL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Caldera.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Caldera",
             "name": "Caldera License",
             "reference": "https://spdx.org/licenses/Caldera.html",
-            "referenceNumber": 264,
+            "referenceNumber": 178,
             "seeAlso": [
                 "http://www.lemis.com/grog/UNIX/ancient-source-all.pdf"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CATOSL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "CATOSL-1.1",
             "name": "Computer Associates Trusted Open Source License 1.1",
             "reference": "https://spdx.org/licenses/CATOSL-1.1.html",
-            "referenceNumber": 481,
+            "referenceNumber": 253,
             "seeAlso": [
                 "https://opensource.org/licenses/CATOSL-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-1.0",
             "name": "Creative Commons Attribution 1.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-1.0.html",
-            "referenceNumber": 65,
+            "referenceNumber": 205,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/1.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-2.0",
             "name": "Creative Commons Attribution 2.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-2.0.html",
-            "referenceNumber": 280,
+            "referenceNumber": 61,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/2.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-2.5.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-2.5",
             "name": "Creative Commons Attribution 2.5 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-2.5.html",
-            "referenceNumber": 377,
+            "referenceNumber": 171,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/2.5/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-2.5-AU.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-2.5-AU",
             "name": "Creative Commons Attribution 2.5 Australia",
             "reference": "https://spdx.org/licenses/CC-BY-2.5-AU.html",
-            "referenceNumber": 256,
+            "referenceNumber": 128,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/2.5/au/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-3.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-3.0",
             "name": "Creative Commons Attribution 3.0 Unported",
             "reference": "https://spdx.org/licenses/CC-BY-3.0.html",
-            "referenceNumber": 273,
+            "referenceNumber": 435,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/3.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-3.0-AT.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-3.0-AT",
             "name": "Creative Commons Attribution 3.0 Austria",
             "reference": "https://spdx.org/licenses/CC-BY-3.0-AT.html",
-            "referenceNumber": 356,
+            "referenceNumber": 7,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/3.0/at/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-3.0-DE.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-3.0-DE",
             "name": "Creative Commons Attribution 3.0 Germany",
             "reference": "https://spdx.org/licenses/CC-BY-3.0-DE.html",
-            "referenceNumber": 454,
+            "referenceNumber": 317,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/3.0/de/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-3.0-IGO.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-3.0-IGO",
             "name": "Creative Commons Attribution 3.0 IGO",
             "reference": "https://spdx.org/licenses/CC-BY-3.0-IGO.html",
-            "referenceNumber": 126,
+            "referenceNumber": 141,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/3.0/igo/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-3.0-NL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-3.0-NL",
             "name": "Creative Commons Attribution 3.0 Netherlands",
             "reference": "https://spdx.org/licenses/CC-BY-3.0-NL.html",
-            "referenceNumber": 291,
+            "referenceNumber": 193,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/3.0/nl/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-3.0-US.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-3.0-US",
             "name": "Creative Commons Attribution 3.0 United States",
             "reference": "https://spdx.org/licenses/CC-BY-3.0-US.html",
-            "referenceNumber": 407,
+            "referenceNumber": 156,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/3.0/us/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-4.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "CC-BY-4.0",
             "name": "Creative Commons Attribution 4.0 International",
             "reference": "https://spdx.org/licenses/CC-BY-4.0.html",
-            "referenceNumber": 188,
+            "referenceNumber": 495,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/4.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-1.0",
             "name": "Creative Commons Attribution Non Commercial 1.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-NC-1.0.html",
-            "referenceNumber": 52,
+            "referenceNumber": 293,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc/1.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-2.0",
             "name": "Creative Commons Attribution Non Commercial 2.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-NC-2.0.html",
-            "referenceNumber": 160,
+            "referenceNumber": 143,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc/2.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-2.5.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-2.5",
             "name": "Creative Commons Attribution Non Commercial 2.5 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-NC-2.5.html",
-            "referenceNumber": 433,
+            "referenceNumber": 457,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc/2.5/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-3.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-3.0",
             "name": "Creative Commons Attribution Non Commercial 3.0 Unported",
             "reference": "https://spdx.org/licenses/CC-BY-NC-3.0.html",
-            "referenceNumber": 108,
+            "referenceNumber": 216,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc/3.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-3.0-DE.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-3.0-DE",
             "name": "Creative Commons Attribution Non Commercial 3.0 Germany",
             "reference": "https://spdx.org/licenses/CC-BY-NC-3.0-DE.html",
-            "referenceNumber": 392,
+            "referenceNumber": 196,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc/3.0/de/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-4.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-4.0",
             "name": "Creative Commons Attribution Non Commercial 4.0 International",
             "reference": "https://spdx.org/licenses/CC-BY-NC-4.0.html",
-            "referenceNumber": 237,
+            "referenceNumber": 245,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc/4.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-ND-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-ND-1.0",
             "name": "Creative Commons Attribution Non Commercial No Derivatives 1.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-NC-ND-1.0.html",
-            "referenceNumber": 419,
+            "referenceNumber": 368,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nd-nc/1.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-ND-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-ND-2.0",
             "name": "Creative Commons Attribution Non Commercial No Derivatives 2.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-NC-ND-2.0.html",
-            "referenceNumber": 1,
+            "referenceNumber": 462,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-nd/2.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-ND-2.5.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-ND-2.5",
             "name": "Creative Commons Attribution Non Commercial No Derivatives 2.5 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-NC-ND-2.5.html",
-            "referenceNumber": 352,
+            "referenceNumber": 464,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-nd/2.5/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-ND-3.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-ND-3.0",
             "name": "Creative Commons Attribution Non Commercial No Derivatives 3.0 Unported",
             "reference": "https://spdx.org/licenses/CC-BY-NC-ND-3.0.html",
-            "referenceNumber": 257,
+            "referenceNumber": 478,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-nd/3.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-ND-3.0-DE.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-ND-3.0-DE",
             "name": "Creative Commons Attribution Non Commercial No Derivatives 3.0 Germany",
             "reference": "https://spdx.org/licenses/CC-BY-NC-ND-3.0-DE.html",
-            "referenceNumber": 184,
+            "referenceNumber": 384,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-nd/3.0/de/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-ND-3.0-IGO.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-ND-3.0-IGO",
             "name": "Creative Commons Attribution Non Commercial No Derivatives 3.0 IGO",
             "reference": "https://spdx.org/licenses/CC-BY-NC-ND-3.0-IGO.html",
-            "referenceNumber": 59,
+            "referenceNumber": 211,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-nd/3.0/igo/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-ND-4.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-ND-4.0",
             "name": "Creative Commons Attribution Non Commercial No Derivatives 4.0 International",
             "reference": "https://spdx.org/licenses/CC-BY-NC-ND-4.0.html",
-            "referenceNumber": 253,
+            "referenceNumber": 469,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-nd/4.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-SA-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-SA-1.0",
             "name": "Creative Commons Attribution Non Commercial Share Alike 1.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-NC-SA-1.0.html",
-            "referenceNumber": 130,
+            "referenceNumber": 129,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-sa/1.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-SA-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-SA-2.0",
             "name": "Creative Commons Attribution Non Commercial Share Alike 2.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-NC-SA-2.0.html",
-            "referenceNumber": 466,
+            "referenceNumber": 432,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-sa/2.0/legalcode"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-SA-2.0-DE.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "CC-BY-NC-SA-2.0-DE",
+            "name": "Creative Commons Attribution Non Commercial Share Alike 2.0 Germany",
+            "reference": "https://spdx.org/licenses/CC-BY-NC-SA-2.0-DE.html",
+            "referenceNumber": 452,
+            "seeAlso": [
+                "https://creativecommons.org/licenses/by-nc-sa/2.0/de/legalcode"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-SA-2.0-FR.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-SA-2.0-FR",
             "name": "Creative Commons Attribution-NonCommercial-ShareAlike 2.0 France",
             "reference": "https://spdx.org/licenses/CC-BY-NC-SA-2.0-FR.html",
-            "referenceNumber": 203,
+            "referenceNumber": 25,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-sa/2.0/fr/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-SA-2.0-UK.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-SA-2.0-UK",
             "name": "Creative Commons Attribution Non Commercial Share Alike 2.0 England and Wales",
             "reference": "https://spdx.org/licenses/CC-BY-NC-SA-2.0-UK.html",
-            "referenceNumber": 201,
+            "referenceNumber": 460,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-sa/2.0/uk/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-SA-2.5.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-SA-2.5",
             "name": "Creative Commons Attribution Non Commercial Share Alike 2.5 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-NC-SA-2.5.html",
-            "referenceNumber": 262,
+            "referenceNumber": 8,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-sa/2.5/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-SA-3.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-SA-3.0",
             "name": "Creative Commons Attribution Non Commercial Share Alike 3.0 Unported",
             "reference": "https://spdx.org/licenses/CC-BY-NC-SA-3.0.html",
-            "referenceNumber": 209,
+            "referenceNumber": 271,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-sa/3.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-SA-3.0-DE.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-SA-3.0-DE",
             "name": "Creative Commons Attribution Non Commercial Share Alike 3.0 Germany",
             "reference": "https://spdx.org/licenses/CC-BY-NC-SA-3.0-DE.html",
-            "referenceNumber": 326,
+            "referenceNumber": 505,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-sa/3.0/de/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-SA-3.0-IGO.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-SA-3.0-IGO",
             "name": "Creative Commons Attribution Non Commercial Share Alike 3.0 IGO",
             "reference": "https://spdx.org/licenses/CC-BY-NC-SA-3.0-IGO.html",
-            "referenceNumber": 29,
+            "referenceNumber": 14,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-sa/3.0/igo/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-SA-4.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-SA-4.0",
             "name": "Creative Commons Attribution Non Commercial Share Alike 4.0 International",
             "reference": "https://spdx.org/licenses/CC-BY-NC-SA-4.0.html",
-            "referenceNumber": 415,
+            "referenceNumber": 338,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-ND-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-ND-1.0",
             "name": "Creative Commons Attribution No Derivatives 1.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-ND-1.0.html",
-            "referenceNumber": 53,
+            "referenceNumber": 115,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nd/1.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-ND-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-ND-2.0",
             "name": "Creative Commons Attribution No Derivatives 2.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-ND-2.0.html",
-            "referenceNumber": 422,
+            "referenceNumber": 116,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nd/2.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-ND-2.5.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-ND-2.5",
             "name": "Creative Commons Attribution No Derivatives 2.5 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-ND-2.5.html",
-            "referenceNumber": 157,
+            "referenceNumber": 13,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nd/2.5/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-ND-3.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-ND-3.0",
             "name": "Creative Commons Attribution No Derivatives 3.0 Unported",
             "reference": "https://spdx.org/licenses/CC-BY-ND-3.0.html",
-            "referenceNumber": 323,
+            "referenceNumber": 28,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nd/3.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-ND-3.0-DE.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-ND-3.0-DE",
             "name": "Creative Commons Attribution No Derivatives 3.0 Germany",
             "reference": "https://spdx.org/licenses/CC-BY-ND-3.0-DE.html",
-            "referenceNumber": 338,
+            "referenceNumber": 322,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nd/3.0/de/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-ND-4.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-ND-4.0",
             "name": "Creative Commons Attribution No Derivatives 4.0 International",
             "reference": "https://spdx.org/licenses/CC-BY-ND-4.0.html",
-            "referenceNumber": 74,
+            "referenceNumber": 44,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nd/4.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-SA-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-SA-1.0",
             "name": "Creative Commons Attribution Share Alike 1.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-SA-1.0.html",
-            "referenceNumber": 446,
+            "referenceNumber": 71,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-sa/1.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-SA-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-SA-2.0",
             "name": "Creative Commons Attribution Share Alike 2.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-SA-2.0.html",
-            "referenceNumber": 267,
+            "referenceNumber": 252,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-sa/2.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-SA-2.0-UK.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-SA-2.0-UK",
             "name": "Creative Commons Attribution Share Alike 2.0 England and Wales",
             "reference": "https://spdx.org/licenses/CC-BY-SA-2.0-UK.html",
-            "referenceNumber": 98,
+            "referenceNumber": 72,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-sa/2.0/uk/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-SA-2.1-JP.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-SA-2.1-JP",
             "name": "Creative Commons Attribution Share Alike 2.1 Japan",
             "reference": "https://spdx.org/licenses/CC-BY-SA-2.1-JP.html",
-            "referenceNumber": 55,
+            "referenceNumber": 54,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-sa/2.1/jp/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-SA-2.5.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-SA-2.5",
             "name": "Creative Commons Attribution Share Alike 2.5 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-SA-2.5.html",
-            "referenceNumber": 143,
+            "referenceNumber": 375,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-sa/2.5/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-SA-3.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-SA-3.0",
             "name": "Creative Commons Attribution Share Alike 3.0 Unported",
             "reference": "https://spdx.org/licenses/CC-BY-SA-3.0.html",
-            "referenceNumber": 75,
+            "referenceNumber": 139,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-sa/3.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-SA-3.0-AT.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-SA-3.0-AT",
             "name": "Creative Commons Attribution Share Alike 3.0 Austria",
             "reference": "https://spdx.org/licenses/CC-BY-SA-3.0-AT.html",
-            "referenceNumber": 70,
+            "referenceNumber": 190,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-sa/3.0/at/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-SA-3.0-DE.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-SA-3.0-DE",
             "name": "Creative Commons Attribution Share Alike 3.0 Germany",
             "reference": "https://spdx.org/licenses/CC-BY-SA-3.0-DE.html",
-            "referenceNumber": 231,
+            "referenceNumber": 385,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-sa/3.0/de/legalcode"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/CC-BY-SA-3.0-IGO.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "CC-BY-SA-3.0-IGO",
+            "name": "Creative Commons Attribution-ShareAlike 3.0 IGO",
+            "reference": "https://spdx.org/licenses/CC-BY-SA-3.0-IGO.html",
+            "referenceNumber": 213,
+            "seeAlso": [
+                "https://creativecommons.org/licenses/by-sa/3.0/igo/legalcode"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-SA-4.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "CC-BY-SA-4.0",
             "name": "Creative Commons Attribution Share Alike 4.0 International",
             "reference": "https://spdx.org/licenses/CC-BY-SA-4.0.html",
-            "referenceNumber": 44,
+            "referenceNumber": 342,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-sa/4.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-PDDC.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-PDDC",
             "name": "Creative Commons Public Domain Dedication and Certification",
             "reference": "https://spdx.org/licenses/CC-PDDC.html",
-            "referenceNumber": 139,
+            "referenceNumber": 230,
             "seeAlso": [
                 "https://creativecommons.org/licenses/publicdomain/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC0-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "CC0-1.0",
             "name": "Creative Commons Zero v1.0 Universal",
             "reference": "https://spdx.org/licenses/CC0-1.0.html",
-            "referenceNumber": 331,
+            "referenceNumber": 279,
             "seeAlso": [
                 "https://creativecommons.org/publicdomain/zero/1.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CDDL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "CDDL-1.0",
             "name": "Common Development and Distribution License 1.0",
             "reference": "https://spdx.org/licenses/CDDL-1.0.html",
-            "referenceNumber": 369,
+            "referenceNumber": 187,
             "seeAlso": [
                 "https://opensource.org/licenses/cddl1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CDDL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CDDL-1.1",
             "name": "Common Development and Distribution License 1.1",
             "reference": "https://spdx.org/licenses/CDDL-1.1.html",
-            "referenceNumber": 491,
+            "referenceNumber": 352,
             "seeAlso": [
                 "http://glassfish.java.net/public/CDDL+GPL_1_1.html",
                 "https://javaee.github.io/glassfish/LICENSE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CDL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CDL-1.0",
             "name": "Common Documentation License 1.0",
             "reference": "https://spdx.org/licenses/CDL-1.0.html",
-            "referenceNumber": 409,
+            "referenceNumber": 11,
             "seeAlso": [
                 "http://www.opensource.apple.com/cdl/",
                 "https://fedoraproject.org/wiki/Licensing/Common_Documentation_License",
                 "https://www.gnu.org/licenses/license-list.html#ACDL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CDLA-Permissive-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CDLA-Permissive-1.0",
             "name": "Community Data License Agreement Permissive 1.0",
             "reference": "https://spdx.org/licenses/CDLA-Permissive-1.0.html",
-            "referenceNumber": 336,
+            "referenceNumber": 241,
             "seeAlso": [
                 "https://cdla.io/permissive-1-0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CDLA-Permissive-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CDLA-Permissive-2.0",
             "name": "Community Data License Agreement Permissive 2.0",
             "reference": "https://spdx.org/licenses/CDLA-Permissive-2.0.html",
-            "referenceNumber": 357,
+            "referenceNumber": 272,
             "seeAlso": [
                 "https://cdla.dev/permissive-2-0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CDLA-Sharing-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CDLA-Sharing-1.0",
             "name": "Community Data License Agreement Sharing 1.0",
             "reference": "https://spdx.org/licenses/CDLA-Sharing-1.0.html",
-            "referenceNumber": 102,
+            "referenceNumber": 536,
             "seeAlso": [
                 "https://cdla.io/sharing-1-0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CECILL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CECILL-1.0",
             "name": "CeCILL Free Software License Agreement v1.0",
             "reference": "https://spdx.org/licenses/CECILL-1.0.html",
-            "referenceNumber": 7,
+            "referenceNumber": 376,
             "seeAlso": [
                 "http://www.cecill.info/licences/Licence_CeCILL_V1-fr.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CECILL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CECILL-1.1",
             "name": "CeCILL Free Software License Agreement v1.1",
             "reference": "https://spdx.org/licenses/CECILL-1.1.html",
-            "referenceNumber": 43,
+            "referenceNumber": 522,
             "seeAlso": [
                 "http://www.cecill.info/licences/Licence_CeCILL_V1.1-US.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CECILL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "CECILL-2.0",
             "name": "CeCILL Free Software License Agreement v2.0",
             "reference": "https://spdx.org/licenses/CECILL-2.0.html",
-            "referenceNumber": 153,
+            "referenceNumber": 150,
             "seeAlso": [
                 "http://www.cecill.info/licences/Licence_CeCILL_V2-en.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CECILL-2.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "CECILL-2.1",
             "name": "CeCILL Free Software License Agreement v2.1",
             "reference": "https://spdx.org/licenses/CECILL-2.1.html",
-            "referenceNumber": 344,
+            "referenceNumber": 227,
             "seeAlso": [
                 "http://www.cecill.info/licences/Licence_CeCILL_V2.1-en.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CECILL-B.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "CECILL-B",
             "name": "CeCILL-B Free Software License Agreement",
             "reference": "https://spdx.org/licenses/CECILL-B.html",
-            "referenceNumber": 403,
+            "referenceNumber": 308,
             "seeAlso": [
                 "http://www.cecill.info/licences/Licence_CeCILL-B_V1-en.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CECILL-C.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "CECILL-C",
             "name": "CeCILL-C Free Software License Agreement",
             "reference": "https://spdx.org/licenses/CECILL-C.html",
-            "referenceNumber": 205,
+            "referenceNumber": 125,
             "seeAlso": [
                 "http://www.cecill.info/licences/Licence_CeCILL-C_V1-en.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CERN-OHL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CERN-OHL-1.1",
             "name": "CERN Open Hardware Licence v1.1",
             "reference": "https://spdx.org/licenses/CERN-OHL-1.1.html",
-            "referenceNumber": 367,
+            "referenceNumber": 348,
             "seeAlso": [
                 "https://www.ohwr.org/project/licenses/wikis/cern-ohl-v1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CERN-OHL-1.2.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CERN-OHL-1.2",
             "name": "CERN Open Hardware Licence v1.2",
             "reference": "https://spdx.org/licenses/CERN-OHL-1.2.html",
-            "referenceNumber": 456,
+            "referenceNumber": 472,
             "seeAlso": [
                 "https://www.ohwr.org/project/licenses/wikis/cern-ohl-v1.2"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CERN-OHL-P-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "CERN-OHL-P-2.0",
             "name": "CERN Open Hardware Licence Version 2 - Permissive",
             "reference": "https://spdx.org/licenses/CERN-OHL-P-2.0.html",
-            "referenceNumber": 333,
+            "referenceNumber": 442,
             "seeAlso": [
                 "https://www.ohwr.org/project/cernohl/wikis/Documents/CERN-OHL-version-2"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CERN-OHL-S-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "CERN-OHL-S-2.0",
             "name": "CERN Open Hardware Licence Version 2 - Strongly Reciprocal",
             "reference": "https://spdx.org/licenses/CERN-OHL-S-2.0.html",
-            "referenceNumber": 159,
+            "referenceNumber": 497,
             "seeAlso": [
                 "https://www.ohwr.org/project/cernohl/wikis/Documents/CERN-OHL-version-2"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CERN-OHL-W-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "CERN-OHL-W-2.0",
             "name": "CERN Open Hardware Licence Version 2 - Weakly Reciprocal",
             "reference": "https://spdx.org/licenses/CERN-OHL-W-2.0.html",
-            "referenceNumber": 22,
+            "referenceNumber": 493,
             "seeAlso": [
                 "https://www.ohwr.org/project/cernohl/wikis/Documents/CERN-OHL-version-2"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/CFITSIO.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "CFITSIO",
+            "name": "CFITSIO License",
+            "reference": "https://spdx.org/licenses/CFITSIO.html",
+            "referenceNumber": 395,
+            "seeAlso": [
+                "https://heasarc.gsfc.nasa.gov/docs/software/fitsio/c/f_user/node9.html"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/checkmk.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "checkmk",
             "name": "Checkmk License",
             "reference": "https://spdx.org/licenses/checkmk.html",
-            "referenceNumber": 427,
+            "referenceNumber": 475,
             "seeAlso": [
                 "https://github.com/libcheck/check/blob/master/checkmk/checkmk.in"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ClArtistic.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "ClArtistic",
             "name": "Clarified Artistic License",
             "reference": "https://spdx.org/licenses/ClArtistic.html",
-            "referenceNumber": 54,
+            "referenceNumber": 412,
             "seeAlso": [
                 "http://gianluca.dellavedova.org/2011/01/03/clarified-artistic-license/",
                 "http://www.ncftp.com/ncftp/doc/LICENSE.txt"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Clips.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Clips",
+            "name": "Clips License",
+            "reference": "https://spdx.org/licenses/Clips.html",
+            "referenceNumber": 32,
+            "seeAlso": [
+                "https://github.com/DrItanium/maya/blob/master/LICENSE.CLIPS"
+            ]
+        },
+        {
+            "detailsUrl": "https://spdx.org/licenses/CMU-Mach.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "CMU-Mach",
+            "name": "CMU Mach License",
+            "reference": "https://spdx.org/licenses/CMU-Mach.html",
+            "referenceNumber": 355,
+            "seeAlso": [
+                "https://www.cs.cmu.edu/~410/licenses.html"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/CNRI-Jython.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CNRI-Jython",
             "name": "CNRI Jython License",
             "reference": "https://spdx.org/licenses/CNRI-Jython.html",
-            "referenceNumber": 191,
+            "referenceNumber": 491,
             "seeAlso": [
                 "http://www.jython.org/license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CNRI-Python.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "CNRI-Python",
             "name": "CNRI Python License",
             "reference": "https://spdx.org/licenses/CNRI-Python.html",
-            "referenceNumber": 346,
+            "referenceNumber": 120,
             "seeAlso": [
                 "https://opensource.org/licenses/CNRI-Python"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CNRI-Python-GPL-Compatible.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CNRI-Python-GPL-Compatible",
             "name": "CNRI Python Open Source GPL Compatible License Agreement",
             "reference": "https://spdx.org/licenses/CNRI-Python-GPL-Compatible.html",
-            "referenceNumber": 34,
+            "referenceNumber": 404,
             "seeAlso": [
                 "http://www.python.org/download/releases/1.6.1/download_win/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/COIL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "COIL-1.0",
             "name": "Copyfree Open Innovation License",
             "reference": "https://spdx.org/licenses/COIL-1.0.html",
-            "referenceNumber": 17,
+            "referenceNumber": 163,
             "seeAlso": [
                 "https://coil.apotheon.org/plaintext/01.0.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Community-Spec-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Community-Spec-1.0",
             "name": "Community Specification License 1.0",
             "reference": "https://spdx.org/licenses/Community-Spec-1.0.html",
-            "referenceNumber": 36,
+            "referenceNumber": 345,
             "seeAlso": [
                 "https://github.com/CommunitySpecification/1.0/blob/master/1._Community_Specification_License-v1.md"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Condor-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "Condor-1.1",
             "name": "Condor Public License v1.1",
             "reference": "https://spdx.org/licenses/Condor-1.1.html",
-            "referenceNumber": 410,
+            "referenceNumber": 351,
             "seeAlso": [
                 "http://research.cs.wisc.edu/condor/license.html#condor",
                 "http://web.archive.org/web/20111123062036/http://research.cs.wisc.edu/condor/license.html#condor"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/copyleft-next-0.3.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "copyleft-next-0.3.0",
             "name": "copyleft-next 0.3.0",
             "reference": "https://spdx.org/licenses/copyleft-next-0.3.0.html",
-            "referenceNumber": 370,
+            "referenceNumber": 259,
             "seeAlso": [
                 "https://github.com/copyleft-next/copyleft-next/blob/master/Releases/copyleft-next-0.3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/copyleft-next-0.3.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "copyleft-next-0.3.1",
             "name": "copyleft-next 0.3.1",
             "reference": "https://spdx.org/licenses/copyleft-next-0.3.1.html",
-            "referenceNumber": 180,
+            "referenceNumber": 265,
             "seeAlso": [
                 "https://github.com/copyleft-next/copyleft-next/blob/master/Releases/copyleft-next-0.3.1"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Cornell-Lossless-JPEG.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Cornell-Lossless-JPEG",
+            "name": "Cornell Lossless JPEG License",
+            "reference": "https://spdx.org/licenses/Cornell-Lossless-JPEG.html",
+            "referenceNumber": 377,
+            "seeAlso": [
+                "https://android.googlesource.com/platform/external/dng_sdk/+/refs/heads/master/source/dng_lossless_jpeg.cpp#16",
+                "https://www.mssl.ucl.ac.uk/~mcrw/src/20050920/proto.h",
+                "https://gitlab.freedesktop.org/libopenraw/libopenraw/blob/master/lib/ljpegdecompressor.cpp#L32"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/CPAL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "CPAL-1.0",
             "name": "Common Public Attribution License 1.0",
             "reference": "https://spdx.org/licenses/CPAL-1.0.html",
-            "referenceNumber": 86,
+            "referenceNumber": 411,
             "seeAlso": [
                 "https://opensource.org/licenses/CPAL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "CPL-1.0",
             "name": "Common Public License 1.0",
             "reference": "https://spdx.org/licenses/CPL-1.0.html",
-            "referenceNumber": 397,
+            "referenceNumber": 488,
             "seeAlso": [
                 "https://opensource.org/licenses/CPL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CPOL-1.02.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CPOL-1.02",
             "name": "Code Project Open License 1.02",
             "reference": "https://spdx.org/licenses/CPOL-1.02.html",
-            "referenceNumber": 272,
+            "referenceNumber": 381,
             "seeAlso": [
                 "http://www.codeproject.com/info/cpol10.aspx"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Crossword.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Crossword",
             "name": "Crossword License",
             "reference": "https://spdx.org/licenses/Crossword.html",
-            "referenceNumber": 216,
+            "referenceNumber": 229,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Crossword"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CrystalStacker.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CrystalStacker",
             "name": "CrystalStacker License",
             "reference": "https://spdx.org/licenses/CrystalStacker.html",
-            "referenceNumber": 109,
+            "referenceNumber": 104,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing:CrystalStacker?rd=Licensing/CrystalStacker"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CUA-OPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "CUA-OPL-1.0",
             "name": "CUA Office Public License v1.0",
             "reference": "https://spdx.org/licenses/CUA-OPL-1.0.html",
-            "referenceNumber": 183,
+            "referenceNumber": 110,
             "seeAlso": [
                 "https://opensource.org/licenses/CUA-OPL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Cube.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Cube",
             "name": "Cube License",
             "reference": "https://spdx.org/licenses/Cube.html",
-            "referenceNumber": 173,
+            "referenceNumber": 182,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Cube"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/curl.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "curl",
             "name": "curl License",
             "reference": "https://spdx.org/licenses/curl.html",
-            "referenceNumber": 362,
+            "referenceNumber": 332,
             "seeAlso": [
                 "https://github.com/bagder/curl/blob/master/COPYING"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/D-FSL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "D-FSL-1.0",
             "name": "Deutsche Freie Software Lizenz",
             "reference": "https://spdx.org/licenses/D-FSL-1.0.html",
-            "referenceNumber": 468,
+            "referenceNumber": 337,
             "seeAlso": [
                 "http://www.dipp.nrw.de/d-fsl/lizenzen/",
                 "http://www.dipp.nrw.de/d-fsl/index_html/lizenzen/de/D-FSL-1_0_de.txt",
                 "http://www.dipp.nrw.de/d-fsl/index_html/lizenzen/en/D-FSL-1_0_en.txt",
                 "https://www.hbz-nrw.de/produkte/open-access/lizenzen/dfsl",
                 "https://www.hbz-nrw.de/produkte/open-access/lizenzen/dfsl/deutsche-freie-software-lizenz",
                 "https://www.hbz-nrw.de/produkte/open-access/lizenzen/dfsl/german-free-software-license",
@@ -2068,311 +2268,323 @@
         {
             "detailsUrl": "https://spdx.org/licenses/diffmark.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "diffmark",
             "name": "diffmark license",
             "reference": "https://spdx.org/licenses/diffmark.html",
-            "referenceNumber": 187,
+            "referenceNumber": 302,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/diffmark"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/DL-DE-BY-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "DL-DE-BY-2.0",
             "name": "Data licence Germany \u2013 attribution \u2013 version 2.0",
             "reference": "https://spdx.org/licenses/DL-DE-BY-2.0.html",
-            "referenceNumber": 483,
+            "referenceNumber": 93,
             "seeAlso": [
                 "https://www.govdata.de/dl-de/by-2-0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/DOC.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "DOC",
             "name": "DOC License",
             "reference": "https://spdx.org/licenses/DOC.html",
-            "referenceNumber": 412,
+            "referenceNumber": 260,
             "seeAlso": [
                 "http://www.cs.wustl.edu/~schmidt/ACE-copying.html",
                 "https://www.dre.vanderbilt.edu/~schmidt/ACE-copying.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Dotseqn.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Dotseqn",
             "name": "Dotseqn License",
             "reference": "https://spdx.org/licenses/Dotseqn.html",
-            "referenceNumber": 322,
+            "referenceNumber": 98,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Dotseqn"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/DRL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "DRL-1.0",
             "name": "Detection Rule License 1.0",
             "reference": "https://spdx.org/licenses/DRL-1.0.html",
-            "referenceNumber": 168,
+            "referenceNumber": 325,
             "seeAlso": [
                 "https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/DSDP.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "DSDP",
             "name": "DSDP License",
             "reference": "https://spdx.org/licenses/DSDP.html",
-            "referenceNumber": 41,
+            "referenceNumber": 379,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/DSDP"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/dtoa.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "dtoa",
+            "name": "David M. Gay dtoa License",
+            "reference": "https://spdx.org/licenses/dtoa.html",
+            "referenceNumber": 144,
+            "seeAlso": [
+                "https://github.com/SWI-Prolog/swipl-devel/blob/master/src/os/dtoa.c"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/dvipdfm.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "dvipdfm",
             "name": "dvipdfm License",
             "reference": "https://spdx.org/licenses/dvipdfm.html",
-            "referenceNumber": 395,
+            "referenceNumber": 289,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/dvipdfm"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ECL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "ECL-1.0",
             "name": "Educational Community License v1.0",
             "reference": "https://spdx.org/licenses/ECL-1.0.html",
-            "referenceNumber": 404,
+            "referenceNumber": 242,
             "seeAlso": [
                 "https://opensource.org/licenses/ECL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ECL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "ECL-2.0",
             "name": "Educational Community License v2.0",
             "reference": "https://spdx.org/licenses/ECL-2.0.html",
-            "referenceNumber": 476,
+            "referenceNumber": 246,
             "seeAlso": [
                 "https://opensource.org/licenses/ECL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/eCos-2.0.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "eCos-2.0",
             "name": "eCos license version 2.0",
             "reference": "https://spdx.org/licenses/eCos-2.0.html",
-            "referenceNumber": 163,
+            "referenceNumber": 36,
             "seeAlso": [
                 "https://www.gnu.org/licenses/ecos-license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/EFL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "EFL-1.0",
             "name": "Eiffel Forum License v1.0",
             "reference": "https://spdx.org/licenses/EFL-1.0.html",
-            "referenceNumber": 330,
+            "referenceNumber": 485,
             "seeAlso": [
                 "http://www.eiffel-nice.org/license/forum.txt",
                 "https://opensource.org/licenses/EFL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/EFL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "EFL-2.0",
             "name": "Eiffel Forum License v2.0",
             "reference": "https://spdx.org/licenses/EFL-2.0.html",
-            "referenceNumber": 56,
+            "referenceNumber": 436,
             "seeAlso": [
                 "http://www.eiffel-nice.org/license/eiffel-forum-license-2.html",
                 "https://opensource.org/licenses/EFL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/eGenix.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "eGenix",
             "name": "eGenix.com Public License 1.1.0",
             "reference": "https://spdx.org/licenses/eGenix.html",
-            "referenceNumber": 334,
+            "referenceNumber": 165,
             "seeAlso": [
                 "http://www.egenix.com/products/eGenix.com-Public-License-1.1.0.pdf",
                 "https://fedoraproject.org/wiki/Licensing/eGenix.com_Public_License_1.1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Elastic-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Elastic-2.0",
             "name": "Elastic License 2.0",
             "reference": "https://spdx.org/licenses/Elastic-2.0.html",
-            "referenceNumber": 32,
+            "referenceNumber": 547,
             "seeAlso": [
                 "https://www.elastic.co/licensing/elastic-license",
                 "https://github.com/elastic/elasticsearch/blob/master/licenses/ELASTIC-LICENSE-2.0.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Entessa.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Entessa",
             "name": "Entessa Public License v1.0",
             "reference": "https://spdx.org/licenses/Entessa.html",
-            "referenceNumber": 176,
+            "referenceNumber": 89,
             "seeAlso": [
                 "https://opensource.org/licenses/Entessa"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/EPICS.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "EPICS",
             "name": "EPICS Open License",
             "reference": "https://spdx.org/licenses/EPICS.html",
-            "referenceNumber": 398,
+            "referenceNumber": 508,
             "seeAlso": [
                 "https://epics.anl.gov/license/open.php"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/EPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "EPL-1.0",
             "name": "Eclipse Public License 1.0",
             "reference": "https://spdx.org/licenses/EPL-1.0.html",
-            "referenceNumber": 144,
+            "referenceNumber": 388,
             "seeAlso": [
                 "http://www.eclipse.org/legal/epl-v10.html",
                 "https://opensource.org/licenses/EPL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/EPL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "EPL-2.0",
             "name": "Eclipse Public License 2.0",
             "reference": "https://spdx.org/licenses/EPL-2.0.html",
-            "referenceNumber": 425,
+            "referenceNumber": 114,
             "seeAlso": [
                 "https://www.eclipse.org/legal/epl-2.0",
                 "https://www.opensource.org/licenses/EPL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ErlPL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "ErlPL-1.1",
             "name": "Erlang Public License v1.1",
             "reference": "https://spdx.org/licenses/ErlPL-1.1.html",
-            "referenceNumber": 368,
+            "referenceNumber": 239,
             "seeAlso": [
                 "http://www.erlang.org/EPLICENSE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/etalab-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "etalab-2.0",
             "name": "Etalab Open License 2.0",
             "reference": "https://spdx.org/licenses/etalab-2.0.html",
-            "referenceNumber": 394,
+            "referenceNumber": 273,
             "seeAlso": [
                 "https://github.com/DISIC/politique-de-contribution-open-source/blob/master/LICENSE.pdf",
                 "https://raw.githubusercontent.com/DISIC/politique-de-contribution-open-source/master/LICENSE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/EUDatagrid.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "EUDatagrid",
             "name": "EU DataGrid Software License",
             "reference": "https://spdx.org/licenses/EUDatagrid.html",
-            "referenceNumber": 111,
+            "referenceNumber": 29,
             "seeAlso": [
                 "http://eu-datagrid.web.cern.ch/eu-datagrid/license.html",
                 "https://opensource.org/licenses/EUDatagrid"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/EUPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "EUPL-1.0",
             "name": "European Union Public License 1.0",
             "reference": "https://spdx.org/licenses/EUPL-1.0.html",
-            "referenceNumber": 110,
+            "referenceNumber": 363,
             "seeAlso": [
                 "http://ec.europa.eu/idabc/en/document/7330.html",
                 "http://ec.europa.eu/idabc/servlets/Doc027f.pdf?id=31096"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/EUPL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "EUPL-1.1",
             "name": "European Union Public License 1.1",
             "reference": "https://spdx.org/licenses/EUPL-1.1.html",
-            "referenceNumber": 297,
+            "referenceNumber": 108,
             "seeAlso": [
                 "https://joinup.ec.europa.eu/software/page/eupl/licence-eupl",
                 "https://joinup.ec.europa.eu/sites/default/files/custom-page/attachment/eupl1.1.-licence-en_0.pdf",
                 "https://opensource.org/licenses/EUPL-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/EUPL-1.2.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "EUPL-1.2",
             "name": "European Union Public License 1.2",
             "reference": "https://spdx.org/licenses/EUPL-1.2.html",
-            "referenceNumber": 211,
+            "referenceNumber": 164,
             "seeAlso": [
                 "https://joinup.ec.europa.eu/page/eupl-text-11-12",
                 "https://joinup.ec.europa.eu/sites/default/files/custom-page/attachment/eupl_v1.2_en.pdf",
                 "https://joinup.ec.europa.eu/sites/default/files/custom-page/attachment/2020-03/EUPL-1.2%20EN.txt",
                 "https://joinup.ec.europa.eu/sites/default/files/inline-files/EUPL%20v1_2%20EN(1).txt",
                 "http://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:32017D0863",
                 "https://opensource.org/licenses/EUPL-1.2"
@@ -2381,3916 +2593,4419 @@
         {
             "detailsUrl": "https://spdx.org/licenses/Eurosym.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Eurosym",
             "name": "Eurosym License",
             "reference": "https://spdx.org/licenses/Eurosym.html",
-            "referenceNumber": 152,
+            "referenceNumber": 49,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Eurosym"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Fair.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Fair",
             "name": "Fair License",
             "reference": "https://spdx.org/licenses/Fair.html",
-            "referenceNumber": 121,
+            "referenceNumber": 438,
             "seeAlso": [
                 "http://fairlicense.org/",
                 "https://opensource.org/licenses/Fair"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/FDK-AAC.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "FDK-AAC",
             "name": "Fraunhofer FDK AAC Codec Library",
             "reference": "https://spdx.org/licenses/FDK-AAC.html",
-            "referenceNumber": 375,
+            "referenceNumber": 159,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/FDK-AAC",
                 "https://directory.fsf.org/wiki/License:Fdk"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Frameworx-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Frameworx-1.0",
             "name": "Frameworx Open License 1.0",
             "reference": "https://spdx.org/licenses/Frameworx-1.0.html",
-            "referenceNumber": 192,
+            "referenceNumber": 219,
             "seeAlso": [
                 "https://opensource.org/licenses/Frameworx-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/FreeBSD-DOC.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "FreeBSD-DOC",
             "name": "FreeBSD Documentation License",
             "reference": "https://spdx.org/licenses/FreeBSD-DOC.html",
-            "referenceNumber": 401,
+            "referenceNumber": 169,
             "seeAlso": [
                 "https://www.freebsd.org/copyright/freebsd-doc-license/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/FreeImage.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "FreeImage",
             "name": "FreeImage Public License v1.0",
             "reference": "https://spdx.org/licenses/FreeImage.html",
-            "referenceNumber": 67,
+            "referenceNumber": 533,
             "seeAlso": [
                 "http://freeimage.sourceforge.net/freeimage-license.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/FSFAP.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "FSFAP",
             "name": "FSF All Permissive License",
             "reference": "https://spdx.org/licenses/FSFAP.html",
-            "referenceNumber": 202,
+            "referenceNumber": 340,
             "seeAlso": [
                 "https://www.gnu.org/prep/maintain/html_node/License-Notices-for-Other-Files.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/FSFUL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "FSFUL",
             "name": "FSF Unlimited License",
             "reference": "https://spdx.org/licenses/FSFUL.html",
-            "referenceNumber": 199,
+            "referenceNumber": 393,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/FSF_Unlimited_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/FSFULLR.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "FSFULLR",
             "name": "FSF Unlimited License (with License Retention)",
             "reference": "https://spdx.org/licenses/FSFULLR.html",
-            "referenceNumber": 311,
+            "referenceNumber": 528,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/FSF_Unlimited_License#License_Retention_Variant"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/FSFULLRWD.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "FSFULLRWD",
-            "name": "FSF Unlimited License (With License Retention    and Warranty Disclaimer)",
+            "name": "FSF Unlimited License (With License Retention and Warranty Disclaimer)",
             "reference": "https://spdx.org/licenses/FSFULLRWD.html",
-            "referenceNumber": 208,
+            "referenceNumber": 512,
             "seeAlso": [
                 "https://lists.gnu.org/archive/html/autoconf/2012-04/msg00061.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/FTL.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "FTL",
             "name": "Freetype Project License",
             "reference": "https://spdx.org/licenses/FTL.html",
-            "referenceNumber": 239,
+            "referenceNumber": 210,
             "seeAlso": [
                 "http://freetype.fis.uniroma2.it/FTL.TXT",
                 "http://git.savannah.gnu.org/cgit/freetype/freetype2.git/tree/docs/FTL.TXT",
                 "http://gitlab.freedesktop.org/freetype/freetype/-/raw/master/docs/FTL.TXT"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GD.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GD",
             "name": "GD License",
             "reference": "https://spdx.org/licenses/GD.html",
-            "referenceNumber": 371,
+            "referenceNumber": 294,
             "seeAlso": [
                 "https://libgd.github.io/manuals/2.3.0/files/license-txt.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.1.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.1",
             "name": "GNU Free Documentation License v1.1",
             "reference": "https://spdx.org/licenses/GFDL-1.1.html",
-            "referenceNumber": 12,
+            "referenceNumber": 59,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.1.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.1-invariants-only.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.1-invariants-only",
             "name": "GNU Free Documentation License v1.1 only - invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.1-invariants-only.html",
-            "referenceNumber": 72,
+            "referenceNumber": 521,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.1.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.1-invariants-or-later.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.1-invariants-or-later",
             "name": "GNU Free Documentation License v1.1 or later - invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.1-invariants-or-later.html",
-            "referenceNumber": 465,
+            "referenceNumber": 281,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.1.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.1-no-invariants-only.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.1-no-invariants-only",
             "name": "GNU Free Documentation License v1.1 only - no invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.1-no-invariants-only.html",
-            "referenceNumber": 443,
+            "referenceNumber": 132,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.1.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.1-no-invariants-or-later.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.1-no-invariants-or-later",
             "name": "GNU Free Documentation License v1.1 or later - no invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.1-no-invariants-or-later.html",
-            "referenceNumber": 149,
+            "referenceNumber": 391,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.1.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.1-only.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.1-only",
             "name": "GNU Free Documentation License v1.1 only",
             "reference": "https://spdx.org/licenses/GFDL-1.1-only.html",
-            "referenceNumber": 229,
+            "referenceNumber": 10,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.1.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.1-or-later.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.1-or-later",
             "name": "GNU Free Documentation License v1.1 or later",
             "reference": "https://spdx.org/licenses/GFDL-1.1-or-later.html",
-            "referenceNumber": 242,
+            "referenceNumber": 197,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.1.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.2.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.2",
             "name": "GNU Free Documentation License v1.2",
             "reference": "https://spdx.org/licenses/GFDL-1.2.html",
-            "referenceNumber": 453,
+            "referenceNumber": 188,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.2.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.2-invariants-only.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.2-invariants-only",
             "name": "GNU Free Documentation License v1.2 only - invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.2-invariants-only.html",
-            "referenceNumber": 8,
+            "referenceNumber": 200,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.2.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.2-invariants-or-later.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.2-invariants-or-later",
             "name": "GNU Free Documentation License v1.2 or later - invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.2-invariants-or-later.html",
-            "referenceNumber": 230,
+            "referenceNumber": 314,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.2.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.2-no-invariants-only.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.2-no-invariants-only",
             "name": "GNU Free Documentation License v1.2 only - no invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.2-no-invariants-only.html",
-            "referenceNumber": 42,
+            "referenceNumber": 427,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.2.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.2-no-invariants-or-later.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.2-no-invariants-or-later",
             "name": "GNU Free Documentation License v1.2 or later - no invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.2-no-invariants-or-later.html",
-            "referenceNumber": 459,
+            "referenceNumber": 285,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.2.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.2-only.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.2-only",
             "name": "GNU Free Documentation License v1.2 only",
             "reference": "https://spdx.org/licenses/GFDL-1.2-only.html",
-            "referenceNumber": 290,
+            "referenceNumber": 244,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.2.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.2-or-later.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.2-or-later",
             "name": "GNU Free Documentation License v1.2 or later",
             "reference": "https://spdx.org/licenses/GFDL-1.2-or-later.html",
-            "referenceNumber": 274,
+            "referenceNumber": 349,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.2.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.3.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.3",
             "name": "GNU Free Documentation License v1.3",
             "reference": "https://spdx.org/licenses/GFDL-1.3.html",
-            "referenceNumber": 300,
+            "referenceNumber": 437,
             "seeAlso": [
                 "https://www.gnu.org/licenses/fdl-1.3.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.3-invariants-only.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.3-invariants-only",
             "name": "GNU Free Documentation License v1.3 only - invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.3-invariants-only.html",
-            "referenceNumber": 0,
+            "referenceNumber": 38,
             "seeAlso": [
                 "https://www.gnu.org/licenses/fdl-1.3.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.3-invariants-or-later.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.3-invariants-or-later",
             "name": "GNU Free Documentation License v1.3 or later - invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.3-invariants-or-later.html",
-            "referenceNumber": 234,
+            "referenceNumber": 406,
             "seeAlso": [
                 "https://www.gnu.org/licenses/fdl-1.3.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.3-no-invariants-only.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.3-no-invariants-only",
             "name": "GNU Free Documentation License v1.3 only - no invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.3-no-invariants-only.html",
-            "referenceNumber": 289,
+            "referenceNumber": 249,
             "seeAlso": [
                 "https://www.gnu.org/licenses/fdl-1.3.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.3-no-invariants-or-later.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.3-no-invariants-or-later",
             "name": "GNU Free Documentation License v1.3 or later - no invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.3-no-invariants-or-later.html",
-            "referenceNumber": 151,
+            "referenceNumber": 523,
             "seeAlso": [
                 "https://www.gnu.org/licenses/fdl-1.3.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.3-only.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.3-only",
             "name": "GNU Free Documentation License v1.3 only",
             "reference": "https://spdx.org/licenses/GFDL-1.3-only.html",
-            "referenceNumber": 450,
+            "referenceNumber": 258,
             "seeAlso": [
                 "https://www.gnu.org/licenses/fdl-1.3.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.3-or-later.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.3-or-later",
             "name": "GNU Free Documentation License v1.3 or later",
             "reference": "https://spdx.org/licenses/GFDL-1.3-or-later.html",
-            "referenceNumber": 343,
+            "referenceNumber": 336,
             "seeAlso": [
                 "https://www.gnu.org/licenses/fdl-1.3.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Giftware.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Giftware",
             "name": "Giftware License",
             "reference": "https://spdx.org/licenses/Giftware.html",
-            "referenceNumber": 85,
+            "referenceNumber": 331,
             "seeAlso": [
                 "http://liballeg.org/license.html#allegro-4-the-giftware-license"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GL2PS.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GL2PS",
             "name": "GL2PS License",
             "reference": "https://spdx.org/licenses/GL2PS.html",
-            "referenceNumber": 106,
+            "referenceNumber": 461,
             "seeAlso": [
                 "http://www.geuz.org/gl2ps/COPYING.GL2PS"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Glide.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Glide",
             "name": "3dfx Glide License",
             "reference": "https://spdx.org/licenses/Glide.html",
-            "referenceNumber": 222,
+            "referenceNumber": 353,
             "seeAlso": [
                 "http://www.users.on.net/~triforce/glidexp/COPYING.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Glulxe.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Glulxe",
             "name": "Glulxe License",
             "reference": "https://spdx.org/licenses/Glulxe.html",
-            "referenceNumber": 190,
+            "referenceNumber": 530,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Glulxe"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GLWTPL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GLWTPL",
             "name": "Good Luck With That Public License",
             "reference": "https://spdx.org/licenses/GLWTPL.html",
-            "referenceNumber": 15,
+            "referenceNumber": 318,
             "seeAlso": [
                 "https://github.com/me-shaon/GLWTPL/commit/da5f6bc734095efbacb442c0b31e33a65b9d6e85"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/gnuplot.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "gnuplot",
             "name": "gnuplot License",
             "reference": "https://spdx.org/licenses/gnuplot.html",
-            "referenceNumber": 84,
+            "referenceNumber": 455,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Gnuplot"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-1.0.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": false,
             "licenseId": "GPL-1.0",
             "name": "GNU General Public License v1.0 only",
             "reference": "https://spdx.org/licenses/GPL-1.0.html",
-            "referenceNumber": 439,
+            "referenceNumber": 212,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/gpl-1.0-standalone.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-1.0+.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": false,
             "licenseId": "GPL-1.0+",
             "name": "GNU General Public License v1.0 or later",
             "reference": "https://spdx.org/licenses/GPL-1.0+.html",
-            "referenceNumber": 135,
+            "referenceNumber": 220,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/gpl-1.0-standalone.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-1.0-only.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GPL-1.0-only",
             "name": "GNU General Public License v1.0 only",
             "reference": "https://spdx.org/licenses/GPL-1.0-only.html",
-            "referenceNumber": 293,
+            "referenceNumber": 235,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/gpl-1.0-standalone.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-1.0-or-later.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GPL-1.0-or-later",
             "name": "GNU General Public License v1.0 or later",
             "reference": "https://spdx.org/licenses/GPL-1.0-or-later.html",
-            "referenceNumber": 39,
+            "referenceNumber": 85,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/gpl-1.0-standalone.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-2.0.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "GPL-2.0",
             "name": "GNU General Public License v2.0 only",
             "reference": "https://spdx.org/licenses/GPL-2.0.html",
-            "referenceNumber": 478,
+            "referenceNumber": 1,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/gpl-2.0-standalone.html",
                 "https://opensource.org/licenses/GPL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-2.0+.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "GPL-2.0+",
             "name": "GNU General Public License v2.0 or later",
             "reference": "https://spdx.org/licenses/GPL-2.0+.html",
-            "referenceNumber": 134,
+            "referenceNumber": 499,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/gpl-2.0-standalone.html",
                 "https://opensource.org/licenses/GPL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-2.0-only.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "GPL-2.0-only",
             "name": "GNU General Public License v2.0 only",
             "reference": "https://spdx.org/licenses/GPL-2.0-only.html",
-            "referenceNumber": 265,
+            "referenceNumber": 439,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/gpl-2.0-standalone.html",
                 "https://opensource.org/licenses/GPL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-2.0-or-later.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "GPL-2.0-or-later",
             "name": "GNU General Public License v2.0 or later",
             "reference": "https://spdx.org/licenses/GPL-2.0-or-later.html",
-            "referenceNumber": 62,
+            "referenceNumber": 16,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/gpl-2.0-standalone.html",
                 "https://opensource.org/licenses/GPL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-2.0-with-autoconf-exception.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": false,
             "licenseId": "GPL-2.0-with-autoconf-exception",
             "name": "GNU General Public License v2.0 w/Autoconf exception",
             "reference": "https://spdx.org/licenses/GPL-2.0-with-autoconf-exception.html",
-            "referenceNumber": 384,
+            "referenceNumber": 296,
             "seeAlso": [
                 "http://ac-archive.sourceforge.net/doc/copyright.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-2.0-with-bison-exception.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": false,
             "licenseId": "GPL-2.0-with-bison-exception",
             "name": "GNU General Public License v2.0 w/Bison exception",
             "reference": "https://spdx.org/licenses/GPL-2.0-with-bison-exception.html",
-            "referenceNumber": 247,
+            "referenceNumber": 68,
             "seeAlso": [
                 "http://git.savannah.gnu.org/cgit/bison.git/tree/data/yacc.c?id=193d7c7054ba7197b0789e14965b739162319b5e#n141"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-2.0-with-classpath-exception.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": false,
             "licenseId": "GPL-2.0-with-classpath-exception",
             "name": "GNU General Public License v2.0 w/Classpath exception",
             "reference": "https://spdx.org/licenses/GPL-2.0-with-classpath-exception.html",
-            "referenceNumber": 288,
+            "referenceNumber": 261,
             "seeAlso": [
                 "https://www.gnu.org/software/classpath/license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-2.0-with-font-exception.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": false,
             "licenseId": "GPL-2.0-with-font-exception",
             "name": "GNU General Public License v2.0 w/Font exception",
             "reference": "https://spdx.org/licenses/GPL-2.0-with-font-exception.html",
-            "referenceNumber": 171,
+            "referenceNumber": 87,
             "seeAlso": [
                 "https://www.gnu.org/licenses/gpl-faq.html#FontException"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-2.0-with-GCC-exception.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": false,
             "licenseId": "GPL-2.0-with-GCC-exception",
             "name": "GNU General Public License v2.0 w/GCC Runtime Library exception",
             "reference": "https://spdx.org/licenses/GPL-2.0-with-GCC-exception.html",
-            "referenceNumber": 354,
+            "referenceNumber": 468,
             "seeAlso": [
                 "https://gcc.gnu.org/git/?p=gcc.git;a=blob;f=gcc/libgcc1.c;h=762f5143fc6eed57b6797c82710f3538aa52b40b;hb=cb143a3ce4fb417c68f5fa2691a1b1b1053dfba9#l10"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-3.0.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "GPL-3.0",
             "name": "GNU General Public License v3.0 only",
             "reference": "https://spdx.org/licenses/GPL-3.0.html",
-            "referenceNumber": 78,
+            "referenceNumber": 55,
             "seeAlso": [
                 "https://www.gnu.org/licenses/gpl-3.0-standalone.html",
                 "https://opensource.org/licenses/GPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-3.0+.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "GPL-3.0+",
             "name": "GNU General Public License v3.0 or later",
             "reference": "https://spdx.org/licenses/GPL-3.0+.html",
-            "referenceNumber": 286,
+            "referenceNumber": 146,
             "seeAlso": [
                 "https://www.gnu.org/licenses/gpl-3.0-standalone.html",
                 "https://opensource.org/licenses/GPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-3.0-only.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "GPL-3.0-only",
             "name": "GNU General Public License v3.0 only",
             "reference": "https://spdx.org/licenses/GPL-3.0-only.html",
-            "referenceNumber": 332,
+            "referenceNumber": 184,
             "seeAlso": [
                 "https://www.gnu.org/licenses/gpl-3.0-standalone.html",
                 "https://opensource.org/licenses/GPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-3.0-or-later.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "GPL-3.0-or-later",
             "name": "GNU General Public License v3.0 or later",
             "reference": "https://spdx.org/licenses/GPL-3.0-or-later.html",
-            "referenceNumber": 486,
+            "referenceNumber": 425,
             "seeAlso": [
                 "https://www.gnu.org/licenses/gpl-3.0-standalone.html",
                 "https://opensource.org/licenses/GPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-3.0-with-autoconf-exception.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": false,
             "licenseId": "GPL-3.0-with-autoconf-exception",
             "name": "GNU General Public License v3.0 w/Autoconf exception",
             "reference": "https://spdx.org/licenses/GPL-3.0-with-autoconf-exception.html",
-            "referenceNumber": 91,
+            "referenceNumber": 484,
             "seeAlso": [
                 "https://www.gnu.org/licenses/autoconf-exception-3.0.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-3.0-with-GCC-exception.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": true,
             "licenseId": "GPL-3.0-with-GCC-exception",
             "name": "GNU General Public License v3.0 w/GCC Runtime Library exception",
             "reference": "https://spdx.org/licenses/GPL-3.0-with-GCC-exception.html",
-            "referenceNumber": 80,
+            "referenceNumber": 446,
             "seeAlso": [
                 "https://www.gnu.org/licenses/gcc-exception-3.1.html"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Graphics-Gems.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Graphics-Gems",
+            "name": "Graphics Gems License",
+            "reference": "https://spdx.org/licenses/Graphics-Gems.html",
+            "referenceNumber": 315,
+            "seeAlso": [
+                "https://github.com/erich666/GraphicsGems/blob/master/LICENSE.md"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/gSOAP-1.3b.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "gSOAP-1.3b",
             "name": "gSOAP Public License v1.3b",
             "reference": "https://spdx.org/licenses/gSOAP-1.3b.html",
-            "referenceNumber": 496,
+            "referenceNumber": 550,
             "seeAlso": [
                 "http://www.cs.fsu.edu/~engelen/license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/HaskellReport.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "HaskellReport",
             "name": "Haskell Language Report License",
             "reference": "https://spdx.org/licenses/HaskellReport.html",
-            "referenceNumber": 5,
+            "referenceNumber": 135,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Haskell_Language_Report_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Hippocratic-2.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Hippocratic-2.1",
             "name": "Hippocratic License 2.1",
             "reference": "https://spdx.org/licenses/Hippocratic-2.1.html",
-            "referenceNumber": 19,
+            "referenceNumber": 5,
             "seeAlso": [
                 "https://firstdonoharm.dev/version/2/1/license.html",
                 "https://github.com/EthicalSource/hippocratic-license/blob/58c0e646d64ff6fbee275bfe2b9492f914e3ab2a/LICENSE.txt"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/HP-1986.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "HP-1986",
+            "name": "Hewlett-Packard 1986 License",
+            "reference": "https://spdx.org/licenses/HP-1986.html",
+            "referenceNumber": 96,
+            "seeAlso": [
+                "https://sourceware.org/git/?p=newlib-cygwin.git;a=blob;f=newlib/libc/machine/hppa/memchr.S;h=1cca3e5e8867aa4bffef1f75a5c1bba25c0c441e;hb=HEAD#l2"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/HPND.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "HPND",
             "name": "Historical Permission Notice and Disclaimer",
             "reference": "https://spdx.org/licenses/HPND.html",
-            "referenceNumber": 285,
+            "referenceNumber": 172,
             "seeAlso": [
                 "https://opensource.org/licenses/HPND"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/HPND-export-US.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "HPND-export-US",
+            "name": "HPND with US Government export control warning",
+            "reference": "https://spdx.org/licenses/HPND-export-US.html",
+            "referenceNumber": 275,
+            "seeAlso": [
+                "https://www.kermitproject.org/ck90.html#source"
+            ]
+        },
+        {
+            "detailsUrl": "https://spdx.org/licenses/HPND-Markus-Kuhn.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "HPND-Markus-Kuhn",
+            "name": "Historical Permission Notice and Disclaimer - Markus Kuhn variant",
+            "reference": "https://spdx.org/licenses/HPND-Markus-Kuhn.html",
+            "referenceNumber": 118,
+            "seeAlso": [
+                "https://www.cl.cam.ac.uk/~mgk25/ucs/wcwidth.c",
+                "https://sourceware.org/git/?p=binutils-gdb.git;a=blob;f=readline/readline/support/wcwidth.c;h=0f5ec995796f4813abbcf4972aec0378ab74722a;hb=HEAD#l55"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/HPND-sell-variant.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "HPND-sell-variant",
             "name": "Historical Permission Notice and Disclaimer - sell variant",
             "reference": "https://spdx.org/licenses/HPND-sell-variant.html",
-            "referenceNumber": 335,
+            "referenceNumber": 424,
             "seeAlso": [
                 "https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/tree/net/sunrpc/auth_gss/gss_generic_token.c?h=v4.19"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/HPND-sell-variant-MIT-disclaimer.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "HPND-sell-variant-MIT-disclaimer",
+            "name": "HPND sell variant with MIT disclaimer",
+            "reference": "https://spdx.org/licenses/HPND-sell-variant-MIT-disclaimer.html",
+            "referenceNumber": 103,
+            "seeAlso": [
+                "https://github.com/sigmavirus24/x11-ssh-askpass/blob/master/README"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/HTMLTIDY.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "HTMLTIDY",
             "name": "HTML Tidy License",
             "reference": "https://spdx.org/licenses/HTMLTIDY.html",
-            "referenceNumber": 361,
+            "referenceNumber": 535,
             "seeAlso": [
                 "https://github.com/htacg/tidy-html5/blob/next/README/LICENSE.md"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/IBM-pibs.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "IBM-pibs",
             "name": "IBM PowerPC Initialization and Boot Software",
             "reference": "https://spdx.org/licenses/IBM-pibs.html",
-            "referenceNumber": 16,
+            "referenceNumber": 99,
             "seeAlso": [
                 "http://git.denx.de/?p=u-boot.git;a=blob;f=arch/powerpc/cpu/ppc4xx/miiphy.c;h=297155fdafa064b955e53e9832de93bfb0cfb85b;hb=9fab4bf4cc077c21e43941866f3f2c196f28670d"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ICU.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "ICU",
             "name": "ICU License",
             "reference": "https://spdx.org/licenses/ICU.html",
-            "referenceNumber": 366,
+            "referenceNumber": 254,
             "seeAlso": [
                 "http://source.icu-project.org/repos/icu/icu/trunk/license.html"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/IEC-Code-Components-EULA.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "IEC-Code-Components-EULA",
+            "name": "IEC    Code Components End-user licence agreement",
+            "reference": "https://spdx.org/licenses/IEC-Code-Components-EULA.html",
+            "referenceNumber": 546,
+            "seeAlso": [
+                "https://www.iec.ch/webstore/custserv/pdf/CC-EULA.pdf",
+                "https://www.iec.ch/CCv1",
+                "https://www.iec.ch/copyright"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/IJG.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "IJG",
             "name": "Independent JPEG Group License",
             "reference": "https://spdx.org/licenses/IJG.html",
-            "referenceNumber": 87,
+            "referenceNumber": 109,
             "seeAlso": [
                 "http://dev.w3.org/cvsweb/Amaya/libjpeg/Attic/README?rev=1.2"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/IJG-short.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "IJG-short",
+            "name": "Independent JPEG Group License - short",
+            "reference": "https://spdx.org/licenses/IJG-short.html",
+            "referenceNumber": 374,
+            "seeAlso": [
+                "https://sourceforge.net/p/xmedcon/code/ci/master/tree/libs/ljpg/"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/ImageMagick.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "ImageMagick",
             "name": "ImageMagick License",
             "reference": "https://spdx.org/licenses/ImageMagick.html",
-            "referenceNumber": 435,
+            "referenceNumber": 287,
             "seeAlso": [
                 "http://www.imagemagick.org/script/license.php"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/iMatix.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "iMatix",
             "name": "iMatix Standard Function Library Agreement",
             "reference": "https://spdx.org/licenses/iMatix.html",
-            "referenceNumber": 275,
+            "referenceNumber": 430,
             "seeAlso": [
                 "http://legacy.imatix.com/html/sfl/sfl4.htm#license"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Imlib2.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "Imlib2",
             "name": "Imlib2 License",
             "reference": "https://spdx.org/licenses/Imlib2.html",
-            "referenceNumber": 474,
+            "referenceNumber": 477,
             "seeAlso": [
                 "http://trac.enlightenment.org/e/browser/trunk/imlib2/COPYING",
                 "https://git.enlightenment.org/legacy/imlib2.git/tree/COPYING"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Info-ZIP.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Info-ZIP",
             "name": "Info-ZIP License",
             "reference": "https://spdx.org/licenses/Info-ZIP.html",
-            "referenceNumber": 447,
+            "referenceNumber": 361,
             "seeAlso": [
                 "http://www.info-zip.org/license.html"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Inner-Net-2.0.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Inner-Net-2.0",
+            "name": "Inner Net License v2.0",
+            "reference": "https://spdx.org/licenses/Inner-Net-2.0.html",
+            "referenceNumber": 240,
+            "seeAlso": [
+                "https://fedoraproject.org/wiki/Licensing/Inner_Net_License",
+                "https://sourceware.org/git/?p=glibc.git;a=blob;f=LICENSES;h=530893b1dc9ea00755603c68fb36bd4fc38a7be8;hb=HEAD#l207"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Intel.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "Intel",
             "name": "Intel Open Source License",
             "reference": "https://spdx.org/licenses/Intel.html",
-            "referenceNumber": 137,
+            "referenceNumber": 486,
             "seeAlso": [
                 "https://opensource.org/licenses/Intel"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Intel-ACPI.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Intel-ACPI",
             "name": "Intel ACPI Software License Agreement",
             "reference": "https://spdx.org/licenses/Intel-ACPI.html",
-            "referenceNumber": 128,
+            "referenceNumber": 65,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Intel_ACPI_Software_License_Agreement"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Interbase-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Interbase-1.0",
             "name": "Interbase Public License v1.0",
             "reference": "https://spdx.org/licenses/Interbase-1.0.html",
-            "referenceNumber": 494,
+            "referenceNumber": 307,
             "seeAlso": [
                 "https://web.archive.org/web/20060319014854/http://info.borland.com/devsupport/interbase/opensource/IPL.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/IPA.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "IPA",
             "name": "IPA Font License",
             "reference": "https://spdx.org/licenses/IPA.html",
-            "referenceNumber": 238,
+            "referenceNumber": 383,
             "seeAlso": [
                 "https://opensource.org/licenses/IPA"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/IPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "IPL-1.0",
             "name": "IBM Public License v1.0",
             "reference": "https://spdx.org/licenses/IPL-1.0.html",
-            "referenceNumber": 324,
+            "referenceNumber": 221,
             "seeAlso": [
                 "https://opensource.org/licenses/IPL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ISC.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "ISC",
             "name": "ISC License",
             "reference": "https://spdx.org/licenses/ISC.html",
-            "referenceNumber": 363,
+            "referenceNumber": 264,
             "seeAlso": [
                 "https://www.isc.org/licenses/",
                 "https://www.isc.org/downloads/software-support-policy/isc-license/",
                 "https://opensource.org/licenses/ISC"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Jam.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Jam",
             "name": "Jam License",
             "reference": "https://spdx.org/licenses/Jam.html",
-            "referenceNumber": 18,
+            "referenceNumber": 445,
             "seeAlso": [
                 "https://www.boost.org/doc/libs/1_35_0/doc/html/jam.html",
                 "https://web.archive.org/web/20160330173339/https://swarm.workshop.perforce.com/files/guest/perforce_software/jam/src/README"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/JasPer-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "JasPer-2.0",
             "name": "JasPer License",
             "reference": "https://spdx.org/licenses/JasPer-2.0.html",
-            "referenceNumber": 105,
+            "referenceNumber": 538,
             "seeAlso": [
                 "http://www.ece.uvic.ca/~mdadams/jasper/LICENSE"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/JPL-image.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "JPL-image",
+            "name": "JPL Image Use Policy",
+            "reference": "https://spdx.org/licenses/JPL-image.html",
+            "referenceNumber": 91,
+            "seeAlso": [
+                "https://www.jpl.nasa.gov/jpl-image-use-policy"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/JPNIC.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "JPNIC",
             "name": "Japan Network Information Center License",
             "reference": "https://spdx.org/licenses/JPNIC.html",
-            "referenceNumber": 73,
+            "referenceNumber": 52,
             "seeAlso": [
                 "https://gitlab.isc.org/isc-projects/bind9/blob/master/COPYRIGHT#L366"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/JSON.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "JSON",
             "name": "JSON License",
             "reference": "https://spdx.org/licenses/JSON.html",
-            "referenceNumber": 353,
+            "referenceNumber": 543,
             "seeAlso": [
                 "http://www.json.org/license.html"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Kazlib.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Kazlib",
+            "name": "Kazlib License",
+            "reference": "https://spdx.org/licenses/Kazlib.html",
+            "referenceNumber": 233,
+            "seeAlso": [
+                "http://git.savannah.gnu.org/cgit/kazlib.git/tree/except.c?id=0062df360c2d17d57f6af19b0e444c51feb99036"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Knuth-CTAN.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Knuth-CTAN",
             "name": "Knuth CTAN License",
             "reference": "https://spdx.org/licenses/Knuth-CTAN.html",
-            "referenceNumber": 345,
+            "referenceNumber": 225,
             "seeAlso": [
                 "https://ctan.org/license/knuth"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LAL-1.2.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "LAL-1.2",
             "name": "Licence Art Libre 1.2",
             "reference": "https://spdx.org/licenses/LAL-1.2.html",
-            "referenceNumber": 284,
+            "referenceNumber": 176,
             "seeAlso": [
                 "http://artlibre.org/licence/lal/licence-art-libre-12/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LAL-1.3.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "LAL-1.3",
             "name": "Licence Art Libre 1.3",
             "reference": "https://spdx.org/licenses/LAL-1.3.html",
-            "referenceNumber": 131,
+            "referenceNumber": 513,
             "seeAlso": [
                 "https://artlibre.org/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Latex2e.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Latex2e",
             "name": "Latex2e License",
             "reference": "https://spdx.org/licenses/Latex2e.html",
-            "referenceNumber": 214,
+            "referenceNumber": 299,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Latex2e"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Latex2e-translated-notice.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Latex2e-translated-notice",
+            "name": "Latex2e with translated notice permission",
+            "reference": "https://spdx.org/licenses/Latex2e-translated-notice.html",
+            "referenceNumber": 24,
+            "seeAlso": [
+                "https://git.savannah.gnu.org/cgit/indent.git/tree/doc/indent.texi?id=a74c6b4ee49397cf330b333da1042bffa60ed14f#n74"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Leptonica.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Leptonica",
             "name": "Leptonica License",
             "reference": "https://spdx.org/licenses/Leptonica.html",
-            "referenceNumber": 473,
+            "referenceNumber": 206,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Leptonica"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-2.0.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": true,
             "licenseId": "LGPL-2.0",
             "name": "GNU Library General Public License v2 only",
             "reference": "https://spdx.org/licenses/LGPL-2.0.html",
-            "referenceNumber": 492,
+            "referenceNumber": 500,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/lgpl-2.0-standalone.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-2.0+.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": true,
             "licenseId": "LGPL-2.0+",
             "name": "GNU Library General Public License v2 or later",
             "reference": "https://spdx.org/licenses/LGPL-2.0+.html",
-            "referenceNumber": 37,
+            "referenceNumber": 81,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/lgpl-2.0-standalone.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-2.0-only.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "LGPL-2.0-only",
             "name": "GNU Library General Public License v2 only",
             "reference": "https://spdx.org/licenses/LGPL-2.0-only.html",
-            "referenceNumber": 61,
+            "referenceNumber": 18,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/lgpl-2.0-standalone.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-2.0-or-later.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "LGPL-2.0-or-later",
             "name": "GNU Library General Public License v2 or later",
             "reference": "https://spdx.org/licenses/LGPL-2.0-or-later.html",
-            "referenceNumber": 431,
+            "referenceNumber": 350,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/lgpl-2.0-standalone.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-2.1.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "LGPL-2.1",
             "name": "GNU Lesser General Public License v2.1 only",
             "reference": "https://spdx.org/licenses/LGPL-2.1.html",
-            "referenceNumber": 388,
+            "referenceNumber": 556,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/lgpl-2.1-standalone.html",
                 "https://opensource.org/licenses/LGPL-2.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-2.1+.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "LGPL-2.1+",
-            "name": "GNU Library General Public License v2.1 or later",
+            "name": "GNU Lesser General Public License v2.1 or later",
             "reference": "https://spdx.org/licenses/LGPL-2.1+.html",
-            "referenceNumber": 145,
+            "referenceNumber": 198,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/lgpl-2.1-standalone.html",
                 "https://opensource.org/licenses/LGPL-2.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-2.1-only.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "LGPL-2.1-only",
             "name": "GNU Lesser General Public License v2.1 only",
             "reference": "https://spdx.org/licenses/LGPL-2.1-only.html",
-            "referenceNumber": 340,
+            "referenceNumber": 359,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/lgpl-2.1-standalone.html",
                 "https://opensource.org/licenses/LGPL-2.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-2.1-or-later.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "LGPL-2.1-or-later",
             "name": "GNU Lesser General Public License v2.1 or later",
             "reference": "https://spdx.org/licenses/LGPL-2.1-or-later.html",
-            "referenceNumber": 360,
+            "referenceNumber": 66,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/lgpl-2.1-standalone.html",
                 "https://opensource.org/licenses/LGPL-2.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-3.0.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "LGPL-3.0",
             "name": "GNU Lesser General Public License v3.0 only",
             "reference": "https://spdx.org/licenses/LGPL-3.0.html",
-            "referenceNumber": 101,
+            "referenceNumber": 551,
             "seeAlso": [
                 "https://www.gnu.org/licenses/lgpl-3.0-standalone.html",
                 "https://www.gnu.org/licenses/lgpl+gpl-3.0.txt",
                 "https://opensource.org/licenses/LGPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-3.0+.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "LGPL-3.0+",
             "name": "GNU Lesser General Public License v3.0 or later",
             "reference": "https://spdx.org/licenses/LGPL-3.0+.html",
-            "referenceNumber": 100,
+            "referenceNumber": 232,
             "seeAlso": [
                 "https://www.gnu.org/licenses/lgpl-3.0-standalone.html",
                 "https://www.gnu.org/licenses/lgpl+gpl-3.0.txt",
                 "https://opensource.org/licenses/LGPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-3.0-only.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "LGPL-3.0-only",
             "name": "GNU Lesser General Public License v3.0 only",
             "reference": "https://spdx.org/licenses/LGPL-3.0-only.html",
-            "referenceNumber": 156,
+            "referenceNumber": 12,
             "seeAlso": [
                 "https://www.gnu.org/licenses/lgpl-3.0-standalone.html",
                 "https://www.gnu.org/licenses/lgpl+gpl-3.0.txt",
                 "https://opensource.org/licenses/LGPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-3.0-or-later.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "LGPL-3.0-or-later",
             "name": "GNU Lesser General Public License v3.0 or later",
             "reference": "https://spdx.org/licenses/LGPL-3.0-or-later.html",
-            "referenceNumber": 196,
+            "referenceNumber": 297,
             "seeAlso": [
                 "https://www.gnu.org/licenses/lgpl-3.0-standalone.html",
                 "https://www.gnu.org/licenses/lgpl+gpl-3.0.txt",
                 "https://opensource.org/licenses/LGPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPLLR.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "LGPLLR",
             "name": "Lesser General Public License For Linguistic Resources",
             "reference": "https://spdx.org/licenses/LGPLLR.html",
-            "referenceNumber": 328,
+            "referenceNumber": 50,
             "seeAlso": [
                 "http://www-igm.univ-mlv.fr/~unitex/lgpllr.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Libpng.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Libpng",
             "name": "libpng License",
             "reference": "https://spdx.org/licenses/Libpng.html",
-            "referenceNumber": 452,
+            "referenceNumber": 26,
             "seeAlso": [
                 "http://www.libpng.org/pub/png/src/libpng-LICENSE.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/libpng-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "libpng-2.0",
             "name": "PNG Reference Library version 2",
             "reference": "https://spdx.org/licenses/libpng-2.0.html",
-            "referenceNumber": 250,
+            "referenceNumber": 453,
             "seeAlso": [
                 "http://www.libpng.org/pub/png/src/libpng-LICENSE.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/libselinux-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "libselinux-1.0",
             "name": "libselinux public domain notice",
             "reference": "https://spdx.org/licenses/libselinux-1.0.html",
-            "referenceNumber": 268,
+            "referenceNumber": 507,
             "seeAlso": [
                 "https://github.com/SELinuxProject/selinux/blob/master/libselinux/LICENSE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/libtiff.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "libtiff",
             "name": "libtiff License",
             "reference": "https://spdx.org/licenses/libtiff.html",
-            "referenceNumber": 186,
+            "referenceNumber": 228,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/libtiff"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/libutil-David-Nugent.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "libutil-David-Nugent",
             "name": "libutil David Nugent License",
             "reference": "https://spdx.org/licenses/libutil-David-Nugent.html",
-            "referenceNumber": 464,
+            "referenceNumber": 531,
             "seeAlso": [
                 "http://web.mit.edu/freebsd/head/lib/libutil/login_ok.3",
                 "https://cgit.freedesktop.org/libbsd/tree/man/setproctitle.3bsd"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LiLiQ-P-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "LiLiQ-P-1.1",
             "name": "Licence Libre du Qu\u00e9bec \u2013 Permissive version 1.1",
             "reference": "https://spdx.org/licenses/LiLiQ-P-1.1.html",
-            "referenceNumber": 169,
+            "referenceNumber": 47,
             "seeAlso": [
                 "https://forge.gouv.qc.ca/licence/fr/liliq-v1-1/",
                 "http://opensource.org/licenses/LiLiQ-P-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LiLiQ-R-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "LiLiQ-R-1.1",
             "name": "Licence Libre du Qu\u00e9bec \u2013 R\u00e9ciprocit\u00e9 version 1.1",
             "reference": "https://spdx.org/licenses/LiLiQ-R-1.1.html",
-            "referenceNumber": 296,
+            "referenceNumber": 418,
             "seeAlso": [
                 "https://www.forge.gouv.qc.ca/participez/licence-logicielle/licence-libre-du-quebec-liliq-en-francais/licence-libre-du-quebec-reciprocite-liliq-r-v1-1/",
                 "http://opensource.org/licenses/LiLiQ-R-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LiLiQ-Rplus-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "LiLiQ-Rplus-1.1",
             "name": "Licence Libre du Qu\u00e9bec \u2013 R\u00e9ciprocit\u00e9 forte version 1.1",
             "reference": "https://spdx.org/licenses/LiLiQ-Rplus-1.1.html",
-            "referenceNumber": 306,
+            "referenceNumber": 286,
             "seeAlso": [
                 "https://www.forge.gouv.qc.ca/participez/licence-logicielle/licence-libre-du-quebec-liliq-en-francais/licence-libre-du-quebec-reciprocite-forte-liliq-r-v1-1/",
                 "http://opensource.org/licenses/LiLiQ-Rplus-1.1"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Linux-man-pages-1-para.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Linux-man-pages-1-para",
+            "name": "Linux man-pages - 1 paragraph",
+            "reference": "https://spdx.org/licenses/Linux-man-pages-1-para.html",
+            "referenceNumber": 409,
+            "seeAlso": [
+                "https://git.kernel.org/pub/scm/docs/man-pages/man-pages.git/tree/man2/getcpu.2#n4"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Linux-man-pages-copyleft.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Linux-man-pages-copyleft",
             "name": "Linux man-pages Copyleft",
             "reference": "https://spdx.org/licenses/Linux-man-pages-copyleft.html",
-            "referenceNumber": 40,
+            "referenceNumber": 463,
             "seeAlso": [
                 "https://www.kernel.org/doc/man-pages/licenses.html"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Linux-man-pages-copyleft-2-para.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Linux-man-pages-copyleft-2-para",
+            "name": "Linux man-pages Copyleft - 2 paragraphs",
+            "reference": "https://spdx.org/licenses/Linux-man-pages-copyleft-2-para.html",
+            "referenceNumber": 168,
+            "seeAlso": [
+                "https://git.kernel.org/pub/scm/docs/man-pages/man-pages.git/tree/man2/move_pages.2#n5",
+                "https://git.kernel.org/pub/scm/docs/man-pages/man-pages.git/tree/man2/migrate_pages.2#n8"
+            ]
+        },
+        {
+            "detailsUrl": "https://spdx.org/licenses/Linux-man-pages-copyleft-var.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Linux-man-pages-copyleft-var",
+            "name": "Linux man-pages Copyleft Variant",
+            "reference": "https://spdx.org/licenses/Linux-man-pages-copyleft-var.html",
+            "referenceNumber": 400,
+            "seeAlso": [
+                "https://git.kernel.org/pub/scm/docs/man-pages/man-pages.git/tree/man2/set_mempolicy.2#n5"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Linux-OpenIB.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Linux-OpenIB",
             "name": "Linux Kernel Variant of OpenIB.org license",
             "reference": "https://spdx.org/licenses/Linux-OpenIB.html",
-            "referenceNumber": 455,
+            "referenceNumber": 31,
             "seeAlso": [
                 "https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/tree/drivers/infiniband/core/sa.h"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/LOOP.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "LOOP",
+            "name": "Common Lisp LOOP License",
+            "reference": "https://spdx.org/licenses/LOOP.html",
+            "referenceNumber": 358,
+            "seeAlso": [
+                "https://gitlab.com/embeddable-common-lisp/ecl/-/blob/develop/src/lsp/loop.lsp",
+                "http://git.savannah.gnu.org/cgit/gcl.git/tree/gcl/lsp/gcl_loop.lsp?h=Version_2_6_13pre",
+                "https://sourceforge.net/p/sbcl/sbcl/ci/master/tree/src/code/loop.lisp",
+                "https://github.com/cl-adams/adams/blob/master/LICENSE.md",
+                "https://github.com/blakemcbride/eclipse-lisp/blob/master/lisp/loop.lisp",
+                "https://gitlab.common-lisp.net/cmucl/cmucl/-/blob/master/src/code/loop.lisp"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/LPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "LPL-1.0",
             "name": "Lucent Public License Version 1.0",
             "reference": "https://spdx.org/licenses/LPL-1.0.html",
-            "referenceNumber": 308,
+            "referenceNumber": 102,
             "seeAlso": [
                 "https://opensource.org/licenses/LPL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LPL-1.02.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "LPL-1.02",
             "name": "Lucent Public License v1.02",
             "reference": "https://spdx.org/licenses/LPL-1.02.html",
-            "referenceNumber": 71,
+            "referenceNumber": 0,
             "seeAlso": [
                 "http://plan9.bell-labs.com/plan9/license.html",
                 "https://opensource.org/licenses/LPL-1.02"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LPPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "LPPL-1.0",
             "name": "LaTeX Project Public License v1.0",
             "reference": "https://spdx.org/licenses/LPPL-1.0.html",
-            "referenceNumber": 226,
+            "referenceNumber": 541,
             "seeAlso": [
                 "http://www.latex-project.org/lppl/lppl-1-0.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LPPL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "LPPL-1.1",
             "name": "LaTeX Project Public License v1.1",
             "reference": "https://spdx.org/licenses/LPPL-1.1.html",
-            "referenceNumber": 460,
+            "referenceNumber": 94,
             "seeAlso": [
                 "http://www.latex-project.org/lppl/lppl-1-1.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LPPL-1.2.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "LPPL-1.2",
             "name": "LaTeX Project Public License v1.2",
             "reference": "https://spdx.org/licenses/LPPL-1.2.html",
-            "referenceNumber": 30,
+            "referenceNumber": 429,
             "seeAlso": [
                 "http://www.latex-project.org/lppl/lppl-1-2.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LPPL-1.3a.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "LPPL-1.3a",
             "name": "LaTeX Project Public License v1.3a",
             "reference": "https://spdx.org/licenses/LPPL-1.3a.html",
-            "referenceNumber": 31,
+            "referenceNumber": 516,
             "seeAlso": [
                 "http://www.latex-project.org/lppl/lppl-1-3a.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LPPL-1.3c.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "LPPL-1.3c",
             "name": "LaTeX Project Public License v1.3c",
             "reference": "https://spdx.org/licenses/LPPL-1.3c.html",
-            "referenceNumber": 11,
+            "referenceNumber": 237,
             "seeAlso": [
                 "http://www.latex-project.org/lppl/lppl-1-3c.txt",
                 "https://opensource.org/licenses/LPPL-1.3c"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LZMA-SDK-9.11-to-9.20.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "LZMA-SDK-9.11-to-9.20",
             "name": "LZMA SDK License (versions 9.11 to 9.20)",
             "reference": "https://spdx.org/licenses/LZMA-SDK-9.11-to-9.20.html",
-            "referenceNumber": 57,
+            "referenceNumber": 431,
             "seeAlso": [
                 "https://www.7-zip.org/sdk.html",
                 "https://sourceforge.net/projects/sevenzip/files/LZMA%20SDK/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LZMA-SDK-9.22.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "LZMA-SDK-9.22",
             "name": "LZMA SDK License (versions 9.22 and beyond)",
             "reference": "https://spdx.org/licenses/LZMA-SDK-9.22.html",
-            "referenceNumber": 219,
+            "referenceNumber": 449,
             "seeAlso": [
                 "https://www.7-zip.org/sdk.html",
                 "https://sourceforge.net/projects/sevenzip/files/LZMA%20SDK/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MakeIndex.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "MakeIndex",
             "name": "MakeIndex License",
             "reference": "https://spdx.org/licenses/MakeIndex.html",
-            "referenceNumber": 319,
+            "referenceNumber": 124,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/MakeIndex"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Martin-Birgmeier.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Martin-Birgmeier",
+            "name": "Martin Birgmeier License",
+            "reference": "https://spdx.org/licenses/Martin-Birgmeier.html",
+            "referenceNumber": 380,
+            "seeAlso": [
+                "https://github.com/Perl/perl5/blob/blead/util.c#L6136"
+            ]
+        },
+        {
+            "detailsUrl": "https://spdx.org/licenses/metamail.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "metamail",
+            "name": "metamail License",
+            "reference": "https://spdx.org/licenses/metamail.html",
+            "referenceNumber": 473,
+            "seeAlso": [
+                "https://github.com/Dual-Life/mime-base64/blob/master/Base64.xs#L12"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Minpack.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Minpack",
             "name": "Minpack License",
             "reference": "https://spdx.org/licenses/Minpack.html",
-            "referenceNumber": 493,
+            "referenceNumber": 306,
             "seeAlso": [
                 "http://www.netlib.org/minpack/disclaimer",
                 "https://gitlab.com/libeigen/eigen/-/blob/master/COPYING.MINPACK"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MirOS.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "MirOS",
             "name": "The MirOS Licence",
             "reference": "https://spdx.org/licenses/MirOS.html",
-            "referenceNumber": 148,
+            "referenceNumber": 443,
             "seeAlso": [
                 "https://opensource.org/licenses/MirOS"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MIT.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "MIT",
             "name": "MIT License",
             "reference": "https://spdx.org/licenses/MIT.html",
-            "referenceNumber": 479,
+            "referenceNumber": 223,
             "seeAlso": [
                 "https://opensource.org/licenses/MIT"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MIT-0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "MIT-0",
             "name": "MIT No Attribution",
             "reference": "https://spdx.org/licenses/MIT-0.html",
-            "referenceNumber": 480,
+            "referenceNumber": 369,
             "seeAlso": [
                 "https://github.com/aws/mit-0",
                 "https://romanrm.net/mit-zero",
                 "https://github.com/awsdocs/aws-cloud9-user-guide/blob/master/LICENSE-SAMPLECODE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MIT-advertising.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "MIT-advertising",
             "name": "Enlightenment License (e16)",
             "reference": "https://spdx.org/licenses/MIT-advertising.html",
-            "referenceNumber": 112,
+            "referenceNumber": 382,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/MIT_With_Advertising"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MIT-CMU.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "MIT-CMU",
             "name": "CMU License",
             "reference": "https://spdx.org/licenses/MIT-CMU.html",
-            "referenceNumber": 303,
+            "referenceNumber": 20,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing:MIT?rd=Licensing/MIT#CMU_Style",
                 "https://github.com/python-pillow/Pillow/blob/fffb426092c8db24a5f4b6df243a8a3c01fb63cd/LICENSE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MIT-enna.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "MIT-enna",
             "name": "enna License",
             "reference": "https://spdx.org/licenses/MIT-enna.html",
-            "referenceNumber": 320,
+            "referenceNumber": 466,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/MIT#enna"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MIT-feh.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "MIT-feh",
             "name": "feh License",
             "reference": "https://spdx.org/licenses/MIT-feh.html",
-            "referenceNumber": 307,
+            "referenceNumber": 234,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/MIT#feh"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/MIT-Festival.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "MIT-Festival",
+            "name": "MIT Festival Variant",
+            "reference": "https://spdx.org/licenses/MIT-Festival.html",
+            "referenceNumber": 423,
+            "seeAlso": [
+                "https://github.com/festvox/flite/blob/master/COPYING",
+                "https://github.com/festvox/speech_tools/blob/master/COPYING"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/MIT-Modern-Variant.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "MIT-Modern-Variant",
             "name": "MIT License Modern Variant",
             "reference": "https://spdx.org/licenses/MIT-Modern-Variant.html",
-            "referenceNumber": 463,
+            "referenceNumber": 548,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing:MIT#Modern_Variants",
                 "https://ptolemy.berkeley.edu/copyright.htm",
                 "https://pirlwww.lpl.arizona.edu/resources/guide/software/PerlTk/Tixlic.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MIT-open-group.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "MIT-open-group",
             "name": "MIT Open Group variant",
             "reference": "https://spdx.org/licenses/MIT-open-group.html",
-            "referenceNumber": 418,
+            "referenceNumber": 43,
             "seeAlso": [
                 "https://gitlab.freedesktop.org/xorg/app/iceauth/-/blob/master/COPYING",
                 "https://gitlab.freedesktop.org/xorg/app/xvinfo/-/blob/master/COPYING",
                 "https://gitlab.freedesktop.org/xorg/app/xsetroot/-/blob/master/COPYING",
                 "https://gitlab.freedesktop.org/xorg/app/xauth/-/blob/master/COPYING"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/MIT-Wu.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "MIT-Wu",
+            "name": "MIT Tom Wu Variant",
+            "reference": "https://spdx.org/licenses/MIT-Wu.html",
+            "referenceNumber": 421,
+            "seeAlso": [
+                "https://github.com/chromium/octane/blob/master/crypto.js"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/MITNFA.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "MITNFA",
             "name": "MIT +no-false-attribs license",
             "reference": "https://spdx.org/licenses/MITNFA.html",
-            "referenceNumber": 82,
+            "referenceNumber": 145,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/MITNFA"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Motosoto.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Motosoto",
             "name": "Motosoto License",
             "reference": "https://spdx.org/licenses/Motosoto.html",
-            "referenceNumber": 470,
+            "referenceNumber": 357,
             "seeAlso": [
                 "https://opensource.org/licenses/Motosoto"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/mpi-permissive.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "mpi-permissive",
             "name": "mpi Permissive License",
             "reference": "https://spdx.org/licenses/mpi-permissive.html",
-            "referenceNumber": 244,
+            "referenceNumber": 295,
             "seeAlso": [
                 "https://sources.debian.org/src/openmpi/4.1.0-10/ompi/debuggers/msgq_interface.h/?hl=19#L19"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/mpich2.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "mpich2",
             "name": "mpich2 License",
             "reference": "https://spdx.org/licenses/mpich2.html",
-            "referenceNumber": 13,
+            "referenceNumber": 283,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/MIT"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "MPL-1.0",
             "name": "Mozilla Public License 1.0",
             "reference": "https://spdx.org/licenses/MPL-1.0.html",
-            "referenceNumber": 413,
+            "referenceNumber": 95,
             "seeAlso": [
                 "http://www.mozilla.org/MPL/MPL-1.0.html",
                 "https://opensource.org/licenses/MPL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MPL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "MPL-1.1",
             "name": "Mozilla Public License 1.1",
             "reference": "https://spdx.org/licenses/MPL-1.1.html",
-            "referenceNumber": 304,
+            "referenceNumber": 192,
             "seeAlso": [
                 "http://www.mozilla.org/MPL/MPL-1.1.html",
                 "https://opensource.org/licenses/MPL-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MPL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "MPL-2.0",
             "name": "Mozilla Public License 2.0",
             "reference": "https://spdx.org/licenses/MPL-2.0.html",
-            "referenceNumber": 116,
+            "referenceNumber": 236,
             "seeAlso": [
                 "https://www.mozilla.org/MPL/2.0/",
                 "https://opensource.org/licenses/MPL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MPL-2.0-no-copyleft-exception.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "MPL-2.0-no-copyleft-exception",
             "name": "Mozilla Public License 2.0 (no copyleft exception)",
             "reference": "https://spdx.org/licenses/MPL-2.0-no-copyleft-exception.html",
-            "referenceNumber": 342,
+            "referenceNumber": 67,
             "seeAlso": [
                 "https://www.mozilla.org/MPL/2.0/",
                 "https://opensource.org/licenses/MPL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/mplus.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "mplus",
             "name": "mplus Font License",
             "reference": "https://spdx.org/licenses/mplus.html",
-            "referenceNumber": 103,
+            "referenceNumber": 157,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing:Mplus?rd=Licensing/mplus"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MS-LPL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "MS-LPL",
             "name": "Microsoft Limited Public License",
             "reference": "https://spdx.org/licenses/MS-LPL.html",
-            "referenceNumber": 179,
+            "referenceNumber": 186,
             "seeAlso": [
                 "https://www.openhub.net/licenses/mslpl",
                 "https://github.com/gabegundy/atlserver/blob/master/License.txt",
                 "https://en.wikipedia.org/wiki/Shared_Source_Initiative#Microsoft_Limited_Public_License_(Ms-LPL)"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MS-PL.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "MS-PL",
             "name": "Microsoft Public License",
             "reference": "https://spdx.org/licenses/MS-PL.html",
-            "referenceNumber": 254,
+            "referenceNumber": 420,
             "seeAlso": [
                 "http://www.microsoft.com/opensource/licenses.mspx",
                 "https://opensource.org/licenses/MS-PL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MS-RL.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "MS-RL",
             "name": "Microsoft Reciprocal License",
             "reference": "https://spdx.org/licenses/MS-RL.html",
-            "referenceNumber": 414,
+            "referenceNumber": 22,
             "seeAlso": [
                 "http://www.microsoft.com/opensource/licenses.mspx",
                 "https://opensource.org/licenses/MS-RL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MTLL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "MTLL",
             "name": "Matrix Template Library License",
             "reference": "https://spdx.org/licenses/MTLL.html",
-            "referenceNumber": 165,
+            "referenceNumber": 80,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Matrix_Template_Library_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MulanPSL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "MulanPSL-1.0",
             "name": "Mulan Permissive Software License, Version 1",
             "reference": "https://spdx.org/licenses/MulanPSL-1.0.html",
-            "referenceNumber": 81,
+            "referenceNumber": 304,
             "seeAlso": [
                 "https://license.coscl.org.cn/MulanPSL/",
                 "https://github.com/yuwenlong/longphp/blob/25dfb70cc2a466dc4bb55ba30901cbce08d164b5/LICENSE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MulanPSL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "MulanPSL-2.0",
             "name": "Mulan Permissive Software License, Version 2",
             "reference": "https://spdx.org/licenses/MulanPSL-2.0.html",
-            "referenceNumber": 467,
+            "referenceNumber": 481,
             "seeAlso": [
                 "https://license.coscl.org.cn/MulanPSL2/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Multics.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Multics",
             "name": "Multics License",
             "reference": "https://spdx.org/licenses/Multics.html",
-            "referenceNumber": 488,
+            "referenceNumber": 248,
             "seeAlso": [
                 "https://opensource.org/licenses/Multics"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Mup.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Mup",
             "name": "Mup License",
             "reference": "https://spdx.org/licenses/Mup.html",
-            "referenceNumber": 314,
+            "referenceNumber": 480,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Mup"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NAIST-2003.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NAIST-2003",
             "name": "Nara Institute of Science and Technology License (2003)",
             "reference": "https://spdx.org/licenses/NAIST-2003.html",
-            "referenceNumber": 477,
+            "referenceNumber": 30,
             "seeAlso": [
                 "https://enterprise.dejacode.com/licenses/public/naist-2003/#license-text",
                 "https://github.com/nodejs/node/blob/4a19cc8947b1bba2b2d27816ec3d0edf9b28e503/LICENSE#L343"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NASA-1.3.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": true,
             "licenseId": "NASA-1.3",
             "name": "NASA Open Source Agreement 1.3",
             "reference": "https://spdx.org/licenses/NASA-1.3.html",
-            "referenceNumber": 35,
+            "referenceNumber": 360,
             "seeAlso": [
                 "http://ti.arc.nasa.gov/opensource/nosa/",
                 "https://opensource.org/licenses/NASA-1.3"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Naumen.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Naumen",
             "name": "Naumen Public License",
             "reference": "https://spdx.org/licenses/Naumen.html",
-            "referenceNumber": 449,
+            "referenceNumber": 339,
             "seeAlso": [
                 "https://opensource.org/licenses/Naumen"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NBPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NBPL-1.0",
             "name": "Net Boolean Public License v1",
             "reference": "https://spdx.org/licenses/NBPL-1.0.html",
-            "referenceNumber": 294,
+            "referenceNumber": 517,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=37b4b3f6cc4bf34e1d3dec61e69914b9819d8894"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NCGL-UK-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NCGL-UK-2.0",
             "name": "Non-Commercial Government Licence",
             "reference": "https://spdx.org/licenses/NCGL-UK-2.0.html",
-            "referenceNumber": 99,
+            "referenceNumber": 112,
             "seeAlso": [
                 "http://www.nationalarchives.gov.uk/doc/non-commercial-government-licence/version/2/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NCSA.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "NCSA",
             "name": "University of Illinois/NCSA Open Source License",
             "reference": "https://spdx.org/licenses/NCSA.html",
-            "referenceNumber": 339,
+            "referenceNumber": 201,
             "seeAlso": [
                 "http://otm.illinois.edu/uiuc_openSource",
                 "https://opensource.org/licenses/NCSA"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Net-SNMP.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Net-SNMP",
             "name": "Net-SNMP License",
             "reference": "https://spdx.org/licenses/Net-SNMP.html",
-            "referenceNumber": 359,
+            "referenceNumber": 75,
             "seeAlso": [
                 "http://net-snmp.sourceforge.net/about/license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NetCDF.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NetCDF",
             "name": "NetCDF license",
             "reference": "https://spdx.org/licenses/NetCDF.html",
-            "referenceNumber": 251,
+            "referenceNumber": 321,
             "seeAlso": [
                 "http://www.unidata.ucar.edu/software/netcdf/copyright.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Newsletr.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Newsletr",
             "name": "Newsletr License",
             "reference": "https://spdx.org/licenses/Newsletr.html",
-            "referenceNumber": 364,
+            "referenceNumber": 539,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Newsletr"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NGPL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "NGPL",
             "name": "Nethack General Public License",
             "reference": "https://spdx.org/licenses/NGPL.html",
-            "referenceNumber": 206,
+            "referenceNumber": 301,
             "seeAlso": [
                 "https://opensource.org/licenses/NGPL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NICTA-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NICTA-1.0",
             "name": "NICTA Public Software License, Version 1.0",
             "reference": "https://spdx.org/licenses/NICTA-1.0.html",
-            "referenceNumber": 438,
+            "referenceNumber": 545,
             "seeAlso": [
                 "https://opensource.apple.com/source/mDNSResponder/mDNSResponder-320.10/mDNSPosix/nss_ReadMe.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NIST-PD.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NIST-PD",
             "name": "NIST Public Domain Notice",
             "reference": "https://spdx.org/licenses/NIST-PD.html",
-            "referenceNumber": 21,
+            "referenceNumber": 346,
             "seeAlso": [
                 "https://github.com/tcheneau/simpleRPL/blob/e645e69e38dd4e3ccfeceb2db8cba05b7c2e0cd3/LICENSE.txt",
                 "https://github.com/tcheneau/Routing/blob/f09f46fcfe636107f22f2c98348188a65a135d98/README.md"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NIST-PD-fallback.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NIST-PD-fallback",
             "name": "NIST Public Domain Notice with license fallback",
             "reference": "https://spdx.org/licenses/NIST-PD-fallback.html",
-            "referenceNumber": 355,
+            "referenceNumber": 319,
             "seeAlso": [
                 "https://github.com/usnistgov/jsip/blob/59700e6926cbe96c5cdae897d9a7d2656b42abe3/LICENSE",
                 "https://github.com/usnistgov/fipy/blob/86aaa5c2ba2c6f1be19593c5986071cf6568cc34/LICENSE.rst"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/NIST-Software.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "NIST-Software",
+            "name": "NIST Software License",
+            "reference": "https://spdx.org/licenses/NIST-Software.html",
+            "referenceNumber": 413,
+            "seeAlso": [
+                "https://github.com/open-quantum-safe/liboqs/blob/40b01fdbb270f8614fde30e65d30e9da18c02393/src/common/rand/rand_nist.c#L1-L15"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/NLOD-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NLOD-1.0",
             "name": "Norwegian Licence for Open Government Data (NLOD) 1.0",
             "reference": "https://spdx.org/licenses/NLOD-1.0.html",
-            "referenceNumber": 255,
+            "referenceNumber": 525,
             "seeAlso": [
                 "http://data.norge.no/nlod/en/1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NLOD-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NLOD-2.0",
             "name": "Norwegian Licence for Open Government Data (NLOD) 2.0",
             "reference": "https://spdx.org/licenses/NLOD-2.0.html",
-            "referenceNumber": 379,
+            "referenceNumber": 51,
             "seeAlso": [
                 "http://data.norge.no/nlod/en/2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NLPL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NLPL",
             "name": "No Limit Public License",
             "reference": "https://spdx.org/licenses/NLPL.html",
-            "referenceNumber": 150,
+            "referenceNumber": 529,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/NLPL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Nokia.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "Nokia",
             "name": "Nokia Open Source License",
             "reference": "https://spdx.org/licenses/Nokia.html",
-            "referenceNumber": 6,
+            "referenceNumber": 84,
             "seeAlso": [
                 "https://opensource.org/licenses/nokia"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NOSL.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "NOSL",
             "name": "Netizen Open Source License",
             "reference": "https://spdx.org/licenses/NOSL.html",
-            "referenceNumber": 123,
+            "referenceNumber": 417,
             "seeAlso": [
                 "http://bits.netizen.com.au/licenses/NOSL/nosl.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Noweb.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Noweb",
             "name": "Noweb License",
             "reference": "https://spdx.org/licenses/Noweb.html",
-            "referenceNumber": 434,
+            "referenceNumber": 398,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Noweb"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "NPL-1.0",
             "name": "Netscape Public License v1.0",
             "reference": "https://spdx.org/licenses/NPL-1.0.html",
-            "referenceNumber": 24,
+            "referenceNumber": 56,
             "seeAlso": [
                 "http://www.mozilla.org/MPL/NPL/1.0/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NPL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "NPL-1.1",
             "name": "Netscape Public License v1.1",
             "reference": "https://spdx.org/licenses/NPL-1.1.html",
-            "referenceNumber": 451,
+            "referenceNumber": 53,
             "seeAlso": [
                 "http://www.mozilla.org/MPL/NPL/1.1/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NPOSL-3.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "NPOSL-3.0",
             "name": "Non-Profit Open Software License 3.0",
             "reference": "https://spdx.org/licenses/NPOSL-3.0.html",
-            "referenceNumber": 217,
+            "referenceNumber": 549,
             "seeAlso": [
                 "https://opensource.org/licenses/NOSL3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NRL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NRL",
             "name": "NRL License",
             "reference": "https://spdx.org/licenses/NRL.html",
-            "referenceNumber": 442,
+            "referenceNumber": 458,
             "seeAlso": [
                 "http://web.mit.edu/network/isakmp/nrllicense.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NTP.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "NTP",
             "name": "NTP License",
             "reference": "https://spdx.org/licenses/NTP.html",
-            "referenceNumber": 444,
+            "referenceNumber": 2,
             "seeAlso": [
                 "https://opensource.org/licenses/NTP"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NTP-0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NTP-0",
             "name": "NTP No Attribution",
             "reference": "https://spdx.org/licenses/NTP-0.html",
-            "referenceNumber": 402,
+            "referenceNumber": 476,
             "seeAlso": [
                 "https://github.com/tytso/e2fsprogs/blob/master/lib/et/et_name.c"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Nunit.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "Nunit",
             "name": "Nunit License",
             "reference": "https://spdx.org/licenses/Nunit.html",
-            "referenceNumber": 223,
+            "referenceNumber": 456,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Nunit"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/O-UDA-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "O-UDA-1.0",
             "name": "Open Use of Data Agreement v1.0",
             "reference": "https://spdx.org/licenses/O-UDA-1.0.html",
-            "referenceNumber": 372,
+            "referenceNumber": 542,
             "seeAlso": [
                 "https://github.com/microsoft/Open-Use-of-Data-Agreement/blob/v1.0/O-UDA-1.0.md",
                 "https://cdla.dev/open-use-of-data-agreement-v1-0/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OCCT-PL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OCCT-PL",
             "name": "Open CASCADE Technology Public License",
             "reference": "https://spdx.org/licenses/OCCT-PL.html",
-            "referenceNumber": 349,
+            "referenceNumber": 298,
             "seeAlso": [
                 "http://www.opencascade.com/content/occt-public-license"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OCLC-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "OCLC-2.0",
             "name": "OCLC Research Public License 2.0",
             "reference": "https://spdx.org/licenses/OCLC-2.0.html",
-            "referenceNumber": 317,
+            "referenceNumber": 370,
             "seeAlso": [
                 "http://www.oclc.org/research/activities/software/license/v2final.htm",
                 "https://opensource.org/licenses/OCLC-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ODbL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "ODbL-1.0",
             "name": "Open Data Commons Open Database License v1.0",
             "reference": "https://spdx.org/licenses/ODbL-1.0.html",
-            "referenceNumber": 118,
+            "referenceNumber": 356,
             "seeAlso": [
                 "http://www.opendatacommons.org/licenses/odbl/1.0/",
                 "https://opendatacommons.org/licenses/odbl/1-0/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ODC-By-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "ODC-By-1.0",
             "name": "Open Data Commons Attribution License v1.0",
             "reference": "https://spdx.org/licenses/ODC-By-1.0.html",
-            "referenceNumber": 400,
+            "referenceNumber": 64,
             "seeAlso": [
                 "https://opendatacommons.org/licenses/by/1.0/"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/OFFIS.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "OFFIS",
+            "name": "OFFIS License",
+            "reference": "https://spdx.org/licenses/OFFIS.html",
+            "referenceNumber": 105,
+            "seeAlso": [
+                "https://sourceforge.net/p/xmedcon/code/ci/master/tree/libs/dicom/README"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/OFL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "OFL-1.0",
             "name": "SIL Open Font License 1.0",
             "reference": "https://spdx.org/licenses/OFL-1.0.html",
-            "referenceNumber": 104,
+            "referenceNumber": 419,
             "seeAlso": [
                 "http://scripts.sil.org/cms/scripts/page.php?item_id=OFL10_web"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OFL-1.0-no-RFN.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OFL-1.0-no-RFN",
             "name": "SIL Open Font License 1.0 with no Reserved Font Name",
             "reference": "https://spdx.org/licenses/OFL-1.0-no-RFN.html",
-            "referenceNumber": 178,
+            "referenceNumber": 354,
             "seeAlso": [
                 "http://scripts.sil.org/cms/scripts/page.php?item_id=OFL10_web"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OFL-1.0-RFN.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OFL-1.0-RFN",
             "name": "SIL Open Font License 1.0 with Reserved Font Name",
             "reference": "https://spdx.org/licenses/OFL-1.0-RFN.html",
-            "referenceNumber": 195,
+            "referenceNumber": 250,
             "seeAlso": [
                 "http://scripts.sil.org/cms/scripts/page.php?item_id=OFL10_web"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OFL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "OFL-1.1",
             "name": "SIL Open Font License 1.1",
             "reference": "https://spdx.org/licenses/OFL-1.1.html",
-            "referenceNumber": 408,
+            "referenceNumber": 3,
             "seeAlso": [
                 "http://scripts.sil.org/cms/scripts/page.php?item_id=OFL_web",
                 "https://opensource.org/licenses/OFL-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OFL-1.1-no-RFN.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "OFL-1.1-no-RFN",
             "name": "SIL Open Font License 1.1 with no Reserved Font Name",
             "reference": "https://spdx.org/licenses/OFL-1.1-no-RFN.html",
-            "referenceNumber": 154,
+            "referenceNumber": 117,
             "seeAlso": [
                 "http://scripts.sil.org/cms/scripts/page.php?item_id=OFL_web",
                 "https://opensource.org/licenses/OFL-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OFL-1.1-RFN.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "OFL-1.1-RFN",
             "name": "SIL Open Font License 1.1 with Reserved Font Name",
             "reference": "https://spdx.org/licenses/OFL-1.1-RFN.html",
-            "referenceNumber": 107,
+            "referenceNumber": 518,
             "seeAlso": [
                 "http://scripts.sil.org/cms/scripts/page.php?item_id=OFL_web",
                 "https://opensource.org/licenses/OFL-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OGC-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OGC-1.0",
             "name": "OGC Software License, Version 1.0",
             "reference": "https://spdx.org/licenses/OGC-1.0.html",
-            "referenceNumber": 90,
+            "referenceNumber": 15,
             "seeAlso": [
                 "https://www.ogc.org/ogc/software/1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OGDL-Taiwan-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OGDL-Taiwan-1.0",
             "name": "Taiwan Open Government Data License, version 1.0",
             "reference": "https://spdx.org/licenses/OGDL-Taiwan-1.0.html",
-            "referenceNumber": 393,
+            "referenceNumber": 284,
             "seeAlso": [
                 "https://data.gov.tw/license"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OGL-Canada-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OGL-Canada-2.0",
             "name": "Open Government Licence - Canada",
             "reference": "https://spdx.org/licenses/OGL-Canada-2.0.html",
-            "referenceNumber": 309,
+            "referenceNumber": 214,
             "seeAlso": [
                 "https://open.canada.ca/en/open-government-licence-canada"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OGL-UK-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OGL-UK-1.0",
             "name": "Open Government Licence v1.0",
             "reference": "https://spdx.org/licenses/OGL-UK-1.0.html",
-            "referenceNumber": 241,
+            "referenceNumber": 161,
             "seeAlso": [
                 "http://www.nationalarchives.gov.uk/doc/open-government-licence/version/1/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OGL-UK-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OGL-UK-2.0",
             "name": "Open Government Licence v2.0",
             "reference": "https://spdx.org/licenses/OGL-UK-2.0.html",
-            "referenceNumber": 4,
+            "referenceNumber": 303,
             "seeAlso": [
                 "http://www.nationalarchives.gov.uk/doc/open-government-licence/version/2/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OGL-UK-3.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OGL-UK-3.0",
             "name": "Open Government Licence v3.0",
             "reference": "https://spdx.org/licenses/OGL-UK-3.0.html",
-            "referenceNumber": 380,
+            "referenceNumber": 415,
             "seeAlso": [
                 "http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OGTSL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "OGTSL",
             "name": "Open Group Test Suite License",
             "reference": "https://spdx.org/licenses/OGTSL.html",
-            "referenceNumber": 50,
+            "referenceNumber": 133,
             "seeAlso": [
                 "http://www.opengroup.org/testing/downloads/The_Open_Group_TSL.txt",
                 "https://opensource.org/licenses/OGTSL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-1.1",
             "name": "Open LDAP Public License v1.1",
             "reference": "https://spdx.org/licenses/OLDAP-1.1.html",
-            "referenceNumber": 218,
+            "referenceNumber": 208,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=806557a5ad59804ef3a44d5abfbe91d706b0791f"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-1.2.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-1.2",
             "name": "Open LDAP Public License v1.2",
             "reference": "https://spdx.org/licenses/OLDAP-1.2.html",
-            "referenceNumber": 210,
+            "referenceNumber": 100,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=42b0383c50c299977b5893ee695cf4e486fb0dc7"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-1.3.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-1.3",
             "name": "Open LDAP Public License v1.3",
             "reference": "https://spdx.org/licenses/OLDAP-1.3.html",
-            "referenceNumber": 127,
+            "referenceNumber": 328,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=e5f8117f0ce088d0bd7a8e18ddf37eaa40eb09b1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-1.4.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-1.4",
             "name": "Open LDAP Public License v1.4",
             "reference": "https://spdx.org/licenses/OLDAP-1.4.html",
-            "referenceNumber": 215,
+            "referenceNumber": 327,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=c9f95c2f3f2ffb5e0ae55fe7388af75547660941"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.0",
             "name": "Open LDAP Public License v2.0 (or possibly 2.0A and 2.0B)",
             "reference": "https://spdx.org/licenses/OLDAP-2.0.html",
-            "referenceNumber": 83,
+            "referenceNumber": 519,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=cbf50f4e1185a21abd4c0a54d3f4341fe28f36ea"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.0.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.0.1",
             "name": "Open LDAP Public License v2.0.1",
             "reference": "https://spdx.org/licenses/OLDAP-2.0.1.html",
-            "referenceNumber": 115,
+            "referenceNumber": 324,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=b6d68acd14e51ca3aab4428bf26522aa74873f0e"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.1",
             "name": "Open LDAP Public License v2.1",
             "reference": "https://spdx.org/licenses/OLDAP-2.1.html",
-            "referenceNumber": 263,
+            "referenceNumber": 402,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=b0d176738e96a0d3b9f85cb51e140a86f21be715"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.2.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.2",
             "name": "Open LDAP Public License v2.2",
             "reference": "https://spdx.org/licenses/OLDAP-2.2.html",
-            "referenceNumber": 167,
+            "referenceNumber": 162,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=470b0c18ec67621c85881b2733057fecf4a1acc3"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.2.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.2.1",
             "name": "Open LDAP Public License v2.2.1",
             "reference": "https://spdx.org/licenses/OLDAP-2.2.1.html",
-            "referenceNumber": 63,
+            "referenceNumber": 451,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=4bc786f34b50aa301be6f5600f58a980070f481e"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.2.2.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.2.2",
             "name": "Open LDAP Public License 2.2.2",
             "reference": "https://spdx.org/licenses/OLDAP-2.2.2.html",
-            "referenceNumber": 193,
+            "referenceNumber": 140,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=df2cc1e21eb7c160695f5b7cffd6296c151ba188"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.3.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.3",
             "name": "Open LDAP Public License v2.3",
             "reference": "https://spdx.org/licenses/OLDAP-2.3.html",
-            "referenceNumber": 448,
+            "referenceNumber": 42,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=d32cf54a32d581ab475d23c810b0a7fbaf8d63c3"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.4.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.4",
             "name": "Open LDAP Public License v2.4",
             "reference": "https://spdx.org/licenses/OLDAP-2.4.html",
-            "referenceNumber": 421,
+            "referenceNumber": 474,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=cd1284c4a91a8a380d904eee68d1583f989ed386"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.5.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.5",
             "name": "Open LDAP Public License v2.5",
             "reference": "https://spdx.org/licenses/OLDAP-2.5.html",
-            "referenceNumber": 495,
+            "referenceNumber": 554,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=6852b9d90022e8593c98205413380536b1b5a7cf"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.6.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.6",
             "name": "Open LDAP Public License v2.6",
             "reference": "https://spdx.org/licenses/OLDAP-2.6.html",
-            "referenceNumber": 182,
+            "referenceNumber": 270,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=1cae062821881f41b73012ba816434897abf4205"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.7.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.7",
             "name": "Open LDAP Public License v2.7",
             "reference": "https://spdx.org/licenses/OLDAP-2.7.html",
-            "referenceNumber": 315,
+            "referenceNumber": 134,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=47c2415c1df81556eeb39be6cad458ef87c534a2"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.8.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "OLDAP-2.8",
             "name": "Open LDAP Public License v2.8",
             "reference": "https://spdx.org/licenses/OLDAP-2.8.html",
-            "referenceNumber": 405,
+            "referenceNumber": 540,
             "seeAlso": [
                 "http://www.openldap.org/software/release/license.html"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/OLFL-1.3.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": true,
+            "licenseId": "OLFL-1.3",
+            "name": "Open Logistics Foundation License Version 1.3",
+            "reference": "https://spdx.org/licenses/OLFL-1.3.html",
+            "referenceNumber": 482,
+            "seeAlso": [
+                "https://openlogisticsfoundation.org/licenses/",
+                "https://opensource.org/license/olfl-1-3/"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/OML.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OML",
             "name": "Open Market License",
             "reference": "https://spdx.org/licenses/OML.html",
-            "referenceNumber": 417,
+            "referenceNumber": 155,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Open_Market_License"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/OpenPBS-2.3.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "OpenPBS-2.3",
+            "name": "OpenPBS v2.3 Software License",
+            "reference": "https://spdx.org/licenses/OpenPBS-2.3.html",
+            "referenceNumber": 378,
+            "seeAlso": [
+                "https://github.com/adaptivecomputing/torque/blob/master/PBS_License.txt",
+                "https://www.mcs.anl.gov/research/projects/openpbs/PBS_License.txt"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/OpenSSL.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "OpenSSL",
             "name": "OpenSSL License",
             "reference": "https://spdx.org/licenses/OpenSSL.html",
-            "referenceNumber": 385,
+            "referenceNumber": 276,
             "seeAlso": [
                 "http://www.openssl.org/source/license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "OPL-1.0",
             "name": "Open Public License v1.0",
             "reference": "https://spdx.org/licenses/OPL-1.0.html",
-            "referenceNumber": 194,
+            "referenceNumber": 501,
             "seeAlso": [
                 "http://old.koalateam.com/jackaroo/OPL_1_0.TXT",
                 "https://fedoraproject.org/wiki/Licensing/Open_Public_License"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/OPL-UK-3.0.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "OPL-UK-3.0",
+            "name": "United    Kingdom Open Parliament Licence v3.0",
+            "reference": "https://spdx.org/licenses/OPL-UK-3.0.html",
+            "referenceNumber": 247,
+            "seeAlso": [
+                "https://www.parliament.uk/site-information/copyright-parliament/open-parliament-licence/"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/OPUBL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OPUBL-1.0",
             "name": "Open Publication License v1.0",
             "reference": "https://spdx.org/licenses/OPUBL-1.0.html",
-            "referenceNumber": 94,
+            "referenceNumber": 514,
             "seeAlso": [
                 "http://opencontent.org/openpub/",
                 "https://www.debian.org/opl",
                 "https://www.ctan.org/license/opl"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OSET-PL-2.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "OSET-PL-2.1",
             "name": "OSET Public License version 2.1",
             "reference": "https://spdx.org/licenses/OSET-PL-2.1.html",
-            "referenceNumber": 258,
+            "referenceNumber": 274,
             "seeAlso": [
                 "http://www.osetfoundation.org/public-license",
                 "https://opensource.org/licenses/OPL-2.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OSL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "OSL-1.0",
             "name": "Open Software License 1.0",
             "reference": "https://spdx.org/licenses/OSL-1.0.html",
-            "referenceNumber": 25,
+            "referenceNumber": 371,
             "seeAlso": [
                 "https://opensource.org/licenses/OSL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OSL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "OSL-1.1",
             "name": "Open Software License 1.1",
             "reference": "https://spdx.org/licenses/OSL-1.1.html",
-            "referenceNumber": 260,
+            "referenceNumber": 311,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/OSL1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OSL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "OSL-2.0",
             "name": "Open Software License 2.0",
             "reference": "https://spdx.org/licenses/OSL-2.0.html",
-            "referenceNumber": 399,
+            "referenceNumber": 405,
             "seeAlso": [
                 "http://web.archive.org/web/20041020171434/http://www.rosenlaw.com/osl2.0.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OSL-2.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "OSL-2.1",
             "name": "Open Software License 2.1",
             "reference": "https://spdx.org/licenses/OSL-2.1.html",
-            "referenceNumber": 325,
+            "referenceNumber": 251,
             "seeAlso": [
                 "http://web.archive.org/web/20050212003940/http://www.rosenlaw.com/osl21.htm",
                 "https://opensource.org/licenses/OSL-2.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OSL-3.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "OSL-3.0",
             "name": "Open Software License 3.0",
             "reference": "https://spdx.org/licenses/OSL-3.0.html",
-            "referenceNumber": 140,
+            "referenceNumber": 19,
             "seeAlso": [
                 "https://web.archive.org/web/20120101081418/http://rosenlaw.com:80/OSL3.0.htm",
                 "https://opensource.org/licenses/OSL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Parity-6.0.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Parity-6.0.0",
             "name": "The Parity Public License 6.0.0",
             "reference": "https://spdx.org/licenses/Parity-6.0.0.html",
-            "referenceNumber": 60,
+            "referenceNumber": 69,
             "seeAlso": [
                 "https://paritylicense.com/versions/6.0.0.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Parity-7.0.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Parity-7.0.0",
             "name": "The Parity Public License 7.0.0",
             "reference": "https://spdx.org/licenses/Parity-7.0.0.html",
-            "referenceNumber": 437,
+            "referenceNumber": 323,
             "seeAlso": [
                 "https://paritylicense.com/versions/7.0.0.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/PDDL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "PDDL-1.0",
             "name": "Open Data Commons Public Domain Dedication & License 1.0",
             "reference": "https://spdx.org/licenses/PDDL-1.0.html",
-            "referenceNumber": 138,
+            "referenceNumber": 40,
             "seeAlso": [
                 "http://opendatacommons.org/licenses/pddl/1.0/",
                 "https://opendatacommons.org/licenses/pddl/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/PHP-3.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "PHP-3.0",
             "name": "PHP License v3.0",
             "reference": "https://spdx.org/licenses/PHP-3.0.html",
-            "referenceNumber": 281,
+            "referenceNumber": 450,
             "seeAlso": [
                 "http://www.php.net/license/3_0.txt",
                 "https://opensource.org/licenses/PHP-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/PHP-3.01.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "PHP-3.01",
             "name": "PHP License v3.01",
             "reference": "https://spdx.org/licenses/PHP-3.01.html",
-            "referenceNumber": 348,
+            "referenceNumber": 58,
             "seeAlso": [
                 "http://www.php.net/license/3_01.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Plexus.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Plexus",
             "name": "Plexus Classworlds License",
             "reference": "https://spdx.org/licenses/Plexus.html",
-            "referenceNumber": 132,
+            "referenceNumber": 97,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Plexus_Classworlds_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/PolyForm-Noncommercial-1.0.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "PolyForm-Noncommercial-1.0.0",
             "name": "PolyForm Noncommercial License 1.0.0",
             "reference": "https://spdx.org/licenses/PolyForm-Noncommercial-1.0.0.html",
-            "referenceNumber": 429,
+            "referenceNumber": 113,
             "seeAlso": [
                 "https://polyformproject.org/licenses/noncommercial/1.0.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/PolyForm-Small-Business-1.0.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "PolyForm-Small-Business-1.0.0",
             "name": "PolyForm Small Business License 1.0.0",
             "reference": "https://spdx.org/licenses/PolyForm-Small-Business-1.0.0.html",
-            "referenceNumber": 461,
+            "referenceNumber": 167,
             "seeAlso": [
                 "https://polyformproject.org/licenses/small-business/1.0.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/PostgreSQL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "PostgreSQL",
             "name": "PostgreSQL License",
             "reference": "https://spdx.org/licenses/PostgreSQL.html",
-            "referenceNumber": 189,
+            "referenceNumber": 527,
             "seeAlso": [
                 "http://www.postgresql.org/about/licence",
                 "https://opensource.org/licenses/PostgreSQL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/PSF-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "PSF-2.0",
             "name": "Python Software Foundation License 2.0",
             "reference": "https://spdx.org/licenses/PSF-2.0.html",
-            "referenceNumber": 428,
+            "referenceNumber": 88,
             "seeAlso": [
                 "https://opensource.org/licenses/Python-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/psfrag.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "psfrag",
             "name": "psfrag License",
             "reference": "https://spdx.org/licenses/psfrag.html",
-            "referenceNumber": 88,
+            "referenceNumber": 191,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/psfrag"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/psutils.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "psutils",
             "name": "psutils License",
             "reference": "https://spdx.org/licenses/psutils.html",
-            "referenceNumber": 129,
+            "referenceNumber": 21,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/psutils"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Python-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "Python-2.0",
             "name": "Python License 2.0",
             "reference": "https://spdx.org/licenses/Python-2.0.html",
-            "referenceNumber": 351,
+            "referenceNumber": 459,
             "seeAlso": [
                 "https://opensource.org/licenses/Python-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Python-2.0.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Python-2.0.1",
             "name": "Python License 2.0.1",
             "reference": "https://spdx.org/licenses/Python-2.0.1.html",
-            "referenceNumber": 233,
+            "referenceNumber": 305,
             "seeAlso": [
                 "https://www.python.org/download/releases/2.0.1/license/",
                 "https://docs.python.org/3/license.html",
                 "https://github.com/python/cpython/blob/main/LICENSE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Qhull.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Qhull",
             "name": "Qhull License",
             "reference": "https://spdx.org/licenses/Qhull.html",
-            "referenceNumber": 378,
+            "referenceNumber": 158,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Qhull"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/QPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "QPL-1.0",
             "name": "Q Public License 1.0",
             "reference": "https://spdx.org/licenses/QPL-1.0.html",
-            "referenceNumber": 14,
+            "referenceNumber": 470,
             "seeAlso": [
                 "http://doc.qt.nokia.com/3.3/license.html",
                 "https://opensource.org/licenses/QPL-1.0",
                 "https://doc.qt.io/archives/3.3/license.html"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/QPL-1.0-INRIA-2004.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "QPL-1.0-INRIA-2004",
+            "name": "Q Public License 1.0 - INRIA 2004 variant",
+            "reference": "https://spdx.org/licenses/QPL-1.0-INRIA-2004.html",
+            "referenceNumber": 62,
+            "seeAlso": [
+                "https://github.com/maranget/hevea/blob/master/LICENSE"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Rdisc.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Rdisc",
             "name": "Rdisc License",
             "reference": "https://spdx.org/licenses/Rdisc.html",
-            "referenceNumber": 312,
+            "referenceNumber": 222,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Rdisc_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/RHeCos-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "RHeCos-1.1",
             "name": "Red Hat eCos Public License v1.1",
             "reference": "https://spdx.org/licenses/RHeCos-1.1.html",
-            "referenceNumber": 469,
+            "referenceNumber": 422,
             "seeAlso": [
                 "http://ecos.sourceware.org/old-license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/RPL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "RPL-1.1",
             "name": "Reciprocal Public License 1.1",
             "reference": "https://spdx.org/licenses/RPL-1.1.html",
-            "referenceNumber": 347,
+            "referenceNumber": 17,
             "seeAlso": [
                 "https://opensource.org/licenses/RPL-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/RPL-1.5.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "RPL-1.5",
             "name": "Reciprocal Public License 1.5",
             "reference": "https://spdx.org/licenses/RPL-1.5.html",
-            "referenceNumber": 197,
+            "referenceNumber": 136,
             "seeAlso": [
                 "https://opensource.org/licenses/RPL-1.5"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/RPSL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "RPSL-1.0",
             "name": "RealNetworks Public Source License v1.0",
             "reference": "https://spdx.org/licenses/RPSL-1.0.html",
-            "referenceNumber": 221,
+            "referenceNumber": 290,
             "seeAlso": [
                 "https://helixcommunity.org/content/rpsl",
                 "https://opensource.org/licenses/RPSL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/RSA-MD.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "RSA-MD",
             "name": "RSA Message-Digest License",
             "reference": "https://spdx.org/licenses/RSA-MD.html",
-            "referenceNumber": 45,
+            "referenceNumber": 506,
             "seeAlso": [
                 "http://www.faqs.org/rfcs/rfc1321.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/RSCPL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "RSCPL",
             "name": "Ricoh Source Code Public License",
             "reference": "https://spdx.org/licenses/RSCPL.html",
-            "referenceNumber": 147,
+            "referenceNumber": 175,
             "seeAlso": [
                 "http://wayback.archive.org/web/20060715140826/http://www.risource.org/RPL/RPL-1.0A.shtml",
                 "https://opensource.org/licenses/RSCPL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Ruby.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "Ruby",
             "name": "Ruby License",
             "reference": "https://spdx.org/licenses/Ruby.html",
-            "referenceNumber": 227,
+            "referenceNumber": 60,
             "seeAlso": [
                 "http://www.ruby-lang.org/en/LICENSE.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SAX-PD.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SAX-PD",
             "name": "Sax Public Domain Notice",
             "reference": "https://spdx.org/licenses/SAX-PD.html",
-            "referenceNumber": 374,
+            "referenceNumber": 390,
             "seeAlso": [
                 "http://www.saxproject.org/copying.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Saxpath.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Saxpath",
             "name": "Saxpath License",
             "reference": "https://spdx.org/licenses/Saxpath.html",
-            "referenceNumber": 198,
+            "referenceNumber": 372,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Saxpath_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SCEA.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SCEA",
             "name": "SCEA Shared Source License",
             "reference": "https://spdx.org/licenses/SCEA.html",
-            "referenceNumber": 228,
+            "referenceNumber": 179,
             "seeAlso": [
                 "http://research.scea.com/scea_shared_source_license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SchemeReport.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SchemeReport",
             "name": "Scheme Language Report License",
             "reference": "https://spdx.org/licenses/SchemeReport.html",
-            "referenceNumber": 485,
+            "referenceNumber": 39,
             "seeAlso": []
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Sendmail.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Sendmail",
             "name": "Sendmail License",
             "reference": "https://spdx.org/licenses/Sendmail.html",
-            "referenceNumber": 3,
+            "referenceNumber": 27,
             "seeAlso": [
                 "http://www.sendmail.com/pdfs/open_source/sendmail_license.pdf",
                 "https://web.archive.org/web/20160322142305/https://www.sendmail.com/pdfs/open_source/sendmail_license.pdf"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Sendmail-8.23.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Sendmail-8.23",
             "name": "Sendmail License 8.23",
             "reference": "https://spdx.org/licenses/Sendmail-8.23.html",
-            "referenceNumber": 79,
+            "referenceNumber": 344,
             "seeAlso": [
                 "https://www.proofpoint.com/sites/default/files/sendmail-license.pdf",
                 "https://web.archive.org/web/20181003101040/https://www.proofpoint.com/sites/default/files/sendmail-license.pdf"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SGI-B-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SGI-B-1.0",
             "name": "SGI Free Software License B v1.0",
             "reference": "https://spdx.org/licenses/SGI-B-1.0.html",
-            "referenceNumber": 271,
+            "referenceNumber": 122,
             "seeAlso": [
                 "http://oss.sgi.com/projects/FreeB/SGIFreeSWLicB.1.0.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SGI-B-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SGI-B-1.1",
             "name": "SGI Free Software License B v1.1",
             "reference": "https://spdx.org/licenses/SGI-B-1.1.html",
-            "referenceNumber": 487,
+            "referenceNumber": 330,
             "seeAlso": [
                 "http://oss.sgi.com/projects/FreeB/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SGI-B-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "SGI-B-2.0",
             "name": "SGI Free Software License B v2.0",
             "reference": "https://spdx.org/licenses/SGI-B-2.0.html",
-            "referenceNumber": 482,
+            "referenceNumber": 278,
             "seeAlso": [
                 "http://oss.sgi.com/projects/FreeB/SGIFreeSWLicB.2.0.pdf"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/SGP4.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "SGP4",
+            "name": "SGP4 Permission Notice",
+            "reference": "https://spdx.org/licenses/SGP4.html",
+            "referenceNumber": 520,
+            "seeAlso": [
+                "https://celestrak.org/publications/AIAA/2006-6753/faq.php"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/SHL-0.5.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SHL-0.5",
             "name": "Solderpad Hardware License v0.5",
             "reference": "https://spdx.org/licenses/SHL-0.5.html",
-            "referenceNumber": 484,
+            "referenceNumber": 510,
             "seeAlso": [
                 "https://solderpad.org/licenses/SHL-0.5/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SHL-0.51.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SHL-0.51",
             "name": "Solderpad Hardware License, Version 0.51",
             "reference": "https://spdx.org/licenses/SHL-0.51.html",
-            "referenceNumber": 47,
+            "referenceNumber": 492,
             "seeAlso": [
                 "https://solderpad.org/licenses/SHL-0.51/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SimPL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "SimPL-2.0",
             "name": "Simple Public License 2.0",
             "reference": "https://spdx.org/licenses/SimPL-2.0.html",
-            "referenceNumber": 49,
+            "referenceNumber": 387,
             "seeAlso": [
                 "https://opensource.org/licenses/SimPL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SISSL.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "SISSL",
             "name": "Sun Industry Standards Source License v1.1",
             "reference": "https://spdx.org/licenses/SISSL.html",
-            "referenceNumber": 92,
+            "referenceNumber": 199,
             "seeAlso": [
                 "http://www.openoffice.org/licenses/sissl_license.html",
                 "https://opensource.org/licenses/SISSL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SISSL-1.2.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SISSL-1.2",
             "name": "Sun Industry Standards Source License v1.2",
             "reference": "https://spdx.org/licenses/SISSL-1.2.html",
-            "referenceNumber": 430,
+            "referenceNumber": 267,
             "seeAlso": [
                 "http://gridscheduler.sourceforge.net/Gridengine_SISSL_license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Sleepycat.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "Sleepycat",
             "name": "Sleepycat License",
             "reference": "https://spdx.org/licenses/Sleepycat.html",
-            "referenceNumber": 277,
+            "referenceNumber": 170,
             "seeAlso": [
                 "https://opensource.org/licenses/Sleepycat"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SMLNJ.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "SMLNJ",
             "name": "Standard ML of New Jersey License",
             "reference": "https://spdx.org/licenses/SMLNJ.html",
-            "referenceNumber": 69,
+            "referenceNumber": 243,
             "seeAlso": [
                 "https://www.smlnj.org/license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SMPPL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SMPPL",
             "name": "Secure Messaging Protocol Public License",
             "reference": "https://spdx.org/licenses/SMPPL.html",
-            "referenceNumber": 316,
+            "referenceNumber": 399,
             "seeAlso": [
                 "https://github.com/dcblake/SMP/blob/master/Documentation/License.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SNIA.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SNIA",
             "name": "SNIA Public License 1.1",
             "reference": "https://spdx.org/licenses/SNIA.html",
-            "referenceNumber": 38,
+            "referenceNumber": 334,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/SNIA_Public_License"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/snprintf.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "snprintf",
+            "name": "snprintf License",
+            "reference": "https://spdx.org/licenses/snprintf.html",
+            "referenceNumber": 142,
+            "seeAlso": [
+                "https://github.com/openssh/openssh-portable/blob/master/openbsd-compat/bsd-snprintf.c#L2"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Spencer-86.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Spencer-86",
             "name": "Spencer License 86",
             "reference": "https://spdx.org/licenses/Spencer-86.html",
-            "referenceNumber": 97,
+            "referenceNumber": 300,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Henry_Spencer_Reg-Ex_Library_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Spencer-94.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Spencer-94",
             "name": "Spencer License 94",
             "reference": "https://spdx.org/licenses/Spencer-94.html",
-            "referenceNumber": 490,
+            "referenceNumber": 394,
             "seeAlso": [
-                "https://fedoraproject.org/wiki/Licensing/Henry_Spencer_Reg-Ex_Library_License"
+                "https://fedoraproject.org/wiki/Licensing/Henry_Spencer_Reg-Ex_Library_License",
+                "https://metacpan.org/release/KNOK/File-MMagic-1.30/source/COPYING#L28"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Spencer-99.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Spencer-99",
             "name": "Spencer License 99",
             "reference": "https://spdx.org/licenses/Spencer-99.html",
-            "referenceNumber": 462,
+            "referenceNumber": 173,
             "seeAlso": [
                 "http://www.opensource.apple.com/source/tcl/tcl-5/tcl/generic/regfronts.c"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "SPL-1.0",
             "name": "Sun Public License v1.0",
             "reference": "https://spdx.org/licenses/SPL-1.0.html",
-            "referenceNumber": 475,
+            "referenceNumber": 441,
             "seeAlso": [
                 "https://opensource.org/licenses/SPL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SSH-OpenSSH.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SSH-OpenSSH",
             "name": "SSH OpenSSH license",
             "reference": "https://spdx.org/licenses/SSH-OpenSSH.html",
-            "referenceNumber": 26,
+            "referenceNumber": 471,
             "seeAlso": [
                 "https://github.com/openssh/openssh-portable/blob/1b11ea7c58cd5c59838b5fa574cd456d6047b2d4/LICENCE#L10"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SSH-short.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SSH-short",
             "name": "SSH short notice",
             "reference": "https://spdx.org/licenses/SSH-short.html",
-            "referenceNumber": 204,
+            "referenceNumber": 160,
             "seeAlso": [
                 "https://github.com/openssh/openssh-portable/blob/1b11ea7c58cd5c59838b5fa574cd456d6047b2d4/pathnames.h",
                 "http://web.mit.edu/kolya/.f/root/athena.mit.edu/sipb.mit.edu/project/openssh/OldFiles/src/openssh-2.9.9p2/ssh-add.1",
                 "https://joinup.ec.europa.eu/svn/lesoll/trunk/italc/lib/src/dsa_key.cpp"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SSPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SSPL-1.0",
             "name": "Server Side Public License, v 1",
             "reference": "https://spdx.org/licenses/SSPL-1.0.html",
-            "referenceNumber": 207,
+            "referenceNumber": 218,
             "seeAlso": [
                 "https://www.mongodb.com/licensing/server-side-public-license"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/StandardML-NJ.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "StandardML-NJ",
             "name": "Standard ML of New Jersey License",
             "reference": "https://spdx.org/licenses/StandardML-NJ.html",
-            "referenceNumber": 499,
+            "referenceNumber": 226,
             "seeAlso": [
-                "http://www.smlnj.org//license.html"
+                "https://www.smlnj.org/license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SugarCRM-1.1.3.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SugarCRM-1.1.3",
             "name": "SugarCRM Public License v1.1.3",
             "reference": "https://spdx.org/licenses/SugarCRM-1.1.3.html",
-            "referenceNumber": 436,
+            "referenceNumber": 366,
             "seeAlso": [
                 "http://www.sugarcrm.com/crm/SPL"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/SunPro.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "SunPro",
+            "name": "SunPro License",
+            "reference": "https://spdx.org/licenses/SunPro.html",
+            "referenceNumber": 490,
+            "seeAlso": [
+                "https://github.com/freebsd/freebsd-src/blob/main/lib/msun/src/e_acosh.c",
+                "https://github.com/freebsd/freebsd-src/blob/main/lib/msun/src/e_lgammal.c"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/SWL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SWL",
             "name": "Scheme Widget Library (SWL) Software License Agreement",
             "reference": "https://spdx.org/licenses/SWL.html",
-            "referenceNumber": 76,
+            "referenceNumber": 181,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/SWL"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Symlinks.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Symlinks",
+            "name": "Symlinks License",
+            "reference": "https://spdx.org/licenses/Symlinks.html",
+            "referenceNumber": 262,
+            "seeAlso": [
+                "https://www.mail-archive.com/debian-bugs-rc@lists.debian.org/msg11494.html"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/TAPR-OHL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "TAPR-OHL-1.0",
             "name": "TAPR Open Hardware License v1.0",
             "reference": "https://spdx.org/licenses/TAPR-OHL-1.0.html",
-            "referenceNumber": 287,
+            "referenceNumber": 496,
             "seeAlso": [
                 "https://www.tapr.org/OHL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/TCL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "TCL",
             "name": "TCL/TK License",
             "reference": "https://spdx.org/licenses/TCL.html",
-            "referenceNumber": 305,
+            "referenceNumber": 123,
             "seeAlso": [
                 "http://www.tcl.tk/software/tcltk/license.html",
                 "https://fedoraproject.org/wiki/Licensing/TCL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/TCP-wrappers.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "TCP-wrappers",
             "name": "TCP Wrappers License",
             "reference": "https://spdx.org/licenses/TCP-wrappers.html",
-            "referenceNumber": 279,
+            "referenceNumber": 86,
             "seeAlso": [
                 "http://rc.quest.com/topics/openssh/license.php#tcpwrappers"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/TermReadKey.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "TermReadKey",
+            "name": "TermReadKey License",
+            "reference": "https://spdx.org/licenses/TermReadKey.html",
+            "referenceNumber": 489,
+            "seeAlso": [
+                "https://github.com/jonathanstowe/TermReadKey/blob/master/README#L9-L10"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/TMate.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "TMate",
             "name": "TMate Open Source License",
             "reference": "https://spdx.org/licenses/TMate.html",
-            "referenceNumber": 261,
+            "referenceNumber": 35,
             "seeAlso": [
                 "http://svnkit.com/license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/TORQUE-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "TORQUE-1.1",
             "name": "TORQUE v2.5+ Software License v1.1",
             "reference": "https://spdx.org/licenses/TORQUE-1.1.html",
-            "referenceNumber": 28,
+            "referenceNumber": 416,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/TORQUEv1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/TOSL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "TOSL",
             "name": "Trusster Open Source License",
             "reference": "https://spdx.org/licenses/TOSL.html",
-            "referenceNumber": 125,
+            "referenceNumber": 426,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/TOSL"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/TPDL.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "TPDL",
+            "name": "Time::ParseDate License",
+            "reference": "https://spdx.org/licenses/TPDL.html",
+            "referenceNumber": 433,
+            "seeAlso": [
+                "https://metacpan.org/pod/Time::ParseDate#LICENSE"
+            ]
+        },
+        {
+            "detailsUrl": "https://spdx.org/licenses/TPL-1.0.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "TPL-1.0",
+            "name": "THOR Public License 1.0",
+            "reference": "https://spdx.org/licenses/TPL-1.0.html",
+            "referenceNumber": 224,
+            "seeAlso": [
+                "https://fedoraproject.org/wiki/Licensing:ThorPublicLicense"
+            ]
+        },
+        {
+            "detailsUrl": "https://spdx.org/licenses/TTWL.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "TTWL",
+            "name": "Text-Tabs+Wrap License",
+            "reference": "https://spdx.org/licenses/TTWL.html",
+            "referenceNumber": 403,
+            "seeAlso": [
+                "https://fedoraproject.org/wiki/Licensing/TTWL",
+                "https://github.com/ap/Text-Tabs/blob/master/lib.modern/Text/Tabs.pm#L148"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/TU-Berlin-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "TU-Berlin-1.0",
             "name": "Technische Universitaet Berlin License 1.0",
             "reference": "https://spdx.org/licenses/TU-Berlin-1.0.html",
-            "referenceNumber": 185,
+            "referenceNumber": 92,
             "seeAlso": [
                 "https://github.com/swh/ladspa/blob/7bf6f3799fdba70fda297c2d8fd9f526803d9680/gsm/COPYRIGHT"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/TU-Berlin-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "TU-Berlin-2.0",
             "name": "Technische Universitaet Berlin License 2.0",
             "reference": "https://spdx.org/licenses/TU-Berlin-2.0.html",
-            "referenceNumber": 278,
+            "referenceNumber": 326,
             "seeAlso": [
                 "https://github.com/CorsixTH/deps/blob/fd339a9f526d1d9c9f01ccf39e438a015da50035/licences/libgsm.txt"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/UCAR.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "UCAR",
+            "name": "UCAR License",
+            "reference": "https://spdx.org/licenses/UCAR.html",
+            "referenceNumber": 454,
+            "seeAlso": [
+                "https://github.com/Unidata/UDUNITS-2/blob/master/COPYRIGHT"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/UCL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "UCL-1.0",
             "name": "Upstream Compatibility License v1.0",
             "reference": "https://spdx.org/licenses/UCL-1.0.html",
-            "referenceNumber": 213,
+            "referenceNumber": 414,
             "seeAlso": [
                 "https://opensource.org/licenses/UCL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Unicode-DFS-2015.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Unicode-DFS-2015",
             "name": "Unicode License Agreement - Data Files and Software (2015)",
             "reference": "https://spdx.org/licenses/Unicode-DFS-2015.html",
-            "referenceNumber": 295,
+            "referenceNumber": 291,
             "seeAlso": [
                 "https://web.archive.org/web/20151224134844/http://unicode.org/copyright.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Unicode-DFS-2016.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Unicode-DFS-2016",
             "name": "Unicode License Agreement - Data Files and Software (2016)",
             "reference": "https://spdx.org/licenses/Unicode-DFS-2016.html",
-            "referenceNumber": 164,
+            "referenceNumber": 544,
             "seeAlso": [
+                "https://www.unicode.org/license.txt",
+                "http://web.archive.org/web/20160823201924/http://www.unicode.org/copyright.html#License",
                 "http://www.unicode.org/copyright.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Unicode-TOU.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Unicode-TOU",
             "name": "Unicode Terms of Use",
             "reference": "https://spdx.org/licenses/Unicode-TOU.html",
-            "referenceNumber": 95,
+            "referenceNumber": 268,
             "seeAlso": [
+                "http://web.archive.org/web/20140704074106/http://www.unicode.org/copyright.html",
                 "http://www.unicode.org/copyright.html"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/UnixCrypt.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "UnixCrypt",
+            "name": "UnixCrypt License",
+            "reference": "https://spdx.org/licenses/UnixCrypt.html",
+            "referenceNumber": 48,
+            "seeAlso": [
+                "https://foss.heptapod.net/python-libs/passlib/-/blob/branch/stable/LICENSE#L70",
+                "https://opensource.apple.com/source/JBoss/JBoss-737/jboss-all/jetty/src/main/org/mortbay/util/UnixCrypt.java.auto.html",
+                "https://archive.eclipse.org/jetty/8.0.1.v20110908/xref/org/eclipse/jetty/http/security/UnixCrypt.html"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Unlicense.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "Unlicense",
             "name": "The Unlicense",
             "reference": "https://spdx.org/licenses/Unlicense.html",
-            "referenceNumber": 406,
+            "referenceNumber": 137,
             "seeAlso": [
                 "https://unlicense.org/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/UPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "UPL-1.0",
             "name": "Universal Permissive License v1.0",
             "reference": "https://spdx.org/licenses/UPL-1.0.html",
-            "referenceNumber": 426,
+            "referenceNumber": 204,
             "seeAlso": [
                 "https://opensource.org/licenses/UPL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Vim.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "Vim",
             "name": "Vim License",
             "reference": "https://spdx.org/licenses/Vim.html",
-            "referenceNumber": 376,
+            "referenceNumber": 526,
             "seeAlso": [
                 "http://vimdoc.sourceforge.net/htmldoc/uganda.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/VOSTROM.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "VOSTROM",
             "name": "VOSTROM Public License for Open Source",
             "reference": "https://spdx.org/licenses/VOSTROM.html",
-            "referenceNumber": 200,
+            "referenceNumber": 6,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/VOSTROM"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/VSL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "VSL-1.0",
             "name": "Vovida Software License v1.0",
             "reference": "https://spdx.org/licenses/VSL-1.0.html",
-            "referenceNumber": 158,
+            "referenceNumber": 153,
             "seeAlso": [
                 "https://opensource.org/licenses/VSL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/W3C.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "W3C",
             "name": "W3C Software Notice and License (2002-12-31)",
             "reference": "https://spdx.org/licenses/W3C.html",
-            "referenceNumber": 27,
+            "referenceNumber": 335,
             "seeAlso": [
                 "http://www.w3.org/Consortium/Legal/2002/copyright-software-20021231.html",
                 "https://opensource.org/licenses/W3C"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/W3C-19980720.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "W3C-19980720",
             "name": "W3C Software Notice and License (1998-07-20)",
             "reference": "https://spdx.org/licenses/W3C-19980720.html",
-            "referenceNumber": 249,
+            "referenceNumber": 408,
             "seeAlso": [
                 "http://www.w3.org/Consortium/Legal/copyright-software-19980720.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/W3C-20150513.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "W3C-20150513",
             "name": "W3C Software Notice and Document License (2015-05-13)",
             "reference": "https://spdx.org/licenses/W3C-20150513.html",
-            "referenceNumber": 240,
+            "referenceNumber": 9,
             "seeAlso": [
                 "https://www.w3.org/Consortium/Legal/2015/copyright-software-and-document"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/w3m.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "w3m",
+            "name": "w3m License",
+            "reference": "https://spdx.org/licenses/w3m.html",
+            "referenceNumber": 37,
+            "seeAlso": [
+                "https://github.com/tats/w3m/blob/master/COPYING"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Watcom-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": true,
             "licenseId": "Watcom-1.0",
             "name": "Sybase Open Watcom Public License 1.0",
             "reference": "https://spdx.org/licenses/Watcom-1.0.html",
-            "referenceNumber": 381,
+            "referenceNumber": 185,
             "seeAlso": [
                 "https://opensource.org/licenses/Watcom-1.0"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Widget-Workshop.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Widget-Workshop",
+            "name": "Widget Workshop License",
+            "reference": "https://spdx.org/licenses/Widget-Workshop.html",
+            "referenceNumber": 364,
+            "seeAlso": [
+                "https://github.com/novnc/noVNC/blob/master/core/crypto/des.js#L24"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Wsuipa.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Wsuipa",
             "name": "Wsuipa License",
             "reference": "https://spdx.org/licenses/Wsuipa.html",
-            "referenceNumber": 20,
+            "referenceNumber": 440,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Wsuipa"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/WTFPL.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "WTFPL",
             "name": "Do What The F*ck You Want To Public License",
             "reference": "https://spdx.org/licenses/WTFPL.html",
-            "referenceNumber": 142,
+            "referenceNumber": 511,
             "seeAlso": [
                 "http://www.wtfpl.net/about/",
                 "http://sam.zoy.org/wtfpl/COPYING"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/wxWindows.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": true,
             "licenseId": "wxWindows",
             "name": "wxWindows Library License",
             "reference": "https://spdx.org/licenses/wxWindows.html",
-            "referenceNumber": 220,
+            "referenceNumber": 57,
             "seeAlso": [
                 "https://opensource.org/licenses/WXwindows"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/X11.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "X11",
             "name": "X11 License",
             "reference": "https://spdx.org/licenses/X11.html",
-            "referenceNumber": 23,
+            "referenceNumber": 504,
             "seeAlso": [
                 "http://www.xfree86.org/3.3.6/COPYRIGHT2.html#3"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/X11-distribute-modifications-variant.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "X11-distribute-modifications-variant",
             "name": "X11 License Distribution Modification Variant",
             "reference": "https://spdx.org/licenses/X11-distribute-modifications-variant.html",
-            "referenceNumber": 248,
+            "referenceNumber": 288,
             "seeAlso": [
                 "https://github.com/mirror/ncurses/blob/master/COPYING"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Xdebug-1.03.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Xdebug-1.03",
+            "name": "Xdebug License v 1.03",
+            "reference": "https://spdx.org/licenses/Xdebug-1.03.html",
+            "referenceNumber": 127,
+            "seeAlso": [
+                "https://github.com/xdebug/xdebug/blob/master/LICENSE"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Xerox.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Xerox",
             "name": "Xerox License",
             "reference": "https://spdx.org/licenses/Xerox.html",
-            "referenceNumber": 170,
+            "referenceNumber": 180,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Xerox"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Xfig.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Xfig",
+            "name": "Xfig License",
+            "reference": "https://spdx.org/licenses/Xfig.html",
+            "referenceNumber": 255,
+            "seeAlso": [
+                "https://github.com/Distrotech/transfig/blob/master/transfig/transfig.c",
+                "https://fedoraproject.org/wiki/Licensing:MIT#Xfig_Variant",
+                "https://sourceforge.net/p/mcj/xfig/ci/master/tree/src/Makefile.am"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/XFree86-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "XFree86-1.1",
             "name": "XFree86 License 1.1",
             "reference": "https://spdx.org/licenses/XFree86-1.1.html",
-            "referenceNumber": 243,
+            "referenceNumber": 138,
             "seeAlso": [
                 "http://www.xfree86.org/current/LICENSE4.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/xinetd.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "xinetd",
             "name": "xinetd License",
             "reference": "https://spdx.org/licenses/xinetd.html",
-            "referenceNumber": 58,
+            "referenceNumber": 312,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Xinetd_License"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/xlock.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "xlock",
+            "name": "xlock License",
+            "reference": "https://spdx.org/licenses/xlock.html",
+            "referenceNumber": 343,
+            "seeAlso": [
+                "https://fossies.org/linux/tiff/contrib/ras/ras2tif.c"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Xnet.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Xnet",
             "name": "X.Net License",
             "reference": "https://spdx.org/licenses/Xnet.html",
-            "referenceNumber": 64,
+            "referenceNumber": 119,
             "seeAlso": [
                 "https://opensource.org/licenses/Xnet"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/xpp.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "xpp",
             "name": "XPP License",
             "reference": "https://spdx.org/licenses/xpp.html",
-            "referenceNumber": 396,
+            "referenceNumber": 407,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/xpp"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/XSkat.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "XSkat",
             "name": "XSkat License",
             "reference": "https://spdx.org/licenses/XSkat.html",
-            "referenceNumber": 373,
+            "referenceNumber": 46,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/XSkat_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/YPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "YPL-1.0",
             "name": "Yahoo! Public License v1.0",
             "reference": "https://spdx.org/licenses/YPL-1.0.html",
-            "referenceNumber": 270,
+            "referenceNumber": 76,
             "seeAlso": [
                 "http://www.zimbra.com/license/yahoo_public_license_1.0.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/YPL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "YPL-1.1",
             "name": "Yahoo! Public License v1.1",
             "reference": "https://spdx.org/licenses/YPL-1.1.html",
-            "referenceNumber": 358,
+            "referenceNumber": 215,
             "seeAlso": [
                 "http://www.zimbra.com/license/yahoo_public_license_1.1.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Zed.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Zed",
             "name": "Zed License",
             "reference": "https://spdx.org/licenses/Zed.html",
-            "referenceNumber": 302,
+            "referenceNumber": 532,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Zed"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Zend-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "Zend-2.0",
             "name": "Zend License v2.0",
             "reference": "https://spdx.org/licenses/Zend-2.0.html",
-            "referenceNumber": 174,
+            "referenceNumber": 373,
             "seeAlso": [
                 "https://web.archive.org/web/20130517195954/http://www.zend.com/license/2_00.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Zimbra-1.3.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "Zimbra-1.3",
             "name": "Zimbra Public License v1.3",
             "reference": "https://spdx.org/licenses/Zimbra-1.3.html",
-            "referenceNumber": 166,
+            "referenceNumber": 107,
             "seeAlso": [
                 "http://web.archive.org/web/20100302225219/http://www.zimbra.com/license/zimbra-public-license-1-3.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Zimbra-1.4.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Zimbra-1.4",
             "name": "Zimbra Public License v1.4",
             "reference": "https://spdx.org/licenses/Zimbra-1.4.html",
-            "referenceNumber": 172,
+            "referenceNumber": 121,
             "seeAlso": [
                 "http://www.zimbra.com/legal/zimbra-public-license-1-4"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Zlib.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "Zlib",
             "name": "zlib License",
             "reference": "https://spdx.org/licenses/Zlib.html",
-            "referenceNumber": 252,
+            "referenceNumber": 73,
             "seeAlso": [
                 "http://www.zlib.net/zlib_license.html",
                 "https://opensource.org/licenses/Zlib"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/zlib-acknowledgement.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "zlib-acknowledgement",
             "name": "zlib/libpng License with Acknowledgement",
             "reference": "https://spdx.org/licenses/zlib-acknowledgement.html",
-            "referenceNumber": 232,
+            "referenceNumber": 362,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/ZlibWithAcknowledgement"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ZPL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "ZPL-1.1",
             "name": "Zope Public License 1.1",
             "reference": "https://spdx.org/licenses/ZPL-1.1.html",
-            "referenceNumber": 9,
+            "referenceNumber": 498,
             "seeAlso": [
                 "http://old.zope.org/Resources/License/ZPL-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ZPL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "ZPL-2.0",
             "name": "Zope Public License 2.0",
             "reference": "https://spdx.org/licenses/ZPL-2.0.html",
-            "referenceNumber": 318,
+            "referenceNumber": 82,
             "seeAlso": [
                 "http://old.zope.org/Resources/License/ZPL-2.0",
                 "https://opensource.org/licenses/ZPL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ZPL-2.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "ZPL-2.1",
             "name": "Zope Public License 2.1",
             "reference": "https://spdx.org/licenses/ZPL-2.1.html",
-            "referenceNumber": 66,
+            "referenceNumber": 101,
             "seeAlso": [
                 "http://old.zope.org/Resources/ZPL/"
             ]
         }
     ],
-    "releaseDate": "2022-11-23"
+    "releaseDate": "2023-06-21"
 }
```

