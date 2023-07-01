# Comparing `tmp/xia_agent-0.1.5-cp39-none-win_amd64.whl.zip` & `tmp/xia_agent-0.1.6-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3608 bytes, number of entries: 7
--rw-r--r--  2.0 unx      145 b- defN 23-Jun-30 11:16 xia_agent/__init__.py
+Zip file size: 3604 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      145 b- defN 23-Jul-01 17:46 xia_agent/__init__.py
 -rw-r--r--  2.0 unx     7183 b- defN 23-Jun-29 20:32 xia_agent/agent.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:17 xia_agent-0.1.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      462 b- defN 23-Jun-30 11:17 xia_agent-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:17 xia_agent-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-30 11:17 xia_agent-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      550 b- defN 23-Jun-30 11:17 xia_agent-0.1.5.dist-info/RECORD
-7 files, 8600 bytes uncompressed, 2630 bytes compressed:  69.4%
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 17:46 xia_agent-0.1.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      462 b- defN 23-Jul-01 17:46 xia_agent-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 17:46 xia_agent-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-01 17:46 xia_agent-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      550 b- defN 23-Jul-01 17:46 xia_agent-0.1.6.dist-info/RECORD
+7 files, 8600 bytes uncompressed, 2626 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_agent/__init__.py
 Comment: 
 
 Filename: xia_agent/agent.py
 Comment: 
 
-Filename: xia_agent-0.1.5.dist-info/LICENSE.txt
+Filename: xia_agent-0.1.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_agent-0.1.5.dist-info/METADATA
+Filename: xia_agent-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: xia_agent-0.1.5.dist-info/WHEEL
+Filename: xia_agent-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: xia_agent-0.1.5.dist-info/top_level.txt
+Filename: xia_agent-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_agent-0.1.5.dist-info/RECORD
+Filename: xia_agent-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_agent/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_agent.agent import Agent, AgentFunction, MetaFunction
 
 __all__ = [
     "Agent", "AgentFunction", "MetaFunction"
 ]
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
```

## Comparing `xia_agent-0.1.5.dist-info/RECORD` & `xia_agent-0.1.6.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_agent/__init__.py,sha256=gpDkoaiLFGdLEb0df4BaIzCCAZDRt68ubTIH_leM6Ls,145
+xia_agent/__init__.py,sha256=ur1Xd8wATFWxrhlnW9iz9KjxqVxHLxHqZYmBsS5kjZ4,145
 xia_agent/agent.py,sha256=qmWuNrR05n-7BkqOkcZsRXV0L_-Qwel3jNNkd3hN_EU,7183
-xia_agent-0.1.5.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
-xia_agent-0.1.5.dist-info/METADATA,sha256=wtoftBtOAVCC4hJL1NTXVNvVDbb5n2wVXnofPJ_GlOs,462
-xia_agent-0.1.5.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_agent-0.1.5.dist-info/top_level.txt,sha256=uiK8HE2yj2wekdrxVgGRL0zCqajqbV6xrgTp7HlCXYU,10
-xia_agent-0.1.5.dist-info/RECORD,,
+xia_agent-0.1.6.dist-info/LICENSE.txt,sha256=VI2DRhUdOX7ADnFkyNfO3YiExtoLHTFKKd8XFlFAbWw,151
+xia_agent-0.1.6.dist-info/METADATA,sha256=O9LbmPcSjWRvjFwW5i1RH0p-lKIDfqek8B3gXswLEKo,462
+xia_agent-0.1.6.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_agent-0.1.6.dist-info/top_level.txt,sha256=uiK8HE2yj2wekdrxVgGRL0zCqajqbV6xrgTp7HlCXYU,10
+xia_agent-0.1.6.dist-info/RECORD,,
```

