# Comparing `tmp/pulumiverse_exoscale-0.49.0.tar.gz` & `tmp/pulumiverse_exoscale-0.50.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_exoscale-0.49.0.tar", last modified: Mon Jun 12 08:57:37 2023, max compression
+gzip compressed data, was "pulumiverse_exoscale-0.50.0.tar", last modified: Sat Jul  1 20:47:39 2023, max compression
```

## Comparing `pulumiverse_exoscale-0.49.0.tar` & `pulumiverse_exoscale-0.50.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:57:37.173968 pulumiverse_exoscale-0.49.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-12 08:57:37.173968 pulumiverse_exoscale-0.49.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:57:37.169968 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51270 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/anti_affinity_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    59349 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    50320 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/compute_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:57:37.173968 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    39665 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    17348 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    18856 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/elastic_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_anti_affinity_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_compute_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    20159 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_compute_instance_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_compute_ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_compute_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_database_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_elastic_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_instance_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_instance_pool_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_nlb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_private_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_security_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    19402 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_sks_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    18631 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_sks_cluster_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    18303 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_sks_nodepool.py
--rw-r--r--   0 runner    (1001) docker     (123)    19063 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_sks_nodepool_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/iam_access_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    53079 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/instance_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    37973 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    20752 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    12155 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/nic.py
--rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/nlb.py
--rw-r--r--   0 runner    (1001) docker     (123)    25072 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/nlb_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    90177 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/private_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    16360 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/secondary_ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/security_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    39602 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/security_group_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/security_group_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    40583 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/sks_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/sks_kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    41557 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/sks_nodepool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/ssh_keypair.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:57:37.173968 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-12 08:57:37.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-12 08:57:37.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 08:57:37.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 08:57:37.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-12 08:57:37.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-12 08:57:37.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 08:57:37.173968 pulumiverse_exoscale-0.49.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:47:39.309935 pulumiverse_exoscale-0.50.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-01 20:47:39.309935 pulumiverse_exoscale-0.50.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:47:39.309935 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/
+-rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69999 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/anti_affinity_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59628 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49571 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/compute_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:47:39.309935 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39581 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17152 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18912 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/elastic_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_anti_affinity_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14679 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_compute_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20444 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_compute_instance_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_compute_ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_compute_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_database_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_elastic_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_instance_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_instance_pool_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_nlb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_private_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19663 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_sks_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18901 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_sks_cluster_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18603 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_sks_nodepool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19333 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_sks_nodepool_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15680 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/iam_access_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53173 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/instance_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37861 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21404 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/nic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15474 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/nlb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24827 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/nlb_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107961 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16160 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/private_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/secondary_ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39926 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/security_group_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/security_group_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41174 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/sks_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23739 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/sks_kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40692 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/sks_nodepool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10691 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/ssh_keypair.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:47:39.309935 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-01 20:47:39.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-01 20:47:39.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:47:39.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:47:39.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-01 20:47:39.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-01 20:47:39.000000 pulumiverse_exoscale-0.50.0/pulumiverse_exoscale.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 20:47:39.309935 pulumiverse_exoscale-0.50.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-01 20:47:38.000000 pulumiverse_exoscale-0.50.0/setup.py
```

### Comparing `pulumiverse_exoscale-0.49.0/PKG-INFO` & `pulumiverse_exoscale-0.50.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_exoscale
-Version: 0.49.0
+Version: 0.50.0
 Summary: A Pulumi package for creating and managing exoscale cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-exoscale
 Keywords: pulumi exoscale category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_exoscale-0.49.0/README.md` & `pulumiverse_exoscale-0.50.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/__init__.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/_utilities.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/affinity.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/affinity.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,54 +15,54 @@
 class AffinityArgs:
     def __init__(__self__, *,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Affinity resource.
-        :param pulumi.Input[str] description: A free-form text describing the group.
-        :param pulumi.Input[str] name: The anti-affinity group name.
-        :param pulumi.Input[str] type: The type of the group (`host anti-affinity` is the only supported value).
+        :param pulumi.Input[str] description: ❗ A free-form text describing the group.
+        :param pulumi.Input[str] name: ❗ The anti-affinity group name.
+        :param pulumi.Input[str] type: ❗ The type of the group (`host anti-affinity` is the only supported value).
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        A free-form text describing the group.
+        ❗ A free-form text describing the group.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The anti-affinity group name.
+        ❗ The anti-affinity group name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        The type of the group (`host anti-affinity` is the only supported value).
+        ❗ The type of the group (`host anti-affinity` is the only supported value).
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -72,17 +72,17 @@
     def __init__(__self__, *,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  virtual_machine_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering Affinity resources.
-        :param pulumi.Input[str] description: A free-form text describing the group.
-        :param pulumi.Input[str] name: The anti-affinity group name.
-        :param pulumi.Input[str] type: The type of the group (`host anti-affinity` is the only supported value).
+        :param pulumi.Input[str] description: ❗ A free-form text describing the group.
+        :param pulumi.Input[str] name: ❗ The anti-affinity group name.
+        :param pulumi.Input[str] type: ❗ The type of the group (`host anti-affinity` is the only supported value).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machine_ids: The compute instances (IDs) members of the group.
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if type is not None:
@@ -90,39 +90,39 @@
         if virtual_machine_ids is not None:
             pulumi.set(__self__, "virtual_machine_ids", virtual_machine_ids)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        A free-form text describing the group.
+        ❗ A free-form text describing the group.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The anti-affinity group name.
+        ❗ The anti-affinity group name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        The type of the group (`host anti-affinity` is the only supported value).
+        ❗ The type of the group (`host anti-affinity` is the only supported value).
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -149,17 +149,17 @@
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use AntiAffinityGroup instead.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] description: A free-form text describing the group.
-        :param pulumi.Input[str] name: The anti-affinity group name.
-        :param pulumi.Input[str] type: The type of the group (`host anti-affinity` is the only supported value).
+        :param pulumi.Input[str] description: ❗ A free-form text describing the group.
+        :param pulumi.Input[str] name: ❗ The anti-affinity group name.
+        :param pulumi.Input[str] type: ❗ The type of the group (`host anti-affinity` is the only supported value).
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[AffinityArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -214,17 +214,17 @@
         """
         Get an existing Affinity resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] description: A free-form text describing the group.
-        :param pulumi.Input[str] name: The anti-affinity group name.
-        :param pulumi.Input[str] type: The type of the group (`host anti-affinity` is the only supported value).
+        :param pulumi.Input[str] description: ❗ A free-form text describing the group.
+        :param pulumi.Input[str] name: ❗ The anti-affinity group name.
+        :param pulumi.Input[str] type: ❗ The type of the group (`host anti-affinity` is the only supported value).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machine_ids: The compute instances (IDs) members of the group.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _AffinityState.__new__(_AffinityState)
 
         __props__.__dict__["description"] = description
@@ -233,31 +233,31 @@
         __props__.__dict__["virtual_machine_ids"] = virtual_machine_ids
         return Affinity(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
-        A free-form text describing the group.
+        ❗ A free-form text describing the group.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The anti-affinity group name.
+        ❗ The anti-affinity group name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[Optional[str]]:
         """
-        The type of the group (`host anti-affinity` is the only supported value).
+        ❗ The type of the group (`host anti-affinity` is the only supported value).
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="virtualMachineIds")
     def virtual_machine_ids(self) -> pulumi.Output[Sequence[str]]:
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/anti_affinity_group.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/anti_affinity_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,39 +14,39 @@
 @pulumi.input_type
 class AntiAffinityGroupArgs:
     def __init__(__self__, *,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a AntiAffinityGroup resource.
-        :param pulumi.Input[str] description: A free-form text describing the group.
-        :param pulumi.Input[str] name: The anti-affinity group name.
+        :param pulumi.Input[str] description: ❗ A free-form text describing the group.
+        :param pulumi.Input[str] name: ❗ The anti-affinity group name.
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        A free-form text describing the group.
+        ❗ A free-form text describing the group.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The anti-affinity group name.
+        ❗ The anti-affinity group name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -54,39 +54,39 @@
 @pulumi.input_type
 class _AntiAffinityGroupState:
     def __init__(__self__, *,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering AntiAffinityGroup resources.
-        :param pulumi.Input[str] description: A free-form text describing the group.
-        :param pulumi.Input[str] name: The anti-affinity group name.
+        :param pulumi.Input[str] description: ❗ A free-form text describing the group.
+        :param pulumi.Input[str] name: ❗ The anti-affinity group name.
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        A free-form text describing the group.
+        ❗ A free-form text describing the group.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The anti-affinity group name.
+        ❗ The anti-affinity group name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -110,16 +110,16 @@
 
          exoscale_anti_affinity_group.my_anti_affinity_group \\
 
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] description: A free-form text describing the group.
-        :param pulumi.Input[str] name: The anti-affinity group name.
+        :param pulumi.Input[str] description: ❗ A free-form text describing the group.
+        :param pulumi.Input[str] name: ❗ The anti-affinity group name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[AntiAffinityGroupArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -179,34 +179,34 @@
         """
         Get an existing AntiAffinityGroup resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] description: A free-form text describing the group.
-        :param pulumi.Input[str] name: The anti-affinity group name.
+        :param pulumi.Input[str] description: ❗ A free-form text describing the group.
+        :param pulumi.Input[str] name: ❗ The anti-affinity group name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _AntiAffinityGroupState.__new__(_AntiAffinityGroupState)
 
         __props__.__dict__["description"] = description
         __props__.__dict__["name"] = name
         return AntiAffinityGroup(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
-        A free-form text describing the group.
+        ❗ A free-form text describing the group.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The anti-affinity group name.
+        ❗ The anti-affinity group name.
         """
         return pulumi.get(self, "name")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/compute.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/compute.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,38 +32,31 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  template: Optional[pulumi.Input[str]] = None,
                  template_id: Optional[pulumi.Input[str]] = None,
                  user_data: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Compute resource.
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`).
-        :param pulumi.Input[str] zone: The Exoscale Zone name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of anti-affinity groups (IDs; at creation time only; conflicts with `affinity_groups`).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_groups: A list of anti-affinity groups (names; at creation time only; conflicts with `affinity_group_ids`).
-        :param pulumi.Input[str] display_name: The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS'
-               *hostname* during creation, so the value must contain only alphanumeric and hyphen (" - ") characters; it can be changed
-               to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will
-               be generated automatically.
-        :param pulumi.Input[str] hostname: The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or
-               `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value
-               requires to reboot the instance.
+        :param pulumi.Input[str] zone: ❗ The Exoscale Zone name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: ❗ A list of anti-affinity groups (IDs; at creation time only; conflicts with `affinity_groups`).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_groups: ❗ A list of anti-affinity groups (names; at creation time only; conflicts with `affinity_group_ids`).
+        :param pulumi.Input[str] display_name: The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS' *hostname* during creation, so the value must contain only alphanumeric and hyphen (" - ") characters; it can be changed to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically.
+        :param pulumi.Input[str] hostname: The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value requires to reboot the instance.
         :param pulumi.Input[bool] ip4: Request an IPv4 address on the default NIC
         :param pulumi.Input[bool] ip6: Request an IPv6 address on the default NIC
-        :param pulumi.Input[str] key_pair: The SSH keypair (name) to authorize in the instance.
-        :param pulumi.Input[str] keyboard: The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`,
-               `pt`, `uk`, `us`; at creation time only).
+        :param pulumi.Input[str] key_pair: ❗ The SSH keypair (name) to authorize in the instance.
+        :param pulumi.Input[str] keyboard: The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`, `pt`, `uk`, `us`; at creation time only).
         :param pulumi.Input[str] reverse_dns: The instance reverse DNS record (must end with a `.`; e.g: `my-instance.example.net.`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of security groups (IDs; conflicts with `security_groups`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_groups: A list of security groups (names; conflicts with `security_group_ids`).
         :param pulumi.Input[str] size: The instance size (`Tiny`, `Small`, `Medium`, `Large`, etc.)
         :param pulumi.Input[str] state: The instance state (`Running` or `Stopped`; default: `Running`)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
-        :param pulumi.Input[str] template: The compute instance template (name). Only *featured* templates are available, if you want to reference *custom
-               templates* use the `template_id` attribute instead.
-        :param pulumi.Input[str] template_id: The compute instance template (ID). Usage of the `exoscale_compute_template` data source is recommended.
+        :param pulumi.Input[str] template: ❗ The compute instance template (name). Only *featured* templates are available, if you want to reference *custom templates* use the `template_id` attribute instead.
+        :param pulumi.Input[str] template_id: ❗ The compute instance template (ID). Usage of the `get_compute_template` data source is recommended.
         :param pulumi.Input[str] user_data: cloud-init configuration (no need to base64-encode or gzip it as the provider will take care of it).
         """
         pulumi.set(__self__, "disk_size", disk_size)
         pulumi.set(__self__, "zone", zone)
         if affinity_group_ids is not None:
             pulumi.set(__self__, "affinity_group_ids", affinity_group_ids)
         if affinity_groups is not None:
@@ -111,68 +104,63 @@
     def disk_size(self, value: pulumi.Input[int]):
         pulumi.set(self, "disk_size", value)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
-        The Exoscale Zone name.
+        ❗ The Exoscale Zone name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
     @property
     @pulumi.getter(name="affinityGroupIds")
     def affinity_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of anti-affinity groups (IDs; at creation time only; conflicts with `affinity_groups`).
+        ❗ A list of anti-affinity groups (IDs; at creation time only; conflicts with `affinity_groups`).
         """
         return pulumi.get(self, "affinity_group_ids")
 
     @affinity_group_ids.setter
     def affinity_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "affinity_group_ids", value)
 
     @property
     @pulumi.getter(name="affinityGroups")
     def affinity_groups(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of anti-affinity groups (names; at creation time only; conflicts with `affinity_group_ids`).
+        ❗ A list of anti-affinity groups (names; at creation time only; conflicts with `affinity_group_ids`).
         """
         return pulumi.get(self, "affinity_groups")
 
     @affinity_groups.setter
     def affinity_groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "affinity_groups", value)
 
     @property
     @pulumi.getter(name="displayName")
     def display_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS'
-        *hostname* during creation, so the value must contain only alphanumeric and hyphen (" - ") characters; it can be changed
-        to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will
-        be generated automatically.
+        The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS' *hostname* during creation, so the value must contain only alphanumeric and hyphen (" - ") characters; it can be changed to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically.
         """
         return pulumi.get(self, "display_name")
 
     @display_name.setter
     def display_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "display_name", value)
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[pulumi.Input[str]]:
         """
-        The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or
-        `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value
-        requires to reboot the instance.
+        The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value requires to reboot the instance.
         """
         return pulumi.get(self, "hostname")
 
     @hostname.setter
     def hostname(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "hostname", value)
 
@@ -200,28 +188,27 @@
     def ip6(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ip6", value)
 
     @property
     @pulumi.getter(name="keyPair")
     def key_pair(self) -> Optional[pulumi.Input[str]]:
         """
-        The SSH keypair (name) to authorize in the instance.
+        ❗ The SSH keypair (name) to authorize in the instance.
         """
         return pulumi.get(self, "key_pair")
 
     @key_pair.setter
     def key_pair(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key_pair", value)
 
     @property
     @pulumi.getter
     def keyboard(self) -> Optional[pulumi.Input[str]]:
         """
-        The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`,
-        `pt`, `uk`, `us`; at creation time only).
+        The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`, `pt`, `uk`, `us`; at creation time only).
         """
         return pulumi.get(self, "keyboard")
 
     @keyboard.setter
     def keyboard(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "keyboard", value)
 
@@ -297,28 +284,27 @@
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
     @pulumi.getter
     def template(self) -> Optional[pulumi.Input[str]]:
         """
-        The compute instance template (name). Only *featured* templates are available, if you want to reference *custom
-        templates* use the `template_id` attribute instead.
+        ❗ The compute instance template (name). Only *featured* templates are available, if you want to reference *custom templates* use the `template_id` attribute instead.
         """
         return pulumi.get(self, "template")
 
     @template.setter
     def template(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "template", value)
 
     @property
     @pulumi.getter(name="templateId")
     def template_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The compute instance template (ID). Usage of the `exoscale_compute_template` data source is recommended.
+        ❗ The compute instance template (ID). Usage of the `get_compute_template` data source is recommended.
         """
         return pulumi.get(self, "template_id")
 
     @template_id.setter
     def template_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "template_id", value)
 
@@ -363,47 +349,39 @@
                  template_id: Optional[pulumi.Input[str]] = None,
                  user_data: Optional[pulumi.Input[str]] = None,
                  user_data_base64: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Compute resources.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of anti-affinity groups (IDs; at creation time only; conflicts with `affinity_groups`).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_groups: A list of anti-affinity groups (names; at creation time only; conflicts with `affinity_group_ids`).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: ❗ A list of anti-affinity groups (IDs; at creation time only; conflicts with `affinity_groups`).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_groups: ❗ A list of anti-affinity groups (names; at creation time only; conflicts with `affinity_group_ids`).
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`).
-        :param pulumi.Input[str] display_name: The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS'
-               *hostname* during creation, so the value must contain only alphanumeric and hyphen (" - ") characters; it can be changed
-               to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will
-               be generated automatically.
-        :param pulumi.Input[str] hostname: The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or
-               `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value
-               requires to reboot the instance.
+        :param pulumi.Input[str] display_name: The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS' *hostname* during creation, so the value must contain only alphanumeric and hyphen (" - ") characters; it can be changed to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically.
+        :param pulumi.Input[str] hostname: The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value requires to reboot the instance.
         :param pulumi.Input[bool] ip4: Request an IPv4 address on the default NIC
         :param pulumi.Input[bool] ip6: Request an IPv6 address on the default NIC
         :param pulumi.Input[str] ip6_address: The instance (main network interface) IPv6 address (if enabled).
         :param pulumi.Input[str] ip_address: The instance (main network interface) IPv4 address.
-        :param pulumi.Input[str] key_pair: The SSH keypair (name) to authorize in the instance.
-        :param pulumi.Input[str] keyboard: The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`,
-               `pt`, `uk`, `us`; at creation time only).
+        :param pulumi.Input[str] key_pair: ❗ The SSH keypair (name) to authorize in the instance.
+        :param pulumi.Input[str] keyboard: The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`, `pt`, `uk`, `us`; at creation time only).
         :param pulumi.Input[str] name: The instance hostname. Please use the `hostname` argument instead.
         :param pulumi.Input[str] password: The instance initial password and/or encrypted password.
         :param pulumi.Input[str] reverse_dns: The instance reverse DNS record (must end with a `.`; e.g: `my-instance.example.net.`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of security groups (IDs; conflicts with `security_groups`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_groups: A list of security groups (names; conflicts with `security_group_ids`).
         :param pulumi.Input[str] size: The instance size (`Tiny`, `Small`, `Medium`, `Large`, etc.)
         :param pulumi.Input[str] state: The instance state (`Running` or `Stopped`; default: `Running`)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
-        :param pulumi.Input[str] template: The compute instance template (name). Only *featured* templates are available, if you want to reference *custom
-               templates* use the `template_id` attribute instead.
-        :param pulumi.Input[str] template_id: The compute instance template (ID). Usage of the `exoscale_compute_template` data source is recommended.
+        :param pulumi.Input[str] template: ❗ The compute instance template (name). Only *featured* templates are available, if you want to reference *custom templates* use the `template_id` attribute instead.
+        :param pulumi.Input[str] template_id: ❗ The compute instance template (ID). Usage of the `get_compute_template` data source is recommended.
         :param pulumi.Input[str] user_data: cloud-init configuration (no need to base64-encode or gzip it as the provider will take care of it).
         :param pulumi.Input[bool] user_data_base64: was the cloud-init configuration base64 encoded
-        :param pulumi.Input[str] username: The user to use to connect to the instance. If you've referenced a *custom template* in the resource, use the
-               `exoscale_compute_template` data source `username` attribute instead.
-        :param pulumi.Input[str] zone: The Exoscale Zone name.
+        :param pulumi.Input[str] username: The user to use to connect to the instance. If you've referenced a *custom template* in the resource, use the `get_compute_template` data source `username` attribute instead.
+        :param pulumi.Input[str] zone: ❗ The Exoscale Zone name.
         """
         if affinity_group_ids is not None:
             pulumi.set(__self__, "affinity_group_ids", affinity_group_ids)
         if affinity_groups is not None:
             pulumi.set(__self__, "affinity_groups", affinity_groups)
         if disk_size is not None:
             pulumi.set(__self__, "disk_size", disk_size)
@@ -462,27 +440,27 @@
         if zone is not None:
             pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter(name="affinityGroupIds")
     def affinity_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of anti-affinity groups (IDs; at creation time only; conflicts with `affinity_groups`).
+        ❗ A list of anti-affinity groups (IDs; at creation time only; conflicts with `affinity_groups`).
         """
         return pulumi.get(self, "affinity_group_ids")
 
     @affinity_group_ids.setter
     def affinity_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "affinity_group_ids", value)
 
     @property
     @pulumi.getter(name="affinityGroups")
     def affinity_groups(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of anti-affinity groups (names; at creation time only; conflicts with `affinity_group_ids`).
+        ❗ A list of anti-affinity groups (names; at creation time only; conflicts with `affinity_group_ids`).
         """
         return pulumi.get(self, "affinity_groups")
 
     @affinity_groups.setter
     def affinity_groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "affinity_groups", value)
 
@@ -498,18 +476,15 @@
     def disk_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "disk_size", value)
 
     @property
     @pulumi.getter(name="displayName")
     def display_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS'
-        *hostname* during creation, so the value must contain only alphanumeric and hyphen (" - ") characters; it can be changed
-        to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will
-        be generated automatically.
+        The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS' *hostname* during creation, so the value must contain only alphanumeric and hyphen (" - ") characters; it can be changed to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically.
         """
         return pulumi.get(self, "display_name")
 
     @display_name.setter
     def display_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "display_name", value)
 
@@ -522,17 +497,15 @@
     def gateway(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "gateway", value)
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[pulumi.Input[str]]:
         """
-        The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or
-        `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value
-        requires to reboot the instance.
+        The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value requires to reboot the instance.
         """
         return pulumi.get(self, "hostname")
 
     @hostname.setter
     def hostname(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "hostname", value)
 
@@ -593,41 +566,43 @@
     def ip_address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ip_address", value)
 
     @property
     @pulumi.getter(name="keyPair")
     def key_pair(self) -> Optional[pulumi.Input[str]]:
         """
-        The SSH keypair (name) to authorize in the instance.
+        ❗ The SSH keypair (name) to authorize in the instance.
         """
         return pulumi.get(self, "key_pair")
 
     @key_pair.setter
     def key_pair(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key_pair", value)
 
     @property
     @pulumi.getter
     def keyboard(self) -> Optional[pulumi.Input[str]]:
         """
-        The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`,
-        `pt`, `uk`, `us`; at creation time only).
+        The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`, `pt`, `uk`, `us`; at creation time only).
         """
         return pulumi.get(self, "keyboard")
 
     @keyboard.setter
     def keyboard(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "keyboard", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         The instance hostname. Please use the `hostname` argument instead.
         """
+        warnings.warn("""use `hostname` attribute instead""", DeprecationWarning)
+        pulumi.log.warn("""name is deprecated: use `hostname` attribute instead""")
+
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
@@ -714,28 +689,27 @@
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
     @pulumi.getter
     def template(self) -> Optional[pulumi.Input[str]]:
         """
-        The compute instance template (name). Only *featured* templates are available, if you want to reference *custom
-        templates* use the `template_id` attribute instead.
+        ❗ The compute instance template (name). Only *featured* templates are available, if you want to reference *custom templates* use the `template_id` attribute instead.
         """
         return pulumi.get(self, "template")
 
     @template.setter
     def template(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "template", value)
 
     @property
     @pulumi.getter(name="templateId")
     def template_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The compute instance template (ID). Usage of the `exoscale_compute_template` data source is recommended.
+        ❗ The compute instance template (ID). Usage of the `get_compute_template` data source is recommended.
         """
         return pulumi.get(self, "template_id")
 
     @template_id.setter
     def template_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "template_id", value)
 
@@ -763,28 +737,30 @@
     def user_data_base64(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "user_data_base64", value)
 
     @property
     @pulumi.getter
     def username(self) -> Optional[pulumi.Input[str]]:
         """
-        The user to use to connect to the instance. If you've referenced a *custom template* in the resource, use the
-        `exoscale_compute_template` data source `username` attribute instead.
+        The user to use to connect to the instance. If you've referenced a *custom template* in the resource, use the `get_compute_template` data source `username` attribute instead.
         """
+        warnings.warn("""broken, use `compute_template` data source `username` attribute""", DeprecationWarning)
+        pulumi.log.warn("""username is deprecated: broken, use `compute_template` data source `username` attribute""")
+
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The Exoscale Zone name.
+        ❗ The Exoscale Zone name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -817,40 +793,33 @@
         """
         !> **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use ComputeInstance instead.
 
         Manage Exoscale Compute Instances.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of anti-affinity groups (IDs; at creation time only; conflicts with `affinity_groups`).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_groups: A list of anti-affinity groups (names; at creation time only; conflicts with `affinity_group_ids`).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: ❗ A list of anti-affinity groups (IDs; at creation time only; conflicts with `affinity_groups`).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_groups: ❗ A list of anti-affinity groups (names; at creation time only; conflicts with `affinity_group_ids`).
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`).
-        :param pulumi.Input[str] display_name: The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS'
-               *hostname* during creation, so the value must contain only alphanumeric and hyphen (" - ") characters; it can be changed
-               to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will
-               be generated automatically.
-        :param pulumi.Input[str] hostname: The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or
-               `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value
-               requires to reboot the instance.
+        :param pulumi.Input[str] display_name: The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS' *hostname* during creation, so the value must contain only alphanumeric and hyphen (" - ") characters; it can be changed to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically.
+        :param pulumi.Input[str] hostname: The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value requires to reboot the instance.
         :param pulumi.Input[bool] ip4: Request an IPv4 address on the default NIC
         :param pulumi.Input[bool] ip6: Request an IPv6 address on the default NIC
-        :param pulumi.Input[str] key_pair: The SSH keypair (name) to authorize in the instance.
-        :param pulumi.Input[str] keyboard: The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`,
-               `pt`, `uk`, `us`; at creation time only).
+        :param pulumi.Input[str] key_pair: ❗ The SSH keypair (name) to authorize in the instance.
+        :param pulumi.Input[str] keyboard: The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`, `pt`, `uk`, `us`; at creation time only).
         :param pulumi.Input[str] reverse_dns: The instance reverse DNS record (must end with a `.`; e.g: `my-instance.example.net.`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of security groups (IDs; conflicts with `security_groups`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_groups: A list of security groups (names; conflicts with `security_group_ids`).
         :param pulumi.Input[str] size: The instance size (`Tiny`, `Small`, `Medium`, `Large`, etc.)
         :param pulumi.Input[str] state: The instance state (`Running` or `Stopped`; default: `Running`)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
-        :param pulumi.Input[str] template: The compute instance template (name). Only *featured* templates are available, if you want to reference *custom
-               templates* use the `template_id` attribute instead.
-        :param pulumi.Input[str] template_id: The compute instance template (ID). Usage of the `exoscale_compute_template` data source is recommended.
+        :param pulumi.Input[str] template: ❗ The compute instance template (name). Only *featured* templates are available, if you want to reference *custom templates* use the `template_id` attribute instead.
+        :param pulumi.Input[str] template_id: ❗ The compute instance template (ID). Usage of the `get_compute_template` data source is recommended.
         :param pulumi.Input[str] user_data: cloud-init configuration (no need to base64-encode or gzip it as the provider will take care of it).
-        :param pulumi.Input[str] zone: The Exoscale Zone name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale Zone name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ComputeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -975,47 +944,39 @@
         """
         Get an existing Compute resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of anti-affinity groups (IDs; at creation time only; conflicts with `affinity_groups`).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_groups: A list of anti-affinity groups (names; at creation time only; conflicts with `affinity_group_ids`).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: ❗ A list of anti-affinity groups (IDs; at creation time only; conflicts with `affinity_groups`).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_groups: ❗ A list of anti-affinity groups (names; at creation time only; conflicts with `affinity_group_ids`).
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`).
-        :param pulumi.Input[str] display_name: The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS'
-               *hostname* during creation, so the value must contain only alphanumeric and hyphen (" - ") characters; it can be changed
-               to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will
-               be generated automatically.
-        :param pulumi.Input[str] hostname: The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or
-               `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value
-               requires to reboot the instance.
+        :param pulumi.Input[str] display_name: The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS' *hostname* during creation, so the value must contain only alphanumeric and hyphen (" - ") characters; it can be changed to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically.
+        :param pulumi.Input[str] hostname: The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value requires to reboot the instance.
         :param pulumi.Input[bool] ip4: Request an IPv4 address on the default NIC
         :param pulumi.Input[bool] ip6: Request an IPv6 address on the default NIC
         :param pulumi.Input[str] ip6_address: The instance (main network interface) IPv6 address (if enabled).
         :param pulumi.Input[str] ip_address: The instance (main network interface) IPv4 address.
-        :param pulumi.Input[str] key_pair: The SSH keypair (name) to authorize in the instance.
-        :param pulumi.Input[str] keyboard: The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`,
-               `pt`, `uk`, `us`; at creation time only).
+        :param pulumi.Input[str] key_pair: ❗ The SSH keypair (name) to authorize in the instance.
+        :param pulumi.Input[str] keyboard: The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`, `pt`, `uk`, `us`; at creation time only).
         :param pulumi.Input[str] name: The instance hostname. Please use the `hostname` argument instead.
         :param pulumi.Input[str] password: The instance initial password and/or encrypted password.
         :param pulumi.Input[str] reverse_dns: The instance reverse DNS record (must end with a `.`; e.g: `my-instance.example.net.`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of security groups (IDs; conflicts with `security_groups`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_groups: A list of security groups (names; conflicts with `security_group_ids`).
         :param pulumi.Input[str] size: The instance size (`Tiny`, `Small`, `Medium`, `Large`, etc.)
         :param pulumi.Input[str] state: The instance state (`Running` or `Stopped`; default: `Running`)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
-        :param pulumi.Input[str] template: The compute instance template (name). Only *featured* templates are available, if you want to reference *custom
-               templates* use the `template_id` attribute instead.
-        :param pulumi.Input[str] template_id: The compute instance template (ID). Usage of the `exoscale_compute_template` data source is recommended.
+        :param pulumi.Input[str] template: ❗ The compute instance template (name). Only *featured* templates are available, if you want to reference *custom templates* use the `template_id` attribute instead.
+        :param pulumi.Input[str] template_id: ❗ The compute instance template (ID). Usage of the `get_compute_template` data source is recommended.
         :param pulumi.Input[str] user_data: cloud-init configuration (no need to base64-encode or gzip it as the provider will take care of it).
         :param pulumi.Input[bool] user_data_base64: was the cloud-init configuration base64 encoded
-        :param pulumi.Input[str] username: The user to use to connect to the instance. If you've referenced a *custom template* in the resource, use the
-               `exoscale_compute_template` data source `username` attribute instead.
-        :param pulumi.Input[str] zone: The Exoscale Zone name.
+        :param pulumi.Input[str] username: The user to use to connect to the instance. If you've referenced a *custom template* in the resource, use the `get_compute_template` data source `username` attribute instead.
+        :param pulumi.Input[str] zone: ❗ The Exoscale Zone name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ComputeState.__new__(_ComputeState)
 
         __props__.__dict__["affinity_group_ids"] = affinity_group_ids
         __props__.__dict__["affinity_groups"] = affinity_groups
@@ -1046,23 +1007,23 @@
         __props__.__dict__["zone"] = zone
         return Compute(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="affinityGroupIds")
     def affinity_group_ids(self) -> pulumi.Output[Sequence[str]]:
         """
-        A list of anti-affinity groups (IDs; at creation time only; conflicts with `affinity_groups`).
+        ❗ A list of anti-affinity groups (IDs; at creation time only; conflicts with `affinity_groups`).
         """
         return pulumi.get(self, "affinity_group_ids")
 
     @property
     @pulumi.getter(name="affinityGroups")
     def affinity_groups(self) -> pulumi.Output[Sequence[str]]:
         """
-        A list of anti-affinity groups (names; at creation time only; conflicts with `affinity_group_ids`).
+        ❗ A list of anti-affinity groups (names; at creation time only; conflicts with `affinity_group_ids`).
         """
         return pulumi.get(self, "affinity_groups")
 
     @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> pulumi.Output[int]:
         """
@@ -1070,33 +1031,28 @@
         """
         return pulumi.get(self, "disk_size")
 
     @property
     @pulumi.getter(name="displayName")
     def display_name(self) -> pulumi.Output[str]:
         """
-        The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS'
-        *hostname* during creation, so the value must contain only alphanumeric and hyphen (" - ") characters; it can be changed
-        to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will
-        be generated automatically.
+        The displayed instance name. Note: if the `hostname` attribute is not set, this attribute is also used to set the OS' *hostname* during creation, so the value must contain only alphanumeric and hyphen (" - ") characters; it can be changed to any character during a later update. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically.
         """
         return pulumi.get(self, "display_name")
 
     @property
     @pulumi.getter
     def gateway(self) -> pulumi.Output[str]:
         return pulumi.get(self, "gateway")
 
     @property
     @pulumi.getter
     def hostname(self) -> pulumi.Output[str]:
         """
-        The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or
-        `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value
-        requires to reboot the instance.
+        The instance hostname, must contain only alphanumeric and hyphen (`-`) characters. If neither `display_name` or `hostname` attributes are set, a random value will be generated automatically. Note: updating this attribute's value requires to reboot the instance.
         """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def ip4(self) -> pulumi.Output[Optional[bool]]:
         """
@@ -1133,33 +1089,35 @@
         """
         return pulumi.get(self, "ip_address")
 
     @property
     @pulumi.getter(name="keyPair")
     def key_pair(self) -> pulumi.Output[Optional[str]]:
         """
-        The SSH keypair (name) to authorize in the instance.
+        ❗ The SSH keypair (name) to authorize in the instance.
         """
         return pulumi.get(self, "key_pair")
 
     @property
     @pulumi.getter
     def keyboard(self) -> pulumi.Output[Optional[str]]:
         """
