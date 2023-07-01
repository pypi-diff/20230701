# Comparing `tmp/torchlights-0.3.8.1.tar.gz` & `tmp/torchlights-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchlights-0.3.8.1.tar", last modified: Sun Sep 18 15:04:48 2022, max compression
+gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/torchlight/dist/.tmp-vqclfdz0/torchlights-0.4.0.tar", last modified: Sat Jul  1 16:29:48 2023, max compression
```

## Comparing `torchlights-0.3.8.1.tar` & `torchlights-0.4.0.tar`

### file list

```diff
@@ -1,113 +1,175 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.095689 torchlights-0.3.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-09-18 15:04:48.095689 torchlights-0.3.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2565 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-18 15:04:48.095689 torchlights-0.3.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.083689 torchlights-0.3.8.1/torchlight/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.083689 torchlights-0.3.8.1/torchlight/contrib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.083689 torchlights-0.3.8.1/torchlight/contrib/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/contrib/datasets/ICVL.py
--rw-r--r--   0 runner    (1001) docker     (121)      639 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/contrib/datasets/SIDD.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/contrib/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.083689 torchlights-0.3.8.1/torchlight/contrib/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     2664 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/contrib/scripts/SIDD_test.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/contrib/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2470 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/contrib/scripts/mnist.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.083689 torchlights-0.3.8.1/torchlight/contrib/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/contrib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/contrib/utils/hsi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.087689 torchlights-0.3.8.1/torchlight/data/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2262 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/data/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3421 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.087689 torchlights-0.3.8.1/torchlight/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/data/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3774 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/data/datasets/pair.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/data/datasets/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/data/image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.087689 torchlights-0.3.8.1/torchlight/logging/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6171 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/logging/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     1177 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/logging/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.087689 torchlights-0.3.8.1/torchlight/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2155 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/metrics/_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/metrics/simple.py
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/metrics/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.087689 torchlights-0.3.8.1/torchlight/nn/
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1678 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.087689 torchlights-0.3.8.1/torchlight/nn/blocks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/blocks/residual.py
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/blocks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (121)     3629 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/conversion.py
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/init.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.087689 torchlights-0.3.8.1/torchlight/nn/loss/
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/loss/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.087689 torchlights-0.3.8.1/torchlight/nn/loss/functional/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/loss/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/loss/functional/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2985 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/loss/landmark.py
--rw-r--r--   0 runner    (1001) docker     (121)     3576 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/loss/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/loss/vggloss.py
--rw-r--r--   0 runner    (1001) docker     (121)     6639 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/lr_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.091689 torchlights-0.3.8.1/torchlight/nn/ops/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4165 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/ops/flow.py
--rw-r--r--   0 runner    (1001) docker     (121)     2885 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/ops/gradient.py
--rw-r--r--   0 runner    (1001) docker     (121)     1678 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/ops/interpolate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.091689 torchlights-0.3.8.1/torchlight/nn/ops/sync_batchnorm/
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/ops/sync_batchnorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12973 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/ops/sync_batchnorm/batchnorm.py
--rw-r--r--   0 runner    (1001) docker     (121)     4278 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/ops/sync_batchnorm/comm.py
--rw-r--r--   0 runner    (1001) docker     (121)     3226 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/ops/sync_batchnorm/replicate.py
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/ops/sync_batchnorm/unittest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2366 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/reproducibility.py
--rw-r--r--   0 runner    (1001) docker     (121)     3144 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/nn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.091689 torchlights-0.3.8.1/torchlight/trainer/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7654 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/trainer/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    12426 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/trainer/engine.py
--rw-r--r--   0 runner    (1001) docker     (121)     2749 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/trainer/entry.py
--rw-r--r--   0 runner    (1001) docker     (121)     2624 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/trainer/module.py
--rw-r--r--   0 runner    (1001) docker     (121)     5419 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/trainer/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.091689 torchlights-0.3.8.1/torchlight/transforms/
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/transforms/_util.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/transforms/conversion.py
--rw-r--r--   0 runner    (1001) docker     (121)     3092 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/transforms/degrade.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.091689 torchlights-0.3.8.1/torchlight/transforms/functional/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/transforms/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3315 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/transforms/functional/general.py
--rw-r--r--   0 runner    (1001) docker     (121)    13909 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/transforms/functional/matlab.py
--rw-r--r--   0 runner    (1001) docker     (121)     2427 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/transforms/general.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.091689 torchlights-0.3.8.1/torchlight/transforms/kernels/
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/transforms/kernels/misr_spe_p.mat
--rw-r--r--   0 runner    (1001) docker     (121)     5009 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/transforms/noise.py
--rw-r--r--   0 runner    (1001) docker     (121)     3303 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/transforms/stateful.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.091689 torchlights-0.3.8.1/torchlight/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/utils/example.py
--rw-r--r--   0 runner    (1001) docker     (121)     7376 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/utils/flow.py
--rw-r--r--   0 runner    (1001) docker     (121)     5341 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3856 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/utils/os.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.091689 torchlights-0.3.8.1/torchlight/utils/registration/
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/utils/registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3739 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/utils/registration/affine_ransac.py
--rw-r--r--   0 runner    (1001) docker     (121)     4498 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/utils/registration/affine_transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     6298 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/utils/registration/align_transform.py
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/utils/stat.py
--rw-r--r--   0 runner    (1001) docker     (121)     4635 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-09-18 15:04:38.000000 torchlights-0.3.8.1/torchlight/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 15:04:48.095689 torchlights-0.3.8.1/torchlights.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-09-18 15:04:48.000000 torchlights-0.3.8.1/torchlights.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2843 2022-09-18 15:04:48.000000 torchlights-0.3.8.1/torchlights.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-18 15:04:48.000000 torchlights-0.3.8.1/torchlights.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-09-18 15:04:48.000000 torchlights-0.3.8.1/torchlights.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-18 15:04:48.000000 torchlights-0.3.8.1/torchlights.egg-info/top_level.txt
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2199 2022-06-25 14:48:59.000000 torchlights-0.4.0/.gitignore
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      715 2021-12-29 01:20:49.000000 torchlights-0.4.0/.readthedocs.yaml
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       35 2021-12-08 07:31:18.000000 torchlights-0.4.0/MANIFEST.in
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      290 2023-07-01 16:29:48.000000 torchlights-0.4.0/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2565 2022-07-07 02:23:26.000000 torchlights-0.4.0/README.md
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:47.000000 torchlights-0.4.0/docs/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      638 2021-12-28 16:11:29.000000 torchlights-0.4.0/docs/Makefile
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      804 2021-12-28 16:11:29.000000 torchlights-0.4.0/docs/make.bat
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       70 2021-12-29 03:18:30.000000 torchlights-0.4.0/docs/requirements.txt
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/docs/source/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2620 2021-12-29 03:29:44.000000 torchlights-0.4.0/docs/source/conf.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       74 2022-01-14 16:07:58.000000 torchlights-0.4.0/docs/source/getstart.md
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1012 2022-01-14 16:13:22.000000 torchlights-0.4.0/docs/source/index.md
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/docs/source/modules/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       35 2022-01-14 16:14:17.000000 torchlights-0.4.0/docs/source/modules/logging.md
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       35 2022-01-14 16:14:46.000000 torchlights-0.4.0/docs/source/modules/transforms.md
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:47.000000 torchlights-0.4.0/examples/
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/examples/demo/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      959 2021-11-29 13:18:49.000000 torchlights-0.4.0/examples/demo/demo_fft.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      103 2021-11-29 13:20:23.000000 torchlights-0.4.0/examples/demo/demo_logging.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      259 2021-11-29 13:19:56.000000 torchlights-0.4.0/examples/demo/demo_match.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      585 2021-11-29 13:20:23.000000 torchlights-0.4.0/examples/demo/demo_metrics.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    97133 2021-09-14 04:02:18.000000 torchlights-0.4.0/examples/demo/lena.png
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      156 2021-07-20 03:27:15.000000 torchlights-0.4.0/examples/demo/test.json
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      103 2021-07-20 03:41:49.000000 torchlights-0.4.0/examples/demo/test.yaml
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4758 2021-12-13 08:41:08.000000 torchlights-0.4.0/examples/demo/test_dataset.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      361 2021-12-07 12:58:35.000000 torchlights-0.4.0/examples/demo/test_module.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1004 2021-09-14 16:40:16.000000 torchlights-0.4.0/examples/demo/test_qqdm.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/examples/demo/test_registration/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)   445478 2021-10-14 12:52:29.000000 torchlights-0.4.0/examples/demo/test_registration/img1.png
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)   469922 2021-10-14 12:52:29.000000 torchlights-0.4.0/examples/demo/test_registration/img2.png
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)   351120 2021-10-14 12:52:29.000000 torchlights-0.4.0/examples/demo/test_registration/mona_source.png
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)   149059 2021-10-14 12:52:29.000000 torchlights-0.4.0/examples/demo/test_registration/mona_target.jpg
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2140 2021-10-14 12:52:29.000000 torchlights-0.4.0/examples/demo/test_registration/test_registration.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      513 2021-09-14 12:37:28.000000 torchlights-0.4.0/examples/demo/test_tqdm.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/examples/mnist/
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/examples/mnist/config/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      225 2021-12-21 08:47:44.000000 torchlights-0.4.0/examples/mnist/config/config.yaml
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       24 2021-09-26 12:10:12.000000 torchlights-0.4.0/examples/mnist/config/override.yaml
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2474 2022-05-05 14:25:41.000000 torchlights-0.4.0/examples/mnist/minimal.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1045 2021-11-30 02:53:51.000000 torchlights-0.4.0/examples/mnist/module.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1864 2021-09-18 03:31:59.000000 torchlights-0.4.0/examples/mnist/net.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1045 2021-10-20 14:14:25.000000 torchlights-0.4.0/examples/mnist/run.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1774 2021-10-20 14:33:58.000000 torchlights-0.4.0/examples/mnist/run2.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1043 2021-12-07 12:05:08.000000 torchlights-0.4.0/examples/mnist/run3.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-07-01 16:29:48.000000 torchlights-0.4.0/setup.cfg
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      522 2023-07-01 16:29:43.000000 torchlights-0.4.0/setup.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/tests/
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/tests/sample/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    97133 2021-11-26 08:55:25.000000 torchlights-0.4.0/tests/sample/lena.png
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      830 2022-06-23 09:43:26.000000 torchlights-0.4.0/tests/test_dataset.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      294 2022-06-11 10:38:52.000000 torchlights-0.4.0/tests/test_io.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3688 2022-01-11 09:30:56.000000 torchlights-0.4.0/tests/test_metric.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      144 2022-06-27 02:54:59.000000 torchlights-0.4.0/torchlight/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/contrib/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2022-06-24 03:13:15.000000 torchlights-0.4.0/torchlight/contrib/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/contrib/basicsr_data/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5051 2022-06-11 06:47:04.000000 torchlights-0.4.0/torchlight/contrib/basicsr_data/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2033 2022-06-11 06:47:03.000000 torchlights-0.4.0/torchlight/contrib/basicsr_data/data_sampler.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    12358 2022-06-11 06:47:03.000000 torchlights-0.4.0/torchlight/contrib/basicsr_data/data_util.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2749 2022-06-11 06:47:03.000000 torchlights-0.4.0/torchlight/contrib/basicsr_data/ffhq_dataset.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11314 2022-06-11 06:47:03.000000 torchlights-0.4.0/torchlight/contrib/basicsr_data/paired_image_SR_LR_FullImage_Memory_dataset.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11677 2022-06-11 06:47:03.000000 torchlights-0.4.0/torchlight/contrib/basicsr_data/paired_image_SR_LR_dataset.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5561 2022-06-11 06:47:03.000000 torchlights-0.4.0/torchlight/contrib/basicsr_data/paired_image_dataset.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3536 2022-06-11 06:47:03.000000 torchlights-0.4.0/torchlight/contrib/basicsr_data/prefetch_dataloader.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    10190 2022-06-11 06:47:03.000000 torchlights-0.4.0/torchlight/contrib/basicsr_data/reds_dataset.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2934 2022-06-11 06:47:04.000000 torchlights-0.4.0/torchlight/contrib/basicsr_data/single_image_dataset.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     8509 2022-06-11 06:47:04.000000 torchlights-0.4.0/torchlight/contrib/basicsr_data/transforms.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13063 2022-06-11 06:47:04.000000 torchlights-0.4.0/torchlight/contrib/basicsr_data/video_test_dataset.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4991 2022-06-11 06:47:03.000000 torchlights-0.4.0/torchlight/contrib/basicsr_data/vimeo90k_dataset.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/contrib/datasets/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2022-06-03 12:05:29.000000 torchlights-0.4.0/torchlight/contrib/datasets/ICVL.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      639 2022-06-24 03:14:48.000000 torchlights-0.4.0/torchlight/contrib/datasets/SIDD.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2022-06-24 03:13:33.000000 torchlights-0.4.0/torchlight/contrib/datasets/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/contrib/scripts/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2664 2022-06-27 10:11:57.000000 torchlights-0.4.0/torchlight/contrib/scripts/SIDD_test.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2022-06-11 10:12:24.000000 torchlights-0.4.0/torchlight/contrib/scripts/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2470 2022-05-27 06:31:01.000000 torchlights-0.4.0/torchlight/contrib/scripts/mnist.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/contrib/utils/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2022-06-24 04:31:25.000000 torchlights-0.4.0/torchlight/contrib/utils/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      250 2022-06-24 04:32:01.000000 torchlights-0.4.0/torchlight/contrib/utils/hsi.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/data/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      123 2022-05-30 11:39:48.000000 torchlights-0.4.0/torchlight/data/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2262 2021-12-20 12:51:17.000000 torchlights-0.4.0/torchlight/data/dataloader.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3421 2022-05-30 10:51:43.000000 torchlights-0.4.0/torchlight/data/dataset.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/data/datasets/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2022-06-24 03:14:15.000000 torchlights-0.4.0/torchlight/data/datasets/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3774 2022-06-23 09:43:26.000000 torchlights-0.4.0/torchlight/data/datasets/pair.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      404 2022-06-03 03:27:27.000000 torchlights-0.4.0/torchlight/data/datasets/wrapper.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      736 2022-01-11 13:16:01.000000 torchlights-0.4.0/torchlight/data/image_folder.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/logging/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       26 2021-11-26 07:14:52.000000 torchlights-0.4.0/torchlight/logging/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6171 2022-06-27 02:57:56.000000 torchlights-0.4.0/torchlight/logging/logger.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1177 2022-04-18 12:20:46.000000 torchlights-0.4.0/torchlight/logging/visualization.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/metrics/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       80 2021-11-26 08:14:26.000000 torchlights-0.4.0/torchlight/metrics/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2208 2022-10-16 07:17:05.000000 torchlights-0.4.0/torchlight/metrics/_util.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1311 2022-01-07 13:05:43.000000 torchlights-0.4.0/torchlight/metrics/simple.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      559 2021-11-26 07:36:09.000000 torchlights-0.4.0/torchlight/metrics/torch.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/nn/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      203 2022-06-11 10:11:45.000000 torchlights-0.4.0/torchlight/nn/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1608 2023-04-13 12:14:03.000000 torchlights-0.4.0/torchlight/nn/benchmark.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/nn/blocks/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2022-06-11 10:11:26.000000 torchlights-0.4.0/torchlight/nn/blocks/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1095 2022-06-11 06:38:05.000000 torchlights-0.4.0/torchlight/nn/blocks/residual.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      830 2022-06-11 06:39:52.000000 torchlights-0.4.0/torchlight/nn/blocks/upsample.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3629 2022-06-11 10:32:25.000000 torchlights-0.4.0/torchlight/nn/conversion.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1349 2022-06-11 06:36:22.000000 torchlights-0.4.0/torchlight/nn/init.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/nn/loss/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      159 2021-09-20 09:51:54.000000 torchlights-0.4.0/torchlight/nn/loss/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/nn/loss/functional/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       34 2021-09-24 11:49:16.000000 torchlights-0.4.0/torchlight/nn/loss/functional/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      367 2021-09-26 12:10:14.000000 torchlights-0.4.0/torchlight/nn/loss/functional/misc.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2985 2021-10-03 03:57:55.000000 torchlights-0.4.0/torchlight/nn/loss/landmark.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3576 2021-09-26 12:10:14.000000 torchlights-0.4.0/torchlight/nn/loss/misc.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1837 2022-06-11 04:19:57.000000 torchlights-0.4.0/torchlight/nn/loss/vggloss.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6639 2022-06-11 04:29:06.000000 torchlights-0.4.0/torchlight/nn/lr_scheduler.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/nn/ops/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2021-09-20 03:09:51.000000 torchlights-0.4.0/torchlight/nn/ops/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4165 2022-06-11 06:40:12.000000 torchlights-0.4.0/torchlight/nn/ops/flow.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2885 2021-10-14 12:52:29.000000 torchlights-0.4.0/torchlight/nn/ops/gradient.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1678 2021-10-16 13:02:06.000000 torchlights-0.4.0/torchlight/nn/ops/image.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      455 2021-10-20 07:15:54.000000 torchlights-0.4.0/torchlight/nn/ops/interpolate.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/nn/ops/sync_batchnorm/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      449 2021-09-10 08:34:59.000000 torchlights-0.4.0/torchlight/nn/ops/sync_batchnorm/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    12973 2021-09-10 08:35:00.000000 torchlights-0.4.0/torchlight/nn/ops/sync_batchnorm/batchnorm.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4278 2021-09-10 08:35:00.000000 torchlights-0.4.0/torchlight/nn/ops/sync_batchnorm/comm.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3226 2021-09-10 08:35:00.000000 torchlights-0.4.0/torchlight/nn/ops/sync_batchnorm/replicate.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      835 2021-09-10 08:35:00.000000 torchlights-0.4.0/torchlight/nn/ops/sync_batchnorm/unittest.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2366 2022-07-07 02:23:26.000000 torchlights-0.4.0/torchlight/nn/reproducibility.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3144 2022-06-27 02:57:56.000000 torchlights-0.4.0/torchlight/nn/utils.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/trainer/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      135 2022-06-27 02:57:56.000000 torchlights-0.4.0/torchlight/trainer/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7654 2022-06-27 02:57:56.000000 torchlights-0.4.0/torchlight/trainer/config.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    12426 2022-07-07 02:23:26.000000 torchlights-0.4.0/torchlight/trainer/engine.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2749 2022-06-27 02:57:56.000000 torchlights-0.4.0/torchlight/trainer/entry.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2624 2022-07-07 02:23:26.000000 torchlights-0.4.0/torchlight/trainer/module.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6670 2022-06-25 14:48:01.000000 torchlights-0.4.0/torchlight/trainer/util.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/transforms/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      350 2022-06-11 10:07:00.000000 torchlights-0.4.0/torchlight/transforms/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      329 2021-10-14 12:52:29.000000 torchlights-0.4.0/torchlight/transforms/_util.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      399 2022-06-11 10:16:27.000000 torchlights-0.4.0/torchlight/transforms/conversion.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3092 2022-04-18 13:12:47.000000 torchlights-0.4.0/torchlight/transforms/degrade.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/transforms/functional/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       22 2022-01-11 09:11:02.000000 torchlights-0.4.0/torchlight/transforms/functional/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3315 2022-06-11 06:34:08.000000 torchlights-0.4.0/torchlight/transforms/functional/general.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13909 2022-06-11 06:31:43.000000 torchlights-0.4.0/torchlight/transforms/functional/matlab.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2427 2022-04-04 05:23:21.000000 torchlights-0.4.0/torchlight/transforms/general.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/transforms/kernels/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      454 2021-10-14 12:52:29.000000 torchlights-0.4.0/torchlight/transforms/kernels/misr_spe_p.mat
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5009 2022-01-20 05:25:12.000000 torchlights-0.4.0/torchlight/transforms/noise.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3303 2022-01-13 08:19:36.000000 torchlights-0.4.0/torchlight/transforms/stateful.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/utils/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      126 2022-06-23 09:43:26.000000 torchlights-0.4.0/torchlight/utils/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       71 2022-06-11 10:37:04.000000 torchlights-0.4.0/torchlight/utils/example.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7376 2021-10-15 09:16:59.000000 torchlights-0.4.0/torchlight/utils/flow.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5341 2022-09-18 06:41:08.000000 torchlights-0.4.0/torchlight/utils/helper.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3856 2022-09-18 06:27:21.000000 torchlights-0.4.0/torchlight/utils/io.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1673 2022-06-11 06:44:36.000000 torchlights-0.4.0/torchlight/utils/os.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlight/utils/registration/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      167 2021-10-14 12:52:29.000000 torchlights-0.4.0/torchlight/utils/registration/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3739 2021-11-07 15:28:44.000000 torchlights-0.4.0/torchlight/utils/registration/affine_ransac.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4498 2021-10-14 12:52:29.000000 torchlights-0.4.0/torchlight/utils/registration/affine_transform.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6298 2021-10-14 12:52:29.000000 torchlights-0.4.0/torchlight/utils/registration/align_transform.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      638 2021-12-06 14:12:28.000000 torchlights-0.4.0/torchlight/utils/stat.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4635 2022-06-28 06:03:06.000000 torchlights-0.4.0/torchlight/utils/timer.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       21 2022-06-27 09:57:07.000000 torchlights-0.4.0/torchlight/version.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-07-01 16:29:48.000000 torchlights-0.4.0/torchlights.egg-info/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      290 2023-07-01 16:29:47.000000 torchlights-0.4.0/torchlights.egg-info/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4567 2023-07-01 16:29:47.000000 torchlights-0.4.0/torchlights.egg-info/SOURCES.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-07-01 16:29:47.000000 torchlights-0.4.0/torchlights.egg-info/dependency_links.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       50 2023-07-01 16:29:47.000000 torchlights-0.4.0/torchlights.egg-info/requires.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       11 2023-07-01 16:29:47.000000 torchlights-0.4.0/torchlights.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `torchlights-0.3.8.1/README.md` & `torchlights-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/setup.py` & `torchlights-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='torchlights',
     packages=find_packages(),
-    version='0.3.8.1',
+    version='0.4.0',
     description='Torchlights - an light-weight PyTorch trainer, as well as many useful utils',
     author='Zeqiang Lai',
     author_email='laizeqiang@outlook.com',
     long_description_content_type = 'text/markdown',
     url='https://github.com/Zeqiang-Lai/torchlight',
     install_requires=['munch', 'colorama', 'readchar', 'tqdm', 'qqdm', 'pyyaml', 'colorlog'],
     include_package_data=True
```

