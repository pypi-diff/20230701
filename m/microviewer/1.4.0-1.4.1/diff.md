# Comparing `tmp/microviewer-1.4.0.tar.gz` & `tmp/microviewer-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microviewer-1.4.0.tar", last modified: Fri Jun 30 19:53:17 2023, max compression
+gzip compressed data, was "microviewer-1.4.1.tar", last modified: Sat Jul  1 18:43:23 2023, max compression
```

## Comparing `microviewer-1.4.0.tar` & `microviewer-1.4.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-30 19:53:17.001271 microviewer-1.4.0/
--rw-r--r--   0 wms        (501) staff       (20)       52 2023-06-30 19:53:16.000000 microviewer-1.4.0/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)     2758 2023-06-30 19:53:16.000000 microviewer-1.4.0/ChangeLog
--rw-r--r--   0 wms        (501) staff       (20)    26526 2023-06-05 21:07:17.000000 microviewer-1.4.0/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)       65 2023-06-30 16:44:34.000000 microviewer-1.4.0/MANIFEST.in
--rw-r--r--   0 wms        (501) staff       (20)     2663 2023-06-30 19:53:17.001457 microviewer-1.4.0/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)     1649 2023-06-28 21:32:21.000000 microviewer-1.4.0/README.md
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-30 19:53:16.989706 microviewer-1.4.0/microviewer/
--rw-r--r--   0 wms        (501) staff       (20)     6155 2023-06-30 18:35:40.000000 microviewer-1.4.0/microviewer/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     9295 2023-06-30 16:44:34.000000 microviewer-1.4.0/microviewer/crackle.js
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-30 19:53:17.000409 microviewer-1.4.0/microviewer/cursors/
--rwxr-xr-x   0 wms        (501) staff       (20)      617 2023-06-23 03:27:00.000000 microviewer-1.4.0/microviewer/cursors/exact-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      612 2023-06-23 03:27:00.000000 microviewer-1.4.0/microviewer/cursors/exact.png
--rwxr-xr-x   0 wms        (501) staff       (20)      926 2023-06-23 03:27:00.000000 microviewer-1.4.0/microviewer/cursors/large-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      946 2023-06-23 03:27:00.000000 microviewer-1.4.0/microviewer/cursors/large.png
--rwxr-xr-x   0 wms        (501) staff       (20)      563 2023-06-23 03:27:00.000000 microviewer-1.4.0/microviewer/cursors/medium-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      560 2023-06-23 03:27:00.000000 microviewer-1.4.0/microviewer/cursors/medium.png
--rwxr-xr-x   0 wms        (501) staff       (20)      348 2023-06-23 03:27:00.000000 microviewer-1.4.0/microviewer/cursors/small-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      339 2023-06-23 03:27:00.000000 microviewer-1.4.0/microviewer/cursors/small.png
--rw-r--r--   0 wms        (501) staff       (20)    48063 2023-06-30 19:17:20.000000 microviewer-1.4.0/microviewer/datacube.js
--rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-05 21:09:00.000000 microviewer-1.4.0/microviewer/favicon.ico
--rw-r--r--   0 wms        (501) staff       (20)    31097 2023-06-30 19:47:12.000000 microviewer-1.4.0/microviewer/index.html
--rw-r--r--   0 wms        (501) staff       (20)    87462 2023-06-06 04:26:20.000000 microviewer-1.4.0/microviewer/jquery-3.7.0.min.js
--rwxr-xr-x   0 wms        (501) staff       (20)   333433 2023-06-30 16:44:34.000000 microviewer-1.4.0/microviewer/libcrackle.wasm
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-30 19:53:16.996987 microviewer-1.4.0/microviewer.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)     2663 2023-06-30 19:53:16.000000 microviewer-1.4.0/microviewer.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)      871 2023-06-30 19:53:16.000000 microviewer-1.4.0/microviewer.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-30 19:53:16.000000 microviewer-1.4.0/microviewer.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)       47 2023-06-30 19:53:16.000000 microviewer-1.4.0/microviewer.egg-info/entry_points.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-06 04:24:32.000000 microviewer-1.4.0/microviewer.egg-info/not-zip-safe
--rw-r--r--   0 wms        (501) staff       (20)       46 2023-06-30 19:53:16.000000 microviewer-1.4.0/microviewer.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)       12 2023-06-30 19:53:16.000000 microviewer-1.4.0/microviewer.egg-info/requires.txt
--rw-r--r--   0 wms        (501) staff       (20)       28 2023-06-30 19:53:16.000000 microviewer-1.4.0/microviewer.egg-info/top_level.txt
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-30 19:53:17.000946 microviewer-1.4.0/microviewer_cli/
--rw-r--r--   0 wms        (501) staff       (20)       18 2023-06-06 04:44:54.000000 microviewer-1.4.0/microviewer_cli/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     4473 2023-06-30 17:53:12.000000 microviewer-1.4.0/microviewer_cli/cli.py
--rw-r--r--   0 wms        (501) staff       (20)       11 2023-06-06 04:58:06.000000 microviewer-1.4.0/requirements.txt
--rw-r--r--   0 wms        (501) staff       (20)   297931 2023-06-28 20:05:35.000000 microviewer-1.4.0/seg-demo.png
--rw-r--r--   0 wms        (501) staff       (20)     1032 2023-06-30 19:53:17.002122 microviewer-1.4.0/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)      298 2023-06-28 20:10:25.000000 microviewer-1.4.0/setup.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-01 18:43:23.284656 microviewer-1.4.1/
+-rw-r--r--   0 wms        (501) staff       (20)       52 2023-07-01 18:43:23.000000 microviewer-1.4.1/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)     2941 2023-07-01 18:43:23.000000 microviewer-1.4.1/ChangeLog
+-rw-r--r--   0 wms        (501) staff       (20)    26526 2023-06-05 21:07:17.000000 microviewer-1.4.1/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)       65 2023-06-30 16:44:34.000000 microviewer-1.4.1/MANIFEST.in
+-rw-r--r--   0 wms        (501) staff       (20)     2663 2023-07-01 18:43:23.284840 microviewer-1.4.1/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)     1649 2023-06-28 21:32:21.000000 microviewer-1.4.1/README.md
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-01 18:43:23.278924 microviewer-1.4.1/microviewer/
+-rw-r--r--   0 wms        (501) staff       (20)     6155 2023-06-30 18:35:40.000000 microviewer-1.4.1/microviewer/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     9295 2023-06-30 16:44:34.000000 microviewer-1.4.1/microviewer/crackle.js
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-01 18:43:23.283769 microviewer-1.4.1/microviewer/cursors/
+-rwxr-xr-x   0 wms        (501) staff       (20)      617 2023-06-23 03:27:00.000000 microviewer-1.4.1/microviewer/cursors/exact-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      612 2023-06-23 03:27:00.000000 microviewer-1.4.1/microviewer/cursors/exact.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      926 2023-06-23 03:27:00.000000 microviewer-1.4.1/microviewer/cursors/large-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      946 2023-06-23 03:27:00.000000 microviewer-1.4.1/microviewer/cursors/large.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      563 2023-06-23 03:27:00.000000 microviewer-1.4.1/microviewer/cursors/medium-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      560 2023-06-23 03:27:00.000000 microviewer-1.4.1/microviewer/cursors/medium.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      348 2023-06-23 03:27:00.000000 microviewer-1.4.1/microviewer/cursors/small-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      339 2023-06-23 03:27:00.000000 microviewer-1.4.1/microviewer/cursors/small.png
+-rw-r--r--   0 wms        (501) staff       (20)    42363 2023-07-01 18:42:55.000000 microviewer-1.4.1/microviewer/datacube.js
+-rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-05 21:09:00.000000 microviewer-1.4.1/microviewer/favicon.ico
+-rw-r--r--   0 wms        (501) staff       (20)    31097 2023-06-30 19:47:12.000000 microviewer-1.4.1/microviewer/index.html
+-rw-r--r--   0 wms        (501) staff       (20)    87462 2023-06-06 04:26:20.000000 microviewer-1.4.1/microviewer/jquery-3.7.0.min.js
+-rwxr-xr-x   0 wms        (501) staff       (20)   333433 2023-06-30 16:44:34.000000 microviewer-1.4.1/microviewer/libcrackle.wasm
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-01 18:43:23.282141 microviewer-1.4.1/microviewer.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)     2663 2023-07-01 18:43:23.000000 microviewer-1.4.1/microviewer.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)      871 2023-07-01 18:43:23.000000 microviewer-1.4.1/microviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-07-01 18:43:23.000000 microviewer-1.4.1/microviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)       47 2023-07-01 18:43:23.000000 microviewer-1.4.1/microviewer.egg-info/entry_points.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-06 04:24:32.000000 microviewer-1.4.1/microviewer.egg-info/not-zip-safe
+-rw-r--r--   0 wms        (501) staff       (20)       46 2023-07-01 18:43:23.000000 microviewer-1.4.1/microviewer.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)       12 2023-07-01 18:43:23.000000 microviewer-1.4.1/microviewer.egg-info/requires.txt
+-rw-r--r--   0 wms        (501) staff       (20)       28 2023-07-01 18:43:23.000000 microviewer-1.4.1/microviewer.egg-info/top_level.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-01 18:43:23.284320 microviewer-1.4.1/microviewer_cli/
+-rw-r--r--   0 wms        (501) staff       (20)       18 2023-06-06 04:44:54.000000 microviewer-1.4.1/microviewer_cli/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     5009 2023-07-01 18:00:31.000000 microviewer-1.4.1/microviewer_cli/cli.py
+-rw-r--r--   0 wms        (501) staff       (20)       11 2023-06-06 04:58:06.000000 microviewer-1.4.1/requirements.txt
+-rw-r--r--   0 wms        (501) staff       (20)   297931 2023-06-28 20:05:35.000000 microviewer-1.4.1/seg-demo.png
+-rw-r--r--   0 wms        (501) staff       (20)     1032 2023-07-01 18:43:23.285490 microviewer-1.4.1/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)      298 2023-06-28 20:10:25.000000 microviewer-1.4.1/setup.py
```

### Comparing `microviewer-1.4.0/ChangeLog` & `microviewer-1.4.1/ChangeLog`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+1.4.1
+-----
+
+* refactor: make HyperVolume a child class of SegmentationVolume
+* fix: painting was broken for rectangular images
+* fix: automatically select a new port if 8080 in use
+
 1.4.0
 -----
 
 * ui: add some help text to the save options
 * ui: display memory usage
 * fix: preload cursor images
 * feat: add show unselected rendering mode to hyperview
```

