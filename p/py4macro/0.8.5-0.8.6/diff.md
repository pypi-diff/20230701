# Comparing `tmp/py4macro-0.8.5.tar.gz` & `tmp/py4macro-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4macro-0.8.5.tar", last modified: Thu May 25 13:47:47 2023, max compression
+gzip compressed data, was "py4macro-0.8.6.tar", last modified: Sat Jul  1 04:42:35 2023, max compression
```

## Comparing `py4macro-0.8.5.tar` & `py4macro-0.8.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-25 13:47:47.130170 py4macro-0.8.5/
--rw-r--r--   0 runner     (501) staff       (20)     1065 2023-05-25 13:47:25.000000 py4macro-0.8.5/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       36 2023-05-25 13:47:25.000000 py4macro-0.8.5/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     6903 2023-05-25 13:47:47.130375 py4macro-0.8.5/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     6516 2023-05-25 13:47:25.000000 py4macro-0.8.5/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-25 13:47:47.085906 py4macro-0.8.5/py4macro/
--rw-r--r--   0 runner     (501) staff       (20)     1259 2023-05-25 13:47:25.000000 py4macro-0.8.5/py4macro/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-25 13:47:47.122594 py4macro-0.8.5/py4macro/data/
--rw-r--r--   0 runner     (501) staff       (20)  1046508 2023-05-25 13:47:25.000000 py4macro-0.8.5/py4macro/data/WEOApr2021all.csv.bz2
--rw-r--r--   0 runner     (501) staff       (20)    35244 2023-05-25 13:47:25.000000 py4macro-0.8.5/py4macro/data/bigmac.csv.bz2
--rw-r--r--   0 runner     (501) staff       (20)      285 2023-05-25 13:47:25.000000 py4macro-0.8.5/py4macro/data/cycle_dates.csv.bz2
--rw-r--r--   0 runner     (501) staff       (20)    14026 2023-05-25 13:47:25.000000 py4macro-0.8.5/py4macro/data/jpn_money.csv.bz2
--rw-r--r--   0 runner     (501) staff       (20)     9425 2023-05-25 13:47:25.000000 py4macro-0.8.5/py4macro/data/jpn_quarterly.csv.bz2
--rw-r--r--   0 runner     (501) staff       (20)   134814 2023-05-25 13:47:25.000000 py4macro-0.8.5/py4macro/data/mad_country.csv.bz2
--rw-r--r--   0 runner     (501) staff       (20)      869 2023-05-25 13:47:25.000000 py4macro-0.8.5/py4macro/data/mad_definitions.csv
--rw-r--r--   0 runner     (501) staff       (20)     4424 2023-05-25 13:47:25.000000 py4macro-0.8.5/py4macro/data/mad_regions.csv
--rw-r--r--   0 runner     (501) staff       (20)     2872 2023-05-25 13:47:25.000000 py4macro-0.8.5/py4macro/data/mad_regions_original.csv
--rw-r--r--   0 runner     (501) staff       (20)  2779563 2023-05-25 13:47:25.000000 py4macro-0.8.5/py4macro/data/pwt_data.csv.bz2
--rw-r--r--   0 runner     (501) staff       (20)     3972 2023-05-25 13:47:25.000000 py4macro-0.8.5/py4macro/data/pwt_definitions.csv
--rw-r--r--   0 runner     (501) staff       (20)    29530 2023-05-25 13:47:25.000000 py4macro-0.8.5/py4macro/data/real_ex_rate.csv.bz2
--rw-r--r--   0 runner     (501) staff       (20)    98831 2023-05-25 13:47:25.000000 py4macro-0.8.5/py4macro/data/world_money.csv.bz2
--rw-r--r--   0 runner     (501) staff       (20)    28011 2023-05-25 13:47:25.000000 py4macro-0.8.5/py4macro/py4macro.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-25 13:47:47.127888 py4macro-0.8.5/py4macro.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     6903 2023-05-25 13:47:46.000000 py4macro-0.8.5/py4macro.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      717 2023-05-25 13:47:47.000000 py4macro-0.8.5/py4macro.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-05-25 13:47:46.000000 py4macro-0.8.5/py4macro.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        7 2023-05-25 13:47:46.000000 py4macro-0.8.5/py4macro.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        9 2023-05-25 13:47:46.000000 py4macro-0.8.5/py4macro.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)       61 2023-05-25 13:47:47.132193 py4macro-0.8.5/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      894 2023-05-25 13:47:25.000000 py4macro-0.8.5/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-01 04:42:35.281763 py4macro-0.8.6/
+-rw-r--r--   0 runner     (501) staff       (20)     1065 2023-07-01 04:42:22.000000 py4macro-0.8.6/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       36 2023-07-01 04:42:22.000000 py4macro-0.8.6/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     6883 2023-07-01 04:42:35.282015 py4macro-0.8.6/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     6496 2023-07-01 04:42:22.000000 py4macro-0.8.6/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-01 04:42:35.261769 py4macro-0.8.6/py4macro/
+-rw-r--r--   0 runner     (501) staff       (20)     1259 2023-07-01 04:42:22.000000 py4macro-0.8.6/py4macro/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-01 04:42:35.277898 py4macro-0.8.6/py4macro/data/
+-rw-r--r--   0 runner     (501) staff       (20)  1046508 2023-07-01 04:42:22.000000 py4macro-0.8.6/py4macro/data/WEOApr2021all.csv.bz2
+-rw-r--r--   0 runner     (501) staff       (20)    17024 2023-07-01 04:42:22.000000 py4macro-0.8.6/py4macro/data/bigmac.csv.bz2
+-rw-r--r--   0 runner     (501) staff       (20)      285 2023-07-01 04:42:22.000000 py4macro-0.8.6/py4macro/data/cycle_dates.csv.bz2
+-rw-r--r--   0 runner     (501) staff       (20)    14026 2023-07-01 04:42:22.000000 py4macro-0.8.6/py4macro/data/jpn_money.csv.bz2
+-rw-r--r--   0 runner     (501) staff       (20)     9425 2023-07-01 04:42:22.000000 py4macro-0.8.6/py4macro/data/jpn_quarterly.csv.bz2
+-rw-r--r--   0 runner     (501) staff       (20)   134814 2023-07-01 04:42:22.000000 py4macro-0.8.6/py4macro/data/mad_country.csv.bz2
+-rw-r--r--   0 runner     (501) staff       (20)      869 2023-07-01 04:42:22.000000 py4macro-0.8.6/py4macro/data/mad_definitions.csv
+-rw-r--r--   0 runner     (501) staff       (20)     4424 2023-07-01 04:42:22.000000 py4macro-0.8.6/py4macro/data/mad_regions.csv
+-rw-r--r--   0 runner     (501) staff       (20)     2872 2023-07-01 04:42:22.000000 py4macro-0.8.6/py4macro/data/mad_regions_original.csv
+-rw-r--r--   0 runner     (501) staff       (20)  2779563 2023-07-01 04:42:22.000000 py4macro-0.8.6/py4macro/data/pwt_data.csv.bz2
+-rw-r--r--   0 runner     (501) staff       (20)     3972 2023-07-01 04:42:22.000000 py4macro-0.8.6/py4macro/data/pwt_definitions.csv
+-rw-r--r--   0 runner     (501) staff       (20)    29530 2023-07-01 04:42:22.000000 py4macro-0.8.6/py4macro/data/real_ex_rate.csv.bz2
+-rw-r--r--   0 runner     (501) staff       (20)    98831 2023-07-01 04:42:22.000000 py4macro-0.8.6/py4macro/data/world_money.csv.bz2
+-rw-r--r--   0 runner     (501) staff       (20)    27892 2023-07-01 04:42:22.000000 py4macro-0.8.6/py4macro/py4macro.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-01 04:42:35.280869 py4macro-0.8.6/py4macro.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     6883 2023-07-01 04:42:35.000000 py4macro-0.8.6/py4macro.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      717 2023-07-01 04:42:35.000000 py4macro-0.8.6/py4macro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-01 04:42:35.000000 py4macro-0.8.6/py4macro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        7 2023-07-01 04:42:35.000000 py4macro-0.8.6/py4macro.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        9 2023-07-01 04:42:35.000000 py4macro-0.8.6/py4macro.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)       61 2023-07-01 04:42:35.282664 py4macro-0.8.6/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      894 2023-07-01 04:42:22.000000 py4macro-0.8.6/setup.py
```

### Comparing `py4macro-0.8.5/LICENSE` & `py4macro-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py4macro-0.8.5/PKG-INFO` & `py4macro-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4macro
-Version: 0.8.5
+Version: 0.8.6
 Summary: A module for py4macro.github.io
 Home-page: https://github.com/Py4Macro/py4macro
 Author: Tetsu Haruyama
 Author-email: haruyama@econ.kobe-u.ac.jp
 License: MIT
 Keywords: data,Penn World Table,IMF World Economic Outlook,Maddison Project,Hodrick-Prescott filter,Japan
 Description-Content-Type: text/markdown
