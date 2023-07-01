# Comparing `tmp/ScandEval-7.1.0.tar.gz` & `tmp/scandeval-7.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScandEval-7.1.0.tar", max compression
+gzip compressed data, was "scandeval-7.1.1.tar", max compression
```

## Comparing `ScandEval-7.1.0.tar` & `scandeval-7.1.1.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1077 2023-01-26 21:11:58.574218 ScandEval-7.1.0/LICENSE
--rw-r--r--   0        0        0     6755 2023-05-13 14:13:06.300002 ScandEval-7.1.0/README.md
--rw-r--r--   0        0        0     1845 2023-05-15 13:06:56.154168 ScandEval-7.1.0/pyproject.toml
--rw-r--r--   0        0        0      839 2023-05-13 13:56:49.238045 ScandEval-7.1.0/src/scandeval/__init__.py
--rw-r--r--   0        0        0     8919 2023-04-12 09:02:17.736254 ScandEval-7.1.0/src/scandeval/benchmark_config_factory.py
--rw-r--r--   0        0        0    28601 2023-05-13 13:50:06.250309 ScandEval-7.1.0/src/scandeval/benchmark_dataset.py
--rw-r--r--   0        0        0    17639 2023-04-12 09:02:17.736765 ScandEval-7.1.0/src/scandeval/benchmarker.py
--rw-r--r--   0        0        0     1382 2022-11-03 09:23:55.848473 ScandEval-7.1.0/src/scandeval/callbacks.py
--rw-r--r--   0        0        0     6661 2023-04-12 09:02:17.736945 ScandEval-7.1.0/src/scandeval/cli.py
--rw-r--r--   0        0        0     6035 2023-04-12 09:02:17.737107 ScandEval-7.1.0/src/scandeval/config.py
--rw-r--r--   0        0        0     4962 2022-12-29 15:49:44.942921 ScandEval-7.1.0/src/scandeval/dataset_configs.py
--rw-r--r--   0        0        0     1920 2022-11-03 09:23:55.849427 ScandEval-7.1.0/src/scandeval/dataset_factory.py
--rw-r--r--   0        0        0     3352 2022-12-29 15:49:44.943265 ScandEval-7.1.0/src/scandeval/dataset_tasks.py
--rw-r--r--   0        0        0      650 2022-07-22 11:05:37.491231 ScandEval-7.1.0/src/scandeval/exceptions.py
--rw-r--r--   0        0        0    12351 2023-02-22 12:37:31.608038 ScandEval-7.1.0/src/scandeval/hf_hub.py
--rw-r--r--   0        0        0     7946 2022-07-14 15:19:22.963227 ScandEval-7.1.0/src/scandeval/languages.py
--rw-r--r--   0        0        0    17159 2023-05-15 13:06:18.166268 ScandEval-7.1.0/src/scandeval/model_loading.py
--rw-r--r--   0        0        0    15045 2023-03-10 17:33:33.955970 ScandEval-7.1.0/src/scandeval/named_entity_recognition.py
--rw-r--r--   0        0        0    29225 2023-05-15 13:06:18.166623 ScandEval-7.1.0/src/scandeval/norbert.py
--rw-r--r--   0        0        0    14150 2023-04-12 09:02:17.737732 ScandEval-7.1.0/src/scandeval/question_answering.py
--rw-r--r--   0        0        0    11733 2022-12-24 12:57:14.794624 ScandEval-7.1.0/src/scandeval/question_answering_trainer.py
--rw-r--r--   0        0        0     4692 2022-12-29 15:49:44.943541 ScandEval-7.1.0/src/scandeval/scores.py
--rw-r--r--   0        0        0     3899 2022-12-24 12:57:14.794885 ScandEval-7.1.0/src/scandeval/sequence_classification.py
--rw-r--r--   0        0        0     5812 2023-04-12 09:02:17.737892 ScandEval-7.1.0/src/scandeval/speed_benchmark.py
--rw-r--r--   0        0        0      163 2022-11-03 09:23:55.851896 ScandEval-7.1.0/src/scandeval/types.py
--rw-r--r--   0        0        0     9001 2023-05-13 13:57:24.239401 ScandEval-7.1.0/src/scandeval/utils.py
--rw-r--r--   0        0        0     8623 1970-01-01 00:00:00.000000 ScandEval-7.1.0/setup.py
--rw-r--r--   0        0        0     8243 1970-01-01 00:00:00.000000 ScandEval-7.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-01-26 21:11:58.574218 scandeval-7.1.1/LICENSE
+-rw-r--r--   0        0        0     6750 2023-07-01 19:13:27.814691 scandeval-7.1.1/README.md
+-rw-r--r--   0        0        0     1845 2023-07-01 19:16:24.863905 scandeval-7.1.1/pyproject.toml
+-rw-r--r--   0        0        0      839 2023-07-01 18:45:52.001335 scandeval-7.1.1/src/scandeval/__init__.py
+-rw-r--r--   0        0        0     8919 2023-07-01 18:45:52.001569 scandeval-7.1.1/src/scandeval/benchmark_config_factory.py
+-rw-r--r--   0        0        0    28605 2023-07-01 19:13:27.815074 scandeval-7.1.1/src/scandeval/benchmark_dataset.py
+-rw-r--r--   0        0        0    17639 2023-07-01 18:45:52.002190 scandeval-7.1.1/src/scandeval/benchmarker.py
+-rw-r--r--   0        0        0     1382 2022-11-03 09:23:55.848473 scandeval-7.1.1/src/scandeval/callbacks.py
+-rw-r--r--   0        0        0     6661 2023-07-01 18:45:52.002354 scandeval-7.1.1/src/scandeval/cli.py
+-rw-r--r--   0        0        0     6035 2023-07-01 18:45:52.002513 scandeval-7.1.1/src/scandeval/config.py
+-rw-r--r--   0        0        0     4962 2023-07-01 18:45:52.002664 scandeval-7.1.1/src/scandeval/dataset_configs.py
+-rw-r--r--   0        0        0     1920 2023-07-01 18:45:52.002926 scandeval-7.1.1/src/scandeval/dataset_factory.py
+-rw-r--r--   0        0        0     3352 2023-07-01 18:45:52.003106 scandeval-7.1.1/src/scandeval/dataset_tasks.py
+-rw-r--r--   0        0        0      650 2022-07-22 11:05:37.491231 scandeval-7.1.1/src/scandeval/exceptions.py
+-rw-r--r--   0        0        0    12351 2023-07-01 18:45:52.003254 scandeval-7.1.1/src/scandeval/hf_hub.py
+-rw-r--r--   0        0        0     7946 2023-07-01 18:45:52.003641 scandeval-7.1.1/src/scandeval/languages.py
+-rw-r--r--   0        0        0    17159 2023-07-01 18:45:52.004243 scandeval-7.1.1/src/scandeval/model_loading.py
+-rw-r--r--   0        0        0    15041 2023-07-01 19:13:27.815284 scandeval-7.1.1/src/scandeval/named_entity_recognition.py
+-rw-r--r--   0        0        0    29225 2023-07-01 18:45:52.004663 scandeval-7.1.1/src/scandeval/norbert.py
+-rw-r--r--   0        0        0    14150 2023-07-01 18:45:52.004871 scandeval-7.1.1/src/scandeval/question_answering.py
+-rw-r--r--   0        0        0    11733 2023-07-01 18:45:52.005045 scandeval-7.1.1/src/scandeval/question_answering_trainer.py
+-rw-r--r--   0        0        0     4692 2023-07-01 18:45:52.005167 scandeval-7.1.1/src/scandeval/scores.py
+-rw-r--r--   0        0        0     3899 2023-07-01 19:04:19.892632 scandeval-7.1.1/src/scandeval/sequence_classification.py
+-rw-r--r--   0        0        0     5812 2023-07-01 18:45:52.006157 scandeval-7.1.1/src/scandeval/speed_benchmark.py
+-rw-r--r--   0        0        0      163 2023-07-01 18:45:52.006248 scandeval-7.1.1/src/scandeval/types.py
+-rw-r--r--   0        0        0     9001 2023-07-01 18:45:52.006432 scandeval-7.1.1/src/scandeval/utils.py
+-rw-r--r--   0        0        0     8238 1970-01-01 00:00:00.000000 scandeval-7.1.1/PKG-INFO
```

### Comparing `ScandEval-7.1.0/LICENSE` & `scandeval-7.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ScandEval-7.1.0/README.md` & `scandeval-7.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ### Evaluation of pretrained language models on mono- or multilingual Scandinavian language tasks.
 
 ______________________________________________________________________
 [![PyPI Status](https://badge.fury.io/py/scandeval.svg)](https://pypi.org/project/scandeval/)
 [![Paper](https://img.shields.io/badge/arXiv-2304.00906-b31b1b.svg)](https://arxiv.org/abs/2304.00906)
 [![License](https://img.shields.io/github/license/saattrupdan/ScandEval)](https://github.com/saattrupdan/ScandEval/blob/main/LICENSE)
 [![LastCommit](https://img.shields.io/github/last-commit/saattrupdan/ScandEval)](https://github.com/saattrupdan/ScandEval/commits/main)
-[![Code Coverage](https://img.shields.io/badge/Coverage-76%25-yellowgreen.svg)](https://github.com/saattrupdan/ScandEval/tree/main/tests)
+[![Code Coverage](https://img.shields.io/badge/Coverage-64%25-yellow.svg)](https://github.com/saattrupdan/ScandEval/tree/main/tests)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)](https://github.com/saattrupdan/ScandEval/blob/main/CODE_OF_CONDUCT.md)
 
 
 ## Installation
 To install the package simply write the following command in your favorite terminal:
 ```
 $ pip install scandeval
```

### Comparing `ScandEval-7.1.0/pyproject.toml` & `scandeval-7.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ScandEval"
-version = "7.1.0"
+version = "7.1.1"
 description = "Evaluation of pretrained language models on mono- or multilingual Scandinavian language tasks."
 authors = ["Dan Saattrup Nielsen <saattrupdan@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://scandeval.github.io"
 repository = "https://github.com/saattrupdan/ScandEval"
```

### Comparing `ScandEval-7.1.0/src/scandeval/__init__.py` & `scandeval-7.1.1/src/scandeval/__init__.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.1.0/src/scandeval/benchmark_config_factory.py` & `scandeval-7.1.1/src/scandeval/benchmark_config_factory.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.1.0/src/scandeval/benchmark_dataset.py` & `scandeval-7.1.1/src/scandeval/benchmark_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,18 +460,18 @@
         test = dataset_dict["test"]
 
         # Remove empty examples from the datasets
         if "tokens" in train.features:
             train = train.filter(lambda x: len(x["tokens"]) > 0)
             val = val.filter(lambda x: len(x["tokens"]) > 0)
             test = test.filter(lambda x: len(x["tokens"]) > 0)
-        elif "doc" in train.features:
-            train = train.filter(lambda x: len(x["doc"]) > 0)
-            val = val.filter(lambda x: len(x["doc"]) > 0)
-            test = test.filter(lambda x: len(x["doc"]) > 0)
+        elif "text" in train.features:
+            train = train.filter(lambda x: len(x["text"]) > 0)
+            val = val.filter(lambda x: len(x["text"]) > 0)
+            test = test.filter(lambda x: len(x["text"]) > 0)
 
         # If we are testing then truncate the test set
         if self.benchmark_config.testing:
             test = test.select(range(128))
 
         return train, val, test
```

### Comparing `ScandEval-7.1.0/src/scandeval/benchmarker.py` & `scandeval-7.1.1/src/scandeval/benchmarker.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.1.0/src/scandeval/callbacks.py` & `scandeval-7.1.1/src/scandeval/callbacks.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.1.0/src/scandeval/cli.py` & `scandeval-7.1.1/src/scandeval/cli.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.1.0/src/scandeval/config.py` & `scandeval-7.1.1/src/scandeval/config.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.1.0/src/scandeval/dataset_configs.py` & `scandeval-7.1.1/src/scandeval/dataset_configs.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.1.0/src/scandeval/dataset_factory.py` & `scandeval-7.1.1/src/scandeval/dataset_factory.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.1.0/src/scandeval/dataset_tasks.py` & `scandeval-7.1.1/src/scandeval/dataset_tasks.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.1.0/src/scandeval/exceptions.py` & `scandeval-7.1.1/src/scandeval/exceptions.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.1.0/src/scandeval/hf_hub.py` & `scandeval-7.1.1/src/scandeval/hf_hub.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.1.0/src/scandeval/languages.py` & `scandeval-7.1.1/src/scandeval/languages.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.1.0/src/scandeval/model_loading.py` & `scandeval-7.1.1/src/scandeval/model_loading.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.1.0/src/scandeval/named_entity_recognition.py` & `scandeval-7.1.1/src/scandeval/named_entity_recognition.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         Returns:
             DatasetDict:
                 The processed dataset dictionary.
         """
         # Check what labels are present in the dataset, and store if MISC tags are not
         # present
         labels_in_train: Set[str] = {
-            tag for tag_list in dataset_dict["train"]["ner_tags"] for tag in tag_list
+            tag for tag_list in dataset_dict["train"]["labels"] for tag in tag_list
         }
         self.has_misc_tags = "B-MISC" in labels_in_train or "I-MISC" in labels_in_train
 
         # Return the dataset dictionary
         return dataset_dict
 
     def _compute_metrics(
@@ -172,15 +172,15 @@
 
         # Extract a mapping between all the tokens and their corresponding word. If the
         # tokenizer is of a "fast" variant then this can be accessed through the
         # `word_ids` method. Otherwise, we have to extract it manually.
         all_labels: List[List[int]] = list()
         labels: List[str]
         word_ids: List[Optional[int]]
-        for i, labels in enumerate(examples["ner_tags"]):
+        for i, labels in enumerate(examples["labels"]):
             # Try to get the word IDs from the tokenizer
             try:
                 word_ids = tokenized_inputs.word_ids(batch_index=i)
 
             # If the tokenizer is not of a "fast" variant, we have to extract the word
             # IDs manually
             except ValueError:
```

### Comparing `ScandEval-7.1.0/src/scandeval/norbert.py` & `scandeval-7.1.1/src/scandeval/norbert.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.1.0/src/scandeval/question_answering.py` & `scandeval-7.1.1/src/scandeval/question_answering.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.1.0/src/scandeval/question_answering_trainer.py` & `scandeval-7.1.1/src/scandeval/question_answering_trainer.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.1.0/src/scandeval/scores.py` & `scandeval-7.1.1/src/scandeval/scores.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.1.0/src/scandeval/sequence_classification.py` & `scandeval-7.1.1/src/scandeval/sequence_classification.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.1.0/src/scandeval/speed_benchmark.py` & `scandeval-7.1.1/src/scandeval/speed_benchmark.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.1.0/src/scandeval/utils.py` & `scandeval-7.1.1/src/scandeval/utils.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.1.0/setup.py` & `scandeval-7.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,225 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-package_dir = \
-{'': 'src'}
-
-packages = \
-['scandeval']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['accelerate>=0.19.0,<1.0.0',
- 'click>=8.1.3,<9.0.0',
- 'datasets>=2.7.0,<3.0.0',
- 'evaluate>=0.3.0,<1.0.0',
- 'flax>=0.6.3,<1.0.0',
- 'huggingface-hub>=0.7.0,<1.0.0',
- 'jax>=0.4.1,<1.0.0',
- 'jaxlib>=0.4.1,<1.0.0',
- 'numpy>=1.23.0,<2.0.0',
- 'pandas>=1.4.0,<2.0.0',
- 'protobuf>=3.20.0,<3.21.0',
- 'pyinfer>=0.0.3,<1.0.0',
- 'python-dotenv>=0.20.0,<1.0.0',
- 'sacremoses>=0.0.53,<1.0.0',
- 'sentencepiece>=0.1.96,<1.0.0',
- 'seqeval>=1.2.2,<2.0.0',
- 'termcolor>=1.1.0,<2.0.0',
- 'torch>=2.0.0,<3.0.0',
- 'tqdm>=4.62.0,<5.0.0',
- 'transformers>=4.20.0,<5.0.0']
-
-entry_points = \
-{'console_scripts': ['scandeval = scandeval.cli:benchmark']}
-
-setup_kwargs = {
-    'name': 'scandeval',
-    'version': '7.1.0',
-    'description': 'Evaluation of pretrained language models on mono- or multilingual Scandinavian language tasks.',
-    'long_description': '<div align=\'center\'>\n<img src="https://raw.githubusercontent.com/saattrupdan/ScandEval/main/gfx/scandeval.png" width="517" height="217">\n</div>\n\n### Evaluation of pretrained language models on mono- or multilingual Scandinavian language tasks.\n\n______________________________________________________________________\n[![PyPI Status](https://badge.fury.io/py/scandeval.svg)](https://pypi.org/project/scandeval/)\n[![Paper](https://img.shields.io/badge/arXiv-2304.00906-b31b1b.svg)](https://arxiv.org/abs/2304.00906)\n[![License](https://img.shields.io/github/license/saattrupdan/ScandEval)](https://github.com/saattrupdan/ScandEval/blob/main/LICENSE)\n[![LastCommit](https://img.shields.io/github/last-commit/saattrupdan/ScandEval)](https://github.com/saattrupdan/ScandEval/commits/main)\n[![Code Coverage](https://img.shields.io/badge/Coverage-76%25-yellowgreen.svg)](https://github.com/saattrupdan/ScandEval/tree/main/tests)\n[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)](https://github.com/saattrupdan/ScandEval/blob/main/CODE_OF_CONDUCT.md)\n\n\n## Installation\nTo install the package simply write the following command in your favorite terminal:\n```\n$ pip install scandeval\n```\n\n## Quickstart\n### Benchmarking from the Command Line\nThe easiest way to benchmark pretrained models is via the command line interface. After\nhaving installed the package, you can benchmark your favorite model like so:\n```\n$ scandeval --model-id <model-id>\n```\n\nHere `model_id` is the HuggingFace model ID, which can be found on the [HuggingFace\nHub](https://huggingface.co/models). By default this will benchmark the model on all\nthe datasets eligible. If you want to benchmark on a specific dataset, this can be done\nvia the `--dataset` flag. This will for instance evaluate the model on the\n`AngryTweets` dataset:\n```\n$ scandeval --model-id <model-id> --dataset angry-tweets\n```\n\nWe can also separate by language. To benchmark all Danish models on all Danish\ndatasets, say, this can be done using the `language` tag, like so:\n```\n$ scandeval --language da\n```\n\nMultiple models, datasets and/or languages can be specified by just attaching multiple\narguments. Here is an example with two models:\n```\n$ scandeval --model-id <model-id1> --model-id <model-id2> --dataset angry-tweets\n```\n\nThe specific model version to use can also be added after the suffix \'@\':\n```\n$ scandeval --model-id <model-id>@<commit>\n```\n\nIt can be a branch name, a tag name, or a commit id. It defaults to \'main\' for latest.\n\nSee all the arguments and options available for the `scandeval` command by typing\n```\n$ scandeval --help\n```\n\n### Benchmarking from a Script\nIn a script, the syntax is similar to the command line interface. You simply initialise\nan object of the `Benchmarker` class, and call this benchmark object with your favorite\nmodels and/or datasets:\n```\n>>> from scandeval import Benchmarker\n>>> benchmark = Benchmarker()\n>>> benchmark(\'<model-id>\')\n```\n\nTo benchmark on a specific dataset, you simply specify the second argument, shown here\nwith the `AngryTweets` dataset again:\n```\n>>> benchmark(\'<model_id>\', \'angry-tweets\')\n```\n\nIf you want to benchmark a subset of all the models on the Hugging Face Hub, you can\nspecify several parameters in the `Benchmarker` initializer to narrow down the list of\nmodels to the ones you care about. As a simple example, the following would benchmark\nall the Nynorsk models on Nynorsk datasets:\n```\n>>> benchmark = Benchmarker(language=\'nn\')\n>>> benchmark()\n```\n\n\n## Citing ScandEval\nIf you want to cite the framework then feel free to use this:\n\n```\n@inproceedings{nielsen2023scandeval,\n  title={ScandEval: A Benchmark for Scandinavian Natural Language Processing},\n  author={Nielsen, Dan Saattrup},\n  booktitle={The 24rd Nordic Conference on Computational Linguistics},\n  year={2023}\n}\n```\n\n\n## Remarks\nThe image used in the logo has been created by the amazing [Scandinavia and the\nWorld](https://satwcomic.com/) team. Go check them out!\n\n\n## Project structure\n```\n.\n├── .flake8\n├── .github\n│\xa0\xa0 └── workflows\n│\xa0\xa0     └── ci.yaml\n├── .gitignore\n├── .pre-commit-config.yaml\n├── CHANGELOG.md\n├── LICENSE\n├── README.md\n├── gfx\n│\xa0\xa0 └── scandeval.png\n├── makefile\n├── poetry.toml\n├── pyproject.toml\n├── src\n│\xa0\xa0 ├── scandeval\n│\xa0\xa0 │\xa0\xa0 ├── __init__.py\n│\xa0\xa0 │\xa0\xa0 ├── benchmark_config_factory.py\n│\xa0\xa0 │\xa0\xa0 ├── benchmark_dataset.py\n│\xa0\xa0 │\xa0\xa0 ├── benchmarker.py\n│\xa0\xa0 │\xa0\xa0 ├── callbacks.py\n│\xa0\xa0 │\xa0\xa0 ├── cli.py\n│\xa0\xa0 │\xa0\xa0 ├── config.py\n│\xa0\xa0 │\xa0\xa0 ├── dataset_configs.py\n│\xa0\xa0 │\xa0\xa0 ├── dataset_factory.py\n│\xa0\xa0 │\xa0\xa0 ├── dataset_tasks.py\n│\xa0\xa0 │\xa0\xa0 ├── exceptions.py\n│\xa0\xa0 │\xa0\xa0 ├── hf_hub.py\n│\xa0\xa0 │\xa0\xa0 ├── languages.py\n│\xa0\xa0 │\xa0\xa0 ├── model_loading.py\n│\xa0\xa0 │\xa0\xa0 ├── named_entity_recognition.py\n│\xa0\xa0 │\xa0\xa0 ├── question_answering.py\n│\xa0\xa0 │\xa0\xa0 ├── question_answering_trainer.py\n│\xa0\xa0 │\xa0\xa0 ├── scores.py\n│\xa0\xa0 │\xa0\xa0 ├── sequence_classification.py\n│\xa0\xa0 │\xa0\xa0 ├── speed_benchmark.py\n│\xa0\xa0 │\xa0\xa0 ├── types.py\n│\xa0\xa0 │\xa0\xa0 └── utils.py\n│\xa0\xa0 └── scripts\n│\xa0\xa0     ├── create_angry_tweets.py\n│\xa0\xa0     ├── create_dane.py\n│\xa0\xa0     ├── create_mim_gold_ner.py\n│\xa0\xa0     ├── create_norec.py\n│\xa0\xa0     ├── create_norne.py\n│\xa0\xa0     ├── create_scala.py\n│\xa0\xa0     ├── create_scandiqa.py\n│\xa0\xa0     ├── create_suc3.py\n│\xa0\xa0     ├── create_swerec.py\n│\xa0\xa0     ├── create_wikiann_fo.py\n│\xa0\xa0     ├── fill_in_missing_model_metadata.py\n│\xa0\xa0     ├── fix_dot_env_file.py\n│\xa0\xa0     ├── load_ud_pos.py\n│\xa0\xa0     └── versioning.py\n└── tests\n    ├── __init__.py\n    ├── conftest.py\n    ├── test_benchmark_config_factory.py\n    ├── test_benchmark_dataset.py\n    ├── test_benchmarker.py\n    ├── test_callbacks.py\n    ├── test_cli.py\n    ├── test_config.py\n    ├── test_dataset_configs.py\n    ├── test_dataset_factory.py\n    ├── test_dataset_tasks.py\n    ├── test_exceptions.py\n    ├── test_hf_hub.py\n    ├── test_languages.py\n    ├── test_model_loading.py\n    ├── test_named_entity_recognition.py\n    ├── test_question_answering.py\n    ├── test_question_answering_trainer.py\n    ├── test_scores.py\n    ├── test_sequence_classification.py\n    ├── test_speed_benchmark.py\n    ├── test_types.py\n    └── test_utils.py\n```\n',
-    'author': 'Dan Saattrup Nielsen',
-    'author_email': 'saattrupdan@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://scandeval.github.io',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.11',
+Metadata-Version: 2.1
+Name: scandeval
+Version: 7.1.1
+Summary: Evaluation of pretrained language models on mono- or multilingual Scandinavian language tasks.
+Home-page: https://scandeval.github.io
+License: MIT
+Author: Dan Saattrup Nielsen
+Author-email: saattrupdan@gmail.com
+Requires-Python: >=3.8,<3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: accelerate (>=0.19.0,<1.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: datasets (>=2.7.0,<3.0.0)
+Requires-Dist: evaluate (>=0.3.0,<1.0.0)
+Requires-Dist: flax (>=0.6.3,<1.0.0)
+Requires-Dist: huggingface-hub (>=0.7.0,<1.0.0)
+Requires-Dist: jax (>=0.4.1,<1.0.0)
+Requires-Dist: jaxlib (>=0.4.1,<1.0.0)
+Requires-Dist: numpy (>=1.23.0,<2.0.0)
+Requires-Dist: pandas (>=1.4.0,<2.0.0)
+Requires-Dist: protobuf (>=3.20.0,<3.21.0)
+Requires-Dist: pyinfer (>=0.0.3,<1.0.0)
+Requires-Dist: python-dotenv (>=0.20.0,<1.0.0)
+Requires-Dist: sacremoses (>=0.0.53,<1.0.0)
+Requires-Dist: sentencepiece (>=0.1.96,<1.0.0)
+Requires-Dist: seqeval (>=1.2.2,<2.0.0)
+Requires-Dist: termcolor (>=1.1.0,<2.0.0)
+Requires-Dist: torch (>=2.0.0,<3.0.0)
+Requires-Dist: tqdm (>=4.62.0,<5.0.0)
+Requires-Dist: transformers (>=4.20.0,<5.0.0)
+Project-URL: Repository, https://github.com/saattrupdan/ScandEval
+Description-Content-Type: text/markdown
+
+<div align='center'>
+<img src="https://raw.githubusercontent.com/saattrupdan/ScandEval/main/gfx/scandeval.png" width="517" height="217">
+</div>
+
+### Evaluation of pretrained language models on mono- or multilingual Scandinavian language tasks.
+
+______________________________________________________________________
+[![PyPI Status](https://badge.fury.io/py/scandeval.svg)](https://pypi.org/project/scandeval/)
+[![Paper](https://img.shields.io/badge/arXiv-2304.00906-b31b1b.svg)](https://arxiv.org/abs/2304.00906)
+[![License](https://img.shields.io/github/license/saattrupdan/ScandEval)](https://github.com/saattrupdan/ScandEval/blob/main/LICENSE)
+[![LastCommit](https://img.shields.io/github/last-commit/saattrupdan/ScandEval)](https://github.com/saattrupdan/ScandEval/commits/main)
+[![Code Coverage](https://img.shields.io/badge/Coverage-64%25-yellow.svg)](https://github.com/saattrupdan/ScandEval/tree/main/tests)
+[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)](https://github.com/saattrupdan/ScandEval/blob/main/CODE_OF_CONDUCT.md)
+
+
+## Installation
+To install the package simply write the following command in your favorite terminal:
+```
+$ pip install scandeval
+```
+
+## Quickstart
+### Benchmarking from the Command Line
+The easiest way to benchmark pretrained models is via the command line interface. After
+having installed the package, you can benchmark your favorite model like so:
+```
+$ scandeval --model-id <model-id>
+```
+
+Here `model_id` is the HuggingFace model ID, which can be found on the [HuggingFace
+Hub](https://huggingface.co/models). By default this will benchmark the model on all
+the datasets eligible. If you want to benchmark on a specific dataset, this can be done
+via the `--dataset` flag. This will for instance evaluate the model on the
+`AngryTweets` dataset:
+```
+$ scandeval --model-id <model-id> --dataset angry-tweets
+```
+
+We can also separate by language. To benchmark all Danish models on all Danish
+datasets, say, this can be done using the `language` tag, like so:
+```
+$ scandeval --language da
+```
+
+Multiple models, datasets and/or languages can be specified by just attaching multiple
+arguments. Here is an example with two models:
+```
+$ scandeval --model-id <model-id1> --model-id <model-id2> --dataset angry-tweets
+```
+
+The specific model version to use can also be added after the suffix '@':
+```
+$ scandeval --model-id <model-id>@<commit>
+```
+
+It can be a branch name, a tag name, or a commit id. It defaults to 'main' for latest.
+
+See all the arguments and options available for the `scandeval` command by typing
+```
+$ scandeval --help
+```
+
+### Benchmarking from a Script
+In a script, the syntax is similar to the command line interface. You simply initialise
+an object of the `Benchmarker` class, and call this benchmark object with your favorite
+models and/or datasets:
+```
+>>> from scandeval import Benchmarker
+>>> benchmark = Benchmarker()
+>>> benchmark('<model-id>')
+```
+
+To benchmark on a specific dataset, you simply specify the second argument, shown here
+with the `AngryTweets` dataset again:
+```
+>>> benchmark('<model_id>', 'angry-tweets')
+```
+
+If you want to benchmark a subset of all the models on the Hugging Face Hub, you can
+specify several parameters in the `Benchmarker` initializer to narrow down the list of
+models to the ones you care about. As a simple example, the following would benchmark
+all the Nynorsk models on Nynorsk datasets:
+```
+>>> benchmark = Benchmarker(language='nn')
+>>> benchmark()
+```
+
+
+## Citing ScandEval
+If you want to cite the framework then feel free to use this:
+
+```
+@inproceedings{nielsen2023scandeval,
+  title={ScandEval: A Benchmark for Scandinavian Natural Language Processing},
+  author={Nielsen, Dan Saattrup},
+  booktitle={The 24rd Nordic Conference on Computational Linguistics},
+  year={2023}
 }
+```
+
 
+## Remarks
+The image used in the logo has been created by the amazing [Scandinavia and the
+World](https://satwcomic.com/) team. Go check them out!
+
+
+## Project structure
+```
+.
+├── .flake8
+├── .github
+│   └── workflows
+│       └── ci.yaml
+├── .gitignore
+├── .pre-commit-config.yaml
+├── CHANGELOG.md
+├── LICENSE
+├── README.md
+├── gfx
+│   └── scandeval.png
+├── makefile
+├── poetry.toml
+├── pyproject.toml
+├── src
+│   ├── scandeval
+│   │   ├── __init__.py
+│   │   ├── benchmark_config_factory.py
+│   │   ├── benchmark_dataset.py
+│   │   ├── benchmarker.py
+│   │   ├── callbacks.py
+│   │   ├── cli.py
+│   │   ├── config.py
+│   │   ├── dataset_configs.py
+│   │   ├── dataset_factory.py
+│   │   ├── dataset_tasks.py
+│   │   ├── exceptions.py
+│   │   ├── hf_hub.py
+│   │   ├── languages.py
+│   │   ├── model_loading.py
+│   │   ├── named_entity_recognition.py
+│   │   ├── question_answering.py
+│   │   ├── question_answering_trainer.py
+│   │   ├── scores.py
+│   │   ├── sequence_classification.py
+│   │   ├── speed_benchmark.py
+│   │   ├── types.py
+│   │   └── utils.py
+│   └── scripts
+│       ├── create_angry_tweets.py
+│       ├── create_dane.py
+│       ├── create_mim_gold_ner.py
+│       ├── create_norec.py
+│       ├── create_norne.py
+│       ├── create_scala.py
+│       ├── create_scandiqa.py
+│       ├── create_suc3.py
+│       ├── create_swerec.py
+│       ├── create_wikiann_fo.py
+│       ├── fill_in_missing_model_metadata.py
+│       ├── fix_dot_env_file.py
+│       ├── load_ud_pos.py
+│       └── versioning.py
+└── tests
+    ├── __init__.py
+    ├── conftest.py
+    ├── test_benchmark_config_factory.py
+    ├── test_benchmark_dataset.py
+    ├── test_benchmarker.py
+    ├── test_callbacks.py
+    ├── test_cli.py
+    ├── test_config.py
+    ├── test_dataset_configs.py
+    ├── test_dataset_factory.py
+    ├── test_dataset_tasks.py
+    ├── test_exceptions.py
+    ├── test_hf_hub.py
+    ├── test_languages.py
+    ├── test_model_loading.py
+    ├── test_named_entity_recognition.py
+    ├── test_question_answering.py
+    ├── test_question_answering_trainer.py
+    ├── test_scores.py
+    ├── test_sequence_classification.py
+    ├── test_speed_benchmark.py
+    ├── test_types.py
+    └── test_utils.py
+```
 
-setup(**setup_kwargs)
```

