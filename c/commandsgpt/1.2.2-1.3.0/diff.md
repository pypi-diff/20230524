# Comparing `tmp/commandsgpt-1.2.2.tar.gz` & `tmp/commandsgpt-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commandsgpt-1.2.2.tar", last modified: Sat May 13 18:51:29 2023, max compression
+gzip compressed data, was "commandsgpt-1.3.0.tar", last modified: Wed May 24 21:55:06 2023, max compression
```

## Comparing `commandsgpt-1.2.2.tar` & `commandsgpt-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 18:51:29.596086 commandsgpt-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-13 18:51:16.000000 commandsgpt-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-05-13 18:51:29.596086 commandsgpt-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-13 18:51:16.000000 commandsgpt-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 18:51:29.592086 commandsgpt-1.2.2/commands_gpt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 18:51:29.592086 commandsgpt-1.2.2/commands_gpt/commands_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 18:51:16.000000 commandsgpt-1.2.2/commands_gpt/commands_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-13 18:51:16.000000 commandsgpt-1.2.2/commands_gpt/commands_gpt/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 18:51:29.592086 commandsgpt-1.2.2/commands_gpt/commands_gpt/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 18:51:16.000000 commandsgpt-1.2.2/commands_gpt/commands_gpt/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-13 18:51:16.000000 commandsgpt-1.2.2/commands_gpt/commands_gpt/commands/commands_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-05-13 18:51:16.000000 commandsgpt-1.2.2/commands_gpt/commands_gpt/commands/graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-13 18:51:16.000000 commandsgpt-1.2.2/commands_gpt/commands_gpt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-05-13 18:51:16.000000 commandsgpt-1.2.2/commands_gpt/commands_gpt/instruction_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-13 18:51:16.000000 commandsgpt-1.2.2/commands_gpt/commands_gpt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-13 18:51:16.000000 commandsgpt-1.2.2/commands_gpt/commands_gpt/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-13 18:51:16.000000 commandsgpt-1.2.2/commands_gpt/commands_gpt/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 18:51:29.596086 commandsgpt-1.2.2/commands_gpt/commandsgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-05-13 18:51:29.000000 commandsgpt-1.2.2/commands_gpt/commandsgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-13 18:51:29.000000 commandsgpt-1.2.2/commands_gpt/commandsgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 18:51:29.000000 commandsgpt-1.2.2/commands_gpt/commandsgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-13 18:51:29.000000 commandsgpt-1.2.2/commands_gpt/commandsgpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-13 18:51:16.000000 commandsgpt-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-13 18:51:29.596086 commandsgpt-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:55:06.625001 commandsgpt-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-05-24 21:55:06.625001 commandsgpt-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:55:06.621001 commandsgpt-1.3.0/commands_gpt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:55:06.621001 commandsgpt-1.3.0/commands_gpt/commands_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/commands_gpt/commands_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/commands_gpt/commands_gpt/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:55:06.621001 commandsgpt-1.3.0/commands_gpt/commands_gpt/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/commands_gpt/commands_gpt/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/commands_gpt/commands_gpt/commands/commands_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/commands_gpt/commands_gpt/commands/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/commands_gpt/commands_gpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/commands_gpt/commands_gpt/instruction_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/commands_gpt/commands_gpt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/commands_gpt/commands_gpt/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:55:06.625001 commandsgpt-1.3.0/commands_gpt/commandsgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-05-24 21:55:06.000000 commandsgpt-1.3.0/commands_gpt/commandsgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-24 21:55:06.000000 commandsgpt-1.3.0/commands_gpt/commandsgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 21:55:06.000000 commandsgpt-1.3.0/commands_gpt/commandsgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 21:55:06.000000 commandsgpt-1.3.0/commands_gpt/commandsgpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-24 21:55:06.625001 commandsgpt-1.3.0/setup.cfg
```

### Comparing `commandsgpt-1.2.2/LICENSE` & `commandsgpt-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.2.2/PKG-INFO` & `commandsgpt-1.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commandsgpt
-Version: 1.2.2
+Version: 1.3.0
 Summary: An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 Home-page: https://github.com/AlexisAndradeDev/CommandsGPT
 Author: Martín Alexis Martínez Andrade
 Author-email: alexis.martinez.contacto@gmail.com
 Project-URL: Bug Tracker, https://github.com/AlexisAndradeDev/CommandsGPT/issues
 Project-URL: repository, https://github.com/AlexisAndradeDev/CommandsGPT
 Classifier: License :: OSI Approved :: BSD License
@@ -18,42 +18,43 @@
 
 An implementation of GPT-4 to recognize instructions. It recognizes which commands it must run to fulfill the user's instruction, using a graph where each node is a command and the data generated by each command can be passed to other commands.
 
 Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 
 # Installation
 
-Install the `commandsgpt` module.
+* Install the `commandsgpt` module.
 
 ```
 pip install commandsgpt
 ```
 
 If you're using a virtual environment:
 ```
 pipenv install commandsgpt
 ```
 
-You also have to install the OpenAI package:
+* You also have to install the OpenAI package:
 
 ```
 pip install openai
 ```
 
 or
 
 ```
 pipenv install openai
 ```
 
-# Basic usage
+* Set an environment variable OPENAI_API_KEY to store your OpenAI key.
 
-Create a `commands` dictionary that will store the commands described in natural language. Create the functions that will be called when the commands are executed (they must match the arguments and return values of the `commands` dict; the first parameter of these functions must be a Config object). Create a `command_name_to_func` dictionary that will take the name of a command and return the corresponding function.
+# Usage
+
+Create a `commands` dictionary that will store the commands described in natural language. 
 
-*Example of commands dictionary*
 ```python
 commands = {
     "REQUEST_USER_INPUT": {
         "description": "Asks the user to input data through the interface.",
         "arguments": {
             "message": {"description": "Message displayed to the user related to the data that will be requested (example: 'Enter your age').", "type": "string"},
         },
@@ -61,78 +62,93 @@
             "input": {"description": "Data entered by the user", "type": "string"},
         },
     },
     ...
 }
 ```
 
+Now, create the functions that will be called when the commands are executed.
+
+* The name of the function is irrelevant.
+* The first parameter must be the Config object; the second one must be the Graph object. Normally, you won't work directly with these objects, so you don't have to worry about them. Just use them as the first two parameters.
+* The following parameters must match those described in the commands dictionary (name and data type).
+* The return value must be a dictionary. Its keys, values and data types must match the return values described in the commands dictionary.
+
 *Example of a command function*
