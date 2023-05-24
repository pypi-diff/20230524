# Comparing `tmp/museval-0.3.1.tar.gz` & `tmp/museval-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/museval-0.3.1.tar", last modified: Sun Oct  4 12:14:20 2020, max compression
+gzip compressed data, was "dist/museval-0.4.0.tar", last modified: Sun Jan 31 08:47:22 2021, max compression
```

## Comparing `museval-0.3.1.tar` & `museval-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 faro       (501) staff       (20)        0 2020-10-04 12:14:20.000000 museval-0.3.1/
--rw-r--r--   0 faro       (501) staff       (20)     1063 2018-03-11 20:51:24.000000 museval-0.3.1/LICENSE
--rw-r--r--   0 faro       (501) staff       (20)       55 2020-10-04 12:05:29.000000 museval-0.3.1/MANIFEST.in
--rw-r--r--   0 faro       (501) staff       (20)    10874 2020-10-04 12:14:20.000000 museval-0.3.1/PKG-INFO
--rw-r--r--   0 faro       (501) staff       (20)     8715 2019-09-02 12:56:41.000000 museval-0.3.1/README.md
-drwxr-xr-x   0 faro       (501) staff       (20)        0 2020-10-04 12:14:20.000000 museval-0.3.1/museval/
--rw-r--r--   0 faro       (501) staff       (20)    11528 2020-02-29 10:55:53.000000 museval-0.3.1/museval/__init__.py
--rw-r--r--   0 faro       (501) staff       (20)    12794 2020-10-04 12:05:29.000000 museval-0.3.1/museval/aggregate.py
--rw-r--r--   0 faro       (501) staff       (20)     2276 2019-08-15 16:03:04.000000 museval-0.3.1/museval/cli.py
--rw-r--r--   0 faro       (501) staff       (20)    25577 2019-08-15 16:03:04.000000 museval-0.3.1/museval/metrics.py
--rw-r--r--   0 faro       (501) staff       (20)     1136 2019-08-15 16:03:04.000000 museval-0.3.1/museval/musdb.schema.json
--rw-r--r--   0 faro       (501) staff       (20)       19 2020-10-04 12:06:37.000000 museval-0.3.1/museval/version.py
-drwxr-xr-x   0 faro       (501) staff       (20)        0 2020-10-04 12:14:20.000000 museval-0.3.1/museval.egg-info/
--rw-r--r--   0 faro       (501) staff       (20)    10874 2020-10-04 12:14:20.000000 museval-0.3.1/museval.egg-info/PKG-INFO
--rw-r--r--   0 faro       (501) staff       (20)      386 2020-10-04 12:14:20.000000 museval-0.3.1/museval.egg-info/SOURCES.txt
--rw-r--r--   0 faro       (501) staff       (20)        1 2020-10-04 12:14:20.000000 museval-0.3.1/museval.egg-info/dependency_links.txt
--rw-r--r--   0 faro       (501) staff       (20)       79 2020-10-04 12:14:20.000000 museval-0.3.1/museval.egg-info/entry_points.txt
--rw-r--r--   0 faro       (501) staff       (20)        1 2018-08-21 15:44:45.000000 museval-0.3.1/museval.egg-info/not-zip-safe
--rw-r--r--   0 faro       (501) staff       (20)      163 2020-10-04 12:14:20.000000 museval-0.3.1/museval.egg-info/requires.txt
--rw-r--r--   0 faro       (501) staff       (20)        8 2020-10-04 12:14:20.000000 museval-0.3.1/museval.egg-info/top_level.txt
--rw-r--r--   0 faro       (501) staff       (20)      194 2020-10-04 12:14:20.000000 museval-0.3.1/setup.cfg
--rw-r--r--   0 faro       (501) staff       (20)     2435 2020-10-04 12:13:07.000000 museval-0.3.1/setup.py
+drwxr-xr-x   0 faro       (501) staff       (20)        0 2021-01-31 08:47:22.000000 museval-0.4.0/
+-rw-r--r--   0 faro       (501) staff       (20)     1063 2018-03-11 20:51:24.000000 museval-0.4.0/LICENSE
+-rw-r--r--   0 faro       (501) staff       (20)       55 2020-10-04 12:05:29.000000 museval-0.4.0/MANIFEST.in
+-rw-r--r--   0 faro       (501) staff       (20)    10850 2021-01-31 08:47:22.000000 museval-0.4.0/PKG-INFO
+-rw-r--r--   0 faro       (501) staff       (20)     8691 2021-01-31 08:43:09.000000 museval-0.4.0/README.md
+drwxr-xr-x   0 faro       (501) staff       (20)        0 2021-01-31 08:47:22.000000 museval-0.4.0/museval/
+-rw-r--r--   0 faro       (501) staff       (20)    11554 2020-12-17 23:28:32.000000 museval-0.4.0/museval/__init__.py
+-rw-r--r--   0 faro       (501) staff       (20)    12794 2020-10-04 12:05:29.000000 museval-0.4.0/museval/aggregate.py
+-rw-r--r--   0 faro       (501) staff       (20)     2276 2019-08-15 16:03:04.000000 museval-0.4.0/museval/cli.py
+-rw-r--r--   0 faro       (501) staff       (20)    25577 2019-08-15 16:03:04.000000 museval-0.4.0/museval/metrics.py
+-rw-r--r--   0 faro       (501) staff       (20)     1136 2019-08-15 16:03:04.000000 museval-0.4.0/museval/musdb.schema.json
+-rw-r--r--   0 faro       (501) staff       (20)       19 2021-01-31 08:43:09.000000 museval-0.4.0/museval/version.py
+drwxr-xr-x   0 faro       (501) staff       (20)        0 2021-01-31 08:47:22.000000 museval-0.4.0/museval.egg-info/
+-rw-r--r--   0 faro       (501) staff       (20)    10850 2021-01-31 08:47:22.000000 museval-0.4.0/museval.egg-info/PKG-INFO
+-rw-r--r--   0 faro       (501) staff       (20)      386 2021-01-31 08:47:22.000000 museval-0.4.0/museval.egg-info/SOURCES.txt
+-rw-r--r--   0 faro       (501) staff       (20)        1 2021-01-31 08:47:22.000000 museval-0.4.0/museval.egg-info/dependency_links.txt
+-rw-r--r--   0 faro       (501) staff       (20)       79 2021-01-31 08:47:22.000000 museval-0.4.0/museval.egg-info/entry_points.txt
+-rw-r--r--   0 faro       (501) staff       (20)        1 2018-08-21 15:44:45.000000 museval-0.4.0/museval.egg-info/not-zip-safe
+-rw-r--r--   0 faro       (501) staff       (20)      163 2021-01-31 08:47:22.000000 museval-0.4.0/museval.egg-info/requires.txt
+-rw-r--r--   0 faro       (501) staff       (20)        8 2021-01-31 08:47:22.000000 museval-0.4.0/museval.egg-info/top_level.txt
+-rw-r--r--   0 faro       (501) staff       (20)      194 2021-01-31 08:47:22.000000 museval-0.4.0/setup.cfg
+-rw-r--r--   0 faro       (501) staff       (20)     2435 2021-01-31 08:43:09.000000 museval-0.4.0/setup.py
```

### Comparing `museval-0.3.1/LICENSE` & `museval-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `museval-0.3.1/PKG-INFO` & `museval-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: museval
-Version: 0.3.1
+Version: 0.4.0
 Summary: Evaluation tools for the SIGSEP MUS database
 Home-page: https://github.com/sigsep/sigsep-mus-eval
 Author: Fabian-Robert Stoeter
 Author-email: mail@faroit.com
 License: MIT
 Description: # museval
         
-        [![Build Status](https://travis-ci.org/sigsep/sigsep-mus-eval.svg?branch=master)](https://travis-ci.org/sigsep/sigsep-mus-eval)
+        [![Build Status](https://github.com/sigsep/sigsep-mus-eval/workflows/CI/badge.svg)](https://github.com/sigsep/sigsep-mus-eval/actions?query=workflow%3ACI+branch%3Amaster+event%3Apush)
         [![Latest Version](https://img.shields.io/pypi/v/museval.svg)](https://pypi.python.org/pypi/museval)
         [![Supported Python versions](https://img.shields.io/pypi/pyversions/museval.svg)](https://pypi.python.org/pypi/museval)
         
         A python package to evaluate source separation results using the [MUSDB18](https://sigsep.github.io/musdb) dataset. This package was part of the [MUS task](https://sisec.inria.fr/home/2018-professionally-produced-music-recordings/) of the [Signal Separation Evaluation Campaign (SISEC)](https://sisec.inria.fr/).
         
         ### BSSEval v4
         
@@ -66,15 +66,15 @@
         
         Make sure `output_dir` is set. `museval` will recreate the `musdb` file structure in that folder and write the evaluation results to this folder.
         
         ### Evaluate MUSDB18 tracks later
         
         If you have already computed your estimates, we provide you with an easy-to-use function to process evaluation results afterwards.
         
-        Simply use the `museval.eval_mus_dir` to evaluate your `estimates_dir` and write the results into the `output_dir`. For convenience, the `eval_mus_dir` function accepts all parameters of the `musdb.run()`. That way e.g. multiprocessing can easily be enabled by setting `parallel=True`:
+        Simply use the `museval.eval_mus_dir` to evaluate your `estimates_dir` and write the results into the `output_dir`. For convenience, the `eval_mus_dir` function accepts all parameters of the `musdb.run()`.
         
         ```python
         import musdb
         import museval
         
         # initiate musdb
         mus = musdb.DB()
