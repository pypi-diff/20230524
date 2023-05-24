# Comparing `tmp/agixt-1.1.71b0.tar.gz` & `tmp/agixt-1.1.72b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.71b0.tar", last modified: Wed May 24 02:29:52 2023, max compression
+gzip compressed data, was "agixt-1.1.72b0.tar", last modified: Wed May 24 16:11:02 2023, max compression
```

## Comparing `agixt-1.1.71b0.tar` & `agixt-1.1.72b0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:29:52.819882 agixt-1.1.71b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-24 02:29:38.000000 agixt-1.1.71b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-24 02:29:38.000000 agixt-1.1.71b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-24 02:29:52.819882 agixt-1.1.71b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:29:52.819882 agixt-1.1.71b0/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    17365 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/AGiXT.py
--rw-r--r--   0 runner    (1001) docker     (123)    14049 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/Commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/CustomPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/Main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/Tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:29:52.819882 agixt-1.1.71b0/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/provider/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/provider/llamacppapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 02:29:38.000000 agixt-1.1.71b0/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:29:52.819882 agixt-1.1.71b0/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-24 02:29:52.000000 agixt-1.1.71b0/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-24 02:29:52.000000 agixt-1.1.71b0/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 02:29:52.000000 agixt-1.1.71b0/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-24 02:29:52.000000 agixt-1.1.71b0/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 02:29:52.000000 agixt-1.1.71b0/agixt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:29:52.819882 agixt-1.1.71b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-24 02:29:38.000000 agixt-1.1.71b0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 02:29:38.000000 agixt-1.1.71b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 02:29:52.819882 agixt-1.1.71b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-24 02:29:38.000000 agixt-1.1.71b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:02.015688 agixt-1.1.72b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-24 16:10:49.000000 agixt-1.1.72b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-24 16:10:49.000000 agixt-1.1.72b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-24 16:11:02.015688 agixt-1.1.72b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:02.011688 agixt-1.1.72b0/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/AGiXT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/Commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/CustomPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/Main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/Tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:02.015688 agixt-1.1.72b0/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/llamacppapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:02.011688 agixt-1.1.72b0/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-24 16:11:01.000000 agixt-1.1.72b0/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-24 16:11:02.000000 agixt-1.1.72b0/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:11:01.000000 agixt-1.1.72b0/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-24 16:11:01.000000 agixt-1.1.72b0/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 16:11:01.000000 agixt-1.1.72b0/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:02.015688 agixt-1.1.72b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-24 16:10:49.000000 agixt-1.1.72b0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 16:10:49.000000 agixt-1.1.72b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:11:02.015688 agixt-1.1.72b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-24 16:10:49.000000 agixt-1.1.72b0/setup.py
```

### Comparing `agixt-1.1.71b0/LICENSE` & `agixt-1.1.72b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/PKG-INFO` & `agixt-1.1.72b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.71b0
+Version: 1.1.72b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.71b0/agixt/AGiXT.py` & `agixt-1.1.72b0/agixt/AGiXT.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 import re
 import asyncio
 import regex
 import json
 import time
+import spacy
 from datetime import datetime
 from Agent import Agent
 from CustomPrompt import CustomPrompt
 from duckduckgo_search import ddg
 from urllib.parse import urlparse
 
 
 class AGiXT:
     def __init__(self, agent_name: str = "AGiXT"):
         self.agent_name = agent_name
         self.agent = Agent(self.agent_name)
+        self.agent_commands = self.agent.get_commands_string()
         self.stop_running_event = None
         self.browsed_links = []
         self.failures = 0
+        self.nlp = None
+
+    def load_spacy_model(self):
+        if not self.nlp:
+            try:
+                self.nlp = spacy.load("en_core_web_sm")
+            except:
+                spacy.cli.download("en_core_web_sm")
+                self.nlp = spacy.load("en_core_web_sm")
+        self.nlp.max_length = 99999999999999999999999
 
     def custom_format(self, string, **kwargs):
         if isinstance(string, list):
             string = "".join(str(x) for x in string)
 
         def replace(match):
             key = match.group(1)
@@ -56,25 +68,23 @@
             except:
                 context = "None."
         command_list = self.agent.get_commands_string()
         formatted_prompt = self.custom_format(
             prompt,
             task=task,
             agent_name=self.agent_name,
-            COMMANDS=command_list,
+            COMMANDS=self.agent_commands,
             context=context,
             command_list=command_list,
             date=datetime.now().strftime("%B %d, %Y %I:%M %p"),
             **kwargs,
         )
