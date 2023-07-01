# Comparing `tmp/cronsim-2.4.1.tar.gz` & `tmp/cronsim-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cronsim-2.4.1.tar", last modified: Thu Apr 27 15:49:44 2023, max compression
+gzip compressed data, was "cronsim-2.5.tar", last modified: Sat Jul  1 07:48:53 2023, max compression
```

## Comparing `cronsim-2.4.1.tar` & `cronsim-2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 cepe      (1000) cepe      (1000)        0 2023-04-27 15:49:44.206700 cronsim-2.4.1/
--rw-r--r--   0 cepe      (1000) cepe      (1000)     1484 2021-05-16 16:31:36.000000 cronsim-2.4.1/LICENSE
--rw-rw-r--   0 cepe      (1000) cepe      (1000)       24 2022-09-28 14:26:08.000000 cronsim-2.4.1/MANIFEST.in
--rw-rw-r--   0 cepe      (1000) cepe      (1000)     5502 2023-04-27 15:49:44.206700 cronsim-2.4.1/PKG-INFO
--rw-rw-r--   0 cepe      (1000) cepe      (1000)     4707 2023-04-27 15:47:03.000000 cronsim-2.4.1/README.md
-drwxrwxr-x   0 cepe      (1000) cepe      (1000)        0 2023-04-27 15:49:44.206700 cronsim-2.4.1/cronsim/
--rw-rw-r--   0 cepe      (1000) cepe      (1000)       70 2022-09-28 11:52:58.000000 cronsim-2.4.1/cronsim/__init__.py
--rw-rw-r--   0 cepe      (1000) cepe      (1000)    10693 2023-04-24 10:56:48.000000 cronsim-2.4.1/cronsim/cronsim.py
--rw-rw-r--   0 cepe      (1000) cepe      (1000)    19130 2023-04-27 15:47:50.000000 cronsim-2.4.1/cronsim/explain.py
--rw-rw-r--   0 cepe      (1000) cepe      (1000)        0 2022-09-28 07:26:47.000000 cronsim-2.4.1/cronsim/py.typed
-drwxrwxr-x   0 cepe      (1000) cepe      (1000)        0 2023-04-27 15:49:44.206700 cronsim-2.4.1/cronsim.egg-info/
--rw-rw-r--   0 cepe      (1000) cepe      (1000)     5502 2023-04-27 15:49:44.000000 cronsim-2.4.1/cronsim.egg-info/PKG-INFO
--rw-rw-r--   0 cepe      (1000) cepe      (1000)      267 2023-04-27 15:49:44.000000 cronsim-2.4.1/cronsim.egg-info/SOURCES.txt
--rw-rw-r--   0 cepe      (1000) cepe      (1000)        1 2023-04-27 15:49:44.000000 cronsim-2.4.1/cronsim.egg-info/dependency_links.txt
--rw-rw-r--   0 cepe      (1000) cepe      (1000)        1 2022-09-28 14:37:53.000000 cronsim-2.4.1/cronsim.egg-info/not-zip-safe
--rw-rw-r--   0 cepe      (1000) cepe      (1000)        8 2023-04-27 15:49:44.000000 cronsim-2.4.1/cronsim.egg-info/top_level.txt
--rw-rw-r--   0 cepe      (1000) cepe      (1000)       38 2023-04-27 15:49:44.206700 cronsim-2.4.1/setup.cfg
--rw-rw-r--   0 cepe      (1000) cepe      (1000)     1449 2023-04-27 15:46:20.000000 cronsim-2.4.1/setup.py
+drwxrwxr-x   0 cepe      (1000) cepe      (1000)        0 2023-07-01 07:48:53.912428 cronsim-2.5/
+-rw-r--r--   0 cepe      (1000) cepe      (1000)     1484 2021-05-16 16:31:36.000000 cronsim-2.5/LICENSE
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)       24 2022-09-28 14:26:08.000000 cronsim-2.5/MANIFEST.in
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)     6654 2023-07-01 07:48:53.912428 cronsim-2.5/PKG-INFO
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)     5850 2023-07-01 07:42:47.000000 cronsim-2.5/README.md
+drwxrwxr-x   0 cepe      (1000) cepe      (1000)        0 2023-07-01 07:48:53.912428 cronsim-2.5/cronsim/
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)       70 2022-09-28 11:52:58.000000 cronsim-2.5/cronsim/__init__.py
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)    11716 2023-07-01 07:19:35.000000 cronsim-2.5/cronsim/cronsim.py
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)    19921 2023-07-01 06:56:44.000000 cronsim-2.5/cronsim/explain.py
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)        0 2022-09-28 07:26:47.000000 cronsim-2.5/cronsim/py.typed
+drwxrwxr-x   0 cepe      (1000) cepe      (1000)        0 2023-07-01 07:48:53.912428 cronsim-2.5/cronsim.egg-info/
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)     6654 2023-07-01 07:48:53.000000 cronsim-2.5/cronsim.egg-info/PKG-INFO
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)      267 2023-07-01 07:48:53.000000 cronsim-2.5/cronsim.egg-info/SOURCES.txt
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)        1 2023-07-01 07:48:53.000000 cronsim-2.5/cronsim.egg-info/dependency_links.txt
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)        1 2022-09-28 14:37:53.000000 cronsim-2.5/cronsim.egg-info/not-zip-safe
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)        8 2023-07-01 07:48:53.000000 cronsim-2.5/cronsim.egg-info/top_level.txt
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)       38 2023-07-01 07:48:53.912428 cronsim-2.5/setup.cfg
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)     1458 2023-07-01 06:53:03.000000 cronsim-2.5/setup.py
```

### Comparing `cronsim-2.4.1/LICENSE` & `cronsim-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cronsim-2.4.1/PKG-INFO` & `cronsim-2.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cronsim
-Version: 2.4.1
+Version: 2.5
 Summary: Cron expression parser and evaluator
 Home-page: https://github.com/cuu508/cronsim
 Author: Pēteris Caune
