# Comparing `tmp/komm-0.7.3.tar.gz` & `tmp/komm-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "komm-0.7.3.tar", last modified: Fri May 19 20:27:46 2023, max compression
+gzip compressed data, was "komm-0.7.4.tar", last modified: Wed May 24 20:32:30 2023, max compression
```

## Comparing `komm-0.7.3.tar` & `komm-0.7.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-19 20:27:46.246847 komm-0.7.3/
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    35147 2022-07-22 15:17:50.000000 komm-0.7.3/LICENSE
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1372 2023-05-19 20:27:46.243513 komm-0.7.3/PKG-INFO
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1757 2023-05-13 23:19:40.000000 komm-0.7.3/README.rst
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-19 20:27:46.230180 komm-0.7.3/komm/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      620 2023-05-13 23:18:38.000000 komm-0.7.3/komm/__init__.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    32335 2023-05-13 23:09:56.000000 komm-0.7.3/komm/_algebra.py
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      189 2022-07-22 15:17:50.000000 komm-0.7.3/komm/_aux.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    14964 2023-05-19 20:25:27.000000 komm-0.7.3/komm/_channels.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    67646 2023-05-13 23:12:00.000000 komm-0.7.3/komm/_error_control_block.py
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      123 2022-07-22 15:17:50.000000 komm-0.7.3/komm/_error_control_checksum.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    20369 2023-05-13 23:09:56.000000 komm-0.7.3/komm/_error_control_convolutional.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    18086 2023-05-13 23:08:37.000000 komm-0.7.3/komm/_finite_state_machine.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    30566 2023-05-13 23:11:52.000000 komm-0.7.3/komm/_modulation.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    14874 2023-05-13 23:08:37.000000 komm-0.7.3/komm/_pulses.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     8251 2023-05-13 23:08:37.000000 komm-0.7.3/komm/_quantization.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    19729 2023-05-13 23:08:28.000000 komm-0.7.3/komm/_sequences.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    19050 2022-07-22 15:17:50.000000 komm-0.7.3/komm/_source_coding.py
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2190 2023-05-13 23:08:37.000000 komm-0.7.3/komm/_sources.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     5404 2023-05-13 23:36:24.000000 komm-0.7.3/komm/_util.py
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-19 20:27:46.230180 komm-0.7.3/komm.egg-info/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1372 2023-05-19 20:27:46.000000 komm-0.7.3/komm.egg-info/PKG-INFO
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      791 2023-05-19 20:27:46.000000 komm-0.7.3/komm.egg-info/SOURCES.txt
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        1 2023-05-19 20:27:46.000000 komm-0.7.3/komm.egg-info/dependency_links.txt
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       12 2023-05-19 20:27:46.000000 komm-0.7.3/komm.egg-info/requires.txt
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        5 2023-05-19 20:27:46.000000 komm-0.7.3/komm.egg-info/top_level.txt
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       38 2023-05-19 20:27:46.246847 komm-0.7.3/setup.cfg
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1623 2023-05-19 20:26:34.000000 komm-0.7.3/setup.py
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-19 20:27:46.240180 komm-0.7.3/tests/
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     7141 2022-07-22 15:17:50.000000 komm-0.7.3/tests/test_algebra.py
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      509 2022-07-22 15:17:50.000000 komm-0.7.3/tests/test_channels.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    14875 2023-05-13 23:08:28.000000 komm-0.7.3/tests/test_error_control_block.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     8605 2023-05-13 23:08:28.000000 komm-0.7.3/tests/test_error_control_convolutional.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2661 2022-07-22 15:17:50.000000 komm-0.7.3/tests/test_finite_state_machine.py
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1860 2022-07-22 15:17:50.000000 komm-0.7.3/tests/test_modulation.py
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1802 2022-07-22 15:17:50.000000 komm-0.7.3/tests/test_quantization.py
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      976 2023-05-13 23:08:28.000000 komm-0.7.3/tests/test_sequences.py
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3028 2022-07-22 15:17:50.000000 komm-0.7.3/tests/test_source_coding.py
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      289 2023-05-13 23:08:28.000000 komm-0.7.3/tests/test_sources.py
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      509 2022-07-22 15:17:50.000000 komm-0.7.3/tests/test_util.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-24 20:32:30.483378 komm-0.7.4/
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    35147 2022-07-22 15:17:50.000000 komm-0.7.4/LICENSE
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1372 2023-05-24 20:32:30.483378 komm-0.7.4/PKG-INFO
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1757 2023-05-13 23:19:40.000000 komm-0.7.4/README.rst
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-24 20:32:30.473378 komm-0.7.4/komm/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      620 2023-05-13 23:18:38.000000 komm-0.7.4/komm/__init__.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    32335 2023-05-13 23:09:56.000000 komm-0.7.4/komm/_algebra.py
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      189 2022-07-22 15:17:50.000000 komm-0.7.4/komm/_aux.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    15361 2023-05-24 18:32:24.000000 komm-0.7.4/komm/_channels.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    67646 2023-05-13 23:12:00.000000 komm-0.7.4/komm/_error_control_block.py
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      123 2022-07-22 15:17:50.000000 komm-0.7.4/komm/_error_control_checksum.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    20369 2023-05-13 23:09:56.000000 komm-0.7.4/komm/_error_control_convolutional.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    18086 2023-05-13 23:08:37.000000 komm-0.7.4/komm/_finite_state_machine.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    30566 2023-05-13 23:11:52.000000 komm-0.7.4/komm/_modulation.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    14874 2023-05-13 23:08:37.000000 komm-0.7.4/komm/_pulses.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     8251 2023-05-13 23:08:37.000000 komm-0.7.4/komm/_quantization.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    19729 2023-05-13 23:08:28.000000 komm-0.7.4/komm/_sequences.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    19050 2022-07-22 15:17:50.000000 komm-0.7.4/komm/_source_coding.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2484 2023-05-24 18:32:24.000000 komm-0.7.4/komm/_sources.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     5469 2023-05-24 18:32:24.000000 komm-0.7.4/komm/_util.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-24 20:32:30.473378 komm-0.7.4/komm.egg-info/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1372 2023-05-24 20:32:30.000000 komm-0.7.4/komm.egg-info/PKG-INFO
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      791 2023-05-24 20:32:30.000000 komm-0.7.4/komm.egg-info/SOURCES.txt
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        1 2023-05-24 20:32:30.000000 komm-0.7.4/komm.egg-info/dependency_links.txt
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       12 2023-05-24 20:32:30.000000 komm-0.7.4/komm.egg-info/requires.txt
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        5 2023-05-24 20:32:30.000000 komm-0.7.4/komm.egg-info/top_level.txt
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       38 2023-05-24 20:32:30.483378 komm-0.7.4/setup.cfg
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1623 2023-05-24 20:31:35.000000 komm-0.7.4/setup.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-24 20:32:30.483378 komm-0.7.4/tests/
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     7141 2022-07-22 15:17:50.000000 komm-0.7.4/tests/test_algebra.py
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      509 2022-07-22 15:17:50.000000 komm-0.7.4/tests/test_channels.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    14875 2023-05-13 23:08:28.000000 komm-0.7.4/tests/test_error_control_block.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     8605 2023-05-13 23:08:28.000000 komm-0.7.4/tests/test_error_control_convolutional.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2661 2022-07-22 15:17:50.000000 komm-0.7.4/tests/test_finite_state_machine.py
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1860 2022-07-22 15:17:50.000000 komm-0.7.4/tests/test_modulation.py
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1802 2022-07-22 15:17:50.000000 komm-0.7.4/tests/test_quantization.py
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      976 2023-05-13 23:08:28.000000 komm-0.7.4/tests/test_sequences.py
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3028 2022-07-22 15:17:50.000000 komm-0.7.4/tests/test_source_coding.py
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      289 2023-05-13 23:08:28.000000 komm-0.7.4/tests/test_sources.py
+-rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      509 2022-07-22 15:17:50.000000 komm-0.7.4/tests/test_util.py
```

### Comparing `komm-0.7.3/LICENSE` & `komm-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `komm-0.7.3/PKG-INFO` & `komm-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: komm
-Version: 0.7.3
+Version: 0.7.4
 Summary: An open-source library for Python 3 providing tools for analysis and simulation of analog and digital communication systems.
 Home-page: https://github.com/rwnobrega/komm/
 Author: Roberto W. Nobrega
 Author-email: rwnobrega@gmail.com
 License: GPL
 Project-URL: Documentation, http://komm.readthedocs.io/
 Project-URL: Source, https://github.com/rwnobrega/komm/
```

