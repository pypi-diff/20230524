# Comparing `tmp/llmo-0.3.0.tar.gz` & `tmp/llmo-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmo-0.3.0.tar", last modified: Wed May 24 03:21:59 2023, max compression
+gzip compressed data, was "llmo-0.4.0.tar", last modified: Wed May 24 03:59:09 2023, max compression
```

## Comparing `llmo-0.3.0.tar` & `llmo-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.3.0/LICENSE
--rw-r--r--   0        0        0     2134 2023-05-22 08:06:19.890271 llmo-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.3.0/llmo/__init__.py
--rw-r--r--   0        0        0     2961 2023-05-24 03:21:31.439301 llmo-0.3.0/llmo/cli.py
--rw-r--r--   0        0        0      122 2023-05-22 21:51:03.475865 llmo-0.3.0/llmo/constants.py
--rw-r--r--   0        0        0     9793 2023-05-23 03:53:39.625867 llmo-0.3.0/llmo/gui.py
--rw-r--r--   0        0        0      341 2023-05-23 03:17:45.469101 llmo-0.3.0/llmo/layout.css
--rw-r--r--   0        0        0     5982 2023-05-23 03:45:21.644631 llmo-0.3.0/llmo/llms.py
--rw-r--r--   0        0        0     1593 2023-05-23 04:53:16.585981 llmo-0.3.0/llmo/shell_mode.py
--rw-r--r--   0        0        0      699 2023-05-24 03:21:59.296374 llmo-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      838 2023-05-22 22:24:34.139710 llmo-0.3.0/tests/test_openai.py
--rw-r--r--   0        0        0     2479 1970-01-01 00:00:00.000000 llmo-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2134 2023-05-22 08:06:19.890271 llmo-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.4.0/llmo/__init__.py
+-rw-r--r--   0        0        0     2961 2023-05-24 03:21:31.439301 llmo-0.4.0/llmo/cli.py
+-rw-r--r--   0        0        0      122 2023-05-22 21:51:03.475865 llmo-0.4.0/llmo/constants.py
+-rw-r--r--   0        0        0     9793 2023-05-23 03:53:39.625867 llmo-0.4.0/llmo/gui.py
+-rw-r--r--   0        0        0      341 2023-05-23 03:17:45.469101 llmo-0.4.0/llmo/layout.css
+-rw-r--r--   0        0        0     6420 2023-05-24 03:57:19.021780 llmo-0.4.0/llmo/llms.py
+-rw-r--r--   0        0        0     1593 2023-05-23 04:53:16.585981 llmo-0.4.0/llmo/shell_mode.py
+-rw-r--r--   0        0        0      722 2023-05-24 03:59:09.885403 llmo-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      838 2023-05-22 22:24:34.139710 llmo-0.4.0/tests/test_openai.py
+-rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 llmo-0.4.0/PKG-INFO
```

### Comparing `llmo-0.3.0/LICENSE` & `llmo-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmo-0.3.0/README.md` & `llmo-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `llmo-0.3.0/llmo/cli.py` & `llmo-0.4.0/llmo/cli.py`

 * *Files identical despite different names*

### Comparing `llmo-0.3.0/llmo/gui.py` & `llmo-0.4.0/llmo/gui.py`

 * *Files identical despite different names*

### Comparing `llmo-0.3.0/llmo/llms.py` & `llmo-0.4.0/llmo/llms.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,41 @@
 from collections import deque
 from copy import copy
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import TypedDict, Literal, Iterable
 
 import openai
+import openai.error
+from tenacity import retry, stop_after_attempt, wait_fixed, retry_if_exception_type
 
 from llmo.constants import ESTIMATED_CHAR_PER_TOKEN
 
 
 class Message(TypedDict):
     role: Literal["user", "system", "assistant"]
     content: str
 
 
 class SystemMessage(TypedDict):
     role: Literal["system"]
     content: str
 
 
