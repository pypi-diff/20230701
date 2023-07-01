# Comparing `tmp/dan-build-0.2.4.tar.gz` & `tmp/dan-build-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dan-build-0.2.4.tar", last modified: Fri Jun 16 06:05:16 2023, max compression
+gzip compressed data, was "dan-build-0.2.5.tar", last modified: Sat Jul  1 13:06:01 2023, max compression
```

## Comparing `dan-build-0.2.4.tar` & `dan-build-0.2.5.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.952009 dan-build-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-16 06:05:02.000000 dan-build-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-16 06:05:16.948009 dan-build-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-16 06:05:02.000000 dan-build-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.932009 dan-build-0.2.4/completion/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.936009 dan-build-0.2.4/completion/bash/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-16 06:05:02.000000 dan-build-0.2.4/completion/bash/dan-io.sh
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-16 06:05:02.000000 dan-build-0.2.4/completion/bash/dan.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.936009 dan-build-0.2.4/completion/zsh/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-16 06:05:02.000000 dan-build-0.2.4/completion/zsh/dan-io.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-16 06:05:02.000000 dan-build-0.2.4/completion/zsh/dan.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.936009 dan-build-0.2.4/dan/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.940009 dan-build-0.2.4/dan/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cli/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cli/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13511 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cli/vscode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.940009 dan-build-0.2.4/dan/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cmake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cmake/configure_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.940009 dan-build-0.2.4/dan/conan/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/conan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/conan/requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.944009 dan-build-0.2.4/dan/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/aiofiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/find.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/include.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/osinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/pm.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16928 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/core/win.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.944009 dan-build-0.2.4/dan/cxx/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/compile_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.944009 dan-build-0.2.4/dan/cxx/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/data/detect.cmd
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/data/empty.c
--rw-r--r--   0 runner    (1001) docker     (123)    24471 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/msvc_toolchain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.944009 dan-build-0.2.4/dan/cxx/support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/support/qt.py
--rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9903 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/toolchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/cxx/unix_toolchain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.948009 dan-build-0.2.4/dan/io/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/io/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/io/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    20464 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/make.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.948009 dan-build-0.2.4/dan/pkgconfig/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/pkgconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/pkgconfig/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.948009 dan-build-0.2.4/dan/pkgconfig/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/pkgconfig/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/pkgconfig/templates/pkg.pc.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.948009 dan-build-0.2.4/dan/src/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/src/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/src/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/src/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-16 06:05:02.000000 dan-build-0.2.4/dan/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.948009 dan-build-0.2.4/dan_build.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-16 06:05:16.000000 dan-build-0.2.4/dan_build.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-16 06:05:16.000000 dan-build-0.2.4/dan_build.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:05:16.000000 dan-build-0.2.4/dan_build.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-16 06:05:16.000000 dan-build-0.2.4/dan_build.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-16 06:05:16.000000 dan-build-0.2.4/dan_build.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-16 06:05:16.000000 dan-build-0.2.4/dan_build.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-16 06:05:02.000000 dan-build-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 06:05:16.952009 dan-build-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:05:16.948009 dan-build-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-16 06:05:02.000000 dan-build-0.2.4/tests/test_cxx_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-16 06:05:02.000000 dan-build-0.2.4/tests/test_cxx_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-16 06:05:02.000000 dan-build-0.2.4/tests/test_cxx_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-16 06:05:02.000000 dan-build-0.2.4/tests/test_cxx_src_catch2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-16 06:05:02.000000 dan-build-0.2.4/tests/test_python_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.412398 dan-build-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-01 13:05:53.000000 dan-build-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-01 13:06:01.412398 dan-build-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-01 13:05:53.000000 dan-build-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.400398 dan-build-0.2.5/completion/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.400398 dan-build-0.2.5/completion/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-01 13:05:53.000000 dan-build-0.2.5/completion/bash/dan-io.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-01 13:05:53.000000 dan-build-0.2.5/completion/bash/dan.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.400398 dan-build-0.2.5/completion/zsh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-01 13:05:53.000000 dan-build-0.2.5/completion/zsh/dan-io.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-01 13:05:53.000000 dan-build-0.2.5/completion/zsh/dan.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.400398 dan-build-0.2.5/dan/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.404399 dan-build-0.2.5/dan/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cli/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cli/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cli/vscode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.404399 dan-build-0.2.5/dan/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cmake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cmake/configure_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.404399 dan-build-0.2.5/dan/conan/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/conan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/conan/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.408398 dan-build-0.2.5/dan/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/aiofiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/osinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/pm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17254 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/core/win.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.408398 dan-build-0.2.5/dan/cxx/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/compile_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.408398 dan-build-0.2.5/dan/cxx/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/data/detect.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/data/empty.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24754 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/msvc_toolchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.408398 dan-build-0.2.5/dan/cxx/support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/support/qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19620 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/toolchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/cxx/unix_toolchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.408398 dan-build-0.2.5/dan/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/io/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/io/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20886 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/make.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.408398 dan-build-0.2.5/dan/pkgconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/pkgconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/pkgconfig/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.408398 dan-build-0.2.5/dan/pkgconfig/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/pkgconfig/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/pkgconfig/templates/pkg.pc.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.408398 dan-build-0.2.5/dan/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/src/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/src/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/src/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-01 13:05:53.000000 dan-build-0.2.5/dan/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.408398 dan-build-0.2.5/dan_build.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-01 13:06:01.000000 dan-build-0.2.5/dan_build.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-01 13:06:01.000000 dan-build-0.2.5/dan_build.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 13:06:01.000000 dan-build-0.2.5/dan_build.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-01 13:06:01.000000 dan-build-0.2.5/dan_build.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-01 13:06:01.000000 dan-build-0.2.5/dan_build.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-01 13:06:01.000000 dan-build-0.2.5/dan_build.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-01 13:05:53.000000 dan-build-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 13:06:01.412398 dan-build-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:06:01.412398 dan-build-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-01 13:05:53.000000 dan-build-0.2.5/tests/test_cxx_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-01 13:05:53.000000 dan-build-0.2.5/tests/test_cxx_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-01 13:05:53.000000 dan-build-0.2.5/tests/test_cxx_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-01 13:05:53.000000 dan-build-0.2.5/tests/test_cxx_src_catch2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-01 13:05:53.000000 dan-build-0.2.5/tests/test_python_errors.py
```

### Comparing `dan-build-0.2.4/LICENSE` & `dan-build-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/PKG-INFO` & `dan-build-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dan-build
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python-based build system.
 Author-email: Garcia Sylvain <garcia.6l20@gmail.com>, garcia.6l20@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Sylvain Garcia
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dan-build-0.2.4/README.md` & `dan-build-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/completion/bash/dan-io.sh` & `dan-build-0.2.5/completion/bash/dan-io.sh`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/completion/bash/dan.sh` & `dan-build-0.2.5/completion/bash/dan.sh`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/completion/zsh/dan-io.sh` & `dan-build-0.2.5/completion/zsh/dan-io.sh`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/completion/zsh/dan.sh` & `dan-build-0.2.5/completion/zsh/dan.sh`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/cli/main.py` & `dan-build-0.2.5/dan/cli/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -88,39 +88,31 @@
               help='Maximum jobs', default=None, type=int)
 @click.pass_context
 def cli(ctx: click.AsyncContext, **kwds):
     ctx.obj = CommandsContext(**kwds)
     ctx.call_on_close(show_diags)
 
 
-def available_toolchains():
-    from dan.cxx.detect import get_toolchains
-    return ['default', *[name for name in get_toolchains(create=False)['toolchains'].keys()]]
-
-
-_toolchain_choice = click.Choice(available_toolchains(), case_sensitive=False)
-
-
 @cli.command()
 @click.option('--verbose', '-v', is_flag=True,
               help='Pring debug informations')
 @click.option('--toolchain', '-t', help='The toolchain to use',
-              type=_toolchain_choice)
+              type=click.ToolchainParamType())
 @click.option('--setting', '-s', 'settings', help='Set or change a setting', multiple=True, type=click.SettingsParamType(Settings))
-@click.option('--option', '-o', 'options', help='Set or change an option', multiple=True)
+@click.option('--option', '-o', 'options', help='Set or change an option', multiple=True, type=click.OptionsParamType())
 @click.option('--build-path', '-B', help='Path where dan has been initialized.',
               type=click.Path(resolve_path=True, path_type=Path), required=True, default='build', envvar='DAN_BUILD_PATH')
 @click.option('--source-path', '-S', help='Path where source is located.',
               type=click.Path(resolve_path=True, path_type=Path), required=True, default='.')
 @pass_context
 async def configure(ctx: CommandsContext, toolchain: str, settings: tuple[str], options: tuple[str], source_path: Path, **kwds):
     """Configure dan project"""
     ctx(**kwds)  # update kwds
     if toolchain is None and ctx.make.config.toolchain is None:
-        toolchain = click.prompt('Toolchain', type=_toolchain_choice, default='default')
+        toolchain = click.prompt('Toolchain', type=click.ToolchainParamType(), default='default')
 
     await ctx.make.configure(source_path, toolchain)
 
     if len(settings):
         await ctx.make.apply_settings(*settings)
 
     # NOTE: intializing make after applying setting
@@ -132,30 +124,30 @@
 
 
 @cli.command()
 @click.option('--for-install', is_flag=True, help='Build for install purpose (will update rpaths [posix only])')
 @common_opts
 @click.option('--force', '-f', is_flag=True,
               help='Clean before building')
-@click.argument('TARGETS', nargs=-1)
+@click.argument('TARGETS', nargs=-1, type=click.TargetParamType())
 @pass_context
 async def build(ctx: CommandsContext, force=False, **kwds):
     """Build targets"""
     ctx(**kwds)  # update kwds
     if force:
         await ctx.make.clean()
     await ctx.make.build()
     # from dan.cxx import target_toolchain
     # target_toolchain.compile_commands.update()
 
 
 @cli.command()
 @common_opts
 @click.argument('MODE', type=click.Choice([v.name for v in InstallMode]), default=InstallMode.user.name)
