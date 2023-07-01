# Comparing `tmp/fnattr-0.2.8.tar.gz` & `tmp/fnattr-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnattr-0.2.8.tar", last modified: Thu Jun 15 14:54:49 2023, max compression
+gzip compressed data, was "fnattr-0.2.9.tar", last modified: Sat Jul  1 14:01:30 2023, max compression
```

## Comparing `fnattr-0.2.8.tar` & `fnattr-0.2.9.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1057 2023-05-06 18:55:15.000000 fnattr-0.2.8/LICENSE
--rw-rw-r--   0 kevin     (1001) dialout     (20)       31 2023-05-07 00:42:08.000000 fnattr-0.2.8/MANIFEST.in
--rw-rw-r--   0 kevin     (1001) dialout     (20)     5174 2023-06-15 14:54:49.000000 fnattr-0.2.8/PKG-INFO
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4523 2023-06-03 16:51:05.000000 fnattr-0.2.8/README.md
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/config/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1638 2023-05-27 20:42:39.000000 fnattr-0.2.8/config/vlju.toml
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/doc/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2976 2023-05-31 13:53:09.000000 fnattr-0.2.8/doc/configuration.md
--rw-rw-r--   0 kevin     (1001) dialout     (20)    10407 2023-05-25 00:54:41.000000 fnattr-0.2.8/doc/fna.md
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4501 2023-05-30 12:57:29.000000 fnattr-0.2.8/doc/keys.md
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4685 2023-06-15 14:44:48.000000 fnattr-0.2.8/pyproject.toml
--rw-rw-r--   0 kevin     (1001) dialout     (20)       38 2023-06-15 14:54:49.000000 fnattr-0.2.8/setup.cfg
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/extra/
--rw-rw-r--   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/extra/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     6253 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/extra/danname.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     8832 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/extra/fnaffle.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4547 2023-06-08 03:14:19.000000 fnattr-0.2.8/src/fnattr/extra/make_isbn_ranges.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     9356 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/extra/tellico_sqlite3_rename.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/fna/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3788 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/fna/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/util/
--rw-rw-r--   0 kevin     (1001) dialout     (20)       23 2023-05-30 23:01:42.000000 fnattr-0.2.8/src/fnattr/util/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      778 2023-05-30 23:01:42.000000 fnattr-0.2.8/src/fnattr/util/checksum.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4693 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/util/config.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      625 2023-05-30 23:01:42.000000 fnattr-0.2.8/src/fnattr/util/docsplit.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     9200 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/util/duration.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      102 2023-05-30 23:01:43.000000 fnattr-0.2.8/src/fnattr/util/error.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2181 2023-05-30 23:01:43.000000 fnattr-0.2.8/src/fnattr/util/escape.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1243 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/util/fearmat.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1857 2023-05-30 23:01:43.000000 fnattr-0.2.8/src/fnattr/util/io.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      560 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/util/log.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3535 2023-05-30 23:01:43.000000 fnattr-0.2.8/src/fnattr/util/multimap.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2157 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/util/nested.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1063 2023-05-30 23:01:43.000000 fnattr-0.2.8/src/fnattr/util/pytestutil.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1738 2023-05-30 23:01:43.000000 fnattr-0.2.8/src/fnattr/util/registry.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1099 2023-05-30 23:01:43.000000 fnattr-0.2.8/src/fnattr/util/repr.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     8362 2023-06-12 19:21:48.000000 fnattr-0.2.8/src/fnattr/util/sqlite.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      472 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/util/typecheck.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1797 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      401 2023-05-30 23:01:44.000000 fnattr-0.2.8/src/fnattr/vlju/testutil.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/
--rw-rw-r--   0 kevin     (1001) dialout     (20)       23 2023-05-30 23:01:44.000000 fnattr-0.2.8/src/fnattr/vlju/types/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      920 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/all.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/doi/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4175 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/doi/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)  1136932 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/doi/org.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/ean/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1687 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/ean/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3214 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/ean/isbn.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)    40480 2023-05-30 23:01:45.000000 fnattr-0.2.8/src/fnattr/vlju/types/ean/isbn_ranges.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      666 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/ean/ismn.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1307 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/ean/issn.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/file/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1998 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/file/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/info/
--rw-rw-r--   0 kevin     (1001) dialout     (20)      983 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/info/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2870 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/info/kinds.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/lccn/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1282 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/lccn/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/site/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3990 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/site/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/timestamp/
--rw-rw-r--   0 kevin     (1001) dialout     (20)      888 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/timestamp/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/uri/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     8655 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/uri/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/url/
--rw-rw-r--   0 kevin     (1001) dialout     (20)      772 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/url/__init__.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vlju/types/urn/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1372 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/urn/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4046 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vlju/types/urn/kinds.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vljum/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     9288 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/vljum/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3136 2023-06-15 14:30:53.000000 fnattr-0.2.8/src/fnattr/vljum/m.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)    10570 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vljum/runner.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr/vljumap/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1218 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vljumap/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)    23350 2023-06-12 19:21:48.000000 fnattr-0.2.8/src/fnattr/vljumap/enc.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1357 2023-05-30 23:01:46.000000 fnattr-0.2.8/src/fnattr/vljumap/factory.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr.egg-info/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     5174 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr.egg-info/PKG-INFO
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1843 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr.egg-info/SOURCES.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)        1 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr.egg-info/dependency_links.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)       76 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr.egg-info/entry_points.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)        7 2023-06-15 14:54:49.000000 fnattr-0.2.8/src/fnattr.egg-info/top_level.txt
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:30.000000 fnattr-0.2.9/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1057 2023-05-06 18:55:15.000000 fnattr-0.2.9/LICENSE
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       31 2023-05-07 00:42:08.000000 fnattr-0.2.9/MANIFEST.in
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5174 2023-07-01 14:01:30.000000 fnattr-0.2.9/PKG-INFO
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4523 2023-06-03 16:51:05.000000 fnattr-0.2.9/README.md
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:29.000000 fnattr-0.2.9/config/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1638 2023-05-27 20:42:39.000000 fnattr-0.2.9/config/vlju.toml
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:29.000000 fnattr-0.2.9/doc/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3563 2023-06-26 14:22:25.000000 fnattr-0.2.9/doc/configuration.md
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    10407 2023-05-25 00:54:41.000000 fnattr-0.2.9/doc/fna.md
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4501 2023-05-30 12:57:29.000000 fnattr-0.2.9/doc/keys.md
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4685 2023-07-01 13:59:32.000000 fnattr-0.2.9/pyproject.toml
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       38 2023-07-01 14:01:30.000000 fnattr-0.2.9/setup.cfg
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:29.000000 fnattr-0.2.9/src/
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:29.000000 fnattr-0.2.9/src/fnattr/
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:29.000000 fnattr-0.2.9/src/fnattr/extra/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)        0 2023-06-15 14:30:53.000000 fnattr-0.2.9/src/fnattr/extra/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     6228 2023-07-01 13:57:58.000000 fnattr-0.2.9/src/fnattr/extra/danname.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     8807 2023-07-01 13:57:58.000000 fnattr-0.2.9/src/fnattr/extra/fnaffle.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4547 2023-06-08 03:14:19.000000 fnattr-0.2.9/src/fnattr/extra/make_isbn_ranges.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     9248 2023-07-01 13:56:59.000000 fnattr-0.2.9/src/fnattr/extra/tellico_sqlite3_rename.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:29.000000 fnattr-0.2.9/src/fnattr/fna/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4238 2023-07-01 03:12:47.000000 fnattr-0.2.9/src/fnattr/fna/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:30.000000 fnattr-0.2.9/src/fnattr/util/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       23 2023-05-30 23:01:42.000000 fnattr-0.2.9/src/fnattr/util/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      778 2023-05-30 23:01:42.000000 fnattr-0.2.9/src/fnattr/util/checksum.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4566 2023-06-30 17:47:16.000000 fnattr-0.2.9/src/fnattr/util/config.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      625 2023-05-30 23:01:42.000000 fnattr-0.2.9/src/fnattr/util/docsplit.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     9200 2023-05-30 23:01:46.000000 fnattr-0.2.9/src/fnattr/util/duration.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      102 2023-05-30 23:01:43.000000 fnattr-0.2.9/src/fnattr/util/error.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2181 2023-05-30 23:01:43.000000 fnattr-0.2.9/src/fnattr/util/escape.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1243 2023-06-15 14:30:53.000000 fnattr-0.2.9/src/fnattr/util/fearmat.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1857 2023-05-30 23:01:43.000000 fnattr-0.2.9/src/fnattr/util/io.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      860 2023-07-01 03:12:28.000000 fnattr-0.2.9/src/fnattr/util/log.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3535 2023-05-30 23:01:43.000000 fnattr-0.2.9/src/fnattr/util/multimap.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2157 2023-06-15 14:30:53.000000 fnattr-0.2.9/src/fnattr/util/nested.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2037 2023-07-01 01:40:01.000000 fnattr-0.2.9/src/fnattr/util/pytestutil.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1738 2023-05-30 23:01:43.000000 fnattr-0.2.9/src/fnattr/util/registry.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1099 2023-05-30 23:01:43.000000 fnattr-0.2.9/src/fnattr/util/repr.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     8362 2023-06-12 19:21:48.000000 fnattr-0.2.9/src/fnattr/util/sqlite.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      479 2023-06-28 01:27:42.000000 fnattr-0.2.9/src/fnattr/util/typecheck.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:30.000000 fnattr-0.2.9/src/fnattr/vlju/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1797 2023-05-30 23:01:46.000000 fnattr-0.2.9/src/fnattr/vlju/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      401 2023-05-30 23:01:44.000000 fnattr-0.2.9/src/fnattr/vlju/testutil.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:30.000000 fnattr-0.2.9/src/fnattr/vlju/types/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       23 2023-05-30 23:01:44.000000 fnattr-0.2.9/src/fnattr/vlju/types/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      910 2023-07-01 13:59:31.000000 fnattr-0.2.9/src/fnattr/vlju/types/all.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:30.000000 fnattr-0.2.9/src/fnattr/vlju/types/doi/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4175 2023-05-30 23:01:46.000000 fnattr-0.2.9/src/fnattr/vlju/types/doi/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)  1136932 2023-05-30 23:01:46.000000 fnattr-0.2.9/src/fnattr/vlju/types/doi/org.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:30.000000 fnattr-0.2.9/src/fnattr/vlju/types/ean/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1687 2023-05-30 23:01:46.000000 fnattr-0.2.9/src/fnattr/vlju/types/ean/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3214 2023-05-30 23:01:46.000000 fnattr-0.2.9/src/fnattr/vlju/types/ean/isbn.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    40480 2023-05-30 23:01:45.000000 fnattr-0.2.9/src/fnattr/vlju/types/ean/isbn_ranges.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      666 2023-05-30 23:01:46.000000 fnattr-0.2.9/src/fnattr/vlju/types/ean/ismn.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1307 2023-05-30 23:01:46.000000 fnattr-0.2.9/src/fnattr/vlju/types/ean/issn.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:30.000000 fnattr-0.2.9/src/fnattr/vlju/types/file/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1998 2023-05-30 23:01:46.000000 fnattr-0.2.9/src/fnattr/vlju/types/file/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:30.000000 fnattr-0.2.9/src/fnattr/vlju/types/info/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      983 2023-05-30 23:01:46.000000 fnattr-0.2.9/src/fnattr/vlju/types/info/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2850 2023-07-01 13:59:31.000000 fnattr-0.2.9/src/fnattr/vlju/types/info/kinds.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:30.000000 fnattr-0.2.9/src/fnattr/vlju/types/lccn/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1282 2023-05-30 23:01:46.000000 fnattr-0.2.9/src/fnattr/vlju/types/lccn/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:30.000000 fnattr-0.2.9/src/fnattr/vlju/types/site/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3990 2023-05-30 23:01:46.000000 fnattr-0.2.9/src/fnattr/vlju/types/site/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:30.000000 fnattr-0.2.9/src/fnattr/vlju/types/timestamp/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      888 2023-05-30 23:01:46.000000 fnattr-0.2.9/src/fnattr/vlju/types/timestamp/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:30.000000 fnattr-0.2.9/src/fnattr/vlju/types/uri/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     8655 2023-05-30 23:01:46.000000 fnattr-0.2.9/src/fnattr/vlju/types/uri/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:30.000000 fnattr-0.2.9/src/fnattr/vlju/types/url/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      772 2023-05-30 23:01:46.000000 fnattr-0.2.9/src/fnattr/vlju/types/url/__init__.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:30.000000 fnattr-0.2.9/src/fnattr/vlju/types/urn/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1372 2023-05-30 23:01:46.000000 fnattr-0.2.9/src/fnattr/vlju/types/urn/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4046 2023-05-30 23:01:46.000000 fnattr-0.2.9/src/fnattr/vlju/types/urn/kinds.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:30.000000 fnattr-0.2.9/src/fnattr/vljum/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     9288 2023-06-15 14:30:53.000000 fnattr-0.2.9/src/fnattr/vljum/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3136 2023-06-15 14:30:53.000000 fnattr-0.2.9/src/fnattr/vljum/m.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    10570 2023-05-30 23:01:46.000000 fnattr-0.2.9/src/fnattr/vljum/runner.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:30.000000 fnattr-0.2.9/src/fnattr/vljumap/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1218 2023-05-30 23:01:46.000000 fnattr-0.2.9/src/fnattr/vljumap/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    23350 2023-06-12 19:21:48.000000 fnattr-0.2.9/src/fnattr/vljumap/enc.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1357 2023-05-30 23:01:46.000000 fnattr-0.2.9/src/fnattr/vljumap/factory.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-07-01 14:01:29.000000 fnattr-0.2.9/src/fnattr.egg-info/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5174 2023-07-01 14:01:29.000000 fnattr-0.2.9/src/fnattr.egg-info/PKG-INFO
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1843 2023-07-01 14:01:29.000000 fnattr-0.2.9/src/fnattr.egg-info/SOURCES.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)        1 2023-07-01 14:01:29.000000 fnattr-0.2.9/src/fnattr.egg-info/dependency_links.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       76 2023-07-01 14:01:29.000000 fnattr-0.2.9/src/fnattr.egg-info/entry_points.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)        7 2023-07-01 14:01:29.000000 fnattr-0.2.9/src/fnattr.egg-info/top_level.txt
```

### Comparing `fnattr-0.2.8/LICENSE` & `fnattr-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/PKG-INFO` & `fnattr-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnattr
-Version: 0.2.8
+Version: 0.2.9
 Summary: Manage key/value metadata in file names.
 License: MIT License
 Project-URL: repository, https://codeberg.org/datatravelandexperiments/fna
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fnattr-0.2.8/README.md` & `fnattr-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/config/vlju.toml` & `fnattr-0.2.9/config/vlju.toml`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/doc/configuration.md` & `fnattr-0.2.9/doc/configuration.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 # Configuration
 
 Configuration files are in [TOML](https://toml.io/) form.
 
-## Default configuration files
+## Files
 
-Unless otherwise directed by a command line option,
-`fna` tries to read `fnattr/vlju.toml` and/or `fnattr/fna.toml`
-under XDG locations (e.g. `$XDG_CONFIG_HOME/` or `$HOME/.config/`).
-The former — `vlju.toml` — is shared by all tools
+`fna` first tries to read fixed configuration files,
+and then any files named by `--config` command line options, in order.
+Later files override earlier ones.
+
+For fixed configuration files, `fna` follows
+[XDG conventions](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html).
+The highest priority location is `$XDG_CONFIG_HOME`,
+or if that is not set, `$HOME/.config`.
+Next are the directories given by `$XDG_CONFIG_DIRS`,
+or if that is not set, `/etc/xdg`.
+(If configuration files are present in multiple such locations,
+they are read in the opposite order, so that the first listed has priority.)
+
+`fna` first reads any `fnattr/vlju.toml` in those locations,
+and then any `fnattr/fna.toml`.
+(For clarity, _all_ of the former will be read before _any_ of the latter.)
+The former — `vlju.toml` — is shared by all tools
 using the Vlju library; the latter applies only to the `fna` command.
 
 ## Sections
 
 ### `[option]`
 
 An `[option]` section can contain key-value pairs corresponding
```

