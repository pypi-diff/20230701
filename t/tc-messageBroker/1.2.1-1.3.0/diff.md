# Comparing `tmp/tc-messageBroker-1.2.1.tar.gz` & `tmp/tc-messageBroker-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tc-messageBroker-1.2.1.tar", last modified: Wed Jun  7 05:58:00 2023, max compression
+gzip compressed data, was "tc-messageBroker-1.3.0.tar", last modified: Sat Jul  1 08:52:14 2023, max compression
```

## Comparing `tc-messageBroker-1.2.1.tar` & `tc-messageBroker-1.3.0.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.651239 tc-messageBroker-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-07 05:58:00.651239 tc-messageBroker-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 05:58:00.651239 tc-messageBroker-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.647239 tc-messageBroker-1.2.1/tc_messageBroker/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/message_broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.647239 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.647239 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/db_operations/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/db_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/db_operations/mongodb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.647239 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/event/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/event/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/event/events_microservice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.647239 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/queue/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/queue/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.647239 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/choreography.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/choreography_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/saga.py
--rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/saga_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/transaction_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.647239 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.647239 tc-messageBroker-1.2.1/tc_messageBroker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-07 05:58:00.000000 tc-messageBroker-1.2.1/tc_messageBroker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-07 05:58:00.000000 tc-messageBroker-1.2.1/tc_messageBroker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 05:58:00.000000 tc-messageBroker-1.2.1/tc_messageBroker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-07 05:58:00.000000 tc-messageBroker-1.2.1/tc_messageBroker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-07 05:58:00.000000 tc-messageBroker-1.2.1/tc_messageBroker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.647239 tc-messageBroker-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.647239 tc-messageBroker-1.2.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/integration/test_message_broker_exchange_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/integration/test_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/integration/test_saga.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:58:00.651239 tc-messageBroker-1.2.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_choreagraphy_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_enum_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_message_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_predefined_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_saga_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_saga_base_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_saga_next.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_saga_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-07 05:57:37.000000 tc-messageBroker-1.2.1/tests/unit/test_transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.853272 tc-messageBroker-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-01 08:52:14.853272 tc-messageBroker-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 08:52:14.853272 tc-messageBroker-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.845271 tc-messageBroker-1.3.0/tc_messageBroker/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/message_broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.849271 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.849271 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/db_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/db_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/db_operations/mongodb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.849271 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/event/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/event/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/event/events_microservice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.849271 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/queue/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.849271 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/choreography.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/choreography_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/saga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/saga_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/transaction_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.849271 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.849271 tc-messageBroker-1.3.0/tc_messageBroker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-01 08:52:14.000000 tc-messageBroker-1.3.0/tc_messageBroker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-01 08:52:14.000000 tc-messageBroker-1.3.0/tc_messageBroker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 08:52:14.000000 tc-messageBroker-1.3.0/tc_messageBroker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-01 08:52:14.000000 tc-messageBroker-1.3.0/tc_messageBroker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-01 08:52:14.000000 tc-messageBroker-1.3.0/tc_messageBroker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.849271 tc-messageBroker-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.849271 tc-messageBroker-1.3.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/integration/test_message_broker_exchange_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/integration/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/integration/test_saga.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:14.853272 tc-messageBroker-1.3.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_choreagraphy_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_enum_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_message_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_predefined_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_saga_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_saga_base_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_saga_next.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_saga_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-01 08:51:52.000000 tc-messageBroker-1.3.0/tests/unit/test_transactions.py
```

### Comparing `tc-messageBroker-1.2.1/PKG-INFO` & `tc-messageBroker-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-messageBroker
-Version: 1.2.1
+Version: 1.3.0
 Summary: Shared library for message broker in Python
 Author: Mohammad Amin Dadgar, RnDAO
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Description-Content-Type: text/markdown
 
 # tc-messageBrokerPython
