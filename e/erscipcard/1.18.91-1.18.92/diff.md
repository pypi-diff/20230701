# Comparing `tmp/erscipcard-1.18.91.tar.gz` & `tmp/erscipcard-1.18.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erscipcard-1.18.91.tar", last modified: Thu Jun  8 20:16:53 2023, max compression
+gzip compressed data, was "erscipcard-1.18.92.tar", last modified: Sat Jul  1 05:20:19 2023, max compression
```

## Comparing `erscipcard-1.18.91.tar` & `erscipcard-1.18.92.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:16:53.457708 erscipcard-1.18.91/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-06-08 20:16:46.000000 erscipcard-1.18.91/LICENSE
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-08 20:16:46.000000 erscipcard-1.18.91/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1692 2023-06-08 20:16:53.457708 erscipcard-1.18.91/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1398 2023-06-08 20:16:46.000000 erscipcard-1.18.91/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:16:53.446708 erscipcard-1.18.91/erscipcard/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/__init__.py
--rw-r--r--   0 root         (0) root         (0)       87 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/admin.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/apps.py
--rw-r--r--   0 root         (0) root         (0)      714 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/forms.py
--rw-r--r--   0 root         (0) root         (0)     1939 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/inst.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:16:53.447708 erscipcard-1.18.91/erscipcard/migrations/
--rw-r--r--   0 root         (0) root         (0)     2100 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2107 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:16:53.449707 erscipcard-1.18.91/erscipcard/static/
--rw-r--r--   0 root         (0) root         (0)    11041 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/1.docx
--rw-r--r--   0 root         (0) root         (0)    11792 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/2.docx
--rw-r--r--   0 root         (0) root         (0)    60820 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/BNAZANIN.TTF
--rw-r--r--   0 root         (0) root         (0)    61268 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/BTITR.TTF
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:16:53.443708 erscipcard-1.18.91/erscipcard/static/bt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:16:53.450708 erscipcard-1.18.91/erscipcard/static/bt/css/
--rw-r--r--   0 root         (0) root         (0)   175814 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/bt/css/bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)    31000 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/bt/css/font-awesome.min.css
--rw-r--r--   0 root         (0) root         (0)     9182 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/bt/css/loginstyle.css
--rw-r--r--   0 root         (0) root         (0)     3804 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/bt/css/persianDatepicker-default.css
--rw-r--r--   0 root         (0) root         (0)     5557 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/bt/css/style.css
--rw-r--r--   0 root         (0) root         (0)    83821 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/bt/css/util.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:16:53.451707 erscipcard-1.18.91/erscipcard/static/bt/fonts/
--rw-r--r--   0 root         (0) root         (0)    60820 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/bt/fonts/BNAZANIN.TTF
--rw-r--r--   0 root         (0) root         (0)    61268 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/bt/fonts/BTITR.TTF
--rw-r--r--   0 root         (0) root         (0)    84624 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/bt/fonts/Vazir.ttf
--rw-r--r--   0 root         (0) root         (0)   165548 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/bt/fonts/fontawesome-webfont.ttf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:16:53.452707 erscipcard-1.18.91/erscipcard/static/bt/js/
--rw-r--r--   0 root         (0) root         (0)    78694 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/bt/js/bootstrap.bundle.min.js
--rw-r--r--   0 root         (0) root         (0)    88145 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/bt/js/jquery.min.js
--rw-r--r--   0 root         (0) root         (0)    29875 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/bt/js/persianDatepicker.js
--rw-r--r--   0 root         (0) root         (0)     1728 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/bt/js/scripts.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:16:53.452707 erscipcard-1.18.91/erscipcard/static/bt/pics/
--rw-r--r--   0 root         (0) root         (0)    29117 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/bt/pics/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    35195 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/bt/pics/logo.png
--rw-r--r--   0 root         (0) root         (0)     4929 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/custom_modelField_with_formField
--rw-r--r--   0 root         (0) root         (0)    19286 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/ersci_app.zip
--rw-r--r--   0 root         (0) root         (0)    12683 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/ersci_viddown_tab2-1.4.xpi
--rw-r--r--   0 root         (0) root         (0)    29117 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)      696 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/inst
--rw-r--r--   0 root         (0) root         (0)    35195 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/logo.png
--rw-r--r--   0 root         (0) root         (0)     1126 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/main.css
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/s
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:16:53.456708 erscipcard-1.18.91/erscipcard/static/spinner/
--rw-r--r--   0 root         (0) root         (0)     7573 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/atebits.css
--rw-r--r--   0 root         (0) root         (0)    14641 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/ball.css
--rw-r--r--   0 root         (0) root         (0)     1716 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/circles.css
--rw-r--r--   0 root         (0) root         (0)    11683 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/dots.css
--rw-r--r--   0 root         (0) root         (0)     2705 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/echo.css
--rw-r--r--   0 root         (0) root         (0)     3476 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/flower.css
--rw-r--r--   0 root         (0) root         (0)     6259 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/gauge.css
--rw-r--r--   0 root         (0) root         (0)     3523 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/heartbeat.css
--rw-r--r--   0 root         (0) root         (0)    17599 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/hexdots.css
--rw-r--r--   0 root         (0) root         (0)     1421 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/hole-pulse.css
--rw-r--r--   0 root         (0) root         (0)     2713 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/inner-circles.css
--rw-r--r--   0 root         (0) root         (0)     6223 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/plus-loader.css
--rw-r--r--   0 root         (0) root         (0)    18677 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/plus.css
--rw-r--r--   0 root         (0) root         (0)    12802 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/pong.css
--rw-r--r--   0 root         (0) root         (0)     1437 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/pulse.css
--rw-r--r--   0 root         (0) root         (0)     1532 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/refreshing.css
--rw-r--r--   0 root         (0) root         (0)     2105 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/spinner.css
--rw-r--r--   0 root         (0) root         (0)     4661 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/spinning-pixels.css
--rw-r--r--   0 root         (0) root         (0)     1257 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/three-quarters.css
--rw-r--r--   0 root         (0) root         (0)     1599 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/throbber.css
--rw-r--r--   0 root         (0) root         (0)     2220 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/timer.css
--rw-r--r--   0 root         (0) root         (0)    22371 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/whirly.css
--rw-r--r--   0 root         (0) root         (0)     3093 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinner/wobblebar.css
--rw-r--r--   0 root         (0) root         (0)   143659 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/spinners.css
--rw-r--r--   0 root         (0) root         (0)        2 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/static/ytvid.mp4
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:16:53.456708 erscipcard-1.18.91/erscipcard/templates/
--rw-r--r--   0 root         (0) root         (0)      241 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/templates/AvatarFileUploadInput.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:16:53.456708 erscipcard-1.18.91/erscipcard/templates/erscipcard/
--rw-r--r--   0 root         (0) root         (0)     2606 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/templates/erscipcard/login.html
--rw-r--r--   0 root         (0) root         (0)    12711 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/templates/erscipcard/ou.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:16:53.457708 erscipcard-1.18.91/erscipcard/templatetags/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/templatetags/__init__.py
--rw-r--r--   0 root         (0) root         (0)      143 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/templatetags/basepath.py
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/tests.py
--rw-r--r--   0 root         (0) root         (0)     1342 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/urls.py
--rw-r--r--   0 root         (0) root         (0)    12726 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/views.py
--rw-r--r--   0 root         (0) root         (0)     1202 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/widget.py
--rw-r--r--   0 root         (0) root         (0)      296 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/yturls.py
--rw-r--r--   0 root         (0) root         (0)     8838 2023-06-08 20:16:46.000000 erscipcard-1.18.91/erscipcard/ytviews.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:16:53.447708 erscipcard-1.18.91/erscipcard.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1692 2023-06-08 20:16:53.000000 erscipcard-1.18.91/erscipcard.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2704 2023-06-08 20:16:53.000000 erscipcard-1.18.91/erscipcard.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 20:16:53.000000 erscipcard-1.18.91/erscipcard.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       93 2023-06-08 20:16:53.000000 erscipcard-1.18.91/erscipcard.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-08 20:16:53.000000 erscipcard-1.18.91/erscipcard.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      780 2023-06-08 20:16:53.457708 erscipcard-1.18.91/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-08 20:16:46.000000 erscipcard-1.18.91/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 05:20:19.270719 erscipcard-1.18.92/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-07-01 05:20:03.000000 erscipcard-1.18.92/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      150 2023-07-01 05:20:03.000000 erscipcard-1.18.92/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-07-01 05:20:19.270719 erscipcard-1.18.92/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-07-01 05:20:03.000000 erscipcard-1.18.92/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 05:20:19.256718 erscipcard-1.18.92/erscipcard/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/admin.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/apps.py
+-rw-r--r--   0 root         (0) root         (0)      714 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/forms.py
+-rw-r--r--   0 root         (0) root         (0)     2074 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/inst.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 05:20:19.257718 erscipcard-1.18.92/erscipcard/migrations/
+-rw-r--r--   0 root         (0) root         (0)     2100 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 05:20:19.261718 erscipcard-1.18.92/erscipcard/static/
+-rw-r--r--   0 root         (0) root         (0)    11041 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/1.docx
+-rw-r--r--   0 root         (0) root         (0)    11792 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/2.docx
+-rw-r--r--   0 root         (0) root         (0)    60820 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/BNAZANIN.TTF
+-rw-r--r--   0 root         (0) root         (0)    61268 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/BTITR.TTF
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 05:20:19.252718 erscipcard-1.18.92/erscipcard/static/bt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 05:20:19.262719 erscipcard-1.18.92/erscipcard/static/bt/css/
+-rw-r--r--   0 root         (0) root         (0)   175814 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/bt/css/bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)    31000 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/bt/css/font-awesome.min.css
+-rw-r--r--   0 root         (0) root         (0)     9182 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/bt/css/loginstyle.css
+-rw-r--r--   0 root         (0) root         (0)     3804 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/bt/css/persianDatepicker-default.css
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/bt/css/style.css
+-rw-r--r--   0 root         (0) root         (0)    83821 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/bt/css/util.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 05:20:19.263718 erscipcard-1.18.92/erscipcard/static/bt/fonts/
+-rw-r--r--   0 root         (0) root         (0)    60820 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/bt/fonts/BNAZANIN.TTF
+-rw-r--r--   0 root         (0) root         (0)    61268 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/bt/fonts/BTITR.TTF
+-rw-r--r--   0 root         (0) root         (0)    84624 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/bt/fonts/Vazir.ttf
+-rw-r--r--   0 root         (0) root         (0)   165548 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/bt/fonts/fontawesome-webfont.ttf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 05:20:19.264719 erscipcard-1.18.92/erscipcard/static/bt/js/
+-rw-r--r--   0 root         (0) root         (0)    78694 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/bt/js/bootstrap.bundle.min.js
+-rw-r--r--   0 root         (0) root         (0)    88145 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/bt/js/jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)    29875 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/bt/js/persianDatepicker.js
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/bt/js/scripts.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 05:20:19.265719 erscipcard-1.18.92/erscipcard/static/bt/pics/
+-rw-r--r--   0 root         (0) root         (0)    29117 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/bt/pics/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    35195 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/bt/pics/logo.png
+-rw-r--r--   0 root         (0) root         (0)     4929 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/custom_modelField_with_formField
+-rw-r--r--   0 root         (0) root         (0)    19286 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/ersci_app.zip
+-rw-r--r--   0 root         (0) root         (0)    12683 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/ersci_viddown_tab2-1.4.xpi
+-rw-r--r--   0 root         (0) root         (0)    29117 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)      696 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/inst
+-rw-r--r--   0 root         (0) root         (0)    35195 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/logo.png
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/main.css
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/s
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 05:20:19.269719 erscipcard-1.18.92/erscipcard/static/spinner/
+-rw-r--r--   0 root         (0) root         (0)     7573 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/atebits.css
+-rw-r--r--   0 root         (0) root         (0)    14641 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/ball.css
+-rw-r--r--   0 root         (0) root         (0)     1716 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/circles.css
+-rw-r--r--   0 root         (0) root         (0)    11683 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/dots.css
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/echo.css
+-rw-r--r--   0 root         (0) root         (0)     3476 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/flower.css
+-rw-r--r--   0 root         (0) root         (0)     6259 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/gauge.css
+-rw-r--r--   0 root         (0) root         (0)     3523 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/heartbeat.css
+-rw-r--r--   0 root         (0) root         (0)    17599 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/hexdots.css
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/hole-pulse.css
+-rw-r--r--   0 root         (0) root         (0)     2713 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/inner-circles.css
+-rw-r--r--   0 root         (0) root         (0)     6223 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/plus-loader.css
+-rw-r--r--   0 root         (0) root         (0)    18677 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/plus.css
+-rw-r--r--   0 root         (0) root         (0)    12802 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/pong.css
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/pulse.css
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/refreshing.css
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/spinner.css
+-rw-r--r--   0 root         (0) root         (0)     4661 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/spinning-pixels.css
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/three-quarters.css
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/throbber.css
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/timer.css
+-rw-r--r--   0 root         (0) root         (0)    22371 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/whirly.css
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinner/wobblebar.css
+-rw-r--r--   0 root         (0) root         (0)   143659 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/spinners.css
+-rw-r--r--   0 root         (0) root         (0)        2 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/static/ytvid.mp4
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 05:20:19.269719 erscipcard-1.18.92/erscipcard/templates/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/templates/AvatarFileUploadInput.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 05:20:19.270719 erscipcard-1.18.92/erscipcard/templates/erscipcard/
+-rw-r--r--   0 root         (0) root         (0)     2606 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/templates/erscipcard/login.html
+-rw-r--r--   0 root         (0) root         (0)    12711 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/templates/erscipcard/ou.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 05:20:19.270719 erscipcard-1.18.92/erscipcard/templatetags/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/templatetags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      143 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/templatetags/basepath.py
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/tests.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/urls.py
+-rw-r--r--   0 root         (0) root         (0)    12726 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/views.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/widget.py
+-rw-r--r--   0 root         (0) root         (0)      296 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/yturls.py
+-rw-r--r--   0 root         (0) root         (0)     8838 2023-07-01 05:20:03.000000 erscipcard-1.18.92/erscipcard/ytviews.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 05:20:19.257718 erscipcard-1.18.92/erscipcard.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-07-01 05:20:19.000000 erscipcard-1.18.92/erscipcard.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2704 2023-07-01 05:20:19.000000 erscipcard-1.18.92/erscipcard.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-01 05:20:19.000000 erscipcard-1.18.92/erscipcard.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-01 05:20:19.000000 erscipcard-1.18.92/erscipcard.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-01 05:20:19.000000 erscipcard-1.18.92/erscipcard.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      780 2023-07-01 05:20:19.271719 erscipcard-1.18.92/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-01 05:20:03.000000 erscipcard-1.18.92/setup.py
```

### Comparing `erscipcard-1.18.91/LICENSE` & `erscipcard-1.18.92/LICENSE`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/PKG-INFO` & `erscipcard-1.18.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erscipcard
-Version: 1.18.91
+Version: 1.18.92
 Summary: Erscipcard is a Django app to create personeli card.
 Home-page: https://github.com/epg900/erscipcard.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `erscipcard-1.18.91/README.md` & `erscipcard-1.18.92/README.md`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/forms.py` & `erscipcard-1.18.92/erscipcard/forms.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/inst.py` & `erscipcard-1.18.92/erscipcard/inst.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         ''')
         f=open ('proj/proj/settings.py', 'r' )
         content = f.read()
         content_new = re.sub('(ALLOWED_HOSTS = \[)', r"\1'*'", content, flags = re.M)
         content_new = re.sub('(INSTALLED_APPS = \[)', r"\1\n'erscipcard',", content_new, flags = re.M)
         webhost=os.getenv('WEB_HOST')
         content_new += "\nERSCIYT_LINK = 'https://80-{}'".format(webhost)
-        content_new += "\nCSRF_TRUSTED_ORIGINS = ['https://8000-{}','https://127.0.0.1']".format(webhost)
+        content_new += "\nCSRF_TRUSTED_ORIGINS = ['https://*.cloudshell.dev','https://*.cs-us-central1-pits.cloudshell.dev','https://127.0.0.1','https://*.trycloudflare.com']".format(webhost)
         f.close()
         f=open ('proj/proj/settings.py', 'w' )
         f.write(content_new)
         f.close()
         f=open ('proj/proj/urls.py', 'r' )
         content = f.read()
         content_new = re.sub('(from django.urls import path)', r"\1,include", content, flags = re.M)
@@ -32,12 +32,13 @@
         f.close()
         f=open ('proj/proj/urls.py', 'w' )
         f.write(content_new)
         f.close() 
         os.system('python proj/manage.py migrate')
         os.system('echo "python proj/manage.py runserver" > s')
         os.system('chmod +x s')
-        os.system('python proj/manage.py createsuperuser --username=admin')
+        from django.contrib.auth.models import User
+        User.objects.create_superuser('root', 'epg900@gmail.com', '123')
         os.system('python proj/manage.py runserver')
     except:
         print('Error in command')
```