-        The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`,
-        `pt`, `uk`, `us`; at creation time only).
+        The keyboard layout configuration (`de`, `de-ch`, `es`, `fi`, `fr`, `fr-be`, `fr-ch`, `is`, `it`, `jp`, `nl-be`, `no`, `pt`, `uk`, `us`; at creation time only).
         """
         return pulumi.get(self, "keyboard")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
         The instance hostname. Please use the `hostname` argument instead.
         """
+        warnings.warn("""use `hostname` attribute instead""", DeprecationWarning)
+        pulumi.log.warn("""name is deprecated: use `hostname` attribute instead""")
+
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Output[str]:
         """
         The instance initial password and/or encrypted password.
@@ -1214,24 +1172,23 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def template(self) -> pulumi.Output[str]:
         """
-        The compute instance template (name). Only *featured* templates are available, if you want to reference *custom
-        templates* use the `template_id` attribute instead.
+        ❗ The compute instance template (name). Only *featured* templates are available, if you want to reference *custom templates* use the `template_id` attribute instead.
         """
         return pulumi.get(self, "template")
 
     @property
     @pulumi.getter(name="templateId")
     def template_id(self) -> pulumi.Output[str]:
         """
-        The compute instance template (ID). Usage of the `exoscale_compute_template` data source is recommended.
+        ❗ The compute instance template (ID). Usage of the `get_compute_template` data source is recommended.
         """
         return pulumi.get(self, "template_id")
 
     @property
     @pulumi.getter(name="userData")
     def user_data(self) -> pulumi.Output[Optional[str]]:
         """
@@ -1247,20 +1204,22 @@
         """
         return pulumi.get(self, "user_data_base64")
 
     @property
     @pulumi.getter
     def username(self) -> pulumi.Output[str]:
         """
-        The user to use to connect to the instance. If you've referenced a *custom template* in the resource, use the
-        `exoscale_compute_template` data source `username` attribute instead.
+        The user to use to connect to the instance. If you've referenced a *custom template* in the resource, use the `get_compute_template` data source `username` attribute instead.
         """
+        warnings.warn("""broken, use `compute_template` data source `username` attribute""", DeprecationWarning)
+        pulumi.log.warn("""username is deprecated: broken, use `compute_template` data source `username` attribute""")
+
         return pulumi.get(self, "username")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale Zone name.
+        ❗ The Exoscale Zone name.
         """
         return pulumi.get(self, "zone")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/compute_instance.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/compute_instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,35 +31,31 @@
                  reverse_dns: Optional[pulumi.Input[str]] = None,
                  security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ssh_key: Optional[pulumi.Input[str]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  user_data: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ComputeInstance resource.
-        :param pulumi.Input[str] template_id: The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the instance.
-        :param pulumi.Input[str] type: The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) -
-               `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts
-               the instance.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to attach to the instance (may only be set at
-               creation time).
-        :param pulumi.Input[str] deploy_target_id: A deploy target ID.
+        :param pulumi.Input[str] template_id: ❗ The exoscale*compute*template (ID) to use when creating the instance.
+        :param pulumi.Input[str] type: The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts the instance.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: ❗ A list of exoscale*anti*affinity_group (IDs) to attach to the instance (may only be set at creation time).
+        :param pulumi.Input[str] deploy_target_id: ❗ A deploy target ID.
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`). **WARNING**: updating this attribute stops/restarts the instance.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs) to attach to the instance.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of exoscale*elastic*ip (IDs) to attach to the instance.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on the instance (boolean; default: `false`).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The compute instance name.
         :param pulumi.Input[Sequence[pulumi.Input['ComputeInstanceNetworkInterfaceArgs']]] network_interfaces: Private network interfaces (may be specified multiple times). Structure is documented below.
         :param pulumi.Input[bool] private: Whether the instance is private (no public IP addresses; default: false)
         :param pulumi.Input[str] reverse_dns: Domain name for reverse DNS record.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_group.md) (IDs) to attach to the instance.
-        :param pulumi.Input[str] ssh_key: The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the instance (may only be set at creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of exoscale*security*group (IDs) to attach to the instance.
+        :param pulumi.Input[str] ssh_key: The exoscale*ssh*key (name) to authorize in the instance (may only be set at creation time).
         :param pulumi.Input[str] state: The instance state (`running` or `stopped`; default: `running`).
-        :param pulumi.Input[str] user_data: [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will
-               take care of it).
+        :param pulumi.Input[str] user_data: [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will take care of it).
         """
         pulumi.set(__self__, "template_id", template_id)
         pulumi.set(__self__, "type", type)
         pulumi.set(__self__, "zone", zone)
         if anti_affinity_group_ids is not None:
             pulumi.set(__self__, "anti_affinity_group_ids", anti_affinity_group_ids)
         if deploy_target_id is not None:
@@ -89,66 +85,63 @@
         if user_data is not None:
             pulumi.set(__self__, "user_data", user_data)
 
     @property
     @pulumi.getter(name="templateId")
     def template_id(self) -> pulumi.Input[str]:
         """
-        The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the instance.
+        ❗ The exoscale*compute*template (ID) to use when creating the instance.
         """
         return pulumi.get(self, "template_id")
 
     @template_id.setter
     def template_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "template_id", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         """
-        The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) -
-        `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts
-        the instance.
+        The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts the instance.
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
     @property
     @pulumi.getter(name="antiAffinityGroupIds")
     def anti_affinity_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to attach to the instance (may only be set at
-        creation time).
+        ❗ A list of exoscale*anti*affinity_group (IDs) to attach to the instance (may only be set at creation time).
         """
         return pulumi.get(self, "anti_affinity_group_ids")
 
     @anti_affinity_group_ids.setter
     def anti_affinity_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "anti_affinity_group_ids", value)
 
     @property
     @pulumi.getter(name="deployTargetId")
     def deploy_target_id(self) -> Optional[pulumi.Input[str]]:
         """
-        A deploy target ID.
+        ❗ A deploy target ID.
         """
         return pulumi.get(self, "deploy_target_id")
 
     @deploy_target_id.setter
     def deploy_target_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "deploy_target_id", value)
 
@@ -164,15 +157,15 @@
     def disk_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "disk_size", value)
 
     @property
     @pulumi.getter(name="elasticIpIds")
     def elastic_ip_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs) to attach to the instance.
+        A list of exoscale*elastic*ip (IDs) to attach to the instance.
         """
         return pulumi.get(self, "elastic_ip_ids")
 
     @elastic_ip_ids.setter
     def elastic_ip_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "elastic_ip_ids", value)
 
@@ -248,27 +241,27 @@
     def reverse_dns(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "reverse_dns", value)
 
     @property
     @pulumi.getter(name="securityGroupIds")
     def security_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of [exoscale_security_group](./security_group.md) (IDs) to attach to the instance.
+        A list of exoscale*security*group (IDs) to attach to the instance.
         """
         return pulumi.get(self, "security_group_ids")
 
     @security_group_ids.setter
     def security_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "security_group_ids", value)
 
     @property
     @pulumi.getter(name="sshKey")
     def ssh_key(self) -> Optional[pulumi.Input[str]]:
         """
-        The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the instance (may only be set at creation time).
+        The exoscale*ssh*key (name) to authorize in the instance (may only be set at creation time).
         """
         return pulumi.get(self, "ssh_key")
 
     @ssh_key.setter
     def ssh_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ssh_key", value)
 
@@ -284,16 +277,15 @@
     def state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "state", value)
 
     @property
     @pulumi.getter(name="userData")
     def user_data(self) -> Optional[pulumi.Input[str]]:
         """
-        [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will
-        take care of it).
+        [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will take care of it).
         """
         return pulumi.get(self, "user_data")
 
     @user_data.setter
     def user_data(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_data", value)
 
@@ -320,40 +312,35 @@
                  state: Optional[pulumi.Input[str]] = None,
                  template_id: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  user_data: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ComputeInstance resources.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to attach to the instance (may only be set at
-               creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: ❗ A list of exoscale*anti*affinity_group (IDs) to attach to the instance (may only be set at creation time).
         :param pulumi.Input[str] created_at: The instance creation date.
-        :param pulumi.Input[str] deploy_target_id: A deploy target ID.
+        :param pulumi.Input[str] deploy_target_id: ❗ A deploy target ID.
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`). **WARNING**: updating this attribute stops/restarts the instance.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs) to attach to the instance.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of exoscale*elastic*ip (IDs) to attach to the instance.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on the instance (boolean; default: `false`).
         :param pulumi.Input[str] ipv6_address: The instance (main network interface) IPv6 address (if enabled).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The compute instance name.
         :param pulumi.Input[Sequence[pulumi.Input['ComputeInstanceNetworkInterfaceArgs']]] network_interfaces: Private network interfaces (may be specified multiple times). Structure is documented below.
         :param pulumi.Input[bool] private: Whether the instance is private (no public IP addresses; default: false)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of private networks (IDs) attached to the instance. Please use the `network_interface.*.network_id` argument
-               instead.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of private networks (IDs) attached to the instance. Please use the `network_interface.*.network_id` argument instead.
         :param pulumi.Input[str] public_ip_address: The instance (main network interface) IPv4 address.
         :param pulumi.Input[str] reverse_dns: Domain name for reverse DNS record.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_group.md) (IDs) to attach to the instance.
-        :param pulumi.Input[str] ssh_key: The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the instance (may only be set at creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of exoscale*security*group (IDs) to attach to the instance.
+        :param pulumi.Input[str] ssh_key: The exoscale*ssh*key (name) to authorize in the instance (may only be set at creation time).
         :param pulumi.Input[str] state: The instance state (`running` or `stopped`; default: `running`).
-        :param pulumi.Input[str] template_id: The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the instance.
-        :param pulumi.Input[str] type: The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) -
-               `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts
-               the instance.
-        :param pulumi.Input[str] user_data: [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will
-               take care of it).
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] template_id: ❗ The exoscale*compute*template (ID) to use when creating the instance.
+        :param pulumi.Input[str] type: The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts the instance.
+        :param pulumi.Input[str] user_data: [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will take care of it).
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if anti_affinity_group_ids is not None:
             pulumi.set(__self__, "anti_affinity_group_ids", anti_affinity_group_ids)
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
         if deploy_target_id is not None:
             pulumi.set(__self__, "deploy_target_id", deploy_target_id)
@@ -397,16 +384,15 @@
         if zone is not None:
             pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter(name="antiAffinityGroupIds")
     def anti_affinity_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to attach to the instance (may only be set at
-        creation time).
+        ❗ A list of exoscale*anti*affinity_group (IDs) to attach to the instance (may only be set at creation time).
         """
         return pulumi.get(self, "anti_affinity_group_ids")
 
     @anti_affinity_group_ids.setter
     def anti_affinity_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "anti_affinity_group_ids", value)
 
@@ -422,15 +408,15 @@
     def created_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_at", value)
 
     @property
     @pulumi.getter(name="deployTargetId")
     def deploy_target_id(self) -> Optional[pulumi.Input[str]]:
         """
-        A deploy target ID.
+        ❗ A deploy target ID.
         """
         return pulumi.get(self, "deploy_target_id")
 
     @deploy_target_id.setter
     def deploy_target_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "deploy_target_id", value)
 
@@ -446,15 +432,15 @@
     def disk_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "disk_size", value)
 
     @property
     @pulumi.getter(name="elasticIpIds")
     def elastic_ip_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs) to attach to the instance.
+        A list of exoscale*elastic*ip (IDs) to attach to the instance.
         """
         return pulumi.get(self, "elastic_ip_ids")
 
     @elastic_ip_ids.setter
     def elastic_ip_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "elastic_ip_ids", value)
 
@@ -530,17 +516,19 @@
     def private(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "private", value)
 
     @property
     @pulumi.getter(name="privateNetworkIds")
     def private_network_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of private networks (IDs) attached to the instance. Please use the `network_interface.*.network_id` argument
-        instead.
+        A list of private networks (IDs) attached to the instance. Please use the `network_interface.*.network_id` argument instead.
         """
+        warnings.warn("""Use the network_interface block instead.""", DeprecationWarning)
+        pulumi.log.warn("""private_network_ids is deprecated: Use the network_interface block instead.""")
+
         return pulumi.get(self, "private_network_ids")
 
     @private_network_ids.setter
     def private_network_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "private_network_ids", value)
 
     @property
@@ -567,27 +555,27 @@
     def reverse_dns(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "reverse_dns", value)
 
     @property
     @pulumi.getter(name="securityGroupIds")
     def security_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of [exoscale_security_group](./security_group.md) (IDs) to attach to the instance.
+        A list of exoscale*security*group (IDs) to attach to the instance.
         """
         return pulumi.get(self, "security_group_ids")
 
     @security_group_ids.setter
     def security_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "security_group_ids", value)
 
     @property
     @pulumi.getter(name="sshKey")
     def ssh_key(self) -> Optional[pulumi.Input[str]]:
         """
-        The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the instance (may only be set at creation time).
+        The exoscale*ssh*key (name) to authorize in the instance (may only be set at creation time).
         """
         return pulumi.get(self, "ssh_key")
 
     @ssh_key.setter
     def ssh_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ssh_key", value)
 
@@ -603,54 +591,51 @@
     def state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "state", value)
 
     @property
     @pulumi.getter(name="templateId")
     def template_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the instance.
+        ❗ The exoscale*compute*template (ID) to use when creating the instance.
         """
         return pulumi.get(self, "template_id")
 
     @template_id.setter
     def template_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "template_id", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) -
-        `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts
-        the instance.
+        The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts the instance.
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter(name="userData")
     def user_data(self) -> Optional[pulumi.Input[str]]:
         """
-        [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will
-        take care of it).
+        [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will take care of it).
         """
         return pulumi.get(self, "user_data")
 
     @user_data.setter
     def user_data(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_data", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -689,35 +674,31 @@
 
          exoscale_compute_instance.my_instance \\
 
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to attach to the instance (may only be set at
-               creation time).
-        :param pulumi.Input[str] deploy_target_id: A deploy target ID.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: ❗ A list of exoscale*anti*affinity_group (IDs) to attach to the instance (may only be set at creation time).
+        :param pulumi.Input[str] deploy_target_id: ❗ A deploy target ID.
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`). **WARNING**: updating this attribute stops/restarts the instance.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs) to attach to the instance.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of exoscale*elastic*ip (IDs) to attach to the instance.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on the instance (boolean; default: `false`).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The compute instance name.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ComputeInstanceNetworkInterfaceArgs']]]] network_interfaces: Private network interfaces (may be specified multiple times). Structure is documented below.
         :param pulumi.Input[bool] private: Whether the instance is private (no public IP addresses; default: false)
         :param pulumi.Input[str] reverse_dns: Domain name for reverse DNS record.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_group.md) (IDs) to attach to the instance.
-        :param pulumi.Input[str] ssh_key: The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the instance (may only be set at creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of exoscale*security*group (IDs) to attach to the instance.
+        :param pulumi.Input[str] ssh_key: The exoscale*ssh*key (name) to authorize in the instance (may only be set at creation time).
         :param pulumi.Input[str] state: The instance state (`running` or `stopped`; default: `running`).
-        :param pulumi.Input[str] template_id: The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the instance.
-        :param pulumi.Input[str] type: The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) -
-               `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts
-               the instance.
-        :param pulumi.Input[str] user_data: [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will
-               take care of it).
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] template_id: ❗ The exoscale*compute*template (ID) to use when creating the instance.
+        :param pulumi.Input[str] type: The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts the instance.
+        :param pulumi.Input[str] user_data: [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will take care of it).
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ComputeInstanceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -836,40 +817,35 @@
         """
         Get an existing ComputeInstance resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to attach to the instance (may only be set at
-               creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: ❗ A list of exoscale*anti*affinity_group (IDs) to attach to the instance (may only be set at creation time).
         :param pulumi.Input[str] created_at: The instance creation date.
-        :param pulumi.Input[str] deploy_target_id: A deploy target ID.
+        :param pulumi.Input[str] deploy_target_id: ❗ A deploy target ID.
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`). **WARNING**: updating this attribute stops/restarts the instance.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs) to attach to the instance.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of exoscale*elastic*ip (IDs) to attach to the instance.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on the instance (boolean; default: `false`).
         :param pulumi.Input[str] ipv6_address: The instance (main network interface) IPv6 address (if enabled).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The compute instance name.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ComputeInstanceNetworkInterfaceArgs']]]] network_interfaces: Private network interfaces (may be specified multiple times). Structure is documented below.
         :param pulumi.Input[bool] private: Whether the instance is private (no public IP addresses; default: false)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of private networks (IDs) attached to the instance. Please use the `network_interface.*.network_id` argument
-               instead.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of private networks (IDs) attached to the instance. Please use the `network_interface.*.network_id` argument instead.
         :param pulumi.Input[str] public_ip_address: The instance (main network interface) IPv4 address.
         :param pulumi.Input[str] reverse_dns: Domain name for reverse DNS record.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_group.md) (IDs) to attach to the instance.
-        :param pulumi.Input[str] ssh_key: The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the instance (may only be set at creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of exoscale*security*group (IDs) to attach to the instance.
+        :param pulumi.Input[str] ssh_key: The exoscale*ssh*key (name) to authorize in the instance (may only be set at creation time).
         :param pulumi.Input[str] state: The instance state (`running` or `stopped`; default: `running`).
-        :param pulumi.Input[str] template_id: The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the instance.
-        :param pulumi.Input[str] type: The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) -
-               `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts
-               the instance.
-        :param pulumi.Input[str] user_data: [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will
-               take care of it).
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] template_id: ❗ The exoscale*compute*template (ID) to use when creating the instance.
+        :param pulumi.Input[str] type: The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts the instance.
+        :param pulumi.Input[str] user_data: [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will take care of it).
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ComputeInstanceState.__new__(_ComputeInstanceState)
 
         __props__.__dict__["anti_affinity_group_ids"] = anti_affinity_group_ids
         __props__.__dict__["created_at"] = created_at
@@ -894,16 +870,15 @@
         __props__.__dict__["zone"] = zone
         return ComputeInstance(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="antiAffinityGroupIds")
     def anti_affinity_group_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to attach to the instance (may only be set at
-        creation time).
+        ❗ A list of exoscale*anti*affinity_group (IDs) to attach to the instance (may only be set at creation time).
         """
         return pulumi.get(self, "anti_affinity_group_ids")
 
     @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> pulumi.Output[str]:
         """
@@ -911,15 +886,15 @@
         """
         return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter(name="deployTargetId")
     def deploy_target_id(self) -> pulumi.Output[Optional[str]]:
         """
-        A deploy target ID.
+        ❗ A deploy target ID.
         """
         return pulumi.get(self, "deploy_target_id")
 
     @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> pulumi.Output[int]:
         """
@@ -927,15 +902,15 @@
         """
         return pulumi.get(self, "disk_size")
 
     @property
     @pulumi.getter(name="elasticIpIds")
     def elastic_ip_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs) to attach to the instance.
+        A list of exoscale*elastic*ip (IDs) to attach to the instance.
         """
         return pulumi.get(self, "elastic_ip_ids")
 
     @property
     @pulumi.getter
     def ipv6(self) -> pulumi.Output[Optional[bool]]:
         """
@@ -983,17 +958,19 @@
         """
         return pulumi.get(self, "private")
 
     @property
     @pulumi.getter(name="privateNetworkIds")
     def private_network_ids(self) -> pulumi.Output[Sequence[str]]:
         """
-        A list of private networks (IDs) attached to the instance. Please use the `network_interface.*.network_id` argument
-        instead.
+        A list of private networks (IDs) attached to the instance. Please use the `network_interface.*.network_id` argument instead.
         """
+        warnings.warn("""Use the network_interface block instead.""", DeprecationWarning)
+        pulumi.log.warn("""private_network_ids is deprecated: Use the network_interface block instead.""")
+
         return pulumi.get(self, "private_network_ids")
 
     @property
     @pulumi.getter(name="publicIpAddress")
     def public_ip_address(self) -> pulumi.Output[str]:
         """
         The instance (main network interface) IPv4 address.
@@ -1008,23 +985,23 @@
         """
         return pulumi.get(self, "reverse_dns")
 
     @property
     @pulumi.getter(name="securityGroupIds")
     def security_group_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of [exoscale_security_group](./security_group.md) (IDs) to attach to the instance.
+        A list of exoscale*security*group (IDs) to attach to the instance.
         """
         return pulumi.get(self, "security_group_ids")
 
     @property
     @pulumi.getter(name="sshKey")
     def ssh_key(self) -> pulumi.Output[Optional[str]]:
         """
-        The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the instance (may only be set at creation time).
+        The exoscale*ssh*key (name) to authorize in the instance (may only be set at creation time).
         """
         return pulumi.get(self, "ssh_key")
 
     @property
     @pulumi.getter
     def state(self) -> pulumi.Output[str]:
         """
@@ -1032,38 +1009,35 @@
         """
         return pulumi.get(self, "state")
 
     @property
     @pulumi.getter(name="templateId")
     def template_id(self) -> pulumi.Output[str]:
         """
-        The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the instance.
+        ❗ The exoscale*compute*template (ID) to use when creating the instance.
         """
         return pulumi.get(self, "template_id")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
-        The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) -
-        `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts
-        the instance.
+        The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts the instance.
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="userData")
     def user_data(self) -> pulumi.Output[Optional[str]]:
         """
-        [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will
-        take care of it).
+        [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will take care of it).
         """
         return pulumi.get(self, "user_data")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/config/vars.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/database.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,24 +26,22 @@
                  name: Optional[pulumi.Input[str]] = None,
                  opensearch: Optional[pulumi.Input['DatabaseOpensearchArgs']] = None,
                  pg: Optional[pulumi.Input['DatabasePgArgs']] = None,
                  redis: Optional[pulumi.Input['DatabaseRedisArgs']] = None,
                  termination_protection: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Database resource.
-        :param pulumi.Input[str] plan: The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show
-               <TYPE>` - for reference).
-        :param pulumi.Input[str] type: The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] plan: The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show <TYPE>` - for reference).
+        :param pulumi.Input[str] type: ❗ The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         :param pulumi.Input['DatabaseKafkaArgs'] kafka: *kafka* database service type specific arguments.
-        :param pulumi.Input[str] maintenance_dow: The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`,
-               `thursday`, `friday`, `saturday`, `sunday`).
+        :param pulumi.Input[str] maintenance_dow: The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`).
         :param pulumi.Input[str] maintenance_time: The time of day to perform the automated database service maintenance (`HH:MM:SS`)
         :param pulumi.Input['DatabaseMysqlArgs'] mysql: *mysql* database service type specific arguments.
-        :param pulumi.Input[str] name: The name of the database service.
+        :param pulumi.Input[str] name: ❗ The name of the database service.
         :param pulumi.Input['DatabaseOpensearchArgs'] opensearch: *opensearch* database service type specific arguments.
         :param pulumi.Input['DatabasePgArgs'] pg: *pg* database service type specific arguments. Structure is documented below.
         :param pulumi.Input['DatabaseRedisArgs'] redis: *redis* database service type specific arguments. Structure is documented below.
         :param pulumi.Input[bool] termination_protection: The database service protection boolean flag against termination/power-off.
         """
         pulumi.set(__self__, "plan", plan)
         pulumi.set(__self__, "type", type)
@@ -67,40 +65,39 @@
         if termination_protection is not None:
             pulumi.set(__self__, "termination_protection", termination_protection)
 
     @property
     @pulumi.getter
     def plan(self) -> pulumi.Input[str]:
         """
-        The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show
-        <TYPE>` - for reference).
+        The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show <TYPE>` - for reference).
         """
         return pulumi.get(self, "plan")
 
     @plan.setter
     def plan(self, value: pulumi.Input[str]):
         pulumi.set(self, "plan", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         """
-        The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
+        ❗ The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
@@ -116,16 +113,15 @@
     def kafka(self, value: Optional[pulumi.Input['DatabaseKafkaArgs']]):
         pulumi.set(self, "kafka", value)
 
     @property
     @pulumi.getter(name="maintenanceDow")
     def maintenance_dow(self) -> Optional[pulumi.Input[str]]:
         """
-        The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`,
-        `thursday`, `friday`, `saturday`, `sunday`).
+        The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`).
         """
         return pulumi.get(self, "maintenance_dow")
 
     @maintenance_dow.setter
     def maintenance_dow(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "maintenance_dow", value)
 
@@ -153,15 +149,15 @@
     def mysql(self, value: Optional[pulumi.Input['DatabaseMysqlArgs']]):
         pulumi.set(self, "mysql", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the database service.
+        ❗ The name of the database service.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -239,32 +235,30 @@
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Database resources.
         :param pulumi.Input[str] ca_certificate: CA Certificate required to reach a DBaaS service through a TLS-protected connection.
         :param pulumi.Input[str] created_at: The creation date of the database service.
         :param pulumi.Input[int] disk_size: The disk size of the database service.
         :param pulumi.Input['DatabaseKafkaArgs'] kafka: *kafka* database service type specific arguments.
-        :param pulumi.Input[str] maintenance_dow: The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`,
-               `thursday`, `friday`, `saturday`, `sunday`).
+        :param pulumi.Input[str] maintenance_dow: The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`).
         :param pulumi.Input[str] maintenance_time: The time of day to perform the automated database service maintenance (`HH:MM:SS`)
         :param pulumi.Input['DatabaseMysqlArgs'] mysql: *mysql* database service type specific arguments.
-        :param pulumi.Input[str] name: The name of the database service.
+        :param pulumi.Input[str] name: ❗ The name of the database service.
         :param pulumi.Input[int] node_cpus: The number of CPUs of the database service.
         :param pulumi.Input[int] node_memory: The amount of memory of the database service.
         :param pulumi.Input[int] nodes: The number of nodes of the database service.
         :param pulumi.Input['DatabaseOpensearchArgs'] opensearch: *opensearch* database service type specific arguments.
         :param pulumi.Input['DatabasePgArgs'] pg: *pg* database service type specific arguments. Structure is documented below.
-        :param pulumi.Input[str] plan: The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show
-               <TYPE>` - for reference).
+        :param pulumi.Input[str] plan: The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show <TYPE>` - for reference).
         :param pulumi.Input['DatabaseRedisArgs'] redis: *redis* database service type specific arguments. Structure is documented below.
         :param pulumi.Input[str] state: The current state of the database service.
         :param pulumi.Input[bool] termination_protection: The database service protection boolean flag against termination/power-off.
-        :param pulumi.Input[str] type: The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
+        :param pulumi.Input[str] type: ❗ The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
         :param pulumi.Input[str] updated_at: The date of the latest database service update.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if ca_certificate is not None:
             pulumi.set(__self__, "ca_certificate", ca_certificate)
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
         if disk_size is not None:
             pulumi.set(__self__, "disk_size", disk_size)
@@ -351,16 +345,15 @@
     def kafka(self, value: Optional[pulumi.Input['DatabaseKafkaArgs']]):
         pulumi.set(self, "kafka", value)
 
     @property
     @pulumi.getter(name="maintenanceDow")
     def maintenance_dow(self) -> Optional[pulumi.Input[str]]:
         """
-        The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`,
-        `thursday`, `friday`, `saturday`, `sunday`).
+        The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`).
         """
         return pulumi.get(self, "maintenance_dow")
 
     @maintenance_dow.setter
     def maintenance_dow(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "maintenance_dow", value)
 
@@ -388,15 +381,15 @@
     def mysql(self, value: Optional[pulumi.Input['DatabaseMysqlArgs']]):
         pulumi.set(self, "mysql", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the database service.
+        ❗ The name of the database service.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -460,16 +453,15 @@
     def pg(self, value: Optional[pulumi.Input['DatabasePgArgs']]):
         pulumi.set(self, "pg", value)
 
     @property
     @pulumi.getter
     def plan(self) -> Optional[pulumi.Input[str]]:
         """
-        The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show
-        <TYPE>` - for reference).
+        The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show <TYPE>` - for reference).
         """
         return pulumi.get(self, "plan")
 
     @plan.setter
     def plan(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "plan", value)
 
@@ -509,15 +501,15 @@
     def termination_protection(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "termination_protection", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
+        ❗ The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -533,15 +525,15 @@
     def updated_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "updated_at", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -576,27 +568,25 @@
          exoscale_database.my_database \\
 
          my-database@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['DatabaseKafkaArgs']] kafka: *kafka* database service type specific arguments.
-        :param pulumi.Input[str] maintenance_dow: The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`,
-               `thursday`, `friday`, `saturday`, `sunday`).
+        :param pulumi.Input[str] maintenance_dow: The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`).
         :param pulumi.Input[str] maintenance_time: The time of day to perform the automated database service maintenance (`HH:MM:SS`)
         :param pulumi.Input[pulumi.InputType['DatabaseMysqlArgs']] mysql: *mysql* database service type specific arguments.
-        :param pulumi.Input[str] name: The name of the database service.
+        :param pulumi.Input[str] name: ❗ The name of the database service.
         :param pulumi.Input[pulumi.InputType['DatabaseOpensearchArgs']] opensearch: *opensearch* database service type specific arguments.
         :param pulumi.Input[pulumi.InputType['DatabasePgArgs']] pg: *pg* database service type specific arguments. Structure is documented below.
-        :param pulumi.Input[str] plan: The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show
-               <TYPE>` - for reference).
+        :param pulumi.Input[str] plan: The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show <TYPE>` - for reference).
         :param pulumi.Input[pulumi.InputType['DatabaseRedisArgs']] redis: *redis* database service type specific arguments. Structure is documented below.
         :param pulumi.Input[bool] termination_protection: The database service protection boolean flag against termination/power-off.
-        :param pulumi.Input[str] type: The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] type: ❗ The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: DatabaseArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -712,32 +702,30 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] ca_certificate: CA Certificate required to reach a DBaaS service through a TLS-protected connection.
         :param pulumi.Input[str] created_at: The creation date of the database service.
         :param pulumi.Input[int] disk_size: The disk size of the database service.
         :param pulumi.Input[pulumi.InputType['DatabaseKafkaArgs']] kafka: *kafka* database service type specific arguments.
-        :param pulumi.Input[str] maintenance_dow: The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`,
-               `thursday`, `friday`, `saturday`, `sunday`).
+        :param pulumi.Input[str] maintenance_dow: The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`).
         :param pulumi.Input[str] maintenance_time: The time of day to perform the automated database service maintenance (`HH:MM:SS`)
         :param pulumi.Input[pulumi.InputType['DatabaseMysqlArgs']] mysql: *mysql* database service type specific arguments.
-        :param pulumi.Input[str] name: The name of the database service.
+        :param pulumi.Input[str] name: ❗ The name of the database service.
         :param pulumi.Input[int] node_cpus: The number of CPUs of the database service.
         :param pulumi.Input[int] node_memory: The amount of memory of the database service.
         :param pulumi.Input[int] nodes: The number of nodes of the database service.
         :param pulumi.Input[pulumi.InputType['DatabaseOpensearchArgs']] opensearch: *opensearch* database service type specific arguments.
         :param pulumi.Input[pulumi.InputType['DatabasePgArgs']] pg: *pg* database service type specific arguments. Structure is documented below.
-        :param pulumi.Input[str] plan: The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show
-               <TYPE>` - for reference).
+        :param pulumi.Input[str] plan: The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show <TYPE>` - for reference).
         :param pulumi.Input[pulumi.InputType['DatabaseRedisArgs']] redis: *redis* database service type specific arguments. Structure is documented below.
         :param pulumi.Input[str] state: The current state of the database service.
         :param pulumi.Input[bool] termination_protection: The database service protection boolean flag against termination/power-off.
-        :param pulumi.Input[str] type: The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
+        :param pulumi.Input[str] type: ❗ The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
         :param pulumi.Input[str] updated_at: The date of the latest database service update.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _DatabaseState.__new__(_DatabaseState)
 
         __props__.__dict__["ca_certificate"] = ca_certificate
         __props__.__dict__["created_at"] = created_at
@@ -793,16 +781,15 @@
         """
         return pulumi.get(self, "kafka")
 
     @property
     @pulumi.getter(name="maintenanceDow")
     def maintenance_dow(self) -> pulumi.Output[str]:
         """
-        The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`,
-        `thursday`, `friday`, `saturday`, `sunday`).
+        The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`).
         """
         return pulumi.get(self, "maintenance_dow")
 
     @property
     @pulumi.getter(name="maintenanceTime")
     def maintenance_time(self) -> pulumi.Output[str]:
         """
@@ -818,15 +805,15 @@
         """
         return pulumi.get(self, "mysql")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The name of the database service.
+        ❗ The name of the database service.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="nodeCpus")
     def node_cpus(self) -> pulumi.Output[int]:
         """
@@ -866,16 +853,15 @@
         """
         return pulumi.get(self, "pg")
 
     @property
     @pulumi.getter
     def plan(self) -> pulumi.Output[str]:
         """
-        The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show
-        <TYPE>` - for reference).
+        The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show <TYPE>` - for reference).
         """
         return pulumi.get(self, "plan")
 
     @property
     @pulumi.getter
     def redis(self) -> pulumi.Output[Optional['outputs.DatabaseRedis']]:
         """
@@ -899,15 +885,15 @@
         """
         return pulumi.get(self, "termination_protection")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
-        The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
+        ❗ The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="updatedAt")
     def updated_at(self) -> pulumi.Output[str]:
         """
@@ -915,11 +901,11 @@
         """
         return pulumi.get(self, "updated_at")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/domain.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/domain.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 
 @pulumi.input_type
 class DomainArgs:
     def __init__(__self__, *,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Domain resource.
-        :param pulumi.Input[str] name: The DNS domain name.
+        :param pulumi.Input[str] name: ❗ The DNS domain name.
         """
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The DNS domain name.
+        ❗ The DNS domain name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -43,15 +43,15 @@
                  name: Optional[pulumi.Input[str]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  token: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Domain resources.
         :param pulumi.Input[bool] auto_renew: Whether the DNS domain has automatic renewal enabled (boolean).
         :param pulumi.Input[str] expires_on: The domain expiration date, if known.
-        :param pulumi.Input[str] name: The DNS domain name.
+        :param pulumi.Input[str] name: ❗ The DNS domain name.
         :param pulumi.Input[str] state: The domain state.
         :param pulumi.Input[str] token: A security token that can be used as an alternative way to manage DNS domains via the Exoscale API.
         """
         if auto_renew is not None:
             warnings.warn("""Not used, will be removed in the future""", DeprecationWarning)
             pulumi.log.warn("""auto_renew is deprecated: Not used, will be removed in the future""")
         if auto_renew is not None:
@@ -76,62 +76,74 @@
 
     @property
     @pulumi.getter(name="autoRenew")
     def auto_renew(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether the DNS domain has automatic renewal enabled (boolean).
         """
+        warnings.warn("""Not used, will be removed in the future""", DeprecationWarning)
+        pulumi.log.warn("""auto_renew is deprecated: Not used, will be removed in the future""")
+
         return pulumi.get(self, "auto_renew")
 
     @auto_renew.setter
     def auto_renew(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "auto_renew", value)
 
     @property
     @pulumi.getter(name="expiresOn")
     def expires_on(self) -> Optional[pulumi.Input[str]]:
         """
         The domain expiration date, if known.
         """
+        warnings.warn("""Not used, will be removed in the future""", DeprecationWarning)
+        pulumi.log.warn("""expires_on is deprecated: Not used, will be removed in the future""")
+
         return pulumi.get(self, "expires_on")
 
     @expires_on.setter
     def expires_on(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "expires_on", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The DNS domain name.
+        ❗ The DNS domain name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def state(self) -> Optional[pulumi.Input[str]]:
         """
         The domain state.
         """
+        warnings.warn("""Not used, will be removed in the future""", DeprecationWarning)
+        pulumi.log.warn("""state is deprecated: Not used, will be removed in the future""")
+
         return pulumi.get(self, "state")
 
     @state.setter
     def state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "state", value)
 
     @property
     @pulumi.getter
     def token(self) -> Optional[pulumi.Input[str]]:
         """
         A security token that can be used as an alternative way to manage DNS domains via the Exoscale API.
         """
+        warnings.warn("""Not used, will be removed in the future""", DeprecationWarning)
+        pulumi.log.warn("""token is deprecated: Not used, will be removed in the future""")
+
         return pulumi.get(self, "token")
 
     @token.setter
     def token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "token", value)
 
 
