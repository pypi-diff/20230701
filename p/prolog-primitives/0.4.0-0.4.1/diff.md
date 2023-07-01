# Comparing `tmp/prolog_primitives-0.4.0.tar.gz` & `tmp/prolog_primitives-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prolog_primitives-0.4.0.tar", last modified: Fri Jun 30 13:52:24 2023, max compression
+gzip compressed data, was "prolog_primitives-0.4.1.tar", last modified: Sat Jul  1 10:35:10 2023, max compression
```

## Comparing `prolog_primitives-0.4.0.tar` & `prolog_primitives-0.4.1.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.348921 prolog_primitives-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-30 13:52:24.348921 prolog_primitives-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.336921 prolog_primitives-0.4.0/prolog_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-30 13:52:15.000000 prolog_primitives-0.4.0/prolog_primitives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.340921 prolog_primitives-0.4.0/prolog_primitives/basic/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/basic/DBManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/basic/DistributedElements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/basic/PrimitiveWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/basic/Session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/basic/SubRequestEvent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/basic/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/basic/filterKbPrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/basic/ntPrimitive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.340921 prolog_primitives-0.4.0/prolog_primitives/generatedProto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:15.000000 prolog_primitives-0.4.0/prolog_primitives/generatedProto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-06-30 13:52:15.000000 prolog_primitives-0.4.0/prolog_primitives/generatedProto/basicMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 13:52:15.000000 prolog_primitives-0.4.0/prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-06-30 13:52:15.000000 prolog_primitives-0.4.0/prolog_primitives/generatedProto/errorsMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 13:52:15.000000 prolog_primitives-0.4.0/prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-06-30 13:52:15.000000 prolog_primitives-0.4.0/prolog_primitives/generatedProto/primitiveService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-30 13:52:15.000000 prolog_primitives-0.4.0/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-06-30 13:52:15.000000 prolog_primitives-0.4.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 13:52:15.000000 prolog_primitives-0.4.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.340921 prolog_primitives-0.4.0/prolog_primitives/ml_lib/
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/Collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.344921 prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/fold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/randomSplit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/theoryToDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.344921 prolog_primitives-0.4.0/prolog_primitives/ml_lib/neuralNetwork/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/neuralNetwork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.344921 prolog_primitives-0.4.0/prolog_primitives/ml_lib/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/predictors/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/predictors/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/predictors/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/predictors/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.344921 prolog_primitives-0.4.0/prolog_primitives/ml_lib/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/schema/schemaClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/schema/theoryToSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.348921 prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/one_hot_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/schema_trasformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/transformationClass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.336921 prolog_primitives-0.4.0/prolog_primitives.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-30 13:52:24.000000 prolog_primitives-0.4.0/prolog_primitives.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-30 13:52:24.000000 prolog_primitives-0.4.0/prolog_primitives.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:52:24.000000 prolog_primitives-0.4.0/prolog_primitives.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:52:24.000000 prolog_primitives-0.4.0/prolog_primitives.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-30 13:52:24.000000 prolog_primitives-0.4.0/prolog_primitives.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 13:52:24.000000 prolog_primitives-0.4.0/prolog_primitives.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 13:52:24.348921 prolog_primitives-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.107066 prolog_primitives-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-01 10:35:10.107066 prolog_primitives-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.099066 prolog_primitives-0.4.1/prolog_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-01 10:35:03.000000 prolog_primitives-0.4.1/prolog_primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.099066 prolog_primitives-0.4.1/prolog_primitives/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/basic/DBManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/basic/DistributedElements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/basic/PrimitiveWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/basic/Session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/basic/SubRequestEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/basic/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/basic/filterKbPrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/basic/ntPrimitive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.103066 prolog_primitives-0.4.1/prolog_primitives/generatedProto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:03.000000 prolog_primitives-0.4.1/prolog_primitives/generatedProto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-07-01 10:35:03.000000 prolog_primitives-0.4.1/prolog_primitives/generatedProto/basicMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-01 10:35:03.000000 prolog_primitives-0.4.1/prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-01 10:35:03.000000 prolog_primitives-0.4.1/prolog_primitives/generatedProto/errorsMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-01 10:35:03.000000 prolog_primitives-0.4.1/prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-07-01 10:35:03.000000 prolog_primitives-0.4.1/prolog_primitives/generatedProto/primitiveService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-01 10:35:03.000000 prolog_primitives-0.4.1/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-01 10:35:03.000000 prolog_primitives-0.4.1/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-01 10:35:03.000000 prolog_primitives-0.4.1/prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.103066 prolog_primitives-0.4.1/prolog_primitives/ml_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/Collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.103066 prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/fold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/randomSplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/theoryToDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.103066 prolog_primitives-0.4.1/prolog_primitives/ml_lib/neuralNetwork/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/neuralNetwork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.103066 prolog_primitives-0.4.1/prolog_primitives/ml_lib/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/predictors/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/predictors/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/predictors/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/predictors/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.103066 prolog_primitives-0.4.1/prolog_primitives/ml_lib/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/schema/schemaClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/schema/theoryToSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.107066 prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/one_hot_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/schema_trasformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/transformationClass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.099066 prolog_primitives-0.4.1/prolog_primitives.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-01 10:35:10.000000 prolog_primitives-0.4.1/prolog_primitives.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-01 10:35:10.000000 prolog_primitives-0.4.1/prolog_primitives.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 10:35:10.000000 prolog_primitives-0.4.1/prolog_primitives.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 10:35:09.000000 prolog_primitives-0.4.1/prolog_primitives.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-01 10:35:10.000000 prolog_primitives-0.4.1/prolog_primitives.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-01 10:35:10.000000 prolog_primitives-0.4.1/prolog_primitives.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 10:35:10.107066 prolog_primitives-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/setup.py
```

### Comparing `prolog_primitives-0.4.0/LICENSE` & `prolog_primitives-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.0/PKG-INFO` & `prolog_primitives-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog_primitives
-Version: 0.4.0
+Version: 0.4.1
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/basic/DBManager.py` & `prolog_primitives-0.4.1/prolog_primitives/basic/DBManager.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.0/prolog_primitives/basic/DistributedElements.py` & `prolog_primitives-0.4.1/prolog_primitives/basic/DistributedElements.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.0/prolog_primitives/basic/PrimitiveWrapper.py` & `prolog_primitives-0.4.1/prolog_primitives/basic/PrimitiveWrapper.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.0/prolog_primitives/basic/Session.py` & `prolog_primitives-0.4.1/prolog_primitives/basic/Session.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.0/prolog_primitives/basic/SubRequestEvent.py` & `prolog_primitives-0.4.1/prolog_primitives/basic/SubRequestEvent.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.0/prolog_primitives/basic/Utils.py` & `prolog_primitives-0.4.1/prolog_primitives/basic/Utils.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.0/prolog_primitives/basic/filterKbPrimitive.py` & `prolog_primitives-0.4.1/prolog_primitives/basic/filterKbPrimitive.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.0/prolog_primitives/basic/ntPrimitive.py` & `prolog_primitives-0.4.1/prolog_primitives/basic/ntPrimitive.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.0/prolog_primitives/generatedProto/basicMessages_pb2.py` & `prolog_primitives-0.4.1/prolog_primitives/generatedProto/basicMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.0/prolog_primitives/generatedProto/errorsMessages_pb2.py` & `prolog_primitives-0.4.1/prolog_primitives/generatedProto/errorsMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.0/prolog_primitives/generatedProto/primitiveService_pb2.py` & `prolog_primitives-0.4.1/prolog_primitives/generatedProto/primitiveService_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.0/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py` & `prolog_primitives-0.4.1/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py` & `prolog_primitives-0.4.1/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/Collections.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/Collections.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/__main__.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/launcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,42 +20,43 @@
 from .predictors.train import trainPrimitive
 from .predictors.predict import predictPrimitive
 from .predictors.classify import classifyPrimitive
 from .predictors.score import msePrimitive
 from ..basic import PrimitiveWrapper, DistributedElements
 from concurrent.futures import ThreadPoolExecutor
 
