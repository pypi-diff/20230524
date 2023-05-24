# Comparing `tmp/coder_coder-0.2.0.tar.gz` & `tmp/coder_coder-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coder_coder-0.2.0.tar", max compression
+gzip compressed data, was "coder_coder-0.2.1.tar", max compression
```

## Comparing `coder_coder-0.2.0.tar` & `coder_coder-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      591 2023-05-07 00:14:21.467321 coder_coder-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-28 01:18:29.778418 coder_coder-0.2.0/coder_coder/__init__.py
--rw-r--r--   0        0        0     8845 2023-05-06 17:09:20.222938 coder_coder-0.2.0/coder_coder/cli.py
--rw-r--r--   0        0        0     1399 2023-05-06 01:03:12.267329 coder_coder-0.2.0/coder_coder/content.py
--rw-r--r--   0        0        0     3614 2023-05-06 20:44:18.429199 coder_coder-0.2.0/coder_coder/main.py
--rw-r--r--   0        0        0      543 2023-05-07 00:34:26.571293 coder_coder-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1287 1970-01-01 00:00:00.000000 coder_coder-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-05-07 00:14:21.467321 coder_coder-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 01:18:29.778418 coder_coder-0.2.1/coder_coder/__init__.py
+-rw-r--r--   0        0        0     8845 2023-05-06 17:09:20.222938 coder_coder-0.2.1/coder_coder/cli.py
+-rw-r--r--   0        0        0     1399 2023-05-06 01:03:12.267329 coder_coder-0.2.1/coder_coder/content.py
+-rw-r--r--   0        0        0     3547 2023-05-24 00:41:50.132273 coder_coder-0.2.1/coder_coder/main.py
+-rw-r--r--   0        0        0      472 2023-05-24 00:44:37.144179 coder_coder-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1150 1970-01-01 00:00:00.000000 coder_coder-0.2.1/PKG-INFO
```

### Comparing `coder_coder-0.2.0/README.md` & `coder_coder-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `coder_coder-0.2.0/coder_coder/cli.py` & `coder_coder-0.2.1/coder_coder/cli.py`

 * *Files identical despite different names*

### Comparing `coder_coder-0.2.0/coder_coder/content.py` & `coder_coder-0.2.1/coder_coder/content.py`

 * *Files identical despite different names*

### Comparing `coder_coder-0.2.0/coder_coder/main.py` & `coder_coder-0.2.1/coder_coder/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,50 +1,47 @@
 import json
-import os
 from pathlib import Path
-from typing import Optional, Any
+from textwrap import dedent
+from typing import Optional
 
 import typer
 
 import openai
-from dotenv import load_dotenv
 
 coder_env = Path.home() / ".coder_code"
 if not coder_env.exists():
     coder_env.mkdir()
 
 
 def load_config():
     config_file = coder_env / "config.json"
     if config_file.exists():
         with open(config_file, "r") as f:
             config = json.load(f)
     else:
         config = {"text_model": "gpt-4"}
-    for k, v in config.items():
-        os.environ[k] = v
     return config
 
 def save_config(config):
     config_file = coder_env / "config.json"
     with open(config_file, "w") as f:
         json.dump(config, f)
 
 
 CONFIG = load_config()
-openai.api_key = os.environ["OPENAI_API_KEY"]
-openai.organization = os.environ["OPENAI_ORG_ID"]
+openai.api_key = CONFIG.get("OPENAI_API_KEY")
+openai.organization = CONFIG.get("OPENAI_ORG_ID")
 
 app = typer.Typer()
 
 
 @app.callback()
 def callback():
     """
-    Awesome Portal Gun
+    Coder Coder
     """
 
 
 @app.command()
 def code(user_prompt: str = typer.Argument(...),
          out_file: Optional[str] = typer.Option(None),
          in_file: Optional[str] = typer.Option(None)):
@@ -77,17 +74,17 @@
     typer.echo(text_response)
 
 
 @app.command()
 def plan(user_prompt: str = typer.Argument(...),
          out_file: Optional[str] = typer.Option(None)):
     typer.echo(f"Planning: {user_prompt}")
-    prompt = f"""
-Develop a plan for the following goal: {user_prompt}
-"""
+    prompt = dedent(f"""
+    Develop a plan for the following goal: {user_prompt}
+    """)
     completion = openai.ChatCompletion.create(model=CONFIG["text_model"], messages=[{"role": "user", "content": prompt}])
     text_response = completion.choices[0].message.content
     typer.echo(text_response)
     if out_file:
         with open(out_file, "w") as f:
             f.write(text_response)
```

### Comparing `coder_coder-0.2.0/PKG-INFO` & `coder_coder-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: coder-coder
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Kevin Fortier
 Author-email: kevin.r.fortier@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: install (>=1.3.5,<2.0.0)
 Requires-Dist: openai (>=0.27.5,<0.28.0)
 Requires-Dist: pip (>=23.1.2,<24.0.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: s3fs (>=2023.4.0,<2024.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # Coder-Coder
 Coder-Coder is a commandline tool that facilitates coding with GPT-4.
 
 ## Installation
```

