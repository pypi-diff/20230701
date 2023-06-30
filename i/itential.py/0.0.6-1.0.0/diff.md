# Comparing `tmp/itential.py-0.0.6.tar.gz` & `tmp/itential.py-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itential.py-0.0.6.tar", last modified: Fri Nov 11 04:36:39 2022, max compression
+gzip compressed data, was "itential.py-1.0.0.tar", last modified: Fri Jun 30 22:45:54 2023, max compression
```

## Comparing `itential.py-0.0.6.tar` & `itential.py-1.0.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxrwxrwx   0        0        0        0 2022-11-11 04:36:39.118023 itential.py-0.0.6/
--rw-rw-rw-   0        0        0     1107 2022-08-18 04:06:22.000000 itential.py-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     2910 2022-11-11 04:36:39.118023 itential.py-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      853 2022-11-11 03:57:13.000000 itential.py-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2022-11-11 04:36:39.089159 itential.py-0.0.6/itential/
--rw-rw-rw-   0        0        0       36 2022-08-18 04:06:22.000000 itential.py-0.0.6/itential/__init__.py
--rw-rw-rw-   0        0        0     4659 2022-11-11 04:33:37.000000 itential.py-0.0.6/itential/core.py
-drwxrwxrwx   0        0        0        0 2022-11-11 04:36:39.099295 itential.py-0.0.6/itential/modules/
--rw-rw-rw-   0        0        0        0 2022-08-18 04:06:22.000000 itential.py-0.0.6/itential/modules/__init__.py
--rw-rw-rw-   0        0        0     1052 2022-11-11 03:57:13.000000 itential.py-0.0.6/itential/modules/utils.py
-drwxrwxrwx   0        0        0        0 2022-11-11 04:36:39.115030 itential.py-0.0.6/itential/modules/v2020_2/
--rw-rw-rw-   0        0        0     1137 2022-11-11 03:57:13.000000 itential.py-0.0.6/itential/modules/v2020_2/__init__.py
--rw-rw-rw-   0        0        0     5701 2022-11-11 04:17:18.000000 itential.py-0.0.6/itential/modules/v2020_2/_adapter_automation_gateway.py
--rw-rw-rw-   0        0        0      823 2022-11-11 03:57:13.000000 itential.py-0.0.6/itential/modules/v2020_2/_app_admin_essentials.py
--rw-rw-rw-   0        0        0     2230 2022-11-11 03:57:13.000000 itential.py-0.0.6/itential/modules/v2020_2/_app_ag_manager.py
--rw-rw-rw-   0        0        0     7795 2022-11-11 03:57:13.000000 itential.py-0.0.6/itential/modules/v2020_2/_app_automation_catalog.py
--rw-rw-rw-   0        0        0     8289 2022-11-11 03:57:13.000000 itential.py-0.0.6/itential/modules/v2020_2/_app_automation_studio.py
--rw-rw-rw-   0        0        0     4994 2022-11-11 03:57:13.000000 itential.py-0.0.6/itential/modules/v2020_2/_app_configuration_manager.py
--rw-rw-rw-   0        0        0     1069 2022-11-11 03:57:13.000000 itential.py-0.0.6/itential/modules/v2020_2/_app_form_builder.py
--rw-rw-rw-   0        0        0      717 2022-11-11 03:57:13.000000 itential.py-0.0.6/itential/modules/v2020_2/_app_json_forms.py
--rw-rw-rw-   0        0        0     5641 2022-11-11 03:57:13.000000 itential.py-0.0.6/itential/modules/v2020_2/_app_jst.py
--rw-rw-rw-   0        0        0     1738 2022-11-11 03:57:13.000000 itential.py-0.0.6/itential/modules/v2020_2/_app_mop.py
--rw-rw-rw-   0        0        0     1422 2022-11-11 03:57:13.000000 itential.py-0.0.6/itential/modules/v2020_2/_app_nso_manager.py
--rw-rw-rw-   0        0        0     1117 2022-11-11 03:57:13.000000 itential.py-0.0.6/itential/modules/v2020_2/_app_operations_manager.py
--rw-rw-rw-   0        0        0      706 2022-11-11 03:57:13.000000 itential.py-0.0.6/itential/modules/v2020_2/_app_service_catalog.py
--rw-rw-rw-   0        0        0     1098 2022-11-11 03:57:13.000000 itential.py-0.0.6/itential/modules/v2020_2/_app_service_management.py
--rw-rw-rw-   0        0        0      253 2022-11-11 03:57:13.000000 itential.py-0.0.6/itential/modules/v2020_2/_app_task_worker.py
--rw-rw-rw-   0        0        0      278 2022-11-11 03:57:13.000000 itential.py-0.0.6/itential/modules/v2020_2/_app_template_builder.py
--rw-rw-rw-   0        0        0    10052 2022-11-11 03:57:13.000000 itential.py-0.0.6/itential/modules/v2020_2/_app_workflow_builder.py
--rw-rw-rw-   0        0        0    51910 2022-11-11 03:57:13.000000 itential.py-0.0.6/itential/modules/v2020_2/_app_workflow_engine.py
--rw-rw-rw-   0        0        0     3584 2022-11-11 03:57:13.000000 itential.py-0.0.6/itential/modules/v2020_2/_pronghorn_core.py
-drwxrwxrwx   0        0        0        0 2022-11-11 04:36:39.116028 itential.py-0.0.6/itential/modules/v2021_1/
--rw-rw-rw-   0        0        0       34 2022-11-11 03:57:13.000000 itential.py-0.0.6/itential/modules/v2021_1/__init__.py
--rw-rw-rw-   0        0        0      390 2022-08-18 04:06:22.000000 itential.py-0.0.6/itential/modules/v2021_1/_app_form_builder.py
-drwxrwxrwx   0        0        0        0 2022-11-11 04:36:39.117025 itential.py-0.0.6/itential/modules/v2021_2/
--rw-rw-rw-   0        0        0       53 2022-08-18 04:06:22.000000 itential.py-0.0.6/itential/modules/v2021_2/__init__.py
--rw-rw-rw-   0        0        0      227 2022-08-18 04:06:22.000000 itential.py-0.0.6/itential/modules/v2021_2/_app_form_builder.py
-drwxrwxrwx   0        0        0        0 2022-11-11 04:36:39.098298 itential.py-0.0.6/itential.py.egg-info/
--rw-rw-rw-   0        0        0     2910 2022-11-11 04:36:39.000000 itential.py-0.0.6/itential.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1410 2022-11-11 04:36:39.000000 itential.py-0.0.6/itential.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-11 04:36:39.000000 itential.py-0.0.6/itential.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-11-11 04:36:39.000000 itential.py-0.0.6/itential.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-11 04:36:39.000000 itential.py-0.0.6/itential.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1129 2022-11-11 04:36:30.000000 itential.py-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-11-11 04:36:39.119020 itential.py-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-30 22:45:54.469673 itential.py-1.0.0/
+-rw-rw-rw-   0        0        0     1107 2022-08-18 04:06:22.000000 itential.py-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2853 2023-06-30 22:45:54.468673 itential.py-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      794 2023-06-30 22:20:26.000000 itential.py-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 22:45:54.416681 itential.py-1.0.0/itential/
+-rw-rw-rw-   0        0        0       36 2022-08-18 04:06:22.000000 itential.py-1.0.0/itential/__init__.py
+-rw-rw-rw-   0        0        0     6771 2023-06-30 22:44:45.000000 itential.py-1.0.0/itential/core.py
+drwxrwxrwx   0        0        0        0 2023-06-30 22:45:54.437672 itential.py-1.0.0/itential/modules/
+-rw-rw-rw-   0        0        0        0 2022-08-18 04:06:22.000000 itential.py-1.0.0/itential/modules/__init__.py
+-rw-rw-rw-   0        0        0     1052 2023-06-30 03:50:41.000000 itential.py-1.0.0/itential/modules/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 22:45:54.462674 itential.py-1.0.0/itential/modules/v2020_2/
+-rw-rw-rw-   0        0        0     1137 2022-08-18 04:06:22.000000 itential.py-1.0.0/itential/modules/v2020_2/__init__.py
+-rw-rw-rw-   0        0        0     5651 2023-06-30 22:26:53.000000 itential.py-1.0.0/itential/modules/v2020_2/_adapter_automation_gateway.py
+-rw-rw-rw-   0        0        0      833 2023-06-30 22:14:37.000000 itential.py-1.0.0/itential/modules/v2020_2/_app_admin_essentials.py
+-rw-rw-rw-   0        0        0     2106 2023-06-30 22:26:53.000000 itential.py-1.0.0/itential/modules/v2020_2/_app_ag_manager.py
+-rw-rw-rw-   0        0        0     7365 2023-06-30 22:26:53.000000 itential.py-1.0.0/itential/modules/v2020_2/_app_automation_catalog.py
+-rw-rw-rw-   0        0        0     7669 2023-06-30 22:26:53.000000 itential.py-1.0.0/itential/modules/v2020_2/_app_automation_studio.py
+-rw-rw-rw-   0        0        0     4994 2022-08-18 04:06:22.000000 itential.py-1.0.0/itential/modules/v2020_2/_app_configuration_manager.py
+-rw-rw-rw-   0        0        0     1069 2022-08-18 04:06:22.000000 itential.py-1.0.0/itential/modules/v2020_2/_app_form_builder.py
+-rw-rw-rw-   0        0        0      717 2022-08-18 04:06:22.000000 itential.py-1.0.0/itential/modules/v2020_2/_app_json_forms.py
+-rw-rw-rw-   0        0        0     5249 2023-06-30 22:26:53.000000 itential.py-1.0.0/itential/modules/v2020_2/_app_jst.py
+-rw-rw-rw-   0        0        0     1738 2022-08-18 04:06:22.000000 itential.py-1.0.0/itential/modules/v2020_2/_app_mop.py
+-rw-rw-rw-   0        0        0     1422 2022-08-18 04:06:22.000000 itential.py-1.0.0/itential/modules/v2020_2/_app_nso_manager.py
+-rw-rw-rw-   0        0        0     1117 2022-08-18 04:06:22.000000 itential.py-1.0.0/itential/modules/v2020_2/_app_operations_manager.py
+-rw-rw-rw-   0        0        0      706 2022-08-18 04:06:22.000000 itential.py-1.0.0/itential/modules/v2020_2/_app_service_catalog.py
+-rw-rw-rw-   0        0        0     1098 2022-08-18 04:06:22.000000 itential.py-1.0.0/itential/modules/v2020_2/_app_service_management.py
+-rw-rw-rw-   0        0        0      253 2022-08-18 04:06:22.000000 itential.py-1.0.0/itential/modules/v2020_2/_app_task_worker.py
+-rw-rw-rw-   0        0        0      278 2022-08-18 04:06:22.000000 itential.py-1.0.0/itential/modules/v2020_2/_app_template_builder.py
+-rw-rw-rw-   0        0        0     9282 2023-06-30 22:26:53.000000 itential.py-1.0.0/itential/modules/v2020_2/_app_workflow_builder.py
+-rw-rw-rw-   0        0        0    47628 2023-06-30 22:26:53.000000 itential.py-1.0.0/itential/modules/v2020_2/_app_workflow_engine.py
+-rw-rw-rw-   0        0        0     3584 2022-08-18 04:06:22.000000 itential.py-1.0.0/itential/modules/v2020_2/_pronghorn_core.py
+drwxrwxrwx   0        0        0        0 2023-06-30 22:45:54.466673 itential.py-1.0.0/itential/modules/v2021_1/
+-rw-rw-rw-   0        0        0       34 2022-08-18 04:06:22.000000 itential.py-1.0.0/itential/modules/v2021_1/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-30 22:21:37.000000 itential.py-1.0.0/itential/modules/v2021_1/_app_form_builder.py
+-rw-rw-rw-   0        0        0        0 2023-06-30 05:43:26.000000 itential.py-1.0.0/itential/modules/v2021_1/_app_workflow_builder.py
+drwxrwxrwx   0        0        0        0 2023-06-30 22:45:54.467672 itential.py-1.0.0/itential/modules/v2021_2/
+-rw-rw-rw-   0        0        0       53 2022-08-18 04:06:22.000000 itential.py-1.0.0/itential/modules/v2021_2/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-30 22:21:37.000000 itential.py-1.0.0/itential/modules/v2021_2/_app_form_builder.py
+drwxrwxrwx   0        0        0        0 2023-06-30 22:45:54.436708 itential.py-1.0.0/itential.py.egg-info/
+-rw-rw-rw-   0        0        0     2853 2023-06-30 22:45:54.000000 itential.py-1.0.0/itential.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1460 2023-06-30 22:45:54.000000 itential.py-1.0.0/itential.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 22:45:54.000000 itential.py-1.0.0/itential.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-30 22:45:54.000000 itential.py-1.0.0/itential.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-30 22:45:54.000000 itential.py-1.0.0/itential.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1137 2023-06-30 22:40:59.000000 itential.py-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 22:45:54.469673 itential.py-1.0.0/setup.cfg
```

### Comparing `itential.py-0.0.6/LICENSE` & `itential.py-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `itential.py-0.0.6/PKG-INFO` & `itential.py-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itential.py
-Version: 0.0.6
+Version: 1.0.0
 Summary: A Python wrapper for the Itential API.
 Author: Tagmeh
 License: The MIT License (MIT)
         
         Copyright (c) 2022-present John Epperson
         
         Permission is hereby granted, free of charge, to any person obtaining a
@@ -36,22 +36,34 @@
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Itential.py
+A library to (hopefully) make Itential scripting via Python a little easier.
 
-#### An effort to write a python library for the Itential API. (https://apidocs.itential.com/2021.2/api/) (New Link to Old Docs)
-
-8.5.2022 - I took a break after Itential updated their documentation, and broke all of their existing links (including every link I had posted in the method doc strings...). Pretty demoralizing, and a month or so after the Great Link Breakin'ing, they are still all broken. But, my motivation has returned, and work will continue. I plan on getting this pushed out as a package as quickly as possible.
+Pypi: https://pypi.org/project/itential.py/
 
+## Remote Install
+```text
+pip install itential.py
+```
 
-Usage
+## Usage
 ```python
 from itential import Itential
 from itential.modules.v2020_2 import AppWorkflowEngine
 
 client = Itential()  # Contains default login and localhost url information
 
