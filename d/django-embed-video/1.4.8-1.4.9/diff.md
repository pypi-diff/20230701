# Comparing `tmp/django-embed-video-1.4.8.tar.gz` & `tmp/django-embed-video-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-embed-video-1.4.8.tar", last modified: Sat Nov 19 11:05:17 2022, max compression
+gzip compressed data, was "django-embed-video-1.4.9.tar", last modified: Sat Jul  1 14:24:54 2023, max compression
```

## Comparing `django-embed-video-1.4.8.tar` & `django-embed-video-1.4.9.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.399021 django-embed-video-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.383021 django-embed-video-1.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.387021 django-embed-video-1.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2141 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     8050 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2375 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11970 2022-11-19 11:05:17.399021 django-embed-video-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2729 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.391021 django-embed-video-1.4.8/django_embed_video.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11970 2022-11-19 11:05:17.000000 django-embed-video-1.4.8/django_embed_video.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2729 2022-11-19 11:05:17.000000 django-embed-video-1.4.8/django_embed_video.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-19 11:05:17.000000 django-embed-video-1.4.8/django_embed_video.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-19 11:05:17.000000 django-embed-video-1.4.8/django_embed_video.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-19 11:05:17.000000 django-embed-video-1.4.8/django_embed_video.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.391021 django-embed-video-1.4.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     6809 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.391021 django-embed-video-1.4.8/docs/api/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/api/embed_video.admin.rst
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/api/embed_video.backends.rst
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/api/embed_video.fields.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/api/embed_video.settings.rst
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/api/embed_video.template_tags.rst
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/api/embed_video.utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9296 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.391021 django-embed-video-1.4.8/docs/development/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/development/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/development/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/development/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/development/testing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/example-project.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3910 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.391021 django-embed-video-1.4.8/docs/ext/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7381 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/ext/djangodocs.py
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6725 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/docs/websites.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.395021 django-embed-video-1.4.8/embed_video/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2501 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)    11224 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/backends.py
--rw-r--r--   0 runner    (1001) docker     (121)     1424 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.383021 django-embed-video-1.4.8/embed_video/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.383021 django-embed-video-1.4.8/embed_video/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.395021 django-embed-video-1.4.8/embed_video/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.387021 django-embed-video-1.4.8/embed_video/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.395021 django-embed-video-1.4.8/embed_video/templates/embed_video/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/templates/embed_video/embed_code.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.395021 django-embed-video-1.4.8/embed_video/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7774 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/templatetags/embed_video_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.395021 django-embed-video-1.4.8/embed_video/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.395021 django-embed-video-1.4.8/embed_video/tests/backends/
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/tests/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/tests/backends/tests_custom_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     2134 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/tests/backends/tests_soundcloud.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/tests/backends/tests_videobackend.py
--rw-r--r--   0 runner    (1001) docker     (121)     1685 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/tests/backends/tests_vimeo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2985 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/tests/backends/tests_youtube.py
--rw-r--r--   0 runner    (1001) docker     (121)     1348 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/tests/django_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.395021 django-embed-video-1.4.8/embed_video/tests/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/tests/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11742 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/tests/templatetags/tests_embed_video_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)     2465 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/tests/tests_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/embed_video/tests/tests_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.395021 django-embed-video-1.4.8/example_project/
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.395021 django-embed-video-1.4.8/example_project/example_project/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/example_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.395021 django-embed-video-1.4.8/example_project/example_project/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/example_project/fixtures/initial_data.yaml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/example_project/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/example_project/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.399021 django-embed-video-1.4.8/example_project/example_project/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/example_project/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/example_project/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/example_project/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      258 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.399021 django-embed-video-1.4.8/example_project/posts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/posts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/posts/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.399021 django-embed-video-1.4.8/example_project/posts/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)     1390 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/posts/fixtures/initial_data.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.399021 django-embed-video-1.4.8/example_project/posts/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/posts/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/posts/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/posts/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.387021 django-embed-video-1.4.8/example_project/posts/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 11:05:17.399021 django-embed-video-1.4.8/example_project/posts/templates/posts/
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/posts/templates/posts/post_detail.html
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/posts/templates/posts/post_list.html
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/posts/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/posts/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/posts/views.py
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/example_project/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-19 11:05:17.399021 django-embed-video-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1728 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-11-19 11:04:58.000000 django-embed-video-1.4.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.226327 django-embed-video-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.198326 django-embed-video-1.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.206326 django-embed-video-1.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-07-01 14:24:54.226327 django-embed-video-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.210327 django-embed-video-1.4.9/django_embed_video.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-07-01 14:24:54.000000 django-embed-video-1.4.9/django_embed_video.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-01 14:24:54.000000 django-embed-video-1.4.9/django_embed_video.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 14:24:54.000000 django-embed-video-1.4.9/django_embed_video.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-01 14:24:54.000000 django-embed-video-1.4.9/django_embed_video.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-01 14:24:54.000000 django-embed-video-1.4.9/django_embed_video.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.210327 django-embed-video-1.4.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.214326 django-embed-video-1.4.9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/api/embed_video.admin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/api/embed_video.backends.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/api/embed_video.fields.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/api/embed_video.settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/api/embed_video.template_tags.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/api/embed_video.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.214326 django-embed-video-1.4.9/docs/development/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/development/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/development/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/development/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/development/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/example-project.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.214326 django-embed-video-1.4.9/docs/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/ext/djangodocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/docs/websites.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.214326 django-embed-video-1.4.9/embed_video/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.202326 django-embed-video-1.4.9/embed_video/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.202326 django-embed-video-1.4.9/embed_video/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.214326 django-embed-video-1.4.9/embed_video/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.202326 django-embed-video-1.4.9/embed_video/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.214326 django-embed-video-1.4.9/embed_video/templates/embed_video/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/templates/embed_video/embed_code.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.214326 django-embed-video-1.4.9/embed_video/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/templatetags/embed_video_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.218326 django-embed-video-1.4.9/embed_video/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.218326 django-embed-video-1.4.9/embed_video/tests/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/tests/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/tests/backends/tests_custom_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/tests/backends/tests_soundcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/tests/backends/tests_videobackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/tests/backends/tests_vimeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/tests/backends/tests_youtube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/tests/django_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.218326 django-embed-video-1.4.9/embed_video/tests/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/tests/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13202 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/tests/templatetags/tests_embed_video_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/tests/tests_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/embed_video/tests/tests_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.218326 django-embed-video-1.4.9/example_project/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.222326 django-embed-video-1.4.9/example_project/example_project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/example_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.222326 django-embed-video-1.4.9/example_project/example_project/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/example_project/fixtures/initial_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/example_project/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/example_project/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.222326 django-embed-video-1.4.9/example_project/example_project/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/example_project/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/example_project/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/example_project/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      258 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.222326 django-embed-video-1.4.9/example_project/posts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/posts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/posts/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.222326 django-embed-video-1.4.9/example_project/posts/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/posts/fixtures/initial_data.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.222326 django-embed-video-1.4.9/example_project/posts/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/posts/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/posts/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/posts/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.202326 django-embed-video-1.4.9/example_project/posts/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:54.222326 django-embed-video-1.4.9/example_project/posts/templates/posts/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/posts/templates/posts/post_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/posts/templates/posts/post_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/posts/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/posts/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/posts/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/example_project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 14:24:54.226327 django-embed-video-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-01 14:24:35.000000 django-embed-video-1.4.9/tox.ini
```

### Comparing `django-embed-video-1.4.8/.github/workflows/release.yml` & `django-embed-video-1.4.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/CHANGES.rst` & `django-embed-video-1.4.9/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 
 Changes
 =======
 
 
