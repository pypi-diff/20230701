# Comparing `tmp/bioblend-1.1.1.tar.gz` & `tmp/bioblend-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioblend-1.1.1.tar", last modified: Tue Feb 21 15:49:35 2023, max compression
+gzip compressed data, was "bioblend-1.2.0.tar", last modified: Fri Jun 30 22:50:07 2023, max compression
```

## Comparing `bioblend-1.1.1.tar` & `bioblend-1.2.0.tar`

### file list

```diff
@@ -1,158 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.664031 bioblend-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-02-21 15:49:14.000000 bioblend-1.1.1/ABOUT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-02-21 15:49:14.000000 bioblend-1.1.1/CITATION
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-02-21 15:49:14.000000 bioblend-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-02-21 15:49:14.000000 bioblend-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-02-21 15:49:35.664031 bioblend-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-02-21 15:49:14.000000 bioblend-1.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.652031 bioblend-1.1.1/bioblend/
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.656031 bioblend-1.1.1/bioblend/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/GalaxyTestBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/README.TXT
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/TestGalaxyConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/TestGalaxyDatasetCollections.py
--rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/TestGalaxyDatasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/TestGalaxyFolders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/TestGalaxyGroups.py
--rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/TestGalaxyHistories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/TestGalaxyInstance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/TestGalaxyInvocations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10426 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/TestGalaxyJobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/TestGalaxyLibraries.py
--rw-r--r--   0 runner    (1001) docker     (123)    39951 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/TestGalaxyObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/TestGalaxyQuotas.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/TestGalaxyRoles.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/TestGalaxyToolData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/TestGalaxyToolDependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/TestGalaxyToolInputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/TestGalaxyTools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/TestGalaxyUsers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/TestGalaxyWorkflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/TestToolshed.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/_tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/data/1.bed
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/data/Galaxy-History-Test-history-for-export.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/data/paste_columns.ga
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/data/paste_columns_collections.ga
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/data/paste_columns_subworkflow.ga
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/data/select_first.ga
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/data/test_workflow_pause.ga
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/data/workflow_with_parameter_input.ga
--rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/pytest_galaxy_test_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/template_galaxy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/template_galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/_tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/dataset_collections/
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/dataset_collections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)    17031 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/folders/
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/folders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/forms/
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/forms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/ftpfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/ftpfiles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/genomes/
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/genomes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/groups/
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/groups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/histories/
--rw-r--r--   0 runner    (1001) docker     (123)    31954 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/histories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/invocations/
--rw-r--r--   0 runner    (1001) docker     (123)    17574 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/invocations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)    18001 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/jobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/libraries/
--rw-r--r--   0 runner    (1001) docker     (123)    27793 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/libraries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/objects/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20315 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/objects/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/objects/galaxy_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    63473 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/objects/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/quotas/
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/quotas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/roles/
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/roles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/tool_data/
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/tool_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/tool_dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/tool_dependencies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/tools/
--rw-r--r--   0 runner    (1001) docker     (123)    22359 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/tools/inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/toolshed/
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/toolshed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/users/
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/users/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/visual/
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/visual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/galaxy/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)    30065 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxy/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/galaxyclient.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/toolshed/
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/toolshed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/toolshed/categories/
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/toolshed/categories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.660031 bioblend-1.1.1/bioblend/toolshed/repositories/
--rw-r--r--   0 runner    (1001) docker     (123)    23149 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/toolshed/repositories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.664031 bioblend-1.1.1/bioblend/toolshed/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/toolshed/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.664031 bioblend-1.1.1/bioblend/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-02-21 15:49:14.000000 bioblend-1.1.1/bioblend/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.652031 bioblend-1.1.1/bioblend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-02-21 15:49:35.000000 bioblend-1.1.1/bioblend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-02-21 15:49:35.000000 bioblend-1.1.1/bioblend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 15:49:35.000000 bioblend-1.1.1/bioblend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-21 15:49:35.000000 bioblend-1.1.1/bioblend.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-21 15:49:35.000000 bioblend-1.1.1/bioblend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-21 15:49:35.000000 bioblend-1.1.1/bioblend.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.664031 bioblend-1.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.664031 bioblend-1.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/_static/.empty
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.664031 bioblend-1.1.1/docs/api_docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.664031 bioblend-1.1.1/docs/api_docs/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/api_docs/galaxy/all.rst
--rw-r--r--   0 runner    (1001) docker     (123)    19720 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/api_docs/galaxy/docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/api_docs/lib_config.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.664031 bioblend-1.1.1/docs/api_docs/toolshed/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/api_docs/toolshed/all.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.664031 bioblend-1.1.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/examples/create_user_get_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/examples/list_data_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/examples/list_histories.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/examples/list_workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.664031 bioblend-1.1.1/docs/examples/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/examples/objects/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/examples/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/examples/objects/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/examples/objects/list_data_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/examples/objects/list_histories.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/examples/objects/list_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/examples/objects/small.ga
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/examples/objects/small.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/examples/objects/w2_bacterial_reseq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/examples/objects/w3_bacterial_denovo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/examples/objects/w5_galaxy_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/examples/objects/w5_metagenomics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/examples/run_imported_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/examples/tophat_cufflinks_pairedend_workflow.ga
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-21 15:49:14.000000 bioblend-1.1.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-21 15:49:14.000000 bioblend-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-02-21 15:49:35.668031 bioblend-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 15:49:14.000000 bioblend-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 15:49:35.664031 bioblend-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-02-21 15:49:14.000000 bioblend-1.1.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.508705 bioblend-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-30 22:49:48.000000 bioblend-1.2.0/ABOUT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-30 22:49:48.000000 bioblend-1.2.0/CITATION
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-30 22:49:48.000000 bioblend-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-30 22:49:48.000000 bioblend-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-30 22:50:07.508705 bioblend-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-30 22:49:48.000000 bioblend-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.488704 bioblend-1.2.0/bioblend/
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/GalaxyTestBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/README.TXT
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyDatasetCollections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyFolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyGroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12630 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyHistories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyInstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyInvocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyJobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyLibraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39904 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyQuotas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyRoles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyToolContainerResolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyToolData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyToolDependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyToolInputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyUsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestGalaxyWorkflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/TestToolshed.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/_tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/data/1.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/data/Galaxy-History-Test-history-for-export.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/data/paste_columns.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/data/paste_columns_collections.ga
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/data/paste_columns_subworkflow.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/data/select_first.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/data/test_workflow_pause.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/data/workflow_with_parameter_input.ga
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/pytest_galaxy_test_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/template_galaxy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/template_galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/_tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/container_resolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/container_resolution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/dataset_collections/
+-rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/dataset_collections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/folders/
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/folders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/forms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/ftpfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/ftpfiles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/genomes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/genomes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/groups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.492704 bioblend-1.2.0/bioblend/galaxy/histories/
+-rw-r--r--   0 runner    (1001) docker     (123)    31835 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/histories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/invocations/
+-rw-r--r--   0 runner    (1001) docker     (123)    17574 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/invocations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/jobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/libraries/
+-rw-r--r--   0 runner    (1001) docker     (123)    27818 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/libraries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20315 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/objects/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/objects/galaxy_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63473 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/objects/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/quotas/
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/quotas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/roles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/tool_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/tool_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/tool_dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/tool_dependencies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    23017 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/tools/inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/toolshed/
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/toolshed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/users/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.496704 bioblend-1.2.0/bioblend/galaxy/visual/
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/visual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.500704 bioblend-1.2.0/bioblend/galaxy/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)    30065 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxy/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13202 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/galaxyclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.500704 bioblend-1.2.0/bioblend/toolshed/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/toolshed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.500704 bioblend-1.2.0/bioblend/toolshed/categories/
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/toolshed/categories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.500704 bioblend-1.2.0/bioblend/toolshed/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)    23149 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/toolshed/repositories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.500704 bioblend-1.2.0/bioblend/toolshed/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/toolshed/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.500704 bioblend-1.2.0/bioblend/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-30 22:49:48.000000 bioblend-1.2.0/bioblend/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.488704 bioblend-1.2.0/bioblend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-30 22:50:07.000000 bioblend-1.2.0/bioblend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-30 22:50:07.000000 bioblend-1.2.0/bioblend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:50:07.000000 bioblend-1.2.0/bioblend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-30 22:50:07.000000 bioblend-1.2.0/bioblend.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 22:50:07.000000 bioblend-1.2.0/bioblend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 22:50:07.000000 bioblend-1.2.0/bioblend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.500704 bioblend-1.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.500704 bioblend-1.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/_static/.empty
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.500704 bioblend-1.2.0/docs/api_docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.504705 bioblend-1.2.0/docs/api_docs/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/api_docs/galaxy/all.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19720 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/api_docs/galaxy/docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/api_docs/lib_config.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.504705 bioblend-1.2.0/docs/api_docs/toolshed/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/api_docs/toolshed/all.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.504705 bioblend-1.2.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/create_user_get_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/list_data_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/list_histories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/list_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.508705 bioblend-1.2.0/docs/examples/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/list_data_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/list_histories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/list_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/small.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/small.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/w2_bacterial_reseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/w3_bacterial_denovo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/w5_galaxy_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/objects/w5_metagenomics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/run_imported_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/examples/tophat_cufflinks_pairedend_workflow.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 22:49:48.000000 bioblend-1.2.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-30 22:49:48.000000 bioblend-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-30 22:50:07.508705 bioblend-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 22:49:48.000000 bioblend-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:50:07.508705 bioblend-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-30 22:49:48.000000 bioblend-1.2.0/tests/test_util.py
```

### Comparing `bioblend-1.1.1/ABOUT.rst` & `bioblend-1.2.0/ABOUT.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 `BioBlend <https://bioblend.readthedocs.io/>`_ is a Python library for
 interacting with the `Galaxy`_ API.
 
 BioBlend is supported and tested on:
 
 - Python 3.7 - 3.11