### Comparing `torchlights-0.3.8.1/torchlight/contrib/datasets/SIDD.py` & `torchlights-0.4.0/torchlight/contrib/datasets/SIDD.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/contrib/scripts/SIDD_test.py` & `torchlights-0.4.0/torchlight/contrib/scripts/SIDD_test.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/contrib/scripts/mnist.py` & `torchlights-0.4.0/torchlight/contrib/scripts/mnist.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/data/dataloader.py` & `torchlights-0.4.0/torchlight/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/data/dataset.py` & `torchlights-0.4.0/torchlight/data/dataset.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/data/datasets/pair.py` & `torchlights-0.4.0/torchlight/data/datasets/pair.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/data/image_folder.py` & `torchlights-0.4.0/torchlight/data/image_folder.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/logging/logger.py` & `torchlights-0.4.0/torchlight/logging/logger.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/logging/visualization.py` & `torchlights-0.4.0/torchlight/logging/visualization.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/metrics/_util.py` & `torchlights-0.4.0/torchlight/metrics/_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     def warpped(output, target, *args, **kwargs):
         if DATA_FORMAT == FORMAT_CHW:
             C = output.shape[-3]
             total = 0
             for ch in range(C):
                 x = output[ch, :, :]
                 y = target[ch, :, :]
+                # print(func(x, y, *args, **kwargs))
                 total += func(x, y, *args, **kwargs)
             return total / C
         else:
             C = output.shape[-1]
             total = 0
             for ch in range(C):
                 x = output[:, :, ch]
