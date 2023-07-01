# Comparing `tmp/easy_local_features-0.2.3.tar.gz` & `tmp/easy_local_features-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_local_features-0.2.3.tar", last modified: Mon Jun 12 16:21:09 2023, max compression
+gzip compressed data, was "easy_local_features-0.3.0.tar", last modified: Sat Jul  1 17:24:56 2023, max compression
```

## Comparing `easy_local_features-0.2.3.tar` & `easy_local_features-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,82 @@
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 16:21:09.279602 easy_local_features-0.2.3/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      927 2023-06-12 16:21:09.279602 easy_local_features-0.2.3/PKG-INFO
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      773 2023-06-12 16:04:27.000000 easy_local_features-0.2.3/README.md
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 16:21:09.275602 easy_local_features-0.2.3/easy_local_features/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      335 2023-06-12 16:21:02.000000 easy_local_features-0.2.3/easy_local_features/__init__.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    34250 2023-06-12 15:41:05.000000 easy_local_features-0.2.3/easy_local_features/baseline_dalf.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2496 2023-06-12 15:18:17.000000 easy_local_features-0.2.3/easy_local_features/baseline_deal.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     6102 2023-06-09 08:29:10.000000 easy_local_features-0.2.3/easy_local_features/baseline_disk.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     4458 2023-06-09 08:29:10.000000 easy_local_features-0.2.3/easy_local_features/baseline_r2d2.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3979 2023-06-09 08:29:10.000000 easy_local_features-0.2.3/easy_local_features/baseline_superglue.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2063 2023-06-09 08:29:10.000000 easy_local_features-0.2.3/easy_local_features/baseline_superpoint.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 16:21:09.279602 easy_local_features-0.2.3/easy_local_features/datasets/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 07:43:29.000000 easy_local_features-0.2.3/easy_local_features/datasets/__init__.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3034 2023-06-12 07:45:31.000000 easy_local_features-0.2.3/easy_local_features/datasets/download.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 16:21:09.279602 easy_local_features-0.2.3/easy_local_features.egg-info/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      927 2023-06-12 16:21:09.000000 easy_local_features-0.2.3/easy_local_features.egg-info/PKG-INFO
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      575 2023-06-12 16:21:09.000000 easy_local_features-0.2.3/easy_local_features.egg-info/SOURCES.txt
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        1 2023-06-12 16:21:09.000000 easy_local_features-0.2.3/easy_local_features.egg-info/dependency_links.txt
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       20 2023-06-12 16:21:09.000000 easy_local_features-0.2.3/easy_local_features.egg-info/top_level.txt
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       38 2023-06-12 16:21:09.279602 easy_local_features-0.2.3/setup.cfg
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      760 2023-06-12 16:20:01.000000 easy_local_features-0.2.3/setup.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 16:21:09.279602 easy_local_features-0.2.3/tests/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      112 2023-06-12 16:01:43.000000 easy_local_features-0.2.3/tests/test_dalf.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      112 2023-06-12 16:01:22.000000 easy_local_features-0.2.3/tests/test_deal.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.709808 easy_local_features-0.3.0/
+-rw-r--r--   0 cadar      (501) staff       (20)    32722 2023-07-01 15:16:15.000000 easy_local_features-0.3.0/LICENSE_DISK.txt
+-rw-r--r--   0 cadar      (501) staff       (20)    21121 2023-07-01 17:04:24.000000 easy_local_features-0.3.0/LICENSE_R2D2.txt
+-rw-r--r--   0 cadar      (501) staff       (20)     7009 2023-07-01 16:24:52.000000 easy_local_features-0.3.0/LICENSE_SUPERGLUE.txt
+-rw-r--r--   0 cadar      (501) staff       (20)     1597 2023-07-01 17:24:56.709543 easy_local_features-0.3.0/PKG-INFO
+-rw-r--r--   0 cadar      (501) staff       (20)     1345 2023-07-01 17:24:12.000000 easy_local_features-0.3.0/README.md
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.696457 easy_local_features-0.3.0/easy_local_features/
+-rw-r--r--   0 cadar      (501) staff       (20)        1 2023-07-01 15:35:14.000000 easy_local_features-0.3.0/easy_local_features/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)    34250 2023-06-12 19:58:13.000000 easy_local_features-0.3.0/easy_local_features/baseline_dalf.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2624 2023-07-01 09:14:35.000000 easy_local_features-0.3.0/easy_local_features/baseline_deal.py
+-rw-r--r--   0 cadar      (501) staff       (20)     6746 2023-07-01 15:51:12.000000 easy_local_features-0.3.0/easy_local_features/baseline_disk.py
+-rw-r--r--   0 cadar      (501) staff       (20)     6012 2023-07-01 17:02:37.000000 easy_local_features-0.3.0/easy_local_features/baseline_r2d2.py
+-rw-r--r--   0 cadar      (501) staff       (20)     5116 2023-07-01 16:48:02.000000 easy_local_features-0.3.0/easy_local_features/baseline_superglue.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2857 2023-07-01 16:59:28.000000 easy_local_features-0.3.0/easy_local_features/baseline_superpoint.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.697523 easy_local_features-0.3.0/easy_local_features/datasets/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-06-12 19:58:13.000000 easy_local_features-0.3.0/easy_local_features/datasets/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     3034 2023-06-12 19:58:13.000000 easy_local_features-0.3.0/easy_local_features/datasets/download.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.697694 easy_local_features-0.3.0/easy_local_features/submodules/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:42:35.000000 easy_local_features-0.3.0/easy_local_features/submodules/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.697860 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:23:41.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.698012 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/
+-rw-r--r--   0 cadar      (501) staff       (20)       24 2023-07-01 15:39:51.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.698432 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/common/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:40:58.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/common/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2675 2023-07-01 08:54:41.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/common/structs.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.699742 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/geom/
+-rw-r--r--   0 cadar      (501) staff       (20)       79 2023-07-01 08:54:41.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/geom/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)      271 2023-07-01 08:54:41.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/geom/distance_matrix.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2253 2023-07-01 08:54:41.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/geom/epi.py
+-rw-r--r--   0 cadar      (501) staff       (20)     3377 2023-07-01 08:54:41.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/geom/pose.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.701372 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/model/
+-rw-r--r--   0 cadar      (501) staff       (20)      113 2023-07-01 08:54:41.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/model/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2744 2023-07-01 15:52:24.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2544 2023-07-01 15:34:26.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py
+-rw-r--r--   0 cadar      (501) staff       (20)     5573 2023-07-01 15:33:05.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/model/detector.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2265 2023-07-01 15:52:15.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/model/disk.py
+-rw-r--r--   0 cadar      (501) staff       (20)      881 2023-07-01 08:54:41.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_disk/disk/model/nms.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.702965 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:53:50.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     6223 2023-07-01 17:01:09.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/extract.py
+-rw-r--r--   0 cadar      (501) staff       (20)     9927 2023-07-01 16:26:30.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/extract_kapture.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.704634 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:54:54.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2360 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/ap_loss.py
+-rw-r--r--   0 cadar      (501) staff       (20)     1720 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/losses.py
+-rw-r--r--   0 cadar      (501) staff       (20)     7158 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/patchnet.py
+-rw-r--r--   0 cadar      (501) staff       (20)     1760 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/reliability_loss.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2006 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/repeatability_loss.py
+-rw-r--r--   0 cadar      (501) staff       (20)    15031 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/nets/sampler.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.706082 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:54:23.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     1080 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/common.py
+-rw-r--r--   0 cadar      (501) staff       (20)    14318 2023-07-01 17:00:44.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/dataloader.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2208 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/trainer.py
+-rw-r--r--   0 cadar      (501) staff       (20)    18298 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/transforms.py
+-rw-r--r--   0 cadar      (501) staff       (20)     7160 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/transforms_tools.py
+-rw-r--r--   0 cadar      (501) staff       (20)     5647 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/tools/viz.py
+-rw-r--r--   0 cadar      (501) staff       (20)     5018 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/train.py
+-rw-r--r--   0 cadar      (501) staff       (20)     4203 2023-07-01 16:26:31.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_r2d2/viz_heatmaps.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.706318 easy_local_features-0.3.0/easy_local_features/submodules/git_superglue/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:22:28.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_superglue/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.707414 easy_local_features-0.3.0/easy_local_features/submodules/git_superglue/models/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:16:09.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_superglue/models/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     3417 2023-07-01 16:16:09.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_superglue/models/matching.py
+-rw-r--r--   0 cadar      (501) staff       (20)    11537 2023-07-01 16:40:16.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_superglue/models/superglue.py
+-rw-r--r--   0 cadar      (501) staff       (20)     8092 2023-07-01 16:40:03.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_superglue/models/superpoint.py
+-rw-r--r--   0 cadar      (501) staff       (20)    20039 2023-07-01 16:16:09.000000 easy_local_features-0.3.0/easy_local_features/submodules/git_superglue/models/utils.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.697180 easy_local_features-0.3.0/easy_local_features.egg-info/
+-rw-r--r--   0 cadar      (501) staff       (20)     1597 2023-07-01 17:24:56.000000 easy_local_features-0.3.0/easy_local_features.egg-info/PKG-INFO
+-rw-r--r--   0 cadar      (501) staff       (20)     3094 2023-07-01 17:24:56.000000 easy_local_features-0.3.0/easy_local_features.egg-info/SOURCES.txt
+-rw-r--r--   0 cadar      (501) staff       (20)        1 2023-07-01 17:24:56.000000 easy_local_features-0.3.0/easy_local_features.egg-info/dependency_links.txt
+-rw-r--r--   0 cadar      (501) staff       (20)       20 2023-07-01 17:24:56.000000 easy_local_features-0.3.0/easy_local_features.egg-info/top_level.txt
+-rw-r--r--   0 cadar      (501) staff       (20)       38 2023-07-01 17:24:56.709863 easy_local_features-0.3.0/setup.cfg
+-rw-r--r--   0 cadar      (501) staff       (20)      760 2023-07-01 17:18:43.000000 easy_local_features-0.3.0/setup.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-01 17:24:56.709127 easy_local_features-0.3.0/tests/
+-rw-r--r--   0 cadar      (501) staff       (20)      146 2023-07-01 17:21:05.000000 easy_local_features-0.3.0/tests/test_dalf.py
+-rw-r--r--   0 cadar      (501) staff       (20)      146 2023-07-01 17:20:49.000000 easy_local_features-0.3.0/tests/test_deal.py
+-rw-r--r--   0 cadar      (501) staff       (20)      146 2023-07-01 17:20:35.000000 easy_local_features-0.3.0/tests/test_disk.py
+-rw-r--r--   0 cadar      (501) staff       (20)      146 2023-07-01 17:21:41.000000 easy_local_features-0.3.0/tests/test_r2d2.py
+-rw-r--r--   0 cadar      (501) staff       (20)      161 2023-07-01 17:21:58.000000 easy_local_features-0.3.0/tests/test_superglue.py
+-rw-r--r--   0 cadar      (501) staff       (20)      164 2023-07-01 17:22:12.000000 easy_local_features-0.3.0/tests/test_superpoint.py
```

### Comparing `easy_local_features-0.2.3/easy_local_features/baseline_dalf.py` & `easy_local_features-0.3.0/easy_local_features/baseline_dalf.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.2.3/easy_local_features/baseline_deal.py` & `easy_local_features-0.3.0/easy_local_features/baseline_deal.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 import cv2, os
 
 import pyrootutils
 root = pyrootutils.find_root()
 
 class DEAL_baseline():
