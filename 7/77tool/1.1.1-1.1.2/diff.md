# Comparing `tmp/77tool-1.1.1.tar.gz` & `tmp/77tool-1.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "77tool-1.1.1.tar", last modified: Fri Jun 30 15:31:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

