# Comparing `tmp/flytekit-1.7.1b0.tar.gz` & `tmp/flytekit-1.7.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekit-1.7.1b0.tar", last modified: Fri Jun 16 18:14:08 2023, max compression
+gzip compressed data, was "flytekit-1.7.1b1.tar", last modified: Tue Jun 27 22:00:44 2023, max compression
```

## Comparing `flytekit-1.7.1b0.tar` & `flytekit-1.7.1b1.tar`

### file list

```diff
@@ -1,254 +1,257 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.246565 flytekit-1.7.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-16 18:14:08.246565 flytekit-1.7.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.210566 flytekit-1.7.1b0/flytekit/
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-06-16 18:14:06.000000 flytekit-1.7.1b0/flytekit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.218566 flytekit-1.7.1b0/flytekit/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23210 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/bin/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.218566 flytekit-1.7.1b0/flytekit/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.218566 flytekit-1.7.1b0/flytekit/clients/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/auth/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/auth/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/auth/default_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/auth/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/auth/token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/friendly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.218566 flytekit-1.7.1b0/flytekit/clients/grpc_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/grpc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/grpc_utils/auth_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28489 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clients/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.218566 flytekit-1.7.1b0/flytekit/clis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.218566 flytekit-1.7.1b0/flytekit/clis/flyte_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/flyte_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/flyte_cli/example.config
--rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/flyte_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.218566 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/launchplan.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/pyflyte.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/register.py
--rw-r--r--   0 runner    (1001) docker     (123)    31991 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/clis/sdk_in_container/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.222566 flytekit-1.7.1b0/flytekit/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    36185 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/configuration/default_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/configuration/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/configuration/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/configuration/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.226566 flytekit-1.7.1b0/flytekit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/base_sql_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    31002 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/base_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/class_based_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    36384 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/data_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/dynamic_workflow_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    18343 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/map_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/mock_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/node_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/pod_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    46442 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/promise.py
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/python_auto_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/python_customized_container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/python_function_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/reference_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/shim_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/tracked_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    77560 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/type_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/type_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    41135 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.230566 flytekit-1.7.1b0/flytekit/deck/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/deck/deck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.230566 flytekit-1.7.1b0/flytekit/deck/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/deck/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/deck/html/template.html
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/deck/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.230566 flytekit-1.7.1b0/flytekit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/exceptions/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/exceptions/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/exceptions/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.230566 flytekit-1.7.1b0/flytekit/extend/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.230566 flytekit-1.7.1b0/flytekit/extend/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extend/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extend/backend/agent_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extend/backend/base_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.230566 flytekit-1.7.1b0/flytekit/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/cloud_pickle_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.230566 flytekit-1.7.1b0/flytekit/extras/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/pytorch/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/pytorch/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.230566 flytekit-1.7.1b0/flytekit/extras/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/sklearn/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.230566 flytekit-1.7.1b0/flytekit/extras/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/sqlite3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/sqlite3/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.230566 flytekit-1.7.1b0/flytekit/extras/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/tasks/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.234566 flytekit-1.7.1b0/flytekit/extras/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/tensorflow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/extras/tensorflow/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.234566 flytekit-1.7.1b0/flytekit/image_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/image_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/image_spec/image_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.234566 flytekit-1.7.1b0/flytekit/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/interaction/parse_stdin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.234566 flytekit-1.7.1b0/flytekit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/interfaces/cli_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/interfaces/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.234566 flytekit-1.7.1b0/flytekit/interfaces/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/interfaces/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/interfaces/stats/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/interfaces/stats/taggable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.234566 flytekit-1.7.1b0/flytekit/lazy_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/lazy_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/lazy_import/lazy_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.238566 flytekit-1.7.1b0/flytekit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.238566 flytekit-1.7.1b0/flytekit/models/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/admin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/admin/task_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/admin/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/array_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.238566 flytekit-1.7.1b0/flytekit/models/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/core/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/core/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/core/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/dynamic_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    25993 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/matchable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/node_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/presto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/qubole.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/models/workflow_closure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.242565 flytekit-1.7.1b0/flytekit/remote/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/remote/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/remote/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/remote/executions.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/remote/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/remote/lazy_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    87310 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/remote/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/remote/remote_callable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.242565 flytekit-1.7.1b0/flytekit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.242565 flytekit-1.7.1b0/flytekit/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/tools/fast_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/tools/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/tools/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/tools/module_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/tools/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/tools/script_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/tools/serialize_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/tools/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/tools/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.242565 flytekit-1.7.1b0/flytekit/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.242565 flytekit-1.7.1b0/flytekit/types/directory/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/directory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/directory/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.242565 flytekit-1.7.1b0/flytekit/types/file/
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.246565 flytekit-1.7.1b0/flytekit/types/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/numpy/ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.246565 flytekit-1.7.1b0/flytekit/types/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/pickle/pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.246565 flytekit-1.7.1b0/flytekit/types/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/schema/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/schema/types_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.246565 flytekit-1.7.1b0/flytekit/types/structured/
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/structured/basic_dfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/structured/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    44541 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit/types/structured/structured_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.218566 flytekit-1.7.1b0/flytekit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-16 18:14:08.000000 flytekit-1.7.1b0/flytekit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-06-16 18:14:08.000000 flytekit-1.7.1b0/flytekit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:14:08.000000 flytekit-1.7.1b0/flytekit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-16 18:14:08.000000 flytekit-1.7.1b0/flytekit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-16 18:14:08.000000 flytekit-1.7.1b0/flytekit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 18:14:08.000000 flytekit-1.7.1b0/flytekit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:08.246565 flytekit-1.7.1b0/flytekit_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit_scripts/Readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit_scripts/flytekit_build_image.sh
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/flytekit_scripts/flytekit_venv
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-16 18:13:54.000000 flytekit-1.7.1b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-16 18:14:08.246565 flytekit-1.7.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-16 18:14:06.000000 flytekit-1.7.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.916439 flytekit-1.7.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-27 22:00:44.916439 flytekit-1.7.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.896438 flytekit-1.7.1b1/flytekit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-27 22:00:42.000000 flytekit-1.7.1b1/flytekit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.896438 flytekit-1.7.1b1/flytekit/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23210 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/bin/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.896438 flytekit-1.7.1b1/flytekit/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.900438 flytekit-1.7.1b1/flytekit/clients/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/auth/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/auth/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/auth/default_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/auth/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/auth/token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/friendly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.900438 flytekit-1.7.1b1/flytekit/clients/grpc_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/grpc_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/grpc_utils/auth_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28489 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clients/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.900438 flytekit-1.7.1b1/flytekit/clis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.900438 flytekit-1.7.1b1/flytekit/clis/flyte_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/flyte_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/flyte_cli/example.config
+-rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/flyte_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.900438 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/launchplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/pyflyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31991 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/clis/sdk_in_container/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.900438 flytekit-1.7.1b1/flytekit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    36420 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/configuration/default_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/configuration/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/configuration/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/configuration/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.904439 flytekit-1.7.1b1/flytekit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/base_sql_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31360 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/class_based_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36384 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/data_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/dynamic_workflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18343 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18295 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/map_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/mock_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/node_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/pod_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41843 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/promise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/python_auto_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/python_customized_container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/python_function_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/reference_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/shim_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/tracked_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78535 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/type_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/type_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38243 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.904439 flytekit-1.7.1b1/flytekit/deck/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/deck/deck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.904439 flytekit-1.7.1b1/flytekit/deck/html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/deck/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/deck/html/template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/deck/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.904439 flytekit-1.7.1b1/flytekit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/exceptions/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/exceptions/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/exceptions/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/extend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/extend/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extend/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extend/backend/agent_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extend/backend/base_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/cloud_pickle_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/extras/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/pytorch/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/pytorch/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/extras/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/sklearn/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/extras/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/sqlite3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/sqlite3/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/extras/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/tasks/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/extras/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/tensorflow/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/extras/tensorflow/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/image_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/image_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/image_spec/image_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/interaction/parse_stdin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/interfaces/cli_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/interfaces/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/interfaces/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/interfaces/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/interfaces/stats/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/interfaces/stats/taggable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.908439 flytekit-1.7.1b1/flytekit/lazy_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/lazy_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/lazy_import/lazy_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.912439 flytekit-1.7.1b1/flytekit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.912439 flytekit-1.7.1b1/flytekit/models/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/admin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/admin/task_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/admin/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/array_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.912439 flytekit-1.7.1b1/flytekit/models/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/core/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/core/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/core/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/dynamic_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25993 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/matchable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/node_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/presto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/qubole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/models/workflow_closure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.912439 flytekit-1.7.1b1/flytekit/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/remote/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/remote/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/remote/executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/remote/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/remote/lazy_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87310 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/remote/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/remote/remote_callable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.912439 flytekit-1.7.1b1/flytekit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.912439 flytekit-1.7.1b1/flytekit/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/tools/fast_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/tools/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/tools/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/tools/module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/tools/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/tools/script_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/tools/serialize_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/tools/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/tools/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.912439 flytekit-1.7.1b1/flytekit/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.912439 flytekit-1.7.1b1/flytekit/types/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/directory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/directory/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.916439 flytekit-1.7.1b1/flytekit/types/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.916439 flytekit-1.7.1b1/flytekit/types/iterator/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/iterator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/iterator/iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.916439 flytekit-1.7.1b1/flytekit/types/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/numpy/ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.916439 flytekit-1.7.1b1/flytekit/types/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/pickle/pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.916439 flytekit-1.7.1b1/flytekit/types/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/schema/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/schema/types_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.916439 flytekit-1.7.1b1/flytekit/types/structured/
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/structured/basic_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/structured/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44541 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit/types/structured/structured_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.896438 flytekit-1.7.1b1/flytekit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-27 22:00:44.000000 flytekit-1.7.1b1/flytekit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-06-27 22:00:44.000000 flytekit-1.7.1b1/flytekit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 22:00:44.000000 flytekit-1.7.1b1/flytekit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-27 22:00:44.000000 flytekit-1.7.1b1/flytekit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-27 22:00:44.000000 flytekit-1.7.1b1/flytekit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 22:00:44.000000 flytekit-1.7.1b1/flytekit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:44.916439 flytekit-1.7.1b1/flytekit_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit_scripts/Readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit_scripts/flytekit_build_image.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/flytekit_scripts/flytekit_venv
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-27 22:00:35.000000 flytekit-1.7.1b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-27 22:00:44.916439 flytekit-1.7.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-27 22:00:42.000000 flytekit-1.7.1b1/setup.py
```

### Comparing `flytekit-1.7.1b0/LICENSE` & `flytekit-1.7.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/MANIFEST.in` & `flytekit-1.7.1b1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/PKG-INFO` & `flytekit-1.7.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.7.1b0
+Version: 1.7.1b1
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.7.1b0 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.7.1b1 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.7.1b0/README.md` & `flytekit-1.7.1b1/README.md`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/__init__.py` & `flytekit-1.7.1b1/flytekit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,23 +231,23 @@
 from flytekit.loggers import logger
 from flytekit.models.common import Annotations, AuthRole, Labels
 from flytekit.models.core.execution import WorkflowExecutionPhase
 from flytekit.models.core.types import BlobType
 from flytekit.models.documentation import Description, Documentation, SourceCode
 from flytekit.models.literals import Blob, BlobMetadata, Literal, Scalar
 from flytekit.models.types import LiteralType
-from flytekit.types import directory, file
+from flytekit.types import directory, file, iterator
 from flytekit.types.structured.structured_dataset import (
     StructuredDataset,
     StructuredDatasetFormat,
     StructuredDatasetTransformerEngine,
     StructuredDatasetType,
 )
 
-__version__ = "1.7.1b0"
+__version__ = "1.7.1b1"
 
 
 def current_context() -> ExecutionParameters:
     """
     Use this method to get a handle of specific parameters available in a flyte task.
 
     Usage
```

