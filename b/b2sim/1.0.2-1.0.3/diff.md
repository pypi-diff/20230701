# Comparing `tmp/b2sim-1.0.2.tar.gz` & `tmp/b2sim-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2sim-1.0.2.tar", last modified: Sat Jul  1 20:21:17 2023, max compression
+gzip compressed data, was "b2sim-1.0.3.tar", last modified: Sat Jul  1 20:38:37 2023, max compression
```

## Comparing `b2sim-1.0.2.tar` & `b2sim-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-01 20:21:17.680006 b2sim-1.0.2/
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    35823 2023-05-09 05:51:58.000000 b2sim-1.0.2/LICENSE
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       87 2023-06-20 11:17:51.000000 b2sim-1.0.2/MANIFEST.in
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      274 2023-07-01 20:21:17.679004 b2sim-1.0.2/PKG-INFO
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    10205 2023-06-30 02:57:26.000000 b2sim-1.0.2/README.md
-drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-01 20:21:17.650967 b2sim-1.0.2/b2sim/
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       81 2023-06-20 01:13:34.000000 b2sim-1.0.2/b2sim/__init__.py
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     9099 2023-07-01 19:00:38.000000 b2sim-1.0.2/b2sim/actions.py
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     8686 2023-06-28 19:52:48.000000 b2sim-1.0.2/b2sim/info.py
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    97691 2023-07-01 20:11:44.000000 b2sim-1.0.2/b2sim/main.py
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     3673 2023-06-21 03:02:53.000000 b2sim-1.0.2/b2sim/rounds.py
-drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-01 20:21:17.678003 b2sim-1.0.2/b2sim/templates/
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     2027 2023-06-26 11:10:38.000000 b2sim-1.0.2/b2sim/templates/eco_send_info.csv
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      412 2023-06-19 10:21:44.000000 b2sim-1.0.2/b2sim/templates/nat_send_lengths.csv
-drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-01 20:21:17.665992 b2sim-1.0.2/b2sim.egg-info/
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      274 2023-07-01 20:21:17.000000 b2sim-1.0.2/b2sim.egg-info/PKG-INFO
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      332 2023-07-01 20:21:17.000000 b2sim-1.0.2/b2sim.egg-info/SOURCES.txt
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        1 2023-07-01 20:21:17.000000 b2sim-1.0.2/b2sim.egg-info/dependency_links.txt
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       24 2023-07-01 20:21:17.000000 b2sim-1.0.2/b2sim.egg-info/requires.txt
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        6 2023-07-01 20:21:17.000000 b2sim-1.0.2/b2sim.egg-info/top_level.txt
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       38 2023-07-01 20:21:17.680006 b2sim-1.0.2/setup.cfg
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      401 2023-07-01 18:08:56.000000 b2sim-1.0.2/setup.py
+drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-01 20:38:37.130669 b2sim-1.0.3/
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    35823 2023-05-09 05:51:58.000000 b2sim-1.0.3/LICENSE
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       87 2023-06-20 11:17:51.000000 b2sim-1.0.3/MANIFEST.in
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      274 2023-07-01 20:38:37.129668 b2sim-1.0.3/PKG-INFO
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    10205 2023-06-30 02:57:26.000000 b2sim-1.0.3/README.md
+drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-01 20:38:37.097654 b2sim-1.0.3/b2sim/
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       81 2023-06-20 01:13:34.000000 b2sim-1.0.3/b2sim/__init__.py
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     9099 2023-07-01 19:00:38.000000 b2sim-1.0.3/b2sim/actions.py
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     8686 2023-06-28 19:52:48.000000 b2sim-1.0.3/b2sim/info.py
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    97691 2023-07-01 20:11:44.000000 b2sim-1.0.3/b2sim/main.py
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     3673 2023-06-21 03:02:53.000000 b2sim-1.0.3/b2sim/rounds.py
+drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-01 20:38:37.106662 b2sim-1.0.3/b2sim/templates/
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     2027 2023-06-26 11:10:38.000000 b2sim-1.0.3/b2sim/templates/eco_send_info.csv
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      412 2023-06-19 10:21:44.000000 b2sim-1.0.3/b2sim/templates/nat_send_lengths.csv
+drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-01 20:38:37.104661 b2sim-1.0.3/b2sim.egg-info/
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      274 2023-07-01 20:38:37.000000 b2sim-1.0.3/b2sim.egg-info/PKG-INFO
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      332 2023-07-01 20:38:37.000000 b2sim-1.0.3/b2sim.egg-info/SOURCES.txt
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        1 2023-07-01 20:38:37.000000 b2sim-1.0.3/b2sim.egg-info/dependency_links.txt
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       24 2023-07-01 20:38:37.000000 b2sim-1.0.3/b2sim.egg-info/requires.txt
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        6 2023-07-01 20:38:37.000000 b2sim-1.0.3/b2sim.egg-info/top_level.txt
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       38 2023-07-01 20:38:37.131670 b2sim-1.0.3/setup.cfg
+-rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      401 2023-07-01 20:38:26.000000 b2sim-1.0.3/setup.py
```

### Comparing `b2sim-1.0.2/LICENSE` & `b2sim-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.2/README.md` & `b2sim-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.2/b2sim/actions.py` & `b2sim-1.0.3/b2sim/actions.py`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.2/b2sim/info.py` & `b2sim-1.0.3/b2sim/info.py`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.2/b2sim/main.py` & `b2sim-1.0.3/b2sim/main.py`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.2/b2sim/rounds.py` & `b2sim-1.0.3/b2sim/rounds.py`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.2/b2sim/templates/eco_send_info.csv` & `b2sim-1.0.3/b2sim/templates/eco_send_info.csv`

 * *Files identical despite different names*

