# Comparing `tmp/discopy-1.1.0.tar.gz` & `tmp/discopy-1.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discopy-1.1.0.tar", last modified: Wed May 24 09:01:49 2023, max compression
+gzip compressed data, was "discopy-1.1.0a0.tar", last modified: Wed May 24 09:41:26 2023, max compression
```

## Comparing `discopy-1.1.0.tar` & `discopy-1.1.0a0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:01:49.535480 discopy-1.1.0/
--rw-r--r--   0 aleumi     (502) staff       (20)     1520 2023-04-18 08:36:50.000000 discopy-1.1.0/LICENSE
--rw-r--r--   0 aleumi     (502) staff       (20)     5160 2023-05-24 09:01:49.535785 discopy-1.1.0/PKG-INFO
--rw-r--r--   0 aleumi     (502) staff       (20)     4532 2023-05-24 08:20:40.000000 discopy-1.1.0/README.md
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:01:49.489088 discopy-1.1.0/discopy/
--rw-r--r--   0 aleumi     (502) staff       (20)      424 2023-05-24 08:20:29.000000 discopy-1.1.0/discopy/__init__.py
--rw-r--r--   0 aleumi     (502) staff       (20)     5758 2023-05-23 16:32:40.000000 discopy-1.1.0/discopy/balanced.py
--rw-r--r--   0 aleumi     (502) staff       (20)     8612 2023-05-23 16:31:12.000000 discopy-1.1.0/discopy/braided.py
--rw-r--r--   0 aleumi     (502) staff       (20)    28200 2023-05-23 16:32:41.000000 discopy-1.1.0/discopy/cat.py
--rw-r--r--   0 aleumi     (502) staff       (20)     8982 2023-05-23 16:24:44.000000 discopy-1.1.0/discopy/closed.py
--rw-r--r--   0 aleumi     (502) staff       (20)     4413 2023-05-23 16:32:40.000000 discopy-1.1.0/discopy/compact.py
--rw-r--r--   0 aleumi     (502) staff       (20)      236 2023-05-23 16:24:44.000000 discopy-1.1.0/discopy/config.py
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:01:49.499871 discopy-1.1.0/discopy/drawing/
--rw-r--r--   0 aleumi     (502) staff       (20)     1060 2023-05-23 16:32:40.000000 discopy-1.1.0/discopy/drawing/__init__.py
--rw-r--r--   0 aleumi     (502) staff       (20)    13920 2023-05-23 16:33:01.000000 discopy-1.1.0/discopy/drawing/grid.py
--rw-r--r--   0 aleumi     (502) staff       (20)    37886 2023-05-23 16:32:40.000000 discopy-1.1.0/discopy/drawing/legacy.py
--rw-r--r--   0 aleumi     (502) staff       (20)    11613 2023-05-24 08:19:50.000000 discopy-1.1.0/discopy/frobenius.py
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:01:49.514610 discopy-1.1.0/discopy/grammar/
--rw-r--r--   0 aleumi     (502) staff       (20)      225 2023-04-18 08:36:50.000000 discopy-1.1.0/discopy/grammar/__init__.py
--rw-r--r--   0 aleumi     (502) staff       (20)     9597 2023-05-23 16:24:44.000000 discopy-1.1.0/discopy/grammar/categorial.py
--rw-r--r--   0 aleumi     (502) staff       (20)     6890 2023-04-18 08:36:50.000000 discopy-1.1.0/discopy/grammar/cfg.py
--rw-r--r--   0 aleumi     (502) staff       (20)      926 2023-04-18 08:36:50.000000 discopy-1.1.0/discopy/grammar/dependency.py
--rw-r--r--   0 aleumi     (502) staff       (20)     5550 2023-05-23 16:32:21.000000 discopy-1.1.0/discopy/grammar/pregroup.py
--rw-r--r--   0 aleumi     (502) staff       (20)     2410 2023-05-24 08:43:34.000000 discopy-1.1.0/discopy/grammar/thue.py
--rw-r--r--   0 aleumi     (502) staff       (20)    48229 2023-05-23 16:33:01.000000 discopy-1.1.0/discopy/hypergraph.py
--rw-r--r--   0 aleumi     (502) staff       (20)    14082 2023-05-23 16:32:40.000000 discopy-1.1.0/discopy/interaction.py
--rw-r--r--   0 aleumi     (502) staff       (20)     8057 2023-05-24 08:54:26.000000 discopy-1.1.0/discopy/markov.py
--rw-r--r--   0 aleumi     (502) staff       (20)    14740 2023-05-23 16:32:41.000000 discopy-1.1.0/discopy/matrix.py
--rw-r--r--   0 aleumi     (502) staff       (20)     1617 2023-05-23 16:31:12.000000 discopy-1.1.0/discopy/messages.py
--rw-r--r--   0 aleumi     (502) staff       (20)    34458 2023-05-23 16:33:01.000000 discopy-1.1.0/discopy/monoidal.py
--rw-r--r--   0 aleumi     (502) staff       (20)     6871 2023-05-23 16:31:13.000000 discopy-1.1.0/discopy/pivotal.py
--rw-r--r--   0 aleumi     (502) staff       (20)     7845 2023-05-23 16:32:40.000000 discopy-1.1.0/discopy/python.py
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:01:49.533141 discopy-1.1.0/discopy/quantum/
--rw-r--r--   0 aleumi     (502) staff       (20)      667 2023-04-18 08:36:50.000000 discopy-1.1.0/discopy/quantum/__init__.py
--rw-r--r--   0 aleumi     (502) staff       (20)     5238 2023-04-18 08:36:50.000000 discopy-1.1.0/discopy/quantum/ansatze.py
--rw-r--r--   0 aleumi     (502) staff       (20)    11626 2023-04-18 08:36:50.000000 discopy-1.1.0/discopy/quantum/channel.py
--rw-r--r--   0 aleumi     (502) staff       (20)    33893 2023-05-24 07:55:57.000000 discopy-1.1.0/discopy/quantum/circuit.py
--rw-r--r--   0 aleumi     (502) staff       (20)    22165 2023-05-23 16:37:12.000000 discopy-1.1.0/discopy/quantum/gates.py
--rw-r--r--   0 aleumi     (502) staff       (20)    15738 2023-05-24 07:55:57.000000 discopy-1.1.0/discopy/quantum/pennylane.py
--rw-r--r--   0 aleumi     (502) staff       (20)    16429 2023-05-24 07:55:57.000000 discopy-1.1.0/discopy/quantum/tk.py
--rw-r--r--   0 aleumi     (502) staff       (20)    13451 2023-05-23 16:32:40.000000 discopy-1.1.0/discopy/quantum/zx.py
--rw-r--r--   0 aleumi     (502) staff       (20)     6916 2023-05-23 16:31:12.000000 discopy-1.1.0/discopy/ribbon.py
--rw-r--r--   0 aleumi     (502) staff       (20)    26017 2023-05-23 16:24:44.000000 discopy-1.1.0/discopy/rigid.py
--rw-r--r--   0 aleumi     (502) staff       (20)     9003 2023-05-23 16:33:01.000000 discopy-1.1.0/discopy/symmetric.py
--rw-r--r--   0 aleumi     (502) staff       (20)    23052 2023-05-23 16:33:01.000000 discopy-1.1.0/discopy/tensor.py
--rw-r--r--   0 aleumi     (502) staff       (20)     7593 2023-05-23 16:32:41.000000 discopy-1.1.0/discopy/traced.py
--rw-r--r--   0 aleumi     (502) staff       (20)    18153 2023-05-23 16:33:01.000000 discopy-1.1.0/discopy/utils.py
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:01:49.495721 discopy-1.1.0/discopy.egg-info/
--rw-r--r--   0 aleumi     (502) staff       (20)     5160 2023-05-24 09:01:49.000000 discopy-1.1.0/discopy.egg-info/PKG-INFO
--rw-r--r--   0 aleumi     (502) staff       (20)     1055 2023-05-24 09:01:49.000000 discopy-1.1.0/discopy.egg-info/SOURCES.txt
--rw-r--r--   0 aleumi     (502) staff       (20)        1 2023-05-24 09:01:49.000000 discopy-1.1.0/discopy.egg-info/dependency_links.txt
--rw-r--r--   0 aleumi     (502) staff       (20)      412 2023-05-24 09:01:49.000000 discopy-1.1.0/discopy.egg-info/requires.txt
--rw-r--r--   0 aleumi     (502) staff       (20)        8 2023-05-24 09:01:49.000000 discopy-1.1.0/discopy.egg-info/top_level.txt
--rw-r--r--   0 aleumi     (502) staff       (20)      208 2023-05-24 09:01:49.536976 discopy-1.1.0/setup.cfg
--rw-r--r--   0 aleumi     (502) staff       (20)     2163 2023-04-18 08:36:51.000000 discopy-1.1.0/setup.py
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:41:26.953556 discopy-1.1.0a0/
+-rw-r--r--   0 aleumi     (502) staff       (20)     1520 2023-04-18 08:36:50.000000 discopy-1.1.0a0/LICENSE
+-rw-r--r--   0 aleumi     (502) staff       (20)     5163 2023-05-24 09:41:26.953856 discopy-1.1.0a0/PKG-INFO
+-rw-r--r--   0 aleumi     (502) staff       (20)     4532 2023-05-24 09:11:24.000000 discopy-1.1.0a0/README.md
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:41:26.866685 discopy-1.1.0a0/discopy/
+-rw-r--r--   0 aleumi     (502) staff       (20)      425 2023-05-24 09:39:26.000000 discopy-1.1.0a0/discopy/__init__.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     5758 2023-05-23 16:32:40.000000 discopy-1.1.0a0/discopy/balanced.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     8328 2023-05-24 09:11:24.000000 discopy-1.1.0a0/discopy/braided.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    28200 2023-05-23 16:32:41.000000 discopy-1.1.0a0/discopy/cat.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    10182 2023-05-24 09:11:24.000000 discopy-1.1.0a0/discopy/closed.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     4417 2023-05-24 09:11:24.000000 discopy-1.1.0a0/discopy/compact.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     1487 2023-05-24 09:11:24.000000 discopy-1.1.0a0/discopy/config.py
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:41:26.885961 discopy-1.1.0a0/discopy/drawing/
+-rw-r--r--   0 aleumi     (502) staff       (20)     1060 2023-05-23 16:32:40.000000 discopy-1.1.0a0/discopy/drawing/__init__.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    13920 2023-05-23 16:33:01.000000 discopy-1.1.0a0/discopy/drawing/grid.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    36769 2023-05-24 09:11:24.000000 discopy-1.1.0a0/discopy/drawing/legacy.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    11613 2023-05-24 09:11:24.000000 discopy-1.1.0a0/discopy/frobenius.py
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:41:26.926894 discopy-1.1.0a0/discopy/grammar/
+-rw-r--r--   0 aleumi     (502) staff       (20)      225 2023-04-18 08:36:50.000000 discopy-1.1.0a0/discopy/grammar/__init__.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     9405 2023-05-24 09:11:24.000000 discopy-1.1.0a0/discopy/grammar/categorial.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     6890 2023-04-18 08:36:50.000000 discopy-1.1.0a0/discopy/grammar/cfg.py
+-rw-r--r--   0 aleumi     (502) staff       (20)      926 2023-04-18 08:36:50.000000 discopy-1.1.0a0/discopy/grammar/dependency.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     7162 2023-05-24 09:11:24.000000 discopy-1.1.0a0/discopy/grammar/pregroup.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     2410 2023-05-24 09:11:24.000000 discopy-1.1.0a0/discopy/grammar/thue.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    48280 2023-05-24 09:11:24.000000 discopy-1.1.0a0/discopy/hypergraph.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    14028 2023-05-24 09:11:24.000000 discopy-1.1.0a0/discopy/interaction.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     8050 2023-05-24 09:11:24.000000 discopy-1.1.0a0/discopy/markov.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    16146 2023-05-24 09:11:24.000000 discopy-1.1.0a0/discopy/matrix.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     1555 2023-05-24 09:11:24.000000 discopy-1.1.0a0/discopy/messages.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    35222 2023-05-24 09:11:24.000000 discopy-1.1.0a0/discopy/monoidal.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     6871 2023-05-23 16:31:13.000000 discopy-1.1.0a0/discopy/pivotal.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     7845 2023-05-23 16:32:40.000000 discopy-1.1.0a0/discopy/python.py
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:41:26.950197 discopy-1.1.0a0/discopy/quantum/
+-rw-r--r--   0 aleumi     (502) staff       (20)      667 2023-04-18 08:36:50.000000 discopy-1.1.0a0/discopy/quantum/__init__.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     5238 2023-04-18 08:36:50.000000 discopy-1.1.0a0/discopy/quantum/ansatze.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    11626 2023-04-18 08:36:50.000000 discopy-1.1.0a0/discopy/quantum/channel.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    32818 2023-05-24 09:11:24.000000 discopy-1.1.0a0/discopy/quantum/circuit.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    24488 2023-05-24 09:11:24.000000 discopy-1.1.0a0/discopy/quantum/gates.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    15738 2023-05-24 07:55:57.000000 discopy-1.1.0a0/discopy/quantum/pennylane.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    16429 2023-05-24 07:55:57.000000 discopy-1.1.0a0/discopy/quantum/tk.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    13451 2023-05-23 16:32:40.000000 discopy-1.1.0a0/discopy/quantum/zx.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     6916 2023-05-23 16:31:12.000000 discopy-1.1.0a0/discopy/ribbon.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    25765 2023-05-24 09:11:24.000000 discopy-1.1.0a0/discopy/rigid.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     9007 2023-05-24 09:11:24.000000 discopy-1.1.0a0/discopy/symmetric.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    23082 2023-05-24 09:11:24.000000 discopy-1.1.0a0/discopy/tensor.py
+-rw-r--r--   0 aleumi     (502) staff       (20)     7593 2023-05-23 16:32:41.000000 discopy-1.1.0a0/discopy/traced.py
+-rw-r--r--   0 aleumi     (502) staff       (20)    20851 2023-05-24 09:11:24.000000 discopy-1.1.0a0/discopy/utils.py
+drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-24 09:41:26.880418 discopy-1.1.0a0/discopy.egg-info/
+-rw-r--r--   0 aleumi     (502) staff       (20)     5163 2023-05-24 09:41:25.000000 discopy-1.1.0a0/discopy.egg-info/PKG-INFO
+-rw-r--r--   0 aleumi     (502) staff       (20)     1055 2023-05-24 09:41:26.000000 discopy-1.1.0a0/discopy.egg-info/SOURCES.txt
+-rw-r--r--   0 aleumi     (502) staff       (20)        1 2023-05-24 09:41:25.000000 discopy-1.1.0a0/discopy.egg-info/dependency_links.txt
+-rw-r--r--   0 aleumi     (502) staff       (20)      412 2023-05-24 09:41:25.000000 discopy-1.1.0a0/discopy.egg-info/requires.txt
+-rw-r--r--   0 aleumi     (502) staff       (20)        8 2023-05-24 09:41:25.000000 discopy-1.1.0a0/discopy.egg-info/top_level.txt
+-rw-r--r--   0 aleumi     (502) staff       (20)      261 2023-05-24 09:41:26.959013 discopy-1.1.0a0/setup.cfg
+-rw-r--r--   0 aleumi     (502) staff       (20)     2185 2023-05-24 09:37:47.000000 discopy-1.1.0a0/setup.py
```

### Comparing `discopy-1.1.0/LICENSE` & `discopy-1.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `discopy-1.1.0/PKG-INFO` & `discopy-1.1.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: discopy
-Version: 1.1.0
+Version: 1.1.0a0
 Summary: The Python toolkit for computing with string diagrams.
 Home-page: https://discopy.org
-Download-URL: https://github.com/discopy/discopy/archive/1.1.0.tar.gz
+Download-URL: https://github.com/discopy/discopy/archive/1.1.0a.tar.gz
 Author: Alexis Toumi
 Author-email: alexis@toumi.email
 Project-URL: Documentation, https://docs.discopy.org
 Project-URL: Source, https://github.com/discopy/discopy
 Project-URL: Tracker, https://github.com/discopy/discopy/issues
 Keywords: diagrams category-theory quantum-computing nlp
 Requires-Python: >=3.9
```

