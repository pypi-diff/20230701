# Comparing `tmp/spotify_recommender_api-4.3.1-py3-none-any.whl.zip` & `tmp/spotify_recommender_api-4.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 40747 bytes, number of entries: 13
--rw-rw-r--  2.0 unx       21 b- defN 23-Jun-23 14:38 spotify_recommender_api/__init__.py
--rw-rw-r--  2.0 unx     1262 b- defN 23-Jun-23 14:31 spotify_recommender_api/authentication.py
--rw-rw-r--  2.0 unx    15037 b- defN 23-Jun-23 14:31 spotify_recommender_api/core.py
+Zip file size: 41895 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx       21 b- defN 23-Jul-01 13:50 spotify_recommender_api/__init__.py
+-rw-rw-r--  2.0 unx     1263 b- defN 23-Jul-01 13:50 spotify_recommender_api/authentication.py
+-rw-rw-r--  2.0 unx    15397 b- defN 23-Jul-01 14:16 spotify_recommender_api/core.py
 -rw-rw-r--  2.0 unx     2042 b- defN 23-Jun-23 14:32 spotify_recommender_api/error.py
--rw-rw-r--  2.0 unx   111983 b- defN 23-Jun-23 14:37 spotify_recommender_api/recommender.py
--rw-rw-r--  2.0 unx     6305 b- defN 23-Jun-23 14:31 spotify_recommender_api/request_handler.py
+-rw-rw-r--  2.0 unx   116978 b- defN 23-Jul-01 14:24 spotify_recommender_api/recommender.py
+-rw-rw-r--  2.0 unx     6306 b- defN 23-Jul-01 13:51 spotify_recommender_api/request_handler.py
 -rw-rw-r--  2.0 unx       99 b- defN 22-Jun-25 22:21 spotify_recommender_api/sensitive.py
--rw-rw-r--  2.0 unx     6720 b- defN 23-Jun-23 14:32 spotify_recommender_api/server.py
--rw-rw-r--  2.0 unx     9510 b- defN 23-Jun-23 14:32 spotify_recommender_api/util.py
--rw-rw-r--  2.0 unx    21409 b- defN 23-Jun-23 14:40 spotify_recommender_api-4.3.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-23 14:40 spotify_recommender_api-4.3.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       24 b- defN 23-Jun-23 14:40 spotify_recommender_api-4.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1194 b- defN 23-Jun-23 14:40 spotify_recommender_api-4.3.1.dist-info/RECORD
-13 files, 175698 bytes uncompressed, 38715 bytes compressed:  78.0%
+-rw-rw-r--  2.0 unx     6722 b- defN 23-Jul-01 13:51 spotify_recommender_api/server.py
+-rw-rw-r--  2.0 unx     9726 b- defN 23-Jul-01 14:17 spotify_recommender_api/util.py
+-rw-rw-r--  2.0 unx    21574 b- defN 23-Jul-01 14:26 spotify_recommender_api-4.4.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-01 14:26 spotify_recommender_api-4.4.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       24 b- defN 23-Jul-01 14:26 spotify_recommender_api-4.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1194 b- defN 23-Jul-01 14:26 spotify_recommender_api-4.4.0.dist-info/RECORD
+13 files, 181438 bytes uncompressed, 39863 bytes compressed:  78.0%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: spotify_recommender_api/server.py
 Comment: 
 
 Filename: spotify_recommender_api/util.py
 Comment: 
 
-Filename: spotify_recommender_api-4.3.1.dist-info/METADATA
+Filename: spotify_recommender_api-4.4.0.dist-info/METADATA
 Comment: 
 
-Filename: spotify_recommender_api-4.3.1.dist-info/WHEEL
+Filename: spotify_recommender_api-4.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: spotify_recommender_api-4.3.1.dist-info/top_level.txt
+Filename: spotify_recommender_api-4.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: spotify_recommender_api-4.3.1.dist-info/RECORD
+Filename: spotify_recommender_api-4.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spotify_recommender_api/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '4.3.1'
+__version__ = '4.4.0'
```

## spotify_recommender_api/authentication.py

```diff
@@ -1,10 +1,11 @@
 import os
 import logging
 import spotify_recommender_api.request_handler as requests
