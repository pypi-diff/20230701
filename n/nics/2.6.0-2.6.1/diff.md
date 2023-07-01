# Comparing `tmp/nics-2.6.0.tar.gz` & `tmp/nics-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-s6y16jz8/nics-2.6.0.tar", last modified: Sat Jul  1 19:34:37 2023, max compression
+gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-u_y13uar/nics-2.6.1.tar", last modified: Sat Jul  1 19:47:39 2023, max compression
```

## Comparing `nics-2.6.0.tar` & `nics-2.6.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:37.000000 nics-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-01 19:34:22.000000 nics-2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-01 19:34:22.000000 nics-2.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-01 19:34:37.000000 nics-2.6.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:37.000000 nics-2.6.0/nics/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-01 19:34:22.000000 nics-2.6.0/nics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:37.000000 nics-2.6.0/nics/main/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:37.000000 nics-2.6.0/nics/main/_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:37.000000 nics-2.6.0/nics/main/_template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/_template/docs/404.md
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/_template/docs/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:37.000000 nics-2.6.0/nics/main/_template/docs/tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/_template/docs/tree/1 -- THIS-IS-TITLE -- THIS-IS-URL.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:37.000000 nics-2.6.0/nics/main/_template/docs/tree/2 -- Bar -- bar/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/_template/docs/tree/2 -- Bar -- bar/Hello -- world.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/_template/docs/tree/2 -- Bar -- bar/Without Numbering -- Without-Numbering.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/_template/docs/tree/2 -- Bar -- bar/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:37.000000 nics-2.6.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:37.000000 nics-2.6.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/Without index.md -- without-index-md.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/02 -- bar -- bar.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/index.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/_template/docs/tree/4 -- About -- about.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/_template/docs/tree/5 -- This is a demo -- This-Is-A-Demo.md
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/_template/docs/tree/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/_template/docs/tree/nics-logo500.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:37.000000 nics-2.6.0/nics/main/_template/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:37.000000 nics-2.6.0/nics/main/_template/web/_layouts/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/_template/web/_layouts/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:37.000000 nics-2.6.0/nics/main/_template/web/_sass/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/_template/web/_sass/footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/_template/web/_sass/header.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/_template/web/_sass/main.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:37.000000 nics-2.6.0/nics/main/_template/web/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/_template/web/scripts/header.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:37.000000 nics-2.6.0/nics/main/compile/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/compile/copying_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/compile/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/compile/update_404_and_favicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/compile/update_docs_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/compile/update_footer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/compile/update_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/compile/update_jekyll_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/compile/update_sass_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:37.000000 nics-2.6.0/nics/main/upgrade/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/upgrade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:37.000000 nics-2.6.0/nics/main/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/wizard/settings_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-01 19:34:22.000000 nics-2.6.0/nics/main/wizard/workflow_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:34:37.000000 nics-2.6.0/nics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-01 19:34:37.000000 nics-2.6.0/nics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-01 19:34:37.000000 nics-2.6.0/nics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 19:34:37.000000 nics-2.6.0/nics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-01 19:34:37.000000 nics-2.6.0/nics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-01 19:34:37.000000 nics-2.6.0/nics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 19:34:37.000000 nics-2.6.0/nics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-01 19:34:22.000000 nics-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 19:34:37.000000 nics-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-01 19:34:22.000000 nics-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-01 19:47:22.000000 nics-2.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-01 19:47:22.000000 nics-2.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-01 19:47:39.000000 nics-2.6.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-01 19:47:22.000000 nics-2.6.1/nics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/_template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/404.md
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/_template/docs/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/1 -- THIS-IS-TITLE -- THIS-IS-URL.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/_template/docs/tree/2 -- Bar -- bar/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/2 -- Bar -- bar/Hello -- world.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/2 -- Bar -- bar/Without Numbering -- Without-Numbering.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/2 -- Bar -- bar/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/Without index.md -- without-index-md.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/02 -- bar -- bar.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/4 -- About -- about.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/5 -- This is a demo -- This-Is-A-Demo.md
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/docs/tree/nics-logo500.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/_template/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/_template/web/_layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/web/_layouts/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/_template/web/_sass/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/web/_sass/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/web/_sass/header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/web/_sass/main.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/_template/web/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/_template/web/scripts/header.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/compile/copying_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/compile/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/compile/update_404_and_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/compile/update_docs_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/compile/update_footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/compile/update_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/compile/update_jekyll_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/compile/update_sass_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/upgrade/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/upgrade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics/main/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/wizard/settings_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-01 19:47:22.000000 nics-2.6.1/nics/main/wizard/workflow_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:47:39.000000 nics-2.6.1/nics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-01 19:47:39.000000 nics-2.6.1/nics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-01 19:47:39.000000 nics-2.6.1/nics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 19:47:39.000000 nics-2.6.1/nics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-01 19:47:39.000000 nics-2.6.1/nics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-01 19:47:39.000000 nics-2.6.1/nics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 19:47:39.000000 nics-2.6.1/nics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-01 19:47:22.000000 nics-2.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 19:47:39.000000 nics-2.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-01 19:47:22.000000 nics-2.6.1/setup.py
```

### Comparing `nics-2.6.0/LICENSE` & `nics-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nics-2.6.0/PKG-INFO` & `nics-2.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 2.6.0
-Summary: Minimalist GitHub documentation tool
+Version: 2.6.1
+Summary: Automated markdown-based documentation tool
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: Report bugs, https://github.com/nvfp/now-i-can-sleep/issues
 Project-URL: Repository, https://github.com/nvfp/now-i-can-sleep
