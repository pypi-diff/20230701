# Comparing `tmp/iam_actions-1.2.20230630.tar.gz` & `tmp/iam_actions-1.2.20230701.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230630.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230701.tar", max compression
```

## Comparing `iam_actions-1.2.20230630.tar` & `iam_actions-1.2.20230701.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/LICENSE
--rw-r--r--   0        0        0     2302 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/README.md
--rw-r--r--   0        0        0      228 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/iam_actions/__init__.py
--rw-r--r--   0        0        0  4360093 2023-06-30 02:47:51.000463 iam_actions-1.2.20230630/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/iam_actions/generate/services.py
--rw-r--r--   0        0        0   560805 2023-06-30 02:47:51.000463 iam_actions-1.2.20230630/iam_actions/policies.json
--rw-r--r--   0        0        0   197240 2023-06-30 02:47:51.000463 iam_actions-1.2.20230630/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   543926 2023-06-30 02:47:51.000463 iam_actions-1.2.20230630/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-06-30 02:47:51.880422 iam_actions-1.2.20230630/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230630/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230630/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-01 03:00:50.105448 iam_actions-1.2.20230701/LICENSE
+-rw-r--r--   0        0        0     2302 2023-07-01 03:00:50.105448 iam_actions-1.2.20230701/README.md
+-rw-r--r--   0        0        0      228 2023-07-01 03:00:50.105448 iam_actions-1.2.20230701/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4362506 2023-07-01 03:02:47.346267 iam_actions-1.2.20230701/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-07-01 03:00:50.105448 iam_actions-1.2.20230701/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-07-01 03:00:50.105448 iam_actions-1.2.20230701/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-07-01 03:00:50.105448 iam_actions-1.2.20230701/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-07-01 03:00:50.105448 iam_actions-1.2.20230701/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-07-01 03:00:50.105448 iam_actions-1.2.20230701/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-07-01 03:00:50.105448 iam_actions-1.2.20230701/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-07-01 03:00:50.105448 iam_actions-1.2.20230701/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-07-01 03:00:50.105448 iam_actions-1.2.20230701/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   560956 2023-07-01 03:02:47.346267 iam_actions-1.2.20230701/iam_actions/policies.json
+-rw-r--r--   0        0        0   197380 2023-07-01 03:02:47.346267 iam_actions-1.2.20230701/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   544073 2023-07-01 03:02:47.346267 iam_actions-1.2.20230701/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-07-01 03:02:48.290336 iam_actions-1.2.20230701/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230701/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230701/PKG-INFO
```

### Comparing `iam_actions-1.2.20230630/LICENSE` & `iam_actions-1.2.20230701/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230630/README.md` & `iam_actions-1.2.20230701/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230630/iam_actions/actions.json` & `iam_actions-1.2.20230701/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999305779119417%*

 * *Differences: {"'appstream'": "{'TagResource': {'resources': {insert: [(1, 'app-block-builder')]}}, "*

 * *                "'UntagResource': {'resources': {insert: [(1, 'app-block-builder')]}}, "*

 * *                "'CreateAppBlockBuilderStreamingURL': {'access_level': 'Write', 'condition_keys': "*

 * *                "['aws:ResourceTag/${TagKey}'], 'description': 'Grants permission to create a URL "*

 * *                "to start an app block builder streaming session', 'resources': "*

 * *                "['app-block-builder']}, 'StartAppBlo […]*

```diff
@@ -6360,20 +6360,25 @@
             "resources": [
                 "vpcingressconnection"
             ]
         }
     },
     "appstream": {
         "AssociateAppBlockBuilderAppBlock": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateAppBlockBuilderAppBlock",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to associate the specified app block builder with the app block",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "app-block",
+                "app-block-builder"
+            ]
         },
         "AssociateApplicationFleet": {
             "access_level": "Write",
             "action": "AssociateApplicationFleet",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
@@ -6452,28 +6457,37 @@
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create an app block. App blocks store details about the virtual hard disk that contains the files for the application in an S3 bucket. It also stores the setup script with details about how to mount the virtual hard disk. App blocks are only supported for Elastic fleets",
             "orphan": false,
             "resources": []
         },
         "CreateAppBlockBuilder": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateAppBlockBuilder",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create an app block builder. An app block builder is a virtual machine that is used to create an app block",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "app-block-builder"
+            ]
         },
         "CreateAppBlockBuilderStreamingURL": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateAppBlockBuilderStreamingURL",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to create a URL to start an app block builder streaming session",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "app-block-builder"
+            ]
         },
         "CreateApplication": {
             "access_level": "Write",
             "action": "CreateApplication",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
@@ -6608,20 +6622,24 @@
             "description": "Grants permission to delete the specified app block",
             "orphan": false,
             "resources": [
                 "app-block"
             ]
         },
         "DeleteAppBlockBuilder": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteAppBlockBuilder",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to delete the specified app block builder and release capacity",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "app-block-builder"
+            ]
         },
         "DeleteApplication": {
             "access_level": "Write",
             "action": "DeleteApplication",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
@@ -6722,28 +6740,33 @@
             "action": "DeleteUser",
             "condition_keys": [],
             "description": "Grants permission to delete a user from the user pool",
             "orphan": false,
             "resources": []
         },
         "DescribeAppBlockBuilderAppBlockAssociations": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeAppBlockBuilderAppBlockAssociations",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve the associations that are associated with the specified app block builder or app block",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "app-block",
+                "app-block-builder"
+            ]
         },
         "DescribeAppBlockBuilders": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeAppBlockBuilders",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve a list that describes one or more specified app block builders, if the app block builder names are provided. Otherwise, all app block builders in the account are described",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "app-block-builder"
+            ]
         },
         "DescribeAppBlocks": {
             "access_level": "Read",
             "action": "DescribeAppBlocks",
             "condition_keys": [],
             "description": "Grants permission to retrieve a list that describes one or more specified app blocks, if the app block arns are provided. Otherwise, all app blocks in the account are described",
             "orphan": false,
@@ -6882,20 +6905,25 @@
             "action": "DisableUser",
             "condition_keys": [],
             "description": "Grants permission to disable the specified user in the user pool. This action does not delete the user",
             "orphan": false,
             "resources": []
         },
         "DisassociateAppBlockBuilderAppBlock": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateAppBlockBuilderAppBlock",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to disassociate the specified app block builder with the app block",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "app-block",
+                "app-block-builder"
+            ]
         },
         "DisassociateApplicationFleet": {
             "access_level": "Write",
             "action": "DisassociateApplicationFleet",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
@@ -6980,20 +7008,24 @@
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Grants permission to retrieve a list of all tags for the specified AppStream 2.0 resource. The following resources can be tagged: Image builders, images, fleets, and stacks",
             "orphan": false,
             "resources": []
         },
         "StartAppBlockBuilder": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartAppBlockBuilder",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to start the specified app block builder",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "app-block-builder"
+            ]
         },
         "StartFleet": {
             "access_level": "Write",
             "action": "StartFleet",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
@@ -7012,20 +7044,24 @@
             "description": "Grants permission to start the specified image builder",
             "orphan": false,
             "resources": [
                 "image-builder"
             ]
         },
         "StopAppBlockBuilder": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StopAppBlockBuilder",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to stop the specified app block builder",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "app-block-builder"
+            ]
         },
         "StopFleet": {
             "access_level": "Write",
             "action": "StopFleet",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
@@ -7067,14 +7103,15 @@
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to add or overwrite one or more tags for the specified AppStream 2.0 resource. The following resources can be tagged: Image builders, images, fleets, stacks, app blocks and applications",
             "orphan": false,
             "resources": [
                 "app-block",
+                "app-block-builder",
                 "application",
                 "fleet",
                 "image",
                 "image-builder",
                 "stack"
             ]
         },
@@ -7084,28 +7121,33 @@
             "condition_keys": [
                 "aws:TagKeys"
             ],
             "description": "Grants permission to disassociate one or more tags from the specified AppStream 2.0 resource",
             "orphan": false,
             "resources": [
                 "app-block",
+                "app-block-builder",
                 "application",
                 "fleet",
                 "image",
                 "image-builder",
                 "stack"
             ]
         },
         "UpdateAppBlockBuilder": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateAppBlockBuilder",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to update a specific app block builder. An app block builder is a virtual machine that is used to create an app block",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "app-block-builder"
+            ]
         },
         "UpdateApplication": {
             "access_level": "Write",
             "action": "UpdateApplication",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
@@ -57830,18 +57872,18 @@
             "action": "ListStudios",
             "condition_keys": [],
             "description": "Grants permission to list summary information about EMR Studios",
             "orphan": false,
             "resources": []
         },
         "ListSupportedInstanceTypes": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListSupportedInstanceTypes",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list the Amazon EC2 instance types that an Amazon EMR release supports",
             "orphan": false,
             "resources": []
         },
         "ListWorkspaceAccessIdentities": {
             "access_level": "List",
             "action": "ListWorkspaceAccessIdentities",
             "condition_keys": [],
@@ -115682,14 +115724,22 @@
             ],
             "description": "Grants permission to automatically create the specified Amazon Redshift user if it does not exist",
             "orphan": false,
             "resources": [
                 "dbuser"
             ]
         },
+        "CreateCustomDomainAssociation": {
+            "access_level": "Undocumented",
+            "action": "CreateCustomDomainAssociation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateEndpointAccess": {
             "access_level": "Write",
             "action": "CreateEndpointAccess",
             "condition_keys": [],
             "description": "Grants permission to create a redshift-managed vpc endpoint",
             "orphan": false,
             "resources": []
@@ -115882,14 +115932,22 @@
             "condition_keys": [],
             "description": "Grants permission to delete a cluster subnet group",
             "orphan": false,
             "resources": [
                 "subnetgroup"
             ]
         },
+        "DeleteCustomDomainAssociation": {
+            "access_level": "Undocumented",
+            "action": "DeleteCustomDomainAssociation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteEndpointAccess": {
             "access_level": "Write",
             "action": "DeleteEndpointAccess",
             "condition_keys": [],
             "description": "Grants permission to delete a redshift-managed vpc endpoint",
             "orphan": false,
             "resources": []
@@ -116091,14 +116149,22 @@
             "access_level": "List",
             "action": "DescribeClusters",
             "condition_keys": [],
             "description": "Grants permission to describe properties of provisioned clusters",
             "orphan": false,
             "resources": []
         },
+        "DescribeCustomDomainAssociations": {
+            "access_level": "Undocumented",
+            "action": "DescribeCustomDomainAssociations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeDataShares": {
             "access_level": "Read",
             "action": "DescribeDataShares",
             "condition_keys": [],
             "description": "Grants permission to describe datashares created and consumed by your clusters",
             "orphan": false,
             "resources": []
@@ -116599,14 +116665,22 @@
             "condition_keys": [],
             "description": "Grants permission to modify a cluster subnet group to include the specified list of VPC subnets",
             "orphan": false,
             "resources": [
                 "subnetgroup"
             ]
         },
+        "ModifyCustomDomainAssociation": {
+            "access_level": "Undocumented",
+            "action": "ModifyCustomDomainAssociation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ModifyEndpointAccess": {
             "access_level": "Write",
             "action": "ModifyEndpointAccess",
             "condition_keys": [],
             "description": "Grants permission to modify a redshift-managed vpc endpoint",
             "orphan": false,
             "resources": []
```

### Comparing `iam_actions-1.2.20230630/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230701/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230630/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230701/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230630/iam_actions/generate/generate.py` & `iam_actions-1.2.20230701/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230630/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230701/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230630/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230701/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230630/iam_actions/generate/services.py` & `iam_actions-1.2.20230701/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230630/iam_actions/policies.json` & `iam_actions-1.2.20230701/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999996889386586%*

 * *Differences: {"'serviceMap'": "{'Amazon Redshift': {'Actions': {insert: [(20, 'CreateCustomDomainAssociation'), "*

 * *                 "(38, 'DeleteCustomDomainAssociation'), (61, 'DescribeCustomDomainAssociations'), "*

 * *                 "(117, 'ModifyCustomDomainAssociation')]}}}"}*

```diff
@@ -17493,14 +17493,15 @@
                 "CreateAuthenticationProfile",
                 "CreateCluster",
                 "CreateClusterParameterGroup",
                 "CreateClusterSecurityGroup",
                 "CreateClusterSnapshot",
                 "CreateClusterSubnetGroup",
                 "CreateClusterUser",
+                "CreateCustomDomainAssociation",
                 "CreateEndpointAccess",
                 "CreateEventSubscription",
                 "CreateHsmClientCertificate",
                 "CreateHsmConfiguration",
                 "CreateSavedQuery",
                 "CreateScheduledAction",
                 "CreateSnapshotCopyGrant",
@@ -17510,14 +17511,15 @@
                 "DeauthorizeDataShare",
                 "DeleteAuthenticationProfile",
                 "DeleteCluster",
                 "DeleteClusterParameterGroup",
                 "DeleteClusterSecurityGroup",
                 "DeleteClusterSnapshot",
                 "DeleteClusterSubnetGroup",
+                "DeleteCustomDomainAssociation",
                 "DeleteEndpointAccess",
                 "DeleteEventSubscription",
                 "DeleteHsmClientCertificate",
                 "DeleteHsmConfiguration",
                 "DeletePartner",
                 "DeleteSavedQueries",
                 "DeleteScheduledAction",
@@ -17532,14 +17534,15 @@
                 "DescribeClusterParameters",
                 "DescribeClusterSecurityGroups",
                 "DescribeClusterSnapshots",
                 "DescribeClusterSubnetGroups",
                 "DescribeClusterTracks",
                 "DescribeClusterVersions",
                 "DescribeClusters",
+                "DescribeCustomDomainAssociations",
                 "DescribeDataShares",
                 "DescribeDataSharesForConsumer",
                 "DescribeDataSharesForProducer",
                 "DescribeDefaultClusterParameters",
                 "DescribeEndpointAccess",
                 "DescribeEndpointAuthorization",
                 "DescribeEventCategories",
@@ -17587,14 +17590,15 @@
                 "ModifyClusterDbRevision",
                 "ModifyClusterIamRoles",
                 "ModifyClusterMaintenance",
                 "ModifyClusterParameterGroup",
                 "ModifyClusterSnapshot",
                 "ModifyClusterSnapshotSchedule",
                 "ModifyClusterSubnetGroup",
+                "ModifyCustomDomainAssociation",
                 "ModifyEndpointAccess",
                 "ModifyEventSubscription",
                 "ModifySavedQuery",
                 "ModifyScheduledAction",
                 "ModifySnapshotCopyRetentionPeriod",
                 "ModifySnapshotSchedule",
                 "ModifyUsageLimit",
```

### Comparing `iam_actions-1.2.20230630/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230701/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998032270759544%*

 * *Differences: {"'appstream'": "{'app-block-builder': OrderedDict([('arn_pattern', "*

 * *                "'arn:*:appstream:*:*:app-block-builder/*'), ('condition_keys', "*

 * *                "'aws:ResourceTag/${TagKey}')])}"}*

```diff
@@ -581,14 +581,18 @@
         }
     },
     "appstream": {
         "app-block": {
             "arn_pattern": "arn:*:appstream:*:*:app-block/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "app-block-builder": {
+            "arn_pattern": "arn:*:appstream:*:*:app-block-builder/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "application": {
             "arn_pattern": "arn:*:appstream:*:*:application/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "fleet": {
             "arn_pattern": "arn:*:appstream:*:*:fleet/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
```

### Comparing `iam_actions-1.2.20230630/iam_actions/services.json` & `iam_actions-1.2.20230701/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999967437104768%*

 * *Differences: {"'redshift'": "{'Actions': {insert: [(20, 'CreateCustomDomainAssociation'), (38, "*

 * *               "'DeleteCustomDomainAssociation'), (61, 'DescribeCustomDomainAssociations'), (117, "*

 * *               "'ModifyCustomDomainAssociation')]}}"}*

```diff
@@ -16213,14 +16213,15 @@
             "CreateAuthenticationProfile",
             "CreateCluster",
             "CreateClusterParameterGroup",
             "CreateClusterSecurityGroup",
             "CreateClusterSnapshot",
             "CreateClusterSubnetGroup",
             "CreateClusterUser",
+            "CreateCustomDomainAssociation",
             "CreateEndpointAccess",
             "CreateEventSubscription",
             "CreateHsmClientCertificate",
             "CreateHsmConfiguration",
             "CreateSavedQuery",
             "CreateScheduledAction",
             "CreateSnapshotCopyGrant",
@@ -16230,14 +16231,15 @@
             "DeauthorizeDataShare",
             "DeleteAuthenticationProfile",
             "DeleteCluster",
             "DeleteClusterParameterGroup",
             "DeleteClusterSecurityGroup",
             "DeleteClusterSnapshot",
             "DeleteClusterSubnetGroup",
+            "DeleteCustomDomainAssociation",
             "DeleteEndpointAccess",
             "DeleteEventSubscription",
             "DeleteHsmClientCertificate",
             "DeleteHsmConfiguration",
             "DeletePartner",
             "DeleteSavedQueries",
             "DeleteScheduledAction",
@@ -16252,14 +16254,15 @@
             "DescribeClusterParameters",
             "DescribeClusterSecurityGroups",
             "DescribeClusterSnapshots",
             "DescribeClusterSubnetGroups",
             "DescribeClusterTracks",
             "DescribeClusterVersions",
             "DescribeClusters",
+            "DescribeCustomDomainAssociations",
             "DescribeDataShares",
             "DescribeDataSharesForConsumer",
             "DescribeDataSharesForProducer",
             "DescribeDefaultClusterParameters",
             "DescribeEndpointAccess",
             "DescribeEndpointAuthorization",
             "DescribeEventCategories",
@@ -16307,14 +16310,15 @@
             "ModifyClusterDbRevision",
             "ModifyClusterIamRoles",
             "ModifyClusterMaintenance",
             "ModifyClusterParameterGroup",
             "ModifyClusterSnapshot",
             "ModifyClusterSnapshotSchedule",
             "ModifyClusterSubnetGroup",
+            "ModifyCustomDomainAssociation",
             "ModifyEndpointAccess",
             "ModifyEventSubscription",
             "ModifySavedQuery",
             "ModifyScheduledAction",
             "ModifySnapshotCopyRetentionPeriod",
             "ModifySnapshotSchedule",
             "ModifyUsageLimit",
```

### Comparing `iam_actions-1.2.20230630/pyproject.toml` & `iam_actions-1.2.20230701/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230630"
+version = "1.2.20230701"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230630/setup.py` & `iam_actions-1.2.20230701/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230630',
+    'version': '1.2.20230701',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230630/PKG-INFO` & `iam_actions-1.2.20230701/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230630
+Version: 1.2.20230701
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

