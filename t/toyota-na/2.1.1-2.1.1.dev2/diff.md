# Comparing `tmp/toyota-na-2.1.1.tar.gz` & `tmp/toyota-na-2.1.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toyota-na-2.1.1.tar", max compression
+gzip compressed data, was "toyota-na-2.1.1.dev2.tar", max compression
```

## Comparing `toyota-na-2.1.1.tar` & `toyota-na-2.1.1.dev2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1069 2022-05-01 23:05:47.262883 toyota-na-2.1.1/LICENSE
--rw-r--r--   0        0        0     2262 2022-05-01 23:05:47.262883 toyota-na-2.1.1/README.md
--rw-r--r--   0        0        0     1439 2022-05-01 23:06:21.327455 toyota-na-2.1.1/pyproject.toml
--rw-r--r--   0        0        0       68 2022-05-01 23:05:47.262883 toyota-na-2.1.1/toyota_na/__init__.py
--rw-r--r--   0        0        0     4134 2022-05-01 23:05:47.262883 toyota-na-2.1.1/toyota_na/app.py
--rw-r--r--   0        0        0     7626 2022-05-01 23:05:47.262883 toyota-na-2.1.1/toyota_na/auth.py
--rw-r--r--   0        0        0     7750 2022-05-01 23:05:47.262883 toyota-na-2.1.1/toyota_na/client.py
--rw-r--r--   0        0        0      160 2022-05-01 23:05:47.262883 toyota-na-2.1.1/toyota_na/exceptions.py
--rw-r--r--   0        0        0        0 2022-05-01 23:05:47.262883 toyota-na-2.1.1/toyota_na/vehicle/__init__.py
--rw-r--r--   0        0        0     4423 2022-05-01 23:05:47.262883 toyota-na-2.1.1/toyota_na/vehicle/base_vehicle.py
--rw-r--r--   0        0        0      579 2022-05-01 23:05:47.262883 toyota-na-2.1.1/toyota_na/vehicle/entity_types/ToyotaLocation.py
--rw-r--r--   0        0        0      538 2022-05-01 23:05:47.262883 toyota-na-2.1.1/toyota_na/vehicle/entity_types/ToyotaLockableOpening.py
--rw-r--r--   0        0        0      571 2022-05-01 23:05:47.266883 toyota-na-2.1.1/toyota_na/vehicle/entity_types/ToyotaNumeric.py
--rw-r--r--   0        0        0      350 2022-05-01 23:05:47.266883 toyota-na-2.1.1/toyota_na/vehicle/entity_types/ToyotaOpening.py
--rw-r--r--   0        0        0     2142 2022-05-01 23:05:47.266883 toyota-na-2.1.1/toyota_na/vehicle/entity_types/ToyotaRemoteStart.py
--rw-r--r--   0        0        0        0 2022-05-01 23:05:47.266883 toyota-na-2.1.1/toyota_na/vehicle/entity_types/__init__.py
--rw-r--r--   0        0        0     1627 2022-05-01 23:05:47.266883 toyota-na-2.1.1/toyota_na/vehicle/vehicle.py
--rw-r--r--   0        0        0        0 2022-05-01 23:05:47.266883 toyota-na-2.1.1/toyota_na/vehicle/vehicle_generations/__init__.py
--rw-r--r--   0        0        0     7356 2022-05-01 23:05:47.266883 toyota-na-2.1.1/toyota_na/vehicle/vehicle_generations/seventeen_cy.py
--rw-r--r--   0        0        0     6859 2022-05-01 23:05:47.266883 toyota-na-2.1.1/toyota_na/vehicle/vehicle_generations/seventeen_cy_plus.py
--rw-r--r--   0        0        0     3103 2022-05-01 23:06:21.405820 toyota-na-2.1.1/setup.py
--rw-r--r--   0        0        0     2887 2022-05-01 23:06:21.406221 toyota-na-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-05-01 22:51:57.815857 toyota-na-2.1.1.dev2/LICENSE
+-rw-r--r--   0        0        0     2262 2022-05-01 22:51:57.815857 toyota-na-2.1.1.dev2/README.md
+-rw-r--r--   0        0        0     1444 2022-05-01 22:52:33.448127 toyota-na-2.1.1.dev2/pyproject.toml
+-rw-r--r--   0        0        0       68 2022-05-01 22:51:57.819857 toyota-na-2.1.1.dev2/toyota_na/__init__.py
+-rw-r--r--   0        0        0     4134 2022-05-01 22:51:57.819857 toyota-na-2.1.1.dev2/toyota_na/app.py
+-rw-r--r--   0        0        0     7626 2022-05-01 22:51:57.819857 toyota-na-2.1.1.dev2/toyota_na/auth.py
+-rw-r--r--   0        0        0     7750 2022-05-01 22:51:57.819857 toyota-na-2.1.1.dev2/toyota_na/client.py
+-rw-r--r--   0        0        0      160 2022-05-01 22:51:57.819857 toyota-na-2.1.1.dev2/toyota_na/exceptions.py
+-rw-r--r--   0        0        0        0 2022-05-01 22:51:57.819857 toyota-na-2.1.1.dev2/toyota_na/vehicle/__init__.py
+-rw-r--r--   0        0        0     4423 2022-05-01 22:51:57.819857 toyota-na-2.1.1.dev2/toyota_na/vehicle/base_vehicle.py
+-rw-r--r--   0        0        0      579 2022-05-01 22:51:57.819857 toyota-na-2.1.1.dev2/toyota_na/vehicle/entity_types/ToyotaLocation.py
+-rw-r--r--   0        0        0      538 2022-05-01 22:51:57.819857 toyota-na-2.1.1.dev2/toyota_na/vehicle/entity_types/ToyotaLockableOpening.py
+-rw-r--r--   0        0        0      571 2022-05-01 22:51:57.819857 toyota-na-2.1.1.dev2/toyota_na/vehicle/entity_types/ToyotaNumeric.py
+-rw-r--r--   0        0        0      350 2022-05-01 22:51:57.819857 toyota-na-2.1.1.dev2/toyota_na/vehicle/entity_types/ToyotaOpening.py
+-rw-r--r--   0        0        0     2142 2022-05-01 22:51:57.819857 toyota-na-2.1.1.dev2/toyota_na/vehicle/entity_types/ToyotaRemoteStart.py
+-rw-r--r--   0        0        0        0 2022-05-01 22:51:57.819857 toyota-na-2.1.1.dev2/toyota_na/vehicle/entity_types/__init__.py
+-rw-r--r--   0        0        0     1627 2022-05-01 22:51:57.819857 toyota-na-2.1.1.dev2/toyota_na/vehicle/vehicle.py
+-rw-r--r--   0        0        0        0 2022-05-01 22:51:57.819857 toyota-na-2.1.1.dev2/toyota_na/vehicle/vehicle_generations/__init__.py
+-rw-r--r--   0        0        0     7356 2022-05-01 22:51:57.819857 toyota-na-2.1.1.dev2/toyota_na/vehicle/vehicle_generations/seventeen_cy.py
+-rw-r--r--   0        0        0     6859 2022-05-01 22:51:57.819857 toyota-na-2.1.1.dev2/toyota_na/vehicle/vehicle_generations/seventeen_cy_plus.py
+-rw-r--r--   0        0        0     3108 2022-05-01 22:52:33.541978 toyota-na-2.1.1.dev2/setup.py
+-rw-r--r--   0        0        0     2892 2022-05-01 22:52:33.542436 toyota-na-2.1.1.dev2/PKG-INFO
```

### Comparing `toyota-na-2.1.1/LICENSE` & `toyota-na-2.1.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `toyota-na-2.1.1/README.md` & `toyota-na-2.1.1.dev2/README.md`

 * *Files identical despite different names*

