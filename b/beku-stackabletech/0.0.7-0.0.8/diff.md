# Comparing `tmp/beku_stackabletech-0.0.7-py3-none-any.whl.zip` & `tmp/beku_stackabletech-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 14723 bytes, number of entries: 18
+Zip file size: 14841 bytes, number of entries: 18
 -rw-rw-r--  2.0 unx       43 b- defN 23-Jun-23 15:42 beku/__init__.py
 -rw-rw-r--  2.0 unx       79 b- defN 23-Feb-19 16:46 beku/__main__.py
--rw-rw-r--  2.0 unx    15694 b- defN 23-Jun-26 05:49 beku/kuttl.py
+-rw-rw-r--  2.0 unx    15730 b- defN 23-Jul-01 11:22 beku/kuttl.py
 -rw-rw-r--  2.0 unx     2370 b- defN 23-Jun-26 05:49 beku/main.py
 -rw-rw-r--  2.0 unx     7397 b- defN 23-Jun-23 15:42 beku/testsuite.py
--rw-rw-r--  2.0 unx      105 b- defN 23-Jun-26 05:50 beku/version.py
+-rw-rw-r--  2.0 unx      105 b- defN 23-Jul-01 11:34 beku/version.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-26 05:49 beku/test/__init__.py
--rw-rw-r--  2.0 unx    10548 b- defN 23-Jun-26 05:49 beku/test/test_render_from_stream.py
+-rw-rw-r--  2.0 unx    10843 b- defN 23-Jul-01 11:22 beku/test/test_render_from_stream.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-23 15:02 test/__init__.py
 -rw-rw-r--  2.0 unx     9050 b- defN 23-Jun-25 12:18 test/test_reneder_from_stream.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-23 09:39 tests/__init__.py
 -rw-rw-r--  2.0 unx     1425 b- defN 23-Jun-24 06:37 tests/testsuite.py
--rw-rw-r--  2.0 unx     1069 b- defN 23-Jun-26 05:54 beku_stackabletech-0.0.7.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1410 b- defN 23-Jun-26 05:54 beku_stackabletech-0.0.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-26 05:54 beku_stackabletech-0.0.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       40 b- defN 23-Jun-26 05:54 beku_stackabletech-0.0.7.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        5 b- defN 23-Jun-26 05:54 beku_stackabletech-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1447 b- defN 23-Jun-26 05:54 beku_stackabletech-0.0.7.dist-info/RECORD
-18 files, 50774 bytes uncompressed, 12345 bytes compressed:  75.7%
+-rw-rw-r--  2.0 unx     1069 b- defN 23-Jul-01 11:35 beku_stackabletech-0.0.8.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1639 b- defN 23-Jul-01 11:35 beku_stackabletech-0.0.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-01 11:35 beku_stackabletech-0.0.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       40 b- defN 23-Jul-01 11:35 beku_stackabletech-0.0.8.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jul-01 11:35 beku_stackabletech-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1447 b- defN 23-Jul-01 11:35 beku_stackabletech-0.0.8.dist-info/RECORD
+18 files, 51334 bytes uncompressed, 12463 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/testsuite.py
 Comment: 
 
-Filename: beku_stackabletech-0.0.7.dist-info/LICENSE
+Filename: beku_stackabletech-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: beku_stackabletech-0.0.7.dist-info/METADATA
+Filename: beku_stackabletech-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: beku_stackabletech-0.0.7.dist-info/WHEEL
+Filename: beku_stackabletech-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: beku_stackabletech-0.0.7.dist-info/entry_points.txt
+Filename: beku_stackabletech-0.0.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: beku_stackabletech-0.0.7.dist-info/top_level.txt
+Filename: beku_stackabletech-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: beku_stackabletech-0.0.7.dist-info/RECORD
+Filename: beku_stackabletech-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## beku/kuttl.py