-@click.argument('TARGETS', nargs=-1)
+@click.argument('TARGETS', nargs=-1, type=click.TargetParamType())
 @pass_context
 async def install(ctx: CommandsContext, mode: str, **kwargs):
     """Install targets"""
     ctx(**kwargs)
     mode = InstallMode[mode]
     await ctx.make.install(mode)
 
@@ -262,36 +254,36 @@
     kwargs['quiet'] = True
     for name, _ in Make.toolchains()['toolchains'].items():
         click.echo(name)
 
 
 @cli.command()
 @common_opts
-@click.argument('TARGETS', nargs=-1)
+@click.argument('TARGETS', nargs=-1, type=click.TargetParamType())
 @pass_context
 async def clean(ctx, **kwargs):
     """Clean generated stuff"""
     ctx(**kwargs)
     await ctx.make.clean()
 
 
 @cli.command()
 @common_opts
-@click.argument('TARGETS', nargs=-1)
+@click.argument('TARGETS', nargs=-1, type=click.TargetParamType())
 @pass_context
 async def run(ctx, **kwargs):
     """Run executable(s)"""
     ctx(**kwargs)
     rc = await ctx.make.run()
     sys.exit(rc)
 
 
 @cli.command()
 @common_opts
-@click.argument('TARGETS', nargs=-1)
+@click.argument('TARGETS', nargs=-1, type=click.TargetParamType())
 @pass_context
 async def test(ctx, **kwargs):
     """Run tests"""
     ctx(**kwargs)
     rc = await ctx.make.test()
     sys.exit(rc)
 
@@ -431,8 +423,9 @@
         import traceback
         click.logger.debug(' '.join(traceback.format_tb(tb)))
         try:
             # wait asyncio loop to terminate
             asyncio.get_running_loop().run_until_complete()
         except Exception:
             pass
+        asyncio.run(Cache.save_all())
         return -1
```

### Comparing `dan-build-0.2.4/dan/cli/vscode.py` & `dan-build-0.2.5/dan/cli/vscode.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/cmake/configure_file.py` & `dan-build-0.2.5/dan/cmake/configure_file.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/conan/requirements.py` & `dan-build-0.2.5/dan/conan/requirements.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/core/aiofiles.py` & `dan-build-0.2.5/dan/core/aiofiles.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/core/asyncio.py` & `dan-build-0.2.5/dan/core/asyncio.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,37 +2,64 @@
 
 import threading
 import typing as t
 
 from dan.core.functools import BaseDecorator
 
 
-class cached(BaseDecorator):
+class Cached(BaseDecorator):
 
-    def __init__(self, fn):
+    def __init__(self, fn, unique=False):
         self.__fn = fn
-        self.__cache: dict[int, Future] = dict()
+        self.__unique = unique
+        self.__is_method = fn.__call__.__class__.__name__ == 'method-wrapper'
+        if not self.__is_method and self.__unique:
+            self.__cache = None
+        else:
+            self.__cache: dict[int, Future] = dict()
 
     async def __call__(self, *args, **kwds):
-        key = hash((args, frozenset(kwds)))
-        if key not in self.__cache:
-            self.__cache[key] = Future()
-            try:
-                self.__cache[key].set_result(await self.__fn(*args, **kwds))
-            except Exception as ex:
-                self.__cache[key].set_exception(ex)
-        elif not self.__cache[key].done():
-            await self.__cache[key]
+        if not self.__is_method and self.__unique:
+            if self.__cache is None:
+                self.__cache = Future()
+                try:
+                    self.__cache.set_result(await self.__fn(*args, **kwds))
+                except Exception as ex:
+                    self.__cache.set_exception(ex)
+            elif not self.__cache.done():
+                await self.__cache
+            return self.__cache.result()
+        else:
+            key = id(args[0]) if self.__unique else hash((args, frozenset(kwds)))
+            if key not in self.__cache:
+                self.__cache[key] = Future()
+                try:
+                    self.__cache[key].set_result(await self.__fn(*args, **kwds))
+                except Exception as ex:
+                    self.__cache[key].set_exception(ex)
+            elif not self.__cache[key].done():
+                await self.__cache[key]
 
-        return self.__cache[key].result()
+            return self.__cache[key].result()
 
     def clear_all(self):
-        self.__cache = dict()
+        if self.__unique:
+            self.__cache = dict()
+        else:
+            self.__cache = None
 
 
+def cached(*args, **kwargs):
+    if len(args) == 1 and callable(args[0]):
+        return Cached(args[0])
+    else:
+        def wrapper(fn):
+            return Cached(fn, *args, **kwargs)
+        return wrapper
+
 class _SyncWaitThread(threading.Thread):
     def __init__(self, coro):
         self.coro = coro
         self.result = None
         self.err = None
         super().__init__()
```

### Comparing `dan-build-0.2.4/dan/core/cache.py` & `dan-build-0.2.5/dan/core/cache.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/core/diagnostics.py` & `dan-build-0.2.5/dan/core/diagnostics.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/core/find.py` & `dan-build-0.2.5/dan/core/find.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/core/functools.py` & `dan-build-0.2.5/dan/core/functools.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/core/generator.py` & `dan-build-0.2.5/dan/core/generator.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/core/include.py` & `dan-build-0.2.5/dan/core/include.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 class Context(Logging):
     def __init__(self) -> None:
         self.__root: MakeFile = None
         self.__current: MakeFile = None
         self.__all_makefiles: set[MakeFile] = set()
         self.imported_makefiles: dict[Path, MakeFile] = dict()
         self.__prev_ctx: Context = None
+        self.__attributes = dict()
         super().__init__('context')
 
     @property
     def root(self):
         return self.__root
 
     @property
@@ -65,22 +66,22 @@
         self.__all_makefiles.add(current)
 
     def up(self):
         if self.__current != self.__root:
             self.__current = self.__current.parent
 
     def get(self, name, default=None):
-        if hasattr(self, name):
-            return getattr(self, name)
+        if name in self.__attributes:
+            return self.__attributes[name]
         if default is not None:
-            setattr(self, name, default)
+            self.__attributes[name] = default
             return default
 
     def set(self, name, value):
-        setattr(self, name, value)
+        self.__attributes[name] = value
 
     def __enter__(self):
         global context
         self.__prev_ctx = context
         context = self
         return self
```

### Comparing `dan-build-0.2.4/dan/core/makefile.py` & `dan-build-0.2.5/dan/core/makefile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from functools import cached_property
+import functools
 from pathlib import Path
 import sys
 
 from dan.core.cache import Cache
 from dan.core.target import Options, Target
 from dan.core.test import Test
 
@@ -39,57 +40,87 @@
 
     @property
     def cache(self) -> Cache:
         if not self.__cache:
             self.__cache = Cache(
                 self.build_path / f'{self.name}.cache', cache_name=self.fullname, binary=True)
         return self.__cache
+    
+    @property
+    def parents(self):
+        parent = self.parent
+        while parent is not None:
+            yield parent
+            parent = parent.parent
+
 
+    __target_fullnames = list()
+    __test_fullnames = list()
     def register(self, cls: type[Target | Test]):
         """Register Target/Test class"""
+        t = cls()
         if issubclass(cls, Target):
-            self.__targets.add(cls())
+            # if t.fullname in MakeFile.__target_fullnames:
+            #     raise RuntimeError(f'duplicate target name: {t.fullname}')
+            MakeFile.__target_fullnames.append(t.fullname)
+            self.__targets.add(t)
+            self.__find.cache_clear()
+            for parent in self.parents:
+                parent.__find.cache_clear()
         if issubclass(cls, Test):
-            self.__tests.add(cls())
+            # if t.fullname in MakeFile.__test_fullnames:
+            #     raise RuntimeError(f'duplicate test name: {t.fullname}')
+            MakeFile.__test_fullnames.append(t.fullname)
+            self.__tests.add(t)
         return cls
 
     def wraps(self, cls: type[Target]):
         def decorator(new_cls: type[Target]):
             assert issubclass(
                 new_cls, cls), 'Target wrapper must inherit from original target'
             for t in self.__targets:
                 if type(t) == cls:
                     self.__targets.remove(t)
-                    return cls
+                    return new_cls
             assert False, 'Original target has not been registered'
         return decorator
 
-    def find(self, name_or_class) -> Target:
-        """Find a target.
-
-        Args:
-            name (str): The target name to find.
 
-        Returns:
-            Target: The found target or None.
-        """
+    @functools.cache
+    def __find(self, name_or_class) -> Target:
         if isinstance(name_or_class, type):
             def check(t: Target):
                 return type(t) == name_or_class
         else:
             def check(t: Target):
                 return t.name == name_or_class
         for t in self.targets:
             if check(t):
                 return t
         for c in self.children:
-            t = c.find(name_or_class)
+            t = c.__find(name_or_class)
             if t:
                 return t
-    
+
+    def find(self, name_or_class) -> Target:
+        """Find a target.
+
+        Args:
+            name (str): The target name to find.
+
+        Returns:
+            Target: The found target or None.
+        """
+        t = self.__find(name_or_class)
+        if t is not None:
+            return t
+        
+        if self.parent:
+            return self.parent.find(name_or_class)
+
     def __getitem__(self, name_or_class) -> Target:
         return self.find(name_or_class)
 
     @property
     def requirements(self):
         if self.name == 'dan-requires':
             return self
```

### Comparing `dan-build-0.2.4/dan/core/osinfo.py` & `dan-build-0.2.5/dan/core/osinfo.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/core/pathlib.py` & `dan-build-0.2.5/dan/core/pathlib.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/core/pm.py` & `dan-build-0.2.5/dan/core/pm.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/core/register.py` & `dan-build-0.2.5/dan/core/register.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/core/requirements.py` & `dan-build-0.2.5/dan/core/requirements.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,32 +39,35 @@
 
 class RequiredPackage(Logging):
     def __init__(self, name: str, version_spec: VersionSpec = None):
         self.version_spec = version_spec
         super().__init__(name)
         self.target : 'Target' = None
         self.package, self.name, self.repository = parse_package(name)
+        self.__skipped = list()
 
     def is_compatible(self, t: 'Target'):
         if self.version_spec is not None:
             version_ok = self.version_spec.is_compatible(t.version)
         else:
             version_ok = True
