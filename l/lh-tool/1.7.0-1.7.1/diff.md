# Comparing `tmp/lh-tool-1.7.0.tar.gz` & `tmp/lh-tool-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lh-tool-1.7.0.tar", last modified: Sun Jun 11 04:57:35 2023, max compression
+gzip compressed data, was "lh-tool-1.7.1.tar", last modified: Sat Jul  1 02:52:44 2023, max compression
```

## Comparing `lh-tool-1.7.0.tar` & `lh-tool-1.7.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 04:57:35.486128 lh-tool-1.7.0/
--rw-rw-rw-   0        0        0     1091 2022-03-23 16:19:34.000000 lh-tool-1.7.0/LICENSE
--rw-rw-rw-   0        0        0     1105 2023-06-11 04:57:35.486128 lh-tool-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0      610 2023-06-11 04:50:22.000000 lh-tool-1.7.0/README.md
--rw-rw-rw-   0        0        0       86 2022-03-23 16:08:06.000000 lh-tool-1.7.0/pyproject.toml
--rw-rw-rw-   0        0        0     1312 2023-06-11 04:57:35.488124 lh-tool-1.7.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-11 04:57:35.446234 lh-tool-1.7.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 04:57:35.475158 lh-tool-1.7.0/src/lh_tool/
--rw-rw-rw-   0        0        0     2667 2022-03-23 16:05:06.000000 lh-tool-1.7.0/src/lh_tool/Email.py
--rw-rw-rw-   0        0        0    10678 2023-06-11 04:36:25.000000 lh-tool-1.7.0/src/lh_tool/Iterator.py
--rw-rw-rw-   0        0        0       23 2022-04-01 16:15:00.000000 lh-tool-1.7.0/src/lh_tool/__init__.py
--rw-rw-rw-   0        0        0     1326 2022-04-01 13:04:28.000000 lh-tool-1.7.0/src/lh_tool/compress_pdf.py
--rw-rw-rw-   0        0        0     4882 2023-02-12 01:05:19.000000 lh-tool-1.7.0/src/lh_tool/concat_image.py
--rw-rw-rw-   0        0        0     2342 2022-04-01 07:22:34.000000 lh-tool-1.7.0/src/lh_tool/excel2latex.py
--rw-rw-rw-   0        0        0     3093 2022-04-01 07:22:34.000000 lh-tool-1.7.0/src/lh_tool/excel2markdown.py
--rw-rw-rw-   0        0        0     2219 2023-02-12 01:05:19.000000 lh-tool-1.7.0/src/lh_tool/image2gif.py
--rw-rw-rw-   0        0        0     2651 2023-02-12 01:05:19.000000 lh-tool-1.7.0/src/lh_tool/image2image.py
--rw-rw-rw-   0        0        0     1387 2022-04-01 10:20:50.000000 lh-tool-1.7.0/src/lh_tool/image2pdf.py
--rw-rw-rw-   0        0        0     2966 2023-02-12 01:05:19.000000 lh-tool-1.7.0/src/lh_tool/image2video.py
--rw-rw-rw-   0        0        0     1425 2022-04-01 10:20:50.000000 lh-tool-1.7.0/src/lh_tool/pdf2image.py
--rw-rw-rw-   0        0        0     1142 2023-02-12 01:05:19.000000 lh-tool-1.7.0/src/lh_tool/play_image.py
--rw-rw-rw-   0        0        0     2247 2023-02-12 01:22:51.000000 lh-tool-1.7.0/src/lh_tool/rename_postfix.py
--rw-rw-rw-   0        0        0      670 2022-03-25 08:46:06.000000 lh-tool-1.7.0/src/lh_tool/startup.py
--rw-rw-rw-   0        0        0     2482 2023-02-12 01:05:19.000000 lh-tool-1.7.0/src/lh_tool/video2image.py
-drwxrwxrwx   0        0        0        0 2023-06-11 04:57:35.482138 lh-tool-1.7.0/src/lh_tool.egg-info/
--rw-rw-rw-   0        0        0     1105 2023-06-11 04:57:35.000000 lh-tool-1.7.0/src/lh_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      714 2023-06-11 04:57:35.000000 lh-tool-1.7.0/src/lh_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 04:57:35.000000 lh-tool-1.7.0/src/lh_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      519 2023-06-11 04:57:35.000000 lh-tool-1.7.0/src/lh_tool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       68 2023-06-11 04:57:35.000000 lh-tool-1.7.0/src/lh_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-11 04:57:35.000000 lh-tool-1.7.0/src/lh_tool.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-11 04:57:35.484133 lh-tool-1.7.0/tests/
--rw-rw-rw-   0        0        0      285 2022-04-01 03:54:12.000000 lh-tool-1.7.0/tests/test_email.py
--rw-rw-rw-   0        0        0     1404 2023-06-11 04:34:12.000000 lh-tool-1.7.0/tests/test_iterator.py
+drwxrwxrwx   0        0        0        0 2023-07-01 02:52:44.646420 lh-tool-1.7.1/
+-rw-rw-rw-   0        0        0     1091 2022-03-23 16:19:34.000000 lh-tool-1.7.1/LICENSE
+-rw-rw-rw-   0        0        0     1279 2023-07-01 02:52:44.646420 lh-tool-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0      784 2023-06-30 14:09:16.000000 lh-tool-1.7.1/README.md
+-rw-rw-rw-   0        0        0       86 2022-03-23 16:08:06.000000 lh-tool-1.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1312 2023-07-01 02:52:44.646420 lh-tool-1.7.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-01 02:52:44.601429 lh-tool-1.7.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-01 02:52:44.631423 lh-tool-1.7.1/src/lh_tool/
+-rw-rw-rw-   0        0        0     2667 2022-03-23 16:05:06.000000 lh-tool-1.7.1/src/lh_tool/Email.py
+-rw-rw-rw-   0        0        0    10627 2023-06-30 14:04:28.000000 lh-tool-1.7.1/src/lh_tool/Iterator.py
+-rw-rw-rw-   0        0        0       23 2022-04-01 16:15:00.000000 lh-tool-1.7.1/src/lh_tool/__init__.py
+-rw-rw-rw-   0        0        0     1326 2022-04-01 13:04:28.000000 lh-tool-1.7.1/src/lh_tool/compress_pdf.py
+-rw-rw-rw-   0        0        0     4882 2023-07-01 02:47:46.000000 lh-tool-1.7.1/src/lh_tool/concat_image.py
+-rw-rw-rw-   0        0        0     2342 2022-04-01 07:22:34.000000 lh-tool-1.7.1/src/lh_tool/excel2latex.py
+-rw-rw-rw-   0        0        0     3093 2022-04-01 07:22:34.000000 lh-tool-1.7.1/src/lh_tool/excel2markdown.py
+-rw-rw-rw-   0        0        0     2219 2023-02-12 01:05:19.000000 lh-tool-1.7.1/src/lh_tool/image2gif.py
+-rw-rw-rw-   0        0        0     2651 2023-02-12 01:05:19.000000 lh-tool-1.7.1/src/lh_tool/image2image.py
+-rw-rw-rw-   0        0        0     1387 2022-04-01 10:20:50.000000 lh-tool-1.7.1/src/lh_tool/image2pdf.py
+-rw-rw-rw-   0        0        0     2987 2023-07-01 02:47:57.000000 lh-tool-1.7.1/src/lh_tool/image2video.py
+-rw-rw-rw-   0        0        0     1425 2022-04-01 10:20:50.000000 lh-tool-1.7.1/src/lh_tool/pdf2image.py
+-rw-rw-rw-   0        0        0     1116 2023-07-01 02:42:10.000000 lh-tool-1.7.1/src/lh_tool/play_image.py
+-rw-rw-rw-   0        0        0     2247 2023-02-12 01:22:51.000000 lh-tool-1.7.1/src/lh_tool/rename_postfix.py
+-rw-rw-rw-   0        0        0      670 2022-03-25 08:46:06.000000 lh-tool-1.7.1/src/lh_tool/startup.py
+-rw-rw-rw-   0        0        0     2503 2023-07-01 02:47:57.000000 lh-tool-1.7.1/src/lh_tool/video2image.py
+drwxrwxrwx   0        0        0        0 2023-07-01 02:52:44.646420 lh-tool-1.7.1/src/lh_tool.egg-info/
+-rw-rw-rw-   0        0        0     1279 2023-07-01 02:52:44.000000 lh-tool-1.7.1/src/lh_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      714 2023-07-01 02:52:44.000000 lh-tool-1.7.1/src/lh_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 02:52:44.000000 lh-tool-1.7.1/src/lh_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      519 2023-07-01 02:52:44.000000 lh-tool-1.7.1/src/lh_tool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       68 2023-07-01 02:52:44.000000 lh-tool-1.7.1/src/lh_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-01 02:52:44.000000 lh-tool-1.7.1/src/lh_tool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 02:52:44.646420 lh-tool-1.7.1/tests/
+-rw-rw-rw-   0        0        0      285 2022-04-01 03:54:12.000000 lh-tool-1.7.1/tests/test_email.py
+-rw-rw-rw-   0        0        0     1404 2023-06-12 15:07:36.000000 lh-tool-1.7.1/tests/test_iterator.py
```

### Comparing `lh-tool-1.7.0/LICENSE` & `lh-tool-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lh-tool-1.7.0/setup.cfg` & `lh-tool-1.7.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 682d 746f 6f6c 0d0a 7665 7273   = lh-tool..vers
-00000020: 696f 6e20 3d20 312e 372e 300d 0a61 7574  ion = 1.7.0..aut
+00000020: 696f 6e20 3d20 312e 372e 310d 0a61 7574  ion = 1.7.1..aut
 00000030: 686f 7220 3d20 6c68 3931 3731 3333 380d  hor = lh9171338.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 6c69 6861 6f32 3031 3540 7768 752e 6564  lihao2015@whu.ed
 00000060: 752e 636e 0d0a 6465 7363 7269 7074 696f  u.cn..descriptio
 00000070: 6e20 3d20 4120 746f 6f6c 2070 6163 6b61  n = A tool packa
 00000080: 6765 0d0a 6c6f 6e67 5f64 6573 6372 6970  ge..long_descrip
 00000090: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