-        if command_list == "No commands.":
-            formatted_prompt = formatted_prompt.replace(
-                "Commands Available To Complete Task:", ""
-            )
-        tokens = len(self.agent.memories.nlp(formatted_prompt))
+        if not self.nlp:
+            self.load_spacy_model()
+        tokens = len(self.nlp(formatted_prompt))
         return formatted_prompt, prompt, tokens
 
     def run(
         self,
         task: str,
         prompt: str = "",
         context_results: int = 5,
```

### Comparing `agixt-1.1.71b0/agixt/Agent.py` & `agixt-1.1.72b0/agixt/Agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,27 +74,28 @@
             if command not in [cmd[0] for cmd in self.commands]:
                 del self.AGENT_CONFIG["commands"][command]
         with open(f"agents/{self.agent_name}/config.json", "w") as f:
             json.dump(self.AGENT_CONFIG, f)
 
     def get_commands_string(self):
         if len(self.available_commands) == 0:
-            return "No commands."
+            return None
 
         enabled_commands = filter(
             lambda command: command.get("enabled", True), self.available_commands
         )
         if not enabled_commands:
-            return "No commands."
+            return None
 
         friendly_names = map(
             lambda command: f"{command['friendly_name']} - {command['name']}({command['args']})",
             enabled_commands,
         )
-        return "\n".join(friendly_names)
+        command_list = "\n".join(friendly_names)
+        return f"Commands Available To Complete Task:\n{command_list}\n\n"
 
     def get_provider(self):
         config_file = self.get_agent_config()
         if "provider" in config_file:
             return config_file["provider"]
         else:
             return "openai"
```

### Comparing `agixt-1.1.71b0/agixt/Chain.py` & `agixt-1.1.72b0/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/Commands.py` & `agixt-1.1.72b0/agixt/Commands.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/Config.py` & `agixt-1.1.72b0/agixt/Config.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/CustomPrompt.py` & `agixt-1.1.72b0/agixt/CustomPrompt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/Embedding.py` & `agixt-1.1.72b0/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/Main.py` & `agixt-1.1.72b0/agixt/Main.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/Memories.py` & `agixt-1.1.72b0/agixt/Memories.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,69 +12,79 @@
 from playwright.async_api import async_playwright
 from bs4 import BeautifulSoup
 
 
 class Memories:
     def __init__(self, agent_name: str = "AGiXT", agent_config=None):
         self.agent_name = agent_name
-        self.nlp = self.load_spacy_model()
-        self.nlp.max_length = 99999999999999999999999
-        embedder = Embedding(agent_config)
-        self.embedding_function = embedder.embed
-        self.chunk_size = embedder.chunk_size
+        self.agent_config = agent_config
+        self.chroma_client = None
+        self.collection = None
+        self.nlp = None
         self.chroma_persist_dir = f"agents/{self.agent_name}/memories"
         if not os.path.exists(self.chroma_persist_dir):
             os.makedirs(self.chroma_persist_dir)
-        self.chroma_client = self.initialize_chroma_client()
-        self.collection = self.get_or_create_collection()
 
     def load_spacy_model(self):
-        try:
-            return spacy.load("en_core_web_sm")
-        except:
-            spacy.cli.download("en_core_web_sm")
-            return spacy.load("en_core_web_sm")
+        if not self.nlp:
+            try:
+                self.nlp = spacy.load("en_core_web_sm")
+            except:
+                spacy.cli.download("en_core_web_sm")
+                self.nlp = spacy.load("en_core_web_sm")
+        self.nlp.max_length = 99999999999999999999999
 
     def initialize_chroma_client(self):
         try:
             return chromadb.Client(
                 settings=chromadb.config.Settings(
                     chroma_db_impl="duckdb+parquet",
                     persist_directory=self.chroma_persist_dir,
                     anonymized_telemetry=False,
                 )
             )
         except Exception as e:
             raise RuntimeError(f"Unable to initialize chroma client: {e}")
 
     def get_or_create_collection(self):
+        if not self.chroma_client:
+            self.chroma_client = self.initialize_chroma_client()
+        embedder = Embedding(self.agent_config)
+        self.embedding_function = embedder.embed
+        self.chunk_size = embedder.chunk_size
         try:
             return self.chroma_client.get_collection(
                 name="memories", embedding_function=self.embedding_function
             )
         except ValueError:
             print(f"Memories for {self.agent_name} do not exist. Creating...")
             return self.chroma_client.create_collection(
                 name="memories", embedding_function=self.embedding_function
             )
 
     def generate_id(self, content: str, timestamp: str):
         return sha256((content + timestamp).encode()).hexdigest()
 
     def store_memory(self, id: str, content: str, metadatas: dict):
+        if not self.chroma_client:
+            self.chroma_client = self.initialize_chroma_client()
+            self.collection = self.get_or_create_collection()
         try:
             self.collection.add(
                 ids=id,
                 documents=content,
                 metadatas=metadatas,
             )
         except Exception as e:
             print(f"Failed to store memory: {e}")
 
     def store_result(self, task_name: str, result: str):
+        if not self.chroma_client:
+            self.chroma_client = self.initialize_chroma_client()
+            self.collection = self.get_or_create_collection()
         if result:
             timestamp = datetime.now()  # current time as datetime object
             if not isinstance(result, str):
                 result = str(result)
             chunks = self.chunk_content(result, task_name)
             for chunk in chunks:
                 result_id = self.generate_id(chunk, timestamp.isoformat())
@@ -85,14 +95,17 @@
                         "task": task_name,
                         "result": chunk,
                         "timestamp": timestamp.isoformat(),
                     },
                 )
 
     def context_agent(self, query: str, top_results_num: int) -> List[str]:
+        if not self.chroma_client:
+            self.chroma_client = self.initialize_chroma_client()
+            self.collection = self.get_or_create_collection()
         count = self.collection.count()
         if count == 0:
             return []
         results = self.collection.query(
             query_texts=query,
             n_results=min(top_results_num, count),
             include=["metadatas"],
@@ -106,46 +119,54 @@
             ),
             reverse=True,
         )
 
         context = [item["result"] for item in sorted_results]
         trimmed_context = self.trim_context(context)
         print(f"CONTEXT: {trimmed_context}")
-        return "\n".join(trimmed_context)
+        context_str = "\n".join(trimmed_context)
+        response = f"Context: {context_str}\n\n"
+        return response
 
     def trim_context(self, context: List[str]) -> List[str]:
+        if not self.nlp:
+            self.load_spacy_model()
         trimmed_context = []
         total_tokens = 0
         for item in context:
             item_tokens = len(self.nlp(item))
             if total_tokens + item_tokens <= self.chunk_size:
                 trimmed_context.append(item)
                 total_tokens += item_tokens
             else:
                 break
         return trimmed_context
 
     def get_keywords(self, query: str):
         """Extract keywords from a query using Spacy's part-of-speech tagging."""
+        if not self.nlp:
+            self.load_spacy_model()
         doc = self.nlp(query)
         keywords = [
             token.text for token in doc if token.pos_ in {"NOUN", "PROPN", "VERB"}
         ]
         return set(keywords)
 
     def score_chunk(self, chunk: str, keywords: set):
         """Score a chunk based on the number of query keywords it contains."""
         chunk_counter = Counter(chunk.split())
         score = sum(chunk_counter[keyword] for keyword in keywords)
         return score
 
     def chunk_content(self, content: str, query: str, overlap: int = 2) -> List[str]:
-        content_chunks = []
+        if not self.nlp:
+            self.load_spacy_model()
         doc = self.nlp(content)
         sentences = list(doc.sents)
+        content_chunks = []
         chunk = []
         chunk_len = 0
         keywords = self.get_keywords(query)
 
         for i, sentence in enumerate(sentences):
             sentence_tokens = len(sentence)
             if chunk_len + sentence_tokens > self.chunk_size and chunk:
```

### Comparing `agixt-1.1.71b0/agixt/Tasks.py` & `agixt-1.1.72b0/agixt/Tasks.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,242 +1,184 @@
 from AGiXT import AGiXT
 import re
 import os
 import json
-import uuid
 import yaml
-import time
-from pathlib import Path
 from Agent import Agent
 from collections import deque
-from typing import List, Dict
 
 
 class Tasks:
     def __init__(self, agent_name: str = "AGiXT"):
         self.agent_name = agent_name
