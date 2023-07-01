# Comparing `tmp/hrbot-0.1.2.tar.gz` & `tmp/hrbot-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrbot-0.1.2.tar", max compression
+gzip compressed data, was "hrbot-0.1.3.tar", max compression
```

## Comparing `hrbot-0.1.2.tar` & `hrbot-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      158 2023-06-15 08:01:29.191231 hrbot-0.1.2/hrbot/__init__.py
--rw-r--r--   0        0        0       31 2023-05-18 14:31:32.146814 hrbot-0.1.2/hrbot/bot/__init__.py
--rw-r--r--   0        0        0      988 2023-06-15 08:48:39.851385 hrbot-0.1.2/hrbot/bot/base.py
--rw-r--r--   0        0        0     3602 2023-06-20 03:58:41.942703 hrbot-0.1.2/hrbot/bot/bot.py
--rw-r--r--   0        0        0       59 2023-05-18 14:31:32.138854 hrbot-0.1.2/hrbot/dispatcher/__init__.py
--rw-r--r--   0        0        0     9474 2023-06-20 03:13:28.257902 hrbot-0.1.2/hrbot/dispatcher/__pycache__/dispatсher.cpython-311.pyc
--rw-r--r--   0        0        0     6343 2023-06-20 03:13:27.988046 hrbot-0.1.2/hrbot/dispatcher/dispatсher.py
--rw-r--r--   0        0        0    10632 2023-06-20 03:12:45.077146 hrbot-0.1.2/hrbot/dispatcher/filter.py
--rw-r--r--   0        0        0       30 2023-05-31 10:19:08.115326 hrbot-0.1.2/hrbot/dispatcher/fsm/__init__.py
--rw-r--r--   0        0        0     1972 2023-06-15 09:02:33.436860 hrbot-0.1.2/hrbot/dispatcher/fsm/state.py
--rw-r--r--   0        0        0     4675 2023-06-14 06:55:24.164338 hrbot-0.1.2/hrbot/dispatcher/fsm/storage.py
--rw-r--r--   0        0        0     1337 2023-06-14 07:07:30.601511 hrbot-0.1.2/hrbot/dispatcher/handler.py
--rw-r--r--   0        0        0      284 2023-06-11 09:43:38.740611 hrbot-0.1.2/hrbot/types/__init__.py
--rw-r--r--   0        0        0      402 2023-06-19 02:47:45.500862 hrbot-0.1.2/hrbot/types/handler.py
--rw-r--r--   0        0        0       31 2023-05-14 15:25:08.437975 hrbot-0.1.2/hrbot/types/hr.py
--rw-r--r--   0        0        0        0 2023-05-14 13:14:36.307325 hrbot-0.1.2/hrbot/utils/__init__.py
--rw-r--r--   0        0        0     1084 2023-06-18 13:15:36.011849 hrbot-0.1.2/LICENSE
--rw-r--r--   0        0        0      459 2023-06-20 03:58:41.907078 hrbot-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1612 2023-06-19 07:04:11.369368 hrbot-0.1.2/README.md
--rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 hrbot-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      158 2023-06-15 08:01:29.191231 hrbot-0.1.3/hrbot/__init__.py
+-rw-r--r--   0        0        0       31 2023-05-18 14:31:32.146814 hrbot-0.1.3/hrbot/bot/__init__.py
+-rw-r--r--   0        0        0      988 2023-06-15 08:48:39.851385 hrbot-0.1.3/hrbot/bot/base.py
+-rw-r--r--   0        0        0     3774 2023-07-01 12:31:29.301795 hrbot-0.1.3/hrbot/bot/bot.py
+-rw-r--r--   0        0        0       59 2023-05-18 14:31:32.138854 hrbot-0.1.3/hrbot/dispatcher/__init__.py
+-rw-r--r--   0        0        0     9653 2023-07-01 12:29:57.935681 hrbot-0.1.3/hrbot/dispatcher/__pycache__/dispatсher.cpython-311.pyc
+-rw-r--r--   0        0        0     6433 2023-07-01 12:29:57.520228 hrbot-0.1.3/hrbot/dispatcher/dispatсher.py
+-rw-r--r--   0        0        0    10692 2023-07-01 12:29:57.528779 hrbot-0.1.3/hrbot/dispatcher/filter.py
+-rw-r--r--   0        0        0       30 2023-05-31 10:19:08.115326 hrbot-0.1.3/hrbot/dispatcher/fsm/__init__.py
+-rw-r--r--   0        0        0     1972 2023-06-15 09:02:33.436860 hrbot-0.1.3/hrbot/dispatcher/fsm/state.py
+-rw-r--r--   0        0        0     4675 2023-06-14 06:55:24.164338 hrbot-0.1.3/hrbot/dispatcher/fsm/storage.py
+-rw-r--r--   0        0        0     1337 2023-06-14 07:07:30.601511 hrbot-0.1.3/hrbot/dispatcher/handler.py
+-rw-r--r--   0        0        0      284 2023-06-11 09:43:38.740611 hrbot-0.1.3/hrbot/types/__init__.py
+-rw-r--r--   0        0        0      402 2023-06-19 02:47:45.500862 hrbot-0.1.3/hrbot/types/handler.py
+-rw-r--r--   0        0        0       31 2023-05-14 15:25:08.437975 hrbot-0.1.3/hrbot/types/hr.py
+-rw-r--r--   0        0        0        0 2023-05-14 13:14:36.307325 hrbot-0.1.3/hrbot/utils/__init__.py
+-rw-r--r--   0        0        0     1084 2023-06-18 13:15:36.011849 hrbot-0.1.3/LICENSE
+-rw-r--r--   0        0        0      459 2023-07-01 05:33:00.474819 hrbot-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1612 2023-07-01 05:33:00.485987 hrbot-0.1.3/README.md
+-rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 hrbot-0.1.3/PKG-INFO
```

### Comparing `hrbot-0.1.2/hrbot/bot/base.py` & `hrbot-0.1.3/hrbot/bot/base.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.2/hrbot/bot/bot.py` & `hrbot-0.1.3/hrbot/bot/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from .base import BaseBot
 from ..types import _bcolors
 from ..types.hr import SessionMetadata, User, Position, AnchorPosition, Reaction, CurrencyItem, Item
 from typing import Literal
+from quattro import TaskGroup
 
 class Bot(BaseBot):
     @staticmethod
     def __event_handler(func):
         async def wrapper(self, *args, **kwargs):
             event_name = func.__name__
             await func(self, *args, **kwargs)
             await self.dp._process_event(event_name, *args, **kwargs)
 
         return wrapper
 
     @__event_handler
+    async def before_start(self, tg: TaskGroup) -> None:
+        """Called before the bot starts."""
+        pass
+
+    @__event_handler
     async def on_start(self, session_metadata: SessionMetadata) -> None:
         """On a connection to the room being established.
 
         This may be called multiple times, since the connection may be dropped
         and reestablished.
         """
         self.id = session_metadata.user_id
