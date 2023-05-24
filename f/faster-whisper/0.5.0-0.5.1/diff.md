# Comparing `tmp/faster-whisper-0.5.0.tar.gz` & `tmp/faster-whisper-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faster-whisper-0.5.0.tar", last modified: Tue Apr 25 15:02:25 2023, max compression
+gzip compressed data, was "faster-whisper-0.5.1.tar", last modified: Wed Apr 26 15:40:24 2023, max compression
```

## Comparing `faster-whisper-0.5.0.tar` & `faster-whisper-0.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:02:25.441650 faster-whisper-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-25 15:02:25.441650 faster-whisper-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:02:25.441650 faster-whisper-0.5.0/faster_whisper/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/faster_whisper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:02:25.441650 faster-whisper-0.5.0/faster_whisper/assets/
--rw-r--r--   0 runner    (1001) docker     (123)  1807524 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/faster_whisper/assets/silero_vad.onnx
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/faster_whisper/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/faster_whisper/feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/faster_whisper/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    33067 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/faster_whisper/transcribe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/faster_whisper/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/faster_whisper/vad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:02:25.441650 faster-whisper-0.5.0/faster_whisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-25 15:02:25.000000 faster-whisper-0.5.0/faster_whisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-25 15:02:25.000000 faster-whisper-0.5.0/faster_whisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:02:25.000000 faster-whisper-0.5.0/faster_whisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-25 15:02:25.000000 faster-whisper-0.5.0/faster_whisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 15:02:25.000000 faster-whisper-0.5.0/faster_whisper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-25 15:02:25.441650 faster-whisper-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-25 15:02:22.000000 faster-whisper-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:40:24.684096 faster-whisper-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-26 15:40:24.684096 faster-whisper-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:40:24.680096 faster-whisper-0.5.1/faster_whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/faster_whisper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:40:24.680096 faster-whisper-0.5.1/faster_whisper/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)  1807524 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/faster_whisper/assets/silero_vad.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/faster_whisper/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/faster_whisper/feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/faster_whisper/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33120 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/faster_whisper/transcribe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/faster_whisper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/faster_whisper/vad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:40:24.680096 faster-whisper-0.5.1/faster_whisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-26 15:40:23.000000 faster-whisper-0.5.1/faster_whisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-26 15:40:24.000000 faster-whisper-0.5.1/faster_whisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:40:23.000000 faster-whisper-0.5.1/faster_whisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-26 15:40:23.000000 faster-whisper-0.5.1/faster_whisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 15:40:23.000000 faster-whisper-0.5.1/faster_whisper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-26 15:40:24.684096 faster-whisper-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-26 15:40:11.000000 faster-whisper-0.5.1/setup.py
```

### Comparing `faster-whisper-0.5.0/LICENSE` & `faster-whisper-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.5.0/PKG-INFO` & `faster-whisper-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster-whisper
-Version: 0.5.0
+Version: 0.5.1
 Summary: Faster Whisper transcription with CTranslate2
 Home-page: https://github.com/guillaumekln/faster-whisper
 Author: Guillaume Klein
 License: MIT
 Description: [![CI](https://github.com/guillaumekln/faster-whisper/workflows/CI/badge.svg)](https://github.com/guillaumekln/faster-whisper/actions?query=workflow%3ACI) [![PyPI version](https://badge.fury.io/py/faster-whisper.svg)](https://badge.fury.io/py/faster-whisper)
         
         # Faster Whisper transcription with CTranslate2
```

### Comparing `faster-whisper-0.5.0/README.md` & `faster-whisper-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.5.0/faster_whisper/assets/silero_vad.onnx` & `faster-whisper-0.5.1/faster_whisper/assets/silero_vad.onnx`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.5.0/faster_whisper/audio.py` & `faster-whisper-0.5.1/faster_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.5.0/faster_whisper/feature_extractor.py` & `faster-whisper-0.5.1/faster_whisper/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.5.0/faster_whisper/tokenizer.py` & `faster-whisper-0.5.1/faster_whisper/tokenizer.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.5.0/faster_whisper/transcribe.py` & `faster-whisper-0.5.1/faster_whisper/transcribe.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         model_size_or_path: str,
         device: str = "auto",
         device_index: Union[int, List[int]] = 0,
         compute_type: str = "default",
         cpu_threads: int = 0,
         num_workers: int = 1,
         download_root: Optional[str] = None,
-        local_files_only: Optional[bool] = False,
+        local_files_only: bool = False,
     ):
         """Initializes the Whisper model.
 
         Args:
           model_size_or_path: Size of the model to use (tiny, tiny.en, base, base.en,
             small, small.en, medium, medium.en, large-v1, or large-v2) or a path to a converted
             model directory. When a size is configured, the converted model is downloaded
@@ -97,26 +97,28 @@
             See https://opennmt.net/CTranslate2/quantization.html.
           cpu_threads: Number of threads to use when running on CPU (4 by default).
             A non zero value overrides the OMP_NUM_THREADS environment variable.
           num_workers: When transcribe() is called from multiple Python threads,
             having multiple workers enables true parallelism when running the model
             (concurrent calls to self.model.generate() will run in parallel).
             This can improve the global throughput at the cost of increased memory usage.
-          download_root: Directory where the model should be saved. If not set, the model
-            is saved in the standard Hugging Face cache directory.
+          download_root: Directory where the models should be saved. If not set, the models
+            are saved in the standard Hugging Face cache directory.
           local_files_only:  If True, avoid downloading the file and return the path to the
             local cached file if it exists.
         """
         self.logger = get_logger()
 
         if os.path.isdir(model_size_or_path):
             model_path = model_size_or_path
         else:
             model_path = download_model(
-                model_size_or_path, download_root, local_files_only
+                model_size_or_path,
+                local_files_only=local_files_only,
+                cache_dir=download_root,
             )
 
         self.model = ctranslate2.models.Whisper(
             model_path,
             device=device,
             device_index=device_index,
             compute_type=compute_type,
```

### Comparing `faster-whisper-0.5.0/faster_whisper/utils.py` & `faster-whisper-0.5.1/faster_whisper/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,27 +30,29 @@
     """Returns the module logger."""
     return logging.getLogger("faster_whisper")
 
 
 def download_model(
     size: str,
     output_dir: Optional[str] = None,
-    local_files_only: Optional[bool] = False,
+    local_files_only: bool = False,
+    cache_dir: Optional[str] = None,
 ):
     """Downloads a CTranslate2 Whisper model from the Hugging Face Hub.
 
     The model is downloaded from https://huggingface.co/guillaumekln.
 
     Args:
       size: Size of the model to download (tiny, tiny.en, base, base.en, small, small.en,
         medium, medium.en, large-v1, or large-v2).
       output_dir: Directory where the model should be saved. If not set, the model is saved in
-        the standard Hugging Face cache directory.
+        the cache directory.
       local_files_only:  If True, avoid downloading the file and return the path to the local
         cached file if it exists.
+      cache_dir: Path to the folder where cached files are stored.
 
     Returns:
       The path to the downloaded model.
 
     Raises:
       ValueError: if the model size is invalid.
     """
@@ -62,14 +64,17 @@
     repo_id = "guillaumekln/faster-whisper-%s" % size
     kwargs = {}
     kwargs["local_files_only"] = local_files_only
     if output_dir is not None:
         kwargs["local_dir"] = output_dir
         kwargs["local_dir_use_symlinks"] = False
 
+    if cache_dir is not None:
+        kwargs["cache_dir"] = cache_dir
+
     allow_patterns = [
         "config.json",
         "model.bin",
         "tokenizer.json",
         "vocabulary.txt",
     ]
```

### Comparing `faster-whisper-0.5.0/faster_whisper/vad.py` & `faster-whisper-0.5.1/faster_whisper/vad.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-0.5.0/faster_whisper.egg-info/PKG-INFO` & `faster-whisper-0.5.1/faster_whisper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster-whisper
-Version: 0.5.0
+Version: 0.5.1
 Summary: Faster Whisper transcription with CTranslate2
 Home-page: https://github.com/guillaumekln/faster-whisper
 Author: Guillaume Klein
 License: MIT
 Description: [![CI](https://github.com/guillaumekln/faster-whisper/workflows/CI/badge.svg)](https://github.com/guillaumekln/faster-whisper/actions?query=workflow%3ACI) [![PyPI version](https://badge.fury.io/py/faster-whisper.svg)](https://badge.fury.io/py/faster-whisper)
         
         # Faster Whisper transcription with CTranslate2
```

### Comparing `faster-whisper-0.5.0/setup.py` & `faster-whisper-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 install_requires = get_requirements(os.path.join(base_dir, "requirements.txt"))
 conversion_requires = get_requirements(
     os.path.join(base_dir, "requirements.conversion.txt")
 )
 
 setup(
     name="faster-whisper",
-    version="0.5.0",
+    version="0.5.1",
     license="MIT",
     description="Faster Whisper transcription with CTranslate2",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     author="Guillaume Klein",
     url="https://github.com/guillaumekln/faster-whisper",
     classifiers=[
```

