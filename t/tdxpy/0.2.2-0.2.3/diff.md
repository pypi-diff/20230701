# Comparing `tmp/tdxpy-0.2.2.tar.gz` & `tmp/tdxpy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdxpy-0.2.2.tar", max compression
+gzip compressed data, was "tdxpy-0.2.3.tar", max compression
```

## Comparing `tdxpy-0.2.2.tar` & `tdxpy-0.2.3.tar`

### file list

```diff
@@ -1,58 +1,57 @@
--rw-r--r--   0        0        0     1064 2023-05-11 05:15:06.906347 tdxpy-0.2.2/LICENSE
--rw-r--r--   0        0        0     1289 2023-05-11 05:15:33.958134 tdxpy-0.2.2/README.md
--rw-r--r--   0        0        0     1368 2023-06-30 04:27:37.138097 tdxpy-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       63 2023-06-30 04:27:37.138097 tdxpy-0.2.2/tdxpy/__init__.py
--rw-r--r--   0        0        0     9315 2023-06-30 04:24:13.884279 tdxpy-0.2.2/tdxpy/base_socket_client.py
--rw-r--r--   0        0        0     6449 2023-06-30 04:24:13.884279 tdxpy-0.2.2/tdxpy/constants.py
--rw-r--r--   0        0        0       48 2023-05-11 05:15:06.910347 tdxpy-0.2.2/tdxpy/crawler/__init__.py
--rw-r--r--   0        0        0     3619 2023-06-30 04:24:13.884279 tdxpy-0.2.2/tdxpy/crawler/base_crawler.py
--rw-r--r--   0        0        0     6030 2023-06-30 04:24:13.884279 tdxpy-0.2.2/tdxpy/crawler/history_financial_crawler.py
--rw-r--r--   0        0        0      394 2023-06-30 04:24:13.884279 tdxpy-0.2.2/tdxpy/exceptions.py
--rw-r--r--   0        0        0     4910 2023-05-11 05:15:06.910347 tdxpy-0.2.2/tdxpy/exhq.py
--rw-r--r--   0        0        0     1391 2023-06-30 04:24:13.884279 tdxpy-0.2.2/tdxpy/heartbeat.py
--rw-r--r--   0        0        0     5941 2023-06-30 04:24:13.884279 tdxpy-0.2.2/tdxpy/helper.py
--rw-r--r--   0        0        0    11730 2023-06-30 04:24:13.884279 tdxpy-0.2.2/tdxpy/hq.py
--rw-r--r--   0        0        0      320 2023-06-30 04:24:13.884279 tdxpy-0.2.2/tdxpy/logger.py
--rw-r--r--   0        0        0        0 2023-05-11 05:15:06.910347 tdxpy-0.2.2/tdxpy/parser/__init__.py
--rw-r--r--   0        0        0     4746 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/base.py
--rw-r--r--   0        0        0        0 2023-05-11 05:15:06.910347 tdxpy-0.2.2/tdxpy/parser/ext/__init__.py
--rw-r--r--   0        0        0     2637 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_history_instrument_bars_range.py
--rw-r--r--   0        0        0     1223 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_history_minute_time_data.py
--rw-r--r--   0        0        0     4170 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_history_transaction_data.py
--rw-r--r--   0        0        0     2130 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_instrument_bars.py
--rw-r--r--   0        0        0      345 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_instrument_count.py
--rw-r--r--   0        0        0     1350 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_instrument_info.py
--rw-r--r--   0        0        0     2854 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_instrument_quote.py
--rw-r--r--   0        0        0     6336 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_instrument_quote_list.py
--rw-r--r--   0        0        0     1307 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_markets.py
--rw-r--r--   0        0        0     1332 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_minute_time_data.py
--rw-r--r--   0        0        0     4078 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/ext/ex_get_transaction_data.py
--rw-r--r--   0        0        0      396 2023-05-11 05:15:06.910347 tdxpy-0.2.2/tdxpy/parser/raw_parser.py
--rw-r--r--   0        0        0     1272 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/setup_commands.py
--rw-r--r--   0        0        0        0 2023-05-11 05:15:06.910347 tdxpy-0.2.2/tdxpy/parser/std/__init__.py
--rw-r--r--   0        0        0     2308 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_block_info.py
--rw-r--r--   0        0        0     1549 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_company_info_category.py
--rw-r--r--   0        0        0     1082 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_company_info_content.py
--rw-r--r--   0        0        0     3999 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_finance_info.py
--rw-r--r--   0        0        0     1767 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_history_minute_time_data.py
--rw-r--r--   0        0        0     1849 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_history_transaction_data.py
--rw-r--r--   0        0        0     3243 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_index_bars.py
--rw-r--r--   0        0        0     1515 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_minute_time_data.py
--rw-r--r--   0        0        0      969 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_report_file.py
--rw-r--r--   0        0        0     3024 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_security_bars.py
--rw-r--r--   0        0        0      570 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_security_count.py
--rw-r--r--   0        0        0     1444 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_security_list.py
--rw-r--r--   0        0        0     7845 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_security_quotes.py
--rw-r--r--   0        0        0     1689 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_transaction_data.py
--rw-r--r--   0        0        0     3915 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/parser/std/get_xdxr_info.py
--rw-r--r--   0        0        0      744 2023-05-11 05:15:06.914347 tdxpy-0.2.2/tdxpy/reader/__init__.py
--rw-r--r--   0        0        0     1293 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/reader/base_reader.py
--rw-r--r--   0        0        0     4746 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/reader/block_reader.py
--rw-r--r--   0        0        0     5698 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/reader/daily_bar_reader.py
--rw-r--r--   0        0        0     1713 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/reader/exhq_daily_bar_reader.py
--rw-r--r--   0        0        0      937 2023-05-11 05:15:06.914347 tdxpy-0.2.2/tdxpy/reader/history_financial_reader.py
--rw-r--r--   0        0        0     2587 2023-05-11 05:15:06.914347 tdxpy-0.2.2/tdxpy/reader/lc_min_bar_reader.py
--rw-r--r--   0        0        0     3052 2023-05-11 05:15:06.914347 tdxpy-0.2.2/tdxpy/reader/min_bar_reader.py
--rw-r--r--   0        0        0       46 2023-06-30 04:24:13.888279 tdxpy-0.2.2/tdxpy/version.py
--rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 tdxpy-0.2.2/setup.py
--rw-r--r--   0        0        0     1795 1970-01-01 00:00:00.000000 tdxpy-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-12 13:36:58.030340 tdxpy-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1289 2023-06-12 13:37:42.309435 tdxpy-0.2.3/README.md
+-rw-r--r--   0        0        0     1368 2023-07-01 01:41:54.795959 tdxpy-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       63 2023-07-01 01:41:54.789435 tdxpy-0.2.3/tdxpy/__init__.py
+-rw-r--r--   0        0        0     9315 2023-06-12 13:37:42.310173 tdxpy-0.2.3/tdxpy/base_socket_client.py
+-rw-r--r--   0        0        0     6449 2023-06-12 13:37:42.310312 tdxpy-0.2.3/tdxpy/constants.py
+-rw-r--r--   0        0        0       48 2023-06-12 13:36:58.032358 tdxpy-0.2.3/tdxpy/crawler/__init__.py
+-rw-r--r--   0        0        0     3619 2023-06-12 13:37:42.310450 tdxpy-0.2.3/tdxpy/crawler/base_crawler.py
+-rw-r--r--   0        0        0     6030 2023-06-12 13:37:42.310578 tdxpy-0.2.3/tdxpy/crawler/history_financial_crawler.py
+-rw-r--r--   0        0        0      394 2023-06-12 13:37:42.310685 tdxpy-0.2.3/tdxpy/exceptions.py
+-rw-r--r--   0        0        0     4910 2023-06-12 13:36:58.032745 tdxpy-0.2.3/tdxpy/exhq.py
+-rw-r--r--   0        0        0     1391 2023-06-12 13:37:42.310809 tdxpy-0.2.3/tdxpy/heartbeat.py
+-rw-r--r--   0        0        0     5694 2023-07-01 01:38:42.801497 tdxpy-0.2.3/tdxpy/helper.py
+-rw-r--r--   0        0        0    11730 2023-06-12 13:37:42.311027 tdxpy-0.2.3/tdxpy/hq.py
+-rw-r--r--   0        0        0      320 2023-06-12 13:37:42.311139 tdxpy-0.2.3/tdxpy/logger.py
+-rw-r--r--   0        0        0        0 2023-06-12 13:36:58.033141 tdxpy-0.2.3/tdxpy/parser/__init__.py
+-rw-r--r--   0        0        0     4746 2023-06-12 13:37:42.311253 tdxpy-0.2.3/tdxpy/parser/base.py
+-rw-r--r--   0        0        0        0 2023-06-12 13:36:58.033289 tdxpy-0.2.3/tdxpy/parser/ext/__init__.py
+-rw-r--r--   0        0        0     2637 2023-06-12 13:37:42.311381 tdxpy-0.2.3/tdxpy/parser/ext/ex_get_history_instrument_bars_range.py
+-rw-r--r--   0        0        0     1223 2023-06-12 13:37:42.311510 tdxpy-0.2.3/tdxpy/parser/ext/ex_get_history_minute_time_data.py
+-rw-r--r--   0        0        0     4170 2023-06-12 13:37:42.311621 tdxpy-0.2.3/tdxpy/parser/ext/ex_get_history_transaction_data.py
+-rw-r--r--   0        0        0     2130 2023-06-12 13:37:42.311738 tdxpy-0.2.3/tdxpy/parser/ext/ex_get_instrument_bars.py
+-rw-r--r--   0        0        0      345 2023-06-12 13:37:42.311847 tdxpy-0.2.3/tdxpy/parser/ext/ex_get_instrument_count.py
+-rw-r--r--   0        0        0     1350 2023-06-12 13:37:42.311969 tdxpy-0.2.3/tdxpy/parser/ext/ex_get_instrument_info.py
+-rw-r--r--   0        0        0     2854 2023-06-12 13:37:42.312100 tdxpy-0.2.3/tdxpy/parser/ext/ex_get_instrument_quote.py
+-rw-r--r--   0        0        0     6336 2023-06-12 13:37:42.312263 tdxpy-0.2.3/tdxpy/parser/ext/ex_get_instrument_quote_list.py
+-rw-r--r--   0        0        0     1307 2023-06-12 13:37:42.312393 tdxpy-0.2.3/tdxpy/parser/ext/ex_get_markets.py
+-rw-r--r--   0        0        0     1332 2023-06-12 13:37:42.312719 tdxpy-0.2.3/tdxpy/parser/ext/ex_get_minute_time_data.py
+-rw-r--r--   0        0        0     4078 2023-06-12 13:37:42.312835 tdxpy-0.2.3/tdxpy/parser/ext/ex_get_transaction_data.py
+-rw-r--r--   0        0        0      396 2023-06-12 13:36:58.034300 tdxpy-0.2.3/tdxpy/parser/raw_parser.py
+-rw-r--r--   0        0        0     1272 2023-06-12 13:37:42.312943 tdxpy-0.2.3/tdxpy/parser/setup_commands.py
+-rw-r--r--   0        0        0        0 2023-06-12 13:36:58.034424 tdxpy-0.2.3/tdxpy/parser/std/__init__.py
+-rw-r--r--   0        0        0     2308 2023-06-12 13:37:42.313066 tdxpy-0.2.3/tdxpy/parser/std/get_block_info.py
+-rw-r--r--   0        0        0     1549 2023-06-12 13:37:42.313175 tdxpy-0.2.3/tdxpy/parser/std/get_company_info_category.py
+-rw-r--r--   0        0        0     1082 2023-06-12 13:37:42.313299 tdxpy-0.2.3/tdxpy/parser/std/get_company_info_content.py
+-rw-r--r--   0        0        0     3999 2023-06-12 13:37:42.313432 tdxpy-0.2.3/tdxpy/parser/std/get_finance_info.py
+-rw-r--r--   0        0        0     1703 2023-07-01 01:38:42.801671 tdxpy-0.2.3/tdxpy/parser/std/get_history_minute_time_data.py
+-rw-r--r--   0        0        0     1849 2023-06-12 13:37:42.313669 tdxpy-0.2.3/tdxpy/parser/std/get_history_transaction_data.py
+-rw-r--r--   0        0        0     3243 2023-06-12 13:37:42.313791 tdxpy-0.2.3/tdxpy/parser/std/get_index_bars.py
+-rw-r--r--   0        0        0     1317 2023-07-01 01:38:42.801824 tdxpy-0.2.3/tdxpy/parser/std/get_minute_time_data.py
+-rw-r--r--   0        0        0      969 2023-06-12 13:37:42.314023 tdxpy-0.2.3/tdxpy/parser/std/get_report_file.py
+-rw-r--r--   0        0        0     3024 2023-06-12 13:37:42.314137 tdxpy-0.2.3/tdxpy/parser/std/get_security_bars.py
+-rw-r--r--   0        0        0      570 2023-06-12 13:37:42.314256 tdxpy-0.2.3/tdxpy/parser/std/get_security_count.py
+-rw-r--r--   0        0        0     1444 2023-06-12 13:37:42.314401 tdxpy-0.2.3/tdxpy/parser/std/get_security_list.py
+-rw-r--r--   0        0        0     7842 2023-07-01 01:40:57.119902 tdxpy-0.2.3/tdxpy/parser/std/get_security_quotes.py
+-rw-r--r--   0        0        0     1689 2023-06-12 13:37:42.314626 tdxpy-0.2.3/tdxpy/parser/std/get_transaction_data.py
+-rw-r--r--   0        0        0     3915 2023-06-12 13:37:42.314753 tdxpy-0.2.3/tdxpy/parser/std/get_xdxr_info.py
+-rw-r--r--   0        0        0      744 2023-06-12 13:36:58.035848 tdxpy-0.2.3/tdxpy/reader/__init__.py
+-rw-r--r--   0        0        0     1293 2023-06-12 13:37:42.314871 tdxpy-0.2.3/tdxpy/reader/base_reader.py
+-rw-r--r--   0        0        0     4746 2023-06-12 13:37:42.315006 tdxpy-0.2.3/tdxpy/reader/block_reader.py
+-rw-r--r--   0        0        0     5698 2023-06-12 13:37:42.315148 tdxpy-0.2.3/tdxpy/reader/daily_bar_reader.py
+-rw-r--r--   0        0        0     1713 2023-06-12 13:37:42.315268 tdxpy-0.2.3/tdxpy/reader/exhq_daily_bar_reader.py
+-rw-r--r--   0        0        0      937 2023-06-12 13:36:58.036256 tdxpy-0.2.3/tdxpy/reader/history_financial_reader.py
+-rw-r--r--   0        0        0     2587 2023-06-12 13:36:58.036356 tdxpy-0.2.3/tdxpy/reader/lc_min_bar_reader.py
+-rw-r--r--   0        0        0     3052 2023-06-12 13:36:58.036421 tdxpy-0.2.3/tdxpy/reader/min_bar_reader.py
+-rw-r--r--   0        0        0       46 2023-06-12 13:37:42.315342 tdxpy-0.2.3/tdxpy/version.py
+-rw-r--r--   0        0        0     1795 1970-01-01 00:00:00.000000 tdxpy-0.2.3/PKG-INFO
```

### Comparing `tdxpy-0.2.2/LICENSE` & `tdxpy-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/README.md` & `tdxpy-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/pyproject.toml` & `tdxpy-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tdxpy"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["bopo <ibopo@126.com>"]
 readme = "README.md"
 packages = [{ include = "tdxpy" }]
 include = ["CHANGELOG.md"]
