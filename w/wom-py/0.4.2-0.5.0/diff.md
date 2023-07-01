# Comparing `tmp/wom_py-0.4.2.tar.gz` & `tmp/wom_py-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wom_py-0.4.2.tar", max compression
+gzip compressed data, was "wom_py-0.5.0.tar", max compression
```

## Comparing `wom_py-0.4.2.tar` & `wom_py-0.5.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1074 2023-06-16 02:46:15.366136 wom_py-0.4.2/LICENSE
--rw-r--r--   0        0        0     2712 2023-06-16 02:46:15.366136 wom_py-0.4.2/README.md
--rw-r--r--   0        0        0     2157 2023-06-16 02:46:15.370136 wom_py-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     4385 2023-06-16 02:46:15.450135 wom_py-0.4.2/wom/__init__.py
--rw-r--r--   0        0        0     1324 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/__main__.py
--rw-r--r--   0        0        0     1808 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/_cli.py
--rw-r--r--   0        0        0     8648 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/client.py
--rw-r--r--   0        0        0     1447 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/constants.py
--rw-r--r--   0        0        0     7388 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/enums.py
--rw-r--r--   0        0        0     1729 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/errors.py
--rw-r--r--   0        0        0     3228 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/__init__.py
--rw-r--r--   0        0        0     1557 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/base.py
--rw-r--r--   0        0        0     1673 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/competitions/__init__.py
--rw-r--r--   0        0        0     1591 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/competitions/enums.py
--rw-r--r--   0        0        0     7413 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/competitions/models.py
--rw-r--r--   0        0        0     1289 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/deltas/__init__.py
--rw-r--r--   0        0        0     1824 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/deltas/models.py
--rw-r--r--   0        0        0     1716 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/groups/__init__.py
--rw-r--r--   0        0        0     7780 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/groups/enums.py
--rw-r--r--   0        0        0     9275 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/groups/models.py
--rw-r--r--   0        0        0     1738 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/http.py
--rw-r--r--   0        0        0     1471 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/names/__init__.py
--rw-r--r--   0        0        0     1793 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/names/enums.py
--rw-r--r--   0        0        0     4894 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/names/models.py
--rw-r--r--   0        0        0     1754 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/players/__init__.py
--rw-r--r--   0        0        0     5686 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/players/enums.py
--rw-r--r--   0        0        0    11907 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/players/models.py
--rw-r--r--   0        0        0     1300 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/records/__init__.py
--rw-r--r--   0        0        0     2217 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/records/models.py
--rw-r--r--   0        0        0        0 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/py.typed
--rw-r--r--   0        0        0     5561 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/result.py
--rw-r--r--   0        0        0     6505 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/routes.py
--rw-r--r--   0        0        0    34477 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/serializer.py
--rw-r--r--   0        0        0     1709 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/services/__init__.py
--rw-r--r--   0        0        0     2050 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/services/base.py
--rw-r--r--   0        0        0    21170 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/services/competitions.py
--rw-r--r--   0        0        0     3528 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/services/deltas.py
--rw-r--r--   0        0        0     3688 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/services/efficiency.py
--rw-r--r--   0        0        0    24099 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/services/groups.py
--rw-r--r--   0        0        0     5772 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/services/http.py
--rw-r--r--   0        0        0     4031 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/services/names.py
--rw-r--r--   0        0        0    18088 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/services/players.py
--rw-r--r--   0        0        0     3506 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/services/records.py
--rw-r--r--   0        0        0     3828 1970-01-01 00:00:00.000000 wom_py-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-01 18:21:28.398859 wom_py-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2712 2023-07-01 18:21:28.398859 wom_py-0.5.0/README.md
+-rw-r--r--   0        0        0     2157 2023-07-01 18:21:28.398859 wom_py-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4438 2023-07-01 18:21:28.486856 wom_py-0.5.0/wom/__init__.py
+-rw-r--r--   0        0        0     1324 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/__main__.py
+-rw-r--r--   0        0        0     1808 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/_cli.py
+-rw-r--r--   0        0        0     8648 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/client.py
+-rw-r--r--   0        0        0     1447 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/constants.py
+-rw-r--r--   0        0        0     7388 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/enums.py
+-rw-r--r--   0        0        0     1729 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/errors.py
+-rw-r--r--   0        0        0     3281 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/models/__init__.py
+-rw-r--r--   0        0        0     1557 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/models/base.py
+-rw-r--r--   0        0        0     1673 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/models/competitions/__init__.py
+-rw-r--r--   0        0        0     1591 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/models/competitions/enums.py
+-rw-r--r--   0        0        0     7413 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/models/competitions/models.py
+-rw-r--r--   0        0        0     1289 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/models/deltas/__init__.py
+-rw-r--r--   0        0        0     1824 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/models/deltas/models.py
+-rw-r--r--   0        0        0     1740 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/groups/__init__.py
+-rw-r--r--   0        0        0     7780 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/groups/enums.py
+-rw-r--r--   0        0        0     9738 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/groups/models.py
+-rw-r--r--   0        0        0     1738 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/http.py
+-rw-r--r--   0        0        0     1471 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/names/__init__.py
+-rw-r--r--   0        0        0     1793 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/names/enums.py
+-rw-r--r--   0        0        0     4894 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/names/models.py
+-rw-r--r--   0        0        0     1783 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/players/__init__.py
+-rw-r--r--   0        0        0     5686 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/players/enums.py
+-rw-r--r--   0        0        0    12222 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/players/models.py
+-rw-r--r--   0        0        0     1300 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/records/__init__.py
+-rw-r--r--   0        0        0     2217 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/records/models.py
+-rw-r--r--   0        0        0        0 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/py.typed
+-rw-r--r--   0        0        0     5561 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/result.py
+-rw-r--r--   0        0        0     6596 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/routes.py
+-rw-r--r--   0        0        0    35491 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/serializer.py
+-rw-r--r--   0        0        0     1709 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/services/__init__.py
+-rw-r--r--   0        0        0     2050 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/services/base.py
+-rw-r--r--   0        0        0    21170 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/services/competitions.py
+-rw-r--r--   0        0        0     3528 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/services/deltas.py
+-rw-r--r--   0        0        0     3688 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/services/efficiency.py
+-rw-r--r--   0        0        0    24089 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/services/groups.py
+-rw-r--r--   0        0        0     5772 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/services/http.py
+-rw-r--r--   0        0        0     4031 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/services/names.py
+-rw-r--r--   0        0        0    20107 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/services/players.py
+-rw-r--r--   0        0        0     3506 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/services/records.py
+-rw-r--r--   0        0        0     3828 1970-01-01 00:00:00.000000 wom_py-0.5.0/PKG-INFO
```

### Comparing `wom_py-0.4.2/LICENSE` & `wom_py-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/README.md` & `wom_py-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/pyproject.toml` & `wom_py-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wom.py"
-version = "0.4.2"
+version = "0.5.0"
 description = "An asynchronous wrapper for the Wise Old Man API."
 authors = ["Jonxslays"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jonxslays/wom.py"
 repository = "https://github.com/Jonxslays/wom.py"
 documentation = "https://jonxslays.github.io/wom.py"
```

### Comparing `wom_py-0.4.2/wom/__init__.py` & `wom_py-0.5.0/wom/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,23 +28,23 @@
 """
 
 from __future__ import annotations
 
 from typing import Final
 
 __packagename__: Final[str] = "wom.py"
-__version__: Final[str] = "0.4.2"
+__version__: Final[str] = "0.5.0"
 __author__: Final[str] = "Jonxslays"
 __copyright__: Final[str] = "2023-present Jonxslays"
 __description__: Final[str] = "An asynchronous wrapper for the Wise Old Man API."
 __url__: Final[str] = "https://github.com/Jonxslays/wom.py"
 __docs__: Final[str] = "https://jonxslays.github.io/wom.py"
 __repository__: Final[str] = __url__
 __license__: Final[str] = "MIT"
-__git_sha__: Final[str] = "[ea0f52d]"
+__git_sha__: Final[str] = "[c4955d3]"
 
 from . import client
 from . import constants
 from . import enums
 from . import errors
 from . import models
 from . import result
@@ -103,23 +103,24 @@
     "ComputedMetrics",
     "DeltaLeaderboardEntry",
     "DeltaService",
     "DeniedNameChangeReviewContext",
     "EfficiencyService",
     "Err",
     "Gains",
+    "Group",
     "GroupDetail",
     "GroupHiscoresActivityItem",
     "GroupHiscoresBossItem",
     "GroupHiscoresComputedMetricItem",
     "GroupHiscoresEntry",
     "GroupHiscoresSkillItem",
     "GroupMemberFragment",
+    "GroupMemberGains",
     "GroupMembership",
-    "Group",
     "GroupRole",
     "GroupService",
     "GroupStatistics",
     "HttpErrorResponse",
     "HttpService",
     "HttpSuccessResponse",
     "Membership",
@@ -154,12 +155,13 @@
     "Skill",
     "SkillGains",
     "SkillLeader",
     "Skills",
     "SkippedNameChangeReviewContext",
     "SnapshotData",
     "Snapshot",
+    "SnapshotTimelineEntry",
     "Team",
     "Top5ProgressResult",
     "UnwrapError",
     "WomError",
 )
```

### Comparing `wom_py-0.4.2/wom/__main__.py` & `wom_py-0.5.0/wom/__main__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/_cli.py` & `wom_py-0.5.0/wom/_cli.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/client.py` & `wom_py-0.5.0/wom/client.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/constants.py` & `wom_py-0.5.0/wom/constants.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/enums.py` & `wom_py-0.5.0/wom/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/errors.py` & `wom_py-0.5.0/wom/errors.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/models/__init__.py` & `wom_py-0.5.0/wom/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,22 +56,23 @@
     "ComputedGains",
     "ComputedMetric",
     "ComputedMetricLeader",
     "DeltaLeaderboardEntry",
     "DeniedNameChangeReviewContext",
     "Gains",
     "GroupDetail",
+    "Group",
     "GroupHiscoresActivityItem",
     "GroupHiscoresBossItem",
     "GroupHiscoresComputedMetricItem",
     "GroupHiscoresEntry",
     "GroupHiscoresSkillItem",
     "GroupMemberFragment",
+    "GroupMemberGains",
     "GroupMembership",
-    "Group",
     "GroupRole",
     "GroupStatistics",
     "HttpErrorResponse",
     "HttpSuccessResponse",
     "Membership",
     "MetricLeaders",
     "NameChange",
@@ -94,14 +95,15 @@
     "RecordLeaderboardEntry",
     "Skill",
     "SkillGains",
     "SkillLeader",
     "SkippedNameChangeReviewContext",
     "SnapshotData",
     "Snapshot",
+    "SnapshotTimelineEntry",
     "Team",
     "Top5ProgressResult",
 )
 
 from .base import *
 from .competitions import *
 from .deltas import *
```

### Comparing `wom_py-0.4.2/wom/models/base.py` & `wom_py-0.5.0/wom/models/base.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/models/competitions/__init__.py` & `wom_py-0.5.0/wom/models/competitions/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/models/competitions/enums.py` & `wom_py-0.5.0/wom/models/competitions/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/models/competitions/models.py` & `wom_py-0.5.0/wom/models/competitions/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/models/deltas/__init__.py` & `wom_py-0.5.0/wom/models/deltas/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/models/deltas/models.py` & `wom_py-0.5.0/wom/models/deltas/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/models/groups/__init__.py` & `wom_py-0.5.0/wom/models/groups/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,23 +23,24 @@
 
 from __future__ import annotations
 
 __all__ = (
     "ActivityLeader",
     "BossLeader",
     "ComputedMetricLeader",
+    "Group",
     "GroupDetail",
     "GroupHiscoresActivityItem",
     "GroupHiscoresBossItem",
     "GroupHiscoresComputedMetricItem",
     "GroupHiscoresEntry",
     "GroupHiscoresSkillItem",
     "GroupMemberFragment",
+    "GroupMemberGains",
     "GroupMembership",
-    "Group",
     "GroupRole",
     "GroupStatistics",
     "Membership",
     "MetricLeaders",
     "PlayerMembership",
     "SkillLeader",
 )
```

### Comparing `wom_py-0.4.2/wom/models/groups/enums.py` & `wom_py-0.5.0/wom/models/groups/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/models/groups/models.py` & `wom_py-0.5.0/wom/models/groups/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,31 +25,33 @@
 from datetime import datetime
 
 import attrs
 
 from wom import enums
 
 from ..base import BaseModel
+from ..players import Gains
 from ..players import Player
 from ..players import Snapshot
 from .enums import GroupRole
 
 __all__ = (
     "ActivityLeader",
     "BossLeader",
     "ComputedMetricLeader",
+    "Group",
     "GroupDetail",
     "GroupHiscoresActivityItem",
     "GroupHiscoresBossItem",
     "GroupHiscoresComputedMetricItem",
     "GroupHiscoresEntry",
     "GroupHiscoresSkillItem",
     "GroupMemberFragment",
+    "GroupMemberGains",
     "GroupMembership",
-    "Group",
     "GroupStatistics",
     "Membership",
     "MetricLeaders",
     "PlayerMembership",
     "SkillLeader",
 )
 
@@ -355,7 +357,24 @@
     average_stats: Snapshot
     """The average group statistics in a [`Snapshot`][wom.Snapshot]."""
 
     metric_leaders: MetricLeaders
     """The [`MetricLeaders`][wom.MetricLeaders] in this group for each
     metric.
     """
+
+
+@attrs.define(init=False)
+class GroupMemberGains(BaseModel):
+    """Represents a leaderboard entry over the given delta."""
+
+    start_date: datetime
+    """The start date of the gains."""
+
+    end_date: datetime
+    """The end date of the gains."""
+
+    player: Player
+    """The [`Player`][wom.Player] that attained these gains."""
+
+    data: Gains
+    """The [`Gains`][wom.Gains] for this group member."""
```

### Comparing `wom_py-0.4.2/wom/models/http.py` & `wom_py-0.5.0/wom/models/http.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/models/names/__init__.py` & `wom_py-0.5.0/wom/models/names/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/models/names/enums.py` & `wom_py-0.5.0/wom/models/names/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/models/names/models.py` & `wom_py-0.5.0/wom/models/names/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/models/players/__init__.py` & `wom_py-0.5.0/wom/models/players/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,11 +44,12 @@
     "PlayerDetail",
     "PlayerStatus",
     "PlayerType",
     "SkillGains",
     "Skill",
     "SnapshotData",
     "Snapshot",
+    "SnapshotTimelineEntry",
 )
 
 from .enums import *
 from .models import *
```

### Comparing `wom_py-0.4.2/wom/models/players/enums.py` & `wom_py-0.5.0/wom/models/players/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/models/players/models.py` & `wom_py-0.5.0/wom/models/players/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     "PlayerGains",
     "Player",
     "PlayerDetail",
     "SkillGains",
     "Skill",
     "SnapshotData",
     "Snapshot",
+    "SnapshotTimelineEntry",
 )
 
 
 @attrs.define(init=False)
 class Skill(BaseModel):
     """Details regarding a particular skill."""
 
@@ -458,7 +459,18 @@
     """The date the gains started at."""
 
     ends_at: datetime
     """The date the gains ended at."""
 
     data: PlayerGainsData
     """The [`PlayerGainsData`][wom.PlayerGainsData] for the player."""
+
+
+@attrs.define(init=False)
+class SnapshotTimelineEntry(BaseModel):
+    """An entry representing a point in time of a players gains."""
+
+    value: int
+    """The total xp gained since the last timeline entry."""
+
+    date: datetime
+    """The date this timeline entry was recorded."""
```

### Comparing `wom_py-0.4.2/wom/models/records/__init__.py` & `wom_py-0.5.0/wom/models/records/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/models/records/models.py` & `wom_py-0.5.0/wom/models/records/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/result.py` & `wom_py-0.5.0/wom/result.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/routes.py` & `wom_py-0.5.0/wom/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,15 @@
 PLAYER_ACHIEVEMENT_PROGRESS: t.Final[Route] = Route("GET", "/players/{}/achievements/progress")
 PLAYER_COMPETITION_PARTICIPATION: t.Final[Route] = Route("GET", "/players/{}/competitions")
 PLAYER_COMPETITION_STANDINGS: t.Final[Route] = Route("GET", "/players/{}/competitions/standings")
 PLAYER_GROUP_MEMBERSHIPS: t.Final[Route] = Route("GET", "/players/{}/groups")
 PLAYER_GAINS: t.Final[Route] = Route("GET", "/players/{}/gained")
 PLAYER_RECORDS: t.Final[Route] = Route("GET", "/players/{}/records")
 PLAYER_SNAPSHOTS: t.Final[Route] = Route("GET", "/players/{}/snapshots")
+PLAYER_SNAPSHOTS_TIMELINE: t.Final[Route] = Route("GET", "/players/{}/snapshots/timeline")
 SEARCH_NAME_CHANGES: t.Final[Route] = Route("GET", "/names")
 SUBMIT_NAME_CHANGE: t.Final[Route] = Route("POST", "/names")
 PLAYER_NAME_CHANGES: t.Final[Route] = Route("GET", "/players/{}/names")
 GLOBAL_RECORD_LEADERS: t.Final[Route] = Route("GET", "/records/leaderboard")
 GLOBAL_EFFICIENCY_LEADERS: t.Final[Route] = Route("GET", "/efficiency/leaderboard")
 GLOBAL_DELTA_LEADERS: t.Final[Route] = Route("GET", "/deltas/leaderboard")
 SEARCH_GROUPS: t.Final[Route] = Route("GET", "/groups")
```

### Comparing `wom_py-0.4.2/wom/serializer.py` & `wom_py-0.5.0/wom/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -559,14 +559,30 @@
         delta.gained = data["gained"]
         delta.player_id = data["playerId"]
         delta.end_date = self._dt_from_iso(data["endDate"])
         delta.start_date = self._dt_from_iso(data["startDate"])
         delta.player = self.deserialize_player(data["player"])
         return delta
 
+    def deserialize_group_member_gains(self, data: DictT) -> models.GroupMemberGains:
+        """Deserializes the data into a group member gains model.
+
+        Args:
+            data: The JSON payload.
+
+        Returns:
+            The requested model.
+        """
+        gains = models.GroupMemberGains()
+        gains.end_date = self._dt_from_iso(data["endDate"])
+        gains.start_date = self._dt_from_iso(data["startDate"])
+        gains.player = self.deserialize_player(data["player"])
+        gains.data = self.deserialize_gains(data["data"])
+        return gains
+
     def deserialize_group(self, data: DictT) -> models.Group:
         """Deserializes the data into a group model.
 
         Args:
             data: The JSON payload.
 
         Returns:
@@ -1026,7 +1042,21 @@
         leaders.bosses = self.__map(self.deserialize_boss_leader, data["bosses"].values())
         leaders.computed = self.__map(self.deserialize_computed_leader, data["computed"].values())
         leaders.activities = self.__map(
             self.deserialize_activity_leader, data["activities"].values()
         )
 
         return leaders
+
+    def deserialize_snapshot_timeline_entry(self, data: DictT) -> models.SnapshotTimelineEntry:
+        """Deserializes the data into a snapshot timeline entry model.
+
+        Args:
+            data: The JSON payload.
+
+        Returns:
+            The requested model.
+        """
+        entry = models.SnapshotTimelineEntry()
+        entry.date = self._dt_from_iso(data["date"])
+        entry.value = data["value"]
+        return entry
```

### Comparing `wom_py-0.4.2/wom/services/__init__.py` & `wom_py-0.5.0/wom/services/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/services/base.py` & `wom_py-0.5.0/wom/services/base.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/services/competitions.py` & `wom_py-0.5.0/wom/services/competitions.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/services/deltas.py` & `wom_py-0.5.0/wom/services/deltas.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/services/efficiency.py` & `wom_py-0.5.0/wom/services/efficiency.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/services/groups.py` & `wom_py-0.5.0/wom/services/groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -535,15 +535,15 @@
         metric: enums.Metric,
         *,
         period: t.Optional[enums.Period] = None,
         start_date: t.Optional[datetime] = None,
         end_date: t.Optional[datetime] = None,
         limit: t.Optional[int] = None,
         offset: t.Optional[int] = None,
-    ) -> ResultT[t.List[models.DeltaLeaderboardEntry]]:
+    ) -> ResultT[t.List[models.GroupMemberGains]]:
         """Gets the gains for a group over a particular time frame.
 
         Args:
             id: The ID of the group.
 
             metric: The metric to filter on.
 
@@ -595,15 +595,15 @@
 
         route = routes.GROUP_GAINS.compile(id).with_params(params)
         data = await self._http.fetch(route, self._list)
 
         if isinstance(data, models.HttpErrorResponse):
             return result.Err(data)
 
-        return result.Ok([self._serializer.deserialize_delta_leaderboard_entry(d) for d in data])
+        return result.Ok([self._serializer.deserialize_group_member_gains(d) for d in data])
 
     async def get_achievements(
         self,
         id: int,
         *,
         limit: t.Optional[int] = None,
         offset: t.Optional[int] = None,
```

### Comparing `wom_py-0.4.2/wom/services/http.py` & `wom_py-0.5.0/wom/services/http.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/services/names.py` & `wom_py-0.5.0/wom/services/names.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/wom/services/players.py` & `wom_py-0.5.0/wom/services/players.py`

 * *Files 7% similar despite different names*

```diff
@@ -590,7 +590,71 @@
         route = routes.PLAYER_NAME_CHANGES.compile(username)
         data = await self._http.fetch(route, self._list)
 
         if isinstance(data, models.HttpErrorResponse):
             return result.Err(data)
 
         return result.Ok([self._serializer.deserialize_name_change(c) for c in data])
+
+    async def get_snapshots_timeline(
+        self,
+        username: str,
+        metric: enums.Metric,
+        *,
+        period: t.Optional[enums.Period] = None,
+        start_date: t.Optional[datetime] = None,
+        end_date: t.Optional[datetime] = None,
+    ) -> ResultT[t.List[models.SnapshotTimelineEntry]]:
+        """Gets the snapshots timeline for the given player and metric.
+
+        Args:
+            username: The username to get the timeline for.
+
+            metric: The metric to get the timeline for.
+
+        Keyword Args:
+            period: The optional period of time to get snapshots for.
+                Defaults to `None`.
+
+            start_date: The minimum date to get the snapshots from.
+                Defaults to `None`.
+
+            end_date: The maximum date to get the snapshots from.
+                Defaults to `None`.
+
+        Returns:
+            A [`Result`][wom.Result] containing the list of snapshots timeline
+                entries.
+
+        !!! info
+
+            You can pass either (`period`) or (`start_date` +
+            `end_date`), but not both.
+
+        ??? example
+
+            ```py
+            import wom
+
+            client = wom.Client(...)
+
+            await client.start()
+
+            result = await client.players.get_snapshots_timeline(
+                "Jonxslays", wom.Skills.Attack, period=wom.Period.Week
+            )
+            ```
+        """
+        params = self._generate_map(
+            period=period.value if period else None,
+            startDate=start_date.isoformat() if start_date else None,
+            endDate=end_date.isoformat() if end_date else None,
+            metric=metric.value,
+        )
+
+        route = routes.PLAYER_SNAPSHOTS_TIMELINE.compile(username).with_params(params)
+        data = await self._http.fetch(route, self._list)
+
+        if isinstance(data, models.HttpErrorResponse):
+            return result.Err(data)
+
+        return result.Ok([self._serializer.deserialize_snapshot_timeline_entry(e) for e in data])
```

### Comparing `wom_py-0.4.2/wom/services/records.py` & `wom_py-0.5.0/wom/services/records.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.2/PKG-INFO` & `wom_py-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wom-py
-Version: 0.4.2
+Version: 0.5.0
 Summary: An asynchronous wrapper for the Wise Old Man API.
 Home-page: https://github.com/Jonxslays/wom.py
 License: MIT
 Author: Jonxslays
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wom-py Version: 0.4.2 Summary: An asynchronous
+Metadata-Version: 2.1 Name: wom-py Version: 0.5.0 Summary: An asynchronous
 wrapper for the Wise Old Man API. Home-page: https://github.com/Jonxslays/
 wom.py License: MIT Author: Jonxslays Requires-Python: >=3.8 Classifier:
 Development Status :: 4 - Beta Classifier: Framework :: AsyncIO Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

