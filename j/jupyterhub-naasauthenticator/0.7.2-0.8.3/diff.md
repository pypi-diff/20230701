# Comparing `tmp/jupyterhub-naasauthenticator-0.7.2.tar.gz` & `tmp/jupyterhub-naasauthenticator-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jupyterhub-naasauthenticator-0.7.2.tar", last modified: Wed Nov 24 08:18:51 2021, max compression
+gzip compressed data, was "jupyterhub-naasauthenticator-0.8.3.tar", last modified: Sat Jul  1 07:56:06 2023, max compression
```

## Comparing `jupyterhub-naasauthenticator-0.7.2.tar` & `jupyterhub-naasauthenticator-0.8.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-24 08:18:51.321437 jupyterhub-naasauthenticator-0.7.2/
--rw-r--r--   0 root         (0) root         (0)     1510 2021-11-24 08:18:08.000000 jupyterhub-naasauthenticator-0.7.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      166 2021-11-24 08:18:08.000000 jupyterhub-naasauthenticator-0.7.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1346 2021-11-24 08:18:51.321437 jupyterhub-naasauthenticator-0.7.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      789 2021-11-24 08:18:08.000000 jupyterhub-naasauthenticator-0.7.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-24 08:18:51.309437 jupyterhub-naasauthenticator-0.7.2/docs/
--rw-r--r--   0 root         (0) root         (0)      580 2021-11-24 08:18:08.000000 jupyterhub-naasauthenticator-0.7.2/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-24 08:18:51.317437 jupyterhub-naasauthenticator-0.7.2/docs/_static/
--rw-r--r--   0 root         (0) root         (0)   188847 2021-11-24 08:18:08.000000 jupyterhub-naasauthenticator-0.7.2/docs/_static/authorization_area.png
--rw-r--r--   0 root         (0) root         (0)  2487640 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/docs/_static/block_user_failed_logins.png
--rw-r--r--   0 root         (0) root         (0)   161847 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/docs/_static/change-password.png
--rw-r--r--   0 root         (0) root         (0)    85574 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/docs/_static/login-two-factor-auth.png
--rw-r--r--   0 root         (0) root         (0)  1355938 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/docs/_static/native_auth_flow.png
--rw-r--r--   0 root         (0) root         (0)    91790 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/docs/_static/signup-two-factor-auth.png
--rw-r--r--   0 root         (0) root         (0)    78767 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/docs/_static/wrong_signup.png
--rw-r--r--   0 root         (0) root         (0)     5390 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     1008 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      787 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)     4785 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/docs/options.rst
--rw-r--r--   0 root         (0) root         (0)     2979 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/docs/quickstart.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-24 08:18:51.317437 jupyterhub-naasauthenticator-0.7.2/jupyterhub_naasauthenticator.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1346 2021-11-24 08:18:51.000000 jupyterhub-naasauthenticator-0.7.2/jupyterhub_naasauthenticator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1462 2021-11-24 08:18:51.000000 jupyterhub-naasauthenticator-0.7.2/jupyterhub_naasauthenticator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-24 08:18:51.000000 jupyterhub-naasauthenticator-0.7.2/jupyterhub_naasauthenticator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      136 2021-11-24 08:18:51.000000 jupyterhub-naasauthenticator-0.7.2/jupyterhub_naasauthenticator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2021-11-24 08:18:51.000000 jupyterhub-naasauthenticator-0.7.2/jupyterhub_naasauthenticator.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-24 08:18:51.317437 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/
--rw-r--r--   0 root         (0) root         (0)      109 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76508 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/common-credentials.txt
--rw-r--r--   0 root         (0) root         (0)    18595 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/handlers.py
--rw-r--r--   0 root         (0) root         (0)    10457 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/naasauthenticator.py
--rw-r--r--   0 root         (0) root         (0)     2210 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/orm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-24 08:18:51.321437 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/templates/
--rw-r--r--   0 root         (0) root         (0)      173 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/templates/admin.html
--rw-r--r--   0 root         (0) root         (0)     2032 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/templates/autorization-area.html
--rw-r--r--   0 root         (0) root         (0)     1561 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/templates/change-password.html
--rw-r--r--   0 root         (0) root         (0)       85 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/templates/home.html
--rw-r--r--   0 root         (0) root         (0)     3861 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/templates/native-login.html
--rw-r--r--   0 root         (0) root         (0)       89 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/templates/not_running.html
--rw-r--r--   0 root         (0) root         (0)     3501 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/templates/page.html
--rw-r--r--   0 root         (0) root         (0)     1133 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/templates/reset-password.html
--rw-r--r--   0 root         (0) root         (0)       83 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/templates/spawn.html
--rw-r--r--   0 root         (0) root         (0)     1040 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/templates/spawn_pending.html
--rw-r--r--   0 root         (0) root         (0)       90 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/templates/stop_pending.html
--rw-r--r--   0 root         (0) root         (0)       83 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/templates/token.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-24 08:18:51.321437 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7607 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/tests/test_authenticator.py
--rw-r--r--   0 root         (0) root         (0)      906 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/naasauthenticator/tests/test_orm.py
--rw-r--r--   0 root         (0) root         (0)       70 2021-11-24 08:18:51.321437 jupyterhub-naasauthenticator-0.7.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      874 2021-11-24 08:18:09.000000 jupyterhub-naasauthenticator-0.7.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:06.592546 jupyterhub-naasauthenticator-0.8.3/
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      166 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-07-01 07:56:06.592546 jupyterhub-naasauthenticator-0.8.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      789 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:06.580546 jupyterhub-naasauthenticator-0.8.3/docs/
+-rw-r--r--   0 root         (0) root         (0)      580 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:06.588546 jupyterhub-naasauthenticator-0.8.3/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)   188847 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/_static/authorization_area.png
+-rw-r--r--   0 root         (0) root         (0)  2487640 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/_static/block_user_failed_logins.png
+-rw-r--r--   0 root         (0) root         (0)   161847 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/_static/change-password.png
+-rw-r--r--   0 root         (0) root         (0)    85574 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/_static/login-two-factor-auth.png
+-rw-r--r--   0 root         (0) root         (0)  1355938 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/_static/native_auth_flow.png
+-rw-r--r--   0 root         (0) root         (0)    91790 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/_static/signup-two-factor-auth.png
+-rw-r--r--   0 root         (0) root         (0)    78767 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/_static/wrong_signup.png
+-rw-r--r--   0 root         (0) root         (0)     5390 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      787 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)     4785 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/options.rst
+-rw-r--r--   0 root         (0) root         (0)     2979 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/docs/quickstart.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:06.588546 jupyterhub-naasauthenticator-0.8.3/jupyterhub_naasauthenticator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-07-01 07:56:06.000000 jupyterhub-naasauthenticator-0.8.3/jupyterhub_naasauthenticator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1462 2023-07-01 07:56:06.000000 jupyterhub-naasauthenticator-0.8.3/jupyterhub_naasauthenticator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-01 07:56:06.000000 jupyterhub-naasauthenticator-0.8.3/jupyterhub_naasauthenticator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2023-07-01 07:56:06.000000 jupyterhub-naasauthenticator-0.8.3/jupyterhub_naasauthenticator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-01 07:56:06.000000 jupyterhub-naasauthenticator-0.8.3/jupyterhub_naasauthenticator.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:06.588546 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76508 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/common-credentials.txt
+-rw-r--r--   0 root         (0) root         (0)    18595 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/handlers.py
+-rw-r--r--   0 root         (0) root         (0)    10457 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/naasauthenticator.py
+-rw-r--r--   0 root         (0) root         (0)     2210 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/orm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:06.592546 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/
+-rw-r--r--   0 root         (0) root         (0)      173 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/admin.html
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/autorization-area.html
+-rw-r--r--   0 root         (0) root         (0)     1561 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/change-password.html
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/home.html
+-rw-r--r--   0 root         (0) root         (0)     6580 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/native-login.html
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/not_running.html
+-rw-r--r--   0 root         (0) root         (0)     3502 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/page.html
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/reset-password.html
+-rw-r--r--   0 root         (0) root         (0)       83 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/spawn.html
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/spawn_pending.html
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/stop_pending.html
+-rw-r--r--   0 root         (0) root         (0)       83 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/token.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 07:56:06.592546 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7607 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/tests/test_authenticator.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/naasauthenticator/tests/test_orm.py
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-01 07:56:06.592546 jupyterhub-naasauthenticator-0.8.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      874 2023-07-01 07:55:34.000000 jupyterhub-naasauthenticator-0.8.3/setup.py
```

### Comparing `jupyterhub-naasauthenticator-0.7.2/LICENSE` & `jupyterhub-naasauthenticator-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/PKG-INFO` & `jupyterhub-naasauthenticator-0.8.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: jupyterhub-naasauthenticator
-Version: 0.7.2
+Version: 0.8.3
 Summary: JupyterHub Native Authenticator
 Home-page: https://github.com/cashstory/naasauthenticator
 Author: Martin DONADIEU
 Author-email: bob@cashstory.com
 License: 3 Clause BSD