### Comparing `fnattr-0.2.8/doc/fna.md` & `fnattr-0.2.9/doc/fna.md`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/doc/keys.md` & `fnattr-0.2.9/doc/keys.md`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/pyproject.toml` & `fnattr-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fnattr"
-version = "0.2.8"
+version = "0.2.9"
 description = "Manage key/value metadata in file names."
 license.text = "MIT License"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
```

### Comparing `fnattr-0.2.8/src/fnattr/extra/danname.py` & `fnattr-0.2.9/src/fnattr/extra/danname.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         help='Merge with existing attributes.')
     parser.add_argument(
         '--log-level',
         '-L',
         metavar='LEVEL',
         type=str,
         choices=log.CHOICES,
-        default='info')
+        default=log.level_name(logging.INFO))
     parser.add_argument(
         '--url',
         '-u',
         metavar='URL',
         type=str,
         default='https://danbooru.donmai.us/')
     parser.add_argument('--user', '-U', metavar='USER', type=str)
@@ -149,15 +149,15 @@
         metavar='FILENAME',
         type=str,
         nargs=argparse.REMAINDER,
         default=[],
         help='File name(s).')
     args = parser.parse_args(argv[1 :])
 
-    log.level(cmd, args.log_level, dryrun=args.dryrun)
+    log_level = log.config(cmd, args)
     config, options = read_cmd_configs_and_merge_options(
         ['fnaffle', cmd],
         args.config,
         args,
         decoder='v3',
         encoder='v3',
         user={'option': 'provider.danbooru.user'},
@@ -202,13 +202,13 @@
     return 0
 
 def main(argv: list[str] | None = None) -> int:
     try:
         return run(argv)
     except Exception as e:
         logging.error('Unhandled exception: %s%s', type(e).__name__, e.args)
-        if logging.getLogger().getEffectiveLevel() < logging.INFO:
+        if log_level < logging.INFO:
             raise
-        return 1
+        return 2
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `fnattr-0.2.8/src/fnattr/extra/fnaffle.py` & `fnattr-0.2.9/src/fnattr/extra/fnaffle.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,24 +250,24 @@
         help='Renaming map file.')
     parser.add_argument(
         '--log-level',
         '-L',
         metavar='LEVEL',
         type=str,
         choices=log.CHOICES,
-        default='WARNING')
+        default=log.level_name(logging.WARNING))
     parser.add_argument(
         'file',
         metavar='FILENAME',
         type=str,
         nargs=argparse.REMAINDER,
         default=[],
         help='File name(s).')
     args = parser.parse_args(argv[1 :])
-    log.level(cmd, args.log_level, dryrun=args.dryrun)
+    log_level = log.config(cmd, args)
     config, options = read_cmd_configs_and_merge_options(
         cmd, args.config, args, decoder='v3')
     M.configure_options(options)
     #   M.configure_sites(config.get('site', {}))
 
     d = Destinations.from_config(config)
     for file in args.file:
@@ -280,13 +280,13 @@
     return 0
 
 def main(argv: list[str] | None = None) -> int:
     try:
         return run(argv)
     except Exception as e:
         logging.error('Unhandled exception: %s%s', type(e).__name__, e.args)
-        if logging.getLogger().getEffectiveLevel() < logging.INFO:
+        if log_level < logging.INFO:
             raise
-        return 1
+        return 2
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `fnattr-0.2.8/src/fnattr/extra/make_isbn_ranges.py` & `fnattr-0.2.9/src/fnattr/extra/make_isbn_ranges.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/extra/tellico_sqlite3_rename.py` & `fnattr-0.2.9/src/fnattr/extra/tellico_sqlite3_rename.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import os
 import re
 import sys
 
 from pathlib import Path
 from typing import Any
 
+from fnattr.util import log
 from fnattr.util.config import read_cmd_configs_and_merge_options
 from fnattr.util.sqlite import SQLite
 from fnattr.vlju.types.all import DOI
 from fnattr.vljum.m import M
 from fnattr.vljumap import enc
 
 COLUMNS = [
@@ -223,34 +224,31 @@
         action='store_true',
         help='Ignore hash collisions; use first entry.')
     parser.add_argument(
         '--log-level',
         '-L',
         metavar='LEVEL',
         type=str,
-        choices=[c for c in logging.getLevelNamesMapping() if c != 'NOTSET'],
-        default='INFO')
+        choices=log.CHOICES,
+        default=log.level_name(logging.INFO))
     parser.add_argument('--sha', action='store_true', help='Print SHA1 only.')
     parser.add_argument(
         '--the',
         choices=('start', 'end', 'none'),
         help='Move ‘The’ in titles.',
     )
     parser.add_argument(
         'files',
         metavar='FILE',
         type=str,
         nargs='+',
         help='Files to rename',
     )
     args = parser.parse_args(argv[1 :])
