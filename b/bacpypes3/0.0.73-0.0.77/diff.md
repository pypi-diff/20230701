# Comparing `tmp/bacpypes3-0.0.73.tar.gz` & `tmp/bacpypes3-0.0.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacpypes3-0.0.73.tar", last modified: Wed May 10 06:11:40 2023, max compression
+gzip compressed data, was "bacpypes3-0.0.77.tar", last modified: Sat Jul  1 17:58:49 2023, max compression
```

## Comparing `bacpypes3-0.0.73.tar` & `bacpypes3-0.0.77.tar`

### file list

```diff
@@ -1,121 +1,126 @@
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.109958 bacpypes3-0.0.73/
--rw-rw-r--   0 joel      (1000) joel      (1000)      666 2023-05-10 06:11:40.109958 bacpypes3-0.0.73/PKG-INFO
--rw-rw-r--   0 joel      (1000) joel      (1000)      346 2023-03-09 18:20:30.000000 bacpypes3-0.0.73/README.md
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.093958 bacpypes3-0.0.73/bacpypes3/
--rw-rw-r--   0 joel      (1000) joel      (1000)     1370 2023-05-10 06:05:09.000000 bacpypes3-0.0.73/bacpypes3/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    23678 2023-04-21 19:39:28.000000 bacpypes3-0.0.73/bacpypes3/__main__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    56648 2023-01-24 05:27:28.000000 bacpypes3-0.0.73/bacpypes3/apdu.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    32984 2023-04-03 19:01:08.000000 bacpypes3-0.0.73/bacpypes3/app.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    65777 2023-04-04 12:53:18.000000 bacpypes3-0.0.73/bacpypes3/appservice.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    21553 2023-03-22 18:04:43.000000 bacpypes3-0.0.73/bacpypes3/argparse.py
--rw-rw-r--   0 joel      (1000) joel      (1000)   109678 2023-05-10 06:07:50.000000 bacpypes3-0.0.73/bacpypes3/basetypes.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    16150 2023-04-03 15:32:38.000000 bacpypes3-0.0.73/bacpypes3/cmd.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     7934 2022-11-21 19:40:26.000000 bacpypes3-0.0.73/bacpypes3/comm.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     7128 2023-01-24 05:27:28.000000 bacpypes3-0.0.73/bacpypes3/console.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    64295 2023-04-07 19:15:02.000000 bacpypes3-0.0.73/bacpypes3/constructeddata.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    10883 2023-01-24 13:27:43.000000 bacpypes3-0.0.73/bacpypes3/debugging.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     9685 2023-02-08 13:29:16.000000 bacpypes3-0.0.73/bacpypes3/errors.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.097958 bacpypes3-0.0.73/bacpypes3/ipv4/
--rw-rw-r--   0 joel      (1000) joel      (1000)     9099 2023-01-09 14:29:42.000000 bacpypes3-0.0.73/bacpypes3/ipv4/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8238 2023-04-22 03:23:44.000000 bacpypes3-0.0.73/bacpypes3/ipv4/app.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    25882 2023-04-21 19:42:07.000000 bacpypes3-0.0.73/bacpypes3/ipv4/bvll.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4119 2023-02-12 01:55:32.000000 bacpypes3-0.0.73/bacpypes3/ipv4/link.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    61699 2023-04-21 19:25:10.000000 bacpypes3-0.0.73/bacpypes3/ipv4/service.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.097958 bacpypes3-0.0.73/bacpypes3/ipv6/
--rw-rw-r--   0 joel      (1000) joel      (1000)     6298 2023-01-09 14:29:42.000000 bacpypes3-0.0.73/bacpypes3/ipv6/__init__.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    32041 2023-01-24 14:48:16.000000 bacpypes3-0.0.73/bacpypes3/ipv6/bvll.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    57488 2023-02-01 12:39:44.000000 bacpypes3-0.0.73/bacpypes3/ipv6/service.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.097958 bacpypes3-0.0.73/bacpypes3/json/
--rw-rw-r--   0 joel      (1000) joel      (1000)      102 2023-01-24 13:54:53.000000 bacpypes3-0.0.73/bacpypes3/json/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      132 2022-09-06 15:15:46.000000 bacpypes3-0.0.73/bacpypes3/json/__main__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    16743 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/bacpypes3/json/util.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.097958 bacpypes3-0.0.73/bacpypes3/lib/
--rw-rw-r--   0 joel      (1000) joel      (1000)       41 2023-01-24 05:27:28.000000 bacpypes3-0.0.73/bacpypes3/lib/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    10085 2021-08-04 12:18:07.000000 bacpypes3-0.0.73/bacpypes3/lib/batchread.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.097958 bacpypes3-0.0.73/bacpypes3/local/
--rw-rw-r--   0 joel      (1000) joel      (1000)      381 2023-02-06 04:19:11.000000 bacpypes3-0.0.73/bacpypes3/local/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     5393 2023-01-03 14:48:04.000000 bacpypes3-0.0.73/bacpypes3/local/cmd.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    18792 2022-11-24 07:17:25.000000 bacpypes3-0.0.73/bacpypes3/local/cov.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     5769 2023-01-24 13:31:42.000000 bacpypes3-0.0.73/bacpypes3/local/device.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4822 2023-02-06 04:19:11.000000 bacpypes3-0.0.73/bacpypes3/local/networkport.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     9811 2022-11-21 19:38:08.000000 bacpypes3-0.0.73/bacpypes3/local/object.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     1046 2023-01-03 14:48:04.000000 bacpypes3-0.0.73/bacpypes3/local/oos.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    24830 2023-02-06 04:19:11.000000 bacpypes3-0.0.73/bacpypes3/local/schedule.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    76370 2023-04-14 14:22:25.000000 bacpypes3-0.0.73/bacpypes3/netservice.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    28240 2023-01-24 05:27:28.000000 bacpypes3-0.0.73/bacpypes3/npdu.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    93858 2023-05-10 06:05:09.000000 bacpypes3-0.0.73/bacpypes3/object.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    64688 2023-02-15 17:04:37.000000 bacpypes3-0.0.73/bacpypes3/pdu.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    80966 2023-02-17 06:25:03.000000 bacpypes3-0.0.73/bacpypes3/primitivedata.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.101958 bacpypes3-0.0.73/bacpypes3/rdf/
--rw-rw-r--   0 joel      (1000) joel      (1000)      353 2023-01-24 13:54:37.000000 bacpypes3-0.0.73/bacpypes3/rdf/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      130 2022-08-22 23:43:00.000000 bacpypes3-0.0.73/bacpypes3/rdf/__main__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    10595 2023-05-04 14:15:16.000000 bacpypes3-0.0.73/bacpypes3/rdf/core.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    19634 2023-01-27 13:19:10.000000 bacpypes3-0.0.73/bacpypes3/rdf/util.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.101958 bacpypes3-0.0.73/bacpypes3/sc/
--rw-rw-r--   0 joel      (1000) joel      (1000)       65 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/bacpypes3/sc/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    33859 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/bacpypes3/sc/bvll.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    18081 2023-02-27 03:52:18.000000 bacpypes3-0.0.73/bacpypes3/sc/service.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.101958 bacpypes3-0.0.73/bacpypes3/service/
--rw-rw-r--   0 joel      (1000) joel      (1000)       78 2023-01-24 13:55:00.000000 bacpypes3-0.0.73/bacpypes3/service/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    22512 2023-04-03 19:06:43.000000 bacpypes3-0.0.73/bacpypes3/service/cov.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    22741 2023-04-04 12:42:09.000000 bacpypes3-0.0.73/bacpypes3/service/device.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    31277 2023-04-03 19:49:50.000000 bacpypes3-0.0.73/bacpypes3/service/object.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3884 2023-01-27 13:49:14.000000 bacpypes3-0.0.73/bacpypes3/settings.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.101958 bacpypes3-0.0.73/bacpypes3/vlan/
--rw-rw-r--   0 joel      (1000) joel      (1000)    10230 2023-01-24 05:27:28.000000 bacpypes3-0.0.73/bacpypes3/vlan/__init__.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.093958 bacpypes3-0.0.73/bacpypes3.egg-info/
--rw-rw-r--   0 joel      (1000) joel      (1000)      666 2023-05-10 06:11:40.000000 bacpypes3-0.0.73/bacpypes3.egg-info/PKG-INFO
--rw-rw-r--   0 joel      (1000) joel      (1000)     2924 2023-05-10 06:11:40.000000 bacpypes3-0.0.73/bacpypes3.egg-info/SOURCES.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)        1 2023-05-10 06:11:40.000000 bacpypes3-0.0.73/bacpypes3.egg-info/dependency_links.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)        1 2021-06-28 12:41:48.000000 bacpypes3-0.0.73/bacpypes3.egg-info/not-zip-safe
--rw-rw-r--   0 joel      (1000) joel      (1000)       16 2023-05-10 06:11:40.000000 bacpypes3-0.0.73/bacpypes3.egg-info/top_level.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)      100 2022-08-22 00:12:37.000000 bacpypes3-0.0.73/pyproject.toml
--rw-rw-r--   0 joel      (1000) joel      (1000)       38 2023-05-10 06:11:40.109958 bacpypes3-0.0.73/setup.cfg
--rw-rw-r--   0 joel      (1000) joel      (1000)     1219 2023-05-04 14:51:12.000000 bacpypes3-0.0.73/setup.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.101958 bacpypes3-0.0.73/tests/
--rw-rw-r--   0 joel      (1000) joel      (1000)      351 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2298 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/clocked_test.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      372 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/conftest.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    49924 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/state_machine.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      644 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_1.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3054 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test__template.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.105958 bacpypes3-0.0.73/tests/test_constructed_data/
--rw-rw-r--   0 joel      (1000) joel      (1000)      247 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_constructed_data/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2616 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_constructed_data/test_any.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2526 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_constructed_data/test_array.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2894 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_constructed_data/test_choice.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2071 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_constructed_data/test_list.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4013 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_constructed_data/test_read_property_multiple.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    10217 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_constructed_data/test_sequence.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8422 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_constructed_data/test_sequence_of.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.105958 bacpypes3-0.0.73/tests/test_pdu/
--rw-rw-r--   0 joel      (1000) joel      (1000)      126 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_pdu/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    16509 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_pdu/test_address.py
--rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_pdu/test_pci.py
--rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_pdu/test_pdu.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.105958 bacpypes3-0.0.73/tests/test_primitive_data/
--rw-rw-r--   0 joel      (1000) joel      (1000)      456 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3309 2023-01-09 14:29:42.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_bit_string.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2629 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_boolean.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3204 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_character_string.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2671 2023-02-17 06:25:03.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_date.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2794 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_double.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3266 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_enumerated.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2632 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_integer.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2363 2022-10-03 15:42:31.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_null.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3739 2021-07-22 21:59:33.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_object_identifier.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2775 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_octet_string.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2785 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_real.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4262 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_tag.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2546 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_time.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3588 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_unsigned.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.105958 bacpypes3-0.0.73/tests/test_utilities/
--rw-rw-r--   0 joel      (1000) joel      (1000)      130 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_utilities/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    18594 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_utilities/test_state_machine.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.109958 bacpypes3-0.0.73/tests/test_vlan/
--rw-rw-r--   0 joel      (1000) joel      (1000)      200 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_vlan/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8287 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_vlan/test_ipv4_network.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     6304 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_vlan/test_ipv4_router.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8904 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_vlan/test_network.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    12098 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/trapped_classes.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     1397 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/utilities.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.507772 bacpypes3-0.0.77/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      666 2023-07-01 17:58:49.507772 bacpypes3-0.0.77/PKG-INFO
+-rw-rw-r--   0 joel      (1000) joel      (1000)      346 2023-03-09 18:20:30.000000 bacpypes3-0.0.77/README.md
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.491772 bacpypes3-0.0.77/bacpypes3/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1370 2023-07-01 17:57:36.000000 bacpypes3-0.0.77/bacpypes3/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    23928 2023-07-01 17:57:36.000000 bacpypes3-0.0.77/bacpypes3/__main__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    56648 2023-01-24 05:27:28.000000 bacpypes3-0.0.77/bacpypes3/apdu.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    34041 2023-07-01 17:57:36.000000 bacpypes3-0.0.77/bacpypes3/app.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    65777 2023-04-04 12:53:18.000000 bacpypes3-0.0.77/bacpypes3/appservice.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    20848 2023-05-31 11:51:39.000000 bacpypes3-0.0.77/bacpypes3/argparse.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)   112385 2023-06-23 03:49:41.000000 bacpypes3-0.0.77/bacpypes3/basetypes.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    16150 2023-04-03 15:32:38.000000 bacpypes3-0.0.77/bacpypes3/cmd.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     7934 2022-11-21 19:40:26.000000 bacpypes3-0.0.77/bacpypes3/comm.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     7128 2023-01-24 05:27:28.000000 bacpypes3-0.0.77/bacpypes3/console.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    64295 2023-04-07 19:15:02.000000 bacpypes3-0.0.77/bacpypes3/constructeddata.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10659 2023-06-29 13:02:40.000000 bacpypes3-0.0.77/bacpypes3/debugging.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     9685 2023-02-08 13:29:16.000000 bacpypes3-0.0.77/bacpypes3/errors.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.495772 bacpypes3-0.0.77/bacpypes3/ipv4/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     9245 2023-06-26 19:19:16.000000 bacpypes3-0.0.77/bacpypes3/ipv4/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8238 2023-04-22 03:23:44.000000 bacpypes3-0.0.77/bacpypes3/ipv4/app.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    25882 2023-04-21 19:42:07.000000 bacpypes3-0.0.77/bacpypes3/ipv4/bvll.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4119 2023-02-12 01:55:32.000000 bacpypes3-0.0.77/bacpypes3/ipv4/link.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    61699 2023-04-21 19:25:10.000000 bacpypes3-0.0.77/bacpypes3/ipv4/service.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.495772 bacpypes3-0.0.77/bacpypes3/ipv6/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     6298 2023-01-09 14:29:42.000000 bacpypes3-0.0.77/bacpypes3/ipv6/__init__.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    32041 2023-01-24 14:48:16.000000 bacpypes3-0.0.77/bacpypes3/ipv6/bvll.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    57488 2023-02-01 12:39:44.000000 bacpypes3-0.0.77/bacpypes3/ipv6/service.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.495772 bacpypes3-0.0.77/bacpypes3/json/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      102 2023-01-24 13:54:53.000000 bacpypes3-0.0.77/bacpypes3/json/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      132 2022-09-06 15:15:46.000000 bacpypes3-0.0.77/bacpypes3/json/__main__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    16743 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/bacpypes3/json/util.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.495772 bacpypes3-0.0.77/bacpypes3/lib/
+-rw-rw-r--   0 joel      (1000) joel      (1000)       41 2023-01-24 05:27:28.000000 bacpypes3-0.0.77/bacpypes3/lib/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10085 2021-08-04 12:18:07.000000 bacpypes3-0.0.77/bacpypes3/lib/batchread.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.499772 bacpypes3-0.0.77/bacpypes3/local/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      463 2023-06-20 12:14:17.000000 bacpypes3-0.0.77/bacpypes3/local/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     5804 2023-06-21 18:50:45.000000 bacpypes3-0.0.77/bacpypes3/local/analog.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4447 2023-06-21 18:50:45.000000 bacpypes3-0.0.77/bacpypes3/local/binary.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     6059 2023-06-20 12:14:17.000000 bacpypes3-0.0.77/bacpypes3/local/cmd.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    18826 2023-06-20 12:14:17.000000 bacpypes3-0.0.77/bacpypes3/local/cov.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     5769 2023-01-24 13:31:42.000000 bacpypes3-0.0.77/bacpypes3/local/device.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    87515 2023-06-26 19:19:16.000000 bacpypes3-0.0.77/bacpypes3/local/event.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    14523 2023-06-21 18:50:45.000000 bacpypes3-0.0.77/bacpypes3/local/fault.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     5022 2023-07-01 17:57:36.000000 bacpypes3-0.0.77/bacpypes3/local/networkport.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    23309 2023-06-21 18:50:45.000000 bacpypes3-0.0.77/bacpypes3/local/object.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1046 2023-01-03 14:48:04.000000 bacpypes3-0.0.77/bacpypes3/local/oos.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    24830 2023-02-06 04:19:11.000000 bacpypes3-0.0.77/bacpypes3/local/schedule.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    77433 2023-07-01 17:57:36.000000 bacpypes3-0.0.77/bacpypes3/netservice.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    28240 2023-01-24 05:27:28.000000 bacpypes3-0.0.77/bacpypes3/npdu.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    94171 2023-06-20 12:14:17.000000 bacpypes3-0.0.77/bacpypes3/object.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    65850 2023-06-26 19:19:16.000000 bacpypes3-0.0.77/bacpypes3/pdu.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    80966 2023-02-17 06:25:03.000000 bacpypes3-0.0.77/bacpypes3/primitivedata.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.499772 bacpypes3-0.0.77/bacpypes3/rdf/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      353 2023-01-24 13:54:37.000000 bacpypes3-0.0.77/bacpypes3/rdf/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      130 2022-08-22 23:43:00.000000 bacpypes3-0.0.77/bacpypes3/rdf/__main__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10595 2023-05-04 14:15:16.000000 bacpypes3-0.0.77/bacpypes3/rdf/core.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    19634 2023-01-27 13:19:10.000000 bacpypes3-0.0.77/bacpypes3/rdf/util.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.499772 bacpypes3-0.0.77/bacpypes3/sc/
+-rw-rw-r--   0 joel      (1000) joel      (1000)       65 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/bacpypes3/sc/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    33859 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/bacpypes3/sc/bvll.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    18081 2023-02-27 03:52:18.000000 bacpypes3-0.0.77/bacpypes3/sc/service.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.499772 bacpypes3-0.0.77/bacpypes3/service/
+-rw-rw-r--   0 joel      (1000) joel      (1000)       78 2023-01-24 13:55:00.000000 bacpypes3-0.0.77/bacpypes3/service/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    22512 2023-04-03 19:06:43.000000 bacpypes3-0.0.77/bacpypes3/service/cov.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    22741 2023-04-04 12:42:09.000000 bacpypes3-0.0.77/bacpypes3/service/device.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    31277 2023-04-03 19:49:50.000000 bacpypes3-0.0.77/bacpypes3/service/object.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3869 2023-05-31 11:51:39.000000 bacpypes3-0.0.77/bacpypes3/settings.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.499772 bacpypes3-0.0.77/bacpypes3/vlan/
+-rw-rw-r--   0 joel      (1000) joel      (1000)    11838 2023-07-01 17:57:36.000000 bacpypes3-0.0.77/bacpypes3/vlan/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1692 2023-07-01 17:57:36.000000 bacpypes3-0.0.77/bacpypes3/vlan/link.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.495772 bacpypes3-0.0.77/bacpypes3.egg-info/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      666 2023-07-01 17:58:49.000000 bacpypes3-0.0.77/bacpypes3.egg-info/PKG-INFO
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3049 2023-07-01 17:58:49.000000 bacpypes3-0.0.77/bacpypes3.egg-info/SOURCES.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)        1 2023-07-01 17:58:49.000000 bacpypes3-0.0.77/bacpypes3.egg-info/dependency_links.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)        1 2021-06-28 12:41:48.000000 bacpypes3-0.0.77/bacpypes3.egg-info/not-zip-safe
+-rw-rw-r--   0 joel      (1000) joel      (1000)       16 2023-07-01 17:58:49.000000 bacpypes3-0.0.77/bacpypes3.egg-info/top_level.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)      100 2022-08-22 00:12:37.000000 bacpypes3-0.0.77/pyproject.toml
+-rw-rw-r--   0 joel      (1000) joel      (1000)       38 2023-07-01 17:58:49.507772 bacpypes3-0.0.77/setup.cfg
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1219 2023-05-04 14:51:12.000000 bacpypes3-0.0.77/setup.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.503772 bacpypes3-0.0.77/tests/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      351 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2298 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/clocked_test.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      372 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/conftest.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    49924 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/state_machine.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      644 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_1.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3054 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test__template.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.503772 bacpypes3-0.0.77/tests/test_constructed_data/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      247 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_constructed_data/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2616 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_constructed_data/test_any.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2526 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_constructed_data/test_array.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2894 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_constructed_data/test_choice.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2071 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_constructed_data/test_list.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4013 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_constructed_data/test_read_property_multiple.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10217 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_constructed_data/test_sequence.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8422 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_constructed_data/test_sequence_of.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.503772 bacpypes3-0.0.77/tests/test_pdu/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      126 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_pdu/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    16509 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_pdu/test_address.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_pdu/test_pci.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_pdu/test_pdu.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.507772 bacpypes3-0.0.77/tests/test_primitive_data/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      456 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3309 2023-01-09 14:29:42.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_bit_string.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2629 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_boolean.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3204 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_character_string.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2671 2023-02-17 06:25:03.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_date.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2794 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_double.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3266 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_enumerated.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2632 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_integer.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2363 2022-10-03 15:42:31.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_null.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3739 2021-07-22 21:59:33.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_object_identifier.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2775 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_octet_string.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2785 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_real.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4262 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_tag.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2546 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_time.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3588 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_unsigned.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.507772 bacpypes3-0.0.77/tests/test_utilities/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      130 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_utilities/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    18594 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_utilities/test_state_machine.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.507772 bacpypes3-0.0.77/tests/test_vlan/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      200 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_vlan/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8287 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_vlan/test_ipv4_network.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     6304 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_vlan/test_ipv4_router.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8904 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_vlan/test_network.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    12098 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/trapped_classes.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1397 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/utilities.py
```

### Comparing `bacpypes3-0.0.73/PKG-INFO` & `bacpypes3-0.0.77/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacpypes3
-Version: 0.0.73
+Version: 0.0.77
 Summary: BACnet Communications Library
 Home-page: https://github.com/JoelBender/bacpypes3
 Author: Joel Bender
 Author-email: joel@carrickbender.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bacpypes3-0.0.73/bacpypes3/__init__.py` & `bacpypes3-0.0.77/bacpypes3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 if _sys.platform not in _supported_platforms:
     _warnings.warn("unsupported platform", RuntimeWarning)
 
 #
 #   Project Metadata
 #
 
