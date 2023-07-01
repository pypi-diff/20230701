# Comparing `tmp/nics-2.4.1.tar.gz` & `tmp/nics-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-rkebf4qw/nics-2.4.1.tar", last modified: Sat Jul  1 17:02:01 2023, max compression
+gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-fl49sicm/nics-2.5.0.tar", last modified: Sat Jul  1 18:11:09 2023, max compression
```

## Comparing `nics-2.4.1.tar` & `nics-2.5.0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:02:01.000000 nics-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-01 17:01:42.000000 nics-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-01 17:01:42.000000 nics-2.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-01 17:02:01.000000 nics-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-01 17:01:42.000000 nics-2.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:02:01.000000 nics-2.4.1/nics/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-01 17:01:42.000000 nics-2.4.1/nics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:02:01.000000 nics-2.4.1/nics/main/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:02:01.000000 nics-2.4.1/nics/main/_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:02:01.000000 nics-2.4.1/nics/main/_template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/_template/docs/404.md
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/_template/docs/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:02:01.000000 nics-2.4.1/nics/main/_template/docs/tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/_template/docs/tree/1 -- THIS-IS-TITLE -- THIS-IS-URL.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:02:01.000000 nics-2.4.1/nics/main/_template/docs/tree/2 -- Bar -- bar/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/_template/docs/tree/2 -- Bar -- bar/Hello -- world.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/_template/docs/tree/2 -- Bar -- bar/Without Numbering -- Without-Numbering.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/_template/docs/tree/2 -- Bar -- bar/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:02:01.000000 nics-2.4.1/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:02:01.000000 nics-2.4.1/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/Without index.md -- without-index-md.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/02 -- bar -- bar.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/index.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/_template/docs/tree/4 -- About -- about.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/_template/docs/tree/5 -- This is a demo -- This-Is-A-Demo.md
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/_template/docs/tree/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/_template/docs/tree/nics-logo500.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:02:01.000000 nics-2.4.1/nics/main/_template/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:02:01.000000 nics-2.4.1/nics/main/_template/web/_layouts/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/_template/web/_layouts/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:02:01.000000 nics-2.4.1/nics/main/_template/web/_sass/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/_template/web/_sass/footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/_template/web/_sass/header.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/_template/web/_sass/main.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:02:01.000000 nics-2.4.1/nics/main/_template/web/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/_template/web/scripts/header.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:02:01.000000 nics-2.4.1/nics/main/compile/
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/compile/copying_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/compile/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/compile/update_404_and_favicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/compile/update_docs_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/compile/update_footer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/compile/update_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/compile/update_jekyll_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/compile/update_sass_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:02:01.000000 nics-2.4.1/nics/main/upgrade/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/upgrade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:02:01.000000 nics-2.4.1/nics/main/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/wizard/settings_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-01 17:01:42.000000 nics-2.4.1/nics/main/wizard/workflow_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:02:01.000000 nics-2.4.1/nics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-01 17:02:01.000000 nics-2.4.1/nics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-01 17:02:01.000000 nics-2.4.1/nics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 17:02:01.000000 nics-2.4.1/nics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-01 17:02:01.000000 nics-2.4.1/nics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-01 17:02:01.000000 nics-2.4.1/nics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 17:02:01.000000 nics-2.4.1/nics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-01 17:01:42.000000 nics-2.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 17:02:01.000000 nics-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-01 17:01:42.000000 nics-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:11:09.000000 nics-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-01 18:10:53.000000 nics-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-01 18:10:53.000000 nics-2.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-01 18:11:09.000000 nics-2.5.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:11:09.000000 nics-2.5.0/nics/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-01 18:10:53.000000 nics-2.5.0/nics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:11:09.000000 nics-2.5.0/nics/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:11:09.000000 nics-2.5.0/nics/main/_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:11:09.000000 nics-2.5.0/nics/main/_template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/_template/docs/404.md
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/_template/docs/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:11:09.000000 nics-2.5.0/nics/main/_template/docs/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/_template/docs/tree/1 -- THIS-IS-TITLE -- THIS-IS-URL.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:11:09.000000 nics-2.5.0/nics/main/_template/docs/tree/2 -- Bar -- bar/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/_template/docs/tree/2 -- Bar -- bar/Hello -- world.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/_template/docs/tree/2 -- Bar -- bar/Without Numbering -- Without-Numbering.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/_template/docs/tree/2 -- Bar -- bar/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:11:09.000000 nics-2.5.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:11:09.000000 nics-2.5.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/Without index.md -- without-index-md.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/02 -- bar -- bar.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/_template/docs/tree/4 -- About -- about.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/_template/docs/tree/5 -- This is a demo -- This-Is-A-Demo.md
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/_template/docs/tree/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/_template/docs/tree/nics-logo500.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:11:09.000000 nics-2.5.0/nics/main/_template/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:11:09.000000 nics-2.5.0/nics/main/_template/web/_layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/_template/web/_layouts/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:11:09.000000 nics-2.5.0/nics/main/_template/web/_sass/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/_template/web/_sass/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/_template/web/_sass/header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/_template/web/_sass/main.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:11:09.000000 nics-2.5.0/nics/main/_template/web/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/_template/web/scripts/header.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:11:09.000000 nics-2.5.0/nics/main/compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/compile/copying_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/compile/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/compile/update_404_and_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/compile/update_docs_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/compile/update_footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/compile/update_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/compile/update_jekyll_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/compile/update_sass_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:11:09.000000 nics-2.5.0/nics/main/upgrade/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/upgrade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:11:09.000000 nics-2.5.0/nics/main/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/wizard/settings_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-01 18:10:53.000000 nics-2.5.0/nics/main/wizard/workflow_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:11:09.000000 nics-2.5.0/nics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-01 18:11:09.000000 nics-2.5.0/nics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-01 18:11:09.000000 nics-2.5.0/nics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 18:11:09.000000 nics-2.5.0/nics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-01 18:11:09.000000 nics-2.5.0/nics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-01 18:11:09.000000 nics-2.5.0/nics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 18:11:09.000000 nics-2.5.0/nics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-01 18:10:53.000000 nics-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 18:11:09.000000 nics-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-01 18:10:53.000000 nics-2.5.0/setup.py
```

### Comparing `nics-2.4.1/LICENSE` & `nics-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nics-2.4.1/nics/main/__init__.py` & `nics-2.5.0/nics/main/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.4.1/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg` & `nics-2.5.0/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg`

 * *Files identical despite different names*

### Comparing `nics-2.4.1/nics/main/_template/docs/tree/nics-logo500.jpg` & `nics-2.5.0/nics/main/_template/docs/tree/nics-logo500.jpg`

 * *Files identical despite different names*

### Comparing `nics-2.4.1/nics/main/_template/web/_sass/header.scss` & `nics-2.5.0/nics/main/_template/web/_sass/header.scss`

 * *Files identical despite different names*

### Comparing `nics-2.4.1/nics/main/_template/web/_sass/main.scss` & `nics-2.5.0/nics/main/_template/web/_sass/main.scss`

 * *Files identical despite different names*

### Comparing `nics-2.4.1/nics/main/_template/web/scripts/header.js` & `nics-2.5.0/nics/main/_template/web/scripts/header.js`

 * *Files identical despite different names*

### Comparing `nics-2.4.1/nics/main/compile/__init__.py` & `nics-2.5.0/nics/main/compile/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,8 +60,8 @@
 
     update_jekyll_config(D_JEKYLL_CONFIG, cfg.author, cfg._gh_username, cfg._gh_repo)
     update_404_and_favicon(C_404, C_ICON, D_404, D_ICON)
 
     copying_template(dock)
     update_sass_constants(D_SASS_CONSTANTS, cfg.color_hue)
 