+
 ```python
+from commands_gpt.config import Config
+from commands_gpt.commands.graphs import Graph
+
 def request_user_input_command(config: Config, graph: Graph, message: str) -> dict[str, Any]:
     input_ = input(f"{message}\n*: ")
     results = {
         "input": input_,
     }
     return results
 ```
 
+Create a `command_name_to_func` dictionary that will take the name of a command and return the corresponding function.
+
 *Example of command_name_to_func dictionary*
 ```python
 command_name_to_func = {
     "REQUEST_USER_INPUT": request_user_input_command,
     ...
 }
 ```
 
 Add the ***essential commands*** to your commands dictionaries.
 * These are the default commands that implement core logic to the model's thinking, like an IF command.
-* If you already defined your own core logic commands (IF command, THINK command, etc.), then you are free not to use them.
+* If you already defined your own core logic commands (IF command, THINK command, CALCULATE command, etc.), then you are free not to use them.
 
 ```python
 from commands_gpt.commands.commands_funcs import add_essential_commands
 add_essential_commands(commands, command_name_to_func)
 ```
 
 Your `config` object:
 ```python
 # keyword arguments are optional
-config = Config("gpt-4-0314", verbosity=1, explain_graph=True)
+config = Config("gpt-4-0314", verbosity=1, explain_graph=True, save_graph_as_file=False)
 ```
 
 Create an instruction:
 
 ```python
 instruction = input("Enter your instruction: ")
 ```
 
 Pass your instruction to the recognizer model:
 
 ```python
 graph = recognize_instruction_and_create_graph(
     instruction, config.chat_model, commands, command_name_to_func,
-    verbosity=config.verbosity,
+    verbosity=config.verbosity, save_graph_as_file=config.save_graph_as_file
 )
 ```
 
 Finally, execute the graph of commands:
 
 ```python
 graph.execute_commands(config)
 ```
 
-# Basic example
+# Example
+
+Create two files: `custom_commands.py` and `main.py`.
+
+## custom_commands.py
 
 ```python
 from typing import Any
 from pathlib import Path
-from commands_gpt.instruction_recognition import recognize_instruction_and_create_graph
-from commands_gpt.commands.graphs import execute_commands
-from commands_gpt.config import Config
 
-# Commands Natural Language Dict
+from commands_gpt.config import Config
+from commands_gpt.commands.graphs import Graph
 
 commands = {
     "WRITE_TO_USER": {
         "description": "Writes something to the interface to communicate with the user.",
         "arguments": {
             "content": {"description": "Content to write.", "type": "string"},
         },
@@ -151,23 +167,31 @@
         "description": "Write a file.",
         "arguments": {
             "content": {"description": "Content that will be written.", "type": "string"},
             "file_path": {"description": "Complete path of the file that will be written.", "type": "string"},
         },
         "generates_data": {},
     },
+    "CONCATENATE_STRINGS": {
+        "description": "Concatenates two strings. \"Hello\" and \"World\": \"HelloWorld\"",
+        "arguments": {
+            "str1": {"description": "String 1.", "type": "string"},
+            "str2": {"description": "String 2.", "type": "string"},
+            "sep": {"description": "Separator between the strs. Ex: \"\\n\", \",\", \"\".", "type": "string"},
+        },
+        "generates_data": {
+            "concatenated": {"description": "Concatenated string.", "type": "str"},
+        },
+    },
 }
 
 # Commands functions
 
 def write_to_user_command(config: Config, graph: Graph, content: str) -> dict[str, Any]:
-    # add newlines because regex data injection replaces newline characters
-    # by \\n substrings.
-    content_with_newlines = "\n".join(content.split("\\n"))
-    print(f">>> {content_with_newlines}")
+    print(f">>> {content}")
     return {}
 
 def request_user_input_command(config: Config, graph: Graph, message: str) -> dict[str, Any]:
     input_ = input(f"{message}\n*: ")
     results = {
         "input": input_,
     }
@@ -177,136 +201,52 @@
     file_dir = Path(file_path).parent
     assert file_dir.exists(), f"Container directory '{file_dir}' does not exist."
     with open(file_path, "w+", encoding="utf-8") as f:
         f.write(content)
         f.close()
     return {}
 
-# Command name to function dict
+def concatenate_strings_command(config: Config, graph: Graph, str1: str, 
+        str2: str, sep: str) -> dict[str, Any]:
+    concatenated = f"{sep}".join((str1, str2))
+    results = {
+        "concatenated": concatenated,
+    }
+    return results
+
+# add your functions here
 command_name_to_func = {
     "WRITE_TO_USER": write_to_user_command,
     "REQUEST_USER_INPUT": request_user_input_command,
     "WRITE_FILE": write_file_command,
+    "CONCATENATE_STRINGS": concatenate_strings_command,
 }
+```
+
+## main.py
+```python
+from commands_gpt.instruction_recognition import recognize_instruction_and_create_graph
+from commands_gpt.config import Config
+from custom_commands import commands, command_name_to_func
 
 from commands_gpt.commands.commands_funcs import add_essential_commands
 add_essential_commands(commands, command_name_to_func)
 
 chat_model = "gpt-4-0314"
 
-config = Config(chat_model, verbosity=1, explain_graph=True)
+config = Config(chat_model, verbosity=2, explain_graph=False, save_graph_as_file=False)
 
 instruction = input("Enter your prompt: ")
 graph = recognize_instruction_and_create_graph(
     instruction, config.chat_model, commands, command_name_to_func,
-    verbosity=config.verbosity,
+    verbosity=config.verbosity, save_graph_as_file=config.save_graph_as_file
 )
 graph.execute_commands(config)
 ```
 