-__version__ = "0.0.73"
+__version__ = "0.0.77"
 __author__ = "Joel Bender"
 __email__ = "joel@carrickbender.com"
 
 #
 #   Settings and Debugging
 #
```

### Comparing `bacpypes3-0.0.73/bacpypes3/__main__.py` & `bacpypes3-0.0.77/bacpypes3/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,24 +29,24 @@
 from bacpypes3.netservice import NetworkAdapter
 
 # for BVLL services
 from bacpypes3.ipv4.bvll import Result as IPv4BVLLResult
 from bacpypes3.ipv4.service import BVLLServiceAccessPoint, BVLLServiceElement
 
 # for serializing the configuration
-from bacpypes3.json import sequence_to_json
+from .json import sequence_to_json
 
 # some debugging
 _debug = 0
 _log = ModuleLogger(globals())
 
 
 # globals
-app: Application
-bvll_ase: BVLLServiceElement
+app: Optional[Application] = None
+bvll_ase: Optional[BVLLServiceElement] = None
 
 # 'property[index]' matching
 property_index_re = re.compile(r"^([A-Za-z-]+)(?:\[([0-9]+)\])?$")
 
 
 @bacpypes_debugging
 class CmdShell(Cmd):
@@ -158,17 +158,17 @@
         except Exception as err:
             if _debug:
                 CmdShell._debug("    - exception: %r", err)
             await self.response(str(err))
 
     async def do_whois(
         self,
-        address: Address = None,
-        low_limit: int = None,
-        high_limit: int = None,
+        address: Optional[Address] = None,
+        low_limit: Optional[int] = None,
+        high_limit: Optional[int] = None,
     ) -> None:
         """
         Send a Who-Is request and wait for the response(s).
 
         usage: whois [ address [ low_limit high_limit ] ]
         """
         if _debug:
@@ -181,15 +181,15 @@
             for i_am in i_ams:
                 if _debug:
                     CmdShell._debug("    - i_am: %r", i_am)
                 await self.response(f"{i_am.iAmDeviceIdentifier[1]} {i_am.pduSource}")
 
     async def do_iam(
         self,
-        address: Address = None,
+        address: Optional[Address] = None,
     ) -> None:
         """
         Send an I-Am request, no response.
 
         usage: iam [ address ]
         """
         if _debug:
@@ -207,50 +207,50 @@
         usage: whohas [ low_limit high_limit ] [ objid ] [ objname ] [ address ]
         """
         if _debug:
             CmdShell._debug("do_whohas %r", args)
 
         if not args:
             raise RuntimeError("object-identifier or object-name expected")
-        args = list(args)
+        args_list: List[str] = list(args)
 
-        if args[0].isdigit():
-            low_limit = int(args.pop(0))
+        if args_list[0].isdigit():
+            low_limit = int(args_list.pop(0))
         else:
             low_limit = None
-        if args[0].isdigit():
-            high_limit = int(args.pop(0))
+        if args_list[0].isdigit():
+            high_limit = int(args_list.pop(0))
         else:
             high_limit = None
         if _debug:
             CmdShell._debug(
                 "    - low_limit, high_limit: %r, %r", low_limit, high_limit
             )
 
-        if not args:
+        if not args_list:
             raise RuntimeError("object-identifier expected")
         try:
-            object_identifier = ObjectIdentifier(args[0])
-            del args[0]
+            object_identifier = ObjectIdentifier(args_list[0])
+            del args_list[0]
         except ValueError:
             object_identifier = None
         if _debug:
             CmdShell._debug("    - object_identifier: %r", object_identifier)
 
-        if len(args) == 0:
+        if len(args_list) == 0:
             object_name = address = None
-        elif len(args) == 2:
-            object_name = args[0]
-            address = Address(args[1])
-        elif len(args) == 1:
+        elif len(args_list) == 2:
+            object_name = args_list[0]
+            address = Address(args_list[1])
+        elif len(args_list) == 1:
             try:
-                address = Address(args[0])
+                address = Address(args_list[0])
                 object_name = None
             except ValueError:
-                object_name = args[0]
+                object_name = args_list[0]
                 address = None
         else:
             raise RuntimeError("unrecognized arguments")
         if _debug:
             CmdShell._debug("    - object_name: %r", object_name)
             CmdShell._debug("    - address: %r", address)
 
@@ -267,15 +267,15 @@
                     f"{i_have.deviceIdentifier[1]} {i_have.objectIdentifier} {i_have.objectName!r}"
                 )
 
     async def do_ihave(
         self,
         object_identifier: ObjectIdentifier,
         object_name: CharacterString,
-        address: Address = None,
+        address: Optional[Address] = None,
     ) -> None:
         """
         Send an I-Have request.
 
         usage: ihave objid objname [ address ]
         """
         if _debug:
@@ -293,15 +293,15 @@
         """
         Read Property Multiple
 
         usage: rpm address ( objid ( prop [ indx ] )... )...
         """
         if _debug:
             CmdShell._debug("do_rpm %r %r", address, args)
-        args = list(args)
+        args_list: List[str] = list(args)
 
         # get information about the device from the cache
         device_info = await app.device_info_cache.get_device_info(address)
         if _debug:
             CmdShell._debug("    - device_info: %r", device_info)
 
         # using the device info, look up the vendor information
@@ -309,29 +309,29 @@
             vendor_info = get_vendor_info(device_info.vendor_identifier)
         else:
             vendor_info = get_vendor_info(0)
         if _debug:
             CmdShell._debug("    - vendor_info: %r", vendor_info)
 
         parameter_list = []
-        while args:
+        while args_list:
             # get the object identifier and using the vendor information, look
             # up the class
-            object_identifier = vendor_info.object_identifier(args.pop(0))
+            object_identifier = vendor_info.object_identifier(args_list.pop(0))
             object_class = vendor_info.get_object_class(object_identifier[0])
             if not object_class:
                 await self.response(f"unrecognized object type: {object_identifier}")
                 return
 
             # save this as a parameter
             parameter_list.append(object_identifier)
 
             while args:
                 # now get the property type from the class
-                property_identifier = vendor_info.property_identifier(args.pop(0))
+                property_identifier = vendor_info.property_identifier(args_list.pop(0))
                 if _debug:
                     CmdShell._debug(
                         "    - property_identifier: %r", property_identifier
                     )
                 if property_identifier not in (
                     PropertyIdentifier.all,
                     PropertyIdentifier.required,
@@ -346,21 +346,21 @@
                         )
                         return
 
                 # save this as a parameter
                 parameter_list.append(property_identifier)
 
                 # check for a property array index
-                if args and args[0].isdigit():
-                    property_array_index = int(args.pop(0))
+                if args and args_list[0].isdigit():
+                    property_array_index = int(args_list.pop(0))
                     # save this as a parameter
                     parameter_list.append(property_array_index)
 
                 # crude check to see if the next thing is an object identifier
-                if args and ((":" in args[0]) or ("," in args[0])):
+                if args and ((":" in args_list[0]) or ("," in args_list[0])):
                     break
 
         if not parameter_list:
             await self.response("object identifier expected")
             return
 
         try:
@@ -385,15 +385,17 @@
                     f"{object_identifier} {property_identifier}[{property_array_index}] {property_value}"
                 )
             else:
                 await self.response(
                     f"{object_identifier} {property_identifier} {property_value}"
                 )
 
-    async def do_wirtn(self, address: Address = None, network: int = None) -> None:
+    async def do_wirtn(
+        self, address: Optional[Address] = None, network: Optional[int] = None
+    ) -> None:
         """
         Who Is Router To Network
 
         usage: wirtn [ address [ network ] ]
         """
         if _debug:
             CmdShell._debug("do_wirtn %r %r", address, network)
@@ -431,15 +433,15 @@
                 + ", ".join(
                     str(dnet) for dnet in i_am_router_to_network.iartnNetworkList
                 )
             )
 
         await self.response("\n".join(report))
 
-    async def do_irt(self, address: Address = None) -> None:
+    async def do_irt(self, address: Optional[Address] = None) -> None:
         """
         Initialize Routing Table
 
         usage: irt [ address ]
         """
         if _debug:
             CmdShell._debug("do_irt %r", address)
@@ -642,16 +644,14 @@
         else:
             raise ValueError("format")
 
 
 async def main() -> None:
     global app, bvll_ase
 
-    app = None
-    bvll_ase = None
     try:
         parser = SimpleArgumentParser(prog="bacpypes3")
         parser.add_argument(
             "-v",
             "--version",
             help="print the version and exit",
             action="store_true",
@@ -704,14 +704,15 @@
         if _debug:
             _log.debug("app: %r", app)
 
         # pick out the BVLL service access point from the local adapter
         local_adapter = app.nsap.local_adapter
         if _debug:
             _log.debug("local_adapter: %r", local_adapter)
+        assert local_adapter
         bvll_sap = local_adapter.clientPeer
 
         # only IPv4 for now
         if isinstance(bvll_sap, BVLLServiceAccessPoint):
             if _debug:
                 _log.debug("bvll_sap: %r", bvll_sap)
```

### Comparing `bacpypes3-0.0.73/bacpypes3/apdu.py` & `bacpypes3-0.0.77/bacpypes3/apdu.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/app.py` & `bacpypes3-0.0.77/bacpypes3/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,21 +70,24 @@
 from .service.device import WhoIsIAmServices, WhoHasIHaveServices
 from .service.object import (
     ReadWritePropertyServices,
     ReadWritePropertyMultipleServices,
 )
 from .service.cov import ChangeOfValueServices
 
+# network port interpretation
 from .local.networkport import NetworkPortObject
 from .ipv4.link import (
     NormalLinkLayer as NormalLinkLayer_ipv4,
     ForeignLinkLayer as ForeignLinkLayer_ipv4,
     BBMDLinkLayer as BBMDLinkLayer_ipv4,
 )
+from .vlan.link import VirtualLinkLayer
 
+# objects with specialized interpreters
 from .local.schedule import ScheduleObject
 
 # for serialized parameter initialization
 from .json import json_to_sequence
 
 if TYPE_CHECKING:
     # class is declared as generic in stubs but not at runtime
@@ -649,14 +652,35 @@
                     self.nsap.bind(
                         link_layer, net=obj.networkNumber, address=link_address
                     )
 
             elif obj.networkType == NetworkType.ipv6:
                 raise NotImplementedError("IPv6")
 
+            elif obj.networkType == NetworkType.virtual:
+                link_address = obj.address
+                if _debug:
+                    Application._debug("     - link_address: %r", link_address)
+
+                link_layer = VirtualLinkLayer(link_address, obj.networkInterfaceName)
+                if _debug:
+                    Application._debug("     - link_layer: %r", link_layer)
+
+                # save a reference from the object to the link layer, maybe
+                # this will be deleted (in which case it will be closed)
+                self.link_layers[obj.objectIdentifier] = link_layer
+
+                # let the NSAP know about this link layer
+                if obj.networkNumber == 0:
+                    self.nsap.bind(link_layer, address=link_address)
+                else:
+                    self.nsap.bind(
+                        link_layer, net=obj.networkNumber, address=link_address
+                    )
+
             else:
                 raise NotImplementedError(f"{obj.networkType}")
 
         # if this is a schedule object interpret it which will also schedule it
         # to be interpreted again at the next transition
         if isinstance(obj, ScheduleObject):
             obj.interpret_schedule()
```

### Comparing `bacpypes3-0.0.73/bacpypes3/appservice.py` & `bacpypes3-0.0.77/bacpypes3/appservice.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/argparse.py` & `bacpypes3-0.0.77/bacpypes3/argparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/python
 
 """
 argparse
 """
 
 import os
+import os.path
 import sys
 import asyncio
 import shlex
 import json
 import logging
 import logging.handlers
 import argparse
@@ -459,15 +460,15 @@
 
 
 @bacpypes_debugging
 class INIArgumentParser(ArgumentParser):
 
     """
     INIArgumentParser extends the ArgumentParser with the functionality to
-    read in an INI configuration file.  The contents of the [BACpypes] section
+    read in an INI configuration file.  The contents of the file
     will be in the settings.ini attribute.
 
         --ini INI       provide a separate INI file
     """
 
     _debug: Callable[..., None]
 
@@ -496,46 +497,41 @@
         settings["ini"] = os.getenv("BACPYPES_INI", "BACpypes.ini")
 
     def expand_args(self, result_args: argparse.Namespace) -> None:
         """Take the result of parsing the args and interpret them."""
         if _debug:
             INIArgumentParser._debug("expand_args %r", result_args)
 
-        settings["ini"] = result_args.ini
+        if not os.path.exists(result_args.ini):
+            raise RuntimeError("settings file not found: %r\n" % (settings.ini,))
 
-        # read in the configuration file
         config = _ConfigParser()
         config.read(result_args.ini)
         if _debug:
             _log.debug("    - config: %r", config)
 
-        # check for BACpypes section
-        if not config.has_section("BACpypes"):
-            raise RuntimeError("INI file with BACpypes section required")
-
-        # convert the contents to an object
-        ini_obj = dict(config.items("BACpypes"))
-        dict_settings(**ini_obj)
-        if _debug:
-            _log.debug("    - ini_obj: %r", ini_obj)
+        # simplify the content
+        config_dict = {}
+        for section in config.sections():
+            config_dict[section] = dict(config.items(section))
+
+        # save it in settings
+        settings["ini"] = config_dict
 
         # continue with normal expansion
         ArgumentParser.expand_args(self, result_args)
 
-        # stuff the ini contents into settings
-        settings.config = ini_obj
-
 
 @bacpypes_debugging
 class JSONArgumentParser(ArgumentParser):
 
     """
     JSONArgumentParser extends the ArgumentParser with the functionality to
-    read in a JSON configuration file.  The contents of the "BACpypes" element
-    will be in the settings.json attribute.
+    read in a JSON configuration file.  The contents of the file will be in the
+    settings.json attribute.
 
         --json JSON    provide a separate JSON file
     """
 
     _debug: Callable[..., None]
 
     def __init__(self, **kwargs: Any):
@@ -565,34 +561,27 @@
     def expand_args(self, result_args: argparse.Namespace) -> None:
         """Take the result of parsing the args and interpret them."""
         if _debug:
             JSONArgumentParser._debug("expand_args %r", result_args)
 
         # read in the settings file
         try:
-            settings["json"] = result_args.json
             with open(result_args.json) as json_file:
-                json_obj = json.load(json_file, object_hook=Settings)
+                json_obj = json.load(json_file)
                 if _debug:
                     JSONArgumentParser._debug("    - json_obj: %r", json_obj)
         except FileNotFoundError:
             raise RuntimeError("settings file not found: %r\n" % (settings.json,))
 
-        # look for settings
-        if "BACpypes" in json_obj:
-            dict_settings(**json_obj["BACpypes"])
-            if _debug:
-                JSONArgumentParser._debug("    - settings: %r", settings)
+        # save the content
+        settings["json"] = json_obj
 
         # continue with normal expansion
         ArgumentParser.expand_args(self, result_args)
 
-        # stuff the ini contents into settings
-        settings.config = json_obj
-
 
 @bacpypes_debugging
 class YAMLArgumentParser(ArgumentParser):
 
     """
     YAMLArgumentParser extends the ArgumentParser with the functionality to
     read in a YAML configuration file.  The contents of the "BACpypes" element
@@ -639,18 +628,12 @@
             with open(result_args.yaml) as yaml_file:
                 yaml_obj = yaml.safe_load(yaml_file)
                 if _debug:
                     YAMLArgumentParser._debug("    - yaml_obj: %r", yaml_obj)
         except FileNotFoundError:
             raise RuntimeError("settings file not found: %r\n" % (settings.yaml,))
 
