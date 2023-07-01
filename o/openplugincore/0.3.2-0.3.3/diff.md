# Comparing `tmp/openplugincore-0.3.2.tar.gz` & `tmp/openplugincore-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugincore-0.3.2.tar", last modified: Sat Jul  1 18:06:11 2023, max compression
+gzip compressed data, was "openplugincore-0.3.3.tar", last modified: Sat Jul  1 19:33:22 2023, max compression
```

## Comparing `openplugincore-0.3.2.tar` & `openplugincore-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 18:06:11.184897 openplugincore-0.3.2/
--rw-rw-rw-   0        0        0      826 2023-07-01 18:06:11.183899 openplugincore-0.3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-01 18:06:11.150898 openplugincore-0.3.2/openplugincore/
--rw-rw-rw-   0        0        0       61 2023-07-01 15:22:26.000000 openplugincore-0.3.2/openplugincore/__init__.py
--rw-rw-rw-   0        0        0     9291 2023-07-01 15:16:30.000000 openplugincore-0.3.2/openplugincore/openplugincore.py
--rw-rw-rw-   0        0        0    19151 2023-07-01 05:38:42.000000 openplugincore-0.3.2/openplugincore/plugins.json
--rw-rw-rw-   0        0        0      696 2023-06-27 03:28:44.000000 openplugincore-0.3.2/openplugincore/types.py
-drwxrwxrwx   0        0        0        0 2023-07-01 18:06:11.175898 openplugincore-0.3.2/openplugincore.egg-info/
--rw-rw-rw-   0        0        0      826 2023-07-01 18:06:11.000000 openplugincore-0.3.2/openplugincore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2023-07-01 18:06:11.000000 openplugincore-0.3.2/openplugincore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 18:06:11.000000 openplugincore-0.3.2/openplugincore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-01 18:06:11.000000 openplugincore-0.3.2/openplugincore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-01 18:06:11.000000 openplugincore-0.3.2/openplugincore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 18:06:11.184897 openplugincore-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1515 2023-07-01 18:06:08.000000 openplugincore-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 18:06:11.181901 openplugincore-0.3.2/tests/
--rw-rw-rw-   0        0        0        0 2023-06-30 23:02:19.000000 openplugincore-0.3.2/tests/__init__.py
--rw-rw-rw-   0        0        0     1589 2023-07-01 01:03:27.000000 openplugincore-0.3.2/tests/mock_data.py
--rw-rw-rw-   0        0        0     2491 2023-07-01 15:22:55.000000 openplugincore-0.3.2/tests/test_basicTest.py
--rw-rw-rw-   0        0        0    13215 2023-07-01 15:23:05.000000 openplugincore-0.3.2/tests/test_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:33:22.414908 openplugincore-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-01 19:33:22.410908 openplugincore-0.3.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:33:22.410908 openplugincore-0.3.3/openplugincore/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-01 19:33:07.000000 openplugincore-0.3.3/openplugincore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-07-01 19:33:07.000000 openplugincore-0.3.3/openplugincore/openplugincore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17627 2023-07-01 19:33:07.000000 openplugincore-0.3.3/openplugincore/plugins.json
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-01 19:33:07.000000 openplugincore-0.3.3/openplugincore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:33:22.410908 openplugincore-0.3.3/openplugincore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-01 19:33:22.000000 openplugincore-0.3.3/openplugincore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-01 19:33:22.000000 openplugincore-0.3.3/openplugincore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 19:33:22.000000 openplugincore-0.3.3/openplugincore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-01 19:33:22.000000 openplugincore-0.3.3/openplugincore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-01 19:33:22.000000 openplugincore-0.3.3/openplugincore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 19:33:22.414908 openplugincore-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-01 19:33:07.000000 openplugincore-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:33:22.410908 openplugincore-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:33:07.000000 openplugincore-0.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-01 19:33:07.000000 openplugincore-0.3.3/tests/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-01 19:33:07.000000 openplugincore-0.3.3/tests/test_basicTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-07-01 19:33:07.000000 openplugincore-0.3.3/tests/test_e2e.py
```

### Comparing `openplugincore-0.3.2/openplugincore/openplugincore.py` & `openplugincore-0.3.3/openplugincore/openplugincore.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,211 +1,211 @@
-import json
-import requests
-from typing import Any, List, Dict, Union, Tuple, Callable
-import os
-from .types import ChatgptAssistantMessage, ChatgptFunctionMessage, PluginConfigs
-from langchain.chains.openai_functions.openapi import openapi_spec_to_openai_fn
-from langchain.utilities.openapi import OpenAPISpec
-from langchain.output_parsers.openai_functions import JsonOutputFunctionsParser
-from langchain.prompts import ChatPromptTemplate
-from langchain.chat_models import ChatOpenAI
-from langchain.schema import HumanMessage, AIMessage, SystemMessage, FunctionMessage
-from langchain import LLMChain
-import openai
-from dotenv import load_dotenv
-load_dotenv()
-
-OPENAI_API_KEY = os.getenv('OPENAI_API_KEY')
-
-plugin_configs: Dict[str, PluginConfigs] = {}
-
-def openplugin_completion(openai_api_key: str, plugin_name: str, prompt: str, **chatgpt_args):
-    # set environment variable to OPENAI_API_KEY
-    os.environ["OPENAI_API_KEY"] = openai_api_key
-    openai.api_key = openai_api_key
-    if not plugin_name:
-        return openai.ChatCompletion.create(
-            **chatgpt_args,
-            messages=[
-                {"role": "user", "content": prompt}
-            ]
-        )
-    plugin = OpenPlugin(plugin_name)
-    try:
-        function_response = plugin.fetch_plugin(
-            prompt=prompt,
-            **chatgpt_args
-        )
-    except ValueError as e:
-        if "Not a plugin function" in str(e):
-            return openai.ChatCompletion.create(
-                **chatgpt_args,
-                messages=[
-                    {"role": "user", "content": prompt}
-                ]
-            )
-        else:
-            raise e
-    all_chatgpt_args = {
-        **chatgpt_args,
-        "messages": [
-            {"role": "user", "content": prompt},
-            function_response
-        ]
-    }
-    summarize = openai.ChatCompletion.create(**all_chatgpt_args)
-    return summarize
-
-class OpenPlugin:
-    def __init__(self, plugin_name: str, openai_api_key: str = None, root_url: str = None, verbose: bool = False):
-        self.name: str = plugin_name
-        self.root_url: str = root_url
-        self.description: str = None
-        self.manifest: Any = None
-        self.functions: List[Dict[str, Any]] = None
-        self.call_api_fn: Callable = None
-        self.verbose: bool = verbose
-
-        if openai_api_key is None:
-            openai_api_key = os.getenv('OPENAI_API_KEY')
-            if openai_api_key is None:
-                raise ValueError("OPENAI_API_KEY not found. You can pass in the parameter openai_api_key. You can also set the environment variable OPENAI_API_KEY=<API-KEY>.")
-        os.environ["OPENAI_API_KEY"] = openai_api_key
-        openai.api_key = openai_api_key
-        self.init(plugin_name)
-        self.name: str = self.manifest["name_for_model"]
-        self.description: str = self.manifest["description_for_model"]
-
-    def init(self, plugin_name: str) -> None:
-        base_dir = os.path.dirname(os.path.realpath(__file__))
-        plugins_file_path = os.path.join(base_dir, "plugins.json")
-        with open(plugins_file_path) as f:
-            plugins = json.load(f)
-        # if self.root_url has a value
-        if self.root_url is None:
-            try:
-                self.root_url = plugins[plugin_name]
-            except KeyError:
-                # throw error
-                raise KeyError("Plugin not found")
-        self.manifest = self.fetch_manifest(self.root_url)
-        self.functions, self.call_api_fn = self.openapi_to_functions_and_call_api_fn(self.manifest)
-
-    def fetch_manifest(self, root_url: str) -> Any:
-        if plugin_configs.get(self.name, {}).get("manifest", None) is not None:
-            return plugin_configs[self.name]["manifest"]
-        
-        response = requests.get(root_url + "/.well-known/ai-plugin.json")
-        response.raise_for_status()  # Raise exception if the request failed
-        manifest = response.json()
-        if self.verbose:
-            print(f"\"{self.name}\" manifest: ", json.dumps(manifest, indent=2))
-
-        # add manifest to plugin_configs
-        plugin_configs[self.name] = {
-            **plugin_configs.get(self.name, {}),
-            "manifest": manifest
-        }
-        return manifest
-    
-    def openapi_to_functions_and_call_api_fn(self, manifest: Any) -> Tuple[List[Dict[str, Any]], Callable]:
-        openapi_url = manifest.get("api", {}).get("url")
-        if self.verbose:
-            print(f"\"{self.name}\" openapi_url: ", openapi_url)
-        if openapi_url == None:
-            raise ValueError("OpenAPI URL not found in manifest")
-        if isinstance(openapi_url, Union[OpenAPISpec, str]):
-            for conversion in (
-                OpenAPISpec.from_url,
-                OpenAPISpec.from_file,
-                OpenAPISpec.from_text,
-            ):
-                try:
-                    openapi_url = conversion(openapi_url)  # type: ignore[arg-type]
-                    break
-                except Exception:  # noqa: E722
-                    pass
-            if isinstance(openapi_url, str):
-                raise ValueError(f"Unable to parse spec from source {openapi_url}")
-        openai_fns, call_api_fn = openapi_spec_to_openai_fn(openapi_url)
-        if self.verbose:
-            print(f"\"{self.name}\" functions: ", json.dumps(openai_fns, indent=2))
-        return openai_fns, call_api_fn
-
-    def _convert_openai_messages_to_langchain_messages(self, openai_messages: List[Any]) -> List[ChatgptAssistantMessage]:
-        langchain_messages = []
-
-        for openai_message in openai_messages:
-            if openai_message["role"] == "system":
-                langchain_messages.append(SystemMessage(content=openai_message["content"]))
-            elif openai_message["role"] == "user":
-                langchain_messages.append(HumanMessage(content=openai_message["content"]))
-            elif openai_message["role"] == "function":
-                langchain_messages.append(FunctionMessage(name=openai_message["name"], content=openai_message["content"]))
-            elif openai_message["role"] == "assistant":
-                # set veriable content to "" if it is None
-                content = openai_message["content"] if openai_message["content"] is not None else ""
-                langchain_messages.append(AIMessage(content=content, additional_kwargs={"function_call": openai_message["function_call"]}))
-        
-        return langchain_messages
-
-    def fetch_plugin(self, prompt: str, **chatgpt_args) -> ChatgptFunctionMessage:
-        if chatgpt_args.get("model", None) not in ["gpt-3.5-turbo-0613", "gpt-4-0613"]:
-            raise ValueError("Model must be either gpt-3.5-turbo-0613 or gpt-4-0613")
-        
-        llm =  ChatOpenAI(
-            **chatgpt_args,
-        )
-        llm_chain = LLMChain(
-            llm=llm,
-            prompt=ChatPromptTemplate.from_template("{query}"),
-            llm_kwargs={"functions": self.functions},
-            output_parser=JsonOutputFunctionsParser(args_only=False),
-            output_key="function",
-            verbose=self.verbose,
-            # **(llm_kwargs or {}),
-        )
-        # if it is plugin function response
-        try:
-            llm_chain_out = llm_chain.run(prompt)
-            if self.verbose:
-                print("Using plugin: " + self.name)
-        except KeyError as e:
-            # if error includes "function_call" then it is not a plugin function
-            if "function_call" in str(e):
-                raise ValueError("Not a plugin function")
-            else:
-                raise e
-        if llm_chain_out["name"] not in [function["name"] for function in self.functions]:
-            raise ValueError("Not a plugin function")
-
-        # EDGE CASE
-        def remove_empty_from_dict(input_dict):
-            cleaned_dict = {}
-            for k, v in input_dict.items():
-                if isinstance(v, dict):
-                    v = remove_empty_from_dict(v)
-                if v and v != "none":  # only add to cleaned_dict if v is not empty
-                    cleaned_dict[k] = v
-            return cleaned_dict
-        llm_chain_out["arguments"] = remove_empty_from_dict(llm_chain_out["arguments"])
-        if self.verbose:
-            print(f"\"{self.name}\" llm_chain_out: ", json.dumps(llm_chain_out, indent=2))
-
-        # make the api call
-        def request_chain(name,arguments):
-            res = self.call_api_fn(
-                name, arguments, headers=None, params=None
-            )
-            return res
-        request_out = request_chain(**llm_chain_out)
-        json_response = request_out.json()
-        if self.verbose:
-            print(f"\"{self.name}\" json_response: ", json.dumps(json_response, indent=2))
-        try:
-            return ChatgptFunctionMessage(
-                role="function",
-                name=llm_chain_out["name"],
-                content=json.dumps(json_response)
-            )
-        except json.decoder.JSONDecodeError:
-            raise json.decoder.JSONDecodeError(f"API call failed, API returned the following non-JSON response:\n{response.content}")
+import json
+import requests
+from typing import Any, List, Dict, Union, Tuple, Callable
+import os
+from .types import ChatgptAssistantMessage, ChatgptFunctionMessage, PluginConfigs
+from langchain.chains.openai_functions.openapi import openapi_spec_to_openai_fn
+from langchain.utilities.openapi import OpenAPISpec
+from langchain.output_parsers.openai_functions import JsonOutputFunctionsParser
+from langchain.prompts import ChatPromptTemplate
+from langchain.chat_models import ChatOpenAI
+from langchain.schema import HumanMessage, AIMessage, SystemMessage, FunctionMessage
+from langchain import LLMChain
+import openai
+from dotenv import load_dotenv
+load_dotenv()
+
+OPENAI_API_KEY = os.getenv('OPENAI_API_KEY')
+
+plugin_configs: Dict[str, PluginConfigs] = {}
+
+def openplugin_completion(openai_api_key: str, plugin_name: str, prompt: str, **chatgpt_args):
+    # set environment variable to OPENAI_API_KEY
+    os.environ["OPENAI_API_KEY"] = openai_api_key
+    openai.api_key = openai_api_key
+    if not plugin_name:
+        return openai.ChatCompletion.create(
+            **chatgpt_args,
+            messages=[
+                {"role": "user", "content": prompt}
+            ]
+        )
+    plugin = OpenPlugin(plugin_name)
+    try:
+        function_response = plugin.fetch_plugin(
+            prompt=prompt,
+            **chatgpt_args
+        )
+    except ValueError as e:
+        if "Not a plugin function" in str(e):
+            return openai.ChatCompletion.create(
+                **chatgpt_args,
+                messages=[
+                    {"role": "user", "content": prompt}
+                ]
+            )
+        else:
+            raise e
+    all_chatgpt_args = {
+        **chatgpt_args,
+        "messages": [
+            {"role": "user", "content": prompt},
+            function_response
+        ]
+    }
+    summarize = openai.ChatCompletion.create(**all_chatgpt_args)
+    return summarize
+
+class OpenPlugin:
+    def __init__(self, plugin_name: str, openai_api_key: str = None, root_url: str = None, verbose: bool = False):
+        self.name: str = plugin_name
+        self.root_url: str = root_url
+        self.description: str = None
+        self.manifest: Any = None
+        self.functions: List[Dict[str, Any]] = None
+        self.call_api_fn: Callable = None
+        self.verbose: bool = verbose
+
+        if openai_api_key is None:
+            openai_api_key = os.getenv('OPENAI_API_KEY')
+            if openai_api_key is None:
+                raise ValueError("OPENAI_API_KEY not found. You can pass in the parameter openai_api_key. You can also set the environment variable OPENAI_API_KEY=<API-KEY>.")
+        os.environ["OPENAI_API_KEY"] = openai_api_key
+        openai.api_key = openai_api_key
+        self.init(plugin_name)
+        self.name: str = self.manifest["name_for_model"]
+        self.description: str = self.manifest["description_for_model"]
+
+    def init(self, plugin_name: str) -> None:
+        base_dir = os.path.dirname(os.path.realpath(__file__))
+        plugins_file_path = os.path.join(base_dir, "plugins.json")
+        with open(plugins_file_path) as f:
+            plugins = json.load(f)
+        # if self.root_url has a value
+        if self.root_url is None:
+            try:
+                self.root_url = plugins[plugin_name]
+            except KeyError:
+                # throw error
+                raise KeyError("Plugin not found")
+        self.manifest = self.fetch_manifest(self.root_url)
+        self.functions, self.call_api_fn = self.openapi_to_functions_and_call_api_fn(self.manifest)
+
+    def fetch_manifest(self, root_url: str) -> Any:
+        if plugin_configs.get(self.name, {}).get("manifest", None) is not None:
+            return plugin_configs[self.name]["manifest"]
+        
+        response = requests.get(root_url + "/.well-known/ai-plugin.json")
+        response.raise_for_status()  # Raise exception if the request failed
+        manifest = response.json()
+        if self.verbose:
+            print(f"\"{self.name}\" manifest: ", json.dumps(manifest, indent=2))
+
+        # add manifest to plugin_configs
+        plugin_configs[self.name] = {
+            **plugin_configs.get(self.name, {}),
+            "manifest": manifest
+        }
+        return manifest
+    
+    def openapi_to_functions_and_call_api_fn(self, manifest: Any) -> Tuple[List[Dict[str, Any]], Callable]:
+        openapi_url = manifest.get("api", {}).get("url")
+        if self.verbose:
+            print(f"\"{self.name}\" openapi_url: ", openapi_url)
+        if openapi_url == None:
+            raise ValueError("OpenAPI URL not found in manifest")
+        if isinstance(openapi_url, Union[OpenAPISpec, str]):
+            for conversion in (
+                OpenAPISpec.from_url,
+                OpenAPISpec.from_file,
+                OpenAPISpec.from_text,
+            ):
+                try:
+                    openapi_url = conversion(openapi_url)  # type: ignore[arg-type]
+                    break
+                except Exception:  # noqa: E722
+                    pass
+            if isinstance(openapi_url, str):
+                raise ValueError(f"Unable to parse spec from source {openapi_url}")
+        openai_fns, call_api_fn = openapi_spec_to_openai_fn(openapi_url)
+        if self.verbose:
+            print(f"\"{self.name}\" functions: ", json.dumps(openai_fns, indent=2))
+        return openai_fns, call_api_fn
+
+    def _convert_openai_messages_to_langchain_messages(self, openai_messages: List[Any]) -> List[ChatgptAssistantMessage]:
+        langchain_messages = []
+
+        for openai_message in openai_messages:
+            if openai_message["role"] == "system":
+                langchain_messages.append(SystemMessage(content=openai_message["content"]))
+            elif openai_message["role"] == "user":
+                langchain_messages.append(HumanMessage(content=openai_message["content"]))
+            elif openai_message["role"] == "function":
+                langchain_messages.append(FunctionMessage(name=openai_message["name"], content=openai_message["content"]))
+            elif openai_message["role"] == "assistant":
+                # set veriable content to "" if it is None
+                content = openai_message["content"] if openai_message["content"] is not None else ""
+                langchain_messages.append(AIMessage(content=content, additional_kwargs={"function_call": openai_message["function_call"]}))
+        
+        return langchain_messages
+
+    def fetch_plugin(self, prompt: str, **chatgpt_args) -> ChatgptFunctionMessage:
+        if chatgpt_args.get("model", None) not in ["gpt-3.5-turbo-0613", "gpt-4-0613"]:
+            raise ValueError("Model must be either gpt-3.5-turbo-0613 or gpt-4-0613")
+        
+        llm =  ChatOpenAI(
+            **chatgpt_args,
+        )
+        llm_chain = LLMChain(
+            llm=llm,
+            prompt=ChatPromptTemplate.from_template("{query}"),
+            llm_kwargs={"functions": self.functions},
+            output_parser=JsonOutputFunctionsParser(args_only=False),
+            output_key="function",
+            verbose=self.verbose,
+            # **(llm_kwargs or {}),
+        )
+        # if it is plugin function response
+        try:
+            llm_chain_out = llm_chain.run(prompt)
+            if self.verbose:
+                print("Using plugin: " + self.name)
+        except KeyError as e:
+            # if error includes "function_call" then it is not a plugin function
+            if "function_call" in str(e):
+                raise ValueError("Not a plugin function")
+            else:
+                raise e
+        if llm_chain_out["name"] not in [function["name"] for function in self.functions]:
+            raise ValueError("Not a plugin function")
+
+        # EDGE CASE
+        def remove_empty_from_dict(input_dict):
+            cleaned_dict = {}
+            for k, v in input_dict.items():
+                if isinstance(v, dict):
+                    v = remove_empty_from_dict(v)
+                if v and v != "none":  # only add to cleaned_dict if v is not empty
+                    cleaned_dict[k] = v
+            return cleaned_dict
+        llm_chain_out["arguments"] = remove_empty_from_dict(llm_chain_out["arguments"])
+        if self.verbose:
+            print(f"\"{self.name}\" llm_chain_out: ", json.dumps(llm_chain_out, indent=2))
+
+        # make the api call
+        def request_chain(name,arguments):
+            res = self.call_api_fn(
+                name, arguments, headers=None, params=None
+            )
+            return res
+        request_out = request_chain(**llm_chain_out)
+        json_response = request_out.json()
+        if self.verbose:
+            print(f"\"{self.name}\" json_response: ", json.dumps(json_response, indent=2))
+        try:
+            return ChatgptFunctionMessage(
+                role="function",
+                name=llm_chain_out["name"],
+                content=json.dumps(json_response)
+            )
+        except json.decoder.JSONDecodeError:
+            raise json.decoder.JSONDecodeError(f"API call failed, API returned the following non-JSON response:\n{json_response.content}")
```

### Comparing `openplugincore-0.3.2/openplugincore/plugins.json` & `openplugincore-0.3.3/openplugincore/plugins.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9209770114942529%*

 * *Differences: {"'currencyconverter'": "'https://currency-conversion--nerrosa.repl.co'",*

 * * "'mbti'": "'https://mbti.bowang17.repl.co'",*

 * * "'medecinedata'": "'https://pubmed-explorer.narhasweet.repl.co'",*

 * * "'paperchat'": "'https://paperchat.fwdoperators.com'",*

 * * 'delete': "['ABCmouse', 'ArtCollection', 'AskMarcie', 'Avalara', 'BOXIL_SaaS', 'Bohita', "*

 * *           "'Broadway', 'BubbleGoods', 'ChatWithBible', 'ChatWithQuran', 'CheckTheChain', "*

 * *           "'Checkers', 'CloudDiagramGen', 'Company_Transcripts', "*

 * *           "'Crea […]*

```diff
@@ -1,56 +1,36 @@
 {
-    "ABCmouse": "https://ai.abcmouse.com",
     "AMAZON_product_desc_generator": "https://turboooo.com",
     "Agones": "https://agones.gr",
     "Ai_PDF": "https://plugin-3c56b9d4c8a6465998395f28b6a445b2-jexkai4vea-uc.a.run.app",
     "Algorithma": "https://algorithma.ruvnet.repl.co",
     "ApexMap": "https://apex-map-plugin-d1u8.vercel.app",
     "AppyPieAIAppBuilder": "https://appypie.com",
-    "ArtCollection": "https://artcollection--chao-gu-ge-lei.repl.co",
     "AskCars": "https://askcars.ai",
-    "AskMarcie": "https://askmarcie-backend.herokuapp.com",
     "AskTheCode": "https://askthecode.dsomok.online",
     "Austrian_Bank_Rates": "https://banken-vergleich.net",
-    "Avalara": "https://plugins.midgard.avalara.io",
-    "BOXIL_SaaS": "https://boxil.jp",
     "Bardeen": "https://bardeen.ai",
-    "Bohita": "https://gptshop.bohita.com",
-    "Broadway": "https://www.broadway.com",
-    "BubbleGoods": "https://chatgpt.bubblegoods.com",
     "ByByAI": "https://byby.ai",
     "C3_Glide": "https://c3glide-d9g5.boldstratus.com",
     "CTCP": "https://ctcp.japaneast.cloudapp.azure.com",
-    "ChatWithBible": "https://bible.religions.chat",
-    "ChatWithQuran": "https://quran.religions.chat",
-    "CheckTheChain": "https://www.nani.ooo",
-    "Checkers": "https://0a8e9b8e7f0912323de2d3653f1ea597.preview.pluginlab.ai",
-    "CloudDiagramGen": "https://ei6xvhnd3r.eu-west-1.awsapprunner.com",
-    "Company_Transcripts": "https://transcripts.koyfin.com",
     "Coupert": "https://www.coupert.com",
     "CranePumpsManuals": "https://cpsconnect.cranepumps.com",
-    "Creaticode_Extension_of_MIT_Scratch": "https://openai.creaticode.com",
     "CreatuityStores": "https://chatgpt.wild.creatuity.net",
     "CreditYelp": "https://credityelp.com",
     "CribbageScorer": "https://cribbage.azurewebsites.net",
-    "CryptoPrices": "https://data-api.cryptocompare.com",
-    "DAIZY": "https://plugin.daizy.com",
-    "Diagrams": "https://diagrams.herokuapp.com",
     "Dr_Thoths_Tarot": "https://dr-thoth-tarot.herokuapp.com",
     "DreamInterpreter": "https://dreamplugin.bgnetmobile.com",
     "DuoduoEnglish": "https://n4nbxo32xi.execute-api.ap-northeast-1.amazonaws.com",
     "EasyProductSearch": "https://easy-search.techno-gauss.com",
     "Etihad_Airline": "https://gpt-etihad.botim.me",
     "Ferryhopper": "https://openai.ferryhopper.com",
     "Figlet": "https://figletgptplugin.wisemonkey.repl.co",
-    "FreshTech": "https://6yq93jqsc3.execute-api.us-west-1.amazonaws.com",
     "GameSight": "https://openai.tapapis.com",
     "Gate2AI": "https://gate2ai.com",
     "GifApi": "https://chat-plugin-giphy.efficiency.tools",
-    "Glowing": "https://stage.glowing.ai",
     "Google_Ads_Shopping_Microsoft_Ads_pay_per_click": "https://www.storeya.com",
     "Horoscopes_by_Inner_Self": "https://innerself.ai",
     "ImageSearch": "https://imgser.aigenprompt.com",
     "IndoorPlants": "https://kirill.customgpt.ai",
     "Instacart": "https://instacart.com",
     "IsotonixProducts": "https://www.isotonix.com",
     "JetBookClick": "https://jetbook.click",
@@ -97,15 +77,14 @@
     "Roshi": "https://www.roshi-server.com",
     "SHOPCOMProducts": "https://shop.com",
     "ScholarlyInsight": "https://scholarlyinsight--chao-gu-ge-lei.repl.co",
     "ShopMate": "https://shopmate-o5kx.onrender.com",
     "ShoppingTools": "https://shoppingtools.biz",
     "SignalPlus": "https://chatgptpi.signalplus.com",
     "Singapore_Places_Of_Interest": "https://sg-places.herokuapp.com",
-    "Smart_Price_Finder": "https://api.spendless.ai",
     "Spirify_model_qrcode": "https://spirifyqrcode.azurewebsites.net",
     "StockData": "https://portfoliometa.com",
     "Sudoku": "https://chat-sudoku-api.bricks.cool",
     "SuperchargeMyEV": "https://plugin.charge-my-ev.guide",
     "Supercharger": "https://supercharger-958358-jexkai4vea-uc.a.run.app",
     "Surveillance_API": "https://surveillance-api.synology.com",
     "Tabor": "https://plugin.tabor.ai",
@@ -160,15 +139,14 @@
     "champdex": "https://champdex.com",
     "charity": "https://charitysense.com",
     "chat_with_gsheet": "https://chatgsheet.com",
     "chatspot": "https://chatspot.ai",
     "chattoolfinder": "https://plugin.pluginfinder.gimmee.info",
     "chatwithpdf": "https://chatwithpdf.sdan.io",
     "chatwithvideo": "https://chatwithvideo.sdan.io",
-    "chatwithwebsite": "https://chatwithwebsite.sdan.io",
     "chicago_data_portal": "https://chatgpt.deepdigits.pizza",
     "clinical_trial_radar": "https://trialradar2.marketflare.repl.co",
     "coincap": "https://coincap.gptplug.chat",
     "companieshouse": "https://companieshouse.tradexy.repl.co",
     "competitorppcads": "https://ppc-optimizer.gcs.ai",
     "converter_app": "https://converter-app-chat-gpt-plugin.vercel.app",
     "copilot": "https://gpt.copilotsearch.com",
@@ -177,15 +155,15 @@
     "create_qr_code": "https://create-qr-code.modelxy.com",
     "creativemind": "https://gpt-4dall-e.pranavbhatt402.repl.co",
     "cryptoPriceAndNews": "https://crypto-news.replit.app",
     "crypto_price_checker": "https://cryptoprices.smoothplugins.com",
     "cryptomation": "https://chat.cryptomation.com",
     "cryptopulse": "https://crypto-pulse-top.vercel.app",
     "currency_today": "https://today-currency-converter.oiconma.repl.co",
-    "currencyconverter": "https://currency-convert-chatgpt-plugin.vercel.app",
+    "currencyconverter": "https://currency-conversion--nerrosa.repl.co",
     "customplugin": "https://customplugin.customplugin.ai",
     "daigram": "https://daigr.am",
     "deepmemory": "https://apiv2.deepmemory.io",
     "defillama": "https://llamawrapper-prod.onrender.com",
     "dev": "https://dev.to",
     "dfa": "https://domainfinderai.com",
     "diceroller": "https://dmtoolkit.magejosh.repl.co",
@@ -247,14 +225,16 @@
     "litmaps": "https://api.litmaps.com",
     "local": "https://local.goodcall.ai",
     "locate_inventory_for_electronic_components": "https://api.getamplio.com",
     "lsongai": "https://lsong.org",
     "magi_codex": "https://mtg-rules-chatgpt-plugin.fly.dev",
     "magic_conch": "https://magic-conch.onrender.com",
     "maps": "https://maps.smoothplugins.com",
+    "mbti": "https://mbti.bowang17.repl.co",
+    "medecinedata": "https://pubmed-explorer.narhasweet.repl.co",
     "mediaready": "https://chatgpt.mediareadyai.com",
     "message_in_a_bottle": "https://messagesinbottles.space",
     "metar": "https://metar.pluginai.ai",
     "mintbasesearch": "https://search-ai.mintbase.xyz",
     "mobula": "https://api.app-mobula.com",
     "modeal_api": "https://api.modeal.net",
     "momentxguidex": "https://departmentstoreguide-plugin.momentxwill.repl.co",
@@ -263,16 +243,16 @@
     "ndricks_sports_api": "https://api.ndricks.com",
     "news": "https://simbiss.net",
     "nextpaper": "https://nextpaperplugin--mengzhao1.repl.co",
     "nonprofits": "https://api.getchange.io",
     "openarch": "https://www.openarch.nl",
     "opentools": "https://gptplugin.opentools.ai",
     "owd": "https://oneword.domains",
+    "paperchat": "https://paperchat.fwdoperators.com",
     "paxiai": "https://paxi.ai",
-    "ph_ai_news_query": "https://ph-api-prototype.azurewebsites.net",
     "photorealistic": "https://midjourney-ruddy.vercel.app",
     "plug_finder": "https://plugin.lyrai.app",
     "podcastSearch": "https://esne.ai",
     "polarr": "https://polarr.co",
     "pollthepeople": "https://pollthepeople.customplugin.ai",
     "portfoliopilot": "https://portfoliopilot.com",
     "product_recommendation": "https://lexi-shopping-assistant-chatgpt-plugin.iamnazzty.repl.co",
@@ -333,15 +313,14 @@
     "wahi": "https://wahi.com",
     "wanted_job_search": "https://assistant.wanted.co.kr",
     "web5": "https://chatgpt.tbddev.org",
     "web_pilot": "https://webreader.webpilotai.com",
     "web_requests": "https://plugin.wegpt.ai",
     "web_scraper": "https://scraper.gafo.tech",
     "what_to_watch": "https://gpt-show-search.fly.dev",
-    "whimsical": "https://whimsical.com",
     "whois_domain_checker": "https://whois.smoothplugins.com",
     "wishbucket": "https://www.phloxcorp.io",
     "word_and_character_count": "https://text-count.modelxy.com",
     "word_sneak": "https://word-sneak.jeevnayak.repl.co",
     "wordly_guess_the_word_game": "https://chat-wordle-ai-7vdz5.ondigitalocean.app",
     "yt_caption_retriever": "https://youtube-caption-retriever.world-designer.repl.co"
 }
```

### Comparing `openplugincore-0.3.2/setup.py` & `openplugincore-0.3.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-from setuptools import setup, find_packages
-
-# Setting up
-setup(
-       # the name must match the folder name 'verysimplemodule'
-        name='openplugincore', 
-        version="0.3.2",
-        author="Sebastian Sosa",
-        author_email="1sebastian1sosa1@gmail.com",
-        description='Seamlessly integrate with OpenAI ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!',
-        long_description='Seamlessly integrate with OpenAIs ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!',
-        packages=find_packages(),
-        package_data={
-            "openplugincore": ["*.json"],  # include all .json files in the openplugin package
-        },
-        exclude=['tests'],
-        install_requires=[
-            'pyyaml',
-            'requests',
-            'openai',
-            'langchain',
-            'python-dotenv',
-        ], # add any additional packages
-        
-        keywords=[
-            'python',
-            'openai',
-            'chatgpt',
-            'chat',
-            'plugin'
-        ],
-        classifiers= [
-            "Development Status :: 2 - Pre-Alpha",
-            "Intended Audience :: Developers",
-            "Programming Language :: Python :: 3.10",
-            "Programming Language :: Python :: 3",
-            "Operating System :: MacOS :: MacOS X",
-            "Operating System :: Microsoft :: Windows",
-        ]
+from setuptools import setup, find_packages
+
+# Setting up
+setup(
+       # the name must match the folder name 'verysimplemodule'
+        name='openplugincore', 
+        version="0.3.3",
+        author="Sebastian Sosa",
+        author_email="1sebastian1sosa1@gmail.com",
+        description='Seamlessly integrate with OpenAI ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!',
+        long_description='Seamlessly integrate with OpenAIs ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!',
+        packages=find_packages(),
+        package_data={
+            "openplugincore": ["*.json"],  # include all .json files in the openplugin package
+        },
+        exclude=['tests'],
+        install_requires=[
+            'requests',
+            'openai',
+            'langchain',
+            'python-dotenv',
+        ], # add any additional packages
+        
+        keywords=[
+            'python',
+            'openai',
+            'chatgpt',
+            'chat',
+            'plugin'
+        ],
+        classifiers= [
+            "Development Status :: 2 - Pre-Alpha",
+            "Intended Audience :: Developers",
+            "Programming Language :: Python :: 3.10",
+            "Programming Language :: Python :: 3",
+            "Operating System :: MacOS :: MacOS X",
+            "Operating System :: Microsoft :: Windows",
+        ]
 )
```

### Comparing `openplugincore-0.3.2/tests/test_basicTest.py` & `openplugincore-0.3.3/tests/test_basicTest.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-import json
-import pytest
-from .mock_data import todo_plugin
-import os
-from openplugincore import OpenPlugin, openplugin_completion
-import random
-import requests
-from dotenv import load_dotenv
-load_dotenv()
-
-OPENAI_API_KEY = os.getenv('OPENAI_API_KEY')
-
-def test_initiate_todo_with_url():
-    plugin = OpenPlugin("NA", root_url="http://localhost:3333")
-    assert plugin.manifest is not None
-    assert plugin.manifest.get("name_for_model") == "todo"
-
-@pytest.fixture
-def todo_openplugin():
-    plugin = OpenPlugin("__testing__")
-    return plugin 
-
-def test_initiate_todo(todo_openplugin):
-    assert todo_openplugin.manifest is not None
-    assert todo_openplugin.manifest.get("name_for_model") == "todo"
-
-def test_openapi_to_functions_and_call_api_fn(todo_openplugin):
-    # test functions
-    assert len(todo_openplugin.functions) == 2
-    addTodo = None
-    getTodos = None
-    for function in todo_openplugin.functions:
-        if function["name"] == "addTodo":
-            addTodo = function
-        if function["name"] == "getTodos":
-            getTodos = function
-    
-    assert addTodo is not None
-    assert addTodo == todo_plugin["functions"][0]
-
-    assert getTodos is not None
-    assert getTodos == todo_plugin["functions"][1]
-
-    # test call_api_fn
-    request_out = todo_openplugin.call_api_fn(
-        todo_plugin["llm_chain_out"]["name"],
-        todo_plugin["llm_chain_out"]["arguments"]
-    )
-    assert request_out.json() == todo_plugin["request_out.json()"]
-
-
-def test_fetch_plugin(todo_openplugin):
-    response = todo_openplugin.fetch_plugin(
-        prompt=todo_plugin["prompt"],
-        model="gpt-3.5-turbo-0613"
-    )
-    assert response is not None
-    assert response["role"] == "function"
-    assert response["name"] == "addTodo"
-    json_content = json.loads(response["content"])
-    assert json_content["todo"] == "buy milk"
-
-def test_openplugin_completion():
-    todo = f'test_chat_completion_{random.randint(0, 100000)}'
-
-    completion = openplugin_completion(
-        openai_api_key = OPENAI_API_KEY,
-        plugin_name = "__testing__",
-        prompt = f"add '{todo}' to my todo list",
-        model = "gpt-3.5-turbo-0613",
-        temperature = 0,
-    )
-
-    todos_request = requests.get("http://localhost:3333/todos")
-    todos_body = todos_request.json()
-    
-    assert todo in completion["choices"][0]["message"]["content"]
-    assert todo in todos_body["todos"]
-
+import json
+import pytest
+from .mock_data import todo_plugin
+import os
+from openplugincore import OpenPlugin, openplugin_completion
+import random
+import requests
+from dotenv import load_dotenv
+load_dotenv()
+
+OPENAI_API_KEY = os.getenv('OPENAI_API_KEY')
+
+def test_initiate_todo_with_url():
+    plugin = OpenPlugin("NA", root_url="http://localhost:3333")
+    assert plugin.manifest is not None
+    assert plugin.manifest.get("name_for_model") == "todo"
+
+@pytest.fixture
+def todo_openplugin():
+    plugin = OpenPlugin("__testing__")
+    return plugin 
+
+def test_initiate_todo(todo_openplugin):
+    assert todo_openplugin.manifest is not None
+    assert todo_openplugin.manifest.get("name_for_model") == "todo"
+
+def test_openapi_to_functions_and_call_api_fn(todo_openplugin):
+    # test functions
+    assert len(todo_openplugin.functions) == 2
+    addTodo = None
+    getTodos = None
+    for function in todo_openplugin.functions:
+        if function["name"] == "addTodo":
+            addTodo = function
+        if function["name"] == "getTodos":
+            getTodos = function
+    
+    assert addTodo is not None
+    assert addTodo == todo_plugin["functions"][0]
+
+    assert getTodos is not None
+    assert getTodos == todo_plugin["functions"][1]
+
+    # test call_api_fn
+    request_out = todo_openplugin.call_api_fn(
+        todo_plugin["llm_chain_out"]["name"],
+        todo_plugin["llm_chain_out"]["arguments"]
+    )
+    assert request_out.json() == todo_plugin["request_out.json()"]
+
+
+def test_fetch_plugin(todo_openplugin):
+    response = todo_openplugin.fetch_plugin(
+        prompt=todo_plugin["prompt"],
+        model="gpt-3.5-turbo-0613"
+    )
+    assert response is not None
+    assert response["role"] == "function"
+    assert response["name"] == "addTodo"
+    json_content = json.loads(response["content"])
+    assert json_content["todo"] == "buy milk"
+
+def test_openplugin_completion():
+    todo = f'test_chat_completion_{random.randint(0, 100000)}'
+
+    completion = openplugin_completion(
+        openai_api_key = OPENAI_API_KEY,
+        plugin_name = "__testing__",
+        prompt = f"add '{todo}' to my todo list",
+        model = "gpt-3.5-turbo-0613",
+        temperature = 0,
+    )
+
+    todos_request = requests.get("http://localhost:3333/todos")
+    todos_body = todos_request.json()
+    
+    assert todo in completion["choices"][0]["message"]["content"]
+    assert todo in todos_body["todos"]
+
```

### Comparing `openplugincore-0.3.2/tests/test_e2e.py` & `openplugincore-0.3.3/tests/test_e2e.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,366 +1,366 @@
-import json
-import pytest
-import os
-import openai
-from .mock_data import todo_plugin
-from openplugincore import OpenPlugin
-
-OPENAI_API_KEY = os.getenv('OPENAI_API_KEY')
-
-def test_initiate_and_fetch_todo():
-    plugin = OpenPlugin("__testing__")
-    assert plugin.manifest is not None
-    assert plugin.manifest.get("name_for_model") == "todo"
-
-    for function in plugin.functions:
-        if function["name"] == "addTodo":
-            addTodo = function
-        if function["name"] == "getTodos":
-            getTodos = function
-    
-    assert addTodo is not None
-    assert addTodo == todo_plugin["functions"][0]
-
-    assert getTodos is not None
-    assert getTodos == todo_plugin["functions"][1]
-
-    # fetch after chatgpt response
-    response = plugin.fetch_plugin(
-        prompt=todo_plugin["prompt"],
-        model="gpt-3.5-turbo-0613",
-        temperature=0,
-    )
-    assert response is not None
-    assert response["role"] == "function"
-    assert response["name"] == "addTodo"
-    json_content = json.loads(response["content"])
-    assert json_content["todo"] == "buy milk"
-
-def test_initiate_and_fetch_LGTM():
-    plugin = OpenPlugin("LGTM")
-    assert plugin.manifest is not None
-
-    # # create chatgpt request that will call the addTodo function
-    chatgpt_prompt = 'Show me markdown for a 2 by 2 table with LGTM'
-    response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
-        model="gpt-3.5-turbo-0613",
-        temperature=0,
-    )
-
-    assert response is not None
-    assert response["role"] == "function"
-    json_content = json.loads(response["content"])
-    # # ensure that the json_content has a key of image_url and that is starts with https://lgtm.lol
-    assert "image_url" in json_content
-    assert json_content["image_url"].startswith("https://lgtm.lol")
-
-if False: # server too inconsistent
-    def test_initiate_and_fetch_Figlet():
-        plugin = OpenPlugin("Figlet")
-        assert plugin.manifest is not None
-
-        # create chatgpt request that will call the addTodo function
-        chatgpt_prompt = 'Convert "Testing" to the Doom ASCII font.'
-        response = plugin.fetch_plugin(
-            prompt=chatgpt_prompt,
-            model="gpt-3.5-turbo-0613",
-            temperature=0,
-        )
-
-        assert response is not None
-        assert response["role"] == "function"
-
-        json_content = json.loads(response["content"])
-        assert json_content["font"] == "doom"
-
-def test_initiate_and_fetch_yt_caption_retriever():
-    plugin = OpenPlugin("yt_caption_retriever")
-    assert plugin.manifest is not None
-
-    # create chatgpt request that will call the addTodo function
-    chatgpt_prompt = 'give me a 2 sentence summary of the following yt video https://www.youtube.com/watch?v=P310I19L3Ko'
-    response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
-        model="gpt-3.5-turbo-0613",
-        temperature=0,
-    )
-
-    assert response is not None
-    assert response["role"] == "function"
-    json_content = json.loads(response["content"])
-
-    # Replace the line below with a test for the final output in json_content
-    assert "en" in json_content["captions"]
-
-def test_initiate_and_fetch_twtData():
-    plugin = OpenPlugin("twtData")
-    assert plugin.manifest is not None
-
-    # create chatgpt request that will call the addTodo function
-    chatgpt_prompt = 'show me the amount of people @Sebasti54919704 is following'
-    response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
-        model="gpt-3.5-turbo-0613",
-        temperature=0,
-    )
-
-    assert response is not None
-    assert response["role"] == "function"
-    json_content = json.loads(response["content"])
-
-    # Replace the line below with a test for the final output in json_content
-    assert json_content["stats"]["account_found"] == True
-
-def test_initiate_and_fetch_tailor_erp():
-    plugin = OpenPlugin("tailor_erp")
-    assert plugin.manifest is not None
-
-    # create chatgpt request that will call the addTodo function
-    chatgpt_prompt = 'create a CRM template with ERP generator'
-    response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
-        model="gpt-3.5-turbo-0613",
-        temperature=0,
-    )
-
-    assert response is not None
-    assert response["role"] == "function"
-    json_content = json.loads(response["content"])
-
-    # assert that json_content.applyTemplate.path is not None
-    assert json_content["APP_ID"] is not None
-
-def test_initiate_and_fetch_surge_ai_trends():
-    plugin = OpenPlugin("surge_ai_trends")
-    assert plugin.manifest is not None
-
-    # create chatgpt request that will call the addTodo function
-    chatgpt_prompt = 'What are the trnding searches for "gpu" in amazon'
-    response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
-        model="gpt-3.5-turbo-0613",
-        temperature=0,
-    )
-
-    assert response is not None
-    assert response["role"] == "function"
-    json_content = json.loads(response["content"])
-
-    # assert that json_content.items is a list
-    assert isinstance(json_content["items"], list)
-
-def test_initiate_and_fetch_speedy_marketing():
-    plugin = OpenPlugin("speedy_marketing")
-    assert plugin.manifest is not None
-
-    # create chatgpt request that will call the addTodo function
-    chatgpt_prompt = 'write me an SEO blog about react for marketing'
-    response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
-        model="gpt-3.5-turbo-0613",
-        temperature=0,
-    )
-
-    assert response is not None
-    assert response["role"] == "function"
-    json_content = json.loads(response["content"])
-
-    # Replace the line below with a test for the final output in json_content
-    assert isinstance(json_content["blog"], str)
-
-def test_initiate_and_fetch_socialsearch():
-    plugin = OpenPlugin("socialsearch")
-    assert plugin.manifest is not None
-    print("plugin.manifest: ", json.dumps(plugin.manifest, indent=2))
-    # create chatgpt request that will call the addTodo function
-    chatgpt_prompt = 'show me elon musk latest tweet'
-    response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
-        verbose=True,
-        model="gpt-3.5-turbo-0613",
-        temperature=0,
-    )
-
-    assert response is not None
-    assert response["role"] == "function"
-    json_content = json.loads(response["content"])
-
-    # Replace the line below with a test for the final output in json_content
-    assert isinstance(json_content["message"], str)
-
-if False: # unable to convert url
-    def test_initiate_and_fetch_show_me_diagrams():
-        plugin = OpenPlugin("show_me_diagrams")
-        plugin.verbose = True
-        assert plugin.manifest is not None
-
-        # create chatgpt request that will call the addTodo function
-        chatgpt_prompt = 'make a diagram of one node connected to two others that will be yes or no'
-        response = plugin.fetch_plugin(
-            prompt=chatgpt_prompt,
-            model="gpt-3.5-turbo-0613",
-            temperature=0,
-        )
-
-        assert response is not None
-        assert response["role"] == "function"
-        json_content = json.loads(response["content"])
-
-        # Replace the line below with a test for the final output in json_content
-        assert isinstance(json_content["results"][0]["image"], str)
-
-def test_initiate_and_fetch_scholarai():
-    plugin = OpenPlugin("scholarai")
-    assert plugin.manifest is not None
-
-
-    # create chatgpt request that will call the addTodo function
-    chatgpt_prompt = 'What scientific research exists for semantic representation of language through brain waves. dont sort.'
-    response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
-        model="gpt-3.5-turbo-0613",
-        temperature=0,
-    )
-
-    assert response is not None
-    assert response["role"] == "function"
-    json_content = json.loads(response["content"])
-
-    # Replace the line below with a test for the final output in json_content
-    assert isinstance(json_content["total_num_results"], int)
-
-def test_initiate_and_fetch_rephrase():
-    plugin = OpenPlugin("rephrase")
-    assert plugin.manifest is not None
-
-    # create chatgpt request that will call the addTodo function
-    chatgpt_prompt = 'I want to code a react ui with hello world please rephrase that'
-    response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
-        model="gpt-3.5-turbo-0613",
-        temperature=0,
-    )
-
-    assert response is not None
-    assert response["role"] == "function"
-    json_content = json.loads(response["content"])
-
-    # Replace the line below with a test for the final output in json_content
-    assert isinstance(json_content["rephrased"]["text"], str)
-
-def test_initiate_and_fetch_DreamInterpreter():
-    plugin = OpenPlugin("DreamInterpreter", verbose=True)
-    assert plugin.manifest is not None
-    
-    # create chatgpt request that will call the addTodo function
-    chatgpt_prompt = 'I dreamt of being in a room without any windows getting smaller overtime'
-    response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
-        model="gpt-3.5-turbo-0613",
-        temperature=0,
-    )
-
-    assert response is not None
-    assert response["role"] == "function"
-    json_content = json.loads(response["content"])
-
-    # Replace the line below with a test for the final output in json_content
-    assert isinstance(json_content["dreamResult"], str)
-
-def test_initiate_and_fetch_portfoliopilot():
-    plugin = OpenPlugin("portfoliopilot", verbose=True)
-    assert plugin.manifest is not None
-    
-    # create chatgpt request that will call the addTodo function
-    chatgpt_prompt = 'What stocks should I add for my long term tech portfolio'
-    response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
-        model="gpt-3.5-turbo-0613",
-        temperature=0,
-    )
-
-    assert response is not None
-    assert response["role"] == "function"
-    json_content = json.loads(response["content"])
-
-    # Replace the line below with a test for the final output in json_content
-    assert isinstance(json_content["top_stocks"], list)
-
-def test_initiate_and_fetch_C3_Glide():
-    plugin = OpenPlugin("C3_Glide", verbose=True)
-    assert plugin.manifest is not None
-    
-    # create chatgpt request that will call the addTodo function
-    chatgpt_prompt = 'Provide me TAF for KJFK with reguards to aviation weather'
-    response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
-        model="gpt-3.5-turbo-0613",
-        temperature=0,
-    )
-
-    assert response is not None
-    assert response["role"] == "function"
-    json_content = json.loads(response["content"])
-
-    # Replace the line below with a test for the final output in json_content
-    assert isinstance(json_content["tafs"], list)
-
-def test_initiate_and_fetch_Ai_PDF():
-    plugin = OpenPlugin("Ai_PDF", verbose=True)
-    assert plugin.manifest is not None
-    
-    # create chatgpt request that will call the addTodo function
-    chatgpt_prompt = 'Can I have my data be private according to this pdf https://www.unodc.org/pdf/criminal_justice/UN_Basic_Principles_on_the_Role_of_Lawyers.pdf'
-    response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
-        model="gpt-3.5-turbo-0613",
-        temperature=0,
-    )
-
-    assert response is not None
-    assert response["role"] == "function"
-    json_content = json.loads(response["content"])
-
-    # Replace the line below with a test for the final output in json_content
-    assert isinstance(json_content[0], str)
-
-"""
-TEMPLATE for testing a new plugin
-0. test the plugin with a prompt in ChatGPT
-1. make sure to replace the PLUGIN with the name of your plugin
-2. make sure to replace the PLUGIN_PROMPT with the prompt you used on ChatGPT
-3. replace the INTENTIONAL_FAILURE error with a test for the final output in json_content
-4. remove the segments under the DELETE comment
-"""
-# def test_initiate_and_fetch_PLUGIN():
-#     plugin = OpenPlugin("PLUGIN", verbose=True)
-#     assert plugin.manifest is not None
-
-#     # DELETE
-#     if not os.path.exists("logs"):
-#         os.makedirs("logs")
-#     with open("logs/manifest.json", "w") as f:
-#         f.write(json.dumps(plugin.manifest, indent=2))
-#     with open("logs/functions.json", "w") as f:
-#         f.write(json.dumps(plugin.functions, indent=2))
-    
-#     # create chatgpt request that will call the addTodo function
-#     chatgpt_prompt = 'PLUGIN_PROMPT'
-#     response = plugin.fetch_plugin(
-#         prompt=chatgpt_prompt,
-#         model="gpt-3.5-turbo-0613",
-#         temperature=0,
-#     )
-
-#     # DELETE
-#     with open("logs/plugin_response.json", "w") as f:
-#         f.write(json.dumps(response, indent=2))
-
-#     assert response is not None
-#     assert response["role"] == "function"
-#     json_content = json.loads(response["content"])
-
-#     # Replace the line below with a test for the final output in json_content
-#     raise Exception("INTENTIONAL_FAILURE")
-
+import json
+import pytest
+import os
+import openai
+from .mock_data import todo_plugin
+from openplugincore import OpenPlugin
+
+OPENAI_API_KEY = os.getenv('OPENAI_API_KEY')
+
+def test_initiate_and_fetch_todo():
+    plugin = OpenPlugin("__testing__")
+    assert plugin.manifest is not None
+    assert plugin.manifest.get("name_for_model") == "todo"
+
+    for function in plugin.functions:
+        if function["name"] == "addTodo":
+            addTodo = function
+        if function["name"] == "getTodos":
+            getTodos = function
+    
+    assert addTodo is not None
+    assert addTodo == todo_plugin["functions"][0]
+
+    assert getTodos is not None
+    assert getTodos == todo_plugin["functions"][1]
+
+    # fetch after chatgpt response
+    response = plugin.fetch_plugin(
+        prompt=todo_plugin["prompt"],
+        model="gpt-3.5-turbo-0613",
+        temperature=0,
+    )
+    assert response is not None
+    assert response["role"] == "function"
+    assert response["name"] == "addTodo"
+    json_content = json.loads(response["content"])
+    assert json_content["todo"] == "buy milk"
+
+def test_initiate_and_fetch_LGTM():
+    plugin = OpenPlugin("LGTM")
+    assert plugin.manifest is not None
+
+    # # create chatgpt request that will call the addTodo function
+    chatgpt_prompt = 'Show me markdown for a 2 by 2 table with LGTM'
+    response = plugin.fetch_plugin(
+        prompt=chatgpt_prompt,
+        model="gpt-3.5-turbo-0613",
+        temperature=0,
+    )
+
+    assert response is not None
+    assert response["role"] == "function"
+    json_content = json.loads(response["content"])
+    # # ensure that the json_content has a key of image_url and that is starts with https://lgtm.lol
+    assert "image_url" in json_content
+    assert json_content["image_url"].startswith("https://lgtm.lol")
+
+if False: # server too inconsistent
+    def test_initiate_and_fetch_Figlet():
+        plugin = OpenPlugin("Figlet")
+        assert plugin.manifest is not None
+
+        # create chatgpt request that will call the addTodo function
+        chatgpt_prompt = 'Convert "Testing" to the Doom ASCII font.'
+        response = plugin.fetch_plugin(
+            prompt=chatgpt_prompt,
+            model="gpt-3.5-turbo-0613",
+            temperature=0,
+        )
+
+        assert response is not None
+        assert response["role"] == "function"
+
+        json_content = json.loads(response["content"])
+        assert json_content["font"] == "doom"
+
+def test_initiate_and_fetch_yt_caption_retriever():
+    plugin = OpenPlugin("yt_caption_retriever")
+    assert plugin.manifest is not None
+
+    # create chatgpt request that will call the addTodo function
+    chatgpt_prompt = 'give me a 2 sentence summary of the following yt video https://www.youtube.com/watch?v=P310I19L3Ko'
+    response = plugin.fetch_plugin(
+        prompt=chatgpt_prompt,
+        model="gpt-3.5-turbo-0613",
+        temperature=0,
+    )
+
+    assert response is not None
+    assert response["role"] == "function"
+    json_content = json.loads(response["content"])
+
+    # Replace the line below with a test for the final output in json_content
+    assert "en" in json_content["captions"]
+
+def test_initiate_and_fetch_twtData():
+    plugin = OpenPlugin("twtData")
+    assert plugin.manifest is not None
+
+    # create chatgpt request that will call the addTodo function
+    chatgpt_prompt = 'show me the amount of people @Sebasti54919704 is following'
+    response = plugin.fetch_plugin(
+        prompt=chatgpt_prompt,
+        model="gpt-3.5-turbo-0613",
+        temperature=0,
+    )
+
+    assert response is not None
+    assert response["role"] == "function"
+    json_content = json.loads(response["content"])
+
+    # Replace the line below with a test for the final output in json_content
+    assert json_content["stats"]["account_found"] == True
+
+def test_initiate_and_fetch_tailor_erp():
+    plugin = OpenPlugin("tailor_erp")
+    assert plugin.manifest is not None
+
+    # create chatgpt request that will call the addTodo function
+    chatgpt_prompt = 'create a CRM template with ERP generator'
+    response = plugin.fetch_plugin(
+        prompt=chatgpt_prompt,
+        model="gpt-3.5-turbo-0613",
+        temperature=0,
+    )
+
+    assert response is not None
+    assert response["role"] == "function"
+    json_content = json.loads(response["content"])
+
+    # assert that json_content.applyTemplate.path is not None
+    assert json_content["APP_ID"] is not None
+
+def test_initiate_and_fetch_surge_ai_trends():
+    plugin = OpenPlugin("surge_ai_trends")
+    assert plugin.manifest is not None
+
+    # create chatgpt request that will call the addTodo function
+    chatgpt_prompt = 'What are the trnding searches for "gpu" in amazon'
+    response = plugin.fetch_plugin(
+        prompt=chatgpt_prompt,
+        model="gpt-3.5-turbo-0613",
+        temperature=0,
+    )
+
+    assert response is not None
+    assert response["role"] == "function"
+    json_content = json.loads(response["content"])
+
+    # assert that json_content.items is a list
+    assert isinstance(json_content["items"], list)
+
+def test_initiate_and_fetch_speedy_marketing():
+    plugin = OpenPlugin("speedy_marketing")
+    assert plugin.manifest is not None
+
+    # create chatgpt request that will call the addTodo function
+    chatgpt_prompt = 'write me an SEO blog about react for marketing'
+    response = plugin.fetch_plugin(
+        prompt=chatgpt_prompt,
+        model="gpt-3.5-turbo-0613",
+        temperature=0,
+    )
+
+    assert response is not None
+    assert response["role"] == "function"
+    json_content = json.loads(response["content"])
+
+    # Replace the line below with a test for the final output in json_content
+    assert isinstance(json_content["blog"], str)
+
+def test_initiate_and_fetch_socialsearch():
+    plugin = OpenPlugin("socialsearch")
+    assert plugin.manifest is not None
+    print("plugin.manifest: ", json.dumps(plugin.manifest, indent=2))
+    # create chatgpt request that will call the addTodo function
+    chatgpt_prompt = 'show me elon musk latest tweet'
+    response = plugin.fetch_plugin(
+        prompt=chatgpt_prompt,
+        verbose=True,
+        model="gpt-3.5-turbo-0613",
+        temperature=0,
+    )
+
+    assert response is not None
+    assert response["role"] == "function"
+    json_content = json.loads(response["content"])
+
+    # Replace the line below with a test for the final output in json_content
+    assert isinstance(json_content["message"], str)
+
+if False: # unable to convert url
+    def test_initiate_and_fetch_show_me_diagrams():
+        plugin = OpenPlugin("show_me_diagrams")
+        plugin.verbose = True
+        assert plugin.manifest is not None
+
+        # create chatgpt request that will call the addTodo function
+        chatgpt_prompt = 'make a diagram of one node connected to two others that will be yes or no'
+        response = plugin.fetch_plugin(
+            prompt=chatgpt_prompt,
+            model="gpt-3.5-turbo-0613",
+            temperature=0,
+        )
+
+        assert response is not None
+        assert response["role"] == "function"
+        json_content = json.loads(response["content"])
+
+        # Replace the line below with a test for the final output in json_content
+        assert isinstance(json_content["results"][0]["image"], str)
+
+def test_initiate_and_fetch_scholarai():
+    plugin = OpenPlugin("scholarai")
+    assert plugin.manifest is not None
+
+
+    # create chatgpt request that will call the addTodo function
+    chatgpt_prompt = 'What scientific research exists for semantic representation of language through brain waves. dont sort.'
+    response = plugin.fetch_plugin(
+        prompt=chatgpt_prompt,
+        model="gpt-3.5-turbo-0613",
+        temperature=0,
+    )
+
+    assert response is not None
+    assert response["role"] == "function"
+    json_content = json.loads(response["content"])
+
+    # Replace the line below with a test for the final output in json_content
+    assert isinstance(json_content["total_num_results"], int)
+
+def test_initiate_and_fetch_rephrase():
+    plugin = OpenPlugin("rephrase")
+    assert plugin.manifest is not None
+
+    # create chatgpt request that will call the addTodo function
+    chatgpt_prompt = 'I want to code a react ui with hello world please rephrase that'
+    response = plugin.fetch_plugin(
+        prompt=chatgpt_prompt,
+        model="gpt-3.5-turbo-0613",
+        temperature=0,
+    )
+
+    assert response is not None
+    assert response["role"] == "function"
+    json_content = json.loads(response["content"])
+
+    # Replace the line below with a test for the final output in json_content
+    assert isinstance(json_content["rephrased"]["text"], str)
+
+def test_initiate_and_fetch_DreamInterpreter():
+    plugin = OpenPlugin("DreamInterpreter", verbose=True)
+    assert plugin.manifest is not None
+    
+    # create chatgpt request that will call the addTodo function
+    chatgpt_prompt = 'I dreamt of being in a room without any windows getting smaller overtime'
+    response = plugin.fetch_plugin(
+        prompt=chatgpt_prompt,
+        model="gpt-3.5-turbo-0613",
+        temperature=0,
+    )
+
+    assert response is not None
+    assert response["role"] == "function"
+    json_content = json.loads(response["content"])
+
+    # Replace the line below with a test for the final output in json_content
+    assert isinstance(json_content["dreamResult"], str)
+
+def test_initiate_and_fetch_portfoliopilot():
+    plugin = OpenPlugin("portfoliopilot", verbose=True)
+    assert plugin.manifest is not None
+    
+    # create chatgpt request that will call the addTodo function
+    chatgpt_prompt = 'What stocks should I add for my long term tech portfolio'
+    response = plugin.fetch_plugin(
+        prompt=chatgpt_prompt,
+        model="gpt-3.5-turbo-0613",
+        temperature=0,
+    )
+
+    assert response is not None
+    assert response["role"] == "function"
+    json_content = json.loads(response["content"])
+
+    # Replace the line below with a test for the final output in json_content
+    assert isinstance(json_content["top_stocks"], list)
+
+def test_initiate_and_fetch_C3_Glide():
+    plugin = OpenPlugin("C3_Glide", verbose=True)
+    assert plugin.manifest is not None
+    
+    # create chatgpt request that will call the addTodo function
+    chatgpt_prompt = 'Provide me TAF for KJFK with reguards to aviation weather'
+    response = plugin.fetch_plugin(
+        prompt=chatgpt_prompt,
+        model="gpt-3.5-turbo-0613",
+        temperature=0,
+    )
+
+    assert response is not None
+    assert response["role"] == "function"
+    json_content = json.loads(response["content"])
+
+    # Replace the line below with a test for the final output in json_content
+    assert isinstance(json_content["tafs"], list)
+
+def test_initiate_and_fetch_Ai_PDF():
+    plugin = OpenPlugin("Ai_PDF", verbose=True)
+    assert plugin.manifest is not None
+    
+    # create chatgpt request that will call the addTodo function
+    chatgpt_prompt = 'Can I have my data be private according to this pdf https://www.unodc.org/pdf/criminal_justice/UN_Basic_Principles_on_the_Role_of_Lawyers.pdf'
+    response = plugin.fetch_plugin(
+        prompt=chatgpt_prompt,
+        model="gpt-3.5-turbo-0613",
+        temperature=0,
+    )
+
+    assert response is not None
+    assert response["role"] == "function"
+    json_content = json.loads(response["content"])
+
+    # Replace the line below with a test for the final output in json_content
+    assert isinstance(json_content[0], str)
+
+"""
+TEMPLATE for testing a new plugin
+0. test the plugin with a prompt in ChatGPT
+1. make sure to replace the PLUGIN with the name of your plugin
+2. make sure to replace the PLUGIN_PROMPT with the prompt you used on ChatGPT
+3. replace the INTENTIONAL_FAILURE error with a test for the final output in json_content
+4. remove the segments under the DELETE comment
+"""
+# def test_initiate_and_fetch_PLUGIN():
+#     plugin = OpenPlugin("PLUGIN", verbose=True)
+#     assert plugin.manifest is not None
+
+#     # DELETE
+#     if not os.path.exists("logs"):
+#         os.makedirs("logs")
+#     with open("logs/manifest.json", "w") as f:
+#         f.write(json.dumps(plugin.manifest, indent=2))
+#     with open("logs/functions.json", "w") as f:
+#         f.write(json.dumps(plugin.functions, indent=2))
+    
+#     # create chatgpt request that will call the addTodo function
+#     chatgpt_prompt = 'PLUGIN_PROMPT'
+#     response = plugin.fetch_plugin(
+#         prompt=chatgpt_prompt,
+#         model="gpt-3.5-turbo-0613",
+#         temperature=0,
+#     )
+
+#     # DELETE
+#     with open("logs/plugin_response.json", "w") as f:
+#         f.write(json.dumps(response, indent=2))
+
+#     assert response is not None
+#     assert response["role"] == "function"
+#     json_content = json.loads(response["content"])
+
+#     # Replace the line below with a test for the final output in json_content
+#     raise Exception("INTENTIONAL_FAILURE")
+
```

