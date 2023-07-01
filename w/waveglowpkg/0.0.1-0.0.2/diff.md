# Comparing `tmp/waveglowpkg-0.0.1.tar.gz` & `tmp/waveglowpkg-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waveglowpkg-0.0.1.tar", last modified: Sat Jul  1 13:35:32 2023, max compression
+gzip compressed data, was "waveglowpkg-0.0.2.tar", last modified: Sat Jul  1 13:56:29 2023, max compression
```

## Comparing `waveglowpkg-0.0.1.tar` & `waveglowpkg-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-01 13:35:32.733800 waveglowpkg-0.0.1/
--rw-r--r--   0 essam      (501) staff       (20)    11357 2023-06-18 07:29:29.000000 waveglowpkg-0.0.1/LICENSE
--rw-r--r--   0 essam      (501) staff       (20)      741 2023-07-01 13:35:32.733633 waveglowpkg-0.0.1/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)       38 2023-07-01 13:35:32.733856 waveglowpkg-0.0.1/setup.cfg
--rw-r--r--   0 essam      (501) staff       (20)     1608 2023-07-01 13:35:12.000000 waveglowpkg-0.0.1/setup.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-01 13:35:32.732454 waveglowpkg-0.0.1/waveglow/
--rw-r--r--   0 essam      (501) staff       (20)       92 2023-07-01 10:32:44.000000 waveglowpkg-0.0.1/waveglow/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)     1826 2023-07-01 10:30:29.000000 waveglowpkg-0.0.1/waveglow/convert_model.py
--rw-r--r--   0 essam      (501) staff       (20)    13756 2023-07-01 10:30:29.000000 waveglowpkg-0.0.1/waveglow/glow.py
--rw-r--r--   0 essam      (501) staff       (20)     2637 2023-07-01 10:32:59.000000 waveglowpkg-0.0.1/waveglow/inference.py
--rw-r--r--   0 essam      (501) staff       (20)     1013 2023-07-01 13:28:41.000000 waveglowpkg-0.0.1/waveglow/load.py
--rw-r--r--   0 essam      (501) staff       (20)     6042 2023-07-01 10:30:29.000000 waveglowpkg-0.0.1/waveglow/mel2samp.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-01 13:35:32.733271 waveglowpkg-0.0.1/waveglowpkg.egg-info/
--rw-r--r--   0 essam      (501) staff       (20)      741 2023-07-01 13:35:32.000000 waveglowpkg-0.0.1/waveglowpkg.egg-info/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)      314 2023-07-01 13:35:32.000000 waveglowpkg-0.0.1/waveglowpkg.egg-info/SOURCES.txt
--rw-r--r--   0 essam      (501) staff       (20)        1 2023-07-01 13:35:32.000000 waveglowpkg-0.0.1/waveglowpkg.egg-info/dependency_links.txt
--rw-r--r--   0 essam      (501) staff       (20)       39 2023-07-01 13:35:32.000000 waveglowpkg-0.0.1/waveglowpkg.egg-info/requires.txt
--rw-r--r--   0 essam      (501) staff       (20)        9 2023-07-01 13:35:32.000000 waveglowpkg-0.0.1/waveglowpkg.egg-info/top_level.txt
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-01 13:56:29.259201 waveglowpkg-0.0.2/
+-rw-r--r--   0 essam      (501) staff       (20)    11357 2023-06-18 07:29:29.000000 waveglowpkg-0.0.2/LICENSE
+-rw-r--r--   0 essam      (501) staff       (20)      741 2023-07-01 13:56:29.259046 waveglowpkg-0.0.2/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)       38 2023-07-01 13:56:29.259253 waveglowpkg-0.0.2/setup.cfg
+-rw-r--r--   0 essam      (501) staff       (20)     1608 2023-07-01 13:56:07.000000 waveglowpkg-0.0.2/setup.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-01 13:56:29.254726 waveglowpkg-0.0.2/waveglow/
+-rw-r--r--   0 essam      (501) staff       (20)       92 2023-07-01 10:32:44.000000 waveglowpkg-0.0.2/waveglow/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)     1826 2023-07-01 10:30:29.000000 waveglowpkg-0.0.2/waveglow/convert_model.py
+-rw-r--r--   0 essam      (501) staff       (20)    13756 2023-07-01 10:30:29.000000 waveglowpkg-0.0.2/waveglow/glow.py
+-rw-r--r--   0 essam      (501) staff       (20)     2637 2023-07-01 10:32:59.000000 waveglowpkg-0.0.2/waveglow/inference.py
+-rw-r--r--   0 essam      (501) staff       (20)     1060 2023-07-01 13:55:56.000000 waveglowpkg-0.0.2/waveglow/load.py
+-rw-r--r--   0 essam      (501) staff       (20)     6042 2023-07-01 10:30:29.000000 waveglowpkg-0.0.2/waveglow/mel2samp.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-01 13:56:29.258835 waveglowpkg-0.0.2/waveglowpkg.egg-info/
+-rw-r--r--   0 essam      (501) staff       (20)      741 2023-07-01 13:56:29.000000 waveglowpkg-0.0.2/waveglowpkg.egg-info/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)      314 2023-07-01 13:56:29.000000 waveglowpkg-0.0.2/waveglowpkg.egg-info/SOURCES.txt
+-rw-r--r--   0 essam      (501) staff       (20)        1 2023-07-01 13:56:29.000000 waveglowpkg-0.0.2/waveglowpkg.egg-info/dependency_links.txt
+-rw-r--r--   0 essam      (501) staff       (20)       39 2023-07-01 13:56:29.000000 waveglowpkg-0.0.2/waveglowpkg.egg-info/requires.txt
+-rw-r--r--   0 essam      (501) staff       (20)        9 2023-07-01 13:56:29.000000 waveglowpkg-0.0.2/waveglowpkg.egg-info/top_level.txt
```

### Comparing `waveglowpkg-0.0.1/LICENSE` & `waveglowpkg-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `waveglowpkg-0.0.1/PKG-INFO` & `waveglowpkg-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waveglowpkg
-Version: 0.0.1
+Version: 0.0.2
 Summary: WaveGlow model to generate audio from mel-spectrograms
 Home-page: https://waveglow.readthedocs.io/
 Author: Essam
 Author-email: essamwisam@outlook.com
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `waveglowpkg-0.0.1/setup.py` & `waveglowpkg-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         requirements = f.read().splitlines()
     return requirements
 
 
 # This call to setup() does all the work
 setup(
     name="waveglowpkg",
-    version="0.0.1",
+    version="0.0.2",
     description="WaveGlow model to generate audio from mel-spectrograms",
     long_description="WaveGlow for Botiverse Package",
     long_description_content_type="text/markdown",
     url="https://waveglow.readthedocs.io/",
     author="Essam",
     author_email="essamwisam@outlook.com",
     license="",
```

### Comparing `waveglowpkg-0.0.1/waveglow/convert_model.py` & `waveglowpkg-0.0.2/waveglow/convert_model.py`

 * *Files identical despite different names*

### Comparing `waveglowpkg-0.0.1/waveglow/glow.py` & `waveglowpkg-0.0.2/waveglow/glow.py`

 * *Files identical despite different names*

### Comparing `waveglowpkg-0.0.1/waveglow/inference.py` & `waveglowpkg-0.0.2/waveglow/inference.py`

 * *Files identical despite different names*

### Comparing `waveglowpkg-0.0.1/waveglow/load.py` & `waveglowpkg-0.0.2/waveglow/load.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
     curr_dir = os.path.dirname(os.path.abspath(__file__))
     waveglow_path = os.path.join(curr_dir, 'waveglow.pt')
     sys.path.insert(0, curr_dir)
     # see if waveglow.pt exists
     if not os.path.exists(waveglow_path) or download:
         # download waveglow.pt
+         print("Downloading WaveGlow Weights")
          f_id = '1UJ71BsMIO90LWokp2B84vOl7cvgpnkE4' 
          gdown.download(f'https://drive.google.com/uc?export=download&confirm=pbef&id={f_id}', waveglow_path, quiet=False)            
     
     wave_glow = torch.load(waveglow_path, map_location=device)['model']
     wave_glow = wave_glow.remove_weightnorm(wave_glow)
     
     if device == torch.device('cuda'):
```

### Comparing `waveglowpkg-0.0.1/waveglow/mel2samp.py` & `waveglowpkg-0.0.2/waveglow/mel2samp.py`

 * *Files identical despite different names*

### Comparing `waveglowpkg-0.0.1/waveglowpkg.egg-info/PKG-INFO` & `waveglowpkg-0.0.2/waveglowpkg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waveglowpkg
-Version: 0.0.1
+Version: 0.0.2
 Summary: WaveGlow model to generate audio from mel-spectrograms
 Home-page: https://waveglow.readthedocs.io/
 Author: Essam
 Author-email: essamwisam@outlook.com
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

