# Comparing `tmp/djangocms-rawhtml-1.2.1.tar.gz` & `tmp/djangocms-rawhtml-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-rawhtml-1.2.1.tar", last modified: Sat Dec 17 05:24:17 2022, max compression
+gzip compressed data, was "djangocms-rawhtml-1.3.0.tar", last modified: Sat Jul  1 09:28:36 2023, max compression
```

## Comparing `djangocms-rawhtml-1.2.1.tar` & `djangocms-rawhtml-1.3.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 nicka    (10001) Domain Users  (2513)        0 2022-12-17 05:24:17.623367 djangocms-rawhtml-1.2.1/
--rw-r--r--   0 nicka    (10001) Domain Users  (2513)     1528 2020-12-23 07:31:40.000000 djangocms-rawhtml-1.2.1/LICENSE
--rw-r--r--   0 nicka    (10001) Domain Users  (2513)       87 2020-12-23 07:31:40.000000 djangocms-rawhtml-1.2.1/MANIFEST.in
--rw-r--r--   0 nicka    (10001) Domain Users  (2513)     2693 2022-12-17 05:24:17.623367 djangocms-rawhtml-1.2.1/PKG-INFO
--rw-r--r--   0 nicka    (10001) Domain Users  (2513)     1263 2021-02-28 02:44:26.000000 djangocms-rawhtml-1.2.1/README.rst
-drwxr-xr-x   0 nicka    (10001) Domain Users  (2513)        0 2022-12-17 05:24:17.579366 djangocms-rawhtml-1.2.1/djangocms_rawhtml/
--rw-r--r--   0 nicka    (10001) Domain Users  (2513)        0 2020-12-23 07:31:40.000000 djangocms-rawhtml-1.2.1/djangocms_rawhtml/__init__.py
--rw-r--r--   0 nicka    (10001) Domain Users  (2513)     1229 2021-02-28 02:27:21.000000 djangocms-rawhtml-1.2.1/djangocms_rawhtml/cms_plugins.py
-drwxr-xr-x   0 nicka    (10001) Domain Users  (2513)        0 2022-12-17 05:24:17.599366 djangocms-rawhtml-1.2.1/djangocms_rawhtml/migrations/
--rw-r--r--   0 nicka    (10001) Domain Users  (2513)      925 2020-12-23 07:31:40.000000 djangocms-rawhtml-1.2.1/djangocms_rawhtml/migrations/0001_rawhtmlplugindata.py
--rw-r--r--   0 nicka    (10001) Domain Users  (2513)      586 2022-12-17 05:01:13.000000 djangocms-rawhtml-1.2.1/djangocms_rawhtml/migrations/0002_auto_20221216_1029.py
--rw-r--r--   0 nicka    (10001) Domain Users  (2513)        0 2020-12-23 07:31:40.000000 djangocms-rawhtml-1.2.1/djangocms_rawhtml/migrations/__init__.py
--rw-r--r--   0 nicka    (10001) Domain Users  (2513)      748 2020-12-23 07:36:11.000000 djangocms-rawhtml-1.2.1/djangocms_rawhtml/models.py
-drwxr-xr-x   0 nicka    (10001) Domain Users  (2513)        0 2022-12-17 05:24:17.579366 djangocms-rawhtml-1.2.1/djangocms_rawhtml/templates/
-drwxr-xr-x   0 nicka    (10001) Domain Users  (2513)        0 2022-12-17 05:24:17.579366 djangocms-rawhtml-1.2.1/djangocms_rawhtml/templates/admin/
-drwxr-xr-x   0 nicka    (10001) Domain Users  (2513)        0 2022-12-17 05:24:17.599366 djangocms-rawhtml-1.2.1/djangocms_rawhtml/templates/admin/djangocms_rawhtml/
--rw-r--r--   0 nicka    (10001) Domain Users  (2513)     1360 2021-02-28 02:26:11.000000 djangocms-rawhtml-1.2.1/djangocms_rawhtml/templates/admin/djangocms_rawhtml/change_form.html
-drwxr-xr-x   0 nicka    (10001) Domain Users  (2513)        0 2022-12-17 05:24:17.579366 djangocms-rawhtml-1.2.1/djangocms_rawhtml/templates/djangocms_rawhtml/
-drwxr-xr-x   0 nicka    (10001) Domain Users  (2513)        0 2022-12-17 05:24:17.615366 djangocms-rawhtml-1.2.1/djangocms_rawhtml/templates/djangocms_rawhtml/plugins/
--rw-r--r--   0 nicka    (10001) Domain Users  (2513)       64 2020-12-23 07:31:40.000000 djangocms-rawhtml-1.2.1/djangocms_rawhtml/templates/djangocms_rawhtml/plugins/raw.html
-drwxr-xr-x   0 nicka    (10001) Domain Users  (2513)        0 2022-12-17 05:24:17.599366 djangocms-rawhtml-1.2.1/djangocms_rawhtml.egg-info/
--rw-r--r--   0 nicka    (10001) Domain Users  (2513)     2693 2022-12-17 05:24:17.000000 djangocms-rawhtml-1.2.1/djangocms_rawhtml.egg-info/PKG-INFO
--rw-r--r--   0 nicka    (10001) Domain Users  (2513)      578 2022-12-17 05:24:17.000000 djangocms-rawhtml-1.2.1/djangocms_rawhtml.egg-info/SOURCES.txt
--rw-r--r--   0 nicka    (10001) Domain Users  (2513)        1 2022-12-17 05:24:17.000000 djangocms-rawhtml-1.2.1/djangocms_rawhtml.egg-info/dependency_links.txt
--rw-r--r--   0 nicka    (10001) Domain Users  (2513)       18 2022-12-17 05:24:17.000000 djangocms-rawhtml-1.2.1/djangocms_rawhtml.egg-info/top_level.txt
--rw-r--r--   0 nicka    (10001) Domain Users  (2513)       38 2022-12-17 05:24:17.623367 djangocms-rawhtml-1.2.1/setup.cfg
--rw-r--r--   0 nicka    (10001) Domain Users  (2513)     1594 2022-12-17 05:09:13.000000 djangocms-rawhtml-1.2.1/setup.py
+drwxr-xr-x   0 nicka    (10001) Domain Users  (2513)        0 2023-07-01 09:28:36.940873 djangocms-rawhtml-1.3.0/
+-rw-r--r--   0 nicka    (10001) Domain Users  (2513)     1532 2023-07-01 09:21:06.000000 djangocms-rawhtml-1.3.0/LICENSE
+-rw-r--r--   0 nicka    (10001) Domain Users  (2513)       87 2020-12-23 07:31:40.000000 djangocms-rawhtml-1.3.0/MANIFEST.in
+-rw-r--r--   0 nicka    (10001) Domain Users  (2513)     2963 2023-07-01 09:28:36.940873 djangocms-rawhtml-1.3.0/PKG-INFO
+-rw-r--r--   0 nicka    (10001) Domain Users  (2513)     1254 2023-07-01 08:55:38.000000 djangocms-rawhtml-1.3.0/README.rst
+drwxr-xr-x   0 nicka    (10001) Domain Users  (2513)        0 2023-07-01 09:28:36.940873 djangocms-rawhtml-1.3.0/djangocms_rawhtml/
+-rw-r--r--   0 nicka    (10001) Domain Users  (2513)        0 2020-12-23 07:31:40.000000 djangocms-rawhtml-1.3.0/djangocms_rawhtml/__init__.py
+-rw-r--r--   0 nicka    (10001) Domain Users  (2513)     1228 2023-07-01 00:27:41.000000 djangocms-rawhtml-1.3.0/djangocms_rawhtml/cms_plugins.py
+drwxr-xr-x   0 nicka    (10001) Domain Users  (2513)        0 2023-07-01 09:28:36.940873 djangocms-rawhtml-1.3.0/djangocms_rawhtml/migrations/
+-rw-r--r--   0 nicka    (10001) Domain Users  (2513)      925 2020-12-23 07:31:40.000000 djangocms-rawhtml-1.3.0/djangocms_rawhtml/migrations/0001_rawhtmlplugindata.py
+-rw-r--r--   0 nicka    (10001) Domain Users  (2513)      586 2022-12-17 05:01:13.000000 djangocms-rawhtml-1.3.0/djangocms_rawhtml/migrations/0002_auto_20221216_1029.py
+-rw-r--r--   0 nicka    (10001) Domain Users  (2513)      783 2023-07-01 09:07:10.000000 djangocms-rawhtml-1.3.0/djangocms_rawhtml/migrations/0003_alter_rawhtmlplugindata_cmsplugin_ptr.py
+-rw-r--r--   0 nicka    (10001) Domain Users  (2513)        0 2020-12-23 07:31:40.000000 djangocms-rawhtml-1.3.0/djangocms_rawhtml/migrations/__init__.py
+-rw-r--r--   0 nicka    (10001) Domain Users  (2513)      675 2023-07-01 09:08:06.000000 djangocms-rawhtml-1.3.0/djangocms_rawhtml/models.py
+drwxr-xr-x   0 nicka    (10001) Domain Users  (2513)        0 2023-07-01 09:28:36.940873 djangocms-rawhtml-1.3.0/djangocms_rawhtml/templates/
+drwxr-xr-x   0 nicka    (10001) Domain Users  (2513)        0 2023-07-01 09:28:36.940873 djangocms-rawhtml-1.3.0/djangocms_rawhtml/templates/admin/
+drwxr-xr-x   0 nicka    (10001) Domain Users  (2513)        0 2023-07-01 09:28:36.940873 djangocms-rawhtml-1.3.0/djangocms_rawhtml/templates/admin/djangocms_rawhtml/
+-rw-r--r--   0 nicka    (10001) Domain Users  (2513)     1360 2021-02-28 02:26:11.000000 djangocms-rawhtml-1.3.0/djangocms_rawhtml/templates/admin/djangocms_rawhtml/change_form.html
+drwxr-xr-x   0 nicka    (10001) Domain Users  (2513)        0 2023-07-01 09:28:36.940873 djangocms-rawhtml-1.3.0/djangocms_rawhtml/templates/djangocms_rawhtml/
+drwxr-xr-x   0 nicka    (10001) Domain Users  (2513)        0 2023-07-01 09:28:36.940873 djangocms-rawhtml-1.3.0/djangocms_rawhtml/templates/djangocms_rawhtml/plugins/
+-rw-r--r--   0 nicka    (10001) Domain Users  (2513)       64 2020-12-23 07:31:40.000000 djangocms-rawhtml-1.3.0/djangocms_rawhtml/templates/djangocms_rawhtml/plugins/raw.html
+drwxr-xr-x   0 nicka    (10001) Domain Users  (2513)        0 2023-07-01 09:28:36.940873 djangocms-rawhtml-1.3.0/djangocms_rawhtml.egg-info/
+-rw-r--r--   0 nicka    (10001) Domain Users  (2513)     2963 2023-07-01 09:28:36.000000 djangocms-rawhtml-1.3.0/djangocms_rawhtml.egg-info/PKG-INFO
+-rw-r--r--   0 nicka    (10001) Domain Users  (2513)      653 2023-07-01 09:28:36.000000 djangocms-rawhtml-1.3.0/djangocms_rawhtml.egg-info/SOURCES.txt
+-rw-r--r--   0 nicka    (10001) Domain Users  (2513)        1 2023-07-01 09:28:36.000000 djangocms-rawhtml-1.3.0/djangocms_rawhtml.egg-info/dependency_links.txt
+-rw-r--r--   0 nicka    (10001) Domain Users  (2513)       18 2023-07-01 09:28:36.000000 djangocms-rawhtml-1.3.0/djangocms_rawhtml.egg-info/top_level.txt
+-rw-r--r--   0 nicka    (10001) Domain Users  (2513)       38 2023-07-01 09:28:36.940873 djangocms-rawhtml-1.3.0/setup.cfg
+-rw-r--r--   0 nicka    (10001) Domain Users  (2513)     1876 2023-07-01 09:26:33.000000 djangocms-rawhtml-1.3.0/setup.py
```

### Comparing `djangocms-rawhtml-1.2.1/LICENSE` & `djangocms-rawhtml-1.3.0/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2017, Nick Avgerinos, Axcella, LLC
+Copyright (c) 2017-2023, Nick Avgerinos, axcella.com
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `djangocms-rawhtml-1.2.1/README.rst` & `djangocms-rawhtml-1.3.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,33 +9,27 @@
 with `code-editor-django-admin <https://mr-coffee.net/blog/code-editor-django-admin>`_ by giving 
 you a nice HTML editor `CodeMirror <http://codemirror.net/>`_ to edit the code in rather than 
 a default ``TextField``.
 
 Installation
 ------------
 
