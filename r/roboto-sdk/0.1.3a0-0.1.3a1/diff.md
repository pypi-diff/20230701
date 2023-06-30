# Comparing `tmp/roboto_sdk-0.1.3a0.tar.gz` & `tmp/roboto_sdk-0.1.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboto_sdk-0.1.3a0.tar", max compression
+gzip compressed data, was "roboto_sdk-0.1.3a1.tar", max compression
```

## Comparing `roboto_sdk-0.1.3a0.tar` & `roboto_sdk-0.1.3a1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0       22 2023-06-30 00:27:04.984881 roboto_sdk-0.1.3a0/README.md
--rw-r--r--   0        0        0      808 2023-06-30 00:27:04.984881 roboto_sdk-0.1.3a0/pyproject.toml
--rw-r--r--   0        0        0       62 2023-06-30 00:27:05.016881 roboto_sdk-0.1.3a0/src/roboto_sdk/__init__.py
--rw-r--r--   0        0        0       48 2023-06-30 00:27:05.016881 roboto_sdk-0.1.3a0/src/roboto_sdk/auth/__init__.py
--rw-r--r--   0        0        0     3892 2023-06-30 00:27:05.016881 roboto_sdk-0.1.3a0/src/roboto_sdk/auth/pat.py
--rw-r--r--   0        0        0      132 2023-06-30 00:27:05.020881 roboto_sdk-0.1.3a0/src/roboto_sdk/cli/__init__.py
--rw-r--r--   0        0        0      334 2023-06-30 00:27:05.020881 roboto_sdk-0.1.3a0/src/roboto_sdk/cli/command/__init__.py
--rw-r--r--   0        0        0     1182 2023-06-30 00:27:05.020881 roboto_sdk-0.1.3a0/src/roboto_sdk/cli/command/args.py
--rw-r--r--   0        0        0     2033 2023-06-30 00:27:05.020881 roboto_sdk-0.1.3a0/src/roboto_sdk/cli/command/model.py
--rw-r--r--   0        0        0      790 2023-06-30 00:27:05.020881 roboto_sdk-0.1.3a0/src/roboto_sdk/cli/context.py
--rw-r--r--   0        0        0      110 2023-06-30 00:27:05.020881 roboto_sdk-0.1.3a0/src/roboto_sdk/cli/datasets/__init__.py
--rw-r--r--   0        0        0     6691 2023-06-30 00:27:05.020881 roboto_sdk-0.1.3a0/src/roboto_sdk/cli/datasets/commands.py
--rw-r--r--   0        0        0     3223 2023-06-30 00:27:05.020881 roboto_sdk-0.1.3a0/src/roboto_sdk/cli/entry.py
--rw-r--r--   0        0        0      108 2023-06-30 00:27:05.020881 roboto_sdk-0.1.3a0/src/roboto_sdk/cli/help/__init__.py
--rw-r--r--   0        0        0      167 2023-06-30 00:27:05.020881 roboto_sdk-0.1.3a0/src/roboto_sdk/cli/help/args.py
--rw-r--r--   0        0        0      110 2023-06-30 00:27:05.024881 roboto_sdk-0.1.3a0/src/roboto_sdk/cli/orgs/__init__.py
--rw-r--r--   0        0        0     3386 2023-06-30 00:27:05.024881 roboto_sdk-0.1.3a0/src/roboto_sdk/cli/orgs/commands.py
--rw-r--r--   0        0        0      110 2023-06-30 00:27:05.024881 roboto_sdk-0.1.3a0/src/roboto_sdk/cli/tokens/__init__.py
--rw-r--r--   0        0        0     3301 2023-06-30 00:27:05.024881 roboto_sdk-0.1.3a0/src/roboto_sdk/cli/tokens/commands.py
--rw-r--r--   0        0        0      110 2023-06-30 00:27:05.028881 roboto_sdk-0.1.3a0/src/roboto_sdk/cli/triggers/__init__.py
--rw-r--r--   0        0        0     2874 2023-06-30 00:27:05.028881 roboto_sdk-0.1.3a0/src/roboto_sdk/cli/triggers/commands.py
--rw-r--r--   0        0        0      110 2023-06-30 00:27:05.028881 roboto_sdk-0.1.3a0/src/roboto_sdk/cli/users/__init__.py
--rw-r--r--   0        0        0      733 2023-06-30 00:27:05.028881 roboto_sdk-0.1.3a0/src/roboto_sdk/cli/users/commands.py
--rw-r--r--   0        0        0       48 2023-06-30 00:27:05.028881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/__init__.py
--rw-r--r--   0        0        0     1633 2023-06-30 00:27:05.032881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/__init__.py
--rw-r--r--   0        0        0     7019 2023-06-30 00:27:05.032881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/action.py
--rw-r--r--   0        0        0     2804 2023-06-30 00:27:05.032881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/action_delegate.py
--rw-r--r--   0        0        0     5167 2023-06-30 00:27:05.032881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/action_http_delegate.py
--rw-r--r--   0        0        0      651 2023-06-30 00:27:05.032881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/action_http_resources.py
--rw-r--r--   0        0        0      792 2023-06-30 00:27:05.032881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/action_record.py
--rw-r--r--   0        0        0      106 2023-06-30 00:27:05.032881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/error.py
--rw-r--r--   0        0        0     4294 2023-06-30 00:27:05.032881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/invocation.py
--rw-r--r--   0        0        0     1653 2023-06-30 00:27:05.032881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/invocation_delegate.py
--rw-r--r--   0        0        0     4684 2023-06-30 00:27:05.032881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/invocation_http_delegate.py
--rw-r--r--   0        0        0      534 2023-06-30 00:27:05.032881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/invocation_http_resources.py
--rw-r--r--   0        0        0     1592 2023-06-30 00:27:05.032881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/invocation_record.py
--rw-r--r--   0        0        0      546 2023-06-30 00:27:05.036881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/datasets/__init__.py
--rw-r--r--   0        0        0     9572 2023-06-30 00:27:05.036881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/datasets/dataset.py
--rw-r--r--   0        0        0     2132 2023-06-30 00:27:05.036881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/datasets/delegate.py
--rw-r--r--   0        0        0     4759 2023-06-30 00:27:05.036881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/datasets/http_delegate.py
--rw-r--r--   0        0        0      340 2023-06-30 00:27:05.036881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/datasets/http_resources.py
--rw-r--r--   0        0        0      817 2023-06-30 00:27:05.036881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/datasets/record.py
--rw-r--r--   0        0        0      436 2023-06-30 00:27:05.036881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/files/__init__.py
--rw-r--r--   0        0        0     1156 2023-06-30 00:27:05.036881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/files/delegate.py
--rw-r--r--   0        0        0      771 2023-06-30 00:27:05.036881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/files/file.py
--rw-r--r--   0        0        0     2110 2023-06-30 00:27:05.036881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/files/http_delegate.py
--rw-r--r--   0        0        0      168 2023-06-30 00:27:05.036881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/files/http_resources.py
--rw-r--r--   0        0        0      385 2023-06-30 00:27:05.036881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/files/record.py
--rw-r--r--   0        0        0     2320 2023-06-30 00:27:05.036881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/files/s3_delegate.py
--rw-r--r--   0        0        0      633 2023-06-30 00:27:05.040881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/orgs/__init__.py
--rw-r--r--   0        0        0     1620 2023-06-30 00:27:05.040881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/orgs/delegate.py
--rw-r--r--   0        0        0     3610 2023-06-30 00:27:05.040881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/orgs/http_delegate.py
--rw-r--r--   0        0        0      359 2023-06-30 00:27:05.040881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/orgs/http_resources.py
--rw-r--r--   0        0        0     2381 2023-06-30 00:27:05.040881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/orgs/org.py
--rw-r--r--   0        0        0     1145 2023-06-30 00:27:05.040881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/orgs/org_role.py
--rw-r--r--   0        0        0      563 2023-06-30 00:27:05.040881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/orgs/record.py
--rw-r--r--   0        0        0      387 2023-06-30 00:27:05.040881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/tokens/__init__.py
--rw-r--r--   0        0        0      818 2023-06-30 00:27:05.040881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/tokens/delegate.py
--rw-r--r--   0        0        0     1968 2023-06-30 00:27:05.040881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/tokens/http_delegate.py
--rw-r--r--   0        0        0      184 2023-06-30 00:27:05.040881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/tokens/http_resources.py
--rw-r--r--   0        0        0      412 2023-06-30 00:27:05.040881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/tokens/record.py
--rw-r--r--   0        0        0     1807 2023-06-30 00:27:05.040881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/tokens/token.py
--rw-r--r--   0        0        0      391 2023-06-30 00:27:05.044881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/triggers/__init__.py
--rw-r--r--   0        0        0     2255 2023-06-30 00:27:05.044881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/triggers/http_delegate.py
--rw-r--r--   0        0        0      205 2023-06-30 00:27:05.044881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/triggers/http_resources.py
--rw-r--r--   0        0        0     2661 2023-06-30 00:27:05.044881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/triggers/trigger.py
--rw-r--r--   0        0        0      857 2023-06-30 00:27:05.044881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/triggers/trigger_delegate.py
--rw-r--r--   0        0        0      249 2023-06-30 00:27:05.044881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/triggers/trigger_record.py
--rw-r--r--   0        0        0      262 2023-06-30 00:27:05.044881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/users/__init__.py
--rw-r--r--   0        0        0     1016 2023-06-30 00:27:05.044881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/users/http_delegate.py
--rw-r--r--   0        0        0     1200 2023-06-30 00:27:05.044881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/users/user.py
--rw-r--r--   0        0        0      451 2023-06-30 00:27:05.044881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/users/user_delegate.py
--rw-r--r--   0        0        0      162 2023-06-30 00:27:05.044881 roboto_sdk-0.1.3a0/src/roboto_sdk/domain/users/user_record.py
--rw-r--r--   0        0        0      704 2023-06-30 00:27:05.048881 roboto_sdk-0.1.3a0/src/roboto_sdk/http/__init__.py
--rw-r--r--   0        0        0      216 2023-06-30 00:27:05.048881 roboto_sdk-0.1.3a0/src/roboto_sdk/http/constants.py
--rw-r--r--   0        0        0     8880 2023-06-30 00:27:05.048881 roboto_sdk-0.1.3a0/src/roboto_sdk/http/http_client.py
--rw-r--r--   0        0        0     3032 2023-06-30 00:27:05.048881 roboto_sdk-0.1.3a0/src/roboto_sdk/http/request_decorators.py
--rw-r--r--   0        0        0      994 2023-06-30 00:27:05.048881 roboto_sdk-0.1.3a0/src/roboto_sdk/http/testing_util.py
--rw-r--r--   0        0        0      158 2023-06-30 00:27:05.048881 roboto_sdk-0.1.3a0/src/roboto_sdk/logging.py
--rw-r--r--   0        0        0      211 2023-06-30 00:27:05.048881 roboto_sdk-0.1.3a0/src/roboto_sdk/pagination.py
--rw-r--r--   0        0        0      168 2023-06-30 00:27:05.048881 roboto_sdk-0.1.3a0/src/roboto_sdk/profile/__init__.py
--rw-r--r--   0        0        0     2809 2023-06-30 00:27:05.048881 roboto_sdk-0.1.3a0/src/roboto_sdk/profile/profile.py
--rw-r--r--   0        0        0        0 2023-06-30 00:27:05.048881 roboto_sdk-0.1.3a0/src/roboto_sdk/py.typed
--rw-r--r--   0        0        0      651 2023-06-30 00:27:05.048881 roboto_sdk-0.1.3a0/src/roboto_sdk/serde.py
--rw-r--r--   0        0        0      112 2023-06-30 00:27:05.048881 roboto_sdk-0.1.3a0/src/roboto_sdk/time.py
--rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 roboto_sdk-0.1.3a0/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-05-31 20:34:51.104994 roboto_sdk-0.1.3a1/README.md
+-rw-r--r--   0        0        0      950 2023-06-30 22:24:22.193303 roboto_sdk-0.1.3a1/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-05-31 20:34:51.105420 roboto_sdk-0.1.3a1/src/roboto_sdk/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-31 20:51:22.684541 roboto_sdk-0.1.3a1/src/roboto_sdk/auth/__init__.py
+-rw-r--r--   0        0        0     4034 2023-06-30 22:13:00.631826 roboto_sdk-0.1.3a1/src/roboto_sdk/auth/pat.py
+-rw-r--r--   0        0        0      132 2023-05-31 21:34:25.532839 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/__init__.py
+-rw-r--r--   0        0        0      334 2023-06-21 21:00:10.362037 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/command/__init__.py
+-rw-r--r--   0        0        0     1182 2023-06-21 21:02:17.537089 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/command/args.py
+-rw-r--r--   0        0        0     2033 2023-06-21 21:18:40.940344 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/command/model.py
+-rw-r--r--   0        0        0      790 2023-06-29 16:05:04.384582 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/context.py
+-rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/datasets/__init__.py
+-rw-r--r--   0        0        0     6691 2023-06-29 16:05:04.385345 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/datasets/commands.py
+-rw-r--r--   0        0        0     3584 2023-06-30 22:13:00.626079 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/entry.py
+-rw-r--r--   0        0        0      108 2023-06-21 21:18:40.926071 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/help/__init__.py
+-rw-r--r--   0        0        0      167 2023-06-21 21:18:40.928579 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/help/args.py
+-rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/orgs/__init__.py
+-rw-r--r--   0        0        0     3386 2023-06-28 22:21:48.431065 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/orgs/commands.py
+-rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/tokens/__init__.py
+-rw-r--r--   0        0        0     3301 2023-06-27 00:52:24.673209 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/tokens/commands.py
+-rw-r--r--   0        0        0      110 2023-06-21 18:17:36.115870 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/triggers/__init__.py
+-rw-r--r--   0        0        0     2874 2023-06-21 21:18:41.332847 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/triggers/commands.py
+-rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/users/__init__.py
+-rw-r--r--   0        0        0      733 2023-06-23 21:06:13.848323 roboto_sdk-0.1.3a1/src/roboto_sdk/cli/users/commands.py
+-rw-r--r--   0        0        0       48 2023-06-21 18:17:36.116077 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/__init__.py
+-rw-r--r--   0        0        0     1633 2023-06-29 15:35:56.463310 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/__init__.py
+-rw-r--r--   0        0        0     7019 2023-06-29 15:35:56.463411 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/action.py
+-rw-r--r--   0        0        0     2804 2023-06-29 15:35:56.463471 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/action_delegate.py
+-rw-r--r--   0        0        0     5167 2023-06-29 15:35:56.463534 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/action_http_delegate.py
+-rw-r--r--   0        0        0      651 2023-06-29 15:35:56.463581 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/action_http_resources.py
+-rw-r--r--   0        0        0      792 2023-06-29 15:35:56.463632 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/action_record.py
+-rw-r--r--   0        0        0      106 2023-06-29 15:35:56.463681 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/error.py
+-rw-r--r--   0        0        0     4294 2023-06-29 15:35:56.463871 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/invocation.py
+-rw-r--r--   0        0        0     1653 2023-06-29 15:35:56.463945 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/invocation_delegate.py
+-rw-r--r--   0        0        0     4684 2023-06-29 15:35:56.464027 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/invocation_http_delegate.py
+-rw-r--r--   0        0        0      534 2023-06-29 15:35:56.464078 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/invocation_http_resources.py
+-rw-r--r--   0        0        0     1592 2023-06-29 15:35:56.464142 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/invocation_record.py
+-rw-r--r--   0        0        0      546 2023-06-29 15:35:56.464218 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/__init__.py
+-rw-r--r--   0        0        0     9572 2023-06-29 15:35:56.464288 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/dataset.py
+-rw-r--r--   0        0        0     2132 2023-06-29 15:35:56.464354 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/delegate.py
+-rw-r--r--   0        0        0     4759 2023-06-29 15:35:56.464409 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/http_delegate.py
+-rw-r--r--   0        0        0      340 2023-06-29 15:35:56.464452 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/http_resources.py
+-rw-r--r--   0        0        0      817 2023-06-29 15:35:56.464498 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/record.py
+-rw-r--r--   0        0        0      436 2023-06-29 15:35:56.464570 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/__init__.py
+-rw-r--r--   0        0        0     1156 2023-06-29 15:35:56.464729 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/delegate.py
+-rw-r--r--   0        0        0      771 2023-06-29 15:35:56.464889 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/file.py
+-rw-r--r--   0        0        0     2110 2023-06-29 15:35:56.464947 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/http_delegate.py
+-rw-r--r--   0        0        0      168 2023-06-29 15:35:56.464990 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/http_resources.py
+-rw-r--r--   0        0        0      385 2023-06-29 15:35:56.465086 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/record.py
+-rw-r--r--   0        0        0     2320 2023-06-29 15:35:56.465141 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/s3_delegate.py
+-rw-r--r--   0        0        0      633 2023-06-29 21:05:11.294925 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/__init__.py
+-rw-r--r--   0        0        0     1620 2023-06-29 00:30:17.060813 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/delegate.py
+-rw-r--r--   0        0        0     3610 2023-06-29 00:30:17.061047 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/http_delegate.py
+-rw-r--r--   0        0        0      359 2023-06-28 06:35:03.341928 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/http_resources.py
+-rw-r--r--   0        0        0     2381 2023-06-29 00:30:17.061322 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/org.py
+-rw-r--r--   0        0        0     1145 2023-06-28 21:49:35.087173 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/org_role.py
+-rw-r--r--   0        0        0      563 2023-06-29 21:05:11.295549 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/record.py
+-rw-r--r--   0        0        0      387 2023-06-23 21:06:13.848727 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/tokens/__init__.py
+-rw-r--r--   0        0        0      818 2023-06-27 00:52:24.673479 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/tokens/delegate.py
+-rw-r--r--   0        0        0     1968 2023-06-27 00:52:24.673652 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/tokens/http_delegate.py
+-rw-r--r--   0        0        0      184 2023-06-27 00:52:24.673821 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/tokens/http_resources.py
+-rw-r--r--   0        0        0      412 2023-06-27 00:52:24.673996 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/tokens/record.py
+-rw-r--r--   0        0        0     1807 2023-06-27 00:52:24.674186 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/tokens/token.py
+-rw-r--r--   0        0        0      391 2023-06-21 18:17:36.116185 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/triggers/__init__.py
+-rw-r--r--   0        0        0     2255 2023-06-21 18:17:36.116295 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/triggers/http_delegate.py
+-rw-r--r--   0        0        0      205 2023-06-21 18:17:36.116397 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/triggers/http_resources.py
+-rw-r--r--   0        0        0     2661 2023-06-29 16:05:04.386157 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/triggers/trigger.py
+-rw-r--r--   0        0        0      857 2023-06-21 18:17:36.116610 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/triggers/trigger_delegate.py
+-rw-r--r--   0        0        0      249 2023-06-21 18:17:36.116722 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/triggers/trigger_record.py
+-rw-r--r--   0        0        0      262 2023-06-23 21:06:13.849582 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/users/__init__.py
+-rw-r--r--   0        0        0     1016 2023-06-23 21:17:31.788229 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/users/http_delegate.py
+-rw-r--r--   0        0        0     1200 2023-06-23 21:17:31.796065 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/users/user.py
+-rw-r--r--   0        0        0      451 2023-06-23 21:17:31.793509 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/users/user_delegate.py
+-rw-r--r--   0        0        0      162 2023-06-23 21:06:13.850109 roboto_sdk-0.1.3a1/src/roboto_sdk/domain/users/user_record.py
+-rw-r--r--   0        0        0      704 2023-06-29 00:30:17.043102 roboto_sdk-0.1.3a1/src/roboto_sdk/http/__init__.py
+-rw-r--r--   0        0        0      216 2023-06-23 21:06:13.850449 roboto_sdk-0.1.3a1/src/roboto_sdk/http/constants.py
+-rw-r--r--   0        0        0     8880 2023-06-13 17:13:48.415283 roboto_sdk-0.1.3a1/src/roboto_sdk/http/http_client.py
+-rw-r--r--   0        0        0     3127 2023-06-30 22:09:49.535434 roboto_sdk-0.1.3a1/src/roboto_sdk/http/request_decorators.py
+-rw-r--r--   0        0        0      994 2023-06-29 00:30:17.043313 roboto_sdk-0.1.3a1/src/roboto_sdk/http/testing_util.py
+-rw-r--r--   0        0        0      158 2023-05-31 20:51:22.686567 roboto_sdk-0.1.3a1/src/roboto_sdk/logging.py
+-rw-r--r--   0        0        0      211 2023-06-26 18:41:27.400684 roboto_sdk-0.1.3a1/src/roboto_sdk/pagination.py
+-rw-r--r--   0        0        0      168 2023-06-25 17:00:28.638279 roboto_sdk-0.1.3a1/src/roboto_sdk/profile/__init__.py
+-rw-r--r--   0        0        0     2958 2023-06-30 22:11:44.938691 roboto_sdk-0.1.3a1/src/roboto_sdk/profile/profile.py
+-rw-r--r--   0        0        0        0 2023-05-31 20:34:27.418611 roboto_sdk-0.1.3a1/src/roboto_sdk/py.typed
+-rw-r--r--   0        0        0      651 2023-06-13 17:13:48.417645 roboto_sdk-0.1.3a1/src/roboto_sdk/serde.py
+-rw-r--r--   0        0        0      112 2023-06-01 19:18:26.925334 roboto_sdk-0.1.3a1/src/roboto_sdk/time.py
+-rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 roboto_sdk-0.1.3a1/PKG-INFO
```

### Comparing `roboto_sdk-0.1.3a0/pyproject.toml` & `roboto_sdk-0.1.3a1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires-python = ">=3.10"
 # Ignore this version attribute, it is here to satisfy setuptools.
 # The actual version is set by Poetry in the [tool.poetry] section.
 version = "0.0.0"
 
 [tool.poetry]
 name = "roboto_sdk"
