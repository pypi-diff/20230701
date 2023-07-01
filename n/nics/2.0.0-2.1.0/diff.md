# Comparing `tmp/nics-2.0.0.tar.gz` & `tmp/nics-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-zi7w0cc3/nics-2.0.0.tar", last modified: Fri Jun 30 15:28:43 2023, max compression
+gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-2aa6xe26/nics-2.1.0.tar", last modified: Sat Jul  1 05:19:43 2023, max compression
```

## Comparing `nics-2.0.0.tar` & `nics-2.1.0.tar`

### file list

```diff
@@ -1,66 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:43.000000 nics-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-30 15:28:19.000000 nics-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-30 15:28:19.000000 nics-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-30 15:28:43.000000 nics-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-30 15:28:19.000000 nics-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:42.000000 nics-2.0.0/nics/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-30 15:28:19.000000 nics-2.0.0/nics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:42.000000 nics-2.0.0/nics/main/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:42.000000 nics-2.0.0/nics/main/_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:42.000000 nics-2.0.0/nics/main/_template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/404.md
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:42.000000 nics-2.0.0/nics/main/_template/docs/tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/1 -- THIS-IS-TITLE -- THIS-IS-URL.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:42.000000 nics-2.0.0/nics/main/_template/docs/tree/2 -- Bar -- bar/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/2 -- Bar -- bar/Hello -- world.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/2 -- Bar -- bar/Without Numbering -- Without-Numbering.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/2 -- Bar -- bar/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:42.000000 nics-2.0.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:43.000000 nics-2.0.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/Without index.md -- without-index-md.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/02 -- bar -- bar.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/index.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/4 -- About -- about.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/5 -- This is a demo -- This-Is-A-Demo.md
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/docs/tree/nics-logo500.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:42.000000 nics-2.0.0/nics/main/_template/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:43.000000 nics-2.0.0/nics/main/_template/web/_layouts/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/web/_layouts/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:43.000000 nics-2.0.0/nics/main/_template/web/_sass/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/web/_sass/footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/web/_sass/header.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/web/_sass/main.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:43.000000 nics-2.0.0/nics/main/_template/web/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/_template/web/scripts/header.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:43.000000 nics-2.0.0/nics/main/compile/
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/compile/copying_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/compile/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/compile/update_404_and_favicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/compile/update_docs_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/compile/update_footer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/compile/update_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/compile/update_jekyll_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/compile/update_sass_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:43.000000 nics-2.0.0/nics/main/upgrade/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/upgrade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:43.000000 nics-2.0.0/nics/main/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/wizard/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/wizard/settings_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-30 15:28:19.000000 nics-2.0.0/nics/main/wizard/workflow_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:28:42.000000 nics-2.0.0/nics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-30 15:28:42.000000 nics-2.0.0/nics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-30 15:28:42.000000 nics-2.0.0/nics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:28:42.000000 nics-2.0.0/nics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-30 15:28:42.000000 nics-2.0.0/nics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-30 15:28:42.000000 nics-2.0.0/nics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 15:28:42.000000 nics-2.0.0/nics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-30 15:28:19.000000 nics-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-30 15:28:43.000000 nics-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-30 15:28:19.000000 nics-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:43.000000 nics-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-01 05:19:22.000000 nics-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-01 05:19:22.000000 nics-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-01 05:19:43.000000 nics-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-01 05:19:22.000000 nics-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:43.000000 nics-2.1.0/nics/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-01 05:19:22.000000 nics-2.1.0/nics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:43.000000 nics-2.1.0/nics/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:43.000000 nics-2.1.0/nics/main/_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:43.000000 nics-2.1.0/nics/main/_template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/_template/docs/404.md
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/_template/docs/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:43.000000 nics-2.1.0/nics/main/_template/docs/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/_template/docs/tree/1 -- THIS-IS-TITLE -- THIS-IS-URL.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:43.000000 nics-2.1.0/nics/main/_template/docs/tree/2 -- Bar -- bar/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/_template/docs/tree/2 -- Bar -- bar/Hello -- world.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/_template/docs/tree/2 -- Bar -- bar/Without Numbering -- Without-Numbering.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/_template/docs/tree/2 -- Bar -- bar/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:43.000000 nics-2.1.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:43.000000 nics-2.1.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/Without index.md -- without-index-md.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/02 -- bar -- bar.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/_template/docs/tree/4 -- About -- about.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/_template/docs/tree/5 -- This is a demo -- This-Is-A-Demo.md
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/_template/docs/tree/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/_template/docs/tree/nics-logo500.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:43.000000 nics-2.1.0/nics/main/_template/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:43.000000 nics-2.1.0/nics/main/_template/web/_layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/_template/web/_layouts/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:43.000000 nics-2.1.0/nics/main/_template/web/_sass/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/_template/web/_sass/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/_template/web/_sass/header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/_template/web/_sass/main.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:43.000000 nics-2.1.0/nics/main/_template/web/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/_template/web/scripts/header.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:43.000000 nics-2.1.0/nics/main/compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/compile/copying_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/compile/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/compile/update_404_and_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/compile/update_docs_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/compile/update_footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/compile/update_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/compile/update_jekyll_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/compile/update_sass_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:43.000000 nics-2.1.0/nics/main/upgrade/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/upgrade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:43.000000 nics-2.1.0/nics/main/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/wizard/settings_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-01 05:19:22.000000 nics-2.1.0/nics/main/wizard/workflow_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:19:43.000000 nics-2.1.0/nics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-01 05:19:43.000000 nics-2.1.0/nics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-01 05:19:43.000000 nics-2.1.0/nics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 05:19:43.000000 nics-2.1.0/nics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-01 05:19:43.000000 nics-2.1.0/nics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-01 05:19:43.000000 nics-2.1.0/nics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 05:19:43.000000 nics-2.1.0/nics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-01 05:19:22.000000 nics-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 05:19:43.000000 nics-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-01 05:19:22.000000 nics-2.1.0/setup.py
```

### Comparing `nics-2.0.0/LICENSE` & `nics-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nics-2.0.0/PKG-INFO` & `nics-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 2.0.0
+Version: 2.1.0
 Summary: Automated docs repo generator
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-2.0.0/README.md` & `nics-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nics-2.0.0/nics/main/__init__.py` & `nics-2.1.0/nics/main/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.0.0/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg` & `nics-2.1.0/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg`

 * *Files identical despite different names*

### Comparing `nics-2.0.0/nics/main/_template/docs/tree/nics-logo500.jpg` & `nics-2.1.0/nics/main/_template/docs/tree/nics-logo500.jpg`

 * *Files identical despite different names*

### Comparing `nics-2.0.0/nics/main/_template/web/_sass/header.scss` & `nics-2.1.0/nics/main/_template/web/_sass/header.scss`

 * *Files identical despite different names*

### Comparing `nics-2.0.0/nics/main/_template/web/_sass/main.scss` & `nics-2.1.0/nics/main/_template/web/_sass/main.scss`

 * *Files identical despite different names*

### Comparing `nics-2.0.0/nics/main/_template/web/scripts/header.js` & `nics-2.1.0/nics/main/_template/web/scripts/header.js`

 * *Files identical despite different names*

### Comparing `nics-2.0.0/nics/main/compile/__init__.py` & `nics-2.1.0/nics/main/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.0.0/nics/main/compile/copying_template.py` & `nics-2.1.0/nics/main/compile/copying_template.py`

 * *Files identical despite different names*

### Comparing `nics-2.0.0/nics/main/compile/update_404_and_favicon.py` & `nics-2.1.0/nics/main/compile/update_404_and_favicon.py`

 * *Files identical despite different names*

### Comparing `nics-2.0.0/nics/main/compile/update_docs_tree.py` & `nics-2.1.0/nics/main/compile/update_docs_tree.py`

 * *Files identical despite different names*

### Comparing `nics-2.0.0/nics/main/compile/update_header.py` & `nics-2.1.0/nics/main/compile/update_header.py`

 * *Files identical despite different names*

### Comparing `nics-2.0.0/nics/main/compile/update_jekyll_config.py` & `nics-2.1.0/nics/main/compile/update_jekyll_config.py`

 * *Files identical despite different names*

### Comparing `nics-2.0.0/nics/main/constants.py` & `nics-2.1.0/nics/main/constants.py`

 * *Files identical despite different names*

### Comparing `nics-2.0.0/nics/main/upgrade/__init__.py` & `nics-2.1.0/nics/main/upgrade/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.0.0/nics/main/wizard/__init__.py` & `nics-2.1.0/nics/main/wizard/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,53 @@
 import os
 import shutil
