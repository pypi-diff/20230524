# Comparing `tmp/yarrow_diagrams-0.0.2.tar.gz` & `tmp/yarrow_diagrams-0.0.2.1.tar.gz`

## Comparing `yarrow_diagrams-0.0.2.tar` & `yarrow_diagrams-0.0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/__init__.py
--rw-r--r--   0        0        0     8173 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/bipartite_multigraph.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/cupy.py
--rw-r--r--   0        0        0    11961 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/diagram.py
--rw-r--r--   0        0        0    12537 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/finite_function.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/array/__init__.py
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/array/cupy.py
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/array/numpy.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/decompose/frobenius.py
--rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/functor/functor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/segmented/__init__.py
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/segmented/finite_function.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/yarrow/segmented/operations.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/LICENSE
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/README.md
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/__init__.py
+-rw-r--r--   0        0        0     8194 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/bipartite_multigraph.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/cupy.py
+-rw-r--r--   0        0        0    12065 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/diagram.py
+-rw-r--r--   0        0        0    12758 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/finite_function.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/array/__init__.py
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/array/cupy.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/array/numpy.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/decompose/frobenius.py
+-rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/functor/functor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/segmented/__init__.py
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/segmented/finite_function.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/segmented/operations.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/LICENSE
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/README.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/PKG-INFO
```

### Comparing `yarrow_diagrams-0.0.2/yarrow/bipartite_multigraph.py` & `yarrow_diagrams-0.0.2.1/yarrow/bipartite_multigraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,15 +233,15 @@
     """
     Given a coequalizer q : B → Q of morphisms a, b : A → B
     and some f : B → B' such that f(a) = f(b),
     Compute the universal map u : Q → B'
     such that q ; u = f.
     """
     target = f.target
-    u = q._Array.zeros(q.target)
+    u = q._Array.zeros(q.target, dtype=f.table.dtype)
     # TODO: in the below we assume the PRAM CRCW model: multiple writes to the
     # same memory location in the 'u' array can happen in parallel, with an
     # arbitrary write succeeding.
     # Note that this doesn't affect correctness because q and f are co-forks,
     # and q is a coequalizer.
     # However, this won't perform well on e.g., GPU hardware. FIXME!
     u[q.table] = f.table
```

### Comparing `yarrow_diagrams-0.0.2/yarrow/cupy.py` & `yarrow_diagrams-0.0.2.1/yarrow/cupy.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.2/yarrow/diagram.py` & `yarrow_diagrams-0.0.2.1/yarrow/diagram.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,15 @@
             x: A single operation represented as an AbstractFiniteFunction of type `1 → Σ₁`
             a: The input type of `x` as a finite function `A → Σ₀`
             b: The output type of `x` as a finite function `B → Σ₀`
 
         Returns:
             AbstractDiagram: a diagram with a single generating operation.
         """
+        Array = cls._Fun._Array
         F = cls._Fun
         assert F == type(a)
         assert F == type(b)
         assert F == type(xn)
 
         # x : 1 → Σ₁
         assert xn.source == 1
@@ -237,17 +238,18 @@
             # xi : A → 1         xo : B → 1
             xi = F.terminal(a.source),
             xo = F.terminal(b.source),
 
             # wn : A + B → Σ₀
             wn = a + b,
 
-            # pi : A → Nat       po : B → Nat
-            pi = F.identity(a.source),
-            po = F.identity(b.source),
+            # pi' : A → Nat       po' : B → Nat
+            # pi = pi';ι          po  = po';ι
+            pi = F(None, Array.arange(a.source)),
+            po = F(None, Array.arange(b.source)),
 
             xn = xn,
         )
 
         # Note: s=inj0, t=inj1, so we just reuse wi and wo.
         return cls(s=wi, t=wo, G=G)
```

### Comparing `yarrow_diagrams-0.0.2/yarrow/finite_function.py` & `yarrow_diagrams-0.0.2.1/yarrow/finite_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,24 +44,30 @@
 class AbstractFiniteFunction:
     """
     Finite functions parametrised over the underlying array type (the "backend").
     This implementation assumes there is a cls._Array member implementing various primitives.
     For example, cls._Array.sum() should compute the sum of an array.
     """
     def __init__(self, target, table, dtype=DTYPE):
+        # TODO: this constructor is too complicated; it should be simplified.
         # _Array is the "array functions module"
         # It lets us parametrise AbstractFiniteFunction by a module like "numpy".
-        self.table = type(self)._Array.array(table, dtype=dtype)
+        Array = type(self)._Array
+        if type(table) == Array.Type:
+           self.table = table
+        else:
+            self.table = Array.array(table, dtype=dtype)
+
         self.target = target
 
         assert len(self.table.shape) == 1 # ensure 1D array
         assert self.source >= 0
         if self.source > 0 and self.target is not None:
             assert self.target >= 0
-            assert self.target > type(self)._Array.max(table)
+            assert self.target > Array.max(table)
 
     @property
     def source(self):
         """The source (aka "domain") of this finite function"""
         return len(self.table)
 
     def __len__(self):
@@ -176,14 +182,15 @@
         """
         return type(f)(a + f.target, a + f.table)
 
     def coproduct(f, g):
         """ Given maps ``f : A₀ → B`` and ``g : A₁ → B``
         compute the coproduct ``f.coproduct(g) : A₀ + A₁ → B``"""
         assert f.target == g.target