@@ -30,15 +30,15 @@
     * IMF World Economic Outlook 2021
     * Maddison Project Database 2020
     * 日本の四半期データ（GDPなど）
     * 日本の四半期データ（マネーストックなど）
     * 177ヵ国のマネーストックなど
     * 円/ドル為替レートなど
     * 景気循環日付と拡張・後退期間
-    * Big Mac インデックスと購買力平価
+    * Big Macインデックス
 
 # 使い方
 ```
 import py4macro
 ```
 
 ## Hodrick-Prescottフィルターによるトレンド抽出
@@ -202,15 +202,15 @@
     * `'weo'`:   IMF World Economic Outlook 2021
     * `'mad'`:   country data of Maddison Project Database 2020
     * `'mad-regions'`:   regional data of Maddison Project Database 2020
     * `'jpn-q'`: 日本の四半期データ（GDPなど）
     * `'jpn-money'`: 日本の月次データ（CPIとマネーストック）
     * `'world-money'`: 177ヵ国のマネーストックなど
     * `'ex'`: 円/ドル為替レートなど
-    * `'bigmac'`: Big Mac インデックスと購買力平価
+    * `'bigmac'`: Big Macインデックスと購買力平価
 
 
 * `description` (デフォルト：`0`, 整数型):
     * `0`: データのDataFrameを返す
         * 全てのデータセット
     * `1`: 変数の定義を全て表示する
         * 全てのデータセット
