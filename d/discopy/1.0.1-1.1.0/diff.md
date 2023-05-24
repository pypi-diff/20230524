# Comparing `tmp/discopy-1.0.1.tar.gz` & `tmp/discopy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discopy-1.0.1.tar", last modified: Wed May 24 07:57:59 2023, max compression
+gzip compressed data, was "discopy-1.1.0.tar", last modified: Wed May 24 09:01:49 2023, max compression
```

## Comparing `discopy-1.0.1.tar` & `discopy-1.1.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 07:57:59.847364 discopy-1.0.1/
--rw-r--r--   0 aleumi     (502) staff       (20)     1520 2023-04-18 08:36:50.000000 discopy-1.0.1/LICENSE
--rw-r--r--   0 aleumi     (502) staff       (20)     4976 2023-05-24 07:57:59.847661 discopy-1.0.1/PKG-INFO
--rw-r--r--   0 aleumi     (502) staff       (20)     4348 2023-04-18 08:36:50.000000 discopy-1.0.1/README.md
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 07:57:59.802680 discopy-1.0.1/discopy/
--rw-r--r--   0 aleumi     (502) staff       (20)      426 2023-05-23 16:36:04.000000 discopy-1.0.1/discopy/__init__.py
--rw-r--r--   0 aleumi     (502) staff       (20)     5758 2023-05-23 16:32:40.000000 discopy-1.0.1/discopy/balanced.py
--rw-r--r--   0 aleumi     (502) staff       (20)     8612 2023-05-23 16:31:12.000000 discopy-1.0.1/discopy/braided.py
--rw-r--r--   0 aleumi     (502) staff       (20)    28200 2023-05-23 16:32:41.000000 discopy-1.0.1/discopy/cat.py
--rw-r--r--   0 aleumi     (502) staff       (20)     8982 2023-05-23 16:24:44.000000 discopy-1.0.1/discopy/closed.py
--rw-r--r--   0 aleumi     (502) staff       (20)     8095 2023-05-23 16:33:01.000000 discopy-1.0.1/discopy/comonoid.py
--rw-r--r--   0 aleumi     (502) staff       (20)     4413 2023-05-23 16:32:40.000000 discopy-1.0.1/discopy/compact.py
--rw-r--r--   0 aleumi     (502) staff       (20)      236 2023-05-23 16:24:44.000000 discopy-1.0.1/discopy/config.py
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 07:57:59.813121 discopy-1.0.1/discopy/drawing/
--rw-r--r--   0 aleumi     (502) staff       (20)     1060 2023-05-23 16:32:40.000000 discopy-1.0.1/discopy/drawing/__init__.py
--rw-r--r--   0 aleumi     (502) staff       (20)    13920 2023-05-23 16:33:01.000000 discopy-1.0.1/discopy/drawing/grid.py
--rw-r--r--   0 aleumi     (502) staff       (20)    37886 2023-05-23 16:32:40.000000 discopy-1.0.1/discopy/drawing/legacy.py
--rw-r--r--   0 aleumi     (502) staff       (20)    11634 2023-05-23 16:32:40.000000 discopy-1.0.1/discopy/frobenius.py
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 07:57:59.827128 discopy-1.0.1/discopy/grammar/
--rw-r--r--   0 aleumi     (502) staff       (20)      225 2023-04-18 08:36:50.000000 discopy-1.0.1/discopy/grammar/__init__.py
--rw-r--r--   0 aleumi     (502) staff       (20)     9597 2023-05-23 16:24:44.000000 discopy-1.0.1/discopy/grammar/categorial.py
--rw-r--r--   0 aleumi     (502) staff       (20)     6890 2023-04-18 08:36:50.000000 discopy-1.0.1/discopy/grammar/cfg.py
--rw-r--r--   0 aleumi     (502) staff       (20)      926 2023-04-18 08:36:50.000000 discopy-1.0.1/discopy/grammar/dependency.py
--rw-r--r--   0 aleumi     (502) staff       (20)     5550 2023-05-23 16:32:21.000000 discopy-1.0.1/discopy/grammar/pregroup.py
--rw-r--r--   0 aleumi     (502) staff       (20)     2449 2023-04-18 08:36:50.000000 discopy-1.0.1/discopy/grammar/thue.py
--rw-r--r--   0 aleumi     (502) staff       (20)    48229 2023-05-23 16:33:01.000000 discopy-1.0.1/discopy/hypergraph.py
--rw-r--r--   0 aleumi     (502) staff       (20)    14082 2023-05-23 16:32:40.000000 discopy-1.0.1/discopy/interaction.py
--rw-r--r--   0 aleumi     (502) staff       (20)    14740 2023-05-23 16:32:41.000000 discopy-1.0.1/discopy/matrix.py
--rw-r--r--   0 aleumi     (502) staff       (20)     1617 2023-05-23 16:31:12.000000 discopy-1.0.1/discopy/messages.py
--rw-r--r--   0 aleumi     (502) staff       (20)    34458 2023-05-23 16:33:01.000000 discopy-1.0.1/discopy/monoidal.py
--rw-r--r--   0 aleumi     (502) staff       (20)     6871 2023-05-23 16:31:13.000000 discopy-1.0.1/discopy/pivotal.py
--rw-r--r--   0 aleumi     (502) staff       (20)     7845 2023-05-23 16:32:40.000000 discopy-1.0.1/discopy/python.py
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 07:57:59.845158 discopy-1.0.1/discopy/quantum/
--rw-r--r--   0 aleumi     (502) staff       (20)      667 2023-04-18 08:36:50.000000 discopy-1.0.1/discopy/quantum/__init__.py
--rw-r--r--   0 aleumi     (502) staff       (20)     5238 2023-04-18 08:36:50.000000 discopy-1.0.1/discopy/quantum/ansatze.py
--rw-r--r--   0 aleumi     (502) staff       (20)    11626 2023-04-18 08:36:50.000000 discopy-1.0.1/discopy/quantum/channel.py
--rw-r--r--   0 aleumi     (502) staff       (20)    33893 2023-05-24 07:55:57.000000 discopy-1.0.1/discopy/quantum/circuit.py
--rw-r--r--   0 aleumi     (502) staff       (20)    22165 2023-05-23 16:37:12.000000 discopy-1.0.1/discopy/quantum/gates.py
--rw-r--r--   0 aleumi     (502) staff       (20)    15738 2023-05-24 07:55:57.000000 discopy-1.0.1/discopy/quantum/pennylane.py
--rw-r--r--   0 aleumi     (502) staff       (20)    16429 2023-05-24 07:55:57.000000 discopy-1.0.1/discopy/quantum/tk.py
--rw-r--r--   0 aleumi     (502) staff       (20)    13451 2023-05-23 16:32:40.000000 discopy-1.0.1/discopy/quantum/zx.py
--rw-r--r--   0 aleumi     (502) staff       (20)     6916 2023-05-23 16:31:12.000000 discopy-1.0.1/discopy/ribbon.py
--rw-r--r--   0 aleumi     (502) staff       (20)    26017 2023-05-23 16:24:44.000000 discopy-1.0.1/discopy/rigid.py
--rw-r--r--   0 aleumi     (502) staff       (20)     9003 2023-05-23 16:33:01.000000 discopy-1.0.1/discopy/symmetric.py
--rw-r--r--   0 aleumi     (502) staff       (20)    23052 2023-05-23 16:33:01.000000 discopy-1.0.1/discopy/tensor.py
--rw-r--r--   0 aleumi     (502) staff       (20)     7593 2023-05-23 16:32:41.000000 discopy-1.0.1/discopy/traced.py
--rw-r--r--   0 aleumi     (502) staff       (20)    18153 2023-05-23 16:33:01.000000 discopy-1.0.1/discopy/utils.py
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 07:57:59.810721 discopy-1.0.1/discopy.egg-info/
--rw-r--r--   0 aleumi     (502) staff       (20)     4976 2023-05-24 07:57:59.000000 discopy-1.0.1/discopy.egg-info/PKG-INFO
--rw-r--r--   0 aleumi     (502) staff       (20)     1057 2023-05-24 07:57:59.000000 discopy-1.0.1/discopy.egg-info/SOURCES.txt
--rw-r--r--   0 aleumi     (502) staff       (20)        1 2023-05-24 07:57:59.000000 discopy-1.0.1/discopy.egg-info/dependency_links.txt
--rw-r--r--   0 aleumi     (502) staff       (20)      405 2023-05-24 07:57:59.000000 discopy-1.0.1/discopy.egg-info/requires.txt
--rw-r--r--   0 aleumi     (502) staff       (20)        8 2023-05-24 07:57:59.000000 discopy-1.0.1/discopy.egg-info/top_level.txt
--rw-r--r--   0 aleumi     (502) staff       (20)      208 2023-05-24 07:57:59.848829 discopy-1.0.1/setup.cfg
--rw-r--r--   0 aleumi     (502) staff       (20)     2163 2023-04-18 08:36:51.000000 discopy-1.0.1/setup.py
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:01:49.535480 discopy-1.1.0/
+-rw-r--r--   0 aleumi     (502) staff       (20)     1520 2023-04-18 08:36:50.000000 discopy-1.1.0/LICENSE
+-rw-r--r--   0 aleumi     (502) staff       (20)     5160 2023-05-24 09:01:49.535785 discopy-1.1.0/PKG-INFO
+-rw-r--r--   0 aleumi     (502) staff       (20)     4532 2023-05-24 08:20:40.000000 discopy-1.1.0/README.md
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:01:49.489088 discopy-1.1.0/discopy/
+-rw-r--r--   0 aleumi     (502) staff       (20)      424 2023-05-24 08:20:29.000000 discopy-1.1.0/discopy/__init__.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     5758 2023-05-23 16:32:40.000000 discopy-1.1.0/discopy/balanced.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     8612 2023-05-23 16:31:12.000000 discopy-1.1.0/discopy/braided.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    28200 2023-05-23 16:32:41.000000 discopy-1.1.0/discopy/cat.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     8982 2023-05-23 16:24:44.000000 discopy-1.1.0/discopy/closed.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     4413 2023-05-23 16:32:40.000000 discopy-1.1.0/discopy/compact.py
+-rw-r--r--   0 aleumi     (502) staff       (20)      236 2023-05-23 16:24:44.000000 discopy-1.1.0/discopy/config.py
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:01:49.499871 discopy-1.1.0/discopy/drawing/
+-rw-r--r--   0 aleumi     (502) staff       (20)     1060 2023-05-23 16:32:40.000000 discopy-1.1.0/discopy/drawing/__init__.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    13920 2023-05-23 16:33:01.000000 discopy-1.1.0/discopy/drawing/grid.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    37886 2023-05-23 16:32:40.000000 discopy-1.1.0/discopy/drawing/legacy.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    11613 2023-05-24 08:19:50.000000 discopy-1.1.0/discopy/frobenius.py
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:01:49.514610 discopy-1.1.0/discopy/grammar/
+-rw-r--r--   0 aleumi     (502) staff       (20)      225 2023-04-18 08:36:50.000000 discopy-1.1.0/discopy/grammar/__init__.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     9597 2023-05-23 16:24:44.000000 discopy-1.1.0/discopy/grammar/categorial.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     6890 2023-04-18 08:36:50.000000 discopy-1.1.0/discopy/grammar/cfg.py
+-rw-r--r--   0 aleumi     (502) staff       (20)      926 2023-04-18 08:36:50.000000 discopy-1.1.0/discopy/grammar/dependency.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     5550 2023-05-23 16:32:21.000000 discopy-1.1.0/discopy/grammar/pregroup.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     2410 2023-05-24 08:43:34.000000 discopy-1.1.0/discopy/grammar/thue.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    48229 2023-05-23 16:33:01.000000 discopy-1.1.0/discopy/hypergraph.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    14082 2023-05-23 16:32:40.000000 discopy-1.1.0/discopy/interaction.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     8057 2023-05-24 08:54:26.000000 discopy-1.1.0/discopy/markov.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    14740 2023-05-23 16:32:41.000000 discopy-1.1.0/discopy/matrix.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     1617 2023-05-23 16:31:12.000000 discopy-1.1.0/discopy/messages.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    34458 2023-05-23 16:33:01.000000 discopy-1.1.0/discopy/monoidal.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     6871 2023-05-23 16:31:13.000000 discopy-1.1.0/discopy/pivotal.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     7845 2023-05-23 16:32:40.000000 discopy-1.1.0/discopy/python.py
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:01:49.533141 discopy-1.1.0/discopy/quantum/
+-rw-r--r--   0 aleumi     (502) staff       (20)      667 2023-04-18 08:36:50.000000 discopy-1.1.0/discopy/quantum/__init__.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     5238 2023-04-18 08:36:50.000000 discopy-1.1.0/discopy/quantum/ansatze.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    11626 2023-04-18 08:36:50.000000 discopy-1.1.0/discopy/quantum/channel.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    33893 2023-05-24 07:55:57.000000 discopy-1.1.0/discopy/quantum/circuit.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    22165 2023-05-23 16:37:12.000000 discopy-1.1.0/discopy/quantum/gates.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    15738 2023-05-24 07:55:57.000000 discopy-1.1.0/discopy/quantum/pennylane.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    16429 2023-05-24 07:55:57.000000 discopy-1.1.0/discopy/quantum/tk.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    13451 2023-05-23 16:32:40.000000 discopy-1.1.0/discopy/quantum/zx.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     6916 2023-05-23 16:31:12.000000 discopy-1.1.0/discopy/ribbon.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    26017 2023-05-23 16:24:44.000000 discopy-1.1.0/discopy/rigid.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     9003 2023-05-23 16:33:01.000000 discopy-1.1.0/discopy/symmetric.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    23052 2023-05-23 16:33:01.000000 discopy-1.1.0/discopy/tensor.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     7593 2023-05-23 16:32:41.000000 discopy-1.1.0/discopy/traced.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    18153 2023-05-23 16:33:01.000000 discopy-1.1.0/discopy/utils.py
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:01:49.495721 discopy-1.1.0/discopy.egg-info/
+-rw-r--r--   0 aleumi     (502) staff       (20)     5160 2023-05-24 09:01:49.000000 discopy-1.1.0/discopy.egg-info/PKG-INFO
+-rw-r--r--   0 aleumi     (502) staff       (20)     1055 2023-05-24 09:01:49.000000 discopy-1.1.0/discopy.egg-info/SOURCES.txt
+-rw-r--r--   0 aleumi     (502) staff       (20)        1 2023-05-24 09:01:49.000000 discopy-1.1.0/discopy.egg-info/dependency_links.txt
+-rw-r--r--   0 aleumi     (502) staff       (20)      412 2023-05-24 09:01:49.000000 discopy-1.1.0/discopy.egg-info/requires.txt
+-rw-r--r--   0 aleumi     (502) staff       (20)        8 2023-05-24 09:01:49.000000 discopy-1.1.0/discopy.egg-info/top_level.txt
+-rw-r--r--   0 aleumi     (502) staff       (20)      208 2023-05-24 09:01:49.536976 discopy-1.1.0/setup.cfg
+-rw-r--r--   0 aleumi     (502) staff       (20)     2163 2023-04-18 08:36:51.000000 discopy-1.1.0/setup.py
```

### Comparing `discopy-1.0.1/LICENSE` & `discopy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/PKG-INFO` & `discopy-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: discopy
-Version: 1.0.1
+Version: 1.1.0
 Summary: The Python toolkit for computing with string diagrams.
 Home-page: https://discopy.org
