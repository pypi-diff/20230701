# Comparing `tmp/trongrid_extractor-0.3.8.tar.gz` & `tmp/trongrid_extractor-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trongrid_extractor-0.3.8.tar", max compression
+gzip compressed data, was "trongrid_extractor-0.3.9.tar", max compression
```

## Comparing `trongrid_extractor-0.3.8.tar` & `trongrid_extractor-0.3.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1113 2023-06-30 21:32:01.529646 trongrid_extractor-0.3.8/CHANGELOG.md
--rw-r--r--   0        0        0       36 2023-06-27 21:57:40.566976 trongrid_extractor-0.3.8/LICENSE
--rw-r--r--   0        0        0     3788 2023-06-29 06:44:04.355607 trongrid_extractor-0.3.8/README.md
--rw-r--r--   0        0        0      710 2023-06-30 21:32:01.535883 trongrid_extractor-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      459 2023-06-28 08:24:37.997172 trongrid_extractor-0.3.8/trongrid_extractor/__init__.py
--rw-r--r--   0        0        0    10610 2023-06-30 21:31:49.147464 trongrid_extractor-0.3.8/trongrid_extractor/api.py
--rw-r--r--   0        0        0      326 2023-06-29 00:31:04.580384 trongrid_extractor-0.3.8/trongrid_extractor/config.py
--rw-r--r--   0        0        0     1888 2023-06-30 21:31:49.147977 trongrid_extractor-0.3.8/trongrid_extractor/helpers/address_helpers.py
--rw-r--r--   0        0        0     2243 2023-06-28 19:11:14.811112 trongrid_extractor-0.3.8/trongrid_extractor/helpers/argument_parser.py
--rw-r--r--   0        0        0     2194 2023-06-30 02:06:04.627545 trongrid_extractor-0.3.8/trongrid_extractor/helpers/csv_helper.py
--rw-r--r--   0        0        0      196 2023-06-28 02:11:34.501085 trongrid_extractor-0.3.8/trongrid_extractor/helpers/dict_helper.py
--rw-r--r--   0        0        0      311 2023-06-30 21:31:49.148646 trongrid_extractor-0.3.8/trongrid_extractor/helpers/string_constants.py
--rw-r--r--   0        0        0     1431 2023-06-27 21:52:41.750623 trongrid_extractor-0.3.8/trongrid_extractor/helpers/time_helpers.py
--rw-r--r--   0        0        0     3097 2023-06-30 21:31:49.149188 trongrid_extractor-0.3.8/trongrid_extractor/progress_tracker.py
--rw-r--r--   0        0        0     3760 2023-06-30 21:31:49.151159 trongrid_extractor-0.3.8/trongrid_extractor/response.py
--rw-r--r--   0        0        0     4336 2023-06-28 19:40:28.066469 trongrid_extractor-0.3.8/trongrid_extractor/trc20_txn.py
--rw-r--r--   0        0        0     4430 1970-01-01 00:00:00.000000 trongrid_extractor-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1216 2023-07-01 02:48:46.590358 trongrid_extractor-0.3.9/CHANGELOG.md
+-rw-r--r--   0        0        0       36 2023-06-27 21:57:40.566976 trongrid_extractor-0.3.9/LICENSE
+-rw-r--r--   0        0        0     3788 2023-06-29 06:44:04.355607 trongrid_extractor-0.3.9/README.md
+-rw-r--r--   0        0        0      710 2023-07-01 02:48:46.593961 trongrid_extractor-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      459 2023-06-28 08:24:37.997172 trongrid_extractor-0.3.9/trongrid_extractor/__init__.py
+-rw-r--r--   0        0        0    10593 2023-07-01 02:48:05.498975 trongrid_extractor-0.3.9/trongrid_extractor/api.py
+-rw-r--r--   0        0        0      326 2023-06-29 00:31:04.580384 trongrid_extractor-0.3.9/trongrid_extractor/config.py
+-rw-r--r--   0        0        0     1888 2023-07-01 01:36:13.931502 trongrid_extractor-0.3.9/trongrid_extractor/helpers/address_helpers.py
+-rw-r--r--   0        0        0     2243 2023-06-28 19:11:14.811112 trongrid_extractor-0.3.9/trongrid_extractor/helpers/argument_parser.py
+-rw-r--r--   0        0        0     2194 2023-06-30 02:06:04.627545 trongrid_extractor-0.3.9/trongrid_extractor/helpers/csv_helper.py
+-rw-r--r--   0        0        0      196 2023-06-28 02:11:34.501085 trongrid_extractor-0.3.9/trongrid_extractor/helpers/dict_helper.py
+-rw-r--r--   0        0        0      311 2023-06-30 21:31:49.148646 trongrid_extractor-0.3.9/trongrid_extractor/helpers/string_constants.py
+-rw-r--r--   0        0        0     1431 2023-06-27 21:52:41.750623 trongrid_extractor-0.3.9/trongrid_extractor/helpers/time_helpers.py
+-rw-r--r--   0        0        0     3097 2023-06-30 21:31:49.149188 trongrid_extractor-0.3.9/trongrid_extractor/progress_tracker.py
+-rw-r--r--   0        0        0     4436 2023-07-01 02:39:18.865395 trongrid_extractor-0.3.9/trongrid_extractor/response.py
+-rw-r--r--   0        0        0     4336 2023-06-28 19:40:28.066469 trongrid_extractor-0.3.9/trongrid_extractor/trc20_txn.py
+-rw-r--r--   0        0        0     4430 1970-01-01 00:00:00.000000 trongrid_extractor-0.3.9/PKG-INFO
```

### Comparing `trongrid_extractor-0.3.8/CHANGELOG.md` & `trongrid_extractor-0.3.9/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # NEXT RELEASE
 
