# Comparing `tmp/no_vtf-3.0.1.tar.gz` & `tmp/no_vtf-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "no_vtf-3.0.1.tar", last modified: Sat Jun 24 10:20:05 2023, max compression
+gzip compressed data, was "no_vtf-3.1.0.tar", last modified: Sat Jul  1 19:19:31 2023, max compression
```

## Comparing `no_vtf-3.0.1.tar` & `no_vtf-3.1.0.tar`

### file list

```diff
@@ -1,118 +1,117 @@
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.137010 no_vtf-3.0.1/
--rw-r--r--   0 build     (1000) build     (1000)     1655 2023-06-24 10:09:58.000000 no_vtf-3.0.1/.build.yml
--rw-r--r--   0 build     (1000) build     (1000)      336 2023-06-24 10:09:58.000000 no_vtf-3.0.1/.gitignore
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.121010 no_vtf-3.0.1/.reuse/
--rw-r--r--   0 build     (1000) build     (1000)      189 2023-06-24 10:09:58.000000 no_vtf-3.0.1/.reuse/dep5
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.121010 no_vtf-3.0.1/LICENSES/
--rw-r--r--   0 build     (1000) build     (1000)    17023 2023-06-24 10:09:58.000000 no_vtf-3.0.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 build     (1000) build     (1000)     7048 2023-06-24 10:09:58.000000 no_vtf-3.0.1/LICENSES/CC0-1.0.txt
--rw-r--r--   0 build     (1000) build     (1000)    34670 2023-06-24 10:09:58.000000 no_vtf-3.0.1/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0 build     (1000) build     (1000)    42098 2023-06-24 10:09:58.000000 no_vtf-3.0.1/LICENSES/LGPL-3.0-or-later.txt
--rw-r--r--   0 build     (1000) build     (1000)      138 2023-06-24 10:09:58.000000 no_vtf-3.0.1/MANIFEST.in
--rw-r--r--   0 build     (1000) build     (1000)     9540 2023-06-24 10:20:05.137010 no_vtf-3.0.1/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1000)     8269 2023-06-24 10:09:58.000000 no_vtf-3.0.1/README.md
--rw-r--r--   0 build     (1000) build     (1000)       95 2023-06-24 10:09:58.000000 no_vtf-3.0.1/README.md.license
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.125010 no_vtf-3.0.1/builds/
--rw-r--r--   0 build     (1000) build     (1000)      559 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/common
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.125010 no_vtf-3.0.1/builds/debian/
--rw-r--r--   0 build     (1000) build     (1000)      162 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/debian/common
--rwxr-xr-x   0 build     (1000) build     (1000)      401 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/debian/env.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      404 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/debian/ksc-install.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      510 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/debian/python3.10-build_dep.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      855 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/debian/wine-install.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      180 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/diff_generated.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      188 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/nox.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      198 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/nox_wine.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      641 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/publish_frozen.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      466 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/python3.10-install.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      363 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/verify_signatures.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      264 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/with_clone.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      989 2023-06-24 10:09:58.000000 no_vtf-3.0.1/builds/with_wine.sh
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.125010 no_vtf-3.0.1/ksy/
--rwxr-xr-x   0 build     (1000) build     (1000)      205 2023-06-24 10:09:58.000000 no_vtf-3.0.1/ksy/compile.sh
--rw-r--r--   0 build     (1000) build     (1000)    10409 2023-06-24 10:09:58.000000 no_vtf-3.0.1/ksy/vtf.ksy
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.125010 no_vtf-3.0.1/no_vtf/
--rw-r--r--   0 build     (1000) build     (1000)      329 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      300 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/__main__.py
--rw-r--r--   0 build     (1000) build     (1000)      160 2023-06-24 10:20:04.000000 no_vtf-3.0.1/no_vtf/_version.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.129010 no_vtf-3.0.1/no_vtf/deferred/
--rw-r--r--   0 build     (1000) build     (1000)      186 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/deferred/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     1471 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/deferred/deferred.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.129010 no_vtf-3.0.1/no_vtf/filesystem/
--rw-r--r--   0 build     (1000) build     (1000)      287 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/filesystem/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     2023 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/filesystem/input_paths.py
--rw-r--r--   0 build     (1000) build     (1000)      895 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/filesystem/output_directories.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.129010 no_vtf-3.0.1/no_vtf/image/
--rw-r--r--   0 build     (1000) build     (1000)      441 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     1667 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/channel_separator.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.129010 no_vtf-3.0.1/no_vtf/image/decoder/
--rw-r--r--   0 build     (1000) build     (1000)      198 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/decoder/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      486 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/decoder/decoder.py
--rw-r--r--   0 build     (1000) build     (1000)     7697 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/decoder/generic.py
--rw-r--r--   0 build     (1000) build     (1000)     2797 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/decoder/vtf.py
--rw-r--r--   0 build     (1000) build     (1000)     1497 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/image.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.133010 no_vtf-3.0.1/no_vtf/image/modifier/
--rw-r--r--   0 build     (1000) build     (1000)      202 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/modifier/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     1632 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/modifier/fp_precision_modifier.py
--rw-r--r--   0 build     (1000) build     (1000)      540 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/modifier/modifier.py
--rw-r--r--   0 build     (1000) build     (1000)      946 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/image/ndarray.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.133010 no_vtf-3.0.1/no_vtf/io/
--rw-r--r--   0 build     (1000) build     (1000)      264 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/io/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      573 2023-06-24 10:09:59.000000 no_vtf-3.0.1/no_vtf/io/bytes.py
--rw-r--r--   0 build     (1000) build     (1000)     7976 2023-06-24 10:09:59.000000 no_vtf-3.0.1/no_vtf/io/image.py
--rw-r--r--   0 build     (1000) build     (1000)      933 2023-06-24 10:09:59.000000 no_vtf-3.0.1/no_vtf/io/io.py
--rw-r--r--   0 build     (1000) build     (1000)    11148 2023-06-24 10:09:59.000000 no_vtf-3.0.1/no_vtf/main.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.133010 no_vtf-3.0.1/no_vtf/parser/
--rw-r--r--   0 build     (1000) build     (1000)        0 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/parser/__init__.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.133010 no_vtf-3.0.1/no_vtf/parser/generated/
--rw-r--r--   0 build     (1000) build     (1000)        0 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/parser/generated/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)    25192 2023-06-24 10:19:46.000000 no_vtf-3.0.1/no_vtf/parser/generated/vtf.py
--rw-r--r--   0 build     (1000) build     (1000)       93 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/parser/generated/vtf.py.license
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.133010 no_vtf-3.0.1/no_vtf/pipeline/
--rw-r--r--   0 build     (1000) build     (1000)      186 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/pipeline/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     4935 2023-06-24 10:09:59.000000 no_vtf-3.0.1/no_vtf/pipeline/pipeline.py
--rw-r--r--   0 build     (1000) build     (1000)        0 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/py.typed
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.133010 no_vtf-3.0.1/no_vtf/task_runner/
--rw-r--r--   0 build     (1000) build     (1000)      356 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/task_runner/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     1524 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/task_runner/parallel.py
--rw-r--r--   0 build     (1000) build     (1000)      826 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/task_runner/sequential.py
--rw-r--r--   0 build     (1000) build     (1000)     1085 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/task_runner/task_runner.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.133010 no_vtf-3.0.1/no_vtf/texture/
--rw-r--r--   0 build     (1000) build     (1000)        0 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/texture/__init__.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.133010 no_vtf-3.0.1/no_vtf/texture/decoder/
--rw-r--r--   0 build     (1000) build     (1000)      204 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/texture/decoder/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      486 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/texture/decoder/decoder.py
--rw-r--r--   0 build     (1000) build     (1000)     4485 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/texture/decoder/vtf.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.137010 no_vtf-3.0.1/no_vtf/texture/extractor/
--rw-r--r--   0 build     (1000) build     (1000)      212 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/texture/extractor/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      453 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/texture/extractor/extractor.py
--rw-r--r--   0 build     (1000) build     (1000)     4010 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/texture/extractor/vtf.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.137010 no_vtf-3.0.1/no_vtf/texture/filter/
--rw-r--r--   0 build     (1000) build     (1000)      200 2023-06-24 10:09:59.000000 no_vtf-3.0.1/no_vtf/texture/filter/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      367 2023-06-24 10:09:59.000000 no_vtf-3.0.1/no_vtf/texture/filter/filter.py
--rw-r--r--   0 build     (1000) build     (1000)     2756 2023-06-24 10:09:59.000000 no_vtf-3.0.1/no_vtf/texture/filter/vtf.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.137010 no_vtf-3.0.1/no_vtf/texture/namer/
--rw-r--r--   0 build     (1000) build     (1000)      196 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/texture/namer/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      374 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/texture/namer/namer.py
--rw-r--r--   0 build     (1000) build     (1000)     1025 2023-06-24 10:09:59.000000 no_vtf-3.0.1/no_vtf/texture/namer/vtf.py
--rw-r--r--   0 build     (1000) build     (1000)      663 2023-06-24 10:09:58.000000 no_vtf-3.0.1/no_vtf/texture/vtf.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.129010 no_vtf-3.0.1/no_vtf.egg-info/
--rw-r--r--   0 build     (1000) build     (1000)     9540 2023-06-24 10:20:04.000000 no_vtf-3.0.1/no_vtf.egg-info/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1000)     2434 2023-06-24 10:20:05.000000 no_vtf-3.0.1/no_vtf.egg-info/SOURCES.txt
--rw-r--r--   0 build     (1000) build     (1000)        1 2023-06-24 10:20:04.000000 no_vtf-3.0.1/no_vtf.egg-info/dependency_links.txt
--rw-r--r--   0 build     (1000) build     (1000)       49 2023-06-24 10:20:04.000000 no_vtf-3.0.1/no_vtf.egg-info/entry_points.txt
--rw-r--r--   0 build     (1000) build     (1000)        1 2023-06-24 10:19:06.000000 no_vtf-3.0.1/no_vtf.egg-info/not-zip-safe
--rw-r--r--   0 build     (1000) build     (1000)      183 2023-06-24 10:20:04.000000 no_vtf-3.0.1/no_vtf.egg-info/requires.txt
--rw-r--r--   0 build     (1000) build     (1000)        7 2023-06-24 10:20:04.000000 no_vtf-3.0.1/no_vtf.egg-info/top_level.txt
--rw-r--r--   0 build     (1000) build     (1000)     9785 2023-06-24 10:09:58.000000 no_vtf-3.0.1/noxfile.py
--rw-r--r--   0 build     (1000) build     (1000)      682 2023-06-24 10:09:58.000000 no_vtf-3.0.1/pyproject.toml
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.121010 no_vtf-3.0.1/resources/
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.137010 no_vtf-3.0.1/resources/docs/
--rw-r--r--   0 build     (1000) build     (1000)   123671 2023-06-24 10:09:58.000000 no_vtf-3.0.1/resources/docs/screencast.gif
--rw-r--r--   0 build     (1000) build     (1000)       95 2023-06-24 10:09:58.000000 no_vtf-3.0.1/resources/docs/screencast.gif.license
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-24 10:20:05.137010 no_vtf-3.0.1/resources/pyinstaller/
--rw-r--r--   0 build     (1000) build     (1000)        6 2023-06-24 10:09:58.000000 no_vtf-3.0.1/resources/pyinstaller/empty.ico
--rw-r--r--   0 build     (1000) build     (1000)       93 2023-06-24 10:09:58.000000 no_vtf-3.0.1/resources/pyinstaller/empty.ico.license
--rwxr-xr-x   0 build     (1000) build     (1000)      276 2023-06-24 10:09:58.000000 no_vtf-3.0.1/resources/pyinstaller/no_vtf.desktop
--rw-r--r--   0 build     (1000) build     (1000)      103 2023-06-24 10:09:58.000000 no_vtf-3.0.1/resources/pyinstaller/no_vtf.desktop.license
--rw-r--r--   0 build     (1000) build     (1000)     2640 2023-06-24 10:20:05.141010 no_vtf-3.0.1/setup.cfg
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.722456 no_vtf-3.1.0/
+-rw-r--r--   0 build     (1000) build     (1000)     1754 2023-07-01 19:09:49.000000 no_vtf-3.1.0/.build.yml
+-rw-r--r--   0 build     (1000) build     (1000)      336 2023-07-01 19:09:49.000000 no_vtf-3.1.0/.gitignore
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.706455 no_vtf-3.1.0/.reuse/
+-rw-r--r--   0 build     (1000) build     (1000)      189 2023-07-01 19:09:49.000000 no_vtf-3.1.0/.reuse/dep5
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.706455 no_vtf-3.1.0/LICENSES/
+-rw-r--r--   0 build     (1000) build     (1000)    17023 2023-07-01 19:09:49.000000 no_vtf-3.1.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 build     (1000) build     (1000)     7048 2023-07-01 19:09:49.000000 no_vtf-3.1.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 build     (1000) build     (1000)    34670 2023-07-01 19:09:49.000000 no_vtf-3.1.0/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 build     (1000) build     (1000)    42098 2023-07-01 19:09:49.000000 no_vtf-3.1.0/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 build     (1000) build     (1000)      138 2023-07-01 19:09:49.000000 no_vtf-3.1.0/MANIFEST.in
+-rw-r--r--   0 build     (1000) build     (1000)     9371 2023-07-01 19:19:31.722456 no_vtf-3.1.0/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1000)     8100 2023-07-01 19:09:49.000000 no_vtf-3.1.0/README.md
+-rw-r--r--   0 build     (1000) build     (1000)       95 2023-07-01 19:09:49.000000 no_vtf-3.1.0/README.md.license
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.706455 no_vtf-3.1.0/builds/
+-rw-r--r--   0 build     (1000) build     (1000)      559 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/common
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.710456 no_vtf-3.1.0/builds/debian/
+-rw-r--r--   0 build     (1000) build     (1000)      162 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/debian/common
+-rwxr-xr-x   0 build     (1000) build     (1000)      409 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/debian/env.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      412 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/debian/ksc-install.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      518 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/debian/python3.10-build_dep.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      863 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/debian/wine-install.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      188 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/diff_generated.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      196 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/nox.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      206 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/nox_wine.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      649 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/publish_frozen.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      474 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/python3.10-install.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      371 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/verify_signatures.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      272 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/with_clone.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      997 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/with_wine.sh
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.710456 no_vtf-3.1.0/ksy/
+-rwxr-xr-x   0 build     (1000) build     (1000)      205 2023-07-01 19:09:49.000000 no_vtf-3.1.0/ksy/compile.sh
+-rw-r--r--   0 build     (1000) build     (1000)    10409 2023-07-01 19:09:49.000000 no_vtf-3.1.0/ksy/vtf.ksy
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.710456 no_vtf-3.1.0/no_vtf/
+-rw-r--r--   0 build     (1000) build     (1000)      329 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      300 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/__main__.py
+-rw-r--r--   0 build     (1000) build     (1000)      160 2023-07-01 19:19:31.000000 no_vtf-3.1.0/no_vtf/_version.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.710456 no_vtf-3.1.0/no_vtf/deferred/
+-rw-r--r--   0 build     (1000) build     (1000)      186 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/deferred/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     1471 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/deferred/deferred.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.714456 no_vtf-3.1.0/no_vtf/filesystem/
+-rw-r--r--   0 build     (1000) build     (1000)      287 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/filesystem/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     2023 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/filesystem/input_paths.py
+-rw-r--r--   0 build     (1000) build     (1000)      895 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/filesystem/output_directories.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.714456 no_vtf-3.1.0/no_vtf/image/
+-rw-r--r--   0 build     (1000) build     (1000)      441 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     1667 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/channel_separator.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.714456 no_vtf-3.1.0/no_vtf/image/decoder/
+-rw-r--r--   0 build     (1000) build     (1000)      198 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/decoder/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      486 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/decoder/decoder.py
+-rw-r--r--   0 build     (1000) build     (1000)     7697 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/decoder/generic.py
+-rw-r--r--   0 build     (1000) build     (1000)     2797 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/decoder/vtf.py
+-rw-r--r--   0 build     (1000) build     (1000)     1497 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/image.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.714456 no_vtf-3.1.0/no_vtf/image/modifier/
+-rw-r--r--   0 build     (1000) build     (1000)      202 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/modifier/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     1632 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/modifier/fp_precision_modifier.py
+-rw-r--r--   0 build     (1000) build     (1000)      540 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/modifier/modifier.py
+-rw-r--r--   0 build     (1000) build     (1000)      946 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/ndarray.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.714456 no_vtf-3.1.0/no_vtf/io/
+-rw-r--r--   0 build     (1000) build     (1000)      264 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/io/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      866 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/io/bytes.py
+-rw-r--r--   0 build     (1000) build     (1000)     9249 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/io/image.py
+-rw-r--r--   0 build     (1000) build     (1000)     1246 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/io/io.py
+-rw-r--r--   0 build     (1000) build     (1000)    22474 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/main.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.714456 no_vtf-3.1.0/no_vtf/parser/
+-rw-r--r--   0 build     (1000) build     (1000)        0 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/parser/__init__.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.714456 no_vtf-3.1.0/no_vtf/parser/generated/
+-rw-r--r--   0 build     (1000) build     (1000)        0 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/parser/generated/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)    25192 2023-07-01 19:19:13.000000 no_vtf-3.1.0/no_vtf/parser/generated/vtf.py
+-rw-r--r--   0 build     (1000) build     (1000)       93 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/parser/generated/vtf.py.license
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.718456 no_vtf-3.1.0/no_vtf/pipeline/
+-rw-r--r--   0 build     (1000) build     (1000)      186 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/pipeline/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     7894 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/pipeline/pipeline.py
+-rw-r--r--   0 build     (1000) build     (1000)        0 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/py.typed
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.718456 no_vtf-3.1.0/no_vtf/task_runner/
+-rw-r--r--   0 build     (1000) build     (1000)      356 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/task_runner/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     1524 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/task_runner/parallel.py
+-rw-r--r--   0 build     (1000) build     (1000)      826 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/task_runner/sequential.py
+-rw-r--r--   0 build     (1000) build     (1000)     1085 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/task_runner/task_runner.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.718456 no_vtf-3.1.0/no_vtf/texture/
+-rw-r--r--   0 build     (1000) build     (1000)        0 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/__init__.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.718456 no_vtf-3.1.0/no_vtf/texture/decoder/
+-rw-r--r--   0 build     (1000) build     (1000)      204 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/decoder/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      486 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/decoder/decoder.py
+-rw-r--r--   0 build     (1000) build     (1000)     4485 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/decoder/vtf.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.718456 no_vtf-3.1.0/no_vtf/texture/extractor/
+-rw-r--r--   0 build     (1000) build     (1000)      212 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/extractor/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      453 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/extractor/extractor.py
+-rw-r--r--   0 build     (1000) build     (1000)     4010 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/extractor/vtf.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.718456 no_vtf-3.1.0/no_vtf/texture/filter/
+-rw-r--r--   0 build     (1000) build     (1000)      252 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/filter/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      702 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/filter/filter.py
+-rw-r--r--   0 build     (1000) build     (1000)     4774 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/filter/vtf.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.718456 no_vtf-3.1.0/no_vtf/texture/namer/
+-rw-r--r--   0 build     (1000) build     (1000)      196 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/namer/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      374 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/namer/namer.py
+-rw-r--r--   0 build     (1000) build     (1000)     1079 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/namer/vtf.py
+-rw-r--r--   0 build     (1000) build     (1000)      663 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/vtf.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.710456 no_vtf-3.1.0/no_vtf.egg-info/
+-rw-r--r--   0 build     (1000) build     (1000)     9371 2023-07-01 19:19:31.000000 no_vtf-3.1.0/no_vtf.egg-info/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1000)     2389 2023-07-01 19:19:31.000000 no_vtf-3.1.0/no_vtf.egg-info/SOURCES.txt
+-rw-r--r--   0 build     (1000) build     (1000)        1 2023-07-01 19:19:31.000000 no_vtf-3.1.0/no_vtf.egg-info/dependency_links.txt
+-rw-r--r--   0 build     (1000) build     (1000)       49 2023-07-01 19:19:31.000000 no_vtf-3.1.0/no_vtf.egg-info/entry_points.txt
+-rw-r--r--   0 build     (1000) build     (1000)        1 2023-07-01 19:18:33.000000 no_vtf-3.1.0/no_vtf.egg-info/not-zip-safe
+-rw-r--r--   0 build     (1000) build     (1000)      183 2023-07-01 19:19:31.000000 no_vtf-3.1.0/no_vtf.egg-info/requires.txt
+-rw-r--r--   0 build     (1000) build     (1000)        7 2023-07-01 19:19:31.000000 no_vtf-3.1.0/no_vtf.egg-info/top_level.txt
+-rw-r--r--   0 build     (1000) build     (1000)     9847 2023-07-01 19:09:49.000000 no_vtf-3.1.0/noxfile.py
+-rw-r--r--   0 build     (1000) build     (1000)      682 2023-07-01 19:09:49.000000 no_vtf-3.1.0/pyproject.toml
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.702455 no_vtf-3.1.0/resources/
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.722456 no_vtf-3.1.0/resources/docs/
+-rw-r--r--   0 build     (1000) build     (1000)   123671 2023-07-01 19:09:49.000000 no_vtf-3.1.0/resources/docs/screencast.gif
+-rw-r--r--   0 build     (1000) build     (1000)       95 2023-07-01 19:09:49.000000 no_vtf-3.1.0/resources/docs/screencast.gif.license
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.722456 no_vtf-3.1.0/resources/pyinstaller/
+-rw-r--r--   0 build     (1000) build     (1000)        6 2023-07-01 19:09:49.000000 no_vtf-3.1.0/resources/pyinstaller/empty.ico
+-rw-r--r--   0 build     (1000) build     (1000)       93 2023-07-01 19:09:49.000000 no_vtf-3.1.0/resources/pyinstaller/empty.ico.license
+-rwxr-xr-x   0 build     (1000) build     (1000)      385 2023-07-01 19:09:49.000000 no_vtf-3.1.0/resources/pyinstaller/no_vtf.desktop
+-rw-r--r--   0 build     (1000) build     (1000)     2640 2023-07-01 19:19:31.722456 no_vtf-3.1.0/setup.cfg
```

### Comparing `no_vtf-3.0.1/.build.yml` & `no_vtf-3.1.0/.build.yml`

 * *Files 8% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
   - verify_signatures: |
       cd no_vtf
       builds/verify_signatures.sh || complete-build
 
   - pre-release: |
       cd no_vtf
+      [ "$(git rev-parse --verify HEAD)" == "$(git rev-parse --verify master)" ] || complete-build
       git describe --exact-match 2>/dev/null || complete-build
 
   - publish_frozen: |
       cd no_vtf
       builds/publish_frozen.sh ~ no_vtf-linux_x64.tar.xz no_vtf-windows_x64.zip
 
   - publish_package: |
```