+Release 1.4.9 (July 1, 2023)
+----------------------------
+
+- Update Python and Django versions.
+- Fix Soundcloud tests.
+- Add example sites.
+
+
 Release 1.4.8 (November 19, 2022)
 ---------------------------------
 
 - Fixes in migrations and documentation.
 
 
 Release 1.4.7 (September 28, 2022)
```

### Comparing `django-embed-video-1.4.8/CODE_OF_CONDUCT.md` & `django-embed-video-1.4.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/LICENSE` & `django-embed-video-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/PKG-INFO` & `django-embed-video-1.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: django-embed-video
-Version: 1.4.8
+Version: 1.4.9
 Summary: Django app for easy embedding YouTube and Vimeo videos and music from SoundCloud.
 Home-page: https://github.com/jazzband/django-embed-video
 Author: Cedric Carrard
 Author-email: cedric.carrard@gmail.com
 Keywords: youtube,vimeo,video,soundcloud
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Environment :: Plugins
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP
 License-File: LICENSE
 
 django-embed-video
 ==================
 
 Django app for easy embedding YouTube and Vimeo videos and music from SoundCloud.
@@ -128,14 +127,22 @@
 and follow the `guidelines <https://jazzband.co/about/guidelines>`_.
 
 
 Changes
 =======
 
 
