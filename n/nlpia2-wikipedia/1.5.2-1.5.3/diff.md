# Comparing `tmp/nlpia2_wikipedia-1.5.2.tar.gz` & `tmp/nlpia2_wikipedia-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpia2_wikipedia-1.5.2.tar", max compression
+gzip compressed data, was "nlpia2_wikipedia-1.5.3.tar", max compression
```

## Comparing `nlpia2_wikipedia-1.5.2.tar` & `nlpia2_wikipedia-1.5.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1057 2022-02-24 21:47:29.044908 nlpia2_wikipedia-1.5.2/LICENSE
--rw-r--r--   0        0        0     3798 2022-05-04 23:25:18.637807 nlpia2_wikipedia-1.5.2/README.md
--rw-r--r--   0        0        0     1615 2023-06-28 21:55:20.132739 nlpia2_wikipedia-1.5.2/pyproject.toml
--rw-r--r--   0        0        0       76 2022-05-04 23:22:34.280323 nlpia2_wikipedia-1.5.2/src/nlpia2_wikipedia/__init__.py
--rw-r--r--   0        0        0     2280 2022-02-24 21:47:29.048910 nlpia2_wikipedia-1.5.2/src/nlpia2_wikipedia/exceptions.py
--rw-r--r--   0        0        0      985 2022-02-24 21:47:29.048910 nlpia2_wikipedia-1.5.2/src/nlpia2_wikipedia/util.py
--rw-r--r--   0        0        0    23481 2022-02-24 22:35:10.763977 nlpia2_wikipedia-1.5.2/src/nlpia2_wikipedia/wikipedia.py
--rw-r--r--   0        0        0     4773 1970-01-01 00:00:00.000000 nlpia2_wikipedia-1.5.2/setup.py
--rw-r--r--   0        0        0     5250 1970-01-01 00:00:00.000000 nlpia2_wikipedia-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1057 2022-02-24 21:47:29.044908 nlpia2_wikipedia-1.5.3/LICENSE
+-rw-r--r--   0        0        0     3798 2022-05-04 23:25:18.637807 nlpia2_wikipedia-1.5.3/README.md
+-rw-r--r--   0        0        0     1616 2023-07-01 00:19:11.797373 nlpia2_wikipedia-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0       99 2023-07-01 00:11:01.060006 nlpia2_wikipedia-1.5.3/src/nlpia2_wikipedia/__init__.py
+-rw-r--r--   0        0        0     2420 2023-06-30 23:36:01.865166 nlpia2_wikipedia-1.5.3/src/nlpia2_wikipedia/exceptions.py
+-rw-r--r--   0        0        0     1623 2023-07-01 00:11:05.932013 nlpia2_wikipedia-1.5.3/src/nlpia2_wikipedia/parsers.py
+-rw-r--r--   0        0        0     1069 2023-06-30 23:31:53.674041 nlpia2_wikipedia-1.5.3/src/nlpia2_wikipedia/util.py
+-rw-r--r--   0        0        0    23481 2022-02-24 22:35:10.763977 nlpia2_wikipedia-1.5.3/src/nlpia2_wikipedia/wikipedia.py
+-rw-r--r--   0        0        0     4773 1970-01-01 00:00:00.000000 nlpia2_wikipedia-1.5.3/setup.py
+-rw-r--r--   0        0        0     5250 1970-01-01 00:00:00.000000 nlpia2_wikipedia-1.5.3/PKG-INFO
```

### Comparing `nlpia2_wikipedia-1.5.2/LICENSE` & `nlpia2_wikipedia-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nlpia2_wikipedia-1.5.2/README.md` & `nlpia2_wikipedia-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `nlpia2_wikipedia-1.5.2/pyproject.toml` & `nlpia2_wikipedia-1.5.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nlpia2_wikipedia"
-version = "1.5.2"
-description = "Updated version of `wikipedia` package because original repo has been abansdonedsince 2014."
+version = "1.5.3"
+description = "Updated version of `wikipedia` package because original repo has been abandoned since 2014."
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 authors = [
     "Hobson Lane <hobson@tangibleai.com>",
     ]
 homepage = "https://gitlab.com/tangibleai/community/nlpia2_wikipedia"
 repository = "https://gitlab.com/tangibleai/community/nlpia2_wikipedia"
 documentation = "https://gitlab.com/tangibleai/community/nlpia2_wikipedia"
 packages = [
     {include="nlpia2_wikipedia", from="src"},
     ]
 
 
+
 keywords = [
     'wiki',
     'Wikipedia',
     'scraping',
     'api',
     'wrapper',
     'crawler',
```

