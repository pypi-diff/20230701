# Comparing `tmp/pyoptools-0.1.1.tar.gz` & `tmp/pyoptools-0.2.0-cp310-cp310-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyoptools-0.1.1.tar", last modified: Tue Aug  1 19:58:09 2017, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

