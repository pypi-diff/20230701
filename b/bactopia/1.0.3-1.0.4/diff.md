# Comparing `tmp/bactopia-1.0.3.tar.gz` & `tmp/bactopia-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bactopia-1.0.3.tar", max compression
+gzip compressed data, was "bactopia-1.0.4.tar", max compression
```

## Comparing `bactopia-1.0.3.tar` & `bactopia-1.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1065 2023-05-31 04:39:04.837370 bactopia-1.0.3/LICENSE
--rw-r--r--   0        0        0    27493 2023-05-31 04:39:04.837370 bactopia-1.0.3/README.md
--rw-r--r--   0        0        0      113 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/cli/__init__.py
--rw-r--r--   0        0        0     2667 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/cli/citations.py
--rw-r--r--   0        0        0     5118 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/cli/datasets.py
--rw-r--r--   0        0        0    19341 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/cli/download.py
--rw-r--r--   0        0        0     2416 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/cli/jsonify.py
--rw-r--r--   0        0        0    16397 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/cli/prepare.py
--rw-r--r--   0        0        0    20125 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/cli/search.py
--rw-r--r--   0        0        0    15455 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/cli/summary.py
--rw-r--r--   0        0        0     1398 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parse.py
--rw-r--r--   0        0        0      267 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/__init__.py
--rw-r--r--   0        0        0      484 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/amrfinderplus.py
--rw-r--r--   0        0        0     1000 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/annotator.py
--rw-r--r--   0        0        0     2783 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/ariba.py
--rw-r--r--   0        0        0      664 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/assembler.py
--rw-r--r--   0        0        0     4673 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/blast.py
--rw-r--r--   0        0        0     1365 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/error.py
--rw-r--r--   0        0        0      372 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/gather.py
--rw-r--r--   0        0        0     1492 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/generic.py
--rw-r--r--   0        0        0     2683 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/mapping.py
--rw-r--r--   0        0        0      640 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/mlst.py
--rw-r--r--   0        0        0     1599 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/parsables.py
--rw-r--r--   0        0        0     3093 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/qc.py
--rw-r--r--   0        0        0     5014 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/sketcher.py
--rw-r--r--   0        0        0     2574 2023-05-31 04:39:04.837370 bactopia-1.0.3/bactopia/parsers/variants.py
--rw-r--r--   0        0        0      874 2023-05-31 04:39:04.841370 bactopia-1.0.3/bactopia/parsers/versions.py
--rw-r--r--   0        0        0     5292 2023-05-31 04:39:04.841370 bactopia-1.0.3/bactopia/summary.py
--rw-r--r--   0        0        0     4496 2023-05-31 04:39:04.841370 bactopia-1.0.3/bactopia/utils.py
--rw-r--r--   0        0        0     1034 2023-05-31 04:39:04.841370 bactopia-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    29064 1970-01-01 00:00:00.000000 bactopia-1.0.3/setup.py
--rw-r--r--   0        0        0    28407 1970-01-01 00:00:00.000000 bactopia-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-01 00:24:13.088709 bactopia-1.0.4/LICENSE
+-rw-r--r--   0        0        0    27493 2023-07-01 00:24:13.088709 bactopia-1.0.4/README.md
+-rw-r--r--   0        0        0      113 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/cli/__init__.py
+-rw-r--r--   0        0        0     2667 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/cli/citations.py
+-rw-r--r--   0        0        0     5118 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/cli/datasets.py
+-rw-r--r--   0        0        0    19341 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/cli/download.py
+-rw-r--r--   0        0        0     2416 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/cli/jsonify.py
+-rw-r--r--   0        0        0    16397 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/cli/prepare.py
+-rw-r--r--   0        0        0    20125 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/cli/search.py
+-rw-r--r--   0        0        0    15455 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/cli/summary.py
+-rw-r--r--   0        0        0     1388 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parse.py
+-rw-r--r--   0        0        0      267 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/__init__.py
+-rw-r--r--   0        0        0      484 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/amrfinderplus.py
+-rw-r--r--   0        0        0     1000 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/annotator.py
+-rw-r--r--   0        0        0     2783 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/ariba.py
+-rw-r--r--   0        0        0      664 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/assembler.py
+-rw-r--r--   0        0        0     4673 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/blast.py
+-rw-r--r--   0        0        0     1365 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/error.py
+-rw-r--r--   0        0        0      372 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/gather.py
+-rw-r--r--   0        0        0     1492 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/generic.py
+-rw-r--r--   0        0        0     2683 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/mapping.py
+-rw-r--r--   0        0        0      640 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/mlst.py
+-rw-r--r--   0        0        0     1500 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/parsables.py
+-rw-r--r--   0        0        0     3093 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/qc.py
+-rw-r--r--   0        0        0     5014 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/sketcher.py
+-rw-r--r--   0        0        0     2574 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/variants.py
+-rw-r--r--   0        0        0      874 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/parsers/versions.py
+-rw-r--r--   0        0        0     5292 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/summary.py
+-rw-r--r--   0        0        0     4496 2023-07-01 00:24:13.092709 bactopia-1.0.4/bactopia/utils.py
+-rw-r--r--   0        0        0     1034 2023-07-01 00:24:13.092709 bactopia-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    29064 1970-01-01 00:00:00.000000 bactopia-1.0.4/setup.py
+-rw-r--r--   0        0        0    28407 1970-01-01 00:00:00.000000 bactopia-1.0.4/PKG-INFO
```

### Comparing `bactopia-1.0.3/LICENSE` & `bactopia-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/README.md` & `bactopia-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/bactopia/cli/citations.py` & `bactopia-1.0.4/bactopia/cli/citations.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/bactopia/cli/datasets.py` & `bactopia-1.0.4/bactopia/cli/datasets.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/bactopia/cli/download.py` & `bactopia-1.0.4/bactopia/cli/download.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/bactopia/cli/jsonify.py` & `bactopia-1.0.4/bactopia/cli/jsonify.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/bactopia/cli/prepare.py` & `bactopia-1.0.4/bactopia/cli/prepare.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/bactopia/cli/search.py` & `bactopia-1.0.4/bactopia/cli/search.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/bactopia/cli/summary.py` & `bactopia-1.0.4/bactopia/cli/summary.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/bactopia/parse.py` & `bactopia-1.0.4/bactopia/parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Example: bactopia.parse(result_type, filename)
 """
 from pathlib import Path
 
 IGNORE_LIST = [
     ".nextflow",
     ".nextflow.log",
+    "bactopia-runs",
     "nf-reports",
     "work",
 ]
 
 
 def parse_bactopia_directory(path: str) -> list:
     """