-        # look for settings
-        if "BACpypes" in yaml_obj:
-            dict_settings(**yaml_obj["BACpypes"])
-            if _debug:
-                YAMLArgumentParser._debug("    - settings: %r", settings)
+        # save the content
+        settings["yaml"] = yaml_obj
 
         # continue with normal expansion
         ArgumentParser.expand_args(self, result_args)
-
-        # stuff the ini contents into settings
-        settings.config = yaml_obj
```

### Comparing `bacpypes3-0.0.73/bacpypes3/basetypes.py` & `bacpypes3-0.0.77/bacpypes3/basetypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -884,23 +884,28 @@
     accessEvent = 13
     doubleOutOfRange = 14
     signedOutOfRange = 15
     unsignedOutOfRange = 16
     changeOfCharacterstring = 17
     changeOfStatusFlags = 18
     changeOfReliability = 19
+    none = 20
+    changeOfDiscreteValue = 21
+    changeOfTimer = 22
 
 
 class FaultType(Enumerated):
     none = 0
     faultCharacterstring = 1
     faultExtended = 2
     faultLifeSafety = 3
     faultState = 4
     faultStatusFlags = 5
+    faultOutOfRange = 6
+    faultListed = 7
 
 
 class FileAccessMethod(Enumerated):
     recordAccess = 0
     streamAccess = 1
 
 
@@ -2232,26 +2237,69 @@
         """
         if when is None:
             when = time.time()
 
         # return an instance
         return cast(DateTime, cls(date=Date.now(when), time=Time.now(when)))
 
+    def __str__(self) -> str:
+        return f"{self.date} {self.time}"
+
 
 class TimeValue(Sequence):
     _order = ("time", "value")
     time = Time()
     value = AnyAtomic()
 
 
+@bacpypes_debugging
 class DeviceAddress(Sequence):
     _order = ("networkNumber", "macAddress")
     networkNumber = Unsigned()
     macAddress = OctetString()
 
+    def __init__(
+        self,
+        arg: Optional[str] = None,
+        **kwargs,
+    ) -> None:
+        if _debug:
+            DeviceAddress._debug("DeviceAddress.__init__ %r %r", arg, kwargs)
+
+        if arg is None:
+            pass
+        else:
+            if isinstance(arg, str):
+                arg = _Address(arg)
+            if not isinstance(arg, _Address):
+                raise TypeError(type(arg))
+            if not any(
+                (
+                    arg.is_localbroadcast,
+                    arg.is_localstation,
+                    arg.is_remotebroadcast,
+                    arg.is_remotestation,
+                )
+            ):
+                raise ValueError(arg)
+            kwargs["networkNumber"] = arg.addrNet or 0
+            kwargs["macAddress"] = arg.addrAddr or b""
+
+        super().__init__(**kwargs)
+
+    @classmethod
+    def cast(cls, arg):
+        if _debug:
+            HostAddress._debug("DeviceAddress.cast %r", arg)
+
+        if isinstance(arg, (bytes, bytearray, str, dict, IPv4Address, IPv6Address)):
+            return arg
+        else:
+            raise TypeError(type(arg))
+
 
 _sequence_number = 0
 
 
 class TimeStamp(Choice):
     time = Time(_context=0)
     sequenceNumber = Unsigned(_context=1)
@@ -2269,14 +2317,17 @@
             now = _sequence_number % 65536
         return cls(sequenceNumber=now)
 
     @classmethod
     def as_dateTime(cls: type, when: Optional[float] = None) -> TimeStamp:
         return cls(dateTime=DateTime.now(when))
 
+    def __str__(self) -> str:
+        return str(getattr(self, self._choice, "None"))
+
 
 class Recipient(Choice):
     device = ObjectIdentifier(_context=0)
     address = DeviceAddress(_context=1)
 
 
 class ListOfRecipient(ListOf(Recipient)):
@@ -3248,15 +3299,22 @@
     bitmask = BitString(_context=1)
     listOfBitstringValues = SequenceOf(BitString, _context=2)
 
 
 class EventParameterChangeOfCharacterString(Sequence):
     _order = ("timeDelay", "listOfAlarmValues")
     timeDelay = Unsigned(_context=0)
-    listOfAlarmValues = SequenceOf(CharacterString, _context=1)
+    listOfAlarmValues = SequenceOf(
+        CharacterString, _context=1
+    )  # maybe ArrayOf(OptionalCharacterString)
+
+
+class EventParameterChangeOfDiscreteValue(Sequence):
+    _order = ("timeDelay",)
+    timeDelay = Unsigned(_context=0)
 
 
 class EventParameterChangeOfLifeSafety(Sequence):
     _order = (
         "timeDelay",
         "listOfLifeSafetyAlarmValues",
         "listOfAlarmValues",
@@ -3276,14 +3334,21 @@
 
 class EventParameterChangeOfStatusFlags(Sequence):
     _order = ("timeDelay", "selectedFlags")
     timeDelay = Unsigned(_context=0)
     selectedFlags = StatusFlags(_context=1)
 
 
+class EventParameterChangeOfTimer(Sequence):
+    _order = ("timeDelay", "alarmValues", "updateTimeReference")
+    timeDelay = Unsigned(_context=0)
+    alarmValues = SequenceOf(TimerState, _context=1)
+    updateTimeReference = DeviceObjectPropertyReference(_context=2)
+
+
 class EventParameterChangeOfValueCOVCriteria(Choice):
     bitmask = BitString(_context=0)
     referencedPropertyIncrement = Real(_context=1)
 
 
 class EventParameterChangeOfValue(Sequence):
     _order = ("timeDelay", "covCriteria")
@@ -3434,14 +3499,32 @@
 
 
 class FaultParameterStatusFlags(Sequence):
     _order = ("statusFlagsReference",)
     statusFlagsReference = DeviceObjectPropertyReference(_context=0)
 
 
+class FaultParameterOutOfRangeValue(Choice):
+    real = Real()
+    unsigned = Unsigned()
+    double = Double()
+    integer = Integer()
+
+
+class FaultParameterOutOfRange(Sequence):
+    _order = ("minNormalValue", "maxNormalValue")
+    minNormalValue = FaultParameterOutOfRangeValue(_context=0)
+    maxNormalValue = FaultParameterOutOfRangeValue(_context=1)
+
+
+class FaultParametersFaultListed(Sequence):
+    _order = ("faultListReference",)
+    faultListReference = SequenceOf(DeviceObjectPropertyReference, _context=0)
+
+
 class GetAlarmSummaryAlarmSummary(Sequence):
     _order = ("objectIdentifier", "alarmState", "acknowledgedTransitions")
     objectIdentifier = ObjectIdentifier()
     alarmState = EventState()
     acknowledgedTransitions = EventTransitionBits()
 
 
@@ -3941,23 +4024,29 @@
     unsignedRange = EventParameterUnsignedRange(_context=11)
     accessEvent = EventParameterAccessEvent(_context=13)
     doubleOutOfRange = EventParameterDoubleOutOfRange(_context=14)
     signedOutOfRange = EventParameterSignedOutOfRange(_context=15)
     unsignedOutOfRange = EventParameterUnsignedOutOfRange(_context=16)
     changeOfCharacterstring = EventParameterChangeOfCharacterString(_context=17)
     changeOfStatusflags = EventParameterChangeOfStatusFlags(_context=18)
+    # choice 19 intentionally omitted
+    none = Null(_context=20)
+    changeOfDiscreteValue = EventParameterChangeOfDiscreteValue(_context=21)
+    changeOfTimer = EventParameterChangeOfTimer(_context=22)
 
 
 class FaultParameter(Choice):
     none = Null(_context=0)
     faultCharacterString = FaultParameterCharacterString(_context=1)
     faultExtended = FaultParameterExtended(_context=2)
     faultLifeSafety = FaultParameterLifeSafety(_context=3)
     faultState = FaultParameterState(_context=4)
     faultStatusFlags = FaultParameterStatusFlags(_context=5)
+    faultOutOfRange = FaultParameterOutOfRange(_context=6)
+    faultListed = FaultParametersFaultListed(_context=7)
 
 
 class ObjectSelector(Choice):
     none = Null()
     object = ObjectIdentifier()
     objectType = ObjectType()
```

### Comparing `bacpypes3-0.0.73/bacpypes3/cmd.py` & `bacpypes3-0.0.77/bacpypes3/cmd.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/comm.py` & `bacpypes3-0.0.77/bacpypes3/comm.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/console.py` & `bacpypes3-0.0.77/bacpypes3/console.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/constructeddata.py` & `bacpypes3-0.0.77/bacpypes3/constructeddata.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/debugging.py` & `bacpypes3-0.0.77/bacpypes3/debugging.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,17 @@
     Optional,
     TextIO,
     Tuple,
     TypeVar,
     Union,
 )
 
-# create a root logger
+# create a root logger with a Null handler
 root_logger = logging.getLogger("bacpypes3")
+root_logger.addHandler(logging.NullHandler())
 
 # types
 FuncType = Callable[..., Any]
 F = TypeVar("F", bound=FuncType)
 
 # module loggers
 module_loggers: Dict[logging.Logger, Dict[str, Any]] = {}
@@ -83,21 +84,14 @@
 
     # create a logger to be assigned to _log
     logger = logging.getLogger(logger_name)
 
     # put in a reference to the module globals
     module_loggers[logger] = globs
 
-    # if this is a "root" logger add a default handler for warnings and up
-    if "." not in logger_name:
-        hdlr = logging.StreamHandler()
-        hdlr.setLevel(logging.WARNING)
-        hdlr.setFormatter(logging.Formatter(logging.BASIC_FORMAT, None))
-        logger.addHandler(hdlr)
-
     return logger
 
 
 # some debugging
 _debug = 0
 _log = ModuleLogger(globals())
```

### Comparing `bacpypes3-0.0.73/bacpypes3/errors.py` & `bacpypes3-0.0.77/bacpypes3/errors.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/ipv4/__init__.py` & `bacpypes3-0.0.77/bacpypes3/ipv4/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import functools
 
 from typing import Any, Callable, Optional, List, Tuple, Union, cast
 
 from ..debugging import ModuleLogger, bacpypes_debugging
 
 from ..comm import Server
-from ..pdu import LocalBroadcast, IPv4Address, PDU
+from ..pdu import LocalStation, LocalBroadcast, IPv4Address, PDU
 
 
 # some debugging
 _debug = 0
 _log = ModuleLogger(globals())
 
 
@@ -209,22 +209,24 @@
                 IPv4DatagramServer._debug(
                     "    - waiting for tasks: %r", self._transport_tasks
                 )
             await asyncio.gather(*self._transport_tasks)
             self._transport_tasks = []
 
         # downstream packets can have a specific or local broadcast address
-        if isinstance(pdu.pduDestination, LocalBroadcast):
+        if isinstance(pdu.pduDestination, LocalStation):
+            pdu_destination = IPv4Address(pdu.pduDestination).addrTuple
+        elif isinstance(pdu.pduDestination, LocalBroadcast):
             if not self.broadcast_address:
                 raise RuntimeError("no broadcast")
             pdu_destination = self.broadcast_address
         elif isinstance(pdu.pduDestination, IPv4Address):
             pdu_destination = pdu.pduDestination.addrTuple
         else:
-            raise ValueError("invalid destination: {pdu.pduDestination}")
+            raise ValueError(f"invalid destination: {pdu.pduDestination}")
         if _debug:
             IPv4DatagramServer._debug("    - pdu_destination: %r", pdu_destination)
 
         # send it along
         self.local_transport.sendto(pdu.pduData, pdu_destination)
 
     async def confirmation(self, pdu: PDU) -> None:
```

### Comparing `bacpypes3-0.0.73/bacpypes3/ipv4/app.py` & `bacpypes3-0.0.77/bacpypes3/ipv4/app.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/ipv4/bvll.py` & `bacpypes3-0.0.77/bacpypes3/ipv4/bvll.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/ipv4/link.py` & `bacpypes3-0.0.77/bacpypes3/ipv4/link.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/ipv4/service.py` & `bacpypes3-0.0.77/bacpypes3/ipv4/service.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/ipv6/__init__.py` & `bacpypes3-0.0.77/bacpypes3/ipv6/__init__.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/ipv6/bvll.py` & `bacpypes3-0.0.77/bacpypes3/ipv6/bvll.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/ipv6/service.py` & `bacpypes3-0.0.77/bacpypes3/ipv6/service.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/json/util.py` & `bacpypes3-0.0.77/bacpypes3/json/util.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/lib/batchread.py` & `bacpypes3-0.0.77/bacpypes3/lib/batchread.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/local/cmd.py` & `bacpypes3-0.0.77/bacpypes3/local/cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,19 @@
     Optional,
     Union,
 )
 
 from bacpypes3.debugging import bacpypes_debugging, ModuleLogger
 
 from bacpypes3.errors import PropertyError
-from bacpypes3.basetypes import PriorityArray as _PriorityArray, PriorityValue
+from bacpypes3.basetypes import (
+    OptionalUnsigned,
+    PriorityArray as _PriorityArray,
+    PriorityValue,
+)
 from bacpypes3.local.object import Object as _Object
 
 # some debugging
 _debug = 0
 _log = ModuleLogger(globals())
 
 
@@ -74,14 +78,20 @@
         super().__init__(**kwargs)
 
         # default priority-array is all Null
         if priority_array is None:
             priority_array = [PriorityValue(null=()) for _ in range(16)]
         self.priorityArray = PriorityArray(priority_array, obj=self)
 
+        # default relinquishDefault is initial presentValue
+        if self.relinquishDefault is None:
+            super().__setattr__("relinquishDefault", self.presentValue)
+        if self.currentCommandPriority is None:
+            super().__setattr__("currentCommandPriority", OptionalUnsigned(null=()))
+
     def __setattr__(self, attr: str, value: _Any) -> None:
         """
         Changing the presentValue is actully writing to the priorityArray
         with a default of the lowest priority.  Writing the entire
         priorityArray is usually done during initialization with
         a keyword value or from unmarshalling from a JSON blob or
         RDF graph.
