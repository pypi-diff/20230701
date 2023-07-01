# Comparing `tmp/nicovideo.py-0.0.3.tar.gz` & `tmp/nicovideo.py-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nicovideo.py-0.0.3.tar", last modified: Sat Jun 24 13:38:19 2023, max compression
+gzip compressed data, was "nicovideo.py-0.0.4.tar", last modified: Sat Jul  1 05:48:46 2023, max compression
```

## Comparing `nicovideo.py-0.0.3.tar` & `nicovideo.py-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-06-24 13:38:19.690008 nicovideo.py-0.0.3/
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     7559 2023-06-24 05:49:10.000000 nicovideo.py-0.0.3/LICENSE.md
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     3057 2023-06-24 13:38:19.686007 nicovideo.py-0.0.3/PKG-INFO
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     2302 2023-06-24 05:53:31.000000 nicovideo.py-0.0.3/README.md
-drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-06-24 13:38:19.682007 nicovideo.py-0.0.3/nicovideo/
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     4430 2023-06-24 13:37:46.000000 nicovideo.py-0.0.3/nicovideo/__init__.py
-drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-06-24 13:38:19.686007 nicovideo.py-0.0.3/nicovideo.py.egg-info/
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     3057 2023-06-24 13:38:19.000000 nicovideo.py-0.0.3/nicovideo.py.egg-info/PKG-INFO
--rw-rw-r--   0 okaits    (1000) okaits    (1000)      195 2023-06-24 13:38:19.000000 nicovideo.py-0.0.3/nicovideo.py.egg-info/SOURCES.txt
--rw-rw-r--   0 okaits    (1000) okaits    (1000)        1 2023-06-24 13:38:19.000000 nicovideo.py-0.0.3/nicovideo.py.egg-info/dependency_links.txt
--rw-rw-r--   0 okaits    (1000) okaits    (1000)       10 2023-06-24 13:38:19.000000 nicovideo.py-0.0.3/nicovideo.py.egg-info/top_level.txt
--rw-rw-r--   0 okaits    (1000) okaits    (1000)       38 2023-06-24 13:38:19.690008 nicovideo.py-0.0.3/setup.cfg
--rw-rw-r--   0 okaits    (1000) okaits    (1000)      976 2023-06-24 13:37:51.000000 nicovideo.py-0.0.3/setup.py
+drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-07-01 05:48:46.563040 nicovideo.py-0.0.4/
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     7559 2023-06-24 05:49:10.000000 nicovideo.py-0.0.4/LICENSE.md
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     3557 2023-07-01 05:48:46.563040 nicovideo.py-0.0.4/PKG-INFO
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     2802 2023-06-24 15:54:52.000000 nicovideo.py-0.0.4/README.md
+drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-07-01 05:48:46.563040 nicovideo.py-0.0.4/nicovideo/
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     4784 2023-07-01 05:47:03.000000 nicovideo.py-0.0.4/nicovideo/__init__.py
+drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-07-01 05:48:46.563040 nicovideo.py-0.0.4/nicovideo.py.egg-info/
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     3557 2023-07-01 05:48:46.000000 nicovideo.py-0.0.4/nicovideo.py.egg-info/PKG-INFO
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)      195 2023-07-01 05:48:46.000000 nicovideo.py-0.0.4/nicovideo.py.egg-info/SOURCES.txt
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)        1 2023-07-01 05:48:46.000000 nicovideo.py-0.0.4/nicovideo.py.egg-info/dependency_links.txt
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)       10 2023-07-01 05:48:46.000000 nicovideo.py-0.0.4/nicovideo.py.egg-info/top_level.txt
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)       38 2023-07-01 05:48:46.563040 nicovideo.py-0.0.4/setup.cfg
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)      993 2023-07-01 05:47:08.000000 nicovideo.py-0.0.4/setup.py
```

### Comparing `nicovideo.py-0.0.3/LICENSE.md` & `nicovideo.py-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nicovideo.py-0.0.3/PKG-INFO` & `nicovideo.py-0.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicovideo.py
-Version: 0.0.3
+Version: 0.0.4
 Summary: Get nicovideo's video metadata.
 Home-page: https://github.com/okaits/nicovideo.py
 Author: okaits#7534
 Author-email: okaits@okaits7534.mydns.jp
 License: GNU Lesser General Public License 3.0
 Keywords: nicovideo
 Platform: UNKNOWN
