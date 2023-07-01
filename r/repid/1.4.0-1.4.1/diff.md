# Comparing `tmp/repid-1.4.0.tar.gz` & `tmp/repid-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repid-1.4.0.tar", last modified: Wed Jun 28 22:20:52 2023, max compression
+gzip compressed data, was "repid-1.4.1.tar", last modified: Sat Jul  1 09:57:27 2023, max compression
```

## Comparing `repid-1.4.0.tar` & `repid-1.4.1.tar`

### file list

```diff
@@ -1,86 +1,87 @@
--rw-r--r--   0        0        0     1069 2023-06-28 22:20:25.053776 repid-1.4.0/LICENSE
--rw-r--r--   0        0        0     2589 2023-06-28 22:20:25.053776 repid-1.4.0/README.md
--rw-r--r--   0        0        0     4041 2023-06-28 22:20:52.294243 repid-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     1138 2023-06-28 22:20:25.061776 repid-1.4.0/repid/__init__.py
--rw-r--r--   0        0        0     1552 2023-06-28 22:20:25.061776 repid-1.4.0/repid/_asyncify.py
--rw-r--r--   0        0        0     5063 2023-06-28 22:20:25.061776 repid-1.4.0/repid/_processor.py
--rw-r--r--   0        0        0     4061 2023-06-28 22:20:25.061776 repid-1.4.0/repid/_runner.py
--rw-r--r--   0        0        0      434 2023-06-28 22:20:25.061776 repid-1.4.0/repid/_utils/__init__.py
--rw-r--r--   0        0        0      501 2023-06-28 22:20:25.061776 repid-1.4.0/repid/_utils/args_bucket_in_message_id.py
--rw-r--r--   0        0        0      272 2023-06-28 22:20:25.061776 repid-1.4.0/repid/_utils/dataclass_hacks.py
--rw-r--r--   0        0        0     1268 2023-06-28 22:20:25.061776 repid-1.4.0/repid/_utils/is_installed.py
--rw-r--r--   0        0        0      536 2023-06-28 22:20:25.061776 repid-1.4.0/repid/_utils/json_encoder.py
--rw-r--r--   0        0        0      135 2023-06-28 22:20:25.061776 repid-1.4.0/repid/_utils/regex_validators.py
--rw-r--r--   0        0        0      504 2023-06-28 22:20:25.061776 repid-1.4.0/repid/actor.py
--rw-r--r--   0        0        0     2499 2023-06-28 22:20:25.061776 repid-1.4.0/repid/config.py
--rw-r--r--   0        0        0     4525 2023-06-28 22:20:25.061776 repid-1.4.0/repid/connection.py
--rw-r--r--   0        0        0      761 2023-06-28 22:20:25.061776 repid-1.4.0/repid/connections/__init__.py
--rw-r--r--   0        0        0     6594 2023-06-28 22:20:25.061776 repid-1.4.0/repid/connections/abc.py
--rw-r--r--   0        0        0      314 2023-06-28 22:20:25.061776 repid-1.4.0/repid/connections/dummy/__init__.py
--rw-r--r--   0        0        0      260 2023-06-28 22:20:25.061776 repid-1.4.0/repid/connections/in_memory/__init__.py
--rw-r--r--   0        0        0     1823 2023-06-28 22:20:25.061776 repid-1.4.0/repid/connections/in_memory/bucket_broker.py
--rw-r--r--   0        0        0     2766 2023-06-28 22:20:25.061776 repid-1.4.0/repid/connections/in_memory/consumer.py
--rw-r--r--   0        0        0     4093 2023-06-28 22:20:25.061776 repid-1.4.0/repid/connections/in_memory/message_broker.py
--rw-r--r--   0        0        0      860 2023-06-28 22:20:25.061776 repid-1.4.0/repid/connections/in_memory/utils.py
--rw-r--r--   0        0        0       90 2023-06-28 22:20:25.061776 repid-1.4.0/repid/connections/rabbitmq/__init__.py
--rw-r--r--   0        0        0     6161 2023-06-28 22:20:25.061776 repid-1.4.0/repid/connections/rabbitmq/consumer.py
--rw-r--r--   0        0        0     7092 2023-06-28 22:20:25.061776 repid-1.4.0/repid/connections/rabbitmq/message_broker.py
--rw-r--r--   0        0        0      362 2023-06-28 22:20:25.061776 repid-1.4.0/repid/connections/rabbitmq/protocols.py
--rw-r--r--   0        0        0      910 2023-06-28 22:20:25.061776 repid-1.4.0/repid/connections/rabbitmq/utils.py
--rw-r--r--   0        0        0      158 2023-06-28 22:20:25.061776 repid-1.4.0/repid/connections/redis/__init__.py
--rw-r--r--   0        0        0     1513 2023-06-28 22:20:25.061776 repid-1.4.0/repid/connections/redis/bucket_broker.py
--rw-r--r--   0        0        0     7593 2023-06-28 22:20:25.061776 repid-1.4.0/repid/connections/redis/consumer.py
--rw-r--r--   0        0        0     7609 2023-06-28 22:20:25.061776 repid-1.4.0/repid/connections/redis/message_broker.py
--rw-r--r--   0        0        0     3818 2023-06-28 22:20:25.065776 repid-1.4.0/repid/connections/redis/utils.py
--rw-r--r--   0        0        0     7882 2023-06-28 22:20:25.065776 repid-1.4.0/repid/converter.py
--rw-r--r--   0        0        0      355 2023-06-28 22:20:25.065776 repid-1.4.0/repid/data/__init__.py
--rw-r--r--   0        0        0     2276 2023-06-28 22:20:25.065776 repid-1.4.0/repid/data/_buckets.py
--rw-r--r--   0        0        0      820 2023-06-28 22:20:25.065776 repid-1.4.0/repid/data/_key.py
--rw-r--r--   0        0        0     5510 2023-06-28 22:20:25.065776 repid-1.4.0/repid/data/_parameters.py
--rw-r--r--   0        0        0       95 2023-06-28 22:20:25.065776 repid-1.4.0/repid/data/priorities.py
--rw-r--r--   0        0        0     3859 2023-06-28 22:20:25.065776 repid-1.4.0/repid/data/protocols.py
--rw-r--r--   0        0        0     3270 2023-06-28 22:20:25.065776 repid-1.4.0/repid/health_check_server.py
--rw-r--r--   0        0        0     7426 2023-06-28 22:20:25.065776 repid-1.4.0/repid/job.py
--rw-r--r--   0        0        0      546 2023-06-28 22:20:25.065776 repid-1.4.0/repid/logger.py
--rw-r--r--   0        0        0     1887 2023-06-28 22:20:25.065776 repid-1.4.0/repid/main.py
--rw-r--r--   0        0        0      257 2023-06-28 22:20:25.065776 repid-1.4.0/repid/middlewares/__init__.py
--rw-r--r--   0        0        0      347 2023-06-28 22:20:25.065776 repid-1.4.0/repid/middlewares/consts.py
--rw-r--r--   0        0        0     3696 2023-06-28 22:20:25.065776 repid-1.4.0/repid/middlewares/middleware.py
--rw-r--r--   0        0        0     3647 2023-06-28 22:20:25.065776 repid-1.4.0/repid/middlewares/wrapper.py
--rw-r--r--   0        0        0        0 2023-06-28 22:20:25.065776 repid-1.4.0/repid/py.typed
--rw-r--r--   0        0        0     1065 2023-06-28 22:20:25.065776 repid-1.4.0/repid/queue.py
--rw-r--r--   0        0        0     1319 2023-06-28 22:20:25.065776 repid-1.4.0/repid/retry_policy.py
--rw-r--r--   0        0        0     5022 2023-06-28 22:20:25.065776 repid-1.4.0/repid/router.py
--rw-r--r--   0        0        0      719 2023-06-28 22:20:25.065776 repid-1.4.0/repid/serializer.py
--rw-r--r--   0        0        0      845 2023-06-28 22:20:25.065776 repid-1.4.0/repid/testing/__init__.py
--rw-r--r--   0        0        0     3184 2023-06-28 22:20:25.065776 repid-1.4.0/repid/testing/modifiers.py
--rw-r--r--   0        0        0     6099 2023-06-28 22:20:25.065776 repid-1.4.0/repid/testing/plugin.py
--rw-r--r--   0        0        0     4726 2023-06-28 22:20:25.065776 repid-1.4.0/repid/worker.py
--rw-r--r--   0        0        0        0 2023-06-28 22:20:25.065776 repid-1.4.0/tests/__init__.py
--rw-r--r--   0        0        0     1145 2023-06-28 22:20:25.065776 repid-1.4.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-28 22:20:25.065776 repid-1.4.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     3241 2023-06-28 22:20:25.065776 repid-1.4.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     1337 2023-06-28 22:20:25.065776 repid-1.4.0/tests/integration/test_buckets.py
--rw-r--r--   0        0        0     4335 2023-06-28 22:20:25.065776 repid-1.4.0/tests/integration/test_consumer.py
--rw-r--r--   0        0        0     4003 2023-06-28 22:20:25.065776 repid-1.4.0/tests/integration/test_default_flow.py
--rw-r--r--   0        0        0     1904 2023-06-28 22:20:25.065776 repid-1.4.0/tests/integration/test_no_messages_lost.py
--rw-r--r--   0        0        0      431 2023-06-28 22:20:25.065776 repid-1.4.0/tests/test_actor.py
--rw-r--r--   0        0        0     4620 2023-06-28 22:20:25.065776 repid-1.4.0/tests/test_config.py
--rw-r--r--   0        0        0     2986 2023-06-28 22:20:25.065776 repid-1.4.0/tests/test_connection.py
--rw-r--r--   0        0        0     3834 2023-06-28 22:20:25.065776 repid-1.4.0/tests/test_consumer.py
--rw-r--r--   0        0        0     2835 2023-06-28 22:20:25.065776 repid-1.4.0/tests/test_consumer_abc.py
--rw-r--r--   0        0        0    10234 2023-06-28 22:20:25.065776 repid-1.4.0/tests/test_default_data_models.py
--rw-r--r--   0        0        0     2110 2023-06-28 22:20:25.065776 repid-1.4.0/tests/test_health_check_server.py
--rw-r--r--   0        0        0     3004 2023-06-28 22:20:25.065776 repid-1.4.0/tests/test_hypothesis.py
--rw-r--r--   0        0        0     3591 2023-06-28 22:20:25.065776 repid-1.4.0/tests/test_job.py
--rw-r--r--   0        0        0     1366 2023-06-28 22:20:25.065776 repid-1.4.0/tests/test_main.py
--rw-r--r--   0        0        0     7842 2023-06-28 22:20:25.065776 repid-1.4.0/tests/test_middleware.py
--rw-r--r--   0        0        0     1097 2023-06-28 22:20:25.065776 repid-1.4.0/tests/test_multiprocessing.py
--rw-r--r--   0        0        0     7388 2023-06-28 22:20:25.065776 repid-1.4.0/tests/test_pydantic.py
--rw-r--r--   0        0        0     3819 2023-06-28 22:20:25.065776 repid-1.4.0/tests/test_pytest_plugin.py
--rw-r--r--   0        0        0      414 2023-06-28 22:20:25.065776 repid-1.4.0/tests/test_queue.py
--rw-r--r--   0        0        0     3180 2023-06-28 22:20:25.065776 repid-1.4.0/tests/test_router.py
--rw-r--r--   0        0        0      764 2023-06-28 22:20:25.065776 repid-1.4.0/tests/test_serializer.py
--rw-r--r--   0        0        0     1895 2023-06-28 22:20:25.065776 repid-1.4.0/tests/test_utils.py
--rw-r--r--   0        0        0     7633 2023-06-28 22:20:25.065776 repid-1.4.0/tests/test_worker.py
--rw-r--r--   0        0        0     4108 1970-01-01 00:00:00.000000 repid-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-01 09:57:07.325157 repid-1.4.1/LICENSE
+-rw-r--r--   0        0        0     2589 2023-07-01 09:57:07.325157 repid-1.4.1/README.md
+-rw-r--r--   0        0        0     4041 2023-07-01 09:57:27.797185 repid-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1138 2023-07-01 09:57:07.329157 repid-1.4.1/repid/__init__.py
+-rw-r--r--   0        0        0     1552 2023-07-01 09:57:07.329157 repid-1.4.1/repid/_asyncify.py
+-rw-r--r--   0        0        0     5063 2023-07-01 09:57:07.329157 repid-1.4.1/repid/_processor.py
+-rw-r--r--   0        0        0     4061 2023-07-01 09:57:07.329157 repid-1.4.1/repid/_runner.py
+-rw-r--r--   0        0        0      434 2023-07-01 09:57:07.329157 repid-1.4.1/repid/_utils/__init__.py
+-rw-r--r--   0        0        0      501 2023-07-01 09:57:07.329157 repid-1.4.1/repid/_utils/args_bucket_in_message_id.py
+-rw-r--r--   0        0        0      272 2023-07-01 09:57:07.329157 repid-1.4.1/repid/_utils/dataclass_hacks.py
+-rw-r--r--   0        0        0     1268 2023-07-01 09:57:07.329157 repid-1.4.1/repid/_utils/is_installed.py
+-rw-r--r--   0        0        0     1012 2023-07-01 09:57:07.329157 repid-1.4.1/repid/_utils/json_encoder.py
+-rw-r--r--   0        0        0      135 2023-07-01 09:57:07.329157 repid-1.4.1/repid/_utils/regex_validators.py
+-rw-r--r--   0        0        0      504 2023-07-01 09:57:07.329157 repid-1.4.1/repid/actor.py
+-rw-r--r--   0        0        0     2499 2023-07-01 09:57:07.329157 repid-1.4.1/repid/config.py
+-rw-r--r--   0        0        0     4525 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connection.py
+-rw-r--r--   0        0        0      761 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/__init__.py
+-rw-r--r--   0        0        0     6594 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/abc.py
+-rw-r--r--   0        0        0      314 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/dummy/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/in_memory/__init__.py
+-rw-r--r--   0        0        0     1823 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/in_memory/bucket_broker.py
+-rw-r--r--   0        0        0     2766 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/in_memory/consumer.py
+-rw-r--r--   0        0        0     4093 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/in_memory/message_broker.py
+-rw-r--r--   0        0        0      860 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/in_memory/utils.py
+-rw-r--r--   0        0        0       90 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     6161 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/rabbitmq/consumer.py
+-rw-r--r--   0        0        0     7092 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/rabbitmq/message_broker.py
+-rw-r--r--   0        0        0      362 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/rabbitmq/protocols.py
+-rw-r--r--   0        0        0      910 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/rabbitmq/utils.py
+-rw-r--r--   0        0        0      158 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/redis/__init__.py
+-rw-r--r--   0        0        0     1513 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/redis/bucket_broker.py
+-rw-r--r--   0        0        0     7593 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/redis/consumer.py
+-rw-r--r--   0        0        0     7609 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/redis/message_broker.py
+-rw-r--r--   0        0        0     3818 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/redis/utils.py
+-rw-r--r--   0        0        0     7136 2023-07-01 09:57:07.329157 repid-1.4.1/repid/converter.py
+-rw-r--r--   0        0        0      355 2023-07-01 09:57:07.329157 repid-1.4.1/repid/data/__init__.py
+-rw-r--r--   0        0        0     2276 2023-07-01 09:57:07.329157 repid-1.4.1/repid/data/_buckets.py
+-rw-r--r--   0        0        0      820 2023-07-01 09:57:07.329157 repid-1.4.1/repid/data/_key.py
+-rw-r--r--   0        0        0     5510 2023-07-01 09:57:07.329157 repid-1.4.1/repid/data/_parameters.py
+-rw-r--r--   0        0        0       95 2023-07-01 09:57:07.329157 repid-1.4.1/repid/data/priorities.py
+-rw-r--r--   0        0        0     3859 2023-07-01 09:57:07.329157 repid-1.4.1/repid/data/protocols.py
+-rw-r--r--   0        0        0     3270 2023-07-01 09:57:07.329157 repid-1.4.1/repid/health_check_server.py
+-rw-r--r--   0        0        0     7426 2023-07-01 09:57:07.333157 repid-1.4.1/repid/job.py
+-rw-r--r--   0        0        0      546 2023-07-01 09:57:07.333157 repid-1.4.1/repid/logger.py
+-rw-r--r--   0        0        0     1887 2023-07-01 09:57:07.333157 repid-1.4.1/repid/main.py
+-rw-r--r--   0        0        0      257 2023-07-01 09:57:07.333157 repid-1.4.1/repid/middlewares/__init__.py
+-rw-r--r--   0        0        0      347 2023-07-01 09:57:07.333157 repid-1.4.1/repid/middlewares/consts.py
+-rw-r--r--   0        0        0     3696 2023-07-01 09:57:07.333157 repid-1.4.1/repid/middlewares/middleware.py
+-rw-r--r--   0        0        0     3647 2023-07-01 09:57:07.333157 repid-1.4.1/repid/middlewares/wrapper.py
+-rw-r--r--   0        0        0        0 2023-07-01 09:57:07.333157 repid-1.4.1/repid/py.typed
+-rw-r--r--   0        0        0     1065 2023-07-01 09:57:07.333157 repid-1.4.1/repid/queue.py
+-rw-r--r--   0        0        0     1319 2023-07-01 09:57:07.333157 repid-1.4.1/repid/retry_policy.py
+-rw-r--r--   0        0        0     5022 2023-07-01 09:57:07.333157 repid-1.4.1/repid/router.py
+-rw-r--r--   0        0        0      520 2023-07-01 09:57:07.333157 repid-1.4.1/repid/serializer.py
+-rw-r--r--   0        0        0      845 2023-07-01 09:57:07.333157 repid-1.4.1/repid/testing/__init__.py
+-rw-r--r--   0        0        0     3184 2023-07-01 09:57:07.333157 repid-1.4.1/repid/testing/modifiers.py
+-rw-r--r--   0        0        0     6099 2023-07-01 09:57:07.333157 repid-1.4.1/repid/testing/plugin.py
+-rw-r--r--   0        0        0     4726 2023-07-01 09:57:07.333157 repid-1.4.1/repid/worker.py
+-rw-r--r--   0        0        0        0 2023-07-01 09:57:07.333157 repid-1.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     1145 2023-07-01 09:57:07.333157 repid-1.4.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-01 09:57:07.333157 repid-1.4.1/tests/integration/__init__.py
+-rw-r--r--   0        0        0     3241 2023-07-01 09:57:07.333157 repid-1.4.1/tests/integration/conftest.py
+-rw-r--r--   0        0        0     1337 2023-07-01 09:57:07.333157 repid-1.4.1/tests/integration/test_buckets.py
+-rw-r--r--   0        0        0     4335 2023-07-01 09:57:07.333157 repid-1.4.1/tests/integration/test_consumer.py
+-rw-r--r--   0        0        0     4003 2023-07-01 09:57:07.333157 repid-1.4.1/tests/integration/test_default_flow.py
+-rw-r--r--   0        0        0     1904 2023-07-01 09:57:07.333157 repid-1.4.1/tests/integration/test_no_messages_lost.py
+-rw-r--r--   0        0        0      431 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_actor.py
+-rw-r--r--   0        0        0     4620 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_config.py
+-rw-r--r--   0        0        0     2986 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_connection.py
+-rw-r--r--   0        0        0     3834 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_consumer.py
+-rw-r--r--   0        0        0     2835 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_consumer_abc.py
+-rw-r--r--   0        0        0    10230 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_default_data_models.py
+-rw-r--r--   0        0        0     2110 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_health_check_server.py
+-rw-r--r--   0        0        0     3004 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_hypothesis.py
+-rw-r--r--   0        0        0     3591 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_job.py
+-rw-r--r--   0        0        0     2298 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_json.py
+-rw-r--r--   0        0        0     1366 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_main.py
+-rw-r--r--   0        0        0     7842 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_middleware.py
+-rw-r--r--   0        0        0     1097 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_multiprocessing.py
+-rw-r--r--   0        0        0     7388 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_pydantic.py
+-rw-r--r--   0        0        0     3819 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_pytest_plugin.py
+-rw-r--r--   0        0        0      414 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_queue.py
+-rw-r--r--   0        0        0     3180 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_router.py
+-rw-r--r--   0        0        0      762 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_serializer.py
+-rw-r--r--   0        0        0     1893 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_utils.py
+-rw-r--r--   0        0        0     7633 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_worker.py
+-rw-r--r--   0        0        0     4108 1970-01-01 00:00:00.000000 repid-1.4.1/PKG-INFO
```

### Comparing `repid-1.4.0/LICENSE` & `repid-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/README.md` & `repid-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/pyproject.toml` & `repid-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "packaging>=22.0",
 ]
 description = "Repid framework: simple to use, fast to run and extensible to adopt job scheduler"
 dynamic = []
 name = "repid"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "1.4.0"