@@ -20,15 +21,15 @@
     Args:
         path (str):  a path to expected Bactopia results
 
     Returns:
         list: Parsed results for all samples in a Bactopia directory
     """
     results = []
-    for directory in Path(f"{path}/bactopia-samples").iterdir():
+    for directory in Path(path).iterdir():
         if directory.is_dir():
             if directory.name not in IGNORE_LIST:
                 results.append(
                     {
                         "id": directory.name,
                         "path": directory.absolute(),
                         "is_bactopia": _is_bactopia_dir(
@@ -47,8 +48,8 @@
     Args:
         path (str): a path to expected Bactopia results
         name (str): the name of sample to test
 
     Returns:
         bool: path looks like Bactopia (True) or not (False)
     """
-    return Path(f"{path}/bactopia-main/gather/{name}-meta.tsv").exists()
+    return Path(f"{path}/main/gather/{name}-meta.tsv").exists()
```

### Comparing `bactopia-1.0.3/bactopia/parsers/annotator.py` & `bactopia-1.0.4/bactopia/parsers/annotator.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/bactopia/parsers/ariba.py` & `bactopia-1.0.4/bactopia/parsers/ariba.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/bactopia/parsers/assembler.py` & `bactopia-1.0.4/bactopia/parsers/assembler.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/bactopia/parsers/blast.py` & `bactopia-1.0.4/bactopia/parsers/blast.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/bactopia/parsers/error.py` & `bactopia-1.0.4/bactopia/parsers/error.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/bactopia/parsers/generic.py` & `bactopia-1.0.4/bactopia/parsers/generic.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/bactopia/parsers/mapping.py` & `bactopia-1.0.4/bactopia/parsers/mapping.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/bactopia/parsers/mlst.py` & `bactopia-1.0.4/bactopia/parsers/mlst.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/bactopia/parsers/parsables.py` & `bactopia-1.0.4/bactopia/parsers/parsables.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,27 +19,27 @@
     "amrfinderplus_genes_hits",
     "amrfinderplus_proteins_hits",
 ]
 
 
 def get_parsable_files(path: str, name: str) -> list:
     return {
-        # bactopia-main
+        # main
         # annotator
-        f"{path}/bactopia-main/annotator/prokka/{name}.txt": "annotator",
+        f"{path}/main/annotator/prokka/{name}.txt": "annotator",
         # assembler
-        f"{path}/bactopia-main/assembler/{name}.tsv": "assembler",
+        f"{path}/main/assembler/{name}.tsv": "assembler",
         # gather
-        f"{path}/bactopia-main/gather/{name}-meta.tsv": "gather",
+        f"{path}/main/gather/{name}-meta.tsv": "gather",
         # qc
-        f"{path}/bactopia-main/qc/summary/{name}-final.json": "qc",
-        f"{path}/bactopia-main/qc/summary/{name}-original.json": "qc",
+        f"{path}/main/qc/summary/{name}-final.json": "qc",
+        f"{path}/main/qc/summary/{name}-original.json": "qc",
         # sketcher
-        f"{path}/bactopia-main/sketcher/summary/{name}-mash-refseq88-k21.txt": "sketcher",
-        f"{path}/bactopia-main/sketcher/summary/{name}-sourmash-gtdb-rs207-k31.txt": "sketcher",
+        f"{path}/main/sketcher/summary/{name}-mash-refseq88-k21.txt": "sketcher",
+        f"{path}/main/sketcher/summary/{name}-sourmash-gtdb-rs207-k31.txt": "sketcher",
         # bactopia-tools
         # amrfinderplus
-        f"{path}/bactopia-tools/amrfinderplus/{name}-genes.tsv": "amrfinderplus",
-        f"{path}/bactopia-tools/amrfinderplus/{name}-proteins.tsv": "amrfinderplus",
+        f"{path}/tools/amrfinderplus/{name}-genes.tsv": "amrfinderplus",
+        f"{path}/tools/amrfinderplus/{name}-proteins.tsv": "amrfinderplus",
         # mlst
-        f"{path}/bactopia-tools/mlst/{name}.tsv": "mlst",
+        f"{path}/tools/mlst/{name}.tsv": "mlst",
     }
