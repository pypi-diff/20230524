# Comparing `tmp/shellgenius-0.1.4.tar.gz` & `tmp/shellgenius-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellgenius-0.1.4.tar", last modified: Thu May  4 18:34:41 2023, max compression
+gzip compressed data, was "shellgenius-0.1.5.tar", last modified: Tue May  9 15:23:27 2023, max compression
```

## Comparing `shellgenius-0.1.4.tar` & `shellgenius-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 18:34:41.834706 shellgenius-0.1.4/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-06 02:44:20.000000 shellgenius-0.1.4/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3368 2023-05-04 18:34:41.834706 shellgenius-0.1.4/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3235 2023-05-04 18:15:13.000000 shellgenius-0.1.4/README.md
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-05-04 18:34:41.834706 shellgenius-0.1.4/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-05-04 18:34:32.000000 shellgenius-0.1.4/setup.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 18:34:41.834706 shellgenius-0.1.4/shellgenius/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 13:06:06.000000 shellgenius-0.1.4/shellgenius/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3076 2023-05-04 18:34:00.000000 shellgenius-0.1.4/shellgenius/cli.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5522 2023-05-04 18:04:38.000000 shellgenius-0.1.4/shellgenius/gpt_integration.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 18:34:41.834706 shellgenius-0.1.4/shellgenius.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3368 2023-05-04 18:34:41.000000 shellgenius-0.1.4/shellgenius.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      312 2023-05-04 18:34:41.000000 shellgenius-0.1.4/shellgenius.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-05-04 18:34:41.000000 shellgenius-0.1.4/shellgenius.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-05-04 18:34:41.000000 shellgenius-0.1.4/shellgenius.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      341 2023-05-04 18:34:41.000000 shellgenius-0.1.4/shellgenius.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-05-04 18:34:41.000000 shellgenius-0.1.4/shellgenius.egg-info/top_level.txt
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-09 15:23:27.662842 shellgenius-0.1.5/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-06 02:44:20.000000 shellgenius-0.1.5/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3589 2023-05-09 15:23:27.662842 shellgenius-0.1.5/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3456 2023-05-07 14:10:31.000000 shellgenius-0.1.5/README.md
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-05-09 15:23:27.662842 shellgenius-0.1.5/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-05-09 15:22:46.000000 shellgenius-0.1.5/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-09 15:23:27.662842 shellgenius-0.1.5/shellgenius/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 13:06:06.000000 shellgenius-0.1.5/shellgenius/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3179 2023-05-09 15:21:52.000000 shellgenius-0.1.5/shellgenius/cli.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5499 2023-05-09 15:21:07.000000 shellgenius-0.1.5/shellgenius/gpt_integration.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-09 15:23:27.662842 shellgenius-0.1.5/shellgenius.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3589 2023-05-09 15:23:27.000000 shellgenius-0.1.5/shellgenius.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      312 2023-05-09 15:23:27.000000 shellgenius-0.1.5/shellgenius.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-05-09 15:23:27.000000 shellgenius-0.1.5/shellgenius.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-05-09 15:23:27.000000 shellgenius-0.1.5/shellgenius.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      341 2023-05-09 15:23:27.000000 shellgenius-0.1.5/shellgenius.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-05-09 15:23:27.000000 shellgenius-0.1.5/shellgenius.egg-info/top_level.txt
```

### Comparing `shellgenius-0.1.4/LICENSE` & `shellgenius-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shellgenius-0.1.4/PKG-INFO` & `shellgenius-0.1.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,14 @@
-Metadata-Version: 2.1
-Name: shellgenius
-Version: 0.1.4
-Author: sderev
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ShellGenius
 
 ShellGenius is an intuitive CLI tool designed to enhance your command-line experience by turning your task descriptions into efficient shell commands.
 
 Powered by OpenAI's gpt-3.5-turbo AI model, ShellGenius generates accurate commands based on your input and provides step-by-step explanations to help you understand the underlying logic.
 
