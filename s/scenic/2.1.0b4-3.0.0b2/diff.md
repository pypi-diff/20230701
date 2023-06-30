# Comparing `tmp/scenic-2.1.0b4.tar.gz` & `tmp/scenic-3.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scenic-2.1.0b4.tar", max compression
+gzip compressed data, was "scenic-3.0.0b2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `scenic-2.1.0b4.tar` & `scenic-3.0.0b2.tar`

### file list

```diff
@@ -1,101 +1,115 @@
--rw-r--r--   0        0        0     1622 2019-02-12 18:33:34.000000 scenic-2.1.0b4/LICENSE
--rw-r--r--   0        0        0     1658 2022-04-24 16:36:45.885697 scenic-2.1.0b4/README.md
--rw-r--r--   0        0        0     2093 2022-07-09 23:56:11.148992 scenic-2.1.0b4/pyproject.toml
--rw-r--r--   0        0        0      366 2022-04-24 16:33:57.790325 scenic-2.1.0b4/src/scenic/__init__.py
--rw-r--r--   0        0        0     9259 2022-07-08 21:40:44.209853 scenic-2.1.0b4/src/scenic/__main__.py
--rw-r--r--   0        0        0      373 2022-04-24 16:36:45.929919 scenic-2.1.0b4/src/scenic/core/__init__.py
--rw-r--r--   0        0        0    36192 2022-07-16 19:21:11.005420 scenic-2.1.0b4/src/scenic/core/distributions.py
--rw-r--r--   0        0        0    29833 2022-07-09 23:25:21.999399 scenic-2.1.0b4/src/scenic/core/dynamics.py
--rw-r--r--   0        0        0     9816 2022-07-10 05:06:48.708826 scenic-2.1.0b4/src/scenic/core/errors.py
--rw-r--r--   0        0        0    13400 2022-07-10 03:34:32.523487 scenic-2.1.0b4/src/scenic/core/external_params.py
--rw-r--r--   0        0        0    12856 2022-07-08 21:40:44.212554 scenic-2.1.0b4/src/scenic/core/geometry.py
--rw-r--r--   0        0        0     6796 2022-04-24 16:36:45.962569 scenic-2.1.0b4/src/scenic/core/lazy_eval.py
--rw-r--r--   0        0        0    20228 2022-07-18 16:35:29.980016 scenic-2.1.0b4/src/scenic/core/object_types.py
--rw-r--r--   0        0        0    12414 2022-04-24 16:36:45.963963 scenic-2.1.0b4/src/scenic/core/pruning.py
--rw-r--r--   0        0        0    39541 2022-07-08 21:40:44.213967 scenic-2.1.0b4/src/scenic/core/regions.py
--rw-r--r--   0        0        0     6164 2022-04-24 16:36:45.965391 scenic-2.1.0b4/src/scenic/core/requirements.py
--rw-r--r--   0        0        0    13833 2022-07-09 23:31:00.854589 scenic-2.1.0b4/src/scenic/core/scenarios.py
--rw-r--r--   0        0        0      404 2022-04-24 16:36:45.966373 scenic-2.1.0b4/src/scenic/core/serialization.py
--rw-r--r--   0        0        0    19682 2022-07-09 23:32:03.104973 scenic-2.1.0b4/src/scenic/core/simulators.py
--rw-r--r--   0        0        0     2601 2022-04-24 16:36:45.967557 scenic-2.1.0b4/src/scenic/core/specifiers.py
--rw-r--r--   0        0        0    12608 2022-04-24 16:36:45.968141 scenic-2.1.0b4/src/scenic/core/type_support.py
--rw-r--r--   0        0        0     5016 2022-04-24 16:36:45.968689 scenic-2.1.0b4/src/scenic/core/utils.py
--rw-r--r--   0        0        0    14062 2022-07-08 21:40:44.216168 scenic-2.1.0b4/src/scenic/core/vectors.py
--rw-r--r--   0        0        0     2649 2022-07-09 23:25:22.000743 scenic-2.1.0b4/src/scenic/core/workspaces.py
--rw-r--r--   0        0        0      138 2022-04-24 16:33:57.796326 scenic-2.1.0b4/src/scenic/domains/__init__.py
--rw-r--r--   0        0        0     2310 2022-07-18 16:35:30.002456 scenic-2.1.0b4/src/scenic/domains/driving/__init__.py
--rw-r--r--   0        0        0     5733 2022-04-26 19:07:13.823332 scenic-2.1.0b4/src/scenic/domains/driving/actions.py
--rw-r--r--   0        0        0    13057 2022-07-08 21:40:44.217189 scenic-2.1.0b4/src/scenic/domains/driving/behaviors.scenic
--rw-r--r--   0        0        0     2584 2022-04-24 16:36:45.970921 scenic-2.1.0b4/src/scenic/domains/driving/controllers.py
--rw-r--r--   0        0        0    13822 2022-07-08 21:40:44.217797 scenic-2.1.0b4/src/scenic/domains/driving/model.scenic
--rw-r--r--   0        0        0    47867 2022-04-24 16:36:45.972235 scenic-2.1.0b4/src/scenic/domains/driving/roads.py
--rw-r--r--   0        0        0     2976 2022-07-08 21:40:44.218060 scenic-2.1.0b4/src/scenic/domains/driving/simulators.py
--rw-r--r--   0        0        0      383 2022-04-24 16:33:57.798077 scenic-2.1.0b4/src/scenic/domains/driving/workspace.py
--rw-r--r--   0        0        0      155 2022-04-24 16:33:57.798207 scenic-2.1.0b4/src/scenic/formats/__init__.py
--rw-r--r--   0        0        0      227 2022-04-24 16:36:45.972794 scenic-2.1.0b4/src/scenic/formats/opendrive/__init__.py
--rw-r--r--   0        0        0     1980 2022-04-24 16:33:57.798461 scenic-2.1.0b4/src/scenic/formats/opendrive/workspace.py
--rw-r--r--   0        0        0    81055 2022-04-24 16:36:45.973972 scenic-2.1.0b4/src/scenic/formats/opendrive/xodr_parser.py
--rw-r--r--   0        0        0      200 2022-04-24 16:36:45.975486 scenic-2.1.0b4/src/scenic/simulators/__init__.py
--rw-r--r--   0        0        0      886 2022-04-24 16:36:45.976086 scenic-2.1.0b4/src/scenic/simulators/carla/__init__.py
--rw-r--r--   0        0        0     7156 2022-07-08 21:40:44.218601 scenic-2.1.0b4/src/scenic/simulators/carla/actions.py
--rw-r--r--   0        0        0     2454 2022-04-24 16:36:45.977244 scenic-2.1.0b4/src/scenic/simulators/carla/behaviors.scenic
--rw-r--r--   0        0        0     5292 2022-07-08 21:40:44.219255 scenic-2.1.0b4/src/scenic/simulators/carla/blueprints.scenic
--rw-r--r--   0        0        0     5846 2022-04-24 16:33:57.799989 scenic-2.1.0b4/src/scenic/simulators/carla/misc.py
--rw-r--r--   0        0        0    12705 2022-07-08 21:40:44.220040 scenic-2.1.0b4/src/scenic/simulators/carla/model.scenic
--rw-r--r--   0        0        0     9416 2022-07-09 23:25:22.001084 scenic-2.1.0b4/src/scenic/simulators/carla/simulator.py
--rw-r--r--   0        0        0     1924 2022-04-24 16:33:57.800516 scenic-2.1.0b4/src/scenic/simulators/carla/utils/utils.py
--rw-r--r--   0        0        0    12797 2022-04-24 16:33:57.800671 scenic-2.1.0b4/src/scenic/simulators/carla/utils/visuals.py
--rw-r--r--   0        0        0      201 2022-04-24 16:33:57.800841 scenic-2.1.0b4/src/scenic/simulators/gta/__init__.py
--rw-r--r--   0        0        0    10603 2022-07-10 17:05:35.882932 scenic-2.1.0b4/src/scenic/simulators/gta/center_detection.py
--rw-r--r--   0        0        0     3676 2019-01-18 03:51:30.000000 scenic-2.1.0b4/src/scenic/simulators/gta/img_modf.py
--rw-r--r--   0        0        0     7902 2022-07-16 19:08:11.787725 scenic-2.1.0b4/src/scenic/simulators/gta/interface.py
--rw-r--r--   0        0        0      234 2019-01-18 03:51:30.000000 scenic-2.1.0b4/src/scenic/simulators/gta/map.py
--rw-r--r--   0        0        0     3835 2019-01-18 03:51:30.000000 scenic-2.1.0b4/src/scenic/simulators/gta/messages.py
--rw-r--r--   0        0        0     2682 2022-04-24 16:33:57.801264 scenic-2.1.0b4/src/scenic/simulators/gta/model.scenic
--rw-r--r--   0        0        0      745 2022-04-24 16:36:45.979393 scenic-2.1.0b4/src/scenic/simulators/lgsvl/__init__.py
--rw-r--r--   0        0        0     4288 2022-04-24 16:36:45.979800 scenic-2.1.0b4/src/scenic/simulators/lgsvl/actions.py
--rw-r--r--   0        0        0      573 2022-04-24 16:36:45.980239 scenic-2.1.0b4/src/scenic/simulators/lgsvl/behaviors.scenic
--rw-r--r--   0        0        0     4011 2022-07-08 21:40:44.221024 scenic-2.1.0b4/src/scenic/simulators/lgsvl/model.scenic
--rw-r--r--   0        0        0     6014 2022-04-24 16:36:45.981209 scenic-2.1.0b4/src/scenic/simulators/lgsvl/simulator.py
--rw-r--r--   0        0        0      973 2022-04-24 16:36:45.981581 scenic-2.1.0b4/src/scenic/simulators/lgsvl/utils.py
--rw-r--r--   0        0        0      528 2022-07-18 16:35:30.002784 scenic-2.1.0b4/src/scenic/simulators/newtonian/__init__.py
--rw-r--r--   0        0        0       44 2022-04-24 16:36:45.982132 scenic-2.1.0b4/src/scenic/simulators/newtonian/actions.py
--rw-r--r--   0        0        0       79 2022-04-24 16:36:45.982552 scenic-2.1.0b4/src/scenic/simulators/newtonian/behaviors.scenic
--rw-r--r--   0        0        0    73799 2022-04-24 16:36:45.983622 scenic-2.1.0b4/src/scenic/simulators/newtonian/car.png
--rw-r--r--   0        0        0     1691 2022-07-18 16:35:30.002987 scenic-2.1.0b4/src/scenic/simulators/newtonian/driving_model.scenic
--rw-r--r--   0        0        0      454 2022-07-18 16:35:30.003236 scenic-2.1.0b4/src/scenic/simulators/newtonian/model.scenic
--rw-r--r--   0        0        0    10012 2022-07-08 21:40:44.222567 scenic-2.1.0b4/src/scenic/simulators/newtonian/simulator.py
--rw-r--r--   0        0        0      390 2022-04-24 16:36:45.984979 scenic-2.1.0b4/src/scenic/simulators/newtonian/utils/utils.py
--rw-r--r--   0        0        0      141 2022-04-24 16:33:57.803684 scenic-2.1.0b4/src/scenic/simulators/utils/__init__.py
--rw-r--r--   0        0        0     3643 2022-07-08 21:40:44.223097 scenic-2.1.0b4/src/scenic/simulators/utils/colors.py
--rw-r--r--   0        0        0     1609 2022-04-24 16:33:57.804475 scenic-2.1.0b4/src/scenic/simulators/webots/WBT.g4
--rw-r--r--   0        0        0     5657 2022-04-24 16:33:57.805105 scenic-2.1.0b4/src/scenic/simulators/webots/WBTLexer.py
--rw-r--r--   0        0        0    26889 2022-04-24 16:33:57.805897 scenic-2.1.0b4/src/scenic/simulators/webots/WBTParser.py
--rw-r--r--   0        0        0     2028 2022-04-24 16:33:57.806485 scenic-2.1.0b4/src/scenic/simulators/webots/WBTVisitor.py
--rw-r--r--   0        0        0      566 2022-04-24 16:36:45.985970 scenic-2.1.0b4/src/scenic/simulators/webots/__init__.py
--rw-r--r--   0        0        0     1462 2022-04-24 16:36:45.986314 scenic-2.1.0b4/src/scenic/simulators/webots/actions.py
--rw-r--r--   0        0        0      368 2021-08-12 22:11:42.443022 scenic-2.1.0b4/src/scenic/simulators/webots/controllers.py
--rw-r--r--   0        0        0      401 2022-04-24 16:33:57.807003 scenic-2.1.0b4/src/scenic/simulators/webots/guideways/__init__.py
--rw-r--r--   0        0        0     5196 2022-04-24 16:33:57.807447 scenic-2.1.0b4/src/scenic/simulators/webots/guideways/interface.py
--rw-r--r--   0        0        0      311 2022-04-24 16:33:57.807623 scenic-2.1.0b4/src/scenic/simulators/webots/guideways/intersection.py
--rw-r--r--   0        0        0     1209 2022-04-24 16:33:57.807747 scenic-2.1.0b4/src/scenic/simulators/webots/guideways/model.scenic
--rw-r--r--   0        0        0      143 2022-04-24 16:33:57.807903 scenic-2.1.0b4/src/scenic/simulators/webots/mars/__init__.py
--rw-r--r--   0        0        0     1235 2022-04-24 16:36:45.986850 scenic-2.1.0b4/src/scenic/simulators/webots/mars/model.scenic
--rw-r--r--   0        0        0     7920 2022-07-08 21:40:44.223992 scenic-2.1.0b4/src/scenic/simulators/webots/model.scenic
--rw-r--r--   0        0        0      295 2022-04-24 16:33:57.808437 scenic-2.1.0b4/src/scenic/simulators/webots/road/__init__.py
--rw-r--r--   0        0        0      661 2022-07-16 18:51:09.650912 scenic-2.1.0b4/src/scenic/simulators/webots/road/car_models.py
--rw-r--r--   0        0        0    13160 2022-04-24 16:36:45.988720 scenic-2.1.0b4/src/scenic/simulators/webots/road/interface.py
--rw-r--r--   0        0        0     2799 2022-04-24 16:33:57.809189 scenic-2.1.0b4/src/scenic/simulators/webots/road/model.scenic
--rw-r--r--   0        0        0      439 2022-04-24 16:33:57.809737 scenic-2.1.0b4/src/scenic/simulators/webots/road/world.py
--rw-r--r--   0        0        0     7318 2022-07-08 21:40:44.224632 scenic-2.1.0b4/src/scenic/simulators/webots/simulator.py
--rw-r--r--   0        0        0     4104 2022-04-24 16:36:45.990222 scenic-2.1.0b4/src/scenic/simulators/webots/utils.py
--rw-r--r--   0        0        0     3069 2022-04-24 16:33:57.810747 scenic-2.1.0b4/src/scenic/simulators/webots/world_parser.py
--rw-r--r--   0        0        0      295 2022-04-24 16:33:57.812410 scenic-2.1.0b4/src/scenic/simulators/xplane/__init__.py
--rw-r--r--   0        0        0      262 2022-04-24 16:33:57.813980 scenic-2.1.0b4/src/scenic/simulators/xplane/model.scenic
--rw-r--r--   0        0        0      165 2022-04-24 16:33:57.815847 scenic-2.1.0b4/src/scenic/syntax/__init__.py
--rw-r--r--   0        0        0      267 2022-04-24 16:33:57.816790 scenic-2.1.0b4/src/scenic/syntax/pygment.py
--rw-r--r--   0        0        0     8756 2022-04-24 16:33:57.819070 scenic-2.1.0b4/src/scenic/syntax/relations.py
--rw-r--r--   0        0        0    84583 2022-07-10 15:03:46.763904 scenic-2.1.0b4/src/scenic/syntax/translator.py
--rw-r--r--   0        0        0    37548 2022-07-09 23:25:22.002850 scenic-2.1.0b4/src/scenic/syntax/veneer.py
--rw-r--r--   0        0        0     4258 2022-07-19 17:52:00.259221 scenic-2.1.0b4/setup.py
--rw-r--r--   0        0        0     3961 2022-07-19 17:52:00.259606 scenic-2.1.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1622 2019-02-12 18:33:34.000000 scenic-3.0.0b2/LICENSE
+-rw-r--r--   0        0        0     1844 2023-05-09 15:10:50.278771 scenic-3.0.0b2/README.md
+-rw-r--r--   0        0        0     2735 2023-06-30 22:49:11.376668 scenic-3.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0    10244 2023-02-12 21:53:28.063140 scenic-3.0.0b2/src/scenic/.DS_Store
+-rw-r--r--   0        0        0      329 2023-06-30 22:40:23.467525 scenic-3.0.0b2/src/scenic/__init__.py
+-rw-r--r--   0        0        0    10383 2023-06-30 22:40:23.468246 scenic-3.0.0b2/src/scenic/__main__.py
+-rw-r--r--   0        0        0     6148 2023-04-20 16:43:54.709970 scenic-3.0.0b2/src/scenic/core/.DS_Store
+-rw-r--r--   0        0        0       55 2023-06-30 22:40:23.468901 scenic-3.0.0b2/src/scenic/core/__init__.py
+-rw-r--r--   0        0        0    51195 2023-06-30 22:40:23.469944 scenic-3.0.0b2/src/scenic/core/distributions.py
+-rw-r--r--   0        0        0    32997 2023-06-30 22:40:23.471175 scenic-3.0.0b2/src/scenic/core/dynamics.py
+-rw-r--r--   0        0        0    11090 2023-06-30 22:40:23.472296 scenic-3.0.0b2/src/scenic/core/errors.py
+-rw-r--r--   0        0        0    15140 2023-06-30 22:40:23.473237 scenic-3.0.0b2/src/scenic/core/external_params.py
+-rw-r--r--   0        0        0    10400 2023-06-30 22:40:23.474054 scenic-3.0.0b2/src/scenic/core/geometry.py
+-rw-r--r--   0        0        0     9536 2023-06-30 22:40:23.474969 scenic-3.0.0b2/src/scenic/core/lazy_eval.py
+-rw-r--r--   0        0        0    66305 2023-06-30 22:40:23.476364 scenic-3.0.0b2/src/scenic/core/object_types.py
+-rw-r--r--   0        0        0     6559 2023-06-30 22:40:23.477046 scenic-3.0.0b2/src/scenic/core/propositions.py
+-rw-r--r--   0        0        0    15990 2023-06-30 22:40:23.479989 scenic-3.0.0b2/src/scenic/core/pruning.py
+-rw-r--r--   0        0        0   138471 2023-06-30 22:40:23.482098 scenic-3.0.0b2/src/scenic/core/regions.py
+-rw-r--r--   0        0        0    13568 2023-06-30 22:40:23.482913 scenic-3.0.0b2/src/scenic/core/requirements.py
+-rw-r--r--   0        0        0     4393 2023-06-30 22:40:23.483637 scenic-3.0.0b2/src/scenic/core/sample_checking.py
+-rw-r--r--   0        0        0    28991 2023-06-30 22:40:23.484395 scenic-3.0.0b2/src/scenic/core/scenarios.py
+-rw-r--r--   0        0        0    11484 2023-06-30 22:40:23.485118 scenic-3.0.0b2/src/scenic/core/serialization.py
+-rw-r--r--   0        0        0     7264 2023-06-30 22:40:23.485675 scenic-3.0.0b2/src/scenic/core/shapes.py
+-rw-r--r--   0        0        0    39129 2023-06-30 22:40:23.486547 scenic-3.0.0b2/src/scenic/core/simulators.py
+-rw-r--r--   0        0        0     4445 2023-06-30 22:40:23.487268 scenic-3.0.0b2/src/scenic/core/specifiers.py
+-rw-r--r--   0        0        0    15751 2023-06-30 22:40:23.488150 scenic-3.0.0b2/src/scenic/core/type_support.py
+-rw-r--r--   0        0        0     6148 2023-04-20 16:43:54.707226 scenic-3.0.0b2/src/scenic/core/type_support/.DS_Store
+-rw-r--r--   0        0        0     5022 2023-06-30 22:40:23.488952 scenic-3.0.0b2/src/scenic/core/utils.py
+-rw-r--r--   0        0        0    27741 2023-06-30 22:40:23.489783 scenic-3.0.0b2/src/scenic/core/vectors.py
+-rw-r--r--   0        0        0    25874 2023-06-30 22:40:23.490355 scenic-3.0.0b2/src/scenic/core/visibility.py
+-rw-r--r--   0        0        0     4555 2023-06-30 22:40:23.491019 scenic-3.0.0b2/src/scenic/core/workspaces.py
+-rw-r--r--   0        0        0     6148 2022-09-29 05:01:12.946087 scenic-3.0.0b2/src/scenic/domains/.DS_Store
+-rw-r--r--   0        0        0       55 2023-05-09 15:10:50.304640 scenic-3.0.0b2/src/scenic/domains/__init__.py
+-rw-r--r--   0        0        0     2146 2023-05-09 15:10:50.304928 scenic-3.0.0b2/src/scenic/domains/driving/__init__.py
+-rw-r--r--   0        0        0     7626 2023-06-30 22:40:23.491706 scenic-3.0.0b2/src/scenic/domains/driving/actions.py
+-rw-r--r--   0        0        0    12962 2023-06-29 20:07:50.086992 scenic-3.0.0b2/src/scenic/domains/driving/behaviors.scenic
+-rw-r--r--   0        0        0     3000 2023-06-30 22:40:23.492538 scenic-3.0.0b2/src/scenic/domains/driving/controllers.py
+-rw-r--r--   0        0        0    12663 2023-06-30 22:40:23.493317 scenic-3.0.0b2/src/scenic/domains/driving/model.scenic
+-rw-r--r--   0        0        0    50790 2023-06-30 22:40:23.494161 scenic-3.0.0b2/src/scenic/domains/driving/roads.py
+-rw-r--r--   0        0        0     3017 2023-06-30 22:40:23.494785 scenic-3.0.0b2/src/scenic/domains/driving/simulators.py
+-rw-r--r--   0        0        0      387 2023-06-30 22:40:23.495478 scenic-3.0.0b2/src/scenic/domains/driving/workspace.py
+-rw-r--r--   0        0        0     6148 2020-09-15 22:57:40.000000 scenic-3.0.0b2/src/scenic/formats/.DS_Store
+-rw-r--r--   0        0        0       70 2023-05-09 15:10:50.306678 scenic-3.0.0b2/src/scenic/formats/__init__.py
+-rw-r--r--   0        0        0      127 2023-05-09 15:10:50.307038 scenic-3.0.0b2/src/scenic/formats/opendrive/__init__.py
+-rw-r--r--   0        0        0     1881 2023-06-30 22:40:23.497272 scenic-3.0.0b2/src/scenic/formats/opendrive/workspace.py
+-rw-r--r--   0        0        0    80566 2023-06-30 22:40:23.498250 scenic-3.0.0b2/src/scenic/formats/opendrive/xodr_parser.py
+-rw-r--r--   0        0        0     8196 2023-02-12 21:53:34.597183 scenic-3.0.0b2/src/scenic/simulators/.DS_Store
+-rw-r--r--   0        0        0       61 2023-05-09 15:10:50.308928 scenic-3.0.0b2/src/scenic/simulators/__init__.py
+-rw-r--r--   0        0        0     6148 2020-04-13 10:57:15.000000 scenic-3.0.0b2/src/scenic/simulators/carla/.DS_Store
+-rw-r--r--   0        0        0      750 2023-06-30 22:40:23.498929 scenic-3.0.0b2/src/scenic/simulators/carla/__init__.py
+-rw-r--r--   0        0        0     8255 2023-06-30 22:40:23.499712 scenic-3.0.0b2/src/scenic/simulators/carla/actions.py
+-rw-r--r--   0        0        0     2386 2023-06-30 22:40:23.500644 scenic-3.0.0b2/src/scenic/simulators/carla/behaviors.scenic
+-rw-r--r--   0        0        0     5292 2023-06-21 22:25:24.345822 scenic-3.0.0b2/src/scenic/simulators/carla/blueprints.scenic
+-rw-r--r--   0        0        0     6010 2023-06-30 22:40:23.501275 scenic-3.0.0b2/src/scenic/simulators/carla/misc.py
+-rw-r--r--   0        0        0    12784 2023-06-30 22:40:23.502215 scenic-3.0.0b2/src/scenic/simulators/carla/model.scenic
+-rw-r--r--   0        0        0    11780 2023-06-30 22:40:23.503028 scenic-3.0.0b2/src/scenic/simulators/carla/simulator.py
+-rw-r--r--   0        0        0     2536 2023-06-30 22:40:23.503894 scenic-3.0.0b2/src/scenic/simulators/carla/utils/utils.py
+-rw-r--r--   0        0        0    15118 2023-06-30 22:40:23.505021 scenic-3.0.0b2/src/scenic/simulators/carla/utils/visuals.py
+-rw-r--r--   0        0        0     6148 2020-04-13 07:04:31.000000 scenic-3.0.0b2/src/scenic/simulators/gta/.DS_Store
+-rw-r--r--   0        0        0      205 2023-06-30 22:40:23.505977 scenic-3.0.0b2/src/scenic/simulators/gta/__init__.py
+-rw-r--r--   0        0        0     8700 2023-06-30 22:40:23.506724 scenic-3.0.0b2/src/scenic/simulators/gta/center_detection.py
+-rw-r--r--   0        0        0     1496 2023-06-30 22:40:23.507436 scenic-3.0.0b2/src/scenic/simulators/gta/img_modf.py
+-rw-r--r--   0        0        0     8665 2023-06-30 22:40:23.508247 scenic-3.0.0b2/src/scenic/simulators/gta/interface.py
+-rw-r--r--   0        0        0      234 2023-06-30 22:40:23.508695 scenic-3.0.0b2/src/scenic/simulators/gta/map.py
+-rw-r--r--   0        0        0     4010 2023-06-30 22:40:23.509552 scenic-3.0.0b2/src/scenic/simulators/gta/messages.py
+-rw-r--r--   0        0        0     2747 2023-06-30 22:40:23.509911 scenic-3.0.0b2/src/scenic/simulators/gta/model.scenic
+-rw-r--r--   0        0        0      622 2023-06-30 22:40:23.510668 scenic-3.0.0b2/src/scenic/simulators/lgsvl/__init__.py
+-rw-r--r--   0        0        0     5130 2023-06-30 22:40:23.512361 scenic-3.0.0b2/src/scenic/simulators/lgsvl/actions.py
+-rw-r--r--   0        0        0      601 2023-06-30 22:40:23.512813 scenic-3.0.0b2/src/scenic/simulators/lgsvl/behaviors.scenic
+-rw-r--r--   0        0        0     4124 2023-06-30 22:40:23.513528 scenic-3.0.0b2/src/scenic/simulators/lgsvl/model.scenic
+-rw-r--r--   0        0        0     6114 2023-06-30 22:40:23.514263 scenic-3.0.0b2/src/scenic/simulators/lgsvl/simulator.py
+-rw-r--r--   0        0        0      979 2023-06-30 22:40:23.514816 scenic-3.0.0b2/src/scenic/simulators/lgsvl/utils.py
+-rw-r--r--   0        0        0      418 2023-05-09 15:10:50.313101 scenic-3.0.0b2/src/scenic/simulators/newtonian/__init__.py
+-rw-r--r--   0        0        0    73799 2022-04-24 16:36:45.983622 scenic-3.0.0b2/src/scenic/simulators/newtonian/car.png
+-rw-r--r--   0        0        0     1759 2023-06-30 22:40:23.515069 scenic-3.0.0b2/src/scenic/simulators/newtonian/driving_model.scenic
+-rw-r--r--   0        0        0      454 2023-06-29 20:07:50.091051 scenic-3.0.0b2/src/scenic/simulators/newtonian/model.scenic
+-rw-r--r--   0        0        0    10438 2023-06-30 22:40:23.515786 scenic-3.0.0b2/src/scenic/simulators/newtonian/simulator.py
+-rw-r--r--   0        0        0       59 2023-05-09 15:10:50.313974 scenic-3.0.0b2/src/scenic/simulators/utils/__init__.py
+-rw-r--r--   0        0        0     4389 2023-06-30 22:40:23.516386 scenic-3.0.0b2/src/scenic/simulators/utils/colors.py
+-rw-r--r--   0        0        0    10244 2023-02-13 14:29:52.230267 scenic-3.0.0b2/src/scenic/simulators/webots/.DS_Store
+-rw-r--r--   0        0        0     1609 2022-04-24 16:33:57.804475 scenic-3.0.0b2/src/scenic/simulators/webots/WBT.g4
+-rw-r--r--   0        0        0     5416 2023-06-30 22:40:23.517077 scenic-3.0.0b2/src/scenic/simulators/webots/WBTLexer.py
+-rw-r--r--   0        0        0    26753 2023-06-30 22:40:23.517884 scenic-3.0.0b2/src/scenic/simulators/webots/WBTParser.py
+-rw-r--r--   0        0        0     2032 2023-06-30 22:40:23.518740 scenic-3.0.0b2/src/scenic/simulators/webots/WBTVisitor.py
+-rw-r--r--   0        0        0      375 2023-06-30 22:40:23.519420 scenic-3.0.0b2/src/scenic/simulators/webots/__init__.py
+-rw-r--r--   0        0        0     1468 2023-06-30 22:40:23.520099 scenic-3.0.0b2/src/scenic/simulators/webots/actions.py
+-rw-r--r--   0        0        0     6148 2019-02-12 18:47:25.000000 scenic-3.0.0b2/src/scenic/simulators/webots/guideways/.DS_Store
+-rw-r--r--   0        0        0      291 2023-06-30 22:40:23.521027 scenic-3.0.0b2/src/scenic/simulators/webots/guideways/__init__.py
+-rw-r--r--   0        0        0     6049 2023-06-30 22:40:23.521974 scenic-3.0.0b2/src/scenic/simulators/webots/guideways/interface.py
+-rw-r--r--   0        0        0      311 2023-06-30 22:40:23.522290 scenic-3.0.0b2/src/scenic/simulators/webots/guideways/intersection.py
+-rw-r--r--   0        0        0     1270 2023-06-30 22:40:23.522879 scenic-3.0.0b2/src/scenic/simulators/webots/guideways/model.scenic
+-rw-r--r--   0        0        0     6148 2019-02-12 18:47:20.000000 scenic-3.0.0b2/src/scenic/simulators/webots/mars/.DS_Store
+-rw-r--r--   0        0        0    13755 2023-06-30 22:40:23.523654 scenic-3.0.0b2/src/scenic/simulators/webots/model.scenic
+-rw-r--r--   0        0        0     6148 2019-02-12 18:47:15.000000 scenic-3.0.0b2/src/scenic/simulators/webots/road/.DS_Store
+-rw-r--r--   0        0        0      178 2023-06-30 22:40:23.524575 scenic-3.0.0b2/src/scenic/simulators/webots/road/__init__.py
+-rw-r--r--   0        0        0      796 2023-06-30 22:40:23.525283 scenic-3.0.0b2/src/scenic/simulators/webots/road/car_models.py
+-rw-r--r--   0        0        0    16983 2023-06-30 22:40:23.526112 scenic-3.0.0b2/src/scenic/simulators/webots/road/interface.py
+-rw-r--r--   0        0        0     2949 2023-06-30 22:40:23.526921 scenic-3.0.0b2/src/scenic/simulators/webots/road/model.scenic
+-rw-r--r--   0        0        0      440 2023-06-30 22:40:23.527267 scenic-3.0.0b2/src/scenic/simulators/webots/road/world.py
+-rw-r--r--   0        0        0    11074 2023-06-30 22:40:23.528010 scenic-3.0.0b2/src/scenic/simulators/webots/simulator.py
+-rw-r--r--   0        0        0     3370 2023-06-30 22:40:23.528740 scenic-3.0.0b2/src/scenic/simulators/webots/utils.py
+-rw-r--r--   0        0        0     3429 2023-06-30 22:40:23.529388 scenic-3.0.0b2/src/scenic/simulators/webots/world_parser.py
+-rw-r--r--   0        0        0      215 2023-05-09 15:10:50.317105 scenic-3.0.0b2/src/scenic/simulators/xplane/__init__.py
+-rw-r--r--   0        0        0      262 2022-04-24 16:33:57.813980 scenic-3.0.0b2/src/scenic/simulators/xplane/model.scenic
+-rw-r--r--   0        0        0     6148 2022-09-27 14:43:55.355940 scenic-3.0.0b2/src/scenic/syntax/.DS_Store
+-rw-r--r--   0        0        0     1141 2023-06-30 22:40:23.530061 scenic-3.0.0b2/src/scenic/syntax/__init__.py
+-rw-r--r--   0        0        0    32133 2023-06-30 22:40:23.530497 scenic-3.0.0b2/src/scenic/syntax/ast.py
+-rw-r--r--   0        0        0    60871 2023-06-30 22:40:23.531247 scenic-3.0.0b2/src/scenic/syntax/compiler.py
+-rw-r--r--   0        0        0   468409 2023-06-30 18:16:53.130193 scenic-3.0.0b2/src/scenic/syntax/parser.py
+-rw-r--r--   0        0        0    33410 2023-06-30 22:40:23.532150 scenic-3.0.0b2/src/scenic/syntax/pygment.py
+-rw-r--r--   0        0        0     9042 2023-06-30 22:40:23.532913 scenic-3.0.0b2/src/scenic/syntax/relations.py
+-rw-r--r--   0        0        0    96273 2023-06-30 22:40:23.534325 scenic-3.0.0b2/src/scenic/syntax/scenic.gram
+-rw-r--r--   0        0        0    26355 2023-06-30 22:40:23.535315 scenic-3.0.0b2/src/scenic/syntax/translator.py
+-rw-r--r--   0        0        0    64003 2023-06-30 22:40:23.536531 scenic-3.0.0b2/src/scenic/syntax/veneer.py
+-rw-r--r--   0        0        0     4193 1970-01-01 00:00:00.000000 scenic-3.0.0b2/PKG-INFO
```

### Comparing `scenic-2.1.0b4/LICENSE` & `scenic-3.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `scenic-2.1.0b4/README.md` & `scenic-3.0.0b2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Scenic
 
 [![Documentation Status](https://readthedocs.org/projects/scenic-lang/badge/?version=latest)](https://scenic-lang.readthedocs.io/en/latest/?badge=latest)
+[![Tests Status](https://github.com/BerkeleyLearnVerify/Scenic/actions/workflows/run-tests.yml/badge.svg)](https://github.com/BerkeleyLearnVerify/Scenic/actions/workflows/run-tests.yml)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
 A compiler and scenario generator for the Scenic scenario description language.
 Please see the [documentation](https://scenic-lang.readthedocs.io/) for installation instructions, as well as tutorials and other information about the Scenic language, its implementation, and its interfaces to various simulators.
 
 For a description of the language and some of its applications, see [our journal paper](https://link.springer.com/article/10.1007/s10994-021-06120-5), which extends our [PLDI 2019 paper](https://arxiv.org/abs/1809.09310) (*note:* the syntax of Scenic has changed slightly since the PLDI paper, and many features such as support for dynamic scenarios have been added; these are described in the journal paper).
 Scenic was designed and implemented by Daniel J. Fremont, Edward Kim, Tommaso Dreossi, Shromona Ghosh, Xiangyu Yue, Alberto L. Sangiovanni-Vincentelli, and Sanjit A. Seshia.
```

### Comparing `scenic-2.1.0b4/src/scenic/__main__.py` & `scenic-3.0.0b2/src/scenic/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,216 +1,334 @@
-
 ### Top-level functionality of the scenic package as a script:
 ### load a scenario and generate scenes in an infinite loop.
 
-import sys
-import time
 import argparse
+from importlib import metadata
 import random
+import sys
+import time
+import warnings
 
-if sys.version_info >= (3, 8):
-    from importlib import metadata
-else:
-    import importlib_metadata as metadata
+import numpy
 
-import scenic.syntax.translator as translator
+import scenic
+from scenic.core.distributions import RejectionException
 import scenic.core.errors as errors
 from scenic.core.simulators import SimulationCreationError
+import scenic.syntax.translator as translator
+
+parser = argparse.ArgumentParser(
+    prog="scenic",
+    add_help=False,
+    usage="scenic [-h | --help] [options] FILE [options]",
+    description="Sample from a Scenic scenario, optionally "
+    "running dynamic simulations.",
+)
 
-parser = argparse.ArgumentParser(prog='scenic', add_help=False,
-                                 usage='scenic [-h | --help] [options] FILE [options]',
-                                 description='Sample from a Scenic scenario, optionally '
-                                             'running dynamic simulations.')
-
-mainOptions = parser.add_argument_group('main options')
-mainOptions.add_argument('-S', '--simulate', action='store_true',
-                         help='run dynamic simulations from scenes '
-                              'instead of simply showing diagrams of scenes')
-mainOptions.add_argument('-s', '--seed', help='random seed', type=int)
-mainOptions.add_argument('-v', '--verbosity', help='verbosity level (default 1)',
-                         type=int, choices=(0, 1, 2, 3), default=1)
-mainOptions.add_argument('-p', '--param', help='override a global parameter',
-                         nargs=2, default=[], action='append', metavar=('PARAM', 'VALUE'))
-mainOptions.add_argument('-m', '--model', help='specify a Scenic world model', default=None)
-mainOptions.add_argument('--scenario', default=None,
-                         help='name of scenario to run (if file contains multiple)')
+mainOptions = parser.add_argument_group("main options")
+mainOptions.add_argument(
+    "-S",
+    "--simulate",
+    action="store_true",
+    help="run dynamic simulations from scenes "
+    "instead of simply showing diagrams of scenes",
+)
+mainOptions.add_argument("-s", "--seed", help="random seed", type=int)
+mainOptions.add_argument(
+    "-v",
+    "--verbosity",
+    help="verbosity level (default 1)",
+    type=int,
+    choices=(0, 1, 2, 3),
+    default=1,
+)
+mainOptions.add_argument(
+    "-p",
+    "--param",
+    help="override a global parameter",
+    nargs=2,
+    default=[],
+    action="append",
+    metavar=("PARAM", "VALUE"),
+)
+mainOptions.add_argument(
+    "-m", "--model", help="specify a Scenic world model", default=None
+)
+mainOptions.add_argument(
+    "--scenario", default=None, help="name of scenario to run (if file contains multiple)"
+)
+mainOptions.add_argument(
+    "--2d", action="store_true", help="run Scenic in 2D compatibility mode"
+)
 
 # Simulation options
-simOpts = parser.add_argument_group('dynamic simulation options')
-simOpts.add_argument('--time', help='time bound for simulations (default none)',
-                     type=int, default=None)
-simOpts.add_argument('--count', help='number of successful simulations to run (default infinity)',
-                     type=int, default=0)
-simOpts.add_argument('--max-sims-per-scene', type=int, default=1, metavar='N',
-                     help='max # of rejected simulations before sampling a new scene (default 1)')
+simOpts = parser.add_argument_group("dynamic simulation options")
+simOpts.add_argument(
+    "--time", help="time bound for simulations (default none)", type=int, default=None
+)
+simOpts.add_argument(
+    "--count",
+    help="number of successful simulations to run (default infinity)",
+    type=int,
+    default=0,
+)
+simOpts.add_argument(
+    "--max-sims-per-scene",
+    type=int,
+    default=1,
+    metavar="N",
+    help="max # of rejected simulations before sampling a new scene (default 1)",
+)
 
 # Interactive rendering options
-intOptions = parser.add_argument_group('static scene diagramming options')
-intOptions.add_argument('-d', '--delay', type=float,
-                        help='loop automatically with this delay (in seconds) '
-                             'instead of waiting for the user to close the diagram')
-intOptions.add_argument('-z', '--zoom', help='zoom expansion factor (default 1)',
-                        type=float, default=1)
+intOptions = parser.add_argument_group("static scene diagramming options")
+intOptions.add_argument(
+    "-d",
+    "--delay",
+    type=float,
+    help="loop automatically with this delay (in seconds) "
+    "instead of waiting for the user to close the diagram",
+)
+intOptions.add_argument(
+    "-z",
+    "--zoom",
+    type=float,
+    default=1,
+    help="zoom expansion factor, or 0 to show the whole workspace (default 1)",
+)
+intOptions.add_argument(
+    "--axes", help="display the global coordinate axes", action="store_true"
+)
 
 # Debugging options
-debugOpts = parser.add_argument_group('debugging options')
-debugOpts.add_argument('--show-params', help='show values of global parameters',
-                       action='store_true')
-debugOpts.add_argument('--show-records', help='show values of recorded expressions',
-                       action='store_true')
-debugOpts.add_argument('-b', '--full-backtrace', help='show full internal backtraces',
-                       action='store_true')
-debugOpts.add_argument('--pdb', action='store_true',
-                       help='enter interactive debugger on errors (implies "-b")')
-debugOpts.add_argument('--pdb-on-reject', action='store_true',
-                       help='enter interactive debugger on rejections (implies "-b")')
-ver = metadata.version('scenic')
-debugOpts.add_argument('--version', action='version', version=f'Scenic {ver}',
-                       help='print Scenic version information and exit')
-debugOpts.add_argument('--dump-initial-python', help='dump initial translated Python',
-                       action='store_true')
-debugOpts.add_argument('--dump-ast', help='dump final AST', action='store_true')
-debugOpts.add_argument('--dump-python', help='dump Python equivalent of final AST',
-                       action='store_true')
-debugOpts.add_argument('--no-pruning', help='disable pruning', action='store_true')
-debugOpts.add_argument('--gather-stats', type=int, metavar='N',
-                       help='collect timing statistics over this many scenes')
+debugOpts = parser.add_argument_group("debugging options")
+debugOpts.add_argument(
+    "--show-params", help="show values of global parameters", action="store_true"
+)
+debugOpts.add_argument(
+    "--show-records", help="show values of recorded expressions", action="store_true"
+)
+debugOpts.add_argument(
+    "-b", "--full-backtrace", help="show full internal backtraces", action="store_true"
+)
+debugOpts.add_argument(
+    "--pdb",
+    action="store_true",
+    help='enter interactive debugger on errors (implies "-b")',
+)
+debugOpts.add_argument(
+    "--pdb-on-reject",
+    action="store_true",
+    help='enter interactive debugger on rejections (implies "-b")',
+)
+ver = metadata.version("scenic")
+debugOpts.add_argument(
+    "--version",
+    action="version",
+    version=f"Scenic {ver}",
+    help="print Scenic version information and exit",
+)
+debugOpts.add_argument("--dump-scenic-ast", help="dump Scenic AST", action="store_true")
+debugOpts.add_argument("--dump-ast", help="dump final AST", action="store_true")
+debugOpts.add_argument(
+    "--dump-python", help="dump Python equivalent of final AST", action="store_true"
+)
+debugOpts.add_argument("--no-pruning", help="disable pruning", action="store_true")
+debugOpts.add_argument(
+    "--gather-stats",
+    type=int,
+    metavar="N",
+    help="collect timing statistics over this many scenes"
+    " (or iterations, if negative)",
+)
 
-parser.add_argument('-h', '--help', action='help', default=argparse.SUPPRESS,
-                    help=argparse.SUPPRESS)
+parser.add_argument(
+    "-h", "--help", action="help", default=argparse.SUPPRESS, help=argparse.SUPPRESS
+)
 
 # Positional arguments
-parser.add_argument('scenicFile', help='a Scenic file to run', metavar='FILE')
+parser.add_argument("scenicFile", help="a Scenic file to run", metavar="FILE")
 
 # Parse arguments and set up configuration
 args = parser.parse_args()
 delay = args.delay
-errors.showInternalBacktrace = args.full_backtrace
-if args.pdb:
-    errors.postMortemDebugging = True
-    errors.showInternalBacktrace = True
-if args.pdb_on_reject:
-    errors.postMortemRejections = True
-    errors.showInternalBacktrace = True
+mode2D = getattr(args, "2d")
+
+if not mode2D:
+    if args.delay is not None:
+        warnings.warn("Delay parameter is not supported by the 3D viewer.")
+    if args.zoom != 1:
+        warnings.warn("Zoom parameter is not supported by the 3D viewer.")
+
+scenic.setDebuggingOptions(
+    verbosity=args.verbosity,
+    fullBacktrace=args.full_backtrace,
+    debugExceptions=args.pdb,
+    debugRejections=args.pdb_on_reject,
+)
 params = {}
 for name, value in args.param:
     # Convert params to ints or floats if possible
     try:
         value = int(value)
     except ValueError:
         try:
             value = float(value)
         except ValueError:
             pass
     params[name] = value
-translator.dumpTranslatedPython = args.dump_initial_python
+translator.dumpScenicAST = args.dump_scenic_ast
 translator.dumpFinalAST = args.dump_ast
 translator.dumpASTPython = args.dump_python
-translator.verbosity = args.verbosity
 translator.usePruning = not args.no_pruning
-if args.seed is not None and args.verbosity >= 1:
-    print(f'Using random seed = {args.seed}')
+if args.seed is not None:
+    if args.verbosity >= 1:
+        print(f"Using random seed = {args.seed}")
+
     random.seed(args.seed)
+    numpy.random.seed(args.seed)
 
 # Load scenario from file
 if args.verbosity >= 1:
-    print('Beginning scenario construction...')
+    print("Beginning scenario construction...")
 startTime = time.time()
 scenario = errors.callBeginningScenicTrace(
-    lambda: translator.scenarioFromFile(args.scenicFile,
-                                        params=params,
-                                        model=args.model,
-                                        scenario=args.scenario)
+    lambda: translator.scenarioFromFile(
+        args.scenicFile,
+        params=params,
+        model=args.model,
+        scenario=args.scenario,
+        mode2D=mode2D,
+    )
 )
 totalTime = time.time() - startTime
 if args.verbosity >= 1:
-    print(f'Scenario constructed in {totalTime:.2f} seconds.')
+    print(f"Scenario constructed in {totalTime:.2f} seconds.")
 
 if args.simulate:
     simulator = errors.callBeginningScenicTrace(scenario.getSimulator)
 
-def generateScene():
+
+def generateScene(maxIterations=2000):
     startTime = time.time()
     scene, iterations = errors.callBeginningScenicTrace(
-        lambda: scenario.generate(verbosity=args.verbosity)
+        lambda: scenario.generate(maxIterations=maxIterations, verbosity=args.verbosity)
     )
     if args.verbosity >= 1:
         totalTime = time.time() - startTime
-        print(f'  Generated scene in {iterations} iterations, {totalTime:.4g} seconds.')
+        print(f"  Generated scene in {iterations} iterations, {totalTime:.4g} seconds.")
         if args.show_params:
             for param, value in scene.params.items():
                 print(f'    Parameter "{param}": {value}')
     return scene, iterations
 
+
 def runSimulation(scene):
     startTime = time.time()
     if args.verbosity >= 1:
-        print(f'  Beginning simulation of {scene.dynamicScenario}...')
+        print(f"  Beginning simulation of {scene.dynamicScenario}...")
     try:
         simulation = errors.callBeginningScenicTrace(
-            lambda: simulator.simulate(scene, maxSteps=args.time, verbosity=args.verbosity,
-                                       maxIterations=args.max_sims_per_scene)
+            lambda: simulator.simulate(
+                scene,
+                maxSteps=args.time,
+                verbosity=args.verbosity,
+                maxIterations=args.max_sims_per_scene,
+            )
         )
     except SimulationCreationError as e:
         if args.verbosity >= 1:
-            print(f'  Failed to create simulation: {e}')
+            print(f"  Failed to create simulation: {e}")
         return False
     if args.verbosity >= 1:
         totalTime = time.time() - startTime
-        print(f'  Ran simulation in {totalTime:.4g} seconds.')
+        print(f"  Ran simulation in {totalTime:.4g} seconds.")
     if simulation and args.show_records:
         for name, value in simulation.result.records.items():
             if isinstance(value, list):
                 print(f'    Record "{name}": (time series)')
                 for step, subval in value:
-                    print(f'      {step:4d}: {subval}')
+                    print(f"      {step:4d}: {subval}")
             else:
                 print(f'    Record "{name}": {value}')
     return simulation is not None
 
+
 try:
-    if args.gather_stats is None:   # Generate scenes interactively until killed
-        if not args.simulate:   # will need matplotlib to draw scene schematic
+    if args.gather_stats is None:  # Generate scenes interactively until killed
+        if not args.simulate:  # will need matplotlib to draw scene schematic
             import matplotlib
             import matplotlib.pyplot as plt
-            if matplotlib.get_backend().lower() == 'agg':
+
+            if matplotlib.get_backend().lower() == "agg":
                 raise RuntimeError(
-                    'need an interactive matplotlib backend to display scenes\n'
-                    '(try installing python3-tk)')
+                    "need an interactive matplotlib backend to display scenes\n"
+                    "(try installing python3-tk)"
+                )
 
         successCount = 0
         while True:
             scene, _ = generateScene()
             if args.simulate:
                 success = runSimulation(scene)
                 if success:
                     successCount += 1
                     if 0 < args.count <= successCount:
                         break
             else:
-                if delay is None:
-                    scene.show(zoom=args.zoom)
+                if mode2D:
+                    if delay is None:
+                        scene.show2D(zoom=args.zoom)
+                    else:
+                        scene.show2D(zoom=args.zoom, block=False)
+                        plt.pause(delay)
+                        plt.clf()
                 else:
-                    scene.show(zoom=args.zoom, block=False)
-                    plt.pause(delay)
-                    plt.clf()
-    else:   # Gather statistics over the specified number of scenes
+                    scene.show(axes=args.axes)
+
+    else:  # Gather statistics over the specified number of scenes/iterations
         its = []
+        maxIterations = 2000
+        iterations = 0
+        totalIterations = 0
+        if args.gather_stats >= 0:  # scenes
+
+            def keepGoing():
+                return len(its) < args.gather_stats
+
+        else:  # iterations
+            maxIterations = -args.gather_stats
+
+            def keepGoing():
+                global maxIterations
+                maxIterations -= iterations
+                return maxIterations > 0
+
         startTime = time.time()
-        while len(its) < args.gather_stats:
-            scene, iterations = generateScene()
-            its.append(iterations)
+        while keepGoing():
+            try:
+                scene, iterations = generateScene(maxIterations=maxIterations)
+            except RejectionException:
+                if args.gather_stats >= 0:
+                    raise
+                iterations = maxIterations
+            else:
+                its.append(iterations)
+            totalIterations += iterations
         totalTime = time.time() - startTime
-        count = len(its)
-        print(f'Sampled {len(its)} scenes in {totalTime:.2f} seconds.')
-        print(f'Average iterations/scene: {sum(its)/count}')
-        print(f'Average time/scene: {totalTime/count:.2f} seconds.')
+
+        count = len(its) if its else float("nan")
+        print(f"Sampled {len(its)} scenes in {totalTime:.2f} seconds.")
+        print(f"Average iterations/scene: {totalIterations/count}")
+        print(f"Average time/iteration: {totalTime/totalIterations:.2g} seconds.")
+        print(f"Average time/scene: {totalTime/count:.2f} seconds.")
 
 except KeyboardInterrupt:
     pass
 
 finally:
     if args.simulate:
         simulator.destroy()
 
-def dummy():    # for the 'scenic' entry point to call after importing this module
+
+def dummy():  # for the 'scenic' entry point to call after importing this module
     pass
```

### Comparing `scenic-2.1.0b4/src/scenic/core/dynamics.py` & `scenic-3.0.0b2/src/scenic/core/dynamics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,74 @@
 """Support for dynamic behaviors and modular scenarios."""
 
 from collections import defaultdict
+import dataclasses
 import enum
+import functools
 import inspect
 import itertools
+import sys
 import types
 import warnings
+import weakref
 
-from scenic.core.distributions import Samplable, Options, toDistribution, needsSampling
-from scenic.core.errors import RuntimeParseError, InvalidScenarioError
+import rv_ltl
+
+from scenic.core.distributions import Options, Samplable, needsSampling, toDistribution
+from scenic.core.errors import InvalidScenarioError
 from scenic.core.lazy_eval import DelayedArgument, needsLazyEvaluation
-from scenic.core.requirements import (RequirementType, PendingRequirement,
-                                      DynamicRequirement)
-from scenic.core.simulators import (RejectSimulationException, EndSimulationAction,
-                                    EndScenarioAction)
-from scenic.core.utils import argsToString, alarm
+from scenic.core.requirements import (
+    DynamicRequirement,
+    PendingRequirement,
+    RequirementType,
+)
+from scenic.core.simulators import (
+    EndScenarioAction,
+    EndSimulationAction,
+    RejectSimulationException,
+)
+from scenic.core.type_support import CoercionFailure
+from scenic.core.utils import alarm, argsToString
+from scenic.core.workspaces import Workspace
 
 # Utilities
 
+
 class StuckBehaviorWarning(UserWarning):
     """Warning issued when a behavior/scenario may have gotten stuck.
 
     When a behavior or compose block of a modular scenario executes for a long
     time without yielding control, there is no way to tell whether it has
     entered an infinite loop with no take/wait statements, or is actually doing
     some long computation. But since forgetting a wait statement in a wait loop
     is an easy mistake, we raise this warning after a behavior/scenario has run
     for `stuckBehaviorWarningTimeout` seconds without yielding.
     """
+
     pass
 
+
 #: Timeout in seconds after which a `StuckBehaviorWarning` will be raised.
 stuckBehaviorWarningTimeout = 10
 
 # Scenarios
 
+
 class Invocable:
     """Abstract class with common code for behaviors and modular scenarios.
 
     Both of these types of objects can be called like functions, can have guards, and can
     suspend their own execution to invoke sub-behaviors/scenarios.
     """
+
     def __init__(self, *args, **kwargs):
         if veneer.evaluatingGuard:
-            raise RuntimeParseError(
-                'tried to invoke behavior/scenario from inside guard or interrupt condition')
+            raise InvalidScenarioError(
+                "tried to invoke behavior/scenario from inside guard or interrupt condition"
+            )
         self._args = args
         self._kwargs = kwargs
         self._agent = None
         self._runningIterator = None
         self._isRunning = False
 
     def _start(self):
@@ -80,71 +100,80 @@
                 self._kwargs[name] = arg.evaluateInner(None)
 
     def _invokeSubBehavior(self, agent, subs, modifier=None, schedule=None):
         def pickEnabledInvocable(opts):
             enabled = {}
             if isinstance(opts, dict):
                 for sub, weight in opts.items():
-                    if sub._isEnabled:
+                    if sub._isEnabledForAgent(agent):
                         enabled[sub] = weight
             else:
                 for sub in opts:
-                    if sub._isEnabled:
+                    if sub._isEnabledForAgent(agent):
                         enabled[sub] = 1
             if not enabled:
                 raise RejectSimulationException('deadlock in "do choose/shuffle"')
             if len(enabled) == 1:
                 choice = list(enabled)[0]
             else:
                 choice = Options(enabled)
             return choice
 
         scheduler = None
-        if schedule == 'choose':
+        if schedule == "choose":
             if len(subs) == 1 and isinstance(subs[0], dict):
                 subs = subs[0]
             subs = (pickEnabledInvocable(subs),)
-        elif schedule == 'shuffle':
+        elif schedule == "shuffle":
             if len(subs) == 1 and isinstance(subs[0], dict):
                 subs = subs[0]
             else:
                 subs = {item: 1 for item in subs}
+
             def scheduler():
                 while subs:
                     choice = pickEnabledInvocable(subs)
                     subs.pop(choice)
                     yield from self._invokeInner(agent, (choice,))
+
         else:
             assert schedule is None
         if not scheduler:
+
             def scheduler():
                 yield from self._invokeInner(agent, subs)
 
         if modifier:
-            if modifier.name == 'for':  # do X for Y [seconds | steps]
+            if modifier.name == "for":  # do X for Y [seconds | steps]
                 timeLimit = modifier.value
                 if not isinstance(timeLimit, (float, int)):
-                    raise RuntimeParseError('"do X for Y" with Y not a number')
-                assert modifier.terminator in (None, 'seconds', 'steps')
-                if modifier.terminator != 'steps':
+                    raise TypeError('"do X for Y" with Y not a number')
+                assert modifier.terminator in (None, "seconds", "steps")
+                if modifier.terminator != "steps":
                     timeLimit /= veneer.currentSimulation.timestep
                 startTime = veneer.currentSimulation.currentTime
-                condition = lambda: veneer.currentSimulation.currentTime - startTime >= timeLimit
-            elif modifier.name == 'until':  # do X until Y
+                condition = (
+                    lambda: veneer.currentSimulation.currentTime - startTime >= timeLimit
+                )
+            elif modifier.name == "until":  # do X until Y
                 condition = modifier.value
             else:
-                raise RuntimeError(f'internal parsing error: impossible modifier {modifier}')
+                raise RuntimeError(
+                    f"internal parsing error: impossible modifier {modifier}"
+                )
 
             def body(behavior, agent):
                 yield from scheduler()
+
             def handler(behavior, agent):
                 for sub in subs:
                     if sub._isRunning:
                         sub._stop(f'"{modifier.name}" condition met')
                 return BlockConclusion.ABORT
+
             yield from runTryInterrupt(self, agent, body, [condition], [handler])
         else:
             yield from scheduler()
 
     def _invokeInner(self, agent, subs):
         """Run the given sub-behavior/scenario(s) in parallel.
 
@@ -152,75 +181,92 @@
         """
         raise NotImplementedError
 
     def _checkAllPreconditions(self):
         self.checkPreconditions(self._agent, *self._args, **self._kwargs)
         self.checkInvariants(self._agent, *self._args, **self._kwargs)
 
-    @property
-    def _isEnabled(self):
+    def _isEnabledForAgent(self, agent):
+        assert not self._isRunning
+        assert self._agent is None
         try:
+            self._agent = agent  # in case `self` is used in a precondition
             self._checkAllPreconditions()
             return True
         except GuardViolation:
             return False
+        finally:
+            self._agent = None
+
 
 class DynamicScenario(Invocable):
     """Internal class for scenarios which can execute during dynamic simulations.
 
     Provides additional information complementing `Scenario`, which originally only
     supported static scenarios. The two classes should probably eventually be merged.
     """
+
     def __init_subclass__(cls, *args, **kwargs):
         veneer.registerDynamicScenarioClass(cls)
 
-    _requirementSyntax = None   # overridden by subclasses
+        target = cls._setup or cls._compose or (lambda self, agent: 0)
+        target = functools.partial(target, 0, 0)  # account for Scenic-inserted args
+        cls.__signature__ = inspect.signature(target)
+
+    _requirementSyntax = None  # overridden by subclasses
     _simulatorFactory = None
     _globalParameters = None
     _locals = ()
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._ego = None
-        self._objects = []      # ordered for reproducibility
+        self._workspace = None
+        self._instances = []  # ordered for reproducibility
+        # _objects should contain a reference to the most complete version of
+        # the objects in this scene (sampled > unsampled)
+        self._objects = []  # ordered for reproducibility
+        self._sampledObjects = self._objects
         self._externalParameters = []
         self._pendingRequirements = defaultdict(list)
         self._requirements = []
-        self._requirementDeps = set()   # things needing to be sampled to evaluate the requirements
+        # things needing to be sampled to evaluate the requirements
+        self._requirementDeps = set()
 
         self._agents = []
         self._monitors = []
         self._behaviors = []
-        self._alwaysRequirements = []
-        self._eventuallyRequirements = []
+        self._monitorRequirements = []
+        self._temporalRequirements = []
         self._terminationConditions = []
         self._terminateSimulationConditions = []
         self._recordedExprs = []
         self._recordedInitialExprs = []
         self._recordedFinalExprs = []
 
         self._subScenarios = []
         self._endWithBehaviors = False
         self._timeLimit = None
         self._timeLimitIsInSeconds = False
         self._prepared = False
         self._delayingPreconditionCheck = False
         self._dummyNamespace = None
 
-        self._timeLimitInSteps = None   # computed at simulation time
+        self._timeLimitInSteps = None  # computed at simulation time
         self._elapsedTime = 0
         self._eventuallySatisfied = None
         self._overrides = {}
 
+        self._requirementMonitors = None
+
     @classmethod
-    def _dummy(cls, filename, namespace):
+    def _dummy(cls, namespace):
         scenario = cls()
         scenario._setup = None
         scenario._compose = None
-        scenario._filename = filename   # for debugging
         scenario._prepared = True
         scenario._dummyNamespace = namespace
         return scenario
 
     @classmethod
     def _requiresArguments(cls):
         """Whether this scenario cannot be instantiated without arguments."""
@@ -228,15 +274,15 @@
             func = cls._setup
         elif cls._compose:
             func = cls._compose
         else:
             return True
         sig = inspect.signature(func)
         try:
-            sig.bind(None, None)    # first two arguments are added internally by Scenic
+            sig.bind(None, None)  # first two arguments are added internally by Scenic
             return False
         except TypeError:
             return True
 
     @property
     def ego(self):
         if self._ego is None:
@@ -246,30 +292,31 @@
     @property
     def objects(self):
         return tuple(self._objects)
 
     def _bindTo(self, scene):
         """Bind this scenario to a sampled scene when starting a new simulation."""
         self._ego = scene.egoObject
+        self._workspace = scene.workspace
         self._objects = list(scene.objects)
         self._agents = [obj for obj in scene.objects if obj.behavior is not None]
-        self._alwaysRequirements = scene.alwaysRequirements
-        self._eventuallyRequirements = scene.eventuallyRequirements
+        self._monitors = list(scene.monitors)
+        self._temporalRequirements = scene.temporalRequirements
         self._terminationConditions = scene.terminationConditions
         self._terminateSimulationConditions = scene.terminateSimulationConditions
         self._recordedExprs = scene.recordedExprs
         self._recordedInitialExprs = scene.recordedInitialExprs
         self._recordedFinalExprs = scene.recordedFinalExprs
 
     def _prepare(self, delayPreconditionCheck=False):
         """Prepare the scenario for execution, executing its setup block."""
         assert not self._prepared
         self._prepared = True
 
-        self._finalizeArguments()   # TODO generalize _prepare for Invocable?
+        self._finalizeArguments()  # TODO generalize _prepare for Invocable?
 
         veneer.prepareScenario(self)
         with veneer.executeInScenario(self, inheritEgo=True):
             # Check preconditions and invariants
             if delayPreconditionCheck:
                 self._delayingPreconditionCheck = True
             else:
@@ -300,199 +347,249 @@
 
         # Compute time limit now that we know the simulation timestep
         self._elapsedTime = 0
         self._timeLimitInSteps = self._timeLimit
         if self._timeLimitIsInSeconds:
             self._timeLimitInSteps /= veneer.currentSimulation.timestep
 
-        # Keep track of which 'require eventually' conditions have been satisfied
-        self._eventuallySatisfied = { req: False for req in self._eventuallyRequirements }
+        # create monitors for each requirement used for this simulation
+        self._requirementMonitors = [r.toMonitor() for r in self._temporalRequirements]
 
         veneer.startScenario(self)
         with veneer.executeInScenario(self):
             # Start compose block
             if self._compose is not None:
                 if not inspect.isgeneratorfunction(self._compose):
                     from scenic.syntax.translator import composeBlock
-                    raise RuntimeParseError(f'"{composeBlock}" does not invoke any scenarios')
+
+                    raise InvalidScenarioError(
+                        f'"{composeBlock}" does not invoke any scenarios'
+                    )
                 self._runningIterator = self._compose(None, *self._args, **self._kwargs)
 
             # Initialize behavior coroutines of agents
             for agent in self._agents:
-                assert isinstance(agent.behavior, Behavior), agent.behavior
-                agent.behavior._start(agent)
+                behavior = agent.behavior
+                assert isinstance(behavior, Behavior), behavior
+                behavior._assignTo(agent)
             # Initialize monitor coroutines
             for monitor in self._monitors:
                 monitor._start()
 
     def _step(self):
         """Execute the (already-started) scenario for one time step.
 
         Returns:
             `None` if the scenario will continue executing; otherwise a string describing
             why it has terminated.
         """
         super()._step()
 
-        # Check 'require always' and 'require eventually' conditions
-        for req in self._alwaysRequirements:
-            if not req.isTrue():
-                # always requirements should never be violated at time 0, since
-                # they are enforced during scene sampling
-                assert veneer.currentSimulation.currentTime > 0
-                raise RejectSimulationException(str(req))
-        for req in self._eventuallyRequirements:
-            if not self._eventuallySatisfied[req] and req.isTrue():
-                self._eventuallySatisfied[req] = True
+        # Check temporal requirements
+        for m in self._requirementMonitors:
+            result = m.value()
+            if result == rv_ltl.B4.FALSE:
+                raise RejectSimulationException(str(m))
 
         # Check if we have reached the time limit, if any
-        if self._timeLimitInSteps is not None and self._elapsedTime >= self._timeLimitInSteps:
-            return self._stop('reached time limit')
+        if (
+            self._timeLimitInSteps is not None
+            and self._elapsedTime >= self._timeLimitInSteps
+        ):
+            return self._stop("reached time limit")
         self._elapsedTime += 1
 
         # Execute compose block, if any
         composeDone = False
         if self._runningIterator is None:
-            composeDone = True      # compose block ended in an earlier step
+            composeDone = True  # compose block ended in an earlier step
         else:
+
             def alarmHandler(signum, frame):
-                warnings.warn(f'the compose block of scenario {self} is taking a long time; '
-                              'maybe you have an infinite loop with no "wait" statement?',
-                              StuckBehaviorWarning)
-            with veneer.executeInScenario(self), alarm(stuckBehaviorWarningTimeout, alarmHandler):
+                if sys.gettrace():
+                    return  # skip the warning if we're in the debugger
+                warnings.warn(
+                    f"the compose block of scenario {self} is taking a long time; "
+                    'maybe you have an infinite loop with no "wait" statement?',
+                    StuckBehaviorWarning,
+                )
+
+            with veneer.executeInScenario(self), alarm(
+                stuckBehaviorWarningTimeout, alarmHandler
+            ):
                 try:
                     result = self._runningIterator.send(None)
                     if isinstance(result, (EndSimulationAction, EndScenarioAction)):
                         return self._stop(result)
                 except StopIteration:
                     self._runningIterator = None
                     composeDone = True
 
         # If there is a compose block and it has finished, we're done
         if self._compose is not None and composeDone:
-            return self._stop('finished compose block')
+            return self._stop("finished compose block")
 
         # Optionally end when all our agents' behaviors have ended
         if self._endWithBehaviors:
             if all(agent.behavior._isFinished for agent in self._agents):
-                return self._stop('all behaviors finished')
+                return self._stop("all behaviors finished")
 
         # Check if any termination conditions apply
         for req in self._terminationConditions:
-            if req.isTrue():
+            if req.evaluate():
                 return self._stop(req)
 
         # Scenario will not terminate yet
         return None
 
     def _stop(self, reason, quiet=False):
         """Stop the scenario's execution, for the given reason."""
-        if not quiet:
-            # Reject if we never satisfied a 'require eventually'
-            for req in self._eventuallyRequirements:
-                if not self._eventuallySatisfied[req] and not req.isTrue():
-                    raise RejectSimulationException(str(req))
+        assert self._isRunning
 
-        super()._stop(reason)
-        veneer.endScenario(self, reason, quiet=quiet)
+        # Stop monitors and subscenarios.
+        for monitor in self._monitors:
+            if monitor._isRunning:
+                monitor._stop()
+        self._monitors = []
+        for sub in self._subScenarios:
+            if sub._isRunning:
+                sub._stop("parent scenario ending", quiet=quiet)
+        self._runningIterator = None
+
+        # Revert overrides.
         for obj, oldVals in self._overrides.items():
             obj._revert(oldVals)
-        self._runningIterator = None
+
+        # Inform the veneer we have stopped, and mark ourselves finished.
+        veneer.endScenario(self, reason, quiet=quiet)
+        super()._stop(reason)
+
+        # Reject if a temporal requirement was not satisfied.
+        if not quiet:
+            for req in self._requirementMonitors:
+                if req.lastValue.is_falsy:
+                    raise RejectSimulationException(str(req))
+        self._requirementMonitors = None
+
         return reason
 
     def _invokeInner(self, agent, subs):
         for sub in subs:
             if not isinstance(sub, DynamicScenario):
-                raise RuntimeParseError(f'expected a scenario, got {sub}')
+                raise TypeError(f"expected a scenario, got {sub}")
             sub._prepare()
             sub._start()
         self._subScenarios = list(subs)
         while True:
             newSubs = []
             for sub in self._subScenarios:
                 terminationReason = sub._step()
                 if isinstance(terminationReason, EndSimulationAction):
                     yield terminationReason
+                    assert False, self  # should never get here since simulation ends
                 elif terminationReason is None:
                     newSubs.append(sub)
             self._subScenarios = newSubs
             if not newSubs:
                 return
             yield None
+            # Check if any sub-scenarios stopped during action execution
+            self._subScenarios = [sub for sub in self._subScenarios if sub._isRunning]
 
     def _evaluateRecordedExprs(self, ty):
         if ty is RequirementType.record:
-            place = '_recordedExprs'
+            place = "_recordedExprs"
         elif ty is RequirementType.recordInitial:
-            place = '_recordedInitialExprs'
+            place = "_recordedInitialExprs"
         elif ty is RequirementType.recordFinal:
-            place = '_recordedFinalExprs'
+            place = "_recordedFinalExprs"
         else:
-            assert False, 'invalid record type requested'
+            assert False, "invalid record type requested"
         return self._evaluateRecordedExprsAt(place)
 
     def _evaluateRecordedExprsAt(self, place):
         values = {}
         for rec in getattr(self, place):
-            values[rec.name] = rec.value()
+            values[rec.name] = rec.evaluate()
         for sub in self._subScenarios:
             subvals = sub._evaluateRecordedExprsAt(place)
             values.update(subvals)
         return values
 
     def _runMonitors(self):
         terminationReason = None
+        endScenario = None
         for monitor in self._monitors:
             action = monitor._step()
+            # do not exit early, since subsequent monitors could reject the simulation
             if isinstance(action, EndSimulationAction):
                 terminationReason = action
-                # do not exit early, since subsequent monitors could reject the simulation
+            elif isinstance(action, EndScenarioAction):
+                assert action.scenario is None
+                endScenario = action
         for sub in self._subScenarios:
             subreason = sub._runMonitors()
             if subreason is not None:
                 terminationReason = subreason
-        return terminationReason
+        if endScenario:
+            self._stop(endScenario)
+        return terminationReason or endScenario
 
     def _checkSimulationTerminationConditions(self):
         for req in self._terminateSimulationConditions:
-            if req.isTrue():
+            if req.isTrue().is_truthy:
                 return req
         return None
 
     @property
     def _allAgents(self):
         agents = list(self._agents)
         for sub in self._subScenarios:
             agents.extend(sub._allAgents)
         return agents
 
     def _inherit(self, other):
+        if not self._workspace:
+            self._workspace = other._workspace
+        self._instances.extend(other._instances)
         self._objects.extend(other._objects)
         self._agents.extend(other._agents)
         self._globalParameters.update(other._globalParameters)
         self._externalParameters.extend(other._externalParameters)
         self._requirements.extend(other._requirements)
         self._behaviors.extend(other._behaviors)
 
+    def _registerInstance(self, inst):
+        self._instances.append(inst)
+
     def _registerObject(self, obj):
+        self._registerInstance(obj)
         self._objects.append(obj)
-        if getattr(obj, 'behavior', None) is not None:
+        if getattr(obj, "behavior", None) is not None:
             self._agents.append(obj)
 
+        obj._parentScenario = weakref.ref(self)
+
     def _addRequirement(self, ty, reqID, req, line, name, prob):
         """Save a requirement defined at compile-time for later processing."""
         assert reqID not in self._pendingRequirements
         preq = PendingRequirement(ty, req, line, prob, name, self._ego)
         self._pendingRequirements[reqID] = preq
 
     def _addDynamicRequirement(self, ty, req, line, name):
         """Add a requirement defined during a dynamic simulation."""
-        assert ty is not RequirementType.require
         dreq = DynamicRequirement(ty, req, line, name)
-        self._registerCompiledRequirement(dreq)
+        self._temporalRequirements.append(dreq)
+
+    def _addMonitor(self, monitor):
+        """Add a monitor during a dynamic simulation."""
+        assert isinstance(monitor, Monitor)
+        self._monitors.append(monitor)
+        if self._isRunning:
+            monitor._start()
 
     def _compileRequirements(self):
         namespace = self._dummyNamespace if self._dummyNamespace else self.__dict__
         requirementSyntax = self._requirementSyntax
         assert requirementSyntax is not None
         for reqID, requirement in self._pendingRequirements.items():
             syntax = requirementSyntax[reqID] if requirementSyntax else None
@@ -500,133 +597,175 @@
 
             self._registerCompiledRequirement(compiledReq)
             self._requirementDeps.update(compiledReq.dependencies)
 
     def _registerCompiledRequirement(self, req):
         if req.ty is RequirementType.require:
             place = self._requirements
-        elif req.ty is RequirementType.requireAlways:
-            place = self._alwaysRequirements
-        elif req.ty is RequirementType.requireEventually:
-            place = self._eventuallyRequirements
+        elif req.ty is RequirementType.monitor:
+            place = self._monitorRequirements
         elif req.ty is RequirementType.terminateWhen:
             place = self._terminationConditions
         elif req.ty is RequirementType.terminateSimulationWhen:
             place = self._terminateSimulationConditions
         elif req.ty is RequirementType.record:
             place = self._recordedExprs
         elif req.ty is RequirementType.recordInitial:
             place = self._recordedInitialExprs
         elif req.ty is RequirementType.recordFinal:
             place = self._recordedFinalExprs
         else:
-            raise RuntimeError(f'internal error: requirement {req} has unknown type!')
+            raise RuntimeError(f"internal error: requirement {req} has unknown type!")
         place.append(req)
 
     def _setTimeLimit(self, timeLimit, inSeconds=True):
         self._timeLimit = timeLimit
         self._timeLimitIsInSeconds = inSeconds
 
     def _override(self, obj, specifiers):
         oldVals = obj._override(specifiers)
         if obj not in self._overrides:
             self._overrides[obj] = oldVals
 
     def _toScenario(self, namespace):
         assert self._prepared
 
-        if self._ego is None and self._compose is None:
-            msg = 'did not specify ego object'
-            modScenarios = namespace['_scenarios']
-            if self._dummyNamespace and len(modScenarios) == 1:
-                if modScenarios[0]._requiresArguments():
-                    msg += ('\n(Note: this Scenic file contains a modular scenario, but it\n'
-                            'cannot be used as the top-level scenario since it requires\n'
-                            'arguments; so the whole file is being used as a top-level\n'
-                            'scenario and needs an ego object.)')
-                else:
-                    msg += ('\n(Note: this Scenic file contains a modular scenario, but also\n'
-                            'other code; so the whole file is being used as a top-level\n'
-                            'scenario and needs an ego object.)')
-            raise InvalidScenarioError(msg)
-
-        workspace = namespace['_workspace']
+        if not self._workspace:
+            self._workspace = Workspace()  # default empty workspace
+        astHash = namespace["_astHash"]
+        name = None if self._dummyNamespace else self.__class__.__name__
+        options = dataclasses.replace(namespace["_compileOptions"], scenario=name)
 
         from scenic.core.scenarios import Scenario
-        scenario = Scenario(workspace, self._simulatorFactory,
-                            self._objects, self._ego,
-                            self._globalParameters, self._externalParameters,
-                            self._requirements, self._requirementDeps,
-                            self._monitors, self._behaviorNamespaces,
-                            self)   # TODO unify these!
+
+        scenario = Scenario(
+            self._workspace,
+            self._simulatorFactory,
+            self._instances,
+            self._objects,
+            self._ego,
+            self._globalParameters,
+            self._externalParameters,
+            self._requirements,
+            self._requirementDeps,
+            self._monitorRequirements,
+            self._behaviorNamespaces,
+            self,
+            astHash,
+            options,
+        )  # TODO unify these!
         return scenario
 
     def __getattr__(self, name):
         if name in self._locals:
-            return DelayedArgument((), lambda context: getattr(self, name), _internal=True)
+            return DelayedArgument(
+                (), lambda context: getattr(self, name), _internal=True
+            )
         return object.__getattribute__(self, name)
 
     def __str__(self):
         if self._dummyNamespace:
-            return 'top-level scenario'
+            return "top-level scenario"
         else:
-            args = argsToString(itertools.chain(self._args, self._kwargs.items()))
-            return self.__class__.__name__ + args
+            args = argsToString(self._args, self._kwargs)
+            return f"{self.__class__.__name__}({args})"
+
 
 # Behaviors
 
+
 class Behavior(Invocable, Samplable):
     """Dynamic behaviors of agents.
 
     Behavior statements are translated into definitions of subclasses of this class.
     """
+
     def __init_subclass__(cls):
+        if "__signature__" in cls.__dict__:
+            # We're unpickling a behavior; skip this step.
+            return
+
         if cls.__module__ is not __name__:
-            veneer.currentScenario._behaviors.append(cls)
+            if veneer.currentScenario:
+                veneer.currentScenario._behaviors.append(cls)
+
+            target = cls.makeGenerator
+            target = functools.partial(target, 0, 0)  # account for Scenic-inserted args
+            cls.__signature__ = inspect.signature(target)
 
     def __init__(self, *args, **kwargs):
         args = tuple(toDistribution(arg) for arg in args)
-        kwargs = { name: toDistribution(arg) for name, arg in kwargs.items() }
+        kwargs = {name: toDistribution(arg) for name, arg in kwargs.items()}
 
         # Validate arguments to the behavior
         sig = inspect.signature(self.makeGenerator)
-        try:
-            sig.bind(None, *args, **kwargs)
-        except TypeError as e:
-            raise RuntimeParseError(str(e)) from e
+        sig.bind(None, *args, **kwargs)  # raises TypeError on incompatible arguments
         Samplable.__init__(self, itertools.chain(args, kwargs.values()))
         Invocable.__init__(self, *args, **kwargs)
 
         if not inspect.isgeneratorfunction(self.makeGenerator):
-            raise RuntimeParseError(f'{self} does not take any actions'
-                                    ' (perhaps you forgot to use "take" or "do"?)')
+            raise InvalidScenarioError(
+                f"{self} does not take any actions"
+                ' (perhaps you forgot to use "take" or "do"?)'
+            )
+
+    @classmethod
+    def _canCoerceType(cls, ty):
+        return issubclass(ty, cls) or ty in (type, type(None))
+
+    @classmethod
+    def _coerce(cls, thing):
+        if thing is None or isinstance(thing, cls):
+            return thing
+        elif issubclass(thing, cls):
+            return thing()
+        else:
+            raise CoercionFailure(f"expected type of behavior, got {thing}")
 
     def sampleGiven(self, value):
         args = (value[arg] for arg in self._args)
-        kwargs = { name: value[val] for name, val in self._kwargs.items() }
+        kwargs = {name: value[val] for name, val in self._kwargs.items()}
         return type(self)(*args, **kwargs)
 
+    def _assignTo(self, agent):
+        if self._agent and agent is self._agent._dynamicProxy:
+            # Assigned again (e.g. by override) to same agent; do nothing.
+            return
+        if self._isRunning:
+            raise InvalidScenarioError(
+                f"tried to reuse behavior object {self} already assigned to {self._agent}"
+            )
+        self._start(agent)
+
     def _start(self, agent):
         super()._start()
         self._agent = agent
         self._runningIterator = self.makeGenerator(agent, *self._args, **self._kwargs)
         self._checkAllPreconditions()
 
     def _step(self):
         super()._step()
         assert self._runningIterator
+
         def alarmHandler(signum, frame):
-            warnings.warn(f'the behavior {self} is taking a long time to take an action; '
-                          'maybe you have an infinite loop with no take/wait statements?',
-                          StuckBehaviorWarning)
-        with veneer.executeInBehavior(self), alarm(stuckBehaviorWarningTimeout, alarmHandler):
+            if sys.gettrace():
+                return  # skip the warning if we're in the debugger
+            warnings.warn(
+                f"the behavior {self} is taking a long time to take an action; "
+                "maybe you have an infinite loop with no take/wait statements?",
+                StuckBehaviorWarning,
+            )
+
+        with veneer.executeInBehavior(self), alarm(
+            stuckBehaviorWarningTimeout, alarmHandler
+        ):
             try:
                 actions = self._runningIterator.send(None)
             except StopIteration:
-                actions = ()    # behavior ended early
+                actions = ()  # behavior ended early
         return actions
 
     def _stop(self, reason=None):
         super()._stop(reason)
         self._agent = None
         self._runningIterator = None
 
@@ -634,112 +773,141 @@
     def _isFinished(self):
         return self._runningIterator is None
 
     def _invokeInner(self, agent, subs):
         assert len(subs) == 1
         sub = subs[0]
         if not isinstance(sub, Behavior):
-            raise RuntimeParseError(f'expected a behavior, got {sub}')
+            raise TypeError(f"expected a behavior, got {sub}")
         sub._start(agent)
         with veneer.executeInBehavior(sub):
             try:
                 yield from sub._runningIterator
             finally:
                 if sub._isRunning:
                     sub._stop()
 
-    def __str__(self):
-        args = argsToString(itertools.chain(self._args, self._kwargs.items()))
-        return self.__class__.__name__ + args
+    def __repr__(self):
+        items = itertools.chain(
+            (repr(arg) for arg in self._args),
+            (f"{key}={repr(val)}" for key, val in self._kwargs.items()),
+        )
+        allArgs = ", ".join(items)
+        return f"{self.__class__.__name__}({allArgs})"
+
 
-def makeTerminationAction(line):
+def _makeTerminationAction(agent, line):
+    assert not veneer.isActive()
+    if agent:
+        scenario = agent._parentScenario()
+        assert scenario is not None
+    else:
+        scenario = None
+    return EndScenarioAction(scenario, line)
+
+
+def _makeSimulationTerminationAction(line):
     assert not veneer.isActive()
     return EndSimulationAction(line)
 
+
 # Monitors
 
+
 class Monitor(Behavior):
     """Monitors for dynamic simulations.
 
     Monitor statements are translated into definitions of subclasses of this class.
     """
-    def __init_subclass__(cls):
-        super().__init_subclass__()
-        veneer.currentScenario._monitors.append(cls())
 
     def _start(self):
         return super()._start(None)
 
-monitorPrefix = '_Scenic_monitor_'
-def functionForMonitor(name):
-    return monitorPrefix + name
-def isAMonitorName(name):
-    return name.startswith(monitorPrefix)
-def monitorName(name):
-    return name[len(monitorPrefix):]
 
 # Guards
 
+
 class GuardViolation(Exception):
     """Abstract exception raised when a guard of a behavior is violated.
 
     This will never be raised directly; either of the subclasses `PreconditionViolation`
     or `InvariantViolation` will be used, as appropriate.
     """
-    violationType = 'guard'
+
+    violationType = "guard"
 
     def __init__(self, behavior, lineno):
         self.behaviorName = behavior.__class__.__name__
         self.lineno = lineno
 
     def __str__(self):
-        return f'violated {self.violationType} of {self.behaviorName} on line {self.lineno}'
+        return (
+            f"violated {self.violationType} of {self.behaviorName} on line {self.lineno}"
+        )
+
 
 class PreconditionViolation(GuardViolation):
-    """Raised when a precondition is violated when invoking a behavior."""
-    violationType = 'precondition'
+    """Exception raised when a precondition is violated
+
+    Raised when a precondition is violated when invoking a behavior
+    or when a precondition encounters a `RejectionException`, so that
+    rejections count as precondition violations.
+    """
+
+    violationType = "precondition"
+
 
 class InvariantViolation(GuardViolation):
-    """Raised when an invariant is violated when invoking/resuming a behavior."""
-    violationType = 'invariant'
+    """Exception raised when an invariant is violated
+
+    Raised when an invariant is violated when invoking/resuming a behavior
+    or when an invariant encounters a `RejectionException`, so that
+    rejections count as invariant violations.
+    """
+
+    violationType = "invariant"
+
 
 # Try-interrupt blocks
 
+
 def runTryInterrupt(behavior, agent, body, conditions, handlers):
     body = InterruptBlock(None, body)
     interrupts = [InterruptBlock(c, h) for c, h in zip(conditions, handlers)]
     while True:
         # find next block to run, if any
         block = body
         for interrupt in interrupts:
             if interrupt.isEnabled or interrupt.isRunning:
                 block = interrupt
                 break
         result, concluded = block.step(behavior, agent)
         if concluded:
             if result is BlockConclusion.FINISHED and block is not body:
-                continue    # interrupt handler finished
+                continue  # interrupt handler finished
             else:
-                return result   # entire try-interrupt statement will terminate
+                return result  # entire try-interrupt statement will terminate
         else:
             yield result
             behavior.checkInvariants(None, *behavior._args, **behavior._kwargs)
 
+
 @enum.unique
 class BlockConclusion(enum.Enum):
     FINISHED = enum.auto()
     ABORT = enum.auto()
     RETURN = enum.auto()
     BREAK = enum.auto()
     CONTINUE = enum.auto()
 
     def __call__(self, value):
         self.return_value = value
         return self
 
+
 class InterruptBlock:
     def __init__(self, condition, body):
         self.condition = condition
         self.body = body
         self.runningIterator = None
 
     @property
@@ -765,8 +933,9 @@
         try:
             result = self.runningIterator.send(None)
             return (result, False)
         except StopIteration as e:
             self.runningIterator = None
             return (e.value, True)
 
+
 import scenic.syntax.veneer as veneer
```

### Comparing `scenic-2.1.0b4/src/scenic/core/errors.py` & `scenic-3.0.0b2/src/scenic/core/errors.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,128 +1,177 @@
 """Common exceptions and error handling."""
 
 import importlib
 import itertools
 import pathlib
 import pdb
+import sys
 import traceback
 import types
-import sys
 import warnings
 
 import scenic
 import scenic.core
 import scenic.syntax
 
 ## Configuration
 
+
+def setDebuggingOptions(
+    *, verbosity=0, fullBacktrace=False, debugExceptions=False, debugRejections=False
+):
+    """Configure Scenic's debugging options.
+
+    Args:
+        verbosity (int): Verbosity level. Zero by default, although the command-line
+            interface uses 1 by default. See the :option:`--verbosity` option for the
+            allowed values.
+        fullBacktrace (bool): Whether to include Scenic's innards in backtraces
+            (like the :option:`-b` command-line option).
+        debugExceptions (bool): Whether to use `pdb` for post-mortem debugging of
+            uncaught exceptions (like the :option:`--pdb` option).
+        debugRejections (bool): Whether to enter `pdb` when a scene or simulation is
+            rejected (like the :option:`--pdb-on-reject` option).
+    """
+    global verbosityLevel, showInternalBacktrace, postMortemDebugging
+    global postMortemRejections
+    verbosityLevel = verbosity
+    postMortemDebugging = debugExceptions
+    postMortemRejections = debugRejections
+    if debugExceptions or debugRejections:
+        fullBacktrace = True  # partial backtraces would be confusing in the debugger
+    showInternalBacktrace = fullBacktrace
+
+
+#: Verbosity level. See :option:`--verbosity` for the allowed values.
+verbosityLevel = 0
+
 #: Whether or not to include Scenic's innards in backtraces.
 #:
 #: Set to True by default so that any errors during import of the scenic module
 #: will get full backtraces; the :mod:`scenic` module's *__init__.py* sets it to False.
 showInternalBacktrace = True
 
 #: Whether or not to do post-mortem debugging of uncaught exceptions.
 postMortemDebugging = False
 
 #: Whether or not to do "post-mortem" debugging of rejected scenes/simulations.
 postMortemRejections = False
 
+# fmt: off
 #: Folders elided from backtraces when :obj:`showInternalBacktrace` is false.
 #:
 #: :meta hide-value:
 hiddenFolders = [
     pathlib.Path(scenic.core.__file__).parent,      # scenic.core submodules
     pathlib.Path(scenic.syntax.__file__).parent,    # scenic.syntax submodules
     '<frozen importlib._bootstrap>',                # parts of importlib used internally
     pathlib.Path(importlib.__file__).parent,
 ]
+# fmt: on
 
 ## Exceptions
 
+
 class ScenicError(Exception):
     """An error produced during Scenic compilation, scene generation, or simulation."""
+
     pass
 
+
 class ScenicSyntaxError(ScenicError):
     """An error produced by attempting to parse an invalid Scenic program.
 
     This is intentionally not a subclass of SyntaxError so that pdb can be used
     for post-mortem debugging of the parser. Our custom excepthook below will
     arrange to still have it formatted as a SyntaxError, though.
     """
+
     pass
 
-class TokenParseError(ScenicSyntaxError):
-    """Parse error occurring during token translation."""
-    def __init__(self, tokenOrLine, filename, message):
-        self.filename = filename
-        self.msg = message
-        if hasattr(tokenOrLine, 'start'):
-            self.lineno, self.offset = tokenOrLine.start
-            self.end_lineno, self.end_offset = tokenOrLine.end
-            self.offset += 1
-            self.end_offset += 1
-            self.text = tokenOrLine.line
-        else:
-            self.lineno = self.end_lineno = tokenOrLine
-            self.text, self.offset, self.end_offset = getText(filename, tokenOrLine)
-        super().__init__(message)
 
-class PythonParseError(ScenicSyntaxError):
-    """Parse error occurring during Python parsing or compilation."""
+class ParseCompileError(ScenicSyntaxError):
+    """Error occurring during Scenic/Python parsing or compilation."""
+
     def __init__(self, exc):
         self.msg = exc.args[0]
         self.filename, self.lineno = exc.filename, exc.lineno
-        self.end_lineno = getattr(exc, 'end_lineno', None)  # added in Python 3.10
-        end_offset = getattr(exc, 'end_offset', None)       # ditto
-        self.text, self.offset, self.end_offset = getText(self.filename, self.lineno, exc.text,
-                                                          exc.offset, end_offset)
+        self.end_lineno = getattr(exc, "end_lineno", None)  # added in Python 3.10
+        end_offset = getattr(exc, "end_offset", None)  # ditto
+        self.text, self.offset, self.end_offset = getText(
+            self.filename, self.lineno, exc.text, exc.offset, end_offset
+        )
         super().__init__(self.msg)
         self.with_traceback(exc.__traceback__)
 
+
+class ScenicParseError(ParseCompileError):
+    """Error occuring during Scenic parsing or compilation."""
+
+    pass
+
+
+class PythonCompileError(ParseCompileError):
+    """Error occuring during Python compilation of translated Scenic code."""
+
+    pass
+
+
 class ASTParseError(ScenicSyntaxError):
     """Parse error occuring during modification of the Python AST."""
+
     def __init__(self, node, message, filename):
         self.msg = message
         self.lineno = node.lineno
-        self.end_lineno = getattr(node, 'end_lineno', None) # not always present
-        end_offset = getattr(node, 'end_col_offset', None)  # ditto
+        self.end_lineno = getattr(node, "end_lineno", None)  # not always present
+        end_offset = getattr(node, "end_col_offset", None)  # ditto
         self.filename = filename
-        self.text, self.offset, self.end_offset = getText(filename, node.lineno,
-                                                          offset=node.col_offset,
-                                                          end_offset=end_offset)
+        self.text, self.offset, self.end_offset = getText(
+            filename, node.lineno, offset=node.col_offset, end_offset=end_offset
+        )
         super().__init__(message)
 
-class RuntimeParseError(ScenicSyntaxError):
-    """A Scenic parse error generated during execution of the translated Python."""
-    def __init__(self, msg, loc=None):
-        super().__init__(msg)
-        self.loc = loc
 
 class InvalidScenarioError(ScenicError):
     """Error raised for syntactically-valid but otherwise problematic Scenic programs."""
+
     pass
 
+
 class InconsistentScenarioError(InvalidScenarioError):
     """Error for scenarios with inconsistent requirements."""
+
     def __init__(self, line, message):
         self.lineno = line
-        super().__init__('Inconsistent requirement on line ' + str(line) + ': ' + message)
+        super().__init__("Inconsistent requirement on line " + str(line) + ": " + message)
+
+
+class SpecifierError(ScenicError):
+    """Error for illegal uses of specifiers."""
+
+    pass
+
 
 ## Scenic backtraces
 
+
 def excepthook(ty, value, tb):
-    displayScenicException(value)
+    if sys.version_info >= (3, 11) and issubclass(ty, BaseExceptionGroup):
+        # Use the default mechanism since we don't handle ExceptionGroups
+        sys.__excepthook__(ty, value, tb)
+    else:
+        displayScenicException(value)
 
     if postMortemDebugging:
-        print('Uncaught exception. Entering post-mortem debugging')
+        print("Uncaught exception. Entering post-mortem debugging")
         import pdb
+
         pdb.post_mortem(tb)
 
+
 def displayScenicException(exc, seen=None):
     """Print a Scenic exception, cleaning up the traceback if desired.
 
     If ``showInternalBacktrace`` is False, this hides frames inside Scenic itself.
     """
     ty = type(exc)
     tb = exc.__traceback__
@@ -132,128 +181,148 @@
     if seen is None:
         seen = set()
     seen.add(id(exc))
     cause = exc.__cause__
     context = exc.__context__
     if cause is not None and id(cause) not in seen:
         displayScenicException(cause, seen)
-        print('\nThe above exception was the direct cause of the following exception:\n',
-              file=sys.stderr)
+        print(
+            "\nThe above exception was the direct cause of the following exception:\n",
+            file=sys.stderr,
+        )
     elif context is not None and not exc.__suppress_context__ and id(context) not in seen:
         displayScenicException(context, seen)
-        print('\nDuring handling of the above exception, another exception occurred:\n',
-              file=sys.stderr)
+        print(
+            "\nDuring handling of the above exception, another exception occurred:\n",
+            file=sys.stderr,
+        )
 
     if showInternalBacktrace:
-        strings = ['Traceback (most recent call last):\n']
+        strings = ["Traceback (most recent call last):\n"]
     else:
-        strings = ['Traceback (most recent call last; use -b to show Scenic internals):\n']
+        strings = [
+            "Traceback (most recent call last; use -b to show Scenic internals):\n"
+        ]
 
     # Work out how to present the exception type
-    pseudoSyntaxError = (issubclass(ty, ScenicSyntaxError)
-                         and not issubclass(ty, RuntimeParseError))
+    pseudoSyntaxError = issubclass(ty, ScenicSyntaxError)
     if issubclass(ty, ScenicError):
         if issubclass(ty, ScenicSyntaxError) and not showInternalBacktrace:
-            name = 'ScenicSyntaxError'
+            name = "ScenicSyntaxError"
         else:
             name = ty.__name__
         if pseudoSyntaxError:
             # hack to get format_exception_only to format this like a bona fide SyntaxError
             bases = (SyntaxError,)
         else:
             bases = ty.__bases__
         formatTy = type(name, bases, {})
         if not showInternalBacktrace:
-            formatTy.__module__ = '__main__'    # hide qualified name of the exception
+            formatTy.__module__ = "__main__"  # hide qualified name of the exception
     else:
         formatTy = ty
 
     if issubclass(ty, SyntaxError) or (pseudoSyntaxError and not showInternalBacktrace):
-        pass    # no backtrace for these types of errors
-    elif issubclass(ty, RuntimeParseError) and exc.loc and not showInternalBacktrace:
-        strings.extend(traceback.format_list([exc.loc]))
+        pass  # no backtrace for these types of errors
+    elif loc := getattr(exc, "_scenic_location", None):
+        strings.extend(traceback.format_list([loc]))
     else:
         summary = traceback.extract_tb(tb)
         if showInternalBacktrace:
             filtered = summary
         else:
             filtered = []
             skip = False
             for frame in summary:
                 if skip:
                     skip = False
                     continue
-                if frame.name == 'callBeginningScenicTrace':
+                if frame.name == "callBeginningScenicTrace":
                     filtered = []
                     skip = True
                 elif includeFrame(frame):
                     filtered.append(frame)
         if filtered:
             strings.extend(traceback.format_list(filtered))
         else:
-            strings.append('  <Scenic internals>\n')
+            strings.append("  <Scenic internals>\n")
     # Note: we can't directly call traceback.format_exception_only any more,
     # since as of Python 3.10 it ignores the exception class passed in and
     # uses type(exc) instead, foiling our formatTy hack.
     tbe = traceback.TracebackException(formatTy, exc, None)
     strings.extend(tbe.format_exception_only())
-    message = ''.join(strings)
-    print(message, end='', file=sys.stderr)
+    message = "".join(strings)
+    print(message, end="", file=sys.stderr)
+
 
 def includeFrame(frame):
     if frame.filename in hiddenFolders:
         return False
     parents = pathlib.Path(frame.filename).parents
     return not any(folder in parents for folder in hiddenFolders)
 
-if sys.excepthook is not sys.__excepthook__:
-    warnings.warn('unable to install sys.excepthook to format Scenic backtraces')
+
+# Install our excepthook if nobody else has already installed one;
+# we specially allow overwriting excepthooks from the following modules,
+# which are known to not cause problems:
+#   - exceptiongroup (PEP 654 backport for pre-3.11)
+if sys.excepthook is not sys.__excepthook__ and not sys.excepthook.__module__.startswith(
+    "exceptiongroup"
+):
+    warnings.warn("unable to install sys.excepthook to format Scenic backtraces")
 else:
     sys.excepthook = excepthook
 
+
 def callBeginningScenicTrace(func):
     """Call the given function, starting the Scenic backtrace at that point.
 
     This function is just a convenience to make Scenic backtraces cleaner when
     running Scenic programs from the command line.
     """
     return func()
 
+
 def saveErrorLocation():
     stack = traceback.extract_stack()
     for frame in reversed(stack):
         if includeFrame(frame):
             return frame
     return None
 
+
 ## Utilities
 
+
 def optionallyDebugRejection(exc=None):
     if not postMortemRejections:
         return
-    print('Scene/simulation rejected. Entering debugger...')
+    print("Scene/simulation rejected. Entering debugger...")
     if exc:
         pdb.post_mortem(exc.__traceback__)
     else:
         debugger = pdb.Pdb()
-        debugger.set_trace(sys._getframe().f_back)   # TODO more portable way to do this?
+        debugger.set_trace(sys._getframe().f_back)  # TODO more portable way to do this?
+
 
-def getText(filename, lineno, line='', offset=0, end_offset=None):
+def getText(filename, lineno, line="", offset=0, end_offset=None):
     """Attempt to recover the text of an error from the original Scenic file."""
+    if not filename or filename in {"<stream>", "<string>", "<unknown>"}:
+        return line, offset, end_offset  # don't bother with the filesystem
     try:
-        with open(filename, 'r') as f:
-            line = list(itertools.islice(f, lineno-1, lineno))
-        line = line[0] if line else ''
+        with open(filename, "r") as f:
+            line = list(itertools.islice(f, lineno - 1, lineno))
+        line = line[0] if line else ""
         # TODO improve reconstruction of error position?
         # (see TracebackException._format_syntax_error for spaces calculation below)
-        rline = line.rstrip('\n')
-        lline = rline.lstrip(' \n\f')
+        rline = line.rstrip("\n")
+        lline = rline.lstrip(" \n\f")
         spaces = len(rline) - len(lline)
         if end_offset is not None:
-            adj_end_offset = min(end_offset, len(line)+1)
-            offset = max(spaces+1, adj_end_offset - (end_offset - offset))
+            adj_end_offset = min(end_offset, len(line) + 1)
+            offset = max(spaces + 1, adj_end_offset - (end_offset - offset))
             end_offset = adj_end_offset
         else:
             offset = min(offset, len(line))
-    except FileNotFoundError:
+    except OSError:
         pass
     return line, offset, end_offset
```

### Comparing `scenic-2.1.0b4/src/scenic/core/external_params.py` & `scenic-3.0.0b2/src/scenic/core/external_params.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,84 +6,84 @@
 External samplers provide a mechanism to use different types of sampling
 techniques, like optimization or quasi-random sampling, from within a Scenic
 program. Ordinary random values in Scenic are instances of `Distribution`;
 this module defines a special subclass, `ExternalParameter`, representing a
 value which is sampled externally. Scenic programs with external parameters
 are handled as follows:
 
-	1. During compilation, all instances of `ExternalParameter` are gathered
-	   together and given to the `ExternalSampler.forParameters` function;
-	   this function creates an appropriate `ExternalSampler`,
-	   whose configuration can be controlled using :term:`global parameters`
-	   (see the function documentation for details).
-
-	2. When sampling a scene, before sampling any other distributions the
-	   :obj:`~ExternalSampler.sample` method of the `ExternalSampler` is
-	   called to sample all the external parameters. For active samplers, this
-	   method passes along the ``feedback`` value given to `Scenario.generate`,
-	   if any.
-
-	3. Once the external parameters have values, the program is equivalent to
-	   one without external parameters, and sampling proceeds as usual. As for
-	   every instance of `Distribution`, the external parameters will have
-	   their :obj:`~Samplable.sampleGiven` method called once all their
-	   dependencies have been sampled; by default this method just returns the
-	   value sampled for this parameter in step (2).
+    1. During compilation, all instances of `ExternalParameter` are gathered
+       together and given to the `ExternalSampler.forParameters` function;
+       this function creates an appropriate `ExternalSampler`,
+       whose configuration can be controlled using :term:`global parameters`
+       (see the function documentation for details).
+
+    2. When sampling a scene, before sampling any other distributions the
+       :obj:`~ExternalSampler.sample` method of the `ExternalSampler` is
+       called to sample all the external parameters. For active samplers, this
+       method passes along the ``feedback`` value given to `Scenario.generate`,
+       if any.
+
+    3. Once the external parameters have values, the program is equivalent to
+       one without external parameters, and sampling proceeds as usual. As for
+       every instance of `Distribution`, the external parameters will have
+       their :obj:`~Samplable.sampleGiven` method called once all their
+       dependencies have been sampled; by default this method just returns the
+       value sampled for this parameter in step (2).
 
 .. note::
 
-	Note that while external parameters, like all instances of `Distribution`,
-	are allowed to have dependencies, they are an exception to the usual rule
-	that dependencies are always sampled before dependents, because the
-	`ExternalSampler.sample` method is called before any other sampling.
-	However, as explained above, the :obj:`~Samplable.sampleGiven` method is
-	called in the proper order and external samplers which need to do sampling
-	based on the values of other distributions can be invoked from it. The
-	two-step mechanism with `ExternalSampler.sample` is provided for samplers
-	which sample the whole space of external parameters at once (e.g. the
-	VerifAI samplers).
+    Note that while external parameters, like all instances of `Distribution`,
+    are allowed to have dependencies, they are an exception to the usual rule
+    that dependencies are always sampled before dependents, because the
+    `ExternalSampler.sample` method is called before any other sampling.
+    However, as explained above, the :obj:`~Samplable.sampleGiven` method is
+    called in the proper order and external samplers which need to do sampling
+    based on the values of other distributions can be invoked from it. The
+    two-step mechanism with `ExternalSampler.sample` is provided for samplers
+    which sample the whole space of external parameters at once (e.g. the
+    VerifAI samplers).
 
 Samplers from VerifAI
 =====================
 
 The external sampling mechanism is designed to be extensible. The only built-in
 `ExternalSampler` is the `VerifaiSampler`, which provides access to the
 samplers in the `VerifAI`_ toolkit (which in turn can use Scenic as a modeling
 language).
 
 The `VerifaiSampler` supports several types of external parameters corresponding
 to the primitive distributions: `VerifaiRange` and `VerifaiDiscreteRange` for
 continuous and discrete intervals, and `VerifaiOptions` for discrete sets.
 For example, suppose we write::
 
-	ego = Object at (VerifaiRange(5, 15), 0)
+    ego = new Object at (VerifaiRange(5, 15), 0)
 
-This is equivalent to the ordinary Scenic line :samp:`ego = Object at (Range(5, 15), 0)`,
+This is equivalent to the ordinary Scenic line :scenic:`ego = new Object at (Range(5, 15), 0)`,
 except that the X coordinate of the ego is sampled by VerifAI within the range
 (5, 15) instead of being uniformly distributed over it. By default the
 `VerifaiSampler` uses VerifAI's `Halton`_ sampler, so the range will still be
 covered uniformly but more systematically. If we want to use a different sampler,
 we can set the ``verifaiSamplerType`` global parameter::
 
-	param verifaiSamplerType = 'ce'
-	ego = Object at (VerifaiRange(5, 15), 0)
+    param verifaiSamplerType = 'ce'
+    ego = new Object at (VerifaiRange(5, 15), 0)
 
 Now the X coordinate will be sampled using VerifAI's `cross-entropy`_ sampler.
 If we pass a feedback value to `Scenario.generate` which scores the previous
 scene, then the coordinate will not be sampled uniformly but rather converge to
 a distribution concentrated on values minimizing the score. Active samplers like
 cross-entropy can be used for falsification in this way, driving a system toward
 parts of the parameter space where a specification is violated.
 
 The cross-entropy sampler in VerifAI can be started from a non-uniform prior.
 Scenic provides a convenient way to define this prior using the ordinary syntax
 for distributions::
 
-	param verifaiSamplerType = 'ce'
-	ego = Object at (VerifaiParameter.withPrior(Normal(10, 3)), 0)
+    param verifaiSamplerType = 'ce'
+    ego = new Object at (VerifaiParameter.withPrior(Normal(10, 3)), 0)
 
 Now cross-entropy sampling will start from a normal distribution with mean 10
 and standard deviation 3. Priors are restricted to primitive distributions and
 in general may be approximated so that VerifAI can handle them -- see
 `VerifaiParameter.withPrior` for details.
 
 For more information on how to customize the sampler, see `VerifaiSampler`.
@@ -98,244 +98,277 @@
 
 from dotmap import DotMap
 import numpy
 
 from scenic.core.distributions import Distribution, Options
 from scenic.core.errors import InvalidScenarioError
 
+
 class ExternalSampler:
-	"""Abstract class for objects called to sample values for each external parameter.
+    """Abstract class for objects called to sample values for each external parameter.
+
+    The initializer for this class takes the same arguments as the factory function
+    `forParameters` below.
 
-	The initializer for this class takes the same arguments as the factory function
-	`forParameters` below.
+    Attributes:
+        rejectionFeedback: Value passed to the `sample` method when the last sample was rejected.
+          This value can be chosen by a Scenic scenario using the global parameter
+          ``externalSamplerRejectionFeedback``.
+    """
+
+    def __init__(self, params, globalParams):
+        # feedback value passed to external sampler when the last scene was rejected
+        self.rejectionFeedback = globalParams.get("externalSamplerRejectionFeedback")
+
+    @staticmethod
+    def forParameters(params, globalParams):
+        """Create an `ExternalSampler` given the sets of external and global parameters.
+
+        The scenario may explicitly select an external sampler by assigning the
+        :term:`global parameter` ``externalSampler`` to a subclass of `ExternalSampler`.
+        Otherwise, a `VerifaiSampler` is used by default.
+
+        Args:
+            params (tuple): Tuple listing each `ExternalParameter`.
+            globalParams (dict): Dictionary of global parameters for the `Scenario`, made
+              available here to support sampler customization through setting parameters.
+              Note that the values of these parameters may be instances of `Distribution`!
+
+        Returns:
+            An `ExternalSampler` configured for the given parameters.
+        """
+        if len(params) > 0:
+            externalSampler = globalParams.get("externalSampler", VerifaiSampler)
+            if not issubclass(externalSampler, ExternalSampler):
+                raise InvalidScenarioError(
+                    f"externalSampler type {externalSampler}"
+                    " not subclass of ExternalSampler"
+                )
+            return externalSampler(params, globalParams)
+        else:
+            return None
+
+    def sample(self, feedback):
+        """Sample values for all the external parameters.
+
+        Args:
+            feedback: Feedback from the last sample (for active samplers).
+        """
+        self.cachedSample = self.nextSample(feedback)
+
+    def nextSample(self, feedback):
+        """Actually do the sampling. Implemented by subclasses."""
+        raise NotImplementedError
+
+    def valueFor(self, param):
+        """Return the sampled value for a parameter. Implemented by subclasses."""
+        raise NotImplementedError
 
-	Attributes:
-		rejectionFeedback: Value passed to the `sample` method when the last sample was rejected.
-		  This value can be chosen by a Scenic scenario using the global parameter
-		  ``externalSamplerRejectionFeedback``.
-	"""
-	def __init__(self, params, globalParams):
-		# feedback value passed to external sampler when the last scene was rejected
-		self.rejectionFeedback = globalParams.get('externalSamplerRejectionFeedback')
-
-	@staticmethod
-	def forParameters(params, globalParams):
-		"""Create an `ExternalSampler` given the sets of external and global parameters.
-
-		The scenario may explicitly select an external sampler by assigning the
-		:term:`global parameter` ``externalSampler`` to a subclass of `ExternalSampler`.
-		Otherwise, a `VerifaiSampler` is used by default.
-
-		Args:
-			params (tuple): Tuple listing each `ExternalParameter`.
-			globalParams (dict): Dictionary of global parameters for the `Scenario`, made
-			  available here to support sampler customization through setting parameters.
-			  Note that the values of these parameters may be instances of `Distribution`!
-
-		Returns:
-			An `ExternalSampler` configured for the given parameters.
-		"""
-		if len(params) > 0:
-			externalSampler = globalParams.get('externalSampler', VerifaiSampler)
-			if not issubclass(externalSampler, ExternalSampler):
-				raise InvalidScenarioError(f'externalSampler type {externalSampler}'
-				                           ' not subclass of ExternalSampler')
-			return externalSampler(params, globalParams)
-		else:
-			return None
-
-	def sample(self, feedback):
-		"""Sample values for all the external parameters.
-
-		Args:
-			feedback: Feedback from the last sample (for active samplers).
-		"""
-		self.cachedSample = self.nextSample(feedback)
-
-	def nextSample(self, feedback):
-		"""Actually do the sampling. Implemented by subclasses."""
-		raise NotImplementedError
-
-	def valueFor(self, param):
-		"""Return the sampled value for a parameter. Implemented by subclasses."""
-		raise NotImplementedError
 
 class VerifaiSampler(ExternalSampler):
-	"""An external sampler exposing the samplers in the VerifAI toolkit.
+    """An external sampler exposing the samplers in the VerifAI toolkit.
+
+    The sampler can be configured using the following Scenic :term:`global parameters`:
 
-	The sampler can be configured using the following Scenic :term:`global parameters`:
+        * ``verifaiSamplerType`` -- sampler type (see the ``verifai.server.choose_sampler``
+          function); the default is ``'halton'``
+        * ``verifaiSamplerParams`` -- ``DotMap`` of options passed to the sampler
+
+    The `VerifaiSampler` supports external parameters which are instances of `VerifaiParameter`.
+    """
+
+    def __init__(self, params, globalParams):
+        super().__init__(params, globalParams)
+        import verifai.features
+        import verifai.server
+
+        # construct FeatureSpace
+        usingProbs = False
+        self.params = tuple(params)
+        for index, param in enumerate(self.params):
+            if not isinstance(param, VerifaiParameter):
+                raise RuntimeError(
+                    f"VerifaiSampler given parameter of wrong type: {param}"
+                )
+            param.sampler = self
+            param.index = index
+            if param.probs is not None:
+                usingProbs = True
+        space = verifai.features.FeatureSpace(
+            {
+                f"param{index}": verifai.features.Feature(param.domain)
+                for index, param in enumerate(self.params)
+            }
+        )
+
+        # set up VerifAI sampler
+        samplerType = globalParams.get("verifaiSamplerType", "halton")
+        samplerParams = globalParams.get("verifaiSamplerParams", None)
+        if usingProbs and samplerType == "ce":
+            if samplerParams is None:
+                samplerParams = DotMap()
+            if "cont" in samplerParams or "disc" in samplerParams:
+                raise RuntimeError(
+                    "CE distributions specified in both VerifaiParameters"
+                    "and verifaiSamplerParams"
+                )
+            cont_buckets = []
+            cont_dists = []
+            disc_dists = []
+            for param in self.params:
+                if isinstance(param, VerifaiRange):
+                    if param.probs is None:
+                        buckets = 5
+                        dist = numpy.ones(buckets) / buckets
+                    else:
+                        dist = numpy.array(param.probs)
+                        buckets = len(dist)
+                    cont_buckets.append(buckets)
+                    cont_dists.append(dist)
+                elif isinstance(param, VerifaiDiscreteRange):
+                    n = param.high - param.low + 1
+                    dist = (
+                        numpy.ones(n) / n
+                        if param.probs is None
+                        else numpy.array(param.probs)
+                    )
+                    disc_dists.append(dist)
+                else:
+                    raise RuntimeError(f"Parameter {param} not supported by CE sampler")
+            samplerParams.cont.buckets = cont_buckets
+            samplerParams.cont.dist = numpy.array(cont_dists)
+            samplerParams.disc.dist = numpy.array(disc_dists)
+        data = verifai.server.choose_sampler(
+            space, samplerType, sampler_params=samplerParams
+        )
+        if not data:
+            raise RuntimeError(f'Unknown VerifAI sampler type "{samplerType}"')
+        self.sampler = data[1]
+
+        # default rejection feedback is positive so cross-entropy sampler won't update;
+        # for other active samplers an appropriate value should be set manually
+        if self.rejectionFeedback is None:
+            self.rejectionFeedback = 1
+        self.cachedSample = None
+
+    def nextSample(self, feedback):
+        return self.sampler.nextSample(feedback)
 
-		* ``verifaiSamplerType`` -- sampler type (see the ``verifai.server.choose_sampler``
-		  function); the default is ``'halton'``
-		* ``verifaiSamplerParams`` -- ``DotMap`` of options passed to the sampler
-
-	The `VerifaiSampler` supports external parameters which are instances of `VerifaiParameter`.
-	"""
-
-	def __init__(self, params, globalParams):
-		super().__init__(params, globalParams)
-		import verifai.features
-		import verifai.server
-
-		# construct FeatureSpace
-		usingProbs = False
-		self.params = tuple(params)
-		for index, param in enumerate(self.params):
-			if not isinstance(param, VerifaiParameter):
-				raise RuntimeError(f'VerifaiSampler given parameter of wrong type: {param}')
-			param.sampler = self
-			param.index = index
-			if param.probs is not None:
-				usingProbs = True
-		space = verifai.features.FeatureSpace({
-		    f'param{index}': verifai.features.Feature(param.domain)
-		    for index, param in enumerate(self.params)
-		})
-
-		# set up VerifAI sampler
-		samplerType = globalParams.get('verifaiSamplerType', 'halton')
-		samplerParams = globalParams.get('verifaiSamplerParams', None)
-		if usingProbs and samplerType == 'ce':
-			if samplerParams is None:
-				samplerParams = DotMap()
-			if 'cont' in samplerParams or 'disc' in samplerParams:
-				raise RuntimeError('CE distributions specified in both VerifaiParameters'
-				                   'and verifaiSamplerParams')
-			cont_buckets = []
-			cont_dists = []
-			disc_dists = []
-			for param in self.params:
-				if isinstance(param, VerifaiRange):
-					if param.probs is None:
-						buckets = 5
-						dist = numpy.ones(buckets) / buckets
-					else:
-						dist = numpy.array(param.probs)
-						buckets = len(dist)
-					cont_buckets.append(buckets)
-					cont_dists.append(dist)
-				elif isinstance(param, VerifaiDiscreteRange):
-					n = param.high - param.low + 1
-					dist = numpy.ones(n)/n if param.probs is None else numpy.array(param.probs)
-					disc_dists.append(dist)
-				else:
-					raise RuntimeError(f'Parameter {param} not supported by CE sampler')
-			samplerParams.cont.buckets = cont_buckets
-			samplerParams.cont.dist = numpy.array(cont_dists)
-			samplerParams.disc.dist = numpy.array(disc_dists)
-		data = verifai.server.choose_sampler(space, samplerType,
-		                                     sampler_params=samplerParams)
-		if not data:
-			raise RuntimeError(f'Unknown VerifAI sampler type "{samplerType}"')
-		self.sampler = data[1]
-
-		# default rejection feedback is positive so cross-entropy sampler won't update;
-		# for other active samplers an appropriate value should be set manually
-		if self.rejectionFeedback is None:
-			self.rejectionFeedback = 1
-		self.cachedSample = None
-
-	def nextSample(self, feedback):
-		return self.sampler.nextSample(feedback)
+    def update(self, sample, info, rho):
+        self.sampler.update(sample, info, rho)
 
-	def update(self, sample, info, rho):
-		self.sampler.update(sample, info, rho)
+    def getSample(self):
+        return self.sampler.getSample()
 
-	def getSample(self):
-		return self.sampler.getSample()
+    def valueFor(self, param):
+        return self.cachedSample[param.index]
 
-	def valueFor(self, param):
-		return self.cachedSample[param.index]
 
 class ExternalParameter(Distribution):
-	"""A value determined by external code rather than Scenic's internal sampler."""
-	def __init__(self):
-		super().__init__()
-		self.sampler = None
-		import scenic.syntax.veneer as veneer	# TODO improve?
-		veneer.registerExternalParameter(self)
-
-	def sampleGiven(self, value):
-		"""Specialization of  `Samplable.sampleGiven` for external parameters.
-
-		By default, this method simply looks up the value previously sampled by
-		`ExternalSampler.sample`.
-		"""
-		assert self.sampler is not None
-		return self.sampler.valueFor(self)
+    """A value determined by external code rather than Scenic's internal sampler."""
+
+    def __init__(self):
+        super().__init__()
+        self.sampler = None
+        import scenic.syntax.veneer as veneer  # TODO improve?
+
+        veneer.registerExternalParameter(self)
+
+    def sampleGiven(self, value):
+        """Specialization of  `Samplable.sampleGiven` for external parameters.
+
+        By default, this method simply looks up the value previously sampled by
+        `ExternalSampler.sample`.
+        """
+        assert self.sampler is not None
+        return self.sampler.valueFor(self)
+
 
 class VerifaiParameter(ExternalParameter):
-	"""An external parameter sampled using one of VerifAI's samplers."""
+    """An external parameter sampled using one of VerifAI's samplers."""
+
+    def __init__(self, domain):
+        super().__init__()
+        self.domain = domain
+
+    @staticmethod
+    def withPrior(dist, buckets=None):
+        """Creates a `VerifaiParameter` using the given distribution as a prior.
+
+        Since the VerifAI cross-entropy sampler currently only supports piecewise-constant
+        distributions, if the prior is not of that form it may be approximated. For most
+        built-in distributions, the approximation is exact: for a particular distribution,
+        check its `bucket` method.
+        """
+        if not dist.isPrimitive:
+            raise RuntimeError(
+                "VerifaiParameter.withPrior called on "
+                f"non-primitive distribution {dist}"
+            )
+        bucketed = dist.bucket(buckets=buckets)
+        return VerifaiOptions(
+            bucketed.optWeights if bucketed.optWeights else bucketed.options
+        )
 
-	def __init__(self, domain):
-		super().__init__()
-		self.domain = domain
-
-	@staticmethod
-	def withPrior(dist, buckets=None):
-		"""Creates a `VerifaiParameter` using the given distribution as a prior.
-
-		Since the VerifAI cross-entropy sampler currently only supports piecewise-constant
-		distributions, if the prior is not of that form it may be approximated. For most
-		built-in distributions, the approximation is exact: for a particular distribution,
-		check its `bucket` method.
-		"""
-		if not dist.isPrimitive:
-			raise RuntimeError('VerifaiParameter.withPrior called on '
-			                   f'non-primitive distribution {dist}')
-		bucketed = dist.bucket(buckets=buckets)
-		return VerifaiOptions(bucketed.optWeights if bucketed.optWeights else bucketed.options)
 
 class VerifaiRange(VerifaiParameter):
-	"""A :obj:`~scenic.core.distributions.Range` (real interval) sampled by VerifAI."""
+    """A :obj:`~scenic.core.distributions.Range` (real interval) sampled by VerifAI."""
+
+    _defaultValueType = float
+
+    def __init__(self, low, high, buckets=None, weights=None):
+        import verifai.features
 
-	_defaultValueType = float
+        super().__init__(verifai.features.Box([low, high]))
+        if weights is not None:
+            weights = tuple(weights)
+            if buckets is not None and len(weights) != buckets:
+                raise RuntimeError(
+                    f"VerifaiRange created with {len(weights)} weights "
+                    f"but {buckets} buckets"
+                )
+        elif buckets is not None:
+            weights = [1] * buckets
+        else:
+            self.probs = None
+            return
+        total = sum(weights)
+        self.probs = tuple(wt / total for wt in weights)
+
+    def sampleGiven(self, value):
+        value = super().sampleGiven(value)
+        assert len(value) == 1
+        return value[0]
 
-	def __init__(self, low, high, buckets=None, weights=None):
-		import verifai.features
-		super().__init__(verifai.features.Box([low, high]))
-		if weights is not None:
-			weights = tuple(weights)
-			if buckets is not None and len(weights) != buckets:
-				raise RuntimeError(f'VerifaiRange created with {len(weights)} weights '
-				                   f'but {buckets} buckets')
-		elif buckets is not None:
-			weights = [1] * buckets
-		else:
-			self.probs = None
-			return
-		total = sum(weights)
-		self.probs = tuple(wt/total for wt in weights)
-
-	def sampleGiven(self, value):
-		value = super().sampleGiven(value)
-		assert len(value) == 1
-		return value[0]
 
 class VerifaiDiscreteRange(VerifaiParameter):
-	"""A :obj:`~scenic.core.distributions.DiscreteRange` (integer interval) sampled by VerifAI."""
+    """A :obj:`~scenic.core.distributions.DiscreteRange` (integer interval) sampled by VerifAI."""
+
+    _defaultValueType = float
+
+    def __init__(self, low, high, weights=None):
+        import verifai.features
 
-	_defaultValueType = float
+        super().__init__(verifai.features.DiscreteBox([low, high]))
+        if weights is not None:
+            if len(weights) != (high - low + 1):
+                raise RuntimeError(
+                    f"VerifaiDiscreteRange created with {len(weights)} weights "
+                    f"for {high - low + 1} values"
+                )
+            total = sum(weights)
+            self.probs = tuple(wt / total for wt in weights)
+        else:
+            self.probs = None
+
+    def sampleGiven(self, value):
+        value = super().sampleGiven(value)
+        assert len(value) == 1
+        return value[0]
 
-	def __init__(self, low, high, weights=None):
-		import verifai.features
-		super().__init__(verifai.features.DiscreteBox([low, high]))
-		if weights is not None:
-			if len(weights) != (high - low + 1):
-				raise RuntimeError(f'VerifaiDiscreteRange created with {len(weights)} weights '
-				                   f'for {high - low + 1} values')
-			total = sum(weights)
-			self.probs = tuple(wt/total for wt in weights)
-		else:
-			self.probs = None
-
-	def sampleGiven(self, value):
-		value = super().sampleGiven(value)
-		assert len(value) == 1
-		return value[0]
 
 class VerifaiOptions(Options):
-	"""An :obj:`~scenic.core.distributions.Options` (discrete set) sampled by VerifAI."""
+    """An :obj:`~scenic.core.distributions.Options` (discrete set) sampled by VerifAI."""
 
-	@staticmethod
-	def makeSelector(n, weights):
-		return VerifaiDiscreteRange(0, n, weights)
+    @staticmethod
+    def makeSelector(n, weights):
+        return VerifaiDiscreteRange(0, n, weights)
```

### Comparing `scenic-2.1.0b4/src/scenic/core/pruning.py` & `scenic-3.0.0b2/src/scenic/core/pruning.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,141 +1,259 @@
 """Pruning parts of the sample space which violate requirements.
 
 The top-level function here, `prune`, is called as the very last step of scenario
 compilation (from `translator.constructScenarioFrom`).
 """
 
+import builtins
 import math
 import time
+
 import shapely.geometry
 import shapely.geos
 
-from scenic.core.distributions import (Samplable, MethodDistribution, OperatorDistribution,
-                                       needsSampling, supportInterval, underlyingFunction)
-from scenic.core.object_types import Point, Object
-from scenic.core.geometry import normalizeAngle, polygonUnion, plotPolygon
-from scenic.core.vectors import VectorField, PolygonalVectorField, VectorMethodDistribution
-from scenic.core.workspaces import Workspace
-from scenic.syntax.relations import RelativeHeadingRelation, DistanceRelation
+from scenic.core.distributions import (
+    AttributeDistribution,
+    FunctionDistribution,
+    MethodDistribution,
+    OperatorDistribution,
+    Samplable,
+    needsSampling,
+    supportInterval,
+    underlyingFunction,
+)
 from scenic.core.errors import InvalidScenarioError
+from scenic.core.geometry import hypot, normalizeAngle, plotPolygon, polygonUnion
+from scenic.core.object_types import Object, Point
 import scenic.core.regions as regions
+from scenic.core.regions import EmptyRegion, MeshSurfaceRegion, MeshVolumeRegion
+from scenic.core.type_support import TypecheckedDistribution
+from scenic.core.vectors import (
+    PolygonalVectorField,
+    VectorField,
+    VectorMethodDistribution,
+    VectorOperatorDistribution,
+)
+from scenic.core.workspaces import Workspace
+from scenic.syntax.relations import DistanceRelation, RelativeHeadingRelation
 
 ### Utilities
 
+
 def currentPropValue(obj, prop):
     """Get the current value of an object's property, taking into account prior pruning."""
     value = getattr(obj, prop)
     return value._conditioned if isinstance(value, Samplable) else value
 
+
 def isMethodCall(thing, method):
     """Match calls to a given method, taking into account distribution decorators."""
     if not isinstance(thing, (MethodDistribution, VectorMethodDistribution)):
         return False
     return thing.method is underlyingFunction(method)
 
+
+def isFunctionCall(thing, function):
+    """Match calls to a given function, taking into account distribution decorators."""
+    if not isinstance(thing, FunctionDistribution):
+        return False
+    return thing.function is underlyingFunction(function)
+
+
 def matchInRegion(position):
-    """Match uniform samples from a `Region`, returning the Region if any."""
+    """Match uniform samples from a `Region`
+
+    Returns the Region, if any, and a lower and upper bound
+    on the distance the object will be placed along with any
+    offset that should be added to the base.
+    """
+    # Case 1: Position is simply a point in a region
     if isinstance(position, regions.PointInRegionDistribution):
         reg = position.region
         if isinstance(reg, Workspace):
             reg = reg.region
-        return reg
-    return None
+        return reg, 0, 0, None
+
+    # Case 2: Position is a point in a region with a vector offset.
+    if isinstance(position, VectorOperatorDistribution) and position.operator in (
+        "__add__",
+        "__radd__",
+    ):
+        if isinstance(position.object, regions.PointInRegionDistribution):
+            reg = position.object.region
+            assert len(position.operands) == 1
+            offset = position.operands[0]
+            # TODO: Proper vector supportInterval calculations. Right now this gives us None
+            # if value is not exact
+            lower, upper = supportInterval(offset.norm())
+
+            return reg, lower, upper, offset
+
+    return None, 0, 0, None
+
 
 def matchPolygonalField(heading, position):
-    """Match headings defined by a `PolygonalVectorField` at the given position.
+    """Match orientation yaw defined by a `PolygonalVectorField` at the given position.
 
-    Matches headings exactly equal to a `PolygonalVectorField`, or offset by a
-    bounded disturbance. Returns a triple consisting of the matched field if
-    any, together with lower/upper bounds on the disturbance.
+    Matches the yaw attribute of orientations exactly equal to a `PolygonalVectorField`,
+    or offset by a bounded disturbance. Returns a triple consisting of the matched field
+    if any, together with lower/upper bounds on the disturbance.
     """
-    if (isMethodCall(heading, VectorField.__getitem__)
-        and isinstance(heading.object, PolygonalVectorField)
-        and heading.arguments == (position,)):
-        return heading.object, 0, 0
-    elif isinstance(heading, OperatorDistribution) and heading.operator in ('__add__', '__radd__'):
+    if isFunctionCall(heading, normalizeAngle):
+        assert len(heading.arguments) == 1
+        return matchPolygonalField(heading.arguments[0], position)
+
+    if (
+        isinstance(heading, TypecheckedDistribution)
+        and heading._valueType is builtins.float
+    ):
+        return matchPolygonalField(heading._dist, position)
+
+    if (
+        isinstance(heading, AttributeDistribution) and heading.attribute == "yaw"
+    ):  # TODO generalize to other 3D angles?
+        orientation = heading.object
+        if (
+            isMethodCall(orientation, VectorField.__getitem__)
+            and isinstance(orientation.object, PolygonalVectorField)
+            and orientation.arguments == (position,)
+        ):
+            return orientation.object, 0, 0
+
+    if isinstance(heading, OperatorDistribution) and heading.operator in (
+        "__add__",
+        "__radd__",
+    ):
         field, lower, upper = matchPolygonalField(heading.object, position)
         if field is not None:
             assert len(heading.operands) == 1
             offset = heading.operands[0]
             ol, oh = supportInterval(offset)
             if ol is not None and oh is not None:
                 return field, lower + ol, upper + oh
+
     return None, 0, 0
 
+
 ### Pruning procedures
 
+
 def prune(scenario, verbosity=1):
     """Prune a `Scenario`, removing infeasible parts of the space.
 
     This function directly modifies the Distributions used in the Scenario,
     but leaves the conditional distribution under the scenario's requirements
     unchanged. See `Samplable.conditionTo`.
 
     Currently, the following pruning techniques are applied in order:
 
         * Pruning based on containment (`pruneContainment`)
         * Pruning based on relative heading bounds (`pruneRelativeHeading`)
     """
     if verbosity >= 1:
-        print('  Pruning scenario...')
+        print("  Pruning scenario...")
         startTime = time.time()
 
     pruneContainment(scenario, verbosity)
     pruneRelativeHeading(scenario, verbosity)
 
     if verbosity >= 1:
         totalTime = time.time() - startTime
-        print(f'  Pruned scenario in {totalTime:.4g} seconds.')
+        print(f"  Pruned scenario in {totalTime:.4g} seconds.")
+
 
 ## Pruning based on containment
 
+
 def pruneContainment(scenario, verbosity):
     """Prune based on the requirement that individual Objects fit within their container.
 
-    Specifically, if O is positioned uniformly in region B and has container C, then we
-    can instead pick a position uniformly in their intersection. If we can also lower
-    bound the radius of O, then we can first erode C by that distance.
+    Specifically, if O is positioned uniformly (with a possible offset) in region B and
+    has container C, then we can instead pick a position uniformly in their intersection.
+    If we can also lower bound the radius of O, then we can first erode C by that distance
+    minus that maximum offset distance.
     """
     for obj in scenario.objects:
-        base = matchInRegion(obj.position)
-        if base is None:                    # match objects positioned uniformly in a Region
+        # Extract the base region and container region, while doing minor checks.
+        base, _, maxDistance, offset = matchInRegion(obj.position)
+
+        if base is None or needsSampling(base):
             continue
+
         if isinstance(base, regions.EmptyRegion):
-            raise InvalidScenarioError(f'Object {obj} placed in empty region')
-        basePoly = regions.toPolygon(base)
-        if basePoly is None:                # to prune, the Region must be polygonal
-            continue
-        if basePoly.is_empty:
-            raise InvalidScenarioError(f'Object {obj} placed in empty region')
+            raise InvalidScenarioError(f"Object {obj} placed in empty region")
+
         container = scenario.containerOfObject(obj)
-        containerPoly = regions.toPolygon(container)
-        if containerPoly is None:           # the object's container must also be polygonal
+
+        if container is None or needsSampling(container):
             continue
+
+        if isinstance(container, regions.EmptyRegion):
+            raise InvalidScenarioError(f"Object {obj} contained in empty region")
+
+        # Erode the container region if possible.
         minRadius, _ = supportInterval(obj.inradius)
-        if minRadius is not None:           # if we can lower bound the radius, erode the container
-            containerPoly = containerPoly.buffer(-minRadius)
-        elif base is container:
+
+        if (
+            hasattr(container, "buffer")
+            and maxDistance is not None
+            and minRadius is not None
+        ):
+            maxErosion = minRadius - maxDistance
+            if maxErosion > 0:
+                container = container.buffer(-maxErosion)
+
+        # Restrict the base region to the container, unless
+        # they're the same in which case we're done
+        if base is container:
             continue
-        newBasePoly = basePoly & containerPoly      # restrict the base Region to the container
-        if newBasePoly.is_empty:
-            raise InvalidScenarioError(f'Object {obj} does not fit in container')
+
+        newBase = base.intersect(container)
+        newBase.orientation = base.orientation
+
+        # Check if base was a volume and newBase is a surface,
+        # in which case the mesh operation might be undefined and we abort.
+        if isinstance(base, MeshVolumeRegion) and isinstance(newBase, MeshSurfaceRegion):
+            continue
+
+        if isinstance(newBase, EmptyRegion):
+            raise InvalidScenarioError(f"Object {obj} does not fit in container")
+
         if verbosity >= 1:
-            if basePoly.area > 0:
-                ratio = newBasePoly.area / basePoly.area
-            else:
-                ratio = newBasePoly.length / basePoly.length
-            percent = 100 * (1.0 - ratio)
-            print(f'    Region containment constraint pruned {percent:.1f}% of space.')
-        newBase = regions.regionFromShapelyObject(newBasePoly, orientation=base.orientation)
+            if (
+                base.dimensionality is None
+                or newBase.dimensionality is None
+                or base.dimensionality != newBase.dimensionality
+            ):
+                print(
+                    f"    Region containment constraint pruning attempted but could not compute percentage for {base} and {newBase}."
+                )
+            elif base.dimensionality == newBase.dimensionality:
+                ratio = newBase.size / base.size
+                percent = max(0, 100 * (1.0 - ratio))
+
+                if percent <= 0.001:
+                    # We didn't really prune anything, don't bother setting new position
+                    continue
+
+                print(
+                    f"    Region containment constraint pruned {percent:.1f}% of space."
+                )
+
         newPos = regions.Region.uniformPointIn(newBase)
+
+        if offset is not None:
+            newPos += offset
+
         obj.position.conditionTo(newPos)
 
+
 ## Pruning based on orientation
 
+
 def pruneRelativeHeading(scenario, verbosity):
     """Prune based on requirements bounding the relative heading of an Object.
 
     Specifically, if an object O is:
 
         * positioned uniformly within a polygonal region B;
         * aligned to a polygonal vector field F (up to a bounded offset);
@@ -146,75 +264,106 @@
         * at most some finite maximum distance from O;
         * required to have relative heading within a bounded offset of that of O;
 
     then we can instead position O uniformly in the subset of B intersecting the cells
     of F which satisfy the relative heading requirements w.r.t. some cell of F' which
     is within the distance bound.
     """
+    # TODO Add test for empty pruned polygon (Might cause crash?)
     # Check which objects are (approximately) aligned to polygonal vector fields
     fields = {}
     for obj in scenario.objects:
         field, offsetL, offsetR = matchPolygonalField(obj.heading, obj.position)
         if field is not None:
             fields[obj] = (field, offsetL, offsetR)
+
     # Check for relative heading relations among such objects
     for obj, (field, offsetL, offsetR) in fields.items():
-        position = currentPropValue(obj, 'position')
-        base = matchInRegion(position)
-        if base is None:        # obj must be positioned uniformly in a Region
+        position = currentPropValue(obj, "position")
+        base, _, _, offset = matchInRegion(position)
+
+        # obj must be positioned uniformly in a Region
+        if base is None or needsSampling(base):
             continue
+
+        if offset is not None:
+            continue
+
         basePoly = regions.toPolygon(base)
-        if basePoly is None:    # the Region must be polygonal
+        if basePoly is None:  # the Region must be polygonal
             continue
+
         newBasePoly = basePoly
         for rel in obj._relations:
             if isinstance(rel, RelativeHeadingRelation) and rel.target in fields:
                 tField, tOffsetL, tOffsetR = fields[rel.target]
                 maxDist = maxDistanceBetween(scenario, obj, rel.target)
-                if maxDist == float('inf'):     # the distance between the objects must be bounded
+                if maxDist == float("inf"):
+                    # the distance between the objects must be bounded
                     continue
-                feasible = feasibleRHPolygon(field, offsetL, offsetR,
-                                             tField, tOffsetL, tOffsetR,
-                                             rel.lower, rel.upper, maxDist)
-                if feasible is None:    # the RH bounds may be too weak to restrict the space
+                feasible = feasibleRHPolygon(
+                    field,
+                    offsetL,
+                    offsetR,
+                    tField,
+                    tOffsetL,
+                    tOffsetR,
+                    rel.lower,
+                    rel.upper,
+                    maxDist,
+                )
+                if feasible is None:
+                    # the RH bounds may be too weak to restrict the space
                     continue
                 try:
                     pruned = newBasePoly & feasible
-                except shapely.geos.TopologicalError:   # TODO how can we prevent these??
+                except shapely.geos.TopologicalError:  # TODO how can we prevent these??
                     pruned = newBasePoly & feasible.buffer(0.1, cap_style=2)
                 if verbosity >= 1:
                     percent = 100 * (1.0 - (pruned.area / newBasePoly.area))
-                    print(f'    Relative heading constraint pruned {percent:.1f}% of space.')
+                    print(
+                        f"    Relative heading constraint pruned {percent:.1f}% of space."
+                    )
                 newBasePoly = pruned
+
         if newBasePoly is not basePoly:
-            newBase = regions.PolygonalRegion(polygon=newBasePoly,
-                                              orientation=base.orientation)
+            newBase = regions.PolygonalRegion(
+                polygon=newBasePoly, orientation=base.orientation
+            )
             newPos = regions.Region.uniformPointIn(newBase)
             obj.position.conditionTo(newPos)
 
+
 def maxDistanceBetween(scenario, obj, target):
     """Upper bound the distance between the given Objects."""
-    # If one of the objects is the ego, use visibility requirements
+    # visDist is initialized to infinity. Then we can use
+    # various visibility constraints to upper bound it,
+    # keeping the tightest bound.
     ego = scenario.egoObject
+    visDist = float("inf")
+
     if obj is ego and target.requireVisible:
-        visDist = visibilityBound(ego, target)
-    elif target is ego and obj.requireVisible:
-        visDist = visibilityBound(ego, obj)
-    else:
-        visDist = float('inf')
+        visDist = min(visDist, visibilityBound(ego, target))
+    if target is ego and obj.requireVisible:
+        visDist = min(visDist, visibilityBound(ego, obj))
+    if obj._observingEntity is target:
+        visDist = min(visDist, visibilityBound(target, obj))
+    if target._observingEntity is obj:
+        visDist = min(visDist, visibilityBound(obj, target))
 
     # Check for any distance bounds implied by user-specified requirements
-    reqDist = float('inf')
+    reqDist = float("inf")
     for rel in obj._relations:
         if isinstance(rel, DistanceRelation) and rel.target is target:
             if rel.upper < reqDist:
                 reqDist = rel.upper
 
     return min(visDist, reqDist)
 
+
 def visibilityBound(obj, target):
     """Upper bound the distance from an Object to another it can see."""
     # Upper bound on visible distance is a sum of several terms:
     # 1. obj.visibleDistance
     _, maxVisibleDistance = supportInterval(obj.visibleDistance)
     if maxVisibleDistance is None:
         return None
@@ -227,45 +376,55 @@
     # 3. radius of target
     _, maxRadius = supportInterval(target.radius)
     if maxRadius is None:
         return None
     maxVisibleDistance += maxRadius
     return maxVisibleDistance
 
-def feasibleRHPolygon(field, offsetL, offsetR,
-                      tField, tOffsetL, tOffsetR,
-                      lowerBound, upperBound, maxDist):
+
+def feasibleRHPolygon(
+    field, offsetL, offsetR, tField, tOffsetL, tOffsetR, lowerBound, upperBound, maxDist
+):
     """Find where objects aligned to the given fields can satisfy the given RH bounds."""
-    if (offsetR - offsetL >= math.tau
+    if (
+        offsetR - offsetL >= math.tau
         or tOffsetR - tOffsetL >= math.tau
-        or upperBound - lowerBound >= math.tau):
+        or upperBound - lowerBound >= math.tau
+    ):
         return None
     polygons = []
     expanded = [(poly.buffer(maxDist), heading) for poly, heading in tField.cells]
-    for baseCell, baseHeading in field.cells:   # TODO skip cells not contained in base region?
+    for baseCell, baseHeading in field.cells:
+        # TODO skip cells not contained in base region?
         for expandedTargetCell, targetHeading in expanded:
-            lower, upper = relativeHeadingRange(baseHeading, offsetL, offsetR,
-                                                targetHeading, tOffsetL, tOffsetR)
-            if (upper >= lowerBound and lower <= upperBound):   # RH intervals overlap
+            lower, upper = relativeHeadingRange(
+                baseHeading, offsetL, offsetR, targetHeading, tOffsetL, tOffsetR
+            )
+            if upper >= lowerBound and lower <= upperBound:  # RH intervals overlap
                 intersection = baseCell & expandedTargetCell
                 if not intersection.is_empty:
-                    assert isinstance(intersection, shapely.geometry.Polygon), intersection
+                    assert isinstance(
+                        intersection, shapely.geometry.Polygon
+                    ), intersection
                     polygons.append(intersection)
     return polygonUnion(polygons)
 
-def relativeHeadingRange(baseHeading, offsetL, offsetR,
-                         targetHeading, tOffsetL, tOffsetR):
+
+def relativeHeadingRange(
+    baseHeading, offsetL, offsetR, targetHeading, tOffsetL, tOffsetR
+):
     """Lower/upper bound the possible RH between two headings with bounded disturbances."""
-    if baseHeading is None or targetHeading is None:    # heading may not be constant within cell
+    if baseHeading is None or targetHeading is None:
+        # heading may not be constant within cell
         return -math.pi, math.pi
     lower = normalizeAngle(baseHeading + offsetL)
     upper = normalizeAngle(baseHeading + offsetR)
     points = [lower, upper]
     if upper < lower:
         points.extend((math.pi, -math.pi))
     tLower = normalizeAngle(targetHeading + tOffsetL)
     tUpper = normalizeAngle(targetHeading + tOffsetR)
     tPoints = [tLower, tUpper]
     if tUpper < tLower:
         tPoints.extend((math.pi, -math.pi))
-    rhs = [tp - p for tp in tPoints for p in points]    # TODO improve
+    rhs = [tp - p for tp in tPoints for p in points]  # TODO improve
     return min(rhs), max(rhs)
```

### Comparing `scenic-2.1.0b4/src/scenic/core/utils.py` & `scenic-3.0.0b2/src/scenic/core/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,161 +1,188 @@
 """Assorted utility functions."""
 
+import bz2
 import collections
 from contextlib import contextmanager
+import functools
+import itertools
 import math
+import os
 import signal
 import sys
 import typing
+import weakref
 
-import decorator
+import trimesh
 
 sqrt2 = math.sqrt(2)
 
+if sys.version_info >= (3, 12):
+    from itertools import batched
+else:
+
+    def batched(iterable, n):
+        if n < 1:
+            raise ValueError("n must be at least one")
+        it = iter(iterable)
+        while batch := tuple(itertools.islice(it, n)):
+            yield batch
+
+
 def cached(oldMethod):
     """Decorator for making a method with no arguments cache its result"""
-    storageName = f'_cached_{oldMethod.__name__}'
-    @decorator.decorator
-    def wrapper(wrapped, *args, **kwargs):
-        self = args[0]
+    storageName = f"_cached_{oldMethod.__name__}"
+
+    @functools.wraps(oldMethod)
+    def wrapper(self):
         try:
             # Use __getattribute__ for direct lookup in case self is a Distribution
             return self.__getattribute__(storageName)
         except AttributeError:
-            value = wrapped(self)
+            value = oldMethod(self)
             setattr(self, storageName, value)
             return value
-    return wrapper(oldMethod)
+
+    return wrapper
+
+
+_methodCaches = weakref.WeakKeyDictionary()
+
+
+def cached_method(oldMethod):
+    """Decorator for making a method cache its result on a per-object basis.
+
+    Like ``functools.lru_cache(maxsize=None)`` except using a separate cache
+    for each object, with the cache automatically deallocated when the object
+    is garbage collected.
+    """
+    name = oldMethod.__name__
+
+    @functools.wraps(oldMethod)
+    def wrapper(self, *args, **kwargs):
+        caches = _methodCaches.get(self, collections.defaultdict(dict))
+        cachedMethod = caches.get(name)
+        if cachedMethod is None:
+            cachedMethod = functools.lru_cache(maxsize=None)(oldMethod)
+            caches[name] = cachedMethod
+        return cachedMethod(self, *args, **kwargs)
+
+    return wrapper
+
 
 def cached_property(oldMethod):
     return property(cached(oldMethod))
 
-def argsToString(args):
-    names = (f'{a[0]}={a[1]}' if isinstance(a, tuple) else str(a) for a in args)
-    joinedArgs = ', '.join(names)
-    return f'({joinedArgs})'
+
+def argsToString(args, kwargs={}):
+    args = ", ".join(repr(arg) for arg in args)
+    kwargs = ", ".join(f"{name}={value!r}" for name, value in kwargs.items())
+    parts = []
+    if args:
+        parts.append(args)
+    if kwargs:
+        parts.append(kwargs)
+    return ", ".join(parts)
+
 
 @contextmanager
 def alarm(seconds, handler=None, noNesting=False):
-    if seconds <= 0:
+    if seconds <= 0 or not hasattr(signal, "SIGALRM"):  # SIGALRM not supported on Windows
         yield
         return
     if handler is None:
         handler = signal.SIG_IGN
-    try:
-        signal.signal(signal.SIGALRM, handler)
-        if noNesting:
-            assert oldHandler is signal.SIG_DFL, 'SIGALRM handler already installed'
-    except ValueError:
-        yield      # SIGALRM not supported on Windows
-        return
-    previous = signal.alarm(seconds)
+    signal.signal(signal.SIGALRM, handler)
+    if noNesting:
+        assert oldHandler is signal.SIG_DFL, "SIGALRM handler already installed"
+    length = int(math.ceil(seconds))
+    previous = signal.alarm(length)
     if noNesting:
         assert previous == 0, 'nested call to "alarm"'
     try:
         yield
     finally:
         signal.alarm(0)
         signal.signal(signal.SIGALRM, signal.SIG_DFL)
 
-def areEquivalent(a, b):
-    """Whether two objects are equivalent, i.e. have the same properties.
 
-    This is only used for debugging, e.g. to check that a Distribution is the
-    same before and after pickling. We don't want to define __eq__ for such
-    objects since for example two values sampled with the same distribution are
-    equivalent but not semantically identical: the code::
+def loadMesh(path, filetype, compressed, binary):
+    working_path = path
+
+    if binary:
+        mode = "rb"
+    else:
+        mode = "r"
 
-        X = (0, 1)
-        Y = (0, 1)
+    # Check if file is compressed
+    if compressed is None:
+        root, ext = os.path.splitext(working_path)
 
-    does not make X and Y always have equal values!
-    """
-    if isinstance(a, (list, tuple)) and isinstance(b, (list, tuple)):
-        if len(a) != len(b):
-            return False
-        for x, y in zip(a, b):
-            if not areEquivalent(x, y):
-                return False
-        return True
-    elif isinstance(a, (set, frozenset)) and isinstance(b, (set, frozenset)):
-        if len(a) != len(b):
-            return False
-        mb = set(b)
-        for x in a:
-            found = False
-            for y in mb:
-                if areEquivalent(x, y):
-                    mb.remove(y)
-                    found = True
-                    break
-            if not found:
-                return False
-        return True
-    elif isinstance(a, dict) and isinstance(b, dict):
-        if len(a) != len(b):
-            return False
-        for x, v in a.items():
-            found = False
-            for y, w in b.items():
-                if areEquivalent(x, y) and areEquivalent(v, w):
-                    del b[y]
-                    found = True
-                    break
-            if not found:
-                return False
-        return True
-    elif hasattr(a, 'isEquivalentTo'):
-        return a.isEquivalentTo(b)
-    elif hasattr(b, 'isEquivalentTo'):
-        return b.isEquivalentTo(a)
+        if ext == ".bz2":
+            compressed = True
+            working_path = root
+        else:
+            compressed = False
+
+    # Check mesh filetype
+    if filetype is None:
+        root, ext = os.path.splitext(working_path)
+
+        if ext == "":
+            raise ValueError("Mesh filetype not provided, but could not be extracted")
+
+        filetype = ext
+
+    if compressed:
+        open_function = bz2.open
     else:
-        return a == b
+        open_function = open
+
+    with open_function(path, mode) as mesh_file:
+        mesh = trimesh.load(mesh_file, file_type=filetype)
+
+    return mesh
+
 
 class DefaultIdentityDict:
     """Dictionary which is the identity map by default.
 
     The map works on all objects, even unhashable ones, but doesn't support all
     of the standard mapping operations.
     """
+
     def __init__(self):
         self.storage = {}
 
+    def clear(self):
+        self.storage.clear()
+
     def __getitem__(self, key):
         return self.storage.get(id(key), key)
 
     def __setitem__(self, key, value):
         self.storage[id(key)] = value
 
     def __contains__(self, key):
         return id(key) in self.storage
 
     def __repr__(self):
-        pairs = (f'{hex(key)}: {value!r}' for key, value in self.storage.items())
-        allPairs = ', '.join(pairs)
-        return f'<DefaultIdentityDict {{{allPairs}}}>'
-
-# Generic type introspection functions backported to Python 3.7
-# (code taken from their Python 3.8 implementations)
-
-def get_type_origin(tp):
-    """Version of `typing.get_origin` supporting Python 3.7."""
-    assert sys.version_info >= (3, 7)
-    if sys.version_info >= (3, 8):
-        return typing.get_origin(tp)
-    if isinstance(tp, typing._GenericAlias):
-        return tp.__origin__
-    if tp is typing.Generic:
-        return typing.Generic
-    return None
-
-def get_type_args(tp):
-    """Version of `typing.get_args` supporting Python 3.7."""
-    assert sys.version_info >= (3, 7)
-    if sys.version_info >= (3, 8):
-        return typing.get_args(tp)
-    if isinstance(tp, typing._GenericAlias) and not tp._special:
-        res = tp.__args__
-        if get_type_origin(tp) is collections.abc.Callable and res[0] is not Ellipsis:
-            res = (list(res[:-1]), res[-1])
-        return res
-    return ()
+        pairs = (f"{hex(key)}: {value!r}" for key, value in self.storage.items())
+        allPairs = ", ".join(pairs)
+        return f"<DefaultIdentityDict {{{allPairs}}}>"
+
+
+# Patched version of typing.get_type_hints fixing bpo-37838
+
+if sys.version_info >= (3, 8, 1) or (
+    sys.version_info < (3, 8) and sys.version_info >= (3, 7, 6)
+):
+    get_type_hints = typing.get_type_hints
+else:
+
+    def get_type_hints(obj, globalns=None, localns=None):
+        if not isinstance(obj, (type, types.ModuleType)) and globalns is None:
+            wrapped = obj
+            while hasattr(wrapped, "__wrapped__"):
+                wrapped = wrapped.__wrapped__
+            globalns = getattr(wrapped, "__globals__", {})
+        return typing.get_type_hints(obj, globalns, localns)
```

### Comparing `scenic-2.1.0b4/src/scenic/domains/driving/__init__.py` & `scenic-3.0.0b2/src/scenic/domains/driving/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Domain for driving scenarios.
 
 The :doc:`world model <scenic.domains.driving.model>` defines Scenic classes for cars,
 pedestrians, etc., actions for dynamic agents which walk or drive, as well as simple
 behaviors like lane-following. Scenarios for the driving domain should import the model
-as follows:
-
-.. code-block:: scenic
+as follows::
 
     model scenic.domains.driving.model
 
 Scenarios written for the driving domain should work without changes [#f1]_ in any of the
 following simulators:
 
     * CARLA, using the model :doc:`scenic.simulators.carla.model`
@@ -46,27 +44,13 @@
         .. code-block:: console
 
             $ scenic -S --model scenic.simulators.lgsvl.model \\
                 --param map tests/formats/opendrive/maps/LGSVL/borregasave.xodr \\
                 --param lgsvl_map BorregasAve \\
                 examples/driving/badlyParkedCarPullingIn.scenic
 
-.. raw:: html
-
-   <h2>Submodules</h2>
-
-.. autosummary::
-   :toctree:
-
-   model
-   behaviors
-   actions
-   roads
-   controllers
-   workspace
-
 .. rubric:: Footnotes
 
 .. [#f1] Assuming the simulator supports the selected map. If necessary, the map may be
     changed from the command line using the :option:`--param` option; see the
     :doc:`model documentation <scenic.domains.driving.model>` for details.
 """
```

### Comparing `scenic-2.1.0b4/src/scenic/domains/driving/behaviors.scenic` & `scenic-3.0.0b2/src/scenic/domains/driving/behaviors.scenic`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Library of useful behaviors for dynamic agents in driving scenarios.
 
 These behaviors are automatically imported when using the driving domain.
 """
 
+import math
+
 from scenic.domains.driving.actions import *
 import scenic.domains.driving.model as _model
 from scenic.domains.driving.roads import ManeuverType
-from scenic.core.regions import regionFromShapelyObject
-from shapely.geometry import LineString
-import math
 
 def concatenateCenterlines(centerlines=[]):
     return PolylineRegion.unionAll(centerlines)
 
 behavior ConstantThrottleBehavior(x):
     while True:
         take SetThrottleAction(x), SetReverseAction(False), SetHandBrakeAction(False)
```

### Comparing `scenic-2.1.0b4/src/scenic/domains/driving/model.scenic` & `scenic-3.0.0b2/src/scenic/domains/driving/model.scenic`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 Imports actions and behaviors for dynamic agents from
 :doc:`scenic.domains.driving.actions` and :doc:`scenic.domains.driving.behaviors`.
 
 The map file to use for the scenario must be specified before importing this model by
 defining the global parameter ``map``. This path is passed to the `Network.fromFile`
 function to create a `Network` object representing the road network. Extra options may be
 passed to the function by defining the global parameter ``map_options``, which should be
-a dictionary of keyword arguments. For example, we could write:
-
-.. code-block:: scenic
+a dictionary of keyword arguments. For example, we could write::
 
     param map = localPath('mymap.xodr')
     param map_options = { 'tolerance': 0.1 }
     model scenic.domains.driving.model
 
 If you are writing a generic scenario that supports multiple maps, you may leave the
 ``map`` parameter undefined; then running the scenario will produce an error unless the
@@ -24,15 +22,14 @@
     If you are using a simulator, you may have to also define simulator-specific global
     parameters to tell the simulator which world to load. For example, our LGSVL
     interface uses a parameter ``lgsvl_map`` to specify the name of the Unity scene.
     See the :doc:`documentation <scenic.simulators>` of the simulator interfaces for
     details.
 """
 
-from abc import ABC, abstractmethod
 from typing import Optional
 
 from scenic.domains.driving.workspace import DrivingWorkspace
 from scenic.domains.driving.roads import (ManeuverType, Network, Road, Lane, LaneSection,
                                           LaneGroup, Intersection, PedestrianCrossing,
                                           NetworkElement)
 from scenic.domains.driving.actions import *
@@ -79,14 +76,18 @@
 #: Inside intersections or anywhere else where there can be multiple nominal
 #: traffic directions, the choice is arbitrary. At such points, the function
 #: `Network.nominalDirectionsAt` can be used to get all nominal directions.
 roadDirection : VectorField = network.roadDirection
 
 ## Standard object types
 
+def is2DMode():
+    from scenic.syntax.veneer import mode2D
+    return mode2D
+
 class DrivingObject:
     """Abstract class for objects in a road network.
 
     Provides convenience properties for the lane, road, intersection, etc. at the
     object's current position (if any).
 
     Also defines the ``elevation`` property as a standard way to access the Z
@@ -98,15 +99,15 @@
 
     Properties:
         elevation (float or None; dynamic): default ``None`` (see above).
         requireVisible (bool): Default value ``False`` (overriding the default
             from `Object`).
     """
 
-    elevation[dynamic]: None
+    elevation[dynamic]: None if is2DMode() else float(self.position.z)
 
     requireVisible: False
 
     # Semantic category properties
 
     @property
     def isVehicle(self):
@@ -220,15 +221,15 @@
         return network.elementAt(self)
 
     # Utility functions
 
     def distanceToClosest(self, type: type) -> Object:
         """Compute the distance to the closest object of the given type.
 
-        For example, one could write :samp:`self.distanceToClosest(Car)` in a behavior.
+        For example, one could write :scenic:`self.distanceToClosest(Car)` in a behavior.
         """
         objects = simulation().objects
         minDist = float('inf')
         for obj in objects:
             if not isinstance(obj, type):
                 continue
             d = distance from self to obj
@@ -249,24 +250,24 @@
 
     Properties:
         position: The default position is uniformly random over the `road`.
         heading: The default heading is aligned with `roadDirection`, plus an offset
             given by **roadDeviation**.
         roadDeviation (float): Relative heading with respect to the road direction at
             the `Vehicle`'s position. Used by the default value for **heading**.
-        regionContainedIn: The default container is `roadOrShoulder`.
+        regionContainedIn: The default container is :obj:`roadOrShoulder`.
         viewAngle: The default view angle is 90 degrees.
         width: The default width is 2 meters.
         length: The default length is 4.5 meters.
         color (:obj:`Color` or RGB tuple): Color of the vehicle. The default value is a
             distribution derived from car color popularity statistics; see
             :obj:`Color.defaultCarColor`.
     """
     regionContainedIn: roadOrShoulder
-    position: Point on road
+    position: new Point on road
     heading: (roadDirection at self.position) + self.roadDeviation
     roadDeviation: 0
     viewAngle: 90 deg
     width: 2
     length: 4.5
     color: Color.defaultCarColor()
 
@@ -293,61 +294,21 @@
         viewAngle: The default view angle is 90 degrees.
         width: The default width is 0.75 m.
         length: The default length is 0.75 m.
         color: The default color is turquoise. Pedestrian colors are not necessarily
             used by simulators, but do appear in the debugging diagram.
     """
     regionContainedIn: network.walkableRegion
-    position: Point on network.walkableRegion
+    position: new Point on network.walkableRegion
     heading: Range(0, 360) deg
     viewAngle: 90 deg
     width: 0.75
     length: 0.75
     color: [0, 0.5, 1]
 
-# Mixin classes indicating support for various types of actions
-
-class Steers(ABC):
-    """Mixin protocol for agents which can steer.
-
-    Specifically, agents must support throttling, braking, steering, setting the hand
-    brake, and going into reverse.
-    """
-    @abstractmethod
-    def setThrottle(self, throttle): pass
-
-    @abstractmethod
-    def setSteering(self, steering): pass
-
-    @abstractmethod
-    def setBraking(self, braking): pass
-
-    @abstractmethod
-    def setHandbrake(self, handbrake): pass
-
-    @abstractmethod
-    def setReverse(self, reverse): pass
-
-class Walks(ABC):
-    """Mixin protocol for agents which can walk with a given direction and speed.
-
-    We provide a simplistic implementation which directly sets the velocity of the agent.
-    This implementation needs to be explicitly opted-into, since simulators may provide a
-    more sophisticated API that properly animates pedestrians.
-    """
-    @abstractmethod
-    def setWalkingDirection(self, heading):
-        velocity = Vector(0, self.speed).rotatedBy(heading)
-        self.setVelocity(velocity)
-
-    @abstractmethod
-    def setWalkingSpeed(self, speed):
-        velocity = speed * self.velocity.normalized()
-        self.setVelocity(velocity)
-
 ## Utility functions
 
 def withinDistanceToAnyCars(car, thresholdDistance):
     """ returns boolean """
     objects = simulation().objects
     for obj in objects:
         if obj is car or not isinstance(obj, Vehicle):
@@ -383,8 +344,8 @@
         inter = network.intersectionAt(vehicle)
         if inter and inter != network.intersectionAt(obj):    # different intersections
             continue
         if not inter and network.laneAt(vehicle) != network.laneAt(obj):    # different lanes
             continue
         if (distance from vehicle to obj) < thresholdDistance:
             return True
-    return False
+    return False
```

### Comparing `scenic-2.1.0b4/src/scenic/domains/driving/roads.py` & `scenic-3.0.0b2/src/scenic/domains/driving/roads.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,116 +2,137 @@
 
 A road network is represented by an instance of the :obj:`Network` class, which can
 be created from a map file using :obj:`Network.fromFile`.
 
 .. note::
 
     This library is a prototype under active development. We will try not to make
-    backwards-incompatible changes, but the API may not be entirely stable. Some
-    network information, such as traffic signals, has not yet been made available.
+    backwards-incompatible changes, but the API may not be entirely stable.
 """
 
 from __future__ import annotations  # allow forward references for type annotations
 
-import io
 import enum
+import gzip
 import hashlib
+import io
+import itertools
 import math
 import numbers
-from typing import FrozenSet, Union, Tuple, Optional, Sequence, List
-import itertools
 import pathlib
-import gzip
 import pickle
-import time
 import struct
+import time
+from typing import FrozenSet, List, Optional, Sequence, Tuple, Union
 import weakref
 
 import attr
-from shapely.geometry import Polygon, MultiPolygon
+import shapely
+from shapely.geometry import MultiPolygon, Polygon
 
-from scenic.core.distributions import distributionFunction, distributionMethod
-from scenic.core.vectors import Vector, VectorField
-from scenic.core.regions import PolygonalRegion, PolylineRegion
-from scenic.core.object_types import Point
-import scenic.core.geometry as geometry
-import scenic.core.utils as utils
+from scenic.core.distributions import (
+    RejectionException,
+    distributionFunction,
+    distributionMethod,
+)
 from scenic.core.errors import InvalidScenarioError
-from scenic.core.distributions import RejectionException, distributionFunction
+import scenic.core.geometry as geometry
+from scenic.core.object_types import Point
+from scenic.core.regions import PolygonalRegion, PolylineRegion
 import scenic.core.type_support as type_support
-from scenic.syntax.veneer import verbosePrint
+import scenic.core.utils as utils
+from scenic.core.vectors import Orientation, Vector, VectorField
 import scenic.syntax.veneer as veneer
+from scenic.syntax.veneer import verbosePrint
 
 ## Typing and utilities
 
 #: Alias for types which can be interpreted as positions in Scenic.
 #:
 #: This includes instances of `Point` and `Object`, and pairs of numbers.
 Vectorlike = Union[Vector, Point, Tuple[numbers.Real, numbers.Real]]
 
+
 def _toVector(thing: Vectorlike) -> Vector:
     return type_support.toVector(thing)
 
+
 def _rejectSample(message):
     if veneer.isActive():
         raise InvalidScenarioError(message)
     else:
         raise RejectionException(message)
 
-def _rejectIfNonexistent(element, name='network element'):
+
+def _rejectIfNonexistent(element, name="network element"):
     if element is None:
-        _rejectSample(f'requested {name} does not exist')
+        _rejectSample(f"requested {name} does not exist")
     return element
 
+
 class _ElementReferencer:
     """Mixin class to improve pickling of classes that reference network elements.
 
     :meta private:
     """
+
     def __getstate__(self):
-        if hasattr(super(), '__getstate__'):
+        if hasattr(super(), "__getstate__"):
             state = super().__getstate__()
+            if state is self.__dict__:
+                state = state.copy()
         else:
             state = self.__dict__.copy()
         # replace links to network elements by placeholders to prevent deep
         # recursions during pickling; as a result of this, only entire `Network`
         # objects can be properly unpickled
         for key, value in state.items():
             if isinstance(value, NetworkElement):
                 state[key] = _ElementPlaceholder(value.uid)
         return state
 
+
 class _ElementPlaceholder:
     """Placeholder for a link to a pickled `NetworkElement`.
 
     :meta private:
     """
+
     def __init__(self, uid):
         self.uid = uid
 
+
 ## Metadata
 
+
 @enum.unique
 class VehicleType(enum.Enum):
     """A type of vehicle, including pedestrians. Used to classify lanes."""
+
     CAR = 1
     BICYCLE = 2
     PEDESTRIAN = 3
 
+
 @enum.unique
 class ManeuverType(enum.Enum):
     """A type of `Maneuver`, e.g., going straight or turning left."""
-    STRAIGHT = enum.auto()      #: Straight, including one lane merging into another.
-    LEFT_TURN = enum.auto()     #: Left turn.
-    RIGHT_TURN = enum.auto()    #: Right turn.
-    U_TURN = enum.auto()        #: U-turn.
+
+    STRAIGHT = enum.auto()  #: Straight, including one lane merging into another.
+    LEFT_TURN = enum.auto()  #: Left turn.
+    RIGHT_TURN = enum.auto()  #: Right turn.
+    U_TURN = enum.auto()  #: U-turn.
 
     @staticmethod
-    def guessTypeFromLanes(start: Lane, end: Lane, connecting: Union[Lane, None],
-                           turnThreshold: float = math.radians(20)):
+    def guessTypeFromLanes(
+        start: Lane,
+        end: Lane,
+        connecting: Union[Lane, None],
+        turnThreshold: float = math.radians(20),
+    ):
         """For formats lacking turn information, guess it from the geometry.
 
         Arguments:
             start: starting lane of the maneuver.
             end: ending lane of the maneuver.
             connecting: connecting lane of the maneuver, if any.
             turnThreshold: angle beyond which to consider a maneuver a turn.
@@ -128,70 +149,77 @@
         if turnAngle >= turnThreshold:
             return ManeuverType.LEFT_TURN
         elif turnAngle <= -turnThreshold:
             return ManeuverType.RIGHT_TURN
         else:
             return ManeuverType.STRAIGHT
 
+
 @attr.s(auto_attribs=True, kw_only=True, eq=False)
 class Maneuver(_ElementReferencer):
     """Maneuver()
 
     A maneuver which can be taken upon reaching the end of a lane.
     """
-    type: ManeuverType = None   #: type of maneuver (straight, left turn, etc.)
-    startLane: Lane             #: starting lane of the maneuver
-    endLane: Lane               #: ending lane of the maneuver
+
+    type: ManeuverType = None  #: type of maneuver (straight, left turn, etc.)
+    startLane: Lane  #: starting lane of the maneuver
+    endLane: Lane  #: ending lane of the maneuver
 
     # the following attributes are None if startLane directly merges into endLane,
     # rather than connecting via a maneuver through an intersection
 
     #: connecting lane from the start to the end lane, if any (`None` for lane mergers)
     connectingLane: Union[Lane, None] = None
     #: intersection where the maneuver takes place, if any (`None` for lane mergers)
     intersection: Union[Intersection, None] = None
 
     def __attrs_post_init__(self):
         assert self.type is ManeuverType.STRAIGHT or self.connectingLane is not None
 
-        if self.type is None:   # unknown maneuver type; need to guess from geometry
-            ty = ManeuverType.guessTypeFromLanes(self.startLane, self.endLane, self.connectingLane)
-            object.__setattr__(self, 'type', ty)
+        if self.type is None:  # unknown maneuver type; need to guess from geometry
+            ty = ManeuverType.guessTypeFromLanes(
+                self.startLane, self.endLane, self.connectingLane
+            )
+            object.__setattr__(self, "type", ty)
 
     @property
     @utils.cached
     def conflictingManeuvers(self) -> Tuple[Maneuver]:
         """Maneuvers whose connecting lanes intersect this one's."""
         if not self.connectingLane:
             return ()
         guideway = self.connectingLane
         start = self.startLane
         conflicts = []
         for maneuver in self.intersection.maneuvers:
-            if (maneuver.startLane is not start
-                and maneuver.connectingLane.centerline.intersects(guideway.centerline)):
+            if (
+                maneuver.startLane is not start
+                and maneuver.connectingLane.centerline.intersects(guideway.centerline)
+            ):
                 conflicts.append(maneuver)
         return tuple(conflicts)
 
     @property
     @utils.cached
     def reverseManeuvers(self) -> Tuple[Maneuver]:
-    	"""Maneuvers whose start and end roads are the reverse of this one's."""
-    	start = self.startLane.road
-    	end = self.endLane.road
-    	reverses = []
-    	for maneuver in self.intersection.maneuvers:
-    		if (maneuver.startLane.road is end
-    			and maneuver.endLane.road is start):
-    			reverses.append(maneuver)
-    	return tuple(reverses)
+        """Maneuvers whose start and end roads are the reverse of this one's."""
+        start = self.startLane.road
+        end = self.endLane.road
+        reverses = []
+        for maneuver in self.intersection.maneuvers:
+            if maneuver.startLane.road is end and maneuver.endLane.road is start:
+                reverses.append(maneuver)
+        return tuple(reverses)
+
 
 ## Road networks
 
-@attr.s(auto_attribs=True, kw_only=True, repr=False)
+
+@attr.s(auto_attribs=True, kw_only=True, repr=False, eq=False)
 class NetworkElement(_ElementReferencer, PolygonalRegion):
     """NetworkElement()
 
     Abstract class for part of a road network.
 
     Includes roads, lane groups, lanes, sidewalks, pedestrian crossings,
     and intersections.
@@ -201,20 +229,20 @@
     distances to an element, etc.
     """
 
     # from PolygonalRegion
     polygon: Union[Polygon, MultiPolygon]
     orientation: Optional[VectorField] = None
 
-    name: str = ''      #: Human-readable name, if any.
+    name: str = ""  #: Human-readable name, if any.
     #: Unique identifier; from underlying format, if possible.
     #: (In OpenDRIVE, for example, ids are not necessarily unique, so we invent our own.)
     uid: str = None
-    id: Optional[str] = None    #: Identifier from underlying format, if any.
-    network: Network = None     #: Link to parent network.
+    id: Optional[str] = None  #: Identifier from underlying format, if any.
+    network: Network = None  #: Link to parent network.
 
     ## Traffic info
 
     #: Which types of vehicles (car, bicycle, etc.) can be here.
     vehicleTypes: FrozenSet[VehicleType] = frozenset([VehicleType.CAR])
     #: Optional speed limit, which may be inherited from parent.
     speedLimit: Union[float, None] = None
@@ -222,41 +250,53 @@
     tags: FrozenSet[str] = frozenset()
 
     def __attrs_post_init__(self):
         assert self.uid is not None or self.id is not None
         if self.uid is None:
             self.uid = self.id
 
-        super().__init__(polygon=self.polygon, orientation=self.orientation, name=self.name)
+        super().__init__(
+            polygon=self.polygon, orientation=self.orientation, name=self.name
+        )
 
     @distributionFunction
-    def nominalDirectionsAt(self, point: Vectorlike) -> Tuple[float]:
+    def nominalDirectionsAt(self, point: Vectorlike) -> Tuple[Orientation]:
         """Get nominal traffic direction(s) at a point in this element.
 
         There must be at least one such direction. If there are multiple, we
         pick one arbitrarily to be the orientation of the element as a `Region`.
         (So ``Object in element`` will align by default to that orientation.)
         """
+        assert self.orientation, self
         return (self.orientation[_toVector(point)],)
 
     def __getstate__(self):
         state = super().__getstate__()
-        del state['network']    # do not pickle weak reference to parent network
+        del state["network"]  # do not pickle weak reference to parent network
         return state
 
+    def __eq__(self, other):
+        if not isinstance(other, NetworkElement):
+            return NotImplemented
+        return self.network is other.network and self.uid == other.uid
+
+    def __hash__(self):
+        return hash((self.network.__hash__(), self.uid))
+
     def __repr__(self):
-        s = f'<{type(self).__name__} at {hex(id(self))}; '
+        s = f"<{type(self).__name__} at {hex(id(self))}; "
         if self.name:
             s += f'name="{self.name}", '
         if self.id and self.id != self.uid:
             s += f'id="{self.id}", '
         s += f'uid="{self.uid}">'
         return s
 
-@attr.s(auto_attribs=True, kw_only=True, repr=False)
+
+@attr.s(auto_attribs=True, kw_only=True, repr=False, eq=False)
 class LinearElement(NetworkElement):
     """LinearElement()
 
     A part of a road network with (mostly) linear 1- or 2-way flow.
 
     Includes roads, lane groups, lanes, sidewalks, and pedestrian crossings,
     but not intersections.
@@ -271,24 +311,24 @@
 
     # Geometric info (on top of the overall polygon from PolygonalRegion)
     centerline: PolylineRegion
     leftEdge: PolylineRegion
     rightEdge: PolylineRegion
 
     # Links to next/previous element
-    _successor: Union[NetworkElement, None] = None   # going forward
-    _predecessor: Union[NetworkElement, None] = None # going backward
+    _successor: Union[NetworkElement, None] = None  # going forward
+    _predecessor: Union[NetworkElement, None] = None  # going backward
 
     @property
     def successor(self):
-        return _rejectIfNonexistent(self._successor, 'successor')
+        return _rejectIfNonexistent(self._successor, "successor")
 
     @property
     def predecessor(self):
-        return _rejectIfNonexistent(self._predecessor, 'predecessor')
+        return _rejectIfNonexistent(self._predecessor, "predecessor")
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         # Check that left and right edges lie inside the element.
         # (don't check centerline here since it can lie inside a median, for example)
         # (TODO reconsider the decision to have polygon only include drivable areas?)
         assert self.containsRegion(self.leftEdge, tolerance=0.5)
@@ -306,17 +346,21 @@
         :meta private:
         """
         point = _toVector(point)
         start, end = self.centerline.nearestSegmentTo(point)
         return start.angleTo(end)
 
     @distributionFunction
-    def flowFrom(self, point: Vectorlike, distance: float,
-                 steps: Union[int, None] = None,
-                 stepSize: float = 5) -> Vector:
+    def flowFrom(
+        self,
+        point: Vectorlike,
+        distance: float,
+        steps: Union[int, None] = None,
+        stepSize: float = 5,
+    ) -> Vector:
         """Advance a point along this element by a given distance.
 
         Equivalent to ``follow element.orientation from point for distance``, but
         possibly more accurate. The default implementation uses the forward
         Euler approximation with a step size of 5 meters; subclasses may ignore
         the **steps** and **stepSize** parameters if they can compute the flow
         exactly.
@@ -325,27 +369,31 @@
             point: point to start from.
             distance: distance to travel.
             steps: number of steps to take, or :obj:`None` to compute the
                 number of steps based on the distance (default :obj:`None`).
             stepSize: length used to compute how many steps to take, if **steps** is not
                 specified (default 5 meters).
         """
-        return self.orientation.followFrom(_toVector(point), distance,
-                                           steps=steps, stepSize=stepSize)
+        return self.orientation.followFrom(
+            _toVector(point), distance, steps=steps, stepSize=stepSize
+        )
+
 
 class _ContainsCenterline:
     """Mixin which asserts that the centerline is contained in the polygon.
 
     :meta private:
     """
+
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         assert self.containsRegion(self.centerline, tolerance=0.5)
 
-@attr.s(auto_attribs=True, kw_only=True, repr=False)
+
+@attr.s(auto_attribs=True, kw_only=True, repr=False, eq=False)
 class Road(LinearElement):
     """Road()
 
     A road consisting of one or more lanes.
 
     Lanes are grouped into 1 or 2 instances of `LaneGroup`:
 
@@ -355,24 +403,25 @@
     One of these may be None if there are no lanes in that direction.
 
     Because of splits and mergers, the Lanes of a `Road` do not necessarily start
     or end at the same point as the `Road`. Such intermediate branching points
     cause the `Road` to be partitioned into multiple road sections, within which
     the configuration of lanes is fixed.
     """
+
     #: All lanes of this road, in either direction.
     #:
     #: The order of the lanes is arbitrary. To access lanes in order according to their
     #: geometry, use `LaneGroup.lanes`.
     lanes: Tuple[Lane]
 
     #: Group of lanes aligned with the direction of the road, if any.
     forwardLanes: Union[LaneGroup, None]
     #: Group of lanes going in the opposite direction, if any.
-    backwardLanes: Union[LaneGroup, None]   # lanes going the other direction
+    backwardLanes: Union[LaneGroup, None]  # lanes going the other direction
 
     #: All LaneGroups of this road, with `forwardLanes` being first if it exists.
     laneGroups: Tuple[LaneGroup] = None
 
     #: All sections of this road, ordered from start to end.
     sections: Tuple[RoadSection]
 
@@ -428,129 +477,132 @@
 
     @distributionFunction
     def laneGroupAt(self, point: Vectorlike, reject=False) -> Union[LaneGroup, None]:
         """Get the `LaneGroup` passing through a given point."""
         return self.network.findPointIn(point, self.laneGroups, reject)
 
     @distributionFunction
-    def crossingAt(self, point: Vectorlike, reject=False) -> Union[PedestrianCrossing, None]:
+    def crossingAt(
+        self, point: Vectorlike, reject=False
+    ) -> Union[PedestrianCrossing, None]:
         """Get the :obj:`.PedestrianCrossing` passing through a given point."""
         return self.network.findPointIn(point, self.crossings, reject)
 
     @distributionFunction
     def shiftLanes(self, point: Vectorlike, offset: int) -> Union[Vector, None]:
         """Find the point equivalent to this one but shifted over some # of lanes."""
-        raise NotImplementedError   # TODO implement this
+        raise NotImplementedError  # TODO implement this
 
     @property
     def is1Way(self) -> bool:
         return self.forwardLanes is None or self.backwardLanes is None
 
-@attr.s(auto_attribs=True, kw_only=True, repr=False)
+
+@attr.s(auto_attribs=True, kw_only=True, repr=False, eq=False)
 class LaneGroup(LinearElement):
     """LaneGroup()
 
     A group of parallel lanes with the same type and direction.
     """
 
-    road: Road          #: Parent road.
+    road: Road  #: Parent road.
     lanes: Tuple[Lane]  #: Lanes, partially ordered with lane 0 being closest to the curb.
 
     #: Region representing the associated curb, which is not necessarily adjacent if
     #: there are parking lanes or some other kind of shoulder.
     curb: PolylineRegion
 
     # associated elements not actually part of this group
-    _sidewalk: Union[Sidewalk, None] = None     #: Adjacent sidewalk, if any.
+    _sidewalk: Union[Sidewalk, None] = None  #: Adjacent sidewalk, if any.
     _bikeLane: Union[Lane, None] = None
-    _shoulder: Union[Shoulder, None] = None     #: Adjacent shoulder, if any.
+    _shoulder: Union[Shoulder, None] = None  #: Adjacent shoulder, if any.
     #: Opposite lane group of the same road, if any.
     _opposite: Union[LaneGroup, None] = None
 
     @property
     def sidewalk(self) -> Sidewalk:
         """The adjacent sidewalk; rejects if there is none."""
-        return _rejectIfNonexistent(self._sidewalk, 'sidewalk')
+        return _rejectIfNonexistent(self._sidewalk, "sidewalk")
 
     @property
     def bikeLane(self) -> Lane:
-        return _rejectIfNonexistent(self._bikeLane, 'bike lane')
+        return _rejectIfNonexistent(self._bikeLane, "bike lane")
 
     @property
     def shoulder(self) -> Shoulder:
         """The adjacent shoulder; rejects if there is none."""
-        return _rejectIfNonexistent(self._shoulder, 'shoulder')
+        return _rejectIfNonexistent(self._shoulder, "shoulder")
 
     @property
     def opposite(self) -> LaneGroup:
         """The opposite lane group of the same road; rejects if there is none."""
-        return _rejectIfNonexistent(self._opposite, 'opposite lane group')
+        return _rejectIfNonexistent(self._opposite, "opposite lane group")
 
     def _defaultHeadingAt(self, point):
         point = _toVector(point)
         lane = self.laneAt(point)
         if lane:
             return lane.orientation[point]
         return super()._defaultHeadingAt(point)
 
     @distributionFunction
     def laneAt(self, point: Vectorlike, reject=False) -> Union[Lane, None]:
         """Get the `Lane` passing through a given point."""
         return self.network.findPointIn(point, self.lanes, reject)
 
-@attr.s(auto_attribs=True, kw_only=True, eq=False, repr=False)
+
+@attr.s(auto_attribs=True, kw_only=True, repr=False, eq=False)
 class Lane(_ContainsCenterline, LinearElement):
     """Lane()
 
     A lane for cars, bicycles, or other vehicles.
     """
 
-    group: LaneGroup            # parent lane group
-    road: Road                  # grandparent road
-    sections: Tuple[LaneSection]    # sections in order from start to end
+    group: LaneGroup  # parent lane group
+    road: Road  # grandparent road
+    sections: Tuple[LaneSection]  # sections in order from start to end
 
-    adjacentLanes: Tuple[Lane] = ()     # adjacent lanes of same type, if any
+    adjacentLanes: Tuple[Lane] = ()  # adjacent lanes of same type, if any
 
-    maneuvers: Tuple[Maneuver] = ()     # possible maneuvers upon reaching the end of this lane
+    # possible maneuvers upon reaching the end of this lane
+    maneuvers: Tuple[Maneuver] = ()
 
     @distributionFunction
     def sectionAt(self, point: Vectorlike, reject=False) -> Union[LaneSection, None]:
         """Get the LaneSection passing through a given point."""
         return self.network.findPointIn(point, self.sections, reject)
 
-    # TODO remove hack; freeze all these classes
-    __hash__ = object.__hash__
 
-@attr.s(auto_attribs=True, kw_only=True, repr=False)
+@attr.s(auto_attribs=True, kw_only=True, repr=False, eq=False)
 class RoadSection(LinearElement):
     """RoadSection()
 
     Part of a road with a fixed number of lanes.
 
     A RoadSection has a fixed number of lanes: when a lane begins or ends, we
     move to a new section (which will be the successor of the current one).
     """
 
-    road: Road      # parent road
-    lanes: Tuple[LaneSection] = ()   # in order, with lane 0 being the rightmost
-    forwardLanes: Tuple[LaneSection] = ()   # as above
+    road: Road  # parent road
+    lanes: Tuple[LaneSection] = ()  # in order, with lane 0 being the rightmost
+    forwardLanes: Tuple[LaneSection] = ()  # as above
     backwardLanes: Tuple[LaneSection] = ()  # as above
 
     lanesByOpenDriveID: Dict[LaneSection]
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         if not self.lanes and not self.lanesByOpenDriveID:
-            raise RuntimeError('RoadSection created with no lanes')
+            raise RuntimeError("RoadSection created with no lanes")
         if self.lanesByOpenDriveID and not self.lanes:
             forward, backward = [], []
             rightmost = min(self.lanesByOpenDriveID)
             assert rightmost != 0, self.lanesByOpenDriveID
             leftmost = max(self.lanesByOpenDriveID)
-            for i in range(rightmost, leftmost+1):
+            for i in range(rightmost, leftmost + 1):
                 if i == 0:
                     continue
                 if i not in self.lanesByOpenDriveID:
                     continue
                 (forward if i < 0 else backward).append(self.lanesByOpenDriveID[i])
             self.forwardLanes = tuple(forward)
             self.backwardLanes = tuple(backward)
@@ -569,33 +621,34 @@
         if lane:
             return lane.orientation[point]
         return super()._defaultHeadingAt(point)
 
     @distributionFunction
     def laneAt(self, point: Vectorlike, reject=False) -> Union[LaneSection, None]:
         """Get the lane section passing through a given point."""
-        return self.network.findPointIn(point, self.lane, reject)
+        return self.network.findPointIn(point, self.lanes, reject)
+
 
-@attr.s(auto_attribs=True, kw_only=True, repr=False)
+@attr.s(auto_attribs=True, kw_only=True, repr=False, eq=False)
 class LaneSection(_ContainsCenterline, LinearElement):
     """LaneSection()
 
     Part of a lane in a single `RoadSection`.
 
     Since the lane configuration in a `RoadSection` is fixed, a `LaneSection` can have
     at most one adjacent lane to left or right. These are accessible using the
     `laneToLeft` and `laneToRight` properties, which for convenience reject the
     simulation if the desired lane does not exist. If rejection is not desired (for
     example if you want to handle the case where there is no lane to the left yourself),
     you can use the `_laneToLeft` and `_laneToRight` properties instead.
     """
 
-    lane: Lane          #: Parent lane.
-    group: LaneGroup    #: Grandparent lane group.
-    road: Road          #: Great-grandparent road.
+    lane: Lane  #: Parent lane.
+    group: LaneGroup  #: Grandparent lane group.
+    road: Road  #: Great-grandparent road.
 
     #: ID number as in OpenDRIVE (number of lanes to left of center, with 1 being the
     # first lane left of the centerline and -1 being the first lane to the right).
     openDriveID: int
     #: Whether this lane has the same direction as its parent road.
     isForward: bool = True
 
@@ -612,119 +665,151 @@
     _fasterLane: Union[LaneSection, None] = None
     #: Slower adjacent lane of same type, if any.
     _slowerLane: Union[LaneSection, None] = None
 
     @property
     def laneToLeft(self) -> LaneSection:
         """The adjacent lane of the same type to the left; rejects if there is none."""
-        return _rejectIfNonexistent(self._laneToLeft, 'lane to left')
+        return _rejectIfNonexistent(self._laneToLeft, "lane to left")
 
     @property
     def laneToRight(self) -> LaneSection:
         """The adjacent lane of the same type to the right; rejects if there is none."""
-        return _rejectIfNonexistent(self._laneToRight, 'lane to right')
+        return _rejectIfNonexistent(self._laneToRight, "lane to right")
 
     @property
     def fasterLane(self) -> LaneSection:
         """The faster adjacent lane of the same type; rejects if there is none."""
-        return _rejectIfNonexistent(self._fasterLane, 'faster lane')
+        return _rejectIfNonexistent(self._fasterLane, "faster lane")
 
     @property
     def slowerLane(self) -> LaneSection:
         """The slower adjacent lane of the same type; rejects if there is none."""
-        return _rejectIfNonexistent(self._slowerLane, 'slower lane')
+        return _rejectIfNonexistent(self._slowerLane, "slower lane")
 
     @distributionFunction
     def shiftedBy(self, offset: int) -> Union[LaneSection, None]:
         """Find the lane a given number of lanes over from this lane."""
         current = self
         for i in range(abs(offset)):
             if offset > 0:
                 current = current.laneToLeft
             else:
                 current = current.laneToRight
             if current is None:
                 return None
         return current
 
-@attr.s(auto_attribs=True, kw_only=True, repr=False)
+
+@attr.s(auto_attribs=True, kw_only=True, repr=False, eq=False)
 class Sidewalk(_ContainsCenterline, LinearElement):
     """Sidewalk()
 
     A sidewalk.
     """
+
     road: Road
     crossings: Tuple[PedestrianCrossing]
 
-@attr.s(auto_attribs=True, kw_only=True, repr=False)
+
+@attr.s(auto_attribs=True, kw_only=True, repr=False, eq=False)
 class PedestrianCrossing(_ContainsCenterline, LinearElement):
     """PedestrianCrossing()
 
     A pedestrian crossing (crosswalk).
     """
+
     parent: Union[Road, Intersection]
     startSidewalk: Sidewalk
     endSidewalk: Sidewalk
 
-@attr.s(auto_attribs=True, kw_only=True, repr=False)
+
+@attr.s(auto_attribs=True, kw_only=True, repr=False, eq=False)
 class Shoulder(_ContainsCenterline, LinearElement):
     """Shoulder()
 
     A shoulder of a road, including parking lanes by default.
     """
+
     road: Road
 
-@attr.s(auto_attribs=True, kw_only=True, repr=False)
+
+@attr.s(auto_attribs=True, kw_only=True, repr=False, eq=False)
 class Intersection(NetworkElement):
     """Intersection()
 
     An intersection where multiple roads meet.
     """
-    roads: Tuple[Road]     # in some order, preserving adjacency
+
+    roads: Tuple[Road]  # in some order, preserving adjacency
     incomingLanes: Tuple[Lane]
     outgoingLanes: Tuple[Lane]
     maneuvers: Tuple[Maneuver]  # all possible maneuvers through the intersection
 
     signals: Tuple[Signal]
 
-    crossings: Tuple[PedestrianCrossing]    # also ordered to preserve adjacency
+    crossings: Tuple[PedestrianCrossing]  # also ordered to preserve adjacency
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         for maneuver in self.maneuvers:
             assert maneuver.connectingLane, maneuver
             assert self.containsRegion(maneuver.connectingLane, tolerance=0.5)
+        if self.orientation is None:
+            self.orientation = VectorField(self.name, self._defaultHeadingAt)
+
+    def _defaultHeadingAt(self, point):
+        """Default orientation for this Intersection.
+
+        We align along the closest connecting lane.
+
+        :meta private:
+        """
+        point = _toVector(point)
+        man = min(self.maneuvers, key=lambda man: man.connectingLane.distanceTo(point))
+        return man.connectingLane.orientation[point]
 
     @property
     def is3Way(self) -> bool:
         """bool: Whether or not this is a 3-way intersection."""
         return len(self.roads) == 3
+
     @property
     def is4Way(self) -> bool:
         """bool: Whether or not this is a 4-way intersection."""
         return len(self.roads) == 4
 
     @property
     def isSignalized(self) -> bool:
         """bool: Whether or not this is a signalized intersection."""
         return len(self.signals) > 0
 
     @distributionFunction
     def maneuversAt(self, point: Vectorlike) -> List[Maneuver]:
         """Get all maneuvers possible at a given point in the intersection."""
-        return self.network._findPointInAll(point, self.maneuvers,
-                                            key=lambda m: m.connectingLane)
+        maneuvers = self.network._findPointInAll(
+            point, self.maneuvers, key=lambda m: m.connectingLane
+        )
+        if maneuvers:
+            return maneuvers
+        # If we filled holes in intersections when computing the geometry, there
+        # might be no maneuvers at some points inside the intersection. We'll pick
+        # the closest one.
+        man = min(self.maneuvers, key=lambda man: man.connectingLane.distanceTo(point))
+        return [man]
 
     @distributionFunction
-    def nominalDirectionsAt(self, point: Vectorlike) -> List[float]:
+    def nominalDirectionsAt(self, point: Vectorlike) -> Tuple[Orientation]:
         point = _toVector(point)
         maneuvers = self.maneuversAt(point)
-        return [m.connectingLane.orientation[point] for m in maneuvers]
+        assert maneuvers, self
+        return tuple(m.connectingLane.orientation[point] for m in maneuvers)
 
-@attr.s(auto_attribs=True, kw_only=True, repr=False)
+
+@attr.s(auto_attribs=True, kw_only=True, repr=False, eq=False)
 class Signal:
     """Traffic lights, stop signs, etc.
 
     .. warning::
 
         Signal parsing is a work in progress and the API is likely to change in the future.
     """
@@ -738,15 +823,16 @@
     type: str
 
     @property
     def isTrafficLight(self) -> bool:
         """Whether or not this signal is a traffic light."""
         return self.type == "1000001"
 
-@attr.s(auto_attribs=True, kw_only=True, repr=False)
+
+@attr.s(auto_attribs=True, kw_only=True, repr=False, eq=False)
 class Network:
     """Network()
 
     A road network.
 
     Networks are composed of roads, intersections, sidewalks, etc., which are all
     instances of `NetworkElement`.
@@ -823,62 +909,79 @@
         if self.sidewalkRegion is None:
             self.sidewalkRegion = PolygonalRegion.unionAll(self.sidewalks)
         if self.shoulderRegion is None:
             self.shoulderRegion = PolygonalRegion.unionAll(self.shoulders)
 
         if self.drivableRegion is None:
             self.drivableRegion = self.laneRegion.union(self.intersectionRegion)
+        assert self.drivableRegion.containsRegion(
+            self.laneRegion, tolerance=self.tolerance
+        )
+        assert self.drivableRegion.containsRegion(
+            self.intersectionRegion, tolerance=self.tolerance
+        )
         if self.walkableRegion is None:
             self.walkableRegion = self.sidewalkRegion.union(self.crossingRegion)
+        assert self.walkableRegion.containsRegion(
+            self.sidewalkRegion, tolerance=self.tolerance
+        )
+        assert self.walkableRegion.containsRegion(
+            self.crossingRegion, tolerance=self.tolerance
+        )
 
         if self.curbRegion is None:
             edges = []
-            for road in self.roads:     # only include curbs of ordinary roads
+            for road in self.roads:  # only include curbs of ordinary roads
                 if road.forwardLanes:
                     edges.append(road.forwardLanes.curb)
                 if road.backwardLanes:
                     edges.append(road.backwardLanes.curb)
             self.curbRegion = PolylineRegion.unionAll(edges)
 
         if self.roadDirection is None:
             # TODO replace with a PolygonalVectorField for better pruning
-            self.roadDirection = VectorField('roadDirection', self._defaultRoadDirection)
+            self.roadDirection = VectorField("roadDirection", self._defaultRoadDirection)
+
+        # Build R-tree for faster lookup of roads, etc. at given points
+        self._uidForIndex = tuple(self.elements)
+        self._rtree = shapely.STRtree([elem.polygons for elem in self.elements.values()])
 
     def _defaultRoadDirection(self, point):
         """Default value for the `roadDirection` vector field.
 
         :meta private:
         """
         point = _toVector(point)
         road = self.roadAt(point)
         return 0 if road is None else road.orientation[point]
 
     #: File extension for cached versions of processed networks.
-    pickledExt = '.snet'
+    pickledExt = ".snet"
 
     @classmethod
     def _currentFormatVersion(cls):
         """Version number for the road network format.
 
         Should be incremented whenever attributes of `Network`, `NetworkElement`, etc.,
         attributes of the underlying Regions, or the serialization process itself are
         changed, so that cached networks will be properly regenerated (rather than being
         unpickled in an inconsistent state and causing errors later). Changes to the map
         geometry calculations should be included, even if the format itself is unchanged.
 
         :meta private:
         """
-        return 17
+        return 29
 
     class DigestMismatchError(Exception):
         """Exception raised when loading a cached map not matching the original file."""
+
         pass
 
     @classmethod
-    def fromFile(cls, path, useCache:bool = True, writeCache:bool = True, **kwargs):
+    def fromFile(cls, path, useCache: bool = True, writeCache: bool = True, **kwargs):
         """Create a `Network` from a map file.
 
         This function calls an appropriate parsing routine based on the extension of the
         given file. Supported map formats are:
 
             * OpenDRIVE (``.xodr``): `Network.fromOpenDrive`
 
@@ -900,178 +1003,206 @@
         Raises:
             FileNotFoundError: no readable map was found at the given path.
             ValueError: the given map is of an unknown format.
         """
         path = pathlib.Path(path)
         ext = path.suffix
 
-        handlers = {    # in order of decreasing priority
-            '.xodr': cls.fromOpenDrive,         # OpenDRIVE
-
+        handlers = {  # in order of decreasing priority
+            ".xodr": cls.fromOpenDrive,  # OpenDRIVE
             # Pickled native representation; this is the lowest priority, since original
             # maps should take precedence, but if the pickled version exists and matches
             # the original, we'll use it.
-            cls.pickledExt: cls.fromPickle
+            cls.pickledExt: cls.fromPickle,
         }
 
-        if not ext:     # no extension was given; search through possible formats
+        if not ext:  # no extension was given; search through possible formats
             found = False
             for ext in handlers:
                 newPath = path.with_suffix(ext)
                 if newPath.exists():
                     path = newPath
                     found = True
                     break
             if not found:
-                raise FileNotFoundError(f'no readable maps found for path {path}')
+                raise FileNotFoundError(f"no readable maps found for path {path}")
         elif ext not in handlers:
-            raise ValueError(f'unknown type of road network file {path}')
+            raise ValueError(f"unknown type of road network file {path}")
 
         # If we don't have an underlying map file, return the pickled version directly
         if ext == cls.pickledExt:
             return cls.fromPickle(path)
 
         # Otherwise, hash the underlying file to detect when the pickle is outdated
-        with open(path, 'rb') as f:
+        with open(path, "rb") as f:
             data = f.read()
         digest = hashlib.blake2b(data).digest()
 
         # By default, use the pickled version if it exists and is not outdated
         pickledPath = path.with_suffix(cls.pickledExt)
         if useCache and pickledPath.exists():
             try:
                 return cls.fromPickle(pickledPath, originalDigest=digest)
             except pickle.UnpicklingError:
-                verbosePrint('Unable to load cached network (old format or corrupted).')
+                verbosePrint("Unable to load cached network (old format or corrupted).")
             except cls.DigestMismatchError:
-                verbosePrint('Cached network does not match original file; ignoring it.')
+                verbosePrint("Cached network does not match original file; ignoring it.")
 
         # Not using the pickled version; parse the original file based on its extension
         network = handlers[ext](path, **kwargs)
         if writeCache:
-            verbosePrint(f'Caching road network in {cls.pickledExt} file.')
+            verbosePrint(f"Caching road network in {cls.pickledExt} file.")
             network.dumpPickle(path.with_suffix(cls.pickledExt), digest)
         return network
 
     @classmethod
-    def fromOpenDrive(cls, path, ref_points:int = 20, tolerance:float = 0.05,
-                      fill_gaps:bool = True, fill_intersections:bool = True,
-                      elide_short_roads:bool = False):
+    def fromOpenDrive(
+        cls,
+        path,
+        ref_points: int = 20,
+        tolerance: float = 0.05,
+        fill_gaps: bool = True,
+        fill_intersections: bool = True,
+        elide_short_roads: bool = False,
+    ):
         """Create a `Network` from an OpenDRIVE file.
 
         Args:
             path: Path to the file, as in `Network.fromFile`.
             ref_points: Number of points to discretize continuous reference lines
                 into.
             tolerance: Tolerance for merging nearby geometries.
             fill_gaps: Whether to attempt to fill gaps between adjacent lanes.
             fill_intersections: Whether to attempt to fill gaps inside
                 intersections.
             elide_short_roads: Whether to attempt to fix geometry artifacts by
                 eliding roads with length less than **tolerance**.
         """
         import scenic.formats.opendrive.xodr_parser as xodr_parser
-        road_map = xodr_parser.RoadMap(tolerance=tolerance,
-                                       fill_intersections=fill_intersections,
-                                       elide_short_roads=elide_short_roads)
+
+        road_map = xodr_parser.RoadMap(
+            tolerance=tolerance,
+            fill_intersections=fill_intersections,
+            elide_short_roads=elide_short_roads,
+        )
         startTime = time.time()
-        verbosePrint('Parsing OpenDRIVE file...')
+        verbosePrint("Parsing OpenDRIVE file...")
         road_map.parse(path)
-        verbosePrint('Computing road geometry... (this may take a while)')
+        verbosePrint("Computing road geometry... (this may take a while)")
         road_map.calculate_geometry(ref_points, calc_gap=fill_gaps, calc_intersect=True)
         network = road_map.toScenicNetwork()
         totalTime = time.time() - startTime
-        verbosePrint(f'Finished loading OpenDRIVE map in {totalTime:.2f} seconds.')
+        verbosePrint(f"Finished loading OpenDRIVE map in {totalTime:.2f} seconds.")
         return network
 
     @classmethod
     def fromPickle(cls, path, originalDigest=None):
         startTime = time.time()
-        verbosePrint('Loading cached version of road network...')
+        verbosePrint("Loading cached version of road network...")
 
-        with open(path, 'rb') as f:
+        with open(path, "rb") as f:
             versionField = f.read(4)
             if len(versionField) != 4:
-                raise pickle.UnpicklingError(f'{cls.pickledExt} file is corrupted')
-            version = struct.unpack('<I', versionField)
+                raise pickle.UnpicklingError(f"{cls.pickledExt} file is corrupted")
+            version = struct.unpack("<I", versionField)
             if version[0] != cls._currentFormatVersion():
-                raise pickle.UnpicklingError(f'{cls.pickledExt} file is too old; '
-                                             'regenerate it from the original map')
+                raise pickle.UnpicklingError(
+                    f"{cls.pickledExt} file is too old; "
+                    "regenerate it from the original map"
+                )
             digest = f.read(64)
             if len(digest) != 64:
-                raise pickle.UnpicklingError(f'{cls.pickledExt} file is corrupted')
+                raise pickle.UnpicklingError(f"{cls.pickledExt} file is corrupted")
             if originalDigest and originalDigest != digest:
                 raise cls.DigestMismatchError(
-                    f'{cls.pickledExt} file does not correspond to the original map; '
-                    ' regenerate it'
+                    f"{cls.pickledExt} file does not correspond to the original map; "
+                    " regenerate it"
                 )
             with gzip.open(f) as gf:
                 try:
-                    network = pickle.load(gf)
+                    network = pickle.load(gf)  # invokes __setstate__ below
                 except pickle.UnpicklingError:
-                    raise    # propagate unpickling errors
+                    raise  # propagate unpickling errors
                 except Exception as e:
                     # convert various other ways unpickling can fail into a more
                     # standard exception
-                    raise pickle.UnpicklingError('unpickling failed') from e
+                    raise pickle.UnpicklingError("unpickling failed") from e
+
+        totalTime = time.time() - startTime
+        verbosePrint(f"Loaded cached network in {totalTime:.2f} seconds.")
+        return network
+
+    def __setstate__(self, state):
+        # Restore our attributes (default behavior when __setstate__ isn't defined)
+        self.__dict__.update(state)
 
         # Reconnect links between network elements
         def reconnect(thing):
             state = thing.__dict__
             for key, value in state.items():
                 if isinstance(value, _ElementPlaceholder):
-                    state[key] = network.elements[value.uid]
-        proxy = weakref.proxy(network)
-        for elem in network.elements.values():
+                    state[key] = self.elements[value.uid]
+
+        proxy = weakref.proxy(self)
+        for elem in self.elements.values():
             reconnect(elem)
             elem.network = proxy
-        for elem in itertools.chain(network.lanes, network.intersections):
+        for elem in itertools.chain(self.lanes, self.intersections):
             for maneuver in elem.maneuvers:
                 reconnect(maneuver)
 
-        totalTime = time.time() - startTime
-        verbosePrint(f'Loaded cached network in {totalTime:.2f} seconds.')
-        return network
-
     def dumpPickle(self, path, digest):
         path = pathlib.Path(path)
         if not path.suffix:
             path = path.with_suffix(self.pickledExt)
-        version = struct.pack('<I', self._currentFormatVersion())
+        version = struct.pack("<I", self._currentFormatVersion())
         data = pickle.dumps(self)
-        with open(path, 'wb') as f:
-            f.write(version)    # uncompressed in case we change compression schemes later
-            f.write(digest)     # uncompressed for quick lookup
-            with gzip.open(f, 'wb') as gf:
+        with open(path, "wb") as f:
+            f.write(version)  # uncompressed in case we change compression schemes later
+            f.write(digest)  # uncompressed for quick lookup
+            with gzip.open(f, "wb") as gf:
                 gf.write(data)
 
     @distributionMethod
-    def findPointIn(self, point: Vectorlike,
-                    elems: Sequence[NetworkElement],
-                    reject: Union[bool, str]) -> Union[NetworkElement, None]:
+    def findPointIn(
+        self, point: Vectorlike, elems: Sequence[NetworkElement], reject: Union[bool, str]
+    ) -> Union[NetworkElement, None]:
         """Find the first of the given elements containing the point.
 
         Elements which *actually* contain the point have priority; if none contain the
         point, then we search again allowing an error of up to **tolerance**. If there
         are still no matches, we return None, unless **reject** is true, in which case we
         reject the current sample.
         """
-        point = _toVector(point)
-        for element in elems:
-            if element.containsPoint(point):
-                return element
-        if self.tolerance > 0:
-            for element in elems:
-                if element.distanceTo(point) <= self.tolerance:
-                    return element
+        point = shapely.geometry.Point(_toVector(point))
+
+        def findElementWithin(distance):
+            target = point if distance == 0 else point.buffer(distance)
+            indices = self._rtree.query(target, predicate="intersects")
+            candidates = {self._uidForIndex[index] for index in indices}
+            if candidates:
+                for elem in elems:
+                    if elem.uid in candidates:
+                        return elem
+            return None
+
+        # First pass: check for elements containing the point.
+        if elem := findElementWithin(0):
+            return elem
+
+        # Second pass: check for elements within tolerance of the point.
+        if self.tolerance > 0 and (elem := findElementWithin(self.tolerance)):
+            return elem
+
+        # No matches found.
         if reject:
             if isinstance(reject, str):
                 message = reject
             else:
-                message = 'requested element does not exist'
+                message = "requested element does not exist"
             _rejectSample(message)
         return None
 
     def _findPointInAll(self, point, things, key=lambda e: e):
         point = _toVector(point)
         found = []
         for thing in things:
@@ -1118,70 +1249,86 @@
     def laneGroupAt(self, point: Vectorlike, reject=False) -> Union[LaneGroup, None]:
         """Get the `LaneGroup` passing through a given point."""
         point = _toVector(point)
         road = self.roadAt(point, reject=reject)
         return None if road is None else road.laneGroupAt(point, reject=reject)
 
     @distributionMethod
-    def crossingAt(self, point: Vectorlike,
-                   reject=False) -> Union[PedestrianCrossing, None]:
+    def crossingAt(
+        self, point: Vectorlike, reject=False
+    ) -> Union[PedestrianCrossing, None]:
         """Get the `PedestrianCrossing` passing through a given point."""
         point = _toVector(point)
         road = self.roadAt(point, reject=reject)
         return None if road is None else road.crossingAt(point, reject=reject)
 
     @distributionMethod
-    def intersectionAt(self, point: Vectorlike,
-                       reject=False) -> Union[Intersection, None]:
+    def intersectionAt(
+        self, point: Vectorlike, reject=False
+    ) -> Union[Intersection, None]:
         """Get the `Intersection` at a given point."""
         return self.findPointIn(point, self.intersections, reject)
 
     @distributionMethod
-    def nominalDirectionsAt(self, point: Vectorlike, reject=False) -> Tuple[float]:
+    def nominalDirectionsAt(self, point: Vectorlike, reject=False) -> Tuple[Orientation]:
         """Get the nominal traffic direction(s) at a given point, if any.
 
         There can be more than one such direction in an intersection, for example: a car
         at a given point could be going straight, turning left, etc.
         """
         inter = self.intersectionAt(point)
         if inter is not None:
             return inter.nominalDirectionsAt(point)
         road = self.roadAt(point, reject=reject)
         if road is not None:
             return road.nominalDirectionsAt(point)
         return ()
 
-    def show(self):
+    def show(self, labelIncomingLanes=False):
         """Render a schematic of the road network for debugging.
 
         If you call this function directly, you'll need to subsequently call
         `matplotlib.pyplot.show` to actually display the diagram.
+
+        Args:
+            labelIncomingLanes (bool): Whether to label the incoming lanes of
+                intersections with their indices in ``incomingLanes``.
         """
         import matplotlib.pyplot as plt
-        self.walkableRegion.show(plt, style='-', color='#00A0FF')
-        self.shoulderRegion.show(plt, style='-', color='#606060')
+
+        self.walkableRegion.show(plt, style="-", color="#00A0FF")
+        self.shoulderRegion.show(plt, style="-", color="#606060")
         for road in self.roads:
-            road.show(plt, style='r-')
-            for lane in road.lanes:     # will loop only over lanes of main roads
-                lane.leftEdge.show(plt, style='r--')
-                lane.rightEdge.show(plt, style='r--')
+            road.show(plt, style="r-")
+            for lane in road.lanes:  # will loop only over lanes of main roads
+                lane.leftEdge.show(plt, style="r--")
+                lane.rightEdge.show(plt, style="r--")
 
                 # Draw arrows indicating road direction
                 if lane.centerline.length >= 40:
-                    pts = lane.centerline.equallySpacedPoints(20)
+                    pts = lane.centerline.pointsSeparatedBy(20)
                 else:
                     pts = [lane.centerline.pointAlongBy(0.5, normalized=True)]
-                hs = [lane.centerline.orientation[pt] for pt in pts]
-                x, y = zip(*pts)
-                u = [math.cos(h + (math.pi/2)) for h in hs]
-                v = [math.sin(h + (math.pi/2)) for h in hs]
-                plt.quiver(x, y, u, v,
-                           pivot='middle', headlength=4.5,
-                           scale=0.06, units='dots', color='#A0A0A0')
-        for lane in self.lanes:     # draw centerlines of all lanes (including connecting)
-            lane.centerline.show(plt, style=':', color='#A0A0A0')
-        self.intersectionRegion.show(plt, style='g')
-        # for intersection in self.intersections:
-        #     for i, lane in enumerate(intersection.incomingLanes):
-        #         x, y = lane.centerline[-1]
-        #         plt.plot([x], [y], '*b')
-        #         plt.annotate(str(i), (x, y))
+                hs = [lane.centerline.orientation[pt].yaw for pt in pts]
+                x, y, _ = zip(*pts)
+                u = [math.cos(h + (math.pi / 2)) for h in hs]
+                v = [math.sin(h + (math.pi / 2)) for h in hs]
+                plt.quiver(
+                    x,
+                    y,
+                    u,
+                    v,
+                    pivot="middle",
+                    headlength=4.5,
+                    scale=0.06,
+                    units="dots",
+                    color="#A0A0A0",
+                )
+        for lane in self.lanes:  # draw centerlines of all lanes (including connecting)
+            lane.centerline.show(plt, style=":", color="#A0A0A0")
+        self.intersectionRegion.show(plt, style="g")
+        if labelIncomingLanes:
+            for intersection in self.intersections:
+                for i, lane in enumerate(intersection.incomingLanes):
+                    x, y, _ = lane.centerline[-1]
+                    plt.plot([x], [y], "*b")
+                    plt.annotate(str(i), (x, y))
```

### Comparing `scenic-2.1.0b4/src/scenic/domains/driving/simulators.py` & `scenic-3.0.0b2/src/scenic/domains/driving/simulators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-
 """Abstract interface to simulators supporting the driving domain."""
 
-from scenic.core.simulators import Simulator, Simulation
-from scenic.domains.driving.controllers import PIDLongitudinalController, PIDLateralController
+from scenic.core.simulators import Simulation, Simulator
+from scenic.domains.driving.controllers import (
+    PIDLateralController,
+    PIDLongitudinalController,
+)
+
 
 class DrivingSimulator(Simulator):
     """A `Simulator` supporting the driving domain."""
-    def createSimulation(self, scene):
-        raise NotImplementedError
+
+    pass
+
 
 class DrivingSimulation(Simulation):
     """A `Simulation` with a simulator supporting the driving domain.
 
     This subclass of `Simulation` provides no special behavior by itself; it
     just provides convenience methods for creating controllers to be used by
     `FollowLaneBehavior` and related behaviors, so that the parameters of these
@@ -30,32 +34,38 @@
             A pair of controllers for throttle and steering respectively.
         """
         dt = self.timestep
         if agent.isCar:
             lon_controller = PIDLongitudinalController(K_P=0.5, K_D=0.1, K_I=0.7, dt=dt)
             lat_controller = PIDLateralController(K_P=0.2, K_D=0.1, K_I=0.0, dt=dt)
         else:
-            lon_controller = PIDLongitudinalController(K_P=0.25, K_D=0.025, K_I=0.0, dt=dt)
+            lon_controller = PIDLongitudinalController(
+                K_P=0.25, K_D=0.025, K_I=0.0, dt=dt
+            )
             lat_controller = PIDLateralController(K_P=0.2, K_D=0.1, K_I=0.0, dt=dt)
         return lon_controller, lat_controller
 
     def getTurningControllers(self, agent):
         """Get longitudinal and lateral controllers for turning."""
         dt = self.timestep
         if agent.isCar:
             lon_controller = PIDLongitudinalController(K_P=0.5, K_D=0.1, K_I=0.7, dt=dt)
             lat_controller = PIDLateralController(K_P=0.8, K_D=0.2, K_I=0.0, dt=dt)
         else:
-            lon_controller = PIDLongitudinalController(K_P=0.25, K_D=0.025, K_I=0.0, dt=dt)
+            lon_controller = PIDLongitudinalController(
+                K_P=0.25, K_D=0.025, K_I=0.0, dt=dt
+            )
             lat_controller = PIDLateralController(K_P=0.4, K_D=0.1, K_I=0.0, dt=dt)
         return lon_controller, lat_controller
 
     def getLaneChangingControllers(self, agent):
         """Get longitudinal and lateral controllers for lane changing."""
         dt = self.timestep
         if agent.isCar:
             lon_controller = PIDLongitudinalController(K_P=0.5, K_D=0.1, K_I=0.7, dt=dt)
             lat_controller = PIDLateralController(K_P=0.08, K_D=0.3, K_I=0.0, dt=dt)
         else:
-            lon_controller = PIDLongitudinalController(K_P=0.25, K_D=0.025, K_I=0.0, dt=dt)
+            lon_controller = PIDLongitudinalController(
+                K_P=0.25, K_D=0.025, K_I=0.0, dt=dt
+            )
             lat_controller = PIDLateralController(K_P=0.1, K_D=0.3, K_I=0.0, dt=dt)
         return lon_controller, lat_controller
```

### Comparing `scenic-2.1.0b4/src/scenic/formats/opendrive/workspace.py` & `scenic-3.0.0b2/src/scenic/formats/opendrive/workspace.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 """Workspaces based on OpenDRIVE maps."""
 
-from .xodr_parser import RoadMap
-from scenic.core.workspaces import Workspace
-from scenic.core.regions import regionFromShapelyObject, nowhere
+from scenic.core.regions import nowhere, regionFromShapelyObject
 from scenic.core.vectors import VectorField
+from scenic.core.workspaces import Workspace
+
+from .xodr_parser import RoadMap
+
 
 class OpenDriveWorkspace(Workspace):
     def __init__(self, path, n=20, tolerance=None):
-        '''Initialize from OpenDRIVE file at @path, with
-        @n points per lane section reference line.'''
+        """Initialize from OpenDRIVE file at @path, with
+        @n points per lane section reference line."""
         self.road_map = RoadMap(tolerance=tolerance)
         self.road_map.parse(path)
         self.road_map.calculate_geometry(n, calc_intersect=True)
         drivable_poly = self.road_map.drivable_region
         sidewalk_poly = self.road_map.sidewalk_region
         intersect_poly = self.road_map.intersection_region
-        self.road_direction = VectorField('Road Direction',
-                                          self.road_map.heading_at)
-        self.drivable_region = regionFromShapelyObject(drivable_poly,
-                                                       orientation=self.road_direction)
+        self.road_direction = VectorField("Road Direction", self.road_map.heading_at)
+        self.drivable_region = regionFromShapelyObject(
+            drivable_poly, orientation=self.road_direction
+        )
         self.sidewalk_region = regionFromShapelyObject(sidewalk_poly)
-        self.intersection_region = regionFromShapelyObject(intersect_poly,
-                                                           orientation=self.road_direction)
+        self.intersection_region = regionFromShapelyObject(
+            intersect_poly, orientation=self.road_direction
+        )
         super().__init__()
 
         # lane_sec_dict is dict of road id to list of dict of lane id to Region.
         self.lane_sec_dict = {}
         for id_ in self.road_map.roads:
             lane_dicts = []
             for d in self.road_map.roads[id_].sec_lane_polys:
-                lane_dicts.append({i: regionFromShapelyObject(d[i],
-                                                              orientation=self.road_direction)
-                                   for i in d.keys()})
+                lane_dicts.append(
+                    {
+                        i: regionFromShapelyObject(d[i], orientation=self.road_direction)
+                        for i in d.keys()
+                    }
+                )
             self.lane_sec_dict[id_] = lane_dicts
 
     def show(self, plt):
         self.drivable_region.show(plt)
-        self.sidewalk_region.show(plt, style='b')
-        self.intersection_region.show(plt, style='g')
+        self.sidewalk_region.show(plt, style="b")
+        self.intersection_region.show(plt, style="g")
```

### Comparing `scenic-2.1.0b4/src/scenic/formats/opendrive/xodr_parser.py` & `scenic-3.0.0b2/src/scenic/formats/opendrive/xodr_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,149 +1,178 @@
 """Parser for OpenDRIVE (.xodr) files."""
 
-import math
+import abc
+from collections import defaultdict
 import itertools
+import math
 import warnings
 import xml.etree.ElementTree as ET
-import numpy as np
-from scipy.integrate import quad
-from scipy.integrate import solve_ivp
-from pynverse import inversefunc
-from shapely.geometry import Polygon, MultiPolygon, GeometryCollection, Point, MultiPoint
-from shapely.ops import unary_union, snap
-import abc
-from collections import defaultdict
 
+import numpy as np
+from scipy.integrate import quad, solve_ivp
+from scipy.optimize import brentq
+from shapely.geometry import GeometryCollection, MultiPoint, MultiPolygon, Point, Polygon
+from shapely.ops import snap, unary_union
+
+from scenic.core.geometry import (
+    averageVectors,
+    cleanChain,
+    cleanPolygon,
+    plotPolygon,
+    polygonUnion,
+    removeHoles,
+)
 from scenic.core.regions import PolygonalRegion, PolylineRegion
-from scenic.core.geometry import (polygonUnion, cleanPolygon, cleanChain, plotPolygon,
-                                  removeHoles, averageVectors)
 from scenic.core.vectors import Vector
 from scenic.domains.driving import roads as roadDomain
 
+
 class OpenDriveWarning(UserWarning):
     pass
 
+
 def warn(message):
     warnings.warn(message, OpenDriveWarning, stacklevel=2)
 
+
 def buffer_union(polys, tolerance=0.01):
     return polygonUnion(polys, buf=tolerance, tolerance=tolerance)
 
+
 class Poly3:
-    '''Cubic polynomial.'''
+    """Cubic polynomial."""
+
     def __init__(self, a, b, c, d):
         self.a = a
         self.b = b
         self.c = c
         self.d = d
 
     def eval_at(self, x):
-        return self.a + self.b * x + self.c * x ** 2 + self.d * x ** 3
+        return self.a + self.b * x + self.c * x**2 + self.d * x**3
 
     def grad_at(self, x):
-        return self.b + 2 * self.c * x + 3 * self.d * x ** 2
+        return self.b + 2 * self.c * x + 3 * self.d * x**2
 
 
 class Curve:
-    ''' Geometric elements which compose road reference lines.
-    See the OpenDRIVE Format Specification for coordinate system details.'''
+    """Geometric elements which compose road reference lines.
+    See the OpenDRIVE Format Specification for coordinate system details."""
+
     def __init__(self, x0, y0, hdg, length):
         self.x0 = x0
         self.y0 = y0
-        self.hdg = hdg    # In radians counterclockwise, 0 at positive x-axis.
+        self.hdg = hdg  # In radians counterclockwise, 0 at positive x-axis.
         self.cos_hdg, self.sin_hdg = math.cos(hdg), math.sin(hdg)
         self.length = length
 
     def to_points(self, num, extra_points=[]):
-        '''Sample NUM evenly-spaced points from curve.
+        """Sample NUM evenly-spaced points from curve.
 
         Points are tuples of (x, y, s) with (x, y) absolute coordinates
         and s the arc length along the curve. Additional points at s values in
         extra_points are included if they are contained in the curve (unless
         they are extremely close to one of the equally-spaced points).
-        '''
+        """
         s_vals = []
-        extras = itertools.chain(extra_points, itertools.repeat(float('inf')))
+        extras = itertools.chain(extra_points, itertools.repeat(float("inf")))
         next_extra = next(extras)
         last_s = 0
         for s in np.linspace(0, self.length, num=num):
             while next_extra <= s:
                 if last_s + 1e-6 < next_extra < s - 1e-6:
                     s_vals.append(next_extra)
                 next_extra = next(extras)
             s_vals.append(s)
             last_s = s
         return [self.point_at(s) for s in s_vals]
 
     @abc.abstractmethod
     def point_at(self, s):
-        '''Get an (x, y, s) point along the curve at the given s coordinate.'''
+        """Get an (x, y, s) point along the curve at the given s coordinate."""
         return
 
     def rel_to_abs(self, point):
-        '''Convert from relative coordinates of curve to absolute coordinates.
-        I.e. rotate counterclockwise by self.hdg and translate by (x0, x1).'''
+        """Convert from relative coordinates of curve to absolute coordinates.
+        I.e. rotate counterclockwise by self.hdg and translate by (x0, x1)."""
         x, y, s = point
-        return (self.x0 + self.cos_hdg * x - self.sin_hdg * y,
-                self.y0 + self.sin_hdg * x + self.cos_hdg * y,
-                s)
+        return (
+            self.x0 + self.cos_hdg * x - self.sin_hdg * y,
+            self.y0 + self.sin_hdg * x + self.cos_hdg * y,
+            s,
+        )
 
 
 class Cubic(Curve):
-    '''A curve defined by the cubic polynomial a + bu + cu^2 + du^3.
-    The curve starts at (X0, Y0) in direction HDG, with length LENGTH.'''
+    """A curve defined by the cubic polynomial a + bu + cu^2 + du^3.
+    The curve starts at (X0, Y0) in direction HDG, with length LENGTH."""
+
     def __init__(self, x0, y0, hdg, length, a, b, c, d):
         super().__init__(x0, y0, hdg, length)
         self.poly = Poly3(a, b, c, d)
+        # Crude upper bound for u (used to bracket u for a given s in point_at)
+        if d != 0:
+            self.ubound = max(
+                2 * abs(c / d), abs(b / d) ** 0.5, (3 * length / abs(d)) ** (1 / 3)
+            )
+        elif c != 0:
+            self.ubound = max(abs(b / c), (2 * length / abs(c)) ** 0.5)
+        else:
+            self.ubound = length / abs(b)
 
     def arclength(self, u):
         d_arc = lambda x: np.sqrt(1 + self.poly.grad_at(x) ** 2)
         return quad(d_arc, 0, u)[0]
 
     def point_at(self, s):
-        u = float(inversefunc(self.arclength, s))
+        # Use Brent's method to find parameter u corresponding to arclength s;
+        # (N.B. Brent's method proved to be faster than Newton's and has no potential
+        # convergence issues.)
+        root_func = lambda x: self.arclength(x) - s
+        u = float(brentq(root_func, 0, self.ubound))
         pt = (s, self.poly.eval_at(u), s)
         return self.rel_to_abs(pt)
 
 
 class ParamCubic(Curve):
-    ''' A curve defined by the parametric equations
+    """A curve defined by the parametric equations
     u = a_u + b_up + c_up^2 + d_up^3,
     v = a_v + b_vp + c_vp^2 + d_up^3,
     with p in [0, p_range].
-    The curve starts at (X0, Y0) in direction HDG, with length LENGTH.'''
-    def __init__(self, x0, y0, hdg, length,
-                 au, bu, cu, du, av, bv, cv, dv, p_range=1):
+    The curve starts at (X0, Y0) in direction HDG, with length LENGTH."""
+
+    def __init__(self, x0, y0, hdg, length, au, bu, cu, du, av, bv, cv, dv, p_range=1):
         super().__init__(x0, y0, hdg, length)
         self.u_poly = Poly3(au, bu, cu, du)
         self.v_poly = Poly3(av, bv, cv, dv)
         self.p_range = p_range if p_range else 1
 
     def arclength(self, p):
-        d_arc = lambda x: math.hypot(self.u_poly.grad_at(x),
-                                     self.v_poly.grad_at(x))
+        d_arc = lambda x: math.hypot(self.u_poly.grad_at(x), self.v_poly.grad_at(x))
         return quad(d_arc, 0, p)[0]
 
     def point_at(self, s):
-        p = float(inversefunc(self.arclength, s))
+        root_func = lambda x: self.arclength(x) - s
+        p = float(brentq(root_func, 0, self.p_range))
         pt = (self.u_poly.eval_at(p), self.v_poly.eval_at(p), s)
         return self.rel_to_abs(pt)
 
 
 class Clothoid(Curve):
-    '''An Euler spiral with curvature varying linearly between CURV0 and CURV1.
-    The spiral starts at (X0, Y0) in direction HDG, with length LENGTH.'''
+    """An Euler spiral with curvature varying linearly between CURV0 and CURV1.
+    The spiral starts at (X0, Y0) in direction HDG, with length LENGTH."""
+
     def __init__(self, x0, y0, hdg, length, curv0, curv1):
         super().__init__(x0, y0, hdg, length)
         # Initial and final curvature.
         self.curv0 = curv0
         self.curv1 = curv1
         self.curve_rate = (curv1 - curv0) / length
         self.a = abs(curv0)
-        self.r = 1 / self.a if curv0 != 0 else 1    # value not used if curv0 == 0
+        self.r = 1 / self.a if curv0 != 0 else 1  # value not used if curv0 == 0
         self.ode_init = np.array([x0, y0, hdg])
 
     def point_at(self, s):
         # Generate a origin-centered clothoid with zero curvature at origin,
         # then translate/rotate the relevant segment.
         # Arcs are just a degenerate clothoid:
         if self.curv0 == self.curv1:
@@ -154,102 +183,110 @@
                 th = s * self.a
                 if self.curv0 > 0:
                     pt = (r * math.sin(th), r - r * math.cos(th), s)
                 else:
                     pt = (r * math.sin(th), -r + r * math.cos(th), s)
             return self.rel_to_abs(pt)
         else:
+
             def clothoid_ode(s, state):
                 x, y, theta = state
-                return np.array([math.cos(theta), math.sin(theta),
-                                self.curv0 + (self.curve_rate * s)])
+                return np.array(
+                    [math.cos(theta), math.sin(theta), self.curv0 + (self.curve_rate * s)]
+                )
+
             sol = solve_ivp(clothoid_ode, (0, s), self.ode_init)
-            x, y, hdg = sol.y[:,-1]
+            x, y, hdg = sol.y[:, -1]
             return (x, y, s)
 
+
 class Line(Curve):
-    '''A line segment between (x0, y0) and (x1, y1).'''
+    """A line segment between (x0, y0) and (x1, y1)."""
+
     def __init__(self, x0, y0, hdg, length):
         super().__init__(x0, y0, hdg, length)
         # Endpoints of line.
         self.x1 = x0 + length * math.cos(hdg)
         self.y1 = y0 + length * math.sin(hdg)
 
     def point_at(self, s):
         return self.rel_to_abs((s, 0, s))
 
 
-class Lane():
+class Lane:
     def __init__(self, id_, type_, pred=None, succ=None):
         self.id_ = id_
-        self.width = []    # List of tuples (Poly3, int) for width and s-offset.
+        self.width = []  # List of tuples (Poly3, int) for width and s-offset.
         self.type_ = type_
         self.pred = pred
         self.succ = succ
-        self.left_bounds = []    # to be filled in later
+        self.left_bounds = []  # to be filled in later
         self.right_bounds = []
         self.centerline = []
         self.parent_lane_poly = None
 
     def width_at(self, s):
         # S here is relative to start of LaneSection this lane is in.
         ind = 0
         while ind + 1 < len(self.width) and self.width[ind + 1][1] <= s:
             ind += 1
-        assert self.width[ind][1] <= s, 'No matching width entry found.'
+        assert self.width[ind][1] <= s, "No matching width entry found."
         w_poly, s_off = self.width[ind]
         w = w_poly.eval_at(s - s_off)
-        if w < -1e-6:    # allow for numerical error
-            raise RuntimeError('OpenDRIVE lane has negative width')
+        if w < -1e-6:  # allow for numerical error
+            raise RuntimeError("OpenDRIVE lane has negative width")
         return max(w, 0)
 
 
-class LaneSection():
+class LaneSection:
     def __init__(self, s0, left_lanes={}, right_lanes={}):
         self.s0 = s0
         self.left_lanes = left_lanes
         self.right_lanes = right_lanes
         self.left_lane_ids = sorted(self.left_lanes.keys())
         self.right_lane_ids = sorted(self.right_lanes.keys(), reverse=True)
         self.lanes = dict(list(left_lanes.items()) + list(right_lanes.items()))
 
     def get_lane(self, id_):
         if id_ in self.left_lanes:
             return self.left_lanes[id_]
         elif id_ in self.right_lanes:
             return self.right_lanes[id_]
         elif id_ == 0:
-            return Lane(0, 'none')
+            return Lane(0, "none")
         else:
-            raise RuntimeError('Lane with id', id_, 'not found')
+            raise RuntimeError("Lane with id", id_, "not found")
 
     def get_offsets(self, s):
-        '''Returns dict of lane id and offset from
+        """Returns dict of lane id and offset from
         reference line of lane boundary at coordinate S along line.
         By convention, left lanes have positive width offset and right lanes
-        have negative.'''
-        assert s >= self.s0, 'Input s is before lane start position.'
+        have negative."""
+        assert s >= self.s0, "Input s is before lane start position."
         offsets = {}
         for lane_id in self.left_lane_ids:
             if lane_id - 1 in self.left_lane_ids:
-                offsets[lane_id] = offsets[lane_id - 1] \
-                    + self.left_lanes[lane_id].width_at(s - self.s0)
+                offsets[lane_id] = offsets[lane_id - 1] + self.left_lanes[
+                    lane_id
+                ].width_at(s - self.s0)
             else:
                 offsets[lane_id] = self.left_lanes[lane_id].width_at(s - self.s0)
         for lane_id in self.right_lane_ids:
             if lane_id + 1 in self.right_lane_ids:
-                offsets[lane_id] = offsets[lane_id + 1] \
-                    - self.right_lanes[lane_id].width_at(s - self.s0)
+                offsets[lane_id] = offsets[lane_id + 1] - self.right_lanes[
+                    lane_id
+                ].width_at(s - self.s0)
             else:
                 offsets[lane_id] = -self.right_lanes[lane_id].width_at(s - self.s0)
         return offsets
 
 
 class RoadLink:
-    '''Indicates Roads a and b, with ids id_a and id_b respectively, are connected.'''
+    """Indicates Roads a and b, with ids id_a and id_b respectively, are connected."""
+
     def __init__(self, id_a, id_b, contact_a, contact_b):
         self.id_a = id_a
         self.id_b = id_b
         # contact_a and contact_b should be of value "start" or "end"
         # and indicate which end of each road is connected to the other.
         self.contact_a = contact_a
         self.contact_b = contact_b
@@ -271,138 +308,121 @@
         self.name = name
         self.connections = []
         # Ids of roads that are paths within junction:
         self.paths = []
         self.poly = None
 
     def add_connection(self, incoming_id, connecting_id, connecting_contact, lane_links):
-        conn = Junction.Connection(incoming_id, connecting_id, connecting_contact, lane_links)
+        conn = Junction.Connection(
+            incoming_id, connecting_id, connecting_contact, lane_links
+        )
         self.connections.append(conn)
 
+
 class Road:
     def __init__(self, name, id_, length, junction, drive_on_right=True):
         self.name = name
         self.id_ = id_
         self.length = length
-        self.junction = junction if junction != '-1' else None
+        self.junction = junction if junction != "-1" else None
         self.predecessor = None
         self.successor = None
-        self.signals = []    # List of Signal objects.
-        self.lane_secs = []    # List of LaneSection objects.
-        self.ref_line = []    # List of Curve objects defining reference line.
+        self.signals = []  # List of Signal objects.
+        self.lane_secs = []  # List of LaneSection objects.
+        self.ref_line = []  # List of Curve objects defining reference line.
         # NOTE: sec_points, sec_polys, sec_lane_polys should be ordered according to lane_secs.
-        self.sec_points = []   # List of lists of points, one for each LaneSection.
-        self.sec_polys = []   # List of Polygons, one for each LaneSections.
-        self.sec_lane_polys = []    # List of dict of lane id to Polygon for each LaneSection.
-        self.lane_polys = []    # List of lane polygons. Not a dict b/c lane id is not unique along road.
+        self.sec_points = []  # List of lists of points, one for each LaneSection.
+        self.sec_polys = []  # List of Polygons, one for each LaneSections.
+        # List of dict of lane id to Polygon for each LaneSection.
+        self.sec_lane_polys = []
+        # List of lane polygons. Not a dict b/c lane id is not unique along road.
+        self.lane_polys = []
         # Each polygon in lane_polys is the union of connected lane section polygons.
         # lane_polys is currently not used.
         # Reference line offset:
-        self.offset = []    # List of tuple (Poly3, s-coordinate).
+        self.offset = []  # List of tuple (Poly3, s-coordinate).
         self.drive_on_right = drive_on_right
         # Used to fill in gaps between roads:
         self.start_bounds_left = {}
         self.start_bounds_right = {}
         self.end_bounds_left = {}
         self.end_bounds_right = {}
 
-        self.remappedStartLanes = None      # hack for handling spurious initial lane sections
-
-    def get_lane(self, id_, s):
-        '''Returns Lane object with id_ at coordinate S along line.'''
-        ind = 0
-        while ind + 1 < len(self.lane_secs) and self.lane_secs[ind + 1].s0 <= s:
-            ind += 1
-        assert self.lane_secs[ind].s0 <= s, 'No matching lane section found.'
-        return self.lane_secs[ind].get_lane(id_)
+        self.remappedStartLanes = None  # hack for handling spurious initial lane sections
 
     def get_ref_line_offset(self, s):
         if not self.offset:
             return 0
         ind = 0
         while ind + 1 < len(self.offset) and self.offset[ind + 1][1] <= s:
             ind += 1
         poly, s0 = self.offset[ind]
         assert s >= s0
         return poly.eval_at(s - s0)
 
     def get_ref_points(self, num):
-        '''Returns list of list of points for each piece of ref_line.
+        """Returns list of list of points for each piece of ref_line.
         List of list structure necessary because each piece needs to be
         constructed into Polygon separately then unioned afterwards to avoid
-        self-intersecting lines.'''
+        self-intersecting lines."""
         ref_points = []
         transition_points = [sec.s0 for sec in self.lane_secs[1:]]
         last_s = 0
         for piece in self.ref_line:
             piece_points = piece.to_points(num, extra_points=transition_points)
-            assert piece_points, 'Failed to get piece points'
+            assert piece_points, "Failed to get piece points"
             if ref_points:
                 last_s = ref_points[-1][-1][2]
-                piece_points = [(p[0], p[1], p[2] + last_s)
-                                for p in piece_points]
+                piece_points = [(p[0], p[1], p[2] + last_s) for p in piece_points]
             ref_points.append(piece_points)
             transition_points = [s - last_s for s in transition_points if s > last_s]
         return ref_points
 
-    def get_lane_offsets(self, s):
-        '''Returns dict of lane id and offset from
-        reference line of lane boundary at coordinate S along line.'''
-        s = float(s)
-        ind = 0
-        while ind + 1 < len(self.lane_secs) and self.lane_secs[ind + 1].s0 <= s:
-            ind += 1
-        assert self.lane_secs[ind].s0 <= s, 'No matching lane section found.'
-        offsets = self.lane_secs[ind].get_offsets(s)
-        offsets[0] = 0    # Center lane has width 0 by convention.
-        for id_ in offsets.keys():
-            offsets[id_] += self.get_ref_line_offset(s)
-        return offsets
-
     def heading_at(self, point):
         # Convert point to shapely Point.
         point = Point(point.x, point.y)
         for i in range(len(self.lane_secs)):
             ref_points = self.sec_points[i]
             poly = self.sec_polys[i]
             if point.within(poly.buffer(1)):
                 lane_id = None
                 for id_ in self.sec_lane_polys[i].keys():
                     if point.within(self.sec_lane_polys[i][id_].buffer(1)):
                         lane_id = id_
                         break
-                assert lane_id is not None, 'Point not found in sec_lane_polys.'
-                min_dist = float('inf')
+                assert lane_id is not None, "Point not found in sec_lane_polys."
+                min_dist = float("inf")
                 for i in range(len(ref_points)):
                     cur_point = Point(ref_points[i][0], ref_points[i][1])
                     if point.distance(cur_point) < min_dist:
                         closest_idx = i
                 if closest_idx >= len(ref_points) - 1:
-                   closest_idx = len(ref_points) - 2
+                    closest_idx = len(ref_points) - 2
                 dy = ref_points[closest_idx + 1][1] - ref_points[closest_idx][1]
                 dx = ref_points[closest_idx + 1][0] - ref_points[closest_idx][0]
                 heading = math.atan2(dy, dx)
                 # Right lanes have negative lane_id.
                 # Flip heading if drive_on_right XOR right lane.
                 if self.drive_on_right != (lane_id < 0):
                     heading += math.pi
                 # Heading 0 is defined differently between OpenDrive and Scenic(?)
                 heading -= math.pi / 2
                 return (heading + math.pi) % (2 * math.pi) - math.pi
 
-        raise RuntimeError('Point not found in piece_polys')
+        raise RuntimeError("Point not found in piece_polys")
 
     def calc_geometry_for_type(self, lane_types, num, tolerance, calc_gap=False):
-        '''Given a list of lane types, returns a tuple of:
+        """Given a list of lane types, returns a tuple of:
         - List of lists of points along the reference line, with same indexing as self.lane_secs
         - List of region polygons, with same indexing as self.lane_secs
         - List of dictionary of lane id to polygon, with same indexing as self.lane_secs
         - List of polygons for each lane (not necessarily by id, but respecting lane successor/predecessor)
         - Polygon for entire region.
-        If calc_gap=True, fills in gaps between connected roads. This is fairly expensive.'''
+        If calc_gap=True, fills in gaps between connected roads. This is fairly expensive.
+        """
         road_polygons = []
         ref_points = self.get_ref_points(num)
         self.ref_line_points = list(itertools.chain.from_iterable(ref_points))
         cur_lane_polys = {}
         sec_points = []
         sec_polys = []
         sec_lane_polys = []
@@ -414,15 +434,15 @@
         for i in range(len(self.lane_secs)):
             cur_sec = self.lane_secs[i]
             cur_sec_points = []
             if i < len(self.lane_secs) - 1:
                 next_sec = self.lane_secs[i + 1]
                 s_stop = next_sec.s0
             else:
-                s_stop = float('inf')
+                s_stop = float("inf")
             left_bounds = defaultdict(list)
             right_bounds = defaultdict(list)
             cur_sec_lane_polys = defaultdict(list)
             cur_sec_polys = []
             end_of_sec = False
 
             while ref_points and not end_of_sec:
@@ -442,17 +462,22 @@
                         right = right_bounds[id_][::-1]
                         bounds = left + right
 
                         if len(bounds) < 3:
                             continue
                         poly = cleanPolygon(Polygon(bounds), tolerance)
                         if not poly.is_empty:
-                            if poly.geom_type == 'MultiPolygon':
-                                poly = MultiPolygon([p for p in poly.geoms
-                                                     if not p.is_empty and p.exterior])
+                            if poly.geom_type == "MultiPolygon":
+                                poly = MultiPolygon(
+                                    [
+                                        p
+                                        for p in poly.geoms
+                                        if not p.is_empty and p.exterior
+                                    ]
+                                )
                                 cur_sec_polys.extend(poly.geoms)
                             else:
                                 cur_sec_polys.append(poly)
                             cur_sec_lane_polys[id_].append(poly)
                         cur_last_lefts[id_] = left_bounds[id_][-1]
                         cur_last_rights[id_] = right_bounds[id_][-1]
                         if i == 0 or not self.start_bounds_left:
@@ -470,29 +495,27 @@
                     s = min(max(cur_p[2], cur_sec.s0), s_stop - 1e-6)
                     offsets = cur_sec.get_offsets(s)
                     offsets[0] = 0
                     for id_ in offsets:
                         offsets[id_] += self.get_ref_line_offset(s)
                     if len(ref_points[0]) > 1:
                         next_p = ref_points[0][1]
-                        tan_vec = (next_p[0] - cur_p[0],
-                                   next_p[1] - cur_p[1])
+                        tan_vec = (next_p[0] - cur_p[0], next_p[1] - cur_p[1])
                     else:
                         if len(cur_sec_points) >= 2:
                             prev_p = cur_sec_points[-2]
                         else:
                             assert len(sec_points) > 0
                             if sec_points[-1]:
                                 assert sec_points[-1][-1] == cur_p
                                 prev_p = sec_points[-1][-2]
                             else:
                                 prev_p = sec_points[-2][-2]
 
-                        tan_vec = (cur_p[0] - prev_p[0],
-                                   cur_p[1] - prev_p[1])
+                        tan_vec = (cur_p[0] - prev_p[0], cur_p[1] - prev_p[1])
                     tan_norm = math.hypot(tan_vec[0], tan_vec[1])
                     assert tan_norm > 1e-10
                     normal_vec = (-tan_vec[1] / tan_norm, tan_vec[0] / tan_norm)
                     if cur_p[2] < s_stop:
                         # if at end of section, keep current point to be included in
                         # the next section as well; otherwise remove it
                         ref_points[0].pop(0)
@@ -503,23 +526,29 @@
                     for id_ in offsets:
                         lane = cur_sec.get_lane(id_)
                         if lane.type_ in lane_types:
                             if id_ > 0:
                                 prev_id = id_ - 1
                             else:
                                 prev_id = id_ + 1
-                            left_bound = [cur_p[0] + normal_vec[0] * offsets[id_],
-                                          cur_p[1] + normal_vec[1] * offsets[id_]]
-                            right_bound = [cur_p[0] + normal_vec[0] * offsets[prev_id],
-                                           cur_p[1] + normal_vec[1] * offsets[prev_id]]
+                            left_bound = [
+                                cur_p[0] + normal_vec[0] * offsets[id_],
+                                cur_p[1] + normal_vec[1] * offsets[id_],
+                            ]
+                            right_bound = [
+                                cur_p[0] + normal_vec[0] * offsets[prev_id],
+                                cur_p[1] + normal_vec[1] * offsets[prev_id],
+                            ]
                             if id_ < 0:
                                 left_bound, right_bound = right_bound, left_bound
                             halfway = (offsets[id_] + offsets[prev_id]) / 2
-                            centerline = [cur_p[0] + normal_vec[0] * halfway,
-                                          cur_p[1] + normal_vec[1] * halfway]
+                            centerline = [
+                                cur_p[0] + normal_vec[0] * halfway,
+                                cur_p[1] + normal_vec[1] * halfway,
+                            ]
                             left_bounds[id_].append(left_bound)
                             right_bounds[id_].append(right_bound)
                             lane.left_bounds.append(left_bound)
                             lane.right_bounds.append(right_bound)
                             lane.centerline.append(centerline)
             assert len(cur_sec_points) >= 2, i
             sec_points.append(cur_sec_points)
@@ -529,40 +558,54 @@
                 cur_sec_lane_polys[id_] = poly
                 cur_sec.get_lane(id_).poly = poly
             sec_lane_polys.append(dict(cur_sec_lane_polys))
             next_lane_polys = {}
             for id_ in cur_sec_lane_polys:
                 pred_id = cur_sec.get_lane(id_).pred
                 if pred_id and pred_id in cur_lane_polys:
-                    next_lane_polys[id_] = cur_lane_polys.pop(pred_id) \
-                        + [cur_sec_lane_polys[id_]]
+                    next_lane_polys[id_] = cur_lane_polys.pop(pred_id) + [
+                        cur_sec_lane_polys[id_]
+                    ]
                 else:
                     next_lane_polys[id_] = [cur_sec_lane_polys[id_]]
             for id_ in cur_lane_polys:
                 poly = buffer_union(cur_lane_polys[id_], tolerance=tolerance)
                 lane_polys.append(poly)
-                self.lane_secs[i-1].get_lane(id_).parent_lane_poly = poly
+                self.lane_secs[i - 1].get_lane(id_).parent_lane_poly = poly
             cur_lane_polys = next_lane_polys
         for id_ in cur_lane_polys:
             poly = buffer_union(cur_lane_polys[id_], tolerance=tolerance)
             lane_polys.append(poly)
             cur_sec.get_lane(id_).parent_lane_poly = poly
         union_poly = buffer_union(sec_polys, tolerance=tolerance)
         if last_lefts and last_rights:
             self.end_bounds_left.update(last_lefts)
             self.end_bounds_right.update(last_rights)
         return (sec_points, sec_polys, sec_lane_polys, lane_polys, union_poly)
 
-    def calculate_geometry(self, num, tolerance, calc_gap, drivable_lane_types,
-                           sidewalk_lane_types, shoulder_lane_types):
+    def calculate_geometry(
+        self,
+        num,
+        tolerance,
+        calc_gap,
+        drivable_lane_types,
+        sidewalk_lane_types,
+        shoulder_lane_types,
+    ):
         # Note: this also calculates self.start_bounds_left, self.start_bounds_right,
         # self.end_bounds_left, self.end_bounds_right
-        (self.sec_points, self.sec_polys, self.sec_lane_polys,
-         self.lane_polys, self.drivable_region) = self.calc_geometry_for_type(
-            drivable_lane_types, num, tolerance, calc_gap=calc_gap)
+        (
+            self.sec_points,
+            self.sec_polys,
+            self.sec_lane_polys,
+            self.lane_polys,
+            self.drivable_region,
+        ) = self.calc_geometry_for_type(
+            drivable_lane_types, num, tolerance, calc_gap=calc_gap
+        )
 
         for i, sec in enumerate(self.lane_secs):
             sec.drivable_lanes = {}
             sec.sidewalk_lanes = {}
             sec.shoulder_lanes = {}
             for id_, lane in sec.lanes.items():
                 ty = lane.type_
@@ -589,73 +632,79 @@
             assert leftmost is not None, i
             sec.left_edge = leftmost.left_bounds
             assert len(sec.left_edge) >= 2
             sec.right_edge = rightmost.right_bounds
             assert len(sec.right_edge) >= 2
 
         _, _, _, _, self.sidewalk_region = self.calc_geometry_for_type(
-            sidewalk_lane_types, num, tolerance, calc_gap=calc_gap)
+            sidewalk_lane_types, num, tolerance, calc_gap=calc_gap
+        )
 
         _, _, _, _, self.shoulder_region = self.calc_geometry_for_type(
-            shoulder_lane_types, num, tolerance, calc_gap=calc_gap)
+            shoulder_lane_types, num, tolerance, calc_gap=calc_gap
+        )
 
     def toScenicRoad(self, tolerance):
         assert self.sec_points
         allElements = []
         # Create lane and road sections
         roadSections = []
         last_section = None
         sidewalkSections = defaultdict(list)
         shoulderSections = defaultdict(list)
-        for sec, pts, sec_poly, lane_polys in zip(self.lane_secs, self.sec_points,
-                                                  self.sec_polys, self.sec_lane_polys):
+        for sec, pts, sec_poly, lane_polys in zip(
+            self.lane_secs, self.sec_points, self.sec_polys, self.sec_lane_polys
+        ):
+            pts = [pt[:2] for pt in pts]  # drop s coordinate
             assert sec.drivable_lanes
             laneSections = {}
             for id_, lane in sec.drivable_lanes.items():
-                succ = None     # will set this later
+                succ = None  # will set this later
                 if last_section and lane.pred:
                     if lane.pred in last_section.lanesByOpenDriveID:
                         pred = last_section.lanesByOpenDriveID[lane.pred]
                     else:
-                        warn(f'road {self.id_} section {len(roadSections)} '
-                             f'lane {id_} has a non-drivable predecessor')
+                        warn(
+                            f"road {self.id_} section {len(roadSections)} "
+                            f"lane {id_} has a non-drivable predecessor"
+                        )
                         pred = None
                 else:
-                    pred = lane.pred    # will correct inter-road links later
+                    pred = lane.pred  # will correct inter-road links later
                 left, center, right = lane.left_bounds, lane.centerline, lane.right_bounds
-                if id_ > 0:     # backward lane
+                if id_ > 0:  # backward lane
                     left, center, right = right[::-1], center[::-1], left[::-1]
                     succ, pred = pred, succ
                 section = roadDomain.LaneSection(
-                    id=f'road{self.id_}_sec{len(roadSections)}_lane{id_}',
+                    id=f"road{self.id_}_sec{len(roadSections)}_lane{id_}",
                     polygon=lane_polys[id_],
                     centerline=PolylineRegion(cleanChain(center)),
                     leftEdge=PolylineRegion(cleanChain(left)),
                     rightEdge=PolylineRegion(cleanChain(right)),
                     successor=succ,
                     predecessor=pred,
-                    lane=None,      # will set these later
+                    lane=None,  # will set these later
                     group=None,
                     road=None,
                     openDriveID=id_,
-                    isForward=id_ < 0
+                    isForward=id_ < 0,
                 )
                 section._original_lane = lane
                 laneSections[id_] = section
                 allElements.append(section)
             section = roadDomain.RoadSection(
-                id=f'road{self.id_}_sec{len(roadSections)}',
+                id=f"road{self.id_}_sec{len(roadSections)}",
                 polygon=sec_poly,
                 centerline=PolylineRegion(cleanChain(pts)),
                 leftEdge=PolylineRegion(cleanChain(sec.left_edge)),
                 rightEdge=PolylineRegion(cleanChain(sec.right_edge)),
                 successor=None,
                 predecessor=last_section,
                 road=None,  # will set later
-                lanesByOpenDriveID=laneSections
+                lanesByOpenDriveID=laneSections,
             )
             roadSections.append(section)
             allElements.append(section)
             last_section = section
 
             for id_, lane in sec.sidewalk_lanes.items():
                 sidewalkSections[id_].append(lane)
@@ -669,80 +718,86 @@
         for id_ in sidewalkSections:
             (forwardSidewalks if id_ < 0 else backwardSidewalks).append(id_)
         for id_ in shoulderSections:
             (forwardShoulders if id_ < 0 else backwardShoulders).append(id_)
 
         def combineSections(laneIDs, sections, name):
             leftmost, rightmost = max(laneIDs), min(laneIDs)
-            if len(laneIDs) != leftmost-rightmost+1:
-                warn(f'ignoring {name} in the middle of road {self.id_}')
+            if len(laneIDs) != leftmost - rightmost + 1:
+                warn(f"ignoring {name} in the middle of road {self.id_}")
             leftPoints, rightPoints = [], []
             if leftmost < 0:
                 leftmost = rightmost
-                while leftmost+1 in laneIDs:
-                    leftmost = leftmost+1
+                while leftmost + 1 in laneIDs:
+                    leftmost = leftmost + 1
                 leftSecs, rightSecs = sections[leftmost], sections[rightmost]
                 for leftSec, rightSec in zip(leftSecs, rightSecs):
                     leftPoints.extend(leftSec.left_bounds)
                     rightPoints.extend(rightSec.right_bounds)
             else:
                 rightmost = leftmost
-                while rightmost-1 in laneIDs:
-                    rightmost = rightmost-1
+                while rightmost - 1 in laneIDs:
+                    rightmost = rightmost - 1
                 leftSecs = reversed(sections[leftmost])
                 rightSecs = reversed(sections[rightmost])
                 for leftSec, rightSec in zip(leftSecs, rightSecs):
                     leftPoints.extend(reversed(rightSec.right_bounds))
                     rightPoints.extend(reversed(leftSec.left_bounds))
             leftEdge = PolylineRegion(cleanChain(leftPoints))
             rightEdge = PolylineRegion(cleanChain(rightPoints))
 
             # Heuristically create some kind of reasonable centerline
             if len(leftPoints) == len(rightPoints):
-                centerPoints = list(averageVectors(l, r) for l, r in zip(leftPoints, rightPoints))
+                centerPoints = list(
+                    averageVectors(l, r) for l, r in zip(leftPoints, rightPoints)
+                )
             else:
                 num = max(len(leftPoints), len(rightPoints))
                 centerPoints = []
                 for d in np.linspace(0, 1, num):
                     l = leftEdge.lineString.interpolate(d, normalized=True)
                     r = rightEdge.lineString.interpolate(d, normalized=True)
                     centerPoints.append(averageVectors(l.coords[0], r.coords[0]))
             centerline = PolylineRegion(cleanChain(centerPoints))
-            allPolys = (sec.poly
-                        for id_ in range(rightmost, leftmost+1)
-                        for sec in sections[id_])
+            allPolys = (
+                sec.poly
+                for id_ in range(rightmost, leftmost + 1)
+                for sec in sections[id_]
+            )
             union = buffer_union(allPolys, tolerance=tolerance)
-            id_ = f'road{self.id_}_{name}({leftmost},{rightmost})'
+            id_ = f"road{self.id_}_{name}({leftmost},{rightmost})"
             return id_, union, centerline, leftEdge, rightEdge
 
         def makeSidewalk(laneIDs):
             if not laneIDs:
                 return None
             id_, union, centerline, leftEdge, rightEdge = combineSections(
-                laneIDs, sidewalkSections, 'sidewalk')
+                laneIDs, sidewalkSections, "sidewalk"
+            )
             sidewalk = roadDomain.Sidewalk(
                 id=id_,
                 polygon=union,
                 centerline=centerline,
                 leftEdge=leftEdge,
                 rightEdge=rightEdge,
                 road=None,
-                crossings=()    # TODO add crosswalks
+                crossings=(),  # TODO add crosswalks
             )
             allElements.append(sidewalk)
             return sidewalk
 
         forwardSidewalk = makeSidewalk(forwardSidewalks)
         backwardSidewalk = makeSidewalk(backwardSidewalks)
 
         def makeShoulder(laneIDs):
             if not laneIDs:
                 return None
             id_, union, centerline, leftEdge, rightEdge = combineSections(
-                laneIDs, shoulderSections, 'shoulder')
+                laneIDs, shoulderSections, "shoulder"
+            )
             shoulder = roadDomain.Shoulder(
                 id=id_,
                 polygon=union,
                 centerline=centerline,
                 leftEdge=leftEdge,
                 rightEdge=rightEdge,
                 road=None,
@@ -757,15 +812,16 @@
         next_section = None
         for sec, section in reversed(list(zip(self.lane_secs, roadSections))):
             if next_section is None:
                 next_section = section
                 for id_, lane in sec.drivable_lanes.items():
                     newLane = section.lanesByOpenDriveID[id_]
                     if newLane.isForward:
-                        newLane._successor = lane.succ   # will correct inter-road links later
+                        # will correct inter-road links later
+                        newLane._successor = lane.succ
                     else:
                         newLane._predecessor = lane.succ
                 continue
             section._successor = next_section
             for id_, lane in sec.drivable_lanes.items():
                 newLane = section.lanesByOpenDriveID[id_]
                 if newLane.isForward:
@@ -810,28 +866,32 @@
         nextID = 0
         forwardLanes, backwardLanes = [], []
         for roadSection in roadSections:
             for laneSection in roadSection.lanes:
                 laneSection._visited = False
         for roadSection, sec in zip(roadSections, self.lane_secs):
             for laneSection in roadSection.lanes:
-                if not laneSection._visited:     # start of new lane
+                if not laneSection._visited:  # start of new lane
                     forward = laneSection.isForward
                     sections = []
+                    successorLane = None  # lane this one will merge into
                     while True:
                         sections.append(laneSection)
                         laneSection._visited = True
                         assert laneSection.isForward == forward
                         if forward:
                             nextSection = laneSection._successor
                         else:
                             nextSection = laneSection._predecessor
-                        if (not nextSection
-                            or not isinstance(nextSection, roadDomain.LaneSection)
-                            or nextSection._visited):
+                        if not nextSection or not isinstance(
+                            nextSection, roadDomain.LaneSection
+                        ):
+                            break
+                        elif nextSection._visited:
+                            successorLane = nextSection.lane
                             break
                         laneSection = nextSection
                     ls = laneSection._original_lane
                     assert ls.parent_lane_poly
 
                     if not forward:
                         sections = tuple(reversed(sections))
@@ -840,22 +900,23 @@
                         leftPoints.extend(section.leftEdge.points)
                         rightPoints.extend(section.rightEdge.points)
                         centerPoints.extend(section.centerline.points)
                     leftEdge = PolylineRegion(cleanChain(leftPoints))
                     rightEdge = PolylineRegion(cleanChain(rightPoints))
                     centerline = PolylineRegion(cleanChain(centerPoints))
                     lane = roadDomain.Lane(
-                        id=f'road{self.id_}_lane{nextID}',
+                        id=f"road{self.id_}_lane{nextID}",
                         polygon=ls.parent_lane_poly,
                         centerline=centerline,
                         leftEdge=leftEdge,
                         rightEdge=rightEdge,
                         group=None,
                         road=None,
-                        sections=tuple(sections)
+                        sections=tuple(sections),
+                        successor=successorLane,  # will correct inter-road links later
                     )
                     nextID += 1
                     for section in sections:
                         section.lane = lane
                     (forwardLanes if forward else backwardLanes).append(lane)
                     allElements.append(lane)
         lanes = forwardLanes + backwardLanes
@@ -873,38 +934,39 @@
             if forward:
                 sec = roadSections[0]
                 startLanes = sec.forwardLanes
             else:
                 sec = roadSections[-1]
                 startLanes = sec.backwardLanes
             leftPoints = []
-            current = startLanes[-1]    # get leftmost lane of the first section
+            current = startLanes[-1]  # get leftmost lane of the first section
             while current and isinstance(current, roadDomain.LaneSection):
                 if current._laneToLeft and current._laneToLeft.isForward == forward:
                     current = current._laneToLeft
                 leftPoints.extend(current.leftEdge.points)
                 current = current._successor
             leftEdge = PolylineRegion(cleanChain(leftPoints))
             rightPoints = []
-            current = startLanes[0]     # get rightmost lane of the first section
+            current = startLanes[0]  # get rightmost lane of the first section
             while current and isinstance(current, roadDomain.LaneSection):
                 if current._laneToRight and current._laneToRight.isForward == forward:
                     current = current._laneToRight
                 rightPoints.extend(current.rightEdge.points)
                 current = current._successor
             rightEdge = PolylineRegion(cleanChain(rightPoints))
-            middleLane = startLanes[len(startLanes)//2].lane     # rather arbitrary
+            middleLane = startLanes[len(startLanes) // 2].lane  # rather arbitrary
             return leftEdge, middleLane.centerline, rightEdge
 
         if forwardLanes:
             leftEdge, centerline, rightEdge = getEdges(forward=True)
             forwardGroup = roadDomain.LaneGroup(
-                id=f'road{self.id_}_forward',
-                polygon=buffer_union((lane.polygon for lane in forwardLanes),
-                                     tolerance=tolerance),
+                id=f"road{self.id_}_forward",
+                polygon=buffer_union(
+                    (lane.polygon for lane in forwardLanes), tolerance=tolerance
+                ),
                 centerline=centerline,
                 leftEdge=leftEdge,
                 rightEdge=rightEdge,
                 road=None,
                 lanes=tuple(forwardLanes),
                 curb=(forwardShoulder.rightEdge if forwardShoulder else rightEdge),
                 sidewalk=forwardSidewalk,
@@ -914,17 +976,18 @@
             )
             allElements.append(forwardGroup)
         else:
             forwardGroup = None
         if backwardLanes:
             leftEdge, centerline, rightEdge = getEdges(forward=False)
             backwardGroup = roadDomain.LaneGroup(
-                id=f'road{self.id_}_backward',
-                polygon=buffer_union((lane.polygon for lane in backwardLanes),
-                                     tolerance=tolerance),
+                id=f"road{self.id_}_backward",
+                polygon=buffer_union(
+                    (lane.polygon for lane in backwardLanes), tolerance=tolerance
+                ),
                 centerline=centerline,
                 leftEdge=leftEdge,
                 rightEdge=rightEdge,
                 road=None,
                 lanes=tuple(backwardLanes),
                 curb=(backwardShoulder.rightEdge if backwardShoulder else rightEdge),
                 sidewalk=backwardSidewalk,
@@ -938,47 +1001,46 @@
         else:
             backwardGroup = None
 
         # Create signal
         roadSignals = []
         for i, signal_ in enumerate(self.signals):
             signal = roadDomain.Signal(
-                uid=f'signal{signal_.id_}_{self.id_}_{i}',
+                uid=f"signal{signal_.id_}_{self.id_}_{i}",
                 openDriveID=signal_.id_,
                 country=signal_.country,
-                type=signal_.type_
+                type=signal_.type_,
             )
             roadSignals.append(signal)
-            allElements.append(signal)
 
         # Create road
         assert forwardGroup or backwardGroup
         if forwardGroup:
             rightEdge = forwardGroup.rightEdge
         else:
             rightEdge = backwardGroup.leftEdge
         if backwardGroup:
             leftEdge = backwardGroup.rightEdge
         else:
             leftEdge = forwardGroup.leftEdge
         centerline = PolylineRegion(tuple(pt[:2] for pt in self.ref_line_points))
         road = roadDomain.Road(
             name=self.name,
-            uid=f'road{self.id_}',      # need prefix to prevent collisions with intersections
+            uid=f"road{self.id_}",  # need prefix to prevent collisions with intersections
             id=self.id_,
             polygon=self.drivable_region,
             centerline=centerline,
             leftEdge=leftEdge,
             rightEdge=rightEdge,
             lanes=lanes,
             forwardLanes=forwardGroup,
             backwardLanes=backwardGroup,
             sections=roadSections,
             signals=tuple(roadSignals),
-            crossings=(),       # TODO add these!
+            crossings=(),  # TODO add these!
         )
         allElements.append(road)
 
         # Set up parent references
         if forwardGroup:
             forwardGroup.road = road
             if forwardGroup._sidewalk:
@@ -1008,45 +1070,59 @@
             for sec in lane.sections:
                 sec.group = backwardGroup
                 sec.road = road
                 del sec._original_lane
 
         return road, allElements
 
+
 class Signal:
-    '''Traffic lights, stop signs, etc.'''
+    """Traffic lights, stop signs, etc."""
+
     def __init__(self, id_, country, type_, subtype, orientation, validity=None):
         self.id_ = id_
         self.country = country
         self.type_ = type_
         self.subtype = subtype
         self.orientation = orientation
         self.validity = validity
 
     def is_valid(self):
         return self.validity is None or self.validity != [0, 0]
 
+
 class SignalReference:
     def __init__(self, id_, orientation, validity=None):
         self.id_ = id_
         self.validity = validity
         self.orientation = orientation
 
     def is_valid(self):
         return self.validity is None or self.validity != [0, 0]
 
+
 class RoadMap:
     defaultTolerance = 0.05
 
-    def __init__(self, tolerance=None, fill_intersections=True,
-                 drivable_lane_types=('driving', 'entry', 'exit', 'offRamp', 'onRamp',
-                                      'connectingRamp'),
-                 sidewalk_lane_types=('sidewalk',),
-                 shoulder_lane_types=('shoulder', 'parking', 'stop', 'border'),
-                 elide_short_roads=False):
+    def __init__(
+        self,
+        tolerance=None,
+        fill_intersections=True,
+        drivable_lane_types=(
+            "driving",
+            "entry",
+            "exit",
+            "offRamp",
+            "onRamp",
+            "connectingRamp",
+        ),
+        sidewalk_lane_types=("sidewalk",),
+        shoulder_lane_types=("shoulder", "parking", "stop", "border"),
+        elide_short_roads=False,
+    ):
         self.tolerance = self.defaultTolerance if tolerance is None else tolerance
         self.roads = {}
         self.road_links = []
         self.junctions = {}
         self.sec_lane_polys = []
         self.lane_polys = []
         self.intersection_region = None
@@ -1057,18 +1133,22 @@
         self.elide_short_roads = elide_short_roads
 
     def calculate_geometry(self, num, calc_gap=False, calc_intersect=True):
         # If calc_gap=True, fills in gaps between connected roads.
         # If calc_intersect=True, calculates intersection regions.
         # These are fairly expensive.
         for road in self.roads.values():
-            road.calculate_geometry(num, calc_gap=calc_gap, tolerance=self.tolerance,
-                                    drivable_lane_types=self.drivable_lane_types,
-                                    sidewalk_lane_types=self.sidewalk_lane_types,
-                                    shoulder_lane_types=self.shoulder_lane_types)
+            road.calculate_geometry(
+                num,
+                calc_gap=calc_gap,
+                tolerance=self.tolerance,
+                drivable_lane_types=self.drivable_lane_types,
+                sidewalk_lane_types=self.sidewalk_lane_types,
+                shoulder_lane_types=self.shoulder_lane_types,
+            )
             self.sec_lane_polys.extend(road.sec_lane_polys)
             self.lane_polys.extend(road.lane_polys)
 
         if calc_gap:
             drivable_polys = []
             sidewalk_polys = []
             shoulder_polys = []
@@ -1082,48 +1162,52 @@
                     sidewalk_polys.append(sidewalk_poly)
                 if not (shoulder_poly is None or shoulder_poly.is_empty):
                     shoulder_polys.append(shoulder_poly)
 
             for link in self.road_links:
                 road_a = self.roads[link.id_a]
                 road_b = self.roads[link.id_b]
-                assert link.contact_a in ['start', 'end'], 'Invalid link record.'
-                assert link.contact_b in ['start', 'end'], 'Invalid link record.'
-                if link.contact_a == 'start':
+                assert link.contact_a in ["start", "end"], "Invalid link record."
+                assert link.contact_b in ["start", "end"], "Invalid link record."
+                if link.contact_a == "start":
                     a_sec = road_a.lane_secs[0]
                     a_bounds_left = road_a.start_bounds_left
                     a_bounds_right = road_a.start_bounds_right
                 else:
                     a_sec = road_a.lane_secs[-1]
                     a_bounds_left = road_a.end_bounds_left
                     a_bounds_right = road_a.end_bounds_right
-                if link.contact_b == 'start':
+                if link.contact_b == "start":
                     b_bounds_left = road_b.start_bounds_left
                     b_bounds_right = road_b.start_bounds_right
                 else:
                     b_bounds_left = road_b.end_bounds_left
                     b_bounds_right = road_b.end_bounds_right
 
                 for id_, lane in a_sec.lanes.items():
-                    if link.contact_a == 'start':
+                    if link.contact_a == "start":
                         other_id = lane.pred
                     else:
                         other_id = lane.succ
                     if other_id not in b_bounds_left or other_id not in b_bounds_right:
                         continue
                     if id_ not in a_bounds_left or id_ not in a_bounds_right:
                         continue
 
-                    gap_poly = MultiPoint([
-                        a_bounds_left[id_], a_bounds_right[id_],
-                        b_bounds_left[other_id], b_bounds_right[other_id]
-                    ]).convex_hull
+                    gap_poly = MultiPoint(
+                        [
+                            a_bounds_left[id_],
+                            a_bounds_right[id_],
+                            b_bounds_left[other_id],
+                            b_bounds_right[other_id],
+                        ]
+                    ).convex_hull
                     if not gap_poly.is_valid:
                         continue
-                    if gap_poly.geom_type == 'Polygon' and not gap_poly.is_empty:
+                    if gap_poly.geom_type == "Polygon" and not gap_poly.is_empty:
                         if lane.type_ in self.drivable_lane_types:
                             drivable_polys.append(gap_poly)
                         elif lane.type_ in self.sidewalk_lane_types:
                             sidewalk_polys.append(gap_poly)
                         elif lane.type_ in self.shoulder_lane_types:
                             shoulder_polys.append(gap_poly)
         else:
@@ -1148,185 +1232,161 @@
                 union = removeHoles(union)
             assert union.is_valid
             junc.poly = union
             intersect_polys.append(union)
         self.intersection_region = buffer_union(intersect_polys, tolerance=self.tolerance)
 
     def heading_at(self, point):
-        '''Return the road heading at point.'''
+        """Return the road heading at point."""
         # Convert point to shapely Point.
         point = Point(point.x, point.y)
         for road in self.roads.values():
             if point.within(road.drivable_region.buffer(1)):
                 return road.heading_at(point)
-        #raise RuntimeError('Point not in RoadMap: ', point)
+        # raise RuntimeError('Point not in RoadMap: ', point)
         return 0
 
-    def plot_line(self, plt, num=500):
-        '''Plot center line of road map for sanity check.'''
-        for road in self.roads.values():
-            for piece in road.ref_line:
-                points = piece.to_points(num)
-                x = [p[0] for p in points]
-                y = [p[1] for p in points]
-                plt.plot(x, y, 'b')
-        plt.show()
-
-    def plot_lanes(self, plt, num=500):
-        '''Plot lane boundaries of road map for sanity check.'''
-        bounds_x =[]
-        bounds_y = []
-        for road in self.roads.values():
-            for piece in road.ref_line:
-                ref_points = piece.to_points(num)
-                for i in range(len(ref_points) - 1):
-                    offsets = road.get_lane_offsets(ref_points[i][2])
-                    tan_vec = (ref_points[i + 1][0] - ref_points[i][0],
-                               ref_points[i + 1][1] - ref_points[i][1])
-                    tan_norm = np.sqrt(tan_vec[0] ** 2 + tan_vec[1] ** 2)
-                    normal_vec = (-tan_vec[1] / tan_norm, tan_vec[0] / tan_norm)
-                    # ortho_line_x = []
-                    # ortho_line_y = []
-                    for id_ in offsets.keys():
-                        if road.get_lane(id_, ref_points[i][2]).type_ == 'driving':
-                            bounds_x.append(ref_points[i][0] + normal_vec[0] * offsets[id_])
-                            bounds_y.append(ref_points[i][1] + normal_vec[1] * offsets[id_])
-        plt.scatter(bounds_x, bounds_y, c='r', s=2)
-        plt.show()
-
     def __parse_lanes(self, lanes_elem):
-        '''Lanes_elem should be <left> or <right> element.
-        Returns dict of lane ids and Lane objects.'''
+        """Lanes_elem should be <left> or <right> element.
+        Returns dict of lane ids and Lane objects."""
         lanes = {}
-        for l in lanes_elem.iter('lane'):
-            id_ = int(l.get('id'))
-            type_ = l.get('type')
-            link = l.find('link')
+        for l in lanes_elem.iter("lane"):
+            id_ = int(l.get("id"))
+            type_ = l.get("type")
+            link = l.find("link")
             pred = None
             succ = None
             if link is not None:
-                pred_elem = link.find('predecessor')
-                succ_elem = link.find('successor')
+                pred_elem = link.find("predecessor")
+                succ_elem = link.find("successor")
                 if pred_elem is not None:
-                    pred = int(pred_elem.get('id'))
+                    pred = int(pred_elem.get("id"))
                 if succ_elem is not None:
-                    succ = int(succ_elem.get('id'))
+                    succ = int(succ_elem.get("id"))
             lane = Lane(id_, type_, pred, succ)
-            for w in l.iter('width'):
-                w_poly = Poly3(float(w.get('a')),
-                               float(w.get('b')),
-                               float(w.get('c')),
-                               float(w.get('d')))
-                lane.width.append((w_poly, float(w.get('sOffset'))))
+            for w in l.iter("width"):
+                w_poly = Poly3(
+                    float(w.get("a")),
+                    float(w.get("b")),
+                    float(w.get("c")),
+                    float(w.get("d")),
+                )
+                lane.width.append((w_poly, float(w.get("sOffset"))))
             lanes[id_] = lane
         return lanes
 
     def __parse_link(self, link_elem, road, contact):
         if link_elem is None:
             return
         road_id = road.id_
-        if link_elem.get('elementType') == 'road':
-            id_b = int(link_elem.get('elementId'))
-            contact_b = link_elem.get('contactPoint')
+        if link_elem.get("elementType") == "road":
+            id_b = int(link_elem.get("elementId"))
+            contact_b = link_elem.get("contactPoint")
             link = RoadLink(road_id, id_b, contact, contact_b)
             self.road_links.append(link)
             return link
         else:
-            assert link_elem.get('elementType') == 'junction', 'Unknown link type'
-            junction = int(link_elem.get('elementId'))
+            assert link_elem.get("elementType") == "junction", "Unknown link type"
+            junction = int(link_elem.get("elementId"))
             if junction not in self.junctions:
-                return    # junction had no connecting roads, so we skipped it
-            if contact == 'start':
+                return  # junction had no connecting roads, so we skipped it
+            if contact == "start":
                 road.predecessor = junction
             else:
                 road.successor = junction
             connections = self.junctions[junction].connections
             for c in connections:
                 if c.incoming_id == road_id:
-                    self.road_links.append(RoadLink(road_id,
-                                                    c.connecting_id,
-                                                    contact,
-                                                    c.connecting_contact))
+                    self.road_links.append(
+                        RoadLink(road_id, c.connecting_id, contact, c.connecting_contact)
+                    )
 
     def __parse_signal_validity(self, validity_elem):
         if validity_elem is None:
             return None
-        return [int(validity_elem.get('fromLane')), int(validity_elem.get('toLane'))]
+        return [int(validity_elem.get("fromLane")), int(validity_elem.get("toLane"))]
 
     def __parse_signal(self, signal_elem):
         return Signal(
-            signal_elem.get('id'),
-            signal_elem.get('country'),
-            signal_elem.get('type'),
-            signal_elem.get('subtype'),
-            signal_elem.get('orientation'),
-            self.__parse_signal_validity(signal_elem.find('validity'))
+            signal_elem.get("id"),
+            signal_elem.get("country"),
+            signal_elem.get("type"),
+            signal_elem.get("subtype"),
+            signal_elem.get("orientation"),
+            self.__parse_signal_validity(signal_elem.find("validity")),
         )
 
     def __parse_signal_reference(self, signal_reference_elem):
         return SignalReference(
-            signal_reference_elem.get('id'),
-            signal_reference_elem.get('orientation'),
-            self.__parse_signal_validity(signal_reference_elem.find('validity'))
+            signal_reference_elem.get("id"),
+            signal_reference_elem.get("orientation"),
+            self.__parse_signal_validity(signal_reference_elem.find("validity")),
         )
 
     def parse(self, path):
         tree = ET.parse(path)
         root = tree.getroot()
-        if root.tag != 'OpenDRIVE':
-            raise RuntimeError(f'{path} does not appear to be an OpenDRIVE file')
+        if root.tag != "OpenDRIVE":
+            raise ValueError(f"{path} does not appear to be an OpenDRIVE file")
 
         # parse junctions
-        for j in root.iter('junction'):
-            junction = Junction(int(j.get('id')), j.get('name'))
-            for c in j.iter('connection'):
-                ty = c.get('type', 'default')
-                if ty != 'default':
-                    raise RuntimeError(f'unhandled "{ty}" type of junction connection')
+        for j in root.iter("junction"):
+            junction = Junction(int(j.get("id")), j.get("name"))
+            for c in j.iter("connection"):
+                ty = c.get("type", "default")
+                if ty != "default":
+                    raise NotImplementedError(
+                        f'unhandled "{ty}" type of junction connection'
+                    )
                 lane_links = {}
-                for l in c.iter('laneLink'):
-                    lane_links[int(l.get('from'))] = int(l.get('to'))
-                junction.add_connection(int(c.get('incomingRoad')),
-                                        int(c.get('connectingRoad')),
-                                        c.get('contactPoint'),
-                                        lane_links)
-                junction.paths.append(int(c.get('connectingRoad')))
+                for l in c.iter("laneLink"):
+                    lane_links[int(l.get("from"))] = int(l.get("to"))
+                junction.add_connection(
+                    int(c.get("incomingRoad")),
+                    int(c.get("connectingRoad")),
+                    c.get("contactPoint"),
+                    lane_links,
+                )
+                junction.paths.append(int(c.get("connectingRoad")))
             if not junction.paths:
-                warn(f'junction {junction.id_} has no connecting roads; skipping it')
+                warn(f"junction {junction.id_} has no connecting roads; skipping it")
                 continue
             self.junctions[junction.id_] = junction
 
         # Creating temporal signals container to resolve referenced signals.
         _temp_signals = {}
-        for r in root.iter('road'):
-            signals = r.find('signals')
+        for r in root.iter("road"):
+            signals = r.find("signals")
             if signals is not None:
-                for s in signals.iter('signal'):
+                for s in signals.iter("signal"):
                     signal = self.__parse_signal(s)
                     _temp_signals[signal.id_] = signal
 
         # parse roads
         self.elidedRoads = {}
-        for r in root.iter('road'):
-            road = Road(r.get('name'), int(r.get('id')), float(r.get('length')),
-                        r.get('junction'))
-            link = r.find('link')
+        for r in root.iter("road"):
+            road = Road(
+                r.get("name"), int(r.get("id")), float(r.get("length")), r.get("junction")
+            )
+            link = r.find("link")
             if link is not None:
-                pred_elem = link.find('predecessor')
-                succ_elem = link.find('successor')
-                pred_link = self.__parse_link(pred_elem, road, 'start')
-                succ_link = self.__parse_link(succ_elem, road, 'end')
+                pred_elem = link.find("predecessor")
+                succ_elem = link.find("successor")
+                pred_link = self.__parse_link(pred_elem, road, "start")
+                succ_link = self.__parse_link(succ_elem, road, "end")
             else:
                 pred_link = succ_link = None
 
             if road.length < self.tolerance:
-                warn(f'road {road.id_} has length shorter than tolerance;'
-                     ' geometry may contain artifacts')
+                warn(
+                    f"road {road.id_} has length shorter than tolerance;"
+                    " geometry may contain artifacts"
+                )
                 if self.elide_short_roads:
-                    warn(f'attempting to elide road {road.id_} of length {road.length}')
+                    warn(f"attempting to elide road {road.id_} of length {road.length}")
                     assert road.junction is None
                     self.elidedRoads[road.id_] = road
                     if pred_link:
                         road.predecessor = pred_link.id_b
                         road.predecessorContact = pred_link.contact_b
                     else:
                         road.predecessorContact = None
@@ -1334,167 +1394,184 @@
                         road.successor = succ_link.id_b
                         road.successorContact = succ_link.contact_b
                     else:
                         road.successorContact = None
                     continue
 
             # Parse planView:
-            plan_view = r.find('planView')
+            plan_view = r.find("planView")
             curves = []
-            for geom in plan_view.iter('geometry'):
-                x0 = float(geom.get('x'))
-                y0 = float(geom.get('y'))
-                s0 = float(geom.get('s'))
-                hdg = float(geom.get('hdg'))
-                length = float(geom.get('length'))
+            for geom in plan_view.iter("geometry"):
+                x0 = float(geom.get("x"))
+                y0 = float(geom.get("y"))
+                s0 = float(geom.get("s"))
+                hdg = float(geom.get("hdg"))
+                length = float(geom.get("length"))
                 curve_elem = geom[0]
                 curve = None
-                if curve_elem.tag == 'line':
+                if curve_elem.tag == "line":
                     curve = Line(x0, y0, hdg, length)
-                elif curve_elem.tag == 'arc':
+                elif curve_elem.tag == "arc":
                     # Arc is clothoid of constant curvature.
-                    curv = float(curve_elem.get('curvature'))
+                    curv = float(curve_elem.get("curvature"))
                     curve = Clothoid(x0, y0, hdg, length, curv, curv)
-                elif curve_elem.tag == 'spiral':
-                    curv0 = float(curve_elem.get('curvStart'))
-                    curv1 = float(curve_elem.get('curvEnd'))
+                elif curve_elem.tag == "spiral":
+                    curv0 = float(curve_elem.get("curvStart"))
+                    curv1 = float(curve_elem.get("curvEnd"))
                     curve = Clothoid(x0, y0, hdg, length, curv0, curv1)
-                elif curve_elem.tag == 'poly3':
-                    a, b, c, d = cubic_elem.get('a'), \
-                        float(curve_elem.get('b')), \
-                        float(curve_elem.get('c')), \
-                        float(curve_elem.get('d'))
+                elif curve_elem.tag == "poly3":
+                    a, b, c, d = (
+                        cubic_elem.get("a"),
+                        float(curve_elem.get("b")),
+                        float(curve_elem.get("c")),
+                        float(curve_elem.get("d")),
+                    )
                     curve = Cubic(x0, y0, hdg, length, a, b, c, d)
-                elif curve_elem.tag == 'paramPoly3':
-                    au, bu, cu, du, av, bv, cv, dv = \
-                        float(curve_elem.get('aU')), \
-                        float(curve_elem.get('bU')), \
-                        float(curve_elem.get('cU')), \
-                        float(curve_elem.get('dU')), \
-                        float(curve_elem.get('aV')), \
-                        float(curve_elem.get('bV')), \
-                        float(curve_elem.get('cV')), \
-                        float(curve_elem.get('dV'))
-                    p_range = curve_elem.get('pRange')
-                    if p_range and p_range != 'normalized':
+                elif curve_elem.tag == "paramPoly3":
+                    au, bu, cu, du, av, bv, cv, dv = (
+                        float(curve_elem.get("aU")),
+                        float(curve_elem.get("bU")),
+                        float(curve_elem.get("cU")),
+                        float(curve_elem.get("dU")),
+                        float(curve_elem.get("aV")),
+                        float(curve_elem.get("bV")),
+                        float(curve_elem.get("cV")),
+                        float(curve_elem.get("dV")),
+                    )
+                    p_range = curve_elem.get("pRange")
+                    if p_range and p_range != "normalized":
                         # TODO support arcLength
-                        raise RuntimeError('unsupported pRange for paramPoly3')
+                        raise NotImplementedError("unsupported pRange for paramPoly3")
                     else:
                         p_range = 1
-                    curve = ParamCubic(x0, y0, hdg, length,
-                                       au, bu, cu, du, av, bv,
-                                       cv, dv, p_range)
+                    curve = ParamCubic(
+                        x0, y0, hdg, length, au, bu, cu, du, av, bv, cv, dv, p_range
+                    )
                 curves.append((s0, curve))
             if not curves:
-                raise RuntimeError(f'road {road.id_} has an empty planView')
+                raise ValueError(f"road {road.id_} has an empty planView")
             if not curves[0][0] == 0:
-                raise RuntimeError(f'reference line of road {road.id_} does not start at s=0')
+                raise ValueError(
+                    f"reference line of road {road.id_} does not start at s=0"
+                )
             lastS = 0
             lastCurve = curves[0][1]
             refLine = []
             for s0, curve in curves[1:]:
                 l = s0 - lastS
                 if abs(lastCurve.length - l) > 1e-4:
-                    raise RuntimeError(f'planView of road {road.id_} has inconsistent length')
+                    raise ValueError(
+                        f"planView of road {road.id_} has inconsistent length"
+                    )
                 if l < 0:
-                    raise RuntimeError(f'planView of road {road.id_} is not in order')
+                    raise ValueError(f"planView of road {road.id_} is not in order")
                 elif l < 1e-6:
-                    warn(f'road {road.id_} reference line has a geometry of '
-                         f'length {l}; skipping it')
+                    warn(
+                        f"road {road.id_} reference line has a geometry of "
+                        f"length {l}; skipping it"
+                    )
                 else:
                     refLine.append(lastCurve)
                 lastS = s0
                 lastCurve = curve
             if refLine and lastCurve.length < 1e-6:
-                warn(f'road {road.id_} reference line has a geometry of '
-                     f'length {lastCurve.length}; skipping it')
+                warn(
+                    f"road {road.id_} reference line has a geometry of "
+                    f"length {lastCurve.length}; skipping it"
+                )
             else:
                 # even if the last curve is shorter than the threshold, we'll keep it if
                 # it is the only curve; getting rid of the road entirely is handled by
                 # road elision above
                 refLine.append(lastCurve)
             assert refLine
             road.ref_line = refLine
 
             # Parse lanes:
-            lanes = r.find('lanes')
-            for offset in lanes.iter('laneOffset'):
-                road.offset.append((Poly3(float(offset.get('a')),
-                                         float(offset.get('b')),
-                                         float(offset.get('c')),
-                                         float(offset.get('d'))),
-                                   float(offset.get('s'))))
+            lanes = r.find("lanes")
+            for offset in lanes.iter("laneOffset"):
+                road.offset.append(
+                    (
+                        Poly3(
+                            float(offset.get("a")),
+                            float(offset.get("b")),
+                            float(offset.get("c")),
+                            float(offset.get("d")),
+                        ),
+                        float(offset.get("s")),
+                    )
+                )
 
             def popLastSectionIfShort(l):
                 if l < 1e-6:
-                    warn(f'road {road.id_} has a lane section of length {l}; skipping it')
+                    warn(f"road {road.id_} has a lane section of length {l}; skipping it")
 
                     # delete the length-0 section and re-link lanes appropriately
                     badSec = road.lane_secs.pop()
                     if road.lane_secs:
                         prev = road.lane_secs[-1]
                         for id_, lane in prev.lanes.items():
                             if lane.succ is not None:
                                 lane.succ = badSec.lanes[lane.succ].succ
                     else:
                         if road.remappedStartLanes is None:
-                            road.remappedStartLanes = { l: l for l in badSec.lanes }
+                            road.remappedStartLanes = {l: l for l in badSec.lanes}
                         for start, current in road.remappedStartLanes.items():
                             road.remappedStartLanes[start] = badSec.lanes[current].succ
                     return badSec
                 else:
                     return None
 
-            last_s = float('-inf')
-            for ls_elem in lanes.iter('laneSection'):
-                s = float(ls_elem.get('s'))
+            last_s = float("-inf")
+            for ls_elem in lanes.iter("laneSection"):
+                s = float(ls_elem.get("s"))
                 l = s - last_s
                 assert l >= 0
                 badSec = popLastSectionIfShort(l)
 
                 last_s = s
-                left = ls_elem.find('left')
-                right = ls_elem.find('right')
+                left = ls_elem.find("left")
+                right = ls_elem.find("right")
                 left_lanes = {}
                 right_lanes = {}
 
                 if left is not None:
                     left_lanes = self.__parse_lanes(left)
 
                 if right is not None:
                     right_lanes = self.__parse_lanes(right)
 
                 lane_sec = LaneSection(s, left_lanes, right_lanes)
 
-                if badSec is not None:      # finish re-linking lanes across deleted section
+                if badSec is not None:  # finish re-linking lanes across deleted section
                     for id_, lane in lane_sec.lanes.items():
                         if lane.pred is not None:
                             lane.pred = badSec.lanes[lane.pred].pred
 
                 road.lane_secs.append(lane_sec)
 
             # parse signals
-            signals = r.find('signals')
+            signals = r.find("signals")
             if signals is not None:
-                for signal_elem in signals.iter('signal'):
+                for signal_elem in signals.iter("signal"):
                     signal = self.__parse_signal(signal_elem)
                     if signal.is_valid():
                         road.signals.append(signal)
 
-                for signal_ref_elem in signals.iter('signalReference'):
+                for signal_ref_elem in signals.iter("signalReference"):
                     signalReference = self.__parse_signal_reference(signal_ref_elem)
                     if signalReference.is_valid():
                         referencedSignal = _temp_signals[signalReference.id_]
                         signal = Signal(
                             referencedSignal.id_,
                             referencedSignal.country,
                             referencedSignal.type_,
                             referencedSignal.subtype,
                             signalReference.orientation,
-                            signalReference.validity
+                            signalReference.validity,
                         )
                         road.signals.append(signal)
 
             if len(road.lane_secs) > 1:
                 popLastSectionIfShort(road.length - s)
             assert road.lane_secs
             self.roads[road.id_] = road
@@ -1502,66 +1579,68 @@
         # Handle links to/from elided roads
         new_links = []
         for link in self.road_links:
             if link.id_a in self.elidedRoads:
                 continue
             if link.id_b in self.elidedRoads:
                 elided = self.elidedRoads[link.id_b]
-                if link.contact_b == 'start':
+                if link.contact_b == "start":
                     link.id_b = elided.successor
                     link.contact_b = elided.successorContact
                 else:
                     link.id_b = elided.predecessor
                     link.contact_b = elided.predecessorContact
                 if link.contact_b is None:
-                    continue    # link to intersection
+                    continue  # link to intersection
             new_links.append(link)
         self.road_links = new_links
 
     def toScenicNetwork(self):
         assert self.intersection_region is not None
 
         # Prepare registry of network elements
         allElements = {}
+
         def register(element):
             assert element.uid is not None
             assert element.uid not in allElements, element.uid
             allElements[element.uid] = element
+
         def registerAll(elements):
             for elt in elements:
                 register(elt)
 
         # Convert roads
         mainRoads, connectingRoads, roads = {}, {}, {}
         for id_, road in self.roads.items():
             if road.drivable_region.is_empty:
-                continue    # not actually a road you can drive on
+                continue  # not actually a road you can drive on
             newRoad, elts = road.toScenicRoad(tolerance=self.tolerance)
             registerAll(elts)
             (connectingRoads if road.junction else mainRoads)[id_] = newRoad
             roads[id_] = newRoad
 
         # Hook up inter-road links
         for link in self.road_links:
             if link.id_b in connectingRoads:
-                continue    # actually a road-to-junction link; handled later
+                continue  # actually a road-to-junction link; handled later
             if link.id_a not in roads or link.id_b not in roads:
-                continue    # may link non-drivable roads we haven't parsed; ignore it
+                continue  # may link non-drivable roads we haven't parsed; ignore it
 
             # Work out connectivity of roads and adjacent sections
             roadA, roadB = roads[link.id_a], roads[link.id_b]
-            if link.contact_a == 'start':
+            if link.contact_a == "start":
                 secA = roadA.sections[0]
                 roadA._predecessor = roadB
                 forwardA = True
             else:
                 secA = roadA.sections[-1]
                 roadA._successor = roadB
                 forwardA = False
-            if link.contact_b == 'start':
+            if link.contact_b == "start":
                 secB = roadB.sections[0]
             else:
                 secB = roadB.sections[-1]
 
             # Connect corresponding lanes
             lanesB = secB.lanesByOpenDriveID
             for laneA in secA.lanes:
@@ -1587,47 +1666,47 @@
         # Hook up connecting road links and create intersections
         intersections = {}
         for jid, junction in self.junctions.items():
             if not junction.connections:
                 continue
             assert junction.poly is not None
             if junction.poly.is_empty:
-                warn(f'skipping empty junction {jid}')
+                warn(f"skipping empty junction {jid}")
                 continue
 
             # Gather all lanes involved in the junction's connections
             allIncomingLanes, allOutgoingLanes = [], []
             allRoads, seenRoads = [], set()
             allSignals, seenSignals = [], set()
             maneuversForLane = defaultdict(list)
             for connection in junction.connections:
                 incomingID = connection.incoming_id
                 incomingRoad = mainRoads.get(incomingID)
                 if not incomingRoad:
-                    continue    # incoming road has no drivable lanes; skip it
+                    continue  # incoming road has no drivable lanes; skip it
 
                 connectingID = connection.connecting_id
                 connectingRoad = connectingRoads.get(connectingID)
                 if not connectingRoad:
-                    continue    # connecting road has no drivable lanes; skip it
+                    continue  # connecting road has no drivable lanes; skip it
 
                 for signal in connectingRoad.signals:
                     if signal.openDriveID not in seenSignals:
                         allSignals.append(signal)
                         seenSignals.add(signal.openDriveID)
 
                 # Find possible incoming lanes for this connection
                 if incomingID not in seenRoads:
                     allRoads.append(incomingRoad)
                     seenRoads.add(incomingID)
                 oldRoad = self.roads[incomingID]
                 incomingSection = None
                 if oldRoad.predecessor == jid:
                     incomingSection = incomingRoad.sections[0]
-                    remapping = self.roads[incomingID].remappedStartLanes     # could be None
+                    remapping = self.roads[incomingID].remappedStartLanes  # could be None
                 if oldRoad.successor == jid:
                     assert incomingSection is None
                     incomingSection = incomingRoad.sections[-1]
                     remapping = None
                 assert incomingSection is not None
                 if remapping is None:
                     incomingLaneIDs = incomingSection.lanesByOpenDriveID
@@ -1636,65 +1715,69 @@
                     newIDs = incomingSection.lanesByOpenDriveID
                     for start, remapped in remapping.items():
                         if remapped in newIDs:
                             incomingLaneIDs[start] = newIDs[remapped]
                     assert len(incomingLaneIDs) == len(newIDs)
 
                 # Connect incoming lanes to connecting road
-                if connection.connecting_contact == 'start':
+                if connection.connecting_contact == "start":
                     connectingSection = connectingRoad.sections[0]
-                    remapping = self.roads[connectingID].remappedStartLanes   # could be None
+                    remapping = self.roads[
+                        connectingID
+                    ].remappedStartLanes  # could be None
                 else:
                     connectingSection = connectingRoad.sections[-1]
                     remapping = None
                 if remapping is None:
                     connectingLaneIDs = connectingSection.lanesByOpenDriveID
                 else:
                     connectingLaneIDs = {}
                     newIDs = connectingSection.lanesByOpenDriveID
                     for start, remapped in remapping.items():
                         if remapped in newIDs:
                             connectingLaneIDs[start] = newIDs[remapped]
                     assert len(connectingLaneIDs) == len(newIDs)
                 lane_links = connection.lane_links
-                if not lane_links:   # all lanes connect to that with the same id
-                    lane_links = { l: l for l in incomingLaneIDs }
+                if not lane_links:  # all lanes connect to that with the same id
+                    lane_links = {l: l for l in incomingLaneIDs}
                 for fromID, fromLane in incomingLaneIDs.items():
                     # Link incoming lane to connecting road
                     # (we only handle lanes in incomingLaneIDs, thus skipping non-drivable lanes)
                     if fromID not in lane_links:
-                        continue    # lane not linked by this connection
+                        continue  # lane not linked by this connection
                     toID = lane_links[fromID]
                     toLane = connectingLaneIDs[toID]
                     if fromLane.lane not in allIncomingLanes:
                         allIncomingLanes.append(fromLane.lane)
                     fromLane._successor = toLane
                     fromLane.lane._successor = toLane.lane
                     toLane._predecessor = fromLane
                     toLane.lane._predecessor = fromLane.lane
 
                     # Collect outgoing lane and road
                     # TODO why is it allowed for this not to exist?
                     outgoingLane = toLane.lane._successor
                     if outgoingLane is None:
-                        warn(f'connecting road {connectingID} lane {toID} has no successor lane')
+                        warn(
+                            f"connecting road {connectingID} lane {toID} has no successor lane"
+                        )
                     else:
                         if outgoingLane not in allOutgoingLanes:
                             allOutgoingLanes.append(outgoingLane)
                         outgoingRoad = outgoingLane.road
                         if outgoingRoad.id not in seenRoads:
                             allRoads.append(outgoingRoad)
                             seenRoads.add(outgoingRoad.id)
 
                         # TODO future OpenDRIVE extension annotating left/right turns?
                         maneuver = roadDomain.Maneuver(
                             startLane=fromLane.lane,
                             connectingLane=toLane.lane,
                             endLane=outgoingLane,
-                            intersection=None   # will be patched once the Intersection is created
+                            intersection=None,  # will be patched once the Intersection is created
                         )
                         maneuversForLane[fromLane.lane].append(maneuver)
 
             # Gather maneuvers
             allManeuvers = []
             for lane, maneuvers in maneuversForLane.items():
                 assert lane.maneuvers == ()
@@ -1704,43 +1787,45 @@
             # Order connected roads and lanes by adjacency
             def cyclicOrder(elements, contactStart=None):
                 points = []
                 for element in elements:
                     if contactStart is None:
                         old = self.roads[element.id]
                         assert old.predecessor == jid or old.successor == jid
-                        contactStart = (old.predecessor == jid)
+                        contactStart = old.predecessor == jid
                     point = element.centerline[0 if contactStart else -1]
                     points.append(point)
                 centroid = sum(points, Vector(0, 0)) / len(points)
-                pairs = sorted(zip(elements, points), key=lambda pair: centroid.angleTo(pair[1]))
+                pairs = sorted(
+                    zip(elements, points), key=lambda pair: centroid.angleTo(pair[1])
+                )
                 return tuple(elem for elem, pt in pairs)
 
             # Create intersection
             intersection = roadDomain.Intersection(
                 polygon=junction.poly,
                 name=junction.name,
-                uid=f'intersection{jid}',   # need prefix to prevent collisions with roads
+                uid=f"intersection{jid}",  # need prefix to prevent collisions with roads
                 id=jid,
                 roads=cyclicOrder(allRoads),
                 incomingLanes=cyclicOrder(allIncomingLanes, contactStart=False),
                 outgoingLanes=cyclicOrder(allOutgoingLanes, contactStart=True),
                 maneuvers=tuple(allManeuvers),
                 signals=tuple(allSignals),
-                crossings=(),       # TODO add these
+                crossings=(),  # TODO add these
             )
             register(intersection)
             intersections[jid] = intersection
             for maneuver in allManeuvers:
-                object.__setattr__(maneuver, 'intersection', intersection)
+                object.__setattr__(maneuver, "intersection", intersection)
 
         # Hook up road-intersection links
         for rid, oldRoad in self.roads.items():
             if rid not in roads:
-                continue    # road does not have any drivable lanes, so we skipped it
+                continue  # road does not have any drivable lanes, so we skipped it
             newRoad = roads[rid]
             if oldRoad.predecessor:
                 intersection = intersections[oldRoad.predecessor]
                 newRoad._predecessor = intersection
                 newRoad.sections[0]._predecessor = intersection
                 if newRoad.backwardLanes:
                     newRoad.backwardLanes._successor = intersection
@@ -1759,29 +1844,32 @@
         for road in allRoads:
             if road.forwardLanes:
                 groups.append(road.forwardLanes)
             if road.backwardLanes:
                 groups.append(road.backwardLanes)
         lanes = [lane for road in allRoads for lane in road.lanes]
         intersections = tuple(intersections.values())
-        crossings = ()      # TODO add these
+        crossings = ()  # TODO add these
         sidewalks, shoulders = [], []
         for group in groups:
             sidewalk = group._sidewalk
             if sidewalk:
                 sidewalks.append(sidewalk)
             shoulder = group._shoulder
             if shoulder:
                 shoulders.append(shoulder)
 
         # Add dummy maneuvers for lanes which merge/turn into another lane
         for lane in lanes:
             if not lane.maneuvers and lane._successor:
-                maneuver = roadDomain.Maneuver(type=roadDomain.ManeuverType.STRAIGHT,
-                                               startLane=lane, endLane=lane._successor)
+                maneuver = roadDomain.Maneuver(
+                    type=roadDomain.ManeuverType.STRAIGHT,
+                    startLane=lane,
+                    endLane=lane._successor,
+                )
                 lane.maneuvers = (maneuver,)
 
         def combine(regions):
             return PolygonalRegion.unionAll(regions, buf=self.tolerance)
 
         return roadDomain.Network(
             elements=allElements,
@@ -1794,9 +1882,9 @@
             sidewalks=tuple(sidewalks),
             shoulders=tuple(shoulders),
             tolerance=self.tolerance,
             roadRegion=combine(roads),
             laneRegion=combine(lanes),
             intersectionRegion=combine(intersections),
             crossingRegion=combine(crossings),
-            sidewalkRegion=combine(sidewalks)
+            sidewalkRegion=combine(sidewalks),
         )
```

### Comparing `scenic-2.1.0b4/src/scenic/simulators/carla/behaviors.scenic` & `scenic-3.0.0b2/src/scenic/simulators/carla/behaviors.scenic`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """Behaviors for dynamic agents in CARLA scenarios."""
 
 from scenic.domains.driving.behaviors import *	# use common driving behaviors
-import scenic.domains.driving.model as _model
 
 try:
     from scenic.simulators.carla.actions import *
 except ModuleNotFoundError:
     pass    # ignore; error will be caught later if user attempts to run a simulation
 
 behavior AutopilotBehavior():
     """Behavior causing a vehicle to use CARLA's built-in autopilot."""
     take SetAutopilotAction(True)
 
 behavior WalkForwardBehavior(speed=0.5):
-	take SetWalkingDirectionAction(self.heading), SetWalkingSpeedAction(speed)
+    take SetWalkingDirectionAction(self.heading), SetWalkingSpeedAction(speed)
 
 behavior WalkBehavior(maxSpeed=1.4):
-	take SetWalkAction(True, maxSpeed)
+    take SetWalkAction(True, maxSpeed)
 
 behavior CrossingBehavior(reference_actor, min_speed=1, threshold=10, final_speed=None):
     """
     This behavior dynamically controls the speed of an actor that will perpendicularly (or close to)
     cross the road, so that it arrives at a spot in the road at the same time as a reference actor.
 
     Args:
@@ -50,16 +49,16 @@
         ref_speed = reference_actor.speed
         ref_time = ref_speed / ref_dist
 
         actor_speed = actor_dist * ref_time
         if actor_speed < min_speed:
             actor_speed = min_speed
 
-        if isinstance(self, _model.Walks):
+        if isinstance(self, Walks):
             do WalkForwardBehavior(actor_speed)
-        elif isinstance(self, _model.Steers):
+        elif isinstance(self, Steers):
             take SetSpeedAction(actor_speed)
 
-    if isinstance(self, _model.Walks):
+    if isinstance(self, Walks):
         do WalkForwardBehavior(final_speed)
-    elif isinstance(self, _model.Steers):
+    elif isinstance(self, Steers):
         take SetSpeedAction(final_speed)
```

### Comparing `scenic-2.1.0b4/src/scenic/simulators/carla/blueprints.scenic` & `scenic-3.0.0b2/src/scenic/simulators/carla/blueprints.scenic`

 * *Files identical despite different names*

### Comparing `scenic-2.1.0b4/src/scenic/simulators/carla/misc.py` & `scenic-3.0.0b2/src/scenic/simulators/carla/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 #
 # This work is licensed under the terms of the MIT license.
 # For a copy, see <https://opensource.org/licenses/MIT>.
 
 """ Module with auxiliary functions. """
 
 import math
-import numpy as np
+
 import carla
+import numpy as np
+
 
 def draw_waypoints(world, waypoints, z=0.5):
     """
     Draw a list of waypoints at a certain height given in z.
 
         :param world: carla.world object
         :param waypoints: list or iterable container with the waypoints to draw
@@ -33,86 +35,113 @@
     Compute speed of a vehicle in Km/h.
 
         :param vehicle: the vehicle for which speed is calculated
         :return: speed as a float in Km/h
     """
     vel = vehicle.get_velocity()
 
-    return 3.6 * math.sqrt(vel.x ** 2 + vel.y ** 2 + vel.z ** 2)
+    return 3.6 * math.sqrt(vel.x**2 + vel.y**2 + vel.z**2)
+
 
 def is_within_distance_ahead(target_transform, current_transform, max_distance):
     """
     Check if a target object is within a certain distance in front of a reference object.
 
     :param target_transform: location of the target object
     :param current_transform: location of the reference object
     :param orientation: orientation of the reference object
     :param max_distance: maximum allowed distance
     :return: True if target object is within max_distance ahead of the reference object
     """
-    target_vector = np.array([target_transform.location.x - current_transform.location.x, target_transform.location.y - current_transform.location.y])
+    target_vector = np.array(
+        [
+            target_transform.location.x - current_transform.location.x,
+            target_transform.location.y - current_transform.location.y,
+        ]
+    )
     norm_target = np.linalg.norm(target_vector)
 
     # If the vector is too short, we can simply stop here
     if norm_target < 0.001:
         return True
 
     if norm_target > max_distance:
         return False
 
     fwd = current_transform.get_forward_vector()
     forward_vector = np.array([fwd.x, fwd.y])
-    d_angle = math.degrees(math.acos(np.clip(np.dot(forward_vector, target_vector) / norm_target, -1., 1.)))
+    d_angle = math.degrees(
+        math.acos(np.clip(np.dot(forward_vector, target_vector) / norm_target, -1.0, 1.0))
+    )
 
     return d_angle < 90.0
 
-def is_within_distance(target_location, current_location, orientation, max_distance, d_angle_th_up, d_angle_th_low=0):
+
+def is_within_distance(
+    target_location,
+    current_location,
+    orientation,
+    max_distance,
+    d_angle_th_up,
+    d_angle_th_low=0,
+):
     """
     Check if a target object is within a certain distance from a reference object.
     A vehicle in front would be something around 0 deg, while one behind around 180 deg.
 
         :param target_location: location of the target object
         :param current_location: location of the reference object
         :param orientation: orientation of the reference object
         :param max_distance: maximum allowed distance
         :param d_angle_th_up: upper thereshold for angle
         :param d_angle_th_low: low thereshold for angle (optional, default is 0)
         :return: True if target object is within max_distance ahead of the reference object
     """
-    target_vector = np.array([target_location.x - current_location.x, target_location.y - current_location.y])
+    target_vector = np.array(
+        [target_location.x - current_location.x, target_location.y - current_location.y]
+    )
     norm_target = np.linalg.norm(target_vector)
 
     # If the vector is too short, we can simply stop here
     if norm_target < 0.001:
         return True
 
     if norm_target > max_distance:
         return False
 
     forward_vector = np.array(
-        [math.cos(math.radians(orientation)), math.sin(math.radians(orientation))])
-    d_angle = math.degrees(math.acos(np.clip(np.dot(forward_vector, target_vector) / norm_target, -1., 1.)))
+        [math.cos(math.radians(orientation)), math.sin(math.radians(orientation))]
+    )
+    d_angle = math.degrees(
+        math.acos(np.clip(np.dot(forward_vector, target_vector) / norm_target, -1.0, 1.0))
+    )
 
     return d_angle_th_low < d_angle < d_angle_th_up
 
 
 def compute_magnitude_angle(target_location, current_location, orientation):
     """
     Compute relative angle and distance between a target_location and a current_location
 
         :param target_location: location of the target object
         :param current_location: location of the reference object
         :param orientation: orientation of the reference object
         :return: a tuple composed by the distance to the object and the angle between both objects
     """
-    target_vector = np.array([target_location.x - current_location.x, target_location.y - current_location.y])
+    target_vector = np.array(
+        [target_location.x - current_location.x, target_location.y - current_location.y]
+    )
     norm_target = np.linalg.norm(target_vector)
 
-    forward_vector = np.array([math.cos(math.radians(orientation)), math.sin(math.radians(orientation))])
-    d_angle = math.degrees(math.acos(np.clip(np.dot(forward_vector, target_vector) / norm_target, -1., 1.)))
+    forward_vector = np.array(
+        [math.cos(math.radians(orientation)), math.sin(math.radians(orientation))]
+    )
+    d_angle = math.degrees(
+        math.acos(np.clip(np.dot(forward_vector, target_vector) / norm_target, -1.0, 1.0))
+    )
 
     return (norm_target, d_angle)
 
 
 def distance_vehicle(waypoint, vehicle_transform):
     """
     Returns the 2D distance from a waypoint to a vehicle
@@ -157,9 +186,7 @@
 def positive(num):
     """
     Return the given number if positive, else 0
 
         :param num: value to check
     """
     return num if num > 0.0 else 0.0
-
-
```

### Comparing `scenic-2.1.0b4/src/scenic/simulators/carla/model.scenic` & `scenic-3.0.0b2/src/scenic/simulators/carla/model.scenic`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,19 @@
 
 try:
     from scenic.simulators.carla.simulator import CarlaSimulator    # for use in scenarios
     from scenic.simulators.carla.actions import *
     import scenic.simulators.carla.utils.utils as _utils
 except ModuleNotFoundError:
     # for convenience when testing without the carla package
+    from scenic.core.simulators import SimulatorInterfaceWarning
     import warnings
     warnings.warn('the "carla" package is not installed; '
-                  'will not be able to run dynamic simulations')
+                  'will not be able to run dynamic simulations',
+                  SimulatorInterfaceWarning)
 
     def CarlaSimulator(*args, **kwargs):
         """Dummy simulator to allow compilation without the 'carla' package.
 
         :meta private:
         """
         raise RuntimeError('the "carla" package is required to run simulations '
@@ -159,15 +161,15 @@
     def _getClosestTrafficLight(self, distance=100):
         return _getClosestTrafficLight(self, distance)
 
 class Car(Vehicle):
     """A car.
 
     The default ``blueprint`` (see `CarlaActor`) is a uniform distribution over the
-    blueprints listed in `scenic.simulators.carla.blueprints.carModels`.
+    blueprints listed in :obj:`scenic.simulators.carla.blueprints.carModels`.
     """
     blueprint: Uniform(*blueprints.carModels)
 
     @property
     def isCar(self):
         return True
 
@@ -192,39 +194,38 @@
     blueprint: Uniform(*blueprints.truckModels)
 
 
 class Pedestrian(Pedestrian, CarlaActor, Walks):
     """A pedestrian.
 
     The default ``blueprint`` (see `CarlaActor`) is a uniform distribution over the
-    blueprints listed in `scenic.simulators.carla.blueprints.walkerModels`.
+    blueprints listed in :obj:`scenic.simulators.carla.blueprints.walkerModels`.
     """
     width: 0.5
     length: 0.5
     blueprint: Uniform(*blueprints.walkerModels)
     carlaController: None
 
     def setWalkingDirection(self, heading):
-        direction = Vector(0, 1).rotatedBy(heading)
-        zComp = self.control.direction.z
-        self.control.direction = _utils.scenicToCarlaVector3D(*direction, zComp)
+        direction = Vector(0, 1, 0).rotatedBy(heading)
+        self.control.direction = _utils.scenicToCarlaVector3D(*direction)
 
     def setWalkingSpeed(self, speed):
         self.control.speed = speed
 
 
 class Prop(CarlaActor):
     """Abstract class for props, i.e. non-moving objects.
 
     Properties:
         heading (float): Default value overridden to be uniformly random.
         physics (bool): Default value overridden to be false.
     """
     regionContainedIn: road
-    position: Point on road
+    position: new Point on road
     heading: Range(0, 360) deg
     width: 0.5
     length: 0.5
     physics: False
 
 class Trash(Prop):
     blueprint: Uniform(*blueprints.trashModels)
```

### Comparing `scenic-2.1.0b4/src/scenic/simulators/carla/utils/visuals.py` & `scenic-3.0.0b2/src/scenic/simulators/carla/utils/visuals.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,201 +22,223 @@
 # BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 import datetime
 import math
 import weakref
-import pygame
-import numpy as np
+
 import carla
 from carla import ColorConverter as cc
+import numpy as np
+import pygame
 
 
 def get_actor_display_name(actor, truncate=250):
-    name = ' '.join(actor.type_id.replace('_', '.').title().split('.')[1:])
-    return (name[:truncate-1] + u'\u2026') if len(name) > truncate else name
+    name = " ".join(actor.type_id.replace("_", ".").title().split(".")[1:])
+    return (name[: truncate - 1] + "\u2026") if len(name) > truncate else name
 
 
 # ==============================================================================
 # -- HUD -----------------------------------------------------------------------
 # ==============================================================================
 
+
 class HUD(object):
-	def __init__(self, width, height):
-		self.dim = (width, height)
-		font = pygame.font.Font(pygame.font.get_default_font(), 20)
-		fonts = [x for x in pygame.font.get_fonts() if 'mono' in x]
-		default_font = 'ubuntumono'
-		mono = default_font if default_font in fonts else fonts[0]
-		mono = pygame.font.match_font(mono)
-		self._font_mono = pygame.font.Font(mono, 14)
-		self._notifications = FadingText(font, (width, 40), (0, height - 40))
-		self.server_fps = 0
-		self.frame = 0
-		self.simulation_time = 0
-		self._info_text = []
-		self._server_clock = pygame.time.Clock()
-
-	def on_world_tick(self, timestamp):
-		self._server_clock.tick()
-		self.server_fps = self._server_clock.get_fps()
-		self.frame = timestamp.frame
-		self.simulation_time = timestamp.elapsed_seconds
-
-	def tick(self, world, ego, clock, showLabels=True):
-		if ego.carlaActor is None:
-			return  # ego not spawned yet
-
-		t = ego.carlaActor.get_transform()
-		v = ego.carlaActor.get_velocity()
-		c = ego.carlaActor.get_control()
-
-		heading = 'N' if abs(t.rotation.yaw) < 89.5 else ''
-		heading += 'S' if abs(t.rotation.yaw) > 90.5 else ''
-		heading += 'E' if 179.5 > t.rotation.yaw > 0.5 else ''
-		heading += 'W' if -0.5 > t.rotation.yaw > -179.5 else ''
-
-		#colhist = collisionSensor.get_collision_history()
-		#collision = [colhist[x + self.frame - 200] for x in range(0, 200)]
-		#max_col = max(1.0, max(collision))
-		#collision = [x / max_col for x in collision]
-
-		vehicles = world.get_actors().filter('vehicle.*')
-		pedestrians = world.get_actors().filter('walker.pedestrian.*')
-
-		self._info_text = [
-			'Server:  % 16d FPS' % self.server_fps,
-			'Map:	 % 20s' % world.get_map().name,
-			'Simulation time: % 12s' % datetime.timedelta(seconds=int(self.simulation_time)),
-			'',
-			'Number of vehicles: % 8d' % len(vehicles),
-			'Number of pedestrians: % 8d' % len(pedestrians),
-			'',
-			'Ego: % 20s' % get_actor_display_name(ego.carlaActor, truncate=20),
-			'',
-			'Speed:   % 15.0f m/s' % math.sqrt(v.x**2 + v.y**2 + v.z**2),
-			u'Heading:% 16.0f\N{DEGREE SIGN} % 2s' % (t.rotation.yaw, heading),
-			'Location:% 20s' % ('(% 5.3f, % 5.3f)' % (t.location.x, t.location.y)),
-			'Height:  % 18.0f m' % t.location.z,
-		]
-
-		try:
-			_control_text = [
-				'',
-				('Throttle:', c.throttle, 0.0, 1.0),
-				('Steer:', c.steer, -1.0, 1.0),
-				('Brake:', c.brake, 0.0, 1.0),
-				('Reverse:', c.reverse),
-				('Hand brake:', c.hand_brake),
-				('Manual:', c.manual_gear_shift),
-				'Gear:		%s' % {-1: 'R', 0: 'N'}.get(c.gear, c.gear),
-				#'',
-				#'Collision:', collision,
-			]
-		except:
-			_control_text = []
-		finally:
-			self._info_text.extend(_control_text)
-
-		if len(vehicles) > 1:
-			self._info_text += ['Nearby vehicles:']
-			distance = lambda l: math.sqrt((l.x - t.location.x)**2 + (l.y - t.location.y)**2 + (l.z - t.location.z)**2)
-			vehicles = [(distance(x.get_location()), x)
-						for x in vehicles if x.id != ego.carlaActor.id]
-			for d, vehicle in sorted(vehicles):
-				if d > 200.0:
-					break
-				vehicle_type = get_actor_display_name(vehicle, truncate=22)
-				self._info_text.append('% 4dm %s' % (d, vehicle_type))
-
-	def render(self, display):
-		info_surface = pygame.Surface((220, self.dim[1]))
-		info_surface.set_alpha(100)
-		display.blit(info_surface, (0, 0))
-		v_offset = 4
-		bar_h_offset = 100
-		bar_width = 106
-		for item in self._info_text:
-			if v_offset + 18 > self.dim[1]:
-				break
-			if isinstance(item, list):
-				if len(item) > 1:
-					points = [(x + 8, v_offset + 8 + (1.0 - y) * 30) for x, y in enumerate(item)]
-					pygame.draw.lines(display, (255, 136, 0), False, points, 2)
-				item = None
-				v_offset += 18
-			elif isinstance(item, tuple):
-				if isinstance(item[1], bool):
-					rect = pygame.Rect((bar_h_offset, v_offset + 8), (6, 6))
-					pygame.draw.rect(display, (255, 255, 255), rect, 0 if item[1] else 1)
-				else:
-					rect_border = pygame.Rect((bar_h_offset, v_offset + 8), (bar_width, 6))
-					pygame.draw.rect(display, (255, 255, 255), rect_border, 1)
-					f = (item[1] - item[2]) / (item[3] - item[2])
-					if item[2] < 0.0:
-						rect = pygame.Rect((bar_h_offset + f * (bar_width - 6), v_offset + 8), (6, 6))
-					else:
-						rect = pygame.Rect((bar_h_offset, v_offset + 8), (f * bar_width, 6))
-					pygame.draw.rect(display, (255, 255, 255), rect)
-				item = item[0]
-			if item: # At this point has to be a str
-				surface = self._font_mono.render(item, True, (255, 255, 255))
-				display.blit(surface, (8, v_offset))
-			v_offset += 18
+    def __init__(self, width, height):
+        self.dim = (width, height)
+        font = pygame.font.Font(pygame.font.get_default_font(), 20)
+        fonts = [x for x in pygame.font.get_fonts() if "mono" in x]
+        default_font = "ubuntumono"
+        mono = default_font if default_font in fonts else fonts[0]
+        mono = pygame.font.match_font(mono)
+        self._font_mono = pygame.font.Font(mono, 14)
+        self._notifications = FadingText(font, (width, 40), (0, height - 40))
+        self.server_fps = 0
+        self.frame = 0
+        self.simulation_time = 0
+        self._info_text = []
+        self._server_clock = pygame.time.Clock()
+
+    def on_world_tick(self, timestamp):
+        self._server_clock.tick()
+        self.server_fps = self._server_clock.get_fps()
+        self.frame = timestamp.frame
+        self.simulation_time = timestamp.elapsed_seconds
+
+    def tick(self, world, ego, clock, showLabels=True):
+        if ego.carlaActor is None:
+            return  # ego not spawned yet
+
+        t = ego.carlaActor.get_transform()
+        v = ego.carlaActor.get_velocity()
+        c = ego.carlaActor.get_control()
+
+        heading = "N" if abs(t.rotation.yaw) < 89.5 else ""
+        heading += "S" if abs(t.rotation.yaw) > 90.5 else ""
+        heading += "E" if 179.5 > t.rotation.yaw > 0.5 else ""
+        heading += "W" if -0.5 > t.rotation.yaw > -179.5 else ""
+
+        # colhist = collisionSensor.get_collision_history()
+        # collision = [colhist[x + self.frame - 200] for x in range(0, 200)]
+        # max_col = max(1.0, max(collision))
+        # collision = [x / max_col for x in collision]
+
+        vehicles = world.get_actors().filter("vehicle.*")
+        pedestrians = world.get_actors().filter("walker.pedestrian.*")
+
+        self._info_text = [
+            "Server:  % 16d FPS" % self.server_fps,
+            "Map:    % 20s" % world.get_map().name,
+            "Simulation time: % 12s"
+            % datetime.timedelta(seconds=int(self.simulation_time)),
+            "",
+            "Number of vehicles: % 8d" % len(vehicles),
+            "Number of pedestrians: % 8d" % len(pedestrians),
+            "",
+            "Ego: % 20s" % get_actor_display_name(ego.carlaActor, truncate=20),
+            "",
+            "Speed:   % 15.0f m/s" % math.sqrt(v.x**2 + v.y**2 + v.z**2),
+            "Heading:% 16.0f\N{DEGREE SIGN} % 2s" % (t.rotation.yaw, heading),
+            "Location:% 20s" % ("(% 5.3f, % 5.3f)" % (t.location.x, t.location.y)),
+            "Height:  % 18.0f m" % t.location.z,
+        ]
+
+        try:
+            _control_text = [
+                "",
+                ("Throttle:", c.throttle, 0.0, 1.0),
+                ("Steer:", c.steer, -1.0, 1.0),
+                ("Brake:", c.brake, 0.0, 1.0),
+                ("Reverse:", c.reverse),
+                ("Hand brake:", c.hand_brake),
+                ("Manual:", c.manual_gear_shift),
+                "Gear:      %s" % {-1: "R", 0: "N"}.get(c.gear, c.gear),
+                #'',
+                #'Collision:', collision,
+            ]
+        except:
+            _control_text = []
+        finally:
+            self._info_text.extend(_control_text)
+
+        if len(vehicles) > 1:
+            self._info_text += ["Nearby vehicles:"]
+            distance = lambda l: math.sqrt(
+                (l.x - t.location.x) ** 2
+                + (l.y - t.location.y) ** 2
+                + (l.z - t.location.z) ** 2
+            )
+            vehicles = [
+                (distance(x.get_location()), x)
+                for x in vehicles
+                if x.id != ego.carlaActor.id
+            ]
+            for d, vehicle in sorted(vehicles):
+                if d > 200.0:
+                    break
+                vehicle_type = get_actor_display_name(vehicle, truncate=22)
+                self._info_text.append("% 4dm %s" % (d, vehicle_type))
+
+    def render(self, display):
+        info_surface = pygame.Surface((220, self.dim[1]))
+        info_surface.set_alpha(100)
+        display.blit(info_surface, (0, 0))
+        v_offset = 4
+        bar_h_offset = 100
+        bar_width = 106
+        for item in self._info_text:
+            if v_offset + 18 > self.dim[1]:
+                break
+            if isinstance(item, list):
+                if len(item) > 1:
+                    points = [
+                        (x + 8, v_offset + 8 + (1.0 - y) * 30) for x, y in enumerate(item)
+                    ]
+                    pygame.draw.lines(display, (255, 136, 0), False, points, 2)
+                item = None
+                v_offset += 18
+            elif isinstance(item, tuple):
+                if isinstance(item[1], bool):
+                    rect = pygame.Rect((bar_h_offset, v_offset + 8), (6, 6))
+                    pygame.draw.rect(display, (255, 255, 255), rect, 0 if item[1] else 1)
+                else:
+                    rect_border = pygame.Rect(
+                        (bar_h_offset, v_offset + 8), (bar_width, 6)
+                    )
+                    pygame.draw.rect(display, (255, 255, 255), rect_border, 1)
+                    f = (item[1] - item[2]) / (item[3] - item[2])
+                    if item[2] < 0.0:
+                        rect = pygame.Rect(
+                            (bar_h_offset + f * (bar_width - 6), v_offset + 8), (6, 6)
+                        )
+                    else:
+                        rect = pygame.Rect(
+                            (bar_h_offset, v_offset + 8), (f * bar_width, 6)
+                        )
+                    pygame.draw.rect(display, (255, 255, 255), rect)
+                item = item[0]
+            if item:  # At this point has to be a str
+                surface = self._font_mono.render(item, True, (255, 255, 255))
+                display.blit(surface, (8, v_offset))
+            v_offset += 18
 
 
 # ==============================================================================
 # -- FadingText ----------------------------------------------------------------
 # ==============================================================================
 
+
 class FadingText(object):
-	def __init__(self, font, dim, pos):
-		self.font = font
-		self.dim = dim
-		self.pos = pos
-		self.seconds_left = 0
-		self.surface = pygame.Surface(self.dim)
-
-	def set_text(self, text, color=(255, 255, 255), seconds=2.0):
-		text_texture = self.font.render(text, True, color)
-		self.surface = pygame.Surface(self.dim)
-		self.seconds_left = seconds
-		self.surface.fill((0, 0, 0, 0))
-		self.surface.blit(text_texture, (10, 11))
-
-	def tick(self, _, clock):
-		delta_seconds = 1e-3 * clock.get_time()
-		self.seconds_left = max(0.0, self.seconds_left - delta_seconds)
-		self.surface.set_alpha(500.0 * self.seconds_left)
+    def __init__(self, font, dim, pos):
+        self.font = font
+        self.dim = dim
+        self.pos = pos
+        self.seconds_left = 0
+        self.surface = pygame.Surface(self.dim)
+
+    def set_text(self, text, color=(255, 255, 255), seconds=2.0):
+        text_texture = self.font.render(text, True, color)
+        self.surface = pygame.Surface(self.dim)
+        self.seconds_left = seconds
+        self.surface.fill((0, 0, 0, 0))
+        self.surface.blit(text_texture, (10, 11))
+
+    def tick(self, _, clock):
+        delta_seconds = 1e-3 * clock.get_time()
+        self.seconds_left = max(0.0, self.seconds_left - delta_seconds)
+        self.surface.set_alpha(500.0 * self.seconds_left)
 
-	def render(self, display):
-		display.blit(self.surface, self.pos)
+    def render(self, display):
+        display.blit(self.surface, self.pos)
 
 
 # ==============================================================================
 # -- CollisionSensor -----------------------------------------------------------
 # ==============================================================================
 
+
 class CollisionSensor(object):
     def __init__(self, world, actor, hud=None):
         self.sensor = None
         self._history = []
         self._actor = actor
         self._actor_mass = actor.get_physics_control().mass
         self._hud = hud
         self._world = world
-        bp = self._world.get_blueprint_library().find('sensor.other.collision')
-        self.sensor = self._world.spawn_actor(bp, carla.Transform(), attach_to=self._actor)
+        bp = self._world.get_blueprint_library().find("sensor.other.collision")
+        self.sensor = self._world.spawn_actor(
+            bp, carla.Transform(), attach_to=self._actor
+        )
         # Pass the lambda a weak reference to self to avoid circular reference
         weak_self = weakref.ref(self)
         self.sensor.listen(lambda event: CollisionSensor._on_collision(weak_self, event))
 
     def get_collision_speeds(self):
-        '''Convert collision intensities from momentem (kg*m/s) to speed (m/s).'''
+        """Convert collision intensities from momentem (kg*m/s) to speed (m/s)."""
         return [(c[0], c[1] / self._actor_mass) for c in self._history]
 
     def get_collision_history(self):
         history = collections.defaultdict(int)
         for frame, intensity in self._history:
             history[frame] += intensity
         return history
@@ -224,109 +246,128 @@
     @staticmethod
     def _on_collision(weak_self, event):
         self = weak_self()
         if not self:
             return
         actor_type = get_actor_display_name(event.other_actor)
         if self._hud:
-            self._hud.notification('Collision with %r, id = %d'
-                                   % (actor_type, event.other_actor.id))
+            self._hud.notification(
+                "Collision with %r, id = %d" % (actor_type, event.other_actor.id)
+            )
         impulse = event.normal_impulse
-        intensity = math.sqrt(impulse.x ** 2 + impulse.y ** 2 + impulse.z ** 2)
+        intensity = math.sqrt(impulse.x**2 + impulse.y**2 + impulse.z**2)
         self._history.append((event.frame, intensity))
         if len(self._history) > 4000:
             self._history.pop(0)
 
 
 # ==============================================================================
 # -- CameraManager -------------------------------------------------------------
 # ==============================================================================
 
+
 class CameraManager(object):
-	def __init__(self, world, actor, hud):
-		self.sensor = None
-		self._surface = None
-		self._actor = actor
-		self._hud = hud
-		self.images = []
-		self._camera_transforms = [
-			carla.Transform(carla.Location(x=-5.5, z=2.8), carla.Rotation(pitch=-15)),
-			carla.Transform(carla.Location(x=1.6, z=1.7))]
-		self._transform_index = 1
-		self._sensors = [
-			['sensor.camera.rgb', cc.Raw, 'Camera RGB'],
-			['sensor.camera.depth', cc.Raw, 'Camera Depth (Raw)'],
-			['sensor.camera.depth', cc.Depth, 'Camera Depth (Gray Scale)'],
-			['sensor.camera.depth', cc.LogarithmicDepth, 'Camera Depth (Logarithmic Gray Scale)'],
-			['sensor.camera.semantic_segmentation', cc.Raw, 'Camera Semantic Segmentation (Raw)'],
-			['sensor.camera.semantic_segmentation', cc.CityScapesPalette,
-			 'Camera Semantic Segmentation (CityScapes Palette)'],
-			['sensor.lidar.ray_cast', None, 'Lidar (Ray-Cast)']]
-		self._world = world
-		bp_library = self._world.get_blueprint_library()
-		for item in self._sensors:
-			bp = bp_library.find(item[0])
-			if item[0].startswith('sensor.camera'):
-				bp.set_attribute('image_size_x', str(hud.dim[0]))
-				bp.set_attribute('image_size_y', str(hud.dim[1]))
-			item.append(bp)
-		self._index = None
-
-	def toggle_camera(self):
-		set_transform((self._transform_index + 1) % len(self._camera_transforms))
-
-	def set_transform(self, idx):
-		self._transform_index = idx
-		self.sensor.set_transform(self._camera_transforms[self._transform_index])
-
-	def set_sensor(self, index):
-		index = index % len(self._sensors)
-		needs_respawn = True if self._index is None \
-			else self._sensors[index][0] != self._sensors[self._index][0]
-		if needs_respawn:
-			if self.sensor is not None:
-				self.sensor.destroy()
-				self._surface = None
-			self.sensor = self._world.spawn_actor(
-				self._sensors[index][-1],
-				self._camera_transforms[self._transform_index],
-				attach_to=self._actor)
-			# Pass lambda a weak reference to self to avoid circular reference
-			weak_self = weakref.ref(self)
-			self.sensor.listen(lambda image: CameraManager._parse_image(weak_self, image))
-		self._index = index
-
-	def render(self, display):
-		if self._surface is not None:
-			display.blit(self._surface, (0, 0))
-
-	@staticmethod
-	def _parse_image(weak_self, image):
-		self = weak_self()
-		if not self:
-			return
-		if self._sensors[self._index][0].startswith('sensor.lidar'):
-			points = np.frombuffer(image.raw_data, dtype=np.dtype('f4'))
-			points = np.reshape(points, (int(points.shape[0] / 3), 3))
-			lidar_data = np.array(points[:, :2])
-			lidar_data *= min(self._hud.dim) / 100.0
-			lidar_data += (0.5 * self._hud.dim[0], 0.5 * self._hud.dim[1])
-			lidar_data = np.fabs(lidar_data)
-			lidar_data = lidar_data.astype(np.int32)
-			lidar_data = np.reshape(lidar_data, (-1, 2))
-			lidar_img_size = (self._hud.dim[0], self._hud.dim[1], 3)
-			lidar_img = np.zeros(lidar_img_size)
-			lidar_img[tuple(lidar_data.T)] = (255, 255, 255)
-			self._surface = pygame.surfarray.make_surface(lidar_img)
-		else:
-			image.convert(self._sensors[self._index][1])
-			array = np.frombuffer(image.raw_data, dtype=np.dtype("uint8"))
-			array = np.reshape(array, (image.height, image.width, 4))
-			array = array[:, :, :3]
-			array = array[:, :, ::-1]
-			self._surface = pygame.surfarray.make_surface(array.swapaxes(0, 1))
-		self.images.append(image)
-
-	def destroy_sensor(self):
-		if self.sensor is not None:
-			self.sensor.stop()
-			self.sensor.destroy()
+    def __init__(self, world, actor, hud):
+        self.sensor = None
+        self._surface = None
+        self._actor = actor
+        self._hud = hud
+        self.images = []
+        self._camera_transforms = [
+            carla.Transform(carla.Location(x=-5.5, z=2.8), carla.Rotation(pitch=-15)),
+            carla.Transform(carla.Location(x=1.6, z=1.7)),
+        ]
+        self._transform_index = 1
+        self._sensors = [
+            ["sensor.camera.rgb", cc.Raw, "Camera RGB"],
+            ["sensor.camera.depth", cc.Raw, "Camera Depth (Raw)"],
+            ["sensor.camera.depth", cc.Depth, "Camera Depth (Gray Scale)"],
+            [
+                "sensor.camera.depth",
+                cc.LogarithmicDepth,
+                "Camera Depth (Logarithmic Gray Scale)",
+            ],
+            [
+                "sensor.camera.semantic_segmentation",
+                cc.Raw,
+                "Camera Semantic Segmentation (Raw)",
+            ],
+            [
+                "sensor.camera.semantic_segmentation",
+                cc.CityScapesPalette,
+                "Camera Semantic Segmentation (CityScapes Palette)",
+            ],
+            ["sensor.lidar.ray_cast", None, "Lidar (Ray-Cast)"],
+        ]
+        self._world = world
+        bp_library = self._world.get_blueprint_library()
+        for item in self._sensors:
+            bp = bp_library.find(item[0])
+            if item[0].startswith("sensor.camera"):
+                bp.set_attribute("image_size_x", str(hud.dim[0]))
+                bp.set_attribute("image_size_y", str(hud.dim[1]))
+            item.append(bp)
+        self._index = None
+
+    def toggle_camera(self):
+        set_transform((self._transform_index + 1) % len(self._camera_transforms))
+
+    def set_transform(self, idx):
+        self._transform_index = idx
+        self.sensor.set_transform(self._camera_transforms[self._transform_index])
+
+    def set_sensor(self, index):
+        index = index % len(self._sensors)
+        needs_respawn = (
+            True
+            if self._index is None
+            else self._sensors[index][0] != self._sensors[self._index][0]
+        )
+        if needs_respawn:
+            if self.sensor is not None:
+                self.sensor.destroy()
+                self._surface = None
+            self.sensor = self._world.spawn_actor(
+                self._sensors[index][-1],
+                self._camera_transforms[self._transform_index],
+                attach_to=self._actor,
+            )
+            # Pass lambda a weak reference to self to avoid circular reference
+            weak_self = weakref.ref(self)
+            self.sensor.listen(lambda image: CameraManager._parse_image(weak_self, image))
+        self._index = index
+
+    def render(self, display):
+        if self._surface is not None:
+            display.blit(self._surface, (0, 0))
+
+    @staticmethod
+    def _parse_image(weak_self, image):
+        self = weak_self()
+        if not self:
+            return
+        if self._sensors[self._index][0].startswith("sensor.lidar"):
+            points = np.frombuffer(image.raw_data, dtype=np.dtype("f4"))
+            points = np.reshape(points, (int(points.shape[0] / 3), 3))
+            lidar_data = np.array(points[:, :2])
+            lidar_data *= min(self._hud.dim) / 100.0
+            lidar_data += (0.5 * self._hud.dim[0], 0.5 * self._hud.dim[1])
+            lidar_data = np.fabs(lidar_data)
+            lidar_data = lidar_data.astype(np.int32)
+            lidar_data = np.reshape(lidar_data, (-1, 2))
+            lidar_img_size = (self._hud.dim[0], self._hud.dim[1], 3)
+            lidar_img = np.zeros(lidar_img_size)
+            lidar_img[tuple(lidar_data.T)] = (255, 255, 255)
+            self._surface = pygame.surfarray.make_surface(lidar_img)
+        else:
+            image.convert(self._sensors[self._index][1])
+            array = np.frombuffer(image.raw_data, dtype=np.dtype("uint8"))
+            array = np.reshape(array, (image.height, image.width, 4))
+            array = array[:, :, :3]
+            array = array[:, :, ::-1]
+            self._surface = pygame.surfarray.make_surface(array.swapaxes(0, 1))
+        self.images.append(image)
+
+    def destroy_sensor(self):
+        if self.sensor is not None:
+            self.sensor.stop()
+            self.sensor.destroy()
```

### Comparing `scenic-2.1.0b4/src/scenic/simulators/gta/center_detection.py` & `scenic-3.0.0b2/src/scenic/simulators/gta/center_detection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,108 +1,99 @@
-'''
+"""
 This file contains helper functions
-'''
+"""
 
+from copy import deepcopy
 import itertools
 from typing import NamedTuple, Tuple
-from copy import deepcopy
 
 from scenic.simulators.gta.img_modf import *
 
-'''
+"""
 Compute neighbors of a given point/pixel
-'''
+"""
+
+
 def generate_neighbors(x):
     delta = np.arange(-1, 2)
     grid_delta = np.array(list(itertools.product(delta, delta)))
-    return np.array(x)+ grid_delta
+    return np.array(x) + grid_delta
 
 
-'''
+"""
 Generate circle of a given radius and transformed by a center and a theta
-'''
+"""
+
+
 def generate_circle(radius, num_samples, theta, center):
     transformed_center = transform_center(center, radius, theta)
-    thetas = np.linspace(0, 2*np.pi+0.01, num_samples)
-    return transformed_center[0] + radius*np.cos(thetas), \
-           transformed_center[1] + radius*np.sin(thetas)
+    thetas = np.linspace(0, 2 * np.pi + 0.01, num_samples)
+    return transformed_center[0] + radius * np.cos(thetas), transformed_center[
+        1
+    ] + radius * np.sin(thetas)
 
-'''
+
+"""
 Transform the circle center as x+r*cos(90+theta) and y-r*sin(90+theta)
-'''
+"""
+
+
 def transform_center(center, radius, theta):
-    return [center[0] + radius * np.cos(theta), center[1] - radius * np.sin(
-        theta)]
+    return [center[0] + radius * np.cos(theta), center[1] - radius * np.sin(theta)]
 
 
-'''
+"""
 Compute image gradients from sobel edge detector
-'''
-def compute_gradient_sobel(img_data=None, img_file=None, threshold=100,
-                     kernelsize=1, bw_kernelsize=3):
+"""
+
+
+def compute_gradient_sobel(
+    img_data=None, img_file=None, threshold=100, kernelsize=1, bw_kernelsize=3
+):
     assert img_data is not None or img_file is not None
     if img_data is None:
         img_data = Image.open(img_file)
 
     img_copy = img_data.copy()
 
     # Get the black and white image
-    img_bw = convert_black_white(img_data=img_copy, img_file=img_file,
-                                 threshold=threshold)
+    img_bw = convert_black_white(
+        img_data=img_copy, img_file=img_file, threshold=threshold
+    )
     cv_bw = cv2.cvtColor(np.array(img_bw), cv2.COLOR_RGB2BGR)
 
     # Gradients along x, y. The laplacian used for edge detection is actually
     #  a combination of these two
     sobelx = cv2.Sobel(cv_bw, cv2.CV_64F, 1, 0, ksize=kernelsize)
     sobely = cv2.Sobel(cv_bw, cv2.CV_64F, 0, 1, ksize=kernelsize)
 
     angle_sobel = np.arctan(sobelx / (sobely + 1e-6))
 
-    edge_image = get_edges(img_data=img_copy, img_file=img_file,
-                           threshold=threshold, kernelsize=bw_kernelsize)
+    edge_image = get_edges(
+        img_data=img_copy,
+        img_file=img_file,
+        threshold=threshold,
+        kernelsize=bw_kernelsize,
+    )
 
     edge_x, edge_y = np.nonzero(np.asarray(edge_image))
 
     angle_along_edge = {}
     for x, y in zip(edge_x, edge_y):
-        angle_along_edge[(x,y)] = angle_sobel[x][y][0]
+        angle_along_edge[(x, y)] = angle_sobel[x][y][0]
 
     return angle_along_edge
 
-'''
-This is very coarse, avoid using this
-'''
-def compute_gradient_manual(img_data=None, img_file=None, threshold=100,
-                     kernelsize=1):
-    assert img_data is not None or img_file is not None
-    if img_data is None:
-        img_data = Image.open(img_file)
-
-    img_copy = img_data.copy()
-
-    # Directly work with the edges
-    edge_image = get_edges(img_data=img_copy, img_file=img_file,
-                           threshold=threshold, kernelsize=kernelsize)
 
-    edge_x, edge_y = np.nonzero(np.asarray(edge_image))
-    grad_x, grad_y = np.gradient(np.asarray(edge_image))
-    angle_grad = np.arctan(grad_x/(grad_y+1e-6))
-
-    angle_along_edge = {}
-    for x, y in zip(edge_x, edge_y):
-        angle_along_edge[(x,y)] = angle_grad[x][y]
-
-    return angle_along_edge
-
-'''
+"""
 Compute all connected edges
-'''
+"""
 
-def generate_connected_edges(edge_locs):
 
+def generate_connected_edges(edge_locs):
     # This is a list of collected edges
     collected_edges = []
     while len(edge_locs) > 0:
         start_point = edge_locs.pop()
         new_edge = set({start_point})
         neighbors = set(tuple(map(tuple, generate_neighbors(start_point))))
         to_visit = neighbors.intersection(edge_locs)
@@ -114,170 +105,179 @@
             to_visit.update(neighbors.intersection(edge_locs))
             new_edge.update(neighbors.intersection(edge_locs))
             edge_locs.difference_update(new_edge.intersection(edge_locs))
 
         collected_edges.append(new_edge)
     return collected_edges
 
-'''
+
+"""
 To find the center of the road perpendicular to a given point
 num_samples is function which can potentially change with the radius of the
 circle
-'''
+"""
 
-def find_center(x, theta, collected_edges, all_edges,  num_samples, bw_image):
 
-    '''
+def find_center(x, theta, collected_edges, all_edges, num_samples, bw_image):
+    """
     Find which edge x lies in
-    '''
+    """
     for edge in collected_edges:
         if tuple([x[1], x[0]]) in edge:
             x_edge = edge
             break
 
     possible_opp_edge = all_edges.difference(x_edge)
 
     r = 1
 
-    '''
+    """
     Find direction of computing the growing circles
-    '''
+    """
     if theta < 0:
-        theta = theta + 2*np.pi
-    theta_plus = theta + np.pi/2.
-    theta_minus = theta - np.pi / 2.
+        theta = theta + 2 * np.pi
+    theta_plus = theta + np.pi / 2.0
+    theta_minus = theta - np.pi / 2.0
 
     center_plus = transform_center(center=x, radius=2, theta=theta_plus)
 
     center_plus = np.array(np.around(center_plus), dtype=int)
 
     if center_plus[0] >= bw_image.shape[1]:
         center_plus[0] = bw_image.shape[1] - 1
     if center_plus[1] >= bw_image.shape[0]:
         center_plus[1] = bw_image.shape[0] - 1
     if bw_image[center_plus[1]][center_plus[0]] == 0:
         theta = theta_plus
-        tangent_theta = theta - np.pi/2.
+        tangent_theta = theta - np.pi / 2.0
     else:
         theta = theta_minus
-        tangent_theta = theta + np.pi / 2.
+        tangent_theta = theta + np.pi / 2.0
 
     while True:
-        circle_x, circle_y = generate_circle(radius=r, center=x, theta=theta,
-                                             num_samples=num_samples(r))
-
-        int_circle = set(itertools.product(np.array(np.around(circle_y),
-                        dtype=int), np.array(np.around(circle_x), dtype=int)))
-
+        circle_x, circle_y = generate_circle(
+            radius=r, center=x, theta=theta, num_samples=num_samples(r)
+        )
+
+        int_circle = set(
+            itertools.product(
+                np.array(np.around(circle_y), dtype=int),
+                np.array(np.around(circle_x), dtype=int),
+            )
+        )
 
         if len(possible_opp_edge.intersection(int_circle)) > 0:
             opp_edge = possible_opp_edge.intersection(int_circle)
             break
 
         r += 1
     if len(opp_edge) > 1:
-        arg_min = np.linalg.norm(np.array(list(opp_edge)) - np.array([x[1],
-                                x[0]]), axis=1).argmin()
+        arg_min = np.linalg.norm(
+            np.array(list(opp_edge)) - np.array([x[1], x[0]]), axis=1
+        ).argmin()
         opp_point = np.array(list(opp_edge))[arg_min]
     else:
         opp_point = opp_edge.pop()
 
-    mid_loc = np.array(np.around((np.array([x[1],x[0]]) +
-                                  np.array(opp_point))/2.), dtype=int)
+    mid_loc = np.array(
+        np.around((np.array([x[1], x[0]]) + np.array(opp_point)) / 2.0), dtype=int
+    )
 
     orig_theta = tangent_theta
 
     # When there is a clear greater than and less than
     if mid_loc[0] > x[1] and mid_loc[1] < x[0]:
         if tangent_theta > np.pi:
             tangent_theta = tangent_theta - np.pi
-        if tangent_theta < np.pi/2.:
+        if tangent_theta < np.pi / 2.0:
             tangent_theta = tangent_theta + np.pi
     elif mid_loc[0] > x[1] and mid_loc[1] > x[0]:
         if tangent_theta < np.pi:
             tangent_theta = tangent_theta + np.pi
     elif mid_loc[0] < x[1] and mid_loc[1] < x[0]:
-        if tangent_theta > np.pi/2.:
+        if tangent_theta > np.pi / 2.0:
             tangent_theta = tangent_theta - np.pi
     elif mid_loc[0] < x[1] and mid_loc[1] > x[0]:
-        if tangent_theta < 3.*np.pi/2. and tangent_theta > 0:
+        if tangent_theta < 3.0 * np.pi / 2.0 and tangent_theta > 0:
             tangent_theta = tangent_theta + np.pi
 
-
     # When there exists one equality
     if mid_loc[0] == x[1]:
         if mid_loc[1] < x[0]:
             if tangent_theta > np.pi:
                 tangent_theta = tangent_theta - np.pi
         else:
-            if tangent_theta < 3./2.*np.pi:
+            if tangent_theta < 3.0 / 2.0 * np.pi:
                 tangent_theta = tangent_theta + np.pi
 
     if mid_loc[1] == x[0]:
         if mid_loc[0] < x[1]:
-            if tangent_theta > np.pi/2.:
+            if tangent_theta > np.pi / 2.0:
                 tangent_theta = tangent_theta - np.pi
         else:
             if tangent_theta < np.pi:
                 tangent_theta = tangent_theta + np.pi
 
-
     if tangent_theta < 0:
         tangent_theta = tangent_theta + 2 * np.pi
 
-
-
-
     return orig_theta, tangent_theta, tuple(opp_point), tuple(mid_loc)
 
 
-'''
+"""
 Update all edges with the bounding box of the image
-'''
+"""
+
 
 def compute_bb(img_dimensions):
     im_x_min = -1
     im_y_min = -1
     im_x_max = img_dimensions[1]
     im_y_max = img_dimensions[0]
 
-    '''
+    """
     Compute the bounding box
-    '''
+    """
     bb = set()
-    bb.update({(im_x_min, y) for y in range(im_y_min, im_y_max+1)})
+    bb.update({(im_x_min, y) for y in range(im_y_min, im_y_max + 1)})
     bb.update({(im_x_max, y) for y in range(im_y_min, im_y_max + 1)})
     bb.update({(x, im_y_min) for x in range(im_x_min, im_x_max + 1)})
     bb.update({(x, im_y_max) for x in range(im_x_min, im_x_max + 1)})
 
     return bb
 
+
 class EdgeData(NamedTuple):
     init_theta: float
     tangent: float
     opp_loc: Tuple[float, float]
     mid_loc: Tuple[float, float]
 
-'''
+
+"""
 Compute the dictionary with key is the start state and the values are a tuple
 consisting of the angle, mid point and the the opposite edge
-'''
+"""
 
-def compute_midpoints(img_data, bw_kernelsize=1, kernelsize=3, threshold=100,
-                      num_samples = lambda r:16):
+
+def compute_midpoints(
+    img_data, bw_kernelsize=1, kernelsize=3, threshold=100, num_samples=lambda r: 16
+):
     # First compute the black and white image and store it
     img_bw = convert_black_white(img_data=img_data)
-    img_bw = img_bw.convert('L')
+    img_bw = img_bw.convert("L")
     img_bw_int = np.array(img_bw, dtype=int)
 
     # Compute the point to the tangent angle dictionary
-    cae = compute_gradient_sobel(img_data=img_data,
-                                 bw_kernelsize=bw_kernelsize,
-                                 kernelsize=kernelsize,
-                                 threshold=threshold)
+    cae = compute_gradient_sobel(
+        img_data=img_data,
+        bw_kernelsize=bw_kernelsize,
+        kernelsize=kernelsize,
+        threshold=threshold,
+    )
 
     # Collect all edges
     all_edges = set(cae.keys())
 
     # Collect all roads
     connected_edges = generate_connected_edges(edge_locs=deepcopy(all_edges))
 
@@ -286,47 +286,18 @@
 
     all_edges.update(bb)
 
     # Compute midpoints
     point_data = {}
     for edge in connected_edges:
         for x in edge:
-            init_theta, theta, opp_loc, mid_loc = find_center(x=[x[1], x[0]],
-                                                    theta=cae[x],
-                                           collected_edges=connected_edges,
-                                           all_edges=all_edges,
-                                           num_samples=num_samples,
-                                           bw_image=img_bw_int)
-
-            point_data[x] = EdgeData(init_theta=float(init_theta), tangent=float(theta),
-                             opp_loc=opp_loc, mid_loc=mid_loc \
-                    if opp_loc not in bb else (np.nan, np.nan))
+            init_theta, theta, opp_loc, mid_loc = find_center(
+                x=[x[1], x[0]],
+                theta=cae[x],
+                collected_edges=connected_edges,
+                all_edges=all_edges,
+                num_samples=num_samples,
+                bw_image=img_bw_int,
+            )
 
+            point_data[x] = float(theta)
     return point_data
-
-'''
-Compute the heading at a random sample
-'''
-
-def compute_heading(x, point_data):
-    road_edges = tuple(point_data.keys())
-    edge_distance = np.linalg.norm(np.array(list(road_edges)) - np.array(x),1,
-                                   axis=1)
-    closest_edge = list(road_edges)[edge_distance.argmin()]
-
-    return closest_edge, point_data[closest_edge]
-
-'''
-Sampling from road
-'''
-
-def sample_from_road(img_data, num_samples):
-    img_bw = convert_black_white(img_data=img_data)
-    img_bw = img_bw.convert('L')
-    img_bw_int = np.array(img_bw, dtype=int)
-
-    road_y, road_x = np.where(img_bw_int == 0)
-    all_roads = list(zip(road_y, road_x))
-
-    locs = np.random.choice(len(all_roads), num_samples, replace=False)
-
-    return np.array(all_roads)[locs]
```

### Comparing `scenic-2.1.0b4/src/scenic/simulators/gta/interface.py` & `scenic-3.0.0b2/src/scenic/simulators/gta/interface.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,260 +1,286 @@
 """Python supporting code for the GTA model."""
 
 from dataclasses import dataclass
 import math
+import random
 import time
 
 import numpy
 import scipy.spatial
 
 try:
-	import PIL
+    import PIL
 except ModuleNotFoundError as e:
-	raise RuntimeError('GTA scenarios require the PIL module;'
-	                   ' try "pip install pillow"') from e
+    raise RuntimeError(
+        "GTA scenarios require the PIL module;" ' try "pip install pillow"'
+    ) from e
 
 try:
-	import cv2
+    import cv2
 except ModuleNotFoundError as e:
-	raise RuntimeError('GTA scenarios require the cv2 module;'
-	                   ' try "pip install opencv-python"') from e
-
+    raise RuntimeError(
+        "GTA scenarios require the cv2 module;" ' try "pip install opencv-python"'
+    ) from e
+
+from scenic.core.distributions import (
+    Distribution,
+    Normal,
+    Options,
+    Range,
+    Samplable,
+    distributionMethod,
+    toDistribution,
+)
+from scenic.core.geometry import *
+from scenic.core.lazy_eval import valueInContext
+from scenic.core.regions import GridRegion, PointSetRegion
+import scenic.core.utils as utils
+from scenic.core.vectors import VectorField
+from scenic.core.workspaces import Workspace
 import scenic.simulators.gta.center_detection as center_detection
 import scenic.simulators.gta.img_modf as img_modf
 import scenic.simulators.gta.messages as messages
 from scenic.simulators.utils.colors import Color
-
-from scenic.core.distributions import (Samplable, Distribution, Range, Normal, Options,
-                                       distributionMethod, toDistribution)
-from scenic.core.lazy_eval import valueInContext
-
-from scenic.core.workspaces import Workspace
-from scenic.core.vectors import VectorField
-from scenic.core.regions import PointSetRegion, GridRegion
-import scenic.core.utils as utils
-from scenic.core.geometry import *
-
 from scenic.syntax.veneer import verbosePrint
 
 ### Abstract GTA interface
 
+
 class GTA:
-	@staticmethod
-	def Config(scene):
-		ego = scene.egoObject
-		vehicles = [GTA.Vehicle(car) for car in scene.objects if car is not ego]
-		cameraLoc = GTA.langToGTACoords(ego.position)
-		cameraHeading = GTA.langToGTAHeading(ego.heading)
-
-		params = dict(scene.params)
-		time = int(round(params.pop('time')))
-		minute = time % 60
-		hour = int((time - minute) / 60)
-		assert hour < 24
-		weather = params.pop('weather')
-		for param in params:
-			print(f'WARNING: unused scene parameter "{param}"')
-
-		return messages.Formal_Config(cameraLoc, [hour, minute], weather,
-		                              vehicles, cameraHeading)
-
-	@staticmethod
-	def Vehicle(car):
-		loc3 = GTA.langToGTACoords(car.position)
-		heading = GTA.langToGTAHeading(car.heading)
-		scol = list(Color.realToByte(car.color))
-		return messages.Vehicle(car.model.name, scol, loc3, heading)
-	
-	@staticmethod
-	def langToGTACoords(point):
-		x, y = point
-		return [x, y, 60]
-
-	@staticmethod
-	def langToGTAHeading(heading):
-		h = math.degrees(heading)
-		return (h + 360) % 360
+    @staticmethod
+    def Config(scene):
+        ego = scene.egoObject
+        vehicles = [GTA.Vehicle(car) for car in scene.objects if car is not ego]
+        cameraLoc = GTA.langToGTACoords(ego.position)
+        cameraHeading = GTA.langToGTAHeading(ego.heading)
+
+        params = dict(scene.params)
+        time = int(round(params.pop("time")))
+        minute = time % 60
+        hour = int((time - minute) / 60)
+        assert hour < 24
+        weather = params.pop("weather")
+        for param in params:
+            print(f'WARNING: unused scene parameter "{param}"')
+
+        return messages.Formal_Config(
+            cameraLoc, [hour, minute], weather, vehicles, cameraHeading
+        )
+
+    @staticmethod
+    def Vehicle(car):
+        loc3 = GTA.langToGTACoords(car.position)
+        heading = GTA.langToGTAHeading(car.heading)
+        scol = list(Color.realToByte(car.color))
+        return messages.Vehicle(car.model.name, scol, loc3, heading)
+
+    @staticmethod
+    def langToGTACoords(point):
+        x, y, _ = point
+        return [x, y, 60]
+
+    @staticmethod
+    def langToGTAHeading(heading):
+        h = math.degrees(heading)
+        return (h + 360) % 360
+
 
 ### Map
 
+
 class Map:
-	"""Represents roads and obstacles in GTA, extracted from a map image.
+    """Represents roads and obstacles in GTA, extracted from a map image.
+
+    This code handles images from the `GTA V Interactive Map <https://gta-5-map.com/>`_,
+    rendered with the "Road" setting.
 
-	This code handles images from the `GTA V Interactive Map <https://gta-5-map.com/>`_,
-	rendered with the "Road" setting.
+    Args:
+        imagePath (str): path to image file
+        Ax (float): width of one pixel in GTA coordinates
+        Ay (float): height of one pixel in GTA coordinates
+        Bx (float): GTA X-coordinate of bottom-left corner of image
+        By (float): GTA Y-coordinate of bottom-left corner of image
+    """
+
+    def __init__(self, imagePath, Ax, Ay, Bx, By):
+        self.Ax, self.Ay = Ax, Ay
+        self.Bx, self.By = Bx, By
+        if imagePath != None:
+            startTime = time.time()
+            # open image
+            image = PIL.Image.open(imagePath)
+            self.sizeX, self.sizeY = image.size
+            # create version of image for display
+            de = img_modf.get_edges(image).convert("RGB")
+            self.displayImage = cv2.cvtColor(numpy.array(de), cv2.COLOR_RGB2BGR)
+            # detect edges of roads
+            ed = center_detection.compute_midpoints(img_data=image, kernelsize=5)
+            edges, tangents = [], []
+            for (y, x), tangent in ed.items():
+                edges.append(self.gridToScenicCoords((x, y)))
+                tangents.append(tangent)
+            self.edges = numpy.array(edges)
+            self.edgeTangents = numpy.array(tangents)
+            # build k-D tree
+            self.edgeTree = scipy.spatial.KDTree(self.edges)
+            # identify points on roads
+            self.roadArray = numpy.array(
+                img_modf.convert_black_white(img_data=image).convert("L"), dtype=int
+            )
+            totalTime = time.time() - startTime
+            verbosePrint(f"Created GTA map from image in {totalTime:.2f} seconds.")
+
+    @staticmethod
+    def fromFile(path):
+        startTime = time.time()
+        with numpy.load(path) as data:
+            Ax, Ay, Bx, By, sizeX, sizeY = data["misc"]
+            m = Map(None, Ax, Ay, Bx, By)
+            m.sizeX, m.sizeY = sizeX, sizeY
+            m.displayImage = data["displayImage"]
+
+            m.edges = data["edges"]
+            m.edgeTangents = data["tangents"]
+            m.edgeTree = scipy.spatial.KDTree(m.edges)  # rebuild k-D tree
+
+            m.roadArray = data["roadArray"]
+            totalTime = time.time() - startTime
+            verbosePrint(f"Loaded GTA map in {totalTime:.2f} seconds.")
+            return m
+
+    def dumpToFile(self, path):
+        misc = numpy.array((self.Ax, self.Ay, self.Bx, self.By, self.sizeX, self.sizeY))
+
+        numpy.savez_compressed(
+            path,
+            misc=misc,
+            displayImage=self.displayImage,
+            edges=self.edges,
+            tangents=self.edgeTangents,
+            roadArray=self.roadArray,
+        )
+
+    @property
+    @utils.cached
+    def roadDirection(self):
+        return VectorField("roadDirection", self.roadHeadingAt)
+
+    @property
+    @utils.cached
+    def roadRegion(self):
+        return GridRegion(
+            "road",
+            self.roadArray,
+            self.Ax,
+            self.Ay,
+            self.Bx,
+            self.By,
+            orientation=self.roadDirection,
+        )
+
+    @property
+    @utils.cached
+    def curbRegion(self):
+        return PointSetRegion("curb", self.edges, orientation=self.roadDirection)
+
+    def gridToScenicCoords(self, point):
+        x, y = point[0], point[1]
+        return ((self.Ax * x) + self.Bx, (self.Ay * y) + self.By)
+
+    def gridToScenicHeading(self, heading):
+        return heading - (math.pi / 2)
+
+    def scenicToGridCoords(self, point):
+        x, y = point[0], point[1]
+        return ((x - self.Bx) / self.Ax, (y - self.By) / self.Ay)
+
+    def scenicToGridHeading(self, heading):
+        return heading + (math.pi / 2)
+
+    @distributionMethod
+    def roadHeadingAt(self, point):
+        # find closest edge
+        point2d = (point[0], point[1])
+        distance, location = self.edgeTree.query(point2d)
+        # get direction of edge
+        return self.gridToScenicHeading(self.edgeTangents[location])
 
-	Args:
-		imagePath (str): path to image file
-		Ax (float): width of one pixel in GTA coordinates
-		Ay (float): height of one pixel in GTA coordinates
-		Bx (float): GTA X-coordinate of bottom-left corner of image
-		By (float): GTA Y-coordinate of bottom-left corner of image
-	"""
-	def __init__(self, imagePath, Ax, Ay, Bx, By):
-		self.Ax, self.Ay = Ax, Ay
-		self.Bx, self.By = Bx, By
-		if imagePath != None:
-			startTime = time.time()
-			# open image
-			image = PIL.Image.open(imagePath)
-			self.sizeX, self.sizeY = image.size
-			# create version of image for display
-			de = img_modf.get_edges(image).convert('RGB')
-			self.displayImage = cv2.cvtColor(numpy.array(de), cv2.COLOR_RGB2BGR)
-			# detect edges of roads
-			ed = center_detection.compute_midpoints(img_data=image, kernelsize=5)
-			self.edgeData = {
-				self.gridToScenicCoords((x, y)): datum
-				for (y, x), datum in ed.items()
-			}
-			self.orderedCurbPoints = list(self.edgeData.keys())
-			# build k-D tree
-			self.edgeTree = scipy.spatial.cKDTree(self.orderedCurbPoints)
-			# identify points on roads
-			self.roadArray = numpy.array(img_modf.convert_black_white(img_data=image).convert('L'),
-			                             dtype=int)
-			totalTime = time.time() - startTime
-			verbosePrint(f'Created GTA map from image in {totalTime:.2f} seconds.')
-
-	@staticmethod
-	def fromFile(path):
-		startTime = time.time()
-		with numpy.load(path, allow_pickle=True) as data:
-			Ax, Ay, Bx, By, sizeX, sizeY = data['misc']
-			m = Map(None, Ax, Ay, Bx, By)
-			m.sizeX, m.sizeY = sizeX, sizeY
-			m.displayImage = data['displayImage']
-			
-			m.edgeData = { tuple(e): center_detection.EdgeData(*rest) for e, *rest in data['edges'] }
-			m.orderedCurbPoints = list(m.edgeData.keys())
-			m.edgeTree = scipy.spatial.cKDTree(m.orderedCurbPoints)		# rebuild k-D tree
-
-			m.roadArray = data['roadArray']
-			totalTime = time.time() - startTime
-			verbosePrint(f'Loaded GTA map in {totalTime:.2f} seconds.')
-			return m
-
-	def dumpToFile(self, path):
-		misc = numpy.array((self.Ax, self.Ay, self.Bx, self.By, self.sizeX, self.sizeY))
-		edges = numpy.array([(edge,) + tuple(datum) for edge, datum in self.edgeData.items()])
-		roadArray = self.roadArray
-
-		numpy.savez_compressed(path,
-			misc=misc, displayImage=self.displayImage,
-			edges=edges, roadArray=self.roadArray)
-
-	@property
-	@utils.cached
-	def roadDirection(self):
-		return VectorField('roadDirection', self.roadHeadingAt)
-	
-	@property
-	@utils.cached
-	def roadRegion(self):
-		return GridRegion('road', self.roadArray,
-		                  self.Ax, self.Ay, self.Bx, self.By,
-		                  orientation=self.roadDirection)
-
-	@property
-	@utils.cached
-	def curbRegion(self):
-		return PointSetRegion('curb', self.orderedCurbPoints,
-		                      kdTree=self.edgeTree,
-		                      orientation=self.roadDirection)
-
-	def gridToScenicCoords(self, point):
-		x, y = point[0], point[1]
-		return ((self.Ax * x) + self.Bx, (self.Ay * y) + self.By)
-
-	def gridToScenicHeading(self, heading):
-		return heading - (math.pi / 2)
-
-	def scenicToGridCoords(self, point):
-		x, y = point[0], point[1]
-		return ((x - self.Bx) / self.Ax, (y - self.By) / self.Ay)
-
-	def scenicToGridHeading(self, heading):
-		return heading + (math.pi / 2)
-
-	@distributionMethod
-	def roadHeadingAt(self, point):
-		# find closest edge
-		distance, location = self.edgeTree.query(point)
-		closest = tuple(self.edgeTree.data[location])
-		# get direction of edge
-		return self.gridToScenicHeading(self.edgeData[closest].tangent)
+    def show(self, plt):
+        plt.imshow(self.displayImage)
 
-	def show(self, plt):
-		plt.imshow(self.displayImage)
 
 class MapWorkspace(Workspace):
-	"""Workspace whose rendering is handled by a Map"""
-	def __init__(self, mappy, region):
-		super().__init__(region)
-		self.map = mappy
-
-	def scenicToSchematicCoords(self, coords):
-		return self.map.scenicToGridCoords(coords)
-
-	def show(self, plt):
-		return self.map.show(plt)
-
-	@property
-	def minimumZoomSize(self):
-		return 40 / min(abs(self.map.Ax), abs(self.map.Ay))
+    """Workspace whose rendering is handled by a Map"""
+
+    def __init__(self, mappy, region):
+        super().__init__(region)
+        self.map = mappy
+
+    def scenicToSchematicCoords(self, coords):
+        return self.map.scenicToGridCoords(coords)
+
+    def show2D(self, plt):
+        return self.map.show(plt)
+
+    @property
+    def minimumZoomSize(self):
+        return 40 / min(abs(self.map.Ax), abs(self.map.Ay))
+
 
 ### Car models and colors
 
+
 @dataclass(frozen=True)
 class CarModel:
-	"""A model of car in GTA.
+    """A model of car in GTA.
+
+    Attributes:
+        name (str): name of model in GTA
+        width (float): width of this model of car
+        length (float): length of this model of car
+        viewAngle (float): view angle in radians (default is 90 degrees)
+
+    Class Attributes:
+        models: dict mapping model names to the corresponding `CarModel`
+    """
+
+    name: str
+    width: float
+    length: float
+    viewAngle: float = math.radians(90)
+
+    @classmethod
+    def uniformModel(self):
+        return Options(self.modelProbs.keys())
+
+    @classmethod
+    def egoModel(self):
+        return self.models["BLISTA"]
+
+    @classmethod
+    def defaultModel(self):
+        return Options(self.modelProbs)
 
-	Attributes:
-		name (str): name of model in GTA
-		width (float): width of this model of car
-		length (float): length of this model of car
-		viewAngle (float): view angle in radians (default is 90 degrees)
-
-	Class Attributes:
-		models: dict mapping model names to the corresponding `CarModel`
-	"""
-
-	name: str
-	width: float
-	length: float
-	viewAngle: float = math.radians(90)
-
-	@classmethod
-	def uniformModel(self):
-		return Options(self.modelProbs.keys())
-
-	@classmethod
-	def egoModel(self):
-		return self.models['BLISTA']
-
-	@classmethod
-	def defaultModel(self):
-		return Options(self.modelProbs)
+    def __str__(self):
+        return f"<CarModel {self.name}>"
 
-	def __str__(self):
-		return f'<CarModel {self.name}>'
 
 CarModel.modelProbs = {
-	CarModel('BLISTA', 1.75871, 4.10139): 1,
-	CarModel('BUS', 2.9007, 13.202): 0,
-	CarModel('NINEF', 2.07699, 4.50658): 1,
-	CarModel('ASEA', 1.83066, 4.45861): 1,
-	CarModel('BALLER', 2.10791, 5.10333): 1,
-	CarModel('BISON', 2.29372, 5.4827): 1,
-	CarModel('BUFFALO', 2.04265, 5.07782): 1,
-	CarModel('BOBCATXL', 2.37944, 5.78222): 1,
-	CarModel('DOMINATOR', 1.9353, 4.9355): 1,
-	CarModel('GRANGER', 3.02698, 5.94577): 1,
-	CarModel('JACKAL', 2.00041, 4.91436): 1,
-	CarModel('ORACLE', 2.07787, 5.12544): 1,
-	CarModel('PATRIOT', 2.26679, 5.13695): 1,
-	CarModel('PRANGER', 3.02698, 5.94577): 1
+    CarModel("BLISTA", 1.75871, 4.10139): 1,
+    CarModel("BUS", 2.9007, 13.202): 0,
+    CarModel("NINEF", 2.07699, 4.50658): 1,
+    CarModel("ASEA", 1.83066, 4.45861): 1,
+    CarModel("BALLER", 2.10791, 5.10333): 1,
+    CarModel("BISON", 2.29372, 5.4827): 1,
+    CarModel("BUFFALO", 2.04265, 5.07782): 1,
+    CarModel("BOBCATXL", 2.37944, 5.78222): 1,
+    CarModel("DOMINATOR", 1.9353, 4.9355): 1,
+    CarModel("GRANGER", 3.02698, 5.94577): 1,
+    CarModel("JACKAL", 2.00041, 4.91436): 1,
+    CarModel("ORACLE", 2.07787, 5.12544): 1,
+    CarModel("PATRIOT", 2.26679, 5.13695): 1,
+    CarModel("PRANGER", 3.02698, 5.94577): 1,
 }
-CarModel.models = { model.name: model for model in CarModel.modelProbs }
+CarModel.models = {model.name: model for model in CarModel.modelProbs}
 
-CarColor = Color 	# for backwards compatibility
+CarColor = Color  # for backwards compatibility
```

### Comparing `scenic-2.1.0b4/src/scenic/simulators/gta/model.scenic` & `scenic-3.0.0b2/src/scenic/simulators/gta/model.scenic`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """World model for GTA."""
 
 import random
 
 from scenic.simulators.gta.interface import (Map, MapWorkspace, GTA,
 	CarModel)
 from scenic.simulators.utils.colors import Color, ColorMutator
+CarColor = Color	# alias for backwards compatibility
 
 # Load map and set up regions, etc.
 from scenic.simulators.gta.map import mapPath
 if mapPath is None:
 	raise RuntimeError('need to select GTA map for this scenario')
 m = Map.fromFile(mapPath)
 
@@ -51,15 +52,15 @@
 		heading: The default heading is aligned with `roadDirection`, plus an offset
 		  given by ``roadDeviation``.
 		roadDeviation (float): Relative heading with respect to the road direction
 		  at the `Car`'s position. Used by the default value for ``heading``.
 		model (`CarModel`): Model of the car.
 		color (:obj:`Color` or RGB tuple): Color of the car.
 	"""
-	position: Point on road
+	position: new Point on road
 	heading: (roadDirection at self.position) + self.roadDeviation
 	roadDeviation: 0
 	width: self.model.width
 	length: self.model.length
 	viewAngle: 80 deg
 	visibleDistance: 30
 	model: CarModel.defaultModel()
@@ -82,11 +83,11 @@
 def createPlatoonAt(car, numCars, model=None, dist=Range(2, 8),
                     shift=Range(-0.5, 0.5), wiggle=0):
 	"""Create a platoon starting from the given car."""
 	cars = [car]
 	lastCar = car
 	for i in range(numCars-1):
 		center = follow roadDirection from (front of lastCar) for resample(dist)
-		pos = OrientedPoint right of center by shift, facing resample(wiggle) relative to roadDirection
-		lastCar = Car ahead of pos, with model (car.model if model is None else resample(model))
+		pos = new OrientedPoint right of center by shift, facing resample(wiggle) relative to roadDirection
+		lastCar = new Car ahead of pos, with model (car.model if model is None else resample(model))
 		cars.append(lastCar)
 	return cars
```

### Comparing `scenic-2.1.0b4/src/scenic/simulators/lgsvl/__init__.py` & `scenic-3.0.0b2/src/scenic/simulators/lgsvl/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 """Interface to the LGSVL driving simulator.
 
 This interface has been tested with `LGSVL <https://www.lgsvlsimulator.com/>`_ version
 2020.06. It supports dynamic scenarios involving vehicles and pedestrians.
 
 The interface implements the :obj:`scenic.domains.driving` abstract domain, so any
 object types, behaviors, utility functions, etc. from that domain may be used freely.
-
-.. raw:: html
-
-   <h2>Submodules</h2>
-
-.. autosummary::
-   :toctree:
-
-   model
-   actions
-   behaviors
-   simulator
-   utils
 """
 
 # Only import LGSVLSimulator if the lgsvl package is installed; otherwise the
 # import would raise an exception.
 lgsvl = None
 try:
-   import lgsvl
+    import lgsvl
 except ImportError:
-   pass
+    pass
 if lgsvl:
-   from .simulator import LGSVLSimulator
+    from .simulator import LGSVLSimulator
 del lgsvl
```

### Comparing `scenic-2.1.0b4/src/scenic/simulators/lgsvl/behaviors.scenic` & `scenic-3.0.0b2/src/scenic/simulators/lgsvl/behaviors.scenic`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Behaviors for dynamic agents in LGSVL."""
 
-from scenic.domains.driving.behaviors import *	# use all common driving behaviors
+from scenic.domains.driving.behaviors import *  # use all common driving behaviors
 
 try:
     from scenic.simulators.lgsvl.actions import *
 except ModuleNotFoundError:
     pass    # ignore; error will be caught later if user attempts to run a simulation
 
 behavior DriveTo(target):
-	action = SetDestinationAction(target)
-	while True:
-		take action
+    action = SetDestinationAction(target)
+    while True:
+        take action
 
 behavior WalkBehavior(maxSpeed=1.4):
-	take SetWalkAction(True, maxSpeed)
+    take SetWalkAction(True, maxSpeed)
 
 behavior FollowWaypoints(waypoints):
-	action = FollowWaypointsAction(waypoints)
-	while True:
-		take action
+    action = FollowWaypointsAction(waypoints)
+    while True:
+        take action
```

### Comparing `scenic-2.1.0b4/src/scenic/simulators/lgsvl/model.scenic` & `scenic-3.0.0b2/src/scenic/simulators/lgsvl/model.scenic`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 except ModuleNotFoundError:
     # to allow generating static scenes without having the lgsvl package installed
     EGO_TYPE = 'EGO'
     NPC_TYPE = 'NPC'
     PEDESTRIAN_TYPE = 'PEDESTRIAN'
     LINCOLN_MODULAR = 'Lincoln2017MKZ'
 
+    from scenic.core.simulators import SimulatorInterfaceWarning
     import warnings
     warnings.warn('the "lgsvl" package is not installed; '
-                  'will not be able to run dynamic simulations')
+                  'will not be able to run dynamic simulations',
+                  SimulatorInterfaceWarning)
 
     def LGSVLSimulator(*args, **kwargs):
         raise RuntimeError('the "lgsvl" package is required to run simulations '
                            'from this scenario')
 
 if 'lgsvl_map' not in globalParameters:
     raise RuntimeError('need to specify map before importing LGSVL model '
@@ -100,15 +102,15 @@
         'Transform',
         'Routing',
         'Prediction',
         'Planning',
         'Camera',
         'Traffic Light',
         'Control'
-	]
+    ]
     bridgeHost: 'localhost'
     bridgePort: 9090
 
     dreamview: None     # connection to Dreamview (set at runtime)
 
 class NPCCar(NPCCar, Vehicle):
     lgsvlName: 'Sedan'
```

### Comparing `scenic-2.1.0b4/src/scenic/simulators/lgsvl/simulator.py` & `scenic-3.0.0b2/src/scenic/simulators/lgsvl/simulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,71 +1,79 @@
 """Dynamic simulator interface for LGSVL."""
 
 import math
+import time
 import warnings
 
 import lgsvl
-import time
 
 import scenic.core.simulators as simulators
+from scenic.core.vectors import Vector
 import scenic.simulators.lgsvl.utils as utils
 from scenic.syntax.veneer import verbosePrint
-from scenic.core.vectors import Vector
+
 
 class LGSVLSimulator(simulators.Simulator):
     """A connection to an instance of LGSVL.
 
     See the `SVL documentation`_ for details on how to set the parameters below.
 
+    Uses a default timestep of 0.1 seconds.
+
     Args:
         sceneID (str): Identifier for the map ("scene") to load in SVL.
         address (str): Address where SVL is running.
         port (int): Port on which to connect to SVL.
         alwaysReload (bool): Whether to force reloading the map upon connecting,
             even if the simulator already has the desired map loaded.
 
     .. _SVL documentation: https://www.svlsimulator.com/docs/python-api/python-api
     """
-    def __init__(self, sceneID, address='localhost', port=8181, alwaysReload=False):
+
+    def __init__(self, sceneID, address="localhost", port=8181, alwaysReload=False):
         super().__init__()
-        verbosePrint('Connecting to LGSVL Simulator...')
+        verbosePrint("Connecting to LGSVL Simulator...")
         self.client = lgsvl.Simulator(address=address, port=port)
-        if alwaysReload or self.client.current_scene != lgsvl_scene:
+        if alwaysReload or self.client.current_scene != sceneID:
             self.client.load(scene=sceneID)
-        verbosePrint('Map loaded in simulator.')
+        verbosePrint("Map loaded in simulator.")
 
-    def createSimulation(self, scene, verbosity=0):
-        return LGSVLSimulation(scene, self.client, verbosity=verbosity)
+    def createSimulation(self, scene, **kwargs):
+        return LGSVLSimulation(scene, self.client, **kwargs)
 
 
 class LGSVLSimulation(simulators.Simulation):
     """Subclass of `Simulation` for LGSVL."""
-    def __init__(self, scene, client, verbosity=0):
-        timestep = scene.params.get('time_step', 1.0/10)
-        super().__init__(scene, timestep=timestep, verbosity=verbosity)
+
+    def __init__(self, scene, client, *, timestep, **kwargs):
         self.client = client
         self.usingApollo = False
         self.data = {}
         self.collisionOccurred = False
 
+        if timestep is None:
+            timestep = scene.params.get("time_step", 0.1)  # backwards-compatibility
+
+        super().__init__(scene, timestep=timestep, **kwargs)
+
+    def setup(self):
         # Reset simulator (deletes all existing objects)
         self.client.reset()
 
-        # Create LGSVL objects corresponding to Scenic objects
-        for obj in self.objects:
-            if not hasattr(obj, 'lgsvlObject'):
-                continue    # not an LGSVL object
-            self.createObjectInSimulator(obj)
+        super().setup()
 
     def createObjectInSimulator(self, obj):
+        if not hasattr(obj, "lgsvlObject"):
+            return  # not an LGSVL object
+
         # Figure out what type of LGSVL object this is
-        if not hasattr(obj, 'lgsvlName'):
-            raise RuntimeError(f'object {obj} does not have an lgsvlName property')
-        if not hasattr(obj, 'lgsvlAgentType'):
-            raise RuntimeError(f'object {obj} does not have an lgsvlAgentType property')
+        if not hasattr(obj, "lgsvlName"):
+            raise RuntimeError(f"object {obj} does not have an lgsvlName property")
+        if not hasattr(obj, "lgsvlAgentType"):
+            raise RuntimeError(f"object {obj} does not have an lgsvlAgentType property")
         name = obj.lgsvlName
         agentType = obj.lgsvlAgentType
 
         # Set up position and orientation
         state = lgsvl.AgentState()
         elevation = obj.elevation
         if elevation is None:
@@ -76,83 +84,89 @@
         # Create LGSVL object
         lgsvlObj = self.client.add_agent(name, agentType, state)
         obj.lgsvlObject = lgsvlObj
 
         # Initialize Data
         self.data[obj] = {}
         # Initialize Apollo if needed
-        if getattr(obj, 'apolloVehicle', None):
+        if getattr(obj, "apolloVehicle", None):
             self.initApolloFor(obj, lgsvlObj)
 
     def groundElevationAt(self, pos):
         origin = utils.scenicToLGSVLPosition(pos, 100000)
         result = self.client.raycast(origin, lgsvl.Vector(0, -1, 0), 1)
         if result is None:
-            warnings.warn(f'no ground at position {pos}')
+            warnings.warn(
+                f"no ground at position {pos}", simulators.SimulatorInterfaceWarning
+            )
             return 0
         return result.point.y
 
     def initApolloFor(self, obj, lgsvlObj):
         """Initialize Apollo for an ego vehicle.
 
         Uses LG's interface which injects packets into Dreamview.
         """
         if self.usingApollo:
-            raise RuntimeError('can only use one Apollo vehicle')
+            raise RuntimeError("can only use one Apollo vehicle")
         self.usingApollo = True
 
         def on_collision(agent1, agent2, contact):
             if agent1 is not None and agent1.name == lgsvlObj.name:
-                self.data[obj]['collision'] = True
+                self.data[obj]["collision"] = True
             if agent2 is not None and agent2.name == lgsvlObj.name:
-                self.data[obj]['collision'] = True
-            if self.data[obj]['collision']:
+                self.data[obj]["collision"] = True
+            if self.data[obj]["collision"]:
                 self.collisionOccurred = True
 
         # Initialize Data
-        self.data[obj]['collision'] = False
+        self.data[obj]["collision"] = False
         lgsvlObj.on_collision(on_collision)
 
         # connect bridge from LGSVL to Apollo
         lgsvlObj.connect_bridge(obj.bridgeHost, obj.bridgePort)
 
         # set up connection and map/vehicle configuration
         from lgsvl import dreamview
+
         dv = dreamview.Connection(self.client, lgsvlObj)
         obj.dreamview = dv
-        hdMap = self.scene.params['apolloHDMap']
+        hdMap = self.scene.params["apolloHDMap"]
         dv.set_hd_map(hdMap)
         dv.set_vehicle(obj.apolloVehicle)
 
     def executeActions(self, allActions):
         super().executeActions(allActions)
 
         # Apply state/control updates which were accumulated while executing the actions
         for obj in self.agents:
             if obj._stateUpdated:
                 obj.lgsvlObject.state = obj.state
                 obj._stateUpdated = False
-            ctrl = getattr(obj, '_control', None)
+            ctrl = getattr(obj, "_control", None)
             if ctrl is not None:
                 obj.lgsvlObject.apply_control(ctrl, obj._stickyControl)
                 obj._control = None
 
     def step(self):
         self.client.run(time_limit=self.timestep)
 
     def getProperties(self, obj, properties):
         lgsvlObj = obj.lgsvlObject
         state = lgsvlObj.state
-        obj.state = state   # cache state for subsequent updates
+        obj.state = state  # cache state for subsequent updates
 
         velocity = utils.lgsvlToScenicPosition(state.velocity)
         speed = math.hypot(*velocity)
 
         values = dict(
             position=utils.lgsvlToScenicPosition(state.position),
             elevation=utils.lgsvlToScenicElevation(state.position),
             heading=utils.lgsvlToScenicRotation(state.rotation),
             velocity=velocity,
             speed=speed,
             angularSpeed=utils.lgsvlToScenicAngularSpeed(state.rotation),
         )
         return values
+
+    def destroy(self):
+        self.client.reset()
```

### Comparing `scenic-2.1.0b4/src/scenic/simulators/lgsvl/utils.py` & `scenic-3.0.0b2/src/scenic/simulators/lgsvl/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,45 @@
-
 """Common LGSVL interface."""
 
 import math
 
 import lgsvl
 
-from scenic.core.vectors import Vector
 from scenic.core.geometry import normalizeAngle
+from scenic.core.vectors import Vector
+
 
 def lgsvlToScenicPosition(pos):
     """Convert LGSVL positions to Scenic positions."""
     return Vector(pos.x, pos.z)
 
+
 def gpsToScenicPosition(northing, easting):
     """Convert GPS positions to Scenic positions."""
     pos = lgsvl.map_from_gps(northing, easting)
     return Vector(pos.x, pos.z)
 
+
 def lgsvlToScenicElevation(pos):
     """Convert LGSVL positions to Scenic elevations."""
     return pos.y
 
+
 def scenicToLGSVLPosition(pos, y=0):
     x, z = pos
     return lgsvl.Vector(x, y, z)
 
+
 def lgsvlToScenicRotation(rot):
     """Convert LGSVL rotations to Scenic headings.
 
     Drops all but the Y component.
     """
     return normalizeAngle(-math.radians(rot.y))
 
+
 def lgsvlToScenicAngularSpeed(rot):
     return -math.radians(rot.y)
 
+
 def scenicToLGSVLRotation(heading):
     return lgsvl.Vector(0, -math.degrees(heading), 0)
```

### Comparing `scenic-2.1.0b4/src/scenic/simulators/newtonian/car.png` & `scenic-3.0.0b2/src/scenic/simulators/newtonian/car.png`

 * *Files identical despite different names*

### Comparing `scenic-2.1.0b4/src/scenic/simulators/newtonian/driving_model.scenic` & `scenic-3.0.0b2/src/scenic/simulators/newtonian/driving_model.scenic`

 * *Files 4% similar despite different names*

```diff
@@ -52,11 +52,14 @@
     pass
 
 class Car(Vehicle, Steers):
     @property
     def isCar(self):
         return True
 
+class Pedestrian(Pedestrian, NewtonianActor, Walks):
+    pass
+
 class Debris:
-	"""Abstract class for debris scattered randomly in the workspace."""
-	position: Point in workspace
-	heading: Range(0, 360) deg
+    """Abstract class for debris scattered randomly in the workspace."""
+    position: Point in workspace
+    yaw: Range(0, 360) deg
```

### Comparing `scenic-2.1.0b4/src/scenic/simulators/newtonian/simulator.py` & `scenic-3.0.0b2/src/scenic/simulators/newtonian/simulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,106 +1,118 @@
 """Newtonian simulator implementation."""
 
 from cmath import atan, pi, tan
 import math
-from math import sin, radians, degrees, copysign
+from math import copysign, degrees, radians, sin
 import os
 import pathlib
 import time
 
-from scenic.domains.driving.simulators import DrivingSimulator, DrivingSimulation
-from scenic.core.geometry import allChains
+import scenic.core.errors as errors  # isort: skip
+
+if errors.verbosityLevel == 0:  # suppress pygame advertisement at zero verbosity
+    os.environ["PYGAME_HIDE_SUPPORT_PROMPT"] = "hide"
+import pygame
+import shapely
+
+from scenic.core.geometry import allChains, findMinMax
 from scenic.core.regions import toPolygon
 from scenic.core.simulators import SimulationCreationError
-from scenic.syntax.veneer import verbosePrint
-from scenic.core.vectors import Vector
-import scenic.simulators.newtonian.utils.utils as utils
-from scenic.domains.driving.controllers import PIDLongitudinalController, PIDLateralController
+from scenic.core.vectors import Orientation, Vector
+from scenic.domains.driving.controllers import (
+    PIDLateralController,
+    PIDLongitudinalController,
+)
 from scenic.domains.driving.roads import Network
-from scenic.syntax.translator import verbosity
-
-import shapely
-if verbosity == 0:  # suppress pygame advertisement at zero verbosity
-    os.environ['PYGAME_HIDE_SUPPORT_PROMPT'] = 'hide'
-import pygame
+from scenic.domains.driving.simulators import DrivingSimulation, DrivingSimulator
+from scenic.syntax.veneer import verbosePrint
 
 current_dir = pathlib.Path(__file__).parent.absolute()
 
 WIDTH = 1280
 HEIGHT = 800
-MAX_ACCELERATION = 5.6 # in m/s2, seems to be a pretty reasonable value
+MAX_ACCELERATION = 5.6  # in m/s2, seems to be a pretty reasonable value
 MAX_BRAKING = 4.6
 
 ROAD_COLOR = (0, 0, 0)
 ROAD_WIDTH = 2
 LANE_COLOR = (96, 96, 96)
 CENTERLINE_COLOR = (224, 224, 224)
 SIDEWALK_COLOR = (0, 128, 255)
 SHOULDER_COLOR = (96, 96, 96)
 
+
 class NewtonianSimulator(DrivingSimulator):
     """Implementation of `Simulator` for the Newtonian simulator.
 
     Args:
         network (Network): road network to display in the background, if any.
-        timestep (float): time step to use.
         render (bool): whether to render the simulation in a window.
+
+    .. versionchanged:: 3.0
+
+        The **timestep** argument is removed: it can be specified when calling
+        `simulate` instead. The default timestep for the Newtonian simulator
+        when not otherwise specified is still 0.1 seconds.
     """
-    def __init__(self, network=None, timestep=0.1, render=False):
-        self.timestep = timestep
+
+    def __init__(self, network=None, render=False):
+        super().__init__()
         self.render = render
         self.network = network
 
-    def createSimulation(self, scene, verbosity=0):
-        return NewtonianSimulation(scene, self.network, timestep=self.timestep,
-                                   verbosity=verbosity, render=self.render)
+    def createSimulation(self, scene, **kwargs):
+        return NewtonianSimulation(scene, self.network, self.render, **kwargs)
+
 
 class NewtonianSimulation(DrivingSimulation):
-    def __init__(self, scene, network, timestep, verbosity=0, render=False):
-        super().__init__(scene, timestep=timestep, verbosity=verbosity)
+    """Implementation of `Simulation` for the Newtonian simulator."""
+
+    def __init__(self, scene, network, render, timestep, **kwargs):
         self.render = render
         self.network = network
-        self.ego = self.objects[0]
 
-        # Set actor's initial speed
-        for obj in self.objects:
-            obj.speed = math.hypot(*obj.velocity)
+        if timestep is None:
+            timestep = 0.1
+
+        super().__init__(scene, timestep=timestep, **kwargs)
+
+    def setup(self):
+        super().setup()
 
         if self.render:
             # determine window size
-            min_x, min_y = self.ego.position
-            max_x, max_y = self.ego.position
-            for obj in self.objects:
-                x, y = obj.position
-                min_x, max_x = min(min_x, x), max(max_x, x)
-                min_y, max_y = min(min_y, y), max(max_y, y)
+            min_x, max_x = findMinMax(obj.x for obj in self.objects)
+            min_y, max_y = findMinMax(obj.y for obj in self.objects)
 
             pygame.init()
             pygame.font.init()
-            self.screen = pygame.display.set_mode((WIDTH,HEIGHT),
-                                                  pygame.HWSURFACE | pygame.DOUBLEBUF)
+            self.screen = pygame.display.set_mode(
+                (WIDTH, HEIGHT), pygame.HWSURFACE | pygame.DOUBLEBUF
+            )
             self.screen.fill((255, 255, 255))
-            x, y = self.ego.position
-            self.min_x, self.max_x = min_x-50, max_x+50
-            self.min_y, self.max_y = min_y-50, max_y+50
+            x, y, _ = self.objects[0].position
+            self.min_x, self.max_x = min_x - 50, max_x + 50
+            self.min_y, self.max_y = min_y - 50, max_y + 50
             self.size_x = self.max_x - self.min_x
             self.size_y = self.max_y - self.min_y
-            self.screen_poly = shapely.geometry.Polygon((
-                (self.min_x, self.min_y),
-                (self.max_x, self.min_y),
-                (self.max_x, self.max_y),
-                (self.min_x, self.max_y)
-            ))
+            self.screen_poly = shapely.geometry.Polygon(
+                (
+                    (self.min_x, self.min_y),
+                    (self.max_x, self.min_y),
+                    (self.max_x, self.max_y),
+                    (self.min_x, self.max_y),
+                )
+            )
 
-            img_path = os.path.join(current_dir, 'car.png')
+            img_path = os.path.join(current_dir, "car.png")
             self.car = pygame.image.load(img_path)
             self.car_width = int(3.5 * WIDTH / self.size_x)
             self.car_height = self.car_width
-            self.car = pygame.transform.scale(self.car, (self.car_width,
-                                                         self.car_height))
+            self.car = pygame.transform.scale(self.car, (self.car_width, self.car_height))
             self.parse_network()
             self.draw_objects()
 
     def parse_network(self):
         self.network_polygons = []
         if not self.network:
             return
@@ -111,43 +123,44 @@
                 return
             for chain in allChains(poly):
                 coords = tuple(self.scenicToScreenVal(pt) for pt in chain.coords)
                 self.network_polygons.append((coords, color, width))
 
         addRegion(self.network.walkableRegion, SIDEWALK_COLOR)
         addRegion(self.network.shoulderRegion, SHOULDER_COLOR)
-        for road in self.network.roads: # loop over main roads
+        for road in self.network.roads:  # loop over main roads
             for lane in road.lanes:
                 addRegion(lane.leftEdge, LANE_COLOR)
                 addRegion(lane.rightEdge, LANE_COLOR)
             addRegion(road, ROAD_COLOR, ROAD_WIDTH)
-        for lane in self.network.lanes: # loop over all lanes, even in intersections
+        for lane in self.network.lanes:  # loop over all lanes, even in intersections
             addRegion(lane.centerline, CENTERLINE_COLOR)
         addRegion(self.network.intersectionRegion, ROAD_COLOR)
 
     def scenicToScreenVal(self, pos):
-        x, y = pos
+        x, y = pos[:2]
         x_prop = (x - self.min_x) / self.size_x
         y_prop = (y - self.min_y) / self.size_y
         return int(x_prop * WIDTH), HEIGHT - 1 - int(y_prop * HEIGHT)
 
     def createObjectInSimulator(self, obj):
-        pass
+        # Set actor's initial speed
+        obj.speed = math.hypot(*obj.velocity)
 
-    def actionsAreCompatible(self, agent, actions):
-        return True
+        if hasattr(obj, "elevation"):
+            obj.elevation = 0.0
 
     def isOnScreen(self, x, y):
         return self.min_x <= x <= self.max_x and self.min_y <= y <= self.max_y
 
     def step(self):
         for obj in self.objects:
             current_speed = obj.velocity.norm()
-            if hasattr(obj, 'hand_brake'):
-                forward = (obj.velocity.dot(Vector(0, 1).rotatedBy(obj.heading)) >= 0)
+            if hasattr(obj, "hand_brake"):
+                forward = obj.velocity.dot(Vector(0, 1).rotatedBy(obj.heading)) >= 0
                 signed_speed = current_speed if forward else -current_speed
                 if obj.hand_brake or obj.brake > 0:
                     braking = MAX_BRAKING * max(obj.hand_brake, obj.brake)
                     acceleration = braking * self.timestep
                     if acceleration >= current_speed:
                         signed_speed = 0
                     elif forward:
@@ -167,75 +180,94 @@
                 else:
                     obj.angularSpeed = 0
                 obj.speed = abs(signed_speed)
             else:
                 obj.speed = current_speed
             obj.position += obj.velocity * self.timestep
             obj.heading += obj.angularSpeed * self.timestep
+
         if self.render:
             self.draw_objects()
+            pygame.event.pump()
 
     def draw_objects(self):
         self.screen.fill((255, 255, 255))
         for screenPoints, color, width in self.network_polygons:
             pygame.draw.lines(self.screen, color, False, screenPoints, width=width)
 
-        for obj in self.objects:
-            color = (255, 0, 0) if obj is self.ego else (0, 0, 255)
+        for i, obj in enumerate(self.objects):
+            color = (255, 0, 0) if i == 0 else (0, 0, 255)
             h, w = obj.length, obj.width
             pos_vec = Vector(-1.75, 1.75)
             neg_vec = Vector(w / 2, h / 2)
             heading_vec = Vector(0, 10).rotatedBy(obj.heading)
             dx, dy = int(heading_vec.x), -int(heading_vec.y)
             x, y = self.scenicToScreenVal(obj.position)
             rect_x, rect_y = self.scenicToScreenVal(obj.position + pos_vec)
-            if hasattr(obj, 'isCar') and obj.isCar:
-                self.rotated_car = pygame.transform.rotate(self.car, math.degrees(obj.heading))
+            if hasattr(obj, "isCar") and obj.isCar:
+                self.rotated_car = pygame.transform.rotate(
+                    self.car, math.degrees(obj.heading)
+                )
                 self.screen.blit(self.rotated_car, (rect_x, rect_y))
             else:
-                corners = [self.scenicToScreenVal(corner) for corner in obj.corners]
+                corners = [self.scenicToScreenVal(corner) for corner in obj._corners2D]
                 pygame.draw.polygon(self.screen, color, corners)
 
         pygame.display.update()
         time.sleep(self.timestep)
 
     def getProperties(self, obj, properties):
+        yaw, _, _ = obj.parentOrientation.globalToLocalAngles(obj.heading, 0, 0)
+
         values = dict(
             position=obj.position,
-            heading=obj.heading,
+            yaw=yaw,
+            pitch=0,
+            roll=0,
             velocity=obj.velocity,
             speed=obj.speed,
             angularSpeed=obj.angularSpeed,
+            angularVelocity=obj.angularVelocity,
         )
-        if 'elevation' in properties:
-            values['elevation'] = obj.elevation
+        if "elevation" in properties:
+            values["elevation"] = obj.elevation
         return values
 
+    def destroy(self):
+        if self.render:
+            pygame.quit()
+
     def getLaneFollowingControllers(self, agent):
         dt = self.timestep
         if agent.isCar:
             lon_controller = PIDLongitudinalController(K_P=0.5, K_D=0.1, K_I=0.7, dt=dt)
             lat_controller = PIDLateralController(K_P=0.1, K_D=0.1, K_I=0.02, dt=dt)
         else:
-            lon_controller = PIDLongitudinalController(K_P=0.25, K_D=0.025, K_I=0.0, dt=dt)
+            lon_controller = PIDLongitudinalController(
+                K_P=0.25, K_D=0.025, K_I=0.0, dt=dt
+            )
             lat_controller = PIDLateralController(K_P=0.2, K_D=0.1, K_I=0.0, dt=dt)
         return lon_controller, lat_controller
 
     def getTurningControllers(self, agent):
         dt = self.timestep
         if agent.isCar:
             lon_controller = PIDLongitudinalController(K_P=0.5, K_D=0.1, K_I=0.7, dt=dt)
             lat_controller = PIDLateralController(K_P=0.2, K_D=0.2, K_I=0.2, dt=dt)
         else:
-            lon_controller = PIDLongitudinalController(K_P=0.25, K_D=0.025, K_I=0.0, dt=dt)
+            lon_controller = PIDLongitudinalController(
+                K_P=0.25, K_D=0.025, K_I=0.0, dt=dt
+            )
             lat_controller = PIDLateralController(K_P=0.4, K_D=0.1, K_I=0.0, dt=dt)
         return lon_controller, lat_controller
 
     def getLaneChangingControllers(self, agent):
         dt = self.timestep
         if agent.isCar:
             lon_controller = PIDLongitudinalController(K_P=0.5, K_D=0.1, K_I=0.7, dt=dt)
             lat_controller = PIDLateralController(K_P=0.2, K_D=0.2, K_I=0.02, dt=dt)
         else:
-            lon_controller = PIDLongitudinalController(K_P=0.25, K_D=0.025, K_I=0.0, dt=dt)
+            lon_controller = PIDLongitudinalController(
+                K_P=0.25, K_D=0.025, K_I=0.0, dt=dt
+            )
             lat_controller = PIDLateralController(K_P=0.1, K_D=0.3, K_I=0.0, dt=dt)
         return lon_controller, lat_controller
```

### Comparing `scenic-2.1.0b4/src/scenic/simulators/utils/colors.py` & `scenic-3.0.0b2/src/scenic/simulators/utils/colors.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,103 +1,122 @@
-
 """A basic color type.
 
 This used for example to represent car colors in the abstract driving domain,
 as well as in the interfaces to GTA and Webots.
 """
 
-import colorsys
 from collections import namedtuple
+import colorsys
 import random
+import struct
 
-from scenic.core.distributions import Distribution, Range, Normal, Options, toDistribution
+from scenic.core.distributions import Distribution, Normal, Options, Range, toDistribution
 from scenic.core.lazy_eval import valueInContext
 from scenic.core.object_types import Mutator
 
-class Color(namedtuple('Color', ['r', 'g', 'b'])):
-	"""A color as an RGB tuple."""
-	@classmethod
-	def withBytes(cls, color):
-		return cls._make(c / 255.0 for c in color)
-
-	@staticmethod
-	def realToByte(color):
-		return tuple(int(round(255 * c)) for c in color)
-
-	@staticmethod
-	def uniformColor():
-		"""Return a uniformly random color."""
-		return toDistribution(Color(Range(0, 1), Range(0, 1), Range(0, 1)))
-
-	@staticmethod
-	def defaultCarColor():
-		"""Default color distribution for cars.
-
-		The distribution starts with a base distribution over 9 discrete colors,
-		then adds Gaussian HSL noise. The base distribution uses color popularity
-		statistics from a `2012 DuPont survey`_.
-
-		.. _2012 DuPont survey: https://web.archive.org/web/20121229065631/http://www2.dupont.com/Media_Center/en_US/color_popularity/Images_2012/DuPont2012ColorPopularity.pdf
-		"""
-		baseColors = {
-			(248, 248, 248): 0.24,	# white
-			(50, 50, 50): 0.19,		# black
-			(188, 185, 183): 0.16,	# silver
-			(130, 130, 130): 0.15,	# gray
-			(194, 92, 85): 0.10,	# red
-			(75, 119, 157): 0.07,	# blue
-			(197, 166, 134): 0.05,	# brown/beige
-			(219, 191, 105): 0.02,	# yellow/gold
-			(68, 160, 135): 0.02,	# green
-		}
-		converted = { Color.withBytes(color): prob for color, prob in baseColors.items() }
-		baseColor = Options(converted)
-		# TODO improve this?
-		hueNoise = Normal(0, 0.1)
-		satNoise = Normal(0, 0.1)
-		lightNoise = Normal(0, 0.1)
-		return NoisyColorDistribution(baseColor, hueNoise, satNoise, lightNoise)
+
+class Color(namedtuple("Color", ["r", "g", "b"])):
+    """A color as an RGB tuple."""
+
+    @classmethod
+    def withBytes(cls, color):
+        return cls._make(c / 255.0 for c in color)
+
+    @staticmethod
+    def realToByte(color):
+        return tuple(int(round(255 * c)) for c in color)
+
+    @staticmethod
+    def encodeTo(color, stream):
+        stream.write(struct.pack("<ddd", *color))
+
+    @staticmethod
+    def decodeFrom(stream):
+        return Color(*struct.unpack("<ddd", stream.read(24)))
+
+    @staticmethod
+    def uniformColor():
+        """Return a uniformly random color."""
+        return toDistribution(Color(Range(0, 1), Range(0, 1), Range(0, 1)))
+
+    @staticmethod
+    def defaultCarColor():
+        """Default color distribution for cars.
+
+        The distribution starts with a base distribution over 9 discrete colors,
+        then adds Gaussian HSL noise. The base distribution uses color popularity
+        statistics from a `2012 DuPont survey`_.
+
+        .. _2012 DuPont survey: https://web.archive.org/web/20121229065631/http://www2.dupont.com/Media_Center/en_US/color_popularity/Images_2012/DuPont2012ColorPopularity.pdf
+        """
+        baseColors = {
+            (248, 248, 248): 0.24,  # white
+            (50, 50, 50): 0.19,  # black
+            (188, 185, 183): 0.16,  # silver
+            (130, 130, 130): 0.15,  # gray
+            (194, 92, 85): 0.10,  # red
+            (75, 119, 157): 0.07,  # blue
+            (197, 166, 134): 0.05,  # brown/beige
+            (219, 191, 105): 0.02,  # yellow/gold
+            (68, 160, 135): 0.02,  # green
+        }
+        converted = {Color.withBytes(color): prob for color, prob in baseColors.items()}
+        baseColor = Options(converted)
+        # TODO improve this?
+        hueNoise = Normal(0, 0.1)
+        satNoise = Normal(0, 0.1)
+        lightNoise = Normal(0, 0.1)
+        return NoisyColorDistribution(baseColor, hueNoise, satNoise, lightNoise)
+
 
 class NoisyColorDistribution(Distribution):
-	"""A distribution given by HSL noise around a base color.
+    """A distribution given by HSL noise around a base color.
+
+    Arguments:
+        baseColor (RGB tuple): base color
+        hueNoise (float): noise to add to base hue
+        satNoise (float): noise to add to base saturation
+        lightNoise (float): noise to add to base lightness
+    """
+
+    def __init__(self, baseColor, hueNoise, satNoise, lightNoise):
+        super().__init__(baseColor, hueNoise, satNoise, lightNoise, valueType=Color)
+        self.baseColor = baseColor
+        self.hueNoise = hueNoise
+        self.satNoise = satNoise
+        self.lightNoise = lightNoise
+
+    @staticmethod
+    def addNoiseTo(color, hueNoise, lightNoise, satNoise):
+        hue, lightness, saturation = colorsys.rgb_to_hls(*color)
+        hue = max(0, min(1, hue + hueNoise))
+        lightness = max(0, min(1, lightness + lightNoise))
+        saturation = max(0, min(1, saturation + satNoise))
+        return colorsys.hls_to_rgb(hue, lightness, saturation)
+
+    def sampleGiven(self, value):
+        bc = value[self.baseColor]
+        return Color(
+            *self.addNoiseTo(
+                bc, value[self.hueNoise], value[self.lightNoise], value[self.satNoise]
+            )
+        )
+
+    def evaluateInner(self, context):
+        self.baseColor = valueInContext(self.baseColor, context)
+        self.hueNoise = valueInContext(self.hueNoise, context)
+        self.satNoise = valueInContext(self.satNoise, context)
+        self.lightNoise = valueInContext(self.lightNoise, context)
 
-	Arguments:
-		baseColor (RGB tuple): base color
-		hueNoise (float): noise to add to base hue
-		satNoise (float): noise to add to base saturation
-		lightNoise (float): noise to add to base lightness
-	"""
-
-	def __init__(self, baseColor, hueNoise, satNoise, lightNoise):
-		super().__init__(baseColor, hueNoise, satNoise, lightNoise, valueType=Color)
-		self.baseColor = baseColor
-		self.hueNoise = hueNoise
-		self.satNoise = satNoise
-		self.lightNoise = lightNoise
-
-	@staticmethod
-	def addNoiseTo(color, hueNoise, lightNoise, satNoise):
-		hue, lightness, saturation = colorsys.rgb_to_hls(*color)
-		hue = max(0, min(1, hue + hueNoise))
-		lightness = max(0, min(1, lightness + lightNoise))
-		saturation = max(0, min(1, saturation + satNoise))
-		return colorsys.hls_to_rgb(hue, lightness, saturation)
-
-	def sampleGiven(self, value):
-		bc = value[self.baseColor]
-		return Color(*self.addNoiseTo(bc, value[self.hueNoise],
-		    value[self.lightNoise], value[self.satNoise]))
-
-	def evaluateInner(self, context):
-		self.baseColor = valueInContext(self.baseColor, context)
-		self.hueNoise = valueInContext(self.hueNoise, context)
-		self.satNoise = valueInContext(self.satNoise, context)
-		self.lightNoise = valueInContext(self.lightNoise, context)
 
 class ColorMutator(Mutator):
-	"""Mutator that adds Gaussian HSL noise to the ``color`` property."""
-	def appliedTo(self, obj):
-		hueNoise = random.gauss(0, 0.05)
-		satNoise = random.gauss(0, 0.05)
-		lightNoise = random.gauss(0, 0.05)
-		color = NoisyColorDistribution.addNoiseTo(obj.color, hueNoise, lightNoise, satNoise)
-		return tuple([obj._copyWith(color=color), True])		# allow further mutation
+    """Mutator that adds Gaussian HSL noise to the ``color`` property."""
+
+    def appliedTo(self, obj):
+        stddev = 0.05 * obj.mutationScale
+        hueNoise = random.gauss(0, stddev)
+        satNoise = random.gauss(0, stddev)
+        lightNoise = random.gauss(0, stddev)
+        color = NoisyColorDistribution.addNoiseTo(
+            obj.color, hueNoise, lightNoise, satNoise
+        )
+        return (obj._copyWith(color=color), True)  # allow further mutation
```

### Comparing `scenic-2.1.0b4/src/scenic/simulators/webots/WBT.g4` & `scenic-3.0.0b2/src/scenic/simulators/webots/WBT.g4`

 * *Files identical despite different names*

### Comparing `scenic-2.1.0b4/src/scenic/simulators/webots/WBTParser.py` & `scenic-3.0.0b2/src/scenic/simulators/webots/WBTParser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,58 @@
-# Generated from WBT.g4 by ANTLR 4.8
+# Generated from WBT.g4 by ANTLR 4.11.1
 # encoding: utf-8
-from antlr4 import *
 from io import StringIO
 import sys
+
+from antlr4 import *
+
 if sys.version_info[1] > 5:
-	from typing import TextIO
+    from typing import TextIO
 else:
-	from typing.io import TextIO
-
+    from typing.io import TextIO
 
 def serializedATN():
-    with StringIO() as buf:
-        buf.write("\3\u608b\ua72a\u8133\ub9ed\u417c\u3be7\u7786\u5964\3\21")
-        buf.write("q\4\2\t\2\4\3\t\3\4\4\t\4\4\5\t\5\4\6\t\6\4\7\t\7\4\b")
-        buf.write("\t\b\4\t\t\t\4\n\t\n\4\13\t\13\4\f\t\f\3\2\3\2\7\2\33")
-        buf.write("\n\2\f\2\16\2\36\13\2\3\3\3\3\3\3\3\3\3\4\3\4\3\4\3\4")
-        buf.write("\3\4\3\4\5\4*\n\4\3\5\3\5\3\5\7\5/\n\5\f\5\16\5\62\13")
-        buf.write("\5\3\6\3\6\3\6\3\6\3\6\5\69\n\6\3\7\3\7\3\7\3\7\3\7\5")
-        buf.write("\7@\n\7\3\b\6\bC\n\b\r\b\16\bD\3\t\3\t\3\n\3\n\3\n\7\n")
-        buf.write("L\n\n\f\n\16\nO\13\n\3\n\5\nR\n\n\3\n\3\n\3\n\3\n\3\n")
-        buf.write("\6\nY\n\n\r\n\16\nZ\3\n\5\n^\n\n\3\n\3\n\5\nb\n\n\3\13")
-        buf.write("\5\13e\n\13\3\13\3\13\5\13i\n\13\6\13k\n\13\r\13\16\13")
-        buf.write("l\3\f\3\f\3\f\2\2\r\2\4\6\b\n\f\16\20\22\24\26\2\3\3\2")
-        buf.write("\n\13\2w\2\34\3\2\2\2\4\37\3\2\2\2\6#\3\2\2\2\b\60\3\2")
-        buf.write("\2\2\n8\3\2\2\2\f?\3\2\2\2\16B\3\2\2\2\20F\3\2\2\2\22")
-        buf.write("a\3\2\2\2\24j\3\2\2\2\26n\3\2\2\2\30\33\5\6\4\2\31\33")
-        buf.write("\5\4\3\2\32\30\3\2\2\2\32\31\3\2\2\2\33\36\3\2\2\2\34")
-        buf.write("\32\3\2\2\2\34\35\3\2\2\2\35\3\3\2\2\2\36\34\3\2\2\2\37")
-        buf.write(" \7\3\2\2 !\7\16\2\2!\"\5\6\4\2\"\5\3\2\2\2#$\7\16\2\2")
-        buf.write("$%\7\4\2\2%&\7\21\2\2&\'\5\b\5\2\')\7\5\2\2(*\7\21\2\2")
-        buf.write(")(\3\2\2\2)*\3\2\2\2*\7\3\2\2\2+,\5\n\6\2,-\7\21\2\2-")
-        buf.write("/\3\2\2\2.+\3\2\2\2/\62\3\2\2\2\60.\3\2\2\2\60\61\3\2")
-        buf.write("\2\2\61\t\3\2\2\2\62\60\3\2\2\2\63\64\7\6\2\2\64\65\7")
-        buf.write("\16\2\2\659\5\f\7\2\66\67\7\16\2\2\679\5\f\7\28\63\3\2")
-        buf.write("\2\28\66\3\2\2\29\13\3\2\2\2:@\5\16\b\2;@\5\20\t\2<@\5")
-        buf.write("\22\n\2=@\5\6\4\2>@\5\26\f\2?:\3\2\2\2?;\3\2\2\2?<\3\2")
-        buf.write("\2\2?=\3\2\2\2?>\3\2\2\2@\r\3\2\2\2AC\7\17\2\2BA\3\2\2")
-        buf.write("\2CD\3\2\2\2DB\3\2\2\2DE\3\2\2\2E\17\3\2\2\2FG\7\20\2")
-        buf.write("\2G\21\3\2\2\2HM\7\7\2\2IJ\7\21\2\2JL\5\f\7\2KI\3\2\2")
-        buf.write("\2LO\3\2\2\2MK\3\2\2\2MN\3\2\2\2NQ\3\2\2\2OM\3\2\2\2P")
-        buf.write("R\7\21\2\2QP\3\2\2\2QR\3\2\2\2RS\3\2\2\2Sb\7\b\2\2TU\7")
-        buf.write("\7\2\2UX\5\24\13\2VW\7\t\2\2WY\5\24\13\2XV\3\2\2\2YZ\3")
-        buf.write("\2\2\2ZX\3\2\2\2Z[\3\2\2\2[]\3\2\2\2\\^\7\t\2\2]\\\3\2")
-        buf.write("\2\2]^\3\2\2\2^_\3\2\2\2_`\7\b\2\2`b\3\2\2\2aH\3\2\2\2")
-        buf.write("aT\3\2\2\2b\23\3\2\2\2ce\7\21\2\2dc\3\2\2\2de\3\2\2\2")
-        buf.write("ef\3\2\2\2fh\7\17\2\2gi\7\21\2\2hg\3\2\2\2hi\3\2\2\2i")
-        buf.write("k\3\2\2\2jd\3\2\2\2kl\3\2\2\2lj\3\2\2\2lm\3\2\2\2m\25")
-        buf.write("\3\2\2\2no\t\2\2\2o\27\3\2\2\2\21\32\34)\608?DMQZ]adh")
-        buf.write("l")
-        return buf.getvalue()
-
+    return [
+        4,1,15,111,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,2,6,7,
+        6,2,7,7,7,2,8,7,8,2,9,7,9,2,10,7,10,1,0,1,0,5,0,25,8,0,10,0,12,0,
+        28,9,0,1,1,1,1,1,1,1,1,1,2,1,2,1,2,1,2,1,2,1,2,3,2,40,8,2,1,3,1,
+        3,1,3,5,3,45,8,3,10,3,12,3,48,9,3,1,4,1,4,1,4,1,4,1,4,3,4,55,8,4,
+        1,5,1,5,1,5,1,5,1,5,3,5,62,8,5,1,6,4,6,65,8,6,11,6,12,6,66,1,7,1,
+        7,1,8,1,8,1,8,5,8,74,8,8,10,8,12,8,77,9,8,1,8,3,8,80,8,8,1,8,1,8,
+        1,8,1,8,1,8,4,8,87,8,8,11,8,12,8,88,1,8,3,8,92,8,8,1,8,1,8,3,8,96,
+        8,8,1,9,3,9,99,8,9,1,9,1,9,3,9,103,8,9,4,9,105,8,9,11,9,12,9,106,
+        1,10,1,10,1,10,0,0,11,0,2,4,6,8,10,12,14,16,18,20,0,1,1,0,8,9,117,
+        0,26,1,0,0,0,2,29,1,0,0,0,4,33,1,0,0,0,6,46,1,0,0,0,8,54,1,0,0,0,
+        10,61,1,0,0,0,12,64,1,0,0,0,14,68,1,0,0,0,16,95,1,0,0,0,18,104,1,
+        0,0,0,20,108,1,0,0,0,22,25,3,4,2,0,23,25,3,2,1,0,24,22,1,0,0,0,24,
+        23,1,0,0,0,25,28,1,0,0,0,26,24,1,0,0,0,26,27,1,0,0,0,27,1,1,0,0,
+        0,28,26,1,0,0,0,29,30,5,1,0,0,30,31,5,12,0,0,31,32,3,4,2,0,32,3,
+        1,0,0,0,33,34,5,12,0,0,34,35,5,2,0,0,35,36,5,15,0,0,36,37,3,6,3,
+        0,37,39,5,3,0,0,38,40,5,15,0,0,39,38,1,0,0,0,39,40,1,0,0,0,40,5,
+        1,0,0,0,41,42,3,8,4,0,42,43,5,15,0,0,43,45,1,0,0,0,44,41,1,0,0,0,
+        45,48,1,0,0,0,46,44,1,0,0,0,46,47,1,0,0,0,47,7,1,0,0,0,48,46,1,0,
+        0,0,49,50,5,4,0,0,50,51,5,12,0,0,51,55,3,10,5,0,52,53,5,12,0,0,53,
+        55,3,10,5,0,54,49,1,0,0,0,54,52,1,0,0,0,55,9,1,0,0,0,56,62,3,12,
+        6,0,57,62,3,14,7,0,58,62,3,16,8,0,59,62,3,4,2,0,60,62,3,20,10,0,
+        61,56,1,0,0,0,61,57,1,0,0,0,61,58,1,0,0,0,61,59,1,0,0,0,61,60,1,
+        0,0,0,62,11,1,0,0,0,63,65,5,13,0,0,64,63,1,0,0,0,65,66,1,0,0,0,66,
+        64,1,0,0,0,66,67,1,0,0,0,67,13,1,0,0,0,68,69,5,14,0,0,69,15,1,0,
+        0,0,70,75,5,5,0,0,71,72,5,15,0,0,72,74,3,10,5,0,73,71,1,0,0,0,74,
+        77,1,0,0,0,75,73,1,0,0,0,75,76,1,0,0,0,76,79,1,0,0,0,77,75,1,0,0,
+        0,78,80,5,15,0,0,79,78,1,0,0,0,79,80,1,0,0,0,80,81,1,0,0,0,81,96,
+        5,6,0,0,82,83,5,5,0,0,83,86,3,18,9,0,84,85,5,7,0,0,85,87,3,18,9,
+        0,86,84,1,0,0,0,87,88,1,0,0,0,88,86,1,0,0,0,88,89,1,0,0,0,89,91,
+        1,0,0,0,90,92,5,7,0,0,91,90,1,0,0,0,91,92,1,0,0,0,92,93,1,0,0,0,
+        93,94,5,6,0,0,94,96,1,0,0,0,95,70,1,0,0,0,95,82,1,0,0,0,96,17,1,
+        0,0,0,97,99,5,15,0,0,98,97,1,0,0,0,98,99,1,0,0,0,99,100,1,0,0,0,
+        100,102,5,13,0,0,101,103,5,15,0,0,102,101,1,0,0,0,102,103,1,0,0,
+        0,103,105,1,0,0,0,104,98,1,0,0,0,105,106,1,0,0,0,106,104,1,0,0,0,
+        106,107,1,0,0,0,107,19,1,0,0,0,108,109,7,0,0,0,109,21,1,0,0,0,15,
+        24,26,39,46,54,61,66,75,79,88,91,95,98,102,106
+    ]
 
 class WBTParser ( Parser ):
 
     grammarFileName = "WBT.g4"
 
     atn = ATNDeserializer().deserialize(serializedATN())
 
@@ -99,22 +98,23 @@
     Identifier=12
     Number=13
     String=14
     Newline=15
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.8")
+        self.checkVersion("4.11.1")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
 
 
 
     class WorldContext(ParserRuleContext):
+        __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def node(self, i:int=None):
             if i is None:
@@ -148,23 +148,23 @@
         self.enterRule(localctx, 0, self.RULE_world)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
             self.state = 26
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            while _la==WBTParser.T__0 or _la==WBTParser.Identifier:
+            while _la==1 or _la==12:
                 self.state = 24
                 self._errHandler.sync(self)
                 token = self._input.LA(1)
-                if token in [WBTParser.Identifier]:
+                if token in [12]:
                     self.state = 22
                     self.node()
                     pass
-                elif token in [WBTParser.T__0]:
+                elif token in [1]:
                     self.state = 23
                     self.defn()
                     pass
                 else:
                     raise NoViableAltException(self)
 
                 self.state = 28
@@ -177,14 +177,15 @@
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
 
     class DefnContext(ParserRuleContext):
+        __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def Identifier(self):
             return self.getToken(WBTParser.Identifier, 0)
@@ -223,14 +224,15 @@
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
 
     class NodeContext(ParserRuleContext):
+        __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def Identifier(self):
             return self.getToken(WBTParser.Identifier, 0)
@@ -287,14 +289,15 @@
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
 
     class NodeBodyContext(ParserRuleContext):
+        __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def attribute(self, i:int=None):
             if i is None:
@@ -327,15 +330,15 @@
         self.enterRule(localctx, 6, self.RULE_nodeBody)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
             self.state = 46
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            while _la==WBTParser.T__3 or _la==WBTParser.Identifier:
+            while _la==4 or _la==12:
                 self.state = 41
                 self.attribute()
                 self.state = 42
                 self.match(WBTParser.Newline)
                 self.state = 48
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
@@ -346,14 +349,15 @@
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
 
     class AttributeContext(ParserRuleContext):
+        __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def Identifier(self):
             return self.getToken(WBTParser.Identifier, 0)
@@ -378,24 +382,24 @@
 
         localctx = WBTParser.AttributeContext(self, self._ctx, self.state)
         self.enterRule(localctx, 8, self.RULE_attribute)
         try:
             self.state = 54
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [WBTParser.T__3]:
+            if token in [4]:
                 self.enterOuterAlt(localctx, 1)
                 self.state = 49
                 self.match(WBTParser.T__3)
                 self.state = 50
                 self.match(WBTParser.Identifier)
                 self.state = 51
                 self.value()
                 pass
-            elif token in [WBTParser.Identifier]:
+            elif token in [12]:
                 self.enterOuterAlt(localctx, 2)
                 self.state = 52
                 self.match(WBTParser.Identifier)
                 self.state = 53
                 self.value()
                 pass
             else:
@@ -407,14 +411,15 @@
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
 
     class ValueContext(ParserRuleContext):
+        __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def vector(self):
             return self.getTypedRuleContext(WBTParser.VectorContext,0)
@@ -452,35 +457,35 @@
 
         localctx = WBTParser.ValueContext(self, self._ctx, self.state)
         self.enterRule(localctx, 10, self.RULE_value)
         try:
             self.state = 61
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [WBTParser.Number]:
+            if token in [13]:
                 self.enterOuterAlt(localctx, 1)
                 self.state = 56
                 self.vector()
                 pass
-            elif token in [WBTParser.String]:
+            elif token in [14]:
                 self.enterOuterAlt(localctx, 2)
                 self.state = 57
                 self.string()
                 pass
-            elif token in [WBTParser.T__4]:
+            elif token in [5]:
                 self.enterOuterAlt(localctx, 3)
                 self.state = 58
                 self.array()
                 pass
-            elif token in [WBTParser.Identifier]:
+            elif token in [12]:
                 self.enterOuterAlt(localctx, 4)
                 self.state = 59
                 self.node()
                 pass
-            elif token in [WBTParser.T__7, WBTParser.T__8]:
+            elif token in [8, 9]:
                 self.enterOuterAlt(localctx, 5)
                 self.state = 60
                 self.boolean()
                 pass
             else:
                 raise NoViableAltException(self)
 
@@ -490,14 +495,15 @@
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
 
     class VectorContext(ParserRuleContext):
+        __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def Number(self, i:int=None):
             if i is None:
@@ -529,27 +535,28 @@
             _la = self._input.LA(1)
             while True:
                 self.state = 63
                 self.match(WBTParser.Number)
                 self.state = 66 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if not (_la==WBTParser.Number):
+                if not (_la==13):
                     break
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
 
     class StringContext(ParserRuleContext):
+        __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def String(self):
             return self.getToken(WBTParser.String, 0)
@@ -580,14 +587,15 @@
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
 
     class ArrayContext(ParserRuleContext):
+        __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def Newline(self, i:int=None):
             if i is None:
@@ -646,15 +654,15 @@
                     self.state = 77
                     self._errHandler.sync(self)
                     _alt = self._interp.adaptivePredict(self._input,7,self._ctx)
 
                 self.state = 79
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==WBTParser.Newline:
+                if _la==15:
                     self.state = 78
                     self.match(WBTParser.Newline)
 
 
                 self.state = 81
                 self.match(WBTParser.T__5)
                 pass
@@ -680,15 +688,15 @@
                     self.state = 88 
                     self._errHandler.sync(self)
                     _alt = self._interp.adaptivePredict(self._input,9,self._ctx)
 
                 self.state = 91
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==WBTParser.T__6:
+                if _la==7:
                     self.state = 90
                     self.match(WBTParser.T__6)
 
 
                 self.state = 93
                 self.match(WBTParser.T__5)
                 pass
@@ -700,14 +708,15 @@
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
 
     class VectorWithNewlinesContext(ParserRuleContext):
+        __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def Number(self, i:int=None):
             if i is None:
@@ -743,15 +752,15 @@
             self.state = 104 
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while True:
                 self.state = 98
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==WBTParser.Newline:
+                if _la==15:
                     self.state = 97
                     self.match(WBTParser.Newline)
 
 
                 self.state = 100
                 self.match(WBTParser.Number)
                 self.state = 102
@@ -761,27 +770,28 @@
                     self.state = 101
                     self.match(WBTParser.Newline)
 
 
                 self.state = 106 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if not (_la==WBTParser.Number or _la==WBTParser.Newline):
+                if not (_la==13 or _la==15):
                     break
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
 
     class BooleanContext(ParserRuleContext):
+        __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
 
         def getRuleIndex(self):
@@ -801,15 +811,15 @@
         localctx = WBTParser.BooleanContext(self, self._ctx, self.state)
         self.enterRule(localctx, 20, self.RULE_boolean)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
             self.state = 108
             _la = self._input.LA(1)
-            if not(_la==WBTParser.T__7 or _la==WBTParser.T__8):
+            if not(_la==8 or _la==9):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
```

### Comparing `scenic-2.1.0b4/src/scenic/simulators/webots/WBTVisitor.py` & `scenic-3.0.0b2/src/scenic/simulators/webots/WBTVisitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# Generated from WBT.g4 by ANTLR 4.8
+# Generated from WBT.g4 by ANTLR 4.11.1
 from antlr4 import *
+
 if __name__ is not None and "." in __name__:
     from .WBTParser import WBTParser
 else:
     from WBTParser import WBTParser
 
 # This class defines a complete generic visitor for a parse tree produced by WBTParser.
```

### Comparing `scenic-2.1.0b4/src/scenic/simulators/webots/actions.py` & `scenic-3.0.0b2/src/scenic/simulators/webots/actions.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,39 +2,45 @@
 
 import pickle
 
 from scenic.core.simulators import Action
 from scenic.core.type_support import toScalar, toVector
 import scenic.simulators.webots.utils as utils
 
+
 class OffsetAction(Action):
     """Move an object by the given offset relative to its current heading."""
+
     def __init__(self, offset):
-        self.offset = toVector(offset, 'OffsetAction with non-vector offset')
+        self.offset = toVector(offset, "OffsetAction with non-vector offset")
 
     def applyTo(self, obj, sim):
         pos = obj.position.offsetRotated(obj.heading, self.offset)
         pos = sim.coordinateSystem.positionFromScenic(pos, elevation=obj.elevation)
-        obj.webotsObject.getField('translation').setSFVec3f(pos)
+        obj.webotsObject.getField("translation").setSFVec3f(pos)
+
 
 class ApplyForceAction(Action):
     """Apply a given force to the object."""
+
     def __init__(self, force, relative=False):
-        self.force = toVector(force, 'ApplyForceAction with non-vector force')
+        self.force = toVector(force, "ApplyForceAction with non-vector force")
         self.relative = relative
 
     def applyTo(self, obj, sim):
         force = sim.coordinateSystem.positionFromScenic(self.force)
         obj.webotsObject.addForce(force, self.relative)
 
+
 class WriteFileAction(Action):
     """Pickle the given data and write the result to a file.
 
     For use in communication with external controllers or other code.
     """
+
     def __init__(self, path, data):
         self.path = path
         self.data = data
 
     def applyTo(self, obj, sim):
-        with open(self.path, 'wb') as outFile:
+        with open(self.path, "wb") as outFile:
             pickle.dump(self.data, outFile)
```

### Comparing `scenic-2.1.0b4/src/scenic/simulators/webots/guideways/model.scenic` & `scenic-3.0.0b2/src/scenic/simulators/webots/guideways/model.scenic`

 * *Files 19% similar despite different names*

```diff
@@ -4,38 +4,38 @@
 from scenic.simulators.webots.guideways.interface import Intersection, IntersectionWorkspace
 from scenic.simulators.webots.guideways.intersection import intersectionPath, intersectionOrigin
 from scenic.simulators.webots.road.car_models import CarModel, carModels, modelWithName
 
 # Load intersection information and set up workspace
 
 if intersectionPath is None:
-	raise RuntimeError('need to select intersection for this scenario')
+    raise RuntimeError('need to select intersection for this scenario')
 with open(intersectionPath, 'r') as f:
-	intersection = Intersection(json.load(f), origin=intersectionOrigin)
+    intersection = Intersection(json.load(f), origin=intersectionOrigin)
 
 workspace = IntersectionWorkspace(intersection)
 
 # Set up various regions
 
 road = workspace.drivableRegion
-roadDirection = workspace.roadDirection		# NOTE: chooses arbitrarily where guideways overlap!
+roadDirection = workspace.roadDirection     # NOTE: chooses arbitrarily where guideways overlap!
 
 # Types of objects
 
 class Car:
-	regionContainedIn: road
-	position: Point on road
-	heading: roadDirection at self.position
-	webotsType: self.model.name
-	model: modelWithName['ToyotaPrius']
-	width: self.model.width
-	length: self.model.length
-	requireVisible: False
-	viewAngle: 90 deg
-	visibleDistance: 60
-	cameraOffset: 0 @ (self.length / 2)		# camera is at the front
+    regionContainedIn: road
+    position: new Point on road
+    heading: roadDirection at self.position
+    webotsType: self.model.name
+    model: modelWithName['ToyotaPrius']
+    width: self.model.width
+    length: self.model.length
+    requireVisible: False
+    viewAngle: 90 deg
+    visibleDistance: 60
+    cameraOffset: 0 @ (self.length / 2)     # camera is at the front
 
 class Marker:
-	width: 0.1
-	length: 0.1
-	allowCollisions: True
-	requireVisible: False
+    width: 0.1
+    length: 0.1
+    allowCollisions: True
+    requireVisible: False
```

### Comparing `scenic-2.1.0b4/src/scenic/simulators/webots/road/model.scenic` & `scenic-3.0.0b2/src/scenic/simulators/webots/road/model.scenic`

 * *Files 13% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import math
 import time
 
 import scenic.simulators.webots.world_parser as parser
 from scenic.simulators.webots.road.interface import WebotsWorkspace
 from scenic.simulators.webots.road.world import worldPath
 from scenic.simulators.webots.road.car_models import CarModel, carModels, \
-	modelWithName, smallVehicles
+    modelWithName, smallVehicles
 
 from scenic.simulators.utils.colors import Color as CarColor
 
 # Load map and set up workspace
 
 if worldPath is None:
-	raise RuntimeError('need to set Webots world for this scenario')
+    raise RuntimeError('need to set Webots world for this scenario')
 startTime = time.time()
 world = parser.parse(worldPath)
 totalTime = time.time() - startTime
 verbosePrint(f'Parsed .wbt file in {totalTime:.3} seconds.')
 
 workspace = WebotsWorkspace(world)
 
@@ -32,81 +32,82 @@
 sidewalk = workspace.sidewalksRegion
 crossing = workspace.crossingsRegion
 walkway = workspace.walkableRegion
 
 # types of objects
 
 class WebotsObject:
-	webotsName: 'unspecified_name'
-	webotsObject: None 	# gets filled in at simulation time
-	elevation: None 	# ditto (this is the Webots y coordinate)
+    webotsName: 'unspecified_name'
+    webotsObject: None  # gets filled in at simulation time
+    elevation: None     # ditto (this is the Webots y coordinate)
 
 class Car(WebotsObject):
-	regionContainedIn: road
-	position: Point on road
-	heading: (roadDirection at self.position) + self.roadDeviation
-	roadDeviation: 0
-	model: Uniform(*carModels)
-	width: self.model.width
-	length: self.model.length
-	webotsType: self.model.name
-	viewAngle: 90 deg
-	cameraOffset: 0 @ (self.length / 2)		# camera is at the front
-	color: CarColor.defaultCarColor()
+    regionContainedIn: road
+    position: new Point on road
+    heading: roadDirection at self.position
+    yaw: self.roadDeviation
+    roadDeviation: 0
+    model: Uniform(*carModels)
+    width: self.model.width
+    length: self.model.length
+    webotsType: self.model.name
+    viewAngle: 90 deg
+    cameraOffset: 0 @ (self.length / 2)     # camera is at the front
+    color: CarColor.defaultCarColor()
 
 class SmallCar(Car):
-	model: Uniform(*smallVehicles)
+    model: Uniform(*smallVehicles)
 
 class BmwX5(Car):
-	model: modelWithName['BmwX5']
+    model: modelWithName['BmwX5']
 
 class CitroenCZero(Car):
-	model: modelWithName['CitroenCZero']
+    model: modelWithName['CitroenCZero']
 
 class LincolnMKZ(Car):
-	model: modelWithName['LincolnMKZ']
+    model: modelWithName['LincolnMKZ']
 
 class RangeRoverSportSVR(Car):
-	model: modelWithName['RangeRoverSportSVR']
+    model: modelWithName['RangeRoverSportSVR']
 
 class ToyotaPrius(Car):
-	model: modelWithName['ToyotaPrius']
+    model: modelWithName['ToyotaPrius']
 
 class Bus(Car):
-	model: modelWithName['Bus']
+    model: modelWithName['Bus']
 
 class Truck(Car):
-	model: modelWithName['Truck']
+    model: modelWithName['Truck']
 
 class Tractor(Car):
-	model: modelWithName['Tractor']
+    model: modelWithName['Tractor']
 
 class Motorcycle(Car):
-	model: modelWithName['MotorBikeSimple']
-	primaryColor: CarColor.defaultCarColor()
-	secondaryColor: CarColor.uniformColor()		# TODO improve
+    model: modelWithName['MotorBikeSimple']
+    primaryColor: CarColor.defaultCarColor()
+    secondaryColor: CarColor.uniformColor()     # TODO improve
 
 class Pedestrian(WebotsObject):
-	regionContainedIn: walkway
-	position: Point on walkway
-	heading: Range(0, 360) deg
-	width: 0.5
-	length: 0.5
-	shirtColor: CarColor.uniformColor()
-	pantsColor: CarColor.uniformColor()
-	shoesColor: CarColor.uniformColor()
+    regionContainedIn: walkway
+    position: new Point on walkway
+    yaw: Range(0, 360) deg
+    width: 0.5
+    length: 0.5
+    shirtColor: CarColor.uniformColor()
+    pantsColor: CarColor.uniformColor()
+    shoesColor: CarColor.uniformColor()
 
 class OilBarrel(WebotsObject):
-	width: 0.61
-	length: 0.61
+    width: 0.61
+    length: 0.61
 
 class SolidBox(WebotsObject):
-	width: 2
-	length: 2
+    width: 2
+    length: 2
 
 class TrafficCone(WebotsObject):
-	width: 0.5
-	length: 0.5
+    width: 0.5
+    length: 0.5
 
 class WorkBarrier(WebotsObject):
-	width: 1.2
-	length: 0.4
+    width: 1.2
+    length: 0.4
```

### Comparing `scenic-2.1.0b4/src/scenic/simulators/webots/simulator.py` & `scenic-3.0.0b2/src/scenic/simulators/webots/simulator.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,165 +11,284 @@
 are instances of `WebotsObject` will be matched to Webots nodes; see the model
 documentation for details.
 
 .. _Robot node: https://www.cyberbotics.com/doc/reference/robot
 """
 
 from collections import defaultdict
+import ctypes
 import math
-
-from scenic.core.simulators import Simulator, Simulation, Action
+from os import path
+import tempfile
+from textwrap import dedent
+
+import trimesh
+
+from scenic.core.regions import MeshVolumeRegion
+from scenic.core.simulators import Simulation, Simulator
+from scenic.core.type_support import toOrientation
 from scenic.core.vectors import Vector
-from scenic.simulators.webots.utils import WebotsCoordinateSystem, ENU
+from scenic.simulators.webots.utils import ENU, WebotsCoordinateSystem
+
 
 class WebotsSimulator(Simulator):
     """`Simulator` object for Webots.
 
     Args:
         supervisor: Supervisor node handle from the Webots Python API.
     """
+
     def __init__(self, supervisor):
         super().__init__()
         self.supervisor = supervisor
-        topLevelNodes = supervisor.getRoot().getField('children')
+        topLevelNodes = supervisor.getRoot().getField("children")
         worldInfo = None
         for i in range(topLevelNodes.getCount()):
             child = topLevelNodes.getMFNode(i)
-            if child.getTypeName() == 'WorldInfo':
+            if child.getTypeName() == "WorldInfo":
                 worldInfo = child
                 break
         if not worldInfo:
-            raise RuntimeError('Webots world does not contain a WorldInfo node')
-        system = worldInfo.getField('coordinateSystem').getSFString()
+            raise RuntimeError("Webots world does not contain a WorldInfo node")
+        system = worldInfo.getField("coordinateSystem").getSFString()
         self.coordinateSystem = WebotsCoordinateSystem(system)
 
-    def createSimulation(self, scene, verbosity=0):
-        return WebotsSimulation(scene, self.supervisor,
-                                coordinateSystem=self.coordinateSystem)
+    def createSimulation(self, scene, **kwargs):
+        return WebotsSimulation(
+            scene, self.supervisor, coordinateSystem=self.coordinateSystem, **kwargs
+        )
+
 
 class WebotsSimulation(Simulation):
     """`Simulation` object for Webots.
 
     Attributes:
         supervisor: Webots supervisor node used for the simulation. This is
             exposed for the use of scenarios which need to call Webots APIs
-            directly; e.g. :samp:`simulation().supervisor.setLabel({...})`.
+            directly; e.g. :scenic:`simulation().supervisor.setLabel({...})`.
     """
-    def __init__(self, scene, supervisor, verbosity=0, coordinateSystem=ENU):
-        timestep = supervisor.getBasicTimeStep() / 1000
-        super().__init__(scene, timestep=timestep, verbosity=verbosity)
+
+    def __init__(self, scene, supervisor, coordinateSystem=ENU, *, timestep, **kwargs):
         self.supervisor = supervisor
         self.coordinateSystem = coordinateSystem
-        self.objects = scene.objects
+        self.mode2D = scene.compileOptions.mode2D
+        self.nextAdHocObjectId = 1
+        self.usedObjectNames = defaultdict(lambda: 0)
+
+        # directory to store proto files for adhoc webots objects
+        self.tmpMeshDir = tempfile.mkdtemp()
+
+        timestep = supervisor.getBasicTimeStep() / 1000 if timestep is None else timestep
+
+        super().__init__(scene, timestep=timestep, **kwargs)
+
+    def setup(self):
+        super().setup()
 
-        # Find Webots objects corresponding to Scenic objects
-        self.webotsObjects = {}
-        usedNames = defaultdict(lambda: 0)
-        for obj in self.objects:
-            if not hasattr(obj, 'webotsName'):
-                continue    # not a Webots object
+        # Reset Webots simulation
+        self.supervisor.simulationResetPhysics()
+
+    def createObjectInSimulator(self, obj):
+        if not hasattr(obj, "webotsName"):
+            return  # not a Webots object
+
+        # Find the name of the Webots node for this object.
+        name = None
+        if obj.webotsAdhoc is not None:
+            # Dynamically generate object from Scenic object
+            objectRawMesh = obj.shape.mesh
+            objectScaledMesh = MeshVolumeRegion(
+                mesh=objectRawMesh,
+                dimensions=(obj.width, obj.length, obj.height),
+            ).mesh
+            objFilePath = path.join(self.tmpMeshDir, f"{self.nextAdHocObjectId}.obj")
+            trimesh.exchange.export.export_mesh(objectScaledMesh, objFilePath)
+
+            name = self._getAdhocObjectName(self.nextAdHocObjectId)
+            protoName = (
+                "ScenicObjectWithPhysics" if isPhysicsEnabled(obj) else "ScenicObject"
+            )
+            protoDef = dedent(
+                f"""
+                DEF {name} {protoName} {{
+                    url "{objFilePath}"
+                }}
+                """
+            )
+
+            rootNode = self.supervisor.getRoot()
+            rootChildrenField = rootNode.getField("children")
+            rootChildrenField.importMFNodeFromString(-1, protoDef)
+            self.nextAdHocObjectId += 1
+        else:
             if obj.webotsName:
                 name = obj.webotsName
             else:
                 ty = obj.webotsType
                 if not ty:
-                    raise RuntimeError(f'object {obj} has no webotsName or webotsType')
-                nextID = usedNames[ty]
-                usedNames[ty] += 1
-                if nextID == 0 and supervisor.getFromDef(ty):
+                    raise RuntimeError(f"object {obj} has no webotsName or webotsType")
+                nextID = self.usedObjectNames[ty]
+                self.usedObjectNames[ty] += 1
+                if nextID == 0 and self.supervisor.getFromDef(ty):
                     name = ty
                 else:
-                    name = f'{ty}_{nextID}'
-            webotsObj = supervisor.getFromDef(name)
-            if webotsObj is None:
-                raise RuntimeError(f'Webots object {name} does not exist in world')
-            self.webotsObjects[obj] = webotsObj
-            obj.webotsObject = webotsObj
-            obj.webotsName = name
+                    name = f"{ty}_{nextID}"
 
-            # get starting elevation
+        # Get handle to Webots node.
+        webotsObj = self.supervisor.getFromDef(name)
+        if webotsObj is None:
+            raise SimulationCreationError(f"Webots object {name} does not exist in world")
+        obj.webotsObject = webotsObj
+        obj.webotsName = name
+
+        # Set the fields of the Webots object:
+
+        # position
+        if self.mode2D:  # 2D compatibility mode
+            # Set initial elevation if unspecified
             if obj.elevation is None:
-                pos = webotsObj.getField('translation').getSFVec3f()
+                pos = webotsObj.getField("translation").getSFVec3f()
                 spos = self.coordinateSystem.positionToScenic(pos)
                 obj.elevation = spos[2]
 
-        # Reset Webots simulation
-        supervisor.simulationResetPhysics()
-
-        # Set initial properties of Webots objects
-        self.writePropertiesToWebots()
-
-    def writePropertiesToWebots(self):
-        for obj, webotsObj in self.webotsObjects.items():
-            # position
+            # Overwrite Z value with elevation
             pos = self.coordinateSystem.positionFromScenic(
-                obj.position + obj.positionOffset,
-                elevation=obj.elevation
+                Vector(obj.position.x, obj.position.y, obj.elevation) + obj.positionOffset
             )
-            webotsObj.getField('translation').setSFVec3f(pos)
-            # heading
-            rot = self.coordinateSystem.rotationFromScenic(
-                obj.heading + obj.rotationOffset
+            webotsObj.getField("translation").setSFVec3f(pos)
+        else:
+            pos = self.coordinateSystem.positionFromScenic(
+                obj.position + obj.positionOffset
             )
-            webotsObj.getField('rotation').setSFRotation(rot)
-            # battery
-            battery = getattr(obj, 'battery', None)
-            if battery:
-                if not isinstance(battery, (tuple, list)) or len(battery) != 3:
-                    raise RuntimeError(f'"battery" of {obj.webotsName} does not'
-                                       ' have 3 components')
-                field = webotsObj.getField('battery')
-                field.setMFFloat(0, battery[0])
-                field.setMFFloat(1, battery[1])
-                field.setMFFloat(2, battery[2])
-            # customData
-            customData = getattr(obj, 'customData', None)
-            if customData:
-                if not isinstance(customData, str):
-                    raise RuntimeError(f'"customData" of {obj.webotsName} is not a string')
-                webotsObj.getField('customData').setSFString(customData)
-            # controller
-            if obj.controller:
-                controllerField = webotsObj.getField('controller')
-                curCont = controllerField.getSFString()
-                if obj.controller != curCont:
-                    # the following operation also causes the controller to be restarted
-                    controllerField.setSFString(obj.controller)
-                elif obj.resetController:
-                    webotsObj.restartController()
+            webotsObj.getField("translation").setSFVec3f(pos)
 
-    def createObjectInSimulator(self, obj):
-        raise RuntimeError('the Webots interface does not support dynamic object creation')
+        # orientation
+        offsetOrientation = toOrientation(obj.rotationOffset)
+        webotsObj.getField("rotation").setSFRotation(
+            self.coordinateSystem.orientationFromScenic(
+                obj.orientation, offsetOrientation
+            )
+        )
+
+        # density
+        densityField = getFieldSafe(webotsObj, "density")
+        if densityField is not None:
+            if obj.density is None:
+                # Get initial value for property if unspecified
+                obj.density = densityField.getSFFloat()
+            else:
+                densityField.setSFFloat(float(obj.density))
+
+        # battery
+        battery = getattr(obj, "battery", None)
+        if battery:
+            if not isinstance(battery, (tuple, list)) or len(battery) != 3:
+                raise TypeError(f'"battery" of {name} does not have 3 components')
+            field = webotsObj.getField("battery")
+            field.setMFFloat(0, battery[0])
+            field.setMFFloat(1, battery[1])
+            field.setMFFloat(2, battery[2])
+
+        # customData
+        customData = getattr(obj, "customData", None)
+        if customData:
+            if not isinstance(customData, str):
+                raise TypeError(f'"customData" of {name} is not a string')
+            webotsObj.getField("customData").setSFString(customData)
+
+        # controller
+        if obj.controller:
+            controllerField = webotsObj.getField("controller")
+            curCont = controllerField.getSFString()
+            if obj.controller != curCont:
+                # the following operation also causes the controller to be restarted
+                controllerField.setSFString(obj.controller)
+            elif obj.resetController:
+                webotsObj.restartController()
 
     def step(self):
         ms = round(1000 * self.timestep)
         self.supervisor.step(ms)
 
     def getProperties(self, obj, properties):
-        webotsObj = self.webotsObjects.get(obj)
-        if not webotsObj:   # static object with no Webots counterpart
-            return { prop: getattr(obj, prop) for prop in properties }
-
-        pos = webotsObj.getField('translation').getSFVec3f()
-        x, y, elevation = self.coordinateSystem.positionToScenic(pos)
-        rot = webotsObj.getField('rotation').getSFRotation()
-        heading = self.coordinateSystem.rotationToScenic(rot)
+        webotsObj = getattr(obj, "webotsObject", None)
+        if not webotsObj:  # static object with no Webots counterpart
+            return {prop: getattr(obj, prop) for prop in properties}
+
+        pos = webotsObj.getField("translation").getSFVec3f()
+        x, y, z = self.coordinateSystem.positionToScenic(pos)
         lx, ly, lz, ax, ay, az = webotsObj.getVelocity()
         vx, vy, vz = self.coordinateSystem.positionToScenic((lx, ly, lz))
-        velocity = (vx, vy)
+        velocity = Vector(vx, vy, vz)
         speed = math.hypot(*velocity)
+        angularSpeed = math.hypot(ax, ay, az)
+
+        offsetOrientation = toOrientation(obj.rotationOffset)
+        globalOrientation = self.coordinateSystem.orientationToScenic(
+            webotsObj.getField("rotation").getSFRotation(), offsetOrientation
+        )
+        yaw, pitch, roll = obj.parentOrientation.localAnglesFor(globalOrientation)
 
         values = dict(
-            position=Vector(x, y),
-            elevation=elevation,
-            heading=heading,
+            position=Vector(x, y, z),
             velocity=velocity,
             speed=speed,
-            angularSpeed=ay,
+            angularSpeed=angularSpeed,
+            angularVelocity=Vector(ax, ay, az),
+            yaw=yaw,
+            pitch=pitch,
+            roll=roll,
+            elevation=z,
         )
 
-        if hasattr(obj, 'battery'):
-            field = webotsObj.getField('battery')
+        if hasattr(obj, "battery"):
+            field = webotsObj.getField("battery")
             val = (field.getMFFloat(0), obj.battery[1], obj.battery[2])
-            values['battery'] = val
+            values["battery"] = val
 
         return values
+
+    def destroy(self):
+        # Destroy adhoc objects generated at the beginning of the simulation
+        for i in range(1, self.nextAdHocObjectId):
+            name = self._getAdhocObjectName(i)
+            node = self.supervisor.getFromDef(name)
+            node.remove()
+
+    def _getAdhocObjectName(self, i: int) -> str:
+        return f"SCENIC_ADHOC_{i}"
+
+
+def getFieldSafe(webotsObject, fieldName):
+    """Get field from webots object. Return null if no such field exists.
+
+    Needed to workaround this issue (https://github.com/cyberbotics/webots/issues/5646)
+
+    Args:
+        webotsObject: webots object
+        fieldName: name of the field to look for
+
+    Returns:
+        Field|None: Field object if the field with the given name exists. None otherwise.
+    """
+
+    field = webotsObject.getField(fieldName)
+    # this seems to always return some object, but return None if field is None
+    if field is None:
+        return None
+
+    # if field is valid, it has a valid pointer
+    if isinstance(field._ref, ctypes.c_void_p) and field._ref.value is not None:
+        # then the field is valid and we return the reference
+        return field
+
+    # if the pointer points to None, then the field does not exist on this object
+    return None
+
+
+def isPhysicsEnabled(webotsObject):
+    """Whether or not physics is enabled for this `WebotsObject`"""
+    if webotsObject.webotsAdhoc is None:
+        return webotsObject
+    if isinstance(webotsObject.webotsAdhoc, dict):
+        return webotsObject.webotsAdhoc.get("physics", True)
+    raise TypeError(f"webotsAdhoc must be None or a dictionary")
```

### Comparing `scenic-2.1.0b4/src/scenic/syntax/relations.py` & `scenic-3.0.0b2/src/scenic/syntax/relations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,92 +1,120 @@
-
 """Extracting relations (for later pruning) from the syntax of requirements."""
 
-import math
+from ast import (
+    Add,
+    BinOp,
+    Call,
+    Compare,
+    Eq,
+    Expression,
+    Gt,
+    GtE,
+    Lt,
+    LtE,
+    Name,
+    NotEq,
+    Sub,
+)
 from collections import defaultdict
-from ast import Compare, BinOp, Eq, NotEq, Lt, LtE, Gt, GtE, Call, Add, Sub, Expression, Name
+import math
 
 from scenic.core.distributions import needsSampling
-from scenic.core.object_types import Point, Object
-from scenic.core.errors import InvalidScenarioError, InconsistentScenarioError
+from scenic.core.errors import InconsistentScenarioError, InvalidScenarioError
+from scenic.core.object_types import Object, Point
+
 
 def inferRelationsFrom(reqNode, namespace, ego, line):
     """Infer relations between objects implied by a requirement."""
     matcher = RequirementMatcher(namespace)
 
     inferRelativeHeadingRelations(matcher, reqNode, ego, line)
     inferDistanceRelations(matcher, reqNode, ego, line)
 
+
 def inferRelativeHeadingRelations(matcher, reqNode, ego, line):
     """Infer bounds on relative headings from a requirement."""
-    rhMatcher = lambda node: matcher.matchUnaryFunction('RelativeHeading', node)
+    rhMatcher = lambda node: matcher.matchUnaryFunction("RelativeHeading", node)
     allBounds = matcher.matchBounds(reqNode, rhMatcher)
     for target, bounds in allBounds:
         if not isinstance(target, Object):
             continue
         assert target is not ego
         if ego is None:
-            raise InvalidScenarioError('relative heading w.r.t. unassigned ego on line {line}')
+            raise InvalidScenarioError(
+                "relative heading w.r.t. unassigned ego on line {line}"
+            )
         lower, upper = bounds
         if lower < -math.pi:
             lower = -math.pi
         if upper > math.pi:
             upper = math.pi
         if lower == -math.pi and upper == math.pi:
-            continue    # skip trivial bounds
+            continue  # skip trivial bounds
         rel = RelativeHeadingRelation(target, lower, upper)
         ego._relations.append(rel)
         conv = RelativeHeadingRelation(ego, -upper, -lower)
         target._relations.append(conv)
 
+
 def inferDistanceRelations(matcher, reqNode, ego, line):
     """Infer bounds on distances from a requirement."""
-    distMatcher = lambda node: matcher.matchUnaryFunction('DistanceFrom', node)
+    distMatcher = lambda node: matcher.matchUnaryFunction("DistanceFrom", node)
     allBounds = matcher.matchBounds(reqNode, distMatcher)
     for target, bounds in allBounds:
         if not isinstance(target, Object):
             continue
         assert target is not ego
         if ego is None:
-            raise InvalidScenarioError('distance w.r.t. unassigned ego on line {line}')
+            raise InvalidScenarioError("distance w.r.t. unassigned ego on line {line}")
         lower, upper = bounds
         if lower < 0:
             lower = 0
-            if upper == float('inf'):
-                continue    # skip trivial bounds
+            if upper == float("inf"):
+                continue  # skip trivial bounds
         rel = DistanceRelation(target, lower, upper)
         ego._relations.append(rel)
         conv = DistanceRelation(ego, lower, upper)
         target._relations.append(conv)
 
+
 class BoundRelation:
     """Abstract relation bounding something about another object."""
+
     def __init__(self, target, lower, upper):
         self.target = target
         self.lower, self.upper = lower, upper
 
+
 class RelativeHeadingRelation(BoundRelation):
     """Relation bounding another object's relative heading with respect to this one."""
+
     pass
 
+
 class DistanceRelation(BoundRelation):
     """Relation bounding another object's distance from this one."""
+
     pass
 
+
 class RequirementMatcher:
     def __init__(self, namespace):
         self.namespace = namespace
 
     def inconsistencyError(self, node, message):
         raise InconsistentScenarioError(node.lineno, message)
 
     def matchUnaryFunction(self, name, node):
         """Match a call to a specified unary function, returning the value of its argument."""
-        if not (isinstance(node, Call) and isinstance(node.func, Name)
-                and node.func.id == name):
+        if not (
+            isinstance(node, Call)
+            and isinstance(node.func, Name)
+            and node.func.id == name
+        ):
             return None
         if len(node.args) != 1:
             return None
         if len(node.keywords) != 0:
             return None
         return self.matchValue(node.args[0])
 
@@ -94,23 +122,23 @@
         """Match upper/lower bounds on something matched by the given function.
 
         Returns a list of all bounds found, pairing the bounded quantity with a
         pair (low, high) of lower/upper bounds.
         """
         if not isinstance(node, Compare):
             return {}
-        bounds = defaultdict(lambda: (float('-inf'), float('inf')))
+        bounds = defaultdict(lambda: (float("-inf"), float("inf")))
         targets = {}
         first = node.left
         for second, op in zip(node.comparators, node.ops):
             lower, upper, target = self.matchBoundsInner(first, second, op, matchAtom)
             first = second
             if target is None:
                 continue
-            targetID = id(target)    # use id to support unhashable types
+            targetID = id(target)  # use id to support unhashable types
             targets[targetID] = target
             bestLower, bestUpper = bounds[targetID]
             if lower is not None and lower > bestLower:
                 bestLower = lower
             if upper is not None and upper < bestUpper:
                 bestUpper = upper
             bounds[targetID] = (bestLower, bestUpper)
@@ -123,63 +151,75 @@
             return self.matchBoundsInner(right, left, Lt(), matchAtom)
         elif isinstance(op, GtE):
             return self.matchBoundsInner(right, left, LtE(), matchAtom)
         # Try matching a constant lower bound on the atom or its absolute value
         lconst = self.matchConstant(left)
         if isinstance(lconst, (int, float)):
             target = matchAtom(right)
-            if target is not None:     # CONST op QUANTITY
-                return (lconst, lconst, target) if isinstance(op, Eq) else (lconst, None, target)
+            if target is not None:  # CONST op QUANTITY
+                return (
+                    (lconst, lconst, target)
+                    if isinstance(op, Eq)
+                    else (lconst, None, target)
+                )
             else:
                 bounds = self.matchAbsBounds(right, lconst, op, False, matchAtom)
-                if bounds is not None:      # CONST op abs(QUANTITY [+/- CONST])
+                if bounds is not None:  # CONST op abs(QUANTITY [+/- CONST])
                     return bounds
         # Try matching a constant upper bound on the atom or its absolute value
         rconst = self.matchConstant(right)
         if isinstance(rconst, (int, float)):
             target = matchAtom(left)
-            if target is not None:      # QUANTITY op CONST
-                return (rconst, rconst, target) if isinstance(op, Eq) else (None, rconst, target)
+            if target is not None:  # QUANTITY op CONST
+                return (
+                    (rconst, rconst, target)
+                    if isinstance(op, Eq)
+                    else (None, rconst, target)
+                )
             else:
                 bounds = self.matchAbsBounds(left, rconst, op, True, matchAtom)
-                if bounds is not None:      # abs(QUANTITY [+/- CONST]) op CONST
+                if bounds is not None:  # abs(QUANTITY [+/- CONST]) op CONST
                     return bounds
         return None, None, None
 
     def matchAbsBounds(self, node, const, op, isUpperBound, matchAtom):
         """Extract bounds on an atom from a comparison involving its absolute value."""
-        if not (isinstance(node, Call) and isinstance(node.func, Name)
-                and node.func.id == 'abs'):
-            return None     # not an invocation of abs
+        if not (
+            isinstance(node, Call)
+            and isinstance(node.func, Name)
+            and node.func.id == "abs"
+        ):
+            return None  # not an invocation of abs
         if not isUpperBound and not isinstance(op, Eq):
-            return None     # lower bounds on abs value don't bound underlying quantity
+            return None  # lower bounds on abs value don't bound underlying quantity
         if const < 0:
-            self.inconsistencyError(node, f'absolute value cannot be negative')
+            self.inconsistencyError(node, f"absolute value cannot be negative")
         assert len(node.args) == 1
         arg = node.args[0]
         target = matchAtom(arg)
-        if target is not None:   # abs(QUANTITY) </= CONST
+        if target is not None:  # abs(QUANTITY) </= CONST
             return (-const, const, target)
-        elif isinstance(arg, BinOp) and isinstance(arg.op, (Add, Sub)):   # abs(X +/- Y) </= CONST
+        elif isinstance(arg, BinOp) and isinstance(arg.op, (Add, Sub)):
+            # abs(X +/- Y) </= CONST
             match = None
             slconst = self.matchConstant(arg.left)
             target = matchAtom(arg.right)
-            if (isinstance(slconst, (int, float))
-                and target is not None):   # abs(CONST +/- QUANTITY) </= CONST
+            if isinstance(slconst, (int, float)) and target is not None:
+                # abs(CONST +/- QUANTITY) </= CONST
                 match = slconst
             else:
                 srconst = self.matchConstant(arg.right)
                 target = matchAtom(arg.left)
-                if (isinstance(srconst, (int, float))
-                    and target is not None):    # abs(QUANTITY +/- CONST) </= CONST
+                if isinstance(srconst, (int, float)) and target is not None:
+                    # abs(QUANTITY +/- CONST) </= CONST
                     match = srconst
             if match is not None:
-                if isinstance(arg.op, Add):    # abs(QUANTITY + CONST) </= CONST
+                if isinstance(arg.op, Add):  # abs(QUANTITY + CONST) </= CONST
                     return (-const - match, const - match, target)
-                else:   # abs(QUANTITY - CONST) </= CONST
+                else:  # abs(QUANTITY - CONST) </= CONST
                     return (-const + match, const + match, target)
         return None
 
     def matchConstant(self, node):
         """Match constant values, i.e. values known prior to sampling."""
         value = self.matchValue(node)
         return None if needsSampling(value) else value
@@ -187,12 +227,12 @@
     def matchValue(self, node):
         """Match any expression which can be evaluated, returning its value.
 
         This method could have undesirable side-effects, but conditions in
         requirements should not have side-effects to begin with.
         """
         try:
-            code = compile(Expression(node), '<internal>', 'eval')
+            code = compile(Expression(node), "<internal>", "eval")
             value = eval(code, dict(self.namespace))
         except Exception:
             return None
         return value
```