@@ -153,15 +165,15 @@
 
          exoscale_domain.my_domain \\
 
          89083a5c-b648-474a-0000-0000000f67bd
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] name: The DNS domain name.
+        :param pulumi.Input[str] name: ❗ The DNS domain name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[DomainArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -228,15 +240,15 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] auto_renew: Whether the DNS domain has automatic renewal enabled (boolean).
         :param pulumi.Input[str] expires_on: The domain expiration date, if known.
-        :param pulumi.Input[str] name: The DNS domain name.
+        :param pulumi.Input[str] name: ❗ The DNS domain name.
         :param pulumi.Input[str] state: The domain state.
         :param pulumi.Input[str] token: A security token that can be used as an alternative way to manage DNS domains via the Exoscale API.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _DomainState.__new__(_DomainState)
 
@@ -249,41 +261,53 @@
 
     @property
     @pulumi.getter(name="autoRenew")
     def auto_renew(self) -> pulumi.Output[bool]:
         """
         Whether the DNS domain has automatic renewal enabled (boolean).
         """
+        warnings.warn("""Not used, will be removed in the future""", DeprecationWarning)
+        pulumi.log.warn("""auto_renew is deprecated: Not used, will be removed in the future""")
+
         return pulumi.get(self, "auto_renew")
 
     @property
     @pulumi.getter(name="expiresOn")
     def expires_on(self) -> pulumi.Output[str]:
         """
         The domain expiration date, if known.
         """
+        warnings.warn("""Not used, will be removed in the future""", DeprecationWarning)
+        pulumi.log.warn("""expires_on is deprecated: Not used, will be removed in the future""")
+
         return pulumi.get(self, "expires_on")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The DNS domain name.
+        ❗ The DNS domain name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def state(self) -> pulumi.Output[str]:
         """
         The domain state.
         """
+        warnings.warn("""Not used, will be removed in the future""", DeprecationWarning)
+        pulumi.log.warn("""state is deprecated: Not used, will be removed in the future""")
+
         return pulumi.get(self, "state")
 
     @property
     @pulumi.getter
     def token(self) -> pulumi.Output[str]:
         """
         A security token that can be used as an alternative way to manage DNS domains via the Exoscale API.
         """
+        warnings.warn("""Not used, will be removed in the future""", DeprecationWarning)
+        pulumi.log.warn("""token is deprecated: Not used, will be removed in the future""")
+
         return pulumi.get(self, "token")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/domain_record.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/domain_record.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,17 +19,16 @@
                  record_type: pulumi.Input[str],
                  name: Optional[pulumi.Input[str]] = None,
                  prio: Optional[pulumi.Input[int]] = None,
                  ttl: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a DomainRecord resource.
         :param pulumi.Input[str] content: The record value.
-        :param pulumi.Input[str] domain: The parent [exoscale_domain](./domain.md) to attach the record to.
-        :param pulumi.Input[str] record_type: The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`,
-               `TXT`, `URL`).
+        :param pulumi.Input[str] domain: ❗ The parent Domain to attach the record to.
+        :param pulumi.Input[str] record_type: ❗ The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`, `TXT`, `URL`).
         :param pulumi.Input[str] name: The record name, Leave blank (`""`) to create a root record (similar to using `@` in a DNS zone file).
         :param pulumi.Input[int] prio: The record priority (for types that support it; minimum `0`).
         :param pulumi.Input[int] ttl: The record TTL (seconds; minimum `0`; default: `3600`).
         """
         pulumi.set(__self__, "content", content)
         pulumi.set(__self__, "domain", domain)
         pulumi.set(__self__, "record_type", record_type)
@@ -52,28 +51,27 @@
     def content(self, value: pulumi.Input[str]):
         pulumi.set(self, "content", value)
 
     @property
     @pulumi.getter
     def domain(self) -> pulumi.Input[str]:
         """
-        The parent [exoscale_domain](./domain.md) to attach the record to.
+        ❗ The parent Domain to attach the record to.
         """
         return pulumi.get(self, "domain")
 
     @domain.setter
     def domain(self, value: pulumi.Input[str]):
         pulumi.set(self, "domain", value)
 
     @property
     @pulumi.getter(name="recordType")
     def record_type(self) -> pulumi.Input[str]:
         """
-        The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`,
-        `TXT`, `URL`).
+        ❗ The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`, `TXT`, `URL`).
         """
         return pulumi.get(self, "record_type")
 
     @record_type.setter
     def record_type(self, value: pulumi.Input[str]):
         pulumi.set(self, "record_type", value)
 
@@ -123,20 +121,19 @@
                  name: Optional[pulumi.Input[str]] = None,
                  prio: Optional[pulumi.Input[int]] = None,
                  record_type: Optional[pulumi.Input[str]] = None,
                  ttl: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering DomainRecord resources.
         :param pulumi.Input[str] content: The record value.
-        :param pulumi.Input[str] domain: The parent [exoscale_domain](./domain.md) to attach the record to.
+        :param pulumi.Input[str] domain: ❗ The parent Domain to attach the record to.
         :param pulumi.Input[str] hostname: The record *Fully Qualified Domain Name* (FQDN). Useful for aliasing `A`/`AAAA` records with `CNAME`.
         :param pulumi.Input[str] name: The record name, Leave blank (`""`) to create a root record (similar to using `@` in a DNS zone file).
         :param pulumi.Input[int] prio: The record priority (for types that support it; minimum `0`).
-        :param pulumi.Input[str] record_type: The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`,
-               `TXT`, `URL`).
+        :param pulumi.Input[str] record_type: ❗ The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`, `TXT`, `URL`).
         :param pulumi.Input[int] ttl: The record TTL (seconds; minimum `0`; default: `3600`).
         """
         if content is not None:
             pulumi.set(__self__, "content", content)
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
         if hostname is not None:
@@ -162,15 +159,15 @@
     def content(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "content", value)
 
     @property
     @pulumi.getter
     def domain(self) -> Optional[pulumi.Input[str]]:
         """
-        The parent [exoscale_domain](./domain.md) to attach the record to.
+        ❗ The parent Domain to attach the record to.
         """
         return pulumi.get(self, "domain")
 
     @domain.setter
     def domain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "domain", value)
 
@@ -210,16 +207,15 @@
     def prio(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "prio", value)
 
     @property
     @pulumi.getter(name="recordType")
     def record_type(self) -> Optional[pulumi.Input[str]]:
         """
-        The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`,
-        `TXT`, `URL`).
+        ❗ The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`, `TXT`, `URL`).
         """
         return pulumi.get(self, "record_type")
 
     @record_type.setter
     def record_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "record_type", value)
 
@@ -260,19 +256,18 @@
          exoscale_domain_record.my_host \\
 
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] content: The record value.
-        :param pulumi.Input[str] domain: The parent [exoscale_domain](./domain.md) to attach the record to.
+        :param pulumi.Input[str] domain: ❗ The parent Domain to attach the record to.
         :param pulumi.Input[str] name: The record name, Leave blank (`""`) to create a root record (similar to using `@` in a DNS zone file).
         :param pulumi.Input[int] prio: The record priority (for types that support it; minimum `0`).
-        :param pulumi.Input[str] record_type: The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`,
-               `TXT`, `URL`).
+        :param pulumi.Input[str] record_type: ❗ The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`, `TXT`, `URL`).
         :param pulumi.Input[int] ttl: The record TTL (seconds; minimum `0`; default: `3600`).
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: DomainRecordArgs,
@@ -354,20 +349,19 @@
         Get an existing DomainRecord resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] content: The record value.
-        :param pulumi.Input[str] domain: The parent [exoscale_domain](./domain.md) to attach the record to.
+        :param pulumi.Input[str] domain: ❗ The parent Domain to attach the record to.
         :param pulumi.Input[str] hostname: The record *Fully Qualified Domain Name* (FQDN). Useful for aliasing `A`/`AAAA` records with `CNAME`.
         :param pulumi.Input[str] name: The record name, Leave blank (`""`) to create a root record (similar to using `@` in a DNS zone file).
         :param pulumi.Input[int] prio: The record priority (for types that support it; minimum `0`).
-        :param pulumi.Input[str] record_type: The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`,
-               `TXT`, `URL`).
+        :param pulumi.Input[str] record_type: ❗ The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`, `TXT`, `URL`).
         :param pulumi.Input[int] ttl: The record TTL (seconds; minimum `0`; default: `3600`).
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _DomainRecordState.__new__(_DomainRecordState)
 
         __props__.__dict__["content"] = content
@@ -387,15 +381,15 @@
         """
         return pulumi.get(self, "content")
 
     @property
     @pulumi.getter
     def domain(self) -> pulumi.Output[str]:
         """
-        The parent [exoscale_domain](./domain.md) to attach the record to.
+        ❗ The parent Domain to attach the record to.
         """
         return pulumi.get(self, "domain")
 
     @property
     @pulumi.getter
     def hostname(self) -> pulumi.Output[str]:
         """
@@ -419,16 +413,15 @@
         """
         return pulumi.get(self, "prio")
 
     @property
     @pulumi.getter(name="recordType")
     def record_type(self) -> pulumi.Output[str]:
         """
-        The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`,
-        `TXT`, `URL`).
+        ❗ The record type (`A`, `AAAA`, `ALIAS`, `CAA`, `CNAME`, `HINFO`, `MX`, `NAPTR`, `NS`, `POOL`, `SPF`, `SRV`, `SSHFP`, `TXT`, `URL`).
         """
         return pulumi.get(self, "record_type")
 
     @property
     @pulumi.getter
     def ttl(self) -> pulumi.Output[int]:
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/elastic_ip.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/elastic_ip.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
                  address_family: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  healthcheck: Optional[pulumi.Input['ElasticIPHealthcheckArgs']] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  reverse_dns: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ElasticIP resource.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
-        :param pulumi.Input[str] address_family: The Elastic IP (EIP) address family (`inet4` or `inet6`; default: `inet4`).
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] address_family: ❗ The Elastic IP (EIP) address family (`inet4` or `inet6`; default: `inet4`).
         :param pulumi.Input[str] description: A free-form text describing the Elastic IP (EIP).
         :param pulumi.Input['ElasticIPHealthcheckArgs'] healthcheck: Healthcheck configuration for *managed* EIPs. It can not be added to an existing *Unmanaged* EIP.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] reverse_dns: Domain name for reverse DNS record.
         """
         pulumi.set(__self__, "zone", zone)
         if address_family is not None:
@@ -43,27 +43,27 @@
         if reverse_dns is not None:
             pulumi.set(__self__, "reverse_dns", reverse_dns)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
     @property
     @pulumi.getter(name="addressFamily")
     def address_family(self) -> Optional[pulumi.Input[str]]:
         """
-        The Elastic IP (EIP) address family (`inet4` or `inet6`; default: `inet4`).
+        ❗ The Elastic IP (EIP) address family (`inet4` or `inet6`; default: `inet4`).
         """
         return pulumi.get(self, "address_family")
 
     @address_family.setter
     def address_family(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "address_family", value)
 
@@ -125,22 +125,22 @@
                  healthcheck: Optional[pulumi.Input['ElasticIPHealthcheckArgs']] = None,
                  ip_address: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  reverse_dns: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ElasticIP resources.
-        :param pulumi.Input[str] address_family: The Elastic IP (EIP) address family (`inet4` or `inet6`; default: `inet4`).
+        :param pulumi.Input[str] address_family: ❗ The Elastic IP (EIP) address family (`inet4` or `inet6`; default: `inet4`).
         :param pulumi.Input[str] cidr: The Elastic IP (EIP) CIDR.
         :param pulumi.Input[str] description: A free-form text describing the Elastic IP (EIP).
         :param pulumi.Input['ElasticIPHealthcheckArgs'] healthcheck: Healthcheck configuration for *managed* EIPs. It can not be added to an existing *Unmanaged* EIP.
         :param pulumi.Input[str] ip_address: The Elastic IP (EIP) IPv4 or IPv6 address.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] reverse_dns: Domain name for reverse DNS record.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if address_family is not None:
             pulumi.set(__self__, "address_family", address_family)
         if cidr is not None:
             pulumi.set(__self__, "cidr", cidr)
         if description is not None:
             pulumi.set(__self__, "description", description)
@@ -155,15 +155,15 @@
         if zone is not None:
             pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter(name="addressFamily")
     def address_family(self) -> Optional[pulumi.Input[str]]:
         """
-        The Elastic IP (EIP) address family (`inet4` or `inet6`; default: `inet4`).
+        ❗ The Elastic IP (EIP) address family (`inet4` or `inet6`; default: `inet4`).
         """
         return pulumi.get(self, "address_family")
 
     @address_family.setter
     def address_family(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "address_family", value)
 
@@ -239,15 +239,15 @@
     def reverse_dns(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "reverse_dns", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -275,20 +275,20 @@
 
          exoscale_elastic_ip.my_elastic_ip \\
 
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] address_family: The Elastic IP (EIP) address family (`inet4` or `inet6`; default: `inet4`).
+        :param pulumi.Input[str] address_family: ❗ The Elastic IP (EIP) address family (`inet4` or `inet6`; default: `inet4`).
         :param pulumi.Input[str] description: A free-form text describing the Elastic IP (EIP).
         :param pulumi.Input[pulumi.InputType['ElasticIPHealthcheckArgs']] healthcheck: Healthcheck configuration for *managed* EIPs. It can not be added to an existing *Unmanaged* EIP.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] reverse_dns: Domain name for reverse DNS record.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ElasticIPArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -366,22 +366,22 @@
         """
         Get an existing ElasticIP resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] address_family: The Elastic IP (EIP) address family (`inet4` or `inet6`; default: `inet4`).
+        :param pulumi.Input[str] address_family: ❗ The Elastic IP (EIP) address family (`inet4` or `inet6`; default: `inet4`).
         :param pulumi.Input[str] cidr: The Elastic IP (EIP) CIDR.
         :param pulumi.Input[str] description: A free-form text describing the Elastic IP (EIP).
         :param pulumi.Input[pulumi.InputType['ElasticIPHealthcheckArgs']] healthcheck: Healthcheck configuration for *managed* EIPs. It can not be added to an existing *Unmanaged* EIP.
         :param pulumi.Input[str] ip_address: The Elastic IP (EIP) IPv4 or IPv6 address.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] reverse_dns: Domain name for reverse DNS record.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ElasticIPState.__new__(_ElasticIPState)
 
         __props__.__dict__["address_family"] = address_family
         __props__.__dict__["cidr"] = cidr
@@ -393,15 +393,15 @@
         __props__.__dict__["zone"] = zone
         return ElasticIP(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="addressFamily")
     def address_family(self) -> pulumi.Output[str]:
         """
-        The Elastic IP (EIP) address family (`inet4` or `inet6`; default: `inet4`).
+        ❗ The Elastic IP (EIP) address family (`inet4` or `inet6`; default: `inet4`).
         """
         return pulumi.get(self, "address_family")
 
     @property
     @pulumi.getter
     def cidr(self) -> pulumi.Output[str]:
         """
@@ -449,11 +449,11 @@
         """
         return pulumi.get(self, "reverse_dns")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_affinity.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_affinity.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,16 +69,16 @@
     __args__ = dict()
     __args__['id'] = id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getAffinity:getAffinity', __args__, opts=opts, typ=GetAffinityResult).value
 
     return AwaitableGetAffinityResult(
-        id=__ret__.id,
-        name=__ret__.name)
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'))
 
 
 @_utilities.lift_output_func(get_affinity)
 def get_affinity_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                         name: Optional[pulumi.Input[Optional[str]]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAffinityResult]:
     """
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_anti_affinity_group.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_anti_affinity_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,17 +80,17 @@
     __args__ = dict()
     __args__['id'] = id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getAntiAffinityGroup:getAntiAffinityGroup', __args__, opts=opts, typ=GetAntiAffinityGroupResult).value
 
     return AwaitableGetAntiAffinityGroupResult(
-        id=__ret__.id,
-        instances=__ret__.instances,
-        name=__ret__.name)
+        id=pulumi.get(__ret__, 'id'),
+        instances=pulumi.get(__ret__, 'instances'),
+        name=pulumi.get(__ret__, 'name'))
 
 
 @_utilities.lift_output_func(get_anti_affinity_group)
 def get_anti_affinity_group_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                                    name: Optional[pulumi.Input[Optional[str]]] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAntiAffinityGroupResult]:
     """
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_compute.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_compute.py`

 * *Files 6% similar despite different names*

```diff
@@ -216,28 +216,28 @@
     __args__['hostname'] = hostname
     __args__['id'] = id
     __args__['tags'] = tags
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getCompute:getCompute', __args__, opts=opts, typ=GetComputeResult).value
 
     return AwaitableGetComputeResult(
-        cpu=__ret__.cpu,
-        created=__ret__.created,
-        disk_size=__ret__.disk_size,
-        hostname=__ret__.hostname,
-        id=__ret__.id,
-        ip6_address=__ret__.ip6_address,
-        ip_address=__ret__.ip_address,
-        memory=__ret__.memory,
-        private_network_ip_addresses=__ret__.private_network_ip_addresses,
-        size=__ret__.size,
-        state=__ret__.state,
-        tags=__ret__.tags,
-        template=__ret__.template,
-        zone=__ret__.zone)
+        cpu=pulumi.get(__ret__, 'cpu'),
+        created=pulumi.get(__ret__, 'created'),
+        disk_size=pulumi.get(__ret__, 'disk_size'),
+        hostname=pulumi.get(__ret__, 'hostname'),
+        id=pulumi.get(__ret__, 'id'),
+        ip6_address=pulumi.get(__ret__, 'ip6_address'),
+        ip_address=pulumi.get(__ret__, 'ip_address'),
+        memory=pulumi.get(__ret__, 'memory'),
+        private_network_ip_addresses=pulumi.get(__ret__, 'private_network_ip_addresses'),
+        size=pulumi.get(__ret__, 'size'),
+        state=pulumi.get(__ret__, 'state'),
+        tags=pulumi.get(__ret__, 'tags'),
+        template=pulumi.get(__ret__, 'template'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_compute)
 def get_compute_output(hostname: Optional[pulumi.Input[Optional[str]]] = None,
                        id: Optional[pulumi.Input[Optional[str]]] = None,
                        tags: Optional[pulumi.Input[Optional[Mapping[str, str]]]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetComputeResult]:
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_compute_instance.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_compute_instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -317,36 +317,36 @@
     __args__['labels'] = labels
     __args__['name'] = name
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getComputeInstance:getComputeInstance', __args__, opts=opts, typ=GetComputeInstanceResult).value
 
     return AwaitableGetComputeInstanceResult(
-        anti_affinity_group_ids=__ret__.anti_affinity_group_ids,
-        created_at=__ret__.created_at,
-        deploy_target_id=__ret__.deploy_target_id,
-        disk_size=__ret__.disk_size,
-        elastic_ip_ids=__ret__.elastic_ip_ids,
-        id=__ret__.id,
-        ipv6=__ret__.ipv6,
-        ipv6_address=__ret__.ipv6_address,
-        labels=__ret__.labels,
-        manager_id=__ret__.manager_id,
-        manager_type=__ret__.manager_type,
-        name=__ret__.name,
-        private_network_ids=__ret__.private_network_ids,
-        public_ip_address=__ret__.public_ip_address,
-        reverse_dns=__ret__.reverse_dns,
-        security_group_ids=__ret__.security_group_ids,
-        ssh_key=__ret__.ssh_key,
-        state=__ret__.state,
-        template_id=__ret__.template_id,
-        type=__ret__.type,
-        user_data=__ret__.user_data,
-        zone=__ret__.zone)
+        anti_affinity_group_ids=pulumi.get(__ret__, 'anti_affinity_group_ids'),
+        created_at=pulumi.get(__ret__, 'created_at'),
+        deploy_target_id=pulumi.get(__ret__, 'deploy_target_id'),
+        disk_size=pulumi.get(__ret__, 'disk_size'),
+        elastic_ip_ids=pulumi.get(__ret__, 'elastic_ip_ids'),
+        id=pulumi.get(__ret__, 'id'),
+        ipv6=pulumi.get(__ret__, 'ipv6'),
+        ipv6_address=pulumi.get(__ret__, 'ipv6_address'),
+        labels=pulumi.get(__ret__, 'labels'),
+        manager_id=pulumi.get(__ret__, 'manager_id'),
+        manager_type=pulumi.get(__ret__, 'manager_type'),
+        name=pulumi.get(__ret__, 'name'),
+        private_network_ids=pulumi.get(__ret__, 'private_network_ids'),
+        public_ip_address=pulumi.get(__ret__, 'public_ip_address'),
+        reverse_dns=pulumi.get(__ret__, 'reverse_dns'),
+        security_group_ids=pulumi.get(__ret__, 'security_group_ids'),
+        ssh_key=pulumi.get(__ret__, 'ssh_key'),
+        state=pulumi.get(__ret__, 'state'),
+        template_id=pulumi.get(__ret__, 'template_id'),
+        type=pulumi.get(__ret__, 'type'),
+        user_data=pulumi.get(__ret__, 'user_data'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_compute_instance)
 def get_compute_instance_output(anti_affinity_group_ids: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                                 id: Optional[pulumi.Input[Optional[str]]] = None,
                                 labels: Optional[pulumi.Input[Optional[Mapping[str, str]]]] = None,
                                 name: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_compute_instance_list.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_compute_instance_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -321,33 +321,33 @@
     __args__['type'] = type
     __args__['userData'] = user_data
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getComputeInstanceList:getComputeInstanceList', __args__, opts=opts, typ=GetComputeInstanceListResult).value
 
     return AwaitableGetComputeInstanceListResult(
-        created_at=__ret__.created_at,
-        deploy_target_id=__ret__.deploy_target_id,
-        disk_size=__ret__.disk_size,
-        id=__ret__.id,
-        instances=__ret__.instances,
-        ipv6=__ret__.ipv6,
-        ipv6_address=__ret__.ipv6_address,
-        labels=__ret__.labels,
-        manager_id=__ret__.manager_id,
-        manager_type=__ret__.manager_type,
-        name=__ret__.name,
-        public_ip_address=__ret__.public_ip_address,
-        reverse_dns=__ret__.reverse_dns,
-        ssh_key=__ret__.ssh_key,
-        state=__ret__.state,
-        template_id=__ret__.template_id,
-        type=__ret__.type,
-        user_data=__ret__.user_data,
-        zone=__ret__.zone)
+        created_at=pulumi.get(__ret__, 'created_at'),
+        deploy_target_id=pulumi.get(__ret__, 'deploy_target_id'),
+        disk_size=pulumi.get(__ret__, 'disk_size'),
+        id=pulumi.get(__ret__, 'id'),
+        instances=pulumi.get(__ret__, 'instances'),
+        ipv6=pulumi.get(__ret__, 'ipv6'),
+        ipv6_address=pulumi.get(__ret__, 'ipv6_address'),
+        labels=pulumi.get(__ret__, 'labels'),
+        manager_id=pulumi.get(__ret__, 'manager_id'),
+        manager_type=pulumi.get(__ret__, 'manager_type'),
+        name=pulumi.get(__ret__, 'name'),
+        public_ip_address=pulumi.get(__ret__, 'public_ip_address'),
+        reverse_dns=pulumi.get(__ret__, 'reverse_dns'),
+        ssh_key=pulumi.get(__ret__, 'ssh_key'),
+        state=pulumi.get(__ret__, 'state'),
+        template_id=pulumi.get(__ret__, 'template_id'),
+        type=pulumi.get(__ret__, 'type'),
+        user_data=pulumi.get(__ret__, 'user_data'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_compute_instance_list)
 def get_compute_instance_list_output(created_at: Optional[pulumi.Input[Optional[str]]] = None,
                                      deploy_target_id: Optional[pulumi.Input[Optional[str]]] = None,
                                      disk_size: Optional[pulumi.Input[Optional[int]]] = None,
                                      id: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_compute_ip_address.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_compute_ip_address.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,19 +114,19 @@
     __args__['ipAddress'] = ip_address
     __args__['tags'] = tags
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getComputeIPAddress:getComputeIPAddress', __args__, opts=opts, typ=GetComputeIPAddressResult).value
 
     return AwaitableGetComputeIPAddressResult(
-        description=__ret__.description,
-        id=__ret__.id,
-        ip_address=__ret__.ip_address,
-        tags=__ret__.tags,
-        zone=__ret__.zone)
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        ip_address=pulumi.get(__ret__, 'ip_address'),
+        tags=pulumi.get(__ret__, 'tags'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_compute_ip_address)
 def get_compute_ip_address_output(description: Optional[pulumi.Input[Optional[str]]] = None,
                                   id: Optional[pulumi.Input[Optional[str]]] = None,
                                   ip_address: Optional[pulumi.Input[Optional[str]]] = None,
                                   tags: Optional[pulumi.Input[Optional[Mapping[str, str]]]] = None,
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_compute_template.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_compute_template.py`

 * *Files 12% similar despite different names*

```diff
@@ -110,19 +110,19 @@
     __args__['id'] = id
     __args__['name'] = name
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getComputeTemplate:getComputeTemplate', __args__, opts=opts, typ=GetComputeTemplateResult).value
 
     return AwaitableGetComputeTemplateResult(
-        filter=__ret__.filter,
-        id=__ret__.id,
-        name=__ret__.name,
-        username=__ret__.username,
-        zone=__ret__.zone)
+        filter=pulumi.get(__ret__, 'filter'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        username=pulumi.get(__ret__, 'username'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_compute_template)
 def get_compute_template_output(filter: Optional[pulumi.Input[Optional[str]]] = None,
                                 id: Optional[pulumi.Input[Optional[str]]] = None,
                                 name: Optional[pulumi.Input[Optional[str]]] = None,
                                 zone: Optional[pulumi.Input[str]] = None,
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_database_uri.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_database_uri.py`

 * *Files 8% similar despite different names*

```diff
@@ -137,19 +137,19 @@
     __args__['name'] = name
     __args__['type'] = type
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getDatabaseURI:getDatabaseURI', __args__, opts=opts, typ=GetDatabaseURIResult).value
 
     return AwaitableGetDatabaseURIResult(
-        id=__ret__.id,
-        name=__ret__.name,
-        type=__ret__.type,
-        uri=__ret__.uri,
-        zone=__ret__.zone)
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        type=pulumi.get(__ret__, 'type'),
+        uri=pulumi.get(__ret__, 'uri'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_database_uri)
 def get_database_uri_output(name: Optional[pulumi.Input[str]] = None,
                             type: Optional[pulumi.Input[str]] = None,
                             zone: Optional[pulumi.Input[str]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatabaseURIResult]:
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_domain.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_domain.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,16 +65,16 @@
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getDomain:getDomain', __args__, opts=opts, typ=GetDomainResult).value
 
     return AwaitableGetDomainResult(
-        id=__ret__.id,
-        name=__ret__.name)
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'))
 
 
 @_utilities.lift_output_func(get_domain)
 def get_domain_output(name: Optional[pulumi.Input[str]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDomainResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_domain_record.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_domain_record.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,18 +94,18 @@
     __args__ = dict()
     __args__['domain'] = domain
     __args__['filter'] = filter
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getDomainRecord:getDomainRecord', __args__, opts=opts, typ=GetDomainRecordResult).value
 
     return AwaitableGetDomainRecordResult(
-        domain=__ret__.domain,
-        filter=__ret__.filter,
-        id=__ret__.id,
-        records=__ret__.records)
+        domain=pulumi.get(__ret__, 'domain'),
+        filter=pulumi.get(__ret__, 'filter'),
+        id=pulumi.get(__ret__, 'id'),
+        records=pulumi.get(__ret__, 'records'))
 
 
 @_utilities.lift_output_func(get_domain_record)
 def get_domain_record_output(domain: Optional[pulumi.Input[str]] = None,
                              filter: Optional[pulumi.Input[pulumi.InputType['GetDomainRecordFilterArgs']]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDomainRecordResult]:
     """
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_elastic_ip.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_elastic_ip.py`

 * *Files 9% similar despite different names*

```diff
@@ -159,23 +159,23 @@
     __args__['ipAddress'] = ip_address
     __args__['labels'] = labels
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getElasticIP:getElasticIP', __args__, opts=opts, typ=GetElasticIPResult).value
 
     return AwaitableGetElasticIPResult(
-        address_family=__ret__.address_family,
-        cidr=__ret__.cidr,
-        description=__ret__.description,
-        healthchecks=__ret__.healthchecks,
-        id=__ret__.id,
-        ip_address=__ret__.ip_address,
-        labels=__ret__.labels,
-        reverse_dns=__ret__.reverse_dns,
-        zone=__ret__.zone)
+        address_family=pulumi.get(__ret__, 'address_family'),
+        cidr=pulumi.get(__ret__, 'cidr'),
+        description=pulumi.get(__ret__, 'description'),
+        healthchecks=pulumi.get(__ret__, 'healthchecks'),
+        id=pulumi.get(__ret__, 'id'),
+        ip_address=pulumi.get(__ret__, 'ip_address'),
+        labels=pulumi.get(__ret__, 'labels'),
+        reverse_dns=pulumi.get(__ret__, 'reverse_dns'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_elastic_ip)
 def get_elastic_ip_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                           ip_address: Optional[pulumi.Input[Optional[str]]] = None,
                           labels: Optional[pulumi.Input[Optional[Mapping[str, str]]]] = None,
                           zone: Optional[pulumi.Input[str]] = None,
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_instance_pool.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_instance_pool.py`

 * *Files 12% similar despite different names*

```diff
@@ -291,34 +291,34 @@
     __args__['labels'] = labels
     __args__['name'] = name
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getInstancePool:getInstancePool', __args__, opts=opts, typ=GetInstancePoolResult).value
 
     return AwaitableGetInstancePoolResult(
-        affinity_group_ids=__ret__.affinity_group_ids,
-        deploy_target_id=__ret__.deploy_target_id,
-        description=__ret__.description,
-        disk_size=__ret__.disk_size,
-        elastic_ip_ids=__ret__.elastic_ip_ids,
-        id=__ret__.id,
-        instance_prefix=__ret__.instance_prefix,
-        instance_type=__ret__.instance_type,
-        instances=__ret__.instances,
-        ipv6=__ret__.ipv6,
-        key_pair=__ret__.key_pair,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        network_ids=__ret__.network_ids,
-        security_group_ids=__ret__.security_group_ids,
-        size=__ret__.size,
-        state=__ret__.state,
-        template_id=__ret__.template_id,
-        user_data=__ret__.user_data,
-        zone=__ret__.zone)
+        affinity_group_ids=pulumi.get(__ret__, 'affinity_group_ids'),
+        deploy_target_id=pulumi.get(__ret__, 'deploy_target_id'),
+        description=pulumi.get(__ret__, 'description'),
+        disk_size=pulumi.get(__ret__, 'disk_size'),
+        elastic_ip_ids=pulumi.get(__ret__, 'elastic_ip_ids'),
+        id=pulumi.get(__ret__, 'id'),
+        instance_prefix=pulumi.get(__ret__, 'instance_prefix'),
+        instance_type=pulumi.get(__ret__, 'instance_type'),
+        instances=pulumi.get(__ret__, 'instances'),
+        ipv6=pulumi.get(__ret__, 'ipv6'),
+        key_pair=pulumi.get(__ret__, 'key_pair'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        network_ids=pulumi.get(__ret__, 'network_ids'),
+        security_group_ids=pulumi.get(__ret__, 'security_group_ids'),
+        size=pulumi.get(__ret__, 'size'),
+        state=pulumi.get(__ret__, 'state'),
+        template_id=pulumi.get(__ret__, 'template_id'),
+        user_data=pulumi.get(__ret__, 'user_data'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_instance_pool)
 def get_instance_pool_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                              labels: Optional[pulumi.Input[Optional[Mapping[str, str]]]] = None,
                              name: Optional[pulumi.Input[Optional[str]]] = None,
                              zone: Optional[pulumi.Input[str]] = None,
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_instance_pool_list.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_instance_pool_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -78,17 +78,17 @@
     """
     __args__ = dict()
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getInstancePoolList:getInstancePoolList', __args__, opts=opts, typ=GetInstancePoolListResult).value
 
     return AwaitableGetInstancePoolListResult(
-        id=__ret__.id,
-        pools=__ret__.pools,
-        zone=__ret__.zone)
+        id=pulumi.get(__ret__, 'id'),
+        pools=pulumi.get(__ret__, 'pools'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_instance_pool_list)
 def get_instance_pool_list_output(zone: Optional[pulumi.Input[str]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInstancePoolListResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_network.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_network.py`

 * *Files 12% similar despite different names*

```diff
@@ -132,21 +132,21 @@
     __args__['id'] = id
     __args__['name'] = name
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getNetwork:getNetwork', __args__, opts=opts, typ=GetNetworkResult).value
 
     return AwaitableGetNetworkResult(
-        description=__ret__.description,
-        end_ip=__ret__.end_ip,
-        id=__ret__.id,
-        name=__ret__.name,
-        netmask=__ret__.netmask,
-        start_ip=__ret__.start_ip,
-        zone=__ret__.zone)
+        description=pulumi.get(__ret__, 'description'),
+        end_ip=pulumi.get(__ret__, 'end_ip'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        netmask=pulumi.get(__ret__, 'netmask'),
+        start_ip=pulumi.get(__ret__, 'start_ip'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_network)
 def get_network_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                        name: Optional[pulumi.Input[Optional[str]]] = None,
                        zone: Optional[pulumi.Input[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNetworkResult]:
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_nlb.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_nlb.py`

 * *Files 19% similar despite different names*

```diff
@@ -131,21 +131,21 @@
     __args__['id'] = id
     __args__['name'] = name
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getNLB:getNLB', __args__, opts=opts, typ=GetNLBResult).value
 
     return AwaitableGetNLBResult(
-        created_at=__ret__.created_at,
-        description=__ret__.description,
-        id=__ret__.id,
-        ip_address=__ret__.ip_address,
-        name=__ret__.name,
-        state=__ret__.state,
-        zone=__ret__.zone)
+        created_at=pulumi.get(__ret__, 'created_at'),
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        ip_address=pulumi.get(__ret__, 'ip_address'),
+        name=pulumi.get(__ret__, 'name'),
+        state=pulumi.get(__ret__, 'state'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_nlb)
 def get_nlb_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                    name: Optional[pulumi.Input[Optional[str]]] = None,
                    zone: Optional[pulumi.Input[str]] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNLBResult]:
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_private_network.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_private_network.py`

 * *Files 7% similar despite different names*

