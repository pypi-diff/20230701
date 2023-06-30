# Comparing `tmp/codespeak-0.1.2.tar.gz` & `tmp/codespeak-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codespeak-0.1.2.tar", max compression
+gzip compressed data, was "codespeak-0.1.3.tar", max compression
```

## Comparing `codespeak-0.1.2.tar` & `codespeak-0.1.3.tar`

### file list

```diff
@@ -1,54 +1,56 @@
--rw-r--r--   0        0        0     5715 2023-06-20 19:39:40.677547 codespeak-0.1.2/README.md
--rw-r--r--   0        0        0     6148 2023-06-13 18:29:30.684245 codespeak-0.1.2/codespeak/.DS_Store
--rw-r--r--   0        0        0      153 2023-06-20 19:39:40.677947 codespeak-0.1.2/codespeak/__init__.py
--rw-r--r--   0        0        0     4411 2023-06-20 19:39:40.678280 codespeak-0.1.2/codespeak/_clean.py
--rw-r--r--   0        0        0      541 2023-06-20 19:39:40.678546 codespeak-0.1.2/codespeak/_cli/main.py
--rw-r--r--   0        0        0        0 2023-06-20 19:39:40.678610 codespeak-0.1.2/codespeak/_core/__init__.py
--rw-r--r--   0        0        0     7148 2023-06-20 19:39:40.678871 codespeak-0.1.2/codespeak/_core/code_generator.py
--rw-r--r--   0        0        0     5755 2023-06-20 19:39:40.679073 codespeak-0.1.2/codespeak/_core/codespeak_service.py
--rw-r--r--   0        0        0     1433 2023-06-20 19:39:40.679249 codespeak-0.1.2/codespeak/_core/diff.py
--rw-r--r--   0        0        0     1444 2023-06-20 19:39:40.679443 codespeak-0.1.2/codespeak/_core/executor.py
--rw-r--r--   0        0        0     3058 2023-06-20 19:39:40.679626 codespeak-0.1.2/codespeak/_core/openai_service.py
--rw-r--r--   0        0        0     2723 2023-06-20 19:39:40.679773 codespeak-0.1.2/codespeak/_core/prompt.py
--rw-r--r--   0        0        0     4043 2023-06-20 19:39:40.679962 codespeak-0.1.2/codespeak/_core/results_collector.py
--rw-r--r--   0        0        0     2555 2023-06-20 19:39:40.680156 codespeak-0.1.2/codespeak/_declaration/body_imports.py
--rw-r--r--   0        0        0     5144 2023-06-20 19:39:40.680337 codespeak-0.1.2/codespeak/_declaration/codespeak_declaration.py
--rw-r--r--   0        0        0     6200 2023-06-20 19:39:40.680582 codespeak-0.1.2/codespeak/_declaration/declaration_file_service.py
--rw-r--r--   0        0        0     1716 2023-06-20 19:39:40.680747 codespeak-0.1.2/codespeak/_declaration/declaration_helpers.py
--rw-r--r--   0        0        0     3363 2023-06-20 19:39:40.681007 codespeak-0.1.2/codespeak/_decorate.py
--rw-r--r--   0        0        0       91 2023-06-20 19:39:40.681118 codespeak-0.1.2/codespeak/_definitions/__init__.py
--rw-r--r--   0        0        0     5659 2023-06-20 19:39:40.681303 codespeak-0.1.2/codespeak/_definitions/classify.py
--rw-r--r--   0        0        0      919 2023-06-20 19:39:40.681422 codespeak-0.1.2/codespeak/_definitions/definition.py
--rw-r--r--   0        0        0     1046 2023-06-20 19:39:40.681540 codespeak-0.1.2/codespeak/_definitions/free_modules.py
--rw-r--r--   0        0        0      492 2023-06-20 19:39:40.681714 codespeak-0.1.2/codespeak/_definitions/types/builtin.py
--rw-r--r--   0        0        0      672 2023-06-20 19:39:40.681864 codespeak-0.1.2/codespeak/_definitions/types/custom_type_reference.py
--rw-r--r--   0        0        0      498 2023-06-20 19:39:40.682010 codespeak-0.1.2/codespeak/_definitions/types/generic.py
--rw-r--r--   0        0        0      649 2023-06-20 19:39:40.682171 codespeak-0.1.2/codespeak/_definitions/types/installed_class.py
--rw-r--r--   0        0        0     2987 2023-06-20 19:39:40.682339 codespeak-0.1.2/codespeak/_definitions/types/local_class.py
--rw-r--r--   0        0        0     1196 2023-06-20 19:39:40.682503 codespeak-0.1.2/codespeak/_definitions/types/local_class_as_self.py
--rw-r--r--   0        0        0      477 2023-06-20 19:39:40.682674 codespeak-0.1.2/codespeak/_definitions/types/none.py
--rw-r--r--   0        0        0     1955 2023-06-20 19:39:40.682849 codespeak-0.1.2/codespeak/_definitions/types/typing_type.py
--rw-r--r--   0        0        0      636 2023-06-20 19:39:40.683011 codespeak-0.1.2/codespeak/_definitions/types/union_type.py
--rw-r--r--   0        0        0      561 2023-06-20 19:39:40.683191 codespeak-0.1.2/codespeak/_definitions/utils/dedupe.py
--rw-r--r--   0        0        0      560 2023-06-20 19:39:40.683334 codespeak-0.1.2/codespeak/_definitions/utils/flat_uniques.py
--rw-r--r--   0        0        0      277 2023-06-20 19:39:40.683486 codespeak-0.1.2/codespeak/_definitions/utils/flatten.py
--rw-r--r--   0        0        0      400 2023-06-20 19:39:40.683646 codespeak-0.1.2/codespeak/_definitions/utils/group.py
--rw-r--r--   0        0        0     1133 2023-06-20 19:39:40.683802 codespeak-0.1.2/codespeak/_definitions/utils/swap_custom_types.py
--rw-r--r--   0        0        0        0 2023-06-20 19:39:40.683843 codespeak-0.1.2/codespeak/_helpers/__init__.py
--rw-r--r--   0        0        0      875 2023-06-20 19:39:40.684119 codespeak-0.1.2/codespeak/_helpers/auto_detect_abspath_to_project_root.py
--rw-r--r--   0        0        0      495 2023-06-20 19:39:40.684233 codespeak-0.1.2/codespeak/_helpers/gather_arguments.py
--rw-r--r--   0        0        0      363 2023-06-20 19:39:40.684357 codespeak-0.1.2/codespeak/_helpers/get_attr_from_qualname.py
--rw-r--r--   0        0        0      530 2023-06-20 19:39:40.684491 codespeak-0.1.2/codespeak/_helpers/self_type.py
--rw-r--r--   0        0        0      388 2023-06-20 19:39:40.684583 codespeak-0.1.2/codespeak/_helpers/set_attr_for_qualname.py
--rw-r--r--   0        0        0      310 2023-06-20 19:39:40.684732 codespeak-0.1.2/codespeak/_metadata/__init__.py
--rw-r--r--   0        0        0     1029 2023-06-20 19:39:40.684841 codespeak-0.1.2/codespeak/_metadata/digest.py
--rw-r--r--   0        0        0     2164 2023-06-20 19:39:40.685005 codespeak-0.1.2/codespeak/_settings/_settings.py
--rw-r--r--   0        0        0       83 2023-06-20 19:39:40.685229 codespeak-0.1.2/codespeak/_settings/environment.py
--rw-r--r--   0        0        0       74 2023-06-20 19:39:40.685405 codespeak-0.1.2/codespeak/public/codespeak_helpers/__init__.py
--rw-r--r--   0        0        0     1265 2023-06-20 19:39:40.685580 codespeak-0.1.2/codespeak/public/codespeak_helpers/generate.py
--rw-r--r--   0        0        0     2056 2023-06-20 19:39:40.685742 codespeak-0.1.2/codespeak/public/codespeak_helpers/unsafe_execute.py
--rw-r--r--   0        0        0     1813 2023-06-20 19:39:40.685906 codespeak-0.1.2/codespeak/public/codespeak_settings.py
--rw-r--r--   0        0        0      194 2023-06-20 19:39:40.686058 codespeak-0.1.2/codespeak/public/example_return.py
--rw-r--r--   0        0        0      632 2023-06-20 19:39:40.686161 codespeak-0.1.2/codespeak/public/generated_exception.py
--rw-r--r--   0        0        0      457 2023-06-20 19:40:57.543890 codespeak-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 codespeak-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     8297 2023-06-30 22:27:56.734266 codespeak-0.1.3/README.md
+-rw-r--r--   0        0        0     6148 2023-06-13 18:29:30.684245 codespeak-0.1.3/codespeak/.DS_Store
+-rw-r--r--   0        0        0      407 2023-06-28 19:18:32.065524 codespeak-0.1.3/codespeak/__init__.py
+-rw-r--r--   0        0        0     4366 2023-06-28 01:05:00.663878 codespeak-0.1.3/codespeak/clean.py
+-rw-r--r--   0        0        0      539 2023-06-28 01:05:00.664137 codespeak-0.1.3/codespeak/cli/main.py
+-rw-r--r--   0        0        0       77 2023-06-30 18:42:40.227352 codespeak-0.1.3/codespeak/constants.py
+-rw-r--r--   0        0        0     3071 2023-06-29 22:46:49.809872 codespeak-0.1.3/codespeak/decorate/infer.py
+-rw-r--r--   0        0        0      838 2023-06-28 01:05:00.667487 codespeak-0.1.3/codespeak/executor.py
+-rw-r--r--   0        0        0     4033 2023-06-29 22:46:49.810219 codespeak-0.1.3/codespeak/frame.py
+-rw-r--r--   0        0        0      336 2023-06-28 19:19:34.165480 codespeak-0.1.3/codespeak/frame_tests.py
+-rw-r--r--   0        0        0       31 2023-06-28 01:05:00.667805 codespeak-0.1.3/codespeak/function/__init__.py
+-rw-r--r--   0        0        0     6532 2023-06-29 22:46:49.810576 codespeak-0.1.3/codespeak/function/function.py
+-rw-r--r--   0        0        0      161 2023-06-29 21:46:09.662368 codespeak-0.1.3/codespeak/function/function_attributes.py
+-rw-r--r--   0        0        0     4139 2023-06-29 22:46:49.810885 codespeak-0.1.3/codespeak/function/function_declaration.py
+-rw-r--r--   0        0        0     1558 2023-06-29 22:46:49.811215 codespeak-0.1.3/codespeak/function/function_digest.py
+-rw-r--r--   0        0        0     5001 2023-06-29 22:46:49.811530 codespeak-0.1.3/codespeak/function/function_file_service.py
+-rw-r--r--   0        0        0      720 2023-06-28 01:05:00.668743 codespeak-0.1.3/codespeak/function/function_manager.py
+-rw-r--r--   0        0        0      695 2023-06-29 22:46:49.811862 codespeak-0.1.3/codespeak/function/function_metadata.py
+-rw-r--r--   0        0        0     1185 2023-06-28 19:18:32.067533 codespeak-0.1.3/codespeak/function/function_resources.py
+-rw-r--r--   0        0        0      150 2023-06-28 01:05:00.669222 codespeak-0.1.3/codespeak/function/helper_types/make_inference_response.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:05:00.670065 codespeak-0.1.3/codespeak/helpers/__init__.py
+-rw-r--r--   0        0        0      747 2023-06-28 19:18:32.067930 codespeak-0.1.3/codespeak/helpers/auto_detect_abspath_to_project_root.py
+-rw-r--r--   0        0        0     1424 2023-06-28 01:05:00.670419 codespeak-0.1.3/codespeak/helpers/derive_module_qualname_for_object.py
+-rw-r--r--   0        0        0      503 2023-06-28 01:05:00.670656 codespeak-0.1.3/codespeak/helpers/gather_arguments.py
+-rw-r--r--   0        0        0      363 2023-06-28 01:05:00.670750 codespeak-0.1.3/codespeak/helpers/get_attr_from_qualname.py
+-rw-r--r--   0        0        0      730 2023-06-29 22:46:49.812250 codespeak-0.1.3/codespeak/helpers/get_definitions_from_function_signature.py
+-rw-r--r--   0        0        0      464 2023-06-28 19:18:32.068181 codespeak-0.1.3/codespeak/helpers/guarantee_abspath_to_root_exists.py
+-rw-r--r--   0        0        0      531 2023-06-28 01:05:00.670895 codespeak-0.1.3/codespeak/helpers/self_type.py
+-rw-r--r--   0        0        0      388 2023-06-28 01:05:00.670990 codespeak-0.1.3/codespeak/helpers/set_attr_for_qualname.py
+-rw-r--r--   0        0        0     6092 2023-06-28 19:38:20.277870 codespeak-0.1.3/codespeak/inference/codespeak_service.py
+-rw-r--r--   0        0        0     7494 2023-06-29 22:46:49.812583 codespeak-0.1.3/codespeak/inference/inference_engine.py
+-rw-r--r--   0        0        0     3089 2023-06-29 22:46:49.812871 codespeak-0.1.3/codespeak/inference/openai_service.py
+-rw-r--r--   0        0        0     2711 2023-06-29 22:46:49.813165 codespeak-0.1.3/codespeak/inference/prompt.py
+-rw-r--r--   0        0        0     4042 2023-06-28 01:05:00.671847 codespeak-0.1.3/codespeak/inference/results_collector.py
+-rw-r--r--   0        0        0     1491 2023-06-28 19:18:32.068890 codespeak-0.1.3/codespeak/module_frame.py
+-rw-r--r--   0        0        0      194 2023-06-20 19:39:40.686058 codespeak-0.1.3/codespeak/public/example_return.py
+-rw-r--r--   0        0        0      675 2023-06-28 01:05:00.672008 codespeak-0.1.3/codespeak/public/inferred_exception.py
+-rw-r--r--   0        0        0     1811 2023-06-28 01:05:00.672152 codespeak-0.1.3/codespeak/public/settings.py
+-rw-r--r--   0        0        0     2363 2023-06-29 22:46:49.813468 codespeak-0.1.3/codespeak/settings/_settings.py
+-rw-r--r--   0        0        0       83 2023-06-29 21:13:50.829187 codespeak-0.1.3/codespeak/settings/environment.py
+-rw-r--r--   0        0        0      478 2023-06-28 19:18:32.069006 codespeak-0.1.3/codespeak/test_function.py
+-rw-r--r--   0        0        0     5627 2023-06-29 22:46:49.813683 codespeak-0.1.3/codespeak/type_definitions/classify.py
+-rw-r--r--   0        0        0     1046 2023-06-29 22:46:49.813932 codespeak-0.1.3/codespeak/type_definitions/free_modules.py
+-rw-r--r--   0        0        0     1336 2023-06-29 22:46:49.814095 codespeak-0.1.3/codespeak/type_definitions/type_definition.py
+-rw-r--r--   0        0        0      509 2023-06-29 22:46:49.814272 codespeak-0.1.3/codespeak/type_definitions/types/builtin.py
+-rw-r--r--   0        0        0      689 2023-06-29 22:46:49.814428 codespeak-0.1.3/codespeak/type_definitions/types/custom_type_reference.py
+-rw-r--r--   0        0        0      515 2023-06-29 22:46:49.814592 codespeak-0.1.3/codespeak/type_definitions/types/generic.py
+-rw-r--r--   0        0        0      666 2023-06-29 22:46:49.814762 codespeak-0.1.3/codespeak/type_definitions/types/installed_class.py
+-rw-r--r--   0        0        0     2826 2023-06-29 22:46:49.814941 codespeak-0.1.3/codespeak/type_definitions/types/local_class.py
+-rw-r--r--   0        0        0     1200 2023-06-29 22:46:49.815108 codespeak-0.1.3/codespeak/type_definitions/types/local_class_as_self.py
+-rw-r--r--   0        0        0      494 2023-06-29 22:46:49.815270 codespeak-0.1.3/codespeak/type_definitions/types/none.py
+-rw-r--r--   0        0        0     1929 2023-06-29 22:46:49.815433 codespeak-0.1.3/codespeak/type_definitions/types/typing_type.py
+-rw-r--r--   0        0        0      657 2023-06-29 22:46:49.815593 codespeak-0.1.3/codespeak/type_definitions/types/union_type.py
+-rw-r--r--   0        0        0     1162 2023-06-29 22:46:49.815772 codespeak-0.1.3/codespeak/type_definitions/utils/swap_custom_types.py
+-rw-r--r--   0        0        0      457 2023-06-30 22:29:46.891087 codespeak-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     8891 1970-01-01 00:00:00.000000 codespeak-0.1.3/PKG-INFO
```

### Comparing `codespeak-0.1.2/codespeak/.DS_Store` & `codespeak-0.1.3/codespeak/.DS_Store`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.2/codespeak/_clean.py` & `codespeak-0.1.3/codespeak/clean.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-"""cleans out codespeak_generated directory and removes unused functions"""
+"""cleans out codespeak_inferred directory and removes unused functions"""
 import os
 import fnmatch
 import shutil
 from typing import Any
 from importlib import import_module
-from codespeak._declaration.declaration_file_service import (
-    codegen_dirname,
-    metadata_file_prefix,
-)
 
-# if run as command, assume that it's in the same directory as the codespeak_generated directory
+from codespeak.constants import metadata_file_prefix, codegen_dirname
+
+# if run as command, assume that it's in the same directory as the codespeak_inferred directory
 # otherwise, get the rootpath and use that
 
 
 def extract_modulepath(abs_filepath: str):
     # Split the path into parts
     path_parts = abs_filepath.split(os.sep)
 
@@ -106,19 +104,19 @@
         return False
     return has_attr_from_qualname(module, func_qualname)
 
 
 # from cwd
 def codegen_directory_abspath() -> str:
     cwd = os.getcwd()
-    # Look for "codespeak_generated" in the current directory
+    # Look for "codespeak_inferred" in the current directory
     expected_path = os.path.join(cwd, codegen_dirname)
     if not os.path.isdir(expected_path):
         raise Exception(
-            f"Couldn't find 'codespeak_generated' directory, run from project root that contains 'codespeak_generated'"
+            f"Couldn't find 'codespeak_inferred' directory, run from project root that contains 'codespeak_inferred'"
         )
     return expected_path
 
 
 def clean(codegen_directory_abspath: str):
     remove_unused_generated_code(codegen_directory_abspath=codegen_directory_abspath)
```