### Comparing `flytekit-1.7.1b0/flytekit/bin/entrypoint.py` & `flytekit-1.7.1b1/flytekit/bin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clients/auth/auth_client.py` & `flytekit-1.7.1b1/flytekit/clients/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clients/auth/authenticator.py` & `flytekit-1.7.1b1/flytekit/clients/auth/authenticator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clients/auth/keyring.py` & `flytekit-1.7.1b1/flytekit/clients/auth/keyring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clients/auth/token_client.py` & `flytekit-1.7.1b1/flytekit/clients/auth/token_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clients/auth_helper.py` & `flytekit-1.7.1b1/flytekit/clients/auth_helper.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clients/friendly.py` & `flytekit-1.7.1b1/flytekit/clients/friendly.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clients/grpc_utils/auth_interceptor.py` & `flytekit-1.7.1b1/flytekit/clients/grpc_utils/auth_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py` & `flytekit-1.7.1b1/flytekit/clients/grpc_utils/wrap_exception_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clients/helpers.py` & `flytekit-1.7.1b1/flytekit/clients/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clients/raw.py` & `flytekit-1.7.1b1/flytekit/clients/raw.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clis/flyte_cli/main.py` & `flytekit-1.7.1b1/flytekit/clis/flyte_cli/main.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clis/helpers.py` & `flytekit-1.7.1b1/flytekit/clis/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/backfill.py` & `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/build.py` & `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/build.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/constants.py` & `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/helpers.py` & `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/init.py` & `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/init.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/launchplan.py` & `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/launchplan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/metrics.py` & `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/metrics.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/package.py` & `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/package.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/pyflyte.py` & `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/pyflyte.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/register.py` & `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/register.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/run.py` & `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/run.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/serialize.py` & `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/serialize.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 @system_entry_point
 def serialize_all(
     pkgs: typing.List[str] = None,
     local_source_root: typing.Optional[str] = None,
     folder: typing.Optional[str] = None,
     mode: typing.Optional[SerializationMode] = None,
-    image: typing.Optional[str] = None,
+    image_config: typing.Optional[ImageConfig] = None,
     flytekit_virtualenv_root: typing.Optional[str] = None,
     python_interpreter: typing.Optional[str] = None,
     config_file: typing.Optional[str] = None,
 ):
     """
     This function will write to the folder specified the following protobuf types ::
         flyteidl.admin.launch_plan_pb2.LaunchPlan
@@ -45,40 +45,48 @@
 
     See :py:class:`flytekit.models.core.identifier.ResourceType` to match the trailing index in the file name with the
     entity type.
     :param pkgs: Dot-delimited Python packages/subpackages to look into for serialization.
     :param local_source_root: Where to start looking for the code.
     :param folder: Where to write the output protobuf files
     :param mode: Regular vs fast
-    :param image: The fully qualified and versioned default image to use
+    :param image_config: ImageConfig object to use
     :param flytekit_virtualenv_root: The full path of the virtual env in the container.
     """
 
     if not (mode == SerializationMode.DEFAULT or mode == SerializationMode.FAST):
         raise AssertionError(f"Unrecognized serialization mode: {mode}")
 
     serialization_settings = SerializationSettings(
-        image_config=ImageConfig.auto(config_file, img_name=image),
+        image_config=image_config or ImageConfig.auto(config_file),
         fast_serialization_settings=FastSerializationSettings(
             enabled=mode == SerializationMode.FAST,
             # TODO: if we want to move the destination dir as a serialization argument, we should initialize it here
         ),
         flytekit_virtualenv_root=flytekit_virtualenv_root,
         python_interpreter=python_interpreter,
     )
 
     serialize_to_folder(pkgs, serialization_settings, local_source_root, folder)
 
 
 @click.group("serialize", cls=click.RichGroup)
 @click.option(
+    "-i",
     "--image",
+    "image_config",
     required=False,
-    default=lambda: os.environ.get("FLYTE_INTERNAL_IMAGE", ""),
-    help="Text tag, for example ``somedocker.com/myimage:someversion123``",
+    multiple=True,
+    type=click.UNPROCESSED,
+    callback=ImageConfig.validate_image,
+    help="A fully qualified tag for an docker image, for example ``somedocker.com/myimage:someversion123``. This is a "
+    "multi-option and can be of the form ``--image xyz.io/docker:latest"
+    " --image my_image=xyz.io/docker2:latest``. Note, the ``name=image_uri``. The name is optional, if not "
+    "provided the image will be used as the default image. All the names have to be unique, and thus "
+    "there can only be one ``--image`` option with no name.",
 )
 @click.option(
     "--local-source-root",
     required=False,
     default=lambda: os.getcwd(),
     help="Root dir for Python code containing workflow definitions to operate on when not the current working directory. "
     "Optional when running ``pyflyte serialize`` in out-of-container-mode and your code lies outside of your working directory.",
@@ -95,25 +103,27 @@
     required=False,
     help="DEPRECATED: This flag is ignored! This is the root of the flytekit virtual env in your container. "
     "The reason it needs to be a separate option is because this pyflyte utility cannot know where flytekit is "
     "installed inside your container. Required for running `pyflyte serialize` in out of container mode when "
     "your container installs the flytekit virtualenv outside of the default `/opt/venv`",
 )
 @click.pass_context
-def serialize(ctx, image, local_source_root, in_container_config_path, in_container_virtualenv_root):
+def serialize(
+    ctx, image_config: ImageConfig, local_source_root, in_container_config_path, in_container_virtualenv_root
+):
     """
     This command produces protobufs for tasks and templates.
     For tasks, one pb file is produced for each task, representing one TaskTemplate object.
     For workflows, one pb file is produced for each workflow, representing a WorkflowClosure object. The closure
     object contains the WorkflowTemplate, along with the relevant tasks for that workflow. In lieu of Admin,
     this serialization step will set the URN of the tasks to the fully qualified name of the task function.
     """
-    ctx.obj[CTX_IMAGE] = image
+    ctx.obj[CTX_IMAGE] = image_config
     ctx.obj[CTX_LOCAL_SRC_ROOT] = local_source_root
-    click.echo("Serializing Flyte elements with image {}".format(image))
+    click.echo(f"Serializing Flyte elements with image {image_config}")
 
     if in_container_virtualenv_root:
         ctx.obj[CTX_FLYTEKIT_VIRTUALENV_ROOT] = in_container_virtualenv_root
         ctx.obj[CTX_PYTHON_INTERPRETER] = os.path.join(in_container_virtualenv_root, "/bin/python3")
     else:
         # For in container serialize we make sure to never accept an override the entrypoint path and determine it here
         # instead.
