# Comparing `tmp/nics-2.2.0.tar.gz` & `tmp/nics-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-6em6jjiq/nics-2.2.0.tar", last modified: Sat Jul  1 10:59:10 2023, max compression
+gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-tbz7445v/nics-2.2.2.tar", last modified: Sat Jul  1 11:49:47 2023, max compression
```

## Comparing `nics-2.2.0.tar` & `nics-2.2.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:59:10.000000 nics-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-01 10:58:54.000000 nics-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-01 10:58:54.000000 nics-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-01 10:59:10.000000 nics-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-01 10:58:54.000000 nics-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:59:10.000000 nics-2.2.0/nics/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-01 10:58:54.000000 nics-2.2.0/nics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:59:10.000000 nics-2.2.0/nics/main/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:59:10.000000 nics-2.2.0/nics/main/_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:59:10.000000 nics-2.2.0/nics/main/_template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/_template/docs/404.md
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/_template/docs/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:59:10.000000 nics-2.2.0/nics/main/_template/docs/tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/_template/docs/tree/1 -- THIS-IS-TITLE -- THIS-IS-URL.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:59:10.000000 nics-2.2.0/nics/main/_template/docs/tree/2 -- Bar -- bar/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/_template/docs/tree/2 -- Bar -- bar/Hello -- world.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/_template/docs/tree/2 -- Bar -- bar/Without Numbering -- Without-Numbering.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/_template/docs/tree/2 -- Bar -- bar/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:59:10.000000 nics-2.2.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:59:10.000000 nics-2.2.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/Without index.md -- without-index-md.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/02 -- bar -- bar.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/index.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/_template/docs/tree/4 -- About -- about.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/_template/docs/tree/5 -- This is a demo -- This-Is-A-Demo.md
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/_template/docs/tree/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/_template/docs/tree/nics-logo500.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:59:10.000000 nics-2.2.0/nics/main/_template/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:59:10.000000 nics-2.2.0/nics/main/_template/web/_layouts/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/_template/web/_layouts/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:59:10.000000 nics-2.2.0/nics/main/_template/web/_sass/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/_template/web/_sass/footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/_template/web/_sass/header.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/_template/web/_sass/main.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:59:10.000000 nics-2.2.0/nics/main/_template/web/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/_template/web/scripts/header.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:59:10.000000 nics-2.2.0/nics/main/compile/
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/compile/copying_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/compile/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/compile/update_404_and_favicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/compile/update_docs_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/compile/update_footer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/compile/update_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/compile/update_jekyll_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/compile/update_sass_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:59:10.000000 nics-2.2.0/nics/main/upgrade/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/upgrade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:59:10.000000 nics-2.2.0/nics/main/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/wizard/settings_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-01 10:58:54.000000 nics-2.2.0/nics/main/wizard/workflow_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:59:10.000000 nics-2.2.0/nics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-01 10:59:10.000000 nics-2.2.0/nics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-01 10:59:10.000000 nics-2.2.0/nics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 10:59:10.000000 nics-2.2.0/nics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-01 10:59:10.000000 nics-2.2.0/nics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-01 10:59:10.000000 nics-2.2.0/nics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 10:59:10.000000 nics-2.2.0/nics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-01 10:58:54.000000 nics-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 10:59:10.000000 nics-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-01 10:58:54.000000 nics-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:47.000000 nics-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-01 11:49:31.000000 nics-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-01 11:49:31.000000 nics-2.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-01 11:49:47.000000 nics-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-01 11:49:31.000000 nics-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:47.000000 nics-2.2.2/nics/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-01 11:49:31.000000 nics-2.2.2/nics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:47.000000 nics-2.2.2/nics/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:47.000000 nics-2.2.2/nics/main/_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:47.000000 nics-2.2.2/nics/main/_template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/_template/docs/404.md
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/_template/docs/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:47.000000 nics-2.2.2/nics/main/_template/docs/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/_template/docs/tree/1 -- THIS-IS-TITLE -- THIS-IS-URL.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:47.000000 nics-2.2.2/nics/main/_template/docs/tree/2 -- Bar -- bar/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/_template/docs/tree/2 -- Bar -- bar/Hello -- world.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/_template/docs/tree/2 -- Bar -- bar/Without Numbering -- Without-Numbering.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/_template/docs/tree/2 -- Bar -- bar/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:47.000000 nics-2.2.2/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:47.000000 nics-2.2.2/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/Without index.md -- without-index-md.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/02 -- bar -- bar.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/_template/docs/tree/4 -- About -- about.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/_template/docs/tree/5 -- This is a demo -- This-Is-A-Demo.md
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/_template/docs/tree/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/_template/docs/tree/nics-logo500.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:47.000000 nics-2.2.2/nics/main/_template/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:47.000000 nics-2.2.2/nics/main/_template/web/_layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/_template/web/_layouts/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:47.000000 nics-2.2.2/nics/main/_template/web/_sass/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/_template/web/_sass/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/_template/web/_sass/header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/_template/web/_sass/main.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:47.000000 nics-2.2.2/nics/main/_template/web/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/_template/web/scripts/header.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:47.000000 nics-2.2.2/nics/main/compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/compile/copying_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/compile/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/compile/update_404_and_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/compile/update_docs_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/compile/update_footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/compile/update_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/compile/update_jekyll_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/compile/update_sass_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:47.000000 nics-2.2.2/nics/main/upgrade/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/upgrade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:47.000000 nics-2.2.2/nics/main/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/wizard/settings_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-01 11:49:31.000000 nics-2.2.2/nics/main/wizard/workflow_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:49:47.000000 nics-2.2.2/nics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-01 11:49:47.000000 nics-2.2.2/nics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-01 11:49:47.000000 nics-2.2.2/nics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 11:49:47.000000 nics-2.2.2/nics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-01 11:49:47.000000 nics-2.2.2/nics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-01 11:49:47.000000 nics-2.2.2/nics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 11:49:47.000000 nics-2.2.2/nics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-01 11:49:31.000000 nics-2.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 11:49:47.000000 nics-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-01 11:49:31.000000 nics-2.2.2/setup.py
```

### Comparing `nics-2.2.0/LICENSE` & `nics-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nics-2.2.0/README.md` & `nics-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nics-2.2.0/nics/main/__init__.py` & `nics-2.2.2/nics/main/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.2.0/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg` & `nics-2.2.2/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg`

 * *Files identical despite different names*

### Comparing `nics-2.2.0/nics/main/_template/docs/tree/nics-logo500.jpg` & `nics-2.2.2/nics/main/_template/docs/tree/nics-logo500.jpg`

 * *Files identical despite different names*

### Comparing `nics-2.2.0/nics/main/_template/web/_sass/header.scss` & `nics-2.2.2/nics/main/_template/web/_sass/header.scss`

 * *Files identical despite different names*

### Comparing `nics-2.2.0/nics/main/_template/web/_sass/main.scss` & `nics-2.2.2/nics/main/_template/web/_sass/main.scss`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 ---
 # Jekyll requires this front matter, including the "#" sign, to convert main.scss to main.css.
 ---
 
 @import url('https://fonts.googleapis.com/css2?family=Caveat&display=swap');
 @import url('https://fonts.googleapis.com/css2?family=Caveat&family=Grandstander&display=swap');
+@import url('https://fonts.googleapis.com/css2?family=Ubuntu+Mono&display=swap');
 $font: 'Caveat', cursive;
 $font2: 'Grandstander', cursive;
+$font3: 'Ubuntu Mono', monospace;
 
 $font-size-mobile: 16px;
 $mobile-width: 850px;
 
 @import "constants";  // will be created during compilation
 @import "header";
 @import "footer";
@@ -45,14 +47,15 @@
 	width: 68%;
 	@media (max-width: $mobile-width) {
 		width: 91%;
 	}
 
 	margin: 0 auto;
 	margin-top: 58px;
+	margin-bottom: 72px;
 
 	font-family: $font2;
 	font-size: 17px;
 	@media (max-width: $mobile-width) {
 		font-size: $font-size-mobile;
 	}
 
@@ -73,8 +76,15 @@
 	ul {
 		line-height: 1.5;
 	}
 
 	img {
 		max-width: 100%;
 	}
+
+	code {
+		background-color: hsl($hue-signature, 7%, 73%);
+		padding: 2px 5px;
+		border-radius: 5px;
+		font-family: $font3;
+	}
 }
```

