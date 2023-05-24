# Comparing `tmp/remyxai-0.1.2.tar.gz` & `tmp/remyxai-0.1.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remyxai-0.1.2.tar", last modified: Mon May 22 05:50:22 2023, max compression
+gzip compressed data, was "remyxai-0.1.2.post1.tar", last modified: Wed May 24 00:32:28 2023, max compression
```

## Comparing `remyxai-0.1.2.tar` & `remyxai-0.1.2.post1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 funk      (1000) funk      (1000)        0 2023-05-22 05:50:22.554465 remyxai-0.1.2/
--rw-rw-r--   0 funk      (1000) funk      (1000)     1065 2023-04-25 04:59:23.000000 remyxai-0.1.2/LICENSE
--rw-rw-r--   0 funk      (1000) funk      (1000)     2565 2023-05-22 05:50:22.554465 remyxai-0.1.2/PKG-INFO
--rw-rw-r--   0 funk      (1000) funk      (1000)     2451 2023-05-22 05:49:17.000000 remyxai-0.1.2/README.md
-drwxrwxr-x   0 funk      (1000) funk      (1000)        0 2023-05-22 05:50:22.550465 remyxai-0.1.2/remyxai/
--rw-rw-r--   0 funk      (1000) funk      (1000)        0 2023-04-24 16:17:23.000000 remyxai-0.1.2/remyxai/__init__.py
--rw-rw-r--   0 funk      (1000) funk      (1000)     1685 2023-05-22 02:50:15.000000 remyxai-0.1.2/remyxai/api.py
--rw-rw-r--   0 funk      (1000) funk      (1000)     4343 2023-05-22 02:45:56.000000 remyxai-0.1.2/remyxai/cli.py
--rw-rw-r--   0 funk      (1000) funk      (1000)     5721 2023-05-22 05:22:13.000000 remyxai-0.1.2/remyxai/utils.py
-drwxrwxr-x   0 funk      (1000) funk      (1000)        0 2023-05-22 05:50:22.554465 remyxai-0.1.2/remyxai.egg-info/
--rw-rw-r--   0 funk      (1000) funk      (1000)     2565 2023-05-22 05:50:22.000000 remyxai-0.1.2/remyxai.egg-info/PKG-INFO
--rw-rw-r--   0 funk      (1000) funk      (1000)      281 2023-05-22 05:50:22.000000 remyxai-0.1.2/remyxai.egg-info/SOURCES.txt
--rw-rw-r--   0 funk      (1000) funk      (1000)        1 2023-05-22 05:50:22.000000 remyxai-0.1.2/remyxai.egg-info/dependency_links.txt
--rw-rw-r--   0 funk      (1000) funk      (1000)       45 2023-05-22 05:50:22.000000 remyxai-0.1.2/remyxai.egg-info/entry_points.txt
--rw-rw-r--   0 funk      (1000) funk      (1000)       44 2023-05-22 05:50:22.000000 remyxai-0.1.2/remyxai.egg-info/requires.txt
--rw-rw-r--   0 funk      (1000) funk      (1000)        8 2023-05-22 05:50:22.000000 remyxai-0.1.2/remyxai.egg-info/top_level.txt
--rw-rw-r--   0 funk      (1000) funk      (1000)       38 2023-05-22 05:50:22.554465 remyxai-0.1.2/setup.cfg
--rw-rw-r--   0 funk      (1000) funk      (1000)      632 2023-05-22 01:31:37.000000 remyxai-0.1.2/setup.py
+drwxrwxr-x   0 funk      (1000) funk      (1000)        0 2023-05-24 00:32:28.391552 remyxai-0.1.2.post1/
+-rw-rw-r--   0 funk      (1000) funk      (1000)     1065 2023-04-25 04:59:23.000000 remyxai-0.1.2.post1/LICENSE
+-rw-rw-r--   0 funk      (1000) funk      (1000)     2805 2023-05-24 00:32:28.391552 remyxai-0.1.2.post1/PKG-INFO
+-rw-rw-r--   0 funk      (1000) funk      (1000)     2685 2023-05-24 00:00:27.000000 remyxai-0.1.2.post1/README.md
+drwxrwxr-x   0 funk      (1000) funk      (1000)        0 2023-05-24 00:32:28.391552 remyxai-0.1.2.post1/remyxai/
+-rw-rw-r--   0 funk      (1000) funk      (1000)        0 2023-04-24 16:17:23.000000 remyxai-0.1.2.post1/remyxai/__init__.py
+-rw-rw-r--   0 funk      (1000) funk      (1000)     1685 2023-05-22 19:24:51.000000 remyxai-0.1.2.post1/remyxai/api.py
+-rw-rw-r--   0 funk      (1000) funk      (1000)     4714 2023-05-24 00:04:08.000000 remyxai-0.1.2.post1/remyxai/cli.py
+-rw-rw-r--   0 funk      (1000) funk      (1000)     4987 2023-05-23 23:38:43.000000 remyxai-0.1.2.post1/remyxai/utils.py
+drwxrwxr-x   0 funk      (1000) funk      (1000)        0 2023-05-24 00:32:28.391552 remyxai-0.1.2.post1/remyxai.egg-info/
+-rw-rw-r--   0 funk      (1000) funk      (1000)     2805 2023-05-24 00:32:28.000000 remyxai-0.1.2.post1/remyxai.egg-info/PKG-INFO
+-rw-rw-r--   0 funk      (1000) funk      (1000)      281 2023-05-24 00:32:28.000000 remyxai-0.1.2.post1/remyxai.egg-info/SOURCES.txt
+-rw-rw-r--   0 funk      (1000) funk      (1000)        1 2023-05-24 00:32:28.000000 remyxai-0.1.2.post1/remyxai.egg-info/dependency_links.txt
+-rw-rw-r--   0 funk      (1000) funk      (1000)       45 2023-05-24 00:32:28.000000 remyxai-0.1.2.post1/remyxai.egg-info/entry_points.txt
+-rw-rw-r--   0 funk      (1000) funk      (1000)       44 2023-05-24 00:32:28.000000 remyxai-0.1.2.post1/remyxai.egg-info/requires.txt
+-rw-rw-r--   0 funk      (1000) funk      (1000)        8 2023-05-24 00:32:28.000000 remyxai-0.1.2.post1/remyxai.egg-info/top_level.txt
+-rw-rw-r--   0 funk      (1000) funk      (1000)       38 2023-05-24 00:32:28.391552 remyxai-0.1.2.post1/setup.cfg
+-rw-rw-r--   0 funk      (1000) funk      (1000)      634 2023-05-24 00:00:52.000000 remyxai-0.1.2.post1/setup.py
```

### Comparing `remyxai-0.1.2/LICENSE` & `remyxai-0.1.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `remyxai-0.1.2/PKG-INFO` & `remyxai-0.1.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remyxai
-Version: 0.1.2
+Version: 0.1.2.post1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Remyx AI command-line client
 
 ## Installation
 To install the Remyx AI CLI in Python virtual environment, run:
@@ -32,14 +32,25 @@
 ```
 * python command:
 ```python
 from remyxai.api import list_models
 print(list_models())
 ```
 