```

### Comparing `lh-tool-1.7.0/src/lh_tool/Email.py` & `lh-tool-1.7.1/src/lh_tool/Email.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.7.0/src/lh_tool/Iterator.py` & `lh-tool-1.7.1/src/lh_tool/Iterator.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,15 +234,17 @@
 
 class ParallelProcess(Iterator):
     """
     ParallelProcess
 
     """
 
-    def __init__(self, process, total=None, nprocs=multiprocessing.cpu_count(), **kwargs):
+    def __init__(
+        self, process, total=None, nprocs=multiprocessing.cpu_count(), **kwargs
+    ):
         super().__init__(process, total)
 
         self.nprocs = nprocs if nprocs > 0 else multiprocessing.cpu_count()
 
     def parse(self, *args, **kwargs):
         """parse"""
 
@@ -256,76 +258,79 @@
         # infer the number of expected iterations from kwargs
         if self.total is None:
             for _, value in kwargs.items():
                 if isinstance(value, list):
                     self.total = len(value)
                     break
 
-        assert self.total is not None, 'Can not infer the number of expected iterations'
+        assert self.total is not None, "Can not infer the number of expected iterations"
 
         # split tasks
-        indices = np.linspace(0, self.total, self.nprocs + 1).astype('int32')
+        indices = np.linspace(0, self.total, self.nprocs + 1).astype("int32")
 
         # parse args
         self.dynamic_args = [[] for _ in range(self.nprocs)]
         self.static_args = []
         for arg in args:
             if isinstance(arg, list):
