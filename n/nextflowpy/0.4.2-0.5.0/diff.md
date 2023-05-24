# Comparing `tmp/nextflowpy-0.4.2-py3-none-any.whl.zip` & `tmp/nextflowpy-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 23266 bytes, number of entries: 10
--rw-r--r--  2.0 unx      356 b- defN 22-Oct-31 17:04 nextflow/__init__.py
+Zip file size: 23474 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      356 b- defN 22-Oct-31 17:06 nextflow/__init__.py
 -rw-r--r--  2.0 unx      148 b- defN 22-Oct-31 16:51 nextflow/exceptions.py
 -rw-r--r--  2.0 unx     9133 b- defN 22-Oct-31 17:04 nextflow/execution.py
--rw-r--r--  2.0 unx     7152 b- defN 22-Oct-31 17:03 nextflow/pipeline.py
+-rw-r--r--  2.0 unx     7652 b- defN 22-Oct-31 17:06 nextflow/pipeline.py
 -rw-r--r--  2.0 unx     6989 b- defN 22-Oct-31 17:04 nextflow/utils.py
--rw-r--r--  2.0 unx    35148 b- defN 22-Oct-31 17:05 nextflowpy-0.4.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     9803 b- defN 22-Oct-31 17:05 nextflowpy-0.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Oct-31 17:05 nextflowpy-0.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 22-Oct-31 17:05 nextflowpy-0.4.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      784 b- defN 22-Oct-31 17:05 nextflowpy-0.4.2.dist-info/RECORD
-10 files, 69614 bytes uncompressed, 21936 bytes compressed:  68.5%
+-rw-r--r--  2.0 unx    35148 b- defN 22-Oct-31 17:08 nextflowpy-0.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10131 b- defN 22-Oct-31 17:08 nextflowpy-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Oct-31 17:08 nextflowpy-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 22-Oct-31 17:08 nextflowpy-0.5.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      785 b- defN 22-Oct-31 17:08 nextflowpy-0.5.0.dist-info/RECORD
+10 files, 70443 bytes uncompressed, 22144 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: nextflow/pipeline.py
 Comment: 
 
 Filename: nextflow/utils.py
 Comment: 
 
-Filename: nextflowpy-0.4.2.dist-info/LICENSE
+Filename: nextflowpy-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: nextflowpy-0.4.2.dist-info/METADATA
+Filename: nextflowpy-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: nextflowpy-0.4.2.dist-info/WHEEL
+Filename: nextflowpy-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: nextflowpy-0.4.2.dist-info/top_level.txt
+Filename: nextflowpy-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: nextflowpy-0.4.2.dist-info/RECORD
+Filename: nextflowpy-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nextflow/__init__.py

```diff
@@ -1,12 +1,12 @@
 from shutil import which
 from .exceptions import NextflowNotInstalledError
 from .execution import Execution
 from .pipeline import Pipeline, run, run_and_poll
 
 __author__ = "Sam Ireland"
-__version__ = "0.4.2"
+__version__ = "0.5.0"
 
 if not which("nextflow"):
     raise NextflowNotInstalledError(
         "Nextflow is either not installed, not in PATH, or is not executable."
     )
```

## nextflow/pipeline.py