```

### Comparing `tdxpy-0.2.2/tdxpy/base_socket_client.py` & `tdxpy-0.2.3/tdxpy/base_socket_client.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/constants.py` & `tdxpy-0.2.3/tdxpy/constants.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/crawler/base_crawler.py` & `tdxpy-0.2.3/tdxpy/crawler/base_crawler.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/crawler/history_financial_crawler.py` & `tdxpy-0.2.3/tdxpy/crawler/history_financial_crawler.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/exhq.py` & `tdxpy-0.2.3/tdxpy/exhq.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/heartbeat.py` & `tdxpy-0.2.3/tdxpy/heartbeat.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/helper.py` & `tdxpy-0.2.3/tdxpy/helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -167,18 +167,14 @@
 
 
 # TODO 增加 get_coefficient 函数
 def get_security_coefficient(market=None, code=None):
     try:
         security_type = get_security_type(market=market, code=code)
         coefficient = SECURITY_COEFFICIENT[security_type]
-
-        logger.warning(f'security_type => {security_type}')
-        logger.warning(f'coefficient => {coefficient}')
-
         return coefficient[0]
     except NotImplementedError:
         logger.error('NotImplementedError')
         return 0.01
 
 
 def get_security_type(market, code):
@@ -190,18 +186,14 @@
     :return:
     """
 
     # code = Path(code).stem
     code = str(code)
     code_head = str(code)[:2]
 
-    logger.warning(f'market => {market}')
-    logger.warning(f'code => {code}')
-    logger.warning(f'code_head => {code_head}')
-
     if market in ["SZ", "sz", 0]:
         if code_head in ["00", "30"]:
             return "SZ_A_STOCK"
 
         if code_head in ["20"]:
             return "SZ_B_STOCK"
```

### Comparing `tdxpy-0.2.2/tdxpy/hq.py` & `tdxpy-0.2.3/tdxpy/hq.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/base.py` & `tdxpy-0.2.3/tdxpy/parser/base.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/ext/ex_get_history_instrument_bars_range.py` & `tdxpy-0.2.3/tdxpy/parser/ext/ex_get_history_instrument_bars_range.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/ext/ex_get_history_minute_time_data.py` & `tdxpy-0.2.3/tdxpy/parser/ext/ex_get_history_minute_time_data.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/ext/ex_get_history_transaction_data.py` & `tdxpy-0.2.3/tdxpy/parser/ext/ex_get_history_transaction_data.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/ext/ex_get_instrument_bars.py` & `tdxpy-0.2.3/tdxpy/parser/ext/ex_get_instrument_bars.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/ext/ex_get_instrument_info.py` & `tdxpy-0.2.3/tdxpy/parser/ext/ex_get_instrument_info.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/ext/ex_get_instrument_quote.py` & `tdxpy-0.2.3/tdxpy/parser/ext/ex_get_instrument_quote.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/ext/ex_get_instrument_quote_list.py` & `tdxpy-0.2.3/tdxpy/parser/ext/ex_get_instrument_quote_list.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/ext/ex_get_markets.py` & `tdxpy-0.2.3/tdxpy/parser/ext/ex_get_markets.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/ext/ex_get_minute_time_data.py` & `tdxpy-0.2.3/tdxpy/parser/ext/ex_get_minute_time_data.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/ext/ex_get_transaction_data.py` & `tdxpy-0.2.3/tdxpy/parser/ext/ex_get_transaction_data.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/setup_commands.py` & `tdxpy-0.2.3/tdxpy/parser/setup_commands.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/std/get_block_info.py` & `tdxpy-0.2.3/tdxpy/parser/std/get_block_info.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/std/get_company_info_category.py` & `tdxpy-0.2.3/tdxpy/parser/std/get_company_info_category.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/std/get_company_info_content.py` & `tdxpy-0.2.3/tdxpy/parser/std/get_company_info_content.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/std/get_finance_info.py` & `tdxpy-0.2.3/tdxpy/parser/std/get_finance_info.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/std/get_history_minute_time_data.py` & `tdxpy-0.2.3/tdxpy/parser/std/get_history_minute_time_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,14 @@
         设置参数
         :param market: 0/1 股票市场
         :param code: '000001' 股票代码
         :param date: 20161201  类似这样的整型
         :return:
         """
         self.coefficient = get_security_coefficient(market=market, code=code)