-- Galaxy release 17.09 and later.
+- Galaxy release 19.05 and later.
 
 BioBlend's goal is to make it easier to script and automate the running of
 Galaxy analyses and administering of a Galaxy server.
 In practice, it makes it possible to do things like this:
 
 - Interact with Galaxy via a straightforward API::
```

### Comparing `bioblend-1.1.1/CITATION` & `bioblend-1.2.0/CITATION`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/LICENSE` & `bioblend-1.2.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2012-2020 Galaxy Project
+Copyright (c) 2012-2023 Galaxy Project
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `bioblend-1.1.1/PKG-INFO` & `bioblend-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioblend
-Version: 1.1.1
+Version: 1.2.0
 Summary: Library for interacting with the Galaxy API
 Home-page: https://bioblend.readthedocs.io/
 Author: Enis Afgan
 Author-email: afgane@gmail.com
 Maintainer: Nicola Soranzo
 Maintainer-email: nicola.soranzo@earlham.ac.uk
 License: MIT
@@ -42,14 +42,14 @@
 
 
 BioBlend is a Python library for interacting with the `Galaxy`_ API.
 
 BioBlend is supported and tested on:
 
 - Python 3.7 - 3.11
-- Galaxy release 17.09 and later.
+- Galaxy release 19.05 and later.
 
 Full docs are available at https://bioblend.readthedocs.io/ with a quick library
 overview also available in `ABOUT.rst <./ABOUT.rst>`_.
 
 .. References/hyperlinks used above
 .. _Galaxy: https://galaxyproject.org/
```

### Comparing `bioblend-1.1.1/README.rst` & `bioblend-1.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 
 
 BioBlend is a Python library for interacting with the `Galaxy`_ API.
 
 BioBlend is supported and tested on:
 
 - Python 3.7 - 3.11
-- Galaxy release 17.09 and later.
+- Galaxy release 19.05 and later.
 
 Full docs are available at https://bioblend.readthedocs.io/ with a quick library
 overview also available in `ABOUT.rst <./ABOUT.rst>`_.
 
 .. References/hyperlinks used above
 .. _Galaxy: https://galaxyproject.org/
```

### Comparing `bioblend-1.1.1/bioblend/__init__.py` & `bioblend-1.2.0/bioblend/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from bioblend.config import (
     BioBlendConfigLocations,
     Config,
 )
 
 # Current version of the library
-__version__ = "1.1.1"
+__version__ = "1.2.0"
 
 # default chunk size (in bytes) for reading remote data
 try:
     import resource
 
     CHUNK_SIZE = resource.getpagesize()
 except Exception:
```

### Comparing `bioblend-1.1.1/bioblend/_tests/GalaxyTestBase.py` & `bioblend-1.2.0/bioblend/_tests/GalaxyTestBase.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/README.TXT` & `bioblend-1.2.0/bioblend/_tests/README.TXT`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/TestGalaxyDatasetCollections.py` & `bioblend-1.2.0/bioblend/_tests/TestGalaxyDatasetCollections.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,15 @@
     Any,
     Dict,
     Union,
 )
 from zipfile import ZipFile
 
 from bioblend.galaxy import dataset_collections
-from . import (
-    GalaxyTestBase,
-    test_util,
-)
+from . import GalaxyTestBase
 
 
 class TestGalaxyDatasetCollections(GalaxyTestBase.GalaxyTestBase):
     def test_create_list_in_history(self):
         history_id = self.gi.histories.create_history(name="TestDSListCreate")["id"]
         dataset1_id = self._test_dataset(history_id)
         dataset2_id = self._test_dataset(history_id)
@@ -149,15 +146,14 @@
             assert dataset_collection1[key] == dataset_collection2[key]
         for element1, element2 in zip(dataset_collection1["elements"], dataset_collection2["elements"]):
             assert element1["id"] == element2["id"]
             assert element1.keys() == element2.keys()
             for key in element1["object"].keys():
                 assert key in element2["object"].keys()
 
-    @test_util.skip_unless_galaxy("release_18.01")
     def test_download_dataset_collection(self):
         history_id = self.gi.histories.create_history(name="TestDatasetCollectionDownload")["id"]
         dataset_collection_id = self._create_pair_in_history(history_id)["id"]
         self.gi.dataset_collections.wait_for_dataset_collection(dataset_collection_id)
 
         tempdir = tempfile.mkdtemp(prefix="bioblend_test_dataset_collection_download_")
         archive_path = os.path.join(tempdir, "dataset_collection")
```

### Comparing `bioblend-1.1.1/bioblend/_tests/TestGalaxyDatasets.py` & `bioblend-1.2.0/bioblend/_tests/TestGalaxyDatasets.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/TestGalaxyFolders.py` & `bioblend-1.2.0/bioblend/_tests/TestGalaxyFolders.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/TestGalaxyGroups.py` & `bioblend-1.2.0/bioblend/_tests/TestGalaxyGroups.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/TestGalaxyHistories.py` & `bioblend-1.2.0/bioblend/_tests/TestGalaxyHistories.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,14 @@
         self._wait_and_verify_dataset(dataset1_id, b"1\t2\t3\n")
         original_hda = self.gi.datasets.show_dataset(dataset1_id)
         assert original_hda["extension"] == "bed"
         self.gi.histories.update_dataset(history_id, dataset1_id, datatype="tabular")
         updated_hda = self.gi.datasets.show_dataset(dataset1_id)
         assert updated_hda["extension"] == "tabular"
 
-    @test_util.skip_unless_galaxy("release_19.01")
     def test_get_extra_files(self):
         history_id = self.history["id"]
         dataset_id = self._test_dataset(history_id)
         extra_files = self.gi.histories.get_extra_files(history_id, dataset_id)
         assert extra_files == []
 
     def tearDown(self):
```

### Comparing `bioblend-1.1.1/bioblend/_tests/TestGalaxyInstance.py` & `bioblend-1.2.0/bioblend/_tests/TestGalaxyInstance.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,22 @@
 
 
 class TestGalaxyInstance(unittest.TestCase):
     def setUp(self):
         # "connect" to a fake Galaxy instance
         self.gi = GalaxyInstance("http://localhost:56789", key="whatever")
 
+    def test_url_attribute(self):
+        assert self.gi.base_url == "http://localhost:56789"
+        assert self.gi.url == "http://localhost:56789/api"
+        # Test instance served at a subdirectory
+        gi = GalaxyInstance("http://localhost:56789/galaxy/", key="whatever")
+        assert gi.base_url == "http://localhost:56789/galaxy"
+        assert gi.url == "http://localhost:56789/galaxy/api"
+
     def test_set_max_get_attempts(self):
         self.gi.max_get_attempts = 3
         assert 3 == self.gi.max_get_attempts
 
     def test_set_retry_delay(self):
         self.gi.get_retry_delay = 5.0
         assert 5.0 == self.gi.get_retry_delay
```

### Comparing `bioblend-1.1.1/bioblend/_tests/TestGalaxyInvocations.py` & `bioblend-1.2.0/bioblend/_tests/TestGalaxyInvocations.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,16 @@
 
         invocation_id = invocation["id"]
         workflow_id = invocation["workflow_id"]
         report = self.gi.invocations.get_invocation_report(invocation_id)
         assert report["workflows"] == {workflow_id: {"name": "paste_columns"}}
         with contextlib.suppress(Exception):
             # This can fail if dependencies as weasyprint are not installed on the Galaxy server
-            self.gi.invocations.get_invocation_report_pdf(invocation_id, "report.pdf")
+            ret = self.gi.invocations.get_invocation_report_pdf(invocation_id, "report.pdf")
+            assert ret is None
 
     @test_util.skip_unless_galaxy("release_20.09")
     def test_get_invocation_biocompute_object(self):
         invocation = self._invoke_workflow()
 
         self.gi.invocations.wait_for_invocation(invocation["id"])
         biocompute_object = self.gi.invocations.get_invocation_biocompute_object(invocation["id"])
```

### Comparing `bioblend-1.1.1/bioblend/_tests/TestGalaxyJobs.py` & `bioblend-1.2.0/bioblend/_tests/TestGalaxyJobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,14 @@
         # in https://github.com/galaxyproject/galaxy/commit/3e7f03cd1f229b8c9421ade02002728a33e131d8
         self.gi.jobs.wait_for_job(job_id)
         response = self.gi.jobs.get_destination_params(job_id)
         assert "Runner" in response
         assert "Runner Job ID" in response
         assert "Handler" in response
 
