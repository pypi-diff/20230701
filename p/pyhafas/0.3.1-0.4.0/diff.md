# Comparing `tmp/pyhafas-0.3.1.tar.gz` & `tmp/pyhafas-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhafas-0.3.1.tar", last modified: Wed Mar 29 17:45:02 2023, max compression
+gzip compressed data, was "pyhafas-0.4.0.tar", last modified: Sat Jul  1 19:32:02 2023, max compression
```

## Comparing `pyhafas-0.3.1.tar` & `pyhafas-0.4.0.tar`

### file list

```diff
@@ -1,152 +1,222 @@
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.761224 pyhafas-0.3.1/
--rw-r--r--   0 n0emis    (1000) users      (100)     1099 2020-06-29 08:20:43.000000 pyhafas-0.3.1/LICENSE
--rw-r--r--   0 n0emis    (1000) users      (100)      317 2020-11-15 18:33:56.000000 pyhafas-0.3.1/MANIFEST.in
--rw-r--r--   0 n0emis    (1000) users      (100)     2803 2023-03-29 17:45:02.761224 pyhafas-0.3.1/PKG-INFO
--rw-r--r--   0 n0emis    (1000) users      (100)     2075 2020-11-15 18:33:56.000000 pyhafas-0.3.1/README.md
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.738224 pyhafas-0.3.1/docs/
--rw-r--r--   0 n0emis    (1000) users      (100)      634 2020-01-21 19:45:23.000000 pyhafas-0.3.1/docs/Makefile
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.731224 pyhafas-0.3.1/docs/_static/
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.731224 pyhafas-0.3.1/docs/_static/usage/
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.738224 pyhafas-0.3.1/docs/_static/usage/images/
--rw-r--r--   0 n0emis    (1000) users      (100)   620978 2020-11-15 18:33:56.000000 pyhafas-0.3.1/docs/_static/usage/images/examples_3_journeys_map.jpg
--rw-r--r--   0 n0emis    (1000) users      (100)     1029 2023-03-29 17:34:48.000000 pyhafas-0.3.1/docs/changelog.rst
--rw-r--r--   0 n0emis    (1000) users      (100)     2312 2023-03-29 17:34:00.000000 pyhafas-0.3.1/docs/conf.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.740224 pyhafas-0.3.1/docs/development/
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.732224 pyhafas-0.3.1/docs/development/api/
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.740224 pyhafas-0.3.1/docs/development/api/profiles/
--rw-r--r--   0 n0emis    (1000) users      (100)     1793 2020-11-15 18:33:56.000000 pyhafas-0.3.1/docs/development/api/profiles/base.rst
--rw-r--r--   0 n0emis    (1000) users      (100)      272 2020-11-15 18:33:56.000000 pyhafas-0.3.1/docs/development/api/profiles/db.rst
--rw-r--r--   0 n0emis    (1000) users      (100)     1728 2020-11-15 18:33:56.000000 pyhafas-0.3.1/docs/development/api/profiles/interfaces.rst
--rw-r--r--   0 n0emis    (1000) users      (100)      275 2020-11-15 18:33:56.000000 pyhafas-0.3.1/docs/development/api/profiles/vsn.rst
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.741224 pyhafas-0.3.1/docs/development/api/types/
--rw-r--r--   0 n0emis    (1000) users      (100)      128 2020-11-15 18:33:56.000000 pyhafas-0.3.1/docs/development/api/types/hafas_response.rst
--rw-r--r--   0 n0emis    (1000) users      (100)      155 2020-11-15 18:33:56.000000 pyhafas-0.3.1/docs/development/api/types/station_board_request.rst
--rw-r--r--   0 n0emis    (1000) users      (100)      161 2020-11-15 18:33:56.000000 pyhafas-0.3.1/docs/development/api.rst
--rw-r--r--   0 n0emis    (1000) users      (100)     2097 2020-11-15 18:33:56.000000 pyhafas-0.3.1/docs/development/code_structure.rst
--rw-r--r--   0 n0emis    (1000) users      (100)     1246 2020-11-15 18:33:56.000000 pyhafas-0.3.1/docs/development/introduction.rst
--rw-r--r--   0 n0emis    (1000) users      (100)     3047 2020-11-15 18:33:56.000000 pyhafas-0.3.1/docs/development/profiles.rst
--rw-r--r--   0 n0emis    (1000) users      (100)     1027 2020-11-15 18:33:56.000000 pyhafas-0.3.1/docs/glossary.rst
--rw-r--r--   0 n0emis    (1000) users      (100)     1546 2020-11-15 18:33:56.000000 pyhafas-0.3.1/docs/index.rst
--rw-r--r--   0 n0emis    (1000) users      (100)      795 2020-01-21 19:45:23.000000 pyhafas-0.3.1/docs/make.bat
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.742224 pyhafas-0.3.1/docs/usage/
--rw-r--r--   0 n0emis    (1000) users      (100)      252 2020-11-15 18:33:56.000000 pyhafas-0.3.1/docs/usage/client.rst
--rw-r--r--   0 n0emis    (1000) users      (100)     7692 2020-11-15 18:33:56.000000 pyhafas-0.3.1/docs/usage/examples.rst
--rw-r--r--   0 n0emis    (1000) users      (100)      236 2020-11-15 18:33:56.000000 pyhafas-0.3.1/docs/usage/exceptions.rst
--rw-r--r--   0 n0emis    (1000) users      (100)      491 2020-11-15 18:33:56.000000 pyhafas-0.3.1/docs/usage/fptf.rst
--rw-r--r--   0 n0emis    (1000) users      (100)     2338 2020-11-15 18:33:56.000000 pyhafas-0.3.1/docs/usage/get_started.rst
--rw-r--r--   0 n0emis    (1000) users      (100)     2013 2021-12-31 16:20:50.000000 pyhafas-0.3.1/docs/usage/profiles.rst
--rw-r--r--   0 n0emis    (1000) users      (100)     1773 2022-11-20 17:33:12.000000 pyhafas-0.3.1/example.py
--rw-r--r--   0 n0emis    (1000) users      (100)     1099 2021-12-31 16:20:50.000000 pyhafas-0.3.1/example_rejseplanen.py
--rw-r--r--   0 n0emis    (1000) users      (100)      541 2020-04-07 18:58:26.000000 pyhafas-0.3.1/generateSalt.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.742224 pyhafas-0.3.1/pyhafas/
--rw-r--r--   0 n0emis    (1000) users      (100)      358 2020-07-22 19:48:07.000000 pyhafas-0.3.1/pyhafas/__init__.py
--rw-r--r--   0 n0emis    (1000) users      (100)    10761 2022-01-01 02:50:20.000000 pyhafas-0.3.1/pyhafas/client.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.744224 pyhafas-0.3.1/pyhafas/profile/
--rw-r--r--   0 n0emis    (1000) users      (100)      169 2021-12-31 16:20:50.000000 pyhafas-0.3.1/pyhafas/profile/__init__.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.744224 pyhafas-0.3.1/pyhafas/profile/base/
--rw-r--r--   0 n0emis    (1000) users      (100)     1645 2023-03-29 17:31:39.000000 pyhafas-0.3.1/pyhafas/profile/base/__init__.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.745224 pyhafas-0.3.1/pyhafas/profile/base/helper/
--rw-r--r--   0 n0emis    (1000) users      (100)        0 2020-07-22 19:48:07.000000 pyhafas-0.3.1/pyhafas/profile/base/helper/__init__.py
--rw-r--r--   0 n0emis    (1000) users      (100)     2984 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pyhafas/profile/base/helper/date_time.py
--rw-r--r--   0 n0emis    (1000) users      (100)     1690 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pyhafas/profile/base/helper/format_products_filter.py
--rw-r--r--   0 n0emis    (1000) users      (100)     6380 2021-12-31 16:20:50.000000 pyhafas-0.3.1/pyhafas/profile/base/helper/parse_leg.py
--rw-r--r--   0 n0emis    (1000) users      (100)     1978 2021-12-31 16:20:50.000000 pyhafas-0.3.1/pyhafas/profile/base/helper/parse_lid.py
--rw-r--r--   0 n0emis    (1000) users      (100)     2645 2022-11-20 15:37:51.000000 pyhafas-0.3.1/pyhafas/profile/base/helper/request.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.746224 pyhafas-0.3.1/pyhafas/profile/base/mappings/
--rw-r--r--   0 n0emis    (1000) users      (100)        0 2020-07-22 19:48:07.000000 pyhafas-0.3.1/pyhafas/profile/base/mappings/__init__.py
--rw-r--r--   0 n0emis    (1000) users      (100)      994 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pyhafas/profile/base/mappings/error_codes.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.747224 pyhafas-0.3.1/pyhafas/profile/base/requests/
--rw-r--r--   0 n0emis    (1000) users      (100)        0 2020-07-22 19:48:07.000000 pyhafas-0.3.1/pyhafas/profile/base/requests/__init__.py
--rw-r--r--   0 n0emis    (1000) users      (100)     1353 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pyhafas/profile/base/requests/journey.py
--rw-r--r--   0 n0emis    (1000) users      (100)     5437 2022-01-01 02:50:20.000000 pyhafas-0.3.1/pyhafas/profile/base/requests/journeys.py
--rw-r--r--   0 n0emis    (1000) users      (100)     1752 2021-12-31 16:20:50.000000 pyhafas-0.3.1/pyhafas/profile/base/requests/location.py
--rw-r--r--   0 n0emis    (1000) users      (100)     4451 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pyhafas/profile/base/requests/station_board.py
--rw-r--r--   0 n0emis    (1000) users      (100)     1100 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pyhafas/profile/base/requests/trip.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.747224 pyhafas-0.3.1/pyhafas/profile/db/
--rw-r--r--   0 n0emis    (1000) users      (100)     1415 2022-01-01 02:50:20.000000 pyhafas-0.3.1/pyhafas/profile/db/__init__.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.747224 pyhafas-0.3.1/pyhafas/profile/interfaces/
--rw-r--r--   0 n0emis    (1000) users      (100)     3371 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pyhafas/profile/interfaces/__init__.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.748224 pyhafas-0.3.1/pyhafas/profile/interfaces/helper/
--rw-r--r--   0 n0emis    (1000) users      (100)        0 2020-07-22 19:48:07.000000 pyhafas-0.3.1/pyhafas/profile/interfaces/helper/__init__.py
--rw-r--r--   0 n0emis    (1000) users      (100)     1544 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pyhafas/profile/interfaces/helper/date_time.py
--rw-r--r--   0 n0emis    (1000) users      (100)      394 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pyhafas/profile/interfaces/helper/format_products_filter.py
--rw-r--r--   0 n0emis    (1000) users      (100)     1399 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pyhafas/profile/interfaces/helper/parse_leg.py
--rw-r--r--   0 n0emis    (1000) users      (100)      950 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pyhafas/profile/interfaces/helper/parse_lid.py
--rw-r--r--   0 n0emis    (1000) users      (100)     1355 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pyhafas/profile/interfaces/helper/request.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.749224 pyhafas-0.3.1/pyhafas/profile/interfaces/mappings/
--rw-r--r--   0 n0emis    (1000) users      (100)        0 2020-07-22 19:48:07.000000 pyhafas-0.3.1/pyhafas/profile/interfaces/mappings/__init__.py
--rw-r--r--   0 n0emis    (1000) users      (100)      246 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pyhafas/profile/interfaces/mappings/error_codes.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.750224 pyhafas-0.3.1/pyhafas/profile/interfaces/requests/
--rw-r--r--   0 n0emis    (1000) users      (100)        0 2020-07-22 19:48:07.000000 pyhafas-0.3.1/pyhafas/profile/interfaces/requests/__init__.py
--rw-r--r--   0 n0emis    (1000) users      (100)      703 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pyhafas/profile/interfaces/requests/journey.py
--rw-r--r--   0 n0emis    (1000) users      (100)     2263 2022-01-01 02:50:20.000000 pyhafas-0.3.1/pyhafas/profile/interfaces/requests/journeys.py
--rw-r--r--   0 n0emis    (1000) users      (100)      825 2021-12-31 16:20:50.000000 pyhafas-0.3.1/pyhafas/profile/interfaces/requests/location.py
--rw-r--r--   0 n0emis    (1000) users      (100)     1717 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pyhafas/profile/interfaces/requests/station_board.py
--rw-r--r--   0 n0emis    (1000) users      (100)      645 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pyhafas/profile/interfaces/requests/trip.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.750224 pyhafas-0.3.1/pyhafas/profile/rkrp/
--rw-r--r--   0 n0emis    (1000) users      (100)     1726 2021-12-31 16:20:50.000000 pyhafas-0.3.1/pyhafas/profile/rkrp/__init__.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.751224 pyhafas-0.3.1/pyhafas/profile/vsn/
--rw-r--r--   0 n0emis    (1000) users      (100)     1509 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pyhafas/profile/vsn/__init__.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.751224 pyhafas-0.3.1/pyhafas/profile/vsn/requests/
--rw-r--r--   0 n0emis    (1000) users      (100)        0 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pyhafas/profile/vsn/requests/__init__.py
--rw-r--r--   0 n0emis    (1000) users      (100)      796 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pyhafas/profile/vsn/requests/journey.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.752224 pyhafas-0.3.1/pyhafas/types/
--rw-r--r--   0 n0emis    (1000) users      (100)        0 2020-07-22 19:48:07.000000 pyhafas-0.3.1/pyhafas/types/__init__.py
--rw-r--r--   0 n0emis    (1000) users      (100)      908 2020-07-22 19:48:07.000000 pyhafas-0.3.1/pyhafas/types/exceptions.py
--rw-r--r--   0 n0emis    (1000) users      (100)    13697 2021-12-31 16:20:50.000000 pyhafas-0.3.1/pyhafas/types/fptf.py
--rw-r--r--   0 n0emis    (1000) users      (100)     2522 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pyhafas/types/hafas_response.py
--rw-r--r--   0 n0emis    (1000) users      (100)      265 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pyhafas/types/station_board_request.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.743224 pyhafas-0.3.1/pyhafas.egg-info/
--rw-r--r--   0 n0emis    (1000) users      (100)     2803 2023-03-29 17:45:02.000000 pyhafas-0.3.1/pyhafas.egg-info/PKG-INFO
--rw-r--r--   0 n0emis    (1000) users      (100)     3801 2023-03-29 17:45:02.000000 pyhafas-0.3.1/pyhafas.egg-info/SOURCES.txt
--rw-r--r--   0 n0emis    (1000) users      (100)        1 2023-03-29 17:45:02.000000 pyhafas-0.3.1/pyhafas.egg-info/dependency_links.txt
--rw-r--r--   0 n0emis    (1000) users      (100)       27 2023-03-29 17:45:02.000000 pyhafas-0.3.1/pyhafas.egg-info/requires.txt
--rw-r--r--   0 n0emis    (1000) users      (100)        8 2023-03-29 17:45:02.000000 pyhafas-0.3.1/pyhafas.egg-info/top_level.txt
--rw-r--r--   0 n0emis    (1000) users      (100)        1 2020-01-21 19:26:53.000000 pyhafas-0.3.1/pyhafas.egg-info/zip-safe
--rw-r--r--   0 n0emis    (1000) users      (100)       89 2020-11-15 18:33:56.000000 pyhafas-0.3.1/pytest.ini
--rw-r--r--   0 n0emis    (1000) users      (100)      152 2020-11-15 18:33:56.000000 pyhafas-0.3.1/requirements.txt
--rw-r--r--   0 n0emis    (1000) users      (100)       38 2023-03-29 17:45:02.761224 pyhafas-0.3.1/setup.cfg
--rw-r--r--   0 n0emis    (1000) users      (100)     1347 2023-03-29 17:33:14.000000 pyhafas-0.3.1/setup.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.753224 pyhafas-0.3.1/tests/
--rw-r--r--   0 n0emis    (1000) users      (100)       44 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/__init__.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.753224 pyhafas-0.3.1/tests/base/
--rw-r--r--   0 n0emis    (1000) users      (100)        0 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/base/__init__.py
--rw-r--r--   0 n0emis    (1000) users      (100)      916 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/base/products_filter_test.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.753224 pyhafas-0.3.1/tests/db/
--rw-r--r--   0 n0emis    (1000) users      (100)        0 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/db/__init__.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.756224 pyhafas-0.3.1/tests/db/parsing/
--rw-r--r--   0 n0emis    (1000) users      (100)        0 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/db/parsing/__init__.py
--rw-r--r--   0 n0emis    (1000) users      (100)    10793 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/db/parsing/departures_raw.json
--rw-r--r--   0 n0emis    (1000) users      (100)     1122 2021-12-31 16:20:50.000000 pyhafas-0.3.1/tests/db/parsing/departures_test.py
--rw-r--r--   0 n0emis    (1000) users      (100)     8751 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/db/parsing/journey_raw.json
--rw-r--r--   0 n0emis    (1000) users      (100)     3147 2021-12-31 16:20:50.000000 pyhafas-0.3.1/tests/db/parsing/journey_test.py
--rw-r--r--   0 n0emis    (1000) users      (100)     9011 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/db/parsing/journeys_raw.json
--rw-r--r--   0 n0emis    (1000) users      (100)     3112 2021-12-31 16:20:50.000000 pyhafas-0.3.1/tests/db/parsing/journeys_test.py
--rw-r--r--   0 n0emis    (1000) users      (100)     3518 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/db/parsing/locations_raw.json
--rw-r--r--   0 n0emis    (1000) users      (100)      969 2021-12-31 16:20:50.000000 pyhafas-0.3.1/tests/db/parsing/locations_test.py
--rw-r--r--   0 n0emis    (1000) users      (100)    12733 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/db/parsing/trip_raw.json
--rw-r--r--   0 n0emis    (1000) users      (100)    15711 2021-12-31 16:20:50.000000 pyhafas-0.3.1/tests/db/parsing/trip_test.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.758224 pyhafas-0.3.1/tests/db/request/
--rw-r--r--   0 n0emis    (1000) users      (100)        0 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/db/request/__init__.py
--rw-r--r--   0 n0emis    (1000) users      (100)      312 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/db/request/arrivals_test.py
--rw-r--r--   0 n0emis    (1000) users      (100)      320 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/db/request/departures_test.py
--rw-r--r--   0 n0emis    (1000) users      (100)      415 2021-12-31 16:20:50.000000 pyhafas-0.3.1/tests/db/request/journey_test.py
--rw-r--r--   0 n0emis    (1000) users      (100)      362 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/db/request/journeys_test.py
--rw-r--r--   0 n0emis    (1000) users      (100)      233 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/db/request/locations_test.py
--rw-r--r--   0 n0emis    (1000) users      (100)      387 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/types.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.758224 pyhafas-0.3.1/tests/vsn/
--rw-r--r--   0 n0emis    (1000) users      (100)        0 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/vsn/__init__.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.759224 pyhafas-0.3.1/tests/vsn/parsing/
--rw-r--r--   0 n0emis    (1000) users      (100)        0 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/vsn/parsing/__init__.py
--rw-r--r--   0 n0emis    (1000) users      (100)     6258 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/vsn/parsing/departures_raw.json
--rw-r--r--   0 n0emis    (1000) users      (100)     1123 2021-12-31 16:20:50.000000 pyhafas-0.3.1/tests/vsn/parsing/departures_test.py
--rw-r--r--   0 n0emis    (1000) users      (100)    15666 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/vsn/parsing/journeys_raw.json
--rw-r--r--   0 n0emis    (1000) users      (100)     4596 2021-12-31 16:20:50.000000 pyhafas-0.3.1/tests/vsn/parsing/journeys_test.py
-drwxr-xr-x   0 n0emis    (1000) users      (100)        0 2023-03-29 17:45:02.761224 pyhafas-0.3.1/tests/vsn/request/
--rw-r--r--   0 n0emis    (1000) users      (100)        0 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/vsn/request/__init__.py
--rw-r--r--   0 n0emis    (1000) users      (100)      307 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/vsn/request/arrivals_test.py
--rw-r--r--   0 n0emis    (1000) users      (100)      315 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/vsn/request/departures_test.py
--rw-r--r--   0 n0emis    (1000) users      (100)      415 2021-12-31 16:20:50.000000 pyhafas-0.3.1/tests/vsn/request/journey_test.py
--rw-r--r--   0 n0emis    (1000) users      (100)      369 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/vsn/request/journeys_test.py
--rw-r--r--   0 n0emis    (1000) users      (100)      241 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tests/vsn/request/locations_test.py
--rw-r--r--   0 n0emis    (1000) users      (100)      444 2020-11-15 18:33:56.000000 pyhafas-0.3.1/tox.ini
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.497029 pyhafas-0.4.0/
+-rw-r--r--   0 leona     (1000) users      (100)     1099 2021-02-20 21:54:48.000000 pyhafas-0.4.0/LICENSE
+-rw-r--r--   0 leona     (1000) users      (100)      317 2021-02-20 21:54:48.000000 pyhafas-0.4.0/MANIFEST.in
+-rw-r--r--   0 leona     (1000) users      (100)     2827 2023-07-01 19:32:02.497029 pyhafas-0.4.0/PKG-INFO
+-rw-r--r--   0 leona     (1000) users      (100)     2075 2021-02-20 21:54:48.000000 pyhafas-0.4.0/README.md
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.435036 pyhafas-0.4.0/docs/
+-rw-r--r--   0 leona     (1000) users      (100)      634 2021-02-20 21:56:12.000000 pyhafas-0.4.0/docs/Makefile
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.421038 pyhafas-0.4.0/docs/_build/
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.421038 pyhafas-0.4.0/docs/_build/html/
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.435036 pyhafas-0.4.0/docs/_build/html/_images/
+-rw-r--r--   0 leona     (1000) users      (100)   620978 2021-02-20 21:56:12.000000 pyhafas-0.4.0/docs/_build/html/_images/examples_3_journeys_map.jpg
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.421038 pyhafas-0.4.0/docs/_build/html/_static/
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.421038 pyhafas-0.4.0/docs/_build/html/_static/usage/
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.439036 pyhafas-0.4.0/docs/_build/html/_static/usage/images/
+-rw-r--r--   0 leona     (1000) users      (100)   620978 2021-02-20 21:56:13.000000 pyhafas-0.4.0/docs/_build/html/_static/usage/images/examples_3_journeys_map.jpg
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.422037 pyhafas-0.4.0/docs/_static/
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.422037 pyhafas-0.4.0/docs/_static/usage/
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.441035 pyhafas-0.4.0/docs/_static/usage/images/
+-rw-r--r--   0 leona     (1000) users      (100)   620978 2021-02-20 21:56:13.000000 pyhafas-0.4.0/docs/_static/usage/images/examples_3_journeys_map.jpg
+-rw-r--r--   0 leona     (1000) users      (100)     1237 2023-07-01 19:26:02.000000 pyhafas-0.4.0/docs/changelog.rst
+-rw-r--r--   0 leona     (1000) users      (100)     2312 2023-07-01 18:29:13.000000 pyhafas-0.4.0/docs/conf.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.445035 pyhafas-0.4.0/docs/development/
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.422037 pyhafas-0.4.0/docs/development/api/
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.448035 pyhafas-0.4.0/docs/development/api/profiles/
+-rw-r--r--   0 leona     (1000) users      (100)     1793 2021-02-20 21:56:13.000000 pyhafas-0.4.0/docs/development/api/profiles/base.rst
+-rw-r--r--   0 leona     (1000) users      (100)      272 2021-02-20 21:56:13.000000 pyhafas-0.4.0/docs/development/api/profiles/db.rst
+-rw-r--r--   0 leona     (1000) users      (100)     1728 2021-02-20 21:56:13.000000 pyhafas-0.4.0/docs/development/api/profiles/interfaces.rst
+-rw-r--r--   0 leona     (1000) users      (100)      275 2021-02-20 21:56:13.000000 pyhafas-0.4.0/docs/development/api/profiles/vsn.rst
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.449034 pyhafas-0.4.0/docs/development/api/types/
+-rw-r--r--   0 leona     (1000) users      (100)      128 2021-02-20 21:56:13.000000 pyhafas-0.4.0/docs/development/api/types/hafas_response.rst
+-rw-r--r--   0 leona     (1000) users      (100)      155 2021-02-20 21:56:13.000000 pyhafas-0.4.0/docs/development/api/types/station_board_request.rst
+-rw-r--r--   0 leona     (1000) users      (100)      161 2021-02-20 21:56:13.000000 pyhafas-0.4.0/docs/development/api.rst
+-rw-r--r--   0 leona     (1000) users      (100)     2097 2021-02-20 21:56:13.000000 pyhafas-0.4.0/docs/development/code_structure.rst
+-rw-r--r--   0 leona     (1000) users      (100)     1246 2021-02-20 21:56:13.000000 pyhafas-0.4.0/docs/development/introduction.rst
+-rw-r--r--   0 leona     (1000) users      (100)     3047 2021-02-20 21:56:13.000000 pyhafas-0.4.0/docs/development/profiles.rst
+-rw-r--r--   0 leona     (1000) users      (100)     1027 2021-02-20 21:56:12.000000 pyhafas-0.4.0/docs/glossary.rst
+-rw-r--r--   0 leona     (1000) users      (100)     1546 2021-02-20 21:56:12.000000 pyhafas-0.4.0/docs/index.rst
+-rw-r--r--   0 leona     (1000) users      (100)      795 2021-02-20 21:56:12.000000 pyhafas-0.4.0/docs/make.bat
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.451034 pyhafas-0.4.0/docs/usage/
+-rw-r--r--   0 leona     (1000) users      (100)      252 2021-02-20 21:56:13.000000 pyhafas-0.4.0/docs/usage/client.rst
+-rw-r--r--   0 leona     (1000) users      (100)     7692 2023-07-01 18:29:13.000000 pyhafas-0.4.0/docs/usage/examples.rst
+-rw-r--r--   0 leona     (1000) users      (100)      236 2021-02-20 21:56:13.000000 pyhafas-0.4.0/docs/usage/exceptions.rst
+-rw-r--r--   0 leona     (1000) users      (100)      491 2021-02-20 21:56:13.000000 pyhafas-0.4.0/docs/usage/fptf.rst
+-rw-r--r--   0 leona     (1000) users      (100)     2353 2023-05-23 23:21:57.000000 pyhafas-0.4.0/docs/usage/get_started.rst
+-rw-r--r--   0 leona     (1000) users      (100)     2658 2023-06-13 18:37:38.000000 pyhafas-0.4.0/docs/usage/profiles.rst
+-rw-r--r--   0 leona     (1000) users      (100)     1031 2023-07-01 18:29:13.000000 pyhafas-0.4.0/example.py
+-rw-r--r--   0 leona     (1000) users      (100)     1193 2023-07-01 19:22:41.000000 pyhafas-0.4.0/exampleDB.py
+-rw-r--r--   0 leona     (1000) users      (100)     1099 2023-07-01 18:29:13.000000 pyhafas-0.4.0/example_rejseplanen.py
+-rw-r--r--   0 leona     (1000) users      (100)      541 2023-07-01 18:29:13.000000 pyhafas-0.4.0/generateSalt.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.452034 pyhafas-0.4.0/pyhafas/
+-rw-r--r--   0 leona     (1000) users      (100)      358 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/__init__.py
+-rw-r--r--   0 leona     (1000) users      (100)    10761 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/client.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.454034 pyhafas-0.4.0/pyhafas/profile/
+-rw-r--r--   0 leona     (1000) users      (100)      197 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/__init__.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.454034 pyhafas-0.4.0/pyhafas/profile/base/
+-rw-r--r--   0 leona     (1000) users      (100)     1751 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/base/__init__.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.456034 pyhafas-0.4.0/pyhafas/profile/base/helper/
+-rw-r--r--   0 leona     (1000) users      (100)        0 2021-02-20 21:56:13.000000 pyhafas-0.4.0/pyhafas/profile/base/helper/__init__.py
+-rw-r--r--   0 leona     (1000) users      (100)     2984 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/base/helper/date_time.py
+-rw-r--r--   0 leona     (1000) users      (100)     1690 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/base/helper/format_products_filter.py
+-rw-r--r--   0 leona     (1000) users      (100)     6754 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/base/helper/parse_leg.py
+-rw-r--r--   0 leona     (1000) users      (100)     1978 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/base/helper/parse_lid.py
+-rw-r--r--   0 leona     (1000) users      (100)      977 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/base/helper/parse_remark.py
+-rw-r--r--   0 leona     (1000) users      (100)     3250 2023-07-01 19:22:41.000000 pyhafas-0.4.0/pyhafas/profile/base/helper/request.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.456034 pyhafas-0.4.0/pyhafas/profile/base/mappings/
+-rw-r--r--   0 leona     (1000) users      (100)        0 2021-02-20 21:56:13.000000 pyhafas-0.4.0/pyhafas/profile/base/mappings/__init__.py
+-rw-r--r--   0 leona     (1000) users      (100)      994 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/base/mappings/error_codes.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.458033 pyhafas-0.4.0/pyhafas/profile/base/requests/
+-rw-r--r--   0 leona     (1000) users      (100)        0 2021-02-20 21:56:13.000000 pyhafas-0.4.0/pyhafas/profile/base/requests/__init__.py
+-rw-r--r--   0 leona     (1000) users      (100)     1353 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/base/requests/journey.py
+-rw-r--r--   0 leona     (1000) users      (100)     5437 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/base/requests/journeys.py
+-rw-r--r--   0 leona     (1000) users      (100)     1752 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/base/requests/location.py
+-rw-r--r--   0 leona     (1000) users      (100)     4451 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/base/requests/station_board.py
+-rw-r--r--   0 leona     (1000) users      (100)     1100 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/base/requests/trip.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.458033 pyhafas-0.4.0/pyhafas/profile/db/
+-rw-r--r--   0 leona     (1000) users      (100)     1415 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/db/__init__.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.458033 pyhafas-0.4.0/pyhafas/profile/interfaces/
+-rw-r--r--   0 leona     (1000) users      (100)     3493 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/interfaces/__init__.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.460033 pyhafas-0.4.0/pyhafas/profile/interfaces/helper/
+-rw-r--r--   0 leona     (1000) users      (100)        0 2021-02-20 21:56:13.000000 pyhafas-0.4.0/pyhafas/profile/interfaces/helper/__init__.py
+-rw-r--r--   0 leona     (1000) users      (100)     1544 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/interfaces/helper/date_time.py
+-rw-r--r--   0 leona     (1000) users      (100)      394 2021-02-20 21:56:13.000000 pyhafas-0.4.0/pyhafas/profile/interfaces/helper/format_products_filter.py
+-rw-r--r--   0 leona     (1000) users      (100)     1399 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/interfaces/helper/parse_leg.py
+-rw-r--r--   0 leona     (1000) users      (100)      950 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/interfaces/helper/parse_lid.py
+-rw-r--r--   0 leona     (1000) users      (100)      468 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/interfaces/helper/parse_remark.py
+-rw-r--r--   0 leona     (1000) users      (100)     1355 2021-02-20 21:56:13.000000 pyhafas-0.4.0/pyhafas/profile/interfaces/helper/request.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.461033 pyhafas-0.4.0/pyhafas/profile/interfaces/mappings/
+-rw-r--r--   0 leona     (1000) users      (100)        0 2021-02-20 21:56:13.000000 pyhafas-0.4.0/pyhafas/profile/interfaces/mappings/__init__.py
+-rw-r--r--   0 leona     (1000) users      (100)      246 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/interfaces/mappings/error_codes.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.463033 pyhafas-0.4.0/pyhafas/profile/interfaces/requests/
+-rw-r--r--   0 leona     (1000) users      (100)        0 2021-02-20 21:56:13.000000 pyhafas-0.4.0/pyhafas/profile/interfaces/requests/__init__.py
+-rw-r--r--   0 leona     (1000) users      (100)      703 2021-02-20 21:56:13.000000 pyhafas-0.4.0/pyhafas/profile/interfaces/requests/journey.py
+-rw-r--r--   0 leona     (1000) users      (100)     2263 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/interfaces/requests/journeys.py
+-rw-r--r--   0 leona     (1000) users      (100)      825 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/interfaces/requests/location.py
+-rw-r--r--   0 leona     (1000) users      (100)     1717 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/interfaces/requests/station_board.py
+-rw-r--r--   0 leona     (1000) users      (100)      645 2021-02-20 21:56:13.000000 pyhafas-0.4.0/pyhafas/profile/interfaces/requests/trip.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.463033 pyhafas-0.4.0/pyhafas/profile/kvb/
+-rw-r--r--   0 leona     (1000) users      (100)     1181 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/kvb/__init__.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.464033 pyhafas-0.4.0/pyhafas/profile/kvb/requests/
+-rw-r--r--   0 leona     (1000) users      (100)        0 2023-06-13 18:37:38.000000 pyhafas-0.4.0/pyhafas/profile/kvb/requests/__init__.py
+-rw-r--r--   0 leona     (1000) users      (100)     1484 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/kvb/requests/journey.py
+-rw-r--r--   0 leona     (1000) users      (100)      930 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/kvb/requests/journeys.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.464033 pyhafas-0.4.0/pyhafas/profile/rkrp/
+-rw-r--r--   0 leona     (1000) users      (100)     1726 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/rkrp/__init__.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.464033 pyhafas-0.4.0/pyhafas/profile/vsn/
+-rw-r--r--   0 leona     (1000) users      (100)     1509 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/vsn/__init__.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.464033 pyhafas-0.4.0/pyhafas/profile/vsn/requests/
+-rw-r--r--   0 leona     (1000) users      (100)        0 2021-02-20 21:56:13.000000 pyhafas-0.4.0/pyhafas/profile/vsn/requests/__init__.py
+-rw-r--r--   0 leona     (1000) users      (100)      796 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/profile/vsn/requests/journey.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.465033 pyhafas-0.4.0/pyhafas/types/
+-rw-r--r--   0 leona     (1000) users      (100)        0 2021-02-20 21:56:13.000000 pyhafas-0.4.0/pyhafas/types/__init__.py
+-rw-r--r--   0 leona     (1000) users      (100)      908 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/types/exceptions.py
+-rw-r--r--   0 leona     (1000) users      (100)    15546 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/types/fptf.py
+-rw-r--r--   0 leona     (1000) users      (100)     2522 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/types/hafas_response.py
+-rw-r--r--   0 leona     (1000) users      (100)      265 2023-07-01 18:29:13.000000 pyhafas-0.4.0/pyhafas/types/station_board_request.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.454034 pyhafas-0.4.0/pyhafas.egg-info/
+-rw-r--r--   0 leona     (1000) users      (100)     2827 2023-07-01 19:32:02.000000 pyhafas-0.4.0/pyhafas.egg-info/PKG-INFO
+-rw-r--r--   0 leona     (1000) users      (100)     6550 2023-07-01 19:32:02.000000 pyhafas-0.4.0/pyhafas.egg-info/SOURCES.txt
+-rw-r--r--   0 leona     (1000) users      (100)        1 2023-07-01 19:32:02.000000 pyhafas-0.4.0/pyhafas.egg-info/dependency_links.txt
+-rw-r--r--   0 leona     (1000) users      (100)       27 2023-07-01 19:32:02.000000 pyhafas-0.4.0/pyhafas.egg-info/requires.txt
+-rw-r--r--   0 leona     (1000) users      (100)        8 2023-07-01 19:32:02.000000 pyhafas-0.4.0/pyhafas.egg-info/top_level.txt
+-rw-r--r--   0 leona     (1000) users      (100)        1 2021-02-20 21:56:13.000000 pyhafas-0.4.0/pyhafas.egg-info/zip-safe
+-rw-r--r--   0 leona     (1000) users      (100)       89 2021-02-20 21:54:48.000000 pyhafas-0.4.0/pytest.ini
+-rw-r--r--   0 leona     (1000) users      (100)      152 2023-06-17 17:01:56.000000 pyhafas-0.4.0/requirements.txt
+-rw-r--r--   0 leona     (1000) users      (100)       38 2023-07-01 19:32:02.497029 pyhafas-0.4.0/setup.cfg
+-rw-r--r--   0 leona     (1000) users      (100)     1371 2023-07-01 19:24:00.000000 pyhafas-0.4.0/setup.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.466033 pyhafas-0.4.0/tests/
+-rw-r--r--   0 leona     (1000) users      (100)       44 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/__init__.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.468032 pyhafas-0.4.0/tests/__pycache__/
+-rw-r--r--   0 leona     (1000) users      (100)      189 2021-06-05 12:28:19.000000 pyhafas-0.4.0/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 leona     (1000) users      (100)      932 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/__pycache__/foo.cpython-38-pytest-6.0.1.pyc
+-rw-r--r--   0 leona     (1000) users      (100)      937 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/__pycache__/foo_test.cpython-38-pytest-6.0.1.pyc
+-rw-r--r--   0 leona     (1000) users      (100)      874 2021-06-05 12:28:20.000000 pyhafas-0.4.0/tests/__pycache__/types.cpython-38.pyc
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.469032 pyhafas-0.4.0/tests/base/
+-rw-r--r--   0 leona     (1000) users      (100)        0 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/base/__init__.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.470032 pyhafas-0.4.0/tests/base/__pycache__/
+-rw-r--r--   0 leona     (1000) users      (100)      143 2021-06-05 12:28:19.000000 pyhafas-0.4.0/tests/base/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 leona     (1000) users      (100)      941 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/base/__pycache__/foo_test.cpython-38-pytest-6.0.1.pyc
+-rw-r--r--   0 leona     (1000) users      (100)     1652 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/base/__pycache__/products_filter_test.cpython-38-pytest-6.0.1.pyc
+-rw-r--r--   0 leona     (1000) users      (100)      916 2023-07-01 18:29:13.000000 pyhafas-0.4.0/tests/base/products_filter_test.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.470032 pyhafas-0.4.0/tests/db/
+-rw-r--r--   0 leona     (1000) users      (100)        0 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/db/__init__.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.471032 pyhafas-0.4.0/tests/db/__pycache__/
+-rw-r--r--   0 leona     (1000) users      (100)      141 2021-06-05 12:28:20.000000 pyhafas-0.4.0/tests/db/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 leona     (1000) users      (100)     1965 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/db/__pycache__/departures_parsing_test.cpython-38-pytest-6.0.1.pyc
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.476031 pyhafas-0.4.0/tests/db/parsing/
+-rw-r--r--   0 leona     (1000) users      (100)        0 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/db/parsing/__init__.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.478031 pyhafas-0.4.0/tests/db/parsing/__pycache__/
+-rw-r--r--   0 leona     (1000) users      (100)      149 2021-06-05 12:28:20.000000 pyhafas-0.4.0/tests/db/parsing/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 leona     (1000) users      (100)     1945 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/db/parsing/__pycache__/departures_test.cpython-38-pytest-6.0.1.pyc
+-rw-r--r--   0 leona     (1000) users      (100)     2546 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/db/parsing/__pycache__/journey_test.cpython-38-pytest-6.0.1.pyc
+-rw-r--r--   0 leona     (1000) users      (100)     2534 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/db/parsing/__pycache__/journeys_test.cpython-38-pytest-6.0.1.pyc
+-rw-r--r--   0 leona     (1000) users      (100)     1606 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/db/parsing/__pycache__/locations_test.cpython-38-pytest-6.0.1.pyc
+-rw-r--r--   0 leona     (1000) users      (100)     5402 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/db/parsing/__pycache__/trip_test.cpython-38-pytest-6.0.1.pyc
+-rw-r--r--   0 leona     (1000) users      (100)    10793 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/db/parsing/departures_raw.json
+-rw-r--r--   0 leona     (1000) users      (100)     1122 2023-07-01 18:29:13.000000 pyhafas-0.4.0/tests/db/parsing/departures_test.py
+-rw-r--r--   0 leona     (1000) users      (100)     8751 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/db/parsing/journey_raw.json
+-rw-r--r--   0 leona     (1000) users      (100)     3943 2023-07-01 18:29:13.000000 pyhafas-0.4.0/tests/db/parsing/journey_test.py
+-rw-r--r--   0 leona     (1000) users      (100)     9011 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/db/parsing/journeys_raw.json
+-rw-r--r--   0 leona     (1000) users      (100)     4033 2023-07-01 18:29:13.000000 pyhafas-0.4.0/tests/db/parsing/journeys_test.py
+-rw-r--r--   0 leona     (1000) users      (100)     3518 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/db/parsing/locations_raw.json
+-rw-r--r--   0 leona     (1000) users      (100)      969 2023-07-01 18:29:13.000000 pyhafas-0.4.0/tests/db/parsing/locations_test.py
+-rw-r--r--   0 leona     (1000) users      (100)    12733 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/db/parsing/trip_raw.json
+-rw-r--r--   0 leona     (1000) users      (100)    17071 2023-07-01 18:29:13.000000 pyhafas-0.4.0/tests/db/parsing/trip_test.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.481031 pyhafas-0.4.0/tests/db/request/
+-rw-r--r--   0 leona     (1000) users      (100)        0 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/db/request/__init__.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.483031 pyhafas-0.4.0/tests/db/request/__pycache__/
+-rw-r--r--   0 leona     (1000) users      (100)      149 2021-06-05 12:28:20.000000 pyhafas-0.4.0/tests/db/request/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 leona     (1000) users      (100)     1097 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/db/request/__pycache__/arrivals_test.cpython-38-pytest-6.0.1.pyc
+-rw-r--r--   0 leona     (1000) users      (100)     1103 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/db/request/__pycache__/departures_test.cpython-38-pytest-6.0.1.pyc
+-rw-r--r--   0 leona     (1000) users      (100)     1117 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/db/request/__pycache__/journey_test.cpython-38-pytest-6.0.1.pyc
+-rw-r--r--   0 leona     (1000) users      (100)      867 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/db/request/__pycache__/journeys_test.cpython-38-pytest-6.0.1.pyc
+-rw-r--r--   0 leona     (1000) users      (100)     1045 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/db/request/__pycache__/locations_test.cpython-38-pytest-6.0.1.pyc
+-rw-r--r--   0 leona     (1000) users      (100)      312 2023-07-01 18:29:13.000000 pyhafas-0.4.0/tests/db/request/arrivals_test.py
+-rw-r--r--   0 leona     (1000) users      (100)      320 2023-07-01 18:29:13.000000 pyhafas-0.4.0/tests/db/request/departures_test.py
+-rw-r--r--   0 leona     (1000) users      (100)      415 2023-05-23 23:21:57.000000 pyhafas-0.4.0/tests/db/request/journey_test.py
+-rw-r--r--   0 leona     (1000) users      (100)      362 2023-07-01 18:29:13.000000 pyhafas-0.4.0/tests/db/request/journeys_test.py
+-rw-r--r--   0 leona     (1000) users      (100)      233 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/db/request/locations_test.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.484031 pyhafas-0.4.0/tests/kvb/
+-rw-r--r--   0 leona     (1000) users      (100)        0 2023-06-13 18:37:38.000000 pyhafas-0.4.0/tests/kvb/__init__.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.484031 pyhafas-0.4.0/tests/kvb/parsing/
+-rw-r--r--   0 leona     (1000) users      (100)        0 2023-06-13 18:37:38.000000 pyhafas-0.4.0/tests/kvb/parsing/__init__.py
+-rw-r--r--   0 leona     (1000) users      (100)    13082 2023-07-01 18:29:13.000000 pyhafas-0.4.0/tests/kvb/parsing/departures_raw.json
+-rw-r--r--   0 leona     (1000) users      (100)     1138 2023-07-01 18:29:13.000000 pyhafas-0.4.0/tests/kvb/parsing/departures_test.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.487030 pyhafas-0.4.0/tests/kvb/request/
+-rw-r--r--   0 leona     (1000) users      (100)        0 2023-06-13 18:37:38.000000 pyhafas-0.4.0/tests/kvb/request/__init__.py
+-rw-r--r--   0 leona     (1000) users      (100)      307 2023-07-01 18:29:13.000000 pyhafas-0.4.0/tests/kvb/request/arrivals_test.py
+-rw-r--r--   0 leona     (1000) users      (100)      315 2023-07-01 18:29:13.000000 pyhafas-0.4.0/tests/kvb/request/departures_test.py
+-rw-r--r--   0 leona     (1000) users      (100)      421 2023-06-13 18:37:38.000000 pyhafas-0.4.0/tests/kvb/request/journey_test.py
+-rw-r--r--   0 leona     (1000) users      (100)      369 2023-07-01 19:23:21.000000 pyhafas-0.4.0/tests/kvb/request/journeys_test.py
+-rw-r--r--   0 leona     (1000) users      (100)      227 2023-06-13 18:37:38.000000 pyhafas-0.4.0/tests/kvb/request/locations_test.py
+-rw-r--r--   0 leona     (1000) users      (100)      387 2023-07-01 18:29:13.000000 pyhafas-0.4.0/tests/types.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.487030 pyhafas-0.4.0/tests/vsn/
+-rw-r--r--   0 leona     (1000) users      (100)        0 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/vsn/__init__.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.488030 pyhafas-0.4.0/tests/vsn/__pycache__/
+-rw-r--r--   0 leona     (1000) users      (100)      142 2021-06-05 12:28:20.000000 pyhafas-0.4.0/tests/vsn/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 leona     (1000) users      (100)     1919 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/vsn/__pycache__/departures_parsing_test.cpython-38-pytest-6.0.1.pyc
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.490030 pyhafas-0.4.0/tests/vsn/parsing/
+-rw-r--r--   0 leona     (1000) users      (100)        0 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/vsn/parsing/__init__.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.492030 pyhafas-0.4.0/tests/vsn/parsing/__pycache__/
+-rw-r--r--   0 leona     (1000) users      (100)      150 2021-06-05 12:28:20.000000 pyhafas-0.4.0/tests/vsn/parsing/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 leona     (1000) users      (100)     1951 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/vsn/parsing/__pycache__/departures_test.cpython-38-pytest-6.0.1.pyc
+-rw-r--r--   0 leona     (1000) users      (100)     2659 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/vsn/parsing/__pycache__/journeys_test.cpython-38-pytest-6.0.1.pyc
+-rw-r--r--   0 leona     (1000) users      (100)     6258 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/vsn/parsing/departures_raw.json
+-rw-r--r--   0 leona     (1000) users      (100)     1123 2023-07-01 18:29:13.000000 pyhafas-0.4.0/tests/vsn/parsing/departures_test.py
+-rw-r--r--   0 leona     (1000) users      (100)    15666 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/vsn/parsing/journeys_raw.json
+-rw-r--r--   0 leona     (1000) users      (100)     5690 2023-07-01 18:29:13.000000 pyhafas-0.4.0/tests/vsn/parsing/journeys_test.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.494029 pyhafas-0.4.0/tests/vsn/request/
+-rw-r--r--   0 leona     (1000) users      (100)        0 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/vsn/request/__init__.py
+drwxr-xr-x   0 leona     (1000) users      (100)        0 2023-07-01 19:32:02.496029 pyhafas-0.4.0/tests/vsn/request/__pycache__/
+-rw-r--r--   0 leona     (1000) users      (100)      150 2021-06-05 12:28:20.000000 pyhafas-0.4.0/tests/vsn/request/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 leona     (1000) users      (100)      819 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/vsn/request/__pycache__/arrivals_test.cpython-38-pytest-6.0.1.pyc
+-rw-r--r--   0 leona     (1000) users      (100)      825 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/vsn/request/__pycache__/departures_test.cpython-38-pytest-6.0.1.pyc
+-rw-r--r--   0 leona     (1000) users      (100)     1095 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/vsn/request/__pycache__/journey_test.cpython-38-pytest-6.0.1.pyc
+-rw-r--r--   0 leona     (1000) users      (100)      874 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/vsn/request/__pycache__/journeys_test.cpython-38-pytest-6.0.1.pyc
+-rw-r--r--   0 leona     (1000) users      (100)     1053 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/vsn/request/__pycache__/locations_test.cpython-38-pytest-6.0.1.pyc
+-rw-r--r--   0 leona     (1000) users      (100)      307 2023-07-01 18:29:13.000000 pyhafas-0.4.0/tests/vsn/request/arrivals_test.py
+-rw-r--r--   0 leona     (1000) users      (100)      315 2023-07-01 18:29:13.000000 pyhafas-0.4.0/tests/vsn/request/departures_test.py
+-rw-r--r--   0 leona     (1000) users      (100)      415 2023-05-23 23:21:57.000000 pyhafas-0.4.0/tests/vsn/request/journey_test.py
+-rw-r--r--   0 leona     (1000) users      (100)      369 2023-07-01 18:29:13.000000 pyhafas-0.4.0/tests/vsn/request/journeys_test.py
+-rw-r--r--   0 leona     (1000) users      (100)      241 2021-02-20 21:56:13.000000 pyhafas-0.4.0/tests/vsn/request/locations_test.py
+-rw-r--r--   0 leona     (1000) users      (100)      444 2021-02-20 21:54:48.000000 pyhafas-0.4.0/tox.ini
```

### Comparing `pyhafas-0.3.1/LICENSE` & `pyhafas-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/PKG-INFO` & `pyhafas-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pyhafas
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python client for HAFAS public transport APIs
-Home-page: https://github.com/n0emis/pyhafas
-Download-URL: https://github.com/n0emis/pyhafas/releases
-Author: Simeon Keske, Leo Maroni
-Author-email: dev@n0emis.eu, hello@em0lar.de
+Home-page: https://github.com/FahrplanDatenGarten/pyhafas
+Download-URL: https://github.com/FahrplanDatenGarten/pyhafas/releases
+Author: Ember Keske, Leona Maroni
+Author-email: dev@n0emis.eu, dev@leona.is
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyhafas-0.3.1/README.md` & `pyhafas-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/docs/Makefile` & `pyhafas-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/docs/_static/usage/images/examples_3_journeys_map.jpg` & `pyhafas-0.4.0/docs/_build/html/_images/examples_3_journeys_map.jpg`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/docs/changelog.rst` & `pyhafas-0.4.0/docs/changelog.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 Changelog
 =========
 
 .. contents::
 
+v0.4.0
+------
+* [feature] Parse leg remarks
+* [feature] Add KVB Profile
+* [feature] Add optional retry parameter for requests. You might activate retries with the `activate_retry()` function on your profile
+
 v0.3.1
 ------
 * [BUG] Fix setting of default user agent
 
 v0.3.0
 ------
 * [FEATURE] Add timezone awareness to all datetime time objects
```