@@ -182,10 +182,10 @@
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Topic :: Multimedia :: Sound/Audio :: Sound Synthesis
 Description-Content-Type: text/markdown
+Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: tests
-Provides-Extra: docs
```

### Comparing `museval-0.3.1/README.md` & `museval-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # museval
 
-[![Build Status](https://travis-ci.org/sigsep/sigsep-mus-eval.svg?branch=master)](https://travis-ci.org/sigsep/sigsep-mus-eval)
+[![Build Status](https://github.com/sigsep/sigsep-mus-eval/workflows/CI/badge.svg)](https://github.com/sigsep/sigsep-mus-eval/actions?query=workflow%3ACI+branch%3Amaster+event%3Apush)
 [![Latest Version](https://img.shields.io/pypi/v/museval.svg)](https://pypi.python.org/pypi/museval)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/museval.svg)](https://pypi.python.org/pypi/museval)
 
 A python package to evaluate source separation results using the [MUSDB18](https://sigsep.github.io/musdb) dataset. This package was part of the [MUS task](https://sisec.inria.fr/home/2018-professionally-produced-music-recordings/) of the [Signal Separation Evaluation Campaign (SISEC)](https://sisec.inria.fr/).
 
 ### BSSEval v4
 
@@ -58,15 +58,15 @@
 
 Make sure `output_dir` is set. `museval` will recreate the `musdb` file structure in that folder and write the evaluation results to this folder.
 
 ### Evaluate MUSDB18 tracks later
 
 If you have already computed your estimates, we provide you with an easy-to-use function to process evaluation results afterwards.
 
-Simply use the `museval.eval_mus_dir` to evaluate your `estimates_dir` and write the results into the `output_dir`. For convenience, the `eval_mus_dir` function accepts all parameters of the `musdb.run()`. That way e.g. multiprocessing can easily be enabled by setting `parallel=True`:
+Simply use the `museval.eval_mus_dir` to evaluate your `estimates_dir` and write the results into the `output_dir`. For convenience, the `eval_mus_dir` function accepts all parameters of the `musdb.run()`.
 
 ```python
 import musdb
 import museval
 
 # initiate musdb
 mus = musdb.DB()
```

### Comparing `museval-0.3.1/museval/__init__.py` & `museval-0.4.0/museval/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,14 +268,15 @@
         # add vocals and accompaniments as a separate scenario
         eval_targets = ['vocals', 'accompaniment']
 
         audio_estimates = []
         audio_reference = []
 
         for target in eval_targets:
+            print(target)
             audio_estimates.append(user_estimates[target])
             audio_reference.append(track.targets[target].audio)
 
         SDR, ISR, SIR, SAR = evaluate(
             audio_reference,
             audio_estimates,
             win=int(win*track.rate),
```

### Comparing `museval-0.3.1/museval/aggregate.py` & `museval-0.4.0/museval/aggregate.py`

 * *Files identical despite different names*

### Comparing `museval-0.3.1/museval/cli.py` & `museval-0.4.0/museval/cli.py`

 * *Files identical despite different names*

### Comparing `museval-0.3.1/museval/metrics.py` & `museval-0.4.0/museval/metrics.py`

 * *Files identical despite different names*

### Comparing `museval-0.3.1/museval/musdb.schema.json` & `museval-0.4.0/museval/musdb.schema.json`

 * *Files identical despite different names*

### Comparing `museval-0.3.1/museval.egg-info/PKG-INFO` & `museval-0.4.0/museval.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: museval
-Version: 0.3.1
+Version: 0.4.0
 Summary: Evaluation tools for the SIGSEP MUS database
 Home-page: https://github.com/sigsep/sigsep-mus-eval
 Author: Fabian-Robert Stoeter
 Author-email: mail@faroit.com
 License: MIT
 Description: # museval
         
-        [![Build Status](https://travis-ci.org/sigsep/sigsep-mus-eval.svg?branch=master)](https://travis-ci.org/sigsep/sigsep-mus-eval)
+        [![Build Status](https://github.com/sigsep/sigsep-mus-eval/workflows/CI/badge.svg)](https://github.com/sigsep/sigsep-mus-eval/actions?query=workflow%3ACI+branch%3Amaster+event%3Apush)
         [![Latest Version](https://img.shields.io/pypi/v/museval.svg)](https://pypi.python.org/pypi/museval)
         [![Supported Python versions](https://img.shields.io/pypi/pyversions/museval.svg)](https://pypi.python.org/pypi/museval)
         
         A python package to evaluate source separation results using the [MUSDB18](https://sigsep.github.io/musdb) dataset. This package was part of the [MUS task](https://sisec.inria.fr/home/2018-professionally-produced-music-recordings/) of the [Signal Separation Evaluation Campaign (SISEC)](https://sisec.inria.fr/).
         
         ### BSSEval v4
         
@@ -66,15 +66,15 @@
         
         Make sure `output_dir` is set. `museval` will recreate the `musdb` file structure in that folder and write the evaluation results to this folder.
         
         ### Evaluate MUSDB18 tracks later
         
         If you have already computed your estimates, we provide you with an easy-to-use function to process evaluation results afterwards.
         
-        Simply use the `museval.eval_mus_dir` to evaluate your `estimates_dir` and write the results into the `output_dir`. For convenience, the `eval_mus_dir` function accepts all parameters of the `musdb.run()`. That way e.g. multiprocessing can easily be enabled by setting `parallel=True`:
+        Simply use the `museval.eval_mus_dir` to evaluate your `estimates_dir` and write the results into the `output_dir`. For convenience, the `eval_mus_dir` function accepts all parameters of the `musdb.run()`.
         
         ```python
         import musdb
         import museval
         
         # initiate musdb
         mus = musdb.DB()
@@ -182,10 +182,10 @@
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Topic :: Multimedia :: Sound/Audio :: Sound Synthesis
 Description-Content-Type: text/markdown
+Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: tests
-Provides-Extra: docs
```

### Comparing `museval-0.3.1/setup.py` & `museval-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                 'museval=museval.cli:museval',
                 'bsseval=museval.cli:bsseval'
             ],
         },
         # Dependencies, this installs the entire Python scientific
         # computations stack
         install_requires=[
-            'musdb>=0.3.0',
+            'musdb>=0.4.0',
             'pandas>=1.0.1',
             'numpy',
             'scipy',
             'simplejson',
             'soundfile',
             'jsonschema'
         ],
```

