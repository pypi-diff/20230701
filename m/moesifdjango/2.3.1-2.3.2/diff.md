# Comparing `tmp/moesifdjango-2.3.1.tar.gz` & `tmp/moesifdjango-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moesifdjango-2.3.1.tar", last modified: Thu Oct 13 04:06:00 2022, max compression
+gzip compressed data, was "dist/moesifdjango-2.3.2.tar", last modified: Sat Jul  1 00:57:44 2023, max compression
```

## Comparing `moesifdjango-2.3.1.tar` & `moesifdjango-2.3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2022-10-13 04:06:00.756892 moesifdjango-2.3.1/
--rwxr-xr-x   0 praveen    (501) staff       (20)    11918 2022-02-11 21:55:41.000000 moesifdjango-2.3.1/LICENSE
--rw-r--r--   0 praveen    (501) staff       (20)       61 2022-02-11 21:55:41.000000 moesifdjango-2.3.1/MANIFEST.in
--rw-r--r--   0 praveen    (501) staff       (20)    19523 2022-10-13 04:06:00.757002 moesifdjango-2.3.1/PKG-INFO
--rwxr-xr-x   0 praveen    (501) staff       (20)    18400 2022-09-07 20:59:56.000000 moesifdjango-2.3.1/README.md
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2022-10-13 04:06:00.755391 moesifdjango-2.3.1/moesifdjango/
--rw-r--r--   0 praveen    (501) staff       (20)       63 2022-02-11 21:55:41.000000 moesifdjango-2.3.1/moesifdjango/__init__.py
--rw-r--r--   0 praveen    (501) staff       (20)      648 2022-09-07 20:59:56.000000 moesifdjango-2.3.1/moesifdjango/block_response_buffer.py
--rw-r--r--   0 praveen    (501) staff       (20)     4855 2022-02-11 21:55:41.000000 moesifdjango-2.3.1/moesifdjango/client_ip.py
--rw-r--r--   0 praveen    (501) staff       (20)     1504 2022-02-11 21:55:41.000000 moesifdjango-2.3.1/moesifdjango/event_mapper.py
--rw-r--r--   0 praveen    (501) staff       (20)      501 2022-09-07 20:59:56.000000 moesifdjango-2.3.1/moesifdjango/governance_rule_response.py
--rw-r--r--   0 praveen    (501) staff       (20)     2152 2022-09-07 20:59:56.000000 moesifdjango-2.3.1/moesifdjango/governance_rules.py
--rw-r--r--   0 praveen    (501) staff       (20)      616 2022-02-11 21:55:41.000000 moesifdjango-2.3.1/moesifdjango/http_response_catcher.py
--rw-r--r--   0 praveen    (501) staff       (20)     3212 2022-10-13 04:04:23.000000 moesifdjango-2.3.1/moesifdjango/job_scheduler.py
--rw-r--r--   0 praveen    (501) staff       (20)    14517 2022-02-11 21:55:41.000000 moesifdjango-2.3.1/moesifdjango/logger_helper.py
--rw-r--r--   0 praveen    (501) staff       (20)     1403 2022-02-11 21:55:41.000000 moesifdjango-2.3.1/moesifdjango/masks.py
--rw-r--r--   0 praveen    (501) staff       (20)    15993 2022-10-13 04:04:23.000000 moesifdjango-2.3.1/moesifdjango/middleware.py
--rw-r--r--   0 praveen    (501) staff       (20)    13072 2022-10-13 04:04:23.000000 moesifdjango-2.3.1/moesifdjango/middleware_pre19.py
--rw-r--r--   0 praveen    (501) staff       (20)    25796 2022-09-08 01:08:35.000000 moesifdjango-2.3.1/moesifdjango/moesif_gov.py
--rw-r--r--   0 praveen    (501) staff       (20)     2471 2022-09-07 20:59:56.000000 moesifdjango-2.3.1/moesifdjango/parse_body.py
--rw-r--r--   0 praveen    (501) staff       (20)     6657 2022-02-11 21:55:41.000000 moesifdjango-2.3.1/moesifdjango/update_companies.py
--rw-r--r--   0 praveen    (501) staff       (20)     6381 2022-02-11 21:55:41.000000 moesifdjango-2.3.1/moesifdjango/update_users.py
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2022-10-13 04:06:00.756051 moesifdjango-2.3.1/moesifdjango.egg-info/
--rw-r--r--   0 praveen    (501) staff       (20)    19523 2022-10-13 04:06:00.000000 moesifdjango-2.3.1/moesifdjango.egg-info/PKG-INFO
--rw-r--r--   0 praveen    (501) staff       (20)      861 2022-10-13 04:06:00.000000 moesifdjango-2.3.1/moesifdjango.egg-info/SOURCES.txt
--rw-r--r--   0 praveen    (501) staff       (20)        1 2022-10-13 04:06:00.000000 moesifdjango-2.3.1/moesifdjango.egg-info/dependency_links.txt
--rw-r--r--   0 praveen    (501) staff       (20)      136 2022-10-13 04:06:00.000000 moesifdjango-2.3.1/moesifdjango.egg-info/requires.txt
--rw-r--r--   0 praveen    (501) staff       (20)       19 2022-10-13 04:06:00.000000 moesifdjango-2.3.1/moesifdjango.egg-info/top_level.txt
--rw-r--r--   0 praveen    (501) staff       (20)       67 2022-10-13 04:06:00.757325 moesifdjango-2.3.1/setup.cfg
--rw-r--r--   0 praveen    (501) staff       (20)     3363 2022-10-13 04:04:23.000000 moesifdjango-2.3.1/setup.py
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2022-10-13 04:06:00.751110 moesifdjango-2.3.1/tests/
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2022-10-13 04:06:00.756265 moesifdjango-2.3.1/tests/middleware_pre19_tests/
--rw-r--r--   0 praveen    (501) staff       (20)        0 2022-02-11 21:55:41.000000 moesifdjango-2.3.1/tests/middleware_pre19_tests/__init__.py
--rw-r--r--   0 praveen    (501) staff       (20)     4990 2022-02-11 21:55:41.000000 moesifdjango-2.3.1/tests/middleware_pre19_tests/tests.py
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2022-10-13 04:06:00.756653 moesifdjango-2.3.1/tests/middleware_tests/
--rw-r--r--   0 praveen    (501) staff       (20)        0 2022-02-11 21:55:41.000000 moesifdjango-2.3.1/tests/middleware_tests/__init__.py
--rw-r--r--   0 praveen    (501) staff       (20)     5266 2022-09-07 20:59:56.000000 moesifdjango-2.3.1/tests/middleware_tests/tests.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-07-01 00:57:44.613497 moesifdjango-2.3.2/
+-rwxr-xr-x   0 keyur      (501) staff       (20)    11918 2020-12-27 23:18:46.000000 moesifdjango-2.3.2/LICENSE
+-rw-r--r--   0 keyur      (501) staff       (20)       61 2020-05-04 14:40:14.000000 moesifdjango-2.3.2/MANIFEST.in
+-rw-r--r--   0 keyur      (501) staff       (20)    23072 2023-07-01 00:57:44.614194 moesifdjango-2.3.2/PKG-INFO
+-rwxr-xr-x   0 keyur      (501) staff       (20)    18400 2022-07-12 17:48:38.000000 moesifdjango-2.3.2/README.md
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-07-01 00:57:44.602151 moesifdjango-2.3.2/moesifdjango/
+-rw-r--r--   0 keyur      (501) staff       (20)       63 2020-05-04 14:40:14.000000 moesifdjango-2.3.2/moesifdjango/__init__.py
+-rw-r--r--   0 keyur      (501) staff       (20)      666 2023-07-01 00:56:37.000000 moesifdjango-2.3.2/moesifdjango/block_response_buffer.py
+-rw-r--r--   0 keyur      (501) staff       (20)     4855 2020-12-29 03:43:47.000000 moesifdjango-2.3.2/moesifdjango/client_ip.py
+-rw-r--r--   0 keyur      (501) staff       (20)     1570 2023-07-01 00:56:37.000000 moesifdjango-2.3.2/moesifdjango/event_mapper.py
+-rw-r--r--   0 keyur      (501) staff       (20)      555 2023-07-01 00:56:37.000000 moesifdjango-2.3.2/moesifdjango/governance_rule_response.py
+-rw-r--r--   0 keyur      (501) staff       (20)     2152 2022-07-12 17:48:38.000000 moesifdjango-2.3.2/moesifdjango/governance_rules.py
+-rw-r--r--   0 keyur      (501) staff       (20)      616 2020-05-04 14:40:14.000000 moesifdjango-2.3.2/moesifdjango/http_response_catcher.py
+-rw-r--r--   0 keyur      (501) staff       (20)     3212 2023-06-30 20:29:59.000000 moesifdjango-2.3.2/moesifdjango/job_scheduler.py
+-rw-r--r--   0 keyur      (501) staff       (20)    14517 2021-07-08 18:25:55.000000 moesifdjango-2.3.2/moesifdjango/logger_helper.py
+-rw-r--r--   0 keyur      (501) staff       (20)     1403 2020-12-29 05:09:32.000000 moesifdjango-2.3.2/moesifdjango/masks.py
+-rw-r--r--   0 keyur      (501) staff       (20)    17343 2023-07-01 00:56:37.000000 moesifdjango-2.3.2/moesifdjango/middleware.py
+-rw-r--r--   0 keyur      (501) staff       (20)    14371 2023-06-30 20:31:52.000000 moesifdjango-2.3.2/moesifdjango/middleware_pre19.py
+-rw-r--r--   0 keyur      (501) staff       (20)    25617 2023-07-01 00:56:37.000000 moesifdjango-2.3.2/moesifdjango/moesif_gov.py
+-rw-r--r--   0 keyur      (501) staff       (20)     2471 2022-07-12 17:48:38.000000 moesifdjango-2.3.2/moesifdjango/parse_body.py
+-rw-r--r--   0 keyur      (501) staff       (20)     6657 2020-12-29 03:47:33.000000 moesifdjango-2.3.2/moesifdjango/update_companies.py
+-rw-r--r--   0 keyur      (501) staff       (20)     6381 2020-12-29 03:47:52.000000 moesifdjango-2.3.2/moesifdjango/update_users.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-07-01 00:57:44.609494 moesifdjango-2.3.2/moesifdjango.egg-info/
+-rw-r--r--   0 keyur      (501) staff       (20)    23072 2023-07-01 00:57:44.000000 moesifdjango-2.3.2/moesifdjango.egg-info/PKG-INFO
+-rw-r--r--   0 keyur      (501) staff       (20)      861 2023-07-01 00:57:44.000000 moesifdjango-2.3.2/moesifdjango.egg-info/SOURCES.txt
+-rw-r--r--   0 keyur      (501) staff       (20)        1 2023-07-01 00:57:44.000000 moesifdjango-2.3.2/moesifdjango.egg-info/dependency_links.txt
+-rw-r--r--   0 keyur      (501) staff       (20)      136 2023-07-01 00:57:44.000000 moesifdjango-2.3.2/moesifdjango.egg-info/requires.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       19 2023-07-01 00:57:44.000000 moesifdjango-2.3.2/moesifdjango.egg-info/top_level.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       67 2023-07-01 00:57:44.615083 moesifdjango-2.3.2/setup.cfg
+-rw-r--r--   0 keyur      (501) staff       (20)     3363 2023-07-01 00:56:37.000000 moesifdjango-2.3.2/setup.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-07-01 00:57:44.571308 moesifdjango-2.3.2/tests/
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-07-01 00:57:44.610762 moesifdjango-2.3.2/tests/middleware_pre19_tests/
+-rw-r--r--   0 keyur      (501) staff       (20)        0 2020-05-04 14:40:14.000000 moesifdjango-2.3.2/tests/middleware_pre19_tests/__init__.py
+-rw-r--r--   0 keyur      (501) staff       (20)     4990 2020-12-29 19:17:16.000000 moesifdjango-2.3.2/tests/middleware_pre19_tests/tests.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-07-01 00:57:44.612281 moesifdjango-2.3.2/tests/middleware_tests/
+-rw-r--r--   0 keyur      (501) staff       (20)        0 2020-05-04 14:40:14.000000 moesifdjango-2.3.2/tests/middleware_tests/__init__.py
+-rw-r--r--   0 keyur      (501) staff       (20)     5266 2022-07-12 17:48:38.000000 moesifdjango-2.3.2/tests/middleware_tests/tests.py
```

### Comparing `moesifdjango-2.3.1/LICENSE` & `moesifdjango-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.1/PKG-INFO` & `moesifdjango-2.3.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: moesifdjango
-Version: 2.3.1
-Summary: Moesif Middleware for Python Django
-Home-page: https://www.moesif.com/docs/server-integration/django/
-Author: Moesif, Inc
-Author-email: derric@moesif.com
-License: Apache Software License
-Keywords: log analysis restful api development debug
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Internet :: Log Analysis
-Classifier: Topic :: Software Development :: Debuggers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE
-
 # Moesif Middleware for Python Django
 
 [![Built For][ico-built-for]][link-built-for]
 [![Latest Version][ico-version]][link-package]
 [![Language Versions][ico-language]][link-language]
 [![Software License][ico-license]][link-license]
 [![Source Code][ico-source]][link-source]
