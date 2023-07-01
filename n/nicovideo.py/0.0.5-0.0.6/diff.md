# Comparing `tmp/nicovideo.py-0.0.5.tar.gz` & `tmp/nicovideo.py-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nicovideo.py-0.0.5.tar", last modified: Sat Jul  1 07:09:59 2023, max compression
+gzip compressed data, was "nicovideo.py-0.0.6.tar", last modified: Sat Jul  1 07:59:56 2023, max compression
```

## Comparing `nicovideo.py-0.0.5.tar` & `nicovideo.py-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-07-01 07:09:59.785252 nicovideo.py-0.0.5/
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     7559 2023-06-24 05:49:10.000000 nicovideo.py-0.0.5/LICENSE.md
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     3557 2023-07-01 07:09:59.785252 nicovideo.py-0.0.5/PKG-INFO
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     2802 2023-06-24 15:54:52.000000 nicovideo.py-0.0.5/README.md
-drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-07-01 07:09:59.785252 nicovideo.py-0.0.5/nicovideo/
--rw-rw-r--   0 okaits    (1000) okaits    (1000)    10894 2023-07-01 07:08:21.000000 nicovideo.py-0.0.5/nicovideo/__init__.py
-drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-07-01 07:09:59.785252 nicovideo.py-0.0.5/nicovideo.py.egg-info/
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     3557 2023-07-01 07:09:59.000000 nicovideo.py-0.0.5/nicovideo.py.egg-info/PKG-INFO
--rw-rw-r--   0 okaits    (1000) okaits    (1000)      195 2023-07-01 07:09:59.000000 nicovideo.py-0.0.5/nicovideo.py.egg-info/SOURCES.txt
--rw-rw-r--   0 okaits    (1000) okaits    (1000)        1 2023-07-01 07:09:59.000000 nicovideo.py-0.0.5/nicovideo.py.egg-info/dependency_links.txt
--rw-rw-r--   0 okaits    (1000) okaits    (1000)       10 2023-07-01 07:09:59.000000 nicovideo.py-0.0.5/nicovideo.py.egg-info/top_level.txt
--rw-rw-r--   0 okaits    (1000) okaits    (1000)       38 2023-07-01 07:09:59.785252 nicovideo.py-0.0.5/setup.cfg
--rw-rw-r--   0 okaits    (1000) okaits    (1000)      993 2023-07-01 07:08:25.000000 nicovideo.py-0.0.5/setup.py
+drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-07-01 07:59:56.269100 nicovideo.py-0.0.6/
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     7559 2023-06-24 05:49:10.000000 nicovideo.py-0.0.6/LICENSE.md
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     6180 2023-07-01 07:59:56.269100 nicovideo.py-0.0.6/PKG-INFO
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     5425 2023-07-01 07:58:26.000000 nicovideo.py-0.0.6/README.md
+drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-07-01 07:59:56.269100 nicovideo.py-0.0.6/nicovideo/
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)    12016 2023-07-01 07:59:03.000000 nicovideo.py-0.0.6/nicovideo/__init__.py
+drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-07-01 07:59:56.269100 nicovideo.py-0.0.6/nicovideo.py.egg-info/
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     6180 2023-07-01 07:59:55.000000 nicovideo.py-0.0.6/nicovideo.py.egg-info/PKG-INFO
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)      195 2023-07-01 07:59:56.000000 nicovideo.py-0.0.6/nicovideo.py.egg-info/SOURCES.txt
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)        1 2023-07-01 07:59:55.000000 nicovideo.py-0.0.6/nicovideo.py.egg-info/dependency_links.txt
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)       10 2023-07-01 07:59:56.000000 nicovideo.py-0.0.6/nicovideo.py.egg-info/top_level.txt
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)       38 2023-07-01 07:59:56.269100 nicovideo.py-0.0.6/setup.cfg
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)      993 2023-07-01 07:59:09.000000 nicovideo.py-0.0.6/setup.py
```

### Comparing `nicovideo.py-0.0.5/LICENSE.md` & `nicovideo.py-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nicovideo.py-0.0.5/PKG-INFO` & `nicovideo.py-0.0.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: nicovideo.py
-Version: 0.0.5
-Summary: Get nicovideo's video metadata.
-Home-page: https://github.com/okaits/nicovideo.py
-Author: okaits#7534
-Author-email: okaits@okaits7534.mydns.jp
-License: GNU Lesser General Public License 3.0
-Keywords: nicovideo
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Natural Language :: Japanese
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # nicovideo.py
 ## What's this
 ニコニコ動画に投稿された動画の情報を取得するライブラリです。動画をダウンロードすることはできません。
 
 ## 使い方
 ### 初期設定
 Python3を使える環境を作り、cloneしたらrequirements.txtから依存モジュールをインストールしてください。  