-Author-email: cuu508@gmail.com
+Author-email: cuu508@monkeyseemonkeydo.lv
 License: BSD
 Project-URL: Changelog, https://github.com/cuu508/cronsim/blob/main/CHANGELOG.md
 Keywords: cron,cronjob,crontab,schedule
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -50,29 +50,63 @@
 from cronsim import CronSim
 
 it = CronSim("0 0 * 2 MON#5", datetime.now())
 for x in range(0, 10):
     print(next(it))
 ```
 
-Outputs:
+Produces:
 
 ```
 2044-02-29 00:00:00
 2072-02-29 00:00:00
 2112-02-29 00:00:00
 2140-02-29 00:00:00
 2168-02-29 00:00:00
 2196-02-29 00:00:00
 2208-02-29 00:00:00
 2236-02-29 00:00:00
 2264-02-29 00:00:00
 2292-02-29 00:00:00
 ```
 
+If CronSim receives an invalid cron expression, it raises `cronsim.CronSimError`:
+
+```python
+from datetime import datetime
+from cronsim import CronSim
+
+CronSim("123 * * * *", datetime.now())
+```
+
+Produces:
+
+```
+cronsim.cronsim.CronSimError: Bad minute
+```
+
+If CronSim cannot find a matching datetime in the next 50 years from the start
+date or from the previous match, it stops iteration by raising `StopIteration`:
+
+```python
+from datetime import datetime
+from cronsim import CronSim
+
+# Every minute of 1st and 21st of month,
+# if it is also the *last Monday* of the month:
+it = CronSim("* * */20 * 1L", datetime.now())
+print(next(it))
+```
+
+Produces:
+
+```
+StopIteration
+```
+
 ## CronSim Works With zoneinfo
 
 CronSim starting from version 2.0 is designed to work with timezones provided by
 the zoneinfo module.
 
 A previous version, CronSim 1.0, was designed for pytz and relied on its
 following non-standard features:
@@ -109,32 +143,39 @@
 ```
 
 See test cases in `test_cronsim.py`, `TestDstTransitions` class
 for examples of this special handling.
 
 ## Cron Expression Feature Matrix
 
