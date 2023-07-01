# Comparing `tmp/fluxoperator-0.0.3.tar.gz` & `tmp/fluxoperator-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluxoperator-0.0.3.tar", last modified: Sun Jun 25 05:43:07 2023, max compression
+gzip compressed data, was "fluxoperator-0.0.31.tar", last modified: Sat Jul  1 08:16:07 2023, max compression
```

## Comparing `fluxoperator-0.0.3.tar` & `fluxoperator-0.0.31.tar`

### file list

```diff
@@ -1,77 +1,79 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:43:07.069711 fluxoperator-0.0.3/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2816 2023-06-25 05:43:07.069711 fluxoperator-0.0.3/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      391 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:43:07.065711 fluxoperator-0.0.3/fluxoperator/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2173 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/fluxoperator/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:43:07.065711 fluxoperator-0.0.3/fluxoperator/api/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       87 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/api/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    27361 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/api_client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13767 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/fluxoperator/client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16066 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/configuration.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      756 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/fluxoperator/decorator.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       75 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/fluxoperator/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/exceptions.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:43:07.065711 fluxoperator-0.0.3/fluxoperator/models/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1697 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/fluxoperator/models/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4552 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/fluxoperator/models/bursted_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4674 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/fluxoperator/models/bursting.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8452 2023-06-25 05:13:07.000000 fluxoperator-0.0.3/fluxoperator/models/commands.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4338 2023-06-25 05:13:07.000000 fluxoperator-0.0.3/fluxoperator/models/container_resources.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4322 2023-06-25 05:13:07.000000 fluxoperator-0.0.3/fluxoperator/models/container_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6193 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/fluxoperator/models/flux_broker.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6774 2023-06-25 05:13:07.000000 fluxoperator-0.0.3/fluxoperator/models/flux_restful.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13103 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/fluxoperator/models/flux_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4119 2023-06-25 05:13:07.000000 fluxoperator-0.0.3/fluxoperator/models/flux_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4402 2023-06-25 05:13:07.000000 fluxoperator-0.0.3/fluxoperator/models/life_cycle.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6622 2023-06-25 05:13:07.000000 fluxoperator-0.0.3/fluxoperator/models/logging_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7375 2023-06-25 05:13:07.000000 fluxoperator-0.0.3/fluxoperator/models/mini_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3612 2023-06-25 05:13:07.000000 fluxoperator-0.0.3/fluxoperator/models/mini_cluster_archive.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    23480 2023-06-25 05:13:07.000000 fluxoperator-0.0.3/fluxoperator/models/mini_cluster_container.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8150 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/models/mini_cluster_existing_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6969 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/models/mini_cluster_list.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16961 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/models/mini_cluster_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8718 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/models/mini_cluster_status.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4434 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/models/mini_cluster_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13029 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/models/mini_cluster_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3714 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/models/network.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7124 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/models/pod_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3683 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/models/security_context.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:43:07.069711 fluxoperator-0.0.3/fluxoperator/resource/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/fluxoperator/resource/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1910 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/fluxoperator/resource/network.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6890 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/fluxoperator/resource/pods.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12590 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/rest.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:43:07.065711 fluxoperator-0.0.3/fluxoperator.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2816 2023-06-25 05:43:06.000000 fluxoperator-0.0.3/fluxoperator.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2157 2023-06-25 05:43:07.000000 fluxoperator-0.0.3/fluxoperator.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 05:43:06.000000 fluxoperator-0.0.3/fluxoperator.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-02-25 05:06:19.000000 fluxoperator-0.0.3/fluxoperator.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       20 2023-06-25 05:43:06.000000 fluxoperator-0.0.3/fluxoperator.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       18 2023-06-25 05:43:06.000000 fluxoperator-0.0.3/fluxoperator.egg-info/top_level.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       69 2023-06-25 05:43:07.069711 fluxoperator-0.0.3/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2152 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/setup.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:43:07.069711 fluxoperator-0.0.3/test/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/test/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1352 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_bursted_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1831 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_bursting.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1224 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/test/test_commands.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1351 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/test/test_container_resources.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1335 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/test/test_container_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1341 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_flux_broker.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1271 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/test/test_flux_restful.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1234 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_flux_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/test/test_flux_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1226 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/test/test_life_cycle.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1277 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/test/test_logging_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7553 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_mini_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1316 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_mini_cluster_archive.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3352 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_mini_cluster_container.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1504 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_mini_cluster_existing_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16512 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_mini_cluster_list.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    11270 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_mini_cluster_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1414 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_mini_cluster_status.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1334 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_mini_cluster_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1773 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_mini_cluster_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_network.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1284 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/test/test_pod_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1289 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/test/test_security_context.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 08:16:07.120089 fluxoperator-0.0.31/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2840 2023-07-01 08:16:07.120089 fluxoperator-0.0.31/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      391 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 08:16:07.116089 fluxoperator-0.0.31/fluxoperator/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2219 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/__init__.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 08:16:07.116089 fluxoperator-0.0.31/fluxoperator/api/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       87 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/api/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    27361 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/api_client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13767 2023-06-28 02:00:02.000000 fluxoperator-0.0.31/fluxoperator/client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16066 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/configuration.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      756 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/fluxoperator/decorator.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       75 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/fluxoperator/defaults.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/exceptions.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 08:16:07.120089 fluxoperator-0.0.31/fluxoperator/models/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1743 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4552 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/bursted_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4674 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/bursting.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8452 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/commands.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4338 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/container_resources.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4322 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/container_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6193 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/flux_broker.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6774 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/flux_restful.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13103 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/flux_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4119 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/flux_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4402 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/life_cycle.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6622 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/logging_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7375 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/mini_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3612 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/mini_cluster_archive.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    24483 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/mini_cluster_container.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8150 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/mini_cluster_existing_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6969 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/mini_cluster_list.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16961 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/mini_cluster_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7727 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/mini_cluster_status.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4434 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/mini_cluster_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13029 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/mini_cluster_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3714 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/network.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7124 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/pod_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4440 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/secret.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3683 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/security_context.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 08:16:07.120089 fluxoperator-0.0.31/fluxoperator/resource/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/fluxoperator/resource/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1910 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/fluxoperator/resource/network.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6890 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/fluxoperator/resource/pods.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12590 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/rest.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 08:16:07.116089 fluxoperator-0.0.31/fluxoperator.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2840 2023-07-01 08:16:07.000000 fluxoperator-0.0.31/fluxoperator.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2207 2023-07-01 08:16:07.000000 fluxoperator-0.0.31/fluxoperator.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-01 08:16:07.000000 fluxoperator-0.0.31/fluxoperator.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-02-25 05:06:19.000000 fluxoperator-0.0.31/fluxoperator.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       20 2023-07-01 08:16:07.000000 fluxoperator-0.0.31/fluxoperator.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       18 2023-07-01 08:16:07.000000 fluxoperator-0.0.31/fluxoperator.egg-info/top_level.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       69 2023-07-01 08:16:07.120089 fluxoperator-0.0.31/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2153 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 08:16:07.120089 fluxoperator-0.0.31/test/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/test/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1352 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_bursted_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1831 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_bursting.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1224 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/test/test_commands.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1351 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/test/test_container_resources.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1335 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/test/test_container_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1341 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_flux_broker.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1271 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/test/test_flux_restful.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1234 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_flux_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/test/test_flux_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1226 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/test/test_life_cycle.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1277 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/test/test_logging_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7553 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_mini_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1316 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_mini_cluster_archive.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3352 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_mini_cluster_container.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1504 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_mini_cluster_existing_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16512 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_mini_cluster_list.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    11270 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_mini_cluster_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1414 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_mini_cluster_status.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1334 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_mini_cluster_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1773 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_mini_cluster_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_network.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1284 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/test/test_pod_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1314 2023-07-01 07:43:43.000000 fluxoperator-0.0.31/test/test_secret.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1289 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/test/test_security_context.py
```

### Comparing `fluxoperator-0.0.3/PKG-INFO` & `fluxoperator-0.0.31/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxoperator
-Version: 0.0.3
+Version: 0.0.31
 Summary: Python SDK for the Flux Operator
 Home-page: https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: Apache 2.0
 Keywords: flux-operator,flux-framework,kubernetes,workflows,jobs-api
