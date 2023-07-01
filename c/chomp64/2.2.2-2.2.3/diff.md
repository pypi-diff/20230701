# Comparing `tmp/chomp64-2.2.2.tar.gz` & `tmp/chomp64-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chomp64-2.2.2.tar", last modified: Sun Jun 25 11:22:46 2023, max compression
+gzip compressed data, was "chomp64-2.2.3.tar", last modified: Sat Jul  1 12:40:29 2023, max compression
```

## Comparing `chomp64-2.2.2.tar` & `chomp64-2.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 11:22:46.590826 chomp64-2.2.2/
--rw-rw-rw-   0        0        0     1094 2023-06-25 08:49:13.000000 chomp64-2.2.2/LICENSE
--rw-rw-rw-   0        0        0      429 2023-06-25 11:22:46.588815 chomp64-2.2.2/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-06-25 08:49:13.000000 chomp64-2.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 11:22:46.568451 chomp64-2.2.2/chomp64/
--rw-rw-rw-   0        0        0        0 2023-06-25 09:38:56.000000 chomp64-2.2.2/chomp64/__init__.py
--rw-rw-rw-   0        0        0     9657 2023-06-25 11:20:20.000000 chomp64-2.2.2/chomp64/v2BasicChomper.py
-drwxrwxrwx   0        0        0        0 2023-06-25 11:22:46.587809 chomp64-2.2.2/chomp64.egg-info/
--rw-rw-rw-   0        0        0      429 2023-06-25 11:22:46.000000 chomp64-2.2.2/chomp64.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-06-25 11:22:46.000000 chomp64-2.2.2/chomp64.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 11:22:46.000000 chomp64-2.2.2/chomp64.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-25 11:22:46.000000 chomp64-2.2.2/chomp64.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 11:22:46.593829 chomp64-2.2.2/setup.cfg
--rw-rw-rw-   0        0        0      512 2023-06-25 11:20:34.000000 chomp64-2.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 12:40:29.453547 chomp64-2.2.3/
+-rw-rw-rw-   0        0        0     1094 2023-06-25 08:49:13.000000 chomp64-2.2.3/LICENSE
+-rw-rw-rw-   0        0        0      461 2023-07-01 12:40:29.452553 chomp64-2.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      694 2023-07-01 12:34:46.000000 chomp64-2.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 12:40:29.420333 chomp64-2.2.3/chomp64/
+-rw-rw-rw-   0        0        0        0 2023-06-25 11:32:10.000000 chomp64-2.2.3/chomp64/__init__.py
+-rw-rw-rw-   0        0        0     9882 2023-07-01 12:34:46.000000 chomp64-2.2.3/chomp64/v2BasicChomper.py
+drwxrwxrwx   0        0        0        0 2023-07-01 12:40:29.450576 chomp64-2.2.3/chomp64.egg-info/
+-rw-rw-rw-   0        0        0      461 2023-07-01 12:40:29.000000 chomp64-2.2.3/chomp64.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-07-01 12:40:29.000000 chomp64-2.2.3/chomp64.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 12:40:29.000000 chomp64-2.2.3/chomp64.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-01 12:40:29.000000 chomp64-2.2.3/chomp64.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 12:40:29.453547 chomp64-2.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      512 2023-07-01 12:37:35.000000 chomp64-2.2.3/setup.py
```

### Comparing `chomp64-2.2.2/LICENSE` & `chomp64-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chomp64-2.2.2/chomp64/v2BasicChomper.py` & `chomp64-2.2.3/chomp64/v2BasicChomper.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,31 +105,34 @@
         line = line.upper()
         line_no_quoted_material = self.__remove_quoted_material(line)
         tokenized_line = []
 
         if ("REM" in line_no_quoted_material):
             if (self.verbose):
                 print("CHOMP64: Remarked line, continuing...")
-            comment_line = self.__convert_to_list(line_no_quoted_material.replace("REM",""))
+            split = line.index("REM")
+            left, comment_line = line[0:split],line[split+3:]
+            tokenized_line_left, comment_line_list = self.__tokenize_line(left), self.__convert_to_list(comment_line) 
+            tokenized_line.extend(tokenized_line_left)
             tokenized_line.extend([0x8F])
-            tokenized_line.extend(comment_line)
+            tokenized_line.extend(comment_line_list)
             self.line_tokens.append("REM")
             return tokenized_line
         
         if (':' in line_no_quoted_material):
             if (self.verbose):
                 print("CHOMP64: Multiple commands in line, splitting...")
             
             split = line.index(':')
             left, right = line[0:split], line[split+1:]
-            split_left, split_right = self.__tokenize_line(left), self.__tokenize_line(right)
+            tokenized_line_left, tokenized_line_right = self.__tokenize_line(left), self.__tokenize_line(right)
 
-            tokenized_line.extend(split_left)
+            tokenized_line.extend(tokenized_line_left)
             tokenized_line.extend([ord(":")])
-            tokenized_line.extend(split_right)
+            tokenized_line.extend(tokenized_line_right)
 
             tokenized_line = [i for i in tokenized_line if i!='']
             return tokenized_line
 
         for i in range(len(self.keywords)):
             current_keyword = self.keywords[i]
```

### Comparing `chomp64-2.2.2/setup.py` & `chomp64-2.2.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 setup(
     name='chomp64',
-    version='2.2.2',
+    version='2.2.3',
     description='v2 BASIC Tokenizer',
     url='https://github.com/gvbarker/CHOMP',
     author='Giancarlo Barker',
     author_email='jonzomb80@gmail.com',
     license='MIT',
     packages=['chomp64'],
     classifiers=[
```