### Comparing `komm-0.7.3/README.rst` & `komm-0.7.4/README.rst`

 * *Files identical despite different names*

### Comparing `komm-0.7.3/komm/__init__.py` & `komm-0.7.4/komm/__init__.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.3/komm/_algebra.py` & `komm-0.7.4/komm/_algebra.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.3/komm/_channels.py` & `komm-0.7.4/komm/_channels.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,31 +182,40 @@
             The mutual information :math:`\\mathrm{I}(X ; Y)` between the input :math:`X` and the output :math:`Y`.
 
         .. rubric:: Examples
 
         >>> dmc = komm.DiscreteMemorylessChannel([[0.6, 0.3, 0.1], [0.7, 0.1, 0.2], [0.5, 0.05, 0.45]])
         >>> dmc.mutual_information([1/3, 1/3, 1/3])
         0.12381109879798724
+        >>> dmc.mutual_information([1/3, 1/3, 1/3], base=3)
+        0.07811610605402552
         """
         return _mutual_information(input_pmf, self._transition_matrix, base)
 
 
-    def capacity(self):
+    def capacity(self, base=2.0):
         """
         Returns the channel capacity :math:`C`. It is given by :math:`C = \\max_{p_X} \\mathrm{I}(X;Y)`. This method computes the channel capacity via the Arimoto--Blahut algorithm. See :cite:`Cover.Thomas.06` (Sec. 10.8).
 
