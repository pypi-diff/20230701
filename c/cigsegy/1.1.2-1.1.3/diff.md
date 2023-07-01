# Comparing `tmp/cigsegy-1.1.2.tar.gz` & `tmp/cigsegy-1.1.3-cp39-cp39-macosx_13_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cigsegy-1.1.2.tar", last modified: Sat May 27 10:07:05 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

