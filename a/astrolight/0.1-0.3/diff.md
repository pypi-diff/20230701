# Comparing `tmp/astrolight-0.1-py3-none-any.whl.zip` & `tmp/astrolight-0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 7447 bytes, number of entries: 16
+Zip file size: 7725 bytes, number of entries: 16
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 astrolight/__init__.py
--rw-r--r--  2.0 unx     1191 b- defN 80-Jan-01 00:00 astrolight/__main__.py
+-rw-r--r--  2.0 unx     1208 b- defN 80-Jan-01 00:00 astrolight/__main__.py
 -rw-r--r--  2.0 unx      381 b- defN 80-Jan-01 00:00 astrolight/account_connector.py
--rw-r--r--  2.0 unx     2549 b- defN 80-Jan-01 00:00 astrolight/app.py
+-rw-r--r--  2.0 unx     3751 b- defN 80-Jan-01 00:00 astrolight/app.py
 -rw-r--r--  2.0 unx      301 b- defN 80-Jan-01 00:00 astrolight/config.py
 -rw-r--r--  2.0 unx      934 b- defN 80-Jan-01 00:00 astrolight/ewelink_connector.py
 -rw-r--r--  2.0 unx      904 b- defN 80-Jan-01 00:00 astrolight/timer.py
 -rw-r--r--  2.0 unx      336 b- defN 80-Jan-01 00:00 astrolight/times/__init__.py
 -rw-r--r--  2.0 unx     1024 b- defN 80-Jan-01 00:00 astrolight/times/dynamic_time.py
 -rw-r--r--  2.0 unx     2447 b- defN 80-Jan-01 00:00 astrolight/times/expression.py
 -rw-r--r--  2.0 unx      811 b- defN 80-Jan-01 00:00 astrolight/times/sun_time.py
--rw-r--r--  2.0 unx     1459 b- defN 80-Jan-01 00:00 astrolight-0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 astrolight-0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       56 b- defN 80-Jan-01 00:00 astrolight-0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 80-Jan-01 00:00 astrolight-0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1296 b- defN 80-Jan-01 00:00 astrolight-0.1.dist-info/RECORD
-16 files, 13792 bytes uncompressed, 5303 bytes compressed:  61.6%
+-rw-r--r--  2.0 unx     1464 b- defN 80-Jan-01 00:00 astrolight-0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 astrolight-0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 80-Jan-01 00:00 astrolight-0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 80-Jan-01 00:00 astrolight-0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1296 b- defN 80-Jan-01 00:00 astrolight-0.3.dist-info/RECORD
+16 files, 15016 bytes uncompressed, 5581 bytes compressed:  62.8%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: astrolight/times/expression.py
 Comment: 
 
 Filename: astrolight/times/sun_time.py
 Comment: 
 
-Filename: astrolight-0.1.dist-info/METADATA
+Filename: astrolight-0.3.dist-info/METADATA
 Comment: 
 
-Filename: astrolight-0.1.dist-info/WHEEL
+Filename: astrolight-0.3.dist-info/WHEEL
 Comment: 
 
-Filename: astrolight-0.1.dist-info/entry_points.txt
+Filename: astrolight-0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: astrolight-0.1.dist-info/top_level.txt
+Filename: astrolight-0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: astrolight-0.1.dist-info/RECORD
+Filename: astrolight-0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## astrolight/__main__.py

```diff
@@ -33,16 +33,16 @@
     start_time = datetime.now()
 
     def get_time_func() -> datetime:
         return start_time + time_multiplier * (datetime.now() - start_time)
 
     interval: float = args.interval / time_multiplier
 
-    app = App(config, get_time_func)
-    await app.run(interval)
+    async with App(config, get_time_func) as app:
+        await app.run(interval)
 
 
 def main() -> None:
     asyncio.run(amain())
 
 
 if __name__ == "__main__":
```

## astrolight/app.py

