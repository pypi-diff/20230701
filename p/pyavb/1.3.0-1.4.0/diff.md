# Comparing `tmp/pyavb-1.3.0.tar.gz` & `tmp/pyavb-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyavb-1.3.0.tar", last modified: Sat Jul  9 00:42:41 2022, max compression
+gzip compressed data, was "pyavb-1.4.0.tar", last modified: Sat Jul  1 21:43:57 2023, max compression
```

## Comparing `pyavb-1.3.0.tar` & `pyavb-1.4.0.tar`

### file list

```diff
@@ -1,33 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 00:42:41.508107 pyavb-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-07-09 00:42:30.000000 pyavb-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-07-09 00:42:30.000000 pyavb-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2595 2022-07-09 00:42:41.508107 pyavb-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-07-09 00:42:30.000000 pyavb-1.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-07-09 00:42:30.000000 pyavb-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-07-09 00:42:41.508107 pyavb-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4112 2022-07-09 00:42:30.000000 pyavb-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 00:42:41.504107 pyavb-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 00:42:41.504107 pyavb-1.3.0/src/avb/
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-07-09 00:42:30.000000 pyavb-1.3.0/src/avb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)  1232099 2022-07-09 00:42:41.000000 pyavb-1.3.0/src/avb/_ext.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    20699 2022-07-09 00:42:30.000000 pyavb-1.3.0/src/avb/_ext.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    34917 2022-07-09 00:42:30.000000 pyavb-1.3.0/src/avb/_ext_core.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4676 2022-07-09 00:42:30.000000 pyavb-1.3.0/src/avb/attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)    14760 2022-07-09 00:42:30.000000 pyavb-1.3.0/src/avb/bin.py
--rw-r--r--   0 runner    (1001) docker     (121)    29307 2022-07-09 00:42:30.000000 pyavb-1.3.0/src/avb/components.py
--rw-r--r--   0 runner    (1001) docker     (121)     6942 2022-07-09 00:42:30.000000 pyavb-1.3.0/src/avb/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    49971 2022-07-09 00:42:30.000000 pyavb-1.3.0/src/avb/essence.py
--rw-r--r--   0 runner    (1001) docker     (121)    10514 2022-07-09 00:42:30.000000 pyavb-1.3.0/src/avb/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     7253 2022-07-09 00:42:30.000000 pyavb-1.3.0/src/avb/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (121)    11850 2022-07-09 00:42:30.000000 pyavb-1.3.0/src/avb/ioctx.py
--rw-r--r--   0 runner    (1001) docker     (121)    39218 2022-07-09 00:42:30.000000 pyavb-1.3.0/src/avb/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)    19957 2022-07-09 00:42:30.000000 pyavb-1.3.0/src/avb/mobid.py
--rw-r--r--   0 runner    (1001) docker     (121)    47448 2022-07-09 00:42:30.000000 pyavb-1.3.0/src/avb/parameter_uuids.py
--rw-r--r--   0 runner    (1001) docker     (121)    39726 2022-07-09 00:42:30.000000 pyavb-1.3.0/src/avb/trackgroups.py
--rw-r--r--   0 runner    (1001) docker     (121)     3125 2022-07-09 00:42:30.000000 pyavb-1.3.0/src/avb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 00:42:41.508107 pyavb-1.3.0/src/pyavb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2595 2022-07-09 00:42:41.000000 pyavb-1.3.0/src/pyavb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-07-09 00:42:41.000000 pyavb-1.3.0/src/pyavb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-09 00:42:41.000000 pyavb-1.3.0/src/pyavb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-07-09 00:42:41.000000 pyavb-1.3.0/src/pyavb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-07-09 00:42:41.000000 pyavb-1.3.0/src/pyavb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:43:57.312265 pyavb-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-01 21:43:46.000000 pyavb-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-01 21:43:46.000000 pyavb-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-01 21:43:57.312265 pyavb-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-01 21:43:46.000000 pyavb-1.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-01 21:43:46.000000 pyavb-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-01 21:43:57.312265 pyavb-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-01 21:43:46.000000 pyavb-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:43:57.308265 pyavb-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:43:57.312265 pyavb-1.4.0/src/avb/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-01 21:43:46.000000 pyavb-1.4.0/src/avb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1232099 2023-07-01 21:43:56.000000 pyavb-1.4.0/src/avb/_ext.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20699 2023-07-01 21:43:46.000000 pyavb-1.4.0/src/avb/_ext.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    34917 2023-07-01 21:43:46.000000 pyavb-1.4.0/src/avb/_ext_core.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-07-01 21:43:46.000000 pyavb-1.4.0/src/avb/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15018 2023-07-01 21:43:46.000000 pyavb-1.4.0/src/avb/bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29471 2023-07-01 21:43:46.000000 pyavb-1.4.0/src/avb/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-07-01 21:43:46.000000 pyavb-1.4.0/src/avb/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52335 2023-07-01 21:43:46.000000 pyavb-1.4.0/src/avb/essence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10897 2023-07-01 21:43:46.000000 pyavb-1.4.0/src/avb/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-07-01 21:43:46.000000 pyavb-1.4.0/src/avb/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-01 21:43:46.000000 pyavb-1.4.0/src/avb/ioctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39257 2023-07-01 21:43:46.000000 pyavb-1.4.0/src/avb/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19957 2023-07-01 21:43:46.000000 pyavb-1.4.0/src/avb/mobid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47448 2023-07-01 21:43:46.000000 pyavb-1.4.0/src/avb/parameter_uuids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40596 2023-07-01 21:43:46.000000 pyavb-1.4.0/src/avb/trackgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-01 21:43:46.000000 pyavb-1.4.0/src/avb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:43:57.312265 pyavb-1.4.0/src/pyavb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-01 21:43:57.000000 pyavb-1.4.0/src/pyavb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-01 21:43:57.000000 pyavb-1.4.0/src/pyavb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 21:43:57.000000 pyavb-1.4.0/src/pyavb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-01 21:43:57.000000 pyavb-1.4.0/src/pyavb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-01 21:43:57.000000 pyavb-1.4.0/src/pyavb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:43:57.312265 pyavb-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-07-01 21:43:46.000000 pyavb-1.4.0/tests/test_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-01 21:43:46.000000 pyavb-1.4.0/tests/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-01 21:43:46.000000 pyavb-1.4.0/tests/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-01 21:43:46.000000 pyavb-1.4.0/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-01 21:43:46.000000 pyavb-1.4.0/tests/test_retime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-01 21:43:46.000000 pyavb-1.4.0/tests/test_write.py
```

### Comparing `pyavb-1.3.0/LICENSE` & `pyavb-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyavb-1.3.0/PKG-INFO` & `pyavb-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyavb
-Version: 1.3.0
+Version: 1.4.0
 Summary: A python module for the reading and writing Avid Bin Files files.
 Home-page: https://github.com/markreidvfx/pyavb
 Author: Mark Reid
 Author-email: mindmark@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/markreidvfx/pyavb
 Project-URL: Documentation, http://pyavb.readthedocs.io
