# Comparing `tmp/llmo-0.2.2.tar.gz` & `tmp/llmo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmo-0.2.2.tar", last modified: Tue May 23 04:56:57 2023, max compression
+gzip compressed data, was "llmo-0.3.0.tar", last modified: Wed May 24 03:21:59 2023, max compression
```

## Comparing `llmo-0.2.2.tar` & `llmo-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.2.2/LICENSE
--rw-r--r--   0        0        0     2134 2023-05-22 08:06:19.890271 llmo-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.2.2/llmo/__init__.py
--rw-r--r--   0        0        0     2898 2023-05-22 22:11:47.649149 llmo-0.2.2/llmo/cli.py
--rw-r--r--   0        0        0      122 2023-05-22 21:51:03.475865 llmo-0.2.2/llmo/constants.py
--rw-r--r--   0        0        0     9793 2023-05-23 03:53:39.625867 llmo-0.2.2/llmo/gui.py
--rw-r--r--   0        0        0      341 2023-05-23 03:17:45.469101 llmo-0.2.2/llmo/layout.css
--rw-r--r--   0        0        0     5982 2023-05-23 03:45:21.644631 llmo-0.2.2/llmo/llms.py
--rw-r--r--   0        0        0     1593 2023-05-23 04:53:16.585981 llmo-0.2.2/llmo/shell_mode.py
--rw-r--r--   0        0        0      699 2023-05-23 04:56:57.394313 llmo-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      838 2023-05-22 22:24:34.139710 llmo-0.2.2/tests/test_openai.py
--rw-r--r--   0        0        0     2479 1970-01-01 00:00:00.000000 llmo-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2134 2023-05-22 08:06:19.890271 llmo-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.3.0/llmo/__init__.py
+-rw-r--r--   0        0        0     2961 2023-05-24 03:21:31.439301 llmo-0.3.0/llmo/cli.py
+-rw-r--r--   0        0        0      122 2023-05-22 21:51:03.475865 llmo-0.3.0/llmo/constants.py
+-rw-r--r--   0        0        0     9793 2023-05-23 03:53:39.625867 llmo-0.3.0/llmo/gui.py
+-rw-r--r--   0        0        0      341 2023-05-23 03:17:45.469101 llmo-0.3.0/llmo/layout.css
+-rw-r--r--   0        0        0     5982 2023-05-23 03:45:21.644631 llmo-0.3.0/llmo/llms.py
+-rw-r--r--   0        0        0     1593 2023-05-23 04:53:16.585981 llmo-0.3.0/llmo/shell_mode.py
+-rw-r--r--   0        0        0      699 2023-05-24 03:21:59.296374 llmo-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      838 2023-05-22 22:24:34.139710 llmo-0.3.0/tests/test_openai.py
+-rw-r--r--   0        0        0     2479 1970-01-01 00:00:00.000000 llmo-0.3.0/PKG-INFO
```

### Comparing `llmo-0.2.2/LICENSE` & `llmo-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmo-0.2.2/README.md` & `llmo-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `llmo-0.2.2/llmo/cli.py` & `llmo-0.3.0/llmo/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -96,18 +96,19 @@
         max_tokens=args.max_tokens,
     )
 
     if args.personality:
         openai_client.add_personality()
 
     if args.shell_mode:
+        files = [Path(f) for f in args.files] if args.files else []
         run_shell_mode(
             openai_client,
             prompt=args.prompt,
-            files=args.files,
+            files=files,
             rich_text_mode=args.rich_text_mode,
         )
     else:
         app = LLMO(
             prompt=args.prompt,
             staged_files=staged_files,
             llm_client=openai_client,
```

### Comparing `llmo-0.2.2/llmo/gui.py` & `llmo-0.3.0/llmo/gui.py`

 * *Files identical despite different names*

### Comparing `llmo-0.2.2/llmo/llms.py` & `llmo-0.3.0/llmo/llms.py`

 * *Files identical despite different names*

### Comparing `llmo-0.2.2/llmo/shell_mode.py` & `llmo-0.3.0/llmo/shell_mode.py`

 * *Files identical despite different names*

### Comparing `llmo-0.2.2/pyproject.toml` & `llmo-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llmo"
-version = "0.2.2"
+version = "0.3.0"
 description = "AI pair programmer"
 authors = [
     { name = "Stephan Fitzpatrick", email = "stephan@knowsuchagency.com" },
 ]
 dependencies = [
     "textual>=0.26.0",
     "openai>=0.27.6",
```

### Comparing `llmo-0.2.2/tests/test_openai.py` & `llmo-0.3.0/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `llmo-0.2.2/PKG-INFO` & `llmo-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmo
-Version: 0.2.2
+Version: 0.3.0
 Summary: AI pair programmer
 Author-Email: Stephan Fitzpatrick <stephan@knowsuchagency.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/knowsuchagency/llmo
 Requires-Python: >=3.10
 Requires-Dist: textual>=0.26.0
 Requires-Dist: openai>=0.27.6
```