+### 0.3.9
+* Don't consider small timespan queries failures in need of rescuing if they return 0 rows.
+
 ### 0.3.8
 * Fix buggy handling of false completes
 
 ### 0.3.7
 * Delete output CSV if it already exists
 * Fix bug with resuming from CSV with out of order rows
 * Only do a rescue when it is impossible to load next page
```

### Comparing `trongrid_extractor-0.3.8/README.md` & `trongrid_extractor-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.8/pyproject.toml` & `trongrid_extractor-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trongrid-extractor"
-version = "0.3.8"
+version = "0.3.9"
 description = "Extract transactions from the Trongrid API."
 authors = ["Chain Argos"]
 readme = "README.md"
 packages = [{include = "trongrid_extractor"}]
 homepage = "https://chainargos.com"
 
 include = [
```

### Comparing `trongrid_extractor-0.3.8/trongrid_extractor/api.py` & `trongrid_extractor-0.3.9/trongrid_extractor/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,14 @@
             # Pull the next record
             if response.next_url() is not None:
                 response = Response.get_response(response.next_url())
             elif force_continue_from_rescue:
                 log.info(f"Forcibly continuing so making a request for {params}")
                 response = Response.get_response(contract_url, params)
             else:
-                log.error(f"Unparseable response!")
                 response.pretty_print()
                 raise ValueError("Unparseable response!")
 
             force_continue_from_rescue = False
 
             # Trongrid doesn't like it when you page more than 5 pages of 200 results. When the
             # "next URL" paging fails we go back to filtering by timestamp but move the
@@ -152,14 +151,15 @@
         """
         raise ValueError("This endpoint doesn't really work.")
         contract_url = f"{self.base_uri}contracts/{contract_addr}/transactions"
         params = Api.build_params(extra={'contract_address': contract_addr})
         response = Response.get_response(contract_url, params)
         return response
 
+    # TODO: this might be defunct.
     def _rescue_extraction(self, url: str, params: Dict[str, Union[str, float]], walkback: int) -> List[Trc20Txn]:
         """
         Try a smaller time range; maybe the "next URL" thing will work. The idea here is that the
         'next' URL paging doesn't work very well if you request a large timespan - it only lets
         you retrieve a few pages before barfing. So here we temporarily switch to a much smaller
         time range.
```

### Comparing `trongrid_extractor-0.3.8/trongrid_extractor/helpers/address_helpers.py` & `trongrid_extractor-0.3.9/trongrid_extractor/helpers/address_helpers.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.8/trongrid_extractor/helpers/argument_parser.py` & `trongrid_extractor-0.3.9/trongrid_extractor/helpers/argument_parser.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.8/trongrid_extractor/helpers/csv_helper.py` & `trongrid_extractor-0.3.9/trongrid_extractor/helpers/csv_helper.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.8/trongrid_extractor/helpers/time_helpers.py` & `trongrid_extractor-0.3.9/trongrid_extractor/helpers/time_helpers.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.8/trongrid_extractor/progress_tracker.py` & `trongrid_extractor-0.3.9/trongrid_extractor/progress_tracker.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.8/trongrid_extractor/response.py` & `trongrid_extractor-0.3.9/trongrid_extractor/response.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 from tenacity import after_log, retry, stop_after_attempt, wait_exponential
 
 from trongrid_extractor.config import log
 from trongrid_extractor.helpers.csv_helper import *
 from trongrid_extractor.helpers.string_constants import *
 from trongrid_extractor.helpers.time_helpers import *
 
+# If the distance between min and max_timestamp is less than this don't consider a 0 row
+# result a failure.
+OK_DURATION_FOR_ZERO_TXNS_MS = 10000
 JSON_HEADERS = {'Accept': 'application/json'}
 
 
 @dataclass
 class Response:
     raw_response: requests.models.Response
     params: Dict[str, Any]
@@ -30,24 +33,35 @@
 
     @classmethod
     @retry(wait=wait_exponential(multiplier=1, min=15, max=300), stop=stop_after_attempt(5), after=after_log(log, logging.DEBUG))
     def get_response(cls, url: str, params: Optional[Dict[str, Union[str, int, float]]] = None) -> 'Response':
         """Alternate constructor that calls the API with retries."""
         params = params or {}
 
+        # If an API call yields too many rows to fit in one response a 'next URL' is given and
+        # our requests use that URL without params.
+        is_new_query = MIN_TIMESTAMP in params and MAX_TIMESTAMP in params
+
         # Min/Max timestamps are INCLUSIVE.
-        if MIN_TIMESTAMP in params and MAX_TIMESTAMP in params:
+        if is_new_query:
             msg = f"Requesting records from {ms_to_datetime(params[MIN_TIMESTAMP])} to {ms_to_datetime(params[MAX_TIMESTAMP])}."
             log.info(msg)
 
         log.debug(f"Request URL: {url}\nParams: {params}")
         raw_response = requests.get(url, headers=JSON_HEADERS, params=params)
         response = cls(raw_response, deepcopy(params))
 
         if response.is_false_complete_response():
+            if is_new_query:
+                duration_queried_ms = params[MAX_TIMESTAMP] - params[MIN_TIMESTAMP]
+
+                if duration_queried_ms <= OK_DURATION_FOR_ZERO_TXNS_MS:
+                    log.warning(f"Looks like a bad 'paging complete' response but only {duration_queried_ms}ms in range.")
+                    return response
+
             msg = f"False positive reponse! {response.response}"
             log.error(msg)
             response.pretty_print()
             log.warning(dump.dump_all(response.raw_response).decode('utf-8'))
             raise ValueError(msg)
 
         return response
```

### Comparing `trongrid_extractor-0.3.8/trongrid_extractor/trc20_txn.py` & `trongrid_extractor-0.3.9/trongrid_extractor/trc20_txn.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.8/PKG-INFO` & `trongrid_extractor-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trongrid-extractor
-Version: 0.3.8
+Version: 0.3.9
 Summary: Extract transactions from the Trongrid API.
 Home-page: https://chainargos.com
 Author: Chain Argos
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

