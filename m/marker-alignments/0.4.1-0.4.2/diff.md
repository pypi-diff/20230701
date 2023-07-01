# Comparing `tmp/marker_alignments-0.4.1.tar.gz` & `tmp/marker_alignments-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/wbazant/dev/marker_alignments/dist/tmpincv72j3/marker_alignments-0.4.1.tar", last modified: Fri Apr  1 14:26:39 2022, max compression
+gzip compressed data, was "marker_alignments-0.4.2.tar", last modified: Sat Jul  1 15:54:11 2023, max compression
```

## Comparing `marker_alignments-0.4.1.tar` & `marker_alignments-0.4.2.tar`

### file list

```diff
@@ -1,23 +1,31 @@
-drwxrwxr-x   0 wbazant   (1001) wbazant   (1001)        0 2022-04-01 14:26:39.000000 marker_alignments-0.4.1/
--rw-rw-r--   0 wbazant   (1001) wbazant   (1001)    11281 2022-04-01 13:17:50.000000 marker_alignments-0.4.1/README.md
--rw-rw-r--   0 wbazant   (1001) wbazant   (1001)    11685 2022-04-01 14:26:38.000000 marker_alignments-0.4.1/PKG-INFO
--rw-rw-r--   0 wbazant   (1001) wbazant   (1001)       85 2022-04-01 11:38:56.000000 marker_alignments-0.4.1/pyproject.toml
--rw-r--r--   0 wbazant   (1001) wbazant   (1001)     1093 2022-04-01 11:39:35.000000 marker_alignments-0.4.1/LICENSE
--rw-rw-r--   0 wbazant   (1001) wbazant   (1001)       38 2022-04-01 14:26:39.000000 marker_alignments-0.4.1/setup.cfg
--rw-rw-r--   0 wbazant   (1001) wbazant   (1001)      846 2022-04-01 14:26:00.000000 marker_alignments-0.4.1/setup.py
-drwxrwxr-x   0 wbazant   (1001) wbazant   (1001)        0 2022-04-01 14:26:38.000000 marker_alignments-0.4.1/src/
-drwxrwxr-x   0 wbazant   (1001) wbazant   (1001)        0 2022-04-01 14:26:38.000000 marker_alignments-0.4.1/src/marker_alignments.egg-info/
--rw-rw-r--   0 wbazant   (1001) wbazant   (1001)       18 2022-04-01 14:26:38.000000 marker_alignments-0.4.1/src/marker_alignments.egg-info/top_level.txt
--rw-rw-r--   0 wbazant   (1001) wbazant   (1001)    11685 2022-04-01 14:26:38.000000 marker_alignments-0.4.1/src/marker_alignments.egg-info/PKG-INFO
--rw-rw-r--   0 wbazant   (1001) wbazant   (1001)      539 2022-04-01 14:26:38.000000 marker_alignments-0.4.1/src/marker_alignments.egg-info/SOURCES.txt
--rw-rw-r--   0 wbazant   (1001) wbazant   (1001)       26 2022-04-01 14:26:38.000000 marker_alignments-0.4.1/src/marker_alignments.egg-info/requires.txt
--rw-rw-r--   0 wbazant   (1001) wbazant   (1001)       67 2022-04-01 14:26:38.000000 marker_alignments-0.4.1/src/marker_alignments.egg-info/entry_points.txt
--rw-rw-r--   0 wbazant   (1001) wbazant   (1001)        1 2022-04-01 14:26:38.000000 marker_alignments-0.4.1/src/marker_alignments.egg-info/dependency_links.txt
-drwxrwxr-x   0 wbazant   (1001) wbazant   (1001)        0 2022-04-01 14:26:38.000000 marker_alignments-0.4.1/src/marker_alignments/
--rw-rw-r--   0 wbazant   (1001) wbazant   (1001)        0 2021-09-13 10:01:05.000000 marker_alignments-0.4.1/src/marker_alignments/__init__.py
--rw-rw-r--   0 wbazant   (1001) wbazant   (1001)     7715 2021-10-01 18:27:42.000000 marker_alignments-0.4.1/src/marker_alignments/mcl.py
--rw-rw-r--   0 wbazant   (1001) wbazant   (1001)    11327 2022-02-09 14:44:50.000000 marker_alignments-0.4.1/src/marker_alignments/store.py
--rw-rw-r--   0 wbazant   (1001) wbazant   (1001)     2262 2021-10-26 13:56:17.000000 marker_alignments-0.4.1/src/marker_alignments/pysam2.py
--rw-rw-r--   0 wbazant   (1001) wbazant   (1001)     6122 2022-02-09 15:07:56.000000 marker_alignments-0.4.1/src/marker_alignments/write.py
--rw-rw-r--   0 wbazant   (1001) wbazant   (1001)     1078 2021-09-29 11:24:03.000000 marker_alignments-0.4.1/src/marker_alignments/refdb_pattern.py
--rw-rw-r--   0 wbazant   (1001) wbazant   (1001)    10865 2022-04-01 12:35:58.000000 marker_alignments-0.4.1/src/marker_alignments/main.py
+drwxrwxr-x   0 wbazant   (1001) wbazant   (1001)        0 2023-07-01 15:54:11.939890 marker_alignments-0.4.2/
+-rw-r--r--   0 wbazant   (1001) wbazant   (1001)     1093 2022-04-01 11:39:35.000000 marker_alignments-0.4.2/LICENSE
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)    11354 2023-07-01 15:54:11.939890 marker_alignments-0.4.2/PKG-INFO
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)    10970 2023-07-01 15:50:08.000000 marker_alignments-0.4.2/README.md
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)       85 2022-04-01 11:38:56.000000 marker_alignments-0.4.2/pyproject.toml
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)       38 2023-07-01 15:54:11.939890 marker_alignments-0.4.2/setup.cfg
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)      851 2023-07-01 15:50:08.000000 marker_alignments-0.4.2/setup.py
+drwxrwxr-x   0 wbazant   (1001) wbazant   (1001)        0 2023-07-01 15:54:11.935890 marker_alignments-0.4.2/src/
+drwxrwxr-x   0 wbazant   (1001) wbazant   (1001)        0 2023-07-01 15:54:11.939890 marker_alignments-0.4.2/src/marker_alignments/
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)        0 2021-09-13 10:01:05.000000 marker_alignments-0.4.2/src/marker_alignments/__init__.py
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)    10865 2022-07-11 10:04:31.000000 marker_alignments-0.4.2/src/marker_alignments/main.py
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)     7715 2021-10-01 18:27:42.000000 marker_alignments-0.4.2/src/marker_alignments/mcl.py
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)     2262 2021-10-26 13:56:17.000000 marker_alignments-0.4.2/src/marker_alignments/pysam2.py
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)     1078 2021-09-29 11:24:03.000000 marker_alignments-0.4.2/src/marker_alignments/refdb_pattern.py
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)    11327 2022-02-09 14:44:50.000000 marker_alignments-0.4.2/src/marker_alignments/store.py
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)     6122 2022-02-09 15:07:56.000000 marker_alignments-0.4.2/src/marker_alignments/write.py
+drwxrwxr-x   0 wbazant   (1001) wbazant   (1001)        0 2023-07-01 15:54:11.939890 marker_alignments-0.4.2/src/marker_alignments.egg-info/
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)    11354 2023-07-01 15:54:11.000000 marker_alignments-0.4.2/src/marker_alignments.egg-info/PKG-INFO
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)      731 2023-07-01 15:54:11.000000 marker_alignments-0.4.2/src/marker_alignments.egg-info/SOURCES.txt
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)        1 2023-07-01 15:54:11.000000 marker_alignments-0.4.2/src/marker_alignments.egg-info/dependency_links.txt
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)       66 2023-07-01 15:54:11.000000 marker_alignments-0.4.2/src/marker_alignments.egg-info/entry_points.txt
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)       31 2023-07-01 15:54:11.000000 marker_alignments-0.4.2/src/marker_alignments.egg-info/requires.txt
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)       18 2023-07-01 15:54:11.000000 marker_alignments-0.4.2/src/marker_alignments.egg-info/top_level.txt
+drwxrwxr-x   0 wbazant   (1001) wbazant   (1001)        0 2023-07-01 15:54:11.939890 marker_alignments-0.4.2/tests/
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)      869 2022-04-01 11:54:16.000000 marker_alignments-0.4.2/tests/test_mcl.py
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)     1875 2021-12-02 16:50:08.000000 marker_alignments-0.4.2/tests/test_parse_args.py
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)     2225 2021-12-02 16:48:37.000000 marker_alignments-0.4.2/tests/test_read_alignments.py
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)     2456 2021-09-13 10:01:05.000000 marker_alignments-0.4.2/tests/test_refdb_pattern.py
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)     9311 2022-04-01 12:25:16.000000 marker_alignments-0.4.2/tests/test_store_counting.py
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)     3683 2022-02-09 14:44:38.000000 marker_alignments-0.4.2/tests/test_store_filter.py
+-rw-rw-r--   0 wbazant   (1001) wbazant   (1001)     4050 2021-10-04 11:06:46.000000 marker_alignments-0.4.2/tests/test_store_transform_taxa.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `marker_alignments-0.4.1/README.md` & `marker_alignments-0.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,59 @@
+Metadata-Version: 2.1
+Name: marker_alignments
+Version: 0.4.2
+Summary: Process and summarise alignments of metagenomic sequencing reads to reference databases of marker genes
+Home-page: http://github.com/wbazant/marker_alignments
+Author: wbazant
+Author-email: wojciech.bazant@gmail.com
+License: MIT
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # marker alignments
 This a Python package to process and summarise alignments of metagenomic sequencing reads to a reference database of marker genes. You can use it in conjunction with an aligner like `bowtie2` to produce an estimate of taxa present in a metagenomic sample.
 
-The package was developed in the context of looking for eukaryotes - most of the facilities are for producing good guesses from small amounts of potentially unreliable information. There are read level filters, clustering facilities for making sense of multiple alignments per query, and a number of thresholds.
+Features:
+- filtering reads on alignment properties
+- summarizing by marker and taxon
+- clustering based on multiple alignments per query
+- quantification
+
 
-## Installation
+## Usage
 
-To install via pip:
+### Installation
+
+Install via pip:
 ```
 pip install marker_alignments
 ```
 
-## Usage
-
-### Introduction
+### Getting started
 
 Download a small example alignment file, and run `marker_alignments` with most basic options:
 
 ```
 wget "https://raw.githubusercontent.com/wbazant/marker_alignments/main/tests/data/example.sam"
 
 marker_alignments --input example.sam --output /dev/stdout
 ```
 
-If the package installed correctly, you should see a coverage report for each reference in the alignments file. `marker_alignments --help` should show you all filtering options.
+If the package installed correctly, you should see a coverage report for each reference in the alignments file. Try it with your input file next, and take it from there: `marker_alignments --help` will show you all options about filtering and output types.
+
+### Is this suitable for my data?
+
+This package is for analysing metagenomic reads from whole genome sequencing, aligned to a reference of your choice.
 
+An allowed input is an alignment file in `.sam` or `.bam` format, coming from `bowtie2` or similar enough: @SQ lines on top, reads and MD tags in the output. See [example .sam](https://raw.githubusercontent.com/wbazant/marker_alignments/main/tests/data/example.sam) here.
 
-### Detecting eukaryotes
+The package was developed in the context of looking for eukaryotes using marker genes - see [CORRAL](github.com/wbazant/CORRAL) for a packaged workflow. It can also be useful for analysing aligned bacterial reads, e.g. to get quantification outputs.
+
+## Example - detecting eukaryotes
 
 First download the EukDetect reference database following [EukDetect installation instructions](https://github.com/allind/EukDetect).
 
 Then follow this example to download an example metagenomic file, run alignments to a reference database bundled with EukDetect, and obtain a profile using suitable filtering options:
 
 ```
 REFDB_LOCATION="eukdb"