-response: "requests.Response" = AppWorkflowEngine.get_job_output(client=client, job_id="example-job-id")
+workflow_engine = AppWorkflowEngine(client=client)  # Pass in the auth client
+
+response: "requests.Response" = workflow_engine.get_job_output(job_id="example-job-id")
+```
+
+## Local Install
+Curently the repository is setup for pipenv. I'm looking into making the repository agnostic to the python environment manager (poetry, pipnev, venv).
+```text
+pip install pipenv
+pipenv install . --dev
 ```
```

### Comparing `itential.py-0.0.6/itential/core.py` & `itential.py-1.0.0/itential/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,104 @@
 import logging
-from typing import Dict, Any
+from typing import Dict, Any, Union
 
 import requests
+from requests.adapters import HTTPAdapter, Retry
 
-logging.basicConfig(level=logging.WARNING)
 log = logging.getLogger(__name__)
 
 
 class Itential:
     def __init__(self, **kwargs) -> None:  # type: ignore
         """
         :param username: Known defaults include "admin@pronghorn" and "admin@itential"
         :param password: For authenticating with the server. Never stored or printed.
-        :param version: Not in use yet, might help with using the correct methods for authentication in the future.
         :param url: Used to change the server. Default is the local machine.
         :param session: Pass in a previously saved requests.Session object in order to bypass the authentication call.
+        :param max_retries: The maximum number of times to retry a failed request. Default is 3.
+        :param backoff_factor: The factor to multiply the backoff time by. Default is 0.2.
+                               0.2 is a 20% increase per backoff.
+        :param backoff_delay: The initial delay to use. Default is 2.
         """
         self.username: str = kwargs.get("username", "admin@pronghorn")
         self.password: str = kwargs.get("password", "admin")
-        self.version: str = kwargs.get("version", "latest")
         self.auth_body: Dict[str, Dict[str, str]] = {"user": {"username": self.username, "password": self.password}}
-
-        self._url: str = "http://localhost:3000"
-        # self._url - Probably a better way to do this.
-        # self.__setattr__('url', kwargs.get('url', "http://localhost:3000"))
-
+        self.url: str = self.clean_and_validate_url(kwargs.get("url"))
         self.session: requests.Session = kwargs.get('session', requests.Session())
 
-    @property
-    def url(self) -> str:
-        return self._url
+        self.max_retries: int = kwargs.get("max_retries", 3)
+
+        self.backoff_factor: float = float((kwargs.get("backoff_factor", 0.2)))
+        if self.backoff_factor < 0:
+            log.warning("backoff_factor cannot be less than 0. Setting to 0.1 (10%).")
+            self.backoff_factor = 0.1
+
+        self.backoff_delay: int = kwargs.get("backoff_delay", 2)
+        if self.backoff_delay < 1:
+            log.warning("backoff_delay is less than 1. Setting to 1.")
+            self.backoff_delay = 1
+
+        self.setup_requests_retry()
+
+    def setup_requests_retry(self) -> None:
+        """
+        Sets up the retry mechanism for the requests library.
+        """
+        status_forcelist = [
+            408,  # Request Timeout
+            409,  # Conflict
+            429,  # Too Many Requests
+            500,  # Internal Server Error
+            502,  # Bad Gateway
+            503,  # Service Unavailable
+            504,  # Gateway Timeout
+        ]
+        log.debug(
+            f'Configuring Requests retry for status codes: {", ".join([str(status) for status in status_forcelist])}'
+        )
+
+        retry = Retry(total=self.max_retries, backoff_factor=self.backoff_factor, status_forcelist=status_forcelist)
+        log.debug(
+            f'Configured requests.Retry for with '
+            f'max_retries={self.max_retries} and backoff_factor={self.backoff_factor}'
+        )
+
+        adapter = HTTPAdapter(max_retries=retry)
+        self.session.mount('http://', adapter)
+        log.debug('Retry set for "http://"')
+        self.session.mount('https://', adapter)
+        log.debug('Retry set for "https://"')
 
-    @url.setter
-    def url(self, value: str) -> None:
+    @staticmethod
+    def clean_and_validate_url(value: Union[None, str]) -> str:
         """Cleans the input URL of any extra whitespace and trailing slashes."""
+        log.debug(f'Cleaning/validating user-defined URL: {value}')
         if value:
             trimmed_value = value.strip()
             if trimmed_value.endswith('/'):
                 value = trimmed_value[::-1].replace('/', '', 1)[::-1]
-            self._url = value
+            log.debug(f'Cleaned/validated URL: {value}')
+            return value
+        return "http://localhost:3000"
 
     def call(self, method: str, url: str, **kwargs: Any) -> requests.Response:
         """
-        Wrapper for the Requests request method. Designed to have the Itential class authenticate with the server
-        or verify its connection before making the module call.
+        Calls the given endpoint, authenticates with the server if necessary.
         """
-        self.authenticate()
-
         headers = kwargs.get("headers", {"Content-Type": "application/json"})  # Required by some calls.
         verify = kwargs.get("verify", False)
+        # retry is only here to prevent a loop. Causes errors if passed into session.request, thus, we pop it.
+        retry = kwargs.pop('retry', False)
+
+        response = self.session.request(method=method, url=url, headers=headers, verify=verify, **kwargs)
 
-        return self.session.request(method=method, url=url, headers=headers, verify=verify, **kwargs)
+        if response.status_code in [401, 403] and not retry:
+            self.authenticate()
+            return self.call(method=method, url=url, retry=True, **kwargs)  # Retry the call after authenticating.
+        return response
 
     def authenticate(self) -> None:
         """
         Authenticates with the specified server. Attempts to use self.session if available.
         Updates the self.session for use with subsequent calls.
         """
         # Make initial authentication check with old/previous session cookies.
```

### Comparing `itential.py-0.0.6/itential/modules/utils.py` & `itential.py-1.0.0/itential/modules/utils.py`

 * *Files identical despite different names*

### Comparing `itential.py-0.0.6/itential/modules/v2020_2/__init__.py` & `itential.py-1.0.0/itential/modules/v2020_2/__init__.py`

 * *Files identical despite different names*

### Comparing `itential.py-0.0.6/itential/modules/v2020_2/_adapter_automation_gateway.py` & `itential.py-1.0.0/itential/modules/v2020_2/_adapter_automation_gateway.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,56 +74,59 @@
 if TYPE_CHECKING:
     from itential.core import Itential
 
 
 class AdapterAutomationGateway:
     """https://apidocs.itential.com/2020.2/api/adapter-automation_gateway/"""
 
-    @staticmethod
-    def netmiko_send_command(client: "Itential", host: str, commands: List[str],
-                             connection_options: Dict[str, str]) -> requests.Response:
+    def __init__(self, client: "Itential"):
+        self.client = client
+
+    def netmiko_send_command(
+        self, host: str, commands: List[str], connection_options: Dict[str, str]
+    ) -> requests.Response:
         """
         Wrapper of send_command of netmiko.
-
         https://apidocs.itential.com/2020.2/api/adapter-automation_gateway/netmikoSendCommand/
 
-        :param client: The Itential state object
         :param host: Device TID/Name
         :param commands: A List of commands to run.
         :param connection_options: Connection and Authentication information.
          Keys: "device_type", "port", "username", "password".
          See Netmiko documentation for more detail.
         :return: A JSON Object containing status, code and the result
         """
         body = {
             "netmikoSendCommandParameters": {
                 "host": host,
                 "commands": commands,
-                "connection_options": connection_options
+                "connection_options": connection_options,
             }
         }
-        return client.call(method="POST", url=f"{client.url}/automationgateway/netmiko/send_command", json=body)
-
-    @staticmethod
-    def netmiko_send_config(client: "Itential", host: str, config_commands: List[str],
-                            connection_options: Dict[str, Union[int, str]]) -> requests.Response:
+        return self.client.call(
+            method="POST", url=f"{self.client.url}/automationgateway/netmiko/send_command", json=body
+        )
+
+    def netmiko_send_config(
+        self, host: str, config_commands: List[str], connection_options: Dict[str, Union[int, str]]
+    ) -> requests.Response:
         """
         Wrapper of send_config_set of netmiko.
-
         https://apidocs.itential.com/2020.2/api/adapter-automation_gateway/netmikoSendConfig/
 
-        :param client: The Itential state object
         :param host: Device TID/Name
         :param config_commands: A List of config commands to run.
         :param connection_options: Connection and Authentication information.
          Keys: "device_type", "port", "username", "password".
          See Netmiko documentation for more detail.
         :return: A JSON Object containing status, code and the result
         """
         body = {
             "netmikoSendConfigParameters": {
                 "host": host,
                 "config_commands": config_commands,
-                "connection_options": connection_options
+                "connection_options": connection_options,
             }
         }
-        return client.call(method="POST", url=f"{client.url}/automationgateway/netmiko/send_config", json=body)
+        return self.client.call(
+            method="POST", url=f"{self.client.url}/automationgateway/netmiko/send_config", json=body
+        )
```

### Comparing `itential.py-0.0.6/itential/modules/v2020_2/_app_admin_essentials.py` & `itential.py-1.0.0/itential/modules/v2020_2/_app_admin_essentials.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,18 @@
     from itential.core import Itential
     import requests
 
 
 class AppAdminEssentials:
     """https://apidocs.itential.com/2020.2/api/app-admin_essentials/"""
 
-    @staticmethod
-    def get_services_health(client: "Itential") -> "requests.Response":
+    def __init__(self, client: "Itential"):
+        self.client = client
+
+    def get_services_health(self) -> "requests.Response":
         """
         Gets the health of all services in an IAP environment.
         https://apidocs.itential.com/2020.2/api/app-admin_essentials/getServicesHealth/
-        :param client: Itential state object
+
         :return:
         """
-        return client.call(method="GET", url=f"{client.url}/admin/services/health")
+        return self.client.call(method="GET", url=f"{self.client.url}/admin/services/health")
```

### Comparing `itential.py-0.0.6/itential/modules/v2020_2/_app_ag_manager.py` & `itential.py-1.0.0/itential/modules/v2020_2/_app_ag_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,41 +12,41 @@
     from itential.core import Itential
     import requests
 
 
 class AppAgManager:
     """https://apidocs.itential.com/2020.2/api/app-ag_manager/"""
 
-    @staticmethod
-    def discover_modules(client: "Itential", adapter_id: str) -> "requests.Response":
+    def __init__(self, client: "Itential"):
+        self.client = client
+
+    def discover_modules(self, adapter_id: str) -> "requests.Response":
         """
         Discovers all actions from a specified IAG adapter.
         This will restart this app and display a corresponding log message.
         https://apidocs.itential.com/2020.2/api/app-ag_manager/discoverModules/
-        :param client: Itential state object
+
         :param adapter_id: Automation Gateway adapter ID
         :return: requests.Response: A pronghorn.json object.
         """
-        return client.call(method="GET", url=f"{client.url}/ag-manager/actions/{adapter_id}")
+        return self.client.call(method="GET", url=f"{self.client.url}/ag-manager/actions/{adapter_id}")
 
-    @staticmethod
-    def undiscover_all(client: "Itential") -> "requests.Response":
+    def undiscover_all(self) -> "requests.Response":
         """
         Discovers all actions from all IAG adapters.
         This will restart this app and display a corresponding log message.
         https://apidocs.itential.com/2020.2/api/app-ag_manager/undiscoverAll/
-        :param client: Itential state object
+
         :return: requests.Response: A pronghorn.json object.
         """
-        return client.call(method="DELETE", url=f"{client.url}/ag-manager/actions")
+        return self.client.call(method="DELETE", url=f"{self.client.url}/ag-manager/actions")
 