-
-    logging.basicConfig(
-        level=getattr(logging, args.log_level.upper()),
-        format=f'{cmd}: %(levelname)s: %(message)s')
+    log.config(cmd, args)
 
     _config, options = read_cmd_configs_and_merge_options(
         cmd,
         args.config,
         args,
         db=None,
         table='ebooks',
```

### Comparing `fnattr-0.2.8/src/fnattr/fna/__init__.py` & `fnattr-0.2.9/src/fnattr/fna/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 
 import argparse
 import logging
 import pathlib
 import sys
 
 import fnattr.util.config
+import fnattr.util.error
 import fnattr.util.io
 import fnattr.util.log
 import fnattr.vljum.m
 import fnattr.vljum.runner
 import fnattr.vljumap.enc
 
 def main(argv: list[str] | None = None) -> int:
-    if argv is None:
-        argv = sys.argv
+    if argv is None:        # pragma: no branch
+        argv = sys.argv     # pragma: no cover
     cmd = pathlib.Path(argv[0]).stem
     parser = argparse.ArgumentParser(
         prog=cmd,
         description='Manage key/value attributes in file names',
         epilog=(f'For a list of subcommands, run `{cmd} help`. '
                 f'For information on a specific subcommand, '
                 f'run `{cmd} help ‹subcommand›`'))
@@ -27,14 +28,20 @@
         '--config',
         '-c',
         metavar='FILE',
         type=str,
         action='append',
         help='Configuration file.')
     parser.add_argument(
+        '--no-default-config',
+        dest='default_config',
+        action='store_false',
+        default=True,
+        help='Read default configuration files.')
+    parser.add_argument(
         '--decoder',
         '-d',
         metavar='DECODER',
         type=str,
         choices=fnattr.vljumap.enc.decoder.keys(),
         help='Default string decoder.')
     parser.add_argument(
@@ -46,15 +53,15 @@
         help='Default string encoder.')
     parser.add_argument(
         '--log-level',
         '-L',
         metavar='LEVEL',
         type=str,
         choices=fnattr.util.log.CHOICES,
-        default='WARNING')
+        default=fnattr.util.log.level_name(logging.WARNING))
     mode = parser.add_mutually_exclusive_group()
     mode.add_argument(
         '--dsl',
         '-D',
         dest='mode',
         default='dsl',
         const='dsl',
@@ -86,15 +93,15 @@
         metavar='ARGUMENT',
         type=str,
         nargs=argparse.REMAINDER,
         default=[],
         help='Part of a subcommand, or an expression or statement.')
     args = parser.parse_args(argv[1 :])
 