```

### Comparing `py4macro-0.8.5/README.md` & `py4macro-0.8.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     * IMF World Economic Outlook 2021
     * Maddison Project Database 2020
     * 日本の四半期データ（GDPなど）
     * 日本の四半期データ（マネーストックなど）
     * 177ヵ国のマネーストックなど
     * 円/ドル為替レートなど
     * 景気循環日付と拡張・後退期間
-    * Big Mac インデックスと購買力平価
+    * Big Macインデックス
 
 # 使い方
 ```
 import py4macro
 ```
 
 ## Hodrick-Prescottフィルターによるトレンド抽出
@@ -190,15 +190,15 @@
     * `'weo'`:   IMF World Economic Outlook 2021
     * `'mad'`:   country data of Maddison Project Database 2020
     * `'mad-regions'`:   regional data of Maddison Project Database 2020
     * `'jpn-q'`: 日本の四半期データ（GDPなど）
     * `'jpn-money'`: 日本の月次データ（CPIとマネーストック）
     * `'world-money'`: 177ヵ国のマネーストックなど
     * `'ex'`: 円/ドル為替レートなど
-    * `'bigmac'`: Big Mac インデックスと購買力平価
+    * `'bigmac'`: Big Macインデックスと購買力平価
 
 
 * `description` (デフォルト：`0`, 整数型):
     * `0`: データのDataFrameを返す
         * 全てのデータセット
     * `1`: 変数の定義を全て表示する
         * 全てのデータセット
```

### Comparing `py4macro-0.8.5/py4macro/__init__.py` & `py4macro-0.8.6/py4macro/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # https://github.com/Py4Macro/py4macro.git
 
 from .py4macro import *
 
 __all__ = ['data','trend','show','xvalues','recessions','fukyo']
 
 __author__ = 'Tetsu Haruyama'