-Description: # Naas Authenticator
-        
-        Naas Authenticator provides the following features:
-        
-        * New users can signup on the system;
-        * New users can be blocked of accessing the system and need an admin authorization;
-        * Option of increase password security by avoiding common passwords or minimum password length;
-        * Option to block users after a number attempts of login;
-        * Option of open signup and no need for initial authorization;
-        * Option of open change password (open_change_password);
-        * Option of adding more information about users on signup.
-        
-        
-        ## Documentation
-        
-        Documentation is available [here](https://naas-authenticator.readthedocs.io)
-        
-        
-        ## Running tests
-        
-        To run the tests locally, you can install the development dependencies:
-        
-        `$ pip install -e '.[dev]'`
-        
-        Then run tests with pytest:
-        
-        `$ pytest`
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# Naas Authenticator
+
+Naas Authenticator provides the following features:
+
+* New users can signup on the system;
+* New users can be blocked of accessing the system and need an admin authorization;
+* Option of increase password security by avoiding common passwords or minimum password length;
+* Option to block users after a number attempts of login;
+* Option of open signup and no need for initial authorization;
+* Option of open change password (open_change_password);
+* Option of adding more information about users on signup.
+
+
+## Documentation
+
+Documentation is available [here](https://naas-authenticator.readthedocs.io)
+
+
+## Running tests
+
+To run the tests locally, you can install the development dependencies:
+
+`$ pip install -e '.[dev]'`
+
+Then run tests with pytest:
+
+`$ pytest`
```

### Comparing `jupyterhub-naasauthenticator-0.7.2/README.md` & `jupyterhub-naasauthenticator-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/docs/Makefile` & `jupyterhub-naasauthenticator-0.8.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/docs/_static/authorization_area.png` & `jupyterhub-naasauthenticator-0.8.3/docs/_static/authorization_area.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/docs/_static/block_user_failed_logins.png` & `jupyterhub-naasauthenticator-0.8.3/docs/_static/block_user_failed_logins.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/docs/_static/change-password.png` & `jupyterhub-naasauthenticator-0.8.3/docs/_static/change-password.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/docs/_static/login-two-factor-auth.png` & `jupyterhub-naasauthenticator-0.8.3/docs/_static/login-two-factor-auth.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/docs/_static/native_auth_flow.png` & `jupyterhub-naasauthenticator-0.8.3/docs/_static/native_auth_flow.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/docs/_static/signup-two-factor-auth.png` & `jupyterhub-naasauthenticator-0.8.3/docs/_static/signup-two-factor-auth.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/docs/_static/wrong_signup.png` & `jupyterhub-naasauthenticator-0.8.3/docs/_static/wrong_signup.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/docs/conf.py` & `jupyterhub-naasauthenticator-0.8.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/docs/index.rst` & `jupyterhub-naasauthenticator-0.8.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/docs/make.bat` & `jupyterhub-naasauthenticator-0.8.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/docs/options.rst` & `jupyterhub-naasauthenticator-0.8.3/docs/options.rst`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/docs/quickstart.rst` & `jupyterhub-naasauthenticator-0.8.3/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/jupyterhub_naasauthenticator.egg-info/PKG-INFO` & `jupyterhub-naasauthenticator-0.8.3/jupyterhub_naasauthenticator.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: jupyterhub-naasauthenticator
-Version: 0.7.2
+Version: 0.8.3
 Summary: JupyterHub Native Authenticator
 Home-page: https://github.com/cashstory/naasauthenticator
 Author: Martin DONADIEU
 Author-email: bob@cashstory.com
 License: 3 Clause BSD
-Description: # Naas Authenticator
-        
-        Naas Authenticator provides the following features:
-        
-        * New users can signup on the system;
-        * New users can be blocked of accessing the system and need an admin authorization;
-        * Option of increase password security by avoiding common passwords or minimum password length;
-        * Option to block users after a number attempts of login;
-        * Option of open signup and no need for initial authorization;
-        * Option of open change password (open_change_password);
-        * Option of adding more information about users on signup.
-        
-        
-        ## Documentation
-        
-        Documentation is available [here](https://naas-authenticator.readthedocs.io)
-        
-        
-        ## Running tests
-        
-        To run the tests locally, you can install the development dependencies:
-        
-        `$ pip install -e '.[dev]'`
-        
-        Then run tests with pytest:
-        
-        `$ pytest`
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# Naas Authenticator
+
+Naas Authenticator provides the following features:
+
+* New users can signup on the system;
+* New users can be blocked of accessing the system and need an admin authorization;
+* Option of increase password security by avoiding common passwords or minimum password length;
+* Option to block users after a number attempts of login;
+* Option of open signup and no need for initial authorization;
+* Option of open change password (open_change_password);
+* Option of adding more information about users on signup.
+
+
+## Documentation
+
+Documentation is available [here](https://naas-authenticator.readthedocs.io)
+
+
+## Running tests
+
+To run the tests locally, you can install the development dependencies:
+
+`$ pip install -e '.[dev]'`
+
+Then run tests with pytest:
+
+`$ pytest`
```

### Comparing `jupyterhub-naasauthenticator-0.7.2/jupyterhub_naasauthenticator.egg-info/SOURCES.txt` & `jupyterhub-naasauthenticator-0.8.3/jupyterhub_naasauthenticator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/naasauthenticator/common-credentials.txt` & `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/common-credentials.txt`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/naasauthenticator/handlers.py` & `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/naasauthenticator/naasauthenticator.py` & `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/naasauthenticator.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/naasauthenticator/orm.py` & `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/orm.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/naasauthenticator/templates/autorization-area.html` & `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/autorization-area.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/naasauthenticator/templates/change-password.html` & `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/change-password.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/naasauthenticator/templates/page.html` & `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/page.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% extends "templates/page.html" %}
 
-{% block title %}Naas hub{% endblock %}
+{% block title %}Lab{% endblock %}
 {% block favicon %}
 <link rel="icon" href="logo" type="image/x-icon">
 {% endblock %}
 {% block stylesheet %}
 {{ super() }}
 <style>
   body {
@@ -106,15 +106,15 @@
 
   .auth-form-body {
     border: 2px solid !important;
   }
 
   .naas-logo {
     width: 100% !important;
-    height: 15rem;
+    /* height: 15rem; */
   }
 
   .btn-primary {
     background-color: rgba(71, 221, 130, 1);
     border-color: rgba(71, 221, 130, 1);
   }
   .btn-primary:active,
```

### Comparing `jupyterhub-naasauthenticator-0.7.2/naasauthenticator/templates/spawn_pending.html` & `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/templates/spawn_pending.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/naasauthenticator/tests/test_authenticator.py` & `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/tests/test_authenticator.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 async def test_list_users(tmpcwd, app):
     auth = NaasAuthenticator(db=app.db)
     auth.create_user("johnsnow", "password")
     auth.create_user("johnsnow2", "password2")
 
     res = auth.get_users()
     users = [item.as_dict() for item in res]
-    assert len(users) == 2
+    assert len(users) == 3
     user = dict(users[0])
     assert type(user) == dict
 
 
 async def test_delete_user(tmpcwd, app):
     auth = NaasAuthenticator(db=app.db)
     auth.create_user("johnsnow", "password")
```

### Comparing `jupyterhub-naasauthenticator-0.7.2/naasauthenticator/tests/test_orm.py` & `jupyterhub-naasauthenticator-0.8.3/naasauthenticator/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-naasauthenticator-0.7.2/setup.py` & `jupyterhub-naasauthenticator-0.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="jupyterhub-naasauthenticator",
-    version="0.7.2",
+    version="0.8.3",
     description="JupyterHub Native Authenticator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cashstory/naasauthenticator",
     author="Martin DONADIEU",
     author_email="bob@cashstory.com",
     license="3 Clause BSD",
```