-    @test_util.skip_unless_galaxy("release_18.01")
     @test_util.skip_unless_tool("random_lines1")
     def test_search_jobs(self):
         job_id = self._run_tool()["jobs"][0]["id"]
         inputs = {
             "num_lines": "1",
             "input": {"src": "hda", "id": self.dataset_id},
             "seed_source|seed_source_selector": "set_seed",
@@ -215,15 +214,14 @@
     @test_util.skip_unless_galaxy("release_20.05")
     def test_update_job_lock(self):
         status = self.gi.jobs.update_job_lock(active=True)
         assert status
         status = self.gi.jobs.update_job_lock(active=False)
         assert not status
 
-    @test_util.skip_unless_galaxy("release_18.01")
     def test_cancel_job(self):
         job_id = self._run_tool()["jobs"][0]["id"]
         self.gi.jobs.cancel_job(job_id)
         job = self.gi.jobs.wait_for_job(job_id, check=False)
         assert job["state"] in ("deleted", "deleting")
 
     def _run_tool(self, input_format: Literal["21.01", "legacy"] = "legacy") -> dict:
```

### Comparing `bioblend-1.1.1/bioblend/_tests/TestGalaxyLibraries.py` & `bioblend-1.2.0/bioblend/_tests/TestGalaxyLibraries.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/TestGalaxyObjects.py` & `bioblend-1.2.0/bioblend/_tests/TestGalaxyObjects.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         self.w.a = 222
         self.w.b[0] = 222
         assert self.w.a == 222
         assert self.w.b[0] == 222
         assert self.d["a"] == 1
         assert self.d["b"][0] == 2
         with pytest.raises(AttributeError):
-            self.w.foo  # type: ignore[attr-defined]
+            _ = self.w.foo  # type: ignore[attr-defined]
         with pytest.raises(AttributeError):
             self.w.foo = 0  # type: ignore[assignment]
 
     def test_taint(self):
         assert not self.w.is_modified
         self.w.a = 111  # pylint: disable=W0201
         assert self.w.is_modified
@@ -498,15 +498,14 @@
         self._check_and_del_workflow(wf)
 
     def test_workflow_collections_from_str(self):
         with open(SAMPLE_WF_COLL_FN) as f:
             wf = self.gi.workflows.import_new(f.read())
         self._check_and_del_workflow(wf)
 
-    @test_util.skip_unless_galaxy("release_19.01")
     def test_workflow_parameter_input(self):
         with open(SAMPLE_WF_PARAMETER_INPUT_FN) as f:
             self.gi.workflows.import_new(f.read())
 
     def test_workflow_from_dict(self):
         with open(SAMPLE_FN) as f:
             wf = self.gi.workflows.import_new(json.load(f))
```

### Comparing `bioblend-1.1.1/bioblend/_tests/TestGalaxyQuotas.py` & `bioblend-1.2.0/bioblend/_tests/TestGalaxyQuotas.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/TestGalaxyRoles.py` & `bioblend-1.2.0/bioblend/_tests/TestGalaxyRoles.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/TestGalaxyToolData.py` & `bioblend-1.2.0/bioblend/_tests/TestGalaxyToolData.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/TestGalaxyToolInputs.py` & `bioblend-1.2.0/bioblend/_tests/TestGalaxyToolInputs.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/TestGalaxyTools.py` & `bioblend-1.2.0/bioblend/_tests/TestGalaxyTools.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/TestGalaxyUsers.py` & `bioblend-1.2.0/bioblend/_tests/TestGalaxyUsers.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/TestGalaxyWorkflows.py` & `bioblend-1.2.0/bioblend/_tests/TestGalaxyWorkflows.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,14 @@
                 break
 
             time.sleep(0.5)
 
         invocation = self.gi.workflows.show_invocation(workflow_id, invocation_id)
         assert invocation["state"] == "scheduled"
 
-    @test_util.skip_unless_galaxy("release_19.01")
     def test_invoke_workflow_parameters_normalized(self):
         path = test_util.get_abspath(os.path.join("data", "paste_columns_subworkflow.ga"))
         workflow_id = self.gi.workflows.import_workflow_from_local_path(path)["id"]
         history_id = self.gi.histories.create_history(name="TestWorkflowInvokeParametersNormalized")["id"]
         dataset_id = self._test_dataset(history_id)
         with pytest.raises(ConnectionError):
             self.gi.workflows.invoke_workflow(
@@ -85,14 +84,15 @@
         self.gi.workflows.invoke_workflow(
             workflow_id,
             inputs={"0": {"src": "hda", "id": dataset_id}},
             params={"1": {"1|2": "comma"}},
             parameters_normalized=True,
         )
 
+    @test_util.skip_unless_galaxy("release_19.09")
     @test_util.skip_unless_tool("cat1")
     @test_util.skip_unless_tool("cat")
     def test_cancelling_workflow_scheduling(self):
         path = test_util.get_abspath(os.path.join("data", "test_workflow_pause.ga"))
         workflow = self.gi.workflows.import_workflow_from_local_path(path)
         workflow_id = workflow["id"]
         history_id = self.gi.histories.create_history(name="TestWorkflowState")["id"]
@@ -110,15 +110,15 @@
         assert len(invocations) == 1
         assert invocations[0]["id"] == invocation_id
 
         invocation = self.gi.workflows.show_invocation(workflow_id, invocation_id)
         assert invocation["state"] in ["new", "ready"]
 
         self.gi.workflows.cancel_invocation(workflow_id, invocation_id)
-        invocation = self.gi.workflows.show_invocation(workflow_id, invocation_id)
+        invocation = self.gi.invocations.wait_for_invocation(invocation_id, check=False)
         assert invocation["state"] == "cancelled"
 
     def test_import_export_workflow_from_local_path(self):
         with pytest.raises(TypeError):
             self.gi.workflows.import_workflow_from_local_path(None)  # type: ignore[arg-type]
         path = test_util.get_abspath(os.path.join("data", "paste_columns.ga"))
         imported_wf = self.gi.workflows.import_workflow_from_local_path(path)
@@ -190,15 +190,14 @@
         wf_data = self.gi.workflows.show_workflow(wf["id"])
         assert wf_data["id"] == wf["id"]
         assert wf_data["name"] == wf["name"]
         assert wf_data["url"] == wf["url"]
         assert len(wf_data["steps"]) == 3
         assert wf_data["inputs"] is not None
 
-    @test_util.skip_unless_galaxy("release_18.05")
     def test_update_workflow_name(self):
         path = test_util.get_abspath(os.path.join("data", "paste_columns.ga"))
         wf = self.gi.workflows.import_workflow_from_local_path(path)
         new_name = "new name"
         updated_wf = self.gi.workflows.update_workflow(wf["id"], name=new_name)
         assert updated_wf["name"] == new_name
 
@@ -264,15 +263,14 @@
         wf2 = self.gi.workflows.show_workflow(wf2["id"])
         assert wf2["name"] == new_workflow_name
         assert len(wf1["steps"]) == len(wf2["steps"])
         for i in range(len(wf1["steps"])):
             assert wf1["steps"][str(i)]["type"] == wf2["steps"][str(i)]["type"]
             assert wf1["steps"][str(i)]["tool_id"] == wf2["steps"][str(i)]["tool_id"]
 
-    @test_util.skip_unless_galaxy("release_18.09")
     def test_show_versions(self):
         path = test_util.get_abspath(os.path.join("data", "paste_columns.ga"))
         wf = self.gi.workflows.import_workflow_from_local_path(path)
         versions = self.gi.workflows.show_versions(wf["id"])
         assert len(versions) == 1
         version = versions[0]
         assert version["version"] == 0
```

### Comparing `bioblend-1.1.1/bioblend/_tests/TestToolshed.py` & `bioblend-1.2.0/bioblend/_tests/TestToolshed.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/data/1.bed` & `bioblend-1.2.0/bioblend/_tests/data/1.bed`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/data/Galaxy-History-Test-history-for-export.tar.gz` & `bioblend-1.2.0/bioblend/_tests/data/Galaxy-History-Test-history-for-export.tar.gz`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/data/paste_columns.ga` & `bioblend-1.2.0/bioblend/_tests/data/paste_columns.ga`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/data/paste_columns_collections.ga` & `bioblend-1.2.0/bioblend/_tests/data/paste_columns_collections.ga`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/data/paste_columns_subworkflow.ga` & `bioblend-1.2.0/bioblend/_tests/data/paste_columns_subworkflow.ga`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/data/select_first.ga` & `bioblend-1.2.0/bioblend/_tests/data/select_first.ga`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/data/test_workflow_pause.ga` & `bioblend-1.2.0/bioblend/_tests/data/test_workflow_pause.ga`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/data/workflow_with_parameter_input.ga` & `bioblend-1.2.0/bioblend/_tests/data/workflow_with_parameter_input.ga`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/pytest_galaxy_test_wrapper.py` & `bioblend-1.2.0/bioblend/_tests/pytest_galaxy_test_wrapper.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/template_galaxy.ini` & `bioblend-1.2.0/bioblend/_tests/template_galaxy.ini`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/template_galaxy.yml` & `bioblend-1.2.0/bioblend/_tests/template_galaxy.yml`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/_tests/test_util.py` & `bioblend-1.2.0/bioblend/_tests/test_util.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/config.py` & `bioblend-1.2.0/bioblend/config.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/galaxy/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 A base representation of an instance of Galaxy
 """
 from typing import Optional
 
 from bioblend.galaxy import (
     config,
+    container_resolution,
     dataset_collections,
     datasets,
     datatypes,
     folders,
     forms,
     ftpfiles,
     genomes,
@@ -89,14 +90,15 @@
         self.dataset_collections = dataset_collections.DatasetCollectionClient(self)
         self.users = users.UserClient(self)
         self.genomes = genomes.GenomeClient(self)
         self.tools = tools.ToolClient(self)
         self.toolshed = toolshed.ToolShedClient(self)
         self.toolShed = self.toolshed  # historical alias
         self.config = config.ConfigClient(self)
+        self.container_resolution = container_resolution.ContainerResolutionClient(self)
         self.visual = visual.VisualClient(self)
         self.quotas = quotas.QuotaClient(self)
         self.groups = groups.GroupsClient(self)
         self.roles = roles.RolesClient(self)
         self.datatypes = datatypes.DatatypesClient(self)
         self.jobs = jobs.JobsClient(self)
         self.forms = forms.FormsClient(self)
```

### Comparing `bioblend-1.1.1/bioblend/galaxy/client.py` & `bioblend-1.2.0/bioblend/galaxy/client.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/galaxy/config/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/config/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,7 +68,17 @@
              'id': '4aaaaa85aacc9caa',
              'last_password_change': '2021-07-29T05:34:54.632345',
              'model_class': 'User',
              'username': 'julia'}
         """
         url = self.gi.url + "/whoami"
         return self._get(url=url)
+
+    def reload_toolbox(self) -> None:
+        """
+        Reload the Galaxy toolbox (but not individual tools)
+
+        :rtype: None
+        :return: None
+        """
+        url = f"{self._make_url()}/toolbox"
+        return self._put(url=url)
```

### Comparing `bioblend-1.1.1/bioblend/galaxy/dataset_collections/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/dataset_collections/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,14 @@
 
         :rtype: dict
         :return: Information about the downloaded archive.
 
         .. note::
           This method downloads a ``zip`` archive for Galaxy 21.01 and later.
           For earlier versions of Galaxy this method downloads a ``tgz`` archive.
-          This method works only on Galaxy 18.01 or later.
         """
         url = self._make_url(module_id=dataset_collection_id) + "/download"
         r = self.gi.make_get_request(url, stream=True)
         r.raise_for_status()
 
         archive_type = "zip" if self.gi.config.get_version()["version_major"] >= "21.01" else "tgz"
```

### Comparing `bioblend-1.1.1/bioblend/galaxy/datasets/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/datasets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     List,
     Optional,
     overload,
     Tuple,
     TYPE_CHECKING,
     Union,
 )
-from urllib.parse import urljoin
 
 from requests import Response
 from typing_extensions import Literal
 
 import bioblend
 from bioblend import TimeoutException
 from bioblend.galaxy.client import Client
@@ -82,15 +81,15 @@
         # The preferred download URL is
         # '/api/histories/<history_id>/contents/<dataset_id>/display?to_ext=<dataset_ext>'
         # since the old URL:
         # '/dataset/<dataset_id>/display?to_ext=<dataset_ext>'
         # does not work when using REMOTE_USER with access disabled to
         # everything but /api without auth
         download_url = dataset["download_url"] + "?to_ext=" + file_ext
-        url = urljoin(self.gi.base_url, download_url)
+        url = f"{self.gi.base_url}{download_url}"
 
         r = self.gi.make_get_request(url, stream=stream_content)
         r.raise_for_status()
         return dataset, file_ext, r
 
     @overload
     def download_dataset(
```

### Comparing `bioblend-1.1.1/bioblend/galaxy/datatypes/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/galaxy/folders/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/folders/__init__.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/galaxy/forms/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/galaxy/ftpfiles/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/ftpfiles/__init__.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/galaxy/genomes/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/genomes/__init__.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/galaxy/groups/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/galaxy/histories/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/histories/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     IO,
     List,
     Optional,
     overload,
     Pattern,
     Union,
 )
-from urllib.parse import urljoin
 
 from typing_extensions import Literal
 
 import bioblend
 from bioblend import ConnectionError
 from bioblend.galaxy.client import Client
 from bioblend.galaxy.dataset_collections import CollectionDescription
@@ -866,15 +865,15 @@
         .. warning::
           After opening the specified history, all previously opened Galaxy tabs
           in the browser session will have the current history changed to this
           one, even if the interface still shows another history. Refreshing
           any such tab is recommended.
         """
 
-        url = urljoin(self.gi.base_url, f"history/switch_to_history?hist_id={history_id}")
+        url = f"{self.gi.base_url}/history/switch_to_history?hist_id={history_id}"
         webbrowser.open_new_tab(url)
 
     def get_extra_files(self, history_id: str, dataset_id: str) -> List[str]:
         """
         Get extra files associated with a composite dataset, or an empty list if
         there are none.
 
@@ -882,13 +881,10 @@
         :param history_id: history ID
 
         :type dataset_id: str
         :param dataset_id: dataset ID
 
         :rtype: list
         :return: List of extra files
-
-        .. note::
-          This method works only on Galaxy 19.01 or later.
         """
         url = "/".join((self._make_url(history_id, contents=True), dataset_id, "extra_files"))
         return self._get(url=url)
```

### Comparing `bioblend-1.1.1/bioblend/galaxy/invocations/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/invocations/__init__.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/galaxy/jobs/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/jobs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,17 +293,14 @@
         records of jobs with identical input parameters and datasets. This can
         be used to minimize the amount of repeated work by simply recycling the
         old results.
 
         .. versionchanged:: 0.16.0
           Replaced the ``job_info`` parameter with separate ``tool_id``,
           ``inputs`` and ``state``.
-
-        .. note::
-          This method works only on Galaxy 18.01 or later.
         """
         job_info = {
             "tool_id": tool_id,
             "inputs": inputs,
         }
         if state:
             job_info["state"] = state
@@ -424,17 +421,14 @@
         Resume a job if it is paused.
 
         :type job_id: str
         :param job_id: job ID
 
         :rtype: list of dicts
         :return: list of dictionaries containing output dataset associations
-
-        .. note::
-          This method works only on Galaxy 18.09 or later.
         """
         url = self._make_url(module_id=job_id) + "/resume"
         return self._put(url=url)
 
     def get_destination_params(self, job_id: str) -> Dict[str, Any]:
         """
         Get destination parameters for a job, describing
```

### Comparing `bioblend-1.1.1/bioblend/galaxy/libraries/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/libraries/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
     def update_library_dataset(self, dataset_id: str, **kwargs: Any) -> Dict[str, Any]:
         """
         Update library dataset metadata. Some of the attributes that can be
         modified are documented below.
 
         :type dataset_id: str
-        :param dataset_id: id of the dataset to be deleted
+        :param dataset_id: id of the dataset to be updated
 
         :type name: str
         :param name: Replace library dataset name with the given string
 
         :type misc_info: str
         :param misc_info: Replace library dataset misc_info with given string
 
@@ -201,15 +201,15 @@
                     state,
                     time_left,
                 )
                 time.sleep(min(time_left, interval))
                 time_left -= interval
             else:
                 raise DatasetTimeoutException(
-                    f"Waited too long for dataset {dataset_id} in library {library_id} to complete"
+                    f"Dataset {dataset_id} in library {library_id} is still in non-terminal state {state} after {maxwait} s"
                 )
 
     def show_folder(self, library_id: str, folder_id: str) -> Dict[str, Any]:
         """
         Get details about a given folder. The required ``folder_id`` can be
         obtained from the folder's library content details.
```

### Comparing `bioblend-1.1.1/bioblend/galaxy/objects/client.py` & `bioblend-1.2.0/bioblend/galaxy/objects/client.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/galaxy/objects/galaxy_instance.py` & `bioblend-1.2.0/bioblend/galaxy/objects/galaxy_instance.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/galaxy/objects/wrappers.py` & `bioblend-1.2.0/bioblend/galaxy/objects/wrappers.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/galaxy/quotas/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/quotas/__init__.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/galaxy/roles/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/roles/__init__.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/galaxy/tool_data/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/tool_data/__init__.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/galaxy/tool_dependencies/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/tool_dependencies/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 Contains interactions dealing with Galaxy dependency resolvers.
 """
 from typing import (
+    Any,
+    Dict,
     List,
     Optional,
     TYPE_CHECKING,
 )
 
 from typing_extensions import Literal
 
@@ -97,7 +99,26 @@
         if resolver_type:
             params["resolver_type"] = resolver_type
         if container_type:
             params["container_type"] = container_type
 
         url = "/".join((self._make_url(), "toolbox"))
         return self._get(url=url, params=params)
+
+    def unused_dependency_paths(self) -> List[str]:
+        """
+        List unused dependencies
+        """
+        url = "/".join((self._make_url(), "unused_paths"))
+        return self._get(url=url)
+
+    def delete_unused_dependency_paths(self, paths: List[str]) -> None:
+        """
+        Delete unused paths
+
+        :type paths: list
+        :param paths: paths to delete
+
+        """
+        payload: Dict[str, Any] = {"paths": paths}
+        url = "/".join((self._make_url(), "unused_paths"))
+        self._put(url=url, payload=payload)
```

### Comparing `bioblend-1.1.1/bioblend/galaxy/tools/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -329,25 +329,36 @@
 
     def run_tool(
         self,
         history_id: str,
         tool_id: str,
         tool_inputs: Union[InputsBuilder, dict],
         input_format: Literal["21.01", "legacy"] = "legacy",
+        data_manager_mode: Optional[Literal["populate", "dry_run", "bundle"]] = None,
     ) -> Dict[str, Any]:
         """
         Runs tool specified by ``tool_id`` in history indicated
         by ``history_id`` with inputs from ``dict`` ``tool_inputs``.
 
         :type history_id: str
         :param history_id: encoded ID of the history in which to run the tool
 
         :type tool_id: str
         :param tool_id: ID of the tool to be run
 
+        :type data_manager_mode: str
+        :param data_manager_mode: Possible values are 'populate', 'dry_run' and 'bundle'.
+
+          'populate' is the default behavior for data manager tools and results in tool data table
+          files being updated after the data manager job completes.
+
+          'dry_run' will skip any processing after the data manager job completes
+
+          'bundle' will create a data manager bundle that can be imported on other Galaxy servers.
+
         :type tool_inputs: dict
         :param tool_inputs: dictionary of input datasets and parameters
           for the tool (see below)
 
         :type input_format:  string
         :param input_format: input format for the payload. Possible values are the
           default 'legacy' (where inputs nested inside conditionals
@@ -412,14 +423,18 @@
             "input_format": input_format,
         }
 
         if isinstance(tool_inputs, InputsBuilder):
             payload["inputs"] = tool_inputs.to_dict()
         else:
             payload["inputs"] = tool_inputs
+
+        if data_manager_mode:
+            payload["data_manager_mode"] = data_manager_mode
+
         return self._post(payload)
 
     def upload_file(
         self,
         path: str,
         history_id: str,
         storage: Optional[str] = None,
```

### Comparing `bioblend-1.1.1/bioblend/galaxy/tools/inputs.py` & `bioblend-1.2.0/bioblend/galaxy/tools/inputs.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/galaxy/toolshed/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/toolshed/__init__.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/galaxy/users/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/users/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -227,26 +227,35 @@
 
         .. note::
           This method works only on Galaxy 21.01 or later.
         """
         url = self._make_url(user_id) + "/api_key"
         return self._get(url=url)
 
-    def update_user(self, user_id: str, **kwargs: Any) -> Dict[str, Any]:
+    def update_user(self, user_id: str, user_data: Optional[Dict] = None, **kwargs: Any) -> Dict[str, Any]:
         """
-        Update user information. Some of the attributes that can be
-        modified are documented below.
+        Update user information. You can either pass the attributes you want to
+        change in the user_data dictionary, or provide them separately as
+        keyword arguments.
+        For attributes that cannot be expressed as keywords (e.g.
+        extra_user_preferences use a `|` sign), pass them in user_data.
 
         :type user_id: str
         :param user_id: encoded user ID
 
+        :type user_data: dict
+        :param user_data: a dict containing the values to be updated, eg. { "username" : "newUsername", "email": "new@email" }
+
         :type username: str
         :param username: Replace user name with the given string
 
         :type email: str
         :param email: Replace user email with the given string
 
         :rtype: dict
         :return: details of the updated user
         """
+        if user_data is None:
+            user_data = {}
+        user_data.update(kwargs)
         url = self._make_url(user_id) + "/information/inputs"
-        return self._put(url=url, payload=kwargs, id=user_id)
+        return self._put(url=url, payload=user_data, id=user_id)
```

### Comparing `bioblend-1.1.1/bioblend/galaxy/visual/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/visual/__init__.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/galaxy/workflows/__init__.py` & `bioblend-1.2.0/bioblend/galaxy/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/galaxyclient.py` & `bioblend-1.2.0/bioblend/galaxyclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import contextlib
 import json
 import logging
 from typing import (
     Any,
     Optional,
 )
-from urllib.parse import urljoin
 
 import requests
 import tusclient.client
 import tusclient.exceptions
 import tusclient.storage.filestorage
 import tusclient.uploader
 from requests_toolbelt import MultipartEncoder
@@ -62,17 +61,17 @@
                     )
                     r.raise_for_status()
                     found_scheme = scheme
                     break
             else:
                 raise ValueError(f"Missing scheme in url {url}")
             url = found_scheme + url