-![ShellGenius Demo](assets/demo.gif)
+https://user-images.githubusercontent.com/24412384/236322725-435b92c6-6d33-421f-8662-7eb6355d3f64.mp4
 
 ## Table of Contents
 
 * [Installation](#installation)
 * [Usage](#usage)
 * [Examples](#examples)
 * [Limitations](#limitations)
@@ -23,20 +16,20 @@
 * [License](#license)
 
 ## Installation
 
 Ensure you have Python 3.8 or later installed on your system. To install ShellGenius, use the following command:
 
 ```bash
-pip install shellgenius
+python3 -m pip install shellgenius
 ```
 
 ### Install via `pipx` (recommended)
 
-`pipx` is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. I recommend using `pipx` to install VocabMaster.
+`pipx` is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. I recommend using `pipx` to install ShellGenius.
 
 **First, install `pipx` if you haven't already:**
 
 * On macOS and Linux:
 
   ```
   python3 -m pip install --user pipx
@@ -48,29 +41,37 @@
 * On Windows:
 
   ```
   py -m pip install --user pipx
   py -m pipx ensurepath
   ```
 
-**Once `pipx` is installed, you can install VocabMaster using the following command:**
+**Once `pipx` is installed, you can install ShellGenius using the following command:**
 
 ```
-pipx install vocabmaster
+pipx install shellgenius
 ```
 
 ### OpenAI API key
 
 ShellGenius requires an OpenAI API key to function. You can obtain a key by signing up for an account at [OpenAI's website](https://platform.openai.com/account/api-keys).
 
 Once you have your API key, set it as an environment variable:
 
-```bash
-export OPENAI_API_KEY="your-api-key-here"
-```
+* On macOS and Linux:
+
+  ```bash
+  export OPENAI_API_KEY="your-api-key-here"
+  ```
+
+* On Windows:
+
+  ```
+  setx OPENAI_API_KEY your_key
+  ```
 
 ## Usage
 
 To use ShellGenius, simply type `shellgenius` followed by a description of the task you want to perform:
 
 ```bash
 shellgenius "description of your task"
@@ -80,46 +81,51 @@
 
 The tool will generate a shell command based on your description, display it with an explanation, and prompt you to confirm if you want to execute the command.
 
 ## Examples
 
 Here are some examples of ShellGenius in action:
 
+### Create a file
+
 ```bash
 shellgenius "create a new file called example.txt"
 ```
 
 **Output:**
 
 ```markdown
 touch example.txt
 
 Explanation:
 * touch command is used to create a new file if it doesn't exist
 * example.txt is the name of the new file
 
-Be carefula with your answer.
+Be careful with your answer.
 Do you want to execute this command? [Y/n]: y
 ```
 ___
 
+### Number of lines in a file
+
 ```bash
 shellgenius "count the number of lines in a file called data.csv"
 ```
 
 **Output:**
 
-```
+```markdown
 wc -l data.csv
+
 Explanation:
 * wc is a word, line, and byte count utility
 * -l flag counts the number of lines
 * data.csv is the target file
 
-Be carefula with your answer.
+Be careful with your answer.
 Do you want to execute this command? [Y/n]: y
 ```
 
 ## Limitations
 
 ShellGenius is powered by an AI model and may not always generate the most efficient or accurate commands. Exercise caution when executing commands, especially when working with sensitive data or critical systems.
```

### Comparing `shellgenius-0.1.4/README.md` & `shellgenius-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,21 @@
+Metadata-Version: 2.1
+Name: shellgenius
+Version: 0.1.5
+Author: sderev
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ShellGenius
 
 ShellGenius is an intuitive CLI tool designed to enhance your command-line experience by turning your task descriptions into efficient shell commands.
 
 Powered by OpenAI's gpt-3.5-turbo AI model, ShellGenius generates accurate commands based on your input and provides step-by-step explanations to help you understand the underlying logic.
 
-![ShellGenius Demo](assets/demo.gif)
+https://user-images.githubusercontent.com/24412384/236322725-435b92c6-6d33-421f-8662-7eb6355d3f64.mp4
 
 ## Table of Contents
 
 * [Installation](#installation)
 * [Usage](#usage)
 * [Examples](#examples)
 * [Limitations](#limitations)
@@ -16,20 +23,20 @@
 * [License](#license)
 
 ## Installation
 
 Ensure you have Python 3.8 or later installed on your system. To install ShellGenius, use the following command:
 
 ```bash
-pip install shellgenius
+python3 -m pip install shellgenius
 ```
 
 ### Install via `pipx` (recommended)
 
-`pipx` is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. I recommend using `pipx` to install VocabMaster.
+`pipx` is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. I recommend using `pipx` to install ShellGenius.
 
 **First, install `pipx` if you haven't already:**
 
 * On macOS and Linux:
 
   ```
   python3 -m pip install --user pipx
@@ -41,29 +48,37 @@
 * On Windows:
 
   ```
   py -m pip install --user pipx
   py -m pipx ensurepath
   ```
 
-**Once `pipx` is installed, you can install VocabMaster using the following command:**
+**Once `pipx` is installed, you can install ShellGenius using the following command:**
 
 ```
-pipx install vocabmaster
+pipx install shellgenius
 ```
 
 ### OpenAI API key
 
 ShellGenius requires an OpenAI API key to function. You can obtain a key by signing up for an account at [OpenAI's website](https://platform.openai.com/account/api-keys).
 
 Once you have your API key, set it as an environment variable:
 
-```bash
-export OPENAI_API_KEY="your-api-key-here"
-```
+* On macOS and Linux:
+
+  ```bash
+  export OPENAI_API_KEY="your-api-key-here"
+  ```
+
+* On Windows:
+
+  ```
+  setx OPENAI_API_KEY your_key
+  ```
 
 ## Usage
 
 To use ShellGenius, simply type `shellgenius` followed by a description of the task you want to perform:
 
 ```bash
 shellgenius "description of your task"
@@ -73,46 +88,51 @@
 
 The tool will generate a shell command based on your description, display it with an explanation, and prompt you to confirm if you want to execute the command.
 
 ## Examples
 
 Here are some examples of ShellGenius in action:
 
+### Create a file
+
 ```bash
 shellgenius "create a new file called example.txt"
 ```
 
 **Output:**
 
 ```markdown
 touch example.txt
 
 Explanation:
 * touch command is used to create a new file if it doesn't exist
 * example.txt is the name of the new file
 
-Be carefula with your answer.
+Be careful with your answer.
 Do you want to execute this command? [Y/n]: y
 ```
 ___
 
+### Number of lines in a file
+
 ```bash
 shellgenius "count the number of lines in a file called data.csv"
 ```
 
 **Output:**
 
-```
+```markdown
 wc -l data.csv
+
 Explanation:
 * wc is a word, line, and byte count utility
 * -l flag counts the number of lines
 * data.csv is the target file
 
-Be carefula with your answer.
+Be careful with your answer.
 Do you want to execute this command? [Y/n]: y
 ```
 
 ## Limitations
 
 ShellGenius is powered by an AI model and may not always generate the most efficient or accurate commands. Exercise caution when executing commands, especially when working with sensitive data or critical systems.
```

### Comparing `shellgenius-0.1.4/setup.py` & `shellgenius-0.1.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = file.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as file:
     requirements = [line.strip() for line in file]
 
 setup(
     name="shellgenius",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "shellgenius = shellgenius.cli:shellgenius",
         ]
     },
```

### Comparing `shellgenius-0.1.4/shellgenius/cli.py` & `shellgenius-0.1.5/shellgenius/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         
     * rich_markdown_callback(chunk: str) -> None
         Update the live markdown display with the received chunk of text from the gpt-3.5-turbo AI
         API.
 """
 import re
 import subprocess
+import platform
 import click
 from rich.console import Console
 from rich.markdown import Markdown
 from rich.live import Live
 from .gpt_integration import format_prompt, chatgpt_request
 
 
@@ -68,15 +69,16 @@
         Do you want to execute this command? [Y/n]: y
     """
     if not command_description:
         click.echo(ctx.get_help())
         return
 
     command_description = " ".join(command_description)
-    prompt = format_prompt(command_description)
+    os_name = "macOS" if platform.system() == "Darwin" else platform.system()
+    prompt = format_prompt(command_description, os_name)
     click.echo()
 
     with live:
         generated_text = chatgpt_request(
             prompt,
             stream=True,
             chunk_callback=rich_markdown_callback,
```

### Comparing `shellgenius-0.1.4/shellgenius/gpt_integration.py` & `shellgenius-0.1.5/shellgenius/gpt_integration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import os
 import openai
 import tiktoken
 import time
 
 
-def format_prompt(command_description):
+def format_prompt(command_description, os_name):
     prompt = [
         {
             "role": "system",
-            "content": (
-                "You are an expert in using Unix-like OS and the shell terminal."
-            ),
+            "content": f"You are an expert in using {os_name} and the shell terminal.",
         },
         {
             "role": "user",
             "content": f"""
-            I will give you a brief description of something I want to achieve in a Unix-like shell.
+            I will give you a brief description of something I want to achieve in a {os_name} shell.
             I want you to answer with the command that matches the result I want to produce.
             The first line of your answer will be the said shell command.
             Then, I want you to explain it step by step with a bullet list.
 
             This is very important:
             * In absolutely no circumstance you are allowed to start your message by anything but the shell command. 
 
@@ -70,18 +68,18 @@
 
         # Iterate through the stream of events
         for chunk in response:
             collected_chunks.append(chunk)  # save the event response
             chunk_message = chunk["choices"][0]["delta"]  # extract the message
             collected_messages.append(chunk_message)  # save the message
 
-            if chunk_callback: # call the callback with the chunk message
+            if chunk_callback:  # call the callback with the chunk message
                 chunk_callback(chunk_message.get("content", ""))
             # print(chunk_message.get("content", ""), end="")  # stream the message
-        #print()
+        # print()
         response = collected_chunks
 
         # Save the time delay and text received
         response_time = (time.monotonic_ns() - start_time) / 1e9
         generated_text = "".join([m.get("content", "") for m in collected_messages])
 
     else:
```

### Comparing `shellgenius-0.1.4/shellgenius.egg-info/PKG-INFO` & `shellgenius-0.1.5/shellgenius.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: shellgenius
-Version: 0.1.4
+Version: 0.1.5
 Author: sderev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ShellGenius
 
 ShellGenius is an intuitive CLI tool designed to enhance your command-line experience by turning your task descriptions into efficient shell commands.
 
 Powered by OpenAI's gpt-3.5-turbo AI model, ShellGenius generates accurate commands based on your input and provides step-by-step explanations to help you understand the underlying logic.
 
-![ShellGenius Demo](assets/demo.gif)
+https://user-images.githubusercontent.com/24412384/236322725-435b92c6-6d33-421f-8662-7eb6355d3f64.mp4
 
 ## Table of Contents
 
 * [Installation](#installation)
 * [Usage](#usage)
 * [Examples](#examples)
 * [Limitations](#limitations)
@@ -23,20 +23,20 @@
 * [License](#license)
 
 ## Installation
 
 Ensure you have Python 3.8 or later installed on your system. To install ShellGenius, use the following command:
 
 ```bash
-pip install shellgenius
+python3 -m pip install shellgenius
 ```
 
 ### Install via `pipx` (recommended)
 
-`pipx` is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. I recommend using `pipx` to install VocabMaster.
+`pipx` is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. I recommend using `pipx` to install ShellGenius.
 
 **First, install `pipx` if you haven't already:**
 
 * On macOS and Linux:
 
   ```
   python3 -m pip install --user pipx
@@ -48,29 +48,37 @@
 * On Windows:
 
   ```
   py -m pip install --user pipx
   py -m pipx ensurepath
   ```
 
-**Once `pipx` is installed, you can install VocabMaster using the following command:**
+**Once `pipx` is installed, you can install ShellGenius using the following command:**
 
 ```
-pipx install vocabmaster
+pipx install shellgenius
 ```
 
 ### OpenAI API key
 
 ShellGenius requires an OpenAI API key to function. You can obtain a key by signing up for an account at [OpenAI's website](https://platform.openai.com/account/api-keys).
 
 Once you have your API key, set it as an environment variable:
 
-```bash
-export OPENAI_API_KEY="your-api-key-here"
-```
+* On macOS and Linux:
+
+  ```bash
+  export OPENAI_API_KEY="your-api-key-here"
+  ```
+
+* On Windows:
+
+  ```
+  setx OPENAI_API_KEY your_key
+  ```
 
 ## Usage
 
 To use ShellGenius, simply type `shellgenius` followed by a description of the task you want to perform:
 
 ```bash
 shellgenius "description of your task"
@@ -80,46 +88,51 @@
 
 The tool will generate a shell command based on your description, display it with an explanation, and prompt you to confirm if you want to execute the command.
 
 ## Examples
 
 Here are some examples of ShellGenius in action:
 
+### Create a file
+
 ```bash
 shellgenius "create a new file called example.txt"
 ```
 
 **Output:**
 
 ```markdown
 touch example.txt
 
 Explanation:
 * touch command is used to create a new file if it doesn't exist
 * example.txt is the name of the new file
 
-Be carefula with your answer.
+Be careful with your answer.
 Do you want to execute this command? [Y/n]: y
 ```
 ___
 
+### Number of lines in a file
+
 ```bash
 shellgenius "count the number of lines in a file called data.csv"
 ```
 
 **Output:**
 
-```
+```markdown
 wc -l data.csv
+
 Explanation:
 * wc is a word, line, and byte count utility
 * -l flag counts the number of lines
 * data.csv is the target file
 
-Be carefula with your answer.
+Be careful with your answer.
 Do you want to execute this command? [Y/n]: y
 ```
 
 ## Limitations
 
 ShellGenius is powered by an AI model and may not always generate the most efficient or accurate commands. Exercise caution when executing commands, especially when working with sensitive data or critical systems.
```

