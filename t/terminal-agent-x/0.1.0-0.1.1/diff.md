# Comparing `tmp/terminal-agent-x-0.1.0.tar.gz` & `tmp/terminal-agent-x-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal-agent-x-0.1.0.tar", last modified: Tue May  9 01:22:11 2023, max compression
+gzip compressed data, was "terminal-agent-x-0.1.1.tar", last modified: Wed May 24 17:23:40 2023, max compression
```

## Comparing `terminal-agent-x-0.1.0.tar` & `terminal-agent-x-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-09 01:22:11.448836 terminal-agent-x-0.1.0/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35149 2023-05-08 10:01:27.000000 terminal-agent-x-0.1.0/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2140 2023-05-09 01:22:11.448836 terminal-agent-x-0.1.0/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1377 2023-05-09 01:08:47.000000 terminal-agent-x-0.1.0/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      869 2023-05-09 01:22:00.000000 terminal-agent-x-0.1.0/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-09 01:22:11.448836 terminal-agent-x-0.1.0/setup.cfg
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-09 01:22:11.444836 terminal-agent-x-0.1.0/terminal_agent_x/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-09 00:14:06.000000 terminal-agent-x-0.1.0/terminal_agent_x/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4770 2023-05-08 12:43:17.000000 terminal-agent-x-0.1.0/terminal_agent_x/tax.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-09 01:22:11.448836 terminal-agent-x-0.1.0/terminal_agent_x.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2140 2023-05-09 01:22:11.000000 terminal-agent-x-0.1.0/terminal_agent_x.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      288 2023-05-09 01:22:11.000000 terminal-agent-x-0.1.0/terminal_agent_x.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-09 01:22:11.000000 terminal-agent-x-0.1.0/terminal_agent_x.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       50 2023-05-09 01:22:11.000000 terminal-agent-x-0.1.0/terminal_agent_x.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2023-05-09 01:22:11.000000 terminal-agent-x-0.1.0/terminal_agent_x.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-24 17:23:40.149061 terminal-agent-x-0.1.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35149 2023-05-08 10:01:27.000000 terminal-agent-x-0.1.1/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2602 2023-05-24 17:23:40.149061 terminal-agent-x-0.1.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1840 2023-05-24 17:23:29.000000 terminal-agent-x-0.1.1/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      869 2023-05-24 17:08:45.000000 terminal-agent-x-0.1.1/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-24 17:23:40.149061 terminal-agent-x-0.1.1/setup.cfg
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-24 17:23:40.145061 terminal-agent-x-0.1.1/terminal_agent_x/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-09 00:14:06.000000 terminal-agent-x-0.1.1/terminal_agent_x/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4359 2023-05-24 17:07:28.000000 terminal-agent-x-0.1.1/terminal_agent_x/tax.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-24 17:23:40.149061 terminal-agent-x-0.1.1/terminal_agent_x.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2602 2023-05-24 17:23:40.000000 terminal-agent-x-0.1.1/terminal_agent_x.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      288 2023-05-24 17:23:40.000000 terminal-agent-x-0.1.1/terminal_agent_x.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-24 17:23:40.000000 terminal-agent-x-0.1.1/terminal_agent_x.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       50 2023-05-24 17:23:40.000000 terminal-agent-x-0.1.1/terminal_agent_x.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2023-05-24 17:23:40.000000 terminal-agent-x-0.1.1/terminal_agent_x.egg-info/top_level.txt
```

### Comparing `terminal-agent-x-0.1.0/LICENSE` & `terminal-agent-x-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal-agent-x-0.1.0/PKG-INFO` & `terminal-agent-x-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-agent-x
-Version: 0.1.0
+Version: 0.1.1
 Summary: A terminal agent for terminal users.
 Author-email: LyuLumos <lyujiuyang0@gmail.com>
 Project-URL: Homepage, https://github.com/LyuLumos/Terminal-Agent-X
 Project-URL: Bug Tracker, https://github.com/LyuLumos/Terminal-Agent-X/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Terminal-Agent-X
 