### Comparing `nics-2.2.0/nics/main/_template/web/scripts/header.js` & `nics-2.2.2/nics/main/_template/web/scripts/header.js`

 * *Files identical despite different names*

### Comparing `nics-2.2.0/nics/main/compile/__init__.py` & `nics-2.2.2/nics/main/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.2.0/nics/main/compile/copying_template.py` & `nics-2.2.2/nics/main/compile/copying_template.py`

 * *Files identical despite different names*

### Comparing `nics-2.2.0/nics/main/compile/update_404_and_favicon.py` & `nics-2.2.2/nics/main/compile/update_404_and_favicon.py`

 * *Files identical despite different names*

### Comparing `nics-2.2.0/nics/main/compile/update_docs_tree.py` & `nics-2.2.2/nics/main/compile/update_docs_tree.py`

 * *Files identical despite different names*

### Comparing `nics-2.2.0/nics/main/compile/update_header.py` & `nics-2.2.2/nics/main/compile/update_header.py`

 * *Files identical despite different names*

### Comparing `nics-2.2.0/nics/main/compile/update_jekyll_config.py` & `nics-2.2.2/nics/main/compile/update_jekyll_config.py`

 * *Files identical despite different names*

### Comparing `nics-2.2.0/nics/main/constants.py` & `nics-2.2.2/nics/main/constants.py`

 * *Files identical despite different names*

### Comparing `nics-2.2.0/nics/main/upgrade/__init__.py` & `nics-2.2.2/nics/main/upgrade/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.2.0/nics/main/wizard/__init__.py` & `nics-2.2.2/nics/main/wizard/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.2.0/nics/main/wizard/settings_writer.py` & `nics-2.2.2/nics/main/wizard/settings_writer.py`

 * *Files identical despite different names*

### Comparing `nics-2.2.0/nics/main/wizard/workflow_writer.py` & `nics-2.2.2/nics/main/wizard/workflow_writer.py`

 * *Files identical despite different names*

### Comparing `nics-2.2.0/nics.egg-info/SOURCES.txt` & `nics-2.2.2/nics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nics-2.2.0/pyproject.toml` & `nics-2.2.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "nics"
-version = "2.2.0"
-description = "Automated docs repo generator"
+version = "2.2.2"
+description = "Minimalist GitHub documentation tool."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
 keywords = ["python", "toolkit", "mykit"]
 classifiers = [
-	"Topic :: Scientific/Engineering",
     "License :: OSI Approved :: MIT License",
+    "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3 :: Only",
-    "Natural Language :: English"
+    "Topic :: Scientific/Engineering",
 ]
 dependencies = [
     "mykit==4.1.0",
 ]
 
 
 [tool.setuptools.packages.find]
```