+        .. rubric:: Input
+
+        :code:`base` : :obj:`float` or :obj:`str`, optional
+            The base of the logarithm to be used. It must be a positive float or the string :code:`'e'`. The default value is :code:`2.0`.
+
         .. rubric:: Examples
 
         >>> dmc = komm.DiscreteMemorylessChannel([[0.6, 0.3, 0.1], [0.7, 0.1, 0.2], [0.5, 0.05, 0.45]])
         >>> dmc.capacity()
         0.1616318609548566
+        >>> dmc.capacity(base=3)
+        0.10197835020154389
         """
         initial_guess = np.ones(self._input_cardinality, dtype=float) / self._input_cardinality
         optimal_input_pmf = self._arimoto_blahut(self._transition_matrix, initial_guess, **self._arimoto_blahut_kwargs)
-        return _mutual_information(optimal_input_pmf, self._transition_matrix)
+        return _mutual_information(optimal_input_pmf, self._transition_matrix, base=base)
 
     def __call__(self, input_sequence):
         output_sequence = [np.random.choice(self._output_cardinality, p=self._transition_matrix[input_symbol])
                            for input_symbol in input_sequence]
         return np.array(output_sequence)
 
     def __repr__(self):
```

### Comparing `komm-0.7.3/komm/_error_control_block.py` & `komm-0.7.4/komm/_error_control_block.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.3/komm/_error_control_convolutional.py` & `komm-0.7.4/komm/_error_control_convolutional.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.3/komm/_finite_state_machine.py` & `komm-0.7.4/komm/_finite_state_machine.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.3/komm/_modulation.py` & `komm-0.7.4/komm/_modulation.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.3/komm/_pulses.py` & `komm-0.7.4/komm/_pulses.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.3/komm/_quantization.py` & `komm-0.7.4/komm/_quantization.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.3/komm/_sequences.py` & `komm-0.7.4/komm/_sequences.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.3/komm/_source_coding.py` & `komm-0.7.4/komm/_source_coding.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.3/komm/_sources.py` & `komm-0.7.4/komm/_sources.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,25 +43,32 @@
     @property
     def cardinality(self):
         """
         The cardinality :math:`|\\mathcal{X}|` of the source alphabet. This property is read-only.
         """
         return self._cardinality
 
-    def entropy(self):
+    def entropy(self, base=2.0):
         """
         Returns the source entropy :math:`\\mathrm{H}(X)`.
 
