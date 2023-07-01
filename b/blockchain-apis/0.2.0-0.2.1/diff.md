# Comparing `tmp/blockchain-apis-0.2.0.tar.gz` & `tmp/blockchain-apis-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockchain-apis-0.2.0.tar", last modified: Fri Jun 16 11:35:00 2023, max compression
+gzip compressed data, was "blockchain-apis-0.2.1.tar", last modified: Sat Jul  1 10:06:10 2023, max compression
```

## Comparing `blockchain-apis-0.2.0.tar` & `blockchain-apis-0.2.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-16 11:35:00.608572 blockchain-apis-0.2.0/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1095 2023-05-30 13:02:28.000000 blockchain-apis-0.2.0/LICENSE
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4722 2023-06-16 11:35:00.608572 blockchain-apis-0.2.0/PKG-INFO
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3170 2023-06-02 15:30:18.000000 blockchain-apis-0.2.0/README.md
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       38 2023-06-16 11:35:00.608572 blockchain-apis-0.2.0/setup.cfg
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1970 2023-06-16 11:33:21.000000 blockchain-apis-0.2.0/setup.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-16 11:35:00.592571 blockchain-apis-0.2.0/src/
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-16 11:35:00.596572 blockchain-apis-0.2.0/src/blockchain_apis.egg-info/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4722 2023-06-16 11:35:00.000000 blockchain-apis-0.2.0/src/blockchain_apis.egg-info/PKG-INFO
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2009 2023-06-16 11:35:00.000000 blockchain-apis-0.2.0/src/blockchain_apis.egg-info/SOURCES.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        1 2023-06-16 11:35:00.000000 blockchain-apis-0.2.0/src/blockchain_apis.egg-info/dependency_links.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       17 2023-06-16 11:35:00.000000 blockchain-apis-0.2.0/src/blockchain_apis.egg-info/requires.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       15 2023-06-16 11:35:00.000000 blockchain-apis-0.2.0/src/blockchain_apis.egg-info/top_level.txt
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-16 11:35:00.596572 blockchain-apis-0.2.0/src/blockchainapis/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    30775 2023-06-16 11:29:53.000000 blockchain-apis-0.2.0/src/blockchainapis/BlockchainAPIs.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    29587 2023-06-16 11:32:43.000000 blockchain-apis-0.2.0/src/blockchainapis/BlockchainAPIsSync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      622 2023-06-16 11:33:29.000000 blockchain-apis-0.2.0/src/blockchainapis/__init__.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-16 11:35:00.600572 blockchain-apis-0.2.0/src/blockchainapis/exceptions/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      460 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/exceptions/BlockchainAPIsException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      683 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/exceptions/BlockchainNotSupportedException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      676 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/exceptions/ExchangeNotSupportedException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      773 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/exceptions/InvalidPageException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      796 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/exceptions/PairNotFoundException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      775 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/exceptions/TokenNotFoundException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      710 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/exceptions/TooManyRequestsException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      693 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/exceptions/UnauthorizedException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      418 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/exceptions/UnknownBlockchainAPIsException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      922 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/exceptions/__init__.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-16 11:35:00.600572 blockchain-apis-0.2.0/src/blockchainapis/models/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      859 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/AmountIn.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      870 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/AmountOut.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      579 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/Blockchain.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      547 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/Exchange.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      863 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/Exchanges.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      677 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/Pair.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      933 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/Pairs.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      794 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/Reserve.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      760 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/Token.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1826 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/Tokens.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1475 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/__init__.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-16 11:35:00.608572 blockchain-apis-0.2.0/tests/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1564 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_amount_in.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1540 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_amount_in_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1568 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_amount_out.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1544 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_amount_out_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      425 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_blockchains.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      419 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_blockchains_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3237 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_decimal_unsigned.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3169 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_decimal_unsigned_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      569 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_decimals.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      563 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_decimals_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1291 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_exchanges.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1231 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_exchanges_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1322 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_get_token_decimal_form.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1296 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_get_token_decimal_form_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1561 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_get_token_unsigned_form.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1529 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_get_token_unsigned_form_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      593 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_info.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      587 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_info_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2699 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_pairs.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2567 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_pairs_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1392 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_reserves.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1368 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_reserves_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1249 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_tokens.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1189 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_tokens_sync.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-07-01 10:06:10.586140 blockchain-apis-0.2.1/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1095 2023-05-30 13:02:28.000000 blockchain-apis-0.2.1/LICENSE
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4722 2023-07-01 10:06:10.582140 blockchain-apis-0.2.1/PKG-INFO
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3170 2023-06-02 15:30:18.000000 blockchain-apis-0.2.1/README.md
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       38 2023-07-01 10:06:10.586140 blockchain-apis-0.2.1/setup.cfg
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1970 2023-07-01 10:01:58.000000 blockchain-apis-0.2.1/setup.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-07-01 10:06:10.574140 blockchain-apis-0.2.1/src/
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-07-01 10:06:10.578140 blockchain-apis-0.2.1/src/blockchain_apis.egg-info/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4722 2023-07-01 10:06:10.000000 blockchain-apis-0.2.1/src/blockchain_apis.egg-info/PKG-INFO
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2009 2023-07-01 10:06:10.000000 blockchain-apis-0.2.1/src/blockchain_apis.egg-info/SOURCES.txt
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        1 2023-07-01 10:06:10.000000 blockchain-apis-0.2.1/src/blockchain_apis.egg-info/dependency_links.txt
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       17 2023-07-01 10:06:10.000000 blockchain-apis-0.2.1/src/blockchain_apis.egg-info/requires.txt
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       15 2023-07-01 10:06:10.000000 blockchain-apis-0.2.1/src/blockchain_apis.egg-info/top_level.txt
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-07-01 10:06:10.578140 blockchain-apis-0.2.1/src/blockchainapis/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    31023 2023-07-01 10:01:09.000000 blockchain-apis-0.2.1/src/blockchainapis/BlockchainAPIs.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    29587 2023-07-01 10:01:21.000000 blockchain-apis-0.2.1/src/blockchainapis/BlockchainAPIsSync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      622 2023-07-01 10:01:38.000000 blockchain-apis-0.2.1/src/blockchainapis/__init__.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-07-01 10:06:10.578140 blockchain-apis-0.2.1/src/blockchainapis/exceptions/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      460 2023-07-01 10:00:26.000000 blockchain-apis-0.2.1/src/blockchainapis/exceptions/BlockchainAPIsException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      683 2023-07-01 10:00:26.000000 blockchain-apis-0.2.1/src/blockchainapis/exceptions/BlockchainNotSupportedException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      676 2023-07-01 10:00:26.000000 blockchain-apis-0.2.1/src/blockchainapis/exceptions/ExchangeNotSupportedException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      773 2023-07-01 10:00:26.000000 blockchain-apis-0.2.1/src/blockchainapis/exceptions/InvalidPageException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      796 2023-07-01 10:00:26.000000 blockchain-apis-0.2.1/src/blockchainapis/exceptions/PairNotFoundException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      775 2023-07-01 10:00:26.000000 blockchain-apis-0.2.1/src/blockchainapis/exceptions/TokenNotFoundException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      710 2023-07-01 10:00:26.000000 blockchain-apis-0.2.1/src/blockchainapis/exceptions/TooManyRequestsException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      693 2023-07-01 10:00:26.000000 blockchain-apis-0.2.1/src/blockchainapis/exceptions/UnauthorizedException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      418 2023-07-01 10:00:26.000000 blockchain-apis-0.2.1/src/blockchainapis/exceptions/UnknownBlockchainAPIsException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      922 2023-07-01 10:00:26.000000 blockchain-apis-0.2.1/src/blockchainapis/exceptions/__init__.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-07-01 10:06:10.582140 blockchain-apis-0.2.1/src/blockchainapis/models/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      859 2023-07-01 10:00:26.000000 blockchain-apis-0.2.1/src/blockchainapis/models/AmountIn.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      870 2023-07-01 10:00:26.000000 blockchain-apis-0.2.1/src/blockchainapis/models/AmountOut.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      579 2023-07-01 10:00:26.000000 blockchain-apis-0.2.1/src/blockchainapis/models/Blockchain.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      547 2023-07-01 10:00:26.000000 blockchain-apis-0.2.1/src/blockchainapis/models/Exchange.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      863 2023-07-01 10:00:26.000000 blockchain-apis-0.2.1/src/blockchainapis/models/Exchanges.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      677 2023-07-01 10:00:26.000000 blockchain-apis-0.2.1/src/blockchainapis/models/Pair.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      933 2023-07-01 10:00:26.000000 blockchain-apis-0.2.1/src/blockchainapis/models/Pairs.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      794 2023-07-01 10:00:26.000000 blockchain-apis-0.2.1/src/blockchainapis/models/Reserve.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      760 2023-07-01 10:00:26.000000 blockchain-apis-0.2.1/src/blockchainapis/models/Token.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1826 2023-07-01 10:00:26.000000 blockchain-apis-0.2.1/src/blockchainapis/models/Tokens.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1475 2023-07-01 10:00:26.000000 blockchain-apis-0.2.1/src/blockchainapis/models/__init__.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-07-01 10:06:10.582140 blockchain-apis-0.2.1/tests/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1564 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_amount_in.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1540 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_amount_in_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1568 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_amount_out.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1544 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_amount_out_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      425 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_blockchains.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      419 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_blockchains_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3237 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_decimal_unsigned.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3169 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_decimal_unsigned_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      569 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_decimals.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      563 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_decimals_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1291 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_exchanges.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1231 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_exchanges_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1322 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_get_token_decimal_form.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1296 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_get_token_decimal_form_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1561 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_get_token_unsigned_form.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1529 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_get_token_unsigned_form_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      593 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_info.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      587 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_info_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2699 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_pairs.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2567 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_pairs_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1392 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_reserves.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1368 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_reserves_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1249 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_tokens.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1189 2023-06-16 11:29:16.000000 blockchain-apis-0.2.1/tests/test_tokens_sync.py
```

### Comparing `blockchain-apis-0.2.0/LICENSE` & `blockchain-apis-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/PKG-INFO` & `blockchain-apis-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockchain-apis
-Version: 0.2.0
+Version: 0.2.1
 Summary: Fastest and easiest way to access decentralized finance data
 Home-page: https://www.blockchainapis.io
 Author: Clarensia
 Author-email: contact@blockchainapis.io
 License: MIT
 Project-URL: Documentation, https://api.blockchainapis.io/docs
 Project-URL: Source, https://github.com/blockchainapis/blockchain-apis-python-client
