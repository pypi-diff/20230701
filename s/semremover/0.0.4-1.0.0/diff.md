# Comparing `tmp/semremover-0.0.4.tar.gz` & `tmp/semremover-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semremover-0.0.4.tar", last modified: Wed Jun 21 06:07:43 2023, max compression
+gzip compressed data, was "semremover-1.0.0.tar", last modified: Sat Jul  1 15:11:39 2023, max compression
```

## Comparing `semremover-0.0.4.tar` & `semremover-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:07:43.439881 semremover-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-21 06:07:39.000000 semremover-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-21 06:07:43.439881 semremover-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-21 06:07:39.000000 semremover-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-21 06:07:41.000000 semremover-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:07:43.435881 semremover-0.0.4/semremover/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 06:07:39.000000 semremover-0.0.4/semremover/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-21 06:07:39.000000 semremover-0.0.4/semremover/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:07:43.435881 semremover-0.0.4/semremover/models/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-21 06:07:39.000000 semremover-0.0.4/semremover/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-21 06:07:39.000000 semremover-0.0.4/semremover/models/lama.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-21 06:07:39.000000 semremover-0.0.4/semremover/models/maskformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-21 06:07:39.000000 semremover-0.0.4/semremover/models/semremover.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-21 06:07:39.000000 semremover-0.0.4/semremover/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:07:43.435881 semremover-0.0.4/semremover.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-21 06:07:43.000000 semremover-0.0.4/semremover.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-21 06:07:43.000000 semremover-0.0.4/semremover.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 06:07:43.000000 semremover-0.0.4/semremover.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 06:07:43.000000 semremover-0.0.4/semremover.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 06:07:43.439881 semremover-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-21 06:07:39.000000 semremover-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:11:39.598241 semremover-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-01 15:11:36.000000 semremover-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-01 15:11:39.598241 semremover-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-01 15:11:36.000000 semremover-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-01 15:11:37.000000 semremover-1.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:11:39.598241 semremover-1.0.0/semremover/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-01 15:11:36.000000 semremover-1.0.0/semremover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-01 15:11:36.000000 semremover-1.0.0/semremover/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:11:39.598241 semremover-1.0.0/semremover/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-01 15:11:36.000000 semremover-1.0.0/semremover/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-01 15:11:36.000000 semremover-1.0.0/semremover/models/lama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-01 15:11:36.000000 semremover-1.0.0/semremover/models/maskformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-01 15:11:36.000000 semremover-1.0.0/semremover/models/semremover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-01 15:11:36.000000 semremover-1.0.0/semremover/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:11:39.598241 semremover-1.0.0/semremover.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-01 15:11:39.000000 semremover-1.0.0/semremover.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-01 15:11:39.000000 semremover-1.0.0/semremover.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 15:11:39.000000 semremover-1.0.0/semremover.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-01 15:11:39.000000 semremover-1.0.0/semremover.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 15:11:39.598241 semremover-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-01 15:11:36.000000 semremover-1.0.0/setup.py
```

### Comparing `semremover-0.0.4/LICENSE` & `semremover-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semremover-0.0.4/PKG-INFO` & `semremover-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semremover
-Version: 0.0.4
+Version: 1.0.0
 Summary: semantic object removal made easy.
 Author-email: Jesse Visser <jssvssr2000@gmail.com>
 Project-URL: Homepage, https://github.com/Jessseee/semantic-object-removal
 Project-URL: Bug Tracker, https://github.com/Jessseee/semantic-object-removal/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -41,15 +41,15 @@
 
 ### Usage
 To use the script you can call it with various options. The first positional argument is the input path, which can point to either an image or a directory of images. To remove objects from a picture add them to the labels option when running the script. The default labels can be found in `./semremover/models/config/ade20k_labels.json`.
 
 ### Example
 **input**
 ```
-    python -m semremover example/paris.jpg --labels car minibike van
+python -m semremover example/paris.jpg --labels car minibike van
 ```
 
 ![A picture of a street lined with cars in Paris.](https://github.com/Jessseee/semantic-object-removal/blob/main/example/paris.jpg?raw=true)
 
 **Output**
 
 ![A picture of the same street in paris with the cars digitally removed.](https://github.com/Jessseee/semantic-object-removal/blob/main/example/paris-inpainted.jpg?raw=true)
```

### Comparing `semremover-0.0.4/README.md` & `semremover-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 ### Usage
 To use the script you can call it with various options. The first positional argument is the input path, which can point to either an image or a directory of images. To remove objects from a picture add them to the labels option when running the script. The default labels can be found in `./semremover/models/config/ade20k_labels.json`.
 
 ### Example
 **input**
 ```
-    python -m semremover example/paris.jpg --labels car minibike van
+python -m semremover example/paris.jpg --labels car minibike van
 ```
 
 ![A picture of a street lined with cars in Paris.](https://github.com/Jessseee/semantic-object-removal/blob/main/example/paris.jpg?raw=true)
 
 **Output**
 
 ![A picture of the same street in paris with the cars digitally removed.](https://github.com/Jessseee/semantic-object-removal/blob/main/example/paris-inpainted.jpg?raw=true)
```

### Comparing `semremover-0.0.4/pyproject.toml` & `semremover-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "semremover"
-version = "0.0.4"
+version = "1.0.0"
 authors = [
   { name="Jesse Visser", email="jssvssr2000@gmail.com" },
 ]
 description = "semantic object removal made easy."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `semremover-0.0.4/semremover/__main__.py` & `semremover-1.0.0/semremover/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         help="Dilate kernel size.",
     )
     parser.add_argument(
         "--label_file", type=str, default=package_path("models/config/ade20k_labels.json"),
         help="The json file containing the output labels of the maskformer model"
     )
     parser.add_argument(
-        "--lama_ckpt", type=str, default=package_path("../models/weights/big-lama"),
+        "--lama_ckpt", type=str, default=package_path("models/weights/big-lama"),
         help="The path to the lama checkpoint.",
     )
     parser.add_argument(
         "--lama_config", type=str, default=package_path("models/config/lama_default.yaml"),
         help="The path to the config file of lama model.",
     )
     parser.add_argument(
@@ -77,12 +77,12 @@
         image_paths = [entry.path for entry in os.scandir(input_path) if entry.is_file()
                        and os.path.splitext(entry.name)[0] not in processed]
         if len(image_paths) == 0:
             print(f"There are no (unprocessed) files in {input_path}.")
             continue
         for image_path in tqdm(image_paths):
             inpainted_image = sem_obj_remover.remove_objects_from_image(image_path, args.labels, args.dilate_kernel_size)
-            save_image(inpainted_image, image_path, args.output_dir, args.output_type)
+            save_image(inpainted_image, args.output_dir, args.output_type)
     else:
         print(input_path)
         inpainted_image = sem_obj_remover.remove_objects_from_image(input_path, args.labels, args.dilate_kernel_size)
-        save_image(inpainted_image, input_path, args.output_dir, args.output_type)
+        save_image(inpainted_image, args.output_dir, args.output_type)
```

### Comparing `semremover-0.0.4/semremover/models/lama.py` & `semremover-1.0.0/semremover/models/lama.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from urllib.request import urlopen
 from zipfile import ZipFile
 import logging
 
 import yaml
 import torch
 import numpy as np
-from omegaconf import OmegaConf
+from omegaconf import OmegaConf, DictConfig
 
 log = logging.getLogger(__name__)
 
 os.environ['OMP_NUM_THREADS'] = '1'
 os.environ['OPENBLAS_NUM_THREADS'] = '1'
 os.environ['MKL_NUM_THREADS'] = '1'
 os.environ['VECLIB_MAXIMUM_THREADS'] = '1'
@@ -28,15 +28,15 @@
     def __init__(self, ckpt, config):
         if not os.path.exists(ckpt):
             log.warning(f"Could not find LaMa checkpoint at specified path.")
             ckpt = self.__download_lama_weights()
         self.model, self.config, self.device = self.__load_config(ckpt, config)
 
     @staticmethod
-    def __download_lama_weights():
+    def __download_lama_weights() -> str:
         ckpt_dir = package_path("models/weights/big-lama")
         ckpt_file = os.path.join(ckpt_dir, "models", "best.ckpt")
         config_file = os.path.join(ckpt_dir, "config.yaml")
         if os.path.exists(ckpt_file) and os.path.exists(config_file):
             log.info("Using default Big-LaMa weights.")
             return ckpt_dir
         os.makedirs(ckpt_dir, exist_ok=True)
@@ -44,15 +44,15 @@
         url = "https://github.com/Jessseee/lama/releases/latest/download/big-lama.zip"
         with urlopen(url) as zip_repr:
             with ZipFile(BytesIO(zip_repr.read())) as zip_file:
                 zip_file.extractall(ckpt_dir)
         return ckpt_dir
 
     @staticmethod
-    def __load_config(ckpt, config):
+    def __load_config(ckpt, config) -> tuple[torch.nn.Module, DictConfig, torch.device]:
         predict_config = OmegaConf.load(config)
         predict_config.model.input_path = ckpt
         device = torch.device("cuda")
         train_config_path = os.path.join(predict_config.model.input_path, 'config.yaml')
         with open(train_config_path, 'r') as f:
             train_config = OmegaConf.create(yaml.safe_load(f))
         train_config.training_model.predict_only = True
```

### Comparing `semremover-0.0.4/semremover/models/maskformer.py` & `semremover-1.0.0/semremover/models/maskformer.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class MaskFormer:
     def __init__(self, ckpt: str | os.PathLike, label_file: str | os.PathLike):
         self.model = MaskFormerForInstanceSegmentation.from_pretrained(ckpt)
         self.processor = MaskFormerImageProcessor()
         self.labels = json.load(open(label_file, "r"))
 
-    def segment(self, image: np.ndarray, to_select: list[str]):
+    def segment(self, image: np.ndarray, to_select: list[str]) -> tuple[np.ndarray, list[str]]:
         inputs = self.processor(images=image, return_tensors="pt")
         outputs = self.model(**inputs)
         batch_size = outputs.class_queries_logits.shape[0]
         outputs = self.processor.post_process_instance_segmentation(
             outputs,
             target_sizes=[image.shape[:2] for _ in range(batch_size)],
             return_binary_maps=True
```

### Comparing `semremover-0.0.4/semremover/models/semremover.py` & `semremover-1.0.0/semremover/models/semremover.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,41 +17,49 @@
     def __load_image_to_array(image_path: str | os.PathLike) -> np.ndarray:
         img = Image.open(image_path)
         if img.mode == "RGBA":
             img = img.convert("RGB")
         return np.array(img)
 
     @staticmethod
-    def __array_to_image(img_array: np.ndarray) -> Image:
-        return Image.fromarray(img_array.astype(np.uint8))
+    def __array_to_image(img_array: np.ndarray, input_path: str | os.PathLike) -> Image:
+        image = Image.fromarray(img_array.astype(np.uint8))
+        image.filename = os.path.split(input_path)[-1]
+        return image
 
     @staticmethod
     def __dilate_mask(mask: np.ndarray, dilate_factor: int = 15) -> np.ndarray:
         mask = mask.astype(np.uint8)
         mask = cv2.dilate(mask, np.ones((dilate_factor, dilate_factor), np.uint8), iterations=1)
         return mask
 
     def remove_objects_from_image(self, input_path: str | os.PathLike, labels: list[str], dilate_kernel_size: int = 15) -> Image:
-        """ Remove objects specified by labels from input image. """
+        """
+        Remove objects specified by labels from input image.
+        :param input_path: path to input image.
+        :param labels: labels of objects to remove.
+        :param dilate_kernel_size: the amount of pixels to dilate the mask.
+        :return: Image with objects removed.
+        """
         if not os.path.exists(input_path) or os.path.isdir(input_path):
             raise IOError(f"{input_path} is not a file.")
 
         # Load the image from file into ndarray
         image = self.__load_image_to_array(input_path)
 
         # Get masks from segmentation
         masks, labels = self.maskformer.segment(image, labels)
 
         # Save original image if no objects were found to remove
         if masks is None and labels is None:
-            return self.__array_to_image(image)
+            return self.__array_to_image(image, input_path)
 
         # Dilate mask to avoid unmasked edge effect
         if dilate_kernel_size > 0:
             masks = [self.__dilate_mask(mask, dilate_kernel_size) for mask in masks]
 
         # Loop over masks and do in-painting for each selected label
         for mask, label in zip(masks, labels):
             image = self.lama.inpaint(image, mask)
 
         # return final result
-        return self.__array_to_image(image)
+        return self.__array_to_image(image, input_path)
```

### Comparing `semremover-0.0.4/semremover.egg-info/PKG-INFO` & `semremover-1.0.0/semremover.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semremover
-Version: 0.0.4
+Version: 1.0.0
 Summary: semantic object removal made easy.
 Author-email: Jesse Visser <jssvssr2000@gmail.com>
 Project-URL: Homepage, https://github.com/Jessseee/semantic-object-removal
 Project-URL: Bug Tracker, https://github.com/Jessseee/semantic-object-removal/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -41,15 +41,15 @@
 
 ### Usage
 To use the script you can call it with various options. The first positional argument is the input path, which can point to either an image or a directory of images. To remove objects from a picture add them to the labels option when running the script. The default labels can be found in `./semremover/models/config/ade20k_labels.json`.
 
 ### Example
 **input**
 ```
-    python -m semremover example/paris.jpg --labels car minibike van
+python -m semremover example/paris.jpg --labels car minibike van
 ```
 
 ![A picture of a street lined with cars in Paris.](https://github.com/Jessseee/semantic-object-removal/blob/main/example/paris.jpg?raw=true)
 
 **Output**
 
 ![A picture of the same street in paris with the cars digitally removed.](https://github.com/Jessseee/semantic-object-removal/blob/main/example/paris-inpainted.jpg?raw=true)
```