-        return t.name == self.name and version_ok
+        return version_ok
     
     @property
     def found(self):
         return self.target is not None
     
     @property
     def modification_time(self):
         return self.target.modification_time if self.target else 0.0
 
     def __skipped_method_call(self, name, *args, **kwargs):
-        self.debug('call to %s skipped (unresolved)', name)
+        if name not in self.__skipped:
+            self.debug('call to %s skipped (unresolved)', name)
+            self.__skipped.append(name)
 
     def __getattr__(self, name):
         if not self.found:
             return functools.partial(self.__skipped_method_call, name)
         else:
             return getattr(self.target, name)
     
@@ -87,15 +90,15 @@
     from dan.pkgconfig.package import find_package
     from dan.logging import _get_makefile_logger
     from dan.io import Package
 
     if logger is None:
         logger = _get_makefile_logger()
 
-    deps_install_path = makefile.pkgs_path
+    deps_install_path = makefile.root.pkgs_path
     deps_settings = InstallSettings(deps_install_path)
 
     pkgs_search_paths = [deps_install_path]
     if makefile.requirements:
         pkgs_search_paths.append(makefile.requirements.pkgs_path)
 
     resolved: list[RequiredPackage] = list()
@@ -124,18 +127,21 @@
                     # install requirement from dan-requires.py
                     t = makefile.requirements.find(req.name)
                     if not t:
                         raise RuntimeError(f'Unresolved requirement {req}, it should have been defined in {makefile.requirements.__file__}')
                     logger.debug('%s using requirements\' target %s', req, t.fullname)
                 else:
                     with makefile.context:
-                        t = Package(req.name, req.version_spec, package=req.package, repository=req.repository, makefile=makefile)
-                    logger.debug('%s: adding package %s', req, t.fullname)
-                unresolved.append(req)
+                        t, is_new = Package.instance(req.name, req.version_spec, package=req.package, repository=req.repository, makefile=makefile.root)
+                    if is_new:
+                        logger.debug('%s: adding package %s', req, t.fullname)
+                    else:
+                        logger.debug('%s: package already beeing installed at version %s', req, t.version)
                 group.create_task(t.install(deps_settings, InstallMode.dev))
+                unresolved.append(req)
 
 
 
     if install:
         for req in unresolved:
             pkg = find_package(req.name, req.version_spec, search_paths=pkgs_search_paths, makefile=makefile)
             if pkg is None:
```

### Comparing `dan-build-0.2.4/dan/core/runners.py` & `dan-build-0.2.5/dan/core/runners.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/core/settings.py` & `dan-build-0.2.5/dan/core/settings.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/core/target.py` & `dan-build-0.2.5/dan/core/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             case type():
                 assert issubclass(dependency, Target)
                 self._content.append(self.makefile.find(dependency))
             case str():
                 from dan.pkgconfig.package import Package
                 for pkg in Package.all.values():
                     if pkg.name == dependency:
-                        self.append(pkg)
+                        self._content.append(pkg)
                         break
                 else:
                     if Path(self.parent.source_path / dependency).exists():
                         self._content.append(FileDependency(
                             self.parent.source_path / dependency))
                     else:
                         from dan.pkgconfig.package import parse_requirement
@@ -295,14 +295,18 @@
         self.diagnostics = diags.DiagnosticCollection()
 
     @property
     def output(self):
         if self._output is None:
             return None
         return self.build_path / self._output
+
+    @property
+    def routput(self):
+        return self._output
     
     @property
     def version(self):
         version = self._version
         if isinstance(version, Option):
             version = version.value
         if isinstance(version, str):
@@ -312,17 +316,20 @@
     @version.setter
     def version(self, value):
         self._version = value
 
     @output.setter
     def output(self, path):
         path = Path(path)
-        if path.is_absolute() and self.build_path in path.parents:
+        if not path.is_absolute() and self.build_path in path.parents:
             raise RuntimeError(f'output must not be an absolute path within build directory')
-        self._output = path
+        elif path.is_absolute() and self.build_path in path.parents:
+            self._output = path.relative_to(self.build_path)
+        else:
+            self._output = path
 
     @property
     def is_requirement(self) -> bool:
         return self.makefile.name.endswith('requirements')
 
     @property
     def source_path(self) -> Path:
@@ -390,15 +397,15 @@
         return res
 
     @property
     def modification_time(self):
         output = self.build_path / f'{self.name}.stamp' if self.output is None else self.output  
         return output.stat().st_mtime if output.exists() else 0.0
 
-    @property
+    @cached_property
     def up_to_date(self):
         output = self.build_path / f'{self.name}.stamp' if self.output is None else self.output
         if output and not output.exists():
             return False
         elif not self.dependencies.up_to_date:
             return False
         elif self.dependencies.modification_time > self.modification_time:
@@ -462,17 +469,20 @@
             for f in self.other_generated_files:
                 if f.exists():
                     group.create_task(aiofiles.os.remove(f))
             res = self.__clean__()
             if inspect.iscoroutine(res):
                 group.create_task(res)
 
-    @asyncio.cached
+    @asyncio.cached(unique = True)
     async def install(self, settings: InstallSettings, mode: InstallMode):
         await self.build()
+
+        self.debug('installing %s to %s', self.name, settings.destination)
+
         installed_files = list()
         if mode == InstallMode.dev:
             if len(self.utils) > 0:
                 lines = list()
                 for fn in self.utils:
                     tmp = inspect.getsourcelines(fn)[0]
                     tmp[0] = f'\n\n@self.utility\n'
```

### Comparing `dan-build-0.2.4/dan/core/test.py` & `dan-build-0.2.5/dan/core/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
         out = self.workingDir / f'{base}.stdout'
         err = self.workingDir / f'{base}.stderr'
         return out, err
 
     async def _run_test(self, caze: Case):
         name = f'{self.name}.{caze.name}' if caze is not None else self.name
         args = [str(a) for a in caze.args]
+        self.debug('testing %s', name)
         out, err, rc = await self.executable.execute(*args, no_raise=True, cwd=self.workingDir)
         out_log, out_err = self.outs(caze)
         async with aiofiles.open(out_log, 'w') as outlog, \
                 aiofiles.open(out_err, 'w') as errlog:
             async with asyncio.TaskGroup(f'writing {name} log files') as group:
                 group.create_task(outlog.write(out))
                 group.create_task(errlog.write(err))
@@ -120,14 +121,17 @@
                 out = out.strip()
                 err = err.strip()
                 msg = f'Test \'{name}\' failed (output: {out}, expected: {expected_output.strip()}) !'
                 raise RuntimeError(msg)
 
     async def run_test(self):
         try:
+            if len(self.cases) == 0:
+                self.error('%s contains no test case', self.name)
+                return False
             async with asyncio.TaskGroup(f'running {self.name} tests') as tests:
                 for caze in self.cases:
                     tests.create_task(self._run_test(caze))
         except asyncio.ExceptionGroup as errors:
             for err in errors.errors:
                 self.error(err)
             return False
```

### Comparing `dan-build-0.2.4/dan/core/utils.py` & `dan-build-0.2.5/dan/core/utils.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/core/version.py` & `dan-build-0.2.5/dan/core/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,19 +84,19 @@
 
     def __ge__(self, other: 'Version'):
         if isinstance(other, str):
             other = Version(other)
         elif not isinstance(other, Version):
             return False
         for mine, their in zip(self._parts, other._parts):
-            if mine >= their:
+            if mine > their:
                 return True
             if mine < their:
                 return False
-        return False
+        return True
     
     def __lt__(self, other: 'Version'):
         if isinstance(other, str):
             other = Version(other)
         elif not isinstance(other, Version):
             return False
         for mine, their in zip(self._parts, other._parts):
@@ -153,14 +153,16 @@
 
 
     def __init__(self, version: Version, op: str) -> None:
         self.version = version
         self.op = op
         
     def is_compatible(self, version: Version):
+        if isinstance(version, VersionSpec):
+            version = version.version
         match self.op:
             case '==':
                 return version == self.version
             case '=':
                 return version.is_compatible(self.version)
             case '>':
                 return version > self.version
```

### Comparing `dan-build-0.2.4/dan/core/win.py` & `dan-build-0.2.5/dan/core/win.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/cxx/__init__.py` & `dan-build-0.2.5/dan/cxx/__init__.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/cxx/compile_commands.py` & `dan-build-0.2.5/dan/cxx/compile_commands.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/cxx/detect.py` & `dan-build-0.2.5/dan/cxx/detect.py`

 * *Files 2% similar despite different names*

```diff
@@ -439,15 +439,15 @@
         logger.debug('looking for clang%s', logging.lazy_fmt(lambda: '' if paths is None else ' in' + ', '.join(paths)))
         for clang in find_executables(r'clang(-\d+)?(\.exe)?', paths, default_paths):
             clang = clang.resolve()
             compilers.add(Compiler(clang, logger=logger))
     return compilers
 
 unix_tools = [
-    'nm', 'ranlib', 'strip', 'readelf', 'ar', 'ranlib'
+    'nm', 'ranlib', 'strip', 'readelf', 'ar', 'ranlib', ('dbg', 'gdb')
 ]
 
 if os.name != 'nt':
     _required_tools = unix_tools
 else:
     _required_tools = list()
 
@@ -477,14 +477,16 @@
     data['arch'] = compiler.arch
     data['system'] = compiler.system
 
     if compiler.env:
         data['env'] = compiler.env
 
     def get_compiler_tool(tool, toolname=None):
+        if isinstance(tool, tuple):
+            tool, toolname = tool
         if not toolname:
             toolname = f'{base_name}-{tool}'
         if prefix:
             toolname = f'{prefix}{toolname}'
         if suffix:
             toolname = f'{toolname}{suffix}'
         tool_path = (base_path / toolname).with_suffix(extension)
@@ -492,16 +494,18 @@
             logger.debug(f'found {tool} tool: {tool_path}')
             data[tool] = str(tool_path)
         else:
             logger.debug(f'{tool} tool not found: {tool_path}')
     if compiler.name == 'gcc':
         get_compiler_tool('cxx', 'g++')
         get_compiler_tool('as')
+        get_compiler_tool('dbg', 'gdb')
     elif compiler.name == 'clang':
         get_compiler_tool('cxx', 'clang++')