@@ -468,9 +439,7 @@
 [ico-source]: https://img.shields.io/github/last-commit/moesif/moesifdjango.svg?style=social
 
 [link-built-for]: https://www.djangoproject.com/
 [link-package]: https://pypi.python.org/pypi/moesifdjango
 [link-language]: https://pypi.python.org/pypi/moesifdjango
 [link-license]: https://raw.githubusercontent.com/Moesif/moesifdjango/master/LICENSE
 [link-source]: https://github.com/Moesif/moesifdjango
-
-
```

### Comparing `moesifdjango-2.3.1/moesifdjango/block_response_buffer.py` & `moesifdjango-2.3.2/moesifdjango/block_response_buffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 class BlockResponseBufferList:
     def __init__(self):
         self.responses = []
         self.rule_type = None
         self.blocked = False
 
-    def update(self, block, updated_gr_status, updated_gr_headers, updated_gr_body):
+    def update(self, block, updated_gr_status, updated_gr_headers, updated_gr_body, rule_id):
         if not self.rule_type:
             self.rule_type = 'regex'
         if block and not self.blocked:
             self.blocked = True
 
         gov_rule_response = GovernanceRuleBlockResponse()
-        gov_rule_response.update_response(updated_gr_status, updated_gr_headers, updated_gr_body, block)
+        gov_rule_response.update_response(updated_gr_status, updated_gr_headers, updated_gr_body, block, rule_id)
         self.responses.append(gov_rule_response)
