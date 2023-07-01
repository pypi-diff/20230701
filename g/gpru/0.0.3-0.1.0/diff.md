# Comparing `tmp/gpru-0.0.3.tar.gz` & `tmp/gpru-0.1.0.tar.gz`

## Comparing `gpru-0.0.3.tar` & `gpru-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/__about__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/__init__.py
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/_client.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/_logger.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/azure/__init__.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/azure/_api.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/azure/_utils.py
--rw-r--r--   0        0        0    37103 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/azure/preview_2022_03_01.py
--rw-r--r--   0        0        0    40310 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/azure/preview_2022_06_01.py
--rw-r--r--   0        0        0    54413 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/azure/preview_2023_03_15.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/azure/py.typed
--rw-r--r--   0        0        0    46831 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/azure/stable_2022_12_01.py
--rw-r--r--   0        0        0    49072 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/azure/stable_2023_05_15.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/openai/__init__.py
--rw-r--r--   0        0        0    55082 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/openai/api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.3/gpru/openai/py.typed
--rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 gpru-0.0.3/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 gpru-0.0.3/LICENSE
--rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 gpru-0.0.3/README.md
--rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 gpru-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 gpru-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/__about__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/__init__.py
+-rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/_client.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/_logger.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/azure/__init__.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/azure/_api.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/azure/_utils.py
+-rw-r--r--   0        0        0    37103 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/azure/preview_2022_03_01.py
+-rw-r--r--   0        0        0    40310 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/azure/preview_2022_06_01.py
+-rw-r--r--   0        0        0    54413 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/azure/preview_2023_03_15.py
+-rw-r--r--   0        0        0    59066 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/azure/preview_2023_06_01.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/azure/py.typed
+-rw-r--r--   0        0        0    46831 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/azure/stable_2022_12_01.py
+-rw-r--r--   0        0        0    49153 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/azure/stable_2023_05_15.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/openai/__init__.py
+-rw-r--r--   0        0        0    55082 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/openai/api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.1.0/gpru/openai/py.typed
+-rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 gpru-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 gpru-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 gpru-0.1.0/README.md
+-rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 gpru-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 gpru-0.1.0/PKG-INFO
```

### Comparing `gpru-0.0.3/gpru/_client.py` & `gpru-0.1.0/gpru/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 _API_FAILED = "API request failed."
 _IMPLEMENTATION_ERROR = f"Implementation error in gpru@{__version__}."
 
 
 def _raise_api_error(error_response_model: Type[T], response: httpx.Response) -> None:
     logger.error(_API_FAILED)
+    logger.debug(response.json())
     error_response = error_response_model.parse_obj(response.json())
     error = error_response.error if hasattr(error_response, "error") else error_response
     raise ApiError(response.status_code, error)
 
 
 def _retry_condition(e: BaseException) -> bool:
     if type(e) == ApiError:
```

### Comparing `gpru-0.0.3/gpru/exceptions.py` & `gpru-0.1.0/gpru/exceptions.py`

 * *Files identical despite different names*

### Comparing `gpru-0.0.3/gpru/azure/_api.py` & `gpru-0.1.0/gpru/azure/_api.py`

 * *Files identical despite different names*

### Comparing `gpru-0.0.3/gpru/azure/preview_2022_03_01.py` & `gpru-0.1.0/gpru/azure/preview_2022_03_01.py`

 * *Files identical despite different names*

### Comparing `gpru-0.0.3/gpru/azure/preview_2022_06_01.py` & `gpru-0.1.0/gpru/azure/preview_2022_06_01.py`

 * *Files identical despite different names*

### Comparing `gpru-0.0.3/gpru/azure/preview_2023_03_15.py` & `gpru-0.1.0/gpru/azure/preview_2023_03_15.py`

 * *Files identical despite different names*

### Comparing `gpru-0.0.3/gpru/azure/stable_2022_12_01.py` & `gpru-0.1.0/gpru/azure/stable_2022_12_01.py`

 * *Files identical despite different names*

### Comparing `gpru-0.0.3/gpru/azure/stable_2023_05_15.py` & `gpru-0.1.0/gpru/azure/stable_2023_05_15.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 from typing import Any, Dict, Generator, List, Optional, Union
 
 from httpx._config import DEFAULT_TIMEOUT_CONFIG
 from httpx._types import TimeoutTypes
 from pydantic import BaseModel, Field
 
 from gpru.azure._api import Api