```

### Comparing `bactopia-1.0.3/bactopia/parsers/qc.py` & `bactopia-1.0.4/bactopia/parsers/qc.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/bactopia/parsers/sketcher.py` & `bactopia-1.0.4/bactopia/parsers/sketcher.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/bactopia/parsers/variants.py` & `bactopia-1.0.4/bactopia/parsers/variants.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/bactopia/parsers/versions.py` & `bactopia-1.0.4/bactopia/parsers/versions.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/bactopia/summary.py` & `bactopia-1.0.4/bactopia/summary.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/bactopia/utils.py` & `bactopia-1.0.4/bactopia/utils.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.3/pyproject.toml` & `bactopia-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bactopia"
-version = "1.0.3"
+version = "1.0.4"
 description = "A Python package for working with Bactopia"
 authors = [
     "Robert A. Petit III <robbie.petit@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://bactopia.github.io/"
```

### Comparing `bactopia-1.0.3/setup.py` & `bactopia-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                      'bactopia-download = bactopia.cli.download:main',
                      'bactopia-prepare = bactopia.cli.prepare:main',
                      'bactopia-search = bactopia.cli.search:main',
                      'bactopia-summary = bactopia.cli.summary:main']}
 
 setup_kwargs = {
     'name': 'bactopia',
-    'version': '1.0.3',
+    'version': '1.0.4',
     'description': 'A Python package for working with Bactopia',
     'long_description': "[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-908a85?logo=gitpod)](https://gitpod.io/#https://github.com/bactopia/bactopia-py)\n\n![Bactopia Logo](https://raw.githubusercontent.com/bactopia/bactopia/master/data/bactopia-logo.png)\n\n# bactopia-py\nA Python package for working with [Bactopia](https://bactopia.github.io/)\n\n## Bactopia Subcommands\n\nThere are many subcommands available in Bactopia. Here is a brief description of each command:\n\n| Command              | Description                                                                |\n|----------------------|----------------------------------------------------------------------------|\n| `bactopia-citations` | Print out tools and citations used throughout Bactopia                     |\n| `bactopia-datasets`  | Download optional datasets to supplement your analyses with Bactopia       |\n| `bactopia-download`  | Builds Bactopia environments for use with Nextflow.                        |\n| `bactopia-prepare`   | Create a 'file of filenames' (FOFN) of samples to be processed by Bactopia |\n| `bactopia-search`    | Query against ENA and SRA for public accessions to process with Bactopia   |\n| `bactopia-summary`   | Generate a summary table from the Bactopia results.                        |\n\nBelow is the `--help` output for each subcommand.\n\n### `bactopia-citations`\n\n```{bash}\n Usage: bactopia-citations [OPTIONS]\n\n Print out tools and citations used throughout Bactopia\n\n╭─ Options ────────────────────────────────────────────────────────────────────────────╮\n│    --version        -V        Show the version and exit.                             │\n│ *  --bactopia-path  -b  TEXT  Directory where Bactopia repository is stored          │\n│                               [required]                                             │\n│    --name           -n  TEXT  Only print citation matching a given name              │\n│    --plain-text     -p        Disable rich formatting                                │\n│    --help                     Show this message and exit.                            │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-datasets`\n\n```{bash}\n Usage: bactopia-datasets [OPTIONS] [UNKNOWN]...\n\n Download optional datasets to supplement your analyses with Bactopia\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --bactopia-path    TEXT  Directory where Bactopia repository is stored [required] │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Download Related Options ───────────────────────────────────────────────────────────╮\n│ --datasets_cache    TEXT     Base directory to download datasets to (Defaults to env │\n│                              variable BACTOPIA_CACHEDIR, a subfolder called datasets │\n│                              will be created)                                        │\n│                              [default: ${HOME}/.bactopia]                 │\n│ --force                      Force overwrite of existing pre-built environments.     │\n│ --max_retry         INTEGER  Maximum times to attempt creating Conda environment.    │\n│                              (Default: 3)                                            │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --verbose      Print debug related text.                                             │\n│ --silent       Only critical errors will be printed.                                 │\n│ --version      Show the version and exit.                                            │\n│ --help         Show this message and exit.                                           │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n\n```\n\n### `bactopia-download`\n\n```{bash}\n Usage: bactopia-download [OPTIONS] [UNKNOWN]...\n\n Builds Bactopia environments for use with Nextflow.\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --bactopia-path    TEXT  Directory where Bactopia results are stored [required]   │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Build Related Options ──────────────────────────────────────────────────────────────╮\n│ --envtype                     [conda|docker|singularity|  The type of environment to │\n│                               all]                        build.                     │\n│                                                           [default: conda]           │\n│ --wf                          TEXT                        Build a environment for a  │\n│                                                           the given workflow         │\n│                                                           [default: bactopia]        │\n│ --condadir                    TEXT                        Directory to create Conda  │\n│                                                           environments               │\n│                                                           (NXF_CONDA_CACHEDIR env    │\n│                                                           variable takes precedence) │\n│ --use_conda                                               Use Conda for building     │\n│                                                           Conda environments instead │\n│                                                           of Mamba                   │\n│ --singularity_cache           TEXT                        Directory to download      │\n│                                                           Singularity images         │\n│                                                           (NXF_SINGULARITY_CACHEDIR  │\n│                                                           env variable takes         │\n│                                                           precedence)                │\n│ --singularity_pull_docker…                                Force conversion of Docker │\n│                                                           containers, instead        │\n│                                                           downloading Singularity    │\n│                                                           images directly            │\n│ --force_rebuild                                           Force overwrite of         │\n│                                                           existing pre-built         │\n│                                                           environments.              │\n│ --max_retry                   INTEGER                     Maximum times to attempt   │\n│                                                           creating Conda             │\n│                                                           environment. (Default: 3)  │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --verbose      Print debug related text.                                             │\n│ --silent       Only critical errors will be printed.                                 │\n│ --version      Show the version and exit.                                            │\n│ --help         Show this message and exit.                                           │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Options ────────────────────────────────────────────────────────────────────────────╮\n│ --build-all         Builds all environments for Bactopia workflows                   │\n│ --build-nfcore      Builds all nf-core related environments                          │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-prepare`\n\n```{bash}\n Usage: bactopia-prepare [OPTIONS]\n\n Create a 'file of filenames' (FOFN) of samples to be processed by Bactopia\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --path  -p  TEXT  Directory where FASTQ files are stored [required]               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Matching Options ───────────────────────────────────────────────────────────────────╮\n│ --assembly-ext     -a  TEXT  Extension of the FASTA assemblies [default: .fna.gz]    │\n│ --fastq-ext        -f  TEXT  Extension of the FASTQs [default: .fastq.gz]            │\n│ --fastq-separator      TEXT  Split FASTQ name on the last occurrence of the          │\n│                              separator                                               │\n│                              [default: _]                                            │\n│ --pe1-pattern          TEXT  Designates difference first set of paired-end reads     │\n│                              [default: [Aa]|[Rr]1|1]                                 │\n│ --pe2-pattern          TEXT  Designates difference second set of paired-end reads    │\n│                              [default: [Bb]|[Rr]2|2]                                 │\n│ --merge                      Flag samples with multiple read sets to be merged by    │\n│                              Bactopia                                                │\n│ --ont                        Single-end reads should be treated as Oxford Nanopore   │\n│                              reads                                                   │\n│ --recursive        -r        Directories will be traversed recursively               │\n│ --prefix               TEXT  Prefix to add to the path                               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Sample Information Options ─────────────────────────────────────────────────────────╮\n│ --metadata             TEXT     Metadata per sample with genome size and species     │\n│                                 information                                          │\n│ --genome-size  -gsize  INTEGER  Genome size to use for all samples                   │\n│ --species      -s      TEXT     Species to use for all samples (If available, can be │\n│                                 used to determine genome size)                       │\n│ --taxid                TEXT     Use the genome size of the Taxon ID for all samples  │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --examples        Print example usage                                                │\n│ --verbose         Increase the verbosity of output                                   │\n│ --silent          Only critical errors will be printed                               │\n│ --version   -V    Show the version and exit.                                         │\n│ --help            Show this message and exit.                                        │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-search`\n\n```{bash}\n Usage: bactopia-search [OPTIONS]\n\n Query against ENA and SRA for public accessions to process with Bactopia\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --query  -q  TEXT  Taxon ID or Study, BioSample, or Run accession (can also be    │\n│                       comma separated or a file of accessions)                       │\n│                       [required]                                                     │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Query Options ──────────────────────────────────────────────────────────────────────╮\n│ --exact-taxon                     Exclude Taxon ID descendants                       │\n│ --limit             -l   INTEGER  Maximum number of results (per query) to return    │\n│                                   [default: 1000000]                                 │\n│ --accession-limit   -al  INTEGER  Maximum number of accessions to query at once      │\n│                                   [default: 5000]                                    │\n│ --biosample-subset       INTEGER  If a BioSample has multiple Experiments, maximum   │\n│                                   number to randomly select (0 = disabled)           │\n│                                   [default: 0]                                       │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Filtering Options ──────────────────────────────────────────────────────────────────╮\n│ --min-base-count   -mbc  INTEGER  Filters samples based on minimum base pair count   │\n│                                   (0 = disabled)                                     │\n│                                   [default: 0]                                       │\n│ --min-read-length  -mrl  INTEGER  Filters samples based on minimum mean read length  │\n│                                   (0 = disabled)                                     │\n│                                   [default: 0]                                       │\n│ --min-coverage     -mc   INTEGER  Filter samples based on minimum coverage (requires │\n│                                   --genome_size, 0 = disabled)                       │\n│                                   [default: 0]                                       │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --genome-size  -gsize  INTEGER  Genome size to be used for all samples, and for      │\n│                                 calculating min coverage                             │\n│                                 [default: 0]                                         │\n│ --outdir       -o      TEXT     Directory to write output [default: ./]              │\n│ --prefix       -p      TEXT     Prefix to use for output file names                  │\n│                                 [default: bactopia]                                  │\n│ --force                         Overwrite existing reports                           │\n│ --verbose                       Increase the verbosity of output                     │\n│ --silent                        Only critical errors will be printed                 │\n│ --version      -V               Show the version and exit.                           │\n│ --help                          Show this message and exit.                          │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-summary`\n\n```{bash}\n Usage: bactopia-summary [OPTIONS]\n\n Generate a summary table from the Bactopia results.\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --bactopia-path  -b  TEXT  Directory where Bactopia results are stored [required] │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Gold Cutoffs ───────────────────────────────────────────────────────────────────────╮\n│ --gold-coverage     -gcov      INTEGER  Minimum amount of coverage required for Gold │\n│                                         status                                       │\n│                                         [default: 100]                               │\n│ --gold-quality      -gqual     INTEGER  Minimum per-read mean quality score required │\n│                                         for Gold status                              │\n│                                         [default: 30]                                │\n│ --gold-read-length  -glen      INTEGER  Minimum mean read length required for Gold   │\n│                                         status                                       │\n│                                         [default: 95]                                │\n│ --gold-contigs      -gcontigs  INTEGER  Maximum contig count required for Gold       │\n│                                         status                                       │\n│                                         [default: 100]                               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Silver Cutoffs ─────────────────────────────────────────────────────────────────────╮\n│ --silver-coverage     -scov      INTEGER  Minimum amount of coverage required for    │\n│                                           Silver status                              │\n│                                           [default: 50]                              │\n│ --silver-quality      -squal     INTEGER  Minimum per-read mean quality score        │\n│                                           required for Silver status                 │\n│                                           [default: 20]                              │\n│ --silver-read-length  -slen      INTEGER  Minimum mean read length required for      │\n│                                           Silver status                              │\n│                                           [default: 75]                              │\n│ --silver-contigs      -scontigs  INTEGER  Maximum contig count required for Silver   │\n│                                           status                                     │\n│                                           [default: 200]                             │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Fail Cutoffs ───────────────────────────────────────────────────────────────────────╮\n│ --min-coverage        -mincov   INTEGER  Minimum amount of coverage required to pass │\n│                                          [default: 20]                               │\n│ --min-quality         -minqual  INTEGER  Minimum per-read mean quality score         │\n│                                          required to pass                            │\n│                                          [default: 12]                               │\n│ --min-read-length     -minlen   INTEGER  Minimum mean read length required to pass   │\n│                                          [default: 49]                               │\n│ --max-contigs                   INTEGER  Maximum contig count required to pass       │\n│                                          [default: 500]                              │\n│ --min-assembled-size            INTEGER  Minimum assembled genome size               │\n│ --max-assembled-size            INTEGER  Maximum assembled genome size               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --outdir   -o  PATH  Directory to write output [default: ./]                         │\n│ --prefix   -p  TEXT  Prefix to use for output files [default: bactopia]              │\n│ --force              Overwrite existing reports                                      │\n│ --verbose            Increase the verbosity of output                                │\n│ --silent             Only critical errors will be printed                            │\n│ --version  -V        Show the version and exit.                                      │\n│ --help               Show this message and exit.                                     │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n# Feedback\nYour feedback is very valuable! If you run into any issues using Bactopia, have questions, or have some ideas to improve Bactopia, I highly encourage you to submit it to the [Issue Tracker](https://github.com/bactopia/bactopia/issues).\n\n# License\n[MIT License](https://raw.githubusercontent.com/bactopia/bactopia/master/LICENSE)\n\n# Citation\n\nPetit III RA, Read TD, *Bactopia: a flexible pipeline for complete analysis of bacterial genomes.* __mSystems__. 5 (2020), https://doi.org/10.1128/mSystems.00190-20.\n\n# Author\n\n* Robert A. Petit III\n* Twitter: [@rpetit3](https://twitter.com/rpetit3)\n",
     'author': 'Robert A. Petit III',
     'author_email': 'robbie.petit@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://bactopia.github.io/',
```

### Comparing `bactopia-1.0.3/PKG-INFO` & `bactopia-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bactopia
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python package for working with Bactopia
 Home-page: https://bactopia.github.io/
 License: MIT
 Keywords: bioinformatics,bacteria,bactopia,SRA,ENA
 Author: Robert A. Petit III
 Author-email: robbie.petit@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
```