@@ -53,28 +77,21 @@
   --refdb-format eukprot \
   --refdb-marker-to-taxon-path $REFDB_LOCATION/busco_taxid_link.txt \
   --output-type taxon_all \
   --num-reads $(grep -c '^@' $FASTQ_1) \
   $FILTERING_OPTS
 ```
 
-To do this for multiple samples, try the Nextflow pipeline [wbazant/CORRAL](https://github.com/wbazant/CORRAL).
-
-
-### Other uses
-The basic workflow type supported by this package is to give it an alignment file, and look at reports produced. 
-
-There are multiple filtering options aiming to reduce noise enough that the resulting taxonomic profile can be passed on to other tools. Alternatively, you can specify `--output-type pairs_of_taxa_shared_queries` or `output-type taxa_in_marker_clusters` and look at shared alignments between the queries, and get a detailed view of what the sequences in your metagenomic sample are most similar to.
-
-This is research software, and its usefulness apart from its original context of detecting eukaryotes is not yet known :). Reference sequences are grouped by taxon, so its use with another reference database requires the provision of options `--refdb-format` or `--refdb-marker-to-taxon-path`. 
-
-
 ## Filtering options
 
-Recommended presets are:
+### Bacteria
+Recommended setting for bacteria is: `--min-read-query-length 60 --min-taxon-num-reads 100` - only use alignments of length at least 60, report organisms with at least a hundred aligned reads.
+
+### Eukaryotes
+Recommended presets for eukaryotes are:
 
 `" --min-read-mapq 30 --min-read-query-length 60 --min-read-match-identity 0.9 --min-taxon-num-markers 2"`
 if using single best alignment per query.
 
 
 If using multiple alignments, the following preset recommended if you're okay with relying on MCL clusters:
 ` --min-read-query-length 60 --min-taxon-num-markers 2 --min-taxon-num-reads 2 --min-taxon-better-marker-cluster-averages-ratio 1.01 --threshold-avg-match-identity-to-call-known-taxon 0.97  --threshold-num-taxa-to-call-unknown-taxon 1 --threshold-num-markers-to-call-unknown-taxon 4     --threshold-num-reads-to-call-unknown-taxon 8`
@@ -108,35 +125,38 @@
 An unknown species will match as a mixture of results. The clustering option `--min-taxon-better-marker-cluster-averages-ratio` tries to take care of removing the overall inferior evidence, and the `--threshold-avg-match-identity-to-call-known-taxon` only passes
 
 The suggested value of 0.97 has been chosen empirically. Is a bit lower than CCMetagen's 0.9841 quoted from [Vu et al (2019)](https://pubmed.ncbi.nlm.nih.gov/29955203/), as this number was calculated from ribosomal subunits, we're not aware of a study that calculates average identity for BUSCOs. Most unknown taxa seem to match at around 0.9 identity, and a value 0.95 still permitted an unknown <i>Penicillinum</i> species to appear as a mixture.
 
 3. Threshold of evidence for making claims
 Claiming a eukaryote is present based on one read would be preposterous! It's not clear how many reads are "enough" to make a claim, and actually, no number of reads is enough because off-target matches follow patterns. We suggest gaining evidence from at least two markers, and a higher standard for ambiguous hits coming from species not in the reference. You can also only report unknown species if the results indicate its two nearest taxa with `--threshold-num-taxa-to-call-unknown-taxon` option.
 
+## Outputs
 
-### Other info
+### Output types
+The default option is coverage To get most outputs, set `--output_type taxon_all` for aggregated outputs, or `--output_type marker_all` for the breakdown. See `marker_alignments --help` for other available options.
 
-#### More output options
-You can save an intermediate database produced by providing the `--sqlite-db-path` argument, and then query it with a `sqlite3` client.
+### Quantification
 
-#### Custom or different reference database
-The default `--refdb-format` is `generic`, which tries to produce nice names, but may or may not match how you want it to. Set `--refdb-format` to `no-split` if you don't want the nice names, and if you want the taxa to be recognised really correctly, list a lookup table under `--refdb-marker-to-taxon-path`.
+**Coverage per marker**
+= number of reads aligned to the marker times read length divided by length of a marker
 
-## Known issues
-Quantitative information might be unreliable when there is very few reads.
+**Coverage per taxon**
+= average coverage between all markers with nonzero coverage
 
+**CPM (copies per million)** 
+= taxon coverage divided by total number of reads and multiplied by one million
 
+CPMs are the most useful number for comparing between different taxa and across samples, since they correct for different sequencing depth between samples, and different reference length between taxa.
 
-For a large enough file, the sqlite query engine runs out of page numbers when doing a `group by`. In [my fork of HuMAnN with similar query code](https://github.com/wbazant/humann/commit/1dc767f855) I have solved this by adding `'PRAGMA max_page_count = 4294967292;'` before the `group by`. I've not yet ran into this issue when using this package.
+Please note that quantitative information might be unreliable when there is very few reads.
 
-## Credits
-I took the method of splitting multiple aligned reads by a weighted average (with the second power of match identity as weights), and the method of calculating CPMs, from HuMAnN.
-I was inspired by how MetaPhlAn calculates taxon CPMs from marker CPMs, although they have more options and I just ported the simple one.
-I copied the package setup from EukDetect, and developed the package mostly in the context of alignments to the EukDetect reference.
-An idea for what outputs might be useful to users comes jointly from these three tools.
+## Custom use
 
-For inspiration of what read properties are worth filtering on and how to do it, some credit goes to [TALON's `transcript_utils` file](https://github.com/mortazavilab/TALON/blob/master/src/talon/transcript_utils.py).
+### Reference databases
+For each reference database, we need to know what taxon each contig or marker sequence is for. This can be provided externally, through a lookup table with the `--refdb-marker-to-taxon-path` option, but we also try support all reference databases of interest to our users through the --refdb-format option. If `--refdb-format generic` produces errors for you, please open a ticket with the details about the reference database and the raised error.
 
-## How to cite
+### Additional output options
+You can save an intermediate database produced by providing the `--sqlite-db-path` argument, and then query it with a `sqlite3` client.
 
-We now have a preprint on biorxiv: https://doi.org/10.1101/2022.03.09.483664 .
+## How to cite
+Please cite our Microbiome publication, https://doi.org/10.1186/s40168-023-01505-1 .
```