+        self.base_url = url.rstrip("/")
         # All of Galaxy's and ToolShed's API's are rooted at <url>/api so make that the url
-        self.base_url = url
-        self.url = urljoin(url, "api")
+        self.url = f"{self.base_url}/api"
         # If key has been supplied, use it; otherwise just set email and
         # password and grab user's key before first request.
         if key:
             self._key: Optional[str] = key
         else:
             self._key = None
             self.email = email
```

### Comparing `bioblend-1.1.1/bioblend/toolshed/__init__.py` & `bioblend-1.2.0/bioblend/toolshed/__init__.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/toolshed/categories/__init__.py` & `bioblend-1.2.0/bioblend/toolshed/categories/__init__.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/toolshed/repositories/__init__.py` & `bioblend-1.2.0/bioblend/toolshed/repositories/__init__.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/toolshed/tools/__init__.py` & `bioblend-1.2.0/bioblend/toolshed/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend/util/__init__.py` & `bioblend-1.2.0/bioblend/util/__init__.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/bioblend.egg-info/PKG-INFO` & `bioblend-1.2.0/bioblend.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioblend
-Version: 1.1.1
+Version: 1.2.0
 Summary: Library for interacting with the Galaxy API
 Home-page: https://bioblend.readthedocs.io/
 Author: Enis Afgan
 Author-email: afgane@gmail.com
 Maintainer: Nicola Soranzo
 Maintainer-email: nicola.soranzo@earlham.ac.uk
 License: MIT