### Comparing `codespeak-0.1.2/codespeak/_core/code_generator.py` & `codespeak-0.1.3/codespeak/inference/inference_engine.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # need to give it import paths
 
 import inspect
 from typing import Any, Callable, Dict, List
 from pydantic import BaseModel
 import pytest
-from codespeak._core.codespeak_service import CodespeakService
-from codespeak.public.generated_exception import GeneratedException
-from codespeak._core.executor import execute_unsafe
-from codespeak._core.results_collector import TestRunner
-from codespeak._declaration.codespeak_declaration import CodespeakDeclaration
+from codespeak.function.function_declaration import FunctionDeclaration
+from codespeak.inference.codespeak_service import CodespeakService
+from codespeak.function.function_file_service import FunctionFileService
+from codespeak.function.function_digest import FunctionDigest
+from codespeak.public.inferred_exception import InferredException
+from codespeak.executor import execute_unchecked
+from codespeak.inference.results_collector import TestRunner
+from codespeak.test_function import TestFunction
+from codespeak.settings import _settings
 
 
 class ExecutionResponse(BaseModel):
     result: Any
     did_regenerate_source: bool = False
 
 
@@ -20,151 +24,153 @@
     did_regenerate_source: bool
 
 
 class GenerationResponse(BaseModel):
     execution_result: Any | None = None
 
 