+        get_compiler_tool('dbg', 'lldb')
     elif compiler.name == 'msvc':
         data['link'] = str(compiler.tools['link'])
         data['lib'] = str(compiler.tools['lib'])
 
     if compiler.compiler_id.is_unix:
         for tool in unix_tools:
             get_compiler_tool(tool)
@@ -612,15 +616,19 @@
             else:
                 logger.info(f'updating toolchain \'{k}\'')
         else:
             logger.info(f'toolchain \'{k}\' unchanged')
             continue
         toolchains[k] = v
     for tool in _required_tools:
-        tools[tool] = str(find_executable(tool, paths, default_paths))
+        if isinstance(tool, tuple):
+            tool, toolname = tool
+        else:
+            toolname = tool
+        tools[tool] = str(find_executable(toolname, paths, default_paths))
     data['tools'] = tools
     data['toolchains'] = toolchains
     if not 'default' in data:
         from dan.core.osinfo import OSInfo
         osi = OSInfo()
         default_toolchain = None
         for name, toolchain in toolchains.items():
```

### Comparing `dan-build-0.2.4/dan/cxx/msvc_toolchain.py` & `dan-build-0.2.5/dan/cxx/msvc_toolchain.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,25 +69,30 @@
         _, err, _ = sync_run([self.cxx, *opts], no_raise=True)
         # D9002 => unknown option
         return err.splitlines()[0].find('D9002') == 0
 
     def make_include_options(self, include_paths: set[Path]) -> list[str]:
         return [f'/I{p}' for p in include_paths]
 
-    def make_link_options(self, libraries: set[Path | str]) -> list[str]:
+    def make_libpath_options(self, libraries: set[Path | str]) -> list[str]:
         lib_paths = list()
-        libs = list()
         for lib in libraries:
             if isinstance(lib, Path):
                 lib_paths.append(f'/LIBPATH:{lib.parent}')
+        return lib_paths
+
+    def make_link_options(self, libraries: set[Path | str]) -> list[str]:
+        libs = list()
+        for lib in libraries:
+            if isinstance(lib, Path):
                 libs.append(f'{lib.stem}.lib')
             else:
                 assert isinstance(lib, str)
                 libs.append(f'{lib}.lib')
-        return [*libs, *lib_paths]
+        return libs
 
     def make_compile_definitions(self, definitions: set[str]) -> list[str]:
         return [f'/D{d}' for d in definitions]
 
     def make_library_name(self, basename: str, shared: bool) -> str:
         return f'{basename}.{"dll" if shared else "lib"}'
 
@@ -154,27 +159,19 @@
             args.append(f'/Fd{str(output.with_suffix(".pdb"))}')
         return [args]
 
     def make_link_commands(self, objects: set[Path], output: Path, options: list[str]) -> CommandArgsList:
         return [[self.lnk, *self.common_flags, *options, *objects, f'/OUT:{str(output)}']]
 
     def make_static_lib_commands(self, objects: set[Path], output: Path, options: list[str]) -> CommandArgsList:
-        objects = list(objects)
-        objs = [objects[0].name]
-        for obj in objects[1:]:
-            objs.append(obj.name)
-        return [[self.lib, *self.common_flags, *objs, f'/OUT:{output}']]
+        return [[self.lib, *self.common_flags, *objects, f'/OUT:{output}']]
 
     def make_shared_lib_commands(self, objects: set[Path], output: Path, options: list[str]) -> CommandArgsList:
-        objects = list(objects)
-        objs = [objects[0].name]
-        for obj in objects[1:]:
-            objs.append(obj.name)
         return [[self.lnk, *self.common_flags,
-                f'/IMPLIB:{output.with_suffix(".lib")}', '/DLL', *options, *objs, f'/OUT:{output.with_suffix(".dll")}']]
+                f'/IMPLIB:{output.with_suffix(".lib")}', '/DLL', *options, *objects, f'/OUT:{output.with_suffix(".dll")}']]
 
     async def _handle_compile_output(self, lines) -> t.Iterable[diag.Diagnostic]:
         async for line in lines:
             line = line.strip()
             match re_match(line):
                 case r'(.+)\((\d+)\):\s+(?:fatal\s+)?(error|warning)\s(\w+\d+):\s(.+)$' as m:
                     yield diag.Diagnostic(
```

### Comparing `dan-build-0.2.4/dan/cxx/support/qt.py` & `dan-build-0.2.5/dan/cxx/support/qt.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 from dan.cxx.targets import CXXObject, Executable, Library, CXXObjectsTarget
 from dan.pkgconfig.package import Package
 
 
 class _QtMoccer:
     
     async def __initialize__(self):
-        qt_core = Package('Qt5Core', makefile=self.makefile)
+        qt_core = Package(f'Qt{self.qt_major}Core', makefile=self.makefile)
         await qt_core.initialize()
         self.moc = self.makefile.cache.get('moc_executable')
         if not self.moc:
+            search_paths = [qt_core.host_bins if hasattr(qt_core, 'host_bins') else qt_core.bindir, qt_core.prefix]
             self.moc = find_executable(
-                'moc', paths=[qt_core.host_bins], default_paths=False)
+                'moc', paths=search_paths, default_paths=False)
             self.makefile.cache.moc_executable = str(self.moc)
         self.dependencies.add(qt_core)
 
         self.includes.private.append(self.build_path)
 
         for module in self.qt_modules:
-            pkg = Package(f'Qt5{module}', makefile=self.makefile)
+            pkg = Package(f'Qt{self.qt_major}{module}', makefile=self.makefile)
             await pkg.initialize()
             self.dependencies.add(pkg)
 
         self.mocs = self.cache.get('mocs', list())
         for moc_name in self.mocs:
             moc_path = self.build_path / moc_name
             self.objs.append(
@@ -81,15 +82,18 @@
         # update cache
         self.cache['mocs'] = self.mocs
 
         # continue parent build process
         await super().__build__()
 
 
-def moc(modules: list[str]):
+def moc(modules: list[str] = None, major=6):
+    if modules is None:
+        modules = ['Widgets']
     def decorator(cls):
         from dan.core.include import context
         @context.current.wraps(cls)
         class QtWapped(_QtMoccer, cls):
             qt_modules = modules
+            qt_major = major
         return cls
     return decorator
```

### Comparing `dan-build-0.2.4/dan/cxx/targets.py` & `dan-build-0.2.5/dan/cxx/targets.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,23 +9,34 @@
 from dan.core.pathlib import Path
 from dan.core import aiofiles, cache
 from dan.core.settings import InstallMode, InstallSettings
 from dan.core.target import Target
 from dan.core.utils import chunks, unique
 from dan.core.runners import async_run
 from dan.core import asyncio
-from dan.cxx.toolchain import CompilationFailure, LinkageFailure, Toolchain
+from dan.cxx.toolchain import CompilationFailure, LibraryList, LinkageFailure, Toolchain
 
 
 class CXXObject(Target, internal=True):
-    def __init__(self, source:Path, parent: 'CXXTarget') -> None:
-        super().__init__(source.stem, parent=parent, default=False)
+    def __init__(self, source:Path, parent: 'CXXTarget', root: Path = None) -> None:
+        if source.is_absolute():
+            if root is None:
+                root = parent.build_path
+            name = '-'.join(source.relative_to(root).with_suffix(f'').parts)
+        else:
+            name = '-'.join(source.with_suffix(f'').parts)
+        super().__init__(name, parent=parent, default=False)
         self.parent = parent
-        self.source = self.source_path / source
+        self.source = source
         self.toolchain: Toolchain = self.context.get('cxx_target_toolchain')
+        obj_fname = source.with_suffix('.obj' if self.toolchain.type == 'msvc' else '.o')
+        if source.is_absolute():
+            self.output = self.build_path / obj_fname.name
+        else:
+            self.output = self.build_path / obj_fname
         self.__dirty = False
 
     @property
     def cxx_flags(self):
         return self.parent.cxx_flags
 
     @property
@@ -39,55 +50,52 @@
     @property
     def compile_definitions(self):
         return self.parent.compile_definitions
 
     async def __initialize__(self):
         await self.parent.preload()
 
-        ext = 'o' if os.name != 'nt' else 'obj'
-        self.output: Path = Path(f'{self.source.stem}.{ext}')
-
         deps = self.cache.get('deps')
         if deps is not None:
             self.dependencies.update(deps)
 
         self.dependencies.add(self.source)
 
         self.other_generated_files.update(
             self.toolchain.compile_generated_files(self.output))
 
         previous_args = self.cache.get('compile_args')
         if previous_args:
             args = self.toolchain.make_compile_commands(
-                self.source, self.output, self.private_cxx_flags)[0]
+                self.source_path / self.source, self.output, self.private_cxx_flags)[0]
             args = [str(arg) for arg in args]
             if sorted(args) != sorted(previous_args):
                 self.__dirty = True
         else:
             self.__dirty = True
 
-    @property
+    @cached_property
     def up_to_date(self):
-        res = super().up_to_date
-        if res and self.__dirty:
-            res = False
-        return res
+        if self.__dirty:
+            return False
+        return super().up_to_date
 
     async def __build__(self):
         self.info('generating %s...', self.output.name)
         try:
-            commands, diags = await self.toolchain.compile(self.source, self.output, self.private_cxx_flags)
+            self.output.parent.mkdir(parents=True, exist_ok=True)
+            commands, diags = await self.toolchain.compile(self.source_path / self.source, self.output, self.private_cxx_flags)
             self.parent.diagnostics.insert(diags, str(self.source))
         except CompilationFailure as err:
             self.parent.diagnostics.insert(err.diags, str(self.source))
             err.target = self
             raise
         self.cache['compile_args'] = [str(a) for a in commands[0]]
         self.debug('scanning dependencies of %s', self.source.name)
-        deps = await self.toolchain.scan_dependencies(self.source, self.private_cxx_flags, self.build_path)
+        deps = await self.toolchain.scan_dependencies(self.source_path / self.source, self.private_cxx_flags, self.build_path)
         deps = [d for d in deps
                 if self.makefile.root.source_path in Path(d).parents
                 or self.build_path in Path(d).parents]
         self.cache['deps'] = deps
 
 
 class OptionSet:
@@ -148,25 +156,27 @@
                     self._private.append(value)
 
     def update(self, values: 'OptionSet', private=False):
         self._public = values._public
         if private:
             self._private = values._private
 
