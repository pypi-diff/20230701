# Comparing `tmp/omnivoreql-0.1.tar.gz` & `tmp/omnivoreql-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnivoreql-0.1.tar", last modified: Sat Jul  1 14:54:03 2023, max compression
+gzip compressed data, was "omnivoreql-0.2.1.tar", last modified: Sat Jul  1 17:12:55 2023, max compression
```

## Comparing `omnivoreql-0.1.tar` & `omnivoreql-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 14:54:03.886581 omnivoreql-0.1/
--rw-rw-rw-   0        0        0     1086 2023-06-27 21:56:13.000000 omnivoreql-0.1/LICENSE
--rw-rw-rw-   0        0        0      263 2023-07-01 14:54:03.887581 omnivoreql-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      804 2023-06-27 22:29:17.000000 omnivoreql-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 14:54:03.884585 omnivoreql-0.1/omnivoreql.egg-info/
--rw-rw-rw-   0        0        0      263 2023-07-01 14:54:03.000000 omnivoreql-0.1/omnivoreql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-07-01 14:54:03.000000 omnivoreql-0.1/omnivoreql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 14:54:03.000000 omnivoreql-0.1/omnivoreql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-01 14:54:03.000000 omnivoreql-0.1/omnivoreql.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 14:54:03.000000 omnivoreql-0.1/omnivoreql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 14:54:03.888580 omnivoreql-0.1/setup.cfg
--rw-rw-rw-   0        0        0      361 2023-07-01 14:51:44.000000 omnivoreql-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 14:54:03.885581 omnivoreql-0.1/test/
--rw-rw-rw-   0        0        0     2269 2023-07-01 14:32:45.000000 omnivoreql-0.1/test/test_omnivoreql.py
+drwxrwxrwx   0        0        0        0 2023-07-01 17:12:55.282087 omnivoreql-0.2.1/
+-rw-rw-rw-   0        0        0     1086 2023-06-27 21:56:13.000000 omnivoreql-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2102 2023-07-01 17:12:55.282087 omnivoreql-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1492 2023-07-01 16:14:34.000000 omnivoreql-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 17:12:55.282087 omnivoreql-0.2.1/omnivoreql.egg-info/
+-rw-rw-rw-   0        0        0     2102 2023-07-01 17:12:55.000000 omnivoreql-0.2.1/omnivoreql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-07-01 17:12:55.000000 omnivoreql-0.2.1/omnivoreql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 17:12:55.000000 omnivoreql-0.2.1/omnivoreql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-01 17:12:55.000000 omnivoreql-0.2.1/omnivoreql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 17:12:55.000000 omnivoreql-0.2.1/omnivoreql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 17:12:55.290083 omnivoreql-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1117 2023-07-01 17:12:22.000000 omnivoreql-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 17:12:55.282087 omnivoreql-0.2.1/test/
+-rw-rw-rw-   0        0        0     2490 2023-07-01 15:33:30.000000 omnivoreql-0.2.1/test/test_omnivoreql.py
```

### Comparing `omnivoreql-0.1/LICENSE` & `omnivoreql-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `omnivoreql-0.1/test/test_omnivoreql.py` & `omnivoreql-0.2.1/test/test_omnivoreql.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,10 +50,15 @@
         self.assertFalse('errorCodes' in articles['article'])
 
     def test_get_labels(self):
         labels = self.omnivoreql.get_labels()
         self.assertIsNotNone(labels)
         self.assertFalse('errorCodes' in labels['labels'])
 
+    def test_get_subscriptions(self):
+        subscriptions = self.omnivoreql.get_subscriptions()
+        self.assertIsNotNone(subscriptions)
+        self.assertFalse('errorCodes' in subscriptions['subscriptions'])
+
 
 if __name__ == '__main__':
     unittest.main()
```