+version = "1.4.1"
 
 [project.license]
 text = "MIT"
 
 [project.entry-points.pytest11]
 repid = "repid.testing.plugin"
 
@@ -41,15 +41,15 @@
 amqp = [
     "aiormq<7.0.0,>=6.4.0",
 ]
 cron = [
     "croniter<2.0.0,>=1.3.4",
 ]
 pydantic = [
-    "pydantic>=2.0a1,<3.0.0",
+    "pydantic>=2.0.0,<3.0.0",
 ]
 redis = [
     "redis<5.0.0,>=4.3.3",
 ]
 test = [
     "pytest",
     "pytest-asyncio",
```

### Comparing `repid-1.4.0/repid/__init__.py` & `repid-1.4.1/repid/__init__.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/_asyncify.py` & `repid-1.4.1/repid/_asyncify.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/_processor.py` & `repid-1.4.1/repid/_processor.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/_runner.py` & `repid-1.4.1/repid/_runner.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/_utils/is_installed.py` & `repid-1.4.1/repid/_utils/is_installed.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/config.py` & `repid-1.4.1/repid/config.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/connection.py` & `repid-1.4.1/repid/connection.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/connections/__init__.py` & `repid-1.4.1/repid/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/connections/abc.py` & `repid-1.4.1/repid/connections/abc.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/connections/in_memory/bucket_broker.py` & `repid-1.4.1/repid/connections/in_memory/bucket_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/connections/in_memory/consumer.py` & `repid-1.4.1/repid/connections/in_memory/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/connections/in_memory/message_broker.py` & `repid-1.4.1/repid/connections/in_memory/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/connections/in_memory/utils.py` & `repid-1.4.1/repid/connections/in_memory/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/connections/rabbitmq/consumer.py` & `repid-1.4.1/repid/connections/rabbitmq/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/connections/rabbitmq/message_broker.py` & `repid-1.4.1/repid/connections/rabbitmq/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/connections/rabbitmq/utils.py` & `repid-1.4.1/repid/connections/rabbitmq/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/connections/redis/bucket_broker.py` & `repid-1.4.1/repid/connections/redis/bucket_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/connections/redis/consumer.py` & `repid-1.4.1/repid/connections/redis/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/connections/redis/message_broker.py` & `repid-1.4.1/repid/connections/redis/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/connections/redis/utils.py` & `repid-1.4.1/repid/connections/redis/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/converter.py` & `repid-1.4.1/repid/converter.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,34 +6,16 @@
 from warnings import warn
 
 from repid._utils import JSON_ENCODER, is_installed
 
 if is_installed("pydantic"):
     from pydantic import BaseModel, Field, create_model
 
-    if is_installed("pydantic", ">=2.0.0a1,<3.0.0"):
-        from pydantic import model_serializer, root_validator
-
-        # workaround until AnalysedType releases
-        class RootBaseModel(BaseModel):  # pragma: no cover
-            @root_validator(pre=True)
-            @classmethod
-            def populate_root(cls, values: Any) -> dict:
-                return {"root": values}
-
-            @model_serializer(mode="wrap")
-            def _serialize(self, handler, info):  # type: ignore[no-untyped-def]
-                data = handler(self)
-                if info.mode == "json":
-                    return data["root"]
-                return data
-
-            @classmethod
-            def model_modify_json_schema(cls, json_schema):  # type: ignore[no-untyped-def]
-                return json_schema["properties"]["root"]
+    if is_installed("pydantic", ">=2.0.0,<3.0.0"):
+        from pydantic import RootModel
 
 
 FnR = TypeVar("FnR", contravariant=True)
 Params = Tuple[List, Dict]
 
 
 class ConverterT(Protocol[FnR]):
@@ -45,15 +27,15 @@
 
     def convert_outputs(self, data: FnR) -> str:
         ...
 
 
 class DefaultConverter:
     def __new__(cls, fn: Callable[..., Coroutine[Any, Any, FnR]]) -> ConverterT[FnR]:  # type: ignore[misc]
-        if is_installed("pydantic", ">=2.0.0a1,<3.0.0"):
+        if is_installed("pydantic", ">=2.0.0,<3.0.0"):
             return PydanticConverter(fn)
         if is_installed("pydantic", ">=1.0.0,<2.0.0"):
             return PydanticV1Converter(fn)
         return BasicConverter(fn)
 
     # pretend to be an implementation of ConverterT
     def __init__(self, fn: Callable[..., Coroutine[Any, Any, FnR]]) -> None:
@@ -151,15 +133,15 @@
                     signature.return_annotation,
                 )
 
     @staticmethod
     def _generate_output_model(fn_name: str, return_annotation: Any) -> BaseModel:
         return create_model(  # type: ignore[return-value]
             f"{fn_name}_output_repid_model",
-            __base__=RootBaseModel,
+            __base__=RootModel,
             root=(return_annotation, Field()),
         )
 
     def convert_inputs(self, data: str) -> Params:
         loaded = dict(self.input_pydantic_model.model_validate_json(data))
 
         if self.args:
```

### Comparing `repid-1.4.0/repid/data/_buckets.py` & `repid-1.4.1/repid/data/_buckets.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/data/_key.py` & `repid-1.4.1/repid/data/_key.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/data/_parameters.py` & `repid-1.4.1/repid/data/_parameters.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/data/protocols.py` & `repid-1.4.1/repid/data/protocols.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/health_check_server.py` & `repid-1.4.1/repid/health_check_server.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/job.py` & `repid-1.4.1/repid/job.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/logger.py` & `repid-1.4.1/repid/logger.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/main.py` & `repid-1.4.1/repid/main.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/middlewares/middleware.py` & `repid-1.4.1/repid/middlewares/middleware.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/middlewares/wrapper.py` & `repid-1.4.1/repid/middlewares/wrapper.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/queue.py` & `repid-1.4.1/repid/queue.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/retry_policy.py` & `repid-1.4.1/repid/retry_policy.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/router.py` & `repid-1.4.1/repid/router.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/serializer.py` & `repid-1.4.1/repid/_utils/json_encoder.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+import json
 from dataclasses import asdict, is_dataclass
-from typing import Any, Protocol
+from datetime import date, datetime, time, timedelta
+from typing import Any
 
-from repid._utils import JSON_ENCODER, is_installed
+from repid._utils.is_installed import is_installed
 