+Release 1.4.9 (July 1, 2023)
+----------------------------
+
+- Update Python and Django versions.
+- Fix Soundcloud tests.
+- Add example sites.
+
+
 Release 1.4.8 (November 19, 2022)
 ---------------------------------
 
 - Fixes in migrations and documentation.
 
 
 Release 1.4.7 (September 28, 2022)
```

### Comparing `django-embed-video-1.4.8/README.rst` & `django-embed-video-1.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/django_embed_video.egg-info/PKG-INFO` & `django-embed-video-1.4.9/django_embed_video.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: django-embed-video
-Version: 1.4.8
+Version: 1.4.9
 Summary: Django app for easy embedding YouTube and Vimeo videos and music from SoundCloud.
 Home-page: https://github.com/jazzband/django-embed-video
 Author: Cedric Carrard
 Author-email: cedric.carrard@gmail.com
 Keywords: youtube,vimeo,video,soundcloud
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Environment :: Plugins
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP
 License-File: LICENSE
 
 django-embed-video
 ==================
 
 Django app for easy embedding YouTube and Vimeo videos and music from SoundCloud.
@@ -128,14 +127,22 @@
 and follow the `guidelines <https://jazzband.co/about/guidelines>`_.
 
 
 Changes
 =======
 
 
+Release 1.4.9 (July 1, 2023)
+----------------------------
+
+- Update Python and Django versions.
+- Fix Soundcloud tests.
+- Add example sites.
+
+
 Release 1.4.8 (November 19, 2022)
 ---------------------------------
 
 - Fixes in migrations and documentation.
 
 
 Release 1.4.7 (September 28, 2022)
```

### Comparing `django-embed-video-1.4.8/django_embed_video.egg-info/SOURCES.txt` & `django-embed-video-1.4.9/django_embed_video.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/docs/Makefile` & `django-embed-video-1.4.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/docs/api/embed_video.settings.rst` & `django-embed-video-1.4.9/docs/api/embed_video.settings.rst`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/docs/conf.py` & `django-embed-video-1.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/docs/examples.rst` & `django-embed-video-1.4.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/docs/ext/djangodocs.py` & `django-embed-video-1.4.9/docs/ext/djangodocs.py`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/docs/index.rst` & `django-embed-video-1.4.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/docs/make.bat` & `django-embed-video-1.4.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/embed_video/admin.py` & `django-embed-video-1.4.9/embed_video/admin.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django import forms
-from django.core.validators import URLValidator
 from django.core.exceptions import ValidationError
+from django.core.validators import URLValidator
 from django.utils.safestring import mark_safe
 
 from embed_video.backends import (
     UnknownBackendException,
     VideoDoesntExistException,
     detect_backend,
 )
```

### Comparing `django-embed-video-1.4.8/embed_video/backends.py` & `django-embed-video-1.4.9/embed_video/backends.py`

 * *Files 1% similar despite different names*

```diff
@@ -427,15 +427,18 @@
             self.base_url.format(protocol=self.protocol),
             params=params,
             timeout=EMBED_VIDEO_TIMEOUT,
         )
 
         if r.status_code != 200:
             raise VideoDoesntExistException(
-                "SoundCloud returned status code `{0}`.".format(r.status_code)
+                "SoundCloud returned status code `{status_code}` for URL `{url}`.".format(
+                    status_code=r.status_code,
+                    url=r.url,
+                )
             )
 
         return json.loads(r.text)
 
     def get_thumbnail_url(self):
         return self.info.get("thumbnail_url")
