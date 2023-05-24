# Comparing `tmp/generic-etl-0.1.dev2.tar.gz` & `tmp/generic-etl-0.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generic-etl-0.1.dev2.tar", last modified: Wed Dec 14 22:51:22 2022, max compression
+gzip compressed data, was "generic-etl-0.1.dev3.tar", last modified: Mon Jan 16 23:59:13 2023, max compression
```

## Comparing `generic-etl-0.1.dev2.tar` & `generic-etl-0.1.dev3.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-12-14 22:51:22.336293 generic-etl-0.1.dev2/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      164 2022-12-14 22:51:22.332293 generic-etl-0.1.dev2/PKG-INFO
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       14 2022-10-24 22:07:11.000000 generic-etl-0.1.dev2/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-12-14 22:51:22.332293 generic-etl-0.1.dev2/etl/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       53 2022-12-14 20:00:52.000000 generic-etl-0.1.dev2/etl/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1431 2022-12-04 17:08:29.000000 generic-etl-0.1.dev2/etl/etl.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-12-14 22:51:22.332293 generic-etl-0.1.dev2/etl/functions/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2022-12-04 17:08:29.000000 generic-etl-0.1.dev2/etl/functions/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3212 2022-12-14 16:53:10.000000 generic-etl-0.1.dev2/etl/functions/general.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2793 2022-12-14 18:20:26.000000 generic-etl-0.1.dev2/etl/models.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-12-14 22:51:22.332293 generic-etl-0.1.dev2/etl/utils/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2022-11-02 13:28:05.000000 generic-etl-0.1.dev2/etl/utils/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     5092 2022-12-14 18:26:51.000000 generic-etl-0.1.dev2/etl/utils/database.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       40 2022-11-02 13:28:05.000000 generic-etl-0.1.dev2/etl/utils/exceptions.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1487 2022-12-14 22:47:58.000000 generic-etl-0.1.dev2/etl/utils/runtime.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2415 2022-12-14 18:37:40.000000 generic-etl-0.1.dev2/etl/utils/utils.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-12-14 22:51:22.332293 generic-etl-0.1.dev2/generic_etl.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      164 2022-12-14 22:51:22.000000 generic-etl-0.1.dev2/generic_etl.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      430 2022-12-14 22:51:22.000000 generic-etl-0.1.dev2/generic_etl.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2022-12-14 22:51:22.000000 generic-etl-0.1.dev2/generic_etl.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2022-12-14 22:51:22.000000 generic-etl-0.1.dev2/generic_etl.egg-info/entry_points.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      204 2022-12-14 22:51:22.000000 generic-etl-0.1.dev2/generic_etl.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        4 2022-12-14 22:51:22.000000 generic-etl-0.1.dev2/generic_etl.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2022-12-14 22:51:22.336293 generic-etl-0.1.dev2/setup.cfg
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      589 2022-12-14 22:49:03.000000 generic-etl-0.1.dev2/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-01-16 23:59:13.421685 generic-etl-0.1.dev3/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      164 2023-01-16 23:59:13.421685 generic-etl-0.1.dev3/PKG-INFO
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       14 2022-10-24 22:07:11.000000 generic-etl-0.1.dev3/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-01-16 23:59:13.421685 generic-etl-0.1.dev3/etl/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       54 2023-01-16 02:27:52.000000 generic-etl-0.1.dev3/etl/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1466 2023-01-16 03:00:13.000000 generic-etl-0.1.dev3/etl/etl.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-01-16 23:59:13.421685 generic-etl-0.1.dev3/etl/functions/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      287 2023-01-16 03:00:13.000000 generic-etl-0.1.dev3/etl/functions/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2531 2023-01-16 23:50:41.000000 generic-etl-0.1.dev3/etl/functions/ccsv.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2950 2023-01-16 03:00:13.000000 generic-etl-0.1.dev3/etl/functions/general.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1180 2023-01-16 02:56:58.000000 generic-etl-0.1.dev3/etl/models.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-01-16 23:59:13.421685 generic-etl-0.1.dev3/etl/utils/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2023-01-16 02:27:39.000000 generic-etl-0.1.dev3/etl/utils/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     5155 2023-01-16 02:34:53.000000 generic-etl-0.1.dev3/etl/utils/database.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       40 2022-11-02 13:28:05.000000 generic-etl-0.1.dev3/etl/utils/exceptions.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3741 2023-01-04 13:41:13.000000 generic-etl-0.1.dev3/etl/utils/runtime.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2351 2023-01-16 02:54:11.000000 generic-etl-0.1.dev3/etl/utils/utils.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-01-16 23:59:13.421685 generic-etl-0.1.dev3/generic_etl.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      164 2023-01-16 23:59:13.000000 generic-etl-0.1.dev3/generic_etl.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      488 2023-01-16 23:59:13.000000 generic-etl-0.1.dev3/generic_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-01-16 23:59:13.000000 generic-etl-0.1.dev3/generic_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-01-16 23:59:13.000000 generic-etl-0.1.dev3/generic_etl.egg-info/entry_points.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      204 2023-01-16 23:59:13.000000 generic-etl-0.1.dev3/generic_etl.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-01-16 23:59:13.000000 generic-etl-0.1.dev3/generic_etl.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-01-16 23:59:13.421685 generic-etl-0.1.dev3/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      614 2023-01-04 13:46:56.000000 generic-etl-0.1.dev3/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-01-16 23:59:13.421685 generic-etl-0.1.dev3/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2022-12-16 15:47:07.000000 generic-etl-0.1.dev3/tests/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1372 2023-01-16 23:58:13.000000 generic-etl-0.1.dev3/tests/conftest.py
```

### Comparing `generic-etl-0.1.dev2/etl/etl.py` & `generic-etl-0.1.dev3/etl/etl.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,39 @@
+import logging
 import sys