```

### Comparing `torchlights-0.3.8.1/torchlight/metrics/simple.py` & `torchlights-0.4.0/torchlight/metrics/simple.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/metrics/torch.py` & `torchlights-0.4.0/torchlight/metrics/torch.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/nn/benchmark.py` & `torchlights-0.4.0/torchlight/nn/benchmark.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import time
 import torch
 
+
 def measure_inference_speed(model, data, max_iter=200, log_interval=50):
     model.eval()
 
     # the first several iterations may be very slow so skip them
     num_warmup = 5
     pure_inf_time = 0
     fps = 0
@@ -36,19 +37,18 @@
             print(
                 f'Overall fps: {fps:.1f} img / s, '
                 f'times per image: {1000 / fps:.1f} ms / img',
                 flush=True)
             break
     return fps
 
-def model_size(model):
-    total = sum([param.nelement() for param in model.parameters()])
-    return total/1e6
 
+def model_size(model, trainable=False):
+    if trainable:
+        total = sum(p.numel() for p in model.parameters() if p.requires_grad)
+    else:
+        total = sum([param.nelement() for param in model.parameters()])
+    return total / 1e6
 
-    # def __str__(self):
-    #     """
-    #     Model prints with number of trainable parameters
-    #     """
-    #     model_parameters = filter(lambda p: p.requires_grad, self.parameters())
-    #     params = sum([np.prod(p.size()) for p in model_parameters])
-    #     return super().__str__() + '\nTrainable parameters: {}'.format(params)
+def trainable_model_size(model):
+    total = sum([param.nelement() for param in model.parameters() if param.requires_grad])
+    return total/1e6
```

### Comparing `torchlights-0.3.8.1/torchlight/nn/blocks/residual.py` & `torchlights-0.4.0/torchlight/nn/blocks/residual.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/nn/blocks/upsample.py` & `torchlights-0.4.0/torchlight/nn/blocks/upsample.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/nn/conversion.py` & `torchlights-0.4.0/torchlight/nn/conversion.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/nn/init.py` & `torchlights-0.4.0/torchlight/nn/init.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/nn/loss/landmark.py` & `torchlights-0.4.0/torchlight/nn/loss/landmark.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/nn/loss/misc.py` & `torchlights-0.4.0/torchlight/nn/loss/misc.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/nn/loss/vggloss.py` & `torchlights-0.4.0/torchlight/nn/loss/vggloss.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/nn/lr_scheduler.py` & `torchlights-0.4.0/torchlight/nn/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/nn/ops/flow.py` & `torchlights-0.4.0/torchlight/nn/ops/flow.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/nn/ops/gradient.py` & `torchlights-0.4.0/torchlight/nn/ops/gradient.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/nn/ops/image.py` & `torchlights-0.4.0/torchlight/nn/ops/image.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/nn/ops/sync_batchnorm/batchnorm.py` & `torchlights-0.4.0/torchlight/nn/ops/sync_batchnorm/batchnorm.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/nn/ops/sync_batchnorm/comm.py` & `torchlights-0.4.0/torchlight/nn/ops/sync_batchnorm/comm.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/nn/ops/sync_batchnorm/replicate.py` & `torchlights-0.4.0/torchlight/nn/ops/sync_batchnorm/replicate.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/nn/ops/sync_batchnorm/unittest.py` & `torchlights-0.4.0/torchlight/nn/ops/sync_batchnorm/unittest.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/nn/reproducibility.py` & `torchlights-0.4.0/torchlight/nn/reproducibility.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/nn/utils.py` & `torchlights-0.4.0/torchlight/nn/utils.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/trainer/config.py` & `torchlights-0.4.0/torchlight/trainer/config.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/trainer/engine.py` & `torchlights-0.4.0/torchlight/trainer/engine.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/trainer/entry.py` & `torchlights-0.4.0/torchlight/trainer/entry.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/trainer/module.py` & `torchlights-0.4.0/torchlight/trainer/module.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/trainer/util.py` & `torchlights-0.4.0/torchlight/trainer/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     res = ''
     options = ['y', 'n', 'Y', 'N']
     print(msg + " Press y/n")
     while res not in options:
         res = readchar.readchar()
     return res == 'y' or res == 'Y'
 