### Comparing `erscipcard-1.18.91/erscipcard/migrations/0001_initial.py` & `erscipcard-1.18.92/erscipcard/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/models.py` & `erscipcard-1.18.92/erscipcard/models.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/1.docx` & `erscipcard-1.18.92/erscipcard/static/1.docx`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/2.docx` & `erscipcard-1.18.92/erscipcard/static/2.docx`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/BNAZANIN.TTF` & `erscipcard-1.18.92/erscipcard/static/BNAZANIN.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/BTITR.TTF` & `erscipcard-1.18.92/erscipcard/static/BTITR.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/bt/css/bootstrap.min.css` & `erscipcard-1.18.92/erscipcard/static/bt/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/bt/css/font-awesome.min.css` & `erscipcard-1.18.92/erscipcard/static/bt/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/bt/css/loginstyle.css` & `erscipcard-1.18.92/erscipcard/static/bt/css/loginstyle.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/bt/css/persianDatepicker-default.css` & `erscipcard-1.18.92/erscipcard/static/bt/css/persianDatepicker-default.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/bt/css/style.css` & `erscipcard-1.18.92/erscipcard/static/bt/css/style.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/bt/css/util.css` & `erscipcard-1.18.92/erscipcard/static/bt/css/util.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/bt/fonts/BNAZANIN.TTF` & `erscipcard-1.18.92/erscipcard/static/bt/fonts/BNAZANIN.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/bt/fonts/BTITR.TTF` & `erscipcard-1.18.92/erscipcard/static/bt/fonts/BTITR.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/bt/fonts/Vazir.ttf` & `erscipcard-1.18.92/erscipcard/static/bt/fonts/Vazir.ttf`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/bt/fonts/fontawesome-webfont.ttf` & `erscipcard-1.18.92/erscipcard/static/bt/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/bt/js/bootstrap.bundle.min.js` & `erscipcard-1.18.92/erscipcard/static/bt/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/bt/js/jquery.min.js` & `erscipcard-1.18.92/erscipcard/static/bt/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/bt/js/persianDatepicker.js` & `erscipcard-1.18.92/erscipcard/static/bt/js/persianDatepicker.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/bt/js/scripts.js` & `erscipcard-1.18.92/erscipcard/static/bt/js/scripts.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/bt/pics/favicon.ico` & `erscipcard-1.18.92/erscipcard/static/bt/pics/favicon.ico`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/bt/pics/logo.png` & `erscipcard-1.18.92/erscipcard/static/bt/pics/logo.png`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/custom_modelField_with_formField` & `erscipcard-1.18.92/erscipcard/static/custom_modelField_with_formField`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/ersci_app.zip` & `erscipcard-1.18.92/erscipcard/static/ersci_app.zip`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/ersci_viddown_tab2-1.4.xpi` & `erscipcard-1.18.92/erscipcard/static/ersci_viddown_tab2-1.4.xpi`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/favicon.ico` & `erscipcard-1.18.92/erscipcard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/inst` & `erscipcard-1.18.92/erscipcard/static/inst`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/logo.png` & `erscipcard-1.18.92/erscipcard/static/logo.png`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/main.css` & `erscipcard-1.18.92/erscipcard/static/main.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/atebits.css` & `erscipcard-1.18.92/erscipcard/static/spinner/atebits.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/ball.css` & `erscipcard-1.18.92/erscipcard/static/spinner/ball.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/circles.css` & `erscipcard-1.18.92/erscipcard/static/spinner/circles.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/dots.css` & `erscipcard-1.18.92/erscipcard/static/spinner/dots.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/echo.css` & `erscipcard-1.18.92/erscipcard/static/spinner/echo.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/flower.css` & `erscipcard-1.18.92/erscipcard/static/spinner/flower.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/gauge.css` & `erscipcard-1.18.92/erscipcard/static/spinner/gauge.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/heartbeat.css` & `erscipcard-1.18.92/erscipcard/static/spinner/heartbeat.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/hexdots.css` & `erscipcard-1.18.92/erscipcard/static/spinner/hexdots.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/hole-pulse.css` & `erscipcard-1.18.92/erscipcard/static/spinner/hole-pulse.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/inner-circles.css` & `erscipcard-1.18.92/erscipcard/static/spinner/inner-circles.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/plus-loader.css` & `erscipcard-1.18.92/erscipcard/static/spinner/plus-loader.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/plus.css` & `erscipcard-1.18.92/erscipcard/static/spinner/plus.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/pong.css` & `erscipcard-1.18.92/erscipcard/static/spinner/pong.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/pulse.css` & `erscipcard-1.18.92/erscipcard/static/spinner/pulse.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/refreshing.css` & `erscipcard-1.18.92/erscipcard/static/spinner/refreshing.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/spinner.css` & `erscipcard-1.18.92/erscipcard/static/spinner/spinner.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/spinning-pixels.css` & `erscipcard-1.18.92/erscipcard/static/spinner/spinning-pixels.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/three-quarters.css` & `erscipcard-1.18.92/erscipcard/static/spinner/three-quarters.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/throbber.css` & `erscipcard-1.18.92/erscipcard/static/spinner/throbber.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/timer.css` & `erscipcard-1.18.92/erscipcard/static/spinner/timer.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/whirly.css` & `erscipcard-1.18.92/erscipcard/static/spinner/whirly.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinner/wobblebar.css` & `erscipcard-1.18.92/erscipcard/static/spinner/wobblebar.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/static/spinners.css` & `erscipcard-1.18.92/erscipcard/static/spinners.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/templates/erscipcard/login.html` & `erscipcard-1.18.92/erscipcard/templates/erscipcard/login.html`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/templates/erscipcard/ou.html` & `erscipcard-1.18.92/erscipcard/templates/erscipcard/ou.html`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/urls.py` & `erscipcard-1.18.92/erscipcard/urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,7 +44,10 @@
 	path('uploadtpl/', views.uploadtpl),
 	path('printalluser/', views.printalluser),
         path('showpic/<int:picid>/', views.showpic , name = 'showpic'),
         path('setpicwidth/<int:picwidth>/', views.setpicwidth ),
         path('qr/<str:idx>/', views.shqr ),
 ]
 
+from django.contrib.staticfiles.urls import staticfiles_urlpatterns
+urlpatterns += staticfiles_urlpatterns()
+
```

### Comparing `erscipcard-1.18.91/erscipcard/views.py` & `erscipcard-1.18.92/erscipcard/views.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/widget.py` & `erscipcard-1.18.92/erscipcard/widget.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard/ytviews.py` & `erscipcard-1.18.92/erscipcard/ytviews.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/erscipcard.egg-info/PKG-INFO` & `erscipcard-1.18.92/erscipcard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erscipcard
-Version: 1.18.91
+Version: 1.18.92
 Summary: Erscipcard is a Django app to create personeli card.
 Home-page: https://github.com/epg900/erscipcard.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `erscipcard-1.18.91/erscipcard.egg-info/SOURCES.txt` & `erscipcard-1.18.92/erscipcard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.91/setup.cfg` & `erscipcard-1.18.92/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = erscipcard
-version = 1.18.91
+version = 1.18.92
 description = Erscipcard is a Django app to create personeli card.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/erscipcard.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
```