+
 from spotify_recommender_api.server import up_server
 
 
 def get_auth() -> str:
     """Function to retrieve the authentication token for the first time in the execution
 
     Returns:
```

## spotify_recommender_api/core.py

```diff
@@ -2,15 +2,17 @@
 import logging
 import datetime
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 import spotify_recommender_api.util as util
 import spotify_recommender_api.request_handler as requests
+
 from typing import Union, Any
+
 sns.set()
 
 
 def list_distance(indexed_genre_list_a: 'list[int]', indexed_genre_list_b: 'list[int]') -> float:
     """The weighted algorithm that calculates the distance between two songs according to either the distance between each song list of genres or the distance between each song list of artists
 
     Note:
@@ -168,16 +170,16 @@
 
     elif type == 'artist':
         playlist_name = f"This once was {additional_info!r}"
         description = f'''{additional_info}'{"" if additional_info[-1] == "s" else "s"} songs, within the playlist {base_playlist_name}'''
 
     elif type == 'profile-recommendation':
         criteria = additional_info[0] if additional_info[0] != 'mixed' else 'genres, tracks and artists'
-        playlist_name = "Profile Recommendation"
-        description = f'''Profile-based recommendations based on favorite {criteria}'''
+        playlist_name = f"Profile {additional_info[2].replace('_', ' ').capitalize()} Recommendation"
+        description = f'''Profile-based {additional_info[2].replace('_', ' ')} recommendations based on favorite {criteria}'''
 
         if additional_info[1]:
             now = datetime.datetime.now(tz=pytz.timezone('UTC'))
             playlist_name += f' ({criteria} - {now.strftime("%Y-%m-%d")})'
             description += f' - {now.strftime("%Y-%m-%d")} snapshot'
         else:
             playlist_name += f' ({criteria})'
@@ -202,41 +204,47 @@
     elif type == 'mood':
         playlist_name = f"{additional_info[0]} Songs".capitalize()
         description = f'Songs related to the mood "{additional_info[0]}"{", excluding the mostly instrumental songs" if additional_info[1] else ""}, within the playlist {base_playlist_name}'
 
     else:
         raise ValueError('type not valid')
 
-    if playlist_id_found := util.playlist_exists(name=playlist_name, base_playlist_name=base_playlist_name, headers=headers, _update_created_playlists=_update_created_playlists):
-        new_id = playlist_id_found
+    if playlist_found := util.playlist_exists(name=playlist_name, base_playlist_name=base_playlist_name, headers=headers, _update_created_playlists=_update_created_playlists):
+        new_id = playlist_found[0]
 
         playlist_tracks = list(map(lambda track: {'uri': track['track']['uri']}, requests.get_request(
             url=f'https://api.spotify.com/v1/playlists/{new_id}/tracks', headers=headers).json()['items']))
 
         delete_json = requests.delete_request(
             url=f'https://api.spotify.com/v1/playlists/{new_id}/tracks', headers=headers, data={"tracks": playlist_tracks}).json()
 
-        if _update_created_playlists:
+        if (
+            _update_created_playlists or
+            (
+                playlist_name.lower().startswith('profile short term recommendation') and
+                playlist_found[1] == playlist_name.replace('Short term ', '')
+            )
+        ):
             data = {
                 "name": playlist_name,
                 "description": description,
                 "public": False
             }
 
-            update_playlist_details = requests.put_request(
-                url=f'https://api.spotify.com/v1/playlists/{new_id}', headers=headers, data=data)
+            logging.info(f'Updating playlist {playlist_found[1]} details')
+
+            update_playlist_details = requests.put_request(url=f'https://api.spotify.com/v1/playlists/{new_id}', headers=headers, data=data)
 
     else:
         data = {
             "name": playlist_name,
             "description": description,
             "public": False
         }