@@ -137,15 +147,15 @@
     pkgs = ctx.obj[CTX_PACKAGES]
     dir = ctx.obj[CTX_LOCAL_SRC_ROOT]
     serialize_all(
         pkgs,
         dir,
         folder,
         SerializationMode.DEFAULT,
-        image=ctx.obj[CTX_IMAGE],
+        image_config=ctx.obj[CTX_IMAGE],
         flytekit_virtualenv_root=ctx.obj[CTX_FLYTEKIT_VIRTUALENV_ROOT],
         python_interpreter=ctx.obj[CTX_PYTHON_INTERPRETER],
         config_file=ctx.obj.get(constants.CTX_CONFIG_FILE, None),
     )
 
 
 @click.group("fast", cls=click.RichGroup)
@@ -176,15 +186,15 @@
     pkgs = ctx.obj[CTX_PACKAGES]
     dir = ctx.obj[CTX_LOCAL_SRC_ROOT]
     serialize_all(
         pkgs,
         dir,
         folder,
         SerializationMode.FAST,
-        image=ctx.obj[CTX_IMAGE],
+        image_config=ctx.obj[CTX_IMAGE],
         flytekit_virtualenv_root=ctx.obj[CTX_FLYTEKIT_VIRTUALENV_ROOT],
         python_interpreter=ctx.obj[CTX_PYTHON_INTERPRETER],
         config_file=ctx.obj.get(constants.CTX_CONFIG_FILE, None),
     )
 
 
 fast.add_command(fast_workflows)
```

### Comparing `flytekit-1.7.1b0/flytekit/clis/sdk_in_container/serve.py` & `flytekit-1.7.1b1/flytekit/clis/sdk_in_container/serve.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/configuration/__init__.py` & `flytekit-1.7.1b1/flytekit/configuration/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,14 +278,17 @@
                     f"Only one default image can be specified. Received multiple {default_image} & {img} for {param}"
                 )
             if img.name == DEFAULT_IMAGE_NAME:
                 default_image = img
             else:
                 images.append(img)
 
+        if default_image is None:
+            default_image_str = os.environ.get("FLYTE_INTERNAL_IMAGE", DefaultImages.default_image())
+            default_image = Image.look_up_image_info(DEFAULT_IMAGE_NAME, default_image_str, False)
         return ImageConfig.create_from(default_image=default_image, other_images=images)
 
     @classmethod
     def create_from(
         cls, default_image: Optional[Image], other_images: typing.Optional[typing.List[Image]] = None
     ) -> ImageConfig:
         if default_image and not isinstance(default_image, Image):
```

### Comparing `flytekit-1.7.1b0/flytekit/configuration/default_images.py` & `flytekit-1.7.1b1/flytekit/configuration/default_images.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/configuration/feature_flags.py` & `flytekit-1.7.1b1/flytekit/configuration/feature_flags.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/configuration/file.py` & `flytekit-1.7.1b1/flytekit/configuration/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/configuration/internal.py` & `flytekit-1.7.1b1/flytekit/configuration/internal.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/annotation.py` & `flytekit-1.7.1b1/flytekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/base_sql_task.py` & `flytekit-1.7.1b1/flytekit/core/base_sql_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/base_task.py` & `flytekit-1.7.1b1/flytekit/core/base_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -505,14 +505,15 @@
         * ``Literal Map`` is returned when the task returns either one more outputs in the declaration. Individual outputs
           may be none
         * ``DynamicJobSpec`` is returned when a dynamic workflow is executed
         """
 
         # Invoked before the task is executed
         new_user_params = self.pre_execute(ctx.user_space_params)
+        from flytekit.deck.deck import _output_deck
 
         # Create another execution context with the new user params, but let's keep the same working dir
         with FlyteContextManager.with_context(
             ctx.with_execution_state(
                 cast(ExecutionState, ctx.execution_state).with_params(user_space_params=new_user_params)
             )
             # type: ignore
@@ -597,14 +598,18 @@
                 for k, v in native_inputs.items():
                     input_deck.append(TypeEngine.to_html(ctx, v, self.get_type_for_input_var(k, v)))
 
                 output_deck = Deck(OUTPUT)
                 for k, v in native_outputs_as_map.items():
                     output_deck.append(TypeEngine.to_html(ctx, v, self.get_type_for_output_var(k, v)))
 
+                if ctx.execution_state and ctx.execution_state.mode == ExecutionState.Mode.LOCAL_WORKFLOW_EXECUTION:
+                    # When we run the workflow remotely, flytekit outputs decks at the end of _dispatch_execute
+                    _output_deck(self.name.split(".")[-1], new_user_params)
+
             outputs_literal_map = _literal_models.LiteralMap(literals=literals)
             # After the execute has been successfully completed
             return outputs_literal_map
 
     def pre_execute(self, user_params: Optional[ExecutionParameters]) -> Optional[ExecutionParameters]:  # type: ignore
         """
         This is the method that will be invoked directly before executing the task method and before all the inputs
```

### Comparing `flytekit-1.7.1b0/flytekit/core/checkpointer.py` & `flytekit-1.7.1b1/flytekit/core/checkpointer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/class_based_resolver.py` & `flytekit-1.7.1b1/flytekit/core/class_based_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/condition.py` & `flytekit-1.7.1b1/flytekit/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/constants.py` & `flytekit-1.7.1b1/flytekit/core/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/container_task.py` & `flytekit-1.7.1b1/flytekit/core/container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/context_manager.py` & `flytekit-1.7.1b1/flytekit/core/context_manager.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/data_persistence.py` & `flytekit-1.7.1b1/flytekit/core/data_persistence.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/docstring.py` & `flytekit-1.7.1b1/flytekit/core/docstring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/dynamic_workflow_task.py` & `flytekit-1.7.1b1/flytekit/core/dynamic_workflow_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/gate.py` & `flytekit-1.7.1b1/flytekit/core/gate.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/interface.py` & `flytekit-1.7.1b1/flytekit/core/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/launch_plan.py` & `flytekit-1.7.1b1/flytekit/core/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/local_cache.py` & `flytekit-1.7.1b1/flytekit/core/local_cache.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/map_task.py` & `flytekit-1.7.1b1/flytekit/core/map_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from flytekit.core import tracker
 from flytekit.core.base_task import PythonTask, Task, TaskResolverMixin
 from flytekit.core.constants import SdkTaskType
 from flytekit.core.context_manager import ExecutionState, FlyteContext, FlyteContextManager
 from flytekit.core.interface import transform_interface_to_list_interface
 from flytekit.core.python_function_task import PythonFunctionTask, PythonInstanceTask
 from flytekit.core.tracker import TrackedInstance
+from flytekit.core.type_engine import UnionTransformer
 from flytekit.core.utils import timeit
 from flytekit.exceptions import scopes as exception_scopes
 from flytekit.models.array_job import ArrayJob
 from flytekit.models.interface import Variable
 from flytekit.models.task import Container, K8sPod, Sql
 from flytekit.tools.module_loader import load_object_from_module
 
@@ -69,25 +70,32 @@
                 pass
             else:
                 raise ValueError("Map tasks can only compose of PythonFuncton and PythonInstanceTasks currently")
 
         if len(actual_task.python_interface.outputs.keys()) > 1:
             raise ValueError("Map tasks only accept python function tasks with 0 or 1 outputs")
 
+        if (
+            min_success_ratio
+            and min_success_ratio != 1
+            and not UnionTransformer.is_optional_type(actual_task.python_interface.outputs["o0"])
+        ):
+            raise ValueError("Map tasks with min_success_ratio < 1 must have an optional output")
+
         self._bound_inputs: typing.Set[str] = set(bound_inputs) if bound_inputs else set()
         if self._partial:
             self._bound_inputs = set(self._partial.keywords.keys())
 
         collection_interface = transform_interface_to_list_interface(actual_task.python_interface, self._bound_inputs)
-        self._run_task: PythonFunctionTask = actual_task
+        self._run_task: typing.Union[PythonFunctionTask, PythonInstanceTask] = actual_task  # type: ignore
         if isinstance(actual_task, PythonInstanceTask):
             mod = actual_task.task_type
             f = actual_task.lhs
         else:
-            _, mod, f, _ = tracker.extract_task_module(actual_task.task_function)
+            _, mod, f, _ = tracker.extract_task_module(typing.cast(PythonFunctionTask, actual_task).task_function)
         h = hashlib.md5(collection_interface.__str__().encode("utf-8")).hexdigest()
         name = f"{mod}.map_{f}_{h}"
 
         self._cmd_prefix: typing.Optional[typing.List[str]] = None
         self._max_concurrency: typing.Optional[int] = concurrency
         self._min_success_ratio: typing.Optional[float] = min_success_ratio
         self._array_task_interface = actual_task.python_interface
@@ -164,15 +172,15 @@
     def get_custom(self, settings: SerializationSettings) -> Dict[str, Any]:
         return ArrayJob(parallelism=self._max_concurrency, min_success_ratio=self._min_success_ratio).to_dict()
 
     def get_config(self, settings: SerializationSettings) -> Optional[Dict[str, str]]:
         return self._run_task.get_config(settings)
 
     @property