@@ -156,15 +166,21 @@
 
         value: _Any
         priority_array = self.priorityArray
         for i in range(0, 16):
             pv = priority_array[i]
             if pv.null is None:
                 value = getattr(pv, pv._choice)
+                if _debug:
+                    Commandable._debug("    - value at %d: %r", i, value)
+                super().__setattr__(
+                    "currentCommandPriority", OptionalUnsigned(unsigned=i + 1)
+                )
                 break
         else:
             value = self.relinquishDefault
-        if _debug:
-            Commandable._debug("    - present value: %r", value)
+            super().__setattr__("currentCommandPriority", OptionalUnsigned(null=()))
+            if _debug:
+                Commandable._debug("    - relinquish default")
 
         # update the presentValue
         super().__setattr__("presentValue", value)
```

### Comparing `bacpypes3-0.0.73/bacpypes3/local/cov.py` & `bacpypes3-0.0.77/bacpypes3/local/cov.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,14 @@
 #
 #   DetectionAlgorithm
 #
 
 
 @bacpypes_debugging
 class DetectionAlgorithm:
-
     _debug: Callable[..., None]
 
     _monitors: List[DetectionMonitor]
     _execute_handle: asyncio.Handle
 
     def __init__(self):
         if _debug:
@@ -191,15 +190,14 @@
 #
 #   COVDetection
 #
 
 
 @bacpypes_debugging
 class COVDetection(DetectionAlgorithm):
-
     properties_tracked = ()
     properties_reported = ()
     monitored_property_reference = None
 
     def __init__(self, obj) -> None:
         if _debug:
             COVDetection._debug("__init__ %r", obj)
@@ -336,29 +334,27 @@
                 COVDetection._debug("    - request: %s", repr(request))
 
             # let the application send it
             self.obj._app.cov_notification(cov, request)
 
 
 class GenericCriteria(COVDetection):
-
     properties_tracked = (
         "presentValue",
         "statusFlags",
     )
     properties_reported = (
         "presentValue",
         "statusFlags",
     )
     monitored_property_reference = "presentValue"
 
 
 @bacpypes_debugging
 class COVIncrementCriteria(COVDetection):
