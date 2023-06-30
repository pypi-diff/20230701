# Comparing `tmp/autogluon.multimodal-0.8.1b20230630.tar.gz` & `tmp/autogluon.multimodal-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.multimodal-0.8.1b20230630.tar", last modified: Fri Jun 30 09:04:34 2023, max compression
+gzip compressed data, was "autogluon.multimodal-0.8.2.tar", last modified: Fri Jun 30 22:17:20 2023, max compression
```

## Comparing `autogluon.multimodal-0.8.1b20230630.tar` & `autogluon.multimodal-0.8.2.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:34.552754 autogluon.multimodal-0.8.1b20230630/
--rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-06-30 09:04:34.552754 autogluon.multimodal-0.8.1b20230630/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 09:04:34.552754 autogluon.multimodal-0.8.1b20230630/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:34.540754 autogluon.multimodal-0.8.1b20230630/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:34.540754 autogluon.multimodal-0.8.1b20230630/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:34.544754 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:34.544754 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/cli/prepare_detection_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/cli/voc2coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:34.544754 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:34.544754 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:34.544754 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:34.544754 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:34.544754 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/voc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:34.544754 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/yolox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8xb8-300e_coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:34.544754 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/ovd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:34.544754 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:34.548754 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:34.548754 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/dataset_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32962 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/mixup.py
--rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/preprocess_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_document.py
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:34.548754 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/randaug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/template_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/trivial_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    87088 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:34.548754 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/adaptation_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/categorical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/categorical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/document_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:34.548754 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/fusion/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/fusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/fusion/fusion_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/fusion/fusion_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/fusion/fusion_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/huggingface_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/mmdet_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/mmocr_text_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/mmocr_text_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/ner_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/numerical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/numerical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/t_few.py
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/timm_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    26208 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:34.552754 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/optimization/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/optimization/lit_distiller.py
--rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/optimization/lit_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/optimization/lit_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/optimization/lit_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/optimization/lit_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/optimization/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/optimization/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/optimization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   121028 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    26209 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/problem_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:34.552754 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/export.py
--rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/few_shot_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    19409 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/mmcv.py
--rw-r--r--   0 runner    (1001) docker     (123)    22641 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/nlpaug.py
--rw-r--r--   0 runner    (1001) docker     (123)    53333 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/object_detection_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-30 09:04:00.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-30 09:04:34.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:34.540754 autogluon.multimodal-0.8.1b20230630/src/autogluon.multimodal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-06-30 09:04:34.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon.multimodal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-30 09:04:34.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon.multimodal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:04:34.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon.multimodal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 09:04:34.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon.multimodal.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-30 09:04:34.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon.multimodal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 09:04:34.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon.multimodal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:04:34.000000 autogluon.multimodal-0.8.1b20230630/src/autogluon.multimodal.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:20.225596 autogluon.multimodal-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-06-30 22:17:20.225596 autogluon.multimodal-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 22:17:20.225596 autogluon.multimodal-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:20.209596 autogluon.multimodal-0.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:20.209596 autogluon.multimodal-0.8.2/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:20.209596 autogluon.multimodal-0.8.2/src/autogluon/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:20.209596 autogluon.multimodal-0.8.2/src/autogluon/multimodal/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/cli/prepare_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/cli/voc2coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:20.213596 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:20.213596 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:20.213596 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:20.213596 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:20.213596 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:20.213596 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/yolox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8xb8-300e_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:20.213596 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/ovd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:20.213596 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:20.217596 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:20.217596 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/dataset_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32962 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/mixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/preprocess_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_label.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:20.217596 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/randaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/template_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/trivial_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87088 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:20.217596 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/adaptation_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/categorical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/categorical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/document_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:20.217596 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/fusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/fusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/fusion/fusion_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/fusion/fusion_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/fusion/fusion_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/huggingface_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/mmdet_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/mmocr_text_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/mmocr_text_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/ner_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/numerical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/numerical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/t_few.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/timm_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26208 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:20.221596 autogluon.multimodal-0.8.2/src/autogluon/multimodal/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/optimization/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/optimization/lit_distiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/optimization/lit_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/optimization/lit_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/optimization/lit_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/optimization/lit_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/optimization/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/optimization/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/optimization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121028 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26209 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/problem_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:20.225596 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/few_shot_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19409 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/mmcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22641 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/nlpaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53333 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/object_detection_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-30 22:16:45.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 22:17:19.000000 autogluon.multimodal-0.8.2/src/autogluon/multimodal/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:20.209596 autogluon.multimodal-0.8.2/src/autogluon.multimodal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-06-30 22:17:20.000000 autogluon.multimodal-0.8.2/src/autogluon.multimodal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-30 22:17:20.000000 autogluon.multimodal-0.8.2/src/autogluon.multimodal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:17:20.000000 autogluon.multimodal-0.8.2/src/autogluon.multimodal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 22:17:20.000000 autogluon.multimodal-0.8.2/src/autogluon.multimodal.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-30 22:17:20.000000 autogluon.multimodal-0.8.2/src/autogluon.multimodal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 22:17:20.000000 autogluon.multimodal-0.8.2/src/autogluon.multimodal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:17:20.000000 autogluon.multimodal-0.8.2/src/autogluon.multimodal.egg-info/zip-safe
```

### Comparing `autogluon.multimodal-0.8.1b20230630/PKG-INFO` & `autogluon.multimodal-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.8.1b20230630
+Version: 0.8.2
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -33,15 +33,15 @@
         
         ## Example
         
         ```python
         # First install package from terminal:
         # pip install -U pip
         # pip install -U setuptools wheel
-        # pip install autogluon  # autogluon==0.8.0
+        # pip install autogluon  # autogluon==0.8.1
         
         from autogluon.tabular import TabularDataset, TabularPredictor
         train_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/train.csv')
         test_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/test.csv')
         predictor = TabularPredictor(label='class').fit(train_data, time_limit=120)  # Fit models for 120s
         leaderboard = predictor.leaderboard(test_data)
         ```