### Comparing `discopy-1.1.0/README.md` & `discopy-1.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `discopy-1.1.0/discopy/balanced.py` & `discopy-1.1.0a0/discopy/balanced.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.0/discopy/braided.py` & `discopy-1.1.0a0/discopy/braided.py`

 * *Files 16% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 from __future__ import annotations
 
 from collections.abc import Callable
 
 from discopy import monoidal
 from discopy.cat import factory, AxiomError
 from discopy.monoidal import Ty, assert_isatomic, Match
-from discopy.utils import factory_name, from_tree
+from discopy.utils import factory_name, from_tree, BinaryBoxConstructor
 
 
 @factory
 class Diagram(monoidal.Diagram):
     """
     A braided diagram is a monoidal diagram with :class:`Braid` boxes.
 
@@ -108,14 +108,27 @@
         Slide a box through a braid.
 
         Parameters:
             i : The index of the box to slide.
             left : Whether to slide left or right.
             down : Whether to slide down or up.
             braid : The braiding method to be used.
+
+        Examples
+        --------
+        >>> x, y, z = map(Ty, "xyz")
+        >>> f = Box('f', x, y)
+        >>> top_left = f @ z >> Braid(y, z)
+        >>> top_right = z @ f >> Braid(z, y)
+        >>> bot_left = Braid(z, x) >> f @ z
+        >>> bot_right = Braid(x, z) >> z @ f
+        >>> assert top_right.naturality(0) == bot_left
+        >>> assert top_left.naturality(0, left=False) == bot_right
+        >>> assert bot_right.naturality(1, down=False) == top_left
+        >>> assert bot_left.naturality(1, left=False, down=False) == top_right
         """
         braid = braid or self.braid
         left_wires, box, right_wires = self.inside[i]
         if left and down:
             source = left_wires[-1] @ box >> braid(left_wires[-1], box.cod)
             target = braid(left_wires[-1], box.dom) >> box @ left_wires[-1]
         elif left:
@@ -142,40 +155,14 @@
         name (str) : The name of the box.
         dom (monoidal.Ty) : The domain of the box, i.e. its input.
         cod (monoidal.Ty) : The codomain of the box, i.e. its output.
     """
     __ambiguous_inheritance__ = (monoidal.Box, )
 
 
-class BinaryBoxConstructor:
-    """
-    Box constructor with attributes ``left`` and ``right`` as input.
-
-    Parameters:
-        left : Some attribute on the left.
-        right : Some attribute on the right.
-    """
-    def __init__(self, left, right):
-        self.left, self.right = left, right
-
-    def __repr__(self):
-        return factory_name(type(self))\
-            + f"({repr(self.left)}, {repr(self.right)})"
-
-    def to_tree(self) -> dict:
-        """ Serialise a binary box constructor. """
-        left, right = self.left.to_tree(), self.right.to_tree()
-        return dict(factory=factory_name(type(self)), left=left, right=right)
-
-    @classmethod
-    def from_tree(cls, tree: dict) -> BinaryBoxConstructor:
-        """ Decode a serialised binary box constructor. """
-        return cls(*map(from_tree, (tree['left'], tree['right'])))
-
-
 class Braid(BinaryBoxConstructor, Box):
     """
     The braiding of atomic types :code:`left` and :code:`right`.
 
     Parameters:
         left : The type on the top left and bottom right.
         right : The type on the top right and bottom left.
```

### Comparing `discopy-1.1.0/discopy/cat.py` & `discopy-1.1.0a0/discopy/cat.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.0/discopy/closed.py` & `discopy-1.1.0a0/discopy/closed.py`

 * *Files 13% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 .. image:: /_static/closed/uncurry.png
     :align: center
 """
 
 from __future__ import annotations
 
-from discopy import cat, monoidal
+from discopy import cat, monoidal, messages
 from discopy.cat import Category, factory
 from discopy.utils import (
     factory_name,
     from_tree,
 )
 
 
@@ -92,32 +92,81 @@
     def __rshift__(self, other):
         return Under(other, self)
 
     def __repr__(self):
         return factory_name(type(self))\
             + f"({', '.join(map(repr, self.inside))})"
 
+    @property
+    def left(self) -> Ty:
+        return self.inside[0].left if self.is_exp else None
+
+    @property
+    def right(self) -> Ty:
+        return self.inside[0].right if self.is_exp else None
+
+    @property
+    def is_exp(self):
+        """
+        Whether the type is an :class:`Exp` object.
+
+        Example
+        -------
+        >>> x, y = Ty('x'), Ty('y')
+        >>> assert (x ** y).is_exp and (x ** y @ Ty()).is_exp
+        """
+        return len(self) == 1 and isinstance(self.inside[0], Exp)
+
+    @property
+    def is_under(self):
+        """
+        Whether the type is an :class:`Under` object.
+
+        Example
+        -------
+        >>> x, y = Ty('x'), Ty('y')
+        >>> assert (x >> y).is_under and (x >> y @ Ty()).is_under
+        """
+        return len(self) == 1 and isinstance(self.inside[0], Under)
+
+    @property
+    def is_over(self):
+        """
+        Whether the type is an :class:`Over` object.
+
+        Example
+        -------
+        >>> x, y = Ty('x'), Ty('y')
+        >>> assert (x << y).is_over and (x << y @ Ty()).is_over
+        """
+        return len(self) == 1 and isinstance(self.inside[0], Over)
+
 
 class Exp(Ty, cat.Ob):
     """
     A :code:`base` type to an :code:`exponent` type, called with :code:`**`.
 
     Parameters:
         base : The base type.
         exponent : The exponent type.
     """
     __ambiguous_inheritance__ = (cat.Ob, )
 
     def __init__(self, base: Ty, exponent: Ty):
         self.base, self.exponent = base, exponent
-        # TODO : replace left and right by base and exponent
-        self.left, self.right =\
-            (exponent, base) if isinstance(self, Under) else (base, exponent)
         super().__init__(self)
 
+    @property
+    def left(self):
+        return self.exponent if isinstance(self, Under) else self.base
+
+    @property
+    def right(self):
+        return self.base if isinstance(self, Under) else self.exponent
+
     def __eq__(self, other):
         if isinstance(other, type(self)):
             return (self.base, self.exponent) == (other.base, other.exponent)
         if isinstance(other, Exp):
             return False  # Avoid infinite loop with Over(x, y) == Under(x, y).
         return isinstance(other, Ty) and other.inside == (self, )
```

### Comparing `discopy-1.1.0/discopy/compact.py` & `discopy-1.1.0a0/discopy/compact.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 >>> assert Diagram.caps(x @ y, y.r @ x.r)\\
 ...     == Cap(x, x.r) @ Cap(y, y.r) >> x @ Diagram.swap(x.r, y @ y.r)
 """
 
 from discopy import symmetric, ribbon
 from discopy.cat import factory
-from discopy.pivotal import Ty
+from discopy.pivotal import Ob, Ty
 
 
 @factory
 class Diagram(symmetric.Diagram, ribbon.Diagram):
     """
     A compact diagram is a symmetric diagram and a ribbon diagram.
```

### Comparing `discopy-1.1.0/discopy/drawing/__init__.py` & `discopy-1.1.0a0/discopy/drawing/__init__.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.0/discopy/drawing/grid.py` & `discopy-1.1.0a0/discopy/drawing/grid.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.0/discopy/drawing/legacy.py` & `discopy-1.1.0a0/discopy/drawing/legacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,58 +35,17 @@
 
 import matplotlib.pyplot as plt
 from PIL import Image
 from matplotlib.patches import PathPatch
 from matplotlib.path import Path
 
 from discopy.utils import assert_isinstance
-
-# Mapping from attribute to function from box to default value.
-ATTRIBUTES = {
-    "draw_as_braid": lambda _: False,
-    "draw_as_wires": lambda box: box.draw_as_braid,
-    "draw_as_spider": lambda _: False,
-    "draw_as_brakets": lambda _: False,
-    "draw_as_discards": lambda _: False,
-    "draw_as_measures": lambda _: False,
-    "draw_as_controlled": lambda _: False,
-    "shape": lambda box:
-        "circle" if getattr(box, "draw_as_spider", False) else None,
-    "color": lambda box:
-        "red" if getattr(box, "draw_as_spider", False) else "white",
-    "drawing_name": lambda box: box.name,
-    "tikzstyle_name": lambda box: box.name,
-}
-# Default drawing parameters.
-DEFAULT = {
-    "aspect": "auto",
-    "fontsize": 12,
-    "margins": (.05, .1),
-    "textpad": (.1, .1),
-    "color": 'white',
-    "use_tikzstyles": False,
-    "braid_shadow": (.3, .1)
-}
-# Mapping from tikz colors to hexcodes.
-COLORS = {
-    "white": '#ffffff',
-    "red": '#e8a5a5',
-    "green": '#d8f8d8',
-    "blue": '#776ff3',
-    "yellow": '#f7f700',
-    "black": '#000000',
-}
-# Mapping from tikz shapes to matplotlib shapes.
-SHAPES = {
-    "rectangle": 's',
-    "triangle_up": '^',
-    "triangle_down": 'v',
-    "circle": 'o',
-    "plus": '+',
-}
+from discopy.config import (
+    DRAWING_ATTRIBUTES as ATTRIBUTES,
+    DRAWING_DEFAULT as DEFAULT, COLORS, SHAPES)
 
 
 class Node:
     """ Node in a :class:`networkx.Graph`, can hold arbitrary data. """
     def __init__(self, kind, **data):
         self.kind, self.data = kind, data
         for key, value in data.items():
```

### Comparing `discopy-1.1.0/discopy/frobenius.py` & `discopy-1.1.0a0/discopy/frobenius.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.0/discopy/grammar/categorial.py` & `discopy-1.1.0a0/discopy/grammar/categorial.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 .. autosummary::
     :template: class.rst
     :nosignatures:
     :toctree:
 
     Diagram
-    Rule
+    Box
     Word
     FA
     BA
     FC
     BC
     FX
     BX
@@ -32,35 +32,35 @@
         cat2ty
         tree2diagram
 """
 
 import re
 
 from discopy import closed, messages
-from discopy.braided import BinaryBoxConstructor
 from discopy.cat import factory, AxiomError
 from discopy.grammar import thue
-from discopy.utils import assert_isinstance, factory_name, from_tree
+from discopy.closed import Ty, Over, Under
+from discopy.utils import (
+    assert_isinstance, factory_name, from_tree, BinaryBoxConstructor)
 
 
 @factory
 class Diagram(closed.Diagram):
     """
     A categorial diagram is a closed diagram with rules and words as boxes.
     """
     def to_pregroup(self):
-        from discopy import rigid
         from discopy.grammar import pregroup
 
         return Functor(
             ob=lambda x: pregroup.Ty(x.inside[0].name),
             ar=lambda f: pregroup.Box(f.name,
                                       Diagram.to_pregroup(f.dom),
                                       Diagram.to_pregroup(f.cod)),
-            cod=rigid.Category(rigid.Ty, pregroup.Diagram))(self)
+            cod=pregroup.Category())(self)
 
     @staticmethod
     def fa(left, right):
         """ Forward application. """
         return FA(left << right)
 
     @staticmethod
@@ -85,39 +85,39 @@
 
     @staticmethod
     def bx(left, middle, right):
         """ Backward crossed composition. """
         return BX(middle << left, middle >> right)
 
 
-class Rule(thue.Rule, Diagram):
+class Box(closed.Box, Diagram):
     """
