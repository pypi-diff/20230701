# Comparing `tmp/wizzi_utils-8.0.5.tar.gz` & `tmp/wizzi_utils-8.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wizzi_utils-8.0.5.tar", last modified: Fri Jun  9 13:36:53 2023, max compression
+gzip compressed data, was "dist\wizzi_utils-8.0.6.tar", last modified: Sat Jul  1 09:58:35 2023, max compression
```

## Comparing `wizzi_utils-8.0.5.tar` & `wizzi_utils-8.0.6.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.135202 wizzi_utils-8.0.5/
--rw-rw-rw-   0        0        0     1077 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0     6839 2023-06-09 13:36:53.135202 wizzi_utils-8.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     6003 2023-05-26 18:32:12.000000 wizzi_utils-8.0.5/README.md
--rw-rw-rw-   0        0        0       86 2023-06-09 13:36:53.136199 wizzi_utils-8.0.5/setup.cfg
--rw-rw-rw-   0        0        0     2721 2023-06-09 13:35:15.000000 wizzi_utils-8.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.098326 wizzi_utils-8.0.5/wizzi_utils/
--rw-rw-rw-   0        0        0     2215 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.102313 wizzi_utils-8.0.5/wizzi_utils/google/
--rw-rw-rw-   0        0        0      140 2023-05-18 12:28:31.000000 wizzi_utils-8.0.5/wizzi_utils/google/__init__.py
--rw-rw-rw-   0        0        0    29127 2023-05-18 12:36:17.000000 wizzi_utils-8.0.5/wizzi_utils/google/google_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.103309 wizzi_utils-8.0.5/wizzi_utils/google/test/
--rw-rw-rw-   0        0        0      111 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/google/test/__init__.py
--rw-rw-rw-   0        0        0    12539 2023-05-18 12:32:45.000000 wizzi_utils-8.0.5/wizzi_utils/google/test/test_google_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.105302 wizzi_utils-8.0.5/wizzi_utils/json/
--rw-rw-rw-   0        0        0      134 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/json/__init__.py
--rw-rw-rw-   0        0        0     3035 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/json/json_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.106299 wizzi_utils-8.0.5/wizzi_utils/json/test/
--rw-rw-rw-   0        0        0      107 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/json/test/__init__.py
--rw-rw-rw-   0        0        0     1815 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/json/test/test_json_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.106299 wizzi_utils-8.0.5/wizzi_utils/misc/
--rw-rw-rw-   0        0        0      134 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/misc/__init__.py
--rw-rw-rw-   0        0        0    93477 2023-06-09 13:35:19.000000 wizzi_utils-8.0.5/wizzi_utils/misc/misc_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.108292 wizzi_utils-8.0.5/wizzi_utils/misc/test/
--rw-rw-rw-   0        0        0      107 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/misc/test/__init__.py
--rw-rw-rw-   0        0        0    41133 2023-05-18 11:21:37.000000 wizzi_utils-8.0.5/wizzi_utils/misc/test/test_misc_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.110286 wizzi_utils-8.0.5/wizzi_utils/models/
--rw-rw-rw-   0        0        0      316 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/__init__.py
--rw-rw-rw-   0        0        0    32920 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/base_models.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.112279 wizzi_utils-8.0.5/wizzi_utils/models/cv2_models/
--rw-rw-rw-   0        0        0      447 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/cv2_models/__init__.py
--rw-rw-rw-   0        0        0    11967 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/cv2_models/object_detection.py
--rw-rw-rw-   0        0        0    30085 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/cv2_models/pose_detection.py
--rw-rw-rw-   0        0        0    13099 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/cv2_models/tracking.py
--rw-rw-rw-   0        0        0    41515 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/labels_bank.py
--rw-rw-rw-   0        0        0    53088 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/models_configs.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.116266 wizzi_utils-8.0.5/wizzi_utils/models/test/
--rw-rw-rw-   0        0        0      201 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/test/__init__.py
--rw-rw-rw-   0        0        0     9974 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/test/shared_code_for_tests.py
--rw-rw-rw-   0        0        0     3796 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/test/test_cv2_od.py
--rw-rw-rw-   0        0        0     4868 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/test/test_cv2_pd.py
--rw-rw-rw-   0        0        0     5884 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/test/test_cv2_tracking.py
--rw-rw-rw-   0        0        0     1916 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/test/test_models.py
--rw-rw-rw-   0        0        0     3683 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/test/test_tflite_od.py
--rw-rw-rw-   0        0        0     4392 2023-05-18 13:12:36.000000 wizzi_utils-8.0.5/wizzi_utils/models/test/test_tflite_pd.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.118259 wizzi_utils-8.0.5/wizzi_utils/models/tflite_models/
--rw-rw-rw-   0        0        0      308 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/tflite_models/__init__.py
--rw-rw-rw-   0        0        0    12906 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/tflite_models/object_detection.py
--rw-rw-rw-   0        0        0    19806 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/models/tflite_models/pose_detection.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.119255 wizzi_utils-8.0.5/wizzi_utils/open_cv/
--rw-rw-rw-   0        0        0      143 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/open_cv/__init__.py
--rw-rw-rw-   0        0        0    53198 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/open_cv/open_cv_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.120252 wizzi_utils-8.0.5/wizzi_utils/open_cv/test/
--rw-rw-rw-   0        0        0      113 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/open_cv/test/__init__.py
--rw-rw-rw-   0        0        0    40649 2023-05-18 12:57:14.000000 wizzi_utils-8.0.5/wizzi_utils/open_cv/test/test_open_cv_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.121249 wizzi_utils-8.0.5/wizzi_utils/pyplot/
--rw-rw-rw-   0        0        0      140 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/pyplot/__init__.py
--rw-rw-rw-   0        0        0    67007 2023-06-09 13:22:11.000000 wizzi_utils-8.0.5/wizzi_utils/pyplot/pyplot_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.122245 wizzi_utils-8.0.5/wizzi_utils/pyplot/test/
--rw-rw-rw-   0        0        0      111 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/pyplot/test/__init__.py
--rw-rw-rw-   0        0        0    38480 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/pyplot/test/test_pyplot_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.123242 wizzi_utils-8.0.5/wizzi_utils/socket/
--rw-rw-rw-   0        0        0      140 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/socket/__init__.py
--rw-rw-rw-   0        0        0    24353 2023-05-18 11:25:24.000000 wizzi_utils-8.0.5/wizzi_utils/socket/socket_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.124239 wizzi_utils-8.0.5/wizzi_utils/socket/test/
--rw-rw-rw-   0        0        0      111 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/socket/test/__init__.py
--rw-rw-rw-   0        0        0    10494 2023-05-18 11:29:49.000000 wizzi_utils-8.0.5/wizzi_utils/socket/test/test_socket_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.125235 wizzi_utils-8.0.5/wizzi_utils/tflite/
--rw-rw-rw-   0        0        0      264 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/tflite/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.125235 wizzi_utils-8.0.5/wizzi_utils/tflite/test/
--rw-rw-rw-   0        0        0      105 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/tflite/test/__init__.py
--rw-rw-rw-   0        0        0      403 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/tflite/test/test_tflite.py
--rw-rw-rw-   0        0        0     2952 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/tflite/tflite_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.126232 wizzi_utils-8.0.5/wizzi_utils/torch/
--rw-rw-rw-   0        0        0      636 2023-05-26 18:23:15.000000 wizzi_utils-8.0.5/wizzi_utils/torch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.127229 wizzi_utils-8.0.5/wizzi_utils/torch/test/
--rw-rw-rw-   0        0        0      109 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/torch/test/__init__.py
--rw-rw-rw-   0        0        0    16354 2023-05-18 13:15:33.000000 wizzi_utils-8.0.5/wizzi_utils/torch/test/test_torch_tools.py
--rw-rw-rw-   0        0        0    26441 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/torch/torch_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.128225 wizzi_utils-8.0.5/wizzi_utils/tts/
--rw-rw-rw-   0        0        0      125 2023-05-18 13:05:38.000000 wizzi_utils-8.0.5/wizzi_utils/tts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.129222 wizzi_utils-8.0.5/wizzi_utils/tts/test/
--rw-rw-rw-   0        0        0       99 2023-05-18 08:10:35.000000 wizzi_utils-8.0.5/wizzi_utils/tts/test/__init__.py
--rw-rw-rw-   0        0        0     3309 2023-06-09 13:28:53.000000 wizzi_utils-8.0.5/wizzi_utils/tts/test/test_tts.py
--rw-rw-rw-   0        0        0    21600 2023-06-09 13:31:50.000000 wizzi_utils-8.0.5/wizzi_utils/tts/tts.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:36:53.101315 wizzi_utils-8.0.5/wizzi_utils.egg-info/
--rw-rw-rw-   0        0        0     6839 2023-06-09 13:36:53.000000 wizzi_utils-8.0.5/wizzi_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4360 2023-06-09 13:36:53.000000 wizzi_utils-8.0.5/wizzi_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 13:36:53.000000 wizzi_utils-8.0.5/wizzi_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-09 13:36:53.000000 wizzi_utils-8.0.5/wizzi_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0      491 2023-06-09 13:36:53.000000 wizzi_utils-8.0.5/wizzi_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.785164 wizzi_utils-8.0.6/
+-rw-rw-rw-   0        0        0     1077 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     6835 2023-07-01 09:58:35.785164 wizzi_utils-8.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6003 2023-06-22 14:42:14.000000 wizzi_utils-8.0.6/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-01 09:58:35.785164 wizzi_utils-8.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2721 2023-07-01 09:52:52.000000 wizzi_utils-8.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.675813 wizzi_utils-8.0.6/wizzi_utils/
+-rw-rw-rw-   0        0        0     2215 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.675813 wizzi_utils-8.0.6/wizzi_utils/google/
+-rw-rw-rw-   0        0        0      140 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/google/__init__.py
+-rw-rw-rw-   0        0        0    29127 2023-06-22 14:42:14.000000 wizzi_utils-8.0.6/wizzi_utils/google/google_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.675813 wizzi_utils-8.0.6/wizzi_utils/google/test/
+-rw-rw-rw-   0        0        0      111 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/google/test/__init__.py
+-rw-rw-rw-   0        0        0    12539 2023-06-22 14:42:14.000000 wizzi_utils-8.0.6/wizzi_utils/google/test/test_google_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.691435 wizzi_utils-8.0.6/wizzi_utils/json/
+-rw-rw-rw-   0        0        0      134 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/json/__init__.py
+-rw-rw-rw-   0        0        0     3035 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/json/json_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.691435 wizzi_utils-8.0.6/wizzi_utils/json/test/
+-rw-rw-rw-   0        0        0      107 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/json/test/__init__.py
+-rw-rw-rw-   0        0        0     1815 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/json/test/test_json_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.691435 wizzi_utils-8.0.6/wizzi_utils/misc/
+-rw-rw-rw-   0        0        0      134 2023-07-01 09:46:02.000000 wizzi_utils-8.0.6/wizzi_utils/misc/__init__.py
+-rw-rw-rw-   0        0        0    94492 2023-07-01 09:50:28.000000 wizzi_utils-8.0.6/wizzi_utils/misc/misc_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.691435 wizzi_utils-8.0.6/wizzi_utils/misc/test/
+-rw-rw-rw-   0        0        0      107 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/misc/test/__init__.py
+-rw-rw-rw-   0        0        0    42238 2023-06-22 15:16:40.000000 wizzi_utils-8.0.6/wizzi_utils/misc/test/test_misc_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.707056 wizzi_utils-8.0.6/wizzi_utils/models/
+-rw-rw-rw-   0        0        0      316 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/models/__init__.py
+-rw-rw-rw-   0        0        0    32920 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/models/base_models.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.707056 wizzi_utils-8.0.6/wizzi_utils/models/cv2_models/
+-rw-rw-rw-   0        0        0      447 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/models/cv2_models/__init__.py
+-rw-rw-rw-   0        0        0    11967 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/models/cv2_models/object_detection.py
+-rw-rw-rw-   0        0        0    30085 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/models/cv2_models/pose_detection.py
+-rw-rw-rw-   0        0        0    13099 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/models/cv2_models/tracking.py
+-rw-rw-rw-   0        0        0    41515 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/models/labels_bank.py
+-rw-rw-rw-   0        0        0    53088 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/models/models_configs.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.722679 wizzi_utils-8.0.6/wizzi_utils/models/test/
+-rw-rw-rw-   0        0        0      201 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/models/test/__init__.py
+-rw-rw-rw-   0        0        0     9974 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/models/test/shared_code_for_tests.py
+-rw-rw-rw-   0        0        0     3796 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/models/test/test_cv2_od.py
+-rw-rw-rw-   0        0        0     4868 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/models/test/test_cv2_pd.py
+-rw-rw-rw-   0        0        0     5884 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/models/test/test_cv2_tracking.py
+-rw-rw-rw-   0        0        0     1916 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/models/test/test_models.py
+-rw-rw-rw-   0        0        0     3683 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/models/test/test_tflite_od.py
+-rw-rw-rw-   0        0        0     4392 2023-06-22 14:42:14.000000 wizzi_utils-8.0.6/wizzi_utils/models/test/test_tflite_pd.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.738299 wizzi_utils-8.0.6/wizzi_utils/models/tflite_models/
+-rw-rw-rw-   0        0        0      308 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/models/tflite_models/__init__.py
+-rw-rw-rw-   0        0        0    12906 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/models/tflite_models/object_detection.py
+-rw-rw-rw-   0        0        0    19806 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/models/tflite_models/pose_detection.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.738299 wizzi_utils-8.0.6/wizzi_utils/open_cv/
+-rw-rw-rw-   0        0        0      143 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/open_cv/__init__.py
+-rw-rw-rw-   0        0        0    53198 2023-06-22 14:42:14.000000 wizzi_utils-8.0.6/wizzi_utils/open_cv/open_cv_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.738299 wizzi_utils-8.0.6/wizzi_utils/open_cv/test/
+-rw-rw-rw-   0        0        0      113 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/open_cv/test/__init__.py
+-rw-rw-rw-   0        0        0    40649 2023-06-22 14:42:14.000000 wizzi_utils-8.0.6/wizzi_utils/open_cv/test/test_open_cv_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.753921 wizzi_utils-8.0.6/wizzi_utils/pyplot/
+-rw-rw-rw-   0        0        0      140 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/pyplot/__init__.py
+-rw-rw-rw-   0        0        0    66916 2023-07-01 09:48:07.000000 wizzi_utils-8.0.6/wizzi_utils/pyplot/pyplot_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.753921 wizzi_utils-8.0.6/wizzi_utils/pyplot/test/
+-rw-rw-rw-   0        0        0      111 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/pyplot/test/__init__.py
+-rw-rw-rw-   0        0        0    38480 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/pyplot/test/test_pyplot_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.753921 wizzi_utils-8.0.6/wizzi_utils/socket/
+-rw-rw-rw-   0        0        0      140 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/socket/__init__.py
+-rw-rw-rw-   0        0        0    24353 2023-06-22 14:42:14.000000 wizzi_utils-8.0.6/wizzi_utils/socket/socket_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.753921 wizzi_utils-8.0.6/wizzi_utils/socket/test/
+-rw-rw-rw-   0        0        0      111 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/socket/test/__init__.py
+-rw-rw-rw-   0        0        0    10494 2023-06-22 14:42:14.000000 wizzi_utils-8.0.6/wizzi_utils/socket/test/test_socket_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.769542 wizzi_utils-8.0.6/wizzi_utils/tflite/
+-rw-rw-rw-   0        0        0      264 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/tflite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.769542 wizzi_utils-8.0.6/wizzi_utils/tflite/test/
+-rw-rw-rw-   0        0        0      105 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/tflite/test/__init__.py
+-rw-rw-rw-   0        0        0      403 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/tflite/test/test_tflite.py
+-rw-rw-rw-   0        0        0     2952 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/tflite/tflite_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.769542 wizzi_utils-8.0.6/wizzi_utils/torch/
+-rw-rw-rw-   0        0        0      636 2023-06-22 14:42:14.000000 wizzi_utils-8.0.6/wizzi_utils/torch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.769542 wizzi_utils-8.0.6/wizzi_utils/torch/test/
+-rw-rw-rw-   0        0        0      109 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/torch/test/__init__.py
+-rw-rw-rw-   0        0        0    16354 2023-06-22 14:42:14.000000 wizzi_utils-8.0.6/wizzi_utils/torch/test/test_torch_tools.py
+-rw-rw-rw-   0        0        0    26441 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/torch/torch_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.769542 wizzi_utils-8.0.6/wizzi_utils/tts/
+-rw-rw-rw-   0        0        0      125 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/tts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.785164 wizzi_utils-8.0.6/wizzi_utils/tts/test/
+-rw-rw-rw-   0        0        0       99 2023-01-06 15:24:49.000000 wizzi_utils-8.0.6/wizzi_utils/tts/test/__init__.py
+-rw-rw-rw-   0        0        0     3309 2023-06-22 14:42:14.000000 wizzi_utils-8.0.6/wizzi_utils/tts/test/test_tts.py
+-rw-rw-rw-   0        0        0    21600 2023-06-22 14:42:14.000000 wizzi_utils-8.0.6/wizzi_utils/tts/tts.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:58:35.675813 wizzi_utils-8.0.6/wizzi_utils.egg-info/
+-rw-rw-rw-   0        0        0     6835 2023-07-01 09:58:35.000000 wizzi_utils-8.0.6/wizzi_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4360 2023-07-01 09:58:35.000000 wizzi_utils-8.0.6/wizzi_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 09:58:35.000000 wizzi_utils-8.0.6/wizzi_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-01 09:58:35.000000 wizzi_utils-8.0.6/wizzi_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      491 2023-07-01 09:58:35.000000 wizzi_utils-8.0.6/wizzi_utils.egg-info/top_level.txt
```

### Comparing `wizzi_utils-8.0.5/LICENSE.txt` & `wizzi_utils-8.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/PKG-INFO` & `wizzi_utils-8.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: wizzi_utils
-Version: 8.0.5
+Version: 8.0.6
 Summary: Debugging tools and fast coding
 Home-page: https://github.com/2easy4wizzi/wizzi_utils_pypi