```

### Comparing `autogluon.multimodal-0.8.1b20230630/setup.py` & `autogluon.multimodal-0.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,18 +35,17 @@
     "timm>=0.9.2,<0.10.0",
     "torch>=1.9,<1.14",
     "torchvision<0.15.0",
     "scikit-image>=0.19.1,<0.20.0",
     "pytorch-lightning>=1.9.0,<1.10.0",
     "text-unidecode>=1.3,<1.4",
     "torchmetrics>=0.11.0,<0.12.0",
-    "transformers>=4.23.0,<4.27.0",
+    "transformers[sentencepiece]>=4.23.0,<4.27.0",
     "nptyping>=1.4.4,<2.5.0",
     "omegaconf>=2.1.1,<2.3.0",
-    "sentencepiece>=0.1.95,<0.2.0",
     f"autogluon.core[raytune]=={version}",
     f"autogluon.features=={version}",
     f"autogluon.common=={version}",
     "pytorch-metric-learning>=1.3.0,<2.0",
     "nlpaug>=1.1.10,<1.2.0",
     "nltk>=3.4.5,<4.0.0",
     "openmim>=0.3.7,<0.4.0",
```

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/cli/prepare_detection_dataset.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/cli/prepare_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/cli/voc2coco.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/cli/voc2coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/constants.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/__init__.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/collator.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/collator.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/datamodule.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/dataset.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/infer_types.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/infer_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/label_encoder.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/label_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/mixup.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/mixup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/preprocess_dataframe.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/preprocess_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_categorical.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_categorical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_document.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_document.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_image.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_label.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_label.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             model=model,
             collate_func=CollateMMDet,
             max_img_num_per_col=max_img_num_per_col,
             missing_value_strategy=missing_value_strategy,
             requires_column_info=requires_column_info,
         )
 
-        # for yolox we seperate loading pipeline to support multi_image_mix_dataset
+        # for yolox we separate loading pipeline to support multi_image_mix_dataset
         if "loading_pipeline" in self.cfg.keys():
             self.load_processor = Compose(self.cfg.loading_pipeline)
 
     def prepare_one_sample(
         self,
         image_paths: Dict[str, List[str]],
         is_training: bool,
```

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_ner.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_numerical.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_numerical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_ovd.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/process_text.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/process_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/randaug.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/randaug.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     return f
 
 
 def Identity(img, v):
     return img
 
 
-def augment_list():  # 16 oeprations and their ranges
+def augment_list():  # 16 operations and their ranges
     # https://github.com/google-research/uda/blob/master/image/randaugment/policies.py#L57
     # l = [
     #     (Identity, 0., 1.0),
     #     (ShearX, 0., 0.3),  # 0
     #     (ShearY, 0., 0.3),  # 1
     #     (TranslateX, 0., 0.33),  # 2
     #     (TranslateY, 0., 0.33),  # 3