-    update_docs_tree(C_TREE, D__PAGES, cfg.lowercase_the_url)
+    update_docs_tree(C_TREE, D__PAGES, cfg.lowercase_the_url, cfg._gh_username, cfg._gh_repo)
```

### Comparing `nics-2.4.1/nics/main/compile/copying_template.py` & `nics-2.5.0/nics/main/compile/copying_template.py`

 * *Files identical despite different names*

### Comparing `nics-2.4.1/nics/main/compile/update_404_and_favicon.py` & `nics-2.5.0/nics/main/compile/update_404_and_favicon.py`

 * *Files identical despite different names*

### Comparing `nics-2.4.1/nics/main/compile/update_docs_tree.py` & `nics-2.5.0/nics/main/compile/update_docs_tree.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 import re
+import requests
 import shutil
 
 from mykit.kit.utils import printer
 
 
-def update_recursively(D__PAGES, lowercase_the_url, pth, base):
+def update_recursively(D__PAGES, lowercase_the_url, gh_username, gh_repo, pth, base):
     printer(f'DEBUG: Updating docs-tree, pth: {repr(pth)}, base: {repr(base)}')
 
     for i in os.listdir(pth):
         pth2 = os.path.join(pth, i)
 
         ## handle non-markdown files
         if os.path.isfile(pth2) and (not i.endswith('.md')):
@@ -25,25 +26,38 @@
                 text = (
                     '---\n'
                     'permalink: /\n'
                     'layout: main\n'
                     'title: Home\n'
                     '---\n\n'
                 )
+                with open(pth2, 'r') as f:
+                    homepage = f.read()
+                    if homepage.strip() == 'use-repo-readme':
+                        printer('INFO: Using GitHub repo readme.')
+                        repo_readme = requests.get(f'https://raw.githubusercontent.com/{gh_username}/{gh_repo}/main/README.md')
+                        if repo_readme == '404: Not Found':
+                            repo_readme = requests.get(f'https://raw.githubusercontent.com/{gh_username}/{gh_repo}/main/readme.md')
+                        if repo_readme == '404: Not Found':
+                            raise FileNotFoundError('Readme file not found in GitHub repository.')
+                        text += repo_readme
+                    else:
+                        text += homepage
+                with open(dst, 'w') as f: f.write(text)
             else:
                 dst = os.path.join(D__PAGES, os.sep.join(filter(lambda s:s!='', base.split('/'))), 'index.md')
                 text = (
                     '---\n'
                     f'permalink: {base}\n'
                     'layout: main\n'
                     f"title: {list(filter(lambda s:s!='', base.split('/')))[-1]}\n"
                     '---\n\n'
                 )