-version = "0.1.3a0"
+version = "0.1.3a1"
 description = "Tools for interacting with roboto.ai"
 license = "MIT"
 readme = "README.md"
 authors = ["Roboto <admin@roboto.ai>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -24,7 +24,12 @@
 # While Poetry is used for dependency and venv management,
 # it relies on setuptools for packaging when installing from a local directory.
 [tool.setuptools.package-data]
 roboto_sdk = ["py.typed"]
 
 [tool.poetry.scripts]
 roboto = 'roboto_sdk.cli:entry'
+
+[tool.pytest.ini_options]
+markers = [
+    "cli: tests which assume that the CLI is available on ${PATH}. (deselect with '-m \"not cli\"')",
+]
```

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/auth/pat.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/auth/pat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
+
 import datetime
 import pathlib
 from typing import Any, Optional
 
 import boto3
 import jwt
 
@@ -27,24 +28,31 @@
 
 
 class BearerTokenVendor:
     _client_id: str
     _cognito: Any
     _expires: datetime.datetime
     _id_token: Optional[str]
+    _profile: RobotoProfile
 
-    def __init__(self, client_id: str, cognito: Any | None = None):
+    def __init__(
+        self,
+        client_id: str,
+        cognito: Any | None = None,
+        profile: RobotoProfile = RobotoProfile(),
+    ):
         self._client_id = client_id
         self._cognito = (
             cognito
             if cognito is not None
             else boto3.client("cognito-idp", region_name="us-west-2")
         )
         self._expires = datetime.datetime.now()
         self._id_token = None
+        self._profile = profile
 
     def perform_cognito_handshake(self, user_id: str, token: str):
         try:
             res = self._cognito.initiate_auth(
                 AuthFlow="CUSTOM_AUTH",
                 ClientId=self._client_id,
                 AuthParameters={"USERNAME": user_id},
@@ -71,15 +79,15 @@
         except self._cognito.exceptions.NotAuthorizedException:
             raise RejectedTokenException("Authorization rejected by Cognito!")
         except self._cognito.exceptions.UserNotFoundException:
             raise RejectedTokenException(f"User {user_id} does not exist!")
 
     def refresh_tokens(self):
         now = datetime.datetime.now()
-        entry = RobotoProfile.get_entry()
+        entry = self._profile.get_entry()
         id_token_file = pathlib.Path(f"{ROBOTO_TEMPDIR}/{entry.token}_id_token")
 
         if id_token_file.exists():
             with open(id_token_file, "r") as f:
                 content = f.read()
 
             # We don't need to verify signature because we'll get rejected by Roboto Service if the signature is invalid
```

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/cli/command/args.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/cli/command/args.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/cli/command/model.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/cli/command/model.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/cli/context.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/cli/context.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/cli/datasets/commands.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/cli/datasets/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/cli/entry.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/cli/entry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
 import argparse
 import logging
+import pathlib
 import sys
 from typing import Any
 
 from ..domain.actions import ActionHttpDelegate
 from ..domain.datasets import DatasetHttpDelegate
 from ..domain.orgs import OrgHttpDelegate
 from ..domain.tokens import TokenHttpDelegate
@@ -40,15 +41,20 @@
 ]
 
 BETA_USER_POOL_CLIENT_ID = "7p2e45lijin58tuaairtflf3m8"
 PROD_USER_POOL_CLIENT_ID = "1gricmdmh0vv582qdd84phab5"
 
 
 def __populate_context(args, context: CLIContext):
