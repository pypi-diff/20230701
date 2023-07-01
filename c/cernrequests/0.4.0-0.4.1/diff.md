# Comparing `tmp/cernrequests-0.4.0.tar.gz` & `tmp/cernrequests-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cernrequests-0.4.0.tar", last modified: Fri Jun 30 15:32:16 2023, max compression
+gzip compressed data, was "cernrequests-0.4.1.tar", last modified: Sat Jul  1 09:00:20 2023, max compression
```

## Comparing `cernrequests-0.4.0.tar` & `cernrequests-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-06-30 15:32:16.097247 cernrequests-0.4.0/
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     7651 2023-05-23 15:59:26.000000 cernrequests-0.4.0/LICENSE
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     6466 2023-06-30 15:32:16.097247 cernrequests-0.4.0/PKG-INFO
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     6158 2023-06-30 15:28:53.000000 cernrequests-0.4.0/README.md
-drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-06-30 15:32:16.093248 cernrequests-0.4.0/cernrequests/
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      499 2023-06-30 15:28:53.000000 cernrequests-0.4.0/cernrequests/__init__.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     2718 2023-06-30 14:11:19.000000 cernrequests-0.4.0/cernrequests/certs.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     2479 2023-06-30 14:19:31.000000 cernrequests-0.4.0/cernrequests/cookies.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1811 2023-06-30 15:28:53.000000 cernrequests-0.4.0/cernrequests/core.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1475 2023-06-30 15:28:53.000000 cernrequests-0.4.0/cernrequests/token.py
-drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-06-30 15:32:16.097247 cernrequests-0.4.0/cernrequests.egg-info/
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     6466 2023-06-30 15:32:16.000000 cernrequests-0.4.0/cernrequests.egg-info/PKG-INFO
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      370 2023-06-30 15:32:16.000000 cernrequests-0.4.0/cernrequests.egg-info/SOURCES.txt
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)        1 2023-06-30 15:32:16.000000 cernrequests-0.4.0/cernrequests.egg-info/dependency_links.txt
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       36 2023-06-30 15:32:16.000000 cernrequests-0.4.0/cernrequests.egg-info/requires.txt
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       13 2023-06-30 15:32:16.000000 cernrequests-0.4.0/cernrequests.egg-info/top_level.txt
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       38 2023-06-30 15:32:16.097247 cernrequests-0.4.0/setup.cfg
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1250 2023-06-30 15:28:53.000000 cernrequests-0.4.0/setup.py
-drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-06-30 15:32:16.097247 cernrequests-0.4.0/tests/
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1335 2023-06-30 14:14:27.000000 cernrequests-0.4.0/tests/test_cernrequests.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1531 2023-06-30 15:28:53.000000 cernrequests-0.4.0/tests/test_real_data.py
+drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-07-01 09:00:20.648201 cernrequests-0.4.1/
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     7651 2023-05-23 15:59:26.000000 cernrequests-0.4.1/LICENSE
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     6721 2023-07-01 09:00:20.648201 cernrequests-0.4.1/PKG-INFO
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     6413 2023-07-01 08:57:18.000000 cernrequests-0.4.1/README.md
+drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-07-01 09:00:20.644201 cernrequests-0.4.1/cernrequests/
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      536 2023-07-01 08:57:25.000000 cernrequests-0.4.1/cernrequests/__init__.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)    14605 2023-06-30 14:11:06.000000 cernrequests-0.4.1/cernrequests/cern-cacert.pem
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     2718 2023-06-30 14:11:19.000000 cernrequests-0.4.1/cernrequests/certs.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     2479 2023-06-30 14:19:31.000000 cernrequests-0.4.1/cernrequests/cookies.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1811 2023-07-01 08:57:18.000000 cernrequests-0.4.1/cernrequests/core.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1475 2023-07-01 08:57:18.000000 cernrequests-0.4.1/cernrequests/token.py
+drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-07-01 09:00:20.648201 cernrequests-0.4.1/cernrequests.egg-info/
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     6721 2023-07-01 09:00:20.000000 cernrequests-0.4.1/cernrequests.egg-info/PKG-INFO
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      399 2023-07-01 09:00:20.000000 cernrequests-0.4.1/cernrequests.egg-info/SOURCES.txt
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)        1 2023-07-01 09:00:20.000000 cernrequests-0.4.1/cernrequests.egg-info/dependency_links.txt
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       36 2023-07-01 09:00:20.000000 cernrequests-0.4.1/cernrequests.egg-info/requires.txt
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       13 2023-07-01 09:00:20.000000 cernrequests-0.4.1/cernrequests.egg-info/top_level.txt
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       38 2023-07-01 09:00:20.648201 cernrequests-0.4.1/setup.cfg
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1248 2023-07-01 08:58:54.000000 cernrequests-0.4.1/setup.py
+drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-07-01 09:00:20.648201 cernrequests-0.4.1/tests/
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1335 2023-06-30 14:14:27.000000 cernrequests-0.4.1/tests/test_cernrequests.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1531 2023-07-01 08:57:18.000000 cernrequests-0.4.1/tests/test_real_data.py
```

### Comparing `cernrequests-0.4.0/LICENSE` & `cernrequests-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cernrequests-0.4.0/PKG-INFO` & `cernrequests-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cernrequests
-Version: 0.4.0
+Version: 0.4.1
 Home-page: https://github.com/CMSTrackerDPG/cernrequests
 Author: Peter Stein
 Author-email: peter.stein@cern.ch
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -44,27 +44,33 @@
 The `.pem` certificates have to be **passwordless**.
 
 ### For CERN APIs using the ""new"" SSO
 
 An `.env` file at the root of your project with the following variables set:
 - `SSO_CLIENT_ID`
 - `SSO_CLIENT_SECRET`
