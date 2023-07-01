# Comparing `tmp/blizzardwarcraftapi-0.2.2.tar.gz` & `tmp/blizzardwarcraftapi-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blizzardwarcraftapi-0.2.2.tar", max compression
+gzip compressed data, was "blizzardwarcraftapi-0.2.3.tar", max compression
```

## Comparing `blizzardwarcraftapi-0.2.2.tar` & `blizzardwarcraftapi-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1003 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/BlizzardAuthToken.py
--rw-r--r--   0        0        0     1796 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/BlizzardWarcraftAPI.py
--rw-r--r--   0        0        0      139 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/__init__.py
--rw-r--r--   0        0        0      609 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/data.py
--rw-r--r--   0        0        0      292 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/exceptions.py
--rw-r--r--   0        0        0     1935 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py
--rw-r--r--   0        0        0     1072 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/__init__.py
--rw-r--r--   0        0        0     2195 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/gameData/AchievementAPI.py
--rw-r--r--   0        0        0     1694 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/gameData/AuctionHouseAPI.py
--rw-r--r--   0        0        0     2056 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/gameData/ConnectedRealmAPI.py
--rw-r--r--   0        0        0     3764 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/gameData/CreatureAPI.py
--rw-r--r--   0        0        0     1339 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/gameData/GuildCrestAPI.py
--rw-r--r--   0        0        0      827 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/gameData/HeirloomAPI.py
--rw-r--r--   0        0        0     3652 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/gameData/ItemAPI.py
--rw-r--r--   0        0        0     3420 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/gameData/JournalAPI.py
--rw-r--r--   0        0        0        0 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/gameData/__init__.py
--rw-r--r--   0        0        0     1271 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/profile/CharacterAchievementsAPI.py
--rw-r--r--   0        0        0      683 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/profile/CharacterAppearanceAPI.py
--rw-r--r--   0        0        0     2965 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/profile/CharacterCollectionsAPI.py
--rw-r--r--   0        0        0     1766 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/profile/CharacterEncountersAPI.py
--rw-r--r--   0        0        0      670 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/profile/CharacterEquipmentAPI.py
--rw-r--r--   0        0        0      746 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/profile/CharacterHunterPetsAPI.py
--rw-r--r--   0        0        0      715 2023-06-25 21:10:14.781305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/profile/CharacterMediaAPI.py
--rw-r--r--   0        0        0     1544 2023-06-25 21:10:14.785305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/profile/CharacterMythicKeystoneProfile.py
--rw-r--r--   0        0        0      680 2023-06-25 21:10:14.785305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/profile/CharacterProfessionsAPI.py
--rw-r--r--   0        0        0        0 2023-06-25 21:10:14.785305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/profile/__init__.py
--rw-r--r--   0        0        0      421 2023-06-25 21:10:14.785305 blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/urls.py
--rw-r--r--   0        0        0     1066 2023-06-25 21:10:14.785305 blizzardwarcraftapi-0.2.2/LICENSE
--rw-r--r--   0        0        0     2034 2023-06-25 21:10:14.785305 blizzardwarcraftapi-0.2.2/README.md
--rw-r--r--   0        0        0      916 2023-06-25 21:10:14.785305 blizzardwarcraftapi-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2980 1970-01-01 00:00:00.000000 blizzardwarcraftapi-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1003 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/BlizzardAuthToken.py
+-rw-r--r--   0        0        0     1815 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/BlizzardWarcraftAPI.py
+-rw-r--r--   0        0        0      139 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/__init__.py
+-rw-r--r--   0        0        0      609 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/data.py
+-rw-r--r--   0        0        0      292 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/exceptions.py
+-rw-r--r--   0        0        0     1935 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py
+-rw-r--r--   0        0        0     1088 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/__init__.py
+-rw-r--r--   0        0        0     2195 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/gameData/AchievementAPI.py
+-rw-r--r--   0        0        0     1694 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/gameData/AuctionHouseAPI.py
+-rw-r--r--   0        0        0     2056 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/gameData/ConnectedRealmAPI.py
+-rw-r--r--   0        0        0     3764 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/gameData/CreatureAPI.py
+-rw-r--r--   0        0        0     1339 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/gameData/GuildCrestAPI.py
+-rw-r--r--   0        0        0      827 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/gameData/HeirloomAPI.py
+-rw-r--r--   0        0        0     3652 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/gameData/ItemAPI.py
+-rw-r--r--   0        0        0     3420 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/gameData/JournalAPI.py
+-rw-r--r--   0        0        0        0 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/gameData/__init__.py
+-rw-r--r--   0        0        0     4997 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/profile/AccountProfileAPI.py
+-rw-r--r--   0        0        0     1271 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/profile/CharacterAchievementsAPI.py
+-rw-r--r--   0        0        0      683 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/profile/CharacterAppearanceAPI.py
+-rw-r--r--   0        0        0     2965 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/profile/CharacterCollectionsAPI.py
+-rw-r--r--   0        0        0     1766 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/profile/CharacterEncountersAPI.py
+-rw-r--r--   0        0        0      670 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/profile/CharacterEquipmentAPI.py
+-rw-r--r--   0        0        0      746 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/profile/CharacterHunterPetsAPI.py
+-rw-r--r--   0        0        0      715 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/profile/CharacterMediaAPI.py
+-rw-r--r--   0        0        0     1544 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/profile/CharacterMythicKeystoneProfile.py
+-rw-r--r--   0        0        0      680 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/profile/CharacterProfessionsAPI.py
+-rw-r--r--   0        0        0        0 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/profile/__init__.py
+-rw-r--r--   0        0        0      421 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/urls.py
+-rw-r--r--   0        0        0     1066 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2034 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/README.md
+-rw-r--r--   0        0        0      916 2023-07-01 12:07:00.195842 blizzardwarcraftapi-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2980 1970-01-01 00:00:00.000000 blizzardwarcraftapi-0.2.3/PKG-INFO
```

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/BlizzardAuthToken.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/BlizzardAuthToken.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/BlizzardWarcraftAPI.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/BlizzardWarcraftAPI.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,14 @@
         def __init__(self):
             super().__init__(BlizzardWarcraftAPI.BlizzardAuthToken, BlizzardWarcraftAPI.region, BlizzardWarcraftAPI.locale)
 
     class Profile(CharacterAchievementsAPI, CharacterCollectionsAPI,
                   CharacterEquipmentAPI, CharacterEncountersAPI,
                   CharacterHunterPetsAPI, CharacterAppearanceAPI,
                   CharacterMediaAPI, CharacterProfessionsAPI,
-                  CharacterMythicKeystoneProfile):
+                  CharacterMythicKeystoneProfile, AccountProfileAPI):
         """
         The World of Warcraft profile APIs listed below encompass profile game data.
         https://develop.battle.net/documentation/world-of-warcraft/profile-apis
         """
         def __init__(self):
             super().__init__(BlizzardWarcraftAPI.BlizzardAuthToken, BlizzardWarcraftAPI.region, BlizzardWarcraftAPI.locale)
```

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/data.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/data.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/BlizzardWarcraftAPI_base.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/__init__.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .gameData.AchievementAPI import AchievementAPI
+from BlizzardWarcraftAPI.modules.gameData.AchievementAPI import AchievementAPI
 from .gameData.AuctionHouseAPI import AuctionHouseAPI
 from .gameData.ConnectedRealmAPI import ConnectedRealmAPI
 from .gameData.CreatureAPI import CreatureAPI
 from .gameData.GuildCrestAPI import GuildCrestAPI
 from .gameData.HeirloomAPI import HeirloomAPI
 from .gameData.JournalAPI import JournalAPI
 from .gameData.ItemAPI import ItemAPI
