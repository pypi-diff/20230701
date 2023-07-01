# Comparing `tmp/TrimMCStruct-0.0.5.8.tar.gz` & `tmp/TrimMCStruct-0.0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrimMCStruct-0.0.5.8.tar", last modified: Sat Apr 29 14:12:16 2023, max compression
+gzip compressed data, was "TrimMCStruct-0.0.5.9.tar", last modified: Sat Jul  1 14:07:45 2023, max compression
```

## Comparing `TrimMCStruct-0.0.5.8.tar` & `TrimMCStruct-0.0.5.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 14:12:16.556613 TrimMCStruct-0.0.5.8/
--rw-rw-rw-   0        0        0     1277 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.8/LICENSE(origin).md
--rw-rw-rw-   0        0        0    13331 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.8/LICENSE.md
--rw-rw-rw-   0        0        0     5030 2023-04-29 14:12:16.555616 TrimMCStruct-0.0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     4022 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 14:12:16.544682 TrimMCStruct-0.0.5.8/TrimMCStruct/
--rw-rw-rw-   0        0        0      398 2023-04-29 14:06:24.000000 TrimMCStruct-0.0.5.8/TrimMCStruct/__init__.py
--rw-rw-rw-   0        0        0    21789 2023-04-29 13:57:10.000000 TrimMCStruct-0.0.5.8/TrimMCStruct/main.py
-drwxrwxrwx   0        0        0        0 2023-04-29 14:12:16.554619 TrimMCStruct-0.0.5.8/TrimMCStruct.egg-info/
--rw-rw-rw-   0        0        0     5030 2023-04-29 14:12:16.000000 TrimMCStruct-0.0.5.8/TrimMCStruct.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-04-29 14:12:16.000000 TrimMCStruct-0.0.5.8/TrimMCStruct.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 14:12:16.000000 TrimMCStruct-0.0.5.8/TrimMCStruct.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-29 14:12:16.000000 TrimMCStruct-0.0.5.8/TrimMCStruct.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-29 14:12:16.000000 TrimMCStruct-0.0.5.8/TrimMCStruct.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 14:12:16.556613 TrimMCStruct-0.0.5.8/setup.cfg
--rw-rw-rw-   0        0        0     1495 2023-04-29 14:09:51.000000 TrimMCStruct-0.0.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 14:07:45.944290 TrimMCStruct-0.0.5.9/
+-rw-rw-rw-   0        0        0     1277 2023-03-26 11:30:36.000000 TrimMCStruct-0.0.5.9/LICENSE(origin).md
+-rw-rw-rw-   0        0        0    13331 2023-07-01 14:07:00.000000 TrimMCStruct-0.0.5.9/LICENSE.md
+-rw-rw-rw-   0        0        0     5030 2023-07-01 14:07:45.943586 TrimMCStruct-0.0.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4022 2023-03-26 11:32:56.000000 TrimMCStruct-0.0.5.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 14:07:45.915637 TrimMCStruct-0.0.5.9/TrimMCStruct/
+-rw-rw-rw-   0        0        0      507 2023-07-01 14:07:00.000000 TrimMCStruct-0.0.5.9/TrimMCStruct/__init__.py
+-rw-rw-rw-   0        0        0    21880 2023-07-01 14:07:00.000000 TrimMCStruct-0.0.5.9/TrimMCStruct/main.py
+drwxrwxrwx   0        0        0        0 2023-07-01 14:07:45.941045 TrimMCStruct-0.0.5.9/TrimMCStruct.egg-info/
+-rw-rw-rw-   0        0        0     5030 2023-07-01 14:07:45.000000 TrimMCStruct-0.0.5.9/TrimMCStruct.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-01 14:07:45.000000 TrimMCStruct-0.0.5.9/TrimMCStruct.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 14:07:45.000000 TrimMCStruct-0.0.5.9/TrimMCStruct.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-01 14:07:45.000000 TrimMCStruct-0.0.5.9/TrimMCStruct.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-01 14:07:45.000000 TrimMCStruct-0.0.5.9/TrimMCStruct.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 14:07:45.945291 TrimMCStruct-0.0.5.9/setup.cfg
+-rw-rw-rw-   0        0        0     1495 2023-07-01 14:07:00.000000 TrimMCStruct-0.0.5.9/setup.py
```

### Comparing `TrimMCStruct-0.0.5.8/LICENSE(origin).md` & `TrimMCStruct-0.0.5.9/LICENSE(origin).md`

 * *Files identical despite different names*

### Comparing `TrimMCStruct-0.0.5.8/LICENSE.md` & `TrimMCStruct-0.0.5.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TrimMCStruct-0.0.5.8/PKG-INFO` & `TrimMCStruct-0.0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrimMCStruct
-Version: 0.0.5.8
+Version: 0.0.5.9
 Summary: 读写操作《我的世界》.MCSTRUCTURE文件
 Home-page: https://github.com/TriM-Organization/TrimMCStruct
 Author: Eilles Wan, bgArray, phoenixr-codes(original author) 
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `TrimMCStruct-0.0.5.8/README.md` & `TrimMCStruct-0.0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `TrimMCStruct-0.0.5.8/TrimMCStruct/main.py` & `TrimMCStruct-0.0.5.9/TrimMCStruct/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,16 +125,16 @@
     .. code-block::
 
         Block("minecraft:wool", color = "red")
     """
 
     namespace: str
     base_name: str
-    states: dict[str, Union[int, str, bool]]
-    extra_data: dict[str, Union[int, str, bool]]
+    states: dict[str, Any]
+    extra_data: dict[str, Any]
 
     def __init__(
         self,
         namespace: str,
         base_name: str,
         states: dict[str, Union[int, str, bool]] = {},
         extra_data: dict[str, Union[int, str, bool]] = {},
@@ -305,15 +305,15 @@
 class Structure:
     """
     Class representing a Minecraft structure that
     consists of blocks and entities.
 
     Attributes
     ----------