@@ -42,14 +42,14 @@
 
 
 BioBlend is a Python library for interacting with the `Galaxy`_ API.
 
 BioBlend is supported and tested on:
 
 - Python 3.7 - 3.11
-- Galaxy release 17.09 and later.
+- Galaxy release 19.05 and later.
 
 Full docs are available at https://bioblend.readthedocs.io/ with a quick library
 overview also available in `ABOUT.rst <./ABOUT.rst>`_.
 
 .. References/hyperlinks used above
 .. _Galaxy: https://galaxyproject.org/
```

### Comparing `bioblend-1.1.1/bioblend.egg-info/SOURCES.txt` & `bioblend-1.2.0/bioblend.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 bioblend/_tests/TestGalaxyInstance.py
 bioblend/_tests/TestGalaxyInvocations.py
 bioblend/_tests/TestGalaxyJobs.py
 bioblend/_tests/TestGalaxyLibraries.py
 bioblend/_tests/TestGalaxyObjects.py
 bioblend/_tests/TestGalaxyQuotas.py
 bioblend/_tests/TestGalaxyRoles.py
+bioblend/_tests/TestGalaxyToolContainerResolution.py
 bioblend/_tests/TestGalaxyToolData.py
 bioblend/_tests/TestGalaxyToolDependencies.py
 bioblend/_tests/TestGalaxyToolInputs.py
 bioblend/_tests/TestGalaxyTools.py
 bioblend/_tests/TestGalaxyUsers.py
 bioblend/_tests/TestGalaxyWorkflows.py
 bioblend/_tests/TestToolshed.py
