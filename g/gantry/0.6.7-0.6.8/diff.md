# Comparing `tmp/gantry-0.6.7.tar.gz` & `tmp/gantry-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gantry-0.6.7.tar", last modified: Fri Jun  2 17:03:46 2023, max compression
+gzip compressed data, was "gantry-0.6.8.tar", last modified: Sat Jul  1 00:55:04 2023, max compression
```

## Comparing `gantry-0.6.7.tar` & `gantry-0.6.8.tar`

### file list

```diff
@@ -1,174 +1,175 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.123817 gantry-0.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-06-02 17:03:32.000000 gantry-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-02 17:03:32.000000 gantry-0.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-02 17:03:46.123817 gantry-0.6.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.107817 gantry-0.6.7/gantry/
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.107817 gantry-0.6.7/gantry/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/alerts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/alerts/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/alerts/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.107817 gantry-0.6.7/gantry/applications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/applications/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28849 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/applications/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    17741 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/applications/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/applications/llm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/applications/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.107817 gantry-0.6.7/gantry/automations/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.107817 gantry-0.6.7/gantry/automations/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/actions/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/automations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.111817 gantry-0.6.7/gantry/automations/curators/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/curators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/curators/curators.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/curators/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/curators/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/curators/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/curators/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    26072 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/curators/stock_curators.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.111817 gantry-0.6.7/gantry/automations/triggers/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/automations/triggers/triggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.111817 gantry-0.6.7/gantry/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/cli/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/cli/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/cli/data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/cli/labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/cli/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/cli/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.111817 gantry-0.6.7/gantry/data_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/data_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/data_generator/data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.111817 gantry-0.6.7/gantry/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/dataset/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/dataset/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    64518 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/dataset/gantry_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/dataset/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.111817 gantry-0.6.7/gantry/dataset/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/dataset/templates/load_script_template.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.111817 gantry-0.6.7/gantry/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    94223 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/logger/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/logger/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/logger/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/logger/event_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/logger/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/logger/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/logger/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/logger/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.115817 gantry-0.6.7/gantry/query/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.115817 gantry-0.6.7/gantry/query/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    39147 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/core/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/core/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    20187 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/core/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/core/queryframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.115817 gantry-0.6.7/gantry/query/distance/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/distance/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.115817 gantry-0.6.7/gantry/query/metric/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/metric/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/query/time_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 17:03:32.000000 gantry-0.6.7/gantry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.107817 gantry-0.6.7/gantry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-02 17:03:46.000000 gantry-0.6.7/gantry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-02 17:03:46.000000 gantry-0.6.7/gantry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 17:03:46.000000 gantry-0.6.7/gantry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 17:03:46.000000 gantry-0.6.7/gantry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-02 17:03:46.000000 gantry-0.6.7/gantry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 17:03:46.000000 gantry-0.6.7/gantry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 17:03:46.123817 gantry-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-02 17:03:32.000000 gantry-0.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.115817 gantry-0.6.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.115817 gantry-0.6.7/tests/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/alerts/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/alerts/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/alerts/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.115817 gantry-0.6.7/tests/applications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/applications/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/applications/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/applications/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/applications/test_llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/applications/test_llm_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.115817 gantry-0.6.7/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/cli/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    14561 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/cli/test_data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/cli/test_labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/cli/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/cli/test_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/cli/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.119817 gantry-0.6.7/tests/curator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/curator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/curator/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/curator/test_curator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/curator/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/curator/test_selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.119817 gantry-0.6.7/tests/data_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/data_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/data_generator/test_data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.119817 gantry-0.6.7/tests/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/dataset/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/dataset/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/dataset/test_gantry_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/dataset/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.119817 gantry-0.6.7/tests/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/logger/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)   110166 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/logger/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/logger/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/logger/test_event_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/logger/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/logger/test_stores.py
--rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/logger/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.119817 gantry-0.6.7/tests/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.119817 gantry-0.6.7/tests/query/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/core/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/core/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/core/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/core/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/core/test_queryframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    39032 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/core/test_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/core/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.119817 gantry-0.6.7/tests/query/distance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/distance/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:46.123817 gantry-0.6.7/tests/query/metric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/metric/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/query/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/test_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-02 17:03:32.000000 gantry-0.6.7/tests/test_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.363473 gantry-0.6.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-07-01 00:54:52.000000 gantry-0.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-01 00:54:52.000000 gantry-0.6.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-01 00:55:04.363473 gantry-0.6.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.323473 gantry-0.6.8/gantry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.327473 gantry-0.6.8/gantry/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20961 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/alerts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/alerts/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/alerts/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.327473 gantry-0.6.8/gantry/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/applications/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30565 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/applications/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17976 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/applications/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/applications/llm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/applications/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.327473 gantry-0.6.8/gantry/automations/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.331473 gantry-0.6.8/gantry/automations/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/actions/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/automations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.331473 gantry-0.6.8/gantry/automations/curators/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/curators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23367 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/curators/curators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/curators/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/curators/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/curators/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/curators/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26072 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/curators/stock_curators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.331473 gantry-0.6.8/gantry/automations/triggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13512 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/automations/triggers/triggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.335473 gantry-0.6.8/gantry/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/cli/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/cli/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/cli/data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/cli/labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/cli/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/cli/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.335473 gantry-0.6.8/gantry/data_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/data_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/data_generator/data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.335473 gantry-0.6.8/gantry/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/dataset/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/dataset/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64518 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/dataset/gantry_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/dataset/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.339473 gantry-0.6.8/gantry/dataset/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/dataset/templates/load_script_template.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.339473 gantry-0.6.8/gantry/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94223 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/logger/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/logger/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/logger/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/logger/event_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/logger/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/logger/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/logger/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/logger/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.343473 gantry-0.6.8/gantry/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.343473 gantry-0.6.8/gantry/query/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39714 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/core/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/core/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20187 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/core/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/core/queryframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.343473 gantry-0.6.8/gantry/query/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/distance/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.343473 gantry-0.6.8/gantry/query/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/metric/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/query/time_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-01 00:54:52.000000 gantry-0.6.8/gantry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.323473 gantry-0.6.8/gantry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-01 00:55:04.000000 gantry-0.6.8/gantry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-01 00:55:04.000000 gantry-0.6.8/gantry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 00:55:04.000000 gantry-0.6.8/gantry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-01 00:55:04.000000 gantry-0.6.8/gantry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-01 00:55:04.000000 gantry-0.6.8/gantry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-01 00:55:04.000000 gantry-0.6.8/gantry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 00:55:04.363473 gantry-0.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-01 00:54:52.000000 gantry-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.347473 gantry-0.6.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.347473 gantry-0.6.8/tests/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/alerts/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/alerts/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/alerts/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.351473 gantry-0.6.8/tests/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/applications/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/applications/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/applications/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/applications/test_llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/applications/test_llm_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.351473 gantry-0.6.8/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/cli/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14561 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/cli/test_data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/cli/test_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/cli/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/cli/test_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/cli/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.355473 gantry-0.6.8/tests/curator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/curator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/curator/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/curator/test_curator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/curator/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/curator/test_selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.355473 gantry-0.6.8/tests/data_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/data_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/data_generator/test_data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.355473 gantry-0.6.8/tests/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/dataset/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/dataset/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/dataset/test_gantry_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/dataset/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.359473 gantry-0.6.8/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/logger/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110166 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/logger/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/logger/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/logger/test_event_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/logger/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/logger/test_stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/logger/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.359473 gantry-0.6.8/tests/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.363473 gantry-0.6.8/tests/query/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/core/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/core/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/core/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/core/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/core/test_queryframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39032 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/core/test_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/core/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.363473 gantry-0.6.8/tests/query/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/distance/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:55:04.363473 gantry-0.6.8/tests/query/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/metric/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/query/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/test_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-01 00:54:52.000000 gantry-0.6.8/tests/test_validator.py
```

### Comparing `gantry-0.6.7/LICENSE` & `gantry-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/PKG-INFO` & `gantry-0.6.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: gantry
-Version: 0.6.7
+Version: 0.6.8
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gantry-0.6.7/gantry/__init__.py` & `gantry-0.6.8/gantry/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,10 +111,10 @@
     """
     Get API key from environment if not already supplied. Raise exception if not found.
     """
     api_key = api_key or os.environ.get("GANTRY_API_KEY")
     if api_key is None:
         raise ValueError(
             "Please provide an API key to initialize Gantry SDK. API key can be provided"
-            + "as parameter to init methods or by setting env var GANTRY_API_KEY"
+            + " as parameter to init methods or by setting env var GANTRY_API_KEY"
         )
     return api_key