-    @staticmethod
-    def undiscover_modules(client: "Itential", adapter_id: str) -> "requests.Response":
+    def undiscover_modules(self, adapter_id: str) -> "requests.Response":
         """
         Removes all actions from a specified IAG adapter.
         This will restart this app and display a corresponding log message.
         https://apidocs.itential.com/2020.2/api/app-ag_manager/undiscoverModules/
-        :param client: Itential state object
+
         :param adapter_id: Automation Gateway adapter ID
         :return: requests.Response: A pronghorn.json object.
         """
-        return client.call(method="DELETE", url=f"{client.url}/ag-manager/actions/{adapter_id}")
+        return self.client.call(method="DELETE", url=f"{self.client.url}/ag-manager/actions/{adapter_id}")
```

### Comparing `itential.py-0.0.6/itential/modules/v2020_2/_app_automation_catalog.py` & `itential.py-1.0.0/itential/modules/v2020_2/_app_automation_catalog.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,123 +18,123 @@
     from itential.core import Itential
     import requests
 
 
 class AppAutomationCatalog:
     """https://apidocs.itential.com/2020.2/api/app-automation_catalog/"""
 
-    @staticmethod
-    def create_automation(client: "Itential", name: str, description: str) -> "requests.Response":
+    def __init__(self, client: "Itential"):
+        self.client = client
+
+    def create_automation(self, name: str, description: str) -> "requests.Response":
         """
         Creates an automation with optional description.
         An automation's root structure is based off the agenda.js library,
          with any custom data falling into the 'data' array
         https://apidocs.itential.com/2020.2/api/app-automation_catalog/createAutomation/
-        :param client: Itential state object
+
         :param name: Unique name of the automation
         :param description: Short description of the automation
         :return: requests.Response: Automation document that was created by the request
         """
         body = {"name": name, "description": description}