-from pprint import pprint as print
 
-from etl.functions.general import FUNCTIONS as FUNC
-from etl.functions.general import SUBSET_FUNCTIONS
+from etl.functions import FUNCTIONS
 from etl.models import ETL
 from etl.utils.utils import file_information, load_yaml
 
-FUNCTIONS = {}
-FUNCTIONS.update(FUNC)
-FUNCTIONS.update(SUBSET_FUNCTIONS)
+logging.basicConfig()
+logging.root.setLevel(logging.NOTSET)
+logger = logging.getLogger(__name__)
 
 
 def run(conf: ETL):
     """Runs the ETL pipeline
 
     param :conf, ETL: ETL object to run
     """
-    for k in conf.pipeline.steps:
-        for step in conf.pipeline.steps[k]:
+    for key in conf.order:
+        for step in conf.pipeline.steps[key]:
             try:
-                if step.sub_steps:
-                    for sub in step.sub_steps:
-                        sub_ = step.sub_steps[sub]
-                        FUNCTIONS[str(sub_.app).lower()](k, sub_)
-                else:
-                    FUNCTIONS[str(step.function).lower()](k, step, conf.secrets)
-
-                    if step.file_name:
-                        file_information(step.file_name, conf.meta_output)
+                for sub_step in step:
+                    logger.info("Running %s" % (sub_step))
+                    process: dict = step[sub_step]
+                    FUNCTIONS[process.get("function", None)](
+                        **process, secrets=conf.secrets
+                    )
+                    if conf.meta_output and process.get("file_output", None):
+                        file_information(process.get("file_output"), conf.meta_output)
             except KeyError as ex:
+                logger.error("Got key error, skipping...")
+                logger.error(ex)
                 print(ex)
-                continue
 
 
 def main():
     """Main function"""
     args = sys.argv
     if len(args) < 2:
         raise ValueError("Missing pipeline yaml target...")
```

### Comparing `generic-etl-0.1.dev2/etl/functions/general.py` & `generic-etl-0.1.dev3/etl/functions/general.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,101 +1,102 @@
+import logging
 import os
 import subprocess
 from pathlib import Path
 
 import pandas as pd
-from sqlalchemy.exc import OperationalError, ProgrammingError
 
-from etl.models import Step, SubStep
 from etl.utils.database import Database
 from etl.utils.exceptions import NotSupported
 
+logger = logging.getLogger(__name__)
 
-def execute_sql(title: str, step: Step, secrets: dict, output: str = "csv") -> None:
+
+def execute_sql(
+    connection: str, file_output: str, sql: str, secrets: dict, output: str = "csv", **_
+) -> None:
     """Execute SQL
 
     param :title, str: Title about to be ran
     param :step, Step: Step object
     param :secrets, dict: Connection information
     param :output, str, 'csv': Output file type
     """
-    print(f"Running {title}...")
     df = None
 
-    with Database(secrets, step.connection) as database:
-        df = database.execute(step.sql)
+    with Database(secrets, connection) as database:
+        df = database.execute(sql)
 
-    save_frame(df, step.file_name, output)
+    save_frame(df, file_output, output)
 
 
-def save_frame(df: pd.DataFrame, filename: str, output_type: str = "csv"):
+def save_frame(df: pd.DataFrame, filename: str, output_type: str = "csv", **_):
     if df is not None:
         p = Path(filename)
         p.parent.mkdir(parents=True, exist_ok=True)
-        print(f"\t\tSaving too: {filename}")
+        logger.info(f"Saving {filename}")
 
         if output_type == "csv":
             df.to_csv(filename)
         elif output_type == "hdfs":
             df.to_hdf(filename)
         elif output_type == "parquet":
             df.to_parquet(filename)
         else:
             raise NotSupported(f"{output_type}")
 
 
-def merge_csv(title: str, step: SubStep) -> None:
+def merge_csv(csv_one: str, csv_two: str, column: str, out: str, **_) -> None:
     """Merges based on the item"""
 