@@ -12,9 +12,8 @@
 from .profile.CharacterCollectionsAPI import CharacterCollectionsAPI
 from .profile.CharacterEncountersAPI import CharacterEncountersAPI
 from .profile.CharacterEquipmentAPI import CharacterEquipmentAPI
 from .profile.CharacterHunterPetsAPI import CharacterHunterPetsAPI
 from .profile.CharacterMediaAPI import CharacterMediaAPI
 from .profile.CharacterProfessionsAPI import CharacterProfessionsAPI
 from .profile.CharacterMythicKeystoneProfile import CharacterMythicKeystoneProfile
-
-from BlizzardWarcraftAPI.BlizzardAuthToken import BlizzardAuthToken
+from .profile.AccountProfileAPI import AccountProfileAPI
```

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/gameData/AchievementAPI.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/gameData/AchievementAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/gameData/AuctionHouseAPI.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/gameData/AuctionHouseAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/gameData/ConnectedRealmAPI.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/gameData/ConnectedRealmAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/gameData/CreatureAPI.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/gameData/CreatureAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/gameData/GuildCrestAPI.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/gameData/GuildCrestAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/gameData/HeirloomAPI.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/gameData/HeirloomAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/gameData/ItemAPI.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/gameData/ItemAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/gameData/JournalAPI.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/gameData/JournalAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/profile/CharacterAchievementsAPI.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/profile/CharacterAchievementsAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/profile/CharacterAppearanceAPI.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/profile/CharacterAppearanceAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/profile/CharacterCollectionsAPI.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/profile/CharacterCollectionsAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/profile/CharacterEncountersAPI.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/profile/CharacterEncountersAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/profile/CharacterEquipmentAPI.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/profile/CharacterEquipmentAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/profile/CharacterHunterPetsAPI.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/profile/CharacterHunterPetsAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/profile/CharacterMediaAPI.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/profile/CharacterMediaAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/profile/CharacterMythicKeystoneProfile.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/profile/CharacterMythicKeystoneProfile.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/BlizzardWarcraftAPI/modules/profile/CharacterProfessionsAPI.py` & `blizzardwarcraftapi-0.2.3/BlizzardWarcraftAPI/modules/profile/CharacterProfessionsAPI.py`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/LICENSE` & `blizzardwarcraftapi-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/README.md` & `blizzardwarcraftapi-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `blizzardwarcraftapi-0.2.2/pyproject.toml` & `blizzardwarcraftapi-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "BlizzardWarcraftAPI"
-version = "0.2.2"
+version = "0.2.3"
 authors = ["Angeloffy <angeloffy.work@gmail.com>"]
 maintainers = [
     "Angeloffy <angeloffy.work@gmail.com>",
     "Kotorkovsciy <kotorkovsciy@gmail.com>"
 ]
 description = "Warcraft API"
 readme = "README.md"
```

### Comparing `blizzardwarcraftapi-0.2.2/PKG-INFO` & `blizzardwarcraftapi-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blizzardwarcraftapi
-Version: 0.2.2
+Version: 0.2.3
 Summary: Warcraft API
 Home-page: https://github.com/Angeloffy/BlizzardWarcraftAPI/tree/main
 License: MIT
 Author: Angeloffy
 Author-email: angeloffy.work@gmail.com
 Maintainer: Angeloffy
 Maintainer-email: angeloffy.work@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: blizzardwarcraftapi Version: 0.2.2 Summary:
+Metadata-Version: 2.1 Name: blizzardwarcraftapi Version: 0.2.3 Summary:
 Warcraft API Home-page: https://github.com/Angeloffy/BlizzardWarcraftAPI/tree/
 main License: MIT Author: Angeloffy Author-email: angeloffy.work@gmail.com
 Maintainer: Angeloffy Maintainer-email: angeloffy.work@gmail.com Requires-
 Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

