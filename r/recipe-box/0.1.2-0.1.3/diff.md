# Comparing `tmp/recipe_box-0.1.2.tar.gz` & `tmp/recipe_box-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recipe_box-0.1.2.tar", last modified: Sat Jun 27 19:59:49 2020, max compression
+gzip compressed data, was "dist/recipe_box-0.1.3.tar", last modified: Sat Jul  1 11:52:58 2023, max compression
```

## Comparing `recipe_box-0.1.2.tar` & `recipe_box-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 lcordier  (1000) lcordier  (1000)        0 2020-06-27 19:59:49.552528 recipe_box-0.1.2/
--rw-r--r--   0 lcordier  (1000) lcordier  (1000)     7413 2020-06-27 19:59:49.552528 recipe_box-0.1.2/PKG-INFO
--rw-r--r--   0 lcordier  (1000) lcordier  (1000)     5777 2020-06-27 19:02:47.000000 recipe_box-0.1.2/README.md
-drwxr-xr-x   0 lcordier  (1000) lcordier  (1000)        0 2020-06-27 19:59:49.552528 recipe_box-0.1.2/recipe_box.egg-info/
--rw-r--r--   0 lcordier  (1000) lcordier  (1000)     7413 2020-06-27 19:59:49.000000 recipe_box-0.1.2/recipe_box.egg-info/PKG-INFO
--rw-r--r--   0 lcordier  (1000) lcordier  (1000)      238 2020-06-27 19:59:49.000000 recipe_box-0.1.2/recipe_box.egg-info/SOURCES.txt
--rw-r--r--   0 lcordier  (1000) lcordier  (1000)        1 2020-06-27 19:59:49.000000 recipe_box-0.1.2/recipe_box.egg-info/dependency_links.txt
--rw-r--r--   0 lcordier  (1000) lcordier  (1000)       48 2020-06-27 19:59:49.000000 recipe_box-0.1.2/recipe_box.egg-info/entry_points.txt
--rw-r--r--   0 lcordier  (1000) lcordier  (1000)       16 2020-06-27 19:59:49.000000 recipe_box-0.1.2/recipe_box.egg-info/requires.txt
--rw-r--r--   0 lcordier  (1000) lcordier  (1000)       11 2020-06-27 19:59:49.000000 recipe_box-0.1.2/recipe_box.egg-info/top_level.txt
--rwxr-xr-x   0 lcordier  (1000) lcordier  (1000)     5788 2020-06-27 19:52:35.000000 recipe_box-0.1.2/recipe_box.py
--rw-r--r--   0 lcordier  (1000) lcordier  (1000)       38 2020-06-27 19:59:49.552528 recipe_box-0.1.2/setup.cfg
--rw-rw-r--   0 lcordier  (1000) lcordier  (1000)     1164 2020-06-27 19:59:05.000000 recipe_box-0.1.2/setup.py
+drwxrwxr-x   0 lcordier  (1000) lcordier  (1000)        0 2023-07-01 11:52:58.592652 recipe_box-0.1.3/
+-rw-rw-r--   0 lcordier  (1000) lcordier  (1000)    18149 2023-07-01 11:52:58.592652 recipe_box-0.1.3/PKG-INFO
+-rw-r--r--   0 lcordier  (1000) lcordier  (1000)    14985 2023-07-01 09:49:20.000000 recipe_box-0.1.3/README.md
+drwxrwxr-x   0 lcordier  (1000) lcordier  (1000)        0 2023-07-01 11:52:58.588652 recipe_box-0.1.3/recipe_box.egg-info/
+-rw-r--r--   0 lcordier  (1000) lcordier  (1000)    18149 2023-07-01 11:52:56.000000 recipe_box-0.1.3/recipe_box.egg-info/PKG-INFO
+-rw-r--r--   0 lcordier  (1000) lcordier  (1000)      238 2023-07-01 11:52:56.000000 recipe_box-0.1.3/recipe_box.egg-info/SOURCES.txt
+-rw-r--r--   0 lcordier  (1000) lcordier  (1000)        1 2023-07-01 11:52:56.000000 recipe_box-0.1.3/recipe_box.egg-info/dependency_links.txt
+-rw-r--r--   0 lcordier  (1000) lcordier  (1000)       48 2023-07-01 11:52:56.000000 recipe_box-0.1.3/recipe_box.egg-info/entry_points.txt
+-rw-r--r--   0 lcordier  (1000) lcordier  (1000)       16 2023-07-01 11:52:56.000000 recipe_box-0.1.3/recipe_box.egg-info/requires.txt
+-rw-r--r--   0 lcordier  (1000) lcordier  (1000)       11 2023-07-01 11:52:56.000000 recipe_box-0.1.3/recipe_box.egg-info/top_level.txt
+-rwxr-xr-x   0 lcordier  (1000) lcordier  (1000)     6587 2023-07-01 11:43:00.000000 recipe_box-0.1.3/recipe_box.py
+-rw-rw-r--   0 lcordier  (1000) lcordier  (1000)       38 2023-07-01 11:52:58.592652 recipe_box-0.1.3/setup.cfg
+-rw-rw-r--   0 lcordier  (1000) lcordier  (1000)     1164 2023-07-01 11:51:43.000000 recipe_box-0.1.3/setup.py
```

### Comparing `recipe_box-0.1.2/recipe_box.py` & `recipe_box-0.1.3/recipe_box.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,20 +3,26 @@
 """ Scrape a recipe, convert it to Markdown and store it in a Zettelkasten.
 
     A free recipe-box.
 
     1. https://obsidian.md/
     2. https://www.ourstate.com/a-kitchens-riches/
 """
