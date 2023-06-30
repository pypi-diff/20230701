# Comparing `tmp/bullmq-1.3.1.tar.gz` & `tmp/bullmq-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-1.3.1.tar", last modified: Thu Jun 29 16:23:13 2023, max compression
+gzip compressed data, was "bullmq-1.4.0.tar", last modified: Fri Jun 30 22:04:10 2023, max compression
```

## Comparing `bullmq-1.3.1.tar` & `bullmq-1.4.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:23:13.755871 bullmq-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-29 16:23:13.755871 bullmq-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-29 16:22:04.000000 bullmq-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:23:13.751871 bullmq-1.3.1/bullmq/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-29 16:23:11.000000 bullmq-1.3.1/bullmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-29 16:22:04.000000 bullmq-1.3.1/bullmq/backoffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:23:13.755871 bullmq-1.3.1/bullmq/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/addJob-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/changeDelay-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/changePriority-5.lua
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/drain-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/getState-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/getStateV2-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/moveJobFromActiveToWait-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/moveStalledJobsToWait-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/moveToActive-10.lua
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/moveToFinished-13.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/pause-5.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/promote-7.lua
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/reprocessJob-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/retryJob-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/retryJobs-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/saveStacktrace-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/updateData-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-29 16:22:46.000000 bullmq-1.3.1/bullmq/commands/updateProgress-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-29 16:22:04.000000 bullmq-1.3.1/bullmq/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-29 16:22:04.000000 bullmq-1.3.1/bullmq/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-29 16:22:04.000000 bullmq-1.3.1/bullmq/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-06-29 16:22:04.000000 bullmq-1.3.1/bullmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-29 16:22:04.000000 bullmq-1.3.1/bullmq/redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18344 2023-06-29 16:22:04.000000 bullmq-1.3.1/bullmq/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-29 16:22:04.000000 bullmq-1.3.1/bullmq/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:23:13.755871 bullmq-1.3.1/bullmq/types/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-29 16:22:04.000000 bullmq-1.3.1/bullmq/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-29 16:22:04.000000 bullmq-1.3.1/bullmq/types/backoff_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-29 16:22:04.000000 bullmq-1.3.1/bullmq/types/job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-29 16:22:04.000000 bullmq-1.3.1/bullmq/types/keep_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-29 16:22:04.000000 bullmq-1.3.1/bullmq/types/queue_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 16:22:04.000000 bullmq-1.3.1/bullmq/types/retry_job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-29 16:22:04.000000 bullmq-1.3.1/bullmq/types/worker_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-29 16:22:04.000000 bullmq-1.3.1/bullmq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-06-29 16:22:04.000000 bullmq-1.3.1/bullmq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:23:13.751871 bullmq-1.3.1/bullmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-29 16:23:13.000000 bullmq-1.3.1/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-29 16:23:13.000000 bullmq-1.3.1/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:23:13.000000 bullmq-1.3.1/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-29 16:23:13.000000 bullmq-1.3.1/bullmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 16:23:13.000000 bullmq-1.3.1/bullmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-29 16:23:11.000000 bullmq-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 16:23:13.755871 bullmq-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-29 16:22:04.000000 bullmq-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:10.588881 bullmq-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-30 22:04:10.588881 bullmq-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-30 22:02:38.000000 bullmq-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:10.576881 bullmq-1.4.0/bullmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-30 22:04:08.000000 bullmq-1.4.0/bullmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/backoffs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:10.584881 bullmq-1.4.0/bullmq/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/addJob-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/changeDelay-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/changePriority-5.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/drain-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/getState-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/getStateV2-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/moveJobFromActiveToWait-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/moveStalledJobsToWait-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/moveToActive-10.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/moveToFinished-13.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/moveToWaitingChildren-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/pause-5.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/promote-7.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/reprocessJob-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/retryJob-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/retryJobs-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/saveStacktrace-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-30 22:03:34.000000 bullmq-1.4.0/bullmq/commands/updateProgress-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18344 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:10.584881 bullmq-1.4.0/bullmq/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/types/backoff_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/types/job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/types/keep_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/types/queue_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/types/retry_job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/types/worker_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-06-30 22:02:38.000000 bullmq-1.4.0/bullmq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:04:10.576881 bullmq-1.4.0/bullmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-30 22:04:10.000000 bullmq-1.4.0/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-30 22:04:10.000000 bullmq-1.4.0/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:04:10.000000 bullmq-1.4.0/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-30 22:04:10.000000 bullmq-1.4.0/bullmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 22:04:10.000000 bullmq-1.4.0/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-30 22:04:08.000000 bullmq-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 22:04:10.588881 bullmq-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-30 22:02:38.000000 bullmq-1.4.0/setup.py
```

### Comparing `bullmq-1.3.1/PKG-INFO` & `bullmq-1.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 1.3.1
+Version: 1.4.0
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # BullMQ For Python
```

### Comparing `bullmq-1.3.1/README.md` & `bullmq-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/backoffs.py` & `bullmq-1.4.0/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/addJob-9.lua` & `bullmq-1.4.0/bullmq/commands/addJob-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/changeDelay-3.lua` & `bullmq-1.4.0/bullmq/commands/changeDelay-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/changePriority-5.lua` & `bullmq-1.4.0/bullmq/commands/changePriority-5.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-1.4.0/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/drain-4.lua` & `bullmq-1.4.0/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/getCounts-1.lua` & `bullmq-1.4.0/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/getRanges-1.lua` & `bullmq-1.4.0/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/getState-8.lua` & `bullmq-1.4.0/bullmq/commands/getState-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/getStateV2-8.lua` & `bullmq-1.4.0/bullmq/commands/getStateV2-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/isFinished-3.lua` & `bullmq-1.4.0/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/moveJobFromActiveToWait-9.lua` & `bullmq-1.4.0/bullmq/commands/moveJobFromActiveToWait-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/moveStalledJobsToWait-8.lua` & `bullmq-1.4.0/bullmq/commands/moveStalledJobsToWait-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/moveToActive-10.lua` & `bullmq-1.4.0/bullmq/commands/moveToActive-10.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/moveToDelayed-8.lua` & `bullmq-1.4.0/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/moveToFinished-13.lua` & `bullmq-1.4.0/bullmq/commands/moveToFinished-13.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/moveToWaitingChildren-4.lua` & `bullmq-1.4.0/bullmq/commands/moveToWaitingChildren-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/obliterate-2.lua` & `bullmq-1.4.0/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/pause-5.lua` & `bullmq-1.4.0/bullmq/commands/pause-5.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/promote-7.lua` & `bullmq-1.4.0/bullmq/commands/promote-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/removeJob-1.lua` & `bullmq-1.4.0/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/removeRepeatable-2.lua` & `bullmq-1.4.0/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/reprocessJob-6.lua` & `bullmq-1.4.0/bullmq/commands/reprocessJob-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/retryJob-9.lua` & `bullmq-1.4.0/bullmq/commands/retryJob-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/commands/retryJobs-6.lua` & `bullmq-1.4.0/bullmq/commands/retryJobs-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/event_emitter.py` & `bullmq-1.4.0/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/job.py` & `bullmq-1.4.0/bullmq/job.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/queue.py` & `bullmq-1.4.0/bullmq/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,17 @@
         responses = await self.scripts.getCounts(current_types)
         counts = {}
 
         for index, val in enumerate(responses):
             counts[current_types[index]] = val or 0
         return counts
 