### Comparing `pyhafas-0.3.1/docs/conf.py` & `pyhafas-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/docs/development/api/profiles/base.rst` & `pyhafas-0.4.0/docs/development/api/profiles/base.rst`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/docs/development/api/profiles/interfaces.rst` & `pyhafas-0.4.0/docs/development/api/profiles/interfaces.rst`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/docs/development/code_structure.rst` & `pyhafas-0.4.0/docs/development/code_structure.rst`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/docs/development/introduction.rst` & `pyhafas-0.4.0/docs/development/introduction.rst`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/docs/development/profiles.rst` & `pyhafas-0.4.0/docs/development/profiles.rst`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/docs/glossary.rst` & `pyhafas-0.4.0/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/docs/index.rst` & `pyhafas-0.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/docs/make.bat` & `pyhafas-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/docs/usage/examples.rst` & `pyhafas-0.4.0/docs/usage/examples.rst`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/docs/usage/get_started.rst` & `pyhafas-0.4.0/docs/usage/get_started.rst`

 * *Files 4% similar despite different names*

```diff
@@ -33,24 +33,25 @@
 
 2. It searches for locations (stations) with the term "Berlin" and prints the result
 
 3. It searches for departing trains at Berlin Central Station. Every station is identified by an ID, which (in this case `8011160`) can be obtained by a `location`-request with pyhafas.
 
 .. code:: python
 
+  import datetime
   from pyhafas import HafasClient
   from pyhafas.profile import DBProfile
 
   client = HafasClient(DBProfile())
 
   print(client.locations("Berlin"))
 
   print(client.departures(
       station='8011160',
       date=datetime.datetime.now(),
-      max_journeys=5
+      max_trips=5
   ))
 
 What's next?
 ------------
 
 For a good start with pyHaFAS you should go on reading the documentation. Especially the pages :doc:`/usage/examples` and :doc:`profiles` are a good start.
```

