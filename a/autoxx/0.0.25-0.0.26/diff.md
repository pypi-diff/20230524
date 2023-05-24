# Comparing `tmp/autoxx-0.0.25.tar.gz` & `tmp/autoxx-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.25.tar", max compression
+gzip compressed data, was "autoxx-0.0.26.tar", max compression
```

## Comparing `autoxx-0.0.25.tar` & `autoxx-0.0.26.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.25/README.md
--rw-r--r--   0        0        0     7344 2023-05-23 10:04:32.651102 autoxx-0.0.25/autoxx/agent/babyagi/agi.py
--rw-r--r--   0        0        0     1109 2023-05-22 11:10:29.311248 autoxx-0.0.25/autoxx/agent/babyagi/task_manager.py
--rw-r--r--   0        0        0    10193 2023-05-22 08:58:57.762888 autoxx-0.0.25/autoxx/agent/react/agent.py
--rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.25/autoxx/requirements.txt
--rw-r--r--   0        0        0      801 2023-05-23 08:04:17.676812 autoxx-0.0.25/autoxx/setup.py
--rw-r--r--   0        0        0     5352 2023-05-22 11:51:39.068804 autoxx-0.0.25/autoxx/tools/knowledge_base/utils.py
--rw-r--r--   0        0        0      929 2023-05-22 06:15:52.199109 autoxx-0.0.25/autoxx/tools/llm/utils.py
--rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.25/autoxx/tools/web_search/js/overlay.js
--rw-r--r--   0        0        0     6473 2023-05-23 10:03:19.637350 autoxx-0.0.25/autoxx/tools/web_search/search.py
--rw-r--r--   0        0        0      664 2023-05-23 10:05:40.511480 autoxx-0.0.25/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 autoxx-0.0.25/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.26/README.md
+-rw-r--r--   0        0        0     7157 2023-05-23 12:00:39.378796 autoxx-0.0.26/autoxx/agent/babyagi/agi.py
+-rw-r--r--   0        0        0     1109 2023-05-22 11:10:29.311248 autoxx-0.0.26/autoxx/agent/babyagi/task_manager.py
+-rw-r--r--   0        0        0    10193 2023-05-22 08:58:57.762888 autoxx-0.0.26/autoxx/agent/react/agent.py
+-rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.26/autoxx/requirements.txt
+-rw-r--r--   0        0        0      801 2023-05-23 08:04:17.676812 autoxx-0.0.26/autoxx/setup.py
+-rw-r--r--   0        0        0     5352 2023-05-22 11:51:39.068804 autoxx-0.0.26/autoxx/tools/knowledge_base/utils.py
+-rw-r--r--   0        0        0      929 2023-05-22 06:15:52.199109 autoxx-0.0.26/autoxx/tools/llm/utils.py
+-rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.26/autoxx/tools/web_search/js/overlay.js
+-rw-r--r--   0        0        0     6473 2023-05-23 10:03:19.637350 autoxx-0.0.26/autoxx/tools/web_search/search.py
+-rw-r--r--   0        0        0      664 2023-05-23 12:06:16.822412 autoxx-0.0.26/pyproject.toml
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 autoxx-0.0.26/PKG-INFO
```

### Comparing `autoxx-0.0.25/autoxx/agent/babyagi/agi.py` & `autoxx-0.0.26/autoxx/agent/babyagi/agi.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,16 +35,16 @@
             f"Create new tasks based on the following plan delimited by triple backtick if necessary for the objective. Limit tasks types to those that can be completed with the available tools listed below. Task description should be detailed. "
             f"Your task: decelop a task list .\n"
             f"The current tool option is [web-search, text-completion] only. What each tool does is as follows:\n"
             f"web-search: It supports searching for information from the Internet. Interaction with web pages is not supported. For tasks using [web-search], provide the search query, and only the search query to use (eg. not 'research waterproof shoes, but 'waterproof shoes').\n"
             f"text-completion: It can be used for text extraction, summarization, copywrite, translation, etc., and it can also be used for LLM-based QA.\n"
             f"Make sure all task IDs are in chronological order.\n"
             f"For efficiency, let's think step by step and create the tasks (up to 5 tasks) that are most critical to objective. "
