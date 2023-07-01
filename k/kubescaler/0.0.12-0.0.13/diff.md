# Comparing `tmp/kubescaler-0.0.12.tar.gz` & `tmp/kubescaler-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubescaler-0.0.12.tar", last modified: Sun Jun 25 05:02:22 2023, max compression
+gzip compressed data, was "kubescaler-0.0.13.tar", last modified: Sat Jul  1 07:06:24 2023, max compression
```

## Comparing `kubescaler-0.0.12.tar` & `kubescaler-0.0.13.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:02:22.354797 kubescaler-0.0.12/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-05-24 04:09:38.000000 kubescaler-0.0.12/COPYRIGHT
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-05-24 04:09:38.000000 kubescaler-0.0.12/LICENSE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      317 2023-05-24 04:15:45.000000 kubescaler-0.0.12/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-05-24 04:09:38.000000 kubescaler-0.0.12/NOTICE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3374 2023-06-25 05:02:22.354797 kubescaler-0.0.12/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2512 2023-05-25 18:09:11.000000 kubescaler-0.0.12/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:02:22.350798 kubescaler-0.0.12/kubescaler/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       43 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2370 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1755 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/decorators.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      604 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6105 2023-05-24 04:39:20.000000 kubescaler-0.0.12/kubescaler/logger.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:02:22.350798 kubescaler-0.0.12/kubescaler/scaler/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:02:18.000000 kubescaler-0.0.12/kubescaler/scaler/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:02:22.354797 kubescaler-0.0.12/kubescaler/scaler/aws/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       32 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/scaler/aws/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1103 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/scaler/aws/ami.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    22082 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/scaler/aws/cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1316 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/scaler/aws/template.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    11961 2023-06-21 21:22:35.000000 kubescaler-0.0.12/kubescaler/scaler/google.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:02:22.354797 kubescaler-0.0.12/kubescaler/utils/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      399 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/utils/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5085 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/utils/fileio.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1456 2023-05-24 04:38:11.000000 kubescaler-0.0.12/kubescaler/utils/misc.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      912 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/utils/terminal.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1414 2023-06-25 05:02:18.000000 kubescaler-0.0.12/kubescaler/version.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:02:22.350798 kubescaler-0.0.12/kubescaler.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3374 2023-06-25 05:02:21.000000 kubescaler-0.0.12/kubescaler.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      716 2023-06-25 05:02:22.000000 kubescaler-0.0.12/kubescaler.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 05:02:21.000000 kubescaler-0.0.12/kubescaler.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-24 05:01:47.000000 kubescaler-0.0.12/kubescaler.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      230 2023-06-25 05:02:21.000000 kubescaler-0.0.12/kubescaler.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       11 2023-06-25 05:02:21.000000 kubescaler-0.0.12/kubescaler.egg-info/top_level.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-05-24 04:09:39.000000 kubescaler-0.0.12/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      294 2023-06-25 05:02:22.354797 kubescaler-0.0.12/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3584 2023-06-25 05:02:18.000000 kubescaler-0.0.12/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 07:06:24.801142 kubescaler-0.0.13/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-05-24 04:09:38.000000 kubescaler-0.0.13/COPYRIGHT
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-05-24 04:09:38.000000 kubescaler-0.0.13/LICENSE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      317 2023-05-24 04:15:45.000000 kubescaler-0.0.13/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-05-24 04:09:38.000000 kubescaler-0.0.13/NOTICE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3374 2023-07-01 07:06:24.801142 kubescaler-0.0.13/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2512 2023-05-25 18:09:11.000000 kubescaler-0.0.13/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 07:06:24.797141 kubescaler-0.0.13/kubescaler/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       43 2023-05-25 18:09:11.000000 kubescaler-0.0.13/kubescaler/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2370 2023-05-25 18:09:11.000000 kubescaler-0.0.13/kubescaler/cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1755 2023-05-25 18:09:11.000000 kubescaler-0.0.13/kubescaler/decorators.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      604 2023-05-25 18:09:11.000000 kubescaler-0.0.13/kubescaler/defaults.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6104 2023-07-01 07:06:21.000000 kubescaler-0.0.13/kubescaler/logger.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 07:06:24.801142 kubescaler-0.0.13/kubescaler/scaler/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:02:18.000000 kubescaler-0.0.13/kubescaler/scaler/__init__.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 07:06:24.801142 kubescaler-0.0.13/kubescaler/scaler/aws/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       32 2023-05-25 18:09:11.000000 kubescaler-0.0.13/kubescaler/scaler/aws/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1103 2023-05-25 18:09:11.000000 kubescaler-0.0.13/kubescaler/scaler/aws/ami.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    24799 2023-07-01 07:06:21.000000 kubescaler-0.0.13/kubescaler/scaler/aws/cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1316 2023-05-25 18:09:11.000000 kubescaler-0.0.13/kubescaler/scaler/aws/template.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1321 2023-07-01 07:06:21.000000 kubescaler-0.0.13/kubescaler/scaler/aws/token.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    11961 2023-06-21 21:22:35.000000 kubescaler-0.0.13/kubescaler/scaler/google.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 07:06:24.801142 kubescaler-0.0.13/kubescaler/utils/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      399 2023-05-25 18:09:11.000000 kubescaler-0.0.13/kubescaler/utils/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5085 2023-05-25 18:09:11.000000 kubescaler-0.0.13/kubescaler/utils/fileio.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1456 2023-05-24 04:38:11.000000 kubescaler-0.0.13/kubescaler/utils/misc.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      912 2023-05-25 18:09:11.000000 kubescaler-0.0.13/kubescaler/utils/terminal.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1414 2023-07-01 07:06:21.000000 kubescaler-0.0.13/kubescaler/version.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 07:06:24.801142 kubescaler-0.0.13/kubescaler.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3374 2023-07-01 07:06:24.000000 kubescaler-0.0.13/kubescaler.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      747 2023-07-01 07:06:24.000000 kubescaler-0.0.13/kubescaler.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-01 07:06:24.000000 kubescaler-0.0.13/kubescaler.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-24 05:01:47.000000 kubescaler-0.0.13/kubescaler.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      230 2023-07-01 07:06:24.000000 kubescaler-0.0.13/kubescaler.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       11 2023-07-01 07:06:24.000000 kubescaler-0.0.13/kubescaler.egg-info/top_level.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-05-24 04:09:39.000000 kubescaler-0.0.13/pyproject.toml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      294 2023-07-01 07:06:24.801142 kubescaler-0.0.13/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3584 2023-06-25 05:02:18.000000 kubescaler-0.0.13/setup.py
```

### Comparing `kubescaler-0.0.12/LICENSE` & `kubescaler-0.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.12/NOTICE` & `kubescaler-0.0.13/NOTICE`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.12/PKG-INFO` & `kubescaler-0.0.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubescaler
-Version: 0.0.12
+Version: 0.0.13
 Summary: Helper classes for scaling Kubernetes clusters
 Home-page: https://github.com/converged-computing/kubescaler
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: Kubernetes,elasticity,scaling,EKS,GKE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kubescaler Version: 0.0.12 Summary: Helper classes
+Metadata-Version: 2.1 Name: kubescaler Version: 0.0.13 Summary: Helper classes
 for scaling Kubernetes clusters Home-page: https://github.com/converged-
 computing/kubescaler Author: Vanessa Sochat Author-email:
 vsoch@users.noreply.github.com Maintainer: Vanessa Sochat License: LICENSE
 Keywords: Kubernetes,elasticity,scaling,EKS,GKE Platform: UNKNOWN Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
```

