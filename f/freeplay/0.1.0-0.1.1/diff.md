# Comparing `tmp/freeplay-0.1.0.tar.gz` & `tmp/freeplay-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeplay-0.1.0.tar", max compression
+gzip compressed data, was "freeplay-0.1.1.tar", max compression
```

## Comparing `freeplay-0.1.0.tar` & `freeplay-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-18 13:19:32.515553 freeplay-0.1.0/README.md
--rw-r--r--   0        0        0       62 2023-04-24 20:37:56.560899 freeplay-0.1.0/freeplay/__init__.py
--rw-r--r--   0        0        0     1089 2023-05-17 18:18:52.582428 freeplay-0.1.0/freeplay/api_support.py
--rw-r--r--   0        0        0     2379 2023-05-09 21:11:51.812943 freeplay-0.1.0/freeplay/freeplay.py
--rw-r--r--   0        0        0      350 2023-05-18 13:18:14.883965 freeplay-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 freeplay-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-18 13:19:32.515553 freeplay-0.1.1/README.md
+-rw-r--r--   0        0        0       62 2023-05-18 23:25:20.631072 freeplay-0.1.1/freeplay/__init__.py
+-rw-r--r--   0        0        0     1089 2023-05-18 23:25:20.631179 freeplay-0.1.1/freeplay/api_support.py
+-rw-r--r--   0        0        0     3030 2023-05-23 20:52:35.454357 freeplay-0.1.1/freeplay/freeplay.py
+-rw-r--r--   0        0        0      350 2023-05-23 20:52:35.455138 freeplay-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 freeplay-0.1.1/PKG-INFO
```

### Comparing `freeplay-0.1.0/freeplay/api_support.py` & `freeplay-0.1.1/freeplay/api_support.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.0/freeplay/freeplay.py` & `freeplay-0.1.1/freeplay/freeplay.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,34 +4,56 @@
 
 from . import api_support
 
 T = t.TypeVar("T")
 
 
 @dataclass
+class ChatMessage:
+    role: str
+    content: str
+
+    def format(self, **kwargs: str) -> dict[str, str]:
+        return {
+            'role': self.role,
+            'content': self.content.format(**kwargs)
+        }
+
+
+@dataclass
 class FreePlayPromptTemplate:
     name: str
     content: str
+    messages: list[ChatMessage]
 
 
 @dataclass
 class FreePlayProjectSession:
     session_id: str
     prompt_templates: list[FreePlayPromptTemplate]
 
     def __all_names(self) -> list[str]:
         return [t.name for t in self.prompt_templates]
 
-    def get_template(self, template_name: str) -> str:
-        for t in self.prompt_templates:
-            if t.name == template_name:
-                return t.content
+    def __find_template(self, template_name: str) -> FreePlayPromptTemplate:
+        for template in self.prompt_templates:
+            if template.name == template_name:
+                return template
 
         raise Exception(f'Template with name {template_name} not found. Available names are: {self.__all_names()}')
 
+    def get_template(self, template_name: str) -> str:
+        return self.__find_template(template_name).content
+
+    def get_formatted_chat_messages(self, template_name: str, **kwargs: str) -> list[dict[str, str]]:
+        return [
+            message.format(**kwargs)
+            for message in self.__find_template(template_name).messages
+        ]
+
 
 @dataclass
 class FreePlayTestRunRecord:
     project_id: str
     test_run_id: str
     input_collection: list[dict[str, str]]
```

### Comparing `freeplay-0.1.0/PKG-INFO` & `freeplay-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeplay
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: FreePlay Engineering
 Author-email: engineering@freeplay.ai
 Requires-Python: >=3.7,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

