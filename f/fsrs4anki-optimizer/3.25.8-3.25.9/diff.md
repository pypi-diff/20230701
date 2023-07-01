# Comparing `tmp/fsrs4anki_optimizer-3.25.8.tar.gz` & `tmp/fsrs4anki_optimizer-3.25.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-3.25.8.tar", last modified: Thu Jun 29 14:09:15 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-3.25.9.tar", last modified: Sat Jul  1 12:03:05 2023, max compression
```

## Comparing `fsrs4anki_optimizer-3.25.8.tar` & `fsrs4anki_optimizer-3.25.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:09:15.958477 fsrs4anki_optimizer-3.25.8/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-29 14:09:15.954477 fsrs4anki_optimizer-3.25.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:09:15.954477 fsrs4anki_optimizer-3.25.8/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-29 14:09:05.000000 fsrs4anki_optimizer-3.25.8/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-29 14:09:05.000000 fsrs4anki_optimizer-3.25.8/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45359 2023-06-29 14:09:05.000000 fsrs4anki_optimizer-3.25.8/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:09:15.954477 fsrs4anki_optimizer-3.25.8/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-29 14:09:15.000000 fsrs4anki_optimizer-3.25.8/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-29 14:09:15.000000 fsrs4anki_optimizer-3.25.8/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:09:15.000000 fsrs4anki_optimizer-3.25.8/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-29 14:09:15.000000 fsrs4anki_optimizer-3.25.8/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 14:09:15.000000 fsrs4anki_optimizer-3.25.8/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-29 14:09:05.000000 fsrs4anki_optimizer-3.25.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 14:09:15.958477 fsrs4anki_optimizer-3.25.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-29 14:09:05.000000 fsrs4anki_optimizer-3.25.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 12:03:05.967891 fsrs4anki_optimizer-3.25.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-01 12:03:05.967891 fsrs4anki_optimizer-3.25.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 12:03:05.963891 fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-01 12:02:56.000000 fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-01 12:02:56.000000 fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45447 2023-07-01 12:02:56.000000 fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 12:03:05.967891 fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-01 12:03:05.000000 fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-01 12:03:05.000000 fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 12:03:05.000000 fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-01 12:03:05.000000 fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-01 12:03:05.000000 fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-01 12:02:56.000000 fsrs4anki_optimizer-3.25.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 12:03:05.967891 fsrs4anki_optimizer-3.25.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-01 12:02:56.000000 fsrs4anki_optimizer-3.25.9/setup.py
```

### Comparing `fsrs4anki_optimizer-3.25.8/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-3.25.8/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-3.25.9/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     for li, response in enumerate(response):
         tensor[li][0] = int(ivl[li])
         tensor[li][1] = int(response)
     return tensor
 
 class RevlogDataset(Dataset):
     def __init__(self, dataframe: pd.DataFrame):
-        if len(dataframe) == 0:
+        if dataframe.empty:
             raise ValueError('Training data is inadequate.')
         padded = pad_sequence(dataframe['tensor'].to_list(), batch_first=True, padding_value=0)
         self.x_train = padded.int()
         self.t_train = torch.tensor(dataframe['delta_t'].values, dtype=torch.int)
         self.y_train = torch.tensor(dataframe['y'].values, dtype=torch.float)
         self.seq_len = torch.tensor(dataframe['tensor'].map(len).values, dtype=torch.long)
 
@@ -479,14 +479,16 @@
         https://github.com/open-spaced-repetition/fsrs4anki/wiki/Free-Spaced-Repetition-Scheduler
         '''
 
     def train(self, lr: float = 4e-2, n_epoch: int = 3, n_splits: int = 3, batch_size: int = 512, verbose: bool = True):
         """Step 4"""
         self.dataset = pd.read_csv("./revlog_history.tsv", sep='\t', index_col=None, dtype={'r_history': str ,'t_history': str} )
         self.dataset = self.dataset[(self.dataset['i'] > 1) & (self.dataset['delta_t'] > 0) & (self.dataset['t_history'].str.count(',0') == 0)]
+        if self.dataset.empty:
+            raise ValueError('Training data is inadequate.')
         self.dataset['tensor'] = self.dataset.progress_apply(lambda x: lineToTensor(list(zip([x['t_history']], [x['r_history']]))[0]), axis=1)
         self.dataset['group'] = self.dataset['r_history'] + self.dataset['t_history']
         print("Tensorized!")
         
         n_pre_train_groups = len(self.dataset[self.dataset['i'] == 2]['group'].unique())
         if n_pre_train_groups < n_splits:
             print("Not enough groups for pre-training. Splitting into {} folds.".format(n_pre_train_groups))
```