-                assert len(arg) == self.total or len(
-                    arg) == self.nprocs, f'{len(arg)} != {self.total} or {len(arg)} != {self.nprocs}'
+                assert (
+                    len(arg) == self.total or len(arg) == self.nprocs
+                ), f"{len(arg)} != {self.total} or {len(arg)} != {self.nprocs}"
                 if len(arg) == self.nprocs:
                     for i in range(self.nprocs):
                         self.dynamic_args[i].append(arg[i])
                 else:
                     for i in range(self.nprocs):
-                        self.dynamic_args[i].append(arg[indices[i]:indices[i + 1]])
+                        self.dynamic_args[i].append(arg[indices[i] : indices[i + 1]])
             else:
                 self.static_args.append(arg)
 
         # parse kwargs
         self.dynamic_kwargs = [{} for _ in range(self.nprocs)]
         self.static_kwargs = {}
         for key, value in kwargs.items():
             if isinstance(value, list):
-                assert len(value) == self.total or len(
-                    value) == self.nprocs, f'{len(value)} != {self.total} or {len(value)} != {self.nprocs}'
+                assert (
+                    len(value) == self.total or len(value) == self.nprocs
+                ), f"{len(value)} != {self.total} or {len(value)} != {self.nprocs}"
                 if len(value) == self.nprocs:
                     for i in range(self.nprocs):
                         self.dynamic_kwargs[i][key] = value[i]
                 else:
                     for i in range(self.nprocs):
