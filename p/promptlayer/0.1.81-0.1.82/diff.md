# Comparing `tmp/promptlayer-0.1.81.tar.gz` & `tmp/promptlayer-0.1.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/promptlayer-0.1.81.tar", last modified: Fri May 12 18:11:38 2023, max compression
+gzip compressed data, was "dist/promptlayer-0.1.82.tar", last modified: Wed May 24 19:32:30 2023, max compression
```

## Comparing `promptlayer-0.1.81.tar` & `promptlayer-0.1.82.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-12 18:11:38.661507 promptlayer-0.1.81/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    11357 2023-01-26 22:51:29.000000 promptlayer-0.1.81/LICENSE
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-05-12 18:11:38.661229 promptlayer-0.1.81/PKG-INFO
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3891 2023-01-26 22:51:29.000000 promptlayer-0.1.81/README.md
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-12 18:11:38.655578 promptlayer-0.1.81/promptlayer/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      341 2023-03-13 20:43:03.000000 promptlayer-0.1.81/promptlayer/__init__.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-12 18:11:38.658336 promptlayer-0.1.81/promptlayer/langchain/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        0 2023-02-01 20:15:14.000000 promptlayer-0.1.81/promptlayer/langchain/__init__.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-12 18:11:38.659003 promptlayer-0.1.81/promptlayer/langchain/llms/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-02-01 20:08:36.000000 promptlayer-0.1.81/promptlayer/langchain/llms/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2012 2023-02-15 16:07:17.000000 promptlayer-0.1.81/promptlayer/langchain/llms/openai.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2689 2023-03-27 21:24:30.000000 promptlayer-0.1.81/promptlayer/promptlayer.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-12 18:11:38.659679 promptlayer-0.1.81/promptlayer/prompts/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      124 2023-02-16 22:50:19.000000 promptlayer-0.1.81/promptlayer/prompts/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1285 2023-03-31 18:02:42.000000 promptlayer-0.1.81/promptlayer/prompts/prompts.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-12 18:11:38.660711 promptlayer-0.1.81/promptlayer/track/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       59 2023-03-13 20:43:03.000000 promptlayer-0.1.81/promptlayer/track/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1239 2023-05-12 18:10:56.000000 promptlayer-0.1.81/promptlayer/track/track.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    12965 2023-03-31 18:02:42.000000 promptlayer-0.1.81/promptlayer/utils.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-12 18:11:38.657969 promptlayer-0.1.81/promptlayer.egg-info/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-05-12 18:11:38.000000 promptlayer-0.1.81/promptlayer.egg-info/PKG-INFO
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      502 2023-05-12 18:11:38.000000 promptlayer-0.1.81/promptlayer.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        1 2023-05-12 18:11:38.000000 promptlayer-0.1.81/promptlayer.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-05-12 18:11:38.000000 promptlayer-0.1.81/promptlayer.egg-info/requires.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       12 2023-05-12 18:11:38.000000 promptlayer-0.1.81/promptlayer.egg-info/top_level.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       38 2023-05-12 18:11:38.661613 promptlayer-0.1.81/setup.cfg
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      832 2023-05-12 18:11:05.000000 promptlayer-0.1.81/setup.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-24 19:32:30.496979 promptlayer-0.1.82/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    11357 2023-01-26 22:51:29.000000 promptlayer-0.1.82/LICENSE
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-05-24 19:32:30.496641 promptlayer-0.1.82/PKG-INFO
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3891 2023-01-26 22:51:29.000000 promptlayer-0.1.82/README.md
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-24 19:32:30.490775 promptlayer-0.1.82/promptlayer/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      496 2023-05-24 19:31:54.000000 promptlayer-0.1.82/promptlayer/__init__.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-24 19:32:30.492558 promptlayer-0.1.82/promptlayer/langchain/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        0 2023-02-01 20:15:14.000000 promptlayer-0.1.82/promptlayer/langchain/__init__.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-24 19:32:30.493140 promptlayer-0.1.82/promptlayer/langchain/llms/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-02-01 20:08:36.000000 promptlayer-0.1.82/promptlayer/langchain/llms/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2012 2023-02-15 16:07:17.000000 promptlayer-0.1.82/promptlayer/langchain/llms/openai.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2689 2023-03-27 21:24:30.000000 promptlayer-0.1.82/promptlayer/promptlayer.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-24 19:32:30.494162 promptlayer-0.1.82/promptlayer/prompts/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      124 2023-02-16 22:50:19.000000 promptlayer-0.1.82/promptlayer/prompts/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1285 2023-03-31 18:02:42.000000 promptlayer-0.1.82/promptlayer/prompts/prompts.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-24 19:32:30.495293 promptlayer-0.1.82/promptlayer/track/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       59 2023-03-13 20:43:03.000000 promptlayer-0.1.82/promptlayer/track/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1239 2023-05-12 18:10:56.000000 promptlayer-0.1.82/promptlayer/track/track.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    13445 2023-05-24 19:31:54.000000 promptlayer-0.1.82/promptlayer/utils.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-05-24 19:32:30.492224 promptlayer-0.1.82/promptlayer.egg-info/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-05-24 19:32:30.000000 promptlayer-0.1.82/promptlayer.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      502 2023-05-24 19:32:30.000000 promptlayer-0.1.82/promptlayer.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        1 2023-05-24 19:32:30.000000 promptlayer-0.1.82/promptlayer.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-05-24 19:32:30.000000 promptlayer-0.1.82/promptlayer.egg-info/requires.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       12 2023-05-24 19:32:30.000000 promptlayer-0.1.82/promptlayer.egg-info/top_level.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       38 2023-05-24 19:32:30.497134 promptlayer-0.1.82/setup.cfg
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      832 2023-05-24 19:32:04.000000 promptlayer-0.1.82/setup.py
```

### Comparing `promptlayer-0.1.81/LICENSE` & `promptlayer-0.1.82/LICENSE`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.81/PKG-INFO` & `promptlayer-0.1.82/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.1.81
+Version: 0.1.82
 Summary: PromptLayer is a package to keep track of your GPT models training
 Home-page: https://www.promptlayer.com
 Author: Magniv
 Author-email: hello@magniv.io
 License: UNKNOWN
 Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.1.81 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.1.82 Summary: PromptLayer is
 a package to keep track of your GPT models training Home-page: https://
 www.promptlayer.com Author: Magniv Author-email: hello@magniv.io License:
 UNKNOWN Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-
 Docs-db0e6f50cacf4564a6d09824ba17a629 Description:
 # ð° PromptLayer **The first platform built for prompt engineers** [Python]
                           [Docs] [Demo_with_Loom] ---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
```

