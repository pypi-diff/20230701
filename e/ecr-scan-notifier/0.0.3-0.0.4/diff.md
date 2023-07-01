# Comparing `tmp/ecr-scan-notifier-0.0.3.tar.gz` & `tmp/ecr-scan-notifier-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecr-scan-notifier-0.0.3.tar", last modified: Mon Jun 26 16:05:30 2023, max compression
+gzip compressed data, was "ecr-scan-notifier-0.0.4.tar", last modified: Sat Jul  1 06:37:05 2023, max compression
```

## Comparing `ecr-scan-notifier-0.0.3.tar` & `ecr-scan-notifier-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.836645 ecr-scan-notifier-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-26 16:05:18.000000 ecr-scan-notifier-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 16:05:18.000000 ecr-scan-notifier-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-26 16:05:30.836645 ecr-scan-notifier-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-26 16:05:18.000000 ecr-scan-notifier-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 16:05:18.000000 ecr-scan-notifier-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 16:05:30.836645 ecr-scan-notifier-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-26 16:05:18.000000 ecr-scan-notifier-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.832644 ecr-scan-notifier-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.832644 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier/
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-26 16:05:18.000000 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.832644 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-26 16:05:18.000000 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-06-26 16:05:18.000000 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier/_jsii/ecr-scan-notifier@0.0.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:05:18.000000 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.832644 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-26 16:05:30.000000 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-26 16:05:30.000000 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:05:30.000000 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 16:05:30.000000 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 16:05:30.000000 ecr-scan-notifier-0.0.3/src/ecr_scan_notifier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:37:05.328072 ecr-scan-notifier-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-01 06:36:49.000000 ecr-scan-notifier-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-01 06:36:49.000000 ecr-scan-notifier-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-01 06:37:05.328072 ecr-scan-notifier-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-01 06:36:49.000000 ecr-scan-notifier-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-01 06:36:49.000000 ecr-scan-notifier-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 06:37:05.328072 ecr-scan-notifier-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-01 06:36:49.000000 ecr-scan-notifier-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:37:05.328072 ecr-scan-notifier-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:37:05.328072 ecr-scan-notifier-0.0.4/src/ecr_scan_notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-01 06:36:49.000000 ecr-scan-notifier-0.0.4/src/ecr_scan_notifier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:37:05.328072 ecr-scan-notifier-0.0.4/src/ecr_scan_notifier/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-01 06:36:49.000000 ecr-scan-notifier-0.0.4/src/ecr_scan_notifier/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23665 2023-07-01 06:36:49.000000 ecr-scan-notifier-0.0.4/src/ecr_scan_notifier/_jsii/ecr-scan-notifier@0.0.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 06:36:49.000000 ecr-scan-notifier-0.0.4/src/ecr_scan_notifier/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:37:05.328072 ecr-scan-notifier-0.0.4/src/ecr_scan_notifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-01 06:37:05.000000 ecr-scan-notifier-0.0.4/src/ecr_scan_notifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-01 06:37:05.000000 ecr-scan-notifier-0.0.4/src/ecr_scan_notifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 06:37:05.000000 ecr-scan-notifier-0.0.4/src/ecr_scan_notifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-01 06:37:05.000000 ecr-scan-notifier-0.0.4/src/ecr_scan_notifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-01 06:37:05.000000 ecr-scan-notifier-0.0.4/src/ecr_scan_notifier.egg-info/top_level.txt
```

### Comparing `ecr-scan-notifier-0.0.3/LICENSE` & `ecr-scan-notifier-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ecr-scan-notifier-0.0.3/PKG-INFO` & `ecr-scan-notifier-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecr-scan-notifier
-Version: 0.0.3
+Version: 0.0.4
 Summary: Notifies on new AWS ECR scan results
 Home-page: https://github.com/stefanfreitag/cdk-ecr-scan-notifier.git
 Author: Stefan Freitag<stefan.freitag@rwe.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/cdk-ecr-scan-notifier.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `ecr-scan-notifier-0.0.3/README.md` & `ecr-scan-notifier-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ecr-scan-notifier-0.0.3/setup.py` & `ecr-scan-notifier-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ecr-scan-notifier",
-    "version": "0.0.3",
+    "version": "0.0.4",
     "description": "Notifies on new AWS ECR scan results",
     "license": "Apache-2.0",
     "url": "https://github.com/stefanfreitag/cdk-ecr-scan-notifier.git",
     "long_description_content_type": "text/markdown",
     "author": "Stefan Freitag<stefan.freitag@rwe.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "ecr_scan_notifier",
         "ecr_scan_notifier._jsii"
     ],
     "package_data": {
         "ecr_scan_notifier._jsii": [
-            "ecr-scan-notifier@0.0.3.jsii.tgz"
+            "ecr-scan-notifier@0.0.4.jsii.tgz"
         ],
         "ecr_scan_notifier": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `ecr-scan-notifier-0.0.3/src/ecr_scan_notifier/__init__.py` & `ecr-scan-notifier-0.0.4/src/ecr_scan_notifier/__init__.py`

 * *Files identical despite different names*

### Comparing `ecr-scan-notifier-0.0.3/src/ecr_scan_notifier/_jsii/ecr-scan-notifier@0.0.3.jsii.tgz` & `ecr-scan-notifier-0.0.4/src/ecr_scan_notifier/_jsii/ecr-scan-notifier@0.0.4.jsii.tgz`

 * *Files 25% similar despite different names*

#### Comparing `ecr-scan-notifier@0.0.3.jsii.tgz-content` & `ecr-scan-notifier@0.0.4.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'fingerprint'": "'faiZoXRbs6gVoyvIKsdBk7Ir5ZWnrqN2evQepam/SSQ='", "'version'": "'0.0.4'"}*