-        self.agent = Agent(self.agent_name)
+        self.ai = AGiXT(self.agent_name)
         self.primary_objective = None
         self.task_list = deque([])
         self.output_list = []
         self.stop_running_event = False
 
-    def save_task(self):
-        task_name = re.sub(
-            r"[^\w\s]", "", self.primary_objective
-        )  # remove non-alphanumeric & non-space characters
-        task_name = task_name[:15]  # truncate to 15 characters
-
-        # ensure the directories exist
-        directory = Path(f"agents/{self.agent_name}")
-        directory.mkdir(parents=True, exist_ok=True)
-
-        # serialize the task state and save to a file
-        task_state = {
-            "task_name": task_name,
-            "task_list": list(self.task_list),
-            "output_list": self.output_list,
-            "primary_objective": self.primary_objective,
-        }
-        with open(f"agents/{self.agent_name}/{task_name}.yaml", "w") as f:
-            yaml.dump(task_state, f)
-
-    def load_task(self, task_name):
-        task_name = re.sub(
-            r"[^\w\s]", "", task_name
-        )  # remove non-alphanumeric & non-space characters
-        task_name = task_name[:15]  # truncate to 15 characters
-
+    def load_task(self):
+        out_file = re.sub(r"[^\w\s]", "", self.primary_objective)
+        out_file = out_file[:25]
         try:
-            with open(f"agents/{self.agent_name}/{task_name}.json", "r") as f:
+            with open(f"agents/{self.agent_name}/{out_file}.json", "r") as f:
                 task_state = json.load(f)
 
             self.task_list = deque(task_state["task_list"])
-            self.output_list = task_state["output_list"]
+            self.output_list = task_state["tasks"]
             self.primary_objective = task_state["primary_objective"]
-            print(f"Successfully loaded task '{task_name}'.")
+            print(f"Successfully loaded task '{out_file}'.")
 
         except FileNotFoundError:
-            print(f"No saved task found with the name '{task_name}'.")
+            print(f"No saved task found with the name '{out_file}'.")
         except Exception as e:
             print(f"An error occurred while loading the task: {e}")
 
     def get_status(self):
         if self.task_list:
             return True
         else:
             return False
 