```

### Comparing `nics-2.6.0/nics/main/__init__.py` & `nics-2.6.1/nics/main/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.0/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg` & `nics-2.6.1/nics/main/_template/docs/tree/2 -- Bar -- bar/nics-logo500.jpg`

 * *Files identical despite different names*

### Comparing `nics-2.6.0/nics/main/_template/docs/tree/nics-logo500.jpg` & `nics-2.6.1/nics/main/_template/docs/tree/nics-logo500.jpg`

 * *Files identical despite different names*

### Comparing `nics-2.6.0/nics/main/_template/web/_sass/header.scss` & `nics-2.6.1/nics/main/_template/web/_sass/header.scss`

 * *Files identical despite different names*

### Comparing `nics-2.6.0/nics/main/_template/web/_sass/main.scss` & `nics-2.6.1/nics/main/_template/web/_sass/main.scss`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 ---
 # Jekyll requires this front matter, including the "#" sign, to convert main.scss to main.css.
 ---
 
 @import url('https://fonts.googleapis.com/css2?family=Caveat&display=swap');
-@import url('https://fonts.googleapis.com/css2?family=Caveat&family=Grandstander&display=swap');
-@import url('https://fonts.googleapis.com/css2?family=Ubuntu+Mono&display=swap');
 $font: 'Caveat', cursive;
+@import url('https://fonts.googleapis.com/css2?family=Caveat&family=Grandstander&display=swap');
 $font2: 'Grandstander', cursive;
-$font3: 'Ubuntu Mono', monospace;
+// monospace font
+@import url('https://fonts.googleapis.com/css2?family=IBM+Plex+Mono&display=swap');
+$font3: 'IBM Plex Mono', monospace;
 
 $font-size-mobile: 16px;
 $mobile-width: 850px;
 
 @import "constants";  // will be created during compilation
 @import "header";
 @import "footer";
```

### Comparing `nics-2.6.0/nics/main/_template/web/scripts/header.js` & `nics-2.6.1/nics/main/_template/web/scripts/header.js`

 * *Files identical despite different names*

### Comparing `nics-2.6.0/nics/main/compile/__init__.py` & `nics-2.6.1/nics/main/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.0/nics/main/compile/copying_template.py` & `nics-2.6.1/nics/main/compile/copying_template.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.0/nics/main/compile/update_404_and_favicon.py` & `nics-2.6.1/nics/main/compile/update_404_and_favicon.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.0/nics/main/compile/update_docs_tree.py` & `nics-2.6.1/nics/main/compile/update_docs_tree.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.0/nics/main/compile/update_header.py` & `nics-2.6.1/nics/main/compile/update_header.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.0/nics/main/compile/update_jekyll_config.py` & `nics-2.6.1/nics/main/compile/update_jekyll_config.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.0/nics/main/constants.py` & `nics-2.6.1/nics/main/constants.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.0/nics/main/upgrade/__init__.py` & `nics-2.6.1/nics/main/upgrade/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.0/nics/main/wizard/__init__.py` & `nics-2.6.1/nics/main/wizard/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.0/nics/main/wizard/settings_writer.py` & `nics-2.6.1/nics/main/wizard/settings_writer.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.0/nics/main/wizard/workflow_writer.py` & `nics-2.6.1/nics/main/wizard/workflow_writer.py`

 * *Files identical despite different names*

### Comparing `nics-2.6.0/nics.egg-info/PKG-INFO` & `nics-2.6.1/nics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 2.6.0
-Summary: Minimalist GitHub documentation tool
+Version: 2.6.1
+Summary: Automated markdown-based documentation tool
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: Report bugs, https://github.com/nvfp/now-i-can-sleep/issues
 Project-URL: Repository, https://github.com/nvfp/now-i-can-sleep
```

### Comparing `nics-2.6.0/nics.egg-info/SOURCES.txt` & `nics-2.6.1/nics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nics-2.6.0/pyproject.toml` & `nics-2.6.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "nics"
-version = "2.6.0"
-description = "Minimalist GitHub documentation tool"
+version = "2.6.1"
+description = "Automated markdown-based documentation tool"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
 keywords = ["python", "toolkit", "mykit"]
```