-  
+
+(You can rename the `.env_sample` file to `.env` and add the values there).
+
 To request them, you will need to register your application:
 
 1. Create an SSO registration for your application
     on the [CERN Application Portal](https://application-portal.web.cern.ch):
 
     ![](doc/create_registration_01.png)
 
 2. Add an application identifier and description:
 
     ![](doc/create_registration_02.png)
 
-3. Edit the SSO application, go to the `SSO Registration` tab and click the plus button:
+    The `Application Identifier` can be anything, it's like a username for your application.t 
+    
+    Click `Submit`.
+
+3. Go back to the Application Portal and edit the SSO application (green button). Then, go to the `SSO Registration` tab and click the plus button:
 
     ![](doc/create_registration_03.png)
 
 4. Fill out the form of the new SSO registration as follows:
 
     ![](doc/create_registration_04.png)
```

### Comparing `cernrequests-0.4.0/README.md` & `cernrequests-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,27 +34,33 @@
 The `.pem` certificates have to be **passwordless**.
 
 ### For CERN APIs using the ""new"" SSO
 
 An `.env` file at the root of your project with the following variables set:
 - `SSO_CLIENT_ID`
 - `SSO_CLIENT_SECRET`
-  
+
+(You can rename the `.env_sample` file to `.env` and add the values there).
+
 To request them, you will need to register your application:
 
 1. Create an SSO registration for your application
     on the [CERN Application Portal](https://application-portal.web.cern.ch):
 
     ![](doc/create_registration_01.png)
 
 2. Add an application identifier and description:
 
     ![](doc/create_registration_02.png)
 
-3. Edit the SSO application, go to the `SSO Registration` tab and click the plus button:
+    The `Application Identifier` can be anything, it's like a username for your application.t 
+    
+    Click `Submit`.
+
+3. Go back to the Application Portal and edit the SSO application (green button). Then, go to the `SSO Registration` tab and click the plus button:
 
     ![](doc/create_registration_03.png)
 
 4. Fill out the form of the new SSO registration as follows:
 
     ![](doc/create_registration_04.png)
```

### Comparing `cernrequests-0.4.0/cernrequests/certs.py` & `cernrequests-0.4.1/cernrequests/certs.py`

 * *Files identical despite different names*

### Comparing `cernrequests-0.4.0/cernrequests/cookies.py` & `cernrequests-0.4.1/cernrequests/cookies.py`

 * *Files identical despite different names*

### Comparing `cernrequests-0.4.0/cernrequests/core.py` & `cernrequests-0.4.1/cernrequests/core.py`

 * *Files identical despite different names*

### Comparing `cernrequests-0.4.0/cernrequests/token.py` & `cernrequests-0.4.1/cernrequests/token.py`

 * *Files identical despite different names*

### Comparing `cernrequests-0.4.0/cernrequests.egg-info/PKG-INFO` & `cernrequests-0.4.1/cernrequests.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cernrequests
-Version: 0.4.0
+Version: 0.4.1
 Home-page: https://github.com/CMSTrackerDPG/cernrequests
 Author: Peter Stein
 Author-email: peter.stein@cern.ch
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -44,27 +44,33 @@
 The `.pem` certificates have to be **passwordless**.
 
 ### For CERN APIs using the ""new"" SSO
 
 An `.env` file at the root of your project with the following variables set:
 - `SSO_CLIENT_ID`
 - `SSO_CLIENT_SECRET`
-  
+
+(You can rename the `.env_sample` file to `.env` and add the values there).
+
 To request them, you will need to register your application:
 
 1. Create an SSO registration for your application
     on the [CERN Application Portal](https://application-portal.web.cern.ch):
 
     ![](doc/create_registration_01.png)
 
 2. Add an application identifier and description:
 
     ![](doc/create_registration_02.png)
 
-3. Edit the SSO application, go to the `SSO Registration` tab and click the plus button:
+    The `Application Identifier` can be anything, it's like a username for your application.t 
+    
+    Click `Submit`.
+
+3. Go back to the Application Portal and edit the SSO application (green button). Then, go to the `SSO Registration` tab and click the plus button:
 
     ![](doc/create_registration_03.png)
 
 4. Fill out the form of the new SSO registration as follows:
 
     ![](doc/create_registration_04.png)
```

### Comparing `cernrequests-0.4.0/setup.py` & `cernrequests-0.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 setup(
     name="cernrequests",
-    version="0.4.0",
+    version="0.4.1",
     desription="CERN wrapper around the requests package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CMSTrackerDPG/cernrequests",
     author="Peter Stein",
     author_email="peter.stein@cern.ch",
     packages=["cernrequests"],
     package_dir={"cernrequests": "cernrequests"},
-    # package_data={"cernrequests": ["*.pem"]},
+    package_data={"cernrequests": ["*.pem"]},
     install_requires=["requests", "future", "python-dotenv", "pyjwt"],
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     ],
 )
```

### Comparing `cernrequests-0.4.0/tests/test_cernrequests.py` & `cernrequests-0.4.1/tests/test_cernrequests.py`

 * *Files identical despite different names*

### Comparing `cernrequests-0.4.0/tests/test_real_data.py` & `cernrequests-0.4.1/tests/test_real_data.py`

 * *Files identical despite different names*

