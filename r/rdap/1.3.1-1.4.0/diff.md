# Comparing `tmp/rdap-1.3.1.tar.gz` & `tmp/rdap-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdap-1.3.1.tar", max compression
+gzip compressed data, was "rdap-1.4.0.tar", max compression
```

## Comparing `rdap-1.3.1.tar` & `rdap-1.4.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    11358 2022-07-07 09:06:14.294185 rdap-1.3.1/LICENSE
--rw-r--r--   0        0        0     3146 2022-07-07 09:06:14.294185 rdap-1.3.1/README.md
--rw-r--r--   0        0        0     1454 2022-10-10 13:18:57.158308 rdap-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      309 2022-07-07 09:06:14.294185 rdap-1.3.1/rdap/__init__.py
--rw-r--r--   0        0        0     3984 2022-10-10 13:18:51.134947 rdap-1.3.1/rdap/assignment.py
--rw-r--r--   0        0        0     1872 2022-07-07 09:06:14.294185 rdap-1.3.1/rdap/bootstrap.py
--rw-r--r--   0        0        0     2250 2022-07-07 09:06:14.294185 rdap-1.3.1/rdap/cli.py
--rw-r--r--   0        0        0     9653 2022-07-07 09:06:14.294185 rdap-1.3.1/rdap/client.py
--rw-r--r--   0        0        0      746 2022-07-07 09:06:14.294185 rdap-1.3.1/rdap/config.py
--rw-r--r--   0        0        0      237 2022-07-07 09:06:14.294185 rdap-1.3.1/rdap/exceptions.py
--rw-r--r--   0        0        0     5299 2022-07-07 09:06:14.294185 rdap-1.3.1/rdap/objects.py
--rw-r--r--   0        0        0     4043 2022-10-10 13:19:29.916181 rdap-1.3.1/setup.py
--rw-r--r--   0        0        0     4074 2022-10-10 13:19:29.917244 rdap-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2020-10-30 16:40:23.636777 rdap-1.4.0/LICENSE
+-rw-r--r--   0        0        0     3025 2023-06-30 22:46:20.453257 rdap-1.4.0/README.md
+-rw-r--r--   0        0        0     1381 2023-06-30 22:51:13.194666 rdap-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      309 2021-01-13 02:09:22.693448 rdap-1.4.0/rdap/__init__.py
+-rw-r--r--   0        0        0     3978 2023-06-30 22:24:27.233315 rdap-1.4.0/rdap/assignment.py
+-rw-r--r--   0        0        0     1872 2021-01-13 18:02:14.687255 rdap-1.4.0/rdap/bootstrap.py
+-rw-r--r--   0        0        0     2250 2022-09-23 17:55:38.098616 rdap-1.4.0/rdap/cli.py
+-rw-r--r--   0        0        0    10225 2023-06-30 22:46:20.449257 rdap-1.4.0/rdap/client.py
+-rw-r--r--   0        0        0      746 2021-01-13 18:02:14.688254 rdap-1.4.0/rdap/config.py
+-rw-r--r--   0        0        0      237 2020-10-30 16:40:23.637777 rdap-1.4.0/rdap/exceptions.py
+-rw-r--r--   0        0        0     5323 2023-06-30 22:46:20.449257 rdap-1.4.0/rdap/objects.py
+-rw-r--r--   0        0        0     3944 1970-01-01 00:00:00.000000 rdap-1.4.0/PKG-INFO
```

### Comparing `rdap-1.3.1/LICENSE` & `rdap-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rdap-1.3.1/README.md` & `rdap-1.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 
 # rdap
 
 [![PyPI](https://img.shields.io/pypi/v/rdap.svg?maxAge=3600)](https://pypi.python.org/pypi/rdap)
 [![PyPI](https://img.shields.io/pypi/pyversions/rdap.svg?maxAge=3600)](https://pypi.python.org/pypi/rdap)
-[![Tests](https://github.com/20c/rdap/workflows/tests/badge.svg)](https://github.com/20c/rdap)
+[![tests](https://github.com/20c/rdap/actions/workflows/tests.yml/badge.svg)](https://github.com/20c/rdap/actions/workflows/tests.yml)
 [![Codecov](https://img.shields.io/codecov/c/github/20c/rdap/master.svg?maxAge=3600)](https://codecov.io/github/20c/rdap)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/20c/rdap.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/20c/rdap/context:python)
 
 
 Registration Data Access Protocol tools
 
 ## Installation
 
 ```sh
@@ -71,15 +70,15 @@
   # HTTP request timeout in seconds, used for both connect and read
   timeout: 0.5
 ```
 
 
 ### License
 
-Copyright 2016-2022 20C, LLC
+Copyright 2016-2023 20C, LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this softare except in compliance with the License.
 You may obtain a copy of the License at
 
    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rdap-1.3.1/pyproject.toml` & `rdap-1.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,63 @@
 [tool.poetry]
 name = "rdap"
-version = "1.3.1"
+version = "1.4.0"
 description = "Registration Data Access Protocol tools"
 authors = ["20C <code@20c.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 
 repository = "https://github.com/20c/rdap"
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Internet",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
 ]
 
 
 [tool.poetry.scripts]
 rdap = "rdap.cli:main"
 
 
 [tool.poetry.dependencies]
-python = "^3.7"
-munge = "^1.0.0"
-requests = "^2.25.1"
+python = "^3.8"
+requests = ">=2.25.1"
+munge = {version = ">=1.3", extras = ["yaml"]}
 
 
 [tool.poetry.dev-dependencies]
 # testing
-codecov = ">=2"
 coverage = ">=5"
 pytest = ">=6"
 pytest-django = ">=3.8"
 pytest-filedata = "^0.4.0"
 pytest-cov = "*"
-tox = "^3.20.1"
+tox = ">=3.20"
 tox-gh-actions = "^2.9.1"
 
 # linting
 black = ">=20"
 isort = ">=5.7"
 flake8 = ">=3.8"
 mypy = ">=0.950"
 pre-commit = ">=2.13"
 pyupgrade = ">=2.19"
 
 # docs
 markdown = "*"
 markdown-include = ">=0.5,<1"
-mkdocs = "^1.2.3"
-
-# ctl
-ctl = ">=1"
-jinja2 = ">=2"
-tmpl = ">=1"
-# v4 released 2022-03-31
-twine = "^3.3.0"
+mkdocs = ">=1.2.3"
 
 [tool.poetry.plugins."markdown.extensions"]
 pymdgen = "pymdgen.md:Extension"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rdap-1.3.1/rdap/assignment.py` & `rdap-1.4.0/rdap/assignment.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
     Files will be downloaded from  https://ftp.ripe.net/pub/stats/{rir}/delegated-{rir}-extended-latest
     """
 
     rir_lists = ["afrinic", "apnic", "arin", "lacnic", "ripencc"]
 
     def parse_data(self, line):
-
         """
         Parses a line from a data file and attempts to return the ASN
         and assignment status
 
         A line can parse multiple asns depending of the value in 5th
         column.
 
@@ -35,29 +34,27 @@
         try:
             if parts[2] != "asn":
                 return
         except IndexError:
             return
 
         try:
-
             asn = parts[3]
             count = int(parts[4])
             status = parts[6].strip()
             asns = None
 
             asns = [{"asn": int(asn) + i, "status": status} for i in range(0, count)]
 
             return asns
 
         except IndexError:
             return
 
     def load_data(self, data_path=".", cache_days=1):
-
         """
         Reads RIR assignment data into memory
 
         This is called autoamtically by `get_status`
 
         This will download assignement status files from ripe if they dont
         exist yet or have expired. Initial call of this function will
@@ -70,26 +67,24 @@
 
         - data_path (`str`): directory path to where downloaded files are to be saved
         - cache_days (`int`): maximum age of downloaded files before they will be
             downloaded again
         """
 
         if not hasattr(self, "_data_files"):
-
             self._data_files = []
 
             for rir in self.rir_lists:
                 rir_file_path = os.path.join(
                     data_path, f"delegated-{rir}-extended-latest"
                 )
                 self.download_data(rir, rir_file_path, cache_days)
                 self._data_files.append(rir_file_path)
 
         if not hasattr(self, "_data"):
-
             self._data = {}
 
             for rir_file_path in self._data_files:
                 print(rir_file_path)
                 with open(rir_file_path) as fh:
                     for line in fh.read().splitlines():
                         asns = self.parse_data(line)
@@ -124,15 +119,14 @@
             )
             response = requests.get(url)
 
             with open(file_path, "w") as file:
                 file.write(response.text)
 
     def get_status(self, asn):
-
         """
         Get RIR assignment status for an ASN
         """
 
         if not hasattr(self, "_data"):
             self.load_data()
```

### Comparing `rdap-1.3.1/rdap/bootstrap.py` & `rdap-1.4.0/rdap/bootstrap.py`

 * *Files identical despite different names*

### Comparing `rdap-1.3.1/rdap/cli.py` & `rdap-1.4.0/rdap/cli.py`

 * *Files identical despite different names*

### Comparing `rdap-1.3.1/rdap/client.py` & `rdap-1.4.0/rdap/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -107,15 +107,16 @@
 
         # use setter
         self._recurse_roles = None
         self.recurse_roles = set(
             config.get("recurse_roles", ["administrative", "technical"])
         )
 
-        self._asn_req = None
+        self._last_req = None
+        self._last_req_url = None
         self._history = []
         self._asn_tree = None
         self.timeout = config.get("timeout")
 
         self.http = requests.Session()
         self.http.auth = RdapRequestAuth(
             **dict(
@@ -267,58 +268,76 @@
         if classname in classes:
             return classes[classname](data, self)
         else:
             raise NotImplementedError(
                 f"Unknown objectClassName '{classname}' from '{url}'"
             )
 
+    def _rdap_get(self, query, base_url=None):
+        """Does an HTTP get for the given url and query.
+        sets _last_req_url for future entity lookups
+        """
+        if not base_url:
+            base_url = self.url
+
+        # FIXME - url join
+        url = f"{base_url}{query}"
+        self._last_req = self._get(url)
+        # split query off to get the base url for following entity lookups
+        self._last_req_url = self._last_req.url.rsplit(query, 1)[0]
+        return self._last_req
+
     def get_asn(self, asn):
         """
         Get an ASN object.
         """
         asn = int(asn)
         try:
-            url = f"{self.asn_url(asn)}/autnum/{asn}"
+            url = self.asn_url(asn)
         # catch bootstrap Lookup errors and report as not found
         except LookupError as excinfo:
             raise RdapNotFoundError(str(excinfo))
 
         # save reqest to get url for following entity lookups
-        self._asn_req = self._get(url)
-        return RdapAsn(self._asn_req.json(), self)
+        query = f"/autnum/{asn}"
+        return RdapAsn(self._rdap_get(query, base_url=url).json(), self)
 
     def get_domain(self, domain):
         """
         Get a domain object.
         """
-        url = f"{self.url}/domain/{domain}"
-        return RdapAsn(self._get(url).json(), self)
+        query = f"/domain/{domain}"
+        return RdapDomain(self._rdap_get(query).json(), self)
 
     def get_ip(self, address):
         """
         Get an IP object.
         """
-        url = f"{self.url}/ip/{address}"
-        return RdapNetwork(self._get(url).json(), self)
+        query = f"/ip/{address}"
+        return RdapNetwork(self._rdap_get(query).json(), self)
 
     def get_entity(self, handle, base_url):
         """
         get entity information in object form
         """
-        url = f"{base_url}/entity/{handle}"
-        return RdapEntity(self._get(url).json(), self)
+        query = f"/entity/{handle}"
+        return RdapEntity(self._rdap_get(query).json(), self)
 
     def get_entity_url(self, handle):
         """
         Get entity url for handle.
 
-        This fucntion must be able to handle doing recursive lookups to the current URL after a bootstrap redirect for registries that don't link 'self'
+        This function must be able to handle doing recursive lookups to the current URL
+        after a bootstrap redirect for registries that don't link 'self'
         """
-        if self._asn_req:
-            url = re.split("/autnum/", self._asn_req.url)[0]
+
+        if self._last_req_url:
+            url = self._last_req_url
+
+        # last ditch effort to use bootstrap
         else:
             url = self.url
 
         url = f"{url}/entity/{handle}"
         return url
 
     def get_data(self, url):
```

### Comparing `rdap-1.3.1/rdap/config.py` & `rdap-1.4.0/rdap/config.py`

 * *Files identical despite different names*

### Comparing `rdap-1.3.1/rdap/objects.py` & `rdap-1.4.0/rdap/objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                 elif typ[0] == "kind":
                     vcard[typ[0]] = typ[3].strip()
                 elif typ[0] == "adr":
                     # WORKAROUND ARIN uses label in the extra field
                     adr = typ[1].get("label", "").strip()
                     if not adr:
                         # rest use the text field
-                        adr = "\n".join(typ[3]).strip()
+                        adr = "\n".join([str(item) for item in typ[3]]).strip()
                     if adr:
                         vcard["adr"] = adr
         return vcard
 
     def _parse_entity_self_link(self, entity):
         for link in entity.get("links", []):
             if link["rel"] == "self":
```

### Comparing `rdap-1.3.1/setup.py` & `rdap-1.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,115 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: rdap
+Version: 1.4.0
+Summary: Registration Data Access Protocol tools
+Home-page: https://github.com/20c/rdap
+License: Apache-2.0
+Author: 20C
+Author-email: code@20c.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: munge[yaml] (>=1.3)
+Requires-Dist: requests (>=2.25.1)
+Project-URL: Repository, https://github.com/20c/rdap
+Description-Content-Type: text/markdown
+
+
+# rdap
+
+[![PyPI](https://img.shields.io/pypi/v/rdap.svg?maxAge=3600)](https://pypi.python.org/pypi/rdap)
+[![PyPI](https://img.shields.io/pypi/pyversions/rdap.svg?maxAge=3600)](https://pypi.python.org/pypi/rdap)
+[![tests](https://github.com/20c/rdap/actions/workflows/tests.yml/badge.svg)](https://github.com/20c/rdap/actions/workflows/tests.yml)
+[![Codecov](https://img.shields.io/codecov/c/github/20c/rdap/master.svg?maxAge=3600)](https://codecov.io/github/20c/rdap)
+
+
+Registration Data Access Protocol tools
+
+## Installation
+
+```sh
+pip install rdap
+```
+
+
+## Usage
+
+```
+usage: rdap [-h] [--debug] [--home HOME] [--verbose] [--quiet] [--version] [--output-format OUTPUT_FORMAT] [--show-requests] [--parse]
+            [--write-bootstrap-data]
+            query [query ...]
+
+rdap
+
+positional arguments:
+  query
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --debug               enable extra debug output
+  --home HOME           specify the home directory, by default will check in order: $RDAP_HOME, ./.rdap, /home/$USER/.rdap,
+                        /home/$USER/.config/rdap
+  --verbose             enable more verbose output
+  --quiet               no output at all
+  --version             show version number and exit
+  --output-format OUTPUT_FORMAT
+                        output format (yaml, json, text)
+  --show-requests       show all requests
+  --parse               parse data into object before display
+  --write-bootstrap-data
+                        write bootstrap data for type (as query)
+```
+
+
+## Config file
+
+The client uses the `--home` option to point to a directory, by default will check in order: `$RDAP_HOME`, `./.rdap`, `~/.rdap`, `~/.config/rdap`
+
+The directory should have a `config.yaml` file in it, defaults shown below.
+
+```yaml
+rdap:
+  # URL to bootstrap the initial request off
+  bootstrap_url: https://rdap.db.ripe.net/
+  # boolean to use data from bootstrap_data_url instead of a bootstrap server
+  self_bootstrap: False
+  # url to load bootstrap data from
+  bootstrap_data_url: "https://data.iana.org/rdap/"
+  # length of time in hours to keep bootstrap data
+  bootstrap_cache_ttl: 25
+  # how to format the output
+  output_format: yaml
+  # API key for use at rdap.lacnic.net
+  lacnic_apikey: None
+  # role types to recursively query when processing
+  recurse_roles: ["administrative", "technical"]
+  # HTTP request timeout in seconds, used for both connect and read
+  timeout: 0.5
+```
+
+
+### License
+
+Copyright 2016-2023 20C, LLC
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this softare except in compliance with the License.
+You may obtain a copy of the License at
+
+   http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
 
-packages = \
-['rdap']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['munge>=1.0.0,<2.0.0', 'requests>=2.25.1,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['rdap = rdap.cli:main'],
- 'markdown.extensions': ['pymdgen = pymdgen.md:Extension']}
-
-setup_kwargs = {
-    'name': 'rdap',
-    'version': '1.3.1',
-    'description': 'Registration Data Access Protocol tools',
-    'long_description': '\n# rdap\n\n[![PyPI](https://img.shields.io/pypi/v/rdap.svg?maxAge=3600)](https://pypi.python.org/pypi/rdap)\n[![PyPI](https://img.shields.io/pypi/pyversions/rdap.svg?maxAge=3600)](https://pypi.python.org/pypi/rdap)\n[![Tests](https://github.com/20c/rdap/workflows/tests/badge.svg)](https://github.com/20c/rdap)\n[![Codecov](https://img.shields.io/codecov/c/github/20c/rdap/master.svg?maxAge=3600)](https://codecov.io/github/20c/rdap)\n[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/20c/rdap.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/20c/rdap/context:python)\n\n\nRegistration Data Access Protocol tools\n\n## Installation\n\n```sh\npip install rdap\n```\n\n\n## Usage\n\n```\nusage: rdap [-h] [--debug] [--home HOME] [--verbose] [--quiet] [--version] [--output-format OUTPUT_FORMAT] [--show-requests] [--parse]\n            [--write-bootstrap-data]\n            query [query ...]\n\nrdap\n\npositional arguments:\n  query\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --debug               enable extra debug output\n  --home HOME           specify the home directory, by default will check in order: $RDAP_HOME, ./.rdap, /home/$USER/.rdap,\n                        /home/$USER/.config/rdap\n  --verbose             enable more verbose output\n  --quiet               no output at all\n  --version             show version number and exit\n  --output-format OUTPUT_FORMAT\n                        output format (yaml, json, text)\n  --show-requests       show all requests\n  --parse               parse data into object before display\n  --write-bootstrap-data\n                        write bootstrap data for type (as query)\n```\n\n\n## Config file\n\nThe client uses the `--home` option to point to a directory, by default will check in order: `$RDAP_HOME`, `./.rdap`, `~/.rdap`, `~/.config/rdap`\n\nThe directory should have a `config.yaml` file in it, defaults shown below.\n\n```yaml\nrdap:\n  # URL to bootstrap the initial request off\n  bootstrap_url: https://rdap.db.ripe.net/\n  # boolean to use data from bootstrap_data_url instead of a bootstrap server\n  self_bootstrap: False\n  # url to load bootstrap data from\n  bootstrap_data_url: "https://data.iana.org/rdap/"\n  # length of time in hours to keep bootstrap data\n  bootstrap_cache_ttl: 25\n  # how to format the output\n  output_format: yaml\n  # API key for use at rdap.lacnic.net\n  lacnic_apikey: None\n  # role types to recursively query when processing\n  recurse_roles: ["administrative", "technical"]\n  # HTTP request timeout in seconds, used for both connect and read\n  timeout: 0.5\n```\n\n\n### License\n\nCopyright 2016-2022 20C, LLC\n\nLicensed under the Apache License, Version 2.0 (the "License");\nyou may not use this softare except in compliance with the License.\nYou may obtain a copy of the License at\n\n   http://www.apache.org/licenses/LICENSE-2.0\n\nUnless required by applicable law or agreed to in writing, software\ndistributed under the License is distributed on an "AS IS" BASIS,\nWITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\nSee the License for the specific language governing permissions and\nlimitations under the License.\n',
-    'author': '20C',
-    'author_email': 'code@20c.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/20c/rdap',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