```

### Comparing `moesifdjango-2.3.1/moesifdjango/client_ip.py` & `moesifdjango-2.3.2/moesifdjango/client_ip.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.1/moesifdjango/event_mapper.py` & `moesifdjango-2.3.2/moesifdjango/event_mapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,16 +22,17 @@
         return EventResponseModel(time=rsp_time,
                                   status=status_code,
                                   headers=rsp_headers,
                                   body=rsp_body,
                                   transfer_encoding=transfer_encoding)
 
     @classmethod
-    def to_event(cls, event_req, event_rsp, user_id, company_id, session_token, metadata):
+    def to_event(cls, event_req, event_rsp, user_id, company_id, session_token, metadata, blocked_by=None):
         # Prepare Event Model
         return EventModel(request=event_req,
                           response=event_rsp,
                           user_id=user_id,
                           company_id=company_id,
                           session_token=session_token,
                           metadata=metadata,
-                          direction="Incoming")
+                          direction="Incoming",
+                          blocked_by=blocked_by)
```

### Comparing `moesifdjango-2.3.1/moesifdjango/governance_rules.py` & `moesifdjango-2.3.2/moesifdjango/governance_rules.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.1/moesifdjango/http_response_catcher.py` & `moesifdjango-2.3.2/moesifdjango/http_response_catcher.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.1/moesifdjango/job_scheduler.py` & `moesifdjango-2.3.2/moesifdjango/job_scheduler.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.1/moesifdjango/logger_helper.py` & `moesifdjango-2.3.2/moesifdjango/logger_helper.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.1/moesifdjango/masks.py` & `moesifdjango-2.3.2/moesifdjango/masks.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.1/moesifdjango/middleware.py` & `moesifdjango-2.3.2/moesifdjango/middleware.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from .job_scheduler import JobScheduler
 from apscheduler.schedulers.background import BackgroundScheduler
 from apscheduler.triggers.interval import IntervalTrigger
 from apscheduler.events import EVENT_JOB_ERROR, EVENT_JOB_EXECUTED
 import atexit
 from .moesif_gov import *
 from .parse_body import ParseBody