```

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/template_engine.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/template_engine.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/templates.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/templates.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/trivial_augmenter.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/trivial_augmenter.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/data/utils.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/data/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/matcher.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/__init__.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/adaptation_layers.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/adaptation_layers.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/categorical_mlp.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/categorical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/categorical_transformer.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/categorical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/clip.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/clip.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/document_transformer.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/document_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/ft_transformer.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/fusion/base.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/fusion/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/fusion/fusion_mlp.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/fusion/fusion_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/fusion/fusion_ner.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/fusion/fusion_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/fusion/fusion_transformer.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/fusion/fusion_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/huggingface_text.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/huggingface_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/mlp.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/mmdet_image.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/mmdet_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/mmocr_text_detection.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/mmocr_text_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/mmocr_text_recognition.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/mmocr_text_recognition.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/ner_text.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/ner_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/numerical_mlp.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/numerical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/numerical_transformer.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/numerical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/ovd.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/t_few.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/t_few.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/timm_image.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/timm_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/models/utils.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/models/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/optimization/deepspeed.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/optimization/deepspeed.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/optimization/lit_distiller.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/optimization/lit_distiller.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/optimization/lit_matcher.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/optimization/lit_matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/optimization/lit_mmdet.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/optimization/lit_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/optimization/lit_module.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/optimization/lit_module.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/optimization/lit_ner.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/optimization/lit_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/optimization/losses.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/optimization/losses.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/optimization/lr_scheduler.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/optimization/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/optimization/utils.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/optimization/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/predictor.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/presets.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/problem_types.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/problem_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/registry.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/registry.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/__init__.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/cache.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/cache.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/checkpoint.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/cloud_io.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/cloud_io.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/colormap.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/config.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,15 @@
         `config.names` should also be a attribute of `config`, e.g, `config.timm_image`.
     customized_names
         The provided names to replace the existing ones in `config.names` as well as
         the corresponding attribute names. For example, if `customized_names` is
         ["timm_image_123", "hf_text_abc"], then `config.timm_image` and `config.hf_text`
         are changed to `config.timm_image_123` and `config.hf_text_abc`.
     advanced_hyperparameters
-        The hyperparameters whose values are compelx objects, which can't be stored in config.
+        The hyperparameters whose values are complex objects, which can't be stored in config.
 
     Returns
     -------
         A new config with its first-level attributes customized by the provided names.
     """
     if not customized_names:
         return config, advanced_hyperparameters
```

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/data.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/data.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/download.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/download.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/environment.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/environment.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/export.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/export.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/few_shot_learning.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/few_shot_learning.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/hpo.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/inference.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/inference.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/label_studio.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/label_studio.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/load.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/load.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/log.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/log.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/map.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/map.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/matcher.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/metric.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/metric.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/misc.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/mmcv.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/mmcv.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/model.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/nlpaug.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/nlpaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/object_detection.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/object_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/object_detection_visualizer.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/object_detection_visualizer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/onnx.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/onnx.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         inputs = self.sess.get_inputs()
         outputs = self.sess.get_outputs()
         self.input_names = [i.name for i in inputs]
         self.output_names = [i.name for i in outputs]
 
     def __call__(self, *args):
         """
-        Make the module callable like torch.nn.Module, while runnning forward pass with onnxruntime.
+        Make the module callable like torch.nn.Module, while running forward pass with onnxruntime.
 
         Parameters
         ----------
         args : list of torch.Tensor
             A list of torch.Tensor that are inputs of the model.
 
         Returns
```

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/ovd.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/pipeline.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon/multimodal/utils/save.py` & `autogluon.multimodal-0.8.2/src/autogluon/multimodal/utils/save.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon.multimodal.egg-info/PKG-INFO` & `autogluon.multimodal-0.8.2/src/autogluon.multimodal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.8.1b20230630
+Version: 0.8.2
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -33,15 +33,15 @@
         
         ## Example
         
         ```python
         # First install package from terminal:
         # pip install -U pip
         # pip install -U setuptools wheel
-        # pip install autogluon  # autogluon==0.8.0
+        # pip install autogluon  # autogluon==0.8.1
         
         from autogluon.tabular import TabularDataset, TabularPredictor
         train_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/train.csv')
         test_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/test.csv')
         predictor = TabularPredictor(label='class').fit(train_data, time_limit=120)  # Fit models for 120s
         leaderboard = predictor.leaderboard(test_data)
         ```
```

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon.multimodal.egg-info/SOURCES.txt` & `autogluon.multimodal-0.8.2/src/autogluon.multimodal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.1b20230630/src/autogluon.multimodal.egg-info/requires.txt` & `autogluon.multimodal-0.8.2/src/autogluon.multimodal.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -13,21 +13,20 @@
 timm<0.10.0,>=0.9.2
 torch<1.14,>=1.9
 torchvision<0.15.0
 scikit-image<0.20.0,>=0.19.1
 pytorch-lightning<1.10.0,>=1.9.0
 text-unidecode<1.4,>=1.3
 torchmetrics<0.12.0,>=0.11.0
-transformers<4.27.0,>=4.23.0
+transformers[sentencepiece]<4.27.0,>=4.23.0
 nptyping<2.5.0,>=1.4.4
 omegaconf<2.3.0,>=2.1.1
-sentencepiece<0.2.0,>=0.1.95
-autogluon.core[raytune]==0.8.1b20230630
-autogluon.features==0.8.1b20230630
-autogluon.common==0.8.1b20230630
+autogluon.core[raytune]==0.8.2
+autogluon.features==0.8.2
+autogluon.common==0.8.2
 pytorch-metric-learning<2.0,>=1.3.0
 nlpaug<1.2.0,>=1.1.10
 nltk<4.0.0,>=3.4.5
 openmim<0.4.0,>=0.3.7
 defusedxml<0.7.2,>=0.7.1
 jinja2<3.2,>=3.0.3
 tensorboard<3,>=2.9
```