-        playlist_creation = requests.post_request(
-            url=f'https://api.spotify.com/v1/users/{user_id}/playlists', headers=headers, data=data)
+        playlist_creation = requests.post_request(url=f'https://api.spotify.com/v1/users/{user_id}/playlists', headers=headers, data=data)
         new_id = playlist_creation.json()['id']
 
     return new_id
 
 
 def create_playlist_data_dict(row) -> dict:
     """Function to be applied to the pandas DataFrame to create a dictionary with each row's information
```

## spotify_recommender_api/recommender.py

```diff
@@ -4,17 +4,19 @@
 import operator
 import warnings
 import pandas as pd
 import spotify_recommender_api.util as util
 import spotify_recommender_api.core as core
 import spotify_recommender_api.authentication as auth
 import spotify_recommender_api.request_handler as requests
+
 from functools import reduce
 from typing import Any, Union
 from spotify_recommender_api.error import AccessTokenExpiredError
+
 warnings.filterwarnings('error')
 
 
 class SpotifyAPI:
     """
     Spotify API is the Class that provides access to the playlists recommendations
     """
@@ -475,15 +477,16 @@
             'artist': getattr(self, '_SpotifyAPI__artist_name', None),
             'mood': [
                 getattr(self, '_SpotifyAPI__mood', None),
                 getattr(self, '_SpotifyAPI__exclude_mostly_instrumental', None),
             ],
             'profile-recommendation': [
                 getattr(self, '_SpotifyAPI__profile_recommendation_criteria', None),
-                getattr(self, '_SpotifyAPI__profile_recommendation_date', None)
+                getattr(self, '_SpotifyAPI__profile_recommendation_date', None),
+                getattr(self, '_SpotifyAPI__profile_recommendation_time_range', None)
             ],
             'playlist-recommendation': [
                 getattr(self, '_SpotifyAPI__playlist_recommendation_criteria', None),
                 getattr(self, '_SpotifyAPI__playlist_recommendation_date', None),
                 getattr(self, '_SpotifyAPI__playlist_recommendation_time_range', None)
             ],
             'general-recommendation': [
@@ -1032,15 +1035,22 @@
             bool: The flag that indicates whether the playlist should be updated or not
         """
         _, name, description, _ = playlist
 
         if name in {'Long Term Most-listened Tracks', 'Medium Term Most-listened Tracks', 'Short Term Most-listened Tracks'} and 'most-listened-tracks' in playlist_types_to_update:
             return True
 
-        elif 'Profile Recommendation' in name and ' - 20' not in name and 'profile-recommendation' in playlist_types_to_update:
+        elif (
+            ' - 20' not in name and
+            all(word in name for word in {'Profile', 'Recommendation'}) and
+            any(
+                playlist_type in playlist_types_to_update
+                for playlist_type in {'profile-short-term-recommendation', 'profile-medium-term-recommendation', 'profile-long-term-recommendation'}
+            )
+        ):
             return True
 
         elif f', within the playlist {self.__base_playlist_name}' in description or self.__update_created_files:
             if (re.match(r"\'(.*?)\' Related", name) or re.match(r'\"(.*?)\" Related', name)) and 'song-related' in playlist_types_to_update:
                 return True
 
             elif (re.match(r"\'(.*?)\' Mix", name) or re.match(r'\"(.*?)\" Mix', name)) and 'artist-mix' in playlist_types_to_update:
@@ -1053,24 +1063,49 @@
                 return True
 
             elif 'Songs related to the mood' in description and 'mood' in playlist_types_to_update:
                 return True
 
         return False
 
-    def update_all_generated_playlists(self, *, K: Union[int, None] = None, playlist_types_to_update: Union['list[str]', None] = None):
+    def update_all_generated_playlists(
+            self, *,
+            K: Union[int, None] = None,
+            playlist_types_to_update: Union['list[str]', None] = None,
+            playlist_types_not_to_update: Union['list[str]', None] = None
+        ) -> None:
         """Update all package generated playlists in batch
 
         Note:
             It is NOT recommended to use the K parameter in this function, unless 100% on purpose, since it will make all the playlists have the same number of songs in them
+
+        Arguments:
             K (int, optional): Number of songs in the new playlists, if not set, defaults to the number of songs already in the playlist. Defaults to None.
-            playlist_types_to_update (list[str], optional): List of playlist types to update. For example, if you only want to update song-related playlists use this argument as ['song-related']. Defaults to all - ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'profile-recommendation', 'mood'].
+            playlist_types_to_update (list[str], optional): List of playlist types to update. For example, if you only want to update song-related playlists use this argument as ['song-related']. Defaults to all == ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'profile-short-term-recommendation', 'profile-medium-term-recommendation', 'profile-long-term-recommendation', 'mood'].
+            playlist_types_not_to_update (list[str], optional): List of playlist types not to update. For example, if you want to update all playlists but song-related playlists use this argument as ['song-related']. it can be used alongside with the playlist_types_to_update but it can become confusing or redundant. Defaults to none == [].
         """
         if playlist_types_to_update is None:
-            playlist_types_to_update = ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'profile-recommendation', 'mood']
+            playlist_types_to_update = ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'profile-short-term-recommendation', 'profile-medium-term-recommendation', 'profile-long-term-recommendation', 'mood']
+
+        if playlist_types_not_to_update is None:
+            playlist_types_not_to_update = []
+
+        playlist_types_to_update = [playlist_type for playlist_type in playlist_types_to_update if playlist_type not in playlist_types_not_to_update]
+
+        if 'profile-recommendation' in playlist_types_to_update:
+            logging.info('After version 4.4.0, the profile-recommendation playlists are separated in short, medium and long term. See the update_all_created_playlists docstring or the documentation at: https://github.com/nikolas-virionis/spotify-api')
+            playlist_types_to_update.remove('profile-recommendation')
+            for playlist_type in {'profile-short-term-recommendation', 'profile-medium-term-recommendation', 'profile-long-term-recommendation'}:
+                if playlist_type not in playlist_types_to_update:
+                    playlist_types_to_update.append(playlist_type)
+
+        if 'profile-recommendation' in playlist_types_not_to_update:
+            for playlist_type in {'profile-recommendation', 'profile-short-term-recommendation', 'profile-medium-term-recommendation', 'profile-long-term-recommendation'}:
+                if playlist_type in playlist_types_to_update:
+                    playlist_types_to_update.remove(playlist_type)
 
         total_playlist_count = requests.get_request(url='https://api.spotify.com/v1/me/playlists?limit=0', headers=self.__headers).json()['total']
 
         playlists = []
 
         for offset in range(0, total_playlist_count, 50):
             request = requests.get_request(url=f'https://api.spotify.com/v1/me/playlists?limit=50&{offset=!s}',  headers=self.__headers).json()
@@ -1084,15 +1119,15 @@
                         playlist=playlist,
                         playlist_types_to_update=playlist_types_to_update
                 )
             ]
 
         last_printed_perc_update = 0
 
-        for index, (_, name, description, total_tracks) in enumerate(playlists):
+        for index, (playlist_id, name, description, total_tracks) in enumerate(playlists):
             try:
                 logging.debug(f'Updating song {name} - {index}/{len(playlists)}')
                 if last_printed_perc_update + 10 <= (perc_update := next((perc for perc in range(100, 0, -10) if (100 * index) / len(playlists) >= perc), 100)) < 100:
                     logging.info(f'Playlists update operation at {perc_update}%')
                     last_printed_perc_update = perc_update
 
                 if K is not None:
@@ -1126,14 +1161,20 @@
                             build_playlist=True,
                             artist_name=artist_name,
                             complete_with_similar=False,
                             ensure_all_artist_songs=f'All {artist_name}' in description,
                             _auto=True
                         )
 
+                    # elif name == 'Recent-ish Favorites':
+                    #     self.__write_playlist(type='medium', K=total_tracks)
+
+                    # elif name == 'Latest Favorites':
+                    #     self.__write_playlist(type='short', K=total_tracks)
+
                     elif 'Playlist Recommendation' in name and ' - 20' not in name and 'playlist-recommendation' in playlist_types_to_update:
                         criteria = name.split('(')[1].split(')')[0]
                         if ',' in criteria:
                             criteria = 'mixed'
 
                         time_range = 'all_time' if 'for all_time' in name else name.split('for the last')[-1].split('(')[0].strip()
 
@@ -1152,30 +1193,61 @@
                         self.get_songs_by_mood(
                             mood=mood,
                             K=total_tracks,
                             build_playlist=True,
                             exclude_mostly_instrumental=exclude_mostly_instrumental,
                         )
 
-                elif 'Profile Recommendation' in name and ' - 20' not in name and 'profile-recommendation' in playlist_types_to_update:
+                elif (
+                    ' - 20' not in name and
+                    all(word in name for word in {'Profile', 'Recommendation'}) and
+                    any(
+                        playlist_type in playlist_types_to_update
+                        for playlist_type in {'profile-short-term-recommendation', 'profile-medium-term-recommendation', 'profile-long-term-recommendation'}
+                    )
+                ):
                     criteria = name.split('(')[1].split(')')[0]
+                    criteria_name = criteria
+
                     if ',' in criteria:
                         criteria = 'mixed'
 
