# Comparing `tmp/wasc-0.1.1.tar.gz` & `tmp/wasc-0.1.2.tar.gz`

## Comparing `wasc-0.1.1.tar` & `wasc-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,23 @@
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 wasc-0.1.1/data/criteria.yml
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 wasc-0.1.1/data/design.csv
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 wasc-0.1.1/data/example_websites.csv
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 wasc-0.1.1/src/wasc/__about__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 wasc-0.1.1/src/wasc/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 wasc-0.1.1/src/wasc/__main__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 wasc-0.1.1/src/wasc/abstract_checker.py
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 wasc-0.1.1/src/wasc/checker_factory.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 wasc-0.1.1/src/wasc/criterion.py
--rw-r--r--   0        0        0    15976 2020-02-02 00:00:00.000000 wasc-0.1.1/src/wasc/default_checkers.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 wasc-0.1.1/src/wasc/report.py
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 wasc-0.1.1/src/wasc/utils.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 wasc-0.1.1/src/wasc/cli/__init__.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 wasc-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 wasc-0.1.1/.gitignore
--rw-r--r--   0        0        0    21439 2020-02-02 00:00:00.000000 wasc-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 wasc-0.1.1/README.md
--rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 wasc-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 wasc-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 wasc-0.1.2/data/agro_alim.csv
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 wasc-0.1.2/data/criteria.yml
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 wasc-0.1.2/data/example_websites.csv
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 wasc-0.1.2/src/wasc/__about__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 wasc-0.1.2/src/wasc/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 wasc-0.1.2/src/wasc/__main__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 wasc-0.1.2/src/wasc/abstract_checker.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 wasc-0.1.2/src/wasc/checker_factory.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 wasc-0.1.2/src/wasc/criterion.py
+-rw-r--r--   0        0        0    15835 2020-02-02 00:00:00.000000 wasc-0.1.2/src/wasc/default_checkers.py
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 wasc-0.1.2/src/wasc/report.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 wasc-0.1.2/src/wasc/utils.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 wasc-0.1.2/src/wasc/cli/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 wasc-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     7936 2020-02-02 00:00:00.000000 wasc-0.1.2/tests/test_checker.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 wasc-0.1.2/tests/test_utils.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 wasc-0.1.2/tests/data/crit_example.yml
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 wasc-0.1.2/tests/data/url_example.csv
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wasc-0.1.2/.gitignore
+-rw-r--r--   0        0        0    21439 2020-02-02 00:00:00.000000 wasc-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 wasc-0.1.2/README.md
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 wasc-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 wasc-0.1.2/PKG-INFO
```

### Comparing `wasc-0.1.1/src/wasc/abstract_checker.py` & `wasc-0.1.2/src/wasc/abstract_checker.py`

 * *Files identical despite different names*

### Comparing `wasc-0.1.1/src/wasc/checker_factory.py` & `wasc-0.1.2/src/wasc/checker_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         Returns
         -------
         The checker object corresponding to the checker name
         """
         return self.__checker_dict[checker_name]()
 
 checker_factory = CheckerFactory()
-checker_factory.register("FLBT01", dft.FLBT01)
-checker_factory.register("FLBT02", dft.FLBT02)
-checker_factory.register("FLBT03", dft.FLBT03)
-checker_factory.register("FLBT04", dft.FLBT04)
-checker_factory.register("FLBT05", dft.FLBT05)
-checker_factory.register("FLBT06", dft.FLBT06)
-checker_factory.register("FLBT07", dft.FLBT07)
+checker_factory.register("DFTT01", dft.DFTT01)
+checker_factory.register("DFTT02", dft.DFTT02)
+checker_factory.register("DFTT05", dft.DFTT05)
+checker_factory.register("LangChecker", dft.LangChecker)
+checker_factory.register("DoctypeChecker", dft.DoctypeChecker)
+checker_factory.register("AccessChecker", dft.AccessChecker)
+checker_factory.register("AccessLinkChecker", dft.AccessLinkChecker)
+checker_factory.register("MentionsLegalesChecker", dft.MentionsLegalesChecker)
```

### Comparing `wasc-0.1.1/src/wasc/criterion.py` & `wasc-0.1.2/src/wasc/criterion.py`

 * *Files identical despite different names*

### Comparing `wasc-0.1.1/src/wasc/report.py` & `wasc-0.1.2/src/wasc/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,18 @@
             The dictionary containing the test results for each criterion and
             each URL
         """
         header = {
             "user-agent" : "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/56.0.2924.76 Safari/537.36" ,
             "referer" : "https://www.google.com/"
             }