-__version__ = '0.8.5'
+__version__ = '0.8.6'
 __copyright__ = 'Copyright (c) 2023 Tetsu Haruyama'
 
 __doc__ = """
     「Pythonで学ぶマクロ経済学 (中級＋レベル)」のためのモジュール
 
         * HPフィルターを使いトレンドを抽出する`trend()`関数
         * `DataFrame`を全て表示する`show()`関数
```

### Comparing `py4macro-0.8.5/py4macro/data/WEOApr2021all.csv.bz2` & `py4macro-0.8.6/py4macro/data/WEOApr2021all.csv.bz2`

 * *Files identical despite different names*

### Comparing `py4macro-0.8.5/py4macro/data/jpn_money.csv.bz2` & `py4macro-0.8.6/py4macro/data/jpn_money.csv.bz2`

 * *Files identical despite different names*

### Comparing `py4macro-0.8.5/py4macro/data/jpn_quarterly.csv.bz2` & `py4macro-0.8.6/py4macro/data/jpn_quarterly.csv.bz2`

 * *Files identical despite different names*

### Comparing `py4macro-0.8.5/py4macro/data/mad_country.csv.bz2` & `py4macro-0.8.6/py4macro/data/mad_country.csv.bz2`

 * *Files identical despite different names*

### Comparing `py4macro-0.8.5/py4macro/data/mad_definitions.csv` & `py4macro-0.8.6/py4macro/data/mad_definitions.csv`

 * *Files identical despite different names*

### Comparing `py4macro-0.8.5/py4macro/data/mad_regions.csv` & `py4macro-0.8.6/py4macro/data/mad_regions.csv`

 * *Files identical despite different names*

### Comparing `py4macro-0.8.5/py4macro/data/mad_regions_original.csv` & `py4macro-0.8.6/py4macro/data/mad_regions_original.csv`

 * *Files identical despite different names*

### Comparing `py4macro-0.8.5/py4macro/data/pwt_data.csv.bz2` & `py4macro-0.8.6/py4macro/data/pwt_data.csv.bz2`

 * *Files identical despite different names*

### Comparing `py4macro-0.8.5/py4macro/data/pwt_definitions.csv` & `py4macro-0.8.6/py4macro/data/pwt_definitions.csv`

 * *Files identical despite different names*

### Comparing `py4macro-0.8.5/py4macro/data/real_ex_rate.csv.bz2` & `py4macro-0.8.6/py4macro/data/real_ex_rate.csv.bz2`

 * *Files identical despite different names*

### Comparing `py4macro-0.8.5/py4macro/data/world_money.csv.bz2` & `py4macro-0.8.6/py4macro/data/world_money.csv.bz2`

 * *Files identical despite different names*

### Comparing `py4macro-0.8.5/py4macro/py4macro.py` & `py4macro-0.8.6/py4macro/py4macro.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,27 +143,26 @@
     |                `yama`から`tani2`までの期間 
     |
     | ＜出典＞
     |   * 内閣府
     |   * https://www.esri.cao.go.jp/jp/stat/di/hiduke.html"""
 
 bigmac_definitions="""
-    | `year`: 年
+    | `year`: 年（2000年〜2022年）
     | `country`: 国名
     | `iso`: ISO国コード
     | `currency_code`: 通貨コード
-    | `bm_local_price`: ビッグマックの自国通貨価格
-    | `ppp`: 購買力平価に基づく交換率
+    | `price_local`: Big Macの価格（自国通貨単位）
     | `exr`: 名目為替レート（自国通貨単位/米ドル）
-    | `ngdppc`: 名目一人当たりGDP（自国通貨単位）
-    | `rgdppc`: 実質一人当たりGDP（自国通貨単位）
+    | `gdppc_local`: 名目一人当たりGDP（自国通貨単位）
+    |
+    | * 年次データ
     |
     | ＜出典＞
-    | `bm_local_price`: https://github.com/TheEconomist/big-mac-data
-    | その他: The World Bank"""
+    | https://github.com/TheEconomist/big-mac-data (Copyright The Economist)"""
 
 # ===== Helper functions =======================================================================
 
 def _get_path(f):
     return split(abspath(f))[0]
 
 
@@ -370,15 +369,15 @@
        |         'mad':   country data of Maddison Project Database 2020
        |         'mad-regions':   regional data of Maddison Project Database 2020
        |         'jpn-q': 日本の四半期データ（GDPなど）
        |         'jpn-money': 日本の四半期データ（マネーストックなど）
        |         'world-money': 177ヵ国のマネーストックなど
        |         'ex': 円/ドル為替レートなど
        |         'dates': 景気循環日付と拡張・後退期間
