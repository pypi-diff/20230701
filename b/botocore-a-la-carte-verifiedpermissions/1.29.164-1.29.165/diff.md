# Comparing `tmp/botocore-a-la-carte-verifiedpermissions-1.29.164.tar.gz` & `tmp/botocore-a-la-carte-verifiedpermissions-1.29.165.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-verifiedpermissions-1.29.164.tar", last modified: Fri Jun 30 01:39:17 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-verifiedpermissions-1.29.165.tar", last modified: Sat Jul  1 01:50:15 2023, max compression
```

## Comparing `botocore-a-la-carte-verifiedpermissions-1.29.164.tar` & `botocore-a-la-carte-verifiedpermissions-1.29.165.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:39:17.705726 botocore-a-la-carte-verifiedpermissions-1.29.164/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-30 01:39:17.000000 botocore-a-la-carte-verifiedpermissions-1.29.164/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-30 01:39:17.705726 botocore-a-la-carte-verifiedpermissions-1.29.164/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:39:17.701726 botocore-a-la-carte-verifiedpermissions-1.29.164/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:39:17.701726 botocore-a-la-carte-verifiedpermissions-1.29.164/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:39:17.701726 botocore-a-la-carte-verifiedpermissions-1.29.164/botocore/data/verifiedpermissions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:39:17.705726 botocore-a-la-carte-verifiedpermissions-1.29.164/botocore/data/verifiedpermissions/2021-12-01/
--rw-r--r--   0 runner    (1001) docker     (123)    17676 2023-06-30 01:38:31.000000 botocore-a-la-carte-verifiedpermissions-1.29.164/botocore/data/verifiedpermissions/2021-12-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-30 01:38:31.000000 botocore-a-la-carte-verifiedpermissions-1.29.164/botocore/data/verifiedpermissions/2021-12-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   125993 2023-06-30 01:38:31.000000 botocore-a-la-carte-verifiedpermissions-1.29.164/botocore/data/verifiedpermissions/2021-12-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 01:38:31.000000 botocore-a-la-carte-verifiedpermissions-1.29.164/botocore/data/verifiedpermissions/2021-12-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:39:17.705726 botocore-a-la-carte-verifiedpermissions-1.29.164/botocore_a_la_carte_verifiedpermissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-30 01:39:17.000000 botocore-a-la-carte-verifiedpermissions-1.29.164/botocore_a_la_carte_verifiedpermissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-30 01:39:17.000000 botocore-a-la-carte-verifiedpermissions-1.29.164/botocore_a_la_carte_verifiedpermissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 01:39:17.000000 botocore-a-la-carte-verifiedpermissions-1.29.164/botocore_a_la_carte_verifiedpermissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 01:39:17.000000 botocore-a-la-carte-verifiedpermissions-1.29.164/botocore_a_la_carte_verifiedpermissions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 01:39:17.705726 botocore-a-la-carte-verifiedpermissions-1.29.164/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-30 01:39:17.000000 botocore-a-la-carte-verifiedpermissions-1.29.164/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:50:15.814917 botocore-a-la-carte-verifiedpermissions-1.29.165/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-01 01:50:15.000000 botocore-a-la-carte-verifiedpermissions-1.29.165/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-01 01:50:15.814917 botocore-a-la-carte-verifiedpermissions-1.29.165/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:50:15.810917 botocore-a-la-carte-verifiedpermissions-1.29.165/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:50:15.810917 botocore-a-la-carte-verifiedpermissions-1.29.165/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:50:15.810917 botocore-a-la-carte-verifiedpermissions-1.29.165/botocore/data/verifiedpermissions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:50:15.814917 botocore-a-la-carte-verifiedpermissions-1.29.165/botocore/data/verifiedpermissions/2021-12-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    17676 2023-07-01 01:49:29.000000 botocore-a-la-carte-verifiedpermissions-1.29.165/botocore/data/verifiedpermissions/2021-12-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-01 01:49:29.000000 botocore-a-la-carte-verifiedpermissions-1.29.165/botocore/data/verifiedpermissions/2021-12-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   126009 2023-07-01 01:49:29.000000 botocore-a-la-carte-verifiedpermissions-1.29.165/botocore/data/verifiedpermissions/2021-12-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-01 01:49:29.000000 botocore-a-la-carte-verifiedpermissions-1.29.165/botocore/data/verifiedpermissions/2021-12-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:50:15.814917 botocore-a-la-carte-verifiedpermissions-1.29.165/botocore_a_la_carte_verifiedpermissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-01 01:50:15.000000 botocore-a-la-carte-verifiedpermissions-1.29.165/botocore_a_la_carte_verifiedpermissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-01 01:50:15.000000 botocore-a-la-carte-verifiedpermissions-1.29.165/botocore_a_la_carte_verifiedpermissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 01:50:15.000000 botocore-a-la-carte-verifiedpermissions-1.29.165/botocore_a_la_carte_verifiedpermissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-01 01:50:15.000000 botocore-a-la-carte-verifiedpermissions-1.29.165/botocore_a_la_carte_verifiedpermissions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 01:50:15.814917 botocore-a-la-carte-verifiedpermissions-1.29.165/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-01 01:50:15.000000 botocore-a-la-carte-verifiedpermissions-1.29.165/setup.py
```

### Comparing `botocore-a-la-carte-verifiedpermissions-1.29.164/LICENSE.txt` & `botocore-a-la-carte-verifiedpermissions-1.29.165/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-verifiedpermissions-1.29.164/PKG-INFO` & `botocore-a-la-carte-verifiedpermissions-1.29.165/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-verifiedpermissions
-Version: 1.29.164
+Version: 1.29.165
 Summary: verifiedpermissions data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-verifiedpermissions-1.29.164/botocore/data/verifiedpermissions/2021-12-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-verifiedpermissions-1.29.165/botocore/data/verifiedpermissions/2021-12-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-verifiedpermissions-1.29.164/botocore/data/verifiedpermissions/2021-12-01/paginators-1.json` & `botocore-a-la-carte-verifiedpermissions-1.29.165/botocore/data/verifiedpermissions/2021-12-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-verifiedpermissions-1.29.164/botocore/data/verifiedpermissions/2021-12-01/service-2.json` & `botocore-a-la-carte-verifiedpermissions-1.29.165/botocore/data/verifiedpermissions/2021-12-01/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999494653103808%*

 * *Differences: {"'shapes'": "{'CreateIdentitySourceInput': {'members': {'clientToken': {'documentation': "*

 * *             "'<p>Specifies a unique, case-sensitive ID that you provide to ensure the idempotency "*

 * *             'of the request. This lets you safely retry the request without accidentally '*

 * *             'performing the same operation a second time. Passing the same value to a later call '*

 * *             'to an operation requires that you also pass the same value for all other parameters. '*

 * *             'We recommend […]*

```diff
@@ -967,15 +967,15 @@
             "value": {
                 "shape": "AttributeValue"
             }
         },
         "CreateIdentitySourceInput": {
             "members": {
                 "clientToken": {
-                    "documentation": "<p>Specifies a unique, case-sensitive ID that you provide to ensure the idempotency of the request. This lets you safely retry the request without accidentally performing the same operation a second time. Passing the same value to a later call to an operation requires that you also pass the same value for all other parameters. We recommend that you use a <a href=\"https://wikipedia.org/wiki/Universally_unique_Id\">UUID type of value.</a>.</p> <p>If you don't provide this value, then Amazon Web Services generates a random one for you.</p> <p>If you retry the operation with the same <code>ClientToken</code>, but with different parameters, the retry fails with an <code>IdempotentParameterMismatch</code> error.</p>",
+                    "documentation": "<p>Specifies a unique, case-sensitive ID that you provide to ensure the idempotency of the request. This lets you safely retry the request without accidentally performing the same operation a second time. Passing the same value to a later call to an operation requires that you also pass the same value for all other parameters. We recommend that you use a <a href=\"https://wikipedia.org/wiki/Universally_unique_identifier\">UUID type of value.</a>.</p> <p>If you don't provide this value, then Amazon Web Services generates a random one for you.</p> <p>If you retry the operation with the same <code>ClientToken</code>, but with different parameters, the retry fails with an <code>IdempotentParameterMismatch</code> error.</p>",
                     "idempotencyToken": true,
                     "shape": "IdempotencyToken"
                 },
                 "configuration": {
                     "documentation": "<p>Specifies the details required to communicate with the identity provider (IdP) associated with this identity source.</p> <note> <p>At this time, the only valid member of this structure is a Amazon Cognito user pool configuration.</p> <p>You must specify a <code>UserPoolArn</code>, and optionally, a <code>ClientId</code>.</p> </note>",
                     "shape": "Configuration"
                 },
@@ -1020,15 +1020,15 @@
                 "policyStoreId"
             ],
             "type": "structure"
         },
         "CreatePolicyInput": {
             "members": {
                 "clientToken": {
-                    "documentation": "<p>Specifies a unique, case-sensitive ID that you provide to ensure the idempotency of the request. This lets you safely retry the request without accidentally performing the same operation a second time. Passing the same value to a later call to an operation requires that you also pass the same value for all other parameters. We recommend that you use a <a href=\"https://wikipedia.org/wiki/Universally_unique_Id\">UUID type of value.</a>.</p> <p>If you don't provide this value, then Amazon Web Services generates a random one for you.</p> <p>If you retry the operation with the same <code>ClientToken</code>, but with different parameters, the retry fails with an <code>IdempotentParameterMismatch</code> error.</p>",
+                    "documentation": "<p>Specifies a unique, case-sensitive ID that you provide to ensure the idempotency of the request. This lets you safely retry the request without accidentally performing the same operation a second time. Passing the same value to a later call to an operation requires that you also pass the same value for all other parameters. We recommend that you use a <a href=\"https://wikipedia.org/wiki/Universally_unique_identifier\">UUID type of value.</a>.</p> <p>If you don't provide this value, then Amazon Web Services generates a random one for you.</p> <p>If you retry the operation with the same <code>ClientToken</code>, but with different parameters, the retry fails with an <code>IdempotentParameterMismatch</code> error.</p>",
                     "idempotencyToken": true,
                     "shape": "IdempotencyToken"
                 },
                 "definition": {
                     "documentation": "<p>A structure that specifies the policy type and content to use for the new policy. You must include either a static or a templateLinked element. The policy content must be written in the Cedar policy language.</p>",
                     "shape": "PolicyDefinition"
                 },
@@ -1082,15 +1082,15 @@
                 "lastUpdatedDate"
             ],
             "type": "structure"
         },
         "CreatePolicyStoreInput": {
             "members": {
                 "clientToken": {
-                    "documentation": "<p>Specifies a unique, case-sensitive ID that you provide to ensure the idempotency of the request. This lets you safely retry the request without accidentally performing the same operation a second time. Passing the same value to a later call to an operation requires that you also pass the same value for all other parameters. We recommend that you use a <a href=\"https://wikipedia.org/wiki/Universally_unique_Id\">UUID type of value.</a>.</p> <p>If you don't provide this value, then Amazon Web Services generates a random one for you.</p> <p>If you retry the operation with the same <code>ClientToken</code>, but with different parameters, the retry fails with an <code>IdempotentParameterMismatch</code> error.</p>",
+                    "documentation": "<p>Specifies a unique, case-sensitive ID that you provide to ensure the idempotency of the request. This lets you safely retry the request without accidentally performing the same operation a second time. Passing the same value to a later call to an operation requires that you also pass the same value for all other parameters. We recommend that you use a <a href=\"https://wikipedia.org/wiki/Universally_unique_identifier\">UUID type of value.</a>.</p> <p>If you don't provide this value, then Amazon Web Services generates a random one for you.</p> <p>If you retry the operation with the same <code>ClientToken</code>, but with different parameters, the retry fails with an <code>IdempotentParameterMismatch</code> error.</p>",
                     "idempotencyToken": true,
                     "shape": "IdempotencyToken"
                 },
                 "validationSettings": {
                     "documentation": "<p>Specifies the validation setting for this policy store.</p> <p>Currently, the only valid and required value is <code>Mode</code>.</p> <important> <p>We recommend that you turn on <code>STRICT</code> mode only after you define a schema. If a schema doesn't exist, then <code>STRICT</code> mode causes any policy to fail validation, and Verified Permissions rejects the policy. You can turn off validation by using the <a href=\"https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_UpdatePolicyStore\">UpdatePolicyStore</a>. Then, when you have a schema defined, use <a href=\"https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_UpdatePolicyStore\">UpdatePolicyStore</a> again to turn validation back on.</p> </important>",
                     "shape": "ValidationSettings"
                 }
@@ -1126,15 +1126,15 @@
                 "lastUpdatedDate"
             ],
             "type": "structure"
         },
         "CreatePolicyTemplateInput": {
             "members": {
                 "clientToken": {
-                    "documentation": "<p>Specifies a unique, case-sensitive ID that you provide to ensure the idempotency of the request. This lets you safely retry the request without accidentally performing the same operation a second time. Passing the same value to a later call to an operation requires that you also pass the same value for all other parameters. We recommend that you use a <a href=\"https://wikipedia.org/wiki/Universally_unique_Id\">UUID type of value.</a>.</p> <p>If you don't provide this value, then Amazon Web Services generates a random one for you.</p> <p>If you retry the operation with the same <code>ClientToken</code>, but with different parameters, the retry fails with an <code>IdempotentParameterMismatch</code> error.</p>",
+                    "documentation": "<p>Specifies a unique, case-sensitive ID that you provide to ensure the idempotency of the request. This lets you safely retry the request without accidentally performing the same operation a second time. Passing the same value to a later call to an operation requires that you also pass the same value for all other parameters. We recommend that you use a <a href=\"https://wikipedia.org/wiki/Universally_unique_identifier\">UUID type of value.</a>.</p> <p>If you don't provide this value, then Amazon Web Services generates a random one for you.</p> <p>If you retry the operation with the same <code>ClientToken</code>, but with different parameters, the retry fails with an <code>IdempotentParameterMismatch</code> error.</p>",
                     "idempotencyToken": true,
                     "shape": "IdempotencyToken"
                 },
                 "description": {
                     "documentation": "<p>Specifies a description for the policy template.</p>",
                     "shape": "PolicyTemplateDescription"
                 },
@@ -1382,15 +1382,15 @@
         "EntityType": {
             "max": 200,
             "min": 1,
             "pattern": ".*",
             "type": "string"
         },
         "EvaluationErrorItem": {
-            "documentation": "<p>Contains a description of an evaluation error.</p> <p>This data type is used as a request parameter in the <a href=\"https://docs.aws.amazon.com/amazon-verified-permissions/latest/APIReference/API_IsAuthorized.html\">IsAuthorized</a> and <a href=\"https://docs.aws.amazon.com/amazon-verified-permissions/latest/APIReference/API_IsAuthorizedWithToken.html\">IsAuthorizedWithToken</a> operations.</p>",
+            "documentation": "<p>Contains a description of an evaluation error.</p> <p>This data type is used as a request parameter in the <a href=\"https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_IsAuthorized.html\">IsAuthorized</a> and <a href=\"https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_IsAuthorizedWithToken.html\">IsAuthorizedWithToken</a> operations.</p>",
             "members": {
                 "errorDescription": {
                     "documentation": "<p>The error description.</p>",
                     "shape": "String"
                 }
             },
             "required": [
```

### Comparing `botocore-a-la-carte-verifiedpermissions-1.29.164/botocore_a_la_carte_verifiedpermissions.egg-info/PKG-INFO` & `botocore-a-la-carte-verifiedpermissions-1.29.165/botocore_a_la_carte_verifiedpermissions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-verifiedpermissions
-Version: 1.29.164
+Version: 1.29.165
 Summary: verifiedpermissions data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-verifiedpermissions-1.29.164/botocore_a_la_carte_verifiedpermissions.egg-info/SOURCES.txt` & `botocore-a-la-carte-verifiedpermissions-1.29.165/botocore_a_la_carte_verifiedpermissions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-verifiedpermissions-1.29.164/setup.py` & `botocore-a-la-carte-verifiedpermissions-1.29.165/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-verifiedpermissions',
-    version="1.29.164",
+    version="1.29.165",
     description='verifiedpermissions data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/verifiedpermissions/*/*.json'],
```

