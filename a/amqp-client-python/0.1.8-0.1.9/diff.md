# Comparing `tmp/amqp_client_python-0.1.8.tar.gz` & `tmp/amqp_client_python-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amqp_client_python-0.1.8.tar", max compression
+gzip compressed data, was "amqp_client_python-0.1.9.tar", max compression
```

## Comparing `amqp_client_python-0.1.8.tar` & `amqp_client_python-0.1.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    11356 2023-01-27 16:26:08.907959 amqp_client_python-0.1.8/LICENSE
--rw-r--r--   0        0        0     7641 2023-02-04 19:57:51.088835 amqp_client_python-0.1.8/README.md
--rw-r--r--   0        0        0      142 2023-02-04 19:38:34.636689 amqp_client_python-0.1.8/amqp_client_python/__init__.py
--rw-r--r--   0        0        0       92 2023-02-01 02:17:56.487032 amqp_client_python-0.1.8/amqp_client_python/domain/models/__init__.py
--rw-r--r--   0        0        0     1307 2023-02-08 14:55:41.843240 amqp_client_python-0.1.8/amqp_client_python/domain/models/config.py
--rw-r--r--   0        0        0      190 2023-01-31 15:35:31.488741 amqp_client_python-0.1.8/amqp_client_python/domain/models/connection_type.py
--rw-r--r--   0        0        0      880 2023-02-03 21:23:38.023131 amqp_client_python-0.1.8/amqp_client_python/domain/models/options.py
--rw-r--r--   0        0        0        0 2023-02-03 14:58:38.862370 amqp_client_python-0.1.8/amqp_client_python/domain/models/provider_config.py
--rw-r--r--   0        0        0        0 2023-02-03 14:58:19.414410 amqp_client_python-0.1.8/amqp_client_python/domain/models/publish_config.py
--rw-r--r--   0        0        0      304 2023-02-06 12:15:36.745229 amqp_client_python-0.1.8/amqp_client_python/domain/models/ssl_options.py
--rw-r--r--   0        0        0        0 2023-02-03 14:58:47.730351 amqp_client_python-0.1.8/amqp_client_python/domain/models/sub_config.py
--rw-r--r--   0        0        0      110 2023-01-27 16:26:08.907959 amqp_client_python-0.1.8/amqp_client_python/event/__init__.py
--rw-r--r--   0        0        0      249 2023-01-27 16:26:08.907959 amqp_client_python-0.1.8/amqp_client_python/event/integration_event.py
--rw-r--r--   0        0        0      165 2023-01-27 16:26:08.907959 amqp_client_python-0.1.8/amqp_client_python/event/integration_event_handler.py
--rw-r--r--   0        0        0      385 2023-02-04 19:38:34.636689 amqp_client_python-0.1.8/amqp_client_python/exceptions/__init__.py
--rw-r--r--   0        0        0      282 2023-02-04 19:38:34.636689 amqp_client_python-0.1.8/amqp_client_python/exceptions/auto_reconnect_exception.py
--rw-r--r--   0        0        0      215 2023-01-27 16:26:08.907959 amqp_client_python-0.1.8/amqp_client_python/exceptions/eventbus_exception.py
--rw-r--r--   0        0        0      270 2023-01-27 16:26:08.907959 amqp_client_python-0.1.8/amqp_client_python/exceptions/nack_exception.py
--rw-r--r--   0        0        0      278 2023-02-03 21:23:38.027131 amqp_client_python-0.1.8/amqp_client_python/exceptions/publish_timeout_exception.py
--rw-r--r--   0        0        0      278 2023-02-03 21:23:38.027131 amqp_client_python-0.1.8/amqp_client_python/exceptions/response_timeout_exception.py
--rw-r--r--   0        0        0      277 2023-01-27 16:26:08.907959 amqp_client_python-0.1.8/amqp_client_python/exceptions/rpc_provider_exception.py
--rw-r--r--   0        0        0      273 2023-01-27 16:26:08.907959 amqp_client_python-0.1.8/amqp_client_python/exceptions/timeout_exception.py
--rw-r--r--   0        0        0      614 2023-02-04 19:38:34.636689 amqp_client_python-0.1.8/amqp_client_python/rabbitmq/__init__.py
--rw-r--r--   0        0        0    20738 2023-02-08 15:32:33.970972 amqp_client_python-0.1.8/amqp_client_python/rabbitmq/async_channel.py
--rw-r--r--   0        0        0      259 2023-02-08 13:23:11.187584 amqp_client_python-0.1.8/amqp_client_python/rabbitmq/async_channel_factory.py
--rw-r--r--   0        0        0     8318 2023-02-08 14:55:41.843240 amqp_client_python-0.1.8/amqp_client_python/rabbitmq/async_connection.py
--rw-r--r--   0        0        0      698 2023-02-08 13:49:05.255401 amqp_client_python-0.1.8/amqp_client_python/rabbitmq/async_connection_factory.py
--rw-r--r--   0        0        0     3150 2023-02-04 19:38:34.636689 amqp_client_python-0.1.8/amqp_client_python/rabbitmq/async_eventbus_rabbitmq.py
--rw-r--r--   0        0        0      224 2023-02-07 11:22:22.124702 amqp_client_python-0.1.8/amqp_client_python/rabbitmq/channel_factory_rabbitmq.py
--rw-r--r--   0        0        0      926 2023-02-02 12:53:44.399072 amqp_client_python-0.1.8/amqp_client_python/rabbitmq/channel_pool.py
--rw-r--r--   0        0        0    11867 2023-02-04 19:38:34.640689 amqp_client_python-0.1.8/amqp_client_python/rabbitmq/channel_rabbitmq.py
--rw-r--r--   0        0        0      880 2023-02-04 19:07:03.926063 amqp_client_python-0.1.8/amqp_client_python/rabbitmq/connection_factory_rabbitmq.py
--rw-r--r--   0        0        0     8486 2023-02-04 19:06:59.142291 amqp_client_python-0.1.8/amqp_client_python/rabbitmq/connection_rabbitmq.py
--rw-r--r--   0        0        0     5214 2023-02-04 19:38:34.640689 amqp_client_python-0.1.8/amqp_client_python/rabbitmq/eventbus_rabbitmq.py
--rw-r--r--   0        0        0     2963 2023-02-04 19:38:34.640689 amqp_client_python-0.1.8/amqp_client_python/rabbitmq/eventbus_wrapper_rabbitmq.py
--rw-r--r--   0        0        0      823 2023-02-04 00:04:38.942248 amqp_client_python-0.1.8/amqp_client_python/rabbitmq/ioloop_factory.py
--rw-r--r--   0        0        0      658 2023-02-08 15:42:34.069155 amqp_client_python-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     8611 1970-01-01 00:00:00.000000 amqp_client_python-0.1.8/setup.py
--rw-r--r--   0        0        0     8293 1970-01-01 00:00:00.000000 amqp_client_python-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-01-27 16:26:08.907959 amqp_client_python-0.1.9/LICENSE
+-rw-r--r--   0        0        0     7641 2023-02-04 19:57:51.088835 amqp_client_python-0.1.9/README.md
+-rw-r--r--   0        0        0      142 2023-02-04 19:38:34.636689 amqp_client_python-0.1.9/amqp_client_python/__init__.py
+-rw-r--r--   0        0        0       92 2023-02-01 02:17:56.487032 amqp_client_python-0.1.9/amqp_client_python/domain/models/__init__.py
+-rw-r--r--   0        0        0     1307 2023-02-13 22:35:03.415027 amqp_client_python-0.1.9/amqp_client_python/domain/models/config.py
+-rw-r--r--   0        0        0      190 2023-01-31 15:35:31.488741 amqp_client_python-0.1.9/amqp_client_python/domain/models/connection_type.py
+-rw-r--r--   0        0        0      880 2023-02-03 21:23:38.023131 amqp_client_python-0.1.9/amqp_client_python/domain/models/options.py
+-rw-r--r--   0        0        0        0 2023-02-03 14:58:38.862370 amqp_client_python-0.1.9/amqp_client_python/domain/models/provider_config.py
+-rw-r--r--   0        0        0        0 2023-02-03 14:58:19.414410 amqp_client_python-0.1.9/amqp_client_python/domain/models/publish_config.py
+-rw-r--r--   0        0        0      304 2023-02-06 12:15:36.745229 amqp_client_python-0.1.9/amqp_client_python/domain/models/ssl_options.py
+-rw-r--r--   0        0        0        0 2023-02-03 14:58:47.730351 amqp_client_python-0.1.9/amqp_client_python/domain/models/sub_config.py
+-rw-r--r--   0        0        0      110 2023-01-27 16:26:08.907959 amqp_client_python-0.1.9/amqp_client_python/event/__init__.py
+-rw-r--r--   0        0        0      249 2023-01-27 16:26:08.907959 amqp_client_python-0.1.9/amqp_client_python/event/integration_event.py
+-rw-r--r--   0        0        0      165 2023-01-27 16:26:08.907959 amqp_client_python-0.1.9/amqp_client_python/event/integration_event_handler.py
+-rw-r--r--   0        0        0      385 2023-02-04 19:38:34.636689 amqp_client_python-0.1.9/amqp_client_python/exceptions/__init__.py
+-rw-r--r--   0        0        0      282 2023-02-04 19:38:34.636689 amqp_client_python-0.1.9/amqp_client_python/exceptions/auto_reconnect_exception.py
+-rw-r--r--   0        0        0      215 2023-01-27 16:26:08.907959 amqp_client_python-0.1.9/amqp_client_python/exceptions/eventbus_exception.py
+-rw-r--r--   0        0        0      270 2023-01-27 16:26:08.907959 amqp_client_python-0.1.9/amqp_client_python/exceptions/nack_exception.py
+-rw-r--r--   0        0        0      278 2023-02-03 21:23:38.027131 amqp_client_python-0.1.9/amqp_client_python/exceptions/publish_timeout_exception.py
+-rw-r--r--   0        0        0      278 2023-02-03 21:23:38.027131 amqp_client_python-0.1.9/amqp_client_python/exceptions/response_timeout_exception.py
+-rw-r--r--   0        0        0      277 2023-01-27 16:26:08.907959 amqp_client_python-0.1.9/amqp_client_python/exceptions/rpc_provider_exception.py
+-rw-r--r--   0        0        0      273 2023-01-27 16:26:08.907959 amqp_client_python-0.1.9/amqp_client_python/exceptions/timeout_exception.py
+-rw-r--r--   0        0        0      614 2023-02-04 19:38:34.636689 amqp_client_python-0.1.9/amqp_client_python/rabbitmq/__init__.py
+-rw-r--r--   0        0        0    22864 2023-02-13 22:35:03.415027 amqp_client_python-0.1.9/amqp_client_python/rabbitmq/async_channel.py
+-rw-r--r--   0        0        0      259 2023-02-08 13:23:11.187584 amqp_client_python-0.1.9/amqp_client_python/rabbitmq/async_channel_factory.py
+-rw-r--r--   0        0        0     8613 2023-02-13 22:35:03.415027 amqp_client_python-0.1.9/amqp_client_python/rabbitmq/async_connection.py
+-rw-r--r--   0        0        0      698 2023-02-08 13:49:05.255401 amqp_client_python-0.1.9/amqp_client_python/rabbitmq/async_connection_factory.py
+-rw-r--r--   0        0        0     3884 2023-02-13 22:35:03.415027 amqp_client_python-0.1.9/amqp_client_python/rabbitmq/async_eventbus_rabbitmq.py
+-rw-r--r--   0        0        0      224 2023-02-07 11:22:22.124702 amqp_client_python-0.1.9/amqp_client_python/rabbitmq/channel_factory_rabbitmq.py
+-rw-r--r--   0        0        0      926 2023-02-02 12:53:44.399072 amqp_client_python-0.1.9/amqp_client_python/rabbitmq/channel_pool.py
+-rw-r--r--   0        0        0    11867 2023-02-04 19:38:34.640689 amqp_client_python-0.1.9/amqp_client_python/rabbitmq/channel_rabbitmq.py
+-rw-r--r--   0        0        0      880 2023-02-04 19:07:03.926063 amqp_client_python-0.1.9/amqp_client_python/rabbitmq/connection_factory_rabbitmq.py
+-rw-r--r--   0        0        0     8486 2023-02-04 19:06:59.142291 amqp_client_python-0.1.9/amqp_client_python/rabbitmq/connection_rabbitmq.py
+-rw-r--r--   0        0        0     5214 2023-02-04 19:38:34.640689 amqp_client_python-0.1.9/amqp_client_python/rabbitmq/eventbus_rabbitmq.py
+-rw-r--r--   0        0        0     3758 2023-02-13 22:35:03.419026 amqp_client_python-0.1.9/amqp_client_python/rabbitmq/eventbus_wrapper_rabbitmq.py
+-rw-r--r--   0        0        0      823 2023-02-04 00:04:38.942248 amqp_client_python-0.1.9/amqp_client_python/rabbitmq/ioloop_factory.py
+-rw-r--r--   0        0        0      658 2023-02-13 22:37:21.515191 amqp_client_python-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     8611 1970-01-01 00:00:00.000000 amqp_client_python-0.1.9/setup.py
+-rw-r--r--   0        0        0     8293 1970-01-01 00:00:00.000000 amqp_client_python-0.1.9/PKG-INFO
```

### Comparing `amqp_client_python-0.1.8/LICENSE` & `amqp_client_python-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `amqp_client_python-0.1.8/README.md` & `amqp_client_python-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `amqp_client_python-0.1.8/amqp_client_python/domain/models/config.py` & `amqp_client_python-0.1.9/amqp_client_python/domain/models/config.py`

 * *Files identical despite different names*

### Comparing `amqp_client_python-0.1.8/amqp_client_python/domain/models/options.py` & `amqp_client_python-0.1.9/amqp_client_python/domain/models/options.py`

 * *Files identical despite different names*

### Comparing `amqp_client_python-0.1.8/amqp_client_python/rabbitmq/__init__.py` & `amqp_client_python-0.1.9/amqp_client_python/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `amqp_client_python-0.1.8/amqp_client_python/rabbitmq/async_channel.py` & `amqp_client_python-0.1.9/amqp_client_python/rabbitmq/async_channel.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     PublishTimeoutException,
     ResponseTimeoutException,
     EventBusException,
 )
 from pika.adapters.asyncio_connection import AsyncioConnection
 from pika.channel import Channel
 from pika import BasicProperties
-from asyncio import AbstractEventLoop, Future
+from asyncio import AbstractEventLoop, Future, wait, wait_for, FIRST_COMPLETED
 from functools import partial
 from json import dumps, loads
 from uuid import uuid4
 import logging
 
 
 LOGGER = logging.getLogger(__name__)
@@ -30,23 +30,27 @@
         self.ioloop: AbstractEventLoop = None
         self.channel_factory = channel_factory
         self._channel: Channel = None
         self._connection: AsyncioConnection = None
         self._callback_queue = f"amqp.{uuid4()}"
         self.futures: MutableMapping[str, Mapping[str, Future]] = {}
         self.rpc_consumer = False
-        self.rpc_publisher = False
+        self.rpc_consumer_started = False
+        self.rpc_consumer_starting = False
+        self.rpc_publisher_started = False
+        self.rpc_publisher_starting = False
         self.consumer_tag = None
         self._prefetch_count = prefetch_count
         self.auto_ack = auto_ack
         self.subscribes = {}
         self.consumers = {}
         self.publisher_confirms = False
         self._message_number = 0
         self._deliveries = {}
+        self.response_timeout = 60
 
     @property
     def is_open(self):
         return self._channel and self._channel.is_open
 
     def open(self, connection: AsyncioConnection):
         if not self.is_open:
@@ -62,15 +66,15 @@
         Since the channel is now open, we"ll declare the exchange to use.
         :param pika.channel.Channel channel: The channel object
         """
         LOGGER.info("Channel opened")
         self._channel = channel
         self.add_on_channel_close_callback()
         self.publisher_confirms and self.add_publish_confirms()
-        self.set_qos(self._prefetch_count)
+        self._prefetch_count and self.set_qos(self._prefetch_count)
 
     def add_on_channel_close_callback(self):
         """This method tells pika to call the on_channel_closed method if
         RabbitMQ unexpectedly closes the channel.
         """
         LOGGER.debug("Adding channel close callback")
         self._channel.add_on_close_callback(self.on_channel_closed)
@@ -91,32 +95,31 @@
         else:
             LOGGER.info("Closing connection")
             self._connection.close()
 
     def add_publish_confirms(self):
         self._acked = 0
         self._nacked = 0
-        self._deliveries = {}
+        self._deliveries: MutableMapping[int, Future] = {}
         self._message_number = 0
         self._channel.confirm_delivery(self.on_delivery_confirmation)
         LOGGER.info("Adding Publish Confirmation")
 
     def on_delivery_confirmation(self, method_frame):
         confirmation_type = method_frame.method.NAME.split(".")[1].lower()
         delivery_tag = method_frame.method.delivery_tag
-
         if confirmation_type == "ack":
             self._acked += 1
-            if self._deliveries[delivery_tag] == delivery_tag:
-                future = self.futures[delivery_tag]
+            if delivery_tag in self._deliveries:
+                future = self._deliveries[delivery_tag]
                 not future.done() and future.set_result(True)
         elif confirmation_type == "nack":
             self._nacked += 1
-            if self._deliveries[delivery_tag] in self.futures:
-                future = self.futures[self._deliveries[delivery_tag]]["published"]
+            if delivery_tag in self._deliveries:
+                future = self._deliveries[delivery_tag]
                 not future.done() and future.set_exception(
                     NackException(
                         f"Publish confirmation: nack of {delivery_tag} publish"
                     )
                 )
 
     def setup_exchange(self, exchange_name, exchange_type, durable=True):
@@ -210,108 +213,120 @@
             if not future.done():
                 if properties.type == "error":
                     future.set_exception(
                         RpcProviderException(f"Provider Error: {body.decode()}")
                     )
                 else:
                     future.set_result(body)
-            return not self.auto_ack and self._channel.basic_ack(
+            return not self.auto_ack and self._channel_rpc.basic_ack(
                 basic_deliver.delivery_tag
             )
-        not self.auto_ack and self._channel.basic_nack(
+        not self.auto_ack and self._channel_rpc.basic_nack(
             basic_deliver.delivery_tag, requeue=False
         )
 
     def unsubscribe(self, consumer_tag: str):
-        self.rpc_consumer = False
+        self.rpc_consumer_started = False
+        if self.rpc_consumer_starting and not self.rpc_consumer_future.done():
+            self.rpc_consumer_future.cancel()
         self._channel.basic_cancel(consumer_tag)
 
     async def start_rpc_consumer(self):
-        self.rpc_consumer = True
-        consumer_future = self.ioloop.create_future()
+        if self.rpc_consumer_started:
+            return True
+        if self.rpc_consumer_starting:
+            return await self.rpc_consumer_future
+        self.rpc_consumer_starting = True
+
+        self.rpc_consumer_future = self.ioloop.create_future()
         LOGGER.info("Starting rpc consumer")
 
         def on_open(channel: Channel):
             LOGGER.info("Channel opened - consumer")
             self._channel_rpc.add_on_close_callback(self.on_channel_closed)
 
             def on_declare(channel):
-                self.consumer_tag = self._channel.basic_consume(
+                self.consumer_tag = self._channel_rpc.basic_consume(
                     queue=self._callback_queue,
                     on_message_callback=self.on_response,
                     auto_ack=self.auto_ack,
                     consumer_tag=None,
                 )
-                consumer_future.set_result(True)
+                self.rpc_consumer_started = True
+                self.rpc_consumer_starting = False
+                self.rpc_consumer_future.set_result(True)
 
             LOGGER.info(f"Declaring queue {self._callback_queue}")
             self._channel_rpc.queue_declare(
                 queue=self._callback_queue,
                 durable=False,
                 auto_delete=True,
                 callback=on_declare,
             )
 
         self._channel_rpc: Channel = self.channel_factory.create_channel(
             self._connection, on_channel_open=on_open
         )
 
-        def attemp_failed(future: Future):
-            if not future.done():
-                self.rpc_consumer = False
-                future.set_exception(
+        def attemp_failed():
+            if not self.rpc_consumer_future.done():
+                self.rpc_consumer_started = False
+                self.rpc_consumer_starting = False
+                self.rpc_consumer_future.set_exception(
                     EventBusException("Error: cannot set rpc_consumer")
                 )
 
-        func = partial(attemp_failed, consumer_future)
-        self.ioloop.call_later(2, func)
-        await consumer_future
+        self.ioloop.call_later(2, attemp_failed)
+        return await self.rpc_consumer_future
 
     async def start_rpc_publisher(self):
-        self.rpc_publisher = True
-        publish_future = self.ioloop.create_future()
+        if self.rpc_publisher_started:
+            return True
+        if self.rpc_publisher_starting:
+            return await self.rpc_consumer_future
+        self.rpc_publisher_starting = True
+        self.rpc_publisher_future = self.ioloop.create_future()
 
         def on_open(channel: Channel):
             self._channel_rpc.add_on_close_callback(self.on_channel_closed)
-            publish_future.set_result(True)
+            self.rpc_publisher_started = True
+            self.rpc_publisher_starting = False
+            self.rpc_publisher_future.set_result(True)
 
         self._channel_rpc: Channel = self.channel_factory.create_channel(
             self._connection, on_channel_open=on_open
         )
 
-        def attemp_failed(future: Future):
-            if not future.done():
-                self.rpc_publisher = False
-                future.set_exception(
+        def attemp_failed():
+            if not self.rpc_publisher_future.done():
+                self.rpc_publisher_started = False
+                self.rpc_publisher_starting = False
+                self.rpc_publisher_future.set_exception(
                     EventBusException("Error: cannot set rpc_publisher")
                 )
 
-        func = partial(attemp_failed, publish_future)
-        self.ioloop.call_later(2, func)
-        await publish_future
+        self.ioloop.call_later(2, attemp_failed)
+        return await self.rpc_publisher_future
 
     async def rpc_client(
         self,
         exchange_name: str,
         routing_key: str,
         body,
         content_type,
         timeout,
-        loop: AbstractEventLoop,
     ):
-        future = loop.create_future()
-        publish_future = loop.create_future()
+        future = self.ioloop.create_future()
         message = dumps({"resource_name": routing_key, "handle": body})
         corr_id = str(uuid4())
-        self.futures[corr_id] = {"response": future, "published": publish_future}
+        self.futures[corr_id] = {"response": future}
         clean_response = partial(self.clean_rpc_response, corr_id)
         future.add_done_callback(clean_response)
 
-        if not self.rpc_consumer:
-            await self.start_rpc_consumer()
+        await self.start_rpc_consumer()
 
         self._channel.basic_publish(
             exchange_name,
             routing_key,
             message,
             properties=BasicProperties(
                 reply_to=self._callback_queue,
@@ -321,30 +336,44 @@
         )
 
         def not_arrived(id):
             if id in self.futures:
                 future = self.futures[id]
                 if self.publisher_confirms and not future["published"].done():
                     return future["published"].set_exception(
-                        PublishTimeoutException("Timeout: time limit reached")
+                        PublishTimeoutException("PublishTimeout: time limit reached")
                     )
                 if not future["response"].done():
                     return future["response"].set_exception(
-                        ResponseTimeoutException("Timeout: time limit reached")
+                        ResponseTimeoutException("ResponseTimeout: time limit reached")
                     )
 
         func = partial(not_arrived, corr_id)
-        loop.call_later(timeout, func)
+        self.ioloop.call_later(timeout, func)
 
         if self.publisher_confirms:
-            self.publish_confirmation(publish_future)
-            await publish_future
-
+            return await self.handle_publish(future, corr_id)
         return await future
 
+    async def handle_publish(self, future, corr_id):
+        publish_future = self.ioloop.create_future()
+        self.futures[corr_id]["published"] = publish_future
+        self.publish_confirmation(publish_future)
+        done_all, pending_all = await wait(
+            [publish_future, future], return_when=FIRST_COMPLETED
+        )
+        exception = done_all.pop().exception()
+        if exception:
+            [undone.cancel() for undone in pending_all]
+            raise exception
+        elif len(pending_all):
+            return await future
+        else:
+            return future.result()
+
     async def publish(
         self,
         exchange_name: str,
         routing_key: str,
         body,
         content_type: str,
         timeout=5,
@@ -373,15 +402,15 @@
             func = partial(not_arrived, self._message_number)
             loop.call_later(timeout, func)
             return await publish_future
 
     def publish_confirmation(self, future: Future):
         self._message_number += 1
         self.futures[self._message_number] = future
-        self._deliveries[self._message_number] = self._message_number
+        self._deliveries[self._message_number] = future
         clean = partial(self.clean_publish_confirmation, self._message_number)
         future.add_done_callback(clean)
 
     def clean_publish_confirmation(self, meassage_id, _fut):
         self.futures.pop(meassage_id)
         self._deliveries.pop(meassage_id)
 
@@ -390,20 +419,26 @@
 
     async def rpc_subscribe(
         self,
         exchange_name,
         routing_key: str,
         queue_name: str,
         callback,
+        response_timeout,
         content_type="application/json",
         exchange_type="direct",
     ):
-        if not self.rpc_publisher:
-            await self.start_rpc_publisher()
-        self.add_subscribe(queue_name, routing_key, callback, content_type=content_type)
+        await self.start_rpc_publisher()
+        self.add_subscribe(
+            queue_name,
+            routing_key,
+            callback,
+            content_type=content_type,
+            response_timeout=response_timeout,
+        )
         self.setup_exchange(exchange_name, exchange_type)
         self.queue_declare(queue_name)
         self.queue_bind(queue_name, exchange_name, routing_key)
         if queue_name not in self.consumers:
             self.consumers[queue_name] = True
             func = partial(self.on_message, queue_name)
             self._channel.basic_consume(
@@ -412,18 +447,25 @@
 
     async def subscribe(
         self,
         exchange_name,
         routing_key: str,
         queue_name: str,
         callback,
+        response_timeout,
         content_type="application/json",
         exchange_type="direct",
     ):
-        self.add_subscribe(queue_name, routing_key, callback, content_type=content_type)
+        self.add_subscribe(
+            queue_name,
+            routing_key,
+            callback,
+            content_type=content_type,
+            response_timeout=response_timeout,
+        )
         self.setup_exchange(exchange_name, exchange_type)
         self.queue_declare(queue_name, durable=True)
         self.queue_bind(queue_name, exchange_name, routing_key)
         if queue_name not in self.consumers:
             self.consumers[queue_name] = True
             func = partial(self.on_message, queue_name)
             self._channel.basic_consume(
@@ -441,54 +483,59 @@
         is the message that was sent.
         :param pika.channel.Channel _unused_channel: The channel object
         :param pika.Spec.Basic.Deliver: basic_deliver method
         :param pika.Spec.BasicProperties: properties
         :param bytes body: The message body
         """
 
-        async def handle_message(body):
+        async def handle_message(queue_name, basic_deliver, props, body):
             try:
                 if basic_deliver.routing_key in self.subscribes[queue_name]:
                     body = loads(body)
-                    response = await self.subscribes[queue_name][
-                        basic_deliver.routing_key
-                    ]["handle"](*body["handle"])
-                    if self.rpc_publisher and response and props.reply_to:
+                    response = await wait_for(
+                        self.subscribes[queue_name][basic_deliver.routing_key][
+                            "handle"
+                        ](*body["handle"]),
+                        timeout=self.subscribes[queue_name][basic_deliver.routing_key][
+                            "response_timeout"
+                        ],
+                    )
+                    if self.rpc_publisher_started and response and props.reply_to:
                         self._channel_rpc.basic_publish(
                             "",
                             props.reply_to,
                             response,
                             properties=BasicProperties(
                                 correlation_id=props.correlation_id,
                                 content_type=self.subscribes[queue_name][
                                     basic_deliver.routing_key
                                 ]["content_type"],
                                 type="normal",
                             ),
                         )
-                    not self.auto_ack and self._channel.basic_ack(
+                    not self.auto_ack and not self._channel.basic_ack(
                         basic_deliver.delivery_tag
                     )
                 else:
-                    if self.rpc_publisher and props.reply_to:
+                    if self.rpc_publisher_started and props.reply_to:
                         self._channel_rpc.basic_publish(
                             "",
                             props.reply_to,
                             "Provider Error: routing_key not binded",
                             properties=BasicProperties(
                                 correlation_id=props.correlation_id,
                                 content_type="text/plain",
                                 type="error",
                             ),
                         )
                     not self.auto_ack and self._channel.basic_nack(
                         basic_deliver.delivery_tag, requeue=False
                     )
             except BaseException as err:
-                if self.rpc_publisher and props.reply_to:
+                if self.rpc_publisher_started and props.reply_to:
                     self._channel_rpc.basic_publish(
                         "",
                         props.reply_to,
                         str(err),
                         properties=BasicProperties(
                             correlation_id=props.correlation_id,
                             content_type=self.subscribes[queue_name][
@@ -497,18 +544,21 @@
                             type="error",
                         ),
                     )
                 not self.auto_ack and self._channel.basic_nack(
                     basic_deliver.delivery_tag, requeue=False
                 )
 
-        self.ioloop.create_task(handle_message(body))
+        self.ioloop.create_task(handle_message(queue_name, basic_deliver, props, body))
 
-    def add_subscribe(self, queue_name, routing_key, handle, content_type):
+    def add_subscribe(
+        self, queue_name, routing_key, handle, content_type, response_timeout=None
+    ):
         if queue_name not in self.subscribes:
             if not len(self.subscribes):
                 self.subscribes[queue_name] = {}
         if routing_key not in self.subscribes[queue_name]:
             self.subscribes[queue_name][routing_key] = {
                 "handle": handle,
                 "content_type": content_type,
+                "response_timeout": response_timeout or self.response_timeout,
             }
```

