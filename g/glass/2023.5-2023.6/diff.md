# Comparing `tmp/glass-2023.5.tar.gz` & `tmp/glass-2023.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glass-2023.5.tar", last modified: Wed May 31 23:39:52 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `glass-2023.5.tar` & `glass-2023.6.tar`

### file list

```diff
@@ -1,34 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:39:52.298624 glass-2023.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-31 23:39:43.000000 glass-2023.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-31 23:39:52.298624 glass-2023.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-31 23:39:43.000000 glass-2023.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:39:52.298624 glass-2023.5/glass/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-31 23:39:43.000000 glass-2023.5/glass/all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:39:52.298624 glass-2023.5/glass/core/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-31 23:39:43.000000 glass-2023.5/glass/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-31 23:39:43.000000 glass-2023.5/glass/core/array.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-31 23:39:43.000000 glass-2023.5/glass/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:39:52.298624 glass-2023.5/glass/core/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 23:39:43.000000 glass-2023.5/glass/core/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-31 23:39:43.000000 glass-2023.5/glass/core/test/test_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-05-31 23:39:43.000000 glass-2023.5/glass/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-05-31 23:39:43.000000 glass-2023.5/glass/galaxies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-05-31 23:39:43.000000 glass-2023.5/glass/lensing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-05-31 23:39:43.000000 glass-2023.5/glass/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-05-31 23:39:43.000000 glass-2023.5/glass/points.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-05-31 23:39:43.000000 glass-2023.5/glass/shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-05-31 23:39:43.000000 glass-2023.5/glass/shells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:39:52.298624 glass-2023.5/glass/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-31 23:39:43.000000 glass-2023.5/glass/test/test_galaxies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-31 23:39:43.000000 glass-2023.5/glass/test/test_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-31 23:39:43.000000 glass-2023.5/glass/test/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-31 23:39:43.000000 glass-2023.5/glass/test/test_shells.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-31 23:39:43.000000 glass-2023.5/glass/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:39:52.298624 glass-2023.5/glass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-31 23:39:52.000000 glass-2023.5/glass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-31 23:39:52.000000 glass-2023.5/glass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:39:52.000000 glass-2023.5/glass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-31 23:39:52.000000 glass-2023.5/glass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 23:39:52.000000 glass-2023.5/glass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-31 23:39:52.298624 glass-2023.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 23:39:43.000000 glass-2023.5/setup.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 glass-2023.6/.commitlint.rules.js
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 glass-2023.6/.flake8
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 glass-2023.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 glass-2023.6/.readthedocs.yml
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 glass-2023.6/CHANGELOG.md
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 glass-2023.6/CITATION.md
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 glass-2023.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 glass-2023.6/.github/dependabot.yml
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 glass-2023.6/.github/test-constraints.txt
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 glass-2023.6/.github/workflows/pull_request.yml
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 glass-2023.6/.github/workflows/pull_request_review.yml
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 glass-2023.6/.github/workflows/release.yml
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 glass-2023.6/.github/workflows/test.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 glass-2023.6/docs/Makefile
+-rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 glass-2023.6/docs/conf.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 glass-2023.6/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 glass-2023.6/docs/make.bat
+-rw-r--r--   0        0        0    94661 2020-02-02 00:00:00.000000 glass-2023.6/docs/_static/android-chrome-192x192.png
+-rw-r--r--   0        0        0   704232 2020-02-02 00:00:00.000000 glass-2023.6/docs/_static/android-chrome-512x512.png
+-rw-r--r--   0        0        0    85486 2020-02-02 00:00:00.000000 glass-2023.6/docs/_static/apple-touch-icon.png
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 glass-2023.6/docs/_static/favicon-16x16.png
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 glass-2023.6/docs/_static/favicon-32x32.png
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 glass-2023.6/docs/_static/favicon.ico
+-rw-r--r--   0        0        0   867495 2020-02-02 00:00:00.000000 glass-2023.6/docs/_static/logo.png
+-rw-r--r--   0        0        0   623526 2020-02-02 00:00:00.000000 glass-2023.6/docs/_static/spheres.png
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 glass-2023.6/docs/manual/extensions.rst
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 glass-2023.6/docs/manual/first-steps.rst
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 glass-2023.6/docs/manual/get-in-touch.rst
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 glass-2023.6/docs/manual/index.rst
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 glass-2023.6/docs/manual/installation.rst
+-rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 glass-2023.6/docs/manual/releases.rst
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 glass-2023.6/docs/reference/fields.rst
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 glass-2023.6/docs/reference/galaxies.rst
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 glass-2023.6/docs/reference/index.rst
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 glass-2023.6/docs/reference/lensing.rst
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 glass-2023.6/docs/reference/observations.rst
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 glass-2023.6/docs/reference/points.rst
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 glass-2023.6/docs/reference/shapes.rst
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 glass-2023.6/docs/reference/shells.rst
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 glass-2023.6/docs/reference/user.rst
+-rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 glass-2023.6/docs/user/definitions.rst
+-rw-r--r--   0        0        0     6997 2020-02-02 00:00:00.000000 glass-2023.6/docs/user/how-glass-works.rst
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 glass-2023.6/docs/user/index.rst
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 glass-2023.6/docs/user/publications.rst
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 glass-2023.6/glass/__init__.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 glass-2023.6/glass/_version.py
+-rw-r--r--   0        0        0     9341 2020-02-02 00:00:00.000000 glass-2023.6/glass/fields.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 glass-2023.6/glass/galaxies.py
+-rw-r--r--   0        0        0    12328 2020-02-02 00:00:00.000000 glass-2023.6/glass/lensing.py
+-rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 glass-2023.6/glass/observations.py
+-rw-r--r--   0        0        0     9280 2020-02-02 00:00:00.000000 glass-2023.6/glass/points.py
+-rw-r--r--   0        0        0     8335 2020-02-02 00:00:00.000000 glass-2023.6/glass/shapes.py
+-rw-r--r--   0        0        0     8290 2020-02-02 00:00:00.000000 glass-2023.6/glass/shells.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 glass-2023.6/glass/user.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 glass-2023.6/glass/core/__init__.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 glass-2023.6/glass/core/array.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 glass-2023.6/glass/core/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glass-2023.6/glass/core/test/__init__.py
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 glass-2023.6/glass/core/test/test_array.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 glass-2023.6/glass/ext/__init__.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 glass-2023.6/glass/test/test_galaxies.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 glass-2023.6/glass/test/test_lensing.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 glass-2023.6/glass/test/test_points.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 glass-2023.6/glass/test/test_shapes.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 glass-2023.6/glass/test/test_shells.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 glass-2023.6/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 glass-2023.6/LICENSE
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 glass-2023.6/README.md
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 glass-2023.6/pyproject.toml
+-rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 glass-2023.6/PKG-INFO
```