-
 class CXXTarget(Target, internal=True):
     public_includes: set[str] = set()
     private_includes: set[str] = set()
 
     public_compile_options: set[str] = set()
     private_compile_options: set[str] = set()
     
     public_compile_definitions: set[str] = set()
     private_compile_definitions: set[str] = set()
 
+    public_lib_paths: set[str] = set()
+    private_lib_paths: set[str] = set()
+
     public_link_libraries: set[str] = set()
     private_link_libraries: set[str] = set()
 
     public_link_options: set[str] = set()
     private_link_options: set[str] = set()
 
     def __init__(self,
@@ -180,14 +190,17 @@
                                   transform=self.toolchain.make_include_options)
 
         self.compile_options = OptionSet(self, 'compile_options',
                                          self.public_compile_options, self.private_compile_options)
 
         self.link_libraries = OptionSet(self, 'link_libraries',
                                         self.public_link_libraries, self.private_link_libraries, transform=self.toolchain.make_link_options)
+        
+        self.library_paths = OptionSet(self, 'library_paths',
+                                        self.public_lib_paths, self.private_lib_paths, transform=self.toolchain.make_libpath_options)
 
         self.compile_definitions = OptionSet(self, 'compile_definitions',
                                              self.public_compile_definitions, self.private_compile_definitions, transform=self.toolchain.make_compile_definitions)
 
         self.link_options = OptionSet(self, 'link_options',
                                       self.public_link_options, self.private_link_options)
 
@@ -206,23 +219,33 @@
     def cxx_dependencies(self) -> list['CXXTarget']:
         return [dep for dep in self.dependencies if isinstance(dep, CXXTarget)]
 
     @property
     def library_dependencies(self) -> list['Library']:
         return [dep for dep in self.dependencies if isinstance(dep, Library)]
 
-    @property
-    def libs(self) -> list[str]:
-        tmp = list()
-        tmp.extend(self.link_libraries.public)
-        # TODO move create private_libs()
-        tmp.extend(self.link_libraries.private)
+    @cached_property
+    def lib_paths(self) -> list[str]:
+        tmp = set()
         for dep in self.cxx_dependencies:
+            tmp.update(dep.lib_paths)
+        tmp.update(self.library_paths.public)
+        # # TODO move create private_libs()
+        tmp.update(self.library_paths.private)
+        return list(sorted(tmp))
+
+    @cached_property
+    def libs(self) -> LibraryList:
+        tmp = LibraryList()
+        for dep in reversed(self.cxx_dependencies):
             tmp.extend(dep.libs)
-        return unique(tmp)
+        tmp.extend(self.link_libraries.public)
+        # # TODO move create private_libs()
+        tmp.extend(self.link_libraries.private)
+        return tmp
 
     @cached_property
     def cxx_flags(self):
         flags = self.includes.public
         flags.extend(self.compile_options.public)
         flags.extend(self.compile_definitions.public)
         for dep in self.cxx_dependencies:
@@ -246,34 +269,37 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.objs: list[CXXObject] = list()
 
     @cache.once_method
     def _init_sources(self):
         if callable(self.sources):
-            self.sources = set(self.sources())
+            self.sources = list(self.sources())
         if not isinstance(self.sources, Iterable):
             assert callable(
                 self.sources), f'{self.name} sources parameter should be an iterable or a callable returning an iterable'
         sources = list()
+        source_root = Path(os.path.commonprefix(self.sources))
         for source in self.sources:
             source = Path(source)
-            if not source.is_absolute():
-                source = self.source_path / source
+            if source.is_absolute():
+                root = source_root
+            else:
+                root = self.source_path
             sources.append(source)
             self.objs.append(
-                CXXObject(Path(source), self))
+                CXXObject(Path(source), self, root=root))
         self.sources = sources
             
 
     @property
     def file_dependencies(self):
         return unique(super().file_dependencies, *[o.file_dependencies for o in self.objs])
     
-    @property
+    @cached_property
     def up_to_date(self):
         for obj in self.objs:
             if not obj.up_to_date:
                 return False
         return super().up_to_date
 
     @property
@@ -320,20 +346,31 @@
     def shared(self) -> bool:
         return self.library_type == LibraryType.SHARED
 
     @property
     def interface(self) -> bool:
         return self.library_type == LibraryType.INTERFACE
 
+    @cached_property
+    def lib_paths(self) -> list[str]:
+        tmp = super().lib_paths
+        if not self.interface:
+            tmp.extend(self.toolchain.make_libpath_options([self.output]))
+        return list(sorted(tmp))
+    
     @property
     def libs(self) -> list[str]:
-        tmp = super().libs
         if not self.interface:
-            tmp.extend(self.toolchain.make_link_options([self.output]))
-        return tmp
+            libs = LibraryList()
+            libs.extend(self.toolchain.make_link_options([self.output]))
+            libs.extend(super().libs)
+        else:
+            libs = super().libs
+        
+        return libs
 
     async def __initialize__(self):
         self._init_sources()
 
         if self.library_type == LibraryType.AUTO:
             if len(self.sources) == 0:
                 self.library_type = LibraryType.INTERFACE
@@ -356,37 +393,37 @@
             case LibraryType.STATIC:
                 generate = self.toolchain.static_lib
             case LibraryType.SHARED:
                 generate = self.toolchain.shared_lib
         if generate is not None:
             if previous_args and \
                     previous_args != await generate(
-                        [obj.output for obj in self.objs], self.output, self.libs, dry_run=True):
+                        [obj.routput for obj in self.objs], self.output, self.libs, dry_run=True):
                 self.__dirty = True
             else:
                 self.__dirty = False
         else:
             self.__dirty = False
 
-    @property
+    @cached_property
     def up_to_date(self):
         if self.__dirty:
             return False
         return super().up_to_date
 
     async def __build__(self):
         await super().__build__()
 
         self.info(
             'creating %s library %s...', self.library_type.name.lower(), self.output.name)
 
         if self.static:
-            await self.toolchain.static_lib([obj.output for obj in self.objs], self.output, self.libs)
+            await self.toolchain.static_lib([obj.routput for obj in self.objs], self.output, self.libs)
         elif self.shared:
-            await self.toolchain.shared_lib([obj.output for obj in self.objs], self.output, {*self.private_cxx_flags, *self.libs})
+            await self.toolchain.shared_lib([obj.routput for obj in self.objs], self.output, {*self.private_cxx_flags, *self.libs})
             from .msvc_toolchain import MSVCToolchain
             if isinstance(self.toolchain, MSVCToolchain):
                 self.compile_definitions.add(
                     f'{self.name.upper()}_IMPORT=1', public=True)
         else:
             assert self.interface
             self.output.touch()
@@ -466,34 +503,34 @@
         self.__dirty = False
 
     async def __initialize__(self):
         await super().__initialize__()
 
         previous_args = self.cache.get('link_args')
         if previous_args:
-            args = self.toolchain.make_link_commands([obj.output for obj in self.objs], self.output,
-                                                     [*self.libs, *self.link_options.public, *self.link_options.private])[0]
+            args = self.toolchain.make_link_commands([obj.routput for obj in self.objs], self.output,
+                                                     [*self.lib_paths, *self.libs, *self.link_options.public, *self.link_options.private])[0]
             args = [str(a) for a in args]
             if sorted(previous_args) != sorted(args):
                 self.__dirty = True
 
-    @property
+    @cached_property
     def up_to_date(self):
         if self.__dirty:
             return False
         return super().up_to_date
 
     async def __build__(self):
         await super().__build__()
 
         # link
         self.info('linking %s...', self.output.name)
         try:
-            commands, diags = await self.toolchain.link([obj.output for obj in self.objs], self.output,
-                                                        [*self.libs, *self.link_options.public, *self.link_options.private])
+            commands, diags = await self.toolchain.link([obj.routput for obj in self.objs], self.output,
+                                                        [*self.lib_paths, *self.libs, *self.link_options.public, *self.link_options.private])
             self.diagnostics.insert(diags, str(self.output))
         except LinkageFailure as err:
             self.diagnostics.insert(err.diags, str(self.output))
             err.target = self
             raise
         self.cache['link_args'] = [str(a) for a in commands[0]]
         self.debug('done')
```

### Comparing `dan-build-0.2.4/dan/cxx/toolchain.py` & `dan-build-0.2.5/dan/cxx/toolchain.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,37 @@
 CommandArgs = list[str|Path]
 CommandArgsList = list[CommandArgs]
 
 class RuntimeType(Enum):
     static = 0
     dynamic = 1
 
+class LibraryList:
+    def __init__(self, *items: t.Iterable):
+        self._lst = list()
+        self.extend(items)
+    
+    def add(self, item):
+        if not item in self._lst:
+            self._lst.insert(0, item)
+
+    def extend(self, items):
+        for item in items:
+            try:
+                self._lst.remove(item)
+            except ValueError:
+                pass
+        self._lst.extend(items)
+
+    def __iter__(self):
+        return iter(self._lst)
+    
+    def __reversed__(self):
+        return reversed(self._lst)
+
 
 class BaseFailure(RuntimeError):
     def __init__(self, msg: str, err: CommandError, options: set[str], command: str, toolchain: 'Toolchain', diags: list[diag.Diagnostic], target = None) -> None:
         super().__init__(msg)
         self.options = options
         self.command = command
         self.toolchain = toolchain
@@ -119,14 +142,17 @@
 
     def make_compile_definitions(self, definitions: set[str]) -> list[str]:
         raise NotImplementedError()
 
     def make_include_options(self, include_paths: set[Path]) -> list[str]:
         raise NotImplementedError()
 
+    def make_libpath_options(self, libraries: set[Path | str]) -> list[str]:
+        raise NotImplementedError()
+
     def make_link_options(self, libraries: set[Path]) -> list[str]:
         raise NotImplementedError()
 
     def make_library_name(self, basename: str, shared: bool) -> str:
         raise NotImplementedError()
 
     def make_executable_name(self, basename: str) -> str:
@@ -201,19 +227,19 @@
         for index, command in enumerate(commands):
             try:
                 await self.run(f'static_lib{index}', output, command, **kwds, cwd=output.parent)
             except CommandError as err:
                 raise LinkageFailure(err, objects, options, command, self) from None
         return commands
 