-                        self.dynamic_kwargs[i][key] = value[indices[i]:indices[i + 1]]
+                        self.dynamic_kwargs[i][key] = value[indices[i] : indices[i + 1]]
             else:
                 self.static_kwargs[key] = value
 
         # fix the static args
-        self.partial_func = functools.partial(self.func, *self.static_args, **self.static_kwargs)
+        self.partial_func = functools.partial(
+            self.func, *self.static_args, **self.static_kwargs
+        )
 
-    def __call__(self, dynamic_args, dynamic_kwargs, results_queue, idx):
+    def __call__(self, dynamic_args, dynamic_kwargs, results_dict, idx):
         res = self.partial_func(*dynamic_args, **dynamic_kwargs)
-        results_queue.put((idx, res))
+        results_dict[idx] = res
 
     def run(self, *args, **kwargs):
         """run - Please ensure that static arguments precede dynamic arguments"""
 
         # parse
         self.parse(*args, **kwargs)
 
         # run
         procs = []
-        results_queue = multiprocessing.Queue(self.nprocs)
+        manager = multiprocessing.Manager()
+        results_dict = manager.dict()
         for i in range(self.nprocs):
-            p = multiprocessing.Process(target=self, args=(self.dynamic_args[i], self.dynamic_kwargs[i], results_queue, i))
+            p = multiprocessing.Process(
+                target=self,
+                args=(self.dynamic_args[i], self.dynamic_kwargs[i], results_dict, i),
+            )
             procs.append(p)
             p.start()
 
-        ret_list, indices = [], []
-        for _ in tqdm.trange(self.nprocs, desc=self.func.__name__):
-            idx, res = results_queue.get()
-            indices.append(idx)
-            ret_list.append(res)
-        ret_list = [ret_list[idx] for idx in indices]
-
         for p in procs:
             p.join()
 
+        ret_list = [results_dict[idx] for idx in range(self.nprocs)]
+
         return ret_list
```

### Comparing `lh-tool-1.7.0/src/lh_tool/compress_pdf.py` & `lh-tool-1.7.1/src/lh_tool/compress_pdf.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.7.0/src/lh_tool/concat_image.py` & `lh-tool-1.7.1/src/lh_tool/concat_image.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.7.0/src/lh_tool/excel2latex.py` & `lh-tool-1.7.1/src/lh_tool/excel2latex.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.7.0/src/lh_tool/excel2markdown.py` & `lh-tool-1.7.1/src/lh_tool/excel2markdown.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.7.0/src/lh_tool/image2gif.py` & `lh-tool-1.7.1/src/lh_tool/image2gif.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.7.0/src/lh_tool/image2image.py` & `lh-tool-1.7.1/src/lh_tool/image2image.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.7.0/src/lh_tool/image2pdf.py` & `lh-tool-1.7.1/src/lh_tool/image2pdf.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.7.0/src/lh_tool/image2video.py` & `lh-tool-1.7.1/src/lh_tool/image2video.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import os
 import cv2
 import glob
 import tqdm
 import argparse
 from lh_tool.Iterator import SingleProcess, MultiProcess
