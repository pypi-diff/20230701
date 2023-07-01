# Comparing `tmp/joonmyung-1.4.6.tar.gz` & `tmp/joonmyung-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/joonmyung-1.4.6.tar", last modified: Sun Jun 11 04:46:05 2023, max compression
+gzip compressed data, was "dist/joonmyung-1.4.8.tar", last modified: Sat Jul  1 07:02:54 2023, max compression
```

## Comparing `joonmyung-1.4.6.tar` & `joonmyung-1.4.8.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxrwxr-x   0 joonmyung  (1002) joonmyung  (1003)        0 2023-06-11 04:46:05.518205 joonmyung-1.4.6/
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)        0 2023-02-22 17:22:56.000000 joonmyung-1.4.6/LICENSE.txt
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)      256 2023-06-11 04:46:05.518205 joonmyung-1.4.6/PKG-INFO
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     1138 2023-04-06 18:15:10.000000 joonmyung-1.4.6/README.md
-drwxrwxr-x   0 joonmyung  (1002) joonmyung  (1003)        0 2023-06-11 04:46:05.518205 joonmyung-1.4.6/joonmyung/
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)       15 2023-02-22 17:22:56.000000 joonmyung-1.4.6/joonmyung/__init__.py
-drwxrwxr-x   0 joonmyung  (1002) joonmyung  (1003)        0 2023-06-11 04:46:05.518205 joonmyung-1.4.6/joonmyung/analysis/
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)      110 2023-03-01 06:50:39.000000 joonmyung-1.4.6/joonmyung/analysis/__init__.py
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     6956 2023-05-11 09:50:49.000000 joonmyung-1.4.6/joonmyung/analysis/analysis.py
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     4984 2023-05-21 08:17:20.000000 joonmyung-1.4.6/joonmyung/analysis/benchmark.py
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     4675 2023-05-21 08:24:43.000000 joonmyung-1.4.6/joonmyung/analysis/dataset.py
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)        0 2023-03-01 06:34:05.000000 joonmyung-1.4.6/joonmyung/analysis/hook.py
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     1217 2023-06-06 06:13:54.000000 joonmyung-1.4.6/joonmyung/analysis/metric.py
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     1999 2023-06-06 06:28:53.000000 joonmyung-1.4.6/joonmyung/analysis/model.py
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)      424 2023-06-06 06:36:54.000000 joonmyung-1.4.6/joonmyung/analysis/utils.py
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     6700 2023-04-03 12:26:27.000000 joonmyung-1.4.6/joonmyung/app.py
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)      695 2023-02-24 17:07:52.000000 joonmyung-1.4.6/joonmyung/data.py
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)    13698 2023-05-21 08:03:13.000000 joonmyung-1.4.6/joonmyung/draw.py
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)       29 2023-04-03 12:26:27.000000 joonmyung-1.4.6/joonmyung/dummy.py
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     2755 2023-02-22 17:22:56.000000 joonmyung-1.4.6/joonmyung/file.py
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)      920 2023-02-22 17:22:56.000000 joonmyung-1.4.6/joonmyung/gradcam.py
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)    10232 2023-05-21 08:10:17.000000 joonmyung-1.4.6/joonmyung/log.py
-drwxrwxr-x   0 joonmyung  (1002) joonmyung  (1003)        0 2023-06-11 04:46:05.518205 joonmyung-1.4.6/joonmyung/meta_data/
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)       41 2023-03-01 06:51:46.000000 joonmyung-1.4.6/joonmyung/meta_data/__init__.py
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)    45491 2023-02-22 17:22:56.000000 joonmyung-1.4.6/joonmyung/meta_data/label.py
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     2157 2023-06-11 04:39:41.000000 joonmyung-1.4.6/joonmyung/meta_data/utils.py
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     4031 2023-05-26 13:55:28.000000 joonmyung-1.4.6/joonmyung/metric.py
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     3214 2023-05-11 09:51:38.000000 joonmyung-1.4.6/joonmyung/script.py
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     1487 2023-03-01 13:25:20.000000 joonmyung-1.4.6/joonmyung/status.py
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     3948 2023-06-06 06:13:54.000000 joonmyung-1.4.6/joonmyung/utils.py
-drwxrwxr-x   0 joonmyung  (1002) joonmyung  (1003)        0 2023-06-11 04:46:05.518205 joonmyung-1.4.6/joonmyung.egg-info/
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)      256 2023-06-11 04:46:05.000000 joonmyung-1.4.6/joonmyung.egg-info/PKG-INFO
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)      749 2023-06-11 04:46:05.000000 joonmyung-1.4.6/joonmyung.egg-info/SOURCES.txt
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)        1 2023-06-11 04:46:05.000000 joonmyung-1.4.6/joonmyung.egg-info/dependency_links.txt
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)        1 2023-05-26 13:56:46.000000 joonmyung-1.4.6/joonmyung.egg-info/not-zip-safe
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)       10 2023-06-11 04:46:05.000000 joonmyung-1.4.6/joonmyung.egg-info/top_level.txt
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)       38 2023-06-11 04:46:05.518205 joonmyung-1.4.6/setup.cfg
--rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)      782 2023-06-11 04:43:38.000000 joonmyung-1.4.6/setup.py
+drwxrwxr-x   0 joonmyung  (1006) joonmyung  (1007)        0 2023-07-01 07:02:54.843149 joonmyung-1.4.8/
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)        0 2023-02-22 17:22:56.000000 joonmyung-1.4.8/LICENSE.txt
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)      256 2023-07-01 07:02:54.843149 joonmyung-1.4.8/PKG-INFO
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)     1138 2023-04-06 18:15:10.000000 joonmyung-1.4.8/README.md
+drwxrwxr-x   0 joonmyung  (1006) joonmyung  (1007)        0 2023-07-01 07:02:54.843149 joonmyung-1.4.8/joonmyung/
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)       15 2023-02-22 17:22:56.000000 joonmyung-1.4.8/joonmyung/__init__.py
+drwxrwxr-x   0 joonmyung  (1006) joonmyung  (1007)        0 2023-07-01 07:02:54.843149 joonmyung-1.4.8/joonmyung/analysis/
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)      110 2023-03-01 06:50:39.000000 joonmyung-1.4.8/joonmyung/analysis/__init__.py
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)     6956 2023-05-11 09:50:49.000000 joonmyung-1.4.8/joonmyung/analysis/analysis.py
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)     4675 2023-05-21 08:24:43.000000 joonmyung-1.4.8/joonmyung/analysis/dataset.py
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)        0 2023-03-01 06:34:05.000000 joonmyung-1.4.8/joonmyung/analysis/hook.py
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)     1217 2023-06-06 06:13:54.000000 joonmyung-1.4.8/joonmyung/analysis/metric.py
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)     1999 2023-06-06 06:28:53.000000 joonmyung-1.4.8/joonmyung/analysis/model.py
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)      424 2023-06-06 06:36:54.000000 joonmyung-1.4.8/joonmyung/analysis/utils.py
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)     6700 2023-04-03 12:26:27.000000 joonmyung-1.4.8/joonmyung/app.py
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)      695 2023-02-24 17:07:52.000000 joonmyung-1.4.8/joonmyung/data.py
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)    13698 2023-05-21 08:03:13.000000 joonmyung-1.4.8/joonmyung/draw.py
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)       29 2023-04-03 12:26:27.000000 joonmyung-1.4.8/joonmyung/dummy.py
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)     2755 2023-02-22 17:22:56.000000 joonmyung-1.4.8/joonmyung/file.py
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)      920 2023-02-22 17:22:56.000000 joonmyung-1.4.8/joonmyung/gradcam.py
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)    10232 2023-05-21 08:10:17.000000 joonmyung-1.4.8/joonmyung/log.py
+drwxrwxr-x   0 joonmyung  (1006) joonmyung  (1007)        0 2023-07-01 07:02:54.843149 joonmyung-1.4.8/joonmyung/meta_data/
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)       41 2023-03-01 06:51:46.000000 joonmyung-1.4.8/joonmyung/meta_data/__init__.py
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)    45491 2023-02-22 17:22:56.000000 joonmyung-1.4.8/joonmyung/meta_data/label.py
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)     2187 2023-07-01 06:19:43.000000 joonmyung-1.4.8/joonmyung/meta_data/utils.py
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)     4031 2023-05-26 13:55:28.000000 joonmyung-1.4.8/joonmyung/metric.py
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)     3214 2023-05-11 09:51:38.000000 joonmyung-1.4.8/joonmyung/script.py
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)     1487 2023-03-01 13:25:20.000000 joonmyung-1.4.8/joonmyung/status.py
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)     3948 2023-06-06 06:13:54.000000 joonmyung-1.4.8/joonmyung/utils.py
+drwxrwxr-x   0 joonmyung  (1006) joonmyung  (1007)        0 2023-07-01 07:02:54.843149 joonmyung-1.4.8/joonmyung.egg-info/
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)      256 2023-07-01 07:02:54.000000 joonmyung-1.4.8/joonmyung.egg-info/PKG-INFO
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)      717 2023-07-01 07:02:54.000000 joonmyung-1.4.8/joonmyung.egg-info/SOURCES.txt
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)        1 2023-07-01 07:02:54.000000 joonmyung-1.4.8/joonmyung.egg-info/dependency_links.txt
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)        1 2023-07-01 07:02:33.000000 joonmyung-1.4.8/joonmyung.egg-info/not-zip-safe
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)       10 2023-07-01 07:02:54.000000 joonmyung-1.4.8/joonmyung.egg-info/top_level.txt
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)       38 2023-07-01 07:02:54.843149 joonmyung-1.4.8/setup.cfg
+-rw-rw-r--   0 joonmyung  (1006) joonmyung  (1007)      782 2023-07-01 07:02:12.000000 joonmyung-1.4.8/setup.py
```

### Comparing `joonmyung-1.4.6/README.md` & `joonmyung-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.6/joonmyung/analysis/analysis.py` & `joonmyung-1.4.8/joonmyung/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.6/joonmyung/analysis/benchmark.py` & `joonmyung-1.4.8/joonmyung/metric.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,60 @@
-# Copyright (c) Meta Platforms, Inc. and affiliates.
-# All rights reserved.
-
-# This source code is licensed under the license found in the
-# LICENSE file in the root directory of this source tree.
-# --------------------------------------------------------
-
-
 from fvcore.nn import FlopCountAnalysis, flop_count_table, flop_count_str