```

### Comparing `tc-messageBroker-1.2.1/README.md` & `tc-messageBroker-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.1/setup.py` & `tc-messageBroker-1.3.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 
 setup(
     name="tc-messageBroker",
-    version="1.2.1",
+    version="1.3.0",
     author="Mohammad Amin Dadgar, RnDAO",
     maintainer="Mohammad Amin Dadgar",
     maintainer_email="dadgaramin96@gmail.com",
     packages=find_packages(),
     description="Shared library for message broker in Python",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `tc-messageBroker-1.2.1/tc_messageBroker/message_broker.py` & `tc-messageBroker-1.3.0/tc_messageBroker/message_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,16 @@
     def __new__(cls, broker_url: str, port: int, username: str, password: str):
         ## making it singleton
         if not hasattr(cls, "instance"):
             cls.instance = super(RabbitMQ, cls).__new__(cls)
         return cls.instance
 
     def connect(
-            self, 
-            queue_name: str, 
-            consume_options: dict = None,
-            heartbeat: int = 60
-        ) -> bool:
+        self, queue_name: str, consume_options: dict = None, heartbeat: int = 60
+    ) -> bool:
         """
         connect the rabbitMQ broker and start consuming
 
         Parameters:
         -------------
         queue_name : str
             the queue name to connect
@@ -59,15 +56,15 @@
             credentials = pika.PlainCredentials(self._username, self._password)
             amqpServer = self.broker_url
             self.connection = pika.BlockingConnection(
                 pika.ConnectionParameters(
                     host=amqpServer,
                     port=self.port,
                     credentials=credentials,
-                    heartbeat=heartbeat, ## disabling the heartbeat
+                    heartbeat=heartbeat,  ## disabling the heartbeat
                 ),
             )
             self.channel = self.connection.channel()
 
             # make sure that the channel is created,
             # if not this statement will create it
             self.channel.queue_declare(queue=queue_name)
```

### Comparing `tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/db_operations/mongodb.py` & `tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/db_operations/mongodb.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/choreography.py` & `tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/choreography.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 from .choreography_base import IChoreography
 from .transactions import (
     DISCORD_UPDATE_CHANNELS_TRANSACTIONS,
     DISCORD_SCHEDULED_JOB_TRANSACTIONS,
+    DISCORD_FETCH_MEMBERS_TRANSACTIONS,
 )
 
 
 DISCORD_UPDATE_CHANNELS = IChoreography(
     name="DISCORD_UPDATE_CHANNELS",
     transactions=DISCORD_UPDATE_CHANNELS_TRANSACTIONS,
 )
 
 DISCORD_SCHEDULED_JOB = IChoreography(
     name="DISCORD_SCHEDULED_JOB",
     transactions=DISCORD_SCHEDULED_JOB_TRANSACTIONS,
 )
 
+DISCORD_FETCH_MEMBERS = IChoreography(
+    name="DISCORD_FETCH_MEMBERS",
+    transactions=DISCORD_FETCH_MEMBERS_TRANSACTIONS,
+)
+
 
 class ChoreographyDict:
     DISCORD_UPDATE_CHANNELS = DISCORD_UPDATE_CHANNELS
     DISCORD_SCHEDULED_JOB = DISCORD_SCHEDULED_JOB
+    DISCORD_FETCH_MEMBERS = DISCORD_FETCH_MEMBERS
```

### Comparing `tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/saga.py` & `tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/saga.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/saga_base.py` & `tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/saga_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/transaction_base.py` & `tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/transaction_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/transactions.py` & `tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/transactions.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,20 @@
     ),
     ITransaction(
         Queue.DISCORD_ANALYZER,
         Event.DISCORD_ANALYZER.RUN,
         order=2,
         status=Status.NOT_STARTED,
     ),
+    ITransaction(
+        Queue.DISCORD_BOT,
+        Event.DISCORD_BOT.SEND_MESSAGE,
+        order=3,
+        status=Status.NOT_STARTED,
+    ),
     # ITransaction(
     #     Queue.DISCORD_ANALYZER,
     #     Event.DISCORD_ANALYZER.SAVE,
     #     order=3,
     #     status=Status.NOT_STARTED,
     # ),
     # ITransaction(
