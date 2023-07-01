# Comparing `tmp/aa-simplewiki-1.0.4.tar.gz` & `tmp/aa-simplewiki-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-simplewiki-1.0.4.tar", last modified: Mon Jun 26 14:49:20 2023, max compression
+gzip compressed data, was "aa-simplewiki-1.0.5.tar", last modified: Sat Jul  1 19:41:52 2023, max compression
```

## Comparing `aa-simplewiki-1.0.4.tar` & `aa-simplewiki-1.0.5.tar`

### file list

```diff
@@ -1,80 +1,93 @@
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.703167 aa-simplewiki-1.0.4/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    35164 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/LICENSE
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      123 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/MANIFEST.in
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5930 2023-06-26 14:49:20.703167 aa-simplewiki-1.0.4/PKG-INFO
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4921 2023-06-26 14:44:07.000000 aa-simplewiki-1.0.4/README.md
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.695167 aa-simplewiki-1.0.4/aa_simplewiki.egg-info/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5930 2023-06-26 14:49:20.000000 aa-simplewiki-1.0.4/aa_simplewiki.egg-info/PKG-INFO
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2708 2023-06-26 14:49:20.000000 aa-simplewiki-1.0.4/aa_simplewiki.egg-info/SOURCES.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-06-26 14:49:20.000000 aa-simplewiki-1.0.4/aa_simplewiki.egg-info/dependency_links.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-06-22 13:24:11.000000 aa-simplewiki-1.0.4/aa_simplewiki.egg-info/not-zip-safe
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       28 2023-06-26 14:49:20.000000 aa-simplewiki-1.0.4/aa_simplewiki.egg-info/requires.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       20 2023-06-26 14:49:20.000000 aa-simplewiki-1.0.4/aa_simplewiki.egg-info/top_level.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      104 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/pyproject.toml
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1434 2023-06-26 14:49:20.703167 aa-simplewiki-1.0.4/setup.cfg
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1253 2023-06-26 14:24:39.000000 aa-simplewiki-1.0.4/setup.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.699167 aa-simplewiki-1.0.4/simplewiki/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       47 2023-06-26 14:22:59.000000 aa-simplewiki-1.0.4/simplewiki/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      231 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/admin.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    11916 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/admin_helper_menus.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     8956 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/admin_helper_sections.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      169 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/app_settings.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      284 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/apps.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/auth_hooks.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.699167 aa-simplewiki-1.0.4/simplewiki/migrations/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1489 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0001_initial.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      395 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0002_pageitem_page_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      401 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0003_menuitem_icon.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1532 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1522 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      374 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0006_rename_pageitem_sectionitem.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      392 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0007_rename_page_title_sectionitem_section_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1657 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      658 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      381 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0010_rename_path_menuitem_name.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      372 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0011_rename_name_menuitem_path.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      576 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0012_menuitem_group.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      579 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0013_alter_menuitem_group.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     3030 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      685 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      407 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0016_rename_section_title_sectionitem_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      831 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      399 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0018_rename_group_menuitem_groups.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      492 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0019_alter_general_options.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      538 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0020_menuitem_parent.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4236 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/models.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.695167 aa-simplewiki-1.0.4/simplewiki/static/
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.699167 aa-simplewiki-1.0.4/simplewiki/static/simplewiki/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/static/simplewiki/.gitkeep
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    44136 2023-06-22 23:46:34.000000 aa-simplewiki-1.0.4/simplewiki/static/simplewiki/Sortable.min.js
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      199 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/static/simplewiki/custom.css
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      226 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/tasks.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.695167 aa-simplewiki-1.0.4/simplewiki/templates/
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.699167 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6725 2023-06-26 13:24:54.000000 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/base.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-06-26 12:25:27.000000 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/dynamic_page.html
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.699167 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6630 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/editor_menus.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9500 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/editor_sections.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     3001 2023-06-23 00:32:43.000000 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/editor_sort.html
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.699167 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/partials/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2320 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/partials/_create_menu.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2468 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      593 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/error.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      460 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/index.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1578 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/search.html
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.703167 aa-simplewiki-1.0.4/simplewiki/templatetags/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2327 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/templatetags/custom_filters.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2145 2023-06-26 14:07:13.000000 aa-simplewiki-1.0.4/simplewiki/templatetags/markdown_filters.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.703167 aa-simplewiki-1.0.4/simplewiki/tests/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       27 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/tests/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      448 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/tests/test_example.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      561 2023-06-26 13:47:46.000000 aa-simplewiki-1.0.4/simplewiki/urls.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    13176 2023-06-26 13:47:40.000000 aa-simplewiki-1.0.4/simplewiki/views.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.703167 aa-simplewiki-1.0.4/testauth/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       52 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/testauth/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      654 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/testauth/celery.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9481 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/testauth/settings.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      167 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/testauth/urls.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      425 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/testauth/wsgi.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-07-01 19:41:52.983166 aa-simplewiki-1.0.5/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    35164 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/LICENSE
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      123 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/MANIFEST.in
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6224 2023-07-01 19:41:52.983166 aa-simplewiki-1.0.5/PKG-INFO
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5215 2023-07-01 10:41:32.000000 aa-simplewiki-1.0.5/README.md
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-07-01 19:41:52.951166 aa-simplewiki-1.0.5/aa_simplewiki.egg-info/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6224 2023-07-01 19:41:52.000000 aa-simplewiki-1.0.5/aa_simplewiki.egg-info/PKG-INFO
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     3439 2023-07-01 19:41:52.000000 aa-simplewiki-1.0.5/aa_simplewiki.egg-info/SOURCES.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-07-01 19:41:52.000000 aa-simplewiki-1.0.5/aa_simplewiki.egg-info/dependency_links.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-06-22 13:24:11.000000 aa-simplewiki-1.0.5/aa_simplewiki.egg-info/not-zip-safe
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       51 2023-07-01 19:41:52.000000 aa-simplewiki-1.0.5/aa_simplewiki.egg-info/requires.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       20 2023-07-01 19:41:52.000000 aa-simplewiki-1.0.5/aa_simplewiki.egg-info/top_level.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      104 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/pyproject.toml
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1434 2023-07-01 19:41:52.983166 aa-simplewiki-1.0.5/setup.cfg
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1283 2023-07-01 10:40:43.000000 aa-simplewiki-1.0.5/setup.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-07-01 19:41:52.955166 aa-simplewiki-1.0.5/simplewiki/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       72 2023-07-01 10:27:36.000000 aa-simplewiki-1.0.5/simplewiki/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      231 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/simplewiki/admin.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    11916 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/simplewiki/admin_helper_menus.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     8956 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/simplewiki/admin_helper_sections.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      169 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/simplewiki/app_settings.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      284 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/simplewiki/apps.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/simplewiki/auth_hooks.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-07-01 19:41:52.955166 aa-simplewiki-1.0.5/simplewiki/markdown/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4712 2023-06-30 21:57:11.000000 aa-simplewiki-1.0.5/simplewiki/markdown/renderer.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-07-01 19:41:52.967166 aa-simplewiki-1.0.5/simplewiki/migrations/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1489 2023-07-01 11:33:48.000000 aa-simplewiki-1.0.5/simplewiki/migrations/0001_initial.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      395 2023-07-01 11:33:48.000000 aa-simplewiki-1.0.5/simplewiki/migrations/0002_pageitem_page_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      401 2023-07-01 11:33:48.000000 aa-simplewiki-1.0.5/simplewiki/migrations/0003_menuitem_icon.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1532 2023-07-01 11:33:48.000000 aa-simplewiki-1.0.5/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1522 2023-07-01 11:33:48.000000 aa-simplewiki-1.0.5/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      374 2023-07-01 11:33:48.000000 aa-simplewiki-1.0.5/simplewiki/migrations/0006_rename_pageitem_sectionitem.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      392 2023-07-01 11:33:48.000000 aa-simplewiki-1.0.5/simplewiki/migrations/0007_rename_page_title_sectionitem_section_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1657 2023-07-01 11:33:48.000000 aa-simplewiki-1.0.5/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      658 2023-07-01 11:33:48.000000 aa-simplewiki-1.0.5/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      381 2023-07-01 11:33:48.000000 aa-simplewiki-1.0.5/simplewiki/migrations/0010_rename_path_menuitem_name.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      372 2023-07-01 11:33:48.000000 aa-simplewiki-1.0.5/simplewiki/migrations/0011_rename_name_menuitem_path.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      576 2023-07-01 11:33:48.000000 aa-simplewiki-1.0.5/simplewiki/migrations/0012_menuitem_group.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      579 2023-07-01 11:33:48.000000 aa-simplewiki-1.0.5/simplewiki/migrations/0013_alter_menuitem_group.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     3030 2023-07-01 11:33:48.000000 aa-simplewiki-1.0.5/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      685 2023-07-01 11:33:48.000000 aa-simplewiki-1.0.5/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      407 2023-07-01 11:33:48.000000 aa-simplewiki-1.0.5/simplewiki/migrations/0016_rename_section_title_sectionitem_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      831 2023-07-01 11:33:48.000000 aa-simplewiki-1.0.5/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      399 2023-07-01 11:33:48.000000 aa-simplewiki-1.0.5/simplewiki/migrations/0018_rename_group_menuitem_groups.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      492 2023-07-01 11:33:48.000000 aa-simplewiki-1.0.5/simplewiki/migrations/0019_alter_general_options.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      538 2023-07-01 11:33:48.000000 aa-simplewiki-1.0.5/simplewiki/migrations/0020_menuitem_parent.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-07-01 11:33:48.000000 aa-simplewiki-1.0.5/simplewiki/migrations/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4236 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/simplewiki/models.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-07-01 19:41:52.947166 aa-simplewiki-1.0.5/simplewiki/static/
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-07-01 19:41:52.967166 aa-simplewiki-1.0.5/simplewiki/static/simplewiki/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/simplewiki/static/simplewiki/.gitkeep
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    44136 2023-06-22 23:46:34.000000 aa-simplewiki-1.0.5/simplewiki/static/simplewiki/Sortable.min.js
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      199 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/simplewiki/static/simplewiki/custom.css
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      226 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/simplewiki/tasks.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-07-01 19:41:52.947166 aa-simplewiki-1.0.5/simplewiki/templates/
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-07-01 19:41:52.967166 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6725 2023-06-27 13:15:16.000000 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/base.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-06-27 19:36:10.000000 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/dynamic_page.html
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-07-01 19:41:52.971166 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6630 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/editor_menus.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9515 2023-06-26 23:59:53.000000 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/editor_sections.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     3001 2023-06-23 00:32:43.000000 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/editor_sort.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     3305 2023-06-29 23:27:43.000000 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/guide.html
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-07-01 19:41:52.975166 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/guide_partials/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1453 2023-06-30 22:01:59.000000 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/guide_partials/_guide_alert.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1201 2023-06-30 22:02:07.000000 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/guide_partials/_guide_block.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1210 2023-06-30 22:01:27.000000 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/guide_partials/_guide_gdrive.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1156 2023-06-30 22:02:44.000000 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/guide_partials/_guide_heading.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      609 2023-06-30 22:02:54.000000 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/guide_partials/_guide_image.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1131 2023-06-30 22:02:15.000000 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/guide_partials/_guide_list.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2344 2023-06-30 22:02:26.000000 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/guide_partials/_guide_table.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4542 2023-06-30 22:12:26.000000 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/guide_partials/_guide_text.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      965 2023-06-30 22:03:09.000000 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/guide_partials/_guide_video.html
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-07-01 19:41:52.979166 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/partials/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2320 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/partials/_create_menu.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2468 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      593 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/error.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      460 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/index.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1578 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/search.html
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-07-01 19:41:52.979166 aa-simplewiki-1.0.5/simplewiki/templatetags/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2327 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/simplewiki/templatetags/custom_filters.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      528 2023-06-27 19:24:33.000000 aa-simplewiki-1.0.5/simplewiki/templatetags/markdown_filters.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-07-01 19:41:52.979166 aa-simplewiki-1.0.5/simplewiki/tests/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       27 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/simplewiki/tests/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      448 2023-06-26 20:30:20.000000 aa-simplewiki-1.0.5/simplewiki/tests/test_example.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      679 2023-06-27 19:18:31.000000 aa-simplewiki-1.0.5/simplewiki/urls.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    14640 2023-07-01 11:56:19.000000 aa-simplewiki-1.0.5/simplewiki/views.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-07-01 19:41:52.983166 aa-simplewiki-1.0.5/testauth/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       52 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/testauth/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      654 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/testauth/celery.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9481 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/testauth/settings.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      167 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/testauth/urls.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      425 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.5/testauth/wsgi.py
```

### Comparing `aa-simplewiki-1.0.4/LICENSE` & `aa-simplewiki-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/PKG-INFO` & `aa-simplewiki-1.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-simplewiki
-Version: 1.0.4
+Version: 1.0.5
 Summary: Alliance Auth Wiki Plugin
 Home-page: https://github.com/meowosaurus/aa-simplewiki
 Author: Meowosaurus
 Author-email: info@bjsonnen.de
 Maintainer: Meowosaurus
 Maintainer-email: info@bjsonnen.de
 License: GNU General Public License v3 (GPLv3)