-from joonmyung.log import MetricLogger
-from joonmyung.metric import accuracy
+from torchprofile import profile_macs
 from typing import Tuple
 from thop import profile
 from tqdm import tqdm
 import torch
 import time
 
-def thop(model, size, *kwargs, device="cuda"):
+def thop(model, size, *kwargs,
+         round_num=1, eval = True, device="cuda"):
+    if eval: model.eval().to(device)
     input = torch.randn(size, device=device)
     macs, params = profile(model, inputs=(input, *kwargs))
-    return macs / 1000000000, params / 1000000
+    macs, params = macs / 1000000000, params / 1000000
+
+    print(f"thop macs/params : {macs}/{params}")
 
-def numel(model):
-    return sum([p.numel() for p in model.parameters() if p.requires_grad]) / 1000000
+    return round(macs, round_num), round(params, round_num)
 
-def flops(model, size, *kwargs, p=1, device="cuda"):
+def numel(model,
+          round_num=1):
+    params = sum([p.numel() for p in model.parameters() if p.requires_grad]) / 1000000
+    print(f"numel params : {params}")
+    return round(params, round_num)
+
+def flops(model, size, *kwargs,
+          round_num=1, eval = True, device="cuda"):
+    if eval: model.eval()
     inputs = torch.randn(size, device=device, requires_grad=True)
     flops  = FlopCountAnalysis(model, (inputs, *kwargs))