```

### Comparing `gantry-0.6.7/gantry/alerts/client.py` & `gantry-0.6.8/gantry/alerts/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     """
     Allowed aggregations for Gantry Alerts.
 
     The full list of aggregations are:
 
     .. code-block:: python
 
+        TOTAL_DIFFERENCE
+        PERCENT_DIFFERENCE
         TOTAL
         MAX
         MIN
         MEAN
         STD
         PDF
         QUANTILES
@@ -63,14 +65,16 @@
         PR_CURVE_PLOT
         DISTRIBUTION_SKETCH
         CATEGORICAL_SKETCH
 
     """
 
     # Standard Aggregation
+    TOTAL_DIFFERENCE = "total_difference"
+    PERCENT_DIFFERENCE = "percent_difference"
     TOTAL = "total"
     MAX = "maximum"
     MIN = "minimum"
     MEAN = "mean"
     STD = "stddev"
     PDF = "pdf"
     QUANTILES = "quantiles"
@@ -106,14 +110,29 @@
     PR_CURVE_PLOT = "pr_curve_plot"
     # Sketch Aggregations.
     DISTRIBUTION_SKETCH = "distribution_sketch"
     CATEGORICAL_SKETCH = "categorical_sketch"
 
 
 @dataclass
+class DiffCheck:
+    """
+    Data shape definition for diff checks.
+    """
+
+    field_names: List[str]
+    aggregation: AlertsAggregation
+    trigger_range_type: str
+    subqueries: dict
+    check_type: str = "diff_check"
+    lower_bound: Optional[float] = None
+    upper_bound: Optional[float] = None
+
+
+@dataclass
 class AlertsCheck:
     """
     Data shape definition for alert checks.
 
     column_names correspond to the schema columns in your application.
     """
 
@@ -239,15 +258,15 @@
             )
             return response["data"]["triggered_alerts"]
 
     def _create_or_update_alert(
         self,
         application_name: str,
         alert_name: str,
-        alert_checks: List[AlertsCheck],
+        alert_checks: Union[List[AlertsCheck], List[DiffCheck]],
         evaluation_window: str,
         evaluation_delay: str,
         tags: Optional[Dict[str, str]] = None,
         alert_id: Optional[Union[str, UUID]] = None,
     ) -> str:
         """
         Create or update (upsert) an alert in the Gantry application.
@@ -290,24 +309,53 @@
             application_id = self._get_application(application_name)["id"]
         except GantryException as ge:
             raise ValueError(
                 f'Could not find "{application_name}". Reason: "{ge}". Check the spelling?'
             )
         _alert_checks = []
         for check in alert_checks:
-            check_as_dict = dataclasses.asdict(check)
-            check_as_dict["aggregation"] = check_as_dict["aggregation"].value
-            check_as_dict["data_node_ids"] = [
-                data_node_id
-                for __, data_node_id in self._map_column_names_to_ids(
-                    application_name, check_as_dict["column_names"]
-                ).items()
-            ]
-            check_as_dict.pop("column_names")
-            _alert_checks.append(check_as_dict)
+            if isinstance(check, AlertsCheck):
+                check_as_dict = dataclasses.asdict(check)
+                check_as_dict["aggregation"] = check_as_dict["aggregation"].value
+                check_as_dict["data_node_ids"] = [
+                    data_node_id
+                    for __, data_node_id in self._map_column_names_to_ids(
+                        application_name, check_as_dict["column_names"]
+                    ).items()
+                ]
+                check_as_dict.pop("column_names")
+                _alert_checks.append(check_as_dict)
+            elif isinstance(check, DiffCheck):
+                check_as_dict = dataclasses.asdict(check)
+                application_schema = self._get_application(application_name)
+                application_data_nodes = (
+                    application_schema["prediction_datanodes"]
+                    + application_schema["feedback_datanodes"]
+                )
+                application_data_nodes_map = {}
+                for data_node in application_data_nodes:
+                    application_data_nodes_map[data_node["name"]] = data_node["user_dtype"]
+
+                for i in range(len(check_as_dict["subqueries"])):
+                    subquery = check_as_dict["subqueries"][i]
+                    if subquery["field_names"][0] not in application_data_nodes_map:
+                        raise ValueError(
+                            f'Could not find "{subquery["field_names"]}"'
+                            f'in application "{application_name}".'
+                        )
+                for i in range(len(check_as_dict["subqueries"])):
+                    subquery = check_as_dict["subqueries"][i]
+                    feature = {
+                        "name": subquery["field_names"][0],
+                        "user_dtype": application_data_nodes_map[subquery["field_names"][0]],
+                    }
+                    check_as_dict["subqueries"][i]["features"] = [feature]
+                    check_as_dict["subqueries"][i].pop("field_names")
+                check_as_dict["aggregation"] = check_as_dict["aggregation"].value
+                _alert_checks.append(check_as_dict)
         json_data = {
             "alert_type": GantryAlerts.ALERT_TYPE,
             "alert_name": alert_name,
             "model_node_id": application_id,
             "relative_time": evaluation_window,
             "delay_time": evaluation_delay,
             "checks": _alert_checks,
@@ -323,15 +371,15 @@
         )
         return response["data"]["alert"]["id"]
 
     def create_alert(
         self,
         application_name: str,
         alert_name: str,
-        alert_checks: List[AlertsCheck],
+        alert_checks: Union[List[AlertsCheck], List[DiffCheck]],
         evaluation_window: str,
         evaluation_delay: str,
         tags: Optional[Dict[str, str]] = None,
     ) -> str:
         """
         Create an alert in your Gantry application.