-# Adding custom commands
-
-You can add and modify your own custom commands by creating two dictionaries:
-
-* commands: The commands that the model can use, described in natural language. The keys are the name of the commands, and the values are dictionaries.
-
-    * The nested dictionaries have keys *description*, *arguments* and *generates_data*.
-
-    * **description**: Description of the command in natural language.
-
-    * **arguments**: Arguments that the function of the command receives. It's a dictionary which keys are the names of the arguments, and the values are dictionaries that describe the arguments. 
-
-        * The nested dictionaries have keys *description* and *type*.
-        * **description**: Description of the argument in natural language.
-
-
-        * **type**: Data type. E.g.: "string", "boolean", "int".
-
-    * **generates_data**: The data generated by the command that other commands will be able to access. It's a dictionary which keys are the names of the data field, and the values are dictionaries that describe the data field.
-
-        * The nested dictionaries have keys *description* and *type*.
-
-        * **description**: Description of the data field in natural language.
-
-        * **type**: Data type. E.g.: "string", "boolean", "int".
-
-***Example***
-```python
-commands = {
-    "WRITE_TO_USER": {
-        "description": "Writes something to the interface to communicate with the user.",
-        "arguments": {
-            "content": {"description": "Content to write.", "type": "string"},
-        },
-        "generates_data": {},
-    },
-    "REQUEST_USER_INPUT": {
-        "description": "Asks the user to input data through the interface.",
-        "arguments": {
-            "message": {"description": "Message displayed to the user related to the data that will be requested (example: 'Enter your age').", "type": "string"},
-        },
-        "generates_data": {
-            "input": {"description": "Data entered by the user", "type": "string"},
-        },
-    },
-    "WRITE_FILE": {
-        "description": "Write a file.",
-        "arguments": {
-            "content": {"description": "Content that will be written.", "type": "string"},
-            "file_path": {"description": "Complete path of the file that will be written.", "type": "string"},
-        },
-        "generates_data": {},
-    },
-}
-```
-
-* command_name_to_func: The keys of this dictionary are the name of the commands, and the values are the function.
-
-    * The name of the function is irrelevant.
-
-    * The first argument must be the Config object. The second argument is the Graph object.
-
-    * The arguments must match the arguments from the commands dictionary.
-
-    * The return value must be a dictionary which keys must match the "generates_data" key.
-
-    * The data types must match the ones declared in the commands dictionary.
-
-***Example***
-```python
-def write_to_user_command(config: Config, graph: Graph, content: str) -> dict[str, Any]:
-    # add newlines because regex data injection replaces newline characters
-    # by \\n substrings.
-    content_with_newlines = "\n".join(content.split("\\n"))
-    print(f">>> {content_with_newlines}")
-    return {}
-
-def request_user_input_command(config: Config, graph: Graph, message: str) -> dict[str, Any]:
-    input_ = input(f"{message}\n*: ")
-    results = {
-        "input": input_,
-    }
-    return results
-
-def write_file_command(config: Config, graph: Graph, content: str, file_path: str) -> dict[str, Any]:
-    file_dir = Path(file_path).parent
-    assert file_dir.exists(), f"Container directory '{file_dir}' does not exist."
-    with open(file_path, "w+", encoding="utf-8") as f:
-        f.write(content)
-        f.close()
-    return {}
-
-# add your functions here
-command_name_to_func = {
-    "WRITE_TO_USER": write_to_user_command,
-    "REQUEST_USER_INPUT": request_user_input_command,
-    "WRITE_FILE": write_file_command,
-}
-```
-
 Copyright (c) 2023, Martín Alexis Martínez Andrade.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
```

### Comparing `commandsgpt-1.2.2/README.md` & `commandsgpt-1.3.0/commands_gpt/commandsgpt.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,60 @@
+Metadata-Version: 2.1
+Name: commandsgpt
+Version: 1.3.0
+Summary: An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
+Home-page: https://github.com/AlexisAndradeDev/CommandsGPT
+Author: Martín Alexis Martínez Andrade
+Author-email: alexis.martinez.contacto@gmail.com
+Project-URL: Bug Tracker, https://github.com/AlexisAndradeDev/CommandsGPT/issues
+Project-URL: repository, https://github.com/AlexisAndradeDev/CommandsGPT
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # CommandsGPT
 
 An implementation of GPT-4 to recognize instructions. It recognizes which commands it must run to fulfill the user's instruction, using a graph where each node is a command and the data generated by each command can be passed to other commands.
 
 Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 
 # Installation
 
-Install the `commandsgpt` module.
+* Install the `commandsgpt` module.
 
 ```
 pip install commandsgpt
 ```
 
 If you're using a virtual environment:
 ```
 pipenv install commandsgpt
 ```
 
-You also have to install the OpenAI package:
+* You also have to install the OpenAI package:
 
 ```
 pip install openai
 ```
 
 or
 
 ```
 pipenv install openai
 ```
 
-# Basic usage
+* Set an environment variable OPENAI_API_KEY to store your OpenAI key.
+
+# Usage
 
-Create a `commands` dictionary that will store the commands described in natural language. Create the functions that will be called when the commands are executed (they must match the arguments and return values of the `commands` dict; the first parameter of these functions must be a Config object). Create a `command_name_to_func` dictionary that will take the name of a command and return the corresponding function.
+Create a `commands` dictionary that will store the commands described in natural language. 
 
-*Example of commands dictionary*
 ```python
 commands = {
     "REQUEST_USER_INPUT": {
         "description": "Asks the user to input data through the interface.",
         "arguments": {
             "message": {"description": "Message displayed to the user related to the data that will be requested (example: 'Enter your age').", "type": "string"},
         },
@@ -45,78 +62,93 @@
             "input": {"description": "Data entered by the user", "type": "string"},
         },
     },
     ...
 }
 ```
 
+Now, create the functions that will be called when the commands are executed.
+
+* The name of the function is irrelevant.
+* The first parameter must be the Config object; the second one must be the Graph object. Normally, you won't work directly with these objects, so you don't have to worry about them. Just use them as the first two parameters.
+* The following parameters must match those described in the commands dictionary (name and data type).
+* The return value must be a dictionary. Its keys, values and data types must match the return values described in the commands dictionary.
+
 *Example of a command function*
+
 ```python
+from commands_gpt.config import Config
+from commands_gpt.commands.graphs import Graph
+
 def request_user_input_command(config: Config, graph: Graph, message: str) -> dict[str, Any]:
     input_ = input(f"{message}\n*: ")
     results = {
         "input": input_,
     }
     return results
 ```
 
+Create a `command_name_to_func` dictionary that will take the name of a command and return the corresponding function.
+
 *Example of command_name_to_func dictionary*
 ```python
 command_name_to_func = {
     "REQUEST_USER_INPUT": request_user_input_command,
     ...
 }
 ```
 
 Add the ***essential commands*** to your commands dictionaries.
 * These are the default commands that implement core logic to the model's thinking, like an IF command.