-    if p == 1:
-        print(flop_count_table(flops))
-    elif p == 2:
-        print(flop_count_str(flops))
-    return flops.total() / 1000000000
+    flops_num = flops.total() / 1000000000
+
+    print(flop_count_table(flops))
+    # print(flop_count_str(flops))
+    print(f"fvcore flops : {flops_num}")
+
+    return round(flops_num, round_num)
+
+
+def get_macs(model, size,
+             eval = True, round_num=1, device="cuda"):
+    if eval: model.eval()
+    inputs = torch.randn(size, device=device, requires_grad=True)
+    macs = profile_macs(model, inputs)
+    print(f"torchprofile MACS : {macs}")
+
+    return round(macs, round_num)
 
 def benchmark(
     model: torch.nn.Module,
     device: torch.device = 0,
     input_size: Tuple[int] = (3, 224, 224),
-    batch_size: int = 64,
+    batch_size: int = 1024,
     runs: int = 40,
     throw_out: float = 0.25,
     use_fp16: bool = False,
     verbose: bool = False,
     **kwargs
 ) -> float:
     """
@@ -56,17 +70,14 @@
      - use_fp16: whether or not to benchmark with float16 and autocast
      - verbose: whether or not to use tqdm to print progress / print throughput at end
 
     Returns:
      - the throughput measured in images / second
     """
 