-    def __init__(self, max_kps=1024, device_id=0, model_path=None):
+    def __init__(self, max_kps=1024, device_id=-1, model_path=None):
 
         self.max_kps = max_kps
         self.device_id = device_id
 
         if device_id >= 0:
             device = torch.device(f"cuda:{device_id}")
         else:
@@ -83,8 +83,12 @@
 
 if __name__ == "__main__":
     img = cv2.imread(str(root / "assets" / "notredame.png"))
     extractor = DEAL_baseline()
 
     keypoints0, descriptors0 = extractor.detectAndCompute(img)
     
-    print("keypoints0", len(keypoints0))
+    # Visualize keypoints
+    img_kpts = cv2.drawKeypoints(img, keypoints0, None, color=(0, 255, 0), flags=0)
+
+    cv2.imshow("Keypoints", img_kpts)
+    cv2.waitKey(0)
```

### Comparing `easy_local_features-0.2.3/easy_local_features/baseline_disk.py` & `easy_local_features-0.3.0/easy_local_features/baseline_disk.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-import sys, os
-disk_folder = os.path.dirname(os.path.realpath(__file__)) + '/submodules/git_disk/'
-sys.path.insert(0, disk_folder)
-from disk import DISK, Features
+import pyrootutils
+root = pyrootutils.find_root()
 
