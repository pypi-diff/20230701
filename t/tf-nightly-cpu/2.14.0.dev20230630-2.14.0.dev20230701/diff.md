# Comparing `tmp/tf_nightly_cpu-2.14.0.dev20230630-cp39-cp39-win_amd64.whl.zip` & `tmp/tf_nightly_cpu-2.14.0.dev20230701-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2098 bytes, number of entries: 4
--rw-rw-r--  2.0 unx     2626 b- defN 23-Jun-30 07:51 tf_nightly_cpu-2.14.0.dev20230630.dist-info/METADATA
--rw-rw-r--  2.0 unx       99 b- defN 23-Jun-30 07:51 tf_nightly_cpu-2.14.0.dev20230630.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 23-Jun-30 07:51 tf_nightly_cpu-2.14.0.dev20230630.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      377 b- defN 23-Jun-30 07:51 tf_nightly_cpu-2.14.0.dev20230630.dist-info/RECORD
-4 files, 3103 bytes uncompressed, 1356 bytes compressed:  56.3%
+Zip file size: 2268 bytes, number of entries: 4
+-rw-rw-r--  2.0 unx     3412 b- defN 23-Jul-01 07:50 tf_nightly_cpu-2.14.0.dev20230701.dist-info/METADATA
+-rw-rw-r--  2.0 unx       99 b- defN 23-Jul-01 07:50 tf_nightly_cpu-2.14.0.dev20230701.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-01 07:50 tf_nightly_cpu-2.14.0.dev20230701.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      377 b- defN 23-Jul-01 07:50 tf_nightly_cpu-2.14.0.dev20230701.dist-info/RECORD
+4 files, 3889 bytes uncompressed, 1526 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: tf_nightly_cpu-2.14.0.dev20230630.dist-info/METADATA
+Filename: tf_nightly_cpu-2.14.0.dev20230701.dist-info/METADATA
 Comment: 
 
-Filename: tf_nightly_cpu-2.14.0.dev20230630.dist-info/WHEEL
+Filename: tf_nightly_cpu-2.14.0.dev20230701.dist-info/WHEEL
 Comment: 
 
-Filename: tf_nightly_cpu-2.14.0.dev20230630.dist-info/top_level.txt
+Filename: tf_nightly_cpu-2.14.0.dev20230701.dist-info/top_level.txt
 Comment: 
 
-Filename: tf_nightly_cpu-2.14.0.dev20230630.dist-info/RECORD
+Filename: tf_nightly_cpu-2.14.0.dev20230701.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `tf_nightly_cpu-2.14.0.dev20230630.dist-info/METADATA` & `tf_nightly_cpu-2.14.0.dev20230701.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-nightly-cpu
-Version: 2.14.0.dev20230630
+Version: 2.14.0.dev20230701
 Summary: TensorFlow is an open source machine learning framework for everyone.
 Home-page: https://www.tensorflow.org/
 Author: Google Inc.
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Download-URL: https://github.com/tensorflow/tensorflow/tags
 Keywords: tensorflow tensor machine learning
@@ -25,17 +25,29 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: tf-nightly-macos (==2.14.0-dev20230630) ; platform_system == "Darwin" and platform_machine == "arm64"
-Requires-Dist: tf-nightly-cpu-aws (==2.14.0-dev20230630) ; platform_system == "Linux" and (platform_machine == "arm64" or platform_machine == "aarch64")
-Requires-Dist: tf-nightly-intel (==2.14.0-dev20230630) ; platform_system == "Windows"
+Requires-Dist: tf-nightly-macos (==2.14.0-dev20230701) ; platform_system == "Darwin" and platform_machine == "arm64"
+Requires-Dist: tf-nightly-cpu-aws (==2.14.0-dev20230701) ; platform_system == "Linux" and (platform_machine == "arm64" or platform_machine == "aarch64")
+Requires-Dist: tf-nightly-intel (==2.14.0-dev20230701) ; platform_system == "Windows"
+Provides-Extra: and-cuda
+Requires-Dist: nvidia-cublas-cu11 (==11.11.3.6) ; extra == 'and-cuda'
+Requires-Dist: nvidia-cuda-cupti-cu11 (==11.8.87) ; extra == 'and-cuda'
+Requires-Dist: nvidia-cuda-nvcc-cu11 (==11.8.89) ; extra == 'and-cuda'
+Requires-Dist: nvidia-cuda-runtime-cu11 (==11.8.89) ; extra == 'and-cuda'
+Requires-Dist: nvidia-cudnn-cu11 (==8.7.0.84) ; extra == 'and-cuda'
+Requires-Dist: nvidia-cufft-cu11 (==10.9.0.58) ; extra == 'and-cuda'
+Requires-Dist: nvidia-curand-cu11 (==10.3.0.86) ; extra == 'and-cuda'
+Requires-Dist: nvidia-cusolver-cu11 (==11.4.1.48) ; extra == 'and-cuda'
+Requires-Dist: nvidia-cusparse-cu11 (==11.7.5.86) ; extra == 'and-cuda'
+Requires-Dist: nvidia-nccl-cu11 (==2.16.5) ; extra == 'and-cuda'
+Requires-Dist: tensorrt (==8.5.3.1) ; extra == 'and-cuda'
 
 [![Python](https://img.shields.io/pypi/pyversions/tensorflow.svg?style=plastic)](https://badge.fury.io/py/tensorflow)
 [![PyPI](https://badge.fury.io/py/tensorflow.svg)](https://badge.fury.io/py/tensorflow)
 
 TensorFlow is an open source software library for high performance numerical
 computation. Its flexible architecture allows easy deployment of computation
 across a variety of platforms (CPUs, GPUs, TPUs), and from desktops to clusters
```