-    print(f"Running {title}...")
-    one: pd.DataFrame = pd.read_csv(step.csv_one)
-    two: pd.DataFrame = pd.read_csv(step.csv_two)
-    out: pd.DataFrame = pd.merge(one, two, on=step.on)
-    save_frame(out, step.csv_out, "csv")
+    one: pd.DataFrame = pd.read_csv(csv_one)
+    two: pd.DataFrame = pd.read_csv(csv_two)
+    out: pd.DataFrame = pd.merge(one, two, on=column)
+    save_frame(out, out, "csv")
 
     # chunk_container: pd.DataFrame = pd.read_csv("filename", chunksize=5000)
     # for chunk in chunk_container:
     #     chunk.to_csv("output", mode="a", index=False)
 
 
-def move_frame(title: str, step: Step, secrets: dict) -> None:
+def move_frame(
+    connection: str,
+    target_tables: str,
+    target_connection: str,
+    schema: str,
+    secrets: dict,
+    sql: str,
+    **_,
+) -> None:
     """Moves data from one table to other tables
 
     param :title, str: Title about to be ran
     param :step, Step: Step object
     param :secrets, dict: Connection information
     """
-    print(f"Running {title}...")
-    sql = step.sql
-
-    with Database(secrets, step.connection) as source:
-        with Database(secrets, step.target_connection) as target:
+    with Database(secrets, connection) as source:
+        with Database(secrets, target_connection) as target:
             for df_chunk in pd.read_sql_query(sql, source.engine, chunksize=10):
-                for table in step.target_tables:
+                for table in target_tables:
                     inital = True
                     if inital:
-                        target.execute(basic="delete")
+                        target.execute(basic="delete", table=table)
                         inital = False
 
+                    logger.info("Moving data")
                     df_chunk.to_sql(
                         table,
                         target.engine,
-                        schema=step.schema,
+                        schema=schema,
                         method="multi",
                         index=False,
                         if_exists="append",
                     )
 
 
-def sub_run(title: str, step: SubStep, output: str = "csv") -> None:
+def sub_run(app: str, io: str) -> None:
     """Runs command on a subprocess
 
-    param :title, str: Title about to be ran
     param :step, Step: Step object
     param :output, str, 'csv': Output file type
     """
-    print(f"Running {title}: \n\t\t{step}")
-    print(subprocess.call([step.app, step.io]))
-
-
-FUNCTIONS = {"sql": execute_sql, "pandas_push": move_frame}
-SUBSET_FUNCTIONS = {"cat": sub_run, "python": sub_run, "merge_csv": merge_csv}
+    logger.info(subprocess.call([app, io]))
```

### Comparing `generic-etl-0.1.dev2/etl/utils/database.py` & `generic-etl-0.1.dev3/etl/utils/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 
 BASICS = {
     "sqlite": {"delete": "DELETE FROM {table}"},
     "postgres": {"delete": "DELETE FROM {table}"},
 }
 
 
+import logging
+
+logger = logging.getLogger(__name__)
+
+
 class Database:
     target_host: str = ""
     engine: Optional[Engine] = None
     host_type: str = ""
 
     def __init__(self, secrets: dict, host: str):
         """Init function"""
@@ -56,19 +61,19 @@
             sql = sql.format(table=table)
 
         if os.path.exists(os.path.dirname(sql)):
             with open(sql, "r") as f:
                 sql = " ".join([line.strip() for line in f if line.strip()])
 
         try:
-            print(f"\t\tExecuting..{sql}")
+            logger.info(f"\t\tExecuting..{sql}")
             df = pd.read_sql(sql, self.engine)
         except Exception as ex:
-            print(ex)
-            print("Got an error skipping...")
+            logger.error(ex)
+            logger.info("continuing...")
 
         return df
 
     def _get_connection_string(self) -> Tuple[str, Engine]:
         """Returns correct engine
 
         Returns :Tuple(str,Engine): host type and engine
```

### Comparing `generic-etl-0.1.dev2/etl/utils/utils.py` & `generic-etl-0.1.dev3/etl/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import calendar
 import json
 import os
 import subprocess
 from datetime import datetime
 from pathlib import Path
 
-import dynamic_yaml
 import yaml
 from dynamic_yaml import dump as ddump
 from dynamic_yaml import load as dload
 
-from etl.models import ETL, Pipeline, Step
-
 from .exceptions import NotSupported
 
 today = datetime.today()
 RUNTIME_DEFAULTS = {
     "FIRST_DAY_MONTH": today.replace(day=1).day,
     "LAST_DAY_MONTH": calendar.monthrange(today.year, today.month)[1],
     "YEAR": today.year,
```

### Comparing `generic-etl-0.1.dev2/setup.py` & `generic-etl-0.1.dev3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from setuptools import setup, find_packages
+import os
+from setuptools import find_packages, setup
 
 setup(
     name="generic-etl",
     entry_points={"console_scripts": ["etl=etl.etl:main"]},
-    version="0.1.dev2",
+    version=os.environ.get("RELEASE"),
     packages=find_packages(),
     install_requires=[
         "dynamic-yaml==1.3.3",
         "greenlet==1.1.3.post0",
         "numpy==1.23.4",
         "pandas==1.5.1",
         "psycopg2-binary==2.9.4",
```