-    def run_task(self) -> PythonFunctionTask:
+    def run_task(self) -> typing.Union[PythonFunctionTask, PythonInstanceTask]:
         return self._run_task
 
     def __call__(self, *args, **kwargs):
         """
         This call method modifies the kwargs and adds kwargs from partial.
         This is mostly done in the local_execute and compilation only.
         At runtime, the map_task is created with all the inputs filled in. to support this, we have modified
```

### Comparing `flytekit-1.7.1b0/flytekit/core/mock_stats.py` & `flytekit-1.7.1b1/flytekit/core/mock_stats.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/node.py` & `flytekit-1.7.1b1/flytekit/core/node.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/node_creation.py` & `flytekit-1.7.1b1/flytekit/core/node_creation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/notification.py` & `flytekit-1.7.1b1/flytekit/core/notification.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/pod_template.py` & `flytekit-1.7.1b1/flytekit/core/pod_template.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/promise.py` & `flytekit-1.7.1b1/flytekit/core/promise.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,29 +19,28 @@
 )
 from flytekit.core.interface import Interface
 from flytekit.core.node import Node
 from flytekit.core.type_engine import DictTransformer, ListTransformer, TypeEngine, TypeTransformerFailedError
 from flytekit.exceptions import user as _user_exceptions
 from flytekit.loggers import logger
 from flytekit.models import interface as _interface_models
-from flytekit.models import literals as _literal_models
 from flytekit.models import literals as _literals_models
 from flytekit.models import types as _type_models
 from flytekit.models import types as type_models
 from flytekit.models.core import workflow as _workflow_model
 from flytekit.models.literals import Primitive
 from flytekit.models.types import SimpleType
 
 
 def translate_inputs_to_literals(
     ctx: FlyteContext,
     incoming_values: Dict[str, Any],
     flyte_interface_types: Dict[str, _interface_models.Variable],
     native_types: Dict[str, type],
-) -> Dict[str, _literal_models.Literal]:
+) -> Dict[str, _literals_models.Literal]:
     """
     The point of this function is to extract out Literals from a collection of either Python native values (which would
     be converted into Flyte literals) or Promises (the literals in which would just get extracted).
 
     When calling a task inside a workflow, a user might do something like this.
 
         def my_wf(in1: int) -> int:
@@ -65,95 +64,25 @@
     This helper function is used both when sorting out inputs to a task, as well as outputs of a function.
 
     :param ctx: Context needed in case a non-primitive literal needs to be translated to a Flyte literal (like a file)
     :param incoming_values: This is a map of your task's input or wf's output kwargs basically
     :param flyte_interface_types: One side of an :py:class:`flytekit.models.interface.TypedInterface` basically.
     :param native_types: Map to native Python type.
     """
-
-    def extract_value(
-        ctx: FlyteContext,
-        input_val: Any,
-        val_type: type,
-        flyte_literal_type: _type_models.LiteralType,
-    ) -> _literal_models.Literal:
-        if isinstance(input_val, list):
-            lt = flyte_literal_type
-            python_type = val_type
-            if flyte_literal_type.union_type:
-                for i in range(len(flyte_literal_type.union_type.variants)):
-                    variant = flyte_literal_type.union_type.variants[i]
-                    if variant.collection_type:
-                        lt = variant
-                        python_type = get_args(val_type)[i]
-            if lt.collection_type is None:
-                raise TypeError(f"Not a collection type {flyte_literal_type} but got a list {input_val}")
-            try:
-                sub_type: type = ListTransformer.get_sub_type(python_type)
-            except ValueError:
-                if len(input_val) == 0:
-                    raise
-                sub_type = type(input_val[0])
-            # To maintain consistency between translate_inputs_to_literals and ListTransformer.to_literal for batchable types,
-            # directly call ListTransformer.to_literal to batch process the list items. This is necessary because processing
-            # each list item separately could lead to errors since ListTransformer.to_python_value may treat the literal
-            # as it is batched for batchable types.
-            if ListTransformer.is_batchable(python_type):
-                return TypeEngine.to_literal(ctx, input_val, python_type, lt)
-            literal_list = [extract_value(ctx, v, sub_type, lt.collection_type) for v in input_val]
-            return _literal_models.Literal(collection=_literal_models.LiteralCollection(literals=literal_list))
-        elif isinstance(input_val, dict):
-            lt = flyte_literal_type
-            python_type = val_type
-            if flyte_literal_type.union_type:
-                for i in range(len(flyte_literal_type.union_type.variants)):
-                    variant = flyte_literal_type.union_type.variants[i]
-                    if variant.map_value_type:
-                        lt = variant
-                        python_type = get_args(val_type)[i]
-                    if variant.simple == _type_models.SimpleType.STRUCT:
-                        lt = variant
-                        python_type = get_args(val_type)[i]
-            if lt.map_value_type is None and lt.simple != _type_models.SimpleType.STRUCT:
-                raise TypeError(f"Not a map type {lt} but got a map {input_val}")
-            if lt.simple == _type_models.SimpleType.STRUCT:
-                return TypeEngine.to_literal(ctx, input_val, type(input_val), lt)
-            else:
-                k_type, sub_type = DictTransformer.get_dict_types(python_type)  # type: ignore
-                literal_map = {k: extract_value(ctx, v, sub_type, lt.map_value_type) for k, v in input_val.items()}
-                return _literal_models.Literal(map=_literal_models.LiteralMap(literals=literal_map))
-        elif isinstance(input_val, Promise):
-            # In the example above, this handles the "in2=a" type of argument
-            return input_val.val
-        elif isinstance(input_val, VoidPromise):
-            raise AssertionError(
-                f"Outputs of a non-output producing task {input_val.task_name} cannot be passed to another task."
-            )
-        elif isinstance(input_val, tuple):
-            raise AssertionError(
-                "Tuples are not a supported type for individual values in Flyte - got a tuple -"
-                f" {input_val}. If using named tuple in an inner task, please, de-reference the"
-                "actual attribute that you want to use. For example, in NamedTuple('OP', x=int) then"
-                "return v.x, instead of v, even if this has a single element"
-            )
-        else:
-            # This handles native values, the 5 example
-            return TypeEngine.to_literal(ctx, input_val, val_type, flyte_literal_type)
-
     if incoming_values is None:
         raise ValueError("Incoming values cannot be None, must be a dict")
 
     result = {}  # So as to not overwrite the input_kwargs
     for k, v in incoming_values.items():
         if k not in flyte_interface_types:
             raise ValueError(f"Received unexpected keyword argument {k}")
         var = flyte_interface_types[k]
         t = native_types[k]
         try:
-            result[k] = extract_value(ctx, v, t, var.type)
+            result[k] = TypeEngine.to_literal(ctx, v, t, var.type)
         except TypeTransformerFailedError as exc:
             raise TypeTransformerFailedError(f"Failed argument '{k}': {exc}") from exc
 
     return result
 
 
 def get_primitive_val(prim: Primitive) -> Any:
@@ -215,19 +144,19 @@
                     raise ValueError("Only primitive values can be used in comparison")
         if self._lhs is None:
             self._lhs = type_engine.TypeEngine.to_literal(FlyteContextManager.current_context(), lhs, type(lhs), None)
         if self._rhs is None:
             self._rhs = type_engine.TypeEngine.to_literal(FlyteContextManager.current_context(), rhs, type(rhs), None)
 
     @property
-    def rhs(self) -> Union["Promise", _literal_models.Literal]:
+    def rhs(self) -> Union["Promise", _literals_models.Literal]:
         return self._rhs
 
     @property
-    def lhs(self) -> Union["Promise", _literal_models.Literal]:
+    def lhs(self) -> Union["Promise", _literals_models.Literal]:
         return self._lhs
 
     @property
     def op(self) -> ComparisonOps:
         return self._op
 
     def eval(self) -> bool:
@@ -347,15 +276,15 @@
        If the task returns an integer or a ``(int, str)`` tuple like ``t1`` above, calling ``with_overrides`` on the
        result would throw an error. This Promise object adds that.
     #. Assorted handling for conditionals.
     """
 
     # TODO: Currently, NodeOutput we're creating is the slimmer core package Node class, but since only the
     #  id is used, it's okay for now. Let's clean all this up though.
-    def __init__(self, var: str, val: Union[NodeOutput, _literal_models.Literal]):
+    def __init__(self, var: str, val: Union[NodeOutput, _literals_models.Literal]):
         self._var = var
         self._promise_ready = True
         self._val = val
         if val and isinstance(val, NodeOutput):
             self._ref = val
             self._promise_ready = False
             self._val = None
