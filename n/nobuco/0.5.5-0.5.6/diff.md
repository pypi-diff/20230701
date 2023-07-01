# Comparing `tmp/nobuco-0.5.5.tar.gz` & `tmp/nobuco-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.5.5.tar", last modified: Fri Jun 30 19:09:26 2023, max compression
+gzip compressed data, was "nobuco-0.5.6.tar", last modified: Sat Jul  1 09:40:31 2023, max compression
```

## Comparing `nobuco-0.5.5.tar` & `nobuco-0.5.6.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 19:09:26.176802 nobuco-0.5.5/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.5.5/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)    24625 2023-06-30 19:09:26.176802 nobuco-0.5.5/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    22791 2023-06-30 19:07:43.000000 nobuco-0.5.5/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 19:09:26.168802 nobuco-0.5.5/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-06-23 09:29:01.000000 nobuco-0.5.5/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    13970 2023-06-30 18:23:08.000000 nobuco-0.5.5/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 19:09:26.172802 nobuco-0.5.5/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-19 20:03:57.000000 nobuco-0.5.5/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4095 2023-06-30 18:23:14.000000 nobuco-0.5.5/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 19:09:26.172802 nobuco-0.5.5/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 19:09:26.172802 nobuco-0.5.5/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4419 2023-06-17 09:52:53.000000 nobuco-0.5.5/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1069 2023-06-06 15:58:09.000000 nobuco-0.5.5/nobuco/layers/weight.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 19:09:26.172802 nobuco-0.5.5/nobuco/locate/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/locate/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/locate/link.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/locate/locate.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 19:09:26.176802 nobuco-0.5.5/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     6967 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2225 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/attention.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1169 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1165 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1790 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     5152 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14354 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2213 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2934 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9135 2023-06-30 18:40:38.000000 nobuco-0.5.5/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6449 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11315 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/tensor_manipulation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/tensor_shape.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      452 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/node_converters/torchvision.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 19:09:26.176802 nobuco-0.5.5/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10039 2023-06-23 19:26:03.000000 nobuco-0.5.5/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 19:09:26.176802 nobuco-0.5.5/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.5.5/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-30 19:09:26.172802 nobuco-0.5.5/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    24625 2023-06-30 19:09:26.000000 nobuco-0.5.5/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1702 2023-06-30 19:09:26.000000 nobuco-0.5.5/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-30 19:09:26.000000 nobuco-0.5.5/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-06-30 19:09:26.000000 nobuco-0.5.5/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-06-30 19:09:26.000000 nobuco-0.5.5/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-06-30 18:54:51.000000 nobuco-0.5.5/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-30 19:09:26.176802 nobuco-0.5.5/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-01 09:40:31.317635 nobuco-0.5.6/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.5.6/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)    24897 2023-07-01 09:40:31.317635 nobuco-0.5.6/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    24311 2023-07-01 09:37:46.000000 nobuco-0.5.6/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-01 09:40:31.309635 nobuco-0.5.6/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-06-23 09:29:01.000000 nobuco-0.5.6/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    13970 2023-06-30 18:23:08.000000 nobuco-0.5.6/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-01 09:40:31.313635 nobuco-0.5.6/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.6/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-19 20:03:57.000000 nobuco-0.5.6/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.5.6/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4095 2023-06-30 18:23:14.000000 nobuco-0.5.6/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-01 09:40:31.313635 nobuco-0.5.6/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.6/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.5.6/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-01 09:40:31.313635 nobuco-0.5.6/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.6/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4419 2023-06-17 09:52:53.000000 nobuco-0.5.6/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.5.6/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.5.6/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1069 2023-06-06 15:58:09.000000 nobuco-0.5.6/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-01 09:40:31.313635 nobuco-0.5.6/nobuco/locate/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.6/nobuco/locate/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.5.6/nobuco/locate/link.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.5.6/nobuco/locate/locate.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-01 09:40:31.313635 nobuco-0.5.6/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.5.6/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     6967 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2225 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/node_converters/attention.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1169 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1165 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1790 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     5152 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14354 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2213 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2934 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9135 2023-06-30 18:40:38.000000 nobuco-0.5.6/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6449 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11315 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/node_converters/tensor_manipulation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/node_converters/tensor_shape.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      452 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/node_converters/torchvision.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-01 09:40:31.317635 nobuco-0.5.6/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.6/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10039 2023-06-23 19:26:03.000000 nobuco-0.5.6/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.5.6/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-01 09:40:31.317635 nobuco-0.5.6/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.6/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.5.6/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.5.6/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-01 09:40:31.313635 nobuco-0.5.6/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    24897 2023-07-01 09:40:31.000000 nobuco-0.5.6/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1702 2023-07-01 09:40:31.000000 nobuco-0.5.6/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-01 09:40:31.000000 nobuco-0.5.6/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-07-01 09:40:31.000000 nobuco-0.5.6/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-07-01 09:40:31.000000 nobuco-0.5.6/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      735 2023-07-01 09:40:09.000000 nobuco-0.5.6/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-01 09:40:31.317635 nobuco-0.5.6/setup.cfg
```

### Comparing `nobuco-0.5.5/LICENSE` & `nobuco-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/PKG-INFO` & `nobuco-0.5.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,24 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.5.5
-Summary: Pytorch to Tensorflow conversion made somewhat easy
+Version: 0.5.6
+Summary: Pytorch to Tensorflow conversion made intuitive
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 Alexander Lutsenko
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
 Project-URL: Homepage, https://github.com/AlexanderLutsenko/nobuco
 Project-URL: Bug Tracker, https://github.com/AlexanderLutsenko/nobuco/issues
 Keywords: pytorch,tensorflow,keras,converter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-<img src="docs/nobuco.png">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/nobuco.png">
 <sup><a href="https://www.behance.net/diliajl">diliajl</a></sup>
 </p>
 
 **No** **Bu**llshit **Co**nverter is a tool that helps you translate pytorch models into tensorflow graphs without losing your mind.
 
 - Supports a wide range of architectures
   - [x] Control flow ops (If, While)