-import torch, h5py, imageio, os, argparse
+# disk_folder = str(root / 'easy_local_features' / 'submodules' / 'git_disk') + '/'
+
+from easy_local_features.submodules.git_disk.disk import DISK
+
+import torch
 import numpy as np
 import torch.nn.functional as F
 from functools import partial
-from tqdm import tqdm
-import cv2
+import cv2, os, wget
 
 class Image:
     def __init__(self, bitmap, orig_shape=None):
         self.bitmap     = bitmap
         if orig_shape is None:
             self.orig_shape = self.bitmap.shape[1:]
         else:
@@ -64,21 +65,37 @@
         if x_pad < 0 or y_pad < 0:
             raise ValueError("Attempting to pad by negative value")
 
         return F.pad(image, (0, y_pad, 0, x_pad))
 
 
 class DISK_baseline():
-    def __init__(self, window=8, desc_dim=128, mode='nms', max_feat=2048, model_path=disk_folder+'depth-save.pth', auto_resize=True):
-        self.DEV   = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+    def __init__(self, window=8, desc_dim=128, mode='nms', max_feat=2048, model_path=None, auto_resize=True, device=-1):
         self.CPU   = torch.device('cpu')
+        self.DEV   = torch.device(f'cuda:{device}' if (torch.cuda.is_available() and device >= 0) else 'cpu')
         self.auto_resize = auto_resize
         self.ratio = 0
 
         self.model = DISK(window=window, desc_dim=desc_dim)
