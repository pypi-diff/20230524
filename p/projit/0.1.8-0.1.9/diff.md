# Comparing `tmp/projit-0.1.8.tar.gz` & `tmp/projit-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/projit-0.1.8.tar", last modified: Wed Sep 15 02:01:13 2021, max compression
+gzip compressed data, was "projit-0.1.9.tar", last modified: Wed Feb  2 11:21:23 2022, max compression
```

## Comparing `projit-0.1.8.tar` & `projit-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 john.hawkins  (5534) staff       (20)        0 2021-09-15 02:01:13.000000 projit-0.1.8/
--rw-r--r--   0 john.hawkins  (5534) staff       (20)     4593 2021-09-15 02:01:13.000000 projit-0.1.8/PKG-INFO
-drwxr-xr-x   0 john.hawkins  (5534) staff       (20)        0 2021-09-15 02:01:13.000000 projit-0.1.8/projit/
--rw-r--r--   0 john.hawkins  (5534) staff       (20)      183 2021-04-07 07:32:28.000000 projit-0.1.8/projit/config.py
--rw-r--r--   0 john.hawkins  (5534) staff       (20)    11467 2021-09-15 01:53:47.000000 projit-0.1.8/projit/projit.py
--rw-r--r--   0 john.hawkins  (5534) staff       (20)      136 2021-09-15 01:59:41.000000 projit-0.1.8/projit/__init__.py
--rw-r--r--   0 john.hawkins  (5534) staff       (20)      500 2021-04-27 11:25:46.000000 projit-0.1.8/projit/pdf.py
--rw-r--r--   0 john.hawkins  (5534) staff       (20)     7253 2021-09-15 01:49:51.000000 projit-0.1.8/projit/cli.py
--rw-r--r--   0 john.hawkins  (5534) staff       (20)     3222 2021-03-08 10:28:34.000000 projit-0.1.8/projit/utils.py
--rwxr-xr-x   0 john.hawkins  (5534) staff       (20)     1791 2021-04-08 04:59:41.000000 projit-0.1.8/projit/template.py
-drwxr-xr-x   0 john.hawkins  (5534) staff       (20)        0 2021-09-15 02:01:13.000000 projit-0.1.8/projit/templates/
--rw-r--r--   0 john.hawkins  (5534) staff       (20)      159 2021-04-25 10:32:05.000000 projit-0.1.8/projit/templates/cookiecutter-data-science
--rw-r--r--   0 john.hawkins  (5534) staff       (20)       54 2021-04-07 23:49:51.000000 projit-0.1.8/projit/templates/default
--rw-r--r--   0 john.hawkins  (5534) staff       (20)      136 2021-03-02 12:08:18.000000 projit-0.1.8/projit/__main__.py
--rwxr-xr-x   0 john.hawkins  (5534) staff       (20)       27 2021-04-07 23:22:02.000000 projit-0.1.8/MANIFEST.in
--rw-r--r--   0 john.hawkins  (5534) staff       (20)     3297 2021-09-02 09:20:46.000000 projit-0.1.8/README.md
--rw-r--r--   0 john.hawkins  (5534) staff       (20)     1133 2021-09-02 09:27:59.000000 projit-0.1.8/setup.py
-drwxr-xr-x   0 john.hawkins  (5534) staff       (20)        0 2021-09-15 02:01:13.000000 projit-0.1.8/projit.egg-info/
--rw-r--r--   0 john.hawkins  (5534) staff       (20)     4593 2021-09-15 02:01:12.000000 projit-0.1.8/projit.egg-info/PKG-INFO
--rw-r--r--   0 john.hawkins  (5534) staff       (20)      415 2021-09-15 02:01:12.000000 projit-0.1.8/projit.egg-info/SOURCES.txt
--rw-r--r--   0 john.hawkins  (5534) staff       (20)       44 2021-09-15 02:01:12.000000 projit-0.1.8/projit.egg-info/entry_points.txt
--rw-r--r--   0 john.hawkins  (5534) staff       (20)       25 2021-09-15 02:01:12.000000 projit-0.1.8/projit.egg-info/requires.txt
--rw-r--r--   0 john.hawkins  (5534) staff       (20)        7 2021-09-15 02:01:12.000000 projit-0.1.8/projit.egg-info/top_level.txt
--rw-r--r--   0 john.hawkins  (5534) staff       (20)        1 2021-09-15 02:01:12.000000 projit-0.1.8/projit.egg-info/dependency_links.txt
--rw-r--r--   0 john.hawkins  (5534) staff       (20)       38 2021-09-15 02:01:13.000000 projit-0.1.8/setup.cfg
+drwxr-xr-x   0 john       (501) staff       (20)        0 2022-02-02 11:21:23.498628 projit-0.1.9/
+-rwxr-xr-x   0 john       (501) staff       (20)       27 2021-04-07 23:22:02.000000 projit-0.1.9/MANIFEST.in
+-rw-r--r--   0 john       (501) staff       (20)     4126 2022-02-02 11:21:23.498185 projit-0.1.9/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)     3609 2022-02-02 11:11:07.000000 projit-0.1.9/README.md
+drwxr-xr-x   0 john       (501) staff       (20)        0 2022-02-02 11:21:23.494686 projit-0.1.9/projit/
+-rw-r--r--   0 john       (501) staff       (20)      136 2022-02-02 11:09:18.000000 projit-0.1.9/projit/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)      136 2021-03-02 12:08:18.000000 projit-0.1.9/projit/__main__.py
+-rw-r--r--   0 john       (501) staff       (20)     3978 2022-02-02 08:34:34.000000 projit-0.1.9/projit/ascii_plot.py
+-rw-r--r--   0 john       (501) staff       (20)    14394 2022-02-02 08:43:48.000000 projit-0.1.9/projit/cli.py
+-rw-r--r--   0 john       (501) staff       (20)      217 2022-01-29 22:42:30.000000 projit-0.1.9/projit/config.py
+-rw-r--r--   0 john       (501) staff       (20)      500 2021-04-27 11:25:46.000000 projit-0.1.9/projit/pdf.py
+-rw-r--r--   0 john       (501) staff       (20)    18644 2022-02-02 08:04:16.000000 projit-0.1.9/projit/projit.py
+-rwxr-xr-x   0 john       (501) staff       (20)     1791 2021-04-08 04:59:41.000000 projit-0.1.9/projit/template.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2022-02-02 11:21:23.497536 projit-0.1.9/projit/templates/
+-rw-r--r--   0 john       (501) staff       (20)      159 2021-04-25 10:32:05.000000 projit-0.1.9/projit/templates/cookiecutter-data-science
+-rw-r--r--   0 john       (501) staff       (20)       54 2021-04-07 23:49:51.000000 projit-0.1.9/projit/templates/default
+-rw-r--r--   0 john       (501) staff       (20)     3222 2021-03-08 10:28:34.000000 projit-0.1.9/projit/utils.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2022-02-02 11:21:23.496678 projit-0.1.9/projit.egg-info/
+-rw-r--r--   0 john       (501) staff       (20)     4126 2022-02-02 11:21:23.000000 projit-0.1.9/projit.egg-info/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      436 2022-02-02 11:21:23.000000 projit-0.1.9/projit.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2022-02-02 11:21:23.000000 projit-0.1.9/projit.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (501) staff       (20)       44 2022-02-02 11:21:23.000000 projit-0.1.9/projit.egg-info/entry_points.txt
+-rw-r--r--   0 john       (501) staff       (20)       35 2022-02-02 11:21:23.000000 projit-0.1.9/projit.egg-info/requires.txt
+-rw-r--r--   0 john       (501) staff       (20)        7 2022-02-02 11:21:23.000000 projit-0.1.9/projit.egg-info/top_level.txt
+-rw-r--r--   0 john       (501) staff       (20)       38 2022-02-02 11:21:23.498856 projit-0.1.9/setup.cfg
+-rw-r--r--   0 john       (501) staff       (20)     1146 2022-01-30 01:47:28.000000 projit-0.1.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `projit-0.1.8/projit/projit.py` & `projit-0.1.9/projit/projit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+from datetime import datetime
 import pandas as pd
+import numpy as np
+import hashlib
+import git
 import json
 import re
 import os
 
 from .config import config_file
+from .config import execution_file
 from .config import config_folder
 from .template import load_template
 from .utils import locate_projit_config
 from .pdf import PDF
 
 ##########################################################################################
 
@@ -25,15 +30,16 @@
                  name, 
                  desc="", 
                  experiments=[], 
                  datasets={},
                  results={}, 
                  params={},
                  hyperparams={},
-                 dataresults={}):
+                 dataresults={},
+                 executions={}):
         """
         Initialise a projit project object.
         This class will be used for storing and retrieving all data about the project,
         as well as ensuring that it is written to the projit meta-data files.
 
         :param path: The path to the project file.
         :type path: string, required
@@ -64,105 +70,298 @@
 
         :param dataresults: The dictionary of results on specific data sets.
                             These are used when you want your experimental results broken
                             down by the datasets. 
                             Structure: {'dataset':{'experiment':{'metric':'value'}}}
         :type dataresults: Dictionary of Dictionary of Dictionary, optional
 
+        :param executions: The dictionary of experiment executions.
+                            This structure is used to store all experimental runs.
+                            The ID is a HASH of experiment_name and 
+                            Structure: {'experiment_name':{
+                                             'ID':{ 
+                                                 'start':DATETIME, 
+                                                 'end':DATETIME,
+                                                 'githash':STRING, 
+                                                 'params':DICT,
+                                                 'hyperparams':DICT
+                                              }
+                                           }
+                                       }
+        :type executions: Dictionary of Dictionary of Dictionary, optional
+
         :return: None 
         :rtype: None 
         """
         self.path = path
         self.name = name
         self.desc = desc
         self.experiments = experiments
         self.datasets = datasets
         self.results = results
         self.params = params
         self.hyperparams = hyperparams
         self.dataresults = dataresults
+        self.executions = executions
 
 
     def get_root_path(self):
         """
         Get the path to where the project folder is located
         """
         return self.path[0:len(self.path) - len(config_folder)]
 
+    def start_experiment(self, name, path, params={}):
+        """
+        Start an experiment execution.
+        This function will create a new experiment if this is the first execution
+        otherwise it will simply add a new execution record.
+         It returns an identifer for the execution (needed to end the execution)
+
+        :param name: The experiment name (Unique Identifer)
+        :type name: string, required
+
+        :param path: The path to the experiment script being executed
+        :type path: string, required
+
+        :param params: Optional dictionary of parameters used in the experiment execution
+        :type path: Dictionary, option
+
+        :return: id : The Execution ID
+        :rtype: String
+        """
+        if not self.experiment_exists(name):
+            self.add_experiment(name, path)
+
+        startdt = str(datetime.now())
+        s = name + startdt
+        id = hashlib.sha256(s.encode()).hexdigest()
+        try:
+            repo = git.Repo(search_parent_directories=True)
+            ghash = repo.head.object.hexsha
+        except git.exc.InvalidGitRepositoryError:
+            ghash = ""
+        payload = {'start':startdt, 'end':"", 'githash':ghash, 'params':params}
+        exper_execs = {}
+        if name in self.executions:
+            exper_execs = self.executions[name]
+
+        exper_execs[id] = payload
+        self.executions[name] = exper_execs 
+        self.save()
+        return id
+
+    def end_experiment(self, name, id, hyperparams={}):
+        """
+        End an experiment execution.
+        This function require both the experiment name and the hash ID of the previously started execution
+
+        :param name: The experiment name (Unique Identifer)
+        :type name: string, required
+
+        :param id: The execution hash ID returned by the function: start_experiment 
+        :type id: string, required
+
+        :param hyperparams: Optional dictionary of hyperparameters used in the experiment execution
+        :type path: Dictionary, option
+
+        :return: None
+        :rtype: None
+        """
+
+        if not self.experiment_exists(name):
+            raise Exception(f"ERROR: Cannot end experiment: '{name}' -- Experiment not registered")
+            
+        if name in self.executions:
+            exper_execs = self.executions[name]
+        else:
+            raise Exception(f"ERROR: Cannot end experiment: '{name}' -- Executions not started")
+
+        if id in exper_execs:
+            payload = exper_execs[id]
+        else:
+            raise Exception(f"ERROR: Cannot end experiment: '{name}' -- Executions not started")
+
+        payload['end'] = str(datetime.now())
+        payload['hyperparams'] = hyperparams
+        exper_execs[id] = payload
+        self.executions[name] = exper_execs
+        self.save()
+
+
+    def get_experiment_execution_stats(self, name):
+        """
+        Given an experiment name
+        Return the execution statistics
+        """
+        if name in self.executions:
+            mean_exec_time = self.get_mean_execution_time(name)
+            return len(self.executions[name]), mean_exec_time
+        else:
+            return 0, 0
+
+    def get_mean_execution_time(self, name):
+        exec_times = self.get_execution_times(name)
+        if len(exec_times) > 0:
+            return np.mean(exec_times)
+        else:
+            return 0
+
+    def get_execution_times(self, name):
+        if name in self.executions:
+            exec_times = []
+            for execid, exec in self.executions[name].items():
+                a = datetime.strptime(exec["start"], '%Y-%m-%d %H:%M:%S.%f')
+                b = datetime.strptime(exec["end"], '%Y-%m-%d %H:%M:%S.%f')
+                diff = (b-a).seconds
+                exec_times.append(diff)
+            return exec_times
+        else:
+            return []
 
     def add_experiment(self, name, path):
         """
         Add information of a new experiment to the project. 
         Then save the project configuration.
         This function will overwrite an experiment of the same name
         and delete any previous results.
 
         :param name: The experiment name
         :type name: string, required
 
         :param path: The path to the experiment.
         :type path: string, required
+
+        :return: None
+        :rtype: None
         """
         for elem in self.experiments: 
             if elem[0] == name:
                 self.experiments.remove(elem)
                 self.clean_experimental_results(name)
         self.experiments.append( (name, path) )
         self.save()
 
 
     def experiment_exists(self, name):
+        """
+        Check if a given experiment is in the data structure
+
+        :param name: The experiment name
+        :type name: string, required
+
+        :return: exists
+        :rtype: Boolean
+        """
         for elem in self.experiments:
             if elem[0] == name:
                 return True
         return False
 
     def clean_experimental_results(self, name):
         """
         Remove all results for a given experiment
+
+        :param name: The experiment name
+        :type name: string, required
+
+        :return: None
+        :rtype: None
         """
-        self.results[name] = {}
+        if name in self.results:
+            del self.results[name]
         for dataset in self.dataresults:
-            self.dataresults[dataset][name] = {}
+            if name in self.dataresults[dataset]:
+                del self.dataresults[dataset][name]
 
     def add_dataset(self, name, path):
         """
         Add a named dataset to the project.
 
         :param name: The dataset name
         :type name: string, required
 
         :param path: The path to the data set (either local path, URL or S3 Bucket)
         :type path: string, required
+
+        :return: None
+        :rtype: None
         """
         self.datasets[name] = path
         self.save()
 
+    def rm_dataset(self, name):
+        """
+        Remove a named dataset to the project.
+
+        :param name: The dataset name (or '.' for all datasets)
+        :type path: string, required
+
+        :return: None
+        :rtype: None
+        """
+        if name in self.datasets:
+            del self.datasets[name] 
+            self.save()
+        elif name==".":
+            del self.datasets
+            self.datasets = {}
+            self.save()
+
+    def rm_experiment(self, name):
+        """
+        Remove a named experiment from the project.
+
+        :param name: The experiment name (or '.' for all experiments)
+        :type path: string, required
+
+        :return: None
+        :rtype: None
+        """
+        if name==".":
+            for elem in self.experiments:
+                self.clean_experimental_results(elem[0])
+            self.experiments = []
+            self.save()
+        else:
+            for elem in self.experiments:
+                if elem[0] == name:
+                    self.experiments.remove(elem)
+                    self.clean_experimental_results(name)
+            self.save()
+
+
     def add_param(self, name, value):
         """
         Add a parameter to the project.
 
         :param name: The parameter name
         :type name: string, required
 
         :param value: The value taken by that parameter
         :type value: Any
+
+        :return: None
+        :rtype: None
         """
         self.params[name] = value 
         self.save()
 
     def add_hyperparam(self, name, value):
         """
         Add a set of hyper parameters to the project.
 
         :param name: The experiment name
         :type name: string, required
 
         :param value: The Dictionary of hyperparameters
         :type value: Dictionary
+
+        :return: None
+        :rtype: None
         """
         if self.experiment_exists(name):
             self.hyperparams[name] = value
             self.save()
         else:
             raise Exception("ERROR: No experiment called: '%s' -- Register your experiment first." % name)
 
@@ -233,16 +432,15 @@
         for exp in self.experiments:
             key = exp[0]
             if key in myresults:
                 rez = myresults[key]
             else:
                 rez = {}
             rez['experiment'] = key
-            df = df.append(rez, ignore_index=True)
-
+            df = pd.concat([df, pd.DataFrame(rez, index=[0])], ignore_index=True)
         # Ensure that the first column in the results is "experiments"
         cols = ["experiment"]
         rest = df.columns.to_list()
         rest.remove('experiment')
         cols.extend(rest)
         return df.loc[:,cols]
 
@@ -290,19 +488,25 @@
         return False
 
     def create_local_path(self, ds):
         return self.get_root_path() + ds
 
     def save(self):
         """
-        Save your projit project. 
+        Save your projit project into config files within the projit config dir
         """
+        core_props = self.__dict__.copy()
+        del core_props['executions']
         path_to_json = self.path + "/" + config_file
         with open(path_to_json, 'w') as outfile:
-            json.dump(self.__dict__, outfile, indent=0)
+            json.dump(core_props, outfile, indent=0)
+
+        path_to_json = self.path + "/" + execution_file
+        with open(path_to_json, 'w') as outfile:
+            json.dump(self.executions, outfile, indent=0)
 
     def render(self, path):
         results = self.get_results()
         pdf = PDF()
         pdf.setup()
         pdf.add_title(self.name)
         pdf.add_description(self.desc)
@@ -320,18 +524,27 @@
 
     :param config_path: The path to the projit configuration
     :type config_path: string, required
 
     :return: Projit Object
     :rtype: Projit
     """
+    _dict = {}
     path_to_json = config_path + "/" + config_file
-    with open(path_to_json) as f:
-        _dict = json.load(f)
-    _object = Projit(**_dict)
+    if os.path.exists(path_to_json):
+        with open(path_to_json) as f:
+            _dict = json.load(f)
+
+    _execs = {}
+    path_to_execs = config_path + "/" + execution_file
+    if os.path.exists(path_to_execs):
+        with open(path_to_execs) as f:
+            _execs['executions'] = json.load(f)
+
+    _object = Projit(**_dict, **_execs )
     _object.path = config_path
     return _object
 
 ##########################################################################################
 def projit_load():
     return load( locate_projit_config() )
```