### Comparing `pyhafas-0.3.1/docs/usage/profiles.rst` & `pyhafas-0.4.0/docs/usage/profiles.rst`

 * *Files 12% similar despite different names*

```diff
@@ -69,7 +69,34 @@
 ^^^^^^^^^^^^^^^^
 All available products specified above are enabled by default.
 
 Specialities
 ^^^^^^^^^^^^
 
 * The `max_trips` filter in station board (departures/arrival) requests seems not to work
+
+Kölner Verkehrsbetriebe (KVB)
+-----------------------------
+Usage
+^^^^^^
+.. code:: python
+
+  from pyhafas.profile import KVBProfile
+  client = HafasClient(KVBProfile())
+
+Available Products
+^^^^^^^^^^^^^^^^^^
+
+===================== ==================
+pyHaFAS Internal Name Example Train Type
+===================== ==================
+s-bahn                S
+stadtbahn             U
+bus                   BUS
+fernverkehr           ICE/ECE/IC/EC
+regionalverkehr       RE/IRE
+taxibus               Group Taxi
+===================== ==================
+
+Default Products
+^^^^^^^^^^^^^^^^
+All available products specified above are enabled by default.
```

### Comparing `pyhafas-0.3.1/example_rejseplanen.py` & `pyhafas-0.4.0/example_rejseplanen.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/generateSalt.py` & `pyhafas-0.4.0/generateSalt.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/client.py` & `pyhafas-0.4.0/pyhafas/client.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/base/__init__.py` & `pyhafas-0.4.0/pyhafas/profile/base/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Dict, List
 
 from pyhafas.profile.base.helper.date_time import BaseDateTimeHelper
 from pyhafas.profile.base.helper.format_products_filter import \
     BaseFormatProductsFilterHelper
 from pyhafas.profile.base.helper.parse_leg import BaseParseLegHelper
 from pyhafas.profile.base.helper.parse_lid import BaseParseLidHelper