-import imageio.v2 as iio
 
 
 def images2video(image_path, video_file, postfix, fourcc, fps, frameSize=None, speed=1):
     image_file_list = sorted(glob.glob(os.path.join(image_path, f'*.{postfix}')))
     if len(image_file_list) == 0:
         return
     video_file = os.path.abspath(image_path) + '.mp4' if video_file is None else video_file
 
     if frameSize is None:
-        image = iio.imread(image_file_list[0])
+        image = cv2.imread(image_file_list[0])
+        image = image[:, :, ::-1]   # RGB2BGR
         frameSize = (image.shape[1], image.shape[0])
     videoWriter = cv2.VideoWriter(video_file, fourcc, fps, frameSize)
     assert videoWriter.isOpened(), f'Failed to create file: {video_file}'
 
     image_file_list = [image_file_list[i] for i in range(0, len(image_file_list), speed)]
     for image_file in tqdm.tqdm(image_file_list, desc=video_file):
-        image = iio.imread(image_file)
+        image = cv2.imread(image_file)
         if frameSize != (image.shape[1], image.shape[0]):
             image = cv2.resize(image, tuple(frameSize))
         videoWriter.write(image)
     videoWriter.release()
 
 
 def main():
```

### Comparing `lh-tool-1.7.0/src/lh_tool/pdf2image.py` & `lh-tool-1.7.1/src/lh_tool/pdf2image.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.7.0/src/lh_tool/play_image.py` & `lh-tool-1.7.1/src/lh_tool/play_image.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import os
 import cv2
 import glob
 import tqdm
 import argparse
 import time
-import imageio.v2 as iio
 
 
 def play_image(image_file_list, fps):
     period = 1.0 / fps
     for image_file in tqdm.tqdm(image_file_list):
         start_time = time.time()
-        image = iio.imread(image_file)
+        image = cv2.imread(image_file)
         cv2.namedWindow('image', 0)
         cv2.imshow('image', image)
         current_time = time.time()
         delta_time = current_time - start_time
         sleep_time = max(1, int((period - delta_time) * 1000))
         cv2.waitKey(sleep_time)
```

### Comparing `lh-tool-1.7.0/src/lh_tool/rename_postfix.py` & `lh-tool-1.7.1/src/lh_tool/rename_postfix.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.7.0/src/lh_tool/startup.py` & `lh-tool-1.7.1/src/lh_tool/startup.py`

 * *Files identical despite different names*

### Comparing `lh-tool-1.7.0/src/lh_tool/video2image.py` & `lh-tool-1.7.1/src/lh_tool/video2image.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import cv2
 import glob
 import tqdm
 import argparse
 from lh_tool.Iterator import SingleProcess, MultiProcess
-import imageio.v2 as iio
 
 
 def video2images(video_file, image_path, postfix, frameSize=None):
     assert os.path.isfile(video_file), f'\'{video_file}\' is not a file'
     image_path = os.path.splitext(video_file)[0] if image_path is None else image_path
     os.makedirs(image_path, exist_ok=True)
 
@@ -18,16 +17,17 @@
     frame_count = int(videoCapture.get(cv2.CAP_PROP_FRAME_COUNT))
     for index in tqdm.trange(frame_count, desc=video_file):
         status, image = videoCapture.read()
         if not status:
             break
         if frameSize is not None:
             image = cv2.resize(image, tuple(frameSize))
+        image = image[:, :, ::-1]   # BGR2RGB
         image_file = os.path.join(image_path, f'{index + 1:06d}.{postfix}')
-        iio.imwrite(image_file, image)
+        cv2.imwrite(image_file, image)
 
     videoCapture.release()
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('-i', '--input', type=str, default='.', help='input video file or input path')
```

### Comparing `lh-tool-1.7.0/src/lh_tool.egg-info/SOURCES.txt` & `lh-tool-1.7.1/src/lh_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lh-tool-1.7.0/src/lh_tool.egg-info/entry_points.txt` & `lh-tool-1.7.1/src/lh_tool.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `lh-tool-1.7.0/tests/test_iterator.py` & `lh-tool-1.7.1/tests/test_iterator.py`

 * *Files identical despite different names*

