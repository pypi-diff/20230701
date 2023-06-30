# Comparing `tmp/photos-where-1.1.tar.gz` & `tmp/photos_where-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photos-where-1.1.tar", last modified: Fri Jun 30 19:03:03 2023, max compression
+gzip compressed data, was "photos_where-1.2.tar", last modified: Fri Jun 30 22:42:25 2023, max compression
```

## Comparing `photos-where-1.1.tar` & `photos_where-1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-06-30 19:03:03.290268 photos-where-1.1/
--rw-r--r--   0 visgean    (501) staff       (20)     1063 2022-09-28 18:42:28.000000 photos-where-1.1/LICENSE
--rw-r--r--   0 visgean    (501) staff       (20)       52 2023-06-30 18:32:54.000000 photos-where-1.1/MANIFEST.in
--rw-r--r--   0 visgean    (501) staff       (20)      896 2023-06-30 19:03:03.290115 photos-where-1.1/PKG-INFO
--rw-r--r--   0 visgean    (501) staff       (20)      318 2023-06-30 19:02:35.000000 photos-where-1.1/README.md
-drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-06-30 19:03:03.288830 photos-where-1.1/photos_where.egg-info/
--rw-r--r--   0 visgean    (501) staff       (20)      896 2023-06-30 19:03:03.000000 photos-where-1.1/photos_where.egg-info/PKG-INFO
--rw-r--r--   0 visgean    (501) staff       (20)      297 2023-06-30 19:03:03.000000 photos-where-1.1/photos_where.egg-info/SOURCES.txt
--rw-r--r--   0 visgean    (501) staff       (20)        1 2023-06-30 19:03:03.000000 photos-where-1.1/photos_where.egg-info/dependency_links.txt
--rw-r--r--   0 visgean    (501) staff       (20)       46 2023-06-30 19:03:03.000000 photos-where-1.1/photos_where.egg-info/entry_points.txt
--rw-r--r--   0 visgean    (501) staff       (20)       30 2023-06-30 19:03:03.000000 photos-where-1.1/photos_where.egg-info/requires.txt
--rw-r--r--   0 visgean    (501) staff       (20)        4 2023-06-30 19:03:03.000000 photos-where-1.1/photos_where.egg-info/top_level.txt
--rw-r--r--   0 visgean    (501) staff       (20)       38 2023-06-30 19:03:03.290336 photos-where-1.1/setup.cfg
--rw-r--r--   0 visgean    (501) staff       (20)      944 2023-06-30 19:00:50.000000 photos-where-1.1/setup.py
-drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-06-30 19:03:03.289491 photos-where-1.1/src/
--rw-r--r--   0 visgean    (501) staff       (20)       24 2023-06-30 17:41:46.000000 photos-where-1.1/src/__init__.py
--rwxr-xr-x   0 visgean    (501) staff       (20)     2037 2023-06-30 18:47:13.000000 photos-where-1.1/src/main.py
--rw-r--r--   0 visgean    (501) staff       (20)     5094 2023-06-30 18:35:06.000000 photos-where-1.1/src/where.py
+drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-06-30 22:42:25.819659 photos_where-1.2/
+-rw-r--r--   0 visgean    (501) staff       (20)     1063 2022-09-28 18:42:28.000000 photos_where-1.2/LICENSE
+-rw-r--r--   0 visgean    (501) staff       (20)       52 2023-06-30 18:32:54.000000 photos_where-1.2/MANIFEST.in
+-rw-r--r--   0 visgean    (501) staff       (20)     1941 2023-06-30 22:42:25.819526 photos_where-1.2/PKG-INFO
+-rw-r--r--   0 visgean    (501) staff       (20)     1251 2023-06-30 22:41:25.000000 photos_where-1.2/README.md
+drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-06-30 22:42:25.818537 photos_where-1.2/photos_where/
+-rw-r--r--   0 visgean    (501) staff       (20)       25 2023-06-30 22:30:00.000000 photos_where-1.2/photos_where/__init__.py
+-rwxr-xr-x   0 visgean    (501) staff       (20)     2037 2023-06-30 18:47:13.000000 photos_where-1.2/photos_where/main.py
+-rw-r--r--   0 visgean    (501) staff       (20)     5100 2023-06-30 22:25:30.000000 photos_where-1.2/photos_where/where.py
+drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-06-30 22:42:25.819339 photos_where-1.2/photos_where.egg-info/
+-rw-r--r--   0 visgean    (501) staff       (20)     1941 2023-06-30 22:42:25.000000 photos_where-1.2/photos_where.egg-info/PKG-INFO
+-rw-r--r--   0 visgean    (501) staff       (20)      324 2023-06-30 22:42:25.000000 photos_where-1.2/photos_where.egg-info/SOURCES.txt
+-rw-r--r--   0 visgean    (501) staff       (20)        1 2023-06-30 22:42:25.000000 photos_where-1.2/photos_where.egg-info/dependency_links.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       57 2023-06-30 22:42:25.000000 photos_where-1.2/photos_where.egg-info/entry_points.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       54 2023-06-30 22:42:25.000000 photos_where-1.2/photos_where.egg-info/requires.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       13 2023-06-30 22:42:25.000000 photos_where-1.2/photos_where.egg-info/top_level.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       38 2023-06-30 22:42:25.819699 photos_where-1.2/setup.cfg
+-rw-r--r--   0 visgean    (501) staff       (20)     1017 2023-06-30 22:41:25.000000 photos_where-1.2/setup.py
```

### Comparing `photos-where-1.1/LICENSE` & `photos_where-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `photos-where-1.1/setup.py` & `photos_where-1.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,35 +6,35 @@
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-
 setup(
-    name="photos-where",
-    version="1.1",
+    name="photos_where",
+    version="1.2",
     description="Analyze exif data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Visgean",
     author_email="visgean@gmail.com",
     url="https://github.com/visgean/where",
     packages=[
-        "src",
+        "photos_where",
     ],
-    package_dir={"src": "src"},
+    package_dir={"photos_where": "photos_where"},
     license="MIT",
     keywords="exif sql",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
     ],
     install_requires=[
         "exif2pandas",
         "pandas",
-        "matplotlib"
+        "matplotlib",
+        "reverse-geocoder==1.5.1",
     ],
-    entry_points={"console_scripts": ["where-when = src.main:main"]},
+    entry_points={"console_scripts": ["photos_where = photos_where.main:main"]},
 )
```