```

### Comparing `gantry-0.6.7/gantry/alerts/globals.py` & `gantry-0.6.8/gantry/alerts/globals.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/alerts/main.py` & `gantry-0.6.8/gantry/alerts/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/api_client.py` & `gantry-0.6.8/gantry/api_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/applications/client.py` & `gantry-0.6.8/gantry/applications/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/applications/core.py` & `gantry-0.6.8/gantry/applications/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from gantry.automations.automations import Automation
 from gantry.exceptions import ClientNotInitialized, GantryRequestException
 from gantry.logger.constants import BatchType
 from gantry.logger.main import _upload_data_as_batch, log, log_file
 from gantry.query.core.dataframe import GantryDataFrame
 from gantry.query.core.utils import get_application_node_id
 from gantry.query.time_window import RelativeTimeWindow, TimeWindow
+from gantry.utils import from_isoformat_duration, to_isoformat_duration
 
 logger = logging.getLogger(__name__)
 
 
 class Run:
     """
     Context manager for logging.
@@ -299,15 +300,15 @@
                 is a dict of the features for the i-th prediction to be logged.
             outputs (optional, Union[Any, List[Any], dict, List[dict], pd.DataFrame, pd.Series, np.ndarray): A list of prediction outputs. `outputs[i]`
                 should be the application output for the prediction with features `inputs[i]`.
             feedbacks (optional, Union[dict, List[dict], pd.DataFrame, pd.Series, np.ndarray]): A list of feedbacks. `feedbacks[i]`
                 is a dict of the features for the i-th prediction to be logged.
             ignore_inputs (optional, List[str]): A list of names of input features that should not
                 be monitored.
-            timestamps (optional, Union[List[datetime.datetime], pd.DatetimeIndex, np.array[datetime.datetime]):  # noqa: E501
+            timestamps (optional, Union[List[datetime.datetime], pd.DatetimeIndex, np.array[datetime.datetime]):
                 A list of prediction timestamps.
                 If specified, `timestamps[i]` should be the timestamps for the i-th prediction.
                 If timestamps = None (default), then the prediction
                 timestamp defaults to the time when `log_records` is called.
             sort_on_timestamp (bool, defaults to True): Works when timestamps are provided.
                 Sort using the given timestamp. Default to True.
             sample_rate: Used for down-sampling. The probability as a float that each record
@@ -342,15 +343,15 @@
             join_keys  (optional, Union[List[str], pd.Series[str]]): provide keys to identify
                 each record. These keys can be used later to provide feedback. If not provided,
                 a random record key will be generated for each record.
 
         Returns:
             Tuple ([batch_id, list[join_keys]]): The batch_id will be None if records are not
             logged as batch. The list of join_keys will be the records keys.
-        """
+        """  # noqa: E501
         run_id = None
         run_tags = None
         if Run._current_instance:
             run_id = Run._current_instance.run_id
             run_tags = Run._current_instance.tags
         return log(
             application=self._name,
@@ -398,37 +399,45 @@
                         "upper_bound": 3
                     }
                 ]
             )
 
         Args:
             time_window (optional, Union[TimeWindow, RelativeTimeWindow]): A time window object.
+                If a TimeWindow is passed in, the query is saved with fixed timestamps.
+                If a RelativeTimeWindow is passed in, the query is saved with relative time
+                    window and offset.
             version (optional, Union[int, str]): The version of the application to query.
             env (optional, str) : The environment of the application to query.
             filters (optional, list[dict]) : A list of filters to apply to the query.
             tags (optional, dict) : A dictionary of tags to apply to the query.
 
         Returns:
             Gantry Dataframe with all the query information to fetch data.
         """
         start_time: Union[str, datetime.datetime] = "-24H"
         end_time: Union[str, datetime.datetime] = "now"
         if time_window:
             start_time = time_window.start_time
             end_time = time_window.end_time
-
         return GantryDataFrame(
             api_client=self._api_client,
             application=self._name,
             start_time=start_time,
             end_time=end_time,
             version=version,
             env=env,
             filters=filters,
             tags=tags,
+            relative_time_window=time_window.window_length
+            if time_window is not None and isinstance(time_window, RelativeTimeWindow)
+            else None,
+            relative_time_delay=time_window.offset
+            if time_window is not None and isinstance(time_window, RelativeTimeWindow)
+            else None,
         )
 
     def save_query(self, name: str, query: GantryDataFrame):
         """
         Save a query to the Gantry database.
 
         Example:
@@ -448,16 +457,24 @@
             "tags": query.tags or {},
             "filters": query.filters or [],
             "details": {"color": "default"},
         }
         if query.start_time or query.end_time:
             if not (query.start_time and query.end_time):
                 raise ValueError("Both start_time and end_time must be specified.")
-            data["start_time"] = query.start_time  # type: ignore
-            data["end_time"] = query.end_time  # type: ignore
+            if query.relative_time_window:
+                data["relative_time_window"] = to_isoformat_duration(query.relative_time_window)
+                data["relative_time_delay"] = (
+                    to_isoformat_duration(query.relative_time_delay)
+                    if query.relative_time_delay
+                    else "P0D"
+                )
+            else:
+                data["start_time"] = query.start_time  # type: ignore
+                data["end_time"] = query.end_time  # type: ignore
 
         try:
             model_node_id = get_application_node_id(
                 self._api_client, self._name, version=query.version
             )
             data["model_node_id"] = model_node_id
         except GantryRequestException:
@@ -493,21 +510,33 @@
                 "GET", f"/api/v1/applications/{model_node_id}/queries/{name}"
             )
             query = query["data"]
             deserialized_tags = {}
             for tag in query["tags"]:
                 deserialized_tags[tag["tag_name"]] = tag["tag_value"]
 
+            if query.get("relative_time_window") is not None:
+                query["relative_time_window"] = from_isoformat_duration(
+                    query["relative_time_window"]
+                )
+                query["end_time"] = datetime.datetime.utcnow()
+                query["start_time"] = query["end_time"] - query["relative_time_window"]
             return GantryDataFrame(
                 api_client=self._api_client,
                 application=self._name,
                 start_time=query["start_time"],
                 end_time=query["end_time"],
                 filters=query["filters"],
                 tags=deserialized_tags,
+                relative_time_window=query["relative_time_window"]
+                if query.get("relative_time_window")
+                else None,
+                relative_time_delay=from_isoformat_duration(query["relative_time_delay"])
+                if query.get("relative_time_delay")
+                else None,
             )
         except GantryRequestException:
             raise ValueError("Application does not exist.")
 
     def list_queries(self):
         """
         List all saved queries for this application.