@@ -36,71 +36,71 @@
 ```python3
 import nicovideo
 video = nicovideo.Video('動画ID')
 metadata = video.get_metadata()
 ```
 
 ## クラス・関数やその返り値など
-### class Video
+### `class Video(videoid: str = 動画ID) -> Video`
 動画のクラスです。  
   
 インスタンス変数一覧:
 ```
 videoid: str = 動画ID
 rawdict: dict = 取得した生データ（Video.get_metadataを実行するまではNone）
 ```
 
-#### def Video.get_metadata() -> Video.Metadata
+#### `def Video.get_metadata() -> Video.Metadata`
 動画のメタデータを取得するメソッドです。
 
-#### class Video.Metadata
+#### `class Video.Metadata(長すぎるので省略) -> Video.Metadata`
 動画のメタデータのクラスです。   
 
 インスタンス変数一覧:
 ```
 videoid: str = 動画ID
 title: str = 動画タイトル
 owner: Video.Metadata.User = 投稿者
 counts: Video.Metadata.Counts = 各種カウンター
 duration: int = 動画長（秒）
 postdate: datetime.datetime = 投稿日時
 genre: Video.Metadata.Genre = ジャンル
 tags: list[Video.Metadata.Tag] = タグ一覧
 ```
 
-##### class Video.Metadata.User
+##### `class Video.Metadata.User(nickname: str = ユーザーのニックネーム, id: str = ユーザーID) -> Video.Metadata.User`
 ユーザーのクラスです。投稿者などを表します。  
   
 インスタンス変数一覧:
 ```
 nickname: str = ユーザーニックネーム
 id: int = ユーザーID
 ```
 
-##### class Video.Metadata.Counts
+##### `class Video.Metadata.Counts(comments: int = コメント数, likes: int = いいね！数, mylists: int = マイリス数, views: id = 再生数) -> Video.Metadata.Counts`
 各種カウンターのクラスです。再生数などのカウンターを表します。  
   
 インスタンス変数一覧:
 ```
 comments: int = コメント数
 likes: int = いいね！数
 mylists: int = マイリスト数
 views: int = 再生数
 ```
 
-##### class Video.Metadata.Genre
+##### `class Video.Metadata.Genre(label: str = ジャンル名, key: ジャンルの内部キー) -> Video.Metadata.Genre`
 ジャンルのクラスです。  
   
 インスタンス変数一覧:
 ```
 label: str = ジャンル名
 key: str = 内部識別キー
 ```
 
-##### class Video.Metadata.Tag
+##### `class Video.Metadata.Tag(name: str = タグ名, locked: bool = タグロック) -> Video.Metadata.Tag`
 タグのクラスです。  
   
 インスタンス変数一覧:
 ```
 name: str = タグ名
 locked: bool = タグロック
 ```
```

### Comparing `nicovideo.py-0.0.3/README.md` & `nicovideo.py-0.0.4/nicovideo.py.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: nicovideo.py
+Version: 0.0.4
+Summary: Get nicovideo's video metadata.
+Home-page: https://github.com/okaits/nicovideo.py
+Author: okaits#7534
+Author-email: okaits@okaits7534.mydns.jp
+License: GNU Lesser General Public License 3.0
+Keywords: nicovideo
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Natural Language :: Japanese
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # nicovideo.py
 ## What's this
 ニコニコ動画に投稿された動画の情報を取得するライブラリです。動画をダウンロードすることはできません。
 
 ## 使い方
 ### 初期設定
 Python3を使える環境を作り、cloneしたらrequirements.txtから依存モジュールをインストールしてください。  