-* If you already defined your own core logic commands (IF command, THINK command, etc.), then you are free not to use them.
+* If you already defined your own core logic commands (IF command, THINK command, CALCULATE command, etc.), then you are free not to use them.
 
 ```python
 from commands_gpt.commands.commands_funcs import add_essential_commands
 add_essential_commands(commands, command_name_to_func)
 ```
 
 Your `config` object:
 ```python
 # keyword arguments are optional
-config = Config("gpt-4-0314", verbosity=1, explain_graph=True)
+config = Config("gpt-4-0314", verbosity=1, explain_graph=True, save_graph_as_file=False)
 ```
 
 Create an instruction:
 
 ```python
 instruction = input("Enter your instruction: ")
 ```
 
 Pass your instruction to the recognizer model:
 
 ```python
 graph = recognize_instruction_and_create_graph(
     instruction, config.chat_model, commands, command_name_to_func,
-    verbosity=config.verbosity,
+    verbosity=config.verbosity, save_graph_as_file=config.save_graph_as_file
 )
 ```
 
 Finally, execute the graph of commands:
 
 ```python
 graph.execute_commands(config)
 ```
 
-# Basic example
+# Example
+
+Create two files: `custom_commands.py` and `main.py`.
+
+## custom_commands.py
 
 ```python
 from typing import Any
 from pathlib import Path
-from commands_gpt.instruction_recognition import recognize_instruction_and_create_graph
-from commands_gpt.commands.graphs import execute_commands
-from commands_gpt.config import Config
 
-# Commands Natural Language Dict
+from commands_gpt.config import Config
+from commands_gpt.commands.graphs import Graph
 
 commands = {
     "WRITE_TO_USER": {
         "description": "Writes something to the interface to communicate with the user.",
         "arguments": {
             "content": {"description": "Content to write.", "type": "string"},
         },
@@ -135,23 +167,31 @@
         "description": "Write a file.",
         "arguments": {
             "content": {"description": "Content that will be written.", "type": "string"},
             "file_path": {"description": "Complete path of the file that will be written.", "type": "string"},
         },
         "generates_data": {},
     },
+    "CONCATENATE_STRINGS": {
+        "description": "Concatenates two strings. \"Hello\" and \"World\": \"HelloWorld\"",
+        "arguments": {
+            "str1": {"description": "String 1.", "type": "string"},
+            "str2": {"description": "String 2.", "type": "string"},
+            "sep": {"description": "Separator between the strs. Ex: \"\\n\", \",\", \"\".", "type": "string"},
+        },
+        "generates_data": {
+            "concatenated": {"description": "Concatenated string.", "type": "str"},
+        },
+    },
 }
 
 # Commands functions
 
 def write_to_user_command(config: Config, graph: Graph, content: str) -> dict[str, Any]:
-    # add newlines because regex data injection replaces newline characters
-    # by \\n substrings.
-    content_with_newlines = "\n".join(content.split("\\n"))
-    print(f">>> {content_with_newlines}")
+    print(f">>> {content}")
     return {}
 
 def request_user_input_command(config: Config, graph: Graph, message: str) -> dict[str, Any]:
     input_ = input(f"{message}\n*: ")
     results = {
         "input": input_,
     }
@@ -161,128 +201,69 @@
     file_dir = Path(file_path).parent
     assert file_dir.exists(), f"Container directory '{file_dir}' does not exist."
     with open(file_path, "w+", encoding="utf-8") as f:
         f.write(content)
         f.close()
     return {}
 
-# Command name to function dict
+def concatenate_strings_command(config: Config, graph: Graph, str1: str, 
+        str2: str, sep: str) -> dict[str, Any]:
+    concatenated = f"{sep}".join((str1, str2))
+    results = {
+        "concatenated": concatenated,
+    }
+    return results
+
+# add your functions here
 command_name_to_func = {
     "WRITE_TO_USER": write_to_user_command,
     "REQUEST_USER_INPUT": request_user_input_command,
     "WRITE_FILE": write_file_command,
+    "CONCATENATE_STRINGS": concatenate_strings_command,
 }
+```
+
+## main.py
+```python
+from commands_gpt.instruction_recognition import recognize_instruction_and_create_graph
+from commands_gpt.config import Config
+from custom_commands import commands, command_name_to_func
 
 from commands_gpt.commands.commands_funcs import add_essential_commands
 add_essential_commands(commands, command_name_to_func)
 
 chat_model = "gpt-4-0314"
 
-config = Config(chat_model, verbosity=1, explain_graph=True)
+config = Config(chat_model, verbosity=2, explain_graph=False, save_graph_as_file=False)
 
 instruction = input("Enter your prompt: ")
 graph = recognize_instruction_and_create_graph(
     instruction, config.chat_model, commands, command_name_to_func,
-    verbosity=config.verbosity,
+    verbosity=config.verbosity, save_graph_as_file=config.save_graph_as_file
 )
 graph.execute_commands(config)
 ```
 
-# Adding custom commands
-
-You can add and modify your own custom commands by creating two dictionaries:
-
-* commands: The commands that the model can use, described in natural language. The keys are the name of the commands, and the values are dictionaries.
-
-    * The nested dictionaries have keys *description*, *arguments* and *generates_data*.
-
-    * **description**: Description of the command in natural language.
-
-    * **arguments**: Arguments that the function of the command receives. It's a dictionary which keys are the names of the arguments, and the values are dictionaries that describe the arguments. 
-
-        * The nested dictionaries have keys *description* and *type*.
-        * **description**: Description of the argument in natural language.
-
-
-        * **type**: Data type. E.g.: "string", "boolean", "int".
-
-    * **generates_data**: The data generated by the command that other commands will be able to access. It's a dictionary which keys are the names of the data field, and the values are dictionaries that describe the data field.
-
-        * The nested dictionaries have keys *description* and *type*.
-
-        * **description**: Description of the data field in natural language.
+Copyright (c) 2023, Martín Alexis Martínez Andrade.
+All rights reserved.
 
