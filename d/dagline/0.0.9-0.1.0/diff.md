# Comparing `tmp/dagline-0.0.9.tar.gz` & `tmp/dagline-0.1.0.tar.gz`

## Comparing `dagline-0.0.9.tar` & `dagline-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagline-0.0.9/src/dagline/__init__.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dagline-0.0.9/src/dagline/__main__.py
--rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 dagline-0.0.9/src/dagline/jobs/dag_processor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagline-0.0.9/src/dagline/models/__init__.py
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 dagline-0.0.9/src/dagline/models/dag.py
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 dagline-0.0.9/src/dagline/models/dagbag.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 dagline-0.0.9/src/dagline/models/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagline-0.0.9/src/dagline/models/operators/__init__.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 dagline-0.0.9/src/dagline/models/operators/python.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 dagline-0.0.9/src/dagline/models/operators/winbat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagline-0.0.9/src/dagline/utils/__init__.py
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 dagline-0.0.9/src/dagline/utils/cli.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 dagline-0.0.9/src/dagline/utils/logging_setup.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 dagline-0.0.9/src/dagline/utils/state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagline-0.0.9/src/dagline/utils/commands/__init__.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 dagline-0.0.9/src/dagline/utils/commands/dag_command.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dagline-0.0.9/LICENSE
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 dagline-0.0.9/README.md
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 dagline-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 dagline-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagline-0.1.0/src/dagline/__init__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dagline-0.1.0/src/dagline/__main__.py
+-rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 dagline-0.1.0/src/dagline/jobs/dag_processor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagline-0.1.0/src/dagline/models/__init__.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 dagline-0.1.0/src/dagline/models/dag.py
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 dagline-0.1.0/src/dagline/models/dagbag.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 dagline-0.1.0/src/dagline/models/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagline-0.1.0/src/dagline/models/operators/__init__.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 dagline-0.1.0/src/dagline/models/operators/python.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 dagline-0.1.0/src/dagline/models/operators/winbat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagline-0.1.0/src/dagline/utils/__init__.py
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 dagline-0.1.0/src/dagline/utils/cli.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 dagline-0.1.0/src/dagline/utils/logging_setup.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 dagline-0.1.0/src/dagline/utils/state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagline-0.1.0/src/dagline/utils/commands/__init__.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 dagline-0.1.0/src/dagline/utils/commands/dag_command.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dagline-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 dagline-0.1.0/README.md
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 dagline-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 dagline-0.1.0/PKG-INFO
```

### Comparing `dagline-0.0.9/src/dagline/jobs/dag_processor.py` & `dagline-0.1.0/src/dagline/jobs/dag_processor.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,52 +7,81 @@
 from graphlib import TopologicalSorter
 from typing import Callable
 from dagline.models.dagbag import DagBag
 from dagline.utils.state import State
 from dagline.utils.logging_setup import LoggingMixin
 from contextlib import redirect_stdout
 import io
+import time
 
-def execute_python_task(task, task_done_queue):
+def execute_python_task(task, task_done_queue, retry_flag):
+    if retry_flag == 1:
+        time.sleep(task.retry_delay)
     try:
         '''To capture stdout output from a Python function call'''
         with redirect_stdout(io.StringIO()) as f:
             task.python_callable()
         
         task_ouput = f.getvalue()
         task.exec_ouput = task_ouput
         task.state = State.SUCCESS
     except Exception as e:
-        task.exec_ouput = task_ouput
+        task.exec_ouput = e
         task.state = State.FAILED
         
     task_done_queue.put(task)
 