-
     properties_tracked = (
         "presentValue",
         "statusFlags",
         "covIncrement",
     )
     properties_reported = (
         "presentValue",
@@ -371,15 +367,15 @@
             COVIncrementCriteria._debug("__init__ %r", obj)
         COVDetection.__init__(self, obj)
 
         # previously reported value
         self.previously_reported_value = None
 
     @monitor_filter("presentValue")
-    def present_value_filter(self, old_value, new_value):
+    def present_value_filter(self, old_value, new_value) -> bool:
         if _debug:
             COVIncrementCriteria._debug(
                 "present_value_filter %r %r", old_value, new_value
             )
 
         # first time around initialize to the old value
         if self.previously_reported_value is None:
@@ -406,29 +402,27 @@
         self.previously_reported_value = self.presentValue
 
         # continue
         super().send_cov_notifications(subscription)
 
 
 class AccessDoorCriteria(COVDetection):
-
     properties_tracked = (
         "presentValue",
         "statusFlags",
         "doorAlarmState",
     )
     properties_reported = (
         "presentValue",
         "statusFlags",
         "doorAlarmState",
     )
 
 
 class AccessPointCriteria(COVDetection):
-
     properties_tracked = (
         "accessEventTime",
         "statusFlags",
     )
     properties_reported = (
         "accessEvent",
         "statusFlags",
@@ -437,25 +431,23 @@
         "accessEventCredential",
         "accessEventAuthenticationFactor",
     )
     monitored_property_reference = "accessEvent"
 
 
 class CredentialDataInputCriteria(COVDetection):
-
     properties_tracked = ("updateTime", "statusFlags")
     properties_reported = (
         "presentValue",
         "statusFlags",
         "updateTime",
     )
 
 
 class LoadControlCriteria(COVDetection):
-
     properties_tracked = (
         "presentValue",
         "statusFlags",
         "requestedShedLevel",
         "startTime",
         "shedDuration",
         "dutyWindow",
@@ -468,15 +460,14 @@
         "shedDuration",
         "dutyWindow",
     )
 
 
 @bacpypes_debugging
 class PulseConverterCriteria(COVIncrementCriteria):
-
     properties_tracked = (
         "presentValue",
         "statusFlags",
         "covPeriod",
     )
     properties_reported = (
         "presentValue",
@@ -527,15 +518,15 @@
             if self.cov_period_task and self.cov_period_task.isScheduled:
                 self.cov_period_task.suspend_task()
                 if _debug:
                     PulseConverterCriteria._debug("    - cov period task suspended")
                 self.cov_period_task = None
 
     @monitor_filter("covPeriod")
-    def cov_period_filter(self, old_value, new_value):
+    def cov_period_filter(self, old_value, new_value) -> bool:
         if _debug:
             PulseConverterCriteria._debug(
                 "cov_period_filter %r %r", old_value, new_value
             )
 
         # check for an old period
         if old_value != 0:
@@ -571,17 +562,17 @@
     ObjectType.analogInput: COVIncrementCriteria,
     ObjectType.analogOutput: COVIncrementCriteria,
     ObjectType.analogValue: COVIncrementCriteria,
     "largeAnalogValue": COVIncrementCriteria,
     "integerValue": COVIncrementCriteria,
     "positiveIntegerValue": COVIncrementCriteria,
     "lightingOutput": COVIncrementCriteria,
-    "binaryInput": GenericCriteria,
-    "binaryOutput": GenericCriteria,
-    "binaryValue": GenericCriteria,
+    ObjectType.binaryInput: GenericCriteria,
+    ObjectType.binaryOutput: GenericCriteria,
+    ObjectType.binaryValue: GenericCriteria,
     "lifeSafetyPoint": GenericCriteria,
     "lifeSafetyZone": GenericCriteria,
     "multiStateInput": GenericCriteria,
     "multiStateOutput": GenericCriteria,
     "multiStateValue": GenericCriteria,
     "octetString": GenericCriteria,
     "characterString": GenericCriteria,
```

### Comparing `bacpypes3-0.0.73/bacpypes3/local/device.py` & `bacpypes3-0.0.77/bacpypes3/local/device.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/local/networkport.py` & `bacpypes3-0.0.77/bacpypes3/local/networkport.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from __future__ import annotations
 
 from typing import Callable, Optional
 
 from ..debugging import bacpypes_debugging, ModuleLogger
-from ..pdu import Address, IPv4Address, IPv6Address
+from ..pdu import Address, LocalStation, IPv4Address, IPv6Address
 from ..primitivedata import CharacterString, ObjectType
 
 from ..basetypes import NetworkType, NetworkNumberQuality
 from ..object import NetworkPortObject as _NetworkPortObject
 
 from .object import Object as _Object
 
@@ -144,8 +144,14 @@
             return IPv4Address(addr + "/" + mask + ":" + port)
 
         elif self.networkType == NetworkType.ipv6:
             if _debug:
                 NetworkPortObject._debug("    - IPv6")
             raise NotImplementedError("no IPv6 yet")
 
+        elif self.networkType == NetworkType.virtual:
+            if _debug:
+                NetworkPortObject._debug("    - virtual")
+
+            return LocalStation(self.macAddress)
+
         return None
```

### Comparing `bacpypes3-0.0.73/bacpypes3/local/object.py` & `bacpypes3-0.0.77/bacpypes3/rdf/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,295 +1,354 @@
 """
-Local Object
+Core
 """
 
-import asyncio
-import inspect
+from __future__ import annotations
 
-from collections import defaultdict
-from copy import deepcopy
-from functools import partial
-from threading import Thread
-from typing import Any as _Any, Callable, Dict, List
-
-from ..debugging import bacpypes_debugging, ModuleLogger
-from ..errors import PropertyError
-from ..primitivedata import CharacterString, ObjectIdentifier
+from typing import Any, Callable, Optional
+
+from rdflib import Graph, Literal, BNode, URIRef  # type: ignore[import]
+from rdflib.namespace import Namespace, RDF, RDFS, XSD  # type: ignore[import]
+from rdflib.plugins.sparql import prepareQuery  # type: ignore[import]
+
+from ..debugging import bacpypes_debugging, ModuleLogger, btox
+
+from ..pdu import Address
+from ..primitivedata import (
+    Atomic,
+    ObjectIdentifier,
+)
 from ..basetypes import PropertyIdentifier
-from ..constructeddata import ArrayOf
+from ..constructeddata import Sequence
 
-from ..object import Object as _Object
+from .util import atomic_encode, attr_to_predicate, sequence_to_graph
 
 # some debugging
 _debug = 0
 _log = ModuleLogger(globals())
 
 
-# this is for sample applications
-_vendor_id = 999
+BACnetNS = Namespace("http://data.ashrae.org/bacnet/2016#")
+BACnetURI = Namespace("bacnet:")
 
-
-@bacpypes_debugging
-class PropertyChangeThread(Thread):
-    """
-    An instance of this class is used when the setter and/or getter of
-    a property is a coroutine function and must run in its own event
-    loop.
+#
+#   Node Identifiers
+#
+
+
+def device_node(
+    device_identifier: ObjectIdentifier,
+) -> URIRef:
+    """Given a device identifer return a URI reference for the device, the
+    default function returns a value from Annex Q.8."""
+    return BACnetURI["//" + str(device_identifier[1])]
+
+
+def object_node(
+    device_iri: URIRef,
+    object_identifier: ObjectIdentifier,
+) -> URIRef:
+    """Given a device IRI for context and an object identifier,
+    return a URI reference for the object."""
+    return device_iri + "/" + str(object_identifier)
+
+
+def property_node(
+    object_iri: URIRef,
+    property_identifier: PropertyIdentifier,
+) -> URIRef:
+    """Given an object IRI for context and a property identifier, return a URI
+    reference for the property."""
+    return object_iri + "/" + str(property_identifier)
+
+
+def blank_node() -> URIRef:
+    """Return a blank node."""
+    return BNode()
+
+
+_device_node: Callable[..., URIRef] = device_node
+_object_node: Callable[..., URIRef] = object_node
+_blank_node: Callable[..., URIRef] = blank_node
+
+
+def set_identifier_functions(
+    *,
+    device_node_fn: Callable[..., URIRef] = device_node,
+    object_node_fn: Callable[..., URIRef] = object_node,
+    blank_node_fn: Callable[..., URIRef] = blank_node,
+):
+    """This function allows the application using the library to provide
+    its own functions for contsructing URI node identifiers for
+    devices, objects and blank nodes.
     """
+    global _device_node, _object_node, _blank_node
 
-    def __init__(self, getattr_fn, setattr_fn, new_value) -> None:
-        if _debug:
-            PropertyChangeThread._debug(
-                "__init__ %r %r %r", getattr_fn, setattr_fn, new_value
-            )
-        super().__init__()
+    _device_node = device_node_fn
+    _object_node = object_node_fn
+    _blank_node = blank_node_fn
 
-        self.getattr_fn = getattr_fn
-        self.setattr_fn = setattr_fn
-        self.new_value = new_value
 
-        # result is a (old_value, new_value) tuple if it changed
-        self.result = None
+#
+#   Common prepared queries
+#
 
-        self.start()
 
-    def run(self):
-        loop = asyncio.new_event_loop()
-        self.result = loop.run_until_complete(self._run())
-        loop.close()
+def bacnet_query(query: str) -> Any:
+    """Prepare a SPARQL query with the BACnet namespace prefix included.
+    The prepared query is provided to the `BACnetGraph.query()` method
+    along with initial variable bindings if they have been provided.
+    """
+    return prepareQuery(query, initNs={"bacnet": BACnetNS})
 
-    async def _run(self):
-        if _debug:
-            PropertyChangeThread._debug("_run")
 
-        # get the current value, wait for it if necessary
-        current_value: _Any = self.getattr_fn()
-        if _debug:
-            PropertyChangeThread._debug("    - current_value: %r", current_value)
-        if inspect.isawaitable(current_value):
-            current_value = await current_value
-            if _debug:
-                PropertyChangeThread._debug(
-                    "    - awaited current_value: %r", current_value
-                )
-
-        # usually these are primitive data elements
-        current_value = deepcopy(current_value)
-        if current_value == self.new_value:
-            return
+find_device_by_address = bacnet_query(
+    """
+    select ?s where { ?s bacnet:hasAddress [
+        bacnet::network-number ?net ;
+        bacnet:mac-address ?addr
+        ] }
+    """
+)
+find_device_by_instance = bacnet_query(
+    "select ?s where { ?s bacnet:deviceInstance ?device_instance .}"
+)
+find_object_by_type = bacnet_query(
+    "select ?s where { ?s bacnet:object-type ?objtype .}"
+)
 
-        set_result = self.setattr_fn(self.new_value)
-        if _debug:
-            PropertyChangeThread._debug("    - set_result: %r", set_result)
-        if inspect.isawaitable(set_result):
-            set_result = await set_result
-            if _debug:
-                PropertyChangeThread._debug("    - awaited set_result: %r", set_result)
 
-        return (current_value, self.new_value)
+#
+#   BACnetGraph
+#
 
 
 @bacpypes_debugging
-class Object(_Object):
+class BACnetGraph:
     """
-    A local object has specialized property functions for changing the object
-    name and identifier and has a dynamically generated propertyList property.
+    Creates a graph context where BACnet content can be found.
     """
 
-    __objectName: CharacterString
-    __objectIdentifier: ObjectIdentifier
-    _property_monitors: Dict[str, List[Callable[..., None]]]
-
-    def __init__(self, **kwargs) -> None:
-        if _debug:
-            Object._debug("__init__ %r", kwargs)
+    _debug: Callable[..., None]
 
-        self.__objectName = None
-        self.__objectIdentifier = None
-        self._property_monitors = defaultdict(list)
+    def __init__(self, graph: Graph) -> None:
+        self.graph = graph
 
-        super().__init__(**kwargs)
+        # bind the BACnet namespace
+        self.graph.namespace_manager.bind("bacnet", URIRef(BACnetNS))
 
-    def __setattr__(self, attr: str, value: _Any) -> None:
+    def bind_namespace(self, prefix: str, uri: str) -> Namespace:
         """
-        This function traps changes to properties that have at least
-        one associated monitor function.
+        Create a Namespace and bind a prefix to it in the graph.
         """
-        if attr.startswith("_") or (attr not in self._property_monitors):
-            super().__setattr__(attr, value)
-            return
-        if _debug:
-            Object._debug("__setattr__ %r %r", attr, value)
-
-        element = self._elements[attr]
-        if _debug:
-            Object._debug("    - element: %r", element)
-
-        if value.__class__ != element:
-            if _debug:
-                Object._debug(
-                    f"    - {attr} casting call: %r != %r", value.__class__, element
-                )
-            value = element(element.cast(value))
-
-        # this might not be an @property defined attribute
-        try:
-            attr_property = inspect.getattr_static(self, attr)
-        except AttributeError:
-            attr_property = None
-        if _debug:
-            Object._debug("    - attr_property: %r", attr_property)
+        namespace = Namespace(uri)
+        self.graph.namespace_manager.bind(prefix, URIRef(uri))
+        return namespace
+
+    def query(self, query: Any, **kwargs: Any) -> Any:
+        """Run a prepared SPARQL query in the graph with the initial bindings
+        and return the results.
+        """
+        # translate the query arguments to make it easy
+        init_bindings = {}
+        for k, v in kwargs.items():
+            if isinstance(v, (URIRef, Literal)):
+                pass
+            elif isinstance(v, Atomic):
+                v = atomic_encode(self.graph, v)
+            elif isinstance(v, (int, float, str)):
+                v = Literal(v)
+            else:
+                raise TypeError(f"keyword {k}: {type(v)}")
+
+            init_bindings[k] = v
+
+        # run the query
+        return self.graph.query(query, initBindings=init_bindings)
+
+    def create_device(
+        self,
+        device_address: Optional[Address],
+        device_identifier: Optional[ObjectIdentifier],
+    ) -> DeviceGraph:
+        """Given a device network address or a device identifier (or both)
+        create and return a DeviceGraph for the device.
+        """
+        device_iri = _device_node(device_identifier)
+        self.graph.add((device_iri, RDF.type, BACnetNS.Device))
 
-        # if the getter and/or setter are coroutine functions then both
-        # calls need to run in a separate thread with its own event
-        # loop.
-        if isinstance(attr_property, property) and (
-            inspect.iscoroutinefunction(attr_property.fget)
-            or inspect.iscoroutinefunction(attr_property.fset)
-        ):
-
-            thread = PropertyChangeThread(
-                partial(attr_property.fget, self),
-                partial(attr_property.fset, self),
-                value,
+        if device_address is not None:
+            device_address_iri = _blank_node()
+            self.graph.add((device_iri, BACnetNS.hasAddress, device_address_iri))
+
+            # encode the network portion, local stations are network 0
+            self.graph.add(
+                (device_address_iri, RDFS.label, Literal(str(device_address)))
             )
-            thread.join()
-            if not thread.result:
-                return
 
-            current_value, value = thread.result
-        else:
-            getattr_fn = partial(super().__getattribute__, attr)
-            setattr_fn = partial(super().__setattr__, attr)
-
-            # get the current value
-            current_value: _Any = getattr_fn()
-            if _debug:
-                Object._debug("    - current_value: %r", current_value)
-
-            # usually these are primitive data elements
-            # current_value = deepcopy(current_value)
-            if value == current_value:
-                return
-
-            element.set_attribute(
-                getter=getattr_fn,
-                setter=setattr_fn,
-                value=value,
+            if device_address.addrNet is None:
+                device_address_net = Literal(0)
+            else:
+                device_address_net = Literal(device_address.addrNet)
+
+            # encode the MAC address, hex string?
+            device_address_mac = Literal(
+                btox(device_address.addrAddr), datatype=XSD.hexBinary
             )
 
-        # tell the monitors
-        for fn in self._property_monitors[attr]:
-            fn(current_value, value)
-
-    @property
-    def objectName(self) -> CharacterString:
-        """Return the private value of the object name."""
-        if _debug:
-            Object._debug("objectName(getter)")
+            device_address_proxy = ObjectProxy(self, device_address_iri)
+            device_address_proxy.networkNumber = device_address_net
+            device_address_proxy.macAddress = device_address_mac
+
+        if device_identifier is not None:
+            self.graph.add(
+                (device_iri, BACnetNS.deviceInstance, Literal(device_identifier[1]))
+            )
 
-        return self.__objectName
+        return DeviceGraph(self, device_iri)
 
-    @objectName.setter
-    def objectName(self, value: CharacterString) -> None:
+    def find_device(
+        self,
+        device_address: Optional[Address] = None,
+        device_identifier: Optional[ObjectIdentifier] = None,
+    ) -> Optional[DeviceGraph]:
+        """Given a device network address or a device identifier (or both)
+        find the existing DeviceGraph for the device, or return None if
+        the device isn't defined.
         """
-        Change the object name, and if it is associated with an application,
-        update the application reference to this object.
-        """
-        if _debug:
-            Object._debug("objectName(setter) %r", value)
-        if value is None:
-            raise ValueError("objectName")
-
-        # make sure it's the correct type
-        object_name_class = self.__class__._elements["objectName"]
-        if not isinstance(value, object_name_class):
-            value = object_name_class.cast(value)
-
-        # check if this is associated with an application
-        if not self._app:
-            self.__objectName = value
-        else:
-            # no change
-            if value == self.__objectName:
-                return
-            if value in self._app.objectName:
-                raise PropertyError("duplicate-name")
-
-            # out with the old, in with the new
-            if self.__objectName in self._app.objectName:
-                del self._app.objectName[self.__objectName]
-            self.__objectName = value
-            self._app.objectName[value] = self
+        return None
 
-    @property
-    def objectIdentifier(self) -> ObjectIdentifier:
-        """
-        Return the private value of the object identifier.
+    def delete_device(
+        self,
+        device_address: Optional[Address] = None,
+        device_identifier: Optional[ObjectIdentifier] = None,
+    ) -> None:
+        """Given a device network address or a device identifier (or both)
+        find the existing DeviceGraph for the device and delete all of its
+        associated nodes.
         """
-        if _debug:
-            Object._debug("objectIdentifier(getter)")
+        pass
 
-        return self.__objectIdentifier
 
-    @objectIdentifier.setter
-    def objectIdentifier(self, value: ObjectIdentifier) -> None:
-        """
-        Change the object identifier, and if it is associated with an
-        application, update the application reference to this object.
+#
+#   DeviceGraph
+#
+
+
+@bacpypes_debugging
+class DeviceGraph:
+    """
+    Creates a graph context where BACnet content for a specific device
+    can be found.
+    """
+
+    _debug: Callable[..., None]
+
+    def __init__(self, graph: BACnetGraph, device_iri: URIRef) -> None:
+        self.graph = graph
+        self.device_iri = device_iri
+
+    def create_object(self, object_identifier: ObjectIdentifier) -> ObjectProxy:
+        """Given an object identifier return an ObjectProxy for the object."""
+        object_iri = _object_node(self.device_iri, object_identifier)
+
+        object_proxy = ObjectProxy(self.graph, object_iri)
+        object_proxy.objectType = object_identifier[0]
+        object_proxy.objectIdentifier = object_identifier
+
+        # associate this object with its device -- layer hopping :-/
+        self.graph.graph.add((self.device_iri, BACnetNS.hasObject, object_iri))
+
+        return object_proxy
+
+    def find_object(self, object_identifier: ObjectIdentifier) -> Optional[ObjectProxy]:
+        """Given an object identifier return an ObjectProxy for the object."""
+        return None
+
+    def delete_object(
+        self,
+        object_identifier: ObjectIdentifier,
+    ) -> None:
+        """Given an object identifier find the existing ObjectProxy for the
+        object and delete all of its associated nodes.
         """
+        # object_iri = _object_node(self.device_iri, object_identifier)
+        # self.graph.remove((self.device_iri, BACnetNS.hasObject, object_iri))
+        pass
+
+
+#
+#   ObjectProxy
+#
+
+
+@bacpypes_debugging
+class ObjectProxy:
+    """
+    A proxy for getting and setting property values of an object.
+    """
+
+    _debug: Callable[..., None]
+
+    _graph: BACnetGraph
+    _object_iri: URIRef
+    _object_cls: Optional[type]
+
+    def __init__(
+        self, graph: BACnetGraph, object_iri: URIRef, object_cls: Optional[type] = None
+    ) -> None:
         if _debug:
-            Object._debug("objectIdentifier(setter) %r", value)
-        if value is None:
-            raise ValueError("objectIdentifier")
-
-        # make sure it's the correct type
-        object_identifier_class = self.__class__._elements["objectIdentifier"]
-        if not isinstance(value, object_identifier_class):
-            value = object_identifier_class.cast(value)
-
-        # check if this is associated with an application
-        if not self._app:
-            self.__objectIdentifier = value
-        else:
-            # no change
-            if value == self.__objectIdentifier:
-                return
-            if value in self._app.objectIdentifier:
-                raise PropertyError("duplicate-object-id")
-
-            # no switching object types
-            if value[0] != self.__objectIdentifier[0]:
-                raise PropertyError("value-out-of-range")
-
-            # out with the old, in with the new
-            if self.__objectIdentifier in self._app.objectIdentifier:
-                del self._app.objectIdentifier[self.__objectIdentifier]
-            self.__objectIdentifier = value
-            self._app.objectIdentifier[value] = self
-
-    @property
-    def propertyList(self) -> ArrayOf(PropertyIdentifier):  # type: ignore[valid-type, override]
-        """Return an array of property identifiers."""
+            ObjectProxy._debug("__init__ %r %r", graph, object_iri)
+
+        self._graph = graph
+        self._object_iri = object_iri
+
+        ###TODO look up the object subclass if it hasn't been provided
+        self._object_cls = object_cls
+
+    def __getattr__(self, attr: str) -> Any:
+        if attr.startswith("_"):  #  or (attr not in self._elements):
+            return object.__getattribute__(self, attr)
         if _debug:
-            Object._debug("propertyList(getter)")
+            ObjectProxy._debug("__getattr__ %r", attr)
 
-        property_list = []
-        property_identifier_class = self._property_identifier_class
-        for element_name in self._elements:
-            value = inspect.getattr_static(self, element_name, None)
-            if value is None:
-                continue
-            property_list.append(property_identifier_class(element_name))
+        s = self._object_iri
+        p = attr_to_predicate(attr)
 
-        return ArrayOf(PropertyIdentifier)(property_list)
+        # uses the convenience function for functional properties
+        o = self._graph.value(s, p, default=None)
+        if o is None:
+            raise AttributeError(attr)
 
-    @propertyList.setter
-    def propertyList(self, value: _Any) -> None:
-        """
-        Change the property list, usually called with None in the case of
-        an object being initialized, or in the case when the value is
-        unmarshalled from a JSON blob or RDF graph, in both cases it
-        can be ignored.
-        """
+        # attempt to interpret the thing as a primitive or constructed value
+        value: Any
+        if (self._object_cls is None) or (self._object_cls not in self._elements):
+            value = o
+        else:
+            raise NotImplementedError(attr)
+
+        return value
+
+    def __setattr__(self, attr: str, value: Any) -> None:
+        if attr.startswith("_"):  # (attr not in self._elements) or (value is None):
+            super().__setattr__(attr, value)
+            return
         if _debug:
-            Object._debug("propertyList(setter) %r", value)
+            ObjectProxy._debug("__setattr__ %r %r", attr, value)
+
+        g = self._graph.graph
+        s = self._object_iri
+        p = attr_to_predicate(attr)
+
+        if isinstance(value, Literal):
+            o = value
+        elif isinstance(value, Atomic):
+            o = atomic_encode(self._graph, value)
+        elif isinstance(value, Sequence):
+            o = _blank_node()
+            sequence_to_graph(value, o, self._graph)
+        else:
+            o = Literal(value)
+
+        # uses the convenience function which removes existing triples for
+        # functional properties
+        g.set((s, p, o))
```

### Comparing `bacpypes3-0.0.73/bacpypes3/local/oos.py` & `bacpypes3-0.0.77/bacpypes3/local/oos.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/local/schedule.py` & `bacpypes3-0.0.77/bacpypes3/local/schedule.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/netservice.py` & `bacpypes3-0.0.77/bacpypes3/netservice.py`

 * *Files 0% similar despite different names*

```diff
@@ -599,33 +599,60 @@
 
         # global broadcast
         if npdu.pduDestination.addrType == Address.globalBroadcastAddr:
             # set the destination
             npdu.pduDestination = LocalBroadcast()
             npdu.npduDADR = pdu.pduDestination
 
-            # send it to all of connected adapters
+            # send it to the local adapter
+            await local_adapter.process_npdu(npdu)
+
+            # make it look routed
+            if _debug:
+                NetworkServiceAccessPoint._debug("    - adding SADR")
+            npdu.npduSADR = RemoteStation(
+                local_adapter.adapterNet,  # type: ignore[arg-type]
+                local_adapter.adapterAddr.addrAddr,  # type: ignore[union-attr]
+            )
+
+            # send it to all of the other connected adapters
             for xadapter in self.adapters.values():
-                await xadapter.process_npdu(npdu)
+                if xadapter is not local_adapter:
+                    await xadapter.process_npdu(npdu)
             return
 
         # remote broadcast
         if (npdu.pduDestination.addrType != Address.remoteBroadcastAddr) and (
             npdu.pduDestination.addrType != Address.remoteStationAddr
         ):
             raise RuntimeError(
                 "invalid destination address type: %s" % (npdu.pduDestination.addrType,)
             )
 
         dnet = npdu.pduDestination.addrNet
         if _debug:
             NetworkServiceAccessPoint._debug("    - dnet: %r", dnet)
 
-        # if the network matches the local adapter it's local
-        if local_adapter and (dnet == local_adapter.adapterNet):
+        # look for a direct connection
+        direct_adapter = self.adapters.get(dnet, None)
+        if _debug:
+            NetworkServiceAccessPoint._debug("    - direct_adapter: %r", direct_adapter)
+
+        # found one
+        if direct_adapter:
+            # maybe it looks routed
+            if direct_adapter is not local_adapter:
+                if _debug:
+                    NetworkServiceAccessPoint._debug("    - adding SADR")
+                npdu.npduSADR = RemoteStation(
+                    local_adapter.adapterNet,  # type: ignore[arg-type]
+                    local_adapter.adapterAddr.addrAddr,  # type: ignore[union-attr]
+                )
+
+            # remap the destination
             if npdu.pduDestination.addrType == Address.remoteStationAddr:
                 if _debug:
                     NetworkServiceAccessPoint._debug(
                         "    - mapping remote station to local station"
                     )
                 npdu.pduDestination = LocalStation(npdu.pduDestination.addrAddr)
             elif npdu.pduDestination.addrType == Address.remoteBroadcastAddr:
@@ -633,15 +660,15 @@
                     NetworkServiceAccessPoint._debug(
                         "    - mapping remote broadcast to local broadcast"
                     )
                 npdu.pduDestination = LocalBroadcast()
             else:
                 raise RuntimeError("addressing problem")
 
-            await local_adapter.process_npdu(npdu)
+            await direct_adapter.process_npdu(npdu)
             return
 
         # get it ready to send when the path is found
         npdu.pduDestination = None
         npdu.npduDADR = pdu.pduDestination
         if _debug:
             NetworkServiceAccessPoint._debug(
```

### Comparing `bacpypes3-0.0.73/bacpypes3/npdu.py` & `bacpypes3-0.0.77/bacpypes3/npdu.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/object.py` & `bacpypes3-0.0.77/bacpypes3/object.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 # mypy: ignore-errors
 
 from __future__ import annotations
 
 import sys
 import inspect
+import warnings
 from functools import partial
 
 from typing import (
     cast,
     Any as _Any,
     Callable,
     Dict,
@@ -266,19 +267,22 @@
             VendorInfo._debug(
                 "register_object_class(%d) %r %r",
                 self.vendor_identifier,
                 object_type,
                 object_class,
             )
         if object_type in self.registered_object_classes:
-            raise RuntimeError(
-                f"object type {object_type!r}"
-                f" for vendor identifier {self.vendor_identifier}"
-                f" already registered: {self.registered_object_classes[object_type]}"
-            )
+            # built-in classes have multiple classes with different features
+            if self.vendor_identifier != 999:
+                warnings.warn(
+                    f"object type {object_type!r}"
+                    f" for vendor identifier {self.vendor_identifier}"
+                    f" already registered: {self.registered_object_classes[object_type]}"
+                )
+            return
 
         self.registered_object_classes[object_type] = object_class
 
     def get_object_class(self, object_type: int) -> Optional[type]:
         return self.registered_object_classes.get(
             object_type, None
         ) or ASHRAE_vendor_info.registered_object_classes.get(
@@ -551,24 +555,24 @@
             raise AttributeError(f"not a property: {attr!r}")
 
         element = self._elements[attr]
 
         class_attr = getattr(self.__class__, attr, None)
         if isinstance(class_attr, property):
             if _debug:
-                Object._debug("    - writing to a property")
+                Object._debug("    - writing to a @property")
             getattr_fn = class_attr.fget
             if getattr_fn:
                 getattr_fn = partial(getattr_fn, self)
             setattr_fn = class_attr.fset
             if setattr_fn:
                 setattr_fn = partial(setattr_fn, self)
         else:
             if _debug:
-                Object._debug("    - not writing to a property")
+                Object._debug("    - not writing to a @property")
             getattr_fn = partial(super().__getattribute__, attr)
             setattr_fn = partial(super().__setattr__, attr)
 
         value = await element.write_property(
             getter=getattr_fn,
             setter=setattr_fn,
             value=value,
@@ -1459,14 +1463,15 @@
     outOfService: Boolean
     supportedFormats: ArrayOf(AuthenticationFactorFormat)
     supportedFormatClasses: ArrayOf(Unsigned)
     updateTime: TimeStamp
     eventDetectionEnable: Boolean
     notificationClass: Unsigned
     eventEnable: EventTransitionBits
+    eventState: EventState
     ackedTransitions: EventTransitionBits
     notifyType: NotifyType
     eventTimeStamps: ArrayOf(TimeStamp, _length=3)
     eventMessageTexts: ArrayOf(CharacterString, _length=3)
     eventMessageTextsConfig: ArrayOf(CharacterString, _length=3)
     reliabilityEvaluationInhibit: Boolean
 
@@ -2533,14 +2538,15 @@
     presentValue: OctetString
     statusFlags: StatusFlags
     eventState: EventState
     reliability: Reliability
     outOfService: Boolean
     priorityArray: ArrayOf(PriorityValue, _length=16)
     relinquishDefault: OctetString
+    reliabilityEvaluationInhibit: Boolean
     currentCommandPriority: OptionalUnsigned
     valueSource: ValueSource
     valueSourceArray: ArrayOf(ValueSource, _length=16)
     lastCommandTime: TimeStamp
     commandTimeArray: ArrayOf(TimeStamp, _length=16)
     auditPriorityFilter: OptionalPriorityFilter
 
@@ -2598,14 +2604,15 @@
     instanceOf: CharacterString
     statusFlags: StatusFlags
     reliability: Reliability
     outOfService: Boolean
     eventDetectionEnable: Boolean
     notificationClass: Unsigned
     eventEnable: EventTransitionBits
+    eventState: EventState
     ackedTransitions: EventTransitionBits
     notifyType: NotifyType
     eventTimeStamps: ArrayOf(TimeStamp, _length=3)
     eventMessageTexts: ArrayOf(CharacterString, _length=3)
     eventMessageTextsConfig: ArrayOf(CharacterString, _length=3)
     reliabilityEvaluationInhibit: Boolean
 
@@ -2783,14 +2790,15 @@
     presentValue: Time
     statusFlags: StatusFlags
     eventState: EventState
     reliability: Reliability
     outOfService: Boolean
     priorityArray: ArrayOf(PriorityValue, _length=16)
     relinquishDefault: Time
+    reliabilityEvaluationInhibit: Boolean
     eventDetectionEnable: Boolean
     notificationClass: Unsigned
     eventEnable: EventTransitionBits
     ackedTransitions: EventTransitionBits
     notifyType: NotifyType
     eventTimeStamps: ArrayOf(TimeStamp, _length=3)
     eventMessageTexts: ArrayOf(CharacterString, _length=3)
```

### Comparing `bacpypes3-0.0.73/bacpypes3/pdu.py` & `bacpypes3-0.0.77/bacpypes3/pdu.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     + _ipv6_address_port
     + ")"
     + _at_route
     + "$"
 )
 
 ethernet_re = re.compile(r"^([0-9A-Fa-f][0-9A-Fa-f][:]){5}([0-9A-Fa-f][0-9A-Fa-f])$")
-interface_port_re = re.compile(r"^(?:([\w]+))(?::(\d+))?$")
+interface_port_re = re.compile(r"^(?:([\w.]+))(?::(\d+))?$")
 host_port_re = re.compile(r"^(?:([\w.]+))(?::(\d+))?$")
 
 network_types: Dict[str, type]
 
 
 @bacpypes_debugging
 class AddressMetaclass(type):
@@ -1093,70 +1093,96 @@
                         # get the list of adapters
                         adapters = ifaddr.get_adapters()
 
                         for adapter in adapters:
                             if adapter.name == interface:
                                 break
                         else:
-                            raise ValueError("no interface: %r" % (interface,))
+                            adapter = None
 
-                        # get a list of the IPv4 addresses, IPv6 are tuples
-                        ipv4_addresses = [
-                            ip for ip in adapter.ips if isinstance(ip.ip, str)
-                        ]
-                        if len(ipv4_addresses) == 0:
-                            raise ValueError(
-                                "no IPv4 addresses for interface: %r" % (interface,)
-                            )
-                        if len(ipv4_addresses) > 1:
-                            raise ValueError(
-                                "multiple IPv4 addresses for interface: %r"
-                                % (interface,)
-                            )
+                        if adapter:
+                            # get a list of the IPv4 addresses, IPv6 are tuples
+                            ipv4_addresses = [
+                                ip for ip in adapter.ips if isinstance(ip.ip, str)
+                            ]
+                            if len(ipv4_addresses) == 0:
+                                raise ValueError(
+                                    "no IPv4 addresses for interface: %r" % (interface,)
+                                )
+                            if len(ipv4_addresses) > 1:
+                                raise ValueError(
+                                    "multiple IPv4 addresses for interface: %r"
+                                    % (interface,)
+                                )
 
-                        # extract the address and the network size
-                        ipv4_address = (
-                            ipv4_addresses[0].ip
-                            + "/"
-                            + str(ipv4_addresses[0].network_prefix)
-                        )
+                            # extract the address and the network size
+                            ipv4_address = (
+                                ipv4_addresses[0].ip
+                                + "/"
+                                + str(ipv4_addresses[0].network_prefix)
+                            )
 
-                        ipaddress.IPv4Interface.__init__(self, ipv4_address)
-                        if _port:
-                            port = int(_port)
-                        break
+                            ipaddress.IPv4Interface.__init__(self, ipv4_address)
+                            if _port:
+                                port = int(_port)
+                            break
 
                     if netifaces:
                         ifaddresses = netifaces.ifaddresses(interface)
                         ipv4_addresses = ifaddresses.get(netifaces.AF_INET, None)
-                        if not ipv4_addresses:
-                            raise ValueError(
-                                "no IPv4 address for interface: %r" % (interface,)
+                        if ipv4_addresses:
+                            if len(ipv4_addresses) > 1:
+                                raise ValueError(
+                                    "multiple IPv4 addresses for interface: %r"
+                                    % (interface,)
+                                )
+
+                            ipv4_address = ipv4_addresses[0]
+                            if _debug:
+                                IPv4Address._debug(
+                                    "    - ipv4_address: %r", ipv4_address
+                                )
+
+                            ipaddress.IPv4Interface.__init__(
+                                self,
+                                ipv4_address["addr"] + "/" + ipv4_address["netmask"],
+                            )
+
+                            if _port:
+                                port = int(_port)
+                            break
+
+                    try:
+                        dns_addresses = set(
+                            str(info[4][0])
+                            for info in socket.getaddrinfo(
+                                interface, None, socket.AddressFamily.AF_INET
                             )
-                        if len(ipv4_addresses) > 1:
+                        )
+                    except Exception as err:
+                        dns_addresses = set()
+                        if _debug:
+                            IPv4Address._debug("    - getaddrinfo exception: %r", err)
+                    if dns_addresses:
+                        if len(dns_addresses) > 1:
                             raise ValueError(
-                                "multiple IPv4 addresses for interface: %r"
-                                % (interface,)
+                                f"multiple IPv4 addresses for host {interface}"
                             )
 
-                        ipv4_address = ipv4_addresses[0]
+                        ipv4_address = dns_addresses.pop()
                         if _debug:
                             IPv4Address._debug("    - ipv4_address: %r", ipv4_address)
 
-                        ipaddress.IPv4Interface.__init__(
-                            self, ipv4_address["addr"] + "/" + ipv4_address["netmask"]
-                        )
+                        ipaddress.IPv4Interface.__init__(self, ipv4_address + "/32")
 
                         if _port:
                             port = int(_port)
                         break
 
-                    raise RuntimeError(
-                        "install ifaddr or netifaces for interface name addresses"
-                    )
+                    raise RuntimeError(f"unable to resolve {interface}")
 
                 raise ValueError("invalid address")
 
         elif isinstance(addr, (bytes, bytearray)):
             if _debug:
                 IPv4Address._debug("    - bytes: %r..%r", addr[:4], addr[4:6])
             ipaddress.IPv4Interface.__init__(self, bytes(addr[:4]))
```

### Comparing `bacpypes3-0.0.73/bacpypes3/primitivedata.py` & `bacpypes3-0.0.77/bacpypes3/primitivedata.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/rdf/util.py` & `bacpypes3-0.0.77/bacpypes3/rdf/util.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/sc/bvll.py` & `bacpypes3-0.0.77/bacpypes3/sc/bvll.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/sc/service.py` & `bacpypes3-0.0.77/bacpypes3/sc/service.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/service/cov.py` & `bacpypes3-0.0.77/bacpypes3/service/cov.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/service/device.py` & `bacpypes3-0.0.77/bacpypes3/service/device.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/service/object.py` & `bacpypes3-0.0.77/bacpypes3/service/object.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/bacpypes3/settings.py` & `bacpypes3-0.0.77/bacpypes3/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     debug=[],
     color=False,
     debug_file="",
     max_bytes=1048576,
     backup_count=5,
     route_aware=False,
     cov_lifetime=60,
-    config={},
 )
 
 
 def os_settings() -> None:
     """
     Update the settings from known OS environment variables.
     """
```

### Comparing `bacpypes3-0.0.73/bacpypes3/vlan/__init__.py` & `bacpypes3-0.0.77/bacpypes3/vlan/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from copy import deepcopy
 
 from typing import Any, List, Optional, Callable, TypeVar, Generic
 
 from ..errors import ConfigurationError
 from ..debugging import ModuleLogger, bacpypes_debugging
 
-from ..pdu import IPv4Address, PDU
+from ..pdu import LocalStation, LocalBroadcast, IPv4Address, PDU
 from ..comm import Client, Server, bind
 
 AddrType = TypeVar("AddrType")
 
 # some debugging
 _debug = 0
 _log = ModuleLogger(globals())
@@ -373,7 +373,73 @@
             if inode is not node:
                 if _debug:
                     IPv4Router._debug("    - inode: %r", inode)
                 if pdu.pduDestination in inode.lan.network:
                     if _debug:
                         IPv4Router._debug("    - processing: %r", inode)
                     await inode.process_pdu(pdu)
+
+
+#
+#   VirtualNetwork
+#
+
+
+@bacpypes_debugging
+class VirtualNetwork(Network[LocalStation]):
+
+    """
+    VirtualNetwork instances are Network objects where the addresses on the
+    network are instances of a generic local station.
+    """
+
+    _debug: Callable[..., None]
+    _networks: Dict[str, VirtualNetwork] = {}
+
+    def __init__(self, network_name: str) -> None:
+        if _debug:
+            VirtualNetwork._debug("__init__ %r", network_name)
+        Network.__init__(self, name=network_name, broadcast_address=LocalBroadcast())
+
+        # check for name collisions
+        if network_name in VirtualNetwork._networks:
+            raise ValueError(f"existing network: {network_name!r}")
+
+        # save a reference
+        VirtualNetwork._networks[network_name] = self
+
+
+#
+#   VirtualNode
+#
+
+
+@bacpypes_debugging
+class VirtualNode(Node[LocalStation]):
+
+    """
+    An VirtualNode is a Node where the address is a generic local station.
+    """
+
+    _debug: Callable[..., None]
+
+    def __init__(
+        self,
+        addr: LocalStation,
+        network_name: str,
+    ) -> None:
+        if _debug:
+            VirtualNode._debug("__init__ %r %r", addr, network_name)
+
+        # get a reference to the virtual network
+        lan = VirtualNetwork._networks.get(network_name, None)
+        if _debug:
+            VirtualNode._debug("    - lan: %r", lan)
+        if lan is None:
+            raise ValueError(f"undefined network: {network_name!r}")
+
+        # continue initializing
+        Node.__init__(
+            self,
+            addr,
+            lan=lan,
+        )
```

### Comparing `bacpypes3-0.0.73/bacpypes3.egg-info/PKG-INFO` & `bacpypes3-0.0.77/bacpypes3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacpypes3
-Version: 0.0.73
+Version: 0.0.77
 Summary: BACnet Communications Library
 Home-page: https://github.com/JoelBender/bacpypes3
 Author: Joel Bender
 Author-email: joel@carrickbender.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bacpypes3-0.0.73/bacpypes3.egg-info/SOURCES.txt` & `bacpypes3-0.0.77/bacpypes3.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -35,17 +35,21 @@
 bacpypes3/ipv6/service.py
 bacpypes3/json/__init__.py
 bacpypes3/json/__main__.py
 bacpypes3/json/util.py
 bacpypes3/lib/__init__.py
 bacpypes3/lib/batchread.py
 bacpypes3/local/__init__.py
+bacpypes3/local/analog.py
+bacpypes3/local/binary.py
 bacpypes3/local/cmd.py
 bacpypes3/local/cov.py
 bacpypes3/local/device.py
+bacpypes3/local/event.py
+bacpypes3/local/fault.py
 bacpypes3/local/networkport.py
 bacpypes3/local/object.py
 bacpypes3/local/oos.py
 bacpypes3/local/schedule.py
 bacpypes3/rdf/__init__.py
 bacpypes3/rdf/__main__.py
 bacpypes3/rdf/core.py
@@ -54,14 +58,15 @@
 bacpypes3/sc/bvll.py
 bacpypes3/sc/service.py
 bacpypes3/service/__init__.py
 bacpypes3/service/cov.py
 bacpypes3/service/device.py
 bacpypes3/service/object.py
 bacpypes3/vlan/__init__.py
+bacpypes3/vlan/link.py
 tests/__init__.py
 tests/clocked_test.py
 tests/conftest.py
 tests/state_machine.py
 tests/test_1.py
 tests/test__template.py
 tests/trapped_classes.py
```

### Comparing `bacpypes3-0.0.73/setup.py` & `bacpypes3-0.0.77/setup.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/clocked_test.py` & `bacpypes3-0.0.77/tests/clocked_test.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/state_machine.py` & `bacpypes3-0.0.77/tests/state_machine.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_1.py` & `bacpypes3-0.0.77/tests/test_1.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test__template.py` & `bacpypes3-0.0.77/tests/test__template.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_constructed_data/test_any.py` & `bacpypes3-0.0.77/tests/test_constructed_data/test_any.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_constructed_data/test_array.py` & `bacpypes3-0.0.77/tests/test_constructed_data/test_array.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_constructed_data/test_choice.py` & `bacpypes3-0.0.77/tests/test_constructed_data/test_choice.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_constructed_data/test_list.py` & `bacpypes3-0.0.77/tests/test_constructed_data/test_list.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_constructed_data/test_read_property_multiple.py` & `bacpypes3-0.0.77/tests/test_constructed_data/test_read_property_multiple.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_constructed_data/test_sequence.py` & `bacpypes3-0.0.77/tests/test_constructed_data/test_sequence.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_constructed_data/test_sequence_of.py` & `bacpypes3-0.0.77/tests/test_constructed_data/test_sequence_of.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_pdu/test_address.py` & `bacpypes3-0.0.77/tests/test_pdu/test_address.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_primitive_data/test_bit_string.py` & `bacpypes3-0.0.77/tests/test_primitive_data/test_bit_string.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_primitive_data/test_boolean.py` & `bacpypes3-0.0.77/tests/test_primitive_data/test_boolean.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_primitive_data/test_character_string.py` & `bacpypes3-0.0.77/tests/test_primitive_data/test_character_string.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_primitive_data/test_date.py` & `bacpypes3-0.0.77/tests/test_primitive_data/test_date.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_primitive_data/test_double.py` & `bacpypes3-0.0.77/tests/test_primitive_data/test_double.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_primitive_data/test_enumerated.py` & `bacpypes3-0.0.77/tests/test_primitive_data/test_enumerated.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_primitive_data/test_integer.py` & `bacpypes3-0.0.77/tests/test_primitive_data/test_integer.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_primitive_data/test_null.py` & `bacpypes3-0.0.77/tests/test_primitive_data/test_null.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_primitive_data/test_object_identifier.py` & `bacpypes3-0.0.77/tests/test_primitive_data/test_object_identifier.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_primitive_data/test_octet_string.py` & `bacpypes3-0.0.77/tests/test_primitive_data/test_octet_string.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_primitive_data/test_real.py` & `bacpypes3-0.0.77/tests/test_primitive_data/test_real.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_primitive_data/test_tag.py` & `bacpypes3-0.0.77/tests/test_primitive_data/test_tag.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_primitive_data/test_time.py` & `bacpypes3-0.0.77/tests/test_primitive_data/test_time.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_primitive_data/test_unsigned.py` & `bacpypes3-0.0.77/tests/test_primitive_data/test_unsigned.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_utilities/test_state_machine.py` & `bacpypes3-0.0.77/tests/test_utilities/test_state_machine.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_vlan/test_ipv4_network.py` & `bacpypes3-0.0.77/tests/test_vlan/test_ipv4_network.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_vlan/test_ipv4_router.py` & `bacpypes3-0.0.77/tests/test_vlan/test_ipv4_router.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/test_vlan/test_network.py` & `bacpypes3-0.0.77/tests/test_vlan/test_network.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/trapped_classes.py` & `bacpypes3-0.0.77/tests/trapped_classes.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.73/tests/utilities.py` & `bacpypes3-0.0.77/tests/utilities.py`

 * *Files identical despite different names*