### Comparing `toyota-na-2.1.1/pyproject.toml` & `toyota-na-2.1.1.dev2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 description = "Python client for Toyota North America service API"
 license = "MIT"
 name = "toyota-na"
 readme = "README.md"
-version = "2.1.1"
+version = "2.1.1.dev2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
```

### Comparing `toyota-na-2.1.1/toyota_na/app.py` & `toyota-na-2.1.1.dev2/toyota_na/app.py`

 * *Files identical despite different names*

### Comparing `toyota-na-2.1.1/toyota_na/auth.py` & `toyota-na-2.1.1.dev2/toyota_na/auth.py`

 * *Files identical despite different names*

### Comparing `toyota-na-2.1.1/toyota_na/client.py` & `toyota-na-2.1.1.dev2/toyota_na/client.py`

 * *Files identical despite different names*

### Comparing `toyota-na-2.1.1/toyota_na/vehicle/base_vehicle.py` & `toyota-na-2.1.1.dev2/toyota_na/vehicle/base_vehicle.py`

 * *Files identical despite different names*

### Comparing `toyota-na-2.1.1/toyota_na/vehicle/entity_types/ToyotaLocation.py` & `toyota-na-2.1.1.dev2/toyota_na/vehicle/entity_types/ToyotaLocation.py`

 * *Files identical despite different names*

### Comparing `toyota-na-2.1.1/toyota_na/vehicle/entity_types/ToyotaLockableOpening.py` & `toyota-na-2.1.1.dev2/toyota_na/vehicle/entity_types/ToyotaLockableOpening.py`

 * *Files identical despite different names*

### Comparing `toyota-na-2.1.1/toyota_na/vehicle/entity_types/ToyotaNumeric.py` & `toyota-na-2.1.1.dev2/toyota_na/vehicle/entity_types/ToyotaNumeric.py`

 * *Files identical despite different names*

### Comparing `toyota-na-2.1.1/toyota_na/vehicle/entity_types/ToyotaRemoteStart.py` & `toyota-na-2.1.1.dev2/toyota_na/vehicle/entity_types/ToyotaRemoteStart.py`

 * *Files identical despite different names*

### Comparing `toyota-na-2.1.1/toyota_na/vehicle/vehicle.py` & `toyota-na-2.1.1.dev2/toyota_na/vehicle/vehicle.py`

 * *Files identical despite different names*

### Comparing `toyota-na-2.1.1/toyota_na/vehicle/vehicle_generations/seventeen_cy.py` & `toyota-na-2.1.1.dev2/toyota_na/vehicle/vehicle_generations/seventeen_cy.py`

 * *Files identical despite different names*

### Comparing `toyota-na-2.1.1/toyota_na/vehicle/vehicle_generations/seventeen_cy_plus.py` & `toyota-na-2.1.1.dev2/toyota_na/vehicle/vehicle_generations/seventeen_cy_plus.py`

 * *Files identical despite different names*

### Comparing `toyota-na-2.1.1/setup.py` & `toyota-na-2.1.1.dev2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['PyJWT>=2.1.0', 'aiohttp>=3.8.1', 'cryptography>=35.0.0', 'pytz>=2022.1']
 
 setup_kwargs = {
     'name': 'toyota-na',
-    'version': '2.1.1',
+    'version': '2.1.1.dev2',
     'description': 'Python client for Toyota North America service API',
     'long_description': '# toyota-na\n![PyPI](https://img.shields.io/pypi/v/toyota-na?style=flat-square) ![Codecov branch](https://img.shields.io/codecov/c/github/toyotha/toyota-na/main?style=flat-square) ![PyPI - Downloads](https://img.shields.io/pypi/dm/toyota-na?style=flat-square)\n\nPython client for Toyota North America service API\n\n## Install\n```\npip install toyota-na\n```\n## Usage\n```\npython -m toyota_na.app -h  # Get help\npython -m toyota_na.app authorize <username> <passworde>\npython -m toyota_na.app get_user_vehicle_list  # List vehicle\npython -m toyota_na.app get_vehicle_status <vin>  # Get vehcicle status\n...\n```\n\n## Known Issues\n1. Door/window status not always up-to-date unless you call `send_refresh_status` first and wait for it to complete (there is no notification that it completed successfully).\n\n## Developer Guide\n### Quick Start\n```\nfrom toyota_na.client import ToyotaOneClient\n\nasync def main():\n    cli = ToyotaOneClient()\n    await cli.auth.login(USERNAME, PASSWORD)\n    vehicle_list = await cli.get_user_vehicle_list()\n    vehicle_status = await cli.get_vehicle_status(vehicle_list[0]["vin"])\n    ...\n```\n\n### Abstracted Interface Example\n```\nfrom toyota_na.client import ToyotaOneClient\nfrom toyota_na.vehicle.vehicle import get_vehicles\n\nasync def main():\n    cli = ToyotaOneClient()\n```\n\n### Contributing\nWe use black and isort for opinionated formatting to ensure a consistent look and feel throughout the codebase no matter the contributor.\nPre-commit is used to guarantee the files being checked-in to the repo are formatted correctly.\n\nFor convenience a vscode project settings file is included as well. Editors other than vscode will require some setup if you wish to have formatting take place while working.\n\nGetting started:\n- Install poetry - https://python-poetry.org/docs/#osx--linux--bashonwindows-install-instructions\n- Clone the repo\n- `poetry install`\n- `poetry shell`\n- `pre-commit install`\n\n### Samples\nSample responses from API calls are stored in `samples` folder. The data is sourced from real users and from the Toyota app\'s "Demo Mode"\n\n## Credits:\nThanks @DurgNomis-drol for making the original Toyota module and bring up the discussing of Toyota North America.\n\nThanks @visualage for finding the way to authenticate headlessly.\n',
     'author': 'Gavin Ni',
     'author_email': 'gisngy@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `toyota-na-2.1.1/PKG-INFO` & `toyota-na-2.1.1.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toyota-na
-Version: 2.1.1
+Version: 2.1.1.dev2
 Summary: Python client for Toyota North America service API
 License: MIT
 Author: Gavin Ni
 Author-email: gisngy@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