```diff
@@ -134,21 +134,21 @@
     __args__['id'] = id
     __args__['name'] = name
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getPrivateNetwork:getPrivateNetwork', __args__, opts=opts, typ=GetPrivateNetworkResult).value
 
     return AwaitableGetPrivateNetworkResult(
-        description=__ret__.description,
-        end_ip=__ret__.end_ip,
-        id=__ret__.id,
-        name=__ret__.name,
-        netmask=__ret__.netmask,
-        start_ip=__ret__.start_ip,
-        zone=__ret__.zone)
+        description=pulumi.get(__ret__, 'description'),
+        end_ip=pulumi.get(__ret__, 'end_ip'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        netmask=pulumi.get(__ret__, 'netmask'),
+        start_ip=pulumi.get(__ret__, 'start_ip'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_private_network)
 def get_private_network_output(description: Optional[pulumi.Input[Optional[str]]] = None,
                                id: Optional[pulumi.Input[Optional[str]]] = None,
                                name: Optional[pulumi.Input[Optional[str]]] = None,
                                zone: Optional[pulumi.Input[str]] = None,
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_security_group.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_security_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,17 +80,17 @@
     __args__ = dict()
     __args__['id'] = id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getSecurityGroup:getSecurityGroup', __args__, opts=opts, typ=GetSecurityGroupResult).value
 
     return AwaitableGetSecurityGroupResult(
-        external_sources=__ret__.external_sources,
-        id=__ret__.id,
-        name=__ret__.name)
+        external_sources=pulumi.get(__ret__, 'external_sources'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'))
 
 
 @_utilities.lift_output_func(get_security_group)
 def get_security_group_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                               name: Optional[pulumi.Input[Optional[str]]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSecurityGroupResult]:
     """
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_sks_cluster.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_sks_cluster.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,18 +22,14 @@
 class GetSKSClusterResult:
     """
     A collection of values returned by getSKSCluster.
     """
     def __init__(__self__, addons=None, aggregation_ca=None, auto_upgrade=None, cni=None, control_plane_ca=None, created_at=None, description=None, endpoint=None, exoscale_ccm=None, id=None, kubelet_ca=None, labels=None, metrics_server=None, name=None, nodepools=None, oidc=None, service_level=None, state=None, version=None, zone=None):
         if addons and not isinstance(addons, list):
             raise TypeError("Expected argument 'addons' to be a list")
-        if addons is not None:
-            warnings.warn("""This attribute has been replaced by `exoscale_ccm`/`metrics_server` attributes, it will be removed in a future release.""", DeprecationWarning)
-            pulumi.log.warn("""addons is deprecated: This attribute has been replaced by `exoscale_ccm`/`metrics_server` attributes, it will be removed in a future release.""")
-
         pulumi.set(__self__, "addons", addons)
         if aggregation_ca and not isinstance(aggregation_ca, str):
             raise TypeError("Expected argument 'aggregation_ca' to be a str")
         pulumi.set(__self__, "aggregation_ca", aggregation_ca)
         if auto_upgrade and not isinstance(auto_upgrade, bool):
             raise TypeError("Expected argument 'auto_upgrade' to be a bool")
         pulumi.set(__self__, "auto_upgrade", auto_upgrade)
@@ -88,14 +84,17 @@
         if zone and not isinstance(zone, str):
             raise TypeError("Expected argument 'zone' to be a str")
         pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter
     def addons(self) -> Sequence[str]:
+        warnings.warn("""This attribute has been replaced by `exoscale_ccm`/`metrics_server` attributes, it will be removed in a future release.""", DeprecationWarning)
+        pulumi.log.warn("""addons is deprecated: This attribute has been replaced by `exoscale_ccm`/`metrics_server` attributes, it will be removed in a future release.""")
+
         return pulumi.get(self, "addons")
 
     @property
     @pulumi.getter(name="aggregationCa")
     def aggregation_ca(self) -> str:
         """
         The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g. `metrics-server`).
@@ -332,34 +331,34 @@
     __args__['state'] = state
     __args__['version'] = version
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getSKSCluster:getSKSCluster', __args__, opts=opts, typ=GetSKSClusterResult).value
 
     return AwaitableGetSKSClusterResult(
-        addons=__ret__.addons,
-        aggregation_ca=__ret__.aggregation_ca,
-        auto_upgrade=__ret__.auto_upgrade,
-        cni=__ret__.cni,
-        control_plane_ca=__ret__.control_plane_ca,
-        created_at=__ret__.created_at,
-        description=__ret__.description,
-        endpoint=__ret__.endpoint,
-        exoscale_ccm=__ret__.exoscale_ccm,
-        id=__ret__.id,
-        kubelet_ca=__ret__.kubelet_ca,
-        labels=__ret__.labels,
-        metrics_server=__ret__.metrics_server,
-        name=__ret__.name,
-        nodepools=__ret__.nodepools,
-        oidc=__ret__.oidc,
-        service_level=__ret__.service_level,
-        state=__ret__.state,
-        version=__ret__.version,
-        zone=__ret__.zone)
+        addons=pulumi.get(__ret__, 'addons'),
+        aggregation_ca=pulumi.get(__ret__, 'aggregation_ca'),
+        auto_upgrade=pulumi.get(__ret__, 'auto_upgrade'),
+        cni=pulumi.get(__ret__, 'cni'),
+        control_plane_ca=pulumi.get(__ret__, 'control_plane_ca'),
+        created_at=pulumi.get(__ret__, 'created_at'),
+        description=pulumi.get(__ret__, 'description'),
+        endpoint=pulumi.get(__ret__, 'endpoint'),
+        exoscale_ccm=pulumi.get(__ret__, 'exoscale_ccm'),
+        id=pulumi.get(__ret__, 'id'),
+        kubelet_ca=pulumi.get(__ret__, 'kubelet_ca'),
+        labels=pulumi.get(__ret__, 'labels'),
+        metrics_server=pulumi.get(__ret__, 'metrics_server'),
+        name=pulumi.get(__ret__, 'name'),
+        nodepools=pulumi.get(__ret__, 'nodepools'),
+        oidc=pulumi.get(__ret__, 'oidc'),
+        service_level=pulumi.get(__ret__, 'service_level'),
+        state=pulumi.get(__ret__, 'state'),
+        version=pulumi.get(__ret__, 'version'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_sks_cluster)
 def get_sks_cluster_output(addons: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                            aggregation_ca: Optional[pulumi.Input[Optional[str]]] = None,
                            auto_upgrade: Optional[pulumi.Input[Optional[bool]]] = None,
                            cni: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_sks_cluster_list.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_sks_cluster_list.py`

 * *Files 9% similar despite different names*

```diff
@@ -303,32 +303,32 @@
     __args__['state'] = state
     __args__['version'] = version
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getSKSClusterList:getSKSClusterList', __args__, opts=opts, typ=GetSKSClusterListResult).value
 
     return AwaitableGetSKSClusterListResult(
-        aggregation_ca=__ret__.aggregation_ca,
-        auto_upgrade=__ret__.auto_upgrade,
-        clusters=__ret__.clusters,
-        cni=__ret__.cni,
-        control_plane_ca=__ret__.control_plane_ca,
-        created_at=__ret__.created_at,
-        description=__ret__.description,
-        endpoint=__ret__.endpoint,
-        exoscale_ccm=__ret__.exoscale_ccm,
-        id=__ret__.id,
-        kubelet_ca=__ret__.kubelet_ca,
-        labels=__ret__.labels,
-        metrics_server=__ret__.metrics_server,
-        name=__ret__.name,
-        service_level=__ret__.service_level,
-        state=__ret__.state,
-        version=__ret__.version,
-        zone=__ret__.zone)
+        aggregation_ca=pulumi.get(__ret__, 'aggregation_ca'),
+        auto_upgrade=pulumi.get(__ret__, 'auto_upgrade'),
+        clusters=pulumi.get(__ret__, 'clusters'),
+        cni=pulumi.get(__ret__, 'cni'),
+        control_plane_ca=pulumi.get(__ret__, 'control_plane_ca'),
+        created_at=pulumi.get(__ret__, 'created_at'),
+        description=pulumi.get(__ret__, 'description'),
+        endpoint=pulumi.get(__ret__, 'endpoint'),
+        exoscale_ccm=pulumi.get(__ret__, 'exoscale_ccm'),
+        id=pulumi.get(__ret__, 'id'),
+        kubelet_ca=pulumi.get(__ret__, 'kubelet_ca'),
+        labels=pulumi.get(__ret__, 'labels'),
+        metrics_server=pulumi.get(__ret__, 'metrics_server'),
+        name=pulumi.get(__ret__, 'name'),
+        service_level=pulumi.get(__ret__, 'service_level'),
+        state=pulumi.get(__ret__, 'state'),
+        version=pulumi.get(__ret__, 'version'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_sks_cluster_list)
 def get_sks_cluster_list_output(aggregation_ca: Optional[pulumi.Input[Optional[str]]] = None,
                                 auto_upgrade: Optional[pulumi.Input[Optional[bool]]] = None,
                                 cni: Optional[pulumi.Input[Optional[str]]] = None,
                                 control_plane_ca: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_sks_nodepool.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_sks_nodepool.py`

 * *Files 4% similar despite different names*

