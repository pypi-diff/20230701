# Comparing `tmp/nonebot_adapter_villa-0.4.1.tar.gz` & `tmp/nonebot_adapter_villa-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_villa-0.4.1.tar", max compression
+gzip compressed data, was "nonebot_adapter_villa-0.4.2.tar", max compression
```

## Comparing `nonebot_adapter_villa-0.4.1.tar` & `nonebot_adapter_villa-0.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1062 2023-06-28 12:39:04.676734 nonebot_adapter_villa-0.4.1/LICENSE
--rw-r--r--   0        0        0     4938 2023-06-28 12:39:04.676734 nonebot_adapter_villa-0.4.1/README.md
--rw-r--r--   0        0        0      235 2023-06-28 12:39:04.676734 nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/__init__.py
--rw-r--r--   0        0        0    10684 2023-06-28 12:39:04.676734 nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/adapter.py
--rw-r--r--   0        0        0      114 2023-06-28 12:39:04.676734 nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/api/__init__.py
--rw-r--r--   0        0        0     2905 2023-06-28 12:39:04.676734 nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/api/cilent.pyi
--rw-r--r--   0        0        0     3714 2023-06-28 12:39:04.676734 nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/api/client.py
--rw-r--r--   0        0        0    12434 2023-06-28 12:39:04.676734 nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/api/handle.py
--rw-r--r--   0        0        0     8899 2023-06-28 12:39:04.676734 nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/api/models.py
--rw-r--r--   0        0        0     1514 2023-06-28 12:39:04.676734 nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/api/request.py
--rw-r--r--   0        0        0    12220 2023-06-28 12:39:04.676734 nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/bot.py
--rw-r--r--   0        0        0      359 2023-06-28 12:39:04.676734 nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/config.py
--rw-r--r--   0        0        0    11641 2023-06-28 12:39:04.676734 nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/event.py
--rw-r--r--   0        0        0     1755 2023-06-28 12:39:04.676734 nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/exception.py
--rw-r--r--   0        0        0     6704 2023-06-28 12:39:04.676734 nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/message.py
--rw-r--r--   0        0        0       76 2023-06-28 12:39:04.676734 nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/utils.py
--rw-r--r--   0        0        0     1134 2023-06-28 12:39:04.676734 nonebot_adapter_villa-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     5839 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4938 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/README.md
+-rw-r--r--   0        0        0      235 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/__init__.py
+-rw-r--r--   0        0        0    10977 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/adapter.py
+-rw-r--r--   0        0        0      114 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/__init__.py
+-rw-r--r--   0        0        0     2905 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/cilent.pyi
+-rw-r--r--   0        0        0     3714 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/client.py
+-rw-r--r--   0        0        0    12434 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/handle.py
+-rw-r--r--   0        0        0     8899 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/models.py
+-rw-r--r--   0        0        0     1514 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/request.py
+-rw-r--r--   0        0        0    12770 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/bot.py
+-rw-r--r--   0        0        0      649 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/config.py
+-rw-r--r--   0        0        0    11641 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/event.py
+-rw-r--r--   0        0        0     1755 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/exception.py
+-rw-r--r--   0        0        0     6704 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/message.py
+-rw-r--r--   0        0        0       76 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/utils.py
+-rw-r--r--   0        0        0     1134 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     5839 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.4.2/PKG-INFO
```

### Comparing `nonebot_adapter_villa-0.4.1/LICENSE` & `nonebot_adapter_villa-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.4.1/README.md` & `nonebot_adapter_villa-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/adapter.py` & `nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,21 +46,24 @@
             isinstance(self.driver, ReverseDriver)
             and isinstance(self.driver, ForwardDriver)
         ):
             raise RuntimeError(
                 f"Current driver {self.config.driver} doesn't support connections!"
                 "Villa Adapter need a ReverseDriver and ForwardDriver to work."
             )
-        self._forward_http()
+        self.driver.on_startup(self._forward_http)
         self.driver.on_startup(self._start_forward)
         self.driver.on_shutdown(self._stop_forward)
 
-    def _forward_http(self):
+    async def _forward_http(self):
         for bot_info in self.villa_config.villa_bots:
             if bot_info.callback_url:
+                bot = Bot(self, bot_info.bot_id, bot_info.bot_secret)
+                self.bot_connect(bot)
+                log("INFO", f"<y>Bot {bot.self_id} connected</y>")
                 http_setup = HTTPServerSetup(
                     URL(bot_info.callback_url),
                     "POST",
                     f"大别野 {bot_info.bot_id} HTTP",
                     self._handle_http,
                 )
                 self.setup_http_server(http_setup)
@@ -79,15 +82,15 @@
                                     bot.bot_secret
                                     for bot in self.villa_config.villa_bots
                                     if bot.bot_id == bot_id
                                 ),
                                 None,
                             )
                         ) is not None:
-                            bot = Bot(self, bot_id, event.robot, bot_secret=bot_secret)
+                            bot = Bot(self, bot_id, bot_secret)
                             self.bot_connect(bot)
                             log("INFO", f"<y>Bot {bot.self_id} connected</y>")
                         else:
                             log(
                                 "WARNING",
                                 f"<r>Missing bot secret for bot {bot_id}</r>, event will not be handle",
                             )
@@ -113,14 +116,17 @@
                 )
             return Response(400, content="Invalid Request Body")
         return Response(400, content="Invalid Request Body")
 
     async def _start_forward(self) -> None:
         for bot_info in self.villa_config.villa_bots:
             if bot_info.ws_url:
+                bot = Bot(self, bot_info.bot_id, bot_info.bot_secret)
+                self.bot_connect(bot)
+                log("INFO", f"<y>Bot {bot.self_id} connected</y>")
                 self.tasks.append(
                     asyncio.create_task(
                         self._forward_ws(URL(bot_info.ws_url), bot_info.ws_secret)
                     )
                 )
 
     async def _forward_ws(self, url: URL, secret: Optional[str] = None):
@@ -156,15 +162,14 @@
                                                 ),
                                                 None,
                                             )
                                         ) is not None:
                                             bot = Bot(
                                                 self,
                                                 bot_id,
-                                                event.robot,
                                                 bot_secret=bot_secret,
                                             )
                                             self.bot_connect(bot)
                                             log(
                                                 "INFO",
                                                 f"<y>Bot {bot.self_id} connected</y>",
                                             )
```

### Comparing `nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/api/cilent.pyi` & `nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/cilent.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/api/client.py` & `nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/api/handle.py` & `nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/api/models.py` & `nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/api/request.py` & `nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/bot.py` & `nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/bot.py`

 * *Files 8% similar despite different names*

```diff
@@ -101,48 +101,56 @@
 
 class Bot(BaseBot, ApiClient):
     """
     大别野协议 Bot 适配。
     """
 
     @overrides(BaseBot)
-    def __init__(
-        self, adapter: Adapter, self_id: str, bot_info: Robot, bot_secret: str
-    ):
+    def __init__(self, adapter: Adapter, self_id: str, bot_secret: str):
         super().__init__(adapter, self_id)
         self.adapter: Adapter = adapter
         self.bot_secret: str = bot_secret
-        self._bot_info: Robot = bot_info
+        self._bot_info: Optional[Robot] = None
 
     @overrides(BaseBot)
     def __repr__(self) -> str:
         return f"Bot(type={self.type!r}, self_id={self.self_id!r})"
 
     @property
     def nickname(self) -> str:
         """Bot 昵称"""
+        if not self._bot_info:
+            raise ValueError(f"Bot {self.self_id} hasn't received any events yet.")
         return self._bot_info.template.name
 
     @property
     def commands(self) -> Optional[List[Command]]:
         """Bot 命令预设命令列表"""
+        if not self._bot_info:
+            raise ValueError(f"Bot {self.self_id} hasn't received any events yet.")
         return self._bot_info.template.commands
 
     @property
     def description(self) -> str:
         """Bot 介绍描述"""
+        if not self._bot_info:
+            raise ValueError(f"Bot {self.self_id} hasn't received any events yet.")
         return self._bot_info.template.desc
 
     @property
     def avatar_icon(self) -> str:
         """Bot 头像图标地址"""
+        if not self._bot_info:
+            raise ValueError(f"Bot {self.self_id} hasn't received any events yet.")
         return self._bot_info.template.icon
 
     @property
     def current_villd_id(self) -> int:
+        if not self._bot_info:
+            raise ValueError(f"Bot {self.self_id} hasn't received any events yet.")
         return self._bot_info.villa_id
 
     async def handle_event(self, event: Event):
         """处理事件"""
         if isinstance(event, SendMessageEvent):
             _check_at_me(self, event)
             # await _check_reply(self, event)
```

### Comparing `nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/event.py` & `nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/exception.py` & `nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.4.1/nonebot/adapters/villa/message.py` & `nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.4.1/pyproject.toml` & `nonebot_adapter_villa-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-villa"
-version = "0.4.1"
+version = "0.4.2"
 description = "NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 repository = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 documentation = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
```

### Comparing `nonebot_adapter_villa-0.4.1/PKG-INFO` & `nonebot_adapter_villa-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-villa
-Version: 0.4.1
+Version: 0.4.2
 Summary: NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa
 License: MIT
 Keywords: nonebot,mihoyo,bot
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.4.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.4.2 Summary:
 NoneBot2ç±³æ¸¸ç¤¾å¤§å«éBotééå¨ãMiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa License: MIT
 Keywords: nonebot,mihoyo,bot Author: CMHopeSunshine Author-email:
 277073121@qq.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

