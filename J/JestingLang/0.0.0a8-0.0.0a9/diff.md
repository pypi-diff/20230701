# Comparing `tmp/JestingLang-0.0.0a8.tar.gz` & `tmp/JestingLang-0.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JestingLang-0.0.0a8.tar", last modified: Thu Jun 29 09:19:51 2023, max compression
+gzip compressed data, was "JestingLang-0.0.0a9.tar", last modified: Thu Jun 29 13:16:15 2023, max compression
```

## Comparing `JestingLang-0.0.0a8.tar` & `JestingLang-0.0.0a9.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:51.046224 JestingLang-0.0.0a8/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1085 2023-05-09 15:44:29.000000 JestingLang-0.0.0a8/LICENSE
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      937 2023-06-29 09:19:51.047254 JestingLang-0.0.0a8/PKG-INFO
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     5263 2023-06-29 09:14:50.000000 JestingLang-0.0.0a8/README.md
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      103 2023-06-29 09:19:51.056241 JestingLang-0.0.0a8/setup.cfg
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1564 2023-06-29 09:14:58.000000 JestingLang-0.0.0a8/setup.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:49.108373 JestingLang-0.0.0a8/src/
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:49.432034 JestingLang-0.0.0a8/src/JestingLang/
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:49.650813 JestingLang-0.0.0a8/src/JestingLang/Core/
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:49.904025 JestingLang-0.0.0a8/src/JestingLang/Core/JDereferencer/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      338 2023-06-17 12:27:43.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JDereferencer/AbstractDereferencer.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2027 2023-06-27 11:59:14.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JDereferencer/CachedCellDereferencer.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1097 2023-06-17 13:10:33.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JDereferencer/CachedDereferencer.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1311 2023-06-17 13:10:33.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JDereferencer/KeyValueDereferencer.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:20:09.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JDereferencer/__init__.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:50.004673 JestingLang-0.0.0a8/src/JestingLang/Core/JParsing/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     4813 2023-06-29 07:06:24.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JParsing/JestingAST.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-25 16:59:49.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JParsing/__init__.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:50.258545 JestingLang-0.0.0a8/src/JestingLang/Core/JVisitors/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1561 2023-06-29 00:03:40.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JVisitors/AbstractJestingVisitor.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1528 2023-06-19 14:48:18.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JVisitors/ContextBoundInterpreterVisitor.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     3014 2023-06-24 03:02:41.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JVisitors/ContextfreeInterpreterVisitor.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2593 2023-06-17 13:10:33.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JVisitors/PrettyPrintingVisitors.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:17:36.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JVisitors/__init__.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-17 12:31:05.000000 JestingLang-0.0.0a8/src/JestingLang/Core/__init__.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:50.302727 JestingLang-0.0.0a8/src/JestingLang/JestingScript/
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:50.400545 JestingLang-0.0.0a8/src/JestingLang/JestingScript/JDereferencer/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     6024 2023-06-29 05:30:35.000000 JestingLang-0.0.0a8/src/JestingLang/JestingScript/JDereferencer/ScriptDereferencer.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:20:09.000000 JestingLang-0.0.0a8/src/JestingLang/JestingScript/JDereferencer/__init__.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:50.502179 JestingLang-0.0.0a8/src/JestingLang/JestingScript/JParsing/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2419 2023-06-29 06:38:18.000000 JestingLang-0.0.0a8/src/JestingLang/JestingScript/JParsing/JestingScriptAST.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-25 16:59:49.000000 JestingLang-0.0.0a8/src/JestingLang/JestingScript/JParsing/__init__.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:50.601722 JestingLang-0.0.0a8/src/JestingLang/JestingScript/JVisitors/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     3242 2023-06-29 06:38:18.000000 JestingLang-0.0.0a8/src/JestingLang/JestingScript/JVisitors/ScriptInterpreterVisitor.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:17:36.000000 JestingLang-0.0.0a8/src/JestingLang/JestingScript/JVisitors/__init__.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-17 13:09:13.000000 JestingLang-0.0.0a8/src/JestingLang/JestingScript/__init__.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)    16076 2023-06-29 09:04:57.000000 JestingLang-0.0.0a8/src/JestingLang/LexerParser.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)    14904 2023-06-29 07:06:25.000000 JestingLang-0.0.0a8/src/JestingLang/LexerParser_cachedParseTable.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:50.645722 JestingLang-0.0.0a8/src/JestingLang/Misc/
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:50.799425 JestingLang-0.0.0a8/src/JestingLang/Misc/JLogic/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2391 2023-06-28 12:22:45.000000 JestingLang-0.0.0a8/src/JestingLang/Misc/JLogic/LogicFunctions.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     3540 2023-06-29 07:03:12.000000 JestingLang-0.0.0a8/src/JestingLang/Misc/JLogic/OperationMapping.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 06:01:19.000000 JestingLang-0.0.0a8/src/JestingLang/Misc/JLogic/__init__.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:51.005069 JestingLang-0.0.0a8/src/JestingLang/Misc/JTesting/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      688 2023-06-17 13:17:53.000000 JestingLang-0.0.0a8/src/JestingLang/Misc/JTesting/DereferencerHelper.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      349 2023-06-18 00:00:43.000000 JestingLang-0.0.0a8/src/JestingLang/Misc/JTesting/LexerParserHelpers.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      342 2023-06-27 11:06:51.000000 JestingLang-0.0.0a8/src/JestingLang/Misc/JTesting/NonFileExternalFileLoader.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-22 14:14:47.000000 JestingLang-0.0.0a8/src/JestingLang/Misc/JTesting/__init__.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-22 12:31:24.000000 JestingLang-0.0.0a8/src/JestingLang/Misc/__init__.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 06:05:46.000000 JestingLang-0.0.0a8/src/JestingLang/__init__.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     3037 2023-06-17 13:52:56.000000 JestingLang-0.0.0a8/src/JestingLang/main.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:49.610886 JestingLang-0.0.0a8/src/JestingLang.egg-info/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      937 2023-06-29 09:19:48.000000 JestingLang-0.0.0a8/src/JestingLang.egg-info/PKG-INFO
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1815 2023-06-29 09:19:49.000000 JestingLang-0.0.0a8/src/JestingLang.egg-info/SOURCES.txt
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        1 2023-06-29 09:19:48.000000 JestingLang-0.0.0a8/src/JestingLang.egg-info/dependency_links.txt
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        4 2023-06-29 09:19:48.000000 JestingLang-0.0.0a8/src/JestingLang.egg-info/requires.txt
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)       12 2023-06-29 09:19:48.000000 JestingLang-0.0.0a8/src/JestingLang.egg-info/top_level.txt
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 13:16:15.210217 JestingLang-0.0.0a9/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1085 2023-05-09 15:44:29.000000 JestingLang-0.0.0a9/LICENSE
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      937 2023-06-29 13:16:15.210217 JestingLang-0.0.0a9/PKG-INFO
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     5263 2023-06-29 09:14:50.000000 JestingLang-0.0.0a9/README.md
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      103 2023-06-29 13:16:15.228371 JestingLang-0.0.0a9/setup.cfg
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1564 2023-06-29 13:15:25.000000 JestingLang-0.0.0a9/setup.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 13:16:13.515204 JestingLang-0.0.0a9/src/
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 13:16:13.784747 JestingLang-0.0.0a9/src/JestingLang/
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 13:16:13.976179 JestingLang-0.0.0a9/src/JestingLang/Core/
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 13:16:14.199844 JestingLang-0.0.0a9/src/JestingLang/Core/JDereferencer/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      338 2023-06-17 12:27:43.000000 JestingLang-0.0.0a9/src/JestingLang/Core/JDereferencer/AbstractDereferencer.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2027 2023-06-27 11:59:14.000000 JestingLang-0.0.0a9/src/JestingLang/Core/JDereferencer/CachedCellDereferencer.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1097 2023-06-17 13:10:33.000000 JestingLang-0.0.0a9/src/JestingLang/Core/JDereferencer/CachedDereferencer.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1311 2023-06-17 13:10:33.000000 JestingLang-0.0.0a9/src/JestingLang/Core/JDereferencer/KeyValueDereferencer.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:20:09.000000 JestingLang-0.0.0a9/src/JestingLang/Core/JDereferencer/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 13:16:14.282186 JestingLang-0.0.0a9/src/JestingLang/Core/JParsing/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     4813 2023-06-29 07:06:24.000000 JestingLang-0.0.0a9/src/JestingLang/Core/JParsing/JestingAST.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-25 16:59:49.000000 JestingLang-0.0.0a9/src/JestingLang/Core/JParsing/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 13:16:14.536265 JestingLang-0.0.0a9/src/JestingLang/Core/JVisitors/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1561 2023-06-29 00:03:40.000000 JestingLang-0.0.0a9/src/JestingLang/Core/JVisitors/AbstractJestingVisitor.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1528 2023-06-19 14:48:18.000000 JestingLang-0.0.0a9/src/JestingLang/Core/JVisitors/ContextBoundInterpreterVisitor.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     3014 2023-06-24 03:02:41.000000 JestingLang-0.0.0a9/src/JestingLang/Core/JVisitors/ContextfreeInterpreterVisitor.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2593 2023-06-17 13:10:33.000000 JestingLang-0.0.0a9/src/JestingLang/Core/JVisitors/PrettyPrintingVisitors.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1273 2023-06-29 13:13:55.000000 JestingLang-0.0.0a9/src/JestingLang/Core/JVisitors/ReferencesListerVisitor.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:17:36.000000 JestingLang-0.0.0a9/src/JestingLang/Core/JVisitors/__init__.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-17 12:31:05.000000 JestingLang-0.0.0a9/src/JestingLang/Core/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 13:16:14.585372 JestingLang-0.0.0a9/src/JestingLang/JestingScript/
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 13:16:14.663340 JestingLang-0.0.0a9/src/JestingLang/JestingScript/JDereferencer/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     6024 2023-06-29 05:30:35.000000 JestingLang-0.0.0a9/src/JestingLang/JestingScript/JDereferencer/ScriptDereferencer.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:20:09.000000 JestingLang-0.0.0a9/src/JestingLang/JestingScript/JDereferencer/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 13:16:14.752167 JestingLang-0.0.0a9/src/JestingLang/JestingScript/JParsing/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2419 2023-06-29 06:38:18.000000 JestingLang-0.0.0a9/src/JestingLang/JestingScript/JParsing/JestingScriptAST.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-25 16:59:49.000000 JestingLang-0.0.0a9/src/JestingLang/JestingScript/JParsing/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 13:16:14.843196 JestingLang-0.0.0a9/src/JestingLang/JestingScript/JVisitors/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     3242 2023-06-29 06:38:18.000000 JestingLang-0.0.0a9/src/JestingLang/JestingScript/JVisitors/ScriptInterpreterVisitor.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:17:36.000000 JestingLang-0.0.0a9/src/JestingLang/JestingScript/JVisitors/__init__.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-17 13:09:13.000000 JestingLang-0.0.0a9/src/JestingLang/JestingScript/__init__.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)    16076 2023-06-29 09:04:57.000000 JestingLang-0.0.0a9/src/JestingLang/LexerParser.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)    11304 2023-06-29 13:10:13.000000 JestingLang-0.0.0a9/src/JestingLang/LexerParser_cachedParseTable.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 13:16:14.873012 JestingLang-0.0.0a9/src/JestingLang/Misc/
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 13:16:15.009935 JestingLang-0.0.0a9/src/JestingLang/Misc/JLogic/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2391 2023-06-28 12:22:45.000000 JestingLang-0.0.0a9/src/JestingLang/Misc/JLogic/LogicFunctions.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     3540 2023-06-29 07:03:12.000000 JestingLang-0.0.0a9/src/JestingLang/Misc/JLogic/OperationMapping.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 06:01:19.000000 JestingLang-0.0.0a9/src/JestingLang/Misc/JLogic/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 13:16:15.175845 JestingLang-0.0.0a9/src/JestingLang/Misc/JTesting/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      688 2023-06-17 13:17:53.000000 JestingLang-0.0.0a9/src/JestingLang/Misc/JTesting/DereferencerHelper.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      349 2023-06-18 00:00:43.000000 JestingLang-0.0.0a9/src/JestingLang/Misc/JTesting/LexerParserHelpers.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      342 2023-06-27 11:06:51.000000 JestingLang-0.0.0a9/src/JestingLang/Misc/JTesting/NonFileExternalFileLoader.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-22 14:14:47.000000 JestingLang-0.0.0a9/src/JestingLang/Misc/JTesting/__init__.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-22 12:31:24.000000 JestingLang-0.0.0a9/src/JestingLang/Misc/__init__.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 06:05:46.000000 JestingLang-0.0.0a9/src/JestingLang/__init__.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     3037 2023-06-17 13:52:56.000000 JestingLang-0.0.0a9/src/JestingLang/main.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 13:16:13.944134 JestingLang-0.0.0a9/src/JestingLang.egg-info/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      937 2023-06-29 13:16:12.000000 JestingLang-0.0.0a9/src/JestingLang.egg-info/PKG-INFO
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1873 2023-06-29 13:16:13.000000 JestingLang-0.0.0a9/src/JestingLang.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        1 2023-06-29 13:16:12.000000 JestingLang-0.0.0a9/src/JestingLang.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        4 2023-06-29 13:16:12.000000 JestingLang-0.0.0a9/src/JestingLang.egg-info/requires.txt
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)       12 2023-06-29 13:16:12.000000 JestingLang-0.0.0a9/src/JestingLang.egg-info/top_level.txt
```

### Comparing `JestingLang-0.0.0a8/LICENSE` & `JestingLang-0.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a8/PKG-INFO` & `JestingLang-0.0.0a9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JestingLang
-Version: 0.0.0a8
+Version: 0.0.0a9
 Summary: A compiler for the minimalist spreadsheet language Jesting
 Home-page: https://github.com/itruffat/JestingLang
 Author: itrufat
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `JestingLang-0.0.0a8/README.md` & `JestingLang-0.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a8/setup.py` & `JestingLang-0.0.0a9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='JestingLang',
-    version='0.0.0a8',
+    version='0.0.0a9',
     author='itrufat',
     description='A compiler for the minimalist spreadsheet language Jesting',
     long_description='A compiler + a few node navigators (including an interpreter) for a minimalist language intended to copy the most basic functionalities found in spreadsheet-applications called JestingLang. It was created to be used with Jesting, a spreadsheet terminal tool.',
     long_description_content_type='text/markdown',
     url='https://github.com/itruffat/JestingLang',
     packages=['JestingLang',
               'JestingLang.Core',
```