+from apscheduler.schedulers.base import STATE_STOPPED
 
 
 class moesif_middleware:
     def __init__(self, get_response):
         self.get_response = get_response
         # One-time configuration and initialization.
         self.middleware_settings = settings.MOESIF_MIDDLEWARE
@@ -81,22 +82,19 @@
         self.gov_rules_cacher = GovernanceRulesCacher(self.api_client)
         self.user_governance_rules, self.company_governance_rules, self.regex_governance_rules \
             = self.gov_rules_cacher.generate_rules_caching(self.DEBUG)
 
         self.sampling_percentage = 100
         self.config_etag = None
         self.rules_etag = None
-
         self.last_updated_time = datetime.utcnow()
-        self.last_event_job_run_time = datetime(1970, 1, 1, 0, 0)  # Assuming job never ran, set it to epoch start time
-        self.scheduler = None
+        self._reset_scheduler()
         self.event_queue_size = self.middleware_settings.get('EVENT_QUEUE_SIZE', 10000)
         self.mo_events_queue = queue.Queue(maxsize=self.event_queue_size)
         self.event_batch_size = self.middleware_settings.get('BATCH_SIZE', 25)
-        self.is_event_job_scheduled = False
         try:
             if self.config:
                 self.config_etag, self.sampling_percentage, self.last_updated_time = self.app_config.parse_configuration(
                     self.config, self.DEBUG)
         except Exception as e:
             if self.DEBUG:
                 print('Error while parsing application configuration on initialization')