```diff
@@ -1,12 +1,15 @@
 import asyncio
 import logging
 from datetime import datetime
+from traceback import TracebackException
+from types import TracebackType
 from typing import Callable
 
+from .account_connector import Connector
 from .config import Config
 
 
 class App:
     def __init__(
         self,
         config: Config,
@@ -17,14 +20,28 @@
 
         # Initializing
         self._connectors = [account.connector() for account in config.accounts]
 
         logging.info("Initial states are assumed to be correct.")
         self._previous_light_states = self._light_states(self.get_time_func())
 
+    async def __aenter__(self) -> "App":
+        return self
+
+    async def __aexit__(
+        self,
+        exc_type: Exception,
+        exc_val: TracebackException,
+        traceback: TracebackType,
+    ) -> None:
+        await self.close()
+
+    async def close(self) -> None:
+        await asyncio.wait([connector.close() for connector in self._connectors])
+
     @property
     def lights(self) -> set[str]:
         timers = self.config.on
         # return {light for light in [timer.lights for timer in timers]}
         return {light for timer in timers for light in timer.lights}
 
     async def run(self, interval: float = 300) -> None:
@@ -49,17 +66,15 @@
         logging.info("---")
         logging.info(f"The time is {time}")
         logging.info(f"The (previous) light states were: {self._previous_light_states}")
         logging.info(f"The (current)  light states are:  {current_light_states}")
         logging.info(f"The (changed)  light states are:  {changed_light_states}")
 
         for light, state in changed_light_states.items():
-            logging.info(f"Turning {'on' if state else 'off'} the {light} light.")
-            for connector in self._connectors:
-                await connector.set_light_state(light, state)
+            await self._set_light_state(light, state)
 
         # Finally, update previous light states
         self._previous_light_states = current_light_states
 
     def _light_states(self, time: datetime) -> dict[str, bool]:
         location = self.config.location
 
@@ -70,7 +85,32 @@
         timers = self.config.on
         for timer in timers:
             if timer.is_active(time, location):
                 for light in timer.lights:
                     light_states[light] = True
 
         return light_states
+
+    async def _set_light_state(self, light: str, state: bool) -> None:
+        logging.info(f"Turning {'on' if state else 'off'} the {light} light.")
+
+        async def try_set_light_state(connector: Connector, light: str, state: bool) -> None:
+            errors = []
+
+            for i in range(5):
+                try:
+                    await connector.set_light_state(light, state)
+                    return
+                except Exception as e:
+                    errors.append(e)
+
+            logging.error(
+                "\n".join(
+                    [
+                        f"Failed to turn {'on' if state else 'off'} the {light} light.",
+                        f"Errors: {errors}",
+                    ]
+                )
+            )
+
+        for connector in self._connectors:
+            await try_set_light_state(connector, light, state)
```

## Comparing `astrolight-0.1.dist-info/METADATA` & `astrolight-0.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: astrolight
-Version: 0.1
+Version: 0.3
 Requires-Python: >=3.9
 Requires-Dist: PyYAML
-Requires-Dist: pydantic
+Requires-Dist: pydantic (<2)
 Requires-Dist: suntime
 Requires-Dist: ewelink (~=0.2)
 Provides-Extra: black
 Requires-Dist: black (==22.8.0) ; extra == 'black'
 Provides-Extra: dev
 Requires-Dist: tox ; extra == 'dev'
 Requires-Dist: pytest (>=7) ; extra == 'dev'
```

## Comparing `astrolight-0.1.dist-info/RECORD` & `astrolight-0.3.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 astrolight/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-astrolight/__main__.py,sha256=RdYL-sbW2q9oxROGTXdcSajJ4uS2TzC8rQAQSXMNyY0,1191
+astrolight/__main__.py,sha256=bS0tUU6StLFiScwaniurpgRB0154DR-fAZHJRYDKgPk,1208
 astrolight/account_connector.py,sha256=Rvkk0Q_T9p30vYYu2zCHlAGlI1yukTjyU7A7NqqBA4w,381
-astrolight/app.py,sha256=gRb1y5mtVbctucZMNWk44cOfEIdFRxRLk1cgZrh3Ml4,2549
+astrolight/app.py,sha256=-sGmw3wkB3DL8Giebv1mVRPNxKbxST3Gf8KmLDw87bs,3751
 astrolight/config.py,sha256=EuFDjIEJ1tLbJNpd6-qndCe7d7lecXw-kCaw1uZEQzQ,301
 astrolight/ewelink_connector.py,sha256=uxnkalvvIXdAVC2zXRZtp4FGj2WyfM4kSaqOw-bJVP4,934
 astrolight/timer.py,sha256=ZqZFIw3uEcHptsykS2Rxin78Vw7gNuNSBKikhbHk_xc,904
 astrolight/times/__init__.py,sha256=XisrJv3R2FUwjVddcstWhdvtsql061kCWPxm88-5WNI,336
 astrolight/times/dynamic_time.py,sha256=v7az0s1ghv8PD8Og08Y3CBkuiDHCTFs__R33-NPxITg,1024
 astrolight/times/expression.py,sha256=_C3geVbmsD2rRgywNq4Fb3tC40TezcC1uO7LqT5NqVc,2447
 astrolight/times/sun_time.py,sha256=HdXsTDvon7RF0nbs4eZGjH--VeZpIKFYk_BHeTZ-1aI,811
-astrolight-0.1.dist-info/METADATA,sha256=XMCSxDYNWYzw71Uju_J6vqBZ0ychLJwiawRVJ6OCCKU,1459
-astrolight-0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-astrolight-0.1.dist-info/entry_points.txt,sha256=kErt6MFVuXvbFQi3AJxVmtblUUK6QH6TsuJCAp8OMks,56
-astrolight-0.1.dist-info/top_level.txt,sha256=RwkHCgwISRvXY4av5ntRSqw92f2_TkYDuJY80JeFa5I,11
-astrolight-0.1.dist-info/RECORD,,
+astrolight-0.3.dist-info/METADATA,sha256=s-pgS1N1QDPldvmCzIwP-6Fg65UYzNcyydLuvHxzlwU,1464
+astrolight-0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+astrolight-0.3.dist-info/entry_points.txt,sha256=kErt6MFVuXvbFQi3AJxVmtblUUK6QH6TsuJCAp8OMks,56
+astrolight-0.3.dist-info/top_level.txt,sha256=RwkHCgwISRvXY4av5ntRSqw92f2_TkYDuJY80JeFa5I,11
+astrolight-0.3.dist-info/RECORD,,
```