-        response = requests.get(self.url, headers=header, timeout = 1)
+        try:
+            response = requests.get(self.url, headers=header, timeout = 1)
+        except requests.exceptions.ReadTimeout:
+            return {"TimeOut" : self.url}
         if response.status_code == requests.codes.ok :
             self.__bs_obj = bs4.BeautifulSoup(response.content, "html.parser")
         else:
             return {"bad response" : response.status_code}
         result = {}
         if self.__bs_obj:
             for crit in self.__criteria :
```

### Comparing `wasc-0.1.1/src/wasc/cli/__init__.py` & `wasc-0.1.2/src/wasc/cli/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # SPDX-FileCopyrightText: 2023-present Guillaume Collet <bilouweb@free.fr>
 #
 # SPDX-License-Identifier: CECILL-2.1
 import json
 import sys
 
 import click
+from tqdm import tqdm
 
 from wasc.__about__ import __version__
 from wasc.criterion import Criterion
 from wasc.report import Report
 from wasc.utils import read_criteria_config, read_websites
 
 CONTEXT_SETTINGS = {"help_option_names": ["-h", "--help"]}
-DEFAULT_CRIT_DICT = { "Balise head" : ["FLBT01", "FLBT02"]}
+DEFAULT_CRIT_DICT = { "Accessibilité" : ["AccessChecker", "AccessLinkChecker"], "Mentions légales" : ["MentionsLegalesChecker"]}
 
 @click.command(context_settings=CONTEXT_SETTINGS)
-@click.argument("websites", type=click.File("r"))
+@click.argument("websites", type=click.Path(exists=True))
 @click.option("-c", "--criteria", type=click.Path(exists=True),
               help="Criteria configuration file (yaml)")
 @click.option("-o", "--output", default=sys.stdout,
               type=click.File("w"),
               help="Output file [default=stdout]")
 @click.option("-f", "--output_format", default = "json",
               type=click.Choice(["json", "csv"], case_sensitive=False),
@@ -38,9 +39,12 @@
         click.echo(f"Read criteria from {criteria}")
         crit_dict = read_criteria_config(criteria)
     else :
         click.echo("Use default criteria")
     crit_list = [Criterion(crit, checkers) for crit, checkers in crit_dict.items()]
     websites = read_websites(websites)
     click.echo(f"Analysis of {len(websites)} websites...")
-    report = {label : Report(label, url, crit_list).execute() for label, url in websites}
+    report = {}
+    for i in tqdm(range(len(websites))):
+        label, url = websites[i]
+        report[label] = Report(label, url, crit_list).execute()
     click.echo(json.dumps(report, sort_keys=True, indent=4, ensure_ascii=False), file=output)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wasc-0.1.1/LICENSE.txt` & `wasc-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wasc-0.1.1/pyproject.toml` & `wasc-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -56,23 +56,30 @@
 WASC_CRITERIA_DEFAULT_PATH = "./data/default_criteria.yml"
 
 [tool.hatch.envs.build.env-vars]
 WACS_CRITERIA_DEFAULT_PATH = "./data/default_criteria.yml"
 
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
+all_test = "pytest tests/__init__.py"
 test-cov = "coverage run -m pytest {args:tests}"
+lcov = "coverage lcov"
 cov-report = [
   "- coverage combine",
   "coverage report",
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
+all_cov = [
+  "test-cov tests/__init__.py",
+  "cov-report",
+  "lcov",
+]
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
```

### Comparing `wasc-0.1.1/PKG-INFO` & `wasc-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasc
-Version: 0.1.1
+Version: 0.1.2
 Summary: wasc, for Web Accessibility Simple Checker, helps to evaluate accessibility criteria on a list of websites
 Project-URL: Documentation, https://github.com/gcollet/wasc#readme
 Project-URL: Issues, https://github.com/gcollet/wasc/issues
 Project-URL: Source, https://github.com/gcollet/wasc
 Author-email: Guillaume Collet <bilouweb@free.fr>, Juliette Francis <juliette.francis@etudiant.univ-rennes.fr>
 License-Expression: CECILL-2.1
 License-File: LICENSE.txt
```