+Download-URL: https://github.com/2easy4wizzi/wizzi_utils_pypi/archive/refs/tags/v_8.0.6.tar.gz
 Author: Gilad Eini
 Author-email: giladEini@gmail.com
 License: MIT
-Download-URL: https://github.com/2easy4wizzi/wizzi_utils_pypi/archive/refs/tags/v_8.0.5.tar.gz
 Keywords: debugging tools,json,open cv,pyplot,socket,torch,tf lite
 Platform: windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -183,9 +183,7 @@
 
 # text to speak gui over pyttsx3 and pyQt5 packages
 wu.tts.test.run_machine_buddy_gui_test()
 ```
 
 ![tts img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/tts.PNG?raw=true)
 
-
-
```

### Comparing `wizzi_utils-8.0.5/README.md` & `wizzi_utils-8.0.6/README.md`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/setup.py` & `wizzi_utils-8.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,23 +36,23 @@
         'wizzi_utils/tts',
         'wizzi_utils/tts/test',
         'wizzi_utils/models',
         'wizzi_utils/models/cv2_models',
         'wizzi_utils/models/tflite_models',
         'wizzi_utils/models/test',
     ],
-    version='8.0.5',
+    version='8.0.6',
     license='MIT',  # https://help.github.com/articles/licensing-a-repository
     description='Debugging tools and fast coding',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Gilad Eini',
     author_email='giladEini@gmail.com',
     url='https://github.com/2easy4wizzi/wizzi_utils_pypi',  # link to github