@@ -64,16 +43,15 @@
 - [Channel order wizardry](#channel-order-wizardry)
 - [In-place operations](#in-place-operations)
 - [Going dynamic](#going-dynamic)
   - [Control flows](#control-flows)
   - [Dynamic shapes](#dynamic-shapes)
 - [So we put a converter inside your converter](#so-we-put-a-converter-inside-your-converter)
 - [But was it worth it?](#but-was-it-worth-it)
-- [More nice things](#more-nice-things)
-  - [Nobuco knowledge base](#nobuco-knowledge-base)
+- [Nobuco knowledge base](#nobuco-knowledge-base)
 
 <!-- tocstop -->
 
 ## Essentials
 
 Suppose we want to convert a pytorch module similar to this one:
 
@@ -108,15 +86,15 @@
     inputs_channel_order=ChannelOrder.TENSORFLOW,
     outputs_channel_order=ChannelOrder.TENSORFLOW
 )
 ````
 
 Aaaand done! That's all it takes to... wait, what's that?
 
-<img src="docs/essentials1.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/essentials1.svg" width="100%">
 
 Nobuco says it doesn't know how to handle hard sigmoid.
 Apparently, it's our job to provide a node converter for either `F.hardsigmoid` or the enclosing `Hardsigmoid` module (or the entire `MyModule`, but that makes little sense). Here, we'll go for the former.
 
 Conversion is done directly. No layers upon layers of abstraction, no obscure intermediate representation. 
 A node converter is just a `Callable` that takes in the same arguments as the corresponding node in pytorch and outputs an equivalent node in tensorflow. 
 The converted node preserves the original node's signature, but pytorch tensors replaced with tensorflow counterparts (be that `tf.Tensor`, `KerasTensor`, `tf.Variable`, or `ResourceVariable`).
@@ -125,31 +103,31 @@
 
 ````python
 @nobuco.converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def hardsigmoid(input: torch.Tensor, inplace: bool = False):
     return lambda input, inplace=False: tf.keras.activations.hard_sigmoid(input)
 ````
 
-<img src="docs/essentials2.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/essentials2.svg" width="100%">
 
-It works, but the outputs don't quite match. Perhaps we should check on how [pytorch](https://pytorch.org/docs/stable/generated/torch.nn.functional.hardsigmoid.html) and [tensorflow](https://www.tensorflow.org/api_docs/python/tf/keras/activations/hard_sigmoid) define hard sigmoid. 
+It works, but the outputs don't quite match. Perhaps we should check on how [pytorch](https://pytorch.org/https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/stable/generated/torch.nn.functional.hardsigmoid.html) and [tensorflow](https://www.tensorflow.org/api_https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/python/tf/keras/activations/hard_sigmoid) define hard sigmoid. 
 And sure enough, their implementations differ. Have to type in the formula manually, I guess...
 
 ````python
 @nobuco.converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def hardsigmoid(input: torch.Tensor, inplace: bool = False):
     return lambda input, inplace=False: tf.clip_by_value(input/6 + 1/2, clip_value_min=0, clip_value_max=1)
 ````
 
-<img src="docs/essentials3.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/essentials3.svg" width="100%">
 
 And the happy result:
 
 <p align="center">
-<img src="docs/tutorial.png" width="30%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/tutorial.png" width="30%">
 </p>
 
 The example above is artificial but it illustrates the point.
 It's not feasible to provide a node converter for every existing pytorch op. There's literally [thousands](https://dev-discuss.pytorch.org/t/where-do-the-2000-pytorch-operators-come-from-more-than-you-wanted-to-know/) of them! 
 Best we can do without the converter constantly lacking essential functionality, being riddled with bugs, doing weird stuff and breaking apart with every other PT/TF release 
 is to keep the tool simple and customizable, make it clear where a problem comes from and let the _user_ sort things out.
 Usually it's easy for a human to translate an isolated operation from one framework to another.
@@ -219,28 +197,28 @@
     inputs_channel_order=ChannelOrder.PYTORCH,
 )
 ```
 
 The laziness shoots us in the foot here, and we get not one transpose but two:
 
 <p align="center">
-<img src="docs/channel_ordering.png" width="30%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/channel_ordering.png" width="30%">
 </p>
 
 For such occasions, there's two brethren functions: `force_tensorflow_order` and `force_pytorch_order`.
 
 ```python
 x, hx = self.gru(x)
 x = nobuco.force_tensorflow_order(x)
 x1 = self.conv1(x)
 x2 = self.conv2(x)
 ```
 
 <p align="center">
-<img src="docs/channel_ordering_forced.png" width="30%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/channel_ordering_forced.png" width="30%">
 </p>
 
 In case you are curious, the implementation is trivial:
 
 ```python
 @nobuco.traceable
 def force_tensorflow_order(inputs):
@@ -262,48 +240,48 @@
 class MyModule(nn.Module):
     def forward(self, x):
         x[:, 1:2, 16:25, 8::2] *= 2
         torch.relu_(x)
         return x
 ```
 
-<img src="docs/inplace1.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/inplace1.svg" width="100%">
 
 However, applying in-place operation to a slice yields incorrect result. What gives?
 
 ```python
 class MyModule(nn.Module):
     def forward(self, x):
         torch.relu_(x[:, 1:2, 16:25, 8::2])
         return x
 ```
 
-<img src="docs/inplace2.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/inplace2.svg" width="100%">
 
 You see, tensorflow graphs (and many other formats like ONNX) do not support in-place ops.
 So when we take slice (`x[:, 1:2, 16:25, 8::2]`) in TF/ONNX, the result is not a view of the original tensor but a copy. 
 This copy is then passed to `relu` (which is not in-place either), and its result is not used anywhere. 
 As you can see above, the output tensors of `__getitem__` and `relu_` are <span style="color:gray">grayed out</span>, and these operations are excluded from the graph.
 In fact, it's empty:
 
 <p align="center">
-<img src="docs/inplace_empty.png" width="30%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/inplace_empty.png" width="30%">
 </p>
 
 The easiest way of fixing this is to explicitly assign the result to the slice.
 Conveniently enough, most standard in-place operations in pytorch do return their modified arguments as outputs.
 
 ```python
 class MyModule(nn.Module):
     def forward(self, x):
         x[:, 1:2, 16:25, 8::2] = torch.relu_(x[:, 1:2, 16:25, 8::2])
         return x
 ```
 
-<img src="docs/inplace3.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/inplace3.svg" width="100%">
 
 ## Going dynamic
 
 ### Control flows
 Introducing python control flow statements into the compute graph is no easy feat.
 Tensorflow can do so via `tf.autograph`, but at a cost of [system's complexity](https://www.youtube.com/watch?v=NIEgzljyDyI) and with some notable [limitations](https://github.com/tensorflow/tensorflow/blob/master/tensorflow/python/autograph/g3doc/reference/control_flow.md).
 Stuff like that is way above Nobuco's paygrade, so the following module cannot be properly handled without human intervention.
@@ -385,15 +363,15 @@
     conv_false, out_false = nobuco.pytorch_to_keras(self.conv_false, [out_pre], **kwargs)
     conv_shared, _ = nobuco.pytorch_to_keras(self.conv_shared, [out_true], **kwargs)
     layer = ControlIfKeras(conv_pre, conv_true, conv_false, conv_shared)
     return layer
 ```
 
 <p align="center">
-<img src="docs/control_if.png" width="25%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/control_if.png" width="25%">
 </p>
 
 See [examples](/examples) for other ways to convert control flow ops.
 
 ### Dynamic shapes
 
 What if we wanted our module to accept images of arbitrary height and width?
@@ -425,34 +403,34 @@
     inputs_channel_order=ChannelOrder.TENSORFLOW,
     outputs_channel_order=ChannelOrder.TENSORFLOW,
 )
 ```
 
 Something's not right. We don't see shape extraction ops in the debug output or the graph:
 
-<img src="docs/dynamic_shape1.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/dynamic_shape1.svg" width="100%">
 
 <p align="center">
-<img src="docs/dynamic_shape1.png" width="15%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/dynamic_shape1.png" width="15%">
 </p>
 
 That's not surprising, actually. 
 In pytorch, tensor shape is a tuple of regular integers, not tensors, so it's quite difficult to track them.
 `nobuco.shape` solves this problem.
-This function returns tensors, much like [`tf.shape`](https://www.tensorflow.org/api_docs/python/tf/shape) does:
+This function returns tensors, much like [`tf.shape`](https://www.tensorflow.org/api_https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/python/tf/shape) does:
 
 ```python
 # Allows for dynamic shape
 b, c, h, w = nobuco.shape(x)
 ```
 
-<img src="docs/dynamic_shape2.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/dynamic_shape2.svg" width="100%">
 
 <p align="center">
-<img src="docs/dynamic_shape2.png" width="30%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/dynamic_shape2.png" width="30%">
 </p>
 
 Also, take a moment to appreciate how elegant the solution is. 
 `nobuco.shape` is a one-liner that simply replaces each integer in shape tuple with a scalar tensor.
 No special treatment required!
 
 ```python
@@ -504,15 +482,15 @@
 
     def forward(self, x):
         x = self.conv(x)
         SliceReLU()(x)
         return x
 ```
 
-<img src="docs/converter_inside_converter1.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/converter_inside_converter1.svg" width="100%">
 
 In the previous section, we've seen it's possible to invoke a Nobuco converter inside another Nobuco converter.
 Can we embed some third-party converter? You bet! Why? Because it might just do what we need.
 Let's consider the standard route: pytorch -> onnx -> tensorflow, with the latter step done with [onnx-tf](https://github.com/onnx/onnx-tensorflow).
 This library likes transposing stuff so much, converting the whole graph with it may introduce intolerable inference overhead. Nonetheless, it does the job.
 A sensible tradeoff would be to wrap the problematic operation into its own `nn.Module` and give it a special treat, while handling everything else with Nobuco.
 
@@ -533,15 +511,15 @@
     onnx_model = onnx.load(onnx_path)
     tf_rep = prepare(onnx_model)
     tf_rep.export_graph(model_path)
     model = tf.keras.models.load_model(model_path)
     return keras.layers.Lambda(lambda x: model(input=x))
 ```
 
-<img src="docs/converter_inside_converter2.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/converter_inside_converter2.svg" width="100%">
 
 ## But was it worth it?
 
 Let's cut to the chase, here's the numbers.
 
 **mobilenet_v3_large** (26.8 Mb)
 
@@ -579,15 +557,15 @@
 
 Again, the graph obtained with `onnx_tf` is much slower on x86 CPU.
 Worse yet, on mobile processor, optimized TFLite delegates for both GPU and CPU failed.
 No transpose ops were added this time, so who's to blame?
 It suffices to see what `torch.onnx.export` gives us:
 
 <p align="center">
-  <img src="docs/slice_relu_onnx.png" width="100%">
+  <img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/slice_relu_onnx.png" width="100%">
   <b>slice_relu.onnx</b>
 </p>
 
 `onnx_tf` does a fair job optimizing the graph it's given,
 but combining consecutive `slice` ops seems to be too much to ask.
 It also leaves out garbage nodes sometimes (note the free-floating `While` in this example).
 
@@ -597,28 +575,26 @@
   <tr>
     <th>slice_relu_nobuco</th>
     <th>slice_relu_onnxtf</th>
   </tr>
   <tr>
     <td>
       <p align="center">
-        <img src="docs/slice_relu_nobuco.png" width="60%">
+        <img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/slice_relu_nobuco.png" width="60%">
       </p>
     </td>
     <td>
       <p align="center">
-        <img src="docs/slice_relu_onnxtf.png" width="60%">
+        <img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/slice_relu_onnxtf.png" width="60%">
       </p>
     </td>
   </tr>
 </table>
 
-## More nice things
-
-### Nobuco knowledge base
+## Nobuco knowledge base
 
 Don't want to convert anything but looking for a tensorflow equivalent of a certain pytorch node (operation or module)?
 Nobuco already implements quite a few node converters, most written in concise and (hopefully) understandable way.
 These are located in [nobuco/node_converters](https://github.com/AlexanderLutsenko/nobuco/tree/master/nobuco/node_converters),
 and there's a utility function to help you find what you need:
```

### Comparing `nobuco-0.5.5/README.md` & `nobuco-0.5.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-<img src="docs/nobuco.png">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/nobuco.png">
 <sup><a href="https://www.behance.net/diliajl">diliajl</a></sup>
 </p>
 
 **No** **Bu**llshit **Co**nverter is a tool that helps you translate pytorch models into tensorflow graphs without losing your mind.
 
 - Supports a wide range of architectures
   - [x] Control flow ops (If, While)
@@ -28,16 +28,15 @@
 - [Channel order wizardry](#channel-order-wizardry)
 - [In-place operations](#in-place-operations)
 - [Going dynamic](#going-dynamic)
   - [Control flows](#control-flows)
   - [Dynamic shapes](#dynamic-shapes)
 - [So we put a converter inside your converter](#so-we-put-a-converter-inside-your-converter)
 - [But was it worth it?](#but-was-it-worth-it)
-- [More nice things](#more-nice-things)
-  - [Nobuco knowledge base](#nobuco-knowledge-base)
+- [Nobuco knowledge base](#nobuco-knowledge-base)
 
 <!-- tocstop -->
 
 ## Essentials
 
 Suppose we want to convert a pytorch module similar to this one:
 
@@ -72,15 +71,15 @@
     inputs_channel_order=ChannelOrder.TENSORFLOW,
     outputs_channel_order=ChannelOrder.TENSORFLOW
 )
 ````
 
 Aaaand done! That's all it takes to... wait, what's that?
 
-<img src="docs/essentials1.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/essentials1.svg" width="100%">
 
 Nobuco says it doesn't know how to handle hard sigmoid.
 Apparently, it's our job to provide a node converter for either `F.hardsigmoid` or the enclosing `Hardsigmoid` module (or the entire `MyModule`, but that makes little sense). Here, we'll go for the former.
 
 Conversion is done directly. No layers upon layers of abstraction, no obscure intermediate representation. 
 A node converter is just a `Callable` that takes in the same arguments as the corresponding node in pytorch and outputs an equivalent node in tensorflow. 
 The converted node preserves the original node's signature, but pytorch tensors replaced with tensorflow counterparts (be that `tf.Tensor`, `KerasTensor`, `tf.Variable`, or `ResourceVariable`).
@@ -89,31 +88,31 @@
 
 ````python
 @nobuco.converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def hardsigmoid(input: torch.Tensor, inplace: bool = False):
     return lambda input, inplace=False: tf.keras.activations.hard_sigmoid(input)
 ````
 
-<img src="docs/essentials2.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/essentials2.svg" width="100%">
 
-It works, but the outputs don't quite match. Perhaps we should check on how [pytorch](https://pytorch.org/docs/stable/generated/torch.nn.functional.hardsigmoid.html) and [tensorflow](https://www.tensorflow.org/api_docs/python/tf/keras/activations/hard_sigmoid) define hard sigmoid. 
+It works, but the outputs don't quite match. Perhaps we should check on how [pytorch](https://pytorch.org/https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/stable/generated/torch.nn.functional.hardsigmoid.html) and [tensorflow](https://www.tensorflow.org/api_https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/python/tf/keras/activations/hard_sigmoid) define hard sigmoid. 
 And sure enough, their implementations differ. Have to type in the formula manually, I guess...
 
 ````python
 @nobuco.converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def hardsigmoid(input: torch.Tensor, inplace: bool = False):
     return lambda input, inplace=False: tf.clip_by_value(input/6 + 1/2, clip_value_min=0, clip_value_max=1)
 ````
 
-<img src="docs/essentials3.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/essentials3.svg" width="100%">
 
 And the happy result:
 
 <p align="center">
-<img src="docs/tutorial.png" width="30%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/tutorial.png" width="30%">
 </p>
 
 The example above is artificial but it illustrates the point.
 It's not feasible to provide a node converter for every existing pytorch op. There's literally [thousands](https://dev-discuss.pytorch.org/t/where-do-the-2000-pytorch-operators-come-from-more-than-you-wanted-to-know/) of them! 
 Best we can do without the converter constantly lacking essential functionality, being riddled with bugs, doing weird stuff and breaking apart with every other PT/TF release 
 is to keep the tool simple and customizable, make it clear where a problem comes from and let the _user_ sort things out.
 Usually it's easy for a human to translate an isolated operation from one framework to another.
@@ -183,28 +182,28 @@
     inputs_channel_order=ChannelOrder.PYTORCH,
 )
 ```
 
 The laziness shoots us in the foot here, and we get not one transpose but two:
 
 <p align="center">
-<img src="docs/channel_ordering.png" width="30%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/channel_ordering.png" width="30%">
 </p>
 
 For such occasions, there's two brethren functions: `force_tensorflow_order` and `force_pytorch_order`.
 
 ```python
 x, hx = self.gru(x)
 x = nobuco.force_tensorflow_order(x)
 x1 = self.conv1(x)
 x2 = self.conv2(x)
 ```
 
 <p align="center">
-<img src="docs/channel_ordering_forced.png" width="30%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/channel_ordering_forced.png" width="30%">
 </p>
 
 In case you are curious, the implementation is trivial:
 
 ```python
 @nobuco.traceable
 def force_tensorflow_order(inputs):
@@ -226,48 +225,48 @@
 class MyModule(nn.Module):
     def forward(self, x):
         x[:, 1:2, 16:25, 8::2] *= 2
         torch.relu_(x)
         return x
 ```
 
-<img src="docs/inplace1.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/inplace1.svg" width="100%">
 
 However, applying in-place operation to a slice yields incorrect result. What gives?
 
 ```python
 class MyModule(nn.Module):
     def forward(self, x):
         torch.relu_(x[:, 1:2, 16:25, 8::2])
         return x
 ```
 
-<img src="docs/inplace2.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/inplace2.svg" width="100%">
 
 You see, tensorflow graphs (and many other formats like ONNX) do not support in-place ops.
 So when we take slice (`x[:, 1:2, 16:25, 8::2]`) in TF/ONNX, the result is not a view of the original tensor but a copy. 
 This copy is then passed to `relu` (which is not in-place either), and its result is not used anywhere. 
 As you can see above, the output tensors of `__getitem__` and `relu_` are <span style="color:gray">grayed out</span>, and these operations are excluded from the graph.
 In fact, it's empty:
 
 <p align="center">
-<img src="docs/inplace_empty.png" width="30%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/inplace_empty.png" width="30%">
 </p>
 
 The easiest way of fixing this is to explicitly assign the result to the slice.
 Conveniently enough, most standard in-place operations in pytorch do return their modified arguments as outputs.
 
 ```python
 class MyModule(nn.Module):
     def forward(self, x):
         x[:, 1:2, 16:25, 8::2] = torch.relu_(x[:, 1:2, 16:25, 8::2])
         return x
 ```
 
-<img src="docs/inplace3.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/inplace3.svg" width="100%">
 
 ## Going dynamic
 
 ### Control flows
 Introducing python control flow statements into the compute graph is no easy feat.
 Tensorflow can do so via `tf.autograph`, but at a cost of [system's complexity](https://www.youtube.com/watch?v=NIEgzljyDyI) and with some notable [limitations](https://github.com/tensorflow/tensorflow/blob/master/tensorflow/python/autograph/g3doc/reference/control_flow.md).
 Stuff like that is way above Nobuco's paygrade, so the following module cannot be properly handled without human intervention.
@@ -349,15 +348,15 @@
     conv_false, out_false = nobuco.pytorch_to_keras(self.conv_false, [out_pre], **kwargs)
     conv_shared, _ = nobuco.pytorch_to_keras(self.conv_shared, [out_true], **kwargs)
     layer = ControlIfKeras(conv_pre, conv_true, conv_false, conv_shared)
     return layer
 ```
 
 <p align="center">
-<img src="docs/control_if.png" width="25%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/control_if.png" width="25%">
 </p>
 
 See [examples](/examples) for other ways to convert control flow ops.
 
 ### Dynamic shapes
 
 What if we wanted our module to accept images of arbitrary height and width?
@@ -389,34 +388,34 @@
     inputs_channel_order=ChannelOrder.TENSORFLOW,
     outputs_channel_order=ChannelOrder.TENSORFLOW,
 )
 ```
 
 Something's not right. We don't see shape extraction ops in the debug output or the graph:
 
-<img src="docs/dynamic_shape1.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/dynamic_shape1.svg" width="100%">
 
 <p align="center">
-<img src="docs/dynamic_shape1.png" width="15%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/dynamic_shape1.png" width="15%">
 </p>
 
 That's not surprising, actually. 
 In pytorch, tensor shape is a tuple of regular integers, not tensors, so it's quite difficult to track them.
 `nobuco.shape` solves this problem.
-This function returns tensors, much like [`tf.shape`](https://www.tensorflow.org/api_docs/python/tf/shape) does:
+This function returns tensors, much like [`tf.shape`](https://www.tensorflow.org/api_https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/python/tf/shape) does:
 
 ```python
 # Allows for dynamic shape
 b, c, h, w = nobuco.shape(x)
 ```
 
-<img src="docs/dynamic_shape2.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/dynamic_shape2.svg" width="100%">
 
 <p align="center">
-<img src="docs/dynamic_shape2.png" width="30%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/dynamic_shape2.png" width="30%">
 </p>
 
 Also, take a moment to appreciate how elegant the solution is. 
 `nobuco.shape` is a one-liner that simply replaces each integer in shape tuple with a scalar tensor.
 No special treatment required!
 
 ```python
@@ -468,15 +467,15 @@
 
     def forward(self, x):
         x = self.conv(x)
         SliceReLU()(x)
         return x
 ```
 
-<img src="docs/converter_inside_converter1.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/converter_inside_converter1.svg" width="100%">
 
 In the previous section, we've seen it's possible to invoke a Nobuco converter inside another Nobuco converter.
 Can we embed some third-party converter? You bet! Why? Because it might just do what we need.
 Let's consider the standard route: pytorch -> onnx -> tensorflow, with the latter step done with [onnx-tf](https://github.com/onnx/onnx-tensorflow).
 This library likes transposing stuff so much, converting the whole graph with it may introduce intolerable inference overhead. Nonetheless, it does the job.
 A sensible tradeoff would be to wrap the problematic operation into its own `nn.Module` and give it a special treat, while handling everything else with Nobuco.
 
@@ -497,15 +496,15 @@
     onnx_model = onnx.load(onnx_path)
     tf_rep = prepare(onnx_model)
     tf_rep.export_graph(model_path)
     model = tf.keras.models.load_model(model_path)
     return keras.layers.Lambda(lambda x: model(input=x))
 ```
 
-<img src="docs/converter_inside_converter2.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/converter_inside_converter2.svg" width="100%">
 
 ## But was it worth it?
 
 Let's cut to the chase, here's the numbers.
 
 **mobilenet_v3_large** (26.8 Mb)
 
@@ -543,15 +542,15 @@
 
 Again, the graph obtained with `onnx_tf` is much slower on x86 CPU.
 Worse yet, on mobile processor, optimized TFLite delegates for both GPU and CPU failed.
 No transpose ops were added this time, so who's to blame?
 It suffices to see what `torch.onnx.export` gives us:
 
 <p align="center">
-  <img src="docs/slice_relu_onnx.png" width="100%">
+  <img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/slice_relu_onnx.png" width="100%">
   <b>slice_relu.onnx</b>
 </p>
 
 `onnx_tf` does a fair job optimizing the graph it's given,
 but combining consecutive `slice` ops seems to be too much to ask.
 It also leaves out garbage nodes sometimes (note the free-floating `While` in this example).
 
@@ -561,28 +560,26 @@
   <tr>
     <th>slice_relu_nobuco</th>
     <th>slice_relu_onnxtf</th>
   </tr>
   <tr>
     <td>
       <p align="center">
-        <img src="docs/slice_relu_nobuco.png" width="60%">
+        <img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/slice_relu_nobuco.png" width="60%">
       </p>
     </td>
     <td>
       <p align="center">
-        <img src="docs/slice_relu_onnxtf.png" width="60%">
+        <img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/slice_relu_onnxtf.png" width="60%">
       </p>
     </td>
   </tr>
 </table>
 
-## More nice things
-
-### Nobuco knowledge base
+## Nobuco knowledge base
 
 Don't want to convert anything but looking for a tensorflow equivalent of a certain pytorch node (operation or module)?
 Nobuco already implements quite a few node converters, most written in concise and (hopefully) understandable way.
 These are located in [nobuco/node_converters](https://github.com/AlexanderLutsenko/nobuco/tree/master/nobuco/node_converters),
 and there's a utility function to help you find what you need:
```

### Comparing `nobuco-0.5.5/nobuco/__init__.py` & `nobuco-0.5.6/nobuco/__init__.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/commons.py` & `nobuco-0.5.6/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/convert.py` & `nobuco-0.5.6/nobuco/convert.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/converters/channel_ordering.py` & `nobuco-0.5.6/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/converters/node_converter.py` & `nobuco-0.5.6/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/converters/tensor.py` & `nobuco-0.5.6/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/converters/type_cast.py` & `nobuco-0.5.6/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/converters/validation.py` & `nobuco-0.5.6/nobuco/converters/validation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/entity/keras.py` & `nobuco-0.5.6/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/entity/pytorch.py` & `nobuco-0.5.6/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/funcs.py` & `nobuco-0.5.6/nobuco/funcs.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/layers/channel_order.py` & `nobuco-0.5.6/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/layers/container.py` & `nobuco-0.5.6/nobuco/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/layers/weight.py` & `nobuco-0.5.6/nobuco/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/locate/link.py` & `nobuco-0.5.6/nobuco/locate/link.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/locate/locate.py` & `nobuco-0.5.6/nobuco/locate/locate.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/node_converters/activation.py` & `nobuco-0.5.6/nobuco/node_converters/activation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/node_converters/attention.py` & `nobuco-0.5.6/nobuco/node_converters/attention.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/node_converters/boolean.py` & `nobuco-0.5.6/nobuco/node_converters/boolean.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/node_converters/boolean_mask.py` & `nobuco-0.5.6/nobuco/node_converters/boolean_mask.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/node_converters/comparison.py` & `nobuco-0.5.6/nobuco/node_converters/comparison.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/node_converters/convolution.py` & `nobuco-0.5.6/nobuco/node_converters/convolution.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/node_converters/dropout.py` & `nobuco-0.5.6/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/node_converters/interpolation.py` & `nobuco-0.5.6/nobuco/node_converters/interpolation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/node_converters/linear.py` & `nobuco-0.5.6/nobuco/node_converters/linear.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/node_converters/math.py` & `nobuco-0.5.6/nobuco/node_converters/math.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/node_converters/misc.py` & `nobuco-0.5.6/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/node_converters/normalization.py` & `nobuco-0.5.6/nobuco/node_converters/normalization.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/node_converters/padding.py` & `nobuco-0.5.6/nobuco/node_converters/padding.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/node_converters/pooling.py` & `nobuco-0.5.6/nobuco/node_converters/pooling.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/node_converters/recurrent.py` & `nobuco-0.5.6/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/node_converters/slice.py` & `nobuco-0.5.6/nobuco/node_converters/slice.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/node_converters/tensor_cast.py` & `nobuco-0.5.6/nobuco/node_converters/tensor_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/node_converters/tensor_creation.py` & `nobuco-0.5.6/nobuco/node_converters/tensor_creation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.5.6/nobuco/node_converters/tensor_manipulation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/trace/tensor_storage.py` & `nobuco-0.5.6/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/trace/trace.py` & `nobuco-0.5.6/nobuco/trace/trace.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/util.py` & `nobuco-0.5.6/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/vis/console_stylizer.py` & `nobuco-0.5.6/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco/vis/html_stylizer.py` & `nobuco-0.5.6/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/nobuco.egg-info/PKG-INFO` & `nobuco-0.5.6/nobuco.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,24 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.5.5
-Summary: Pytorch to Tensorflow conversion made somewhat easy
+Version: 0.5.6
+Summary: Pytorch to Tensorflow conversion made intuitive
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 Alexander Lutsenko
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
 Project-URL: Homepage, https://github.com/AlexanderLutsenko/nobuco
 Project-URL: Bug Tracker, https://github.com/AlexanderLutsenko/nobuco/issues
 Keywords: pytorch,tensorflow,keras,converter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-<img src="docs/nobuco.png">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/nobuco.png">
 <sup><a href="https://www.behance.net/diliajl">diliajl</a></sup>
 </p>
 
 **No** **Bu**llshit **Co**nverter is a tool that helps you translate pytorch models into tensorflow graphs without losing your mind.
 
 - Supports a wide range of architectures
   - [x] Control flow ops (If, While)
@@ -64,16 +43,15 @@
 - [Channel order wizardry](#channel-order-wizardry)
 - [In-place operations](#in-place-operations)
 - [Going dynamic](#going-dynamic)
   - [Control flows](#control-flows)
   - [Dynamic shapes](#dynamic-shapes)
 - [So we put a converter inside your converter](#so-we-put-a-converter-inside-your-converter)
 - [But was it worth it?](#but-was-it-worth-it)
-- [More nice things](#more-nice-things)
-  - [Nobuco knowledge base](#nobuco-knowledge-base)
+- [Nobuco knowledge base](#nobuco-knowledge-base)
 
 <!-- tocstop -->
 
 ## Essentials
 
 Suppose we want to convert a pytorch module similar to this one:
 
@@ -108,15 +86,15 @@
     inputs_channel_order=ChannelOrder.TENSORFLOW,
     outputs_channel_order=ChannelOrder.TENSORFLOW
 )
 ````
 
 Aaaand done! That's all it takes to... wait, what's that?
 
-<img src="docs/essentials1.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/essentials1.svg" width="100%">
 
 Nobuco says it doesn't know how to handle hard sigmoid.
 Apparently, it's our job to provide a node converter for either `F.hardsigmoid` or the enclosing `Hardsigmoid` module (or the entire `MyModule`, but that makes little sense). Here, we'll go for the former.
 
 Conversion is done directly. No layers upon layers of abstraction, no obscure intermediate representation. 
 A node converter is just a `Callable` that takes in the same arguments as the corresponding node in pytorch and outputs an equivalent node in tensorflow. 
 The converted node preserves the original node's signature, but pytorch tensors replaced with tensorflow counterparts (be that `tf.Tensor`, `KerasTensor`, `tf.Variable`, or `ResourceVariable`).
@@ -125,31 +103,31 @@
 
 ````python
 @nobuco.converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def hardsigmoid(input: torch.Tensor, inplace: bool = False):
     return lambda input, inplace=False: tf.keras.activations.hard_sigmoid(input)
 ````
 
-<img src="docs/essentials2.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/essentials2.svg" width="100%">
 
-It works, but the outputs don't quite match. Perhaps we should check on how [pytorch](https://pytorch.org/docs/stable/generated/torch.nn.functional.hardsigmoid.html) and [tensorflow](https://www.tensorflow.org/api_docs/python/tf/keras/activations/hard_sigmoid) define hard sigmoid. 
+It works, but the outputs don't quite match. Perhaps we should check on how [pytorch](https://pytorch.org/https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/stable/generated/torch.nn.functional.hardsigmoid.html) and [tensorflow](https://www.tensorflow.org/api_https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/python/tf/keras/activations/hard_sigmoid) define hard sigmoid. 
 And sure enough, their implementations differ. Have to type in the formula manually, I guess...
 
 ````python
 @nobuco.converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def hardsigmoid(input: torch.Tensor, inplace: bool = False):
     return lambda input, inplace=False: tf.clip_by_value(input/6 + 1/2, clip_value_min=0, clip_value_max=1)
 ````
 
-<img src="docs/essentials3.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/essentials3.svg" width="100%">
 
 And the happy result:
 
 <p align="center">
-<img src="docs/tutorial.png" width="30%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/tutorial.png" width="30%">
 </p>
 
 The example above is artificial but it illustrates the point.
 It's not feasible to provide a node converter for every existing pytorch op. There's literally [thousands](https://dev-discuss.pytorch.org/t/where-do-the-2000-pytorch-operators-come-from-more-than-you-wanted-to-know/) of them! 
 Best we can do without the converter constantly lacking essential functionality, being riddled with bugs, doing weird stuff and breaking apart with every other PT/TF release 
 is to keep the tool simple and customizable, make it clear where a problem comes from and let the _user_ sort things out.
 Usually it's easy for a human to translate an isolated operation from one framework to another.
@@ -219,28 +197,28 @@
     inputs_channel_order=ChannelOrder.PYTORCH,
 )
 ```
 
 The laziness shoots us in the foot here, and we get not one transpose but two:
 
 <p align="center">
-<img src="docs/channel_ordering.png" width="30%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/channel_ordering.png" width="30%">
 </p>
 
 For such occasions, there's two brethren functions: `force_tensorflow_order` and `force_pytorch_order`.
 
 ```python
 x, hx = self.gru(x)
 x = nobuco.force_tensorflow_order(x)
 x1 = self.conv1(x)
 x2 = self.conv2(x)
 ```
 
 <p align="center">
-<img src="docs/channel_ordering_forced.png" width="30%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/channel_ordering_forced.png" width="30%">
 </p>
 
 In case you are curious, the implementation is trivial:
 
 ```python
 @nobuco.traceable
 def force_tensorflow_order(inputs):
@@ -262,48 +240,48 @@
 class MyModule(nn.Module):
     def forward(self, x):
         x[:, 1:2, 16:25, 8::2] *= 2
         torch.relu_(x)
         return x
 ```
 
-<img src="docs/inplace1.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/inplace1.svg" width="100%">
 
 However, applying in-place operation to a slice yields incorrect result. What gives?
 
 ```python
 class MyModule(nn.Module):
     def forward(self, x):
         torch.relu_(x[:, 1:2, 16:25, 8::2])
         return x
 ```
 
-<img src="docs/inplace2.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/inplace2.svg" width="100%">
 
 You see, tensorflow graphs (and many other formats like ONNX) do not support in-place ops.
 So when we take slice (`x[:, 1:2, 16:25, 8::2]`) in TF/ONNX, the result is not a view of the original tensor but a copy. 
 This copy is then passed to `relu` (which is not in-place either), and its result is not used anywhere. 
 As you can see above, the output tensors of `__getitem__` and `relu_` are <span style="color:gray">grayed out</span>, and these operations are excluded from the graph.
 In fact, it's empty:
 
 <p align="center">
-<img src="docs/inplace_empty.png" width="30%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/inplace_empty.png" width="30%">
 </p>
 
 The easiest way of fixing this is to explicitly assign the result to the slice.
 Conveniently enough, most standard in-place operations in pytorch do return their modified arguments as outputs.
 
 ```python
 class MyModule(nn.Module):
     def forward(self, x):
         x[:, 1:2, 16:25, 8::2] = torch.relu_(x[:, 1:2, 16:25, 8::2])
         return x
 ```
 
-<img src="docs/inplace3.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/inplace3.svg" width="100%">
 
 ## Going dynamic
 
 ### Control flows
 Introducing python control flow statements into the compute graph is no easy feat.
 Tensorflow can do so via `tf.autograph`, but at a cost of [system's complexity](https://www.youtube.com/watch?v=NIEgzljyDyI) and with some notable [limitations](https://github.com/tensorflow/tensorflow/blob/master/tensorflow/python/autograph/g3doc/reference/control_flow.md).
 Stuff like that is way above Nobuco's paygrade, so the following module cannot be properly handled without human intervention.
@@ -385,15 +363,15 @@
     conv_false, out_false = nobuco.pytorch_to_keras(self.conv_false, [out_pre], **kwargs)
     conv_shared, _ = nobuco.pytorch_to_keras(self.conv_shared, [out_true], **kwargs)
     layer = ControlIfKeras(conv_pre, conv_true, conv_false, conv_shared)
     return layer
 ```
 
 <p align="center">
-<img src="docs/control_if.png" width="25%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/control_if.png" width="25%">
 </p>
 
 See [examples](/examples) for other ways to convert control flow ops.
 
 ### Dynamic shapes
 
 What if we wanted our module to accept images of arbitrary height and width?
@@ -425,34 +403,34 @@
     inputs_channel_order=ChannelOrder.TENSORFLOW,
     outputs_channel_order=ChannelOrder.TENSORFLOW,
 )
 ```
 
 Something's not right. We don't see shape extraction ops in the debug output or the graph:
 
-<img src="docs/dynamic_shape1.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/dynamic_shape1.svg" width="100%">
 
 <p align="center">
-<img src="docs/dynamic_shape1.png" width="15%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/dynamic_shape1.png" width="15%">
 </p>
 
 That's not surprising, actually. 
 In pytorch, tensor shape is a tuple of regular integers, not tensors, so it's quite difficult to track them.
 `nobuco.shape` solves this problem.
-This function returns tensors, much like [`tf.shape`](https://www.tensorflow.org/api_docs/python/tf/shape) does:
+This function returns tensors, much like [`tf.shape`](https://www.tensorflow.org/api_https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/python/tf/shape) does:
 
 ```python
 # Allows for dynamic shape
 b, c, h, w = nobuco.shape(x)
 ```
 
-<img src="docs/dynamic_shape2.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/dynamic_shape2.svg" width="100%">
 
 <p align="center">
-<img src="docs/dynamic_shape2.png" width="30%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/dynamic_shape2.png" width="30%">
 </p>
 
 Also, take a moment to appreciate how elegant the solution is. 
 `nobuco.shape` is a one-liner that simply replaces each integer in shape tuple with a scalar tensor.
 No special treatment required!
 
 ```python
@@ -504,15 +482,15 @@
 
     def forward(self, x):
         x = self.conv(x)
         SliceReLU()(x)
         return x
 ```
 
-<img src="docs/converter_inside_converter1.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/converter_inside_converter1.svg" width="100%">
 
 In the previous section, we've seen it's possible to invoke a Nobuco converter inside another Nobuco converter.
 Can we embed some third-party converter? You bet! Why? Because it might just do what we need.
 Let's consider the standard route: pytorch -> onnx -> tensorflow, with the latter step done with [onnx-tf](https://github.com/onnx/onnx-tensorflow).
 This library likes transposing stuff so much, converting the whole graph with it may introduce intolerable inference overhead. Nonetheless, it does the job.
 A sensible tradeoff would be to wrap the problematic operation into its own `nn.Module` and give it a special treat, while handling everything else with Nobuco.
 
@@ -533,15 +511,15 @@
     onnx_model = onnx.load(onnx_path)
     tf_rep = prepare(onnx_model)
     tf_rep.export_graph(model_path)
     model = tf.keras.models.load_model(model_path)
     return keras.layers.Lambda(lambda x: model(input=x))
 ```
 
-<img src="docs/converter_inside_converter2.svg" width="100%">
+<img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/converter_inside_converter2.svg" width="100%">
 
 ## But was it worth it?
 
 Let's cut to the chase, here's the numbers.
 
 **mobilenet_v3_large** (26.8 Mb)
 
@@ -579,15 +557,15 @@
 
 Again, the graph obtained with `onnx_tf` is much slower on x86 CPU.
 Worse yet, on mobile processor, optimized TFLite delegates for both GPU and CPU failed.
 No transpose ops were added this time, so who's to blame?
 It suffices to see what `torch.onnx.export` gives us:
 
 <p align="center">
-  <img src="docs/slice_relu_onnx.png" width="100%">
+  <img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/slice_relu_onnx.png" width="100%">
   <b>slice_relu.onnx</b>
 </p>
 
 `onnx_tf` does a fair job optimizing the graph it's given,
 but combining consecutive `slice` ops seems to be too much to ask.
 It also leaves out garbage nodes sometimes (note the free-floating `While` in this example).
 
@@ -597,28 +575,26 @@
   <tr>
     <th>slice_relu_nobuco</th>
     <th>slice_relu_onnxtf</th>
   </tr>
   <tr>
     <td>
       <p align="center">
-        <img src="docs/slice_relu_nobuco.png" width="60%">
+        <img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/slice_relu_nobuco.png" width="60%">
       </p>
     </td>
     <td>
       <p align="center">
-        <img src="docs/slice_relu_onnxtf.png" width="60%">
+        <img src="https://raw.githubusercontent.com/AlexanderLutsenko/nobuco/master/docs/slice_relu_onnxtf.png" width="60%">
       </p>
     </td>
   </tr>
 </table>
 
-## More nice things
-
-### Nobuco knowledge base
+## Nobuco knowledge base
 
 Don't want to convert anything but looking for a tensorflow equivalent of a certain pytorch node (operation or module)?
 Nobuco already implements quite a few node converters, most written in concise and (hopefully) understandable way.
 These are located in [nobuco/node_converters](https://github.com/AlexanderLutsenko/nobuco/tree/master/nobuco/node_converters),
 and there's a utility function to help you find what you need:
```

### Comparing `nobuco-0.5.5/nobuco.egg-info/SOURCES.txt` & `nobuco-0.5.6/nobuco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.5/pyproject.toml` & `nobuco-0.5.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.5.5"
-description = "Pytorch to Tensorflow conversion made somewhat easy"
+version = "0.5.6"
+description = "Pytorch to Tensorflow conversion made intuitive"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
-license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["pytorch", "tensorflow", "keras", "converter"]
 dependencies = [
```