-    profile_entry = RobotoProfile.get_entry()
+    profile = (
+        RobotoProfile()
+        if args.config_file is None
+        else RobotoProfile(config_file=args.config_file)
+    )
+    profile_entry = profile.get_entry()
     http_client_args: dict[str, Any] = {
         "default_endpoint": profile_entry.default_endpoint
     }
 
     if "localhost" not in profile_entry.default_endpoint:
         http_client_args["default_auth"] = PATAuthDecorator.for_client(
             client_id=profile_entry.default_client_id
@@ -83,14 +89,21 @@
         ),
     )
 
     parser.add_argument(
         "--debug", help="Sets the log level to DEBUG", action="store_true"
     )
 
+    parser.add_argument(
+        "--config-file",
+        help="Overrides the location of the roboto config.json file. Defaults to ~/.roboto/config.json",
+        type=pathlib.Path,
+        required=False,
+    )
+
     context = CLIContext()
 
     logging.basicConfig(level=logging.ERROR, stream=sys.stderr)
 
     subcommands = parser.add_subparsers()
     subcommands.required = True
```

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/cli/orgs/commands.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/cli/orgs/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/cli/tokens/commands.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/cli/tokens/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/cli/triggers/commands.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/cli/triggers/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/cli/users/commands.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/cli/users/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/__init__.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/action.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/action.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/action_delegate.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/action_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/action_http_delegate.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/action_http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/action_http_resources.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/action_http_resources.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/action_record.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/action_record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/invocation.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/invocation.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/invocation_delegate.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/invocation_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/invocation_http_delegate.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/invocation_http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/invocation_http_resources.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/invocation_http_resources.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/actions/invocation_record.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/actions/invocation_record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/datasets/__init__.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/datasets/dataset.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/datasets/delegate.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/datasets/http_delegate.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/datasets/record.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/datasets/record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/files/delegate.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/files/file.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/file.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/files/http_delegate.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/files/s3_delegate.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/files/s3_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/orgs/__init__.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/orgs/delegate.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/orgs/http_delegate.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/orgs/org.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/org.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/orgs/org_role.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/org_role.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/orgs/record.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/orgs/record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/tokens/delegate.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/tokens/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/tokens/http_delegate.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/tokens/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/tokens/token.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/tokens/token.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/triggers/http_delegate.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/triggers/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/triggers/trigger.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/triggers/trigger.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/triggers/trigger_delegate.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/triggers/trigger_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/users/http_delegate.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/users/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/domain/users/user.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/domain/users/user.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/http/__init__.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/http/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/http/http_client.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/http/http_client.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/http/request_decorators.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/http/request_decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from botocore.awsrequest import AWSRequest
 from botocore.credentials import (
     ReadOnlyCredentials,
 )
 
 from ..auth.pat import BearerTokenVendor
 from ..logging import default_logger
+from ..profile import RobotoProfile
 from .constants import USER_OVERRIDE_HEADER
 from .http_client import HttpRequest
 
 logger = default_logger()
 
 
 class LocalAuthDecorator:
@@ -40,16 +41,16 @@
         if request.headers is None:
             request.headers = {}
 
         request.headers["Authorization"] = self._token_vendor.get_auth_header()
         return request
 
     @staticmethod
-    def for_client(client_id: str, **kwargs):
-        token_vendor = BearerTokenVendor(client_id=client_id, **kwargs)
+    def for_client(client_id: str, profile: RobotoProfile = RobotoProfile(), **kwargs):
+        token_vendor = BearerTokenVendor(client_id=client_id, profile=profile, **kwargs)
         return PATAuthDecorator(token_vendor=token_vendor)
 
 
 class SigV4AuthDecorator:
     __credentials: ReadOnlyCredentials
     __region: str
     __service: str
```

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/http/testing_util.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/http/testing_util.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/profile/profile.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/profile/profile.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 log = default_logger()
 
 PROFILE_ENV_VAR = "ROBOTO_PROFILE"
 
 PROD_USER_POOL_CLIENT_ID = "1gricmdmh0vv582qdd84phab5"
 PROD_ENDPOINT = "https://api.roboto.ai"
 