@@ -598,14 +627,17 @@
 
         Args:
             automation (Automation): An Automation object.
 
         Returns:
             None
         """
+        for existing_automation in self.list_automations():
+            if existing_automation["name"] == automation.name:
+                raise ValueError(f"Automation {automation.name} already exists.")
         automation.add_to_application(self._name)
 
     def get_automation(self, automation_name: Optional[str] = None):
         """
         Get an automation by name
 
         Example:
@@ -682,32 +714,31 @@
         Returns:
             The application schema (in Python dict).
         """
         # GET /api/v1/applications/<model_name>/schemas
         res = self._api_client.request("GET", f"/api/v1/applications/{self._name}/schemas")
         return res["data"]
 
-    def create_dataset(self, name: str, bucket_name: Optional[str] = None):
+    def create_dataset(self, name: str):
         """
         Create a dataset for this application.
 
         Example:
 
         .. code-block:: python
 
-            dataset = app.create_dataset(name="demo_dataset", bucket_name="demo_bucket")
+            dataset = app.create_dataset(name="demo_dataset")
 
         Args:
             name (str): The name of the dataset.
-            bucket_name (optional, str): The bucket name of the dataset.
 
         Return:
             :class:`gantry.dataset.GantryDataset`: an object representing the created dataset.
         """
-        return dataset.create_dataset(name=name, bucket_name=bucket_name, app_name=self._name)
+        return dataset.create_dataset(name=name, app_name=self._name)
 
     def list_datasets(self, include_deleted: bool = False) -> List[Dict[str, Any]]:
         """
         List all datasets for this application.
 
         Example:
```

### Comparing `gantry-0.6.7/gantry/applications/llm.py` & `gantry-0.6.8/gantry/applications/llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,23 +351,27 @@
                 # for latest version, we get a list of all versions and pick the most recent
                 res = self._api_client.request(
                     "GET",
                     f"/api/v1/cms/{self._name}/configurations/{self._configuration_name}/versions",
                     raise_for_status=True,
                 )
                 version_data = res["data"][0]
-            else:
+            elif version in ["prod", "test"]:
                 # for releases, we can get the latest release by environment
                 res = self._api_client.request(
                     "GET",
                     f"/api/v1/cms/{self._name}/configurations/{self._configuration_name}/releases",
                     params={"latest": True, "env": version},
                     raise_for_status=True,
                 )
                 version_data = res["data"][0]["version"]
