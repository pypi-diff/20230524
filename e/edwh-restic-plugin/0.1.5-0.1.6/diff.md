# Comparing `tmp/edwh_restic_plugin-0.1.5.tar.gz` & `tmp/edwh_restic_plugin-0.1.6.tar.gz`

## Comparing `edwh_restic_plugin-0.1.5.tar` & `edwh_restic_plugin-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.5/CHANGELOG.md
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.5/examples/captain-hooks/backup_files.sh
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.5/examples/captain-hooks/backup_minecraft.py
--rwxr-xr-x   0        0        0      593 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.5/examples/captain-hooks/backup_stream.sh
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.5/examples/captain-hooks/backup_stream_sql.sh
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.5/examples/captain-hooks/restore_files.sh
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.5/examples/captain-hooks/restore_stream.sh
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.5/src/edwh_restic_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.5/src/edwh_restic_plugin/__init__.py
--rw-r--r--   0        0        0    28960 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.5/src/edwh_restic_plugin/tasks.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.5/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.5/LICENSE.txt
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.5/README.md
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.6/CHANGELOG.md
+-rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.6/examples/captain-hooks/backup_files.sh
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.6/examples/captain-hooks/backup_minecraft.py
+-rwxr-xr-x   0        0        0      593 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.6/examples/captain-hooks/backup_stream.sh
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.6/examples/captain-hooks/backup_stream_sql.sh
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.6/examples/captain-hooks/restore_files.sh
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.6/examples/captain-hooks/restore_stream.sh
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.6/src/edwh_restic_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.6/src/edwh_restic_plugin/__init__.py
+-rw-r--r--   0        0        0    29025 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.6/src/edwh_restic_plugin/tasks.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.6/LICENSE.txt
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.6/README.md
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.1.6/PKG-INFO
```

### Comparing `edwh_restic_plugin-0.1.5/CHANGELOG.md` & `edwh_restic_plugin-0.1.6/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.1.6 (2023-05-24)
+### Fix
+* Added error logs when giving up -v ([`0667e45`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/0667e45e52aff335f74c1712c7ebb8bba3638751))
+
 ## v0.1.5 (2023-05-24)
 ### Fix
 * Added enviroment variables HOST AND URI for restic(automaticly see https://restic.readthedocs.io/en/latest/040_backup.html?highlight=environment#environment-variables for more). ([`a836553`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/a836553c5478511c9c57416b441e027ad12df9fc))
 * Merge van sh files ([`20c198f`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/20c198ffab40165cf7a50b9dcce98a62b719ed82))
 * Added verbosity to the script output ([`30a824e`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/30a824e8f77f854fe9c201009f4013d23474f5d7))
 
 ### Documentation
```

### Comparing `edwh_restic_plugin-0.1.5/examples/captain-hooks/backup_minecraft.py` & `edwh_restic_plugin-0.1.6/examples/captain-hooks/backup_minecraft.py`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.1.5/examples/captain-hooks/backup_stream.sh` & `edwh_restic_plugin-0.1.6/examples/captain-hooks/backup_stream.sh`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.1.5/src/edwh_restic_plugin/tasks.py` & `edwh_restic_plugin-0.1.6/src/edwh_restic_plugin/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,20 +162,21 @@
 
         snapshots_created = []
         # run all backup/restore files
         for file in tqdm(files):
             if verbose:
                 print("running", file)
 
-            script_stdout = c.run(file, warn=True).stdout
+            ran_script = c.run(file, warn=True)
 
             if verbose:
-                print(script_stdout)
+                print(f"{file} output:")
+                print(f"{ran_script.stdout}\n{ran_script.stderr}")
 
-            snapshot = self.get_snapshot_from(script_stdout)
+            snapshot = self.get_snapshot_from(ran_script.stdout)
             snapshots_created.append(snapshot)
 
         # send message with backup. see message for more info
         # also if a tag in tags is None it will be removed by fix_tags
         if verb != "restore":
             tags = fix_tags(["message"] + snapshots_created)
             c.run(
```

### Comparing `edwh_restic_plugin-0.1.5/LICENSE.txt` & `edwh_restic_plugin-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.1.5/README.md` & `edwh_restic_plugin-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.1.5/pyproject.toml` & `edwh_restic_plugin-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.1.5/PKG-INFO` & `edwh_restic_plugin-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-restic-plugin
-Version: 0.1.5
+Version: 0.1.6
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-restic-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-restic-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-restic-plugin
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