-
-
-
     if not isinstance(device, torch.device):
         device = torch.device(device)
     is_cuda = torch.device(device).type == "cuda"
 
     model = model.eval().to(device)
     input = torch.rand(batch_size, *input_size, device=device)
     if use_fp16:
@@ -92,72 +103,28 @@
     if is_cuda:
         torch.cuda.synchronize()
 
     end = time.time()
     elapsed = end - start
 
     throughput = total / elapsed
-    macs, p = thop(model, (1, 3, 224, 224), device=device)
-
-    n_parameters = numel(model)
-    fv_flops = flops(model, (1, 3, 224, 224), p=0, device=device)
 
     if verbose:
         print(f"Throughput: {throughput:.2f} im/s")
-        print(f"numel  :    {n_parameters:.2f} M")
-        print(f"fvcore :    {fv_flops:.2f} G")
-        print(f"thop   :    {macs:.2f}G, {p:.2f}M")
-
-
-    return throughput
-
-@torch.no_grad()
-def evaluate_benchmark(data_loader, model, device):
-
-    metric_logger = MetricLogger(delimiter="  ")
-    header = 'BENCHMARK:'
 
-    # switch to evaluation mode
-    model.eval()
-    import time
-    start = time.time()
-    cnt_token, cnt_token_diff, total = None, None, 0
-    for images, target in metric_logger.log_every(data_loader, 10, header):
-        images = images.to(device, non_blocking=True)
-        target = target.to(device, non_blocking=True)
-
-        # compute output
-        with torch.cuda.amp.autocast():
-            output = model(images)
-
-        acc1, acc5 = accuracy(output, target, topk=(1, 5))
-
-        batch_size = images.shape[0]
-        metric_logger.meters['acc1'].update(acc1.item(), n=batch_size)
-        metric_logger.meters['acc5'].update(acc5.item(), n=batch_size)
-        total += batch_size
-
-    # gather the stats from all processes
-    metric_logger.synchronize_between_processes()
-    end = time.time()
-    elapsed = end - start
-
-    throughput = total / elapsed
-    print(f"Throughput: {throughput:.2f} im/s")
-    print('* Acc@1 {top1.global_avg:.3f} Acc@5 {top5.global_avg:.3f} loss {losses.global_avg:.3f}'
-          .format(top1=metric_logger.acc1, top5=metric_logger.acc5, losses=metric_logger.loss))
-
-    return {k: meter.global_avg for k, meter in metric_logger.meters.items()}
+    return round(throughput)
 
 
 