+import sys
 
 from mykit.kit.utils import printer, print_screen
 
 from ..constants import TMPL_DOCS_DIR_PTH
-from .inspect import inspect
 from .workflow_writer import workflow_writer
 from .settings_writer import settings_writer
 
 
 def run():
 
     CWD = os.getcwd()
 
     WORKFLOW_FILE_PTH = os.path.join(CWD, '.github', 'workflows', 'rebuild-docs.yml')
     CONTAINER_DIR_PTH = os.path.join(CWD, 'docs')
     SETTINGS_FILE_PTH = os.path.join(CWD, 'docs', 'settings.txt')
 
-    ## inspection
-    inspect(CONTAINER_DIR_PTH, WORKFLOW_FILE_PTH)
+    ## already_use is True if the user has used NICS before and only wants to reinitialize; otherwise, False.
+    already_use = False
+    if os.path.isfile(WORKFLOW_FILE_PTH) and os.path.isdir(CONTAINER_DIR_PTH):
+        already_use = True
+
+    if not already_use:
+        if os.path.isfile(WORKFLOW_FILE_PTH) or os.path.isdir(CONTAINER_DIR_PTH):
+            printer(f'ERROR: Workflow file or docs/ folder already exist.')
+            sys.exit(1)
 
     ## intro
     print_screen(
         'Welcome to NICS!\n'
         '================\n\n'
     )
 