+from pyhafas.profile.base.helper.parse_remark import BaseParseRemarkHelper
 from pyhafas.profile.base.helper.request import BaseRequestHelper
 from pyhafas.profile.base.requests.journey import BaseJourneyRequest
 from pyhafas.profile.base.requests.journeys import BaseJourneysRequest
 from pyhafas.profile.base.requests.location import BaseLocationRequest
 from pyhafas.profile.base.requests.station_board import BaseStationBoardRequest
 from pyhafas.profile.base.requests.trip import BaseTripRequest
 from pyhafas.profile.interfaces import ProfileInterface
@@ -16,14 +17,15 @@
 
 class BaseProfile(
         BaseRequestHelper,
         BaseFormatProductsFilterHelper,
         BaseParseLidHelper,
         BaseDateTimeHelper,
         BaseParseLegHelper,
+        BaseParseRemarkHelper,
         BaseLocationRequest,
         BaseJourneyRequest,
         BaseJourneysRequest,
         BaseStationBoardRequest,
         BaseTripRequest,
         ProfileInterface):
     """
```

### Comparing `pyhafas-0.3.1/pyhafas/profile/base/helper/date_time.py` & `pyhafas-0.4.0/pyhafas/profile/base/helper/date_time.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/base/helper/format_products_filter.py` & `pyhafas-0.4.0/pyhafas/profile/base/helper/format_products_filter.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/base/helper/parse_leg.py` & `pyhafas-0.4.0/pyhafas/profile/base/helper/parse_leg.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                 id=gis['ctx'],
                 origin=leg_origin,
                 destination=leg_destination,
                 departure=self.parse_datetime(departure['dTimeS'], date),
                 arrival=self.parse_datetime(arrival['aTimeS'], date),
                 mode=Mode.WALKING,
                 name=None,
-                distance=gis['dist'] if gis is not None else None
+                distance=gis.get('dist') if gis is not None else None
             )
         else:
             leg_stopovers: List[Stopover] = []
             if 'stopL' in journey:
                 for stopover in journey['stopL']:
                     leg_stopovers.append(
                         Stopover(
@@ -79,14 +79,16 @@
                                 stopover['aTimeR'],
                                 date) - self.parse_datetime(
                                 stopover['aTimeS'],
                                 date) if stopover.get('aTimeR') is not None else None,
                             arrival_platform=stopover.get(
                                 'aPlatfR',
                                 stopover.get('aPlatfS', stopover.get('aPltfR', stopover.get('aPltfS', {})).get('txt'))),
+                            remarks=[self.parse_remark(common['remL'][msg['remX']], common)
+                                     for msg in stopover.get('msgL', []) if msg.get('remX') is not None]
                         ))
 
             return Leg(
                 id=journey['jid'],
                 name=common['prodL'][journey['prodX']]['name'],
                 origin=leg_origin,
                 destination=leg_destination,
@@ -109,15 +111,17 @@
                     arrival['aTimeR'],
                     date) - self.parse_datetime(
                     arrival['aTimeS'],
                     date) if arrival.get('aTimeR') is not None else None,
                 arrival_platform=arrival.get(
                     'aPlatfR',
                     arrival.get('aPlatfS', arrival.get('aPltfR', arrival.get('aPltfS', {})).get('txt'))),
-                stopovers=leg_stopovers)
+                stopovers=leg_stopovers,
+                remarks=[self.parse_remark(common['remL'][msg['remX']], common)
+                         for msg in journey.get('msgL', {}) if msg.get('remX') is not None])
 
     def parse_legs(
             self: ProfileInterface,
             jny: dict,
             common: dict,
             date: datetime.date) -> List[Leg]:
         """
