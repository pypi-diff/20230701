# Comparing `tmp/mltrainer-0.1.5.tar.gz` & `tmp/mltrainer-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltrainer-0.1.5.tar", last modified: Sat Jul  1 19:39:33 2023, max compression
+gzip compressed data, was "mltrainer-0.1.6.tar", last modified: Sat Jul  1 20:14:36 2023, max compression
```

## Comparing `mltrainer-0.1.5.tar` & `mltrainer-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       50 2023-06-30 09:29:35.989842 mltrainer-0.1.5/README.md
--rw-r--r--   0        0        0      177 2023-07-01 19:38:48.061403 mltrainer-0.1.5/mltrainer/__init__.py
--rw-r--r--   0        0        0     1653 2023-06-29 21:12:27.729107 mltrainer-0.1.5/mltrainer/imagemodels.py
--rw-r--r--   0        0        0     1653 2023-06-29 21:14:56.380151 mltrainer-0.1.5/mltrainer/metrics.py
--rw-r--r--   0        0        0     4285 2023-06-29 21:14:36.526642 mltrainer-0.1.5/mltrainer/rnn_models.py
--rw-r--r--   0        0        0     1543 2023-06-29 21:25:52.147263 mltrainer-0.1.5/mltrainer/settings.py
--rw-r--r--   0        0        0     2388 2023-06-29 21:22:50.605098 mltrainer-0.1.5/mltrainer/tokenizer.py
--rw-r--r--   0        0        0     8797 2023-06-30 09:47:07.147102 mltrainer-0.1.5/mltrainer/trainer.py
--rw-r--r--   0        0        0     2489 2023-06-30 09:47:13.271722 mltrainer-0.1.5/mltrainer/vae.py
--rw-r--r--   0        0        0     1643 2023-07-01 19:39:33.290727 mltrainer-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      916 1970-01-01 00:00:00.000000 mltrainer-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      525 2023-07-01 20:13:15.394002 mltrainer-0.1.6/README.md
+-rw-r--r--   0        0        0      177 2023-07-01 20:13:45.704001 mltrainer-0.1.6/mltrainer/__init__.py
+-rw-r--r--   0        0        0     1653 2023-06-29 21:12:27.729107 mltrainer-0.1.6/mltrainer/imagemodels.py
+-rw-r--r--   0        0        0     1653 2023-06-29 21:14:56.380151 mltrainer-0.1.6/mltrainer/metrics.py
+-rw-r--r--   0        0        0     4285 2023-06-29 21:14:36.526642 mltrainer-0.1.6/mltrainer/rnn_models.py
+-rw-r--r--   0        0        0     1517 2023-07-01 19:57:49.930597 mltrainer-0.1.6/mltrainer/settings.py
+-rw-r--r--   0        0        0     2388 2023-06-29 21:22:50.605098 mltrainer-0.1.6/mltrainer/tokenizer.py
+-rw-r--r--   0        0        0     8803 2023-07-01 19:59:48.644092 mltrainer-0.1.6/mltrainer/trainer.py
+-rw-r--r--   0        0        0     2489 2023-06-30 09:47:13.271722 mltrainer-0.1.6/mltrainer/vae.py
+-rw-r--r--   0        0        0     1151 2023-07-01 20:14:36.003703 mltrainer-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1548 1970-01-01 00:00:00.000000 mltrainer-0.1.6/PKG-INFO
```

### Comparing `mltrainer-0.1.5/mltrainer/imagemodels.py` & `mltrainer-0.1.6/mltrainer/imagemodels.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.5/mltrainer/metrics.py` & `mltrainer-0.1.6/mltrainer/metrics.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.5/mltrainer/rnn_models.py` & `mltrainer-0.1.6/mltrainer/rnn_models.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.5/mltrainer/settings.py` & `mltrainer-0.1.6/mltrainer/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 from enum import Enum
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional
 
-from loguru import logger
 from pydantic import BaseModel, root_validator
 
 
 class FileTypes(Enum):
     JPG = ".jpg"
     PNG = ".png"
     TXT = ".txt"
```

### Comparing `mltrainer-0.1.5/mltrainer/tokenizer.py` & `mltrainer-0.1.6/mltrainer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.5/mltrainer/trainer.py` & `mltrainer-0.1.6/mltrainer/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from datetime import datetime
 from pathlib import Path
 from typing import Callable, Dict, Iterator, Optional, Tuple
 
 import gin
 import mlflow
 # needed to make summarywriter load without error
-import torch
 from loguru import logger
 from ray import tune
+import torch
 from torch.utils.tensorboard import SummaryWriter
 from tqdm import tqdm
 
 from mltrainer import ReportTypes, TrainerSettings
 
 
 def write_gin(dir: Path, txt: str) -> None:
@@ -182,18 +182,18 @@
         save: bool = False,
     ) -> None:
         """
         Args:
             log_dir (Path): location to save checkpoint to.
             patience (int): How long to wait after last time validation loss improved.
                             Default: 7
-            verbose (bool): If True, prints a message for each validation loss improvement.
-                            Default: False
-            delta (float): Minimum change in the monitored quantity to qualify as an improvement.
-                            Default: 0.0
+            verbose (bool): If True, prints a message for each validation loss
+            improvement. Default: False
+            delta (float): Minimum change in the monitored quantity to qualify as
+            an improvement. Default: 0.0
         """
         self.patience = patience
         self.verbose = verbose
         self.counter = 0
         self.best_loss = None
         self.early_stop = False
         self.delta = delta
@@ -207,29 +207,31 @@
             if self.save:
                 self.save_checkpoint(val_loss, model)
         elif val_loss >= self.best_loss + self.delta:  # type: ignore
             # we minimize loss. If current loss did not improve
             # the previous best (with a delta) it is considered not to improve.
             self.counter += 1
             logger.info(
-                f"best loss: {self.best_loss:.4f}, current loss {val_loss:.4f}. Counter {self.counter}/{self.patience}."
+                f"best loss: {self.best_loss:.4f}, current loss {val_loss:.4f}."
+                f"Counter {self.counter}/{self.patience}."
             )
             if self.counter >= self.patience:
                 self.early_stop = True
         else:
             # if not the first run, and val_loss is smaller, we improved.
             self.best_loss = val_loss
             if self.save:
                 self.save_checkpoint(val_loss, model)
             self.counter = 0
 
     def save_checkpoint(self, val_loss: float, model: torch.nn.Module) -> None:
         """Saves model when validation loss decrease."""
         if self.verbose:
             logger.info(
-                f"Validation loss ({self.best_loss:.4f} --> {val_loss:.4f}). Saving {self.path} ..."
+                f"Validation loss ({self.best_loss:.4f} --> {val_loss:.4f})."
+                f"Saving {self.path} ..."
             )
         torch.save(model, self.path)
         self.val_loss_min = val_loss
 
     def get_best(self) -> torch.nn.Module:
         return torch.load(self.path)
```

### Comparing `mltrainer-0.1.5/mltrainer/vae.py` & `mltrainer-0.1.6/mltrainer/vae.py`

 * *Files identical despite different names*

