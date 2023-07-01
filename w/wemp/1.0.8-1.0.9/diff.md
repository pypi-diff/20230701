# Comparing `tmp/wemp-1.0.8-py3-none-any.whl.zip` & `tmp/wemp-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 4932 bytes, number of entries: 8
--rw-rw-r--  2.0 unx     8889 b- defN 23-Jun-28 00:11 wemp/__init__.py
+-rw-rw-r--  2.0 unx     8893 b- defN 23-Jul-01 05:03 wemp/__init__.py
 -rw-rw-r--  2.0 unx      120 b- defN 23-Jun-12 14:45 wemp/__main__.py
 -rw-rw-r--  2.0 unx     1086 b- defN 23-Jun-12 15:33 wemp/http.py
--rw-rw-r--  2.0 unx      269 b- defN 23-Jun-28 00:11 wemp-1.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-28 00:11 wemp-1.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       44 b- defN 23-Jun-28 00:11 wemp-1.0.8.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        5 b- defN 23-Jun-28 00:11 wemp-1.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      590 b- defN 23-Jun-28 00:11 wemp-1.0.8.dist-info/RECORD
-8 files, 11095 bytes uncompressed, 3908 bytes compressed:  64.8%
+-rw-rw-r--  2.0 unx      269 b- defN 23-Jul-01 05:03 wemp-1.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-01 05:03 wemp-1.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       44 b- defN 23-Jul-01 05:03 wemp-1.0.9.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jul-01 05:03 wemp-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      590 b- defN 23-Jul-01 05:03 wemp-1.0.9.dist-info/RECORD
+8 files, 11099 bytes uncompressed, 3908 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: wemp/__main__.py
 Comment: 
 
 Filename: wemp/http.py
 Comment: 
 
-Filename: wemp-1.0.8.dist-info/METADATA
+Filename: wemp-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: wemp-1.0.8.dist-info/WHEEL
+Filename: wemp-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: wemp-1.0.8.dist-info/entry_points.txt
+Filename: wemp-1.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: wemp-1.0.8.dist-info/top_level.txt
+Filename: wemp-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: wemp-1.0.8.dist-info/RECORD
+Filename: wemp-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wemp/__init__.py

```diff
@@ -244,15 +244,15 @@
 
         heart_thread.join()
         return True
         
 class Application:
     def __init__(self):
         self.cfg     = Config()
-        self.actions = Actions(self)
+        self.actions = Actions(self.cfg)
 
     def run_with_command(self, args=None)->bool:
         
         if args is not None and isinstance(args, str):
             args = args.split(" ")
         elif args is None:
             args = sys.argv[1:]
```