@@ -96,14 +96,15 @@
  - [MiniClusterSpec](MiniClusterSpec.md)
  - [MiniClusterStatus](MiniClusterStatus.md)
  - [MiniClusterUser](MiniClusterUser.md)
  - [MiniClusterExistingVolume](MiniClusterExistingVolume.md)
  - [MiniClusterVolume](MiniClusterVolume.md)
  - [Network](Network.md)
  - [PodSpec](PodSpec.md)
+ - [Secret](Secret.md)
  - [SecurityContext](SecurityContext.md)
 
 ## Documentation For Authorization
 
  All endpoints do not require authorization (but they do require you have permission via your kubernetes config)
 
 ## Author
```

### Comparing `fluxoperator-0.0.3/fluxoperator/__init__.py` & `fluxoperator-0.0.31/fluxoperator/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,9 +46,10 @@
 from fluxoperator.models.mini_cluster_list import MiniClusterList
 from fluxoperator.models.mini_cluster_spec import MiniClusterSpec
 from fluxoperator.models.mini_cluster_status import MiniClusterStatus
 from fluxoperator.models.mini_cluster_user import MiniClusterUser
 from fluxoperator.models.mini_cluster_volume import MiniClusterVolume
 from fluxoperator.models.network import Network
 from fluxoperator.models.pod_spec import PodSpec