### Comparing `marker_alignments-0.4.1/PKG-INFO` & `marker_alignments-0.4.2/src/marker_alignments.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,59 @@
 Metadata-Version: 2.1
-Name: marker_alignments
-Version: 0.4.1
+Name: marker-alignments
+Version: 0.4.2
 Summary: Process and summarise alignments of metagenomic sequencing reads to reference databases of marker genes
 Home-page: http://github.com/wbazant/marker_alignments
 Author: wbazant
 Author-email: wojciech.bazant@gmail.com
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # marker alignments
 This a Python package to process and summarise alignments of metagenomic sequencing reads to a reference database of marker genes. You can use it in conjunction with an aligner like `bowtie2` to produce an estimate of taxa present in a metagenomic sample.
 
-The package was developed in the context of looking for eukaryotes - most of the facilities are for producing good guesses from small amounts of potentially unreliable information. There are read level filters, clustering facilities for making sense of multiple alignments per query, and a number of thresholds.
+Features:
+- filtering reads on alignment properties
+- summarizing by marker and taxon
+- clustering based on multiple alignments per query
+- quantification
 
-## Installation
 
-To install via pip:
+## Usage
+
+### Installation
+
+Install via pip:
 ```
 pip install marker_alignments
 ```
 
-## Usage
-
-### Introduction
+### Getting started
 
 Download a small example alignment file, and run `marker_alignments` with most basic options:
 
 ```
 wget "https://raw.githubusercontent.com/wbazant/marker_alignments/main/tests/data/example.sam"
 
 marker_alignments --input example.sam --output /dev/stdout
 ```
 
