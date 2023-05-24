# Comparing `tmp/ligo_em_bright-1.1.2.tar.gz` & `tmp/ligo_em_bright-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ligo_em_bright-1.1.2.tar", max compression
+gzip compressed data, was "ligo_em_bright-1.1.3.tar", max compression
```

## Comparing `ligo_em_bright-1.1.2.tar` & `ligo_em_bright-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1093 2023-03-15 17:51:21.569855 ligo_em_bright-1.1.2/LICENSE
--rw-r--r--   0        0        0      985 2023-03-15 17:51:21.569855 ligo_em_bright-1.1.2/README.md
--rw-r--r--   0        0        0      865 2023-04-14 20:10:24.062692 ligo_em_bright-1.1.2/ligo/em_bright/__init__.py
--rw-r--r--   0        0        0     9890 2023-04-07 01:33:56.185447 ligo_em_bright-1.1.2/ligo/em_bright/categorize.py
--rw-r--r--   0        0        0    10141 2023-04-07 01:33:56.185447 ligo_em_bright-1.1.2/ligo/em_bright/computeDiskMass.py
--rw-r--r--   0        0        0    15224 2023-04-07 01:33:56.185447 ligo_em_bright-1.1.2/ligo/em_bright/dag_writer.py
--rw-r--r--   0        0        0     2407 2023-04-07 01:33:56.185447 ligo_em_bright-1.1.2/ligo/em_bright/data/__init__.py
--rw-r--r--   0        0        0     8466 2023-04-07 01:33:56.185447 ligo_em_bright-1.1.2/ligo/em_bright/em_bright.py
--rw-r--r--   0        0        0        0 2023-03-15 17:51:21.925857 ligo_em_bright-1.1.2/ligo/em_bright/tests/__init__.py
--rw-r--r--   0        0        0      307 2023-03-15 17:51:21.925857 ligo_em_bright-1.1.2/ligo/em_bright/tests/data/test_categorize_data.tbl
--rw-r--r--   0        0        0     8100 2023-04-14 20:10:52.375803 ligo_em_bright-1.1.2/ligo/em_bright/tests/test_em_bright.py
--rw-r--r--   0        0        0    23921 2023-04-07 01:46:47.038281 ligo_em_bright-1.1.2/ligo/em_bright/utils.py
--rw-r--r--   0        0        0     1382 2023-04-14 19:58:52.401702 ligo_em_bright-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1700 1970-01-01 00:00:00.000000 ligo_em_bright-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-03-15 17:51:21.569855 ligo_em_bright-1.1.3/LICENSE
+-rw-r--r--   0        0        0      985 2023-03-15 17:51:21.569855 ligo_em_bright-1.1.3/README.md
+-rw-r--r--   0        0        0      865 2023-05-24 19:32:44.968092 ligo_em_bright-1.1.3/ligo/em_bright/__init__.py
+-rw-r--r--   0        0        0     9890 2023-04-07 01:33:56.185447 ligo_em_bright-1.1.3/ligo/em_bright/categorize.py
+-rw-r--r--   0        0        0    10141 2023-04-07 01:33:56.185447 ligo_em_bright-1.1.3/ligo/em_bright/computeDiskMass.py
+-rw-r--r--   0        0        0    15224 2023-04-07 01:33:56.185447 ligo_em_bright-1.1.3/ligo/em_bright/dag_writer.py
+-rw-r--r--   0        0        0     2407 2023-04-07 01:33:56.185447 ligo_em_bright-1.1.3/ligo/em_bright/data/__init__.py
+-rw-r--r--   0        0        0     8588 2023-05-24 19:22:27.251422 ligo_em_bright-1.1.3/ligo/em_bright/em_bright.py
+-rw-r--r--   0        0        0        0 2023-03-15 17:51:21.925857 ligo_em_bright-1.1.3/ligo/em_bright/tests/__init__.py
+-rw-r--r--   0        0        0      307 2023-03-15 17:51:21.925857 ligo_em_bright-1.1.3/ligo/em_bright/tests/data/test_categorize_data.tbl
+-rw-r--r--   0        0        0     8756 2023-05-24 19:32:44.968092 ligo_em_bright-1.1.3/ligo/em_bright/tests/test_em_bright.py
+-rw-r--r--   0        0        0    23921 2023-04-07 01:46:47.038281 ligo_em_bright-1.1.3/ligo/em_bright/utils.py
+-rw-r--r--   0        0        0     1382 2023-05-24 19:32:44.968092 ligo_em_bright-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1700 1970-01-01 00:00:00.000000 ligo_em_bright-1.1.3/PKG-INFO
```

### Comparing `ligo_em_bright-1.1.2/LICENSE` & `ligo_em_bright-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ligo_em_bright-1.1.2/README.md` & `ligo_em_bright-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ligo_em_bright-1.1.2/ligo/em_bright/__init__.py` & `ligo_em_bright-1.1.3/ligo/em_bright/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.1.2'
+__version__ = '1.1.3'
 
 PACKAGE_DATA_BASE_URL = (
     'https://git.ligo.org/emfollow/em-properties/em-bright/'
     f'-/raw/v{__version__}/ligo/em_bright/data'
 )
 
 PACKAGE_DATA_LINKS = {name: f'{PACKAGE_DATA_BASE_URL}/{name}' for name in (
```

### Comparing `ligo_em_bright-1.1.2/ligo/em_bright/categorize.py` & `ligo_em_bright-1.1.3/ligo/em_bright/categorize.py`

 * *Files identical despite different names*

### Comparing `ligo_em_bright-1.1.2/ligo/em_bright/computeDiskMass.py` & `ligo_em_bright-1.1.3/ligo/em_bright/computeDiskMass.py`

 * *Files identical despite different names*

### Comparing `ligo_em_bright-1.1.2/ligo/em_bright/dag_writer.py` & `ligo_em_bright-1.1.3/ligo/em_bright/dag_writer.py`

 * *Files identical despite different names*

### Comparing `ligo_em_bright-1.1.2/ligo/em_bright/data/__init__.py` & `ligo_em_bright-1.1.3/ligo/em_bright/data/__init__.py`

 * *Files identical despite different names*

### Comparing `ligo_em_bright-1.1.2/ligo/em_bright/em_bright.py` & `ligo_em_bright-1.1.3/ligo/em_bright/em_bright.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,18 +194,22 @@
         except ValueError:
             chirp_mass, mass_ratio = samples['chirp_mass'], samples['mass_ratio']  # noqa:E501
             chirp_mass = chirp_mass/(1 + redshifts)
             mass_1 = chirp_mass * (1 + mass_ratio)**(1/5) * (mass_ratio)**(-3/5)  # noqa:E501
             mass_2 = chirp_mass * (1 + mass_ratio)**(1/5) * (mass_ratio)**(2/5)
 
     try:
-        a_1 = samples['a_1'] * np.cos(samples['tilt_1'])
-        a_2 = samples['a_2'] * np.cos(samples['tilt_2'])
+        a_1 = samples["spin_1z"]
+        a_2 = samples["spin_2z"]
     except ValueError:
-        a_1, a_2 = np.zeros(len(mass_1)), np.zeros(len(mass_2))
+        try:
+            a_1 = samples['a_1'] * np.cos(samples['tilt_1'])
+            a_2 = samples['a_2'] * np.cos(samples['tilt_2'])
+        except ValueError:
+            a_1, a_2 = np.zeros(len(mass_1)), np.zeros(len(mass_2))
 
     if num_eos_draws:
         np.random.seed(eos_seed)
         prediction_nss, prediction_ems = [], []
         for m1, m2, a1, a2 in zip(mass_1, mass_2, a_1, a_2):
             rand_subset = np.random.choice(
                 len(ALL_EOS_DRAWS), num_eos_draws if num_eos_draws < len(ALL_EOS_DRAWS) else len(ALL_EOS_DRAWS))  # noqa:E501
```

### Comparing `ligo_em_bright-1.1.2/ligo/em_bright/tests/test_em_bright.py` & `ligo_em_bright-1.1.3/ligo/em_bright/tests/test_em_bright.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from .. import em_bright, categorize, utils
 from ..data import EOS_MAX_MASS
 
 
 def test_version():
     from .. import __version__
-    assert __version__ == '1.1.2'
+    assert __version__ == '1.1.3'
 
 
 @pytest.mark.parametrize(
     'posteriors, dtype, result, result_eos',
     [[[(1.2, 1.0, 0.0, 0.0, 0.0, 0.0, 100.0),
        (2.0, 0.5, 0.99, 0.99, 0.0, 0.0, 150.0)],
       [('chirp_mass', '<f8'), ('mass_ratio', '<f8'), ('a_1', '<f8'),
@@ -56,15 +56,27 @@
      [('ra', '<f8'), ('dec', '<f8'), ('luminosity_distance', '<f8'),
       ('time', '<f8'), ('mass_1', '<f8'), ('mass_2', '<f8')],
      (0.0, 0.0, 1.0), (0.0, 0.0, 1.0)],
      [[(4.5, -0.1, 200.0, 100000, 40.5, 4.4),
        (1.6, 0.3, 201.0, 100000, 40.3, 4.2)],
      [('ra', '<f8'), ('dec', '<f8'), ('luminosity_distance', '<f8'),
       ('time', '<f8'), ('mass_1', '<f8'), ('mass_2', '<f8')],
-     (0.0, 0.0, 1.0), (0.0, 0.0, 1.0)]]
+     (0.0, 0.0, 1.0), (0.0, 0.0, 1.0)],
+     [[(4.5, -0.1, 200.0, 1.0, 2.0, 2.0, 0.0, 0.0),
+       (1.6, 0.3, 201.0, 1.0, 5.0, 2.0, 0.0, 0.0)],
+     [('ra', '<f8'), ('dec', '<f8'), ('luminosity_distance', '<f8'),
+      ('time', '<f8'), ('mass_1', '<f8'), ('mass_2', '<f8'),
+      ('spin_1z', '<f8'), ('spin_2z', '<f8')],
+     (1.0, 0.5, 0.5), (1.0, 0.5, 0.5)],
+     [[(4.5, -0.1, 200.0, 1.0, 2.0, 2.0, 0.99, 0.0),
+       (1.6, 0.3, 201.0, 1.0, 5.0, 2.0, 0.99, 0.0)],
+     [('ra', '<f8'), ('dec', '<f8'), ('luminosity_distance', '<f8'),
+      ('time', '<f8'), ('mass_1', '<f8'), ('mass_2', '<f8'),
+      ('spin_1z', '<f8'), ('spin_2z', '<f8')],
+     (1.0, 1.0, 0.5), (1.0, 0.5, 0.5)]]
 )
 def test_source_classification_pe(posteriors, dtype, result, result_eos):
     """Test em_bright classification from posterior
     samples - both aligned and precessing cases.
     """
     with NamedTemporaryFile() as f:
         filename = f.name
```

### Comparing `ligo_em_bright-1.1.2/ligo/em_bright/utils.py` & `ligo_em_bright-1.1.3/ligo/em_bright/utils.py`

 * *Files identical despite different names*

### Comparing `ligo_em_bright-1.1.2/pyproject.toml` & `ligo_em_bright-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ligo.em-bright"
-version = "1.1.2"
+version = "1.1.3"
 description = "Possibility and properties of Electromagnetically-bright sources of gravitational-wave events"
 readme = "README.md"
 authors = [
     "Deep Chatterjee <deep.chatterjee@ligo.org>",
     "Shaon Ghosh <shaon.ghosh@ligo.org>"]
 packages = [
     { include = "ligo" },
```

### Comparing `ligo_em_bright-1.1.2/PKG-INFO` & `ligo_em_bright-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo-em-bright
-Version: 1.1.2
+Version: 1.1.3
 Summary: Possibility and properties of Electromagnetically-bright sources of gravitational-wave events
 License: MIT
 Author: Deep Chatterjee
 Author-email: deep.chatterjee@ligo.org
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