-ROBOTO_CONFIG_DIR = pathlib.Path(f"{pathlib.Path.home()}/.roboto")
-ROBOTO_PROFILE_FILE = pathlib.Path(f"{ROBOTO_CONFIG_DIR}/config.json")
+DEFAULT_ROBOTO_CONFIG_DIR = pathlib.Path(f"{pathlib.Path.home()}/.roboto")
+DEFAULT_ROBOTO_PROFILE_FILE = pathlib.Path(f"{DEFAULT_ROBOTO_CONFIG_DIR}/config.json")
 
 
 class RobotoProfileEntry(pydantic.BaseModel):
     user_id: str
     token: str
     default_endpoint: str = PROD_ENDPOINT
     default_client_id: str = PROD_USER_POOL_CLIENT_ID
@@ -31,56 +31,60 @@
     none = "none"
     malformed = "malformed"
     implicit = "implicit"
     explicit = "explicit"
 
 
 class RobotoProfile:
-    @staticmethod
+    __config_file: pathlib.Path
+
+    def __init__(self, config_file: pathlib.Path = DEFAULT_ROBOTO_PROFILE_FILE):
+        self.__config_file = config_file
+
     def __base_entry_from_file(
+        self,
         profile_name: str | None,
     ) -> tuple[RobotoProfileFileType, RobotoProfileEntry | None]:
-        if not ROBOTO_PROFILE_FILE.is_file():
+        if not self.__config_file.is_file():
             return RobotoProfileFileType.none, None
 
-        with open(ROBOTO_PROFILE_FILE, "r") as f:
+        with open(self.__config_file, "r") as f:
             contents: dict[str, Any] = json.loads(f.read())
 
         profile_to_check = "default" if profile_name is None else profile_name
         if profile_to_check in contents.keys():
             try:
                 return RobotoProfileFileType.explicit, RobotoProfileEntry.parse_obj(
                     contents.get(profile_to_check)
                 )
             except pydantic.ValidationError:
                 log.warning(
-                    f"Couldn't parse {ROBOTO_PROFILE_FILE} as a multi-profile 'explicit' type"
+                    f"Couldn't parse {self.__config_file} as a multi-profile 'explicit' type"
                 )
                 return RobotoProfileFileType.malformed, None
 
         try:
             return RobotoProfileFileType.implicit, RobotoProfileEntry.parse_obj(
                 contents
             )
         except pydantic.ValidationError:
             log.warning(
-                f"Couldn't parse {ROBOTO_PROFILE_FILE} as single-profile 'implicit' type"
+                f"Couldn't parse {self.__config_file} as single-profile 'implicit' type"
             )
             return RobotoProfileFileType.malformed, None
 