### Comparing `microviewer-1.4.0/LICENSE` & `microviewer-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.0/PKG-INFO` & `microviewer-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microviewer
-Version: 1.4.0
+Version: 1.4.1
 Summary: Visualize 3D numpy arrays in the browser.
 Home-page: https://github.com/seung-lab/microviewer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microviewer-1.4.0/README.md` & `microviewer-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.0/microviewer/__init__.py` & `microviewer-1.4.1/microviewer/__init__.py`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.0/microviewer/crackle.js` & `microviewer-1.4.1/microviewer/crackle.js`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.0/microviewer/cursors/exact-active.png` & `microviewer-1.4.1/microviewer/cursors/exact-active.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.0/microviewer/cursors/exact.png` & `microviewer-1.4.1/microviewer/cursors/exact.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.0/microviewer/cursors/large-active.png` & `microviewer-1.4.1/microviewer/cursors/large-active.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.0/microviewer/cursors/large.png` & `microviewer-1.4.1/microviewer/cursors/large.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.0/microviewer/cursors/medium-active.png` & `microviewer-1.4.1/microviewer/cursors/medium-active.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.0/microviewer/cursors/medium.png` & `microviewer-1.4.1/microviewer/cursors/medium.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.0/microviewer/datacube.js` & `microviewer-1.4.1/microviewer/datacube.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -207,14 +207,18 @@
             .map((segid) => _this.renumbering[segid]);
     }
 
     get(x, y, z) {
         return this.renumbering[this.channel.get(x, y, z)];
     }
 