-        return client.call(method="POST", url=f"{client.url}/automation_catalog/automations", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/automation_catalog/automations", json=body)
 
-    @staticmethod
-    def delete_automations(client: "Itential", ids: List[str]) -> "requests.Response":
+    def delete_automations(self, ids: List[str]) -> "requests.Response":
         """
         Deletes automations (based off an array of Ids)
         https://apidocs.itential.com/2020.2/api/app-automation_catalog/deleteAutomations/
-        :param client: Itential state object
+
         :param ids: List of automation IDs
         :return: requests.Response: Object containing a property removeCount
         """
         body = {"ids": ids}
-        return client.call(method="DELETE", url=f"{client.url}/automation_catalog/automations", json=body)
+        return self.client.call(method="DELETE", url=f"{self.client.url}/automation_catalog/automations", json=body)
 
-    @staticmethod
-    def export_automations(client: "Itential", automation_id: str) -> "requests.Response":
+    def export_automations(self, automation_id: str) -> "requests.Response":
         """
         Returns a single automation formatted for importing
         https://apidocs.itential.com/2020.2/api/app-automation_catalog/exportAutomation/
-        :param client: Itential state object
+
         :param automation_id: Unique id of the automation
         :return: requests.Response: Automation document that was requested in exported format
         """
-        return client.call(method="GET", url=f"{client.url}/automation_catalog/automations/{automation_id}/export")
+        return self.client.call(
+            method="GET", url=f"{self.client.url}/automation_catalog/automations/{automation_id}/export"
+        )
 
-    @staticmethod
-    def get_automation_by_id(client: "Itential", automation_id: str) -> "requests.Response":
+    def get_automation_by_id(self, automation_id: str) -> "requests.Response":
         """
         Gets an single automation by its id
         https://apidocs.itential.com/2020.2/api/app-automation_catalog/getAutomationById/
-        :param client: Itential state object
+
         :param automation_id: Unique id of the automation
         :return: requests.Response: Automation document that was requested
         """
-        return client.call(method="GET", url=f"{client.url}/automation_catalog/automations/{automation_id}")
+        return self.client.call(method="GET", url=f"{self.client.url}/automation_catalog/automations/{automation_id}")
 
-    @staticmethod
-    def get_automations(client: "Itential", query_parameters: Dict[str, Any]) -> "requests.Response":
+    def get_automations(self, query_parameters: Dict[str, Any]) -> "requests.Response":
         """
         Gets all known automations returned in alphabetical order
         https://apidocs.itential.com/2020.2/api/app-automation_catalog/getAutomations/
-        :param client: Itential state object
+
         :param query_parameters: < Undocumented >
         :return: requests.Response: List of all automation documents
         """
         params = {"queryParameters": query_parameters}
-        return client.call(method="GET", url=f"{client.url}/automation_catalog/automations", params=params)
+        return self.client.call(method="GET", url=f"{self.client.url}/automation_catalog/automations", params=params)
 
-    @staticmethod
     def import_automations(
-        client: "Itential", automation_jsons: List[Dict[str, Any]], options: Dict[str, Any]
+        self, automation_jsons: List[Dict[str, Any]], options: Dict[str, Any]
     ) -> "requests.Response":
         """
         Insert automation documents into the automation collection from a user supplied JSON document.
         https://apidocs.itential.com/2020.2/api/app-automation_catalog/importAutomations/
-        :param client: Itential state object
+
         :param automation_jsons: List of json representations of automation catalogs
         :param options:
         :return: requests.Response: Status of automation import operation
         """
         body = {"automations": automation_jsons, "options": options}
-        return client.call(method="POST", url=f"{client.url}/automation_catalog/automations/import", json=body)
+        return self.client.call(
+            method="POST", url=f"{self.client.url}/automation_catalog/automations/import", json=body
+        )
 
-    @staticmethod
-    def migrate_agenda_jobs(client: "Itential", agenda_jobs: List[str]) -> "requests.Response":
+    def migrate_agenda_jobs(self, agenda_jobs: List[str]) -> "requests.Response":
         """
         Takes an existing Agenda Job data structure and converts it to an Automation
         https://apidocs.itential.com/2020.2/api/app-automation_catalog/migrateAgendaJobs/
-        :param client: Itential state object
+
         :param agenda_jobs: List of Unique ids automations
         :return: requests.Response: The result of the migration process
         """
         body = {"agendaJobs": agenda_jobs}
-        return client.call(method="POST", url=f"{client.url}/automation_catalog/automations/migration", json=body)
+        return self.client.call(
+            method="POST", url=f"{self.client.url}/automation_catalog/automations/migration", json=body
+        )
 
-    @staticmethod
-    def run_automation(client: "Itential", automation_id: str, options: Dict[str, Any]) -> "requests.Response":
+    def run_automation(self, automation_id: str, options: Dict[str, Any]) -> "requests.Response":
         """
         Single run of an automation outside its scheduled runs, Requires a workflow to be attached to the automation.
         https://apidocs.itential.com/2020.2/api/app-automation_catalog/runAutomation/
-        :param client: Itential state object
+
         :param automation_id: Unique id of the automation
         :param options: Workflow based properties (Mostly undocumented)
         :return: requests.Response: {"status": "str", "message": {}, "workflowResponse": {}}
         """
         body = {"options": options}
-        return client.call(
-            method="POST", url=f"{client.url}/automation_catalog/automations/{automation_id}/run", json=body
+        return self.client.call(
+            method="POST", url=f"{self.client.url}/automation_catalog/automations/{automation_id}/run", json=body
         )
 
-    @staticmethod
-    def update_automation(client: "Itential", automation_id: str, options: Dict[str, Any]) -> "requests.Response":
+    def update_automation(self, automation_id: str, options: Dict[str, Any]) -> "requests.Response":
         """
         Updates an automation's attributes (including scheduling data).
         https://apidocs.itential.com/2020.2/api/app-automation_catalog/updateAutomation/
-        :param client: Itential state object
+
         :param automation_id: Unique id of the automation
         :param options: Object containing the fields to be updated
             ex: {"options": {
                     "workflowId": "8e3695fe-c5bf-4286-ae83-186b3fea1c1a",
                     "formId": "74cd8ca4367d4a9617c5c849",
                     "gbac": {
                       "write": [
@@ -149,8 +149,10 @@
                     "nextRunAt": "2019-11-25T22:51:39.201Z",
                     "repeatInterval": null
                   }
                 }
         :return: requests.Response: Updated document of requested automation
         """
         body = {"options": options}
-        return client.call(method="PUT", url=f"{client.url}/automation_catalog/automations/{automation_id}", json=body)
+        return self.client.call(
+            method="PUT", url=f"{self.client.url}/automation_catalog/automations/{automation_id}", json=body
+        )
```

### Comparing `itential.py-0.0.6/itential/modules/v2020_2/_app_automation_studio.py` & `itential.py-1.0.0/itential/modules/v2020_2/_app_automation_studio.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,151 +20,145 @@
     from itential.core import Itential
     import requests
 
 
 class AppAutomationStudio:
     """https://apidocs.itential.com/2020.2/api/app-automation_studio/createAutomation/"""
 
-    @staticmethod
-    def create_automation(client: "Itential", automation_json: Dict[str, Any]) -> "requests.Response":
+    def __init__(self, client: "Itential"):
+        self.client = client
+
+    def create_automation(self, automation_json: Dict[str, Any]) -> "requests.Response":
         """
         Creates a new automation document.
         https://apidocs.itential.com/2020.2/api/app-automation_studio/createAutomation/
-        :param client: Itential state object
+
         :param automation_json: json representation of the Automation to create
         :return: requests.Response: Created automation and associated edit URI
         """
         body = {"automation": automation_json}
-        return client.call(method="POST", url=f"{client.url}/automation-studio/automations", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/automation-studio/automations", json=body)
 
-    @staticmethod
-    def create_template(client: "Itential", template_json: Dict[str, Any]) -> "requests.Response":
+    def create_template(self, template_json: Dict[str, Any]) -> "requests.Response":
         """
         Creates a new template document.
         https://apidocs.itential.com/2020.2/api/app-automation_studio/createTemplate/
-        :param client: Itential state object
+
         :param template_json: json representation of the Template to create
         :return: requests.Response: Created template and associated edit URI.
         """
         body = {"template": template_json}
-        return client.call(method="POST", url=f"{client.url}/automation-studio/templates", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/automation-studio/templates", json=body)
 
-    @staticmethod
-    def delete_template(client: "Itential", template_id: str) -> "requests.Response":
+    def delete_template(self, template_id: str) -> "requests.Response":
         """
         Deletes a template document.
         https://apidocs.itential.com/2020.2/api/app-automation_studio/deleteTemplate/
-        :param client: Itential state object
+
         :param template_id: Unique template ID
         :return: requests.Response:
         """
-        return client.call(method="DELETE", url=f"{client.url}/automation-studio/templates/{template_id}")
+        return self.client.call(method="DELETE", url=f"{self.client.url}/automation-studio/templates/{template_id}")
 
-    @staticmethod
-    def get_method_options(client: "Itential") -> "requests.Response":
+    def get_method_options(self) -> "requests.Response":
         """
         Get all available rest calls in IAP.
         https://apidocs.itential.com/2020.2/api/app-automation_studio/getMethodOptions/
-        :param client: Itential state object
+
         :return: requests.Response: List of all rest calls available in the system.
         """
-        return client.call(method="GET", url=f"{client.url}/automation-studio/json-forms/method-options")
+        return self.client.call(method="GET", url=f"{self.client.url}/automation-studio/json-forms/method-options")
 
-    @staticmethod
-    def get_template(client: "Itential", template_id: str, query_parameters: Dict[str, Any]) -> "requests.Response":
+    def get_template(self, template_id: str, query_parameters: Dict[str, Any]) -> "requests.Response":
         """
         Gets a single template document.
         https://apidocs.itential.com/2020.2/api/app-automation_studio/getTemplate/
-        :param client: Itential state object
+
         :param template_id: ObjectId specifying a template entity.
         :param query_parameters: Optional parameters for projecting fields in the template document.
             (example in DOM only)
         :return: requests.Response:
         """
         params = {"queryParameters": query_parameters}
-        return client.call(method="GET", url=f"{client.url}/automation-studio/templates/{template_id}", params=params)
+        return self.client.call(
+            method="GET", url=f"{self.client.url}/automation-studio/templates/{template_id}", params=params
+        )
 
-    @staticmethod
-    def get_templates(client: "Itential", query_parameters: Dict[str, Any]) -> "requests.Response":
+    def get_templates(self, query_parameters: Dict[str, Any]) -> "requests.Response":
         """
         Gets a page of template documents.
         https://apidocs.itential.com/2020.2/api/app-automation_studio/getTemplates/
-        :param client: Itential state object
+
         :param query_parameters: Parameters for filtering, paginating, projecting, and sorting template documents.
             (example in DOM only)
         :return: requests.Response:
         """
         params = {"queryParameters": query_parameters}
-        return client.call(method="GET", url=f"{client.url}/automation-studio/templates", params=params)
+        return self.client.call(method="GET", url=f"{self.client.url}/automation-studio/templates", params=params)
 
-    @staticmethod
-    def import_automations(client: "Itential", automation_list: List[Dict[str, Any]]) -> "requests.Response":
+    def import_automations(self, automation_list: List[Dict[str, Any]]) -> "requests.Response":
         """
         Imports a new automation document.
         https://apidocs.itential.com/2020.2/api/app-automation_studio/importAutomations/
-        :param client: Itential state object
+
         :param automation_list: List of automation json representations.
         :return: requests.Response: Results from each individual import operation.
         """
         body = {"automations": automation_list}
-        return client.call(method="POST", url=f"{client.url}/automation-studio/automations/import", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/automation-studio/automations/import", json=body)
 
-    @staticmethod
-    def import_templates(client: "Itential", template_list: List[Dict[str, Any]]) -> "requests.Response":
+    def import_templates(self, template_list: List[Dict[str, Any]]) -> "requests.Response":
         """
         Imports a new template document.
         https://apidocs.itential.com/2020.2/api/app-automation_studio/importTemplates/
-        :param client: Itential state object
+
         :param template_list: List of template json representations.
         :return: requests.Response: Results from each individual import operation.
         """
         body = {"templates": template_list}
-        return client.call(method="POST", url=f"{client.url}/automation-studio/templates/import", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/automation-studio/templates/import", json=body)
 
-    @staticmethod
-    def run_transformation(
-        client: "Itential", transformation_id: str, transformation_data: Dict[str, Any]
-    ) -> "requests.Response":
+    def run_transformation(self, transformation_id: str, transformation_data: Dict[str, Any]) -> "requests.Response":
         """
         Transforms data using JST transformation document.
         https://apidocs.itential.com/2020.2/api/app-automation_studio/runTransformation/
-        :param client: Itential state object
+
         :param transformation_data: Transformation json representation
         :param transformation_id: Unique transformation ID
         :return: requests.Response: Transformed data.
         """
         body = {"data": transformation_data}
-        return client.call(
+        return self.client.call(
             method="POST",
-            url=f"{client.url}/automation-studio/json-forms/runTransformation/{transformation_id}",
+            url=f"{self.client.url}/automation-studio/json-forms/runTransformation/{transformation_id}",
             json=body,
         )
 
-    @staticmethod
-    def update_automation(
-        client: "Itential", automation_id: str, automation_update: Dict[str, Any]
-    ) -> "requests.Response":
+    def update_automation(self, automation_id: str, automation_update: Dict[str, Any]) -> "requests.Response":
         """
         Replaces a automation document.
         https://apidocs.itential.com/2020.2/api/app-automation_studio/updateAutomation/
-        :param client: Itential state object
+
         :param automation_id: Unique automation ID
         :param automation_update: Complete automation definition/json representation to replace the
             existing automation document with.
         :return: requests.Response:
         """
         body = {"update": automation_update}
-        return client.call(method="PUT", url=f"{client.url}/automation-studio/automations/{automation_id}", json=body)
+        return self.client.call(
+            method="PUT", url=f"{self.client.url}/automation-studio/automations/{automation_id}", json=body
+        )
 
-    @staticmethod
-    def update_template(client: "Itential", template_id: str, template_update: Dict[str, Any]) -> "requests.Response":
+    def update_template(self, template_id: str, template_update: Dict[str, Any]) -> "requests.Response":
         """
         Replaces a template document.
         https://apidocs.itential.com/2020.2/api/app-automation_studio/updateTemplate/
-        :param client: Itential state object
+
         :param template_id: Unique template ID
         :param template_update: Complete template definition to replace the existing template document with.
             May not contain fields '_id', 'created', 'createdBy', 'lastUpdated', or 'lastUpdatedBy'.
         :return: requests.Response:
         """
         body = {"update": template_update}
-        return client.call(method="PUT", url=f"{client.url}/automation-studio/templates/{template_id}", json=body)
+        return self.client.call(
+            method="PUT", url=f"{self.client.url}/automation-studio/templates/{template_id}", json=body
+        )
```

### Comparing `itential.py-0.0.6/itential/modules/v2020_2/_app_configuration_manager.py` & `itential.py-1.0.0/itential/modules/v2020_2/_app_configuration_manager.py`

 * *Files identical despite different names*

### Comparing `itential.py-0.0.6/itential/modules/v2020_2/_app_form_builder.py` & `itential.py-1.0.0/itential/modules/v2020_2/_app_form_builder.py`

 * *Files identical despite different names*

### Comparing `itential.py-0.0.6/itential/modules/v2020_2/_app_json_forms.py` & `itential.py-1.0.0/itential/modules/v2020_2/_app_json_forms.py`

 * *Files identical despite different names*

### Comparing `itential.py-0.0.6/itential/modules/v2020_2/_app_jst.py` & `itential.py-1.0.0/itential/modules/v2020_2/_app_jst.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,93 +19,89 @@
     from itential.core import Itential
     import requests
 
 
 class AppJst:
     """https://apidocs.itential.com/2020.2/api/app-jst"""
 
-    @staticmethod
-    def create_transformation(client: "Itential", jst_obj: Dict[str, Any]) -> "requests.Response":
+    def __init__(self, client: "Itential"):
+        self.client = client
+
+    def create_transformation(self, jst_obj: Dict[str, Any]) -> "requests.Response":
         """
         Creates a single transformation.
         https://apidocs.itential.com/2020.2/api/app-jst/createTransformation/ (Misleading param example and schema)
-        :param client: Itential state object
+
         :param jst_obj: Json object representation of the JST
         :return: requests.Response
         """
-        return client.call(method="POST", url=f"{client.url}/transformations", json=jst_obj)
+        return self.client.call(method="POST", url=f"{self.client.url}/transformations", json=jst_obj)
 
-    @staticmethod
-    def delete_transformation(client: "Itential", jst_id: str) -> "requests.Response":
+    def delete_transformation(self, jst_id: str) -> "requests.Response":
         """
         Deletes a single transformation from the server.
         https://apidocs.itential.com/2020.2/api/app-jst/deleteTransformation/
-        :param client: Itential state object
+
         :param jst_id: "_id" field of the JST json. ex: 6230fd0b56192935eed3eeb8
         :return: requests.Response  200: empty string
         """
-        return client.call(method="DELETE", url=f"{client.url}/transformations/{jst_id}")
+        return self.client.call(method="DELETE", url=f"{self.client.url}/transformations/{jst_id}")
 
-    @staticmethod
-    def get_transformations(client: "Itential", jst_id: str) -> "requests.Response":
+    def get_transformations(self, jst_id: str) -> "requests.Response":
         """
         Returns all transformations from the server, in full. This can return a rather large payload.
         Documentation is incorrect. Doesn't require "queryParameters". Don't have any examples of queryParameters usage.
         https://apidocs.itential.com/2021.2/api/app-jst/searchTransformations/
-        :param client: Itential state object
+
         :param jst_id: "_id" field of the JST json. ex: 6230fd0b56192935eed3eeb8
         :return: requests.Response
         """
-        return client.call(method="GET", url=rf"{client.url}/transformations/{jst_id}")
+        return self.client.call(method="GET", url=rf"{self.client.url}/transformations/{jst_id}")
 
-    @staticmethod
-    def import_transformation(client: "Itential", jst_obj: Dict[str, Any]) -> "requests.Response":
+    def import_transformation(self, jst_obj: Dict[str, Any]) -> "requests.Response":
         """
         Imports a single transformation/JST to the server. Will duplicate files if JST already exists.
         Will append a " (n)" to the end of the JST name. "n" is an incrementing integer
         https://apidocs.itential.com/2020.2/api/app-jst/importTransformation/ (Misleading param example and schema)
-        :param client: Itential state object
+
         :param jst_obj: The json object representation of the transformation/JST
         :return: requests.Response
         """
-        return client.call(method="POST", url=f"{client.url}/transformations/import", json=jst_obj)
+        return self.client.call(method="POST", url=f"{self.client.url}/transformations/import", json=jst_obj)
 
-    @staticmethod
     def run_transformation(
-        client: "Itential", jst_id: str, incoming: Dict[str, Any], options: Optional[Dict[str, Any]] = None
+        self, jst_id: str, incoming: Dict[str, Any], options: Optional[Dict[str, Any]] = None
     ) -> "requests.Response":
         """
         Runs a transformation
         https://apidocs.itential.com/2020.2/api/app-jst/runTransformation/
-        :param client: Itential state object
+
         :param jst_id: "_id" of the JST. ex: 6143988e49bd502787711378
         :param incoming: A dict object of the input schema.
         :param options: < Unclear > This is not required to run a transformation.
         :return: requests.Response Returns the outgoing schema as a json obj
         """
         data = {"incoming": incoming, "options": options if options else {}}
-        return client.call(method="POST", url=f"{client.url}/transformations/{jst_id}", json=data)
+        return self.client.call(method="POST", url=f"{self.client.url}/transformations/{jst_id}", json=data)
 
-    @staticmethod
-    def search_transformations(client: "Itential") -> "requests.Response":
+    def search_transformations(self) -> "requests.Response":
         """
         Returns all transformations from the server, in full. This can return a rather large payload.
         Doesn't require "queryParameters". The usage found in the website DOM is not correct
         Documentation is incomplete. Requires further testing to figure this one out.
         https://apidocs.itential.com/2021.2/api/app-jst/searchTransformations/
-        :param client: Itential state object
+
         :param query_parameters: < Unclear > Omitted the implementation at this time.
         :return: requests.Response
         """
-        return client.call(method="GET", url=rf"{client.url}/transformations")
+        return self.client.call(method="GET", url=rf"{self.client.url}/transformations")
 
-    @staticmethod
-    def update_transformation(client: "Itential", jst_id: str, jst_obj: Dict[str, Any]) -> "requests.Response":
+    def update_transformation(self, jst_id: str, jst_obj: Dict[str, Any]) -> "requests.Response":
         """
         Updates/Overwrites an existing transformation/JST based on ID. Does not create a duplicate file.
         https://apidocs.itential.com/2020.2/api/app-jst/updateTransformation/  (Misleading param example and schema)
-        :param client: Itential state object
+
         :param jst_id: "_id" field of the JST json. ex: 6230fd0b56192935eed3eeb8
         :param jst_obj: Full JST json. Does not require {"transformation": JST_json} like docs show.
         :return: requests.Response
         """
-        return client.call(method="PUT", url=f"{client.url}/transformations/{jst_id}", json=jst_obj)
+        return self.client.call(method="PUT", url=f"{self.client.url}/transformations/{jst_id}", json=jst_obj)
```

### Comparing `itential.py-0.0.6/itential/modules/v2020_2/_app_mop.py` & `itential.py-1.0.0/itential/modules/v2020_2/_app_mop.py`

 * *Files identical despite different names*

### Comparing `itential.py-0.0.6/itential/modules/v2020_2/_app_nso_manager.py` & `itential.py-1.0.0/itential/modules/v2020_2/_app_nso_manager.py`

 * *Files identical despite different names*

### Comparing `itential.py-0.0.6/itential/modules/v2020_2/_app_operations_manager.py` & `itential.py-1.0.0/itential/modules/v2020_2/_app_operations_manager.py`

 * *Files identical despite different names*

### Comparing `itential.py-0.0.6/itential/modules/v2020_2/_app_service_catalog.py` & `itential.py-1.0.0/itential/modules/v2020_2/_app_service_catalog.py`

 * *Files identical despite different names*

### Comparing `itential.py-0.0.6/itential/modules/v2020_2/_app_service_management.py` & `itential.py-1.0.0/itential/modules/v2020_2/_app_service_management.py`

 * *Files identical despite different names*

### Comparing `itential.py-0.0.6/itential/modules/v2020_2/_app_workflow_builder.py` & `itential.py-1.0.0/itential/modules/v2020_2/_app_workflow_builder.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,77 +24,75 @@
 
 
 class AppWorkflowBuilder:
     """
     https://apidocs.itential.com/2020.2/api/app-workflow_builder/
     """
 
-    @staticmethod
-    def delete_workflow(client: "Itential", name: str) -> "requests.Response":
+    def __init__(self, client: "Itential"):
+        self.client = client
+
+    def delete_workflow(self, name: str) -> "requests.Response":
         """
         Deletes a single workflow of the given name.
         https://apidocs.itential.com/2020.2/api/app-workflow_builder/deleteWorkflow/
-        :param client: Itential state object
+
         :param name: Name of the workflow to be deleted.
         :return: requests.Response object
                  A successful delete returns the deleted workflow json.
                  A failed delete returns a 500: "TypeError: Cannot read property '_id' of null"
         """
-        return client.call(method="DELETE", url=f"{client.url}/workflow_builder/workflows/delete/{name}")
+        return self.client.call(method="DELETE", url=f"{self.client.url}/workflow_builder/workflows/delete/{name}")
 
-    @staticmethod
-    def import_workflow(client: "Itential", data: Dict[str, Any]) -> "requests.Response":
+    def import_workflow(self, data: Dict[str, Any]) -> "requests.Response":
         """
         Imports a single workflow.
         https://apidocs.itential.com/2020.2/api/app-workflow_builder/importWorkflow/
-        :param client: Itential state object
+
         :param data: The workflow json object.
         :return: requests.Response object. Successful response ex: {'n': 1, 'ok': 1, 'name': 'automation_name'}
         """
         data = {"workflow": data, "options": {}}
-        return client.call(method="POST", url=f"{client.url}/workflow_builder/import", json=data)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_builder/import", json=data)
 
-    @staticmethod
-    def create_workflow_group_entry(client: "Itential", workflow_name: str, group_name: str) -> "requests.Response":
+    def create_workflow_group_entry(self, workflow_name: str, group_name: str) -> "requests.Response":
         """
         Add Group to a Workflow.
         https://apidocs.itential.com/2020.2/api/app-workflow_builder/createWorkflowGroupEntry/
-        :param client: Itential state object
+
         :param workflow_name: Name of the workflow to be assigned to the group
         :param group_name: < Unclear atm. Docs show an id, but the description says "name".
         :return: requests.Response
                                     500 error: "Invalid group: TestGroupName"
         """
         data = {"group": group_name}
-        return client.call(
-            method="POST", url=f"{client.url}/workflow_builder/workflows/{workflow_name}/groups", json=data
+        return self.client.call(
+            method="POST", url=f"{self.client.url}/workflow_builder/workflows/{workflow_name}/groups", json=data
         )
 
-    @staticmethod
-    def delete_workflow_groups(client: "Itential", workflow_name: str, group_name: str) -> "requests.Response":
+    def delete_workflow_groups(self, workflow_name: str, group_name: str) -> "requests.Response":
         """
         Delete all Groups for a Workflow
         https://apidocs.itential.com/2020.2/api/app-workflow_builder/deleteWorkflowGroups/ (Docs are incomplete)
-        :param client: Itential state object
+
         :param workflow_name: Name of the workflow to delete
         :param group_name: < unclear atm > Itential docs aren't complete for this version.
         :return: requests.Response  200: boolean
                                     500: "Could not find workflow: TestWorkflow". The group_name doesn't seem to matter.
         """
         data = {'groups': group_name}
-        return client.call(
-            method="DELETE", url=f"{client.url}/workflow_builder/workflows/{workflow_name}/groups", json=data
+        return self.client.call(
+            method="DELETE", url=f"{self.client.url}/workflow_builder/workflows/{workflow_name}/groups", json=data
         )
 
-    @staticmethod
-    def export_workflow(client: "Itential", workflow_id: str = '', workflow_name: str = '') -> "requests.Response":
+    def export_workflow(self, workflow_id: str = '', workflow_name: str = '') -> "requests.Response":
         """
         Returns the workflow json (Does not include a "_id" key at the top level)
         https://apidocs.itential.com/2020.2/api/app-workflow_builder/exportWorkflow/
-        :param client: Itential state object
+
         :param workflow_id: ID of the workflow to export
         :param workflow_name: Name of the workflow to export.
         :return: requests.Response  200: Returns the full workflow json.
                 Wrong workflow name 500: "Could not find matching workflow"
                 Wrong workflow ID   500: "Could not find matching workflow"
         """
         data = {'options': {"type": "automation"}}  # "type" is optional
@@ -104,107 +102,101 @@
 
         elif workflow_name:
             data["options"]["name"] = workflow_name
 
         else:
             raise AttributeError("Must have one of 'workflow_id' or 'workflow_name'.")
 
-        return client.call(method="POST", url=f"{client.url}/workflow_builder/export", json=data)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_builder/export", json=data)
 
-    @staticmethod
-    def get_schemas(client: "Itential", workflow_object: Dict[str, Any]) -> "requests.Response":
+    def get_schemas(self, workflow_object: Dict[str, Any]) -> "requests.Response":
         """
         Calculate incoming/outgoing schemas for the workflow
         https://apidocs.itential.com/2020.2/api/app-workflow_builder/getSchemas/
-        :param client: Itential state object
+
         :param workflow_object: A workflow json object.
         :return: requests.Response  200: {"inputSchema": {...}, "outputSchema": {...}}
         """
         data = {"workflow": workflow_object}
-        return client.call(method="POST", url=f"{client.url}/workflow_builder/workflows/schemas", json=data)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_builder/workflows/schemas", json=data)
 
-    @staticmethod
-    def get_task_details(client: "Itential", app_name: str, task_id: str) -> "requests.Response":
+    def get_task_details(self, app_name: str, task_id: str) -> "requests.Response":
         """
         Get Task Details
         https://apidocs.itential.com/2020.2/api/app-workflow_builder/getTaskDetails/
-        :param client: Itential state object
+
         :param app_name: Application Name (Export field in model)
         :param task_id: Task ID (Hexadecimal). < Unclear what this variable is >
         :return: requests.Response  200:
         """
-        return client.call(method="GET", url=f"{client.url}/getTaskDetails/{app_name}/{task_id}")
+        return self.client.call(method="GET", url=f"{self.client.url}/getTaskDetails/{app_name}/{task_id}")
 
-    @staticmethod
-    def get_tasks_list(client: "Itential") -> "requests.Response":
+    def get_tasks_list(self) -> "requests.Response":
         """
         Get all Tasks.
         https://apidocs.itential.com/2020.2/api/app-workflow_builder/getTasksList/
-        :param client: Itential state object
+
         :return: requests.Response
         """
-        return client.call(method="GET", url=f"{client.url}/workflow_builder/tasks/list")
+        return self.client.call(method="GET", url=f"{self.client.url}/workflow_builder/tasks/list")
 
-    @staticmethod
-    def list_workflow_groups(client: "Itential", workflow_name: str) -> "requests.Response":
+    def list_workflow_groups(self, workflow_name: str) -> "requests.Response":
         """
         List the groups that have access to a Workflow
         https://apidocs.itential.com/2020.2/api/app-workflow_builder/listWorkflowGroups/
-        :param client: Itential state object
+
         :param workflow_name: Name of the workflow to query
         :return: requests.Response
         """
-        return client.call(method="GET", url=f"{client.url}/workflow_builder/workflows/{workflow_name}/groups")
+        return self.client.call(
+            method="GET", url=f"{self.client.url}/workflow_builder/workflows/{workflow_name}/groups"
+        )
 
-    @staticmethod
-    def remove_workflow_group(client: "Itential", workflow_name: str, group_name: str) -> "requests.Response":
+    def remove_workflow_group(self, workflow_name: str, group_name: str) -> "requests.Response":
         """
         Remove a group from the list of authorized groups for a Workflow
         https://apidocs.itential.com/2020.2/api/app-workflow_builder/removeWorkflowGroup/
-        :param client: Itential state object
+
         :param workflow_name: Name of workflow to remove group from
         :param group_name: Name of group to remove from workflow.
         :return: requests.Response
         """
-        return client.call(
-            method="DELETE", url=f"{client.url}/workflow_builder/workflows/{workflow_name}/groups/{group_name}"
+        return self.client.call(
+            method="DELETE", url=f"{self.client.url}/workflow_builder/workflows/{workflow_name}/groups/{group_name}"
         )
 
-    @staticmethod
-    def rename_workflow(client: "Itential", workflow_object: Dict[str, Any], new_name: str) -> "requests.Response":
+    def rename_workflow(self, workflow_object: Dict[str, Any], new_name: str) -> "requests.Response":
         """
         Rename a Workflow in the database
         https://apidocs.itential.com/2020.2/api/app-workflow_builder/renameWorkflow/
-        :param client: Itential state object
+
         :param workflow_object: Current workflow object. Minimum requirements are {"_id": "", "name": ""}
         :param new_name: New workflow name.
         :return: requests.Response
         """
         data = {"workflow": workflow_object, "newName": new_name}
-        return client.call(method="POST", url=f"{client.url}/workflow_builder/workflows/rename", json=data)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_builder/workflows/rename", json=data)
 
-    @staticmethod
-    def replace_workflow_groups(client: "Itential", workflow_name: str, group_list: List[str]) -> "requests.Response":
+    def replace_workflow_groups(self, workflow_name: str, group_list: List[str]) -> "requests.Response":
         """
         Overwrite the list of groups that have access to a Workflow
         https://apidocs.itential.com/2020.2/api/app-workflow_builder/replaceWorkflowGroups/
-        :param client: Itential state object
+
         :param workflow_name: Name of the workflow
         :param group_list: List of group IDs (Hexadecimal)
         :return: requests.Response
         """
         data = {"groups": group_list}
-        return client.call(
-            method="PUT", url=f"{client.url}/workflow_builder/workflows/{workflow_name}/groups/", json=data
+        return self.client.call(
+            method="PUT", url=f"{self.client.url}/workflow_builder/workflows/{workflow_name}/groups/", json=data
         )
 
-    @staticmethod
-    def save_workflow(client: "Itential", workflow_obj: Dict[str, Any]) -> "requests.Response":
+    def save_workflow(self, workflow_obj: Dict[str, Any]) -> "requests.Response":
         """
         Add a Workflow to the database (Basically the save button)
         https://apidocs.itential.com/2020.2/api/app-workflow_builder/saveWorkflow/
-        :param client: Itential state object
+
         :param workflow_obj: Full workflow json
         :return: requests.Response
         """
         data = {"workflow": workflow_obj}
-        return client.call(method="POST", url=f"{client.url}/workflow_builder/workflows/save", json=data)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_builder/workflows/save", json=data)
```

### Comparing `itential.py-0.0.6/itential/modules/v2020_2/_app_workflow_engine.py` & `itential.py-1.0.0/itential/modules/v2020_2/_app_workflow_engine.py`

 * *Files 16% similar despite different names*

```diff
@@ -148,235 +148,217 @@
 if TYPE_CHECKING:
     from itential.core import Itential
 
 
 class AppWorkflowEngine:
     """https://apidocs.itential.com/2020.2/api/app-workflow_engine/"""
 
-    @staticmethod
-    def activate(client: "Itential", **kwargs: Dict[str, Any]) -> requests.Response:
+    def __init__(self, client: "Itential"):
+        self.client = client
+
+    def activate(self, **kwargs: Dict[str, Any]) -> requests.Response:
         """
         Activate Task Worker ( API payload not documented. May not be usable/implemented )
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/activate/
-        :param client: The Itential state object
         :param kwargs: Undocumented payload kwargs
         :return: Status flag of activation
         """
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/activate", json=kwargs)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/activate", json=kwargs)
 
-    @staticmethod
-    def add_watchers(client: "Itential", job_id: str, watchers: List[str]) -> requests.Response:
+    def add_watchers(self, job_id: str, watchers: List[str]) -> requests.Response:
         """
         Add users to the watchers list of a job by job ID and username.
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/addWatchers/
-        :param client: The Itential state object
+
         :param job_id: ID of the job to watch.
         :param watchers: Users to add to watchers list.
         :return: User IDs added to the watchers list.
         """
         body = {"job_id": job_id, "watchers": watchers}
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/job/watchers/watch", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/job/watchers/watch", json=body)
 
-    @staticmethod
-    def cancel_job(client: "Itential", job_id: str) -> requests.Response:
+    def cancel_job(self, job_id: str) -> requests.Response:
         """
         Cancel an active job by job ID.
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/cancelJob/
-        :param client: The Itential state object
+
         :param job_id: ID of the job to cancel.
         :return: Data from the canceled job.
         """
         body = {"job_id": job_id}
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/cancelJob", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/cancelJob", json=body)
 
-    @staticmethod
-    def check_workflow_for_job_variables(client: "Itential", workflow_name: str) -> requests.Response:
+    def check_workflow_for_job_variables(self, workflow_name: str) -> requests.Response:
         """
         Get job variables of a workflow by workflow name.
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/checkWorkflowForJobVariables/
-        :param client: The Itential state object
+
         :param workflow_name: Name of the workflow.
         :return: Variables of the workflow matching the name.
         """
-        return client.call(method="GET", url=f"{client.url}/workflow_engine/workflows/variables/{workflow_name}")
+        return self.client.call(
+            method="GET", url=f"{self.client.url}/workflow_engine/workflows/variables/{workflow_name}"
+        )
 
-    @staticmethod
-    def claim_task(client: "Itential", task_id: str, user: str) -> requests.Response:
+    def claim_task(self, task_id: str, user: str) -> requests.Response:
         """
         Claim a manual Task
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/claimTask/
-        :param client: The Itential state object
+
         :param task_id: ID of the Task to claim.
         :param user: User id for the user claiming the Task.
         :return: Result of claiming the Task.
         """
         body = {"task_id": task_id, "user": user}
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/tasks/claim", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/tasks/claim", json=body)
 
-    @staticmethod
-    def create_job_group_entry(client: "Itential", job_id: str, group_id: str) -> requests.Response:
+    def create_job_group_entry(self, job_id: str, group_id: str) -> requests.Response:
         """
         Add a group to the list of groups for a job.
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/createJobGroupEntry/
-        :param client: The Itential state object
+
         :param job_id: ID of job
         :param group_id: A Group id
         :return: Status of adding a group to a job.
         """
         body = {"group": group_id}
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/jobs/{job_id}/groups", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/jobs/{job_id}/groups", json=body)
 
-    @staticmethod
-    def deactivate(client: "Itential", **kwargs: Dict[str, Any]) -> requests.Response:
+    def deactivate(self, **kwargs: Dict[str, Any]) -> requests.Response:
         """
         Deactivate Task Worker ( API payload not documented. May not be usable/implemented )
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/deactivate/
-        :param client: The Itential state object
+
         :param kwargs: Undocumented POST payload
         :return: Status flag of deactivation
         """
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/deactivate", json=kwargs)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/deactivate", json=kwargs)
 
-    @staticmethod
-    def delete_job_groups(client: "Itential", job_id: str) -> requests.Response:
+    def delete_job_groups(self, job_id: str) -> requests.Response:
         """
         Remove all authorization restriction for a job.
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/deleteJobGroups/
-        :param client: The Itential state object
+
         :param job_id: ID of job
         :return: Status of Delete
         """
-        return client.call(method="DELETE", url=f"{client.url}/workflow_engine/jobs/{job_id}/groups")
+        return self.client.call(method="DELETE", url=f"{self.client.url}/workflow_engine/jobs/{job_id}/groups")
 
-    @staticmethod
-    def diff_to_html(client: "Itential", label1: str, value1: str, label2: str, value2: str) -> requests.Response:
+    def diff_to_html(self, label1: str, value1: str, label2: str, value2: str) -> requests.Response:
         """
         DEPRECIATED: Difference between two values in HTML response
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/diffToHTML/
-        :param client: The Itential state object
+
         :param label1: Optional label for value1
         :param value1: Any value to diff against value2
         :param label2: Optional label for value2
         :param value2: Any value to diff against value1
         :return: HTML difference between value1 and value2
         """
         warnings.warn("Marked as depreciated by Itential.", PendingDeprecationWarning)
         body = {"label1": label1, "value1": value1, "label2": label2, "value2": value2}
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/diffToHTML", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/diffToHTML", json=body)
 
-    @staticmethod
-    def find(client: "Itential", query: Dict[str, Any], options: Dict[str, Any]) -> requests.Response:
+    def find(self, query: Dict[str, Any], options: Dict[str, Any]) -> requests.Response:
         """
         Find job Documents based on a query and additional options.
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/find/
-        :param client: The Itential state object
+
         :param query: A MongoDB query object. See docs for an example
         :param options: A MongoDB options object. See docs for an example
         :return: Resulting job Documents that matched query and options.
         """
         body = {"query": query, "options": options}
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/jobs/find", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/jobs/find", json=body)
 
-    @staticmethod
     def find_forward_paths(
-        client: "Itential", start_task_id: str, end_task_id: str, workflow_details: Dict[str, Any]
+        self, start_task_id: str, end_task_id: str, workflow_details: Dict[str, Any]
     ) -> requests.Response:
         """
         Find the paths between two Tasks in a Workflow by Task ids and Workflow details.
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/findForwardPaths/
-        :param client: The Itential state object
+
         :param start_task_id: ID of the start Task.
         :param end_task_id: ID of the end Task.
         :param workflow_details: Workflow data which contain the tasks and transitions properties of the workflow.
         :return: All valid paths between the Tasks.
         """
         body = {"start_task": start_task_id, "end_task": end_task_id, "workflow_details": workflow_details}
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/findForwardPaths", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/findForwardPaths", json=body)
 
-    @staticmethod
-    def finish_manual_task(
-        client: "Itential", task_id: str, job_id: str, task_data: Dict[str, Any]
-    ) -> requests.Response:
+    def finish_manual_task(self, task_id: str, job_id: str, task_data: Dict[str, Any]) -> requests.Response:
         """
         Finishes a manual task with finish state success
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/finishManualTask/
-        :param client: The Itential state object
+
         :param task_id: ID of the Task within that job.
         :param job_id: ID of the Job.
         :param task_data: Data of the completed Task.
         :return: The Current Job Object
         """
         body = {"task_id": task_id, "job_id": job_id, "task_data": task_data}
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/finishTask", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/finishTask", json=body)
 
-    @staticmethod
-    def fix_job(client: "Itential", job_id: str, errored_task: str, revert_task: str) -> requests.Response:
+    def fix_job(self, job_id: str, errored_task: str, revert_task: str) -> requests.Response:
         """
         Revert an errored job to a target task by job ID and task names.
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/fixJob/
-        :param client: The Itential state object
+
         :param job_id: ID of the job to fix.
         :param errored_task: Name of the errored Task.
         :param revert_task: Name of the target Task.
         :return: Job after the revert.
         """
         body = {"job_id": job_id, "errored_task": errored_task, "revert_task": revert_task}
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/fixJob", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/fixJob", json=body)
 