+    def getJobState(self, job_id: str):
+        return self.scripts.getState(job_id)
+
     def getCompletedCount(self):
         return self.getJobCountByTypes('completed')
 
     def getFailedCount(self):
         return self.getJobCountByTypes('failed')
 
     def getActive(self, start = 0, end=-1):
```

### Comparing `bullmq-1.3.1/bullmq/redis_connection.py` & `bullmq-1.4.0/bullmq/redis_connection.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/scripts.py` & `bullmq-1.4.0/bullmq/scripts.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/timer.py` & `bullmq-1.4.0/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/types/job_options.py` & `bullmq-1.4.0/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/types/worker_options.py` & `bullmq-1.4.0/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq/worker.py` & `bullmq-1.4.0/bullmq/worker.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/bullmq.egg-info/PKG-INFO` & `bullmq-1.4.0/bullmq.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 1.3.1
+Version: 1.4.0
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # BullMQ For Python
```

### Comparing `bullmq-1.3.1/bullmq.egg-info/SOURCES.txt` & `bullmq-1.4.0/bullmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bullmq-1.3.1/pyproject.toml` & `bullmq-1.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bullmq"
-version = "1.3.1"
+version = "1.4.0"
 description='BullMQ for Python'
 readme="README.md"
 authors = [
     {name = "Taskforce.sh Inc.", email = "manast@taskforce.sh"},
 ]
 classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Operating System :: POSIX :: Linux',
-    'Programming Language :: Python :: 2',
-    'Programming Language :: Python :: 2.7',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.4',
     'Programming Language :: Python :: 3.5',
 ]
 keywords = ["python", "bullmq", "queues"]
 dependencies = [
     "redis >= 4.5.0, < 5",
```