+                    if 'term' in name.lower():
+                        time_range = '_'.join(name.split(' ')[1:3]).lower()
+                    else:
+                        time_range = 'short_term'
+                        playlist_name = f"Profile {time_range.replace('_', ' ').capitalize()} Recommendation ({criteria_name})"
+                        description = f'''Profile-based {time_range.replace('_', ' ')} recommendations based on favorite {criteria_name}'''
+
+                        data = {
+                            "name": playlist_name,
+                            "description": description,
+                            "public": False
+                        }
+
+                        logging.info(f'Updating the name and description of the playlist {name} because of new time range specifications added to the profile_recommendation function in version 4.4.0')
+                        logging.info('In case of any problems with the feature, submit an issue at: https://github.com/nikolas-virionis/spotify-api/issues')
+
+                        update_playlist_details = requests.put_request(url=f'https://api.spotify.com/v1/playlists/{playlist_id}', headers=self.__headers, data=data)
+
+                    if f"profile-{time_range.replace('_', '-')}-recommendation" not in playlist_types_to_update:
+                        continue
+
                     self.get_profile_recommendation(
                         K=total_tracks,
                         build_playlist=True,
+                        time_range=time_range,
                         main_criteria=criteria,
                     )
 
-                logging.info('Playlists update operation at 100%')
-
             except ValueError as e:
                 logging.error(f"Unfortunately we couldn't update a playlist because\n {e}")
 
+        logging.info('Playlists update operation at 100%')
+
     def get_playlist_trending_genres(self, time_range: str = 'all_time', plot_top: 'int|bool' = False) -> Union[pd.DataFrame, None]:
         """Calculates the amount of times each genre was spotted in the playlist, and can plot a bar chart to represent this information
 
         Args:
             time_range (str, optional): Time range that represents how much of the playlist will be considered for the trend. Can be one of the following: 'all_time', 'month', 'trimester', 'semester', 'year'. Defaults to 'all_time'.
             plot_top(int|bool , optional): the number of top genres to be plotted. Must be 5, 10, 15 or False. No chart will be plotted if set to False. Defaults to False.
 
@@ -1693,41 +1765,46 @@
             'mean_loudness': df['loudness'].mean(),
             'min_instrumentalness': df['instrumentalness'].min(),
             'max_instrumentalness': df['instrumentalness'].max(),
             'mean_instrumentalness': df['instrumentalness'].mean(),
         }
 
     def get_profile_recommendation(
-        self,
-        K: int = 50,
-        main_criteria: str = 'mixed',
-        save_with_date: bool = False,
-        build_playlist: bool = False,
-    ) -> Union[pd.DataFrame, None]:
+            self,
+            K: int = 50,
+            main_criteria: str = 'mixed',
+            save_with_date: bool = False,
+            build_playlist: bool = False,
+            time_range: str = 'short_term'
+        ) -> Union[pd.DataFrame, None]:
         """Builds a Profile based recommendation
 
         Args:
             K (int, optional): Number of songs in the recommendations playlist. Defaults to 50.
             main_criteria (str, optional): Main criteria for the recommendations playlist. Can be one of the following: 'mixed', 'artists', 'tracks', 'genres'. Defaults to 'mixed'.
             save_with_date (bool, optional): Flag to save the recommendations playlist as a Point in Time Snapshot. Defaults to False.
             build_playlist (bool, optional): Flag to build the recommendations playlist in the users library. Defaults to False.
+            time_range (str, optional): The time range to get the profile most listened information from. Can be one of the following: 'short_term', 'medium_term', 'long_term'. Defaults to 'short_term'
 
         Raises:
             ValueError: K must be between 1 and 100
             ValueError: 'mixed', 'artists', 'tracks', 'genres'