```diff
@@ -17,92 +17,99 @@
         self.config = config
     
 
     def __repr__(self):
         return f"<Pipeline ({self.path})>"
     
 
-    @property
-    def config_string(self):
+    def config_string(self, extra_config=None):
         """Gets the full location of the config file as a command line
         argument.
-        
+
+        :param list extra_config: any additional config files to add in.
         :rtype: ``str``"""
         
-        if not self.config: return ""
-        full_config_path = os.path.abspath(self.config)
-        return f" -C \"{full_config_path}\""
+        all_config = []
+        if self.config: all_config.append(self.config)
+        if extra_config: all_config += extra_config
+        if not all_config: return ""
+        all_config = [os.path.abspath(c) for c in all_config]
+        return " " + " ".join(f"-c \"{c}\"" for c in all_config)
     
 
-    def create_command_string(self, params, profile, version):
+    def create_command_string(self, params, profile, version, extra_config=None):
         """Creates the full command line string to run for this pipeline.
         
         :param dict params: the parameters to pass at the command line.
         :param list profile: the names of profiles to use when running.
         :param str version: the Nextflow version to use.
+        :param list extra_config: any additional config files to add in.
         :rtype: ``str``"""
         
+
         full_pipeline_location = os.path.abspath(self.path)
         param_string = " ".join([
             f"--{param[0]}='{param[1]}'" if param[1][0] not in "'\""
             else f"--{param[0]}={param[1]}" for param in params.items()
         ]) if params else ""
         profile_string = (" -profile " + ",".join(profile)) if profile else ""
         command_string = "NXF_ANSI_LOG=false "
         if version: command_string += f"NXF_VER={version} "
-        command_string += f"nextflow -Duser.country=US{self.config_string} "
+        command_string += f"nextflow -Duser.country=US{self.config_string(extra_config)} "
         command_string += f"run \"{full_pipeline_location}\" "
-        command_string += f"{param_string}{profile_string}"
+        command_string += f"{param_string}{profile_string}".strip()
         return command_string
     
     
-    def run(self, location=".", params=None, profile=None, version=None):
+    def run(self, location=".", params=None, profile=None, version=None, config=None):
         """Runs the pipeline and returns an :py:class:`.Execution` object once
         it is completed. You can specifiy where it will run, the command line
         parameters passed to it, the profile(s) it will run with, and the
         Nextflow version it will use.
         
         :param str location: the directory to run within and save outputs to.
         :param dict params: the parameters to pass at the command line.
         :param list profile: the names of profiles to use when running.
         :param str version: the Nextflow version to use.
+        :param list config: any additional config files to use.
         :rtype: ``Execution``"""
         
         full_run_location = os.path.abspath(location)
         original_location = os.getcwd()
-        command_string = self.create_command_string(params, profile, version)
+        command_string = self.create_command_string(params, profile, version, config)
         try:
             os.chdir(full_run_location)
             process = subprocess.run(
                 command_string,
                 stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                 universal_newlines=True, shell=True, cwd=full_run_location
             )
         finally: os.chdir(original_location)
         return Execution.create_from_location(
             full_run_location, self, process.stdout, process.stderr, process.returncode
         )
     
 
-    def run_and_poll(self, location=".", params=None, profile=None, version=None, sleep=5):
+    def run_and_poll(self, location=".", params=None, profile=None, version=None, config=None, sleep=5):
         """Runs the pipeline and creates :py:class:`.Execution` objects at
         intervals, returning them as a generator. You can specifiy where it will
         run, the command line parameters passed to it, the profile(s) it will
         run with, and the Nextflow version it will use.
         
         :param str location: the directory to run within and save outputs to.
         :param dict params: the parameters to pass at the command line.
         :param list profile: the names of profiles to use when running.
         :param str version: the Nextflow version to use.
+        :param list config: any additional config files to use.
         :param int sleep: the amount of time between Execution updates.
         :rtype: ``Execution``"""
         
         full_run_location = os.path.abspath(location)
         original_location = os.getcwd()
-        command_string = self.create_command_string(params, profile, version)
+        command_string = self.create_command_string(params, profile, version, config)
         try:
             os.chdir(full_run_location)
             existing_id = get_directory_id(full_run_location)
             with open("nfstdout", "w") as fout:
                 with open("nfstderr", "w") as ferr:
                     process = subprocess.Popen(
                         command_string, stdout=fout, stderr=ferr,
@@ -122,42 +129,43 @@
         finally:
             if os.path.exists("nfstdout"): os.remove("nfstdout")
             if os.path.exists("nfstderr"): os.remove("nfstderr")
             os.chdir(original_location)
 
 
 
-def run(pipeline, config, *args, **kwargs):
+def run(pipeline, *args, **kwargs):
     """Runs a pipeline by pathand returns an :py:class:`.Execution` object once
     it is completed. You can specifiy where it will run, the command line
     parameters passed to it, the profile(s) it will run with, and the
     Nextflow version it will use.
     
     :param str path: the path to the .nf file.
-    :param str config: the path to the associated config file.
     :param str location: the directory to run within and save outputs to.
     :param dict params: the parameters to pass at the command line.
     :param list profile: the names of profiles to use when running.
+    :param list config: any config files to use.
     :param str version: the Nextflow version to use.
     :rtype: ``Execution``"""
 
-    pipeline = Pipeline(path=pipeline, config=config)
+    pipeline = Pipeline(path=pipeline)
     return pipeline.run(*args, **kwargs)
 
 
-def run_and_poll(pipeline, config, *args, **kwargs):
+def run_and_poll(pipeline, *args, **kwargs):
     """Runs a pipeline by path and creates :py:class:`.Execution` objects at
     intervals, returning them as a generator. You can specifiy where it will
     run, the command line parameters passed to it, the profile(s) it will
     run with, and the Nextflow version it will use.
     
     :param str path: the path to the .nf file.
     :param str config: the path to the associated config file.
     :param str location: the directory to run within and save outputs to.
     :param dict params: the parameters to pass at the command line.
     :param list profile: the names of profiles to use when running.
+    :param list config: any config files to use.
     :param str version: the Nextflow version to use.
     :param int sleep: the amount of time between Execution updates.
     :rtype: ``Execution``"""
 
-    pipeline = Pipeline(path=pipeline, config=config)
+    pipeline = Pipeline(path=pipeline)
     return pipeline.run_and_poll(*args, **kwargs)
```