-            with open(pth2, 'r') as f: text += f.read()
-            with open(dst, 'w') as f: f.write(text)
+                with open(pth2, 'r') as f: text += f.read()
+                with open(dst, 'w') as f: f.write(text)
             printer(f'DEBUG: Updated index.md from {repr(pth2)} to {repr(dst)}.')
             continue
         ## </handling the index.md>
 
         res = re.match(r"^(?:\d+ - )?(?P<name>[\w \-'&\(\).]+?)(?:\.md)?$", i)
         if res is None: raise AssertionError(f'Invalid docs-tree format: {repr(i)}')
         name = res.group('name')
@@ -54,33 +68,33 @@
         if os.path.isdir(pth2):
             ## if the folder doesn't exist, create a new one.
             dir = os.path.join(D__PAGES, os.sep.join(filter(lambda s:s!='', base.split('/'))), url)
             if not os.path.isdir(dir):
                 os.mkdir(dir)
                 printer(f'DEBUG: Dir created: {repr(dir)}.')
             ## do it again
-            update_recursively(D__PAGES, lowercase_the_url, pth2, base+url+'/')
+            update_recursively(D__PAGES, lowercase_the_url, gh_username, gh_repo, pth2, base+url+'/')
         else:
             dst = os.path.join(D__PAGES, os.sep.join(filter(lambda s:s!='', base.split('/'))), f'{name}.md')
             text = (
                 '---\n'
                 f'permalink: {base}{url}/\n'
                 'layout: main\n'
                 f'title: {name}\n'
                 '---\n\n'
             )
             with open(pth2, 'r') as f: text += f.read()
             with open(dst, 'w') as f: f.write(text)
             printer(f'DEBUG: Updated docs-tree file from {repr(pth2)} to {repr(dst)}.')
 
 
-def update_docs_tree(C_TREE, D__PAGES, lowercase_the_url):
+def update_docs_tree(C_TREE, D__PAGES, lowercase_the_url, gh_username, gh_repo):
 
     ## delete the old '_pages' folder in docs branch
     if os.path.isdir(D__PAGES):  # reminder: initially, '_pages' doesn't exist
         printer(f'DEBUG: Deleting {repr(D__PAGES)} recursively.')
         shutil.rmtree(D__PAGES)
 
     printer(f'DEBUG: Creating dir {repr(D__PAGES)}.')
     os.mkdir(D__PAGES)
 
-    update_recursively(D__PAGES, lowercase_the_url, C_TREE, '/')
+    update_recursively(D__PAGES, lowercase_the_url, gh_username, gh_repo, C_TREE, '/')
```

### Comparing `nics-2.4.1/nics/main/compile/update_header.py` & `nics-2.5.0/nics/main/compile/update_header.py`

 * *Files identical despite different names*

### Comparing `nics-2.4.1/nics/main/compile/update_jekyll_config.py` & `nics-2.5.0/nics/main/compile/update_jekyll_config.py`

 * *Files identical despite different names*

### Comparing `nics-2.4.1/nics/main/constants.py` & `nics-2.5.0/nics/main/constants.py`

 * *Files identical despite different names*

### Comparing `nics-2.4.1/nics/main/upgrade/__init__.py` & `nics-2.5.0/nics/main/upgrade/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.4.1/nics/main/wizard/__init__.py` & `nics-2.5.0/nics/main/wizard/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.4.1/nics/main/wizard/settings_writer.py` & `nics-2.5.0/nics/main/wizard/settings_writer.py`

 * *Files identical despite different names*

### Comparing `nics-2.4.1/nics/main/wizard/workflow_writer.py` & `nics-2.5.0/nics/main/wizard/workflow_writer.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 on:
   push:
     branches:
       - {main_branch_name}
 
     paths:
       - 'docs/**'  # only rebuild if 'docs/' folder is modified
+      - README.md  # if using `use-repo-readme` keyword in 'tree/index.md'
 
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 permissions:
   contents: write
```

### Comparing `nics-2.4.1/nics.egg-info/SOURCES.txt` & `nics-2.5.0/nics.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 LICENSE
 MANIFEST.in
-README.md
 pyproject.toml
 setup.cfg
 setup.py
 nics/__main__.py
 nics.egg-info/PKG-INFO
 nics.egg-info/SOURCES.txt
 nics.egg-info/dependency_links.txt
```

### Comparing `nics-2.4.1/pyproject.toml` & `nics-2.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "nics"
-version = "2.4.1"
+version = "2.5.0"
 description = "Minimalist GitHub documentation tool"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