### Comparing `photos-where-1.1/src/main.py` & `photos_where-1.2/photos_where/main.py`

 * *Files identical despite different names*

### Comparing `photos-where-1.1/src/where.py` & `photos_where-1.2/photos_where/where.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             ignore_countries=(),
             processes=5,
             first_interval: Optional[datetime.date] = None,
             last_interval: Optional[datetime.date] = None,
     ):
         self.cities_file = cities_file
         if cities_file is None:
-            self.cities_file = pkg_resources.resource_filename('src', 'cities.csv')
+            self.cities_file = pkg_resources.resource_filename('photos_where', 'cities.csv')
 
         self.ignore_countries = ignore_countries
         self.feather_location = feather_location
         self.first_interval = first_interval
         self.last_interval = last_interval
 
         # get raw dataframe with wide exif rows
@@ -87,23 +87,22 @@
         # add date index, geocoder preservers the
         # order of the rows so this is fine
         country_df.index = df_location.index
         return df_location.join(country_df)
 
 
     def _get_intervals(self):
-        # lol the most hacky way to get the index at loc 0
+        first_row = self.countries_df[:1].to_dict(orient='index')
+        previous_date = list(first_row.keys())[0]
+        previous_country_code = first_row[previous_date]['cc']
+        previous_country = first_row[previous_date]['admin1']
+
 
         if self.first_interval:
             previous_date = self.first_interval
-        else:
-            previous_date = list(self.countries_df[:1].to_dict(orient='index').keys())[0]
-
-        previous_country_code = 'CZ'
-        previous_country = 'Czech Republic'
 
         intervals = []
 
         for dt, row in self.countries_df.iterrows():
             country_code = row['cc']
             country = row['admin1']
```