-    def get_output_list(self):
-        return self.output_list
-
-    def save_task_output(self, agent_name, task_output):
-        # Check if agents/{agent_name}/tasks/task_name.txt exists
-        # If it does, append to it
-        # If it doesn't, create it
-        if "tasks" not in os.listdir(os.path.join("agents", agent_name)):
-            os.makedirs(os.path.join("agents", agent_name, "tasks"))
-        if self.primary_objective is None:
-            self.primary_objective = str(uuid.uuid4())
-        task_output_file = os.path.join(
-            "agents", agent_name, "tasks", f"{self.primary_objective}.yaml"
+    def update_task(self, task_id, task_name, task_output):
+        # Check if the task exists at agents/{agent_name}/tasks/{self.primary_objective}.json
+        # We need to stip out symbols except spaces in primary objective and truncate the primary objective to 15 characters
+        out_file = re.sub(r"[^\w\s]", "", self.primary_objective)
+        out_file = out_file[:25]
+        output_file = os.path.join(
+            "agents", self.agent_name, "tasks", f"{out_file}.json"
+        )
+        if os.path.exists(output_file):
+            # If it does, load it
+            with open(output_file, "r") as f:
+                data = json.load(f)
+        else:
+            # If it doesn't, create it
+            data = {
+                "primary_objective": self.primary_objective,
+                "task_list": list(self.task_list),
+                "tasks": [],
+            }
+        # Check if task is in the data["tasks"] list
+        data["tasks"].append(
+            {
+                "task_id": task_id,
+                "task_name": task_name,
+                "task_output": task_output,
+            }
         )
-        with open(
-            task_output_file,
-            "a" if os.path.exists(task_output_file) else "w",
-            encoding="utf-8",
-        ) as f:
-            yaml.dump(task_output, f)
-        return task_output
+        # Save the data to agents/{agent_name}/tasks/{self.primary_objective}.json
+        with open(output_file, "w") as f:
+            json.dump(data, f)
+        return data
 
     def get_task_output(self):
-        task_name = re.sub(
-            r"[^\w\s]", "", self.primary_objective
-        )  # remove non-alphanumeric & non-space characters
-        task_name = task_name[:15]  # truncate to 15 characters
-
+        out_file = re.sub(r"[^\w\s]", "", self.primary_objective)
+        out_file = out_file[:25]
         try:
-            with open(f"agents/{self.agent_name}/tasks/{task_name}.yaml", "r") as f:
-                task_output = yaml.safe_load(f)
+            with open(f"agents/{self.agent_name}/tasks/{out_file}.json", "r") as f:
+                task_output = json.load(f)
 
-            print(f"Successfully loaded task output for '{task_name}'.")
+            print(f"Successfully loaded task output for '{out_file}'.")
             return task_output
 
         except FileNotFoundError:
-            print(f"No saved task output found with the name '{task_name}'.")
+            print(f"No saved task output found with the name '{out_file}'.")
             return None
         except Exception as e:
             print(f"An error occurred while loading the task output: {e}")
             return None
 
-    def update_output_list(self, output):
-        print(self.save_task_output(self.agent_name, output))
+    def get_tasks_files(self):
+        files = os.listdir(os.path.join("agents", self.agent_name, "tasks"))
+        files = [file[:-5] for file in files]
+        return files
 
     def stop_tasks(self):
         if self.stop_running_event is not None:
             self.stop_running_event = True
         self.task_list.clear()
 
-    def task_agent(self, result: Dict, task_description: str, task_list) -> List[Dict]:
-        tasks = [task["task_name"] for task in task_list]
-        if len(tasks) == 0:
-            return []
-        task_list = ", ".join(tasks)
-
-        response = AGiXT(self.agent_name).run(
-            task=self.primary_objective,
-            prompt="task",
-            result=result,
-            task_description=task_description,
-            tasks=task_list,
-        )
-        if response == None:
-            time.sleep(5)
-            return self.task_agent(result, task_description, task_list)
-        lines = response.split("\n") if "\n" in response else [response]
-        new_tasks = []
-        for line in lines:
-            match = re.match(r"(\d+)\.\s+(.*)", line)
-            if match:
-                task_id, task_name = match.groups()
-                new_tasks.append(
-                    {"task_id": int(task_id), "task_name": task_name.strip()}
-                )
-
-        return new_tasks  # This line will return the list of new tasks
-
     def instruction_agent(self, task, **kwargs):
         if "task_name" in task:
             task = task["task_name"]
 
-        resolver = AGiXT(self.agent_name).run(
+        resolver = self.ai.run(
             task=task,
             prompt="SmartInstruct-StepByStep"
             if self.primary_objective is None
             else "SmartTask-StepByStep",
             context_results=6,
             objective=self.primary_objective,
             **kwargs,
         )
-        execution_response = AGiXT(self.agent_name).run(
-            task=task,
-            prompt="SmartInstruct-Execution"
-            if self.primary_objective is None
-            else "SmartTask-Execution",
-            previous_response=resolver,
-            objective=self.primary_objective,
-            **kwargs,
-        )
-        return (
-            f"RESPONSE:\n{resolver}\n\nCommand Execution Response{execution_response}"
-        )
+        # Check if agent has commands before trying to run execution agent
+        if Agent(self.agent_name).get_commands_string() != None:
+            execution_response = self.ai.run(
+                task=task,
+                prompt="SmartInstruct-Execution"
+                if self.primary_objective is None
+                else "SmartTask-Execution",
+                previous_response=resolver,
+                objective=self.primary_objective,
+                **kwargs,
+            )
+            return f"RESPONSE:\n{resolver}\n\nCommand Execution Response{execution_response}"
+        else:
+            return f"RESPONSE:\n{resolver}"
 
     def run_task(
         self,
-        objective,
+        objective: str = "",
         async_exec: bool = False,
         smart: bool = False,
         load_task: str = "",
         **kwargs,
     ):
-        self.primary_objective = objective
+        initial_task = "Break down the objective into a list of small achievable tasks in the form of instructions that lead up to achieving the ultimate goal of the objective."
         if load_task != "":
             self.load_task(load_task)
-            self.update_output_list(f"Loaded task '{load_task}'.\n\n")
+            print(f"Loaded task '{load_task}'.\n\n")
         else:
-            if self.task_list == deque([]) or self.task_list == []:
-                self.task_list = deque(
-                    [
-                        {
-                            "task_id": 1,
-                            "task_name": "Develop a task list to complete the objective if necessary.  The plan is 'None' if not necessary.",
-                        }
-                    ]
-                )
-            self.update_output_list(
-                f"Starting task with objective: {self.primary_objective}.\n\n"
+            self.primary_objective = objective
+            self.task_list = deque(
+                [
+                    {
+                        "task_id": 1,
+                        "task_name": initial_task,
+                    }
+                ]
             )
+            print(f"Starting task with objective: {self.primary_objective}.\n\n")
 
-        while not self.stop_running_event and self.task_list:
+        while not self.stop_running_event and self.task_list != deque([]):
             task = self.task_list.popleft()
-
             if task["task_name"] in ["None", "None.", ""]:
                 self.stop_tasks()
                 continue
-
-            self.update_output_list(
-                f"\nExecuting task {task['task_id']}: {task['task_name']}\n"
-            )
-
+            print(f"\nExecuting task {task['task_id']}: {task['task_name']}\n")
             if smart != True:
                 result = self.instruction_agent(task=task["task_name"], **kwargs)
             else:
-                result = AGiXT(self.agent_name).smart_instruct(
+                result = self.ai.smart_instruct(
                     task=task["task_name"],
                     shots=3,
                     async_exec=async_exec,
                     objective=self.primary_objective,
                     **kwargs,
                 )
-
-            self.update_output_list(f"\nTask Result:\n\n{result}\n")
-
-            new_tasks = self.task_agent(
-                result=result,
-                task_description=task["task_name"],
-                task_list=self.task_list,
-            )
-
-            self.task_list = deque(new_tasks)
-
-            self.update_output_list(f"\nNew Tasks:\n\n{new_tasks}\n")
-
-            for new_task in new_tasks:
-                new_task_id = len(self.task_list) + 1
-                new_task.update({"task_id": new_task_id})
-                self.task_list.append(new_task)
-
+            self.update_task(task["task_id"], task["task_name"], result)
+            print(f"\nTask Result:\n\n{result}\n")
+            if task["task_name"] == initial_task:
+                lines = result.split("\n") if "\n" in result else [result]
+                new_tasks = []
+                for line in lines:
+                    match = re.match(r"(\d+)\.\s+(.*)", line)
+                    if match:
+                        task_id, task_name = match.groups()
+                        new_tasks.append(
+                            {"task_id": int(task_id), "task_name": task_name.strip()}
+                        )
+                self.task_list = deque(new_tasks)
         if not self.task_list:
             self.stop_tasks()
-        if self.stop_running_event:
-            self.save_task()
-        self.update_output_list("All tasks completed or stopped.")
+        print("All tasks completed or stopped.")
```

### Comparing `agixt-1.1.71b0/agixt/app.py` & `agixt-1.1.72b0/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/provider/__init__.py` & `agixt-1.1.72b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/provider/azure.py` & `agixt-1.1.72b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/provider/bing.py` & `agixt-1.1.72b0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/provider/chatgpt.py` & `agixt-1.1.72b0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/provider/claude.py` & `agixt-1.1.72b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/provider/fastchat.py` & `agixt-1.1.72b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/provider/gpt4all.py` & `agixt-1.1.72b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/provider/gpt4free.py` & `agixt-1.1.72b0/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/provider/gpugpt4all.py` & `agixt-1.1.72b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/provider/huggingchat.py` & `agixt-1.1.72b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/provider/kobold.py` & `agixt-1.1.72b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/provider/llamacpp.py` & `agixt-1.1.72b0/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/provider/llamacppapi.py` & `agixt-1.1.72b0/agixt/provider/llamacppapi.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/provider/oobabooga.py` & `agixt-1.1.72b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/provider/openai.py` & `agixt-1.1.72b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/provider/palm.py` & `agixt-1.1.72b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/provider/transformer.py` & `agixt-1.1.72b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt/requirements.txt` & `agixt-1.1.72b0/agixt/requirements.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt.egg-info/PKG-INFO` & `agixt-1.1.72b0/agixt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.71b0
+Version: 1.1.72b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.71b0/agixt.egg-info/SOURCES.txt` & `agixt-1.1.72b0/agixt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/agixt.egg-info/requires.txt` & `agixt-1.1.72b0/agixt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/docs/README.md` & `agixt-1.1.72b0/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.1.71b0/setup.py` & `agixt-1.1.72b0/setup.py`

 * *Files identical despite different names*