-class TestFunc(BaseModel):
-    file: str
-    qualname: str
-    source_code: str
-
-    @staticmethod
-    def from_callable(test_func: Callable) -> "TestFunc":
-        source_code = inspect.getsource(test_func)
-        file = inspect.getfile(test_func)
-        return TestFunc(
-            file=file,
-            qualname=test_func.__qualname__,
-            source_code=source_code,
-        )
-
-
-class CodeGenerator(BaseModel):
+class InferenceEngine(BaseModel):
     # not modified internally
-    declaration: CodespeakDeclaration
-    service: CodespeakService
+    function_declaration: FunctionDeclaration
+    file_service: FunctionFileService
+    digest: FunctionDigest
+    codespeak_service: CodespeakService
     should_execute: bool
     args: List[Any]
     kwargs: Dict[str, Any]
-    test_func: TestFunc | None
+    test_functions: List[TestFunction]
     latest_source_code: str = ""
 
-    def generate(self) -> GenerationResponse:
-        self.latest_source_code = self.service.generate_source_code()
+    def make_inference(self) -> GenerationResponse:
+        self.latest_source_code = self.codespeak_service.generate_source_code()
         return self._validate_new_source_code()
 
     @property
     def require_execution(self) -> bool:
         return self.should_execute
 
+    @property
+    def has_tests(self) -> bool:
+        return len(self.test_functions) > 0
+
     # this should always be called directly after new source code is generated and stored in self.latest_source_code
     def _validate_new_source_code(self) -> GenerationResponse:
         execution_result = None