-If the package installed correctly, you should see a coverage report for each reference in the alignments file. `marker_alignments --help` should show you all filtering options.
+If the package installed correctly, you should see a coverage report for each reference in the alignments file. Try it with your input file next, and take it from there: `marker_alignments --help` will show you all options about filtering and output types.
+
+### Is this suitable for my data?
 
+This package is for analysing metagenomic reads from whole genome sequencing, aligned to a reference of your choice.
 
-### Detecting eukaryotes
+An allowed input is an alignment file in `.sam` or `.bam` format, coming from `bowtie2` or similar enough: @SQ lines on top, reads and MD tags in the output. See [example .sam](https://raw.githubusercontent.com/wbazant/marker_alignments/main/tests/data/example.sam) here.
+
+The package was developed in the context of looking for eukaryotes using marker genes - see [CORRAL](github.com/wbazant/CORRAL) for a packaged workflow. It can also be useful for analysing aligned bacterial reads, e.g. to get quantification outputs.
+
+## Example - detecting eukaryotes
 
 First download the EukDetect reference database following [EukDetect installation instructions](https://github.com/allind/EukDetect).
 
 Then follow this example to download an example metagenomic file, run alignments to a reference database bundled with EukDetect, and obtain a profile using suitable filtering options:
 
 ```
 REFDB_LOCATION="eukdb"
@@ -66,28 +77,21 @@
   --refdb-format eukprot \
   --refdb-marker-to-taxon-path $REFDB_LOCATION/busco_taxid_link.txt \
   --output-type taxon_all \
   --num-reads $(grep -c '^@' $FASTQ_1) \
   $FILTERING_OPTS
 ```
 
-To do this for multiple samples, try the Nextflow pipeline [wbazant/CORRAL](https://github.com/wbazant/CORRAL).
-
-
-### Other uses
-The basic workflow type supported by this package is to give it an alignment file, and look at reports produced. 
-
-There are multiple filtering options aiming to reduce noise enough that the resulting taxonomic profile can be passed on to other tools. Alternatively, you can specify `--output-type pairs_of_taxa_shared_queries` or `output-type taxa_in_marker_clusters` and look at shared alignments between the queries, and get a detailed view of what the sequences in your metagenomic sample are most similar to.
-
-This is research software, and its usefulness apart from its original context of detecting eukaryotes is not yet known :). Reference sequences are grouped by taxon, so its use with another reference database requires the provision of options `--refdb-format` or `--refdb-marker-to-taxon-path`. 
-
-
 ## Filtering options
 
-Recommended presets are:
+### Bacteria
+Recommended setting for bacteria is: `--min-read-query-length 60 --min-taxon-num-reads 100` - only use alignments of length at least 60, report organisms with at least a hundred aligned reads.
+
+### Eukaryotes
+Recommended presets for eukaryotes are:
 
 `" --min-read-mapq 30 --min-read-query-length 60 --min-read-match-identity 0.9 --min-taxon-num-markers 2"`
 if using single best alignment per query.
 
 
 If using multiple alignments, the following preset recommended if you're okay with relying on MCL clusters:
 ` --min-read-query-length 60 --min-taxon-num-markers 2 --min-taxon-num-reads 2 --min-taxon-better-marker-cluster-averages-ratio 1.01 --threshold-avg-match-identity-to-call-known-taxon 0.97  --threshold-num-taxa-to-call-unknown-taxon 1 --threshold-num-markers-to-call-unknown-taxon 4     --threshold-num-reads-to-call-unknown-taxon 8`
@@ -121,37 +125,38 @@
 An unknown species will match as a mixture of results. The clustering option `--min-taxon-better-marker-cluster-averages-ratio` tries to take care of removing the overall inferior evidence, and the `--threshold-avg-match-identity-to-call-known-taxon` only passes
 
 The suggested value of 0.97 has been chosen empirically. Is a bit lower than CCMetagen's 0.9841 quoted from [Vu et al (2019)](https://pubmed.ncbi.nlm.nih.gov/29955203/), as this number was calculated from ribosomal subunits, we're not aware of a study that calculates average identity for BUSCOs. Most unknown taxa seem to match at around 0.9 identity, and a value 0.95 still permitted an unknown <i>Penicillinum</i> species to appear as a mixture.
 
 3. Threshold of evidence for making claims
 Claiming a eukaryote is present based on one read would be preposterous! It's not clear how many reads are "enough" to make a claim, and actually, no number of reads is enough because off-target matches follow patterns. We suggest gaining evidence from at least two markers, and a higher standard for ambiguous hits coming from species not in the reference. You can also only report unknown species if the results indicate its two nearest taxa with `--threshold-num-taxa-to-call-unknown-taxon` option.
 
+## Outputs
 
-### Other info
-
-#### More output options
-You can save an intermediate database produced by providing the `--sqlite-db-path` argument, and then query it with a `sqlite3` client.
-
-#### Custom or different reference database
-The default `--refdb-format` is `generic`, which tries to produce nice names, but may or may not match how you want it to. Set `--refdb-format` to `no-split` if you don't want the nice names, and if you want the taxa to be recognised really correctly, list a lookup table under `--refdb-marker-to-taxon-path`.
+### Output types
+The default option is coverage To get most outputs, set `--output_type taxon_all` for aggregated outputs, or `--output_type marker_all` for the breakdown. See `marker_alignments --help` for other available options.
 
-## Known issues
-Quantitative information might be unreliable when there is very few reads.
+### Quantification
 
+**Coverage per marker**
+= number of reads aligned to the marker times read length divided by length of a marker
 
+**Coverage per taxon**
+= average coverage between all markers with nonzero coverage
 
-For a large enough file, the sqlite query engine runs out of page numbers when doing a `group by`. In [my fork of HuMAnN with similar query code](https://github.com/wbazant/humann/commit/1dc767f855) I have solved this by adding `'PRAGMA max_page_count = 4294967292;'` before the `group by`. I've not yet ran into this issue when using this package.
+**CPM (copies per million)** 
+= taxon coverage divided by total number of reads and multiplied by one million
 
-## Credits
-I took the method of splitting multiple aligned reads by a weighted average (with the second power of match identity as weights), and the method of calculating CPMs, from HuMAnN.
-I was inspired by how MetaPhlAn calculates taxon CPMs from marker CPMs, although they have more options and I just ported the simple one.
-I copied the package setup from EukDetect, and developed the package mostly in the context of alignments to the EukDetect reference.
-An idea for what outputs might be useful to users comes jointly from these three tools.
+CPMs are the most useful number for comparing between different taxa and across samples, since they correct for different sequencing depth between samples, and different reference length between taxa.
 
-For inspiration of what read properties are worth filtering on and how to do it, some credit goes to [TALON's `transcript_utils` file](https://github.com/mortazavilab/TALON/blob/master/src/talon/transcript_utils.py).
+Please note that quantitative information might be unreliable when there is very few reads.
 
-## How to cite
+## Custom use
 
-We now have a preprint on biorxiv: https://doi.org/10.1101/2022.03.09.483664 .
+### Reference databases
+For each reference database, we need to know what taxon each contig or marker sequence is for. This can be provided externally, through a lookup table with the `--refdb-marker-to-taxon-path` option, but we also try support all reference databases of interest to our users through the --refdb-format option. If `--refdb-format generic` produces errors for you, please open a ticket with the details about the reference database and the raised error.
 
+### Additional output options
+You can save an intermediate database produced by providing the `--sqlite-db-path` argument, and then query it with a `sqlite3` client.
 
+## How to cite
+Please cite our Microbiome publication, https://doi.org/10.1186/s40168-023-01505-1 .
```

### Comparing `marker_alignments-0.4.1/LICENSE` & `marker_alignments-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `marker_alignments-0.4.1/setup.py` & `marker_alignments-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(name='marker_alignments',
-    version='0.4.1',
+    version='0.4.2',
     description="Process and summarise alignments of metagenomic sequencing reads to reference databases of marker genes",
     long_description = long_description,
     long_description_content_type="text/markdown",
     url='http://github.com/wbazant/marker_alignments',
     author='wbazant',
     author_email='wojciech.bazant@gmail.com',
     license="MIT",
     entry_points={"console_scripts": [
         "marker_alignments = marker_alignments.main:main",
     ]},
-    install_requires=["pysam", "scipy", "numpy", "sklearn"],
+    install_requires=["pysam", "scipy", "numpy", "scikit-learn"],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
 )
```

### Comparing `marker_alignments-0.4.1/src/marker_alignments.egg-info/PKG-INFO` & `marker_alignments-0.4.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,47 @@
-Metadata-Version: 2.1
-Name: marker-alignments
-Version: 0.4.1
-Summary: Process and summarise alignments of metagenomic sequencing reads to reference databases of marker genes
-Home-page: http://github.com/wbazant/marker_alignments
-Author: wbazant
-Author-email: wojciech.bazant@gmail.com
-License: MIT
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # marker alignments
 This a Python package to process and summarise alignments of metagenomic sequencing reads to a reference database of marker genes. You can use it in conjunction with an aligner like `bowtie2` to produce an estimate of taxa present in a metagenomic sample.
 
-The package was developed in the context of looking for eukaryotes - most of the facilities are for producing good guesses from small amounts of potentially unreliable information. There are read level filters, clustering facilities for making sense of multiple alignments per query, and a number of thresholds.
+Features:
+- filtering reads on alignment properties
+- summarizing by marker and taxon
+- clustering based on multiple alignments per query
+- quantification
+
+
+## Usage
 
-## Installation
+### Installation
 
-To install via pip:
+Install via pip:
 ```
 pip install marker_alignments
 ```
 
-## Usage
-
-### Introduction
+### Getting started
 
 Download a small example alignment file, and run `marker_alignments` with most basic options:
 
 ```
 wget "https://raw.githubusercontent.com/wbazant/marker_alignments/main/tests/data/example.sam"
 
 marker_alignments --input example.sam --output /dev/stdout
 ```
 
-If the package installed correctly, you should see a coverage report for each reference in the alignments file. `marker_alignments --help` should show you all filtering options.
+If the package installed correctly, you should see a coverage report for each reference in the alignments file. Try it with your input file next, and take it from there: `marker_alignments --help` will show you all options about filtering and output types.
 
+### Is this suitable for my data?
 
-### Detecting eukaryotes
+This package is for analysing metagenomic reads from whole genome sequencing, aligned to a reference of your choice.
+
+An allowed input is an alignment file in `.sam` or `.bam` format, coming from `bowtie2` or similar enough: @SQ lines on top, reads and MD tags in the output. See [example .sam](https://raw.githubusercontent.com/wbazant/marker_alignments/main/tests/data/example.sam) here.
+
+The package was developed in the context of looking for eukaryotes using marker genes - see [CORRAL](github.com/wbazant/CORRAL) for a packaged workflow. It can also be useful for analysing aligned bacterial reads, e.g. to get quantification outputs.
+
+## Example - detecting eukaryotes
 
 First download the EukDetect reference database following [EukDetect installation instructions](https://github.com/allind/EukDetect).
 
 Then follow this example to download an example metagenomic file, run alignments to a reference database bundled with EukDetect, and obtain a profile using suitable filtering options:
 
 ```
 REFDB_LOCATION="eukdb"
@@ -66,28 +65,21 @@
   --refdb-format eukprot \
   --refdb-marker-to-taxon-path $REFDB_LOCATION/busco_taxid_link.txt \
   --output-type taxon_all \
   --num-reads $(grep -c '^@' $FASTQ_1) \
   $FILTERING_OPTS
 ```
 
-To do this for multiple samples, try the Nextflow pipeline [wbazant/CORRAL](https://github.com/wbazant/CORRAL).
-
-
-### Other uses
-The basic workflow type supported by this package is to give it an alignment file, and look at reports produced. 
-
-There are multiple filtering options aiming to reduce noise enough that the resulting taxonomic profile can be passed on to other tools. Alternatively, you can specify `--output-type pairs_of_taxa_shared_queries` or `output-type taxa_in_marker_clusters` and look at shared alignments between the queries, and get a detailed view of what the sequences in your metagenomic sample are most similar to.
-
-This is research software, and its usefulness apart from its original context of detecting eukaryotes is not yet known :). Reference sequences are grouped by taxon, so its use with another reference database requires the provision of options `--refdb-format` or `--refdb-marker-to-taxon-path`. 
-
-
 ## Filtering options
 
-Recommended presets are:
+### Bacteria
+Recommended setting for bacteria is: `--min-read-query-length 60 --min-taxon-num-reads 100` - only use alignments of length at least 60, report organisms with at least a hundred aligned reads.
+
+### Eukaryotes
+Recommended presets for eukaryotes are:
 
 `" --min-read-mapq 30 --min-read-query-length 60 --min-read-match-identity 0.9 --min-taxon-num-markers 2"`
 if using single best alignment per query.
 
 
 If using multiple alignments, the following preset recommended if you're okay with relying on MCL clusters:
 ` --min-read-query-length 60 --min-taxon-num-markers 2 --min-taxon-num-reads 2 --min-taxon-better-marker-cluster-averages-ratio 1.01 --threshold-avg-match-identity-to-call-known-taxon 0.97  --threshold-num-taxa-to-call-unknown-taxon 1 --threshold-num-markers-to-call-unknown-taxon 4     --threshold-num-reads-to-call-unknown-taxon 8`
@@ -121,37 +113,38 @@
 An unknown species will match as a mixture of results. The clustering option `--min-taxon-better-marker-cluster-averages-ratio` tries to take care of removing the overall inferior evidence, and the `--threshold-avg-match-identity-to-call-known-taxon` only passes
 
 The suggested value of 0.97 has been chosen empirically. Is a bit lower than CCMetagen's 0.9841 quoted from [Vu et al (2019)](https://pubmed.ncbi.nlm.nih.gov/29955203/), as this number was calculated from ribosomal subunits, we're not aware of a study that calculates average identity for BUSCOs. Most unknown taxa seem to match at around 0.9 identity, and a value 0.95 still permitted an unknown <i>Penicillinum</i> species to appear as a mixture.
 
 3. Threshold of evidence for making claims
 Claiming a eukaryote is present based on one read would be preposterous! It's not clear how many reads are "enough" to make a claim, and actually, no number of reads is enough because off-target matches follow patterns. We suggest gaining evidence from at least two markers, and a higher standard for ambiguous hits coming from species not in the reference. You can also only report unknown species if the results indicate its two nearest taxa with `--threshold-num-taxa-to-call-unknown-taxon` option.
 
+## Outputs
 
-### Other info
+### Output types
+The default option is coverage To get most outputs, set `--output_type taxon_all` for aggregated outputs, or `--output_type marker_all` for the breakdown. See `marker_alignments --help` for other available options.
 
-#### More output options
-You can save an intermediate database produced by providing the `--sqlite-db-path` argument, and then query it with a `sqlite3` client.
+### Quantification
 
-#### Custom or different reference database
-The default `--refdb-format` is `generic`, which tries to produce nice names, but may or may not match how you want it to. Set `--refdb-format` to `no-split` if you don't want the nice names, and if you want the taxa to be recognised really correctly, list a lookup table under `--refdb-marker-to-taxon-path`.
+**Coverage per marker**
+= number of reads aligned to the marker times read length divided by length of a marker
 
-## Known issues
-Quantitative information might be unreliable when there is very few reads.
+**Coverage per taxon**
+= average coverage between all markers with nonzero coverage
 
+**CPM (copies per million)** 
+= taxon coverage divided by total number of reads and multiplied by one million
 
+CPMs are the most useful number for comparing between different taxa and across samples, since they correct for different sequencing depth between samples, and different reference length between taxa.
 
-For a large enough file, the sqlite query engine runs out of page numbers when doing a `group by`. In [my fork of HuMAnN with similar query code](https://github.com/wbazant/humann/commit/1dc767f855) I have solved this by adding `'PRAGMA max_page_count = 4294967292;'` before the `group by`. I've not yet ran into this issue when using this package.
+Please note that quantitative information might be unreliable when there is very few reads.
 
-## Credits
-I took the method of splitting multiple aligned reads by a weighted average (with the second power of match identity as weights), and the method of calculating CPMs, from HuMAnN.
-I was inspired by how MetaPhlAn calculates taxon CPMs from marker CPMs, although they have more options and I just ported the simple one.
-I copied the package setup from EukDetect, and developed the package mostly in the context of alignments to the EukDetect reference.
-An idea for what outputs might be useful to users comes jointly from these three tools.
+## Custom use
 
-For inspiration of what read properties are worth filtering on and how to do it, some credit goes to [TALON's `transcript_utils` file](https://github.com/mortazavilab/TALON/blob/master/src/talon/transcript_utils.py).
-
-## How to cite
-
-We now have a preprint on biorxiv: https://doi.org/10.1101/2022.03.09.483664 .
+### Reference databases
+For each reference database, we need to know what taxon each contig or marker sequence is for. This can be provided externally, through a lookup table with the `--refdb-marker-to-taxon-path` option, but we also try support all reference databases of interest to our users through the --refdb-format option. If `--refdb-format generic` produces errors for you, please open a ticket with the details about the reference database and the raised error.
 
+### Additional output options
+You can save an intermediate database produced by providing the `--sqlite-db-path` argument, and then query it with a `sqlite3` client.
 
+## How to cite
+Please cite our Microbiome publication, https://doi.org/10.1186/s40168-023-01505-1 .
```

### Comparing `marker_alignments-0.4.1/src/marker_alignments/mcl.py` & `marker_alignments-0.4.2/src/marker_alignments/mcl.py`

 * *Files identical despite different names*

### Comparing `marker_alignments-0.4.1/src/marker_alignments/store.py` & `marker_alignments-0.4.2/src/marker_alignments/store.py`

 * *Files identical despite different names*

### Comparing `marker_alignments-0.4.1/src/marker_alignments/pysam2.py` & `marker_alignments-0.4.2/src/marker_alignments/pysam2.py`

 * *Files identical despite different names*

### Comparing `marker_alignments-0.4.1/src/marker_alignments/write.py` & `marker_alignments-0.4.2/src/marker_alignments/write.py`

 * *Files identical despite different names*

### Comparing `marker_alignments-0.4.1/src/marker_alignments/refdb_pattern.py` & `marker_alignments-0.4.2/src/marker_alignments/refdb_pattern.py`

 * *Files identical despite different names*

### Comparing `marker_alignments-0.4.1/src/marker_alignments/main.py` & `marker_alignments-0.4.2/src/marker_alignments/main.py`

 * *Files identical despite different names*