+            else:
+                raise ValueError(
+                    f"Invalid version '{version}'. Must be one of 'prod', 'test', or 'latest'"
+                )
         except IndexError:
             logger.warn("No version found for '%s'", version)
             return None
 
         # now that we have the version, we can get the config data
         res = self._api_client.request(
             "GET",
@@ -411,14 +415,15 @@
             import openai
             from openai.util import convert_to_dict
 
             gantry.init()
             my_llm_app = gantry.get_application("my-llm-app")
 
             version = my_llm_app.get_version("test")
+            # "latest", "prod", or "test"
             config = version.config
             prompt = config['prompt']
 
             def generate(values):
                 filled_in_prompt = fill_prompt(prompt, values)
                 request = {
                     "model": "text-davinci-002",
```

### Comparing `gantry-0.6.7/gantry/applications/llm_utils.py` & `gantry-0.6.8/gantry/applications/llm_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/applications/main.py` & `gantry-0.6.8/gantry/applications/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/automations/actions/actions.py` & `gantry-0.6.8/gantry/automations/actions/actions.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/automations/automations.py` & `gantry-0.6.8/gantry/automations/automations.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from gantry.api_client import APIClient
 from gantry.automations import globals
 from gantry.automations.actions import Action, SendSlackMessage
 from gantry.automations.curators import Curator
 from gantry.automations.curators.main import get_curator
 from gantry.automations.triggers import AggregationTrigger, IntervalTrigger, Trigger
+from gantry.automations.triggers.triggers import QueriesAggregationTrigger
 
 logger = logging.getLogger(__name__)
 
 
 class Automation:
     """
     Automation is the process of automatically executing tasks.
@@ -138,14 +139,16 @@
     @classmethod
     def from_dict(cls, data):
         trigger = Trigger()
         if data["trigger"]["type"] == "AggregationTrigger":
             trigger = AggregationTrigger.from_dict(data["trigger"]["content"])
         elif data["trigger"]["type"] == "IntervalTrigger":
             trigger = IntervalTrigger.from_dict(data["trigger"]["content"])
+        elif data["trigger"]["type"] == "QueriesAggregationTrigger":
+            trigger = QueriesAggregationTrigger.from_dict(data["trigger"]["content"])
 
         action = Action()
         if data["action"]["type"] == "SendSlackMessage":
             action = SendSlackMessage.from_dict(data["action"]["content"])
         elif data["action"]["type"] == "curator":
             action = get_curator(data["action"]["content"]["curator_name"])
         return cls(
@@ -178,27 +181,32 @@
         if isinstance(self.trigger, IntervalTrigger) and isinstance(self.action, Curator):
             if self.trigger.start_on:
                 self.action.update_curation_start_on(self.trigger.start_on)
             if self.trigger.interval:
                 self.action.update_curation_interval(self.trigger.interval)
             if self.trigger.delay:
                 self.action.update_curation_delay(self.trigger.delay)
-        if isinstance(self.trigger, AggregationTrigger):
+        if isinstance(self.trigger, AggregationTrigger) or isinstance(
+            self.trigger, QueriesAggregationTrigger
+        ):
             alert_id = self.trigger.generate_alert()
             self.action.update_trigger(alert_id)
 
     def start(self):
+        """
+        Start the automation process.
+        """
         self.action.start()
         data = self.to_dict()
         self._api_client.request("POST", "/api/v1/automations", json=data, raise_for_status=True)
         logger.info("Automation has started.")
 
     def stop(self):
         """
-        Stop the automation process.
+        Stop the automation process and delete all relevant actions.
         """
         self._api_client.request(
             "DELETE",
             f"/api/v1/automations/{self.name}",
             params={"application_name": self.application},
             raise_for_status=True,
         )
```

### Comparing `gantry-0.6.7/gantry/automations/curators/__init__.py` & `gantry-0.6.8/gantry/automations/curators/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/automations/curators/curators.py` & `gantry-0.6.8/gantry/automations/curators/curators.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,14 +328,20 @@
 
     def start(self) -> None:
         """
         Trigger to create the curator. This function is called from Automation.
         """
         self.create()
 
+    def stop(self) -> None:
+        """
+        Trigger to delete the curator. This function is called from Automation.
+        """
+        self.delete()
+
     def create(self, enable=True) -> "Curator":
         """
         Creates the Curator. By default, the Curator is also enabled upon creation.
         Use the `enable` parameter to change this
 
         Once created, the Curator will start curating the dataset according to the
         curation_interval. If curate_past_intervals is set to True, it will curate all
```

### Comparing `gantry-0.6.7/gantry/automations/curators/main.py` & `gantry-0.6.8/gantry/automations/curators/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/automations/curators/models.py` & `gantry-0.6.8/gantry/automations/curators/models.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/automations/curators/selectors.py` & `gantry-0.6.8/gantry/automations/curators/selectors.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/automations/curators/stock_curators.py` & `gantry-0.6.8/gantry/automations/curators/stock_curators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/automations/main.py` & `gantry-0.6.8/gantry/automations/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/cli/application.py` & `gantry-0.6.8/gantry/cli/application.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/cli/bucket.py` & `gantry-0.6.8/gantry/cli/bucket.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/cli/data_connector.py` & `gantry-0.6.8/gantry/cli/data_connector.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/cli/labeling.py` & `gantry-0.6.8/gantry/cli/labeling.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/cli/main.py` & `gantry-0.6.8/gantry/cli/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/cli/projection.py` & `gantry-0.6.8/gantry/cli/projection.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/cli/secret.py` & `gantry-0.6.8/gantry/cli/secret.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/data_generator/data_generator.py` & `gantry-0.6.8/gantry/data_generator/data_generator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/dataset/client.py` & `gantry-0.6.8/gantry/dataset/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/dataset/constants.py` & `gantry-0.6.8/gantry/dataset/constants.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/dataset/gantry_dataset.py` & `gantry-0.6.8/gantry/dataset/gantry_dataset.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/dataset/main.py` & `gantry-0.6.8/gantry/dataset/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/dataset/templates/load_script_template.py.jinja` & `gantry-0.6.8/gantry/dataset/templates/load_script_template.py.jinja`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/exceptions.py` & `gantry-0.6.8/gantry/exceptions.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/logger/client.py` & `gantry-0.6.8/gantry/logger/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -489,15 +489,15 @@
                 is a dict of the features for the i-th prediction to be logged.
             outputs (Union[List[dict], pd.Dataframe]): A list of prediction outputs. `outputs[i]`
                 should be the application output for the prediction with features `inputs[i]`.
             feedbacks (Union[List[dict], pd.DataFrame]): A list of feedbacks. `feedbacks[i]`
                 is a dict of the features for the i-th prediction to be logged.
             ignore_inputs (optional, List[str]): A list of names of input features that should not
                 be monitored.
-            timestamps (optional, Union[List[datetime.datetime], pd.DatetimeIndex, np.array[datetime.datetime]):  # noqa: E501
+            timestamps (optional, Union[List[datetime.datetime], pd.DatetimeIndex, np.array[datetime.datetime]):
                 A list of prediction timestamps.
                 If specified, `timestamps[i]` should be the timestamps for the i-th prediction.
                 If timestamps = None (default), then the prediction
                 timestamp defaults to the time when `log_records` is called.
             sort_on_timestamp (bool, defaults to True): Works when timestamps are provided.
                 Sort using the given timestamp. Default to True.
             sample_rate: Used for down-sampling. The probability as a float that each record
@@ -528,15 +528,15 @@
                 'row_tags' param. Only used when log is not called within a run.
             run_id (optional, str): This should never be provided by user. It will be populated automatically when logging within a run to group records together.
             run_tags (optional, Dict[str, str]): This should never be provided by user. It will be populated automatically when logging within a run to provide global tags for all records in the run.
 
             Returns:
             Tuple[batch_id, list[join_keys]]: The batch_id will be None if records are not
             logged as batch. The list of join_keys will be the records keys.
-        """
+        """  # noqa: E501
         if run_id:
             # Generate records/events to be logged as part of the Run.
 
             # Check if inputs, outputs, feedbacks, timestamps, and join keys are singular.
             # If so, convert to list with one element.
             if isinstance(inputs, dict):
                 inputs = [inputs]
```

### Comparing `gantry-0.6.7/gantry/logger/constants.py` & `gantry-0.6.8/gantry/logger/constants.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/logger/consumer.py` & `gantry-0.6.8/gantry/logger/consumer.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/logger/event_builder.py` & `gantry-0.6.8/gantry/logger/event_builder.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/logger/main.py` & `gantry-0.6.8/gantry/logger/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/logger/stores.py` & `gantry-0.6.8/gantry/logger/stores.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/logger/types.py` & `gantry-0.6.8/gantry/logger/types.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/logger/utils.py` & `gantry-0.6.8/gantry/logger/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,23 @@
         return sorted(parts, key=lambda d: d["PartNumber"])  # type: ignore
 
 
 class JoinKey(str):
     @classmethod
     @typechecked
     def from_dict(cls, dict_: Dict) -> str:
+        """
+        Utility function to retrieve a deterministic value from a dictionary.
+        Intended to be used for setting join_key when logging to Gantry.
+
+        Args:
+            dict_ (Dict): The dictionary from which the join key should be generated
+        Returns:
+            str: The generated join key
+        """
         return hashlib.md5(
             json.dumps(dict_, sort_keys=True, cls=EventEncoder).encode("utf-8")
         ).hexdigest()
 
 
 def _get_csv_columns(filepath: str, sep: str) -> List[str]:
     ret = []
```

### Comparing `gantry-0.6.7/gantry/query/__init__.py` & `gantry-0.6.8/gantry/query/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/query/client.py` & `gantry-0.6.8/gantry/query/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/query/core/dataframe.py` & `gantry-0.6.8/gantry/query/core/dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,33 +45,42 @@
         application: str,
         start_time: Union[str, datetime.datetime],
         end_time: Union[str, datetime.datetime],
         version: Optional[Union[int, str]] = None,
         env: Optional[str] = None,
         filters: Optional[List[dict]] = None,
         tags: Optional[dict] = None,
+        relative_time_window: Optional[datetime.timedelta] = None,
+        relative_time_delay: Optional[datetime.timedelta] = None,
     ):
         """
         :meta private: This is to skip constructor in the docs
         """
         self.start_time, self.end_time = GantryQueryFrame.resolve_time_strings(start_time, end_time)
+        if relative_time_window:
+            relative_time_delay = relative_time_delay or datetime.timedelta()
+            self.end_time = datetime.datetime.utcnow() - relative_time_delay
+            self.start_time = self.end_time - relative_time_window
         application_node_id = get_application_node_id(
             api_client, application, self.start_time, self.end_time, version
         )
         super().__init__(
             api_client,
             QueryInfo(
                 application_node_id, application, version, env, self.start_time, self.end_time
             ),
         )
         self.filters = filters or []  # Holds raw dict filters to be used when fetching data
         self.tags = tags  # Holds tags for filtering when fetching data
         self.version = version
         self.env = env
         self.series = self._build_series()
+        self.relative_time_window = relative_time_window
+        self.relative_time_delay = relative_time_delay
+        self.application = application
 
     def create_view(self, name: str) -> None:
         """Create a view from a Gantry Dataframe"""
         # Inline import to avoid circular dependency.
         from gantry.query.main import create_view
 
         create_view(
@@ -570,15 +579,15 @@
         """
         return self._fetch(
             column=self.name,
             query_filters=self.parent_dataframe.filters,
             tags=self.parent_dataframe.tags,
         )
 
-    @runs_on("int", "float")
+    @runs_on("int", "float", "tag")
     def mean(
         self, num_points: int = 1, group_by: Optional[str] = None
     ) -> Union[float, pd.DataFrame]:
         """
         Runs on int and float series only.
         Get the computed average of this GantrySeries, if available
 
@@ -594,15 +603,15 @@
             else a pd.DataFrame.
         """
         try:
             return self._aggregate_query("mean", num_points=num_points, group_by=group_by)
         except (AttributeError, ValueError, KeyError):
             raise QueryError("Invalid query. GantrySeries cannot determine mean")
 
-    @runs_on("int", "float")
+    @runs_on("int", "float", "tag")
     def std(
         self, num_points: int = 1, group_by: Optional[str] = None
     ) -> Union[float, pd.DataFrame]:
         """
         Runs on int and float series only.
         Get the standard deviation for this GantrySeries, if available
 
@@ -618,15 +627,15 @@
             else a pd.DataFrame.
         """
         try:
             return self._aggregate_query("stddev", num_points=num_points, group_by=group_by)
         except (AttributeError, ValueError, KeyError):
             raise QueryError("Invalid query. GantrySeries cannot determine standard deviation")
 
-    @runs_on("int", "float")
+    @runs_on("int", "float", "tag")
     def median(self, num_points: int = 1) -> Union[float, pd.DataFrame]:
         """
         Runs on numeric series only.
         Get the median for this GantrySeries, if available
 
         Args:
             num_points (int, defaults to 1): number of points to divide the
@@ -962,15 +971,15 @@
         if dropna:
             _temp = _temp[_temp.notna()]  # type: ignore
         try:
             return _temp._aggregate_query("percent_false", num_points=num_points, group_by=group_by)
         except (AttributeError, ValueError, KeyError):
             raise QueryError("Invalid query. GantrySeries cannot determine percent_false")
 
-    @runs_on("bool")
+    @runs_on("bool", "tag")
     def percent_null(self, num_points: int = 1, group_by: Optional[str] = None):
         """
         Runs on boolean series only.
         Percent null/NaN.
 
         Args:
             data_node (GantrySeries): GantrySeries which will be calculated
```

### Comparing `gantry-0.6.7/gantry/query/core/distance.py` & `gantry-0.6.8/gantry/query/core/distance.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/query/core/metric.py` & `gantry-0.6.8/gantry/query/core/metric.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/query/core/queryframe.py` & `gantry-0.6.8/gantry/query/core/queryframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/query/core/utils.py` & `gantry-0.6.8/gantry/query/core/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/query/distance/main.py` & `gantry-0.6.8/gantry/query/distance/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/query/globals.py` & `gantry-0.6.8/gantry/query/globals.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/query/main.py` & `gantry-0.6.8/gantry/query/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import warnings
 from typing import Optional
 from urllib.parse import urlparse
 
+from gantry import globals as gantry_globals
 from gantry.api_client import APIClient
 from gantry.const import PROD_API_URL
 from gantry.query import globals
 from gantry.query.client import GantryQuery
 from gantry.query.globals import _query_alias, validate_init
 
 
@@ -50,14 +51,15 @@
             """
             No API key provided. Please pass the api_key parameter or set the GANTRY_API_KEY
             environment variable.
             """
         )
 
     api_client = APIClient(backend, api_key)
+    gantry_globals._API_CLIENT = api_client
     globals._Query = GantryQuery(api_client)  # type: ignore[union-attr]
 
 
 @_query_alias
 def list_applications(*args, **kwargs):
     validate_init()
     return globals._Query.list_applications(*args, **kwargs)  # type: ignore[union-attr]
```

### Comparing `gantry-0.6.7/gantry/query/metric/__init__.py` & `gantry-0.6.8/gantry/query/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/query/metric/main.py` & `gantry-0.6.8/gantry/query/metric/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/query/time_window.py` & `gantry-0.6.8/gantry/query/time_window.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,13 @@
         Initialize a relative time window.
 
         Args:
             window_length (datetime.timedelta): the length of the time window.
             offset (Optional[datetime.timedelta]): the offset of the time window. Defaults to None.
         """
         self.window_length = window_length
-        self.offset = offset
-        if self.offset is None:
-            self.offset = datetime.timedelta()
+        self.offset = offset or datetime.timedelta()
         end_time: datetime.datetime = (
             datetime.datetime.utcnow() - self.offset if self.offset else datetime.datetime.utcnow()
         )
         start_time: datetime.datetime = end_time - window_length
         super().__init__(start_time, end_time)
```

### Comparing `gantry-0.6.7/gantry/serializers.py` & `gantry-0.6.8/gantry/serializers.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/utils.py` & `gantry-0.6.8/gantry/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry/validators.py` & `gantry-0.6.8/gantry/validators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/gantry.egg-info/PKG-INFO` & `gantry-0.6.8/gantry.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: gantry
-Version: 0.6.7
+Version: 0.6.8
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gantry-0.6.7/gantry.egg-info/SOURCES.txt` & `gantry-0.6.8/gantry.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 setup.py
 gantry/__init__.py
 gantry/api_client.py
 gantry/const.py
 gantry/exceptions.py
+gantry/globals.py
 gantry/serializers.py
 gantry/utils.py
 gantry/validators.py
 gantry/version.py
 gantry.egg-info/PKG-INFO
 gantry.egg-info/SOURCES.txt
 gantry.egg-info/dependency_links.txt
```

### Comparing `gantry-0.6.7/setup.py` & `gantry-0.6.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     license="Apache Software License v2",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
     entry_points={
         "console_scripts": ["gantry-cli = gantry.cli.main:cli"],
     },
```

### Comparing `gantry-0.6.7/tests/alerts/test_client.py` & `gantry-0.6.8/tests/alerts/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/alerts/test_main.py` & `gantry-0.6.8/tests/alerts/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/applications/test_client.py` & `gantry-0.6.8/tests/applications/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/applications/test_core.py` & `gantry-0.6.8/tests/applications/test_core.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pytest
 import responses
 
 from gantry.api_client import APIClient
 from gantry.applications.client import ApplicationClient
 from gantry.applications.core import Application
 from gantry.query.core.dataframe import GantryDataFrame
-from gantry.query.time_window import TimeWindow
+from gantry.query.time_window import RelativeTimeWindow, TimeWindow
 
 HOST = "https://test-api"
 CURRENT_TIME = datetime.datetime.utcnow()
 
 
 @pytest.fixture
 def test_api_client():
@@ -105,21 +105,18 @@
 
 
 def test_create_dataset(test_api_client):
     application = Application(name="test_application_name", api_client=test_api_client)
     m = mock.Mock()
     with mock.patch("gantry.dataset.main._DATASET", m):
         getattr(m, "create_dataset").return_value = "return_value"
-        result = application.create_dataset(
-            name="test_dataset_name", bucket_name="test-dataset-bucket"
-        )
+        result = application.create_dataset(name="test_dataset_name")
         assert result == "return_value"
         getattr(m, "create_dataset").assert_called_once_with(
             name="test_dataset_name",
-            bucket_name="test-dataset-bucket",
             app_name="test_application_name",
         )
 
 
 def test_list_datasets(test_api_client):
     application = Application(name="test_application_name", api_client=test_api_client)
     m = mock.Mock()
@@ -303,14 +300,28 @@
                     "end_time": CURRENT_TIME.isoformat(),
                     "filters": [{"feature_name": "inputs.A", "lower_bound": 0, "upper_bound": 10}],
                     "tags": [{"tag_name": "query", "tag_value": "test"}],
                 },
             },
             headers={"Content-Type": "application/json"},
         )
