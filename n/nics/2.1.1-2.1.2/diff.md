# Comparing `tmp/nics-2.1.1.tar.gz` & `tmp/nics-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-l4oib5vb/nics-2.1.1.tar", last modified: Sat Jul  1 05:34:58 2023, max compression
+gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-x2qu8e84/nics-2.1.2.tar", last modified: Sat Jul  1 07:53:46 2023, max compression
```

## Comparing `nics-2.1.1.tar` & `nics-2.1.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:58.000000 nics-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-01 05:34:38.000000 nics-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-01 05:34:38.000000 nics-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-01 05:34:58.000000 nics-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-01 05:34:38.000000 nics-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:58.000000 nics-2.1.1/nics/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-01 05:34:38.000000 nics-2.1.1/nics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:58.000000 nics-2.1.1/nics/main/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:58.000000 nics-2.1.1/nics/main/_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:58.000000 nics-2.1.1/nics/main/_template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/_template/docs/404.md
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/_template/docs/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:58.000000 nics-2.1.1/nics/main/_template/docs/tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/_template/docs/tree/1 -- THIS-IS-TITLE -- THIS-IS-URL.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:58.000000 nics-2.1.1/nics/main/_template/docs/tree/2 -- Bar -- bar/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/_template/docs/tree/2 -- Bar -- bar/Hello -- world.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/_template/docs/tree/2 -- Bar -- bar/Without Numbering -- Without-Numbering.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/_template/docs/tree/2 -- Bar -- bar/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:58.000000 nics-2.1.1/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:58.000000 nics-2.1.1/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/Without index.md -- without-index-md.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/02 -- bar -- bar.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/index.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/_template/docs/tree/4 -- About -- about.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/_template/docs/tree/5 -- This is a demo -- This-Is-A-Demo.md
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/_template/docs/tree/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/_template/docs/tree/nics-logo500.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:58.000000 nics-2.1.1/nics/main/_template/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:58.000000 nics-2.1.1/nics/main/_template/web/_layouts/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/_template/web/_layouts/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:58.000000 nics-2.1.1/nics/main/_template/web/_sass/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/_template/web/_sass/footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/_template/web/_sass/header.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/_template/web/_sass/main.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:58.000000 nics-2.1.1/nics/main/_template/web/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/_template/web/scripts/header.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:58.000000 nics-2.1.1/nics/main/compile/
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/compile/copying_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/compile/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/compile/update_404_and_favicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/compile/update_docs_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/compile/update_footer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/compile/update_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/compile/update_jekyll_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/compile/update_sass_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:58.000000 nics-2.1.1/nics/main/upgrade/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/upgrade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:58.000000 nics-2.1.1/nics/main/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/wizard/settings_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-01 05:34:38.000000 nics-2.1.1/nics/main/wizard/workflow_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:34:58.000000 nics-2.1.1/nics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-01 05:34:58.000000 nics-2.1.1/nics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-01 05:34:58.000000 nics-2.1.1/nics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 05:34:58.000000 nics-2.1.1/nics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-01 05:34:58.000000 nics-2.1.1/nics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-01 05:34:58.000000 nics-2.1.1/nics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 05:34:58.000000 nics-2.1.1/nics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-01 05:34:38.000000 nics-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 05:34:58.000000 nics-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-01 05:34:38.000000 nics-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:46.000000 nics-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-01 07:53:24.000000 nics-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-01 07:53:24.000000 nics-2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-01 07:53:46.000000 nics-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-01 07:53:24.000000 nics-2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:46.000000 nics-2.1.2/nics/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-01 07:53:24.000000 nics-2.1.2/nics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:46.000000 nics-2.1.2/nics/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:46.000000 nics-2.1.2/nics/main/_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:46.000000 nics-2.1.2/nics/main/_template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/_template/docs/404.md
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/_template/docs/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:46.000000 nics-2.1.2/nics/main/_template/docs/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/_template/docs/tree/1 -- THIS-IS-TITLE -- THIS-IS-URL.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:46.000000 nics-2.1.2/nics/main/_template/docs/tree/2 -- Bar -- bar/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/_template/docs/tree/2 -- Bar -- bar/Hello -- world.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/_template/docs/tree/2 -- Bar -- bar/Without Numbering -- Without-Numbering.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/_template/docs/tree/2 -- Bar -- bar/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:46.000000 nics-2.1.2/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:46.000000 nics-2.1.2/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/Without index.md -- without-index-md.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/02 -- bar -- bar.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/_template/docs/tree/4 -- About -- about.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/_template/docs/tree/5 -- This is a demo -- This-Is-A-Demo.md
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/_template/docs/tree/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/_template/docs/tree/nics-logo500.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:46.000000 nics-2.1.2/nics/main/_template/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:46.000000 nics-2.1.2/nics/main/_template/web/_layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/_template/web/_layouts/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:46.000000 nics-2.1.2/nics/main/_template/web/_sass/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/_template/web/_sass/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/_template/web/_sass/header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/_template/web/_sass/main.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:46.000000 nics-2.1.2/nics/main/_template/web/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/_template/web/scripts/header.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:46.000000 nics-2.1.2/nics/main/compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/compile/copying_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/compile/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/compile/update_404_and_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/compile/update_docs_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/compile/update_footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/compile/update_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/compile/update_jekyll_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/compile/update_sass_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:46.000000 nics-2.1.2/nics/main/upgrade/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/upgrade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:46.000000 nics-2.1.2/nics/main/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/wizard/settings_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-01 07:53:24.000000 nics-2.1.2/nics/main/wizard/workflow_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:53:46.000000 nics-2.1.2/nics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-01 07:53:46.000000 nics-2.1.2/nics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-01 07:53:46.000000 nics-2.1.2/nics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 07:53:46.000000 nics-2.1.2/nics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-01 07:53:46.000000 nics-2.1.2/nics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-01 07:53:46.000000 nics-2.1.2/nics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 07:53:46.000000 nics-2.1.2/nics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-01 07:53:24.000000 nics-2.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 07:53:46.000000 nics-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-01 07:53:24.000000 nics-2.1.2/setup.py
```

### Comparing `nics-2.1.1/LICENSE` & `nics-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nics-2.1.1/PKG-INFO` & `nics-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 2.1.1
+Version: 2.1.2
 Summary: Automated docs repo generator
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-2.1.1/README.md` & `nics-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nics-2.1.1/nics/main/__init__.py` & `nics-2.1.2/nics/main/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.1.1/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg` & `nics-2.1.2/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg`

 * *Files identical despite different names*

### Comparing `nics-2.1.1/nics/main/_template/docs/tree/nics-logo500.jpg` & `nics-2.1.2/nics/main/_template/docs/tree/nics-logo500.jpg`

 * *Files identical despite different names*

### Comparing `nics-2.1.1/nics/main/_template/web/_sass/header.scss` & `nics-2.1.2/nics/main/_template/web/_sass/header.scss`

 * *Files identical despite different names*

### Comparing `nics-2.1.1/nics/main/_template/web/_sass/main.scss` & `nics-2.1.2/nics/main/_template/web/_sass/main.scss`

 * *Files identical despite different names*

### Comparing `nics-2.1.1/nics/main/_template/web/scripts/header.js` & `nics-2.1.2/nics/main/_template/web/scripts/header.js`

 * *Files identical despite different names*

### Comparing `nics-2.1.1/nics/main/compile/__init__.py` & `nics-2.1.2/nics/main/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.1.1/nics/main/compile/copying_template.py` & `nics-2.1.2/nics/main/compile/copying_template.py`

 * *Files identical despite different names*

### Comparing `nics-2.1.1/nics/main/compile/update_404_and_favicon.py` & `nics-2.1.2/nics/main/compile/update_404_and_favicon.py`

 * *Files identical despite different names*

### Comparing `nics-2.1.1/nics/main/compile/update_docs_tree.py` & `nics-2.1.2/nics/main/compile/update_docs_tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                 )
             with open(pth2, 'r') as f: text += f.read()
             with open(dst, 'w') as f: f.write(text)
             printer(f'DEBUG: Updated index.md from {repr(pth2)} to {repr(dst)}.')
             continue
         ## </handling the index.md>
 
