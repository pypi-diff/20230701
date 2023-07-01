# Comparing `tmp/fastapi_mqtt-1.0.9.tar.gz` & `tmp/fastapi_mqtt-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_mqtt-1.0.9.tar", max compression
+gzip compressed data, was "fastapi_mqtt-1.1.0.tar", max compression
```

## Comparing `fastapi_mqtt-1.0.9.tar` & `fastapi_mqtt-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2023-05-21 08:27:56.921850 fastapi_mqtt-1.0.9/LICENSE
--rw-r--r--   0        0        0     3465 2023-05-21 08:27:56.921850 fastapi_mqtt-1.0.9/README.md
--rw-r--r--   0        0        0      319 2023-05-21 08:27:56.921850 fastapi_mqtt-1.0.9/fastapi_mqtt/__init__.py
--rw-r--r--   0        0        0     2217 2023-05-21 08:27:56.921850 fastapi_mqtt-1.0.9/fastapi_mqtt/config.py
--rw-r--r--   0        0        0     9473 2023-05-21 08:27:56.925850 fastapi_mqtt-1.0.9/fastapi_mqtt/fastmqtt.py
--rw-r--r--   0        0        0     1573 2023-05-21 08:27:56.925850 fastapi_mqtt-1.0.9/fastapi_mqtt/handlers.py
--rw-r--r--   0        0        0        1 2023-05-21 08:27:56.925850 fastapi_mqtt-1.0.9/fastapi_mqtt/py.typed
--rw-r--r--   0        0        0     1069 2023-05-21 08:28:12.954568 fastapi_mqtt-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     4568 1970-01-01 00:00:00.000000 fastapi_mqtt-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-01 12:46:41.744277 fastapi_mqtt-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3821 2023-07-01 12:46:41.744277 fastapi_mqtt-1.1.0/README.md
+-rw-r--r--   0        0        0      319 2023-07-01 12:46:41.748277 fastapi_mqtt-1.1.0/fastapi_mqtt/__init__.py
+-rw-r--r--   0        0        0     2217 2023-07-01 12:46:41.748277 fastapi_mqtt-1.1.0/fastapi_mqtt/config.py
+-rw-r--r--   0        0        0     9647 2023-07-01 12:46:41.748277 fastapi_mqtt-1.1.0/fastapi_mqtt/fastmqtt.py
+-rw-r--r--   0        0        0     1573 2023-07-01 12:46:41.748277 fastapi_mqtt-1.1.0/fastapi_mqtt/handlers.py
+-rw-r--r--   0        0        0        1 2023-07-01 12:46:41.748277 fastapi_mqtt-1.1.0/fastapi_mqtt/py.typed
+-rw-r--r--   0        0        0     1466 2023-07-01 12:46:55.220411 fastapi_mqtt-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 fastapi_mqtt-1.1.0/PKG-INFO
```

### Comparing `fastapi_mqtt-1.0.9/LICENSE` & `fastapi_mqtt-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_mqtt-1.0.9/README.md` & `fastapi_mqtt-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -112,14 +112,25 @@
 
 
 mqtt = FastMQTT(
     config=mqtt_config)
 
 ```
 
+### ✅ Testing
+
+Run tests with `pytest`, using an external MQTT broker to connect (defaults to 'test.mosquitto.org').
+
+```sh
+ # (opc) Run a local mosquitto MQTT broker with docker
+ $ docker run -d --name mosquitto -p 9001:9001 -p 1883:1883 eclipse-mosquitto:1.6.15
+ # Set host for test broker when running pytest
+ $ TEST_BROKER_HOST=localhost pytest
+```
+
 # Contributing
 
 Fell free to open issue and send pull request.
 
 Thanks To [Contributors](https://github.com/sabuhish/fastapi-mqtt/graphs/contributors).
 Contributions of any kind are welcome!
```