```

### Comparing `hrbot-0.1.2/hrbot/dispatcher/__pycache__/dispatсher.cpython-311.pyc` & `hrbot-0.1.3/hrbot/dispatcher/__pycache__/dispatсher.cpython-311.pyc`

 * *Files 18% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x57199164 (Tue Jun 20 03:13:27 2023 UTC)
-files sz: 6343
+moddate:  0x451ca064 (Sat Jul  1 12:29:57 2023 UTC)
+files sz: 6433
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640264036c026d035a036d
@@ -65,17 +65,17 @@
                 86 LOAD_CONST               8 (<code object DispatcherEvents, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 10>)
                 88 MAKE_FUNCTION            0
                 90 LOAD_CONST               9 ('DispatcherEvents')
                 92 PRECALL                  2
                 96 CALL                     2
                106 STORE_NAME              13 (DispatcherEvents)
    
-   155         108 PUSH_NULL
+   159         108 PUSH_NULL
                110 LOAD_BUILD_CLASS
-               112 LOAD_CONST              10 (<code object Dispatcher, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 155>)
+               112 LOAD_CONST              10 (<code object Dispatcher, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 159>)
                114 MAKE_FUNCTION            0
                116 LOAD_CONST              11 ('Dispatcher')
                118 LOAD_NAME               13 (DispatcherEvents)
                120 PRECALL                  3
                124 CALL                     3
                134 STORE_NAME              14 (Dispatcher)
                136 LOAD_CONST               1 (None)
@@ -91,568 +91,593 @@
       ('Optional', 'Literal')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 18
          flags     : 0
          code
-            0x970065005a0164005a02640184005a03640264026402640365046a0500
-            0000000000000064026402640464059c08640665046a0600000000000000
-            00640765046a070000000000000000640865046a07000000000000000064
-            096508650919000000000000000000640a6508650a190000000000000000
-            00640b6508650919000000000000000000640c6508650919000000000000
-            000000640d6508650a190000000000000000006610640e84065a0b640264
-            026402640365046a05000000000000000064026402640464059c08640665
-            046a060000000000000000640765046a070000000000000000640865046a
-            07000000000000000064096508650919000000000000000000640a650865
-            0a19000000000000000000640b6508650919000000000000000000640c65
-            08650919000000000000000000640d6508650a1900000000000000000066
-            10640f84065a0c6402640264026402640464109c05640665046a06000000
-            0000000000641165046a070000000000000000641265046a060000000000
-            000000640c6508650919000000000000000000640d6508650a1900000000
-            0000000000660a641384065a0d6402640264026402640464149c05640665
-            046a060000000000000000641565046a0e0000000000000000641265046a
-            060000000000000000640c6508650919000000000000000000640d650865
-            0a19000000000000000000660a641684065a0f64026402640464179c0364
-            0665046a060000000000000000640c650865091900000000000000000064
-            0d6508650a190000000000000000006606641884065a1064026402640464
-            179c03640665046a060000000000000000640c6508650919000000000000
-            000000640d6508650a190000000000000000006606641984065a11640264
-            02640264026404641a9c05641b65046a060000000000000000641265046a
-            060000000000000000641c65046a120000000000000000640c6508650919
-            000000000000000000640d6508650a19000000000000000000660a641d84
-            065a136402640264026404641e9c04641f65086509190000000000000000
-            00640765046a070000000000000000642065086514650919000000000000
-            00000019000000000000000000640d6508650a1900000000000000000066
-            08642184065a15640264026402640464229c04640665046a060000000000
-            000000642365046a160000000000000000640c6508650919000000000000
-            000000640d6508650a190000000000000000006608642484065a17640264
-            02640464259c0364266518651965046a060000000000000000651a642719
-            000000000000000000660219000000000000000000190000000000000000
-            006428651b640d6508650a190000000000000000006606642984065a1c64
-            026402640264026404642a9c05642b6509642c6509642d650a640c650865
-            0919000000000000000000640d6508650a19000000000000000000660a64
-            2e84065a1d64025300
+            0x970065005a0164005a02640184005a03640284005a0464036403640364
+            0465056a06000000000000000064036403640564069c08640765056a0700
+            00000000000000640865056a080000000000000000640965056a08000000
+            0000000000640a6509650a19000000000000000000640b6509650b190000
+            00000000000000640c6509650a19000000000000000000640d6509650a19
+            000000000000000000640e6509650b190000000000000000006610640f84
+            065a0c640364036403640465056a06000000000000000064036403640564
+            069c08640765056a070000000000000000640865056a0800000000000000
+            00640965056a080000000000000000640a6509650a190000000000000000
+            00640b6509650b19000000000000000000640c6509650a19000000000000
+            000000640d6509650a19000000000000000000640e6509650b1900000000
+            00000000006610641084065a0d6403640364036403640564119c05640765
+            056a070000000000000000641265056a080000000000000000641365056a
+            070000000000000000640d6509650a19000000000000000000640e650965
+            0b19000000000000000000660a641484065a0e6403640364036403640564
+            159c05640765056a070000000000000000641665056a0f00000000000000
+            00641365056a070000000000000000640d6509650a190000000000000000
+            00640e6509650b19000000000000000000660a641784065a106403640364
+            0564189c03640765056a070000000000000000640d6509650a1900000000
+            0000000000640e6509650b190000000000000000006606641984065a1164
+            036403640564189c03640765056a070000000000000000640d6509650a19
+            000000000000000000640e6509650b190000000000000000006606641a84
+            065a1264036403640364036405641b9c05641c65056a0700000000000000
+            00641365056a070000000000000000641d65056a13000000000000000064
+            0d6509650a19000000000000000000640e6509650b190000000000000000
+            00660a641e84065a146403640364036405641f9c0464206509650a190000
+            00000000000000640865056a080000000000000000642165096515650a19
+            00000000000000000019000000000000000000640e6509650b1900000000
+            00000000006608642284065a16640364036403640564239c04640765056a
+            070000000000000000642465056a170000000000000000640d6509650a19
+            000000000000000000640e6509650b190000000000000000006608642584
+            065a1864036403640564269c0364276519651a65056a0700000000000000
+            00651b642819000000000000000000660219000000000000000000190000
+            000000000000006429651c640e6509650b19000000000000000000660664
+            2a84065a1d64036403640364036405642b9c05642c650a642d650a642e65
+            0b640d6509650a19000000000000000000640e6509650b19000000000000
+            000000660a642f84065a1e64035300
           10           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('DispatcherEvents')
                        8 STORE_NAME               2 (__qualname__)
          
-          11          10 LOAD_CONST               1 (<code object on_start, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 11>)
+          11          10 LOAD_CONST               1 (<code object before_start, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 11>)
                       12 MAKE_FUNCTION            0
-                      14 STORE_NAME               3 (on_start)
+                      14 STORE_NAME               3 (before_start)
          
-          22          16 LOAD_CONST               2 (None)
+          15          16 LOAD_CONST               2 (<code object on_start, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 15>)
+                      18 MAKE_FUNCTION            0
+                      20 STORE_NAME               4 (on_start)
          
-          23          18 LOAD_CONST               2 (None)
+          26          22 LOAD_CONST               3 (None)
          
-          24          20 LOAD_CONST               2 (None)
+          27          24 LOAD_CONST               3 (None)
          
-          25          22 LOAD_CONST               3 ('/.!$#')
+          28          26 LOAD_CONST               3 (None)
          
-          26          24 LOAD_NAME                4 (handler)
-                      26 LOAD_ATTR                5 (CaseIgnoreDefaultValue)
+          29          28 LOAD_CONST               4 ('/.!$#')
          
-          27          36 LOAD_CONST               2 (None)
+          30          30 LOAD_NAME                5 (handler)
+                      32 LOAD_ATTR                6 (CaseIgnoreDefaultValue)
          
-          28          38 LOAD_CONST               2 (None)
+          31          42 LOAD_CONST               3 (None)
          
-          29          40 LOAD_CONST               4 (False)
+          32          44 LOAD_CONST               3 (None)
          
-          19          42 LOAD_CONST               5 (('user', 'message', 'command', 'prefix', 'case_ignore', 'regex', 'state', 'go_on'))
-                      44 BUILD_CONST_KEY_MAP      8
-                      46 LOAD_CONST               6 ('user')
+          33          46 LOAD_CONST               5 (False)
          
-          22          48 LOAD_NAME                4 (handler)
-                      50 LOAD_ATTR                6 (User)
+          23          48 LOAD_CONST               6 (('user', 'message', 'command', 'prefix', 'case_ignore', 'regex', 'state', 'go_on'))
+                      50 BUILD_CONST_KEY_MAP      8
+                      52 LOAD_CONST               7 ('user')
          
-          19          60 LOAD_CONST               7 ('message')
+          26          54 LOAD_NAME                5 (handler)
+                      56 LOAD_ATTR                7 (User)
          
-          23          62 LOAD_NAME                4 (handler)
-                      64 LOAD_ATTR                7 (Message)
+          23          66 LOAD_CONST               8 ('message')
          
-          19          74 LOAD_CONST               8 ('command')
+          27          68 LOAD_NAME                5 (handler)
+                      70 LOAD_ATTR                8 (Message)
          
-          24          76 LOAD_NAME                4 (handler)
-                      78 LOAD_ATTR                7 (Message)
+          23          80 LOAD_CONST               9 ('command')
          
-          19          88 LOAD_CONST               9 ('prefix')
+          28          82 LOAD_NAME                5 (handler)
+                      84 LOAD_ATTR                8 (Message)
          
-          25          90 LOAD_NAME                8 (Optional)
-                      92 LOAD_NAME                9 (str)
-                      94 BINARY_SUBSCR
+          23          94 LOAD_CONST              10 ('prefix')
          
-          19         104 LOAD_CONST              10 ('case_ignore')
+          29          96 LOAD_NAME                9 (Optional)
+                      98 LOAD_NAME               10 (str)
+                     100 BINARY_SUBSCR
          
-          26         106 LOAD_NAME                8 (Optional)
-                     108 LOAD_NAME               10 (bool)
-                     110 BINARY_SUBSCR
+          23         110 LOAD_CONST              11 ('case_ignore')
          
-          19         120 LOAD_CONST              11 ('regex')
+          30         112 LOAD_NAME                9 (Optional)
+                     114 LOAD_NAME               11 (bool)
+                     116 BINARY_SUBSCR
          
-          27         122 LOAD_NAME                8 (Optional)
-                     124 LOAD_NAME                9 (str)
-                     126 BINARY_SUBSCR
+          23         126 LOAD_CONST              12 ('regex')
          
-          19         136 LOAD_CONST              12 ('state')
+          31         128 LOAD_NAME                9 (Optional)
+                     130 LOAD_NAME               10 (str)
+                     132 BINARY_SUBSCR
          
-          28         138 LOAD_NAME                8 (Optional)
-                     140 LOAD_NAME                9 (str)
-                     142 BINARY_SUBSCR
+          23         142 LOAD_CONST              13 ('state')
          
-          19         152 LOAD_CONST              13 ('go_on')
+          32         144 LOAD_NAME                9 (Optional)
+                     146 LOAD_NAME               10 (str)
+                     148 BINARY_SUBSCR
          
-          29         154 LOAD_NAME                8 (Optional)
-                     156 LOAD_NAME               10 (bool)
-                     158 BINARY_SUBSCR
+          23         158 LOAD_CONST              14 ('go_on')
          
-          19         168 BUILD_TUPLE             16
-                     170 LOAD_CONST              14 (<code object on_chat, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 19>)
-                     172 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     174 STORE_NAME              11 (on_chat)
+          33         160 LOAD_NAME                9 (Optional)
+                     162 LOAD_NAME               11 (bool)
+                     164 BINARY_SUBSCR
          
-          38         176 LOAD_CONST               2 (None)
+          23         174 BUILD_TUPLE             16
+                     176 LOAD_CONST              15 (<code object on_chat, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 23>)
+                     178 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     180 STORE_NAME              12 (on_chat)
          
-          39         178 LOAD_CONST               2 (None)
+          42         182 LOAD_CONST               3 (None)
          
-          40         180 LOAD_CONST               2 (None)
+          43         184 LOAD_CONST               3 (None)
          
-          41         182 LOAD_CONST               3 ('/.!$#')
+          44         186 LOAD_CONST               3 (None)
          
-          42         184 LOAD_NAME                4 (handler)
-                     186 LOAD_ATTR                5 (CaseIgnoreDefaultValue)
+          45         188 LOAD_CONST               4 ('/.!$#')
          
-          43         196 LOAD_CONST               2 (None)
+          46         190 LOAD_NAME                5 (handler)
+                     192 LOAD_ATTR                6 (CaseIgnoreDefaultValue)
          
-          44         198 LOAD_CONST               2 (None)
+          47         202 LOAD_CONST               3 (None)
          
-          45         200 LOAD_CONST               4 (False)
+          48         204 LOAD_CONST               3 (None)
          
-          35         202 LOAD_CONST               5 (('user', 'message', 'command', 'prefix', 'case_ignore', 'regex', 'state', 'go_on'))
-                     204 BUILD_CONST_KEY_MAP      8
-                     206 LOAD_CONST               6 ('user')
+          49         206 LOAD_CONST               5 (False)
          
-          38         208 LOAD_NAME                4 (handler)
-                     210 LOAD_ATTR                6 (User)
+          39         208 LOAD_CONST               6 (('user', 'message', 'command', 'prefix', 'case_ignore', 'regex', 'state', 'go_on'))
+                     210 BUILD_CONST_KEY_MAP      8
+                     212 LOAD_CONST               7 ('user')
          
-          35         220 LOAD_CONST               7 ('message')
+          42         214 LOAD_NAME                5 (handler)
+                     216 LOAD_ATTR                7 (User)
          
-          39         222 LOAD_NAME                4 (handler)
-                     224 LOAD_ATTR                7 (Message)
+          39         226 LOAD_CONST               8 ('message')
          
-          35         234 LOAD_CONST               8 ('command')
+          43         228 LOAD_NAME                5 (handler)
+                     230 LOAD_ATTR                8 (Message)
          
-          40         236 LOAD_NAME                4 (handler)
-                     238 LOAD_ATTR                7 (Message)
+          39         240 LOAD_CONST               9 ('command')
          
-          35         248 LOAD_CONST               9 ('prefix')
+          44         242 LOAD_NAME                5 (handler)
+                     244 LOAD_ATTR                8 (Message)
          
-          41         250 LOAD_NAME                8 (Optional)
-                     252 LOAD_NAME                9 (str)
-                     254 BINARY_SUBSCR
+          39         254 LOAD_CONST              10 ('prefix')
          
-          35         264 LOAD_CONST              10 ('case_ignore')
+          45         256 LOAD_NAME                9 (Optional)
+                     258 LOAD_NAME               10 (str)
+                     260 BINARY_SUBSCR
          
-          42         266 LOAD_NAME                8 (Optional)
-                     268 LOAD_NAME               10 (bool)
-                     270 BINARY_SUBSCR
+          39         270 LOAD_CONST              11 ('case_ignore')
          
-          35         280 LOAD_CONST              11 ('regex')
+          46         272 LOAD_NAME                9 (Optional)
+                     274 LOAD_NAME               11 (bool)
+                     276 BINARY_SUBSCR
          
-          43         282 LOAD_NAME                8 (Optional)
-                     284 LOAD_NAME                9 (str)
-                     286 BINARY_SUBSCR
+          39         286 LOAD_CONST              12 ('regex')
          
-          35         296 LOAD_CONST              12 ('state')
+          47         288 LOAD_NAME                9 (Optional)
+                     290 LOAD_NAME               10 (str)
+                     292 BINARY_SUBSCR
          
-          44         298 LOAD_NAME                8 (Optional)
-                     300 LOAD_NAME                9 (str)
-                     302 BINARY_SUBSCR
+          39         302 LOAD_CONST              13 ('state')
          
-          35         312 LOAD_CONST              13 ('go_on')
+          48         304 LOAD_NAME                9 (Optional)
+                     306 LOAD_NAME               10 (str)
+                     308 BINARY_SUBSCR
          
-          45         314 LOAD_NAME                8 (Optional)
-                     316 LOAD_NAME               10 (bool)
-                     318 BINARY_SUBSCR
+          39         318 LOAD_CONST              14 ('go_on')
          
-          35         328 BUILD_TUPLE             16
-                     330 LOAD_CONST              15 (<code object on_whisper, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 35>)
-                     332 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     334 STORE_NAME              12 (on_whisper)
+          49         320 LOAD_NAME                9 (Optional)
+                     322 LOAD_NAME               11 (bool)
+                     324 BINARY_SUBSCR
          
-          54         336 LOAD_CONST               2 (None)
+          39         334 BUILD_TUPLE             16
+                     336 LOAD_CONST              16 (<code object on_whisper, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 39>)
+                     338 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     340 STORE_NAME              13 (on_whisper)
          
-          55         338 LOAD_CONST               2 (None)
+          58         342 LOAD_CONST               3 (None)
          
-          56         340 LOAD_CONST               2 (None)
+          59         344 LOAD_CONST               3 (None)
          
-          57         342 LOAD_CONST               2 (None)
+          60         346 LOAD_CONST               3 (None)
          
-          58         344 LOAD_CONST               4 (False)
+          61         348 LOAD_CONST               3 (None)
          
-          51         346 LOAD_CONST              16 (('user', 'emote_id', 'receiver', 'state', 'go_on'))
-                     348 BUILD_CONST_KEY_MAP      5
-                     350 LOAD_CONST               6 ('user')
+          62         350 LOAD_CONST               5 (False)
          
-          54         352 LOAD_NAME                4 (handler)
-                     354 LOAD_ATTR                6 (User)
+          55         352 LOAD_CONST              17 (('user', 'emote_id', 'receiver', 'state', 'go_on'))
+                     354 BUILD_CONST_KEY_MAP      5
+                     356 LOAD_CONST               7 ('user')
          
-          51         364 LOAD_CONST              17 ('emote_id')
+          58         358 LOAD_NAME                5 (handler)
+                     360 LOAD_ATTR                7 (User)
          
-          55         366 LOAD_NAME                4 (handler)
-                     368 LOAD_ATTR                7 (Message)
+          55         370 LOAD_CONST              18 ('emote_id')
          
-          51         378 LOAD_CONST              18 ('receiver')
+          59         372 LOAD_NAME                5 (handler)
+                     374 LOAD_ATTR                8 (Message)
          
-          56         380 LOAD_NAME                4 (handler)
-                     382 LOAD_ATTR                6 (User)
+          55         384 LOAD_CONST              19 ('receiver')
          
-          51         392 LOAD_CONST              12 ('state')
+          60         386 LOAD_NAME                5 (handler)
+                     388 LOAD_ATTR                7 (User)
          
-          57         394 LOAD_NAME                8 (Optional)
-                     396 LOAD_NAME                9 (str)
-                     398 BINARY_SUBSCR
+          55         398 LOAD_CONST              13 ('state')
          
-          51         408 LOAD_CONST              13 ('go_on')
+          61         400 LOAD_NAME                9 (Optional)
+                     402 LOAD_NAME               10 (str)
+                     404 BINARY_SUBSCR
          
-          58         410 LOAD_NAME                8 (Optional)
-                     412 LOAD_NAME               10 (bool)
-                     414 BINARY_SUBSCR
+          55         414 LOAD_CONST              14 ('go_on')
          
-          51         424 BUILD_TUPLE             10
-                     426 LOAD_CONST              19 (<code object on_emote, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 51>)
-                     428 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     430 STORE_NAME              13 (on_emote)
+          62         416 LOAD_NAME                9 (Optional)
+                     418 LOAD_NAME               11 (bool)
+                     420 BINARY_SUBSCR
          
-          66         432 LOAD_CONST               2 (None)
+          55         430 BUILD_TUPLE             10
+                     432 LOAD_CONST              20 (<code object on_emote, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 55>)
+                     434 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     436 STORE_NAME              14 (on_emote)
          
-          67         434 LOAD_CONST               2 (None)
+          70         438 LOAD_CONST               3 (None)
          
-          68         436 LOAD_CONST               2 (None)
+          71         440 LOAD_CONST               3 (None)
          
-          69         438 LOAD_CONST               2 (None)
+          72         442 LOAD_CONST               3 (None)
          
-          70         440 LOAD_CONST               4 (False)
+          73         444 LOAD_CONST               3 (None)
          
-          64         442 LOAD_CONST              20 (('user', 'reaction', 'receiver', 'state', 'go_on'))
-                     444 BUILD_CONST_KEY_MAP      5
-                     446 LOAD_CONST               6 ('user')
+          74         446 LOAD_CONST               5 (False)
          
-          66         448 LOAD_NAME                4 (handler)
-                     450 LOAD_ATTR                6 (User)
+          68         448 LOAD_CONST              21 (('user', 'reaction', 'receiver', 'state', 'go_on'))
+                     450 BUILD_CONST_KEY_MAP      5
+                     452 LOAD_CONST               7 ('user')
          
-          64         460 LOAD_CONST              21 ('reaction')
+          70         454 LOAD_NAME                5 (handler)
+                     456 LOAD_ATTR                7 (User)
          
-          67         462 LOAD_NAME                4 (handler)
-                     464 LOAD_ATTR               14 (Reaction)
+          68         466 LOAD_CONST              22 ('reaction')
          
-          64         474 LOAD_CONST              18 ('receiver')
+          71         468 LOAD_NAME                5 (handler)
+                     470 LOAD_ATTR               15 (Reaction)
          
-          68         476 LOAD_NAME                4 (handler)
-                     478 LOAD_ATTR                6 (User)
+          68         480 LOAD_CONST              19 ('receiver')
          
-          64         488 LOAD_CONST              12 ('state')
+          72         482 LOAD_NAME                5 (handler)
+                     484 LOAD_ATTR                7 (User)
          
-          69         490 LOAD_NAME                8 (Optional)
-                     492 LOAD_NAME                9 (str)
-                     494 BINARY_SUBSCR
+          68         494 LOAD_CONST              13 ('state')
          
-          64         504 LOAD_CONST              13 ('go_on')
+          73         496 LOAD_NAME                9 (Optional)
+                     498 LOAD_NAME               10 (str)
+                     500 BINARY_SUBSCR
          
-          70         506 LOAD_NAME                8 (Optional)
-                     508 LOAD_NAME               10 (bool)
-                     510 BINARY_SUBSCR
+          68         510 LOAD_CONST              14 ('go_on')
          
-          64         520 BUILD_TUPLE             10
-                     522 LOAD_CONST              22 (<code object on_reaction, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 64>)
-                     524 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     526 STORE_NAME              15 (on_reaction)
+          74         512 LOAD_NAME                9 (Optional)
+                     514 LOAD_NAME               11 (bool)
+                     516 BINARY_SUBSCR
          
-          79         528 LOAD_CONST               2 (None)
+          68         526 BUILD_TUPLE             10
+                     528 LOAD_CONST              23 (<code object on_reaction, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 68>)
+                     530 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     532 STORE_NAME              16 (on_reaction)
          
-          80         530 LOAD_CONST               2 (None)
+          83         534 LOAD_CONST               3 (None)
          
-          81         532 LOAD_CONST               4 (False)
+          84         536 LOAD_CONST               3 (None)
          
-          76         534 LOAD_CONST              23 (('user', 'state', 'go_on'))
-                     536 BUILD_CONST_KEY_MAP      3
-                     538 LOAD_CONST               6 ('user')
+          85         538 LOAD_CONST               5 (False)
          
-          79         540 LOAD_NAME                4 (handler)
-                     542 LOAD_ATTR                6 (User)
+          80         540 LOAD_CONST              24 (('user', 'state', 'go_on'))
+                     542 BUILD_CONST_KEY_MAP      3
+                     544 LOAD_CONST               7 ('user')
          
-          76         552 LOAD_CONST              12 ('state')
+          83         546 LOAD_NAME                5 (handler)
+                     548 LOAD_ATTR                7 (User)
          
-          80         554 LOAD_NAME                8 (Optional)
-                     556 LOAD_NAME                9 (str)
-                     558 BINARY_SUBSCR
+          80         558 LOAD_CONST              13 ('state')
          
-          76         568 LOAD_CONST              13 ('go_on')
+          84         560 LOAD_NAME                9 (Optional)
+                     562 LOAD_NAME               10 (str)
+                     564 BINARY_SUBSCR
          
-          81         570 LOAD_NAME                8 (Optional)
-                     572 LOAD_NAME               10 (bool)
-                     574 BINARY_SUBSCR
+          80         574 LOAD_CONST              14 ('go_on')
          
-          76         584 BUILD_TUPLE              6
-                     586 LOAD_CONST              24 (<code object on_user_join, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 76>)
-                     588 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     590 STORE_NAME              16 (on_user_join)
+          85         576 LOAD_NAME                9 (Optional)
+                     578 LOAD_NAME               11 (bool)
+                     580 BINARY_SUBSCR
          
-          90         592 LOAD_CONST               2 (None)
+          80         590 BUILD_TUPLE              6
+                     592 LOAD_CONST              25 (<code object on_user_join, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 80>)
+                     594 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     596 STORE_NAME              17 (on_user_join)
          
-          91         594 LOAD_CONST               2 (None)
+          94         598 LOAD_CONST               3 (None)
          
-          92         596 LOAD_CONST               4 (False)
+          95         600 LOAD_CONST               3 (None)
          
-          87         598 LOAD_CONST              23 (('user', 'state', 'go_on'))
-                     600 BUILD_CONST_KEY_MAP      3
-                     602 LOAD_CONST               6 ('user')
+          96         602 LOAD_CONST               5 (False)
          
-          90         604 LOAD_NAME                4 (handler)
-                     606 LOAD_ATTR                6 (User)
+          91         604 LOAD_CONST              24 (('user', 'state', 'go_on'))
+                     606 BUILD_CONST_KEY_MAP      3
+                     608 LOAD_CONST               7 ('user')
          
-          87         616 LOAD_CONST              12 ('state')
+          94         610 LOAD_NAME                5 (handler)
+                     612 LOAD_ATTR                7 (User)
          
-          91         618 LOAD_NAME                8 (Optional)
-                     620 LOAD_NAME                9 (str)
-                     622 BINARY_SUBSCR
+          91         622 LOAD_CONST              13 ('state')
          
-          87         632 LOAD_CONST              13 ('go_on')
+          95         624 LOAD_NAME                9 (Optional)
+                     626 LOAD_NAME               10 (str)
+                     628 BINARY_SUBSCR
          
-          92         634 LOAD_NAME                8 (Optional)
-                     636 LOAD_NAME               10 (bool)
-                     638 BINARY_SUBSCR
+          91         638 LOAD_CONST              14 ('go_on')
          
-          87         648 BUILD_TUPLE              6
-                     650 LOAD_CONST              25 (<code object on_user_leave, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 87>)
-                     652 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     654 STORE_NAME              17 (on_user_leave)
+          96         640 LOAD_NAME                9 (Optional)
+                     642 LOAD_NAME               11 (bool)
+                     644 BINARY_SUBSCR
          
-         100         656 LOAD_CONST               2 (None)
+          91         654 BUILD_TUPLE              6
+                     656 LOAD_CONST              26 (<code object on_user_leave, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 91>)
+                     658 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     660 STORE_NAME              18 (on_user_leave)
          
-         101         658 LOAD_CONST               2 (None)
+         104         662 LOAD_CONST               3 (None)
          
-         102         660 LOAD_CONST               2 (None)
+         105         664 LOAD_CONST               3 (None)
          
-         103         662 LOAD_CONST               2 (None)
+         106         666 LOAD_CONST               3 (None)
          
-         104         664 LOAD_CONST               4 (False)
+         107         668 LOAD_CONST               3 (None)
          
-          98         666 LOAD_CONST              26 (('sender', 'receiver', 'tip', 'state', 'go_on'))
-                     668 BUILD_CONST_KEY_MAP      5
-                     670 LOAD_CONST              27 ('sender')
+         108         670 LOAD_CONST               5 (False)
          
-         100         672 LOAD_NAME                4 (handler)
-                     674 LOAD_ATTR                6 (User)
+         102         672 LOAD_CONST              27 (('sender', 'receiver', 'tip', 'state', 'go_on'))
+                     674 BUILD_CONST_KEY_MAP      5
+                     676 LOAD_CONST              28 ('sender')
          
-          98         684 LOAD_CONST              18 ('receiver')
+         104         678 LOAD_NAME                5 (handler)
+                     680 LOAD_ATTR                7 (User)
          
-         101         686 LOAD_NAME                4 (handler)
-                     688 LOAD_ATTR                6 (User)
+         102         690 LOAD_CONST              19 ('receiver')
          
-          98         698 LOAD_CONST              28 ('tip')
+         105         692 LOAD_NAME                5 (handler)
+                     694 LOAD_ATTR                7 (User)
          
-         102         700 LOAD_NAME                4 (handler)
-                     702 LOAD_ATTR               18 (Tip)
+         102         704 LOAD_CONST              29 ('tip')
          
-          98         712 LOAD_CONST              12 ('state')
+         106         706 LOAD_NAME                5 (handler)
+                     708 LOAD_ATTR               19 (Tip)
          
-         103         714 LOAD_NAME                8 (Optional)
-                     716 LOAD_NAME                9 (str)
-                     718 BINARY_SUBSCR
+         102         718 LOAD_CONST              13 ('state')
          
-          98         728 LOAD_CONST              13 ('go_on')
+         107         720 LOAD_NAME                9 (Optional)
+                     722 LOAD_NAME               10 (str)
+                     724 BINARY_SUBSCR
          
-         104         730 LOAD_NAME                8 (Optional)
-                     732 LOAD_NAME               10 (bool)
-                     734 BINARY_SUBSCR
+         102         734 LOAD_CONST              14 ('go_on')
          
-          98         744 BUILD_TUPLE             10
-                     746 LOAD_CONST              29 (<code object on_tip, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 98>)
-                     748 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     750 STORE_NAME              19 (on_tip)
+         108         736 LOAD_NAME                9 (Optional)
+                     738 LOAD_NAME               11 (bool)
+                     740 BINARY_SUBSCR
          
-         112         752 LOAD_CONST               2 (None)
+         102         750 BUILD_TUPLE             10
+                     752 LOAD_CONST              30 (<code object on_tip, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 102>)
+                     754 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     756 STORE_NAME              20 (on_tip)
          
-         113         754 LOAD_CONST               2 (None)
+         116         758 LOAD_CONST               3 (None)
          
-         114         756 LOAD_CONST               2 (None)
+         117         760 LOAD_CONST               3 (None)
          
-         115         758 LOAD_CONST               4 (False)
+         118         762 LOAD_CONST               3 (None)
          
-         110         760 LOAD_CONST              30 (('sender_id', 'message', 'tags', 'go_on'))
-                     762 BUILD_CONST_KEY_MAP      4
-                     764 LOAD_CONST              31 ('sender_id')
+         119         764 LOAD_CONST               5 (False)
          
-         112         766 LOAD_NAME                8 (Optional)
-                     768 LOAD_NAME                9 (str)
-                     770 BINARY_SUBSCR
+         114         766 LOAD_CONST              31 (('sender_id', 'message', 'tags', 'go_on'))
+                     768 BUILD_CONST_KEY_MAP      4
+                     770 LOAD_CONST              32 ('sender_id')
          
-         110         780 LOAD_CONST               7 ('message')
+         116         772 LOAD_NAME                9 (Optional)
+                     774 LOAD_NAME               10 (str)
+                     776 BINARY_SUBSCR
          
-         113         782 LOAD_NAME                4 (handler)
-                     784 LOAD_ATTR                7 (Message)
+         114         786 LOAD_CONST               8 ('message')
          
-         110         794 LOAD_CONST              32 ('tags')
+         117         788 LOAD_NAME                5 (handler)
+                     790 LOAD_ATTR                8 (Message)
          
-         114         796 LOAD_NAME                8 (Optional)
-                     798 LOAD_NAME               20 (set)
-                     800 LOAD_NAME                9 (str)
-                     802 BINARY_SUBSCR
-                     812 BINARY_SUBSCR
+         114         800 LOAD_CONST              33 ('tags')
          
-         110         822 LOAD_CONST              13 ('go_on')
+         118         802 LOAD_NAME                9 (Optional)
+                     804 LOAD_NAME               21 (set)
+                     806 LOAD_NAME               10 (str)
+                     808 BINARY_SUBSCR
+                     818 BINARY_SUBSCR
          
-         115         824 LOAD_NAME                8 (Optional)
-                     826 LOAD_NAME               10 (bool)
-                     828 BINARY_SUBSCR
+         114         828 LOAD_CONST              14 ('go_on')
          
-         110         838 BUILD_TUPLE              8
-                     840 LOAD_CONST              33 (<code object on_channel, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 110>)
-                     842 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     844 STORE_NAME              21 (on_channel)
+         119         830 LOAD_NAME                9 (Optional)
+                     832 LOAD_NAME               11 (bool)
+                     834 BINARY_SUBSCR
          
-         123         846 LOAD_CONST               2 (None)
+         114         844 BUILD_TUPLE              8
+                     846 LOAD_CONST              34 (<code object on_channel, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 114>)
+                     848 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     850 STORE_NAME              22 (on_channel)
          
-         124         848 LOAD_CONST               2 (None)
+         127         852 LOAD_CONST               3 (None)
          
-         125         850 LOAD_CONST               2 (None)
+         128         854 LOAD_CONST               3 (None)
          
-         126         852 LOAD_CONST               4 (False)
+         129         856 LOAD_CONST               3 (None)
          
-         121         854 LOAD_CONST              34 (('user', 'destination', 'state', 'go_on'))
-                     856 BUILD_CONST_KEY_MAP      4
-                     858 LOAD_CONST               6 ('user')
+         130         858 LOAD_CONST               5 (False)
          
-         123         860 LOAD_NAME                4 (handler)
-                     862 LOAD_ATTR                6 (User)
+         125         860 LOAD_CONST              35 (('user', 'destination', 'state', 'go_on'))
+                     862 BUILD_CONST_KEY_MAP      4
+                     864 LOAD_CONST               7 ('user')
          
-         121         872 LOAD_CONST              35 ('destination')
+         127         866 LOAD_NAME                5 (handler)
+                     868 LOAD_ATTR                7 (User)
          
-         124         874 LOAD_NAME                4 (handler)
-                     876 LOAD_ATTR               22 (Destination)
+         125         878 LOAD_CONST              36 ('destination')
          
-         121         886 LOAD_CONST              12 ('state')
+         128         880 LOAD_NAME                5 (handler)
+                     882 LOAD_ATTR               23 (Destination)
          
-         125         888 LOAD_NAME                8 (Optional)
-                     890 LOAD_NAME                9 (str)
-                     892 BINARY_SUBSCR
+         125         892 LOAD_CONST              13 ('state')
          
-         121         902 LOAD_CONST              13 ('go_on')
+         129         894 LOAD_NAME                9 (Optional)
+                     896 LOAD_NAME               10 (str)
+                     898 BINARY_SUBSCR
          
-         126         904 LOAD_NAME                8 (Optional)
-                     906 LOAD_NAME               10 (bool)
-                     908 BINARY_SUBSCR
+         125         908 LOAD_CONST              14 ('go_on')
          
-         121         918 BUILD_TUPLE              8
-                     920 LOAD_CONST              36 (<code object on_user_move, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 121>)
-                     922 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     924 STORE_NAME              23 (on_user_move)
+         130         910 LOAD_NAME                9 (Optional)
+                     912 LOAD_NAME               11 (bool)
+                     914 BINARY_SUBSCR
          
-         134         926 LOAD_CONST               2 (None)
+         125         924 BUILD_TUPLE              8
+                     926 LOAD_CONST              37 (<code object on_user_move, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 125>)
+                     928 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     930 STORE_NAME              24 (on_user_move)
          
-         135         928 LOAD_CONST               2 (None)
+         138         932 LOAD_CONST               3 (None)
          
-         136         930 LOAD_CONST               4 (False)
+         139         934 LOAD_CONST               3 (None)
          
-         132         932 LOAD_CONST              37 (('users', 'seconds_left', 'go_on'))
-                     934 BUILD_CONST_KEY_MAP      3
-                     936 LOAD_CONST              38 ('users')
+         140         936 LOAD_CONST               5 (False)
          
-         134         938 LOAD_NAME               24 (list)
-                     940 LOAD_NAME               25 (tuple)
-                     942 LOAD_NAME                4 (handler)
-                     944 LOAD_ATTR                6 (User)
-                     954 LOAD_NAME               26 (Literal)
-                     956 LOAD_CONST              39 (('voice', 'muted'))
-                     958 BINARY_SUBSCR
-                     968 BUILD_TUPLE              2
-                     970 BINARY_SUBSCR
-                     980 BINARY_SUBSCR
+         136         938 LOAD_CONST              38 (('users', 'seconds_left', 'go_on'))
+                     940 BUILD_CONST_KEY_MAP      3
+                     942 LOAD_CONST              39 ('users')
          
-         132         990 LOAD_CONST              40 ('seconds_left')
+         138         944 LOAD_NAME               25 (list)
+                     946 LOAD_NAME               26 (tuple)
+                     948 LOAD_NAME                5 (handler)
+                     950 LOAD_ATTR                7 (User)
+                     960 LOAD_NAME               27 (Literal)
+                     962 LOAD_CONST              40 (('voice', 'muted'))
+                     964 BINARY_SUBSCR
+                     974 BUILD_TUPLE              2
+                     976 BINARY_SUBSCR
+                     986 BINARY_SUBSCR
          
-         135         992 LOAD_NAME               27 (int)
+         136         996 LOAD_CONST              41 ('seconds_left')
          
-         132         994 LOAD_CONST              13 ('go_on')
+         139         998 LOAD_NAME               28 (int)
          
-         136         996 LOAD_NAME                8 (Optional)
-                     998 LOAD_NAME               10 (bool)
-                    1000 BINARY_SUBSCR
+         136        1000 LOAD_CONST              14 ('go_on')
          
-         132        1010 BUILD_TUPLE              6
-                    1012 LOAD_CONST              41 (<code object on_voice_change, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 132>)
-                    1014 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                    1016 STORE_NAME              28 (on_voice_change)
+         140        1002 LOAD_NAME                9 (Optional)
+                    1004 LOAD_NAME               11 (bool)
+                    1006 BINARY_SUBSCR
          
-         144        1018 LOAD_CONST               2 (None)
+         136        1016 BUILD_TUPLE              6
+                    1018 LOAD_CONST              42 (<code object on_voice_change, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 136>)
+                    1020 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                    1022 STORE_NAME              29 (on_voice_change)
          
-         145        1020 LOAD_CONST               2 (None)
+         148        1024 LOAD_CONST               3 (None)
          
-         146        1022 LOAD_CONST               2 (None)
+         149        1026 LOAD_CONST               3 (None)
          
-         147        1024 LOAD_CONST               2 (None)
+         150        1028 LOAD_CONST               3 (None)
          
-         148        1026 LOAD_CONST               4 (False)
+         151        1030 LOAD_CONST               3 (None)
          
-         142        1028 LOAD_CONST              42 (('user_id', 'conversation_id', 'is_new_conversation', 'state', 'go_on'))
-                    1030 BUILD_CONST_KEY_MAP      5
-                    1032 LOAD_CONST              43 ('user_id')
+         152        1032 LOAD_CONST               5 (False)
          
-         144        1034 LOAD_NAME                9 (str)
+         146        1034 LOAD_CONST              43 (('user_id', 'conversation_id', 'is_new_conversation', 'state', 'go_on'))
+                    1036 BUILD_CONST_KEY_MAP      5
+                    1038 LOAD_CONST              44 ('user_id')
          
-         142        1036 LOAD_CONST              44 ('conversation_id')
+         148        1040 LOAD_NAME               10 (str)
          
-         145        1038 LOAD_NAME                9 (str)
+         146        1042 LOAD_CONST              45 ('conversation_id')
          
-         142        1040 LOAD_CONST              45 ('is_new_conversation')
+         149        1044 LOAD_NAME               10 (str)
          
-         146        1042 LOAD_NAME               10 (bool)
+         146        1046 LOAD_CONST              46 ('is_new_conversation')
          
-         142        1044 LOAD_CONST              12 ('state')
+         150        1048 LOAD_NAME               11 (bool)
          
-         147        1046 LOAD_NAME                8 (Optional)
-                    1048 LOAD_NAME                9 (str)
-                    1050 BINARY_SUBSCR
+         146        1050 LOAD_CONST              13 ('state')
          
-         142        1060 LOAD_CONST              13 ('go_on')
+         151        1052 LOAD_NAME                9 (Optional)
+                    1054 LOAD_NAME               10 (str)
+                    1056 BINARY_SUBSCR
          
-         148        1062 LOAD_NAME                8 (Optional)
-                    1064 LOAD_NAME               10 (bool)
-                    1066 BINARY_SUBSCR
+         146        1066 LOAD_CONST              14 ('go_on')
          
-         142        1076 BUILD_TUPLE             10
-                    1078 LOAD_CONST              46 (<code object on_message, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 142>)
-                    1080 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                    1082 STORE_NAME              29 (on_message)
-                    1084 LOAD_CONST               2 (None)
-                    1086 RETURN_VALUE
+         152        1068 LOAD_NAME                9 (Optional)
+                    1070 LOAD_NAME               11 (bool)
+                    1072 BINARY_SUBSCR
+         
+         146        1082 BUILD_TUPLE             10
+                    1084 LOAD_CONST              47 (<code object on_message, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 146>)
+                    1086 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                    1088 STORE_NAME              30 (on_message)
+                    1090 LOAD_CONST               3 (None)
+                    1092 RETURN_VALUE
          consts
             'DispatcherEvents'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064015300
                 11           0 RESUME                   0
                
-                17           2 LOAD_CONST               1 (None)
+                13           2 LOAD_CONST               1 (None)
+                             4 RETURN_VALUE
+               consts
+                  'Called before the bot starts.'
+                  None
+               names      ()
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
+               name       'before_start'
+               firstlineno 11
+               lnotab 0x0202
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 1
+               flags     : 3
+               code 0x970064015300
+                15           0 RESUME                   0
+               
+                21           2 LOAD_CONST               1 (None)
                              4 RETURN_VALUE
                consts
                   'On a connection to the room being established.\n\n        This may be called multiple times, since the connection may be dropped\n        and reestablished.\n        '
                   None
                names      ()
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       'on_start'
-               firstlineno 11
+               firstlineno 15
                lnotab 0x0206
             None
             '/.!$#'
             False
             ('user', 'message', 'command', 'prefix', 'case_ignore', 'regex', 'state', 'go_on')
             'user'
             'message'
@@ -664,346 +689,346 @@
             'go_on'
             code
                argcount  : 1
                nlocals   : 11
                stacksize : 1
                flags     : 15
                code 0x970064015300
-                19           0 RESUME                   0
+                23           0 RESUME                   0
                
-                33           2 LOAD_CONST               1 (None)
+                37           2 LOAD_CONST               1 (None)
                              4 RETURN_VALUE
                consts
                   'On a received room-wide chat.'
                   None
                names      ()
                varnames   ('self', 'user', 'message', 'command', 'prefix', 'case_ignore', 'regex', 'state', 'go_on', 'custom_filter', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       'on_chat'
-               firstlineno 19
+               firstlineno 23
                lnotab 0x020e
             code
                argcount  : 1
                nlocals   : 11
                stacksize : 1
                flags     : 15
                code 0x970064015300
-                35           0 RESUME                   0
+                39           0 RESUME                   0
                
-                49           2 LOAD_CONST               1 (None)
+                53           2 LOAD_CONST               1 (None)
                              4 RETURN_VALUE
                consts
                   'On a received room whisper.'
                   None
                names      ()
                varnames   ('self', 'user', 'message', 'command', 'prefix', 'case_ignore', 'regex', 'state', 'go_on', 'custom_filter', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       'on_whisper'
-               firstlineno 35
+               firstlineno 39
                lnotab 0x020e
             ('user', 'emote_id', 'receiver', 'state', 'go_on')
             'emote_id'
             'receiver'
             code
                argcount  : 1
                nlocals   : 8
                stacksize : 1
                flags     : 15
                code 0x970064015300
-                51           0 RESUME                   0
+                55           0 RESUME                   0
                
-                62           2 LOAD_CONST               1 (None)
+                66           2 LOAD_CONST               1 (None)
                              4 RETURN_VALUE
                consts
                   'On a received emote.'
                   None
                names      ()
                varnames   ('self', 'user', 'emote_id', 'receiver', 'state', 'go_on', 'custom_filter', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       'on_emote'
-               firstlineno 51
+               firstlineno 55
                lnotab 0x020b
             ('user', 'reaction', 'receiver', 'state', 'go_on')
             'reaction'
             code
                argcount  : 0
                nlocals   : 7
                stacksize : 1
                flags     : 15
                code 0x970064015300
-                64           0 RESUME                   0
+                68           0 RESUME                   0
                
-                74           2 LOAD_CONST               1 (None)
+                78           2 LOAD_CONST               1 (None)
                              4 RETURN_VALUE
                consts
                   'Called when someone reacts in the room.'
                   None
                names      ()
                varnames   ('user', 'reaction', 'receiver', 'state', 'go_on', 'custom_filter', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       'on_reaction'
-               firstlineno 64
+               firstlineno 68
                lnotab 0x020a
             ('user', 'state', 'go_on')
             code
                argcount  : 1
                nlocals   : 6
                stacksize : 1
                flags     : 15
                code 0x970064015300
-                76           0 RESUME                   0
+                80           0 RESUME                   0
                
-                85           2 LOAD_CONST               1 (None)
+                89           2 LOAD_CONST               1 (None)
                              4 RETURN_VALUE
                consts
                   'On a user joining the room.'
                   None
                names      ()
                varnames   ('self', 'user', 'state', 'go_on', 'custom_filter', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       'on_user_join'
-               firstlineno 76
+               firstlineno 80
                lnotab 0x0209
             code
                argcount  : 1
                nlocals   : 6
                stacksize : 1
                flags     : 15
                code 0x970064015300
-                87           0 RESUME                   0
+                91           0 RESUME                   0
                
-                96           2 LOAD_CONST               1 (None)
+               100           2 LOAD_CONST               1 (None)
                              4 RETURN_VALUE
                consts
                   'On a user leaving the room.'
                   None
                names      ()
                varnames   ('self', 'user', 'state', 'go_on', 'custom_filter', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       'on_user_leave'
-               firstlineno 87
+               firstlineno 91
                lnotab 0x0209
             ('sender', 'receiver', 'tip', 'state', 'go_on')
             'sender'
             'tip'
             code
                argcount  : 0
                nlocals   : 7
                stacksize : 1
                flags     : 15
                code 0x970064015300
-                98           0 RESUME                   0
+               102           0 RESUME                   0
                
-               108           2 LOAD_CONST               1 (None)
+               112           2 LOAD_CONST               1 (None)
                              4 RETURN_VALUE
                consts
                   'On a tip received in the room.'
                   None
                names      ()
                varnames   ('sender', 'receiver', 'tip', 'state', 'go_on', 'custom_filter', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       'on_tip'
-               firstlineno 98
+               firstlineno 102
                lnotab 0x020a
             ('sender_id', 'message', 'tags', 'go_on')
             'sender_id'
             'tags'
             code
                argcount  : 0
                nlocals   : 6
                stacksize : 1
                flags     : 15
                code 0x970064015300
-               110           0 RESUME                   0
+               114           0 RESUME                   0
                
-               119           2 LOAD_CONST               1 (None)
+               123           2 LOAD_CONST               1 (None)
                              4 RETURN_VALUE
                consts
                   'On a hidden channel message.'
                   None
                names      ()
                varnames   ('sender_id', 'message', 'tags', 'go_on', 'custom_filter', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       'on_channel'
-               firstlineno 110
+               firstlineno 114
                lnotab 0x0209
             ('user', 'destination', 'state', 'go_on')
             'destination'
             code
                argcount  : 0
                nlocals   : 6
                stacksize : 1
                flags     : 15
                code 0x970064015300
-               121           0 RESUME                   0
+               125           0 RESUME                   0
                
-               130           2 LOAD_CONST               1 (None)
+               134           2 LOAD_CONST               1 (None)
                              4 RETURN_VALUE
                consts
                   'On a user moving in the room.'
                   None
                names      ()
                varnames   ('user', 'destination', 'state', 'go_on', 'custom_filter', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       'on_user_move'
-               firstlineno 121
+               firstlineno 125
                lnotab 0x0209
             ('users', 'seconds_left', 'go_on')
             'users'
             ('voice', 'muted')
             'seconds_left'
             code
                argcount  : 0
                nlocals   : 5
                stacksize : 1
                flags     : 15
                code 0x970064015300
-               132           0 RESUME                   0
+               136           0 RESUME                   0
                
-               140           2 LOAD_CONST               1 (None)
+               144           2 LOAD_CONST               1 (None)
                              4 RETURN_VALUE
                consts
                   'On a change in voice status in the room.'
                   None
                names      ()
                varnames   ('users', 'seconds_left', 'go_on', 'custom_filter', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       'on_voice_change'
-               firstlineno 132
+               firstlineno 136
                lnotab 0x0208
             ('user_id', 'conversation_id', 'is_new_conversation', 'state', 'go_on')
             'user_id'
             'conversation_id'
             'is_new_conversation'
             code
                argcount  : 0
                nlocals   : 7
                stacksize : 1
                flags     : 15
                code 0x970064015300
-               142           0 RESUME                   0
+               146           0 RESUME                   0
                
-               152           2 LOAD_CONST               1 (None)
+               156           2 LOAD_CONST               1 (None)
                              4 RETURN_VALUE
                consts
                   'On a inbox message received from a user.'
                   None
                names      ()
                varnames   ('user_id', 'conversation_id', 'is_new_conversation', 'state', 'go_on', 'custom_filter', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       'on_message'
-               firstlineno 142
+               firstlineno 146
                lnotab 0x020a
-         names      ('__name__', '__module__', '__qualname__', 'on_start', 'handler', 'CaseIgnoreDefaultValue', 'User', 'Message', 'Optional', 'str', 'bool', 'on_chat', 'on_whisper', 'on_emote', 'Reaction', 'on_reaction', 'on_user_join', 'on_user_leave', 'Tip', 'on_tip', 'set', 'on_channel', 'Destination', 'on_user_move', 'list', 'tuple', 'Literal', 'int', 'on_voice_change', 'on_message')
+         names      ('__name__', '__module__', '__qualname__', 'before_start', 'on_start', 'handler', 'CaseIgnoreDefaultValue', 'User', 'Message', 'Optional', 'str', 'bool', 'on_chat', 'on_whisper', 'on_emote', 'Reaction', 'on_reaction', 'on_user_join', 'on_user_leave', 'Tip', 'on_tip', 'set', 'on_channel', 'Destination', 'on_user_move', 'list', 'tuple', 'Literal', 'int', 'on_voice_change', 'on_message')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
          name       'DispatcherEvents'
          firstlineno 10
          lnotab
-            0x0a01060b02010201020102010c010201020102f606030cfd02040cfc02
-            050cfb02060efa02070ef902080ef802090ef7020a0ef608130201020102
-            0102010c010201020102f606030cfd02040cfc02050cfb02060efa02070e
-            f902080ef802090ef7020a0ef60813020102010201020102f906030cfd02
-            040cfc02050cfb02060efa02070ef9080f020102010201020102fa06020c
-            fe02030cfd02040cfc02050efb02060efa080f0201020102fb06030cfd02
-            040efc02050efb080e0201020102fb06030cfd02040efc02050efb080d02
-            0102010201020102fa06020cfe02030cfd02040cfc02050efb02060efa08
-            0e02010201020102fb06020efe02030cfd02041afc02050efb080d020102
-            01020102fb06020cfe02030cfd02040efc02050efb080d0201020102fc06
-            0234fe020302fd02040efc080c020102010201020102fa060202fe020302
-            fd020402fc02050efb02060efa
+            0x0a010604060b02010201020102010c010201020102f606030cfd02040c
+            fc02050cfb02060efa02070ef902080ef802090ef7020a0ef60813020102
+            01020102010c010201020102f606030cfd02040cfc02050cfb02060efa02
+            070ef902080ef802090ef7020a0ef60813020102010201020102f906030c
+            fd02040cfc02050cfb02060efa02070ef9080f020102010201020102fa06
+            020cfe02030cfd02040cfc02050efb02060efa080f0201020102fb06030c
+            fd02040efc02050efb080e0201020102fb06030cfd02040efc02050efb08
+            0d020102010201020102fa06020cfe02030cfd02040cfc02050efb02060e
+            fa080e02010201020102fb06020efe02030cfd02041afc02050efb080d02
+            010201020102fb06020cfe02030cfd02040efc02050efb080d0201020102
+            fc060234fe020302fd02040efc080c020102010201020102fa060202fe02
+            0302fd020402fc02050efb02060efa
       'DispatcherEvents'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x8700970065005a0164005a020900640b6402650365046a050000000000
             0000006a060000000000000000190000000000000000006602640384055a
             07640465086602640584045a09650a6406650b6407650b660464088404a6
             000000ab0000000000000000005a0c88006601640984085a0d640a84005a
             0e880078015a0f5300
                        0 MAKE_CELL                0 (__class__)
          
-         155           2 RESUME                   0
+         159           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Dispatcher')
                       10 STORE_NAME               2 (__qualname__)
          
-         158          12 NOP
+         162          12 NOP
          
-         156          14 LOAD_CONST              11 ((None,))
+         160          14 LOAD_CONST              11 ((None,))
                       16 LOAD_CONST               2 ('fsm_storage')
          
-         158          18 LOAD_NAME                3 (Optional)
+         162          18 LOAD_NAME                3 (Optional)
                       20 LOAD_NAME                4 (fsm)
                       22 LOAD_ATTR                5 (storage)
                       32 LOAD_ATTR                6 (BaseStorage)
                       42 BINARY_SUBSCR
          
-         156          52 BUILD_TUPLE              2
-                      54 LOAD_CONST               3 (<code object __init__, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 156>)
+         160          52 BUILD_TUPLE              2
+                      54 LOAD_CONST               3 (<code object __init__, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 160>)
                       56 MAKE_FUNCTION            5 (defaults, annotations)
                       58 STORE_NAME               7 (__init__)
          
-         168          60 LOAD_CONST               4 ('handler_type')
+         172          60 LOAD_CONST               4 ('handler_type')
                       62 LOAD_NAME                8 (str)
                       64 BUILD_TUPLE              2
-                      66 LOAD_CONST               5 (<code object _process_event, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 168>)
+                      66 LOAD_CONST               5 (<code object _process_event, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 172>)
                       68 MAKE_FUNCTION            4 (annotations)
                       70 STORE_NAME               9 (_process_event)
          
-         171          72 LOAD_NAME               10 (staticmethod)
+         175          72 LOAD_NAME               10 (staticmethod)
          
-         172          74 LOAD_CONST               6 ('handler_data')
+         176          74 LOAD_CONST               6 ('handler_data')
                       76 LOAD_NAME               11 (dict)
                       78 LOAD_CONST               7 ('return')
                       80 LOAD_NAME               11 (dict)
                       82 BUILD_TUPLE              4
-                      84 LOAD_CONST               8 (<code object __pre_processing_handler_data, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 171>)
+                      84 LOAD_CONST               8 (<code object __pre_processing_handler_data, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 175>)
                       86 MAKE_FUNCTION            4 (annotations)
          
-         171          88 PRECALL                  0
+         175          88 PRECALL                  0
                       92 CALL                     0
          
-         172         102 STORE_NAME              12 (_Dispatcher__pre_processing_handler_data)
+         176         102 STORE_NAME              12 (_Dispatcher__pre_processing_handler_data)
          
-         177         104 LOAD_CLOSURE             0 (__class__)
+         181         104 LOAD_CLOSURE             0 (__class__)
                      106 BUILD_TUPLE              1
-                     108 LOAD_CONST               9 (<code object __getattribute__, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 177>)
+                     108 LOAD_CONST               9 (<code object __getattribute__, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 181>)
                      110 MAKE_FUNCTION            8 (closure)
                      112 STORE_NAME              13 (__getattribute__)
          
-         183         114 LOAD_CONST              10 (<code object __create_decorator, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 183>)
+         187         114 LOAD_CONST              10 (<code object __create_decorator, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 187>)
                      116 MAKE_FUNCTION            0
                      118 STORE_NAME              14 (_Dispatcher__create_decorator)
                      120 LOAD_CLOSURE             0 (__class__)
                      122 COPY                     1
                      124 STORE_NAME              15 (__classcell__)
                      126 RETURN_VALUE
          consts
@@ -1022,49 +1047,49 @@
                   0400000000000000000000000000000000000000007c01ac01a6010000ab
                   0100000000000000007c005f0300000000000000007c006a030000000000
                   000000740a000000000000000000006a0600000000000000005f00000000
                   0000000000740f00000000000000000000a6000000ab0000000000000000
                   007c005f0800000000000000007413000000000000000000007c006a0800
                   00000000000000ac02a6010000ab0100000000000000007c005f0a000000
                   000000000064005300
-               156           0 RESUME                   0
+               160           0 RESUME                   0
                
-               160           2 LOAD_FAST                1 (fsm_storage)
+               164           2 LOAD_FAST                1 (fsm_storage)
                              4 POP_JUMP_FORWARD_IF_TRUE    30 (to 66)
                
-               161           6 LOAD_GLOBAL              0 (fsm)
+               165           6 LOAD_GLOBAL              0 (fsm)
                             18 LOAD_ATTR                1 (storage)
                             28 LOAD_METHOD              2 (Memory)
                             50 PRECALL                  0
                             54 CALL                     0
                             64 STORE_FAST               1 (fsm_storage)
                
-               162     >>   66 LOAD_GLOBAL              0 (fsm)
+               166     >>   66 LOAD_GLOBAL              0 (fsm)
                             78 LOAD_ATTR                3 (state)
                             88 LOAD_METHOD              4 (FSMState)
                            110 LOAD_FAST                1 (fsm_storage)
                            112 KW_NAMES                 1
                            114 PRECALL                  1
                            118 CALL                     1
                            128 LOAD_FAST                0 (self)
                            130 STORE_ATTR               3 (state)
                
-               163         140 LOAD_FAST                0 (self)
+               167         140 LOAD_FAST                0 (self)
                            142 LOAD_ATTR                3 (state)
                            152 LOAD_GLOBAL             10 (filter)
                            164 LOAD_ATTR                6 (Check)
                            174 STORE_ATTR               0 (fsm)
                
-               165         184 LOAD_GLOBAL             15 (NULL + list)
+               169         184 LOAD_GLOBAL             15 (NULL + list)
                            196 PRECALL                  0
                            200 CALL                     0
                            210 LOAD_FAST                0 (self)
                            212 STORE_ATTR               8 (_Dispatcher__handlers)
                
-               166         222 LOAD_GLOBAL             19 (NULL + HandlerFactory)
+               170         222 LOAD_GLOBAL             19 (NULL + HandlerFactory)
                            234 LOAD_FAST                0 (self)
                            236 LOAD_ATTR                8 (_Dispatcher__handlers)
                            246 KW_NAMES                 2
                            248 PRECALL                  1
                            252 CALL                     1
                            262 LOAD_FAST                0 (self)
                            264 STORE_ATTR              10 (_Dispatcher__handler_factory)
@@ -1076,31 +1101,31 @@
                   ('handlers',)
                names      ('fsm', 'storage', 'Memory', 'state', 'FSMState', 'filter', 'Check', 'list', '_Dispatcher__handlers', 'HandlerFactory', '_Dispatcher__handler_factory')
                varnames   ('self', 'fsm_storage')
                freevars   ()
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       '__init__'
-               firstlineno 156
+               firstlineno 160
                lnotab 0x020404013c014a012c022601
             'handler_type'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 5
                flags     : 143
                code
                   0x4b000100970002007c006a0000000000000000006a0100000000000000
                   007c0167017c02a201520069007c03a4018e01830064007b035600970386
                   04010064005300
-               168           0 RETURN_GENERATOR
+               172           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               169           6 PUSH_NULL
+               173           6 PUSH_NULL
                              8 LOAD_FAST                0 (self)
                             10 LOAD_ATTR                0 (_Dispatcher__handler_factory)
                             20 LOAD_ATTR                1 (_process)
                             30 LOAD_FAST                1 (handler_type)
                             32 BUILD_LIST               1
                             34 LOAD_FAST                2 (args)
                             36 LIST_EXTEND              1
@@ -1122,61 +1147,61 @@
                   None
                names      ('_Dispatcher__handler_factory', '_process')
                varnames   ('self', 'handler_type', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       '_process_event'
-               firstlineno 168
+               firstlineno 172
                lnotab 0x0601
             'handler_data'
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   00a6020000ab020000000000000000721d7403000000000000000000006a
                   0200000000000000007c00640119000000000000000000a6010000ab0100
                   000000000000007c0064013c0000007c005300
-               171           0 RESUME                   0
+               175           0 RESUME                   0
                
-               173           2 LOAD_FAST                0 (handler_data)
+               177           2 LOAD_FAST                0 (handler_data)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('regex')
                             28 LOAD_CONST               0 (None)
                             30 PRECALL                  2
                             34 CALL                     2
                             44 POP_JUMP_FORWARD_IF_FALSE    29 (to 104)
                
-               174          46 LOAD_GLOBAL              3 (NULL + re)
+               178          46 LOAD_GLOBAL              3 (NULL + re)
                             58 LOAD_ATTR                2 (compile)
                             68 LOAD_FAST                0 (handler_data)
                             70 LOAD_CONST               1 ('regex')
                             72 BINARY_SUBSCR
                             82 PRECALL                  1
                             86 CALL                     1
                             96 LOAD_FAST                0 (handler_data)
                             98 LOAD_CONST               1 ('regex')
                            100 STORE_SUBSCR
                
-               175     >>  104 LOAD_FAST                0 (handler_data)
+               179     >>  104 LOAD_FAST                0 (handler_data)
                            106 RETURN_VALUE
                consts
                   None
                   'regex'
                names      ('get', 're', 'compile')
                varnames   ('handler_data',)
                freevars   ()
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       '__pre_processing_handler_data'
-               firstlineno 171
+               firstlineno 175
                lnotab 0x02022c013a01
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
@@ -1185,39 +1210,39 @@
                   0300000000000000007c01a6020000ab02000000000000000072157c00a0
                   0400000000000000000000000000000000000000007c01a6010000ab0100
                   000000000000005300740b00000000000000000000a6000000ab00000000
                   0000000000a00600000000000000000000000000000000000000007c01a6
                   010000ab0100000000000000005300
                              0 COPY_FREE_VARS           1
                
-               177           2 RESUME                   0
+               181           2 RESUME                   0
                
-               178           4 LOAD_GLOBAL              1 (NULL + importlib)
+               182           4 LOAD_GLOBAL              1 (NULL + importlib)
                             16 LOAD_ATTR                1 (import_module)
                             26 LOAD_CONST               1 ('hrbot.bot.bot')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 STORE_FAST               2 (bot_module)
                
-               179          44 LOAD_GLOBAL              5 (NULL + hasattr)
+               183          44 LOAD_GLOBAL              5 (NULL + hasattr)
                             56 LOAD_FAST                2 (bot_module)
                             58 LOAD_ATTR                3 (Bot)
                             68 LOAD_FAST                1 (method_name)
                             70 PRECALL                  2
                             74 CALL                     2
                             84 POP_JUMP_FORWARD_IF_FALSE    21 (to 128)
                
-               180          86 LOAD_FAST                0 (self)
+               184          86 LOAD_FAST                0 (self)
                             88 LOAD_METHOD              4 (_Dispatcher__create_decorator)
                            110 LOAD_FAST                1 (method_name)
                            112 PRECALL                  1
                            116 CALL                     1
                            126 RETURN_VALUE
                
-               181     >>  128 LOAD_GLOBAL             11 (NULL + super)
+               185     >>  128 LOAD_GLOBAL             11 (NULL + super)
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_METHOD              6 (__getattribute__)
                            176 LOAD_FAST                1 (method_name)
                            178 PRECALL                  1
                            182 CALL                     1
                            192 RETURN_VALUE
@@ -1226,35 +1251,35 @@
                   'hrbot.bot.bot'
                names      ('importlib', 'import_module', 'hasattr', 'Bot', '_Dispatcher__create_decorator', 'super', '__getattribute__')
                varnames   ('self', 'method_name', 'bot_module')
                freevars   ('__class__',)
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       '__getattribute__'
-               firstlineno 177
+               firstlineno 181
                lnotab 0x040128012a012a01
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 2
                flags     : 3
                code 0x870087019700880188006602640184087d027c025300
                              0 MAKE_CELL                0 (self)
                              2 MAKE_CELL                1 (method_name)
                
-               183           4 RESUME                   0
+               187           4 RESUME                   0
                
-               184           6 LOAD_CLOSURE             1 (method_name)
+               188           6 LOAD_CLOSURE             1 (method_name)
                              8 LOAD_CLOSURE             0 (self)
                             10 BUILD_TUPLE              2
-                            12 LOAD_CONST               1 (<code object wrapper, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 184>)
+                            12 LOAD_CONST               1 (<code object wrapper, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 188>)
                             14 MAKE_FUNCTION            8 (closure)
                             16 STORE_FAST               2 (wrapper)
                
-               200          18 LOAD_FAST                2 (wrapper)
+               204          18 LOAD_FAST                2 (wrapper)
                             20 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 0
                      nlocals   : 3
                      stacksize : 4
@@ -1263,33 +1288,33 @@
                         0x95028700870197008904a0000000000000000000000000000000000000
                         0000008901a6010000ab0100000000000000008a01880088018803880466
                         04640184087d027c025300
                                    0 COPY_FREE_VARS           2
                                    2 MAKE_CELL                0 (custom_filter)
                                    4 MAKE_CELL                1 (kwargs)
                      
-                     184           6 RESUME                   0
+                     188           6 RESUME                   0
                      
-                     185           8 LOAD_DEREF               4 (self)
+                     189           8 LOAD_DEREF               4 (self)
                                   10 LOAD_METHOD              0 (_Dispatcher__pre_processing_handler_data)
                                   32 LOAD_DEREF               1 (kwargs)
                                   34 PRECALL                  1
                                   38 CALL                     1
                                   48 STORE_DEREF              1 (kwargs)
                      
-                     187          50 LOAD_CLOSURE             0 (custom_filter)
+                     191          50 LOAD_CLOSURE             0 (custom_filter)
                                   52 LOAD_CLOSURE             1 (kwargs)
                                   54 LOAD_CLOSURE             3 (method_name)
                                   56 LOAD_CLOSURE             4 (self)
                                   58 BUILD_TUPLE              4
-                                  60 LOAD_CONST               1 (<code object decorator, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 187>)
+                                  60 LOAD_CONST               1 (<code object decorator, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 191>)
                                   62 MAKE_FUNCTION            8 (closure)
                                   64 STORE_FAST               2 (decorator)
                      
-                     198          66 LOAD_FAST                2 (decorator)
+                     202          66 LOAD_FAST                2 (decorator)
                                   68 RETURN_VALUE
                      consts
                         None
                         code
                            argcount  : 1
                            nlocals   : 1
                            stacksize : 12
@@ -1299,89 +1324,89 @@
                               000000000000000000740500000000000000000000890374070000000000
                               00000000007408000000000000000000008903a6020000ab020000000000
                               0000007c008901740b0000000000000000000089026401ac02a6020000ab
                               020000000000000000ac03a6050000ab050000000000000000a6010000ab
                               01000000000000000001007c005300
                                          0 COPY_FREE_VARS           4
                            
-                           187           2 RESUME                   0
+                           191           2 RESUME                   0
                            
-                           189           4 LOAD_DEREF               4 (self)
+                           193           4 LOAD_DEREF               4 (self)
                                          6 LOAD_ATTR                0 (_Dispatcher__handlers)
                                         16 LOAD_METHOD              1 (append)
                                         38 LOAD_GLOBAL              5 (NULL + HandlerObj)
                            
-                           190          50 LOAD_DEREF               3 (method_name)
+                           194          50 LOAD_DEREF               3 (method_name)
                            
-                           191          52 LOAD_GLOBAL              7 (NULL + getattr)
+                           195          52 LOAD_GLOBAL              7 (NULL + getattr)
                                         64 LOAD_GLOBAL              8 (filter)
                                         76 LOAD_DEREF               3 (method_name)
                                         78 PRECALL                  2
                                         82 CALL                     2
                            
-                           192          92 LOAD_FAST                0 (callback)
+                           196          92 LOAD_FAST                0 (callback)
                            
-                           193          94 LOAD_DEREF               1 (custom_filter)
+                           197          94 LOAD_DEREF               1 (custom_filter)
                            
-                           194          96 LOAD_GLOBAL             11 (NULL + DictWrapper)
+                           198          96 LOAD_GLOBAL             11 (NULL + DictWrapper)
                                        108 LOAD_DEREF               2 (kwargs)
                                        110 LOAD_CONST               1 (False)
                                        112 KW_NAMES                 2
                                        114 PRECALL                  2
                                        118 CALL                     2
                            
-                           189         128 KW_NAMES                 3
+                           193         128 KW_NAMES                 3
                                        130 PRECALL                  5
                                        134 CALL                     5
                                        144 PRECALL                  1
                                        148 CALL                     1
                                        158 POP_TOP
                            
-                           196         160 LOAD_FAST                0 (callback)
+                           200         160 LOAD_FAST                0 (callback)
                                        162 RETURN_VALUE
                            consts
                               None
                               False
                               ('rise_exception',)
                               ('type', 'filter_func', 'callback', 'custom_filters', 'data')
                            names      ('_Dispatcher__handlers', 'append', 'HandlerObj', 'getattr', 'filter', 'DictWrapper')
                            varnames   ('callback',)
                            freevars   ('custom_filter', 'kwargs', 'method_name', 'self')
                            cellvars   ()
                            filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                            name       'decorator'
-                           firstlineno 187
+                           firstlineno 191
                            lnotab 0x04022e01020128010201020120fb2007
                      names      ('_Dispatcher__pre_processing_handler_data',)
                      varnames   ('custom_filter', 'kwargs', 'decorator')
                      freevars   ('method_name', 'self')
                      cellvars   ('custom_filter', 'kwargs')
                      filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                      name       'wrapper'
-                     firstlineno 184
+                     firstlineno 188
                      lnotab 0x08012a02100b
                names      ()
                varnames   ('self', 'method_name', 'wrapper')
                freevars   ()
                cellvars   ('self', 'method_name')
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       '__create_decorator'
-               firstlineno 183
+               firstlineno 187
                lnotab 0x06010c10
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'Optional', 'fsm', 'storage', 'BaseStorage', '__init__', 'str', '_process_event', 'staticmethod', 'dict', '_Dispatcher__pre_processing_handler_data', '__getattribute__', '_Dispatcher__create_decorator', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
          name       'Dispatcher'
-         firstlineno 155
+         firstlineno 159
          lnotab 0x0c0302fe040222fe080c0c0302010eff0e0102050a06
       'Dispatcher'
    names      ('importlib', 're', 'handler', 'HandlerFactory', 'DictWrapper', 'HandlerObj', '', 'filter', 'fsm', 'types', 'typing', 'Optional', 'Literal', 'DispatcherEvents', 'Dispatcher')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020108010802140110010c0110031a7f0012
+   lnotab 0x00ff020108010802140110010c0110031a7f0016
```