+
 def auto_rename(path):
     count = 1
     new_path = path
     while True:
         if not os.path.exists(new_path):
             return new_path
         file_name = os.path.basename(path)
@@ -38,36 +39,79 @@
         ncols = shutil.get_terminal_size()[0]
     left = ncols // 2
     right = ncols - left
     divider = sym*(left-len(text)) + text + sym*right
     return divider
 
 
+class CheckpointManager:
+    def __init__(self, path, max_keep=5):
+        pass
+
+    def save(self, state, key):
+        pass
+
+
+class Checkpoint:
+    def __init__(self, path, max_keep=5):
+        self.path = path
+        self.max_keep = max_keep
+        self.files = []
+        if os.path.exists(self.path):
+            self.files = [f for f in os.listdir(self.path) if f.endswith('.pth')]
+            self.files.sort()
+            if len(self.files) > self.max_keep:
+                self.files = self.files[:-self.max_keep]
+                for f in self.files:
+                    os.remove(os.path.join(self.path, f))
+
+    def save(self, name, state_dict):
+        import torch
+        torch.save(state_dict, os.path.join(self.path, name+'.pth'))
+        self.files.append(name+'.pth')
+        self.files.sort()
+        if len(self.files) > self.max_keep:
+            self.files = self.files[:-self.max_keep]
+            for f in self.files:
+                os.remove(os.path.join(self.path, f))
+
+    def load(self, name):
+        import torch
+        return torch.load(os.path.join(self.path, name+'.pth'))
+
+    def list(self):
+        return self.files
+
+    def clear(self):
+        for f in self.files:
+            os.remove(os.path.join(self.path, f))
+        self.files = []
+
+
 class CheckpointCleaner:
     def __init__(self, root, keep='all'):
         """ This class provide the ability to control the storage size of checkpoints. 
 
             Args:
                 root: root dir path of checkpoints
                 keep: the mode to control storage. Defaults to 'all'. The valid choice includes
                       `all`: keep all checkpoints, `latest_#`: keep latest n checkpoints
         """
         self.root = root
         self.mode = keep
         self._check_mode()