### Comparing `no_vtf-3.0.1/LICENSES/CC-BY-4.0.txt` & `no_vtf-3.1.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/LICENSES/CC0-1.0.txt` & `no_vtf-3.1.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/LICENSES/GPL-3.0-or-later.txt` & `no_vtf-3.1.0/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/LICENSES/LGPL-3.0-or-later.txt` & `no_vtf-3.1.0/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/PKG-INFO` & `no_vtf-3.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: no_vtf
-Version: 3.0.1
+Version: 3.1.0
 Summary: Valve Texture Format Converter
 Home-page: https://sr.ht/~b5327157/no_vtf
 Author: b5327157
 Author-email: b5327157@protonmail.com
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Download, https://sr.ht/~b5327157/no_vtf/#application-bundle
 Project-URL: Changelog, https://git.sr.ht/~b5327157/no_vtf/refs
@@ -25,15 +25,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSES/GPL-3.0-or-later.txt
 
 # no_vtf
 
-Say no to [.vtf](https://developer.valvesoftware.com/wiki/Valve_Texture_Format) – convert it to one of the standard image formats.
+Say no to [Source Engine](https://developer.valvesoftware.com/wiki/Source)'s [.vtf](https://developer.valvesoftware.com/wiki/Valve_Texture_Format) – convert it to one of the standard image formats.
 
 ![Badge showing supported Python versions](https://img.shields.io/pypi/pyversions/no_vtf?style=flat-square)
 [![Badge showing package version on PyPI](https://img.shields.io/pypi/v/no_vtf?style=flat-square)](https://pypi.org/project/no-vtf/)
 [![Badge showing number of monthly downloads from PyPI](https://img.shields.io/pypi/dm/no_vtf?style=flat-square)](https://pypistats.org/packages/no-vtf)
 [![Badge showing source code repository hosted on SourceHut](https://img.shields.io/badge/sr.ht-repository-white?labelColor=212529&logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjxzdmcKICAgdmlld0JveD0iMCAwIDUxMiA1MTIiCiAgIHZlcnNpb249IjEuMSIKICAgaWQ9InN2ZzUxIgogICBzb2RpcG9kaTpkb2NuYW1lPSJzb3VyY2VodXQtd2hpdGUuc3ZnIgogICBpbmtzY2FwZTp2ZXJzaW9uPSIxLjEgKGM2OGUyMmMzODcsIDIwMjEtMDUtMjMpIgogICB4bWxuczppbmtzY2FwZT0iaHR0cDovL3d3dy5pbmtzY2FwZS5vcmcvbmFtZXNwYWNlcy9pbmtzY2FwZSIKICAgeG1sbnM6c29kaXBvZGk9Imh0dHA6Ly9zb2RpcG9kaS5zb3VyY2Vmb3JnZS5uZXQvRFREL3NvZGlwb2RpLTAuZHRkIgogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciCiAgIHhtbG5zOnN2Zz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgogIDxkZWZzCiAgICAgaWQ9ImRlZnM1NSIgLz4KICA8c29kaXBvZGk6bmFtZWR2aWV3CiAgICAgaWQ9Im5hbWVkdmlldzUzIgogICAgIHBhZ2Vjb2xvcj0iIzUwNTA1MCIKICAgICBib3JkZXJjb2xvcj0iI2ZmZmZmZiIKICAgICBib3JkZXJvcGFjaXR5PSIxIgogICAgIGlua3NjYXBlOnBhZ2VzaGFkb3c9IjAiCiAgICAgaW5rc2NhcGU6cGFnZW9wYWNpdHk9IjAiCiAgICAgaW5rc2NhcGU6cGFnZWNoZWNrZXJib2FyZD0iMSIKICAgICBzaG93Z3JpZD0iZmFsc2UiCiAgICAgaW5rc2NhcGU6em9vbT0iMS42NTQyOTY5IgogICAgIGlua3NjYXBlOmN4PSIyNTYiCiAgICAgaW5rc2NhcGU6Y3k9IjI1NiIKICAgICBpbmtzY2FwZTp3aW5kb3ctd2lkdGg9IjE5MjAiCiAgICAgaW5rc2NhcGU6d2luZG93LWhlaWdodD0iMTA1OSIKICAgICBpbmtzY2FwZTp3aW5kb3cteD0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3cteT0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3ctbWF4aW1pemVkPSIxIgogICAgIGlua3NjYXBlOmN1cnJlbnQtbGF5ZXI9InN2ZzUxIiAvPgogIDxwYXRoCiAgICAgZD0iTTI1NiA4QzExOSA4IDggMTE5IDggMjU2czExMSAyNDggMjQ4IDI0OCAyNDgtMTExIDI0OC0yNDhTMzkzIDggMjU2IDh6bTAgNDQ4Yy0xMTAuNSAwLTIwMC04OS41LTIwMC0yMDBTMTQ1LjUgNTYgMjU2IDU2czIwMCA4OS41IDIwMCAyMDAtODkuNSAyMDAtMjAwIDIwMHoiCiAgICAgaWQ9InBhdGg0OSIKICAgICBzdHlsZT0iZmlsbDojZmZmZmZmIiAvPgo8L3N2Zz4K)](https://sr.ht/~b5327157/no_vtf)
 [![Badge showing builds.sr.ht status](https://builds.sr.ht/~b5327157/no_vtf.svg?search=tags:master)](https://builds.sr.ht/~b5327157/no_vtf?search=tags:master)
 [![Badge showing REUSE compliance status](https://api.reuse.software/badge/git.sr.ht/~b5327157/no_vtf)](https://api.reuse.software/info/git.sr.ht/~b5327157/no_vtf)
@@ -110,14 +110,20 @@
 
 #### Override LDR/HDR output format
 
 ```
 no_vtf --ldr-format png --hdr-format tiff PATH...
 ```
 
+#### Convert animated texture
+
+```
+no_vtf --animate --fps 20 PATH...
+```
+
 #### Further help
 
 ```
 no_vtf --help
 ```
 
 ## Supported formats
@@ -148,15 +154,15 @@
 
 ### Output
 
 The following formats were tested and optimized for use:
 
 #### LDR
 
-- PNG
+- PNG, APNG
 - TGA
 - TIFF (default)
 
 #### HDR
 
 - EXR (default)
 - TIFF
@@ -167,18 +173,14 @@
 
 ### Color space
 
 Color space of LDR textures is inferred from the context in which the texture is used in-game. Since this context is not available when converting the .vtf files directly, color space metadata for the output images cannot be set.
 
 Color space of HDR textures is always linear. It would make sense to set this metadata when converting into the TIFF format, but for technical reasons, this is not done.
 
-### Opaque PNG
-
-When using PNG, the alpha channel is not written when the image is fully opaque. This may pose problems in other programs. In Blender, for example, when such image is not packed and OSL is enabled, the alpha channel is shown as black. For this reason, TIFF is the default LDR format instead of PNG.
-
 ## Benchmark
 
 - Sample: 11 GiB of LDR .vtf files
 - CPU: Intel Core i7-6500U
 
 Size is the total disk usage consumed by the output.
 Conversion was done without extraction of all mipmaps.
```

### Comparing `no_vtf-3.0.1/README.md` & `no_vtf-3.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # no_vtf
 
-Say no to [.vtf](https://developer.valvesoftware.com/wiki/Valve_Texture_Format) – convert it to one of the standard image formats.
+Say no to [Source Engine](https://developer.valvesoftware.com/wiki/Source)'s [.vtf](https://developer.valvesoftware.com/wiki/Valve_Texture_Format) – convert it to one of the standard image formats.
 
 ![Badge showing supported Python versions](https://img.shields.io/pypi/pyversions/no_vtf?style=flat-square)
 [![Badge showing package version on PyPI](https://img.shields.io/pypi/v/no_vtf?style=flat-square)](https://pypi.org/project/no-vtf/)
 [![Badge showing number of monthly downloads from PyPI](https://img.shields.io/pypi/dm/no_vtf?style=flat-square)](https://pypistats.org/packages/no-vtf)
 [![Badge showing source code repository hosted on SourceHut](https://img.shields.io/badge/sr.ht-repository-white?labelColor=212529&logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjxzdmcKICAgdmlld0JveD0iMCAwIDUxMiA1MTIiCiAgIHZlcnNpb249IjEuMSIKICAgaWQ9InN2ZzUxIgogICBzb2RpcG9kaTpkb2NuYW1lPSJzb3VyY2VodXQtd2hpdGUuc3ZnIgogICBpbmtzY2FwZTp2ZXJzaW9uPSIxLjEgKGM2OGUyMmMzODcsIDIwMjEtMDUtMjMpIgogICB4bWxuczppbmtzY2FwZT0iaHR0cDovL3d3dy5pbmtzY2FwZS5vcmcvbmFtZXNwYWNlcy9pbmtzY2FwZSIKICAgeG1sbnM6c29kaXBvZGk9Imh0dHA6Ly9zb2RpcG9kaS5zb3VyY2Vmb3JnZS5uZXQvRFREL3NvZGlwb2RpLTAuZHRkIgogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciCiAgIHhtbG5zOnN2Zz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgogIDxkZWZzCiAgICAgaWQ9ImRlZnM1NSIgLz4KICA8c29kaXBvZGk6bmFtZWR2aWV3CiAgICAgaWQ9Im5hbWVkdmlldzUzIgogICAgIHBhZ2Vjb2xvcj0iIzUwNTA1MCIKICAgICBib3JkZXJjb2xvcj0iI2ZmZmZmZiIKICAgICBib3JkZXJvcGFjaXR5PSIxIgogICAgIGlua3NjYXBlOnBhZ2VzaGFkb3c9IjAiCiAgICAgaW5rc2NhcGU6cGFnZW9wYWNpdHk9IjAiCiAgICAgaW5rc2NhcGU6cGFnZWNoZWNrZXJib2FyZD0iMSIKICAgICBzaG93Z3JpZD0iZmFsc2UiCiAgICAgaW5rc2NhcGU6em9vbT0iMS42NTQyOTY5IgogICAgIGlua3NjYXBlOmN4PSIyNTYiCiAgICAgaW5rc2NhcGU6Y3k9IjI1NiIKICAgICBpbmtzY2FwZTp3aW5kb3ctd2lkdGg9IjE5MjAiCiAgICAgaW5rc2NhcGU6d2luZG93LWhlaWdodD0iMTA1OSIKICAgICBpbmtzY2FwZTp3aW5kb3cteD0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3cteT0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3ctbWF4aW1pemVkPSIxIgogICAgIGlua3NjYXBlOmN1cnJlbnQtbGF5ZXI9InN2ZzUxIiAvPgogIDxwYXRoCiAgICAgZD0iTTI1NiA4QzExOSA4IDggMTE5IDggMjU2czExMSAyNDggMjQ4IDI0OCAyNDgtMTExIDI0OC0yNDhTMzkzIDggMjU2IDh6bTAgNDQ4Yy0xMTAuNSAwLTIwMC04OS41LTIwMC0yMDBTMTQ1LjUgNTYgMjU2IDU2czIwMCA4OS41IDIwMCAyMDAtODkuNSAyMDAtMjAwIDIwMHoiCiAgICAgaWQ9InBhdGg0OSIKICAgICBzdHlsZT0iZmlsbDojZmZmZmZmIiAvPgo8L3N2Zz4K)](https://sr.ht/~b5327157/no_vtf)
 [![Badge showing builds.sr.ht status](https://builds.sr.ht/~b5327157/no_vtf.svg?search=tags:master)](https://builds.sr.ht/~b5327157/no_vtf?search=tags:master)
 [![Badge showing REUSE compliance status](https://api.reuse.software/badge/git.sr.ht/~b5327157/no_vtf)](https://api.reuse.software/info/git.sr.ht/~b5327157/no_vtf)
@@ -81,14 +81,20 @@
 
 #### Override LDR/HDR output format
 
 ```
 no_vtf --ldr-format png --hdr-format tiff PATH...
 ```
 
+#### Convert animated texture
+
+```
+no_vtf --animate --fps 20 PATH...
+```
+
 #### Further help
 
 ```
 no_vtf --help
 ```
 
 ## Supported formats
@@ -119,15 +125,15 @@
 
 ### Output
 
 The following formats were tested and optimized for use:
 
 #### LDR
 
-- PNG
+- PNG, APNG
 - TGA
 - TIFF (default)
 
 #### HDR
 
 - EXR (default)
 - TIFF
@@ -138,18 +144,14 @@
 
 ### Color space
 
 Color space of LDR textures is inferred from the context in which the texture is used in-game. Since this context is not available when converting the .vtf files directly, color space metadata for the output images cannot be set.
 
 Color space of HDR textures is always linear. It would make sense to set this metadata when converting into the TIFF format, but for technical reasons, this is not done.
 
-### Opaque PNG
-
-When using PNG, the alpha channel is not written when the image is fully opaque. This may pose problems in other programs. In Blender, for example, when such image is not packed and OSL is enabled, the alpha channel is shown as black. For this reason, TIFF is the default LDR format instead of PNG.
-
 ## Benchmark
 
 - Sample: 11 GiB of LDR .vtf files
 - CPU: Intel Core i7-6500U
 
 Size is the total disk usage consumed by the output.
 Conversion was done without extraction of all mipmaps.
```

### Comparing `no_vtf-3.0.1/builds/common` & `no_vtf-3.1.0/builds/common`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/builds/debian/wine-install.sh` & `no_vtf-3.1.0/builds/debian/wine-install.sh`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/bin/bash
 
 # SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
-source builds/common
+source builds/common || exit
 
 WINEHQ_KEYRING_PATH='/usr/share/keyrings/winehq-archive-keyring.gpg'
 
 sudo dpkg --add-architecture i386
 
 curl 'https://dl.winehq.org/wine-builds/winehq.key' |
 	gpg --dearmor |
```

### Comparing `no_vtf-3.0.1/builds/publish_frozen.sh` & `no_vtf-3.1.0/builds/publish_frozen.sh`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/bin/bash
 
 # SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
-source builds/common
+source builds/common || exit
 
 ARCHIVE='release.tar.gz'
 SITE='b5327157.srht.site'
 SUBDIRECTORY='no_vtf/release'
 
 acurl() (
 	set +x
```

### Comparing `no_vtf-3.0.1/builds/with_wine.sh` & `no_vtf-3.1.0/builds/with_wine.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/bin/bash
 
 # SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
-source builds/common
+source builds/common || exit
 
 [ -n "$1" ]
 workdir="$1"
 shift
 
 [ -n "$1" ]
```

### Comparing `no_vtf-3.0.1/ksy/vtf.ksy` & `no_vtf-3.1.0/ksy/vtf.ksy`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/no_vtf/deferred/deferred.py` & `no_vtf-3.1.0/no_vtf/deferred/deferred.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/no_vtf/filesystem/input_paths.py` & `no_vtf-3.1.0/no_vtf/filesystem/input_paths.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/no_vtf/filesystem/output_directories.py` & `no_vtf-3.1.0/no_vtf/filesystem/output_directories.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/no_vtf/image/channel_separator.py` & `no_vtf-3.1.0/no_vtf/image/channel_separator.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/no_vtf/image/decoder/generic.py` & `no_vtf-3.1.0/no_vtf/image/decoder/generic.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/no_vtf/image/decoder/vtf.py` & `no_vtf-3.1.0/no_vtf/image/decoder/vtf.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/no_vtf/image/image.py` & `no_vtf-3.1.0/no_vtf/image/image.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/no_vtf/image/modifier/fp_precision_modifier.py` & `no_vtf-3.1.0/no_vtf/image/modifier/fp_precision_modifier.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/no_vtf/image/modifier/modifier.py` & `no_vtf-3.1.0/no_vtf/image/modifier/modifier.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/no_vtf/image/ndarray.py` & `no_vtf-3.1.0/no_vtf/image/ndarray.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/no_vtf/io/image.py` & `no_vtf-3.1.0/no_vtf/io/image.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 from __future__ import annotations
 
 import functools
+import itertools
 import pathlib
 import re
 
+from collections.abc import Sequence
 from dataclasses import dataclass
-from typing import ClassVar, Optional, cast
+from typing import ClassVar, Literal, Optional, Protocol, cast
 
 import imageio.plugins.freeimage
 import imageio.v3
 import numpy as np
 import numpy.typing as npt
 
 from no_vtf.image import Image, ImageData, ImageDataTypes
@@ -23,91 +25,109 @@
 
 
 @dataclass(frozen=True, kw_only=True)
 class ImageIO(IO[Image[ImageDataTypes]]):
     format: str
 
     compress: Optional[bool] = None
+    fps: Optional[int] = None
 
     @classmethod
     def _initialize(cls) -> None:
         # download() seems to be untyped because of implicit reexport
         imageio.plugins.freeimage.download()  # type: ignore[no-untyped-call]
 
     _format_pattern: ClassVar[re.Pattern[str]] = re.compile(r"[a-z0-9]+", re.ASCII | re.IGNORECASE)
 
     def __post_init__(self) -> None:
         assert self._is_initialized(), "IO.initialize() must be called early"
 
         if not self._format_pattern.fullmatch(self.format):
             raise RuntimeError(f"Invalid format: {self.format}")
 
-    def write(self, path: pathlib.Path, image: Image[ImageDataTypes]) -> None:
+    def write_sequence(self, path: pathlib.Path, sequence: Sequence[Image[ImageDataTypes]]) -> None:
         backend = self._get_backend()
-        backend.write(path, image)
+        backend.write(path, sequence)
 
-    def readback(self, path: pathlib.Path, image: Image[ImageDataTypes]) -> None:
+    def readback_sequence(
+        self, path: pathlib.Path, sequence: Sequence[Image[ImageDataTypes]]
+    ) -> None:
         backend = self._get_backend()
-        backend.readback(path, image)
+        backend.readback(path, sequence)
 
     def _get_backend(self) -> _ImageIOBackend:
         compress = self.compress
         if compress is None:
             compress = True
 
         extension = f".{self.format}"
 
         backend: _ImageIOBackend
         match self.format.lower():
+            case "apng":
+                backend = _ImageIOApngBackend(compress=compress, fps=self.fps)
             case "exr":
                 backend = _ImageIOExrBackend(compress=compress)
             case "png":
                 backend = _ImageIOPngBackend(compress=compress)
             case "targa" | "tga":
                 backend = _ImageIOTgaBackend(compress=compress)
             case "tiff":
                 backend = _ImageIOTiffBackend(compress=compress)
             case _:
                 backend = _ImageIOBackend(extension=extension)
         return backend
 
 
+class _Opener(Protocol):
+    def __call__(
+        self,
+        uri: imageio.typing.ImageResource,
+        io_mode: Literal["r", "w"],
+        *,
+        extension: Optional[str] = None,
+        format_hint: Optional[str] = None,
+    ) -> imageio.core.v3_plugin_api.PluginV3:
+        ...
+
+
 class _ImageIOBackend:
-    def __init__(
-        self, *, imageio_format: Optional[str] = None, extension: Optional[str] = None
-    ) -> None:
-        self._imageio_format = imageio_format
+    def __init__(self, *, extension: Optional[str] = None) -> None:
         self._extension = extension
 
-    def write(self, path: pathlib.Path, image: Image[ImageDataTypes]) -> None:
-        kwargs = self._get_writer_kwargs(image)
-        image = self._postprocess(image)
-        data = self._get_data(image)
-
-        legacy_opener = functools.partial(imageio.v3.imopen, legacy_mode=True)
-        with legacy_opener(
-            path, "w", plugin=self._imageio_format, extension=self._extension
-        ) as image_resource:
-            image_resource.write(data, **kwargs)
-
-    def readback(self, path: pathlib.Path, image: Image[ImageDataTypes]) -> None:
-        image = self._postprocess(image)
-        data = self._get_data(image)
-
-        legacy_opener = functools.partial(imageio.v3.imopen, legacy_mode=True)
-        with legacy_opener(
-            path, "r", plugin=self._imageio_format, extension=self._extension
-        ) as image_resource:
-            read_data = image_resource.read(index=0)
+    def write(self, path: pathlib.Path, sequence: Sequence[Image[ImageDataTypes]]) -> None:
+        opener = self._get_opener()
+        with opener(path, "w", extension=self._extension) as image_resource:
+            for image in sequence:
+                kwargs = self._get_writer_kwargs(image)
+                image = self._postprocess(image)
+                data = self._get_data(image)
+
+                image_resource.write(data, **kwargs)
+
+    def readback(self, path: pathlib.Path, sequence: Sequence[Image[ImageDataTypes]]) -> None:
+        opener = self._get_opener()
+        with opener(path, "r", extension=self._extension) as image_resource:
+            for image, read_data in itertools.zip_longest(sequence, image_resource.iter()):
+                if image is None or read_data is None:
+                    raise RuntimeError(
+                        f"{path!r}: Number of frames differs from what is in the file"
+                    )
+
+                image = self._postprocess(image)
+                data = self._get_data(image)
+
+                if data.dtype != read_data.dtype:
+                    raise RuntimeError(f"{path!r}: Data type differs from what is in the file")
 
-            if data.dtype != read_data.dtype:
-                raise RuntimeError(f"{path!r}: Data type differs from what is in the file")
+                if not self._compare_data(data, read_data):
+                    raise RuntimeError(f"{path!r}: Data differs from what is in the file")
 
-            if not self._compare_data(data, read_data):
-                raise RuntimeError(f"{path!r}: Data differs from what is in the file")
+    def _get_opener(self) -> _Opener:
+        return cast(_Opener, imageio.v3.imopen)
 
     def _get_writer_kwargs(self, image: Image[ImageDataTypes]) -> dict[str, object]:
         return {}
 
     def _postprocess(self, image: Image[ImageDataTypes]) -> Image[ImageDataTypes]:
         return image
 
@@ -126,22 +146,65 @@
 
         return data
 
     def _compare_data(self, data: ImageData, read_data: ImageData) -> bool:
         return np.array_equal(data, read_data)
 
 
-class _ImageIOFreeImageBackend(_ImageIOBackend):
+class _ImageIOPillowBackend(_ImageIOBackend):
+    def __init__(self, *, extension: Optional[str] = None) -> None:
+        super().__init__(extension=extension)
+
+    def _get_opener(self) -> _Opener:
+        return functools.partial(imageio.v3.imopen, plugin="pillow")
+
+
+class _ImageIOPngBackend(_ImageIOPillowBackend):
+    def __init__(self, *, compress: bool = True, extension: str = ".png") -> None:
+        super().__init__(extension=extension)
+        self.compress = compress
+
+    def _get_writer_kwargs(self, image: Image[ImageDataTypes]) -> dict[str, object]:
+        kwargs = super()._get_writer_kwargs(image)
+        if not self.compress:
+            kwargs["compress_level"] = 0
+        return kwargs
+
+
+class _ImageIOApngBackend(_ImageIOPngBackend):
+    def __init__(self, *, compress: bool = True, fps: Optional[int] = None) -> None:
+        super().__init__(compress=compress, extension=".apng")
+        self._fps = fps
+
+    def _get_writer_kwargs(self, image: Image[ImageDataTypes]) -> dict[str, object]:
+        kwargs = super()._get_writer_kwargs(image)
+        if self._fps:
+            kwargs["duration"] = 1000 / self._fps
+        return kwargs
+
+
+class _ImageIOLegacyBackend(_ImageIOBackend):
+    def __init__(
+        self, *, imageio_format: Optional[str] = None, extension: Optional[str] = None
+    ) -> None:
+        super().__init__(extension=extension)
+        self._imageio_format = imageio_format
+
+    def _get_opener(self) -> _Opener:
+        return functools.partial(imageio.v3.imopen, legacy_mode=True, plugin=self._imageio_format)
+
+
+class _ImageIOFreeImageBackend(_ImageIOLegacyBackend):
     IO_FLAGS: ClassVar = imageio.plugins.freeimage.IO_FLAGS
 
     def __init__(self, *, imageio_format: str, extension: str) -> None:
         super().__init__(imageio_format=imageio_format, extension=extension)
 
     def _get_writer_kwargs(self, image: Image[ImageDataTypes]) -> dict[str, object]:
-        kwargs: dict[str, object] = {}
+        kwargs = super()._get_writer_kwargs(image)
         kwargs["flags"] = self._get_flags(image)
         return kwargs
 
     def _get_flags(self, image: Image[ImageDataTypes]) -> int:
         return 0
 
 
@@ -161,32 +224,14 @@
             flags |= self.IO_FLAGS.EXR_FLOAT
         return flags
 
     def _postprocess(self, image: Image[ImageDataTypes]) -> Image[ImageDataTypes]:
         return self._fp_force_32_bits(image)
 
 
-class _ImageIOPngBackend(_ImageIOFreeImageBackend):
-    def __init__(self, *, compress: bool = True) -> None:
-        super().__init__(imageio_format="PNG-FI", extension=".png")
-        self.compress = compress
-
-    def _get_writer_kwargs(self, image: Image[ImageDataTypes]) -> dict[str, object]:
-        kwargs: dict[str, object] = super()._get_writer_kwargs(image)
-        kwargs["compression"] = 1 if self.compress else 0
-        return kwargs
-
-    def _compare_data(self, data: ImageData, read_data: ImageData) -> bool:
-        if np.issubdtype(data.dtype, np.uint8) and np.issubdtype(read_data.dtype, np.uint8):
-            if read_data.ndim == 3 and read_data.shape[2] == 3:
-                data = _strip_opaque_alpha(cast(npt.NDArray[np.uint8], data))
-
-        return super()._compare_data(data, read_data)
-
-
 class _ImageIOTgaBackend(_ImageIOFreeImageBackend):
     def __init__(self, *, compress: bool = True) -> None:
         super().__init__(imageio_format="TARGA-FI", extension=".tga")
         self.compress = compress
 
     def _get_flags(self, image: Image[ImageDataTypes]) -> int:
         flags = 0
@@ -206,14 +251,7 @@
     def _get_flags(self, image: Image[ImageDataTypes]) -> int:
         flags = 0
         flags |= self.IO_FLAGS.TIFF_DEFAULT if self.compress else self.IO_FLAGS.TIFF_NONE
         return flags
 
     def _postprocess(self, image: Image[ImageDataTypes]) -> Image[ImageDataTypes]:
         return self._fp_force_32_bits(image)
-
-
-def _strip_opaque_alpha(data: npt.NDArray[np.uint8]) -> npt.NDArray[np.uint8]:
-    if data.ndim == 3 and data.shape[2] == 4 and np.all(data[..., 3] == 255):
-        data = data[..., :3]
-
-    return data
```

### Comparing `no_vtf-3.0.1/no_vtf/io/io.py` & `no_vtf-3.1.0/no_vtf/io/io.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 import pathlib
 
 from abc import abstractmethod
+from collections.abc import Sequence
 from typing import ClassVar, Generic, TypeVar
 
 import no_vtf.io  # noqa: F401  # define all task runners for IO.initialize()
 
 _A_contra = TypeVar("_A_contra", contravariant=True)
 
 
@@ -26,14 +27,20 @@
     def _is_initialized(cls) -> bool:
         return cls._initialized
 
     @classmethod
     def _initialize(cls) -> None:
         pass
 
-    @abstractmethod
     def write(self, path: pathlib.Path, data: _A_contra, /) -> None:
+        self.write_sequence(path, [data])
+
+    def readback(self, path: pathlib.Path, data: _A_contra, /) -> None:
+        self.readback_sequence(path, [data])
+
+    @abstractmethod
+    def write_sequence(self, path: pathlib.Path, sequence: Sequence[_A_contra], /) -> None:
         ...
 
     @abstractmethod
-    def readback(self, path: pathlib.Path, data: _A_contra, /) -> None:
+    def readback_sequence(self, path: pathlib.Path, sequence: Sequence[_A_contra], /) -> None:
         ...
```

### Comparing `no_vtf-3.0.1/no_vtf/parser/generated/vtf.py` & `no_vtf-3.1.0/no_vtf/parser/generated/vtf.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/no_vtf/task_runner/parallel.py` & `no_vtf-3.1.0/no_vtf/task_runner/parallel.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/no_vtf/task_runner/sequential.py` & `no_vtf-3.1.0/no_vtf/task_runner/sequential.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/no_vtf/task_runner/task_runner.py` & `no_vtf-3.1.0/no_vtf/task_runner/task_runner.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/no_vtf/texture/decoder/vtf.py` & `no_vtf-3.1.0/no_vtf/texture/decoder/vtf.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/no_vtf/texture/extractor/vtf.py` & `no_vtf-3.1.0/no_vtf/texture/extractor/vtf.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/no_vtf/texture/namer/vtf.py` & `no_vtf-3.1.0/no_vtf/texture/namer/vtf.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 from no_vtf.texture.namer.namer import TextureNamer
 from no_vtf.texture.vtf import VtfTexture
 
 
 @dataclass(frozen=True, kw_only=True)
 class Vtf2TgaLikeNamer(TextureNamer[VtfTexture]):
     include_mipmap_level: bool
+    include_frame: bool = True
 
     def __call__(self, input_name: str, texture: VtfTexture) -> str:
         output_name = input_name
 
         if texture.is_cubemap:
             face_names = ("rt", "lf", "bk", "ft", "up", "dn", "sph")
             output_name += face_names[texture.face_index]
 
-        if texture.num_frames > 1:
+        if self.include_frame and texture.num_frames > 1:
             output_name += f"{texture.frame_index:03d}"
 
         if self.include_mipmap_level and texture.num_mipmaps > 1:
             mipmap_level = texture.num_mipmaps - texture.mipmap_index - 1
             output_name += f"_mip{mipmap_level}"
 
         if texture.num_slices > 1:
```

### Comparing `no_vtf-3.0.1/no_vtf/texture/vtf.py` & `no_vtf-3.1.0/no_vtf/texture/vtf.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/no_vtf.egg-info/PKG-INFO` & `no_vtf-3.1.0/no_vtf.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: no-vtf
-Version: 3.0.1
+Version: 3.1.0
 Summary: Valve Texture Format Converter
 Home-page: https://sr.ht/~b5327157/no_vtf
 Author: b5327157
 Author-email: b5327157@protonmail.com
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Download, https://sr.ht/~b5327157/no_vtf/#application-bundle
 Project-URL: Changelog, https://git.sr.ht/~b5327157/no_vtf/refs
@@ -25,15 +25,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSES/GPL-3.0-or-later.txt
 
 # no_vtf
 
-Say no to [.vtf](https://developer.valvesoftware.com/wiki/Valve_Texture_Format) – convert it to one of the standard image formats.
+Say no to [Source Engine](https://developer.valvesoftware.com/wiki/Source)'s [.vtf](https://developer.valvesoftware.com/wiki/Valve_Texture_Format) – convert it to one of the standard image formats.
 
 ![Badge showing supported Python versions](https://img.shields.io/pypi/pyversions/no_vtf?style=flat-square)
 [![Badge showing package version on PyPI](https://img.shields.io/pypi/v/no_vtf?style=flat-square)](https://pypi.org/project/no-vtf/)
 [![Badge showing number of monthly downloads from PyPI](https://img.shields.io/pypi/dm/no_vtf?style=flat-square)](https://pypistats.org/packages/no-vtf)
 [![Badge showing source code repository hosted on SourceHut](https://img.shields.io/badge/sr.ht-repository-white?labelColor=212529&logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjxzdmcKICAgdmlld0JveD0iMCAwIDUxMiA1MTIiCiAgIHZlcnNpb249IjEuMSIKICAgaWQ9InN2ZzUxIgogICBzb2RpcG9kaTpkb2NuYW1lPSJzb3VyY2VodXQtd2hpdGUuc3ZnIgogICBpbmtzY2FwZTp2ZXJzaW9uPSIxLjEgKGM2OGUyMmMzODcsIDIwMjEtMDUtMjMpIgogICB4bWxuczppbmtzY2FwZT0iaHR0cDovL3d3dy5pbmtzY2FwZS5vcmcvbmFtZXNwYWNlcy9pbmtzY2FwZSIKICAgeG1sbnM6c29kaXBvZGk9Imh0dHA6Ly9zb2RpcG9kaS5zb3VyY2Vmb3JnZS5uZXQvRFREL3NvZGlwb2RpLTAuZHRkIgogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciCiAgIHhtbG5zOnN2Zz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgogIDxkZWZzCiAgICAgaWQ9ImRlZnM1NSIgLz4KICA8c29kaXBvZGk6bmFtZWR2aWV3CiAgICAgaWQ9Im5hbWVkdmlldzUzIgogICAgIHBhZ2Vjb2xvcj0iIzUwNTA1MCIKICAgICBib3JkZXJjb2xvcj0iI2ZmZmZmZiIKICAgICBib3JkZXJvcGFjaXR5PSIxIgogICAgIGlua3NjYXBlOnBhZ2VzaGFkb3c9IjAiCiAgICAgaW5rc2NhcGU6cGFnZW9wYWNpdHk9IjAiCiAgICAgaW5rc2NhcGU6cGFnZWNoZWNrZXJib2FyZD0iMSIKICAgICBzaG93Z3JpZD0iZmFsc2UiCiAgICAgaW5rc2NhcGU6em9vbT0iMS42NTQyOTY5IgogICAgIGlua3NjYXBlOmN4PSIyNTYiCiAgICAgaW5rc2NhcGU6Y3k9IjI1NiIKICAgICBpbmtzY2FwZTp3aW5kb3ctd2lkdGg9IjE5MjAiCiAgICAgaW5rc2NhcGU6d2luZG93LWhlaWdodD0iMTA1OSIKICAgICBpbmtzY2FwZTp3aW5kb3cteD0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3cteT0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3ctbWF4aW1pemVkPSIxIgogICAgIGlua3NjYXBlOmN1cnJlbnQtbGF5ZXI9InN2ZzUxIiAvPgogIDxwYXRoCiAgICAgZD0iTTI1NiA4QzExOSA4IDggMTE5IDggMjU2czExMSAyNDggMjQ4IDI0OCAyNDgtMTExIDI0OC0yNDhTMzkzIDggMjU2IDh6bTAgNDQ4Yy0xMTAuNSAwLTIwMC04OS41LTIwMC0yMDBTMTQ1LjUgNTYgMjU2IDU2czIwMCA4OS41IDIwMCAyMDAtODkuNSAyMDAtMjAwIDIwMHoiCiAgICAgaWQ9InBhdGg0OSIKICAgICBzdHlsZT0iZmlsbDojZmZmZmZmIiAvPgo8L3N2Zz4K)](https://sr.ht/~b5327157/no_vtf)
 [![Badge showing builds.sr.ht status](https://builds.sr.ht/~b5327157/no_vtf.svg?search=tags:master)](https://builds.sr.ht/~b5327157/no_vtf?search=tags:master)
 [![Badge showing REUSE compliance status](https://api.reuse.software/badge/git.sr.ht/~b5327157/no_vtf)](https://api.reuse.software/info/git.sr.ht/~b5327157/no_vtf)
@@ -110,14 +110,20 @@
 
 #### Override LDR/HDR output format
 
 ```
 no_vtf --ldr-format png --hdr-format tiff PATH...
 ```
 
+#### Convert animated texture
+
+```
+no_vtf --animate --fps 20 PATH...
+```
+
 #### Further help
 
 ```
 no_vtf --help
 ```
 
 ## Supported formats
@@ -148,15 +154,15 @@
 
 ### Output
 
 The following formats were tested and optimized for use:
 
 #### LDR
 
-- PNG
+- PNG, APNG
 - TGA
 - TIFF (default)
 
 #### HDR
 
 - EXR (default)
 - TIFF
@@ -167,18 +173,14 @@
 
 ### Color space
 
 Color space of LDR textures is inferred from the context in which the texture is used in-game. Since this context is not available when converting the .vtf files directly, color space metadata for the output images cannot be set.
 
 Color space of HDR textures is always linear. It would make sense to set this metadata when converting into the TIFF format, but for technical reasons, this is not done.
 
-### Opaque PNG
-
-When using PNG, the alpha channel is not written when the image is fully opaque. This may pose problems in other programs. In Blender, for example, when such image is not packed and OSL is enabled, the alpha channel is shown as black. For this reason, TIFF is the default LDR format instead of PNG.
-
 ## Benchmark
 
 - Sample: 11 GiB of LDR .vtf files
 - CPU: Intel Core i7-6500U
 
 Size is the total disk usage consumed by the output.
 Conversion was done without extraction of all mipmaps.
```

### Comparing `no_vtf-3.0.1/no_vtf.egg-info/SOURCES.txt` & `no_vtf-3.1.0/no_vtf.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -83,9 +83,8 @@
 no_vtf/texture/namer/__init__.py
 no_vtf/texture/namer/namer.py
 no_vtf/texture/namer/vtf.py
 resources/docs/screencast.gif
 resources/docs/screencast.gif.license
 resources/pyinstaller/empty.ico
 resources/pyinstaller/empty.ico.license
-resources/pyinstaller/no_vtf.desktop
-resources/pyinstaller/no_vtf.desktop.license
+resources/pyinstaller/no_vtf.desktop
```

### Comparing `no_vtf-3.0.1/noxfile.py` & `no_vtf-3.1.0/noxfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,14 +202,15 @@
     input_path = base_path / "input"
     output_path = base_path / "output"
 
     sanity_test = SanityTest(
         session=session, executable=executable, input=input_path, output=output_path
     )
     sanity_test.write()
+    sanity_test.readback()
 
 
 @dataclass(frozen=True, kw_only=True)
 class SanityTest:
     session: nox.Session
     executable: Sequence[str]
     paths: Optional[list[str]] = None
@@ -256,15 +257,15 @@
         for combination in itertools.product(*combinations):
             combination_flattened = itertools.chain.from_iterable(combination)
             self._run_formats([*args, *combination_flattened])
 
     def _run_formats(self, args: Sequence[str]) -> None:
         args = list(args)
 
-        ldr_formats = ["raw", "png", "tga", "tiff"]
+        ldr_formats = ["raw", "png", "tga", "tiff", "apng"]
         for ldr_format in ldr_formats:
             self._run([*args, "--ldr-format", ldr_format, "--hdr-format", "skip"])
 
         hdr_formats = ["raw", "exr", "tiff"]
         for hdr_format in hdr_formats:
             self._run([*args, "--ldr-format", "skip", "--hdr-format", hdr_format])
 
@@ -298,9 +299,10 @@
 def samples_archive_view() -> Iterator[pathlib.Path]:
     samples_path = pathlib.Path("resources/test/samples")
     sample_archives = [
         path
         for path in samples_path.iterdir()
         if path.is_file() and not str(path).endswith(".license")
     ]
+    sample_archives.sort()
     with archives_view(sample_archives) as samples_directory:
         yield samples_directory
```

### Comparing `no_vtf-3.0.1/pyproject.toml` & `no_vtf-3.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/resources/docs/screencast.gif` & `no_vtf-3.1.0/resources/docs/screencast.gif`

 * *Files identical despite different names*

### Comparing `no_vtf-3.0.1/setup.cfg` & `no_vtf-3.1.0/setup.cfg`

 * *Files identical despite different names*