-servers = []
-libraryName = "customLibrary"
-
-def launchPrimitive(primitive: DistributedElements.DistributedPrimitiveWrapper, port: int):
-    server = PrimitiveWrapper.serve(primitive, port, libraryName)
-    servers.append(server)
-    server.wait_for_termination()
-    
-primitives = [schemaPrimitive, theoryToSchemaPrimitive,
-              theoryToDatasetPrimitive, randomSplitPrimitive,
-              rowPrimitive, columnPrimitive, cellPrimitive, foldPrimitive, 
-              theoryFromDatasetPrimitive, schemaTrasformation,
-              normalizePrimitive, one_hot_encodePrimitive, dropPrimitive,
-              fitPrimitive, transformPrimitive, inputLayerPrimitive,
-              denseLayerPrimitive, outputLayerPrimitive, neuralNetworkPrimitive,
-              trainPrimitive, predictPrimitive, classifyPrimitive, msePrimitive]
-
-port = 8080
-executor = ThreadPoolExecutor(max_workers=len(primitives))
-
-for primitive in primitives:
-    future = executor.submit(launchPrimitive, primitive, port)
-    port += 1
-
-try:
-    for server in servers:
+def main():
+    servers = []
+    libraryName = "customLibrary"
+
+    def launchPrimitive(primitive: DistributedElements.DistributedPrimitiveWrapper, port: int):
+        server = PrimitiveWrapper.serve(primitive, port, libraryName)
+        servers.append(server)
         server.wait_for_termination()