-Download-URL: https://github.com/discopy/discopy/archive/1.0.1.tar.gz
+Download-URL: https://github.com/discopy/discopy/archive/1.1.0.tar.gz
 Author: Alexis Toumi
 Author-email: alexis@toumi.email
 Project-URL: Documentation, https://docs.discopy.org
 Project-URL: Source, https://github.com/discopy/discopy
 Project-URL: Tracker, https://github.com/discopy/discopy/issues
 Keywords: diagrams category-theory quantum-computing nlp
 Requires-Python: >=3.9
@@ -34,17 +34,18 @@
 * **Paper (for applied category theorists):** https://doi.org/10.4204/EPTCS.333.13
 * **Paper (for quantum computer scientists):** https://arxiv.org/abs/2205.05190
 
 DisCoPy began as an implementation of [DisCoCat](https://en.wikipedia.org/wiki/DisCoCat) and [QNLP](https://en.wikipedia.org/wiki/Quantum_natural_language_processing). This has now become its own library: [lambeq](https://cqcl.github.io/lambeq).
 
 ## Features
 
-* a data structure for arrows in free [dagger categories](https://en.wikipedia.org/wiki/Dagger_category) with formal sums, unary operators and symbolic variables from [SymPy](https://www.sympy.org/en/index.html)
-* data structures for string diagrams in any ([pre](https://ncatlab.org/nlab/show/premonoidal+category))[monoidal category](https://en.wikipedia.org/wiki/Monoidal_category) in the [hierarchy of graphical languages](https://en.wikipedia.org/wiki/String_diagram#Hierarchy_of_graphical_languages) (braids, twists, spiders, etc.)
-* methods for diagram composition, drawing, rewriting and evaluation as:
+* an `Arrow` data structure for free [dagger categories](https://en.wikipedia.org/wiki/Dagger_category) with formal sums, unary operators and symbolic variables from [SymPy](https://www.sympy.org/en/index.html)
+* a `Diagram` data structure for planar string diagrams in any ([pre](https://ncatlab.org/nlab/show/premonoidal+category))[monoidal category](https://en.wikipedia.org/wiki/Monoidal_category) in the [hierarchy of graphical languages](https://en.wikipedia.org/wiki/String_diagram#Hierarchy_of_graphical_languages) (with braids, twists, spiders, etc.)
+* a `Hypergraph` data structure for string diagrams in hypergraph categories and its restrictions to symmetric, traced, compact and Markov categories
+* methods for diagram composition, drawing, rewriting and `Functor` evaluation into:
   - Python code, i.e. wires as types and boxes as functions
   - [tensor networks](https://en.wikipedia.org/wiki/Tensor_network), i.e. wires as dimensions and boxes as arrays from [NumPy](https://numpy.org), [PyTorch](https://pytorch.org/), [TensorFlow](https://www.tensorflow.org/), [TensorNetwork](https://github.com/google/TensorNetwork) and [JAX](https://github.com/google/jax)
 * an implementation of [categorical quantum mechanics](https://en.wikipedia.org/wiki/Categorical_quantum_mechanics) interfacing with:
   - [tket](https://github.com/CQCL/tket) for circuit compilation
   - [PyZX](https://github.com/Quantomatic/pyzx) for optimisation with the [ZX calculus](https://zxcalculus.com/)
   - [PennyLane](https://pennylane.ai/) for automatic differentiation
 * an implementation of formal grammars ([context-free](https://en.wikipedia.org/wiki/Context-free_grammar), [categorial](https://en.wikipedia.org/wiki/Categorial_grammar), [pregroup](https://en.wikipedia.org/wiki/Pregroup_grammar) or [dependency](https://en.wikipedia.org/wiki/Dependency_grammar)) with interfaces to [lambeq](https://cqcl.github.io/lambeq), [spaCy](https://spacy.io/) and [NLTK](https://www.nltk.org/)
```

### Comparing `discopy-1.0.1/README.md` & `discopy-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 * **Paper (for applied category theorists):** https://doi.org/10.4204/EPTCS.333.13
 * **Paper (for quantum computer scientists):** https://arxiv.org/abs/2205.05190
 
 DisCoPy began as an implementation of [DisCoCat](https://en.wikipedia.org/wiki/DisCoCat) and [QNLP](https://en.wikipedia.org/wiki/Quantum_natural_language_processing). This has now become its own library: [lambeq](https://cqcl.github.io/lambeq).
 
 ## Features
 
-* a data structure for arrows in free [dagger categories](https://en.wikipedia.org/wiki/Dagger_category) with formal sums, unary operators and symbolic variables from [SymPy](https://www.sympy.org/en/index.html)
-* data structures for string diagrams in any ([pre](https://ncatlab.org/nlab/show/premonoidal+category))[monoidal category](https://en.wikipedia.org/wiki/Monoidal_category) in the [hierarchy of graphical languages](https://en.wikipedia.org/wiki/String_diagram#Hierarchy_of_graphical_languages) (braids, twists, spiders, etc.)
-* methods for diagram composition, drawing, rewriting and evaluation as:
+* an `Arrow` data structure for free [dagger categories](https://en.wikipedia.org/wiki/Dagger_category) with formal sums, unary operators and symbolic variables from [SymPy](https://www.sympy.org/en/index.html)
+* a `Diagram` data structure for planar string diagrams in any ([pre](https://ncatlab.org/nlab/show/premonoidal+category))[monoidal category](https://en.wikipedia.org/wiki/Monoidal_category) in the [hierarchy of graphical languages](https://en.wikipedia.org/wiki/String_diagram#Hierarchy_of_graphical_languages) (with braids, twists, spiders, etc.)
+* a `Hypergraph` data structure for string diagrams in hypergraph categories and its restrictions to symmetric, traced, compact and Markov categories
+* methods for diagram composition, drawing, rewriting and `Functor` evaluation into:
   - Python code, i.e. wires as types and boxes as functions
   - [tensor networks](https://en.wikipedia.org/wiki/Tensor_network), i.e. wires as dimensions and boxes as arrays from [NumPy](https://numpy.org), [PyTorch](https://pytorch.org/), [TensorFlow](https://www.tensorflow.org/), [TensorNetwork](https://github.com/google/TensorNetwork) and [JAX](https://github.com/google/jax)
 * an implementation of [categorical quantum mechanics](https://en.wikipedia.org/wiki/Categorical_quantum_mechanics) interfacing with:
   - [tket](https://github.com/CQCL/tket) for circuit compilation
   - [PyZX](https://github.com/Quantomatic/pyzx) for optimisation with the [ZX calculus](https://zxcalculus.com/)
   - [PennyLane](https://pennylane.ai/) for automatic differentiation
 * an implementation of formal grammars ([context-free](https://en.wikipedia.org/wiki/Context-free_grammar), [categorial](https://en.wikipedia.org/wiki/Categorial_grammar), [pregroup](https://en.wikipedia.org/wiki/Pregroup_grammar) or [dependency](https://en.wikipedia.org/wiki/Dependency_grammar)) with interfaces to [lambeq](https://cqcl.github.io/lambeq), [spaCy](https://spacy.io/) and [NLTK](https://www.nltk.org/)
```

### Comparing `discopy-1.0.1/discopy/balanced.py` & `discopy-1.1.0/discopy/balanced.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/braided.py` & `discopy-1.1.0/discopy/braided.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/cat.py` & `discopy-1.1.0/discopy/cat.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/closed.py` & `discopy-1.1.0/discopy/closed.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/comonoid.py` & `discopy-1.1.0/discopy/markov.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 """
-The free symmetric category with a supply of (co)commutative (co)monoid,
-also called copy-discard category, see :cite:t:`FritzLiang23`.
+The free Markov category, i.e. the free semicartesian category with a supply of
+commutative comonoid, see :cite:t:`FritzLiang23`.
 
 Summary
 -------
 
 .. autosummary::
     :template: class.rst
     :nosignatures:
@@ -60,39 +60,39 @@
 ...     == copy @ copy >> x @ Swap(x, x) @ x
 >>> assert Diagram.merge(x @ x, n=0) == unit @ unit
 >>> assert Diagram.merge(x @ x)\\
 ...     == x @ Swap(x, x) @ x >> merge @ merge
 
 Note
 ----
-Equality of comonoid diagrams is computed by translation to hypergraph.
+Equality of Markov diagrams is computed by translation to hypergraph.
 Both copy and merge boxes are translated to spiders, thus when they appear
 in the same diagram they automatically satisfy the :mod:`frobenius` axioms.
 """
 
 from __future__ import annotations
 
 from discopy import symmetric, monoidal, hypergraph
 from discopy.cat import factory
 from discopy.monoidal import Ty, assert_isatomic
 
 
 @factory
 class Diagram(symmetric.Diagram):
     """
-    A comonoid diagram is a symmetric diagram with :class:`Copy` boxes.
+    A Markov diagram is a symmetric diagram with :class:`Copy` boxes.
 
     Parameters:
         inside(Layer) : The layers inside the diagram.
         dom (monoidal.Ty) : The domain of the diagram, i.e. its input.
         cod (monoidal.Ty) : The codomain of the diagram, i.e. its output.
 
     Note
     ----
-    We can create arbitrary comonoid diagrams with the standard notation for
+    We can create arbitrary Markov diagrams with the standard notation for
     Python functions.
 
     >>> x = Ty('x')
     >>> f = Box('f', x, x)
 
     >>> copy_then_apply = Diagram.from_callable(x, x @ x)(
     ...     lambda x: (f(x), f(x)))
@@ -100,17 +100,17 @@
     >>> @Diagram.from_callable(x, x @ x)
     ... def apply_then_copy(x):
     ...     y = f(x)
     ...     return x, x
 
     >>> from discopy.drawing import Equation
     >>> Equation(copy_then_apply, apply_then_copy, symbol="$\\\\neq$").draw(
-    ...     path="docs/_static/comonoid/copy_and_apply.png")
+    ...     path="docs/_static/markov/copy_and_apply.png")
 
-    .. image:: /_static/comonoid/copy_and_apply.png
+    .. image:: /_static/markov/copy_and_apply.png
     """
     @classmethod
     def spider_factory(cls, n_legs_in, n_legs_out, typ, phase=None):
         if phase is not None or 1 not in (n_legs_in, n_legs_out):
             raise ValueError
         return cls.copy_factory(typ, n_legs_out) if n_legs_in == 1\
             else cls.merge_factory(typ, n_legs_in)
@@ -137,38 +137,38 @@
             n : The number of copies.
         """
         return cls.copy(x, n).dagger()
 
 
 class Box(symmetric.Box, Diagram):
     """
-    A comonoid box is a symmetric box in a comonoid diagram.
+    A Markov box is a symmetric box in a Markov diagram.
 
     Parameters:
         name (str) : The name of the box.
         dom (monoidal.Ty) : The domain of the box, i.e. its input.
         cod (monoidal.Ty) : The codomain of the box, i.e. its output.
     """
     __ambiguous_inheritance__ = (symmetric.Box, )
 
 
 class Swap(symmetric.Swap, Box):
     """
-    Symmetric swap in a comonoid diagram.
+    Symmetric swap in a Markov diagram.
 
     Parameters:
         left (monoidal.Ty) : The type on the top left and bottom right.
         right (monoidal.Ty) : The type on the top right and bottom left.
     """
     __ambiguous_inheritance__ = (symmetric.Swap, )
 
 
 class Trace(symmetric.Trace, Box):
     """
-    A trace in a category with comonoids.
+    A trace in a Markov category.
 
     Parameters:
         arg : The diagram to trace.
         left : Whether to trace the wires on the left or right.
 
     See also
     --------
@@ -209,26 +209,26 @@
 
     def dagger(self) -> Merge:
         return Copy(self.cod, len(self.dom))
 
 
 class Category(symmetric.Category):
     """
-    A comonoid category is a symmetric category with a method :code:`copy`.
+    A Markov category is a symmetric category with a method :code:`copy`.
 
     Parameters:
         ob : The type of objects.
         ar : The type of arrows.
     """
     ob, ar = Ty, Diagram
 
 
 class Functor(symmetric.Functor):
     """
-    A comonoid functor is a symmetric functor that preserves copies.
+    A Markov functor is a symmetric functor that preserves copies.
 
     Parameters:
         ob (Mapping[monoidal.Ty, monoidal.Ty]) :
             Map from :class:`monoidal.Ty` to :code:`cod.ob`.
         ar (Mapping[Box, Diagram]) : Map from :class:`Box` to :code:`cod.ar`.
         cod (Category) :
             The codomain, :code:`Category(Ty, Diagram)` by default.
@@ -246,17 +246,17 @@
     >>> copy = Copy(x)
     >>> bialgebra_l = copy @ copy >> Id(x) @ Swap(x, x) @ Id(x) >> add @ add
     >>> bialgebra_r = add >> copy
     >>> assert F(bialgebra_l)(54, 46) == F(bialgebra_r)(54, 46)
 
     >>> from discopy.drawing import Equation
     >>> Equation(bialgebra_l, bialgebra_r, symbol="=").draw(
-    ...     path="docs/_static/comonoid/bialgebra.png")
+    ...     path="docs/_static/markov/bialgebra.png")
 
-    .. image:: /_static/comonoid/bialgebra.png
+    .. image:: /_static/markov/bialgebra.png
     """
     dom = cod = Category(Ty, Diagram)
 
     def __call__(self, other):
         if isinstance(other, Copy):
             return self.cod.ar.copy(self(other.dom), len(other.cod))
         if isinstance(other, Merge):
```

### Comparing `discopy-1.0.1/discopy/compact.py` & `discopy-1.1.0/discopy/compact.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/drawing/__init__.py` & `discopy-1.1.0/discopy/drawing/__init__.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/drawing/grid.py` & `discopy-1.1.0/discopy/drawing/grid.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/drawing/legacy.py` & `discopy-1.1.0/discopy/drawing/legacy.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/frobenius.py` & `discopy-1.1.0/discopy/frobenius.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     :align: center
 """
 
 from __future__ import annotations
 
 from collections.abc import Callable
 
-from discopy import comonoid, compact, pivotal, hypergraph
+from discopy import markov, compact, pivotal, hypergraph
 from discopy.cat import factory
 from discopy.monoidal import assert_isatomic
 from discopy.utils import factory_name, assert_isinstance
 
 
 class Ob(pivotal.Ob):
     """
@@ -111,24 +111,24 @@
         return f"Dim({', '.join(map(repr, self.inside)) or '1'})"
 
     __str__ = __repr__
     l = r = property(lambda self: self.factory(*self.inside[::-1]))
 
 
 @factory
-class Diagram(compact.Diagram, comonoid.Diagram):
+class Diagram(compact.Diagram, markov.Diagram):
     """
-    A frobenius diagram is a compact diagram and a comonoid diagram.
+    A frobenius diagram is a compact diagram and a Markov diagram.
 
     Parameters:
         inside(Layer) : The layers of the diagram.
         dom (Ty) : The domain of the diagram, i.e. its input.
         cod (Ty) : The codomain of the diagram, i.e. its output.
     """
-    __ambiguous_inheritance__ = (compact.Diagram, comonoid.Diagram)
+    __ambiguous_inheritance__ = (compact.Diagram, markov.Diagram)
 
     ty_factory = Ty
 
     @classmethod
     def caps(cls, left, right):
         return cls.cups(left, right).dagger()
 
@@ -170,24 +170,24 @@
         F = compact.Functor(
             ob=lambda x: x, ar=lambda f:
                 f.unfuse() if isinstance(f, Spider) else f,
             dom=Category(), cod=Category())
         return F(self)
 
 
-class Box(compact.Box, comonoid.Box, Diagram):
+class Box(compact.Box, markov.Box, Diagram):
     """
-    A frobenius box is a compact and comonoid box in a frobenius diagram.
+    A frobenius box is a compact and Markov box in a frobenius diagram.
 
     Parameters:
         name (str) : The name of the box.
         dom (Ty) : The domain of the box, i.e. its input.
         cod (Ty) : The codomain of the box, i.e. its output.
     """
-    __ambiguous_inheritance__ = (compact.Box, comonoid.Box)
+    __ambiguous_inheritance__ = (compact.Box, markov.Box)
 
 
 class Cup(compact.Cup, Box):
     """
     A frobenius cup is a compact cup in a frobenius diagram.
 
     Parameters:
@@ -204,23 +204,23 @@
     Parameters:
         left (Ty) : The atomic type.
         right (Ty) : Its adjoint.
     """
     __ambiguous_inheritance__ = (compact.Cap, )
 
 
-class Swap(compact.Swap, comonoid.Swap, Box):
+class Swap(compact.Swap, markov.Swap, Box):
     """
-    A frobenius swap is a compact swap in a frobenius diagram.
+    A frobenius swap is a compact and Markov swap in a frobenius diagram.
 
     Parameters:
         left (Ty) : The type on the top left and bottom right.
         right (Ty) : The type on the top right and bottom left.
     """
-    __ambiguous_inheritance__ = (compact.Swap, comonoid.Swap)
+    __ambiguous_inheritance__ = (compact.Swap, markov.Swap)
 
 
 class Spider(Box):
     """
     The spider with :code:`n_legs_in` and :code:`n_legs_out`
     on a given atomic type, with some optional phase as ``data``.
 
@@ -270,48 +270,48 @@
         return type(self)(len(self.cod), len(self.dom), self.typ, self.phase)
 
     def unfuse(self) -> Diagram:
         return coherence(self.factory, type(self))(
             len(self.dom), len(self.cod), self.typ, self.phase)
 
 
-class Category(compact.Category, comonoid.Category):
+class Category(compact.Category, markov.Category):
     """
     A hypergraph category is a compact category with a method :code:`spiders`.
 
     Parameters:
         ob : The objects of the category, default is :class:`Ty`.
         ar : The arrows of the category, default is :class:`Diagram`.
     """
-    __ambiguous_inheritance__ = (compact.Category, comonoid.Category)
+    __ambiguous_inheritance__ = (compact.Category, markov.Category)
 
     ob, ar = Ty, Diagram
 
 
-class Functor(compact.Functor, comonoid.Functor):
+class Functor(compact.Functor, markov.Functor):
     """
     A hypergraph functor is a compact functor that preserves spiders.
 
     Parameters:
         ob (Mapping[Ty, Ty]) : Map from atomic :class:`Ty` to :code:`cod.ob`.
         ar (Mapping[Box, Diagram]) : Map from :class:`Box` to :code:`cod.ar`.
         cod (Category) : The codomain of the functor.
     """
-    __ambiguous_inheritance__ = (compact.Functor, comonoid.Functor)
+    __ambiguous_inheritance__ = (compact.Functor, markov.Functor)
 
     dom = cod = Category()
 
     def __call__(self, other):
         if isinstance(other, Dim):
             return sum([self.ob[x] for x in other], self.cod.ob())
         if isinstance(other, Spider):
             return self.cod.ar.spiders(
                 len(other.dom), len(other.cod), self(other.typ))
-        if isinstance(other, (comonoid.Copy, comonoid.Merge)):
-            return comonoid.Functor.__call__(self, other)
+        if isinstance(other, (markov.Copy, markov.Merge)):
+            return markov.Functor.__call__(self, other)
         return compact.Functor.__call__(self, other)
 
 
 def interleaving(cls: type, factory: Callable
                  ) -> Callable[[int, int, Ty], Diagram]:
     """
     Take a ``factory`` for spiders of atomic types and extend it recursively.
```

### Comparing `discopy-1.0.1/discopy/grammar/categorial.py` & `discopy-1.1.0/discopy/grammar/categorial.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/grammar/cfg.py` & `discopy-1.1.0/discopy/grammar/cfg.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/grammar/dependency.py` & `discopy-1.1.0/discopy/grammar/dependency.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/grammar/pregroup.py` & `discopy-1.1.0/discopy/grammar/pregroup.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/grammar/thue.py` & `discopy-1.1.0/discopy/grammar/thue.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 A formal grammar is a free monoidal category with words and rules as boxes.
 
 Formal grammars are also known as string rewriting or semi-Thue systems, they
-were introduced by Thue :cite:`Thue14`, see :cite:`Power13` for a translation.
+were introduced by Thue :cite:`Thue14`.
 
 The parsing problem is to decide, given two strings, whether there exists a
 diagram from one to the other. It has been shown to be undecidable by Post
 :cite:`Post47` and Markov :cite:`Markov47`.
 
 Summary
 -------
```

### Comparing `discopy-1.0.1/discopy/hypergraph.py` & `discopy-1.1.0/discopy/hypergraph.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/interaction.py` & `discopy-1.1.0/discopy/interaction.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/matrix.py` & `discopy-1.1.0/discopy/matrix.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/messages.py` & `discopy-1.1.0/discopy/messages.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/monoidal.py` & `discopy-1.1.0/discopy/monoidal.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/pivotal.py` & `discopy-1.1.0/discopy/pivotal.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/python.py` & `discopy-1.1.0/discopy/python.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/quantum/__init__.py` & `discopy-1.1.0/discopy/quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/quantum/ansatze.py` & `discopy-1.1.0/discopy/quantum/ansatze.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/quantum/channel.py` & `discopy-1.1.0/discopy/quantum/channel.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/quantum/circuit.py` & `discopy-1.1.0/discopy/quantum/circuit.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/quantum/gates.py` & `discopy-1.1.0/discopy/quantum/gates.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/quantum/pennylane.py` & `discopy-1.1.0/discopy/quantum/pennylane.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/quantum/tk.py` & `discopy-1.1.0/discopy/quantum/tk.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/quantum/zx.py` & `discopy-1.1.0/discopy/quantum/zx.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/ribbon.py` & `discopy-1.1.0/discopy/ribbon.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/rigid.py` & `discopy-1.1.0/discopy/rigid.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/symmetric.py` & `discopy-1.1.0/discopy/symmetric.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/tensor.py` & `discopy-1.1.0/discopy/tensor.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/traced.py` & `discopy-1.1.0/discopy/traced.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy/utils.py` & `discopy-1.1.0/discopy/utils.py`

 * *Files identical despite different names*

### Comparing `discopy-1.0.1/discopy.egg-info/PKG-INFO` & `discopy-1.1.0/discopy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: discopy
-Version: 1.0.1
+Version: 1.1.0
 Summary: The Python toolkit for computing with string diagrams.
 Home-page: https://discopy.org
-Download-URL: https://github.com/discopy/discopy/archive/1.0.1.tar.gz
+Download-URL: https://github.com/discopy/discopy/archive/1.1.0.tar.gz
 Author: Alexis Toumi
 Author-email: alexis@toumi.email
 Project-URL: Documentation, https://docs.discopy.org
 Project-URL: Source, https://github.com/discopy/discopy
 Project-URL: Tracker, https://github.com/discopy/discopy/issues
 Keywords: diagrams category-theory quantum-computing nlp
 Requires-Python: >=3.9
@@ -34,17 +34,18 @@
 * **Paper (for applied category theorists):** https://doi.org/10.4204/EPTCS.333.13
 * **Paper (for quantum computer scientists):** https://arxiv.org/abs/2205.05190
 
 DisCoPy began as an implementation of [DisCoCat](https://en.wikipedia.org/wiki/DisCoCat) and [QNLP](https://en.wikipedia.org/wiki/Quantum_natural_language_processing). This has now become its own library: [lambeq](https://cqcl.github.io/lambeq).
 
 ## Features
 
-* a data structure for arrows in free [dagger categories](https://en.wikipedia.org/wiki/Dagger_category) with formal sums, unary operators and symbolic variables from [SymPy](https://www.sympy.org/en/index.html)
-* data structures for string diagrams in any ([pre](https://ncatlab.org/nlab/show/premonoidal+category))[monoidal category](https://en.wikipedia.org/wiki/Monoidal_category) in the [hierarchy of graphical languages](https://en.wikipedia.org/wiki/String_diagram#Hierarchy_of_graphical_languages) (braids, twists, spiders, etc.)
-* methods for diagram composition, drawing, rewriting and evaluation as:
+* an `Arrow` data structure for free [dagger categories](https://en.wikipedia.org/wiki/Dagger_category) with formal sums, unary operators and symbolic variables from [SymPy](https://www.sympy.org/en/index.html)
+* a `Diagram` data structure for planar string diagrams in any ([pre](https://ncatlab.org/nlab/show/premonoidal+category))[monoidal category](https://en.wikipedia.org/wiki/Monoidal_category) in the [hierarchy of graphical languages](https://en.wikipedia.org/wiki/String_diagram#Hierarchy_of_graphical_languages) (with braids, twists, spiders, etc.)
+* a `Hypergraph` data structure for string diagrams in hypergraph categories and its restrictions to symmetric, traced, compact and Markov categories
+* methods for diagram composition, drawing, rewriting and `Functor` evaluation into:
   - Python code, i.e. wires as types and boxes as functions
   - [tensor networks](https://en.wikipedia.org/wiki/Tensor_network), i.e. wires as dimensions and boxes as arrays from [NumPy](https://numpy.org), [PyTorch](https://pytorch.org/), [TensorFlow](https://www.tensorflow.org/), [TensorNetwork](https://github.com/google/TensorNetwork) and [JAX](https://github.com/google/jax)
 * an implementation of [categorical quantum mechanics](https://en.wikipedia.org/wiki/Categorical_quantum_mechanics) interfacing with:
   - [tket](https://github.com/CQCL/tket) for circuit compilation
   - [PyZX](https://github.com/Quantomatic/pyzx) for optimisation with the [ZX calculus](https://zxcalculus.com/)
   - [PennyLane](https://pennylane.ai/) for automatic differentiation
 * an implementation of formal grammars ([context-free](https://en.wikipedia.org/wiki/Context-free_grammar), [categorial](https://en.wikipedia.org/wiki/Categorial_grammar), [pregroup](https://en.wikipedia.org/wiki/Pregroup_grammar) or [dependency](https://en.wikipedia.org/wiki/Dependency_grammar)) with interfaces to [lambeq](https://cqcl.github.io/lambeq), [spaCy](https://spacy.io/) and [NLTK](https://www.nltk.org/)
```

### Comparing `discopy-1.0.1/discopy.egg-info/SOURCES.txt` & `discopy-1.1.0/discopy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 setup.cfg
 setup.py
 discopy/__init__.py
 discopy/balanced.py
 discopy/braided.py
 discopy/cat.py
 discopy/closed.py
-discopy/comonoid.py
 discopy/compact.py
 discopy/config.py
 discopy/frobenius.py
 discopy/hypergraph.py
 discopy/interaction.py
+discopy/markov.py
 discopy/matrix.py
 discopy/messages.py
 discopy/monoidal.py
 discopy/pivotal.py
 discopy/python.py
 discopy/ribbon.py
 discopy/rigid.py
```

### Comparing `discopy-1.0.1/setup.py` & `discopy-1.1.0/setup.py`

 * *Files identical despite different names*

