# Comparing `tmp/pyNAVIS-1.1.4.tar.gz` & `tmp/pyNAVIS-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyNAVIS-1.1.4.tar", last modified: Sun May  7 08:18:49 2023, max compression
+gzip compressed data, was "pyNAVIS-1.1.5.tar", last modified: Wed May 24 18:49:41 2023, max compression
```

## Comparing `pyNAVIS-1.1.4.tar` & `pyNAVIS-1.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 08:18:49.701945 pyNAVIS-1.1.4/
--rw-rw-rw-   0        0        0     5225 2023-05-07 08:18:49.700943 pyNAVIS-1.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-07 08:18:49.669732 pyNAVIS-1.1.4/pyNAVIS/
--rw-rw-rw-   0        0        0      399 2023-05-06 10:02:02.000000 pyNAVIS-1.1.4/pyNAVIS/__init__.py
--rw-rw-rw-   0        0        0     8409 2023-05-06 10:00:39.000000 pyNAVIS-1.1.4/pyNAVIS/dataset_gen.py
--rw-rw-rw-   0        0        0    18813 2023-05-07 08:18:01.000000 pyNAVIS-1.1.4/pyNAVIS/functions.py
--rw-rw-rw-   0        0        0     8149 2022-03-30 06:38:38.000000 pyNAVIS-1.1.4/pyNAVIS/generators.py
--rw-rw-rw-   0        0        0    22338 2022-03-30 06:38:38.000000 pyNAVIS-1.1.4/pyNAVIS/loaders.py
--rw-rw-rw-   0        0        0     5287 2022-03-30 06:38:38.000000 pyNAVIS-1.1.4/pyNAVIS/main_settings.py
--rw-rw-rw-   0        0        0     2268 2022-03-30 06:38:38.000000 pyNAVIS-1.1.4/pyNAVIS/objects.py
--rw-rw-rw-   0        0        0    35388 2023-05-06 10:22:35.000000 pyNAVIS-1.1.4/pyNAVIS/plots.py
--rw-rw-rw-   0        0        0     7950 2022-03-30 06:38:38.000000 pyNAVIS-1.1.4/pyNAVIS/report_functions.py
--rw-rw-rw-   0        0        0    10205 2022-03-30 06:38:38.000000 pyNAVIS-1.1.4/pyNAVIS/savers.py
--rw-rw-rw-   0        0        0     9241 2022-03-30 06:38:38.000000 pyNAVIS-1.1.4/pyNAVIS/splitters.py
--rw-rw-rw-   0        0        0     3974 2022-03-30 06:38:38.000000 pyNAVIS-1.1.4/pyNAVIS/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-07 08:18:49.693791 pyNAVIS-1.1.4/pyNAVIS.egg-info/
--rw-rw-rw-   0        0        0     5225 2023-05-07 08:18:49.000000 pyNAVIS-1.1.4/pyNAVIS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      412 2023-05-07 08:18:49.000000 pyNAVIS-1.1.4/pyNAVIS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 08:18:49.000000 pyNAVIS-1.1.4/pyNAVIS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-07 08:18:49.000000 pyNAVIS-1.1.4/pyNAVIS.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-07 08:18:49.000000 pyNAVIS-1.1.4/pyNAVIS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 08:18:49.701945 pyNAVIS-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      979 2023-05-07 08:18:32.000000 pyNAVIS-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:49:41.852816 pyNAVIS-1.1.5/
+-rw-rw-rw-   0        0        0     5225 2023-05-24 18:49:41.852816 pyNAVIS-1.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-24 18:49:41.746606 pyNAVIS-1.1.5/pyNAVIS/
+-rw-rw-rw-   0        0        0      399 2023-05-06 10:02:02.000000 pyNAVIS-1.1.5/pyNAVIS/__init__.py
+-rw-rw-rw-   0        0        0     8409 2023-05-06 10:00:39.000000 pyNAVIS-1.1.5/pyNAVIS/dataset_gen.py
+-rw-rw-rw-   0        0        0    18837 2023-05-24 18:46:46.000000 pyNAVIS-1.1.5/pyNAVIS/functions.py
+-rw-rw-rw-   0        0        0     8149 2022-03-30 06:38:38.000000 pyNAVIS-1.1.5/pyNAVIS/generators.py
+-rw-rw-rw-   0        0        0    22338 2022-03-30 06:38:38.000000 pyNAVIS-1.1.5/pyNAVIS/loaders.py
+-rw-rw-rw-   0        0        0     5287 2022-03-30 06:38:38.000000 pyNAVIS-1.1.5/pyNAVIS/main_settings.py
+-rw-rw-rw-   0        0        0     2268 2022-03-30 06:38:38.000000 pyNAVIS-1.1.5/pyNAVIS/objects.py
+-rw-rw-rw-   0        0        0    35388 2023-05-06 10:22:35.000000 pyNAVIS-1.1.5/pyNAVIS/plots.py
+-rw-rw-rw-   0        0        0     7950 2022-03-30 06:38:38.000000 pyNAVIS-1.1.5/pyNAVIS/report_functions.py
+-rw-rw-rw-   0        0        0    10205 2022-03-30 06:38:38.000000 pyNAVIS-1.1.5/pyNAVIS/savers.py
+-rw-rw-rw-   0        0        0     9241 2022-03-30 06:38:38.000000 pyNAVIS-1.1.5/pyNAVIS/splitters.py
+-rw-rw-rw-   0        0        0     3974 2022-03-30 06:38:38.000000 pyNAVIS-1.1.5/pyNAVIS/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:49:41.778143 pyNAVIS-1.1.5/pyNAVIS.egg-info/
+-rw-rw-rw-   0        0        0     5225 2023-05-24 18:49:41.000000 pyNAVIS-1.1.5/pyNAVIS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-05-24 18:49:41.000000 pyNAVIS-1.1.5/pyNAVIS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 18:49:41.000000 pyNAVIS-1.1.5/pyNAVIS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-24 18:49:41.000000 pyNAVIS-1.1.5/pyNAVIS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-24 18:49:41.000000 pyNAVIS-1.1.5/pyNAVIS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 18:49:41.852816 pyNAVIS-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      979 2023-05-24 18:49:17.000000 pyNAVIS-1.1.5/setup.py
```

### Comparing `pyNAVIS-1.1.4/PKG-INFO` & `pyNAVIS-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNAVIS
-Version: 1.1.4
+Version: 1.1.5
 Summary: Useful tools to analyze and process spiking information from neuromorphic auditory sensors.
 Home-page: https://github.com/jpdominguez/pyNAVIS
 Download-URL: https://pypi.org/project/pyNAVIS/
 Author: Juan P. Dominguez-Morales
 Author-email: jpdominguez@us.es
 License: GPL
 Keywords: pyNAVIS,NAVIS,neuromorphic engineering,neuromorphic audio processing,neuromorphic sensors
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyNAVIS Version: 1.1.4 Summary: Useful tools to
+Metadata-Version: 2.1 Name: pyNAVIS Version: 1.1.5 Summary: Useful tools to
 analyze and process spiking information from neuromorphic auditory sensors.
 Home-page: https://github.com/jpdominguez/pyNAVIS Download-URL: https://
 pypi.org/project/pyNAVIS/ Author: Juan P. Dominguez-Morales Author-email:
 jpdominguez@us.es License: GPL Keywords: pyNAVIS,NAVIS,neuromorphic
 engineering,neuromorphic audio processing,neuromorphic sensors Description-
 Content-Type: text/markdown ## pyNAVIS: an open-source cross-platform
 Neuromorphic Auditory VISualizer