+    if already_use:
+        print(
+            'Workflow file and docs/ folder are found, will rewrite these following files:\n'
+            f'- Workflow file {repr(WORKFLOW_FILE_PTH)}\n'
+            f'- Settings file {repr(SETTINGS_FILE_PTH)}'
+        )
+        usr = input('Continue?  (Y/n): ')
+        if usr not in ['', 'y', 'Y']:
+            printer(f'INFO: Exited.')
+            sys.exit(0)
+
     ## saving user's information
     author = input('Enter your name: ')
     email = input('Enter your email: ')
     gh_username = input('Enter your GitHub username: ')
     gh_repo = input('Enter this GitHub repository name: ')
     main_branch_name = input("Enter the main branch name (e.g., master): ")
 
@@ -43,17 +61,18 @@
         if not os.path.isdir(pth):
             os.mkdir(pth)
             printer(f"INFO: Folder {repr(pth)} is created.")
     handle_workflow_dirs()
 
     workflow_writer(WORKFLOW_FILE_PTH, author, email, gh_repo, main_branch_name)
 
-    printer(f"INFO: Copying 'docs/' folder.")
-    shutil.copytree(TMPL_DOCS_DIR_PTH, CONTAINER_DIR_PTH)
-    printer(f'INFO: Done, {repr(CONTAINER_DIR_PTH)} is created.')
+    if not already_use:
+        printer(f"INFO: Copying 'docs/' folder.")
+        shutil.copytree(TMPL_DOCS_DIR_PTH, CONTAINER_DIR_PTH)
+        printer(f'INFO: Done, {repr(CONTAINER_DIR_PTH)} is created.')
 
     settings_writer(SETTINGS_FILE_PTH, author, email, gh_username, gh_repo, main_branch_name)
 
     ## outro
     print_screen(f"""
 Almost done, now you need to do these final steps:
 1. Create docs branch
```

### Comparing `nics-2.0.0/nics/main/wizard/settings_writer.py` & `nics-2.1.0/nics/main/wizard/settings_writer.py`

 * *Files identical despite different names*

### Comparing `nics-2.0.0/nics/main/wizard/workflow_writer.py` & `nics-2.1.0/nics/main/wizard/workflow_writer.py`

 * *Files identical despite different names*

### Comparing `nics-2.0.0/nics.egg-info/PKG-INFO` & `nics-2.1.0/nics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 2.0.0
+Version: 2.1.0
 Summary: Automated docs repo generator
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-2.0.0/nics.egg-info/SOURCES.txt` & `nics-2.1.0/nics.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -39,10 +39,9 @@
 nics/main/compile/update_docs_tree.py
 nics/main/compile/update_footer.py
 nics/main/compile/update_header.py
 nics/main/compile/update_jekyll_config.py
 nics/main/compile/update_sass_constants.py
 nics/main/upgrade/__init__.py
 nics/main/wizard/__init__.py
-nics/main/wizard/inspect.py
 nics/main/wizard/settings_writer.py
 nics/main/wizard/workflow_writer.py
```

### Comparing `nics-2.0.0/pyproject.toml` & `nics-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "nics"
-version = "2.0.0"
+version = "2.1.0"
 description = "Automated docs repo generator"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