-except (Exception, KeyboardInterrupt, SystemExit) as inst:
-    executor.shutdown(wait=False, cancel_futures=True)
-    for server in servers:
-        server.stop(0)
-
-#for primitive in primitives:
-#    DBManager.deletePrimitive(primitive.functor, primitive.arity, libraryName)
-print("Done!")
+        
+    primitives = [schemaPrimitive, theoryToSchemaPrimitive,
+                theoryToDatasetPrimitive, randomSplitPrimitive,
+                rowPrimitive, columnPrimitive, cellPrimitive, foldPrimitive, 
+                theoryFromDatasetPrimitive, schemaTrasformation,
+                normalizePrimitive, one_hot_encodePrimitive, dropPrimitive,
+                fitPrimitive, transformPrimitive, inputLayerPrimitive,
+                denseLayerPrimitive, outputLayerPrimitive, neuralNetworkPrimitive,
+                trainPrimitive, predictPrimitive, classifyPrimitive, msePrimitive]
+
+    port = 8080
+    executor = ThreadPoolExecutor(max_workers=len(primitives))
+
+    for primitive in primitives:
+        future = executor.submit(launchPrimitive, primitive, port)
+        port += 1
+
+    try:
+        for server in servers:
+            server.wait_for_termination()
+    except (Exception, KeyboardInterrupt, SystemExit) as inst:
+        executor.shutdown(wait=False, cancel_futures=True)
+        for server in servers:
+            server.stop(0)
+
+    #for primitive in primitives:
+    #    DBManager.deletePrimitive(primitive.functor, primitive.arity, libraryName)
+    print("Done!")
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/cell.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/cell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 import tensorflow as tf
 
 class __CellPrimitive(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         dataset_ref = request.arguments[0]
         row_index = request.arguments[1]
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/column.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/column.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 import tensorflow as tf
 
 class __ColumnPrimitive(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         dataset_ref = request.arguments[0]
         column = request.arguments[1]
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/fold.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/fold.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 from sklearn.model_selection import KFold
 import numpy as np
 
 class __FoldPrimitive(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         dataset_ref = request.arguments[0]
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/randomSplit.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/randomSplit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 from datasets import Dataset
 
 class __RandomSplitPrimitive(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         dataset_ref = request.arguments[0]
         ratio = request.arguments[1]
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/row.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/row.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 import tensorflow as tf
 
 class __RowPrimitive(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         dataset_ref = request.arguments[0]
         index = request.arguments[1]
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/theoryToDataset.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/theoryToDataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import primitiveService_pb2 as primitiveMsg
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from prolog_primitives.generatedProto import errorsMessages_pb2 as errorMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 from datasets import Dataset
 
 class __TheoryToDatasetPrimitive(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         schema_name = request.arguments[0]
         dataset_ref = request.arguments[1]
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto.sideEffectsMessages_pb2 import SetClausesOfKBMsg, SideEffectMsg
 import prolog_primitives.generatedProto.basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 import tensorflow as tf
 
 def wrapInClause(struct: basicMsg.StructMsg):
     finalStruct = basicMsg.StructMsg(
         functor = ":-"
     )
     finalStruct.arguments.append(basicMsg.ArgumentMsg(struct=struct))
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 import tensorflow as tf
 
 class __DenseLayer(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         topology_in_ref = request.arguments[0]
         size = request.arguments[1]
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 import tensorflow as tf
 from datasets import Dataset
 
 class __InputLayer(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         size = request.arguments[0]
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 import tensorflow as tf
 from datasets import Dataset
 
 class __NeuralNetwork(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         topology_ref = request.arguments[0]
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 import tensorflow as tf
 
 class __OutputLayer(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         topology_in_ref = request.arguments[0]
         size = request.arguments[1]
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/predictors/classify.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/predictors/classify.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 import tensorflow as tf
 from datasets import Dataset
 
 
 
 class __Classify(DistributedElements.DistributedPrimitive):
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/predictors/predict.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/predictors/predict.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 import tensorflow as tf
 from datasets import Dataset
 
 class __Predict(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         predictor_ref = request.arguments[0]
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/predictors/score.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/predictors/score.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 import tensorflow as tf
 from datasets import Dataset
 from abc import ABC, abstractmethod
 
 
 
 class __AssessTemplate(DistributedElements.DistributedPrimitive, ABC):
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/predictors/train.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/predictors/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 import tensorflow as tf
 from datasets import Dataset
 
 def parseParams(structs: list[Utils.Struct]):
     params = {
         "epoch": 1,
         "loss": "mse",
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/schema/schema.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/schema/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 from .schemaClass import Schema, Attribute, parseAttributeFromStruct
 
 class __SchemaPrimitive(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         schema_ref = request.arguments[0]
         schema_name = request.arguments[1]
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/schema/schemaClass.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/schema/schemaClass.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/schema/theoryToSchema.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/schema/theoryToSchema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import primitiveService_pb2 as primitiveMsg
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from .. import Collections
+from .. import collections
 from .schemaClass import parseAttributeFromStruct
 
 class __TheoryToSchemaPrimitive(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         arg0 = request.arguments[0]
         if(arg0.HasField("var")):
@@ -34,17 +34,17 @@
                 primitiveMsg.InspectKbMsg.STATIC,
                 [(primitiveMsg.InspectKbMsg.STARTS_WITH, "schema_target")]))
             if(targetFact == None):
                 yield request.replyFail()
             else:
                 targets = Utils.parseArgumentMsgList(targetFact.arguments[0].struct.arguments[0])
             substitutions = {
-                arg0.var: basicMsg.ArgumentMsg(constant=Collections
+                arg0.var: basicMsg.ArgumentMsg(constant=collections
                                                .SharedCollections()
-                                               .addSchema(Collections.Schema(schema_name, attributes, targets))) 
+                                               .addSchema(collections.Schema(schema_name, attributes, targets))) 
                 }
             yield request.replySuccess(substitutions, hasNext=False)
         else:
             request.replyFail()
             
             
 theoryToSchemaPrimitive = DistributedElements.DistributedPrimitiveWrapper("theoryToSchema", 1, __TheoryToSchemaPrimitive())
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/drop.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/drop.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 from .transformationClass import Dropper, Pipeline
 
 class __Drop(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         transf_in_ref = request.arguments[0]
         attributes = request.arguments[1]
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/fit.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 from .transformationClass import  Pipeline
 from datasets import Dataset
 
 class __Fit(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         transf_in_ref = request.arguments[0]
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/normalization.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/normalization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 from .transformationClass import Normalization, Pipeline
 
 class __Normalize(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         transf_in_ref = request.arguments[0]
         attributes = request.arguments[1]
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/one_hot_encode.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/one_hot_encode.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 from ..schema.schemaClass import Schema
 from .transformationClass import OneHotEncoder, Pipeline
 
 class __One_Hot_Encode(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         transf_in_ref = request.arguments[0]
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/schema_trasformation.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/schema_trasformation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 import tensorflow as tf
 from .transformationClass import Pipeline
 
 class __SchemaTrasformation(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         schema_ref = request.arguments[0]
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/transform.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 from .transformationClass import Pipeline
 from datasets import Dataset
 
 class __Transform(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         dataset_in_ref = request.arguments[0]
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/transformationClass.py` & `prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/transformationClass.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 import tensorflow as tf
-from ..Collections import SharedCollections
+from ..collections import SharedCollections
 from ..schema.schemaClass import Schema
 from datasets import Dataset
 
 class Transformation(ABC):
     applier = None
     inverter = None
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives.egg-info/PKG-INFO` & `prolog_primitives-0.4.1/prolog_primitives.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog-primitives
-Version: 0.4.0
+Version: 0.4.1
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-0.4.0/prolog_primitives.egg-info/SOURCES.txt` & `prolog_primitives-0.4.1/prolog_primitives.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 prolog_primitives/generatedProto/primitiveService_pb2.py
 prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
 prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
 prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
 prolog_primitives/ml_lib/Collections.py
 prolog_primitives/ml_lib/__init__.py
 prolog_primitives/ml_lib/__main__.py
+prolog_primitives/ml_lib/launcher.py
 prolog_primitives/ml_lib/dataset/__init__.py
 prolog_primitives/ml_lib/dataset/cell.py
 prolog_primitives/ml_lib/dataset/column.py
 prolog_primitives/ml_lib/dataset/fold.py
 prolog_primitives/ml_lib/dataset/randomSplit.py
 prolog_primitives/ml_lib/dataset/row.py
 prolog_primitives/ml_lib/dataset/theoryToDataset.py
```

### Comparing `prolog_primitives-0.4.0/setup.py` & `prolog_primitives-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         with version_file.open('w') as f:
             f.write(version)
         return version
     except subprocess.CalledProcessError:
         if version_file.exists():
             return version_file.read_text().strip()
         else:
-            return '0.4.0'
+            return '0.4.1'
 
 
 version = get_version_from_git()
 
 
 print(f"Detected version {version} from git describe")
```

