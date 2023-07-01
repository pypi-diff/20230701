# Comparing `tmp/keras-aug-0.5.5.tar.gz` & `tmp/keras-aug-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-aug-0.5.5.tar", last modified: Mon Jun 26 05:06:19 2023, max compression
+gzip compressed data, was "keras-aug-0.5.6.tar", last modified: Sat Jul  1 09:12:13 2023, max compression
```

## Comparing `keras-aug-0.5.5.tar` & `keras-aug-0.5.6.tar`

### file list

```diff
@@ -1,163 +1,184 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.525474 keras-aug-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-06-26 05:05:50.000000 keras-aug-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27043 2023-06-26 05:06:19.525474 keras-aug-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12706 2023-06-26 05:05:50.000000 keras-aug-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.505474 keras-aug-0.5.5/keras_aug/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.505474 keras-aug-0.5.5/keras_aug/core/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.509474 keras-aug-0.5.5/keras_aug/core/factor_sampler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/constant_factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/constant_factor_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/normal_factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/normal_factor_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/signed_constant_factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/signed_constant_factor_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/signed_normal_factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/signed_normal_factor_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/uniform_factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/uniform_factor_sampler_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.509474 keras-aug-0.5.5/keras_aug/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.509474 keras-aug-0.5.5/keras_aug/layers/__internal__/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/__internal__/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/__internal__/base_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/__internal__/base_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/__internal__/config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/__internal__/graph_xla_mode_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/__internal__/mixed_precision_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15598 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/__internal__/output_common_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10387 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/__internal__/with_bounding_boxes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/__internal__/with_ragged_image_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.509474 keras-aug-0.5.5/keras_aug/layers/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.509474 keras-aug-0.5.5/keras_aug/layers/augmentation/auto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/auto/aug_mix.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/auto/aug_mix_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/auto/rand_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/auto/rand_augment_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14971 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/auto/trivial_augment_wide.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/auto/trivial_augment_wide_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.513474 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23474 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    15409 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_affine_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_crop_and_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_crop_and_resize_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_crop_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_flip_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_resize_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_rotate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15089 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_zoom_and_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_zoom_and_crop_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.517474 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/channel_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/channel_shuffle_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_blur.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_blur_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_channel_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_channel_shift_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_clahe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_clahe_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_color_jitter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_gamma_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_gaussian_blur.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_gaussian_blur_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_hsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_hsv_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_jpeg_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_jpeg_quality_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_posterize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_posterize_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_sharpness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_sharpness_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_solarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_solarize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.517474 keras-aug-0.5.5/keras_aug/layers/augmentation/mix/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/mix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/mix/cut_mix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/mix/cut_mix_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/mix/mix_up.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/mix/mix_up_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17493 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/mix/mosaic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/mix/mosaic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.517474 keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_channel_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_channel_dropout_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_cutout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_cutout_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_erase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_erase_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_grid_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_grid_mask_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.517474 keras-aug-0.5.5/keras_aug/layers/augmentation/utility/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/utility/random_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/utility/random_apply_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/utility/random_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/utility/random_choice_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/utility/repeated_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/utility/repeated_augment_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.517474 keras-aug-0.5.5/keras_aug/layers/base/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/base/vectorized_base_random_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22094 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/base/vectorized_base_random_layer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.517474 keras-aug-0.5.5/keras_aug/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.521474 keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/center_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/center_crop_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10833 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/pad_if_needed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9878 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/pad_if_needed_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15774 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/resize.py
--rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/resize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.521474 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/auto_contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/auto_contrast_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/equalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/equalize_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/grayscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/grayscale_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/identity_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/invert.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/invert_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/normalize_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/rescale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/rescale_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.525474 keras-aug-0.5.5/keras_aug/layers/preprocessing/utility/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/utility/sanitize_bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/utility/sanitize_bounding_box_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.525474 keras-aug-0.5.5/keras_aug/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18127 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/utils/augmentation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/utils/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/utils/bounding_box_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/utils/conditional_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/utils/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/utils/distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.505474 keras-aug-0.5.5/keras_aug.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27043 2023-06-26 05:06:19.000000 keras-aug-0.5.5/keras_aug.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-06-26 05:06:19.000000 keras-aug-0.5.5/keras_aug.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 05:06:19.000000 keras-aug-0.5.5/keras_aug.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-26 05:06:19.000000 keras-aug-0.5.5/keras_aug.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 05:06:19.000000 keras-aug-0.5.5/keras_aug.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-26 05:05:50.000000 keras-aug-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 05:06:19.525474 keras-aug-0.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.034714 keras-aug-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-07-01 09:11:37.000000 keras-aug-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26898 2023-07-01 09:12:13.034714 keras-aug-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-07-01 09:11:37.000000 keras-aug-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:12.998714 keras-aug-0.5.6/keras_aug/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.002714 keras-aug-0.5.6/keras_aug/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.002714 keras-aug-0.5.6/keras_aug/core/factor_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/constant_factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/constant_factor_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/normal_factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/normal_factor_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/signed_constant_factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/signed_constant_factor_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/signed_normal_factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/signed_normal_factor_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/uniform_factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/uniform_factor_sampler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.006714 keras-aug-0.5.6/keras_aug/datapoints/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.006714 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14743 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/converter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/iou_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/to_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/to_dense_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/to_ragged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/to_ragged_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/validate_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/validate_format_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.010714 keras-aug-0.5.6/keras_aug/datapoints/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/image/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/image/get_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/image/get_matrix_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/image/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/image/ops_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.010714 keras-aug-0.5.6/keras_aug/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.010714 keras-aug-0.5.6/keras_aug/layers/__internal__/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/__internal__/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/__internal__/base_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/__internal__/base_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/__internal__/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/__internal__/graph_xla_mode_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14777 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/__internal__/mixed_precision_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15616 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/__internal__/output_common_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10399 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/__internal__/with_bounding_boxes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/__internal__/with_ragged_image_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.010714 keras-aug-0.5.6/keras_aug/layers/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.014714 keras-aug-0.5.6/keras_aug/layers/augmentation/auto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13037 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/auto/aug_mix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/auto/aug_mix_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/auto/rand_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/auto/rand_augment_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/auto/trivial_augment_wide.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/auto/trivial_augment_wide_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.018714 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23369 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_affine_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_crop_and_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_crop_and_resize_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_crop_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_flip_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_resize_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_rotate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14958 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_zoom_and_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_zoom_and_crop_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.022714 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/channel_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/channel_shuffle_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_blur_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_channel_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_channel_shift_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_clahe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_clahe_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_color_jitter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_gamma_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_gaussian_blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_gaussian_blur_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_hsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_hsv_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_jpeg_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_jpeg_quality_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_posterize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_posterize_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_sharpness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_sharpness_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_solarize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.022714 keras-aug-0.5.6/keras_aug/layers/augmentation/mix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/mix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/mix/cut_mix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/mix/cut_mix_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/mix/mix_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/mix/mix_up_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/mix/mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/mix/mosaic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.026714 keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_channel_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_channel_dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_cutout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_cutout_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_erase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_erase_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_grid_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_grid_mask_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.026714 keras-aug-0.5.6/keras_aug/layers/augmentation/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/utility/random_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/utility/random_apply_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/utility/random_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/utility/random_choice_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/utility/repeated_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/utility/repeated_augment_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.030714 keras-aug-0.5.6/keras_aug/layers/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24353 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/base/vectorized_base_random_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22106 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/base/vectorized_base_random_layer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.030714 keras-aug-0.5.6/keras_aug/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.030714 keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/center_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/center_crop_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/pad_if_needed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/pad_if_needed_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15643 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23172 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/resize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.030714 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/auto_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/auto_contrast_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/equalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/equalize_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/grayscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/grayscale_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/identity_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/invert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/invert_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/normalize_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/rescale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/rescale_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.034714 keras-aug-0.5.6/keras_aug/layers/preprocessing/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/utility/sanitize_bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/utility/sanitize_bounding_box_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.034714 keras-aug-0.5.6/keras_aug/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/utils/augmentation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/utils/conditional_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/utils/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/utils/distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.002714 keras-aug-0.5.6/keras_aug.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26898 2023-07-01 09:12:12.000000 keras-aug-0.5.6/keras_aug.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-01 09:12:12.000000 keras-aug-0.5.6/keras_aug.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 09:12:12.000000 keras-aug-0.5.6/keras_aug.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-01 09:12:12.000000 keras-aug-0.5.6/keras_aug.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 09:12:12.000000 keras-aug-0.5.6/keras_aug.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-01 09:11:37.000000 keras-aug-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 09:12:13.034714 keras-aug-0.5.6/setup.cfg
```

### Comparing `keras-aug-0.5.5/LICENSE` & `keras-aug-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/PKG-INFO` & `keras-aug-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-aug
-Version: 0.5.5
+Version: 0.5.6
 Summary: A library that includes pure TF/Keras preprocessing and augmentation layers
 Author: Hongyu, Chiu (james77777778)
 License:    Copyright 2023 The KerasAug Authors. All rights reserved.
         
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -207,15 +207,15 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: homepage, https://github.com/james77777778/keras-aug
 Project-URL: repository, https://github.com/james77777778/keras-aug
 Project-URL: documentation, https://kerasaug.readthedocs.io/en/latest/