-    
+
     def _check_mode(self):
         if self.mode.startswith('latest'):
             n = int(self.mode.split('_')[-1])
         elif self.mode == 'all':
-            return 
+            return
         else:
             raise ValueError(f'Invalid mode {self.mode}')
-            
-            
+
     def clean(self):
         file_names = os.listdir(self.root)
         file_names = filter(lambda x: x.endswith('.pth'), file_names)
         file_names = filter(lambda x: x.startswith('model-epoch'), file_names)
         file_names = [os.path.join(self.root, n) for n in file_names]
         file_names = sorted(file_names, key=lambda x: os.path.getctime(x), reverse=True)
 
@@ -133,15 +177,15 @@
 
         assert self.early_stop_threshold > 0, 'early_stop_threshold should be greater than 0'
         assert self.mnt_mode in ['min', 'max']
 
         self.reset()
 
     def update(self, metric, info=None):
-        improvement = self.mnt_best - metric if self.mnt_mode == 'min' else metric - self.mnt_best 
+        improvement = self.mnt_best - metric if self.mnt_mode == 'min' else metric - self.mnt_best
         improved = improvement >= self.early_stop_threshold
         self.best = False
         if improved:
             self.mnt_best = metric
             self.not_improved_count = 0
             self.best = True
             self.improvement = improvement