-if PYDANTIC_IMPORTED := is_installed("pydantic"):
-    import pydantic
+if is_installed("pydantic"):
+    from pydantic import BaseModel
 
-    PYDANTIC_V2 = is_installed("pydantic", ">=2.0.0a1,<3.0.0")
 
+class _RepidJSONEncoder(json.JSONEncoder):
+    def default(self, obj: Any) -> Any:
+        if isinstance(obj, (datetime, date, time)):
+            return obj.isoformat()
+        if isinstance(obj, timedelta):
+            return obj.total_seconds()
+        if is_dataclass(obj) and not isinstance(obj, type):
+            return asdict(obj)
+        if is_installed("pydantic") and isinstance(obj, BaseModel):
+            if is_installed("pydantic", ">=2.0.0,<3.0.0"):
+                return obj.model_dump(mode="json")
+            return obj.dict()  # pragma: no cover
+        # Let the base class default method raise the TypeError
+        return json.JSONEncoder.default(self, obj)  # pragma: no cover
 
-class SerializerT(Protocol):
-    def __call__(self, data: Any) -> str:
-        ...
 
-
-def default_serializer(data: Any) -> str:
-    if PYDANTIC_IMPORTED and isinstance(data, pydantic.BaseModel):
-        if PYDANTIC_V2:
-            return data.model_dump_json()
-        return data.json()  # pragma: no cover
-    if is_dataclass(data) and not isinstance(data, type):
-        return JSON_ENCODER.encode(asdict(data))
-    return JSON_ENCODER.encode(data)
+JSON_ENCODER = _RepidJSONEncoder(separators=(",", ":"))
```

### Comparing `repid-1.4.0/repid/testing/__init__.py` & `repid-1.4.1/repid/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/testing/modifiers.py` & `repid-1.4.1/repid/testing/modifiers.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/testing/plugin.py` & `repid-1.4.1/repid/testing/plugin.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/repid/worker.py` & `repid-1.4.1/repid/worker.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/tests/conftest.py` & `repid-1.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/tests/integration/conftest.py` & `repid-1.4.1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/tests/integration/test_buckets.py` & `repid-1.4.1/tests/integration/test_buckets.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/tests/integration/test_consumer.py` & `repid-1.4.1/tests/integration/test_consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/tests/integration/test_default_flow.py` & `repid-1.4.1/tests/integration/test_default_flow.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/tests/integration/test_no_messages_lost.py` & `repid-1.4.1/tests/integration/test_no_messages_lost.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/tests/test_config.py` & `repid-1.4.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/tests/test_connection.py` & `repid-1.4.1/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/tests/test_consumer.py` & `repid-1.4.1/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/tests/test_consumer_abc.py` & `repid-1.4.1/tests/test_consumer_abc.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/tests/test_default_data_models.py` & `repid-1.4.1/tests/test_default_data_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,23 +200,23 @@
     ("bucket", "data", "timestamp", "ttl", "expected_encoded"),
     [
         (
             ArgsBucket,
             "some_data",
             datetime(2022, 1, 1),
             timedelta(days=1),
-            '{"data":"some_data","timestamp":"2022-01-01T00:00:00","ttl":"86400.0"}',
+            '{"data":"some_data","timestamp":"2022-01-01T00:00:00","ttl":86400.0}',
         ),
         (
             ResultBucket,
             "some_data",
             datetime(2022, 1, 1),
             timedelta(days=1),
             '{"data":"some_data","started_when":1,"finished_when":2,'
-            '"success":true,"exception":null,"timestamp":"2022-01-01T00:00:00","ttl":"86400.0"}',
+            '"success":true,"exception":null,"timestamp":"2022-01-01T00:00:00","ttl":86400.0}',
         ),
     ],
 )
 def test_bucket_encode_decode(
     bucket: type[BucketT | ResultBucketT],
     data: str,
     timestamp: datetime,
```

### Comparing `repid-1.4.0/tests/test_health_check_server.py` & `repid-1.4.1/tests/test_health_check_server.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/tests/test_hypothesis.py` & `repid-1.4.1/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/tests/test_job.py` & `repid-1.4.1/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/tests/test_main.py` & `repid-1.4.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/tests/test_middleware.py` & `repid-1.4.1/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/tests/test_multiprocessing.py` & `repid-1.4.1/tests/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/tests/test_pydantic.py` & `repid-1.4.1/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/tests/test_pytest_plugin.py` & `repid-1.4.1/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/tests/test_router.py` & `repid-1.4.1/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/tests/test_serializer.py` & `repid-1.4.1/tests/test_serializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,8 +26,8 @@
         args=MyData(
             a=123,
             b=567.34,
             c=datetime(2020, 1, 1, 12, 0, 0),
             d=timedelta(days=2, hours=3),
         ),
     )