```diff
@@ -322,34 +322,34 @@
     __args__['templateId'] = template_id
     __args__['version'] = version
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getSKSNodepool:getSKSNodepool', __args__, opts=opts, typ=GetSKSNodepoolResult).value
 
     return AwaitableGetSKSNodepoolResult(
-        anti_affinity_group_ids=__ret__.anti_affinity_group_ids,
-        cluster_id=__ret__.cluster_id,
-        created_at=__ret__.created_at,
-        deploy_target_id=__ret__.deploy_target_id,
-        description=__ret__.description,
-        disk_size=__ret__.disk_size,
-        id=__ret__.id,
-        instance_pool_id=__ret__.instance_pool_id,
-        instance_prefix=__ret__.instance_prefix,
-        instance_type=__ret__.instance_type,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        private_network_ids=__ret__.private_network_ids,
-        security_group_ids=__ret__.security_group_ids,
-        size=__ret__.size,
-        state=__ret__.state,
-        taints=__ret__.taints,
-        template_id=__ret__.template_id,
-        version=__ret__.version,
-        zone=__ret__.zone)
+        anti_affinity_group_ids=pulumi.get(__ret__, 'anti_affinity_group_ids'),
+        cluster_id=pulumi.get(__ret__, 'cluster_id'),
+        created_at=pulumi.get(__ret__, 'created_at'),
+        deploy_target_id=pulumi.get(__ret__, 'deploy_target_id'),
+        description=pulumi.get(__ret__, 'description'),
+        disk_size=pulumi.get(__ret__, 'disk_size'),
+        id=pulumi.get(__ret__, 'id'),
+        instance_pool_id=pulumi.get(__ret__, 'instance_pool_id'),
+        instance_prefix=pulumi.get(__ret__, 'instance_prefix'),
+        instance_type=pulumi.get(__ret__, 'instance_type'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        private_network_ids=pulumi.get(__ret__, 'private_network_ids'),
+        security_group_ids=pulumi.get(__ret__, 'security_group_ids'),
+        size=pulumi.get(__ret__, 'size'),
+        state=pulumi.get(__ret__, 'state'),
+        taints=pulumi.get(__ret__, 'taints'),
+        template_id=pulumi.get(__ret__, 'template_id'),
+        version=pulumi.get(__ret__, 'version'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_sks_nodepool)
 def get_sks_nodepool_output(anti_affinity_group_ids: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                             cluster_id: Optional[pulumi.Input[str]] = None,
                             created_at: Optional[pulumi.Input[Optional[str]]] = None,
                             deploy_target_id: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_sks_nodepool_list.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_sks_nodepool_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -303,32 +303,32 @@
     __args__['templateId'] = template_id
     __args__['version'] = version
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getSKSNodepoolList:getSKSNodepoolList', __args__, opts=opts, typ=GetSKSNodepoolListResult).value
 
     return AwaitableGetSKSNodepoolListResult(
-        cluster_id=__ret__.cluster_id,
-        created_at=__ret__.created_at,
-        deploy_target_id=__ret__.deploy_target_id,
-        description=__ret__.description,
-        disk_size=__ret__.disk_size,
-        id=__ret__.id,
-        instance_pool_id=__ret__.instance_pool_id,
-        instance_prefix=__ret__.instance_prefix,
-        instance_type=__ret__.instance_type,
-        labels=__ret__.labels,
-        name=__ret__.name,
-        nodepools=__ret__.nodepools,
-        size=__ret__.size,
-        state=__ret__.state,
-        taints=__ret__.taints,
-        template_id=__ret__.template_id,
-        version=__ret__.version,
-        zone=__ret__.zone)
+        cluster_id=pulumi.get(__ret__, 'cluster_id'),
+        created_at=pulumi.get(__ret__, 'created_at'),
+        deploy_target_id=pulumi.get(__ret__, 'deploy_target_id'),
+        description=pulumi.get(__ret__, 'description'),
+        disk_size=pulumi.get(__ret__, 'disk_size'),
+        id=pulumi.get(__ret__, 'id'),
+        instance_pool_id=pulumi.get(__ret__, 'instance_pool_id'),
+        instance_prefix=pulumi.get(__ret__, 'instance_prefix'),
+        instance_type=pulumi.get(__ret__, 'instance_type'),
+        labels=pulumi.get(__ret__, 'labels'),
+        name=pulumi.get(__ret__, 'name'),
+        nodepools=pulumi.get(__ret__, 'nodepools'),
+        size=pulumi.get(__ret__, 'size'),
+        state=pulumi.get(__ret__, 'state'),
+        taints=pulumi.get(__ret__, 'taints'),
+        template_id=pulumi.get(__ret__, 'template_id'),
+        version=pulumi.get(__ret__, 'version'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_sks_nodepool_list)
 def get_sks_nodepool_list_output(cluster_id: Optional[pulumi.Input[Optional[str]]] = None,
                                  created_at: Optional[pulumi.Input[Optional[str]]] = None,
                                  deploy_target_id: Optional[pulumi.Input[Optional[str]]] = None,
                                  description: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_template.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/get_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,19 +110,19 @@
     __args__['name'] = name
     __args__['visibility'] = visibility
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getTemplate:getTemplate', __args__, opts=opts, typ=GetTemplateResult).value
 
     return AwaitableGetTemplateResult(
-        default_user=__ret__.default_user,
-        id=__ret__.id,
-        name=__ret__.name,
-        visibility=__ret__.visibility,
-        zone=__ret__.zone)
+        default_user=pulumi.get(__ret__, 'default_user'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        visibility=pulumi.get(__ret__, 'visibility'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_template)
 def get_template_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                         name: Optional[pulumi.Input[Optional[str]]] = None,
                         visibility: Optional[pulumi.Input[Optional[str]]] = None,
                         zone: Optional[pulumi.Input[str]] = None,
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/iam_access_key.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/iam_access_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,73 +16,69 @@
     def __init__(__self__, *,
                  name: Optional[pulumi.Input[str]] = None,
                  operations: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  resources: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a IAMAccessKey resource.
-        :param pulumi.Input[str] name: The IAM access key name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] operations: A list of API operations to restrict the key to.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: A list of API
-               [resources](https://community.exoscale.com/documentation/iam/quick-start/#restricting-api-access-keys-to-resources) to
-               restrict the key to (`<domain>/<type>:<name>`).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to restrict the key to.
+        :param pulumi.Input[str] name: ❗ The IAM access key name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] operations: ❗ A list of API operations to restrict the key to.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: ❗ A list of API [resources](https://community.exoscale.com/documentation/iam/quick-start/#restricting-api-access-keys-to-resources) to restrict the key to (`<domain>/<type>:<name>`).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: ❗ A list of tags to restrict the key to.
         """
         if name is not None:
             pulumi.set(__self__, "name", name)
         if operations is not None:
             pulumi.set(__self__, "operations", operations)
         if resources is not None:
             pulumi.set(__self__, "resources", resources)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The IAM access key name.
+        ❗ The IAM access key name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def operations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of API operations to restrict the key to.
+        ❗ A list of API operations to restrict the key to.
         """
         return pulumi.get(self, "operations")
 
     @operations.setter
     def operations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "operations", value)
 
     @property
     @pulumi.getter
     def resources(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of API
-        [resources](https://community.exoscale.com/documentation/iam/quick-start/#restricting-api-access-keys-to-resources) to
-        restrict the key to (`<domain>/<type>:<name>`).
+        ❗ A list of API [resources](https://community.exoscale.com/documentation/iam/quick-start/#restricting-api-access-keys-to-resources) to restrict the key to (`<domain>/<type>:<name>`).
         """
         return pulumi.get(self, "resources")
 
     @resources.setter
     def resources(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "resources", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of tags to restrict the key to.
+        ❗ A list of tags to restrict the key to.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -96,21 +92,19 @@
                  resources: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  secret: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tags_operations: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering IAMAccessKey resources.
         :param pulumi.Input[str] key: The IAM access key (identifier).
-        :param pulumi.Input[str] name: The IAM access key name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] operations: A list of API operations to restrict the key to.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: A list of API
-               [resources](https://community.exoscale.com/documentation/iam/quick-start/#restricting-api-access-keys-to-resources) to
-               restrict the key to (`<domain>/<type>:<name>`).
+        :param pulumi.Input[str] name: ❗ The IAM access key name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] operations: ❗ A list of API operations to restrict the key to.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: ❗ A list of API [resources](https://community.exoscale.com/documentation/iam/quick-start/#restricting-api-access-keys-to-resources) to restrict the key to (`<domain>/<type>:<name>`).
         :param pulumi.Input[str] secret: The key secret.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to restrict the key to.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: ❗ A list of tags to restrict the key to.
         """
         if key is not None:
             pulumi.set(__self__, "key", key)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if operations is not None:
             pulumi.set(__self__, "operations", operations)
@@ -135,41 +129,39 @@
     def key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The IAM access key name.
+        ❗ The IAM access key name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def operations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of API operations to restrict the key to.
+        ❗ A list of API operations to restrict the key to.
         """
         return pulumi.get(self, "operations")
 
     @operations.setter
     def operations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "operations", value)
 
     @property
     @pulumi.getter
     def resources(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of API
-        [resources](https://community.exoscale.com/documentation/iam/quick-start/#restricting-api-access-keys-to-resources) to
-        restrict the key to (`<domain>/<type>:<name>`).
+        ❗ A list of API [resources](https://community.exoscale.com/documentation/iam/quick-start/#restricting-api-access-keys-to-resources) to restrict the key to (`<domain>/<type>:<name>`).
         """
         return pulumi.get(self, "resources")
 
     @resources.setter
     def resources(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "resources", value)
 
@@ -185,15 +177,15 @@
     def secret(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of tags to restrict the key to.
+        ❗ A list of tags to restrict the key to.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -217,20 +209,18 @@
                  resources: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Create a IAMAccessKey resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] name: The IAM access key name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] operations: A list of API operations to restrict the key to.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: A list of API
-               [resources](https://community.exoscale.com/documentation/iam/quick-start/#restricting-api-access-keys-to-resources) to
-               restrict the key to (`<domain>/<type>:<name>`).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to restrict the key to.
+        :param pulumi.Input[str] name: ❗ The IAM access key name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] operations: ❗ A list of API operations to restrict the key to.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: ❗ A list of API [resources](https://community.exoscale.com/documentation/iam/quick-start/#restricting-api-access-keys-to-resources) to restrict the key to (`<domain>/<type>:<name>`).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: ❗ A list of tags to restrict the key to.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[IAMAccessKeyArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -294,21 +284,19 @@
         Get an existing IAMAccessKey resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] key: The IAM access key (identifier).
-        :param pulumi.Input[str] name: The IAM access key name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] operations: A list of API operations to restrict the key to.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: A list of API
-               [resources](https://community.exoscale.com/documentation/iam/quick-start/#restricting-api-access-keys-to-resources) to
-               restrict the key to (`<domain>/<type>:<name>`).
+        :param pulumi.Input[str] name: ❗ The IAM access key name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] operations: ❗ A list of API operations to restrict the key to.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: ❗ A list of API [resources](https://community.exoscale.com/documentation/iam/quick-start/#restricting-api-access-keys-to-resources) to restrict the key to (`<domain>/<type>:<name>`).
         :param pulumi.Input[str] secret: The key secret.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of tags to restrict the key to.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: ❗ A list of tags to restrict the key to.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _IAMAccessKeyState.__new__(_IAMAccessKeyState)
 
         __props__.__dict__["key"] = key
         __props__.__dict__["name"] = name
@@ -327,33 +315,31 @@
         """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The IAM access key name.
+        ❗ The IAM access key name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def operations(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of API operations to restrict the key to.
+        ❗ A list of API operations to restrict the key to.
         """
         return pulumi.get(self, "operations")
 
     @property
     @pulumi.getter
     def resources(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of API
-        [resources](https://community.exoscale.com/documentation/iam/quick-start/#restricting-api-access-keys-to-resources) to
-        restrict the key to (`<domain>/<type>:<name>`).
+        ❗ A list of API [resources](https://community.exoscale.com/documentation/iam/quick-start/#restricting-api-access-keys-to-resources) to restrict the key to (`<domain>/<type>:<name>`).
         """
         return pulumi.get(self, "resources")
 
     @property
     @pulumi.getter
     def secret(self) -> pulumi.Output[str]:
         """
@@ -361,15 +347,15 @@
         """
         return pulumi.get(self, "secret")
 
     @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of tags to restrict the key to.
+        ❗ A list of tags to restrict the key to.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tagsOperations")
     def tags_operations(self) -> pulumi.Output[Sequence[str]]:
         return pulumi.get(self, "tags_operations")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/instance_pool.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/instance_pool.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,34 +36,32 @@
                  service_offering: Optional[pulumi.Input[str]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  user_data: Optional[pulumi.Input[str]] = None,
                  virtual_machines: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a InstancePool resource.
         :param pulumi.Input[int] size: The number of managed instances.
-        :param pulumi.Input[str] template_id: The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the managed instances.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs; may only be set at creation time).
+        :param pulumi.Input[str] template_id: The exoscale*compute*template (ID) to use when creating the managed instances.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of exoscale*anti*affinity_group (IDs; may only be set at creation time).
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[str] description: A free-form text describing the pool.
         :param pulumi.Input[int] disk_size: The managed instances disk size (GiB).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of exoscale*elastic*ip (IDs).
         :param pulumi.Input[str] instance_prefix: The string used to prefix managed instances name (default: `pool`).
-        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
-               CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         :param pulumi.Input[Sequence[pulumi.Input['InstancePoolInstanceArgs']]] instances: The list of managed instances. Structure is documented below.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on managed instances (boolean; default: `false`).
-        :param pulumi.Input[str] key_pair: The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the managed instances.
+        :param pulumi.Input[str] key_pair: The exoscale*ssh*key (name) to authorize in the managed instances.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The instance pool name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_ids: A list of [exoscale_private_network](./private_network.md) (IDs).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_groups.md) (IDs).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_ids: A list of exoscale*private*network (IDs).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of exoscale*security*group (IDs).
         :param pulumi.Input[str] service_offering: The managed instances type. Please use the `instance_type` argument instead.
-        :param pulumi.Input[str] user_data: [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances (no need to base64-encode
-               or gzip it as the provider will take care of it).
+        :param pulumi.Input[str] user_data: [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances (no need to base64-encode or gzip it as the provider will take care of it).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machines: The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
         """
         pulumi.set(__self__, "size", size)
         pulumi.set(__self__, "template_id", template_id)
         pulumi.set(__self__, "zone", zone)
         if affinity_group_ids is not None:
             pulumi.set(__self__, "affinity_group_ids", affinity_group_ids)
@@ -120,39 +118,39 @@
     def size(self, value: pulumi.Input[int]):
         pulumi.set(self, "size", value)
 
     @property
     @pulumi.getter(name="templateId")
     def template_id(self) -> pulumi.Input[str]:
         """
-        The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the managed instances.
+        The exoscale*compute*template (ID) to use when creating the managed instances.
         """
         return pulumi.get(self, "template_id")
 
     @template_id.setter
     def template_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "template_id", value)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
     @property
     @pulumi.getter(name="affinityGroupIds")
     def affinity_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs; may only be set at creation time).
+        A list of exoscale*anti*affinity_group (IDs; may only be set at creation time).
         """
         return pulumi.get(self, "affinity_group_ids")
 
     @affinity_group_ids.setter
     def affinity_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "affinity_group_ids", value)
 
@@ -192,15 +190,15 @@
     def disk_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "disk_size", value)
 
     @property
     @pulumi.getter(name="elasticIpIds")
     def elastic_ip_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs).
+        A list of exoscale*elastic*ip (IDs).
         """
         return pulumi.get(self, "elastic_ip_ids")
 
     @elastic_ip_ids.setter
     def elastic_ip_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "elastic_ip_ids", value)
 
@@ -216,16 +214,15 @@
     def instance_prefix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "instance_prefix", value)
 
     @property
     @pulumi.getter(name="instanceType")
     def instance_type(self) -> Optional[pulumi.Input[str]]:
         """
-        The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
-        CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         """
         return pulumi.get(self, "instance_type")
 
     @instance_type.setter
     def instance_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "instance_type", value)
 
@@ -253,15 +250,15 @@
     def ipv6(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ipv6", value)
 
     @property
     @pulumi.getter(name="keyPair")
     def key_pair(self) -> Optional[pulumi.Input[str]]:
         """
-        The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the managed instances.
+        The exoscale*ssh*key (name) to authorize in the managed instances.
         """
         return pulumi.get(self, "key_pair")
 
     @key_pair.setter
     def key_pair(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key_pair", value)
 
@@ -289,40 +286,43 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="networkIds")
     def network_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of [exoscale_private_network](./private_network.md) (IDs).
+        A list of exoscale*private*network (IDs).
         """
         return pulumi.get(self, "network_ids")
 
     @network_ids.setter
     def network_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "network_ids", value)
 
     @property
     @pulumi.getter(name="securityGroupIds")
     def security_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of [exoscale_security_group](./security_groups.md) (IDs).
+        A list of exoscale*security*group (IDs).
         """
         return pulumi.get(self, "security_group_ids")
 
     @security_group_ids.setter
     def security_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "security_group_ids", value)
 
     @property
     @pulumi.getter(name="serviceOffering")
     def service_offering(self) -> Optional[pulumi.Input[str]]:
         """
         The managed instances type. Please use the `instance_type` argument instead.
         """
+        warnings.warn("""This attribute has been replaced by \"instance_type\".""", DeprecationWarning)
+        pulumi.log.warn("""service_offering is deprecated: This attribute has been replaced by \"instance_type\".""")
+
         return pulumi.get(self, "service_offering")
 
     @service_offering.setter
     def service_offering(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_offering", value)
 
     @property
@@ -334,29 +334,31 @@
     def state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "state", value)
 
     @property
     @pulumi.getter(name="userData")
     def user_data(self) -> Optional[pulumi.Input[str]]:
         """
-        [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances (no need to base64-encode
-        or gzip it as the provider will take care of it).
+        [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances (no need to base64-encode or gzip it as the provider will take care of it).
         """
         return pulumi.get(self, "user_data")
 
     @user_data.setter
     def user_data(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_data", value)
 
     @property
     @pulumi.getter(name="virtualMachines")
     def virtual_machines(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
         """
+        warnings.warn("""Use the instances exported attribute instead.""", DeprecationWarning)
+        pulumi.log.warn("""virtual_machines is deprecated: Use the instances exported attribute instead.""")
+
         return pulumi.get(self, "virtual_machines")
 
     @virtual_machines.setter
     def virtual_machines(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "virtual_machines", value)
 
 
@@ -382,36 +384,34 @@
                  state: Optional[pulumi.Input[str]] = None,
                  template_id: Optional[pulumi.Input[str]] = None,
                  user_data: Optional[pulumi.Input[str]] = None,
                  virtual_machines: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering InstancePool resources.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs; may only be set at creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of exoscale*anti*affinity_group (IDs; may only be set at creation time).
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[str] description: A free-form text describing the pool.
         :param pulumi.Input[int] disk_size: The managed instances disk size (GiB).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of exoscale*elastic*ip (IDs).
         :param pulumi.Input[str] instance_prefix: The string used to prefix managed instances name (default: `pool`).
-        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
-               CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         :param pulumi.Input[Sequence[pulumi.Input['InstancePoolInstanceArgs']]] instances: The list of managed instances. Structure is documented below.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on managed instances (boolean; default: `false`).
-        :param pulumi.Input[str] key_pair: The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the managed instances.
+        :param pulumi.Input[str] key_pair: The exoscale*ssh*key (name) to authorize in the managed instances.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The instance pool name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_ids: A list of [exoscale_private_network](./private_network.md) (IDs).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_groups.md) (IDs).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_ids: A list of exoscale*private*network (IDs).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of exoscale*security*group (IDs).
         :param pulumi.Input[str] service_offering: The managed instances type. Please use the `instance_type` argument instead.
         :param pulumi.Input[int] size: The number of managed instances.
-        :param pulumi.Input[str] template_id: The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the managed instances.
-        :param pulumi.Input[str] user_data: [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances (no need to base64-encode
-               or gzip it as the provider will take care of it).
+        :param pulumi.Input[str] template_id: The exoscale*compute*template (ID) to use when creating the managed instances.
+        :param pulumi.Input[str] user_data: [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances (no need to base64-encode or gzip it as the provider will take care of it).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machines: The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if affinity_group_ids is not None:
             pulumi.set(__self__, "affinity_group_ids", affinity_group_ids)
         if deploy_target_id is not None:
             pulumi.set(__self__, "deploy_target_id", deploy_target_id)
         if description is not None:
             pulumi.set(__self__, "description", description)
@@ -458,15 +458,15 @@
         if zone is not None:
             pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter(name="affinityGroupIds")
     def affinity_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs; may only be set at creation time).
+        A list of exoscale*anti*affinity_group (IDs; may only be set at creation time).
         """
         return pulumi.get(self, "affinity_group_ids")
 
     @affinity_group_ids.setter
     def affinity_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "affinity_group_ids", value)
 
@@ -506,15 +506,15 @@
     def disk_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "disk_size", value)
 
     @property
     @pulumi.getter(name="elasticIpIds")
     def elastic_ip_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs).
+        A list of exoscale*elastic*ip (IDs).
         """
         return pulumi.get(self, "elastic_ip_ids")
 
     @elastic_ip_ids.setter
     def elastic_ip_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "elastic_ip_ids", value)
 
@@ -530,16 +530,15 @@
     def instance_prefix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "instance_prefix", value)
 
     @property
     @pulumi.getter(name="instanceType")
     def instance_type(self) -> Optional[pulumi.Input[str]]:
         """
-        The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
-        CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         """
         return pulumi.get(self, "instance_type")
 
     @instance_type.setter
     def instance_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "instance_type", value)
 
@@ -567,15 +566,15 @@
     def ipv6(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ipv6", value)
 
     @property
     @pulumi.getter(name="keyPair")
     def key_pair(self) -> Optional[pulumi.Input[str]]:
         """
-        The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the managed instances.
+        The exoscale*ssh*key (name) to authorize in the managed instances.
         """
         return pulumi.get(self, "key_pair")
 
     @key_pair.setter
     def key_pair(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key_pair", value)
 
@@ -603,40 +602,43 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="networkIds")
     def network_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of [exoscale_private_network](./private_network.md) (IDs).
+        A list of exoscale*private*network (IDs).
         """
         return pulumi.get(self, "network_ids")
 
     @network_ids.setter
     def network_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "network_ids", value)
 
     @property
     @pulumi.getter(name="securityGroupIds")
     def security_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of [exoscale_security_group](./security_groups.md) (IDs).
+        A list of exoscale*security*group (IDs).
         """
         return pulumi.get(self, "security_group_ids")
 
     @security_group_ids.setter
     def security_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "security_group_ids", value)
 
     @property
     @pulumi.getter(name="serviceOffering")
     def service_offering(self) -> Optional[pulumi.Input[str]]:
         """
         The managed instances type. Please use the `instance_type` argument instead.
         """
+        warnings.warn("""This attribute has been replaced by \"instance_type\".""", DeprecationWarning)
+        pulumi.log.warn("""service_offering is deprecated: This attribute has been replaced by \"instance_type\".""")
+
         return pulumi.get(self, "service_offering")
 
     @service_offering.setter
     def service_offering(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_offering", value)
 
     @property
@@ -660,52 +662,54 @@
     def state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "state", value)
 
     @property
     @pulumi.getter(name="templateId")
     def template_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the managed instances.
+        The exoscale*compute*template (ID) to use when creating the managed instances.
         """
         return pulumi.get(self, "template_id")
 
     @template_id.setter
     def template_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "template_id", value)
 
     @property
     @pulumi.getter(name="userData")
     def user_data(self) -> Optional[pulumi.Input[str]]:
         """
-        [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances (no need to base64-encode
-        or gzip it as the provider will take care of it).
+        [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances (no need to base64-encode or gzip it as the provider will take care of it).
         """
         return pulumi.get(self, "user_data")
 
     @user_data.setter
     def user_data(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_data", value)
 
     @property
     @pulumi.getter(name="virtualMachines")
     def virtual_machines(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
         """
+        warnings.warn("""Use the instances exported attribute instead.""", DeprecationWarning)
+        pulumi.log.warn("""virtual_machines is deprecated: Use the instances exported attribute instead.""")
+
         return pulumi.get(self, "virtual_machines")
 
     @virtual_machines.setter
     def virtual_machines(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "virtual_machines", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -748,36 +752,34 @@
 
          exoscale_instance_pool.my_instance_pool \\
 
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs; may only be set at creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of exoscale*anti*affinity_group (IDs; may only be set at creation time).
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[str] description: A free-form text describing the pool.
         :param pulumi.Input[int] disk_size: The managed instances disk size (GiB).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of exoscale*elastic*ip (IDs).
         :param pulumi.Input[str] instance_prefix: The string used to prefix managed instances name (default: `pool`).
-        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
-               CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstancePoolInstanceArgs']]]] instances: The list of managed instances. Structure is documented below.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on managed instances (boolean; default: `false`).
-        :param pulumi.Input[str] key_pair: The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the managed instances.
+        :param pulumi.Input[str] key_pair: The exoscale*ssh*key (name) to authorize in the managed instances.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The instance pool name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_ids: A list of [exoscale_private_network](./private_network.md) (IDs).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_groups.md) (IDs).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_ids: A list of exoscale*private*network (IDs).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of exoscale*security*group (IDs).
         :param pulumi.Input[str] service_offering: The managed instances type. Please use the `instance_type` argument instead.
         :param pulumi.Input[int] size: The number of managed instances.
-        :param pulumi.Input[str] template_id: The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the managed instances.
-        :param pulumi.Input[str] user_data: [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances (no need to base64-encode
-               or gzip it as the provider will take care of it).
+        :param pulumi.Input[str] template_id: The exoscale*compute*template (ID) to use when creating the managed instances.
+        :param pulumi.Input[str] user_data: [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances (no need to base64-encode or gzip it as the provider will take care of it).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machines: The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: InstancePoolArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -906,36 +908,34 @@
         """
         Get an existing InstancePool resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs; may only be set at creation time).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of exoscale*anti*affinity_group (IDs; may only be set at creation time).
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[str] description: A free-form text describing the pool.
         :param pulumi.Input[int] disk_size: The managed instances disk size (GiB).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of exoscale*elastic*ip (IDs).
         :param pulumi.Input[str] instance_prefix: The string used to prefix managed instances name (default: `pool`).
-        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
-               CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstancePoolInstanceArgs']]]] instances: The list of managed instances. Structure is documented below.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on managed instances (boolean; default: `false`).
-        :param pulumi.Input[str] key_pair: The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the managed instances.
+        :param pulumi.Input[str] key_pair: The exoscale*ssh*key (name) to authorize in the managed instances.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The instance pool name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_ids: A list of [exoscale_private_network](./private_network.md) (IDs).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_groups.md) (IDs).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] network_ids: A list of exoscale*private*network (IDs).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of exoscale*security*group (IDs).
         :param pulumi.Input[str] service_offering: The managed instances type. Please use the `instance_type` argument instead.
         :param pulumi.Input[int] size: The number of managed instances.
-        :param pulumi.Input[str] template_id: The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the managed instances.
-        :param pulumi.Input[str] user_data: [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances (no need to base64-encode
-               or gzip it as the provider will take care of it).
+        :param pulumi.Input[str] template_id: The exoscale*compute*template (ID) to use when creating the managed instances.
+        :param pulumi.Input[str] user_data: [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances (no need to base64-encode or gzip it as the provider will take care of it).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machines: The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _InstancePoolState.__new__(_InstancePoolState)
 
         __props__.__dict__["affinity_group_ids"] = affinity_group_ids
         __props__.__dict__["deploy_target_id"] = deploy_target_id
@@ -960,15 +960,15 @@
         __props__.__dict__["zone"] = zone
         return InstancePool(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="affinityGroupIds")
     def affinity_group_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs; may only be set at creation time).
+        A list of exoscale*anti*affinity_group (IDs; may only be set at creation time).
         """
         return pulumi.get(self, "affinity_group_ids")
 
     @property
     @pulumi.getter(name="deployTargetId")
     def deploy_target_id(self) -> pulumi.Output[Optional[str]]:
         """
@@ -992,15 +992,15 @@
         """
         return pulumi.get(self, "disk_size")
 
     @property
     @pulumi.getter(name="elasticIpIds")
     def elastic_ip_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs).
+        A list of exoscale*elastic*ip (IDs).
         """
         return pulumi.get(self, "elastic_ip_ids")
 
     @property
     @pulumi.getter(name="instancePrefix")
     def instance_prefix(self) -> pulumi.Output[Optional[str]]:
         """
@@ -1008,16 +1008,15 @@
         """
         return pulumi.get(self, "instance_prefix")
 
     @property
     @pulumi.getter(name="instanceType")
     def instance_type(self) -> pulumi.Output[str]:
         """
-        The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
-        CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         """
         return pulumi.get(self, "instance_type")
 
     @property
     @pulumi.getter
     def instances(self) -> pulumi.Output[Sequence['outputs.InstancePoolInstance']]:
         """
@@ -1033,15 +1032,15 @@
         """
         return pulumi.get(self, "ipv6")
 
     @property
     @pulumi.getter(name="keyPair")
     def key_pair(self) -> pulumi.Output[Optional[str]]:
         """
-        The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the managed instances.
+        The exoscale*ssh*key (name) to authorize in the managed instances.
         """
         return pulumi.get(self, "key_pair")
 
     @property
     @pulumi.getter
     def labels(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
@@ -1057,32 +1056,35 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="networkIds")
     def network_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of [exoscale_private_network](./private_network.md) (IDs).
+        A list of exoscale*private*network (IDs).
         """
         return pulumi.get(self, "network_ids")
 
     @property
     @pulumi.getter(name="securityGroupIds")
     def security_group_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of [exoscale_security_group](./security_groups.md) (IDs).
+        A list of exoscale*security*group (IDs).
         """
         return pulumi.get(self, "security_group_ids")
 
     @property
     @pulumi.getter(name="serviceOffering")
     def service_offering(self) -> pulumi.Output[str]:
         """
         The managed instances type. Please use the `instance_type` argument instead.
         """
+        warnings.warn("""This attribute has been replaced by \"instance_type\".""", DeprecationWarning)
+        pulumi.log.warn("""service_offering is deprecated: This attribute has been replaced by \"instance_type\".""")
+
         return pulumi.get(self, "service_offering")
 
     @property
     @pulumi.getter
     def size(self) -> pulumi.Output[int]:
         """
         The number of managed instances.
@@ -1094,36 +1096,38 @@
     def state(self) -> pulumi.Output[str]:
         return pulumi.get(self, "state")
 
     @property
     @pulumi.getter(name="templateId")
     def template_id(self) -> pulumi.Output[str]:
         """
-        The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the managed instances.
+        The exoscale*compute*template (ID) to use when creating the managed instances.
         """
         return pulumi.get(self, "template_id")
 
     @property
     @pulumi.getter(name="userData")
     def user_data(self) -> pulumi.Output[Optional[str]]:
         """
-        [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances (no need to base64-encode
-        or gzip it as the provider will take care of it).
+        [cloud-init](http://cloudinit.readthedocs.io/) configuration to apply to the managed instances (no need to base64-encode or gzip it as the provider will take care of it).
         """
         return pulumi.get(self, "user_data")
 
     @property
     @pulumi.getter(name="virtualMachines")
     def virtual_machines(self) -> pulumi.Output[Sequence[str]]:
         """
         The list of managed instances (IDs). Please use the `instances.*.id` attribute instead.
         """
+        warnings.warn("""Use the instances exported attribute instead.""", DeprecationWarning)
+        pulumi.log.warn("""virtual_machines is deprecated: Use the instances exported attribute instead.""")
+
         return pulumi.get(self, "virtual_machines")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/ip_address.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/ip_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,27 +25,25 @@
                  healthcheck_timeout: Optional[pulumi.Input[int]] = None,
                  healthcheck_tls_skip_verify: Optional[pulumi.Input[bool]] = None,
                  healthcheck_tls_sni: Optional[pulumi.Input[str]] = None,
                  reverse_dns: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a IPAddress resource.
-        :param pulumi.Input[str] zone: The Exoscale Zone name
+        :param pulumi.Input[str] zone: ❗ The Exoscale Zone name
         :param pulumi.Input[str] description: A free-form text describing the Elastic IP (EIP).
         :param pulumi.Input[int] healthcheck_interval: The healthcheck probing interval (seconds; must be between `5` and `300`).
-        :param pulumi.Input[str] healthcheck_mode: The healthcheck probing mode (must be `tcp`, `http` or `https`).
+        :param pulumi.Input[str] healthcheck_mode: ❗ The healthcheck probing mode (must be `tcp`, `http` or `https`).
         :param pulumi.Input[str] healthcheck_path: The healthcheck probe HTTP request path (must be specified in `http`/`https` modes).
         :param pulumi.Input[int] healthcheck_port: The healthcheck service port to probe (must be between `1` and `65535`).
         :param pulumi.Input[int] healthcheck_strikes_fail: The number of unsuccessful healthcheck probes before considering the target unhealthy (must be between `1` and `20`).
         :param pulumi.Input[int] healthcheck_strikes_ok: The number of successful healthcheck probes before considering the target healthy (must be between `1` and `20`).
         :param pulumi.Input[int] healthcheck_timeout: The time in seconds before considering a healthcheck probing failed (must be between `2` and `60`).
-        :param pulumi.Input[bool] healthcheck_tls_skip_verify: Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed
-               to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
-        :param pulumi.Input[str] healthcheck_tls_sni: The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty
-               value, it cannot be reset to its default empty value later on (requires a resource re-creation).
+        :param pulumi.Input[bool] healthcheck_tls_skip_verify: Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
+        :param pulumi.Input[str] healthcheck_tls_sni: The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty value, it cannot be reset to its default empty value later on (requires a resource re-creation).
         :param pulumi.Input[str] reverse_dns: The EIP reverse DNS record (must end with a `.`; e.g: `my-eip.example.net.`).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
         """
         pulumi.set(__self__, "zone", zone)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if healthcheck_interval is not None:
@@ -71,15 +69,15 @@
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
-        The Exoscale Zone name
+        ❗ The Exoscale Zone name
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
@@ -107,15 +105,15 @@
     def healthcheck_interval(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "healthcheck_interval", value)
 
     @property
     @pulumi.getter(name="healthcheckMode")
     def healthcheck_mode(self) -> Optional[pulumi.Input[str]]:
         """
-        The healthcheck probing mode (must be `tcp`, `http` or `https`).
+        ❗ The healthcheck probing mode (must be `tcp`, `http` or `https`).
         """
         return pulumi.get(self, "healthcheck_mode")
 
     @healthcheck_mode.setter
     def healthcheck_mode(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "healthcheck_mode", value)
 
@@ -179,29 +177,27 @@
     def healthcheck_timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "healthcheck_timeout", value)
 
     @property
     @pulumi.getter(name="healthcheckTlsSkipVerify")
     def healthcheck_tls_skip_verify(self) -> Optional[pulumi.Input[bool]]:
         """
-        Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed
-        to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
+        Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
         """
         return pulumi.get(self, "healthcheck_tls_skip_verify")
 
     @healthcheck_tls_skip_verify.setter
     def healthcheck_tls_skip_verify(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "healthcheck_tls_skip_verify", value)
 
     @property
     @pulumi.getter(name="healthcheckTlsSni")
     def healthcheck_tls_sni(self) -> Optional[pulumi.Input[str]]:
         """
-        The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty
-        value, it cannot be reset to its default empty value later on (requires a resource re-creation).
+        The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty value, it cannot be reset to its default empty value later on (requires a resource re-creation).
         """
         return pulumi.get(self, "healthcheck_tls_sni")
 
     @healthcheck_tls_sni.setter
     def healthcheck_tls_sni(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "healthcheck_tls_sni", value)
 
@@ -247,28 +243,26 @@
                  reverse_dns: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering IPAddress resources.
         :param pulumi.Input[str] description: A free-form text describing the Elastic IP (EIP).
         :param pulumi.Input[int] healthcheck_interval: The healthcheck probing interval (seconds; must be between `5` and `300`).
-        :param pulumi.Input[str] healthcheck_mode: The healthcheck probing mode (must be `tcp`, `http` or `https`).
+        :param pulumi.Input[str] healthcheck_mode: ❗ The healthcheck probing mode (must be `tcp`, `http` or `https`).
         :param pulumi.Input[str] healthcheck_path: The healthcheck probe HTTP request path (must be specified in `http`/`https` modes).
         :param pulumi.Input[int] healthcheck_port: The healthcheck service port to probe (must be between `1` and `65535`).
         :param pulumi.Input[int] healthcheck_strikes_fail: The number of unsuccessful healthcheck probes before considering the target unhealthy (must be between `1` and `20`).
         :param pulumi.Input[int] healthcheck_strikes_ok: The number of successful healthcheck probes before considering the target healthy (must be between `1` and `20`).
         :param pulumi.Input[int] healthcheck_timeout: The time in seconds before considering a healthcheck probing failed (must be between `2` and `60`).
-        :param pulumi.Input[bool] healthcheck_tls_skip_verify: Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed
-               to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
-        :param pulumi.Input[str] healthcheck_tls_sni: The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty
-               value, it cannot be reset to its default empty value later on (requires a resource re-creation).
+        :param pulumi.Input[bool] healthcheck_tls_skip_verify: Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
+        :param pulumi.Input[str] healthcheck_tls_sni: The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty value, it cannot be reset to its default empty value later on (requires a resource re-creation).
         :param pulumi.Input[str] ip_address: The Elastic IP (EIP) IPv4 address.
         :param pulumi.Input[str] reverse_dns: The EIP reverse DNS record (must end with a `.`; e.g: `my-eip.example.net.`).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
-        :param pulumi.Input[str] zone: The Exoscale Zone name
+        :param pulumi.Input[str] zone: ❗ The Exoscale Zone name
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if healthcheck_interval is not None:
             pulumi.set(__self__, "healthcheck_interval", healthcheck_interval)
         if healthcheck_mode is not None:
             pulumi.set(__self__, "healthcheck_mode", healthcheck_mode)
@@ -319,15 +313,15 @@
     def healthcheck_interval(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "healthcheck_interval", value)
 
     @property
     @pulumi.getter(name="healthcheckMode")
     def healthcheck_mode(self) -> Optional[pulumi.Input[str]]:
         """
-        The healthcheck probing mode (must be `tcp`, `http` or `https`).
+        ❗ The healthcheck probing mode (must be `tcp`, `http` or `https`).
         """
         return pulumi.get(self, "healthcheck_mode")
 
     @healthcheck_mode.setter
     def healthcheck_mode(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "healthcheck_mode", value)
 
@@ -391,29 +385,27 @@
     def healthcheck_timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "healthcheck_timeout", value)
 
     @property
     @pulumi.getter(name="healthcheckTlsSkipVerify")
     def healthcheck_tls_skip_verify(self) -> Optional[pulumi.Input[bool]]:
         """
-        Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed
-        to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
+        Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
         """
         return pulumi.get(self, "healthcheck_tls_skip_verify")
 
     @healthcheck_tls_skip_verify.setter
     def healthcheck_tls_skip_verify(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "healthcheck_tls_skip_verify", value)
 
     @property
     @pulumi.getter(name="healthcheckTlsSni")
     def healthcheck_tls_sni(self) -> Optional[pulumi.Input[str]]:
         """
-        The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty
-        value, it cannot be reset to its default empty value later on (requires a resource re-creation).
+        The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty value, it cannot be reset to its default empty value later on (requires a resource re-creation).
         """
         return pulumi.get(self, "healthcheck_tls_sni")
 
     @healthcheck_tls_sni.setter
     def healthcheck_tls_sni(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "healthcheck_tls_sni", value)
 
@@ -453,15 +445,15 @@
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The Exoscale Zone name
+        ❗ The Exoscale Zone name
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -488,27 +480,25 @@
         """
         !> **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use ElasticIP instead.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A free-form text describing the Elastic IP (EIP).
         :param pulumi.Input[int] healthcheck_interval: The healthcheck probing interval (seconds; must be between `5` and `300`).
-        :param pulumi.Input[str] healthcheck_mode: The healthcheck probing mode (must be `tcp`, `http` or `https`).
+        :param pulumi.Input[str] healthcheck_mode: ❗ The healthcheck probing mode (must be `tcp`, `http` or `https`).
         :param pulumi.Input[str] healthcheck_path: The healthcheck probe HTTP request path (must be specified in `http`/`https` modes).
         :param pulumi.Input[int] healthcheck_port: The healthcheck service port to probe (must be between `1` and `65535`).
         :param pulumi.Input[int] healthcheck_strikes_fail: The number of unsuccessful healthcheck probes before considering the target unhealthy (must be between `1` and `20`).
         :param pulumi.Input[int] healthcheck_strikes_ok: The number of successful healthcheck probes before considering the target healthy (must be between `1` and `20`).
         :param pulumi.Input[int] healthcheck_timeout: The time in seconds before considering a healthcheck probing failed (must be between `2` and `60`).
-        :param pulumi.Input[bool] healthcheck_tls_skip_verify: Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed
-               to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
-        :param pulumi.Input[str] healthcheck_tls_sni: The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty
-               value, it cannot be reset to its default empty value later on (requires a resource re-creation).
+        :param pulumi.Input[bool] healthcheck_tls_skip_verify: Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
+        :param pulumi.Input[str] healthcheck_tls_sni: The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty value, it cannot be reset to its default empty value later on (requires a resource re-creation).
         :param pulumi.Input[str] reverse_dns: The EIP reverse DNS record (must end with a `.`; e.g: `my-eip.example.net.`).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
-        :param pulumi.Input[str] zone: The Exoscale Zone name
+        :param pulumi.Input[str] zone: ❗ The Exoscale Zone name
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: IPAddressArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -597,28 +587,26 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A free-form text describing the Elastic IP (EIP).
         :param pulumi.Input[int] healthcheck_interval: The healthcheck probing interval (seconds; must be between `5` and `300`).
-        :param pulumi.Input[str] healthcheck_mode: The healthcheck probing mode (must be `tcp`, `http` or `https`).
+        :param pulumi.Input[str] healthcheck_mode: ❗ The healthcheck probing mode (must be `tcp`, `http` or `https`).
         :param pulumi.Input[str] healthcheck_path: The healthcheck probe HTTP request path (must be specified in `http`/`https` modes).
         :param pulumi.Input[int] healthcheck_port: The healthcheck service port to probe (must be between `1` and `65535`).
         :param pulumi.Input[int] healthcheck_strikes_fail: The number of unsuccessful healthcheck probes before considering the target unhealthy (must be between `1` and `20`).
         :param pulumi.Input[int] healthcheck_strikes_ok: The number of successful healthcheck probes before considering the target healthy (must be between `1` and `20`).
         :param pulumi.Input[int] healthcheck_timeout: The time in seconds before considering a healthcheck probing failed (must be between `2` and `60`).
-        :param pulumi.Input[bool] healthcheck_tls_skip_verify: Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed
-               to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
-        :param pulumi.Input[str] healthcheck_tls_sni: The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty
-               value, it cannot be reset to its default empty value later on (requires a resource re-creation).
+        :param pulumi.Input[bool] healthcheck_tls_skip_verify: Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
+        :param pulumi.Input[str] healthcheck_tls_sni: The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty value, it cannot be reset to its default empty value later on (requires a resource re-creation).
         :param pulumi.Input[str] ip_address: The Elastic IP (EIP) IPv4 address.
         :param pulumi.Input[str] reverse_dns: The EIP reverse DNS record (must end with a `.`; e.g: `my-eip.example.net.`).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
-        :param pulumi.Input[str] zone: The Exoscale Zone name
+        :param pulumi.Input[str] zone: ❗ The Exoscale Zone name
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _IPAddressState.__new__(_IPAddressState)
 
         __props__.__dict__["description"] = description
         __props__.__dict__["healthcheck_interval"] = healthcheck_interval
@@ -652,15 +640,15 @@
         """
         return pulumi.get(self, "healthcheck_interval")
 
     @property
     @pulumi.getter(name="healthcheckMode")
     def healthcheck_mode(self) -> pulumi.Output[Optional[str]]:
         """
-        The healthcheck probing mode (must be `tcp`, `http` or `https`).
+        ❗ The healthcheck probing mode (must be `tcp`, `http` or `https`).
         """
         return pulumi.get(self, "healthcheck_mode")
 
     @property
     @pulumi.getter(name="healthcheckPath")
     def healthcheck_path(self) -> pulumi.Output[Optional[str]]:
         """
@@ -700,25 +688,23 @@
         """
         return pulumi.get(self, "healthcheck_timeout")
 
     @property
     @pulumi.getter(name="healthcheckTlsSkipVerify")
     def healthcheck_tls_skip_verify(self) -> pulumi.Output[Optional[bool]]:
         """
-        Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed
-        to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
+        Disable TLS certificate validation in `https` mode (boolean; default: `false`). Note: this parameter can only be changed to `true`, it cannot be reset to `false` later on (requires a resource re-creation).
         """
         return pulumi.get(self, "healthcheck_tls_skip_verify")
 
     @property
     @pulumi.getter(name="healthcheckTlsSni")
     def healthcheck_tls_sni(self) -> pulumi.Output[Optional[str]]:
         """
-        The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty
-        value, it cannot be reset to its default empty value later on (requires a resource re-creation).
+        The healthcheck TLS server name to specify in `https` mode. Note: this parameter can only be changed to a non-empty value, it cannot be reset to its default empty value later on (requires a resource re-creation).
         """
         return pulumi.get(self, "healthcheck_tls_sni")
 
     @property
     @pulumi.getter(name="ipAddress")
     def ip_address(self) -> pulumi.Output[str]:
         """
@@ -742,11 +728,11 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale Zone name
+        ❗ The Exoscale Zone name
         """
         return pulumi.get(self, "zone")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/network.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/network.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,20 +20,19 @@
                  name: Optional[pulumi.Input[str]] = None,
                  netmask: Optional[pulumi.Input[str]] = None,
                  network_offering: Optional[pulumi.Input[str]] = None,
                  start_ip: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a Network resource.
-        :param pulumi.Input[str] zone: The Exoscale Zone name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale Zone name.
         :param pulumi.Input[str] display_text: A free-form text describing the network.
         :param pulumi.Input[str] end_ip: The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
         :param pulumi.Input[str] name: The private network name.
-        :param pulumi.Input[str] netmask: The network mask defining the IP network allowed for static leases (see `exoscale_nic` resource). Required for *managed*
-               private networks.
+        :param pulumi.Input[str] netmask: The network mask defining the IP network allowed for static leases (see `NIC` resource). Required for *managed* private networks.
         :param pulumi.Input[str] start_ip: The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
         """
         pulumi.set(__self__, "zone", zone)
         if display_text is not None:
             pulumi.set(__self__, "display_text", display_text)
         if end_ip is not None:
@@ -52,15 +51,15 @@
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
-        The Exoscale Zone name.
+        ❗ The Exoscale Zone name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
@@ -100,26 +99,28 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def netmask(self) -> Optional[pulumi.Input[str]]:
         """
-        The network mask defining the IP network allowed for static leases (see `exoscale_nic` resource). Required for *managed*
-        private networks.
+        The network mask defining the IP network allowed for static leases (see `NIC` resource). Required for *managed* private networks.
         """
         return pulumi.get(self, "netmask")
 
     @netmask.setter
     def netmask(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "netmask", value)
 
     @property
     @pulumi.getter(name="networkOffering")
     def network_offering(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""This attribute is deprecated, please remove it from your configuration.""", DeprecationWarning)
+        pulumi.log.warn("""network_offering is deprecated: This attribute is deprecated, please remove it from your configuration.""")
+
         return pulumi.get(self, "network_offering")
 
     @network_offering.setter
     def network_offering(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "network_offering", value)
 
     @property
@@ -159,19 +160,18 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Network resources.
         :param pulumi.Input[str] display_text: A free-form text describing the network.
         :param pulumi.Input[str] end_ip: The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
         :param pulumi.Input[str] name: The private network name.
-        :param pulumi.Input[str] netmask: The network mask defining the IP network allowed for static leases (see `exoscale_nic` resource). Required for *managed*
-               private networks.
+        :param pulumi.Input[str] netmask: The network mask defining the IP network allowed for static leases (see `NIC` resource). Required for *managed* private networks.
         :param pulumi.Input[str] start_ip: The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
-        :param pulumi.Input[str] zone: The Exoscale Zone name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale Zone name.
         """
         if display_text is not None:
             pulumi.set(__self__, "display_text", display_text)
         if end_ip is not None:
             pulumi.set(__self__, "end_ip", end_ip)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -225,26 +225,28 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def netmask(self) -> Optional[pulumi.Input[str]]:
         """
-        The network mask defining the IP network allowed for static leases (see `exoscale_nic` resource). Required for *managed*
-        private networks.
+        The network mask defining the IP network allowed for static leases (see `NIC` resource). Required for *managed* private networks.
         """
         return pulumi.get(self, "netmask")
 
     @netmask.setter
     def netmask(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "netmask", value)
 
     @property
     @pulumi.getter(name="networkOffering")
     def network_offering(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""This attribute is deprecated, please remove it from your configuration.""", DeprecationWarning)
+        pulumi.log.warn("""network_offering is deprecated: This attribute is deprecated, please remove it from your configuration.""")
+
         return pulumi.get(self, "network_offering")
 
     @network_offering.setter
     def network_offering(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "network_offering", value)
 
     @property
@@ -271,15 +273,15 @@
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The Exoscale Zone name.
+        ❗ The Exoscale Zone name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -302,19 +304,18 @@
         !> **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use PrivateNetwork instead.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] display_text: A free-form text describing the network.
         :param pulumi.Input[str] end_ip: The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
         :param pulumi.Input[str] name: The private network name.
-        :param pulumi.Input[str] netmask: The network mask defining the IP network allowed for static leases (see `exoscale_nic` resource). Required for *managed*
-               private networks.
+        :param pulumi.Input[str] netmask: The network mask defining the IP network allowed for static leases (see `NIC` resource). Required for *managed* private networks.
         :param pulumi.Input[str] start_ip: The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
-        :param pulumi.Input[str] zone: The Exoscale Zone name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale Zone name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: NetworkArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -390,19 +391,18 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] display_text: A free-form text describing the network.
         :param pulumi.Input[str] end_ip: The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
         :param pulumi.Input[str] name: The private network name.
-        :param pulumi.Input[str] netmask: The network mask defining the IP network allowed for static leases (see `exoscale_nic` resource). Required for *managed*
-               private networks.
+        :param pulumi.Input[str] netmask: The network mask defining the IP network allowed for static leases (see `NIC` resource). Required for *managed* private networks.
         :param pulumi.Input[str] start_ip: The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags (key/value). To remove all tags, set `tags = {}`.
-        :param pulumi.Input[str] zone: The Exoscale Zone name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale Zone name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _NetworkState.__new__(_NetworkState)
 
         __props__.__dict__["display_text"] = display_text
         __props__.__dict__["end_ip"] = end_ip
@@ -438,22 +438,24 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def netmask(self) -> pulumi.Output[Optional[str]]:
         """
-        The network mask defining the IP network allowed for static leases (see `exoscale_nic` resource). Required for *managed*
-        private networks.
+        The network mask defining the IP network allowed for static leases (see `NIC` resource). Required for *managed* private networks.
         """
         return pulumi.get(self, "netmask")
 
     @property
     @pulumi.getter(name="networkOffering")
     def network_offering(self) -> pulumi.Output[Optional[str]]:
+        warnings.warn("""This attribute is deprecated, please remove it from your configuration.""", DeprecationWarning)
+        pulumi.log.warn("""network_offering is deprecated: This attribute is deprecated, please remove it from your configuration.""")
+
         return pulumi.get(self, "network_offering")
 
     @property
     @pulumi.getter(name="startIp")
     def start_ip(self) -> pulumi.Output[Optional[str]]:
         """
         The first/last IP addresses used by the DHCP service for dynamic leases. Required for *managed* private networks.
@@ -468,11 +470,11 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale Zone name.
+        ❗ The Exoscale Zone name.
         """
         return pulumi.get(self, "zone")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/nic.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/nic.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,40 +15,40 @@
 class NICArgs:
     def __init__(__self__, *,
                  compute_id: pulumi.Input[str],
                  network_id: pulumi.Input[str],
                  ip_address: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a NIC resource.
-        :param pulumi.Input[str] compute_id: The compute instance ID.
-        :param pulumi.Input[str] network_id: The private network ID.
+        :param pulumi.Input[str] compute_id: ❗ The compute instance ID.
+        :param pulumi.Input[str] network_id: ❗ The private network ID.
         :param pulumi.Input[str] ip_address: The IPv4 address to request as static DHCP lease if the NIC is attached to a *managed* private network.
         """
         pulumi.set(__self__, "compute_id", compute_id)
         pulumi.set(__self__, "network_id", network_id)
         if ip_address is not None:
             pulumi.set(__self__, "ip_address", ip_address)
 
     @property
     @pulumi.getter(name="computeId")
     def compute_id(self) -> pulumi.Input[str]:
         """
-        The compute instance ID.
+        ❗ The compute instance ID.
         """
         return pulumi.get(self, "compute_id")
 
     @compute_id.setter
     def compute_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "compute_id", value)
 
     @property
     @pulumi.getter(name="networkId")
     def network_id(self) -> pulumi.Input[str]:
         """
-        The private network ID.
+        ❗ The private network ID.
         """
         return pulumi.get(self, "network_id")
 
     @network_id.setter
     def network_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "network_id", value)
 
@@ -72,18 +72,18 @@
                  gateway: Optional[pulumi.Input[str]] = None,
                  ip_address: Optional[pulumi.Input[str]] = None,
                  mac_address: Optional[pulumi.Input[str]] = None,
                  netmask: Optional[pulumi.Input[str]] = None,
                  network_id: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering NIC resources.
-        :param pulumi.Input[str] compute_id: The compute instance ID.
+        :param pulumi.Input[str] compute_id: ❗ The compute instance ID.
         :param pulumi.Input[str] ip_address: The IPv4 address to request as static DHCP lease if the NIC is attached to a *managed* private network.
         :param pulumi.Input[str] mac_address: The NIC MAC address.
-        :param pulumi.Input[str] network_id: The private network ID.
+        :param pulumi.Input[str] network_id: ❗ The private network ID.
         """
         if compute_id is not None:
             pulumi.set(__self__, "compute_id", compute_id)
         if gateway is not None:
             pulumi.set(__self__, "gateway", gateway)
         if ip_address is not None:
             pulumi.set(__self__, "ip_address", ip_address)
@@ -94,15 +94,15 @@
         if network_id is not None:
             pulumi.set(__self__, "network_id", network_id)
 
     @property
     @pulumi.getter(name="computeId")
     def compute_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The compute instance ID.
+        ❗ The compute instance ID.
         """
         return pulumi.get(self, "compute_id")
 
     @compute_id.setter
     def compute_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "compute_id", value)
 
@@ -148,15 +148,15 @@
     def netmask(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "netmask", value)
 
     @property
     @pulumi.getter(name="networkId")
     def network_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The private network ID.
+        ❗ The private network ID.
         """
         return pulumi.get(self, "network_id")
 
     @network_id.setter
     def network_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "network_id", value)
 
@@ -171,17 +171,17 @@
                  network_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         !> **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use ComputeInstance `network_interface` block instead.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] compute_id: The compute instance ID.
+        :param pulumi.Input[str] compute_id: ❗ The compute instance ID.
         :param pulumi.Input[str] ip_address: The IPv4 address to request as static DHCP lease if the NIC is attached to a *managed* private network.
-        :param pulumi.Input[str] network_id: The private network ID.
+        :param pulumi.Input[str] network_id: ❗ The private network ID.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: NICArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -244,18 +244,18 @@
         """
         Get an existing NIC resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] compute_id: The compute instance ID.
+        :param pulumi.Input[str] compute_id: ❗ The compute instance ID.
         :param pulumi.Input[str] ip_address: The IPv4 address to request as static DHCP lease if the NIC is attached to a *managed* private network.
         :param pulumi.Input[str] mac_address: The NIC MAC address.
-        :param pulumi.Input[str] network_id: The private network ID.
+        :param pulumi.Input[str] network_id: ❗ The private network ID.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _NICState.__new__(_NICState)
 
         __props__.__dict__["compute_id"] = compute_id
         __props__.__dict__["gateway"] = gateway
@@ -265,15 +265,15 @@
         __props__.__dict__["network_id"] = network_id
         return NIC(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="computeId")
     def compute_id(self) -> pulumi.Output[str]:
         """
-        The compute instance ID.
+        ❗ The compute instance ID.
         """
         return pulumi.get(self, "compute_id")
 
     @property
     @pulumi.getter
     def gateway(self) -> pulumi.Output[str]:
         return pulumi.get(self, "gateway")
@@ -299,11 +299,11 @@
     def netmask(self) -> pulumi.Output[str]:
         return pulumi.get(self, "netmask")
 
     @property
     @pulumi.getter(name="networkId")
     def network_id(self) -> pulumi.Output[str]:
         """
-        The private network ID.
+        ❗ The private network ID.
         """
         return pulumi.get(self, "network_id")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/nlb.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/nlb.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def __init__(__self__, *,
                  zone: pulumi.Input[str],
                  description: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a NLB resource.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         :param pulumi.Input[str] description: A free-form text describing the NLB.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The network load balancer (NLB) name.
         """
         pulumi.set(__self__, "zone", zone)
         if description is not None:
             pulumi.set(__self__, "description", description)
@@ -33,15 +33,15 @@
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
@@ -96,17 +96,17 @@
         """
         Input properties used for looking up and filtering NLB resources.
         :param pulumi.Input[str] created_at: The NLB creation date.
         :param pulumi.Input[str] description: A free-form text describing the NLB.
         :param pulumi.Input[str] ip_address: The NLB IPv4 address.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The network load balancer (NLB) name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: The list of the [exoscale_nlb_service](./nlb_service.md) (names).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: The list of the exoscale*nlb*service (names).
         :param pulumi.Input[str] state: The current NLB state.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if ip_address is not None:
             pulumi.set(__self__, "ip_address", ip_address)
@@ -181,15 +181,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def services(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The list of the [exoscale_nlb_service](./nlb_service.md) (names).
+        The list of the exoscale*nlb*service (names).
         """
         return pulumi.get(self, "services")
 
     @services.setter
     def services(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "services", value)
 
@@ -205,15 +205,15 @@
     def state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "state", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -242,15 +242,15 @@
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A free-form text describing the NLB.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The network load balancer (NLB) name.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: NLBArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -331,17 +331,17 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] created_at: The NLB creation date.
         :param pulumi.Input[str] description: A free-form text describing the NLB.
         :param pulumi.Input[str] ip_address: The NLB IPv4 address.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The network load balancer (NLB) name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: The list of the [exoscale_nlb_service](./nlb_service.md) (names).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: The list of the exoscale*nlb*service (names).
         :param pulumi.Input[str] state: The current NLB state.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _NLBState.__new__(_NLBState)
 
         __props__.__dict__["created_at"] = created_at
         __props__.__dict__["description"] = description
@@ -393,15 +393,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def services(self) -> pulumi.Output[Sequence[str]]:
         """
-        The list of the [exoscale_nlb_service](./nlb_service.md) (names).
+        The list of the exoscale*nlb*service (names).
         """
         return pulumi.get(self, "services")
 
     @property
     @pulumi.getter
     def state(self) -> pulumi.Output[str]:
         """
@@ -409,11 +409,11 @@
         """
         return pulumi.get(self, "state")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/nlb_service.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/nlb_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,19 +25,19 @@
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  protocol: Optional[pulumi.Input[str]] = None,
                  strategy: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a NLBService resource.
         :param pulumi.Input[Sequence[pulumi.Input['NLBServiceHealthcheckArgs']]] healthchecks: The service health checking configuration (may only bet set at creation time).
-        :param pulumi.Input[str] instance_pool_id: The [exoscale_instance_pool](./instance_pool.md) (ID) to forward traffic to.
-        :param pulumi.Input[str] nlb_id: The parent [exoscale_nlb](./nlb.md) ID.
+        :param pulumi.Input[str] instance_pool_id: The exoscale*instance*pool (ID) to forward traffic to.
+        :param pulumi.Input[str] nlb_id: ❗ The parent NLB ID.
         :param pulumi.Input[int] port: The healthcheck port.
         :param pulumi.Input[int] target_port: The (TCP/UDP) port to forward traffic to (on target instance pool members).
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         :param pulumi.Input[str] description: A free-form text describing the NLB service.
         :param pulumi.Input[str] name: The NLB service name.
         :param pulumi.Input[str] protocol: The protocol (`tcp`|`udp`; default: `tcp`).
         :param pulumi.Input[str] strategy: The strategy (`round-robin`|`source-hash`; default: `round-robin`).
         """
         pulumi.set(__self__, "healthchecks", healthchecks)
         pulumi.set(__self__, "instance_pool_id", instance_pool_id)
@@ -66,27 +66,27 @@
     def healthchecks(self, value: pulumi.Input[Sequence[pulumi.Input['NLBServiceHealthcheckArgs']]]):
         pulumi.set(self, "healthchecks", value)
 
     @property
     @pulumi.getter(name="instancePoolId")
     def instance_pool_id(self) -> pulumi.Input[str]:
         """
-        The [exoscale_instance_pool](./instance_pool.md) (ID) to forward traffic to.
+        The exoscale*instance*pool (ID) to forward traffic to.
         """
         return pulumi.get(self, "instance_pool_id")
 
     @instance_pool_id.setter
     def instance_pool_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "instance_pool_id", value)
 
     @property
     @pulumi.getter(name="nlbId")
     def nlb_id(self) -> pulumi.Input[str]:
         """
-        The parent [exoscale_nlb](./nlb.md) ID.
+        ❗ The parent NLB ID.
         """
         return pulumi.get(self, "nlb_id")
 
     @nlb_id.setter
     def nlb_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "nlb_id", value)
 
@@ -114,15 +114,15 @@
     def target_port(self, value: pulumi.Input[int]):
         pulumi.set(self, "target_port", value)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
@@ -189,22 +189,22 @@
                  strategy: Optional[pulumi.Input[str]] = None,
                  target_port: Optional[pulumi.Input[int]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering NLBService resources.
         :param pulumi.Input[str] description: A free-form text describing the NLB service.
         :param pulumi.Input[Sequence[pulumi.Input['NLBServiceHealthcheckArgs']]] healthchecks: The service health checking configuration (may only bet set at creation time).
-        :param pulumi.Input[str] instance_pool_id: The [exoscale_instance_pool](./instance_pool.md) (ID) to forward traffic to.
+        :param pulumi.Input[str] instance_pool_id: The exoscale*instance*pool (ID) to forward traffic to.
         :param pulumi.Input[str] name: The NLB service name.
-        :param pulumi.Input[str] nlb_id: The parent [exoscale_nlb](./nlb.md) ID.
+        :param pulumi.Input[str] nlb_id: ❗ The parent NLB ID.
         :param pulumi.Input[int] port: The healthcheck port.
         :param pulumi.Input[str] protocol: The protocol (`tcp`|`udp`; default: `tcp`).
         :param pulumi.Input[str] strategy: The strategy (`round-robin`|`source-hash`; default: `round-robin`).
         :param pulumi.Input[int] target_port: The (TCP/UDP) port to forward traffic to (on target instance pool members).
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if healthchecks is not None:
             pulumi.set(__self__, "healthchecks", healthchecks)
         if instance_pool_id is not None:
             pulumi.set(__self__, "instance_pool_id", instance_pool_id)
@@ -249,15 +249,15 @@
     def healthchecks(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['NLBServiceHealthcheckArgs']]]]):
         pulumi.set(self, "healthchecks", value)
 
     @property
     @pulumi.getter(name="instancePoolId")
     def instance_pool_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The [exoscale_instance_pool](./instance_pool.md) (ID) to forward traffic to.
+        The exoscale*instance*pool (ID) to forward traffic to.
         """
         return pulumi.get(self, "instance_pool_id")
 
     @instance_pool_id.setter
     def instance_pool_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "instance_pool_id", value)
 
@@ -273,15 +273,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="nlbId")
     def nlb_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The parent [exoscale_nlb](./nlb.md) ID.
+        ❗ The parent NLB ID.
         """
         return pulumi.get(self, "nlb_id")
 
     @nlb_id.setter
     def nlb_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "nlb_id", value)
 
@@ -342,15 +342,15 @@
     def target_port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "target_port", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -384,22 +384,22 @@
 
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6/9ecc6b8b-73d4-4211-8ced-f7f29bb79524@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A free-form text describing the NLB service.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NLBServiceHealthcheckArgs']]]] healthchecks: The service health checking configuration (may only bet set at creation time).
-        :param pulumi.Input[str] instance_pool_id: The [exoscale_instance_pool](./instance_pool.md) (ID) to forward traffic to.
+        :param pulumi.Input[str] instance_pool_id: The exoscale*instance*pool (ID) to forward traffic to.
         :param pulumi.Input[str] name: The NLB service name.
-        :param pulumi.Input[str] nlb_id: The parent [exoscale_nlb](./nlb.md) ID.
+        :param pulumi.Input[str] nlb_id: ❗ The parent NLB ID.
         :param pulumi.Input[int] port: The healthcheck port.
         :param pulumi.Input[str] protocol: The protocol (`tcp`|`udp`; default: `tcp`).
         :param pulumi.Input[str] strategy: The strategy (`round-robin`|`source-hash`; default: `round-robin`).
         :param pulumi.Input[int] target_port: The (TCP/UDP) port to forward traffic to (on target instance pool members).
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: NLBServiceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -499,22 +499,22 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A free-form text describing the NLB service.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NLBServiceHealthcheckArgs']]]] healthchecks: The service health checking configuration (may only bet set at creation time).
-        :param pulumi.Input[str] instance_pool_id: The [exoscale_instance_pool](./instance_pool.md) (ID) to forward traffic to.
+        :param pulumi.Input[str] instance_pool_id: The exoscale*instance*pool (ID) to forward traffic to.
         :param pulumi.Input[str] name: The NLB service name.
-        :param pulumi.Input[str] nlb_id: The parent [exoscale_nlb](./nlb.md) ID.
+        :param pulumi.Input[str] nlb_id: ❗ The parent NLB ID.
         :param pulumi.Input[int] port: The healthcheck port.
         :param pulumi.Input[str] protocol: The protocol (`tcp`|`udp`; default: `tcp`).
         :param pulumi.Input[str] strategy: The strategy (`round-robin`|`source-hash`; default: `round-robin`).
         :param pulumi.Input[int] target_port: The (TCP/UDP) port to forward traffic to (on target instance pool members).
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _NLBServiceState.__new__(_NLBServiceState)
 
         __props__.__dict__["description"] = description
         __props__.__dict__["healthchecks"] = healthchecks
@@ -545,15 +545,15 @@
         """
         return pulumi.get(self, "healthchecks")
 
     @property
     @pulumi.getter(name="instancePoolId")
     def instance_pool_id(self) -> pulumi.Output[str]:
         """
-        The [exoscale_instance_pool](./instance_pool.md) (ID) to forward traffic to.
+        The exoscale*instance*pool (ID) to forward traffic to.
         """
         return pulumi.get(self, "instance_pool_id")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
@@ -561,15 +561,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="nlbId")
     def nlb_id(self) -> pulumi.Output[str]:
         """
-        The parent [exoscale_nlb](./nlb.md) ID.
+        ❗ The parent NLB ID.
         """
         return pulumi.get(self, "nlb_id")
 
     @property
     @pulumi.getter
     def port(self) -> pulumi.Output[int]:
         """
@@ -606,11 +606,11 @@
         """
         return pulumi.get(self, "target_port")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/private_network.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/private_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                  description: Optional[pulumi.Input[str]] = None,
                  end_ip: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  netmask: Optional[pulumi.Input[str]] = None,
                  start_ip: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a PrivateNetwork resource.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         :param pulumi.Input[str] description: A free-form text describing the network.
         :param pulumi.Input[str] end_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         :param pulumi.Input[str] name: The private network name.
         :param pulumi.Input[str] netmask: (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
         :param pulumi.Input[str] start_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         """
         pulumi.set(__self__, "zone", zone)
@@ -41,15 +41,15 @@
         if start_ip is not None:
             pulumi.set(__self__, "start_ip", start_ip)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
@@ -126,15 +126,15 @@
         """
         Input properties used for looking up and filtering PrivateNetwork resources.
         :param pulumi.Input[str] description: A free-form text describing the network.
         :param pulumi.Input[str] end_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         :param pulumi.Input[str] name: The private network name.
         :param pulumi.Input[str] netmask: (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
         :param pulumi.Input[str] start_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if end_ip is not None:
             pulumi.set(__self__, "end_ip", end_ip)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -205,15 +205,15 @@
     def start_ip(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "start_ip", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -246,15 +246,15 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A free-form text describing the network.
         :param pulumi.Input[str] end_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         :param pulumi.Input[str] name: The private network name.
         :param pulumi.Input[str] netmask: (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
         :param pulumi.Input[str] start_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: PrivateNetworkArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -333,15 +333,15 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A free-form text describing the network.
         :param pulumi.Input[str] end_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         :param pulumi.Input[str] name: The private network name.
         :param pulumi.Input[str] netmask: (For managed Privnets) The network mask defining the IPv4 network allowed for static leases.
         :param pulumi.Input[str] start_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _PrivateNetworkState.__new__(_PrivateNetworkState)
 
         __props__.__dict__["description"] = description
         __props__.__dict__["end_ip"] = end_ip
@@ -391,11 +391,11 @@
         """
         return pulumi.get(self, "start_ip")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/provider.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,17 @@
     @config.setter
     def config(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "config", value)
 
     @property
     @pulumi.getter
     def delay(self) -> Optional[pulumi.Input[int]]:
+        warnings.warn("""Does nothing""", DeprecationWarning)
+        pulumi.log.warn("""delay is deprecated: Does nothing""")
+
         return pulumi.get(self, "delay")
 
     @delay.setter
     def delay(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "delay", value)
 
     @property
@@ -148,14 +151,17 @@
     @key.setter
     def key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def profile(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""Use region instead""", DeprecationWarning)
+        pulumi.log.warn("""profile is deprecated: Use region instead""")
+
         return pulumi.get(self, "profile")
 
     @profile.setter
     def profile(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "profile", value)
 
     @property
@@ -193,14 +199,17 @@
     @timeout.setter
     def timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout", value)
 
     @property
     @pulumi.getter
     def token(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""Use key instead""", DeprecationWarning)
+        pulumi.log.warn("""token is deprecated: Use key instead""")
+
         return pulumi.get(self, "token")
 
     @token.setter
     def token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "token", value)
 
 
@@ -352,14 +361,17 @@
         Exoscale API key
         """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def profile(self) -> pulumi.Output[Optional[str]]:
+        warnings.warn("""Use region instead""", DeprecationWarning)
+        pulumi.log.warn("""profile is deprecated: Use region instead""")
+
         return pulumi.get(self, "profile")
 
     @property
     @pulumi.getter
     def region(self) -> pulumi.Output[Optional[str]]:
         """
         CloudStack ini configuration section name (by default: cloudstack)
@@ -373,9 +385,12 @@
         Exoscale API secret
         """
         return pulumi.get(self, "secret")
 
     @property
     @pulumi.getter
     def token(self) -> pulumi.Output[Optional[str]]:
+        warnings.warn("""Use key instead""", DeprecationWarning)
+        pulumi.log.warn("""token is deprecated: Use key instead""")
+
         return pulumi.get(self, "token")
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/secondary_ip_address.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/secondary_ip_address.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,37 +14,37 @@
 @pulumi.input_type
 class SecondaryIPAddressArgs:
     def __init__(__self__, *,
                  compute_id: pulumi.Input[str],
                  ip_address: pulumi.Input[str]):
         """
         The set of arguments for constructing a SecondaryIPAddress resource.
-        :param pulumi.Input[str] compute_id: The compute instance ID.
-        :param pulumi.Input[str] ip_address: The Elastic IP (EIP) address.
+        :param pulumi.Input[str] compute_id: ❗ The compute instance ID.
+        :param pulumi.Input[str] ip_address: ❗ The Elastic IP (EIP) address.
         """
         pulumi.set(__self__, "compute_id", compute_id)
         pulumi.set(__self__, "ip_address", ip_address)
 
     @property
     @pulumi.getter(name="computeId")
     def compute_id(self) -> pulumi.Input[str]:
         """
-        The compute instance ID.
+        ❗ The compute instance ID.
         """
         return pulumi.get(self, "compute_id")
 
     @compute_id.setter
     def compute_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "compute_id", value)
 
     @property
     @pulumi.getter(name="ipAddress")
     def ip_address(self) -> pulumi.Input[str]:
         """
-        The Elastic IP (EIP) address.
+        ❗ The Elastic IP (EIP) address.
         """
         return pulumi.get(self, "ip_address")
 
     @ip_address.setter
     def ip_address(self, value: pulumi.Input[str]):
         pulumi.set(self, "ip_address", value)
 
@@ -54,16 +54,16 @@
     def __init__(__self__, *,
                  compute_id: Optional[pulumi.Input[str]] = None,
                  ip_address: Optional[pulumi.Input[str]] = None,
                  network_id: Optional[pulumi.Input[str]] = None,
                  nic_id: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SecondaryIPAddress resources.
-        :param pulumi.Input[str] compute_id: The compute instance ID.
-        :param pulumi.Input[str] ip_address: The Elastic IP (EIP) address.
+        :param pulumi.Input[str] compute_id: ❗ The compute instance ID.
+        :param pulumi.Input[str] ip_address: ❗ The Elastic IP (EIP) address.
         :param pulumi.Input[str] network_id: The network (ID) the compute instance NIC is attached to.
         :param pulumi.Input[str] nic_id: The network interface (NIC) ID.
         """
         if compute_id is not None:
             pulumi.set(__self__, "compute_id", compute_id)
         if ip_address is not None:
             pulumi.set(__self__, "ip_address", ip_address)
@@ -72,27 +72,27 @@
         if nic_id is not None:
             pulumi.set(__self__, "nic_id", nic_id)
 
     @property
     @pulumi.getter(name="computeId")
     def compute_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The compute instance ID.
+        ❗ The compute instance ID.
         """
         return pulumi.get(self, "compute_id")
 
     @compute_id.setter
     def compute_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "compute_id", value)
 
     @property
     @pulumi.getter(name="ipAddress")
     def ip_address(self) -> Optional[pulumi.Input[str]]:
         """
-        The Elastic IP (EIP) address.
+        ❗ The Elastic IP (EIP) address.
         """
         return pulumi.get(self, "ip_address")
 
     @ip_address.setter
     def ip_address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ip_address", value)
 
@@ -130,16 +130,16 @@
                  ip_address: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         !> **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use ComputeInstance `elastic_ip_ids` list instead.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] compute_id: The compute instance ID.
-        :param pulumi.Input[str] ip_address: The Elastic IP (EIP) address.
+        :param pulumi.Input[str] compute_id: ❗ The compute instance ID.
+        :param pulumi.Input[str] ip_address: ❗ The Elastic IP (EIP) address.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: SecondaryIPAddressArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -197,16 +197,16 @@
         """
         Get an existing SecondaryIPAddress resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] compute_id: The compute instance ID.
-        :param pulumi.Input[str] ip_address: The Elastic IP (EIP) address.
+        :param pulumi.Input[str] compute_id: ❗ The compute instance ID.
+        :param pulumi.Input[str] ip_address: ❗ The Elastic IP (EIP) address.
         :param pulumi.Input[str] network_id: The network (ID) the compute instance NIC is attached to.
         :param pulumi.Input[str] nic_id: The network interface (NIC) ID.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SecondaryIPAddressState.__new__(_SecondaryIPAddressState)
 
@@ -216,23 +216,23 @@
         __props__.__dict__["nic_id"] = nic_id
         return SecondaryIPAddress(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="computeId")
     def compute_id(self) -> pulumi.Output[str]:
         """
-        The compute instance ID.
+        ❗ The compute instance ID.
         """
         return pulumi.get(self, "compute_id")
 
     @property
     @pulumi.getter(name="ipAddress")
     def ip_address(self) -> pulumi.Output[str]:
         """
-        The Elastic IP (EIP) address.
+        ❗ The Elastic IP (EIP) address.
         """
         return pulumi.get(self, "ip_address")
 
     @property
     @pulumi.getter(name="networkId")
     def network_id(self) -> pulumi.Output[str]:
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/security_group.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/security_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,56 +15,54 @@
 class SecurityGroupArgs:
     def __init__(__self__, *,
                  description: Optional[pulumi.Input[str]] = None,
                  external_sources: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a SecurityGroup resource.
-        :param pulumi.Input[str] description: A free-form text describing the group.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_sources: A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio)
-               notation.
-        :param pulumi.Input[str] name: The security group name.
+        :param pulumi.Input[str] description: ❗ A free-form text describing the group.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_sources: A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio) notation.
+        :param pulumi.Input[str] name: ❗ The security group name.
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if external_sources is not None:
             pulumi.set(__self__, "external_sources", external_sources)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        A free-form text describing the group.
+        ❗ A free-form text describing the group.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="externalSources")
     def external_sources(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio)
-        notation.
+        A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio) notation.
         """
         return pulumi.get(self, "external_sources")
 
     @external_sources.setter
     def external_sources(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "external_sources", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The security group name.
+        ❗ The security group name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -73,56 +71,54 @@
 class _SecurityGroupState:
     def __init__(__self__, *,
                  description: Optional[pulumi.Input[str]] = None,
                  external_sources: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SecurityGroup resources.
-        :param pulumi.Input[str] description: A free-form text describing the group.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_sources: A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio)
-               notation.
-        :param pulumi.Input[str] name: The security group name.
+        :param pulumi.Input[str] description: ❗ A free-form text describing the group.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_sources: A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio) notation.
+        :param pulumi.Input[str] name: ❗ The security group name.
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if external_sources is not None:
             pulumi.set(__self__, "external_sources", external_sources)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        A free-form text describing the group.
+        ❗ A free-form text describing the group.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="externalSources")
     def external_sources(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio)
-        notation.
+        A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio) notation.
         """
         return pulumi.get(self, "external_sources")
 
     @external_sources.setter
     def external_sources(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "external_sources", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The security group name.
+        ❗ The security group name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -147,18 +143,17 @@
 
          exoscale_security_group.my_security_group \\
 
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] description: A free-form text describing the group.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_sources: A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio)
-               notation.
-        :param pulumi.Input[str] name: The security group name.
+        :param pulumi.Input[str] description: ❗ A free-form text describing the group.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_sources: A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio) notation.
+        :param pulumi.Input[str] name: ❗ The security group name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[SecurityGroupArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -221,46 +216,44 @@
         """
         Get an existing SecurityGroup resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] description: A free-form text describing the group.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_sources: A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio)
-               notation.
-        :param pulumi.Input[str] name: The security group name.
+        :param pulumi.Input[str] description: ❗ A free-form text describing the group.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_sources: A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio) notation.
+        :param pulumi.Input[str] name: ❗ The security group name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SecurityGroupState.__new__(_SecurityGroupState)
 
         __props__.__dict__["description"] = description
         __props__.__dict__["external_sources"] = external_sources
         __props__.__dict__["name"] = name
         return SecurityGroup(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
-        A free-form text describing the group.
+        ❗ A free-form text describing the group.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="externalSources")
     def external_sources(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio)
-        notation.
+        A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio) notation.
         """
         return pulumi.get(self, "external_sources")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The security group name.
+        ❗ The security group name.
         """
         return pulumi.get(self, "name")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/security_group_rule.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/security_group_rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,34 +25,27 @@
                  security_group: Optional[pulumi.Input[str]] = None,
                  security_group_id: Optional[pulumi.Input[str]] = None,
                  start_port: Optional[pulumi.Input[int]] = None,
                  user_security_group: Optional[pulumi.Input[str]] = None,
                  user_security_group_id: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a SecurityGroupRule resource.
-        :param pulumi.Input[str] type: The traffic direction to match (`INGRESS` or `EGRESS`).
-        :param pulumi.Input[str] cidr: An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR
-               notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with
-               `public_security_group`/`user_security_group`/`user_security_group_id`).
-        :param pulumi.Input[str] description: A free-form text describing the security group rule.
-        :param pulumi.Input[int] end_port: A `TCP`/`UDP` port range to match.
-        :param pulumi.Input[int] icmp_code: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
-        :param pulumi.Input[int] icmp_type: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
-        :param pulumi.Input[str] protocol: The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
-        :param pulumi.Input[str] public_security_group: An (`INGRESS`) source / (`EGRESS`) destination public security group name to match (conflicts with
-               `cidr`/`user_security_group`/`user_security_group_id`).
-        :param pulumi.Input[str] security_group: The parent security group name. Please use the `security_group_id` argument along the
-               [exoscale_security_group](../data-sources/security_group.md) data source instead.
-        :param pulumi.Input[str] security_group_id: The parent [exoscale_security_group](./security_group.md) ID.
-        :param pulumi.Input[int] start_port: A `TCP`/`UDP` port range to match.
-        :param pulumi.Input[str] user_security_group: An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with
-               `cidr`/`public_security_group`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
-               [exoscale_security_group](../data-sources/security_group.md) data source instead.
-        :param pulumi.Input[str] user_security_group_id: An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with
-               `cidr`/`public_security_group`/`user_security_group)`).
+        :param pulumi.Input[str] type: ❗ The traffic direction to match (`INGRESS` or `EGRESS`).
+        :param pulumi.Input[str] cidr: ❗ An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with `public_security_group`/`user_security_group`/`user_security_group_id`).
+        :param pulumi.Input[str] description: ❗ A free-form text describing the security group rule.
+        :param pulumi.Input[int] end_port: ❗ A `TCP`/`UDP` port range to match.
+        :param pulumi.Input[int] icmp_code: ❗ An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
+        :param pulumi.Input[int] icmp_type: ❗ An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
+        :param pulumi.Input[str] protocol: ❗ The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
+        :param pulumi.Input[str] public_security_group: ❗ An (`INGRESS`) source / (`EGRESS`) destination public security group name to match (conflicts with `cidr`/`user_security_group`/`user_security_group_id`).
+        :param pulumi.Input[str] security_group: ❗ The parent security group name. Please use the `security_group_id` argument along the exoscale*security*group data source instead.
+        :param pulumi.Input[str] security_group_id: ❗ The parent exoscale*security*group ID.
+        :param pulumi.Input[int] start_port: ❗ A `TCP`/`UDP` port range to match.
+        :param pulumi.Input[str] user_security_group: ❗ An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with `cidr`/`public_security_group`/`user_security_group_id`). Please use the `user_security_group_id` argument along the exoscale*security*group data source instead.
+        :param pulumi.Input[str] user_security_group_id: ❗ An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with `cidr`/`public_security_group`/`user_security_group)`).
         """
         pulumi.set(__self__, "type", type)
         if cidr is not None:
             pulumi.set(__self__, "cidr", cidr)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if end_port is not None:
@@ -82,166 +75,165 @@
         if user_security_group_id is not None:
             pulumi.set(__self__, "user_security_group_id", user_security_group_id)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         """
-        The traffic direction to match (`INGRESS` or `EGRESS`).
+        ❗ The traffic direction to match (`INGRESS` or `EGRESS`).
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def cidr(self) -> Optional[pulumi.Input[str]]:
         """
-        An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR
-        notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with
-        `public_security_group`/`user_security_group`/`user_security_group_id`).
+        ❗ An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with `public_security_group`/`user_security_group`/`user_security_group_id`).
         """
         return pulumi.get(self, "cidr")
 
     @cidr.setter
     def cidr(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cidr", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        A free-form text describing the security group rule.
+        ❗ A free-form text describing the security group rule.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="endPort")
     def end_port(self) -> Optional[pulumi.Input[int]]:
         """
-        A `TCP`/`UDP` port range to match.
+        ❗ A `TCP`/`UDP` port range to match.
         """
         return pulumi.get(self, "end_port")
 
     @end_port.setter
     def end_port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "end_port", value)
 
     @property
     @pulumi.getter(name="icmpCode")
     def icmp_code(self) -> Optional[pulumi.Input[int]]:
         """
-        An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
+        ❗ An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
         """
         return pulumi.get(self, "icmp_code")
 
     @icmp_code.setter
     def icmp_code(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "icmp_code", value)
 
     @property
     @pulumi.getter(name="icmpType")
     def icmp_type(self) -> Optional[pulumi.Input[int]]:
         """
-        An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
+        ❗ An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
         """
         return pulumi.get(self, "icmp_type")
 
     @icmp_type.setter
     def icmp_type(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "icmp_type", value)
 
     @property
     @pulumi.getter
     def protocol(self) -> Optional[pulumi.Input[str]]:
         """
-        The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
+        ❗ The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
         """
         return pulumi.get(self, "protocol")
 
     @protocol.setter
     def protocol(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "protocol", value)
 
     @property
     @pulumi.getter(name="publicSecurityGroup")
     def public_security_group(self) -> Optional[pulumi.Input[str]]:
         """
-        An (`INGRESS`) source / (`EGRESS`) destination public security group name to match (conflicts with
-        `cidr`/`user_security_group`/`user_security_group_id`).
+        ❗ An (`INGRESS`) source / (`EGRESS`) destination public security group name to match (conflicts with `cidr`/`user_security_group`/`user_security_group_id`).
         """
         return pulumi.get(self, "public_security_group")
 
     @public_security_group.setter
     def public_security_group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "public_security_group", value)
 
     @property
     @pulumi.getter(name="securityGroup")
     def security_group(self) -> Optional[pulumi.Input[str]]:
         """
-        The parent security group name. Please use the `security_group_id` argument along the
-        [exoscale_security_group](../data-sources/security_group.md) data source instead.
+        ❗ The parent security group name. Please use the `security_group_id` argument along the exoscale*security*group data source instead.
         """
+        warnings.warn("""Deprecated in favor of `security_group_id`""", DeprecationWarning)
+        pulumi.log.warn("""security_group is deprecated: Deprecated in favor of `security_group_id`""")
+
         return pulumi.get(self, "security_group")
 
     @security_group.setter
     def security_group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_group", value)
 
     @property
     @pulumi.getter(name="securityGroupId")
     def security_group_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The parent [exoscale_security_group](./security_group.md) ID.
+        ❗ The parent exoscale*security*group ID.
         """
         return pulumi.get(self, "security_group_id")
 
     @security_group_id.setter
     def security_group_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_group_id", value)
 
     @property
     @pulumi.getter(name="startPort")
     def start_port(self) -> Optional[pulumi.Input[int]]:
         """
-        A `TCP`/`UDP` port range to match.
+        ❗ A `TCP`/`UDP` port range to match.
         """
         return pulumi.get(self, "start_port")
 
     @start_port.setter
     def start_port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "start_port", value)
 
     @property
     @pulumi.getter(name="userSecurityGroup")
     def user_security_group(self) -> Optional[pulumi.Input[str]]:
         """
-        An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with
-        `cidr`/`public_security_group`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
-        [exoscale_security_group](../data-sources/security_group.md) data source instead.
+        ❗ An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with `cidr`/`public_security_group`/`user_security_group_id`). Please use the `user_security_group_id` argument along the exoscale*security*group data source instead.
         """
+        warnings.warn("""Deprecated in favor of `user_security_group_id`""", DeprecationWarning)
+        pulumi.log.warn("""user_security_group is deprecated: Deprecated in favor of `user_security_group_id`""")
+
         return pulumi.get(self, "user_security_group")
 
     @user_security_group.setter
     def user_security_group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_security_group", value)
 
     @property
     @pulumi.getter(name="userSecurityGroupId")
     def user_security_group_id(self) -> Optional[pulumi.Input[str]]:
         """
-        An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with
-        `cidr`/`public_security_group`/`user_security_group)`).
+        ❗ An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with `cidr`/`public_security_group`/`user_security_group)`).
         """
         return pulumi.get(self, "user_security_group_id")
 
     @user_security_group_id.setter
     def user_security_group_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_security_group_id", value)
 
@@ -260,34 +252,27 @@
                  security_group_id: Optional[pulumi.Input[str]] = None,
                  start_port: Optional[pulumi.Input[int]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  user_security_group: Optional[pulumi.Input[str]] = None,
                  user_security_group_id: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SecurityGroupRule resources.
-        :param pulumi.Input[str] cidr: An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR
-               notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with
-               `public_security_group`/`user_security_group`/`user_security_group_id`).
-        :param pulumi.Input[str] description: A free-form text describing the security group rule.
-        :param pulumi.Input[int] end_port: A `TCP`/`UDP` port range to match.
-        :param pulumi.Input[int] icmp_code: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
-        :param pulumi.Input[int] icmp_type: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
-        :param pulumi.Input[str] protocol: The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
-        :param pulumi.Input[str] public_security_group: An (`INGRESS`) source / (`EGRESS`) destination public security group name to match (conflicts with
-               `cidr`/`user_security_group`/`user_security_group_id`).
-        :param pulumi.Input[str] security_group: The parent security group name. Please use the `security_group_id` argument along the
-               [exoscale_security_group](../data-sources/security_group.md) data source instead.
-        :param pulumi.Input[str] security_group_id: The parent [exoscale_security_group](./security_group.md) ID.
-        :param pulumi.Input[int] start_port: A `TCP`/`UDP` port range to match.
-        :param pulumi.Input[str] type: The traffic direction to match (`INGRESS` or `EGRESS`).
-        :param pulumi.Input[str] user_security_group: An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with
-               `cidr`/`public_security_group`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
-               [exoscale_security_group](../data-sources/security_group.md) data source instead.
-        :param pulumi.Input[str] user_security_group_id: An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with
-               `cidr`/`public_security_group`/`user_security_group)`).
+        :param pulumi.Input[str] cidr: ❗ An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with `public_security_group`/`user_security_group`/`user_security_group_id`).
+        :param pulumi.Input[str] description: ❗ A free-form text describing the security group rule.
+        :param pulumi.Input[int] end_port: ❗ A `TCP`/`UDP` port range to match.
+        :param pulumi.Input[int] icmp_code: ❗ An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
+        :param pulumi.Input[int] icmp_type: ❗ An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
+        :param pulumi.Input[str] protocol: ❗ The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
+        :param pulumi.Input[str] public_security_group: ❗ An (`INGRESS`) source / (`EGRESS`) destination public security group name to match (conflicts with `cidr`/`user_security_group`/`user_security_group_id`).
+        :param pulumi.Input[str] security_group: ❗ The parent security group name. Please use the `security_group_id` argument along the exoscale*security*group data source instead.
+        :param pulumi.Input[str] security_group_id: ❗ The parent exoscale*security*group ID.
+        :param pulumi.Input[int] start_port: ❗ A `TCP`/`UDP` port range to match.
+        :param pulumi.Input[str] type: ❗ The traffic direction to match (`INGRESS` or `EGRESS`).
+        :param pulumi.Input[str] user_security_group: ❗ An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with `cidr`/`public_security_group`/`user_security_group_id`). Please use the `user_security_group_id` argument along the exoscale*security*group data source instead.
+        :param pulumi.Input[str] user_security_group_id: ❗ An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with `cidr`/`public_security_group`/`user_security_group)`).
         """
         if cidr is not None:
             pulumi.set(__self__, "cidr", cidr)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if end_port is not None:
             pulumi.set(__self__, "end_port", end_port)
@@ -318,166 +303,165 @@
         if user_security_group_id is not None:
             pulumi.set(__self__, "user_security_group_id", user_security_group_id)
 
     @property
     @pulumi.getter
     def cidr(self) -> Optional[pulumi.Input[str]]:
         """
-        An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR
-        notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with
-        `public_security_group`/`user_security_group`/`user_security_group_id`).
+        ❗ An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with `public_security_group`/`user_security_group`/`user_security_group_id`).
         """
         return pulumi.get(self, "cidr")
 
     @cidr.setter
     def cidr(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cidr", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        A free-form text describing the security group rule.
+        ❗ A free-form text describing the security group rule.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="endPort")
     def end_port(self) -> Optional[pulumi.Input[int]]:
         """
-        A `TCP`/`UDP` port range to match.
+        ❗ A `TCP`/`UDP` port range to match.
         """
         return pulumi.get(self, "end_port")
 
     @end_port.setter
     def end_port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "end_port", value)
 
     @property
     @pulumi.getter(name="icmpCode")
     def icmp_code(self) -> Optional[pulumi.Input[int]]:
         """
-        An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
+        ❗ An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
         """
         return pulumi.get(self, "icmp_code")
 
     @icmp_code.setter
     def icmp_code(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "icmp_code", value)
 
     @property
     @pulumi.getter(name="icmpType")
     def icmp_type(self) -> Optional[pulumi.Input[int]]:
         """
-        An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
+        ❗ An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
         """
         return pulumi.get(self, "icmp_type")
 
     @icmp_type.setter
     def icmp_type(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "icmp_type", value)
 
     @property
     @pulumi.getter
     def protocol(self) -> Optional[pulumi.Input[str]]:
         """
-        The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
+        ❗ The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
         """
         return pulumi.get(self, "protocol")
 
     @protocol.setter
     def protocol(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "protocol", value)
 
     @property
     @pulumi.getter(name="publicSecurityGroup")
     def public_security_group(self) -> Optional[pulumi.Input[str]]:
         """
-        An (`INGRESS`) source / (`EGRESS`) destination public security group name to match (conflicts with
-        `cidr`/`user_security_group`/`user_security_group_id`).
+        ❗ An (`INGRESS`) source / (`EGRESS`) destination public security group name to match (conflicts with `cidr`/`user_security_group`/`user_security_group_id`).
         """
         return pulumi.get(self, "public_security_group")
 
     @public_security_group.setter
     def public_security_group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "public_security_group", value)
 
     @property
     @pulumi.getter(name="securityGroup")
     def security_group(self) -> Optional[pulumi.Input[str]]:
         """
-        The parent security group name. Please use the `security_group_id` argument along the
-        [exoscale_security_group](../data-sources/security_group.md) data source instead.
+        ❗ The parent security group name. Please use the `security_group_id` argument along the exoscale*security*group data source instead.
         """
+        warnings.warn("""Deprecated in favor of `security_group_id`""", DeprecationWarning)
+        pulumi.log.warn("""security_group is deprecated: Deprecated in favor of `security_group_id`""")
+
         return pulumi.get(self, "security_group")
 
     @security_group.setter
     def security_group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_group", value)
 
     @property
     @pulumi.getter(name="securityGroupId")
     def security_group_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The parent [exoscale_security_group](./security_group.md) ID.
+        ❗ The parent exoscale*security*group ID.
         """
         return pulumi.get(self, "security_group_id")
 
     @security_group_id.setter
     def security_group_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_group_id", value)
 
     @property
     @pulumi.getter(name="startPort")
     def start_port(self) -> Optional[pulumi.Input[int]]:
         """
-        A `TCP`/`UDP` port range to match.
+        ❗ A `TCP`/`UDP` port range to match.
         """
         return pulumi.get(self, "start_port")
 
     @start_port.setter
     def start_port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "start_port", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        The traffic direction to match (`INGRESS` or `EGRESS`).
+        ❗ The traffic direction to match (`INGRESS` or `EGRESS`).
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter(name="userSecurityGroup")
     def user_security_group(self) -> Optional[pulumi.Input[str]]:
         """
-        An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with
-        `cidr`/`public_security_group`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
-        [exoscale_security_group](../data-sources/security_group.md) data source instead.
+        ❗ An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with `cidr`/`public_security_group`/`user_security_group_id`). Please use the `user_security_group_id` argument along the exoscale*security*group data source instead.
         """
+        warnings.warn("""Deprecated in favor of `user_security_group_id`""", DeprecationWarning)
+        pulumi.log.warn("""user_security_group is deprecated: Deprecated in favor of `user_security_group_id`""")
+
         return pulumi.get(self, "user_security_group")
 
     @user_security_group.setter
     def user_security_group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_security_group", value)
 
     @property
     @pulumi.getter(name="userSecurityGroupId")
     def user_security_group_id(self) -> Optional[pulumi.Input[str]]:
         """
-        An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with
-        `cidr`/`public_security_group`/`user_security_group)`).
+        ❗ An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with `cidr`/`public_security_group`/`user_security_group)`).
         """
         return pulumi.get(self, "user_security_group_id")
 
     @user_security_group_id.setter
     def user_security_group_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_security_group_id", value)
 
@@ -512,34 +496,27 @@
 
          exoscale_security_group_rule.my_security_group_rule \\
 
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6/9ecc6b8b-73d4-4211-8ced-f7f29bb79524
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] cidr: An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR
-               notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with
-               `public_security_group`/`user_security_group`/`user_security_group_id`).
-        :param pulumi.Input[str] description: A free-form text describing the security group rule.
-        :param pulumi.Input[int] end_port: A `TCP`/`UDP` port range to match.
-        :param pulumi.Input[int] icmp_code: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
-        :param pulumi.Input[int] icmp_type: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
-        :param pulumi.Input[str] protocol: The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
-        :param pulumi.Input[str] public_security_group: An (`INGRESS`) source / (`EGRESS`) destination public security group name to match (conflicts with
-               `cidr`/`user_security_group`/`user_security_group_id`).
-        :param pulumi.Input[str] security_group: The parent security group name. Please use the `security_group_id` argument along the
-               [exoscale_security_group](../data-sources/security_group.md) data source instead.
-        :param pulumi.Input[str] security_group_id: The parent [exoscale_security_group](./security_group.md) ID.
-        :param pulumi.Input[int] start_port: A `TCP`/`UDP` port range to match.
-        :param pulumi.Input[str] type: The traffic direction to match (`INGRESS` or `EGRESS`).
-        :param pulumi.Input[str] user_security_group: An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with
-               `cidr`/`public_security_group`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
-               [exoscale_security_group](../data-sources/security_group.md) data source instead.
-        :param pulumi.Input[str] user_security_group_id: An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with
-               `cidr`/`public_security_group`/`user_security_group)`).
+        :param pulumi.Input[str] cidr: ❗ An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with `public_security_group`/`user_security_group`/`user_security_group_id`).
+        :param pulumi.Input[str] description: ❗ A free-form text describing the security group rule.
+        :param pulumi.Input[int] end_port: ❗ A `TCP`/`UDP` port range to match.
+        :param pulumi.Input[int] icmp_code: ❗ An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
+        :param pulumi.Input[int] icmp_type: ❗ An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
+        :param pulumi.Input[str] protocol: ❗ The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
+        :param pulumi.Input[str] public_security_group: ❗ An (`INGRESS`) source / (`EGRESS`) destination public security group name to match (conflicts with `cidr`/`user_security_group`/`user_security_group_id`).
+        :param pulumi.Input[str] security_group: ❗ The parent security group name. Please use the `security_group_id` argument along the exoscale*security*group data source instead.
+        :param pulumi.Input[str] security_group_id: ❗ The parent exoscale*security*group ID.
+        :param pulumi.Input[int] start_port: ❗ A `TCP`/`UDP` port range to match.
+        :param pulumi.Input[str] type: ❗ The traffic direction to match (`INGRESS` or `EGRESS`).
+        :param pulumi.Input[str] user_security_group: ❗ An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with `cidr`/`public_security_group`/`user_security_group_id`). Please use the `user_security_group_id` argument along the exoscale*security*group data source instead.
+        :param pulumi.Input[str] user_security_group_id: ❗ An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with `cidr`/`public_security_group`/`user_security_group)`).
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: SecurityGroupRuleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -640,34 +617,27 @@
         """
         Get an existing SecurityGroupRule resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] cidr: An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR
-               notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with
-               `public_security_group`/`user_security_group`/`user_security_group_id`).
-        :param pulumi.Input[str] description: A free-form text describing the security group rule.
-        :param pulumi.Input[int] end_port: A `TCP`/`UDP` port range to match.
-        :param pulumi.Input[int] icmp_code: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
-        :param pulumi.Input[int] icmp_type: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
-        :param pulumi.Input[str] protocol: The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
-        :param pulumi.Input[str] public_security_group: An (`INGRESS`) source / (`EGRESS`) destination public security group name to match (conflicts with
-               `cidr`/`user_security_group`/`user_security_group_id`).
-        :param pulumi.Input[str] security_group: The parent security group name. Please use the `security_group_id` argument along the
-               [exoscale_security_group](../data-sources/security_group.md) data source instead.
-        :param pulumi.Input[str] security_group_id: The parent [exoscale_security_group](./security_group.md) ID.
-        :param pulumi.Input[int] start_port: A `TCP`/`UDP` port range to match.
-        :param pulumi.Input[str] type: The traffic direction to match (`INGRESS` or `EGRESS`).
-        :param pulumi.Input[str] user_security_group: An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with
-               `cidr`/`public_security_group`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
-               [exoscale_security_group](../data-sources/security_group.md) data source instead.
-        :param pulumi.Input[str] user_security_group_id: An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with
-               `cidr`/`public_security_group`/`user_security_group)`).
+        :param pulumi.Input[str] cidr: ❗ An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with `public_security_group`/`user_security_group`/`user_security_group_id`).
+        :param pulumi.Input[str] description: ❗ A free-form text describing the security group rule.
+        :param pulumi.Input[int] end_port: ❗ A `TCP`/`UDP` port range to match.
+        :param pulumi.Input[int] icmp_code: ❗ An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
+        :param pulumi.Input[int] icmp_type: ❗ An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
+        :param pulumi.Input[str] protocol: ❗ The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
+        :param pulumi.Input[str] public_security_group: ❗ An (`INGRESS`) source / (`EGRESS`) destination public security group name to match (conflicts with `cidr`/`user_security_group`/`user_security_group_id`).
+        :param pulumi.Input[str] security_group: ❗ The parent security group name. Please use the `security_group_id` argument along the exoscale*security*group data source instead.
+        :param pulumi.Input[str] security_group_id: ❗ The parent exoscale*security*group ID.
+        :param pulumi.Input[int] start_port: ❗ A `TCP`/`UDP` port range to match.
+        :param pulumi.Input[str] type: ❗ The traffic direction to match (`INGRESS` or `EGRESS`).
+        :param pulumi.Input[str] user_security_group: ❗ An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with `cidr`/`public_security_group`/`user_security_group_id`). Please use the `user_security_group_id` argument along the exoscale*security*group data source instead.
+        :param pulumi.Input[str] user_security_group_id: ❗ An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with `cidr`/`public_security_group`/`user_security_group)`).
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SecurityGroupRuleState.__new__(_SecurityGroupRuleState)
 
         __props__.__dict__["cidr"] = cidr
         __props__.__dict__["description"] = description
@@ -684,114 +654,113 @@
         __props__.__dict__["user_security_group_id"] = user_security_group_id
         return SecurityGroupRule(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def cidr(self) -> pulumi.Output[Optional[str]]:
         """
-        An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR
-        notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with
-        `public_security_group`/`user_security_group`/`user_security_group_id`).
+        ❗ An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with `public_security_group`/`user_security_group`/`user_security_group_id`).
         """
         return pulumi.get(self, "cidr")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
-        A free-form text describing the security group rule.
+        ❗ A free-form text describing the security group rule.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="endPort")
     def end_port(self) -> pulumi.Output[Optional[int]]:
         """
-        A `TCP`/`UDP` port range to match.
+        ❗ A `TCP`/`UDP` port range to match.
         """
         return pulumi.get(self, "end_port")
 
     @property
     @pulumi.getter(name="icmpCode")
     def icmp_code(self) -> pulumi.Output[Optional[int]]:
         """
-        An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
+        ❗ An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
         """
         return pulumi.get(self, "icmp_code")
 
     @property
     @pulumi.getter(name="icmpType")
     def icmp_type(self) -> pulumi.Output[Optional[int]]:
         """
-        An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
+        ❗ An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
         """
         return pulumi.get(self, "icmp_type")
 
     @property
     @pulumi.getter
     def protocol(self) -> pulumi.Output[Optional[str]]:
         """
-        The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
+        ❗ The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
         """
         return pulumi.get(self, "protocol")
 
     @property
     @pulumi.getter(name="publicSecurityGroup")
     def public_security_group(self) -> pulumi.Output[str]:
         """
-        An (`INGRESS`) source / (`EGRESS`) destination public security group name to match (conflicts with
-        `cidr`/`user_security_group`/`user_security_group_id`).
+        ❗ An (`INGRESS`) source / (`EGRESS`) destination public security group name to match (conflicts with `cidr`/`user_security_group`/`user_security_group_id`).
         """
         return pulumi.get(self, "public_security_group")
 
     @property
     @pulumi.getter(name="securityGroup")
     def security_group(self) -> pulumi.Output[str]:
         """
-        The parent security group name. Please use the `security_group_id` argument along the
-        [exoscale_security_group](../data-sources/security_group.md) data source instead.
+        ❗ The parent security group name. Please use the `security_group_id` argument along the exoscale*security*group data source instead.
         """
+        warnings.warn("""Deprecated in favor of `security_group_id`""", DeprecationWarning)
+        pulumi.log.warn("""security_group is deprecated: Deprecated in favor of `security_group_id`""")
+
         return pulumi.get(self, "security_group")
 
     @property
     @pulumi.getter(name="securityGroupId")
     def security_group_id(self) -> pulumi.Output[str]:
         """
-        The parent [exoscale_security_group](./security_group.md) ID.
+        ❗ The parent exoscale*security*group ID.
         """
         return pulumi.get(self, "security_group_id")
 
     @property
     @pulumi.getter(name="startPort")
     def start_port(self) -> pulumi.Output[Optional[int]]:
         """
-        A `TCP`/`UDP` port range to match.
+        ❗ A `TCP`/`UDP` port range to match.
         """
         return pulumi.get(self, "start_port")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
-        The traffic direction to match (`INGRESS` or `EGRESS`).
+        ❗ The traffic direction to match (`INGRESS` or `EGRESS`).
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="userSecurityGroup")
     def user_security_group(self) -> pulumi.Output[str]:
         """
-        An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with
-        `cidr`/`public_security_group`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
-        [exoscale_security_group](../data-sources/security_group.md) data source instead.
+        ❗ An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with `cidr`/`public_security_group`/`user_security_group_id`). Please use the `user_security_group_id` argument along the exoscale*security*group data source instead.
         """
+        warnings.warn("""Deprecated in favor of `user_security_group_id`""", DeprecationWarning)
+        pulumi.log.warn("""user_security_group is deprecated: Deprecated in favor of `user_security_group_id`""")
+
         return pulumi.get(self, "user_security_group")
 
     @property
     @pulumi.getter(name="userSecurityGroupId")
     def user_security_group_id(self) -> pulumi.Output[Optional[str]]:
         """
-        An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with
-        `cidr`/`public_security_group`/`user_security_group)`).
+        ❗ An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with `cidr`/`public_security_group`/`user_security_group)`).
         """
         return pulumi.get(self, "user_security_group_id")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/security_group_rules.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/security_group_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
                  ingresses: Optional[pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesIngressArgs']]]] = None,
                  security_group: Optional[pulumi.Input[str]] = None,
                  security_group_id: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a SecurityGroupRules resource.
         :param pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesEgressArgs']]] egresses: A security group rule definition (can be specified multiple times).
         :param pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesIngressArgs']]] ingresses: A security group rule definition (can be specified multiple times).
-        :param pulumi.Input[str] security_group: The security group (name) the rules apply to (conflicts with `security_group_id`).
-        :param pulumi.Input[str] security_group_id: The security group (ID) the rules apply to (conficts with `security_group)`.
+        :param pulumi.Input[str] security_group: ❗ The security group (name) the rules apply to (conflicts with `security_group_id`).
+        :param pulumi.Input[str] security_group_id: ❗ The security group (ID) the rules apply to (conficts with `security_group)`.
         """
         if egresses is not None:
             pulumi.set(__self__, "egresses", egresses)
         if ingresses is not None:
             pulumi.set(__self__, "ingresses", ingresses)
         if security_group is not None:
             pulumi.set(__self__, "security_group", security_group)
@@ -60,27 +60,27 @@
     def ingresses(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesIngressArgs']]]]):
         pulumi.set(self, "ingresses", value)
 
     @property
     @pulumi.getter(name="securityGroup")
     def security_group(self) -> Optional[pulumi.Input[str]]:
         """
-        The security group (name) the rules apply to (conflicts with `security_group_id`).
+        ❗ The security group (name) the rules apply to (conflicts with `security_group_id`).
         """
         return pulumi.get(self, "security_group")
 
     @security_group.setter
     def security_group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_group", value)
 
     @property
     @pulumi.getter(name="securityGroupId")
     def security_group_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The security group (ID) the rules apply to (conficts with `security_group)`.
+        ❗ The security group (ID) the rules apply to (conficts with `security_group)`.
         """
         return pulumi.get(self, "security_group_id")
 
     @security_group_id.setter
     def security_group_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_group_id", value)
 
@@ -92,16 +92,16 @@
                  ingresses: Optional[pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesIngressArgs']]]] = None,
                  security_group: Optional[pulumi.Input[str]] = None,
                  security_group_id: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SecurityGroupRules resources.
         :param pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesEgressArgs']]] egresses: A security group rule definition (can be specified multiple times).
         :param pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesIngressArgs']]] ingresses: A security group rule definition (can be specified multiple times).
-        :param pulumi.Input[str] security_group: The security group (name) the rules apply to (conflicts with `security_group_id`).
-        :param pulumi.Input[str] security_group_id: The security group (ID) the rules apply to (conficts with `security_group)`.
+        :param pulumi.Input[str] security_group: ❗ The security group (name) the rules apply to (conflicts with `security_group_id`).
+        :param pulumi.Input[str] security_group_id: ❗ The security group (ID) the rules apply to (conficts with `security_group)`.
         """
         if egresses is not None:
             pulumi.set(__self__, "egresses", egresses)
         if ingresses is not None:
             pulumi.set(__self__, "ingresses", ingresses)
         if security_group is not None:
             pulumi.set(__self__, "security_group", security_group)
@@ -132,27 +132,27 @@
     def ingresses(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SecurityGroupRulesIngressArgs']]]]):
         pulumi.set(self, "ingresses", value)
 
     @property
     @pulumi.getter(name="securityGroup")
     def security_group(self) -> Optional[pulumi.Input[str]]:
         """
-        The security group (name) the rules apply to (conflicts with `security_group_id`).
+        ❗ The security group (name) the rules apply to (conflicts with `security_group_id`).
         """
         return pulumi.get(self, "security_group")
 
     @security_group.setter
     def security_group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_group", value)
 
     @property
     @pulumi.getter(name="securityGroupId")
     def security_group_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The security group (ID) the rules apply to (conficts with `security_group)`.
+        ❗ The security group (ID) the rules apply to (conficts with `security_group)`.
         """
         return pulumi.get(self, "security_group_id")
 
     @security_group_id.setter
     def security_group_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_group_id", value)
 
@@ -170,16 +170,16 @@
         """
         !> **WARNING:** This resource is **DEPRECATED** and will be removed in the next major version. Please use the SecurityGroupRule instead (or refer to the ad-hoc migration guide).
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecurityGroupRulesEgressArgs']]]] egresses: A security group rule definition (can be specified multiple times).
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecurityGroupRulesIngressArgs']]]] ingresses: A security group rule definition (can be specified multiple times).
-        :param pulumi.Input[str] security_group: The security group (name) the rules apply to (conflicts with `security_group_id`).
-        :param pulumi.Input[str] security_group_id: The security group (ID) the rules apply to (conficts with `security_group)`.
+        :param pulumi.Input[str] security_group: ❗ The security group (name) the rules apply to (conflicts with `security_group_id`).
+        :param pulumi.Input[str] security_group_id: ❗ The security group (ID) the rules apply to (conficts with `security_group)`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[SecurityGroupRulesArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -237,16 +237,16 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecurityGroupRulesEgressArgs']]]] egresses: A security group rule definition (can be specified multiple times).
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecurityGroupRulesIngressArgs']]]] ingresses: A security group rule definition (can be specified multiple times).
-        :param pulumi.Input[str] security_group: The security group (name) the rules apply to (conflicts with `security_group_id`).
-        :param pulumi.Input[str] security_group_id: The security group (ID) the rules apply to (conficts with `security_group)`.
+        :param pulumi.Input[str] security_group: ❗ The security group (name) the rules apply to (conflicts with `security_group_id`).
+        :param pulumi.Input[str] security_group_id: ❗ The security group (ID) the rules apply to (conficts with `security_group)`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SecurityGroupRulesState.__new__(_SecurityGroupRulesState)
 
         __props__.__dict__["egresses"] = egresses
         __props__.__dict__["ingresses"] = ingresses
@@ -270,19 +270,19 @@
         """
         return pulumi.get(self, "ingresses")
 
     @property
     @pulumi.getter(name="securityGroup")
     def security_group(self) -> pulumi.Output[str]:
         """
-        The security group (name) the rules apply to (conflicts with `security_group_id`).
+        ❗ The security group (name) the rules apply to (conflicts with `security_group_id`).
         """
         return pulumi.get(self, "security_group")
 
     @property
     @pulumi.getter(name="securityGroupId")
     def security_group_id(self) -> pulumi.Output[str]:
         """
-        The security group (ID) the rules apply to (conficts with `security_group)`.
+        ❗ The security group (ID) the rules apply to (conficts with `security_group)`.
         """
         return pulumi.get(self, "security_group_id")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/sks_cluster.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/sks_cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,29 +26,25 @@
                  metrics_server: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  oidc: Optional[pulumi.Input['SKSClusterOidcArgs']] = None,
                  service_level: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a SKSCluster resource.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         :param pulumi.Input[bool] auto_upgrade: Enable automatic upgrading of the control plane version.
         :param pulumi.Input[str] cni: The CNI plugin that is to be used. Defaults to "calico".
         :param pulumi.Input[str] description: A free-form text describing the cluster.
-        :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the
-               control plane (boolean; default: `true`; may only be set at creation time).
+        :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the control plane (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane
-               (boolean; default: `true`; may only be set at creation time).
+        :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[str] name: The SKS cluster name.
-        :param pulumi.Input['SKSClusterOidcArgs'] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is
-               documented below.
+        :param pulumi.Input['SKSClusterOidcArgs'] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is documented below.
         :param pulumi.Input[str] service_level: The service level of the control plane (`pro` or `starter`; default: `pro`; may only be set at creation time).
-        :param pulumi.Input[str] version: The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for
-               reference; may only be set at creation time).
+        :param pulumi.Input[str] version: The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for reference; may only be set at creation time).
         """
         pulumi.set(__self__, "zone", zone)
         if addons is not None:
             warnings.warn("""This attribute has been replaced by `exoscale_ccm`/`metrics_server` attributes, it will be removed in a future release.""", DeprecationWarning)
             pulumi.log.warn("""addons is deprecated: This attribute has been replaced by `exoscale_ccm`/`metrics_server` attributes, it will be removed in a future release.""")
         if addons is not None:
             pulumi.set(__self__, "addons", addons)
@@ -73,25 +69,28 @@
         if version is not None:
             pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
     @property
     @pulumi.getter
     def addons(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        warnings.warn("""This attribute has been replaced by `exoscale_ccm`/`metrics_server` attributes, it will be removed in a future release.""", DeprecationWarning)
+        pulumi.log.warn("""addons is deprecated: This attribute has been replaced by `exoscale_ccm`/`metrics_server` attributes, it will be removed in a future release.""")
+
         return pulumi.get(self, "addons")
 
     @addons.setter
     def addons(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "addons", value)
 
     @property
@@ -130,16 +129,15 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter(name="exoscaleCcm")
     def exoscale_ccm(self) -> Optional[pulumi.Input[bool]]:
         """
-        Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the
-        control plane (boolean; default: `true`; may only be set at creation time).
+        Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the control plane (boolean; default: `true`; may only be set at creation time).
         """
         return pulumi.get(self, "exoscale_ccm")
 
     @exoscale_ccm.setter
     def exoscale_ccm(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "exoscale_ccm", value)
 
@@ -155,16 +153,15 @@
     def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter(name="metricsServer")
     def metrics_server(self) -> Optional[pulumi.Input[bool]]:
         """
-        Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane
-        (boolean; default: `true`; may only be set at creation time).
+        Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane (boolean; default: `true`; may only be set at creation time).
         """
         return pulumi.get(self, "metrics_server")
 
     @metrics_server.setter
     def metrics_server(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "metrics_server", value)
 
@@ -180,16 +177,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def oidc(self) -> Optional[pulumi.Input['SKSClusterOidcArgs']]:
         """
-        An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is
-        documented below.
+        An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is documented below.
         """
         return pulumi.get(self, "oidc")
 
     @oidc.setter
     def oidc(self, value: Optional[pulumi.Input['SKSClusterOidcArgs']]):
         pulumi.set(self, "oidc", value)
 
@@ -205,16 +201,15 @@
     def service_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_level", value)
 
     @property
     @pulumi.getter
     def version(self) -> Optional[pulumi.Input[str]]:
         """
-        The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for
-        reference; may only be set at creation time).
+        The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for reference; may only be set at creation time).
         """
         return pulumi.get(self, "version")
 
     @version.setter
     def version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "version", value)
 
@@ -239,37 +234,32 @@
                  oidc: Optional[pulumi.Input['SKSClusterOidcArgs']] = None,
                  service_level: Optional[pulumi.Input[str]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SKSCluster resources.
-        :param pulumi.Input[str] aggregation_ca: The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g.
-               `metrics-server`).
+        :param pulumi.Input[str] aggregation_ca: The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g. `metrics-server`).
         :param pulumi.Input[bool] auto_upgrade: Enable automatic upgrading of the control plane version.
         :param pulumi.Input[str] cni: The CNI plugin that is to be used. Defaults to "calico".
         :param pulumi.Input[str] control_plane_ca: The CA certificate (in PEM format) for TLS communications between control plane components.
         :param pulumi.Input[str] created_at: The cluster creation date.
         :param pulumi.Input[str] description: A free-form text describing the cluster.
         :param pulumi.Input[str] endpoint: The cluster API endpoint.
-        :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the
-               control plane (boolean; default: `true`; may only be set at creation time).
+        :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the control plane (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[str] kubelet_ca: The CA certificate (in PEM format) for TLS communications between kubelets and the control plane.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane
-               (boolean; default: `true`; may only be set at creation time).
+        :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[str] name: The SKS cluster name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] nodepools: The list of [exoscale_sks_nodepool](./sks_nodepool.md) (IDs) attached to the cluster.
-        :param pulumi.Input['SKSClusterOidcArgs'] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is
-               documented below.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] nodepools: The list of exoscale*sks*nodepool (IDs) attached to the cluster.
+        :param pulumi.Input['SKSClusterOidcArgs'] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is documented below.
         :param pulumi.Input[str] service_level: The service level of the control plane (`pro` or `starter`; default: `pro`; may only be set at creation time).
         :param pulumi.Input[str] state: The cluster state.
-        :param pulumi.Input[str] version: The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for
-               reference; may only be set at creation time).
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] version: The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for reference; may only be set at creation time).
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if addons is not None:
             warnings.warn("""This attribute has been replaced by `exoscale_ccm`/`metrics_server` attributes, it will be removed in a future release.""", DeprecationWarning)
             pulumi.log.warn("""addons is deprecated: This attribute has been replaced by `exoscale_ccm`/`metrics_server` attributes, it will be removed in a future release.""")
         if addons is not None:
             pulumi.set(__self__, "addons", addons)
         if aggregation_ca is not None:
@@ -308,26 +298,28 @@
             pulumi.set(__self__, "version", version)
         if zone is not None:
             pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter
     def addons(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        warnings.warn("""This attribute has been replaced by `exoscale_ccm`/`metrics_server` attributes, it will be removed in a future release.""", DeprecationWarning)
+        pulumi.log.warn("""addons is deprecated: This attribute has been replaced by `exoscale_ccm`/`metrics_server` attributes, it will be removed in a future release.""")
+
         return pulumi.get(self, "addons")
 
     @addons.setter
     def addons(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "addons", value)
 
     @property
     @pulumi.getter(name="aggregationCa")
     def aggregation_ca(self) -> Optional[pulumi.Input[str]]:
         """
-        The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g.
-        `metrics-server`).
+        The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g. `metrics-server`).
         """
         return pulumi.get(self, "aggregation_ca")
 
     @aggregation_ca.setter
     def aggregation_ca(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "aggregation_ca", value)
 
@@ -403,16 +395,15 @@
     def endpoint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "endpoint", value)
 
     @property
     @pulumi.getter(name="exoscaleCcm")
     def exoscale_ccm(self) -> Optional[pulumi.Input[bool]]:
         """
-        Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the
-        control plane (boolean; default: `true`; may only be set at creation time).
+        Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the control plane (boolean; default: `true`; may only be set at creation time).
         """
         return pulumi.get(self, "exoscale_ccm")
 
     @exoscale_ccm.setter
     def exoscale_ccm(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "exoscale_ccm", value)
 
@@ -440,16 +431,15 @@
     def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter(name="metricsServer")
     def metrics_server(self) -> Optional[pulumi.Input[bool]]:
         """
-        Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane
-        (boolean; default: `true`; may only be set at creation time).
+        Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane (boolean; default: `true`; may only be set at creation time).
         """
         return pulumi.get(self, "metrics_server")
 
     @metrics_server.setter
     def metrics_server(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "metrics_server", value)
 
@@ -465,28 +455,27 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def nodepools(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The list of [exoscale_sks_nodepool](./sks_nodepool.md) (IDs) attached to the cluster.
+        The list of exoscale*sks*nodepool (IDs) attached to the cluster.
         """
         return pulumi.get(self, "nodepools")
 
     @nodepools.setter
     def nodepools(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "nodepools", value)
 
     @property
     @pulumi.getter
     def oidc(self) -> Optional[pulumi.Input['SKSClusterOidcArgs']]:
         """
-        An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is
-        documented below.
+        An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is documented below.
         """
         return pulumi.get(self, "oidc")
 
     @oidc.setter
     def oidc(self, value: Optional[pulumi.Input['SKSClusterOidcArgs']]):
         pulumi.set(self, "oidc", value)
 
@@ -514,28 +503,27 @@
     def state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "state", value)
 
     @property
     @pulumi.getter
     def version(self) -> Optional[pulumi.Input[str]]:
         """
-        The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for
-        reference; may only be set at creation time).
+        The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for reference; may only be set at creation time).
         """
         return pulumi.get(self, "version")
 
     @version.setter
     def version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "version", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -572,26 +560,22 @@
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] auto_upgrade: Enable automatic upgrading of the control plane version.
         :param pulumi.Input[str] cni: The CNI plugin that is to be used. Defaults to "calico".
         :param pulumi.Input[str] description: A free-form text describing the cluster.
-        :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the
-               control plane (boolean; default: `true`; may only be set at creation time).
+        :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the control plane (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane
-               (boolean; default: `true`; may only be set at creation time).
+        :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[str] name: The SKS cluster name.
-        :param pulumi.Input[pulumi.InputType['SKSClusterOidcArgs']] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is
-               documented below.
+        :param pulumi.Input[pulumi.InputType['SKSClusterOidcArgs']] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is documented below.
         :param pulumi.Input[str] service_level: The service level of the control plane (`pro` or `starter`; default: `pro`; may only be set at creation time).
-        :param pulumi.Input[str] version: The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for
-               reference; may only be set at creation time).
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] version: The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for reference; may only be set at creation time).
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: SKSClusterArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -700,37 +684,32 @@
         """
         Get an existing SKSCluster resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] aggregation_ca: The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g.
-               `metrics-server`).
+        :param pulumi.Input[str] aggregation_ca: The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g. `metrics-server`).
         :param pulumi.Input[bool] auto_upgrade: Enable automatic upgrading of the control plane version.
         :param pulumi.Input[str] cni: The CNI plugin that is to be used. Defaults to "calico".
         :param pulumi.Input[str] control_plane_ca: The CA certificate (in PEM format) for TLS communications between control plane components.
         :param pulumi.Input[str] created_at: The cluster creation date.
         :param pulumi.Input[str] description: A free-form text describing the cluster.
         :param pulumi.Input[str] endpoint: The cluster API endpoint.
-        :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the
-               control plane (boolean; default: `true`; may only be set at creation time).
+        :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the control plane (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[str] kubelet_ca: The CA certificate (in PEM format) for TLS communications between kubelets and the control plane.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
-        :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane
-               (boolean; default: `true`; may only be set at creation time).
+        :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[str] name: The SKS cluster name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] nodepools: The list of [exoscale_sks_nodepool](./sks_nodepool.md) (IDs) attached to the cluster.
-        :param pulumi.Input[pulumi.InputType['SKSClusterOidcArgs']] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is
-               documented below.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] nodepools: The list of exoscale*sks*nodepool (IDs) attached to the cluster.
+        :param pulumi.Input[pulumi.InputType['SKSClusterOidcArgs']] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is documented below.
         :param pulumi.Input[str] service_level: The service level of the control plane (`pro` or `starter`; default: `pro`; may only be set at creation time).
         :param pulumi.Input[str] state: The cluster state.
-        :param pulumi.Input[str] version: The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for
-               reference; may only be set at creation time).
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] version: The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for reference; may only be set at creation time).
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SKSClusterState.__new__(_SKSClusterState)
 
         __props__.__dict__["addons"] = addons
         __props__.__dict__["aggregation_ca"] = aggregation_ca
@@ -752,22 +731,24 @@
         __props__.__dict__["version"] = version
         __props__.__dict__["zone"] = zone
         return SKSCluster(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def addons(self) -> pulumi.Output[Sequence[str]]:
+        warnings.warn("""This attribute has been replaced by `exoscale_ccm`/`metrics_server` attributes, it will be removed in a future release.""", DeprecationWarning)
+        pulumi.log.warn("""addons is deprecated: This attribute has been replaced by `exoscale_ccm`/`metrics_server` attributes, it will be removed in a future release.""")
+
         return pulumi.get(self, "addons")
 
     @property
     @pulumi.getter(name="aggregationCa")
     def aggregation_ca(self) -> pulumi.Output[str]:
         """
-        The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g.
-        `metrics-server`).
+        The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g. `metrics-server`).
         """
         return pulumi.get(self, "aggregation_ca")
 
     @property
     @pulumi.getter(name="autoUpgrade")
     def auto_upgrade(self) -> pulumi.Output[Optional[bool]]:
         """
@@ -815,16 +796,15 @@
         """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter(name="exoscaleCcm")
     def exoscale_ccm(self) -> pulumi.Output[Optional[bool]]:
         """
-        Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the
-        control plane (boolean; default: `true`; may only be set at creation time).
+        Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the control plane (boolean; default: `true`; may only be set at creation time).
         """
         return pulumi.get(self, "exoscale_ccm")
 
     @property
     @pulumi.getter(name="kubeletCa")
     def kubelet_ca(self) -> pulumi.Output[str]:
         """
@@ -840,16 +820,15 @@
         """
         return pulumi.get(self, "labels")
 
     @property
     @pulumi.getter(name="metricsServer")
     def metrics_server(self) -> pulumi.Output[Optional[bool]]:
         """
-        Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane
-        (boolean; default: `true`; may only be set at creation time).
+        Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane (boolean; default: `true`; may only be set at creation time).
         """
         return pulumi.get(self, "metrics_server")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
@@ -857,24 +836,23 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def nodepools(self) -> pulumi.Output[Sequence[str]]:
         """
-        The list of [exoscale_sks_nodepool](./sks_nodepool.md) (IDs) attached to the cluster.
+        The list of exoscale*sks*nodepool (IDs) attached to the cluster.
         """
         return pulumi.get(self, "nodepools")
 
     @property
     @pulumi.getter
     def oidc(self) -> pulumi.Output['outputs.SKSClusterOidc']:
         """
-        An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is
-        documented below.
+        An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is documented below.
         """
         return pulumi.get(self, "oidc")
 
     @property
     @pulumi.getter(name="serviceLevel")
     def service_level(self) -> pulumi.Output[Optional[str]]:
         """
@@ -890,20 +868,19 @@
         """
         return pulumi.get(self, "state")
 
     @property
     @pulumi.getter
     def version(self) -> pulumi.Output[str]:
         """
-        The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for
-        reference; may only be set at creation time).
+        The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for reference; may only be set at creation time).
         """
         return pulumi.get(self, "version")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/sks_kubeconfig.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/sks_kubeconfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,79 +18,75 @@
                  groups: pulumi.Input[Sequence[pulumi.Input[str]]],
                  user: pulumi.Input[str],
                  zone: pulumi.Input[str],
                  early_renewal_seconds: Optional[pulumi.Input[int]] = None,
                  ttl_seconds: Optional[pulumi.Input[float]] = None):
         """
         The set of arguments for constructing a SKSKubeconfig resource.
-        :param pulumi.Input[str] cluster_id: The parent [exoscale_sks_cluster](./sks_cluster.md) ID.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: Group names in the generated Kubeconfig. The certificate present in the Kubeconfig will have these roles set in the
-               Organization field.
-        :param pulumi.Input[str] user: User name in the generated Kubeconfig. The certificate present in the Kubeconfig will also have this name set for the CN
-               field.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] cluster_id: ❗ The parent exoscale*sks*cluster ID.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: ❗ Group names in the generated Kubeconfig. The certificate present in the Kubeconfig will have these roles set in the Organization field.
+        :param pulumi.Input[str] user: ❗ User name in the generated Kubeconfig. The certificate present in the Kubeconfig will also have this name set for the CN field.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         :param pulumi.Input[int] early_renewal_seconds: If set, the resource will consider the Kubeconfig to have expired the given number of seconds before its actual CA
                certificate or client certificate expiry time. This can be useful to deploy an updated Kubeconfig in advance of the
                expiration of its internal current certificate. Note however that the old certificate remains valid until its true
                expiration time since this resource does not (and cannot) support revocation. Also note this advance update can only
                take place if the Terraform configuration is applied during the early renewal period (seconds; default: 0).
-        :param pulumi.Input[float] ttl_seconds: The Time-to-Live of the Kubeconfig, after which it will expire / become invalid (seconds; default: 2592000 = 30 days).
+        :param pulumi.Input[float] ttl_seconds: ❗ The Time-to-Live of the Kubeconfig, after which it will expire / become invalid (seconds; default: 2592000 = 30 days).
         """
         pulumi.set(__self__, "cluster_id", cluster_id)
         pulumi.set(__self__, "groups", groups)
         pulumi.set(__self__, "user", user)
         pulumi.set(__self__, "zone", zone)
         if early_renewal_seconds is not None:
             pulumi.set(__self__, "early_renewal_seconds", early_renewal_seconds)
         if ttl_seconds is not None:
             pulumi.set(__self__, "ttl_seconds", ttl_seconds)
 
     @property
     @pulumi.getter(name="clusterId")
     def cluster_id(self) -> pulumi.Input[str]:
         """
-        The parent [exoscale_sks_cluster](./sks_cluster.md) ID.
+        ❗ The parent exoscale*sks*cluster ID.
         """
         return pulumi.get(self, "cluster_id")
 
     @cluster_id.setter
     def cluster_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "cluster_id", value)
 
     @property
     @pulumi.getter
     def groups(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        Group names in the generated Kubeconfig. The certificate present in the Kubeconfig will have these roles set in the
-        Organization field.
+        ❗ Group names in the generated Kubeconfig. The certificate present in the Kubeconfig will have these roles set in the Organization field.
         """
         return pulumi.get(self, "groups")
 
     @groups.setter
     def groups(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "groups", value)
 
     @property
     @pulumi.getter
     def user(self) -> pulumi.Input[str]:
         """
-        User name in the generated Kubeconfig. The certificate present in the Kubeconfig will also have this name set for the CN
-        field.
+        ❗ User name in the generated Kubeconfig. The certificate present in the Kubeconfig will also have this name set for the CN field.
         """
         return pulumi.get(self, "user")
 
     @user.setter
     def user(self, value: pulumi.Input[str]):
         pulumi.set(self, "user", value)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
@@ -110,15 +106,15 @@
     def early_renewal_seconds(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "early_renewal_seconds", value)
 
     @property
     @pulumi.getter(name="ttlSeconds")
     def ttl_seconds(self) -> Optional[pulumi.Input[float]]:
         """
-        The Time-to-Live of the Kubeconfig, after which it will expire / become invalid (seconds; default: 2592000 = 30 days).
+        ❗ The Time-to-Live of the Kubeconfig, after which it will expire / become invalid (seconds; default: 2592000 = 30 days).
         """
         return pulumi.get(self, "ttl_seconds")
 
     @ttl_seconds.setter
     def ttl_seconds(self, value: Optional[pulumi.Input[float]]):
         pulumi.set(self, "ttl_seconds", value)
 
@@ -132,27 +128,25 @@
                  kubeconfig: Optional[pulumi.Input[str]] = None,
                  ready_for_renewal: Optional[pulumi.Input[bool]] = None,
                  ttl_seconds: Optional[pulumi.Input[float]] = None,
                  user: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SKSKubeconfig resources.
-        :param pulumi.Input[str] cluster_id: The parent [exoscale_sks_cluster](./sks_cluster.md) ID.
+        :param pulumi.Input[str] cluster_id: ❗ The parent exoscale*sks*cluster ID.
         :param pulumi.Input[int] early_renewal_seconds: If set, the resource will consider the Kubeconfig to have expired the given number of seconds before its actual CA
                certificate or client certificate expiry time. This can be useful to deploy an updated Kubeconfig in advance of the
                expiration of its internal current certificate. Note however that the old certificate remains valid until its true
                expiration time since this resource does not (and cannot) support revocation. Also note this advance update can only
                take place if the Terraform configuration is applied during the early renewal period (seconds; default: 0).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: Group names in the generated Kubeconfig. The certificate present in the Kubeconfig will have these roles set in the
-               Organization field.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: ❗ Group names in the generated Kubeconfig. The certificate present in the Kubeconfig will have these roles set in the Organization field.
         :param pulumi.Input[str] kubeconfig: The generated Kubeconfig (YAML content).
-        :param pulumi.Input[float] ttl_seconds: The Time-to-Live of the Kubeconfig, after which it will expire / become invalid (seconds; default: 2592000 = 30 days).
-        :param pulumi.Input[str] user: User name in the generated Kubeconfig. The certificate present in the Kubeconfig will also have this name set for the CN
-               field.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[float] ttl_seconds: ❗ The Time-to-Live of the Kubeconfig, after which it will expire / become invalid (seconds; default: 2592000 = 30 days).
+        :param pulumi.Input[str] user: ❗ User name in the generated Kubeconfig. The certificate present in the Kubeconfig will also have this name set for the CN field.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if cluster_id is not None:
             pulumi.set(__self__, "cluster_id", cluster_id)
         if early_renewal_seconds is not None:
             pulumi.set(__self__, "early_renewal_seconds", early_renewal_seconds)
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
@@ -167,15 +161,15 @@
         if zone is not None:
             pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter(name="clusterId")
     def cluster_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The parent [exoscale_sks_cluster](./sks_cluster.md) ID.
+        ❗ The parent exoscale*sks*cluster ID.
         """
         return pulumi.get(self, "cluster_id")
 
     @cluster_id.setter
     def cluster_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cluster_id", value)
 
@@ -195,16 +189,15 @@
     def early_renewal_seconds(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "early_renewal_seconds", value)
 
     @property
     @pulumi.getter
     def groups(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Group names in the generated Kubeconfig. The certificate present in the Kubeconfig will have these roles set in the
-        Organization field.
+        ❗ Group names in the generated Kubeconfig. The certificate present in the Kubeconfig will have these roles set in the Organization field.
         """
         return pulumi.get(self, "groups")
 
     @groups.setter
     def groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "groups", value)
 
@@ -229,40 +222,39 @@
     def ready_for_renewal(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ready_for_renewal", value)
 
     @property
     @pulumi.getter(name="ttlSeconds")
     def ttl_seconds(self) -> Optional[pulumi.Input[float]]:
         """
-        The Time-to-Live of the Kubeconfig, after which it will expire / become invalid (seconds; default: 2592000 = 30 days).
+        ❗ The Time-to-Live of the Kubeconfig, after which it will expire / become invalid (seconds; default: 2592000 = 30 days).
         """
         return pulumi.get(self, "ttl_seconds")
 
     @ttl_seconds.setter
     def ttl_seconds(self, value: Optional[pulumi.Input[float]]):
         pulumi.set(self, "ttl_seconds", value)
 
     @property
     @pulumi.getter
     def user(self) -> Optional[pulumi.Input[str]]:
         """
-        User name in the generated Kubeconfig. The certificate present in the Kubeconfig will also have this name set for the CN
-        field.
+        ❗ User name in the generated Kubeconfig. The certificate present in the Kubeconfig will also have this name set for the CN field.
         """
         return pulumi.get(self, "user")
 
     @user.setter
     def user(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -279,26 +271,24 @@
                  user: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a SKSKubeconfig resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] cluster_id: The parent [exoscale_sks_cluster](./sks_cluster.md) ID.
+        :param pulumi.Input[str] cluster_id: ❗ The parent exoscale*sks*cluster ID.
         :param pulumi.Input[int] early_renewal_seconds: If set, the resource will consider the Kubeconfig to have expired the given number of seconds before its actual CA
                certificate or client certificate expiry time. This can be useful to deploy an updated Kubeconfig in advance of the
                expiration of its internal current certificate. Note however that the old certificate remains valid until its true
                expiration time since this resource does not (and cannot) support revocation. Also note this advance update can only
                take place if the Terraform configuration is applied during the early renewal period (seconds; default: 0).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: Group names in the generated Kubeconfig. The certificate present in the Kubeconfig will have these roles set in the
-               Organization field.
-        :param pulumi.Input[float] ttl_seconds: The Time-to-Live of the Kubeconfig, after which it will expire / become invalid (seconds; default: 2592000 = 30 days).
-        :param pulumi.Input[str] user: User name in the generated Kubeconfig. The certificate present in the Kubeconfig will also have this name set for the CN
-               field.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: ❗ Group names in the generated Kubeconfig. The certificate present in the Kubeconfig will have these roles set in the Organization field.
+        :param pulumi.Input[float] ttl_seconds: ❗ The Time-to-Live of the Kubeconfig, after which it will expire / become invalid (seconds; default: 2592000 = 30 days).
+        :param pulumi.Input[str] user: ❗ User name in the generated Kubeconfig. The certificate present in the Kubeconfig will also have this name set for the CN field.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: SKSKubeconfigArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -373,27 +363,25 @@
         """
         Get an existing SKSKubeconfig resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] cluster_id: The parent [exoscale_sks_cluster](./sks_cluster.md) ID.
+        :param pulumi.Input[str] cluster_id: ❗ The parent exoscale*sks*cluster ID.
         :param pulumi.Input[int] early_renewal_seconds: If set, the resource will consider the Kubeconfig to have expired the given number of seconds before its actual CA
                certificate or client certificate expiry time. This can be useful to deploy an updated Kubeconfig in advance of the
                expiration of its internal current certificate. Note however that the old certificate remains valid until its true
                expiration time since this resource does not (and cannot) support revocation. Also note this advance update can only
                take place if the Terraform configuration is applied during the early renewal period (seconds; default: 0).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: Group names in the generated Kubeconfig. The certificate present in the Kubeconfig will have these roles set in the
-               Organization field.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: ❗ Group names in the generated Kubeconfig. The certificate present in the Kubeconfig will have these roles set in the Organization field.
         :param pulumi.Input[str] kubeconfig: The generated Kubeconfig (YAML content).
-        :param pulumi.Input[float] ttl_seconds: The Time-to-Live of the Kubeconfig, after which it will expire / become invalid (seconds; default: 2592000 = 30 days).
-        :param pulumi.Input[str] user: User name in the generated Kubeconfig. The certificate present in the Kubeconfig will also have this name set for the CN
-               field.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[float] ttl_seconds: ❗ The Time-to-Live of the Kubeconfig, after which it will expire / become invalid (seconds; default: 2592000 = 30 days).
+        :param pulumi.Input[str] user: ❗ User name in the generated Kubeconfig. The certificate present in the Kubeconfig will also have this name set for the CN field.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SKSKubeconfigState.__new__(_SKSKubeconfigState)
 
         __props__.__dict__["cluster_id"] = cluster_id
         __props__.__dict__["early_renewal_seconds"] = early_renewal_seconds
@@ -405,15 +393,15 @@
         __props__.__dict__["zone"] = zone
         return SKSKubeconfig(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="clusterId")
     def cluster_id(self) -> pulumi.Output[str]:
         """
-        The parent [exoscale_sks_cluster](./sks_cluster.md) ID.
+        ❗ The parent exoscale*sks*cluster ID.
         """
         return pulumi.get(self, "cluster_id")
 
     @property
     @pulumi.getter(name="earlyRenewalSeconds")
     def early_renewal_seconds(self) -> pulumi.Output[Optional[int]]:
         """
@@ -425,16 +413,15 @@
         """
         return pulumi.get(self, "early_renewal_seconds")
 
     @property
     @pulumi.getter
     def groups(self) -> pulumi.Output[Sequence[str]]:
         """
-        Group names in the generated Kubeconfig. The certificate present in the Kubeconfig will have these roles set in the
-        Organization field.
+        ❗ Group names in the generated Kubeconfig. The certificate present in the Kubeconfig will have these roles set in the Organization field.
         """
         return pulumi.get(self, "groups")
 
     @property
     @pulumi.getter
     def kubeconfig(self) -> pulumi.Output[str]:
         """
@@ -447,28 +434,27 @@
     def ready_for_renewal(self) -> pulumi.Output[bool]:
         return pulumi.get(self, "ready_for_renewal")
 
     @property
     @pulumi.getter(name="ttlSeconds")
     def ttl_seconds(self) -> pulumi.Output[Optional[float]]:
         """
-        The Time-to-Live of the Kubeconfig, after which it will expire / become invalid (seconds; default: 2592000 = 30 days).
+        ❗ The Time-to-Live of the Kubeconfig, after which it will expire / become invalid (seconds; default: 2592000 = 30 days).
         """
         return pulumi.get(self, "ttl_seconds")
 
     @property
     @pulumi.getter
     def user(self) -> pulumi.Output[str]:
         """
-        User name in the generated Kubeconfig. The certificate present in the Kubeconfig will also have this name set for the CN
-        field.
+        ❗ User name in the generated Kubeconfig. The certificate present in the Kubeconfig will also have this name set for the CN field.
         """
         return pulumi.get(self, "user")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/sks_nodepool.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/sks_nodepool.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,29 +26,27 @@
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  private_network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  taints: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a SKSNodepool resource.
-        :param pulumi.Input[str] cluster_id: The parent [exoscale_sks_cluster](./sks_cluster.md) ID.
-        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
-               CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to be attached to the managed instances.
+        :param pulumi.Input[str] cluster_id: ❗ The parent exoscale*sks*cluster ID.
+        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of exoscale*anti*affinity_group (IDs) to be attached to the managed instances.
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[str] description: A free-form text describing the pool.
         :param pulumi.Input[int] disk_size: The managed instances disk size (GiB; default: `50`).
         :param pulumi.Input[str] instance_prefix: The string used to prefix the managed instances name (default `pool`).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The SKS node pool name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of [exoscale_private_network](./private_network.md) (IDs) to be attached to the managed instances.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_group.md) (IDs) to be attached to the managed instances.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] taints: A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/)
-               (`<value>:<effect>`).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of exoscale*private*network (IDs) to be attached to the managed instances.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of exoscale*security*group (IDs) to be attached to the managed instances.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] taints: A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/) (`<value>:<effect>`).
         """
         pulumi.set(__self__, "cluster_id", cluster_id)
         pulumi.set(__self__, "instance_type", instance_type)
         pulumi.set(__self__, "size", size)
         pulumi.set(__self__, "zone", zone)
         if anti_affinity_group_ids is not None:
             pulumi.set(__self__, "anti_affinity_group_ids", anti_affinity_group_ids)
@@ -71,28 +69,27 @@
         if taints is not None:
             pulumi.set(__self__, "taints", taints)
 
     @property
     @pulumi.getter(name="clusterId")
     def cluster_id(self) -> pulumi.Input[str]:
         """
-        The parent [exoscale_sks_cluster](./sks_cluster.md) ID.
+        ❗ The parent exoscale*sks*cluster ID.
         """
         return pulumi.get(self, "cluster_id")
 
     @cluster_id.setter
     def cluster_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "cluster_id", value)
 
     @property
     @pulumi.getter(name="instanceType")
     def instance_type(self) -> pulumi.Input[str]:
         """
-        The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
-        CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         """
         return pulumi.get(self, "instance_type")
 
     @instance_type.setter
     def instance_type(self, value: pulumi.Input[str]):
         pulumi.set(self, "instance_type", value)
 
@@ -105,27 +102,27 @@
     def size(self, value: pulumi.Input[int]):
         pulumi.set(self, "size", value)
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Input[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
     @property
     @pulumi.getter(name="antiAffinityGroupIds")
     def anti_affinity_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to be attached to the managed instances.
+        A list of exoscale*anti*affinity_group (IDs) to be attached to the managed instances.
         """
         return pulumi.get(self, "anti_affinity_group_ids")
 
     @anti_affinity_group_ids.setter
     def anti_affinity_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "anti_affinity_group_ids", value)
 
@@ -201,40 +198,39 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="privateNetworkIds")
     def private_network_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of [exoscale_private_network](./private_network.md) (IDs) to be attached to the managed instances.
+        A list of exoscale*private*network (IDs) to be attached to the managed instances.
         """
         return pulumi.get(self, "private_network_ids")
 
     @private_network_ids.setter
     def private_network_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "private_network_ids", value)
 
     @property
     @pulumi.getter(name="securityGroupIds")
     def security_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of [exoscale_security_group](./security_group.md) (IDs) to be attached to the managed instances.
+        A list of exoscale*security*group (IDs) to be attached to the managed instances.
         """
         return pulumi.get(self, "security_group_ids")
 
     @security_group_ids.setter
     def security_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "security_group_ids", value)
 
     @property
     @pulumi.getter
     def taints(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/)
-        (`<value>:<effect>`).
+        A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/) (`<value>:<effect>`).
         """
         return pulumi.get(self, "taints")
 
     @taints.setter
     def taints(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "taints", value)
 
@@ -259,34 +255,32 @@
                  state: Optional[pulumi.Input[str]] = None,
                  taints: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  template_id: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SKSNodepool resources.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to be attached to the managed instances.
-        :param pulumi.Input[str] cluster_id: The parent [exoscale_sks_cluster](./sks_cluster.md) ID.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of exoscale*anti*affinity_group (IDs) to be attached to the managed instances.
+        :param pulumi.Input[str] cluster_id: ❗ The parent exoscale*sks*cluster ID.
         :param pulumi.Input[str] created_at: The pool creation date.
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[str] description: A free-form text describing the pool.
         :param pulumi.Input[int] disk_size: The managed instances disk size (GiB; default: `50`).
-        :param pulumi.Input[str] instance_pool_id: The underlying [exoscale_instance_pool](./instance_pool.md) ID.
+        :param pulumi.Input[str] instance_pool_id: The underlying exoscale*instance*pool ID.
         :param pulumi.Input[str] instance_prefix: The string used to prefix the managed instances name (default `pool`).
-        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
-               CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The SKS node pool name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of [exoscale_private_network](./private_network.md) (IDs) to be attached to the managed instances.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_group.md) (IDs) to be attached to the managed instances.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of exoscale*private*network (IDs) to be attached to the managed instances.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of exoscale*security*group (IDs) to be attached to the managed instances.
         :param pulumi.Input[str] state: The current pool state.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] taints: A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/)
-               (`<value>:<effect>`).
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] taints: A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/) (`<value>:<effect>`).
         :param pulumi.Input[str] template_id: The managed instances template ID.
         :param pulumi.Input[str] version: The managed instances version.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if anti_affinity_group_ids is not None:
             pulumi.set(__self__, "anti_affinity_group_ids", anti_affinity_group_ids)
         if cluster_id is not None:
             pulumi.set(__self__, "cluster_id", cluster_id)
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
@@ -323,27 +317,27 @@
         if zone is not None:
             pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter(name="antiAffinityGroupIds")
     def anti_affinity_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to be attached to the managed instances.
+        A list of exoscale*anti*affinity_group (IDs) to be attached to the managed instances.
         """
         return pulumi.get(self, "anti_affinity_group_ids")
 
     @anti_affinity_group_ids.setter
     def anti_affinity_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "anti_affinity_group_ids", value)
 
     @property
     @pulumi.getter(name="clusterId")
     def cluster_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The parent [exoscale_sks_cluster](./sks_cluster.md) ID.
+        ❗ The parent exoscale*sks*cluster ID.
         """
         return pulumi.get(self, "cluster_id")
 
     @cluster_id.setter
     def cluster_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cluster_id", value)
 
@@ -395,15 +389,15 @@
     def disk_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "disk_size", value)
 
     @property
     @pulumi.getter(name="instancePoolId")
     def instance_pool_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The underlying [exoscale_instance_pool](./instance_pool.md) ID.
+        The underlying exoscale*instance*pool ID.
         """
         return pulumi.get(self, "instance_pool_id")
 
     @instance_pool_id.setter
     def instance_pool_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "instance_pool_id", value)
 
@@ -419,16 +413,15 @@
     def instance_prefix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "instance_prefix", value)
 
     @property
     @pulumi.getter(name="instanceType")
     def instance_type(self) -> Optional[pulumi.Input[str]]:
         """
-        The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
-        CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         """
         return pulumi.get(self, "instance_type")
 
     @instance_type.setter
     def instance_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "instance_type", value)
 
@@ -456,27 +449,27 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="privateNetworkIds")
     def private_network_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of [exoscale_private_network](./private_network.md) (IDs) to be attached to the managed instances.
+        A list of exoscale*private*network (IDs) to be attached to the managed instances.
         """
         return pulumi.get(self, "private_network_ids")
 
     @private_network_ids.setter
     def private_network_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "private_network_ids", value)
 
     @property
     @pulumi.getter(name="securityGroupIds")
     def security_group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of [exoscale_security_group](./security_group.md) (IDs) to be attached to the managed instances.
+        A list of exoscale*security*group (IDs) to be attached to the managed instances.
         """
         return pulumi.get(self, "security_group_ids")
 
     @security_group_ids.setter
     def security_group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "security_group_ids", value)
 
@@ -501,16 +494,15 @@
     def state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "state", value)
 
     @property
     @pulumi.getter
     def taints(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/)
-        (`<value>:<effect>`).
+        A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/) (`<value>:<effect>`).
         """
         return pulumi.get(self, "taints")
 
     @taints.setter
     def taints(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "taints", value)
 
@@ -538,15 +530,15 @@
     def version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "version", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -582,29 +574,27 @@
 
          exoscale_sks_nodepool.my_sks_nodepool \\
 
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6/9ecc6b8b-73d4-4211-8ced-f7f29bb79524@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to be attached to the managed instances.
-        :param pulumi.Input[str] cluster_id: The parent [exoscale_sks_cluster](./sks_cluster.md) ID.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of exoscale*anti*affinity_group (IDs) to be attached to the managed instances.
+        :param pulumi.Input[str] cluster_id: ❗ The parent exoscale*sks*cluster ID.
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[str] description: A free-form text describing the pool.
         :param pulumi.Input[int] disk_size: The managed instances disk size (GiB; default: `50`).
         :param pulumi.Input[str] instance_prefix: The string used to prefix the managed instances name (default `pool`).
-        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
-               CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The SKS node pool name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of [exoscale_private_network](./private_network.md) (IDs) to be attached to the managed instances.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_group.md) (IDs) to be attached to the managed instances.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] taints: A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/)
-               (`<value>:<effect>`).
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of exoscale*private*network (IDs) to be attached to the managed instances.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of exoscale*security*group (IDs) to be attached to the managed instances.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] taints: A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/) (`<value>:<effect>`).
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: SKSNodepoolArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -718,34 +708,32 @@
         """
         Get an existing SKSNodepool resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to be attached to the managed instances.
-        :param pulumi.Input[str] cluster_id: The parent [exoscale_sks_cluster](./sks_cluster.md) ID.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of exoscale*anti*affinity_group (IDs) to be attached to the managed instances.
+        :param pulumi.Input[str] cluster_id: ❗ The parent exoscale*sks*cluster ID.
         :param pulumi.Input[str] created_at: The pool creation date.
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[str] description: A free-form text describing the pool.
         :param pulumi.Input[int] disk_size: The managed instances disk size (GiB; default: `50`).
-        :param pulumi.Input[str] instance_pool_id: The underlying [exoscale_instance_pool](./instance_pool.md) ID.
+        :param pulumi.Input[str] instance_pool_id: The underlying exoscale*instance*pool ID.
         :param pulumi.Input[str] instance_prefix: The string used to prefix the managed instances name (default `pool`).
-        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
-               CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        :param pulumi.Input[str] instance_type: The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The SKS node pool name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of [exoscale_private_network](./private_network.md) (IDs) to be attached to the managed instances.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_group.md) (IDs) to be attached to the managed instances.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of exoscale*private*network (IDs) to be attached to the managed instances.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of exoscale*security*group (IDs) to be attached to the managed instances.
         :param pulumi.Input[str] state: The current pool state.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] taints: A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/)
-               (`<value>:<effect>`).
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] taints: A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/) (`<value>:<effect>`).
         :param pulumi.Input[str] template_id: The managed instances template ID.
         :param pulumi.Input[str] version: The managed instances version.
-        :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SKSNodepoolState.__new__(_SKSNodepoolState)
 
         __props__.__dict__["anti_affinity_group_ids"] = anti_affinity_group_ids
         __props__.__dict__["cluster_id"] = cluster_id
@@ -768,23 +756,23 @@
         __props__.__dict__["zone"] = zone
         return SKSNodepool(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="antiAffinityGroupIds")
     def anti_affinity_group_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of [exoscale_anti_affinity_group](./anti_affinity_group.md) (IDs) to be attached to the managed instances.
+        A list of exoscale*anti*affinity_group (IDs) to be attached to the managed instances.
         """
         return pulumi.get(self, "anti_affinity_group_ids")
 
     @property
     @pulumi.getter(name="clusterId")
     def cluster_id(self) -> pulumi.Output[str]:
         """
-        The parent [exoscale_sks_cluster](./sks_cluster.md) ID.
+        ❗ The parent exoscale*sks*cluster ID.
         """
         return pulumi.get(self, "cluster_id")
 
     @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> pulumi.Output[str]:
         """
@@ -816,15 +804,15 @@
         """
         return pulumi.get(self, "disk_size")
 
     @property
     @pulumi.getter(name="instancePoolId")
     def instance_pool_id(self) -> pulumi.Output[str]:
         """
-        The underlying [exoscale_instance_pool](./instance_pool.md) ID.
+        The underlying exoscale*instance*pool ID.
         """
         return pulumi.get(self, "instance_pool_id")
 
     @property
     @pulumi.getter(name="instancePrefix")
     def instance_prefix(self) -> pulumi.Output[Optional[str]]:
         """
@@ -832,16 +820,15 @@
         """
         return pulumi.get(self, "instance_prefix")
 
     @property
     @pulumi.getter(name="instanceType")
     def instance_type(self) -> pulumi.Output[str]:
         """
-        The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale
-        CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
+        The managed compute instances type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo compute instance-type list` - for the list of available types).
         """
         return pulumi.get(self, "instance_type")
 
     @property
     @pulumi.getter
     def labels(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
@@ -857,23 +844,23 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="privateNetworkIds")
     def private_network_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of [exoscale_private_network](./private_network.md) (IDs) to be attached to the managed instances.
+        A list of exoscale*private*network (IDs) to be attached to the managed instances.
         """
         return pulumi.get(self, "private_network_ids")
 
     @property
     @pulumi.getter(name="securityGroupIds")
     def security_group_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of [exoscale_security_group](./security_group.md) (IDs) to be attached to the managed instances.