+        assert f.table.dtype == g.table.dtype
         target = f.target
         table = type(f)._Array.concatenate([f.table, g.table])
         return type(f)(target, table)
 
     def __add__(f, g):
         """ Inline coproduct """
         return f.coproduct(g)
```

### Comparing `yarrow_diagrams-0.0.2/yarrow/array/__init__.py` & `yarrow_diagrams-0.0.2.1/yarrow/array/__init__.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.2/yarrow/array/cupy.py` & `yarrow_diagrams-0.0.2.1/yarrow/array/cupy.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 """
 import cupy as cp
 import cupyx.scipy.sparse as sparse
 from cupyx.scipy.sparse import csgraph
 
 DEFAULT_DTYPE='int64'
 
+Type = cp.ndarray
+
 def array(*args, **kwargs):
     return cp.array(*args, **kwargs)
 
 def max(*args, **kwargs):
     return cp.max(*args, **kwargs)
 
 def arange(*args, **kwargs):
```

### Comparing `yarrow_diagrams-0.0.2/yarrow/array/numpy.py` & `yarrow_diagrams-0.0.2.1/yarrow/array/numpy.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,30 +9,41 @@
 It's used by :py:class:`FiniteFunction`.
 """
 import numpy as np
 import scipy.sparse as sparse
 
 DEFAULT_DTYPE='int64'
 
+Type = np.ndarray
+""" The underlying array type used by functions in the backend. For numpy this is ``np.ndarray``.
+
+   :meta hide-value:
+"""
+# NOTE: we use :meta hide-value: above because numpy is mocked, so sphinx will
+# have the incorrect value in documentation.
+
 def array(*args, **kwargs):
+    kwargs.setdefault('dtype', DEFAULT_DTYPE)
     return np.array(*args, **kwargs)
 
 def max(*args, **kwargs):
     return np.max(*args, **kwargs)
 
 def arange(*args, **kwargs):
     return np.arange(*args, **kwargs)
 
 def all(*args, **kwargs):
     return np.all(*args, **kwargs)
 
 def zeros(*args, **kwargs):
+    kwargs.setdefault('dtype', DEFAULT_DTYPE)
     return np.zeros(*args, **kwargs)
 
 def ones(*args, **kwargs):
+    kwargs.setdefault('dtype', DEFAULT_DTYPE)
     return np.ones(*args, **kwargs)
 
 def cumsum(*args, **kwargs):
     return np.cumsum(*args, **kwargs)
 
 def sum(*args, **kwargs):
     return np.sum(*args, **kwargs)
@@ -108,22 +119,23 @@
         x: An array of the sizes of each "segment" of the output
 
     Returns:
         array:
 
         segmented array with segment ``i`` equal to ``arange(i)``.
     """
-    x = np.array(x)
+    x = np.array(x, dtype=DEFAULT_DTYPE)
 
     # create segment pointer array
     ptr = np.zeros(len(x) + 1, dtype=x.dtype) # O(1) PRAM
     ptr[1:] = np.cumsum(x)                    # O(log x) PRAM
     N = ptr[-1] # total size
 
     r = np.repeat(ptr[:-1], x) # O(log x) PRAM
     return np.arange(0, N) - r # O(1)     PRAM
 
 def bincount(x, *args, **kwargs):
     return np.bincount(x, *args, **kwargs)
 
 def full(n, x, *args, **kwargs):
+    kwargs.setdefault('dtype', DEFAULT_DTYPE)
     return np.full(n, x, *args, **kwargs)
```

### Comparing `yarrow_diagrams-0.0.2/yarrow/decompose/frobenius.py` & `yarrow_diagrams-0.0.2.1/yarrow/decompose/frobenius.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.2/yarrow/functor/functor.py` & `yarrow_diagrams-0.0.2.1/yarrow/functor/functor.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.2/yarrow/segmented/finite_function.py` & `yarrow_diagrams-0.0.2.1/yarrow/segmented/finite_function.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.2/yarrow/segmented/operations.py` & `yarrow_diagrams-0.0.2.1/yarrow/segmented/operations.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.2/LICENSE` & `yarrow_diagrams-0.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.2/README.md` & `yarrow_diagrams-0.0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.2/pyproject.toml` & `yarrow_diagrams-0.0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "yarrow-diagrams"
-version = "0.0.2"
+version = "0.0.2.1"
 authors = [
   { name="Paul Wilson", email="paul@statusfailed.com" }
 ]
 description = "yarrow diagrams"
 readme = "README.md"
 requires-python = ">= 3.7"
 classifiers = [
```

### Comparing `yarrow_diagrams-0.0.2/PKG-INFO` & `yarrow_diagrams-0.0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yarrow-diagrams
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: yarrow diagrams
 Project-URL: Homepage, https://yarrow.id
 Project-URL: Github, https://github.com/yarrow-id/diagrams/
 Project-URL: Documentation, https://yarrow-diagrams.readthedocs.io/
 Author-email: Paul Wilson <paul@statusfailed.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