```diff
@@ -3460,15 +3460,15 @@
             }
         }
     },
     "description": "Notifies on new AWS ECR scan results",
     "docs": {
         "stability": "stable"
     },
-    "fingerprint": "4Y5I08/mv5rLPgfi9vM9GzfLbJJ5bDBMTzhwP4ok1lM=",
+    "fingerprint": "faiZoXRbs6gVoyvIKsdBk7Ir5ZWnrqN2evQepam/SSQ=",
     "homepage": "https://github.com/stefanfreitag/cdk-ecr-scan-notifier.git",
     "jsiiVersion": "1.84.0 (build 5404dcf)",
     "keywords": [
         "aws",
         "cdk",
         "ecr",
         "sns"
@@ -3648,9 +3648,9 @@
                         "fqn": "aws-cdk-lib.aws_logs.RetentionDays"
                     }
                 }
             ],
             "symbolId": "src/ecrScanNotifierProperties:EcrScanNotifierProperties"
         }
     },
-    "version": "0.0.3"
+    "version": "0.0.4"
 }
```

##### package/lib/ecrScanNotifier.js

###### js-beautify {}

```diff
@@ -81,10 +81,10 @@
         return fn;
     }
 }
 exports.EcrScanNotifier = EcrScanNotifier;
 _a = JSII_RTTI_SYMBOL_1;
 EcrScanNotifier[_a] = {
     fqn: "ecr-scan-notifier.EcrScanNotifier",
-    version: "0.0.3"
+    version: "0.0.4"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiZWNyU2Nhbk5vdGlmaWVyLmpzIiwic291cmNlUm9vdCI6IiIsInNvdXJjZXMiOlsiLi4vc3JjL2VjclNjYW5Ob3RpZmllci50cyJdLCJuYW1lcyI6W10sIm1hcHBpbmdzIjoiOzs7OztBQUFBLGlEQUF5QztBQUN6Qyw2QkFBNkI7QUFFN0IsNkNBQXVDO0FBQ3ZDLHVEQUE4QztBQUM5Qyx1RUFBZ0U7QUFDaEUsaURBQXNFO0FBQ3RFLHVEQUFpRTtBQUNqRSxtREFBcUQ7QUFDckQsMkNBQXVDO0FBR3ZDLE1BQWEsZUFBZ0IsU0FBUSxzQkFBUztJQUc1QyxZQUFZLEtBQWdCLEVBQUUsRUFBVSxFQUFFLEtBQWdDO1FBQ3hFLEtBQUssQ0FBQyxLQUFLLEVBQUUsRUFBRSxDQUFDLENBQUM7UUFFakIsSUFBSSxDQUFDLEtBQUssR0FBRyxLQUFLLENBQUM7UUFDbkIsTUFBTSxPQUFPLEdBQUcsSUFBSSxDQUFDLGNBQWMsRUFBRSxDQUFDO1FBRXRDLE1BQU0sYUFBYSxHQUFHLElBQUksbUNBQWMsQ0FBQyxPQUFPLENBQUMsQ0FBQztRQUNsRCxJQUFJLGlCQUFJLENBQUMsSUFBSSxFQUFFLHNCQUFzQixFQUFFO1lBQ3JDLFFBQVEsRUFBRSwwQkFBMEI7WUFDcEMsV0FBVyxFQUFFLHlEQUF5RDtZQUN0RSxPQUFPLEVBQUUsQ0FBQyxhQUFhLENBQUM7WUFDeEIsWUFBWSxFQUFFO2dCQUNaLE1BQU0sRUFBRSxDQUFDLFNBQVMsRUFBRSxnQkFBZ0IsQ0FBQztnQkFDckMsVUFBVSxFQUFFLENBQUMsZ0JBQWdCLEVBQUUsaUJBQWlCLENBQUM7YUFDbEQ7U0FDRixDQUFDLENBQUM7SUFDTCxDQUFDO0lBQ08sY0FBYztRQUNwQixNQUFNLFlBQVksR0FBRyxJQUFJLENBQUMsSUFBSSxDQUFDLFNBQVMsRUFBRSxZQUFZLENBQUMsQ0FBQztRQUV4RCxNQUFNLEVBQUUsR0FBRyxJQUFJLHFCQUFRLENBQUMsSUFBSSxFQUFFLG1CQUFtQixFQUFFO1lBQ2pELE9BQU8sRUFBRSxvQkFBTyxDQUFDLFVBQVU7WUFDM0IsT0FBTyxFQUFFLGVBQWU7WUFDeEIsSUFBSSxFQUFFLGlCQUFJLENBQUMsU0FBUyxDQUFDLFlBQVksRUFBRTtnQkFDakMsUUFBUSxFQUFFO29CQUNSLEtBQUssRUFBRSxvQkFBTyxDQUFDLFVBQVUsQ0FBQyxhQUFhO29CQUN2QyxLQUFLLEVBQUU7d0JBQ0wsU0FBUyxDQUFDLFNBQWlCOzRCQUN6QixJQUFJO2dDQUNGLHdCQUFRLENBQUMsZ0JBQWdCLENBQUMsQ0FBQzs2QkFDNUI7NEJBQUMsTUFBTTtnQ0FDTixPQUFPLEtBQUssQ0FBQzs2QkFDZDs0QkFFRCx3QkFBUSxDQUNOLGtCQUFrQixJQUFJLENBQUMsSUFBSSxDQUN6QixZQUFZLEVBQ1osa0JBQWtCLENBQ25CLE9BQU8sSUFBSSxDQUFDLElBQUksQ0FBQyxTQUFTLENBQUMsRUFBRSxDQUMvQixDQUFDOzRCQUNGLHdCQUFRLENBQUMsVUFBVSxZQUFZLE1BQU0sSUFBSSxDQUFDLElBQUksQ0FBQyxTQUFTLENBQUMsRUFBRSxDQUFDLENBQUM7NEJBQzdELE9BQU8sSUFBSSxDQUFDO3dCQUNkLENBQUM7cUJBQ0Y7aUJBQ0Y7YUFDRixDQUFDO1lBQ0YsV0FBVyxFQUFFO2dCQUNYLFNBQVMsRUFBRSxJQUFJLENBQUMsS0FBSyxDQUFDLFFBQVE7YUFDL0I7WUFDRCxPQUFPLEVBQUUsc0JBQVEsQ0FBQyxPQUFPLENBQUMsQ0FBQyxDQUFDO1lBQzVCLFVBQVUsRUFBRSxHQUFHO1lBQ2YsWUFBWSxFQUFFLElBQUksQ0FBQyxLQUFLLENBQUMsZ0JBQWdCO2dCQUN2QyxDQUFDLENBQUMsSUFBSSxDQUFDLEtBQUssQ0FBQyxnQkFBZ0I7Z0JBQzdCLENBQUMsQ0FBQyx3QkFBYSxDQUFDLFNBQVM7WUFDM0IsV0FBVyxFQUFFLHlEQUF5RDtTQUN2RSxDQUFDLENBQUM7UUFFSCxJQUFJLFVBQVUsR0FBc0IsRUFBRSxDQUFDO1FBQ3ZDLFVBQVUsQ0FBQyxJQUFJLENBQ2IsSUFBSSx5QkFBZSxDQUFDO1lBQ2xCLE1BQU0sRUFBRSxnQkFBTSxDQUFDLEtBQUs7WUFDcEIsT0FBTyxFQUFFLENBQUMsYUFBYSxDQUFDO1lBQ3hCLFNBQVMsRUFBRSxDQUFDLElBQUksQ0FBQyxLQUFLLENBQUMsUUFBUSxDQUFDO1NBQ2pDLENBQUMsQ0FDSCxDQUFDO1FBQ0YsSUFBSSxJQUFJLENBQUMsS0FBSyxDQUFDLE1BQU0sRUFBRTtZQUNyQixVQUFVLENBQUMsSUFBSSxDQUNiLElBQUkseUJBQWUsQ0FBQztnQkFDbEIsTUFBTSxFQUFFLGdCQUFNLENBQUMsS0FBSztnQkFDcEIsT0FBTyxFQUFFLENBQUMsYUFBYSxFQUFFLHFCQUFxQixDQUFDO2dCQUMvQyxTQUFTLEVBQUUsQ0FBQyxJQUFJLENBQUMsS0FBSyxDQUFDLE1BQU8sQ0FBQzthQUNoQyxDQUFDLENBQ0gsQ0FBQztTQUNIO1FBRUQsRUFBRSxDQUFDLElBQUksRUFBRSxrQkFBa0IsQ0FDekIsSUFBSSxnQkFBTSxDQUFDLElBQUksRUFBRSxhQUFhLEVBQUU7WUFDOUIsVUFBVTtTQUNYLENBQUMsQ0FDSCxDQUFDO1FBQ0YsT0FBTyxFQUFFLENBQUM7SUFDWixDQUFDOztBQXBGSCwwQ0FxRkMiLCJzb3VyY2VzQ29udGVudCI6WyJpbXBvcnQgeyBleGVjU3luYyB9IGZyb20gJ2NoaWxkX3Byb2Nlc3MnO1xuaW1wb3J0ICogYXMgcGF0aCBmcm9tICdwYXRoJztcblxuaW1wb3J0IHsgRHVyYXRpb24gfSBmcm9tICdhd3MtY2RrLWxpYic7XG5pbXBvcnQgeyBSdWxlIH0gZnJvbSAnYXdzLWNkay1saWIvYXdzLWV2ZW50cyc7XG5pbXBvcnQgeyBMYW1iZGFGdW5jdGlvbiB9IGZyb20gJ2F3cy1jZGstbGliL2F3cy1ldmVudHMtdGFyZ2V0cyc7XG5pbXBvcnQgeyBFZmZlY3QsIFBvbGljeSwgUG9saWN5U3RhdGVtZW50IH0gZnJvbSAnYXdzLWNkay1saWIvYXdzLWlhbSc7XG5pbXBvcnQgeyBDb2RlLCBGdW5jdGlvbiwgUnVudGltZSB9IGZyb20gJ2F3cy1jZGstbGliL2F3cy1sYW1iZGEnO1xuaW1wb3J0IHsgUmV0ZW50aW9uRGF5cyB9IGZyb20gJ2F3cy1jZGstbGliL2F3cy1sb2dzJztcbmltcG9ydCB7IENvbnN0cnVjdCB9IGZyb20gJ2NvbnN0cnVjdHMnO1xuaW1wb3J0IHsgRWNyU2Nhbk5vdGlmaWVyUHJvcGVydGllcyB9IGZyb20gJy4vZWNyU2Nhbk5vdGlmaWVyUHJvcGVydGllcyc7XG5cbmV4cG9ydCBjbGFzcyBFY3JTY2FuTm90aWZpZXIgZXh0ZW5kcyBDb25zdHJ1Y3Qge1xuICBwcm9wczogRWNyU2Nhbk5vdGlmaWVyUHJvcGVydGllcztcblxuICBjb25zdHJ1Y3RvcihzY29wZTogQ29uc3RydWN0LCBpZDogc3RyaW5nLCBwcm9wczogRWNyU2Nhbk5vdGlmaWVyUHJvcGVydGllcykge1xuICAgIHN1cGVyKHNjb3BlLCBpZCk7XG5cbiAgICB0aGlzLnByb3BzID0gcHJvcHM7XG4gICAgY29uc3QgaGFuZGxlciA9IHRoaXMuY3JlYXRlRnVuY3Rpb24oKTtcblxuICAgIGNvbnN0IGVjclNjYW5UYXJnZXQgPSBuZXcgTGFtYmRhRnVuY3Rpb24oaGFuZGxlcik7XG4gICAgbmV3IFJ1bGUodGhpcywgJ0V2ZW50QnVzRWNySW1hZ2VTY2FuJywge1xuICAgICAgcnVsZU5hbWU6ICdFdmVudEJ1c0VjckltYWdlU2NhblJ1bGUnLFxuICAgICAgZGVzY3JpcHRpb246ICdTZW5kIEVDUiBJbWFnZSBTY2FuIGZpbmRpbmdzIHRvIE1pY3Jvc29mdCBUZWFtcyBjaGFubmVsJyxcbiAgICAgIHRhcmdldHM6IFtlY3JTY2FuVGFyZ2V0XSxcbiAgICAgIGV2ZW50UGF0dGVybjoge1xuICAgICAgICBzb3VyY2U6IFsnYXdzLmVjcicsICdhd3MuaW5zcGVjdG9yMiddLFxuICAgICAgICBkZXRhaWxUeXBlOiBbJ0VDUiBJbWFnZSBTY2FuJywgJ0luc3BlY3RvcjIgU2NhbiddLFxuICAgICAgfSxcbiAgICB9KTtcbiAgfVxuICBwcml2YXRlIGNyZWF0ZUZ1bmN0aW9uKCk6IEZ1bmN0aW9uIHtcbiAgICBjb25zdCBmdW5jdGlvbl9kaXIgPSBwYXRoLmpvaW4oX19kaXJuYW1lLCAnLi4vbGFtYmRhLycpO1xuXG4gICAgY29uc3QgZm4gPSBuZXcgRnVuY3Rpb24odGhpcywgJ2Vjci1zY2FuLW5vdGlmaWVyJywge1xuICAgICAgcnVudGltZTogUnVudGltZS5QWVRIT05fM185LFxuICAgICAgaGFuZGxlcjogJ2luZGV4LmhhbmRsZXInLFxuICAgICAgY29kZTogQ29kZS5mcm9tQXNzZXQoZnVuY3Rpb25fZGlyLCB7XG4gICAgICAgIGJ1bmRsaW5nOiB7XG4gICAgICAgICAgaW1hZ2U6IFJ1bnRpbWUuUFlUSE9OXzNfOS5idW5kbGluZ0ltYWdlLFxuICAgICAgICAgIGxvY2FsOiB7XG4gICAgICAgICAgICB0cnlCdW5kbGUob3V0cHV0RGlyOiBzdHJpbmcpIHtcbiAgICAgICAgICAgICAgdHJ5IHtcbiAgICAgICAgICAgICAgICBleGVjU3luYygncGlwMyAtLXZlcnNpb24nKTtcbiAgICAgICAgICAgICAgfSBjYXRjaCB7XG4gICAgICAgICAgICAgICAgcmV0dXJuIGZhbHNlO1xuICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgZXhlY1N5bmMoXG4gICAgICAgICAgICAgICAgYHBpcCBpbnN0YWxsIC1yICR7cGF0aC5qb2luKFxuICAgICAgICAgICAgICAgICAgZnVuY3Rpb25fZGlyLFxuICAgICAgICAgICAgICAgICAgJ3JlcXVpcmVtZW50cy50eHQnLFxuICAgICAgICAgICAgICAgICl9IC10ICR7cGF0aC5qb2luKG91dHB1dERpcil9YCxcbiAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgZXhlY1N5bmMoYGNwIC1hdSAke2Z1bmN0aW9uX2Rpcn0vKiAke3BhdGguam9pbihvdXRwdXREaXIpfWApO1xuICAgICAgICAgICAgICByZXR1cm4gdHJ1ZTtcbiAgICAgICAgICAgIH0sXG4gICAgICAgICAgfSxcbiAgICAgICAgfSxcbiAgICAgIH0pLFxuICAgICAgZW52aXJvbm1lbnQ6IHtcbiAgICAgICAgVE9QSUNfQVJOOiB0aGlzLnByb3BzLnRvcGljQXJuLFxuICAgICAgfSxcbiAgICAgIHRpbWVvdXQ6IER1cmF0aW9uLm1pbnV0ZXMoMSksXG4gICAgICBtZW1vcnlTaXplOiAxMjgsXG4gICAgICBsb2dSZXRlbnRpb246IHRoaXMucHJvcHMubG9nUmV0ZW50aW9uRGF5c1xuICAgICAgICA/IHRoaXMucHJvcHMubG9nUmV0ZW50aW9uRGF5c1xuICAgICAgICA6IFJldGVudGlvbkRheXMuT05FX01PTlRILFxuICAgICAgZGVzY3JpcHRpb246ICdTZW5kIEVDUiBJbWFnZSBTY2FuIGZpbmRpbmdzIHRvIE1pY3Jvc29mdCBUZWFtcyBjaGFubmVsJyxcbiAgICB9KTtcblxuICAgIGxldCBzdGF0ZW1lbnRzOiBQb2xpY3lTdGF0ZW1lbnRbXSA9IFtdO1xuICAgIHN0YXRlbWVudHMucHVzaChcbiAgICAgIG5ldyBQb2xpY3lTdGF0ZW1lbnQoe1xuICAgICAgICBlZmZlY3Q6IEVmZmVjdC5BTExPVyxcbiAgICAgICAgYWN0aW9uczogWydzbnM6UHVibGlzaCddLFxuICAgICAgICByZXNvdXJjZXM6IFt0aGlzLnByb3BzLnRvcGljQXJuXSxcbiAgICAgIH0pLFxuICAgICk7XG4gICAgaWYgKHRoaXMucHJvcHMua2V5QXJuKSB7XG4gICAgICBzdGF0ZW1lbnRzLnB1c2goXG4gICAgICAgIG5ldyBQb2xpY3lTdGF0ZW1lbnQoe1xuICAgICAgICAgIGVmZmVjdDogRWZmZWN0LkFMTE9XLFxuICAgICAgICAgIGFjdGlvbnM6IFsna21zOkRlY3J5cHQnLCAna21zOkdlbmVyYXRlRGF0YUtleSddLFxuICAgICAgICAgIHJlc291cmNlczogW3RoaXMucHJvcHMua2V5QXJuIV0sXG4gICAgICAgIH0pLFxuICAgICAgKTtcbiAgICB9XG5cbiAgICBmbi5yb2xlPy5hdHRhY2hJbmxpbmVQb2xpY3koXG4gICAgICBuZXcgUG9saWN5KHRoaXMsICdzbnMtcHVibGlzaCcsIHtcbiAgICAgICAgc3RhdGVtZW50cyxcbiAgICAgIH0pLFxuICAgICk7XG4gICAgcmV0dXJuIGZuO1xuICB9XG59XG4iXX0=
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9698879551820728%*

 * *Differences: {"'devDependencies'": "{'projen': '^0.71.118'}", "'version'": "'0.0.4'"}*

```diff
@@ -20,15 +20,15 @@
         "jest": "^27",
         "jest-junit": "^15",
         "jsii": "1.x",
         "jsii-diff": "^1.84.0",
         "jsii-docgen": "^7.2.9",
         "jsii-pacmak": "^1.84.0",
         "npm-check-updates": "^16",
-        "projen": "^0.71.110",
+        "projen": "^0.71.118",
         "standard-version": "^9",
         "ts-jest": "^27",
         "typescript": "^4.9.5"
     },
     "jest": {
         "clearMocks": true,
         "collectCoverage": true,
@@ -139,9 +139,9 @@
         "test:watch": "npx projen test:watch",
         "unbump": "npx projen unbump",
         "upgrade": "npx projen upgrade",
         "watch": "npx projen watch"
     },
     "stability": "stable",
     "types": "lib/index.d.ts",
-    "version": "0.0.3"
+    "version": "0.0.4"
 }
```

### Comparing `ecr-scan-notifier-0.0.3/src/ecr_scan_notifier.egg-info/PKG-INFO` & `ecr-scan-notifier-0.0.4/src/ecr_scan_notifier.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecr-scan-notifier
-Version: 0.0.3
+Version: 0.0.4
 Summary: Notifies on new AWS ECR scan results
 Home-page: https://github.com/stefanfreitag/cdk-ecr-scan-notifier.git
 Author: Stefan Freitag<stefan.freitag@rwe.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/cdk-ecr-scan-notifier.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