-def execute_winbat_task(task, task_done_queue):
+def execute_winbat_task(task, task_done_queue, retry_flag):
+    if retry_flag == 1:
+        time.sleep(task.retry_delay)
     try:
         #subprocess.check_call(task.bat_command)
         cp = subprocess.run(task.bat_command, check=True, text=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
         task.exec_ouput = cp.stdout
         task.state = State.SUCCESS
     except Exception as e:
-        task.exec_ouput = e.stdout
+        task.exec_ouput = e
         task.state = State.FAILED
         
         
     task_done_queue.put(task)
     
     
 class DagProcess(Process, LoggingMixin):
 
     def __init__(self, dag:DAG):
         super().__init__()
         self.dag = dag
         self.logfile = dag.logfile
 
 
+    def new_task_process(self, task, task_done_queue, running_processes, retry_flag):
+        task_func : Callable
+        
+        '''Check the task type'''
+        if isinstance(task, WinbatOperator):
+            task_func = execute_winbat_task
+        elif isinstance(task, PythonOperator):
+            task_func = execute_python_task
+        else:
+            pass
+
+        sub_p = multiprocessing.Process(
+        target=task_func,
+        args=(task, task_done_queue, retry_flag, )
+        )
+        sub_p.start()
+        running_processes[task.task_id] = sub_p
+        
+        if retry_flag == 0:
+            self.log.info(f'''Executing task [{task.task_id}]''')
+        else:
+            self.log.info(f'''Retry Executing task [{task.task_id}] after [{task.retry_delay}] seconds''')
+
+
     def run(self):
         self.log.info(f'''Starting DAG [{self.dag.dag_id}]''')
         dag_tasks = self.dag.tasks
         dag_tasks_flow = self.dag.tasks_flow
         
         task_done_queue = multiprocessing.Queue()
         
@@ -60,31 +89,15 @@
         running_processes = {}
             
         topological_sorter = TopologicalSorter(dag_tasks_flow)
         topological_sorter.prepare()
         while topological_sorter.is_active():
             ready_tasks = topological_sorter.get_ready()
             for task in ready_tasks:
-                task_func : Callable
-                
-                '''Check the task type'''
-                if isinstance(task, WinbatOperator):
-                    task_func = execute_winbat_task
-                elif isinstance(task, PythonOperator):
-                    task_func = execute_python_task
-                else:
-                    pass
-
-                sub_p = multiprocessing.Process(
-                target=task_func,
-                args=(task, task_done_queue,)
-                )
-                sub_p.start()
-                running_processes[task.task_id] = sub_p
-                self.log.info(f'''Executing task [{task.task_id}]''')
+                self.new_task_process(task, task_done_queue, running_processes, retry_flag = 0)
             
             '''Make sure we can jump out of the loop if there are some tasks failed
                Cause TopologicalSorter need to iterate all the nodes of the DAG
                If running_processes is empty, that means no nodes of the DAG will be processed any more
             '''
             if len(running_processes) == 0:
                 break
@@ -96,30 +109,35 @@
             finished_task_exec_output = finished_task.exec_ouput
             
             running_processes.pop(finished_task_id).join()
             dag_finished_task = dag_tasks[finished_task_id]
             dag_finished_task.state = finished_task_state
             dag_finished_task.exec_ouput = finished_task_exec_output
             
-            
 
             if finished_task_state == State.SUCCESS:
                 '''
                 Here we can't use the object from task_done_queue.get() cause the address of the object has been changed 
                 after pass the object to process, it is not the same as the original one
                 '''
                 topological_sorter.done(dag_finished_task)
-                
+
                 '''Log the output of the task'''
                 self.log.info(f'''Output---From---Task [{dag_finished_task.task_id}]\n{dag_finished_task.exec_ouput}''')
+                self.log.info(f'''Finished task [{dag_finished_task.task_id}] (result=[{dag_finished_task.state}])''')
             else:
                 self.log.error(f'''Output---From---Task [{dag_finished_task.task_id}]\n{dag_finished_task.exec_ouput}''')
-
-            self.log.info(f'''Finished task [{dag_finished_task.task_id}] (result=[{dag_finished_task.state}])''')
+                self.log.info(f'''Finished task [{dag_finished_task.task_id}] (result=[{dag_finished_task.state}])''')
+                # Retry the task
+                if dag_finished_task.retry_cnt > 0:
+                    self.new_task_process(dag_finished_task, task_done_queue, running_processes, retry_flag = 1)
+                    dag_finished_task.retry_cnt = dag_finished_task.retry_cnt - 1
+            
             
+        # Assign the skipped state to the tasks that were not to be executed at this batch run
         for task in dag_tasks.values():
             if task.state == None:
                 task.state = State.SKIPPED
                 self.log.info(f'''Finished task [{task.task_id}] (result=[{task.state}])''')
 
         '''If the state of any tasks in the DAG is failed, the the state of the DAG is failed'''
         if len(list(filter(lambda tk:(tk.state == State.FAILED), dag_tasks.values()))) == 0:
```

### Comparing `dagline-0.0.9/src/dagline/models/dag.py` & `dagline-0.1.0/src/dagline/models/dag.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 from dagline.models.operators.python import PythonOperator
 from graphlib import TopologicalSorter
 from dagline.utils.logging_setup import LoggingMixin
 import copy
 
 class DAG(LoggingMixin):
 
-    def __init__(self, dag_id: str, logfile: str, tasks_flow: Dict):
+    def __init__(self, dag_id: str, logfile: str, tasks_flow: Dict, retry_cnt: int = 0, retry_delay: int = 0):
         self.dag_id = dag_id
         self.logfile = logfile
+        self.retry_cnt = retry_cnt
+        self.retry_delay = retry_delay
         '''Each DAG can include the same task instances, we use deepcopy on the tasks
            Make sure each DAG can have its own unique tasks
         '''
         self.tasks_flow = copy.deepcopy(tasks_flow)
         self.sate : str = None
         self._validate_tasks()
         if self.is_valid is True:
@@ -33,17 +35,23 @@
 
 
     def _collect_tasks(self) -> None:
         self.tasks: Dict = {}
         for child_task, p_task_list in self.tasks_flow.items():
             self.tasks[child_task.task_id] = child_task
             child_task.upstream = p_task_list
+            # Retry configuration for the each task
+            child_task.retry_cnt = self.retry_cnt
+            child_task.retry_delay = self.retry_delay
             for parent_task in p_task_list:
                 self.tasks[parent_task.task_id] = parent_task
                 parent_task.downstream.append(child_task)
+                # Retry configuration for the each task
+                parent_task.retry_cnt = self.retry_cnt
+                parent_task.retry_delay = self.retry_delay
          
     '''For running the DAG from some specified tasks, then need to call this function and pass a list of task id'''
     def run_from_tasks(self, task_ids : List) -> None:
         self.task_ids_to_start_with : List = copy.copy(task_ids)
         self.run_from_tasks_flow : Dict = {}
         
         for task_id in self.task_ids_to_start_with:
```

### Comparing `dagline-0.0.9/src/dagline/models/dagbag.py` & `dagline-0.1.0/src/dagline/models/dagbag.py`

 * *Files identical despite different names*

### Comparing `dagline-0.0.9/src/dagline/utils/cli.py` & `dagline-0.1.0/src/dagline/utils/cli.py`

 * *Files identical despite different names*

### Comparing `dagline-0.0.9/src/dagline/utils/logging_setup.py` & `dagline-0.1.0/src/dagline/utils/logging_setup.py`

 * *Files identical despite different names*

### Comparing `dagline-0.0.9/src/dagline/utils/commands/dag_command.py` & `dagline-0.1.0/src/dagline/utils/commands/dag_command.py`

 * *Files identical despite different names*

### Comparing `dagline-0.0.9/LICENSE` & `dagline-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagline-0.0.9/README.md` & `dagline-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,17 @@
 task4 : [task3]
 }
 
 
 with DAG(
     dag_id = 'dag_example',
     tasks_flow = tasks_flow,
-    logfile = "C:\xxx\dag_example.log"
+    logfile = "C:\xxx\dag_example.log",
+    retry_cnt = 3,
+    retry_delay = 10 #seconds
 ) as dag:
     pass
 
 
 ```
 
 *   **Run a DAG in parallel or run a DAG from some specified tasks**
```

### Comparing `dagline-0.0.9/pyproject.toml` & `dagline-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "dagline"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Jason Liang", email="jasonliangyc@qq.com" },
 ]
 description = "Use Python's multiprocessing module to execute tasks(python functon and windows bat script) of a DAG in parallel"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `dagline-0.0.9/PKG-INFO` & `dagline-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagline
-Version: 0.0.9
+Version: 0.1.0
 Summary: Use Python's multiprocessing module to execute tasks(python functon and windows bat script) of a DAG in parallel
 Author-email: Jason Liang <jasonliangyc@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -65,15 +65,17 @@
 task4 : [task3]
 }
 
 
 with DAG(
     dag_id = 'dag_example',
     tasks_flow = tasks_flow,
-    logfile = "C:\xxx\dag_example.log"
+    logfile = "C:\xxx\dag_example.log",
+    retry_cnt = 3,
+    retry_delay = 10 #seconds
 ) as dag:
     pass
 
 
 ```
 
 *   **Run a DAG in parallel or run a DAG from some specified tasks**
```

