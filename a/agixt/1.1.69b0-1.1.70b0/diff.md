# Comparing `tmp/agixt-1.1.69b0.tar.gz` & `tmp/agixt-1.1.70b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.69b0.tar", last modified: Tue May 23 21:09:42 2023, max compression
+gzip compressed data, was "agixt-1.1.70b0.tar", last modified: Wed May 24 01:38:33 2023, max compression
```

## Comparing `agixt-1.1.69b0.tar` & `agixt-1.1.70b0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:09:42.160518 agixt-1.1.69b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-23 21:09:29.000000 agixt-1.1.69b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-23 21:09:29.000000 agixt-1.1.69b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-23 21:09:42.156517 agixt-1.1.69b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:09:42.152517 agixt-1.1.69b0/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    16622 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/AGiXT.py
--rw-r--r--   0 runner    (1001) docker     (123)    14049 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/Commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/CustomPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/Main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/Tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:09:42.156517 agixt-1.1.69b0/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/provider/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/provider/llamacppapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 21:09:29.000000 agixt-1.1.69b0/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:09:42.152517 agixt-1.1.69b0/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-23 21:09:42.000000 agixt-1.1.69b0/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-23 21:09:42.000000 agixt-1.1.69b0/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:09:42.000000 agixt-1.1.69b0/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-23 21:09:42.000000 agixt-1.1.69b0/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 21:09:42.000000 agixt-1.1.69b0/agixt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:09:42.156517 agixt-1.1.69b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-23 21:09:29.000000 agixt-1.1.69b0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-23 21:09:29.000000 agixt-1.1.69b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 21:09:42.160518 agixt-1.1.69b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-23 21:09:29.000000 agixt-1.1.69b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:33.037639 agixt-1.1.70b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-24 01:38:19.000000 agixt-1.1.70b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-24 01:38:19.000000 agixt-1.1.70b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-24 01:38:33.037639 agixt-1.1.70b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:33.033639 agixt-1.1.70b0/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    16622 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/AGiXT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14049 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/Commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/CustomPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/Main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/Tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:33.037639 agixt-1.1.70b0/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/provider/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/provider/llamacppapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 01:38:19.000000 agixt-1.1.70b0/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:33.033639 agixt-1.1.70b0/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-24 01:38:33.000000 agixt-1.1.70b0/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-24 01:38:33.000000 agixt-1.1.70b0/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 01:38:33.000000 agixt-1.1.70b0/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-24 01:38:33.000000 agixt-1.1.70b0/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 01:38:33.000000 agixt-1.1.70b0/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:33.037639 agixt-1.1.70b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-24 01:38:19.000000 agixt-1.1.70b0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 01:38:19.000000 agixt-1.1.70b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 01:38:33.037639 agixt-1.1.70b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-24 01:38:19.000000 agixt-1.1.70b0/setup.py
```

### Comparing `agixt-1.1.69b0/LICENSE` & `agixt-1.1.70b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/PKG-INFO` & `agixt-1.1.70b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.69b0
+Version: 1.1.70b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.69b0/agixt/AGiXT.py` & `agixt-1.1.70b0/agixt/AGiXT.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/Agent.py` & `agixt-1.1.70b0/agixt/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/Chain.py` & `agixt-1.1.70b0/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/Commands.py` & `agixt-1.1.70b0/agixt/Commands.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/Config.py` & `agixt-1.1.70b0/agixt/Config.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/CustomPrompt.py` & `agixt-1.1.70b0/agixt/CustomPrompt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/Embedding.py` & `agixt-1.1.70b0/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/Main.py` & `agixt-1.1.70b0/agixt/Main.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/Memories.py` & `agixt-1.1.70b0/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/Tasks.py` & `agixt-1.1.70b0/agixt/Tasks.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/app.py` & `agixt-1.1.70b0/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/provider/__init__.py` & `agixt-1.1.70b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/provider/azure.py` & `agixt-1.1.70b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/provider/bing.py` & `agixt-1.1.70b0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/provider/chatgpt.py` & `agixt-1.1.70b0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/provider/claude.py` & `agixt-1.1.70b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/provider/fastchat.py` & `agixt-1.1.70b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/provider/gpt4all.py` & `agixt-1.1.70b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/provider/gpt4free.py` & `agixt-1.1.70b0/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/provider/gpugpt4all.py` & `agixt-1.1.70b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/provider/huggingchat.py` & `agixt-1.1.70b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/provider/kobold.py` & `agixt-1.1.70b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/provider/llamacpp.py` & `agixt-1.1.70b0/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/provider/llamacppapi.py` & `agixt-1.1.70b0/agixt/provider/llamacppapi.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/provider/oobabooga.py` & `agixt-1.1.70b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/provider/openai.py` & `agixt-1.1.70b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/provider/palm.py` & `agixt-1.1.70b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/provider/transformer.py` & `agixt-1.1.70b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt/requirements.txt` & `agixt-1.1.70b0/agixt/requirements.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt.egg-info/PKG-INFO` & `agixt-1.1.70b0/agixt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.69b0
+Version: 1.1.70b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.69b0/agixt.egg-info/SOURCES.txt` & `agixt-1.1.70b0/agixt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/agixt.egg-info/requires.txt` & `agixt-1.1.70b0/agixt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/docs/README.md` & `agixt-1.1.70b0/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.1.69b0/setup.py` & `agixt-1.1.70b0/setup.py`

 * *Files identical despite different names*