@@ -50,14 +51,15 @@
 bioblend/_tests/data/paste_columns_subworkflow.ga
 bioblend/_tests/data/select_first.ga
 bioblend/_tests/data/test_workflow_pause.ga
 bioblend/_tests/data/workflow_with_parameter_input.ga
 bioblend/galaxy/__init__.py
 bioblend/galaxy/client.py
 bioblend/galaxy/config/__init__.py
+bioblend/galaxy/container_resolution/__init__.py
 bioblend/galaxy/dataset_collections/__init__.py
 bioblend/galaxy/datasets/__init__.py
 bioblend/galaxy/datatypes/__init__.py
 bioblend/galaxy/folders/__init__.py
 bioblend/galaxy/forms/__init__.py
 bioblend/galaxy/ftpfiles/__init__.py
 bioblend/galaxy/genomes/__init__.py
```

### Comparing `bioblend-1.1.1/docs/Makefile` & `bioblend-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/docs/api_docs/galaxy/all.rst` & `bioblend-1.2.0/docs/api_docs/galaxy/all.rst`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/docs/api_docs/galaxy/docs.rst` & `bioblend-1.2.0/docs/api_docs/galaxy/docs.rst`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/docs/api_docs/toolshed/all.rst` & `bioblend-1.2.0/docs/api_docs/toolshed/all.rst`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/docs/conf.py` & `bioblend-1.2.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ["sphinx.ext.autodoc", "sphinx.ext.todo", "sphinx.ext.coverage", "sphinx.ext.viewcode"]
+extensions = ["sphinx.ext.autodoc", "sphinx.ext.todo", "sphinx.ext.coverage", "sphinx.ext.viewcode", "sphinx_rtd_theme"]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix of source filenames.
 source_suffix = ".rst"
 
@@ -38,15 +38,15 @@
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "BioBlend"
-copyright = "2012-2016, Enis Afgan"
+copyright = "2012-2023, Galaxy Project"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 
 # The short X.Y version.
 version = get_version()
@@ -98,15 +98,15 @@
 # in the documentation.
 autoclass_content = "both"
 
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = "default"
+html_theme = "sphinx_rtd_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 # html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
@@ -188,15 +188,15 @@
     # Additional stuff for the LaTeX preamble.
     # 'preamble': '',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-    ("index", "BioBlend.tex", "BioBlend Documentation", "Enis Afgan", "manual"),
+    ("index", "BioBlend.tex", "BioBlend Documentation", "Galaxy Project", "manual"),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
@@ -216,15 +216,15 @@
 # latex_domain_indices = True
 
 
 # -- Options for manual page output --------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [("index", "bioblend", "BioBlend Documentation", ["Enis Afgan"], 1)]
+man_pages = [("index", "bioblend", "BioBlend Documentation", ["Galaxy Project"], 1)]
 
 # If true, show URL addresses after external links.
 # man_show_urls = False
 
 
 # -- Options for Texinfo output ------------------------------------------------
 
@@ -232,15 +232,15 @@
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (
         "index",
         "BioBlend",
         "BioBlend Documentation",
-        "Enis Afgan",
+        "Galaxy Project",
         "BioBlend",
         "One line description of project.",
         "Miscellaneous",
     ),
 ]
 
 # Documents to append as an appendix to all manuals.
```