-| Feature                              | Debian | croniter | cronsim |
-| ------------------------------------ | :----: | :------: | :-----: |
-| Seconds in the 6th field             | No     | Yes      | No      |
-| "L" as the day-of-month              | No     | Yes      | Yes     |
-| "L" in the day-of-week field         | No     | No       | Yes     |
-| Nth weekday of month                 | No     | Yes      | Yes     |
+| Feature                              | Debian | Quartz | croniter | cronsim |
+| ------------------------------------ | :----: | :----: | :------: | :-----: |
+| Seconds in the 6th field             | No     | Yes    | Yes      | No      |
+| "L" as the day-of-month              | No     | Yes    | Yes      | Yes     |
+| "LW" as the day-of-month             | No     | Yes    | No       | Yes     |
+| "L" in the day-of-week field         | No     | Yes    | No       | Yes     |
+| Nth weekday of month                 | No     | Yes    | Yes      | Yes     |
 
 
 **Seconds in the 6th field**: an optional sixth field specifying seconds.
-Supports the same syntax features as the minutes field.
+Supports the same syntax features as the minutes field. Quartz Scheduler
+expects seconds in the first field, croniter expects seconds in the last field.
 
-Example: `* * * * * */15` (every 15 seconds).
+Quartz example: `*/15 * * * * *` (every 15 seconds).
 
 **"L" as the day-of-month**: support for the "L" special character in the
 day-of-month field. Interpreted as "the last day of the month".
 
 Example: `0 0 L * *` (at the midnight of the last day of every month).
 
+**"LW" as the day-of-month**: support for the "LW" special value in the
+day-of-month field. Interpreted as "the last weekday (Mon-Fri) of the month".
+
+Example: `0 0 LW * *` (at the midnight of the last weekday of every month).
+
 **"L" in the day-of-week field**: support for the "{weekday}L" syntax.
 For example, "5L" means "the last Friday of the month".
 
 Example: `0 0 * * 6L` (at the midnight of the last Saturday of every month).
 
 **Nth weekday of month**: support for "{weekday}#{nth}" syntax.
 For example, "MON#1" means "first Monday of the month", "MON#2" means "second Monday