-[EN](README.md) / [中文](https://github.com/LyuLumos/Terminal-Agent-X/blob/main/README_cn.md)
+[EN](README.md) / [中文](https://github.com/LyuLumos/Terminal-Agent-X/blob/main/README_cn.md) / [Wiki](https://github.com/LyuLumos/Terminal-Agent-X/wiki)
 
 ## Install
 
 ```bash
 pip install terminal-agent-x
 ```
 
@@ -51,25 +51,50 @@
 You can use the `tax <prompt>` to interact with the model, like this:
 
 ```
 tax write a python code for fibonacci
 ```
 
 Use `tax -h` to get more information.
+```bash
+usage: tax.py [-h] [--openai_key OPENAI_KEY] [--model MODEL] [--file FILE] [--url URL] [--show_all] prompt [prompt ...]
+```
 
 ## Support
 
 I have tested on Windows 10/11(cmd) and Ubuntu 22.04, it should work on other platforms.
 
-Current version does not support Windows Powershell, or run on Windows systems early than Windows 10. For these users, you can install `curl on Windows` to use this tool.
-
 ## Attention
 
 You can see a directive after the generated command that says
 ```
 Do you want to execute the command? (y/n)
 ```
 Please execute it or not at your own discretion. I am not responsible for the consequences of generated commands.
 
 ## License
 
 [GNU General Public License v3.0](LICENSE)
+
+## Development Logs
+
+<details>
+<summary>Contents</summary>
+
+<details>
+<summary>0.1.0</summary>
+
+- Implement basic functions
+- Support for Windows cmd and Linux shell
+- Add `--file` option for saving the response to a file
+</details>
+
+<details>
+<summary>0.1.1</summary>
+
+- Add `--show_all` option for showing all contents of the response.
+- Add `--url` option for users not under GFW.
+- support for Windows Powershell
+</details>
+
+
+</details>
```

### Comparing `terminal-agent-x-0.1.0/pyproject.toml` & `terminal-agent-x-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "terminal-agent-x"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="LyuLumos", email="lyujiuyang0@gmail.com" },
 ]
 description = "A terminal agent for terminal users."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `terminal-agent-x-0.1.0/terminal_agent_x.egg-info/PKG-INFO` & `terminal-agent-x-0.1.1/terminal_agent_x.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-agent-x
-Version: 0.1.0
+Version: 0.1.1
 Summary: A terminal agent for terminal users.
 Author-email: LyuLumos <lyujiuyang0@gmail.com>
 Project-URL: Homepage, https://github.com/LyuLumos/Terminal-Agent-X
 Project-URL: Bug Tracker, https://github.com/LyuLumos/Terminal-Agent-X/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Terminal-Agent-X
 
-[EN](README.md) / [中文](https://github.com/LyuLumos/Terminal-Agent-X/blob/main/README_cn.md)
+[EN](README.md) / [中文](https://github.com/LyuLumos/Terminal-Agent-X/blob/main/README_cn.md) / [Wiki](https://github.com/LyuLumos/Terminal-Agent-X/wiki)
 
 ## Install
 
 ```bash
 pip install terminal-agent-x
 ```
 
@@ -51,25 +51,50 @@
 You can use the `tax <prompt>` to interact with the model, like this:
 
 ```
 tax write a python code for fibonacci
 ```
 
 Use `tax -h` to get more information.
+```bash
+usage: tax.py [-h] [--openai_key OPENAI_KEY] [--model MODEL] [--file FILE] [--url URL] [--show_all] prompt [prompt ...]
+```
 
 ## Support
 
 I have tested on Windows 10/11(cmd) and Ubuntu 22.04, it should work on other platforms.
 
-Current version does not support Windows Powershell, or run on Windows systems early than Windows 10. For these users, you can install `curl on Windows` to use this tool.
-
 ## Attention
 
 You can see a directive after the generated command that says
 ```
 Do you want to execute the command? (y/n)
 ```
 Please execute it or not at your own discretion. I am not responsible for the consequences of generated commands.
 
 ## License
 
 [GNU General Public License v3.0](LICENSE)
+
+## Development Logs
+
+<details>
+<summary>Contents</summary>
+
+<details>
+<summary>0.1.0</summary>
+
+- Implement basic functions
+- Support for Windows cmd and Linux shell
+- Add `--file` option for saving the response to a file
+</details>
+
+<details>
+<summary>0.1.1</summary>
+
+- Add `--show_all` option for showing all contents of the response.
+- Add `--url` option for users not under GFW.
+- support for Windows Powershell
+</details>
+
+
+</details>
```