### Comparing `hrbot-0.1.2/hrbot/dispatcher/dispatсher.py` & `hrbot-0.1.3/hrbot/dispatcher/dispatсher.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 from .handler import HandlerFactory, DictWrapper, HandlerObj
 from . import filter, fsm
 from ..types import handler
 from typing import Optional, Literal
 
 
 class DispatcherEvents:
+    def before_start(self):
+        """Called before the bot starts."""
+        pass
+
     def on_start(self):
         """On a connection to the room being established.
 
         This may be called multiple times, since the connection may be dropped
         and reestablished.
         """
         pass
```

### Comparing `hrbot-0.1.2/hrbot/dispatcher/filter.py` & `hrbot-0.1.3/hrbot/dispatcher/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         if event_message[0] not in handler_prefix:
             return False
 
         if event_message[1:] in handler_commands:
             return True
         return False
 
-
+async def before_start(*args, **kwargs) -> bool: return True
 async def on_start(*args, **kwargs) -> bool: return True
 
 
 async def on_chat(
         handler_filter: HandlerObj,
         user: hr.User,
         message: str,
```

### Comparing `hrbot-0.1.2/hrbot/dispatcher/fsm/state.py` & `hrbot-0.1.3/hrbot/dispatcher/fsm/state.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.2/hrbot/dispatcher/fsm/storage.py` & `hrbot-0.1.3/hrbot/dispatcher/fsm/storage.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.2/hrbot/dispatcher/handler.py` & `hrbot-0.1.3/hrbot/dispatcher/handler.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.2/LICENSE` & `hrbot-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.2/README.md` & `hrbot-0.1.3/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 ```shell  
 pip install hrbot  
 ```  
 # Features:  
 - Quick and easy creation of an unlimited number of handlers for any event  
 - FSM (finite state machine). Available storage in memory and Redis  
 - Large number of available conditions in handlers  
-# Unreleased features:
 - Web API support
+# Unreleased features:
 - Spam blocking bypass. Allows you to send an unlimited number of identical messages
 # Example:  
 ```python  
 from hrbot import Bot, Dispatcher  
 from hrbot.types.hr import User  
   
 dp = Dispatcher()
```

### Comparing `hrbot-0.1.2/PKG-INFO` & `hrbot-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: hrbot
-Version: 0.1.2
+Version: 0.1.3
 Summary: The hrbot is a wrapper on top of the HighRise Python Bot SDK that makes it easy to create bots in HighRise.
 License: MIT
 Author: MuoDosta
 Author-email: MuoDostaWork@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: highrise-bot-sdk (==23.1.0b13)
+Requires-Dist: highrise-bot-sdk (==23.1.0b15)
 Requires-Dist: redis (==4.5.5)
 Description-Content-Type: text/markdown
 
 
 # The hrbot  
 The hrbot is a wrapper on top of the [HighRise Python Bot SDK](https://github.com/pocketzworld/python-bot-sdk) that makes it easy to create bots in [HighRise](https://highrise.game/).  
   
@@ -22,16 +22,16 @@
 ```shell  
 pip install hrbot  
 ```  
 # Features:  
 - Quick and easy creation of an unlimited number of handlers for any event  
 - FSM (finite state machine). Available storage in memory and Redis  
 - Large number of available conditions in handlers  
-# Unreleased features:
 - Web API support
+# Unreleased features:
 - Spam blocking bypass. Allows you to send an unlimited number of identical messages
 # Example:  
 ```python  
 from hrbot import Bot, Dispatcher  
 from hrbot.types.hr import User  
   
 dp = Dispatcher()
```