-    log.level(cmd, args.log_level)
+    log_level = fnattr.util.log.config(cmd, args)
 
     config, options = fnattr.util.config.read_cmd_configs_and_merge_options(
         cmd,
         args.config,
         args,
         decoder='v3',
         encoder='v3',
@@ -114,18 +121,22 @@
             case 'execute':
                 for i in args.argument:
                     fnattr.vljum.m.M.execute(i)
             case 'file':
                 for i in args.argument:
                     with fnattr.util.io.open_input(i) as f:
                         fnattr.vljum.m.M.execute(f.read())
-            case _:
+            case _:  # pragma: no cover
                 logging.error('Unknown mode: %s', args.mode)
+    except fnattr.util.error.Error as e:
+        logging.error(e)
+        return 1
     except Exception as e:
         logging.error('Unhandled exception: %s%s', type(e).__name__, e.args)
-        if logging.getLogger().getEffectiveLevel() < logging.INFO:
+        if log_level < logging.INFO:
             raise
+        return 2
 
     return 0
 
-if __name__ == '__main__':
-    sys.exit(main())
+if __name__ == '__main__':  # pramga: no branch
+    sys.exit(main())        # pragma: no cover
```

### Comparing `fnattr-0.2.8/src/fnattr/util/checksum.py` & `fnattr-0.2.9/src/fnattr/util/checksum.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/util/docsplit.py` & `fnattr-0.2.9/src/fnattr/util/docsplit.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/util/duration.py` & `fnattr-0.2.9/src/fnattr/util/duration.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/util/escape.py` & `fnattr-0.2.9/src/fnattr/util/escape.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/util/fearmat.py` & `fnattr-0.2.9/src/fnattr/util/fearmat.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/util/io.py` & `fnattr-0.2.9/src/fnattr/util/io.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/util/log.py` & `fnattr-0.2.9/src/fnattr/util/log.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 # SPDX-License-Identifier: MIT
 """Logging utilities."""
 
 import logging
 
 CHOICES = [c.lower() for c in logging.getLevelNamesMapping() if c != 'NOTSET']
 
-def level(cmd: str,
-          s: str | int,
-          *,
-          dryrun: bool = False,
-          dryrun_level: int = logging.INFO) -> int:
+def level_name(level: int) -> str:
+    return logging.getLevelName(level).lower()
+
+def config_level(cmd: str,
+                 s: str | int,
+                 *,
+                 dryrun: bool = False,
+                 dryrun_level: int = logging.INFO) -> int:
     log_level = getattr(logging, s.upper()) if isinstance(s, str) else s
     if dryrun and log_level > dryrun_level:
         log_level = dryrun_level
     logging.basicConfig(
         level=log_level, format=f'{cmd}: %(levelname)s: %(message)s')
     return log_level
+
+def config(cmd: str, args: object) -> int:
+    return config_level(
+        cmd,
+        getattr(args, 'log_level', logging.WARNING),
+        dryrun=getattr(args, 'dryrun', False))
```

### Comparing `fnattr-0.2.8/src/fnattr/util/multimap.py` & `fnattr-0.2.9/src/fnattr/util/multimap.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/util/nested.py` & `fnattr-0.2.9/src/fnattr/util/nested.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/util/registry.py` & `fnattr-0.2.9/src/fnattr/util/registry.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/util/repr.py` & `fnattr-0.2.9/src/fnattr/util/repr.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/util/sqlite.py` & `fnattr-0.2.9/src/fnattr/util/sqlite.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vlju/__init__.py` & `fnattr-0.2.9/src/fnattr/vlju/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vlju/types/all.py` & `fnattr-0.2.9/src/fnattr/vlju/types/all.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 from fnattr.vlju.types.info import Info
 from fnattr.vlju.types.lccn import LCCN
 from fnattr.vlju.types.timestamp import Timestamp
 from fnattr.vlju.types.uri import URI
 from fnattr.vlju.types.url import URL
 from fnattr.vlju.types.urn import URN
 
-# yapf: disable
+# fmt: off
 VLJU_TYPES: dict[str, type[Vlju]] = {
     'doi':      DOI,
     'ean':      EAN13,
     'file':     File,
     'info':     Info,
     'isbn':     ISBN,
     'ismn':     ISMN,
     'issn':     ISSN,
     'lccn':     LCCN,
     't':        Timestamp,
     'uri':      URI,
     'url':      URL,
     'urn':      URN,
 }
-# yapf: enable
+# fmt: on
```

### Comparing `fnattr-0.2.8/src/fnattr/vlju/types/doi/__init__.py` & `fnattr-0.2.9/src/fnattr/vlju/types/doi/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vlju/types/doi/org.py` & `fnattr-0.2.9/src/fnattr/vlju/types/doi/org.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vlju/types/ean/__init__.py` & `fnattr-0.2.9/src/fnattr/vlju/types/ean/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vlju/types/ean/isbn.py` & `fnattr-0.2.9/src/fnattr/vlju/types/ean/isbn.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vlju/types/ean/isbn_ranges.py` & `fnattr-0.2.9/src/fnattr/vlju/types/ean/isbn_ranges.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vlju/types/ean/ismn.py` & `fnattr-0.2.9/src/fnattr/vlju/types/ean/ismn.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vlju/types/ean/issn.py` & `fnattr-0.2.9/src/fnattr/vlju/types/ean/issn.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vlju/types/file/__init__.py` & `fnattr-0.2.9/src/fnattr/vlju/types/file/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vlju/types/info/__init__.py` & `fnattr-0.2.9/src/fnattr/vlju/types/info/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vlju/types/info/kinds.py` & `fnattr-0.2.9/src/fnattr/vlju/types/info/kinds.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """Kinds of info: URI."""
 
 # https://tools.ietf.org/html/rfc4452
 
 import fnattr.vlju.types.doi
 import fnattr.vlju.types.lccn
 
-# yapf: disable
+# fmt: off
 KIND = {
     'ark':                  None,
     'arxiv':                None,
     'bibcode':              None,
     'bnf':                  None,
     'ddbj-embl-genbank':    None,
     'dlf':                  None,
@@ -34,17 +34,17 @@
     'rfa':                  None,
     'rlgid':                None,
     'sici':                 None,
     'sid':                  None,
     'srw':                  None,
     'ugent-repo':           None,
 }
-# yapf: enable
+# fmt: on
 
-# yapf: disable
+# fmt: off
 ORGANIZATION = {
     'ark':          'Archival Resource Keys',
     'arxiv':        'arXiv.org identifiers',
     'bibcode':      'Astrophysics Data System bibcodes',
     'bnf':          'Bibliothèque nationale de France',
     'ddbj-embl-genbank':    'DDBJ/EMBL/GenBank',
     'dlf':          'Digital Library Federation',
@@ -68,8 +68,8 @@
     'rfa':          'Registry Framework Architecture',
     'rlgid':        'RLG Database Record',
     'sici':         'Serial Item and Contribution',
     'sid':          'Source Identifiers in the NISO OpenURL Framework',
     'srw':          'Search/Retrieve Web Services',
     'ugent-repo':   'University Library Ghent',
 }
-# yapf: enable
+# fmt: on
```

### Comparing `fnattr-0.2.8/src/fnattr/vlju/types/lccn/__init__.py` & `fnattr-0.2.9/src/fnattr/vlju/types/lccn/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vlju/types/site/__init__.py` & `fnattr-0.2.9/src/fnattr/vlju/types/site/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vlju/types/timestamp/__init__.py` & `fnattr-0.2.9/src/fnattr/vlju/types/timestamp/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vlju/types/uri/__init__.py` & `fnattr-0.2.9/src/fnattr/vlju/types/uri/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vlju/types/url/__init__.py` & `fnattr-0.2.9/src/fnattr/vlju/types/url/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vlju/types/urn/__init__.py` & `fnattr-0.2.9/src/fnattr/vlju/types/urn/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vlju/types/urn/kinds.py` & `fnattr-0.2.9/src/fnattr/vlju/types/urn/kinds.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vljum/__init__.py` & `fnattr-0.2.9/src/fnattr/vljum/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vljum/m.py` & `fnattr-0.2.9/src/fnattr/vljum/m.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vljum/runner.py` & `fnattr-0.2.9/src/fnattr/vljum/runner.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vljumap/__init__.py` & `fnattr-0.2.9/src/fnattr/vljumap/__init__.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vljumap/enc.py` & `fnattr-0.2.9/src/fnattr/vljumap/enc.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr/vljumap/factory.py` & `fnattr-0.2.9/src/fnattr/vljumap/factory.py`

 * *Files identical despite different names*

### Comparing `fnattr-0.2.8/src/fnattr.egg-info/PKG-INFO` & `fnattr-0.2.9/src/fnattr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnattr
-Version: 0.2.8
+Version: 0.2.9
 Summary: Manage key/value metadata in file names.
 License: MIT License
 Project-URL: repository, https://codeberg.org/datatravelandexperiments/fna
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fnattr-0.2.8/src/fnattr.egg-info/SOURCES.txt` & `fnattr-0.2.9/src/fnattr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