@@ -55,20 +35,25 @@
 #### `class Video.Metadata(長すぎるので省略) -> Video.Metadata`
 動画のメタデータのクラスです。   
 
 インスタンス変数一覧:
 ```
 videoid: str = 動画ID
 title: str = 動画タイトル
+description: str = 動画概要
 owner: Video.Metadata.User = 投稿者
 counts: Video.Metadata.Counts = 各種カウンター
 duration: int = 動画長（秒）
 postdate: datetime.datetime = 投稿日時
 genre: Video.Metadata.Genre = ジャンル
 tags: list[Video.Metadata.Tag] = タグ一覧
+ranking: Video.Metadata.Ranking = ランキングデータ
+series: Video.Metadata.Series = シリーズ
+thumbnail: Video.Metadata.Thumbnail = サムネイル
+url: str = 視聴URL
 ```
 
 ##### `class Video.Metadata.User(nickname: str = ユーザーのニックネーム, id: str = ユーザーID) -> Video.Metadata.User`
 ユーザーのクラスです。投稿者などを表します。  
   
 インスタンス変数一覧:
 ```
@@ -100,12 +85,53 @@
 タグのクラスです。  
   
 インスタンス変数一覧:
 ```
 name: str = タグ名
 locked: bool = タグロック
 ```
+##### `class Video.Metadata.Ranking(genreranking: Union[Video.Metadata.Ranking.Genre, NoneType] = ジャンルのランキング情報, tagrankings: list[Video.Metadata.Ranking.Tag] = タグ別のランキング情報)`
+ランキングのクラスです。  
+  
+インスタンス変数一覧:
+```
+genreranking: Union[Video.Metadata.Ranking.Genre, NoneType] = ジャンルのランキング情報
+tagrankings: list[Video.Metadata.Ranking.Tag] = タグ別のランキング情報
+```
+###### `class Video.Metadata.Ranking.Genre(genre: Video.Metadata.Genre = ジャンル, rank: int = ランキング最高順位, time: datetime.datetime = 順位獲得日時)`
+ランキング情報とジャンルをまとめて収納するクラスです。  
+  
+インスタンス変数一覧:
+```
+genre: Video.Metadata.Genre = ジャンル
+rank: int = ランキング最高順位
+time: datetime.datetime = 順位獲得日時
+```
+###### `class Video.Metadata.Ranking.Tag(tag: Video.Metadata.Tag = タグ, rank: int = ランキング最高順位, time: datetime.datetime - 順位獲得日時)`
+Video.Metadata.Ranking.Genreと使い方は同じなのでカット。
+
+##### `Class Video.Metadata.Series(seriesid: int = シリーズID, title: str = シリーズタイトル, description: str = シリーズ概要, thumbnail: str = サムネイルURL, prev_video: Union[Video, NoneType] = 前動画, next_video: Union[Video, NoneType] = 次動画, first_video: Union[Video, NoneType] = 最初の動画)`
+シリーズのクラスです。  
+  
+```
+id: int = シリーズID
+title: str = シリーズタイトル
+description: str = シリーズ概要
+thumbnail: str = サムネイルURL
+prev_video: Union[Video, NoneType] = 前動画
+next_video: Union[Video, NoneType] = 次動画
+first_video: Union[Video, NoneType] = 最初の動画
+```
 
+##### `Class Video.Metadata.Thumbnail(small_url: str = サムネイル（小）URL, middle_url: str = サムネイル（中）URL, large_url: str = サムネイル（大）URL, player_url: str = サムネイル（プレイヤー用）URL, ogp_url: str = サムネイル（OGP表示用）URL)`
+サムネイル画像のクラスです。  
+  
+```
+small_url: str = サムネイル（小）URL
+middle_url: str = サムネイル（中）URL
+large_url: str = サムネイル（大）URL
+player_url: str = サムネイル（プレイヤー用）URL
+ogp_url: str = サムネイル（OGP表示用）URL
+```
 # License
 適用ライセンス: LGPL 3.0  
-Copyright © 2023 okaits#7534
-
+Copyright © 2023 okaits#7534
```

