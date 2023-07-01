# Comparing `tmp/spotify_recommender_api-4.4.0-py3-none-any.whl.zip` & `tmp/spotify_recommender_api-4.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 41895 bytes, number of entries: 13
--rw-rw-r--  2.0 unx       21 b- defN 23-Jul-01 13:50 spotify_recommender_api/__init__.py
+Zip file size: 41854 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx       21 b- defN 23-Jul-01 20:09 spotify_recommender_api/__init__.py
 -rw-rw-r--  2.0 unx     1263 b- defN 23-Jul-01 13:50 spotify_recommender_api/authentication.py
--rw-rw-r--  2.0 unx    15397 b- defN 23-Jul-01 14:16 spotify_recommender_api/core.py
+-rw-rw-r--  2.0 unx    15410 b- defN 23-Jul-01 20:09 spotify_recommender_api/core.py
 -rw-rw-r--  2.0 unx     2042 b- defN 23-Jun-23 14:32 spotify_recommender_api/error.py
--rw-rw-r--  2.0 unx   116978 b- defN 23-Jul-01 14:24 spotify_recommender_api/recommender.py
+-rw-rw-r--  2.0 unx   116945 b- defN 23-Jul-01 20:10 spotify_recommender_api/recommender.py
 -rw-rw-r--  2.0 unx     6306 b- defN 23-Jul-01 13:51 spotify_recommender_api/request_handler.py
 -rw-rw-r--  2.0 unx       99 b- defN 22-Jun-25 22:21 spotify_recommender_api/sensitive.py
 -rw-rw-r--  2.0 unx     6722 b- defN 23-Jul-01 13:51 spotify_recommender_api/server.py
--rw-rw-r--  2.0 unx     9726 b- defN 23-Jul-01 14:17 spotify_recommender_api/util.py
--rw-rw-r--  2.0 unx    21574 b- defN 23-Jul-01 14:26 spotify_recommender_api-4.4.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-01 14:26 spotify_recommender_api-4.4.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       24 b- defN 23-Jul-01 14:26 spotify_recommender_api-4.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1194 b- defN 23-Jul-01 14:26 spotify_recommender_api-4.4.0.dist-info/RECORD
-13 files, 181438 bytes uncompressed, 39863 bytes compressed:  78.0%
+-rw-rw-r--  2.0 unx     9726 b- defN 23-Jul-01 20:09 spotify_recommender_api/util.py
+-rw-rw-r--  2.0 unx    21574 b- defN 23-Jul-01 20:11 spotify_recommender_api-4.4.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-01 20:11 spotify_recommender_api-4.4.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       24 b- defN 23-Jul-01 20:11 spotify_recommender_api-4.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1194 b- defN 23-Jul-01 20:11 spotify_recommender_api-4.4.1.dist-info/RECORD
+13 files, 181418 bytes uncompressed, 39822 bytes compressed:  78.0%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: spotify_recommender_api/server.py
 Comment: 
 
 Filename: spotify_recommender_api/util.py
 Comment: 
 
-Filename: spotify_recommender_api-4.4.0.dist-info/METADATA
+Filename: spotify_recommender_api-4.4.1.dist-info/METADATA
 Comment: 
 
-Filename: spotify_recommender_api-4.4.0.dist-info/WHEEL
+Filename: spotify_recommender_api-4.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: spotify_recommender_api-4.4.0.dist-info/top_level.txt
+Filename: spotify_recommender_api-4.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: spotify_recommender_api-4.4.0.dist-info/RECORD
+Filename: spotify_recommender_api-4.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spotify_recommender_api/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '4.4.0'
+__version__ = '4.4.1'
```

## spotify_recommender_api/core.py

```diff
@@ -170,16 +170,16 @@
 
     elif type == 'artist':
         playlist_name = f"This once was {additional_info!r}"
         description = f'''{additional_info}'{"" if additional_info[-1] == "s" else "s"} songs, within the playlist {base_playlist_name}'''
 
     elif type == 'profile-recommendation':
         criteria = additional_info[0] if additional_info[0] != 'mixed' else 'genres, tracks and artists'