+            ValueError: time_range needs to be one of the following: 'short_term', 'medium_term', 'long_term'
 
         Returns:
             pd.DataFrame: Recommendations playlist
         """
         if not (1 < K <= 100):
             raise ValueError('K must be between 1 and 100')
 
-        if main_criteria not in ['mixed', 'artists', 'tracks', 'genres']:
-            raise ValueError(
-                "main_criteria must be one of the following: 'mixed', 'artists', 'tracks', 'genres'")
+        if main_criteria not in {'mixed', 'artists', 'tracks', 'genres'}:
+            raise ValueError("main_criteria must be one of the following: 'mixed', 'artists', 'tracks', 'genres'")
+
+        if time_range not in {'short_term', 'medium_term', 'long_term'}:
+            raise ValueError("time_range needs to be one of the following: 'short_term', 'medium_term', 'long_term'")
 
         tracks = []
         genres = []
         artists = []
 
         for _ in range(2):
             try:
@@ -1735,15 +1812,17 @@
                 if main_criteria != 'tracks':
                     if self.__top_genres or self.__top_artists:
                         genres = self.__top_genres
                         artists = self.__top_artists
 
                     else:
                         top_artists_req = requests.get_request(
-                            url='https://api.spotify.com/v1/me/top/artists?time_range=short_term&limit=5', headers=self.__headers).json()['items']
+                            headers=self.__headers,
+                            url=f'https://api.spotify.com/v1/me/top/artists?time_range={time_range}&limit=5',
+                        ).json()['items']
 
                         artists = [artist['id'] for artist in top_artists_req]
                         genres = list(set(reduce(lambda x, y: x + y, [artist['genres'] for artist in top_artists_req], [])))[:5]
                         self.__top_genres = genres
                         self.__top_artists = artists
 
                 if main_criteria not in ['artists']:
@@ -1751,15 +1830,15 @@
                         tracks = self.__top_tracks
 
                     else:
                         tracks = [
                             track['id']
                             for track in requests.get_request(
                                 headers=self.__headers,
-                                url='https://api.spotify.com/v1/me/top/tracks?time_range=short_term&limit=5'
+                                url=f'https://api.spotify.com/v1/me/top/tracks?time_range={time_range}&limit=5'
                             ).json()['items']
                         ]
 
                         self.__top_tracks = tracks
 
                 url = f'https://api.spotify.com/v1/recommendations?limit={K}'
 
@@ -1800,14 +1879,15 @@
 
                 recommendations_playlist = pd.DataFrame(data=songs)
 
                 ids = recommendations_playlist['id'].tolist()
 
                 if build_playlist:
                     self.__profile_recommendation_date = save_with_date
+                    self.__profile_recommendation_time_range = time_range
                     self.__profile_recommendation_criteria = main_criteria
 
                     self.__write_playlist(
                         K=K,
                         type='profile-recommendation',
                         additional_info=ids
                     )
```

## spotify_recommender_api/request_handler.py

```diff
@@ -1,11 +1,12 @@
 import json
 import time
 import logging
 import requests
+
 from typing import Union
 from spotify_recommender_api.error import HTTPRequestError, TooManyRequestsError, AccessTokenExpiredError
 
 
 def exponential_backoff(func, retries: int = 5, *args, **kwargs) -> requests.Response:
     """Exponential backoff strategy (https://en.wikipedia.org/wiki/Exponential_backoff)
     in order to retry certain function after exponetially increasing delay, to overcome "429: Too Many Requests" error
```

## spotify_recommender_api/server.py

```diff
@@ -1,17 +1,19 @@
 
 import time
 import uvicorn
 import threading
 import webbrowser
 import contextlib
+
 from fastapi import FastAPI, status
 from fastapi.responses import HTMLResponse
 from spotify_recommender_api.sensitive import CLIENT_ID, CLIENT_SECRET
 from spotify_recommender_api.request_handler import post_request_with_auth
+
 app = FastAPI()
 
 redirect_uri = 'http://localhost:8000/callback'
 scope = ["playlist-modify-private", "playlist-read-private", "user-library-read", "user-library-modify", "user-top-read"]
 
 class Server(uvicorn.Server):
     """Subclass of uvicorn.Server so that the run and shutdown methods can be done while running in a separate thread
```

## spotify_recommender_api/util.py

```diff
@@ -1,13 +1,14 @@
 import logging
 import warnings
 import datetime
 import functools
 import pandas as pd
 import spotify_recommender_api.request_handler as requests
+
 from dateutil import tz
 from typing import Union, Any
 
 
 def playlist_url_to_id(url: str) -> str:
     """Extracts the playlist id from it's URL
 
@@ -73,51 +74,55 @@
     Returns:
         list[int]: indexed list of items in binary format in comparison to all the items inside the playlist
     """
 
     return [str(int(all_genres_x in items)) for all_genres_x in all_items]
 
 
-def playlist_exists(name: str, base_playlist_name: str, headers: dict, _update_created_playlists: bool = False) -> 'str|bool':
+def playlist_exists(name: str, base_playlist_name: str, headers: dict, _update_created_playlists: bool = False) -> Union['tuple[str, str, str]', 'tuple[()]']:
     """Function used to check if a playlist exists inside the user's library
     Used before the creation of a new playlist
 
     Args:
         name (str): name of the playlist being created, which could easily be bypassed, if the playlist names were not made automatically
         base_playlist_name (str): name of the base playlist
         headers (dict): Request headers
 
     Returns:
         str|bool: If the playlist already exists, returns the id of the playlist, otherwise returns False
     """
-    total_playlist_count = requests.get_request(
-        url='https://api.spotify.com/v1/me/playlists?limit=1', headers=headers).json()['total']
+    total_playlist_count = requests.get_request(url='https://api.spotify.com/v1/me/playlists?limit=1', headers=headers).json()['total']
     playlists = []
     for offset in range(0, total_playlist_count, 50):
-        request = requests.get_request(
-            url=f'https://api.spotify.com/v1/me/playlists?limit=50&{offset=!s}',  headers=headers).json()
+        request = requests.get_request(url=f'https://api.spotify.com/v1/me/playlists?limit=50&{offset=!s}',  headers=headers).json()
 
-        playlists += list(map(lambda playlist: (
-            playlist['id'], playlist['name'], playlist['description']), request['items']))
+        playlists += list(map(lambda playlist: (playlist['id'], playlist['name'], playlist['description']), request['items']))
 
     return next(
         (
-            playlist[0] for playlist in playlists
-            if playlist[1] == name and
+            playlist for playlist in playlists
+            if (
+                playlist[1] == name or
+                (
+                    name.lower().startswith('profile short term recommendation') and
+                    playlist[1] == name.replace('Short term ', '')
+                )
+            ) and
             (
                 ' Term Most-listened Tracks' in name or
                 f', within the playlist {base_playlist_name}' in playlist[2] or
                 _update_created_playlists or
                 'Recommendation (' in name
             )
         ),
-        False
+        ()
     )
 
 
+
 def query_audio_features(song: pd.Series, headers: dict) -> 'list[float]':
     """Queries the audio features for a given song and returns the ones that match the recommendations within this package
 
     Args:
         song (pd.Series): song containing its base information
         headers (dict): Request headers
```

## Comparing `spotify_recommender_api-4.3.1.dist-info/METADATA` & `spotify_recommender_api-4.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-recommender-api
-Version: 4.3.1
+Version: 4.4.0
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
-update_all_generated_playlists(K: int = None, playlist_types_to_update: list[str] = ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'profile-recommendation'])
+update_all_generated_playlists(K: int = None, playlist_types_to_update: list[str] = ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'profile-short-term-recommendation', 'profile-medium-term-recommendation', 'profile-long-term-recommendation'], playlist_types_not_to_update: list[str] = [])
 # Method Use Example
 api.update_all_generated_playlists()
 # or for example api.update_all_generated_playlists(playlist_types_to_update=['playlist-recommendation'])
 # Function updates all the playlists once generated by this package in batch
 # Note that if only a few updates are preferred, the methods above are a better fit
 # No parameters are mandatory but the default values should be noted, and if a value for K
 # is not specified, it takes as default the already existing playlist total song count which is recommended,