@@ -41,7 +47,16 @@
     ITransaction(
         Queue.DISCORD_ANALYZER,
         Event.DISCORD_ANALYZER.RUN_ONCE,
         order=1,
         status=Status.NOT_STARTED,
     ),
 ]
+
+DISCORD_FETCH_MEMBERS_TRANSACTIONS = [
+    ITransaction(
+        Queue.DISCORD_BOT,
+        Event.DISCORD_BOT.FETCH_MEMBERS,
+        order=1,
+        status=Status.NOT_STARTED,
+    )
+]
```

### Comparing `tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py` & `tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.1/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py` & `tc-messageBroker-1.3.0/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.1/tc_messageBroker.egg-info/PKG-INFO` & `tc-messageBroker-1.3.0/tc_messageBroker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-messageBroker
-Version: 1.2.1
+Version: 1.3.0
 Summary: Shared library for message broker in Python
 Author: Mohammad Amin Dadgar, RnDAO
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Description-Content-Type: text/markdown
 
 # tc-messageBrokerPython
```

### Comparing `tc-messageBroker-1.2.1/tc_messageBroker.egg-info/SOURCES.txt` & `tc-messageBroker-1.3.0/tc_messageBroker.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 tests/integration/test_mongodb.py
 tests/integration/test_saga.py
 tests/unit/__init__.py
 tests/unit/test_choreagraphy_base.py
 tests/unit/test_enum_status.py
 tests/unit/test_event.py
 tests/unit/test_message_broker.py
+tests/unit/test_mongodb.py
 tests/unit/test_predefined_transactions.py
 tests/unit/test_queue.py
 tests/unit/test_saga_base.py
 tests/unit/test_saga_base_utils.py
 tests/unit/test_saga_next.py
 tests/unit/test_saga_start.py
 tests/unit/test_transactions.py
```

### Comparing `tc-messageBroker-1.2.1/tests/integration/test_message_broker_exchange_points.py` & `tc-messageBroker-1.3.0/tests/integration/test_message_broker_exchange_points.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.1/tests/integration/test_mongodb.py` & `tc-messageBroker-1.3.0/tests/integration/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.1/tests/integration/test_saga.py` & `tc-messageBroker-1.3.0/tests/integration/test_saga.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.1/tests/unit/test_choreagraphy_base.py` & `tc-messageBroker-1.3.0/tests/unit/test_choreagraphy_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.1/tests/unit/test_message_broker.py` & `tc-messageBroker-1.3.0/tests/unit/test_message_broker.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.1/tests/unit/test_predefined_transactions.py` & `tc-messageBroker-1.3.0/tests/unit/test_predefined_transactions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,54 @@
 from tc_messageBroker.rabbit_mq.saga.transactions import (
     DISCORD_SCHEDULED_JOB_TRANSACTIONS,
     DISCORD_UPDATE_CHANNELS_TRANSACTIONS,
+    DISCORD_FETCH_MEMBERS_TRANSACTIONS,
 )
 from tc_messageBroker.rabbit_mq.queue import Queue
 from tc_messageBroker.rabbit_mq.event import Event
 from tc_messageBroker.rabbit_mq.status import Status
 
 
 def test_discord_update_channels_tx():
     tx = DISCORD_UPDATE_CHANNELS_TRANSACTIONS
 
-    assert len(tx) == 2
+    assert len(tx) == 3
     assert tx[0].order == 1
     assert tx[0].queue == Queue.DISCORD_BOT
     assert tx[0].event == Event.DISCORD_BOT.FETCH
     assert tx[0].status == Status.NOT_STARTED
 
     assert tx[1].order == 2
     assert tx[1].queue == Queue.DISCORD_ANALYZER
     assert tx[1].event == Event.DISCORD_ANALYZER.RUN
     assert tx[1].status == Status.NOT_STARTED
 
