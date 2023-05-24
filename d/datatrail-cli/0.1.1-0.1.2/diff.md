# Comparing `tmp/datatrail_cli-0.1.1.tar.gz` & `tmp/datatrail_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatrail_cli-0.1.1.tar", max compression
+gzip compressed data, was "datatrail_cli-0.1.2.tar", max compression
```

## Comparing `datatrail_cli-0.1.1.tar` & `datatrail_cli-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1080 2023-05-18 15:48:29.519183 datatrail_cli-0.1.1/LICENSE
--rw-r--r--   0        0        0     3492 2023-05-18 15:48:29.519183 datatrail_cli-0.1.1/README.md
--rw-r--r--   0        0        0      214 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/dtcli/__init__.py
--rw-r--r--   0        0        0      893 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/dtcli/cli.py
--rw-r--r--   0        0        0     3713 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/dtcli/config.py
--rw-r--r--   0        0        0     1062 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/dtcli/config.yaml
--rw-r--r--   0        0        0     3283 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/dtcli/ls.py
--rw-r--r--   0        0        0     4091 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/dtcli/ps.py
--rw-r--r--   0        0        0     3576 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/dtcli/pull.py
--rw-r--r--   0        0        0     8674 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/dtcli/src/functions.py
--rw-r--r--   0        0        0     8262 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/dtcli/utilities/cadcclient.py
--rw-r--r--   0        0        0     1151 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/dtcli/utilities/utilities.py
--rw-r--r--   0        0        0     1048 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4447 1970-01-01 00:00:00.000000 datatrail_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-24 15:44:32.472474 datatrail_cli-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3492 2023-05-24 15:44:32.472474 datatrail_cli-0.1.2/README.md
+-rw-r--r--   0        0        0      214 2023-05-24 15:44:32.480474 datatrail_cli-0.1.2/dtcli/__init__.py
+-rw-r--r--   0        0        0      893 2023-05-24 15:44:32.480474 datatrail_cli-0.1.2/dtcli/cli.py
+-rw-r--r--   0        0        0     3713 2023-05-24 15:44:32.480474 datatrail_cli-0.1.2/dtcli/config.py
+-rw-r--r--   0        0        0     1062 2023-05-24 15:44:32.480474 datatrail_cli-0.1.2/dtcli/config.yaml
+-rw-r--r--   0        0        0     3283 2023-05-24 15:44:32.480474 datatrail_cli-0.1.2/dtcli/ls.py
+-rw-r--r--   0        0        0     4278 2023-05-24 15:44:32.480474 datatrail_cli-0.1.2/dtcli/ps.py
+-rw-r--r--   0        0        0     3717 2023-05-24 15:44:32.480474 datatrail_cli-0.1.2/dtcli/pull.py
+-rw-r--r--   0        0        0     8674 2023-05-24 15:44:32.480474 datatrail_cli-0.1.2/dtcli/src/functions.py
+-rw-r--r--   0        0        0     8262 2023-05-24 15:44:32.484474 datatrail_cli-0.1.2/dtcli/utilities/cadcclient.py
+-rw-r--r--   0        0        0     1151 2023-05-24 15:44:32.484474 datatrail_cli-0.1.2/dtcli/utilities/utilities.py
+-rw-r--r--   0        0        0     1048 2023-05-24 15:44:32.484474 datatrail_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4447 1970-01-01 00:00:00.000000 datatrail_cli-0.1.2/PKG-INFO
```

### Comparing `datatrail_cli-0.1.1/LICENSE` & `datatrail_cli-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.1.1/README.md` & `datatrail_cli-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.1.1/dtcli/cli.py` & `datatrail_cli-0.1.2/dtcli/cli.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.1.1/dtcli/config.py` & `datatrail_cli-0.1.2/dtcli/config.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.1.1/dtcli/config.yaml` & `datatrail_cli-0.1.2/dtcli/config.yaml`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.1.1/dtcli/ls.py` & `datatrail_cli-0.1.2/dtcli/ls.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.1.1/dtcli/ps.py` & `datatrail_cli-0.1.2/dtcli/ps.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,18 @@
         title_style="bold magenta",
     )
     info_table.add_column("Storage Element", style="bold")
     info_table.add_column("Number of Files", style="green")
     info_table.add_column("Size of Files [GB]", style="green")
     if files["file_replica_locations"].get("minoc"):
         minoc_files = files["file_replica_locations"]["minoc"]
-        size = cadcclient.size(os.path.commonpath(minoc_files))
+        common_path = os.path.commonpath(minoc_files)
+        if not common_path.startswith("data") or not common_path.startswith("/data"):
+            common_path = common_path.replace("cadc:CHIMEFRB", "")
+        size = cadcclient.size(common_path)
         info_table.add_row("minoc", f"{len(minoc_files)}", f"{size:.2f}")
     else:
         info_table.add_row("minoc", str(0), str(0))
 
     # Files table
     file_table = Table(
         # header_style="magenta",
```

### Comparing `datatrail_cli-0.1.1/dtcli/pull.py` & `datatrail_cli-0.1.2/dtcli/pull.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,15 +86,18 @@
             "Configuration Missing!! Run `datatrail config init`.",
         )
         raise click.Abort()
 
     # Find files missing from localhost.
     console.print(f"\nSearching for files for {dataset} {scope}...\n")
     files = find_missing_dataset_files(scope, dataset)
-    to_download_size = size(path.commonpath(files["missing"]))
+    common_path = path.commonpath(files["missing"])
+    if common_path.startswith("cadc:CHIMEFRB"):
+        common_path = common_path.replace("cadc:CHIMEFRB", "")
+    to_download_size = size(common_path)
     console.print(
         f" - {len(files['existing'])} files found at {site}.",
         style="green",
     )
     console.print(
         f" - {len(files['missing'])} files can be downloaded from minoc.",
         style="yellow",
```

### Comparing `datatrail_cli-0.1.1/dtcli/src/functions.py` & `datatrail_cli-0.1.2/dtcli/src/functions.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.1.1/dtcli/utilities/cadcclient.py` & `datatrail_cli-0.1.2/dtcli/utilities/cadcclient.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.1.1/dtcli/utilities/utilities.py` & `datatrail_cli-0.1.2/dtcli/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.1.1/pyproject.toml` & `datatrail_cli-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datatrail-cli"
-version = "0.1.1"
+version = "0.1.2"
 description = "CHIME/FRB Datatrail CLI"
 authors = ["CHIME FRB Project Office"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "dtcli" }]
 
 [tool.poetry.dependencies]
```

### Comparing `datatrail_cli-0.1.1/PKG-INFO` & `datatrail_cli-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatrail-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: CHIME/FRB Datatrail CLI
 License: MIT
 Author: CHIME FRB Project Office
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datatrail-cli Version: 0.1.1 Summary: CHIME/FRB
+Metadata-Version: 2.1 Name: datatrail-cli Version: 0.1.2 Summary: CHIME/FRB
 Datatrail CLI License: MIT Author: CHIME FRB Project Office Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: cadcdata (>=2.4,<3.0) Requires-Dist: cadctap
 (>=0.9.11,<0.10.0) Requires-Dist: cadcutils (>=1.5.1.1,<2.0.0.0) Requires-Dist:
```