```

### Comparing `cronsim-2.4.1/README.md` & `cronsim-2.5/cronsim.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: cronsim
+Version: 2.5
+Summary: Cron expression parser and evaluator
+Home-page: https://github.com/cuu508/cronsim
+Author: Pēteris Caune
+Author-email: cuu508@monkeyseemonkeydo.lv
+License: BSD
+Project-URL: Changelog, https://github.com/cuu508/cronsim/blob/main/CHANGELOG.md
+Keywords: cron,cronjob,crontab,schedule
+Platform: any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >= 3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # CronSim
 
 [![Tests](https://github.com/cuu508/cronsim/actions/workflows/pytest.yml/badge.svg)](https://github.com/cuu508/cronsim/actions/workflows/pytest.yml)
 
 Cron Sim(ulator), a cron expression parser and evaluator. Works with Python 3.8+.
 CronSim is written for and being used in
 [Healthchecks](https://github.com/healthchecks/healthchecks/)
@@ -28,29 +50,63 @@
 from cronsim import CronSim
 
 it = CronSim("0 0 * 2 MON#5", datetime.now())
 for x in range(0, 10):
     print(next(it))
 ```
 
-Outputs:
+Produces:
 
 ```
 2044-02-29 00:00:00
 2072-02-29 00:00:00
 2112-02-29 00:00:00
 2140-02-29 00:00:00
 2168-02-29 00:00:00
 2196-02-29 00:00:00
 2208-02-29 00:00:00
 2236-02-29 00:00:00
 2264-02-29 00:00:00
 2292-02-29 00:00:00
 ```
 
+If CronSim receives an invalid cron expression, it raises `cronsim.CronSimError`:
+
+```python
+from datetime import datetime
+from cronsim import CronSim
+
+CronSim("123 * * * *", datetime.now())
+```
+
+Produces:
+
+```
+cronsim.cronsim.CronSimError: Bad minute
+```
+
+If CronSim cannot find a matching datetime in the next 50 years from the start
+date or from the previous match, it stops iteration by raising `StopIteration`:
+
+```python
+from datetime import datetime
+from cronsim import CronSim
+
+# Every minute of 1st and 21st of month,
+# if it is also the *last Monday* of the month:
+it = CronSim("* * */20 * 1L", datetime.now())
+print(next(it))
+```
+
+Produces:
+
+```
+StopIteration
+```
+
 ## CronSim Works With zoneinfo
 
 CronSim starting from version 2.0 is designed to work with timezones provided by
 the zoneinfo module.
 
 A previous version, CronSim 1.0, was designed for pytz and relied on its
 following non-standard features:
@@ -87,32 +143,39 @@
 ```
 
 See test cases in `test_cronsim.py`, `TestDstTransitions` class
 for examples of this special handling.
 
 ## Cron Expression Feature Matrix
 
-| Feature                              | Debian | croniter | cronsim |
-| ------------------------------------ | :----: | :------: | :-----: |
-| Seconds in the 6th field             | No     | Yes      | No      |
-| "L" as the day-of-month              | No     | Yes      | Yes     |
-| "L" in the day-of-week field         | No     | No       | Yes     |
-| Nth weekday of month                 | No     | Yes      | Yes     |
+| Feature                              | Debian | Quartz | croniter | cronsim |
+| ------------------------------------ | :----: | :----: | :------: | :-----: |
+| Seconds in the 6th field             | No     | Yes    | Yes      | No      |
+| "L" as the day-of-month              | No     | Yes    | Yes      | Yes     |
+| "LW" as the day-of-month             | No     | Yes    | No       | Yes     |
+| "L" in the day-of-week field         | No     | Yes    | No       | Yes     |
+| Nth weekday of month                 | No     | Yes    | Yes      | Yes     |
 
 
 **Seconds in the 6th field**: an optional sixth field specifying seconds.
-Supports the same syntax features as the minutes field.
+Supports the same syntax features as the minutes field. Quartz Scheduler
+expects seconds in the first field, croniter expects seconds in the last field.
 
-Example: `* * * * * */15` (every 15 seconds).
+Quartz example: `*/15 * * * * *` (every 15 seconds).
 
 **"L" as the day-of-month**: support for the "L" special character in the
 day-of-month field. Interpreted as "the last day of the month".
 
 Example: `0 0 L * *` (at the midnight of the last day of every month).
 
+**"LW" as the day-of-month**: support for the "LW" special value in the
+day-of-month field. Interpreted as "the last weekday (Mon-Fri) of the month".
+
+Example: `0 0 LW * *` (at the midnight of the last weekday of every month).
+
 **"L" in the day-of-week field**: support for the "{weekday}L" syntax.
 For example, "5L" means "the last Friday of the month".
 
 Example: `0 0 * * 6L` (at the midnight of the last Saturday of every month).
 
 **Nth weekday of month**: support for "{weekday}#{nth}" syntax.
 For example, "MON#1" means "first Monday of the month", "MON#2" means "second Monday
@@ -138,8 +201,9 @@
 ```
 Every fifth minute from 09:00 through 17:59
 ```
 
 The text descriptions are available in English only. The text descriptions
 use the 24-hour time format ("23:00" instead of "11:00 PM").
 
-For examples of generated descriptions see `tests/test_explain.py`.
+For examples of generated descriptions see `tests/test_explain.py`.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cronsim-2.4.1/cronsim/cronsim.py` & `cronsim-2.5/cronsim/cronsim.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         if "/" in s:
             term, step_str = s.split("/", maxsplit=1)
             step = self._int(step_str)
             if step == 0:
                 raise CronSimError(self.msg())
 
             items = self.parse(term)
-            if items == {CronSim.LAST}:
+            if items == {CronSim.LAST} or items == {CronSim.LAST_WEEKDAY}:
                 return items
 
             if len(items) == 1:
                 start = items.pop()
                 assert isinstance(start, int)
                 end = max(RANGES[self])
                 tail = range(start, end + 1)
@@ -114,26 +114,43 @@
             end = self.int(end_str)
 
             if end < start:
                 raise CronSimError(self.msg())
 
             return set(range(start, end + 1))
 
+        if self == Field.DAY and s == "LW":
+            return {CronSim.LAST_WEEKDAY}
+
         if self == Field.DAY and s == "L":
             return {CronSim.LAST}
 
         return {self.int(s)}
 
 
 def is_imaginary(dt: datetime) -> bool:
     return dt != dt.astimezone(UTC).astimezone(dt.tzinfo)
 
 
+def last_weekday(year: int, month: int) -> int:
+    """Return the date of the last weekday of a given year and month."""
+    first_dow, last_date = calendar.monthrange(year, month)
+    last_dow = (first_dow + last_date - 1) % 7
+
+    if last_dow == 6:
+        return last_date - 2
+    elif last_dow == 5:
+        return last_date - 1
+
+    return last_date
+
+
 class CronSim(object):
     LAST = -1000
+    LAST_WEEKDAY = -1001
 
     def __init__(self, expr: str, dt: datetime):
         self.dt = dt.replace(second=0, microsecond=0)
 
         self.parts = expr.upper().split()
         if len(self.parts) != 5:
             raise CronSimError("Wrong number of fields")
@@ -222,15 +239,24 @@
         return True
 
     def match_dom(self, d: date) -> bool:
         """Return True is day-of-month matches."""
         if d.day in self.days:
             return True
 
-        if self.LAST in self.days:
+        # Optimization: there are no months with fewer than 28 days.
+        # If 28th is Sunday, the last weekday of the month is the 26th.
+        # Any date before 26th cannot be the the last weekday of the month.
+        if self.LAST_WEEKDAY in self.days and d.day >= 26:
+            if d.day == last_weekday(d.year, d.month):
+                return True
+
+        # Optimization: there are no months with fewer than 28 days,
+        # so any date before 28th cannot be the the last day of the month
+        if self.LAST in self.days and d.day >= 28:
             _, last = calendar.monthrange(d.year, d.month)
             if d.day == last:
                 return True
 
         return False
 
     def match_dow(self, d: date) -> bool:
```

### Comparing `cronsim-2.4.1/cronsim/explain.py` & `cronsim-2.5/cronsim/explain.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         return f"{l[0]} and {l[1]}"
 
     head = ", ".join(l[:-1])
     return f"{head}, and {l[-1]}"
 
 
 ORDINALS = {
+    -1: "last",
     1: "first",
     2: "second",
     3: "third",
     4: "fourth",
     5: "fifth",
     6: "sixth",
     7: "seventh",
@@ -117,14 +118,16 @@
                 v = self._int(term)
                 yield Sequence(start=v, stop=v, nth=int(nth))
             elif "/" in term:
                 term, step_str = term.split("/")
                 step = int(step_str)
                 if term == "*":
                     yield Sequence(step=step)
+                elif term == "LW":
+                    yield Sequence(start=-2, stop=-2, nth=-1)
                 elif term == "L":
                     yield Sequence(start=-1, stop=-1, nth=-1)
                 else:
                     if "-" in term:
                         start_str, stop_str = term.split("-")
                         start, stop = self._int(start_str), self._int(stop_str)
                     else:
@@ -142,14 +145,16 @@
                     # treat a 2-long sequence as two single values:
                     yield Sequence(start=start, stop=start)
                     yield Sequence(start=stop, stop=stop)
                 elif start <= self.min_value and stop >= self.max_value:
                     yield Sequence()
                 else:
                     yield Sequence(start=start, stop=stop)
+            elif term == "LW":
+                yield Sequence(start=-2, stop=-2, nth=-1)
             elif term == "L":
                 yield Sequence(start=-1, stop=-1, nth=-1)
             else:
                 v = self._int(term)
                 yield Sequence(start=v, stop=v)
 
     def _int(self, value: str) -> int:
@@ -309,34 +314,43 @@
 
         >>> format_single(2)
         'the 2nd day of month'
         """
         return f"the {ordinal(value)} day of month"
 
     def format_nth(self, value: int, nth: int) -> str:
-        """Format the last day of month (L) value.
+        """Format the L and LW values.
 
         >>> format_nth(-1)
         'the last day of the month'
+        >>> format_nth(-2)
+        'the last weekday of the month'
         """
-        if nth == -1:
+        if nth == -1 and value == -1:
             return "the last day of the month"
+        if nth == -1 and value == -2:
+            return "the last weekday of the month"
         return super().format_nth(value, nth)
 
     def format(self) -> str:
         """Format the day field.
 
         This method adds special handling for the case when
         all values are single values. For example, instead of
         "the 1st day of month, the 3rd day of month, and the 5th day of month"
         it produces "the 1st, 3rd, and 5th day of month".
+
+        We cannot apply this optimization if the single values contain "-2"
+        (the special value for "last weekday of the month").
         """
         if self.all_singles and len(self.parsed) > 1:
-            labels = [f"the {ordinal(v)}" for v in self.singles()]
-            return f"{join(labels)} day of month"
+            singles = self.singles()
+            if -2 not in singles:
+                labels = [f"the {ordinal(v)}" for v in singles]
+                return f"{join(labels)} day of month"
         return super().format()
 
     def __str__(self) -> str:
         """Return a human-friendly representation of the day of month field.
 
         This method unconditionally adds the 'on' preposition.
         """
@@ -492,27 +506,32 @@
 
     def optimized_dates(self) -> str | None:
         """Apply formatting optimizations for specific dates.
 
         If day-of-month is L, format it as
         "on the last day of <month description here>".
 
+        If day-of-month is LW, format it as
+        "on the last weekday of <month description here>".
+
         If month and day-of-month each have a single value
         (for example, month 2 and day-of-month 1), format them as
         "February 1st".
 
         If day-of-month has a single value (for example, 2),
         format it as "on the 2nd day of <month description here>".
 
         If no special optimizations apply, return None.
         """
 
         if self.dow.star:
             if self.day.single_value == -1:
                 return f"on the last day of {self.month.format()}"
+            if self.day.single_value == -2:
+                return f"on the last weekday of {self.month.format()}"
             if self.month.single_value and self.day.single_value:
                 return f"on {self.month.format()} {self.day.single_value}"
             if self.day.single_value:
                 date_ord = ordinal(self.day.single_value)
                 return f"on the {date_ord} day of {self.month.format()}"
 
         return None
```

### Comparing `cronsim-2.4.1/cronsim.egg-info/PKG-INFO` & `cronsim-2.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: cronsim
-Version: 2.4.1
-Summary: Cron expression parser and evaluator
-Home-page: https://github.com/cuu508/cronsim
-Author: Pēteris Caune
-Author-email: cuu508@gmail.com
-License: BSD
-Project-URL: Changelog, https://github.com/cuu508/cronsim/blob/main/CHANGELOG.md
-Keywords: cron,cronjob,crontab,schedule
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >= 3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CronSim
 
 [![Tests](https://github.com/cuu508/cronsim/actions/workflows/pytest.yml/badge.svg)](https://github.com/cuu508/cronsim/actions/workflows/pytest.yml)
 
 Cron Sim(ulator), a cron expression parser and evaluator. Works with Python 3.8+.
 CronSim is written for and being used in
 [Healthchecks](https://github.com/healthchecks/healthchecks/)
@@ -50,29 +28,63 @@
 from cronsim import CronSim
 
 it = CronSim("0 0 * 2 MON#5", datetime.now())
 for x in range(0, 10):
     print(next(it))
 ```
 
-Outputs:
+Produces:
 
 ```
 2044-02-29 00:00:00
 2072-02-29 00:00:00
 2112-02-29 00:00:00
 2140-02-29 00:00:00
 2168-02-29 00:00:00
 2196-02-29 00:00:00
 2208-02-29 00:00:00
 2236-02-29 00:00:00
 2264-02-29 00:00:00
 2292-02-29 00:00:00
 ```
 
+If CronSim receives an invalid cron expression, it raises `cronsim.CronSimError`:
+
+```python
+from datetime import datetime
+from cronsim import CronSim
+
+CronSim("123 * * * *", datetime.now())
+```
+
+Produces:
+
+```
+cronsim.cronsim.CronSimError: Bad minute
+```
+
+If CronSim cannot find a matching datetime in the next 50 years from the start
+date or from the previous match, it stops iteration by raising `StopIteration`:
+
+```python
+from datetime import datetime
+from cronsim import CronSim
+
+# Every minute of 1st and 21st of month,
+# if it is also the *last Monday* of the month:
+it = CronSim("* * */20 * 1L", datetime.now())
+print(next(it))
+```
+
+Produces:
+
+```
+StopIteration
+```
+
 ## CronSim Works With zoneinfo
 
 CronSim starting from version 2.0 is designed to work with timezones provided by
 the zoneinfo module.
 
 A previous version, CronSim 1.0, was designed for pytz and relied on its
 following non-standard features:
@@ -109,32 +121,39 @@
 ```
 
 See test cases in `test_cronsim.py`, `TestDstTransitions` class
 for examples of this special handling.
 
 ## Cron Expression Feature Matrix
 
-| Feature                              | Debian | croniter | cronsim |
-| ------------------------------------ | :----: | :------: | :-----: |
-| Seconds in the 6th field             | No     | Yes      | No      |
-| "L" as the day-of-month              | No     | Yes      | Yes     |
-| "L" in the day-of-week field         | No     | No       | Yes     |
-| Nth weekday of month                 | No     | Yes      | Yes     |
+| Feature                              | Debian | Quartz | croniter | cronsim |
+| ------------------------------------ | :----: | :----: | :------: | :-----: |
+| Seconds in the 6th field             | No     | Yes    | Yes      | No      |
+| "L" as the day-of-month              | No     | Yes    | Yes      | Yes     |
+| "LW" as the day-of-month             | No     | Yes    | No       | Yes     |
+| "L" in the day-of-week field         | No     | Yes    | No       | Yes     |
+| Nth weekday of month                 | No     | Yes    | Yes      | Yes     |
 
 
 **Seconds in the 6th field**: an optional sixth field specifying seconds.
-Supports the same syntax features as the minutes field.
+Supports the same syntax features as the minutes field. Quartz Scheduler
+expects seconds in the first field, croniter expects seconds in the last field.
 
-Example: `* * * * * */15` (every 15 seconds).
+Quartz example: `*/15 * * * * *` (every 15 seconds).
 
 **"L" as the day-of-month**: support for the "L" special character in the
 day-of-month field. Interpreted as "the last day of the month".
 
 Example: `0 0 L * *` (at the midnight of the last day of every month).
 
+**"LW" as the day-of-month**: support for the "LW" special value in the
+day-of-month field. Interpreted as "the last weekday (Mon-Fri) of the month".
+
+Example: `0 0 LW * *` (at the midnight of the last weekday of every month).
+
 **"L" in the day-of-week field**: support for the "{weekday}L" syntax.
 For example, "5L" means "the last Friday of the month".
 
 Example: `0 0 * * 6L` (at the midnight of the last Saturday of every month).
 
 **Nth weekday of month**: support for "{weekday}#{nth}" syntax.
 For example, "MON#1" means "first Monday of the month", "MON#2" means "second Monday
@@ -160,9 +179,8 @@
 ```
 Every fifth minute from 09:00 through 17:59
 ```
 
 The text descriptions are available in English only. The text descriptions
 use the 24-hour time format ("23:00" instead of "11:00 PM").
 
-For examples of generated descriptions see `tests/test_explain.py`.
-
+For examples of generated descriptions see `tests/test_explain.py`.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cronsim-2.4.1/setup.py` & `cronsim-2.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 from __future__ import annotations
 
 from setuptools import find_packages, setup
 
 setup(
     name="cronsim",
-    version="2.4.1",
+    version="2.5",
     url="https://github.com/cuu508/cronsim",
     license="BSD",
     author="Pēteris Caune",
-    author_email="cuu508@gmail.com",
+    author_email="cuu508@monkeyseemonkeydo.lv",
     description="Cron expression parser and evaluator",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     keywords="cron,cronjob,crontab,schedule",
     packages=find_packages(),
     include_package_data=True,
     platforms="any",
```