-1. Install via pip:
-
-::
+1. Install via pip::
 
     pip install djangocms-rawhtml
 
-2. Add to your ``INSTALLED_APPS`` (in ``settings.py``):
-
-::
+2. Add to your ``INSTALLED_APPS`` (in ``settings.py``)::
 
     INSTALLED_APPS = (
         ...
         'djangocms_rawhtml',
         ...
     )
 
-3. Run migrations:
-
-::
+3. Run migrations::
 
     python manage.py migrate djangocms_rawhtml
 
 4. "Raw HTML" should now be available as a plugin in the CMS!
 
 
 Configuration
```

### Comparing `djangocms-rawhtml-1.2.1/djangocms_rawhtml/cms_plugins.py` & `djangocms-rawhtml-1.3.0/djangocms_rawhtml/cms_plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from cms.plugin_base import CMSPluginBase
 from cms.plugin_pool import plugin_pool
 from django.conf import settings
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from djangocms_rawhtml.models import RawHTMLPluginData
 
 @plugin_pool.register_plugin
 class RawHTMLPluginPublisher(CMSPluginBase):
     """
     Plugin to manage raw HTML text that needs to be managed from the admin interface.
     """
```

### Comparing `djangocms-rawhtml-1.2.1/djangocms_rawhtml/migrations/0001_rawhtmlplugindata.py` & `djangocms-rawhtml-1.3.0/djangocms_rawhtml/migrations/0001_rawhtmlplugindata.py`

 * *Files identical despite different names*

### Comparing `djangocms-rawhtml-1.2.1/djangocms_rawhtml/migrations/0002_auto_20221216_1029.py` & `djangocms-rawhtml-1.3.0/djangocms_rawhtml/migrations/0002_auto_20221216_1029.py`

 * *Files identical despite different names*

### Comparing `djangocms-rawhtml-1.2.1/djangocms_rawhtml/models.py` & `djangocms-rawhtml-1.3.0/djangocms_rawhtml/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from django.db import models
-from six import python_2_unicode_compatible
 from cms.models.pluginmodel import CMSPlugin
 from django.utils.text import Truncator
 from django.utils.html import strip_tags
 
 