@@ -20,15 +20,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SimpleWiki
-A simple wiki system for alliance auth. It supports multiple pages with different sections. Every page and every section can have their own icon.
+A simple wiki plugin for alliance auth. It supports multiple pages with different sections. Every page and every section can have their own icon. Written in Python with Django.
 
 # Contents
 * [Current Features](#current-features)
   * [ToDo](#todo)
   * [Planned](#planned)
 * [Screenshots](#screenshots)
 * [Installation](#installation)
@@ -40,31 +40,32 @@
 * [Permissions](#permissions)
 * [Support](#support)
 
 # Current Features
 * Create custom wiki menus with dropdowns plus different sections on each menu
 * Add an icon next to menus or sections
 * Edit pages on the admin panel with [markdown](https://www.markdownguide.org/cheat-sheet/)
-  * Support for images
+  * Support for all major GitHub markdown features
   * Support for videos (YouTube and Vimeo)
+  * Support for alerts and Google Drive
 * Search function: Search across all wiki menus and sections
 * Permission system:
   * Editor permissions can be added to single users or groups via the admin panel
   * Alliance Auth groups are synced to simplewiki: Certain pages can only be seen by a specific group
   * Multiple groups support: As long as the user is in any of the required groups, they can access the menu
 * Editor interface
   * Users with editor permission can create, edit and delete custom menus and sections (editor_access)
   * Users with editor permission see edit and delete buttons above all sections (editor_access)
 
 ## ToDo:
 * Quality-of-life updates
+* Implement better logging
 * Improve code documentation
 * Clean-up code
 * Markdown
-  * Tables
   * Buttons
 
 ## Planned
 * Drag and drop system to make indexing menus and sections easier
 * Add translations for 
   * German
   * Spanish
@@ -95,29 +96,27 @@
 ### Alliance Auth Production
 
 #### Non-Docker Version
 1.) Install the pip package via `pip install aa-simplewiki`
 
 2.) Add `simplewiki` to your `INSTALLED_APPS` in your projects `local.py`
 
-3.) Make migrations and migrate, then restart your server
+3.) Restart your server, then run migrations and collectstatic
 
 #### Docker Version
 1.) Please make sure you followed the custom docker-image tutorial [here](https://gitlab.com/allianceauth/allianceauth/-/tree/master/docker#using-a-custom-docker-image): 
 
 2.) Edit your `conf/requirements` and add the following line `aa-simplewiki` (Check https://pypi.org/project/aa-simplewiki/ for different versions!)
 
 3.) Add `simplewiki` to your `INSTALLED_APPS` in your projects `local.py`
 
 4.) Start your server `docker compose --env-file=.env up -d`
 
 5.) Run `docker compose exec allianceauth bash`
 
-6.) Run `allianceauth update myauth`
-
 7.) Run `auth migrate`
 
 8.) Run `auth collectstatic`
 
 ### Alliance Auth Development 
 Make sure you have installed alliance auth in the correct way: https://allianceauth.readthedocs.io/en/latest/development/dev_setup/index.html
 