+        resp.add(
+            resp.GET,
+            f"{HOST}/api/v1/applications/{application._id}/queries/test_query",
+            json={
+                "response": "ok",
+                "data": {
+                    "start_time": (CURRENT_TIME - datetime.timedelta(days=1)).isoformat(),
+                    "end_time": CURRENT_TIME.isoformat(),
+                    "filters": [{"feature_name": "inputs.A", "lower_bound": 0, "upper_bound": 5}],
+                    "tags": [{"tag_name": "query", "tag_value": "test"}],
+                },
+            },
+            headers={"Content-Type": "application/json"},
+        )
         actual_query = application.query(
             time_window=TimeWindow(
                 start_time=CURRENT_TIME - datetime.timedelta(days=1),
                 end_time=CURRENT_TIME,
             ),
             version=None,
             env=None,
@@ -339,13 +350,140 @@
             headers={"Content-Type": "application/json"},
         )
         actual_query = application.query(
             time_window=TimeWindow(
                 start_time=CURRENT_TIME - datetime.timedelta(days=1), end_time=CURRENT_TIME
             ),
             version=None,
-            env="test",
+            env=None,
+            filters=[{"feature_name": "inputs.A", "lower_bound": 0, "upper_bound": 5}],
+            tags={"query": "test"},
+        )
+        application.save_query(name="test_query", query=actual_query)
+        new_saved_query = application.get_query(name="test_query")
+        assert new_saved_query.version == actual_query.version
+        assert new_saved_query.env == actual_query.env
+        assert new_saved_query.filters == actual_query.filters
+        assert new_saved_query.tags == actual_query.tags
+
+
+def test_save_query_with_duration_time_frame(test_api_client):
+    application = Application(name="test_application_name", api_client=test_api_client)
+    assert application._name == "test_application_name"
+
+    with responses.RequestsMock() as resp:
+        resp.add(
+            resp.GET,
+            f"{HOST}/api/v1/models/{application._name}/schemas",
+            json={
+                "response": "ok",
+                "data": {"id": str(application._id)},
+            },
+            headers={"Content-Type": "application/json"},
+        )
+        resp.add(
+            resp.POST,
+            f"{HOST}/api/v1/queries",
+            json={
+                "response": "ok",
+                "data": {"query": "test"},
+            },
+            headers={"Content-Type": "application/json"},
+        )
+        resp.add(
+            resp.PATCH,
+            f"{HOST}/api/v1/queries",
+            json={
+                "response": "ok",
+            },
+            headers={"Content-Type": "application/json"},
+        )
+        resp.add(
+            resp.GET,
+            f"{HOST}/api/v1/applications/{application._id}/queries",
+            json={
+                "response": "ok",
+                "data": [],
+            },
+            headers={"Content-Type": "application/json"},
+        )
+        resp.add(
+            resp.GET,
+            f"{HOST}/api/v1/applications/{application._id}/queries/test_query",
+            json={
+                "response": "ok",
+                "data": {
+                    "start_time": (CURRENT_TIME - datetime.timedelta(days=1)).isoformat(),
+                    "end_time": CURRENT_TIME.isoformat(),
+                    "relative_time_window": "P1D",
+                    "relative_time_delay": "P1D",
+                    "filters": [{"feature_name": "inputs.A", "lower_bound": 0, "upper_bound": 10}],
+                    "tags": [{"tag_name": "query", "tag_value": "test"}],
+                },
+            },
+            headers={"Content-Type": "application/json"},
+        )
+        resp.add(
+            resp.GET,
+            f"{HOST}/api/v1/applications/{application._id}/queries/test_query",
+            json={
+                "response": "ok",
+                "data": {
+                    "start_time": (CURRENT_TIME - datetime.timedelta(days=2)).isoformat(),
+                    "end_time": CURRENT_TIME.isoformat(),
+                    "relative_time_window": "P2D",
+                    "relative_time_delay": "P1D",
+                    "filters": [{"feature_name": "inputs.A", "lower_bound": 0, "upper_bound": 5}],
+                    "tags": [{"tag_name": "query", "tag_value": "test"}],
+                },
+            },
+            headers={"Content-Type": "application/json"},
+        )
+        actual_query = application.query(
+            time_window=RelativeTimeWindow(
+                window_length=datetime.timedelta(days=1), offset=datetime.timedelta(days=1)
+            ),
+            version=None,
+            env=None,
+            filters=[{"feature_name": "inputs.A", "lower_bound": 0, "upper_bound": 10}],
+            tags={"query": "test"},
+        )
+        application.save_query(name="test_query", query=actual_query)
+        saved_query = application.get_query(name="test_query")
+        # Timezone difference, but the assert is still correct
+        # assert saved_query.start_time == actual_query.start_time
+        # assert saved_query.end_time == actual_query.end_time
+        assert saved_query.version == actual_query.version
+        assert saved_query.env == actual_query.env
+        assert saved_query.filters == actual_query.filters
+        assert saved_query.tags == actual_query.tags
+        assert saved_query.relative_time_window == datetime.timedelta(days=1)
+        assert saved_query.relative_time_delay == datetime.timedelta(days=1)
+
+        # Add a mock response that there is a query with the same name in the list
+        # to test if it updates the query instead of saving.
+        resp.add(
+            resp.GET,
+            f"{HOST}/api/v1/applications/{application._id}/queries",
+            json={
+                "response": "ok",
+                "data": [{"name": "test_query", "query": "test"}],
+            },
+            headers={"Content-Type": "application/json"},
+        )
+        actual_query = application.query(
+            time_window=RelativeTimeWindow(
+                window_length=datetime.timedelta(days=2), offset=datetime.timedelta(days=1)
+            ),
+            version=None,
+            env=None,
             filters=[{"feature_name": "inputs.A", "lower_bound": 0, "upper_bound": 5}],
             tags={"query": "test"},
         )
         application.save_query(name="test_query", query=actual_query)
