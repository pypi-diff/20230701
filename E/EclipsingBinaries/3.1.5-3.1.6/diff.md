# Comparing `tmp/EclipsingBinaries-3.1.5.tar.gz` & `tmp/EclipsingBinaries-3.1.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EclipsingBinaries-3.1.5.tar", last modified: Fri Jun 23 22:29:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