```diff
@@ -224,18 +224,18 @@
         patches are discarded."""
         if self.test and self.test != test_name:
             logging.debug(
                 f"Skipping patch for test {[self.test]} for test [{test_name}]")
 
         if self._may_patch(test_name):
             logging.debug(f"Patching test [{test_name}]")
-            result = {}
+            result = {d.name: d for d in dims}
             for _pd in self.patches:
-                for dim in _pd.patch_dimensions(test_name, dims):
-                    result[dim.name] = dim
+                result = {d.name: d for d in _pd.patch_dimensions(
+                    test_name, list(result.values()))}
             return list(result.values())
         return dims
 
     def _may_patch(self, test_name: str) -> bool:
         """A patch can be applied if test_name matches the test attribute or the test attribute is None."""
         return (self.test and self.test == test_name) or not self.test
```

## beku/version.py

```diff
@@ -1,3 +1,3 @@
 """Package version."""
-__version_info__ = (0, 0, '7')
+__version_info__ = (0, 0, '8')
 __version__ = ".".join(map(str, __version_info__))
```

## beku/test/test_render_from_stream.py

```diff
@@ -102,16 +102,17 @@
                         expr: first
                       - name: druid
                         expr: last
         """)
         ets = renderer_from_stream(fixture)
         expected = EffectiveTestSuite(name='two-patches-on-the-same-test',
                                       test_cases=[TestCase(name='smoke',
-                                                           values={'druid': '26.0.0-stackable0.0.0-dev'})])
-        self.assertEqual(expected, ets[0], "Last patch wins")
+                                                           values={'druid': '24.0.0-stackable0.0.0-dev'})])
+        self.assertEqual(
+            expected, ets[0], "Take first and then take last out of that.")
 
     def test_patch_the_same_test_twice(self):
         fixture = textwrap.dedent("""
             ---
             dimensions:
               - name: druid
                 values:
@@ -262,34 +263,41 @@
               - name: zookeeper
                 values:
                   - 3.7.0-stackable0.0.0-dev
                   - 3.8.0-stackable0.0.0-dev
               - name: openshift
                 values:
                   - "false"
+              - name: tls
+                values:
+                  - "false"
             tests:
               - name: smoke
                 dimensions:
                   - druid
                   - zookeeper
                   - openshift
+                  - tls
             suites:
               - name: openshift
                 patch:
                   - dimensions:
                       - expr: last
                   -  dimensions:
                       - name: openshift
                         expr: "true"
+                      - name: tls
+                        expr: "true"
             """)
         ets = renderer_from_stream(fixture)
         expected = EffectiveTestSuite(name='openshift',
                                       test_cases=[TestCase(name='smoke',
                                                            values={'druid': '26.0.0-stackable0.0.0-dev',
                                                                    'openshift': 'true',
-                                                                   'zookeeper': '3.8.0-stackable0.0.0-dev'})])
+                                                                   'zookeeper': '3.8.0-stackable0.0.0-dev',
+                                                                   'tls': 'true'})])
 
         self.assertEqual(expected, ets[0])
 
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `beku_stackabletech-0.0.7.dist-info/LICENSE` & `beku_stackabletech-0.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `beku_stackabletech-0.0.7.dist-info/METADATA` & `beku_stackabletech-0.0.8.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beku-stackabletech
-Version: 0.0.7
+Version: 0.0.8
 Summary: Test suite expander for Stackable Kuttl tests.
 Author-email: Razvan Mihai <razvan.mihai@stackable.tech>
 Project-URL: Homepage, https://github.com/stackabletech/beku.py
 Project-URL: Bug Tracker, https://github.com/stackabletech/beku.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,18 +15,27 @@
 Requires-Dist: PyYAML (>=6.0)
 Provides-Extra: lint
 Requires-Dist: ruff (==0.0.275) ; extra == 'lint'
 Requires-Dist: mypy (==1.4.0) ; extra == 'lint'
 
 # beku
 
-Version: 0.0.7
+Version: 0.0.8
 
 ## Installation
 
+We recommend to use [pipx](https://pypa.github.io/pipx/):
+
+    pipx install beku-stackabletech
+
+But you can also use `pip`:
+
+    # from PyPI
+    pip install beku-stackabletech
+    # from GitHub
     pip install git+https://github.com/stackabletech/beku.py.git@master
 
 ## Usage
 
     cd <stackable operator directory>
     rm -rf tests/_work && beku
     cd tests/_work && kubectl kuttl test
@@ -41,15 +50,15 @@
 
 ## Release a new version
 
 Update the version in:
 
 * `pyproject.toml`
 * `version.py`
-* `README.md`
+* `README.md` : version and pip install command.
 
 Update the CHANGELOG.
 Commit and tag.
 Build and publish:
 
     rm -rf dist/
     python -m build --wheel .
```