-        application.get_query(name="test_query")
+        saved_query = application.get_query(name="test_query")
+        assert saved_query.version == actual_query.version
+        assert saved_query.env == actual_query.env
+        assert saved_query.filters == actual_query.filters
+        assert saved_query.tags == actual_query.tags
+        assert saved_query.relative_time_window == datetime.timedelta(days=2)
+        assert saved_query.relative_time_delay == datetime.timedelta(days=1)
```

### Comparing `gantry-0.6.7/tests/applications/test_llm.py` & `gantry-0.6.8/tests/applications/test_llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,14 +280,19 @@
         with caplog.at_level(logging.WARNING):
             test_version = test_llm_application.get_version(version)  # type: ignore
 
     assert "No version found" in caplog.text
     assert test_version is None
 
 
+def test_get_version_error(test_llm_application: CompletionApplication):
+    with pytest.raises(ValueError):
+        test_llm_application.get_version("invalid version")  # type: ignore
+
+
 def test_log_completion(test_llm_application: CompletionApplication, caplog):
     test_llm_application.log_completion(
         open_ai_api_request={"request": "foo"},
         open_ai_api_response={"response": "bar"},
         request_attributes={"foo": "bar"},
         response_attributes={"bar": "baz"},
         feedback={"foo": "baz"},
```

### Comparing `gantry-0.6.7/tests/applications/test_llm_utils.py` & `gantry-0.6.8/tests/applications/test_llm_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/cli/test_bucket.py` & `gantry-0.6.8/tests/cli/test_bucket.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/cli/test_data_connector.py` & `gantry-0.6.8/tests/cli/test_data_connector.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/cli/test_labeling.py` & `gantry-0.6.8/tests/cli/test_labeling.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/cli/test_projection.py` & `gantry-0.6.8/tests/cli/test_projection.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/cli/test_secrets.py` & `gantry-0.6.8/tests/cli/test_secrets.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/conftest.py` & `gantry-0.6.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/curator/conftest.py` & `gantry-0.6.8/tests/curator/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/curator/test_curator.py` & `gantry-0.6.8/tests/curator/test_curator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/curator/test_main.py` & `gantry-0.6.8/tests/curator/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/curator/test_selectors.py` & `gantry-0.6.8/tests/curator/test_selectors.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/data_generator/test_data_generator.py` & `gantry-0.6.8/tests/data_generator/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/dataset/conftest.py` & `gantry-0.6.8/tests/dataset/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/dataset/test_client.py` & `gantry-0.6.8/tests/dataset/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/dataset/test_gantry_dataset.py` & `gantry-0.6.8/tests/dataset/test_gantry_dataset.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/dataset/test_main.py` & `gantry-0.6.8/tests/dataset/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/logger/test_client.py` & `gantry-0.6.8/tests/logger/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/logger/test_consumer.py` & `gantry-0.6.8/tests/logger/test_consumer.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/logger/test_event_builder.py` & `gantry-0.6.8/tests/logger/test_event_builder.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/logger/test_main.py` & `gantry-0.6.8/tests/logger/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/logger/test_stores.py` & `gantry-0.6.8/tests/logger/test_stores.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/logger/test_utils.py` & `gantry-0.6.8/tests/logger/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/query/conftest.py` & `gantry-0.6.8/tests/query/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/query/core/test_dataframe.py` & `gantry-0.6.8/tests/query/core/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/query/core/test_distance.py` & `gantry-0.6.8/tests/query/core/test_distance.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/query/core/test_filters.py` & `gantry-0.6.8/tests/query/core/test_filters.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/query/core/test_metric.py` & `gantry-0.6.8/tests/query/core/test_metric.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/query/core/test_queryframe.py` & `gantry-0.6.8/tests/query/core/test_queryframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/query/core/test_series.py` & `gantry-0.6.8/tests/query/core/test_series.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/query/core/test_utils.py` & `gantry-0.6.8/tests/query/core/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 @pytest.mark.parametrize(
     ["supported", "valid"],
     [
         (["bool"], "bool"),
         (["bool", "int"], "int"),
         (["str", "float"], "float"),
         (["str", "float"], "str"),
+        (["float", "int", "tag"], "tag"),
     ],
 )
 def test_runs_on_valid(supported, valid):
     dec = runs_on(*supported)
     f = dec(lambda m: True)
     assert f(mock.Mock(dtype=valid))
```

### Comparing `gantry-0.6.7/tests/query/distance/test_main.py` & `gantry-0.6.8/tests/query/distance/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/query/metric/test_main.py` & `gantry-0.6.8/tests/query/metric/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/query/test_client.py` & `gantry-0.6.8/tests/query/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/query/test_main.py` & `gantry-0.6.8/tests/query/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/test_api_client.py` & `gantry-0.6.8/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/test_init.py` & `gantry-0.6.8/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/test_utils.py` & `gantry-0.6.8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.7/tests/test_validator.py` & `gantry-0.6.8/tests/test_validator.py`

 * *Files identical despite different names*