+        A list of exoscale*security*group (IDs) to be attached to the managed instances.
         """
         return pulumi.get(self, "security_group_ids")
 
     @property
     @pulumi.getter
     def size(self) -> pulumi.Output[int]:
         return pulumi.get(self, "size")
@@ -886,16 +873,15 @@
         """
         return pulumi.get(self, "state")
 
     @property
     @pulumi.getter
     def taints(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/)
-        (`<value>:<effect>`).
+        A map of key/value Kubernetes [taints](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/) (`<value>:<effect>`).
         """
         return pulumi.get(self, "taints")
 
     @property
     @pulumi.getter(name="templateId")
     def template_id(self) -> pulumi.Output[str]:
         """
@@ -911,11 +897,11 @@
         """
         return pulumi.get(self, "version")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
-        The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
+        ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/ssh_key.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/ssh_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,39 +14,39 @@
 @pulumi.input_type
 class SSHKeyArgs:
     def __init__(__self__, *,
                  name: Optional[pulumi.Input[str]] = None,
                  public_key: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a SSHKey resource.
-        :param pulumi.Input[str] name: The SSH key name.
-        :param pulumi.Input[str] public_key: The SSH *public* key that will be authorized in compute instances.
+        :param pulumi.Input[str] name: ❗ The SSH key name.
+        :param pulumi.Input[str] public_key: ❗ The SSH *public* key that will be authorized in compute instances.
         """
         if name is not None:
             pulumi.set(__self__, "name", name)
         if public_key is not None:
             pulumi.set(__self__, "public_key", public_key)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The SSH key name.