```

### Comparing `pyhafas-0.3.1/pyhafas/profile/base/helper/parse_lid.py` & `pyhafas-0.4.0/pyhafas/profile/base/helper/parse_lid.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/base/helper/request.py` & `pyhafas-0.4.0/pyhafas/profile/base/helper/request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import json
 from hashlib import md5
 from typing import Tuple
 
 import requests
+from requests.adapters import HTTPAdapter
+from urllib3.util.retry import Retry
 
 from pyhafas.profile import ProfileInterface
 from pyhafas.profile.base.mappings.error_codes import BaseErrorCodesMapping
 from pyhafas.profile.interfaces.helper.request import RequestHelperInterface
 from pyhafas.types.hafas_response import HafasResponse
 
 
 class BaseRequestHelper(RequestHelperInterface):
+    request_session = requests.session()
+
     def calculate_checksum(self: ProfileInterface, data: str) -> str:
         """
         Calculates the checksum of the request (required for most profiles)
 
         :param data: Complete body as string
         :return: Checksum for the request
         """
@@ -52,27 +56,41 @@
                 parameters.append(
                     'mic={}&mac={}'.format(
                         *self.calculate_mic_mac(data)))
             url += '?{}'.format('&'.join(parameters))
 
         return url
 
+    def activate_retry(self: ProfileInterface, retries: int = 4, backoff_factor: float = 1) -> None:
+        self.request_session = requests.Session()
+
+        retry = Retry(
+            total=retries,
+            read=retries,
+            connect=retries,
+            backoff_factor=backoff_factor,
+        )
+
+        adapter = HTTPAdapter(max_retries=retry)
+        self.request_session.mount("http://", adapter)
+        self.request_session.mount("https://", adapter)
+
     def request(self: ProfileInterface, body) -> HafasResponse:
         """
         Sends the request and does a basic parsing of the response and error handling
 
         :param body: Reqeust body as dict (without the `requestBody` of the profile)
         :return: HafasRespone object or Exception when HaFAS response returns an error
         """
         data = {
             'svcReqL': [body]
         }
         data.update(self.requestBody)
         data = json.dumps(data)
 
