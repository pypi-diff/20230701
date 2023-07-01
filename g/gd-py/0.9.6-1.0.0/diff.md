# Comparing `tmp/gd.py-0.9.6.tar.gz` & `tmp/gd_py-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gd.py-0.9.6.tar", last modified: Fri Oct  4 17:12:50 2019, max compression
+gzip compressed data, was "gd_py-1.0.0.tar", max compression
```

## Comparing `gd.py-0.9.6.tar` & `gd_py-1.0.0.tar`

### file list

```diff
@@ -1,69 +1,130 @@
-drwxrwxrwx   0        0        0        0 2019-10-04 17:12:38.000000 gd.py-0.9.6/
-drwxrwxrwx   0        0        0        0 2019-10-04 17:12:38.000000 gd.py-0.9.6/gd/
-drwxrwxrwx   0        0        0        0 2019-10-04 17:12:40.000000 gd.py-0.9.6/gd/api/
--rw-rw-rw-   0        0        0       31 2019-08-25 19:04:20.000000 gd.py-0.9.6/gd/api/__init__.py
-drwxrwxrwx   0        0        0        0 2019-10-04 17:12:40.000000 gd.py-0.9.6/gd/events/
--rw-rw-rw-   0        0        0       33 2019-09-07 21:37:02.000000 gd.py-0.9.6/gd/events/main.py
--rw-rw-rw-   0        0        0       33 2019-09-28 14:34:32.000000 gd.py-0.9.6/gd/events/runner.py
-drwxrwxrwx   0        0        0        0 2019-10-04 17:12:40.000000 gd.py-0.9.6/gd/graphics/
-drwxrwxrwx   0        0        0        0 2019-10-04 17:12:40.000000 gd.py-0.9.6/gd/graphics/resources/
--rw-rw-rw-   0        0        0   743605 2019-07-23 17:02:32.000000 gd.py-0.9.6/gd/graphics/resources/GJ_GameSheet02-uhd.plist
--rw-rw-rw-   0        0        0  3149933 2019-07-23 17:02:32.000000 gd.py-0.9.6/gd/graphics/resources/GJ_GameSheet02-uhd.png
--rw-rw-rw-   0        0        0       33 2019-09-16 19:57:56.000000 gd.py-0.9.6/gd/graphics/__init__.py
--rw-rw-rw-   0        0        0    11176 2019-09-22 16:21:28.000000 gd.py-0.9.6/gd/graphics/generator.py
--rw-rw-rw-   0        0        0     1683 2019-09-01 17:03:24.000000 gd.py-0.9.6/gd/graphics/sprite.py
--rw-rw-rw-   0        0        0     1308 2019-08-29 16:06:18.000000 gd.py-0.9.6/gd/graphics/testing.py
-drwxrwxrwx   0        0        0        0 2019-10-04 17:12:40.000000 gd.py-0.9.6/gd/utils/
-drwxrwxrwx   0        0        0        0 2019-10-04 17:12:40.000000 gd.py-0.9.6/gd/utils/crypto/
--rw-rw-rw-   0        0        0      146 2019-08-06 10:22:44.000000 gd.py-0.9.6/gd/utils/crypto/__init__.py
--rw-rw-rw-   0        0        0     6106 2019-09-21 10:47:52.000000 gd.py-0.9.6/gd/utils/crypto/coders.py
--rw-rw-rw-   0        0        0      964 2019-09-15 11:40:46.000000 gd.py-0.9.6/gd/utils/crypto/xor_cipher.py
--rw-rw-rw-   0        0        0     1031 2019-09-28 12:57:44.000000 gd.py-0.9.6/gd/utils/__init__.py
--rw-rw-rw-   0        0        0     5632 2019-10-04 13:30:36.000000 gd.py-0.9.6/gd/utils/_async.py
--rw-rw-rw-   0        0        0     4673 2019-09-28 14:16:58.000000 gd.py-0.9.6/gd/utils/captcha_solver.py
--rw-rw-rw-   0        0        0     3058 2019-09-13 18:49:12.000000 gd.py-0.9.6/gd/utils/converter.py
--rw-rw-rw-   0        0        0     7493 2019-09-28 12:56:34.000000 gd.py-0.9.6/gd/utils/enums.py
--rw-rw-rw-   0        0        0     7875 2019-09-06 16:30:32.000000 gd.py-0.9.6/gd/utils/filters.py
--rw-rw-rw-   0        0        0     8012 2019-09-22 16:27:34.000000 gd.py-0.9.6/gd/utils/gdpaginator.py
--rw-rw-rw-   0        0        0    10364 2019-09-29 18:37:46.000000 gd.py-0.9.6/gd/utils/http_request.py
--rw-rw-rw-   0        0        0     3213 2019-09-06 16:18:02.000000 gd.py-0.9.6/gd/utils/indexer.py
--rw-rw-rw-   0        0        0      808 2019-08-31 15:41:48.000000 gd.py-0.9.6/gd/utils/mapper.py
--rw-rw-rw-   0        0        0    18380 2019-09-15 08:44:36.000000 gd.py-0.9.6/gd/utils/params.py
--rw-rw-rw-   0        0        0     2059 2019-09-15 12:03:06.000000 gd.py-0.9.6/gd/utils/routes.py
--rw-rw-rw-   0        0        0     1161 2019-09-28 14:16:36.000000 gd.py-0.9.6/gd/utils/save_parser.py
--rw-rw-rw-   0        0        0     1522 2019-09-21 10:47:52.000000 gd.py-0.9.6/gd/utils/search_utils.py
--rw-rw-rw-   0        0        0    14240 2019-09-22 16:29:54.000000 gd.py-0.9.6/gd/utils/tasks.py
--rw-rw-rw-   0        0        0     3648 2019-10-04 16:34:24.000000 gd.py-0.9.6/gd/utils/wrap_tools.py
--rw-rw-rw-   0        0        0     3488 2019-10-04 16:09:56.000000 gd.py-0.9.6/gd/__init__.py
--rw-rw-rw-   0        0        0     1789 2019-09-29 07:13:16.000000 gd.py-0.9.6/gd/__main__.py
--rw-rw-rw-   0        0        0     1302 2019-09-22 16:01:42.000000 gd.py-0.9.6/gd/_jokes.py
--rw-rw-rw-   0        0        0     1519 2019-09-22 16:05:26.000000 gd.py-0.9.6/gd/abstractentity.py
--rw-rw-rw-   0        0        0    12023 2019-09-15 08:50:48.000000 gd.py-0.9.6/gd/abstractuser.py
--rw-rw-rw-   0        0        0    10495 2019-09-27 17:53:22.000000 gd.py-0.9.6/gd/classconverter.py
--rw-rw-rw-   0        0        0    27797 2019-10-04 16:03:52.000000 gd.py-0.9.6/gd/client.py
--rw-rw-rw-   0        0        0     3724 2019-09-22 16:10:32.000000 gd.py-0.9.6/gd/colors.py
--rw-rw-rw-   0        0        0     4466 2019-09-26 09:40:24.000000 gd.py-0.9.6/gd/comment.py
--rw-rw-rw-   0        0        0     4455 2019-09-22 16:20:40.000000 gd.py-0.9.6/gd/errors.py
--rw-rw-rw-   0        0        0     2415 2019-09-05 16:59:16.000000 gd.py-0.9.6/gd/friend_request.py
--rw-rw-rw-   0        0        0     2370 2019-09-01 14:26:14.000000 gd.py-0.9.6/gd/iconset.py
--rw-rw-rw-   0        0        0    15445 2019-09-22 16:23:40.000000 gd.py-0.9.6/gd/level.py
--rw-rw-rw-   0        0        0     2876 2019-09-14 17:49:20.000000 gd.py-0.9.6/gd/level_packs.py
--rw-rw-rw-   0        0        0     2306 2019-09-05 16:59:36.000000 gd.py-0.9.6/gd/message.py
--rw-rw-rw-   0        0        0    39328 2019-09-27 17:25:48.000000 gd.py-0.9.6/gd/session.py
--rw-rw-rw-   0        0        0     1927 2019-09-15 11:42:22.000000 gd.py-0.9.6/gd/song.py
--rw-rw-rw-   0        0        0      661 2019-09-13 18:14:58.000000 gd.py-0.9.6/gd/unreguser.py
--rw-rw-rw-   0        0        0     5463 2019-09-16 20:00:06.000000 gd.py-0.9.6/gd/user.py
-drwxrwxrwx   0        0        0        0 2019-10-04 17:12:38.000000 gd.py-0.9.6/gd.py.egg-info/
--rw-rw-rw-   0        0        0     5283 2019-10-04 17:12:38.000000 gd.py-0.9.6/gd.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1190 2019-10-04 17:12:38.000000 gd.py-0.9.6/gd.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-10-04 17:12:38.000000 gd.py-0.9.6/gd.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2019-10-04 17:12:38.000000 gd.py-0.9.6/gd.py.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       88 2019-10-04 17:12:38.000000 gd.py-0.9.6/gd.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        3 2019-10-04 17:12:38.000000 gd.py-0.9.6/gd.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1064 2019-08-03 10:29:24.000000 gd.py-0.9.6/LICENSE
--rw-rw-rw-   0        0        0       91 2019-08-29 17:05:08.000000 gd.py-0.9.6/MANIFEST.in
--rw-rw-rw-   0        0        0     3587 2019-09-28 08:43:50.000000 gd.py-0.9.6/README.rst
--rw-rw-rw-   0        0        0       28 2019-09-07 22:21:00.000000 gd.py-0.9.6/requirements.txt
--rw-rw-rw-   0        0        0     1821 2019-09-16 19:25:28.000000 gd.py-0.9.6/setup.py
--rw-rw-rw-   0        0        0     5283 2019-10-04 17:12:52.000000 gd.py-0.9.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2019-10-04 17:12:52.000000 gd.py-0.9.6/setup.cfg
+-rw-r--r--   0        0        0     1092 2023-07-01 14:13:53.282007 gd_py-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3625 2023-07-01 14:13:53.282007 gd_py-1.0.0/README.md
+-rw-r--r--   0        0        0      122 2023-07-01 14:13:53.282007 gd_py-1.0.0/_gd/__init__.py
+-rw-r--r--   0        0        0     1888 2023-07-01 14:13:53.282007 gd_py-1.0.0/build.py
+-rw-r--r--   0        0        0     6026 2023-07-01 14:13:53.282007 gd_py-1.0.0/gd/__init__.py
+-rw-r--r--   0        0        0       94 2023-07-01 14:13:53.282007 gd_py-1.0.0/gd/__main__.py
+-rw-r--r--   0        0        0     3508 2023-07-01 14:13:53.282007 gd_py-1.0.0/gd/api/__init__.py
+-rw-r--r--   0        0        0    20476 2023-07-01 14:13:53.282007 gd_py-1.0.0/gd/api/color_channels.py
+-rw-r--r--   0        0        0      118 2023-07-01 14:13:53.282007 gd_py-1.0.0/gd/api/database/__init__.py
+-rw-r--r--   0        0        0     1005 2023-07-01 14:13:53.282007 gd_py-1.0.0/gd/api/database/common.py
+-rw-r--r--   0        0        0    11755 2023-07-01 14:13:53.282007 gd_py-1.0.0/gd/api/database/completed.py
+-rw-r--r--   0        0        0    41285 2023-07-01 14:13:53.282007 gd_py-1.0.0/gd/api/database/database.py
+-rw-r--r--   0        0        0    11021 2023-07-01 14:13:53.282007 gd_py-1.0.0/gd/api/database/statistics.py
+-rw-r--r--   0        0        0    37042 2023-07-01 14:13:53.282007 gd_py-1.0.0/gd/api/database/storage.py
+-rw-r--r--   0        0        0    25126 2023-07-01 14:13:53.286007 gd_py-1.0.0/gd/api/database/unlock_values.py
+-rw-r--r--   0        0        0     7381 2023-07-01 14:13:53.286007 gd_py-1.0.0/gd/api/database/values.py
+-rw-r--r--   0        0        0    76749 2023-07-01 14:13:53.286007 gd_py-1.0.0/gd/api/database/variables.py
+-rw-r--r--   0        0        0     8305 2023-07-01 14:13:53.286007 gd_py-1.0.0/gd/api/editor.py
+-rw-r--r--   0        0        0     1608 2023-07-01 14:13:53.286007 gd_py-1.0.0/gd/api/folder.py
+-rw-r--r--   0        0        0     2772 2023-07-01 14:13:53.286007 gd_py-1.0.0/gd/api/guidelines.py
+-rw-r--r--   0        0        0    19482 2023-07-01 14:13:53.286007 gd_py-1.0.0/gd/api/header.py
+-rw-r--r--   0        0        0     4727 2023-07-01 14:13:53.286007 gd_py-1.0.0/gd/api/hsv.py
+-rw-r--r--   0        0        0    40647 2023-07-01 14:13:53.286007 gd_py-1.0.0/gd/api/levels.py
+-rw-r--r--   0        0        0     2172 2023-07-01 14:13:53.286007 gd_py-1.0.0/gd/api/like.py
+-rw-r--r--   0        0        0   160291 2023-07-01 14:13:53.286007 gd_py-1.0.0/gd/api/objects.py
+-rw-r--r--   0        0        0     6064 2023-07-01 14:13:53.286007 gd_py-1.0.0/gd/api/recording.py
+-rw-r--r--   0        0        0     9065 2023-07-01 14:13:53.286007 gd_py-1.0.0/gd/api/rewards.py
+-rw-r--r--   0        0        0     6040 2023-07-01 14:13:53.286007 gd_py-1.0.0/gd/api/save_manager.py
+-rw-r--r--   0        0        0     7059 2023-07-01 14:13:53.286007 gd_py-1.0.0/gd/api/songs.py
+-rw-r--r--   0        0        0     4614 2023-07-01 14:13:53.286007 gd_py-1.0.0/gd/artist.py
+-rw-r--r--   0        0        0    66226 2023-07-01 14:13:53.286007 gd_py-1.0.0/gd/assets/glow_sheet.json
+-rw-r--r--   0        0        0  1900170 2023-07-01 14:13:53.298007 gd_py-1.0.0/gd/assets/glow_sheet.png
+-rw-r--r--   0        0        0   160373 2023-07-01 14:13:53.298007 gd_py-1.0.0/gd/assets/icon_sheet.json
+-rw-r--r--   0        0        0  3264685 2023-07-01 14:13:53.318007 gd_py-1.0.0/gd/assets/icon_sheet.png
+-rw-r--r--   0        0        0    45605 2023-07-01 14:13:53.318007 gd_py-1.0.0/gd/assets/robot_animation_sheet.json
+-rw-r--r--   0        0        0    18591 2023-07-01 14:13:53.318007 gd_py-1.0.0/gd/assets/spider_animation_sheet.json
+-rw-r--r--   0        0        0      995 2023-07-01 14:13:53.286007 gd_py-1.0.0/gd/assets.py
+-rw-r--r--   0        0        0     1144 2023-07-01 14:13:53.318007 gd_py-1.0.0/gd/asyncio.py
+-rw-r--r--   0        0        0     5756 2023-07-01 14:13:53.318007 gd_py-1.0.0/gd/binary.py
+-rw-r--r--   0        0        0     1820 2023-07-01 14:13:53.318007 gd_py-1.0.0/gd/binary_constants.py
+-rw-r--r--   0        0        0     5908 2023-07-01 14:13:53.318007 gd_py-1.0.0/gd/binary_utils.py
+-rw-r--r--   0        0        0     1508 2023-07-01 14:13:53.318007 gd_py-1.0.0/gd/capacity.py
+-rw-r--r--   0        0        0    60667 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/client.py
+-rw-r--r--   0        0        0     4348 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/color.py
+-rw-r--r--   0        0        0     8884 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/comments.py
+-rw-r--r--   0        0        0     3119 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/constants.py
+-rw-r--r--   0        0        0     1318 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/converter.py
+-rw-r--r--   0        0        0      553 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/credentials.py
+-rw-r--r--   0        0        0     8787 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/date_time.py
+-rw-r--r--   0        0        0     2276 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/decorators.py
+-rw-r--r--   0        0        0     3295 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/difficulty_parameters.py
+-rw-r--r--   0        0        0    10568 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/encoding.py
+-rw-r--r--   0        0        0     2933 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/entity.py
+-rw-r--r--   0        0        0    33138 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/enums.py
+-rw-r--r--   0        0        0     2981 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/errors.py
+-rw-r--r--   0        0        0      667 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/events/__init__.py
+-rw-r--r--   0        0        0     1900 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/events/controller.py
+-rw-r--r--   0        0        0    12922 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/events/listeners.py
+-rw-r--r--   0        0        0    20660 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/filters.py
+-rw-r--r--   0        0        0     5146 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/friend_request.py
+-rw-r--r--   0        0        0    81644 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/http.py
+-rw-r--r--   0        0        0     1015 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/image/__init__.py
+-rw-r--r--   0        0        0     2592 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/image/animation.py
+-rw-r--r--   0        0        0     7066 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/image/converters.py
+-rw-r--r--   0        0        0     8430 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/image/factory.py
+-rw-r--r--   0        0        0     8047 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/image/geometry.py
+-rw-r--r--   0        0        0     6666 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/image/icon.py
+-rw-r--r--   0        0        0     1808 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/image/layer.py
+-rw-r--r--   0        0        0     2684 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/image/sheet.py
+-rw-r--r--   0        0        0     1993 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/image/sprite.py
+-rw-r--r--   0        0        0    22336 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/level.py
+-rw-r--r--   0        0        0     5942 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/level_packs.py
+-rw-r--r--   0        0        0      582 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/main.py
+-rw-r--r--   0        0        0     2213 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/memory/__init__.py
+-rw-r--r--   0        0        0     6052 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/memory/arrays.py
+-rw-r--r--   0        0        0     7047 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/memory/base.py
+-rw-r--r--   0        0        0     7675 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/memory/cocos.py
+-rw-r--r--   0        0        0      347 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/memory/constants.py
+-rw-r--r--   0        0        0    16432 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/memory/data.py
+-rw-r--r--   0        0        0     2916 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/memory/fields.py
+-rw-r--r--   0        0        0    34268 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/memory/gd.py
+-rw-r--r--   0        0        0     7801 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/memory/internal/__init__.py
+-rw-r--r--   0        0        0     9735 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/memory/internal/darwin.py
+-rw-r--r--   0        0        0     2460 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/memory/internal/utils.py
+-rw-r--r--   0        0        0    11754 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/memory/internal/windows.py
+-rw-r--r--   0        0        0     3670 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/memory/pointers.py
+-rw-r--r--   0        0        0      822 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/memory/special.py
+-rw-r--r--   0        0        0    19614 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/memory/state.py
+-rw-r--r--   0        0        0     5389 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/memory/strings.py
+-rw-r--r--   0        0        0      347 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/memory/utils.py
+-rw-r--r--   0        0        0     5411 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/message.py
+-rw-r--r--   0        0        0    95374 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/models.py
+-rw-r--r--   0        0        0     2301 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/models_constants.py
+-rw-r--r--   0        0        0    16226 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/models_utils.py
+-rw-r--r--   0        0        0      674 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/named_dicts.py
+-rw-r--r--   0        0        0     4974 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/newgrounds.py
+-rw-r--r--   0        0        0    11796 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/official_levels.py
+-rw-r--r--   0        0        0     3280 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/official_songs.py
+-rw-r--r--   0        0        0     4367 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/password.py
+-rw-r--r--   0        0        0     2509 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/platform.py
+-rw-r--r--   0        0        0     8284 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/plist.py
+-rw-r--r--   0        0        0     1491 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/progress.py
+-rw-r--r--   0        0        0        0 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/py.typed
+-rw-r--r--   0        0        0     3271 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/rewards.py
+-rw-r--r--   0        0        0      908 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/robtop.py
+-rw-r--r--   0        0        0      927 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/run_iterables.py
+-rw-r--r--   0        0        0     1103 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/server/__init__.py
+-rw-r--r--   0        0        0      583 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/server/artists.py
+-rw-r--r--   0        0        0      627 2023-07-01 14:13:53.322007 gd_py-1.0.0/gd/server/authentication.py
+-rw-r--r--   0        0        0      179 2023-07-01 14:13:53.326007 gd_py-1.0.0/gd/server/constants.py
+-rw-r--r--   0        0        0      378 2023-07-01 14:13:53.326007 gd_py-1.0.0/gd/server/core.py
+-rw-r--r--   0        0        0     1287 2023-07-01 14:13:53.326007 gd_py-1.0.0/gd/server/dependencies.py
+-rw-r--r--   0        0        0      936 2023-07-01 14:13:53.326007 gd_py-1.0.0/gd/server/errors.py
+-rw-r--r--   0        0        0     2336 2023-07-01 14:13:53.326007 gd_py-1.0.0/gd/server/newgrounds.py
+-rw-r--r--   0        0        0      834 2023-07-01 14:13:53.326007 gd_py-1.0.0/gd/server/songs.py
+-rw-r--r--   0        0        0     2044 2023-07-01 14:13:53.326007 gd_py-1.0.0/gd/server/tokens.py
+-rw-r--r--   0        0        0     4503 2023-07-01 14:13:53.326007 gd_py-1.0.0/gd/server/users.py
+-rw-r--r--   0        0        0     2030 2023-07-01 14:13:53.326007 gd_py-1.0.0/gd/server/utils.py
+-rw-r--r--   0        0        0    24572 2023-07-01 14:13:53.326007 gd_py-1.0.0/gd/session.py
+-rw-r--r--   0        0        0     8872 2023-07-01 14:13:53.326007 gd_py-1.0.0/gd/song.py
+-rw-r--r--   0        0        0      197 2023-07-01 14:13:53.326007 gd_py-1.0.0/gd/string_constants.py
+-rw-r--r--   0        0        0     3198 2023-07-01 14:13:53.326007 gd_py-1.0.0/gd/string_utils.py
+-rw-r--r--   0        0        0    10923 2023-07-01 14:13:53.326007 gd_py-1.0.0/gd/tasks.py
+-rw-r--r--   0        0        0      674 2023-07-01 14:13:53.326007 gd_py-1.0.0/gd/timer.py
+-rw-r--r--   0        0        0      784 2023-07-01 14:13:53.326007 gd_py-1.0.0/gd/typing.py
+-rw-r--r--   0        0        0    32942 2023-07-01 14:13:53.326007 gd_py-1.0.0/gd/users.py
+-rw-r--r--   0        0        0      199 2023-07-01 14:13:53.326007 gd_py-1.0.0/gd/version.py
+-rw-r--r--   0        0        0     4034 2023-07-01 14:13:53.326007 gd_py-1.0.0/gd/versions.py
+-rw-r--r--   0        0        0     4676 2023-07-01 14:13:53.326007 gd_py-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5528 1970-01-01 00:00:00.000000 gd_py-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gd.py-0.9.6/LICENSE` & `gd_py-1.0.0/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019 NeKitDS
+Copyright (c) 2019-present, Nikita Tikhonov (nekitdev)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