-    A categorial rule is a grammar rule in a categorial diagram.
+    A categorial box is a grammar rule in a categorial diagram.
     """
 
 
-class Word(thue.Word, Rule):
+class Word(thue.Word, Box):
     """
     A categorial word is a rule with a ``name``, a grammatical type as ``cod``
     and an optional domain ``dom``.
 
     Parameters:
         name (str) : The name of the word.
         cod (closed.Ty) : The grammatical type of the word.
         dom (closed.Ty) : An optional domain for the word, empty by default.
     """
 
 
-class Eval(closed.Eval, Rule):
+class Eval(closed.Eval, Box):
     """
     Evaluation box in a categorial grammar, equivalent to :class:``FA``.
     """
 
 
-class Curry(closed.Curry, Rule):
+class Curry(closed.Curry, Box):
     """
     The currying of a categorial diagram.
     """
 
 
 def unaryBoxConstructor(attr):
     class Constructor:
@@ -128,105 +128,105 @@
         def to_tree(self):
             return {
                 'factory': factory_name(type(self)),
                 attr: getattr(self, attr).to_tree()}
     return Constructor
 
 
-class FA(unaryBoxConstructor("over"), Rule):
+class FA(unaryBoxConstructor("over"), Box):
     """ Forward application rule. """
     def __init__(self, over):
-        assert_isinstance(over, closed.Over)
+        assert_isinstance(over, Over)
         self.over = over
         dom, cod = over @ over.exponent, over.base
-        Rule.__init__(self, dom, cod, name=f"FA{over}")
+        Box.__init__(self, f"FA{over}", dom, cod)
 
     def __repr__(self):
         return f"FA({repr(self.dom[:1])})"
 
 
-class BA(unaryBoxConstructor("under"), Rule):
+class BA(unaryBoxConstructor("under"), Box):
     """ Backward application rule. """
     def __init__(self, under):
-        assert_isinstance(under, closed.Under)
+        assert_isinstance(under, Under)
         self.under = under
         dom, cod = under.exponent @ under, under.base
-        Rule.__init__(self, dom, cod, name=f"BA{under}")
+        Box.__init__(self, f"BA{under}", dom, cod)
 
     def __repr__(self):
         return f"BA({repr(self.dom[1:])})"
 
 
-class FC(BinaryBoxConstructor, Rule):
+class FC(BinaryBoxConstructor, Box):
     """ Forward composition rule. """
     def __init__(self, left, right):
-        assert_isinstance(left, closed.Over)
-        assert_isinstance(right, closed.Over)
+        assert_isinstance(left, Over)
+        assert_isinstance(right, Over)
         if left.exponent != right.base:
             raise AxiomError(messages.NOT_COMPOSABLE.format(
                 left, right, left.exponent, right.base))
         name = f"FC({left}, {right})"
         dom, cod = left @ right, left.base << right.exponent
-        Rule.__init__(self, dom, cod, name=name)
+        Box.__init__(self, name, dom, cod)
         BinaryBoxConstructor.__init__(self, left, right)
 
 
-class BC(BinaryBoxConstructor, Rule):
+class BC(BinaryBoxConstructor, Box):
     """ Backward composition rule. """
     def __init__(self, left, right):
-        assert_isinstance(left, closed.Under)
-        assert_isinstance(right, closed.Under)
+        assert_isinstance(left, Under)
+        assert_isinstance(right, Under)
         if left.base != right.exponent:
             raise AxiomError(messages.NOT_COMPOSABLE.format(
                 left, right, left.base, right.exponent))
         name = f"BC({left}, {right})"
         dom, cod = left @ right, left.exponent >> right.base
-        Rule.__init__(self, dom, cod, name=name)
+        Box.__init__(self, name, dom, cod)
         BinaryBoxConstructor.__init__(self, left, right)
 
 
-class FX(BinaryBoxConstructor, Rule):
+class FX(BinaryBoxConstructor, Box):
     """ Forward crossed composition rule. """
     def __init__(self, left, right):
-        assert_isinstance(left, closed.Over)
-        assert_isinstance(right, closed.Under)
+        assert_isinstance(left, Over)
+        assert_isinstance(right, Under)
         if left.exponent != right.base:
             raise AxiomError(messages.NOT_COMPOSABLE.format(
                 left, right, left.exponent, right.base))
         name = f"FX({left}, {right})"
         dom, cod = left @ right, right.exponent >> left.base
-        Rule.__init__(self, dom, cod, name=name)
+        Box.__init__(self, name, dom, cod)
         BinaryBoxConstructor.__init__(self, left, right)
 
 
-class BX(BinaryBoxConstructor, Rule):
+class BX(BinaryBoxConstructor, Box):
     """ Backward crossed composition rule. """
     def __init__(self, left, right):
-        assert_isinstance(left, closed.Over)
-        assert_isinstance(right, closed.Under)
+        assert_isinstance(left, Over)
+        assert_isinstance(right, Under)
         if left.base != right.exponent:
             raise AxiomError(messages.NOT_COMPOSABLE.format(
                 left, right, left.base, right.exponent))
         name = f"BX({left}, {right})"
         dom, cod = left @ right, right.base << left.exponent
-        Rule.__init__(self, dom, cod, name=name)
+        Box.__init__(self, name, dom, cod)
         BinaryBoxConstructor.__init__(self, left, right)
 
 
 class Functor(closed.Functor):
     """
     A categorial functor is a closed functor with a predefined mapping
     for categorial rules.
 
     Parameters:
         ob (Mapping[Ty, Ty]) : Map from atomic :class:`Ty` to :code:`cod.ob`.
         ar (Mapping[Box, Diagram]) : Map from :class:`Box` to :code:`cod.ar`.
         cod (Category) : The codomain of the functor.
     """
-    dom = cod = closed.Category(closed.Ty, Diagram)
+    dom = cod = closed.Category(Ty, Diagram)
 
     def __call__(self, other):
         if isinstance(other, FA):
             left, right = other.over.left, other.over.right
             return self.cod.ar.fa(self(left), self(right))
         if isinstance(other, BA):
             left, right = other.under.left, other.under.right
@@ -247,15 +247,15 @@
             left = other.dom.inside[0].right
             middle = other.dom.inside[0].left
             right = other.dom.inside[1].right
             return self.cod.ar.bx(self(left), self(middle), self(right))
         return super().__call__(other)
 
 
-def cat2ty(string: str) -> closed.Ty:
+def cat2ty(string: str) -> Ty:
     """
     Translate the string representation of a CCG category into DisCoPy.
 
     Parameters:
         string : The string with slashes representing a CCG category.
     """
     def unbracket(string):
@@ -276,37 +276,37 @@
         return remove_modifier(string), None, None
 
     left, slash, right = split(string)
     if slash == '\\':
         return cat2ty(right) >> cat2ty(left)
     if slash == '/':
         return cat2ty(left) << cat2ty(right)
-    return closed.Ty(left)
+    return Ty(left)
 
 
-def tree2diagram(tree: dict, dom=closed.Ty()) -> Diagram:
+def tree2diagram(tree: dict, dom=Ty()) -> Diagram:
     """
     Translate a depccg.Tree in JSON format into DisCoPy.
 
     Parameters:
         tree : The tree to translate.
         dom : The domain for the word boxes, empty by default.
     """
     if 'word' in tree:
         return Word(tree['word'], cat2ty(tree['cat']), dom=dom)
     children = list(map(tree2diagram, tree['children']))
-    dom = closed.Ty().tensor(*[child.cod for child in children])
+    dom = Ty().tensor(*[child.cod for child in children])
     cod = cat2ty(tree['cat'])
     if tree['type'] == 'ba':
         box = BA(dom.inside[1])
     elif tree['type'] == 'fa':
         box = FA(dom.inside[0])
     elif tree['type'] == 'fc':
         box = FC(dom.inside[0], dom.inside[1])
     else:
-        box = Rule(dom, cod, name=tree['type'])
+        box = Box(tree['type'], dom, cod)
     return Id().tensor(*children) >> box
 
 
 Id = Diagram.id
 Diagram.curry_factory = Curry
 Diagram.eval_factory = Eval
```

### Comparing `discopy-1.1.0/discopy/grammar/cfg.py` & `discopy-1.1.0a0/discopy/grammar/cfg.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.0/discopy/grammar/dependency.py` & `discopy-1.1.0a0/discopy/grammar/dependency.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.0/discopy/grammar/thue.py` & `discopy-1.1.0a0/discopy/grammar/thue.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.0/discopy/hypergraph.py` & `discopy-1.1.0a0/discopy/hypergraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 import matplotlib.pyplot as plt
 
 from networkx import (
     DiGraph as Graph,
     spring_layout,
     draw_networkx,
     dag_longest_path_length,
+    weisfeiler_lehman_graph_hash,
 )
 from networkx.algorithms.isomorphism import is_isomorphic
 
 from discopy import drawing, messages
 from discopy.cat import Category
 from discopy.drawing import Node
 from discopy.utils import (
@@ -518,16 +519,16 @@
     def __eq__(self, other: Any):
         if not isinstance(other, Hypergraph):
             return False
         return self.is_parallel(other) and is_isomorphic(
             self.to_graph(), other.to_graph(), lambda x, y: x == y)
 
     def __hash__(self):
-        return hash(getattr(self, attr) for attr in [
-            'dom', 'cod', 'boxes', 'wires', 'n_spiders'])
+        return hash((self.dom, self.cod, weisfeiler_lehman_graph_hash(
+            self.to_graph(), node_attr="box")))
 
     def __repr__(self):
         spider_types = f", spider_types={self.spider_types}"\
             if self.scalar_spiders else ""
         return factory_name(type(self))\
             + f"(dom={repr(self.dom)}, cod={repr(self.cod)}, " \
               f"boxes={repr(self.boxes)}, " \
@@ -1078,15 +1079,15 @@
             box_node = Node("box", box=box, i=i)
             graph.add_node(box_node, box=box)
             for case, wires in [("dom", dom_wires), ("cod", cod_wires)]:
                 for j, spider in enumerate(wires):
                     obj = self.spider_types[spider]
                     spider_node = Node("spider", i=spider, obj=obj)
                     port_node = Node(case, i=i, j=j)
-                    graph.add_node(port_node, j=j)
+                    graph.add_node(port_node, j=j, box=None)
                     if case == "dom":
                         graph.add_edge(spider_node, port_node)
                         graph.add_edge(port_node, box_node)
                     else:
                         graph.add_edge(box_node, port_node)
                         graph.add_edge(port_node, spider_node)
         graph.add_nodes_from(
```

### Comparing `discopy-1.1.0/discopy/interaction.py` & `discopy-1.1.0a0/discopy/interaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,23 +30,22 @@
 
         Int
 
 Example
 -------
 
 >>> from discopy.grammar import pregroup
->>> from discopy.grammar.pregroup import Word, Cup, Diagram
+>>> from discopy.grammar.pregroup import Word, Cup, Diagram, Functor
 >>> s, n = map(pregroup.Ty, "sn")
 >>> Alice, loves, Bob\\
 ...     = Word('Alice', n), Word('loves', n.r @ s @ n.l), Word('Bob', n)
 >>> who = Word('who', n.r @ n @ (n.r @ s).l)
 >>> noun_phrase = Alice @ who @ loves @ Bob\\
 ...     >> Cup(n, n.r) @ n @ Diagram.cups((n.r @ s).l, n.r @ s) @ Cup(n.l, n)
 
->>> from discopy.rigid import Functor
 >>> from discopy.frobenius import Ty as T, Diagram as D, Box, Category, Swap
 >>> S, N = map(T, "SN")
 >>> F = Functor(
 ...     ob={s: Ty[T](S), n: Ty[T](N)},
 ...     ar={Alice: Box('A', T(), N),
 ...         who: Box('W', S @ N, N @ N),
 ...         loves: Box('L', N @ N, S),
@@ -67,15 +66,14 @@
 from dataclasses import dataclass
 from functools import wraps
 
 from discopy import (
     balanced, traced, rigid, pivotal, ribbon, frobenius, messages)
 from discopy.cat import Composable, assert_iscomposable
 from discopy.monoidal import Whiskerable
-from discopy.rigid import assert_isadjoint
 from discopy.utils import (
     NamedGeneric, unbiased, assert_isinstance, factory_name)
 
 
 @dataclass
 class Ty(NamedGeneric['natural']):
     """