-        res = re.match(r"^(?:\d+ - )?(?P<name>[\w \-'&\(\).]+)(?:\.md)?$", i)
+        res = re.match(r"^(?:\d+ - )?(?P<name>[\w \-'&\(\).]+?)(?:\.md)?$", i)
         if res is None: raise AssertionError(f'Invalid docs-tree format: {repr(i)}')
         name = res.group('name')
         url = name.replace(' ', '-').replace("'", '').replace('&', 'and').replace('(', '').replace(')', '').replace('.', '-')
         if lowercase_the_url: url = url.lower()
         printer(f'DEBUG: name: {repr(name)}; url: {repr(url)}')
 
         if os.path.isdir(pth2):
```

### Comparing `nics-2.1.1/nics/main/compile/update_header.py` & `nics-2.1.2/nics/main/compile/update_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
         for fd in sorted(os.listdir(pth)):  # reminder: the file/dir `fd` order in `pth` matters.
             fd_pth = os.path.join(pth, fd)
 
             if fd == 'index.md': continue  # index.md will not be shown in navigation bar
             if os.path.isfile(fd_pth) and (not fd.endswith('.md')): continue  # ignore non-markdown files
 
-            res = re.match(r"^(?:\d+ - )?(?P<name>[\w \-'&\(\).]+)(?:\.md)?$", fd)
+            res = re.match(r"^(?:\d+ - )?(?P<name>[\w \-'&\(\).]+?)(?:\.md)?$", fd)
             if res is None: raise AssertionError(f'Invalid docs-tree format: {repr(fd)}')
             name = res.group('name')
             url = name.replace(' ', '-').replace("'", '').replace('&', 'and').replace('(', '').replace(')', '').replace('.', '-')
             if lowercase_the_url: url = url.lower()
             printer(f'DEBUG: name: {repr(name)}; url: {repr(url)}')
 
             if os.path.isdir(fd_pth):
```

### Comparing `nics-2.1.1/nics/main/compile/update_jekyll_config.py` & `nics-2.1.2/nics/main/compile/update_jekyll_config.py`

 * *Files identical despite different names*

### Comparing `nics-2.1.1/nics/main/constants.py` & `nics-2.1.2/nics/main/constants.py`

 * *Files identical despite different names*

### Comparing `nics-2.1.1/nics/main/upgrade/__init__.py` & `nics-2.1.2/nics/main/upgrade/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.1.1/nics/main/wizard/__init__.py` & `nics-2.1.2/nics/main/wizard/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.1.1/nics/main/wizard/settings_writer.py` & `nics-2.1.2/nics/main/wizard/settings_writer.py`

 * *Files identical despite different names*

### Comparing `nics-2.1.1/nics/main/wizard/workflow_writer.py` & `nics-2.1.2/nics/main/wizard/workflow_writer.py`

 * *Files identical despite different names*

### Comparing `nics-2.1.1/nics.egg-info/PKG-INFO` & `nics-2.1.2/nics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 2.1.1
+Version: 2.1.2
 Summary: Automated docs repo generator
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-2.1.1/nics.egg-info/SOURCES.txt` & `nics-2.1.2/nics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nics-2.1.1/pyproject.toml` & `nics-2.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "nics"
-version = "2.1.1"
+version = "2.1.2"
 description = "Automated docs repo generator"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