### Comparing `bioblend-1.1.1/docs/examples/create_user_get_api_key.py` & `bioblend-1.2.0/docs/examples/create_user_get_api_key.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/docs/examples/list_data_libraries.py` & `bioblend-1.2.0/docs/examples/list_data_libraries.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/docs/examples/list_histories.py` & `bioblend-1.2.0/docs/examples/list_histories.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/docs/examples/list_workflows.py` & `bioblend-1.2.0/docs/examples/list_workflows.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/docs/examples/objects/README.txt` & `bioblend-1.2.0/docs/examples/objects/README.txt`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/docs/examples/objects/list_data_libraries.py` & `bioblend-1.2.0/docs/examples/objects/list_data_libraries.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/docs/examples/objects/list_histories.py` & `bioblend-1.2.0/docs/examples/objects/list_histories.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/docs/examples/objects/list_workflows.py` & `bioblend-1.2.0/docs/examples/objects/list_workflows.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/docs/examples/objects/small.ga` & `bioblend-1.2.0/docs/examples/objects/small.ga`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/docs/examples/objects/small.py` & `bioblend-1.2.0/docs/examples/objects/small.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/docs/examples/objects/w2_bacterial_reseq.py` & `bioblend-1.2.0/docs/examples/objects/w2_bacterial_reseq.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/docs/examples/objects/w3_bacterial_denovo.py` & `bioblend-1.2.0/docs/examples/objects/w3_bacterial_denovo.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/docs/examples/objects/w5_galaxy_api.py` & `bioblend-1.2.0/docs/examples/objects/w5_galaxy_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import json
 import os
 import sys
-from urllib.parse import urljoin
 
 # This example, provided for comparison with w5_metagenomics.py,
 # contains the code required to run the metagenomics workflow
 # *without* BioBlend.
 
-URL = os.getenv("GALAXY_URL", "https://orione.crs4.it")
-API_URL = urljoin(URL, "api")
+URL = os.getenv("GALAXY_URL", "https://orione.crs4.it").rstrip("/")
+API_URL = f"{URL}/api"
 API_KEY = os.getenv("GALAXY_API_KEY", "YOUR_API_KEY")
 if API_KEY == "YOUR_API_KEY":
     sys.exit("API_KEY not set, see the README.txt file")
 
 # Clone the galaxy git repository and replace
 # YOUR_GALAXY_PATH with the clone's local path in the following code, e.g.:
 #   cd /tmp
```

### Comparing `bioblend-1.1.1/docs/examples/objects/w5_metagenomics.py` & `bioblend-1.2.0/docs/examples/objects/w5_metagenomics.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/docs/examples/run_imported_workflow.py` & `bioblend-1.2.0/docs/examples/run_imported_workflow.py`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/docs/examples/tophat_cufflinks_pairedend_workflow.ga` & `bioblend-1.2.0/docs/examples/tophat_cufflinks_pairedend_workflow.ga`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/docs/index.rst` & `bioblend-1.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bioblend-1.1.1/setup.cfg` & `bioblend-1.2.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 strict_equality = True
 warn_redundant_casts = True
 warn_unused_ignores = True
 warn_unreachable = True
 
 [mypy-bioblend._tests.*]
 disallow_untyped_defs = False
+disable_error_code = func-returns-value
 
 [options]
 install_requires = 
 	requests>=2.20.0
 	requests-toolbelt>=0.5.1,!=0.9.0
 	tuspy
 	typing-extensions
```

### Comparing `bioblend-1.1.1/tests/test_util.py` & `bioblend-1.2.0/tests/test_util.py`

 * *Files identical despite different names*