+from fluxoperator.models.secret import Secret
 from fluxoperator.models.security_context import SecurityContext
```

### Comparing `fluxoperator-0.0.3/fluxoperator/api_client.py` & `fluxoperator-0.0.31/fluxoperator/api_client.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/client.py` & `fluxoperator-0.0.31/fluxoperator/client.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/configuration.py` & `fluxoperator-0.0.31/fluxoperator/configuration.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/decorator.py` & `fluxoperator-0.0.31/fluxoperator/decorator.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/exceptions.py` & `fluxoperator-0.0.31/fluxoperator/exceptions.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/models/__init__.py` & `fluxoperator-0.0.31/fluxoperator/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,8 +32,9 @@
 from fluxoperator.models.mini_cluster_list import MiniClusterList
 from fluxoperator.models.mini_cluster_spec import MiniClusterSpec
 from fluxoperator.models.mini_cluster_status import MiniClusterStatus
 from fluxoperator.models.mini_cluster_user import MiniClusterUser
 from fluxoperator.models.mini_cluster_volume import MiniClusterVolume
 from fluxoperator.models.network import Network
 from fluxoperator.models.pod_spec import PodSpec
+from fluxoperator.models.secret import Secret
 from fluxoperator.models.security_context import SecurityContext
```

### Comparing `fluxoperator-0.0.3/fluxoperator/models/bursted_cluster.py` & `fluxoperator-0.0.31/fluxoperator/models/bursted_cluster.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/models/bursting.py` & `fluxoperator-0.0.31/fluxoperator/models/bursting.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/models/commands.py` & `fluxoperator-0.0.31/fluxoperator/models/commands.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/models/container_resources.py` & `fluxoperator-0.0.31/fluxoperator/models/container_resources.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/models/container_volume.py` & `fluxoperator-0.0.31/fluxoperator/models/container_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/models/flux_broker.py` & `fluxoperator-0.0.31/fluxoperator/models/flux_broker.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/models/flux_restful.py` & `fluxoperator-0.0.31/fluxoperator/models/flux_restful.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/models/flux_spec.py` & `fluxoperator-0.0.31/fluxoperator/models/flux_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/models/flux_user.py` & `fluxoperator-0.0.31/fluxoperator/models/flux_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/models/life_cycle.py` & `fluxoperator-0.0.31/fluxoperator/models/life_cycle.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/models/logging_spec.py` & `fluxoperator-0.0.31/fluxoperator/models/logging_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/models/mini_cluster.py` & `fluxoperator-0.0.31/fluxoperator/models/mini_cluster.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/models/mini_cluster_archive.py` & `fluxoperator-0.0.31/fluxoperator/models/mini_cluster_archive.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/models/mini_cluster_container.py` & `fluxoperator-0.0.31/fluxoperator/models/mini_cluster_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         'logs': 'str',
         'name': 'str',
         'ports': 'list[int]',
         'pre_command': 'str',
         'pull_always': 'bool',
         'resources': 'ContainerResources',
         'run_flux': 'bool',