### Comparing `promptlayer-0.1.81/README.md` & `promptlayer-0.1.82/README.md`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.81/promptlayer/langchain/llms/openai.py` & `promptlayer-0.1.82/promptlayer/langchain/llms/openai.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.81/promptlayer/promptlayer.py` & `promptlayer-0.1.82/promptlayer/promptlayer.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.81/promptlayer/prompts/prompts.py` & `promptlayer-0.1.82/promptlayer/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.81/promptlayer/track/track.py` & `promptlayer-0.1.82/promptlayer/track/track.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.81/promptlayer/utils.py` & `promptlayer-0.1.82/promptlayer/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     request_end_time,
     api_key,
     return_pl_id=False,
 ):
     if isinstance(response, types.GeneratorType) or isinstance(
         response, types.AsyncGeneratorType
     ):
-        return OpenAIGeneratorProxy(
+        return GeneratorProxy(
             response,
             {
                 "function_name": function_name,
                 "provider_type": provider_type,
                 "args": args,
                 "kwargs": kwargs,
                 "tags": tags,
@@ -180,16 +180,15 @@
     """
     Get a prompt from the PromptLayer library
     version: version of the prompt to get, None for latest
     """
     try:
         request_response = requests.post(
             f"{URL_API_PROMPTLAYER}/library-get-prompt-template",
-            json={"prompt_name": prompt_name,
-                  "api_key": api_key, 'version': version},
+            json={"prompt_name": prompt_name, "api_key": api_key, "version": version},
         )
         if request_response.status_code != 200:
             if hasattr(request_response, "json"):
                 raise Exception(
                     f"PromptLayer had the following error while getting your prompt: {request_response.json().get('message')}"
                 )
             else:
@@ -226,15 +225,17 @@
     except Exception as e:
         raise Exception(
             f"PromptLayer had the following error while publishing your prompt: {e}"
         )
     return True
 
 
-def promptlayer_track_prompt(request_id, prompt_name, input_variables, api_key, version):
+def promptlayer_track_prompt(
+    request_id, prompt_name, input_variables, api_key, version
+):
     try:
         request_response = requests.post(
             f"{URL_API_PROMPTLAYER}/library-track-prompt",
             json={
                 "request_id": request_id,
                 "prompt_name": prompt_name,
                 "prompt_input_variables": input_variables,
@@ -264,16 +265,19 @@
     return True
 
 
 def promptlayer_track_metadata(request_id, metadata, api_key):
     try:
         request_response = requests.post(
             f"{URL_API_PROMPTLAYER}/library-track-metadata",
-            json={"request_id": request_id,
-                  "metadata": metadata, "api_key": api_key, },
+            json={
+                "request_id": request_id,
+                "metadata": metadata,
+                "api_key": api_key,
+            },
         )
         if request_response.status_code != 200:
             if hasattr(request_response, "json"):
                 print(
                     f"WARNING: While tracking your metadata PromptLayer had the following error: {request_response.json().get('message')}",
                     file=sys.stderr,
                 )
@@ -293,16 +297,19 @@
     return True
 
 
 def promptlayer_track_score(request_id, score, api_key):
     try:
         request_response = requests.post(
             f"{URL_API_PROMPTLAYER}/library-track-score",
-            json={"request_id": request_id,
-                  "score": score, "api_key": api_key, },
+            json={
+                "request_id": request_id,
+                "score": score,
+                "api_key": api_key,
+            },
         )
         if request_response.status_code != 200:
             if hasattr(request_response, "json"):
                 print(
                     f"WARNING: While tracking your score PromptLayer had the following error: {request_response.json().get('message')}",
                     file=sys.stderr,
                 )
@@ -318,15 +325,15 @@
             f"WARNING: While tracking your score PromptLayer had the following error: {e}",
             file=sys.stderr,
         )
         return False
     return True
 
 
-class OpenAIGeneratorProxy:
+class GeneratorProxy:
     def __init__(self, generator, api_request_arguments):
         self.generator = generator
         self.results = []
         self.api_request_arugments = api_request_arguments
 
     def __iter__(self):
         return self
@@ -340,18 +347,21 @@
 
     def __next__(self):
         result = next(self.generator)
         return self._abstracted_next(result)
 
     def _abstracted_next(self, result):
         self.results.append(result)
-        if (
+        provider_type = self.api_request_arugments["provider_type"]
+        end_anthropic = provider_type == "anthropic" and result.get("stop")
+        end_openai = provider_type == "openai" and (
             result.choices[0].finish_reason == "stop"
             or result.choices[0].finish_reason == "length"
-        ):
+        )
+        if end_anthropic or end_openai:
             request_id = promptlayer_api_request(
                 self.api_request_arugments["function_name"],
                 self.api_request_arugments["provider_type"],
                 self.api_request_arugments["args"],
                 self.api_request_arugments["kwargs"],
                 self.api_request_arugments["tags"],
                 self.cleaned_result(),
@@ -363,14 +373,18 @@
             if self.api_request_arugments["return_pl_id"]:
                 return result, request_id
         if self.api_request_arugments["return_pl_id"]:
             return result, None
         return result
 
     def cleaned_result(self):
+        provider_type = self.api_request_arugments["provider_type"]
+        if provider_type == "anthropic":
+            final_result = deepcopy(self.results[-1])
+            return final_result
         if hasattr(self.results[0].choices[0], "text"):  # this is regular completion
             response = ""
             for result in self.results:
                 response = f"{response}{result.choices[0].text}"
             final_result = deepcopy(self.results[-1])
             final_result.choices[0].text = response
             return final_result
```

### Comparing `promptlayer-0.1.81/promptlayer.egg-info/PKG-INFO` & `promptlayer-0.1.82/promptlayer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.1.81
+Version: 0.1.82
 Summary: PromptLayer is a package to keep track of your GPT models training
 Home-page: https://www.promptlayer.com
 Author: Magniv
 Author-email: hello@magniv.io
 License: UNKNOWN
 Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.1.81 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.1.82 Summary: PromptLayer is
 a package to keep track of your GPT models training Home-page: https://
 www.promptlayer.com Author: Magniv Author-email: hello@magniv.io License:
 UNKNOWN Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-
 Docs-db0e6f50cacf4564a6d09824ba17a629 Description:
 # ð° PromptLayer **The first platform built for prompt engineers** [Python]
                           [Docs] [Demo_with_Loom] ---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
```

### Comparing `promptlayer-0.1.81/setup.py` & `promptlayer-0.1.82/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,12 +13,12 @@
     description="PromptLayer is a package to keep track of your GPT models training",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Magniv",
     author_email="hello@magniv.io",
     url="https://www.promptlayer.com",
     project_urls={"Documentation": "https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629",},
-    version="0.1.81",
+    version="0.1.82",
     py_modules=["promptlayer"],
     packages=find_packages(),
     install_requires=["requests", "openai", "langchain"],
 )
```