## Comparing `nextflowpy-0.4.2.dist-info/LICENSE` & `nextflowpy-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nextflowpy-0.4.2.dist-info/METADATA` & `nextflowpy-0.5.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: nextflowpy
-Version: 0.4.2
+Version: 0.5.0
 Summary: A Python wrapper around Nextflow.
 Home-page: https://github.com/goodwright/nextflow.py
 Author: Sam Ireland
 Author-email: sam@goodwright.com
-License: MIT
+License: GPLv3+
 Keywords: nextflow bioinformatics pipeline
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: !=2.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 nextflow.py
 ===========
 
 |ci| |version| |pypi| |nextfow| |license|
 
 .. |ci| image:: https://github.com/goodwright/nextflow.py/actions/workflows/main.yml/badge.svg
   :target: https://github.com/goodwright/nextflow.py/actions/workflows/main.yml
 
 .. |version| image:: https://img.shields.io/pypi/v/nextflowpy.svg
-  :target: https://pypi.org/project/nextflow/
+  :target: https://pypi.org/project/nextflowpy/
 
 .. |pypi| image:: https://img.shields.io/pypi/pyversions/nextflowpy.svg
-  :target: https://pypi.org/project/nextflow/
+  :target: https://pypi.org/project/nextflowpy/
 
 .. |nextfow| image:: https://img.shields.io/badge/Nextflow-22.04%20%7C%2021.10%20%7C%2020.10-orange
   :target: https://www.nextflow.io/
 
 .. |license| image:: https://img.shields.io/pypi/l/nextflowpy.svg?color=blue)
   :target: https://github.com/goodwright/nextflow.py/blob/master/LICENSE
 
@@ -116,20 +117,21 @@
 
     >>> execution = pipeline.run()
 
 This will return an ``Execution`` object, which represents the pipeline
 execution that just took place. You can customise the execution with various
 options:
 
-    >>> execution = pipeline.run(location="./rundir", params={"param1": "123"}, profile=["docker", "test"], version="22.0.1")
+    >>> execution = pipeline.run(location="./rundir", params={"param1": "123"}, profile=["docker", "test"], version="22.0.1", config=["env.config"])
 
 This sets the execution to take place in a different location, passes
 ``--param1=123`` as a command line argument when the pipeline is run, uses the