+
+        if model_path is None:
+            url = 'https://github.com/cvlab-epfl/disk/raw/master/depth-save.pth'
+            cache_path = os.path.join(os.path.expanduser('~'), '.cache', 'torch', 'hub', 'checkpoints', 'DISK')
+            
+            if not os.path.exists(cache_path):
+                os.makedirs(cache_path, exist_ok=True)
+
+            cache_path = os.path.join(cache_path, 'depth-save.pth')
+            if not os.path.exists(cache_path):
+                print('Downloading DISK model...')
+                wget.download(url, cache_path)
+                print('Done.')
+
+            model_path = cache_path
+
         state_dict = torch.load(model_path, map_location='cpu')
 
         # print(state_dict.keys())
         self.model.load_state_dict(state_dict['extractor'])
         self.model = self.model.to(self.DEV)
         self.model.eval()
 
@@ -171,18 +188,18 @@
 
         features = features.to(self.CPU)
         descriptors = features.desc.numpy()
 
         # TODO convert KeyPoints to mask
 
 if __name__ == "__main__":
-    import pdb
-    img = cv2.imread("../assets/notredame.png")
-    img = cv2.resize(img, None, fx=0.9, fy=1)
+    img = cv2.imread(str(root / "assets" / "notredame.png"))
+    img = cv2.resize(img, (0,0), fx=0.5, fy=0.5)
 
     extractor = DISK_baseline()
 
     keypoints, descriptors = extractor.detectAndCompute(img)
 
     output_image = cv2.drawKeypoints(img, keypoints, 0, (0, 0, 255))
 