@@ -215,15 +215,15 @@
 # Function that returns a dictionary containing the songs that have the maximum and minimum values
 # for the 5 audio features used in this package: ['danceability', 'energy', 'instrumentalness', 'tempo', 'valence']
 ~~~
  - get_profile_recommendation
 ~~~python
 # Parameters
 get_profile_recommendation(K: int = 50, main_criteria: str = 'mixed', save_with_date: bool = False,
-build_playlist: bool = False)
+build_playlist: bool = False, time_range: str = 'short_term')
 # Method Use Example
 api.get_profile_recommendation(build_playlist=True)
 # Function that returns a pandas DataFrame with profile-based recommendations, and creates it in the user account
 # main_criteria is the base info to get the recommendations
 # save_with_date is a flag to save the recommendations as a playlist at a point in time Snapshot
 # BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
 ~~~
@@ -256,15 +256,15 @@
 # Parameters
 select_playlist(user_id: str, playlist_id: str = None, playlist_url: str = None, liked_songs: bool = False)
 # Method Use Example
 api.select_playlist(user_id='USER_ID', liked_songs=True)
 # Function to select a playlist to be mapped and be available on all the playlist-related recommendation
 # functions on an already existing authorization context
 ~~~~~~
- - select_playlist
+ - get_songs_by_mood
 ~~~python
 # Parameters
 get_songs_by_mood(mood: str, K: int = 50, build_playlist: bool = False, exclude_mostly_instrumental: bool = False)
 # Method Use Example
 api.get_songs_by_mood(mood='happy', build_playlist=True)
 # Function to create a playlist based on the general mood of its songs
 # BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
