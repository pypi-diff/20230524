# Comparing `tmp/speech_collator-0.1.6.tar.gz` & `tmp/speech_collator-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speech_collator-0.1.6.tar", last modified: Wed May 24 14:49:29 2023, max compression
+gzip compressed data, was "speech_collator-0.1.7.tar", last modified: Wed May 24 15:20:07 2023, max compression
```

## Comparing `speech_collator-0.1.6.tar` & `speech_collator-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      111 2023-05-14 11:12:31.266135 speech_collator-0.1.6/README.md
--rw-r--r--   0        0        0      522 2023-05-24 14:49:29.283504 speech_collator-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    15109 2023-05-14 17:05:41.228749 speech_collator-0.1.6/speech_collator/__init__.py
--rw-r--r--   0        0        0  5714361 2021-12-07 12:00:26.000000 speech_collator-0.1.6/speech_collator/data/dvector-step250000.pt
--rw-r--r--   0        0        0    62866 2021-12-07 12:00:44.000000 speech_collator-0.1.6/speech_collator/data/wav2mel.pt
--rw-r--r--   0        0        0     5126 2023-05-24 14:46:18.815009 speech_collator-0.1.6/speech_collator/measures/__init__.py
--rw-r--r--   0        0        0     2411 2023-05-14 11:28:31.387233 speech_collator-0.1.6/speech_collator/measures/snr.py
--rw-r--r--   0        0        0     2376 2023-05-14 11:28:43.968453 speech_collator-0.1.6/speech_collator/measures/srmr.py
--rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 speech_collator-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      111 2023-05-14 11:12:31.266135 speech_collator-0.1.7/README.md
+-rw-r--r--   0        0        0      522 2023-05-24 15:20:07.068060 speech_collator-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    15109 2023-05-14 17:05:41.228749 speech_collator-0.1.7/speech_collator/__init__.py
+-rw-r--r--   0        0        0  5714361 2021-12-07 12:00:26.000000 speech_collator-0.1.7/speech_collator/data/dvector-step250000.pt
+-rw-r--r--   0        0        0    62866 2021-12-07 12:00:44.000000 speech_collator-0.1.7/speech_collator/data/wav2mel.pt
+-rw-r--r--   0        0        0     5122 2023-05-24 15:19:29.401590 speech_collator-0.1.7/speech_collator/measures/__init__.py
+-rw-r--r--   0        0        0     2411 2023-05-14 11:28:31.387233 speech_collator-0.1.7/speech_collator/measures/snr.py
+-rw-r--r--   0        0        0     2376 2023-05-14 11:28:43.968453 speech_collator-0.1.7/speech_collator/measures/srmr.py
+-rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 speech_collator-0.1.7/PKG-INFO
```

### Comparing `speech_collator-0.1.6/pyproject.toml` & `speech_collator-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "speech-collator"
-version = "0.1.6"
+version = "0.1.7"
 description = "A collator for speech datasets with different batching strategies and attribute extraction."
 authors = [
     { name = "Christoph Minixhofer", email = "christoph.minixhofer@gmail.com" },
 ]
 dependencies = [
     "numpy<1.24",
     "pyworld>=0.3.3",
```

### Comparing `speech_collator-0.1.6/speech_collator/__init__.py` & `speech_collator-0.1.7/speech_collator/__init__.py`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.6/speech_collator/data/dvector-step250000.pt` & `speech_collator-0.1.7/speech_collator/data/dvector-step250000.pt`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.6/speech_collator/data/wav2mel.pt` & `speech_collator-0.1.7/speech_collator/data/wav2mel.pt`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.6/speech_collator/measures/__init__.py` & `speech_collator-0.1.7/speech_collator/measures/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,16 @@
         )
         pitch = pw.stonemask(audio.astype(np.float64), f0, t, self.sampling_rate).astype(np.float32)
         if sum(durations) < len(pitch):
             pitch = pitch[:sum(durations)]
         if silence_mask is not None:
             pitch[silence_mask] = np.nan
         pitch[pitch < 1e-6] = np.nan
-        # if np.isnan(pitch).all():
-        #     pitch[:] = 1e-6
+        if np.isnan(pitch).all():
+            pitch[:] = 1e-6
         return pitch
 
 class VoiceActivityMeasure(Measure):
     def __init__(
         self,
         name="voice_activity",
         description="Voice activity measure",
```

### Comparing `speech_collator-0.1.6/speech_collator/measures/snr.py` & `speech_collator-0.1.7/speech_collator/measures/snr.py`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.6/speech_collator/measures/srmr.py` & `speech_collator-0.1.7/speech_collator/measures/srmr.py`

 * *Files identical despite different names*

### Comparing `speech_collator-0.1.6/PKG-INFO` & `speech_collator-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speech-collator
-Version: 0.1.6
+Version: 0.1.7
 Summary: A collator for speech datasets with different batching strategies and attribute extraction.
 Author-Email: Christoph Minixhofer <christoph.minixhofer@gmail.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: numpy<1.24
 Requires-Dist: pyworld>=0.3.3
 Requires-Dist: librosa<0.10
```