+    assert tx[2].order == 3
+    assert tx[2].queue == Queue.DISCORD_BOT
+    assert tx[2].event == Event.DISCORD_BOT.SEND_MESSAGE
+    assert tx[2].status == Status.NOT_STARTED
+
 
 def test_discord_scheduled_job_tx():
     tx = DISCORD_SCHEDULED_JOB_TRANSACTIONS
 
     assert len(tx) == 1
     # assert tx[0].order == 1
     # assert tx[0].queue == Queue.DISCORD_BOT
     # assert tx[0].event == Event.DISCORD_BOT.FETCH
     # assert tx[0].status == Status.NOT_STARTED
 
     assert tx[0].order == 1
     assert tx[0].queue == Queue.DISCORD_ANALYZER
     assert tx[0].event == Event.DISCORD_ANALYZER.RUN_ONCE
     assert tx[0].status == Status.NOT_STARTED
+
+
+def test_discord_bot_fetch_tx():
+    tx = DISCORD_FETCH_MEMBERS_TRANSACTIONS
+
+    assert len(tx) == 1
+
+    assert tx[0].order == 1
+    assert tx[0].queue == Queue.DISCORD_BOT
+    assert tx[0].event == Event.DISCORD_BOT.FETCH_MEMBERS
+    assert tx[0].status == Status.NOT_STARTED
```

### Comparing `tc-messageBroker-1.2.1/tests/unit/test_saga_base.py` & `tc-messageBroker-1.3.0/tests/unit/test_saga_next.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,117 +1,142 @@
-"""
-test the saga_base module
-"""
 from tc_messageBroker.rabbit_mq.saga.saga_base import Saga
-from tc_messageBroker.rabbit_mq.saga.choreography import ChoreographyDict
-from tc_messageBroker.rabbit_mq.saga.choreography_base import IChoreography
 from tc_messageBroker.rabbit_mq.saga.transaction_base import ITransaction
+from tc_messageBroker.rabbit_mq.saga.choreography_base import IChoreography
 from datetime import datetime
 from tc_messageBroker.rabbit_mq.status import Status
 
 