@@ -322,28 +320,28 @@
         ...     Diagram.id(x),
         ...     x @ Diagram.caps(-x, x) >> Diagram.cups(x, -x) @ x).draw(
         ...         path="docs/_static/int/int-snake-equations.png")
 
         .. image:: /_static/int/int-snake-equations.png
             :align: center
         """
-        assert_isadjoint(left, right)
+        rigid.Ty.assert_isadjoint(left, right)
         inside = cls.natural.id(left.positive + left.negative)
         return cls(inside, left @ right, type(left)())
 
     @classmethod
     def caps(cls, left: Ty, right: Ty) -> Diagram:
         """
         The integer caps are given by natural identities.
 
         Parameters:
             left : The left-hand side of the caps.
             right : The right-hand side of the caps.
         """
-        assert_isadjoint(left, right)
+        rigid.Ty.assert_isadjoint(right, left)
         inside = cls.natural.id(left.negative + left.positive)
         return cls(inside, type(left)(), left @ right)
 
     def dagger(self):
         """
         The dagger of an integer diagram is given by the dagger of its inside.
```

### Comparing `discopy-1.1.0/discopy/markov.py` & `discopy-1.1.0a0/discopy/markov.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-The free Markov category, i.e. the free semicartesian category with a supply of
+The free Markov category, i.e. a semicartesian category with a supply of
 commutative comonoid, see :cite:t:`FritzLiang23`.
 
 Summary
 -------
 
 .. autosummary::
     :template: class.rst
```

### Comparing `discopy-1.1.0/discopy/matrix.py` & `discopy-1.1.0a0/discopy/matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,27 +20,30 @@
 
     .. autosummary::
         :template: function.rst
         :nosignatures:
         :toctree:
 
         backend
+        set_backend
         get_backend
 
 See also
 --------
 
 * :class:`Tensor` is a subclass of :class:`Matrix` with the Kronecker product
   as tensor.
 * :class:`Matrix` is used to evaluate :class:`quantum.optics.Diagram`.
 
 """
 from __future__ import annotations
 
 from contextlib import contextmanager
+from types import ModuleType
+from typing import Union, Literal as L
 
 from discopy import cat, monoidal, config, messages
 from discopy.cat import (
     factory,
     Composable,
     assert_iscomposable,
     assert_isparallel,
@@ -418,66 +421,118 @@
     import numpy
     numpy.set_printoptions(threshold=config.NUMPY_THRESHOLD)
     return numpy.array2string(array, **dict(params, separator=', '))\
         .replace('[ ', '[').replace('  ', ' ')
 
 
 class Backend:
-    def __init__(self, module, array=None):
+    """
+    A matrix backend.
+
+    Parameters:
+        module : The main module of the backend.
+        array : The array class of the backend.
+    """
+    def __init__(self, module: ModuleType, array: type = None):
         self.module, self.array = module, array or module.array
 
     def __getattr__(self, attr):
         return getattr(self.module, attr)
 
 
 class NumPy(Backend):
+    """ NumPy backend. """
     def __init__(self):
         import numpy
         super().__init__(numpy)
 
 
 class JAX(Backend):
+    """ JAX backend. """
     def __init__(self):
         import jax
         super().__init__(jax.numpy)
 
 
 class PyTorch(Backend):
+    """ PyTorch backend. """
     def __init__(self):
         import torch
         super().__init__(torch, array=torch.as_tensor)
 
 
 class TensorFlow(Backend):
+    """ TensorFlow backend. """
     def __init__(self):
         import tensorflow.experimental.numpy as tnp
         from tensorflow.python.ops.numpy_ops import np_config
         np_config.enable_numpy_behavior()
         super().__init__(tnp)
 
 
 BACKENDS = {
-    'np': NumPy,
     'numpy': NumPy,
     'jax': JAX,
-    'jax.numpy': JAX,
     'pytorch': PyTorch,
-    'torch': PyTorch,
     'tensorflow': TensorFlow,
 }
 
+BackendName = Union[tuple(L[x] for x in BACKENDS)]
+
 
 @contextmanager
-def backend(name=None, _stack=[config.DEFAULT_BACKEND], _cache=dict()):
+def backend(name: BackendName = None,
+            _stack=[config.DEFAULT_BACKEND], _cache=dict()):
+    """
+    Context manager for matrix backend.
+
+    Parameters:
+        name : The name of the backend, default is ``"numpy"``.
+
+    Example
+    -------
+    >>> with backend('jax'):
+    ...     assert type(Matrix([0, 1, 1, 0], 2, 2).array).__module__\\
+    ...         == 'jaxlib.xla_extension'
+    """
     name = name or _stack[-1]
     _stack.append(name)
     try:
         if name not in _cache:
             _cache[name] = BACKENDS[name]()
         yield _cache[name]
     finally:
         _stack.pop()
 
 
-def get_backend():
+def set_backend(name: BackendName) -> None:
+    """
+    Override the default backend.
+
+    Parameters:
+        name : The name of the backend.
+
+    Example
+    -------
+    >>> set_backend('jax')
+    >>> assert type(Matrix([0, 1, 1, 0], 2, 2).array).__module__\\
+    ...     == 'jaxlib.xla_extension'
+    >>> set_backend('numpy')
+    >>> assert type(Matrix([0, 1, 1, 0], 2, 2).array).__module__\\
+    ...     == 'numpy'
+    """
+    backend.__wrapped__.__defaults__[1][-1] = name
+
+
+def get_backend() -> Backend:
+    """
+    Get the current backend.
+
+    Example
+    -------
+    >>> set_backend('jax')
+    >>> assert isinstance(get_backend(), JAX)
+    >>> set_backend('numpy')
+    >>> assert isinstance(get_backend(), NumPy)
+    """
     with backend() as result:
         return result
```

### Comparing `discopy-1.1.0/discopy/messages.py` & `discopy-1.1.0a0/discopy/messages.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,23 +9,22 @@
 NOT_PARALLEL = "Expected parallel arrows, got {} and {} instead."
 NOT_ATOMIC = "Expected {} of length 1, got length {} instead."
 NOT_CONNECTED = "{} is not boundary-connected."
 NOT_TRACEABLE = "Cannot trace {} with {}."
 NOT_ADJOINT = "{} and {} are not adjoints."
 NOT_RIGID_ADJOINT = "{} is not the left adjoint of {}, maybe you meant to use"\
                     " a pivotal type rather than a rigid one?"
-NOT_PREGROUP = "Expected a pregroup diagram of shape `word @ ... @ word "\
-               ">> cups_and_swaps`, use diagram.draw() instead."
 MISSING_TYPES_FOR_EMPTY_SUM = "Empty sum needs a domain and codomain."
 MATRIX_TWO_DTYPES = "Matrix class cannot be indexed twice."
 MATRIX_REPEAT_ERROR = "The reflexive transitive closure is only defined for "\
                       "square boolean matrices."
 PROVIDE_CONTRACTOR = "Provide a contractor when using a non-numpy backend."
 BOX_IS_MIXED = "Pure boxes can have only digits or only qudits as dom and cod."
 LAYERS_MUST_BE_ODD = "Layers must have an odd number of boxes and types."
 NOT_MERGEABLE = "Layers {} and {} cannot be merged."
 INTERCHANGER_ERROR = "Boxes {} and {} do not commute."
 WRONG_PERMUTATION = "Expected a permutation of length {}, got {}."
 ZERO_DISTANCE_CONTROLLED = "Zero-distance controlled gates are ill-defined."
 HAS_NO_ATTRIBUTE = "{!r} object has no attribute {!r}"
 WRONG_DOM = "Expected inside.dom == {}, got {} instead."
 WRONG_COD = "Expected inside.cod == {}, got {} instead."
+COMPLEX_TYPE_HAS_NO_ATTR = "{!r} object of length != 1 has no attribute {!r}"
```

### Comparing `discopy-1.1.0/discopy/monoidal.py` & `discopy-1.1.0a0/discopy/monoidal.py`

 * *Files 2% similar despite different names*

```diff
@@ -582,28 +582,52 @@
 
         .. image:: /_static/monoidal/arrow-example.png
             :align: center
         """
         return self.dom, list(zip(self.boxes, self.offsets))
 
     @classmethod
