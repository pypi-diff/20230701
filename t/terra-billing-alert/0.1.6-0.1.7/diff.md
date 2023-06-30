# Comparing `tmp/terra_billing_alert-0.1.6.tar.gz` & `tmp/terra_billing_alert-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terra_billing_alert-0.1.6.tar", last modified: Thu Dec  1 18:05:27 2022, max compression
+gzip compressed data, was "terra_billing_alert-0.1.7.tar", last modified: Fri Jun 30 23:57:35 2023, max compression
```

## Comparing `terra_billing_alert-0.1.6.tar` & `terra_billing_alert-0.1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2022-12-01 18:05:27.577551 terra_billing_alert-0.1.6/
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1066 2022-08-04 17:44:05.000000 terra_billing_alert-0.1.6/LICENSE
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      519 2022-12-01 18:05:27.577551 terra_billing_alert-0.1.6/PKG-INFO
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     4283 2022-08-29 18:18:59.000000 terra_billing_alert-0.1.6/README.md
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2022-12-01 18:05:27.573551 terra_billing_alert-0.1.6/bin/
--rwxrwxr-x   0 leepc12   (1000) leepc12   (1000)      323 2022-08-29 18:18:59.000000 terra_billing_alert-0.1.6/bin/terra_billing_alert
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       38 2022-12-01 18:05:27.577551 terra_billing_alert-0.1.6/setup.cfg
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1694 2022-12-01 17:38:39.000000 terra_billing_alert-0.1.6/setup.py
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2022-12-01 18:05:27.577551 terra_billing_alert-0.1.6/terra_billing_alert/
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       22 2022-12-01 18:04:53.000000 terra_billing_alert-0.1.6/terra_billing_alert/__init__.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       61 2022-08-29 18:18:59.000000 terra_billing_alert-0.1.6/terra_billing_alert/__main__.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     4965 2022-12-01 00:34:59.000000 terra_billing_alert-0.1.6/terra_billing_alert/alert_item.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      730 2022-08-29 20:17:53.000000 terra_billing_alert-0.1.6/terra_billing_alert/alert_sender.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3962 2022-12-01 00:37:23.000000 terra_billing_alert-0.1.6/terra_billing_alert/bucket.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3422 2022-08-29 20:17:33.000000 terra_billing_alert-0.1.6/terra_billing_alert/cli.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      681 2022-08-29 18:18:59.000000 terra_billing_alert-0.1.6/terra_billing_alert/datetime_util.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    15275 2022-08-29 18:18:59.000000 terra_billing_alert-0.1.6/terra_billing_alert/gcp_machine_type.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6067 2022-12-01 18:04:25.000000 terra_billing_alert-0.1.6/terra_billing_alert/instance.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2595 2022-10-26 16:47:25.000000 terra_billing_alert-0.1.6/terra_billing_alert/terra_util.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6575 2022-12-01 17:37:58.000000 terra_billing_alert-0.1.6/terra_billing_alert/workflow.py
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2022-12-01 18:05:27.577551 terra_billing_alert-0.1.6/terra_billing_alert.egg-info/
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      519 2022-12-01 18:05:27.000000 terra_billing_alert-0.1.6/terra_billing_alert.egg-info/PKG-INFO
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      630 2022-12-01 18:05:27.000000 terra_billing_alert-0.1.6/terra_billing_alert.egg-info/SOURCES.txt
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)        1 2022-12-01 18:05:27.000000 terra_billing_alert-0.1.6/terra_billing_alert.egg-info/dependency_links.txt
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      123 2022-12-01 18:05:27.000000 terra_billing_alert-0.1.6/terra_billing_alert.egg-info/requires.txt
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       20 2022-12-01 18:05:27.000000 terra_billing_alert-0.1.6/terra_billing_alert.egg-info/top_level.txt
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-06-30 23:57:35.005793 terra_billing_alert-0.1.7/
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1066 2022-08-04 17:44:05.000000 terra_billing_alert-0.1.7/LICENSE
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      519 2023-06-30 23:57:35.005793 terra_billing_alert-0.1.7/PKG-INFO
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     4283 2022-08-29 18:18:59.000000 terra_billing_alert-0.1.7/README.md
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-06-30 23:57:35.001793 terra_billing_alert-0.1.7/bin/
+-rwxrwxr-x   0 leepc12   (1000) leepc12   (1000)      323 2022-08-29 18:18:59.000000 terra_billing_alert-0.1.7/bin/terra_billing_alert
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       38 2023-06-30 23:57:35.005793 terra_billing_alert-0.1.7/setup.cfg
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1694 2022-12-01 21:15:59.000000 terra_billing_alert-0.1.7/setup.py
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-06-30 23:57:35.001793 terra_billing_alert-0.1.7/terra_billing_alert/
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       22 2023-06-30 23:57:06.000000 terra_billing_alert-0.1.7/terra_billing_alert/__init__.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       61 2022-08-29 18:18:59.000000 terra_billing_alert-0.1.7/terra_billing_alert/__main__.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     4965 2022-12-01 21:15:59.000000 terra_billing_alert-0.1.7/terra_billing_alert/alert_item.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      730 2022-12-01 21:15:59.000000 terra_billing_alert-0.1.7/terra_billing_alert/alert_sender.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3962 2022-12-01 21:15:59.000000 terra_billing_alert-0.1.7/terra_billing_alert/bucket.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3422 2022-08-29 20:17:33.000000 terra_billing_alert-0.1.7/terra_billing_alert/cli.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      681 2022-08-29 18:18:59.000000 terra_billing_alert-0.1.7/terra_billing_alert/datetime_util.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    15275 2022-08-29 18:18:59.000000 terra_billing_alert-0.1.7/terra_billing_alert/gcp_machine_type.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6067 2022-12-01 21:15:59.000000 terra_billing_alert-0.1.7/terra_billing_alert/instance.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2595 2022-12-01 21:15:59.000000 terra_billing_alert-0.1.7/terra_billing_alert/terra_util.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6776 2023-06-30 23:55:49.000000 terra_billing_alert-0.1.7/terra_billing_alert/workflow.py
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-06-30 23:57:35.005793 terra_billing_alert-0.1.7/terra_billing_alert.egg-info/
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      519 2023-06-30 23:57:34.000000 terra_billing_alert-0.1.7/terra_billing_alert.egg-info/PKG-INFO
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      630 2023-06-30 23:57:34.000000 terra_billing_alert-0.1.7/terra_billing_alert.egg-info/SOURCES.txt
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)        1 2023-06-30 23:57:34.000000 terra_billing_alert-0.1.7/terra_billing_alert.egg-info/dependency_links.txt
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      123 2023-06-30 23:57:34.000000 terra_billing_alert-0.1.7/terra_billing_alert.egg-info/requires.txt
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       20 2023-06-30 23:57:34.000000 terra_billing_alert-0.1.7/terra_billing_alert.egg-info/top_level.txt
```

### Comparing `terra_billing_alert-0.1.6/LICENSE` & `terra_billing_alert-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `terra_billing_alert-0.1.6/PKG-INFO` & `terra_billing_alert-0.1.7/terra_billing_alert.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: terra_billing_alert
-Version: 0.1.6
+Name: terra-billing-alert
+Version: 0.1.7
 Summary: Terra Billing Alert script for Google Cloud Function
 Home-page: https://github.com/IGVF-DACC/terra-billing-alert
 Author: Jin wook Lee
 Author-email: leepc12@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `terra_billing_alert-0.1.6/README.md` & `terra_billing_alert-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `terra_billing_alert-0.1.6/setup.py` & `terra_billing_alert-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `terra_billing_alert-0.1.6/terra_billing_alert/alert_item.py` & `terra_billing_alert-0.1.7/terra_billing_alert/alert_item.py`

 * *Files identical despite different names*

### Comparing `terra_billing_alert-0.1.6/terra_billing_alert/alert_sender.py` & `terra_billing_alert-0.1.7/terra_billing_alert/alert_sender.py`

 * *Files identical despite different names*

### Comparing `terra_billing_alert-0.1.6/terra_billing_alert/bucket.py` & `terra_billing_alert-0.1.7/terra_billing_alert/bucket.py`

 * *Files identical despite different names*

### Comparing `terra_billing_alert-0.1.6/terra_billing_alert/cli.py` & `terra_billing_alert-0.1.7/terra_billing_alert/cli.py`

 * *Files identical despite different names*

### Comparing `terra_billing_alert-0.1.6/terra_billing_alert/datetime_util.py` & `terra_billing_alert-0.1.7/terra_billing_alert/datetime_util.py`

 * *Files identical despite different names*

### Comparing `terra_billing_alert-0.1.6/terra_billing_alert/gcp_machine_type.py` & `terra_billing_alert-0.1.7/terra_billing_alert/gcp_machine_type.py`

 * *Files identical despite different names*

### Comparing `terra_billing_alert-0.1.6/terra_billing_alert/instance.py` & `terra_billing_alert-0.1.7/terra_billing_alert/instance.py`

 * *Files identical despite different names*

### Comparing `terra_billing_alert-0.1.6/terra_billing_alert/terra_util.py` & `terra_billing_alert-0.1.7/terra_billing_alert/terra_util.py`

 * *Files identical despite different names*

### Comparing `terra_billing_alert-0.1.6/terra_billing_alert/workflow.py` & `terra_billing_alert-0.1.7/terra_billing_alert/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,17 @@
                 submit_time = get_utc_datetime_from_dict(
                     submission, 'submissionDate'
                 )
 
                 for workflow in get_all_workflows(
                     namespace, workspace, submission_id,
                 ):
+                    if not workflow or 'workflowId' not in workflow:
+                        logger.error(f'Could not get workflow for {submission_id} on {workspace}')
+                        continue
                     cost = workflow.get('cost') or 0.0
                     workflow_id = workflow['workflowId']
                     status = workflow['status']
                     wf_metadata = get_workflow_metadata(
                         namespace, workspace, submission_id, workflow_id
                     )
                     start_time = get_utc_datetime_from_dict(wf_metadata, 'start')
```

### Comparing `terra_billing_alert-0.1.6/terra_billing_alert.egg-info/PKG-INFO` & `terra_billing_alert-0.1.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: terra-billing-alert
-Version: 0.1.6
+Name: terra_billing_alert
+Version: 0.1.7
 Summary: Terra Billing Alert script for Google Cloud Function
 Home-page: https://github.com/IGVF-DACC/terra-billing-alert
 Author: Jin wook Lee
 Author-email: leepc12@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `terra_billing_alert-0.1.6/terra_billing_alert.egg-info/SOURCES.txt` & `terra_billing_alert-0.1.7/terra_billing_alert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