```

### Comparing `pyavb-1.3.0/README.rst` & `pyavb-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyavb-1.3.0/setup.py` & `pyavb-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup, find_packages
 import setuptools.command.build_py
 import setuptools.command.build_ext
 from distutils.extension import Extension
 
 PROJECT_METADATA = {
-    "version": "1.3.0",
+    "version": "1.4.0",
     "author": 'Mark Reid',
     "author_email": 'mindmark@gmail.com',
     "license": 'MIT',
 }
 
 METADATA_TEMPLATE = """
 __version__ = "{version}"
```

### Comparing `pyavb-1.3.0/src/avb/_ext.cpp` & `pyavb-1.4.0/src/avb/_ext.cpp`

 * *Files identical despite different names*

### Comparing `pyavb-1.3.0/src/avb/_ext.pyx` & `pyavb-1.4.0/src/avb/_ext.pyx`

 * *Files identical despite different names*

### Comparing `pyavb-1.3.0/src/avb/_ext_core.cpp` & `pyavb-1.4.0/src/avb/_ext_core.cpp`

 * *Files identical despite different names*

### Comparing `pyavb-1.3.0/src/avb/attributes.py` & `pyavb-1.4.0/src/avb/attributes.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,14 +46,29 @@
         self.mark_modified()
 
     def pop(self, *args, **kwargs):
         result = super(Attributes, self).pop(*args, **kwargs)
         self.mark_modified()
         return result
 
+    def copy(self, root):
+        obj = root.create.from_name(self.__class__.__name__)
+        for key, value in self.items():
+            if isinstance(value, int):
+                obj[key] = value
+            elif isinstance(value, unicode):
+                obj[key] = value
+            elif isinstance(value, bytearray):
+                obj[key] = value[:]
+            elif isinstance(value, bytes):
+                raise ValueError("%s: bytes value type too ambiguous, use bytearray or unicode str" % key)
+            else:
+                obj[key] = value.copy(root)
+        return obj
+
     def read(self, f):
         ctx = self.root.ictx
         ctx.read_assert_tag(f, 0x02)
         ctx.read_assert_tag(f, 0x01)
 
         count = ctx.read_u32(f)
 
@@ -113,15 +128,15 @@
                 f.write(value)
 
         ctx.write_u8(f, 0x03)
 
 @utils.register_class
 class ParameterList(AVBRefList):
     class_id = b'PRLS'
-    __slots__ = ()
+    __slots__ = ('instance_id',)
     def read(self, f):
         ctx = self.root.ictx
         ctx.read_assert_tag(f, 0x02)
         ctx.read_assert_tag(f, 0x01)
 
         count = ctx.read_s32(f)
         for i in range(count):
@@ -140,15 +155,15 @@
             ctx.write_object_ref(self.root, f, obj)
 
         ctx.write_u8(f, 0x03)
 
 @utils.register_class
 class TimeCrumbList(AVBRefList):
     class_id = b'TMCS'
-    __slots__ = ()
+    __slots__ = ('instance_id',)
 
     def read(self, f):
         ctx = self.root.ictx
         ctx.read_assert_tag(f, 0x02)
         ctx.read_assert_tag(f, 0x01)
 
         count = ctx.read_s16(f)
```

### Comparing `pyavb-1.3.0/src/avb/bin.py` & `pyavb-1.4.0/src/avb/bin.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,15 +212,15 @@
         AVBPropertyDef('home_rect',        'HomeRect',       'rect',       [0, 0 , 300, 600]),
         AVBPropertyDef('background_color', 'BackColor',      'color', [45568, 45568, 45568]),
         AVBPropertyDef('forground_color',  'ForeColor',      'color',    [3328, 3328, 3328]),
         AVBPropertyDef('ql_image_scale',   'QLImageScale',   'int16',         6),
         AVBPropertyDef('attributes',       'BinAttr',        'reference'),
         AVBPropertyDef('was_iconic',       'WasIconic',      'bool',      False),
     ]
-    __slots__ = ('mob_dict')
+    __slots__ = ('_mob_dict')
 
     def __init__(self):
         super(Bin, self).__init__(self)
 
         self.view_setting = self.root.create.BinViewSetting()
         self.uid = utils.generate_uid()
         self.items = []
@@ -228,14 +228,15 @@
 
         self.sifted_settings= []
         for i in range(6):
             s = self.root.create.SiftItem()
             self.sifted_settings.append(s)
 
         self.attributes = self.root.create.Attributes()
+        self._mob_dict ={}
 
     def read(self, f):
         super(Bin, self).read(f)
         ctx = self.root.ictx
         ctx.read_assert_tag(f, 0x02)
 
         version = ctx.read_u8(f)
@@ -251,14 +252,15 @@
         if version == 0x0e:
             object_count = ctx.read_u16(f)
         else:
             #large bin size > max u16
             object_count = ctx.read_u32(f)
 
         self.items = []
+        self._mob_dict ={}
 
         for i in range(object_count):
             bin_obj = BinItem.__new__(BinItem, root=self.root)
             bin_obj.mob = ctx.read_object_ref(self.root, f)
             bin_obj.x = ctx.read_s16(f)
             bin_obj.y = ctx.read_s16(f)
             bin_obj.keyframe = ctx.read_s32(f)
@@ -363,24 +365,33 @@
         ctx.write_s16(f, self.ql_image_scale)
         ctx.write_object_ref(self.root, f, self.attributes)
         ctx.write_bool(f, self.was_iconic)
 
         if self.class_id[:] == b'ABIN':
             ctx.write_u8(f, 0x03)
 
-    def build_mob_dict(self):
-        self.mob_dict = {}
-        for mob in self.mobs:
-            self.mob_dict[mob.mob_id] = mob
+    def find_by_mob_id(self, mob_id):
+
+        # build mob_id dictionary
+        if not self._mob_dict:
+            for mob in self.mobs:
+                self._mob_dict[mob.mob_id] = mob
+
+        return self._mob_dict.get(mob_id, None)
 
     def add_mob(self, mob):
         bin_item = self.root.create.BinItem()
         bin_item.mob = mob
         self.items.append(bin_item)
 
+        if self._mob_dict:
+            self._mob_dict[mob.mob_id] = mob
+
+        return bin_item
+
     @property
     def mobs(self):
         for item in self.items:
             yield item.mob
 
     def toplevel(self):
         for mob in self.mobs:
```

### Comparing `pyavb-1.3.0/src/avb/components.py` & `pyavb-1.4.0/src/avb/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,16 @@
             return "edgecode"
         elif self.media_kind_id == 5:
             return "attribute"
         elif self.media_kind_id == 6:
             return 'effectdata'
         elif self.media_kind_id == 7:
             return 'DescriptiveMetadata'
+        elif self.media_kind_id == 16:
+            return "DataEssenceTrack"
         else:
             return "unknown%d" % self.media_kind_id
 
     @media_kind.setter
     def media_kind(self, value):
         if value == None:
             self.media_kind_id = 0
@@ -127,14 +129,16 @@
             self.media_kind_id = 4
         elif value == "attribute":
             self.media_kind_id = 5
         elif value == 'effectdata':
             self.media_kind_id = 6
         elif value == 'DescriptiveMetadata':
             self.media_kind_id = 7
+        elif value == 'DataEssenceTrack':
+            self.media_kind_id = 16
         else:
             raise ValueError('unknown media kind: %s' % str(value))
 
 @utils.register_class
 class Sequence(Component):
     class_id = b"SEQU"
     propertydefs_dict = {}
@@ -150,15 +154,15 @@
     def read(self, f):
         super(Sequence, self).read(f)
         ctx = self.root.ictx
         ctx.read_assert_tag(f, 0x02)
         ctx.read_assert_tag(f, 0x03)
 
         count = ctx.read_u32(f)
-        self.components = AVBRefList.__new__(AVBRefList, root=self.root)
+        self.components = AVBRefList.__new__(AVBRefList, root=self.root, parent=self)
         for i in range(count):
             ref = ctx.read_object_ref(self.root, f)
             # print ref
             self.components.append(ref)
 
         ctx.read_assert_tag(f, 0x03)
 
@@ -308,15 +312,15 @@
         ctx.write_u8(f, 0x03)
 
     @property
     def mob(self):
         if hasattr(self, 'mob_id'):
             mob_id = self.mob_id
             if mob_id:
-                return self.root.content.mob_dict.get(self.mob_id, None)
+                return self.root.content.find_by_mob_id(self.mob_id)
 
     @property
     def track(self):
         mob = self.mob
         if mob:
             for track in mob.tracks:
                 if track.index == self.track_id and track.component and self.media_kind == track.component.media_kind:
```

### Comparing `pyavb-1.3.0/src/avb/core.py` & `pyavb-1.4.0/src/avb/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,29 +45,41 @@
     def items(self):
         for key, value in super(AVBPropertyData, self).items():
             yield key, self.deref(value)
 
     def get(self, *args, **kwargs):
         return self.deref(super(AVBPropertyData, self).get(*args, **kwargs))
 
+@utils.register_helper_class
 class AVBRefList(list):
     propertydefs = []
-    __slots__ = ('root', 'instance_id', '__weakref__')
+    __slots__ = ('root', 'parent', '__weakref__')
 
     def __new__(cls, *args, **kwargs):
         self = super(AVBRefList, cls).__new__(cls)
         self.root = kwargs.get("root", None)
+        self.parent = kwargs.get("parent", None)
         return self
     # def __init__(self, root):
     #     super(AVBRefList, self).__init__()
     #     self.root = root
 
     def mark_modified(self):
         if not self.root.reading:
-            self.root.add_modified(self)
+            if not hasattr(self, 'class_id'):
+                if self.parent:
+                    self.root.add_modified(self.parent)
+            else:
+                self.root.add_modified(self)
+
+    def copy(self, root, parent=None):
+        obj = root.create.from_name(self.__class__.__name__)
+        for item in self:
+            obj.append(item.copy(root))
+        return obj
 
     def extend(self, x):
         super(AVBRefList, self).extend(x)
         self.mark_modified()
 
     def append(self, x):
         super(AVBRefList, self).append(x)
@@ -202,14 +214,37 @@
 
     def read(self, f):
         pass
 
     def write(self, f):
         pass
 
+    def copy(self, root):
+        obj = root.create.from_name(self.__class__.__name__)
+        for key, value in self.property_data.items():
+            if isinstance(value, AVBObject):
+                obj.property_data[key] = value.copy(root)
+            elif isinstance(value, AVBRefList):
+                obj.property_data[key] = value.copy(root)
+                if value.parent:
+                    obj.property_data[key].parent = obj
+            elif isinstance(value, AVBPropertyData):
+                obj.property_data[key] = value.copy(root)
+            elif isinstance(value, list):
+                obj.property_data[key] = []
+                for item in value:
+                    if isinstance(item, AVBObject):
+                        obj.property_data[key].append(item.copy(root))
+                    else:
+                        obj.property_data[key].append(item)
+            else:
+                obj.property_data[key] = value
+
+        return obj
+
     @property
     def media_kind(self):
         return None
 
     def __repr__(self):
         s = "%s.%s"  % (self.__class__.__module__,
                                 self.__class__.__name__)
```

### Comparing `pyavb-1.3.0/src/avb/essence.py` & `pyavb-1.4.0/src/avb/essence.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
     def read(self, f):
         super(MultiDescriptor, self).read(f)
         ctx = self.root.ictx
         ctx.read_assert_tag(f, 0x02)
         ctx.read_assert_tag(f, 0x01)
 
         count = ctx.read_s32(f)
-        self.descriptors = AVBRefList.__new__(AVBRefList, root=self.root)
+        self.descriptors = AVBRefList.__new__(AVBRefList, root=self.root, parent=self)
         for i in range(count):
             ref = ctx.read_object_ref(self.root, f)
             self.descriptors.append(ref)
 
         ctx.read_assert_tag(f, 0x03)
 
     def write(self, f):
@@ -508,15 +508,15 @@
             ctx.write_u8(f, 77)
             ctx.write_s64(f, self.sub_frame_alignment)
 
         if hasattr(self, 'origin'):
             ctx.write_u8(f, 0x01)
             ctx.write_u8(f, 0x02)
             ctx.write_u8(f, 77)
-            ctx.write_string(f, self.origin)
+            ctx.write_u64(f, self.origin)
 
         ctx.write_u8(f, 0x03)
 
 
 @utils.register_class
 class DIDDescriptor(MediaFileDescriptor):
     class_id = b'DIDD'
@@ -1307,7 +1307,73 @@
             ctx.write_u8(f, 72)
             ctx.write_u32(f, self.alpha_min_ref)
 
             ctx.write_u8(f, 72)
             ctx.write_u32(f, self.alpha_max_ref)
 
         ctx.write_u8(f, 0x03)
+
+
+@utils.register_class
+class DataDescriptor(MediaFileDescriptor):
+    class_id = b'DATD'
+    propertydefs = MediaFileDescriptor.propertydefs + [
+        AVBPropertyDef("is_offset_to_frame_indexes_valid", "OMFI:DATD:IsOffsetToFrameIndexesValid", 'bool'),
+        AVBPropertyDef("offset_to_frame_indexes",          "OMFI:DATD:OffsetToFrameIndexes",        'uint64'),
+        AVBPropertyDef("first_frame_offset",               "OMFI:DATD:FirstFrameOffset",            'int32'),
+        AVBPropertyDef("min_sample_size",                  "OMFI:DATD:MinSampleSize",               'int32'),
+        AVBPropertyDef("max_sample_size",                  "OMFI:DATD:MaxSampleSize",               'int32'),
+    ]
+    __slots__ = ()
+
+    def read(self, f):
+        super(DataDescriptor, self).read(f)
+        ctx = self.root.ictx
+        ctx.read_assert_tag(f, 0x02)
+        ctx.read_assert_tag(f, 0x01)
+
+        self.is_offset_to_frame_indexes_valid = ctx.read_bool(f)
+        self.offset_to_frame_indexes = ctx.read_u64(f)
+        self.first_frame_offset = ctx.read_s32(f)
+        self.min_sample_size = ctx.read_s32(f)
+        self.max_sample_size = ctx.read_s32(f)
+
+    def write(self, f):
+        super(DataDescriptor, self).write(f)
+        ctx = self.root.octx
+        ctx.write_u8(f, 0x02)
+        ctx.write_u8(f, 0x01)
+
+        ctx.write_bool(f, self.is_offset_to_frame_indexes_valid)
+        ctx.write_u64(f, self.offset_to_frame_indexes)
+        ctx.write_s32(f, self.first_frame_offset)
+        ctx.write_s32(f, self.min_sample_size)
+        ctx.write_s32(f, self.max_sample_size)
+
+@utils.register_class
+class ANCDataDescriptor(DataDescriptor):
+    class_id = b'ANCD'
+    propertydefs = DataDescriptor.propertydefs + [
+        AVBPropertyDef("manifest_element_count",  "OMFI:ANCD:ManifestElementCount",  'int32'),
+    ]
+
+    __slots__ = ()
+
+    def read(self, f):
+        super(ANCDataDescriptor, self).read(f)
+        ctx = self.root.ictx
+        ctx.read_assert_tag(f, 0x02)
+        ctx.read_assert_tag(f, 0x01)
+
+        self.manifest_element_count = ctx.read_s32(f)
+
+        ctx.read_assert_tag(f, 0x03)
+
+    def write(self, f):
+        super(ANCDataDescriptor, self).write(f)
+        ctx = self.root.octx
+        ctx.write_u8(f, 0x02)
+        ctx.write_u8(f, 0x01)
+
+        ctx.write_s32(f, self.manifest_element_count)
+
+        ctx.write_u8(f, 0x03)
```

### Comparing `pyavb-1.3.0/src/avb/file.py` & `pyavb-1.4.0/src/avb/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,20 +62,22 @@
 
     def __getattr__(self, name):
         self.class_name = name
         return self.create_instance
 
     def from_name(self, name, *args, **kwargs):
 
-        classobj = obj_class = utils.AVBClassName_dict.get(name, None)
+        classobj = utils.AVBClassName_dict.get(name, None)
+        if not classobj:
+            raise ValueError("could not find class for: " + name)
 
         # obj = classobj(None, *args, **kwargs)
         obj = classobj.__new__(classobj)
         obj.root = self.root
-        if obj.class_id:
+        if hasattr(obj, "class_id") and obj.class_id:
             self.root.next_object_id += 1
             obj.instance_id = self.root.next_object_id
 
             self.root.modified_objects[obj.instance_id] = obj
             self.root.object_cache[obj.instance_id] = obj
 
         obj.__init__(*args, **kwargs)
@@ -105,14 +107,17 @@
         self.reading = False
 
         self.create = AVBFactory(self)
         self.object_cache = WeakValueDictionary()
         self.modified_objects = {}
         self.next_object_id = 0
 
+        self.octx = None
+        self.ictx = None
+
         if fileobject is None:
             self.setup_empty()
             return
 
         if is_fileobject_like(fileobject):
             self.f = fileobject
         else:
@@ -315,14 +320,16 @@
             chunk = AVBChunk(self, class_id, pos, len(data))
             print(chunk.class_id)
             print(chunk.hex())
             raise NotImplementedError(chunk.class_id)
 
     def write_object(self, f, obj):
         buffer = io.BytesIO()
+        if self.octx != obj.root.octx:
+            raise ValueError("object is from different file: " + str(obj))
         obj.write(buffer)
         data = buffer.getvalue()
         assert data[-1:] == b'\x03'
         ctx = self.octx
 
         ctx.write_fourcc(f, obj.class_id)
         ctx.write_u32(f, len(data))
@@ -339,30 +346,32 @@
         #     raise Exception()
 
     def write(self, path, byte_order='little'):
         self.next_chunk_id = 0
         self.ref_mapping = {}
         ctx = AVBIOContext(byte_order)
         self.octx = ctx
-
-        with io.open(path, 'wb') as f:
-            count_pos = self.write_header(f)
-            for obj in walk_references(self.content):
-                if obj.instance_id in self.ref_mapping:
-                    continue
-
-                self.next_chunk_id += 1
-                self.ref_mapping[obj.instance_id] = self.next_chunk_id
-                self.write_object(f, obj)
-
-            pos = f.tell()
-            f.seek(count_pos)
-            ctx.write_u32(f, self.next_chunk_id)
-            ctx.write_u32(f, self.next_chunk_id)
-            f.seek(pos)
+        try:
+            with io.open(path, 'wb') as f:
+                count_pos = self.write_header(f)
+                for obj in walk_references(self.content):
+                    if obj.instance_id in self.ref_mapping:
+                        continue
+
+                    self.next_chunk_id += 1
+                    self.ref_mapping[obj.instance_id] = self.next_chunk_id
+                    self.write_object(f, obj)
+
+                pos = f.tell()
+                f.seek(count_pos)
+                ctx.write_u32(f, self.next_chunk_id)
+                ctx.write_u32(f, self.next_chunk_id)
+                f.seek(pos)
+        finally:
+            self.octx = None
 
     def chunks(self):
         for i in range(len(self.object_positions)):
             yield self.read_chunk(i)
 
     def iter_class_ids(self, class_id_list):
         for i, chunk in enumerate(self.chunks()):
```

### Comparing `pyavb-1.3.0/src/avb/interpolation.py` & `pyavb-1.4.0/src/avb/interpolation.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,17 +141,15 @@
     #      /|<- result
     #     / |
     #    /  |
     #   /   |
     #  /    |
     # /p0---p2
     y = (p1[1] - p0[1]) * (p2[0] - p0[0]) / (p1[0] - p0[0])
-    p.y = p0.y + y;
-    p.x = p2.x;
-    return [p2[0], p[1] + y]
+    return [p2[0], p0[1] + y]
 
 def bezier_interpolate(p0, p1, p2, p3, x):
 
     # degenerate cases 1
     # p0 is after p3
     if p0[0] >= p3[0]:
         return p[1]
```

### Comparing `pyavb-1.3.0/src/avb/ioctx.py` & `pyavb-1.4.0/src/avb/ioctx.py`

 * *Files identical despite different names*

### Comparing `pyavb-1.3.0/src/avb/misc.py` & `pyavb-1.4.0/src/avb/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -987,15 +987,15 @@
     def read(self, f):
         super(TrackerDataSlot, self).read(f)
         ctx = self.root.ictx
         ctx.read_assert_tag(f, 0x02)
         ctx.read_assert_tag(f, 0x01)
 
         count = ctx.read_s32(f)
-        self.tracker_data = AVBRefList.__new__(AVBRefList, root=self.root)
+        self.tracker_data = AVBRefList.__new__(AVBRefList, root=self.root, parent=self)
         for i in range(count):
             ref = ctx.read_object_ref(self.root, f)
             self.tracker_data.append(ref)
 
         for tag in ctx.iter_ext(f):
             if tag == 0x01:
                 ctx.read_assert_tag(f, 66)
@@ -1041,15 +1041,15 @@
         ctx.read_assert_tag(f, 0x01)
         size = ctx.read_s16(f)
         assert size >= 0
         self.settings = bytearray(f.read(size))
 
         count = ctx.read_s32(f)
         assert count >= 0
-        self.params = AVBRefList.__new__(AVBRefList, root=self.root)
+        self.params = AVBRefList.__new__(AVBRefList, root=self.root, parent=self)
         for i in range(count):
             ref = ctx.read_object_ref(self.root, f)
             self.params.append(ref)
 
         ctx.read_assert_tag(f, 0x03)
 
     def write(self, f):
@@ -1091,15 +1091,15 @@
         ctx.read_assert_tag(f, 0x01)
 
         setting_size = ctx.read_s16(f)
         self.settings = bytearray(f.read(setting_size))
         self.clip_version = ctx.read_u32(f)
 
         count = ctx.read_s16(f)
-        self.clips = AVBRefList.__new__(AVBRefList, root=self.root)
+        self.clips = AVBRefList.__new__(AVBRefList, root=self.root, parent=self)
         for i in range(count):
             ref = ctx.read_object_ref(self.root, f)
             self.clips.append(ref)
 
         for tag in ctx.iter_ext(f):
             if tag == 0x01:
                 ctx.read_assert_tag(f, 72)
```

### Comparing `pyavb-1.3.0/src/avb/mobid.py` & `pyavb-1.4.0/src/avb/mobid.py`

 * *Files identical despite different names*

### Comparing `pyavb-1.3.0/src/avb/parameter_uuids.py` & `pyavb-1.4.0/src/avb/parameter_uuids.py`

 * *Files identical despite different names*

### Comparing `pyavb-1.3.0/src/avb/trackgroups.py` & `pyavb-1.4.0/src/avb/trackgroups.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
     absolute_import,
     print_function,
     division,
     )
 import datetime
 
 from . import core
-from .core import AVBPropertyDef, AVBRefList
-from .components import Component
+from .core import AVBPropertyDef, walk_references
 from . import utils
 from . import mobid
 from . utils import peek_data
+from .components import Component, SourceClip
 
 TRACK_LABEL_FLAG            = 1 << 0
 TRACK_ATTRIBUTES_FLAG       = 1 << 1
 TRACK_COMPONENT_FLAG        = 1 << 2
 TRACK_FILLER_PROXY_FLAG     = 1 << 3
 TRACK_BOB_DATA_FLAG         = 1 << 4
 TRACK_CONTROL_CODE_FLAG     = 1 << 5
@@ -221,14 +221,42 @@
             for i in range(len(self.tracks)):
                 ctx.write_u8(f, 69)
                 if hasattr(self.tracks[i], 'lock_number'):
                     ctx.write_s16(f, self.tracks[i].lock_number)
                 else:
                     ctx.write_s16(f, 0)
 
+    def dependant_mobs(self):
+        """
+            Yields all mobs that this mob is dependant on in depth first order.
+        """
+
+        visited = set()
+        stack = [self]
+
+        while stack:
+            mob = stack[-1]
+            children_processed = True
+
+            for obj in walk_references(mob):
+                if isinstance(obj, SourceClip):
+                    ref_mob = obj.mob
+                    if not ref_mob:
+                        continue
+                    if ref_mob.mob_id not in visited:
+                        stack.append(ref_mob)
+                        children_processed = False
+
+            if children_processed:
+                stack.pop(-1)
+                if mob.mob_id not in visited:
+                    visited.add(mob.mob_id)
+                    if mob is not self:
+                        yield mob
+
 
 @utils.register_class
 class TrackEffect(TrackGroup):
     class_id = b'TKFX'
     propertydefs_dict = {}
     propertydefs = TrackGroup.propertydefs + [
         AVBPropertyDef('left_length',         'OMFI:TKFX:MC:LeftLength',            'int32'),
```

### Comparing `pyavb-1.3.0/src/avb/utils.py` & `pyavb-1.4.0/src/avb/utils.py`

 * *Files identical despite different names*

### Comparing `pyavb-1.3.0/src/pyavb.egg-info/PKG-INFO` & `pyavb-1.4.0/src/pyavb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyavb
-Version: 1.3.0
+Version: 1.4.0
 Summary: A python module for the reading and writing Avid Bin Files files.
 Home-page: https://github.com/markreidvfx/pyavb
 Author: Mark Reid
 Author-email: mindmark@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/markreidvfx/pyavb
 Project-URL: Documentation, http://pyavb.readthedocs.io
```