-    def make_static_lib_commands(self, objects: set[Path], output: Path, options: set[str]) -> CommandArgsList:
+    def make_shared_lib_commands(self, objects: set[Path], output: Path, options: set[str]) -> tuple[Path, CommandArgsList]:
         raise NotImplementedError()
 
     async def shared_lib(self, objects: set[Path], output: Path, options: set[str], **kwds):
-        commands = self.make_static_lib_commands(objects, output, options)
+        commands = self.make_shared_lib_commands(objects, output, options)
         for index, command in enumerate(commands):
             await self.run(f'shared_lib{index}', output, command, **kwds, cwd=output.parent)
         return commands
 
     async def run(self, name: str, output: Path, args, quiet=False, **kwds) -> tuple[str, str, int]:
         return await async_run(args, env={**(self.env or dict()), 'LC_ALL': 'C'}, logger=self if not quiet else None, **kwds)
```

### Comparing `dan-build-0.2.4/dan/cxx/unix_toolchain.py` & `dan-build-0.2.5/dan/cxx/unix_toolchain.py`

 * *Files 23% similar despite different names*

```diff
@@ -64,43 +64,49 @@
     def has_cxx_compile_options(self, *opts) -> bool:
         _, err, _ = sync_run([self.cxx, *opts], no_raise=True)
         return err.splitlines()[0].find('no input files') >= 0
 
     def make_include_options(self, include_paths: set[Path]) -> list[str]:
         return unique([f'-I{p}' for p in include_paths])
 
-    def make_link_options(self, libraries: set[Path | str]) -> list[str]:
+    def make_libpath_options(self, libraries: set[Path | str]) -> list[str]:
         opts = list()
         if self.rpath:
             opts.append(f'-Wl,-rpath,{self.rpath}')
 
         for lib in libraries:
             if isinstance(lib, Path):
                 opts.append(f'-L{lib.parent}')
                 if not self.rpath:
                     opts.append(f'-Wl,-rpath,{lib.parent}')
+        return opts
+
+    def make_link_options(self, libraries: set[Path | str]) -> list[str]:
+        opts = list()
+        for lib in libraries:
+            if isinstance(lib, Path):
                 opts.append(f'-l{lib.stem.removeprefix("lib")}')
             else:
                 assert isinstance(lib, str)
                 opts.append(f'-l{lib}')
-        return unique(opts)
+        return opts
 
     def make_compile_definitions(self, definitions: set[str]) -> list[str]:
         return unique([f'-D{d}' for d in definitions])
 
     def make_library_name(self, basename: str, shared: bool) -> str:
         return f'lib{basename}.{"so" if shared else "a"}'
 
     def make_executable_name(self, basename: str) -> str:
         return f'{basename}.exe' if self.system.startswith('msys') else basename
 
     def get_base_compile_args(self, sourcefile: Path) -> list[str]:
         match sourcefile.suffix:
             case _ if sourcefile.suffix in cxx_extensions:
-                return [self.cxx, *self.default_cxxflags]
+                return [self.cxx, *self.default_cxxflags, *self.default_cflags]
             case _ if sourcefile.suffix in c_extensions:
                 return [self.cc, *self.default_cflags]
             case _:
                 raise RuntimeError(
                     f'Unhandled source file extention: {sourcefile.suffix}')
 
     async def scan_dependencies(self, sourcefile: Path, options: list[str], build_path: Path) -> set[FileDependency]:
@@ -110,19 +116,22 @@
         if auto_fpic:
             args.insert(1, '-fPIC')
 
         build_path.mkdir(parents=True, exist_ok=True)
         output = build_path / sourcefile.name
         out, _, _ = await self.run('scan', output, args, log=False, cwd=build_path)
         if out:
-            all = ''.join([dep.replace('\\', ' ')
-                           for dep in out.splitlines()]).split()
-            _obj = all.pop(0)
-            _src = all.pop(0)
-            return all
+            all_deps = list()
+            for dep in out.splitlines():
+                if dep.endswith('\\'):
+                    dep = dep[:-2]
+                all_deps.append(dep.strip())
+            _obj = all_deps.pop(0)
+            _src = all_deps.pop(0)
+            return all_deps
         else:
             return set()
 
     def compile_generated_files(self, output: Path) -> set[Path]:
         return {output.with_suffix(output.suffix + '.d')}
 
     @property
@@ -134,28 +143,28 @@
         args.extend([*self.compile_options, *options, '-MD', '-MT', str(output),
                     '-MF', f'{output}.d', '-o', str(output), '-c', str(sourcefile)])
         if auto_fpic:
             args.insert(1, '-fPIC')
         return [args]
 
     def make_link_commands(self, objects: set[Path], output: Path, options: list[str]) -> CommandArgsList:
-        args = [self.cxx, *[o.name for o in objects], '-o', str(output), *unique(
+        args = [self.cxx, *objects, '-o', str(output), *unique(
             self.default_ldflags, self.default_cflags, self.default_cxxflags, self.link_options, options)]
         commands = [args]
         if self._build_type in [BuildType.release, BuildType.release_min_size]:
             commands.append([self.strip, output])
         return commands
 
     def make_static_lib_commands(self, objects: set[Path], output: Path, options: list[str]) -> CommandArgsList:
         return [
-            [self.ar, 'cr', output, *[o.name for o in objects]], # *options],
+            [self.ar, 'cr', output, *objects], # *options],
             [self.ranlib, output],
         ]
 
-    def make_shared_lib_commands(self, objects: set[Path], output: Path, options: list[str]) -> CommandArgsList:
+    def make_shared_lib_commands(self, objects: set[Path], output: Path, options: list[str]) -> tuple[Path, CommandArgsList]:
         args = [self.cxx, '-shared', *
                 unique(self.default_ldflags, options), *objects, '-o', output]
         commands = [args]
         if self._build_type in [BuildType.release, BuildType.release_min_size]:
             commands.append([self.strip, output])
         return commands
     
@@ -173,24 +182,77 @@
                 match re_match(line):
                     case r'^ (.+)$' as m:
                         includes.append(str(Path(m[1]).resolve()))
             self.cache[cache_key] = includes
         return includes
 
     async def _gen_gcc_compile_diags(self, lines) -> t.Iterable[diag.Diagnostic]:
+        _from = list()
+        prev: diag.Diagnostic|diag.RelatedInformation = None
+        prev_diag: diag.Diagnostic = None
         async for line in lines:
             match re_match(line):
-                case r'(.+):(\d+):(\d+):\s(error|warning):\s(.+)$' as m:
-                    yield diag.Diagnostic(
-                        message=m[5],
-                        range=diag.Range(start=diag.Position(line=int(m[2])-1, character=int(m[3]))),
+                case r'\s+?\|\s(\s+)?(\^~+)' as m:
+                    if prev is not None:
+                        if isinstance(prev, diag.Diagnostic):
+                            rng = prev.range
+                        else:
+                            rng = prev.location.range
+                        rng.start.character = len(m[1]) if m[1] else 0
+                        rng.end.character = rng.start.character + len(m[2])
+                case r'((?:.+)from (.+)):(\d+)[,:]' as m:
+                    message = m[1]
+                    if message.startswith('In file included'):
+                        _from.clear()
+                    filename = m[2]
+                    lineno = int(m[3]) - 1
+                    prev = info = diag.RelatedInformation(
+                        location=diag.Location(diag.Uri(filename),
+                        range=diag.Range(start=diag.Position(lineno), end=diag.Position(lineno))),
+                        message=message)
+                    _from.append(info)
+                case r'(.+?): In instantiation of \'(.+)\'' as m:
+                    _from.clear()
+                case r'(.+?):(\d+):(?:(\d+):)?\s+(required from\s.+)' as m:
+                    filename = m[1]
+                    lineno = int(m[2]) - 1
+                    character = int(m[3]) - 1 if m[3] else 0
+                    message = m[4]
+                    prev = info = diag.RelatedInformation(
+                        location=diag.Location(diag.Uri(filename),
+                        range=diag.Range(start=diag.Position(lineno, character), end=diag.Position(lineno, character))),
+                        message=message)
+                    _from.append(info)
+                case r'(.+?):(\d+):(?:(\d+):)?\s(note):\s(.+)$' as m:
+                    filename = m[1]
+                    character=int(m[3]) if m[3] else 0
+                    lineno = int(m[2]) - 1
+                    message=m[5]
+                    if prev_diag is None:
+                        self.warning('diagnostics: a note is expected to append after a diagnositc')
+                    else:
+                        info = diag.RelatedInformation(
+                            location=diag.Location(diag.Uri(filename),
+                            range=diag.Range(start=diag.Position(lineno, character), end=diag.Position(lineno, character))),
+                            message=message)
+                        prev_diag.related_information.insert(0, info)
+                        prev = info
+                case r'(.+?):(\d+):(?:(\d+):)?\s(?:fatal )?(error|warning):\s(.+)$' as m:
+                    character=int(m[3]) if m[3] else 0
+                    lineno = int(m[2]) - 1
+                    message=m[5]
+                    prev_diag = prev = diag.Diagnostic(
+                        message=message,
+                        range=diag.Range(start=diag.Position(line=lineno, character=character), end=diag.Position(line=lineno)),
                         severity=diag.Severity[m[4].upper()],
                         source=self.type,
-                        filename=m[1]
+                        filename=m[1],
+                        related_information=list(_from)
                     )
+                    yield prev_diag
 
     async def _handle_compile_output(self, lines) -> t.Iterable[diag.Diagnostic]:
         match self.type:
             case 'gcc'|'clang':
                 async for d in self._gen_gcc_compile_diags(lines):
                     yield d
             case _:
@@ -206,17 +268,27 @@
                     function = m[2]
                 case r'(?:.+: )?(?:(.+):)?\((.+)\+(.+)\): (.+)$' as m:
                     # link error may not be associated to a source file,
                     # in which case the associated file is the object
                     filename = m[1] or object
                     section = m[2]
                     section_offset = int(m[3], 0)
-                    message = m[4]
+                    message = m[4].strip()
+                    yield diag.Diagnostic(
+                        message=message,
+                        source=self.type
+                    )
+                case r'(?:.+?: )?(.+?):(\d+): (undefined reference to.+)$' as m:
+                    filename = m[1]
+                    line = int(m[2])
+                    message = m[3].strip()
                     yield diag.Diagnostic(
                         message=message,
+                        filename=filename,
+                        range=diag.Range(start=diag.Position(line=line)),
                         source=self.type
                     )
                 case _:
                     self._logger.debug('unhandled line: %s', line)
 
     async def _handle_link_output(self, lines) -> t.Iterable[diag.Diagnostic]:
         match self.type:
```

### Comparing `dan-build-0.2.4/dan/io/package.py` & `dan-build-0.2.5/dan/io/package.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 import os
 
 from dan.core import aiofiles, asyncio
 from dan.core.pathlib import Path
 from dan.core.settings import InstallMode, InstallSettings
 from dan.core.target import Target
-from dan.core.find import find_files
+from dan.core.find import find_file, find_files
 from dan.core.version import Version, VersionSpec
 from dan.io.repositories import get_packages_path, get_repo_instance
 
 
 class PackageBuild(Target, internal=True):
 
     _all_builds: dict[str, 'PackageBuild'] = dict()
     
     def __init__(self, name, version, package, repository, *args, spec: VersionSpec = None, **kwargs):
         self.spec = spec
-        super().__init__(name, *args, version=version, **kwargs)
+        self.pn = name
+        super().__init__(f'{name}-build', *args, version=version, **kwargs)
         self.package = name if package is None else package
         self.repo = get_repo_instance(repository, self.makefile)
         self.preload_dependencies.add(self.repo)
         self._package_makefile = None
         self._build_path = None
 
     @property
     def package_makefile(self):
         if self._package_makefile is None:
-            target = self.repo.find(self.name, self.package)
+            target = self.repo.find(self.pn, self.package)
             if target is None:
-                raise RuntimeError(f'cannot find {self.name} in {self.repo.name}')
-            self._package_makefile = self.repo.find(self.name, self.package).makefile
+                raise RuntimeError(f'cannot find {self.pn} in {self.repo.name}')
+            self._package_makefile = target.makefile
         return self._package_makefile
 
     def get_sources(self):
         makefile = self.package_makefile
         sources = None
         for target in makefile.all_targets:
             if 'source' in target.name:
                 sources = target
                 break
         if sources is None:
-            raise RuntimeError(f'Cannot find {self.name} pacakge\'s sources target')
+            raise RuntimeError(f'Cannot find {self.pn} package\'s sources target')
         return sources
 
     async def __initialize__(self):
         sources = self.get_sources()
         if self.spec is not None:
             avail_versions = await sources.available_versions()
             if avail_versions is None:
@@ -52,26 +53,30 @@
                 for version in avail_versions:
                     if self.spec.is_compatible(version):
                         self.debug(f'using version {version} to match {self.spec}')
                         self.version = version
                         break
 
         packages_path = get_packages_path()
-        
+        makefile = self.package_makefile
+
+        # set package version
+        version_option = makefile.options.get('version')
+        if self.version is None:
+            self.version = Version(version_option.value)
+        else:
+            version_option.value = str(self.version)
+
         toolchain = self.context.get('cxx_target_toolchain')
         self._build_path = packages_path / toolchain.system / toolchain.arch / toolchain.build_type.name / self.package / str(self.version)
         self.install_settings = InstallSettings(self.build_path)
         
         # update package build-path
-        makefile = self.package_makefile
         makefile.build_path = self.build_path / 'build'
 
-        # set package version
-        if self.version:
-            makefile.options.get('version').value = str(self.version)
 
         # set our output to the last installed package
         # TODO handle multiple outputs, then set our outputs to all installed packages
         pkg_name = makefile.all_installed[-1].name     
         self.output = Path(self.install_settings.libraries_prefix) / 'pkgconfig' / f'{pkg_name}.pc'
         sources.output = self.build_path / 'src' # TODO source_prefix in install settings
 
@@ -114,26 +119,42 @@
             if toolchain is not None and not toolchain.build_type.is_debug_mode:
                 group.create_task(aiofiles.rmtree(self.output / 'src'))
             group.create_task(aiofiles.rmtree(build_path, force=True))
 
 
 class Package(Target, internal=True):
 
+    __all: dict[str, 'Package'] = dict()
+
     def __init__(self,
                  name: str = None,
                  version: str = None,
                  package: str = None,
                  repository: str = None, **kwargs) -> None:
         self.package = package
         self.repository = repository
         if version is not None:
             self.version = version
         if name is not None:
             self.name = name
         super().__init__(**kwargs)
+        if self.name in self.__all:
+            raise RuntimeError(f'duplicate package: {self.name}')
+        self.__all[self.name] = self
+
+    @classmethod
+    def instance(cls, name, version, *args, **kwargs):
+        if name in cls.__all:
+            pkg = cls.__all[name]
+            if not version.is_compatible(pkg.version):
+                raise RuntimeError(f'incompatible package version: {pkg.version} {version}')
+            return pkg, False
+        else:
+            return Package(name, version, *args, **kwargs), True
+
     
     async def __initialize__(self):
 
         match self.version:
             case str():
                 _name, spec = VersionSpec.parse(self.version)
                 if _name is not None:
@@ -178,11 +199,15 @@
         
         if self.output.exists():
             from dan.pkgconfig.package import Data, find_package
             data = Data(self.output)
             async with asyncio.TaskGroup(f'importing {self.name} package requirements') as group:
                 toolchain = self.context.get('cxx_target_toolchain')
                 search_path = get_packages_path() / toolchain.system / toolchain.arch / toolchain.build_type.name
+                dest = self.build_path / self.pkgconfig_path
                 for pkg in data.requires:
-                    pkg = find_package(pkg.name, spec=pkg.version_spec, search_paths=[search_path], makefile=self.makefile)
-                    self.debug('copying %s to %s', pkg.config_path, self.build_path / self.pkgconfig_path)
-                    group.create_task(aiofiles.copy(pkg.config_path, self.build_path / self.pkgconfig_path))
+                    pkgconfig_file = find_file(rf'{pkg.name}.pc$', [search_path])
+                    # NOTE: find_package will resolve to the build-directory installed pkgconfig, wich will result in a failure
+                    # pkg = find_package(pkg.name, spec=pkg.version_spec, search_paths=[search_path], makefile=self.makefile)
+                    if pkgconfig_file is not None and not (dest / pkgconfig_file.name).exists():
+                        self.debug('copying %s to %s', pkgconfig_file, dest)
+                        group.create_task(aiofiles.copy(pkgconfig_file, dest))
```

### Comparing `dan-build-0.2.4/dan/io/repositories.py` & `dan-build-0.2.5/dan/io/repositories.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/jinja.py` & `dan-build-0.2.5/dan/jinja.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/logging.py` & `dan-build-0.2.5/dan/logging.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/make.py` & `dan-build-0.2.5/dan/make.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,25 +243,32 @@
         return items
 
     @functools.cached_property
     def tests(self) -> list[Test]:
         items = list()
         if self.required_targets and len(self.required_targets) > 0:
             for required in self.required_targets:
-                test_name, *test_case = required.split(':')
-                test_case = test_case[0] if len(test_case) else None
+                pos = required.find(':')
+                if pos > 0:
+                    test_name = required[:pos]
+                    test_case = required[pos+1:]
+                else:
+                    test_name = required
+                    test_case = None
 
                 for test in self.root.all_tests:
                     
                     if fnmatch.fnmatch(test.fullname, f'*{test_name}*'):
                         if len(test) > 1 and test_case is not None:
                             cases = list()
                             for case in test.cases:
                                 if fnmatch.fnmatch(case.name, test_case):
                                     cases.append(case)
+                            if len(cases) == 0:
+                                self.warning('couldn\'t find any test case in %s matching \'%s\'', test.name, test_case)
                             test.cases = cases
                         
                         items.append(test)
         else:
             for test in self.root.all_tests:
                 items.append(test)
         return items
@@ -540,16 +547,21 @@
             return await t.run_test()
         except Exception as err:
             self._diagnostics.update(gen_python_diags(err))
             raise
 
     async def test(self):
         await self.initialize()
+        tests = self.tests
+        if len(tests) == 0:
+            self.error('No test selected')
+            return 255
+
         with self.context:
-            with self.progress('testing', self.tests, self._test_target, self.no_progress) as tasks:
+            with self.progress('testing', tests, self._test_target, self.no_progress) as tasks:
                 results = await asyncio.gather(*tasks)
                 if all(results):
                     self.info('Success !')
                     return 0
                 else:
                     self.error('Failed !')
                     return 255
```

### Comparing `dan-build-0.2.4/dan/pkgconfig/package.py` & `dan-build-0.2.5/dan/pkgconfig/package.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 import jinja2
 from dan.core import aiofiles, asyncio
 from dan.core.pathlib import Path
 import re
 import importlib.util
 
 from dan.core.find import find_file, find_files, library_paths_lookup
+from dan.core.pm import re_match
 from dan.core.requirements import RequiredPackage, parse_requirement
 from dan.core.runners import cmdline2list
 from dan.core.settings import InstallMode, InstallSettings
 from dan.core.utils import unique
 from dan.core.version import Version, VersionSpec
 from dan.cxx.targets import CXXTarget, Library
+from dan.cxx.toolchain import LibraryList
 
 import typing as t
 
 
 class MissingPackage(RuntimeError):
     def __init__(self, name) -> None:
         super().__init__(f'package {name} not found')
@@ -114,28 +116,30 @@
         else:
             self.config_path = config_path or find_pkg_config(name, search_paths)
             self.data: Data = None
         self.search_paths = search_paths
         if not self.config_path:
             raise MissingPackage(name)
         self.search_paths.insert(0, self.config_path.parent)
+        self.pn = name
         self.all[name] = self
 
-        super().__init__(name, **kwargs)
+        super().__init__(f'{name}-pkgconfig', **kwargs)
 
         dan_plugin = self.config_path.parent.parent / \
-            'dan' / f'{self.name}.py'
+            'dan' / f'{name}.py'
         if dan_plugin.exists():
             spec = importlib.util.spec_from_file_location(
-                f'{self.name}_plugin', dan_plugin)
+                f'{name}_plugin', dan_plugin)
             module = importlib.util.module_from_spec(spec)
             setattr(module, 'self', self)
             spec.loader.exec_module(module)
         self.__cflags = None
         self.__libs = None
+        self.__lib_paths = None
         if not data:
             self.data = Data(self.config_path)
 
 
         self.version = self.data.version
 
     @property
@@ -152,14 +156,16 @@
         if reqs:
             async with asyncio.TaskGroup(f'resolving {self.name}\'s requirements') as group:
                 for req in reqs:
                     if req.name in self.all and req.is_compatible(self.all[req.name]):
                         dep = self.all[req.name]
                     else:
                         dep = find_package(req.name, req.version_spec, search_paths=self.search_paths, makefile=self.makefile)
+                    if dep is None:
+                        raise RuntimeError(f'Unresolved requirement: {req}')
                     group.create_task(dep.initialize())
                     deps.add(dep)
         self.includes.public.append(self.data.get('includedir'))
         self.dependencies.update(deps)
 
     @property
     def cxx_flags(self):
@@ -175,26 +181,48 @@
             self.__cflags = unique(cflags)
         return self.__cflags
 
     @property
     def package_dependencies(self):
         return [pkg for pkg in self.dependencies if isinstance(pkg, Package)]
 
+    def __init_libs(self):
+        self.__libs = LibraryList()
+        self.__lib_paths = set()
+        libs = self.data.get('libs')
+        if libs is not None:
+            libs = cmdline2list(libs)
+            libs = self.toolchain.from_unix_flags(libs)
+            for l in libs:
+                match re_match(l):
+                    case r'-l(.+)' as m:
+                        self.__libs.add(m[0])
+                    case r'-L(.+)' as m:
+                        self.__lib_paths.add(m[0])
+                    case r'/LIBPATH:(.+)' as m:
+                        self.__lib_paths.add(m[0])
+                    case r'-Wl,-rpath,(.+)' as m:
+                        self.__lib_paths.add(m[0])
+                    case _:
+                        self.__libs.add(l)
+        for pkg in self.package_dependencies:
+            self.__lib_paths.update(pkg.lib_paths)
+            self.__libs.extend(pkg.libs)
+        self.__lib_paths = list(sorted(self.__lib_paths))
+
+    @property
+    def lib_paths(self) -> list[str]:
+        if self.__lib_paths is None:
+            self.__init_libs()
+        return self.__lib_paths
+    
     @property
     def libs(self):
         if self.__libs is None:
-            tmp = list()
-            libs = self.data.get('libs')
-            if libs is not None:
-                libs = cmdline2list(libs)
-                libs = self.toolchain.from_unix_flags(libs)
-                tmp.extend(libs)
-            for pkg in self.package_dependencies:
-                tmp.extend(pkg.libs)
-            self.__libs = unique(tmp)
+            self.__init_libs()
         return self.__libs
 
     @asyncio.cached
     async def install(self, settings: InstallSettings, mode: InstallMode) -> list[Path]:
         settings = deepcopy(settings)
         settings.create_pkg_config = False
         return await super().install(settings, mode)
@@ -214,14 +242,20 @@
         return value
 
 
 _jinja_env: jinja2.Environment = None
 
 
 def find_package(name, spec: VersionSpec = None, search_paths: list = None, makefile = None):
+    
+    if name in Package.all:
+        pkg = Package.all[name]
+        if spec and not spec.is_compatible(pkg.version):
+            raise RuntimeError(f'incompatible package {name} ({pkg.version} {spec})')
+        return pkg
     if makefile is None:
         from dan.core.include import context
         makefile = context.current
     search_paths = search_paths or makefile.pkgs_path
     for config in find_pkg_configs(name, search_paths):
         if spec is not None:
             data = Data(config)
@@ -240,22 +274,31 @@
 
 
 async def create_pkg_config(lib: Library, settings: InstallSettings) -> Path:
     dest = settings.libraries_destination / 'pkgconfig' / f'{lib.name}.pc'
     lib.info(f'creating pkgconfig: {dest}')
 
     requires = list()
-    for req in lib.requires:
-        if req.version_spec:
-            requires.append(f'{req.name} {req.version_spec.op} {req.version_spec.version}')
-        else:
-            requires.append(req.name)
+    for dep in lib.dependencies:
+        match dep:
+            case RequiredPackage():
+                if dep.version_spec:
+                    requires.append(f'{dep.name} {dep.version_spec.op} {dep.version_spec.version}')
+                else:
+                    requires.append(dep.name)
+            case Library():
+                requires.append(dep.name)
+
 
-    libs = lib.toolchain.make_link_options(
-        [Path(f'${{libdir}}/{lib.name}')]) if not lib.interface else []
+    libs = list()
+    if not lib.interface:
+        libs.extend(lib.toolchain.make_libpath_options(
+            [Path(f'${{libdir}}/{lib.name}')]))
+        libs.extend(lib.toolchain.make_link_options(
+            [Path(f'${{libdir}}/{lib.name}')]))
     libs.extend(lib.link_libraries.public)
     libs.extend(lib.link_options.public)
     libs = lib.toolchain.to_unix_flags(libs)
 
     cflags = lib.compile_definitions.public
     cflags.extend(lib.toolchain.make_include_options(['${includedir}']))
     cflags = lib.toolchain.to_unix_flags(cflags)
```

### Comparing `dan-build-0.2.4/dan/src/git.py` & `dan-build-0.2.5/dan/src/git.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan/src/github.py` & `dan-build-0.2.5/dan/src/github.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,64 +5,87 @@
 from dan.core import asyncio
 from dan.src.tar import TarSources
 
 class GitHubReleaseSources(TarSources, internal=True):
 
     user : str
     project : str
+    use_tags = False
 
     @property
     def url(self):
         return self._url
 
     def __init__(self, *args, **kwargs):
         if self.name is None:
             self.name = f'{self.user}-{self.project}-sources'
         super().__init__(*args, **kwargs)
 
     async def __initialize__(self):
         await super().__initialize__()
 
         self._url = self.cache.get('url')
+        if self._url is not None and self.version is not None:
+            prev_version = self.cache.get('version')
+            if prev_version is not None and prev_version != self.version:
+                self._url = None
+            
         if self._url is None:
             avail_versions = await self.available_versions()
             if self.version is None:
                 self.version = sorted(avail_versions, reverse=True)[0]
             version = self.version if isinstance(self.version, Version) else Version(self.version)
             release = avail_versions[version]
-            assets = release['assets']
-            # prefer assets over tarball, asset might contain submodules while tarballs will not
-            for asset in assets:
-                if asset['content_type'] in ('application/zip', 'application/gzip'):
-                    self._url = asset['browser_download_url']
-                    break
-            else:
+            if self.use_tags:
                 if 'tarball_url' in release:
                     self._url = release['tarball_url']
+            else:
+                assets = release['assets']
+                # prefer assets over tarball, asset might contain submodules while tarballs will not
+                for asset in assets:
+                    if asset['content_type'] in ('application/zip', 'application/gzip'):
+                        self._url = asset['browser_download_url']
+                        break
+                else:
+                    if 'tarball_url' in release:
+                        self._url = release['tarball_url']
             if self._url is None:
                 raise RuntimeError(f'cannot resolve url of {self.name}')
+            self.cache['version'] = self.version
             self.cache['url'] = self._url
 
     @asyncio.cached
     async def available_versions(self) -> dict[Version, dict]:
         self.info('fetching github releases')
 
 
         api_token = None
 
         from dan.io.repositories import _get_settings
         settings = _get_settings()
         if settings.github.api_token is not None:
             api_token = settings.github.api_token
 
-        url = f'https://api.github.com/repos/{self.user}/{self.project}/releases'
-        async with aiohttp.ClientSession() as session:
-            if api_token is not None:
-                session.headers['Authorization'] = f'Bearer {api_token}'
-            async with session.get(url) as resp:
-                data = await resp.read()
-                if resp.status != 200:
-                    raise RuntimeError(f'unable to fetch {url}: {data.decode()}')
-                releases = json.loads(data)
-                return {Version(release['tag_name']): release for release in releases}
+        if self.use_tags:
+            url = f'https://api.github.com/repos/{self.user}/{self.project}/tags'
+            async with aiohttp.ClientSession() as session:
+                if api_token is not None:
+                    session.headers['Authorization'] = f'Bearer {api_token}'
+                async with session.get(url) as resp:
+                    data = await resp.read()
+                    if resp.status != 200:
+                        raise RuntimeError(f'unable to fetch {url}: {data.decode()}')
+                    releases = json.loads(data)
+                    return {Version(release['name']): release for release in releases}
+        else:
+            url = f'https://api.github.com/repos/{self.user}/{self.project}/releases'
+            async with aiohttp.ClientSession() as session:
+                if api_token is not None:
+                    session.headers['Authorization'] = f'Bearer {api_token}'
+                async with session.get(url) as resp:
+                    data = await resp.read()
+                    if resp.status != 200:
+                        raise RuntimeError(f'unable to fetch {url}: {data.decode()}')
+                    releases = json.loads(data)
+                    return {Version(release['tag_name']): release for release in releases}
```

### Comparing `dan-build-0.2.4/dan/src/tar.py` & `dan-build-0.2.5/dan/src/tar.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/dan_build.egg-info/PKG-INFO` & `dan-build-0.2.5/dan_build.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dan-build
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python-based build system.
 Author-email: Garcia Sylvain <garcia.6l20@gmail.com>, garcia.6l20@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Sylvain Garcia
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dan-build-0.2.4/dan_build.egg-info/SOURCES.txt` & `dan-build-0.2.5/dan_build.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/pyproject.toml` & `dan-build-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/tests/test_cxx_errors.py` & `dan-build-0.2.5/tests/test_cxx_errors.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/tests/test_cxx_libraries.py` & `dan-build-0.2.5/tests/test_cxx_libraries.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/tests/test_cxx_simple.py` & `dan-build-0.2.5/tests/test_cxx_simple.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/tests/test_cxx_src_catch2.py` & `dan-build-0.2.5/tests/test_cxx_src_catch2.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.4/tests/test_python_errors.py` & `dan-build-0.2.5/tests/test_python_errors.py`

 * *Files identical despite different names*