### Comparing `glass-2023.5/LICENSE` & `glass-2023.6/LICENSE`

 * *Files identical despite different names*

### Comparing `glass-2023.5/PKG-INFO` & `glass-2023.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: glass
-Version: 2023.5
-Summary: Generator for Large Scale Structure
-Home-page: https://github.com/glass-dev/glass
-Maintainer: Nicolas Tessore
-Maintainer-email: n.tessore@ucl.ac.uk
-License: MIT
-Project-URL: Documentation, https://glass.readthedocs.io/
-Project-URL: Issues, https://github.com/glass-dev/glass/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: docs
-License-File: LICENSE
-
 
 **GLASS**: Generator for Large Scale Structure
 ==============================================
 
 [![Documentation](https://readthedocs.org/projects/glass/badge/?version=latest)](https://glass.readthedocs.io/en/latest/)
 [![PyPI](https://img.shields.io/pypi/v/glass)](https://pypi.org/project/glass)
 [![arXiv](https://img.shields.io/badge/arXiv-2302.01942-red)](https://arxiv.org/abs/2302.01942)
```

### Comparing `glass-2023.5/glass/core/array.py` & `glass-2023.6/glass/core/array.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,16 @@
                                left=left, right=right, period=period)
 
 
 def trapz_product(f, *ff, axis=-1):
     '''trapezoidal rule for a product of functions'''
     x, _ = f
     for x_, _ in ff:
-        x = np.union1d(x, x_[(x_ > x[0]) & (x_ < x[-1])])
+        x = np.union1d(x[(x >= x_[0]) & (x <= x_[-1])],
+                       x_[(x_ >= x[0]) & (x_ <= x[-1])])
     y = np.interp(x, *f)
     for f_ in ff:
         y *= np.interp(x, *f_)
     return np.trapz(y, x, axis=axis)
 
 
 def cumtrapz(f, x, dtype=None, out=None):
```

### Comparing `glass-2023.5/glass/core/test/test_array.py` & `glass-2023.6/glass/core/test/test_array.py`

 * *Files 19% similar despite different names*

```diff
@@ -86,7 +86,21 @@
     assert np.shape(y) == (2, 3, 4, 1)
     npt.assert_allclose(y, [[[[1.15], [1.25], [1.35], [1.45]],
                              [[1.45], [1.35], [1.25], [1.15]],
                              [[1.15], [1.45], [1.25], [1.35]]],
                             [[[2.15], [2.25], [2.35], [2.45]],
                              [[2.45], [2.35], [2.25], [2.15]],
                              [[2.15], [2.45], [2.25], [2.35]]]], atol=1e-15)
+
+
+def test_trapz_product():
+    from glass.core.array import trapz_product
+
+    x1 = np.linspace(0, 2, 100)
+    f1 = np.full_like(x1, 2.0)
+
+    x2 = np.linspace(1, 2, 10)
+    f2 = np.full_like(x2, 0.5)
+
+    s = trapz_product((x1, f1), (x2, f2))
+
+    assert np.allclose(s, 1.0)
```

### Comparing `glass-2023.5/glass/fields.py` & `glass-2023.6/glass/fields.py`

 * *Files identical despite different names*

### Comparing `glass-2023.5/glass/galaxies.py` & `glass-2023.6/glass/galaxies.py`

 * *Files identical despite different names*

### Comparing `glass-2023.5/glass/observations.py` & `glass-2023.6/glass/observations.py`

 * *Files identical despite different names*

### Comparing `glass-2023.5/glass/points.py` & `glass-2023.6/glass/points.py`

 * *Files 16% similar despite different names*

```diff
@@ -81,15 +81,16 @@
     delta_g = np.log1p(delta)
     delta_g *= b
     np.expm1(delta_g, out=delta_g)
     return delta_g
 
 
 def positions_from_delta(ngal, delta, bias=None, vis=None, *,
-                         bias_model='linear', remove_monopole=False, rng=None):
+                         bias_model='linear', remove_monopole=False,
+                         batch=1_000_000, rng=None):
     '''Generate positions tracing a density contrast.
 
     The map of expected number counts is constructed from the number
     density, density contrast, an optional bias model, and an optional
     visibility map.
 
     If ``remove_monopole`` is set, the monopole of the computed density
@@ -123,19 +124,21 @@
         The bias model to apply.  If a string, refers to a function in
         the :mod:`~glass.points` module, e.g. ``'linear'`` for
         :func:`linear_bias()` or ``'loglinear'`` for
         :func:`loglinear_bias`.
     remove_monopole : bool, optional
         If true, the monopole of the density contrast after biasing is
         fixed to zero.
+    batch : int, optional
+        Maximum number of positions to yield in one batch.
     rng : :class:`~numpy.random.Generator`, optional
         Random number generator.  If not given, a default RNG is used.
 
-    Returns
-    -------
+    Yields
+    ------
     lon, lat : array_like
         Columns of longitudes and latitudes for the sampled points.
     count : int or array_like
         The number of sampled points.  If multiple populations are
         sampled, an array of counts in the shape of the extra
         dimensions is returned.
 
@@ -159,22 +162,14 @@
         inputs += [(vis, 1)]
     dims, ngal, delta, *rest = broadcast_leading_axes(*inputs)
     if bias is not None:
         bias, *rest = rest
     if vis is not None:
         vis, *rest = rest
 
-    # the output arrays, concatenated over all dimensions
-    ntot = 0
-    lon = np.empty(0)
-    lat = np.empty(0)
-
-    # keep track of counts for each leading dimensions
-    count = np.empty(dims, dtype=int)
-
     # iterate the leading dimensions
     for k in np.ndindex(dims):
 
         # compute density contrast from bias model, or copy
         if bias is None:
             n = np.copy(delta[k])
         else:
@@ -194,97 +189,105 @@
 
         # clip number density at zero
         np.clip(n, 0, None, out=n)
 
         # sample actual number in each pixel
         n = rng.poisson(n)
 
+        # total number of points
+        count = n.sum()
+        # don't go through pixels if there are no points
+        if count == 0:
+            continue
+
         # for converting randomly sampled positions to HEALPix indices
         npix = n.shape[-1]
         nside = healpix.npix2nside(npix)
 
-        # number of points for this population
-        count[k] = n.sum()
-
-        # current and new total number of sampled points
-        ncur, ntot = ntot, ntot + count[k]
+        # create a mask to report the count in the right axis
+        if dims:
+            cmask = np.zeros(dims, dtype=int)
+            cmask[k] = 1
+        else:
+            cmask = 1
 
-        # resize the output arrays to hold the new sample
-        lon.resize(ntot, refcheck=False)
-        lat.resize(ntot, refcheck=False)
-
-        # sample batches of 10000 pixels
-        batch = 10_000
-        for i in range(0, npix, batch):
-            r = n[i:i+batch]
-            bpix = np.repeat(np.arange(i, i+r.size), r)
-            blon, blat = healpix.randang(nside, bpix, lonlat=True, rng=rng)
-            lon[ncur:ncur+blon.size] = blon
-            lat[ncur:ncur+blat.size] = blat
-            ncur += bpix.size
-
-        assert ncur == ntot, 'internal error in sampling'
-
-    # return a plain scalar of counts if there are no dims
-    if not dims:
-        count = count.item()
+        # sample the map in batches
+        step = 1000
+        start, stop, size = 0, 0, 0
+        while count:
+            # tally this group of pixels
+            q = np.cumsum(n[stop:stop+step])
+            # does this group of pixels fill the batch?
+            if size + q[-1] < min(batch, count):
+                # no, we need the next group of pixels to fill the batch
+                stop += step
+                size += q[-1]
+            else:
+                # how many pixels from this group do we need?
+                stop += np.searchsorted(q, batch - size, side='right')
+                # if the first pixel alone is too much, use it anyway
+                if stop == start:
+                    stop += 1
+                # sample this batch of pixels
+                ipix = np.repeat(np.arange(start, stop), n[start:stop])
+                lon, lat = healpix.randang(nside, ipix, lonlat=True, rng=rng)
+                # next batch
+                start, size = stop, 0
+                # keep track of remaining number of points
+                count -= ipix.size
+                # yield the batch
+                yield lon, lat, ipix.size*cmask
 
-    return lon, lat, count
+        # make sure that the correct number of pixels was sampled
+        assert np.sum(n[stop:]) == 0
 
 
 def uniform_positions(ngal, *, rng=None):
     '''Generate positions uniformly over the sphere.
 
     The function supports array input for the ``ngal`` parameter.
 
     Parameters
     ----------
     ngal : float or array_like
         Number density, expected number of positions per arcmin2.
     rng : :class:`~numpy.random.Generator`, optional
         Random number generator.  If not given, a default RNG will be used.
 
-    Returns
-    -------
+    Yields
+    ------
     lon, lat : array_like or list of array_like
         Columns of longitudes and latitudes for the sampled points.
     count : int or list of ints
         The number of sampled points.  For array inputs, an array of
         counts with the same shape is returned.
 
     '''
 
     # get default RNG if not given
     if rng is None:
         rng = np.random.default_rng()
 
     # sample number of galaxies
-    count = rng.poisson(np.multiply(ARCMIN2_SPHERE, ngal))
+    ngal = rng.poisson(np.multiply(ARCMIN2_SPHERE, ngal))
 
     # extra dimensions of the output
-    dims = np.shape(count)
+    dims = np.shape(ngal)
 
     # make sure ntot is an array even if scalar
-    count = np.broadcast_to(count, dims)
-
-    # arrays for results
-    ntot = 0
-    lon = np.empty(0)
-    lat = np.empty(0)
+    ngal = np.broadcast_to(ngal, dims)
 
     # sample each set of points
     for k in np.ndindex(dims):
 
-        # resize output arrays
-        ncur, ntot = ntot, ntot + count[k]
-        lon.resize(ntot, refcheck=False)
-        lat.resize(ntot, refcheck=False)
-
         # sample uniformly over the sphere
-        lon[ncur:ntot] = rng.uniform(-180, 180, size=count[k])
-        lat[ncur:ntot] = np.rad2deg(np.arcsin(rng.uniform(-1, 1, size=count[k])))
+        lon = rng.uniform(-180, 180, size=ngal[k])
+        lat = np.rad2deg(np.arcsin(rng.uniform(-1, 1, size=ngal[k])))
 
-    # return plain scalar if there are no dims
-    if not dims:
-        count = count.item()
+        # report count
+        if dims:
+            count = np.zeros(dims, dtype=int)
+            count[k] = ngal[k]
+        else:
+            count = int(ngal[k])
 
-    return lon, lat, count
+        yield lon, lat, count
```

### Comparing `glass-2023.5/glass/shapes.py` & `glass-2023.6/glass/shapes.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,16 +20,18 @@
 Utilities
 ---------
 
 .. autofunction:: triaxial_axis_ratio
 
 '''
 
+from __future__ import annotations
 
 import numpy as np
+from numpy.typing import ArrayLike, NDArray
 
 
 def triaxial_axis_ratio(zeta, xi, size=None, *, rng=None):
     r'''axis ratio of a randomly projected triaxial ellipsoid
 
     Given the two axis ratios `1 >= zeta >= xi` of a randomly oriented triaxial
     ellipsoid, computes the axis ratio `q` of the projection.
@@ -158,88 +160,113 @@
     e = np.exp(1j*rng.uniform(0, 2*np.pi, size=np.shape(q)))
     e *= (1-q)/(1+q)
 
     # return the ellipticity
     return e
 
 
-def ellipticity_gaussian(size, sigma, *, rng=None):
+def ellipticity_gaussian(count: int | ArrayLike, sigma: ArrayLike, *,
+                         rng: np.random.Generator | None = None
+                         ) -> NDArray:
     r'''Sample Gaussian galaxy ellipticities.
 
-    The ellipticities are sampled from a normal distribution with standard
-    deviation ``sigma`` for each component.  Samples where the ellipticity is
-    larger than unity are discarded.  Hence, do not use this function with too
-    large values of ``sigma``, or the sampling will become inefficient.
+    The ellipticities are sampled from a normal distribution with
+    standard deviation ``sigma`` for each component.  Samples where the
+    ellipticity is larger than unity are discarded.  Hence, do not use
+    this function with too large values of ``sigma``, or the sampling
+    will become inefficient.
 
     Parameters
     ----------
-    size : int
+    count : int or array_like
         Number of ellipticities to be sampled.
     sigma : array_like
         Standard deviation in each component.
     rng : :class:`~numpy.random.Generator`, optional
-        Random number generator.  If not given, a default RNG will be used.
+        Random number generator.  If not given, a default RNG is used.
 
     Returns
     -------
     eps : array_like
         Array of galaxy :term:`ellipticity`.
 
     '''
 
     # default RNG if not provided
     if rng is None:
         rng = np.random.default_rng()
 
-    # sample complex ellipticities
-    # reject those where abs(e) > 0
-    e = rng.standard_normal(2*size, np.float64).view(np.complex128)
-    e *= sigma
-    i = np.where(np.abs(e) > 1)[0]
-    while len(i) > 0:
-        rng.standard_normal(2*len(i), np.float64, e[i].view(np.float64))
-        e[i] *= sigma
-        i = i[np.abs(e[i]) > 1]
-
-    return e
+    # bring inputs into common shape
+    count, sigma = np.broadcast_arrays(count, sigma)
 
+    # allocate flattened output array
+    eps = np.empty(count.sum(), dtype=np.complex128)
 
-def ellipticity_intnorm(size, sigma, *, rng=None):
+    # sample complex ellipticities
+    # reject those where abs(e) > 0
+    i = 0
+    for k in np.ndindex(count.shape):
+        e = rng.standard_normal(2*count[k], np.float64).view(np.complex128)
+        e *= sigma[k]
+        r = np.where(np.abs(e) > 1)[0]
+        while len(r) > 0:
+            rng.standard_normal(2*len(r), np.float64, e[r].view(np.float64))
+            e[r] *= sigma[k]
+            r = r[np.abs(e[r]) > 1]
+        eps[i:i+count[k]] = e
+        i += count[k]
+
+    return eps
+
+
+def ellipticity_intnorm(count: int | ArrayLike, sigma: ArrayLike, *,
+                        rng: np.random.Generator | None = None
+                        ) -> NDArray:
     r'''Sample galaxy ellipticities with intrinsic normal distribution.
 
-    The ellipticities are sampled from an intrinsic normal distribution with
-    standard deviation ``sigma`` for each component.
+    The ellipticities are sampled from an intrinsic normal distribution
+    with standard deviation ``sigma`` for each component.
 
     Parameters
     ----------
-    size : int
+    count : int | array_like
         Number of ellipticities to sample.
     sigma : array_like
         Standard deviation of the ellipticity in each component.
     rng : :class:`~numpy.random.Generator`, optional
-        Random number generator.  If not given, a default RNG will be used.
+        Random number generator.  If not given, a default RNG is used.
 
     Returns
     -------
     eps : array_like
         Array of galaxy :term:`ellipticity`.
 
     '''
 
-    # make sure sigma is admissible
-    if not 0 <= sigma < 0.5**0.5:
-        raise ValueError('sigma must be between 0 and sqrt(0.5)')
-
     # default RNG if not provided
     if rng is None:
         rng = np.random.default_rng()
 
+    # bring inputs into common shape
+    count, sigma = np.broadcast_arrays(count, sigma)
+
+    # make sure sigma is admissible
+    if not np.all((0 <= sigma) & (sigma < 0.5**0.5)):
+        raise ValueError('sigma must be between 0 and sqrt(0.5)')
+
     # convert to sigma_eta using fit
     sigma_eta = sigma*((8 + 5*sigma**2)/(2 - 4*sigma**2))**0.5
 
+    # allocate flattened output array
+    eps = np.empty(count.sum(), dtype=np.complex128)
+
     # sample complex ellipticities
-    e = rng.standard_normal(2*size, np.float64).view(np.complex128)
-    e *= sigma_eta
-    r = np.hypot(e.real, e.imag)
-    e *= np.divide(np.tanh(r/2), r, where=(r > 0), out=r)
+    i = 0
+    for k in np.ndindex(count.shape):
+        e = rng.standard_normal(2*count[k], np.float64).view(np.complex128)
+        e *= sigma_eta[k]
+        r = np.hypot(e.real, e.imag)
+        e *= np.divide(np.tanh(r/2), r, where=(r > 0), out=r)
+        eps[i:i+count[k]] = e
+        i += count[k]
 
-    return e
+    return eps
```

### Comparing `glass-2023.5/glass/shells.py` & `glass-2023.6/glass/shells.py`

 * *Files identical despite different names*

### Comparing `glass-2023.5/glass/test/test_galaxies.py` & `glass-2023.6/glass/test/test_galaxies.py`

 * *Files identical despite different names*

### Comparing `glass-2023.5/glass/test/test_shells.py` & `glass-2023.6/glass/test/test_shells.py`

 * *Files identical despite different names*

### Comparing `glass-2023.5/glass/user.py` & `glass-2023.6/glass/user.py`

 * *Files identical despite different names*