-    def decode(cls, dom: Ty, boxes_and_offsets: list[tuple[Box, int]]
-               ) -> Diagram:
+    def decode(
+            cls,
+            dom: Ty,
+            boxes_and_offsets: list[tuple[Box, int]] = None,
+            boxes: list[Box] = None,
+            offsets: list[int] = None,
+            cod: Ty = None) -> Diagram:
         """
         Turn a tuple of boxes and offsets into a diagram.
 
         Parameters:
             dom : The domain of the diagram.
+            cod : The codomain of the diagram.
             boxes_and_offsets : The boxes and offsets of the diagram.
+            boxes : The list of boxes.
+            offsets : The list of offsets.
+
+        Example
+        -------
+        >>> x, y, z, w = map(Ty, "xyzw")
+        >>> f, g = Box('f', x, y), Box('g', z, w)
+        >>> assert f @ z >> y @ g == Diagram.decode(
+        ...     dom=x @ z, cod=y @ w, boxes=[f, g], offsets=[0, 1])
+
+        Note
+        ----
+        If ``boxes_and_offsets is None``
+        then we set it to ``zip(boxes, offstes)``.
         """
+        if boxes_and_offsets is None:
+            boxes_and_offsets = zip(boxes, offsets)
         diagram = cls.id(dom)
         for box, offset in boxes_and_offsets:
             left = diagram.cod[:offset]
             right = diagram.cod[offset + len(box.dom):]
             diagram = diagram >> left @ box @ right
+        if cod is not None:
+            assert_iscomposable(diagram, cls.id(cod))
         return diagram
 
     def to_drawing(self):
         """ Called before :meth:`Diagram.draw`. """
         return cat.Functor(
             ob=lambda x: x.to_drawing(), ar=Layer.to_drawing, cod=Category())(
                 self)
@@ -663,15 +687,14 @@
 
     def depth(self):
         """
         Computes (an upper bound to) the depth of a diagram by foliating it.
 
         Example
         -------
-        >>> from discopy.monoidal import *
         >>> x, y = Ty('x'), Ty('y')
         >>> f, g = Box('f', x, y), Box('g', y, x)
         >>> assert Id(x @ y).depth() == 0
         >>> assert f.depth() == 1
         >>> assert (f @ g).depth() == 1
         >>> assert (f >> g).depth() == 2
 
@@ -786,20 +809,20 @@
         ------
         NotImplementedError
             Whenever ``normalize`` yields the same rewrite steps twice, e.g.
             the diagram is not boundary-connected.
         """
         cache = set()
         for diagram in itertools.chain([self], self.normalize(**params)):
-            if diagram in cache:
+            if str(diagram) in cache:
                 exception = NotImplementedError(
                     messages.NOT_CONNECTED.format(self))
                 exception.last_step = diagram
                 raise exception
-            cache.add(diagram)
+            cache.add(str(diagram))
         return diagram
 
     @classmethod
     def from_tree(cls, tree):
         if "inside" not in tree:
             warn("Outdated dumps", DeprecationWarning)
             boxes, offsets = map(from_tree, tree['boxes']), tree['offsets']
```

### Comparing `discopy-1.1.0/discopy/pivotal.py` & `discopy-1.1.0a0/discopy/pivotal.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.0/discopy/python.py` & `discopy-1.1.0a0/discopy/python.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.0/discopy/quantum/__init__.py` & `discopy-1.1.0a0/discopy/quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.0/discopy/quantum/ansatze.py` & `discopy-1.1.0a0/discopy/quantum/ansatze.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.0/discopy/quantum/channel.py` & `discopy-1.1.0a0/discopy/quantum/channel.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.0/discopy/quantum/circuit.py` & `discopy-1.1.0a0/discopy/quantum/circuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 >>> Bob = pregroup.Word('Bob', n)
 >>> grammar = pregroup.Cup(n, n.r) @ s @ pregroup.Cup(n.l, n)
 >>> sentence = grammar << Alice @ loves @ Bob
 >>> ob = {s: Ty(), n: qubit}
 >>> ar = {Alice: Ket(0),
 ...       loves: CX << sqrt(2) @ H @ X << Ket(0, 0),
 ...       Bob: Ket(1)}
->>> F = rigid.Functor(ob, ar, cod=Category(Ty, Circuit))
+>>> F = pregroup.Functor(ob, ar, cod=Category(Ty, Circuit))
 >>> assert abs(F(sentence).eval().array) ** 2
 
 >>> from discopy.drawing import Equation
 >>> Equation(
 ...     sentence.to_drawing(), F(sentence), symbol='$\\\\mapsto$').draw(
 ...         figsize=(6, 3), nodesize=.5,
 ...         path='docs/_static/quantum/functor-example.png')
@@ -775,35 +775,14 @@
             gate, head = Controlled(gate, distance=head - x), x
         head = indices[-1]
         for x in sorted(filter(lambda x: x > head, indices)):
             gate, head = Controlled(gate, distance=head - x), x
         return self\
             >> self.cod[:offset] @ gate @ self.cod[offset + len(gate.dom):]
 