### Comparing `kubescaler-0.0.12/README.md` & `kubescaler-0.0.13/README.md`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.12/kubescaler/cluster.py` & `kubescaler-0.0.13/kubescaler/cluster.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.12/kubescaler/decorators.py` & `kubescaler-0.0.13/kubescaler/decorators.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.12/kubescaler/defaults.py` & `kubescaler-0.0.13/kubescaler/defaults.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.12/kubescaler/logger.py` & `kubescaler-0.0.13/kubescaler/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 
 
 def setup_logger(
     quiet=False,
     printshellcmds=False,
     nocolor=False,
     stdout=False,
-    debug=False,
+    debug=True,
     use_threads=False,
 ):
     # console output only if no custom logger was specified
     stream_handler = ColorizingStreamHandler(
         nocolor=nocolor,
         stream=sys.stdout if stdout else sys.stderr,
         use_threads=use_threads,
```

### Comparing `kubescaler-0.0.12/kubescaler/scaler/aws/ami.py` & `kubescaler-0.0.13/kubescaler/scaler/aws/ami.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.12/kubescaler/scaler/aws/cluster.py` & `kubescaler-0.0.13/kubescaler/scaler/aws/cluster.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
+import base64
 import json
 import os
-import subprocess
 import sys
+import tempfile
 import time
 
 try:
     import boto3
 except ImportError:
     sys.exit("Please pip install kubescaler[aws]")
 
@@ -21,14 +22,15 @@
 import kubescaler.utils as utils
 from kubescaler.cluster import Cluster
 from kubescaler.decorators import retry, timed
 from kubescaler.logger import logger
 
 from .ami import get_latest_ami
 from .template import auth_config_data, vpc_template, workers_template
+from .token import get_bearer_token
 
 stack_failure_options = ["DELETE", "DO_NOTHING", "ROLLBACK"]
 
 
 class EKSCluster(Cluster):
     """
     A scaler for an Amazon EKS Cluster
@@ -61,25 +63,28 @@
         self.keypair_file = keypair_file or "aws-worker-secret.pem"
         self.auth_config_file = auth_config_file or "aws-auth-config.yaml"
 
         # You might want to update this to better debug (so not deleted)
         # DO_NOTHING | ROLLBACK | DELETE
         self.set_stack_failure(on_stack_failure)
         self.stack_timeout_minutes = max(1, stack_timeout_minutes)
+        self.token_expires = kwargs.get("token_expires")
 
         # Here we define cluster name from name
         self.cluster_name = self.name
         self.tags = self.tags or {}
         if not isinstance(self.tags, dict):
             raise ValueError("Tags must be key value pairs (dict)")
 
         # kube config file
         self.kube_config_file = kube_config_file or "kubeconfig-aws.yaml"
         self.image_ami = get_latest_ami(self.region, self.kubernetes_version)
         self.machine_type = self.machine_type or "m5.large"
+        self.configuration = None
+        self._kubectl = None
 
         # Client connections
         self.session = boto3.Session(region_name=self.region)
         self.ec2 = self.session.client("ec2")
         self.cf = self.session.client("cloudformation")
         self.iam = self.session.client("iam")
         self.eks = self.session.client("eks")
@@ -103,81 +108,128 @@
             raise ValueError(
                 f"{on_stack_failure} is not a valid option, choices are: {options}"
             )
 
     @timed
     def create_cluster(self):
         """
-        Create a cluster
+        Create a cluster.
+
+        To verify this is working, you should be able to view the Cloud Formation
+        in the console to see the VPC stack, and when that is complete, go to
+        EKS to see the cluster being created. When the cluster is created and
+        the nodes are up, the wait_for_nodes function should finish a little
+        bit after. If you don't see this happening, usually it means a mismatch
+        between the credentials you used to create the cluster, and the ones
+        that the AWS client discovers here (in token.py) to generate a token.
+        It's best to be consistent and use an environment set (that ideally
+        has a long enough expiration) OR just the $HOME/.aws/config.
         """
+        print("🥞️ Creating VPC stack and subnets...")
         self.set_vpc_stack()
         self.set_subnets()
 
+        # Save cluster metadata so we can get the k8s client later
         try:
-            cluster = self.eks.describe_cluster(name=self.cluster_name)
+            self.cluster = self.eks.describe_cluster(name=self.cluster_name)
         except Exception:
-            cluster = self.new_cluster()
+            print("🥣️ Creating cluster...")
+            self.cluster = self.new_cluster()
 
         # Get the status and confirm it's active
-        status = cluster["cluster"]["status"]
+        status = self.cluster["cluster"]["status"]
         if status != "ACTIVE":
             raise ValueError(
                 f"Found cluster {self.cluster_name} but status is {status} and should be ACTIVE"
             )
 
         # Get cluster endpoint and security info so we can make kubectl config
-        self.certificate = cluster["cluster"]["certificateAuthority"]["data"]
-        self.endpoint = cluster["cluster"]["endpoint"]
+        self.certificate = self.cluster["cluster"]["certificateAuthority"]["data"]
+        self.endpoint = self.cluster["cluster"]["endpoint"]
 
         # Ensure we have a config to interact with, and write the keypair file
         self.ensure_kube_config()
         self.get_keypair()
 
         # The cluster is actually created with no nodes - just the control plane!
         # Here is where we create the workers, via a stack. Because apparently
-        # AWS really likes their pancakes.
+        # AWS really likes their pancakes. 🥞️
         self.set_workers_stack()
         self.create_auth_config()
 
         # We can only wait for the node group after we set the auth config!
         # I was surprised this is expecting the workers name and not the node
         # group name.
         self.wait_for_nodes()
 
         print(f"🦊️ Writing config file to {self.kube_config_file}")
         print(f"  Usage: kubectl --kubeconfig={self.kube_config_file} get nodes")
-        return cluster
+        return self.cluster
+
+    def get_k8s_client(self):
+        """
+        Get a client to use to interact with the cluster, either corev1.api
+        or the kubernetes api client.
+
+        https://github.com/googleapis/python-container/issues/6
+        """
+        if self._kubectl:
+            return self._kubectl
+
+        # Save the configuration for advanced users to user later
+        if not self.configuration:
+            # This is separate in case we need to manually call it (expires, etc.)
+            self._generate_configuration()
+
+        # This has .api_client for just the api client
+        self._kubectl = k8s.CoreV1Api(k8s.ApiClient(self.configuration))
+        return self._kubectl
+
+    def _generate_configuration(self):
+        """
+        Generate the kubectl configuration, no matter what.
+
+        This is separate from the get_k8s_client function as we might want
+        to call it to regenerate the self.configuration and self._kubectl.
+        """
+        # Get a token from the aws client, which must be installed
+        # aws eks get-token --cluster-name example
+        token = get_bearer_token(self.cluster_name, self.token_expires)
+        configuration = k8s.Configuration()
+        configuration.host = self.cluster["cluster"]["endpoint"]
+        with tempfile.NamedTemporaryFile(delete=False) as ca_cert:
+            ca_cert.write(
+                base64.b64decode(
+                    self.cluster["cluster"]["certificateAuthority"]["data"]
+                )
+            )
+            configuration.ssl_ca_cert = ca_cert.name
+        configuration.api_key_prefix["authorization"] = "Bearer"
+        configuration.api_key["authorization"] = token["status"]["token"]
+        self.configuration = configuration
 
     @timed
     def wait_for_nodes(self):
         """
         Wait for the nodes to be ready.
 
         We do this separately to allow timing. This function would be improved if
         we didn't need subprocess, but the waiter doesn't seem to work.
         """
+        kubectl = self.get_k8s_client()
         while True:
-            print(f"Waiting for {self.node_count} nodes to be Ready...")
+            print(f"⏱️ Waiting for {self.node_count} nodes to be Ready...")
             time.sleep(5)
-            # TODO fix to not require doing this! Maybe someone else wants to take a look?
-            res = subprocess.check_output(
-                [
-                    "kubectl",
-                    f"--kubeconfig={self.kube_config_file}",
-                    "--no-headers=true",
-                    "get",
-                    "nodes",
-                ]
-            )
-            lines = [x.strip() for x in res.decode("utf-8").split("\n") if x.strip()]
+            nodes = kubectl.list_node()
             ready_count = 0
-            for line in lines:
-                if "NotReady" in line:
-                    continue
-                ready_count += 1
+            for node in nodes.items:
+                for condition in node.status.conditions:
+                    # Don't add to node ready count if not ready
+                    if condition.type == "Ready" and condition.status == "True":
+                        ready_count += 1
             if ready_count == self.node_count:
                 break
 
         # The waiter doesn't seem to work - so we call kubectl until it's ready
         # waiter = self.eks.get_waiter("nodegroup_active")
         # waiter.wait(clusterName=self.cluster_name, nodegroupName=self.node_autoscaling_group_name)
 
@@ -345,15 +397,14 @@
                     "ParameterKey": "Subnets",
                     "ParameterValue": ",".join(self.vpc_subnet_ids),
                 },
             ],
             TimeoutInMinutes=self.stack_timeout_minutes,
             OnFailure=self.on_stack_failure,
         )
-        print(self.stack_timeout_minutes)
         return self._create_stack(stack, self.workers_name)
 
     def new_cluster(self):
         """
         Create a new cluster.
         """
         # Create Kubernetes cluster.
@@ -381,14 +432,15 @@
         """
         # Does it already exist?
         try:
             self.vpc_stack = self.cf.describe_stacks(StackName=self.vpc_name)
         except Exception:
             self.vpc_stack = self.create_vpc_stack()
 