+        .. rubric:: Input
+
+        :code:`base` : :obj:`float` or :obj:`str`, optional
+            The base of the logarithm to be used. It must be a positive float or the string :code:`'e'`. The default value is :code:`2.0`.
+
         .. rubric:: Examples
 
         >>> dms = komm.DiscreteMemorylessSource([1/2, 1/4, 1/8, 1/8])
         >>> dms.entropy()
         1.75
+        >>> dms.entropy(base=4)
+        0.875
         """
-        return _entropy(self._pmf)
+        return _entropy(self._pmf, base=base)
 
     def __call__(self, size):
         return np.random.choice(self._cardinality, p=self._pmf, size=size)
 
     def __repr__(self):
         args = 'pmf={}'.format(self._pmf.tolist())
         return '{}({})'.format(self.__class__.__name__, args)
```

### Comparing `komm-0.7.3/komm/_util.py` & `komm-0.7.4/komm/_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,10 +183,11 @@
     if not np.allclose(np.sum(pmf), 1.0) or not np.alltrue(pmf >= 0.0):
         raise ValueError("Invalid pmf")
     return _entropy(pmf, base)
 
 
 def _mutual_information(input_pmf, transition_probabilities, base=2.0):
     output_pmf = np.dot(input_pmf, transition_probabilities)
-    entropy_output_prior = _entropy(output_pmf, base)
-    entropy_output_posterior = np.dot(input_pmf, np.apply_along_axis(_entropy, 1, transition_probabilities))
+    entropy_output_prior = _entropy(output_pmf, base=base)
+    entropy_base = lambda pmf: _entropy(pmf, base=base)
+    entropy_output_posterior = np.dot(input_pmf, np.apply_along_axis(entropy_base, 1, transition_probabilities))
     return entropy_output_prior - entropy_output_posterior
```

### Comparing `komm-0.7.3/komm.egg-info/PKG-INFO` & `komm-0.7.4/komm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: komm
-Version: 0.7.3
+Version: 0.7.4
 Summary: An open-source library for Python 3 providing tools for analysis and simulation of analog and digital communication systems.
 Home-page: https://github.com/rwnobrega/komm/
 Author: Roberto W. Nobrega
 Author-email: rwnobrega@gmail.com
 License: GPL
 Project-URL: Documentation, http://komm.readthedocs.io/
 Project-URL: Source, https://github.com/rwnobrega/komm/
```

### Comparing `komm-0.7.3/komm.egg-info/SOURCES.txt` & `komm-0.7.4/komm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `komm-0.7.3/setup.py` & `komm-0.7.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 For library reference, please check the project's `documentation page at Read the Docs <http://komm.readthedocs.io/>`_.
 
 This software is still under development. Contributions are very welcome!
 '''
 
 setup(
     name='komm',
-    version='0.7.3',
+    version='0.7.4',
     description='An open-source library for Python 3 providing tools for analysis and simulation of analog and digital communication systems.',
     long_description=_long_description,
     url='https://github.com/rwnobrega/komm/',
     author='Roberto W. Nobrega',
     author_email='rwnobrega@gmail.com',
     license='GPL',
     project_urls={
```

### Comparing `komm-0.7.3/tests/test_algebra.py` & `komm-0.7.4/tests/test_algebra.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.3/tests/test_error_control_block.py` & `komm-0.7.4/tests/test_error_control_block.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.3/tests/test_error_control_convolutional.py` & `komm-0.7.4/tests/test_error_control_convolutional.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.3/tests/test_finite_state_machine.py` & `komm-0.7.4/tests/test_finite_state_machine.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.3/tests/test_modulation.py` & `komm-0.7.4/tests/test_modulation.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.3/tests/test_quantization.py` & `komm-0.7.4/tests/test_quantization.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.3/tests/test_sequences.py` & `komm-0.7.4/tests/test_sequences.py`

 * *Files identical despite different names*

### Comparing `komm-0.7.3/tests/test_source_coding.py` & `komm-0.7.4/tests/test_source_coding.py`

 * *Files identical despite different names*