-        self.declaration.file_service.write_logic(self.latest_source_code)
-        self.declaration.file_service.write_metadata(
-            source_code=self.declaration.source_code,
+        self.file_service.write_logic(self.latest_source_code)
+        self.file_service.write_metadata(
+            source_code=self.function_declaration.source_code,
             require_execution=self.require_execution,
             did_execute=False,
-            has_tests=(not self.test_func is None),
+            has_tests=self.has_tests,
             did_pass_tests=False,
-            digest=self.declaration.digest,
+            digest=self.digest,
         )
         if self.should_execute:
             execution_response = self._try_align_with_execution()
             execution_result = execution_response.result
             if execution_response.did_regenerate_source:
                 return self._validate_new_source_code()
-        if self.test_func:
+        if self.has_tests:
             test_response = self._try_align_with_tests()
             if test_response.did_regenerate_source:
                 return self._validate_new_source_code()
         return GenerationResponse(execution_result=execution_result)
 
     def _try_align_with_execution(self) -> ExecutionResponse:
         try:
-            result = execute_unsafe(
-                self.declaration.file_service.generated_module_qualname,
-                self.declaration.file_service.generated_entrypoint,
+            result = execute_unchecked(
+                self.file_service.generated_module_qualname,
+                self.file_service.generated_entrypoint,
                 *self.args,
                 **self.kwargs,
             )
             self._write_execution_status(did_execute=True)
             return ExecutionResponse(result=result, did_regenerate_source=False)
         except Exception as e:
-            if isinstance(e, GeneratedException):
-                # if the generated code properly raises a GeneratedException, we don't want to regenerate it the next time it's called
+            if isinstance(e, InferredException):
+                # if the generated code properly raises a InferredException, we don't want to regenerate it the next time it's called
                 self._write_execution_status(
                     did_execute=True,
                 )
-                raise e.exception
+                raise e
             else:
                 self.latest_source_code = (
-                    self.service.try_regenerate_from_execution_failure(exception=e)
+                    self.codespeak_service.try_regenerate_from_execution_failure(
+                        exception=e
+                    )
                 )
                 return ExecutionResponse(result=None, did_regenerate_source=True)
 
     def _try_align_with_tests(self) -> TestResponse:
-        if not self.test_func:
+        if not self.has_tests:
             raise Exception("trying to test without a test func")
-        self._write_test_status(has_tests=False, did_pass_tests=False)
-        test_result = TestRunner.run_test_func(
-            test_file=self.test_func.file,
-            test_func_qualname=self.test_func.qualname,
+        total_duration = 0
+        _settings.set_is_testing(
+            True, logic_at_filepath=self.file_service.codegen_logic_filepath
         )
-        did_pass_tests = test_result.exitcode == pytest.ExitCode.OK
-        self._write_test_status(has_tests=False, did_pass_tests=did_pass_tests)
-        if test_result.exitcode == pytest.ExitCode.OK:
-            print(f"All tests passed successfully in {test_result.total_duration}s")
-            return TestResponse(did_regenerate_source=False)
-        elif test_result.exitcode == pytest.ExitCode.TESTS_FAILED:
-            print("Some tests failed.")
-            if len(test_result.crash_reports) == 0:
-                raise Exception("no crash reports but tests failed")
-            self.latest_source_code = self.service.try_regenerate_from_test_failure(
-                test_source_code=self.test_func.source_code,
-                crash_report=test_result.crash_reports[0],
+        for test_function in self.test_functions:
+            test_result = TestRunner.run_test_func(
+                test_file=test_function.file,
+                test_func_qualname=test_function.qualname,
             )
-            return TestResponse(did_regenerate_source=True)
-        else:
-            raise exception_for_exitcode(test_result.exitcode)
+            total_duration += test_result.total_duration
+            if test_result.exitcode == pytest.ExitCode.OK:
+                continue
+            elif test_result.exitcode == pytest.ExitCode.TESTS_FAILED:
+                _settings.set_is_testing(False)
+                self._write_test_status(has_tests=True, did_pass_tests=False)
+                print("Some tests failed.")
+                if len(test_result.crash_reports) == 0:
+                    raise Exception("no crash reports but tests failed")
+                self.latest_source_code = (
+                    self.codespeak_service.try_regenerate_from_test_failure(
+                        test_source_code=test_function.source_code,
+                        crash_report=test_result.crash_reports[0],
+                    )
+                )
+                return TestResponse(did_regenerate_source=True)
+            else:
+                raise exception_for_exitcode(test_result.exitcode)
+        print(f"All tests passed successfully in {total_duration}s")
+        _settings.set_is_testing(False)
+        self._write_test_status(has_tests=True, did_pass_tests=True)
+        return TestResponse(did_regenerate_source=False)
 
     def _write_execution_status(self, did_execute: bool) -> None:
-        prev_metadata = self.declaration.file_service.load_metadata()
+        prev_metadata = self.file_service.load_metadata()
         if prev_metadata:
             has_tests = prev_metadata.has_tests
             did_pass_tests = prev_metadata.did_pass_tests
         else:
-            has_tests = not self.test_func is None
+            has_tests = self.has_tests
             did_pass_tests = False
-        self.declaration.file_service.write_metadata(
-            source_code=self.declaration.source_code,
+        self.file_service.write_metadata(
+            source_code=self.function_declaration.source_code,
             require_execution=self.require_execution,
             did_execute=did_execute,
             has_tests=has_tests,
             did_pass_tests=did_pass_tests,
-            digest=self.declaration.digest,
+            digest=self.digest,
         )
 
     def _write_test_status(self, has_tests: bool, did_pass_tests: bool) -> None:
-        prev_metadata = self.declaration.file_service.load_metadata()
+        prev_metadata = self.file_service.load_metadata()
         if prev_metadata:
             did_execute = prev_metadata.did_execute
             require_execution = prev_metadata.require_execution
         else:
             did_execute = False
             require_execution = self.should_execute
-        self.declaration.file_service.write_metadata(
-            source_code=self.declaration.source_code,
+        self.file_service.write_metadata(
+            source_code=self.function_declaration.source_code,
             require_execution=require_execution,
             did_execute=did_execute,
             has_tests=has_tests,
             did_pass_tests=did_pass_tests,
-            digest=self.declaration.digest,
+            digest=self.digest,
         )
 
 
 def exception_for_exitcode(exitcode: int) -> Exception:
     msg = ""
     if exitcode == pytest.ExitCode.INTERRUPTED:
         msg = "Test execution interrupted by the user."
```

### Comparing `codespeak-0.1.2/codespeak/_core/codespeak_service.py` & `codespeak-0.1.3/codespeak/inference/codespeak_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,101 +1,109 @@
+import json
 import re
 from pydantic import BaseModel
-from codespeak._core import prompt
-from codespeak._core.openai_service import OpenAIService, Roles
-from codespeak._core.results_collector import CrashReport
-from codespeak._settings._settings import get_verbose
-from codespeak._declaration.codespeak_declaration import CodespeakDeclaration
+from codespeak.frame import Frame
+from codespeak.function.function_declaration import FunctionDeclaration
+from codespeak.inference import prompt
+from codespeak.inference.openai_service import OpenAIService, Roles
+from codespeak.inference.results_collector import CrashReport
+from codespeak.settings._settings import get_verbose
 
 
 class IterationState(BaseModel):
     num_code_versions: int = 0
     max_code_versions: int = 3
     num_test_versions: int = 0
     max_test_versions: int = 3
     num_bad_formatting_versions: int = 0
     max_bad_formatting_versions: int = 3
 
 
 class CodespeakService(BaseModel):
     openai_service: OpenAIService
     iterations: IterationState
-    declaration: CodespeakDeclaration
+    function_declaration: FunctionDeclaration
+    frame: Frame
 
     @staticmethod
-    def with_defaults(declaration: CodespeakDeclaration) -> "CodespeakService":
+    def with_defaults(
+        function_declaration: FunctionDeclaration, frame: Frame
+    ) -> "CodespeakService":
         return CodespeakService(
             openai_service=OpenAIService.with_defaults(),
             iterations=IterationState(),
-            declaration=declaration,
+            function_declaration=function_declaration,
+            frame=frame,
         )
 
     def generate_source_code(self) -> str:
-        _prompt = prompt.make(
-            incomplete_file=self.declaration.as_incomplete_file(),
-            custom_types=self.declaration.as_custom_types_str(),
-            declaration_docstring=self.declaration.docstring,
+        custom_types = {"custom_types": self.frame.custom_types()}
+        custom_types_str = json.dumps(custom_types, indent=4)
+        _prompt = prompt.make_prompt(
+            incomplete_file=self.function_declaration.as_incomplete_file(),
+            custom_types_str=custom_types_str,
+            declaration_docstring=self.function_declaration.docstring,
             verbose=get_verbose(),
         )
         return self._fetch_new_source_code(prompt=_prompt)
 
     def _fetch_new_source_code(self, prompt: str) -> str:
         response = self.openai_service.send_user_message(content=prompt)
         if " raise" in response:
-            if not "GeneratedException" in response:
+            if not "InferredException" in response:
                 print("possible manual exception will cause regen in future")
         source_code = self._guarantee_source_formatting(response)
         return source_code
 
     def try_regenerate_from_execution_failure(
         self,
         exception: Exception,
     ) -> str:
         if self.iterations.num_code_versions < self.iterations.max_code_versions:
             print(
                 "regenerating for func: ",
-                self.declaration.qualname,
+                self.function_declaration.qualname,
                 " num attempt: ",
                 self.iterations.num_code_versions + 1,
             )
             print("in response to exception: ", exception)
             self.iterations.num_code_versions += 1
             return self._fetch_new_source_code(
                 prompt=self._corrective_message_for_execution_failure(exception)
             )
         else:
             raise Exception(
-                f"Unable to generate code that executes with the given arguments for {self.declaration.qualname}. Make sure your arguments are of the correct type, clarify your types, or modify your docstring."
+                f"Unable to generate code that executes with the given arguments for {self.function_declaration.qualname}. Make sure your arguments are of the correct type, clarify your types, or modify your docstring."
             )
 
     def try_regenerate_from_test_failure(
         self, test_source_code: str, crash_report: CrashReport
     ) -> str:
         if self.iterations.num_test_versions < self.iterations.max_test_versions:
             print(
                 "regenerating after failed tests for func: ",
-                self.declaration.qualname,
+                self.function_declaration.qualname,
                 " num attempt: ",
                 self.iterations.num_test_versions + 1,
             )
             self.iterations.num_test_versions += 1
             prompt = self._corrective_message_for_test_failure(
                 test_source_code=test_source_code,
                 crash_report=crash_report,
             )
             return self._fetch_new_source_code(prompt=prompt)
         else:
             raise Exception(
-                f"Unable to generate code that executes with the given arguments for {self.declaration.qualname}. Make sure your arguments are of the correct type, clarify your types, or modify your docstring."
+                f"Unable to generate code that executes with the given arguments for {self.function_declaration.qualname}. Make sure your arguments are of the correct type, clarify your types, or modify your docstring."
             )
 
     def _guarantee_source_formatting(self, response: str) -> str:
         pattern = r"```python(.*?)```"
         match = re.search(pattern, response, re.DOTALL)
-        if match:
+        if match is not None:
             return match.group(
                 1
             ).strip()  # group(1) to get the content between the backticks
         else:
             if (
                 self.iterations.num_bad_formatting_versions
                 < self.iterations.max_bad_formatting_versions
@@ -108,15 +116,15 @@
             else:
                 raise Exception("Too many bad formatting versions")
 
     def _corrective_message_for_execution_failure(self, exception: Exception) -> str:
         msg = "The previous code did not execute. It returned the following exception:"
         msg += f"\n```\n{exception}\n```\n\n"
         msg += "Use the same information in my original message to complete the original task."
-        msg += " When correcting your response, be sure to think about the root cause of the exception and adjust for it. Remember, if you want to raise an exception, wrap it in GeneratedException."
+        msg += " When correcting your response, be sure to think about the root cause of the exception and adjust for it. Remember, if you want to raise an exception, wrap it in InferredException."
         return msg
 
     def _corrective_message_for_test_failure(
         self, test_source_code: str, crash_report: CrashReport
     ) -> str:
         msg = f"The following tests were executed: \n```\n{test_source_code}\n```\n\n"
         msg += "The tests failed with message:\n```\n"
```

### Comparing `codespeak-0.1.2/codespeak/_core/openai_service.py` & `codespeak-0.1.3/codespeak/inference/openai_service.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 import openai
 from typing import Any, List
 
 from pydantic import BaseModel, validator
-from codespeak._settings import _settings
+from codespeak.settings import _settings
 
 
 class Roles:
     @staticmethod
     def user():
         return "user"
 
@@ -40,15 +40,15 @@
     @staticmethod
     def with_defaults():
         return OpenAIService(
             model=_settings.get_openai_model(),
             messages=[
                 Message(
                     role=Roles.system(),
-                    content="You are a competent and diligent python programmer.",
+                    content="You are a competent and diligent python programmer. You write python code.",
                 ),
             ],
             num_retries=0,
         )
 
     def json_messages(self):
         return [m.dict() for m in self.messages]
@@ -72,27 +72,27 @@
         try:
             response: Any = openai.ChatCompletion.create(
                 model=self.model,
                 messages=self.json_messages(),
                 stream=True,
             )
             result = ""
-            print("\n\n------START CODEGEN------\n\n")
+            print("\n\n------MAKING INFERENCE------\n\n")
             for chunk in response:
                 chunk: Any = chunk
                 choices: list = chunk.choices
-                if not choices:
+                if choices is None:
                     raise Exception("choices does not exist on completion")
                 if len(choices) == 0:
                     continue
                 delta = choices[0].delta
                 if "content" in delta:
                     result += delta.content
                     print(f"{delta.content}", end="")
-            print("\n\n------END CODEGEN------\n\n")
+            print("\n\n------END INFERENCE------\n\n")
             return result
         except Exception as e:
             if self.num_retries < 5:
                 print("retr completion!!!")
                 self.num_retries += 1
                 time.sleep(1)
                 return self.get_completion()
```

### Comparing `codespeak-0.1.2/codespeak/_core/prompt.py` & `codespeak-0.1.3/codespeak/inference/prompt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Callable, Dict, List, OrderedDict, Type
 import textwrap
 
 
-def make(
+def make_prompt(
     incomplete_file: str,
-    custom_types: str,
+    custom_types_str: str,
     declaration_docstring: str,
     verbose: bool = True,
 ) -> str:
-    text = prompt_text(incomplete_file, custom_types, declaration_docstring)
+    text = prompt_text(incomplete_file, custom_types_str, declaration_docstring)
     if verbose:
         print("\n\n------START PROMPT------\n\n")
         print(text)
         print("\n\n------END PROMPT------\n\n")
     return text
 
 
 def prompt_text(
-    incomplete_file: str, custom_types: str, declaration_docstring: str
+    incomplete_file: str, custom_types_str: str, declaration_docstring: str
 ) -> str:
     return textwrap.dedent(
         f"""
 The following message contains an incomplete python file. 
 
 The file has imports and an incomplete function. Your task is to return the completed version of the file. 
 
@@ -39,25 +39,25 @@
 
 When available, use the incomplete function's name, parameter names, parameter types, and return type to further understand its intent.
 
 You have an entire python interpreter at your disposal. In the completed file, import modules and define helper functions as needed. Be sure to use the incomplete function's exact signature in your completed file.
 
 Here is a json object that contains metadata about custom python types that are relevant to the file. All of these types are already defined and they're available to your file via import. Do not redefine them. Use them as needed to complete the file:
 ```
-{custom_types}
+{custom_types_str}
 ```
 
 
 For installed types, use the qualname and module to recall your existing knowledge of their variables and methods. For local types, use the type hints and source code provided to understand how they could be used.  
 
-Extremely common types, such as those from python's builtin module or the typing module, are intentionally excluded from the object above. Use your existing knowledge of these types to understand them in source code, then import them and use them as needed. 
+Extremely common types, such as those from python's builtin module or the typing module, are intentionally excluded from the object above. Use your existing knowledge of these types to understand them, then import them and use them as needed. 
 
-In your code, provide docstrings, comments, and type hints that an experienced programmer would find helpful, and use comments to note any assumptions that might not be clear from the code. If you would like to raise an exception, wrap it in GeneratedException.
+In your code, provide type hints that an experienced programmer would find helpful. Use docstrings and comments when helpful. If you would like to raise an exception, wrap it in InferredException.
 
-Respond with the completed version of the python file, delimited by triple-backticks and using a python identifier.
+Respond with only the completed version of the python file, delimited by triple-backticks and using a python identifier. Additional information will be ignored.
 
 Example incomplete file:
 ```python
 from typing import List
 
 def get_even_numbers(numbers: List[int]) -> List[int]:
 ```
```

### Comparing `codespeak-0.1.2/codespeak/_core/results_collector.py` & `codespeak-0.1.3/codespeak/inference/results_collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # run.py
 import importlib
 import inspect
 import time
 from typing import Callable, List
 from pydantic import BaseModel
-from codespeak._helpers.set_attr_for_qualname import set_attr_for_qualname
+from codespeak.helpers.set_attr_for_qualname import set_attr_for_qualname
 import pytest
 
 
 class ResultsCollector:
     def __init__(self):
         self.reports = []
         self.collected = 0
```

### Comparing `codespeak-0.1.2/codespeak/_declaration/declaration_file_service.py` & `codespeak-0.1.3/codespeak/function/function_file_service.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,36 +2,37 @@
 import inspect
 import json
 import os
 from types import ModuleType
 from typing import Any, Callable
 from pydantic import BaseModel
 
-from codespeak._settings import _settings
-from codespeak._metadata import FunctionMetadata
-from codespeak._metadata.digest import DeclarationDigest
+from codespeak.settings import _settings
+from codespeak.function.function_metadata import FunctionMetadata
+from codespeak.function.function_digest import FunctionDigest
+from codespeak.constants import metadata_file_prefix, codegen_dirname
+from codespeak.helpers.derive_module_qualname_for_object import (
+    derive_module_qualname_for_object,
+)
 
-codegen_dirname = "codespeak_generated"
-metadata_file_prefix = "_metadata_"
 
-
-class DeclarationFileService(BaseModel):
+class FunctionFileService(BaseModel):
     declaration_filesystem_name: str
     generated_module_qualname: str
     codegen_absolute_dirpath: str
     generated_entrypoint: str
 
     def write_metadata(
         self,
         source_code: str,
         require_execution: bool,
         did_execute: bool,
         has_tests: bool,
         did_pass_tests: bool,
-        digest: DeclarationDigest,
+        digest: FunctionDigest,
     ):
         if not os.path.exists(self.codegen_metadata_dirpath):
             os.makedirs(self.codegen_metadata_dirpath)
 
         metadata = FunctionMetadata(
             declaration_digest=digest,
             declaration_source=source_code,
@@ -63,102 +64,69 @@
     @property
     def codegen_metadata_filepath(self) -> str:
         return f"{self.codegen_metadata_dirpath}/{metadata_file_prefix}{self.declaration_filesystem_name}.json"
 
     @staticmethod
     def gather_generated_module_qualname(decorated_func: Callable) -> str:
         module = inspect.getmodule(decorated_func)
-        if not module:
+        if module is None:
             raise Exception("module not found for func: ", decorated_func.__name__)
-        declared_module_qualname = get_declared_module_qualname(decorated_func)
+        declared_module_qualname = derive_module_qualname_for_object(decorated_func)
         return build_generated_module_qualname(
             declared_module_qualname=declared_module_qualname,
-            func_qualname=decorated_func.__qualname__,
+            inferred_func_qualname=decorated_func.__qualname__,
         )
 
     @staticmethod
-    def from_callable(func: Callable) -> "DeclarationFileService":
+    def from_decorated_func(func: Callable) -> "FunctionFileService":
         module = inspect.getmodule(func)
-        if not module:
+        if module is None:
             raise Exception("module not found for func: ", func.__name__)
-        abspath_to_proj = _settings.get_abspath_to_project_root(func)
-        declared_module_qualname = get_declared_module_qualname(func)
+        abspath_to_proj = _settings.get_abspath_to_project_root()
+        declared_module_qualname = derive_module_qualname_for_object(func)
         declared_module_as_filepath = declared_module_qualname.replace(".", "/")
-        return DeclarationFileService(
-            declaration_filesystem_name=func_qualname_to_filesystem_name(
+        return FunctionFileService(
+            declaration_filesystem_name=inferred_func_qualname_to_filesystem_name(
                 func.__qualname__
             ),
             generated_entrypoint=func.__name__,
             generated_module_qualname=build_generated_module_qualname(
                 declared_module_qualname=declared_module_qualname,
-                func_qualname=func.__qualname__,
+                inferred_func_qualname=func.__qualname__,
             ),
             codegen_absolute_dirpath=f"{abspath_to_proj}/{codegen_dirname}/{declared_module_as_filepath}",
         )
 
-    def does_metadata_exist(self) -> bool:
+    def does_previous_inference_exist(self) -> bool:
         return os.path.exists(self.codegen_logic_filepath) and os.path.exists(
             self.codegen_metadata_filepath
         )
 
+    def does_logic_exist(self) -> bool:
+        return os.path.exists(self.codegen_logic_filepath)
+
     def load_metadata(self) -> FunctionMetadata | None:
         if not os.path.exists(self.codegen_metadata_filepath):
             return None
-        with open(self.codegen_metadata_filepath, "r") as file:
-            data = json.load(file)
-        return FunctionMetadata.parse_obj(data)
+        try:
+            with open(self.codegen_metadata_filepath, "r") as file:
+                data = json.load(file)
+            return FunctionMetadata.parse_obj(data)
+        except Exception as e:
+            print("unable to load metadata")
+            return None
 
     def load_logic(self) -> str:
         with open(self.codegen_logic_filepath, "r") as file:
             return file.read()
 
 
 # this func assumes generated directory is in project root
 # could also add flexibity here to configure this in a toml, later
-def build_generated_module_qualname(declared_module_qualname: str, func_qualname: str):
-    return f"{codegen_dirname}.{declared_module_qualname}.{func_qualname_to_filesystem_name(func_qualname)}"
-
-
-def func_qualname_to_filesystem_name(qualname: str) -> str:
-    return qualname.replace(".", "___")
-
-
-def derive_generated_module_qualname_from_func(func: Callable) -> str:
-    declared_mod_qualname = get_declared_module_qualname(func)
-    return build_generated_module_qualname(declared_mod_qualname, func.__qualname__)
-
-
-# want to leave this as an attribute on the wrapper, just want to get rid of abspath to root
-def get_declared_module_qualname(func: Callable):
-    source_file = inspect.getsourcefile(func)
-    if not source_file:
-        raise Exception("unable to get source file for func: ", func.__name__)
-    return derive_declared_module_qualname_from_filepaths(
-        source_file, _settings.get_abspath_to_project_root(func)
-    )
-
-
-def derive_declared_module_qualname_from_filepaths(
-    declaration_filepath: str, project_root: str
+def build_generated_module_qualname(
+    declared_module_qualname: str, inferred_func_qualname: str
 ):
-    # Make sure both paths are absolute and normalized
-    filepath = os.path.normpath(os.path.abspath(declaration_filepath))
-    project_root = os.path.normpath(os.path.abspath(project_root))
-
-    # Check if the filepath is in the project_root
-    if not filepath.startswith(project_root):
-        raise ValueError("The filepath must be inside the project root")
-
-    # Get the relative path from project_root to filepath
-    rel_path = os.path.relpath(filepath, project_root)
+    return f"{codegen_dirname}.{declared_module_qualname}.{inferred_func_qualname_to_filesystem_name(inferred_func_qualname)}"
 
-    # Remove the '.py' extension
-    module_qualname = os.path.splitext(rel_path)[0]
 
-    # Replace path separators with dots
-    module_qualname = module_qualname.replace(os.sep, ".")
-
-    # If the function is in '__init__', use the parent directory as the module
-    if module_qualname.endswith(".__init__"):
-        module_qualname = module_qualname[: -len(".__init__")]
-
-    return module_qualname
+def inferred_func_qualname_to_filesystem_name(qualname: str) -> str:
+    return qualname.replace(".", "___")
```

### Comparing `codespeak-0.1.2/codespeak/_decorate.py` & `codespeak-0.1.3/codespeak/decorate/infer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,86 +1,82 @@
-from typing import Any, Callable
-
-from pydantic import BaseModel
-from codespeak._core.codespeak_service import CodespeakService
-from codespeak._declaration.codespeak_declaration import CodespeakDeclaration
+import inspect
+from typing import Any, Callable, Dict, List, Tuple, TypeVar
 from functools import wraps
-from codespeak._core import diff, executor
-from codespeak._core.code_generator import CodeGenerator
-from codespeak._declaration.declaration_file_service import (
-    DeclarationFileService,
+from codespeak import executor
+from codespeak.function.function_file_service import (
+    FunctionFileService,
+)
+from codespeak.function.function_declaration import (
+    FunctionDeclaration,
+)
+from codespeak.helpers.guarantee_abspath_to_root_exists import (
+    guarantee_abspath_to_project_root_exists,
 )
-from codespeak._helpers.self_type import self_type_if_exists
-from codespeak._core.code_generator import TestFunc
-from codespeak._settings import _settings
-from codespeak._clean import clean
-from codespeak._settings.environment import Environment
+from codespeak.settings import _settings
+from codespeak.settings.environment import Environment
+from codespeak.function import Function
+from codespeak.function.function_attributes import FunctionAttributes
+from codespeak.frame_tests import FrameTests
+from codespeak.frame import Frame
+from codespeak.helpers.get_definitions_from_function_signature import (
+    get_definitions_from_function_signature,
+)
+
+# type inference remain on original function when no type hints are on the decorator
 
 
-def codespeak(func):
+def infer(func):
     @wraps(func)
-    def dev_execute(*args, **kwargs):
-        if not hasattr(codespeak_function, "file_service"):
-            raise Exception("file service not found")
-        file_service = codespeak_function.file_service
-        self_type = self_type_if_exists(func, list(args), kwargs)
-        declaration = CodespeakDeclaration.from_callable(func, self_type, file_service)
-        should_generate_new_source_code = diff.require_new_codegen(
-            file_service, declaration.digest
-        )
-        pytest_func: TestFunc | None = getattr(codespeak_function, "pytest_func", None)
-        if should_generate_new_source_code:
-            code_generator = CodeGenerator(
-                declaration=declaration,
-                service=CodespeakService.with_defaults(declaration),
-                should_execute=True,
-                test_func=pytest_func,
-                args=list(args),
-                kwargs=kwargs,
-            )
-            generation = code_generator.generate()
-            if _settings.should_auto_clean():
-                clean(_settings.abspath_to_codegen_dir())
-            return generation.execution_result
+    def wrapper(*args, **kwargs):
+        if wrapper._is_prod:  # type: ignore
+            return wrapper._logic(*args, **kwargs)  # type: ignore
         else:
-            return executor.execute_with_attributes(
-                file_service.generated_module_qualname,
-                file_service.generated_entrypoint,
-                *args,
-                **kwargs,
-            )
-
-    class _CodespeakFunction:
-        file_service: DeclarationFileService
-        pytest_func: TestFunc
-        is_prod: bool
-        logic: Callable
-
-        def __call__(self, *args, **kwargs):
-            if self.is_prod:
-                return self.logic(*args, **kwargs)
-            else:
-                return dev_execute(*args, **kwargs)
-
-        def assign_pytest_function(self, _pytest_func: Callable):
-            self.pytest_func = TestFunc.from_callable(_pytest_func)
-
-    codespeak_function = _CodespeakFunction()
-    assign_default_attributes(codespeak_function, func)
-    return codespeak_function
+            nonlocal has_executed
+            function = Function(wrapper)
+            if not has_executed:
+                with Frame.get_manager().manage_for(wrapper):
+                    func(*args, **kwargs)
+                function._try_add_self_to_frame(args, kwargs)
+                has_executed = True
+            if function._is_testing:
+                return function.execute_latest_inference(*args, **kwargs)
+            return function._infer(args, kwargs)
+
+    has_executed = False
+    _assign_default_attributes(wrapper, func)
+    return wrapper
 
 
-def assign_default_attributes(codespeak_function: Callable, decorated_func: Callable):
+def _assign_default_attributes(wrapper: Callable, decorated_func: Callable):
     env = _settings.get_environment()
-    codespeak_function.is_prod = env == Environment.PROD
+    setattr(wrapper, FunctionAttributes.is_prod, env == Environment.PROD)
+    guarantee_abspath_to_project_root_exists(decorated_func)
     if env == _settings.Environment.PROD:
         logic = executor.load_generated_logic_from_module_qualname(
-            DeclarationFileService.gather_generated_module_qualname(
+            FunctionFileService.gather_generated_module_qualname(
                 decorated_func=decorated_func
             ),
             decorated_func.__name__,
         )
-        codespeak_function.logic = logic
+        setattr(wrapper, FunctionAttributes.logic, logic)
     elif env == _settings.Environment.DEV:
-        codespeak_function.file_service = DeclarationFileService.from_callable(
-            decorated_func
+        file_service = FunctionFileService.from_decorated_func(decorated_func)
+        setattr(wrapper, FunctionAttributes.file_service, file_service)
+        signature_definitions = get_definitions_from_function_signature(
+            inspect.signature(decorated_func)
+        )
+        setattr(
+            wrapper,
+            FunctionAttributes.declaration,
+            FunctionDeclaration.from_inferred_func(
+                decorated_func, signature_definitions
+            ),
+        )
+        setattr(
+            wrapper,
+            FunctionAttributes.frame,
+            Frame(
+                type_definitions=signature_definitions,
+                tests=FrameTests(),
+                parents=[Frame.for_module(decorated_func.__module__)],
+            ),
         )
```

### Comparing `codespeak-0.1.2/codespeak/_definitions/classify.py` & `codespeak-0.1.3/codespeak/type_definitions/classify.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import types
 from typing import Any, Callable, Dict, Tuple, get_origin
-import builtins
 from typing import Any, Union, get_args, get_origin, List, get_type_hints
 import inspect
-from codespeak._definitions.free_modules import FREE_MODULES
+from codespeak.type_definitions.free_modules import FREE_MODULES
 import os
 import types
-from codespeak._definitions.definition import Definition
-from codespeak._definitions.types.generic import Generic
-from codespeak._definitions.types.local_class import LocalClass
-from codespeak._definitions.types.local_class_as_self import LocalClassAsSelf
-from codespeak._definitions.types.installed_class import InstalledClass
-from codespeak._definitions.types.builtin import Builtin
-from codespeak._definitions.types.none import NoneDef
-from codespeak._definitions.types.typing_type import TypingType
-from codespeak._definitions.types.union_type import UnionType
+from codespeak.type_definitions.type_definition import TypeDefinition
+from codespeak.type_definitions.types.local_class import LocalClass
+from codespeak.type_definitions.types.local_class_as_self import LocalClassAsSelf
+from codespeak.helpers.derive_module_qualname_for_object import (
+    derive_module_qualname_for_object,
+)
+from codespeak.type_definitions.types.installed_class import InstalledClass
+from codespeak.type_definitions.types.builtin import Builtin
+from codespeak.type_definitions.types.none import NoneDef
+from codespeak.type_definitions.types.typing_type import TypingType
+from codespeak.type_definitions.types.union_type import UnionType
 import pkg_resources
 
 
 def to_union_type(definition: Any) -> UnionType:
     args = get_args(definition)
     _types = []
     for _type in args:
@@ -41,19 +42,17 @@
 def is_local_class(definition: type) -> bool:
     module = inspect.getmodule(definition)
     if not module:
         raise Exception(
             "no module found for type, expected one, possibly undefined behavior: ",
             definition,
         )
-    is_installed = is_installed_package_type(module.__name__)
-    if is_installed:
+    if is_installed_package_type(module.__name__):
         return False
-    is_builtin = is_builtin_type(module.__name__)
-    if is_builtin:
+    if is_builtin_type(module.__name__):
         return False
     # optimistically assumes that if it's not installed and not builtin, it's local
     return True
 
 
 def to_typing_type(definition: Any) -> TypingType:
     args = get_args(definition)
@@ -77,25 +76,25 @@
         "set": True,
         "tuple": True,
     }
     if qualname in builtins_with_args:
         return True
 
 
-def from_any_list(_list: List[Any]) -> List[Definition]:
+def from_any_list(_list: List[Any]) -> List[TypeDefinition]:
     return [from_any(_def) for _def in _list]
 
 
-def from_any_tuple(tup: Tuple[Any]) -> List[Definition]:
+def from_any_tuple(tup: Tuple[Any]) -> List[TypeDefinition]:
     return [from_any(_def) for _def in tup]
 
 
 def from_any(
     definition: Any,
-) -> Definition:
+) -> TypeDefinition:
     if definition is None:
         return NoneDef()
     if not hasattr(definition, "__module__"):
         raise Exception("expected a module on the type")
     if get_origin(definition) is types.UnionType:
         return to_union_type(definition)
     # types.UnionType has no qualname attr
@@ -112,15 +111,17 @@
                 qualname=definition.__qualname__,
                 _def=definition,
             )
     elif inspect.isclass(definition):
         if is_local_class(definition):
             return LocalClass(
                 qualname=definition.__qualname__,
-                module=definition.__module__,
+                module=derive_module_qualname_for_object(
+                    definition
+                ),  # definition.__module__,
                 source_code=inspect.getsource(definition),
                 bases=from_any_tuple(definition.__bases__),
                 type_hints=collect_type_hints(definition),
                 _def=definition,
             )
         else:
             return InstalledClass(
@@ -136,16 +137,16 @@
             "no support for functions right now, can't cast definition: ",
             definition,
         )
     else:
         raise Exception("unsure how to handle definition: ", definition)
 
 
-def from_self_class_obj(self_class_obj: Any, method_name: str) -> Definition:
-    _def = from_any(self_class_obj)
+def from_self_class(self_class: Any, method_name: str) -> TypeDefinition:
+    _def = from_any(self_class)
     if _def.type == "LocalClass":
         return LocalClassAsSelf(
             qualname=_def.qualname,
             module=_def.module,
             source_code=_def.source_code,
             bases=_def.bases,
             type_hints=_def.type_hints,
@@ -153,17 +154,14 @@
             method_name=method_name,
         )
     else:
         return _def
 
 
 # technically get_type_hints can work on some installed types but we aren't using it for that atm
-def collect_type_hints(_class: type) -> Dict[str, Definition]:
+def collect_type_hints(_class: type) -> Dict[str, TypeDefinition]:
     hints = get_type_hints(_class, include_extras=False)
     definitions = {}
     for name, _def in hints.items():
         typed_def = from_any(_def)
         definitions[name] = typed_def
     return definitions
-
-
-# so get_type_hints works for reg classes as long as the instance vars are an_assigned. so it would bundle class vars and instance vars together
```

### Comparing `codespeak-0.1.2/codespeak/_definitions/definition.py` & `codespeak-0.1.3/codespeak/type_definitions/type_definition.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,39 +2,51 @@
 from typing import Any, Dict, List
 
 from pydantic import BaseModel
 from abc import ABC, abstractmethod
 from typing import Literal
 
 
-# needs to go above below imports
-class Definition(ABC, BaseModel):
+class TypeDefinition(ABC, BaseModel):
     qualname: str
     module: str
-    type: Literal["Definition"] = "Definition"
+    type: Literal["TypeDefinition"] = "TypeDefinition"
     _def: Any
 
+    def __hash__(self):
+        return hash((self.module, self.qualname))
+
+    def __eq__(self, other):
+        if isinstance(other, TypeDefinition):
+            return (self.module, self.qualname) == (other.module, other.qualname)
+        return False
+
+    def __lt__(self, other):
+        if isinstance(other, TypeDefinition):
+            return self.import_path() < other.import_path()
+        return NotImplemented
+
     def printable(self) -> str:
         return json.dumps(self.annotate(), indent=4)
 
     @abstractmethod
     def annotate(self) -> Dict:
         pass
 
-    def ref_nested_locals(self) -> List["Definition"]:
+    def ref_nested_locals(self) -> List["TypeDefinition"]:
         return []
 
-    def flatten(self) -> List["Definition"]:
+    def flatten(self) -> List["TypeDefinition"]:
         return [self]
 
     def annotate_in_local_class(self) -> Dict | str:
         return self.annotate()
 
-    def import_path(self):
+    def import_path(self) -> str:
         return self.module + "." + self.qualname
 
     @abstractmethod
     def custom_types(self) -> Dict:
         pass
 
-    def reference_nested_custom_types(self) -> List["Definition"]:
+    def reference_nested_custom_types(self) -> List["TypeDefinition"]:
         return []
```

### Comparing `codespeak-0.1.2/codespeak/_definitions/free_modules.py` & `codespeak-0.1.3/codespeak/type_definitions/free_modules.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.2/codespeak/_definitions/types/custom_type_reference.py` & `codespeak-0.1.3/codespeak/type_definitions/types/custom_type_reference.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, Literal
-from codespeak._definitions.definition import Definition
+from codespeak.type_definitions.type_definition import TypeDefinition
 
 
-class CustomTypeReference(Definition):
+class CustomTypeReference(TypeDefinition):
     type: Literal["ComplexTypeReference"] = "ComplexTypeReference"
 
     def ref(self):
         return "$ref: complex_types/" + self.module + "." + self.qualname
 
     def annotate(self) -> Dict:
         return {
```

### Comparing `codespeak-0.1.2/codespeak/_definitions/types/installed_class.py` & `codespeak-0.1.3/codespeak/type_definitions/types/installed_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Callable, Dict
 from typing import Literal
-from codespeak._definitions.definition import Definition
+from codespeak.type_definitions.type_definition import TypeDefinition
 
 
-class InstalledClass(Definition):
+class InstalledClass(TypeDefinition):
     type: Literal["InstalledClass"] = "InstalledClass"
     origin: str = "installed"
 
     def annotate(self) -> Dict:
         return {
             f"{self.import_path()}": {
                 "origin": "installed",
```

### Comparing `codespeak-0.1.2/codespeak/_definitions/types/local_class.py` & `codespeak-0.1.3/codespeak/type_definitions/types/local_class.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 from typing import Any, Callable, Dict, List, Tuple
 
 from typing import Literal
-from codespeak._definitions.definition import Definition
-from codespeak._definitions.types.custom_type_reference import CustomTypeReference
-from codespeak._definitions.utils.dedupe import dedupe
-from codespeak._definitions.utils.flat_uniques import flat_uniques
-from codespeak._definitions.utils.flatten import flatten_definitions
-import ast
+from codespeak.type_definitions.type_definition import TypeDefinition
+from codespeak.type_definitions.types.custom_type_reference import CustomTypeReference
 
 
-class LocalClass(Definition):
+class LocalClass(TypeDefinition):
     type: Literal["LocalClass"] = "LocalClass"
     source_code: str
-    bases: List[Definition]
-    type_hints: Dict[str, Definition]
+    bases: List[TypeDefinition]
+    type_hints: Dict[str, TypeDefinition]
     origin: str = "local"
     _def: Any
 
-    def reference_nested_custom_types(self) -> List[Definition]:
+    def reference_nested_custom_types(self) -> List[TypeDefinition]:
         referenced = []
         for type_name, _def in self.type_hints.items():
             if _def.type == "LocalClass":
                 self.type_hints[type_name] = CustomTypeReference(
                     qualname=_def.qualname, module=_def.module, _def=_def
                 )
                 referenced.append(_def)
@@ -39,23 +35,23 @@
             elif _def.type == "InstalledClass":
                 self.bases[i] = CustomTypeReference(
                     qualname=_def.qualname, module=_def.module, _def=_def
                 )
                 referenced.append(_def)
         return referenced
 
-    def collect_referenced_types(self) -> List[Definition]:
+    def collect_referenced_types(self) -> List[TypeDefinition]:
         referenced = self.reference_nested_custom_types()
         for _, _def in self.type_hints.items():
             referenced.extend(_def.reference_nested_custom_types())
         for _def in self.bases:
             referenced.extend(_def.reference_nested_custom_types())
         return referenced
 
-    def flatten(self) -> List[Definition]:
+    def flatten(self) -> List[TypeDefinition]:
         return [self]
 
     def custom_types(self) -> Dict:
         types_replaced = self.collect_referenced_types()
         annotxn = self.annotate()
         for _type in types_replaced:
             annotxn.update(_type.custom_types())
```

### Comparing `codespeak-0.1.2/codespeak/_definitions/types/local_class_as_self.py` & `codespeak-0.1.3/codespeak/type_definitions/types/local_class_as_self.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import ast
 from typing import Dict
-from codespeak._definitions.types.local_class import LocalClass
+from codespeak.type_definitions.types.local_class import LocalClass
 
 
 class RemoveFunction(ast.NodeTransformer):
     def __init__(self, function_name):
         self.function_name = function_name
 
     def visit_FunctionDef(self, node):
```

### Comparing `codespeak-0.1.2/codespeak/_definitions/types/typing_type.py` & `codespeak-0.1.3/codespeak/type_definitions/types/typing_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import json
 from typing import Any, Dict, List, Tuple
 
 from typing import Literal
-from codespeak._definitions.types.generic import Generic
-from codespeak._definitions.utils.flat_uniques import flat_uniques
-from codespeak._definitions.definition import Definition
-from codespeak._definitions.utils.swap_custom_types import (
+from codespeak.type_definitions.types.generic import Generic
+from codespeak.type_definitions.type_definition import TypeDefinition
+from codespeak.type_definitions.utils.swap_custom_types import (
     recursively_swap_custom_types_for_references,
 )
 
 
-class TypingType(Definition):
+class TypingType(TypeDefinition):
     qualname: str
     module: str
     # could be dict, union, list, some others but not sure all of them
     origin: Any | None
-    args: List[Definition]
+    args: List[TypeDefinition]
     type: Literal["TypingType"] = "TypingType"
 
-    def flatten(self) -> List[Definition]:
-        flat: List[Definition] = [
+    def flatten(self) -> List[TypeDefinition]:
+        flat: List[TypeDefinition] = [
             Generic(qualname=self.qualname, module=self.module, _def=None)
         ]
         for arg in self.args:
             flat.extend(arg.flatten())
         return flat
 
     def annotate(self) -> Dict:
@@ -42,15 +41,15 @@
         else:
             return {
                 f"{self.module}.{self.qualname}": [
                     arg.annotate_in_local_class() for arg in self.args
                 ]
             }
 
-    def reference_nested_custom_types(self) -> List[Definition]:
+    def reference_nested_custom_types(self) -> List[TypeDefinition]:
         args = self.args
         types_replaced, self.args = recursively_swap_custom_types_for_references(args)
         return types_replaced
 
     def custom_types(self) -> Dict:
         types_replaced = self.reference_nested_custom_types()
         annotxn = {}
```

### Comparing `codespeak-0.1.2/codespeak/_definitions/types/union_type.py` & `codespeak-0.1.3/codespeak/type_definitions/types/union_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Callable, Dict, List
 from typing import Literal
 
-from codespeak._definitions.types.typing_type import TypingType
-from codespeak._definitions.definition import Definition
+from codespeak.type_definitions.types.typing_type import TypingType
+from codespeak.type_definitions.type_definition import TypeDefinition
 
 
 class UnionType(TypingType):
     qualname: str = "UnionType"
     module: str = "types"
-    args: List[Definition]
+    args: List[TypeDefinition]
     type: Literal["UnionType"] = "UnionType"
 
     def annotate(self) -> Dict:
         return {
             f"{self.import_path()}": {
                 "qualname": self.qualname,
                 "module": self.module,
```

### Comparing `codespeak-0.1.2/codespeak/_definitions/utils/swap_custom_types.py` & `codespeak-0.1.3/codespeak/type_definitions/utils/swap_custom_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import List, Tuple
 
-from codespeak._definitions.definition import Definition
-from codespeak._definitions.types.custom_type_reference import CustomTypeReference
+from codespeak.type_definitions.type_definition import TypeDefinition
+from codespeak.type_definitions.types.custom_type_reference import CustomTypeReference
 
 
 def recursively_swap_custom_types_for_references(
-    args: List[Definition],
-) -> Tuple[List[Definition], List[Definition]]:
+    args: List[TypeDefinition],
+) -> Tuple[List[TypeDefinition], List[TypeDefinition]]:
     swapped = []
     for i, _def in enumerate(args):
         if _def.type == "TypingType" or _def.type == "UnionType":
             if hasattr(_def, "args") and _def.args is not None:
                 _swapped, _args = recursively_swap_custom_types_for_references(
                     _def.args
                 )
```

### Comparing `codespeak-0.1.2/codespeak/_helpers/self_type.py` & `codespeak-0.1.3/codespeak/helpers/self_type.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
-from typing import Any, Callable, Dict, List
-from codespeak._helpers.gather_arguments import gather_arguments
+from typing import Any, Callable, Dict, Tuple
+from codespeak.helpers.gather_arguments import gather_arguments
 
 
 def self_type_if_exists(
-    func: Callable, args: List[Any], kwargs: Dict[str, Any]
+    func: Callable, args: Tuple[Any], kwargs: Dict[str, Any]
 ) -> Any | None:
     bounded_args = gather_arguments(func, args, kwargs)
     for index, arg in enumerate(bounded_args):
         if index == 0:
             _type = type(arg.value)
             if arg.name == "self" and inspect.isclass(_type):
                 return _type
```

### Comparing `codespeak-0.1.2/codespeak/_settings/_settings.py` & `codespeak-0.1.3/codespeak/settings/_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from enum import Enum
 import os
 from typing import Callable
 from pydantic import BaseModel
-from codespeak._helpers.auto_detect_abspath_to_project_root import (
-    auto_detect_abspath_to_project_root,
-)
-from codespeak._declaration.declaration_file_service import codegen_dirname
-from codespeak._settings.environment import Environment
+from codespeak.settings.environment import Environment
+from codespeak.constants import codegen_dirname
 
 
 class _Settings(BaseModel):
     """
     Internal representation of settings for codespeak.
 
     - all borrowed from codespeak_Settings.ConfigOptions, except for abspath_to_project_root
@@ -19,20 +16,22 @@
     """
 
     openai_api_key: str | None = None
     environment: Environment
     verbose: bool = False
     abspath_to_project_root: str | None = None
     openai_model: str = "gpt-4"
-    auto_clean: bool = True
+    should_auto_clean: bool = False
+    is_testing: bool = False
+    filepath_for_logic_being_tested: str = ""
 
     @staticmethod
     def from_env():
         env = os.getenv("ENVIRONMENT")
-        if env:
+        if env is not None:
             env = env.lower()
             if env in [e.value for e in Environment]:
                 return _Settings(
                     openai_api_key=os.getenv("OPENAI_API_KEY"),
                     environment=Environment(env),
                 )
         return _Settings(
@@ -44,32 +43,40 @@
 
 
 def abspath_to_codegen_dir() -> str:
     return f"{_settings.abspath_to_project_root}/{codegen_dirname}"
 
 
 def should_auto_clean() -> bool:
-    return _settings.auto_clean
+    return _settings.should_auto_clean
 
 
 def get_openai_model() -> str:
     return _settings.openai_model
 
 
-def get_abspath_to_project_root(decorated_func: Callable) -> str:
+def set_abspath_to_project_root(abspath: str):
+    _settings.abspath_to_project_root = abspath
+
+
+def get_abspath_to_project_root() -> str:
     if _settings.abspath_to_project_root is None:
-        _settings.abspath_to_project_root = auto_detect_abspath_to_project_root(
-            decorated_func
-        )
+        raise Exception("abspath_to_project_root is None")
     return _settings.abspath_to_project_root
 
 
 def get_openai_api_key() -> str | None:
     return _settings.openai_api_key
 
 
 def get_verbose() -> bool:
     return _settings.verbose
 
 
 def get_environment() -> Environment:
     return _settings.environment
+
+
+def set_is_testing(is_testing: bool, logic_at_filepath: str | None = None):
+    _settings.is_testing = is_testing
+    if logic_at_filepath is not None:
+        _settings.filepath_for_logic_being_tested = logic_at_filepath
```

### Comparing `codespeak-0.1.2/codespeak/public/codespeak_settings.py` & `codespeak-0.1.3/codespeak/public/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pydantic import BaseModel
-from codespeak._settings.environment import Environment
-from codespeak._settings._settings import _settings
+from codespeak.settings.environment import Environment
+from codespeak.settings._settings import _settings
 
 
 def set_openai_api_key(key: str):
     _settings.openai_api_key = key
 
 
 def set_verbose(verbose: bool):
```

