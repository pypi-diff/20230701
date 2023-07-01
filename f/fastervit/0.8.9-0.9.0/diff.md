# Comparing `tmp/fastervit-0.8.9.tar.gz` & `tmp/fastervit-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ali/Desktop/Gitlab_repos/FasterViT_pip_test/dist/.tmp-fhq3blvm/fastervit-0.8.9.tar", last modified: Fri Jun 23 00:41:06 2023, max compression
+gzip compressed data, was "/home/ali/Desktop/Gitlab_repos/FasterViT_pip_test/dist/.tmp-pdkhyeni/fastervit-0.9.0.tar", last modified: Sat Jul  1 03:59:10 2023, max compression
```

## Comparing `fastervit-0.8.9.tar` & `fastervit-0.9.0.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-23 00:41:06.000000 fastervit-0.8.9/
--rw-rw-r--   0 ali       (1000) ali       (1000)     4146 2023-06-21 01:30:26.000000 fastervit-0.8.9/LICENSE
--rw-rw-r--   0 ali       (1000) ali       (1000)       45 2023-06-21 01:30:26.000000 fastervit-0.8.9/MANIFEST.in
--rw-rw-r--   0 ali       (1000) ali       (1000)     9830 2023-06-23 00:41:06.000000 fastervit-0.8.9/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)     8880 2023-06-23 00:40:23.000000 fastervit-0.8.9/README.md
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-23 00:41:06.000000 fastervit-0.8.9/fastervit/
--rw-rw-r--   0 ali       (1000) ali       (1000)       41 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/__init__.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-23 00:41:06.000000 fastervit-0.8.9/fastervit/assets/
--rw-rw-r--   0 ali       (1000) ali       (1000)   100537 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/assets/hierarchial_attn.png
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-23 00:41:06.000000 fastervit-0.8.9/fastervit/models/
--rw-rw-r--   0 ali       (1000) ali       (1000)       96 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/models/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    47039 2023-06-23 00:32:18.000000 fastervit-0.8.9/fastervit/models/faster_vit.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    48796 2023-06-23 00:29:36.000000 fastervit-0.8.9/fastervit/models/faster_vit_any_res.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     7844 2023-06-21 01:32:20.000000 fastervit-0.8.9/fastervit/models/registry.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-23 00:41:06.000000 fastervit-0.8.9/fastervit/scheduler/
--rw-rw-r--   0 ali       (1000) ali       (1000)      291 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/scheduler/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     4161 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/scheduler/cosine_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     2098 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/scheduler/multistep_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3457 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/scheduler/plateau_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     4003 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/scheduler/poly_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     5095 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/scheduler/scheduler.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3907 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/scheduler/scheduler_factory.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1902 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/scheduler/step_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3936 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/scheduler/tanh_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      734 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/tensorboard.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    49797 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/train.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    16145 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/validate.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-23 00:41:06.000000 fastervit-0.8.9/fastervit.egg-info/
--rw-rw-r--   0 ali       (1000) ali       (1000)     9830 2023-06-23 00:41:06.000000 fastervit-0.8.9/fastervit.egg-info/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)      768 2023-06-23 00:41:06.000000 fastervit-0.8.9/fastervit.egg-info/SOURCES.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-06-23 00:41:06.000000 fastervit-0.8.9/fastervit.egg-info/dependency_links.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       32 2023-06-23 00:41:06.000000 fastervit-0.8.9/fastervit.egg-info/requires.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       10 2023-06-23 00:41:06.000000 fastervit-0.8.9/fastervit.egg-info/top_level.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)      126 2023-06-23 00:41:06.000000 fastervit-0.8.9/setup.cfg
--rw-rw-r--   0 ali       (1000) ali       (1000)     1549 2023-06-23 00:40:56.000000 fastervit-0.8.9/setup.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-01 03:59:10.000000 fastervit-0.9.0/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4146 2023-07-01 03:20:05.000000 fastervit-0.9.0/LICENSE
+-rw-rw-r--   0 ali       (1000) ali       (1000)       45 2023-07-01 03:20:05.000000 fastervit-0.9.0/MANIFEST.in
+-rw-rw-r--   0 ali       (1000) ali       (1000)    10793 2023-07-01 03:59:10.000000 fastervit-0.9.0/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)     9843 2023-07-01 03:36:57.000000 fastervit-0.9.0/README.md
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit/
+-rw-rw-r--   0 ali       (1000) ali       (1000)       41 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/__init__.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit/assets/
+-rw-rw-r--   0 ali       (1000) ali       (1000)   100537 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/assets/hierarchial_attn.png
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit/models/
+-rw-rw-r--   0 ali       (1000) ali       (1000)       96 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/models/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    42354 2023-07-01 03:28:20.000000 fastervit-0.9.0/fastervit/models/faster_vit.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    44191 2023-07-01 03:29:51.000000 fastervit-0.9.0/fastervit/models/faster_vit_any_res.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     7844 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/models/registry.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit/scheduler/
+-rw-rw-r--   0 ali       (1000) ali       (1000)      291 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/scheduler/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4161 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/scheduler/cosine_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     2098 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/scheduler/multistep_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3457 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/scheduler/plateau_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4003 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/scheduler/poly_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     5095 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/scheduler/scheduler.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3907 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/scheduler/scheduler_factory.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1902 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/scheduler/step_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3936 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/scheduler/tanh_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      734 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/tensorboard.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    49797 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/train.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit/utils/
+-rw-rw-r--   0 ali       (1000) ali       (1000)        0 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/utils/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4288 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/utils/checkpoint.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    19251 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/utils/datasets.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    16145 2023-07-01 03:20:05.000000 fastervit-0.9.0/fastervit/validate.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit.egg-info/
+-rw-rw-r--   0 ali       (1000) ali       (1000)    10793 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit.egg-info/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)      854 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit.egg-info/SOURCES.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit.egg-info/dependency_links.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       32 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit.egg-info/requires.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       10 2023-07-01 03:59:10.000000 fastervit-0.9.0/fastervit.egg-info/top_level.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)      126 2023-07-01 03:59:10.000000 fastervit-0.9.0/setup.cfg
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1549 2023-07-01 03:37:49.000000 fastervit-0.9.0/setup.py
```

### Comparing `fastervit-0.8.9/LICENSE` & `fastervit-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.9/PKG-INFO` & `fastervit-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastervit
-Version: 0.8.9
+Version: 0.9.0
 Summary: FasterViT: Fast Vision Transformers with Hierarchical Attention
 Home-page: https://github.com/NVlabs/FasterViT
 Author: Ali Hatamizadeh
 Author-email: ahatamiz123@gmail.com
 License: NVIDIA Source Code License-NC
 Keywords: pytorch pretrained models efficientnet mobilenetv3 mnasnet resnet vision transformer vit
 Classifier: Programming Language :: Python :: 3.7