### Comparing `projit-0.1.8/projit/utils.py` & `projit-0.1.9/projit/utils.py`

 * *Files identical despite different names*

### Comparing `projit-0.1.8/projit/template.py` & `projit-0.1.9/projit/template.py`

 * *Files identical despite different names*

### Comparing `projit-0.1.8/README.md` & `projit-0.1.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,56 @@
+Metadata-Version: 2.1
+Name: projit
+Version: 0.1.9
+Summary: Python library and CLI for de-coupled data science project integration and management.
+Home-page: http://john-hawkins.github.io
+Author: John Hawkins
+Author-email: john@getting-data-science-done.com
+License: MIT
+Project-URL: Documentation, https://projit.readthedocs.io
+Project-URL: Source, https://github.com/john-hawkins/projit
+Project-URL: Tracker, https://github.com/john-hawkins/projit/issues
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
 # Projit
 ### Project Integrator for Decoupled Data Science
 
-> Status: **Beta** Functional but incomplete. This project is a work in progress.
+> Status: **Beta** Functional.
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Tests](https://github.com/john-hawkins/projit/actions/workflows/python-package.yml/badge.svg)](https://github.com/john-hawkins/projit/actions/workflows/python-package.yml)
 [![Documentation Status](https://readthedocs.org/projects/projit/badge/?version=latest)](https://projit.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/projit.svg)](https://pypi.org/project/projit)
 
 Projit is a utility to help data scientists manage projects that contain multiple experiments
 and components that need to interact in a de-coupled manner. 
-Use it define and manage project structure, properties, data, experiments & collaboration.
+Use it to define and manage project structure, properties, data, experiments & collaboration.
 
-The goal of this project is to data scientists and teams to work on projects in
+The goal of this project is to allow data scientists and teams to work on projects in
 a structured and standardized way. The projit utility allows you to establish a
 project with a centralised meta-data repository. This meta-data is used by the
 application and package to facilitate loosely coupled communication between
-scripts and experiments.
+scripts for experiments, to track results and parameters.
 
 For example, projit provides a python library that can be used inside
 experiments and scripts so references to training, evaluation and test data
 sets can accessed without passing around and maintaing paths.
 
 In addition the project can be initialised according to a standardized layout
 so that the diectory structure is familiar to all team members.
 
 This project was inspired by a combination of other projects:
 * [Cookiecutter Data Science](https://drivendata.github.io/cookiecutter-data-science/)
 * [The Python CookieCutter Application](https://cookiecutter.readthedocs.io/)
 * [The Git Source Control Utility]()
 
-To be released and distributed via setuptools/PyPI/pip for Python 3.
+Released and distributed via setuptools/PyPI/pip for Python 3.
 
-Additional detail available in the [documentation](https://projit.readthedocs.io)
+Additional details and usage instructions available in the [documentation](https://projit.readthedocs.io)
 
 
 ## Notes
 
 Initial implementation is focused allowing the user to initialise a project,
 and then modify it using a python package that can be called independently in
 scripts across the project structure. This creates a central authority for
@@ -83,14 +97,30 @@
 projit init "Test Project"
 ```
 
 This will initialise the current directory as a Data Science Project using the
 default template. Please refer to the
 [documentation for more detail on projit commands](https://projit.readthedocs.io).
 
+## Output
+
+By adding experiments and results to a projit project you can examine them.
+Example output in the table below:
+
+
+Results on [test] 
+-----------------
+| experiment | MAE      | MAPE   |
+| ----------:| --------:| ------:|
+| mytest     | 11230.46 |  13.46 |
+| mytest2    |      nan |  15.86 |
+
+
 # Acknowledgements
 
 Python package built using the
 [bootstrap cmdline template](https://github.com/jgehrcke/python-cmdline-bootstrap)
  by [jgehrcke](https://github.com/jgehrcke)
 
 
+
+
```

### Comparing `projit-0.1.8/setup.py` & `projit-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 with open("README.md", "rb") as f:
     long_descr = f.read().decode("utf-8")
 
 setup(
     name = "projit",
     packages = ["projit"],
     license = "MIT",
-    install_requires = ['numpy', 'pyyaml', 'pandas', 'fpdf'],
+    install_requires = ['numpy', 'pyyaml', 'pandas', 'fpdf', 'gitpython'],
     entry_points = {
         "console_scripts": ['projit = projit.cli:main']
     },
     include_package_data=True,
     version = version,
     description = "Python library and CLI for de-coupled data science project integration and management.",
     long_description = long_descr,
```