-        logger.warning(f'self.coefficient=>{self.coefficient}')
 
         if (type(date) is str) or (type(date) is bytes):
             date = int(date)
 
         if type(code) is str:
             code = code.encode("utf-8")
```

### Comparing `tdxpy-0.2.2/tdxpy/parser/std/get_history_transaction_data.py` & `tdxpy-0.2.3/tdxpy/parser/std/get_history_transaction_data.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/std/get_index_bars.py` & `tdxpy-0.2.3/tdxpy/parser/std/get_index_bars.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/std/get_minute_time_data.py` & `tdxpy-0.2.3/tdxpy/parser/std/get_minute_time_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # cython: language_level=3
 import struct
 from collections import OrderedDict
 
 from tdxpy.helper import get_price, get_security_coefficient
-from tdxpy.logger import logger
 from tdxpy.parser.base import BaseParser
 
 
 class GetMinuteTimeData(BaseParser):
 
     def __init__(self, client, lock=None):
         super().__init__(client, lock)
@@ -24,16 +23,14 @@
 
         pkg = bytearray.fromhex("0c 1b 08 00 01 01 0e 00 0e 00 1d 05")
         pkg.extend(struct.pack("<H6sI", market, code, 0))
 
         self.send_pkg = pkg
         self.coefficient = get_security_coefficient(market=market, code=code)
 