### Comparing `nlpia2_wikipedia-1.5.2/src/nlpia2_wikipedia/exceptions.py` & `nlpia2_wikipedia-1.5.3/src/nlpia2_wikipedia/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,76 +5,76 @@
 import sys
 
 
 ODD_ERROR_MESSAGE = "This shouldn't happen. Please report on GitHub: github.com/goldsmith/Wikipedia"
 
 
 class WikipediaException(Exception):
-  """Base Wikipedia exception class."""
+    """Base Wikipedia exception class."""
 
-  def __init__(self, error):
-    self.error = error
+    def __init__(self, error):
+        self.error = error
 
-  def __unicode__(self):
-    return "An unknown error occured: \"{0}\". Please report it on GitHub!".format(self.error)
+    def __unicode__(self):
+        return "An unknown error occured: \"{0}\". Please report it on GitHub!".format(self.error)
 
-  if sys.version_info > (3, 0):
-    def __str__(self):
-      return self.__unicode__()
+    if sys.version_info > (3, 0):
+        def __str__(self):
+            return self.__unicode__()
 
-  else:
-    def __str__(self):
-      return self.__unicode__().encode('utf8')
+    else:
+        def __str__(self):
+            return self.__unicode__().encode('utf8')
 
 
 class PageError(WikipediaException):
-  """Exception raised when no Wikipedia matched a query."""
-
-  def __init__(self, pageid=None, *args):
-    if pageid:
-      self.pageid = pageid
-    else:
-      self.title = args[0]
+    """Exception raised when no Wikipedia matched a query."""
 
-  def __unicode__(self):
-    if hasattr(self, 'title'):
-      return u"\"{0}\" does not match any pages. Try another query!".format(self.title)
-    else:
-      return u"Page id \"{0}\" does not match any pages. Try another id!".format(self.pageid)
+    def __init__(self, pageid=None, *args):
+        if pageid:
+            self.pageid = pageid
+        else:
+            self.title = args[0]
+
+    def __unicode__(self):
+        if hasattr(self, 'title'):
+            return u"\"{0}\" does not match any pages. Try another query!".format(self.title)
+        else:
+            return u"Page id \"{0}\" does not match any pages. Try another id!".format(self.pageid)
 
 
 class DisambiguationError(WikipediaException):
-  """
-  Exception raised when a page resolves to a Disambiguation page.
+    """
+    Exception raised when a page resolves to a Disambiguation page.
 
-  The `options` property contains a list of titles
-  of Wikipedia pages that the query may refer to.
+    The `options` property contains a list of titles
+    of Wikipedia pages that the query may refer to.
 
-  .. note:: `options` does not include titles that do not link to a valid Wikipedia page.
-  """
+    .. note:: `options` does not include titles that do not link to a valid Wikipedia page.
+    """
 
-  def __init__(self, title, may_refer_to):
-    self.title = title
-    self.options = may_refer_to
+    def __init__(self, title, may_refer_to):
+        self.title = title
+        self.options = may_refer_to
 
-  def __unicode__(self):
-    return u"\"{0}\" may refer to: \n{1}".format(self.title, '\n'.join(self.options))
+    def __unicode__(self):
+        return u"\"{0}\" may refer to: \n{1}".format(self.title, '\n'.join(self.options))
 
 
 class RedirectError(WikipediaException):
-  """Exception raised when a page title unexpectedly resolves to a redirect."""
+    """Exception raised when a page title unexpectedly resolves to a redirect."""
 
-  def __init__(self, title):
-    self.title = title
+    def __init__(self, title):
+        self.title = title
 
-  def __unicode__(self):
-    return u"\"{0}\" resulted in a redirect. Set the redirect property to True to allow automatic redirects.".format(self.title)
+    def __unicode__(self):
+        return u"\"{0}\" resulted in a redirect. Set the redirect property to True to allow automatic redirects.".format(self.title)
 
 
 class HTTPTimeoutError(WikipediaException):
-  """Exception raised when a request to the Mediawiki servers times out."""
+    """Exception raised when a request to the Mediawiki servers times out."""
 
-  def __init__(self, query):
-    self.query = query
+    def __init__(self, query):
+        self.query = query
 