+        'secrets': 'dict(str, Secret)',
         'security_context': 'SecurityContext',
         'volumes': 'dict(str, ContainerVolume)',
         'working_dir': 'str'
     }
 
     attribute_map = {
         'batch': 'batch',
@@ -75,20 +76,21 @@
         'logs': 'logs',
         'name': 'name',
         'ports': 'ports',
         'pre_command': 'preCommand',
         'pull_always': 'pullAlways',
         'resources': 'resources',
         'run_flux': 'runFlux',
+        'secrets': 'secrets',
         'security_context': 'securityContext',
         'volumes': 'volumes',
         'working_dir': 'workingDir'
     }
 
-    def __init__(self, batch=False, batch_raw=False, command='', commands=None, cores=0, diagnostics=False, environment=None, existing_volumes=None, flux_user=None, image='ghcr.io/rse-ops/accounting:app-latest', image_pull_secret='', launcher=False, life_cycle=None, logs='', name='', ports=None, pre_command='', pull_always=False, resources=None, run_flux=False, security_context=None, volumes=None, working_dir='', local_vars_configuration=None):  # noqa: E501
+    def __init__(self, batch=False, batch_raw=False, command='', commands=None, cores=0, diagnostics=False, environment=None, existing_volumes=None, flux_user=None, image='ghcr.io/rse-ops/accounting:app-latest', image_pull_secret='', launcher=False, life_cycle=None, logs='', name='', ports=None, pre_command='', pull_always=False, resources=None, run_flux=False, secrets=None, security_context=None, volumes=None, working_dir='', local_vars_configuration=None):  # noqa: E501
         """MiniClusterContainer - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._batch = None
         self._batch_raw = None
@@ -106,14 +108,15 @@
         self._logs = None
         self._name = None
         self._ports = None
         self._pre_command = None
         self._pull_always = None
         self._resources = None
         self._run_flux = None
+        self._secrets = None
         self._security_context = None
         self._volumes = None
         self._working_dir = None
         self.discriminator = None
 
         if batch is not None:
             self.batch = batch
@@ -151,14 +154,16 @@
             self.pre_command = pre_command
         if pull_always is not None:
             self.pull_always = pull_always
         if resources is not None:
             self.resources = resources
         if run_flux is not None:
             self.run_flux = run_flux
+        if secrets is not None:
+            self.secrets = secrets
         if security_context is not None:
             self.security_context = security_context
         if volumes is not None:
             self.volumes = volumes
         if working_dir is not None:
             self.working_dir = working_dir
 
@@ -611,14 +616,37 @@
         :param run_flux: The run_flux of this MiniClusterContainer.  # noqa: E501
         :type run_flux: bool
         """
 
         self._run_flux = run_flux
 
     @property
+    def secrets(self):
+        """Gets the secrets of this MiniClusterContainer.  # noqa: E501
+
+        Secrets that will be added to the environment The user is expected to create their own secrets for the operator to find  # noqa: E501
+
+        :return: The secrets of this MiniClusterContainer.  # noqa: E501
+        :rtype: dict(str, Secret)
+        """
+        return self._secrets
+
+    @secrets.setter
+    def secrets(self, secrets):
+        """Sets the secrets of this MiniClusterContainer.
+
+        Secrets that will be added to the environment The user is expected to create their own secrets for the operator to find  # noqa: E501
+
+        :param secrets: The secrets of this MiniClusterContainer.  # noqa: E501
+        :type secrets: dict(str, Secret)
+        """
+
+        self._secrets = secrets
+
+    @property
     def security_context(self):
         """Gets the security_context of this MiniClusterContainer.  # noqa: E501
 
 
         :return: The security_context of this MiniClusterContainer.  # noqa: E501
         :rtype: SecurityContext
         """