@@ -384,15 +313,15 @@
                 print(p.val)
            else:
                 print(p.ref)
         """
         return self._promise_ready
 
     @property
-    def val(self) -> _literal_models.Literal:
+    def val(self) -> _literals_models.Literal:
         """
         If the promise is ready then this holds the actual evaluate value in Flyte's type system
         """
         return self._val
 
     @property
     def ref(self) -> NodeOutput:
@@ -589,59 +518,52 @@
         def __rshift__(self, other: Any):
             # See comment for runs_before
             return other
 
     return Output(*promises)  # type: ignore
 
 
-def binding_from_flyte_std(
-    ctx: _flyte_context.FlyteContext,
-    var_name: str,
-    expected_literal_type: _type_models.LiteralType,
-    t_value: Any,
-) -> _literals_models.Binding:
-    binding_data = binding_data_from_python_std(ctx, expected_literal_type, t_value, t_value_type=None)
-    return _literals_models.Binding(var=var_name, binding=binding_data)
-
-
 def binding_data_from_python_std(
     ctx: _flyte_context.FlyteContext,
     expected_literal_type: _type_models.LiteralType,
     t_value: Any,
-    t_value_type: Optional[type] = None,
+    t_value_type: type,
+    nodes: List[Node],
 ) -> _literals_models.BindingData:
     # This handles the case where the given value is the output of another task
     if isinstance(t_value, Promise):
         if not t_value.is_ready:
+            nodes.append(t_value.ref.node)  # keeps track of upstream nodes
             return _literals_models.BindingData(promise=t_value.ref)
 
     elif isinstance(t_value, VoidPromise):
         raise AssertionError(
             f"Cannot pass output from task {t_value.task_name} that produces no outputs to a downstream task"
         )
 
     elif t_value is not None and expected_literal_type.union_type is not None:
         for i in range(len(expected_literal_type.union_type.variants)):
             try:
                 lt_type = expected_literal_type.union_type.variants[i]
                 python_type = get_args(t_value_type)[i] if t_value_type else None
-                return binding_data_from_python_std(ctx, lt_type, t_value, python_type)
+                return binding_data_from_python_std(ctx, lt_type, t_value, python_type, nodes)
             except Exception:
                 logger.debug(
                     f"failed to bind data {t_value} with literal type {expected_literal_type.union_type.variants[i]}."
                 )
         raise AssertionError(
             f"Failed to bind data {t_value} with literal type {expected_literal_type.union_type.variants}."
         )
 
     elif isinstance(t_value, list):
-        sub_type: Optional[type] = ListTransformer.get_sub_type(t_value_type) if t_value_type else None
+        sub_type: type = ListTransformer.get_sub_type(t_value_type)
         collection = _literals_models.BindingDataCollection(
             bindings=[
-                binding_data_from_python_std(ctx, expected_literal_type.collection_type, t, sub_type) for t in t_value
+                binding_data_from_python_std(ctx, expected_literal_type.collection_type, t, sub_type, nodes)
+                for t in t_value
             ]
         )
 
         return _literals_models.BindingData(collection=collection)
 
     elif isinstance(t_value, dict):
         if (
@@ -651,21 +573,20 @@
             raise AssertionError(
                 f"this should be a Dictionary type and it is not: {type(t_value)} vs {expected_literal_type}"
             )
         if expected_literal_type.simple == _type_models.SimpleType.STRUCT:
             lit = TypeEngine.to_literal(ctx, t_value, type(t_value), expected_literal_type)
             return _literals_models.BindingData(scalar=lit.scalar)
         else:
-            _, v_type = (
-                DictTransformer.get_dict_types(t_value_type) if t_value_type else None,
-                None,
-            )
+            _, v_type = DictTransformer.get_dict_types(t_value_type)
             m = _literals_models.BindingDataMap(
                 bindings={
-                    k: binding_data_from_python_std(ctx, expected_literal_type.map_value_type, v, v_type)
+                    k: binding_data_from_python_std(
+                        ctx, expected_literal_type.map_value_type, v, v_type or type(v), nodes
+                    )
                     for k, v in t_value.items()
                 }
             )
         return _literals_models.BindingData(map=m)
 
     elif isinstance(t_value, tuple):
         raise AssertionError(
@@ -682,17 +603,18 @@
 
 def binding_from_python_std(
     ctx: _flyte_context.FlyteContext,
     var_name: str,
     expected_literal_type: _type_models.LiteralType,
     t_value: Any,
     t_value_type: type,
-) -> _literals_models.Binding:
-    binding_data = binding_data_from_python_std(ctx, expected_literal_type, t_value, t_value_type)
-    return _literals_models.Binding(var=var_name, binding=binding_data)
+) -> Tuple[_literals_models.Binding, List[Node]]:
+    nodes: List[Node] = []
+    binding_data = binding_data_from_python_std(ctx, expected_literal_type, t_value, t_value_type, nodes)
+    return _literals_models.Binding(var=var_name, binding=binding_data), nodes
 
 
 def to_binding(p: Promise) -> _literals_models.Binding:
     return _literals_models.Binding(var=p.var, binding=_literals_models.BindingData(promise=p.ref))
 
 
 class VoidPromise(object):
@@ -872,15 +794,15 @@
 
     if _inputs_not_allowed:
         inputs_not_allowed_specified = _inputs_not_allowed.intersection(kwargs.keys())
         if inputs_not_allowed_specified:
             raise _user_exceptions.FlyteAssertion(
                 f"Fixed inputs cannot be specified. Please remove the following inputs - {inputs_not_allowed_specified}"
             )
-
+    nodes = []
     for k in sorted(typed_interface.inputs):
         var = typed_interface.inputs[k]
         if k not in kwargs:
             if _inputs_not_allowed and _ignorable_inputs:
                 if k in _ignorable_inputs or k in _inputs_not_allowed:
                     continue
             # TODO to improve the error message, should we show python equivalent types for var.type?
@@ -891,44 +813,37 @@
         # into the function.
         if isinstance(v, tuple):
             raise AssertionError(
                 f"Variable({k}) for function({entity.name}) cannot receive a multi-valued tuple {v}."
                 f" Check if the predecessor function returning more than one value?"
             )
         try:
-            bindings.append(
-                binding_from_flyte_std(
-                    ctx,
-                    var_name=k,
-                    expected_literal_type=var.type,
-                    t_value=v,
-                )
+            b, n = binding_from_python_std(
+                ctx,
+                var_name=k,
+                expected_literal_type=var.type,
+                t_value=v,
+                t_value_type=type(v),  # since we don't have the python type available
             )
+            bindings.append(b)
+            nodes.extend(n)
             used_inputs.add(k)
         except Exception as e:
             raise AssertionError(f"Failed to Bind variable {k} for function {entity.name}.") from e
 
     extra_inputs = used_inputs ^ set(kwargs.keys())
     if len(extra_inputs) > 0:
         raise _user_exceptions.FlyteAssertion(
             f"Too many inputs for [{entity.name}] Expected inputs: {typed_interface.inputs.keys()} "
             f"- extra inputs: {extra_inputs}"
         )
 
     # Detect upstream nodes
     # These will be our core Nodes until we can amend the Promise to use NodeOutputs that reference our Nodes
-    upstream_nodes = list(
-        set(
-            [
-                input_val.ref.node
-                for input_val in kwargs.values()
-                if isinstance(input_val, Promise) and input_val.ref.node_id != _common_constants.GLOBAL_INPUT_NODE_ID
-            ]
-        )
-    )
+    upstream_nodes = list(set([n for n in nodes if n.id != _common_constants.GLOBAL_INPUT_NODE_ID]))
 
     flytekit_node = Node(
         id=f"{ctx.compilation_state.prefix}n{len(ctx.compilation_state.nodes)}",
         metadata=entity.construct_node_metadata(),
         bindings=sorted(bindings, key=lambda b: b.var),
         upstream_nodes=upstream_nodes,
         flyte_entity=entity,
@@ -961,14 +876,15 @@
     :return:  Optional[Union[Tuple[Promise], Promise, VoidPromise]]
     """
     if ctx.compilation_state is None:
         raise _user_exceptions.FlyteAssertion("Cannot create node when not compiling...")
 
     used_inputs = set()
     bindings = []
+    nodes = []
 
     interface = entity.python_interface
     typed_interface = flyte_interface.transform_interface_to_typed_interface(interface)
     # Mypy needs some extra help to believe that `typed_interface` will not be `None`
     assert typed_interface is not None
 
     for k in sorted(interface.inputs):
@@ -994,44 +910,36 @@
         # into the function.
         if isinstance(v, tuple):
             raise AssertionError(
                 f"Variable({k}) for function({entity.name}) cannot receive a multi-valued tuple {v}."
                 f" Check if the predecessor function returning more than one value?"
             )
         try:
-            bindings.append(
-                binding_from_python_std(
-                    ctx,
-                    var_name=k,
-                    expected_literal_type=var.type,
-                    t_value=v,
-                    t_value_type=interface.inputs[k],
-                )
+            b, n = binding_from_python_std(
+                ctx,
+                var_name=k,
+                expected_literal_type=var.type,
+                t_value=v,
+                t_value_type=interface.inputs[k],
             )
+            bindings.append(b)
+            nodes.extend(n)
             used_inputs.add(k)
         except Exception as e:
             raise AssertionError(f"Failed to Bind variable {k} for function {entity.name}.") from e
 
     extra_inputs = used_inputs ^ set(kwargs.keys())
     if len(extra_inputs) > 0:
         raise _user_exceptions.FlyteAssertion(
             "Too many inputs were specified for the interface.  Extra inputs were: {}".format(extra_inputs)
         )
 
     # Detect upstream nodes
     # These will be our core Nodes until we can amend the Promise to use NodeOutputs that reference our Nodes
-    upstream_nodes = list(
-        set(
-            [
-                input_val.ref.node
-                for input_val in kwargs.values()
-                if isinstance(input_val, Promise) and input_val.ref.node_id != _common_constants.GLOBAL_INPUT_NODE_ID
-            ]
-        )
-    )
+    upstream_nodes = list(set([n for n in nodes if n.id != _common_constants.GLOBAL_INPUT_NODE_ID]))
 
     flytekit_node = Node(
         # TODO: Better naming, probably a derivative of the function name.
         id=f"{ctx.compilation_state.prefix}n{len(ctx.compilation_state.nodes)}",
         metadata=entity.construct_node_metadata(),
         bindings=sorted(bindings, key=lambda b: b.var),
         upstream_nodes=upstream_nodes,
```

### Comparing `flytekit-1.7.1b0/flytekit/core/python_auto_container.py` & `flytekit-1.7.1b1/flytekit/core/python_auto_container.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/python_customized_container_task.py` & `flytekit-1.7.1b1/flytekit/core/python_customized_container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/python_function_task.py` & `flytekit-1.7.1b1/flytekit/core/python_function_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/reference.py` & `flytekit-1.7.1b1/flytekit/core/reference.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/reference_entity.py` & `flytekit-1.7.1b1/flytekit/core/reference_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/resources.py` & `flytekit-1.7.1b1/flytekit/core/resources.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/schedule.py` & `flytekit-1.7.1b1/flytekit/core/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/shim_task.py` & `flytekit-1.7.1b1/flytekit/core/shim_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/task.py` & `flytekit-1.7.1b1/flytekit/core/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         if plugin_config_type in cls._PYTHONFUNCTION_TASK_PLUGINS:
             return cls._PYTHONFUNCTION_TASK_PLUGINS[plugin_config_type]
         # Defaults to returning Base PythonFunctionTask
         return PythonFunctionTask
 
 
 T = TypeVar("T")
+FuncOut = TypeVar("FuncOut")
 
 
 @overload
 def task(
     _task_function: None = ...,
     task_config: Optional[T] = ...,
     cache: bool = ...,
@@ -96,21 +97,21 @@
     secret_requests: Optional[List[Secret]] = ...,
     execution_mode: PythonFunctionTask.ExecutionBehavior = ...,
     task_resolver: Optional[TaskResolverMixin] = ...,
     docs: Optional[Documentation] = ...,
     disable_deck: bool = ...,
     pod_template: Optional["PodTemplate"] = ...,
     pod_template_name: Optional[str] = ...,
-) -> Callable[[Callable[..., Any]], PythonFunctionTask[T]]:
+) -> Callable[[Callable[..., FuncOut]], PythonFunctionTask[T]]:
     ...
 
 
 @overload
 def task(
-    _task_function: Callable[..., Any],
+    _task_function: Callable[..., FuncOut],
     task_config: Optional[T] = ...,
     cache: bool = ...,
     cache_serialize: bool = ...,
     cache_version: str = ...,
     retries: int = ...,
     interruptible: Optional[bool] = ...,
     deprecated: str = ...,
@@ -122,20 +123,20 @@
     secret_requests: Optional[List[Secret]] = ...,
     execution_mode: PythonFunctionTask.ExecutionBehavior = ...,
     task_resolver: Optional[TaskResolverMixin] = ...,
     docs: Optional[Documentation] = ...,
     disable_deck: bool = ...,
     pod_template: Optional["PodTemplate"] = ...,
     pod_template_name: Optional[str] = ...,
-) -> PythonFunctionTask[T]:
+) -> Union[PythonFunctionTask[T], Callable[..., FuncOut]]:
     ...
 
 
 def task(
-    _task_function: Optional[Callable[..., Any]] = None,
+    _task_function: Optional[Callable[..., FuncOut]] = None,
     task_config: Optional[T] = None,
     cache: bool = False,
     cache_serialize: bool = False,
     cache_version: str = "",
     retries: int = 0,
     interruptible: Optional[bool] = None,
     deprecated: str = "",
@@ -147,15 +148,15 @@
     secret_requests: Optional[List[Secret]] = None,
     execution_mode: PythonFunctionTask.ExecutionBehavior = PythonFunctionTask.ExecutionBehavior.DEFAULT,
     task_resolver: Optional[TaskResolverMixin] = None,
     docs: Optional[Documentation] = None,
     disable_deck: bool = True,
     pod_template: Optional["PodTemplate"] = None,
     pod_template_name: Optional[str] = None,
-) -> Union[Callable[[Callable[..., Any]], PythonFunctionTask[T]], PythonFunctionTask[T]]:
+) -> Union[Callable[[Callable[..., FuncOut]], PythonFunctionTask[T]], PythonFunctionTask[T], Callable[..., FuncOut]]:
     """
     This is the core decorator to use for any task type in flytekit.
 
     Tasks are the building blocks of Flyte. They represent users code. Tasks have the following properties
 
     * Versioned (usually tied to the git sha)
     * Strong interfaces (specified inputs and outputs)
```

### Comparing `flytekit-1.7.1b0/flytekit/core/testing.py` & `flytekit-1.7.1b1/flytekit/core/testing.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/tracker.py` & `flytekit-1.7.1b1/flytekit/core/tracker.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/type_engine.py` & `flytekit-1.7.1b1/flytekit/core/type_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -842,14 +842,30 @@
         return res
 
     @classmethod
     def to_literal(cls, ctx: FlyteContext, python_val: typing.Any, python_type: Type, expected: LiteralType) -> Literal:
         """
         Converts a python value of a given type and expected ``LiteralType`` into a resolved ``Literal`` value.
         """
+        from flytekit.core.promise import Promise, VoidPromise
+
+        if isinstance(python_val, Promise):
+            # In the example above, this handles the "in2=a" type of argument
+            return python_val.val
+        if isinstance(python_val, VoidPromise):
+            raise AssertionError(
+                f"Outputs of a non-output producing task {python_val.task_name} cannot be passed to another task."
+            )
+        if isinstance(python_val, tuple):
+            raise AssertionError(
+                "Tuples are not a supported type for individual values in Flyte - got a tuple -"
+                f" {python_val}. If using named tuple in an inner task, please, de-reference the"
+                "actual attribute that you want to use. For example, in NamedTuple('OP', x=int) then"
+                "return v.x, instead of v, even if this has a single element"
+            )
         if python_val is None and expected.union_type is None:
             raise TypeTransformerFailedError(f"Python value cannot be None, expected {python_type}/{expected}")
         transformer = cls.get_transformer(python_type)
         if transformer.type_assertions_enabled:
             transformer.assert_type(python_type, python_val)
 
         # In case the value is an annotated type we inspect the annotations and look for hash-related annotations.
@@ -1219,19 +1235,19 @@
 
     def to_literal(self, ctx: FlyteContext, python_val: T, python_type: Type[T], expected: LiteralType) -> Literal:
         python_type = get_underlying_type(python_type)
 
         found_res = False
         res = None
         res_type = None
-        for t in get_args(python_type):
+        for i in range(len(get_args(python_type))):
             try:
+                t = get_args(python_type)[i]
                 trans: TypeTransformer[T] = TypeEngine.get_transformer(t)
-
-                res = trans.to_literal(ctx, python_val, t, expected)
+                res = trans.to_literal(ctx, python_val, t, expected.union_type.variants[i])
                 res_type = _add_tag_to_type(trans.get_literal_type(t), trans.name)
                 if found_res:
                     # Should really never happen, sanity check
                     raise TypeError("Ambiguous choice of variant for union type")
                 found_res = True
             except (TypeTransformerFailedError, AttributeError, ValueError, AssertionError) as e:
                 logger.debug(f"Failed to convert from {python_val} to {t}", e)
```

### Comparing `flytekit-1.7.1b0/flytekit/core/type_helpers.py` & `flytekit-1.7.1b1/flytekit/core/type_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/utils.py` & `flytekit-1.7.1b1/flytekit/core/utils.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/core/workflow.py` & `flytekit-1.7.1b1/flytekit/core/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 import typing
 from dataclasses import dataclass
 from enum import Enum
 from functools import update_wrapper
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union, cast, overload
 
-from typing_extensions import get_args
-
 from flytekit.core import constants as _common_constants
 from flytekit.core.base_task import PythonTask
 from flytekit.core.class_based_resolver import ClassStorageTaskResolver
 from flytekit.core.condition import ConditionalSection
 from flytekit.core.context_manager import CompilationState, FlyteContext, FlyteContextManager, FlyteEntities
 from flytekit.core.docstring import Docstring
 from flytekit.core.interface import (
@@ -31,34 +29,33 @@
     extract_obj_name,
     flyte_entity_call_handler,
     translate_inputs_to_literals,
 )
 from flytekit.core.python_auto_container import PythonAutoContainerTask
 from flytekit.core.reference_entity import ReferenceEntity, WorkflowReference
 from flytekit.core.tracker import extract_task_module
-from flytekit.core.type_engine import TypeEngine, TypeTransformerFailedError, UnionTransformer
+from flytekit.core.type_engine import TypeEngine
 from flytekit.exceptions import scopes as exception_scopes
 from flytekit.exceptions.user import FlyteValidationException, FlyteValueException
 from flytekit.loggers import logger
 from flytekit.models import interface as _interface_models
 from flytekit.models import literals as _literal_models
-from flytekit.models import types as type_models
 from flytekit.models.core import workflow as _workflow_model
 from flytekit.models.documentation import Description, Documentation
-from flytekit.models.types import TypeStructure
 
 GLOBAL_START_NODE = Node(
     id=_common_constants.GLOBAL_INPUT_NODE_ID,
     metadata=None,
     bindings=[],
     upstream_nodes=[],
     flyte_entity=None,
 )
 
 T = typing.TypeVar("T")
+FuncOut = typing.TypeVar("FuncOut")
 
 
 class WorkflowFailurePolicy(Enum):
     """
     Defines the behavior for a workflow execution in the case of an observed node execution failure. By default, a
     workflow execution will immediately enter a failed state if a component node fails.
     """
@@ -275,71 +272,26 @@
 
     def execute(self, **kwargs):
         raise Exception("Should not be called")
 
     def compile(self, **kwargs):
         pass
 
-    def ensure_literal(
-        self, ctx, py_type: Type[T], input_type: type_models.LiteralType, python_value: Any
-    ) -> _literal_models.Literal:
-        """
-        This function will attempt to convert a python value to a literal. If the python value is a promise, it will
-        return the promise's value.
-        """
-        if input_type.union_type is not None:
-            if python_value is None and UnionTransformer.is_optional_type(py_type):
-                return _literal_models.Literal(scalar=_literal_models.Scalar(none_type=_literal_models.Void()))
-            for i in range(len(input_type.union_type.variants)):
-                lt_type = input_type.union_type.variants[i]
-                python_type = get_args(py_type)[i]
-                try:
-                    final_lt = self.ensure_literal(ctx, python_type, lt_type, python_value)
-                    lt_type._structure = TypeStructure(tag=TypeEngine.get_transformer(python_type).name)
-                    return _literal_models.Literal(
-                        scalar=_literal_models.Scalar(union=_literal_models.Union(value=final_lt, stored_type=lt_type))
-                    )
-                except Exception as e:
-                    logger.debug(f"Failed to convert {python_value} to {lt_type} with error {e}")
-            raise TypeError(f"Failed to convert {python_value} to {input_type}")
-        if isinstance(python_value, list) and input_type.collection_type:
-            collection_lit_type = input_type.collection_type
-            collection_py_type = get_args(py_type)[0]
-            xx = [self.ensure_literal(ctx, collection_py_type, collection_lit_type, pv) for pv in python_value]
-            return _literal_models.Literal(collection=_literal_models.LiteralCollection(literals=xx))
-        elif isinstance(python_value, dict) and input_type.map_value_type:
-            mapped_lit_type = input_type.map_value_type
-            mapped_py_type = get_args(py_type)[1]
-            xx = {k: self.ensure_literal(ctx, mapped_py_type, mapped_lit_type, v) for k, v in python_value.items()}  # type: ignore
-            return _literal_models.Literal(map=_literal_models.LiteralMap(literals=xx))
-        # It is a scalar, convert to Promise if necessary.
-        else:
-            if isinstance(python_value, Promise):
-                return python_value.val
-            if not isinstance(python_value, Promise):
-                try:
-                    res = TypeEngine.to_literal(ctx, python_value, py_type, input_type)
-                    return res
-                except TypeTransformerFailedError as exc:
-                    raise TypeError(
-                        f"Failed to convert input '{python_value}' of workflow '{self.name}':\n  {exc}"
-                    ) from exc
-
     def local_execute(self, ctx: FlyteContext, **kwargs) -> Union[Tuple[Promise], Promise, VoidPromise, None]:
         # This is done to support the invariant that Workflow local executions always work with Promise objects
         # holding Flyte literal values. Even in a wf, a user can call a sub-workflow with a Python native value.
-        for k, v in kwargs.items():
-            py_type = self.python_interface.inputs[k]
-            lit_type = self.interface.inputs[k].type
-            kwargs[k] = Promise(var=k, val=self.ensure_literal(ctx, py_type, lit_type, v))
-
-            # The output of this will always be a combination of Python native values and Promises containing Flyte
-            # Literals.
+        literal_map = translate_inputs_to_literals(
+            ctx,
+            incoming_values=kwargs,
+            flyte_interface_types=self.interface.inputs,
+            native_types=self.python_interface.inputs,
+        )
+        kwargs_literals = {k: Promise(var=k, val=v) for k, v in literal_map.items()}
         self.compile()
-        function_outputs = self.execute(**kwargs)
+        function_outputs = self.execute(**kwargs_literals)
         # First handle the empty return case.
         # A workflow function may return a task that doesn't return anything
         #   def wf():
         #       return t1()
         # or it may not return at all
         #   def wf():
         #       t1()
@@ -606,15 +558,15 @@
 
         flyte_type = TypeEngine.to_literal_type(python_type=python_type)
 
         ctx = FlyteContext.current_context()
         if ctx.compilation_state is not None:
             raise Exception("Can't already be compiling")
         with FlyteContextManager.with_context(ctx.with_compilation_state(self.compilation_state)) as ctx:
-            b = binding_from_python_std(
+            b, _ = binding_from_python_std(
                 ctx, output_name, expected_literal_type=flyte_type, t_value=p, t_value_type=python_type
             )
             self._output_bindings.append(b)
             self._python_interface = self._python_interface.with_outputs(extra_outputs={output_name: python_type})
             self._interface = transform_interface_to_typed_interface(self._python_interface)
 
     def add_task(self, task: PythonTask, **kwargs) -> Node:
@@ -729,15 +681,15 @@
                     )
                 if self.python_interface.output_tuple_name is None:
                     raise AssertionError(
                         "Outputs specification for Workflow does not define a tuple, but return value is a tuple"
                     )
                 workflow_outputs = workflow_outputs[0]
             t = self.python_interface.outputs[output_names[0]]
-            b = binding_from_python_std(
+            b, _ = binding_from_python_std(
                 ctx,
                 output_names[0],
                 self.interface.outputs[output_names[0]].type,
                 workflow_outputs,
                 t,
             )
             bindings.append(b)
@@ -746,15 +698,15 @@
                 raise AssertionError("The Workflow specification indicates multiple return values, received only one")
             if len(output_names) != len(workflow_outputs):
                 raise Exception(f"Length mismatch {len(output_names)} vs {len(workflow_outputs)}")
             for i, out in enumerate(output_names):
                 if isinstance(workflow_outputs[i], ConditionalSection):
                     raise AssertionError("A Conditional block (if-else) should always end with an `else_()` clause")
                 t = self.python_interface.outputs[out]
-                b = binding_from_python_std(
+                b, _ = binding_from_python_std(
                     ctx,
                     out,
                     self.interface.outputs[out].type,
                     workflow_outputs[i],
                     t,
                 )
                 bindings.append(b)
@@ -779,34 +731,34 @@
 
 @overload
 def workflow(
     _workflow_function: None = ...,
     failure_policy: Optional[WorkflowFailurePolicy] = ...,
     interruptible: bool = ...,
     docs: Optional[Documentation] = ...,
-) -> Callable[[Callable[..., Any]], PythonFunctionWorkflow]:
+) -> Callable[[Callable[..., FuncOut]], PythonFunctionWorkflow]:
     ...
 
 
 @overload
 def workflow(
-    _workflow_function: Callable[..., Any],
+    _workflow_function: Callable[..., FuncOut],
     failure_policy: Optional[WorkflowFailurePolicy] = ...,
     interruptible: bool = ...,
     docs: Optional[Documentation] = ...,
-) -> PythonFunctionWorkflow:
+) -> Union[PythonFunctionWorkflow, Callable[..., FuncOut]]:
     ...
 
 
 def workflow(
     _workflow_function: Optional[Callable[..., Any]] = None,
     failure_policy: Optional[WorkflowFailurePolicy] = None,
     interruptible: bool = False,
     docs: Optional[Documentation] = None,
-) -> Union[Callable[[Callable[..., Any]], PythonFunctionWorkflow], PythonFunctionWorkflow]:
+) -> Union[Callable[[Callable[..., FuncOut]], PythonFunctionWorkflow], PythonFunctionWorkflow, Callable[..., FuncOut]]:
     """
     This decorator declares a function to be a Flyte workflow. Workflows are declarative entities that construct a DAG
     of tasks using the data flow between tasks.
 
     Unlike a task, the function body of a workflow is evaluated at serialization-time (aka compile-time). This is
     because while we can determine the entire structure of a task by looking at the function's signature, workflows need
     to run through the function itself because the body of the function is what expresses the workflow structure. It's