-        res = requests.post(
+        res = self.request_session.post(
             self.url_formatter(data),
             data=data,
             headers={
                 'User-Agent': self.userAgent,
                 'Content-Type': 'application/json'})
         return HafasResponse(res, BaseErrorCodesMapping)
```

### Comparing `pyhafas-0.3.1/pyhafas/profile/base/mappings/error_codes.py` & `pyhafas-0.4.0/pyhafas/profile/base/mappings/error_codes.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/base/requests/journey.py` & `pyhafas-0.4.0/pyhafas/profile/base/requests/journey.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/base/requests/journeys.py` & `pyhafas-0.4.0/pyhafas/profile/base/requests/journeys.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/base/requests/location.py` & `pyhafas-0.4.0/pyhafas/profile/base/requests/location.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/base/requests/station_board.py` & `pyhafas-0.4.0/pyhafas/profile/base/requests/station_board.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/base/requests/trip.py` & `pyhafas-0.4.0/pyhafas/profile/base/requests/trip.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/db/__init__.py` & `pyhafas-0.4.0/pyhafas/profile/db/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/interfaces/__init__.py` & `pyhafas-0.4.0/pyhafas/profile/interfaces/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pytz
 
 from pyhafas.profile.interfaces.helper.date_time import DateTimeHelperInterface
 from pyhafas.profile.interfaces.helper.format_products_filter import \
     FormatProductsFilterHelperInterface
 from pyhafas.profile.interfaces.helper.parse_leg import ParseLegHelperInterface
 from pyhafas.profile.interfaces.helper.parse_lid import ParseLidHelperInterface
+from pyhafas.profile.interfaces.helper.parse_remark import ParseRemarkHelperInterface
 from pyhafas.profile.interfaces.helper.request import RequestHelperInterface
 from pyhafas.profile.interfaces.requests.journey import JourneyRequestInterface
 from pyhafas.profile.interfaces.requests.journeys import \
     JourneysRequestInterface
 from pyhafas.profile.interfaces.requests.location import \
     LocationRequestInterface
 from pyhafas.profile.interfaces.requests.station_board import \
@@ -21,14 +22,15 @@
 
 class ProfileInterface(
         RequestHelperInterface,
         FormatProductsFilterHelperInterface,
         ParseLidHelperInterface,
         DateTimeHelperInterface,
         ParseLegHelperInterface,
+        ParseRemarkHelperInterface,
         LocationRequestInterface,
         JourneyRequestInterface,
         JourneysRequestInterface,
         StationBoardRequestInterface,
         TripRequestInterface,
         ABC):
     """
```

### Comparing `pyhafas-0.3.1/pyhafas/profile/interfaces/helper/date_time.py` & `pyhafas-0.4.0/pyhafas/profile/interfaces/helper/date_time.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/interfaces/helper/parse_leg.py` & `pyhafas-0.4.0/pyhafas/profile/interfaces/helper/parse_leg.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/interfaces/helper/parse_lid.py` & `pyhafas-0.4.0/pyhafas/profile/interfaces/helper/parse_lid.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/interfaces/helper/request.py` & `pyhafas-0.4.0/pyhafas/profile/interfaces/helper/request.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/interfaces/requests/journey.py` & `pyhafas-0.4.0/pyhafas/profile/interfaces/requests/journey.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/interfaces/requests/journeys.py` & `pyhafas-0.4.0/pyhafas/profile/interfaces/requests/journeys.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/interfaces/requests/location.py` & `pyhafas-0.4.0/pyhafas/profile/interfaces/requests/location.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/interfaces/requests/station_board.py` & `pyhafas-0.4.0/pyhafas/profile/interfaces/requests/station_board.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/interfaces/requests/trip.py` & `pyhafas-0.4.0/pyhafas/profile/interfaces/requests/trip.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/rkrp/__init__.py` & `pyhafas-0.4.0/pyhafas/profile/rkrp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/vsn/__init__.py` & `pyhafas-0.4.0/pyhafas/profile/vsn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/profile/vsn/requests/journey.py` & `pyhafas-0.4.0/pyhafas/profile/vsn/requests/journey.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/types/exceptions.py` & `pyhafas-0.4.0/pyhafas/types/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas/types/fptf.py` & `pyhafas-0.4.0/pyhafas/types/fptf.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,23 @@
     BICYCLE = 'bicycle'
     WALKING = 'walking'
 
     def __repr__(self):
         return '<%s.%s>' % (self.__class__.__name__, self.name)
 
 
-class Station:
+class FPTFObject:
+    def __repr__(self):
+        return "%s(%r)" % (self.__class__, self.__dict__)
+
+    def __eq__(self, other):
+        return self.__dict__ == other.__dict__
+
+
+class Station(FPTFObject):
     """
     FPTF `Station` object
 
     A station is a point where vehicles stop. It may be a larger building or just a small stop without special infrastructure.
 
     :ivar id: ID of the Station. Typically a number but as a string
     :vartype id: str
@@ -59,22 +67,58 @@
         """
         self.id: str = id
         self.lid: Optional[str] = lid
         self.name: Optional[str] = name
         self.latitude: Optional[float] = latitude
         self.longitude: Optional[float] = longitude
 
-    def __repr__(self):
-        return "%s(%r)" % (self.__class__, self.__dict__)
 
-    def __eq__(self, other):
-        return self.__dict__ == other.__dict__
+class Remark(FPTFObject):
+    """
+    A remark is a textual comment/information, usually added to a Stopover or Leg
 
+    :ivar remark_type: Type/Category of the remark. May have a different meaning depending on the network
+    :vartype remark_type: Optional[str]
+    :ivar code: Code of the remark. May have a different meaning depending on the network
+    :vartype code: Optional[str]
+    :ivar subject: Subject of the remark
+    :vartype subject: Optional[str]
+    :ivar text: Actual content of the remark
+    :vartype text: Optional[str]
+    :ivar priority: Priority of the remark, higher is better
+    :vartype priority: Optional[int]
+    :ivar trip_id: ID to a Trip added to this remark (e.g. a replacement train)
+    :vartype trip_id: Optional[str]
+    """
+    def __init__(
+            self,
+            remark_type: Optional[str] = None,
+            code: Optional[str] = None,
+            subject: Optional[str] = None,
+            text: Optional[str] = None,
+            priority: Optional[int] = None,
+            trip_id: Optional[str] = None):
+        """
 
-class Stopover:
+        :param remark_type: Type/Category of the remark. May have a different meaning depending on the network
+        :param code: Code of the remark. May have a different meaning depending on the network
+        :param subject: Subject of the remark
+        :param text: Actual content of the remark
+        :param priority: Priority of the remark, higher is better
+        :param trip_id: ID to a Trip added to this remark (e.g. a replacement train)
+        """
+        self.remark_type: Optional[str] = remark_type
+        self.code: Optional[str] = code
+        self.subject: Optional[str] = subject
+        self.text: Optional[str] = text
+        self.priority: Optional[int] = priority
+        self.trip_id: Optional[str] = trip_id
+
+
+class Stopover(FPTFObject):
     """
     FPTF `Stopover` object
 
     A stopover represents a vehicle stopping at a stop/station at a specific time.
 
     :ivar stop: Station where the vehicle is stopping
     :vartype stop: Station
@@ -88,55 +132,56 @@
     :vartype arrivalPlatform: Optional[str]
     :ivar departure: Planned departure date and time at the station (maybe `None`)
     :vartype departure: Optional[datetime.datetime]
     :ivar departureDelay: Departure delay at the station (maybe `None`)
     :vartype departureDelay: Optional[datetime.timedelta]
     :ivar departurePlatform: Real-time departure platform at the station (maybe `None`)
     :vartype departurePlatform: Optional[str]
+    :ivar remarks: (optional) List of remarks
+    :vartype remarks: List[Remark]
     """
 
     def __init__(
             self,
             stop: Station,
             cancelled: bool = False,
             arrival: Optional[datetime.datetime] = None,
             arrival_delay: Optional[datetime.timedelta] = None,
             arrival_platform: Optional[str] = None,
             departure: Optional[datetime.datetime] = None,
             departure_delay: Optional[datetime.timedelta] = None,
             departure_platform: Optional[str] = None,
+            remarks: Optional[List[Remark]] = None
     ):
         """
 
         :param stop: Station where the vehicle is stopping
         :param cancelled: (optional) Whether the stop is cancelled. Defaults to `False`
         :param arrival: (optional) Planned arrival date and time at the station. Defaults to `None`
         :param arrival_delay: (optional) Arrival delay at the station. Defaults to `None`
         :param arrival_platform: (optional) Real-time arrival platform at the station. Defaults to `None`
         :param departure: (optional) Planned departure date and time at the station. Defaults to `None`
         :param departure_delay: (optional) Departure delay at the station. Defaults to `None`
         :param departure_platform: (optional) Real-time departure platform at the station. Defaults to `None`
+        :param remarks: (optional) List of remarks. Defaults to `[]`
         """
         self.stop: Station = stop
         self.cancelled: bool = cancelled
         self.arrival: Optional[datetime.datetime] = arrival
         self.arrivalDelay: Optional[datetime.timedelta] = arrival_delay
         self.arrivalPlatform: Optional[str] = arrival_platform
         self.departure: Optional[datetime.datetime] = departure
         self.departureDelay: Optional[datetime.timedelta] = departure_delay
         self.departurePlatform: Optional[str] = departure_platform
+        if remarks is None:
+            remarks = []
+        self.remarks: List[Remark] = remarks
 
-    def __repr__(self):
-        return "%s(%r)" % (self.__class__, self.__dict__)
 
-    def __eq__(self, other):
-        return self.__dict__ == other.__dict__
-
-
-class Leg:
+class Leg(FPTFObject):
     """
     FPTF `Leg` object
 
     A leg or also named trip is most times part of a journey and defines a journey with only one specific vehicle from A to B.
 
     :ivar id: ID of the Leg
     :vartype id: str
@@ -162,14 +207,16 @@
     :vartype departurePlatform: Optional[str]
     :ivar arrivalDelay: Delay at the arrival station (maybe `None`)
     :vartype arrivalDelay: Optional[datetime.timedelta]
     :ivar arrivalPlatform: Real-time platform at the arrival station (maybe `None`)
     :vartype arrivalPlatform: Optional[str]
     :ivar stopovers: List of FPTF `Stopover` objects (maybe `None`)
     :vartype stopovers: Optional[List[Stopover]]
+    :ivar remarks: (optional) List of remarks
+    :vartype remarks: List[Remark]
     """
 
     def __init__(
             self,
             id: str,
             origin: Station,
             destination: Station,
@@ -179,15 +226,16 @@
             name: Optional[str] = None,
             cancelled: bool = False,
             distance: Optional[int] = None,
             departure_delay: Optional[datetime.timedelta] = None,
             departure_platform: Optional[str] = None,
             arrival_delay: Optional[datetime.timedelta] = None,
             arrival_platform: Optional[str] = None,
-            stopovers: Optional[List[Stopover]] = None
+            stopovers: Optional[List[Stopover]] = None,
+            remarks: Optional[List[Remark]] = None
     ):
         """
         FPTF `Leg` object
 
         :param id: Internal ID of the station
         :param origin: FPTF `Station` object of the origin station
         :param destination: FPTF `Station` object of the destination station
@@ -198,14 +246,15 @@
         :param cancelled: (optional) Whether the trip is cancelled. Defaults to False
         :param distance: (optional) Distance of the walk trip in meters. Defaults to None
         :param departure_delay: (optional) Delay at the departure station. Defaults to None
         :param departure_platform: (optional) Real-time platform at the departure station. Defaults to None
         :param arrival_delay: (optional) Delay at the arrival station. Defaults to None
         :param arrival_platform: (optional) Platform at the arrival station. Defaults to None
         :param stopovers: (optional) List of FPTF `Stopover` objects. Defaults to None
+        :param remarks: (optional) List of remarks. Defaults to `[]`
         """
         # Mandatory Variables
         self.id = id
         self.origin: Station = origin
         self.destination: Station = destination
         self.departure: datetime.datetime = departure
         self.arrival: datetime.datetime = arrival
@@ -216,23 +265,20 @@
         self.cancelled: bool = cancelled
         self.distance: Optional[int] = distance
         self.departureDelay: Optional[datetime.timedelta] = departure_delay
         self.departurePlatform: Optional[str] = departure_platform
         self.arrivalDelay: Optional[datetime.timedelta] = arrival_delay
         self.arrivalPlatform: Optional[str] = arrival_platform
         self.stopovers: Optional[List[Stopover]] = stopovers
+        if remarks is None:
+            remarks = []
+        self.remarks: List[Remark] = remarks
 
-    def __repr__(self):
-        return "%s(%r)" % (self.__class__, self.__dict__)
 
-    def __eq__(self, other):
-        return self.__dict__ == other.__dict__
-
-
-class Journey:
+class Journey(FPTFObject):
     """
     FPTF `Journey` object
 
     A journey is a computed set of directions to get from A to B at a specific time. It would typically be the result of a route planning algorithm.
 
     :ivar id: ID of the Journey
     :vartype id: str
@@ -259,22 +305,16 @@
         :param legs: (optional) Longitude coordinate of the station. Defaults to None
         """
         self.id: str = id
         self.date: Optional[datetime.date] = date
         self.duration: Optional[datetime.timedelta] = duration
         self.legs: Optional[List[Leg]] = legs
 
-    def __repr__(self):
-        return "%s(%r)" % (self.__class__, self.__dict__)
 
-    def __eq__(self, other):
-        return self.__dict__ == other.__dict__
-
-
-class StationBoardLeg:
+class StationBoardLeg(FPTFObject):
     """
     `StationBoardLeg` object
 
     Returned at Station Board-Requests. This requests do not have enough information for a FPTF `Leg` object.
     With the ID a `trip` request can be made to get detailed information about the trip
 
     :ivar id: ID of the Leg
@@ -322,13 +362,7 @@
         self.name: str = name
         self.direction: str = direction
         self.station: Station = station
         self.dateTime: datetime.datetime = date_time
         self.cancelled: bool = cancelled
         self.delay: Optional[datetime.timedelta] = delay
         self.platform: Optional[str] = platform
-
-    def __repr__(self):
-        return "%s(%r)" % (self.__class__, self.__dict__)
-
-    def __eq__(self, other):
-        return self.__dict__ == other.__dict__
```

### Comparing `pyhafas-0.3.1/pyhafas/types/hafas_response.py` & `pyhafas-0.4.0/pyhafas/types/hafas_response.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/pyhafas.egg-info/PKG-INFO` & `pyhafas-0.4.0/pyhafas.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pyhafas
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python client for HAFAS public transport APIs
-Home-page: https://github.com/n0emis/pyhafas
-Download-URL: https://github.com/n0emis/pyhafas/releases
-Author: Simeon Keske, Leo Maroni
-Author-email: dev@n0emis.eu, hello@em0lar.de
+Home-page: https://github.com/FahrplanDatenGarten/pyhafas
+Download-URL: https://github.com/FahrplanDatenGarten/pyhafas/releases
+Author: Ember Keske, Leona Maroni
+Author-email: dev@n0emis.eu, dev@leona.is
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyhafas-0.3.1/setup.py` & `pyhafas-0.4.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 
 if sys.argv[-1] == 'publish':
     os.system('python3 setup.py sdist upload')
     sys.exit()
 
 setup(
     name='pyhafas',
-    version='0.3.1',
+    version='0.4.0',
     description='Python client for HAFAS public transport APIs',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url='https://github.com/n0emis/pyhafas',
-    download_url='https://github.com/n0emis/pyhafas/releases',
-    author='Simeon Keske, Leo Maroni',
-    author_email='dev@n0emis.eu, hello@em0lar.de',
+    url='https://github.com/FahrplanDatenGarten/pyhafas',
+    download_url='https://github.com/FahrplanDatenGarten/pyhafas/releases',
+    author='Ember Keske, Leona Maroni',
+    author_email='dev@n0emis.eu, dev@leona.is',
     license='MIT',
     install_requires=['requests~=2.9',
                       'pytz>=2013.6'],
     packages=find_packages(include=['pyhafas', 'pyhafas.*']),
     zip_safe=True,
     classifiers=[
         'Development Status :: 4 - Beta',
```

### Comparing `pyhafas-0.3.1/tests/base/products_filter_test.py` & `pyhafas-0.4.0/tests/base/products_filter_test.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/tests/db/parsing/departures_raw.json` & `pyhafas-0.4.0/tests/db/parsing/departures_raw.json`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/tests/db/parsing/departures_test.py` & `pyhafas-0.4.0/tests/db/parsing/departures_test.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/tests/db/parsing/journey_raw.json` & `pyhafas-0.4.0/tests/db/parsing/journey_raw.json`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/tests/db/parsing/journey_test.py` & `pyhafas-0.4.0/tests/db/parsing/journey_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 import os
 
 from pyhafas.profile import DBProfile
-from pyhafas.types.fptf import Journey, Leg, Mode, Station, Stopover
+from pyhafas.types.fptf import Journey, Leg, Mode, Station, Stopover, Remark
 
 from tests.types import PyTestHafasResponse
 
 
 def test_db_journey_parsing():
     directory = os.path.dirname(os.path.realpath(__file__))
     raw_hafas_json_file = open(directory + "/journey_raw.json", "r")
@@ -49,28 +49,55 @@
                 ),
                 cancelled=False,
                 arrival=None,
                 arrival_delay=None,
                 arrival_platform=None,
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 8, 15, 7)),
                 departure_delay=datetime.timedelta(seconds=240),