@@ -154,9 +153,14 @@
 
 ## Permissions
 Perm | Admin Site | Auth Site 
  --- | --- | --- 
 basic_access | None | Can view all wiki pages
 editor_access | None | Can create, edit and delete wiki pages and menus
 
+## Dependencies
+- [Alliance Auth](https://gitlab.com/allianceauth/allianceauth)
+- [allianceauth-app-utils](https://gitlab.com/ErikKalkoken/allianceauth-app-utils)
+- [Mistune](https://github.com/lepture/mistune)
+
 ## Support
 * On Discord: meowlicious
```

### Comparing `aa-simplewiki-1.0.4/README.md` & `aa-simplewiki-1.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SimpleWiki
-A simple wiki system for alliance auth. It supports multiple pages with different sections. Every page and every section can have their own icon.
+A simple wiki plugin for alliance auth. It supports multiple pages with different sections. Every page and every section can have their own icon. Written in Python with Django.
 
 # Contents
 * [Current Features](#current-features)
   * [ToDo](#todo)
   * [Planned](#planned)
 * [Screenshots](#screenshots)
 * [Installation](#installation)
@@ -15,31 +15,32 @@
 * [Permissions](#permissions)
 * [Support](#support)
 
 # Current Features
 * Create custom wiki menus with dropdowns plus different sections on each menu
 * Add an icon next to menus or sections
 * Edit pages on the admin panel with [markdown](https://www.markdownguide.org/cheat-sheet/)
-  * Support for images
+  * Support for all major GitHub markdown features
   * Support for videos (YouTube and Vimeo)
+  * Support for alerts and Google Drive
 * Search function: Search across all wiki menus and sections
 * Permission system:
   * Editor permissions can be added to single users or groups via the admin panel
   * Alliance Auth groups are synced to simplewiki: Certain pages can only be seen by a specific group
   * Multiple groups support: As long as the user is in any of the required groups, they can access the menu
 * Editor interface
   * Users with editor permission can create, edit and delete custom menus and sections (editor_access)
   * Users with editor permission see edit and delete buttons above all sections (editor_access)
 
 ## ToDo:
 * Quality-of-life updates
+* Implement better logging
 * Improve code documentation
 * Clean-up code
 * Markdown
-  * Tables
   * Buttons
 
 ## Planned
 * Drag and drop system to make indexing menus and sections easier
 * Add translations for 
   * German
   * Spanish
@@ -70,29 +71,27 @@
 ### Alliance Auth Production
 
 #### Non-Docker Version
 1.) Install the pip package via `pip install aa-simplewiki`
 
 2.) Add `simplewiki` to your `INSTALLED_APPS` in your projects `local.py`
 
-3.) Make migrations and migrate, then restart your server
+3.) Restart your server, then run migrations and collectstatic
 
 #### Docker Version
 1.) Please make sure you followed the custom docker-image tutorial [here](https://gitlab.com/allianceauth/allianceauth/-/tree/master/docker#using-a-custom-docker-image): 
 
 2.) Edit your `conf/requirements` and add the following line `aa-simplewiki` (Check https://pypi.org/project/aa-simplewiki/ for different versions!)
 
 3.) Add `simplewiki` to your `INSTALLED_APPS` in your projects `local.py`
 
 4.) Start your server `docker compose --env-file=.env up -d`
 
 5.) Run `docker compose exec allianceauth bash`
 
-6.) Run `allianceauth update myauth`
-
 7.) Run `auth migrate`
 
 8.) Run `auth collectstatic`
 
 ### Alliance Auth Development 
 Make sure you have installed alliance auth in the correct way: https://allianceauth.readthedocs.io/en/latest/development/dev_setup/index.html
 
@@ -129,9 +128,14 @@
 
 ## Permissions
 Perm | Admin Site | Auth Site 
  --- | --- | --- 
 basic_access | None | Can view all wiki pages
 editor_access | None | Can create, edit and delete wiki pages and menus
 
+## Dependencies
+- [Alliance Auth](https://gitlab.com/allianceauth/allianceauth)
+- [allianceauth-app-utils](https://gitlab.com/ErikKalkoken/allianceauth-app-utils)
+- [Mistune](https://github.com/lepture/mistune)
+
 ## Support
 * On Discord: meowlicious
```

### Comparing `aa-simplewiki-1.0.4/aa_simplewiki.egg-info/PKG-INFO` & `aa-simplewiki-1.0.5/aa_simplewiki.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-simplewiki
-Version: 1.0.4
+Version: 1.0.5
 Summary: Alliance Auth Wiki Plugin
 Home-page: https://github.com/meowosaurus/aa-simplewiki
 Author: Meowosaurus
 Author-email: info@bjsonnen.de
 Maintainer: Meowosaurus
 Maintainer-email: info@bjsonnen.de
 License: GNU General Public License v3 (GPLv3)
@@ -20,15 +20,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SimpleWiki
-A simple wiki system for alliance auth. It supports multiple pages with different sections. Every page and every section can have their own icon.
+A simple wiki plugin for alliance auth. It supports multiple pages with different sections. Every page and every section can have their own icon. Written in Python with Django.
 
 # Contents
 * [Current Features](#current-features)
   * [ToDo](#todo)
   * [Planned](#planned)
 * [Screenshots](#screenshots)
 * [Installation](#installation)
@@ -40,31 +40,32 @@
 * [Permissions](#permissions)
 * [Support](#support)
 
 # Current Features
 * Create custom wiki menus with dropdowns plus different sections on each menu
 * Add an icon next to menus or sections
 * Edit pages on the admin panel with [markdown](https://www.markdownguide.org/cheat-sheet/)
-  * Support for images
+  * Support for all major GitHub markdown features
   * Support for videos (YouTube and Vimeo)
+  * Support for alerts and Google Drive
 * Search function: Search across all wiki menus and sections
 * Permission system:
   * Editor permissions can be added to single users or groups via the admin panel
   * Alliance Auth groups are synced to simplewiki: Certain pages can only be seen by a specific group
   * Multiple groups support: As long as the user is in any of the required groups, they can access the menu
 * Editor interface
   * Users with editor permission can create, edit and delete custom menus and sections (editor_access)
   * Users with editor permission see edit and delete buttons above all sections (editor_access)
 
 ## ToDo:
 * Quality-of-life updates
+* Implement better logging
 * Improve code documentation
 * Clean-up code
 * Markdown
-  * Tables
   * Buttons
 
 ## Planned
 * Drag and drop system to make indexing menus and sections easier
 * Add translations for 
   * German
   * Spanish
@@ -95,29 +96,27 @@
 ### Alliance Auth Production
 
 #### Non-Docker Version
 1.) Install the pip package via `pip install aa-simplewiki`
 
 2.) Add `simplewiki` to your `INSTALLED_APPS` in your projects `local.py`
 
-3.) Make migrations and migrate, then restart your server
+3.) Restart your server, then run migrations and collectstatic
 
 #### Docker Version
 1.) Please make sure you followed the custom docker-image tutorial [here](https://gitlab.com/allianceauth/allianceauth/-/tree/master/docker#using-a-custom-docker-image): 
 
 2.) Edit your `conf/requirements` and add the following line `aa-simplewiki` (Check https://pypi.org/project/aa-simplewiki/ for different versions!)
 
 3.) Add `simplewiki` to your `INSTALLED_APPS` in your projects `local.py`
 
 4.) Start your server `docker compose --env-file=.env up -d`
 
 5.) Run `docker compose exec allianceauth bash`
 
-6.) Run `allianceauth update myauth`
-
 7.) Run `auth migrate`
 
 8.) Run `auth collectstatic`
 
 ### Alliance Auth Development 
 Make sure you have installed alliance auth in the correct way: https://allianceauth.readthedocs.io/en/latest/development/dev_setup/index.html
 
@@ -154,9 +153,14 @@
 
 ## Permissions
 Perm | Admin Site | Auth Site 
  --- | --- | --- 
 basic_access | None | Can view all wiki pages
 editor_access | None | Can create, edit and delete wiki pages and menus
 
+## Dependencies
+- [Alliance Auth](https://gitlab.com/allianceauth/allianceauth)
+- [allianceauth-app-utils](https://gitlab.com/ErikKalkoken/allianceauth-app-utils)
+- [Mistune](https://github.com/lepture/mistune)
+
 ## Support
 * On Discord: meowlicious
```

### Comparing `aa-simplewiki-1.0.4/aa_simplewiki.egg-info/SOURCES.txt` & `aa-simplewiki-1.0.5/aa_simplewiki.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 simplewiki/app_settings.py
 simplewiki/apps.py
 simplewiki/auth_hooks.py
 simplewiki/models.py
 simplewiki/tasks.py
 simplewiki/urls.py
 simplewiki/views.py
+simplewiki/markdown/renderer.py
 simplewiki/migrations/0001_initial.py
 simplewiki/migrations/0002_pageitem_page_title.py
 simplewiki/migrations/0003_menuitem_icon.py
 simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py
 simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py
 simplewiki/migrations/0006_rename_pageitem_sectionitem.py
 simplewiki/migrations/0007_rename_page_title_sectionitem_section_title.py
@@ -49,14 +50,24 @@
 simplewiki/templates/simplewiki/dynamic_page.html
 simplewiki/templates/simplewiki/error.html
 simplewiki/templates/simplewiki/index.html
 simplewiki/templates/simplewiki/search.html
 simplewiki/templates/simplewiki/editor/editor_menus.html
 simplewiki/templates/simplewiki/editor/editor_sections.html
 simplewiki/templates/simplewiki/editor/editor_sort.html
+simplewiki/templates/simplewiki/editor/guide.html
+simplewiki/templates/simplewiki/editor/guide_partials/_guide_alert.html
+simplewiki/templates/simplewiki/editor/guide_partials/_guide_block.html
+simplewiki/templates/simplewiki/editor/guide_partials/_guide_gdrive.html
+simplewiki/templates/simplewiki/editor/guide_partials/_guide_heading.html
+simplewiki/templates/simplewiki/editor/guide_partials/_guide_image.html
+simplewiki/templates/simplewiki/editor/guide_partials/_guide_list.html
+simplewiki/templates/simplewiki/editor/guide_partials/_guide_table.html
+simplewiki/templates/simplewiki/editor/guide_partials/_guide_text.html
+simplewiki/templates/simplewiki/editor/guide_partials/_guide_video.html
 simplewiki/templates/simplewiki/editor/partials/_create_menu.html
 simplewiki/templates/simplewiki/editor/partials/_edit_menu.html
 simplewiki/templatetags/custom_filters.py
 simplewiki/templatetags/markdown_filters.py
 simplewiki/tests/__init__.py
 simplewiki/tests/test_example.py
 testauth/__init__.py
```

### Comparing `aa-simplewiki-1.0.4/setup.cfg` & `aa-simplewiki-1.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/setup.py` & `aa-simplewiki-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 install_requires = [
     'mistune>=3.0.1',
     'allianceauth',
+    'allianceauth-app-utils',
 ]
 
 setup(
     name='aa-simplewiki',
     version=__version__,
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `aa-simplewiki-1.0.4/simplewiki/admin_helper_menus.py` & `aa-simplewiki-1.0.5/simplewiki/admin_helper_menus.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/admin_helper_sections.py` & `aa-simplewiki-1.0.5/simplewiki/admin_helper_sections.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/auth_hooks.py` & `aa-simplewiki-1.0.5/simplewiki/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/migrations/0001_initial.py` & `aa-simplewiki-1.0.5/simplewiki/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py` & `aa-simplewiki-1.0.5/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py` & `aa-simplewiki-1.0.5/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py` & `aa-simplewiki-1.0.5/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py` & `aa-simplewiki-1.0.5/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/migrations/0012_menuitem_group.py` & `aa-simplewiki-1.0.5/simplewiki/migrations/0012_menuitem_group.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/migrations/0013_alter_menuitem_group.py` & `aa-simplewiki-1.0.5/simplewiki/migrations/0013_alter_menuitem_group.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py` & `aa-simplewiki-1.0.5/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py` & `aa-simplewiki-1.0.5/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py` & `aa-simplewiki-1.0.5/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/migrations/0020_menuitem_parent.py` & `aa-simplewiki-1.0.5/simplewiki/migrations/0020_menuitem_parent.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/models.py` & `aa-simplewiki-1.0.5/simplewiki/models.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/static/simplewiki/Sortable.min.js` & `aa-simplewiki-1.0.5/simplewiki/static/simplewiki/Sortable.min.js`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/base.html` & `aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/base.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/dynamic_page.html` & `aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/dynamic_page.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/editor_menus.html` & `aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/editor_menus.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/editor_sections.html` & `aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/editor_sections.html`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,15 @@
           <label for="exampleInputPassword1">Icon:</label>
           <input type="text" class="form-control" name="icon" id="iconInput" placeholder="{{ selectedSection.icon }}">
           <p class="help-block">Optional: Go to <a href="https://fontawesome.com/v5/search">https://fontawesome.com/v5/search</a> to find matching icons. We only support free icons. Format example: fas fa-hand-spock</p>
         </div>
         <div class="form-group">
           <label for="exampleInputPassword1">Content:</label>
           <textarea class="form-control" name="content" id="contentInput" rows="10">{{ selectedSection.content|safe }}</textarea>
-          <p class="help-block">Optional: This will be displayed as your main content of the section. You can use markdown. See <a href="https://commonmark.org/help/">https://commonmark.org/help/</a> for references.</p>
+          <p class="help-block">Optional: This will be displayed as your main content of the section. You can use markdown. Check our <a href="{% url 'simplewiki:editor_markdown_guide' %}" target="_blank">guide</a> for references.</p>
         </div>
         <button type="submit" name="confirm_edit" value="0" class="btn btn-default">Cancel</button>
         <div class="pull-right">
           <button type="submit" name="confirm_edit" value="1" class="btn btn-success">Save</button>
         </div>
       </form>
       {% elif user_action == 'delete' %}
```

#### html2text {}

```diff
@@ -48,15 +48,15 @@
 the further to the top is the section.
 Icon: [icon                ]
 Optional: Go to https://fontawesome.com/v5/search to find matching icons. We
 only support free icons. Format example: fas fa-hand-spock
 Content:
 {{ selectedSection.content|safe }}
 Optional: This will be displayed as your main content of the section. You can
-use markdown. See https://commonmark.org/help/ for references.
+use markdown. Check our guide for references.
 Cancel
 Save
 {% elif user_action == 'delete' %}
 Are you sure you want to delete the following section?
 
  {{ selectedSection.title }}
 {% csrf_token %} Cancel
```

### Comparing `aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/editor_sort.html` & `aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/editor_sort.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/partials/_create_menu.html` & `aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/partials/_create_menu.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html` & `aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/error.html` & `aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/error.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/search.html` & `aa-simplewiki-1.0.5/simplewiki/templates/simplewiki/search.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/templatetags/custom_filters.py` & `aa-simplewiki-1.0.5/simplewiki/templatetags/custom_filters.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/simplewiki/urls.py` & `aa-simplewiki-1.0.5/simplewiki/urls.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,8 +12,11 @@
     path('search/', views.search, name='search'),
     path('<str:menu_name>/', views.dynamic_menus, name='dynamic_menu'),
     
     # editor_access pages
     path("editor/menus/", views.editor_menus, name="editor_menus"),
     path("editor/sections/", views.editor_sections, name="editor_sections"),
     #path("editor/sort/", views.editor_sort, name="editor_sort"), # ToDo
+
+    # Markdown guide
+    path("editor/guides/markdown/", views.editor_markdown_guide, name="editor_markdown_guide"),
 ]
```

### Comparing `aa-simplewiki-1.0.4/simplewiki/views.py` & `aa-simplewiki-1.0.5/simplewiki/views.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,20 +8,27 @@
 from django.contrib.auth.models import Group
 from django.core.handlers.wsgi import WSGIRequest
 from django.http import HttpResponse
 from django.shortcuts import render, redirect
 from django.db.models import Q
 from django.core.exceptions import PermissionDenied
 
+from allianceauth.services.hooks import get_extension_logger
+
 # Custom imports
 from .models import MenuItem, SectionItem
 #from .admin_helper import *
 from .admin_helper_menus import *
 from .admin_helper_sections import *
 
+from app_utils.logging import LoggerAddTag
+from . import __title__
+
+logger = LoggerAddTag(get_extension_logger(__name__), __title__)
+
 ### Helper Functions ###
 
 # Standard context for a normal view, required by base.html
 def gen_context(request: WSGIRequest):
     """
     Generates the standard context for the django render function, 
     context includes all menu and section items, if the user is 
@@ -88,46 +95,60 @@
             if first_menu_submenus.count() > 0:
                 for first_menu_item in first_menu_submenus:
                     # If the submenu has any groups
                     if first_menu_item.groups:
                         group_names = first_menu_item.groups.split(',')
                         user_groups = list(request.user.groups.values_list('name', flat=True))
 
-                        print(group_names)
+                        logger_msg = f'Menu "{parent_menu_item.title}" has submenu "{first_menu_item.title}", checking if user "{request.user}" has permission to access it.'
+                        logger.info(logger_msg)
 
                         # If the user has the right to access this submenu
                         if any(group_name in user_groups for group_name in group_names) or any(element == "none" for element in group_names):
                             return redirect('simplewiki:dynamic_menu', first_menu_item)
                     else:
                         return redirect('simplewiki:dynamic_menu', first_menu_item)
             # If the menu doesn't have submenus
             else:
+                logger_msg = f'Unable to find any submenus for "{parent_menu_item}", checking if user "{request.user}" has permission to access it.'
+                logger.info(logger_msg)
+
                 # If the parent menu has any groups
                 if parent_menu_item.groups:
                     group_names = parent_menu_item.groups.split(',')
                     user_groups = list(request.user.groups.values_list('name', flat=True))
 
                     # If the user has the right to access the parent menu
                     if any(group_name in user_groups for group_name in group_names) or any(element == "none" for element in group_names):
                         return redirect('simplewiki:dynamic_menu', parent_menu_item)
                 else:
+                    
+
                     return redirect('simplewiki:dynamic_menu', parent_menu_item)
 
         # If there are no menus the user has permission to access
         error_code = "#1000"
         error_message = "You don't have the permission to access any menus. Please contact the administrator."
         context.update({'error_code': error_code})
         context.update({'error_msg': error_message})
+
+        logger_msg = f'Unable to render any menus: User "{request.user}" doesn\'t have the permission to access any menus.'
+        logger.error(logger_msg)
+
         return render(request, "simplewiki/error.html", context)
     # Show a default "create your first menu.." error page
     else:
         error_code = "#1000"
         error_message = "So far you didn't create any menus. Please create one under Admin -> Menus"
         context.update({'error_code': error_code})
         context.update({'error_msg': error_message})
+
+        logger_msg = f'Unable to render any menus: No menus created.'
+        logger.error(logger_msg)
+
         return render(request, "simplewiki/error.html", context)
 
 @login_required
 @permission_required("simplewiki.basic_access")
 def dynamic_menus(request: WSGIRequest, menu_name: str) -> HttpResponse:
     """
     Dynamic Page View, renders a page based on the URL. This view will check 
@@ -158,16 +179,24 @@
     except Exception as e:
         group_names = ""
 
     context.update({'group_names': group_names})
 
     #if not requested_menu.groups or requested_menu.groups in list(request.user.groups.values_list('name', flat=True)):
     if any(group_name in request.user.groups.values_list('name', flat=True) for group_name in group_names) or any(element == "none" or not element for element in group_names):
+        
+        logger_msg = f'Rendering wiki page "{menu_name}" for user "{request.user}".'
+        logger.info(logger_msg)
+
         return render(request, 'simplewiki/dynamic_page.html', context)
     else:
+        requested_groups = requested_menu.groups.replace(',', ', ')
+        logger_msg = f'Rejected rendering request for menu "{menu_name}", user "{request.user}" doesn\'t have neccessary groups "{requested_groups}"'
+        logger.info(logger_msg)
+
         # If more then two groups are required
         if len(requested_menu.groups.split(',')) > 1:
             group_plural = "groups"
         else:
             group_plural = "group"
         context.update({'error_code': '#1001'})
         print(requested_menu.groups.replace(',', ', '))
@@ -221,14 +250,15 @@
         return render(request, 'simplewiki/error.html', context)
     except Exception as e:
         frame = inspect.currentframe()
         context.update({'error_django': str(e)})
         file_name = inspect.getframeinfo(frame).filename
         line_number = inspect.getframeinfo(frame).lineno
         context.update({'error_msg': 'Unknown error in ' + file_name + ' in line ' + str(line_number)})
+
         return render(request, 'simplewiki/error.html', context)
 
     return render(request, "simplewiki/search.html", context)
 
 ### Admin Views ###
 
 @login_required
@@ -327,7 +357,13 @@
 @permission_required("simplewiki.editor_access")
 def editor_sort(request: WSGIRequest) -> HttpResponse:
     context = gen_context(request)
 
     return render(request, "simplewiki/editor/editor_sort.html", context)
 """
 
+@login_required
+@permission_required("simplewiki.editor_access")
+def editor_markdown_guide(request: WSGIRequest) -> HttpResponse:
+    context = gen_context(request)
+
+    return render(request, "simplewiki/editor/guide.html", context)
```

### Comparing `aa-simplewiki-1.0.4/testauth/celery.py` & `aa-simplewiki-1.0.5/testauth/celery.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.4/testauth/settings.py` & `aa-simplewiki-1.0.5/testauth/settings.py`

 * *Files identical despite different names*