```

### Comparing `flytekit-1.7.1b0/flytekit/deck/deck.py` & `flytekit-1.7.1b1/flytekit/deck/deck.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/deck/html/template.html` & `flytekit-1.7.1b1/flytekit/deck/html/template.html`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/deck/renderer.py` & `flytekit-1.7.1b1/flytekit/deck/renderer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/exceptions/scopes.py` & `flytekit-1.7.1b1/flytekit/exceptions/scopes.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/exceptions/system.py` & `flytekit-1.7.1b1/flytekit/exceptions/system.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/exceptions/user.py` & `flytekit-1.7.1b1/flytekit/exceptions/user.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/extend/__init__.py` & `flytekit-1.7.1b1/flytekit/extend/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/extend/backend/agent_service.py` & `flytekit-1.7.1b1/flytekit/extend/backend/agent_service.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/extend/backend/base_agent.py` & `flytekit-1.7.1b1/flytekit/extend/backend/base_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,8 +156,11 @@
             while not is_terminal_state(state):
                 progress.start_task(task)
                 time.sleep(1)
                 res = agent.get(dummy_context, metadata)
                 state = res.resource.state
                 logger.info(f"Task state: {state}")
 
+        if state != SUCCEEDED:
+            raise Exception(f"Failed to run the task {entity.name}")
+
         return LiteralMap.from_flyte_idl(res.resource.outputs)
```