-    assert j.args == '{"a":123,"b":567.34,"c":"2020-01-01T12:00:00","d":"183600.0"}'
+    assert j.args == '{"a":123,"b":567.34,"c":"2020-01-01T12:00:00","d":183600.0}'
```

### Comparing `repid-1.4.0/tests/test_utils.py` & `repid-1.4.1/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 def test_is_imported(dependency: str, result: bool) -> None:
     assert is_installed(dependency) is result
 
 
 @pytest.mark.parametrize(
     ("dependency", "constraints", "result"),
     [
-        ("pydantic", ">=2.0.0a1,<3.0.0", True),
+        ("pydantic", ">=2.0.0,<3.0.0", True),
         ("pydantic", ">=1.0.0", True),
         ("pydantic", ">=3.0.0", False),
         ("pytest", ">=0.0.0,<100.0.0", True),
         ("flask", ">0.0.0,<2.0.0", False),
         ("blabla", ">0.0.0,<2.0.0", False),
     ],
 )
```

### Comparing `repid-1.4.0/tests/test_worker.py` & `repid-1.4.1/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.0/PKG-INFO` & `repid-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repid
-Version: 1.4.0
+Version: 1.4.1
 Summary: Repid framework: simple to use, fast to run and extensible to adopt job scheduler
 Author-Email: aleksul <me@aleksul.space>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -19,15 +19,15 @@
 Project-URL: Repository, https://github.com/aleksul/repid
 Project-URL: Tracker, https://github.com/aleksul/repid/issues
 Requires-Python: >=3.8
 Requires-Dist: typing-extensions<5.0.0,>=4.3.0; python_version < "3.10"
 Requires-Dist: packaging>=22.0
 Requires-Dist: aiormq<7.0.0,>=6.4.0; extra == "amqp"
 Requires-Dist: croniter<2.0.0,>=1.3.4; extra == "cron"