@@ -159,19 +203,19 @@
         self.not_improved_count = 0
         self.mnt_best = inf if self.mnt_mode == 'min' else -inf
         self.best = False
         self.improvement = 0
         self.mnt_best_info = None
 
     def state_dict(self):
-        return {'not_improved_count': self.not_improved_count, 
-                'mnt_best': self.mnt_best, 
-                'best': self.best, 
+        return {'not_improved_count': self.not_improved_count,
+                'mnt_best': self.mnt_best,
+                'best': self.best,
                 'last_improvement': self.improvement,
                 'mnt_best_info': self.mnt_best_info}
 
     def load_state_dict(self, states):
         self.not_improved_count = states['not_improved_count']
         self.mnt_best = states['mnt_best']
         self.best = states['best']
         self.mnt_best_info = states.get('mnt_best_info')
-        self.improvement  = states.get('last_improvement')
+        self.improvement = states.get('last_improvement')
```

### Comparing `torchlights-0.3.8.1/torchlight/transforms/degrade.py` & `torchlights-0.4.0/torchlight/transforms/degrade.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/transforms/functional/general.py` & `torchlights-0.4.0/torchlight/transforms/functional/general.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/transforms/functional/matlab.py` & `torchlights-0.4.0/torchlight/transforms/functional/matlab.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/transforms/general.py` & `torchlights-0.4.0/torchlight/transforms/general.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/transforms/noise.py` & `torchlights-0.4.0/torchlight/transforms/noise.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/transforms/stateful.py` & `torchlights-0.4.0/torchlight/transforms/stateful.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/utils/flow.py` & `torchlights-0.4.0/torchlight/utils/flow.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/utils/helper.py` & `torchlights-0.4.0/torchlight/utils/helper.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/utils/io.py` & `torchlights-0.4.0/torchlight/utils/io.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/utils/os.py` & `torchlights-0.4.0/torchlight/utils/os.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/utils/registration/affine_ransac.py` & `torchlights-0.4.0/torchlight/utils/registration/affine_ransac.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/utils/registration/affine_transform.py` & `torchlights-0.4.0/torchlight/utils/registration/affine_transform.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/utils/registration/align_transform.py` & `torchlights-0.4.0/torchlight/utils/registration/align_transform.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/utils/stat.py` & `torchlights-0.4.0/torchlight/utils/stat.py`

 * *Files identical despite different names*

### Comparing `torchlights-0.3.8.1/torchlight/utils/timer.py` & `torchlights-0.4.0/torchlight/utils/timer.py`

 * *Files identical despite different names*