```

### Comparing `pyNAVIS-1.1.4/pyNAVIS/dataset_gen.py` & `pyNAVIS-1.1.5/pyNAVIS/dataset_gen.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.4/pyNAVIS/functions.py` & `pyNAVIS-1.1.5/pyNAVIS/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 				SettingsError: If the on_off_both parameter is not set to 1 (both) in the MainSettings.
 		"""
 
 		if settings.on_off_both == 1:
 			prevSpike = [None] * (settings.num_channels) * (1 + settings.mono_stereo)
 			phaseLockedAddrs = []
 			phaseLockedTs = []
-			for i in range(len(spikes_file.addresses)):
+			for i in range(len(spikes_file.addressebrew install openssl@1.1s)):
 				if prevSpike[spikes_file.addresses[i]//2] == None:
 					prevSpike[spikes_file.addresses[i]//2] = spikes_file.addresses[i]%2
 				else:
 					if (prevSpike[spikes_file.addresses[i]//2] == 0 and spikes_file.addresses[i]%2 == 1) or ((prevSpike[spikes_file.addresses[i]//2] == 1 and spikes_file.addresses[i]%2 == 0) and posNeg_both):
 						phaseLockedAddrs.append(spikes_file.addresses[i]//2)
 						phaseLockedTs.append(spikes_file.timestamps[i])
 						prevSpike[spikes_file.addresses[i]//2] = spikes_file.addresses[i]%2
```

### Comparing `pyNAVIS-1.1.4/pyNAVIS/generators.py` & `pyNAVIS-1.1.5/pyNAVIS/generators.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.4/pyNAVIS/loaders.py` & `pyNAVIS-1.1.5/pyNAVIS/loaders.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.4/pyNAVIS/main_settings.py` & `pyNAVIS-1.1.5/pyNAVIS/main_settings.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.4/pyNAVIS/objects.py` & `pyNAVIS-1.1.5/pyNAVIS/objects.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.4/pyNAVIS/plots.py` & `pyNAVIS-1.1.5/pyNAVIS/plots.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.4/pyNAVIS/report_functions.py` & `pyNAVIS-1.1.5/pyNAVIS/report_functions.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.4/pyNAVIS/savers.py` & `pyNAVIS-1.1.5/pyNAVIS/savers.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.4/pyNAVIS/splitters.py` & `pyNAVIS-1.1.5/pyNAVIS/splitters.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.4/pyNAVIS/utils.py` & `pyNAVIS-1.1.5/pyNAVIS/utils.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.4/pyNAVIS.egg-info/PKG-INFO` & `pyNAVIS-1.1.5/pyNAVIS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNAVIS
-Version: 1.1.4
+Version: 1.1.5
 Summary: Useful tools to analyze and process spiking information from neuromorphic auditory sensors.
 Home-page: https://github.com/jpdominguez/pyNAVIS
 Download-URL: https://pypi.org/project/pyNAVIS/
 Author: Juan P. Dominguez-Morales
 Author-email: jpdominguez@us.es
 License: GPL
 Keywords: pyNAVIS,NAVIS,neuromorphic engineering,neuromorphic audio processing,neuromorphic sensors
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyNAVIS Version: 1.1.4 Summary: Useful tools to
+Metadata-Version: 2.1 Name: pyNAVIS Version: 1.1.5 Summary: Useful tools to
 analyze and process spiking information from neuromorphic auditory sensors.
 Home-page: https://github.com/jpdominguez/pyNAVIS Download-URL: https://
 pypi.org/project/pyNAVIS/ Author: Juan P. Dominguez-Morales Author-email:
 jpdominguez@us.es License: GPL Keywords: pyNAVIS,NAVIS,neuromorphic
 engineering,neuromorphic audio processing,neuromorphic sensors Description-
 Content-Type: text/markdown ## pyNAVIS: an open-source cross-platform
 Neuromorphic Auditory VISualizer
```

### Comparing `pyNAVIS-1.1.4/setup.py` & `pyNAVIS-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     README = readme_file.read()
 """
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 """
 setup_args = dict(
     name='pyNAVIS',
-    version='1.1.4',
+    version='1.1.5',
     description='Useful tools to analyze and process spiking information from neuromorphic auditory sensors.',
     long_description_content_type="text/markdown",
     long_description=README,
     license='GPL',
     packages=find_packages(),
     author='Juan P. Dominguez-Morales',
     author_email='jpdominguez@us.es',
```