+Get the summary of a model:
+* cli command:
+```bash
+$ remyxai model summarize --model_name=<your-model-name>
+```
+* python command:
+```python
+from remyxai.api import get_model_summary
+print(get_model_summary(model_name))
+```
+
 Delete a model by name:
 * cli command:
 ```bash
 $ remyxai model delete --model_name=<your-model-name>
 ```
 * python command:
 ```python
@@ -106,20 +117,20 @@
 
 print(get_user_credits())
 ```
 
 ### Utils
 *New!* Label images locally:
 * cli command:
-```
+```bash
 $ remyxai utils label --labels="comma,separated,labels" --image_dir="/path/to/image/dir"
 ```
 
 * python command:
-```
+```python
 from remyxai.utils import labeler
 model_name = "<your-model-name>"
 labels = ["comma", "separated", "labels"]
 image_dir = "/path/to/image/dir"
 print(labeler(labels, image_dir, model_name))
 ```
```

### Comparing `remyxai-0.1.2/README.md` & `remyxai-0.1.2.post1/remyxai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: remyxai
+Version: 0.1.2.post1
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Remyx AI command-line client
 
 ## Installation
 To install the Remyx AI CLI in Python virtual environment, run:
 
 ```
 pip install remyxai
@@ -26,14 +32,25 @@
 ```
 * python command:
 ```python
 from remyxai.api import list_models
 print(list_models())
 ```
 