-# from benchmark import benchmark, evaluate_benchmark
-# evaluate_benchmark(data_loader_val, model, device)
-# benchmark(
-#     model,
-#     device="cuda",
-#     verbose=True,
-#     runs=50,
-#     batch_size=256,
-#     input_size=(3, 224, 224)
-# )
-# return
+def accuracy(output, target, topk=(1,)):
+    """Computes the accuracy over the k top predictions for the specified values of k"""
+    maxk = max(topk)
+    _, pred = output.topk(maxk, 1, True, True)
+    batch_size = target.size(0)
+    pred = pred.t()
+    correct = pred.eq(target.reshape(1, -1).expand_as(pred))
+    return [correct[:k].reshape(-1).float().sum(0) * 100. / batch_size for k in topk]
+
+def targetPred(output, target, topk=5):
+    _, pred = output.topk(topk, 1, True, True)
+    TP = torch.cat([target.unsqueeze(-1), pred], dim=1)
+    return TP
```

### Comparing `joonmyung-1.4.6/joonmyung/analysis/dataset.py` & `joonmyung-1.4.8/joonmyung/analysis/dataset.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.6/joonmyung/analysis/metric.py` & `joonmyung-1.4.8/joonmyung/analysis/metric.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.6/joonmyung/analysis/model.py` & `joonmyung-1.4.8/joonmyung/analysis/model.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.6/joonmyung/app.py` & `joonmyung-1.4.8/joonmyung/app.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.6/joonmyung/data.py` & `joonmyung-1.4.8/joonmyung/data.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.6/joonmyung/draw.py` & `joonmyung-1.4.8/joonmyung/draw.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.6/joonmyung/file.py` & `joonmyung-1.4.8/joonmyung/file.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.6/joonmyung/gradcam.py` & `joonmyung-1.4.8/joonmyung/gradcam.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.6/joonmyung/log.py` & `joonmyung-1.4.8/joonmyung/log.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.6/joonmyung/meta_data/label.py` & `joonmyung-1.4.8/joonmyung/meta_data/label.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.6/joonmyung/meta_data/utils.py` & `joonmyung-1.4.8/joonmyung/meta_data/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,32 +2,30 @@
 import torch.nn.functional as F
 import pandas as pd
 import numpy as np
 import torch
 import socket
 import os
 
-
-
 def data2path(dataset, server = "",
               conference="", wandb_version="", wandb_name="",
-              kisti_id=""):
+              kisti_id="", hub_num = 1):
 
     hostname = socket.gethostname()
     server = server if server is not "" \
                 else hostname if "mlv" in hostname \
                     else "kakao" if "dakao" in hostname \
                         else "kisti"
 
     if "kakao" in server:
         data_path = "/data/opensets"
         output_dir = "/data/project/rw/joonmyung/conference"
     elif "mlv" in server:
-        data_path = "/hub_data1/joonmyung/data"
-        output_dir = "/hub_data1/joonmyung/conference"
+        data_path  = f"/hub_data{hub_num}/joonmyung/data"
+        output_dir = f"/hub_data{hub_num}/joonmyung/conference"
     elif server in ["kisti"]:
         data_path = f"/scratch/{kisti_id}/data"
         output_dir = f"/scratch/{kisti_id}/result"
     else:
         raise ValueError
 
     if dataset in ["imagenet", "IMNET"]:
```

### Comparing `joonmyung-1.4.6/joonmyung/script.py` & `joonmyung-1.4.8/joonmyung/script.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.6/joonmyung/status.py` & `joonmyung-1.4.8/joonmyung/status.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.6/joonmyung/utils.py` & `joonmyung-1.4.8/joonmyung/utils.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.6/joonmyung.egg-info/SOURCES.txt` & `joonmyung-1.4.8/joonmyung.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 joonmyung.egg-info/PKG-INFO
 joonmyung.egg-info/SOURCES.txt
 joonmyung.egg-info/dependency_links.txt
 joonmyung.egg-info/not-zip-safe
 joonmyung.egg-info/top_level.txt
 joonmyung/analysis/__init__.py
 joonmyung/analysis/analysis.py
-joonmyung/analysis/benchmark.py
 joonmyung/analysis/dataset.py
 joonmyung/analysis/hook.py
 joonmyung/analysis/metric.py
 joonmyung/analysis/model.py
 joonmyung/analysis/utils.py
 joonmyung/meta_data/__init__.py
 joonmyung/meta_data/label.py
```

### Comparing `joonmyung-1.4.6/setup.py` & `joonmyung-1.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from setuptools import find_packages
 
 setuptools.setup(
     name="joonmyung",
-    version="1.4.6",
+    version="1.4.8",
     author="JoonMyung Choi",
     author_email="pizard@korea.ac.kr",
     description="JoonMyung's Library",
     url="https://github.com/pizard/JoonMyung.git",
     license="MIT",
     packages=find_packages(exclude=["playground",
                                     "playground.*",
```