+        ❗ The SSH key name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="publicKey")
     def public_key(self) -> Optional[pulumi.Input[str]]:
         """
-        The SSH *public* key that will be authorized in compute instances.
+        ❗ The SSH *public* key that will be authorized in compute instances.
         """
         return pulumi.get(self, "public_key")
 
     @public_key.setter
     def public_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "public_key", value)
 
@@ -56,16 +56,16 @@
     def __init__(__self__, *,
                  fingerprint: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  public_key: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SSHKey resources.
         :param pulumi.Input[str] fingerprint: The SSH key unique identifier.
-        :param pulumi.Input[str] name: The SSH key name.
-        :param pulumi.Input[str] public_key: The SSH *public* key that will be authorized in compute instances.
+        :param pulumi.Input[str] name: ❗ The SSH key name.
+        :param pulumi.Input[str] public_key: ❗ The SSH *public* key that will be authorized in compute instances.
         """
         if fingerprint is not None:
             pulumi.set(__self__, "fingerprint", fingerprint)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if public_key is not None:
             pulumi.set(__self__, "public_key", public_key)
@@ -82,27 +82,27 @@
     def fingerprint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "fingerprint", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The SSH key name.
+        ❗ The SSH key name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="publicKey")
     def public_key(self) -> Optional[pulumi.Input[str]]:
         """
-        The SSH *public* key that will be authorized in compute instances.
+        ❗ The SSH *public* key that will be authorized in compute instances.
         """
         return pulumi.get(self, "public_key")
 
     @public_key.setter
     def public_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "public_key", value)
 
@@ -126,16 +126,16 @@
 
          exoscale_ssh_key.my_ssh_key \\
 
          my-ssh-key
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] name: The SSH key name.
-        :param pulumi.Input[str] public_key: The SSH *public* key that will be authorized in compute instances.
+        :param pulumi.Input[str] name: ❗ The SSH key name.
+        :param pulumi.Input[str] public_key: ❗ The SSH *public* key that will be authorized in compute instances.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[SSHKeyArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -198,16 +198,16 @@
         Get an existing SSHKey resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] fingerprint: The SSH key unique identifier.
-        :param pulumi.Input[str] name: The SSH key name.
-        :param pulumi.Input[str] public_key: The SSH *public* key that will be authorized in compute instances.
+        :param pulumi.Input[str] name: ❗ The SSH key name.
+        :param pulumi.Input[str] public_key: ❗ The SSH *public* key that will be authorized in compute instances.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SSHKeyState.__new__(_SSHKeyState)
 
         __props__.__dict__["fingerprint"] = fingerprint
         __props__.__dict__["name"] = name
@@ -222,19 +222,19 @@
         """
         return pulumi.get(self, "fingerprint")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The SSH key name.
+        ❗ The SSH key name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="publicKey")
     def public_key(self) -> pulumi.Output[str]:
         """
-        The SSH *public* key that will be authorized in compute instances.
+        ❗ The SSH *public* key that will be authorized in compute instances.
         """
         return pulumi.get(self, "public_key")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/ssh_keypair.py` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale/ssh_keypair.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,41 +14,39 @@
 @pulumi.input_type
 class SSHKeypairArgs:
     def __init__(__self__, *,
                  name: Optional[pulumi.Input[str]] = None,
                  public_key: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a SSHKeypair resource.
-        :param pulumi.Input[str] name: The SSH keypair name.
-        :param pulumi.Input[str] public_key: A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the
-               *private* key) is generated and saved locally (see the `private_key` attribute).
+        :param pulumi.Input[str] name: ❗ The SSH keypair name.
+        :param pulumi.Input[str] public_key: ❗ A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the *private* key) is generated and saved locally (see the `private_key` attribute).
         """
         if name is not None:
             pulumi.set(__self__, "name", name)
         if public_key is not None:
             pulumi.set(__self__, "public_key", public_key)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The SSH keypair name.
+        ❗ The SSH keypair name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="publicKey")
     def public_key(self) -> Optional[pulumi.Input[str]]:
         """
-        A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the
-        *private* key) is generated and saved locally (see the `private_key` attribute).
+        ❗ A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the *private* key) is generated and saved locally (see the `private_key` attribute).
         """
         return pulumi.get(self, "public_key")
 
     @public_key.setter
     def public_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "public_key", value)
 
@@ -59,18 +57,17 @@
                  fingerprint: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  private_key: Optional[pulumi.Input[str]] = None,
                  public_key: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SSHKeypair resources.
         :param pulumi.Input[str] fingerprint: The SSH keypair unique identifier.
-        :param pulumi.Input[str] name: The SSH keypair name.
+        :param pulumi.Input[str] name: ❗ The SSH keypair name.
         :param pulumi.Input[str] private_key: The SSH *private* key generated if no public key was provided.
-        :param pulumi.Input[str] public_key: A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the
-               *private* key) is generated and saved locally (see the `private_key` attribute).
+        :param pulumi.Input[str] public_key: ❗ A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the *private* key) is generated and saved locally (see the `private_key` attribute).
         """
         if fingerprint is not None:
             pulumi.set(__self__, "fingerprint", fingerprint)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if private_key is not None:
             pulumi.set(__self__, "private_key", private_key)
@@ -89,15 +86,15 @@
     def fingerprint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "fingerprint", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The SSH keypair name.
+        ❗ The SSH keypair name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -113,16 +110,15 @@
     def private_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "private_key", value)
 
     @property
     @pulumi.getter(name="publicKey")
     def public_key(self) -> Optional[pulumi.Input[str]]:
         """
-        A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the
-        *private* key) is generated and saved locally (see the `private_key` attribute).
+        ❗ A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the *private* key) is generated and saved locally (see the `private_key` attribute).
         """
         return pulumi.get(self, "public_key")
 
     @public_key.setter
     def public_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "public_key", value)
 
@@ -135,17 +131,16 @@
                  name: Optional[pulumi.Input[str]] = None,
                  public_key: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a SSHKeypair resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] name: The SSH keypair name.
-        :param pulumi.Input[str] public_key: A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the
-               *private* key) is generated and saved locally (see the `private_key` attribute).
+        :param pulumi.Input[str] name: ❗ The SSH keypair name.
+        :param pulumi.Input[str] public_key: ❗ A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the *private* key) is generated and saved locally (see the `private_key` attribute).
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[SSHKeypairArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -201,18 +196,17 @@
         Get an existing SSHKeypair resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] fingerprint: The SSH keypair unique identifier.
-        :param pulumi.Input[str] name: The SSH keypair name.
+        :param pulumi.Input[str] name: ❗ The SSH keypair name.
         :param pulumi.Input[str] private_key: The SSH *private* key generated if no public key was provided.
-        :param pulumi.Input[str] public_key: A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the
-               *private* key) is generated and saved locally (see the `private_key` attribute).
+        :param pulumi.Input[str] public_key: ❗ A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the *private* key) is generated and saved locally (see the `private_key` attribute).
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SSHKeypairState.__new__(_SSHKeypairState)
 
         __props__.__dict__["fingerprint"] = fingerprint
         __props__.__dict__["name"] = name
@@ -228,15 +222,15 @@
         """
         return pulumi.get(self, "fingerprint")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The SSH keypair name.
+        ❗ The SSH keypair name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="privateKey")
     def private_key(self) -> pulumi.Output[str]:
         """
@@ -244,12 +238,11 @@
         """
         return pulumi.get(self, "private_key")
 
     @property
     @pulumi.getter(name="publicKey")
     def public_key(self) -> pulumi.Output[Optional[str]]:
         """
-        A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the
-        *private* key) is generated and saved locally (see the `private_key` attribute).
+        ❗ A SSH *public* key that will be authorized in compute instances. If not provided, an SSH keypair (including the *private* key) is generated and saved locally (see the `private_key` attribute).
         """
         return pulumi.get(self, "public_key")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale.egg-info/PKG-INFO` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-exoscale
-Version: 0.49.0
+Version: 0.50.0
 Summary: A Pulumi package for creating and managing exoscale cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-exoscale
 Keywords: pulumi exoscale category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale.egg-info/SOURCES.txt` & `pulumiverse_exoscale-0.50.0/pulumiverse_exoscale.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.49.0/setup.py` & `pulumiverse_exoscale-0.50.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.49.0"
-PLUGIN_VERSION = "0.49.0"
+VERSION = "0.50.0"
+PLUGIN_VERSION = "0.50.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'exoscale', PLUGIN_VERSION, '--server', 'github://api.github.com/pulumiverse/pulumi-exoscale'])
         except OSError as error:
```