@@ -277,45 +275,80 @@
 
             response.status_code = updated_Response.block_response_status
             event_rsp = self.event_mapper.to_response(rsp_time, updated_Response.block_response_status,
                                                       updated_Response.block_response_headers, rsp_body,
                                                       rsp_body_transfer_encoding)
             # Prepare Event Model
             event_model = self.event_mapper.to_event(event_req, event_rsp, user_id, company_id, session_token,
-                                                     metadata)
+                                                     metadata, updated_Response.blocked_by)
 
             # Mask Event Model
             event_model = self.logger_helper.mask_event(event_model, self.middleware_settings, self.DEBUG)
 
         # Create random percentage
         random_percentage = random.random() * 100
         self.sampling_percentage = self.app_config.get_sampling_percentage(event_model, self.config, user_id, company_id)
         if self.sampling_percentage >= random_percentage:
             event_model.weight = 1 if self.sampling_percentage == 0 else math.floor(100 / self.sampling_percentage)
             try:
-                if not self.is_event_job_scheduled and datetime.utcnow() > self.last_event_job_run_time + timedelta(minutes=5):
-                    try:
-                        self.schedule_event_background_job()
-                        self.is_event_job_scheduled = True
-                        self.last_event_job_run_time = datetime.utcnow()
-                    except Exception as ex:
-                        self.is_event_job_scheduled = False
-                        if self.DEBUG:
-                            print('Error while starting the event scheduler job in background')
-                            print(str(ex))
+                # Create scheduler if needed
+                self._create_scheduler_if_needed()
+
                 if self.DEBUG:
-                    print("Add Event to the queue")
+                    print("Add Event to the queue: ", self.mo_events_queue.qsize())
                 self.mo_events_queue.put(event_model)
             except Exception as ex:
                 if self.DEBUG:
                     print("Error while adding event to the queue")
                     print(str(ex))
 
         return response
 
+    def _reset_scheduler(self):
+        """
+        Private Method to reset scheduler to original `init` (aka null) state.
+        """
+        try:
+            # try to  clean up before resetting
+            self.scheduler.remove_job('moesif_events_batch_job')
+            self.scheduler.shutdown()
+        except Exception as es:
+            # ignore because either schedule is null or job is null
+            # cleanup is not needed
+            pass
+        finally:
+            print("----- Event scheduler will start on next event.")
+            # Reset initialize it so that next time schedule job is called it gets created again.
+            self.scheduler = None
+            self.is_event_job_scheduled = False
+            self.last_event_job_run_time = datetime(1970, 1, 1, 0, 0)  # Assuming job never ran, set it to epoch start time
+
+    def _create_scheduler_if_needed(self):
+        """
+        Private method to create scheduler if:
+           1. first time OR
+           2. It exists but is in stopped state - so any subsequent add_job will throw exceptions.
+        """
+        # Check if scheduler exist but in stopped state (for some reason stopped by app/diff middlewares)
+        # Reset it so that it can be restarted
+        if self.scheduler and self.scheduler.state == STATE_STOPPED:
+            self._reset_scheduler()
+
+        # Create scheduler if needed
+        if not self.is_event_job_scheduled and datetime.utcnow() > self.last_event_job_run_time + timedelta(minutes=5):
+            try:
+                self.schedule_event_background_job()
+                self.is_event_job_scheduled = True
+                self.last_event_job_run_time = datetime.utcnow()
+            except Exception as ex:
+                self.is_event_job_scheduled = False
+                if self.DEBUG:
+                    print('Error while starting the event scheduler job in background')
+                    print(str(ex))
+
     def update_user(self, user_profile):
         self.user.update_user(user_profile, self.api_client, self.DEBUG)
 
     def update_users_batch(self, user_profiles):
         self.user.update_users_batch(user_profiles, self.api_client, self.DEBUG)
 
     def update_company(self, company_profile):