```

### Comparing `blockchain-apis-0.2.0/README.md` & `blockchain-apis-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/setup.py` & `blockchain-apis-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
     
 setup(
     name = "blockchain-apis",
-    version = "0.2.0",
+    version = "0.2.1",
     author = "Clarensia",
     author_email = "contact@blockchainapis.io",
     description = "Fastest and easiest way to access decentralized finance data",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://www.blockchainapis.io",
     license="MIT",
```

### Comparing `blockchain-apis-0.2.0/src/blockchain_apis.egg-info/PKG-INFO` & `blockchain-apis-0.2.1/src/blockchain_apis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockchain-apis
-Version: 0.2.0
+Version: 0.2.1
 Summary: Fastest and easiest way to access decentralized finance data
 Home-page: https://www.blockchainapis.io
 Author: Clarensia
 Author-email: contact@blockchainapis.io
 License: MIT
 Project-URL: Documentation, https://api.blockchainapis.io/docs
 Project-URL: Source, https://github.com/blockchainapis/blockchain-apis-python-client
```

### Comparing `blockchain-apis-0.2.0/src/blockchain_apis.egg-info/SOURCES.txt` & `blockchain-apis-0.2.1/src/blockchain_apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/BlockchainAPIs.py` & `blockchain-apis-0.2.1/src/blockchainapis/BlockchainAPIs.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,23 @@
         self._session = ClientSession("https://api.blockchainapis.io")
 
     async def close(self):
         """Close the async session object.
         
         You must call this method at the end of your program or when you have finished
         working with BlockchainAPIs.
+        
+        Please note, if you do:
+        ```py
+        async with BlockchainAPIs() as instance:
+            # do some calls...
+            pass
+        ```
+        
+        The instance is automatically closed at the end of the async with.
         """
         await self._session.close()
 
     async def __aenter__(self):
         """Called when you use `async with`.
         
         For example:
```

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/BlockchainAPIsSync.py` & `blockchain-apis-0.2.1/src/blockchainapis/BlockchainAPIsSync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/__init__.py` & `blockchain-apis-0.2.1/src/blockchainapis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,13 +9,13 @@
 you can use the BlockchainAPIsSync class.
 
 """
 
 # Clarensia: https://www.clarensia.com is the company behind
 # the development of https://www.blockchainapis.io
 __author__ = "Clarensia"
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 from .BlockchainAPIs import BlockchainAPIs
 from .BlockchainAPIsSync import BlockchainAPIsSync
 
 __all__ = ['BlockchainAPIs']
```

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/exceptions/BlockchainNotSupportedException.py` & `blockchain-apis-0.2.1/src/blockchainapis/exceptions/BlockchainNotSupportedException.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/exceptions/ExchangeNotSupportedException.py` & `blockchain-apis-0.2.1/src/blockchainapis/exceptions/ExchangeNotSupportedException.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/exceptions/InvalidPageException.py` & `blockchain-apis-0.2.1/src/blockchainapis/exceptions/InvalidPageException.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/exceptions/PairNotFoundException.py` & `blockchain-apis-0.2.1/src/blockchainapis/exceptions/PairNotFoundException.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/exceptions/TokenNotFoundException.py` & `blockchain-apis-0.2.1/src/blockchainapis/exceptions/TokenNotFoundException.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/exceptions/TooManyRequestsException.py` & `blockchain-apis-0.2.1/src/blockchainapis/exceptions/TooManyRequestsException.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/exceptions/UnauthorizedException.py` & `blockchain-apis-0.2.1/src/blockchainapis/exceptions/UnauthorizedException.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/exceptions/__init__.py` & `blockchain-apis-0.2.1/src/blockchainapis/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/models/AmountIn.py` & `blockchain-apis-0.2.1/src/blockchainapis/models/AmountIn.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/models/AmountOut.py` & `blockchain-apis-0.2.1/src/blockchainapis/models/AmountOut.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/models/Blockchain.py` & `blockchain-apis-0.2.1/src/blockchainapis/models/Blockchain.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/models/Exchange.py` & `blockchain-apis-0.2.1/src/blockchainapis/models/Exchange.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/models/Exchanges.py` & `blockchain-apis-0.2.1/src/blockchainapis/models/Exchanges.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/models/Pair.py` & `blockchain-apis-0.2.1/src/blockchainapis/models/Pair.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/models/Pairs.py` & `blockchain-apis-0.2.1/src/blockchainapis/models/Pairs.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/models/Reserve.py` & `blockchain-apis-0.2.1/src/blockchainapis/models/Reserve.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/models/Token.py` & `blockchain-apis-0.2.1/src/blockchainapis/models/Token.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/models/Tokens.py` & `blockchain-apis-0.2.1/src/blockchainapis/models/Tokens.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/src/blockchainapis/models/__init__.py` & `blockchain-apis-0.2.1/src/blockchainapis/models/__init__.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_amount_in.py` & `blockchain-apis-0.2.1/tests/test_amount_in.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_amount_in_sync.py` & `blockchain-apis-0.2.1/tests/test_amount_in_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_amount_out.py` & `blockchain-apis-0.2.1/tests/test_amount_out.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_amount_out_sync.py` & `blockchain-apis-0.2.1/tests/test_amount_out_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_decimal_unsigned.py` & `blockchain-apis-0.2.1/tests/test_decimal_unsigned.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_decimal_unsigned_sync.py` & `blockchain-apis-0.2.1/tests/test_decimal_unsigned_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_decimals.py` & `blockchain-apis-0.2.1/tests/test_decimals.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_decimals_sync.py` & `blockchain-apis-0.2.1/tests/test_decimals_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_exchanges.py` & `blockchain-apis-0.2.1/tests/test_exchanges.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_exchanges_sync.py` & `blockchain-apis-0.2.1/tests/test_exchanges_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_get_token_decimal_form.py` & `blockchain-apis-0.2.1/tests/test_get_token_decimal_form.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_get_token_decimal_form_sync.py` & `blockchain-apis-0.2.1/tests/test_get_token_decimal_form_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_get_token_unsigned_form.py` & `blockchain-apis-0.2.1/tests/test_get_token_unsigned_form.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_get_token_unsigned_form_sync.py` & `blockchain-apis-0.2.1/tests/test_get_token_unsigned_form_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_info.py` & `blockchain-apis-0.2.1/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_info_sync.py` & `blockchain-apis-0.2.1/tests/test_info_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_pairs.py` & `blockchain-apis-0.2.1/tests/test_pairs.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_pairs_sync.py` & `blockchain-apis-0.2.1/tests/test_pairs_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_reserves.py` & `blockchain-apis-0.2.1/tests/test_reserves.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_reserves_sync.py` & `blockchain-apis-0.2.1/tests/test_reserves_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_tokens.py` & `blockchain-apis-0.2.1/tests/test_tokens.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.2.0/tests/test_tokens_sync.py` & `blockchain-apis-0.2.1/tests/test_tokens_sync.py`

 * *Files identical despite different names*