-    cv2.imwrite("disk_test.png", output_image)
+    cv2.imshow("output", output_image)
+    cv2.waitKey(0)
```

### Comparing `easy_local_features-0.2.3/easy_local_features/baseline_r2d2.py` & `easy_local_features-0.3.0/easy_local_features/baseline_r2d2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-import sys, os
-r2d2_folder = os.path.dirname(os.path.realpath(__file__)) + '/submodules/git_r2d2/'
-sys.path.insert(0, r2d2_folder)
-import os, pdb
-from PIL import Image
+import os
 import numpy as np
 import torch
+import wget
+import cv2
 
-from tools import common
-from tools.dataloader import norm_RGB
-from nets.patchnet import *
-from extract import load_network, NonMaxSuppression, extract_multiscale
+from easy_local_features.submodules.git_r2d2.tools import common
+from easy_local_features.submodules.git_r2d2.tools.dataloader import norm_RGB
+from easy_local_features.submodules.git_r2d2.nets.patchnet import *
+from easy_local_features.submodules.git_r2d2.extract import load_network, NonMaxSuppression, extract_multiscale
+
+# from tools import common
+# from tools.dataloader import norm_RGB
+# from nets.patchnet import *
+# from extract import load_network, NonMaxSuppression, extract_multiscale
 
-import torch
-import numpy as np
-from functools import partial
-import cv2
 
 # Pretrained models
 # -----------------
 # For your convenience, we provide five pre-trained models in the `models/` folder:
 #  - `r2d2_WAF_N16.pt`: this is the model used in most experiments of the paper (on HPatches `MMA@3=0.686`). It was trained with Web images (`W`), Aachen day-time images (`A`) and Aachen optical flow pairs (`F`)
 #  - `r2d2_WASF_N16.pt`: this is the model used in the visual localization experiments (on HPatches `MMA@3=0.721`). It was trained with Web images (`W`), Aachen day-time images (`A`), Aachen day-night synthetic pairs (`S`), and Aachen optical flow pairs (`F`).
 #  - `r2d2_WASF_N8_big.pt`: Same than previous model, but trained with `N=8` instead of `N=16` in the repeatability loss. In other words, it outputs a higher density of keypoints. This can be interesting for certain applications like visual localization, but it implies a drop in MMA since keypoints gets slighlty less reliable.
@@ -27,49 +26,74 @@
 
 # model name	model size  (#weights)	number of keypoints	MMA@3 on HPatches
 # r2d2_WAF_N16.pt	0.5M	5K	0.686
 # r2d2_WASF_N16.pt	0.5M	5K	0.721
 # r2d2_WASF_N8_big.pt	1.0M	10K	0.692
 # faster2d2_WASF_N8_big.pt	1.0M	5K	0.650
 
+models_URLs = {
+    'faster2d2_WASF_N8_big': 'https://github.com/naver/r2d2/raw/master/models/faster2d2_WASF_N16.pt',
+    'faster2d2_WASF_N16': 'https://github.com/naver/r2d2/raw/master/models/faster2d2_WASF_N8_big.pt',
+    'r2d2_WAF_N16': 'https://github.com/naver/r2d2/raw/master/models/r2d2_WAF_N16.pt',
+    'r2d2_WASF_N8_big': 'https://github.com/naver/r2d2/raw/master/models/r2d2_WASF_N16.pt',
+    'r2d2_WASF_N16': 'https://github.com/naver/r2d2/raw/master/models/r2d2_WASF_N8_big.pt',
+}
+
 RGB_mean = [0.485, 0.456, 0.406]
 RGB_std  = [0.229, 0.224, 0.225]
 
 class R2D2_baseline():
     def __init__(self,
                 max_keypoints=2048,
-                model_name='r2d2_WASF_N16.pt',
+                pretrained_weigts='r2d2_WASF_N16',
+                model_path=None,
+                device=-1,
                 rel_thr=0.7,
                 rep_thr=0.7,
                 scale_f=2**0.25,
                 min_scale=0.0,
                 max_scale=1,
                 min_size=256,
                 max_size=1024):
 
         self.top_k = max_keypoints
