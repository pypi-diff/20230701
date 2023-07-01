# Comparing `tmp/fastapi_mqtt-1.1.0.tar.gz` & `tmp/fastapi_mqtt-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_mqtt-1.1.0.tar", max compression
+gzip compressed data, was "fastapi_mqtt-1.1.1.tar", max compression
```

## Comparing `fastapi_mqtt-1.1.0.tar` & `fastapi_mqtt-1.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2023-07-01 12:46:41.744277 fastapi_mqtt-1.1.0/LICENSE
--rw-r--r--   0        0        0     3821 2023-07-01 12:46:41.744277 fastapi_mqtt-1.1.0/README.md
--rw-r--r--   0        0        0      319 2023-07-01 12:46:41.748277 fastapi_mqtt-1.1.0/fastapi_mqtt/__init__.py
--rw-r--r--   0        0        0     2217 2023-07-01 12:46:41.748277 fastapi_mqtt-1.1.0/fastapi_mqtt/config.py
--rw-r--r--   0        0        0     9647 2023-07-01 12:46:41.748277 fastapi_mqtt-1.1.0/fastapi_mqtt/fastmqtt.py
--rw-r--r--   0        0        0     1573 2023-07-01 12:46:41.748277 fastapi_mqtt-1.1.0/fastapi_mqtt/handlers.py
--rw-r--r--   0        0        0        1 2023-07-01 12:46:41.748277 fastapi_mqtt-1.1.0/fastapi_mqtt/py.typed
--rw-r--r--   0        0        0     1466 2023-07-01 12:46:55.220411 fastapi_mqtt-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 fastapi_mqtt-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-01 13:01:51.461254 fastapi_mqtt-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3821 2023-07-01 13:01:51.461254 fastapi_mqtt-1.1.1/README.md
+-rw-r--r--   0        0        0      319 2023-07-01 13:01:51.465255 fastapi_mqtt-1.1.1/fastapi_mqtt/__init__.py
+-rw-r--r--   0        0        0     2217 2023-07-01 13:01:51.465255 fastapi_mqtt-1.1.1/fastapi_mqtt/config.py
+-rw-r--r--   0        0        0     9728 2023-07-01 13:01:51.465255 fastapi_mqtt-1.1.1/fastapi_mqtt/fastmqtt.py
+-rw-r--r--   0        0        0     1573 2023-07-01 13:01:51.465255 fastapi_mqtt-1.1.1/fastapi_mqtt/handlers.py
+-rw-r--r--   0        0        0        1 2023-07-01 13:01:51.465255 fastapi_mqtt-1.1.1/fastapi_mqtt/py.typed
+-rw-r--r--   0        0        0     1466 2023-07-01 13:02:07.889745 fastapi_mqtt-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 fastapi_mqtt-1.1.1/PKG-INFO
```

### Comparing `fastapi_mqtt-1.1.0/LICENSE` & `fastapi_mqtt-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_mqtt-1.1.0/README.md` & `fastapi_mqtt-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_mqtt-1.1.0/fastapi_mqtt/config.py` & `fastapi_mqtt-1.1.1/fastapi_mqtt/config.py`

 * *Files identical despite different names*

### Comparing `fastapi_mqtt-1.1.0/fastapi_mqtt/fastmqtt.py` & `fastapi_mqtt-1.1.1/fastapi_mqtt/fastmqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import uuid
 from functools import partial
+from itertools import zip_longest
 from typing import Any, Callable, Dict, Optional
 
 from fastapi import FastAPI
 from gmqtt import Client as MQTTClient
 from gmqtt import Message
 from gmqtt.mqtt.constants import MQTTv50
 
@@ -90,30 +91,27 @@
     def match(topic, template):
         """
         Defined match topics
 
         topic: topic name
         template: template topic name that contains wildcards
         """
-        topic = topic.split("/")
-        template = template.split("/")
+        topic = topic.split('/')
+        template = template.split('/')
 
-        topic_idx = 0
-        for part in template:
-            if part == "#":
+        for topic_part, part in zip_longest(topic, template):
+            if part == '#' and not str(topic_part).startswith("$"):
                 return True
-            elif len(topic) > topic_idx:
-                if part in ["+", topic[topic_idx]]:
-                    topic_idx += 1
-            else:
+            elif topic_part is None or part not in {'+', topic_part}:
                 return False
+            elif part == '+' and topic_part.startswith('$'):
+                return False
+            continue
 
-        if topic_idx == len(topic):
-            return True
-        return False
+        return len(template) == len(topic)
 
     async def connection(self) -> None:
         if self.client._username:
             self.client.set_auth_credentials(
                 self.client._username, self.client._password
             )
             log_info.debug("user is authenticated")
```

### Comparing `fastapi_mqtt-1.1.0/fastapi_mqtt/handlers.py` & `fastapi_mqtt-1.1.1/fastapi_mqtt/handlers.py`

 * *Files identical despite different names*

### Comparing `fastapi_mqtt-1.1.0/pyproject.toml` & `fastapi_mqtt-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-mqtt"
-version = "1.1.0"
+version = "1.1.1"
 description = "fastapi-mqtt is extension for MQTT protocol"
 authors = ["sabuhish <sabuhi.shukurov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/sabuhish/fastapi-mqtt"
 repository = "https://github.com/sabuhish/fastapi-mqtt"
 classifiers = [
```

### Comparing `fastapi_mqtt-1.1.0/PKG-INFO` & `fastapi_mqtt-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-mqtt
-Version: 1.1.0
+Version: 1.1.1
 Summary: fastapi-mqtt is extension for MQTT protocol
 Home-page: https://github.com/sabuhish/fastapi-mqtt
 License: MIT
 Author: sabuhish
 Author-email: sabuhi.shukurov@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
```