-    _size
+    size
         The size of the structure.
     """
 
     structure_indecis: NDArray[np.intc]
 
     def __init__(
         self,
@@ -460,15 +460,15 @@
         Serialize the structure as a ``mcstructure``.
 
         Parameters
         ----------
         file
             File object to write to.
         """
-        nbt = NBTFile(
+        NBTFile(
             value=dict(
                 format_version=TAG_Int(1),
                 size=TAG_List(TAG_Int, map(TAG_Int, self._size)),
                 structure=TAG_Compound(
                     dict(
                         block_indices=TAG_List(
                             TAG_List,
@@ -533,16 +533,15 @@
                             )
                         ),
                     )
                 ),
                 structure_world_origin=TAG_List(TAG_Int, [0, 0, 0]),
             ),
             little_endian=True,
-        )
-        nbt.save(file, little_endian=True)
+        ).save(file, little_endian=True)
 
     def mirror(self, axis: str) -> Structure:
         """
         Flips the structure.
 
         Parameters
         ----------
@@ -638,25 +637,26 @@
             "Structure Void" blocks will be used.
         """
         x, y, z = coordinate
 
         ident = self._add_block_to_palette(block)
 
         self.structure_indecis[x, y, z] = ident
-        if block.extra_data:
-            self._special_blocks[
-                x * self.size[2] * self.size[1] + y * self.size[2] + z
-            ] = block.extra_data
+        if block:
+            if block.extra_data:
+                self._special_blocks[
+                    x * self.size[2] * self.size[1] + y * self.size[2] + z
+                ] = block.extra_data
         return self
 
     def fill_blocks(
         self,
         from_coordinate: Coordinate,
         to_coordinate: Coordinate,
-        block: Block,
+        block: Optional[Block],
     ) -> Structure:
         """
         Puts multiple blocks into the structure.
 
         Notes
         -----
         Both start and end points are filled.
@@ -686,29 +686,30 @@
                     for j in range(abs(fy - ty) + 1)
                 ]
                 for i in range(abs(fx - tx) + 1)
             ],
             dtype=np.intc,
         ).reshape([abs(i) + 1 for i in (fx - tx, fy - ty, fz - tz)])
 
-        if block.extra_data:
-            self._special_blocks.update(
-                dict(
-                    zip(
-                        [
-                            (x * self.size[2] * self.size[1] + y * self.size[2] + z)
-                            for x in range(fx, tx)
-                            for y in range(fy, ty)
-                            for z in range(fz, tz)
-                        ],
-                        [
-                            block.extra_data
-                            for i in range(
-                                abs((fz - tz) + 1)
-                                * (abs(fy - ty) + 1)
-                                * (abs(fx - tx) + 1)
-                            )
-                        ],
+        if block:
+            if block.extra_data:
+                self._special_blocks.update(
+                    dict(
+                        zip(
+                            [
+                                (x * self.size[2] * self.size[1] + y * self.size[2] + z)
+                                for x in range(fx, tx)
+                                for y in range(fy, ty)
+                                for z in range(fz, tz)
+                            ],
+                            [
+                                block.extra_data
+                                for i in range(
+                                    abs((fz - tz) + 1)
+                                    * (abs(fy - ty) + 1)
+                                    * (abs(fx - tx) + 1)
+                                )
+                            ],
+                        )
                     )
                 )
-            )
         return self
```

### Comparing `TrimMCStruct-0.0.5.8/TrimMCStruct.egg-info/PKG-INFO` & `TrimMCStruct-0.0.5.9/TrimMCStruct.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrimMCStruct
-Version: 0.0.5.8
+Version: 0.0.5.9
 Summary: 读写操作《我的世界》.MCSTRUCTURE文件
 Home-page: https://github.com/TriM-Organization/TrimMCStruct
 Author: Eilles Wan, bgArray, phoenixr-codes(original author) 
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `TrimMCStruct-0.0.5.8/setup.py` & `TrimMCStruct-0.0.5.9/setup.py`

 * *Files identical despite different names*