-        self.model_name = model_name
         self.rel_thr = rel_thr
         self.rep_thr = rep_thr
         self.scale_f = scale_f
         self.min_scale = min_scale
         self.max_scale = max_scale
         self.min_size = min_size
         self.max_size = max_size
 
-        self.DEV   = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+        self.DEV   = torch.device('cuda' if (torch.cuda.is_available() and device>=0) else 'cpu')
         self.CPU   = torch.device('cpu')
 
-        model_path = r2d2_folder + 'models/' + model_name
-
-        if torch.cuda.is_available():
+        if (torch.cuda.is_available() and device >= 0):
             iscuda = common.torch_set_gpu([0])
         else:
             iscuda = False
 
+        if model_path is None:
+            assert pretrained_weigts in list(models_URLs.keys()), f'If a model path is not defined, the pretrained_weigts should be one of: {list(models_URLs.keys())} '
+
+            url = models_URLs[pretrained_weigts]
+            cache_path = os.path.join(os.path.expanduser('~'), '.cache', 'torch', 'hub', 'checkpoints', 'R2D2')
+            model_name = url.split('/')[-1]
+            
+            if not os.path.exists(cache_path):
+                os.makedirs(cache_path, exist_ok=True)
+
+            cache_path = os.path.join(cache_path, model_name)
+            if not os.path.exists(cache_path):
+                print(f'Downloading R2D2 model...')
+                wget.download(url, cache_path)
+                print('Done.')
+
+            model_path = cache_path
+
         # load the network...
         self.net = load_network(model_path)
         if iscuda: self.net = self.net.cuda()
 
         # create the non-maxima detector
         self.detector = NonMaxSuppression(
             rel_thr = rel_thr, 
@@ -109,16 +133,20 @@
         cv_kps, descriptors = self.detectAndCompute(img)
         return cv_kps
 
     def compute(self, img, cv_kps):
         raise NotImplemented
 
 if __name__ == "__main__":
-    img = cv2.imread("assets/notredame.png")
-
+    import pyrootutils
+    root = pyrootutils.find_root()
+    
+    img = cv2.imread(str(root / "assets" / "notredame.png"))
+    img = cv2.resize(img, (0,0), fx=0.5, fy=0.5)
     extractor = R2D2_baseline()
 
     keypoints, descriptors = extractor.detectAndCompute(img)
 
     output_image = cv2.drawKeypoints(img, keypoints, 0, (0, 0, 255))
 
-    cv2.imwrite("r2d2_test.png", output_image)
+    cv2.imshow('img', output_image)
+    cv2.waitKey(0)
```

### Comparing `easy_local_features-0.2.3/easy_local_features/baseline_superglue.py` & `easy_local_features-0.3.0/easy_local_features/baseline_superglue.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,53 @@
 import sys, os
-sp_folder = os.path.dirname(os.path.realpath(__file__)) + '/submodules/git_superglue/'
-sys.path.insert(0, sp_folder)
-from models.superglue import SuperGlue
+
+from easy_local_features.submodules.git_superglue.models.superglue import SuperGlue
 
 import torch
 import numpy as np
 from functools import partial
 import cv2
+import wget
+import pyrootutils
+root = pyrootutils.find_root()
 
 class SuperGlue_baseline():
-    def __init__(self, weights='indoor', sinkhorn_iterations=100, match_threshold=0.2, descriptor_dim=256):
-        self.DEV   = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+    def __init__(self, weights='indoor', sinkhorn_iterations=100, match_threshold=0.2, descriptor_dim=256, device=-1, model_path=None):
+        self.DEV   = torch.device(f'cuda:{device}' if (torch.cuda.is_available() and device>=0) else 'cpu')
         self.CPU   = torch.device('cpu')
     
+        if model_path is None:
+            assert weights in ['indoor', 'outdoor'], "weights must be either 'indoor' or 'outdoor'"
+            if weights == 'indoor':
+                url = 'https://github.com/magicleap/SuperGluePretrainedNetwork/raw/master/models/weights/superglue_indoor.pth'
+            else: # outdoor
+                url = 'https://github.com/magicleap/SuperGluePretrainedNetwork/raw/master/models/weights/superglue_outdoor.pth'
+
+            cache_path = os.path.join(os.path.expanduser('~'), '.cache', 'torch', 'hub', 'checkpoints', 'SuperGlue')
+            model_name = url.split('/')[-1]
+            
+            if not os.path.exists(cache_path):
+                os.makedirs(cache_path, exist_ok=True)
+
+            cache_path = os.path.join(cache_path, model_name)
+            if not os.path.exists(cache_path):
+                print(f'Downloading SuperGlue {weights} model...')
+                wget.download(url, cache_path)
+                print('Done.')
+
+            model_path = cache_path        
+
         config = {
             'descriptor_dim': descriptor_dim,
             'weights': weights,
             'keypoint_encoder': [32, 64, 128, 256],
             'GNN_layers': ['self', 'cross'] * 9,
             'sinkhorn_iterations': sinkhorn_iterations,
             'match_threshold': match_threshold,
+            'model_path': model_path,
         }
 
         self.model = SuperGlue(config)
         self.model = self.model.to(self.DEV)
         self.model.eval()
 
     def _toTorch(self, img):
@@ -83,21 +107,21 @@
 
         return matches1to2, matches2to1
 
 if __name__ == "__main__":
     import pdb
     from baseline_superpoint import SuperPoint_baseline
 
-    img = cv2.imread("../assets/notredame.png")
+    img = cv2.imread(str(root / "assets" / "notredame.png"))
     extractor = SuperPoint_baseline()
     matcher = SuperGlue_baseline()
 
     keypoints0, descriptors0 = extractor.detectAndCompute(img)
     
     matches1to2, matches2to1 = matcher.match(img, keypoints0, descriptors0, img, keypoints0, descriptors0)
 
     matched_img1 = cv2.drawMatches(img, keypoints0, img, keypoints0, matches1to2, None)
     matched_img2 = cv2.drawMatches(img, keypoints0, img, keypoints0, matches2to1, None)
 
     stacked = np.vstack([matched_img1, matched_img2])
-
-    cv2.imwrite("sg_test.png", stacked)
+    cv2.imshow("matches", stacked)
+    cv2.waitKey(0)
```

### Comparing `easy_local_features-0.2.3/easy_local_features/baseline_superpoint.py` & `easy_local_features-0.3.0/easy_local_features/baseline_superpoint.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,46 @@
 import sys, os
-sp_folder = os.path.dirname(os.path.realpath(__file__)) + '/submodules/git_superglue/'
-sys.path.insert(0, sp_folder)
-from models.superpoint import SuperPoint
+from easy_local_features.submodules.git_superglue.models.superpoint import SuperPoint
 
 import torch
 import numpy as np
 from functools import partial
 import cv2
+import wget
+import pyrootutils
+root = pyrootutils.find_root()
 
 class SuperPoint_baseline():
-    def __init__(self, max_keypoints=2048, nms_radius=4, keypoint_threshold=0.005, remove_borders=4, descriptor_dim=256):
-        self.DEV   = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+    def __init__(self, max_keypoints=2048, nms_radius=4, keypoint_threshold=0.005, remove_borders=4, descriptor_dim=256, device=-1, model_path=None):
+        self.DEV   = torch.device('cuda' if (torch.cuda.is_available() and device>=0) else 'cpu')
         self.CPU   = torch.device('cpu')
-    
+
+        if model_path is None:
+            url = 'https://github.com/magicleap/SuperGluePretrainedNetwork/raw/master/models/weights/superpoint_v1.pth'
+            cache_path = os.path.join(os.path.expanduser('~'), '.cache', 'torch', 'hub', 'checkpoints', 'SuperPoint')
+            model_name = url.split('/')[-1]
+            
+            if not os.path.exists(cache_path):
+                os.makedirs(cache_path, exist_ok=True)
+
+            cache_path = os.path.join(cache_path, model_name)
+            if not os.path.exists(cache_path):
+                print(f'Downloading SuperPoint model...')
+                wget.download(url, cache_path)
+                print('Done.')
+
+            model_path = cache_path
+
         config = {
             'descriptor_dim': descriptor_dim,
             'nms_radius': nms_radius,
             'keypoint_threshold': keypoint_threshold,
             'max_keypoints': max_keypoints,
             'remove_borders': remove_borders,
+            'model_path': model_path,
         }
 
         self.model = SuperPoint(config)
         self.model = self.model.to(self.DEV)
         self.model.eval()
 
     def _toTorch(self, img):
@@ -47,16 +65,15 @@
         cv_kps, descriptors = self.detectAndCompute(img)
         return cv_kps
 
     def compute(self, img, cv_kps):
         raise NotImplemented
 
 if __name__ == "__main__":
-    import pdb
-    img = cv2.imread("../assets/notredame.png")
+    img = cv2.imread(str(root / "assets" / "notredame.png"))
     extractor = SuperPoint_baseline()
 
     keypoints, descriptors = extractor.detectAndCompute(img)
 
     output_image = cv2.drawKeypoints(img, keypoints, 0, (0, 0, 255))
-
-    cv2.imwrite("sp_test.png", output_image)
+    cv2.imshow('superpoint', output_image)
+    cv2.waitKey(0)
```

### Comparing `easy_local_features-0.2.3/easy_local_features/datasets/download.py` & `easy_local_features-0.3.0/easy_local_features/datasets/download.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.2.3/easy_local_features.egg-info/PKG-INFO` & `easy_local_features-0.3.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,51 @@
-Metadata-Version: 2.1
-Name: easy-local-features
-Version: 0.2.3
-Author: eucadar
-Author-email: python@eucadar.com
-Description-Content-Type: text/markdown
-
 # easy-local-features-baselines
 
 Just some scripts to make things easier for the local features baselines.
 
 # Installation
 
+
+I suggest using a conda environment to install the requirements. You can create one using the following command.
+
+```bash
+conda create -n elf python=3.9 # the python version is not so critical, but I used 3.9.
+conda activate elf
+```
+
+Now we can insall the requirements using pip.
+
 ```bash
 pip install -r requirements.txt
 pip install .
 ```
 
 # How to use
 
 ```python
-from easy_local_features import DEAL
-# from easy_local_features import DALF, DISK, R2D2, SuperPoint, SuperGlue
+from easy_local_features.baseline_deal import DEAL_baseline
+# from easy_local_features.baseline_dalf import DALF_baseline
+# from easy_local_features.baseline_disk import DISK_baseline
+# from easy_local_features.baseline_r2d2 import R2D2_baseline
+# from easy_local_features.baseline_superglue import SuperGlue_baseline
+# from easy_local_features.baseline_superpoint import SuperPoint_baseline
 
 # Load an image
 img = cv2.imread("assets/notredame.png")
 
 # Initialize the extractor
-extractor = DEAL()
+extractor = DEAL_baseline()
 
 # Return keypoints and descriptors just like OpenCV
 keypoints, descriptors = extractor.detectAndCompute(img)
 
 ```
 # TODO
 
 - [x] Add a setup.py to make it a pip package
 - [ ] Add a script to download some datasets
 - [ ] Add a download script for the pretrained models
 - [ ] Add more baselines :)
   - [ ] ASLFeat
-  - [ ] DELF
+  - [x] DELF
   - [ ] LoFTR
-  - [ ] DKM
+  - [ ] DKM
```

### Comparing `easy_local_features-0.2.3/setup.py` & `easy_local_features-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         long_description = f.read()
 else:
     with open('README.md', encoding='utf-8') as f:
         long_description = f.read()
 
 setup(
     name='easy_local_features',
-    version='0.2.3',
+    version='0.3.0',
     author='eucadar',
     author_email='python@eucadar.com',
     packages=find_packages(exclude=('tests', 'docs', 'assets')),
     include_package_data=True,
     install_requires=[],
     long_description_content_type='text/markdown',
     long_description=long_description,
```

