# Comparing `tmp/spyprot-0.7.8.tar.gz` & `tmp/spyprot-0.8.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyprot-0.7.8.tar", last modified: Sun Nov 21 10:48:37 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