-Requires-Dist: pydantic<3.0.0,>=2.0a1; extra == "pydantic"
+Requires-Dist: pydantic<3.0.0,>=2.0.0; extra == "pydantic"
 Requires-Dist: redis<5.0.0,>=4.3.3; extra == "redis"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Provides-Extra: amqp
 Provides-Extra: cron
 Provides-Extra: pydantic
 Provides-Extra: redis
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: repid Version: 1.4.0 Summary: Repid framework:
+Metadata-Version: 2.1 Name: repid Version: 1.4.1 Summary: Repid framework:
 simple to use, fast to run and extensible to adopt job scheduler Author-Email:
 aleksul
 aleksul.space> License: MIT Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -11,15 +11,15 @@
 :: Typed Project-URL: Documentation, https://repid.aleksul.space Project-URL:
 Funding, https://github.com/sponsors/aleksul Project-URL: Repository, https://
 github.com/aleksul/repid Project-URL: Tracker, https://github.com/aleksul/
 repid/issues Requires-Python: >=3.8 Requires-Dist: typing-
 extensions<5.0.0,>=4.3.0; python_version < "3.10" Requires-Dist:
 packaging>=22.0 Requires-Dist: aiormq<7.0.0,>=6.4.0; extra == "amqp" Requires-
 Dist: croniter<2.0.0,>=1.3.4; extra == "cron" Requires-Dist:
-pydantic<3.0.0,>=2.0a1; extra == "pydantic" Requires-Dist: redis<5.0.0,>=4.3.3;
+pydantic<3.0.0,>=2.0.0; extra == "pydantic" Requires-Dist: redis<5.0.0,>=4.3.3;
 extra == "redis" Requires-Dist: pytest; extra == "test" Requires-Dist: pytest-
 asyncio; extra == "test" Provides-Extra: amqp Provides-Extra: cron Provides-
 Extra: pydantic Provides-Extra: redis Provides-Extra: test Description-Content-
 Type: text/markdown   # repid [Repid's_logo] [![PyPI version](https://
 img.shields.io/pypi/v/repid.svg)](https://pypi.org/project/repid/) [![codecov]
 (https://codecov.io/gh/aleksul/repid/branch/main/graph/
 badge.svg?token=IP3Z1VXB1G)](https://codecov.io/gh/aleksul/repid) [![Tests]
```