### Comparing `JestingLang-0.0.0a8/src/JestingLang/Core/JDereferencer/CachedCellDereferencer.py` & `JestingLang-0.0.0a9/src/JestingLang/Core/JDereferencer/CachedCellDereferencer.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a8/src/JestingLang/Core/JDereferencer/CachedDereferencer.py` & `JestingLang-0.0.0a9/src/JestingLang/Core/JDereferencer/CachedDereferencer.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a8/src/JestingLang/Core/JDereferencer/KeyValueDereferencer.py` & `JestingLang-0.0.0a9/src/JestingLang/Core/JDereferencer/KeyValueDereferencer.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a8/src/JestingLang/Core/JParsing/JestingAST.py` & `JestingLang-0.0.0a9/src/JestingLang/Core/JParsing/JestingAST.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a8/src/JestingLang/Core/JVisitors/AbstractJestingVisitor.py` & `JestingLang-0.0.0a9/src/JestingLang/Core/JVisitors/AbstractJestingVisitor.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a8/src/JestingLang/Core/JVisitors/ContextBoundInterpreterVisitor.py` & `JestingLang-0.0.0a9/src/JestingLang/Core/JVisitors/ContextBoundInterpreterVisitor.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a8/src/JestingLang/Core/JVisitors/ContextfreeInterpreterVisitor.py` & `JestingLang-0.0.0a9/src/JestingLang/Core/JVisitors/ContextfreeInterpreterVisitor.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a8/src/JestingLang/Core/JVisitors/PrettyPrintingVisitors.py` & `JestingLang-0.0.0a9/src/JestingLang/Core/JVisitors/PrettyPrintingVisitors.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a8/src/JestingLang/JestingScript/JDereferencer/ScriptDereferencer.py` & `JestingLang-0.0.0a9/src/JestingLang/JestingScript/JDereferencer/ScriptDereferencer.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a8/src/JestingLang/JestingScript/JParsing/JestingScriptAST.py` & `JestingLang-0.0.0a9/src/JestingLang/JestingScript/JParsing/JestingScriptAST.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a8/src/JestingLang/JestingScript/JVisitors/ScriptInterpreterVisitor.py` & `JestingLang-0.0.0a9/src/JestingLang/JestingScript/JVisitors/ScriptInterpreterVisitor.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a8/src/JestingLang/LexerParser.py` & `JestingLang-0.0.0a9/src/JestingLang/LexerParser.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a8/src/JestingLang/Misc/JLogic/LogicFunctions.py` & `JestingLang-0.0.0a9/src/JestingLang/Misc/JLogic/LogicFunctions.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a8/src/JestingLang/Misc/JLogic/OperationMapping.py` & `JestingLang-0.0.0a9/src/JestingLang/Misc/JLogic/OperationMapping.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a8/src/JestingLang/Misc/JTesting/DereferencerHelper.py` & `JestingLang-0.0.0a9/src/JestingLang/Misc/JTesting/DereferencerHelper.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a8/src/JestingLang/main.py` & `JestingLang-0.0.0a9/src/JestingLang/main.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a8/src/JestingLang.egg-info/PKG-INFO` & `JestingLang-0.0.0a9/src/JestingLang.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JestingLang
-Version: 0.0.0a8
+Version: 0.0.0a9
 Summary: A compiler for the minimalist spreadsheet language Jesting
 Home-page: https://github.com/itruffat/JestingLang
 Author: itrufat
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `JestingLang-0.0.0a8/src/JestingLang.egg-info/SOURCES.txt` & `JestingLang-0.0.0a9/src/JestingLang.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 src/JestingLang/Core/JDereferencer/__init__.py
 src/JestingLang/Core/JParsing/JestingAST.py
 src/JestingLang/Core/JParsing/__init__.py
 src/JestingLang/Core/JVisitors/AbstractJestingVisitor.py
 src/JestingLang/Core/JVisitors/ContextBoundInterpreterVisitor.py
 src/JestingLang/Core/JVisitors/ContextfreeInterpreterVisitor.py
 src/JestingLang/Core/JVisitors/PrettyPrintingVisitors.py
+src/JestingLang/Core/JVisitors/ReferencesListerVisitor.py
 src/JestingLang/Core/JVisitors/__init__.py
 src/JestingLang/JestingScript/__init__.py
 src/JestingLang/JestingScript/JDereferencer/ScriptDereferencer.py
 src/JestingLang/JestingScript/JDereferencer/__init__.py
 src/JestingLang/JestingScript/JParsing/JestingScriptAST.py
 src/JestingLang/JestingScript/JParsing/__init__.py
 src/JestingLang/JestingScript/JVisitors/ScriptInterpreterVisitor.py
```