@@ -16,75 +36,76 @@
 ```python3
 import nicovideo
 video = nicovideo.Video('動画ID')
 metadata = video.get_metadata()
 ```
 
 ## クラス・関数やその返り値など
-### class Video
+### `class Video(videoid: str = 動画ID) -> Video`
 動画のクラスです。  
   
 インスタンス変数一覧:
 ```
 videoid: str = 動画ID
 rawdict: dict = 取得した生データ（Video.get_metadataを実行するまではNone）
 ```
 
-#### def Video.get_metadata() -> Video.Metadata
+#### `def Video.get_metadata() -> Video.Metadata`
 動画のメタデータを取得するメソッドです。
 
-#### class Video.Metadata
+#### `class Video.Metadata(長すぎるので省略) -> Video.Metadata`
 動画のメタデータのクラスです。   
 
 インスタンス変数一覧:
 ```
 videoid: str = 動画ID
 title: str = 動画タイトル
 owner: Video.Metadata.User = 投稿者
 counts: Video.Metadata.Counts = 各種カウンター
 duration: int = 動画長（秒）
 postdate: datetime.datetime = 投稿日時
 genre: Video.Metadata.Genre = ジャンル
 tags: list[Video.Metadata.Tag] = タグ一覧
 ```
 
-##### class Video.Metadata.User
+##### `class Video.Metadata.User(nickname: str = ユーザーのニックネーム, id: str = ユーザーID) -> Video.Metadata.User`
 ユーザーのクラスです。投稿者などを表します。  
   
 インスタンス変数一覧:
 ```
 nickname: str = ユーザーニックネーム
 id: int = ユーザーID
 ```
 
-##### class Video.Metadata.Counts
+##### `class Video.Metadata.Counts(comments: int = コメント数, likes: int = いいね！数, mylists: int = マイリス数, views: id = 再生数) -> Video.Metadata.Counts`
 各種カウンターのクラスです。再生数などのカウンターを表します。  
   
 インスタンス変数一覧:
 ```
 comments: int = コメント数
 likes: int = いいね！数
 mylists: int = マイリスト数
 views: int = 再生数
 ```
 
-##### class Video.Metadata.Genre
+##### `class Video.Metadata.Genre(label: str = ジャンル名, key: ジャンルの内部キー) -> Video.Metadata.Genre`
 ジャンルのクラスです。  
   
 インスタンス変数一覧:
 ```
 label: str = ジャンル名
 key: str = 内部識別キー
 ```
 
-##### class Video.Metadata.Tag
+##### `class Video.Metadata.Tag(name: str = タグ名, locked: bool = タグロック) -> Video.Metadata.Tag`
 タグのクラスです。  
   
 インスタンス変数一覧:
 ```
 name: str = タグ名
 locked: bool = タグロック
 ```
 
 # License
 適用ライセンス: LGPL 3.0  
-Copyright © 2023 okaits#7534
+Copyright © 2023 okaits#7534
+
```

### Comparing `nicovideo.py-0.0.3/nicovideo/__init__.py` & `nicovideo.py-0.0.4/nicovideo/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,64 @@
 """ nicovideo.py (video) """
+from __future__ import annotations
 
-__version__ = '0.0.3'
-
+import datetime
 import pprint
 import urllib.request
 from html import unescape
-import datetime
+from typing import Type
 
 import json5
 from bs4 import BeautifulSoup as bs
 
+__version__ = '0.0.4'
 
 class Video():
     """ Video """
-    def __init__(self, videoid: str):
+    def __init__(self, videoid: str) -> Video:
         self.videoid       = videoid
         self.rawdict: dict = {}
 
     class Metadata():
         """ Meta data """
 
         class User():
             """ User data """
-            def __init__(self, nickname: str, videoid: str):
+            def __init__(self, nickname: str, userid: str) -> Video.Metadata.User:
                 self.nickname: str = nickname
-                self.id      : str = videoid #pylint: disable=C0103
-            def __str__(self):
+                self.id      : str = userid #pylint: disable=C0103
+            def __str__(self) -> str:
                 return f'{self.nickname} [ID: {self.id}]'
 
         class Counts():
             """ Counts data """