-        * **type**: Data type. E.g.: "string", "boolean", "int".
-
-***Example***
-```python
-commands = {
-    "WRITE_TO_USER": {
-        "description": "Writes something to the interface to communicate with the user.",
-        "arguments": {
-            "content": {"description": "Content to write.", "type": "string"},
-        },
-        "generates_data": {},
-    },
-    "REQUEST_USER_INPUT": {
-        "description": "Asks the user to input data through the interface.",
-        "arguments": {
-            "message": {"description": "Message displayed to the user related to the data that will be requested (example: 'Enter your age').", "type": "string"},
-        },
-        "generates_data": {
-            "input": {"description": "Data entered by the user", "type": "string"},
-        },
-    },
-    "WRITE_FILE": {
-        "description": "Write a file.",
-        "arguments": {
-            "content": {"description": "Content that will be written.", "type": "string"},
-            "file_path": {"description": "Complete path of the file that will be written.", "type": "string"},
-        },
-        "generates_data": {},
-    },
-}
-```
-
-* command_name_to_func: The keys of this dictionary are the name of the commands, and the values are the function.
-
-    * The name of the function is irrelevant.
-
-    * The first argument must be the Config object. The second argument is the Graph object.
-
-    * The arguments must match the arguments from the commands dictionary.
-
-    * The return value must be a dictionary which keys must match the "generates_data" key.
-
-    * The data types must match the ones declared in the commands dictionary.
-
-***Example***
-```python
-def write_to_user_command(config: Config, graph: Graph, content: str) -> dict[str, Any]:
-    # add newlines because regex data injection replaces newline characters
-    # by \\n substrings.
-    content_with_newlines = "\n".join(content.split("\\n"))
-    print(f">>> {content_with_newlines}")
-    return {}
-
-def request_user_input_command(config: Config, graph: Graph, message: str) -> dict[str, Any]:
-    input_ = input(f"{message}\n*: ")
-    results = {
-        "input": input_,
-    }
-    return results
-
-def write_file_command(config: Config, graph: Graph, content: str, file_path: str) -> dict[str, Any]:
-    file_dir = Path(file_path).parent
-    assert file_dir.exists(), f"Container directory '{file_dir}' does not exist."
-    with open(file_path, "w+", encoding="utf-8") as f:
-        f.write(content)
-        f.close()
-    return {}
-
-# add your functions here
-command_name_to_func = {
-    "WRITE_TO_USER": write_to_user_command,
-    "REQUEST_USER_INPUT": request_user_input_command,
-    "WRITE_FILE": write_file_command,
-}
-```
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are
+met:
+
+    * Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+
+    * Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+
+    * Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
+A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
+OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
+SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
+LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
+THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `commandsgpt-1.2.2/commands_gpt/commands_gpt/commands/commands_funcs.py` & `commandsgpt-1.3.0/commands_gpt/commands_gpt/commands/commands_funcs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Callable
 
 from ..chat import get_answer_from_model
 from ..config import Config
 from .graphs import Graph
+from ..util.math_expr import safe_eval_math_expr
 
 ESSENTIAL_COMMANDS = {
     "THINK": {
         "description": "Generates a thought in your 'mind' without writing it down yet. This command allows you to create new ideas, reflect, and analyze information. For example, when asked to 'Write a three-paragraph article about Lenz's Law,' you would first use this command to generate the article and then use another to write it.",
         "arguments": {
             "about": {"description": "What to think about. Example: 'Three-paragraph article about Lenz's Law.'", "type": "string"},
         },
@@ -19,14 +20,23 @@
         "arguments": {
             "condition": {"description": "Condition. Can be in natural language.", "type": "string"},
         },
         "generates_data": {
             "result": {"description": "Result of the condition: 0 or 1.", "type": "boolean"},
         },
     },
+    "CALCULATE": {
+        "description": "Evaluates a mathematical expression in a str. Supports +, -, *, /, %, **, //. Can be entered in natural language.",
+        "arguments": {
+            "expression": {"description": "Math expression. '(-1) ** (1/2)', 'Negative one raised to 1/2.'", "type": "string"},
+        },
+        "generates_data": {
+            "result": {"description": "Result of evaluation", "type": "int or float or complex"},
+        },
+    },
     # TODO: Create a FOR command to increment a counter variable
 }
 
 # Commands functions
 # Must be named 'LowercaseCommandName_command'
 # The first argument must be the Config object, followed by the Graph object
 # The arguments must match the arguments from the ESSENTIAL_COMMANDS dictionary
@@ -62,14 +72,33 @@
         raise e
 
     results = {
         "result": result,
     }
     return results
 
+def calculate_command(config: Config, graph: Graph, expression: str) -> dict[str, Any]:
+    try:
+        result = safe_eval_math_expr(expression)
+    except ValueError:
+        # TODO: convert from natural language to math expression
+        messages = [
+            {
+                "role": "system",
+                "content": f"You are a model that takes a math expression in natural language and returns JUST the math expression, without any words. 'Negative one raised to the 1/2 plus eight' -> '(-1) ** (1/2) + 8'"
+            }
+        ]
+        expression_ = get_answer_from_model(expression, config.chat_model, messages)
+        result = safe_eval_math_expr(expression_)
+
+    results = {
+        "result": result,
+    }
+    return results
+
 ESSENTIAL_COMMAND_NAME_TO_COMMAND_FUNC = {
     key: eval(f"{key.lower()}_command")
     for key in ESSENTIAL_COMMANDS
 }
 
 def get_command(command_name: str) -> Callable:
     """
```

### Comparing `commandsgpt-1.2.2/commands_gpt/commands_gpt/instruction_recognition.py` & `commandsgpt-1.3.0/commands_gpt/commands_gpt/instruction_recognition.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,133 +1,124 @@
-import openai
 from typing import Callable
 
-from .static import StaticVar
 from .commands.graphs import Graph