```

### Comparing `django-embed-video-1.4.8/embed_video/fields.py` & `django-embed-video-1.4.9/embed_video/fields.py`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/embed_video/locale/pl/LC_MESSAGES/django.mo` & `django-embed-video-1.4.9/embed_video/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/embed_video/locale/pl/LC_MESSAGES/django.po` & `django-embed-video-1.4.9/embed_video/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/embed_video/settings.py` & `django-embed-video-1.4.9/embed_video/settings.py`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/embed_video/templatetags/embed_video_tags.py` & `django-embed-video-1.4.9/embed_video/templatetags/embed_video_tags.py`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/embed_video/tests/backends/tests_custom_backend.py` & `django-embed-video-1.4.9/embed_video/tests/backends/tests_custom_backend.py`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/embed_video/tests/backends/tests_videobackend.py` & `django-embed-video-1.4.9/embed_video/tests/backends/tests_videobackend.py`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/embed_video/tests/backends/tests_youtube.py` & `django-embed-video-1.4.9/embed_video/tests/backends/tests_youtube.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from unittest import TestCase
 from unittest.mock import patch
 
-from embed_video.backends import UnknownIdException, YoutubeBackend
-from embed_video.tests.backends import BackendTestMixin
+from embed_video.backends import UnknownIdException, YoutubeBackend, detect_backend
 
 
-class YoutubeBackendTestCase(BackendTestMixin, TestCase):
+class YoutubeBackendTestCase(TestCase):
     urls = (
         ("http://youtu.be/jsrRJyHBvzw", "jsrRJyHBvzw"),
         ("http://youtu.be/n17B_uFF4cA", "n17B_uFF4cA"),
         ("http://youtu.be/t-ZRX8984sc", "t-ZRX8984sc"),
         ("https://youtu.be/t-ZRX8984sc", "t-ZRX8984sc"),
         ("http://youtube.com/watch?v=jsrRJyHBvzw", "jsrRJyHBvzw"),
         ("https://youtube.com/watch?v=jsrRJyHBvzw", "jsrRJyHBvzw"),
@@ -41,14 +40,24 @@
         ("https://m.youtube.com/watch?v=IAooXLAPoBQ", "IAooXLAPoBQ"),
         ("https://www.youtube.com/shorts/cOoQ7pc0CoY", "cOoQ7pc0CoY"),
         ("https://youtube.com/shorts/cOoQ7pc0CoY", "cOoQ7pc0CoY"),
     )
 
     instance = YoutubeBackend
 
+    def test_detect(self):
+        for url in self.urls:
+            backend = detect_backend(url[0])
+            self.assertIsInstance(backend, self.instance)
+
+    def test_code(self):
+        for url in self.urls:
+            backend = self.instance(url[0])
+            self.assertEqual(backend.code, url[1])
+
     def test_youtube_keyerror(self):
         """Test for issue #7"""
         backend = self.instance("http://youtube.com/watch?id=5")
         self.assertRaises(UnknownIdException, backend.get_code)
 
     def test_thumbnail(self):
         for url in self.urls:
```

### Comparing `django-embed-video-1.4.8/embed_video/tests/django_settings.py` & `django-embed-video-1.4.9/embed_video/tests/django_settings.py`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/embed_video/tests/templatetags/tests_embed_video_tags.py` & `django-embed-video-1.4.9/embed_video/tests/templatetags/tests_embed_video_tags.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import re
 import urllib.parse as urlparse
+from json import dumps
 from unittest import TestCase
 from unittest.mock import Mock, patch
 
+import requests_mock
 from django.http import HttpRequest
 from django.template import TemplateSyntaxError
 from django.template.base import Template
 from django.template.context import RequestContext
 from django.test.client import RequestFactory
 
 from embed_video.templatetags.embed_video_tags import VideoNode
@@ -167,19 +169,45 @@
     def test_tag_soundcloud(self):
         template = """
             {% load embed_video_tags %}
             {% video 'https://soundcloud.com/community/soundcloud-case-study-wildlife' as soundcloud %}
                 {{ soundcloud.url }} {{ soundcloud.backend }}
             {% endvideo %}
         """