### Comparing `amqp_client_python-0.1.8/amqp_client_python/rabbitmq/async_connection.py` & `amqp_client_python-0.1.9/amqp_client_python/rabbitmq/async_connection.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,48 +22,52 @@
         self.connection_factory = AsyncConnectionFactoryRabbitMQ()
         self._connection: AsyncioConnection = None
         self._prefetch_count = prefetch_count
         self._auto_ack = auto_ack
         self._channel = AsyncChannel(self._prefetch_count, self._auto_ack)
         self._closing = False
         self._consuming = False
+        self.openning = False
         self.reconnecting = False
         self.reconnect_delay = 1
         self.backup = {
             "exchange": {},
             "queue": {},
             "subscribe": {},
             "rpc_subscribe": {},
         }
 
     def open(self, uri):
         self.url = uri
-        if not self.is_open:
+        if not self.is_open and not self.openning:
             if not self.ioloop:
                 self.ioloop = get_event_loop()
+            self.openning = True
             self._connection = self.connection_factory.create_connection(
                 uri=uri,
                 on_connection_open=self.on_connection_open,
                 on_connection_open_error=self.on_connection_open_error,
                 on_connection_closed=self.on_connection_closed,
                 custum_ioloop=self.ioloop,
             )
 
     async def close(self):
         if self.is_open:
             self._connection.close()
 
     def on_connection_open(self, _unused_connection):