-            def __init__(self, comments: int, likes: int, mylists: int, views: int):
+            def __init__(self, comments: int, likes: int, mylists: int, views: int)\
+                    -> Video.Metadata.Counts:
                 self.comments: int = comments
                 self.likes   : int = likes
                 self.mylists : int = mylists
                 self.views   : int = views
-            def __str__(self):
-                returndata = f'Comments: {self.comments}\n'
-                returndata += f'Likes: {self.likes}\n'
+            def __str__(self) -> str:
+                returndata = f'Views: {self.views}\n'
+                returndata += f'Comments: {self.comments}\n'
                 returndata += f'Mylists: {self.mylists}\n'
-                returndata += f'Views: {self.views}'
+                returndata += f'Likes: {self.likes}'
                 return returndata
 
         class Genre():
             """ Genre data """
-            def __init__(self, label, key):
+            def __init__(self, label: str, key: str) -> Video.Metadata.Genre:
                 self.label   : str = label
                 self.key     : str = key
             def __str__(self):
                 return self.label
 
         class Tag():
             """ Tag data """
-            def __init__(self, name: str, locked: bool):
+            def __init__(self, name: str, locked: bool) -> Video.Metadata.Tag:
                 self.name  : str  = name
                 self.locked: bool = locked
             def __str__(self):
                 return f'{self.name}{" [Locked]" if self.locked else ""}'
 
         def __init__(
                 self,
@@ -64,32 +66,35 @@
                 title   : str,
                 owner   : User,
                 counts  : Counts,
                 duration: int,
                 postdate: datetime.datetime,
                 genre   : Genre,
                 tags    : list[Tag]
-                ):
+                ) -> Video.Metadata:
             self.videoid  : str               = videoid #pylint: disable=C0103
             self.title    : str               = title
             self.owner    : self.User         = owner
             self.counts   : self.Counts       = counts
             self.duration : int               = duration
             self.postdate : datetime.datetime = postdate
             self.genre    : self.Genre        = genre
             self.tags     : list[self.Tag]    = tags
+            self.url      : str               = f'https://www.nicovideo.jp/watch/{videoid}'
 
-    def get_metadata(self):
+    def get_metadata(self) -> Video.Metadata:
         """ Get video's metadata """
         watch_url = f"https://www.nicovideo.jp/watch/{self.videoid}"
         with urllib.request.urlopen(watch_url) as response:
             text = response.read()
 
         soup = bs(text, "html.parser")
-        self.rawdict = json5.loads(str(soup.find("div", id="js-initial-watch-data")["data-api-data"]))
+        self.rawdict = json5.loads(
+            str(soup.find("div", id="js-initial-watch-data")["data-api-data"])
+        )
 
         # Tags
         tags = []
         for tag in self.rawdict['tag']['items']:
             tags.append(
                 self.Metadata.Tag(
                     name=tag['name'],
@@ -98,15 +103,15 @@
             )
 
         return self.Metadata(
             videoid  = self.rawdict['video']['id'],
             title    = self.rawdict['video']['title'],
             owner    = self.Metadata.User(
                         nickname = self.rawdict['owner']['nickname'],
-                        videoid  = self.rawdict['owner']['id']
+                        userid   = self.rawdict['owner']['id']
                        ),
             counts   = self.Metadata.Counts(
                         comments = self.rawdict['video']['count']['comment'],
                         likes    = self.rawdict['video']['count']['like'],
                         mylists  = self.rawdict['video']['count']['mylist'],
                         views    = self.rawdict['video']['count']['view']
                        ),
```

### Comparing `nicovideo.py-0.0.3/setup.py` & `nicovideo.py-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+""" Setup.py """
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 readme = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name='nicovideo.py',
-    version='0.0.3',
+    version='0.0.4',
     description='Get nicovideo\'s video metadata.',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='okaits#7534',
     author_email='okaits@okaits7534.mydns.jp',
     url='https://github.com/okaits/nicovideo.py',
     classifiers=[
```