-        playlist_name = f"Profile {additional_info[2].replace('_', ' ').capitalize()} Recommendation"
-        description = f'''Profile-based {additional_info[2].replace('_', ' ')} recommendations based on favorite {criteria}'''
+        playlist_name = f"{additional_info[2].replace('_', ' ').capitalize()} Profile Recommendation"
+        description = f'''{additional_info[2].replace('_', ' ').capitalize()} profile-based recommendations based on favorite {criteria}'''
 
         if additional_info[1]:
             now = datetime.datetime.now(tz=pytz.timezone('UTC'))
             playlist_name += f' ({criteria} - {now.strftime("%Y-%m-%d")})'
             description += f' - {now.strftime("%Y-%m-%d")} snapshot'
         else:
             playlist_name += f' ({criteria})'
@@ -216,15 +216,15 @@
 
         delete_json = requests.delete_request(
             url=f'https://api.spotify.com/v1/playlists/{new_id}/tracks', headers=headers, data={"tracks": playlist_tracks}).json()
 
         if (
             _update_created_playlists or
             (
-                playlist_name.lower().startswith('profile short term recommendation') and
+                playlist_name.lower().startswith('short term profile recommendation') and
                 playlist_found[1] == playlist_name.replace('Short term ', '')
             )
         ):
             data = {
                 "name": playlist_name,
                 "description": description,
                 "public": False
```

## spotify_recommender_api/recommender.py

```diff
@@ -1037,18 +1037,18 @@
         _, name, description, _ = playlist
 
         if name in {'Long Term Most-listened Tracks', 'Medium Term Most-listened Tracks', 'Short Term Most-listened Tracks'} and 'most-listened-tracks' in playlist_types_to_update:
             return True
 
         elif (
             ' - 20' not in name and
-            all(word in name for word in {'Profile', 'Recommendation'}) and
+            'Profile Recommendation' in name and
             any(
                 playlist_type in playlist_types_to_update
-                for playlist_type in {'profile-short-term-recommendation', 'profile-medium-term-recommendation', 'profile-long-term-recommendation'}
+                for playlist_type in {'short-term-profile-recommendation', 'medium-term-profile-recommendation', 'long-term-profile-recommendation'}
             )
         ):
             return True
 
         elif f', within the playlist {self.__base_playlist_name}' in description or self.__update_created_files:
             if (re.match(r"\'(.*?)\' Related", name) or re.match(r'\"(.*?)\" Related', name)) and 'song-related' in playlist_types_to_update:
                 return True
@@ -1076,34 +1076,34 @@
         """Update all package generated playlists in batch
 
         Note:
             It is NOT recommended to use the K parameter in this function, unless 100% on purpose, since it will make all the playlists have the same number of songs in them
 
         Arguments:
             K (int, optional): Number of songs in the new playlists, if not set, defaults to the number of songs already in the playlist. Defaults to None.
-            playlist_types_to_update (list[str], optional): List of playlist types to update. For example, if you only want to update song-related playlists use this argument as ['song-related']. Defaults to all == ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'profile-short-term-recommendation', 'profile-medium-term-recommendation', 'profile-long-term-recommendation', 'mood'].
+            playlist_types_to_update (list[str], optional): List of playlist types to update. For example, if you only want to update song-related playlists use this argument as ['song-related']. Defaults to all == ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'short-term-profile-recommendation', 'medium-term-profile-recommendation', 'long-term-profile-recommendation', 'mood'].
             playlist_types_not_to_update (list[str], optional): List of playlist types not to update. For example, if you want to update all playlists but song-related playlists use this argument as ['song-related']. it can be used alongside with the playlist_types_to_update but it can become confusing or redundant. Defaults to none == [].
         """
         if playlist_types_to_update is None:
-            playlist_types_to_update = ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'profile-short-term-recommendation', 'profile-medium-term-recommendation', 'profile-long-term-recommendation', 'mood']
+            playlist_types_to_update = ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'short-term-profile-recommendation', 'medium-term-profile-recommendation', 'long-term-profile-recommendation', 'mood']
 
         if playlist_types_not_to_update is None:
             playlist_types_not_to_update = []
 
         playlist_types_to_update = [playlist_type for playlist_type in playlist_types_to_update if playlist_type not in playlist_types_not_to_update]
 
         if 'profile-recommendation' in playlist_types_to_update:
             logging.info('After version 4.4.0, the profile-recommendation playlists are separated in short, medium and long term. See the update_all_created_playlists docstring or the documentation at: https://github.com/nikolas-virionis/spotify-api')
             playlist_types_to_update.remove('profile-recommendation')
-            for playlist_type in {'profile-short-term-recommendation', 'profile-medium-term-recommendation', 'profile-long-term-recommendation'}:
+            for playlist_type in {'short-term-profile-recommendation', 'medium-term-profile-recommendation', 'long-term-profile-recommendation'}:
                 if playlist_type not in playlist_types_to_update:
                     playlist_types_to_update.append(playlist_type)
 
         if 'profile-recommendation' in playlist_types_not_to_update:
-            for playlist_type in {'profile-recommendation', 'profile-short-term-recommendation', 'profile-medium-term-recommendation', 'profile-long-term-recommendation'}:
+            for playlist_type in {'profile-recommendation', 'short-term-profile-recommendation', 'medium-term-profile-recommendation', 'long-term-profile-recommendation'}:
                 if playlist_type in playlist_types_to_update:
                     playlist_types_to_update.remove(playlist_type)
 
         total_playlist_count = requests.get_request(url='https://api.spotify.com/v1/me/playlists?limit=0', headers=self.__headers).json()['total']
 
         playlists = []
 
@@ -1195,45 +1195,45 @@
                             K=total_tracks,
                             build_playlist=True,
                             exclude_mostly_instrumental=exclude_mostly_instrumental,
                         )
 
                 elif (
                     ' - 20' not in name and
-                    all(word in name for word in {'Profile', 'Recommendation'}) and
+                    'Profile Recommendation' in name and
                     any(
                         playlist_type in playlist_types_to_update
-                        for playlist_type in {'profile-short-term-recommendation', 'profile-medium-term-recommendation', 'profile-long-term-recommendation'}
+                        for playlist_type in {'short-term-profile-recommendation', 'medium-term-profile-recommendation', 'long-term-profile-recommendation'}
                     )
                 ):
                     criteria = name.split('(')[1].split(')')[0]
                     criteria_name = criteria
 
                     if ',' in criteria:
                         criteria = 'mixed'
 
                     if 'term' in name.lower():
                         time_range = '_'.join(name.split(' ')[1:3]).lower()
                     else:
                         time_range = 'short_term'
-                        playlist_name = f"Profile {time_range.replace('_', ' ').capitalize()} Recommendation ({criteria_name})"
-                        description = f'''Profile-based {time_range.replace('_', ' ')} recommendations based on favorite {criteria_name}'''
+                        playlist_name = f"{time_range.replace('_', ' ').capitalize()} Profile Recommendation ({criteria_name})"
+                        description = f'''{time_range.replace('_', ' ').capitalize()} Profile-based recommendations based on favorite {criteria_name}'''
 
                         data = {
                             "name": playlist_name,
                             "description": description,
                             "public": False
                         }
 
                         logging.info(f'Updating the name and description of the playlist {name} because of new time range specifications added to the profile_recommendation function in version 4.4.0')
                         logging.info('In case of any problems with the feature, submit an issue at: https://github.com/nikolas-virionis/spotify-api/issues')
 
                         update_playlist_details = requests.put_request(url=f'https://api.spotify.com/v1/playlists/{playlist_id}', headers=self.__headers, data=data)
 
-                    if f"profile-{time_range.replace('_', '-')}-recommendation" not in playlist_types_to_update:
+                    if f"{time_range.replace('_', '-')}-profile-recommendation" not in playlist_types_to_update:
                         continue
 
                     self.get_profile_recommendation(
                         K=total_tracks,
                         build_playlist=True,
                         time_range=time_range,
                         main_criteria=criteria,
@@ -2186,16 +2186,16 @@
                         for song, artist in tracks_info: # type: ignore because of the strict typing not recognizing that the condition above makes this a safe operation
                             description += f'{song} by {artist}, '
                         tracks = [
                             requests.get_request(
                                 headers=self.__headers,
                                 url=f'https://api.spotify.com/v1/search?q={song} {artist}&type=track&limit=1',
                             ).json()['tracks']['items'][0]['id']
-                        for song, artist in tracks_info # type: ignore because of the strict typing not recognizing that the condition above makes this a safe operation
-                    ]
+                            for song, artist in tracks_info # type: ignore because of the strict typing not recognizing that the condition above makes this a safe operation
+                        ]
 
                     elif isinstance(tracks_info[0], str):
                         for song in tracks_info:
                             description += f'{song}, '
                         tracks = [
                             requests.get_request(
                                 headers=self.__headers,
```

## Comparing `spotify_recommender_api-4.4.0.dist-info/METADATA` & `spotify_recommender_api-4.4.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-recommender-api
-Version: 4.4.0
+Version: 4.4.1
 Summary: Python package which takes the songs of a greater playlist as starting point to make recommendations of groups of songs that might bond well within that same playlist, using K-Nearest-Neighbors Technique
 Home-page: https://github.com/nikolas-virionis/spotify-api
 Author: Nikolas B Virionis
 Author-email: nikolas.virionis@bandtec.com.br
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -151,15 +151,15 @@
 # No parameters are mandatory but the default values should be noted
 # BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
 ~~~
  - update_all_generated_playlists
 ### WILL CHANGE THE USER'S LIBRARY DRASTICALLY
 ~~~python
 # Parameters
-update_all_generated_playlists(K: int = None, playlist_types_to_update: list[str] = ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'profile-short-term-recommendation', 'profile-medium-term-recommendation', 'profile-long-term-recommendation'], playlist_types_not_to_update: list[str] = [])
+update_all_generated_playlists(K: int = None, playlist_types_to_update: list[str] = ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'short-term-profile-recommendation', 'medium-term-profile-recommendation', 'long-term-profile-recommendation'], playlist_types_not_to_update: list[str] = [])
 # Method Use Example
 api.update_all_generated_playlists()
 # or for example api.update_all_generated_playlists(playlist_types_to_update=['playlist-recommendation'])
 # Function updates all the playlists once generated by this package in batch
 # Note that if only a few updates are preferred, the methods above are a better fit
 # No parameters are mandatory but the default values should be noted, and if a value for K
 # is not specified, it takes as default the already existing playlist total song count which is recommended,