+from gpru.azure._utils import deprecation_warning
+
+deprecation_warning(__name__)
 
 
 class ErrorCode(str, Enum):
     """
     Error codes as defined in the Microsoft REST guidelines.
 
     See Also
```

### Comparing `gpru-0.0.3/gpru/openai/api.py` & `gpru-0.1.0/gpru/openai/api.py`

 * *Files identical despite different names*

### Comparing `gpru-0.0.3/.gitignore` & `gpru-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gpru-0.0.3/LICENSE` & `gpru-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpru-0.0.3/README.md` & `gpru-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 | `AZURE_OPENAI_API_ENDPOINT`      | URL in the form of `https://{your-resource-name}.openai.azure.com/`. |
 | `AZURE_OPENAI_API_KEY`           | Secret key.                                                          |
 | `AZURE_OPENAI_API_DEPLOYMENT_ID` | Custom name you chose for your deployment when you deployed a model. |
 
 ```python
 import os
 
-from gpru.azure.stable_2023_05_15 import (
+from gpru.azure.preview_2023_06_01 import (
     AzureOpenAiApi,
     ChatCompletionRequest,
     UserMessage,
 )
 
 endpoint = os.environ["AZURE_OPENAI_API_ENDPOINT"]
 key = os.environ["AZURE_OPENAI_API_KEY"]
```

### Comparing `gpru-0.0.3/pyproject.toml` & `gpru-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 [tool.hatch.version]
 path = "src/gpru/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]",
-  "datamodel-code-generator[http]<0.18", # https://docs.pydantic.dev/latest/datamodel_code_generator/
+  "datamodel-code-generator[http]", # https://docs.pydantic.dev/latest/datamodel_code_generator/
   "pre-commit",
   "pytest",
 ]
 
 [tool.hatch.envs.default.scripts]
 cov = [
   "test-cov",
@@ -178,14 +178,15 @@
   "S101",
   "FBT",
   "A",
   "COM",
   "FA100",
   "G004",
   "INP",
+  "SLOT000",
   "ERA",
   "PLR2004",
   "TRY300",
 ]
 line-length = 88
 select = ["ALL"]
 target-version = "py37"
@@ -197,12 +198,13 @@
 known-first-party = ["gpru"]
 
 [tool.ruff.mccabe]
 max-complexity = 5
 
 [tool.ruff.per-file-ignores]
 "examples/**/*" = ["T201"]
+"examples/azure/**/*extension*.py" = ["E501"]
 "examples/openai/*_audio.py" = ["E501"]
 "tests/**/*" = ["D10"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
```

### Comparing `gpru-0.0.3/PKG-INFO` & `gpru-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpru
-Version: 0.0.3
+Version: 0.1.0
 Summary: Unofficial Python client library for the OpenAI and Azure OpenAI APIs
 Project-URL: Documentation, https://github.com/sincekmori/gpru#readme
 Project-URL: Issues, https://github.com/sincekmori/gpru/issues
 Project-URL: Source, https://github.com/sincekmori/gpru
 Author-email: Shinsuke Mori <sincekmori@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -102,15 +102,15 @@
 | `AZURE_OPENAI_API_ENDPOINT`      | URL in the form of `https://{your-resource-name}.openai.azure.com/`. |
 | `AZURE_OPENAI_API_KEY`           | Secret key.                                                          |
 | `AZURE_OPENAI_API_DEPLOYMENT_ID` | Custom name you chose for your deployment when you deployed a model. |
 
 ```python
 import os
 
-from gpru.azure.stable_2023_05_15 import (
+from gpru.azure.preview_2023_06_01 import (
     AzureOpenAiApi,
     ChatCompletionRequest,
     UserMessage,
 )
 
 endpoint = os.environ["AZURE_OPENAI_API_ENDPOINT"]
 key = os.environ["AZURE_OPENAI_API_KEY"]
```