-    @staticmethod
-    def get_entry(profile_name: str | None = None) -> RobotoProfileEntry:
+    def get_entry(self, profile_name: str | None = None) -> RobotoProfileEntry:
         profile_to_check = (
             profile_name
             if profile_name is not None
             else os.getenv(PROFILE_ENV_VAR, "default")
         )
         # TODO - Support AWS style order of precedence
-        file_type, entry = RobotoProfile.__base_entry_from_file(profile_to_check)
+        file_type, entry = self.__base_entry_from_file(profile_to_check)
 
         if file_type == RobotoProfileFileType.malformed:
-            raise ValueError(f"Malformed roboto profile file '{ROBOTO_PROFILE_FILE}'")
+            raise ValueError(f"Malformed roboto profile file '{self.__config_file}'")
         elif file_type == RobotoProfileFileType.none:
-            raise ValueError(f"Missing roboto profile file '{ROBOTO_PROFILE_FILE}'")
+            raise ValueError(f"Missing roboto profile file '{self.__config_file}'")
 
         assert entry is not None
         return entry
```

### Comparing `roboto_sdk-0.1.3a0/src/roboto_sdk/serde.py` & `roboto_sdk-0.1.3a1/src/roboto_sdk/serde.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.3a0/PKG-INFO` & `roboto_sdk-0.1.3a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboto-sdk
-Version: 0.1.3a0
+Version: 0.1.3a1
 Summary: Tools for interacting with roboto.ai
 License: MIT
 Author: Roboto
 Author-email: admin@roboto.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