-  def __unicode__(self):
-    return u"Searching for \"{0}\" resulted in a timeout. Try again in a few seconds, and make sure you have rate limiting set to True.".format(self.query)
+    def __unicode__(self):
+        return u"Searching for \"{0}\" resulted in a timeout. Try again in a few seconds, and make sure you have rate limiting set to True.".format(self.query)
```

### Comparing `nlpia2_wikipedia-1.5.2/src/nlpia2_wikipedia/util.py` & `nlpia2_wikipedia-1.5.3/src/nlpia2_wikipedia/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from __future__ import print_function, unicode_literals
 
 import sys
 import functools
 
 def debug(fn):
-  def wrapper(*args, **kwargs):
-    print(fn.__name__, 'called!')
-    print(sorted(args), tuple(sorted(kwargs.items())))
-    res = fn(*args, **kwargs)
-    print(res)
-    return res
-  return wrapper
+    def wrapper(*args, **kwargs):
+        print(fn.__name__, 'called!')
+        print(sorted(args), tuple(sorted(kwargs.items())))
+        res = fn(*args, **kwargs)
+        print(res)
+        return res
+    return wrapper
 
 
 class cache(object):
 
-  def __init__(self, fn):
-    self.fn = fn
-    self._cache = {}
-    functools.update_wrapper(self, fn)
-
-  def __call__(self, *args, **kwargs):
-    key = str(args) + str(kwargs)
-    if key in self._cache:
-      ret = self._cache[key]
-    else:
-      ret = self._cache[key] = self.fn(*args, **kwargs)
+    def __init__(self, fn):
+        self.fn = fn
+        self._cache = {}
+        functools.update_wrapper(self, fn)
+
+    def __call__(self, *args, **kwargs):
+        key = str(args) + str(kwargs)
+        if key in self._cache:
+            ret = self._cache[key]
+        else:
+            ret = self._cache[key] = self.fn(*args, **kwargs)
 
-    return ret
+        return ret
 
-  def clear_cache(self):
-    self._cache = {}
+    def clear_cache(self):
+        self._cache = {}
 
 
 # from http://stackoverflow.com/questions/3627793/best-output-type-and-encoding-practices-for-repr-functions
 def stdout_encode(u, default='UTF8'):