```

### Comparing `moesifdjango-2.3.1/moesifdjango/middleware_pre19.py` & `moesifdjango-2.3.2/moesifdjango/middleware_pre19.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from .logger_helper import LoggerHelper
 from .event_mapper import EventMapper
 from .job_scheduler import JobScheduler
 from apscheduler.schedulers.background import BackgroundScheduler
 from apscheduler.triggers.interval import IntervalTrigger
 from apscheduler.events import EVENT_JOB_ERROR, EVENT_JOB_EXECUTED
 import atexit
+from apscheduler.schedulers.base import STATE_STOPPED
 
 class MoesifMiddlewarePre19(object):
 
     # One-time configuration and initialization.
     def __init__(self):
         self.middleware_settings = settings.MOESIF_MIDDLEWARE
         self.DEBUG = self.middleware_settings.get('LOCAL_DEBUG', False)
@@ -67,20 +68,19 @@
         self.mask_helper = MaskData()
         self.user = User()
         self.company = Company()
         self.config = self.app_config.get_config(self.api_client, self.DEBUG)
         self.sampling_percentage = 100
         self.config_etag = None
         self.last_updated_time = datetime.utcnow()
-        self.last_event_job_run_time = datetime(1970, 1, 1, 0, 0)  # Assuming job never ran, set it to epoch start time
-        self.scheduler = None
+        self._reset_scheduler()
         self.event_queue_size = self.middleware_settings.get('EVENT_QUEUE_SIZE', 10000)
         self.mo_events_queue = queue.Queue(maxsize=self.event_queue_size)
         self.event_batch_size = self.middleware_settings.get('BATCH_SIZE', 25)
-        self.is_event_job_scheduled = False
+
         try:
             if self.config:
                 self.config_etag, self.sampling_percentage, self.last_updated_time = self.app_config.parse_configuration(
                     self.config, self.DEBUG)
         except:
             if self.DEBUG:
                 print('Error while parsing application configuration on initialization')
@@ -236,35 +236,70 @@
 
         # Create random percentage
         random_percentage = random.random() * 100
         self.sampling_percentage = self.app_config.get_sampling_percentage(event_model, self.config, user_id, company_id)
         if self.sampling_percentage >= random_percentage:
             event_model.weight = 1 if self.sampling_percentage == 0 else math.floor(100 / self.sampling_percentage)
             try:
-                if not self.is_event_job_scheduled and datetime.utcnow() > self.last_event_job_run_time + timedelta(
-                        minutes=5):
-                    try:
-                        self.schedule_event_background_job()
-                        self.is_event_job_scheduled = True
-                        self.last_event_job_run_time = datetime.utcnow()
-                    except Exception as ex:
-                        self.is_event_job_scheduled = False
-                        if self.DEBUG:
-                            print('Error while starting the event scheduler job in background')
-                            print(str(ex))
+                # Create scheduler if needed
+                self._create_scheduler_if_needed()
                 if self.DEBUG:
-                    print("Add Event to the queue")
+                    print("Add Event to the queue: ", self.mo_events_queue.qsize())
                 self.mo_events_queue.put(event_model)
             except Exception as ex:
                 if self.DEBUG:
                     print("Error while adding event to the queue")
                     print(str(ex))
 
         return response
 