-        self.assertRenderedTemplate(
-            template,
-            "https://w.soundcloud.com/player/?visual=true&amp;url=https%3A%2F%2Fapi.soundcloud.com%2Ftracks%2F82244706&amp;show_artwork=true "
-            "SoundCloudBackend",
-        )
+
+        # Soundcloud backend generates the following embed URL and fetches the payload from it
+        # you can check the URL contents and update it as needed
+        url = "https://soundcloud.com/oembed?format=json&url=https%3A%2F%2Fsoundcloud.com%2Fcommunity%2Fsoundcloud-case-study-wildlife"
+        response = dumps(
+            {
+                "version": 1.0,
+                "type": "rich",
+                "provider_name": "SoundCloud",
+                "provider_url": "https://soundcloud.com",
+                "height": 400,
+                "width": "100%",
+                "title": "SoundCloud Case Study: Wildlife Control by SoundCloud Community",
+                "description": "Listen to how Wildlife Control makes the most of the SoundCloud platform, and it's API.",
+                "thumbnail_url": "https://i1.sndcdn.com/artworks-000042390403-ouou1g-t500x500.jpg",
+                "html": "<iframe "
+                'width="100%" height="400" scrolling="no" frameborder="no" '
+                'src="https://w.soundcloud.com/player/?visual=true&url=https%3A%2F%2Fapi.soundcloud.com%2Ftracks%2F82244706&show_artwork=true"'
+                "></iframe>",
+                "author_name": "SoundCloud Community",
+                "author_url": "https://soundcloud.com/community",
+            }
+        )
+
+        with requests_mock.Mocker() as m:
+            m.get(url, text=response)
+            self.assertRenderedTemplate(
+                template,
+                "https://w.soundcloud.com/player/?visual=true&amp;url=https%3A%2F%2Fapi.soundcloud.com%2Ftracks%2F82244706&amp;show_artwork=true "
+                "SoundCloudBackend",
+            )
 
     @patch("embed_video.backends.EMBED_VIDEO_TIMEOUT", 0.000001)
     @patch("urllib3.connectionpool.log")
     @patch("embed_video.templatetags.embed_video_tags.logger")
     def test_empty_if_timeout(self, embed_video_logger, urllib_logger):
         template = """
             {% load embed_video_tags %}
```

### Comparing `django-embed-video-1.4.8/embed_video/tests/tests_admin.py` & `django-embed-video-1.4.9/embed_video/tests/tests_admin.py`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/embed_video/tests/tests_fields.py` & `django-embed-video-1.4.9/embed_video/tests/tests_fields.py`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/example_project/README.rst` & `django-embed-video-1.4.9/example_project/README.rst`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/example_project/example_project/settings.py` & `django-embed-video-1.4.9/example_project/example_project/settings.py`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/example_project/example_project/templates/base.html` & `django-embed-video-1.4.9/example_project/example_project/templates/base.html`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/example_project/example_project/wsgi.py` & `django-embed-video-1.4.9/example_project/example_project/wsgi.py`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/example_project/posts/fixtures/initial_data.yaml` & `django-embed-video-1.4.9/example_project/posts/fixtures/initial_data.yaml`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/example_project/posts/migrations/0001_initial.py` & `django-embed-video-1.4.9/example_project/posts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/example_project/posts/templates/posts/post_detail.html` & `django-embed-video-1.4.9/example_project/posts/templates/posts/post_detail.html`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/example_project/posts/templates/posts/post_list.html` & `django-embed-video-1.4.9/example_project/posts/templates/posts/post_list.html`

 * *Files identical despite different names*

### Comparing `django-embed-video-1.4.8/setup.py` & `django-embed-video-1.4.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,26 +19,25 @@
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Environment :: Plugins",
         "Framework :: Django",
         "Framework :: Django :: 3.2",
-        "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Internet :: WWW/HTTP",
     ],
     keywords=["youtube", "vimeo", "video", "soundcloud"],
-    install_requires=["requests >= 2.19", "Django >= 2.2"],
+    install_requires=["requests >= 2.19", "Django >= 3.2"],
     setup_requires=["readme", "setuptools_scm"],
     tests_require=["Django", "requests >= 2.19", "coverage"],
 )
```

### Comparing `django-embed-video-1.4.8/tox.ini` & `django-embed-video-1.4.9/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,58 @@
 [tox]
 envlist =
-    py{37,38,39,310,py3}-dj32
-    py{38,39,310,py3}-dj40
-    py{38,39,310,py3}-dj41
-    py{38,39,310}-djmain
-    py310-djqa
+    py{37,38,39,310}-dj32
+    py{38,39,310}-dj40
+    py{38,39,310,py311}-dj41
+    py{38,39,310,py311}-dj42
+    py{311}-djmain
+    py{311}-djqa
 
 [gh-actions]
 python =
     3.7: py37
     3.8: py38
     3.9: py39
     3.10: py310
-    pypy3: pypy3
+    3.11: py311
 
 [gh-actions:env]
 DJANGO =
     3.2: dj32
     4.0: dj40
     4.1: dj41
+    4.2: dj42
     main: djmain
     qa: djqa
 
 [testenv]
 deps =
     dj32: django>=3.2,<3.3
     dj40: django>=4.0,<4.1
     dj41: django>=4.1,<4.2
+    dj42: django>=4.2,<4.3
     djmain: https://github.com/django/django/archive/main.tar.gz
     coverage
+    requests-mock
 usedevelop = True
 commands =
     coverage run -m django test --settings=embed_video.tests.django_settings
     coverage report
     coverage xml
 setenv =
     PYTHONDONTWRITEBYTECODE=1
 # Django development version is allowed to fail the test matrix
 ignore_outcome =
     djmain: True
 ignore_errors =
     djmain: True
 
-[testenv:py310-djqa]
+[testenv:py311-djqa]
 ignore_errors = true
-basepython = python3.10
+basepython = 3.11
 deps =
     black==22.6.0
     isort==5.6.4
 skip_install = true
 commands =
     isort --profile black --check-only --diff embed_video setup.py
     black -t py38 --check --diff embed_video
```