-        logger.warning(f'self.coefficient=>{self.coefficient}')
-
     def parseResponse(self, body_buf):
         pos = 0
 
         (num,) = struct.unpack("<H", body_buf[:2])
 
         last_price = 0
 
@@ -43,11 +40,10 @@
         for _ in range(num):
             price_raw, pos = get_price(body_buf, pos)
             reversed1, pos = get_price(body_buf, pos)
 
             vol, pos = get_price(body_buf, pos)
             last_price = float(last_price + price_raw)
 
-            # todo 此处不能直接除以 100, 需要计算小数点 增加 get_coefficient 函数
             prices.append(OrderedDict([("price", last_price * self.coefficient), ("vol", vol)]))
 
         return prices
```

### Comparing `tdxpy-0.2.2/tdxpy/parser/std/get_report_file.py` & `tdxpy-0.2.3/tdxpy/parser/std/get_report_file.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/std/get_security_bars.py` & `tdxpy-0.2.3/tdxpy/parser/std/get_security_bars.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/std/get_security_count.py` & `tdxpy-0.2.3/tdxpy/parser/std/get_security_count.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/std/get_security_list.py` & `tdxpy-0.2.3/tdxpy/parser/std/get_security_list.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/std/get_security_quotes.py` & `tdxpy-0.2.3/tdxpy/parser/std/get_security_quotes.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             reversed_bytes7, pos = get_price(body_buf, pos)
             reversed_bytes8, pos = get_price(body_buf, pos)
 
             reversed_bytes9, active2 = struct.unpack("<hH", body_buf[pos : pos + 4])
             pos += 4
 
             code = code.decode("utf-8")