```

## Comparing `spotify_recommender_api-4.4.0.dist-info/RECORD` & `spotify_recommender_api-4.4.1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-spotify_recommender_api/__init__.py,sha256=b5pft4em-htNwFd_2QKFzVlJsxU49kJdOhieNIZ8HVc,21
+spotify_recommender_api/__init__.py,sha256=jE7Hja-Saozkka8sEZeybOD8E6vMn9F1pXhgRC7q-YM,21
 spotify_recommender_api/authentication.py,sha256=jQ49ZXeZ9Vj6x76aooA7uQ09xRRETmMDYCfeRw0TaPQ,1263
-spotify_recommender_api/core.py,sha256=PniP9b2gl_PBRU74Z94cFxvSVh7htbWvw0LJQBLrFgA,15397
+spotify_recommender_api/core.py,sha256=e33Q3Cs_Q-jUcjRzGJRIOIG7YQTVPtWZOzdn19wGikw,15410
 spotify_recommender_api/error.py,sha256=BBG5MUYuoAGElBAV058H6o13R-bYR_sGGgjAT1r7lCg,2042
-spotify_recommender_api/recommender.py,sha256=WiQ3mzwLu226h87QSGfOQ5nsbxoIzlfzF0NQNBuPbSw,116978
+spotify_recommender_api/recommender.py,sha256=kGpSNiNbQA9PHoMbNDs4YYhtVzbFz9e1Z49IEdYsxAg,116945
 spotify_recommender_api/request_handler.py,sha256=f9aqL1s_Kjqvf5NUeDkvJfVC8xgEcLjBq61aO3wdmkk,6306
 spotify_recommender_api/sensitive.py,sha256=Xn2FFn4uUk94Ei_It1U2iT5ZZEafHBt9q--lSPwlaoI,99
 spotify_recommender_api/server.py,sha256=Jq90Sd6GrI4txMaLFDcNoThy3jSWe8MwVUIvQXSkkYQ,6722
 spotify_recommender_api/util.py,sha256=YKe6uhOml0kvsjt9ciXEpuRhPh4uZfi3uik9xzPvYaw,9726
-spotify_recommender_api-4.4.0.dist-info/METADATA,sha256=YXa0S1IjXBVt8rCqI1laANwbIjHWuJu09O3N3mu7jlA,21574
-spotify_recommender_api-4.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-spotify_recommender_api-4.4.0.dist-info/top_level.txt,sha256=X65Ob3YNye88oWqQCXBvKpEUdmLQvio-wg4Ra2Gsh-c,24
-spotify_recommender_api-4.4.0.dist-info/RECORD,,
+spotify_recommender_api-4.4.1.dist-info/METADATA,sha256=8eFHiOy52QO83p0rHuHiNadf6INestg6GAKfLf78OC4,21574
+spotify_recommender_api-4.4.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+spotify_recommender_api-4.4.1.dist-info/top_level.txt,sha256=X65Ob3YNye88oWqQCXBvKpEUdmLQvio-wg4Ra2Gsh-c,24
+spotify_recommender_api-4.4.1.dist-info/RECORD,,
```