```

### Comparing `fluxoperator-0.0.3/fluxoperator/models/mini_cluster_existing_volume.py` & `fluxoperator-0.0.31/fluxoperator/models/mini_cluster_existing_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/models/mini_cluster_list.py` & `fluxoperator-0.0.31/fluxoperator/models/mini_cluster_list.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/models/mini_cluster_spec.py` & `fluxoperator-0.0.31/fluxoperator/models/mini_cluster_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/models/mini_cluster_status.py` & `fluxoperator-0.0.31/fluxoperator/models/mini_cluster_status.py`

 * *Files 19% similar despite different names*

```diff
@@ -29,78 +29,50 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'completed': 'bool',
         'conditions': 'list[V1Condition]',
         'jobid': 'str',
         'maximum_size': 'int',
         'selector': 'str',
         'size': 'int'
     }
 
     attribute_map = {
-        'completed': 'completed',
         'conditions': 'conditions',
         'jobid': 'jobid',
         'maximum_size': 'maximumSize',
         'selector': 'selector',
         'size': 'size'
     }
 
-    def __init__(self, completed=False, conditions=None, jobid='', maximum_size=0, selector='', size=0, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, conditions=None, jobid='', maximum_size=0, selector='', size=0, local_vars_configuration=None):  # noqa: E501
         """MiniClusterStatus - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._completed = None
         self._conditions = None
         self._jobid = None
         self._maximum_size = None
         self._selector = None
         self._size = None
         self.discriminator = None
 
-        if completed is not None:
-            self.completed = completed
         if conditions is not None:
             self.conditions = conditions
         self.jobid = jobid
         self.maximum_size = maximum_size
         self.selector = selector
         self.size = size
 
     @property
-    def completed(self):
-        """Gets the completed of this MiniClusterStatus.  # noqa: E501
-
-        Label to indicate that job is completed, comes from Job.Completed The user can also look at conditions -> JobFinished  # noqa: E501
-
-        :return: The completed of this MiniClusterStatus.  # noqa: E501
-        :rtype: bool
-        """
-        return self._completed
-
-    @completed.setter
-    def completed(self, completed):
-        """Sets the completed of this MiniClusterStatus.
-
-        Label to indicate that job is completed, comes from Job.Completed The user can also look at conditions -> JobFinished  # noqa: E501
-
-        :param completed: The completed of this MiniClusterStatus.  # noqa: E501
-        :type completed: bool
-        """
-
-        self._completed = completed
-
-    @property
     def conditions(self):
         """Gets the conditions of this MiniClusterStatus.  # noqa: E501
 
         conditions hold the latest Flux Job and MiniCluster states  # noqa: E501
 
         :return: The conditions of this MiniClusterStatus.  # noqa: E501
         :rtype: list[V1Condition]
```

### Comparing `fluxoperator-0.0.3/fluxoperator/models/mini_cluster_user.py` & `fluxoperator-0.0.31/fluxoperator/models/mini_cluster_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/models/mini_cluster_volume.py` & `fluxoperator-0.0.31/fluxoperator/models/mini_cluster_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/models/network.py` & `fluxoperator-0.0.31/fluxoperator/models/network.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/models/pod_spec.py` & `fluxoperator-0.0.31/fluxoperator/models/pod_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/models/security_context.py` & `fluxoperator-0.0.31/fluxoperator/models/security_context.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/resource/network.py` & `fluxoperator-0.0.31/fluxoperator/resource/network.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/resource/pods.py` & `fluxoperator-0.0.31/fluxoperator/resource/pods.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator/rest.py` & `fluxoperator-0.0.31/fluxoperator/rest.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/fluxoperator.egg-info/PKG-INFO` & `fluxoperator-0.0.31/fluxoperator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxoperator
-Version: 0.0.3
+Version: 0.0.31
 Summary: Python SDK for the Flux Operator
 Home-page: https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: Apache 2.0
 Keywords: flux-operator,flux-framework,kubernetes,workflows,jobs-api
@@ -96,14 +96,15 @@
  - [MiniClusterSpec](MiniClusterSpec.md)
  - [MiniClusterStatus](MiniClusterStatus.md)
  - [MiniClusterUser](MiniClusterUser.md)
  - [MiniClusterExistingVolume](MiniClusterExistingVolume.md)
  - [MiniClusterVolume](MiniClusterVolume.md)
  - [Network](Network.md)
  - [PodSpec](PodSpec.md)