-       |         'bigmac': Big Macインデックスと購買力平価
+       |         'bigmac': Big Macインデックス
        |
        |     description (デフォルト：0, 整数型):
        |         0: データのDataFrameを返す
        |            * 全てのデータセット
        |         1: 変数の定義を全て表示する
        |            * 全てのデータセット
        |         2: 変数の定義のDataFrameを返す
@@ -445,15 +444,15 @@
     'mad': country data of Maddison Project Database 2020
     'mad-regions': regional data of Maddison Project Database 2020
     'jpn-q': 日本の四半期データ（GDPなど）
     'jpn-money': 日本の四半期データ（マネーストックなど）
     'world-money': 177ヵ国のマネーストックなど
     'ex': 円/ドル為替レートなど
     'dates': 景気循環日付など
-    'bigmac': Big Macインデックスと購買力平価""")
+    'bigmac': Big Macインデックス""")
         except ValueError as e:
             print(e)
 
     # Penn World Table ----------------------------------------------------------------------
     elif (dataset=='pwt') & (description==0):
         return pd.read_csv(join(_get_path(__file__), "data/pwt_data.csv.bz2"), compression="bz2")
```

### Comparing `py4macro-0.8.5/py4macro.egg-info/PKG-INFO` & `py4macro-0.8.6/py4macro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4macro
-Version: 0.8.5
+Version: 0.8.6
 Summary: A module for py4macro.github.io
 Home-page: https://github.com/Py4Macro/py4macro
 Author: Tetsu Haruyama
 Author-email: haruyama@econ.kobe-u.ac.jp
 License: MIT
 Keywords: data,Penn World Table,IMF World Economic Outlook,Maddison Project,Hodrick-Prescott filter,Japan
 Description-Content-Type: text/markdown
@@ -30,15 +30,15 @@
     * IMF World Economic Outlook 2021
     * Maddison Project Database 2020
     * 日本の四半期データ（GDPなど）
     * 日本の四半期データ（マネーストックなど）
     * 177ヵ国のマネーストックなど
     * 円/ドル為替レートなど
     * 景気循環日付と拡張・後退期間
-    * Big Mac インデックスと購買力平価
+    * Big Macインデックス
 
 # 使い方
 ```
 import py4macro
 ```
 
 ## Hodrick-Prescottフィルターによるトレンド抽出
@@ -202,15 +202,15 @@
     * `'weo'`:   IMF World Economic Outlook 2021
     * `'mad'`:   country data of Maddison Project Database 2020
     * `'mad-regions'`:   regional data of Maddison Project Database 2020
     * `'jpn-q'`: 日本の四半期データ（GDPなど）
     * `'jpn-money'`: 日本の月次データ（CPIとマネーストック）
     * `'world-money'`: 177ヵ国のマネーストックなど
     * `'ex'`: 円/ドル為替レートなど
-    * `'bigmac'`: Big Mac インデックスと購買力平価
+    * `'bigmac'`: Big Macインデックスと購買力平価
 
 
 * `description` (デフォルト：`0`, 整数型):
     * `0`: データのDataFrameを返す
         * 全てのデータセット
     * `1`: 変数の定義を全て表示する
         * 全てのデータセット
```

### Comparing `py4macro-0.8.5/py4macro.egg-info/SOURCES.txt` & `py4macro-0.8.6/py4macro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py4macro-0.8.5/setup.py` & `py4macro-0.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 additional_files = []
 for filename in glob.iglob('./py4macro/**', recursive=True):
     additional_files.append(filename.replace('./py4macro/', ''))
 
 
 setup(
     name='py4macro',
-    version='0.8.5',
+    version='0.8.6',
     author='Tetsu Haruyama',
     author_email='haruyama@econ.kobe-u.ac.jp',
     packages=find_packages(exclude=("data_generation",)),
     package_dir={'py4macro': './py4macro'},
     include_package_data=True,
     package_data={'py4macro': additional_files},
     install_requires=['pandas'],
```