+    getSegmentation() {
+        return this.channel;
+    }
+
     clearSelected() {
         this.segments = {};
     }
 
     load(url, progressfn) {
         const _this = this;
         return super.load(url, progressfn)
@@ -231,28 +235,28 @@
 
     render(ctx, axis, slice) {
         let _this = this;
 
         const hover_id = this.hover_id;
         const cache = this.cache;
 
-        const size = this.channel.faceDimensions(axis);
+        const size = this.getSegmentation().faceDimensions(axis);
         const hover_enabled = (size[0] * size[1]) < 1024 * 1024 * 2;
 
         if (cache.valid &&
             cache.pixels &&
             cache.axis === axis &&
             cache.slice === slice &&
             (!hover_enabled || (cache.segid === hover_id))) {
 
             ctx.putImageData(cache.pixels, 0, 0);
             return;
         }
 
-        let seg_slice = this.channel.slice(axis, slice, /*copy=*/ false);
+        let seg_slice = this.getSegmentation().slice(axis, slice, /*copy=*/ false);
 
         let pixels = ctx.getImageData(0, 0, size[0], size[1]);
         let pixels32 = new Uint32Array(pixels.data.buffer);
 
         const color_assignments = this.assigned_colors;
         const brightener = this.colorToUint32({
             r: 10,
@@ -266,15 +270,15 @@
             b: 200
         }, 1);
 
         let segments = this.segments;
         let show_all = true;
         const show_unselected = this.show_unselected;
 
-        let ArrayType = this.channel.arrayType();
+        let ArrayType = this.getSegmentation().arrayType();
         let segarray = new Uint8Array(this.renumbering.length);
         Object.keys(segments).forEach((label) => {
             segarray[label] = !!segments[label];
             show_all &&= !segments[label];
         });
 
         // We sometimes disable the hover highlight to get more performance
@@ -332,17 +336,17 @@
      *
      * Return: segid
      */
     toggleSegment(axis, slice, normx, normy) {
         let _this = this;
         let x, y, z;
 
-        let sizex = _this.channel.size.x,
-            sizey = _this.channel.size.y,
-            sizez = _this.channel.size.z;
+        let sizex = _this.getSegmentation().size.x,
+            sizey = _this.getSegmentation().size.y,
+            sizez = _this.getSegmentation().size.z;
 
         if (axis === 'x') {
             x = slice,
                 y = normx * sizey,
                 z = normy * sizez;
         } else if (axis === 'y') {
             x = normx * sizex,
@@ -354,26 +358,26 @@
                 z = slice;
         }
 
         x = Math.floor(x);
         y = Math.floor(y);
         z = Math.floor(z);
 
-        let segid = _this.channel.get(x, y, z);
+        let segid = _this.getSegmentation().get(x, y, z);
 
         if (segid > 0) {
             _this.segments[segid] = !_this.segments[segid];
         }
 
         return segid;
     }
 
     selectSegment(segid) {
         let _this = this;
-        segid = _this.channel.cast(segid);
+        segid = _this.getSegmentation().cast(segid);
         segid = _this.renumbering.indexOf(segid);
         if (segid !== -1) {
             _this.segments[segid] = true;
         }
     }
 
     /* getSegsInCircle
@@ -386,19 +390,19 @@
      *   cx: 0..1, X coordinate of circle center
      *   cy: 0..1, Y coordinate of circle center
      *
      * Return: [ segids ]
      */
     getSegsInCircle(axis, slice, d, cx, cy) {
         let _this = this;
-        let [width, height] = _this.channel.faceDimensions(axis);
+        let [width, height] = _this.getSegmentation().faceDimensions(axis);
 
         // Nullify anything outside the ellipse. Just like a GRE problem.
 
-        let buffer = _this.channel.slice(axis, slice, /*copy=*/ false);
+        let buffer = _this.getSegmentation().slice(axis, slice, /*copy=*/ false);
 
         cx = Math.floor(cx * width) + 0.5;
         cy = Math.floor(cy * height) + 0.5;
 
         let dx = d * width,
             dy = d * height;
 
@@ -449,15 +453,15 @@
         segs.forEach((segid) => {
             _this.segments[segid] = false;
         });
     }
 
     paintCircle(axis, slice, d, cx, cy, label) {
         let _this = this;
-        let [width, height] = _this.channel.faceDimensions(axis);
+        let [width, height] = _this.getSegmentation().faceDimensions(axis);
 
         if (_this.inverse_renumbering[label] === undefined) {
             _this.renumbering[_this.max_label] = label;
             _this.inverse_renumbering[label] = _this.max_label;
             _this.assigned_colors[_this.max_label] = _this.colorToUint32({
                 r: 0,
                 g: 230,
@@ -478,49 +482,51 @@
             rx2 = dx * dx / 4,
             ry = dy / 2,
             ry2 = dy * dy / 4;
 
         let x0 = Math.max(0, Math.trunc(cx - rx) + 0.5),
             xf = Math.min(width, Math.trunc(cx + rx) + 0.5),
             y0 = Math.max(0, Math.trunc(cy - ry) + 0.5),
-            yf = Math.min(width, Math.trunc(cy + ry) + 0.5);
+            yf = Math.min(height, Math.trunc(cy + ry) + 0.5);
 
         let segid = 0,
             bounds_test = 0.0;
 
         // For anisotropic data, we need to distort our circle (UI) into an ellipse 
         // since we've distorted the data to be square.
         // eqn of an ellipse: ((x - h)^2 / rx^2) + ((y - k)^2 / ry^2) <= 1
         // We'll use < instead of <= though to exclude the boundary
-        let cube = _this.channel.cube;
+        let cube = _this.getSegmentation().cube;
+        const sx = _this.getSegmentation().size.x;
+        const sy = _this.getSegmentation().size.y;
 
         if (axis == 'z') {
             for (var y = y0; y <= yf; y++) {
                 for (var x = x0; x <= xf; x++) {
                     bounds_test = ((x - cx) * (x - cx) / rx2) + ((y - cy) * (y - cy) / ry2);
                     if (bounds_test < 1) {
-                        cube[(x | 0) + width * ((y | 0) + height * (slice | 0))] = label;
+                        cube[(x | 0) + sx * ((y | 0) + sy * (slice | 0))] = label;
                     }
                 }
             }
         } else if (axis == 'y') {
             for (var z = y0; z <= yf; z++) {
                 for (var x = x0; x <= xf; x++) {
                     bounds_test = ((x - cx) * (x - cx) / rx2) + ((z - cy) * (z - cy) / ry2);
                     if (bounds_test < 1) {
-                        cube[(x | 0) + width * ((slice | 0) + height * (z | 0))] = label;
+                        cube[(x | 0) + sx * ((slice | 0) + sy * (z | 0))] = label;
                     }
                 }
             }
         } else if (axis === 'x') {
             for (var z = y0; z <= yf; z++) {
                 for (var y = x0; y <= xf; y++) {
                     bounds_test = ((y - cx) * (y - cx) / rx2) + ((z - cy) * (z - cy) / ry2);
                     if (bounds_test < 1) {
-                        cube[(slice | 0) + width * ((y | 0) + height * (z | 0))] = label;
+                        cube[(slice | 0) + sx * ((y | 0) + sy * (z | 0))] = label;
                     }
                 }
             }
         } else {
             throw new Error("Unsupported axis.")
         }
     }
@@ -536,17 +542,17 @@
  *   channel: A blankable Datacube representing the channel values. 
  *        Since they're grayscale, an efficient representation is 1 byte
  *   segmentation: A blankable Datacube representing segmentation values.
  *      Seg ids don't appear to rise above the high thousands, so 2 bytes is probably sufficent.
  *
  * Return: HyperVolume object
  */
-class HyperVolume extends MonoVolume {
+class HyperVolume extends SegmentationVolume {
     constructor(channel, segmentation) {
-        super(channel);
+        super(segmentation);
         this.channel = channel; // a data cube
         this.segmentation = segmentation; // a segmentation cube
 
         this.renumbering = new segmentation.cube.constructor(1);
         this.inverse_renumbering = {};
         this.has_segmentation = true;
         this.max_label = 0;
@@ -554,42 +560,35 @@
         this.show_unselected = false;
         this.max_label = 0;
 
         this.segments = {};
         this.alpha = 0.5;
     }
 
-    selected() {
-        let _this = this;
-        return Object.keys(_this.segments)
-            .filter((segid) => _this.segments[segid])
-            .map((segid) => _this.renumbering[segid]);
-    }
-
     get(x, y, z) {
         return [
             this.channel.get(x, y, z),
             this.renumbering[this.segmentation.get(x, y, z)],
         ]
     }
 
+    getSegmentation() {
+        return this.segmentation;
+    }
+
     loaded() {
         return this.channel.loaded && this.segmentation.loaded;
     }
 
     progress() {
         let chan = this.channel;
         let seg = this.segmentation;
         return (chan.bytes * chan.progress + seg.bytes * seg.progress) / (chan.bytes + seg.bytes);
     }
 
-    clearSelected() {
-        this.segments = {};
-    }
-
     /* load
      *
      * Download the channel and segmentation and materialize them into
      * their respective datacubes.
      *
      * Return: promise representing download completion state
      */
@@ -749,220 +748,14 @@
             }
         }
 
         ctx.putImageData(pixels, 0, 0);
 
         return this;
     }
-
-    /* toggleSegment
-     *
-     * Given an axis, slice index, and normalized x and y cursor coordinates
-     * ([0, 1]), 0,0 being the top left, select the segment under the mouse.
-     *
-     * Required:
-     *   [0] axis: 'x', 'y', or 'z'
-     *   [1] slice: 0 - 255
-     *   [2] normx: 0...1
-     *   [3] normy: 0...1
-     *
-     * Return: segid
-     */
-    toggleSegment(axis, slice, normx, normy) {
-        let _this = this;
-        let x, y, z;
-
-        let sizex = _this.segmentation.size.x,
-            sizey = _this.segmentation.size.y,
-            sizez = _this.segmentation.size.z;
-
-        if (axis === 'x') {
-            x = slice,
-                y = normx * sizey,
-                z = normy * sizez;
-        } else if (axis === 'y') {
-            x = normx * sizex,
-                y = slice,
-                z = normy * sizez;
-        } else if (axis === 'z') {
-            x = normx * sizex,
-                y = normy * sizey,
-                z = slice;
-        }
-
-        x = Math.floor(x);
-        y = Math.floor(y);
-        z = Math.floor(z);
-
-        let segid = _this.segmentation.get(x, y, z);
-
-        if (segid > 0) {
-            _this.segments[segid] = !_this.segments[segid];
-        }
-
-        return segid;
-    }
-
-    selectSegment(segid) {
-        let _this = this;
-        segid = _this.segmentation.cast(segid);
-        segid = _this.renumbering.indexOf(segid);
-        if (segid !== -1) {
-            _this.segments[segid] = true;
-        }
-    }
-
-    /* getSegsInCircle
-     *
-     * Get the segids located within a circle. All
-     * parameters are normalized between [0, 1]
-     *
-     * Required:
-     *   d: 0..1, Diameter of the circle
-     *   cx: 0..1, X coordinate of circle center
-     *   cy: 0..1, Y coordinate of circle center
-     *
-     * Return: [ segids ]
-     */
-    getSegsInCircle(axis, slice, d, cx, cy) {
-        let _this = this;
-        let [width, height] = _this.segmentation.faceDimensions(axis);
-
-        // Nullify anything outside the ellipse. Just like a GRE problem.
-
-        let buffer = _this.segmentation.slice(axis, slice, /*copy=*/ false);
-
-        cx = Math.floor(cx * width) + 0.5;
-        cy = Math.floor(cy * height) + 0.5;
-
-        let dx = d * width,
-            dy = d * height;
-
-        let rx = dx / 2,
-            rx2 = dx * dx / 4,
-            ry = dy / 2,
-            ry2 = dy * dy / 4;
-
-        let x0 = Math.max(0, Math.trunc(cx - rx) + 0.5),
-            xf = Math.min(width, Math.trunc(cx + rx) + 0.5),
-            y0 = Math.max(0, Math.trunc(cy - ry) + 0.5),
-            yf = Math.min(width, Math.trunc(cy + ry) + 0.5);
-
-        let segid = 0,
-            bounds_test = 0.0;
-
-        let segids = {};
-
-        // For anisotropic data, we need to distort our circle (UI) into an ellipse 
-        // since we've distorted the data to be square.
-        // eqn of an ellipse: ((x - h)^2 / rx^2) + ((y - k)^2 / ry^2) <= 1
-        // We'll use < instead of <= though to exclude the boundary
-
-        for (var x = x0; x <= xf; x++) {
-            for (var y = y0; y <= yf; y++) {
-                bounds_test = ((x - cx) * (x - cx) / rx2) + ((y - cy) * (y - cy) / ry2);
-                segid = ((bounds_test < 1) && buffer[(x | 0) + width * (y | 0)]) | 0;
-                segids[segid] = true;
-            }
-        }
-
-        delete segids[0];
-
-        return Object.keys(segids).map((segid) => parseInt(segid, 10));
-    }
-
-    selectSegsInCircle(axis, slice, d, cx, cy) {
-        let _this = this;
-        let segs = _this.getSegsInCircle(axis, slice, d, cx, cy);
-        segs.forEach((segid) => {
-            _this.segments[segid] = true;
-        });
-    }
-
-    eraseSegsInCircle(axis, slice, d, cx, cy) {
-        let _this = this;
-        let segs = _this.getSegsInCircle(axis, slice, d, cx, cy);
-        segs.forEach((segid) => {
-            _this.segments[segid] = false;
-        });
-    }
-
-    paintCircle(axis, slice, d, cx, cy, label) {
-        let _this = this;
-        let [width, height] = _this.segmentation.faceDimensions(axis);
-
-        if (_this.inverse_renumbering[label] === undefined) {
-            _this.renumbering[_this.max_label] = label;
-            _this.inverse_renumbering[label] = _this.max_label;
-            _this.assigned_colors[_this.max_label] = _this.colorToUint32({
-                r: 0,
-                g: 230,
-                b: 0
-            }, 1);
-            _this.max_label++;
-        }
-        label = _this.inverse_renumbering[label];
-        _this.segments[label] = true;
-
-        cx = Math.floor(cx * width) + 0.5;
-        cy = Math.floor(cy * height) + 0.5;
-
-        let dx = d * width,
-            dy = d * height;
-
-        let rx = dx / 2,
-            rx2 = dx * dx / 4,
-            ry = dy / 2,
-            ry2 = dy * dy / 4;
-
-        let x0 = Math.max(0, Math.trunc(cx - rx) + 0.5),
-            xf = Math.min(width, Math.trunc(cx + rx) + 0.5),
-            y0 = Math.max(0, Math.trunc(cy - ry) + 0.5),
-            yf = Math.min(width, Math.trunc(cy + ry) + 0.5);
-
-        let segid = 0,
-            bounds_test = 0.0;
-
-        // For anisotropic data, we need to distort our circle (UI) into an ellipse 
-        // since we've distorted the data to be square.
-        // eqn of an ellipse: ((x - h)^2 / rx^2) + ((y - k)^2 / ry^2) <= 1
-        // We'll use < instead of <= though to exclude the boundary
-        let cube = _this.segmentation.cube;
-
-        if (axis == 'z') {
-            for (var y = y0; y <= yf; y++) {
-                for (var x = x0; x <= xf; x++) {
-                    bounds_test = ((x - cx) * (x - cx) / rx2) + ((y - cy) * (y - cy) / ry2);
-                    if (bounds_test < 1) {
-                        cube[(x | 0) + width * ((y | 0) + height * (slice | 0))] = label;
-                    }
-                }
-            }
-        } else if (axis == 'y') {
-            for (var z = y0; z <= yf; z++) {
-                for (var x = x0; x <= xf; x++) {
-                    bounds_test = ((x - cx) * (x - cx) / rx2) + ((z - cy) * (z - cy) / ry2);
-                    if (bounds_test < 1) {
-                        cube[(x | 0) + width * ((slice | 0) + height * (z | 0))] = label;
-                    }
-                }
-            }
-        } else if (axis === 'x') {
-            for (var z = y0; z <= yf; z++) {
-                for (var y = x0; y <= xf; y++) {
-                    bounds_test = ((y - cx) * (y - cx) / rx2) + ((z - cy) * (z - cy) / ry2);
-                    if (bounds_test < 1) {
-                        cube[(slice | 0) + width * ((y | 0) + height * (z | 0))] = label;
-                    }
-                }
-            }
-        } else {
-            throw new Error("Unsupported axis.")
-        }
-    }
 }
 
 class CachedImageData {
     constructor(context) {
         this.context = context;
         this.cache = null;
     }
```

### Comparing `microviewer-1.4.0/microviewer/favicon.ico` & `microviewer-1.4.1/microviewer/favicon.ico`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.0/microviewer/index.html` & `microviewer-1.4.1/microviewer/index.html`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.0/microviewer/jquery-3.7.0.min.js` & `microviewer-1.4.1/microviewer/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.0/microviewer/libcrackle.wasm` & `microviewer-1.4.1/microviewer/libcrackle.wasm`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.0/microviewer.egg-info/PKG-INFO` & `microviewer-1.4.1/microviewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microviewer
-Version: 1.4.0
+Version: 1.4.1
 Summary: Visualize 3D numpy arrays in the browser.
 Home-page: https://github.com/seung-lab/microviewer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microviewer-1.4.0/microviewer.egg-info/SOURCES.txt` & `microviewer-1.4.1/microviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.0/microviewer_cli/cli.py` & `microviewer-1.4.1/microviewer_cli/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -130,18 +130,38 @@
     print(f"File not found: {err.filename}")
     return
 
   if not segmentation and paint:
     segmentation_np = np.zeros(image_np.shape, dtype=np.uint16, order="F")
     segmentation = "PAINTING"
 
+  port = 8080
+  working_port = False
+  for i in range(10):
+    port += 1
+    if not is_port_in_use(port):
+      working_port = True
+      break
+  
+  if not working_port:
+    print("Ports 8080 to 8090 are all in use.")
+    return
+
   if segmentation is not None:
     microviewer.hyperview(
       image_np, segmentation_np, 
       browser=browser, 
       cloudpath=[ image, segmentation ],
+      port=port,
     )
   else:
     microviewer.view(
       image_np, seg=seg, 
-      browser=browser, cloudpath=image
+      browser=browser, cloudpath=image,
+      port=port,
     )
+
+# from: https://stackoverflow.com/questions/2470971/fast-way-to-test-if-a-port-is-in-use-using-python
+def is_port_in_use(port: int) -> bool:
+  import socket
+  with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+    return s.connect_ex(('localhost', port)) == 0
```

### Comparing `microviewer-1.4.0/seg-demo.png` & `microviewer-1.4.1/seg-demo.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.4.0/setup.cfg` & `microviewer-1.4.1/setup.cfg`

 * *Files identical despite different names*