+    def _reset_scheduler(self):
+        """
+        Private Method to reset scheduler to original `init` (aka null) state.
+        """
+
+        try:
+            # try to  clean up before resetting
+            self.scheduler.remove_job('moesif_events_batch_job')
+            self.scheduler.shutdown()
+        except Exception as es:
+            # ignore because either schedule is null or job is null
+            # cleanup is not needed
+            pass
+        finally:
+            print("----- Event scheduler will start on next event.")
+
+            # Reset initialize it so that next time schedule job is called it gets created again.
+            self.scheduler = None
+            self.is_event_job_scheduled = False
+            self.last_event_job_run_time = datetime(1970, 1, 1, 0, 0)  # Assuming job never ran, set it to epoch start time
+
+    def _create_scheduler_if_needed(self):
+        """
+        Private method to create scheduler if:
+           1. first time OR
+           2. It exists but is in stopped state - so any subsequent add_job will throw exceptions.
+        """
+        # Check if scheduler exist but in stopped state (for some reason stopped by app/diff middlewares)
+        # Reset it so that it can be restarted
+        if self.scheduler and self.scheduler.state == STATE_STOPPED:
+            self._reset_scheduler()
+
+        # Create scheduler if needed
+        if not self.is_event_job_scheduled and datetime.utcnow() > self.last_event_job_run_time + timedelta(minutes=5):
+            try:
+                self.schedule_event_background_job()
+                self.is_event_job_scheduled = True
+                self.last_event_job_run_time = datetime.utcnow()
+            except Exception as ex:
+                self.is_event_job_scheduled = False
+                if self.DEBUG:
+                    print('Error while starting the event scheduler job in background')
+                    print(str(ex))
+
     def update_user(self, user_profile):
         self.user.update_user(user_profile, self.api_client, self.DEBUG)
 
     def update_users_batch(self, user_profiles):
         self.user.update_users_batch(user_profiles, self.api_client, self.DEBUG)
 
     def update_company(self, company_profile):
```

### Comparing `moesifdjango-2.3.1/moesifdjango/moesif_gov.py` & `moesifdjango-2.3.2/moesifdjango/moesif_gov.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,15 +355,15 @@
                 continue
 
             # update response status, headers and body if one block rule matched
             updated_gr_status, updated_gr_headers, updated_gr_body = self.get_updated_response_with_matched_rules(
                 governance_rule, rule_and_values)
 
             block = governance_rule.get('block', False)
-            response_buffer.update(block, updated_gr_status, updated_gr_headers, updated_gr_body)
+            response_buffer.update(block, updated_gr_status, updated_gr_headers, updated_gr_body, rule_id)
 
             if DEBUG:
                 print("[moesif] request matched with rule_id [{}]".format(rule_id))
 
         return response_buffer
 
     def get_rules_id_if_governance_rule_matched(self, regex_governance_rules, event, ready_for_body_request):
@@ -388,55 +388,48 @@
                 try:
                     matched_rules_id.append(rule['_id'])
                 except KeyError as ke:
                     print('[moesif] Error when fetching matched regex governance rule ', ke)
 
         return matched_rules_id
 
-    def block_request_based_on_governance_rule_regex_config(self, event, ready_for_body_request, regex_governance_rules,
-                                                            DEBUG):
+    def block_request_based_on_governance_rule_regex_config(self, event, ready_for_body_request, regex_governance_rules, DEBUG):
         """
         Check if need to block request based on the governance rule regex config associated with the request
         :param event:
         :param ready_for_body_request:
         :param regex_governance_rules:
         :param DEBUG:
         :return:
         """
 
         response_buffer = BlockResponseBufferList()
-        matched_rules_id = self.get_rules_id_if_governance_rule_matched(regex_governance_rules, event,
-                                                                        ready_for_body_request)
-
-        if not matched_rules_id:
-            if DEBUG:
-                print('[moesif] no regex rule matched with the request')
-        else:
-            for rule_id in matched_rules_id:
-                governance_rule = regex_governance_rules.get(rule_id)
-                if not governance_rule:
-                    if DEBUG:
-                        print(
-                            '[moesif] Skipped blocking request as rule {} is not found'.format(rule_id))
-                        continue
-
-                if 'response' not in governance_rule \
-                        or 'status' not in governance_rule['response'] \
-                        or 'headers' not in governance_rule['response']:
-                    if DEBUG:
-                        print(
-                            '[moesif] Skipped blocking request as response is not set for the governance rule with regex config')
+        matched_rules_id = self.get_rules_id_if_governance_rule_matched(regex_governance_rules, event, ready_for_body_request)
+        for rule_id in matched_rules_id:
+            governance_rule = regex_governance_rules.get(rule_id)
+            if not governance_rule:
+                if DEBUG:
+                    print(
+                        '[moesif] Skipped blocking request as rule {} is not found'.format(rule_id))
                     continue
 