-    @staticmethod
-    def get_all_loop_tasks(client: "Itential", workflow_details: Dict[str, Any]) -> requests.Response:
+    def get_all_loop_tasks(self, workflow_details: Dict[str, Any]) -> requests.Response:
         """
         Get all looped Tasks in a Workflow by Workflow details.
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/getAllLoopTasks/
-        :param client: The Itential state object
+
         :param workflow_details: Workflow to get looped tasks.
         :return: looped Tasks of the Workflow.
         """
         body = {"workflow_details": workflow_details}
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/getAllLoopTasks", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/getAllLoopTasks", json=body)
 
-    @staticmethod
-    def start_job_with_options(client: "Itential", workflow_name: str, options: Dict[str, Any]) -> requests.Response:
+    def start_job_with_options(self, workflow_name: str, options: Dict[str, Any]) -> requests.Response:
         """
         Initiate a job of a workflow with options.
-
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/startJobWithOptions/
 
-        :param client: The Itential state object
         :param workflow_name: Name of the workflow from which to start the job.
         :param options: Parameters to start the workflow with
             Ex: "options": {
                     "description": "str",
                     "variables": {
                         "incoming": {
                         ...
                         }
                     }
                 }
         :return: Job which is started.
         """
         body = {"options": options}
-        return client.call(
-            method="POST", url=f"{client.url}/workflow_engine/startJobWithOptions/{workflow_name}", json=body
+        return self.client.call(
+            method="POST", url=f"{self.client.url}/workflow_engine/startJobWithOptions/{workflow_name}", json=body
         )
 
-    @staticmethod
     def get_associated_jobs(
-        client: "Itential",
+        self,
         filters: Optional[Dict[str, str]] = None,
         sort: Optional[Dict[str, int]] = None,
         limit: int = 10,
         skip: int = 0,
     ) -> requests.Response:
         """
         Search for jobs that the user has touched.
-
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/getAssociatedJobs/
 
-        :param client: The Itential state object
         :param filters: Ex: {"metrics.user": "admin@pronghorn"} to filter for a specific user.
         :param skip: Number of jobs to offset the result. Useful for pagination.
         :param sort: {"name": -1} or {"name": 1}. "name" field can be any field in the workflow json.
         :param limit: Set to 0 to disable pagination.
         :return: All matching jobs. example json(): {"results": ["_id": int, "name": str],
          "skip": int, "limit": int, "total": int}
         """
@@ -391,101 +373,86 @@
 
         if filters:
             body["options"]["filter"] = filters
 
         if sort:
             body["options"]["sort"] = sort
 
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/getAllLoopTasks", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/getAllLoopTasks", json=body)
 