+import argparse
 import json
-import optparse
 import os
-import requests
 import sys
 
+try:
+    import httpx
+    url_getter = httpx.Client(http2=True)
+except ImportError:
+    import requests
+    url_getter = requests
+
 from recipe_scrapers import scrape_me, WebsiteNotImplementedError, SCRAPERS
 
 
 ROOT = '~/.config/recipe_box/'
 
 
 def ensure_directory_exists(path, expand_user=True, file=False):
@@ -35,15 +41,15 @@
     if not os.path.exists(directory) and directory:
         try:
             os.makedirs(directory)
         except OSError as e:
             # A parallel process created the directory after the existence check.
             pass
 
-    return(path)
+    return path
 
 
 def valid_filename(directory, filename=None, ascii=False):
     """ Return a valid "new" filename in a directory, given a filename/directory=path to test.
 
         Deal with duplicate filenames.
     """
@@ -62,109 +68,127 @@
 
     # if ascii:
     #     filename = unidecode(unicode(filename))
     #     filename = ' '.join(filename.splitlines()).strip()
     #     filename = filename.decode('ascii', 'ignore')
 
     # Allow for directories.
-    items = {item: True for item in os.listdir(directory)}
+    items = set(os.listdir(directory))
     if filename in items:
         count = 1
         while test_filename(filename, count) in items:
             count += 1
         if return_path:
             return os.path.join(directory, test_filename(filename, count))
         return test_filename(filename, count)
     else:
         if return_path:
             return os.path.join(directory, filename)
         return filename
 
 