-    def __getattr__(self, attr):
-        from discopy.quantum.gates import GATES, Box, Rotation, Controlled
-        if attr in GATES:
-            gate = GATES[attr]
-            if isinstance(gate, Controlled)\
-                    and isinstance(gate.controlled, Controlled):
-                gate = gate.controlled.controlled
-                return lambda i, j, k: self.apply_controlled(gate, i, j, k)
-            if isinstance(gate, Controlled):
-                gate = gate.controlled
-                return lambda i, j: self.apply_controlled(gate, i, j)
-            if isinstance(gate, Box):
-                return lambda i: self.apply_controlled(gate, i)
-            if issubclass(gate, Rotation) and issubclass(gate, Controlled):
-                gate = gate.controlled
-                return lambda phi, i, j: self.apply_controlled(gate(phi), i, j)
-            if issubclass(gate, Rotation):
-                return lambda phi, i: self.apply_controlled(gate(phi), i)
-        raise AttributeError(messages.HAS_NO_ATTRIBUTE.format(
-            factory_name(type(self)), attr))
-
 
 class Box(tensor.Box, Circuit):
     """
     A circuit box is a tensor box in a circuit diagram.
 
     Parameters:
         name : The name of the box.
```

### Comparing `discopy-1.1.0/discopy/quantum/gates.py` & `discopy-1.1.0a0/discopy/quantum/gates.py`

 * *Files 14% similar despite different names*

```diff
@@ -293,15 +293,15 @@
         """ The digits of a classical state. """
         return list(self._digits)
 
     bitstring = digits
 
     @property
     def array(self):
-        with backend() as np:
+        with backend('numpy') as np:
             array = np.zeros(len(self._digits) * (self._dim, ))
             array[self._digits] = 1
             return array
 
     def dagger(self):
         return Digits(*self.digits, dim=self.dim, is_dagger=not self.is_dagger)
 
@@ -754,7 +754,68 @@
     'Ry': Ry,
     'Rz': Rz,
     'U1': U1,
     'CRx': CRx,
     'CRz': CRz,
     'CU1': CU1,
 }
+
+
+for attr, gate in GATES.items():
+    def closure(attr=attr, gate=gate):
+        """ Eaiest way around the Python late binding gotcha. """
+        if isinstance(gate, Controlled)\
+                and isinstance(gate.controlled, Controlled):
+            def method(self, i: int, j: int, k: int) -> Circuit:
+                """
+                Apply {} gate to a circuit given qubit indices.
+
+                Parameters:
+                    i : First control index.
+                    j : Second control index.
+                    k : Target index.
+                """
+                return self.apply_controlled(
+                    gate.controlled.controlled, i, j, k)
+        elif isinstance(gate, Controlled):
+            def method(self, i: int, j: int) -> Circuit:
+                """
+                Apply {} gate to a circuit given qubit indices.
+
+                Parameters:
+                    i : Control index.
+                    j : Target index.
+                """
+                return self.apply_controlled(gate.controlled, i, j)
+        elif isinstance(gate, Box):
+            def method(self, i: int) -> Circuit:
+                """
+                Apply {} gate to a circuit given qubit index.
+
+                Parameters:
+                    i : Target index.
+                """
+                return self.apply_controlled(gate, i)
+        elif issubclass(gate, Rotation) and issubclass(gate, Controlled):
+            def method(self, phi: float, i: int, j: int) -> Circuit:
+                """
+                Apply :class:`{}` to a circuit given phase and indices.
+
+                Parameters:
+                    phi : Phase.
+                    i : Control index.
+                    j : Target index.
+                """
+                return self.apply_controlled(gate.controlled(phi), i, j)
+        elif issubclass(gate, Rotation):
+            def method(self, phi: float, i: int) -> Circuit:
+                """
+                Apply :class:`{}` to a circuit given phase and target index.
+
+                Parameters:
+                    phi : Phase.
+                    i : Target index.
+                """
+                return self.apply_controlled(gate(phi), i)
+        method.__doc__ = method.__doc__.format(attr)
+        return method
+    setattr(Circuit, attr, closure())
```

### Comparing `discopy-1.1.0/discopy/quantum/pennylane.py` & `discopy-1.1.0a0/discopy/quantum/pennylane.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.0/discopy/quantum/tk.py` & `discopy-1.1.0a0/discopy/quantum/tk.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.0/discopy/quantum/zx.py` & `discopy-1.1.0a0/discopy/quantum/zx.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.0/discopy/ribbon.py` & `discopy-1.1.0a0/discopy/ribbon.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.0/discopy/rigid.py` & `discopy-1.1.0a0/discopy/rigid.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,18 +41,17 @@
 """
 
 from __future__ import annotations
 
 from collections.abc import Callable
 
 from discopy import cat, monoidal, closed, messages
-from discopy.braided import BinaryBoxConstructor
 from discopy.cat import AxiomError, factory
 from discopy.monoidal import assert_isatomic
-from discopy.utils import assert_isinstance, factory_name
+from discopy.utils import assert_isinstance, factory_name, BinaryBoxConstructor
 
 
 class Ob(cat.Ob):
     """
     A rigid object has adjoints :meth:`Ob.l` and :meth:`Ob.r`.
 
     Parameters:
@@ -563,16 +562,16 @@
     def __hash__(self):
         return hash(repr(self))
 
     def rotate(self, left=False):
         dom, cod = (
             getattr(x, 'l' if left else 'r') for x in (self.cod, self.dom))
         z = self.z + (-1 if left else 1)
-        return type(self)(
-            self.name, dom, cod, data=self.data, is_dagger=self.is_dagger, z=z)
+        return type(self)(self.name, dom=dom, cod=cod,
+                          data=self.data, is_dagger=self.is_dagger, z=z)
 
     @property
     def is_transpose(self):
         """ Whether the box is an odd rotation of a generator. """
         return not self.is_dagger and self.z and bool(self.z % 2)
 
     def to_drawing(self):
@@ -588,23 +587,18 @@
     Parameters:
         terms (tuple[Diagram, ...]) : The terms of the formal sum.
         dom (Ty) : The domain of the formal sum.
         cod (Ty) : The codomain of the formal sum.
     """
     __ambiguous_inheritance__ = (monoidal.Sum, )
 
-    @property
-    def l(self) -> Sum:
-        """ The left transpose of a sum, i.e. the sum of left transposes. """
-        return self.sum_factory(
-            tuple(term.l for term in self.terms), self.cod.l, self.dom.l)
-
-    @property
-    def r(self) -> Sum:
-        """ The right transpose of a sum, i.e. the sum of right transposes. """
+    def rotate(self, left=False) -> Sum:
+        if left:
+            return self.sum_factory(
+                tuple(term.l for term in self.terms), self.cod.l, self.dom.l)
         return self.sum_factory(
             tuple(term.r for term in self.terms), self.cod.r, self.dom.r)
 
 
 class Cup(BinaryBoxConstructor, Box):
     """
     The counit of the adjunction for an atomic type.
@@ -621,27 +615,23 @@
 
     .. image:: /_static/rigid/cup.png
         :align: center
     """
     def __init__(self, left: Ty, right: Ty):
         assert_isatomic(left, Ty)
         assert_isatomic(right, Ty)
-        assert_isadjoint(left, right)
+        left.assert_isadjoint(right)
         name = f"Cup({left}, {right})"
         dom, cod = left @ right, self.ty_factory()
         BinaryBoxConstructor.__init__(self, left, right)
         Box.__init__(self, name, dom, cod, draw_as_wires=True)
 
-    @property
-    def l(self):
-        return self.cap_factory(self.right.l, self.left.l)
-
-    @property
-    def r(self):
-        return self.cap_factory(self.right.r, self.left.r)
+    def rotate(self, left=False):
+        return self.cap_factory(self.right.l, self.left.l) if left\
+            else self.cap_factory(self.right.r, self.left.r)
 
     def dagger(self):
         """
         The dagger of a rigid cup is ill-defined,
         use a :class:`pivotal.Cup` instead.
         """
         raise AxiomError("Rigid cups have no dagger, use pivotal instead.")
@@ -663,27 +653,23 @@
 
     .. image:: /_static/rigid/cap.png
         :align: center
     """
     def __init__(self, left: Ty, right: Ty):
         assert_isatomic(left, Ty)
         assert_isatomic(right, Ty)
-        assert_isadjoint(right, left)
+        right.assert_isadjoint(left)
         name = f"Cap({left}, {right})"
         dom, cod = self.ty_factory(), left @ right
         BinaryBoxConstructor.__init__(self, left, right)
         Box.__init__(self, name, dom, cod, draw_as_wires=True)
 
-    @property
-    def l(self):
-        return self.cup_factory(self.right.l, self.left.l)
-
-    @property
-    def r(self):
-        return self.cup_factory(self.right.r, self.left.r)
+    def rotate(self, left=False):
+        return self.cup_factory(self.right.l, self.left.l) if left\
+            else self.cup_factory(self.right.r, self.left.r)
 
     def dagger(self):
         """
         The dagger of a rigid cap is ill-defined,
         use a :class:`pivotal.Cap` instead.
         """
         raise AxiomError("Rigid caps have no dagger, use pivotal instead.")
@@ -771,11 +757,10 @@
         if head.dom:  # We are nesting cups.
             return left[0] @ tail @ right[-1] >> head
         return head >> left[0] @ tail @ right[-1]
 
     return method
 
 
-assert_isadjoint = Ty.assert_isadjoint
 Diagram.cup_factory, Diagram.cap_factory, Diagram.sum_factory = Cup, Cap, Sum
 
 Id = Diagram.id
```

### Comparing `discopy-1.1.0/discopy/symmetric.py` & `discopy-1.1.0a0/discopy/symmetric.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     :align: center
 """
 
 from __future__ import annotations
 
 from discopy import monoidal, balanced, hypergraph, messages
 from discopy.cat import factory
-from discopy.monoidal import Ty, PRO
+from discopy.monoidal import Ob, Ty, PRO
 
 
 @factory
 class Diagram(balanced.Diagram):
     """
     A symmetric diagram is a balanced diagram with :class:`Swap` boxes.
```

### Comparing `discopy-1.1.0/discopy/tensor.py` & `discopy-1.1.0a0/discopy/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,16 @@
 
 from typing import Callable
 
 from discopy import (
     cat, monoidal, rigid, symmetric, frobenius)
 from discopy.cat import factory, assert_iscomposable
 from discopy.frobenius import Dim, Cup, Category
-from discopy.matrix import Matrix, backend
+from discopy.matrix import Matrix, backend, set_backend, get_backend
 from discopy.monoidal import assert_isatomic
-from discopy.rigid import assert_isadjoint
 from discopy.utils import factory_name, assert_isinstance, product
 
 
 @factory
 class Tensor(Matrix):
     """
     A tensor is a :class:`Matrix` with dimensions as domain and codomain and
@@ -87,15 +86,15 @@
     ...     [phi * phi.conjugate() + psi * psi.conjugate()], Dim(1), Dim(1))
 
     These can be substituted and lambdifed.
 
     >>> v.subs(phi, 0).lambdify(psi, dtype=int)(1)
     Tensor[int]([0, 1], dom=Dim(1), cod=Dim(2))
 