### Comparing `nicovideo.py-0.0.5/nicovideo/__init__.py` & `nicovideo.py-0.0.6/nicovideo/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 """ nicovideo.py (video) """
 from __future__ import annotations
 
 import datetime
 import pprint
 import urllib.request
+import urllib.error
 from html import unescape
 from typing import Type, Union
 
 import json5
 from bs4 import BeautifulSoup as bs
 
-__version__ = '0.0.5'
+__version__ = '0.0.6'
+
+class Error():
+    """ Errors """
+    class NicovideoClientError(Exception):
+        """ urllib error """
+        class VideoNotFound(Exception):
+            """ Video not found or deleted """
+        class ConnectionError(Exception):
+            """ Connection error """
 
 class Video():
     """ Video """
     def __init__(self, videoid: str) -> Video:
         self.videoid: str  = videoid
         self.rawdict: dict = {}
 
@@ -83,19 +93,19 @@
                         ) -> Video.Metadata.Ranking.Tag:
                     self.tag : Video.Metadata.Tag  = tag
                     self.rank: int                 = rank
                     self.time: datetime.datetime   = time
 
             def __init__(
                     self,
-                    genreranking: Video.Metadata.Ranking.Genre,
+                    genreranking: Union[Video.Metadata.Ranking.Genre, None],
                     tagrankings: list[Video.Metadata.Ranking.Tag]
                     ) -> Video.Metadata.Ranking:
-                self.genreranking: Video.Metadata.Ranking.Genre       = genreranking
-                self.tagrankings : list[Video.Metadata.Ranking.Genre] = tagrankings
+                self.genreranking: Union[Video.Metadata.Ranking.Genre, None] = genreranking
+                self.tagrankings : list[Video.Metadata.Ranking.Genre]        = tagrankings
 
         class Series():
             """ Series data """
             def __init__(
                     self,
                     seriesid   : int,
                     title      : str,
@@ -134,39 +144,51 @@
                 videoid    : str,
                 title      : str,
                 description: str,
                 owner      : User,
                 counts     : Counts,
                 duration   : int,
                 postdate   : datetime.datetime,
-                genre      : Genre,
+                genre      : Union[Genre, type(None)],
                 tags       : list[Tag],
                 ranking    : Ranking,
                 series     : Series,
                 thumbnail  : Thumbnail
                 ) -> Video.Metadata:
-            self.videoid    : str               = videoid #pylint: disable=C0103
-            self.title      : str               = title
-            self.description: str               = description
-            self.owner      : self.User         = owner
-            self.counts     : self.Counts       = counts
-            self.duration   : int               = duration
-            self.postdate   : datetime.datetime = postdate
-            self.genre      : self.Genre        = genre
-            self.tags       : list[self.Tag]    = tags
-            self.ranking    : self.Ranking      = ranking
-            self.series     : self.Series       = series
-            self.thumbnail  : self.Thumbnail    = thumbnail
-            self.url        : str               = f'https://www.nicovideo.jp/watch/{videoid}'
+            self.videoid    : str                           = videoid #pylint: disable=C0103
+            self.title      : str                           = title
+            self.description: str                           = description
+            self.owner      : self.User                     = owner
+            self.counts     : self.Counts                   = counts
+            self.duration   : int                           = duration
+            self.postdate   : datetime.datetime             = postdate
+            self.genre      : Union[self.Genre, type(None)] = genre
+            self.tags       : list[self.Tag]                = tags
+            self.ranking    : self.Ranking                  = ranking
+            self.series     : self.Series                   = series
+            self.thumbnail  : self.Thumbnail                = thumbnail
+            self.url        : str                           = \
+                f'https://www.nicovideo.jp/watch/{videoid}'
 
     def get_metadata(self) -> Video.Metadata:
         """ Get video's metadata """
         watch_url = f"https://www.nicovideo.jp/watch/{self.videoid}"
-        with urllib.request.urlopen(watch_url) as response:
-            text = response.read()
+        try:
+            with urllib.request.urlopen(watch_url) as response:
+                text = response.read()
+        except urllib.error.HTTPError as exc:
+            if exc.code == 404:
+                raise Error.NicovideoClientError.VideoNotFound("Video not found or deleted.")\
+                    from exc
+            else:
+                raise Error.NicovideoClientError.ConnectionError(
+                    f"Unexpected HTTP Error: {exc.code}"
+                ) from exc
+        except urllib.error.URLError as exc:
+            raise Error.NicovideoClientError.ConnectionError("Connection error.") from exc
 
         soup = bs(text, "html.parser")
         self.rawdict = json5.loads(
             str(soup.find("div", id="js-initial-watch-data")["data-api-data"])
         )
 
         # Tags
@@ -192,15 +214,15 @@
                         )
                     )
                     break
         ranking_genre = self.Metadata.Ranking.Genre(
             self.rawdict['ranking']['genre']['genre'],
             self.rawdict['ranking']['genre']['rank'] ,
             datetime.datetime.fromisoformat(self.rawdict['ranking']['genre']['dateTime'])
-        )
+        ) if self.rawdict['ranking']['genre'] else None
 
         data = self.Metadata(
             videoid     = self.rawdict['video']['id'],
             title       = self.rawdict['video']['title'],
             description = self.rawdict['video']['description'],
             owner       = self.Metadata.User(
                            nickname = self.rawdict['owner']['nickname'],
@@ -228,15 +250,15 @@
                            thumbnail = self.rawdict['series']['thumbnailUrl'],
                            prev_video = Video(self.rawdict['series']['video']['prev']['id'])
                                if self.rawdict['series']['video']['prev'] else None,
                            next_video = Video(self.rawdict['series']['video']['next']['id'])
                                if self.rawdict['series']['video']['next'] else None,
                            first_video = Video(self.rawdict['series']['video']['first']['id'])
                                if self.rawdict['series']['video']['first'] else None
-               ),
+               ) if self.rawdict['series'] else None,
             thumbnail   = self.Metadata.Thumbnail(
                            small_url  = self.rawdict['video']['thumbnail']['url'],
                            middle_url = self.rawdict['video']['thumbnail']['middleUrl'],
                            large_url  = self.rawdict['video']['thumbnail']['largeUrl'],
                            player_url = self.rawdict['video']['thumbnail']['player'],
                            ogp_url    = self.rawdict['video']['thumbnail']['ogp']
                 ),
```

### Comparing `nicovideo.py-0.0.5/setup.py` & `nicovideo.py-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages, setup
 
 readme = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name='nicovideo.py',
-    version='0.0.5',
+    version='0.0.6',
     description='Get nicovideo\'s video metadata.',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='okaits#7534',
     author_email='okaits@okaits7534.mydns.jp',
     url='https://github.com/okaits/nicovideo.py',
     classifiers=[
```