-    @staticmethod
-    def get_entire_job(client: "Itential", job_id: str) -> requests.Response:
+    def get_entire_job(self, job_id: str) -> requests.Response:
         """
         Get entire data of a job by job ID.
         Returns an "exploded" view, where data input into tasks is displayed in a schema view as opposed to the same
         format as it was originally passed in as. Contained about 20% more lines than get_job without containing any
         additional data.
-
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/getEntireJob/
 
-        :param client: Itential client object. Passed in to all commands
         :param job_id: Returned when creating a job or querying for jobs by workflow name.
          Ex: "ec59ef85fef84e59bf36bd1e"
         :return: requests.Response
         """
-        return client.call(method="GET", url=f"{client.url}/workflow_engine/getEntireJob/{job_id}")
+        return self.client.call(method="GET", url=f"{self.client.url}/workflow_engine/getEntireJob/{job_id}")
 
-    @staticmethod
-    def get_job(client: "Itential", job_id: str) -> requests.Response:
+    def get_job(self, job_id: str) -> requests.Response:
         """
         Get a job by job ID.
         The main difference between this endpoint and get_entire_job is that this endpoint seems to have more concise
         input layouts. Showing just the input json as it was passed in, instead of the input json as it is in the schema
         (more of an exploded schema view). About 20% more concise than get_entire_job (limited testing, ~2350 lines from
         get_entire_job down to ~1875 lines from get_job).
-
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/getJob/
 
-        :param client: Itential client object. Passed in to all commands
         :param job_id: Returned when creating a job or querying for jobs by workflow name.
          Ex: "ec59ef85fef84e59bf36bd1e"
         :return: requests.Response
         """
-        return client.call(method="GET", url=f"{client.url}/workflow_engine/getJob/{job_id}")
+        return self.client.call(method="GET", url=f"{self.client.url}/workflow_engine/getJob/{job_id}")
 
-    @staticmethod
-    def get_job_details(client: "Itential", job_id: str) -> requests.Response:
+    def get_job_details(self, job_id: str) -> requests.Response:
         """
         Get a job by job ID.
         Similar to get_job. Returns a smaller payload than get_job. Incoming json variables are shortened to the
         Itential variables (ex $var.60d8.merged_object) as opposed to the entire json being passed into a task. This
         endpoint also excludes some meta data like: created, created_by, last_updated, last_updated_by, etc
         Response is about 20% lighter than get_job (scaling with task input sizes) (1535 vs 1873 lines for same job)
-
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/getJobDetails/
 
-        :param client: Itential client object. Passed in to all commands
         :param job_id: Returned when creating a job or querying for jobs by workflow name.
          Ex: "ec59ef85fef84e59bf36bd1e"
         :return: requests.Response
         """
-        return client.call(method="GET", url=f"{client.url}/workflow_engine/job/{job_id}/details")
+        return self.client.call(method="GET", url=f"{self.client.url}/workflow_engine/job/{job_id}/details")
 
-    @staticmethod
-    def get_job_from_task_query(client: "Itential", task_query: str, options: Dict[str, Any]) -> requests.Response:
+    def get_job_from_task_query(self, task_query: str, options: Dict[str, Any]) -> requests.Response:
         """
         Search for jobs using a task query.
-
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/getJobFromTaskQuery/
 
-        :param client: Itential client object. Passed in to all commands
         :param task_query: A mongodb query partial to run against the tasks to get the requested job.
          Examples: {"status": "running"}
         :param options: Sort, filter, and pagination options.
          Examples: {"filter": {"name": "<workflowName>"}, "page": {"skip": 0, "limit": 50}, "sort:
           {"field": "name", "direction": 1}}
         :return: requests.Response. A list of full job objects
         """
         body = {"task_query": task_query, "options": options}
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/getJobFromTaskQuery", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/getJobFromTaskQuery", json=body)
 
-    @staticmethod
     def get_job_list(
-        client: "Itential",
+        self,
         status: str = "active",
         filters: Optional[Dict[str, str]] = None,
         limit: int = 10,
         skip: int = 0,
     ) -> requests.Response:
         """
         Get a list of jobs by status.
-
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/getJobList/
 
-        :param client: The Itential client state object, required for authentication with the server.
         :param filters: Ex: {"metrics.user": "admin@pronghorn"} to filter for a specific user.
         :param skip: Number of jobs to offset the result. Useful for pagination.
         :param status: Options: "active", "cancelled", "complete", "error", "incomplete", "paused", "running"
         :param limit: Set to 0 to disable pagination.
         :return: requests.Response
         """
 
@@ -497,326 +464,268 @@
                 "sort": {"field": "name", "direction": -1},
             }
         }
 
         if filters:
             body["options"]["filter"] = filters
 
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/getJobList/{status}", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/getJobList/{status}", json=body)
 
-    @staticmethod
-    def get_job_output(client: "Itential", job_id: str) -> requests.Response:
+    def get_job_output(self, job_id: str) -> requests.Response:
         """
         Get the output of a completed job.
-
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/getJobOutput/
 
-        :param client: Itential client object. Passed in to all commands
         :param job_id: Returned when creating a job or querying for jobs by workflow name.
          Ex: "ec59ef85fef84e59bf36bd1e"
         :return: requests.Response
         """
-        return client.call(method="GET", url=f"{client.url}/workflow_engine/job/{job_id}/output")
+        return self.client.call(method="GET", url=f"{self.client.url}/workflow_engine/job/{job_id}/output")
 
-    @staticmethod
-    def get_job_shallow(client: "Itential", job_id: str) -> requests.Response:
+    def get_job_shallow(self, job_id: str) -> requests.Response:
         """
         Get shallow data of a job by job ID. Returns a subset of data returned by omitting tasks' application, tasks'
         incoming arguments, tasks' returned data, and tasks' error information.
         About a 50% smaller payload than get_job (1535 vs 969)
-
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/getJobShallow/
 
-        :param client: Itential client object. Passed in to all commands
         :param job_id: Returned when creating a job or querying for jobs by workflow name.
          Ex: "ec59ef85fef84e59bf36bd1e"
         :return: requests.Response
         """