### Comparing `flytekit-1.7.1b0/flytekit/extras/cloud_pickle_resolver.py` & `flytekit-1.7.1b1/flytekit/extras/cloud_pickle_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/extras/pytorch/__init__.py` & `flytekit-1.7.1b1/flytekit/extras/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/extras/pytorch/checkpoint.py` & `flytekit-1.7.1b1/flytekit/extras/pytorch/checkpoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/extras/pytorch/native.py` & `flytekit-1.7.1b1/flytekit/extras/pytorch/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/extras/sklearn/__init__.py` & `flytekit-1.7.1b1/flytekit/extras/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/extras/sklearn/native.py` & `flytekit-1.7.1b1/flytekit/extras/sklearn/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/extras/sqlite3/task.py` & `flytekit-1.7.1b1/flytekit/extras/sqlite3/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/extras/tasks/shell.py` & `flytekit-1.7.1b1/flytekit/extras/tasks/shell.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/extras/tensorflow/__init__.py` & `flytekit-1.7.1b1/flytekit/extras/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/extras/tensorflow/model.py` & `flytekit-1.7.1b1/flytekit/extras/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/extras/tensorflow/record.py` & `flytekit-1.7.1b1/flytekit/extras/tensorflow/record.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/image_spec/image_spec.py` & `flytekit-1.7.1b1/flytekit/image_spec/image_spec.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/interaction/parse_stdin.py` & `flytekit-1.7.1b1/flytekit/interaction/parse_stdin.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/interfaces/cli_identifiers.py` & `flytekit-1.7.1b1/flytekit/interfaces/cli_identifiers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/interfaces/random.py` & `flytekit-1.7.1b1/flytekit/interfaces/random.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/interfaces/stats/client.py` & `flytekit-1.7.1b1/flytekit/interfaces/stats/client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/interfaces/stats/taggable.py` & `flytekit-1.7.1b1/flytekit/interfaces/stats/taggable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/lazy_import/lazy_module.py` & `flytekit-1.7.1b1/flytekit/lazy_import/lazy_module.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/loggers.py` & `flytekit-1.7.1b1/flytekit/loggers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/admin/common.py` & `flytekit-1.7.1b1/flytekit/models/admin/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/admin/task_execution.py` & `flytekit-1.7.1b1/flytekit/models/admin/task_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/admin/workflow.py` & `flytekit-1.7.1b1/flytekit/models/admin/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/annotation.py` & `flytekit-1.7.1b1/flytekit/models/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/array_job.py` & `flytekit-1.7.1b1/flytekit/models/array_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/common.py` & `flytekit-1.7.1b1/flytekit/models/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/core/catalog.py` & `flytekit-1.7.1b1/flytekit/models/core/catalog.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/core/compiler.py` & `flytekit-1.7.1b1/flytekit/models/core/compiler.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/core/condition.py` & `flytekit-1.7.1b1/flytekit/models/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/core/errors.py` & `flytekit-1.7.1b1/flytekit/models/core/errors.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/core/execution.py` & `flytekit-1.7.1b1/flytekit/models/core/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/core/identifier.py` & `flytekit-1.7.1b1/flytekit/models/core/identifier.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/core/types.py` & `flytekit-1.7.1b1/flytekit/models/core/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/core/workflow.py` & `flytekit-1.7.1b1/flytekit/models/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/documentation.py` & `flytekit-1.7.1b1/flytekit/models/documentation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/dynamic_job.py` & `flytekit-1.7.1b1/flytekit/models/dynamic_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/execution.py` & `flytekit-1.7.1b1/flytekit/models/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/filters.py` & `flytekit-1.7.1b1/flytekit/models/filters.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/interface.py` & `flytekit-1.7.1b1/flytekit/models/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/launch_plan.py` & `flytekit-1.7.1b1/flytekit/models/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/literals.py` & `flytekit-1.7.1b1/flytekit/models/literals.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/matchable_resource.py` & `flytekit-1.7.1b1/flytekit/models/matchable_resource.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/named_entity.py` & `flytekit-1.7.1b1/flytekit/models/named_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/node_execution.py` & `flytekit-1.7.1b1/flytekit/models/node_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/presto.py` & `flytekit-1.7.1b1/flytekit/models/presto.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/project.py` & `flytekit-1.7.1b1/flytekit/models/project.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/qubole.py` & `flytekit-1.7.1b1/flytekit/models/qubole.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/schedule.py` & `flytekit-1.7.1b1/flytekit/models/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/security.py` & `flytekit-1.7.1b1/flytekit/models/security.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/task.py` & `flytekit-1.7.1b1/flytekit/models/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/types.py` & `flytekit-1.7.1b1/flytekit/models/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/models/workflow_closure.py` & `flytekit-1.7.1b1/flytekit/models/workflow_closure.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/remote/__init__.py` & `flytekit-1.7.1b1/flytekit/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/remote/backfill.py` & `flytekit-1.7.1b1/flytekit/remote/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/remote/entities.py` & `flytekit-1.7.1b1/flytekit/remote/entities.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/remote/executions.py` & `flytekit-1.7.1b1/flytekit/remote/executions.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/remote/lazy_entity.py` & `flytekit-1.7.1b1/flytekit/remote/lazy_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/remote/remote.py` & `flytekit-1.7.1b1/flytekit/remote/remote.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/remote/remote_callable.py` & `flytekit-1.7.1b1/flytekit/remote/remote_callable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/testing/__init__.py` & `flytekit-1.7.1b1/flytekit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/tools/fast_registration.py` & `flytekit-1.7.1b1/flytekit/tools/fast_registration.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/tools/ignore.py` & `flytekit-1.7.1b1/flytekit/tools/ignore.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/tools/module_loader.py` & `flytekit-1.7.1b1/flytekit/tools/module_loader.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/tools/repo.py` & `flytekit-1.7.1b1/flytekit/tools/repo.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/tools/script_mode.py` & `flytekit-1.7.1b1/flytekit/tools/script_mode.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/tools/serialize_helpers.py` & `flytekit-1.7.1b1/flytekit/tools/serialize_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/tools/subprocess.py` & `flytekit-1.7.1b1/flytekit/tools/subprocess.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/tools/translator.py` & `flytekit-1.7.1b1/flytekit/tools/translator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/types/directory/__init__.py` & `flytekit-1.7.1b1/flytekit/types/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/types/directory/types.py` & `flytekit-1.7.1b1/flytekit/types/directory/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/types/file/__init__.py` & `flytekit-1.7.1b1/flytekit/types/file/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/types/file/file.py` & `flytekit-1.7.1b1/flytekit/types/file/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/types/numpy/ndarray.py` & `flytekit-1.7.1b1/flytekit/types/numpy/ndarray.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/types/pickle/pickle.py` & `flytekit-1.7.1b1/flytekit/types/pickle/pickle.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,16 @@
             ctx.file_access.get_data(uri, local_path, False)
             uri = local_path
         with open(uri, "rb") as infile:
             data = cloudpickle.load(infile)
         return data
 
     def to_literal(self, ctx: FlyteContext, python_val: T, python_type: Type[T], expected: LiteralType) -> Literal:
+        if python_val is None:
+            raise AssertionError("Cannot pickle None Value.")
         meta = BlobMetadata(
             type=_core_types.BlobType(
                 format=self.PYTHON_PICKLE_FORMAT, dimensionality=_core_types.BlobType.BlobDimensionality.SINGLE
             )
         )
         # Dump the task output into pickle
         local_dir = ctx.file_access.get_random_local_directory()
```

### Comparing `flytekit-1.7.1b0/flytekit/types/schema/types.py` & `flytekit-1.7.1b1/flytekit/types/schema/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/types/schema/types_pandas.py` & `flytekit-1.7.1b1/flytekit/types/schema/types_pandas.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/types/structured/__init__.py` & `flytekit-1.7.1b1/flytekit/types/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/types/structured/basic_dfs.py` & `flytekit-1.7.1b1/flytekit/types/structured/basic_dfs.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/types/structured/bigquery.py` & `flytekit-1.7.1b1/flytekit/types/structured/bigquery.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit/types/structured/structured_dataset.py` & `flytekit-1.7.1b1/flytekit/types/structured/structured_dataset.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit.egg-info/PKG-INFO` & `flytekit-1.7.1b1/flytekit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.7.1b0
+Version: 1.7.1b1
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.7.1b0 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.7.1b1 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.7.1b0/flytekit.egg-info/SOURCES.txt` & `flytekit-1.7.1b1/flytekit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,16 @@
 flytekit/tools/subprocess.py
 flytekit/tools/translator.py
 flytekit/types/__init__.py
 flytekit/types/directory/__init__.py
 flytekit/types/directory/types.py
 flytekit/types/file/__init__.py
 flytekit/types/file/file.py
+flytekit/types/iterator/__init__.py
+flytekit/types/iterator/iterator.py
 flytekit/types/numpy/__init__.py
 flytekit/types/numpy/ndarray.py
 flytekit/types/pickle/__init__.py
 flytekit/types/pickle/pickle.py
 flytekit/types/schema/__init__.py
 flytekit/types/schema/types.py
 flytekit/types/schema/types_pandas.py
```

### Comparing `flytekit-1.7.1b0/flytekit.egg-info/requires.txt` & `flytekit-1.7.1b1/flytekit.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/flytekit_scripts/flytekit_build_image.sh` & `flytekit-1.7.1b1/flytekit_scripts/flytekit_build_image.sh`

 * *Files identical despite different names*

### Comparing `flytekit-1.7.1b0/setup.py` & `flytekit-1.7.1b1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup  # noqa
 
 extras_require = {}
 
-__version__ = "1.7.1b0"
+__version__ = "1.7.1b1"
 
 setup(
     name="flytekit",
     version=__version__,
     maintainer="Flyte Contributors",
     maintainer_email="admin@flyte.org",
     packages=find_packages(
```

