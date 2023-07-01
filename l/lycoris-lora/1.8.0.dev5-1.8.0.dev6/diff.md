# Comparing `tmp/lycoris_lora-1.8.0.dev5.tar.gz` & `tmp/lycoris_lora-1.8.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-1.8.0.dev5.tar", last modified: Sat Jul  1 12:35:34 2023, max compression
+gzip compressed data, was "lycoris_lora-1.8.0.dev6.tar", last modified: Sat Jul  1 13:34:49 2023, max compression
```

## Comparing `lycoris_lora-1.8.0.dev5.tar` & `lycoris_lora-1.8.0.dev6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 12:35:34.736917 lycoris_lora-1.8.0.dev5/
--rw-rw-rw-   0        0        0    11545 2023-06-04 13:36:43.000000 lycoris_lora-1.8.0.dev5/LICENSE.md
--rw-rw-rw-   0        0        0      353 2023-07-01 12:35:34.735918 lycoris_lora-1.8.0.dev5/PKG-INFO
--rw-rw-rw-   0        0        0     7677 2023-06-28 12:51:02.000000 lycoris_lora-1.8.0.dev5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 12:35:34.721911 lycoris_lora-1.8.0.dev5/lycoris/
--rw-rw-rw-   0        0        0        0 2023-07-01 11:57:57.000000 lycoris_lora-1.8.0.dev5/lycoris/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 12:35:34.722910 lycoris_lora-1.8.0.dev5/lycoris/kohya/
--rw-rw-rw-   0        0        0    24690 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev5/lycoris/kohya/__init__.py
--rw-rw-rw-   0        0        0    48868 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev5/lycoris/kohya/kohya_model_utils.py
--rw-rw-rw-   0        0        0     1512 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev5/lycoris/kohya/kohya_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-01 12:35:34.726914 lycoris_lora-1.8.0.dev5/lycoris/modules/
--rw-rw-rw-   0        0        0        0 2023-07-01 07:43:35.000000 lycoris_lora-1.8.0.dev5/lycoris/modules/__init__.py
--rw-rw-rw-   0        0        0     4762 2023-06-30 13:07:32.000000 lycoris_lora-1.8.0.dev5/lycoris/modules/dylora.py
--rw-rw-rw-   0        0        0     4117 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev5/lycoris/modules/glora.py
--rw-rw-rw-   0        0        0     2103 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev5/lycoris/modules/ia3.py
--rw-rw-rw-   0        0        0     4468 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev5/lycoris/modules/locon.py
--rw-rw-rw-   0        0        0     8831 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev5/lycoris/modules/loha.py
--rw-rw-rw-   0        0        0    10856 2023-06-30 13:57:07.000000 lycoris_lora-1.8.0.dev5/lycoris/modules/lokr.py
--rw-rw-rw-   0        0        0    20963 2023-06-04 13:36:43.000000 lycoris_lora-1.8.0.dev5/lycoris/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-01 12:35:34.735918 lycoris_lora-1.8.0.dev5/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      353 2023-07-01 12:35:34.000000 lycoris_lora-1.8.0.dev5/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      545 2023-07-01 12:35:34.000000 lycoris_lora-1.8.0.dev5/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 12:35:34.000000 lycoris_lora-1.8.0.dev5/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-04 13:39:16.000000 lycoris_lora-1.8.0.dev5/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-07-01 12:35:34.000000 lycoris_lora-1.8.0.dev5/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-01 12:35:34.000000 lycoris_lora-1.8.0.dev5/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 12:35:34.736917 lycoris_lora-1.8.0.dev5/setup.cfg
--rw-rw-rw-   0        0        0      566 2023-07-01 12:35:34.000000 lycoris_lora-1.8.0.dev5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 13:34:49.373167 lycoris_lora-1.8.0.dev6/
+-rw-rw-rw-   0        0        0    11545 2023-06-04 13:36:43.000000 lycoris_lora-1.8.0.dev6/LICENSE.md
+-rw-rw-rw-   0        0        0      353 2023-07-01 13:34:49.372142 lycoris_lora-1.8.0.dev6/PKG-INFO
+-rw-rw-rw-   0        0        0     7677 2023-06-28 12:51:02.000000 lycoris_lora-1.8.0.dev6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 13:34:49.357799 lycoris_lora-1.8.0.dev6/lycoris/
+-rw-rw-rw-   0        0        0        0 2023-07-01 11:57:57.000000 lycoris_lora-1.8.0.dev6/lycoris/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 13:34:49.359799 lycoris_lora-1.8.0.dev6/lycoris/kohya/
+-rw-rw-rw-   0        0        0    24690 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev6/lycoris/kohya/__init__.py
+-rw-rw-rw-   0        0        0    48868 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev6/lycoris/kohya/kohya_model_utils.py
+-rw-rw-rw-   0        0        0     1512 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev6/lycoris/kohya/kohya_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-01 13:34:49.363803 lycoris_lora-1.8.0.dev6/lycoris/modules/
+-rw-rw-rw-   0        0        0        0 2023-07-01 07:43:35.000000 lycoris_lora-1.8.0.dev6/lycoris/modules/__init__.py
+-rw-rw-rw-   0        0        0     4762 2023-06-30 13:07:32.000000 lycoris_lora-1.8.0.dev6/lycoris/modules/dylora.py
+-rw-rw-rw-   0        0        0     4117 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev6/lycoris/modules/glora.py
+-rw-rw-rw-   0        0        0     2103 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev6/lycoris/modules/ia3.py
+-rw-rw-rw-   0        0        0     4468 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev6/lycoris/modules/locon.py
+-rw-rw-rw-   0        0        0     8831 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev6/lycoris/modules/loha.py
+-rw-rw-rw-   0        0        0    10810 2023-07-01 13:34:19.000000 lycoris_lora-1.8.0.dev6/lycoris/modules/lokr.py
+-rw-rw-rw-   0        0        0    20963 2023-06-04 13:36:43.000000 lycoris_lora-1.8.0.dev6/lycoris/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-01 13:34:49.372142 lycoris_lora-1.8.0.dev6/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      353 2023-07-01 13:34:49.000000 lycoris_lora-1.8.0.dev6/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      545 2023-07-01 13:34:49.000000 lycoris_lora-1.8.0.dev6/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 13:34:49.000000 lycoris_lora-1.8.0.dev6/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-04 13:39:16.000000 lycoris_lora-1.8.0.dev6/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-07-01 13:34:49.000000 lycoris_lora-1.8.0.dev6/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-01 13:34:49.000000 lycoris_lora-1.8.0.dev6/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 13:34:49.373167 lycoris_lora-1.8.0.dev6/setup.cfg
+-rw-rw-rw-   0        0        0      566 2023-07-01 13:34:47.000000 lycoris_lora-1.8.0.dev6/setup.py
```

### Comparing `lycoris_lora-1.8.0.dev5/LICENSE.md` & `lycoris_lora-1.8.0.dev6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev5/README.md` & `lycoris_lora-1.8.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev5/lycoris/kohya/__init__.py` & `lycoris_lora-1.8.0.dev6/lycoris/kohya/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev5/lycoris/kohya/kohya_model_utils.py` & `lycoris_lora-1.8.0.dev6/lycoris/kohya/kohya_model_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev5/lycoris/kohya/kohya_utils.py` & `lycoris_lora-1.8.0.dev6/lycoris/kohya/kohya_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev5/lycoris/modules/dylora.py` & `lycoris_lora-1.8.0.dev6/lycoris/modules/dylora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev5/lycoris/modules/glora.py` & `lycoris_lora-1.8.0.dev6/lycoris/modules/glora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev5/lycoris/modules/ia3.py` & `lycoris_lora-1.8.0.dev6/lycoris/modules/ia3.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev5/lycoris/modules/locon.py` & `lycoris_lora-1.8.0.dev6/lycoris/modules/locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev5/lycoris/modules/loha.py` & `lycoris_lora-1.8.0.dev6/lycoris/modules/loha.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev5/lycoris/modules/lokr.py` & `lycoris_lora-1.8.0.dev6/lycoris/modules/lokr.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,14 @@
         else:
             torch.nn.init.normal_(self.lokr_w1_a, std=1)
             torch.nn.init.normal_(self.lokr_w1_b, std=0.1)
 
         self.multiplier = multiplier
         self.org_module = [org_module]
         weight = make_kron(
-            self.org_module[0].weight.data, 
             self.lokr_w1 if self.use_w1 else self.lokr_w1_a@self.lokr_w1_b,
             (self.lokr_w2 if self.use_w2 
              else make_weight_cp(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b) if self.cp 
              else self.lokr_w2_a@self.lokr_w2_b),
             torch.tensor(self.multiplier * self.scale)
         )
         assert torch.sum(torch.isnan(weight)) == 0, "weight is nan"
```

### Comparing `lycoris_lora-1.8.0.dev5/lycoris/utils.py` & `lycoris_lora-1.8.0.dev6/lycoris/utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev5/lycoris_lora.egg-info/SOURCES.txt` & `lycoris_lora-1.8.0.dev6/lycoris_lora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev5/setup.py` & `lycoris_lora-1.8.0.dev6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='lycoris_lora',
     packages=find_packages(),
-    version='1.8.0.dev5',
+    version='1.8.0.dev6',
     url='https://github.com/KohakuBlueleaf/LyCORIS',
     description='Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion',
     author='Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao',
     author_email='apolloyeh0123@gmail.com',
     zip_safe=False,
     install_requires=[
         'torch',
```