-Keywords: tensorflow,keras,keras-cv,preprocessing,augmentation
+Keywords: tensorflow,keras,preprocessing,augmentation
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -233,15 +233,14 @@
 License-File: LICENSE
 
 <!-- markdownlint-disable MD033 -->
 # KerasAug
 
 ![Python](https://img.shields.io/badge/python-v3.8.0+-success.svg)
 ![Tensorflow](https://img.shields.io/badge/tensorflow-v2.12.0+-success.svg)
-![KerasCV](https://img.shields.io/badge/keras_cv-v0.5.0+-success.svg)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/james77777778/keras-aug/actions.yml?label=tests)](https://github.com/james77777778/keras-aug/actions/workflows/actions.yml?query=branch%3Amain++)
 [![codecov](https://codecov.io/gh/james77777778/keras-aug/branch/main/graph/badge.svg?token=81ELI3VH7H)](https://codecov.io/gh/james77777778/keras-aug)
 [![PyPI](https://img.shields.io/pypi/v/keras-aug)](https://pypi.org/project/keras-aug/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/keras-aug)
 [![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/james77777778/keras-aug/issues)
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://james77777778-keras-aug-streamlit-appapp-mxd7v1.streamlit.app/)
 
@@ -297,20 +296,17 @@
 
     > **Note**
     > The degenerate bounding boxes (those located at the bottom of the image) are removed.
 
 ## Installation
 
 ```bash
-pip install keras-aug keras-cv tensorflow --upgrade
+pip install keras-aug tensorflow --upgrade
 ```
 
-> **Warning**
-> KerasAug is NOT compatible with `keras-cv < 0.5.0`.
-
 ## Quickstart
 
 <details>
 <summary>Rock, Paper and Scissors Image Classification</summary>
 
 ```python
 import keras_aug
@@ -433,15 +429,15 @@
         path=path,
         dpi=150,
     )
 
 
 def unpackage_raw_tfds_inputs(inputs, bounding_box_format):
     image = inputs["image"]
-    boxes = keras_cv.bounding_box.convert_format(
+    boxes = keras_aug.datapoints.bounding_box.convert_format(
         inputs["objects"]["bbox"],
         images=image,
         source="rel_yxyx",
         target=bounding_box_format,
     )
     bounding_boxes = {
         "classes": tf.cast(inputs["objects"]["label"], dtype=tf.float32),
```

### Comparing `keras-aug-0.5.5/README.md` & `keras-aug-0.5.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!-- markdownlint-disable MD033 -->
 # KerasAug
 
 ![Python](https://img.shields.io/badge/python-v3.8.0+-success.svg)
 ![Tensorflow](https://img.shields.io/badge/tensorflow-v2.12.0+-success.svg)
-![KerasCV](https://img.shields.io/badge/keras_cv-v0.5.0+-success.svg)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/james77777778/keras-aug/actions.yml?label=tests)](https://github.com/james77777778/keras-aug/actions/workflows/actions.yml?query=branch%3Amain++)
 [![codecov](https://codecov.io/gh/james77777778/keras-aug/branch/main/graph/badge.svg?token=81ELI3VH7H)](https://codecov.io/gh/james77777778/keras-aug)
 [![PyPI](https://img.shields.io/pypi/v/keras-aug)](https://pypi.org/project/keras-aug/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/keras-aug)
 [![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/james77777778/keras-aug/issues)
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://james77777778-keras-aug-streamlit-appapp-mxd7v1.streamlit.app/)
 
@@ -63,20 +62,17 @@
 
     > **Note**
     > The degenerate bounding boxes (those located at the bottom of the image) are removed.
 
 ## Installation
 
 ```bash
-pip install keras-aug keras-cv tensorflow --upgrade
+pip install keras-aug tensorflow --upgrade
 ```
 
-> **Warning**
-> KerasAug is NOT compatible with `keras-cv < 0.5.0`.
-
 ## Quickstart
 
 <details>
 <summary>Rock, Paper and Scissors Image Classification</summary>
 
 ```python
 import keras_aug
@@ -199,15 +195,15 @@
         path=path,
         dpi=150,
     )
 
 
 def unpackage_raw_tfds_inputs(inputs, bounding_box_format):
     image = inputs["image"]
-    boxes = keras_cv.bounding_box.convert_format(
+    boxes = keras_aug.datapoints.bounding_box.convert_format(
         inputs["objects"]["bbox"],
         images=image,
         source="rel_yxyx",
         target=bounding_box_format,
     )
     bounding_boxes = {
         "classes": tf.cast(inputs["objects"]["label"], dtype=tf.float32),
```

### Comparing `keras-aug-0.5.5/keras_aug/conftest.py` & `keras-aug-0.5.6/keras_aug/conftest.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/core/__init__.py` & `keras-aug-0.5.6/keras_aug/core/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/core/factor_sampler/constant_factor_sampler.py` & `keras-aug-0.5.6/keras_aug/core/factor_sampler/constant_factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/core/factor_sampler/constant_factor_sampler_test.py` & `keras-aug-0.5.6/keras_aug/core/factor_sampler/constant_factor_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/core/factor_sampler/factor_sampler.py` & `keras-aug-0.5.6/keras_aug/core/factor_sampler/factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/core/factor_sampler/normal_factor_sampler.py` & `keras-aug-0.5.6/keras_aug/core/factor_sampler/normal_factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/core/factor_sampler/normal_factor_sampler_test.py` & `keras-aug-0.5.6/keras_aug/core/factor_sampler/normal_factor_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/core/factor_sampler/signed_constant_factor_sampler.py` & `keras-aug-0.5.6/keras_aug/core/factor_sampler/signed_constant_factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/core/factor_sampler/signed_constant_factor_sampler_test.py` & `keras-aug-0.5.6/keras_aug/core/factor_sampler/signed_constant_factor_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/core/factor_sampler/signed_normal_factor_sampler.py` & `keras-aug-0.5.6/keras_aug/core/factor_sampler/signed_normal_factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/core/factor_sampler/signed_normal_factor_sampler_test.py` & `keras-aug-0.5.6/keras_aug/core/factor_sampler/signed_normal_factor_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/core/factor_sampler/uniform_factor_sampler.py` & `keras-aug-0.5.6/keras_aug/core/factor_sampler/uniform_factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/core/factor_sampler/uniform_factor_sampler_test.py` & `keras-aug-0.5.6/keras_aug/core/factor_sampler/uniform_factor_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/__init__.py` & `keras-aug-0.5.6/keras_aug/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/__internal__/base_layer.py` & `keras-aug-0.5.6/keras_aug/layers/__internal__/base_layer.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/__internal__/base_layer_test.py` & `keras-aug-0.5.6/keras_aug/layers/__internal__/base_layer_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/__internal__/config_test.py` & `keras-aug-0.5.6/keras_aug/layers/__internal__/config_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/__internal__/graph_xla_mode_test.py` & `keras-aug-0.5.6/keras_aug/layers/__internal__/graph_xla_mode_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/__internal__/mixed_precision_test.py` & `keras-aug-0.5.6/keras_aug/layers/__internal__/mixed_precision_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import inspect
 
 import tensorflow as tf
 from absl.testing import parameterized
-from keras_cv import bounding_box
 from tensorflow import keras
 
 from keras_aug import layers
+from keras_aug.datapoints import bounding_box
 from keras_aug.layers import augmentation
 from keras_aug.layers import preprocessing
 from keras_aug.utils.augmentation import BOUNDING_BOXES
 from keras_aug.utils.augmentation import IMAGES
 from keras_aug.utils.augmentation import LABELS
 
 #   (
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/__internal__/output_common_test.py` & `keras-aug-0.5.6/keras_aug/layers/__internal__/output_common_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         layers.ChannelShuffle,
         {"groups": 3},
         True,
     ),
     (
         "RandomBlur",
         layers.RandomBlur,
-        {"factor": (3, 7)},
+        {"factor": (3, 7), "seed": 2024},
         True,
     ),
     (
         "RandomChannelShift",
         layers.RandomChannelShift,
         {"value_range": (0, 255), "factor": 0.1},
         True,
@@ -208,15 +208,15 @@
             "width": 100,
         },
         True,
     ),
     (
         "RandomChannelDropout",
         layers.RandomChannelDropout,
-        {},
+        {"seed": 2024},
         True,
     ),
     (
         "RandomCutout",
         layers.RandomCutout,
         {"height_factor": 0.3, "width_factor": 0.3},
         True,
@@ -368,15 +368,15 @@
     layers.MixUp,  # tf.convert_to_tensor
     layers.RandomCutout,  # tf.where with -1 (invalid bbox)
     layers.RandomHSV,  # stateless_random_uniform
     layers.RandomChannelShift,  # stateless_random_uniform
     layers.RandomColorJitter,  # stateless_random_uniform
     layers.RandomGamma,  # stateless_random_uniform
     layers.RandomGaussianBlur,  # tf.nn.depthwise_conv2d
-    layers.RandomJpegQuality,  # preprocessing_utils.transform_value_range
+    layers.RandomJpegQuality,  # image_utils.transform_value_range
     layers.AutoContrast,  # tf.convert_to_tensor
     layers.Grayscale,  # tf.mul
     layers.Normalize,  # mean, std
 ]
 
 SKIP_DTYPE = [
     # it is hard to change dtype in runtime
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/__internal__/with_bounding_boxes_test.py` & `keras-aug-0.5.6/keras_aug/layers/__internal__/with_bounding_boxes_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 
 import tensorflow as tf
 from absl.testing import parameterized
-from keras_cv import bounding_box
 
 from keras_aug import layers
+from keras_aug.datapoints import bounding_box
 from keras_aug.layers import augmentation
 from keras_aug.layers import preprocessing
 from keras_aug.utils.augmentation import BOUNDING_BOXES
 from keras_aug.utils.augmentation import IMAGES
 from keras_aug.utils.augmentation import LABELS
 
 #   (
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/__internal__/with_ragged_image_test.py` & `keras-aug-0.5.6/keras_aug/layers/__internal__/with_ragged_image_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/__init__.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/auto/aug_mix.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/auto/aug_mix.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import tensorflow as tf
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
 from keras_aug import layers
+from keras_aug.datapoints import image as image_utils
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
 from keras_aug.utils.augmentation import H_AXIS
 from keras_aug.utils.augmentation import IMAGES
 from keras_aug.utils.augmentation import W_AXIS
@@ -116,27 +116,27 @@
         images = self.augment_images(
             images=images, transformations=transformations, **kwargs
         )
         return tf.squeeze(images, axis=0)
 
     def augment_images(self, images, transformations, **kwargs):
         original_shape = images.shape
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images, self.value_range, (0, 255), dtype=self.compute_dtype
         )
         inputs_for_aug_mix_single_image = {
             IMAGES: images,
             "transformations": transformations,
         }
         images = tf.map_fn(
             self.aug_mix_single_image,
             inputs_for_aug_mix_single_image,
             fn_output_signature=self.compute_dtype,
         )
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images, (0, 255), self.value_range, self.compute_dtype
         )
         images = tf.ensure_shape(images, shape=original_shape)
         return images
 
     def augment_labels(self, labels, transformations, **kwargs):
         return labels
@@ -258,69 +258,69 @@
         height = tf.expand_dims(tf.shape(image)[H_AXIS : H_AXIS + 1], axis=0)
         width = tf.expand_dims(tf.shape(image)[W_AXIS : W_AXIS + 1], axis=0)
         height = tf.cast(height, dtype=tf.float32)
         width = tf.cast(width, dtype=tf.float32)
         # tf.raw_ops.ImageProjectiveTransformV3 not support bfloat16
         if image.dtype == tf.bfloat16:
             image = tf.cast(image, dtype=tf.float32)
-        image = preprocessing_utils.transform(
+        image = image_utils.transform(
             tf.expand_dims(image, axis=0),
-            augmentation_utils.get_rotation_matrix(angle, height, width),
+            image_utils.get_rotation_matrix(angle, height, width),
         )
         image = tf.squeeze(image, axis=0)
         return tf.cast(image, dtype=self.compute_dtype)
 
     def solarize(self, image):
         threshold = tf.cast(
             tf.cast(self.severity() * 255, tf.int32), image.dtype
         )
         image = tf.where(image < threshold, image, 255 - image)
         return image
 
     def shear(self, image, along_x=True):
         factor = tf.cast(self.severity() * 0.3, tf.float32)
-        factor *= preprocessing_utils.random_inversion(self._random_generator)
+        factor *= augmentation_utils.random_inversion(self._random_generator)
         if along_x:
             transform = tf.convert_to_tensor(
                 [1.0, factor, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0]
             )
         else:
             transform = tf.convert_to_tensor(
                 [1.0, 0.0, 0.0, factor, 1.0, 0.0, 0.0, 0.0]
             )
         # tf.raw_ops.ImageProjectiveTransformV3 not support bfloat16
         if image.dtype == tf.bfloat16:
             image = tf.cast(image, dtype=tf.float32)
-        image = preprocessing_utils.transform(
+        image = image_utils.transform(
             tf.expand_dims(image, axis=0),
             tf.expand_dims(transform, axis=0),
         )
         image = tf.squeeze(image, axis=0)
         return tf.cast(image, dtype=self.compute_dtype)
 
     def translate(self, image, along_x=True):
         shape = tf.cast(tf.shape(image), tf.float32)
         if along_x:
             size = shape[1]
         else:
             size = shape[0]
         factor = tf.cast(self.severity() * size / 3, tf.float32)
-        factor *= preprocessing_utils.random_inversion(self._random_generator)
+        factor *= augmentation_utils.random_inversion(self._random_generator)
         if along_x:
             transform = tf.convert_to_tensor(
                 [1.0, 0.0, factor, 0.0, 1.0, 0.0, 0.0, 0.0]
             )
         else:
             transform = tf.convert_to_tensor(
                 [1.0, 0.0, 0.0, 0.0, 1.0, factor, 0.0, 0.0]
             )
         # tf.raw_ops.ImageProjectiveTransformV3 not support bfloat16
         if image.dtype == tf.bfloat16:
             image = tf.cast(image, dtype=tf.float32)
-        image = preprocessing_utils.transform(
+        image = image_utils.transform(
             tf.expand_dims(image, axis=0),
             tf.expand_dims(transform, axis=0),
         )
         image = tf.squeeze(image, axis=0)
         return tf.cast(image, dtype=self.compute_dtype)
 
     def get_config(self):
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/auto/aug_mix_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/auto/aug_mix_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/auto/rand_augment.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/auto/rand_augment.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from functools import partial
 
 import tensorflow as tf
-from keras_cv import bounding_box
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
 from keras_aug import layers
 from keras_aug.core import NormalFactorSampler
 from keras_aug.core import SignedNormalFactorSampler
+from keras_aug.datapoints import bounding_box
+from keras_aug.datapoints import image as image_utils
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
 from keras_aug.utils.augmentation import BOUNDING_BOXES
 from keras_aug.utils.augmentation import IMAGES
 
@@ -59,15 +59,15 @@
             ``"reflect"``.
         fill_value (int|float, optional): The value to be filled outside the
             boundaries when ``fill_mode="constant"``. Defaults to ``0``.
         exclude_ops (list(str), optional): Exclude selected operations.
             Defaults to ``None``.
         bounding_box_format (str, optional): The format of bounding
             boxes of input dataset. Refer
-            https://github.com/keras-team/keras-cv/blob/master/keras_cv/bounding_box/converters.py
+            https://github.com/james77777778/keras-aug/blob/main/keras_aug/datapoints/bounding_box/converter.py
             for more details on supported bounding box formats.
         seed (int|float, optional): The random seed. Defaults to ``None``.
 
     References:
         - `RandAugment <https://arxiv.org/abs/1909.13719>`_
         - `Tensorflow Model augment <https://github.com/tensorflow/models/blob/v2.12.0/official/vision/ops/augment.py>`_
         - `torchvision <https://github.com/pytorch/vision>`_
@@ -268,15 +268,15 @@
 
     def _batch_augment(self, inputs):
         images = inputs.get(augmentation_utils.IMAGES, None)
         batch_size = tf.shape(images)[0]
         transformations = self.get_random_transformation_batch(batch_size)
 
         # images value_range transform to [0, 255]
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images, self.value_range, (0, 255), dtype=self.compute_dtype
         )
         inputs[IMAGES] = images
 
         bounding_boxes = inputs.get(BOUNDING_BOXES, None)
         # make bounding_boxes to dense first
         if bounding_boxes is not None:
@@ -301,15 +301,15 @@
                 bounding_boxes = bounding_box.to_ragged(bounding_boxes)
             else:
                 bounding_boxes = bounding_box.to_dense(bounding_boxes)
             result[BOUNDING_BOXES] = bounding_boxes
 
         # recover value_range
         images = result.get(IMAGES, None)
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images, (0, 255), self.value_range, self.compute_dtype
         )
         result[IMAGES] = images
         return result
 
     def rand_augment_single_input(self, inputs):
         input = inputs.get("inputs")
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/auto/rand_augment_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/auto/rand_augment_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/auto/trivial_augment_wide.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/auto/trivial_augment_wide.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from functools import partial
 
 import tensorflow as tf
-from keras_cv import bounding_box
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
 from keras_aug import layers
 from keras_aug.core import UniformFactorSampler
+from keras_aug.datapoints import bounding_box
+from keras_aug.datapoints import image as image_utils
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
 from keras_aug.utils.augmentation import BOUNDING_BOXES
 from keras_aug.utils.augmentation import IMAGES
 
@@ -46,15 +46,15 @@
             ``"reflect"``.
         fill_value (int|float, optional): The value to be filled outside the
             boundaries when ``fill_mode="constant"``. Defaults to ``0``.
         exclude_ops (list(str), optional): Exclude selected operations.
             Defaults to ``None``.
         bounding_box_format (str, optional): The format of bounding
             boxes of input dataset. Refer
-            https://github.com/keras-team/keras-cv/blob/master/keras_cv/bounding_box/converters.py
+            https://github.com/james77777778/keras-aug/blob/main/keras_aug/datapoints/bounding_box/converter.py
             for more details on supported bounding box formats.
         seed (int|float, optional): The random seed. Defaults to ``None``.
 
     References:
         - `TrivialAugment <https://arxiv.org/abs/2103.10158>`_
         - `TrivialAugment Official Repo <https://github.com/automl/trivialaugment>`_
         - `torchvision <https://github.com/pytorch/vision>`_
@@ -259,15 +259,15 @@
 
     def _batch_augment(self, inputs):
         images = inputs.get(augmentation_utils.IMAGES, None)
         batch_size = tf.shape(images)[0]
         transformations = self.get_random_transformation_batch(batch_size)
 
         # images value_range transform to [0, 255]
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images, self.value_range, (0, 255), dtype=self.compute_dtype
         )
         inputs[IMAGES] = images
 
         bounding_boxes = inputs.get(BOUNDING_BOXES, None)
         # make bounding_boxes to dense first
         if bounding_boxes is not None:
@@ -292,15 +292,15 @@
                 bounding_boxes = bounding_box.to_ragged(bounding_boxes)
             else:
                 bounding_boxes = bounding_box.to_dense(bounding_boxes)
             result[BOUNDING_BOXES] = bounding_boxes
 
         # recover value_range
         images = result.get(IMAGES, None)
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images, (0, 255), self.value_range, self.compute_dtype
         )
         result[IMAGES] = images
         return result
 
     def trivial_augment_single_input(self, inputs):
         input = inputs.get("inputs")
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_affine.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_affine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import math
 
 import tensorflow as tf
-from keras_cv import bounding_box
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
+from keras_aug.datapoints import bounding_box
+from keras_aug.datapoints import image as image_utils
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
-from keras_aug.utils import bounding_box as bounding_box_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
 class RandomAffine(VectorizedBaseRandomLayer):
     """Randomly affines transformation of the images keeping center invariant.
 
     Randomly affines by rotation, translation, zoom and shear. RandomAffine
@@ -64,15 +63,15 @@
         fill_mode (str, optional): The fill mode. Supported values:
             ``"constant", "reflect", "wrap", "nearest"``. Defaults to
             ``"constant"``.
         fill_value (int|float, optional): The value to be filled outside the
             boundaries when ``fill_mode="constant"``. Defaults to ``0``.
         bounding_box_format (str, optional): The format of bounding
             boxes of input dataset. Refer
-            https://github.com/keras-team/keras-cv/blob/master/keras_cv/bounding_box/converters.py
+            https://github.com/james77777778/keras-aug/blob/main/keras_aug/datapoints/bounding_box/converter.py
             for more details on supported bounding box formats.
         bounding_box_min_area_ratio (float, optional): The threshold to
             apply sanitize_bounding_boxes. Defaults to ``None``.
         bounding_box_max_aspect_ratio (float, optional): The threshold to
             apply sanitize_bounding_boxes. Defaults to ``None``.
         seed (int|float, optional): The random seed. Defaults to ``None``.
 
@@ -166,15 +165,15 @@
                 max_value=1,
                 center_value=0.0,
                 seed=seed,
             )
 
         self.same_zoom_factor = same_zoom_factor
 
-        preprocessing_utils.check_fill_mode_and_interpolation(
+        augmentation_utils.check_fill_mode_and_interpolation(
             fill_mode, interpolation
         )
         self.interpolation = interpolation
         self.fill_mode = fill_mode
         self.fill_value = fill_value
         self.bounding_box_format = bounding_box_format
         self.bounding_box_min_area_ratio = bounding_box_min_area_ratio
@@ -273,33 +272,33 @@
                 tf.ones((batch_size, 1), dtype=tf.float32),
             ],
             axis=1,
         )
         combined_matrixes = tf.reshape(identity_matrixes, (batch_size, 3, 3))
         # process zoom
         if self._enable_zoom:
-            zoom_matrixes = augmentation_utils.get_zoom_matrix(
+            zoom_matrixes = image_utils.get_zoom_matrix(
                 zooms, heights, widths, to_square=True
             )
             combined_matrixes = zoom_matrixes @ combined_matrixes
         # process rotations
         if self._enable_rotation:
-            rotation_matrixes = augmentation_utils.get_rotation_matrix(
+            rotation_matrixes = image_utils.get_rotation_matrix(
                 angles, heights, widths, to_square=True
             )
             combined_matrixes = rotation_matrixes @ combined_matrixes
         # process shear
         if self._enable_shear:
-            shear_matrixes = augmentation_utils.get_shear_matrix(
+            shear_matrixes = image_utils.get_shear_matrix(
                 shears, to_square=True
             )
             combined_matrixes = shear_matrixes @ combined_matrixes
         # process translations
         if self._enable_translation:
-            translation_matrixes = augmentation_utils.get_translation_matrix(
+            translation_matrixes = image_utils.get_translation_matrix(
                 translations, heights, widths, to_square=True
             )
             combined_matrixes = translation_matrixes @ combined_matrixes
         return {
             "angles": angles,
             "translations": translations,
             "zooms": zooms,
@@ -325,15 +324,15 @@
             combined_matrixes, shape=(batch_size, -1)
         )
         combined_matrixes = combined_matrixes[:, :-1]
 
         # tf.raw_ops.ImageProjectiveTransformV3 not support bfloat16
         if images.dtype == tf.bfloat16:
             images = tf.cast(images, dtype=tf.float32)
-        images = preprocessing_utils.transform(
+        images = image_utils.transform(
             images,
             combined_matrixes,
             fill_mode=self.fill_mode,
             fill_value=self.fill_value,
             interpolation=self.interpolation,
         )
         images = tf.ensure_shape(images, shape=ori_shape)
@@ -450,20 +449,20 @@
             x2s = (x2s - x_offsets) / zoom_widths
             y1s = (y1s - y_offsets) / zoom_heights
             y2s = (y2s - y_offsets) / zoom_heights
             boxes = tf.concat([x1s, y1s, x2s, y2s], axis=-1)
 
         bounding_boxes = bounding_boxes.copy()
         bounding_boxes["boxes"] = boxes
-        bounding_boxes = bounding_box_utils.clip_to_image(
+        bounding_boxes = bounding_box.clip_to_image(
             bounding_boxes,
             bounding_box_format="xyxy",
             images=raw_images,
         )
-        bounding_boxes = bounding_box_utils.sanitize_bounding_boxes(
+        bounding_boxes = bounding_box.sanitize_bounding_boxes(
             bounding_boxes,
             min_area_ratio=self.bounding_box_min_area_ratio,
             max_aspect_ratio=self.bounding_box_max_aspect_ratio,
             bounding_box_format="xyxy",
             reference_bounding_boxes=original_bounding_boxes,
             images=raw_images,
             reference_images=raw_images,
@@ -501,15 +500,15 @@
             combined_matrixes, shape=(batch_size, -1)
         )
         combined_matrixes = combined_matrixes[:, :-1]
 
         # tf.raw_ops.ImageProjectiveTransformV3 not support bfloat16
         if segmentation_masks.dtype == tf.bfloat16:
             segmentation_masks = tf.cast(segmentation_masks, dtype=tf.float32)
-        segmentation_masks = preprocessing_utils.transform(
+        segmentation_masks = image_utils.transform(
             segmentation_masks,
             combined_matrixes,
             fill_mode=self.fill_mode,
             fill_value=0,
             interpolation="nearest",
         )
         segmentation_masks = tf.ensure_shape(
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_affine_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_affine_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import tensorflow as tf
-from keras_cv import bounding_box
+from keras_aug.datapoints import bounding_box
 
 from keras_aug import layers
 
 
 class RandomAffineTest(tf.test.TestCase):
     regular_args = {
         "rotation_factor": 10,
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_crop.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_crop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import tensorflow as tf
-from keras_cv import bounding_box
 from tensorflow import keras
 
+from keras_aug.datapoints import bounding_box
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
-from keras_aug.utils import bounding_box as bounding_box_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
 class RandomCrop(VectorizedBaseRandomLayer):
     """Randomly crops the input images.
 
     This layer will randomly choose a location to crop images down to
@@ -21,15 +20,15 @@
     Args:
         height (int): The height of result image.
         width (int): The width of result image.
         interpolation (str, optional): The interpolation mode. Supported values:
             ``"nearest", "bilinear"``. Defaults to `"bilinear"`.
         bounding_box_format (str, optional): The format of bounding
             boxes of input dataset. Refer
-            https://github.com/keras-team/keras-cv/blob/master/keras_cv/bounding_box/converters.py
+            https://github.com/james77777778/keras-aug/blob/main/keras_aug/datapoints/bounding_box/converter.py
             for more details on supported bounding box formats.
         bounding_box_min_area_ratio (float, optional): The threshold to
             apply sanitize_bounding_boxes. Defaults to ``None``.
         bounding_box_max_aspect_ratio (float, optional): The threshold to
             apply sanitize_bounding_boxes. Defaults to ``None``.
         seed (int|float, optional): The random seed. Defaults to ``None``.
 
@@ -153,20 +152,20 @@
             ),
             self.resize_bounding_boxes(
                 raw_images,
                 bounding_boxes["boxes"],
             ),
         )
         bounding_boxes["boxes"] = boxes
-        bounding_boxes = bounding_box_utils.clip_to_image(
+        bounding_boxes = bounding_box.clip_to_image(
             bounding_boxes,
             bounding_box_format="xyxy",
             images=images,
         )
-        bounding_boxes = bounding_box_utils.sanitize_bounding_boxes(
+        bounding_boxes = bounding_box.sanitize_bounding_boxes(
             bounding_boxes,
             min_area_ratio=self.bounding_box_min_area_ratio,
             max_aspect_ratio=self.bounding_box_max_aspect_ratio,
             bounding_box_format="xyxy",
             reference_bounding_boxes=original_bounding_boxes,
             images=images,
             reference_images=raw_images,
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_crop_and_resize.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_crop_and_resize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import tensorflow as tf
-from keras_cv import bounding_box
 from tensorflow import keras
 
 from keras_aug import core
+from keras_aug.datapoints import bounding_box
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
-from keras_aug.utils import bounding_box as bounding_box_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
 class RandomCropAndResize(VectorizedBaseRandomLayer):
     """Randomly crops a part of an image and resizes it to provided size.
 
     This implementation takes an intuitive approach, where we crop the images to
@@ -36,15 +35,15 @@
             a single float, the factor will be picked between
             ``[1.0 - factor, 1.0]``. For most tasks, this should be
             ``(3/4, 4/3)``.
         interpolation (str, optional): The interpolation mode. Supported values:
             ``"nearest", "bilinear"``. Defaults to `"bilinear"`.
         bounding_box_format (str, optional): The format of bounding
             boxes of input dataset. Refer
-            https://github.com/keras-team/keras-cv/blob/master/keras_cv/bounding_box/converters.py
+            https://github.com/james77777778/keras-aug/blob/main/keras_aug/datapoints/bounding_box/converter.py
             for more details on supported bounding box formats.
         seed (int|float, optional): The random seed. Defaults to ``None``.
 
     References:
         - `KerasCV <https://github.com/keras-team/keras-cv>`_
     """  # noqa: E501
 
@@ -203,15 +202,15 @@
                 (y2s - t_y1s) / t_dys,
             ],
             axis=-1,
         )
         bounding_boxes = bounding_boxes.copy()
         bounding_boxes["boxes"] = output
 
-        bounding_boxes = bounding_box_utils.clip_to_image(
+        bounding_boxes = bounding_box.clip_to_image(
             bounding_boxes,
             bounding_box_format="rel_xyxy",
             images=images,
         )
         bounding_boxes = bounding_box.convert_format(
             bounding_boxes,
             source="rel_xyxy",
@@ -275,28 +274,28 @@
         if (
             not isinstance(crop_area_factor, (tuple, list, core.FactorSampler))
             or isinstance(crop_area_factor, float)
             or isinstance(crop_area_factor, int)
         ):
             raise ValueError(
                 "`crop_area_factor` must be tuple of two positive floats less "
-                "than or equal to 1 or keras_cv.core.FactorSampler instance. "
+                "than or equal to 1 or keras_aug.core.FactorSampler instance. "
                 f"Received crop_area_factor={crop_area_factor}"
             )
 
         if (
             not isinstance(
                 aspect_ratio_factor, (tuple, list, core.FactorSampler)
             )
             or isinstance(aspect_ratio_factor, float)
             or isinstance(aspect_ratio_factor, int)
         ):
             raise ValueError(
                 "`aspect_ratio_factor` must be tuple of two positive floats or "
-                "keras_cv.core.FactorSampler instance. Received "
+                "keras_aug.core.FactorSampler instance. Received "
                 f"aspect_ratio_factor={aspect_ratio_factor}"
             )
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_crop_and_resize_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_crop_and_resize_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import tensorflow as tf
-from keras_cv import bounding_box
 
 from keras_aug import layers
+from keras_aug.datapoints import bounding_box
 
 
 class RandomCropAndResizeTest(tf.test.TestCase):
     ori_height, ori_width = 300, 300
     height, width = 224, 224
     regular_args = {
         "height": 224,
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_crop_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_crop_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_flip.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_flip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import tensorflow as tf
-from keras_cv import bounding_box
 from tensorflow import keras
 
+from keras_aug.datapoints import bounding_box
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
-from keras_aug.utils import bounding_box as bounding_box_utils
 
 # Defining modes for random flipping
 HORIZONTAL = "horizontal"
 VERTICAL = "vertical"
 HORIZONTAL_AND_VERTICAL = "horizontal_and_vertical"
 
 
@@ -27,15 +26,15 @@
             ``"horizontal"``. ``"horizontal"`` is a left-right flip and
             ``"vertical"`` is a top-bottom flip.
         rate (float, optional): The frequency of flipping. ``1.0`` indicates
             that images are always flipped. ``0.0`` indicates no flipping.
             Defaults to ``0.5``.
         bounding_box_format (str, optional): The format of bounding
             boxes of input dataset. Refer
-            https://github.com/keras-team/keras-cv/blob/master/keras_cv/bounding_box/converters.py
+            https://github.com/james77777778/keras-aug/blob/main/keras_aug/datapoints/bounding_box/converter.py
             for more details on supported bounding box formats.
         seed (int|float, optional): The random seed. Defaults to ``None``.
 
     References:
         - `KerasCV <https://github.com/keras-team/keras-cv>`_
     """  # noqa: E501
 
@@ -136,15 +135,15 @@
             boxes = tf.where(
                 flip_verticals > (1.0 - self.rate),
                 self.flip_boxes_vertical(boxes),
                 boxes,
             )
         bounding_boxes = bounding_boxes.copy()
         bounding_boxes["boxes"] = boxes
-        bounding_boxes = bounding_box_utils.clip_to_image(
+        bounding_boxes = bounding_box.clip_to_image(
             bounding_boxes,
             bounding_box_format="rel_xyxy",
             images=raw_images,
         )
         bounding_boxes = bounding_box.convert_format(
             bounding_boxes,
             source="rel_xyxy",
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_flip_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_flip_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 import numpy as np
 import tensorflow as tf
 from absl.testing import parameterized
-from keras_cv import bounding_box
 
 from keras_aug import layers
+from keras_aug.datapoints import bounding_box
 
 
 class RandomFlipTest(tf.test.TestCase, parameterized.TestCase):
     def test_horizontal_flip(self):
         np.random.seed(1337)
         mock_random = tf.convert_to_tensor([[0.6], [0.6]])
         inp = np.random.random((2, 5, 8, 3))
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_resize.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_resize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import typing
 
 import tensorflow as tf
-from keras_cv import bounding_box
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
+from keras_aug.datapoints import bounding_box
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
@@ -28,15 +27,15 @@
         interpolation (str, optional): The interpolation mode.
             Supported values: ``"nearest", "bilinear"``. Defaults to
             ``"bilinear"``.
         antialias (bool, optional): Whether to use antialias. Defaults to
             ``False``.
         bounding_box_format (str, optional): The format of bounding
             boxes of input dataset. Refer
-            https://github.com/keras-team/keras-cv/blob/master/keras_cv/bounding_box/converters.py
+            https://github.com/james77777778/keras-aug/blob/main/keras_aug/datapoints/bounding_box/converter.py
             for more details on supported bounding box formats.
         seed (int|float, optional): The random seed. Defaults to ``None``.
     """  # noqa: E501
 
     def __init__(
         self,
         heights,
@@ -61,17 +60,15 @@
                 f"int. Received: `heights`={heights}, `widths`={widths}"
             )
         if len(self.heights) != len(self.widths):
             raise ValueError(
                 "RandomResize expects `heights` and `widths` to be same "
                 f"length. Received: `heights`={heights}, `widths`={widths}"
             )
-        self.interpolation = preprocessing_utils.get_interpolation(
-            interpolation
-        )
+        self.interpolation = augmentation_utils.get_interpolation(interpolation)
         self.antialias = antialias
         self.bounding_box_format = bounding_box_format
         self.seed = seed
 
         self._heights = tf.convert_to_tensor(self.heights, dtype=tf.int32)
         self._widths = tf.convert_to_tensor(self.widths, dtype=tf.int32)
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_resize_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_resize_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import tensorflow as tf
-from keras_cv import bounding_box
 
 from keras_aug import layers
+from keras_aug.datapoints import bounding_box
 
 
 class RandomResizeTest(tf.test.TestCase):
     height, width = 224, 448
     regular_args = {
         "heights": [224],
         "interpolation": "bilinear",
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_rotate.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_rotate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import math
 
 import tensorflow as tf
-from keras_cv import bounding_box
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
+from keras_aug.datapoints import bounding_box
+from keras_aug.datapoints import image as image_utils
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
-from keras_aug.utils import bounding_box as bounding_box_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
 class RandomRotate(VectorizedBaseRandomLayer):
     """Randomly rotates the input images.
 
     The unit of the factor is degree. A positive value means rotating counter
@@ -30,15 +29,15 @@
         fill_mode (str, optional): The fill mode. Supported values:
             ``"constant", "reflect", "wrap", "nearest"``. Defaults to
             ``"constant"``.
         fill_value (int|float, optional): The value to be filled outside the
             boundaries when ``fill_mode="constant"``. Defaults to ``0``.
         bounding_box_format (str, optional): The format of bounding
             boxes of input dataset. Refer
-            https://github.com/keras-team/keras-cv/blob/master/keras_cv/bounding_box/converters.py
+            https://github.com/james77777778/keras-aug/blob/main/keras_aug/datapoints/bounding_box/converter.py
             for more details on supported bounding box formats.
         seed (int|float, optional): The random seed. Defaults to ``None``.
 
     References:
         - `KerasCV <https://github.com/keras-team/keras-cv>`_
     """  # noqa: E501
 
@@ -57,15 +56,15 @@
             factor,
             min_value=-180,
             max_value=180,
             center_value=0,
             seed=seed,
         )
 
-        preprocessing_utils.check_fill_mode_and_interpolation(
+        augmentation_utils.check_fill_mode_and_interpolation(
             fill_mode, interpolation
         )
         self.interpolation = interpolation
         self.fill_mode = fill_mode
         self.fill_value = fill_value
         self.bounding_box_format = bounding_box_format
         self.seed = seed
@@ -75,15 +74,15 @@
     ):
         # cast to float32 to avoid numerical issue
         heights, widths = augmentation_utils.get_images_shape(
             images, dtype=tf.float32
         )
         angles = self.factor(shape=(batch_size, 1), dtype=tf.float32)
         angles = angles / 360.0 * 2.0 * math.pi
-        rotation_matrixes = augmentation_utils.get_rotation_matrix(
+        rotation_matrixes = image_utils.get_rotation_matrix(
             angles, heights, widths, to_square=True
         )
         # (batch_size, 3, 3)
         return {
             "angles": angles,
             "rotation_matrixes": rotation_matrixes,
         }
@@ -106,15 +105,15 @@
             rotation_matrixes, shape=(batch_size, -1)
         )
         rotation_matrixes = rotation_matrixes[:, :-1]
 
         # tf.raw_ops.ImageProjectiveTransformV3 not support bfloat16
         if images.dtype == tf.bfloat16:
             images = tf.cast(images, dtype=tf.float32)
-        images = preprocessing_utils.transform(
+        images = image_utils.transform(
             images,
             rotation_matrixes,
             fill_mode=self.fill_mode,
             fill_value=self.fill_value,
             interpolation=self.interpolation,
         )
         images = tf.ensure_shape(images, shape=original_shape)
@@ -177,15 +176,15 @@
         out = tf.concat([new_x, new_y], axis=3)
         min_cordinates = tf.math.reduce_min(out, axis=2)
         max_cordinates = tf.math.reduce_max(out, axis=2)
         boxes = tf.concat([min_cordinates, max_cordinates], axis=2)
 
         bounding_boxes = bounding_boxes.copy()
         bounding_boxes["boxes"] = boxes
-        bounding_boxes = bounding_box_utils.clip_to_image(
+        bounding_boxes = bounding_box.clip_to_image(
             bounding_boxes,
             bounding_box_format="xyxy",
             images=raw_images,
         )
         # coordinates cannot be float values, it is cast to int32
         bounding_boxes = bounding_box.convert_format(
             bounding_boxes,
@@ -220,15 +219,15 @@
             rotation_matrixes, shape=(batch_size, -1)
         )
         rotation_matrixes = rotation_matrixes[:, :-1]
 
         # tf.raw_ops.ImageProjectiveTransformV3 not support bfloat16
         if segmentation_masks.dtype == tf.bfloat16:
             segmentation_masks = tf.cast(segmentation_masks, dtype=tf.float32)
-        segmentation_masks = preprocessing_utils.transform(
+        segmentation_masks = image_utils.transform(
             segmentation_masks,
             rotation_matrixes,
             fill_mode=self.fill_mode,
             fill_value=0,
             interpolation="nearest",
         )
         segmentation_masks = tf.ensure_shape(
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_rotate_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_rotate_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import tensorflow as tf
-from keras_cv import bounding_box
 
 from keras_aug import layers
+from keras_aug.datapoints import bounding_box
 
 
 class RandomRotationTest(tf.test.TestCase):
     regular_args = {
         "factor": 10,
         "fill_mode": "constant",
         "fill_value": 0,
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_zoom_and_crop.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_zoom_and_crop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import tensorflow as tf
-from keras_cv import bounding_box
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
+from keras_aug.datapoints import bounding_box
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
-from keras_aug.utils import bounding_box as bounding_box_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
 class RandomZoomAndCrop(VectorizedBaseRandomLayer):
     """RandomZoomAndCrop implements resize with scale distortion.
 
     RandomZoomAndCrop takes a three-step approach to size-distortion based image
@@ -50,15 +48,15 @@
         position (str, optional): The padding method.
             Supported values: ``"center", "top_left", "top_right", "bottom_left", "bottom_right", "random"``.
             Defaults to ``"center"``.
         padding_value (int|float, optional): The padding value.
             Defaults to ``0``.
         bounding_box_format (str, optional): The format of bounding
             boxes of input dataset. Refer
-            https://github.com/keras-team/keras-cv/blob/master/keras_cv/bounding_box/converters.py
+            https://github.com/james77777778/keras-aug/blob/main/keras_aug/datapoints/bounding_box/converter.py
             for more details on supported bounding box formats.
         seed (int|float, optional): The random seed. Defaults to ``None``.
 
     References:
         - `KerasCV <https://github.com/keras-team/keras-cv>`_
     """  # noqa: E501
 
@@ -90,17 +88,15 @@
         self.scale_factor = augmentation_utils.parse_factor(
             scale_factor,
             min_value=0.0,
             max_value=None,
             center_value=1.0,
             seed=seed,
         )
-        self.interpolation = preprocessing_utils.get_interpolation(
-            interpolation
-        )
+        self.interpolation = augmentation_utils.get_interpolation(interpolation)
         self.antialias = antialias
         self.position = augmentation_utils.get_padding_position(position)
         self.padding_value = padding_value
         self.bounding_box_format = bounding_box_format
         self.seed = seed
 
         crop_size = tf.expand_dims(
@@ -256,15 +252,15 @@
         bounding_boxes = bounding_boxes.copy()
         yxyx = bounding_boxes["boxes"]
         yxyx *= tf.tile(image_scales, [1, 2])[..., tf.newaxis, :]
         yxyx -= tf.tile(offsets, [1, 2])[..., tf.newaxis, :]
         yxyx += tf.tile(padding_offsets, [1, 2])[..., tf.newaxis, :]
 
         bounding_boxes["boxes"] = yxyx
-        bounding_boxes = bounding_box_utils.clip_to_image(
+        bounding_boxes = bounding_box.clip_to_image(
             bounding_boxes,
             bounding_box_format="yxyx",
             images=images,
         )
         bounding_boxes = bounding_box.convert_format(
             bounding_boxes,
             source="yxyx",
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_zoom_and_crop_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_zoom_and_crop_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import tensorflow as tf
 from absl.testing import parameterized
-from keras_cv import bounding_box
 
 from keras_aug import layers
+from keras_aug.datapoints import bounding_box
 
 
 class RandomZoomAndCropTest(tf.test.TestCase, parameterized.TestCase):
     batch_size = 4
     ori_height = 9
     ori_width = 8
     seed = 13
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/channel_shuffle.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/channel_shuffle.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/channel_shuffle_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/channel_shuffle_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_blur.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_blur.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import tensorflow as tf
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
+from keras_aug.utils import augmentation as augmentation_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
 class RandomBlur(VectorizedBaseRandomLayer):
     """Randomly blurs the images using random-sized kernels.
 
     This layer applies a mean filter with varying kernel sizes to blur the
@@ -31,29 +31,33 @@
         self,
         factor,
         seed=None,
         **kwargs,
     ):
         super().__init__(seed=seed, **kwargs)
         if isinstance(factor, (tuple, list)):
-            factor_range = (factor[1] - factor[0]) // 2
+            factor_range = (0, (factor[1] - factor[0]) // 2 + 1)
             factor_bias = factor[0]
         else:
-            factor_range = (factor[1] - 1) // 2
+            factor_range = (0, (factor - 1) // 2 + 1)
             factor_bias = 1
-        if factor_range < 0 or factor_bias < 1:
+        if factor_range[1] < 0 or factor_bias < 1:
             raise ValueError(
                 "RandomBlur expects `factor` to be in range `(1, inf)`. Got: "
                 f"`factor` = {factor}"
             )
         self.factor_input = factor
 
         self.factor_bias = factor_bias
-        self.factor = preprocessing_utils.parse_factor(
-            factor_range + 1, min_value=0, max_value=None, seed=seed
+        self.factor = augmentation_utils.parse_factor(
+            factor_range,
+            min_value=0,
+            max_value=None,
+            center_value=None,
+            seed=seed,
         )
         self.seed = seed
 
     def get_random_transformation_batch(self, batch_size, **kwargs):
         blur_kernel_sizes = self.factor(shape=(batch_size, 1), dtype=tf.int32)
         # [0, k] => [0, ..., 2k+1] ensures only odd numbers
         blur_kernel_sizes = blur_kernel_sizes * 2 + self.factor_bias
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_blur_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_blur_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_channel_shift.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_channel_shift.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
+from keras_aug.datapoints import image as image_utils
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
@@ -52,21 +52,21 @@
         transformations = tf.expand_dims(transformation, axis=0)
         images = self.augment_images(
             images=images, transformations=transformations, **kwargs
         )
         return tf.squeeze(images, axis=0)
 
     def augment_images(self, images, transformations=None, **kwargs):
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images, self.value_range, (0, 1), dtype=self.compute_dtype
         )
         shifts = transformations[:, tf.newaxis, tf.newaxis, :]
         images = images + shifts
         images = tf.clip_by_value(images, 0.0, 1.0)
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images, (0, 1), self.value_range, dtype=self.compute_dtype
         )
         return images
 
     def augment_labels(self, labels, transformations, **kwargs):
         return labels
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_channel_shift_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_channel_shift_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_clahe.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_clahe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
+from keras_aug.datapoints import image as image_utils
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
@@ -56,27 +56,27 @@
         transformation = tf.expand_dims(transformation, axis=0)
         image = self.augment_images(
             images=image, transformations=transformation, **kwargs
         )
         return tf.squeeze(image, axis=0)
 
     def augment_images(self, images, transformations, **kwargs):
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images, self.value_range, (0, 255), dtype=self.compute_dtype
         )
         inputs_for_clahe_single_image = {
             "images": images,
             "clip_limits": transformations,
         }
         images = tf.map_fn(
             self.clahe_single_image,
             inputs_for_clahe_single_image,
             fn_output_signature=self.compute_dtype,
         )
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images, (0, 255), self.value_range, dtype=self.compute_dtype
         )
         return images
 
     def augment_labels(self, labels, transformations, **kwargs):
         return labels
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_clahe_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_clahe_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_color_jitter.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_color_jitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
+from keras_aug.datapoints import image as image_utils
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
@@ -137,26 +137,26 @@
         )
         images = self.augment_images(
             images=images, transformations=transformations, **kwargs
         )
         return tf.squeeze(images, axis=0)
 
     def augment_images(self, images, transformations, **kwargs):
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images, self.value_range, (0, 255), dtype=self.compute_dtype
         )
         if self._enable_brightness:
             images = self.adjust_brightness(images, transformations)
         if self._enable_contrast:
             images = self.adjust_contrast(images, transformations)
         if self._enable_saturation:
             images = self.adjust_saturation(images, transformations)
         if self._enable_hue:
             images = self.adjust_hue(images, transformations)
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images, (0, 255), self.value_range, dtype=self.compute_dtype
         )
         return images
 
     def augment_labels(self, labels, transformations, **kwargs):
         return labels
 
@@ -179,24 +179,24 @@
 
     def adjust_contrast(self, images, transformations):
         # cast to float32 to avoid numerical issue
         contrast_factors = tf.cast(
             transformations["contrast_factors"], dtype=tf.float32
         )
         images = tf.cast(images, dtype=tf.float32)
-        degenerates = augmentation_utils.rgb_to_grayscale(images)
+        degenerates = image_utils.rgb_to_grayscale(images)
         degenerates = tf.reduce_mean(degenerates, axis=(1, 2, 3), keepdims=True)
-        images = augmentation_utils.blend(degenerates, images, contrast_factors)
+        images = image_utils.blend(degenerates, images, contrast_factors)
         images = tf.clip_by_value(images, 0, 255)
         return tf.cast(images, dtype=self.compute_dtype)
 
     def adjust_saturation(self, images, transformations):
         saturation_factors = transformations["saturation_factors"]
-        degenerates = augmentation_utils.rgb_to_grayscale(images)
-        images = augmentation_utils.blend(
+        degenerates = image_utils.rgb_to_grayscale(images)
+        images = image_utils.blend(
             degenerates, images, saturation_factors, (0, 255)
         )
         images = tf.clip_by_value(images, 0, 255)
         return images
 
     def adjust_hue(self, images, transformations):
         # cast to float32 to avoid numerical issue
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_color_jitter_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_color_jitter_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_gamma.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_gamma.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
+from keras_aug.datapoints import image as image_utils
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
@@ -53,20 +53,20 @@
         transformation = tf.expand_dims(transformation, axis=0)
         image = self.augment_images(
             images=image, transformations=transformation, **kwargs
         )
         return tf.squeeze(image, axis=0)
 
     def augment_images(self, images, transformations, **kwargs):
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images, self.value_range, (0.0, 1.0), dtype=self.compute_dtype
         )
         factors = transformations
         images = tf.pow(images, factors[:, :, tf.newaxis, tf.newaxis])
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images, (0.0, 1.0), self.value_range, dtype=self.compute_dtype
         )
         return images
 
     def augment_labels(self, labels, transformations, **kwargs):
         return labels
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_gamma_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_gamma_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_gaussian_blur.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_gaussian_blur_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_gaussian_blur_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_hsv.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_hsv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
+from keras_aug.datapoints import image as image_utils
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
@@ -121,24 +121,24 @@
         )
         images = self.augment_images(
             images=images, transformations=transformations, **kwargs
         )
         return tf.squeeze(images, axis=0)
 
     def augment_images(self, images, transformations, **kwargs):
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images, self.value_range, (0, 255), dtype=self.compute_dtype
         )
         if self._enable_hue:
             images = self.adjust_hue(images, transformations)
         if self._enable_saturation:
             images = self.adjust_saturation(images, transformations)
         if self._enable_value:
             images = self.adjust_value(images, transformations)
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images, (0, 255), self.value_range, dtype=self.compute_dtype
         )
         return images
 
     def augment_labels(self, labels, transformations, **kwargs):
         return labels
 
@@ -163,23 +163,23 @@
         )
         images = tf.image.hsv_to_rgb(images)
         images = tf.clip_by_value(images, 0, 255)
         return tf.cast(images, dtype=self.compute_dtype)
 
     def adjust_saturation(self, images, transformations):
         saturation_factors = transformations["saturation_factors"]
-        degenerates = augmentation_utils.rgb_to_grayscale(images)
-        images = augmentation_utils.blend(
+        degenerates = image_utils.rgb_to_grayscale(images)
+        images = image_utils.blend(
             degenerates, images, saturation_factors, (0, 255)
         )
         return images
 
     def adjust_value(self, images, transformations):
         value_factors = transformations["value_factors"]
-        images = augmentation_utils.blend(
+        images = image_utils.blend(
             tf.zeros_like(images), images, value_factors, (0, 255)
         )
         return images
 
     def get_config(self):
         config = super().get_config()
         config.update(
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_hsv_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_hsv_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_jpeg_quality.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_jpeg_quality.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Sequence
 
 import tensorflow as tf
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
 from keras_aug import core
+from keras_aug.datapoints import image as image_utils
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
@@ -73,26 +73,26 @@
         transformation = tf.expand_dims(transformation, axis=0)
         image = self.augment_images(
             images=image, transformations=transformation, **kwargs
         )
         return tf.squeeze(image, axis=0)
 
     def augment_images(self, images, transformations, **kwargs):
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images, self.value_range, target_range=(0, 1)
         )
         inputs_for_adjust_jpeg_qualitye = {
             "images": images,
             "factors": transformations,
         }
         images = tf.vectorized_map(
             self.adjust_jpeg_quality,
             inputs_for_adjust_jpeg_qualitye,
         )
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images, (0, 1), self.value_range, dtype=self.compute_dtype
         )
         return images
 
     def augment_labels(self, labels, transformations, **kwargs):
         return labels
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_jpeg_quality_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_jpeg_quality_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_posterize.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_posterize.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
+from keras_aug.datapoints import image as image_utils
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
@@ -58,30 +58,30 @@
         transformation = tf.expand_dims(transformation, axis=0)
         image = self.augment_images(
             images=image, transformations=transformation, **kwargs
         )
         return tf.squeeze(image, axis=0)
 
     def augment_images(self, images, transformations, **kwargs):
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images,
             original_range=self.value_range,
             target_range=(0, 255),
         )
         images = tf.cast(images, tf.uint8)
 
         inputs_for_posterize_single_image = {
             augmentation_utils.IMAGES: images,
             "bits": transformations,
         }
         images = tf.vectorized_map(
             self.posterize_single_image, inputs_for_posterize_single_image
         )
         images = tf.cast(images, self.compute_dtype)
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images,
             original_range=(0, 255),
             target_range=self.value_range,
             dtype=self.compute_dtype,
         )
         return images
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_posterize_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_posterize_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_sharpness.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_sharpness.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
+from keras_aug.datapoints import image as image_utils
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
@@ -55,15 +55,15 @@
     def augment_ragged_image(self, image, transformation, **kwargs):
         images = tf.expand_dims(image, axis=0)
         new_transformation = tf.expand_dims(transformation, axis=0)
         output = self.augment_images(images, new_transformation)
         return tf.squeeze(output, axis=0)
 
     def augment_images(self, images, transformations, **kwargs):
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images,
             original_range=self.value_range,
             target_range=(0, 255),
             dtype=self.compute_dtype,
         )
         original_images = images
         # [1 1 1]
@@ -95,18 +95,18 @@
         mask = tf.pad(mask, [[0, 0], [1, 1], [1, 1], [0, 0]])
         smoothed_image = tf.pad(
             smoothed_image, [[0, 0], [1, 1], [1, 1], [0, 0]]
         )
 
         images = tf.where(tf.equal(mask, 1), smoothed_image, original_images)
         # Blend the final result.
-        images = augmentation_utils.blend(
+        images = image_utils.blend(
             images, original_images, transformations, (0, 255)
         )
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images,
             original_range=(0, 255),
             target_range=self.value_range,
             dtype=self.compute_dtype,
         )
         return images
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_sharpness_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_sharpness_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_solarize.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_solarize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
+from keras_aug.datapoints import image as image_utils
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
@@ -88,24 +88,24 @@
             images=image, transformations=transformation, **kwargs
         )
         return tf.squeeze(image, axis=0)
 
     def augment_images(self, images, transformations, **kwargs):
         thresholds = transformations["thresholds"]
         additions = transformations["additions"]
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images,
             original_range=self.value_range,
             target_range=(0, 255),
             dtype=self.compute_dtype,
         )
         images = images + additions
         images = tf.clip_by_value(images, 0, 255)
         images = tf.where(images < thresholds, images, 255 - images)
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images,
             original_range=(0, 255),
             target_range=self.value_range,
             dtype=self.compute_dtype,
         )
         return images
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_solarize_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_solarize_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/mix/cut_mix.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/mix/cut_mix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
-from keras_cv.utils import fill_utils
 from tensorflow import keras
 
+from keras_aug.datapoints import image as image_utils
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils.augmentation import BATCHED
 from keras_aug.utils.augmentation import H_AXIS
 from keras_aug.utils.augmentation import LABELS
 from keras_aug.utils.augmentation import SEGMENTATION_MASKS
@@ -87,15 +87,15 @@
                 f"{type(images)}"
             )
         permutation_order = transformations["permutation_order"]
         center_xs = transformations["center_xs"]
         center_ys = transformations["center_ys"]
         cut_heights = transformations["cut_heights"]
         cut_widths = transformations["cut_widths"]
-        images = fill_utils.fill_rectangle(
+        images = image_utils.fill_rectangle(
             images,
             center_xs,
             center_ys,
             cut_widths,
             cut_heights,
             tf.gather(images, permutation_order),
         )
@@ -130,15 +130,15 @@
                 f"segmentation_masks type: {type(segmentation_masks)}"
             )
         permutation_order = transformations["permutation_order"]
         center_xs = transformations["center_xs"]
         center_ys = transformations["center_ys"]
         cut_heights = transformations["cut_heights"]
         cut_widths = transformations["cut_widths"]
-        segmentation_masks = fill_utils.fill_rectangle(
+        segmentation_masks = image_utils.fill_rectangle(
             segmentation_masks,
             center_xs,
             center_ys,
             cut_widths,
             cut_heights,
             tf.gather(segmentation_masks, permutation_order),
         )
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/mix/cut_mix_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/mix/cut_mix_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/mix/mix_up.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/mix/mix_up.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
-from keras_cv import bounding_box
 from tensorflow import keras
 
+from keras_aug.datapoints import bounding_box
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils.augmentation import BATCHED
 from keras_aug.utils.distribution import stateless_random_beta
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/mix/mix_up_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/mix/mix_up_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
-from keras_cv import bounding_box
 
 from keras_aug import layers
+from keras_aug.datapoints import bounding_box
 
 
 class MixUpTest(tf.test.TestCase):
     num_classes = 10
 
     def test_return_shapes(self):
         xs = tf.ones((2, 4, 4, 3))
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/mix/mosaic.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/mix/mosaic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import tensorflow as tf
-from keras_cv import bounding_box
 from tensorflow import keras
 
+from keras_aug.datapoints import bounding_box
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
-from keras_aug.utils import bounding_box as bounding_box_utils
 from keras_aug.utils.augmentation import BATCHED
 from keras_aug.utils.augmentation import BOUNDING_BOXES
 from keras_aug.utils.augmentation import IMAGES
 from keras_aug.utils.augmentation import LABELS
 from keras_aug.utils.augmentation import SEGMENTATION_MASKS
 
 
@@ -33,15 +32,15 @@
             sampled between the two values for every image augmented. When
             represented as a single float, the values will be picked between
             ``[0.5 - offset, 0.5 + offset]``. Defaults to ``(0.25, 0.75)``.
         fill_value (int|float, optional): The value to be filled outside the
             boundaries when ``fill_mode="constant"``. Defaults to ``0``.
         bounding_box_format (str, optional): The format of bounding
             boxes of input dataset. Refer
-            https://github.com/keras-team/keras-cv/blob/master/keras_cv/bounding_box/converters.py
+            https://github.com/james77777778/keras-aug/blob/main/keras_aug/datapoints/bounding_box/converter.py
             for more details on supported bounding box formats.
         seed (int|float, optional): The random seed. Defaults to ``None``.
 
     References:
         - `YOLOV4 <https://arxiv.org/abs/2004.10934>`_
         - `YOLOX Official Repo <https://github.com/Megvii-BaseDetection/YOLOX>`_
         - `ultralytics/ultralytics <https://github.com/ultralytics/ultralytics>`_
@@ -229,15 +228,15 @@
 
         boxes_for_mosaic = tf.reshape(boxes_for_mosaic, [batch_size, -1, 4])
         classes_for_mosaic = tf.reshape(classes_for_mosaic, [batch_size, -1])
         boxes_for_mosaic = {
             "boxes": boxes_for_mosaic,
             "classes": classes_for_mosaic,
         }
-        boxes_for_mosaic = bounding_box_utils.clip_to_image(
+        boxes_for_mosaic = bounding_box.clip_to_image(
             boxes_for_mosaic,
             bounding_box_format="xyxy",
             image_shape=(self.height, self.width, None),
         )
         boxes_for_mosaic = bounding_box.convert_format(
             boxes_for_mosaic,
             source="xyxy",
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/mix/mosaic_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/mix/mosaic_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_channel_dropout.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_channel_dropout.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import tensorflow as tf
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
+from keras_aug.utils import augmentation as augmentation_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
 class RandomChannelDropout(VectorizedBaseRandomLayer):
     """Randomly drop channels of the input images.
 
     Args:
@@ -29,15 +29,15 @@
         if isinstance(factor, (tuple, list)):
             lower = factor[0]
             upper = factor[1] + 1
         else:
             lower = 0
             upper = factor + 1
         self.factor_input = factor
-        self.factor = preprocessing_utils.parse_factor(
+        self.factor = augmentation_utils.parse_factor(
             (lower, upper), min_value=0, max_value=None, seed=seed
         )
         self.fill_value = fill_value
         self.seed = seed
 
         self.upper = upper
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_channel_dropout_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_channel_dropout_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_cutout.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_cutout.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import tensorflow as tf
-from keras_cv import bounding_box
-from keras_cv.bounding_box.iou import _compute_area
-from keras_cv.bounding_box.iou import _compute_intersection
-from keras_cv.utils import fill_utils
 from tensorflow import keras
 
+from keras_aug.datapoints import bounding_box
+from keras_aug.datapoints import image as image_utils
+from keras_aug.datapoints.bounding_box.iou import _compute_area
+from keras_aug.datapoints.bounding_box.iou import _compute_intersection
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
@@ -34,15 +34,15 @@
         fill_value (int|float, optional): The value to be filled in the cutout
             rectangle when ``fill_mode="constant"``. Defaults to ``0``.
         bbox_removal_threshold (float, optional): The bounding boxes having
             content cut above the threshold will be removed.
             Defaults to ``0.6`` which is applied by ultralytics/yolo series.
         bounding_box_format (str, optional): The format of bounding
             boxes of input dataset. Refer
-            https://github.com/keras-team/keras-cv/blob/master/keras_cv/bounding_box/converters.py
+            https://github.com/james77777778/keras-aug/blob/main/keras_aug/datapoints/bounding_box/converter.py
             for more details on supported bounding box formats.
         seed (int|float, optional): The random seed. Defaults to ``None``.
 
     References:
         - `Cutout <https://arxiv.org/abs/1708.04552>`_
         - `KerasCV <https://github.com/keras-team/keras-cv>`_
         - `kaushal2896@Kaggle <https://www.kaggle.com/code/kaushal2896/data-augmentation-tutorial-basic-cutout-mixup>`_
@@ -129,15 +129,15 @@
     def augment_images(self, images, transformations, **kwargs):
         images = tf.cast(images, dtype=self.compute_dtype)
         center_xs = transformations["center_xs"]
         center_ys = transformations["center_ys"]
         cutout_heights = transformations["cutout_heights"]
         cutout_widths = transformations["cutout_widths"]
         rectangle_fills = self.compute_rectangle_fills(images)
-        images = fill_utils.fill_rectangle(
+        images = image_utils.fill_rectangle(
             images,
             center_xs[..., 0],
             center_ys[..., 0],
             cutout_widths[..., 0],
             cutout_heights[..., 0],
             rectangle_fills,
         )
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_cutout_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_cutout_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_erase.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_erase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
-from keras_cv.utils import fill_utils
 from tensorflow import keras
 
+from keras_aug.datapoints import image as image_utils
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
@@ -133,15 +133,15 @@
     def augment_images(self, images, transformations, **kwargs):
         images = tf.cast(images, dtype=self.compute_dtype)
         center_xs = transformations["center_xs"]
         center_ys = transformations["center_ys"]
         erasing_heights = transformations["erasing_heights"]
         erasing_widths = transformations["erasing_widths"]
         rectangle_fills = self.compute_rectangle_fills(images)
-        images = fill_utils.fill_rectangle(
+        images = image_utils.fill_rectangle(
             images,
             center_xs[..., 0],
             center_ys[..., 0],
             erasing_widths[..., 0],
             erasing_heights[..., 0],
             rectangle_fills,
         )
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_erase_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_erase_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_grid_mask.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_grid_mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import math
 
 import tensorflow as tf
-from keras_cv.utils import fill_utils
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
+from keras_aug.datapoints import image as image_utils
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
 from keras_aug.utils.augmentation import H_AXIS
 from keras_aug.utils.augmentation import IMAGES
 from keras_aug.utils.augmentation import W_AXIS
 
 
-@keras.utils.register_keras_serializable(package="keras_cv")
+@keras.utils.register_keras_serializable(package="keras_aug")
 class RandomGridMask(VectorizedBaseRandomLayer):
     """RandomGridMask performs the Grid Mask operation on input images.
 
     Args:
         size_factor (float|Sequence[float]|keras_aug.FactorSampler, optional):
             The relative size for grid masks. When represented as a single
             float, the factor will be picked between ``[0.0, 0.0 + upper]``.
@@ -159,18 +158,18 @@
         # masks (batch_size, height, width, 1)
 
         if self._enable_rotation:
             angles = transformations.get("angles", None)
             heights, widths = augmentation_utils.get_images_shape(
                 images, dtype=tf.float32
             )
-            rotation_matrixes = augmentation_utils.get_rotation_matrix(
+            rotation_matrixes = image_utils.get_rotation_matrix(
                 angles, heights, widths
             )
-            masks = preprocessing_utils.transform(
+            masks = image_utils.transform(
                 tf.cast(masks, dtype=tf.float32),
                 rotation_matrixes,
                 fill_mode="constant",
                 fill_value=0,
                 interpolation="nearest",
             )
         # center crop mask
@@ -231,15 +230,15 @@
         y0 = tf.reshape(y0, [-1])
         x1 = tf.reshape(x1, [-1])
         y1 = tf.reshape(y1, [-1])
         # convert coordinates to mask
         # corners must be tf.float32 for fill_utils.corners_to_mask
         corners = tf.cast(tf.stack([x0, y0, x1, y1], axis=-1), dtype=tf.float32)
         mask_side_len = tf.cast(mask_side_len, dtype=tf.int32)
-        rectangle_masks = fill_utils.corners_to_mask(
+        rectangle_masks = image_utils.corners_to_mask(
             corners, mask_shape=(mask_side_len, mask_side_len)
         )
         grid_mask = tf.reduce_any(rectangle_masks, axis=0)
         return grid_mask
 
     def get_config(self):
         config = super().get_config()
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_grid_mask_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_grid_mask_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/utility/random_apply.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/utility/random_apply.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
-from keras_cv import bounding_box
 from tensorflow import keras
 
+from keras_aug.datapoints import bounding_box
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils.augmentation import BOUNDING_BOXES
 from keras_aug.utils.augmentation import CUSTOM_ANNOTATIONS
 from keras_aug.utils.augmentation import IMAGES
 from keras_aug.utils.augmentation import KEYPOINTS
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/utility/random_apply_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/utility/random_apply_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/utility/random_choice.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/utility/random_choice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from functools import partial
 
 import tensorflow as tf
-from keras_cv import bounding_box
 from tensorflow import keras
 
+from keras_aug.datapoints import bounding_box
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
 from keras_aug.utils.augmentation import BOUNDING_BOXES
 from keras_aug.utils.augmentation import CUSTOM_ANNOTATIONS
 from keras_aug.utils.augmentation import IMAGES
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/utility/random_choice_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/utility/random_choice_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/utility/repeated_augment.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/utility/repeated_augment.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/augmentation/utility/repeated_augment_test.py` & `keras-aug-0.5.6/keras_aug/layers/augmentation/utility/repeated_augment_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/base/vectorized_base_random_layer.py` & `keras-aug-0.5.6/keras_aug/layers/base/vectorized_base_random_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import tensorflow as tf
-from keras_cv import bounding_box
-from keras_cv.utils import preprocessing
 from tensorflow import keras
 
+from keras_aug.datapoints import bounding_box
 from keras_aug.layers.__internal__.base_layer import BaseRandomLayer
+from keras_aug.utils import augmentation as augmentation_utils
 
 H_AXIS = -3
 W_AXIS = -2
 
 IMAGES = "images"
 LABELS = "labels"
 TARGETS = "targets"
@@ -511,28 +511,30 @@
         # preserve any additional inputs unmodified by this layer.
         for key in inputs.keys() - result.keys():
             result[key] = inputs[key]
         return result
 
     def _ensure_inputs_are_compute_dtype(self, inputs):
         if not isinstance(inputs, dict):
-            return preprocessing.ensure_tensor(
+            return augmentation_utils.ensure_tensor(
                 inputs,
                 self.compute_dtype,
             )
-        inputs[IMAGES] = preprocessing.ensure_tensor(
+        inputs[IMAGES] = augmentation_utils.ensure_tensor(
             inputs[IMAGES],
             self.compute_dtype,
         )
         if BOUNDING_BOXES in inputs:
-            inputs[BOUNDING_BOXES]["boxes"] = preprocessing.ensure_tensor(
+            inputs[BOUNDING_BOXES]["boxes"] = augmentation_utils.ensure_tensor(
                 inputs[BOUNDING_BOXES]["boxes"],
                 self.compute_dtype,
             )
-            inputs[BOUNDING_BOXES]["classes"] = preprocessing.ensure_tensor(
+            inputs[BOUNDING_BOXES][
+                "classes"
+            ] = augmentation_utils.ensure_tensor(
                 inputs[BOUNDING_BOXES]["classes"],
                 self.compute_dtype,
             )
         return inputs
 
     def _format_inputs(self, inputs):
         metadata = {IS_DICT: True, USE_TARGETS: False}
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/base/vectorized_base_random_layer_test.py` & `keras-aug-0.5.6/keras_aug/layers/base/vectorized_base_random_layer_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import tensorflow as tf
-from keras_cv import bounding_box
 
+from keras_aug.datapoints import bounding_box
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 
 
 class VectorizedRandomAddLayer(VectorizedBaseRandomLayer):
     def __init__(self, add_range=(0.0, 1.0), fixed_value=None, **kwargs):
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/__init__.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/center_crop.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/center_crop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import tensorflow as tf
-from keras_cv import bounding_box
 from tensorflow import keras
 
+from keras_aug.datapoints import bounding_box
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
-from keras_aug.utils import bounding_box as bounding_box_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
 class CenterCrop(VectorizedBaseRandomLayer):
     """Center crops the images.
 
     CenterCrop crops the central portion of the images to a specified
@@ -20,15 +19,15 @@
     Args:
         height (int): The height of result image.
         width (int): The width of result image.
         padding_value (int|float, optional): The padding value.
             Defaults to ``0``.
         bounding_box_format (str, optional): The format of bounding
             boxes of input dataset. Refer
-            https://github.com/keras-team/keras-cv/blob/master/keras_cv/bounding_box/converters.py
+            https://github.com/james77777778/keras-aug/blob/main/keras_aug/datapoints/bounding_box/converter.py
             for more details on supported bounding box formats.
         bounding_box_min_area_ratio (float, optional): The threshold to
             apply sanitize_bounding_boxes. Defaults to ``None``.
         bounding_box_max_aspect_ratio (float, optional): The threshold to
             apply sanitize_bounding_boxes. Defaults to ``None``.
         seed (int|float, optional): The random seed. Defaults to ``None``.
     """  # noqa: E501
@@ -189,20 +188,20 @@
         y1s += tf.expand_dims(pad_tops - offset_heights, axis=1)
         x2s += tf.expand_dims(pad_lefts - offset_widths, axis=1)
         y2s += tf.expand_dims(pad_tops - offset_heights, axis=1)
         outputs = tf.concat([x1s, y1s, x2s, y2s], axis=-1)
 
         bounding_boxes = bounding_boxes.copy()
         bounding_boxes["boxes"] = outputs
-        bounding_boxes = bounding_box_utils.clip_to_image(
+        bounding_boxes = bounding_box.clip_to_image(
             bounding_boxes,
             bounding_box_format="xyxy",
             images=images,
         )
-        bounding_boxes = bounding_box_utils.sanitize_bounding_boxes(
+        bounding_boxes = bounding_box.sanitize_bounding_boxes(
             bounding_boxes,
             min_area_ratio=self.bounding_box_min_area_ratio,
             max_aspect_ratio=self.bounding_box_max_aspect_ratio,
             bounding_box_format="xyxy",
             reference_bounding_boxes=original_bounding_boxes,
             images=images,
             reference_images=raw_images,
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/center_crop_test.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/center_crop_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import tensorflow as tf
-from keras_cv import bounding_box
 
 from keras_aug import layers
+from keras_aug.datapoints import bounding_box
 
 
 class CenterCropTest(tf.test.TestCase):
     height, width = 224, 224
     regular_args = {
         "height": 112,
         "width": 112,
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/pad_if_needed.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/pad_if_needed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
-from keras_cv import bounding_box
 from tensorflow import keras
 
+from keras_aug.datapoints import bounding_box
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
@@ -29,15 +29,15 @@
         position (str, optional): The padding method.
             Supported values: ``"center", "top_left", "top_right", "bottom_left", "bottom_right", "random"``.
             Defaults to ``"center"``.
         padding_value (int|float, optional): The padding value.
             Defaults to ``0``.
         bounding_box_format (str, optional): The format of bounding
             boxes of input dataset. Refer
-            https://github.com/keras-team/keras-cv/blob/master/keras_cv/bounding_box/converters.py
+            https://github.com/james77777778/keras-aug/blob/main/keras_aug/datapoints/bounding_box/converter.py
             for more details on supported bounding box formats.
         seed (int|float, optional): The random seed. Defaults to ``None``.
 
     References:
         - `Albumentations <https://github.com/albumentations-team/albumentations>`_
     """  # noqa: E501
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/pad_if_needed_test.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/pad_if_needed_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import tensorflow as tf
 from absl.testing import parameterized
-from keras_cv import bounding_box
 
 from keras_aug import layers
+from keras_aug.datapoints import bounding_box
 
 
 class PadIfNeededTest(tf.test.TestCase, parameterized.TestCase):
     height, width = 32, 32
     regular_args = {
         "min_height": 32,
         "min_width": 32,
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/resize.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/resize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import tensorflow as tf
-from keras_cv import bounding_box
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
+from keras_aug.datapoints import bounding_box
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 from keras_aug.utils import augmentation as augmentation_utils
-from keras_aug.utils import bounding_box as bounding_box_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
 class Resize(VectorizedBaseRandomLayer):
     """Resizes the images.
 
     Resize will resize the images to ``(height, width)``. Set
@@ -39,15 +37,15 @@
         position (str, optional): The padding method.
             Supported values: ``"center", "top_left", "top_right", "bottom_left", "bottom_right", "random"``.
             Defaults to ``"center"``.
         padding_value (int|float, optional): The padding value.
             Defaults to ``0``.
         bounding_box_format (str, optional): The format of bounding
             boxes of input dataset. Refer
-            https://github.com/keras-team/keras-cv/blob/master/keras_cv/bounding_box/converters.py
+            https://github.com/james77777778/keras-aug/blob/main/keras_aug/datapoints/bounding_box/converter.py
             for more details on supported bounding box formats.
         seed (int|float, optional): The random seed. Defaults to ``None``.
 
     References:
         - `KerasCV <https://github.com/keras-team/keras-cv>`_
     """  # noqa: E501
 
@@ -69,17 +67,15 @@
         if not isinstance(height, int) or not isinstance(width, int):
             raise ValueError(
                 "`height` and `width` must be integer. Received: "
                 f"`height`={height} `width`={width} "
             )
         self.height = height
         self.width = width
-        self.interpolation = preprocessing_utils.get_interpolation(
-            interpolation
-        )
+        self.interpolation = augmentation_utils.get_interpolation(interpolation)
         self.antialias = antialias
         self.position = augmentation_utils.get_padding_position(position)
         self.padding_value = padding_value
         if crop_to_aspect_ratio is True and pad_to_aspect_ratio is True:
             raise ValueError(
                 "Resize expects at most one of ``crop_to_aspect_ratio`` or "
                 "``pad_to_aspect_ratio`` to be ``True``"
@@ -269,15 +265,15 @@
             x1s = x1s * widths_ratios + lefts
             x2s = x2s * widths_ratios + lefts
             y1s = y1s * height_ratios + tops
             y2s = y2s * height_ratios + tops
         boxes = tf.concat([x1s, y1s, x2s, y2s], axis=-1)
         bounding_boxes = bounding_boxes.copy()
         bounding_boxes["boxes"] = boxes
-        bounding_boxes = bounding_box_utils.clip_to_image(
+        bounding_boxes = bounding_box.clip_to_image(
             bounding_boxes,
             bounding_box_format="xyxy",
             images=images,
         )
         bounding_boxes = bounding_box.convert_format(
             bounding_boxes,
             source="xyxy",
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/resize_test.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/resize_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import tensorflow as tf
 from absl.testing import parameterized
-from keras_cv import bounding_box
 
 from keras_aug import layers
+from keras_aug.datapoints import bounding_box
 
 
 class ResizeTest(tf.test.TestCase, parameterized.TestCase):
     height, width = 224, 224
     regular_args = {
         "height": 224,
         "width": 224,
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/auto_contrast.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/auto_contrast.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
+from keras_aug.datapoints import image as image_utils
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
 class AutoContrast(VectorizedBaseRandomLayer):
@@ -33,28 +33,28 @@
         images = tf.expand_dims(image, axis=0)
         images = self.augment_images(
             images=images, transformations=transformation, **kwargs
         )
         return tf.squeeze(images, axis=0)
 
     def augment_images(self, images, transformations, **kwargs):
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images,
             original_range=self.value_range,
             target_range=(0, 255),
             dtype=self.compute_dtype,
         )
         lows = tf.reduce_min(images, axis=(1, 2), keepdims=True)
         highs = tf.reduce_max(images, axis=(1, 2), keepdims=True)
         scales = 255.0 / (highs - lows)
         eq_idxs = tf.math.is_inf(scales)
         lows = tf.where(eq_idxs, 0.0, lows)
         scales = tf.where(eq_idxs, 1.0, scales)
         images = tf.clip_by_value((images - lows) * scales, 0, 255)
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images,
             original_range=(0, 255),
             target_range=self.value_range,
             dtype=self.compute_dtype,
         )
         return images
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/auto_contrast_test.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/auto_contrast_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/equalize.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/equalize.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
-from keras_cv.utils import preprocessing as preprocessing_utils
 from tensorflow import keras
 
+from keras_aug.datapoints import image as image_utils
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
 class Equalize(VectorizedBaseRandomLayer):
@@ -33,25 +33,25 @@
         image = self.augment_images(
             images=image, transformations=transformation, **kwargs
         )
         return tf.squeeze(image, axis=0)
 
     def augment_images(self, images, transformations=None, **kwargs):
         original_shape = images.shape
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images, self.value_range, (0, 255), dtype=self.compute_dtype
         )
         images = tf.cast(images, dtype=tf.int32)
         images = tf.map_fn(
             self.equalize_single_image,
             images,
         )
         images = tf.transpose(images, (0, 2, 3, 1))
         images = tf.cast(images, dtype=self.compute_dtype)
-        images = preprocessing_utils.transform_value_range(
+        images = image_utils.transform_value_range(
             images, (0, 255), self.value_range, dtype=self.compute_dtype
         )
         images.set_shape(original_shape)
         return tf.cast(images, dtype=self.compute_dtype)
 
     def augment_labels(self, labels, transformations, **kwargs):
         return labels
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/equalize_test.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/equalize_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/grayscale.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/grayscale.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_aug.datapoints import image as image_utils
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
-from keras_aug.utils import augmentation as augmentation_utils
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
 class Grayscale(VectorizedBaseRandomLayer):
     """Grayscale transforms RGB images to grayscale images.
 
     Args:
@@ -38,15 +38,15 @@
 
     def augment_ragged_image(self, image, transformation, **kwargs):
         return self.augment_images(
             image, transformations=transformation, **kwargs
         )
 
     def augment_images(self, images, transformations=None, **kwargs):
-        grayscales = augmentation_utils.rgb_to_grayscale(images)
+        grayscales = image_utils.rgb_to_grayscale(images)
         if self.output_channels == 1:
             return grayscales
         elif self.output_channels == 3:
             return tf.image.grayscale_to_rgb(grayscales)
         else:
             raise ValueError("Unsupported value for `output_channels`.")
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/grayscale_test.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/grayscale_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/identity.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/identity.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/identity_test.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/identity_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/invert.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/invert.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/normalize.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/normalize.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/normalize_test.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/normalize_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/rescale.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/rescale.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/rescale_test.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/rescale_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/utility/sanitize_bounding_box.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/utility/sanitize_bounding_box.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-from keras_cv import bounding_box
 from tensorflow import keras
 
+from keras_aug.datapoints import bounding_box
 from keras_aug.layers.base.vectorized_base_random_layer import (
     VectorizedBaseRandomLayer,
 )
-from keras_aug.utils import bounding_box as bounding_box_utils
 from keras_aug.utils.augmentation import BOUNDING_BOXES
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
 class SanitizeBoundingBox(VectorizedBaseRandomLayer):
     """Remove degenerate/invalid bounding boxes.
 
     Args:
         min_size (int): The minimum size of the smaller side of bounding boxes.
         bounding_box_format (str): The format of bounding boxes of input
             dataset. Refer
-            https://github.com/keras-team/keras-cv/blob/master/keras_cv/bounding_box/converters.py
+            https://github.com/james77777778/keras-aug/blob/main/keras_aug/datapoints/bounding_box/converter.py
             for more details on supported bounding box formats.
 
     References:
         - `torchvision <https://github.com/pytorch/vision>`_
     """
 
     def __init__(self, min_size, bounding_box_format=None, **kwargs):
@@ -44,15 +43,15 @@
             raise ValueError(
                 "`SanitizeBoundingBox()` was called with bounding boxes,"
                 "but no `bounding_box_format` was specified in the constructor."
                 "Please specify a bounding box format in the constructor. i.e."
                 "`SanitizeBoundingBox(..., bounding_box_format='xyxy')`"
             )
         bounding_boxes = bounding_box.to_dense(bounding_boxes)
-        bounding_boxes = bounding_box_utils.sanitize_bounding_boxes(
+        bounding_boxes = bounding_box.sanitize_bounding_boxes(
             bounding_boxes,
             min_size=self.min_size,
             bounding_box_format=self.bounding_box_format,
             images=images,
         )
         return bounding_boxes
```

### Comparing `keras-aug-0.5.5/keras_aug/layers/preprocessing/utility/sanitize_bounding_box_test.py` & `keras-aug-0.5.6/keras_aug/layers/preprocessing/utility/sanitize_bounding_box_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug/utils/augmentation_test.py` & `keras-aug-0.5.6/keras_aug/utils/augmentation_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -214,17 +214,7 @@
             ),
             augmentation_utils.KEYPOINTS: tf.random.uniform((2, 4, 17)),
         }
 
         signatures = augmentation_utils.compute_signature(inputs, tf.float16)
 
         self.assertTrue(inputs.keys() == signatures.keys())
-
-    def test_blend(self):
-        ones = tf.ones(shape=(2, 4, 4, 3))
-        twos = tf.ones(shape=(2, 4, 4, 3)) * 2
-        ratios = tf.ones(shape=(2, 1, 1, 1)) * 0.3
-        expected_result = ratios * ones + (1.0 - ratios) * twos
-
-        result = augmentation_utils.blend(twos, ones, ratios)
-
-        self.assertAllEqual(result, expected_result)
```

### Comparing `keras-aug-0.5.5/keras_aug/utils/bounding_box_test.py` & `keras-aug-0.5.6/keras_aug/datapoints/bounding_box/utils_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import tensorflow as tf
 
-from keras_aug.utils import bounding_box as bounding_box_utils
+from keras_aug.datapoints import bounding_box as bounding_box_utils
 
 
 class BoundingBoxUtilsTest(tf.test.TestCase):
     def test_sanitize_bounding_boxes_intact(self):
         bounding_boxes = {
             "boxes": tf.convert_to_tensor(
                 [[[10, 10, 20, 20], [10, 10, 30, 30]]], dtype=tf.float32
```

### Comparing `keras-aug-0.5.5/keras_aug/utils/demo.py` & `keras-aug-0.5.6/keras_aug/utils/demo.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,21 @@
-import keras_cv
 import tensorflow as tf
 
 try:
     import tensorflow_datasets as tfds
 except ImportError:
     tfds = None
+try:
+    import keras_cv
+except ImportError:
+    keras_cv = None
 
+from keras_aug.datapoints import bounding_box
+from keras_aug.datapoints import image as image_utils
+from keras_aug.utils.conditional_imports import assert_kerascv_installed
 from keras_aug.utils.conditional_imports import assert_tfds_installed
 
 
 def load_voc_dataset(
     bounding_box_format,
     name="voc/2007",
     batch_size=9,
@@ -17,15 +23,15 @@
     assert_tfds_installed("load_voc_dataset")
 
     def preprocess_voc(inputs, format=None):
         image = inputs["image"]
         image = tf.cast(image, tf.float32)
         if format is not None:
             boxes = inputs["objects"]["bbox"]
-            boxes = keras_cv.bounding_box.convert_format(
+            boxes = bounding_box.convert_format(
                 boxes,
                 images=image,
                 source="rel_yxyx",
                 target=format,
             )
             classes = tf.cast(inputs["objects"]["label"], tf.float32)
             bounding_boxes = {"classes": classes, "boxes": boxes}
@@ -107,14 +113,16 @@
     dataset = dataset.batch(batch_size)
     return dataset
 
 
 def visualize_data(
     data, value_range=(0, 255), bounding_box_format=None, output_path=None
 ):
+    assert_kerascv_installed("visualize_data")
+
     data = next(iter(data))
     images = data["images"]
     if isinstance(images, tf.RaggedTensor):
         images = images.to_tensor(0)
     if "labels" in data:
         mask = tf.greater(data["labels"][0], 0)
         non_zero_array = tf.boolean_mask(data["labels"][0], mask)
@@ -137,14 +145,16 @@
             dpi=100,
         )
 
 
 def visualize_data_single(
     data, value_range=(0, 255), bounding_box_format=None, output_path=None
 ):
+    assert_kerascv_installed("visualize_data")
+
     data = next(iter(data))
     images = data["images"]
     images = images[0:1, ...]
     if isinstance(images, tf.RaggedTensor):
         images = images.to_tensor(0)
     if "labels" in data:
         mask = tf.greater(data["labels"][0], 0)
@@ -180,20 +190,20 @@
 
 def visualize_segmentation_masks(
     data,
     image_value_range=(0, 255),
     mask_value_range=None,
     output_path=None,
 ):
+    assert_kerascv_installed("visualize_data")
+
     data = next(iter(data))
     images = data["images"]
     masks = data["segmentation_masks"]
-    masks = keras_cv.utils.transform_value_range(
-        masks, mask_value_range, (0, 255)
-    )
+    masks = image_utils.transform_value_range(masks, mask_value_range, (0, 255))
     masks = tf.concat([masks, masks, masks], axis=-1)
     display_images = tf.concat([images, masks], axis=2)  # B, H, W, C
 
     keras_cv.visualization.plot_image_gallery(
         display_images,
         value_range=image_value_range,
         path=output_path,
```

### Comparing `keras-aug-0.5.5/keras_aug/utils/distribution.py` & `keras-aug-0.5.6/keras_aug/utils/distribution.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.5/keras_aug.egg-info/PKG-INFO` & `keras-aug-0.5.6/keras_aug.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-aug
-Version: 0.5.5
+Version: 0.5.6
 Summary: A library that includes pure TF/Keras preprocessing and augmentation layers
 Author: Hongyu, Chiu (james77777778)
 License:    Copyright 2023 The KerasAug Authors. All rights reserved.
         
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -207,15 +207,15 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: homepage, https://github.com/james77777778/keras-aug
 Project-URL: repository, https://github.com/james77777778/keras-aug
 Project-URL: documentation, https://kerasaug.readthedocs.io/en/latest/
-Keywords: tensorflow,keras,keras-cv,preprocessing,augmentation
+Keywords: tensorflow,keras,preprocessing,augmentation
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -233,15 +233,14 @@
 License-File: LICENSE
 
 <!-- markdownlint-disable MD033 -->
 # KerasAug
 
 ![Python](https://img.shields.io/badge/python-v3.8.0+-success.svg)
 ![Tensorflow](https://img.shields.io/badge/tensorflow-v2.12.0+-success.svg)
-![KerasCV](https://img.shields.io/badge/keras_cv-v0.5.0+-success.svg)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/james77777778/keras-aug/actions.yml?label=tests)](https://github.com/james77777778/keras-aug/actions/workflows/actions.yml?query=branch%3Amain++)
 [![codecov](https://codecov.io/gh/james77777778/keras-aug/branch/main/graph/badge.svg?token=81ELI3VH7H)](https://codecov.io/gh/james77777778/keras-aug)
 [![PyPI](https://img.shields.io/pypi/v/keras-aug)](https://pypi.org/project/keras-aug/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/keras-aug)
 [![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/james77777778/keras-aug/issues)
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://james77777778-keras-aug-streamlit-appapp-mxd7v1.streamlit.app/)
 
@@ -297,20 +296,17 @@
 
     > **Note**
     > The degenerate bounding boxes (those located at the bottom of the image) are removed.
 
 ## Installation
 
 ```bash
-pip install keras-aug keras-cv tensorflow --upgrade
+pip install keras-aug tensorflow --upgrade
 ```
 
-> **Warning**
-> KerasAug is NOT compatible with `keras-cv < 0.5.0`.
-
 ## Quickstart
 
 <details>
 <summary>Rock, Paper and Scissors Image Classification</summary>
 
 ```python
 import keras_aug
@@ -433,15 +429,15 @@
         path=path,
         dpi=150,
     )
 
 
 def unpackage_raw_tfds_inputs(inputs, bounding_box_format):
     image = inputs["image"]
-    boxes = keras_cv.bounding_box.convert_format(
+    boxes = keras_aug.datapoints.bounding_box.convert_format(
         inputs["objects"]["bbox"],
         images=image,
         source="rel_yxyx",
         target=bounding_box_format,
     )
     bounding_boxes = {
         "classes": tf.cast(inputs["objects"]["label"], dtype=tf.float32),
```

### Comparing `keras-aug-0.5.5/keras_aug.egg-info/SOURCES.txt` & `keras-aug-0.5.6/keras_aug.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,34 @@
 keras_aug/core/factor_sampler/normal_factor_sampler_test.py
 keras_aug/core/factor_sampler/signed_constant_factor_sampler.py
 keras_aug/core/factor_sampler/signed_constant_factor_sampler_test.py
 keras_aug/core/factor_sampler/signed_normal_factor_sampler.py
 keras_aug/core/factor_sampler/signed_normal_factor_sampler_test.py
 keras_aug/core/factor_sampler/uniform_factor_sampler.py
 keras_aug/core/factor_sampler/uniform_factor_sampler_test.py
+keras_aug/datapoints/__init__.py
+keras_aug/datapoints/bounding_box/__init__.py
+keras_aug/datapoints/bounding_box/converter.py
+keras_aug/datapoints/bounding_box/converter_test.py
+keras_aug/datapoints/bounding_box/iou.py
+keras_aug/datapoints/bounding_box/iou_test.py
+keras_aug/datapoints/bounding_box/to_dense.py
+keras_aug/datapoints/bounding_box/to_dense_test.py
+keras_aug/datapoints/bounding_box/to_ragged.py
+keras_aug/datapoints/bounding_box/to_ragged_test.py
+keras_aug/datapoints/bounding_box/utils.py
+keras_aug/datapoints/bounding_box/utils_test.py
+keras_aug/datapoints/bounding_box/validate_format.py
+keras_aug/datapoints/bounding_box/validate_format_test.py
+keras_aug/datapoints/image/__init__.py
+keras_aug/datapoints/image/fill.py
+keras_aug/datapoints/image/get_matrix.py
+keras_aug/datapoints/image/get_matrix_test.py
+keras_aug/datapoints/image/ops.py
+keras_aug/datapoints/image/ops_test.py
 keras_aug/layers/__init__.py
 keras_aug/layers/__internal__/__init__.py
 keras_aug/layers/__internal__/base_layer.py
 keras_aug/layers/__internal__/base_layer_test.py
 keras_aug/layers/__internal__/config_test.py
 keras_aug/layers/__internal__/graph_xla_mode_test.py
 keras_aug/layers/__internal__/mixed_precision_test.py
@@ -130,12 +150,10 @@
 keras_aug/layers/preprocessing/intensity/rescale_test.py
 keras_aug/layers/preprocessing/utility/__init__.py
 keras_aug/layers/preprocessing/utility/sanitize_bounding_box.py
 keras_aug/layers/preprocessing/utility/sanitize_bounding_box_test.py
 keras_aug/utils/__init__.py
 keras_aug/utils/augmentation.py
 keras_aug/utils/augmentation_test.py
-keras_aug/utils/bounding_box.py
-keras_aug/utils/bounding_box_test.py
 keras_aug/utils/conditional_imports.py
 keras_aug/utils/demo.py
 keras_aug/utils/distribution.py
```

### Comparing `keras-aug-0.5.5/pyproject.toml` & `keras-aug-0.5.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "keras-aug"
 authors = [{ name = "Hongyu, Chiu (james77777778)" }]
 description = "A library that includes pure TF/Keras preprocessing and augmentation layers"
-keywords = ["tensorflow", "keras", "keras-cv", "preprocessing", "augmentation"]
+keywords = ["tensorflow", "keras", "preprocessing", "augmentation"]
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -23,15 +23,15 @@
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development",
 ]
 dynamic = ["version"]
-dependencies = ["pycocotools", "tensorflow", "keras-cv"]
+dependencies = ["pycocotools", "tensorflow"]
 
 [project.optional-dependencies]
 tests = [
     "ruff",
     "black[jupyter]",
     "pytest",
     "pytest-cov",
```