+ - [Secret](Secret.md)
  - [SecurityContext](SecurityContext.md)
 
 ## Documentation For Authorization
 
  All endpoints do not require authorization (but they do require you have permission via your kubernetes config)
 
 ## Author
```

### Comparing `fluxoperator-0.0.3/fluxoperator.egg-info/SOURCES.txt` & `fluxoperator-0.0.31/fluxoperator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 fluxoperator/models/mini_cluster_list.py
 fluxoperator/models/mini_cluster_spec.py
 fluxoperator/models/mini_cluster_status.py
 fluxoperator/models/mini_cluster_user.py
 fluxoperator/models/mini_cluster_volume.py
 fluxoperator/models/network.py
 fluxoperator/models/pod_spec.py
+fluxoperator/models/secret.py
 fluxoperator/models/security_context.py
 fluxoperator/resource/__init__.py
 fluxoperator/resource/network.py
 fluxoperator/resource/pods.py
 test/__init__.py
 test/test_bursted_cluster.py
 test/test_bursting.py
@@ -62,8 +63,9 @@
 test/test_mini_cluster_list.py
 test/test_mini_cluster_spec.py
 test/test_mini_cluster_status.py
 test/test_mini_cluster_user.py
 test/test_mini_cluster_volume.py
 test/test_network.py
 test/test_pod_spec.py
+test/test_secret.py
 test/test_security_context.py
```

### Comparing `fluxoperator-0.0.3/setup.py` & `fluxoperator-0.0.31/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ################################################################################
 # MAIN #########################################################################
 ################################################################################
 
 if __name__ == "__main__":
     setup(
         name="fluxoperator",
-        version="0.0.3",
+        version="0.0.31",
         author="Vanessasaurus",
         author_email="vsoch@users.noreply.github.com",
         maintainer="Vanessasaurus",
         packages=find_packages(),
         include_package_data=True,
         zip_safe=False,
         url="https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1",
```

### Comparing `fluxoperator-0.0.3/test/test_bursted_cluster.py` & `fluxoperator-0.0.31/test/test_bursted_cluster.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_bursting.py` & `fluxoperator-0.0.31/test/test_bursting.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_commands.py` & `fluxoperator-0.0.31/test/test_commands.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_container_resources.py` & `fluxoperator-0.0.31/test/test_container_resources.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_container_volume.py` & `fluxoperator-0.0.31/test/test_container_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_flux_broker.py` & `fluxoperator-0.0.31/test/test_flux_broker.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_flux_restful.py` & `fluxoperator-0.0.31/test/test_flux_restful.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_flux_spec.py` & `fluxoperator-0.0.31/test/test_flux_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_flux_user.py` & `fluxoperator-0.0.31/test/test_flux_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_life_cycle.py` & `fluxoperator-0.0.31/test/test_life_cycle.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_logging_spec.py` & `fluxoperator-0.0.31/test/test_logging_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_mini_cluster.py` & `fluxoperator-0.0.31/test/test_mini_cluster.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_mini_cluster_archive.py` & `fluxoperator-0.0.31/test/test_mini_cluster_archive.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_mini_cluster_container.py` & `fluxoperator-0.0.31/test/test_mini_cluster_container.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_mini_cluster_existing_volume.py` & `fluxoperator-0.0.31/test/test_mini_cluster_existing_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_mini_cluster_list.py` & `fluxoperator-0.0.31/test/test_mini_cluster_list.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_mini_cluster_spec.py` & `fluxoperator-0.0.31/test/test_mini_cluster_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_mini_cluster_status.py` & `fluxoperator-0.0.31/test/test_mini_cluster_status.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_mini_cluster_user.py` & `fluxoperator-0.0.31/test/test_mini_cluster_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_mini_cluster_volume.py` & `fluxoperator-0.0.31/test/test_mini_cluster_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_network.py` & `fluxoperator-0.0.31/test/test_network.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_pod_spec.py` & `fluxoperator-0.0.31/test/test_pod_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.3/test/test_security_context.py` & `fluxoperator-0.0.31/test/test_security_context.py`

 * *Files identical despite different names*