+from .chat import get_answer_from_model
 
 def recognize_instruction(instruction: str, model: str, commands: dict, 
-        verbosity: int = 0) -> StaticVar:
+        verbosity: int = 0):
     """
     Analyzes an instruction and creates data to create a graph of commands
     that will fulfill the instruction.
 
     Args:
         instruction (str): The user's instruction.
         model (str): Name of the model.
         commands (dict): The commands that the model can use, described in
             natural language.
         verbosity (int): Level of detail printed by the function.
 
     Returns:
-        a StaticVar of string: commands data (the answer from the instruction recognition model).
+        a string: commands data (the answer from the instruction recognition model).
     """
     messages = [
         {
         'role': 'system', 
         'content':
             """You are a tool that, based on the user's prompt, detects the series of commands that must be executed, arguments that each command will have, and the relationship between each command (for example, what data generated by a command will be used as an argument for another)."""
             """\n*IMPORTANT*: *WRITE in the LANGUAGE that the USER writes his/her prompt in*."""
             """\n*IMPORTANT*: You can ONLY use the given commands. **NEVER try to use OTHERS**."""
+            """\n*IMPORTANT*: While creating the graph, you are NOT talking to the user. You are JUST CREATING THE GRAPH, so do not write suggestions for a user inside of the graph. Create the complete graph by your own."""
 
             f"""\n\nCommands:\n{commands}"""
 
             """\n\nDepending on the prompt, you will use different commands and different arguments and relationships between commands. The only way you can see data generated by other commands from a command is by passing them as arguments."""
 
             """\n\n*Your response will have this format, ALWAYS stick to it*:"""
-            """\n[[command_id, "COMMAND_NAME", {"arg1": value1, "arg2": value2, ...}, [[next_command_id, "dependent_on_data", required_value], [...], ...]], [...]]"""
+            """\n[command_id, "COMMAND_NAME", {"arg1": value1, "arg2": value2, ...}, [[next_command_id, "dependent_on_data", required_value], [...], ...]]"""
+            """\n[...]"""
+            """\n\nThe structure is JSON-Lines-like (so, use double quotes to create str, etc.)"""
+            """\nONLY use newline characters to separate the data of each node (as it's a JSON-Lines-like format)."""
             """\nYou will replace EVERYTHING in the format with the correct data."""
-            """\nTo reference data generated by a command, use __&i.data__. 'i' is the ID of the command; 'data' is the name of the generated data, and works like a Python value (if it's a list, you can use __&i.data[i]__, __&i.data[i:j]__, etc.; in a dictionary, __&i.data["key"]__, etc.)."""
+            """\nTo reference data generated by a command, use __&i.data__. 'i' is the ID of the command; 'data' is the name of the generated data."""
+            """\nAlways consider the DATA TYPE of the data you are referencing."""
             """\nYou can ONLY reference data in the arguments of the nodes."""
-            """\nThe structure will ultimately be like a graph. The next_command_id defines which command will be executed next; dependent_on_data is the name of the data generated by the current command which will be used as a condition (null if the next command will be executed no matter what the results of the current command where), and required_value is what value the dependent_on_data must have to execute the next command (null if dependent_on_data was also null)."""
+            """\nThe structure will ultimately be like a graph. The next_command_id defines which command will be executed next; dependent_on_data is the name of the data generated by the current command which will be used as a condition (*null if the next command will be executed no matter what the results of the current command where*), and required_value is what value the dependent_on_data must have to execute the next command (null if dependent_on_data was also null)."""
             """\nNote that dependent_on_data is NOT a data reference for the next command; it's just what will be used as a CONDITION to determine if the next command will be executed."""
+            """\ndependent_on_data field CAN NOT be 'dependent_on_data'. It must be null if it doesn't matter."""
             """\nA command can execute multiple next commands."""
             """\nBe concise but *solid* with the structure."""
             """\n*Consider that the user might write incorrectly and their inputs might be ambiguous*."""
             """\nThe only way to reference the data of other commands is by using the __&i.data__ referencing. Commands DO NOT KNOW each other's data."""
             """\nProvide all the relevant context in the arguments of the commands, so that you're not ambiguous."""
+            """\nNote that each command DOES NOT know about the other commands. You have to use DATA REFERENCES as ARGUMENTS to pass context."""
             """\nBe creative and logic when using the commands' arguments and data references."""
 
             """\n\nFor example:"""
 
             """\n\nExample 1:"""
             """\nUser prompt: 'Write an article about Lenz's Law, copy it to my clipboard and save it as a file.'"""
-            """\nYour response might be: '[[1, "%s", {"about": "Article about Lenz's Law"}, [[2, null, null]]], [2, "%s", {"content": "__&1.thought__"}, [[3, null, null]]], [3, "%s", {"content": "__&1.thought__", "file_name": "Article about Lenz's Law"}, []]]'""" % ("THINK", "WRITE_CLIPBOARD", "WRITE_FILE")
-            +
+            """\nYour response might be: '[1, "THINK", {"about": "Article about Lenz's Law"}, [[2, null, null]]]\n[2, "WRITE_CLIPBOARD", {"content": "__&1.thought__"}, [[3, null, null]]]\n[3, "WRITE_FILE", {"content": "__&1.thought__", "file_name": "Article about Lenz's Law"}, []]'"""
             """\n\nExample 2:"""
             """\nUser prompt: 'Read my clipboard, write a scientific article about the content in it, and save it as a file with a name related to the article.'"""
-            """\nYour response might be: '[[1, "%s", {}, [[1, null, null]]], [2, "%s", {"about": "Scientific article about __&1.content__"}, [[3, null, null]]], [3, "%s", {"about": "Name including extension to save a file about this article: __&2.thought__"}, [[4, null, null]]], [4, "%s", {"content": "__&2.thought__", "file_name": "__&3.thought__"}, []]]'""" % ("READ_CLIPBOARD", "THINK", "THINK", "WRITE_FILE")
-            +
+            """\nYour response might be: '[1, "READ_CLIPBOARD", {}, [[2, null, null]]]\n[2, "THINK", {"about": "Scientific article about __&1.content__"}, [[3, null, null]]]\n[3, "THINK", {"about": "Name including extension to save a file about this article: __&2.thought__"}, [[4, null, null]]]\n[4, "WRITE_FILE", {"content": "__&2.thought__", "file_name": "__&3.thought__"}, []]'"""
             """\n\nExample 3:"""
             """\nUser prompt: 'Look up the best courses on ASP.Net on Google and show me the first page that appears, if it is relevant.'"""
-            """\nYour response might be: '[[1, "%s", {"query": "best courses on ASP.Net"}, [[2, null, null]]], [2, "%s", {"url": "__&1.urls[0]__"}, [[3, null, null]]], [3, "%s", {"condition": "Is this a relevant course on ASP.Net? __&2.text__"}, [[4, "result", 1], [5, "result", 0]]], [4, "%s", {"content": "Relevant course: __&1.urls[0]__"}, []], [5, "%s", {"content": "It is not relevant."}, []]]'""" % ("SEARCH_GOOGLE", "READ_WEBPAGE", "IF", "WRITE_TO_USER", "WRITE_TO_USER")
-            +
-
-            """\n\nThe structure is JSON-like (so, use double quotes to create str, etc.)"""
+            """\nYour response might be: '[1, "SEARCH_GOOGLE", {"query": "best courses on ASP.Net"}, [[2, null, null]]]\n[2, "READ_WEBPAGE", {"url": "__&1.urls[0]__"}, [[3, null, null]]]\n[3, "IF", {"condition": "Is this a relevant course on ASP.Net? __&2.text__"}, [[4, "result", 1], [5, "result", 0]]]\n[4, "WRITE_TO_USER", {"content": "Relevant course: __&1.urls[0]__"}, []]\n[5, "WRITE_TO_USER", {"content": "It is not relevant."}, []]'"""
         }
     ]