-        LOGGER.debug(f"connection openned {self._channel}")
+        LOGGER.info(f"connection openned {_unused_connection}, {self._connection}")
+        self.openning = False
         self._channel = AsyncChannel(self._prefetch_count, self._auto_ack)
         self._channel.publisher_confirms = self.publisher_confirms
         self._channel.open(self._connection)
 
     def on_connection_open_error(self, _unused_connection, err):
-        LOGGER.warn(f"connection open error: {err}, will attempt a connection")
+        LOGGER.info(f"connection open error: {err}, will attempt a connection")
+        self.openning = False
         self.reconnect()
 
     def on_connection_closed(self, _unused_connection, reason):
         """This method is invoked by pika when the connection to RabbitMQ is
         closed unexpectedly. Since it is unexpected, we will reconnect to
         RabbitMQ if it disconnects.
         :param pika.connection.Connection connection: The closed connection obj
@@ -104,24 +108,22 @@
                 for routing_key in self.backup["subscribe"]:
                     params = self.backup["subscribe"][routing_key]
                     await self.subscribe(
                         params["queue_name"],
                         params["exchange_name"],
                         routing_key,
                         params["callback"],
-                        params["auto_ack"],
                     )
                 for routing_key in self.backup["rpc_subscribe"]:
                     params = self.backup["rpc_subscribe"][routing_key]
                     await self.rpc_subscribe(
                         params["queue_name"],
                         params["exchange_name"],
                         routing_key,
                         params["callback"],
-                        params["auto_ack"],
                     )
 
             self.ioloop.create_task(self.add_callback(recorvery))
             self.reconnect_delay = 1
             self.reconnecting = False
 
     @property
@@ -165,50 +167,60 @@
         self._connection = self.connect()
         self._connection.ioloop.run_forever()
 
     async def rpc_client(
         self, exchange_name: str, routing_key: str, body, content_type, timeout
     ):
         return await self._channel.rpc_client(
-            exchange_name, routing_key, body, content_type, timeout, self.ioloop
+            exchange_name,
+            routing_key,
+            body,
+            content_type,
+            timeout,
         )
 
     async def publish(
         self, exchange_name: str, routing_key: str, body, content_type, timeout
     ):
         return await self._channel.publish(
             exchange_name, routing_key, body, content_type, timeout, loop=self.ioloop
         )
 
-    async def rpc_subscribe(self, queue_name, exchange_name, routing_key, callback):
+    async def rpc_subscribe(
+        self, queue_name, exchange_name, routing_key, callback, response_timeout
+    ):
         self.backup["rpc_subscribe"][routing_key] = {
             "queue_name": queue_name,
             "exchange_name": exchange_name,
-            "routing_key": routing_key,
             "callback": callback,
+            "response_timeout": response_timeout,
         }
         await self._channel.rpc_subscribe(
             queue_name=queue_name,
             exchange_name=exchange_name,
             routing_key=routing_key,
             callback=callback,
+            response_timeout=response_timeout,
         )
 
-    async def subscribe(self, queue_name, exchange_name, routing_key, callback):
+    async def subscribe(
+        self, queue_name, exchange_name, routing_key, callback, response_timeout
+    ):
         self.backup["subscribe"][routing_key] = {
             "queue_name": queue_name,
             "exchange_name": exchange_name,
-            "routing_key": routing_key,
             "callback": callback,
+            "response_timeout": response_timeout,
         }
         await self._channel.subscribe(
             exchange_name=exchange_name,
             queue_name=queue_name,
             routing_key=routing_key,
             callback=callback,
+            response_timeout=response_timeout,
         )
 
     async def add_callback(self, callback, retry=4, delay=1):
         while retry > 0:
             retry -= 1
             if self.is_open and self._channel and self._channel.is_open:
                 return await callback()
```

### Comparing `amqp_client_python-0.1.8/amqp_client_python/rabbitmq/async_connection_factory.py` & `amqp_client_python-0.1.9/amqp_client_python/rabbitmq/async_connection_factory.py`

 * *Files identical despite different names*

### Comparing `amqp_client_python-0.1.8/amqp_client_python/rabbitmq/channel_pool.py` & `amqp_client_python-0.1.9/amqp_client_python/rabbitmq/channel_pool.py`

 * *Files identical despite different names*

### Comparing `amqp_client_python-0.1.8/amqp_client_python/rabbitmq/channel_rabbitmq.py` & `amqp_client_python-0.1.9/amqp_client_python/rabbitmq/channel_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `amqp_client_python-0.1.8/amqp_client_python/rabbitmq/connection_factory_rabbitmq.py` & `amqp_client_python-0.1.9/amqp_client_python/rabbitmq/connection_factory_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `amqp_client_python-0.1.8/amqp_client_python/rabbitmq/connection_rabbitmq.py` & `amqp_client_python-0.1.9/amqp_client_python/rabbitmq/connection_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `amqp_client_python-0.1.8/amqp_client_python/rabbitmq/eventbus_rabbitmq.py` & `amqp_client_python-0.1.9/amqp_client_python/rabbitmq/eventbus_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `amqp_client_python-0.1.8/amqp_client_python/rabbitmq/ioloop_factory.py` & `amqp_client_python-0.1.9/amqp_client_python/rabbitmq/ioloop_factory.py`

 * *Files identical despite different names*

### Comparing `amqp_client_python-0.1.8/pyproject.toml` & `amqp_client_python-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "amqp-client-python"
-version = "0.1.8"
+version = "0.1.9"
 description = "Python AMQP Client Library"
 license = "Apache-2.0"
 authors = ["NUTES UEPB <dev.seniorsaudemovel@gmail.com>"]
 readme = "README.md"
 packages = [{include = "amqp_client_python"}]
 
 [project]
```

### Comparing `amqp_client_python-0.1.8/setup.py` & `amqp_client_python-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pika>=1.3.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'amqp-client-python',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Python AMQP Client Library',
     'long_description': '# AMQP Client Python\n\n[![License][license-image]][license-url]\n<a href="https://pypi.org/project/amqp-client-python" target="_blank">\n    <img src="https://img.shields.io/pypi/v/amqp-client-python?color=%2334D058&label=pypi%20package" alt="Package version">\n</a><a href="https://pypi.org/project/amqp-client-python" target="_blank">\n    <img src="https://img.shields.io/pypi/pyversions/amqp-client-python.svg?color=%2334D058" alt="Supported Python versions">\n</a>\n[![Downloads](https://static.pepy.tech/personalized-badge/amqp-client-python?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/amqp-client-python)\n[![Vulnerabilities][known-vulnerabilities-image]][known-vulnerabilities-url]  [![Releases][releases-image]][releases-url] \n\n\n\n\n--------\nClient with high level of abstraction for manipulation of messages in the event bus RabbitMQ.\n\n### Features:\n- Automatic creation and management of queues, exchanges and channels;\n- Connection persistence and auto reconnect;\n- Support for **direct**, **topic** and **fanout** exchanges;\n- Publish;\n- Subscribe;\n- Support for a Remote procedure call _(RPC)_.\n\n\n[//]: # (These are reference links used in the body of this note.)\n[license-image]: https://img.shields.io/badge/license-Apache%202-blue.svg\n[license-url]: https://github.com/nutes-uepb/amqp-client-python/blob/master/LICENSE\n[npm-image]: https://img.shields.io/npm/v/amqp-client-python.svg?color=red&logo=npm\n[npm-url]: https://npmjs.org/package/amqp-client-python\n[downloads-image]: https://img.shields.io/npm/dt/amqp-client-python.svg?logo=npm\n[travis-url]: https://travis-ci.org/nutes-uepb/amqp-client-python\n[coverage-image]: https://coveralls.io/repos/github/nutes-uepb/amqp-client-python/badge.svg\n[coverage-url]: https://coveralls.io/github/nutes-uepb/amqp-client-python?branch=master\n[known-vulnerabilities-image]: https://snyk.io/test/github/nutes-uepb/amqp-client-python/badge.svg?targetFile=requirements.txt\n[known-vulnerabilities-url]: https://snyk.io/test/github/nutes-uepb/amqp-client-python?targetFile=requirements.txt\n[releases-image]: https://img.shields.io/github/release-date/nutes-uepb/amqp-client-python.svg\n[releases-url]: https://github.com/nutes-uepb/amqp-client-python/releases\n\n### Examples:\n#### you can use [sync](https://github.com/nutes-uepb/amqp-client-python/blob/develop/amqp_client_python/rabbitmq/eventbus_rabbitmq.py) , [async eventbus](https://github.com/nutes-uepb/amqp-client-python/blob/develop/amqp_client_python/rabbitmq/async_eventbus_rabbitmq.py) and [sync wrapper](https://github.com/nutes-uepb/amqp-client-python/blob/develop/amqp_client_python/rabbitmq/eventbus_wrapper_rabbitmq.py) of async eventbus\n<details><summary>async usage </summary>\n\n<br>\n\n```Python\n# basic configuration\nfrom amqp_client_python import (\n    AsyncEventbusRabbitMQ,\n    Config, Options\n)\nfrom amqp_client_python.event import IntegrationEvent, IntegrationEventHandler\nconfig = Config(Options("queue", "rpc_queue", "rpc_exchange"))\neventbus = AsyncEventbusRabbitMQ(config)\n# publish\nclass ExampleEvent(IntegrationEvent):\n    EVENT_NAME: str = "ExampleEvent"\n    def __init__(self, event_type: str, message = []) -> None:\n        super().__init__(self.EVENT_NAME, event_type)\n        self.message = message\n\npublish_event = ExampleEvent(rpc_exchange, ["message"])\neventbus.publish(publish_event, rpc_routing_key, "direct")\n# subscribe\nclass ExampleEventHandler(IntegrationEventHandler):\n    def handle(self, body) -> None:\n        print(body) # handle messages\nawait eventbus.subscribe(subscribe_event, subscribe_event_handle, rpc_routing_key)\n# rpc_publish\nresponse = await eventbus.rpc_client(rpc_exchange, "user.find", ["content_message"])\n# provider\nasync def handle2(*body) -> bytes:\n    print(f"body: {body}")\n    return b"content"\nawait eventbus.provide_resource("user.find", handle)\n```\n</details>\n\n<details><summary>sync usage</summary>\n\n```Python\nfrom amqp_client_python import (\n    EventbusRabbitMQ,\n    Config, Options\n)\nfrom amqp_client_python.event import IntegrationEvent, IntegrationEventHandler\nfrom examples.default import queue, rpc_queue, rpc_exchange, rpc_routing_key\n\n\nclass ExampleEvent(IntegrationEvent):\n    EVENT_NAME: str = "ExampleEvent"\n    ROUTING_KEY: str = rpc_routing_key\n\n    def __init__(self, event_type: str, message = []) -> None:\n        super().__init__(self.EVENT_NAME, event_type)\n        self.message = message\n        self.routing_key = self.ROUTING_KEY\n\n\nclass ExampleEventHandler(IntegrationEventHandler):\n    def handle(self, body) -> None:\n        print(body,"subscribe")\n\n\nconfig = Config(Options(queue, rpc_queue, rpc_exchange))\neventbus = EventbusRabbitMQ(config=config)\n\nclass ExampleEvent(IntegrationEvent):\n    EVENT_NAME: str = "ExampleEvent"\n    def __init__(self, event_type: str, message = []) -> None:\n        super().__init__(self.EVENT_NAME, event_type)\n        self.message = message\n\nfrom time import sleep\nfrom random import randint\ndef handle(*body):\n    print(body[0], "rpc_provider")\n    return f"{body[0]}".encode("utf-8")\n\nsubscribe_event = ExampleEvent(rpc_exchange)\npublish_event = ExampleEvent(rpc_exchange, ["message"])\nsubscribe_event_handle = ExampleEventHandler()\neventbus.subscribe(subscribe_event, subscribe_event_handle, rpc_routing_key)\neventbus.provide_resource(rpc_routing_key+"2", handle)\ncount = 0\nrunning = True\nfrom concurrent.futures import TimeoutError\nwhile running:\n    try:\n        count += 1\n        if str(count) != eventbus.rpc_client(rpc_exchange, rpc_routing_key+"2", [f"{count}"]).decode("utf-8"):\n            running = False\n        #eventbus.publish(publish_event, rpc_routing_key, "direct")\n        #running = False\n    except TimeoutError as err:\n        print("timeout!!!: ", str(err))\n    except KeyboardInterrupt:\n        running=False\n    except BaseException as err:\n        print("Err:", err)\n```\n</details>\n\n<details><summary>sync wrapper usage</summary>\n\n```Python\nfrom amqp_client_python import EventbusWrapperRabbitMQ, Config, Options\nfrom amqp_client_python.event import IntegrationEvent, IntegrationEventHandler\n\nconfig = Config(Options(queue, rpc_queue, rpc_exchange))\neventbus = EventbusWrapperRabbitMQ(config=config)\n\nclass ExampleEvent(IntegrationEvent):\n    EVENT_NAME: str = "ExampleEvent"\n    def __init__(self, event_type: str, message = []) -> None:\n        super().__init__(self.EVENT_NAME, event_type)\n        self.message = message\nclass ExampleEventHandler(IntegrationEventHandler):\n    async def handle(self, body) -> None:\n        print(body,"subscribe")\n\nasync def handle(*body):\n    print(body[0], "rpc_provider")\n    return f"{body[0]}".encode("utf-8")\n\nsubscribe_event = ExampleEvent(rpc_exchange)\npublish_event = ExampleEvent(rpc_exchange, ["message"])\nsubscribe_event_handle = ExampleEventHandler()\n# rpc_provider\neventbus.provide_resource(rpc_routing_key+"2", handle).result()\n# subscribe\neventbus.subscribe(subscribe_event, subscribe_event_handle, rpc_routing_key).result()\ncount = 0\nrunning = True\nwhile running:\n    try:\n        count += 1\n        # rpc_client call\n        eventbus.rpc_client(rpc_exchange, rpc_routing_key+"2", [f"{count}"]).result().decode("utf-8")\n        # publish\n        eventbus.publish(publish_event, rpc_routing_key, "direct").result()\n        #running = False\n    except KeyboardInterrupt:\n        running=False\n    except BaseException as err:\n        print("Err:", err)\n```\n</details>\n<br />\n\n### Know Limitations:\n#### sync eventbus\n```sh\nCannot use rpc call when inside of rpc provider and subscribe handlers\n#/obs: works on sync eventbus wrapper\n```',
     'author': 'NUTES UEPB',
     'author_email': 'dev.seniorsaudemovel@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `amqp_client_python-0.1.8/PKG-INFO` & `amqp_client_python-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amqp-client-python
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python AMQP Client Library
 License: Apache-2.0
 Author: NUTES UEPB
 Author-email: dev.seniorsaudemovel@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