@@ -41,27 +41,27 @@
 terms of accuracy vs. image throughput (no extra training data !)
 
 <p align="center">
 <img src="https://github.com/NVlabs/FasterViT/assets/26806394/253d1a2e-b5f5-4a9b-a362-6cdd16bfccc1" width=62% height=62% 
 class="center">
 </p>
 
-
-<!-- We introduce a new self-attention mechanism, denoted as Hierarchical
+We introduce a new self-attention mechanism, denoted as Hierarchical
 Attention (HAT), that captures both short and long-range information by learning
 cross-window carrier tokens.
 
-![teaser](./fastervit/assets/hierarchial_attn.png) -->
-
+![teaser](./fastervit/assets/hierarchial_attn.png)
 
-<!-- ## 💥 News 💥
+## 💥 News 💥
 
-- **[06.18.2023]** 🔥 We have released the FasterViT [pip package](https://pypi.org/project/fastervit/) !
-- **[06.17.2023]** 🔥 [Any-resolution FasterViT](./fastervit/models/faster_vit_any_res.py)  model is now available ! the model can be used for variety of applications such as detection and segmentation or high-resolution fine-tuning with arbitrary input image resolutions. 
-- **[06.09.2023]** 🔥🔥 We have released source code and ImageNet-1K FasterViT-models ! -->
+- **[06.30.2023]** 🔥🔥 We have further improved the [Any-resolution FasterViT](https://developer.nvidia.com/tensorrt-getting-started) throughput of FasterViT models by 10-15% on average across different models.  
+- **[06.29.2023]** 🔥 Any-resolution FasterViT model can now be intitialized from pre-trained ImageNet resolution (224 x 244) models.
+- **[06.18.2023]** We have released the FasterViT [pip package](https://pypi.org/project/fastervit/) !
+- **[06.17.2023]** 🔥 [Any-resolution FasterViT](./fastervit/models/faster_vit_any_res.py)  model is now available ! the model can be used for variety of applications such as detection and segmentation or high-resolution fine-tuning with arbitrary input image resolutions.
+- **[06.09.2023]** 🔥🔥 We have released source code and ImageNet-1K FasterViT-models !
 
 ## Quick Start
 
 The FasterViT can be conveniently installed by:
 
 ```bash
 pip install fastervit
@@ -87,24 +87,26 @@
 >>> model = create_model('faster_vit_1_any_res', 
                           resolution=[576, 960],
                           window_size=[7, 7, 12, 6],
                           ct_size=2,
                           dim=128)
 ```
 
-<!-- ## Catalog
+## Catalog
 - [x] ImageNet-1K training code
 - [x] ImageNet-1K pre-trained models
 - [x] Any-resolution FasterViT
 - [x] FasterViT pip-package release
-- [ ] Update training scripts to support model.compile, 
+- [x] Add capablity to initialize any-resolution FasterViT from ImageNet-pretrained weights. 
+- [ ] Update training scripts to support model.compile
+- [ ] Add isotropic FasterViT
 - [ ] ImageNet-21K pre-trained models
 - [ ] ImageNet-21K fine-tune scripts
 - [ ] Detection code (DINO) + models
-- [ ] Segmentation code + models -->
+- [ ] Segmentation code + models
 
 --- 
 
 ## Results + Pretrained Models
 
 ### ImageNet-1K
 **FasterViT ImageNet-1K Pretrained Models**
@@ -302,46 +304,60 @@
 --checkpoint <checkpoint-path>
 --data_dir <imagenet-path>
 --batch-size <batch-size-per-gpu
 ``` 
 
 Here `--model` is the FasterViT variant (e.g. `faster_vit_0_224_1k`), `--checkpoint` is the path to pretrained model weights, `--data_dir` is the path to ImageNet-1K validation set and `--batch-size` is the number of batch size. We also provide a sample script [here](./fastervit/validate.sh). 
 
+## ONNX Conversion
+
+We provide ONNX conversion script to enable dynamic batch size inference. For instance, to generate ONNX model for `faster_vit_0_any_res` with resolution 576 x 960 and ONNX opset number 17, the following can be used. 
+
+```bash 
+python onnx_convert --model-name faster_vit_0_any_res --resolution-h 576 --resolution-w 960 --onnx-opset 17
+
+```
+
 
 ## Installation
 
 The dependencies can be installed by running:
 
 ```bash
 pip install -r requirements.txt
 ```
 
-## Third-party Extentions
-We always welcome third-party extentions/implementations and usage for other purposes. If you would like your work to be listed in this repository, please raise and issue and provide us with detailed information.  
+## Star History
 
+[![Star History Chart](https://api.star-history.com/svg?repos=NVlabs/FasterViT&type=Date)](https://star-history.com/#NVlabs/FasterViT&Date)
 
-## Acknowledgement
-This repository is built on top of the [timm](https://github.com/huggingface/pytorch-image-models) repository. We thank [Ross Wrightman](https://rwightman.com/) for creating and maintaining this high-quality library.  
+
+## Third-party Extentions
+We always welcome third-party extentions/implementations and usage for other purposes. If you would like your work to be listed in this repository, please raise and issue and provide us with detailed information.  
 
 ## Citation
 
-Please consider citing FasterViT if this repository is useful for your work:
+Please consider citing FasterViT if this repository is useful for your work. 
 
 ```
 @article{hatamizadeh2023fastervit,
   title={FasterViT: Fast Vision Transformers with Hierarchical Attention},
   author={Hatamizadeh, Ali and Heinrich, Greg and Yin, Hongxu and Tao, Andrew and Alvarez, Jose M and Kautz, Jan and Molchanov, Pavlo},
   journal={arXiv preprint arXiv:2306.06189},
   year={2023}
 }
 ```
 
+
 ## Licenses
 
 Copyright © 2023, NVIDIA Corporation. All rights reserved.
 
 This work is made available under the NVIDIA Source Code License-NC. Click [here](LICENSE) to view a copy of this license.
 
 For license information regarding the timm repository, please refer to its [repository](https://github.com/rwightman/pytorch-image-models).
 
 For license information regarding the ImageNet dataset, please see the [ImageNet official website](https://www.image-net.org/). 
 
+## Acknowledgement
+This repository is built on top of the [timm](https://github.com/huggingface/pytorch-image-models) repository. We thank [Ross Wrightman](https://rwightman.com/) for creating and maintaining this high-quality library.  
+
```

### Comparing `fastervit-0.8.9/README.md` & `fastervit-0.9.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -19,27 +19,27 @@
 terms of accuracy vs. image throughput (no extra training data !)
 
 <p align="center">
 <img src="https://github.com/NVlabs/FasterViT/assets/26806394/253d1a2e-b5f5-4a9b-a362-6cdd16bfccc1" width=62% height=62% 
 class="center">
 </p>
 
-
-<!-- We introduce a new self-attention mechanism, denoted as Hierarchical
+We introduce a new self-attention mechanism, denoted as Hierarchical
 Attention (HAT), that captures both short and long-range information by learning
 cross-window carrier tokens.
 
-![teaser](./fastervit/assets/hierarchial_attn.png) -->
-
+![teaser](./fastervit/assets/hierarchial_attn.png)
 
-<!-- ## 💥 News 💥
+## 💥 News 💥
 
-- **[06.18.2023]** 🔥 We have released the FasterViT [pip package](https://pypi.org/project/fastervit/) !
-- **[06.17.2023]** 🔥 [Any-resolution FasterViT](./fastervit/models/faster_vit_any_res.py)  model is now available ! the model can be used for variety of applications such as detection and segmentation or high-resolution fine-tuning with arbitrary input image resolutions. 
-- **[06.09.2023]** 🔥🔥 We have released source code and ImageNet-1K FasterViT-models ! -->
+- **[06.30.2023]** 🔥🔥 We have further improved the [Any-resolution FasterViT](https://developer.nvidia.com/tensorrt-getting-started) throughput of FasterViT models by 10-15% on average across different models.  
+- **[06.29.2023]** 🔥 Any-resolution FasterViT model can now be intitialized from pre-trained ImageNet resolution (224 x 244) models.
+- **[06.18.2023]** We have released the FasterViT [pip package](https://pypi.org/project/fastervit/) !
+- **[06.17.2023]** 🔥 [Any-resolution FasterViT](./fastervit/models/faster_vit_any_res.py)  model is now available ! the model can be used for variety of applications such as detection and segmentation or high-resolution fine-tuning with arbitrary input image resolutions.
+- **[06.09.2023]** 🔥🔥 We have released source code and ImageNet-1K FasterViT-models !
 
 ## Quick Start
 
 The FasterViT can be conveniently installed by:
 
 ```bash
 pip install fastervit
@@ -65,24 +65,26 @@
 >>> model = create_model('faster_vit_1_any_res', 
                           resolution=[576, 960],
                           window_size=[7, 7, 12, 6],
                           ct_size=2,
                           dim=128)
 ```
 
-<!-- ## Catalog
+## Catalog
 - [x] ImageNet-1K training code
 - [x] ImageNet-1K pre-trained models
 - [x] Any-resolution FasterViT
 - [x] FasterViT pip-package release
-- [ ] Update training scripts to support model.compile, 
+- [x] Add capablity to initialize any-resolution FasterViT from ImageNet-pretrained weights. 
+- [ ] Update training scripts to support model.compile
+- [ ] Add isotropic FasterViT
 - [ ] ImageNet-21K pre-trained models
 - [ ] ImageNet-21K fine-tune scripts
 - [ ] Detection code (DINO) + models
-- [ ] Segmentation code + models -->
+- [ ] Segmentation code + models
 
 --- 
 
 ## Results + Pretrained Models
 
 ### ImageNet-1K
 **FasterViT ImageNet-1K Pretrained Models**
@@ -280,46 +282,60 @@
 --checkpoint <checkpoint-path>
 --data_dir <imagenet-path>
 --batch-size <batch-size-per-gpu
 ``` 
 
 Here `--model` is the FasterViT variant (e.g. `faster_vit_0_224_1k`), `--checkpoint` is the path to pretrained model weights, `--data_dir` is the path to ImageNet-1K validation set and `--batch-size` is the number of batch size. We also provide a sample script [here](./fastervit/validate.sh). 
 
+## ONNX Conversion
+
+We provide ONNX conversion script to enable dynamic batch size inference. For instance, to generate ONNX model for `faster_vit_0_any_res` with resolution 576 x 960 and ONNX opset number 17, the following can be used. 
+
+```bash 
+python onnx_convert --model-name faster_vit_0_any_res --resolution-h 576 --resolution-w 960 --onnx-opset 17
+
+```
+
 
 ## Installation
 
 The dependencies can be installed by running:
 
 ```bash
 pip install -r requirements.txt
 ```
 
-## Third-party Extentions
-We always welcome third-party extentions/implementations and usage for other purposes. If you would like your work to be listed in this repository, please raise and issue and provide us with detailed information.  
+## Star History
 
+[![Star History Chart](https://api.star-history.com/svg?repos=NVlabs/FasterViT&type=Date)](https://star-history.com/#NVlabs/FasterViT&Date)
 
-## Acknowledgement
-This repository is built on top of the [timm](https://github.com/huggingface/pytorch-image-models) repository. We thank [Ross Wrightman](https://rwightman.com/) for creating and maintaining this high-quality library.  
+
+## Third-party Extentions
+We always welcome third-party extentions/implementations and usage for other purposes. If you would like your work to be listed in this repository, please raise and issue and provide us with detailed information.  
 
 ## Citation
 
-Please consider citing FasterViT if this repository is useful for your work:
+Please consider citing FasterViT if this repository is useful for your work. 
 
 ```
 @article{hatamizadeh2023fastervit,
   title={FasterViT: Fast Vision Transformers with Hierarchical Attention},
   author={Hatamizadeh, Ali and Heinrich, Greg and Yin, Hongxu and Tao, Andrew and Alvarez, Jose M and Kautz, Jan and Molchanov, Pavlo},
   journal={arXiv preprint arXiv:2306.06189},
   year={2023}
 }
 ```
 
+
 ## Licenses
 
 Copyright © 2023, NVIDIA Corporation. All rights reserved.
 
 This work is made available under the NVIDIA Source Code License-NC. Click [here](LICENSE) to view a copy of this license.
 
 For license information regarding the timm repository, please refer to its [repository](https://github.com/rwightman/pytorch-image-models).
 
 For license information regarding the ImageNet dataset, please see the [ImageNet official website](https://www.image-net.org/). 
 
+## Acknowledgement
+This repository is built on top of the [timm](https://github.com/huggingface/pytorch-image-models) repository. We thank [Ross Wrightman](https://rwightman.com/) for creating and maintaining this high-quality library.  
+
```

#### html2text {}

```diff
@@ -8,26 +8,46 @@
 Kautz](https://jankautz.com/), [Pavlo Molchanov](https://www.pmolchanov.com/).
 For business inquiries, please visit our website and submit the form: [NVIDIA
 Research Licensing](https://www.nvidia.com/en-us/research/inquiries/) --
 - FasterViT achieves a new SOTA Pareto-front in terms of accuracy vs. image
 throughput (no extra training data !)
  [https://github.com/NVlabs/FasterViT/assets/26806394/253d1a2e-b5f5-4a9b-a362-
                                  6cdd16bfccc1]
-  ## Quick Start The FasterViT can be conveniently installed by: ```bash pip
-install fastervit ``` A FasterViT model with default hyper-parameters can be
-created as in the following: ```python >>> from fastervit import create_model #
-Define fastervit-0 model with 224 x 224 resolution >>> model = create_model
-('faster_vit_0_224') ``` We can also use the any-resolution FasterViT model to
-accommodate arbitrary image resolutions. In the following, we define an any-
-resolution FasterViT-1 model with input resolution of 576 x 960, window sizes
-of 12 and 6 in 3rd and 4th stages, carrier token size of 2 and embedding
-dimension of 128: ```python >>> from fastervit import create_model # Define
-any-resolution FasterViT-1 model with 576 x 960 resolution >>> model =
-create_model('faster_vit_1_any_res', resolution=[576, 960], window_size=[7, 7,
-12, 6], ct_size=2, dim=128) ```  --- ## Results + Pretrained Models ###
+We introduce a new self-attention mechanism, denoted as Hierarchical Attention
+(HAT), that captures both short and long-range information by learning cross-
+window carrier tokens. ![teaser](./fastervit/assets/hierarchial_attn.png) ##
+ð¥ News ð¥ - **[06.30.2023]** ð¥ð¥ We have further improved the [Any-
+resolution FasterViT](https://developer.nvidia.com/tensorrt-getting-started)
+throughput of FasterViT models by 10-15% on average across different models. -
+**[06.29.2023]** ð¥ Any-resolution FasterViT model can now be intitialized
+from pre-trained ImageNet resolution (224 x 244) models. - **[06.18.2023]** We
+have released the FasterViT [pip package](https://pypi.org/project/fastervit/
+) ! - **[06.17.2023]** ð¥ [Any-resolution FasterViT](./fastervit/models/
+faster_vit_any_res.py) model is now available ! the model can be used for
+variety of applications such as detection and segmentation or high-resolution
+fine-tuning with arbitrary input image resolutions. - **[06.09.2023]** ð¥ð¥
+We have released source code and ImageNet-1K FasterViT-models ! ## Quick Start
+The FasterViT can be conveniently installed by: ```bash pip install fastervit
+``` A FasterViT model with default hyper-parameters can be created as in the
+following: ```python >>> from fastervit import create_model # Define fastervit-
+0 model with 224 x 224 resolution >>> model = create_model('faster_vit_0_224')
+``` We can also use the any-resolution FasterViT model to accommodate arbitrary
+image resolutions. In the following, we define an any-resolution FasterViT-
+1 model with input resolution of 576 x 960, window sizes of 12 and 6 in 3rd and
+4th stages, carrier token size of 2 and embedding dimension of 128: ```python
+>>> from fastervit import create_model # Define any-resolution FasterViT-
+1 model with 576 x 960 resolution >>> model = create_model
+('faster_vit_1_any_res', resolution=[576, 960], window_size=[7, 7, 12, 6],
+ct_size=2, dim=128) ``` ## Catalog - [x] ImageNet-1K training code - [x]
+ImageNet-1K pre-trained models - [x] Any-resolution FasterViT - [x] FasterViT
+pip-package release - [x] Add capablity to initialize any-resolution FasterViT
+from ImageNet-pretrained weights. - [ ] Update training scripts to support
+model.compile - [ ] Add isotropic FasterViT - [ ] ImageNet-21K pre-trained
+models - [ ] ImageNet-21K fine-tune scripts - [ ] Detection code (DINO) +
+models - [ ] Segmentation code + models --- ## Results + Pretrained Models ###
 ImageNet-1K **FasterViT ImageNet-1K Pretrained Models**
 Name       Acc@1(%) Acc@5(%) Throughput Resolution #Params(M) FLOPs(G) Download
                              (Img/Sec)
 FasterViT- 82.1     95.9     5802       224x224    31.4       3.3      model
 0
 FasterViT- 83.2     96.5     4188       224x224    53.4       5.3      model
 1
@@ -56,27 +76,34 @@
 Training Please see [TRAINING.md](TRAINING.md) for detailed training
 instructions of all models. ## Evaluation The FasterViT models can be evaluated
 on ImageNet-1K validation set using the following: ``` python validate.py \ --
 model  --checkpoint  --data_dir  --batch-size
 `` Here `--model` is the FasterViT variant (e.g. `faster_vit_0_224_1k`), `--
 checkpoint` is the path to pretrained model weights, `--data_dir` is the path
 to ImageNet-1K validation set and `--batch-size` is the number of batch size.
-We also provide a sample script [here](./fastervit/validate.sh). ##
-Installation The dependencies can be installed by running: ```bash pip install
--r requirements.txt ``` ## Third-party Extentions We always welcome third-party
+We also provide a sample script [here](./fastervit/validate.sh). ## ONNX
+Conversion We provide ONNX conversion script to enable dynamic batch size
+inference. For instance, to generate ONNX model for `faster_vit_0_any_res` with
+resolution 576 x 960 and ONNX opset number 17, the following can be used.
+```bash python onnx_convert --model-name faster_vit_0_any_res --resolution-
+h 576 --resolution-w 960 --onnx-opset 17 ``` ## Installation The dependencies
+can be installed by running: ```bash pip install -r requirements.txt ``` ##
+Star History [![Star History Chart](https://api.star-history.com/
+svg?repos=NVlabs/FasterViT&type=Date)](https://star-history.com/#NVlabs/
+FasterViT&Date) ## Third-party Extentions We always welcome third-party
 extentions/implementations and usage for other purposes. If you would like your
 work to be listed in this repository, please raise and issue and provide us
-with detailed information. ## Acknowledgement This repository is built on top
-of the [timm](https://github.com/huggingface/pytorch-image-models) repository.
-We thank [Ross Wrightman](https://rwightman.com/) for creating and maintaining
-this high-quality library. ## Citation Please consider citing FasterViT if this
-repository is useful for your work: ``` @article{hatamizadeh2023fastervit,
+with detailed information. ## Citation Please consider citing FasterViT if this
+repository is useful for your work. ``` @article{hatamizadeh2023fastervit,
 title={FasterViT: Fast Vision Transformers with Hierarchical Attention},
 author={Hatamizadeh, Ali and Heinrich, Greg and Yin, Hongxu and Tao, Andrew and
 Alvarez, Jose M and Kautz, Jan and Molchanov, Pavlo}, journal={arXiv preprint
 arXiv:2306.06189}, year={2023} } ``` ## Licenses Copyright Â© 2023, NVIDIA
 Corporation. All rights reserved. This work is made available under the NVIDIA
 Source Code License-NC. Click [here](LICENSE) to view a copy of this license.
 For license information regarding the timm repository, please refer to its
 [repository](https://github.com/rwightman/pytorch-image-models). For license
 information regarding the ImageNet dataset, please see the [ImageNet official
-website](https://www.image-net.org/).
+website](https://www.image-net.org/). ## Acknowledgement This repository is
+built on top of the [timm](https://github.com/huggingface/pytorch-image-models)
+repository. We thank [Ross Wrightman](https://rwightman.com/) for creating and
+maintaining this high-quality library.
```

### Comparing `fastervit-0.8.9/fastervit/assets/hierarchial_attn.png` & `fastervit-0.9.0/fastervit/assets/hierarchial_attn.png`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.9/fastervit/models/faster_vit.py` & `fastervit-0.9.0/fastervit/models/faster_vit.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,158 +75,26 @@
     return x
 
 
 def ct_dewindow(ct, W, H, window_size):
     bs = ct.shape[0]
     N=ct.shape[2]
     ct2 = ct.view(-1, W//window_size, H//window_size, window_size, window_size, N).permute(0, 5, 1, 3, 2, 4)
-    ct2 = ct2.reshape(bs, N, W, H).flatten(2).transpose(1, 2)
+    ct2 = ct2.reshape(bs, N, W*H).transpose(1, 2)
     return ct2
 
 
 def ct_window(ct, W, H, window_size):
     bs = ct.shape[0]
     N = ct.shape[2]
-    ct = ct.transpose(1, 2).view(bs, N, W, H)
-    ct = ct.view(bs, N, H // window_size, window_size, W // window_size, window_size)
-    ct = ct.permute(0, 2, 4, 3, 5, 1).reshape(-1, H * W, N)
+    ct = ct.view(bs, H // window_size, window_size, W // window_size, window_size, N)
+    ct = ct.permute(0, 1, 3, 2, 4, 5)
     return ct
 
 
-class AddCoords(nn.Module):
-    def __init__(self,
-                 rank,
-                 with_r=False,
-                 use_cuda=False):
-        super(AddCoords, self).__init__()
-        self.rank = rank
-        self.with_r = with_r
-        self.use_cuda = use_cuda
-        self.grid_exists = False
-
-    def forward(self, input_tensor):
-        if self.rank == 2:
-            batch_size_shape, channel_in_shape, dim_y, dim_x = input_tensor.shape
-
-            if not self.grid_exists\
-                    or input_tensor.shape[0] != self.col_idx_v.shape[0] \
-                    or input_tensor.shape[2] != self.col_idx_v.shape[2] \
-                    or input_tensor.shape[3] != self.col_idx_v.shape[3] \
-                    or input_tensor.device != self.col_idx_v.device:
-                n_col, n_row = dim_y, dim_x
-                col_vals = torch.arange(0, n_col)
-                col_repeat = col_vals.repeat(n_row, 1)
-                col_idx = col_repeat.view(1, 1, n_row, n_col)
-
-                row_vals = torch.arange(0, n_row).view(n_row, -1)
-                row_repeat = row_vals.repeat(1, n_col)
-                row_idx = row_repeat.view(1, 1, n_row, n_col)
-
-                self.col_idx_v = col_idx.float().to(input_tensor.device)/float(n_col-1)*2 - 1
-                self.row_idx_v = row_idx.float().to(input_tensor.device)/float(n_row-1)*2 - 1
-
-                self.col_idx_v = torch.repeat_interleave(self.col_idx_v, batch_size_shape, 0)
-                self.row_idx_v = torch.repeat_interleave(self.row_idx_v, batch_size_shape, 0)
-
-                self.col_idx_v.detach_()
-                self.row_idx_v.detach_()
-
-                self.grid_exists = True
-
-            out = torch.cat([input_tensor, self.col_idx_v, self.row_idx_v], dim=1)
-        elif self.rank == 1:
-            batch_size_shape, dim_x, channel_in_shape = input_tensor.shape
-
-            if not self.grid_exists \
-                    or input_tensor.shape[0] != self.row_idx_v.shape[0] \
-                    or input_tensor.shape[1] != self.row_idx_v.shape[1] \
-                    or input_tensor.shape[2] != self.row_idx_v.shape[2] \
-                    or input_tensor.device != self.row_idx_v.device:
-
-                n_row = dim_x
-                row_vals = torch.arange(0, n_row).view(1,  n_row, 1)
-                self.row_idx_v = row_vals.float().to(input_tensor.device)/float(n_row-1)*2 - 1
-                self.row_idx_v.detach_()
-                self.grid_exists = True
-            out = self.row_idx_v
-        else:
-            raise NotImplementedError
-
-        return out
-
-
-class CoordConv2d(nn.Module):
-    def __init__(self,
-                 in_channels,
-                 out_channels,
-                 kernel_size,
-                 stride=1,
-                 padding=0,
-                 dilation=1,
-                 groups=1,
-                 bias=False,
-                 with_r=False,
-                 use_cuda=True):
-
-        super().__init__()
-
-        self.rank = 2
-        self.addcoords = AddCoords(self.rank, with_r, use_cuda=use_cuda)
-        self.conv = nn.Conv2d(in_channels + self.rank + int(with_r),
-                              out_channels,
-                              kernel_size,
-                              stride,
-                              padding,
-                              dilation,
-                              groups,
-                              bias)
-
-    def forward(self, input_tensor):
-        out = self.addcoords(input_tensor)
-        out = self.conv(out)
-        return out
-
-
-class CoordConv1d(nn.Module):
-    def __init__(self,
-                 out_channels,
-                 bias=False,
-                 with_r=False,
-                 use_cuda=True):
-
-        super().__init__()
-        self.rank = 1
-        self.addcoords = AddCoords(self.rank, with_r, use_cuda=use_cuda)
-        self.conv = nn.Linear(self.rank + int(with_r),
-                              out_channels,
-                              bias=bias)
-        self.grid_exists = False
-        self.pos_emb = None
-
-    def forward(self, input_tensor):
-        if self.training:
-            self.grid_exists = False
-
-        if self.grid_exists:
-            if self.pos_emb.shape[1] != input_tensor.shape[1] or input_tensor.device != self.pos_emb.device:
-                self.grid_exists = False
-
-        if not self.grid_exists:
-            out = self.addcoords(input_tensor)
-            pos_emb = self.conv(out)
-            self.pos_emb = pos_emb
-            self.grid_exists = True
-        else:
-            pos_emb = self.pos_emb
-
-        out = input_tensor + pos_emb
-
-        return out
-
-
 class PosEmbMLPSwinv2D(nn.Module):
     def __init__(self,
                  window_size,
                  pretrained_window_size,
                  num_heads, seq_length,
                  ct_correct=False,
                  no_log=False):
```

### Comparing `fastervit-0.8.9/fastervit/models/faster_vit_any_res.py` & `fastervit-0.9.0/fastervit/models/faster_vit_any_res.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import torch
 import torch.nn as nn
 from timm.models.registry import register_model
 from timm.models.layers import trunc_normal_, DropPath, LayerNorm2d
 from .registry import register_pip_model
 import numpy as np
-
+from utils.checkpoint import load_checkpoint
 
 def _cfg(url='', **kwargs):
     return {'url': url,
             'num_classes': 1000,
             'input_size': (3, 224, 224),
             'pool_size': None,
             'crop_pct': 0.875,
@@ -75,158 +75,25 @@
     return x
 
 
 def ct_dewindow(ct, W, H, window_size):
     bs = ct.shape[0]
     N=ct.shape[2]
     ct2 = ct.view(-1, W//window_size, H//window_size, window_size, window_size, N).permute(0, 5, 1, 3, 2, 4)
-    ct2 = ct2.reshape(bs, N, W, H).flatten(2).transpose(1, 2)
+    ct2 = ct2.reshape(bs, N, W*H).transpose(1, 2)
     return ct2
 
 
 def ct_window(ct, W, H, window_size):
     bs = ct.shape[0]
     N = ct.shape[2]
-    ct = ct.transpose(1, 2).view(bs, N, W, H)
-    ct = ct.view(bs, N, H // window_size, window_size, W // window_size, window_size)
-    ct = ct.permute(0, 2, 4, 3, 5, 1).reshape(-1, H * W, N)
+    ct = ct.view(bs, H // window_size, window_size, W // window_size, window_size, N)
+    ct = ct.permute(0, 1, 3, 2, 4, 5)
     return ct
 
-
-class AddCoords(nn.Module):
-    def __init__(self,
-                 rank,
-                 with_r=False,
-                 use_cuda=False):
-        super(AddCoords, self).__init__()
-        self.rank = rank
-        self.with_r = with_r
-        self.use_cuda = use_cuda
-        self.grid_exists = False
-
-    def forward(self, input_tensor):
-        if self.rank == 2:
-            batch_size_shape, channel_in_shape, dim_y, dim_x = input_tensor.shape
-
-            if not self.grid_exists\
-                    or input_tensor.shape[0] != self.col_idx_v.shape[0] \
-                    or input_tensor.shape[2] != self.col_idx_v.shape[2] \
-                    or input_tensor.shape[3] != self.col_idx_v.shape[3] \
-                    or input_tensor.device != self.col_idx_v.device:
-                n_col, n_row = dim_y, dim_x
-                col_vals = torch.arange(0, n_col)
-                col_repeat = col_vals.repeat(n_row, 1)
-                col_idx = col_repeat.view(1, 1, n_row, n_col)
-
-                row_vals = torch.arange(0, n_row).view(n_row, -1)
-                row_repeat = row_vals.repeat(1, n_col)
-                row_idx = row_repeat.view(1, 1, n_row, n_col)
-
-                self.col_idx_v = col_idx.float().to(input_tensor.device)/float(n_col-1)*2 - 1
-                self.row_idx_v = row_idx.float().to(input_tensor.device)/float(n_row-1)*2 - 1
-
-                self.col_idx_v = torch.repeat_interleave(self.col_idx_v, batch_size_shape, 0)
-                self.row_idx_v = torch.repeat_interleave(self.row_idx_v, batch_size_shape, 0)
-
-                self.col_idx_v.detach_()
-                self.row_idx_v.detach_()
-
-                self.grid_exists = True
-
-            out = torch.cat([input_tensor, self.col_idx_v, self.row_idx_v], dim=1)
-        elif self.rank == 1:
-            batch_size_shape, dim_x, channel_in_shape = input_tensor.shape
-
-            if not self.grid_exists \
-                    or input_tensor.shape[0] != self.row_idx_v.shape[0] \
-                    or input_tensor.shape[1] != self.row_idx_v.shape[1] \
-                    or input_tensor.shape[2] != self.row_idx_v.shape[2] \
-                    or input_tensor.device != self.row_idx_v.device:
-
-                n_row = dim_x
-                row_vals = torch.arange(0, n_row).view(1,  n_row, 1)
-                self.row_idx_v = row_vals.float().to(input_tensor.device)/float(n_row-1)*2 - 1
-                self.row_idx_v.detach_()
-                self.grid_exists = True
-            out = self.row_idx_v
-        else:
-            raise NotImplementedError
-
-        return out
-
-
-class CoordConv2d(nn.Module):
-    def __init__(self,
-                 in_channels,
-                 out_channels,
-                 kernel_size,
-                 stride=1,
-                 padding=0,
-                 dilation=1,
-                 groups=1,
-                 bias=False,
-                 with_r=False,
-                 use_cuda=True):
-
-        super().__init__()
-
-        self.rank = 2
-        self.addcoords = AddCoords(self.rank, with_r, use_cuda=use_cuda)
-        self.conv = nn.Conv2d(in_channels + self.rank + int(with_r),
-                              out_channels,
-                              kernel_size,
-                              stride,
-                              padding,
-                              dilation,
-                              groups,
-                              bias)
-
-    def forward(self, input_tensor):
-        out = self.addcoords(input_tensor)
-        out = self.conv(out)
-        return out
-
-
-class CoordConv1d(nn.Module):
-    def __init__(self,
-                 out_channels,
-                 bias=False,
-                 with_r=False,
-                 use_cuda=True):
-
-        super().__init__()
-        self.rank = 1
-        self.addcoords = AddCoords(self.rank, with_r, use_cuda=use_cuda)
-        self.conv = nn.Linear(self.rank + int(with_r),
-                              out_channels,
-                              bias=bias)
-        self.grid_exists = False
-        self.pos_emb = None
-
-    def forward(self, input_tensor):
-        if self.training:
-            self.grid_exists = False
-
-        if self.grid_exists:
-            if self.pos_emb.shape[1] != input_tensor.shape[1] or input_tensor.device != self.pos_emb.device:
-                self.grid_exists = False
-
-        if not self.grid_exists:
-            out = self.addcoords(input_tensor)
-            pos_emb = self.conv(out)
-            self.pos_emb = pos_emb
-            self.grid_exists = True
-        else:
-            pos_emb = self.pos_emb
-
-        out = input_tensor + pos_emb
-
-        return out
-
-
 class PosEmbMLPSwinv2D(nn.Module):
     def __init__(self,
                  window_size,
                  pretrained_window_size,
                  num_heads, seq_length,
                  ct_correct=False,
                  no_log=False):
@@ -996,15 +863,16 @@
         x = torch.flatten(x, 1)
         return x
 
     def forward(self, x):
         x = self.forward_features(x)
         x = self.head(x)
         return x
-
+    def load_state_dict(self, pretrained, strict: bool = False):
+        load_checkpoint(self, pretrained, strict=strict)
 
 @register_pip_model
 @register_model
 def faster_vit_0_any_res(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [2, 3, 6, 5])
     num_heads = kwargs.pop("num_heads", [2, 4, 8, 16])
     window_size = kwargs.pop("window_size", [7, 7, 7, 7])
@@ -1022,15 +890,15 @@
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_0_any_res']
     if pretrained:
-        model.load_state_dict(torch.load(pretrained))
+        model.load_state_dict(pretrained)
     return model
 
 
 @register_pip_model
 @register_model
 def faster_vit_1_any_res(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [1, 3, 8, 5])
@@ -1050,15 +918,15 @@
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_1_any_res']
     if pretrained:
-        model.load_state_dict(torch.load(pretrained))
+        model.load_state_dict(pretrained)
     return model
 
 
 @register_pip_model
 @register_model
 def faster_vit_2_any_res(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [3, 3, 8, 5])
@@ -1078,15 +946,15 @@
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_2_any_res']
     if pretrained:
-        model.load_state_dict(torch.load(pretrained))
+        model.load_state_dict(pretrained)
     return model
 
 
 @register_pip_model
 @register_model
 def faster_vit_3_any_res(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [3, 3, 12, 5])
@@ -1110,15 +978,15 @@
                       drop_path_rate=drop_path_rate,
                       layer_scale=layer_scale,
                       layer_scale_conv=None,
                       do_propagation=True,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_3_any_res']
     if pretrained:
-        model.load_state_dict(torch.load(pretrained))
+        model.load_state_dict(pretrained)
     return model
 
 
 @register_pip_model
 @register_model
 def faster_vit_4_any_res(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [3, 3, 12, 5])
@@ -1143,15 +1011,15 @@
                       layer_scale=layer_scale,
                       layer_scale_conv=None,
                       layer_norm_last=False,
                       do_propagation=True,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_4_any_res']
     if pretrained:
-        model.load_state_dict(torch.load(pretrained))
+        model.load_state_dict(pretrained)
     return model
 
 
 @register_pip_model
 @register_model
 def faster_vit_5_any_res(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [3, 3, 12, 5])
@@ -1176,15 +1044,15 @@
                       layer_scale=layer_scale,
                       layer_scale_conv=None,
                       layer_norm_last=False,
                       do_propagation=True,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_5_any_res']
     if pretrained:
-        model.load_state_dict(torch.load(pretrained))
+        model.load_state_dict(pretrained)
     return model
 
 
 @register_pip_model
 @register_model
 def faster_vit_6_any_res(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [3, 3, 16, 8])
@@ -1209,9 +1077,9 @@
                       layer_scale=layer_scale,
                       layer_scale_conv=None,
                       layer_norm_last=False,
                       do_propagation=True,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_6_any_res']
     if pretrained:
-        model.load_state_dict(torch.load(pretrained))
+        model.load_state_dict(pretrained)
     return model
```

### Comparing `fastervit-0.8.9/fastervit/models/registry.py` & `fastervit-0.9.0/fastervit/models/registry.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.9/fastervit/scheduler/cosine_lr.py` & `fastervit-0.9.0/fastervit/scheduler/cosine_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.9/fastervit/scheduler/multistep_lr.py` & `fastervit-0.9.0/fastervit/scheduler/multistep_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.9/fastervit/scheduler/plateau_lr.py` & `fastervit-0.9.0/fastervit/scheduler/plateau_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.9/fastervit/scheduler/poly_lr.py` & `fastervit-0.9.0/fastervit/scheduler/poly_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.9/fastervit/scheduler/scheduler.py` & `fastervit-0.9.0/fastervit/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.9/fastervit/scheduler/scheduler_factory.py` & `fastervit-0.9.0/fastervit/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.9/fastervit/scheduler/step_lr.py` & `fastervit-0.9.0/fastervit/scheduler/step_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.9/fastervit/scheduler/tanh_lr.py` & `fastervit-0.9.0/fastervit/scheduler/tanh_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.9/fastervit/tensorboard.py` & `fastervit-0.9.0/fastervit/tensorboard.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.9/fastervit/train.py` & `fastervit-0.9.0/fastervit/train.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.9/fastervit/validate.py` & `fastervit-0.9.0/fastervit/validate.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.9/fastervit.egg-info/PKG-INFO` & `fastervit-0.9.0/fastervit.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastervit
-Version: 0.8.9
+Version: 0.9.0
 Summary: FasterViT: Fast Vision Transformers with Hierarchical Attention
 Home-page: https://github.com/NVlabs/FasterViT
 Author: Ali Hatamizadeh
 Author-email: ahatamiz123@gmail.com
 License: NVIDIA Source Code License-NC
 Keywords: pytorch pretrained models efficientnet mobilenetv3 mnasnet resnet vision transformer vit
 Classifier: Programming Language :: Python :: 3.7
@@ -41,27 +41,27 @@
 terms of accuracy vs. image throughput (no extra training data !)
 
 <p align="center">
 <img src="https://github.com/NVlabs/FasterViT/assets/26806394/253d1a2e-b5f5-4a9b-a362-6cdd16bfccc1" width=62% height=62% 
 class="center">
 </p>
 
-
-<!-- We introduce a new self-attention mechanism, denoted as Hierarchical
+We introduce a new self-attention mechanism, denoted as Hierarchical
 Attention (HAT), that captures both short and long-range information by learning
 cross-window carrier tokens.
 
-![teaser](./fastervit/assets/hierarchial_attn.png) -->
-
+![teaser](./fastervit/assets/hierarchial_attn.png)
 
-<!-- ## 💥 News 💥
+## 💥 News 💥
 
-- **[06.18.2023]** 🔥 We have released the FasterViT [pip package](https://pypi.org/project/fastervit/) !
-- **[06.17.2023]** 🔥 [Any-resolution FasterViT](./fastervit/models/faster_vit_any_res.py)  model is now available ! the model can be used for variety of applications such as detection and segmentation or high-resolution fine-tuning with arbitrary input image resolutions. 
-- **[06.09.2023]** 🔥🔥 We have released source code and ImageNet-1K FasterViT-models ! -->
+- **[06.30.2023]** 🔥🔥 We have further improved the [Any-resolution FasterViT](https://developer.nvidia.com/tensorrt-getting-started) throughput of FasterViT models by 10-15% on average across different models.  
+- **[06.29.2023]** 🔥 Any-resolution FasterViT model can now be intitialized from pre-trained ImageNet resolution (224 x 244) models.
+- **[06.18.2023]** We have released the FasterViT [pip package](https://pypi.org/project/fastervit/) !
+- **[06.17.2023]** 🔥 [Any-resolution FasterViT](./fastervit/models/faster_vit_any_res.py)  model is now available ! the model can be used for variety of applications such as detection and segmentation or high-resolution fine-tuning with arbitrary input image resolutions.
+- **[06.09.2023]** 🔥🔥 We have released source code and ImageNet-1K FasterViT-models !
 
 ## Quick Start
 
 The FasterViT can be conveniently installed by:
 
 ```bash
 pip install fastervit
@@ -87,24 +87,26 @@
 >>> model = create_model('faster_vit_1_any_res', 
                           resolution=[576, 960],
                           window_size=[7, 7, 12, 6],
                           ct_size=2,
                           dim=128)
 ```
 
-<!-- ## Catalog
+## Catalog
 - [x] ImageNet-1K training code
 - [x] ImageNet-1K pre-trained models
 - [x] Any-resolution FasterViT
 - [x] FasterViT pip-package release
-- [ ] Update training scripts to support model.compile, 
+- [x] Add capablity to initialize any-resolution FasterViT from ImageNet-pretrained weights. 
+- [ ] Update training scripts to support model.compile
+- [ ] Add isotropic FasterViT
 - [ ] ImageNet-21K pre-trained models
 - [ ] ImageNet-21K fine-tune scripts
 - [ ] Detection code (DINO) + models
-- [ ] Segmentation code + models -->
+- [ ] Segmentation code + models
 
 --- 
 
 ## Results + Pretrained Models
 
 ### ImageNet-1K
 **FasterViT ImageNet-1K Pretrained Models**
@@ -302,46 +304,60 @@
 --checkpoint <checkpoint-path>
 --data_dir <imagenet-path>
 --batch-size <batch-size-per-gpu
 ``` 
 
 Here `--model` is the FasterViT variant (e.g. `faster_vit_0_224_1k`), `--checkpoint` is the path to pretrained model weights, `--data_dir` is the path to ImageNet-1K validation set and `--batch-size` is the number of batch size. We also provide a sample script [here](./fastervit/validate.sh). 
 
+## ONNX Conversion
+
+We provide ONNX conversion script to enable dynamic batch size inference. For instance, to generate ONNX model for `faster_vit_0_any_res` with resolution 576 x 960 and ONNX opset number 17, the following can be used. 
+
+```bash 
+python onnx_convert --model-name faster_vit_0_any_res --resolution-h 576 --resolution-w 960 --onnx-opset 17
+
+```
+
 
 ## Installation
 
 The dependencies can be installed by running:
 
 ```bash
 pip install -r requirements.txt
 ```
 
-## Third-party Extentions
-We always welcome third-party extentions/implementations and usage for other purposes. If you would like your work to be listed in this repository, please raise and issue and provide us with detailed information.  
+## Star History
 
+[![Star History Chart](https://api.star-history.com/svg?repos=NVlabs/FasterViT&type=Date)](https://star-history.com/#NVlabs/FasterViT&Date)
 
-## Acknowledgement
-This repository is built on top of the [timm](https://github.com/huggingface/pytorch-image-models) repository. We thank [Ross Wrightman](https://rwightman.com/) for creating and maintaining this high-quality library.  
+
+## Third-party Extentions
+We always welcome third-party extentions/implementations and usage for other purposes. If you would like your work to be listed in this repository, please raise and issue and provide us with detailed information.  
 
 ## Citation
 
-Please consider citing FasterViT if this repository is useful for your work:
+Please consider citing FasterViT if this repository is useful for your work. 
 
 ```
 @article{hatamizadeh2023fastervit,
   title={FasterViT: Fast Vision Transformers with Hierarchical Attention},
   author={Hatamizadeh, Ali and Heinrich, Greg and Yin, Hongxu and Tao, Andrew and Alvarez, Jose M and Kautz, Jan and Molchanov, Pavlo},
   journal={arXiv preprint arXiv:2306.06189},
   year={2023}
 }
 ```
 
+
 ## Licenses
 
 Copyright © 2023, NVIDIA Corporation. All rights reserved.
 
 This work is made available under the NVIDIA Source Code License-NC. Click [here](LICENSE) to view a copy of this license.
 
 For license information regarding the timm repository, please refer to its [repository](https://github.com/rwightman/pytorch-image-models).
 
 For license information regarding the ImageNet dataset, please see the [ImageNet official website](https://www.image-net.org/). 
 
+## Acknowledgement
+This repository is built on top of the [timm](https://github.com/huggingface/pytorch-image-models) repository. We thank [Ross Wrightman](https://rwightman.com/) for creating and maintaining this high-quality library.  
+
```

### Comparing `fastervit-0.8.9/fastervit.egg-info/SOURCES.txt` & `fastervit-0.9.0/fastervit.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -21,8 +21,11 @@
 fastervit/scheduler/cosine_lr.py
 fastervit/scheduler/multistep_lr.py
 fastervit/scheduler/plateau_lr.py
 fastervit/scheduler/poly_lr.py
 fastervit/scheduler/scheduler.py
 fastervit/scheduler/scheduler_factory.py
 fastervit/scheduler/step_lr.py
-fastervit/scheduler/tanh_lr.py
+fastervit/scheduler/tanh_lr.py
+fastervit/utils/__init__.py
+fastervit/utils/checkpoint.py
+fastervit/utils/datasets.py
```

### Comparing `fastervit-0.8.9/setup.py` & `fastervit-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='fastervit',
-    version='0.8.9',
+    version='0.9.0',
     description='FasterViT: Fast Vision Transformers with Hierarchical Attention',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/NVlabs/FasterViT',
     author='Ali Hatamizadeh',
     author_email='ahatamiz123@gmail.com',
     classifiers=[
```