-@python_2_unicode_compatible
 class RawHTMLPluginData(CMSPlugin):
     """
     Model for Raw HTML Plugin
     
     body - contains the HTML source text
     label - used for display purposes on the admin site
     """
```

### Comparing `djangocms-rawhtml-1.2.1/djangocms_rawhtml/templates/admin/djangocms_rawhtml/change_form.html` & `djangocms-rawhtml-1.3.0/djangocms_rawhtml/templates/admin/djangocms_rawhtml/change_form.html`

 * *Files identical despite different names*

### Comparing `djangocms-rawhtml-1.2.1/djangocms_rawhtml.egg-info/SOURCES.txt` & `djangocms-rawhtml-1.3.0/djangocms_rawhtml.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -7,10 +7,11 @@
 djangocms_rawhtml/models.py
 djangocms_rawhtml.egg-info/PKG-INFO
 djangocms_rawhtml.egg-info/SOURCES.txt
 djangocms_rawhtml.egg-info/dependency_links.txt
 djangocms_rawhtml.egg-info/top_level.txt
 djangocms_rawhtml/migrations/0001_rawhtmlplugindata.py
 djangocms_rawhtml/migrations/0002_auto_20221216_1029.py
+djangocms_rawhtml/migrations/0003_alter_rawhtmlplugindata_cmsplugin_ptr.py
 djangocms_rawhtml/migrations/__init__.py
 djangocms_rawhtml/templates/admin/djangocms_rawhtml/change_form.html
 djangocms_rawhtml/templates/djangocms_rawhtml/plugins/raw.html
```