## Comparing `beku_stackabletech-0.0.7.dist-info/RECORD` & `beku_stackabletech-0.0.8.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 beku/__init__.py,sha256=RBRzPf0eiEH2-LZNfxi8sE3qJENRlXBP-MoOMPeQIYw,43
 beku/__main__.py,sha256=KuEWcDdMSufciWzKjZpAGvFtD7ns5XIKFNw38ZjJGt0,79
-beku/kuttl.py,sha256=3NCw3e7Ybzb0ty2rfhq7274P9pVbk-h0NGTKFPU6jyI,15694
+beku/kuttl.py,sha256=nW_vpSpbCJk9fyV2JUJTQgkzsfoLqSS_Tgv-2wYFfkU,15730
 beku/main.py,sha256=nyogJ4g1zh5dw62FINO96xXUx4KhCtHIsBwgMth7CSw,2370
 beku/testsuite.py,sha256=Z9y9Ok_T7aXZ2DV8LbBGG_OT9l1c6pgqubbyJPCEVsE,7397
-beku/version.py,sha256=fIHv9sBWjAR27R2uJr4ghOlcHGPNZRyCwy5jSdUbHrQ,105
+beku/version.py,sha256=AGnZAgxlnKEuHUSXw239n2biAbqLml8Cw7hyBwYG6do,105
 beku/test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-beku/test/test_render_from_stream.py,sha256=M9ErFJgOdZ7PaYl86wxzOx4j_k4Fnpn06YNCr4mWoa0,10548
+beku/test/test_render_from_stream.py,sha256=11NcLambl8-N635f6K8zpcfa7J7Z8K_MqCejFsMB3Rc,10843
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/test_reneder_from_stream.py,sha256=dqhwM4NCN0Zl39tpLhcUx7KhjFJYzlqjtyAcDTVCm30,9050
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/testsuite.py,sha256=NgyKlko4RS2XVll0Jk98v4YpMmToFLuBtjT-6LYgT4c,1425
-beku_stackabletech-0.0.7.dist-info/LICENSE,sha256=gdYbHSzlrbgvmcpSS2Z4wZdJrl3zRW0xZE8G5U07efY,1069
-beku_stackabletech-0.0.7.dist-info/METADATA,sha256=H5HOKiy1dXoEH1iITsbYANnMO5y8wUTpzo5zM5jp3vE,1410
-beku_stackabletech-0.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-beku_stackabletech-0.0.7.dist-info/entry_points.txt,sha256=MDsqPnsZs4vyidvTH6MjLm9xfko_87bRf86joXxhtKU,40
-beku_stackabletech-0.0.7.dist-info/top_level.txt,sha256=NUVgvsTBHALAVwdKLRiLQ1UBN82NHfyACf_e8cBTWzM,5
-beku_stackabletech-0.0.7.dist-info/RECORD,,
+beku_stackabletech-0.0.8.dist-info/LICENSE,sha256=gdYbHSzlrbgvmcpSS2Z4wZdJrl3zRW0xZE8G5U07efY,1069
+beku_stackabletech-0.0.8.dist-info/METADATA,sha256=nRS_x9vyOJTxUYLXEUlFvmOTYvkvMvxnKipOeTTE-n0,1639
+beku_stackabletech-0.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+beku_stackabletech-0.0.8.dist-info/entry_points.txt,sha256=MDsqPnsZs4vyidvTH6MjLm9xfko_87bRf86joXxhtKU,40
+beku_stackabletech-0.0.8.dist-info/top_level.txt,sha256=NUVgvsTBHALAVwdKLRiLQ1UBN82NHfyACf_e8cBTWzM,5
+beku_stackabletech-0.0.8.dist-info/RECORD,,
```