-                departure_platform='1'
+                departure_platform='1',
+                remarks=[],
             ), Stopover(
                 stop=Station(
                     id='8000135',
                     lid='A=1@O=Troisdorf@X=7150892@Y=50813926@U=80@L=8000135@',
                     name='Troisdorf',
                     latitude=50.813926,
                     longitude=7.150892
                 ),
                 cancelled=False,
                 arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 8, 15, 12)),
                 arrival_delay=datetime.timedelta(seconds=240),
                 arrival_platform='1',
                 departure=None,
                 departure_delay=None,
-                departure_platform=None
+                departure_platform=None,
+                remarks=[],
+            ),
+        ],
+        remarks=[
+            Remark(
+                remark_type='A',
+                code='FB',
+                subject=None,
+                text='Fahrradmitnahme begrenzt möglich',
+                priority=260,
+                trip_id=None
+            ),
+            Remark(
+                remark_type='A',
+                code='K2',
+                subject=None,
+                text='nur 2. Klasse',
+                priority=300,
+                trip_id=None
+            ),
+            Remark(
+                remark_type='A',
+                code='EH',
+                subject=None,
+                text='Fahrzeuggebundene Einstiegshilfe vorhanden',
+                priority=560,
+                trip_id=None
             )
-            ],
-        )]
+        ])]
     )
     assert DBProfile().parse_journey_request(hafas_response) == correct_journey
```

### Comparing `pyhafas-0.3.1/tests/db/parsing/journeys_raw.json` & `pyhafas-0.4.0/tests/db/parsing/journeys_raw.json`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/tests/db/parsing/journeys_test.py` & `pyhafas-0.4.0/tests/db/parsing/journeys_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 import os
 
 from pyhafas.profile import DBProfile
-from pyhafas.types.fptf import Journey, Leg, Mode, Station, Stopover
+from pyhafas.types.fptf import Journey, Leg, Mode, Station, Stopover, Remark
 
 from tests.types import PyTestHafasResponse
 
 
 def test_db_journeys_parsing():
     directory = os.path.dirname(os.path.realpath(__file__))
     raw_hafas_json_file = open(directory + "/journeys_raw.json", "r")
@@ -49,27 +49,55 @@
                     longitude=7.203029),
                 cancelled=False,
                 arrival=None,
                 arrival_delay=None,
                 arrival_platform=None,
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 6, 12, 7)),
                 departure_delay=None,
-                departure_platform='1'),
+                departure_platform='1',
+                remarks=[]),
                 Stopover(
                     stop=Station(
                         id='8000135',
                         lid='A=1@O=Troisdorf@X=7150892@Y=50813926@U=80@L=8000135@',
                         name='Troisdorf',
                         latitude=50.813926,
                         longitude=7.150892),
                     cancelled=False,
                     arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 6, 12, 12)),
                     arrival_delay=datetime.timedelta(0),
                     arrival_platform='1',
                     departure=None,
                     departure_delay=None,
-                    departure_platform=None
-            )
+                    departure_platform=None,
+                    remarks=[],
+                )
+            ],
+            remarks=[
+                Remark(
+                    remark_type='A',
+                    code='FB',
+                    subject=None,
+                    text='Fahrradmitnahme begrenzt möglich',
+                    priority=260,
+                    trip_id=None
+                ),
+                Remark(
+                    remark_type='A',
+                    code='K2',
+                    subject=None,
+                    text='nur 2. Klasse',
+                    priority=300,
+                    trip_id=None
+                ),
+                Remark(
+                    remark_type='A',
+                    code='EH',
+                    subject=None,
+                    text='Fahrzeuggebundene Einstiegshilfe vorhanden',
+                    priority=560,
+                    trip_id=None
+                )
             ]
-        )]
+        )],
     )]
     assert DBProfile().parse_journeys_request(hafas_response) == correct_journeys
```

### Comparing `pyhafas-0.3.1/tests/db/parsing/locations_raw.json` & `pyhafas-0.4.0/tests/db/parsing/locations_raw.json`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/tests/db/parsing/locations_test.py` & `pyhafas-0.4.0/tests/db/parsing/locations_test.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/tests/db/parsing/trip_raw.json` & `pyhafas-0.4.0/tests/db/parsing/trip_raw.json`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/tests/db/parsing/trip_test.py` & `pyhafas-0.4.0/tests/db/parsing/trip_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 import os
 
 from pyhafas.profile import DBProfile
-from pyhafas.types.fptf import Leg, Mode, Station, Stopover
+from pyhafas.types.fptf import Leg, Mode, Station, Stopover, Remark
 
 from tests.types import PyTestHafasResponse
 
 
 def test_db_trips_parsing():
     directory = os.path.dirname(os.path.realpath(__file__))
     raw_hafas_json_file = open(directory + "/trip_raw.json", "r")