-    We can also use jax.numpy using Tensor.backend.
+    We can also use jax.numpy using :func:`backend`.
 
     >>> with backend('jax'):
     ...     f = lambda *xs: d.lambdify(phi, psi, dtype=float)(*xs).array
     ...     import jax
     ...     assert jax.grad(f)(1., 2.) == 2.
     """
     def __class_getitem__(cls, dtype: type, _cache=dict()):
@@ -149,15 +148,15 @@
             array = np.conjugate(np.moveaxis(self.array, source, target))
         return type(self)(array, self.cod, self.dom)
 
     @classmethod
     def cup_factory(cls, left: Dim, right: Dim) -> Tensor:
         assert_isinstance(left, Dim)
         assert_isinstance(right, Dim)
-        assert_isadjoint(left, right)
+        left.assert_isadjoint(right)
         return cls(cls.id(left).array, left @ right, Dim(1))
 
     @classmethod
     def cups(cls, left: Dim, right: Dim) -> Tensor:
         return rigid.nesting(cls, cls.cup_factory)(left, right)
 
     @classmethod
@@ -178,18 +177,19 @@
     def spider_factory(cls, n_legs_in: int, n_legs_out: int,
                        typ: Dim, phase=None) -> Tensor:
         if phase is not None:
             raise NotImplementedError
         assert_isatomic(typ, Dim)
         n, = typ.inside
         dom, cod = typ ** n_legs_in, typ ** n_legs_out
-        result = cls.zero(dom, cod)
-        for i in range(n):
-            result.array[len(dom @ cod) * (i, )] = 1
-        return result
+        with backend('numpy'):
+            result = cls.zero(dom, cod)
+            for i in range(n):
+                result.array[len(dom @ cod) * (i, )] = 1
+            return result
 
     @classmethod
     def spiders(cls, n_legs_in: int, n_legs_out: int, typ: Dim, phase=None
                 ) -> Tensor:
         """
         The tensor of interleaving spiders.
```

### Comparing `discopy-1.1.0/discopy/traced.py` & `discopy-1.1.0a0/discopy/traced.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.0/discopy/utils.py` & `discopy-1.1.0a0/discopy/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 # -*- coding: utf-8 -*-
 
 """ DisCoPy utility functions. """
 
 from __future__ import annotations
 
+import os
+import json
+from functools import wraps
 from abc import ABC, abstractmethod
 from typing import (
     Callable,
     Generic,
     Mapping,
     Iterable,
     TypeVar,
     Any,
+    Hashable,
+    Literal,
+    cast,
+    Union,
     Collection,
     Type,
     Optional,
     TYPE_CHECKING,
 )
 
 import json
 from functools import wraps
 from networkx import Graph, connected_components
+from matplotlib.testing.compare import compare_images
 
 from discopy import messages
+from discopy.config import DRAWING_DEFAULT
+
 if TYPE_CHECKING:
     from discopy.monoidal import Ty, Diagram
 
 KT = TypeVar('KT')
 VT = TypeVar('VT')
 V2T = TypeVar('V2T')
 
@@ -391,14 +401,79 @@
     right_proper = set(range(right)) - set(right_boundary)
     right_pushout.update({
         j: len(left_proper) + len(components) + i
         for i, j in enumerate(right_proper)})
     return left_pushout, right_pushout
 
 
+class BinaryBoxConstructor:
+    """
+    Box constructor with attributes ``left`` and ``right`` as input.
+
+    Parameters:
+        left : Some attribute on the left.
+        right : Some attribute on the right.
+    """
+    def __init__(self, left, right):
+        self.left, self.right = left, right
+
+    def __repr__(self):
+        return factory_name(type(self))\
+            + f"({repr(self.left)}, {repr(self.right)})"
+
+    def to_tree(self) -> dict:
+        """ Serialise a binary box constructor. """
+        left, right = self.left.to_tree(), self.right.to_tree()
+        return dict(factory=factory_name(type(self)), left=left, right=right)
+
+    @classmethod
+    def from_tree(cls, tree: dict) -> BinaryBoxConstructor:
+        """ Decode a serialised binary box constructor. """
+        return cls(*map(from_tree, (tree['left'], tree['right'])))
+
+
+def draw_and_compare(file, folder, tol, **params):
+    """ Draw a given diagram and compare the result with a baseline. """
+    def decorator(func):
+        def wrapper():
+            diagram = func()
+            draw = params.get('draw', type(diagram).draw)
+            true_path = os.path.join(folder, file)
+            test_path = os.path.join(folder, '.' + file)
+            draw(diagram, path=test_path, show=False, **params)
+            test = compare_images(true_path, test_path, tol)
+            assert test is None
+            os.remove(test_path)
+        return wrapper
+    return decorator
+
+
+def tikz_and_compare(file, folder, **params):
+    """ Tikz a given diagram and compare the result with a baseline. """
+    def decorator(func):
+        def wrapper():
+            diagram = func()
+            draw = params.get('draw', type(diagram).draw)
+            true_paths = [os.path.join(folder, file)]
+            test_paths = [os.path.join(folder, '.' + file)]
+            if params.get("use_tikzstyles", DRAWING_DEFAULT['use_tikzstyles']):
+                true_paths.append(
+                    true_paths[0].replace('.tikz', '.tikzstyles'))
+                test_paths.append(
+                    test_paths[0].replace('.tikz', '.tikzstyles'))
+            draw(diagram, path=test_paths[0], **dict(params, to_tikz=True))
+            for true_path, test_path in zip(true_paths, test_paths):
+                with open(true_path, "r") as true:
+                    with open(test_path, "r") as test:
+                        assert true.read() == test.read()
+                os.remove(test_path)
+        return wrapper
+    return decorator
+
+
 def tuplify(stuff: any) -> tuple:
     """
     Turns anything into a tuple, do nothing if it is already.
 
     Parameters:
         stuff : The stuff to turn into a tuple.
     """
```

### Comparing `discopy-1.1.0/discopy.egg-info/PKG-INFO` & `discopy-1.1.0a0/discopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: discopy
-Version: 1.1.0
+Version: 1.1.0a0
 Summary: The Python toolkit for computing with string diagrams.
 Home-page: https://discopy.org
-Download-URL: https://github.com/discopy/discopy/archive/1.1.0.tar.gz
+Download-URL: https://github.com/discopy/discopy/archive/1.1.0a.tar.gz
 Author: Alexis Toumi
 Author-email: alexis@toumi.email
 Project-URL: Documentation, https://docs.discopy.org
 Project-URL: Source, https://github.com/discopy/discopy
 Project-URL: Tracker, https://github.com/discopy/discopy/issues
 Keywords: diagrams category-theory quantum-computing nlp
 Requires-Python: >=3.9
```

### Comparing `discopy-1.1.0/discopy.egg-info/SOURCES.txt` & `discopy-1.1.0a0/discopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discopy-1.1.0/setup.py` & `discopy-1.1.0a0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Setup discopy package.
 """
 
 if __name__ == '__main__':  # pragma: no cover
+    import pathlib
     from re import search, M
     from setuptools import setup, find_packages
 
     def get_version(filename="discopy/__init__.py",
                     pattern=r"^__version__ = ['\"]([^'\"]*)['\"]"):
         with open(filename, 'r') as file:
             MATCH = search(pattern, file.read(), M)
@@ -15,43 +16,45 @@
             else:
                 raise RuntimeError("Unable to find version string.")
 
     VERSION = get_version()
 
     def get_reqs(filename):
         try:
-            with open(filename, 'r') as file:
+            with pathlib.Path(filename).open() as file:
                 return [line.strip() for line in file.readlines()]
         except FileNotFoundError:
             from warnings import warn
             warn("{} not found".format(filename))
             return []
 
+    REQS = get_reqs("requirements.txt")
     TEST_REQS = get_reqs("test/requirements.txt")
     DOCS_REQS = get_reqs("docs/requirements.txt")
 
+    README = open("README.md", "r").read()
+
     setup(name='discopy',
           version=VERSION,
           package_dir={'discopy': 'discopy'},
           packages=find_packages(),
           description='The Python toolkit for computing with string diagrams.',
-          long_description=open("README.md", "r").read(),
+          long_description=README,
           long_description_content_type="text/markdown",
           url='https://discopy.org',
           project_urls={
             'Documentation': 'https://docs.discopy.org',
             'Source': 'https://github.com/discopy/discopy',
             'Tracker': 'https://github.com/discopy/discopy/issues',
           },
           keywords='diagrams category-theory quantum-computing nlp',
           author='Alexis Toumi',
           author_email='alexis@toumi.email',
           download_url='https://github.com/discopy/discopy/archive/'
                        f'{VERSION}.tar.gz',
-          install_requires=[
-              l.strip() for l in open('requirements.txt').readlines()],
+          install_requires=REQS,
           tests_require=TEST_REQS,
           extras_require={'test': TEST_REQS, 'docs': DOCS_REQS},
           data_file=[('test', ['test/requirements.txt']),
                      ('docs', ['docs/requirements.txt'])],
           python_requires='>=3.9',
           )
```