-            f"The last step is always to provide a final summary report including tasks executed and summary of knowledge acquired.\n"
-            f"Do not create any summarizing steps outside of the last step. And provide useful link in the summary report.\n"
+            f"The last step is always to provide a final formal report about objective including summary of knowledge acquired.\n"
+            f"Do not create any summarizing steps outside of the last step.\n"
             f"The task list output format is as follows: "
             "[{\"id\": 1, \"task\": \"Untapped Capital\", \"tool\": \"web-search\", \"dependent_task_ids\": [], \"status\": \"incomplete\", \"result\": null, \"result_summary\": null}, {\"id\": 2, \"task\": \"Consider additional insights that can be reasoned from the results of...\", \"tool\": \"text-completion\", \"dependent_task_ids\": [1], \"status\": \"incomplete\", \"result\": null, \"result_summary\": null}].\n"
             f"Ensure the output can be parsed by Python json.loads.\n task list="
         )
 
         messages = create_message(prompt)
         response = create_chat_completion(
@@ -77,31 +77,28 @@
                     return
                 elif dependent_task:
                     dependent_task_prompt += f"\ntask ({dependent_task['id']}. {dependent_task['task']}) result: {dependent_task['result']}"
 
         # Execute task
         
         task_prompt = (
-            f"Complete your assigned task based on the objective: {self.objective}. Your task: {task['task']}\n"
+            f"Complete your assigned task based on the objective: {self.objective}. Your task: {task['task']}. "
+            f"Please keep the link reference like newbing in the response.\n"
         )
         if dependent_task_prompt != "":
             task_prompt += f"The previous tasks: {dependent_task_prompt}"
 
         task_prompt += "\nResponse:"
         if task["tool"] == "text-completion":
-            result = llm_uils().text_completion(task_prompt)
-            summary_result_prompt = f"Please summarize the following text:\n{result}\nSummary:"
+            result = llm_uils("gpt-4").text_completion(task_prompt)
+            summary_result_prompt = f"Please summarize the following text and and keep the reference links:\n{result}\nSummary:"
             task["result_summary"] = llm_uils().text_completion(summary_result_prompt)
         elif task["tool"] == "web-search":
             result = str(web_search(str(task['task'])))
-            summary_result_prompt = f"Please summarize the following text:\n{result}\nSummary:"
-            task["result_summary"] = llm_uils().text_completion(summary_result_prompt)
-        elif task["tool"] == "search-IT-knowledge-base":
-            result = str(self.it_kb.similarity_search(str(task['task'])))
-            summary_result_prompt = f"Please summarize the following text:\n{result}\nSummary:"
+            summary_result_prompt = f"Please summarize the following text and keep all links:\n{result}\nSummary:"
             task["result_summary"] = llm_uils().text_completion(summary_result_prompt)
         else:
             result = "Unknown tool"
         
         # Update task status and result
         task["status"] = "completed"
         task["result"] = result
@@ -116,15 +113,15 @@
             logging.info(f"\033[95m\033[1m INCOMPLETE TASK LIST({self.objective}) \033[0m\033[0m {[str(t['id'])+': '+t['task'] + '[' + t['tool'] + ']' for t in incomplete_tasks]}")
             if incomplete_tasks:
                 # Sort tasks by ID
                 incomplete_tasks.sort(key=lambda x: x["id"])
 
                 # Pull the first task
                 task = incomplete_tasks[0]
-                logging.info(f"\033[92m\033[1m NEXT TASK({self.objective}) \033[0m\033[0m {task['id']}:{task['task']}[{task['tool']}]")
+                logging.info(f"\033[92m\033[1m NEXT TASK({self.objective}) \033[0m\033[0m {task['id']}:{task['task']}[{task['tool']}], depends on {task['dependent_task_ids']}")
 
                 # Execute task & call task manager from function
                 try:
                     completed_task = self.execute_task(task)
                     logging.info(f"\033[93m\033[1m TASK RESULT({self.objective}) \033[0m\033[0m {completed_task['result']}")
                 except Exception as e:  
                     logging.error(f"An error occurred while executing the task({self.objective}): {e.with_traceback(None)}")
```

### Comparing `autoxx-0.0.25/autoxx/agent/babyagi/task_manager.py` & `autoxx-0.0.26/autoxx/agent/babyagi/task_manager.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.25/autoxx/agent/react/agent.py` & `autoxx-0.0.26/autoxx/agent/react/agent.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.25/autoxx/setup.py` & `autoxx-0.0.26/autoxx/setup.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.25/autoxx/tools/knowledge_base/utils.py` & `autoxx-0.0.26/autoxx/tools/knowledge_base/utils.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.25/autoxx/tools/llm/utils.py` & `autoxx-0.0.26/autoxx/tools/llm/utils.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.25/autoxx/tools/web_search/js/overlay.js` & `autoxx-0.0.26/autoxx/tools/web_search/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.25/autoxx/tools/web_search/search.py` & `autoxx-0.0.26/autoxx/tools/web_search/search.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.25/pyproject.toml` & `autoxx-0.0.26/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.25"
+version = "0.0.26"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `autoxx-0.0.25/PKG-INFO` & `autoxx-0.0.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.25
+Version: 0.0.26
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

