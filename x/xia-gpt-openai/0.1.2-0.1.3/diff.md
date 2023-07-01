# Comparing `tmp/xia_gpt_openai-0.1.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_gpt_openai-0.1.3-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2674 bytes, number of entries: 7
--rw-r--r--  2.0 unx       94 b- defN 23-Jun-30 11:30 xia_gpt_openai/__init__.py
--rw-r--r--  2.0 unx     1724 b- defN 23-Jun-30 11:30 xia_gpt_openai/gpt.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:33 xia_gpt_openai-0.1.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      439 b- defN 23-Jun-30 11:33 xia_gpt_openai-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:33 xia_gpt_openai-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-30 11:33 xia_gpt_openai-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      582 b- defN 23-Jun-30 11:33 xia_gpt_openai-0.1.2.dist-info/RECORD
-7 files, 3104 bytes uncompressed, 1630 bytes compressed:  47.5%
+Zip file size: 2695 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      121 b- defN 23-Jul-01 16:09 xia_gpt_openai/__init__.py
+-rw-r--r--  2.0 unx     1747 b- defN 23-Jul-01 16:09 xia_gpt_openai/gpt.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 16:09 xia_gpt_openai-0.1.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      439 b- defN 23-Jul-01 16:09 xia_gpt_openai-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 16:09 xia_gpt_openai-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jul-01 16:09 xia_gpt_openai-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      583 b- defN 23-Jul-01 16:09 xia_gpt_openai-0.1.3.dist-info/RECORD
+7 files, 3155 bytes uncompressed, 1651 bytes compressed:  47.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_gpt_openai/__init__.py
 Comment: 
 
 Filename: xia_gpt_openai/gpt.py
 Comment: 
 
-Filename: xia_gpt_openai-0.1.2.dist-info/LICENSE.txt
+Filename: xia_gpt_openai-0.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_gpt_openai-0.1.2.dist-info/METADATA
+Filename: xia_gpt_openai-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_gpt_openai-0.1.2.dist-info/WHEEL
+Filename: xia_gpt_openai-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_gpt_openai-0.1.2.dist-info/top_level.txt
+Filename: xia_gpt_openai-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_gpt_openai-0.1.2.dist-info/RECORD
+Filename: xia_gpt_openai-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_gpt_openai/__init__.py

```diff
@@ -1,7 +1,7 @@
-from xia_gpt_openai.gpt import OpenaiGpt
+from xia_gpt_openai.gpt import OpenaiGpt, OpenaiGpt4
 
 __all__ = [
-    "OpenaiGpt"
+    "OpenaiGpt", "OpenaiGpt4"
 ]
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

## xia_gpt_openai/gpt.py

```diff
@@ -4,15 +4,14 @@
 
 
 class OpenaiGpt(Gpt):
     gpt_engine = openai
     gpt_engine_name = "openai"
     gpt_engine.api_key = os.environ.get("OPEN_API_KEY")
     gpt_engine_model = "gpt-3.5-turbo"
-    # gpt_engine_model = "gpt-4"
 
     def chat_complete(self, system: str, message: str, context: list = None, **kwargs):
         """Give the context and
 
         Args:
             system: System Roles
             message: User message to be sent
@@ -30,14 +29,18 @@
             built_request.append({"role": "user", "content": dialog["assistant"]})
         built_request.append({"role": "user", "content": message})
         job_result = openai.ChatCompletion.create(model=self.gpt_engine_model, messages=built_request, **kwargs)
         choices = job_result.pop("choices")
         return choices[0].message["content"], job_result
 
 
+class OpenaiGpt4(Gpt):
+    gpt_engine_model = "gpt-4"
+
+
 if __name__ == '__main__':
     gpt_agent = OpenaiGpt()
     result, job_status = gpt_agent.chat_complete(
         "You are a helpful assistant.",
         "Where was it played?",
         [{"user": "Who won the world series in 2020?",
          "assistant": "The Los Angeles Dodgers won the World Series in 2020."}]
```