-        return client.call(method="GET", url=f"{client.url}/workflow_engine/getJobShallow/{job_id}")
+        return self.client.call(method="GET", url=f"{self.client.url}/workflow_engine/getJobShallow/{job_id}")
 
-    @staticmethod
-    def get_job_visualization_data(client: "Itential", job_id: str) -> requests.Response:
+    def get_job_visualization_data(self, job_id: str) -> requests.Response:
         """
         Get a job's visualization data by job ID.
-
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/getJobVisualizationData/
 
-        :param client: Itential client object. Passed in to all commands
         :param job_id: Returned when creating a job or querying for jobs by workflow name.
          Ex: "ec59ef85fef84e59bf36bd1e"
         :return: requests.Response
         """
-        return client.call(method="GET", url=f"{client.url}/workflow_engine/jobs/visdata/{job_id}")
+        return self.client.call(method="GET", url=f"{self.client.url}/workflow_engine/jobs/visdata/{job_id}")
 
-    @staticmethod
-    def get_manual_task_controller(client: "Itential", job_id: str, task_id: str) -> requests.Response:
+    def get_manual_task_controller(self, job_id: str, task_id: str) -> requests.Response:
         """
         Get a Manual Task's Controller (javascript function code)
-
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/getManualTaskController/
 
-        :param client: Itential client object. Passed in to all commands
         :param job_id: Returned when creating a job or querying for jobs by workflow name.
          Ex: "ec59ef85fef84e59bf36bd1e"
         :param task_id: ID of the task associated with the controller
 
         :return: requests.Response. Contains incoming and outgoing variables, error, and "TaskController"
          javascript code
         """
-        return client.call(
-            method="GET", url=f"{client.url}/workflow_engine/tasks/controller/job/{job_id}/task/{task_id}"
+        return self.client.call(
+            method="GET", url=f"{self.client.url}/workflow_engine/tasks/controller/job/{job_id}/task/{task_id}"
         )
 
-    @staticmethod
-    def get_task(client: "Itential", query: Dict[str, Any], filter: Dict[str, Any]) -> requests.Response:
+    def get_task(self, query: Dict[str, Any], filter: Dict[str, Any]) -> requests.Response:
         """
         Get the first Job's Task matching the query and return the data optionally modified by the filter.
-
         https://apidocs.itential.com/2020.2/api/-workflow_engine/getTask/
 
-        :param client: Itential client object. Passed in to all commands
         :param query: An object of property names and values to use in the query against the tasks collection.
          The property name must exist in the tasks collection. There must be at least 1 field you query upon.
          Ex: {"someFieldName": "value expected in field"}
         :param filter: Filter specifying which fields are returned. The structure of each property must conform to
          'fieldName': 1. Ex: {"name": 1} will return the name field
 
         :return: requests.Response.
         """
         body = {"query": query, "filter": filter}
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/getTask", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/getTask", json=body)
 
-    @staticmethod
-    def get_task_details(client: "Itential", location: str, package: str, method: str) -> requests.Response:
+    def get_task_details(self, location: str, package: str, method: str) -> requests.Response:
         """
         Get the detailed information model for a task. Documentation for this method is incomplete.
-
         https://apidocs.itential.com/2020.2/api/-workflow_engine/getTaskDetails/
 
-        :param client: Itential client object. Passed in to all commands
         :param location: Location: Application, Broker, Adapter
         :param package: Package name
         :param method: Method name
 
         :return: requests.Response.
          Ex: {
             "location": "Broker",
             "name": "query",
             "app": "WorkFlowEngine",
             "variables": {}
             }
         """
-        return client.call(
-            method="GET", url=f"{client.url}/workflow_engine/locations/{location}/packages/{package}/tasks/{method}"
+        return self.client.call(
+            method="GET",
+            url=f"{self.client.url}/workflow_engine/locations/{location}/packages/{package}/tasks/{method}",
         )
 
-    @staticmethod
-    def get_task_statuses(client: "Itential", job_id: str) -> requests.Response:
+    def get_task_statuses(self, job_id: str) -> requests.Response:
         """
         Get the status of each Task in a job by job ID.
-
         https://apidocs.itential.com/2020.2/api/-workflow_engine/getTaskStatuses/
 
-        :param client: Itential client object. Passed in to all commands
         :param job_id: Returned when creating a job or querying for jobs by workflow name.
          Ex: "ec59ef85fef84e59bf36bd1e"
 
         :return: requests.Response Statuses of all Tasks in the job.
         """
-        return client.call(method="GET", url=f"{client.url}/workflow_engine/job/statuses/{job_id}")
+        return self.client.call(method="GET", url=f"{self.client.url}/workflow_engine/job/statuses/{job_id}")
 
-    @staticmethod
-    def get_workflows_detailed_by_name(client: "Itential", workflow_name: str) -> requests.Response:
+    def get_workflows_detailed_by_name(self, workflow_name: str) -> requests.Response:
         """
         Get the status of each Task in a job by job ID.
-
         https://apidocs.itential.com/2020.2/api/-workflow_engine/getWorkflowsDetailedByName/
 
-        :param client: Itential client object. Passed in to all commands
         :param workflow_name: Name of the workflow.
         :return: requests.Response Workflow details matching the Workflow name
         """
-        return client.call(method="GET", url=f"{client.url}/workflow_engine/workflows/detailed/{workflow_name}")
+        return self.client.call(
+            method="GET", url=f"{self.client.url}/workflow_engine/workflows/detailed/{workflow_name}"
+        )
 
-    @staticmethod
-    def is_active(client: "Itential") -> requests.Response:
+    def is_active(self) -> requests.Response:
         """
         Check if Staterator is currently active
-
         https://apidocs.itential.com/2020.2/api/-workflow_engine/isActive/
 
-        :param client: Itential client object. Passed in to all commands
         :return: requests.Response Active flag for Staterator
         """
-        return client.call(method="GET", url=f"{client.url}/workflow_engine/active")
+        return self.client.call(method="GET", url=f"{self.client.url}/workflow_engine/active")
 
-    @staticmethod
-    def list_job_groups(client: "Itential", job_id: str) -> requests.Response:
+    def list_job_groups(self, job_id: str) -> requests.Response:
         """
         List the groups that have access to a job.
-
         https://apidocs.itential.com/2020.2/api/-workflow_engine/listJobGroups/
 
-        :param client: Itential client object. Passed in to all commands
         :param job_id: Returned when creating a job or querying for jobs by workflow name.
          Ex: "ec59ef85fef84e59bf36bd1e"
         :return: requests.Response List of Group IDs.
         """
-        return client.call(method="GET", url=f"{client.url}/workflow_engine/jobs/{job_id}/groups")
+        return self.client.call(method="GET", url=f"{self.client.url}/workflow_engine/jobs/{job_id}/groups")
 
-    @staticmethod
-    def pause_job(client: "Itential", job_id: str) -> requests.Response:
+    def pause_job(self, job_id: str) -> requests.Response:
         """
         Pause a job by job ID.
-
         https://apidocs.itential.com/2020.2/api/-workflow_engine/pauseJob/
 
-        :param client: Itential client object. Passed in to all commands
         :param job_id: Returned when creating a job or querying for jobs by workflow name.
          Ex: "ec59ef85fef84e59bf36bd1e"
         :return: requests.Response Job after the pause.
         """
         body = {"job_id": job_id}
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/pauseJob", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/pauseJob", json=body)
 
-    @staticmethod
-    def prepare_metrics_logs(client: "Itential") -> requests.Response:
+    def prepare_metrics_logs(self) -> requests.Response:
         """
         Compress the metrics logs directory for Jobs and return the link to download it.
-
         https://apidocs.itential.com/2020.2/api/-workflow_engine/prepareMetricsLogs/
 
-        :param client: Itential client object. Passed in to all commands
         :return: requests.Response URL containing the compressed job metrics zipped file
         """
-        return client.call(method="GET", url=f"{client.url}/workflow_engine/metrics/jobs")
+        return self.client.call(method="GET", url=f"{self.client.url}/workflow_engine/metrics/jobs")
 
-    @staticmethod
-    def query_jobs(client: "Itential", query: Dict[str, Any]) -> requests.Response:
+    def query_jobs(self, query: Dict[str, Any]) -> requests.Response:
         """
         Get jobs matching the query.
-
         https://apidocs.itential.com/2020.2/api/-workflow_engine/queryJobs/
 
-        :param client: Itential client object. Passed in to all commands
         :param query: An object of property names and values to use in the query against the jobs collection.
          The property name must exist in the jobs collection. There must be at least 1 field you query upon.
          Ex: {"query": {"someFieldName": "Some Value to query the against the someFieldName property"}}
         :return: requests.Response All jobs matching the query.
         """
         body = {"query": query}
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/queryJobs", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/queryJobs", json=body)
 
-    @staticmethod
-    def query_tasks_brief(client: "Itential", query: Dict[str, Any]) -> requests.Response:
+    def query_tasks_brief(self, query: Dict[str, Any]) -> requests.Response:
         """
         Get brief information about task(s) from the tasks collection in mongoDB.
         This will return only tasks that are attached to a currently running Job
-
         https://apidocs.itential.com/2020.2/api/-workflow_engine/queryTasksBrief/
 
-        :param client: Itential client object. Passed in to all commands
         :param query: An object of property names and values to use in the query against the jobs collection.
          The property name must exist in the jobs collection. There must be at least 1 field you query upon.
          Ex: {"query": {"someFieldName": "Some Value to query the against the someFieldName property"}}
         :return: requests.Response Jobs' Tasks matching the query.
         """
         body = {"query": query}
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/queryTasksBrief", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/queryTasksBrief", json=body)
 
-    @staticmethod
-    def release_task(client: "Itential", task_id: str) -> requests.Response:
+    def release_task(self, task_id: str) -> requests.Response:
         """
         Get brief information about task(s) from the tasks collection in mongoDB.
         This will return only tasks that are attached to a currently running Job
-
         https://apidocs.itential.com/2020.2/api/-workflow_engine/releaseTask/
 
-        :param client: Itential client object. Passed in to all commands
         :param task_id: ID of a specific task. Ex: "cd34"
         :return: requests.Response Task details after releasing the Task.
         """
         body = {"task_id": task_id}
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/tasks/release", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/tasks/release", json=body)
 
-    @staticmethod
-    def remove_job_group(client: "Itential", job_id: str, group_id: str) -> requests.Response:
+    def remove_job_group(self, job_id: str, group_id: str) -> requests.Response:
         """
         Remove a group from the list of authorized groups for a job.
-
         https://apidocs.itential.com/2020.2/api/-workflow_engine/removeJobGroup/
 
-        :param client: Itential client object. Passed in to all commands
         :param job_id: Returned when creating a job or querying for jobs by workflow name.
          Ex: "ec59ef85fef84e59bf36bd1e"
         :param group_id: ID of a group. Ex:
         :return: requests.Response Status of the removal of a group from a job.
         """
-        return client.call(method="DELETE", url=f"{client.url}/workflow_engine/jobs/{job_id}/groups/{group_id}")
+        return self.client.call(
+            method="DELETE", url=f"{self.client.url}/workflow_engine/jobs/{job_id}/groups/{group_id}"
+        )
 
-    @staticmethod
-    def replace_job_groups(client: "Itential", job_id: str, group_list: List[str]) -> requests.Response:
+    def replace_job_groups(self, job_id: str, group_list: List[str]) -> requests.Response:
         """
         Overwrite the list of groups that have access to a job.
-
         https://apidocs.itential.com/2020.2/api/-workflow_engine/replaceJobGroups/
 
-        :param client: Itential client object. Passed in to all commands
         :param job_id: Returned when creating a job or querying for jobs by workflow name.
          Ex: "ec59ef85fef84e59bf36bd1e"
         :param group_list: List of group IDs
         :return: requests.Response Status of the removal of a group from a job.
         """
         body = {"groups": group_list}
-        return client.call(method="PUT", url=f"{client.url}/workflow_engine/jobs/{job_id}/groups", json=body)
+        return self.client.call(method="PUT", url=f"{self.client.url}/workflow_engine/jobs/{job_id}/groups", json=body)
 
-    @staticmethod
-    def resume_job(client: "Itential", job_id: str) -> requests.Response:
+    def resume_job(self, job_id: str) -> requests.Response:
         """
         Resume a paused or errored job by job ID.
-
         https://apidocs.itential.com/2020.2/api/-workflow_engine/resumeJob/
 
-        :param client: Itential client object. Passed in to all commands
         :param job_id: Returned when creating a job or querying for jobs by workflow name.
          Ex: "ec59ef85fef84e59bf36bd1e"
         :return: requests.Response Job after the resume.
         """
         body = {"job_id": job_id}
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/resumeJob", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/resumeJob", json=body)
 