-    download_url='https://github.com/2easy4wizzi/wizzi_utils_pypi/archive/refs/tags/v_8.0.5.tar.gz',
+    download_url='https://github.com/2easy4wizzi/wizzi_utils_pypi/archive/refs/tags/v_8.0.6.tar.gz',
     keywords=[  # Keywords that define your package best
         'debugging tools',
         'json',
         'open cv',
         'pyplot',
         'socket',
         'torch',
```

### Comparing `wizzi_utils-8.0.5/wizzi_utils/__init__.py` & `wizzi_utils-8.0.6/wizzi_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/google/google_tools.py` & `wizzi_utils-8.0.6/wizzi_utils/google/google_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/google/test/test_google_tools.py` & `wizzi_utils-8.0.6/wizzi_utils/google/test/test_google_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/json/json_tools.py` & `wizzi_utils-8.0.6/wizzi_utils/json/json_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/json/test/test_json_tools.py` & `wizzi_utils-8.0.6/wizzi_utils/json/test/test_json_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/misc/misc_tools.py` & `wizzi_utils-8.0.6/wizzi_utils/misc/misc_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,15 @@
         pass
     return cuda_str
 
 
 def get_nvidia_gpus() -> str:
     try:
         cmd = 'nvidia-smi --query-gpu=gpu_name,memory.total --format=csv,noheader'
-        gpu_str_lines = run_shell_command_and_get_out(cmd=cmd, ack_cmd=False)
+        gpu_str_lines = run_shell_command_and_get_out(cmd=cmd, ack_cmd=False, print_if_exception=False)
         # gpu_str_lines = ['Quadro RTX 4000, 8192 Mib', 'Quadro RTX 4000, 8192 Mib']
 
         gpu_str_all = ''
         for i, gpu_str in enumerate(gpu_str_lines):
             gpu_name, gpu_size = gpu_str.split(', ')
             gpu_str_all += '[device {}] {} ({})'.format(i, gpu_name, gpu_size)
             if i + 1 < len(gpu_str_lines):
@@ -519,15 +519,15 @@
 
 
 def version() -> str:
     """
     :return:
     """
     # v = pkg_resources.require("wizzi_utils")[0].version
-    v = '8.0.5'
+    v = '8.0.6'
     return v
 
 
 def is_windows() -> bool:
     """
     :return:
     see os_test() - tested
@@ -2254,38 +2254,59 @@
                 print(avg_str_k)
 
         else:
             exception_error('Times_elapsed is empty', real_exception=False, tabs=tabs)
         return
 
 
-def run_shell_command(cmd: str, ack: bool = True) -> None:
+def run_shell_command(cmd: str, ack: bool = True, suppress_output: bool = False,
+                      print_if_exception: bool = True) -> None:
     try:
         if ack:
             print(add_color(cmd, ops='b'))
-        subprocess.check_call(cmd, shell=True)
+        if suppress_output:
+            # if your cmd is dir or ls, this is a bad idea to suppress output
+            # if you run an aux script that yield output that you dont need, then this is a good idea
+            subprocess.check_call(cmd, shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
+        else:
+            # will force print if there is anything to print
+            subprocess.check_call(cmd, shell=True)
 
     except subprocess.CalledProcessError as e:
-        exception_error(e, real_exception=True)
+        if print_if_exception:  # shows what went wrong
+            exception_error(e, real_exception=True)
     return
 
 
-def run_shell_command_and_get_out(cmd: str, ack_cmd: bool = True, ack_out: bool = False) -> list:
+def run_shell_command_and_get_out(
+        cmd: str,
+        ack_cmd: bool = True,
+        ack_out: bool = False,
+        suppress_errors_from_shell: bool = True,
+        print_if_exception: bool = True,
+) -> list:
     out = ['Failed']
     try:
         if ack_cmd:
             print(add_color(cmd, ops='b'))
-        out = subprocess.check_output(cmd, shell=True)
-        out = out.decode("utf-8").replace('\t', '').replace('\r', '').strip()
-        out = out.split('\n')
+
+        if suppress_errors_from_shell:
+            # let us handle the errors in the except block
+            out = subprocess.check_output(cmd, shell=True, stderr=subprocess.STDOUT)
+        else:
+            # will force print errors regardless to the except block
+            out = subprocess.check_output(cmd, shell=True)
+
+        out = out.decode("utf-8").replace('\t', '').replace('\r', '').strip().split('\n')
         if ack_out:
             for i, line in enumerate(out):
                 print('{}){}'.format(i, line))
     except subprocess.CalledProcessError as e:
-        exception_error(e, real_exception=True)
+        if print_if_exception:  # shows what went wrong
+            exception_error(e, real_exception=True)
     return out
 
 
 def add_sudo_to_cmd(cmd: str, sudo_password: str) -> str:
     cmd_wrap = 'echo {}|sudo -S {}'.format(sudo_password, cmd)
     return cmd_wrap
```

### Comparing `wizzi_utils-8.0.5/wizzi_utils/misc/test/test_misc_tools.py` & `wizzi_utils-8.0.6/wizzi_utils/misc/test/test_misc_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -930,18 +930,35 @@
     mt.generate_requirements_file(fp_out=fp)
     _ = mt.read_file_lines(fp=fp, ack=True)
     return
 
 
 def run_shell_command_test():
     mt.get_function_name_and_line(ack=True, tabs=0)
+
     if mt.is_windows():
-        mt.run_shell_command(cmd='dir')
+        print('dir with suppress output(bad idea with this command)')
+        mt.run_shell_command(cmd='dir', suppress_output=True)
+        print('dir without suppress output(good)')
+        mt.run_shell_command(cmd='dir', suppress_output=False)
+
+        print('bad command without suppress output and without print_if_exception(expecting error from shell)')
+        mt.run_shell_command(cmd='dirx1', suppress_output=False, print_if_exception=False)
+
+        print(
+            'bad command without suppress output and with print_if_exception(expecting error from shell and printing from the code)')
+        mt.run_shell_command(cmd='dirx2', suppress_output=False, print_if_exception=True)
+
+        print('bad command with suppress output and with print_if_exception(expecting printing from the code)')
+        mt.run_shell_command(cmd='dirx3', suppress_output=True, print_if_exception=True)
+
+        print('bad command with suppress output and without print_if_exception(expecting silent error)')
+        mt.run_shell_command(cmd='dirx4', suppress_output=True, print_if_exception=False)
     else:
-        mt.run_shell_command(cmd='ls')
+        mt.run_shell_command(cmd='ls')  # should behave the same as the above
     return
 
 
 def run_shell_command_and_get_out_test():
     mt.get_function_name_and_line(ack=True, tabs=0)
     if mt.is_windows():
         out = mt.run_shell_command_and_get_out(cmd='dir', ack_out=False)
```

### Comparing `wizzi_utils-8.0.5/wizzi_utils/models/base_models.py` & `wizzi_utils-8.0.6/wizzi_utils/models/base_models.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/models/cv2_models/object_detection.py` & `wizzi_utils-8.0.6/wizzi_utils/models/cv2_models/object_detection.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/models/cv2_models/pose_detection.py` & `wizzi_utils-8.0.6/wizzi_utils/models/cv2_models/pose_detection.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/models/cv2_models/tracking.py` & `wizzi_utils-8.0.6/wizzi_utils/models/cv2_models/tracking.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/models/labels_bank.py` & `wizzi_utils-8.0.6/wizzi_utils/models/labels_bank.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/models/models_configs.py` & `wizzi_utils-8.0.6/wizzi_utils/models/models_configs.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/models/test/shared_code_for_tests.py` & `wizzi_utils-8.0.6/wizzi_utils/models/test/shared_code_for_tests.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/models/test/test_cv2_od.py` & `wizzi_utils-8.0.6/wizzi_utils/models/test/test_cv2_od.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/models/test/test_cv2_pd.py` & `wizzi_utils-8.0.6/wizzi_utils/models/test/test_cv2_pd.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/models/test/test_cv2_tracking.py` & `wizzi_utils-8.0.6/wizzi_utils/models/test/test_cv2_tracking.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/models/test/test_models.py` & `wizzi_utils-8.0.6/wizzi_utils/models/test/test_models.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/models/test/test_tflite_od.py` & `wizzi_utils-8.0.6/wizzi_utils/models/test/test_tflite_od.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/models/test/test_tflite_pd.py` & `wizzi_utils-8.0.6/wizzi_utils/models/test/test_tflite_pd.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/models/tflite_models/object_detection.py` & `wizzi_utils-8.0.6/wizzi_utils/models/tflite_models/object_detection.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/models/tflite_models/pose_detection.py` & `wizzi_utils-8.0.6/wizzi_utils/models/tflite_models/pose_detection.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/open_cv/open_cv_tools.py` & `wizzi_utils-8.0.6/wizzi_utils/open_cv/open_cv_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/open_cv/test/test_open_cv_tools.py` & `wizzi_utils-8.0.6/wizzi_utils/open_cv/test/test_open_cv_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/pyplot/pyplot_tools.py` & `wizzi_utils-8.0.6/wizzi_utils/pyplot/pyplot_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 import matplotlib
 import matplotlib.pyplot as plt
 from matplotlib.figure import Figure
 import matplotlib.axes
 from matplotlib.backend_bases import KeyEvent
 from matplotlib.backend_bases import CloseEvent
 from matplotlib.collections import PathCollection
-# noinspection PyProtectedMember
-from matplotlib.backends._backend_tk import TimerTk
 from wizzi_utils.misc import misc_tools as mt
 
 
 class Location(Enum):
     TOP_LEFT = 'top_left'
     TOP_CENTER = 'top_center'
     TOP_RIGHT = 'top_right'
@@ -710,15 +708,15 @@
         path = '{}.png'.format(path)
         size_s = mt.file_or_folder_size(path)
         file_msg = '{}({})'.format(path, size_s)
         print('{}{}'.format(tabs * '\t', mt.SAVED.format(file_msg)))
     return
 
 
-def add_timer(fig: matplotlib.figure, max_time_seconds: float) -> TimerTk:
+def add_timer(fig: matplotlib.figure, max_time_seconds: float) -> any:
     """
     add timer for current fig window
     :param fig:
     :param max_time_seconds:
     :return:
     """
     # creating a timer object and setting an interval of 3000 milliseconds
```

### Comparing `wizzi_utils-8.0.5/wizzi_utils/pyplot/test/test_pyplot_tools.py` & `wizzi_utils-8.0.6/wizzi_utils/pyplot/test/test_pyplot_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/socket/socket_tools.py` & `wizzi_utils-8.0.6/wizzi_utils/socket/socket_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/socket/test/test_socket_tools.py` & `wizzi_utils-8.0.6/wizzi_utils/socket/test/test_socket_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/tflite/tflite_tools.py` & `wizzi_utils-8.0.6/wizzi_utils/tflite/tflite_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/torch/__init__.py` & `wizzi_utils-8.0.6/wizzi_utils/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/torch/test/test_torch_tools.py` & `wizzi_utils-8.0.6/wizzi_utils/torch/test/test_torch_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/torch/torch_tools.py` & `wizzi_utils-8.0.6/wizzi_utils/torch/torch_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/tts/test/test_tts.py` & `wizzi_utils-8.0.6/wizzi_utils/tts/test/test_tts.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils/tts/tts.py` & `wizzi_utils-8.0.6/wizzi_utils/tts/tts.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.5/wizzi_utils.egg-info/PKG-INFO` & `wizzi_utils-8.0.6/wizzi_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: wizzi-utils
-Version: 8.0.5
+Version: 8.0.6
 Summary: Debugging tools and fast coding
 Home-page: https://github.com/2easy4wizzi/wizzi_utils_pypi
+Download-URL: https://github.com/2easy4wizzi/wizzi_utils_pypi/archive/refs/tags/v_8.0.6.tar.gz
 Author: Gilad Eini
 Author-email: giladEini@gmail.com
 License: MIT
-Download-URL: https://github.com/2easy4wizzi/wizzi_utils_pypi/archive/refs/tags/v_8.0.5.tar.gz
 Keywords: debugging tools,json,open cv,pyplot,socket,torch,tf lite
 Platform: windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -183,9 +183,7 @@
 
 # text to speak gui over pyttsx3 and pyQt5 packages
 wu.tts.test.run_machine_buddy_gui_test()
 ```
 
 ![tts img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/tts.PNG?raw=true)
 
-
-
```

### Comparing `wizzi_utils-8.0.5/wizzi_utils.egg-info/SOURCES.txt` & `wizzi_utils-8.0.6/wizzi_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