@@ -48,296 +48,316 @@
                 ),
                 cancelled=False,
                 arrival=None,
                 arrival_delay=None,
                 arrival_platform=None,
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 2)),
                 departure_delay=None,
-                departure_platform='2'
+                departure_platform='2',
+                remarks=[],
             ), Stopover(
                 stop=Station(
                     id='8005556',
                     lid='A=1@O=Siegburg/Bonn@X=7203029@Y=50793916@U=80@L=8005556@',
                     name='Siegburg/Bonn',
                     latitude=50.793916,
                     longitude=7.203029
                 ),
                 cancelled=False,
                 arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 6)),
                 arrival_delay=None,
                 arrival_platform='1',
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 7)),
                 departure_delay=None,
-                departure_platform='1'
+                departure_platform='1',
+                remarks=[],
             ), Stopover(
                 stop=Station(
                     id='8000135',
                     lid='A=1@O=Troisdorf@X=7150892@Y=50813926@U=80@L=8000135@',
                     name='Troisdorf',
                     latitude=50.813926,
                     longitude=7.150892
                 ),
                 cancelled=False,
                 arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 12)),
                 arrival_delay=None,
                 arrival_platform='1',
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 13)),
                 departure_delay=None,
-                departure_platform='1'
+                departure_platform='1',
+                remarks=[],
             ), Stopover(
                 stop=Station(
                     id='8005629',
                     lid='A=1@O=Spich@X=7114917@Y=50826727@U=80@L=8005629@',
                     name='Spich',
                     latitude=50.826727,
                     longitude=7.114917
                 ),
                 cancelled=False,
                 arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 15)),
                 arrival_delay=None,
                 arrival_platform='1',
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 16)),
                 departure_delay=None,
-                departure_platform='1'
+                departure_platform='1',
+                remarks=[],
             ), Stopover(
                 stop=Station(
                     id='8004873',
                     lid='A=1@O=Porz-Wahn@X=7079266@Y=50858135@U=80@L=8004873@',
                     name='Porz-Wahn',
                     latitude=50.858135,
                     longitude=7.079266
                 ),
                 cancelled=False,
                 arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 19)),
                 arrival_delay=None,
                 arrival_platform='1',
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 19)),
                 departure_delay=None,
-                departure_platform='1'
+                departure_platform='1',
+                remarks=[],
             ), Stopover(
                 stop=Station(
                     id='8003330',
                     lid='A=1@O=Köln/Bonn Flughafen@X=7119304@Y=50878900@U=80@L=8003330@',
                     name='Köln/Bonn Flughafen',
                     latitude=50.8789,
                     longitude=7.119304
                 ),
                 cancelled=False,
                 arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 23)),
                 arrival_delay=None,
                 arrival_platform='2',
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 24)),
                 departure_delay=None,
-                departure_platform='2'
+                departure_platform='2',
+                remarks=[],
             ), Stopover(
                 stop=Station(
                     id='8003358',
                     lid='A=1@O=Köln Frankfurter Straße@X=7051264@Y=50915217@U=80@L=8003358@',
                     name='Köln Frankfurter Straße',
                     latitude=50.915217,
                     longitude=7.051264
                 ),
                 cancelled=False,
                 arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 29)),
                 arrival_delay=None,
                 arrival_platform='1',
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 29)),
                 departure_delay=None,
-                departure_platform='1'
+                departure_platform='1',
+                remarks=[],
             ), Stopover(
                 stop=Station(
                     id='8003320',
                     lid='A=1@O=Köln Trimbornstr@X=6996736@Y=50935856@U=80@L=8003320@',
                     name='Köln Trimbornstr',
                     latitude=50.935856,
                     longitude=6.996736),
                 cancelled=False,
                 arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 34)),
                 arrival_delay=None,
                 arrival_platform='2',
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 34)),
                 departure_delay=None,
-                departure_platform='2'
+                departure_platform='2',
+                remarks=[],
             ), Stopover(
                 stop=Station(
                     id='8083368',
                     lid='A=1@O=Köln Messe/Deutz Gl. 9-10@X=6974640@Y=50941303@U=80@L=8083368@',
                     name='Köln Messe/Deutz Gl. 9-10',
                     latitude=50.941303,
                     longitude=6.97464),
                 cancelled=False,
                 arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 36)),
                 arrival_delay=None,
                 arrival_platform='10',
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 37)),
                 departure_delay=None,
-                departure_platform='10'
+                departure_platform='10',
+                remarks=[],
             ), Stopover(
                 stop=Station(
                     id='8000207',
                     lid='A=1@O=Köln Hbf@X=6958730@Y=50943029@U=80@L=8000207@',
                     name='Köln Hbf',
                     latitude=50.943029,
                     longitude=6.95873
                 ),
                 cancelled=False,
                 arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 39)),
                 arrival_delay=None,
                 arrival_platform='11 B-C',
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 40)),
                 departure_delay=None,
-                departure_platform='11 B-C'
+                departure_platform='11 B-C',
+                remarks=[],
             ), Stopover(
                 stop=Station(
                     id='8003392',
                     lid='A=1@O=Köln Hansaring@X=6952563@Y=50949133@U=80@L=8003392@',
                     name='Köln Hansaring',
                     latitude=50.949133,
                     longitude=6.952563
                 ),
                 cancelled=False,
                 arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 42)),
                 arrival_delay=None,
                 arrival_platform='1',
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 42)),
                 departure_delay=None,
-                departure_platform='1'
+                departure_platform='1',
+                remarks=[],
             ), Stopover(
                 stop=Station(
                     id='8000208',
                     lid='A=1@O=Köln-Ehrenfeld@X=6917280@Y=50951533@U=80@L=8000208@',
                     name='Köln-Ehrenfeld',
                     latitude=50.951533,
                     longitude=6.91728),
                 cancelled=False,
                 arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 45)),
                 arrival_delay=None,
                 arrival_platform='2',
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 46)),
                 departure_delay=None,
-                departure_platform='2'
+                departure_platform='2',
+                remarks=[],
             ), Stopover(
                 stop=Station(
                     id='8003375',
                     lid='A=1@O=Köln-Müngersdorf Technologiepark@X=6888200@Y=50948396@U=80@L=8003375@',
                     name='Köln-Müngersdorf Technologiepark',
                     latitude=50.948396,
                     longitude=6.8882
                 ),
                 cancelled=False,
                 arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 48)),
                 arrival_delay=None,
                 arrival_platform='2',
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 49)),
                 departure_delay=None,
-                departure_platform='2'
+                departure_platform='2',
+                remarks=[],
             ), Stopover(
                 stop=Station(
                     id='8003732',
                     lid='A=1@O=Lövenich@X=6834436@Y=50942930@U=80@L=8003732@',
                     name='Lövenich',
                     latitude=50.94293,
                     longitude=6.834436
                 ),
                 cancelled=False,
                 arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 51)),
                 arrival_delay=None,
                 arrival_platform='2',
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 52)),
                 departure_delay=None,
-                departure_platform='2'
+                departure_platform='2',
+                remarks=[],
             ), Stopover(
                 stop=Station(
                     id='8003383',
                     lid='A=1@O=Köln-Weiden West@X=6815136@Y=50940899@U=80@L=8003383@',
                     name='Köln-Weiden West',
                     latitude=50.940899,
                     longitude=6.815136
                 ),
                 cancelled=False,
                 arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 53)),
                 arrival_delay=None,
                 arrival_platform='2',
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 54)),
                 departure_delay=None,
-                departure_platform='2'
+                departure_platform='2',
+                remarks=[],
             ), Stopover(
                 stop=Station(
                     id='8002389',
                     lid='A=1@O=Frechen-Königsdorf@X=6777849@Y=50936503@U=80@L=8002389@',
                     name='Frechen-Königsdorf',
                     latitude=50.936503,
                     longitude=6.777849
                 ),
                 cancelled=False,
                 arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 56)),
                 arrival_delay=None,
                 arrival_platform='2',
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 12, 57)),
                 departure_delay=None,
-                departure_platform='2'
+                departure_platform='2',
+                remarks=[],
             ), Stopover(
                 stop=Station(
                     id='8000178',
                     lid='A=1@O=Horrem@X=6713495@Y=50916250@U=80@L=8000178@',
                     name='Horrem',
                     latitude=50.91625,
                     longitude=6.713495
                 ),
                 cancelled=False,
                 arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 13, 0)),
                 arrival_delay=None,
                 arrival_platform='2',
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 13, 1)),
                 departure_delay=None,
-                departure_platform='2'
+                departure_platform='2',
+                remarks=[],
             ), Stopover(
                 stop=Station(
                     id='8005575',
                     lid='A=1@O=Sindorf@X=6681107@Y=50903711@U=80@L=8005575@',
                     name='Sindorf',
                     latitude=50.903711,
                     longitude=6.681107
                 ), cancelled=False,
                 arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 13, 3)),
                 arrival_delay=None,
                 arrival_platform='1',
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 13, 3)),
                 departure_delay=None,
-                departure_platform='1'
+                departure_platform='1',
+                remarks=[],
             ), Stopover(
                 stop=Station(
                     id='8001264',
                     lid='A=1@O=Buir@X=6574513@Y=50862405@U=80@L=8001264@',
                     name='Buir',
                     latitude=50.862405,
                     longitude=6.574513
                 ),
                 cancelled=False,
                 arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 13, 9)),
                 arrival_delay=None,
                 arrival_platform='2',
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 13, 10)),
                 departure_delay=None,
-                departure_platform='2'
+                departure_platform='2',
+                remarks=[],
             ), Stopover(
                 stop=Station(
                     id='8003990',
                     lid='A=1@O=Merzenich@X=6518051@Y=50840031@U=80@L=8003990@',
                     name='Merzenich',
                     latitude=50.840031,
                     longitude=6.518051
                 ),
                 cancelled=False,
                 arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 13, 13)),
                 arrival_delay=None,
                 arrival_platform='2',
                 departure=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 13, 13)),
                 departure_delay=None,
-                departure_platform='2'
+                departure_platform='2',
+                remarks=[],
             ),
             Stopover(
                 stop=Station(
                     id='8000084',
                     lid='A=1@O=Düren@X=6482454@Y=50809513@U=80@L=8000084@',
                     name='Düren',
                     latitude=50.809513,
@@ -345,12 +365,39 @@
                 ),
                 cancelled=False,
                 arrival=DBProfile().timezone.localize(datetime.datetime(2020, 8, 5, 13, 17)),
                 arrival_delay=None,
                 arrival_platform='5',
                 departure=None,
                 departure_delay=None,
-                departure_platform=None
+                departure_platform=None,
+                remarks=[],
+            )
+        ],
+        remarks=[
+            Remark(
+                remark_type='A',
+                code='FB',
+                subject=None,
+                text='Fahrradmitnahme begrenzt möglich',
+                priority=260,
+                trip_id=None
+            ),
+            Remark(
+                remark_type='A',
+                code='K2',
+                subject=None,
+                text='nur 2. Klasse',
+                priority=300,
+                trip_id=None
+            ),
+            Remark(
+                remark_type='A',
+                code='EH',
+                subject=None,
+                text='Fahrzeuggebundene Einstiegshilfe vorhanden',
+                priority=560,
+                trip_id=None
             )
         ]
     )
     assert DBProfile().parse_trip_request(hafas_response) == correct_trip
```

### Comparing `pyhafas-0.3.1/tests/vsn/parsing/departures_raw.json` & `pyhafas-0.4.0/tests/vsn/parsing/departures_raw.json`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/tests/vsn/parsing/departures_test.py` & `pyhafas-0.4.0/tests/vsn/parsing/departures_test.py`

 * *Files identical despite different names*

### Comparing `pyhafas-0.3.1/tests/vsn/parsing/journeys_raw.json` & `pyhafas-0.4.0/tests/vsn/parsing/journeys_raw.json`

 * *Files identical despite different names*

