# Comparing `tmp/tja2fumen-0.1.1.tar.gz` & `tmp/tja2fumen-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tja2fumen-0.1.1.tar", last modified: Tue Jun 27 23:37:57 2023, max compression
+gzip compressed data, was "tja2fumen-0.2.0.tar", last modified: Sat Jul  1 21:44:13 2023, max compression
```

## Comparing `tja2fumen-0.1.1.tar` & `tja2fumen-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 23:37:57.873737 tja2fumen-0.1.1/
--rw-rw-rw-   0        0        0     1083 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4390 2023-06-27 23:37:57.873737 tja2fumen-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2669 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/README.md
--rw-rw-rw-   0        0        0      770 2023-06-27 23:37:43.000000 tja2fumen-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-27 23:37:57.873737 tja2fumen-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0       98 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 23:37:57.842462 tja2fumen-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-27 23:37:57.858164 tja2fumen-0.1.1/src/tja2fumen/
--rw-rw-rw-   0        0        0     1609 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/src/tja2fumen/__init__.py
--rw-rw-rw-   0        0        0     4430 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/src/tja2fumen/constants.py
--rw-rw-rw-   0        0        0    12255 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/src/tja2fumen/converters.py
--rw-rw-rw-   0        0        0    20582 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/src/tja2fumen/parsers.py
-drwxrwxrwx   0        0        0        0 2023-06-27 23:37:57.873737 tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/
--rw-rw-rw-   0        0        0    23889 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Easy-1.csv
--rw-rw-rw-   0        0        0    23889 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv
--rw-rw-rw-   0        0        0    23890 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv
--rw-rw-rw-   0        0        0    23886 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv
--rw-rw-rw-   0        0        0    23884 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Hard-3.csv
--rw-rw-rw-   0        0        0    23884 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Hard-4.csv
--rw-rw-rw-   0        0        0    23883 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv
--rw-rw-rw-   0        0        0    23889 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv
--rw-rw-rw-   0        0        0    23889 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Normal-3.csv
--rw-rw-rw-   0        0        0    23887 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Normal-4.csv
--rw-rw-rw-   0        0        0    23886 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv
--rw-rw-rw-   0        0        0    23880 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv
--rw-rw-rw-   0        0        0    23872 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Oni-8.csv
--rw-rw-rw-   0        0        0    23869 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv
--rw-rw-rw-   0        0        0     3864 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/src/tja2fumen/utils.py
--rw-rw-rw-   0        0        0     2847 2023-06-27 23:37:02.000000 tja2fumen-0.1.1/src/tja2fumen/writers.py
-drwxrwxrwx   0        0        0        0 2023-06-27 23:37:57.858164 tja2fumen-0.1.1/src/tja2fumen.egg-info/
--rw-rw-rw-   0        0        0     4390 2023-06-27 23:37:57.000000 tja2fumen-0.1.1/src/tja2fumen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-06-27 23:37:57.000000 tja2fumen-0.1.1/src/tja2fumen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 23:37:57.000000 tja2fumen-0.1.1/src/tja2fumen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-27 23:37:57.000000 tja2fumen-0.1.1/src/tja2fumen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-06-27 23:37:57.000000 tja2fumen-0.1.1/src/tja2fumen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-27 23:37:57.000000 tja2fumen-0.1.1/src/tja2fumen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 21:44:13.298722 tja2fumen-0.2.0/
+-rw-rw-rw-   0        0        0     1083 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4388 2023-07-01 21:44:13.298722 tja2fumen-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2669 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/README.md
+-rw-rw-rw-   0        0        0      897 2023-07-01 21:43:57.000000 tja2fumen-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-01 21:44:13.298722 tja2fumen-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       98 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:44:13.267272 tja2fumen-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-01 21:44:13.282905 tja2fumen-0.2.0/src/tja2fumen/
+-rw-rw-rw-   0        0        0     1597 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/__init__.py
+-rw-rw-rw-   0        0        0     3856 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/constants.py
+-rw-rw-rw-   0        0        0    15602 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/converters.py
+-rw-rw-rw-   0        0        0    18892 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/parsers.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:44:13.298722 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/
+-rw-rw-rw-   0        0        0    23889 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Easy-1.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv
+-rw-rw-rw-   0        0        0    23890 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv
+-rw-rw-rw-   0        0        0    23886 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv
+-rw-rw-rw-   0        0        0    23884 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Hard-3.csv
+-rw-rw-rw-   0        0        0    23884 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Hard-4.csv
+-rw-rw-rw-   0        0        0    23883 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Normal-3.csv
+-rw-rw-rw-   0        0        0    23887 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Normal-4.csv
+-rw-rw-rw-   0        0        0    23886 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv
+-rw-rw-rw-   0        0        0    23880 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv
+-rw-rw-rw-   0        0        0    23872 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Oni-8.csv
+-rw-rw-rw-   0        0        0    23869 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv
+-rw-rw-rw-   0        0        0     3308 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/utils.py
+-rw-rw-rw-   0        0        0     2905 2023-07-01 21:42:53.000000 tja2fumen-0.2.0/src/tja2fumen/writers.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:44:13.282905 tja2fumen-0.2.0/src/tja2fumen.egg-info/
+-rw-rw-rw-   0        0        0     4388 2023-07-01 21:44:13.000000 tja2fumen-0.2.0/src/tja2fumen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-07-01 21:44:13.000000 tja2fumen-0.2.0/src/tja2fumen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 21:44:13.000000 tja2fumen-0.2.0/src/tja2fumen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-01 21:44:13.000000 tja2fumen-0.2.0/src/tja2fumen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-07-01 21:44:13.000000 tja2fumen-0.2.0/src/tja2fumen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-01 21:44:13.000000 tja2fumen-0.2.0/src/tja2fumen.egg-info/top_level.txt
```

### Comparing `tja2fumen-0.1.1/LICENSE.txt` & `tja2fumen-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.1.1/PKG-INFO` & `tja2fumen-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.1.1
+Version: 0.2.0
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -25,15 +25,15 @@
         SOFTWARE.
 Project-URL: Homepage, https://github.com/vivaria/tja2fumen/
 Project-URL: Bug Reports, https://github.com/vivaria/tja2fumen/issues/
 Project-URL: Source, https://github.com/vivaria/tja2fumen/
 Keywords: taiko,tatsujin,fumen,TJA
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: build
+Provides-Extra: dev
 License-File: LICENSE.txt
 
 # tja2fumen
 
 `tja2fumen` is a tool for Taiko no Tatsujin games that allows you to convert TJA files (`.tja`) to fumen files (`.bin`).
 
 This project attempts to replace/complement the existing closed-source [tja2bin.exe](https://github.com/Fluto/TakoTako/blob/c269bcab60530877a16c2a473c84796b94d0a5ce/README.md?plain=1#L181) converter packaged alongside TakoTako.
```

### Comparing `tja2fumen-0.1.1/README.md` & `tja2fumen-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.1.1/pyproject.toml` & `tja2fumen-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tja2fumen"
-version = "0.1.1"
+version = "0.2.0"
 description = "Convert TJA chart files into fumen (.bin) chart files"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["taiko", "tatsujin", "fumen", "TJA"]
 
 [project.urls]  # Optional
@@ -14,11 +14,15 @@
 
 # The following would provide a command line executable called `sample`
 # which executes the function `main` from this package when invoked.
 [project.scripts]  # Optional
 tja2fumen = "tja2fumen:main"
 
 [project.optional-dependencies]
-build = ["pyinstaller"]
+dev = ["pytest", "build", "pyinstaller", "twine", "toml-cli"]
 
 [tool.setuptools.packages.find]
-where = ["src"]
+where = ["src"]
+
+[tool.pytest.ini_options]
+addopts = "-vv --tb=short"
+console_output_style = "count"
```

### Comparing `tja2fumen-0.1.1/src/tja2fumen/__init__.py` & `tja2fumen-0.2.0/src/tja2fumen/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     baseName = os.path.splitext(fnameTJA)[0]
     outputFilenames = [baseName + f"_{COURSE_IDS[course]}.bin" if len(parsedSongsTJA) > 1
                        else baseName + ".bin"
                        for course in parsedSongsFumen.keys()]
 
     # Write fumen data to files
     for fumenData, outputName in zip(parsedSongsFumen.values(), outputFilenames):
-        writeFumen(open(outputName, "wb"), fumenData)
+        writeFumen(outputName, fumenData)
 
     if return_vars:
         return parsedSongsTJA, parsedSongsFumen, outputFilenames
 
 
 # NB: This entry point is necessary for the Pyinstaller executable
 if __name__ == "__main__":
```

### Comparing `tja2fumen-0.1.1/src/tja2fumen/constants.py` & `tja2fumen-0.2.0/src/tja2fumen/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-# Various commands and header fields for TJA files
-HEADER_GLOBAL = ['TITLE', 'TITLEJA', 'SUBTITLE', 'SUBTITLEJA', 'BPM', 'WAVE', 'OFFSET', 'DEMOSTART', 'GENRE',
-                 'SCOREMODE', 'BGMOVIE', 'SONGVOL', 'SEVOL']
-HEADER_COURSE = ['COURSE', 'LEVEL', 'BALLOON', 'SCOREINIT', 'SCOREDIFF', 'STYLE']
-BRANCH_COMMANDS = ['START', 'END', 'BRANCHSTART', 'BRANCHEND', 'N', 'E', 'M', 'SECTION']
-MEASURE_COMMANDS = ['MEASURE', 'GOGOSTART', 'GOGOEND', 'BARLINEON', 'BARLINEOFF', 'SCROLL', 'BPMCHANGE', 'DELAY', 'LEVELHOLD']
-COMMAND = BRANCH_COMMANDS + MEASURE_COMMANDS
-
 # Note types for TJA files
 TJA_NOTE_TYPES = {
     '1': 'Don',
     '2': 'Ka',
     '3': 'DON',
     '4': 'KA',
     '5': 'Drumroll',
```

### Comparing `tja2fumen-0.1.1/src/tja2fumen/converters.py` & `tja2fumen-0.2.0/src/tja2fumen/converters.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,230 +1,272 @@
 from copy import deepcopy
+import re
 
 from tja2fumen.utils import computeSoulGaugeBytes
-from tja2fumen.constants import TJA_NOTE_TYPES, DIFFICULTY_BYTES, sampleHeaderMetadata, simpleHeaders
+from tja2fumen.constants import DIFFICULTY_BYTES, sampleHeaderMetadata, simpleHeaders
 
 # Filler metadata that the `writeFumen` function expects
 # TODO: Determine how to properly set the item byte (https://github.com/vivaria/tja2fumen/issues/17)
 default_note = {'type': '', 'pos': 0.0, 'item': 0, 'padding': 0.0,
                 'scoreInit': 0, 'scoreDiff': 0, 'duration': 0.0}
 default_branch = {'length': 0, 'padding': 0, 'speed': 1.0}
 default_measure = {
     'bpm': 0.0,
     'fumenOffset': 0.0,
     'gogo': False,
     'barline': True,
     'padding1': 0,
+    'branchStart': None,
     'branchInfo': [-1, -1, -1, -1, -1, -1],
     'padding2': 0,
     'normal': deepcopy(default_branch),
     'advanced': deepcopy(default_branch),
     'master': deepcopy(default_branch)
 }
 
 
-def preprocessTJAMeasures(tja):
+def processTJACommands(tja):
     """
     Merge TJA 'data' and 'event' fields into a single measure property, and split
-    measures into sub-measures whenever a mid-measure BPM change occurs.
+    measures into sub-measures whenever a mid-measure BPM/SCROLL/GOGO change occurs.
 
     The TJA parser produces measure objects with two important properties:
       - 'data': Contains the note data (1: don, 2: ka, etc.) along with spacing (s)
       - 'events' Contains event commands such as MEASURE, BPMCHANGE, GOGOTIME, etc.
 
     However, notes and events can be intertwined within a single measure. So, it's
     not possible to process them separately; they must be considered as single sequence.
 
     A particular danger is BPM changes. TJA allows multiple BPMs within a single measure,
     but the fumen format permits one BPM per measure. So, a TJA measure must be split up
     if it has multiple BPM changes within a measure.
 
     In the future, this logic should probably be moved into the TJA parser itself.
     """
-    currentBPM = 0
-    currentScroll = 1.0
-    currentGogo = False
-    currentBarline = True
-
-    measuresCorrected = []
-    for measure in tja['measures']:
-        # Step 1: Combine notes and events
-        notes = [{'pos': i, 'type': 'note', 'value': TJA_NOTE_TYPES[note]}
-                 for i, note in enumerate(measure['data']) if note != '0']
-        events = [{'pos': e['position'], 'type': e['name'], 'value': e['value']}
-                  for e in measure['events']]
-        combined = []
-        while notes or events:
-            if events and notes:
-                if notes[0]['pos'] >= events[0]['pos']:
-                    combined.append(events.pop(0))
-                else:
-                    combined.append(notes.pop(0))
-            elif events:
-                combined.append(events.pop(0))
-            elif notes:
-                combined.append(notes.pop(0))
-
-        # Step 2: Split measure into submeasure
-        measure_cur = {'bpm': currentBPM, 'scroll': currentScroll, 'gogo': currentGogo, 'barline': currentBarline,
-                       'subdivisions': len(measure['data']), 'pos_start': 0, 'pos_end': 0,
-                       'time_sig': measure['length'], 'data': []}
-        for data in combined:
-            if data['type'] == 'note':
-                measure_cur['data'].append(data)
-            elif data['type'] == 'bpm':
-                currentBPM = float(data['value'])
-                # Case 1: BPM change at the start of a measure; just change BPM
-                if data['pos'] == 0:
-                    measure_cur['bpm'] = currentBPM
-                # Case 2: BPM change mid-measure, so start a new sub-measure
+    branches = tja['branches']
+    branchesCorrected = {branchName: [] for branchName in branches.keys()}
+    for branchName, branch in branches.items():
+        currentBPM = float(tja['metadata']['bpm'])
+        currentScroll = 1.0
+        currentGogo = False
+        currentBarline = True
+        currentDividend = 4
+        currentDivisor = 4
+        for measure in branch:
+            # Split measure into submeasure
+            measure_cur = {'bpm': currentBPM, 'scroll': currentScroll, 'gogo': currentGogo, 'barline': currentBarline,
+                           'subdivisions': len(measure['data']), 'pos_start': 0, 'pos_end': 0,
+                           'branchStart': None, 'time_sig': [currentDividend, currentDivisor], 'data': []}
+            for data in measure['combined']:
+                # Handle note data
+                if data['type'] == 'note':
+                    measure_cur['data'].append(data)
+
+                # Handle commands that can only be placed between measures (i.e. no mid-measure variations)
+                elif data['type'] == 'branchStart':
+                    measure_cur['branchStart'] = data['value']
+                elif data['type'] == 'barline':
+                    currentBarline = bool(int(data['value']))
+                    measure_cur['barline'] = currentBarline
+                elif data['type'] == 'measure':
+                    matchMeasure = re.match(r"(\d+)/(\d+)", data['value'])
+                    if not matchMeasure:
+                        continue
+                    currentDividend = int(matchMeasure.group(1))
+                    currentDivisor = int(matchMeasure.group(2))
+                    measure_cur['time_sig'] = [currentDividend, currentDivisor]
+
+                # Handle commands that can be placed in the middle of a measure.
+                #    NB: For fumen files, if there is a mid-measure change to BPM/SCROLL/GOGO, then the measure will
+                #    actually be split into two small submeasures. So, we need to start a new measure in those cases.
+                elif data['type'] in ['bpm', 'scroll', 'gogo']:
+                    # Parse the values
+                    if data['type'] == 'bpm':
+                        new_val = currentBPM = float(data['value'])
+                    elif data['type'] == 'scroll':
+                        new_val = currentScroll = data['value']
+                    elif data['type'] == 'gogo':
+                        new_val = currentGogo = bool(int(data['value']))
+                    # Check for mid-measure commands
+                    # - Case 1: Command happens at the start of a measure; just change the value directly
+                    if data['pos'] == 0:
+                        measure_cur[data['type']] = new_val
+                    # - Case 2: Command occurs mid-measure, so start a new sub-measure
+                    else:
+                        measure_cur['pos_end'] = data['pos']
+                        branchesCorrected[branchName].append(measure_cur)
+                        measure_cur = {'bpm': currentBPM, 'scroll': currentScroll, 'gogo': currentGogo,
+                                       'barline': currentBarline,
+                                       'subdivisions': len(measure['data']), 'pos_start': data['pos'], 'pos_end': 0,
+                                       'branchStart': None, 'time_sig': [currentDividend, currentDivisor], 'data': []}
+
                 else:
-                    measure_cur['pos_end'] = data['pos']
-                    measuresCorrected.append(measure_cur)
-                    measure_cur = {'bpm': currentBPM, 'scroll': currentScroll, 'gogo': currentGogo, 'barline': currentBarline,
-                                   'subdivisions': len(measure['data']), 'pos_start': data['pos'], 'pos_end': 0,
-                                   'time_sig': measure['length'], 'data': []}
-            elif data['type'] == 'scroll':
-                currentScroll = data['value']
-                measure_cur['scroll'] = currentScroll
-            elif data['type'] == 'gogo':
-                currentGogo = bool(int(data['value']))
-                measure_cur['gogo'] = currentGogo
-            elif data['type'] == 'barline':
-                currentBarline = bool(int(data['value']))
-                measure_cur['barline'] = currentBarline
-            else:
-                print(f"Unexpected event type: {data['type']}")
-        measure_cur['pos_end'] = len(measure['data'])
-        measuresCorrected.append(measure_cur)
+                    print(f"Unexpected event type: {data['type']}")
 
-    return measuresCorrected
+            measure_cur['pos_end'] = len(measure['data'])
+            branchesCorrected[branchName].append(measure_cur)
 
+    hasBranches = all(len(b) for b in branchesCorrected.values())
+    if hasBranches:
+        branch_lens = [len(b) for b in branches.values()]
+        if not branch_lens.count(branch_lens[0]) == len(branch_lens):
+            raise ValueError("Branches do not have the same number of measures.")
+        else:
+            branchCorrected_lens = [len(b) for b in branchesCorrected.values()]
+            if not branchCorrected_lens.count(branchCorrected_lens[0]) == len(branchCorrected_lens):
+                raise ValueError("Branches do not have matching GOGO/SCROLL/BPM commands.")
 
-def convertTJAToFumen(tja):
-    # Hardcode currentBranch due to current lack of support for branching songs
-    currentBranch = 'normal'  # TODO: Program in branch support
-    tja['measures'] = preprocessTJAMeasures(tja)
-    measureDurationPrev = 0
-    currentDrumroll = None
-    total_notes = 0
+    return branchesCorrected
 
+
+def convertTJAToFumen(tja):
+    # Preprocess commands
+    tja['branches'] = processTJACommands(tja)
     # Parse TJA measures to create converted TJA -> Fumen file
-    tjaConverted = {'measures': []}
-    for idx_m, measureTJA in enumerate(tja['measures']):
-        measureFumen = deepcopy(default_measure)
-
-        # Compute the duration of the measure
-        measureSize = measureTJA['time_sig'][0] / measureTJA['time_sig'][1]
-        measureLength = measureTJA['pos_end'] - measureTJA['pos_start']
-        measureRatio = 1.0 if measureTJA['subdivisions'] == 0.0 else (measureLength / measureTJA['subdivisions'])
-        # - measureDurationBase: The "base" measure duration, computed using a single BPM value.
-        # - measureDuration: The actual measure duration, which may be adjusted if there is a mid-measure BPM change.
-        measureDurationBase = measureDuration = (4 * 60_000 * measureSize * measureRatio / measureTJA['bpm'])
-        # The following adjustment accounts for BPM changes. (!!! Discovered by tana :3 !!!)
-        if idx_m != len(tja['measures'])-1:
-            measureTJANext = tja['measures'][idx_m + 1]
-            if measureTJA['bpm'] != measureTJANext['bpm']:
-                measureDuration -= (4 * 60_000 * ((1 / measureTJANext['bpm']) - (1 / measureTJA['bpm'])))
-
-        # Compute the millisecond offset for each measure
-        if idx_m == 0:
-            pass  # NB: Pass for now, since we need the 2nd measure's duration to compute the 1st measure's offset
-        else:
-            # Compute the 1st measure's offset by subtracting the 2nd measure's duration from the tjaOffset
-            if idx_m == 1:
-                tjaOffset = float(tja['metadata']['offset']) * 1000 * -1
-                tjaConverted['measures'][-1]['fumenOffset'] = tjaOffset - measureDuration
-            # Use the previous measure's offset plus the previous duration to compute the current measure's offset
-            measureOffsetPrev = tjaConverted['measures'][-1]['fumenOffset']
-            measureFumen['fumenOffset'] = measureOffsetPrev + measureDurationPrev
-        measureDurationPrev = measureDuration
-
-        # Best guess at what 'barline' status means for each measure:
-        # - 'True' means the measure lands on a barline (i.e. most measures), and thus barline should be shown
-        # - 'False' means that the measure doesn't land on a barline, and thus barline should be hidden.
-        #   For example:
-        #     1. Measures where #BARLINEOFF has been set
-        #     2. Sub-measures that don't fall on the barline
-        if measureTJA['barline'] is False or (measureRatio != 1.0 and measureTJA['pos_start'] != 0):
-            measureFumen['barline'] = False
-
-        # Create note dictionaries based on TJA measure data (containing 0's plus 1/2/3/4/etc. for notes)
-        note_counter = 0
-        for idx_d, data in enumerate(measureTJA['data']):
-            if data['type'] == 'note':
-                # Note positions must be calculated using the base measure duration (that uses a single BPM value)
-                # (In other words, note positions do not take into account any mid-measure BPM change adjustments.)
-                note_pos = measureDurationBase * (data['pos'] - measureTJA['pos_start']) / measureLength
-                # Handle the note that represents the end of a drumroll/balloon
-                if data['value'] == "EndDRB":
-                    # If a drumroll spans a single measure, then add the difference between start/end position
-                    if 'multimeasure' not in currentDrumroll.keys():
-                        currentDrumroll['duration'] += (note_pos - currentDrumroll['pos'])
-                    # Otherwise, if a drumroll spans multiple measures, then we want to add the duration between
-                    # the start of the measure (i.e. pos=0.0) and the drumroll's end position.
-                    else:
-                        currentDrumroll['duration'] += (note_pos - 0.0)
-                    # 1182, 1385, 1588, 2469, 1568, 752, 1568
-                    currentDrumroll['duration'] = float(int(currentDrumroll['duration']))
-                    currentDrumroll = None
-                    continue
-                # The TJA spec technically allows you to place double-Kusudama notes:
-                #    "Use another 9 to specify when to lower the points for clearing."
-                # But this is unsupported in fumens, so just skip the second Kusudama note.
-                if data['value'] == "Kusudama" and currentDrumroll:
-                    continue
-                # Handle the remaining non-EndDRB, non-double Kusudama notes
-                note = deepcopy(default_note)
-                note['pos'] = note_pos
-                note['type'] = data['value']
-                note['scoreInit'] = tja['scoreInit']  # Probably not fully accurate
-                note['scoreDiff'] = tja['scoreDiff']  # Probably not fully accurate
-                # Handle drumroll/balloon-specific metadata
-                if note['type'] in ["Balloon", "Kusudama"]:
-                    note['hits'] = tja['metadata']['balloon'].pop(0)
-                    note['hitsPadding'] = 0
-                    currentDrumroll = note
-                    total_notes -= 1
-                if note['type'] in ["Drumroll", "DRUMROLL"]:
-                    note['drumrollBytes'] = b'\x00\x00\x00\x00\x00\x00\x00\x00'
-                    currentDrumroll = note
-                    total_notes -= 1
-                measureFumen[currentBranch][note_counter] = note
-                note_counter += 1
-        measureFumen[currentBranch]['length'] = note_counter
-        measureFumen[currentBranch]['speed'] = measureTJA['scroll']
-        measureFumen['gogo'] = measureTJA['gogo']
-        measureFumen['bpm'] = measureTJA['bpm']
-
-        # Append the measure to the tja's list of measures
-        tjaConverted['measures'].append(measureFumen)
-
-        # If drumroll hasn't ended by the end of this measure, increase duration by measure timing
-        if currentDrumroll:
-            if currentDrumroll['duration'] == 0.0:
-                currentDrumroll['duration'] += (measureDurationBase - currentDrumroll['pos'])
-                currentDrumroll['multimeasure'] = True
+    tjaConverted = {'measures': [deepcopy(default_measure) for _ in range(len(tja['branches']['normal']))]}
+    for currentBranch, branch in tja['branches'].items():
+        if not len(branch):
+            continue
+        total_notes = 0
+        total_notes_branch = 0
+        note_counter_branch = 0
+        measureDurationPrev = 0
+        currentDrumroll = None
+        courseBalloons = tja['metadata']['balloon'].copy()
+        for idx_m, measureTJA in enumerate(branch):
+            measureFumen = tjaConverted['measures'][idx_m]
+
+            # Check to see if the measure contains a branching condition
+            if measureTJA['branchStart']:
+                measureFumen['branchStart'] = measureTJA['branchStart']
+            if measureFumen['branchStart']:
+                if measureFumen['branchStart'][0] == 'p':
+                    if currentBranch == 'normal':
+                        idx_b1, idx_b2 = 0, 1
+                    elif currentBranch == 'advanced':
+                        idx_b1, idx_b2 = 2, 3
+                    elif currentBranch == 'master':
+                        idx_b1, idx_b2 = 4, 5
+                    measureFumen['branchInfo'][idx_b1] = int(total_notes_branch * measureFumen['branchStart'][1] * 20)
+                    measureFumen['branchInfo'][idx_b2] = int(total_notes_branch * measureFumen['branchStart'][2] * 20)
+                elif measureTJA['branchStart'][0] == 'r':
+                    pass
+                total_notes_branch = 0
+            total_notes_branch += note_counter_branch
+
+            # Compute the duration of the measure
+            measureSize = measureTJA['time_sig'][0] / measureTJA['time_sig'][1]
+            measureLength = measureTJA['pos_end'] - measureTJA['pos_start']
+            measureRatio = 1.0 if measureTJA['subdivisions'] == 0.0 else (measureLength / measureTJA['subdivisions'])
+            # - measureDurationBase: The "base" measure duration, computed using a single BPM value.
+            # - measureDuration: The actual measure duration, which may be adjusted if there is a mid-measure BPM change.
+            measureDurationBase = measureDuration = (4 * 60_000 * measureSize * measureRatio / measureTJA['bpm'])
+            # The following adjustment accounts for BPM changes. (!!! Discovered by tana :3 !!!)
+            if idx_m != len(branch)-1:
+                measureTJANext = branch[idx_m + 1]
+                if measureTJA['bpm'] != measureTJANext['bpm']:
+                    measureDuration -= (4 * 60_000 * ((1 / measureTJANext['bpm']) - (1 / measureTJA['bpm'])))
+
+            # Compute the millisecond offset for each measure
+            if idx_m == 0:
+                pass  # NB: Pass for now, since we need the 2nd measure's duration to compute the 1st measure's offset
             else:
-                currentDrumroll['duration'] += measureDurationBase
+                # Compute the 1st measure's offset by subtracting the 2nd measure's duration from the tjaOffset
+                if idx_m == 1:
+                    tjaOffset = float(tja['metadata']['offset']) * 1000 * -1
+                    tjaConverted['measures'][idx_m-1]['fumenOffset'] = tjaOffset - measureDurationPrev
+                # Use the previous measure's offset plus the previous duration to compute the current measure's offset
+                measureOffsetPrev = tjaConverted['measures'][idx_m-1]['fumenOffset']
+                measureFumen['fumenOffset'] = measureOffsetPrev + measureDurationPrev
+            measureDurationPrev = measureDuration
+
+            # Best guess at what 'barline' status means for each measure:
+            # - 'True' means the measure lands on a barline (i.e. most measures), and thus barline should be shown
+            # - 'False' means that the measure doesn't land on a barline, and thus barline should be hidden.
+            #   For example:
+            #     1. Measures where #BARLINEOFF has been set
+            #     2. Sub-measures that don't fall on the barline
+            if measureTJA['barline'] is False or (measureRatio != 1.0 and measureTJA['pos_start'] != 0):
+                measureFumen['barline'] = False
+
+            # Create note dictionaries based on TJA measure data (containing 0's plus 1/2/3/4/etc. for notes)
+            note_counter_branch = 0
+            note_counter = 0
+            for idx_d, data in enumerate(measureTJA['data']):
+                if data['type'] == 'note':
+                    # Note positions must be calculated using the base measure duration (that uses a single BPM value)
+                    # (In other words, note positions do not take into account any mid-measure BPM change adjustments.)
+                    note_pos = measureDurationBase * (data['pos'] - measureTJA['pos_start']) / measureLength
+                    # Handle the note that represents the end of a drumroll/balloon
+                    if data['value'] == "EndDRB":
+                        # If a drumroll spans a single measure, then add the difference between start/end position
+                        if 'multimeasure' not in currentDrumroll.keys():
+                            currentDrumroll['duration'] += (note_pos - currentDrumroll['pos'])
+                        # Otherwise, if a drumroll spans multiple measures, then we want to add the duration between
+                        # the start of the measure (i.e. pos=0.0) and the drumroll's end position.
+                        else:
+                            currentDrumroll['duration'] += (note_pos - 0.0)
+                        # 1182, 1385, 1588, 2469, 1568, 752, 1568
+                        currentDrumroll['duration'] = float(int(currentDrumroll['duration']))
+                        currentDrumroll = None
+                        continue
+                    # The TJA spec technically allows you to place double-Kusudama notes:
+                    #    "Use another 9 to specify when to lower the points for clearing."
+                    # But this is unsupported in fumens, so just skip the second Kusudama note.
+                    if data['value'] == "Kusudama" and currentDrumroll:
+                        continue
+                    # Handle the remaining non-EndDRB, non-double Kusudama notes
+                    note = deepcopy(default_note)
+                    note['pos'] = note_pos
+                    note['type'] = data['value']
+                    note['scoreInit'] = tja['metadata']['scoreInit']  # Probably not fully accurate
+                    note['scoreDiff'] = tja['metadata']['scoreDiff']  # Probably not fully accurate
+                    # Handle drumroll/balloon-specific metadata
+                    if note['type'] in ["Balloon", "Kusudama"]:
+                        note['hits'] = courseBalloons.pop(0)
+                        note['hitsPadding'] = 0
+                        currentDrumroll = note
+                        total_notes -= 1
+                    if note['type'] in ["Drumroll", "DRUMROLL"]:
+                        note['drumrollBytes'] = b'\x00\x00\x00\x00\x00\x00\x00\x00'
+                        currentDrumroll = note
+                        total_notes -= 1
+                    # Count dons, kas, and balloons for the purpose of tracking branching accuracy
+                    if note['type'].lower() in ['don', 'ka']:
+                        note_counter_branch += 1
+                    elif note['type'].lower() in ['balloon', 'kusudama']:
+                        note_counter_branch += 1.5
+                    measureFumen[currentBranch][note_counter] = note
+                    note_counter += 1
+            measureFumen[currentBranch]['length'] = note_counter
+            measureFumen[currentBranch]['speed'] = measureTJA['scroll']
+            measureFumen['gogo'] = measureTJA['gogo']
+            measureFumen['bpm'] = measureTJA['bpm']
+
+            # If drumroll hasn't ended by the end of this measure, increase duration by measure timing
+            if currentDrumroll:
+                if currentDrumroll['duration'] == 0.0:
+                    currentDrumroll['duration'] += (measureDurationBase - currentDrumroll['pos'])
+                    currentDrumroll['multimeasure'] = True
+                else:
+                    currentDrumroll['duration'] += measureDurationBase
 
-        total_notes += note_counter
+            total_notes += note_counter
 
     # Take a stock header metadata sample and add song-specific metadata
-    headerMetadata = sampleHeaderMetadata
+    headerMetadata = sampleHeaderMetadata.copy()
     headerMetadata[8] = DIFFICULTY_BYTES[tja['metadata']['course']][0]
     headerMetadata[9] = DIFFICULTY_BYTES[tja['metadata']['course']][1]
     headerMetadata[20], headerMetadata[21] = computeSoulGaugeBytes(
         n_notes=total_notes,
         difficulty=tja['metadata']['course'],
         stars=tja['metadata']['level']
     )
     tjaConverted['headerMetadata'] = b"".join(i.to_bytes(1, 'little') for i in headerMetadata)
     tjaConverted['headerPadding'] = simpleHeaders[0]  # Use a basic, known set of header bytes
     tjaConverted['order'] = '<'
-    tjaConverted['length'] = len(tjaConverted['measures'])
     tjaConverted['unknownMetadata'] = 0
-    tjaConverted['branches'] = False
-    tjaConverted['scoreInit'] = tja['scoreInit']
-    tjaConverted['scoreDiff'] = tja['scoreDiff']
+    tjaConverted['branches'] = all([len(b) for b in tja['branches'].values()])
+    tjaConverted['scoreInit'] = tja['metadata']['scoreInit']
+    tjaConverted['scoreDiff'] = tja['metadata']['scoreDiff']
 
     return tjaConverted
```

### Comparing `tja2fumen-0.1.1/src/tja2fumen/parsers.py` & `tja2fumen-0.2.0/src/tja2fumen/parsers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,344 +1,295 @@
 import os
 import re
 
-from tja2fumen.utils import readStruct, getBool, shortHex, nameValue, debugPrint
-from tja2fumen.constants import (
-    # TJA constants
-    HEADER_GLOBAL, HEADER_COURSE, BRANCH_COMMANDS, MEASURE_COMMANDS, COMMAND, NORMALIZE_COURSE,
-    # Fumen constants
-    branchNames, noteTypes
-)
+from tja2fumen.utils import readStruct, getBool, shortHex
+from tja2fumen.constants import NORMALIZE_COURSE, TJA_NOTE_TYPES, branchNames, noteTypes
 
 
 ########################################################################################################################
 # TJA-parsing functions ( Original source: https://github.com/WHMHammer/tja-tools/blob/master/src/js/parseTJA.js)
 ########################################################################################################################
 
 
 def parseTJA(fnameTJA):
     try:
-        tja = open(fnameTJA, "r", encoding="utf-8-sig")
+        tja_text = open(fnameTJA, "r", encoding="utf-8-sig").read()
     except UnicodeDecodeError:
-        tja = open(fnameTJA, "r", encoding="shift-jis")
+        tja_text = open(fnameTJA, "r", encoding="shift-jis").read()
 
-    # Split into lines
-    lines = tja.read().splitlines()
-    lines = [line for line in lines if line.strip()]  # Discard empty lines
+    lines = [line for line in tja_text.splitlines() if line.strip() != '']
+    courses = getCourseData(lines)
+    for courseData in courses.values():
+        courseData['branches'] = parseCourseMeasures(courseData['data'])
 
-    # Line by line
-    headers = {}
+    return courses
+
+
+def getCourseData(lines):
     courses = {}
     currentCourse = ''
+    songBPM = 0
+    songOffset = 0
+
     for line in lines:
-        parsed = parseLine(line)
-        # Case 1: Comments (ignore)
-        if parsed['type'] == 'comment':
-            pass
-        # Case 2: Global header metadata
-        elif parsed['type'] == 'header' and parsed['scope'] == 'global':
-            headers[parsed['name'].lower()] = parsed['value']
-        # Case 3: Course data (metadata, commands, note data)
-        else:
-            # Check to see if we're starting a new course
-            if parsed['type'] == 'header' and parsed['scope'] == 'course' and parsed['name'] == 'COURSE':
-                currentCourse = NORMALIZE_COURSE[parsed['value']]
+        # Case 1: Header metadata
+        match_header = re.match(r"^([A-Z]+):(.*)", line)
+        if match_header:
+            nameUpper = match_header.group(1).upper()
+            value = match_header.group(2).strip()
+
+            # Global header fields
+            if nameUpper == 'BPM':
+                songBPM = value
+            elif nameUpper == 'OFFSET':
+                songOffset = value
+
+            # Course-specific header fields
+            elif nameUpper == 'COURSE':
+                currentCourse = NORMALIZE_COURSE[value]
                 if currentCourse not in courses.keys():
-                    courses[currentCourse] = []
-            # Append the line to the current course
-            courses[currentCourse].append(parsed)
-
-    # Convert parsed course lines into actual note data
-    songs = {}
-    for courseName, courseLines in courses.items():
-        courseHeader, courseMeasures = getCourse(headers, courseLines)
-        songs[courseName] = applyFumenStructureToParsedTJA(headers, courseHeader, courseMeasures)
-
-    return songs
-
-
-def parseLine(line):
-    # Regex matches for various line types
-    match_comment = re.match(r"//.*", line)
-    match_header = re.match(r"^([A-Z]+):(.*)", line)
-    match_command = re.match(r"^#([A-Z]+)(?:\s+(.+))?", line)
-    match_data = re.match(r"^(([0-9]|A|B|C|F|G)*,?).*$", line)
-
-    if match_comment:
-        return {"type": 'comment', "value": line}
-
-    elif match_header:
-        nameUpper = match_header.group(1).upper()
-        value = match_header.group(2)
-        if nameUpper in HEADER_GLOBAL:
-            return {"type": 'header', "scope": 'global', "name": nameUpper, "value": value.strip()}
-        elif nameUpper in HEADER_COURSE:
-            return {"type": 'header', "scope": 'course', "name": nameUpper, "value": value.strip()}
-
-    elif match_command:
-        nameUpper = match_command.group(1).upper()
-        value = match_command.group(2) if match_command.group(2) else ''
-        if nameUpper in COMMAND:
-            return {"type": 'command', "name": nameUpper, "value": value.strip()}
-
-    elif match_data:
-        return {"type": 'data', "data": match_data.group(1)}
-
-    return {"type": 'unknown', "value": line}
-
-
-def getCourse(tjaHeaders, lines):
-    def parseHeaderMetadata(line):
-        nonlocal headers
-        if line["name"] == 'COURSE':
-            headers['course'] = NORMALIZE_COURSE[line['value']]
-        elif line["name"] == 'LEVEL':
-            headers['level'] = int(line['value']) if line['value'] else 0
-        elif line["name"] == 'SCOREINIT':
-            headers['scoreInit'] = int(line['value']) if line['value'] else 0
-        elif line["name"] == 'SCOREDIFF':
-            headers['scoreDiff'] = int(line['value']) if line['value'] else 0
-        elif line["name"] == 'BALLOON':
-            if line['value']:
-                balloons = [int(v) for v in line['value'].split(",") if v]
+                    courses[currentCourse] = {
+                        'metadata': {'course': currentCourse, 'bpm': songBPM, 'offset': songOffset, 'level': 0,
+                                     'balloon': [], 'scoreInit': 0, 'scoreDiff': 0},
+                        'data': [],
+                    }
+            elif nameUpper == 'LEVEL':
+                courses[currentCourse]['metadata']['level'] = int(value) if value else 0
+            elif nameUpper == 'SCOREINIT':
+                courses[currentCourse]['metadata']['scoreInit'] = int(value) if value else 0
+            elif nameUpper == 'SCOREDIFF':
+                courses[currentCourse]['metadata']['scoreDiff'] = int(value) if value else 0
+            elif nameUpper == 'BALLOON':
+                if value:
+                    balloons = [int(v) for v in value.split(",") if v]
+                    courses[currentCourse]['metadata']['balloon'] = balloons
+            # STYLE is a P1/P2 command, which we don't support yet, so normally this would be a
+            # NotImplemetedError. However, TakoTako outputs `STYLE:SINGLE` when converting Ura
+            # charts, so throwing an error here would prevent Ura charts from being converted.
+            # See: https://github.com/vivaria/tja2fumen/issues/15#issuecomment-1575341088
+            elif nameUpper == 'STYLE':
+                pass
             else:
-                balloons = []
-            headers['balloon'] = balloons
-        # STYLE is a P1/P2 command, which we don't support yet, so normally this would be a NotImplemetedError.
-        # However, TakoTako outputs `STYLE:SINGLE` when converting Ura charts, so throwing an error here prevents
-        # Ura charts from being converted. See: https://github.com/vivaria/tja2fumen/issues/15#issuecomment-1575341088
-        elif line["name"] == 'STYLE':
-            pass
-        else:
-            raise NotImplementedError
-
-    def parseBranchCommands(line):
-        nonlocal flagLevelhold, targetBranch, currentBranch
-        if line["name"] == 'BRANCHSTART':
-            if flagLevelhold:
-                return
-            values = line['value'].split(',')
-            if values[0] == 'r':
-                if len(values) >= 3:
-                    targetBranch = 'M'
-                elif len(values) == 2:
-                    targetBranch = 'E'
-                else:
-                    targetBranch = 'N'
-            elif values[0] == 'p':
-                if len(values) >= 3 and float(values[2]) <= 100:
-                    targetBranch = 'M'
-                elif len(values) >= 2 and float(values[1]) <= 100:
-                    targetBranch = 'E'
-                else:
-                    targetBranch = 'N'
-        elif line["name"] == 'BRANCHEND':
-            currentBranch = targetBranch
-        elif line["name"] == 'N':
-            currentBranch = 'N'
-        elif line["name"] == 'E':
-            currentBranch = 'E'
-        elif line["name"] == 'M':
-            currentBranch = 'M'
-        elif line["name"] == 'START' or line['name'] == 'END':
-            currentBranch = 'N'
-            targetBranch = 'N'
-            flagLevelhold = False
-        elif line['name'] == 'SECTION':
-            raise NotImplementedError
-        else:
-            raise NotImplementedError
-
-    def parseMeasureCommands(line):
-        nonlocal measureDivisor, measureDividend, measureEvents, flagLevelhold
-        if line['name'] == 'MEASURE':
-            matchMeasure = re.match(r"(\d+)/(\d+)", line['value'])
-            if not matchMeasure:
-                return
-            measureDividend = int(matchMeasure.group(1))
-            measureDivisor = int(matchMeasure.group(2))
-        elif line['name'] == 'GOGOSTART':
-            measureEvents.append({"name": 'gogo', "position": len(measureData), "value": '1'})
-        elif line['name'] == 'GOGOEND':
-            measureEvents.append({"name": 'gogo', "position": len(measureData), "value": '0'})
-        elif line['name'] == 'BARLINEON':
-            measureEvents.append({"name": 'barline', "position": len(measureData), "value": '1'})
-        elif line['name'] == 'BARLINEOFF':
-            measureEvents.append({"name": 'barline', "position": len(measureData), "value": '0'})
-        elif line['name'] == 'SCROLL':
-            measureEvents.append({"name": 'scroll', "position": len(measureData), "value": float(line['value'])})
-        elif line['name'] == 'BPMCHANGE':
-            measureEvents.append({"name": 'bpm', "position": len(measureData), "value": float(line['value'])})
-        elif line['name'] == 'LEVELHOLD':
-            flagLevelhold = True
-        elif line['name'] == 'DELAY':
-            raise NotImplementedError
-        elif line['name'] == 'LYRIC':
-            pass
-        elif line['name'] == 'NEXTSONG':
-            pass
-        else:
-            raise NotImplementedError
-
-    def parseMeasureData(line):
-        nonlocal measures, measureData, measureDividend, measureDivisor, measureEvents
-        data = line['data']
-        # If measure has ended, then append the measure and start anew
-        if data.endswith(','):
-            measureData += data[0:-1]
-            measure = {
-                "length": [measureDividend, measureDivisor],
-                "data": measureData,
-                "events": measureEvents,
-            }
-            measures.append(measure)
-            measureData = ''
-            measureEvents = []
-        # Otherwise, keep tracking measureData
-        else:
-            measureData += data
+                pass  # Ignore other header fields such as 'TITLE', 'SUBTITLE', 'WAVE', etc.
 
-    # Define state variables
-    headers = {'balloon': []}  # Charters sometimes exclude `BALLOON` entirely if there are none
-    measures = []
-    measureDividend = 4
-    measureDivisor = 4
-    measureData = ''
-    measureEvents = []
-    currentBranch = 'N'
-    targetBranch = 'N'
+        # Case 2: Commands and note data (to be further processed course-by-course later on)
+        elif not re.match(r"//.*", line):  # Exclude comment-only lines ('//')
+            match_command = re.match(r"^#([A-Z]+)(?:\s+(.+))?", line)
+            match_notes = re.match(r"^(([0-9]|A|B|C|F|G)*,?).*$", line)
+            if match_command:
+                nameUpper = match_command.group(1).upper()
+                value = match_command.group(2).strip() if match_command.group(2) else ''
+            elif match_notes:
+                nameUpper = 'NOTES'
+                value = match_notes.group(1)
+            courses[currentCourse]['data'].append({"name": nameUpper, "value": value})
+
+    return courses
+
+
+def parseCourseMeasures(lines):
+    # Check if the course has branches or not
+    hasBranches = True if [l for l in lines if l['name'] == 'BRANCHSTART'] else False
+    if hasBranches:
+        currentBranch = 'all'
+        targetBranch = 'all'
+    else:
+        currentBranch = 'normal'
+        targetBranch = 'normal'
     flagLevelhold = False
 
     # Process course lines
+    branches = {'normal': [], 'advanced': [], 'master': []}
+    measureNotes = ''
+    measureEvents = []
     for line in lines:
-        if line["type"] == 'header':
-            parseHeaderMetadata(line)
-        elif line["type"] == 'command' and line['name'] in BRANCH_COMMANDS:
-            parseBranchCommands(line)
-        elif line["type"] == 'command' and line['name'] in MEASURE_COMMANDS and currentBranch == targetBranch:
-            parseMeasureCommands(line)
-        elif line['type'] == 'data' and currentBranch == targetBranch:
-            parseMeasureData(line)
-
-    # Post-processing: Ensure the first measure has a BPM event
-    if measures:
-        firstBPMEventFound = False
-        # Search for BPM event in the first measure
-        for i in range(len(measures[0]['events'])):
-            evt = measures[0]['events'][i]
-            if evt['name'] == 'bpm' and evt['position'] == 0:
-                firstBPMEventFound = True
-        # If not present, insert a BPM event into the first measure using the global header metadata
-        if not firstBPMEventFound:
-            # noinspection PyTypeChecker
-            measures[0]['events'].insert(0, {"name": 'bpm', "position": 0, "value": tjaHeaders['bpm']})
-
-    # Post-processing: In case the file doesn't end on a "measure end" symbol (','), append whatever is left
-    if measureData:
-        measures.append({
-            "length": [measureDividend, measureDivisor],
-            "data": measureData,
+        # 1. Parse measure notes
+        if line['name'] == 'NOTES':
+            notes = line['value']
+            # If measure has ended, then append the measure and start anew
+            if notes.endswith(','):
+                measureNotes += notes[0:-1]
+                measureCurrent = {
+                    "data": measureNotes,
+                    "events": measureEvents,
+                }
+                if currentBranch == 'all':
+                    for branch in branches.keys():
+                        branches[branch].append(measureCurrent)
+                else:
+                    branches[currentBranch].append(measureCurrent)
+                measureNotes = ''
+                measureEvents = []
+            # Otherwise, keep tracking measureNotes
+            else:
+                measureNotes += notes
+
+        # 2. Parse commands
+        else:
+            # Measure commands
+            if line['name'] == 'GOGOSTART':
+                measureEvents.append({"name": 'gogo', "position": len(measureNotes), "value": '1'})
+            elif line['name'] == 'GOGOEND':
+                measureEvents.append({"name": 'gogo', "position": len(measureNotes), "value": '0'})
+            elif line['name'] == 'BARLINEON':
+                measureEvents.append({"name": 'barline', "position": len(measureNotes), "value": '1'})
+            elif line['name'] == 'BARLINEOFF':
+                measureEvents.append({"name": 'barline', "position": len(measureNotes), "value": '0'})
+            elif line['name'] == 'SCROLL':
+                measureEvents.append({"name": 'scroll', "position": len(measureNotes), "value": float(line['value'])})
+            elif line['name'] == 'BPMCHANGE':
+                measureEvents.append({"name": 'bpm', "position": len(measureNotes), "value": float(line['value'])})
+            elif line['name'] == 'MEASURE':
+                measureEvents.append({"name": 'measure', "position": len(measureNotes), "value": line['value']})
+
+            # Branch commands
+            elif line["name"] == 'START' or line['name'] == 'END':
+                if hasBranches:
+                    currentBranch = 'all'
+                    targetBranch = 'all'
+                else:
+                    currentBranch = 'normal'
+                    targetBranch = 'normal'
+                flagLevelhold = False
+            elif line['name'] == 'LEVELHOLD':
+                flagLevelhold = True
+            elif line["name"] == 'N':
+                currentBranch = 'normal'
+            elif line["name"] == 'E':
+                currentBranch = 'advanced'
+            elif line["name"] == 'M':
+                currentBranch = 'master'
+            elif line["name"] == 'BRANCHEND':
+                currentBranch = targetBranch
+            elif line["name"] == 'BRANCHSTART':
+                if flagLevelhold:
+                    continue
+                values = line['value'].split(',')
+                if values[0] == 'r':
+                    if len(values) >= 3:
+                        targetBranch = 'master'
+                    elif len(values) == 2:
+                        targetBranch = 'advanced'
+                    else:
+                        targetBranch = 'normal'
+                elif values[0] == 'p':  # p = percentage
+                    values[1] = float(values[1]) / 100  # %
+                    values[2] = float(values[2]) / 100  # %
+                    measureEvents.append({"name": 'branchStart', "position": len(measureNotes), "value": values})
+                    if len(values) >= 3 and float(values[2]) <= 100:
+                        targetBranch = 'master'
+                    elif len(values) >= 2 and float(values[1]) <= 100:
+                        targetBranch = 'advanced'
+                    else:
+                        targetBranch = 'normal'
+
+            # Ignored commands
+            elif line['name'] == 'LYRIC':
+                pass
+            elif line['name'] == 'NEXTSONG':
+                pass
+
+            # Not implemented commands
+            elif line['name'] == 'SECTION':
+                pass  # TODO: Implement
+            elif line['name'] == 'DELAY':
+                raise NotImplementedError
+            else:
+                raise NotImplementedError
+
+    # If there is measure data (i.e. the file doesn't end on a "measure end" symbol ','), append whatever is left
+    if measureNotes:
+        branches[currentBranch].append({
+            "data": measureNotes,
             "events": measureEvents,
         })
-
-    # Post-processing: Otherwise, if the file ends on a measure event (e.g. #GOGOEND), append any remaining events
+    # Otherwise, if the file ends on a measure event (e.g. #GOGOEND), append any remaining events
     elif measureEvents:
         for event in measureEvents:
-            event['position'] = len(measures[len(measures) - 1]['data'])
-            # noinspection PyTypeChecker
-            measures[len(measures) - 1]['events'].append(event)
-
-    return headers, measures
-
-
-def applyFumenStructureToParsedTJA(globalHeader, courseHeader, measures):
-    """Merge song metadata, course metadata, and course data into a single fumen-like object."""
-    song = {'measures': [], 'metadata': {}}
-
-    for k, v in globalHeader.items():
-        song['metadata'][k] = v
-
-    for k, v in courseHeader.items():
-        if k in ['scoreInit', 'scoreDiff']:
-            song[k] = v
-        else:
-            song['metadata'][k] = v
+            event['position'] = len(branches[len(branches) - 1]['data'])
+            branches[currentBranch][len(branches[currentBranch]) - 1]['events'].append(event)
 
-    for i, measure in enumerate(measures):
-        song['measures'].append(measure)
+    # Merge measure data and measure events in chronological order
+    for branchName, branch in branches.items():
+        for measure in branch:
+            notes = [{'pos': i, 'type': 'note', 'value': TJA_NOTE_TYPES[note]}
+                     for i, note in enumerate(measure['data']) if note != '0']
+            events = [{'pos': e['position'], 'type': e['name'], 'value': e['value']}
+                      for e in measure['events']]
+            combined = []
+            while notes or events:
+                if events and notes:
+                    if notes[0]['pos'] >= events[0]['pos']:
+                        combined.append(events.pop(0))
+                    else:
+                        combined.append(notes.pop(0))
+                elif events:
+                    combined.append(events.pop(0))
+                elif notes:
+                    combined.append(notes.pop(0))
+            measure['combined'] = combined
+
+    # Ensure all branches have the same number of measures
+    if hasBranches:
+        branch_lens = [len(b) for b in branches.values()]
+        if not branch_lens.count(branch_lens[0]) == len(branch_lens):
+            raise ValueError("Branches do not have the same number of measures.")
 
-    return song
+    return branches
 
 
 ########################################################################################################################
 # Fumen-parsing functions
 ########################################################################################################################
 
 # Fumen format reverse engineering TODOs
 # TODO: Figure out what drumroll bytes are (8 bytes after every drumroll)
 #       NB: fumen2osu.py assumed these were padding bytes, but they're not!! They contain some sort of metadata.
 # TODO: Figure out what the unknown Wii1, Wii4, and PS4 notes represent (just in case they're important somehow)
 
 
-def readFumen(fumenFile, byteOrder=None, debug=False):
+def readFumen(fumenFile, exclude_empty_measures=False):
     """
     Parse bytes of a fumen .bin file into nested measure, branch, and note dictionaries.
 
     For more information on any of the terms used in this function (e.g. scoreInit, scoreDiff),
     please refer to KatieFrog's excellent guide: https://gist.github.com/KatieFrogs/e000f406bbc70a12f3c34a07303eec8b
     """
-    if type(fumenFile) is str:
-        file = open(fumenFile, "rb")
-    else:
-        file = fumenFile
+    file = open(fumenFile, "rb")
     size = os.fstat(file.fileno()).st_size
 
     # Fetch the header bytes
     fumenHeader = file.read(512)
 
     # Determine:
     #   - The byte order (big or little endian)
     #   - The total number of measures from byte 0x200 (decimal 512)
-    if byteOrder:
-        order = ">" if byteOrder == "big" else "<"
-        totalMeasures = readStruct(file, order, format_string="I", seek=0x200)[0]
+    measuresBig = readStruct(file, order="", format_string=">I", seek=0x200)[0]
+    measuresLittle = readStruct(file, order="", format_string="<I", seek=0x200)[0]
+    if measuresBig < measuresLittle:
+        order = ">"
+        totalMeasures = measuresBig
     else:
-        # Use the number of measures to determine the byte order
-        measuresBig = readStruct(file, order="", format_string=">I", seek=0x200)[0]
-        measuresLittle = readStruct(file, order="", format_string="<I", seek=0x200)[0]
-        if measuresBig < measuresLittle:
-            order = ">"
-            totalMeasures = measuresBig
-        else:
-            order = "<"
-            totalMeasures = measuresLittle
+        order = "<"
+        totalMeasures = measuresLittle
 
     # Initialize the dict that will contain the chart information
     song = {'measures': []}
     song['headerPadding'] = fumenHeader[:432]
     song['headerMetadata'] = fumenHeader[-80:]
     song['order'] = order
-    song["length"] = totalMeasures
 
     # I am unsure what byte this represents
     unknownMetadata = readStruct(file, order, format_string="I", seek=0x204)[0]
     song["unknownMetadata"] = unknownMetadata
 
     # Determine whether the song has branches from byte 0x1b0 (decimal 432)
     hasBranches = getBool(readStruct(file, order, format_string="B", seek=0x1b0)[0])
     song["branches"] = hasBranches
 
-    # Print general debug metadata about the song
-    if debug:
-        debugPrint("Total measures: {0}, {1} branches, {2}-endian".format(
-            totalMeasures,
-            "has" if hasBranches else "no",
-            "Big" if order == ">" else "Little"
-        ))
-
     # Start reading measure data from position 0x208 (decimal 520)
     file.seek(0x208)
     for measureNumber in range(totalMeasures):
         # Parse the measure data using the following `format_string`:
         #   "ffBBHiiiiiii" (12 format characters, 40 bytes per measure)
         #     - 'f': BPM              (represented by one float (4 bytes))
         #     - 'f': fumenOffset      (represented by one float (4 bytes))
@@ -377,40 +328,16 @@
             # Create the branch dictionary using the newly-parsed branch data
             branch = {}
             totalNotes = branchStruct[0]
             branch["length"] = totalNotes
             branch["padding"] = branchStruct[1]
             branch["speed"] = branchStruct[2]
 
-            # Print debug metadata about the branches
-            if debug and (hasBranches or branchNumber == 0 or totalNotes != 0):
-                branchName = " ({0})".format(
-                    branchNames[branchNumber]
-                ) if hasBranches or branchNumber != 0 else ""
-                fileOffset = file.tell()
-                debugPrint("")
-                debugPrint("Measure #{0}{1} at {2}-{3} ({4})".format(
-                    measureNumber + 1,
-                    branchName,
-                    shortHex(fileOffset - 0x8),
-                    shortHex(fileOffset + 0x18 * totalNotes),
-                    nameValue(measure, branch)
-                ))
-                debugPrint("Total notes: {0}".format(totalNotes))
-
             # Iterate through each note in the measure (per branch)
             for noteNumber in range(totalNotes):
-                if debug:
-                    fileOffset = file.tell()
-                    debugPrint("Note #{0} at {1}-{2}".format(
-                        noteNumber + 1,
-                        shortHex(fileOffset),
-                        shortHex(fileOffset + 0x17)
-                    ), end="")
-
                 # Parse the note data using the following `format_string`:
                 #   "ififHHf" (7 format characters, 24 bytes per note cluster)
                 #     - 'i': note type
                 #     - 'f': note position
                 #     - 'i': item
                 #     - 'f': <padding>
                 #     - 'H': scoreInit
@@ -445,18 +372,14 @@
                         song["scoreDiff"] = note['scoreDiff']
                 if noteType == 0x6 or noteType == 0x9 or noteType == 0xa or noteType == 0xc:
                     # Drumroll and balloon duration in ms
                     note["duration"] = noteStruct[6]
                 else:
                     note['duration'] = noteStruct[6]
 
-                # Print debug information about the note
-                if debug:
-                    debugPrint(" ({0})".format(nameValue(note)))
-
                 # Seek forward 8 bytes to account for padding bytes at the end of drumrolls
                 if noteType == 0x6 or noteType == 0x9 or noteType == 0x62:
                     note["drumrollBytes"] = file.read(8)
 
                 # Assign the note to the branch
                 branch[noteNumber] = note
 
@@ -465,8 +388,17 @@
 
         # Assign the measure to the song
         song['measures'].append(measure)
         if file.tell() >= size:
             break
 
     file.close()
+
+    # NB: Official fumens often include empty measures as a way of inserting barlines for visual effect.
+    #     But, TJA authors tend not to add these empty measures, because even without them, the song plays correctly.
+    #     So, in tests, if we want to only compare the timing of the non-empty measures between an official fumen and
+    #     a converted non-official TJA, then it's useful to  exclude the empty measures.
+    if exclude_empty_measures:
+        song['measures'] = [m for m in song['measures']
+                            if m['normal']['length'] or m['advanced']['length'] or m['master']['length']]
+
     return song
```

### Comparing `tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Easy-1.csv` & `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Easy-1.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv` & `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv` & `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv` & `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Hard-3.csv` & `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Hard-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Hard-4.csv` & `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Hard-4.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv` & `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv` & `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Normal-3.csv` & `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Normal-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Normal-4.csv` & `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Normal-4.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv` & `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv` & `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Oni-8.csv` & `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Oni-8.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.1.1/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv` & `tja2fumen-0.2.0/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.1.1/src/tja2fumen/utils.py` & `tja2fumen-0.2.0/src/tja2fumen/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import sys
 import struct
 import csv
 
 
 def computeSoulGaugeBytes(n_notes, difficulty, stars):
     if difficulty in ['Oni', 'Ura']:
         if 9 <= stars:
@@ -89,25 +88,7 @@
 
 def getBool(number):
     return True if number == 0x1 else False if number == 0x0 else number
 
 
 def putBool(boolean):
     return 0x1 if boolean is True else 0x0 if boolean is False else boolean
-
-
-def nameValue(*lists):
-    string = []
-    for lst in lists:
-        for name in lst:
-            if name == "type":
-                string.append(lst[name])
-            elif name != "length" and type(name) is not int:
-                value = lst[name]
-                if type(value) == float and value % 1 == 0.0:
-                    value = int(value)
-                string.append("{0}: {1}".format(name, value))
-    return ", ".join(string)
-
-
-def debugPrint(*args, **kwargs):
-    print(*args, file=sys.stderr, **kwargs)
```

### Comparing `tja2fumen-0.1.1/src/tja2fumen/writers.py` & `tja2fumen-0.2.0/src/tja2fumen/writers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 from tja2fumen.utils import writeStruct, putBool
 from tja2fumen.constants import branchNames, typeNotes
 
 
-def writeFumen(file, song):
+def writeFumen(path_out, song):
     # Fetch the byte order (little/big endian)
     order = song['order']
 
     # Write the header
+    file = open(path_out, "wb")
     file.write(song['headerPadding'])   # Write header padding bytes
     file.write(song['headerMetadata'])  # Write header metadata bytes
 
     # Preallocate space in the file
     len_metadata = 8
     len_measures = 0
-    for measureNumber in range(song['length']):
+    for measureNumber in range(len(song['measures'])):
         len_measures += 40
         measure = song['measures'][measureNumber]
         for branchNumber in range(len(branchNames)):
             len_measures += 8
             branch = measure[branchNames[branchNumber]]
             for noteNumber in range(branch['length']):
                 len_measures += 24
                 note = branch[noteNumber]
                 if note['type'].lower() == "drumroll":
                     len_measures += 8
     file.write(b'\x00' * (len_metadata + len_measures))
 
     # Write metadata
     writeStruct(file, order, format_string="B", value_list=[putBool(song['branches'])], seek=0x1b0)
-    writeStruct(file, order, format_string="I", value_list=[song['length']], seek=0x200)
+    writeStruct(file, order, format_string="I", value_list=[len(song['measures'])], seek=0x200)
     writeStruct(file, order, format_string="I", value_list=[song['unknownMetadata']], seek=0x204)
 
     # Write measure data
     file.seek(0x208)
-    for measureNumber in range(song['length']):
+    for measureNumber in range(len(song['measures'])):
         measure = song['measures'][measureNumber]
         measureStruct = [measure['bpm'], measure['fumenOffset'], int(measure['gogo']), int(measure['barline'])]
         measureStruct.extend([measure['padding1']] + measure['branchInfo'] + [measure['padding2']])
         writeStruct(file, order, format_string="ffBBHiiiiiii", value_list=measureStruct)
 
         for branchNumber in range(len(branchNames)):
             branch = measure[branchNames[branchNumber]]
```

### Comparing `tja2fumen-0.1.1/src/tja2fumen.egg-info/PKG-INFO` & `tja2fumen-0.2.0/src/tja2fumen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.1.1
+Version: 0.2.0
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -25,15 +25,15 @@
         SOFTWARE.
 Project-URL: Homepage, https://github.com/vivaria/tja2fumen/
 Project-URL: Bug Reports, https://github.com/vivaria/tja2fumen/issues/
 Project-URL: Source, https://github.com/vivaria/tja2fumen/
 Keywords: taiko,tatsujin,fumen,TJA
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: build
+Provides-Extra: dev
 License-File: LICENSE.txt
 
 # tja2fumen
 
 `tja2fumen` is a tool for Taiko no Tatsujin games that allows you to convert TJA files (`.tja`) to fumen files (`.bin`).
 
 This project attempts to replace/complement the existing closed-source [tja2bin.exe](https://github.com/Fluto/TakoTako/blob/c269bcab60530877a16c2a473c84796b94d0a5ce/README.md?plain=1#L181) converter packaged alongside TakoTako.
```

### Comparing `tja2fumen-0.1.1/src/tja2fumen.egg-info/SOURCES.txt` & `tja2fumen-0.2.0/src/tja2fumen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