-  encoding = sys.stdout.encoding or default
-  if sys.version_info > (3, 0):
-    return u.encode(encoding).decode(encoding)
-  return u.encode(encoding)
+    encoding = sys.stdout.encoding or default
+    if sys.version_info > (3, 0):
+        return u.encode(encoding).decode(encoding)
+    return u.encode(encoding)
```

### Comparing `nlpia2_wikipedia-1.5.2/src/nlpia2_wikipedia/wikipedia.py` & `nlpia2_wikipedia-1.5.3/src/nlpia2_wikipedia/wikipedia.py`

 * *Files identical despite different names*

### Comparing `nlpia2_wikipedia-1.5.2/setup.py` & `nlpia2_wikipedia-1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 {'': ['*']}
 
 install_requires = \
 ['beautifulsoup4>=4.11', 'poetry>=1.1', 'requests>=2.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'nlpia2-wikipedia',
-    'version': '1.5.2',
-    'description': 'Updated version of `wikipedia` package because original repo has been abansdonedsince 2014.',
+    'version': '1.5.3',
+    'description': 'Updated version of `wikipedia` package because original repo has been abandoned since 2014.',
     'long_description': '# Wikipedia\n\n[![image](https://travis-ci.org/goldsmith/Wikipedia.png?branch=master)](https://travis-ci.org/goldsmith/Wikipedia)\n\n[![image](https://pypip.in/d/wikipedia/badge.png)](https://crate.io/packages/wikipedia)\n\n[![image](https://pypip.in/v/wikipedia/badge.png)](https://crate.io/packages/wikipedia)\n\n[![License](https://pypip.in/license/wikipedia/badge.png)](https://pypi.python.org/pypi/wikipedia/)\n\n**Wikipedia** is a Python library that makes it easy to access and parse\ndata from Wikipedia.\n\nSearch Wikipedia, get article summaries, get data like links and images\nfrom a page, and more. Wikipedia wraps the [MediaWiki\nAPI](https://www.mediawiki.org/wiki/API) so you can focus on using\nWikipedia data, not getting it.\n\n``` {.python}\n>>> import wikipedia\n>>> print wikipedia.summary("Wikipedia")\n# Wikipedia (/ˌwɪkɨˈpiːdiə/ or /ˌwɪkiˈpiːdiə/ WIK-i-PEE-dee-ə) is a collaboratively edited, multilingual, free Internet encyclopedia supported by the non-profit Wikimedia Foundation...\n\n>>> wikipedia.search("Barack")\n# [u\'Barak (given name)\', u\'Barack Obama\', u\'Barack (brandy)\', u\'Presidency of Barack Obama\', u\'Family of Barack Obama\', u\'First inauguration of Barack Obama\', u\'Barack Obama presidential campaign, 2008\', u\'Barack Obama, Sr.\', u\'Barack Obama citizenship conspiracy theories\', u\'Presidential transition of Barack Obama\']\n\n>>> ny = wikipedia.page("New York")\n>>> ny.title\n# u\'New York\'\n>>> ny.url\n# u\'http://en.wikipedia.org/wiki/New_York\'\n>>> ny.content\n# u\'New York is a state in the Northeastern region of the United States. New York is the 27th-most exten\'...\n>>> ny.links[0]\n# u\'1790 United States Census\'\n\n>>> wikipedia.set_lang("fr")\n>>> wikipedia.summary("Facebook", sentences=1)\n# Facebook est un service de réseautage social en ligne sur Internet permettant d\'y publier des informations (photographies, liens, textes, etc.) en contrôlant leur visibilité par différentes catégories de personnes.\n```\n\nNote: this library was designed for ease of use and simplicity, not for\nadvanced use. If you plan on doing serious scraping or automated\nrequests, please use\n[Pywikipediabot](http://www.mediawiki.org/wiki/Manual:Pywikipediabot)\n(or one of the other more advanced [Python MediaWiki API\nwrappers](http://en.wikipedia.org/wiki/Wikipedia:Creating_a_bot#Python)),\nwhich has a larger API, rate limiting, and other features so we can be\nconsiderate of the MediaWiki infrastructure.\n\n## Installation\n\nTo install Wikipedia, simply run:\n\n    $ pip install wikipedia\n\nWikipedia is compatible with Python 2.6+ (2.7+ to run unittest discover)\nand Python 3.3+.\n\n## Documentation\n\nRead the docs at <https://wikipedia.readthedocs.org/en/latest/>.\n\n-   [Quickstart](https://wikipedia.readthedocs.org/en/latest/quickstart.html)\n-   [Full API](https://wikipedia.readthedocs.org/en/latest/code.html)\n\nTo run tests, clone the [repository on\nGitHub](https://github.com/goldsmith/Wikipedia), then run:\n\n    $ pip install -r requirements.txt\n    $ bash runtests  # will run tests for python and python3\n    $ python -m unittest discover tests/ \'*test.py\'  # manual style\n\nin the root project directory.\n\nTo build the documentation yourself, after installing requirements.txt,\nrun:\n\n    $ pip install sphinx\n    $ cd docs/\n    $ make html\n\n## License\n\nMIT licensed. See the [LICENSE\nfile](https://github.com/goldsmith/Wikipedia/blob/master/LICENSE) for\nfull details.\n\n## Credits\n\n-   [wiki-api](https://github.com/richardasaurus/wiki-api) by\n    \\@richardasaurus for inspiration\n-   \\@nmoroze and \\@themichaelyang for feedback and suggestions\n-   The [Wikimedia Foundation](http://wikimediafoundation.org/wiki/Home)\n    for giving the world free access to data\n\n[![Bitdeli badge](https://d2weczhvl823v0.cloudfront.net/goldsmith/wikipedia/trend.png)](https://bitdeli.com/free)\n',
     'author': 'Hobson Lane',
     'author_email': 'hobson@tangibleai.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/tangibleai/community/nlpia2_wikipedia',
     'package_dir': package_dir,
```

### Comparing `nlpia2_wikipedia-1.5.2/PKG-INFO` & `nlpia2_wikipedia-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nlpia2-wikipedia
-Version: 1.5.2
-Summary: Updated version of `wikipedia` package because original repo has been abansdonedsince 2014.
+Version: 1.5.3
+Summary: Updated version of `wikipedia` package because original repo has been abandoned since 2014.
 Home-page: https://gitlab.com/tangibleai/community/nlpia2_wikipedia
 License: AGPL-3.0-or-later
 Keywords: wiki,Wikipedia,scraping,api,wrapper,crawler,markdown,html,parser
 Author: Hobson Lane
 Author-email: hobson@tangibleai.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
```