-    @staticmethod
-    def revert_to_task(client: "Itential", job_id: str, current_task_id: str, target_task_id: str) -> requests.Response:
+    def revert_to_task(self, job_id: str, current_task_id: str, target_task_id: str) -> requests.Response:
         """
         Revert a job from current Task to the target task by job ID and task names.
-
         https://apidocs.itential.com/2020.2/api/-workflow_engine/revertToTask/
 
-        :param client: Itential client object. Passed in to all commands
         :param job_id: Returned when creating a job or querying for jobs by workflow name.
          Ex: "ec59ef85fef84e59bf36bd1e"
         :param current_task_id: Name of the current Task.
         :param target_task_id: Name of the Target Task.
         :return: requests.Response Job after the revert.
         """
         body = {"job_id": job_id, "current_task": current_task_id, "target_task": target_task_id}
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/revertToTask", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/revertToTask", json=body)
 
-    @staticmethod
-    def run_evaluation_group(
-        client: "Itential", evaluation_group: List[Dict[str, Any]], all_true_flag: bool
-    ) -> requests.Response:
+    def run_evaluation_group(self, evaluation_group: List[Dict[str, Any]], all_true_flag: bool) -> requests.Response:
         """
         Run a test evaluation.
-
         Note: This might be an accidentally exposed endpoint for the "evaluation" task within a workflow.
-
         https://apidocs.itential.com/2020.2/api/-workflow_engine/runEvaluationGroup/
 
-        :param client: Itential client object. Passed in to all commands
         :param evaluation_group: Array of evaluations to run
         :param all_true_flag: All evaluation groups must pass, or not
         :return: requests.Response Result of evaluation.
         Ex:
             {
               "evaluation_group": [
                 {
@@ -834,28 +743,22 @@
               "all_true_flag": true
             }
         """
         body = {
             "evaluation_group": evaluation_group,
             "all_true_flag": all_true_flag,
         }
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/runEvaluationGroup", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/runEvaluationGroup", json=body)
 
-    @staticmethod
-    def run_evaluation_groups(
-        client: "Itential", evaluation_group: List[Dict[str, Any]], all_true_flag: bool
-    ) -> requests.Response:
+    def run_evaluation_groups(self, evaluation_group: List[Dict[str, Any]], all_true_flag: bool) -> requests.Response:
         """
         Run a test evaluation.
-
         Note: This might be an accidentally exposed endpoint for the "evaluation" task within a workflow.
-
         https://apidocs.itential.com/2020.2/api/-workflow_engine/runEvaluationGroups/
 
-        :param client: Itential client object. Passed in to all commands
         :param evaluation_group: Array of evaluations to run
         :param all_true_flag: All evaluation groups must pass, or not
         :return: requests.Response Result of evaluation.
         Ex:
             {
               "evaluation_group": [
                 {
@@ -879,48 +782,42 @@
               "all_true_flag": true
             }
         """
         body = {
             "evaluation_group": evaluation_group,
             "all_true_flag": all_true_flag,
         }
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/runEvaluationGroups", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/runEvaluationGroups", json=body)
 
-    @staticmethod
-    def run_validation(client: "Itential", workflow_json: Dict[str, Any]) -> requests.Response:
+    def run_validation(self, workflow_json: Dict[str, Any]) -> requests.Response:
         """
         Validate a workflow, and return the resulting errors and warnings arrays.
-
         https://apidocs.itential.com/2020.2/api/-workflow_engine/runValidation/
 
-        :param client: Itential client object. Passed in to all commands
         :param workflow_json: The workflow object to run validations against.
         :return: requests.Response Errors and warnings output from the validation process
         """
         body = {"workflow": workflow_json}
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/workflows/validate", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/workflows/validate", json=body)
 
-    @staticmethod
     def search_jobs(
-        client: "Itential",
+        self,
         expand: Optional[List[str]] = None,
         query: Optional[Dict[str, str]] = None,
         fields: Optional[Dict[str, int]] = None,
         local: Optional[bool] = True,
         sort: Optional[Dict[str, int]] = None,
         limit: int = 0,
         skip: int = 0,
     ) -> requests.Response:
         """
         TODO: Needs testing to identify what each param actually means. Documentation is very lacking.
         Search jobs with Options. This is similar to search_workflows, but with some additional fields.
-
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/searchJobs/
 
-        :param client: The Itential client state object
         :param expand: {"expand": ["user"]}.
         :param query: {"name": "workflow_name"}. "name" field can be any field in the workflow json.
         :param fields: {"name": 1}. "name" field can be any field in the workflow json.
          Used to filter out other fields
         :param sort: {"name": -1} or {"name": 1}. "name" field can be any field in the workflow json.
         :param limit: Max results to return
         :param local:
@@ -961,37 +858,33 @@
 
         if fields:
             data["options"]["fields"] = fields
 
         if sort:
             data["options"]["sort"] = sort
 
-        return client.call(method="POST", url=rf"{client.url}/workflow_engine/jobs/search", json=data)
+        return self.client.call(method="POST", url=rf"{self.client.url}/workflow_engine/jobs/search", json=data)
 
-    @staticmethod
     def search_tasks(
-        client: "Itential",
+        self,
         filter: Dict[str, Any],
         expand: Optional[List[str]] = None,
         query: Optional[Dict[str, str]] = None,
         fields: Optional[Dict[str, int]] = None,
         local: Optional[bool] = True,
         sort: Optional[Dict[str, int]] = None,
         limit: int = 0,
         skip: int = 0,
     ) -> requests.Response:
         """
         TODO: Needs testing to identify what each param actually means. Documentation is very lacking.
         Search jobs with Options.
-
         Note: Unique in that it has an additional parameter "filter".
-
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/searchTasks/
 
-        :param client: The Itential client state object
         :param filter: Search Filter Ex: {"someFieldName": "Some Value to query the against the someFieldName property"}
         :param expand: {"expand": ["user"]}.
         :param query: {"name": "workflow_name"}. "name" field can be any field in the workflow json.
         :param fields: {"name": 1}. "name" field can be any field in the workflow json.
          Used to filter out other fields
         :param sort: {"name": -1} or {"name": 1}. "name" field can be any field in the workflow json.
         :param limit: Max results to return
@@ -1040,31 +933,28 @@
 
         if fields:
             data["options"]["fields"] = fields
 
         if sort:
             data["options"]["sort"] = sort
 
-        return client.call(method="POST", url=rf"{client.url}/workflow_engine/tasks/search", json=data)
+        return self.client.call(method="POST", url=rf"{self.client.url}/workflow_engine/tasks/search", json=data)
 
-    @staticmethod
     def search_workflows(
-        client: "Itential",
+        self,
         query: Optional[Dict[str, str]] = None,
         fields: Optional[Dict[str, int]] = None,
         sort: Optional[Dict[str, int]] = None,
         limit: int = 0,
         skip: int = 0,
     ) -> requests.Response:
         """
         Search Workflows with Options
-
         https://apidocs.itential.com/2020.2/api/app-workflow_engine/searchWorkflows/
 
-        :param client: The Itential client state object
         :param query: {"name": "workflow_name"}. "name" field can be any field in the workflow json.
         :param fields: {"name": 1}. "name" field can be any field in the workflow json.
          Used to filter out other fields
         :param sort: {"name": -1} or {"name": 1}. "name" field can be any field in the workflow json.
         :param limit: Max results to return
         :param skip: Number to offset the search by
         :return: requests.Response example json(): {"results": ["_id": int, "name": str], "skip": int,
@@ -1078,48 +968,39 @@
 
         if fields:
             data["options"]["fields"] = fields
 
         if sort:
             data["options"]["sort"] = sort
 
-        return client.call(method="POST", url=rf"{client.url}/workflow_engine/workflows/search", json=data)
+        return self.client.call(method="POST", url=rf"{self.client.url}/workflow_engine/workflows/search", json=data)
 
-    @staticmethod
-    def unwatch_job(client: "Itential", job_id: str) -> requests.Response:
+    def unwatch_job(self, job_id: str) -> requests.Response:
         """
         Remove the current user from the watchers list of a job.
-
         https://apidocs.itential.com/2020.2/api/-workflow_engine/unwatchJob/
 
-        :param client: Itential client object. Passed in to all commands
         :param job_id: ID of the job
         :return: requests.Response User id removed from the watchers list.
         """
-        return client.call(method="DELETE", url=f"{client.url}/workflow_engine/job/{job_id}/watch")
+        return self.client.call(method="DELETE", url=f"{self.client.url}/workflow_engine/job/{job_id}/watch")
 
-    @staticmethod
-    def validate_all_loops(client: "Itential", workflow_json: Dict[str, Any]) -> requests.Response:
+    def validate_all_loops(self, workflow_json: Dict[str, Any]) -> requests.Response:
         """
         Validate all looped Tasks in a Workflow by Workflow details.
-
         https://apidocs.itential.com/2020.2/api/-workflow_engine/validateAllLoops/
 
-        :param client: Itential client object. Passed in to all commands
         :param workflow_json: Full workflow json/dict
         :return: requests.Response User id removed from the watchers list.
         """
         body = {"workflow_details": workflow_json}
-        return client.call(method="POST", url=f"{client.url}/workflow_engine/validateAllLoops", json=body)
+        return self.client.call(method="POST", url=f"{self.client.url}/workflow_engine/validateAllLoops", json=body)
 
-    @staticmethod
-    def watch_job(client: "Itential", job_id: str) -> requests.Response:
+    def watch_job(self, job_id: str) -> requests.Response:
         """
         Add current user to a job's watchers list.
-
         https://apidocs.itential.com/2020.2/api/-workflow_engine/watchJob/
 
-        :param client: Itential client object. Passed in to all commands
         :param job_id: ID of the job
         :return: requests.Response User id added to the watchers list.
         """
-        return client.call(method="PUT", url=f"{client.url}/workflow_engine/job/{job_id}/watch")
+        return self.client.call(method="PUT", url=f"{self.client.url}/workflow_engine/job/{job_id}/watch")
```

### Comparing `itential.py-0.0.6/itential/modules/v2020_2/_pronghorn_core.py` & `itential.py-1.0.0/itential/modules/v2020_2/_pronghorn_core.py`

 * *Files identical despite different names*

### Comparing `itential.py-0.0.6/itential.py.egg-info/PKG-INFO` & `itential.py-1.0.0/itential.py.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itential.py
-Version: 0.0.6
+Version: 1.0.0
 Summary: A Python wrapper for the Itential API.
 Author: Tagmeh
 License: The MIT License (MIT)
         
         Copyright (c) 2022-present John Epperson
         
         Permission is hereby granted, free of charge, to any person obtaining a
@@ -36,22 +36,34 @@
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Itential.py
+A library to (hopefully) make Itential scripting via Python a little easier.
 
-#### An effort to write a python library for the Itential API. (https://apidocs.itential.com/2021.2/api/) (New Link to Old Docs)
-
-8.5.2022 - I took a break after Itential updated their documentation, and broke all of their existing links (including every link I had posted in the method doc strings...). Pretty demoralizing, and a month or so after the Great Link Breakin'ing, they are still all broken. But, my motivation has returned, and work will continue. I plan on getting this pushed out as a package as quickly as possible.
+Pypi: https://pypi.org/project/itential.py/
 
+## Remote Install
+```text
+pip install itential.py
+```
 
-Usage
+## Usage
 ```python
 from itential import Itential
 from itential.modules.v2020_2 import AppWorkflowEngine
 
 client = Itential()  # Contains default login and localhost url information
 
-response: "requests.Response" = AppWorkflowEngine.get_job_output(client=client, job_id="example-job-id")
+workflow_engine = AppWorkflowEngine(client=client)  # Pass in the auth client
+
+response: "requests.Response" = workflow_engine.get_job_output(job_id="example-job-id")
+```
+
+## Local Install
+Curently the repository is setup for pipenv. I'm looking into making the repository agnostic to the python environment manager (poetry, pipnev, venv).
+```text
+pip install pipenv
+pipenv install . --dev
 ```
```

### Comparing `itential.py-0.0.6/itential.py.egg-info/SOURCES.txt` & `itential.py-1.0.0/itential.py.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -28,9 +28,10 @@
 itential/modules/v2020_2/_app_task_worker.py
 itential/modules/v2020_2/_app_template_builder.py
 itential/modules/v2020_2/_app_workflow_builder.py
 itential/modules/v2020_2/_app_workflow_engine.py
 itential/modules/v2020_2/_pronghorn_core.py
 itential/modules/v2021_1/__init__.py
 itential/modules/v2021_1/_app_form_builder.py
+itential/modules/v2021_1/_app_workflow_builder.py
 itential/modules/v2021_2/__init__.py
 itential/modules/v2021_2/_app_form_builder.py
```

### Comparing `itential.py-0.0.6/pyproject.toml` & `itential.py-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "itential.py"
-version = "0.0.6"
+version = "1.0.0"
 authors = [{ name = "Tagmeh" }]
 description = "A Python wrapper for the Itential API."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -14,15 +14,15 @@
     "Natural Language :: English",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
-    "requests"
+    "requests ~= 2.28"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/tagmeh/Itential.py"
 "Bug Tracker" = "https://github.com/tagmeh/Itential.py/issues"
 
 [build-system]
```

