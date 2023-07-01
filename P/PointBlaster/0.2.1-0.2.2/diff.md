# Comparing `tmp/PointBlaster-0.2.1.tar.gz` & `tmp/PointBlaster-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PointBlaster-0.2.1.tar", last modified: Thu Jun 29 01:14:30 2023, max compression
+gzip compressed data, was "PointBlaster-0.2.2.tar", last modified: Sat Jul  1 09:53:04 2023, max compression
```

## Comparing `PointBlaster-0.2.1.tar` & `PointBlaster-0.2.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-29 01:14:30.555086 PointBlaster-0.2.1/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-27 16:38:24.000000 PointBlaster-0.2.1/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       61 2023-06-25 06:30:58.000000 PointBlaster-0.2.1/MANIFEST.in
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-29 01:14:30.554953 PointBlaster-0.2.1/PKG-INFO
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-29 01:14:30.535051 PointBlaster-0.2.1/PointBlaster/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-26 05:00:54.000000 PointBlaster-0.2.1/PointBlaster/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    25720 2023-06-28 08:20:45.000000 PointBlaster-0.2.1/PointBlaster/PointBlaster.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      303 2023-06-28 08:20:52.000000 PointBlaster-0.2.1/PointBlaster/__init__.py
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-29 01:14:30.535922 PointBlaster-0.2.1/PointBlaster/db/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-26 05:00:54.000000 PointBlaster-0.2.1/PointBlaster/db/.DS_Store
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-29 01:14:30.537622 PointBlaster-0.2.1/PointBlaster/db/point_mutation/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    10244 2023-06-26 05:03:42.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/.DS_Store
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-29 01:14:30.544080 PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:10:09.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2972 2023-06-19 06:40:55.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/23S.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        4 2023-06-19 06:40:55.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/RNA_genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)  4259822 2023-06-19 06:54:12.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     8705 2023-06-25 07:08:32.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     8657 2023-06-19 06:40:55.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:54:12.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/campylobacter.length.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      149 2023-06-19 06:54:12.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/campylobacter.name
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4936 2023-06-19 06:54:12.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       14 2023-06-19 06:40:55.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     5272 2023-06-19 06:40:55.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2613 2023-06-19 06:40:55.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2523 2023-06-19 06:40:55.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1961 2023-06-19 06:40:55.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      412 2023-06-19 06:40:55.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/rpsL.fsa
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-29 01:14:30.551609 PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1593 2023-06-19 06:40:55.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2023-06-19 06:40:55.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/RNA_genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     3214 2023-06-19 06:40:55.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/acrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:40:55.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2694 2023-06-19 06:40:55.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/gyrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2469 2023-06-19 06:40:55.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/gyrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2311 2023-06-19 06:40:55.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/parC.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1940 2023-06-19 06:40:55.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/parE.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     7137 2023-06-19 06:40:55.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/phenotypes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      698 2023-06-19 06:40:55.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/pmrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1106 2023-06-19 06:40:55.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/pmrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     5026 2023-06-25 07:13:32.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)  4318510 2023-06-19 06:54:12.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    16121 2023-06-25 07:08:53.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/salmonella.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    16025 2023-06-19 06:40:55.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       72 2023-06-19 06:54:12.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/salmonella.length.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      296 2023-06-19 06:54:12.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/salmonella.name
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     7888 2023-06-19 06:54:12.000000 PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-29 01:14:30.535769 PointBlaster-0.2.1/PointBlaster.egg-info/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-29 01:14:30.000000 PointBlaster-0.2.1/PointBlaster.egg-info/PKG-INFO
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2350 2023-06-29 01:14:30.000000 PointBlaster-0.2.1/PointBlaster.egg-info/SOURCES.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2023-06-29 01:14:30.000000 PointBlaster-0.2.1/PointBlaster.egg-info/dependency_links.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       65 2023-06-29 01:14:30.000000 PointBlaster-0.2.1/PointBlaster.egg-info/entry_points.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       39 2023-06-29 01:14:30.000000 PointBlaster-0.2.1/PointBlaster.egg-info/requires.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       13 2023-06-29 01:14:30.000000 PointBlaster-0.2.1/PointBlaster.egg-info/top_level.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1611 2023-06-25 06:11:36.000000 PointBlaster-0.2.1/README.md
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-29 01:14:30.553408 PointBlaster-0.2.1/dist/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-27 05:40:56.000000 PointBlaster-0.2.1/dist/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       57 2023-06-25 05:58:37.000000 PointBlaster-0.2.1/requirements.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2023-06-29 01:14:30.555125 PointBlaster-0.2.1/setup.cfg
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2162 2023-06-25 06:43:25.000000 PointBlaster-0.2.1/setup.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-01 09:53:04.727627 PointBlaster-0.2.2/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-07-01 09:04:52.000000 PointBlaster-0.2.2/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       61 2023-06-25 06:30:58.000000 PointBlaster-0.2.2/MANIFEST.in
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-07-01 09:53:04.727498 PointBlaster-0.2.2/PKG-INFO
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-01 09:53:04.706672 PointBlaster-0.2.2/PointBlaster/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-26 05:00:54.000000 PointBlaster-0.2.2/PointBlaster/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    26523 2023-07-01 09:51:37.000000 PointBlaster-0.2.2/PointBlaster/PointBlaster.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      303 2023-07-01 09:05:12.000000 PointBlaster-0.2.2/PointBlaster/__init__.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-01 09:53:04.707479 PointBlaster-0.2.2/PointBlaster/db/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-26 05:00:54.000000 PointBlaster-0.2.2/PointBlaster/db/.DS_Store
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-01 09:53:04.707796 PointBlaster-0.2.2/PointBlaster/db/point_mutation/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    10244 2023-06-26 05:03:42.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/.DS_Store
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-01 09:53:04.715642 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:10:09.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2972 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/23S.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        4 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/RNA_genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)  4259822 2023-06-19 06:54:12.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     8705 2023-06-25 07:08:32.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     8657 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:54:12.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.length.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      149 2023-06-19 06:54:12.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.name
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4936 2023-06-19 06:54:12.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       14 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     5272 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2613 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2523 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1961 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      412 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/rpsL.fsa
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-01 09:53:04.723445 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1593 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/RNA_genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     3214 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/acrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2694 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/gyrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2469 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/gyrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2311 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/parC.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1940 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/parE.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     7137 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/phenotypes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      698 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/pmrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1106 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/pmrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     5026 2023-06-25 07:13:32.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)  4318510 2023-06-19 06:54:12.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    16121 2023-06-25 07:08:53.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/salmonella.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    16025 2023-06-19 06:40:55.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       72 2023-06-19 06:54:12.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/salmonella.length.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      296 2023-06-19 06:54:12.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/salmonella.name
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     7888 2023-06-19 06:54:12.000000 PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-01 09:53:04.707369 PointBlaster-0.2.2/PointBlaster.egg-info/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-07-01 09:53:04.000000 PointBlaster-0.2.2/PointBlaster.egg-info/PKG-INFO
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2350 2023-07-01 09:53:04.000000 PointBlaster-0.2.2/PointBlaster.egg-info/SOURCES.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2023-07-01 09:53:04.000000 PointBlaster-0.2.2/PointBlaster.egg-info/dependency_links.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       65 2023-07-01 09:53:04.000000 PointBlaster-0.2.2/PointBlaster.egg-info/entry_points.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       39 2023-07-01 09:53:04.000000 PointBlaster-0.2.2/PointBlaster.egg-info/requires.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       13 2023-07-01 09:53:04.000000 PointBlaster-0.2.2/PointBlaster.egg-info/top_level.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1611 2023-06-25 06:11:36.000000 PointBlaster-0.2.2/README.md
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-01 09:53:04.725839 PointBlaster-0.2.2/dist/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-27 05:40:56.000000 PointBlaster-0.2.2/dist/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       57 2023-06-25 05:58:37.000000 PointBlaster-0.2.2/requirements.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2023-07-01 09:53:04.727667 PointBlaster-0.2.2/setup.cfg
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2162 2023-06-25 06:43:25.000000 PointBlaster-0.2.2/setup.py
```

### Comparing `PointBlaster-0.2.1/.DS_Store` & `PointBlaster-0.2.2/.DS_Store`

 * *Files 10% similar despite different names*

```diff
@@ -97,16 +97,16 @@
 00000600: 7062 6c6f 6200 0000 b862 706c 6973 7430  pblob....bplist0
 00000610: 30d6 0102 0304 0506 0708 0708 0b08 5d53  0.............]S
 00000620: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
 00000630: 7754 6f6f 6c62 6172 5b53 686f 7754 6162  wToolbar[ShowTab
 00000640: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
 00000650: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
 00000660: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
-00000670: 6562 6172 0809 0809 5f10 187b 7b32 3936  ebar...._..{{296
-00000680: 2c20 3339 337d 2c20 7b39 3230 2c20 3433  , 393}, {920, 43
+00000670: 6562 6172 0809 0809 5f10 187b 7b32 3937  ebar...._..{{297
+00000680: 2c20 3339 347d 2c20 7b39 3230 2c20 3433  , 394}, {920, 43
 00000690: 367d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  6}}...#/;R_klmno
 000006a0: 8a00 0000 0000 0001 0100 0000 0000 0000  ................
 000006b0: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
 000006c0: 8b00 0000 0c00 5000 6f00 6900 6e00 7400  ......P.o.i.n.t.
 000006d0: 4200 6c00 6100 7300 7400 6500 726c 6731  B.l.a.s.t.e.rlg1
 000006e0: 5363 6f6d 7000 0000 0000 0000 0000 0000  Scomp...........
 000006f0: 0c00 5000 6f00 6900 6e00 7400 4200 6c00  ..P.o.i.n.t.B.l.
```

### Comparing `PointBlaster-0.2.1/PKG-INFO` & `PointBlaster-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PointBlaster
-Version: 0.2.1
+Version: 0.2.2
 Summary: find point mutation in assembled genomes
 Home-page: https://github.com/hbucqp/PointBlaster
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,wgs,blastn,pointmutation
 Platform: any
```

### Comparing `PointBlaster-0.2.1/PointBlaster/.DS_Store` & `PointBlaster-0.2.2/PointBlaster/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/PointBlaster.py` & `PointBlaster-0.2.2/PointBlaster/PointBlaster.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,39 +120,58 @@
             new_sbjct_string = result_dict[item]['SBJCT_SEQ']
             new_query_string = result_dict[item]['QUERY_SEQ']
 
             # get reference sequence of gene
             raw_sbjct_seq = get_sbjct_seq(ref_fasta, gene)
             if new_sbjct_start < gene_list[gene][1]:
                 sbjct_start = new_sbjct_start
-                sbjct_string = raw_sbjct_seq[sbjct_start - 1:len(new_sbjct_string)] + raw_sbjct_seq[len(
-                    new_sbjct_string):gene_list[gene][1] - 1] + gene_list[gene][2]
-                query_string = new_query_string + \
-                    raw_sbjct_seq[len(new_sbjct_string)
-                                      :gene_list[gene][1] - 1] + gene_list[gene][3]
+                second_sbjct_start = gene_list[gene][1]
+                first_sbjct = new_sbjct_string
+                second_sbjct = gene_list[gene][2]
+                first_query = new_query_string
+                second_query = gene_list[gene][3]
             else:
                 sbjct_start = gene_list[gene][1]
-                sbjct_string = gene_list[gene][2] + raw_sbjct_seq[len(
-                    gene_list[gene][2]):new_sbjct_start - 1] + raw_sbjct_seq[sbjct_start - 1:len(new_sbjct_string)]
-                query_string = gene_list[gene][3] + raw_sbjct_seq[len(
-                    gene_list[gene][2]):new_sbjct_start - 1] + new_query_string
+                second_sbjct_start = new_sbjct_start
+                first_sbjct = gene_list[gene][2]
+                second_sbjct = new_sbjct_string
+                first_query = gene_list[gene][3]
+                second_query = new_query_string
+                # sbjct_string = raw_sbjct_seq[sbjct_start - 1:len(new_sbjct_string)] + raw_sbjct_seq[sbjct_start + len(
+                #     new_sbjct_string) - 1:gene_list[gene][1] - 1 ] + gene_list[gene][2]
+            if (sbjct_start + len(first_sbjct) - 1) <= second_sbjct_start:
+                sbjct_string = first_sbjct + raw_sbjct_seq[sbjct_start + len(
+                    first_sbjct) - 1:second_sbjct_start - 1] + second_sbjct
+                query_string = first_query + raw_sbjct_seq[sbjct_start + len(
+                    first_sbjct) - 1:second_sbjct_start - 1] + second_query
+            else:
+                sbjct_string = first_sbjct + second_sbjct[sbjct_start + len(
+                    first_sbjct) - 1:]
+                querey_string = first_query + second_query[sbjct_start + len(
+                    first_query) - 1:]
 
             identity = compute_identity(query_string, sbjct_string)
+            # print(gene)
             coverage = len(sbjct_string) * 100 / len(raw_sbjct_seq)
             # print(coverage)
 
             gene_list[gene] = (gene, sbjct_start, sbjct_string,
                                query_string, coverage, identity)
 
     return gene_list
 
 
 def compute_identity(query_string, sbjct_string):
     a = 1
-    for i in range(0, len(query_string) - 1):
+    # print(len(query_string))
+    # print(len(sbjct_string))
+    for i in range(0, len(query_string)):
+        # print(i)
+        # print(query_string[i])
+        # print(sbjct_string[i])
         # print(i)
         if query_string[i] == sbjct_string[i]:
             a += 1
     identity = a * 100 / len(sbjct_string)
     # print(identity)
     return identity
 
@@ -317,16 +336,16 @@
                         if sub_end_pos % 3 != 0:
                             ref_seq = sbjct_string[i - 1: i +
                                                    len(sub_seq) - 1 + (3 - (sub_end_pos % 3)) + 1]
 
                             query_seq = query_string[i - 1: i +
                                                      len(sub_seq) - 1 + (3 - (sub_end_pos % 3)) + 1]
                         else:
-                            ref_seq = sbjct_string[i - 1: i + len(seq)]
-                            query_seq = query_string[i - 1: i + len(seq)]
+                            ref_seq = sbjct_string[i - 1: i + len(sub_seq)]
+                            query_seq = query_string[i - 1: i + len(sub_seq)]
                 else:
                     ref_seq = sbjct_nuc
 
                     query_seq = query_nuc
 
                 # print(ref_seq, query_seq)
                 if len(sub_seq) == 1:
@@ -670,15 +689,15 @@
             df_tmp['File'] = file_base
             df_tmp['Value'] = 1
             df_final = pd.concat([df_final, df_tmp])
             # print(df_final)
 
     df_pivot = df_final.pivot_table(index='File',
                                     columns='Gene', values='Mutation', aggfunc=lambda x: ','.join(map(str, x)))
-    print(df_pivot)
+    # print(df_pivot)
     summary_file = os.path.join(output_path, 'PointMutation_Summary.csv')
 
     df_pivot.to_csv(summary_file)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `PointBlaster-0.2.1/PointBlaster/db/.DS_Store` & `PointBlaster-0.2.2/PointBlaster/db/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/.DS_Store` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/.DS_Store` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/23S.fsa` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/23S.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/acrB.fsa` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/acrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/gyrA.fsa` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/gyrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/gyrB.fsa` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/gyrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/parC.fsa` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/parC.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/parE.fsa` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/parE.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/phenotypes.txt` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/phenotypes.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/pmrA.fsa` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/pmrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/pmrB.fsa` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/pmrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/salmonella.fsa` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/salmonella.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b` & `PointBlaster-0.2.2/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/PointBlaster.egg-info/PKG-INFO` & `PointBlaster-0.2.2/PointBlaster.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PointBlaster
-Version: 0.2.1
+Version: 0.2.2
 Summary: find point mutation in assembled genomes
 Home-page: https://github.com/hbucqp/PointBlaster
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,wgs,blastn,pointmutation
 Platform: any
```

### Comparing `PointBlaster-0.2.1/PointBlaster.egg-info/SOURCES.txt` & `PointBlaster-0.2.2/PointBlaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/README.md` & `PointBlaster-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/dist/.DS_Store` & `PointBlaster-0.2.2/dist/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.2.1/setup.py` & `PointBlaster-0.2.2/setup.py`

 * *Files identical despite different names*