### Comparing `fastapi_mqtt-1.0.9/fastapi_mqtt/config.py` & `fastapi_mqtt-1.1.0/fastapi_mqtt/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     The last three parameters are used after the client disconnects abnormally
 
     will_message_topic: Topic of the payload
     will_message_payload: The payload
     will_delay_interval: Delay interval
     """
 
-    host: str = 'localhost'
+    host: str = "localhost"
     port: int = 1883
     ssl: Union[bool, SSLContext] = False
     keepalive: int = 60
     username: Optional[str] = None
     password: Optional[str] = None
     version: int = MQTTv50
```

### Comparing `fastapi_mqtt-1.0.9/fastapi_mqtt/fastmqtt.py` & `fastapi_mqtt-1.1.0/fastapi_mqtt/fastmqtt.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,101 +78,108 @@
         ):
             self.client._will_message = Message(
                 self.config.will_message_topic,
                 self.config.will_message_payload,
                 will_delay_interval=self.config.will_delay_interval,
             )
             log_info.debug(
-                f'topic -> {self.config.will_message_topic} \n payload -> {self.config.will_message_payload} \n will_delay_interval -> {self.config.will_delay_interval}'  # noqa E501
+                f"topic -> {self.config.will_message_topic} \n payload -> {self.config.will_message_payload} \n will_delay_interval -> {self.config.will_delay_interval}"  # noqa E501
             )
-            log_info.debug('WILL MESSAGE INITIALIZED')
+            log_info.debug("WILL MESSAGE INITIALIZED")
 
     @staticmethod
     def match(topic, template):
         """
         Defined match topics
 
         topic: topic name
         template: template topic name that contains wildcards
         """
-        topic = topic.split('/')
-        template = template.split('/')
+        topic = topic.split("/")
+        template = template.split("/")
 
         topic_idx = 0
         for part in template:
-            if part == '#':
+            if part == "#":
                 return True
-            elif part in ['+', topic[topic_idx]]:
-                topic_idx += 1
+            elif len(topic) > topic_idx:
+                if part in ["+", topic[topic_idx]]:
+                    topic_idx += 1
             else:
                 return False
 
         if topic_idx == len(topic):
             return True
         return False
 
     async def connection(self) -> None:
-
         if self.client._username:
-            self.client.set_auth_credentials(self.client._username, self.client._password)
-            log_info.debug('user is authenticated')
+            self.client.set_auth_credentials(
+                self.client._username, self.client._password
+            )
+            log_info.debug("user is authenticated")
 
         await self.__set_connetion_config()
 
         version = self.config.version or MQTTv50
-        log_info.warning(f'Used broker version is {version}')
+        log_info.warning(f"Used broker version is {version}")
 
         await self.client.connect(
             self.client._host,
             self.client._port,
             self.client._ssl,
             self.client._keepalive,
             version,
         )
-        log_info.debug('connected to broker..')
+        log_info.debug("connected to broker..")
 
     async def __set_connetion_config(self) -> None:
         """
         The connected MQTT clients will always try to reconnect in case of lost connections.
         The number of reconnect attempts is unlimited.
         For changing this behavior, set reconnect_retries and reconnect_delay with its values.
         For more info: https://github.com/wialon/gmqtt#reconnects
         """
-        self.client.set_config({
-            "reconnect_retries":self.config.reconnect_retries,
-            "reconnect_delay": self.config.reconnect_delay})
-     
+        self.client.set_config(
+            {
+                "reconnect_retries": self.config.reconnect_retries,
+                "reconnect_delay": self.config.reconnect_delay,
+            }
+        )
+
     def __on_connect(self, client, flags, rc, properties) -> None:
         """
         Generic on connecting handler, it would call user handler if defined.
         Will perform subscription for given topics.
         It cannot be done earlier, since subscription relies on connection.
         """
         if self.mqtt_handlers.get_user_connect_handler:
             self.mqtt_handlers.get_user_connect_handler(client, flags, rc, properties)
 
         for topic in self.handlers.keys():
-            log_info.debug(f'Subscribing for {topic}')
+            log_info.debug(f"Subscribing for {topic}")
             self.client.subscribe(topic)
 
     async def __on_message(self, client, topic, payload, qos, properties):
         """
         Generic on message handler, it will call user handler if defined.
         This will invoke per topic handlers that are subscribed for
         """
         gather = []
         if self.mqtt_handlers.get_user_message_handler:
-            log_info.debug('Calling user_message_handler')
+            log_info.debug("Calling user_message_handler")
             gather.append(
-                self.mqtt_handlers.get_user_message_handler(client, topic, payload, qos, properties)
+                self.mqtt_handlers.get_user_message_handler(
+                    client, topic, payload, qos, properties
+                )
             )
 
         for topic_template in self.handlers.keys():
             if self.match(topic, topic_template):
-                log_info.debug(f'Calling specific handler for topic {topic}')
+                log_info.debug(f"Calling specific handler for topic {topic}")
                 for handler in self.handlers[topic_template]:
                     gather.append(handler(client, topic, payload, qos, properties))
 
         return await asyncio.gather(*gather)
 
     def publish(
         self,
@@ -200,36 +207,36 @@
     def unsubscribe(self, topic: str, **kwargs):
         """
         Defined to unsubscribe topic
 
         topic: topic name
         """
         partial(self.client.unsubscribe, topic, **kwargs)
-        log_info.debug('unsubscribe')
+        log_info.debug("unsubscribe")
         if topic in self.handlers.keys():
             del self.handlers[topic]
 
         return self.client.unsubscribe(topic, **kwargs)
 
-    def init_app(self, app: FastAPI) -> None:
-        @app.on_event('startup')
+    def init_app(self, app: FastAPI) -> None:  # pragma: no cover
+        @app.on_event("startup")
         async def startup():
             await self.connection()
 
-        @app.on_event('shutdown')
+        @app.on_event("shutdown")
         async def shutdown():
             await self.client.disconnect()
 
     def subscribe(self, *topics) -> Callable[..., Any]:
         """
         Decorator method used to subscribe for specific topics.
         """
 
         def subscribe_handler(handler: Callable) -> Callable:
-            log_info.debug(f'Subscribe for a topics: {topics}')
+            log_info.debug(f"Subscribe for a topics: {topics}")
             for topic in topics:
                 if topic not in self.handlers.keys():
                     self.handlers[topic] = []
                 # TODO: Consider changing to weak_ref
                 self.handlers[topic].append(handler)
             return handler
 
@@ -237,44 +244,44 @@
 
     def on_connect(self) -> Callable[..., Any]:
         """
         Decorator method used to handle the connection to MQTT.
         """
 
         def connect_handler(handler: Callable) -> Callable:
-            log_info.debug('handler accepted')
+            log_info.debug("handler accepted")
             return self.mqtt_handlers.on_connect(handler)
 
         return connect_handler
 
     def on_message(self) -> Callable[..., Any]:
         """
         The decorator method is used to subscribe to messages from all topics.
         """
 
         def message_handler(handler: Callable) -> Callable:
-            log_info.debug('on_message handler accepted')
+            log_info.debug("on_message handler accepted")
             return self.mqtt_handlers.on_message(handler)
 
         return message_handler
 
     def on_disconnect(self) -> Callable[..., Any]:
         """
         The Decorator method used wrap disconnect callback.
         """
 
         def disconnect_handler(handler: Callable) -> Callable:
-            log_info.debug('on_disconnect handler accepted')
+            log_info.debug("on_disconnect handler accepted")
             return self.mqtt_handlers.on_disconnect(handler)
 
         return disconnect_handler
 
     def on_subscribe(self) -> Callable[..., Any]:
         """
         Decorator method is used to obtain subscribed topics and properties.
         """
 
         def subscribe_handler(handler: Callable):
-            log_info.debug('on_subscribe handler accepted')
+            log_info.debug("on_subscribe handler accepted")
             return self.mqtt_handlers.on_subscribe(handler)
 
         return subscribe_handler
```

### Comparing `fastapi_mqtt-1.0.9/fastapi_mqtt/handlers.py` & `fastapi_mqtt-1.1.0/fastapi_mqtt/handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,32 +16,32 @@
     def __init__(self, client: MQTTClient, handlers: dict):
         self.client = client
         self.handlers = handlers
         self.user_message_handler: Optional[Callable[..., Any]] = None
         self.user_connect_handler: Optional[Callable[..., Any]] = None
 
     def on_message(self, handler: Callable) -> Callable[..., Any]:
-        log_info.info('on_message handler accepted')
+        log_info.info("on_message handler accepted")
         self.user_message_handler = handler
         return handler
 
     def on_subscribe(self, handler: Callable) -> Callable[..., Any]:
         """
         Decorator method is used to obtain subscribed topics and properties.
         """
-        log_info.info('on_subscribe handler accepted')
+        log_info.info("on_subscribe handler accepted")
         self.client.on_subscribe = handler
         return handler
 
     def on_disconnect(self, handler: Callable) -> Callable[..., Any]:
         self.client.on_disconnect = handler
         return handler
 
     def on_connect(self, handler: Callable) -> Callable[..., Any]:
-        log_info.info('on_connect handler accepted')
+        log_info.info("on_connect handler accepted")
         self.user_connect_handler = handler
         return handler
 
     @property
     def get_user_message_handler(self) -> Optional[Callable[..., Any]]:
         return self.user_message_handler
```

### Comparing `fastapi_mqtt-1.0.9/PKG-INFO` & `fastapi_mqtt-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-mqtt
-Version: 1.0.9
+Version: 1.1.0
 Summary: fastapi-mqtt is extension for MQTT protocol
 Home-page: https://github.com/sabuhish/fastapi-mqtt
 License: MIT
 Author: sabuhish
 Author-email: sabuhi.shukurov@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
+Requires-Dist: black (>=23.3.0,<24.0.0)
 Requires-Dist: fastapi (==0.*)
 Requires-Dist: gmqtt (>=0.6.11,<0.7.0)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: uvicorn (>=0.19.0)
 Project-URL: Repository, https://github.com/sabuhish/fastapi-mqtt
 Description-Content-Type: text/markdown
 
@@ -140,14 +141,25 @@
 
 
 mqtt = FastMQTT(
     config=mqtt_config)
 
 ```
 
+### ✅ Testing
+
+Run tests with `pytest`, using an external MQTT broker to connect (defaults to 'test.mosquitto.org').
+
+```sh
+ # (opc) Run a local mosquitto MQTT broker with docker
+ $ docker run -d --name mosquitto -p 9001:9001 -p 1883:1883 eclipse-mosquitto:1.6.15
+ # Set host for test broker when running pytest
+ $ TEST_BROKER_HOST=localhost pytest
+```
+
 # Contributing
 
 Fell free to open issue and send pull request.
 
 Thanks To [Contributors](https://github.com/sabuhish/fastapi-mqtt/graphs/contributors).
 Contributions of any kind are welcome!
```