-                block = governance_rule.get('block', False)
-                gr_status, gr_header, gr_body = self.fetch_governance_rule_response_details(governance_rule)
-
-                response_buffer.update(block, gr_status, gr_header, gr_body)
+            if 'response' not in governance_rule \
+                    or 'status' not in governance_rule['response'] \
+                    or 'headers' not in governance_rule['response']:
                 if DEBUG:
-                    print('[moesif] request matched with regex rule with rule_id {}'.format(rule_id))
+                    print('[moesif] Skipped blocking request as response is not set for the governance rule with regex config')
+                continue
+
+            block = governance_rule.get('block', False)
+            gr_status, gr_header, gr_body = self.fetch_governance_rule_response_details(governance_rule)
+
+            response_buffer.update(block, gr_status, gr_header, gr_body, rule_id)
+            if DEBUG:
+                print('[moesif] request matched with regex rule with rule_id {}'.format(rule_id))
+
         return response_buffer
 
     # TODO can deal with request.body in one place
     @classmethod
     def prepare_request_config_based_on_regex_config(cls, event: EventModel, ready_for_body_request):
         """
         fetch regex config from config mapping
@@ -477,40 +470,44 @@
         if event.response.status:
             regex_config['response.status'] = event.response.status
 
         return regex_config
 
     def generate_blocking_response(self, response_buffers):
         """
-        rearrange matching rules' response, merge all of the headers, and ordered by the rules type priority
+        rearrange matching rules' response, merge all the headers, and ordered by the rules type priority
         updated response_body and response_status with the highest priority blocked rule
 
         :param response_buffers:
         :return: None if none of the rules is blocking request, otherwise return the blocking response
         """
         if not self.check_if_request_blocked(response_buffers):
             return None
 
         updated_body = None
         updated_status = None
         updated_headers = {}
+        blocked_by = None
+        blocked = False
 
         for rule_type in REVERSED_PRIORITY_RULES_ORDER:
             if rule_type in response_buffers:
                 buffer = response_buffers.get(rule_type, None)
                 if buffer:
                     responses = buffer.responses
                     for response in responses:
                         if response.blocked:
                             updated_body = response.block_response_body
                             updated_status = response.block_response_status
+                            blocked_by = response.blocked_by
+                            blocked = response.blocked
                         updated_headers.update(response.block_response_headers)
 
         gov_rule_response = GovernanceRuleBlockResponse()
-        gov_rule_response.update_response(updated_status, updated_headers, updated_body, True)
+        gov_rule_response.update_response(updated_status, updated_headers, updated_body, blocked, blocked_by)
         return gov_rule_response
 
     @classmethod
     def check_if_request_blocked(cls, response_buffers):
         for rule_type in REVERSED_PRIORITY_RULES_ORDER:
             if rule_type in response_buffers:
                 response = response_buffers[rule_type]
```

### Comparing `moesifdjango-2.3.1/moesifdjango/parse_body.py` & `moesifdjango-2.3.2/moesifdjango/parse_body.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.1/moesifdjango/update_companies.py` & `moesifdjango-2.3.2/moesifdjango/update_companies.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.1/moesifdjango/update_users.py` & `moesifdjango-2.3.2/moesifdjango/update_users.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.1/moesifdjango.egg-info/SOURCES.txt` & `moesifdjango-2.3.2/moesifdjango.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.1/setup.py` & `moesifdjango-2.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 setup(
     name='moesifdjango',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='2.3.1',
+    version='2.3.2',
 
     description='Moesif Middleware for Python Django',
     long_description=long_description,
     long_description_content_type="text/markdown",
     
     # The project's main homepage.
     url='https://www.moesif.com/docs/server-integration/django/',
@@ -78,15 +78,15 @@
     # simple. Or you can use find_packages().
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
 
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['requests', 'jsonpickle', 'python-dateutil', 'isodatetimehandler', 'moesifapi>=1.4.0',
+    install_requires=['requests', 'jsonpickle', 'python-dateutil', 'isodatetimehandler', 'moesifapi>=1.4.1',
                       'moesifpythonrequest>=0.3.0', 'apscheduler', 'nose'],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
     # $ pip install -e .[dev,test]
     extras_require={
```

### Comparing `moesifdjango-2.3.1/tests/middleware_pre19_tests/tests.py` & `moesifdjango-2.3.2/tests/middleware_pre19_tests/tests.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.1/tests/middleware_tests/tests.py` & `moesifdjango-2.3.2/tests/middleware_tests/tests.py`

 * *Files identical despite different names*