+Get the summary of a model:
+* cli command:
+```bash
+$ remyxai model summarize --model_name=<your-model-name>
+```
+* python command:
+```python
+from remyxai.api import get_model_summary
+print(get_model_summary(model_name))
+```
+
 Delete a model by name:
 * cli command:
 ```bash
 $ remyxai model delete --model_name=<your-model-name>
 ```
 * python command:
 ```python
@@ -100,20 +117,20 @@
 
 print(get_user_credits())
 ```
 
 ### Utils
 *New!* Label images locally:
 * cli command:
-```
+```bash
 $ remyxai utils label --labels="comma,separated,labels" --image_dir="/path/to/image/dir"
 ```
 
 * python command:
-```
+```python
 from remyxai.utils import labeler
 model_name = "<your-model-name>"
 labels = ["comma", "separated", "labels"]
 image_dir = "/path/to/image/dir"
 print(labeler(labels, image_dir, model_name))
 ```
```

### Comparing `remyxai-0.1.2/remyxai/api.py` & `remyxai-0.1.2.post1/remyxai/api.py`

 * *Files identical despite different names*

### Comparing `remyxai-0.1.2/remyxai/cli.py` & `remyxai-0.1.2.post1/remyxai/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,19 @@
     # Define 'model' action
     model_parser = subparsers_action.add_parser("model", help="Model-related actions")
 
     # Define subactions for 'model' action
     subparsers_model = model_parser.add_subparsers(dest="subaction", help="Model subactions")
 
     # Define 'list' subaction
-    list_parser = subparsers_model.add_parser("list", help="Create a new model")
+    list_parser = subparsers_model.add_parser("list", help="List your models")
+
+    # Define 'summary' subaction
+    summary_parser = subparsers_model.add_parser("summarize", help="Summarize a model")
+    summary_parser.add_argument("--model_name", required=True, help="Name of the model to provide a summary")
 
     # Define 'download' subaction
     download_parser = subparsers_model.add_parser("download", help="Download and convert a model")
     download_parser.add_argument("--model_name", required=True, help="Name of the model to delete")
     download_parser.add_argument("--model_format", required=True, help="of the model to delete")
 
     # Define 'delete' subaction
@@ -55,14 +59,17 @@
 
     args = parser.parse_args()
 
     if args.action == "model":
         if args.subaction == "list":
             models = list_models()
             pprint(models)
+        elif args.subaction == "summarize":
+            model_summary = get_model_summary(args.model_name)
+            pprint(model_summary)
         elif args.subaction == "delete":
             deleted_model = delete_model(args.model_name)
             pprint(deleted_model)
         elif args.subaction == "download":
             downloaded_model = download_model(args.model_name, args.model_format)
             print(downloaded_model)
         else:
```

### Comparing `remyxai-0.1.2/remyxai/utils.py` & `remyxai-0.1.2.post1/remyxai/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -96,44 +96,28 @@
     Wrapper to train a custom image classifier, 
     download model, and run inference on a folder of images.
     """
     # Step 1: Train a model if it doesn't exist
     if model_name is None:
         model_name = "labeler_{}".format("_".join(labels))
     status = get_model_summary(model_name)["message"][0]["status"]
-    if status == "ERROR":
-        print("Model is training, please wait...")
-        training_status = train_classifier(model_name, labels, "3")
-        while True:
-            status = get_model_summary(model_name)["message"][0]["status"]
-            print(f'Current model status: {status}')
-            if status == "FINISHED":
-                break
-            elif status == "RUNNING":
-                # Check back in 5 minutes:
-                time.sleep(300)
-            elif status == "FAILED":
-                print("Model training failed. Please try again.")
-                return
-    elif status != "FINISHED" and status != "ERROR":
+
+    if status == "NOT_FOUND":
         print("Model is training, please wait...")
-        while True:
-            status = get_model_summary(model_name)["message"][0]["status"]
-            print(f'Current model status: {status}')
-            if status == "FINISHED":
-                break
-            elif status == "RUNNING":
-                # Check back in 5 minutes:
-                time.sleep(300)
-            elif status == "FAILED":
-                print("Model training failed. Please try again.")
-                return
-    elif status == "FINISHED":
-        # ready to continue
-        pass
+        train_classifier(model_name, labels, "3")
+
+    while status != "FINISHED":
+        status = get_model_summary(model_name)["message"][0]["status"]
+        print(f'Current model status: {status}')
+        if status == "RUNNING":
+            # Check back in 5 minutes:
+            time.sleep(300)
+        elif status == "FAILED":
+            print("Model training failed. Please try again.")
+            return
 
     print("Model is ready for inference.")
     print("Downloading model...")
     download_message = download_model(model_name=model_name, model_format="onnx")
 
     print(download_message)
     print("Preparing for inference...")                                                                                                                                                                     
@@ -142,9 +126,8 @@
     model_assets_zip = model_assets_path + ".zip"
     with zipfile.ZipFile(model_assets_zip,"r") as zip_ref:
         zip_ref.extractall(model_assets_path)
     model = RemyxModel(model_assets_path)
 
     # Step 3: Process images
     process_message = process_images_in_directory(image_dir, model, chunk_size=8)
-    print(process_message)
-    return "Done!"
+    return process_message
```

### Comparing `remyxai-0.1.2/remyxai.egg-info/PKG-INFO` & `remyxai-0.1.2.post1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: remyxai
-Version: 0.1.2
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Remyx AI command-line client
 
 ## Installation
 To install the Remyx AI CLI in Python virtual environment, run:
 
 ```
 pip install remyxai
@@ -32,14 +26,25 @@
 ```
 * python command:
 ```python
 from remyxai.api import list_models
 print(list_models())
 ```
 
+Get the summary of a model:
+* cli command:
+```bash
+$ remyxai model summarize --model_name=<your-model-name>
+```
+* python command:
+```python
+from remyxai.api import get_model_summary
+print(get_model_summary(model_name))
+```
+
 Delete a model by name:
 * cli command:
 ```bash
 $ remyxai model delete --model_name=<your-model-name>
 ```
 * python command:
 ```python
@@ -106,20 +111,20 @@
 
 print(get_user_credits())
 ```
 
 ### Utils
 *New!* Label images locally:
 * cli command:
-```
+```bash
 $ remyxai utils label --labels="comma,separated,labels" --image_dir="/path/to/image/dir"
 ```
 
 * python command:
-```
+```python
 from remyxai.utils import labeler
 model_name = "<your-model-name>"
 labels = ["comma", "separated", "labels"]
 image_dir = "/path/to/image/dir"
 print(labeler(labels, image_dir, model_name))
 ```
```

### Comparing `remyxai-0.1.2/setup.py` & `remyxai-0.1.2.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="remyxai",
-    version="0.1.2",
+    version="0.1.2-1",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "onnx", 
         "onnxruntime",
         "pillow",
         "requests",
```

