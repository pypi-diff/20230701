# Comparing `tmp/pydiscordself-0.1.0000.tar.gz` & `tmp/pydiscordself-0.2-py3.11.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiscordself-0.1.tar", last modified: Mon Aug 29 19:49:30 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