-    messages.append({"role": "user", "content": instruction})
     print(f"Input tokens used by messages (graph creation): ~{len(str(messages)) / 4} tokens.")
 
-    print("Getting answer from model...")
-    response = openai.ChatCompletion.create(
-        model=model, messages=messages,
-    )
-
-    raw_commands_data = StaticVar(response["choices"][0]["message"]["content"])
+    commands_data_str = get_answer_from_model(instruction, model, messages)
 
     if verbosity >= 2:
-        print(f"\n\n~ ~ ~ ~ Commands graph string generated by the LLM\n\n{raw_commands_data.val}\n\n~ ~ ~ ~")
+        print(f"\n\n~ ~ ~ ~ Commands graph string generated by the LLM\n\n{commands_data_str}\n\n~ ~ ~ ~")
 
-    return raw_commands_data
+    return commands_data_str
 
 def recognize_instruction_and_create_graph(prompt: str, model: str, 
         commands: dict[str, dict], command_name_to_func: dict[str, Callable],
-        verbosity: bool = 0) -> Graph:
-    raw_commands_data = recognize_instruction(prompt, model, commands, verbosity=verbosity)
-    graph = Graph(raw_commands_data, commands, command_name_to_func)
+        verbosity: bool = 0, save_graph_as_file: bool = False) -> Graph:
+    commands_data_str = recognize_instruction(prompt, model, commands, verbosity=verbosity)
+    if save_graph_as_file:
+        with open("graph.txt", "w+") as f:
+            f.write(commands_data_str)
+            f.close()
+    graph = Graph(commands_data_str, commands, command_name_to_func)
     return graph
 
-def explain_graph_in_natural_language(raw_commands_data: str, commands: dict[str, dict]) -> str:
+def explain_graph_in_natural_language(raw_commands_data: str, model: str, commands: dict[str, dict]) -> str:
     messages = [
         {
         'role': 'system', 
         'content':
             """You are a tool that, given a graph of commands, explains in natural language what the graph does, how the nodes connect, and all the details about the graph, commands and nodes."""
             """\n*IMPORTANT*: *WRITE in the LANGUAGE that the USER writes his/her prompt in*."""
 
             f"""\n\nCommands:\n{commands}"""
 
             """\n\nThe graph of commands has this format:"""
-            """\n[[command_id, "COMMAND_NAME", {"arg1": value1, "arg2": value2, ...}, [[next_command_id, "dependent_on_data", required_value], [...], ...]], [...]]"""
+            """\n[command_id, "COMMAND_NAME", {"arg1": value1, "arg2": value2, ...}, [[next_command_id, "dependent_on_data", required_value], [...], ...]]"""
+            """\n[...]"""
             """\nTo reference data generated by a command, use __&i.data__. 'i' is the ID of the command; 'data' is the name of the generated data, and works like a Python value (if it's a list, you can use __&i.data[i]__, __&i.data[i:j]__, etc.; in a dictionary, __&i.data["key"]__, etc.)."""
             """\nThe structure will ultimately be like a graph. The next_command_id defines which command will be executed next, dependent_on_data is the name of the data generated by the current command which will be used as a condition (null if it won't be used), and required_value is what value the dependent_on_data must have to execute the next command (or null if it doesn't matter)."""
             """\nA command can execute multiple next commands."""
 
             """\n\nExamples of graphs of commands generated from the user prompt:"""
 
             """\n\nExample 1:"""
             """\nUser prompt: 'Write an article about Lenz's Law, copy it to my clipboard and save it as a file.'"""
-            """\nThe response might be: '[[1, "%s", {"about": "Article about Lenz's Law"}, [[2, null, null]]], [2, "%s", {"content": "__&1.thought__"}, [[3, null, null]]], [3, "%s", {"content": "__&1.thought__", "file_name": "Article about Lenz's Law"}, []]]'""" % ("THINK", "WRITE_CLIPBOARD", "WRITE_FILE")
-            +
+            """\nThe response might be: '[1, "THINK", {"about": "Article about Lenz's Law"}, [[2, null, null]]]\n[2, "WRITE_CLIPBOARD", {"content": "__&1.thought__"}, [[3, null, null]]]\n[3, "WRITE_FILE", {"content": "__&1.thought__", "file_name": "Article about Lenz's Law"}, []]'"""
             """\n\nExample 2:"""
             """\nUser prompt: 'Read my clipboard, write a scientific article about the content in it, and save it as a file with a name related to the article.'"""
-            """\nThe response might be: '[[1, "%s", {}, [[1, null, null]]], [2, "%s", {"about": "Scientific article about __&1.content__"}, [[3, null, null]]], [3, "%s", {"about": "Name including extension to save a file about this article: __&2.thought__"}, [[4, null, null]]], [4, "%s", {"content": "__&2.thought__", "file_name": "__&3.thought__"}, []]]'""" % ("READ_CLIPBOARD", "THINK", "THINK", "WRITE_FILE")
-            +
+            """\nThe response might be: '[1, "READ_CLIPBOARD", {}, [[2, null, null]]]\n[2, "THINK", {"about": "Scientific article about __&1.content__"}, [[3, null, null]]]\n[3, "THINK", {"about": "Name including extension to save a file about this article: __&2.thought__"}, [[4, null, null]]]\n[4, "WRITE_FILE", {"content": "__&2.thought__", "file_name": "__&3.thought__"}, []]'"""
             """\n\nExample 3:"""
             """\nUser prompt: 'Look up the best courses on ASP.Net on Google and show me the first page that appears, if it is relevant.'"""
-            """\nThe response might be: '[[1, "%s", {"query": "best courses on ASP.Net"}, [[2, null, null]]], [2, "%s", {"url": "__&1.urls[0]__"}, [[3, null, null]]], [3, "%s", {"condition": "Is this a relevant course on ASP.Net? __&2.text__"}, [[4, "result", 1], [5, "result", 0]]], [4, "%s", {"content": "Relevant course: __&1.urls[0]__"}, []], [5, "%s", {"content": "It is not relevant."}, []]]'""" % ("SEARCH_GOOGLE", "READ_WEBPAGE", "IF", "WRITE_TO_USER", "WRITE_TO_USER")
-            +
+            """\nThe response might be: '[1, "SEARCH_GOOGLE", {"query": "best courses on ASP.Net"}, [[2, null, null]]]\n[2, "READ_WEBPAGE", {"url": "__&1.urls[0]__"}, [[3, null, null]]]\n[3, "IF", {"condition": "Is this a relevant course on ASP.Net? __&2.text__"}, [[4, "result", 1], [5, "result", 0]]]\n[4, "WRITE_TO_USER", {"content": "Relevant course: __&1.urls[0]__"}, []]\n[5, "WRITE_TO_USER", {"content": "It is not relevant."}, []]'"""
 
-            """\n\nThe structure is JSON-like."""
+            """\n\nThe structure is JSON-Lines-like."""
         }
     ]