-            coefficient = get_security_coefficient(market, code)[0]
+            coefficient = get_security_coefficient(market, code)
 
             one_stock = OrderedDict(
                 [
                     ("market", market),
                     ("code", code),
                     ("active1", active1),
                     ("price", self._cal_price(price, 0, coefficient)),
```

### Comparing `tdxpy-0.2.2/tdxpy/parser/std/get_transaction_data.py` & `tdxpy-0.2.3/tdxpy/parser/std/get_transaction_data.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/parser/std/get_xdxr_info.py` & `tdxpy-0.2.3/tdxpy/parser/std/get_xdxr_info.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/reader/__init__.py` & `tdxpy-0.2.3/tdxpy/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/reader/base_reader.py` & `tdxpy-0.2.3/tdxpy/reader/base_reader.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/reader/block_reader.py` & `tdxpy-0.2.3/tdxpy/reader/block_reader.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/reader/daily_bar_reader.py` & `tdxpy-0.2.3/tdxpy/reader/daily_bar_reader.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/reader/exhq_daily_bar_reader.py` & `tdxpy-0.2.3/tdxpy/reader/exhq_daily_bar_reader.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/reader/history_financial_reader.py` & `tdxpy-0.2.3/tdxpy/reader/history_financial_reader.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/reader/lc_min_bar_reader.py` & `tdxpy-0.2.3/tdxpy/reader/lc_min_bar_reader.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/tdxpy/reader/min_bar_reader.py` & `tdxpy-0.2.3/tdxpy/reader/min_bar_reader.py`

 * *Files identical despite different names*

### Comparing `tdxpy-0.2.2/PKG-INFO` & `tdxpy-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdxpy
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: bopo
 Author-email: ibopo@126.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