-def test_choreagraphy_sorting_orders_predefined_choreogprahy():
-    saga = Saga(
-        ChoreographyDict.DISCORD_UPDATE_CHANNELS,
-        Status.NOT_STARTED,
-        data=None,
-        created_at=datetime.now(),
+def test_next_single_not_started_tx():
+    choreography = IChoreography(
+        name="choreography_with_random_tx",
+        transactions=[
+            ITransaction("queue", "event", 5, Status.IN_PROGRESS),
+            ITransaction("queue1", "event1", 2, Status.NOT_STARTED),
+            ITransaction("queue", "event", 3, Status.SUCCESS),
+            ITransaction("queue", "event", 1, Status.FAILED),
+            ITransaction("queue", "event", 0, Status.CANCELLED),
+        ],
     )
 
-    ## it should sort the NOT_STARTED transactions
-    (tx_sorted, not_started_count) = saga._sort_transactions(
-        saga.choreography.transactions
-    )
+    def sample_publish(**kwargs):
+        ## shouldn't get to this since there isn't more than on transactions to do
+        assert True is False
+
+    def sample_call():
+        calculations = 6
+        return calculations
 
-    assert not_started_count == 2
-    order_val = 0
-    for tx in tx_sorted:
-        if tx.status == Status.NOT_STARTED:
-            assert order_val < tx.order
-            order_val = tx.order
+    saga = Saga(choreography, Status.NOT_STARTED, data=None, created_at=datetime.now())
 
+    saga.next(
+        publish_method=sample_publish,
+        call_function=sample_call,
+        mongo_creds={},
+        test_mode=True,
+    )
 
-def test_assert_sorting_status_predefined_choreagprahy():
-    """assert the NOT_STARTED transactions to be at the top of the list"""
+    assert saga.status == Status.SUCCESS
+    assert saga.choreography.transactions[1].status == Status.SUCCESS
 
-    saga = Saga(
-        ChoreographyDict.DISCORD_UPDATE_CHANNELS,
-        Status.NOT_STARTED,
-        data=None,
-        created_at=datetime.now(),
-    )
 
-    ## it should sort the NOT_STARTED transactions
-    (tx_sorted, not_started_count) = saga._sort_transactions(
-        saga.choreography.transactions
+def test_next_multiple_not_started_tx():
+    choreography = IChoreography(
+        name="choreography_with_random_tx",
+        transactions=[
+            ITransaction("queue", "event", 5, Status.IN_PROGRESS),
+            ITransaction("queue1", "event1", 2, Status.NOT_STARTED),
+            ITransaction("queue2", "event3", 4, Status.NOT_STARTED),
+            ITransaction("queue", "event", 3, Status.SUCCESS),
+            ITransaction("queue", "event", 1, Status.FAILED),
+            ITransaction("queue", "event", 0, Status.CANCELLED),
+        ],
     )
 
-    assert not_started_count == 2
+    def sample_publish(**kwargs):
+        assert kwargs["queue_name"] == "queue2"
+        assert kwargs["event"] == "event3"
+        assert kwargs["content"]["uuid"] == saga.uuid
+        assert kwargs["content"]["data"] == 6
+
+    def sample_call():
+        calculations = 6
+        return calculations
 
-    condition = False
-    for tx in tx_sorted:
-        if tx.status == Status.NOT_STARTED:
-            assert condition is False
-        else:
-            condition = True
+    saga = Saga(choreography, Status.NOT_STARTED, data=None, created_at=datetime.now())
+
+    saga.next(
+        publish_method=sample_publish,
+        call_function=sample_call,
+        mongo_creds={},
+        test_mode=True,
+    )
+
+    assert saga.status == Status.IN_PROGRESS
+    assert saga.choreography.transactions[1].status == Status.SUCCESS
 
 
-def test_choreagraphy_sorting_orders_random_choreogprahy():
+def test_saga_fails():
     choreography = IChoreography(
         name="choreography_with_random_tx",
         transactions=[
             ITransaction("queue", "event", 5, Status.IN_PROGRESS),
-            ITransaction("queue", "event", 2, Status.NOT_STARTED),
-            ITransaction("queue", "event", 4, Status.NOT_STARTED),
+            ITransaction("queue1", "event1", 2, Status.NOT_STARTED),
+            ITransaction("queue1", "event1", 4, Status.NOT_STARTED),
             ITransaction("queue", "event", 3, Status.SUCCESS),
             ITransaction("queue", "event", 1, Status.FAILED),
             ITransaction("queue", "event", 0, Status.CANCELLED),
         ],
     )
 
+    def sample_publish(**kwargs):
+        ## shouldn't get to this since there isn't more than on transactions to do
+        raise ValueError("An error in pipeline!")
+
+    def sample_call():
+        calculations = 6
+        return calculations
+
     saga = Saga(choreography, Status.NOT_STARTED, data=None, created_at=datetime.now())
 
-    ## it should sort the NOT_STARTED transactions
-    (tx_sorted, not_started_count) = saga._sort_transactions(
-        saga.choreography.transactions
+    saga.next(
+        publish_method=sample_publish,
+        call_function=sample_call,
+        mongo_creds={},
+        test_mode=True,
     )
 
-    assert not_started_count == 2
-    order_val = 0
-    for tx in tx_sorted:
-        if tx.status == Status.NOT_STARTED:
-            assert order_val < tx.order
-            order_val = tx.order
-
+    assert saga.status == Status.FAILED
+    assert saga.choreography.transactions[1].status == Status.SUCCESS
 
-def test_choreagraphy_sorting_status_random_choreogprahy():
-    """assert the NOT_STARTED transactions to be at the top of the list"""
 
+def test_saga_and_transaction_fails():
     choreography = IChoreography(
         name="choreography_with_random_tx",
         transactions=[
             ITransaction("queue", "event", 5, Status.IN_PROGRESS),
-            ITransaction("queue", "event", 2, Status.NOT_STARTED),
-            ITransaction("queue", "event", 4, Status.NOT_STARTED),
+            ITransaction("queue1", "event1", 2, Status.NOT_STARTED),
             ITransaction("queue", "event", 3, Status.SUCCESS),
             ITransaction("queue", "event", 1, Status.FAILED),
             ITransaction("queue", "event", 0, Status.CANCELLED),
         ],
     )
 
+    def sample_publish(**kwargs):
+        ## shouldn't get to this since there isn't more than on transactions to do
+        assert True is False
+
+    def sample_call():
+        calculations = 6
+        raise ValueError("An error in pipeline!")
+        return calculations
+
     saga = Saga(choreography, Status.NOT_STARTED, data=None, created_at=datetime.now())
 
-    ## it should sort the NOT_STARTED transactions
-    (tx_sorted, not_started_count) = saga._sort_transactions(
-        saga.choreography.transactions
+    saga.next(
+        publish_method=sample_publish,
+        call_function=sample_call,
+        mongo_creds={},
+        test_mode=True,
     )
 
-    assert not_started_count == 2
-
-    condition = False
-    status = []
-    for tx in tx_sorted:
-        status.append(tx.status)
-        if tx.status == Status.NOT_STARTED:
-            assert condition is False
-        else:
-            condition = True
+    assert saga.status == Status.FAILED
+    assert saga.choreography.transactions[1].status == Status.FAILED
```

### Comparing `tc-messageBroker-1.2.1/tests/unit/test_saga_base_utils.py` & `tc-messageBroker-1.3.0/tests/unit/test_saga_base_utils.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.1/tests/unit/test_saga_next.py` & `tc-messageBroker-1.3.0/tests/unit/test_saga_base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,142 +1,162 @@
+"""
+test the saga_base module
+"""
 from tc_messageBroker.rabbit_mq.saga.saga_base import Saga
-from tc_messageBroker.rabbit_mq.saga.transaction_base import ITransaction
+from tc_messageBroker.rabbit_mq.saga.choreography import ChoreographyDict
 from tc_messageBroker.rabbit_mq.saga.choreography_base import IChoreography
+from tc_messageBroker.rabbit_mq.saga.transaction_base import ITransaction
 from datetime import datetime
 from tc_messageBroker.rabbit_mq.status import Status
 
 
-def test_next_single_not_started_tx():
-    choreography = IChoreography(
-        name="choreography_with_random_tx",
-        transactions=[
-            ITransaction("queue", "event", 5, Status.IN_PROGRESS),
-            ITransaction("queue1", "event1", 2, Status.NOT_STARTED),
-            ITransaction("queue", "event", 3, Status.SUCCESS),
-            ITransaction("queue", "event", 1, Status.FAILED),
-            ITransaction("queue", "event", 0, Status.CANCELLED),
-        ],
+def test_choreagraphy_sorting_orders_predefined_choreogprahy():
+    saga = Saga(
+        ChoreographyDict.DISCORD_UPDATE_CHANNELS,
+        Status.NOT_STARTED,
+        data=None,
+        created_at=datetime.now(),
     )
 
-    def sample_publish(**kwargs):
-        ## shouldn't get to this since there isn't more than on transactions to do
-        assert True is False
-
-    def sample_call():
-        calculations = 6
-        return calculations
-
-    saga = Saga(choreography, Status.NOT_STARTED, data=None, created_at=datetime.now())
-
-    saga.next(
-        publish_method=sample_publish,
-        call_function=sample_call,
-        mongo_creds={},
-        test_mode=True,
+    ## it should sort the NOT_STARTED transactions
+    (tx_sorted, not_started_count) = saga._sort_transactions(
+        saga.choreography.transactions
     )
 
-    assert saga.status == Status.SUCCESS
-    assert saga.choreography.transactions[1].status == Status.SUCCESS
+    assert not_started_count == 3
+    order_val = 0
+    for tx in tx_sorted:
+        if tx.status == Status.NOT_STARTED:
+            assert order_val < tx.order
+            order_val = tx.order
 
 
-def test_next_multiple_not_started_tx():
-    choreography = IChoreography(
-        name="choreography_with_random_tx",
-        transactions=[
-            ITransaction("queue", "event", 5, Status.IN_PROGRESS),
-            ITransaction("queue1", "event1", 2, Status.NOT_STARTED),
-            ITransaction("queue2", "event3", 4, Status.NOT_STARTED),
-            ITransaction("queue", "event", 3, Status.SUCCESS),
-            ITransaction("queue", "event", 1, Status.FAILED),
-            ITransaction("queue", "event", 0, Status.CANCELLED),
-        ],
-    )
+def test_assert_sorting_status_predefined_choreagprahy():
+    """assert the NOT_STARTED transactions to be at the top of the list"""
 
-    def sample_publish(**kwargs):
-        assert kwargs["queue_name"] == "queue2"
-        assert kwargs["event"] == "event3"
-        assert kwargs["content"]["uuid"] == saga.uuid
-        assert kwargs["content"]["data"] == 6
-
-    def sample_call():
-        calculations = 6
-        return calculations
-
-    saga = Saga(choreography, Status.NOT_STARTED, data=None, created_at=datetime.now())
+    saga = Saga(
+        ChoreographyDict.DISCORD_UPDATE_CHANNELS,
+        Status.NOT_STARTED,
+        data=None,
+        created_at=datetime.now(),
+    )
 
-    saga.next(
-        publish_method=sample_publish,
-        call_function=sample_call,
-        mongo_creds={},
-        test_mode=True,
+    ## it should sort the NOT_STARTED transactions
+    (tx_sorted, not_started_count) = saga._sort_transactions(
+        saga.choreography.transactions
     )
 
-    assert saga.status == Status.IN_PROGRESS
-    assert saga.choreography.transactions[1].status == Status.SUCCESS
+    assert not_started_count == 3
+
+    condition = False
+    for tx in tx_sorted:
+        if tx.status == Status.NOT_STARTED:
+            assert condition is False
+        else:
+            condition = True
 
 
-def test_saga_fails():
+def test_choreagraphy_sorting_orders_random_choreogprahy():
     choreography = IChoreography(
         name="choreography_with_random_tx",
         transactions=[
             ITransaction("queue", "event", 5, Status.IN_PROGRESS),
-            ITransaction("queue1", "event1", 2, Status.NOT_STARTED),
-            ITransaction("queue1", "event1", 4, Status.NOT_STARTED),
+            ITransaction("queue", "event", 2, Status.NOT_STARTED),
+            ITransaction("queue", "event", 4, Status.NOT_STARTED),
             ITransaction("queue", "event", 3, Status.SUCCESS),
             ITransaction("queue", "event", 1, Status.FAILED),
             ITransaction("queue", "event", 0, Status.CANCELLED),
         ],
     )
 
-    def sample_publish(**kwargs):
-        ## shouldn't get to this since there isn't more than on transactions to do
-        raise ValueError("An error in pipeline!")
-
-    def sample_call():
-        calculations = 6
-        return calculations
-
     saga = Saga(choreography, Status.NOT_STARTED, data=None, created_at=datetime.now())
 
-    saga.next(
-        publish_method=sample_publish,
-        call_function=sample_call,
-        mongo_creds={},
-        test_mode=True,
+    ## it should sort the NOT_STARTED transactions
+    (tx_sorted, not_started_count) = saga._sort_transactions(
+        saga.choreography.transactions
     )
 
-    assert saga.status == Status.FAILED
-    assert saga.choreography.transactions[1].status == Status.SUCCESS
+    assert not_started_count == 2
+    order_val = 0
+    for tx in tx_sorted:
+        if tx.status == Status.NOT_STARTED:
+            assert order_val < tx.order
+            order_val = tx.order
+
 
+def test_choreagraphy_sorting_status_random_choreogprahy():
+    """assert the NOT_STARTED transactions to be at the top of the list"""
 
-def test_saga_and_transaction_fails():
     choreography = IChoreography(
         name="choreography_with_random_tx",
         transactions=[
             ITransaction("queue", "event", 5, Status.IN_PROGRESS),
-            ITransaction("queue1", "event1", 2, Status.NOT_STARTED),
+            ITransaction("queue", "event", 2, Status.NOT_STARTED),
+            ITransaction("queue", "event", 4, Status.NOT_STARTED),
             ITransaction("queue", "event", 3, Status.SUCCESS),
             ITransaction("queue", "event", 1, Status.FAILED),
             ITransaction("queue", "event", 0, Status.CANCELLED),
         ],
     )
 
-    def sample_publish(**kwargs):
-        ## shouldn't get to this since there isn't more than on transactions to do
-        assert True is False
-
-    def sample_call():
-        calculations = 6
-        raise ValueError("An error in pipeline!")
-        return calculations
-
     saga = Saga(choreography, Status.NOT_STARTED, data=None, created_at=datetime.now())
 
-    saga.next(
-        publish_method=sample_publish,
-        call_function=sample_call,
-        mongo_creds={},
-        test_mode=True,
-    )
-
-    assert saga.status == Status.FAILED
-    assert saga.choreography.transactions[1].status == Status.FAILED
+    ## it should sort the NOT_STARTED transactions
+    (tx_sorted, not_started_count) = saga._sort_transactions(
+        saga.choreography.transactions
+    )
+
+    assert not_started_count == 2
+
+    condition = False
+    status = []
+    for tx in tx_sorted:
+        status.append(tx.status)
+        if tx.status == Status.NOT_STARTED:
+            assert condition is False
+        else:
+            condition = True
+
+
+def test_saga_create_data():
+    saga_data = {"guild": "some_guildId"}
+    creation_date = datetime.now()
+
+    saga = Saga(
+        ChoreographyDict.DISCORD_UPDATE_CHANNELS,
+        Status.NOT_STARTED,
+        data=saga_data,
+        created_at=creation_date,
+    )
+
+    saga_dict = saga._create_data()
+
+    assert (
+        saga_dict["choreography"]["name"]
+        == ChoreographyDict.DISCORD_UPDATE_CHANNELS.name
+    )
+
+    ## we had a list of transactions
+    for idx, tx in enumerate(saga_dict["choreography"]["transactions"]):
+        predefined_tx = ChoreographyDict.DISCORD_UPDATE_CHANNELS.transactions[idx]
+        assert tx["queue"] == predefined_tx.queue
+        assert tx["event"] == predefined_tx.event
+        assert tx["order"] == predefined_tx.order
+        assert tx["status"] == predefined_tx.status
+        ## these should be not defined in predefine transaction
+        assert "start" not in tx.keys()
+        assert "end" not in tx.keys()
+        assert "runtime" not in tx.keys()
+        assert "message" not in tx.keys()
+        assert "error" not in tx.keys()
+
+        assert predefined_tx.start is None
+        assert predefined_tx.end is None
+        assert predefined_tx.message is None
+        assert predefined_tx.runtime is None
+        assert predefined_tx.error is None
+
+    assert saga_dict["status"] == Status.NOT_STARTED
+    assert saga_dict["data"] == saga_data
+    assert saga_dict["sagaId"] == saga.uuid
+    assert saga_dict["createdAt"] == creation_date
+    assert saga_dict["updatedAt"] is not None
```

### Comparing `tc-messageBroker-1.2.1/tests/unit/test_saga_start.py` & `tc-messageBroker-1.3.0/tests/unit/test_saga_start.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.2.1/tests/unit/test_transactions.py` & `tc-messageBroker-1.3.0/tests/unit/test_transactions.py`

 * *Files identical despite different names*