-    messages.append({"role": "user", "content": raw_commands_data})
     print(f"Input tokens used by messages (graph explanation): ~{len(str(messages)) / 4} tokens.")
 
-    print("Getting answer from model...")
-    response = openai.ChatCompletion.create(
-        model="gpt-4-0314", messages=messages,
-    )
-
-    explanation = response["choices"][0]["message"]["content"]
+    explanation = get_answer_from_model(raw_commands_data, "gpt-4-0314", messages)
 
     return explanation
```

### Comparing `commandsgpt-1.2.2/commands_gpt/commands_gpt/regex.py` & `commandsgpt-1.3.0/commands_gpt/commands_gpt/regex.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,34 +13,42 @@
     if isinstance(data, (list, tuple)):
         return data[int(index)]
     elif isinstance(data, dict):
         return data[index]
     else:
         raise AssertionError(f"Could not get data for {data_name}. Indexes for type {type(data)} are not supported.")
 
-def fix_for_json(value_as_str: str):
+def escape_str_for_json(value_as_str: str):
     # Replace newlines with escaped newlines
     value_as_str = value_as_str.replace(r"\n", "\\n")
 
     # Escape double quotes inside the string
     value_as_str = value_as_str.replace('"', '\\"')
     return value_as_str
 
+def unescape_str_in_json(value_as_str: str):
+    # Replace escaped newlines with newlines
+    value_as_str = value_as_str.replace("\\n", r"\n")
+
+    # Replace escaped double quotes with double quotes
+    value_as_str = value_as_str.replace('\\"', '"')
+    return value_as_str
+
 def replace_generated_data_by_node(match_obj, generated_data_by_node: Dict[str, Any]) -> str:
     # Get the data name from the matched object
     data_name = match_obj.group(1)
 
     # Check if the data name has an index/key
     if '[' in data_name and ']' in data_name:
         value = get_indexed_data(data_name, generated_data_by_node)
     else:
         value = generated_data_by_node[data_name]
 
     value_as_str = str(value)
-    value_as_str = fix_for_json(value_as_str)
+    value_as_str = escape_str_for_json(value_as_str)
 
     return value_as_str
 
 def inject_node_data(raw_commands_data: str, node_id, generated_data_by_node: dict[str, Any]):
     pattern = rf"__&{node_id}\.(\w+)__"
     return re.sub(pattern, lambda m: replace_generated_data_by_node(m, generated_data_by_node), raw_commands_data)
 
@@ -60,15 +68,14 @@
     Returns:
         A dictionary where the keys are command IDs and the values are dictionaries representing the generated data for that
         command. These inner dictionaries have keys that are names of generated data variables and values that are lists of tuples.
         Each tuple in these lists contains the starting and ending positions of the generated data variable within the
         raw_commands_data input string.
 
     Example:
-        >>> find_data_references_indices('''[1, [], "SEARCH_GOOGLE", {"query": "mejores cursos sobre ASP.Net"}], [2, [1, None, None], "READ_WEBPAGE", {"url": "__&1.urls[0]__"}], [3, [2, None, None], "IF", {"condition": "¿Es un curso relevante sobre ASP.Net? __&2.text__"}], [4, [3, "result", 1], "WRITE_TO_USER", {"content": "Curso relevante: __&1.urls[0]__"}], [5, [3, "result", 0], "WRITE_TO_USER", {"content": "No es relevante."}]''')
         {1: {'urls[0]': [(115, 129), (299, 313)]}, 2: {'text': [(214, 225)]}}
     """
     pattern = r"__&(\d+)\.(\w+(?:\[\d+\])*)__"
     matches = re.finditer(pattern, raw_commands_data)
     references = {}
     for match in matches:
         command_id = int(match.group(1))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `commandsgpt-1.2.2/commands_gpt/commandsgpt.egg-info/SOURCES.txt` & `commandsgpt-1.3.0/commands_gpt/commandsgpt.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 setup.cfg
 commands_gpt/commands_gpt/__init__.py
 commands_gpt/commands_gpt/chat.py
 commands_gpt/commands_gpt/config.py
 commands_gpt/commands_gpt/instruction_recognition.py
 commands_gpt/commands_gpt/models.py
 commands_gpt/commands_gpt/regex.py
-commands_gpt/commands_gpt/static.py
 commands_gpt/commands_gpt/commands/__init__.py
 commands_gpt/commands_gpt/commands/commands_funcs.py
 commands_gpt/commands_gpt/commands/graphs.py
 commands_gpt/commandsgpt.egg-info/PKG-INFO
 commands_gpt/commandsgpt.egg-info/SOURCES.txt
 commands_gpt/commandsgpt.egg-info/dependency_links.txt
 commands_gpt/commandsgpt.egg-info/top_level.txt
```

### Comparing `commandsgpt-1.2.2/setup.cfg` & `commandsgpt-1.3.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = commandsgpt
-version = 1.2.2
+version = 1.3.0
 author = Martín Alexis Martínez Andrade
 author_email = alexis.martinez.contacto@gmail.com
 description = An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/AlexisAndradeDev/CommandsGPT
 project_urls =
```