```

## Comparing `spotify_recommender_api-4.3.1.dist-info/RECORD` & `spotify_recommender_api-4.4.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-spotify_recommender_api/__init__.py,sha256=Jvv3z9N6oc9ScnAs6RuIUeoZBeRn4Ehcj0Uwtcb9TpE,21
-spotify_recommender_api/authentication.py,sha256=TnbdK0RDSKqO-NVRToEC5j41jtCKUIJnJNMPbKn0SsU,1262
-spotify_recommender_api/core.py,sha256=Ykaj7Syo5NE1YDAz0tzHGsMYxheZSt-PJXCuK3SBiOM,15037
+spotify_recommender_api/__init__.py,sha256=b5pft4em-htNwFd_2QKFzVlJsxU49kJdOhieNIZ8HVc,21
+spotify_recommender_api/authentication.py,sha256=jQ49ZXeZ9Vj6x76aooA7uQ09xRRETmMDYCfeRw0TaPQ,1263
+spotify_recommender_api/core.py,sha256=PniP9b2gl_PBRU74Z94cFxvSVh7htbWvw0LJQBLrFgA,15397
 spotify_recommender_api/error.py,sha256=BBG5MUYuoAGElBAV058H6o13R-bYR_sGGgjAT1r7lCg,2042
-spotify_recommender_api/recommender.py,sha256=9Bkq47ks65IvK8idTkxgOVrCPhMupt6uafqZOffTPN0,111983
-spotify_recommender_api/request_handler.py,sha256=iBKnJCky25FqTpOmcK89JSp4DFltElI0sTHZudMBWik,6305
+spotify_recommender_api/recommender.py,sha256=WiQ3mzwLu226h87QSGfOQ5nsbxoIzlfzF0NQNBuPbSw,116978
+spotify_recommender_api/request_handler.py,sha256=f9aqL1s_Kjqvf5NUeDkvJfVC8xgEcLjBq61aO3wdmkk,6306
 spotify_recommender_api/sensitive.py,sha256=Xn2FFn4uUk94Ei_It1U2iT5ZZEafHBt9q--lSPwlaoI,99
-spotify_recommender_api/server.py,sha256=GpQ1gQ-q00RN-mqPj969TCn831VgGFVirqjCzx8NJVs,6720
-spotify_recommender_api/util.py,sha256=fGw8QMrCoy_7FW8xD_2BdJ0bUHE4mj8rm0gqa1dxNwU,9510
-spotify_recommender_api-4.3.1.dist-info/METADATA,sha256=P3IeofOsHMyBg9iKKGfYEyLlbwucNCuPihL15PrZJow,21409
-spotify_recommender_api-4.3.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-spotify_recommender_api-4.3.1.dist-info/top_level.txt,sha256=X65Ob3YNye88oWqQCXBvKpEUdmLQvio-wg4Ra2Gsh-c,24
-spotify_recommender_api-4.3.1.dist-info/RECORD,,
+spotify_recommender_api/server.py,sha256=Jq90Sd6GrI4txMaLFDcNoThy3jSWe8MwVUIvQXSkkYQ,6722
+spotify_recommender_api/util.py,sha256=YKe6uhOml0kvsjt9ciXEpuRhPh4uZfi3uik9xzPvYaw,9726
+spotify_recommender_api-4.4.0.dist-info/METADATA,sha256=YXa0S1IjXBVt8rCqI1laANwbIjHWuJu09O3N3mu7jlA,21574
+spotify_recommender_api-4.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+spotify_recommender_api-4.4.0.dist-info/top_level.txt,sha256=X65Ob3YNye88oWqQCXBvKpEUdmLQvio-wg4Ra2Gsh-c,24
+spotify_recommender_api-4.4.0.dist-info/RECORD,,
```