+def retry_openai_call(func):
+    return retry(
+        retry=(
+            retry_if_exception_type(openai.error.APIConnectionError)
+            | retry_if_exception_type(openai.error.RateLimitError)
+        ),
+        stop=stop_after_attempt(5),
+        wait=wait_fixed(2),
+    )(func)
+
+
 @dataclass
 class OpenAI:
     model: str = "gpt-3.5-turbo"
     temperature: float = 0.7
     messages: deque[Message] = field(default_factory=deque)
     api_key: str = None
     system_prompt: str = (
@@ -51,49 +64,14 @@
         self._initial_system_prompt = self.system_prompt
         if self.api_key:
             openai.api_key = self.api_key
 
     def reset(self):
         self.messages = deque()
 
-    def submit(self, prompt: str, files: Iterable[Path] = None):
-        """
-        Submit a prompt to the OpenAI API and return the response.
-
-        If files are provided, they will be added to the prompt as part of the submission.
-        """
-        for file in files or []:
-            # remove any existing messages with the same file content
-            temp_messages = copy(self.messages)
-            for msg in temp_messages:
-                if msg["role"] == "user" and msg["content"].startswith(f"`{file}`"):
-                    self.messages.remove(msg)
-            self.messages.append(
-                {"role": "user", "content": f"`{file}`\n```{file.read_text()}```"}
-            )
-        self.messages.append({"role": "user", "content": prompt})
-
-        self.truncate_old_messages()
-
-        system_message = SystemMessage(
-            role="system",
-            content=self.system_prompt,
-        )
-        messages = [system_message, *self.messages]
-
-        assistant_message = openai.ChatCompletion.create(
-            messages=messages,
-            model=self.model,
-            temperature=self.temperature,
-        )["choices"][0]["message"]
-
-        self.messages.append(assistant_message)
-
-        return assistant_message["content"]
-
     def remove_file_messages(self):
         temp_messages = copy(self.messages)
         for msg in temp_messages:
             if (
                 msg["role"] == "user"
                 and msg["content"].startswith("`")
                 and msg["content"].endswith("```")
@@ -117,14 +95,15 @@
                     # If a file message was removed, continue to the next iteration
                     continue
 
                 estimated_tokens -= (
                     len(removed_message["content"]) / ESTIMATED_CHAR_PER_TOKEN
                 )
 
+    @retry_openai_call
     async def asubmit(self, prompt: str, files: Iterable[Path] = None):
         """
         Submit a prompt to the OpenAI API and asynchronously yield tokens.
 
         If files are provided, they will be added to the prompt as part of the submission.
         """
         for file in files or []:
@@ -169,7 +148,43 @@
                 self.messages.append(assistant_message)
                 return
             if role:
                 continue
             elif content:
                 assistant_message["content"] += content
                 yield content
+
+    @retry_openai_call
+    def submit(self, prompt: str, files: Iterable[Path] = None):
+        """
+        Submit a prompt to the OpenAI API and return the response.
+
+        If files are provided, they will be added to the prompt as part of the submission.
+        """
+        for file in files or []:
+            # remove any existing messages with the same file content
+            temp_messages = copy(self.messages)
+            for msg in temp_messages:
+                if msg["role"] == "user" and msg["content"].startswith(f"`{file}`"):
+                    self.messages.remove(msg)
+            self.messages.append(
+                {"role": "user", "content": f"`{file}`\n```{file.read_text()}```"}
+            )
+        self.messages.append({"role": "user", "content": prompt})
+
+        self.truncate_old_messages()
+
+        system_message = SystemMessage(
+            role="system",
+            content=self.system_prompt,
+        )
+        messages = [system_message, *self.messages]
+
+        assistant_message = openai.ChatCompletion.create(
+            messages=messages,
+            model=self.model,
+            temperature=self.temperature,
+        )["choices"][0]["message"]
+
+        self.messages.append(assistant_message)
+
+        return assistant_message["content"]
```

### Comparing `llmo-0.3.0/llmo/shell_mode.py` & `llmo-0.4.0/llmo/shell_mode.py`

 * *Files identical despite different names*

### Comparing `llmo-0.3.0/pyproject.toml` & `llmo-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [project]
 name = "llmo"
-version = "0.3.0"
+version = "0.4.0"
 description = "AI pair programmer"
 authors = [
     { name = "Stephan Fitzpatrick", email = "stephan@knowsuchagency.com" },
 ]
 dependencies = [
     "textual>=0.26.0",
     "openai>=0.27.6",
+    "tenacity>=8.2.2",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 
 [project.license]
 text = "Apache-2.0"
```

### Comparing `llmo-0.3.0/tests/test_openai.py` & `llmo-0.4.0/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `llmo-0.3.0/PKG-INFO` & `llmo-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: llmo
-Version: 0.3.0
+Version: 0.4.0
 Summary: AI pair programmer
 Author-Email: Stephan Fitzpatrick <stephan@knowsuchagency.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/knowsuchagency/llmo
 Requires-Python: >=3.10
 Requires-Dist: textual>=0.26.0
 Requires-Dist: openai>=0.27.6
+Requires-Dist: tenacity>=8.2.2
 Description-Content-Type: text/markdown
 
 # LLMO (Elmo)
 
 *Meaning:*
 - Protector
 - Worthy to be Loved
```

