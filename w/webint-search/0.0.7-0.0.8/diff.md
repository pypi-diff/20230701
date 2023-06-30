# Comparing `tmp/webint_search-0.0.7.tar.gz` & `tmp/webint_search-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webint_search-0.0.7.tar", max compression
+gzip compressed data, was "webint_search-0.0.8.tar", max compression
```

## Comparing `webint_search-0.0.7.tar` & `webint_search-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      940 2023-06-29 03:28:26.260879 webint_search-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3060 2023-06-21 00:16:47.504283 webint_search-0.0.7/webint_search/__init__.py
--rw-r--r--   0        0        0      128 2023-01-27 00:43:56.444286 webint_search-0.0.7/webint_search/templates/__init__.py
--rw-r--r--   0        0        0      730 2023-01-27 00:43:56.444286 webint_search-0.0.7/webint_search/templates/collections.html
--rw-r--r--   0        0        0       44 2023-03-08 03:53:03.547149 webint_search-0.0.7/webint_search/templates/index.html
--rw-r--r--   0        0        0     1078 2023-01-27 00:43:56.444286 webint_search-0.0.7/webint_search/templates/opensearch.xml
--rw-r--r--   0        0        0     1355 2023-06-19 21:30:39.852261 webint_search-0.0.7/webint_search/templates/results.html
--rw-r--r--   0        0        0      588 2023-06-21 00:17:04.604516 webint_search-0.0.7/webint_search/templates/youtube_results.html
--rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 webint_search-0.0.7/setup.py
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 webint_search-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      999 2023-06-30 22:11:44.564915 webint_search-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4025 2023-06-30 21:54:18.348422 webint_search-0.0.8/webint_search/__init__.py
+-rw-r--r--   0        0        0      128 2023-01-27 00:43:56.444286 webint_search-0.0.8/webint_search/templates/__init__.py
+-rw-r--r--   0        0        0      730 2023-01-27 00:43:56.444286 webint_search-0.0.8/webint_search/templates/collections.html
+-rw-r--r--   0        0        0       44 2023-03-08 03:53:03.547149 webint_search-0.0.8/webint_search/templates/index.html
+-rw-r--r--   0        0        0     1078 2023-01-27 00:43:56.444286 webint_search-0.0.8/webint_search/templates/opensearch.xml
+-rw-r--r--   0        0        0     1567 2023-06-30 21:54:34.692692 webint_search-0.0.8/webint_search/templates/results.html
+-rw-r--r--   0        0        0      588 2023-06-21 00:17:04.604516 webint_search-0.0.8/webint_search/templates/youtube_results.html
+-rw-r--r--   0        0        0      903 1970-01-01 00:00:00.000000 webint_search-0.0.8/setup.py
+-rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 webint_search-0.0.8/PKG-INFO
```

### Comparing `webint_search-0.0.7/pyproject.toml` & `webint_search-0.0.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 [tool.poetry]
 name = "webint-search"
-version = "0.0.7"
+version = "0.0.8"
 description = "search the data on your website and beyond"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "AGPL-3.0-or-later"
 packages = [{include = "webint_search"}]
 
 [tool.poetry.plugins."webapps"]
 search = "webint_search:app"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
 webint = ">=0.0"
 typesense = "^0.15.0"
 youtube-search = "^2.1.2"
+wn = "^0.9.4"
+eng-to-ipa = "^0.0.2"
+pronouncing = "^0.2.0"
 
 [tool.poetry.group.dev.dependencies]
 # gmpg = "^0.0"
 bgq = {path="../bgq", develop=true}
 gmpg = {path="../gmpg", develop=true}
 newmath = {path="../newmath", develop=true}
 sqlyte = {path="../sqlyte", develop=true}
```

### Comparing `webint_search-0.0.7/webint_search/templates/collections.html` & `webint_search-0.0.8/webint_search/templates/collections.html`

 * *Files identical despite different names*

### Comparing `webint_search-0.0.7/webint_search/templates/opensearch.xml` & `webint_search-0.0.8/webint_search/templates/opensearch.xml`

 * *Files identical despite different names*

### Comparing `webint_search-0.0.7/webint_search/templates/results.html` & `webint_search-0.0.8/webint_search/templates/results.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-$def with (query, web_results, code_projects, code_files, books)
+$def with (query, ipa_pronunciation, cmu_pronunciation, definition, rhymes, web_results, code_projects, code_files, books)
 $var breadcrumbs = ("search", "Search")
 $var title: Results for
 
 <form>
     <input name=q value="$query"> <button>Search</button>
 </form>
 
+$if definition:
+    <p><strong title="$cmu_pronunciation">$ipa_pronunciation</strong>, $definition<br>
+    <small>rhymes: $", ".join(rhymes)</small></p>
+
 <h2>Web</h2>
 $if web_results:
     <ul>
     $for result in web_results:
         <li><a href="$webagt.uri(result.element.attrib['href'])['uddg'][0]">$result.text</a></li>
     </ul>
 $else:
```

#### html2text {}

```diff
@@ -1,10 +1,14 @@
-$def with (query, web_results, code_projects, code_files, books) $var
-breadcrumbs = ("search", "Search") $var title: Results for
+$def with (query, ipa_pronunciation, cmu_pronunciation, definition, rhymes,
+web_results, code_projects, code_files, books) $var breadcrumbs = ("search",
+"Search") $var title: Results for
 [$query              ] Search
+$if definition:
+$ipa_pronunciation, $definition
+rhymes: $", ".join(rhymes)
 ***** Web *****
 $if web_results:
     * $for result in web_results:
     * $result.text
 $else:
 0 results
 ***** Code *****
```

### Comparing `webint_search-0.0.7/webint_search/templates/youtube_results.html` & `webint_search-0.0.8/webint_search/templates/youtube_results.html`

 * *Files identical despite different names*

### Comparing `webint_search-0.0.7/setup.py` & `webint_search-0.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,22 +4,27 @@
 packages = \
 ['webint_search', 'webint_search.templates']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['typesense>=0.15.0,<0.16.0', 'webint>=0.0', 'youtube-search>=2.1.2,<3.0.0']
+['eng-to-ipa>=0.0.2,<0.0.3',
+ 'pronouncing>=0.2.0,<0.3.0',
+ 'typesense>=0.15.0,<0.16.0',
+ 'webint>=0.0',
+ 'wn>=0.9.4,<0.10.0',
+ 'youtube-search>=2.1.2,<3.0.0']
 
 entry_points = \
 {'webapps': ['search = webint_search:app']}
 
 setup_kwargs = {
     'name': 'webint-search',
-    'version': '0.0.7',
+    'version': '0.0.8',
     'description': 'search the data on your website and beyond',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