-def main():
-    """ Console script entry point.
+def process_recipe(config, scraper, url, verbose=False):
+    """ Process the recipe at a given URL.
     """
-    parser = optparse.OptionParser('%prog url')
+    recipe_box = ensure_directory_exists(config['recipe_box'])
+    media = ensure_directory_exists(os.path.join(config['recipe_box'], 'media'))
+
+    prefix = scraper.title().lower()
+    path = os.path.join(recipe_box, prefix + '.md')
+    path = valid_filename(path)
+    recipe = open(path, 'w')
+
+    try:
+        image_url = scraper.image()
+        response = url_getter.get(image_url)
+    except:
+        filename = None
+    else:
+        # Not sure about image urls without filename extensions, might need python-magic.
+        # Also, os.path.splitext(url), probably not a good idea. ;)
+        filename = os.path.splitext(os.path.basename(path))[0] + os.path.splitext(scraper.image())[1]
+        filepath = os.path.join(media, filename)
+        image = open(filepath, 'wb')
+        image.write(response.content)
+        image.close()
+        if verbose:
+            print('Saving {url} -> {path}'.format(url=image_url, path=filepath))
+
+    recipe.write('# {title}\n'.format(title=scraper.title()))
+    if filename:
+        recipe.write('![[{filename}]]\n'.format(filename=filename))
+    recipe.write('\n')
+    # This is a placeholder for the user's own notes about the recipe.
+    recipe.write('## Notes\n')
+    recipe.write('\n')
+    recipe.write('## Metadata\n')
+    recipe.write('Yields: {yields}\n'.format(yields=scraper.yields()))
+    recipe.write('Total Time: {total_time}\n'.format(total_time=scraper.total_time()))
+    recipe.write('\n')
+    recipe.write('## Ingredients\n')
+    for ingredient in scraper.ingredients():
+        recipe.write('* {ingredient}\n'.format(ingredient=ingredient))
+
+    recipe.write('\n')
+    recipe.write('## Instructions\n')
+    for instruction in scraper.instructions().split('\n'):
+        instruction = instruction.strip()
+        if instruction:
+            if instruction[0].isdigit():
+                recipe.write('{instruction}\n'.format(instruction=instruction))
+            else:
+                recipe.write('1. {instruction}\n'.format(instruction=instruction))
 
-    parser.add_option('-l',
-                      dest='list',
-                      action='store_true',
-                      default=False,
-                      help='list all available sites')
+    recipe.write('\n')
+    recipe.write('[{url}]({url})\n'.format(url=url))
+    recipe.close()
+    # if verbose:
+    print('Saving {url} -> {path}'.format(url=url, path=path))
 
-    options, args = parser.parse_args()
 
-    if options.list:
+def main():
+    """ Console script entry point.
+    """
+    parser = argparse.ArgumentParser()
+    parser.add_argument('url', metavar='URL', type=str, nargs='*', default='', help='recipe url')
+    parser.add_argument('-l', dest='list', action='store_true', default=False, help='list all available sites')
+    parser.add_argument('-w', dest='wild_mode', action='store_true', default=False, help="try scraping 'unknown' site using wild-mode (some editing of the recipe might be required)")
+    parser.add_argument('-v', dest='verbose', action='store_true', default=False, help='verbose output')
+    args = parser.parse_args()
+
+    if args.list:
         for host in sorted(SCRAPERS):
             print(host)
         sys.exit()
 
+    wild_mode = args.wild_mode
+    verbose = args.verbose
+
     config_path = ensure_directory_exists(os.path.join(ROOT, 'recipe_box.json'), file=True)
     if not os.path.exists(config_path):
         config = {'recipe_box': '~/recipe_box/'}
         with open(config_path, 'w') as f:
             json.dump(config, f, indent=4)
     else:
         with open(config_path, 'r') as f:
             config = json.load(f)
 
-    for url in args:
-        try:
-            scraper = scrape_me(url)
-        except WebsiteNotImplementedError:
-            print('No scraper defined for {url}'.format(url=url))
-            print('It is recommended you add it to recipe-scrapers site, that way everybody gains from the effort.')
-            print('https://github.com/hhursev/recipe-scrapers#if-you-want-a-scraper-for-a-new-site-added')
-            print('')
-            print('Once someone has added the new scraper:')
-            print('pip install --upgrade recipe-scrapers')
-        else:
-            recipe_box = ensure_directory_exists(config['recipe_box'])
-            media = ensure_directory_exists(os.path.join(config['recipe_box'], 'media'))
-
-            prefix = scraper.title().lower()
-            path = os.path.join(recipe_box, prefix + '.md')
-            path = valid_filename(path)
-            recipe = open(path, 'w')
-
+    for url in args.url:
+        if url:
             try:
-                response = requests.get(scraper.image())
-            except:
-                filename = None
+                scraper = scrape_me(url, wild_mode=wild_mode)
+            except WebsiteNotImplementedError:
+                print('No scraper defined for {url}'.format(url=url))
+                print('Try using the -w [wild-mode] option, your mileage may vary.')
+                print('')
+                print('It is recommended you add it to recipe-scrapers site, that way everybody gains from the effort.')
+                print('https://github.com/hhursev/recipe-scrapers#if-you-want-a-scraper-for-a-new-site-added')
+                print('')
+                print('Once someone has added the new scraper:')
+                print('pip install --upgrade recipe-scrapers')
             else:
-                # Not sure about image urls without filename extensions, might need python-magic.
-                # Also, os.path.splitext(url), probably not a good idea. ;)
-                filename = os.path.splitext(os.path.basename(path))[0] + os.path.splitext(scraper.image())[1]
-                image = open(os.path.join(media, filename), 'wb')
-                image.write(response.content)
-                image.close()
-
-            recipe.write('# {title}\n'.format(title=scraper.title()))
-            if filename:
-                recipe.write('![[{filename}]]\n'.format(filename=filename))
-            recipe.write('\n')
-            recipe.write('## Notes\n')
-            recipe.write('\n')
-            recipe.write('## Metadata\n')
-            recipe.write('Yields: {yields}\n'.format(yields=scraper.yields()))
-            recipe.write('Total Time: {total_time}\n'.format(total_time=scraper.total_time()))
-            recipe.write('\n')
-            recipe.write('## Ingredients\n')
-            for ingredient in scraper.ingredients():
-                recipe.write('* {ingredient}\n'.format(ingredient=ingredient))
-
-            recipe.write('\n')
-            recipe.write('## Instructions\n')
-            for instruction in scraper.instructions().split('\n'):
-                instruction = instruction.strip()
-                if instruction:
-                    if instruction[0].isdigit():
-                        recipe.write('{instruction}\n'.format(instruction=instruction))
-                    else:
-                        recipe.write('1. {instruction}\n'.format(instruction=instruction))
-
-            recipe.write('\n')
-            recipe.write('[{url}]({url})\n'.format(url=url))
+                process_recipe(config, scraper, url, verbose)
 
 
 if __name__ == '__main__':
     main()
+
```

### Comparing `recipe_box-0.1.2/setup.py` & `recipe_box-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(
     name='recipe_box',
-    version='0.1.2',
+    version='0.1.3',
     py_modules=['recipe_box'],
     description='Utility to scrape recipes and put it in a local Zettelkasten.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     # https://pypi.org/classifiers/
     classifiers=[
         'Development Status :: 4 - Beta',
```

