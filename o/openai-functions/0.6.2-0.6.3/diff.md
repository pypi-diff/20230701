# Comparing `tmp/openai_functions-0.6.2.tar.gz` & `tmp/openai_functions-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functions-0.6.2.tar", max compression
+gzip compressed data, was "openai_functions-0.6.3.tar", max compression
```

## Comparing `openai_functions-0.6.2.tar` & `openai_functions-0.6.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1065 2023-06-27 20:39:30.589058 openai_functions-0.6.2/LICENSE
--rw-r--r--   0        0        0     3175 2023-06-27 20:41:53.967269 openai_functions-0.6.2/README.md
--rw-r--r--   0        0        0      561 2023-06-24 01:49:09.012365 openai_functions-0.6.2/openai_functions/__init__.py
--rw-r--r--   0        0        0    10879 2023-06-25 06:45:03.861226 openai_functions-0.6.2/openai_functions/conversation.py
--rw-r--r--   0        0        0      371 2023-06-23 23:16:40.645247 openai_functions-0.6.2/openai_functions/functions/__init__.py
--rw-r--r--   0        0        0     2936 2023-06-23 23:39:48.076531 openai_functions-0.6.2/openai_functions/functions/basic_set.py
--rw-r--r--   0        0        0      356 2023-06-24 01:56:28.673664 openai_functions-0.6.2/openai_functions/functions/exceptions.py
--rw-r--r--   0        0        0     2478 2023-06-24 01:57:02.009995 openai_functions-0.6.2/openai_functions/functions/functions.py
--rw-r--r--   0        0        0     4210 2023-06-24 01:50:27.961125 openai_functions-0.6.2/openai_functions/functions/sets.py
--rw-r--r--   0        0        0     1678 2023-06-23 23:33:22.081874 openai_functions-0.6.2/openai_functions/functions/union.py
--rw-r--r--   0        0        0     6327 2023-06-24 01:44:38.621801 openai_functions-0.6.2/openai_functions/functions/wrapper.py
--rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.6.2/openai_functions/json_type.py
--rw-r--r--   0        0        0     5327 2023-06-27 20:08:21.746819 openai_functions-0.6.2/openai_functions/nlp.py
--rw-r--r--   0        0        0     7508 2023-06-25 06:45:07.662263 openai_functions-0.6.2/openai_functions/openai_types.py
--rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.6.2/openai_functions/parsers/__init__.py
--rw-r--r--   0        0        0     1668 2023-06-23 18:20:13.721023 openai_functions-0.6.2/openai_functions/parsers/abc.py
--rw-r--r--   0        0        0      975 2023-06-24 00:28:00.470995 openai_functions-0.6.2/openai_functions/parsers/atomic_type_parser.py
--rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.6.2/openai_functions/parsers/bool_parser.py
--rw-r--r--   0        0        0     1641 2023-06-24 00:45:19.947754 openai_functions-0.6.2/openai_functions/parsers/dataclass_parser.py
--rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.6.2/openai_functions/parsers/default.py
--rw-r--r--   0        0        0     1194 2023-06-23 18:21:17.923529 openai_functions-0.6.2/openai_functions/parsers/dict_parser.py
--rw-r--r--   0        0        0     1067 2023-06-23 18:21:23.392642 openai_functions-0.6.2/openai_functions/parsers/enum_parser.py
--rw-r--r--   0        0        0      520 2023-06-24 01:52:09.574112 openai_functions-0.6.2/openai_functions/parsers/float_parser.py
--rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.6.2/openai_functions/parsers/int_parser.py
--rw-r--r--   0        0        0      993 2023-06-23 18:21:35.574892 openai_functions-0.6.2/openai_functions/parsers/list_parser.py
--rw-r--r--   0        0        0      691 2023-06-23 18:21:54.432274 openai_functions-0.6.2/openai_functions/parsers/none_parser.py
--rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.6.2/openai_functions/parsers/str_parser.py
--rw-r--r--   0        0        0     1273 2023-06-23 18:22:28.365942 openai_functions-0.6.2/openai_functions/parsers/union_parser.py
--rw-r--r--   0        0        0        0 2023-06-23 18:45:36.035799 openai_functions-0.6.2/openai_functions/py.typed
--rw-r--r--   0        0        0      623 2023-06-27 20:42:11.689171 openai_functions-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     3891 1970-01-01 00:00:00.000000 openai_functions-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-27 20:52:53.295744 openai_functions-0.6.3/LICENSE
+-rw-r--r--   0        0        0     4271 2023-07-01 17:19:47.350298 openai_functions-0.6.3/README.md
+-rw-r--r--   0        0        0      987 2023-07-01 15:53:29.387048 openai_functions-0.6.3/openai_functions/__init__.py
+-rw-r--r--   0        0        0    12149 2023-07-01 15:53:52.642235 openai_functions-0.6.3/openai_functions/conversation.py
+-rw-r--r--   0        0        0      613 2023-07-01 15:28:12.336941 openai_functions-0.6.3/openai_functions/functions/__init__.py
+-rw-r--r--   0        0        0     3448 2023-07-01 15:32:10.388033 openai_functions-0.6.3/openai_functions/functions/basic_set.py
+-rw-r--r--   0        0        0      378 2023-07-01 15:56:30.128412 openai_functions-0.6.3/openai_functions/functions/exceptions.py
+-rw-r--r--   0        0        0     2625 2023-07-01 16:03:49.607132 openai_functions-0.6.3/openai_functions/functions/functions.py
+-rw-r--r--   0        0        0     4389 2023-07-01 15:57:49.401955 openai_functions-0.6.3/openai_functions/functions/sets.py
+-rw-r--r--   0        0        0     1678 2023-06-27 20:52:53.296744 openai_functions-0.6.3/openai_functions/functions/union.py
+-rw-r--r--   0        0        0     7500 2023-07-01 16:09:18.414864 openai_functions-0.6.3/openai_functions/functions/wrapper.py
+-rw-r--r--   0        0        0      160 2023-06-27 20:52:53.296744 openai_functions-0.6.3/openai_functions/json_type.py
+-rw-r--r--   0        0        0     5511 2023-07-01 16:09:56.439055 openai_functions-0.6.3/openai_functions/nlp.py
+-rw-r--r--   0        0        0     7790 2023-07-01 16:00:24.507942 openai_functions-0.6.3/openai_functions/openai_types.py
+-rw-r--r--   0        0        0      156 2023-06-27 20:52:53.296744 openai_functions-0.6.3/openai_functions/parsers/__init__.py
+-rw-r--r--   0        0        0     1788 2023-07-01 15:23:08.531382 openai_functions-0.6.3/openai_functions/parsers/abc.py
+-rw-r--r--   0        0        0      975 2023-06-27 20:52:53.296744 openai_functions-0.6.3/openai_functions/parsers/atomic_type_parser.py
+-rw-r--r--   0        0        0      201 2023-06-27 20:52:53.296744 openai_functions-0.6.3/openai_functions/parsers/bool_parser.py
+-rw-r--r--   0        0        0     1641 2023-06-27 20:52:53.296744 openai_functions-0.6.3/openai_functions/parsers/dataclass_parser.py
+-rw-r--r--   0        0        0      760 2023-06-27 20:52:53.296744 openai_functions-0.6.3/openai_functions/parsers/default.py
+-rw-r--r--   0        0        0     1194 2023-06-27 20:52:53.296744 openai_functions-0.6.3/openai_functions/parsers/dict_parser.py
+-rw-r--r--   0        0        0     1067 2023-06-27 20:52:53.296744 openai_functions-0.6.3/openai_functions/parsers/enum_parser.py
+-rw-r--r--   0        0        0      520 2023-06-27 20:52:53.296744 openai_functions-0.6.3/openai_functions/parsers/float_parser.py
+-rw-r--r--   0        0        0      640 2023-06-27 20:52:53.296744 openai_functions-0.6.3/openai_functions/parsers/int_parser.py
+-rw-r--r--   0        0        0      993 2023-06-27 20:52:53.296744 openai_functions-0.6.3/openai_functions/parsers/list_parser.py
+-rw-r--r--   0        0        0      691 2023-06-27 20:52:53.296744 openai_functions-0.6.3/openai_functions/parsers/none_parser.py
+-rw-r--r--   0        0        0      204 2023-06-27 20:52:53.296744 openai_functions-0.6.3/openai_functions/parsers/str_parser.py
+-rw-r--r--   0        0        0     1273 2023-06-27 20:52:53.296744 openai_functions-0.6.3/openai_functions/parsers/union_parser.py
+-rw-r--r--   0        0        0        0 2023-06-27 20:52:53.296744 openai_functions-0.6.3/openai_functions/py.typed
+-rw-r--r--   0        0        0      623 2023-07-01 17:29:36.327849 openai_functions-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     4987 1970-01-01 00:00:00.000000 openai_functions-0.6.3/PKG-INFO
```

### Comparing `openai_functions-0.6.2/LICENSE` & `openai_functions-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.2/openai_functions/conversation.py` & `openai_functions-0.6.3/openai_functions/conversation.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,55 +27,58 @@
         OpenAiFunctionCallInput,
     )
     from .functions.functions import OpenAIFunction
     from .functions.sets import FunctionResult, FunctionSet
 
 
 class Conversation:
-    """A class for running OpenAI functions"""
+    """A class representing a single conversation with the AI
+
+    Contains the messages sent and received, and the skillset used.
+    """
 
     def __init__(
         self,
         skills: list[FunctionSet] | None = None,
         model: str = "gpt-3.5-turbo-0613",
     ) -> None:
         self.messages: list[GenericMessage] = []
         self.skills = UnionSkillSet(*(skills or []))
         self.model = model
 
     @property
-    def functions_schema(self) -> JsonType:
-        """Get the functions schema
+    def functions_schema(self) -> list[JsonType]:
+        """Get the functions schema for the conversation
 
         Returns:
-            JsonType: The functions schema
+            list[JsonType]: The functions schema
         """
         return self.skills.functions_schema
 
     def _add_message(self, message: GenericMessage) -> None:
         """Add a message
 
         Args:
             message (GenericMessage): The message
         """
         self.messages.append(message)
 
     def add_message(self, message: GenericMessage | MessageType | str) -> None:
-        """Add a message
+        """Add a message to the end of the conversation
 
         Args:
             message (GenericMessage | MessageType | str): The message
         """
         if isinstance(message, GenericMessage):
             self._add_message(message)
         else:
             self._add_message(Message(message))
 
     def add_messages(self, messages: list[GenericMessage | MessageType]) -> None:
-        """Add messages
+        """Add multiple messages to the end of the conversation
 
         Args:
             messages (list[GenericMessage | MessageType]): The messages
         """
         for message in messages:
             self.add_message(message)
 
@@ -87,15 +90,15 @@
 
         Returns:
             GenericMessage: The message
         """
         return self.messages.pop(index)
 
     def clear_messages(self) -> None:
-        """Clear the messages"""
+        """Fully clear the messages, but keep the skillset"""
         self.messages = []
 
     @overload
     def _generate_message(
         self, function_call: ForcedFunctionCall
     ) -> IntermediateResponseMessageType:
         ...
@@ -128,63 +131,69 @@
             messages=[message.as_dict() for message in self.messages],
             functions=self.functions_schema,
             function_call=function_call,
         )
         return response["choices"][0]["message"]  # type: ignore
 
     def substitute_last_with_function_result(self, result: str) -> None:
-        """Substitute the last message with the result
+        """Substitute the last message with the result of a function
 
         Args:
             result (str): The function result
         """
         self.pop_message()
         response: NonFunctionMessageType = {
             "role": "assistant",
             "content": result,
         }
         self.add_message(response)
 
     def add_function_result(self, function_result: FunctionResult) -> bool:
-        """Add a function result
+        """Add a function execution result to the chat
 
         Args:
-            function_result (FunctionResult): The function result
+            function_result (FunctionResult): The function execution result
 
         Returns:
             bool: Whether the function result was added
+                (whether save_return was True)
         """
         if function_result.content is None:
             return False
         response: FunctionMessageType = {
             "role": "function",
             "name": function_result.name,
             "content": function_result.content,
         }
         self.add_message(response)
         return True
 
     def add_or_substitute_function_result(
         self, function_result: FunctionResult
     ) -> bool:
-        """Add or substitute a function result
+        """Add or substitute a function execution result
+
+        If the function has interpret_as_response set to True, the last message,
+        which is assumed to be a function call, will be replaced with the function
+        execution result. Otherwise, the function execution result will be added
+        to the chat.
 
         Args:
             function_result (FunctionResult): The function result
 
         Raises:
             TypeError: If the function returns a None value
 
         Returns:
             bool: Whether the function result was added
         """
         if function_result.substitute:
             if function_result.content is None:
                 raise TypeError(
-                    f"Function {function_result.name} returned a None value"
+                    f"Function {function_result.name} did not provide a return"
                 )
             self.substitute_last_with_function_result(function_result.content)
             return True
         return self.add_function_result(function_result)
 
     def run_function_and_substitute(
         self,
@@ -195,22 +204,26 @@
         Args:
             function_call (FunctionCall): The function call
 
         Raises:
             TypeError: If the function returns a None value
 
         Returns:
-            bool: Whether the function result was added
+            bool: Whether the function result was added to the chat
+                (whether save_return was True)
         """
         return self.add_or_substitute_function_result(
             self.skills.run_function(function_call)
         )
 
     def run_function_if_needed(self) -> bool:
-        """Run a function if needed
+        """Run a function if the last message was a function call
+
+        Might run the function over and over again if the function
+        does not save the return.
 
         Returns:
             bool: Whether the function result was added
         """
         if not self.messages:
             return False
 
@@ -219,15 +232,17 @@
             return False
 
         return self.run_function_and_substitute(function_call)
 
     def generate_message(
         self, function_call: OpenAiFunctionCallInput = "auto"
     ) -> GenericMessage:
-        """Generate the next message
+        """Generate the next message. Will run a function if the last message
+        was a function call and the function call is not being overridden;
+        if the function does not save the return a message will still be generated.
 
         Args:
             function_call (OpenAiFunctionCallInput): The function call
 
         Returns:
             GenericMessage: The response
         """
@@ -237,21 +252,22 @@
         message: NonFunctionMessageType = self._generate_message(function_call)
         self.add_message(message)
         return Message(message)
 
     def run_until_response(
         self, allow_function_calls: bool = True
     ) -> FinalResponseMessage:
-        """Run until a response is generated
+        """Run functions query the AI until a response is generated
 
         Args:
-            allow_function_calls (bool): Whether to allow function calls.
+            allow_function_calls (bool): Whether to allow the AI to call functions
 
         Returns:
-            FinalResponseMessage: The response
+            FinalResponseMessage: The final response, either from the AI or a function
+                that has interpret_as_response set to True
         """
         while True:
             message = self.generate_message(
                 function_call="auto" if allow_function_calls else "none"
             )
             if is_final_response_message(message):
                 return message
@@ -288,25 +304,25 @@
         save_return: bool = True,
         serialize: bool = True,
         interpret_as_response: bool = False,
     ) -> (
         Callable[[Callable[..., JsonType]], Callable[..., JsonType]]
         | Callable[..., JsonType]
     ):
-        """Add a function
+        """Add a function to the functions available to the AI
 
         Args:
-            function (OpenAIFunction | Callable[..., JsonType]): The function
-            save_return (bool): Whether to send the return value of this
-                function to the AI. Defaults to True.
-            serialize (bool): Whether to serialize the return value of this
-                function. Defaults to True. Otherwise, the return value must be a
-                string.
-            interpret_as_response (bool): Whether to interpret the return
-                value of this function as a response of the agent. Defaults to False.
+            function (OpenAIFunction | Callable[..., JsonType]): The function to add
+            save_return (bool): Whether to send the return value of this function back
+                to the AI. Defaults to True.
+            serialize (bool): Whether to serialize the return value of this function.
+            Defaults to True. Otherwise, the return value must be a string.
+            interpret_as_response (bool): Whether to interpret the return value of this
+                function as a response of the agent, replacing the function call
+                message. Defaults to False.
 
         Returns:
             Callable[[Callable[..., JsonType]], Callable[..., JsonType]]: A decorator
             Callable[..., JsonType]: The original function
         """
         if function is None:
             return self.skills.add_function(
@@ -328,27 +344,27 @@
 
         Args:
             function (str | OpenAIFunction | Callable[..., JsonType]): The function
         """
         self.skills.remove_function(function)
 
     def ask(self, question: str) -> str:
-        """Ask the AI a question
+        """Ask the AI a question, running until a response is generated
 
         Args:
             question (str): The question
 
         Returns:
             str: The answer to the question
         """
         self.add_message(question)
         return self.run_until_response().content
 
     def add_skill(self, skill: FunctionSet) -> None:
-        """Add a skill
+        """Add a skill to those available to the AI
 
         Args:
             skill (FunctionSet): The skill to add
         """
         self.skills.add_skill(skill)
 
     def run(self, function: str, prompt: str) -> Any:
```

### Comparing `openai_functions-0.6.2/openai_functions/functions/basic_set.py` & `openai_functions-0.6.3/openai_functions/functions/basic_set.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 """A module for running OpenAI functions"""
 from __future__ import annotations
 import json
 from typing import TYPE_CHECKING
 
 from .exceptions import FunctionNotFoundError
 from .functions import FunctionResult, OpenAIFunction, RawFunctionResult
-from .sets import FunctionSet
+from .sets import MutableFunctionSet
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
     from ..openai_types import FunctionCall
 
 
-class BasicFunctionSet(FunctionSet):
-    """A skill set"""
+class BasicFunctionSet(MutableFunctionSet):
+    """A skill set - a set of OpenAIFunction objects ready to be called.
+    Inherited from `MutableFunctionSet`, therefore you can add and remove functions
+    by using the `@add_function` and `remove_function` methods.
+
+    Args:
+        functions (list[OpenAIFunction] | None): The functions to initialize with.
+    """
 
     def __init__(
         self,
         functions: list[OpenAIFunction] | None = None,
     ) -> None:
         self.functions = functions or []
 
     @property
     def functions_schema(self) -> list[JsonType]:
-        """Get the functions schema
+        """Get the functions schema, in the format OpenAI expects
 
         Returns:
-            JsonType: The functions schema
+            JsonType: The schema of all the available functions
         """
         return [function.schema for function in self.functions]
 
     def run_function(self, input_data: FunctionCall) -> FunctionResult:
         """Run the function
 
         Args:
@@ -43,58 +49,57 @@
             FunctionNotFoundError: If the function is not found
         """
         function = self.find_function(input_data["name"])
         result = self.get_function_result(function, json.loads(input_data["arguments"]))
         return FunctionResult(function.name, result, function.interpret_as_response)
 
     def find_function(self, function_name: str) -> OpenAIFunction:
-        """Find a function
+        """Find a function in the skillset
 
         Args:
             function_name (str): The function name
 
         Returns:
-            OpenAIFunction: The function
+            OpenAIFunction: The function of the given name
 
         Raises:
             FunctionNotFoundError: If the function is not found
         """
         for function in self.functions:
             if function.name == function_name:
                 return function
         raise FunctionNotFoundError(f"Function {function_name} not found")
 
     def get_function_result(
         self, function: OpenAIFunction, arguments: dict[str, JsonType]
     ) -> RawFunctionResult | None:
-        """Get the result of a function
+        """Get the result of a function's execution
 
         Args:
-            function (OpenAIFunction): The function
-            arguments (dict[str, JsonType]): The arguments
+            function (OpenAIFunction): The function to run
+            arguments (dict[str, JsonType]): The arguments to run the function with
 
         Returns:
-            RawFunctionResult | None: The result
+            RawFunctionResult | None: The result of the function, or None if the
+                function does not save its return value
         """
         result = function(arguments)
 
         if function.save_return:
-            if function.serialize:
-                return RawFunctionResult(result)
-            return RawFunctionResult(result)
+            return RawFunctionResult(result, serialize=function.serialize)
         return None
 
     def _add_function(self, function: OpenAIFunction) -> None:
-        """Add a function
+        """Add a function to the skillset
 
         Args:
             function (OpenAIFunction): The function
         """
         self.functions.append(function)
 
     def _remove_function(self, name: str) -> None:
-        """Remove a function
+        """Remove a function from the skillset
 
         Args:
             name (str): The name of the function to remove
         """
         self.functions = [f for f in self.functions if f.name != name]
```

### Comparing `openai_functions-0.6.2/openai_functions/functions/functions.py` & `openai_functions-0.6.3/openai_functions/functions/functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
 
 
 @runtime_checkable
 class OpenAIFunction(Protocol):
-    """A protocol for OpenAI functions"""
+    """A protocol for OpenAI functions.
+
+    Requires a __call__ method, a schema property, and a name property,
+    as well as those that define the treatment of the return value.
+    """
 
     def __call__(self, arguments: dict[str, JsonType]) -> JsonType:
         ...
 
     @property
     def schema(self) -> JsonType:
         """Get the schema for this function"""
```

### Comparing `openai_functions-0.6.2/openai_functions/functions/sets.py` & `openai_functions-0.6.3/openai_functions/functions/sets.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
     from ..openai_types import FunctionCall
 
 
 class FunctionSet(ABC):
-    """A skill set"""
+    """A skill set - a provider for a functions schema and a function runner"""
 
     @property
     @abstractmethod
     def functions_schema(self) -> list[JsonType]:
         """Get the functions schema"""
 
     @abstractmethod
@@ -27,14 +27,29 @@
         Args:
             input_data (FunctionCall): The function call
 
         Raises:
             FunctionNotFoundError: If the function is not found
         """
 
+    def __call__(self, input_data: FunctionCall) -> JsonType:
+        """Run the function with the given input data
+
+        Args:
+            input_data (FunctionCall): The input data from OpenAI
+
+        Returns:
+            JsonType: Your function's raw result
+        """
+        return self.run_function(input_data).result
+
+
+class MutableFunctionSet(FunctionSet):
+    """A skill set that can be modified - functions can be added and removed"""
+
     @abstractmethod
     def _add_function(self, function: OpenAIFunction) -> None:
         ...
 
     @overload
     def add_function(self, function: OpenAIFunction) -> OpenAIFunction:
         ...
@@ -121,18 +136,7 @@
         if isinstance(function, str):
             self._remove_function(function)
             return
         if isinstance(function, OpenAIFunction):
             self._remove_function(function.name)
             return
         self._remove_function(function.__name__)
-
-    def __call__(self, input_data: FunctionCall) -> JsonType:
-        """Run the function with the given input data
-
-        Args:
-            input_data (FunctionCall): The input data from OpenAI
-
-        Returns:
-            JsonType: Your function's raw result
-        """
-        return self.run_function(input_data).result
```

### Comparing `openai_functions-0.6.2/openai_functions/functions/union.py` & `openai_functions-0.6.3/openai_functions/functions/union.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.2/openai_functions/functions/wrapper.py` & `openai_functions-0.6.3/openai_functions/functions/wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,24 +10,47 @@
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
 
 
 @dataclass
 class WrapperConfig:
-    """Configuration for a FunctionWrapper"""
+    """Configuration for a FunctionWrapper, one that specifies the parsers for the
+    arguments and the treatment of the return value.
+
+    Args:
+        parsers (list[Type[ArgSchemaParser]] | None): The parsers for the arguments.
+            defaults to `defargparsers`, which support all JSON types, as well
+            as enums and dataclasses
+        save_return (bool): Whether to send the return value back to the AI
+        serialize (bool): Whether to serialize the return value; if False, the
+            return value must be a string
+        interpret_as_response (bool): Whether to interpret the return value as a
+            response from the agent directly, or to base the response on the
+            return value
+    """
 
     parsers: list[Type[ArgSchemaParser]] | None = None
     save_return: bool = True
     serialize: bool = True
     interpret_as_response: bool = False
 
 
 class FunctionWrapper:
-    """Wraps a function for jsonschema io"""
+    """Wraps a function for jsonschema io
+
+    Provides a function schema and a function runner - the function schema is
+    generated from the function's docstring and argument type annotations, and
+    the function runner parses the arguments from JSON and runs the function.
+    They are accessed via the `schema` property and a `__call__` method respectively.
+
+    Args:
+        func (Callable[..., JsonType]): The function to wrap
+        config (WrapperConfig | None, optional): The configuration for the wrapper.
+    """
 
     def __init__(
         self,
         func: Callable[..., Any],
         config: WrapperConfig | None = None,
     ) -> None:
         """Initialize a FunctionWrapper
```

### Comparing `openai_functions-0.6.2/openai_functions/nlp.py` & `openai_functions-0.6.3/openai_functions/nlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,38 +12,38 @@
 Param = ParamSpec("Param")
 Return = TypeVar("Return")
 T = TypeVar("T")
 
 
 @dataclass
 class NaturalLanguageAnnotated(Generic[T]):
-    """A natural language annotated object"""
+    """A natural language annotated function return value"""
 
     function_result: T
     annotation: str
 
 
 # This is a callable protocol, thus pylint can shut up
 class DecoratorProtocol(
     Protocol[Param, Return]
 ):  # pylint: disable=too-few-public-methods
-    """A protocol for decorators"""
+    """A protocol for the nlp decorator"""
 
     def __call__(
         self,
         function: Callable[Param, Return],
         *,
         system_prompt: str | None = None,
         model: str = "gpt-3.5-turbo-0613",
     ) -> Wrapper[Param, Return]:
         ...
 
 
 class Wrapper(Generic[Param, Return]):
-    """A wrapper for a function"""
+    """A wrapper for a function that provides a natural language interface"""
 
     def __init__(
         self,
         origin: Callable[..., Return],
         system_prompt: str | None = None,
         model: str = "gpt-3.5-turbo-0613",
     ) -> None:
@@ -64,15 +64,15 @@
                 {
                     "role": "system",
                     "content": self.system_prompt,
                 }
             )
 
     def from_natural_language(self, prompt: str) -> Return:
-        """Run the function with the given prompt
+        """Run the function with the given natural language input
 
         Args:
             prompt (str): The prompt to use
 
         Returns:
             The result of the original function
         """
@@ -82,34 +82,35 @@
     def natural_language_response(self, prompt: str) -> str:
         """Run the function and respond to the user with natural language
 
         Args:
             prompt (str): The prompt to use
 
         Returns:
-            The response from the AI
+            str: The response from the AI
         """
         self._initialize_conversation()
         self.conversation.add_message(prompt)
         self.conversation.generate_message(
             function_call={"name": self.openai_function.name}
         )
         response = self.conversation.run_until_response(False)
         return response.content
 
     def natural_language_annotated(
         self, prompt: str
     ) -> NaturalLanguageAnnotated[Return]:
-        """Run the function and respond to the user with natural language
+        """Run the function and respond to the user with natural language as well as
+        the raw function result
 
         Args:
             prompt (str): The prompt to use
 
         Returns:
-            The response from the AI
+            NaturalLanguageAnnotated: The response from the AI
         """
         self._initialize_conversation()
         function_result = self.conversation.run(self.openai_function.name, prompt)
         response = self.conversation.run_until_response(False)
         return NaturalLanguageAnnotated(function_result, response.content)
 
 
@@ -169,15 +170,15 @@
     Args:
         function (Callable | None): The function
             to add natural language input to
         system_prompt (str | None): The system prompt to use. Defaults to None.
         model (str): The model to use. Defaults to "gpt-3.5-turbo-0613".
 
     Returns:
-        The function, with natural language input, or a decorator to add natural
-        language input to a function
+        Wrapper | DecoratorProtocol: The function, with natural language input, or a
+        decorator to add natural language input to a function
     """
 
     if function is None:
         return partial(_nlp, system_prompt=system_prompt, model=model)
 
     return _nlp(function, system_prompt=system_prompt, model=model)
```

### Comparing `openai_functions-0.6.2/openai_functions/openai_types.py` & `openai_functions-0.6.3/openai_functions/openai_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,20 @@
 )
 
 if TYPE_CHECKING:
     from typing_extensions import TypeGuard
 
 
 class FunctionCall(TypedDict):
-    """A type for OpenAI function calls"""
+    """A container for OpenAI function calls
+
+    Attributes:
+        name (str): The name of the function
+        arguments (str): The arguments of the function, in JSON format
+    """
 
     name: str
     arguments: str
 
 
 class FinalResponseMessageType(TypedDict):
     """A type for OpenAI messages that are final responses"""
@@ -168,15 +173,15 @@
 
     def __hash__(self) -> int:
         return hash((self.content, self.role))
 
 
 @runtime_checkable
 class GenericMessage(Protocol):
-    """A container for OpenAI messages"""
+    """A container protocol for OpenAI messages"""
 
     message: MessageType
 
     @overload
     def __init__(self, message: MessageType) -> None:
         ...
 
@@ -225,15 +230,19 @@
         ...  # pylint: disable=unnecessary-ellipsis
 
     def __hash__(self) -> int:
         ...
 
 
 class FinalResponseMessage(GenericMessage, Protocol):
-    """A container for OpenAI final response messages"""
+    """A container for OpenAI final response messages
+
+    Inherited from GenericMessage, acts the same, just restricts
+    the message to have content and not be a function call
+    """
 
     message: FinalResponseMessageType  # type: ignore
 
     @property
     def content(self) -> str:
         """Get the content of the message"""
         # This ellipsis is for Pyright #2758
```

### Comparing `openai_functions-0.6.2/openai_functions/parsers/abc.py` & `openai_functions-0.6.3/openai_functions/parsers/abc.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,19 @@
     from typing_extensions import TypeGuard
 
 T = TypeVar("T")
 S = TypeVar("S")
 
 
 class ArgSchemaParser(ABC, Generic[T]):
-    """A parser for a specific argument type"""
+    """An abstract parser for a specific argument type
+
+    Both converts the argument definition to a JSON schema and parses the argument value
+    from JSON.
+    """
 
     def __init__(
         self, argtype: Type[T], rec_parsers: list[Type[ArgSchemaParser]]
     ) -> None:
         self.argtype = argtype
         self.rec_parsers = rec_parsers
```

### Comparing `openai_functions-0.6.2/openai_functions/parsers/atomic_type_parser.py` & `openai_functions-0.6.3/openai_functions/parsers/atomic_type_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.2/openai_functions/parsers/dataclass_parser.py` & `openai_functions-0.6.3/openai_functions/parsers/dataclass_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.2/openai_functions/parsers/default.py` & `openai_functions-0.6.3/openai_functions/parsers/default.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.2/openai_functions/parsers/dict_parser.py` & `openai_functions-0.6.3/openai_functions/parsers/dict_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.2/openai_functions/parsers/enum_parser.py` & `openai_functions-0.6.3/openai_functions/parsers/enum_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.2/openai_functions/parsers/float_parser.py` & `openai_functions-0.6.3/openai_functions/parsers/float_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.2/openai_functions/parsers/int_parser.py` & `openai_functions-0.6.3/openai_functions/parsers/int_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.2/openai_functions/parsers/list_parser.py` & `openai_functions-0.6.3/openai_functions/parsers/list_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.2/openai_functions/parsers/none_parser.py` & `openai_functions-0.6.3/openai_functions/parsers/none_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.2/openai_functions/parsers/union_parser.py` & `openai_functions-0.6.3/openai_functions/parsers/union_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.2/pyproject.toml` & `openai_functions-0.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-functions"
-version = "0.6.2"
+version = "0.6.3"
 description = "Simplifies the usage of OpenAI's function calling."
 authors = ["rizerphe <44440399+rizerphe@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "openai_functions"}]
 
 [tool.poetry.dependencies]
```

### Comparing `openai_functions-0.6.2/PKG-INFO` & `openai_functions-0.6.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functions
-Version: 0.6.2
+Version: 0.6.3
 Summary: Simplifies the usage of OpenAI's function calling.
 License: MIT
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,32 +17,34 @@
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Description-Content-Type: text/markdown
 
 # OpenAI functions
 
 The `openai-functions` Python project simplifies the usage of OpenAI's function calling feature. It abstracts away the complexity of parsing function signatures and docstrings by providing developers with a clean and intuitive interface.
 
-![Tests](https://github.com/rizerphe/openai-functions/actions/workflows/tests.yml/badge.svg) [![Coverage Status](https://coveralls.io/repos/github/rizerphe/openai-functions/badge.svg?branch=main)](https://coveralls.io/github/rizerphe/openai-functions?branch=main) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+![Tests](https://github.com/rizerphe/openai-functions/actions/workflows/tests.yml/badge.svg) [![Coverage Status](https://coveralls.io/repos/github/rizerphe/openai-functions/badge.svg?branch=main)](https://coveralls.io/github/rizerphe/openai-functions?branch=main) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/openai-functions.svg)](https://badge.fury.io/py/openai-functions) [![Documentation Status](https://readthedocs.org/projects/openai-functions/badge/?version=latest)](https://openai-functions.readthedocs.io/en/latest/?badge=latest)
 
 ## Installation
 
 You can install `openai-functions` from PyPI using pip:
 
 ```
 pip install openai-functions
 ```
 
 ## Usage
 
-1. Import the necessary modules:
+1. Import the necessary modules and provide your API key:
 
 ```python
 import enum
 import openai
 from openai_functions import Conversation
+
+openai.api_key = "<YOUR_API_KEY>"
 ```
 
 2. Create a `Conversation` instance:
 
 ```python
 conversation = Conversation()
 ```
@@ -58,64 +60,83 @@
 def get_current_weather(location: str, unit: Unit = Unit.FAHRENHEIT) -> dict:
     """Get the current weather in a given location.
 
     Args:
         location (str): The city and state, e.g., San Francisco, CA
         unit (Unit): The unit to use, e.g., fahrenheit or celsius
     """
-    weather_info = {
+    return {
         "location": location,
         "temperature": "72",
         "unit": unit.value,
         "forecast": ["sunny", "windy"],
     }
-    return weather_info
 ```
 
 4. Ask the AI a question:
 
 ```python
-conversation.ask("What's the weather in San Francisco?")
+response = conversation.ask("What's the weather in San Francisco?")
+# Should return something like:
+# The current weather in San Francisco is 72 degrees Fahrenheit and it is sunny and windy.
+```
+
+You can read more about how to use `Conversation` [here](https://openai-functions.readthedocs.io/en/latest/conversation.html).
+
+## More barebones use - just schema generation and result parsing:
+
+```python
+from openai_functions import FunctionWrapper
+
+wrapper = FunctionWrapper(get_current_weather)
+schema = wrapper.schema
+result = wrapper({"location": "San Francisco, CA"})
 ```
 
+Or you could use [skills](https://openai-functions.readthedocs.io/en/latest/skills.html).
+
 ## Another use case: data extraction
 
-1. Import the necessary modules:
+1. Import the necessary modules and provide your API key:
 
 ```python
 from dataclasses import dataclass
 import openai
 from openai_functions import nlp
+
+openai.api_key = "<YOUR_API_KEY>"
 ```
 
 3. Define your data container using the `@nlp` decorator:
 
 ```python
 @nlp
 @dataclass
 class Person:
     """Extract personal info"""
 
     name: str
     age: int
 ```
 
-4. Ask the AI for a summary of the data:
+4. Ask the AI for the extracted data:
 
 ```python
 person = Person.from_natural_language("I'm Jack and I'm 20 years old.")
 ```
 
+You can read more about `@nlp` [here](https://openai-functions.readthedocs.io/en/latest/nlp_interface.html).
+
 Note: mypy does not parse class decorators ([#3135](https://github.com/python/mypy/issues/3135)), so you might have trouble getting type checking when using it like this. Consider using something like `nlp(Person).from_natural_language` to get proper type support.
 
 ## How it Works
 
 `openai-functions` takes care of the following tasks:
 
-- Parsing the function signatures and docstrings.
+- Parsing the function signatures (with type annotations) and docstrings.
 - Sending the conversation and function descriptions to the OpenAI model.
 - Deciding whether to call a function based on the model's response.
 - Calling the appropriate function with the provided arguments.
 - Updating the conversation with the function response.
 - Repeating the process until the model generates a user-facing message.
 
 This abstraction allows developers to focus on defining their functions and adding user messages without worrying about the details of function calling.
```

