# Comparing `tmp/redashsync-0.0.1.tar.gz` & `tmp/redashsync-0.0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redashsync-0.0.1.tar", last modified: Sat Jul  1 03:15:56 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