-Nextflow profiles 'docker' and 'test', and runs with Nextflow version 22.0.1
-(regardless of what version of Nextflow is installed).
+Nextflow profiles 'docker' and 'test', runs with Nextflow version 22.0.1
+(regardless of what version of Nextflow is installed), and passes in an extra
+config file to use on the run.
 
 Executions
 ##########
 
 An ``Execution`` represents a single execution of a
 ``Pipeline``. It has properties for:
 
@@ -218,19 +220,28 @@
 
 If you just want to run a single pipeline without initialising a
 ``Pipeline`` object first, you can ``run`` or
 ``run_and_poll`` directly, without needing to create a
 ``Pipeline``:
 
     >>> import nextflow
-    >>> execution = nextflow.run(path="pipeline.nf", config="settings.config", params={"param1": "123"})
+    >>> execution = nextflow.run(path="pipeline.nf", config=["settings.config"], params={"param1": "123"})
 
 Changelog
 ---------
 
+Release 0.5.0
+~~~~~~~~~~~~~
+
+`28th October, 2022`
+
+* Little c (`-c`) is now used instead of big C (`-C`) for passing config.
+* You can now pass multiple config files during pipeline execution.
+
+
 Release 0.4.2
 ~~~~~~~~~~~~~
 
 `26th September, 2022`
 
 * Added `bash` attribute to process executions.
```

## Comparing `nextflowpy-0.4.2.dist-info/RECORD` & `nextflowpy-0.5.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-nextflow/__init__.py,sha256=BGxAbU7Gf1Gz4xNyX_qTjcx1KRcXOhHjNJjhOhH14Hk,356
+nextflow/__init__.py,sha256=nPPMANw295PV0UKCzw0cCZ4oCe5z0QTACPhN5Xd2rHs,356
 nextflow/exceptions.py,sha256=ktaEfdLca9Bk52CtJoKYMkGaXLrQ9dZVfYh0QtSC9lk,148
 nextflow/execution.py,sha256=j_wsEuqyZafY3BapmhQBkxAmEJsnq9X-a8ADW3Bs0LA,9133
-nextflow/pipeline.py,sha256=RNSxknXluKUhxq0hcb7BRT-cmEUC5cq7ZuAvN9n3Sko,7152
+nextflow/pipeline.py,sha256=XUCsUtcGW3Ou6resfZJIWGkc5rfAq4gAY-jmZ4md9xo,7652
 nextflow/utils.py,sha256=7jSVHEc57_dZb8ZUNVrpUxIQTs3cp7wLQU9R-r-K6OE,6989
-nextflowpy-0.4.2.dist-info/LICENSE,sha256=ixuiBLtpoK3iv89l7ylKkg9rs2GzF9ukPH7ynZYzK5s,35148
-nextflowpy-0.4.2.dist-info/METADATA,sha256=F8QUPe6kO9krXVoPTizYmS8rhVl1jD3N481CSfsktVg,9803
-nextflowpy-0.4.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-nextflowpy-0.4.2.dist-info/top_level.txt,sha256=uD97_QD0Jwq__urXtKK-PQMFxiAjWT-y63C2Oi_lad0,9
-nextflowpy-0.4.2.dist-info/RECORD,,
+nextflowpy-0.5.0.dist-info/LICENSE,sha256=ixuiBLtpoK3iv89l7ylKkg9rs2GzF9ukPH7ynZYzK5s,35148
+nextflowpy-0.5.0.dist-info/METADATA,sha256=afXZO3ngnKt1X_tFvbHD9Dk2DDR6xJT0JvymShekhyo,10131
+nextflowpy-0.5.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+nextflowpy-0.5.0.dist-info/top_level.txt,sha256=uD97_QD0Jwq__urXtKK-PQMFxiAjWT-y63C2Oi_lad0,9
+nextflowpy-0.5.0.dist-info/RECORD,,
```