+    @timed
     def create_vpc_stack(self):
         """
         Create a new stack from the template
         """
         # If not, create it from the template
         stack = self.cf.create_stack(
             StackName=self.vpc_name,
@@ -411,17 +463,20 @@
 
         if "StackId" not in stack:
             raise ValueError("Could not create VPC stack")
 
         try:
             logger.info(f"Waiting for {stack_name} stack...")
             waiter = self.cf.get_waiter("stack_create_complete")
+            # MaxAttempts defaults to 120, and Delay 30 seconds
             waiter.wait(StackName=stack_name)
-        except Exception:
-            raise ValueError("Waiting for stack creation exceeded wait time.")
+        except Exception as e:
+            # Allow waiting 3 more minutes
+            print(f"Waiting for stack creation exceeded wait time: {e}")
+            time.sleep(180)
 
         # Retrieve the same metadata if we had retrieved it
         return self.cf.describe_stacks(StackName=stack_name)
 
     def delete_stack(self, stack_name):
         """
         Delete a stack and wait for it to be deleted
@@ -552,14 +607,15 @@
         logger.info("⏳️ Cluster deletion started! Waiting...")
         waiter = self.eks.get_waiter("cluster_deleted")
         waiter.wait(name=self.cluster_name)
 
         # Delete the VPC stack and we are done!
         logger.info("🥅️ Deleting VPC and associated assets...")
         self.delete_vpc_stack()
+        self.delete_worker_stack()
         logger.info("⭐️ Done!")
 
     @property
     def data(self):
         """
         Combine class data into json object to save
         """
```

### Comparing `kubescaler-0.0.12/kubescaler/scaler/aws/template.py` & `kubescaler-0.0.13/kubescaler/scaler/aws/template.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.12/kubescaler/scaler/google.py` & `kubescaler-0.0.13/kubescaler/scaler/google.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.12/kubescaler/utils/fileio.py` & `kubescaler-0.0.13/kubescaler/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.12/kubescaler/utils/misc.py` & `kubescaler-0.0.13/kubescaler/utils/misc.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.12/kubescaler/utils/terminal.py` & `kubescaler-0.0.13/kubescaler/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.12/kubescaler/version.py` & `kubescaler-0.0.13/kubescaler/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
-__version__ = "0.0.12"
+__version__ = "0.0.13"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "kubescaler"
 PACKAGE_URL = "https://github.com/converged-computing/kubescaler"
 KEYWORDS = "Kubernetes, elasticity, scaling, EKS, GKE"
 DESCRIPTION = "Helper classes for scaling Kubernetes clusters"
 LICENSE = "LICENSE"
```

### Comparing `kubescaler-0.0.12/kubescaler.egg-info/PKG-INFO` & `kubescaler-0.0.13/kubescaler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubescaler
-Version: 0.0.12
+Version: 0.0.13
 Summary: Helper classes for scaling Kubernetes clusters
 Home-page: https://github.com/converged-computing/kubescaler
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: Kubernetes,elasticity,scaling,EKS,GKE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kubescaler Version: 0.0.12 Summary: Helper classes
+Metadata-Version: 2.1 Name: kubescaler Version: 0.0.13 Summary: Helper classes
 for scaling Kubernetes clusters Home-page: https://github.com/converged-
 computing/kubescaler Author: Vanessa Sochat Author-email:
 vsoch@users.noreply.github.com Maintainer: Vanessa Sochat License: LICENSE
 Keywords: Kubernetes,elasticity,scaling,EKS,GKE Platform: UNKNOWN Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
```

### Comparing `kubescaler-0.0.12/kubescaler.egg-info/SOURCES.txt` & `kubescaler-0.0.13/kubescaler.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -20,11 +20,12 @@
 kubescaler.egg-info/top_level.txt
 kubescaler/scaler/__init__.py
 kubescaler/scaler/google.py
 kubescaler/scaler/aws/__init__.py
 kubescaler/scaler/aws/ami.py
 kubescaler/scaler/aws/cluster.py
 kubescaler/scaler/aws/template.py
+kubescaler/scaler/aws/token.py
 kubescaler/utils/__init__.py
 kubescaler/utils/fileio.py
 kubescaler/utils/misc.py
 kubescaler/utils/terminal.py
```

### Comparing `kubescaler-0.0.12/setup.py` & `kubescaler-0.0.13/setup.py`

 * *Files identical despite different names*

