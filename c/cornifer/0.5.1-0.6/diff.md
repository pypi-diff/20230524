# Comparing `tmp/cornifer-0.5.1.tar.gz` & `tmp/cornifer-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cornifer-0.5.1.tar", last modified: Tue Oct 18 16:03:39 2022, max compression
+gzip compressed data, was "cornifer-0.6.tar", last modified: Thu May 18 14:34:08 2023, max compression
```

## Comparing `cornifer-0.5.1.tar` & `cornifer-0.6.tar`

### file list

```diff
@@ -1,28 +1,33 @@
-drwxrwxrwx   0        0        0        0 2022-10-18 16:03:39.973165 cornifer-0.5.1/
--rw-rw-rw-   0        0        0    35823 2021-08-18 02:15:58.000000 cornifer-0.5.1/LICENSE
--rw-rw-rw-   0        0        0      663 2022-10-18 16:03:39.972164 cornifer-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1376 2022-07-25 17:02:05.000000 cornifer-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2022-10-18 16:03:39.928540 cornifer-0.5.1/lib/
-drwxrwxrwx   0        0        0        0 2022-10-18 16:03:39.953571 cornifer-0.5.1/lib/Cornifer.egg-info/
--rw-rw-rw-   0        0        0      663 2022-10-18 16:03:39.000000 cornifer-0.5.1/lib/Cornifer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      776 2022-10-18 16:03:39.000000 cornifer-0.5.1/lib/Cornifer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-18 16:03:39.000000 cornifer-0.5.1/lib/Cornifer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2022-07-23 17:35:39.000000 cornifer-0.5.1/lib/Cornifer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2022-10-18 16:03:39.000000 cornifer-0.5.1/lib/Cornifer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-10-18 16:03:39.000000 cornifer-0.5.1/lib/Cornifer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-10-18 16:03:39.966176 cornifer-0.5.1/lib/cornifer/
--rw-rw-rw-   0        0        0      897 2022-09-20 19:30:38.000000 cornifer-0.5.1/lib/cornifer/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-18 16:03:39.970165 cornifer-0.5.1/lib/cornifer/_utilities/
--rw-rw-rw-   0        0        0     8649 2022-09-22 16:04:35.000000 cornifer-0.5.1/lib/cornifer/_utilities/__init__.py
--rw-rw-rw-   0        0        0     5685 2022-09-20 19:34:07.000000 cornifer-0.5.1/lib/cornifer/_utilities/lmdb.py
--rw-rw-rw-   0        0        0     7875 2022-09-27 15:43:01.000000 cornifer-0.5.1/lib/cornifer/blocks.py
--rw-rw-rw-   0        0        0     1096 2022-08-25 21:25:33.000000 cornifer-0.5.1/lib/cornifer/errors.py
--rw-rw-rw-   0        0        0      913 2022-08-26 21:17:53.000000 cornifer-0.5.1/lib/cornifer/example.py
--rw-rw-rw-   0        0        0     2406 2022-09-20 19:30:19.000000 cornifer-0.5.1/lib/cornifer/filemetadata.py
--rw-rw-rw-   0        0        0     9481 2022-09-20 19:29:59.000000 cornifer-0.5.1/lib/cornifer/info.py
--rw-rw-rw-   0        0        0     1975 2022-09-19 17:36:03.000000 cornifer-0.5.1/lib/cornifer/regfilestructure.py
--rw-rw-rw-   0        0        0   127174 2022-10-17 17:19:29.000000 cornifer-0.5.1/lib/cornifer/registers.py
--rw-rw-rw-   0        0        0    12242 2022-09-20 19:29:59.000000 cornifer-0.5.1/lib/cornifer/regloader.py
--rw-rw-rw-   0        0        0      739 2022-10-18 16:03:13.000000 cornifer-0.5.1/lib/cornifer/version.py
--rw-rw-rw-   0        0        0       42 2022-10-18 16:03:39.973165 cornifer-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1897 2022-09-27 16:45:39.000000 cornifer-0.5.1/setup.py
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-18 14:34:08.868078 cornifer-0.6/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    35823 2021-08-18 02:15:58.000000 cornifer-0.6/LICENSE
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      644 2023-05-18 14:34:08.861554 cornifer-0.6/PKG-INFO
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1376 2022-07-25 17:02:05.000000 cornifer-0.6/README.md
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-18 14:34:07.200326 cornifer-0.6/lib/
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-18 14:34:07.590525 cornifer-0.6/lib/Cornifer.egg-info/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      644 2023-05-18 14:34:06.000000 cornifer-0.6/lib/Cornifer.egg-info/PKG-INFO
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      878 2023-05-18 14:34:07.000000 cornifer-0.6/lib/Cornifer.egg-info/SOURCES.txt
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        1 2023-05-18 14:34:06.000000 cornifer-0.6/lib/Cornifer.egg-info/dependency_links.txt
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        1 2022-07-23 17:35:39.000000 cornifer-0.6/lib/Cornifer.egg-info/not-zip-safe
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)       35 2023-05-18 14:34:06.000000 cornifer-0.6/lib/Cornifer.egg-info/requires.txt
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        9 2023-05-18 14:34:06.000000 cornifer-0.6/lib/Cornifer.egg-info/top_level.txt
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-18 14:34:08.226106 cornifer-0.6/lib/cornifer/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      897 2022-09-20 19:30:38.000000 cornifer-0.6/lib/cornifer/__init__.py
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-18 14:34:08.577875 cornifer-0.6/lib/cornifer/_utilities/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     8766 2023-05-10 18:49:26.000000 cornifer-0.6/lib/cornifer/_utilities/__init__.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     5805 2023-05-15 19:09:23.000000 cornifer-0.6/lib/cornifer/_utilities/lmdb.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     7900 2023-05-11 19:22:17.000000 cornifer-0.6/lib/cornifer/blocks.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1096 2022-08-25 21:25:33.000000 cornifer-0.6/lib/cornifer/errors.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      943 2023-05-12 15:41:02.000000 cornifer-0.6/lib/cornifer/example.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     2407 2023-05-10 16:54:32.000000 cornifer-0.6/lib/cornifer/filemetadata.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    13499 2023-05-16 15:37:22.000000 cornifer-0.6/lib/cornifer/info.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1987 2023-05-10 16:57:49.000000 cornifer-0.6/lib/cornifer/regfilestructure.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)   126656 2023-05-17 17:38:30.000000 cornifer-0.6/lib/cornifer/registers.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    12323 2023-05-11 19:22:17.000000 cornifer-0.6/lib/cornifer/regloader.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)      730 2023-05-17 19:06:29.000000 cornifer-0.6/lib/cornifer/version.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)       38 2023-05-18 14:34:08.869677 cornifer-0.6/setup.cfg
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     1897 2022-09-27 16:45:39.000000 cornifer-0.6/setup.py
+drwxrwxrwx   0 automorphis  (1000) automorphis  (1000)        0 2023-05-18 14:34:08.791114 cornifer-0.6/tests/
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     9632 2023-05-12 15:41:02.000000 cornifer-0.6/tests/test_blocks.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)    11191 2023-05-12 15:41:02.000000 cornifer-0.6/tests/test_info.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)     2165 2023-05-10 17:07:48.000000 cornifer-0.6/tests/test_register_file_structure.py
+-rwxrwxrwx   0 automorphis  (1000) automorphis  (1000)   135725 2023-05-17 17:41:23.000000 cornifer-0.6/tests/test_registers.py
```

### Comparing `cornifer-0.5.1/LICENSE` & `cornifer-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cornifer-0.5.1/README.md` & `cornifer-0.6/README.md`

 * *Files identical despite different names*

### Comparing `cornifer-0.5.1/lib/Cornifer.egg-info/SOURCES.txt` & `cornifer-0.6/lib/Cornifer.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -20,8 +20,12 @@
 lib/cornifer.egg-info/PKG-INFO
 lib/cornifer.egg-info/SOURCES.txt
 lib/cornifer.egg-info/dependency_links.txt
 lib/cornifer.egg-info/not-zip-safe
 lib/cornifer.egg-info/requires.txt
 lib/cornifer.egg-info/top_level.txt
 lib/cornifer/_utilities/__init__.py
-lib/cornifer/_utilities/lmdb.py
+lib/cornifer/_utilities/lmdb.py
+tests/test_blocks.py
+tests/test_info.py
+tests/test_register_file_structure.py
+tests/test_registers.py
```

### Comparing `cornifer-0.5.1/lib/cornifer/__init__.py` & `cornifer-0.6/lib/cornifer/__init__.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.5.1/lib/cornifer/_utilities/lmdb.py` & `cornifer-0.6/lib/cornifer/_utilities/lmdb.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """
 
 from contextlib import contextmanager
 from pathlib import Path
 
 import lmdb
 
-from .._utilities import isInt
+from .._utilities import is_int
 
 class ReversibleTransaction:
 
     def __init__(self, db):
 
         self.db = db
         self.txn = None
@@ -81,15 +81,15 @@
     def delete(self, key):
 
         if key not in self.undo.keys():
             self.undo[key] = self.txn.get(key, default = None)
 
         self.txn.delete(key)
 
-def lmdbIsClosed(db):
+def lmdb_is_closed(db):
 
     try:
         with db.begin() as _:
             pass
 
     except BaseException as e:
 
@@ -98,20 +98,20 @@
 
         else:
             raise e
 
     else:
         return False
 
-def openLmdb(filepath, mapSize, readonly):
+def open_lmdb(filepath, mapSize, readonly):
 
     if not isinstance(filepath, Path):
         raise TypeError("`filepath` must be of type `pathlib.Path`.")
 
-    if not isInt(mapSize):
+    if not is_int(mapSize):
         raise TypeError("`map_size` must be of type `int`.")
     else:
         mapSize = int(mapSize)
 
     if not isinstance(readonly, bool):
         raise TypeError("`readonly` must be of type `bool`.")
 
@@ -125,75 +125,78 @@
         str(filepath),
         map_size = mapSize,
         subdir = True,
         readonly = readonly,
         create = False
     )
 
-def lmdbHasKey(dbOrTxn, key):
+def lmdb_has_key(db_or_txn, key):
     """
-    :param dbOrTxn: If type `lmdb_cornifer.Environment`, open a new read-only transaction and close it after this function
+    :param db_or_txn: If type `lmdb_cornifer.Environment`, open a new read-only transaction and close it after this function
     resolves. If type `lmdb_cornifer.Transaction`, do not close it after the function resolves.
     :param key: (type `bytes`)
     :return: (type `bool`)
     """
 
-    with _resolveDbOrTxn(dbOrTxn) as txn:
+    with _resolve_db_or_txn(db_or_txn) as txn:
         return txn.get(key, default = None) is not None
 
-def lmdbPrefixList(dbOrTxn, prefix):
+def lmdb_prefix_list(db_or_txn, prefix):
 
-    with lmdbPrefixIter(dbOrTxn, prefix) as it:
+    with lmdb_prefix_iter(db_or_txn, prefix) as it:
         return [t for t in it]
 
 @contextmanager
-def lmdbPrefixIter(dbOrTxn, prefix):
+def lmdb_prefix_iter(db_or_txn, prefix):
     """Iterate over all key-value pairs where they key begins with given prefix.
 
-    :param dbOrTxn: If type `lmdb_cornifer.Environment`, open a new read-only transaction and close it after this function
+    :param db_or_txn: If type `lmdb_cornifer.Environment`, open a new read-only transaction and close it after this function
     resolves. If type `lmdb_cornifer.Transaction`, do not close it after the function resolves.
     :param prefix: (type `bytes`)
     :return: (type `_LMDB_Prefix_Iterator`)
     """
 
-    with _resolveDbOrTxn(dbOrTxn) as txn:
+    with _resolve_db_or_txn(db_or_txn) as txn:
 
         it = _LmdbPrefixIter(txn, prefix)
 
         try:
             yield it
 
         finally:
             it.cursor.close()
 
-def lmdbCountKeys(dbOrTxn, prefix):
+def lmdb_count_keys(db_or_txn, prefix):
 
     count = 0
 
-    with lmdbPrefixIter(dbOrTxn, prefix) as it:
+    with lmdb_prefix_iter(db_or_txn, prefix) as it:
 
          for _ in it:
             count += 1
 
     return count
 
+def is_transaction(txn):
+    return isinstance(txn, (lmdb.Transaction, ReversibleTransaction))
+
 @contextmanager
-def _resolveDbOrTxn(dbOrTxn):
+def _resolve_db_or_txn(db_or_txn):
 
-    if isinstance(dbOrTxn, lmdb.Environment):
+    if isinstance(db_or_txn, lmdb.Environment):
 
-        if lmdbIsClosed(dbOrTxn):
+        if lmdb_is_closed(db_or_txn):
             raise lmdb.Error("Environment should not be closed.")
 
-        txn = dbOrTxn.begin()
+        txn = db_or_txn.begin()
         abort = True
 
-    elif isinstance(dbOrTxn, (lmdb.Transaction, ReversibleTransaction)):
+    elif is_transaction(db_or_txn):
 
-        txn = dbOrTxn
+        txn = db_or_txn
         abort = False
 
     else:
         raise TypeError
 
     try:
         yield txn
```

### Comparing `cornifer-0.5.1/lib/cornifer/blocks.py` & `cornifer-0.6/lib/cornifer/blocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 import sys
 import warnings
 from abc import ABC, abstractmethod
 
 import numpy as np
 
 from .info import ApriInfo
-from ._utilities import checkHasMethod, justifySlice, isInt
+from ._utilities import check_has_method, justify_slice, is_int
 
 
 class Block:
 
     def __init__(self, segment, apri, startn = 0):
 
         if not isinstance(apri, ApriInfo):
-            raise TypeError("`apri` must be of type `ApriInfo`.")
+            raise TypeError("`info` must be of type `ApriInfo`.")
 
-        if not isInt(startn):
+        if not is_int(startn):
             raise TypeError("`startn_` must be of type `int`.")
 
         else:
             startn = int(startn)
 
         if startn < 0:
             raise ValueError("`startn_` must be non-negative.")
@@ -42,15 +42,15 @@
 
         if isinstance(segment, list):
             self._dtype = "list"
 
         elif isinstance(segment, np.ndarray):
             self._dtype = "ndarray"
 
-        elif not checkHasMethod(segment, "__len__"):
+        elif not check_has_method(segment, "__len__"):
             raise ValueError(
                 f"`len(segment)` must be defined. Please define the method `__len__` for the type " +
                 f"`{segment.__class__.__name__}`."
             )
 
         else:
 
@@ -58,31 +58,31 @@
             self._custom_dtype = True
 
         self._startn = startn
         self._apri = apri
         self._seg = segment
         self._seg_ndarray = None
 
-    def _check_and_warn_custom_get_ndarray(self, methodName):
+    def _check_and_warn_custom_get_ndarray(self, method_name):
 
-        if self._custom_dtype and not self._seg_ndarray and not checkHasMethod(self._seg, methodName):
+        if self._custom_dtype and not self._seg_ndarray and not check_has_method(self._seg, method_name):
 
             try:
                 self._seg_ndarray = self._seg.get_ndarray()
 
             except NameError:
                 raise NotImplementedError(
-                    f"If you have not implemented `{methodName}` for the type" +
+                    f"If you have not implemented `{method_name}` for the type" +
                     f" `{self._seg.__class__.__name__}`, then you must implement the method " +
                     f"`get_ndarray()` for the type `{self._seg.__class__.__name__}`."
                 )
 
             warnings.warn(
                 f"The custom type `{self._seg.__class__.__name__}` has not defined the method" +
-                f" `{methodName}`. Cornifer is calling the method `get_ndarray`, which may slow down the " +
+                f" `{method_name}`. Cornifer is calling the method `get_ndarray`, which may slow down the " +
                 f"program or lead to unexpected behavior."
             )
 
             return False
 
         else:
             return True
@@ -92,55 +92,55 @@
 
     def apri(self):
         return self._apri
 
     def startn(self):
         return self._startn
 
-    def setStartn(self, startn):
+    def set_startn(self, startn):
 
-        if not isInt(startn):
-            raise TypeError("`startn_` must be of type `int`")
+        if not is_int(startn):
+            raise TypeError("`startn` must be of type `int`")
         else:
             startn = int(startn)
 
         if startn < 0:
-            raise ValueError("`startn_` must be positive")
+            raise ValueError("`startn` must be positive")
 
         self._startn = startn
 
-    def subdivide(self, subintervalLen):
+    def subdivide(self, subinterval_len):
 
-        if not isInt(subintervalLen):
-            raise TypeError("`subintervalLen` must be an integer")
+        if not is_int(subinterval_len):
+            raise TypeError("`subinterval_len` must be an integer")
         else:
-            subintervalLen = int(subintervalLen)
+            subinterval_len = int(subinterval_len)
 
-        if subintervalLen <= 1:
-            raise ValueError("`subintervalLen` must be at least 2")
+        if subinterval_len <= 1:
+            raise ValueError("`subinterval_len` must be at least 2")
 
         startn = self.startn()
         return [
-            self[i : i + subintervalLen]
-            for i in range(startn, startn + len(self), subintervalLen)
+            self[i : i + subinterval_len]
+            for i in range(startn, startn + len(self), subinterval_len)
         ]
 
     def __getitem__(self, item):
 
         if isinstance(item, tuple):
             raise IndexError(
                 "`blk[]` cannot take more than one index."
             )
 
         elif isinstance(item, slice):
 
             apri = self.apri()
             startn = self.startn()
             length = len(self)
-            item = justifySlice(item, startn, startn + length - 1)
+            item = justify_slice(item, startn, startn + length - 1)
 
             if not self._check_and_warn_custom_get_ndarray("__getitem__"):
                 return Block(self._seg_ndarray[item, ...], apri, startn)
 
             elif self._dtype == "ndarray":
                 return Block(self._seg[item, ...], apri, startn)
 
@@ -177,15 +177,15 @@
     def __contains__(self, n):
         startn = self.startn()
         return startn <= n < startn + len(self)
 
     def __hash__(self):
         raise TypeError(
             f"The type `{self.__class__.__name__}` is not hashable. Please instead hash " +
-            f"`(blk.apri(), blk.startn_(), len(blk))`."
+            f"`(blk.info(), blk.startn_(), len(blk))`."
         )
 
     def __str__(self):
         ret = self.__class__.__name__ + "("
         ret += f"<{self._dtype}>:{len(self)}, "
         ret += repr(self._apri) + ", "
         ret += str(self._startn) + ")"
@@ -242,15 +242,15 @@
                 raise RuntimeError("Couldn't close the `memmap` handle.")
 
             del self._seg
 
         except AttributeError:
             pass
 
-    def changeMode(self, mode):
+    def change_mode(self, mode):
 
         if not isinstance(mode, str):
             raise TypeError("`mode` must be a string.")
 
         filename = self._seg.filename
         self._seg.flush()
         self.release()
```

### Comparing `cornifer-0.5.1/lib/cornifer/errors.py` & `cornifer-0.6/lib/cornifer/errors.py`

 * *Files identical despite different names*

### Comparing `cornifer-0.5.1/lib/cornifer/example.py` & `cornifer-0.6/lib/cornifer/example.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from math import floor, sqrt
 from pathlib import Path
 
-from cornifer import ApriInfo, NumpyRegister, Block
+from cornifer import NumpyRegister, Block
+from cornifer.info import ApriInfo
 
 my_saves_dir = Path.home() / "my_cornifer_saves"
 
 def is_prime(m):
 
     if not isinstance(m, int) or m <= 1:
         return False
@@ -14,24 +15,24 @@
             return False
     return True
 
 lst = []
 descr = ApriInfo(name ="primes")
 blk = Block(lst, descr, 1)
 register = NumpyRegister(my_saves_dir, "primes example")
-register.addRamBlk(blk)
+register.add_ram_blk(blk)
 
 length = 100000
 total_primes = 0
 max_m = 10**9
 
 with register.open() as register:
 
     for m in range(2, max_m+1):
         if is_prime(m):
             total_primes += 1
             lst.append(m)
 
         if (total_primes % length == 0 and total_primes > 0) or m == max_m:
-            register.addDiskBlk(blk)
+            register.add_disk_blk(blk)
             blk.setStartN(total_primes + 1)
             lst.clear()
```

### Comparing `cornifer-0.5.1/lib/cornifer/filemetadata.py` & `cornifer-0.6/lib/cornifer/filemetadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.size = size
         self.size_GB = self.size // BYTES_PER_GB
         self.size_MB = (self.size % BYTES_PER_GB) // BYTES_PER_MB
         self.size_KB = (self.size % BYTES_PER_MB) // BYTES_PER_KB
         self.size_B  = self.size % BYTES_PER_KB
 
     @staticmethod
-    def fromPath(path):
+    def from_path(path):
 
         stat = path.stat()
 
         if platform.system() == 'Windows':
             created = stat.st_ctime
 
         else:
```

### Comparing `cornifer-0.5.1/lib/cornifer/info.py` & `cornifer-0.6/lib/cornifer/info.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,103 @@
-"""
-    Cornifer, an intuitive data manager for empirical and computational mathematics.
-    Copyright (C) 2021 Michael P. Lane
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-"""
-
-
 import json
 from abc import ABC, abstractmethod
 from copy import copy, deepcopy
 
-from ._utilities import orderJsonObj, isInt
+from ._utilities import is_int, order_json_obj
+
+_APRI_ENCODED_PREFIX = "ApriInfo.from_json("
+_APRI_ENCODED_SUFFIX = ")"
+_APRI_ENCODED_PREFIX_LEN = len(_APRI_ENCODED_PREFIX)
+_APRI_ENCODED_SUFFIX_LEN = len(_APRI_ENCODED_SUFFIX)
+_APRI_ENCODED_PRE_SUFFIX_LEN = _APRI_ENCODED_PREFIX_LEN + _APRI_ENCODED_SUFFIX_LEN
+_APOS_ENCODED_PREFIX = "AposInfo.from_json("
+_APOS_ENCODED_SUFFIX = ")"
+_APOS_ENCODED_PREFIX_LEN = len(_APOS_ENCODED_PREFIX)
+_APOS_ENCODED_SUFFIX_LEN = len(_APOS_ENCODED_SUFFIX)
+_APOS_ENCODED_PRE_SUFFIX_LEN = _APOS_ENCODED_PREFIX_LEN + _APOS_ENCODED_SUFFIX_LEN
+
+
+class JSONDecoderWithRoot(json.JSONDecoder, ABC):
+
+    @abstractmethod
+    def decode_root(self, obj):pass
+
 
 class _InfoJsonEncoder(json.JSONEncoder):
 
     def default(self, obj):
 
-        if isinstance(obj, _Info):
-            return obj.__class__.__name__ + ".fromJson(" + obj.toJson() + ")"
+        if isinstance(obj, ApriInfo):
+            return _APRI_ENCODED_PREFIX + obj.to_json() + _APRI_ENCODED_SUFFIX
+
+        elif isinstance(obj, AposInfo):
+            return _APOS_ENCODED_PREFIX + obj.to_json() + _APOS_ENCODED_SUFFIX
 
-        elif isInt(obj):
+        elif is_int(obj):
             return int(obj)
 
         elif isinstance(obj, tuple):
             return list(obj)
 
         else:
             return super().default(obj)
 
-class _InfoJsonDecoder(json.JSONDecoder):
+
+class _InfoJsonDecoder(JSONDecoderWithRoot):
 
     def __init__(self, *args, **kwargs):
         super().__init__(object_hook=self.object_hook, *args, **kwargs)
 
+    @staticmethod
+    def check_return_apri_info_json(str_):
+
+        check = (
+            len(str_) > _APRI_ENCODED_PRE_SUFFIX_LEN and
+            str_[ : _APRI_ENCODED_PREFIX_LEN] == _APRI_ENCODED_PREFIX and
+            str_[-_APRI_ENCODED_SUFFIX_LEN : ] == _APRI_ENCODED_SUFFIX
+        )
+        return (
+            check,
+            str_[_APRI_ENCODED_PREFIX_LEN : -_APRI_ENCODED_SUFFIX_LEN].strip(" \t") if check else None
+        )
+
+    @staticmethod
+    def check_return_apos_info_json(str_):
+
+        check = (
+            len(str_) > _APOS_ENCODED_PRE_SUFFIX_LEN and
+            str_[ : _APOS_ENCODED_PREFIX_LEN] == _APOS_ENCODED_PREFIX and
+            str_[-_APOS_ENCODED_SUFFIX_LEN : ] == _APOS_ENCODED_SUFFIX
+        )
+        return (
+            check,
+            str_[_APOS_ENCODED_PREFIX_LEN : -_APOS_ENCODED_SUFFIX_LEN].strip(" \t") if check else None
+        )
+
     def object_hook(self, obj):
 
         if isinstance(obj, str):
 
             obj = obj.strip(" \t")
-            if (obj[:8] == "ApriInfo" or obj[:8] == "AposInfo") and obj[8:18] == ".fromJson(" and obj[-1] == ")":
 
-                json_str = obj[18:-1].strip(" \t")
+            check_apri, apri_json = _InfoJsonDecoder.check_return_apri_info_json(obj)
+            check_apos, apos_json = _InfoJsonDecoder.check_return_apos_info_json(obj)
+
+            if check_apri:
 
                 try:
+                    return ApriInfo(**self.decode(apri_json))
+
+                except json.JSONDecodeError:
+                    return obj
 
-                    if obj[:8] == "ApriInfo":
-                        return ApriInfo.fromJson(json_str)
+            elif check_apos:
 
-                    else:
-                        return AposInfo.fromJson(json_str)
+                try:
+                    return AposInfo(**self.decode(apos_json))
 
                 except json.JSONDecodeError:
                     return obj
 
             else:
                 return obj
 
@@ -69,179 +106,246 @@
 
         elif isinstance(obj, list):
             return tuple([self.object_hook(item) for item in obj])
 
         else:
             return obj
 
+    def decode_root(self, obj):
+
+        try:
+            decoded_json = self.decode(obj)
+
+        except:
+            raise
+
+        if not isinstance(decoded_json, dict):
+            raise ValueError(
+                "The outermost layer of the passed JSON string must be a JavaScript `object`, that is, " +
+                f"a Python `dict`. The outermost layer of the passed `json_string` is: " +
+                f"`{decoded_json.__class__.__name__}`."
+            )
+
+        return decoded_json
+
+
 class _Info(ABC):
 
-    _reservedKws = ["_json", "_str"]
+    _reserved_kws = ["_memoize_json", "_str", "_json", "_encoder"]
+    _default_encoder = _InfoJsonEncoder(
+        ensure_ascii = True,
+        allow_nan = True,
+        indent = None,
+        separators = (',', ':')
+    )
+    _default_decoder = _InfoJsonDecoder()
+
+    def __init_subclass__(cls, reserved_kws = None, **kwargs):
+
+        super().__init_subclass__(**kwargs)
+
+        if reserved_kws is None:
+            cls._reserved_kws = _Info._reserved_kws
+
+        else:
+            cls._reserved_kws = _Info._reserved_kws + reserved_kws
 
     def __init__(self, **kwargs):
 
         if len(kwargs) == 0:
             raise ValueError("must pass at least one keyword argument.")
 
-        type(self)._checkReservedKws(kwargs)
-
+        type(self)._check_reserved_kws(kwargs)
         self.__dict__.update(kwargs)
-
         self._json = None
-
         self._str = None
+        self._memoize_json = False
+        self._encoder = _Info._default_encoder
 
     @classmethod
-    def _checkReservedKws(cls, kwargs):
+    def _check_reserved_kws(cls, kwargs):
 
-        if any(kw in kwargs for kw in cls._reservedKws):
+        if any(kw in kwargs for kw in cls._reserved_kws):
 
             raise ValueError(
-
                 "The following keyword-argument keys are reserved. Choose a different key.\n" +
-                f"{', '.join(cls._reservedKws)}"
+                f"{', '.join(cls._reserved_kws)}"
             )
 
     @classmethod
-    def fromJson(cls, jsonStr):
+    def from_json(cls, json_str, decoder = None):
 
-        decoded_json = _InfoJsonDecoder().decode(jsonStr)
+        if decoder is None:
+            decoder = cls._default_decoder
 
-        if not isinstance(decoded_json, dict):
-            raise ValueError(
-                "The outermost layer of the passed `json_string` must be a JavaScript `object`, that is, " +
-                f"a Python `dict`. The outermost layer of the passed `json_string` is: " +
-                f"`{decoded_json.__class__.__name__}`."
-            )
+        if not isinstance(decoder, JSONDecoderWithRoot):
+            raise TypeError("`decoder` must subclass `JSONDecoderWithRoot`.")
 
-        return cls(**decoded_json)
+        decoded = decoder.decode_root(json_str)
+        return cls(**decoded)
 
-    def toJson(self):
+    def to_json(self):
 
-        if self._json is not None:
+        if self._memoize_json and self._json is not None:
             return self._json
 
         else:
 
             kwargs = copy(self.__dict__)
 
-            for kw in type(self)._reservedKws:
+            for kw in type(self)._reserved_kws:
                 kwargs.pop(kw,None)
 
-            kwargs = orderJsonObj(kwargs)
+            kwargs = order_json_obj(kwargs)
 
             try:
-                json_rep = _InfoJsonEncoder(
-
-                    ensure_ascii = True,
-                    allow_nan = True,
-                    indent = None,
-                    separators = (',', ':')
-
-                ).encode(kwargs)
+                json_rep = self._encoder.encode(kwargs)
 
             except (TypeError, ValueError) as e:
 
                 raise ValueError(
                     "One of the keyword arguments used to construct this instance cannot be encoded into " +
                     "JSON. Use different keyword arguments, or override the " +
-                    f"classmethod `{self.__class__.__name__}.fromJson` and the instancemethod " +
+                    f"classmethod `{self.__class__.__name__}.from_json` and the instancemethod " +
                     f"`{self.__class__.__name__}.toJson`."
                 ) from e
 
             if "\0" in json_rep:
 
                 raise ValueError(
                     "One of the keyword arguments used to construct this instance contains the null character " +
                     "'\\0'."
                 )
 
-            self._json = json_rep
+            if self._memoize_json:
+                self._json = json_rep
 
             return json_rep
 
-    def iterInnerInfo(self, _rootCall = True):
+    def _iter_inner_info_bfs(self, root_call):
 
-        if not isinstance(_rootCall, bool):
-            raise TypeError("`_rootCall` must be of type `bool`.")
-
-        if _rootCall:
+        if root_call:
             yield None, self
 
+        subinfos = []
+
         for key, val in self.__dict__.items():
 
-            if key not in type(self)._reservedKws and isinstance(val, _Info):
+            if key not in type(self)._reserved_kws and isinstance(val, _Info):
 
+                subinfos.append((key, val))
                 yield key, val
 
-                for inner in val.iterInnerInfo(_rootCall= False):
-                    yield inner
+        for key, val in subinfos:
+            yield from val._iter_inner_info_bfs(False)
+
+    def _iter_inner_info_dfs(self, root_call):
+
+        for key, val in self.__dict__.items():
+
+            if key not in type(self)._reserved_kws and isinstance(val, _Info):
+
+                yield from val._iter_inner_info_dfs(False)
+                yield key, val
+
+        if root_call:
+            yield None, self
+
+    def iter_inner_info(self, mode = "dfs"):
+        """Iterate over `_Info` contained within this `_Info`.
+
+        :param mode: (type `str`) Optional, default "dfs". Whether to return depth- (dfs) or breadth-first (bfs).
+        :return: (type `str`) Keyword names, or `None` for the root.
+        :return: (type `_Info`) Keyword values, `self` for the root.
+        """
+
+        if not isinstance(mode, str):
+            raise TypeError("`mode` must be of type `str`.")
 
-    def changeInfo(self, oldInfo, newInfo, _rootCall = True):
+        if mode != "dfs" and mode != "bfs":
+            raise ValueError("`mode` must be either 'dfs' or 'bfs'.")
+
+        if mode == "dfs":
+            yield from self._iter_inner_info_dfs(True)
+
+        else:
+            yield from self._iter_inner_info_bfs(True)
 
-        if not isinstance(oldInfo, _Info):
-            raise TypeError("`oldInfo` must be of type `_Info`.")
 
-        if not isinstance(newInfo, _Info):
-            raise TypeError("`newInfo` must be of type `_Info`.")
 
-        if not isinstance(_rootCall, bool):
+
+    def change_info(self, old_info, new_info, _root_call = True):
+
+        if not isinstance(old_info, _Info):
+            raise TypeError("`old_info` must be of type `_Info`.")
+
+        if not isinstance(new_info, _Info):
+            raise TypeError("`new_info` must be of type `_Info`.")
+
+        if not isinstance(_root_call, bool):
             raise TypeError("`_rootCall` must be of type `bool`.")
 
-        if _rootCall:
+        if _root_call:
             replaced_info = deepcopy(self)
 
         else:
             replaced_info = self
 
-        if self == oldInfo:
-            return newInfo
+        if self == old_info:
+            return new_info
 
         else:
 
             kw = {}
 
             for key, val in replaced_info.__dict__.items():
 
-                if key not in type(self)._reservedKws:
+                if key not in type(self)._reserved_kws:
 
-                    if val == oldInfo:
-                        kw[key] = newInfo
+                    if val == old_info:
+                        kw[key] = new_info
 
                     elif isinstance(val, _Info):
-                        kw[key] = val.changeInfo(oldInfo, newInfo)
+                        kw[key] = val.change_info(old_info, new_info)
 
                     else:
                         kw[key] = val
 
             return type(self)(**kw)
 
+    def set_encoder(self, encoder):
+
+        if not isinstance(encoder, json.JSONEncoder):
+            raise TypeError("`encoder` must be of type `json.JSONEncoder`.")
+
+        self._encoder = encoder
+
     def __iter__(self):
 
         for key, val in self.__dict__.items():
 
-            if key not in type(self)._reservedKws:
+            if key not in type(self)._reserved_kws:
                 yield key, val
 
     def __contains__(self, apri):
 
         if not isinstance(apri, ApriInfo):
-            raise TypeError("`apri` must be of type `ApriInfo`.")
+            raise TypeError("`info` must be of type `ApriInfo`.")
 
-        return any(inner == apri for _, inner in self.iterInnerInfo())
+        return any(inner == apri for _, inner in self.iter_inner_info())
 
     def __lt__(self, other):
 
         if type(self) != type(other):
             return False
 
         else:
 
-            self_kwargs = sorted([key for key in self.__dict__.keys() if key not in type(self)._reservedKws])
-            other_kwargs = sorted([key for key in other.__dict__.keys() if key not in type(other)._reservedKws])
+            self_kwargs = sorted([key for key in self.__dict__.keys() if key not in type(self)._reserved_kws])
+            other_kwargs = sorted([key for key in other.__dict__.keys() if key not in type(other)._reserved_kws])
 
             for self_kw, other_kw in zip(self_kwargs, other_kwargs):
 
                 if self_kw != other_kw:
                     return self_kw < other_kw
 
             else:
@@ -267,68 +371,98 @@
         else:
             return not(self < other)
 
     @abstractmethod
     def __hash__(self):pass
 
     def __eq__(self, other):
-        return type(self) == type(other) and self.toJson() == other.toJson()
+
+        if type(self) != type(other):
+            return False
+
+        if (
+            self._memoize_json and other._memoize_json and
+            self._json is not None and other._json is not None
+        ):
+            return self._json == other._json
+
+        if len(self.__dict__) != len(other.__dict__):
+            return False
+
+        for key, val in self.__dict__.items():
+
+            if key not in type(self)._reserved_kws:
+
+                if key not in other.__dict__.keys():
+                    return False
+
+                elif val != other.__dict__[key]:
+                    return False
+
+        else:
+            return True
 
     def __str__(self):
 
         if self._str is not None:
             return self._str
 
         else:
 
             ret = f"{self.__class__.__name__}("
             ordered = sorted(
-                [(key, val) for key, val in self.__dict__.items() if key not in type(self)._reservedKws],
+                [(key, val) for key, val in self.__dict__.items() if key not in type(self)._reserved_kws],
                 key = lambda t: t[0]
             )
             ret += ", ".join(f"{key}={repr(val)}" for key, val in ordered)
             ret += ")"
+
             self._str = ret
+
             return self._str
 
     def __repr__(self):
         return str(self)
 
     def __copy__(self):
         info = type(self)(placeholder = "placeholder")
         del info.placeholder
         info.__dict__.update(self.__dict__)
         return info
 
     def __deepcopy__(self, memo):
         return self.__copy__()
 
-class ApriInfo(_Info):
 
-    _reservedKws = ["_json", "_hash", "_str"]
+class ApriInfo(_Info, reserved_kws = ["_hash"]):
 
     def __init__(self, **kwargs):
 
         super().__init__(**kwargs)
-
-        self._hash = hash(type(self))
+        hash_ = hash(type(self))
+        self._memoize_json = True
 
         for key,val in kwargs.items():
 
             try:
-                self._hash += hash(val)
+                hash_ += hash(val)
 
             except (TypeError, AttributeError):
 
                 raise ValueError(
                     f"All keyword arguments must be hashable types. The keyword argument given by \"{key}\" "+
                     f"not a hashable type. The type of that argument is `{val.__class__.__name__}`."
                 )
 
+            if self._memoize_json and isinstance(val, _Info):
+                self._memoize_json = False
+
+        self._hash = hash_
+
     def __hash__(self):
         return self._hash
 
+
 class AposInfo(_Info):
 
     def __hash__(self):
-        raise TypeError("`Apos_Info` is not a hashable type.")
-
+        raise TypeError("`Apos_Info` is not a hashable type.")
```

### Comparing `cornifer-0.5.1/lib/cornifer/regfilestructure.py` & `cornifer-0.6/lib/cornifer/regfilestructure.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,34 +23,34 @@
 DATABASE_FILEPATH      = f"{REG_FILENAME}/database"
 MAP_SIZE_FILEPATH      = f"{REG_FILENAME}/mapsize.txt"
 
 LOCAL_DIR_CHARS        = BASE52
 COMPRESSED_FILE_SUFFIX = ".zip"
 
 
-def checkRegStructure(localDir):
+def check_reg_structure(local_dir):
     """
-    :param localDir: (type `pathlib.Path`) Absolute.
+    :param local_dir: (type `pathlib.Path`) Absolute.
     :raise FileNotFoundError
     """
 
-    if not localDir.is_absolute():
-        raise ValueError(NOT_ABSOLUTE_ERROR_MESSAGE.format(str(localDir)))
+    if not local_dir.is_absolute():
+        raise ValueError(NOT_ABSOLUTE_ERROR_MESSAGE.format(str(local_dir)))
 
     problems = []
 
-    if not localDir.is_dir():
-        problems.append(str(localDir))
+    if not local_dir.is_dir():
+        problems.append(str(local_dir))
 
     for path in [VERSION_FILEPATH, MSG_FILEPATH, CLS_FILEPATH, MAP_SIZE_FILEPATH]:
-        if not (localDir / path).is_file():
-            problems.append(str(localDir / path))
+        if not (local_dir / path).is_file():
+            problems.append(str(local_dir / path))
 
     for path in [DATABASE_FILEPATH]:
-        if not (localDir / path).is_dir():
-            problems.append(str(localDir / path))
+        if not (local_dir / path).is_dir():
+            problems.append(str(local_dir / path))
 
     if len(problems) > 0:
         raise FileNotFoundError(
             "Could not find the following files or directories: " +
             ", ".join(problems)
         )
```

### Comparing `cornifer-0.5.1/lib/cornifer/registers.py` & `cornifer-0.6/lib/cornifer/registers.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,30 +16,31 @@
 import inspect
 import math
 import pickle
 import shutil
 import warnings
 import zipfile
 from contextlib import contextmanager, ExitStack
+from itertools import count
 from pathlib import Path
 from abc import ABC, abstractmethod
 
 import lmdb
 import numpy as np
 
 from .errors import DataNotFoundError, RegisterAlreadyOpenError, RegisterError, CompressionError, \
     DecompressionError, NOT_ABSOLUTE_ERROR_MESSAGE, RegisterRecoveryError
-from .info import ApriInfo, AposInfo
+from .info import ApriInfo, AposInfo, _InfoJsonEncoder, _InfoJsonDecoder, _Info
 from .blocks import Block, MemmapBlock, ReleaseBlock
 from .filemetadata import FileMetadata
-from ._utilities import randomUniqueFilename, isInt, resolvePath, BYTES_PER_MB, isDeletable
-from ._utilities.lmdb import lmdbHasKey, lmdbPrefixIter, openLmdb, lmdbIsClosed, lmdbCountKeys, \
-    ReversibleTransaction
+from ._utilities import random_unique_filename, is_int, resolve_path, BYTES_PER_MB, is_deletable
+from ._utilities.lmdb import lmdb_has_key, lmdb_prefix_iter, open_lmdb, lmdb_is_closed, lmdb_count_keys, \
+    ReversibleTransaction, is_transaction, lmdb_prefix_list
 from .regfilestructure import VERSION_FILEPATH, LOCAL_DIR_CHARS, \
-    COMPRESSED_FILE_SUFFIX, MSG_FILEPATH, CLS_FILEPATH, checkRegStructure, DATABASE_FILEPATH, \
+    COMPRESSED_FILE_SUFFIX, MSG_FILEPATH, CLS_FILEPATH, check_reg_structure, DATABASE_FILEPATH, \
     REG_FILENAME, MAP_SIZE_FILEPATH
 from .version import CURRENT_VERSION, COMPATIBLE_VERSIONS
 
 _NO_DEBUG = 0
 _debug = _NO_DEBUG
 
 #################################
@@ -48,15 +49,15 @@
 _KEY_SEP                   = b"\x00\x00"
 _START_N_HEAD_KEY          = b"head"
 _START_N_TAIL_LENGTH_KEY   = b"tail_length"
 _CLS_KEY                   = b"cls"
 _MSG_KEY                   = b"msg"
 _SUB_KEY_PREFIX            = b"sub"
 _BLK_KEY_PREFIX            = b"blk"
-_APRI_ID_KEY_PREFIX        = b"apri"
+_APRI_ID_KEY_PREFIX        = b"info"
 _ID_APRI_KEY_PREFIX        = b"id"
 _CURR_ID_KEY               = b"curr_id"
 _APOS_KEY_PREFIX           = b"apos"
 _COMPRESSED_KEY_PREFIX     = b"compr"
 _LENGTH_LENGTH_KEY         = b"lenlen"
 
 _KEY_SEP_LEN               = len(_KEY_SEP)
@@ -70,15 +71,15 @@
 _IS_NOT_COMPRESSED_VAL     = b""
 
 _SUB_VAL                   = b""
 
 #################################
 #        ERROR MESSAGES         #
 
-def _blkNotFoundErrMsg(diskonly, apri, n = None, startn = None, length = None):
+def _blk_not_found_err_msg(diskonly, apri, n = None, startn = None, length = None):
 
     if (startn is not None or length is not None) and n is not None:
         raise ValueError
 
     if startn is None and length is not None:
         raise ValueError
 
@@ -102,15 +103,15 @@
 
 _NOT_CREATED_ERROR_MESSAGE = (
     "The `Register` database has not been created. You must do `with reg.open() as reg:` at least once before " +
     "calling the method `{0}`."
 )
 
 _MEMORY_FULL_ERROR_MESSAGE = (
-    "Exceeded max `Register` size of {0} Bytes. Please increase the max size using the method `increaseRegSize`."
+    "Exceeded max `Register` size of {0} Bytes. Please increase the max size using the method `increase_reg_size`."
 )
 
 _REG_ALREADY_ADDED_ERROR_MESSAGE = "Already added as subregister."
 
 _NO_APRI_ERROR_MESSAGE = "The following `ApriInfo` is not known to this `Register` : {0}"
 
 #################################
@@ -123,81 +124,81 @@
 _INITIAL_REGISTER_SIZE_DEFAULT = 5 * BYTES_PER_MB
 
 class Register(ABC):
 
     #################################
     #     PUBLIC INITIALIZATION     #
 
-    def __init__(self, savesDir, msg, initialRegSize = None):
+    def __init__(self, saves_dir, msg, initial_reg_size = None):
         """
-        :param savesDir: (type `str`)
+        :param saves_dir: (type `str`)
         :param msg: (type `str`) A brief message describing this `Register`.
-        :param initialRegSize: (type `int`, default 5) Size in bytes. You may wish to set this lower
+        :param initial_reg_size: (type `int`, default 5) Size in bytes. You may wish to set this lower
         than 5 MB if you do not expect to add many disk `Block`s to your register and you are concerned about disk
         memory. If your `Register` exceeds `initial_register_size`, then you can adjust the database size later via the
-        method `increaseRegSize`. If you are on a non-Windows system, there is no harm in setting this value
+        method `increase_reg_size`. If you are on a non-Windows system, there is no harm in setting this value
         to be very large (e.g. 1 TB).
         """
 
-        if not isinstance(savesDir, (str, Path)):
+        if not isinstance(saves_dir, (str, Path)):
             raise TypeError("`savesDir` must be a string or a `pathlib.Path`.")
 
         if not isinstance(msg, str):
             raise TypeError("`msg` must be a string.")
 
-        if initialRegSize is not None and not isInt(initialRegSize):
+        if initial_reg_size is not None and not is_int(initial_reg_size):
             raise TypeError("`initialRegSize` must be of type `int`.")
 
-        elif initialRegSize is not None:
-            initialRegSize = int(initialRegSize)
+        elif initial_reg_size is not None:
+            initial_reg_size = int(initial_reg_size)
 
         else:
-            initialRegSize = _INITIAL_REGISTER_SIZE_DEFAULT
+            initial_reg_size = _INITIAL_REGISTER_SIZE_DEFAULT
 
-        if initialRegSize <= 0:
+        if initial_reg_size <= 0:
             raise ValueError("`initialRegSize` must be positive.")
 
-        self.savesDir = resolvePath(Path(savesDir))
+        self.saves_dir = resolve_path(Path(saves_dir))
 
-        if not self.savesDir.is_dir():
+        if not self.saves_dir.is_dir():
             raise FileNotFoundError(
-                f"You must create the file `{str(self.savesDir)}` before calling " +
-                f"`{self.__class__.__name__}(\"{str(self.savesDir)}\", \"{msg}\")`."
+                f"You must create the file `{str(self.saves_dir)}` before calling " +
+                f"`{self.__class__.__name__}(\"{str(self.saves_dir)}\", \"{msg}\")`."
             )
 
         self._msg = msg
-        self._msgFilepath = None
+        self._msg_filepath = None
 
-        self._localDir = None
-        self._localDirBytes = None
-        self._subregBytes = None
+        self._local_dir = None
+        self._local_dir_bytes = None
+        self._subreg_bytes = None
 
         self._db = None
-        self._dbFilepath = None
-        self._dbMapSize = initialRegSize
-        self._dbMapSizeFilepath = None
+        self._db_filepath = None
+        self._db_map_size = initial_reg_size
+        self._db_map_size_filepath = None
         self._readonly = None
 
         self._version = CURRENT_VERSION
-        self._versionFilepath = None
+        self._version_filepath = None
 
-        self._clsFilepath = None
+        self._cls_filepath = None
 
-        self._startnHead = _START_N_HEAD_DEFAULT
-        self._startnTailLength = _START_N_TAIL_LENGTH_DEFAULT
-        self._startnTailMod = 10 ** self._startnTailLength
-        self._lengthLength = _LENGTH_LENGTH_DEFAULT
-        self._maxLength = _MAX_LENGTH_DEFAULT
+        self._startn_head = _START_N_HEAD_DEFAULT
+        self._startn_tail_length = _START_N_TAIL_LENGTH_DEFAULT
+        self._startn_tail_mod = 10 ** self._startn_tail_length
+        self._length_length = _LENGTH_LENGTH_DEFAULT
+        self._max_length = _MAX_LENGTH_DEFAULT
 
-        self._ramBlks = {}
+        self._ram_blks = {}
 
         self._created = False
 
     @staticmethod
-    def addSubclass(subclass):
+    def add_subclass(subclass):
 
         if not inspect.isclass(subclass):
             raise TypeError(f"The `subclass` argument must be a class, not a {type(subclass)}.")
 
         if not issubclass(subclass, Register):
             raise TypeError(f"The class `{subclass.__name__}` must be a subclass of `Register`.")
 
@@ -207,38 +208,38 @@
     #     PROTEC INITIALIZATION     #
 
     _constructors = {}
 
     _instances = {}
 
     @staticmethod
-    def _fromLocalDir(localDir):
-        """Return a `Register` instance from a `localDir` with the correct concrete subclass.
+    def _from_local_dir(local_dir):
+        """Return a `Register` instance from a `local_dir` with the correct concrete subclass.
 
-        This static method does not open the `Register` database at any point.
+        This static method does not open the LMDB database at any point.
 
-        :param localDir: (type `pathlib.Path`) Absolute.
+        :param local_dir: (type `pathlib.Path`) Absolute.
         :return: (type `Register`)
         """
 
-        if not localDir.is_absolute():
-            raise ValueError(NOT_ABSOLUTE_ERROR_MESSAGE.format(str(localDir)))
+        if not local_dir.is_absolute():
+            raise ValueError(NOT_ABSOLUTE_ERROR_MESSAGE.format(str(local_dir)))
 
-        if not localDir.exists():
-            raise FileNotFoundError(f"The `Register` database `{str(localDir)}` could not be found.")
+        if not local_dir.exists():
+            raise FileNotFoundError(f"The `Register` database `{str(local_dir)}` could not be found.")
 
-        checkRegStructure(localDir)
+        check_reg_structure(local_dir)
 
-        if Register._instanceExists(localDir):
+        if Register._instance_exists(local_dir):
             # return the `Register` that has already been opened
-            return Register._getInstance(localDir)
+            return Register._get_instance(local_dir)
 
         else:
 
-            with (localDir / CLS_FILEPATH).open("r") as fh:
+            with (local_dir / CLS_FILEPATH).open("r") as fh:
                 cls_name = fh.readline().strip()
 
             if cls_name == "Register":
                 raise TypeError(
                     "`Register` is an abstract class, meaning that `Register` itself cannot be instantiated, " +
                     "only its concrete subclasses."
                 )
@@ -247,304 +248,314 @@
 
             if con is None:
                 raise TypeError(
                     f"`Register` is not aware of a subclass called `{cls_name}`. Please add the subclass to "+
                     f"`Register` via `Register.addSubclass({cls_name})`."
                 )
 
-            with (localDir / MSG_FILEPATH).open("r") as fh:
+            with (local_dir / MSG_FILEPATH).open("r") as fh:
                 msg = fh.read()
 
-            with (localDir / MAP_SIZE_FILEPATH).open("r") as fh:
+            with (local_dir / MAP_SIZE_FILEPATH).open("r") as fh:
                 mapSize = int(fh.readline().strip())
 
-            reg = con(localDir.parent, msg, mapSize)
-            reg._setLocalDir(localDir)
+            reg = con(local_dir.parent, msg, mapSize)
+            reg._set_local_dir(local_dir)
 
-            with (localDir / VERSION_FILEPATH).open("r") as fh:
+            with (local_dir / VERSION_FILEPATH).open("r") as fh:
                 reg._version = fh.readline().strip()
 
             return reg
 
     @staticmethod
-    def _addInstance(localDir, reg):
+    def _add_instance(local_dir, reg):
         """
-        :param localDir: (type `pathlib.Path`) Absolute.
+        :param local_dir: (type `pathlib.Path`) Absolute.
         :param reg: (type `Register`)
         """
 
-        if not localDir.is_absolute():
-            raise ValueError(NOT_ABSOLUTE_ERROR_MESSAGE.format(str(localDir)))
+        if not local_dir.is_absolute():
+            raise ValueError(NOT_ABSOLUTE_ERROR_MESSAGE.format(str(local_dir)))
 
-        Register._instances[localDir] = reg
+        Register._instances[local_dir] = reg
 
     @staticmethod
-    def _instanceExists(localDir):
+    def _instance_exists(local_dir):
         """
-        :param localDir: (type `pathlib.Path`) Absolute.
+        :param local_dir: (type `pathlib.Path`) Absolute.
         :return: (type `bool`)
         """
 
-        if not localDir.is_absolute():
-            raise ValueError(NOT_ABSOLUTE_ERROR_MESSAGE.format(str(localDir)))
+        if not local_dir.is_absolute():
+            raise ValueError(NOT_ABSOLUTE_ERROR_MESSAGE.format(str(local_dir)))
 
-        return localDir in Register._instances.keys()
+        return local_dir in Register._instances.keys()
 
     @staticmethod
-    def _getInstance(localDir):
+    def _get_instance(local_dir):
         """
-        :param localDir: (type `pathlib.Path`) Absolute.
+        :param local_dir: (type `pathlib.Path`) Absolute.
         :return: (type `Register`)
         """
 
-        if not localDir.is_absolute():
-            raise ValueError(NOT_ABSOLUTE_ERROR_MESSAGE.format(str(localDir)))
+        if not local_dir.is_absolute():
+            raise ValueError(NOT_ABSOLUTE_ERROR_MESSAGE.format(str(local_dir)))
 
-        return Register._instances[localDir]
+        return Register._instances[local_dir]
 
     #################################
     #    PUBLIC REGISTER METHODS    #
 
     def __eq__(self, other):
 
         if not self._created or not other._created:
             raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("__eq__"))
 
         elif type(self) != type(other):
             return False
 
         else:
-            return self._localDir == other._localDir
+            return self._local_dir == other._local_dir
 
     def __hash__(self):
 
         if not self._created:
             raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("__hash__"))
 
         else:
-            return hash(str(self._localDir)) + hash(type(self))
+            return hash(str(self._local_dir)) + hash(type(self))
 
     def __str__(self):
         return self._msg
 
     def __repr__(self):
-        return f"{self.__class__.__name__}(\"{str(self.savesDir)}\", \"{self._msg}\")"
+        return f"{self.__class__.__name__}(\"{str(self.saves_dir)}\", \"{self._msg}\")"
 
     def __contains__(self, apri):
 
-        self._checkOpenRaise("__contains__")
+        self._check_open_raise("__contains__")
 
-        if any(blk.apri() == apri for blk in self._ramBlks):
+        if any(blk.apri() == apri for blk in self._ram_blks):
             return True
 
         else:
-            return lmdbHasKey(self._db, _APRI_ID_KEY_PREFIX + apri.toJson().encode("ASCII"))
+
+            with self._db.begin() as txn:
+
+                try:
+                    apri_json = relational_encode_info(self, apri, txn)
+
+                except DataNotFoundError:
+                    return False
+
+                key = _APRI_ID_KEY_PREFIX + apri_json
+                return lmdb_has_key(txn, key)
 
     def __iter__(self):
         return iter(self.apris())
 
-    def setMsg(self, message):
+    def set_msg(self, message):
         """Give this `Register` a brief description.
 
         WARNING: This method OVERWRITES the current msg. In order to append a new msg to the current one, do
         something like the following:
 
             old_message = str(reg)
             new_message = old_message + " Hello!"
-            reg.setMsg(new_message)
+            reg.set_msg(new_message)
 
         :param message: (type `str`)
         """
 
         if not isinstance(message, str):
             raise TypeError("`msg` must be a string.")
 
         self._msg = message
 
         if self._created:
-            with self._msgFilepath.open("w") as fh:
+            with self._msg_filepath.open("w") as fh:
                 fh.write(message)
 
-    def setStartnInfo(self, head = None, tailLen = None):
-        """Set the range of the `startn_` parameters of disk `Block`s belonging to this `Register`.
+    def set_startn_info(self, head = None, tail_len = None):
+        """Set the range of the `startn` parameters of disk `Block`s belonging to this `Register`.
 
-        Reset to default `head` and `tail_length` by omitting the parameters.
+        Reset to default `head` and `tail_len` by omitting the parameters.
 
-        If the `startn_` parameter is very large (of order more than trillions), then the `Register` database can
-        become very bloated by storing many redundant digits for the `startn_` parameter. Calling this method with
-        appropriate `head` and `tail_length` parameters alleviates the bloat.
+        If the `startn` parameter is very large (of order more than trillions), then the `Register` database can
+        become very bloated by storing many redundant digits for the `startn` parameter. Calling this method with
+        appropriate `head` and `tail_len` parameters alleviates the bloat.
 
-        The "head" and "tail" of a non-negative number x is defined by x = head * 10^L + tail, where L is the "length_",
+        The "head" and "tail" of a non-negative number x is defined by x = head * 10^L + tail, where L is the "length",
         or the number of digits, of "tail". (L must be at least 1, and 0 is considered to have 1 digit.)
 
-        By calling `setstartnInfo(head, tail_length)`, the user is asserting that the startn_ of every disk
-        `Block` belong to this `Register` can be decomposed in the fashion startn_ = head * 10^tail_length + tail. The
-        user is discouraged to call this method for large `tail_length` values (>12), as this is likely unnecessary and
+        By calling `set_startn_info(head, tail_len)`, the user is asserting that the `startn` of every disk
+        `Block` belong to this `Register` can be decomposed in the fashion startn = head * 10^tail_length + tail. The
+        user is discouraged to call this method for large `tail_len` values (>12), as this is likely unnecessary and
         defeats the purpose of this method.
 
         :param head: (type `int`, optional) Non-negative. If omitted, resets this `Register` to the default `head`.
-        :param tailLen: (type `int`) Positive. If omitted, resets this `Register` to the default `tail_length`.
+        :param tail_len: (type `int`) Positive. If omitted, resets this `Register` to the default `tail_len`.
         """
 
         # DEBUG : 1, 2
 
-        self._checkOpenRaise("setStartnInfo")
+        self._check_open_raise("set_startn_info")
 
-        self._checkReadwriteRaise("setStartnInfo")
+        self._check_readwrite_raise("set_startn_info")
 
-        if head is not None and not isInt(head):
+        if head is not None and not is_int(head):
             raise TypeError("`head` must be of type `int`.")
 
         elif head is not None:
             head = int(head)
 
         else:
             head = _START_N_HEAD_DEFAULT
 
-        if tailLen is not None and not isInt(tailLen):
-            raise TypeError("`tailLen` must of of type `int`.")
+        if tail_len is not None and not is_int(tail_len):
+            raise TypeError("`tail_len` must of of type `int`.")
 
-        elif tailLen is not None:
-            tailLen = int(tailLen)
+        elif tail_len is not None:
+            tail_len = int(tail_len)
 
         else:
-            tailLen = _START_N_TAIL_LENGTH_DEFAULT
+            tail_len = _START_N_TAIL_LENGTH_DEFAULT
 
         if head < 0:
             raise ValueError("`head` must be non-negative.")
 
-        if tailLen <= 0:
-            raise ValueError("`tailLen` must be positive.")
+        if tail_len <= 0:
+            raise ValueError("`tail_len` must be positive.")
 
-        if head == self._startnHead and tailLen == self._startnTailLength:
+        if head == self._startn_head and tail_len == self._startn_tail_length:
             return
 
-        new_mod = 10 ** tailLen
+        new_mod = 10 ** tail_len
 
-        with lmdbPrefixIter(self._db, _BLK_KEY_PREFIX) as it:
+        with lmdb_prefix_iter(self._db, _BLK_KEY_PREFIX) as it:
 
             for key, _ in it:
 
-                apri, startn, length = self._convertDiskBlockKey(_BLK_KEY_PREFIX_LEN, key)
+                apri, startn, length = self._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, key)
 
                 if startn // new_mod != head:
 
                     raise ValueError(
-                        "The following `startn_` does not have the correct head:\n" +
-                        f"`startn_`   : {startn}\n" +
-                        "That `startn_` is associated with a `Block` whose `ApriInfo` and length_ is:\n" +
-                        f"`ApriInfo` : {str(apri.toJson())}\n" +
-                        f"length_      : {length}\n"
+                        "The following `startn` does not have the correct head:\n" +
+                        f"`startn`   : {startn}\n" +
+                        "That `startn` is associated with a `Block` whose `ApriInfo` and length is:\n" +
+                        f"`ApriInfo` : {str(apri)}\n" +
+                        f"length     : {length}\n"
                     )
 
         if _debug == 1:
             raise KeyboardInterrupt
 
         try:
 
             with self._db.begin(write = True) as rw_txn:
 
                 with self._db.begin() as ro_txn:
 
-                    with lmdbPrefixIter(ro_txn, _BLK_KEY_PREFIX) as it:
+                    with lmdb_prefix_iter(ro_txn, _BLK_KEY_PREFIX) as it:
 
                         rw_txn.put(_START_N_HEAD_KEY, str(head).encode("ASCII"))
-                        rw_txn.put(_START_N_TAIL_LENGTH_KEY, str(tailLen).encode("ASCII"))
+                        rw_txn.put(_START_N_TAIL_LENGTH_KEY, str(tail_len).encode("ASCII"))
 
                         for key, val in it:
 
-                            _, startn, _ = self._convertDiskBlockKey(_BLK_KEY_PREFIX_LEN, key)
-                            apri_json, _, length_bytes = Register._splitDiskBlockKey(_BLK_KEY_PREFIX_LEN, key)
+                            _, startn, _ = self._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, key)
+                            apri_json, _, length_bytes = Register._split_disk_block_key(_BLK_KEY_PREFIX_LEN, key)
 
                             new_startn_bytes = str(startn % new_mod).encode("ASCII")
 
-                            new_key = Register._joinDiskBlockData(
+                            new_key = Register._join_disk_block_data(
                                 _BLK_KEY_PREFIX, apri_json, new_startn_bytes, length_bytes
                             )
 
                             if key != new_key:
 
                                 rw_txn.put(new_key, val)
                                 rw_txn.delete(key)
 
                 if _debug == 2:
                     raise KeyboardInterrupt
 
         except lmdb.MapFullError as e:
-            raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._dbMapSize)) from e
+            raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
 
-        self._startnHead = head
-        self._startnTailLength = tailLen
-        self._startnTailMod = 10 ** self._startnTailLength
+        self._startn_head = head
+        self._startn_tail_length = tail_len
+        self._startn_tail_mod = 10 ** self._startn_tail_length
 
     @contextmanager
     def open(self, readonly = False):
 
         if not self._created and not readonly:
 
             # set local directory info and create levelDB database
-            localDir = randomUniqueFilename(self.savesDir, length = 4, alphabet = LOCAL_DIR_CHARS)
+            local_dir = random_unique_filename(self.saves_dir, length = 4, alphabet = LOCAL_DIR_CHARS)
 
             try:
 
-                localDir.mkdir(exist_ok = False)
-                (localDir / REG_FILENAME).mkdir(exist_ok = False)
+                local_dir.mkdir()
+                (local_dir / REG_FILENAME).mkdir()
 
-                with (localDir / MSG_FILEPATH).open("x") as fh:
+                with (local_dir / MSG_FILEPATH).open("x") as fh:
                     fh.write(self._msg)
 
-                with (localDir / VERSION_FILEPATH).open("x") as fh:
+                with (local_dir / VERSION_FILEPATH).open("x") as fh:
                     fh.write(self._version + "\nDO NOT EDIT THIS FILE. CALL THE FUNCTION `updateRegVersion` INSTEAD.")
 
-                with (localDir / CLS_FILEPATH).open("x") as fh:
+                with (local_dir / CLS_FILEPATH).open("x") as fh:
                     fh.write(str(type(self).__name__) + "\nDO NOT EDIT THIS FILE.")
 
-                with (localDir / MAP_SIZE_FILEPATH).open("x") as fh:
-                    fh.write(str(self._dbMapSize) + "\nDO NOT EDIT THIS FILE. CALL THE FUNCTION `increaseRegSize` INSTEAD.")
+                with (local_dir / MAP_SIZE_FILEPATH).open("x") as fh:
+                    fh.write(str(self._db_map_size) + "\nDO NOT EDIT THIS FILE. CALL THE FUNCTION `increase_reg_size` INSTEAD.")
 
-                (localDir / DATABASE_FILEPATH).mkdir(exist_ok = False)
-                self._setLocalDir(localDir)
-                self._db = openLmdb(self._dbFilepath, self._dbMapSize, False)
+                (local_dir / DATABASE_FILEPATH).mkdir()
+                self._set_local_dir(local_dir)
+                self._db = open_lmdb(self._db_filepath, self._db_map_size, False)
 
                 try:
 
                     with self._db.begin(write = True) as txn:
                         # set register info
-                        txn.put(_START_N_HEAD_KEY, str(self._startnHead).encode("ASCII"))
-                        txn.put(_START_N_TAIL_LENGTH_KEY, str(self._startnTailLength).encode("ASCII"))
+                        txn.put(_START_N_HEAD_KEY, str(self._startn_head).encode("ASCII"))
+                        txn.put(_START_N_TAIL_LENGTH_KEY, str(self._startn_tail_length).encode("ASCII"))
                         txn.put(_LENGTH_LENGTH_KEY, str(_LENGTH_LENGTH_DEFAULT).encode("ASCII"))
                         txn.put(_CURR_ID_KEY, b"0")
 
                 except lmdb.MapFullError as e:
-                    raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._dbMapSize)) from e
+                    raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
 
-                Register._addInstance(localDir, self)
+                Register._add_instance(local_dir, self)
                 yiel = self
 
             except BaseException as e:
 
-                if localDir.is_dir():
-                    shutil.rmtree(localDir)
+                if local_dir.is_dir():
+                    shutil.rmtree(local_dir)
 
                 raise e
 
         elif self._created:
-            yiel = self._openCreated(readonly)
+            yiel = self._open_created(readonly)
 
         else:
             raise ValueError(
                 "You must `open` this `Register` at least once with `readonly = False` before you can open it in "
                 "read-only mode."
             )
 
         try:
             yield yiel
 
         finally:
-            yiel._closeCreated()
+            yiel._close_created()
 
     @staticmethod
     @contextmanager
     def opens(*regs, **kwargs):
 
         if (len(kwargs) == 1 and 'readonlys' not in kwargs) or len(kwargs) > 1:
             raise KeyError("`opens` only takes one keyword-argument, `readonlys`.")
@@ -582,91 +593,91 @@
         with stack:
 
             for reg, readonly in zip(regs, readonlys):
                 yld.append(stack.enter_context(reg.open(readonly = readonly)))
 
             yield tuple(yld)
 
-    def increaseRegSize(self, numBytes):
+    def increase_reg_size(self, num_bytes):
         """WARNING: DO NOT CALL THIS METHOD FROM MORE THAN ONE PYTHON PROCESS AT A TIME. You are safe if you call it
         from only one Python process. You are safe if you have multiple Python processes running and call it from only
         ONE of them. But do NOT call it from multiple processes at once. Doing so may result in catastrophic loss of
         data.
 
-        :param numBytes: (type `int`) Positive.
+        :param num_bytes: (type `int`) Positive.
         """
 
-        self._checkOpenRaise("increaseRegSize")
+        self._check_open_raise("increase_reg_size")
 
-        if not isInt(numBytes):
-            raise TypeError("`numBytes` must be of type `int`.")
+        if not is_int(num_bytes):
+            raise TypeError("`num_bytes` must be of type `int`.")
 
-        if numBytes <= 0:
-            raise ValueError("`numBytes` must be positive.")
+        if num_bytes <= 0:
+            raise ValueError("`num_bytes` must be positive.")
 
-        if numBytes <= self._dbMapSize:
-            raise ValueError("`numBytes` must be larger than the current `Register` size.")
+        if num_bytes <= self._db_map_size:
+            raise ValueError("`num_bytes` must be larger than the current `Register` size.")
 
-        self._db.set_mapsize(numBytes)
-        self._dbMapSize = numBytes
+        self._db.set_mapsize(num_bytes)
+        self._db_map_size = num_bytes
 
-        with self._dbMapSizeFilepath.open("w") as fh:
-            fh.write(str(self._dbMapSize))
+        with self._db_map_size_filepath.open("w") as fh:
+            fh.write(str(self._db_map_size))
 
-    def regSize(self):
-        return self._dbMapSize
+    def reg_size(self):
+        return self._db_map_size
 
     def ident(self):
 
         if not self._created:
             raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("ident"))
 
-        return str(self._localDir)
+        return str(self._local_dir)
 
     #################################
     #    PROTEC REGISTER METHODS    #
 
-    def _openCreated(self, readonly):
+    def _open_created(self, readonly):
 
-        if Register._instanceExists(self._localDir):
-            ret = Register._getInstance(self._localDir)
+        if Register._instance_exists(self._local_dir):
+            ret = Register._get_instance(self._local_dir)
 
         else:
             ret = self
 
         if not ret._created:
-            raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("_openCreated"))
+            raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("_open_created"))
 
-        if ret._db is not None and not ret._dbIsClosed():
+        if ret._db is not None and not ret._db_is_closed():
             raise RegisterAlreadyOpenError()
 
         ret._readonly = readonly
 
-        ret._db = openLmdb(ret._dbFilepath, ret._dbMapSize, readonly)
+        ret._db = open_lmdb(ret._db_filepath, ret._db_map_size, readonly)
 
         with ret._db.begin() as txn:
-            ret._lengthLength = int(txn.get(_LENGTH_LENGTH_KEY))
+            ret._length_length = int(txn.get(_LENGTH_LENGTH_KEY))
 
-        ret._maxLength = 10 ** ret._lengthLength - 1
+        ret._max_length = 10 ** ret._length_length - 1
 
         return ret
 
-    def _closeCreated(self):
+    def _close_created(self):
         self._db.close()
 
     @contextmanager
-    def _recursiveOpen(self, readonly):
+    def _recursive_open(self, readonly):
 
         if not self._created:
-            raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("_recursiveOpen"))
+            raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("_recursive_open"))
 
         else:
 
             try:
-                yiel = self._openCreated(readonly)
+                yiel = self._open_created(readonly)
                 need_close = True
 
             except RegisterAlreadyOpenError:
                 yiel = self
                 need_close = False
 
             if not readonly and yiel._readonly:
@@ -675,30 +686,30 @@
                 )
 
             try:
                 yield yiel
 
             finally:
                 if need_close:
-                    yiel._closeCreated()
+                    yiel._close_created()
 
-    def _checkOpenRaise(self, methodName):
+    def _check_open_raise(self, method_name):
 
-        if self._db is None or self._dbIsClosed():
+        if self._db is None or self._db_is_closed():
             raise RegisterError(
                 f"This `Register` database has not been opened. You must open this register via `with reg.open() as " +
-                f"reg:` before calling the method `{methodName}`."
+                f"reg:` before calling the method `{method_name}`."
             )
 
-    def _checkReadwriteRaise(self, methodName):
-        """Call `self._checkOpenRaise` before this method."""
+    def _check_readwrite_raise(self, method_name):
+        """Call `self._check_open_raise` before this method."""
 
         if self._readonly:
             raise RegisterError(
-                f"This `Register` is `open`ed in read-only mode. In order to call the method `{methodName}`, you must "
+                f"This `Register` is `open`ed in read-only mode. In order to call the method `{method_name}`, you must "
                 "open this `Register` in read-write mode via `with reg.open() as reg:`."
             )
 
     # def _check_memory_raise(self, keys, vals):
     #
     #     stat = self._db.stat()
     #
@@ -706,485 +717,459 @@
     #
     #     entry_size_bytes = sum(len(key) + len(val) for key, val in zip(keys, vals)) * BYTES_PER_CHAR
     #
     #     if current_size + entry_size_bytes >= Register._MEMORY_FULL_PROP * self._dbMapSize:
     #
     #         raise MemoryError(
     #             "The `Register` database is out of memory. Please allocate more memory using the method "
-    #             "`Register.increaseRegSize`."
+    #             "`Register.increase_reg_size`."
     #         )
 
-    def _setLocalDir(self, localDir):
-        """`localDir` and a corresponding register database must exist prior to calling this method.
+    def _set_local_dir(self, local_dir):
+        """`local_dir` and a corresponding register database must exist prior to calling this method.
 
-        :param localDir: (type `pathlib.Path`) Absolute.
+        :param local_dir: (type `pathlib.Path`) Absolute.
         """
 
-        if not localDir.is_absolute():
-            raise ValueError(NOT_ABSOLUTE_ERROR_MESSAGE.format(str(localDir)))
+        if not local_dir.is_absolute():
+            raise ValueError(NOT_ABSOLUTE_ERROR_MESSAGE.format(str(local_dir)))
 
-        if localDir.parent != self.savesDir:
+        if local_dir.parent != self.saves_dir:
             raise ValueError(
-                "The `localDir` argument must be a sub-directory of `reg.savesDir`.\n" +
-                f"`localDir.parent`    : {str(localDir.parent)}\n"
-                f"`reg.savesDir` : {str(self.savesDir)}"
+                "The `local_dir` argument must be a sub-directory of `reg.savesDir`.\n" +
+                f"`local_dir.parent`    : {str(local_dir.parent)}\n"
+                f"`reg.savesDir` : {str(self.saves_dir)}"
             )
 
-        checkRegStructure(localDir)
+        check_reg_structure(local_dir)
 
         self._created = True
 
-        self._localDir = localDir
-        self._localDirBytes = str(self._localDir).encode("ASCII")
+        self._local_dir = local_dir
+        self._local_dir_bytes = str(self._local_dir).encode("ASCII")
 
-        self._dbFilepath = self._localDir / DATABASE_FILEPATH
+        self._db_filepath = self._local_dir / DATABASE_FILEPATH
 
-        self._subregBytes = (
-            _SUB_KEY_PREFIX + self._localDirBytes
+        self._subreg_bytes = (
+            _SUB_KEY_PREFIX + self._local_dir_bytes
         )
 
-        self._versionFilepath = localDir / VERSION_FILEPATH
-        self._msgFilepath = localDir / MSG_FILEPATH
-        self._clsFilepath = localDir / CLS_FILEPATH
-        self._dbMapSizeFilepath = localDir / MAP_SIZE_FILEPATH
+        self._version_filepath = local_dir / VERSION_FILEPATH
+        self._msg_filepath = local_dir / MSG_FILEPATH
+        self._cls_filepath = local_dir / CLS_FILEPATH
+        self._db_map_size_filepath = local_dir / MAP_SIZE_FILEPATH
 
-    def _hasCompatibleVersion(self):
+    def _has_compatible_version(self):
         return self._version in COMPATIBLE_VERSIONS
 
-    def _dbIsClosed(self):
+    def _db_is_closed(self):
 
         if not self._created:
-            raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("_dbIsClosed"))
+            raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("_db_is_closed"))
 
         else:
-            return lmdbIsClosed(self._db)
+            return lmdb_is_closed(self._db)
 
     #################################
     #      PUBLIC APRI METHODS      #
 
     def apris(self, diskonly = False, recursively = False):
 
-        self._checkOpenRaise("apris")
+        self._check_open_raise("apris")
+
+        if not isinstance(diskonly, bool):
+            raise TypeError("`diskonly` must be of type `bool`")
 
         if not isinstance(recursively, bool):
             raise TypeError("`recursively` must be of type `bool`")
 
         ret = []
 
         if not diskonly:
-            ret.extend(self._ramBlks.keys())
+            ret.extend(self._ram_blks.keys())
 
-        with lmdbPrefixIter(self._db, _ID_APRI_KEY_PREFIX) as it:
+        with self._db.begin() as txn:
 
-            for _, val in it:
-                ret.append(ApriInfo.fromJson(val.decode("ASCII")))
+            with lmdb_prefix_iter(txn, _ID_APRI_KEY_PREFIX) as it:
 
+                for _, val in it:
+                    ret.append(relational_decode_info(self, ApriInfo, val, txn))
 
         if recursively:
 
-            for subreg in self._iterSubregs():
+            for subreg in self._iter_subregs():
 
-                with subreg._recursiveOpen(True) as subreg:
+                with subreg._recursive_open(True) as subreg:
                     ret.append(subreg.apris())
 
         return sorted(list(set(ret)))
 
-    def changeApri(self, oldApri, newApri, recursively = False):
+    def change_apri(self, old_apri, new_apri, diskonly = False, recursively = False):
         """Replace an old `ApriInfo`, and all references to it, with a new `ApriInfo`.
 
         If ANY `Block`, `ApriInfo`, or `AposInfo` references `old_apri`, its entries in this `Register` will be
         updated to reflect the replacement of `old_apri` with `new_apri`. (See example below.) After the replacement
         `old_apri` -> `new_apri` is made, the set of `ApriInfo` that changed under that replacement must be disjoint
         from the set of `ApriInfo` that did not change. Otherwise, a `ValueError` is raised.
 
         For example, say we intend to replace
 
         `old_apri = ApriInfo(descr = "periodic points")`
 
         with
 
-        `new_apri = ApriInfo(descr = "odd periods", ref = "Newton et al. 2005")`.
+        `new_apri = ApriInfo(descr = "periodic points", ref = "Newton et al. 2005")`.
 
         In an example `Register`, there are two `Block`s, one with `old_apri` and the other with
 
-        `some_other_apri = ApriInfo(descr = "period length_", respective = old_apri)`.
+        `some_other_apri = ApriInfo(descr = "period length", respective = old_apri)`.
 
-        After a call to `changeApri(old_apri, new_apri)`, the first `Block` will have `new_apri` and the second
+        After a call to `change_apri(old_apri, new_apri)`, the first `Block` will have `new_apri` and the second
         will have
 
-        `ApriInfo(descr = "period length_", respective = new_apri)`.
+        `ApriInfo(descr = "period length", respective = new_apri)`.
 
-        :param oldApri: (type `ApriInfo`)
-        :param newApri: (type `ApriInfo`)
+        :param old_apri: (type `ApriInfo`)
+        :param new_apri: (type `ApriInfo`)
         :param recursively: (type `bool`)
         :raise ValueError: See above.
         """
 
         # DEBUG : 1, 2, 3
 
-        self._checkOpenRaise("changeApri")
+        self._check_open_raise("change_apri")
 
-        self._checkReadwriteRaise("changeApri")
+        self._check_readwrite_raise("change_apri")
 
-        # raises `DataNotFoundError` if `oldApri` does not have an ID
-        old_apri_id = self._getIdByApri(oldApri, None, False)
+        self._check_known_apri(old_apri)
 
-        if oldApri == newApri:
+        if old_apri == new_apri:
             return
 
-        old_apri_json = oldApri.toJson().encode("ASCII")
-
-        old_apri_id_key = _APRI_ID_KEY_PREFIX + old_apri_json
-        old_id_apri_key = _ID_APRI_KEY_PREFIX + old_apri_id
-
-        new_apri_json = newApri.toJson().encode("ASCII")
-
-        if lmdbHasKey(self._db, _APRI_ID_KEY_PREFIX + new_apri_json):
-
-            new_apri_id = self._getIdByApri(newApri, new_apri_json, False)
-            new_id_apri_key = _ID_APRI_KEY_PREFIX + new_apri_id
-            has_new_apri_already = True
-
-            warnings.warn(f"This `Register` already has a reference to {str(newApri)}.")
-
-        else:
-
-            new_apri_id = None
-            new_id_apri_key = None
-            has_new_apri_already = False
-
-        if _debug == 1:
-            raise KeyboardInterrupt
+        # if not diskonly:
+        #
+        #     for apri in self._ram_blks.keys():
+        #         apri.change_info(old_apri, new_apri)
 
         try:
 
-            with self._db.begin(write = True) as rw_txn:
-
-                with self._db.begin() as ro_txn:
-
-                    apris_changed = set()
-                    apris_didnt_change = set()
-
-                    # change all apri_id keys
-                    with lmdbPrefixIter(ro_txn, _APRI_ID_KEY_PREFIX) as it:
-                        for key, val in it:
-
-                            if key == old_apri_id_key:
-                                new_key = _APRI_ID_KEY_PREFIX + new_apri_json
-
-                            else:
-
-                                apri = ApriInfo.fromJson(key[_APRI_ID_KEY_PREFIX_LEN:].decode("ASCII"))
-                                replaced = apri.changeInfo(oldApri, newApri)
-                                new_key = _APRI_ID_KEY_PREFIX + replaced.toJson().encode("ASCII")
-
-                            if new_key != key:
-
-                                rw_txn.put(new_key, val)
-                                rw_txn.delete(key)
-                                apris_changed.add(new_key[_APRI_ID_KEY_PREFIX_LEN : ])
-
-                            else:
-                                apris_didnt_change.add(key[_APRI_ID_KEY_PREFIX_LEN : ])
-
-                    # check `apris_changed` and `apris_didnt_change` are disjoint, otherwise raise ValueError
-                    if not apris_changed.isdisjoint(apris_didnt_change):
-
-                        # ValueError automatically aborts the LMDB transaction
-                        raise ValueError(
-                            "The set of `ApriInfo` that changed under the replacement `oldApri` -> `newApri` must be "
-                            "disjoint from the set of `ApriInfo` that did not change."
-                        )
-
-                    # change all id_apri keys
-                    with lmdbPrefixIter(ro_txn, _ID_APRI_KEY_PREFIX) as it:
-                        for key, val in it:
-
-                            new_key = key
-
-                            if key == old_id_apri_key:
-                                new_val = new_apri_json
+            with self._db.begin(write = True) as txn:
 
-                            else:
+                if _debug == 1:
+                    raise KeyboardInterrupt
 
-                                apri = ApriInfo.fromJson(val.decode("ASCII"))
-                                replaced = apri.changeInfo(oldApri, newApri)
-                                new_val = replaced.toJson().encode("ASCII")
+                try:
+                    self._check_known_apri(new_apri, txn)
 
-                            if has_new_apri_already and key == new_id_apri_key:
-                                new_key = old_id_apri_key
+                except DataNotFoundError:
+                    has_new_apri_already = False
 
-                            if key != new_key or val != new_val:
-                                rw_txn.put(new_key, new_val)
+                else:
+                    has_new_apri_already = True
 
-                    if has_new_apri_already:
+                if has_new_apri_already:
+                    warnings.warn(f"This `Register` already has a reference to {str(new_apri)}.")
 
-                        # change all blocks
-                        for prefix in [_BLK_KEY_PREFIX, _COMPRESSED_KEY_PREFIX]:
+                # delete old_apri and reserve its ID
+                old_id = self._get_id_by_apri(old_apri, None, False, txn, None)
+                old_id_apri_key = _ID_APRI_KEY_PREFIX + old_id
+                old_apri_json = txn.get(old_id_apri_key)
+                old_apri_id_key = _APRI_ID_KEY_PREFIX + old_apri_json
+                txn.delete(old_id_apri_key)
+                txn.delete(old_apri_id_key)
+                reserved = [old_id]
 
-                            with lmdbPrefixIter(ro_txn, prefix + new_apri_id + _KEY_SEP) as it:
-                                for key, val in it:
+                if _debug == 2:
+                    raise KeyboardInterrupt
 
-                                    new_blk_key = prefix + old_apri_id + key[key.index(_KEY_SEP) : ]
-                                    rw_txn.put(new_blk_key, val)
+                # make inner id's if they're missing
+                for key, info in new_apri.iter_inner_info(mode = "dfs"):
 
-                    # change all apos vals
-                    with lmdbPrefixIter(ro_txn, _APOS_KEY_PREFIX) as it:
-                        for key, val in it:
+                    if key is not None and isinstance(info, ApriInfo):
+                        self._get_id_by_apri(info, None, True, txn, reserved)
 
-                            apos = AposInfo.fromJson(val.decode("ASCII"))
-                            replaced = apos.changeInfo(oldApri, newApri)
-                            new_val = replaced.toJson().encode("ASCII")
+                # check for duplicate keys and give old_id new new_apri
+                new_apri_json = relational_encode_info(self, new_apri, txn)
+                new_apri_id_key = _APRI_ID_KEY_PREFIX + new_apri_json
 
-                            if val != new_val:
-                                rw_txn.put(new_key, new_val)
+                if lmdb_has_key(txn, new_apri_id_key):
+                    raise ValueError("Duplicate `ApriInfo`.")
 
-                    if _debug == 2:
-                        raise KeyboardInterrupt
+                Register._add_apri(txn, old_id, new_apri, new_apri_json)
 
                 if _debug == 3:
                     raise KeyboardInterrupt
 
         except lmdb.MapFullError as e:
-            raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._dbMapSize)) from e
+            raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
 
         if recursively:
-            for subreg in self._iterSubregs():
-                with subreg._recursiveOpen(False) as subreg:
-                    subreg.changeApri(oldApri, newApri, True)
 
-    def rmvApri(self, apri, force = False, missingOk = False):
+            for subreg in self._iter_subregs():
+
+                with subreg._recursive_open(False) as subreg:
+                    subreg.change_apri(old_apri, new_apri, True)
+
+    def rmv_apri(self, apri, force = False, missing_ok = False):
         """Remove an `ApriInfo` that is not associated with any other `ApriInfo`, `Block`, nor `AposInfo`.
 
         :param apri: (type `ApriInfo`)
-        :raise ValueError: If there are any `ApriInfo`, `Block`, or `AposInfo` associated with `apri`.
+        :raise ValueError: If there are any `ApriInfo`, `Block`, or `AposInfo` associated with `info`.
         """
 
         # DEBUG : 1, 2, 3, 4, 5
 
-        self._checkOpenRaise("rmvApri")
+        self._check_open_raise("rmv_apri")
 
-        self._checkReadwriteRaise("rmvApri")
+        self._check_readwrite_raise("rmv_apri")
 
         if not isinstance(apri, ApriInfo):
-            raise TypeError("`apri` must be of type `ApriInfo`.")
+            raise TypeError("`info` must be of type `ApriInfo`.")
 
         if not isinstance(force, bool):
             raise TypeError("`force` must be of type `bool`.")
 
-        if not isinstance(missingOk, bool):
-            raise TypeError("`missingOk` must be of type `bool`.")
+        if not isinstance(missing_ok, bool):
+            raise TypeError("`missing_ok` must be of type `bool`.")
 
-        if not missingOk:
-            self._checkKnownApri(apri)
+        if not missing_ok:
+            self._check_known_apri(apri)
 
         txn = None
-        ramBlkDelSuccess = False
+        ram_blk_del_success = False
         reinsert = None
 
         try:
 
-            if apri in self._ramBlks.keys():
+            if apri in self._ram_blks.keys():
 
-                reinsert = self._ramBlks[apri]
-                del self._ramBlks[apri]
-                ramBlkDelSuccess = True
+                reinsert = self._ram_blks[apri]
+                del self._ram_blks[apri]
+                ram_blk_del_success = True
 
             with ReversibleTransaction(self._db).begin(write = True) as txn:
-                blkDatas = self._rmvApriTxn(apri, force, txn)
+                blkDatas = self._rmv_apri_txn(apri, force, txn)
 
             for apri_, startn, length in blkDatas:
-                self.rmvDiskBlk(apri_, startn, length, False, False)
+                self.rmv_disk_blk(apri_, startn, length, False, False)
 
         except BaseException as e:
 
-            if ramBlkDelSuccess:
-                self._ramBlks[apri] = reinsert
+            if ram_blk_del_success:
+                self._ram_blks[apri] = reinsert
 
             if txn is not None:
 
                 with self._db.begin(write = True) as txn_:
                     txn.reverse(txn_)
 
             if isinstance(e, lmdb.MapFullError):
-                raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._dbMapSize)) from e
+                raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
 
             else:
                 raise e
 
     #################################
     #      PROTEC APRI METHODS      #
 
-    def _checkKnownApri(self, apri):
+    def _check_known_apri(self, apri, txn = None):
+
+        commit = txn is None
+
+        if commit:
+            txn = self._db.begin()
 
         try:
-            self._getIdByApri(apri, None, False, None)
 
-        except DataNotFoundError:
-            pass
+            try:
+                self._get_id_by_apri(apri, None, False, None, txn)
 
-        else:
-            return
+            except DataNotFoundError:
+                pass
+
+            else:
+                return
+
+        finally:
+
+            if commit:
+                txn.commit()
 
-        if apri not in self._ramBlks.keys():
+        if apri not in self._ram_blks.keys():
             raise DataNotFoundError(_NO_APRI_ERROR_MESSAGE.format(str(apri)))
 
-    def _getApriJsonById(self, _id, txn = None):
+    def _get_apri_json_by_id(self, id_, txn = None):
         """Get JSON bytestring representing an `ApriInfo` instance.
 
-        :param _id: (type `bytes`)
+        :param id_: (type `bytes`)
         :param txn: (type `lmbd.Transaction`, default `None`) The transaction to query. If `None`, then use open a new
         transaction and commit it after this method resolves.
         :return: (type `bytes`)
         """
 
         commit = txn is None
 
         if commit:
             txn = self._db.begin()
 
         try:
-            return txn.get(_ID_APRI_KEY_PREFIX + _id)
+            return txn.get(_ID_APRI_KEY_PREFIX + id_)
 
         finally:
 
             if commit:
                 txn.commit()
 
-    def _getIdByApri(self, apri, apriJson, missingOk, txn = None):
-        """Get an `ApriInfo` ID for this database. If `missingOk is True`, then create an ID if the passed `apri` or
-        `apriJson` is unknown to this `Register`.
+    def _get_id_by_apri(self, apri, apri_json, missing_ok, txn = None, reserved = None):
+        """Get an `ApriInfo` ID for this database. If `missing_ok is True`, then create an ID if the passed `apri` or
+        `apri_json` is unknown to this `Register`.
 
-        One of `apri` and `apriJson` can be `None`, but not both. If both are not `None`, then `apri` is used.
+        One of `apri` and `apri_json` can be `None`, but not both. If both are not `None`, then `apri` is used.
 
         `self._db` must be opened by the caller.
 
         :param apri: (type `ApriInfo`)
-        :param apriJson: (type `bytes`)
-        :param missingOk: (type `bool`) Create an ID if the passed `apri` or `apriJson` is unknown to this `Register`.
-        :param txn: (type `lmbd.Transaction`, default `None`) The transaction to query. If `None`, then use open a new
-        transaction and commit it after this method resolves.
-        :raises DataNotFoundError: If `apri` or `apriJson` is not known to this `Register` and `missingOk
+        :param apri_json: (type `bytes`)
+        :param missing_ok: (type `bool`) Create an ID if the passed `apri` or `apri_json` is unknown to this `Register`.
+        :param txn: (type `lmbd.Transaction`, default `None`) The transaction to query. If `None`, then open a new
+        transaction and commit it after this method returns.
+        :param reserved: (type `list`, default `None`) Apri ID's that cannot be returned by this method.
+        :raises DataNotFoundError: If `apri` or `apri_json` is not known to this `Register` and `missing_ok
         is False`.
         :return: (type `bytes`)
         """
 
         if apri is not None:
-            key = _APRI_ID_KEY_PREFIX + apri.toJson().encode("ASCII")
+            apri_json =  relational_encode_info(self, apri, txn)
 
-        elif apriJson is not None:
-            key = _APRI_ID_KEY_PREFIX + apriJson
-
-        else:
+        elif apri_json is None:
             raise ValueError
 
         commit = txn is None
+        key = _APRI_ID_KEY_PREFIX + apri_json
 
-        if commit and missingOk:
+        if commit and missing_ok:
             txn = self._db.begin(write = True)
 
         elif commit:
             txn = self._db.begin()
 
         try:
 
-            _id = txn.get(key, default = None)
+            id_ = txn.get(key, default = None)
 
-            if _id is not None:
-                return _id
+            if id_ is not None:
+                return id_
 
-            elif missingOk:
+            elif missing_ok:
 
-                _id = txn.get(_CURR_ID_KEY)
-                next_id = str(int(_id) + 1).encode("ASCII")
-                txn.put(_CURR_ID_KEY, next_id)
-                txn.put(key, _id)
-                txn.put(_ID_APRI_KEY_PREFIX + _id, key[_APRI_ID_KEY_PREFIX_LEN : ])
-
-                if 8 + 6 + len(key) > 4096:
-                    warnings.warn(f"Long `ApriInfo` result in disk memory inefficiency. Long `ApriInfo`: {str(apri)}.")
-
-                return _id
+                next_id = Register._get_new_apri_id(txn, reserved if reserved is not None else [])
+                Register._add_apri(txn, next_id, apri, apri_json)
+                return next_id
 
             else:
 
                 if apri is None:
-                    apri = ApriInfo.fromJson(apriJson.decode("ASCII"))
+                    apri = relational_decode_info(self, ApriInfo, apri_json, txn)
 
                 raise DataNotFoundError(_NO_APRI_ERROR_MESSAGE.format(str(apri)))
 
         finally:
 
             if commit:
 
                 try:
                     txn.commit()
 
                 except lmdb.MapFullError as e:
-                    raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._dbMapSize)) from e
+                    raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
+
+    @staticmethod
+    def _add_apri(txn, id_, apri, apri_json):
+
+        apri_id_key = _APRI_ID_KEY_PREFIX + apri_json
+        id_apri_key = _ID_APRI_KEY_PREFIX + id_
+        txn.put(apri_id_key, id_)
+        txn.put(id_apri_key, apri_json)
+
+        if 8 + 6 + len(apri_id_key) > 4096:
+            warnings.warn(f"Long `ApriInfo` result in disk memory inefficiency. Long `ApriInfo`: {str(apri)}.")
+
+    @staticmethod
+    def _get_new_apri_id(txn, reserved):
+
+        for next_id_num in count(int(txn.get(_CURR_ID_KEY))):
 
-    def _rmvApriTxn(self, apri, force, txn):
+            next_id = str(next_id_num).encode("ASCII")
+
+            if next_id not in reserved:
+                break
+
+        txn.put(_CURR_ID_KEY, str(next_id_num + 1).encode("ASCII"))
+        return next_id
+
+    def _rmv_apri_txn(self, apri, force, txn):
 
         apris = []
         aposs = []
-        blkDatas = []
-        self._rmvApriTxnHelper(txn, apri, apris, aposs, blkDatas, force)
+        blk_datas = []
+        self._rmv_apri_txn_helper(txn, apri, apris, aposs, blk_datas, force)
 
         if force:
 
-            for data in blkDatas:
-                self._rmvDiskBlkTxn(data[0], data[1], data[2], txn)
+            for data in blk_datas:
+                self._rmv_disk_blk_txn(data[0], data[1], data[2], txn)
 
             for apri in aposs:
-                self._rmvAposInfoTxn(apri, txn)
+                self._rmv_apos_info_txn(apri, txn)
 
             for apri in apris:
-                self._rmvApriTxn(apri, False, txn)
+                self._rmv_apri_txn(apri, False, txn)
 
-        apriJson = apri.toJson().encode()
-        apriId = self._getIdByApri(apri, apriJson, False, txn)
-        txn.delete(_ID_APRI_KEY_PREFIX + apriId)
-        txn.delete(_APRI_ID_KEY_PREFIX + apriJson)
+        apri_json = relational_encode_info(self, apri, txn)
+        apri_id = self._get_id_by_apri(apri, apri_json, False, txn)
+        txn.delete(_ID_APRI_KEY_PREFIX + apri_id)
+        txn.delete(_APRI_ID_KEY_PREFIX + apri_json)
 
-        return blkDatas
+        return blk_datas
 
-    def _rmvApriTxnHelper(self, txn, apri, apris, aposs, blkDatas, force):
+    def _rmv_apri_txn_helper(self, txn, apri, apris, aposs, blk_datas, force):
 
         apris.append(apri)
 
         if _debug == 1:
             raise KeyboardInterrupt
 
-        if self._numDiskBlksTxn(apri, txn) != 0:
+        if self._num_disk_blks_txn(apri, txn) != 0:
 
             if not force:
 
                 raise ValueError(
                     f"There are disk `Block`s saved with `{str(apri)}`. Please remove them first and call "
-                    "`rmvApri` again. Or remove them automatically by calling "
-                    "`reg.rmvApri(apri, force = True)`."
+                    "`rmv_apri` again. Or remove them automatically by calling "
+                    "`reg.rmv_apri(info, force = True)`."
                 )
 
             else:
 
-                for key, val in self._iterDiskBlkPairs(_BLK_KEY_PREFIX, apri, None, txn):
+                for key, val in self._iter_disk_blk_pairs(_BLK_KEY_PREFIX, apri, None, txn):
 
-                    blkFilename = val.decode("ASCII")
+                    blk_filename = val.decode("ASCII")
 
-                    if not isDeletable(self._localDir / blkFilename):
-                        raise OSError(f"Cannot delete `Block` file `{blkFilename}`.")
+                    if not is_deletable(self._local_dir / blk_filename):
+                        raise OSError(f"Cannot delete `Block` file `{blk_filename}`.")
 
-                    blkDatas.append(self._convertDiskBlockKey(_BLK_KEY_PREFIX_LEN, key))
+                    blk_datas.append(self._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, key))
 
-                for key, val in self._iterDiskBlkPairs(_COMPRESSED_KEY_PREFIX, apri, None, txn):
+                for key, val in self._iter_disk_blk_pairs(_COMPRESSED_KEY_PREFIX, apri, None, txn):
 
-                    comprFilename = val.decode("ASCII")
+                    compr_filename = val.decode("ASCII")
 
-                    if val != _IS_NOT_COMPRESSED_VAL and not isDeletable(self._localDir / comprFilename):
-                        raise OSError(f"Cannot delete compressed `Block` file `{comprFilename}`.")
+                    if val != _IS_NOT_COMPRESSED_VAL and not is_deletable(self._local_dir / compr_filename):
+                        raise OSError(f"Cannot delete compressed `Block` file `{compr_filename}`.")
 
         if _debug == 2:
             raise KeyboardInterrupt
 
         try:
             self.apos(apri)
 
@@ -1193,279 +1178,279 @@
 
         else:
 
             if not force:
 
                 raise ValueError(
                     f"There is an `AposInfo` associated with `{str(apri)}`. Please remove it first and call "
-                    "`rmvApri` again. Or remove automatically by calling `reg.rmvApri(apri, force = True)`."
+                    "`rmv_apri` again. Or remove automatically by calling `reg.rmv_apri(info, force = True)`."
                 )
 
             else:
                 aposs.append(apri)
 
         if _debug == 3:
             raise KeyboardInterrupt
 
-        with lmdbPrefixIter(txn, _ID_APRI_KEY_PREFIX) as it:
+        with lmdb_prefix_iter(txn, _ID_APRI_KEY_PREFIX) as it:
 
-            for _, _apri_json in it:
+            for _, apri_json_ in it:
 
-                _apri = ApriInfo.fromJson(_apri_json.decode("ASCII"))
+                apri_ = relational_decode_info(self, ApriInfo, apri_json_, txn)
 
-                if apri in _apri and apri != _apri:
+                if apri in apri_ and apri != apri_:
 
                     if not force:
 
                         raise ValueError(
-                            f"{str(_apri)} is associated with {str(apri)}. Please remove the former first before "
-                            f"removing the latter. Or remove automatically by calling `reg.rmvApri(apri, "
+                            f"{str(apri_)} is associated with {str(apri)}. Please remove the former first before "
+                            f"removing the latter. Or remove automatically by calling `reg.rmv_apri(info, "
                             f"force = True)`."
                         )
 
                     else:
-                        self._rmvApriTxnHelper(txn, _apri, apris, aposs, blkDatas, True)
+                        self._rmv_apri_txn_helper(txn, apri_, apris, aposs, blk_datas, True)
 
             if _debug == 4:
                 raise KeyboardInterrupt
 
     #################################
     #      PUBLIC APOS METHODS      #
 
-    def setApos(self, apri, apos):
+    def set_apos(self, apri, apos):
         """Set some `AposInfo` for corresponding `ApriInfo`.
 
         WARNING: This method will OVERWRITE any previous saved `AposInfo`. If you do not want to lose any previously
         saved data, then you should do something like the following:
 
-            apos = reg.apos(apri)
+            apos = reg.apos(info)
             apos.period_length = 5
-            reg.setApos(apos)
+            reg.set_apos(apos)
 
         :param apri: (type `ApriInfo`)
         :param apos: (type `AposInfo`)
         """
 
         # DEBUG : 1, 2
 
-        self._checkOpenRaise("setApos")
+        self._check_open_raise("set_apos")
 
-        self._checkReadwriteRaise("setApos")
+        self._check_readwrite_raise("set_apos")
 
         if not isinstance(apri, ApriInfo):
-            raise TypeError("`apri` must be of type `ApriInfo`")
+            raise TypeError("`info` must be of type `ApriInfo`")
 
         if not isinstance(apos, AposInfo):
             raise TypeError("`apos` must be of type `AposInfo`")
 
         if _debug == 1:
             raise KeyboardInterrupt
 
         try:
 
             with self._db.begin(write = True) as txn:
 
-                self._setAposInfoTxn(apri, apos, txn)
+                self._set_apos_info_txn(apri, apos, txn)
 
                 if _debug == 2:
                     raise KeyboardInterrupt
 
         except lmdb.MapFullError as e:
-            raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._dbMapSize)) from e
+            raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
 
     def apos(self, apri):
         """Get some `AposInfo` associated with a given `ApriInfo`.
 
         :param apri: (type `ApriInfo`)
-        :raises DataNotFoundError: If no `AposInfo` has been associated to `apri`.
+        :raises DataNotFoundError: If no `AposInfo` has been associated to `info`.
         :return: (type `AposInfo`)
         """
 
-        self._checkOpenRaise("apos")
+        self._check_open_raise("apos")
 
         if not isinstance(apri, ApriInfo):
             raise TypeError("`apri` must be of type `ApriInfo`")
 
-        key = self._getAposKey(apri, None, False)
-
         with self._db.begin() as txn:
+
+            key = self._get_apos_key(apri, None, False, txn)
             apos_json = txn.get(key, default=None)
 
-        if apos_json is not None:
-            return AposInfo.fromJson(apos_json.decode("ASCII"))
+            if apos_json is not None:
+                return relational_decode_info(self, AposInfo, apos_json, txn)
 
-        else:
-            raise DataNotFoundError(f"No `AposInfo` associated with `{str(apri)}`.")
+            else:
+                raise DataNotFoundError(f"No `AposInfo` associated with `{str(apri)}`.")
 
-    def rmvApos(self, apri, missingOk = False):
+    def rmv_apos(self, apri, missing_ok = False):
 
         # DEBUG : 1, 2
 
-        self._checkOpenRaise("rmvApos")
+        self._check_open_raise("rmv_apos")
 
-        self._checkReadwriteRaise("rmvApos")
+        self._check_readwrite_raise("rmv_apos")
 
         if not isinstance(apri, ApriInfo):
-            raise TypeError("`apri` must be of type `ApriInfo`.")
+            raise TypeError("`info` must be of type `ApriInfo`.")
 
-        if not isinstance(missingOk, bool):
-            raise TypeError("`missingOk` must be of type `bool`.")
+        if not isinstance(missing_ok, bool):
+            raise TypeError("`missing_ok` must be of type `bool`.")
 
         if _debug == 1:
             raise KeyboardInterrupt
 
         try:
 
             with self._db.begin(write = True) as txn:
 
-                self._rmvAposInfoTxn(apri, txn)
+                self._rmv_apos_info_txn(apri, txn)
 
                 if _debug == 2:
                     raise KeyboardInterrupt
 
         except lmdb.MapFullError as e:
-            raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._dbMapSize)) from e
+            raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
 
         except DataNotFoundError:
 
-            if not missingOk:
+            if not missing_ok:
                 raise
 
     #################################
     #      PROTEC APOS METHODS      #
 
-    def _setAposInfoTxn(self, apri, apos, txn):
+    def _set_apos_info_txn(self, apri, apos, txn):
 
-        key = self._getAposKey(apri, None, True, txn)
-        apos_json = apos.toJson().encode("ASCII")
+        key = self._get_apos_key(apri, None, True, txn)
+        apos_json = relational_encode_info(self, apos, txn)
         txn.put(key, apos_json)
 
         if 6 + 8 + _APOS_KEY_PREFIX_LEN +  len(apos_json) > 4096:
             warnings.warn(f"Long `AposInfo` result in disk memory inefficiency. Long `AposInfo`: {str(apri)}.")
 
-    def _rmvAposInfoTxn(self, apri, txn):
+    def _rmv_apos_info_txn(self, apri, txn):
 
-        key = self._getAposKey(apri, None, False, txn)
+        key = self._get_apos_key(apri, None, False, txn)
 
-        if lmdbHasKey(txn, key):
+        if lmdb_has_key(txn, key):
             txn.delete(key)
 
         else:
             raise DataNotFoundError(f"No `AposInfo` associated with `{str(apri)}`.")
 
-    def _getAposKey(self, apri, apriJson, missingOk, txn = None):
+    def _get_apos_key(self, apri, apri_json, missing_ok, txn = None):
         """Get a key for an `AposInfo` entry.
 
-        One of `apri` and `apriJson` can be `None`, but not both. If both are not `None`, then `apri` is used. If
-        `missingOk is True`, then create a new `ApriInfo` ID if one does not already exist for `apri`.
+        One of `apri` and `apri_json` can be `None`, but not both. If both are not `None`, then `apri` is used. If
+        `missing_ok is True`, then create a new `ApriInfo` ID if one does not already exist for `apri`.
 
         :param apri: (type `ApriInfo`)
-        :param apriJson: (type `bytes`)
-        :param missingOk: (type `bool`)
+        :param apri_json: (type `bytes`)
+        :param missing_ok: (type `bool`)
         :param txn: (type `lmbd.Transaction`, default `None`) The transaction to query. If `None`, then use open a new
         transaction and commit it after this method resolves.
-        :raises DataNotFoundError: If `missingOk is False` and `apri` is not known to this `Register`.
+        :raises DataNotFoundError: If `missing_ok is False` and `apri` is not known to this `Register`.
         :return: (type `bytes`)
         """
 
-        if apri is None and apriJson is None:
+        if apri is None and apri_json is None:
             raise ValueError
 
-        apri_id = self._getIdByApri(apri, apriJson, missingOk, txn)
+        apri_id = self._get_id_by_apri(apri, apri_json, missing_ok, txn)
 
         return _APOS_KEY_PREFIX + _KEY_SEP + apri_id
 
     #################################
     #  PUBLIC SUB-REGISTER METHODS  #
 
-    def addSubreg(self, subreg, existsOk = False):
+    def add_subreg(self, subreg, exists_ok = False):
 
         # DEBUG : 1, 2
 
-        self._checkOpenRaise("addSubreg")
+        self._check_open_raise("add_subreg")
 
-        self._checkReadwriteRaise("addSubreg")
+        self._check_readwrite_raise("add_subreg")
 
         if not isinstance(subreg, Register):
             raise TypeError("`subreg` must be of a `Register` derived type")
 
         if not subreg._created:
-            raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("addSubreg"))
+            raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("add_subreg"))
 
         if _debug == 1:
             raise KeyboardInterrupt
 
         try:
 
             with self._db.begin(write = True) as txn:
-                self._addSubregTxn(subreg, txn)
+                self._add_subreg_txn(subreg, txn)
 
         except lmdb.MapFullError as e:
-            raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._dbMapSize)) from e
+            raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
 
         except RegisterError as e:
 
             if str(e) == _REG_ALREADY_ADDED_ERROR_MESSAGE:
 
-                if not existsOk:
+                if not exists_ok:
                     raise
 
             else:
                 raise
 
-    def rmvSubreg(self, subreg, missingOk = False):
+    def rmv_subreg(self, subreg, missing_ok = False):
         """
         :param subreg: (type `Register`)
         """
 
         # DEBUG : 1, 2
 
-        self._checkOpenRaise("rmvSubreg")
+        self._check_open_raise("rmv_subreg")
 
-        self._checkReadwriteRaise("rmvSubreg")
+        self._check_readwrite_raise("rmv_subreg")
 
         if not isinstance(subreg, Register):
             raise TypeError("`subreg` must be of a `Register` derived type.")
 
-        if not isinstance(missingOk, bool):
-            raise TypeError("`missingOk` must be of type `bool`.")
+        if not isinstance(missing_ok, bool):
+            raise TypeError("`missing_ok` must be of type `bool`.")
 
         if _debug == 1:
             raise KeyboardInterrupt
 
         try:
 
             with self._db.begin(write = True) as txn:
 
-                self._rmvSubregTxn(subreg, txn)
+                self._rmv_subreg_txn(subreg, txn)
 
                 if _debug == 2:
                     raise KeyboardInterrupt
 
         except lmdb.MapFullError as e:
-            raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._dbMapSize)) from e
+            raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
 
         except DataNotFoundError:
 
-            if not missingOk:
+            if not missing_ok:
                 raise
 
     def subregs(self):
-        return list(self._iterSubregs())
+        return list(self._iter_subregs())
 
     #################################
     #  PROTEC SUB-REGISTER METHODS  #
 
-    def _addSubregTxn(self, subreg, txn):
+    def _add_subreg_txn(self, subreg, txn):
 
-        key = subreg._getSubregKey()
+        key = subreg._get_subreg_key()
 
-        if not lmdbHasKey(txn, key):
+        if not lmdb_has_key(txn, key):
 
-            if subreg._checkNoCyclesFrom(self):
+            if subreg._check_no_cycles_from(self):
 
                 txn.put(key, _SUB_VAL)
 
                 if _debug == 2:
                     raise KeyboardInterrupt
 
             else:
@@ -1476,101 +1461,101 @@
                     f'Intended super-register description: "{str(self)}". '
                     f'Intended sub-register description: "{str(subreg)}".'
                 )
 
         else:
             raise RegisterError(_REG_ALREADY_ADDED_ERROR_MESSAGE)
 
-    def _rmvSubregTxn(self, subreg, txn):
+    def _rmv_subreg_txn(self, subreg, txn):
 
-        key = subreg._getSubregKey()
+        key = subreg._get_subreg_key()
 
-        if lmdbHasKey(txn, key):
+        if lmdb_has_key(txn, key):
             txn.delete(key)
 
         else:
             raise RegisterError(f"No subregister found with the following message : {str(subreg)}")
 
-    def _checkNoCyclesFrom(self, original, touched = None):
+    def _check_no_cycles_from(self, original, touched = None):
         """Checks if adding `self` as a subregister to `original` would not create any directed cycles containing the
         arc `original` -> `self` in the subregister relation.
 
         Returns `False` if a directed cycle would be created and `True` otherwise. If `self` is already a subregister
         of `original`, then return `True` if the currently existing relation has no directed cycles that pass through
         `self`, and `False` otherwise. If `self == original`, then return `False`.
 
         :param original: (type `Register`)
         :param touched: used for recursion.
         :return: (type `bool`)
         """
 
         if not self._created or not original._created:
-            raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("_checkNoCyclesFrom"))
+            raise RegisterError(_NOT_CREATED_ERROR_MESSAGE.format("_check_no_cycles_from"))
 
         if self is original:
             return False
 
         if touched is None:
             touched = set()
 
-        with self._recursiveOpen(True) as reg:
+        with self._recursive_open(True) as reg:
 
             if any(
                 original is subreg
-                for subreg in reg._iterSubregs()
+                for subreg in reg._iter_subregs()
             ):
                 return False
 
-            for subreg in reg._iterSubregs():
+            for subreg in reg._iter_subregs():
 
                 if subreg not in touched:
 
                     touched.add(subreg)
-                    if not subreg._checkNoCyclesFrom(original, touched):
+                    if not subreg._check_no_cycles_from(original, touched):
                         return False
 
 
             else:
                 return True
 
-    def _iterSubregs(self):
+    def _iter_subregs(self):
 
-        with lmdbPrefixIter(self._db, _SUB_KEY_PREFIX) as it:
+        with lmdb_prefix_iter(self._db, _SUB_KEY_PREFIX) as it:
 
             for key, _ in it:
 
-                localDir = Path(key[_SUB_KEY_PREFIX_LEN : ].decode("ASCII"))
-                subreg = Register._fromLocalDir(localDir)
+                local_dir = Path(key[_SUB_KEY_PREFIX_LEN : ].decode("ASCII"))
+                subreg = Register._from_local_dir(local_dir)
                 yield subreg
 
-    def _getSubregKey(self):
-        return _SUB_KEY_PREFIX + self._localDirBytes
+    def _get_subreg_key(self):
+        return _SUB_KEY_PREFIX + self._local_dir_bytes
 
     #################################
     #    PUBLIC DISK BLK METHODS    #
 
     @classmethod
     @abstractmethod
-    def dumpDiskData(cls, data, filename, **kwargs):
+    def dump_disk_data(cls, data, filename, **kwargs):
         """Dump data to the disk.
 
         This method should not change any properties of any `Register`, which is why it is a class-method and
         not an instance-method. It merely takes `data`, processes it, and dumps it to disk.
 
-        Most use-cases prefer the instance-method `addDiskBlk`.
+        Most use-cases prefer the instance-method `add_disk_blk`.
 
         :param data: (any type) The raw data to dump.
         :param filename: (type `pathlib.Path`) The filename to dump to. You may edit this filename if
         necessary (such as by adding a suffix), but you must return the edited filename.
         :return: (type `pathlib.Path`) The actual filename of the data on the disk.
         """
 
     @classmethod
     @abstractmethod
-    def loadDiskData(cls, filename, **kwargs):
+    def load_disk_data(cls, filename, **kwargs):
         """Load raw data from the disk.
 
         This method should not change any properties of any `Register`, which is why it is a classmethod and
         not an instancemethod. It merely loads the data saved on the disk, processes it, and returns it.
 
         Most use-cases prefer the method `blk`.
 
@@ -1578,77 +1563,77 @@
         filename if necessary, such as by adding a suffix, but you must return the edited filename.
         :raises DataNotFoundError: If the data could not be loaded because it doesn't exist.
         :return: (any type) The data loaded from the disk.
         :return: (pathlib.Path) The exact path of the data saved to the disk.
         """
 
     @classmethod
-    def cleanDiskData(cls, filename, **kwargs):
+    def clean_disk_data(cls, filename, **kwargs):
         """Remove raw data from the disk.
 
         This method should not change any properties of any `Register`, which is why it is a classmethod and
         not an instancemethod. It merely removes the raw data.
 
-        Most use-cases prefer the method `rmvDiskBlk`.
+        Most use-cases prefer the method `rmv_disk_blk`.
 
         :param filename: (type `pathlib.Path`) Where to remove the raw data.
         :raises DataNotFoundError: If the data could not be cleaned because it doesn't exist.
         """
 
         if not filename.is_absolute():
             raise ValueError(NOT_ABSOLUTE_ERROR_MESSAGE.format(filename))
 
-        filename.unlink(missing_ok = False)
+        filename.unlink()
 
     @classmethod
     @abstractmethod
-    def withSuffix(cls, filename):
+    def with_suffix(cls, filename):
         """Adds a suffix to a filename and returns it.
 
         :param filename: (type `pathlib.Path`)
         :return: (type `pathlib.Path`)
         """
 
-    def addDiskBlk(self, blk, existsOk = False, retMetadata = False, **kwargs):
+    def add_disk_blk(self, blk, exists_ok = False, ret_metadata = False, **kwargs):
         """Save a `Block` to disk and link it with this `Register`.
 
         :param blk: (type `Block`)
-        :param retMetadata: (type `bool`, default `False`) Whether to return a `File_Metadata` object, which
+        :param ret_metadata: (type `bool`, default `False`) Whether to return a `File_Metadata` object, which
         contains file creation date/time and size of dumped data to the disk.
         :raises RegisterError: If a duplicate `Block` already exists in this `Register`.
         """
 
         #DEBUG : 1, 2, 3, 4, 5
 
-        self._checkOpenRaise("addDiskBlk")
-        self._checkReadwriteRaise("addDiskBlk")
+        self._check_open_raise("add_disk_blk")
+        self._check_readwrite_raise("add_disk_blk")
 
         if not isinstance(blk, Block):
             raise TypeError("`blk` must be of type `Block`.")
 
-        if not isinstance(existsOk, bool):
-            raise TypeError("`existsOk` must be of type `bool`.")
+        if not isinstance(exists_ok, bool):
+            raise TypeError("`exists_ok` must be of type `bool`.")
 
-        if not isinstance(retMetadata, bool):
-            raise TypeError("`retMetadata` must be of type `bool`.")
+        if not isinstance(ret_metadata, bool):
+            raise TypeError("`ret_metadata` must be of type `bool`.")
 
-        startnHead = blk.startn() // self._startnTailMod
+        startn_head = blk.startn() // self._startn_tail_mod
 
-        if startnHead != self._startnHead :
+        if startn_head != self._startn_head :
 
             raise IndexError(
                 "The `startn_` for the passed `Block` does not have the correct head:\n"
-                f"`tailLen`       : {self._startnTailLength}\n"
-                f"expected `head` : {self._startnHead}\n"
+                f"`tail_len`       : {self._startn_tail_length}\n"
+                f"expected `head` : {self._startn_head}\n"
                 f"`startn_`       : {blk.startn()}\n"
-                f"`startn_` head  : {startnHead}\n"
-                "Please see the method `setStartnInfo` to troubleshoot this error."
+                f"`startn_` head  : {startn_head}\n"
+                "Please see the method `set_startn_info` to troubleshoot this error."
             )
 
-        if len(blk) > self._maxLength:
+        if len(blk) > self._max_length:
             raise ValueError
 
         if _debug == 1:
             raise KeyboardInterrupt
 
         txn = None
         filename = None
@@ -1656,114 +1641,119 @@
         if _debug == 2:
             raise KeyboardInterrupt
 
         try:
 
             with ReversibleTransaction(self._db).begin(write = True) as txn:
 
-                filename = self._addDiskBlkTxn(blk, txn)
+                filename = self._add_disk_blk_txn(blk, txn)
 
                 if _debug == 3:
                     raise KeyboardInterrupt
 
             if _debug == 4:
                 raise KeyboardInterrupt
 
-            type(self).dumpDiskData(blk.segment(), filename, **kwargs)
+            type(self).dump_disk_data(blk.segment(), filename, **kwargs)
 
             if _debug == 5:
                 raise KeyboardInterrupt
 
         except BaseException as e:
 
-            if not isinstance(e, RegisterError) or not existsOk or not "exist" in str(e):
+            if not isinstance(e, RegisterError) or not exists_ok or not "exist" in str(e):
 
                 try:
 
                     if filename is not None:
-                        filename.unlink(missing_ok = True)
+
+                        try:
+                            filename.unlink()
+
+                        except FileNotFoundError:
+                            pass
 
                     if txn is not None:
 
                         with self._db.begin(write = True) as txn_:
                             txn.reverse(txn_)
 
                 except:
                     raise RegisterRecoveryError("Could not successfully recover from a failed disk `Block` add!") from e
 
                 else:
 
                     if isinstance(e, lmdb.MapFullError):
-                        raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._dbMapSize)) from e
+                        raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
 
                     else:
                         raise e
 
-        if retMetadata:
-            return self.blkMetadata(blk.apri(), blk.startn(), len(blk), False)
+        if ret_metadata:
+            return self.blk_metadata(blk.apri(), blk.startn(), len(blk), False)
 
         else:
             return None
 
-    def appendDiskBlk(self, blk, existsOk = False, retMetadata = False, **kwargs):
+    def append_disk_blk(self, blk, exists_ok = False, ret_metadata = False, **kwargs):
         """Add a `Block` to disk and link it with this `Register`.
 
         If no disk `Block`s with the same `ApriInfo` as `blk` have previously been added to disk, then `blk` will be
-        added to this `Register` via the method `addDiskBlk`. If not, then `startn_` will be set to one more than the
+        added to this `Register` via the method `add_disk_blk`. If not, then `startn_` will be set to one more than the
         largest index among all disk `Block`s with the same `ApriInfo` as `blk`.
 
         :param blk: (type `Block`)
-        :param retMetadata: (type `bool`, default `False`) Whether to return a `File_Metadata` object, which
+        :param ret_metadata: (type `bool`, default `False`) Whether to return a `File_Metadata` object, which
         contains file creation date/time and size of dumped data to the disk.
         :raises RegisterError: If a duplicate `Block` already exists in this `Register`.
         """
 
         if not isinstance(blk, Block):
             raise TypeError("`blk` must be of type `Block`.")
 
-        if not isinstance(existsOk, bool):
-            raise TypeError("`existsOk` must be of type `bool`.")
+        if not isinstance(exists_ok, bool):
+            raise TypeError("`exists_ok` must be of type `bool`.")
 
-        if not isinstance(retMetadata, bool):
-            raise TypeError("`retMetadata` must be of type `bool`.")
+        if not isinstance(ret_metadata, bool):
+            raise TypeError("`ret_metadata` must be of type `bool`.")
 
-        if self.numBlks(blk.apri(), diskonly = True) == 0:
-            return self.addDiskBlk(blk, existsOk, retMetadata, **kwargs)
+        if self.num_blks(blk.apri(), diskonly = True) == 0:
+            return self.add_disk_blk(blk, exists_ok, ret_metadata, **kwargs)
 
         else:
 
             startn = 0
 
-            for key, _ in self._iterDiskBlkPairs(_BLK_KEY_PREFIX, blk.apri(), None):
+            for key, _ in self._iter_disk_blk_pairs(_BLK_KEY_PREFIX, blk.apri(), None):
 
-                _, _startn, _length = self._convertDiskBlockKey(_BLK_KEY_PREFIX_LEN, key)
+                _, _startn, _length = self._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, key)
 
                 if startn < _startn + _length:
                     startn = _startn + _length
 
-            blk.setStartn(startn)
-            return self.addDiskBlk(blk, existsOk, retMetadata, **kwargs)
+            blk.set_startn(startn)
+            return self.add_disk_blk(blk, exists_ok, ret_metadata, **kwargs)
 
-    def rmvDiskBlk(self, apri, startn = None, length = None, missingOk = False, recursively = False, **kwargs):
+    def rmv_disk_blk(self, apri, startn = None, length = None, missing_ok = False, recursively = False, **kwargs):
         """Delete a disk `Block` and unlink it with this `Register`.
 
         :param apri: (type `ApriInfo`)
-        :param startn_: (type `int`) Non-negative.
-        :param length_: (type `int`) Non-negative.
+        :param startn: (type `int`) Non-negative.
+        :param length: (type `int`) Non-negative.
         :param recursively: (type `bool`)
         """
 
         # DEBUG : 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17
 
-        self._checkOpenRaise("rmvDiskBlk")
-        self._checkReadwriteRaise("rmvDiskBlk")
-        startn, length = Register._checkApriStartnLengthRaise(apri, startn, length)
+        self._check_open_raise("rmv_disk_blk")
+        self._check_readwrite_raise("rmv_disk_blk")
+        startn, length = Register._check_apri_startn_length_raise(apri, startn, length)
 
         try:
-            startn_, length_ = self._resolveStartnLength(apri, startn, length, True)
+            startn_, length_ = self._resolve_startn_length(apri, startn, length, True)
 
         except DataNotFoundError:
             pass
 
         else:
 
             if _debug == 1:
@@ -1782,58 +1772,63 @@
                     raise KeyboardInterrupt
 
                 with ReversibleTransaction(self._db).begin(write = True) as txn:
 
                     if _debug == 4:
                         raise KeyboardInterrupt
 
-                    blkFilename, comprFilename = self._rmvDiskBlkTxn(apri, startn_, length_, txn)
+                    blkFilename, comprFilename = self._rmv_disk_blk_txn(apri, startn_, length_, txn)
 
                     if _debug == 5:
                         raise KeyboardInterrupt
 
                 if _debug == 6:
                     raise KeyboardInterrupt
 
-                if not isDeletable(blkFilename):
+                if not is_deletable(blkFilename):
                     raise OSError(f"Cannot delete `Block` file `{str(blkFilename)}`.")
 
                 if _debug == 7:
                     raise KeyboardInterrupt
 
-                if comprFilename is not None and not isDeletable(comprFilename):
+                if comprFilename is not None and not is_deletable(comprFilename):
                     raise OSError(f"Cannot delete compressed `Block` file `{str(comprFilename)}`.")
 
                 if _debug == 8:
                     raise KeyboardInterrupt
 
                 if comprFilename is not None:
 
-                    blkFilename.unlink(missing_ok = False)
+                    blkFilename.unlink()
 
                     if _debug == 9:
                         raise KeyboardInterrupt
 
-                    comprFilename.unlink(missing_ok = False)
+                    comprFilename.unlink()
 
                 else:
-                    type(self).cleanDiskData(blkFilename, **kwargs)
+                    type(self).clean_disk_data(blkFilename, **kwargs)
 
                 return
 
             except BaseException as e:
 
                 FAIL_NO_RECOVER_ERROR_MESSAGE = "Could not successfully recover from a failed disk `Block` remove!"
 
                 try:
 
                     if comprFilename is not None:
 
                         if blkFilename is not None and comprFilename.exists():
-                            blkFilename.touch(exist_ok=True)
+
+                            try:
+                                blkFilename.touch()
+
+                            except FileExistsError:
+                                pass
 
                         else:
                             raise RegisterRecoveryError(FAIL_NO_RECOVER_ERROR_MESSAGE) from e
 
                     elif blkFilename is not None and not blkFilename.exists():
                         raise RegisterRecoveryError(FAIL_NO_RECOVER_ERROR_MESSAGE) from e
 
@@ -1847,139 +1842,139 @@
 
                 except:
                     raise RegisterRecoveryError(FAIL_NO_RECOVER_ERROR_MESSAGE) from e
 
                 else:
 
                     if isinstance(e, lmdb.MapFullError):
-                        raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._dbMapSize)) from e
+                        raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
 
                     else:
                         raise e
 
         if recursively:
 
-            for subreg in self._iterSubregs():
+            for subreg in self._iter_subregs():
 
-                with subreg._recursiveOpen(False) as subreg:
+                with subreg._recursive_open(False) as subreg:
 
                     try:
-                        subreg.rmvDiskBlk(apri, startn, length, False, True, **kwargs)
+                        subreg.rmv_disk_blk(apri, startn, length, False, True, **kwargs)
                         return
 
                     except DataNotFoundError:
                         pass
 
-        if not missingOk:
-            raise DataNotFoundError(_blkNotFoundErrMsg(True, apri, None, startn, length))
+        if not missing_ok:
+            raise DataNotFoundError(_blk_not_found_err_msg(True, apri, None, startn, length))
 
-    def blkMetadata(self, apri, startn = None, length = None, recursively = False):
+    def blk_metadata(self, apri, startn = None, length = None, recursively = False):
 
-        self._checkOpenRaise("blkMetadata")
+        self._check_open_raise("blk_metadata")
 
-        startn, length = Register._checkApriStartnLengthRaise(apri, startn, length)
+        startn, length = Register._check_apri_startn_length_raise(apri, startn, length)
 
         if not isinstance(recursively, bool):
             raise TypeError("`recursively` must be of type `bool`.")
 
-        startn_, length_ = self._resolveStartnLength(apri, startn, length, True)
+        startn_, length_ = self._resolve_startn_length(apri, startn, length, True)
 
         try:
-            blk_key, compressed_key = self._checkBlkCompressedKeysRaise(None, None, apri, None, startn_, length_)
+            blk_key, compressed_key = self._check_blk_compressed_keys_raise(None, None, apri, None, startn_, length_)
 
         except DataNotFoundError:
             pass
 
         else:
-            blk_filename, compressed_filename = self._checkBlkCompressedFilesRaise(
+            blk_filename, compressed_filename = self._check_blk_compressed_files_raise(
                 blk_key, compressed_key, apri, startn_, length_
             )
 
             if compressed_filename is not None:
-                return FileMetadata.fromPath(compressed_filename)
+                return FileMetadata.from_path(compressed_filename)
 
             else:
-                return FileMetadata.fromPath(blk_filename)
+                return FileMetadata.from_path(blk_filename)
 
         if recursively:
 
-            for subreg in self._iterSubregs():
+            for subreg in self._iter_subregs():
 
-                with subreg._recursiveOpen(True) as subreg:
+                with subreg._recursive_open(True) as subreg:
 
                     try:
-                        return subreg.blkMetadata(apri, startn_, length_, True)
+                        return subreg.blk_metadata(apri, startn_, length_, True)
 
                     except DataNotFoundError:
                         pass
 
         raise DataNotFoundError(
-            _blkNotFoundErrMsg(True, apri, None, startn, length)
+            _blk_not_found_err_msg(True, apri, None, startn, length)
         )
 
-    def compress(self, apri, startn = None, length = None, compressionLevel = 6, retMetadata = False):
+    def compress(self, apri, startn = None, length = None, compression_level = 6, ret_metadata = False):
         """Compress a `Block`.
 
         :param apri: (type `ApriInfo`)
         :param startn: (type `int`) Non-negative.
         :param length: (type `int`) Non-negative.
-        :param compressionLevel: (type `int`, default 6) Between 0 and 9, inclusive. 0 is for the fastest compression,
+        :param compression_level: (type `int`, default 6) Between 0 and 9, inclusive. 0 is for the fastest compression,
         but lowest compression ratio; 9 is slowest, but highest ratio. See
         https://docs.python.org/3/library/zlib.html#zlib.compressobj for more information.
-        :param retMetadata: (type `bool`, default `False`) Whether to return a `File_Metadata` object that
+        :param ret_metadata: (type `bool`, default `False`) Whether to return a `File_Metadata` object that
         describes the compressed file.
         :raises CompressionError: If the `Block` is already compressed.
-        :return: (type `File_Metadata`) If `retMetadata is True`.
+        :return: (type `File_Metadata`) If `ret_metadata is True`.
         """
 
         # DEBUG : 1, 2, 3, 4
 
         _FAIL_NO_RECOVER_ERROR_MESSAGE = "Could not recover successfully from a failed disk `Block` compress!"
 
-        self._checkOpenRaise("compress")
+        self._check_open_raise("compress")
 
-        self._checkReadwriteRaise("compress")
+        self._check_readwrite_raise("compress")
 
-        startn, length = Register._checkApriStartnLengthRaise(apri, startn, length)
+        startn, length = Register._check_apri_startn_length_raise(apri, startn, length)
 
-        if not isInt(compressionLevel):
-            raise TypeError("`compressionLevel` must be of type `int`.")
+        if not is_int(compression_level):
+            raise TypeError("`compression_level` must be of type `int`.")
         else:
-            compressionLevel = int(compressionLevel)
+            compression_level = int(compression_level)
 
-        if not isinstance(retMetadata, bool):
-            raise TypeError("`retMetadata` must be of type `bool`.")
+        if not isinstance(ret_metadata, bool):
+            raise TypeError("`ret_metadata` must be of type `bool`.")
 
-        if not (0 <= compressionLevel <= 9):
-            raise ValueError("`compressionLevel` must be between 0 and 9, inclusive.")
+        if not (0 <= compression_level <= 9):
+            raise ValueError("`compression_level` must be between 0 and 9, inclusive.")
 
-        startn_, length_ = self._resolveStartnLength(apri, startn, length, True)
+        startn_, length_ = self._resolve_startn_length(apri, startn, length, True)
 
-        compressed_key = self._getDiskBlkKey(
+        compressed_key = self._get_disk_blk_key(
             _COMPRESSED_KEY_PREFIX, apri, None, startn_, length_, False
         )
 
-        blk_key, compressed_key = self._checkBlkCompressedKeysRaise(
+        blk_key, compressed_key = self._check_blk_compressed_keys_raise(
             None, compressed_key, apri, None, startn_, length_
         )
 
         with self._db.begin() as txn:
             compressed_val = txn.get(compressed_key)
 
         if compressed_val != _IS_NOT_COMPRESSED_VAL:
 
             raise CompressionError(
                 "The disk `Block` with the following data has already been compressed: " +
                 f"{str(apri)}, startn = {startn_}, length = {length_}"
             )
 
         with self._db.begin() as txn:
-            blk_filename = self._localDir / txn.get(blk_key).decode("ASCII")
+            blk_filename = self._local_dir / txn.get(blk_key).decode("ASCII")
 
-        compressed_filename = randomUniqueFilename(self._localDir, COMPRESSED_FILE_SUFFIX)
+        compressed_filename = random_unique_filename(self._local_dir, COMPRESSED_FILE_SUFFIX)
         compressed_val = compressed_filename.name.encode("ASCII")
 
         cleaned = False
 
         if _debug == 1:
             raise KeyboardInterrupt
 
@@ -1994,285 +1989,294 @@
 
             with zipfile.ZipFile(
 
                 compressed_filename,  # target filename
                 "x",  # zip mode (write, but don't overwrite)
                 zipfile.ZIP_DEFLATED,  # compression mode
                 True,  # use zip64
-                compressionLevel,
-                strict_timestamps=False  # change timestamps of old or new files
+                compression_level
 
             ) as compressed_fh:
 
                 compressed_fh.write(blk_filename, blk_filename.name)
 
                 if _debug == 3:
                     raise KeyboardInterrupt
 
             if _debug == 4:
                 raise KeyboardInterrupt
 
-            type(self).cleanDiskData(blk_filename)
+            type(self).clean_disk_data(blk_filename)
             cleaned = True
-            blk_filename.touch(exist_ok = False)
+            blk_filename.touch()
 
         except BaseException as e:
 
             try:
 
                 with self._db.begin(write = True) as txn:
                     txn.put(compressed_key, _IS_NOT_COMPRESSED_VAL)
 
                 if cleaned or not blk_filename.exists():
                     raise RegisterRecoveryError(_FAIL_NO_RECOVER_ERROR_MESSAGE)
 
                 else:
-                    compressed_filename.unlink(missing_ok = True)
+
+                    try:
+                        compressed_filename.unlink()
+
+                    except FileNotFoundError:
+                        pass
 
             except RegisterRecoveryError as ee:
                 raise ee
 
             except BaseException:
                 raise RegisterRecoveryError(_FAIL_NO_RECOVER_ERROR_MESSAGE)
 
             else:
 
                 if isinstance(e, lmdb.MapFullError):
-                    raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._dbMapSize)) from e
+                    raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
 
                 else:
                     raise e
 
-        if retMetadata:
-            return FileMetadata.fromPath(compressed_filename)
+        if ret_metadata:
+            return FileMetadata.from_path(compressed_filename)
 
         else:
             return None
 
-    def decompress(self, apri, startn = None, length = None, retMetadata = False):
+    def decompress(self, apri, startn = None, length = None, ret_metadata = False):
         """Decompress a `Block`.
 
         :param apri: (type `ApriInfo`)
         :param startn: (type `int`) Non-negative.
         :param length: (type `int`) Non-negative.
-        :param retMetadata: (type `bool`, default `False`) Whether to return a `File_Metadata` object that
+        :param ret_metadata: (type `bool`, default `False`) Whether to return a `File_Metadata` object that
         describes the decompressed file.
         :raise DecompressionError: If the `Block` is not compressed.
-        :return: (type `list`) If `retMetadata is True`.
+        :return: (type `list`) If `ret_metadata is True`.
         """
 
         # DEBUG : 1, 2, 3, 4
 
         _FAIL_NO_RECOVER_ERROR_MESSAGE = "Could not recover successfully from a failed disk `Block` decompress!"
 
-        self._checkOpenRaise("decompress")
+        self._check_open_raise("decompress")
 
-        self._checkReadwriteRaise("decompress")
+        self._check_readwrite_raise("decompress")
 
-        startn, length = Register._checkApriStartnLengthRaise(apri, startn, length)
+        startn, length = Register._check_apri_startn_length_raise(apri, startn, length)
 
-        if not isinstance(retMetadata, bool):
-            raise TypeError("`retMetadata` must be of type `bool`.")
+        if not isinstance(ret_metadata, bool):
+            raise TypeError("`ret_metadata` must be of type `bool`.")
 
-        startn_, length_ = self._resolveStartnLength(apri, startn, length, True)
+        startn_, length_ = self._resolve_startn_length(apri, startn, length, True)
 
-        blk_key, compressed_key = self._checkBlkCompressedKeysRaise(None, None, apri, None, startn_, length_)
+        blk_key, compressed_key = self._check_blk_compressed_keys_raise(None, None, apri, None, startn_, length_)
 
         with self._db.begin() as txn:
             compressed_val = txn.get(compressed_key)
 
         if compressed_val == _IS_NOT_COMPRESSED_VAL:
 
             raise DecompressionError(
                 "The disk `Block` with the following data is not compressed: " +
                 f"{str(apri)}, startn = {startn_}, length = {length_}"
             )
 
         with self._db.begin() as txn:
             blk_filename = txn.get(blk_key).decode("ASCII")
 
-        blk_filename = self._localDir / blk_filename
-        compressed_filename = self._localDir / compressed_val.decode("ASCII")
+        blk_filename = self._local_dir / blk_filename
+        compressed_filename = self._local_dir / compressed_val.decode("ASCII")
         deleted = False
 
-        if not isDeletable(blk_filename):
+        if not is_deletable(blk_filename):
             raise OSError(f"Cannot delete ghost file `{str(blk_filename)}`.")
 
-        if not isDeletable(compressed_filename):
+        if not is_deletable(compressed_filename):
             raise OSError(f"Cannot delete compressed file `{str(compressed_filename)}`.")
 
         if _debug == 1:
             raise KeyboardInterrupt
 
         try:
 
             with self._db.begin(write = True) as txn:
 
                 # delete ghost file
-                blk_filename.unlink(missing_ok = False)
+                blk_filename.unlink()
                 deleted = True
 
                 if _debug == 2:
                     raise KeyboardInterrupt
 
                 with zipfile.ZipFile(compressed_filename, "r") as compressed_fh:
 
-                    compressed_fh.extract(blk_filename.name, self._localDir)
+                    compressed_fh.extract(blk_filename.name, self._local_dir)
 
                     if _debug == 3:
                         raise KeyboardInterrupt
 
                 txn.put(compressed_key, _IS_NOT_COMPRESSED_VAL)
 
                 if _debug == 4:
                     raise KeyboardInterrupt
 
-                compressed_filename.unlink(missing_ok = False)
+                compressed_filename.unlink()
 
         except BaseException as e:
 
             try:
 
                 if not compressed_filename.is_file():
                     raise RegisterRecoveryError(_FAIL_NO_RECOVER_ERROR_MESSAGE)
 
                 elif deleted or not blk_filename.is_file():
 
-                    blk_filename.unlink(missing_ok = True)
-                    blk_filename.touch(exist_ok = False)
+                    try:
+                        blk_filename.unlink()
+
+                    except FileNotFoundError:
+                        pass
+
+                    blk_filename.touch()
 
             except RegisterRecoveryError as ee:
                 raise ee
 
             except BaseException:
                 raise RegisterRecoveryError(_FAIL_NO_RECOVER_ERROR_MESSAGE)
 
             else:
 
                 if isinstance(e, lmdb.MapFullError):
-                    raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._dbMapSize)) from e
+                    raise RegisterError(_MEMORY_FULL_ERROR_MESSAGE.format(self._db_map_size)) from e
 
                 else:
                     raise e
 
-        if retMetadata:
-            return FileMetadata.fromPath(blk_filename)
+        if ret_metadata:
+            return FileMetadata.from_path(blk_filename)
 
         else:
             return None
 
-    def isCompressed(self, apri, startn = None, length = None):
+    def is_compressed(self, apri, startn = None, length = None):
 
-        self._checkOpenRaise("isCompressed")
+        self._check_open_raise("is_compressed")
 
-        self._checkApriStartnLengthRaise(apri, startn, length)
+        self._check_apri_startn_length_raise(apri, startn, length)
 
-        startn_, length_ = self._resolveStartnLength(apri, startn, length, True)
+        startn_, length_ = self._resolve_startn_length(apri, startn, length, True)
 
         with self._db.begin() as txn:
             return txn.get(
-                self._getDiskBlkKey(_COMPRESSED_KEY_PREFIX, apri, None, startn_, length_, False, txn)
+                self._get_disk_blk_key(_COMPRESSED_KEY_PREFIX, apri, None, startn_, length_, False, txn)
             ) != _IS_NOT_COMPRESSED_VAL
 
-    # def setHashing(self, apri, hashing):
-    #     """Enable or disable automatic hashing for disk `Block`s with `apri`.
+    # def setHashing(self, info, hashing):
+    #     """Enable or disable automatic hashing for disk `Block`s with `info`.
     #
-    #     If `hashing` is set to `True`, then every disk `Block` with `apri` added to this `Register` will be hashed. A
+    #     If `hashing` is set to `True`, then every disk `Block` with `info` added to this `Register` will be hashed. A
     #     `Block` is hashed by calling `hash` on each of its entries. The hashes are saved to a hash-set on disk.
     #
-    #     If `hashing` is set to `False`, then all hashes associated to `apri` will be DELETED (if they exist) and no
+    #     If `hashing` is set to `False`, then all hashes associated to `info` will be DELETED (if they exist) and no
     #     future hashes are calculated.
     #
-    #     For best results, set hashing to `True` only before adding any disk `Block`s with `apri`.
+    #     For best results, set hashing to `True` only before adding any disk `Block`s with `info`.
     #
     #     :param hashing: (type `bool`)
     #     """
 
     #################################
     #    PROTEC DISK BLK METHODS    #
 
-    def _addDiskBlkTxn(self, blk, txn):
+    def _add_disk_blk_txn(self, blk, txn):
 
         # DEBUG : 6,7,8,9, 10
 
-        apris = [apri for _, apri in blk.apri().iterInnerInfo() if isinstance(apri, ApriInfo)]
+        apris = [apri for _, apri in blk.apri().iter_inner_info() if isinstance(apri, ApriInfo)]
 
         if _debug == 6:
             raise KeyboardInterrupt
 
         # this will create ID's if necessary
         for i, apri in enumerate(apris):
-            self._getIdByApri(apri, None, True, txn)
+            self._get_id_by_apri(apri, None, True, txn)
 
         if _debug == 7:
             raise KeyboardInterrupt
 
-        blkKey = self._getDiskBlkKey(
+        blk_key = self._get_disk_blk_key(
             _BLK_KEY_PREFIX,
             blk.apri(), None, blk.startn(), len(blk),
             False, txn
         )
 
-        if not lmdbHasKey(txn, blkKey):
+        if not lmdb_has_key(txn, blk_key):
 
-            filename = randomUniqueFilename(self._localDir, length=6)
+            filename = random_unique_filename(self._local_dir, length=6)
 
             if _debug == 8:
                 raise KeyboardInterrupt
 
-            filename = type(self).withSuffix(filename)
+            filename = type(self).with_suffix(filename)
 
             if _debug == 9:
                 raise KeyboardInterrupt
 
             filename_bytes = str(filename.name).encode("ASCII")
-            compressed_key = _COMPRESSED_KEY_PREFIX + blkKey[_BLK_KEY_PREFIX_LEN:]
+            compressed_key = _COMPRESSED_KEY_PREFIX + blk_key[_BLK_KEY_PREFIX_LEN:]
 
-            txn.put(blkKey, filename_bytes)
+            txn.put(blk_key, filename_bytes)
             txn.put(compressed_key, _IS_NOT_COMPRESSED_VAL)
 
             if _debug == 10:
                 raise KeyboardInterrupt
 
             if len(blk) == 0:
 
                 warnings.warn(
                     "Added a length_ 0 disk `Block` to this `Register`.\n" +
                     f"`Register` msg: {str(self)}\n" +
                     f"`Block`: {str(blk)}\n" +
-                    f"`Register` location: {str(self._localDir)}"
+                    f"`Register` location: {str(self._local_dir)}"
                 )
 
             return filename
 
         else:
 
             raise RegisterError(
                 f"Duplicate `Block` with the following data already exists in this `Register`: " +
                 f"{str(blk.apri())}, startn_ = {blk.startn()}, length_ = {len(blk)}."
             )
 
-    def _rmvDiskBlkTxn(self, apri, startn, length, txn):
+    def _rmv_disk_blk_txn(self, apri, startn, length, txn):
 
         if _debug == 12:
             raise KeyboardInterrupt
 
         # raises DataNotFoundError
-        self._getIdByApri(apri, None, False, txn)
+        self._get_id_by_apri(apri, None, False, txn)
 
         if _debug == 13:
             raise KeyboardInterrupt
 
         # raises RegisterError and DataNotFoundError
-        blk_key, compressed_key = self._checkBlkCompressedKeysRaise(None, None, apri, None, startn, length, txn)
+        blk_key, compressed_key = self._check_blk_compressed_keys_raise(None, None, apri, None, startn, length, txn)
 
         if _debug == 14:
             raise KeyboardInterrupt
 
-        blkFilename, comprFilename = self._checkBlkCompressedFilesRaise(
+        blk_filename, compr_filename = self._check_blk_compressed_files_raise(
             blk_key, compressed_key, apri, startn, length, txn
         )
 
         if _debug == 15:
             raise KeyboardInterrupt
 
         txn.delete(compressed_key)
@@ -2281,176 +2285,197 @@
             raise KeyboardInterrupt
 
         txn.delete(blk_key)
 
         if _debug == 17:
             raise KeyboardInterrupt
 
-        return blkFilename, comprFilename
+        return blk_filename, compr_filename
 
-    def _getDiskBlkKey(self, prefix, apri, apriJson, startn, length, missingOk, txn = None):
+    def _get_disk_blk_key(self, prefix, apri, apri_json, startn, length, missing_ok, txn = None):
         """Get the database key for a disk `Block`.
 
-        One of `apri` and `apriJson` can be `None`, but not both. If both are not `None`, then `apri` is used.
-        `self._db` must be opened by the caller. This method only queries the database to obtain the `apri` ID.
+        One of `info` and `apri_json` can be `None`, but not both. If both are not `None`, then `info` is used.
+        `self._db` must be opened by the caller. This method only queries the database to obtain the `info` ID.
 
-        If `missingOk is True` and an ID for `apri` does not already exist, then a new one will be created. If
-        `missingOk is False` and an ID does not already exist, then an error is raised.
+        If `missing_ok is True` and an ID for `info` does not already exist, then a new one will be created. If
+        `missing_ok is False` and an ID does not already exist, then an error is raised.
 
         :param prefix: (type `bytes`)
         :param apri: (type `ApriInfo`)
-        :param apriJson: (types `bytes`)
+        :param apri_json: (types `bytes`)
         :param startn: (type `int`) The start index of the `Block`.
         :param length: (type `int`) The length_ of the `Block`.
-        :param missingOk: (type `bool`)
+        :param missing_ok: (type `bool`)
         :param txn: (type `lmbd.Transaction`, default `None`) The transaction to query. If `None`, then use open a new
         transaction and commit it after this method resolves.
-        :raises DataNotFoundError: If `missingOk is False` and `apri` is not known to this `Register`.
+        :raises DataNotFoundError: If `missing_ok is False` and `info` is not known to this `Register`.
         :return: (type `bytes`)
         """
 
-        if apri is None and apriJson is None:
+        if apri is None and apri_json is None:
             raise ValueError
 
-        _id = self._getIdByApri(apri, apriJson, missingOk, txn)
-        tail = startn % self._startnTailMod
-        tail = f"{tail:0{self._startnTailLength}d}".encode("ASCII")
-        opLength = self._maxLength - length
-        opLength = f"{opLength:0{self._lengthLength}d}".encode("ASCII")
+        id_ = self._get_id_by_apri(apri, apri_json, missing_ok, txn)
+        tail = startn % self._startn_tail_mod
+        tail = f"{tail:0{self._startn_tail_length}d}".encode("ASCII")
+        op_length = self._max_length - length
+        op_length = f"{op_length:0{self._length_length}d}".encode("ASCII")
 
         return (
                 prefix   +
-                _id      + _KEY_SEP +
+                id_      + _KEY_SEP +
                 tail     + _KEY_SEP +
-                opLength
+                op_length
         )
 
-    def _numDiskBlksTxn(self, apri, txn):
+    def _num_disk_blks_txn(self, apri, txn):
 
         try:
 
-            return lmdbCountKeys(
+            return lmdb_count_keys(
                 txn,
-                _BLK_KEY_PREFIX + self._getIdByApri(apri, None, False) + _KEY_SEP
+                _BLK_KEY_PREFIX + self._get_id_by_apri(apri, None, False) + _KEY_SEP
             )
 
         except DataNotFoundError:
             return 0
 
-    def _iterDiskBlkPairs(self, prefix, apri, apriJson, txn = None):
+    def _iter_disk_blk_pairs(self, prefix, apri, apri_json, txn = None):
         """Iterate over key-value pairs for block entries.
 
         :param prefix: (type `bytes`)
         :param apri: (type `ApriInfo`)
-        :param apriJson: (type `bytes`)
+        :param apri_json: (type `bytes`)
         :param txn: (type `lmbd.Transaction`, default `None`) The transaction to query. If `None`, then use open a new
         transaction and commit it after this method resolves.
-        :raise DataNotFoundError: If `apri` is not a disk `ApriInfo`.
+        :raise DataNotFoundError: If `info` is not a disk `ApriInfo`.
         :return: (type `bytes`) key
         :return: (type `bytes`) val
         """
 
         try:
-            prefix += self._getIdByApri(apri, apriJson, False, txn)
+            prefix += self._get_id_by_apri(apri, apri_json, False, txn)
 
         except DataNotFoundError:
             pass
 
         else:
 
             prefix += _KEY_SEP
 
-            with lmdbPrefixIter(txn if txn is not None else self._db, prefix) as it:
+            with lmdb_prefix_iter(txn if txn is not None else self._db, prefix) as it:
                 yield from it
 
     @staticmethod
-    def _splitDiskBlockKey(prefixLen, key):
-        return tuple(key[prefixLen:].split(_KEY_SEP))
+    def _split_disk_block_key(prefix_len, key):
+        return tuple(key[prefix_len:].split(_KEY_SEP))
 
     @staticmethod
-    def _joinDiskBlockData(prefix, apriJson, startnBytes, lenBytes):
+    def _join_disk_block_data(prefix, apri_json, startn_bytes, len_bytes):
         return (
                 prefix +
-                apriJson + _KEY_SEP +
-                startnBytes + _KEY_SEP +
-                lenBytes
+                apri_json + _KEY_SEP +
+                startn_bytes + _KEY_SEP +
+                len_bytes
         )
 
-    def _convertDiskBlockKey(self, prefixLen, key, apri = None, txn = None):
+    def _convert_disk_block_key(self, prefix_len, key, apri = None, txn = None):
         """
-        :param prefixLen: (type `int`) Positive.
+        :param prefix_len: (type `int`) Positive.
         :param key: (type `bytes`)
-        :param apri: (type `ApriInfo`, default None) If `None`, the relevant `apri` is acquired through a database
+        :param apri: (type `ApriInfo`, default None) If `None`, the relevant `info` is acquired through a database
         query.
         :param txn: (type `lmbd.Transaction`, default `None`) The transaction to query. If `None`, then use open a new
         transaction and commit it after this method resolves.
         :return: (type `ApriInfo`)
-        :return (type `int`) startn_
-        :return (type `int`) length_, non-negative
+        :return (type `int`) startn
+        :return (type `int`) length, non-negative
         """
 
-        apri_id, startn_bytes, opLength_bytes = Register._splitDiskBlockKey(prefixLen, key)
+        apri_id, startn_bytes, op_length_bytes = Register._split_disk_block_key(prefix_len, key)
+
+        commit = apri is None and txn is None
+
+        if commit:
+            txn = self._db.begin()
+
+        try:
 
-        if apri is None:
+            if apri is None:
 
-            apri_json = self._getApriJsonById(apri_id, txn)
-            apri = ApriInfo.fromJson(apri_json.decode("ASCII"))
+                apri_json = self._get_apri_json_by_id(apri_id, txn)
+                apri = relational_decode_info(self, ApriInfo, apri_json, txn)
+
+        finally:
+
+            if commit:
+                txn.commit()
 
         return (
             apri,
-            int(startn_bytes.decode("ASCII")) + self._startnHead * self._startnTailMod,
-            self._maxLength - int(opLength_bytes.decode("ASCII"))
+            int(startn_bytes.decode("ASCII")) + self._startn_head * self._startn_tail_mod,
+            self._max_length - int(op_length_bytes.decode("ASCII"))
         )
 
-    def _checkBlkCompressedKeysRaise(self, blkKey, compressedKey, apri, apriJson, startn, length, txn = None):
+    def _check_blk_compressed_keys_raise(self, blk_key, compressed_key, apri, apri_json, startn, length, txn = None):
+
+        if compressed_key is None and blk_key is None:
+            compressed_key = self._get_disk_blk_key(_COMPRESSED_KEY_PREFIX, apri, apri_json, startn, length, False, txn)
+
+        if blk_key is not None and compressed_key is None:
+            compressed_key = _COMPRESSED_KEY_PREFIX + blk_key[_BLK_KEY_PREFIX_LEN:]
+
+        elif compressed_key is not None and blk_key is None:
+            blk_key = _BLK_KEY_PREFIX + compressed_key[_COMPRESSED_KEY_PREFIX_LEN:]
+
+        commit = txn is None
 
-        if compressedKey is None and blkKey is None:
-            compressedKey = self._getDiskBlkKey(_COMPRESSED_KEY_PREFIX, apri, apriJson, startn, length, False, txn)
+        if commit:
+            txn = self._db.begin()
 
-        if blkKey is not None and compressedKey is None:
-            compressedKey = _COMPRESSED_KEY_PREFIX + blkKey[_BLK_KEY_PREFIX_LEN:]
+        try:
 
-        elif compressedKey is not None and blkKey is None:
-            blkKey = _BLK_KEY_PREFIX + compressedKey[_COMPRESSED_KEY_PREFIX_LEN:]
+            if apri is None:
+                apri = relational_decode_info(self, ApriInfo, apri_json, txn)
 
-        if apri is None:
-            apri = ApriInfo.fromJson(apriJson.decode("ASCII"))
+            has_blk_key = lmdb_has_key(txn, blk_key)
+            has_compr_key = lmdb_has_key(txn, compressed_key)
 
-        if txn is None:
-            txn = self._db
+        finally:
 
-        hasBlkKey = lmdbHasKey(txn, blkKey)
-        hasComprKey = lmdbHasKey(txn, compressedKey)
+            if commit:
+                txn.commit()
 
-        if (not hasBlkKey and hasComprKey) or (hasBlkKey and not hasComprKey):
+        if (not has_blk_key and has_compr_key) or (has_blk_key and not has_compr_key):
             raise RegisterError("Uncompressed/compressed `Block` key mismatch.")
 
-        if not hasBlkKey:
+        if not has_blk_key:
             raise DataNotFoundError(
-                _blkNotFoundErrMsg(True, apri, None, startn, length)
+                _blk_not_found_err_msg(True, apri, None, startn, length)
             )
 
-        return blkKey, compressedKey
+        return blk_key, compressed_key
 
-    def _checkBlkCompressedFilesRaise(self, blkKey, compressedKey, apri, startn, length, txn = None):
+    def _check_blk_compressed_files_raise(self, blk_key, compressed_key, apri, startn, length, txn = None):
 
         commit = txn is None
 
         try:
 
             if commit:
                 txn = self._db.begin()
 
-            blk_val = txn.get(blkKey)
-            compressed_val = txn.get(compressedKey)
-            blk_filename = self._localDir / blk_val.decode("ASCII")
+            blk_val = txn.get(blk_key)
+            compressed_val = txn.get(compressed_key)
+            blk_filename = self._local_dir / blk_val.decode("ASCII")
 
             if compressed_val != _IS_NOT_COMPRESSED_VAL:
 
-                compressed_filename = self._localDir / compressed_val.decode("ASCII")
+                compressed_filename = self._local_dir / compressed_val.decode("ASCII")
 
                 if not compressed_filename.exists() or not blk_filename.exists():
 
                     raise RegisterError(
                         "Compressed `Block` file or ghost file seems to be missing!"
                     )
 
@@ -2468,26 +2493,26 @@
 
         finally:
 
             if commit:
                 txn.commit()
 
     @staticmethod
-    def _checkApriStartnLengthRaise(apri, startn, length):
+    def _check_apri_startn_length_raise(apri, startn, length):
 
         if not isinstance(apri, ApriInfo):
-            raise TypeError("`apri` must be of type `ApriInfo`")
+            raise TypeError("`info` must be of type `ApriInfo`")
 
-        if not isInt(startn) and startn is not None:
+        if not is_int(startn) and startn is not None:
             raise TypeError("startn_` must be an `int`")
 
         elif startn is not None:
             startn = int(startn)
 
-        if not isInt(length) and length is not None:
+        if not is_int(length) and length is not None:
             raise TypeError("`length_` must be an `int`")
 
         elif length is not None:
             length = int(length)
 
         if startn is not None and startn < 0:
             raise ValueError("`startn_` must be non-negative")
@@ -2496,172 +2521,172 @@
             raise ValueError("`length_` must be non-negative")
 
         return startn, length
 
     #################################
     #    PUBLIC RAM BLK METHODS     #
 
-    def addRamBlk(self, blk):
+    def add_ram_blk(self, blk):
 
-        self._checkOpenRaise("addRamBlk")
+        self._check_open_raise("add_ram_blk")
 
         if not isinstance(blk, Block):
             raise TypeError("`blk` must be of type `Block`.")
 
-        if blk.apri() not in self._ramBlks.keys():
-            self._ramBlks[blk.apri()] = [blk]
+        if blk.apri() not in self._ram_blks.keys():
+            self._ram_blks[blk.apri()] = [blk]
 
-        elif len(self._ramBlks[blk.apri()]) == 0:
-            self._ramBlks[blk.apri()].append(blk)
+        elif len(self._ram_blks[blk.apri()]) == 0:
+            self._ram_blks[blk.apri()].append(blk)
 
         else:
 
-            for i, blk_ in enumerate(self._ramBlks[blk.apri()]):
+            for i, blk_ in enumerate(self._ram_blks[blk.apri()]):
 
                 if blk_ is blk:
                     break
 
                 elif blk.startn() < blk_.startn() or (blk.startn() == blk_.startn() and len(blk) > len(blk_)):
 
-                    self._ramBlks[blk.apri()].insert(i, blk)
+                    self._ram_blks[blk.apri()].insert(i, blk)
                     break
 
             else:
-                self._ramBlks[blk.apri()].append(blk)
+                self._ram_blks[blk.apri()].append(blk)
 
-    def rmvRamBlk(self, blk):
+    def rmv_ram_blk(self, blk):
 
-        self._checkOpenRaise("addRamBlk")
+        self._check_open_raise("add_ram_blk")
 
         if not isinstance(blk, Block):
             raise TypeError("`blk` must be of type `Block`.")
 
-        if blk.apri() not in self._ramBlks.keys():
+        if blk.apri() not in self._ram_blks.keys():
             raise DataNotFoundError(f"No RAM `Block` found with the following data: {str(blk.apri())}.")
 
-        for i, blk_ in enumerate(self._ramBlks[blk.apri()]):
+        for i, blk_ in enumerate(self._ram_blks[blk.apri()]):
 
             if blk_ is blk:
 
-                del self._ramBlks[blk.apri()][i]
+                del self._ram_blks[blk.apri()][i]
 
-                if len(self._ramBlks[blk.apri()]) == 0:
-                    del self._ramBlks[blk.apri()]
+                if len(self._ram_blks[blk.apri()]) == 0:
+                    del self._ram_blks[blk.apri()]
 
                 return
 
         else:
             raise DataNotFoundError(f"No matching RAM disk `Block` found.")
 
-    def rmvAllRamBlks(self):
+    def rmv_all_ram_blks(self):
 
-        self._checkOpenRaise("rmvAllRamBlks")
-        self._ramBlks = {}
+        self._check_open_raise("rmv_all_ram_blks")
+        self._ram_blks = {}
 
     #################################
     #    PROTEC RAM BLK METHODS     #
 
     #################################
     # PUBLIC RAM & DISK BLK METHODS #
 
-    def blkByN(self, apri, n, diskonly = False, recursively = False, retMetadata = False, **kwargs):
+    def blk_by_n(self, apri, n, diskonly = False, recursively = False, ret_metadata = False, **kwargs):
 
-        self._checkOpenRaise("blkByN")
+        self._check_open_raise("blk_by_n")
 
         if not isinstance(apri, ApriInfo):
-            raise TypeError("`apri` must be of type `ApriInfo`.")
+            raise TypeError("`info` must be of type `ApriInfo`.")
 
-        if not isInt(n):
+        if not is_int(n):
             raise TypeError("`n` must be of type `int`.")
 
         else:
             n = int(n)
 
         if not isinstance(diskonly, bool):
             raise TypeError("`diskonly` must be of type `bool`.")
 
         if not isinstance(recursively, bool):
             raise TypeError("`recursively` must be of type `bool`.")
 
-        if not isinstance(retMetadata, bool):
-            raise TypeError("`retMetadata` must be of type `bool`.")
+        if not isinstance(ret_metadata, bool):
+            raise TypeError("`ret_metadata` must be of type `bool`.")
 
         if n < 0:
             raise IndexError("`n` must be non-negative.")
 
         try:
-            self._checkKnownApri(apri)
+            self._check_known_apri(apri)
 
         except DataNotFoundError:
 
             if not recursively:
                 raise
 
         else:
 
             for startn, length in self.intervals(apri, combine = False, diskonly = diskonly, recursively = False):
 
                 if startn <= n < startn + length:
-                    return self.blk(apri, startn, length, diskonly, False, retMetadata, **kwargs)
+                    return self.blk(apri, startn, length, diskonly, False, ret_metadata, **kwargs)
 
         if recursively:
 
-            for subreg in self._iterSubregs():
+            for subreg in self._iter_subregs():
 
-                with subreg._recursiveOpen(True) as subreg:
+                with subreg._recursive_open(True) as subreg:
 
                     try:
-                        return subreg.blkByN(apri, n, diskonly, True, retMetadata, **kwargs)
+                        return subreg.blk_by_n(apri, n, diskonly, True, ret_metadata, **kwargs)
 
                     except DataNotFoundError:
                         pass
 
-        raise DataNotFoundError(_blkNotFoundErrMsg(diskonly, apri, n))
+        raise DataNotFoundError(_blk_not_found_err_msg(diskonly, apri, n))
 
-    def blk(self, apri, startn = None, length = None, diskonly = False, recursively = False, retMetadata = False, **kwargs):
+    def blk(self, apri, startn = None, length = None, diskonly = False, recursively = False, ret_metadata = False, **kwargs):
 
-        self._checkOpenRaise("blk")
+        self._check_open_raise("blk")
 
-        startn, length = Register._checkApriStartnLengthRaise(apri, startn, length)
+        startn, length = Register._check_apri_startn_length_raise(apri, startn, length)
 
         if not isinstance(diskonly, bool):
             raise TypeError("`diskonly` must be of type `bool`.")
 
         if not isinstance(recursively, bool):
             raise TypeError("`recursively` must be of type `bool`.")
 
-        if not isinstance(retMetadata, bool):
-            raise TypeError("`retMetadata` must be of type `bool`.")
+        if not isinstance(ret_metadata, bool):
+            raise TypeError("`ret_metadata` must be of type `bool`.")
 
         try:
-            self._checkKnownApri(apri)
+            self._check_known_apri(apri)
 
         except DataNotFoundError:
 
             if not recursively:
                 raise
 
         else:
 
-            startn_, length_ = self._resolveStartnLength(apri, startn, length, diskonly)
+            startn_, length_ = self._resolve_startn_length(apri, startn, length, diskonly)
 
-            if not diskonly and apri in self._ramBlks.keys():
+            if not diskonly and apri in self._ram_blks.keys():
 
-                for blk in self._ramBlks[apri]:
+                for blk in self._ram_blks[apri]:
 
                     if blk.startn() == startn_ and len(blk) == length_:
 
-                        if retMetadata:
+                        if ret_metadata:
                             return blk, None
 
                         else:
                             return blk
 
             try:
-                blk_key, compressed_key = self._checkBlkCompressedKeysRaise(None, None, apri, None, startn_, length_)
+                blk_key, compressed_key = self._check_blk_compressed_keys_raise(None, None, apri, None, startn_, length_)
 
             except DataNotFoundError:
                 pass
 
             else:
 
                 with self._db.begin() as txn:
@@ -2669,136 +2694,136 @@
                     if txn.get(compressed_key) != _IS_NOT_COMPRESSED_VAL:
                         raise CompressionError(
                             "Could not load disk `Block` with the following data because the `Block` is compressed. "
                             "Please call the `Register` method `decompress` first before loading the data.\n" +
                             f"{apri}, startn = {startn_}, length = {length_}"
                         )
 
-                blk_filename, _ = self._checkBlkCompressedFilesRaise(blk_key, compressed_key, apri, startn_, length_)
-                blk_filename = self._localDir / blk_filename
-                data = type(self).loadDiskData(blk_filename, **kwargs)
+                blk_filename, _ = self._check_blk_compressed_files_raise(blk_key, compressed_key, apri, startn_, length_)
+                blk_filename = self._local_dir / blk_filename
+                data = type(self).load_disk_data(blk_filename, **kwargs)
                 blk = Block(data, apri, startn_)
 
-                if retMetadata:
-                    return blk, FileMetadata.fromPath(blk_filename)
+                if ret_metadata:
+                    return blk, FileMetadata.from_path(blk_filename)
 
                 else:
                     return blk
 
         if recursively:
 
-            for subreg in self._iterSubregs():
+            for subreg in self._iter_subregs():
 
-                with subreg._recursiveOpen(True) as subreg:
+                with subreg._recursive_open(True) as subreg:
 
                     try:
-                        return subreg.blk(apri, startn, length, retMetadata, retMetadata=True)
+                        return subreg.blk(apri, startn, length, ret_metadata, ret_metadata=True)
 
                     except DataNotFoundError:
                         pass
 
         raise DataNotFoundError(
-            _blkNotFoundErrMsg(diskonly, str(apri), None, startn, length)
+            _blk_not_found_err_msg(diskonly, str(apri), None, startn, length)
         )
 
-    def blks(self, apri, sort = False, diskonly = False, recursively = False, retMetadata = False, **kwargs):
+    def blks(self, apri, sort = False, diskonly = False, recursively = False, ret_metadata = False, **kwargs):
 
-        self._checkOpenRaise("blks")
+        self._check_open_raise("blks")
 
         if not isinstance(apri, ApriInfo):
-            raise TypeError("`apri` must be of type `ApriInfo`.")
+            raise TypeError("`info` must be of type `ApriInfo`.")
 
         if not isinstance(diskonly, bool):
             raise TypeError("`diskonly` must be of type `bool`.")
 
-        if not isinstance(retMetadata, bool):
-            raise TypeError("`retMetadata` must be of type `bool`.")
+        if not isinstance(ret_metadata, bool):
+            raise TypeError("`ret_metadata` must be of type `bool`.")
 
         if not isinstance(recursively, bool):
             raise TypeError("`recursively` must be of type `bool`.")
 
         try:
-            self._checkKnownApri(apri)
+            self._check_known_apri(apri)
 
         except DataNotFoundError:
 
             if not recursively:
                 raise
 
         else:
 
             for startn, length in self.intervals(apri, combine = False, diskonly = diskonly, recursively = recursively):
 
                 try:
-                    yield self.blk(apri, startn, length, diskonly, False, retMetadata, **kwargs)
+                    yield self.blk(apri, startn, length, diskonly, False, ret_metadata, **kwargs)
 
                 except DataNotFoundError:
                     pass
 
         if recursively:
 
-            for subreg in self._iterSubregs():
+            for subreg in self._iter_subregs():
 
-                with subreg._recursiveOpen(True) as subreg:
-                    yield from subreg.blks(apri, sort, diskonly, True, retMetadata, **kwargs)
+                with subreg._recursive_open(True) as subreg:
+                    yield from subreg.blks(apri, sort, diskonly, True, ret_metadata, **kwargs)
 
-    def __getitem__(self, apriNDiskonlyRecursively):
+    def __getitem__(self, apri_n_diskonly_recursively):
 
-        if not isinstance(apriNDiskonlyRecursively, tuple) or len(apriNDiskonlyRecursively) <= 1:
+        if not isinstance(apri_n_diskonly_recursively, tuple) or len(apri_n_diskonly_recursively) <= 1:
             raise TypeError("Must pass at least two arguments to `reg[]`.")
 
-        if len(apriNDiskonlyRecursively) >= 5:
+        if len(apri_n_diskonly_recursively) >= 5:
             raise TypeError("Must pass at most four arguments to `reg[]`.")
 
-        if len(apriNDiskonlyRecursively) == 2:
+        if len(apri_n_diskonly_recursively) == 2:
 
-            apri, n = apriNDiskonlyRecursively
+            apri, n = apri_n_diskonly_recursively
             diskonly = False
             recursively = False
 
-        elif len(apriNDiskonlyRecursively) == 3:
+        elif len(apri_n_diskonly_recursively) == 3:
 
-            apri, n, diskonly = apriNDiskonlyRecursively
+            apri, n, diskonly = apri_n_diskonly_recursively
             recursively = False
 
         else:
-            apri, n, diskonly, recursively = apriNDiskonlyRecursively
+            apri, n, diskonly, recursively = apri_n_diskonly_recursively
 
         return self.get(apri, n, diskonly, recursively)
 
     def get(self, apri, n, diskonly = False, recursively = False, **kwargs):
 
-        self._checkOpenRaise("get")
+        self._check_open_raise("get")
 
         if not isinstance(apri, ApriInfo):
             raise TypeError("The first argument to `reg[]` must be an `ApriInfo.")
 
-        if not isInt(n) and not isinstance(n, slice):
+        if not is_int(n) and not isinstance(n, slice):
             raise TypeError("The second argument to `reg[]` must be an `int` or a `slice`.")
 
-        elif isInt(n):
+        elif is_int(n):
             n = int(n)
 
         else:
 
             _n = [None]*3
 
-            if n.start is not None and not isInt(n.start):
+            if n.start is not None and not is_int(n.start):
                 raise TypeError("Start index of slice must be an `int`.")
 
             elif n.start is not None:
                 _n[0] = int(n.start)
 
-            if n.stop is not None and not isInt(n.stop):
+            if n.stop is not None and not is_int(n.stop):
                 raise TypeError("Stop index of slice must be an `int`.")
 
             elif n.stop is not None:
                 _n[1] = int(n.stop)
 
-            if n.step is not None and not isInt(n.step):
+            if n.step is not None and not is_int(n.step):
                 raise TypeError("Step index of slice must be an `int`.")
 
             elif n.step is not None:
                 _n[2] = int(n.stop)
 
             n = slice(*tuple(_n))
 
@@ -2813,59 +2838,59 @@
             if n.start is not None and n.start < 0:
                 raise ValueError("Start index cannot be negative.")
 
             if n.stop is not None and n.stop < 0:
                 raise ValueError("Stop index cannot be negative.")
 
         try:
-            self._checkKnownApri(apri)
+            self._check_known_apri(apri)
 
         except DataNotFoundError:
 
             if not recursively:
                 raise
 
         else:
 
             if isinstance(n, slice):
                 # return iterator if given slice
                 return _ElementIter(self, apri, n, diskonly, recursively, kwargs)
 
             else:
 
-                blk = self.blkByN(apri, n, diskonly, recursively, False, **kwargs)
+                blk = self.blk_by_n(apri, n, diskonly, recursively, False, **kwargs)
                 ret = blk[n]
 
                 if isinstance(blk, ReleaseBlock):
                     blk.release()
 
                 return ret
 
         if recursively:
 
-            for subreg in self._iterSubregs():
+            for subreg in self._iter_subregs():
 
-                with subreg._recursiveOpen(True) as subreg:
+                with subreg._recursive_open(True) as subreg:
 
                     try:
                         return subreg.get(apri, n, diskonly, recursively, **kwargs)
 
                     except DataNotFoundError:
                         pass
 
         raise DataNotFoundError(
-            _blkNotFoundErrMsg(diskonly, str(apri), n)
+            _blk_not_found_err_msg(diskonly, str(apri), n)
         )
 
     def intervals(self, apri, sort = False, combine = False, diskonly = False, recursively = False):
 
-        self._checkOpenRaise("intervals")
+        self._check_open_raise("intervals")
 
         if not isinstance(apri, ApriInfo):
-            raise TypeError("`apri` must be of type `ApriInfo`.")
+            raise TypeError("`info` must be of type `ApriInfo`.")
 
         if not isinstance(sort, bool):
             raise TypeError("`sort` must be of type `bool`.")
 
         if not isinstance(combine, bool):
             raise TypeError("`combine` must be of type `bool`.")
 
@@ -2874,36 +2899,36 @@
 
         if not isinstance(recursively, bool):
             raise TypeError("`recursively` must be of type `bool`.")
 
         if not sort and not combine:
 
             try:
-                self._checkKnownApri(apri)
+                self._check_known_apri(apri)
 
             except DataNotFoundError:
 
                 if not recursively:
                     raise
 
             else:
 
-                if not diskonly and apri in self._ramBlks.keys():
+                if not diskonly and apri in self._ram_blks.keys():
 
-                    for blk in self._ramBlks[apri]:
+                    for blk in self._ram_blks[apri]:
                         yield blk.startn(), len(blk)
 
-                for key, _ in self._iterDiskBlkPairs(_BLK_KEY_PREFIX, apri, None):
-                    yield self._convertDiskBlockKey(_BLK_KEY_PREFIX_LEN, key, apri)[1:]
+                for key, _ in self._iter_disk_blk_pairs(_BLK_KEY_PREFIX, apri, None):
+                    yield self._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, key, apri)[1:]
 
             if recursively:
 
-                for subreg in self._iterSubregs():
+                for subreg in self._iter_subregs():
 
-                    with subreg._recursiveOpen(True) as subreg:
+                    with subreg._recursive_open(True) as subreg:
                         yield from subreg.intervals(apri, sort = False, combine = False, diskonly = diskonly, recursively = True)
 
         elif combine:
 
             ret = []
             intervals_sorted = self.intervals(apri, sort = True, combine = False, diskonly = diskonly, recursively = recursively)
             for startn, length in intervals_sorted:
@@ -2918,218 +2943,218 @@
 
         else:
             yield from sorted(
                 list(self.intervals(apri, sort = False, combine = False, diskonly = diskonly, recursively = recursively)),
                 key = lambda t: (t[0], -t[1])
             )
 
-    def totalLen(self, apri, diskonly = False, recursively = False):
+    def total_len(self, apri, diskonly = False, recursively = False):
 
-        self._checkOpenRaise("totalLen")
+        self._check_open_raise("total_len")
 
         if not isinstance(apri, ApriInfo):
-            raise TypeError("`apri` must be of type `ApriInfo`.")
+            raise TypeError("`info` must be of type `ApriInfo`.")
 
         if not isinstance(diskonly, bool):
             raise TypeError("`diskonly` must be of type `bool`.")
 
         if not isinstance(recursively, bool):
             raise TypeError("`recursively` must be of type `bool`.")
 
         try:
             return sum(t[1] for t in self.intervals(apri, combine = True, diskonly = diskonly, recursively = recursively))
 
         except DataNotFoundError:
             return 0
 
-    def numBlks(self, apri, diskonly = False, recursively = False):
+    def num_blks(self, apri, diskonly = False, recursively = False):
 
-        self._checkOpenRaise("numBlks")
+        self._check_open_raise("num_blks")
 
         if not isinstance(apri, ApriInfo):
-            raise TypeError("`apri` must be of type `ApriInfo`.")
+            raise TypeError("`info` must be of type `ApriInfo`.")
 
         if not isinstance(diskonly, bool):
             raise TypeError("`diskonly` must be of type `bool`.")
 
         if not isinstance(recursively, bool):
             raise TypeError("`recursively` must be of type `bool`.")
 
         try:
-            self._checkKnownApri(apri)
+            self._check_known_apri(apri)
 
         except DataNotFoundError:
 
             if not recursively:
                 return 0
 
         else:
 
             with self._db.begin() as txn:
-                ret = self._numDiskBlksTxn(apri, txn)
+                ret = self._num_disk_blks_txn(apri, txn)
 
             if not diskonly:
-                ret += sum(len(val) for val in self._ramBlks.values())
+                ret += sum(len(val) for val in self._ram_blks.values())
 
         if recursively:
 
-            for subreg in self._iterSubregs():
+            for subreg in self._iter_subregs():
 
-                with subreg._recursiveOpen(True) as subreg:
-                    ret += subreg.numBlks(apri, diskonly, True)
+                with subreg._recursive_open(True) as subreg:
+                    ret += subreg.num_blks(apri, diskonly, True)
 
 
         return ret
 
     def maxn(self, apri, diskonly = False, recursively = False):
 
-        self._checkOpenRaise("maxn")
+        self._check_open_raise("maxn")
 
         if not isinstance(apri, ApriInfo):
-            raise TypeError("`apri` must be of type `ApriInfo`.")
+            raise TypeError("`info` must be of type `ApriInfo`.")
 
         if not isinstance(diskonly, bool):
             raise TypeError("`diskonly` must be of type `bool`.")
 
         if not isinstance(recursively, bool):
             raise TypeError("`recursively` must be of type `bool`.")
 
         ret = -1
 
         try:
-            self._checkKnownApri(apri)
+            self._check_known_apri(apri)
 
         except DataNotFoundError:
 
             if not recursively:
                 raise
 
         else:
 
             for startn, length in self.intervals(apri, sort = False, combine = False, diskonly = diskonly, recursively = recursively):
                 ret = startn + length - 1
 
         if recursively:
 
-            for subreg in self._iterSubregs():
+            for subreg in self._iter_subregs():
 
-                with subreg._recursiveOpen(True) as subreg:
+                with subreg._recursive_open(True) as subreg:
 
                     try:
                         ret = max(ret, subreg.maxn(apri, diskonly = diskonly, recursively = True))
 
                     except DataNotFoundError:
                         pass
 
         if ret == -1:
-            raise DataNotFoundError(_blkNotFoundErrMsg(diskonly, apri))
+            raise DataNotFoundError(_blk_not_found_err_msg(diskonly, apri))
 
         else:
             return ret
 
     #################################
     # PROTEC RAM & DISK BLK METHODS #
 
-    def _resolveStartnLength(self, apri, startn, length, diskonly, txn = None):
+    def _resolve_startn_length(self, apri, startn, length, diskonly, txn = None):
         """
         :param apri: (type `ApriInfo`)
         :param startn: (type `int` or `NoneType`) Non-negative.
         :param length: (type `int` or `NoneType`) Positive.
-        :raise DataNotFoundError: If `apri` is not known to this register, or if no data is found matching startn and
+        :raise DataNotFoundError: If `info` is not known to this register, or if no data is found matching startn and
         length.
         :raise ValueError: If `startn_ is None and length_ is not None`.
         :return: (type `int`) Resolved `startn`, always `int`.
         :return: (type `int`) Resolved `length`, always `int`.
         """
 
         if startn is None and length is not None:
             raise ValueError(f"If you specify a `Block` length, you must also specify a `startn`.")
 
         elif startn is not None and length is not None:
             return startn, length
 
-        if not diskonly and apri in self._ramBlks.keys():
+        if not diskonly and apri in self._ram_blks.keys():
 
             if startn is not None and length is None:
 
-                for blk in self._ramBlks[apri]:
+                for blk in self._ram_blks[apri]:
 
                     if blk.startn() == startn:
                         return startn, len(blk)
 
             else:
-                return self._ramBlks[apri][0].startn(), len(self._ramBlks[apri][0])
+                return self._ram_blks[apri][0].startn(), len(self._ram_blks[apri][0])
 
         if startn is not None and length is None:
 
-            key = self._getDiskBlkKey(_BLK_KEY_PREFIX, apri, None, startn, 1, False, txn) # raises DataNotFoundError
+            key = self._get_disk_blk_key(_BLK_KEY_PREFIX, apri, None, startn, 1, False, txn) # raises DataNotFoundError
             first_key_sep_index = key.find(_KEY_SEP)
             second_key_sep_index = key.find(_KEY_SEP, first_key_sep_index + 1)
             prefix = key [ : second_key_sep_index + 1]
 
-            with lmdbPrefixIter(txn if txn is not None else self._db, prefix) as it:
+            with lmdb_prefix_iter(txn if txn is not None else self._db, prefix) as it:
 
                 for key, _ in it:
-                    return self._convertDiskBlockKey(_BLK_KEY_PREFIX_LEN, key, apri, None)[1:]
+                    return self._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, key, apri, None)[1:]
 
                 else:
                     raise DataNotFoundError(
-                        _blkNotFoundErrMsg(True, apri, None, startn, None)
+                        _blk_not_found_err_msg(True, apri, None, startn, None)
                     )
 
         else:
 
-            prefix = _BLK_KEY_PREFIX + self._getIdByApri(apri, None, False) + _KEY_SEP
+            prefix = _BLK_KEY_PREFIX + self._get_id_by_apri(apri, None, False) + _KEY_SEP
 
-            with lmdbPrefixIter(self._db, prefix) as it:
+            with lmdb_prefix_iter(self._db, prefix) as it:
 
                 for key, _ in it:
-                    return self._convertDiskBlockKey(_BLK_KEY_PREFIX_LEN, key, apri, None)[1:]
+                    return self._convert_disk_block_key(_BLK_KEY_PREFIX_LEN, key, apri, None)[1:]
 
                 else:
-                    raise DataNotFoundError(_blkNotFoundErrMsg(True, apri))
+                    raise DataNotFoundError(_blk_not_found_err_msg(True, apri))
 
 class PickleRegister(Register):
 
     @classmethod
-    def withSuffix(cls, filename):
+    def with_suffix(cls, filename):
         return filename.with_suffix(".pkl")
 
     @classmethod
-    def dumpDiskData(cls, data, filename, **kwargs):
+    def dump_disk_data(cls, data, filename, **kwargs):
 
         if len(kwargs) > 0:
             raise KeyError("This method accepts no keyword-arguments.")
 
         with filename.open("wb") as fh:
             pickle.dump(data, fh)
 
     @classmethod
-    def loadDiskData(cls, filename, **kwargs):
+    def load_disk_data(cls, filename, **kwargs):
 
         if len(kwargs) > 0:
             raise KeyError("`Pickle_Register.blk` accepts no keyword-arguments.")
 
         with filename.open("rb") as fh:
             return pickle.load(fh), filename
 
-Register.addSubclass(PickleRegister)
+Register.add_subclass(PickleRegister)
 
 class NumpyRegister(Register):
 
     @classmethod
-    def dumpDiskData(cls, data, filename, **kwargs):
+    def dump_disk_data(cls, data, filename, **kwargs):
 
         if len(kwargs) > 0:
             raise KeyError("This method accepts no keyword-arguments.")
 
         np.save(filename, data, allow_pickle = False, fix_imports = False)
 
     @classmethod
-    def loadDiskData(cls, filename, **kwargs):
+    def load_disk_data(cls, filename, **kwargs):
 
         if "mmap_mode" in kwargs:
             mmap_mode = kwargs["mmap_mode"]
 
         else:
             mmap_mode = None
 
@@ -3142,317 +3167,317 @@
                 "`None`, 'r+', 'r', 'w+', 'c'. Please see " +
                 "https://numpy.org/doc/stable/reference/generated/numpy.memmap.html#numpy.memmap for more information."
             )
 
         return np.load(filename, mmap_mode = mmap_mode, allow_pickle = False, fix_imports = False)
 
     @classmethod
-    def cleanDiskData(cls, filename, **kwargs):
+    def clean_disk_data(cls, filename, **kwargs):
 
         if len(kwargs) > 0:
             raise KeyError("This method accepts no keyword-arguments.")
 
         filename = filename.with_suffix(".npy")
-        return Register.cleanDiskData(filename)
+        return Register.clean_disk_data(filename)
 
     @classmethod
-    def withSuffix(cls, filename):
+    def with_suffix(cls, filename):
         return filename.with_suffix(".npy")
 
-    def blk(self, apri, startn = None, length = None, diskonly = False, recursively = False, retMetadata = False, **kwargs):
+    def blk(self, apri, startn = None, length = None, diskonly = False, recursively = False, ret_metadata = False, **kwargs):
         """
         :param apri: (type `ApriInfo`)
         :param startn: (type `int`)
         :param length: (type `length_`) non-negative
-        :param retMetadata: (type `bool`, default `False`) Whether to return a `File_Metadata` object, which
+        :param ret_metadata: (type `bool`, default `False`) Whether to return a `File_Metadata` object, which
         contains file creation date/time and size of dumped saved on the disk.
         :param recursively: (type `bool`, default `False`) Search all subregisters for the `Block`.
         :param mmap_mode: (type `str`, optional) Load the Numpy file using memory mapping, see
         https://numpy.org/doc/stable/reference/generated/numpy.memmap.html#numpy.memmap for more information.
-        :return: (type `File_Metadata`) If `retMetadata is True`.
+        :return: (type `File_Metadata`) If `ret_metadata is True`.
         """
 
-        ret = super().blk(apri, startn, length, diskonly, recursively, retMetadata,  **kwargs)
+        ret = super().blk(apri, startn, length, diskonly, recursively, ret_metadata, **kwargs)
 
-        if retMetadata:
+        if ret_metadata:
             blk = ret[0]
 
         else:
             blk = ret
 
         if isinstance(blk.segment(), np.memmap):
             blk = MemmapBlock(blk.segment(), blk.apri(), blk.startn())
 
-        if retMetadata:
+        if ret_metadata:
             return blk, ret[1]
 
         else:
             return blk
 
-    def concatDiskBlks(self, apri, startn = None, length = None, delete = False, retMetadata = False):
+    def concat_disk_blks(self, apri, startn = None, length = None, delete = False, ret_metadata = False):
         """Concatenate several `Block`s into a single `Block` along axis 0 and save the new one to the disk.
 
         If `delete = True`, then the smaller `Block`s are deleted automatically.
 
         The interval `range(startn, startn + length)` must be the disjoint union of intervals of the form
         `range(blk.startn(), blk.startn() + len(blk))`, where `blk` is a disk `Block` with `ApriInfo`
-        given by `apri`.
+        given by `info`.
 
         Length-0 `Block`s are ignored.
 
         If `startn` is not specified, it is taken to be the smallest `startn` of any `Block` saved to this
         `Register`. If `length` is not specified, it is taken to be the length of the largest
         contiguous set of indices that start with `startn`. If `startn` is not specified but `length` is, a
         ValueError is raised.
 
         :param apri: (type `ApriInfo`)
         :param startn: (type `int`) Non-negative.
         :param length: (type `int`) Positive.
         :param delete: (type `bool`, default `False`)
-        :param retMetadata: (type `bool`, default `False`) Whether to return a `File_Metadata` object, which
+        :param ret_metadata: (type `bool`, default `False`) Whether to return a `File_Metadata` object, which
         contains file creation date/time and size of dumped dumped to the disk.
         :raise DataNotFoundError: If the union of the intervals of relevant disk `Block`s does not equal
         `range(startn, startn + length)`.
         :raise ValueError: If any two intervals of relevant disk `Block`s intersect.
         :raise ValueError: If any two relevant disk `Block` segments have inequal shapes.
-        :return: (type `File_Metadata`) If `retMetadata is True`.
+        :return: (type `File_Metadata`) If `ret_metadata is True`.
         """
 
         _FAIL_NO_RECOVER_ERROR_MESSAGE = "Could not successfully recover from a failed disk `Block` concatenation!"
 
-        self._checkOpenRaise("concatDiskBlks")
+        self._check_open_raise("concat_disk_blks")
 
-        self._checkReadwriteRaise("concatDiskBlks")
+        self._check_readwrite_raise("concat_disk_blks")
 
-        startn, length = Register._checkApriStartnLengthRaise(apri, startn, length)
+        startn, length = Register._check_apri_startn_length_raise(apri, startn, length)
 
-        if not isinstance(retMetadata, bool):
-            raise TypeError("`retMetadata` must be of type `bool`.")
+        if not isinstance(ret_metadata, bool):
+            raise TypeError("`ret_metadata` must be of type `bool`.")
 
-        self._checkKnownApri(apri)
+        self._check_known_apri(apri)
         # infer startn
-        startn, _ = self._resolveStartnLength(apri, startn, length, True)
+        startn, _ = self._resolve_startn_length(apri, startn, length, True)
         # this implementation depends on `intervals` returning smaller startn before larger
         # ones and, when ties occur, larger lengths before smaller ones.
         if length is None:
             # infer length
 
             current_segment = False
             length = 0
 
-            for _startn, _length in self.intervals(apri, combine = False, diskonly = False):
+            for startn_, length_ in self.intervals(apri, combine = False, diskonly = False):
 
-                if _length > 0:
+                if length_ > 0:
 
                     if current_segment:
 
-                        if startn > _startn:
+                        if startn > startn_:
                             raise RuntimeError("Could not infer a value for `length`.")
 
-                        elif startn == _startn:
+                        elif startn == startn_:
                             raise ValueError(
                                 f"Overlapping `Block` intervals found with {str(apri)}."
                             )
 
                         else:
 
-                            if startn + length > _startn:
+                            if startn + length > startn_:
                                 raise ValueError(
                                     f"Overlapping `Block` intervals found with {str(apri)}."
                                 )
 
-                            elif startn + length == _startn:
-                                length += _length
+                            elif startn + length == startn_:
+                                length += length_
 
                             else:
                                 break
 
                     else:
 
-                        if startn < _startn:
-                            raise DataNotFoundError(_blkNotFoundErrMsg(True, apri, None, startn))
+                        if startn < startn_:
+                            raise DataNotFoundError(_blk_not_found_err_msg(True, apri, None, startn))
 
-                        elif startn == _startn:
+                        elif startn == startn_:
 
-                            length += _length
+                            length += length_
                             current_segment = True
 
             if length == 0:
                 raise RuntimeError("could not infer a value for `length`.")
 
             warnings.warn(f"`length` value not specified, inferred value: `length = {length}`.")
 
         combined_interval = None
 
         last_check = False
-        last__startn = None
-        _startn = None
-        _length = None
+        last_startn_ = None
+        startn_ = None
+        length_ = None
         intervals_to_get = []
 
-        for _startn, _length in self.intervals(apri, combine = False, diskonly = True):
+        for startn_, length_ in self.intervals(apri, combine = False, diskonly = True):
             # infer blocks to combine
 
             if last_check:
 
-                if last__startn == _startn and _length > 0:
+                if last_startn_ == startn_ and length_ > 0:
                     raise ValueError(f"Overlapping `Block` intervals found with {str(apri)}.")
 
                 else:
                     break
 
-            if _length > 0:
+            if length_ > 0:
 
-                last__startn = _startn
+                last_startn_ = startn_
 
-                if _startn < startn:
+                if startn_ < startn:
 
-                    if startn < _startn + _length:
+                    if startn < startn_ + length_:
                         raise ValueError(
                             f"The first `Block` does not have the right size. Try again by calling "
-                            f"`reg.concatDiskBlks({str(apri)}, {_startn}, {length - (_startn - startn)})`."
+                            f"`reg.concat_disk_blks({str(apri)}, {startn_}, {length - (startn_ - startn)})`."
                         )
 
                 else:
 
                     if combined_interval is None:
 
-                        if _startn > startn:
+                        if startn_ > startn:
 
                             raise DataNotFoundError(
                                 f"No disk `Block` found with the following data: `{str(apri)}, startn = {startn}`."
                             )
 
-                        elif _startn == startn:
+                        elif startn_ == startn:
 
-                            combined_interval = (_startn, _length)
-                            intervals_to_get.append((_startn, _length))
-                            last_check = _startn + _length == startn + length
+                            combined_interval = (startn_, length_)
+                            intervals_to_get.append((startn_, length_))
+                            last_check = startn_ + length_ == startn + length
 
                         else:
                             raise RuntimeError("Something went wrong trying to combine `Block`s.")
 
                     else:
 
-                        if _startn > sum(combined_interval):
+                        if startn_ > sum(combined_interval):
 
                             raise DataNotFoundError(
                                 f"No `Block` found covering indices {sum(combined_interval)} through "
-                                f"{_startn-1} (inclusive) with {str(apri)}."
+                                f"{startn_-1} (inclusive) with {str(apri)}."
                             )
 
-                        elif _startn == sum(combined_interval):
+                        elif startn_ == sum(combined_interval):
 
-                            if _startn + _length > startn + length:
+                            if startn_ + length_ > startn + length:
                                 raise ValueError(
                                     f"The last `Block` does not have the right size. Try again by calling "
-                                    f"`reg.concatDiskBlks({str(apri)}, {startn}, "
-                                    f"{length - (_startn + _length - (startn + length))})`."
+                                    f"`reg.concat_disk_blks({str(apri)}, {startn}, "
+                                    f"{length - (startn_ + length_ - (startn + length))})`."
                                 )
 
-                            combined_interval = (startn, combined_interval[1] + _length)
-                            intervals_to_get.append((_startn, _length))
-                            last_check = _startn + _length == startn + length
+                            combined_interval = (startn, combined_interval[1] + length_)
+                            intervals_to_get.append((startn_, length_))
+                            last_check = startn_ + length_ == startn + length
 
                         else:
                             raise ValueError(f"Overlapping `Block` intervals found with {str(apri)}.")
 
         else:
 
-            if _startn is None:
-                raise DataNotFoundError(_blkNotFoundErrMsg(True, apri))
+            if startn_ is None:
+                raise DataNotFoundError(_blk_not_found_err_msg(True, apri))
 
-            elif _startn + _length != startn + length:
+            elif startn_ + length_ != startn + length:
                 raise ValueError(
                     f"The last `Block` does not have the right size. "
-                    f"Try again by calling `reg.concatDiskBlks(apri, {startn}, {_startn + _length})`."
+                    f"Try again by calling `reg.concat_disk_blks(info, {startn}, {startn_ + length_})`."
                 )
 
         if len(intervals_to_get) == 1:
 
-            if retMetadata:
-                return self.blkMetadata(apri, *intervals_to_get)
+            if ret_metadata:
+                return self.blk_metadata(apri, *intervals_to_get)
 
             else:
                 return None
 
         blks = []
         fixed_shape = None
         ref_blk = None
         failure_reinsert_indices = []
         combined_blk = None
 
         try:
 
-            for _startn, _length in intervals_to_get:
+            for startn_, length_ in intervals_to_get:
                 # check that blocks have the correct shape
 
-                blk = self.blk(apri, _startn, _length, True, False, False, mmap_mode="r")
+                blk = self.blk(apri, startn_, length_, True, False, False, mmap_mode="r")
                 blks.append(blk)
 
                 if fixed_shape is None:
 
                     fixed_shape = blk.segment().shape[1:]
                     ref_blk = blk
 
                 elif fixed_shape != blk.segment().shape[1:]:
 
                     raise ValueError(
                         "Cannot combine the following two `Block`s because all axes other than axis 0 must have the same " +
                         "shape:\n" +
                         f"{str(apri)}, startn = {ref_blk.startn()}, length = {len(ref_blk)}\n, shape = " +
                         f"{str(fixed_shape)}\n" +
-                        f"{str(apri)}, startn = {_startn}, length = {_length}\n, shape = " +
+                        f"{str(apri)}, startn = {startn_}, length = {length_}\n, shape = " +
                         f"{str(blk.segment().shape)}\n"
 
                     )
 
             combined_blk = np.concatenate([blk.segment() for blk in blks], axis=0)
             combined_blk = Block(combined_blk, apri, startn)
-            ret = self.addDiskBlk(combined_blk, retMetadata)
+            ret = self.add_disk_blk(combined_blk, ret_metadata)
 
             if _debug == 1:
                 raise KeyboardInterrupt
 
             if delete:
 
                 for blk in blks:
 
-                    _startn = blk.startn()
-                    _length = len(blk)
+                    startn_ = blk.startn()
+                    length_ = len(blk)
                     blk.release()
-                    self.rmvDiskBlk(apri, _startn, _length, False)
-                    failure_reinsert_indices.append((_startn, _length))
+                    self.rmv_disk_blk(apri, startn_, length_, False)
+                    failure_reinsert_indices.append((startn_, length_))
 
                     if _debug == 2:
                         raise KeyboardInterrupt
 
         except BaseException as e:
 
             try:
 
                 if combined_blk is not None and isinstance(combined_blk, Block) and delete:
 
-                    for _startn, _length in failure_reinsert_indices:
-                        self.addDiskBlk(combined_blk[_startn: _startn + _length])
+                    for startn_, length_ in failure_reinsert_indices:
+                        self.add_disk_blk(combined_blk[startn_: startn_ + length_])
 
             except BaseException:
                 raise RegisterRecoveryError(_FAIL_NO_RECOVER_ERROR_MESSAGE)
 
             else:
                 raise e
 
         finally:
 
             for blk in blks:
                 blk.release()
 
         return ret
 
-Register.addSubclass(NumpyRegister)
+Register.add_subclass(NumpyRegister)
 
 class _ElementIter:
 
     def __init__(self, reg, apri, slc, diskonly, recursively, kwargs):
 
         self.reg = reg
         self.apri = apri
@@ -3461,262 +3486,248 @@
         self.diskonly = diskonly
         self.recursively = recursively
         self.kwargs = kwargs
         self.curr_blk = None
         self.intervals = None
         self.curr_n = slc.start if slc.start else 0
 
-    def updateIntervalsCalculated(self):
+    def update_intervals_calculated(self):
 
         self.intervals = list(
             self.reg.intervals(self.apri, sort = True, combine = False, diskonly = self.diskonly, recursively = self.recursively)
         )
 
-    def getNextBlk(self):
+    def get_next_blk(self):
 
         if self.curr_blk is not None and isinstance(self.curr_blk, ReleaseBlock):
             self.curr_blk.release()
 
-        return self.reg.blkByN(self.apri, self.curr_n, self.diskonly, self.recursively, False, **self.kwargs)
+        return self.reg.blk_by_n(self.apri, self.curr_n, self.diskonly, self.recursively, False, **self.kwargs)
 
     def __iter__(self):
         return self
 
     def __next__(self):
 
         if self.stop is not None and self.curr_n >= self.stop:
             raise StopIteration
 
         elif self.curr_blk is None:
 
-            self.updateIntervalsCalculated()
+            self.update_intervals_calculated()
 
             if len(self.intervals) == 0:
                 raise StopIteration
 
             self.curr_n = max(self.intervals[0][0], self.curr_n)
 
             try:
-                self.curr_blk = self.getNextBlk()
+                self.curr_blk = self.get_next_blk()
 
             except DataNotFoundError:
                 raise StopIteration
 
         elif self.curr_n not in self.curr_blk:
 
             try:
-                self.curr_blk = self.getNextBlk()
+                self.curr_blk = self.get_next_blk()
 
             except DataNotFoundError:
 
-                self.updateIntervalsCalculated()
+                self.update_intervals_calculated()
 
                 for startn, length in self.intervals:
 
                     if startn > self.curr_n:
 
                         self.curr_n += math.ceil( (startn - self.curr_n) / self.step ) * self.step
                         break
 
                 else:
                     raise StopIteration
 
-                self.curr_blk = self.getNextBlk()
+                self.curr_blk = self.get_next_blk()
 
         ret = self.curr_blk[self.curr_n]
         self.curr_n += self.step
         return ret
 
 class _CopyRegister(Register):
 
     @classmethod
-    def withSuffix(cls, filename):
+    def with_suffix(cls, filename):
         return filename
 
     @classmethod
-    def dumpDiskData(cls, data, filename, **kwargs):
+    def dump_disk_data(cls, data, filename, **kwargs):
 
         if not isinstance(data, Path):
             raise TypeError("`data` must of of type `Path`.")
 
         if not data.absolute():
             raise ValueError("`data` must be an absolute `Path`.")
 
         filename = filename.with_suffix(data.suffix)
         shutil.copyfile(data, filename)
         return filename
 
     @classmethod
-    def loadDiskData(cls, filename, **kwargs):
+    def load_disk_data(cls, filename, **kwargs):
         raise NotImplementedError
 
     def setClsName(self, clsName):
 
-        with self._clsFilepath.open() as fh:
+        with self._cls_filepath.open() as fh:
             fh.write(clsName)
 
-# def updateRegVersion(ident):
-#
-#     from venv import EnvBuilder
-#     from subprocess import check_call, DEVNULL
-#     import importlib
-#     import string
-#     import re
-#
-#     ident = Path(ident)
-#
-#     if not ident.absolute():
-#         ident = Path.cwd() / ident
-#
-#     checkRegStructure(ident)
-#
-#     with (ident / VERSION_FILEPATH).open("r") as fh:
-#         oldVers = fh.read()
-#
-#     if oldVers in COMPATIBLE_VERSIONS:
-#
-#         print(f"Register version at {ident} is up-to-date.")
-#         return
-#
-#     builder = EnvBuilder(with_pip = True)
-#     print("Setting up temporary venv....")
-#     envDir = randomUniqueFilename(Path.home())
-#     oldCorniferName = None
-#
-#     try:
-#
-#         builder.create(envDir)
-#         print("... done.")
-#         print("Downloading old cornifer version....")
-#         oldCorniferDir = randomUniqueFilename(Path.home(), length = 25)
-#         oldCorniferDir.mkdir(exist_ok = False)
-#         check_call(
-#             ["git", "clone", "--depth", "1", "--branch", oldVers, "https://github.com/automorphis/cornifer.git", str(oldCorniferDir)],
-#             stderr = DEVNULL, stdout = DEVNULL
-#         )
-#         print("... done.")
-#         print("Installing old cornifer.... ")
-#
-#         # this name is not guaranteed to be a unique package name, but it will be with extremely high probability
-#         oldCorniferName = (
-#             "cornifer_" +
-#             randomUniqueFilename(Path.home(), length = 25, alphabet = string.ascii_uppercase + string.ascii_lowercase).name
-#         )
-#
-#         for filename in oldCorniferDir.glob("**/*.py"):
-#
-#             with filename.open("r") as fh:
-#                 editedText = re.sub("cornifer", oldCorniferName, fh.read())
-#
-#             with filename.open("w") as fh:
-#                 fh.write(editedText)
-#
-#         (oldCorniferDir / "lib" / "cornifer").rename(oldCorniferDir / "lib" / oldCorniferName)
-#         check_call(
-#             ["pip", "install", str(oldCorniferDir)],
-#             stderr = DEVNULL, stdout = DEVNULL
-#         )
-#         importlib.invalidate_caches()
-#         print("... done.")
-#         print("Updating register....")
-#
-#         if oldVers in ["0.1.0", "0.2", "0.3"]:
-#
-#             oldRegLoader = importlib.import_module(".register_loader", oldCorniferName)
-#             dbMapSize = 25 * BYTES_PER_MB
-#
-#         else:
-#
-#             with (ident / MAP_SIZE_FILEPATH).open("r") as fh:
-#                 dbMapSize = int(fh.read())
-#
-#             oldRegLoader = importlib.import_module(".regloader", oldCorniferName)
-#
-#         with (ident / CLS_FILEPATH).open("r") as fh:
-#             clsName = fh.read()
-#
-#         with (ident / MSG_FILEPATH).open("r") as fh:
-#             msg = fh.read()
-#
-#         oldErrors = importlib.import_module(".errors", oldCorniferName)
-#         newReg = _CopyRegister(ident.parent, msg, dbMapSize)
-#         oldReg = oldRegLoader.load(ident)
-#
-#         with oldReg.open() as oldReg:
-#
-#             with newReg.open() as newReg:
-#
-#                 if oldVers in ["0.1.0", "0.2", "0.3"]:
-#
-#                     for apri in oldReg:
-#
-#                         for startn, length in oldReg.disk_intervals(apri):
-#
-#                             metadata = oldReg.get_disk_block_metadata(apri, startn, length)
-#                             apri = ApriInfo.fromJson(apri.to_json())
-#                             newReg.addDiskBlk(Block(blk.get_segment(), apri, blk.get_start_n()))
-#
-#                         try:
-#                             apos = oldReg.get_apos_info()
-#
-#                         except oldErrors.Data_Not_Found_Error:
-#                             pass
-#
-#                         else:
-#                             newReg.setApos(apos)
-#
-#                 else:
-#
-#                     for apri in oldReg:
-#
-#                         for blk in oldReg.diskBlks(apri):
-#
-#                             apri = ApriInfo.fromJson(blk.apri().toJson())
-#                             newReg.addDiskBlk(Block(blk.segment(), apri, blk.startn()))
-#
-#                         try:
-#                             apos = oldReg.apos(apri)
-#
-#                         except oldErrors.DataNotFoundError:
-#                             pass
-#
-#                         else:
-#                             newReg.setApos(apos)
-#
-#         newReg.setClsName(clsName)
-#         print("... done.")
-#         print("Deleting old register....")
-#         shutil.rmtree(ident)
-#         newReg._localDir.rename(ident.name)
-#         print("... done.")
-#
-#     except:
-#
-#         erroredOut = True
-#         raise
-#
-#     else:
-#         erroredOut = False
-#
-#     finally:
-#
-#         if erroredOut:
-#             print("Encountered an error, cleaning up...")
-#
-#         if oldCorniferName is not None:
-#
-#             print("Uninstalling old cornifer....")
-#             check_call(
-#                 ["pip", "uninstall", oldCorniferName],
-#                 stderr = DEVNULL, stdout = DEVNULL
-#             )
-#             print("... done.")
-#
-#         print("Removing temporary venv...")
-#
-#         if envDir.exists():
-#             shutil.rmtree(envDir)
-#
-#         print("... done.")
-#
-#         if not erroredOut:
-#             print("Update successful!")
+###################
+# RELATIONAL INFO #
+###################
+
+_RELATIONAL_APRI_PREFIX = (_APRI_ID_KEY_PREFIX + _KEY_SEP).decode("ASCII")
+_RELATIONAL_APRI_PREFIX_LEN = len(_RELATIONAL_APRI_PREFIX)
+
+class _RelationalInfoJsonEncoder(_InfoJsonEncoder):
+
+    def __init__(self, *args, **kwargs):
+
+        if len(args) < 2:
+            raise RuntimeError("Must give at least two optional args, a `Register` followed by `lmdb.Transaction`.")
+
+        self._reg, self._txn = args[:2]
+
+        if not isinstance(self._reg, Register):
+            raise TypeError("The first argument must have type `Register`.")
+
+        if not is_transaction(self._txn):
+            raise TypeError("The second argument must have type `lmdb.transaction`.")
+
+        super().__init__(*args[2:], **kwargs)
+
+    def default(self, obj):
+
+        if isinstance(obj, ApriInfo):
+            return _RELATIONAL_APRI_PREFIX + self._reg._get_id_by_apri(obj, None, False, self._txn).decode("ASCII")
+
+        else:
+            return super().default(obj)
+
+
+class _RelationalInfoJsonDecoder(_InfoJsonDecoder):
+
+    def __init__(self, *args, **kwargs):
+
+        if len(args) < 2:
+            raise RuntimeError("Must give at least two optional args, a `Register` followed by `lmdb.Transaction`.")
+
+        self._reg, self._txn = args
+
+        if not isinstance(self._reg, Register):
+            raise TypeError("The first argument must have type `Register`.")
+
+        if not is_transaction(self._txn):
+            raise TypeError("The second argument must have type `lmdb.transaction`.")
+
+        super().__init__(*args[2:], **kwargs)
+
+    @staticmethod
+    def check_return_apri_id(str_):
+
+        check = len(str_) > _RELATIONAL_APRI_PREFIX_LEN and str_[:_RELATIONAL_APRI_PREFIX_LEN] == _RELATIONAL_APRI_PREFIX
+        return check, str_[_RELATIONAL_APRI_PREFIX_LEN:].encode("ASCII") if check else None
+
+    def object_hook(self, obj):
+
+        if isinstance(obj, str):
+
+            obj = obj.strip(" \t")
+
+            check_apri, apri_id = _RelationalInfoJsonDecoder.check_return_apri_id(obj)
+            check_apos, apos_json = _InfoJsonDecoder.check_return_apos_info_json(obj)
+
+            if check_apri:
+
+                apri_json = self._reg._get_apri_json_by_id(apri_id, self._txn).decode("ASCII")
+
+                try:
+                    return ApriInfo(**self.decode(apri_json))
+
+                except:
+                    raise
+
+            elif check_apos:
+                return AposInfo(**self.decode(apos_json))
+
+            else:
+                return obj
+
+        else:
+            return super().object_hook(obj)
+
+
+def relational_encode_info(reg, info, txn = None):
+
+    if not isinstance(reg, Register):
+        raise TypeError("`reg` must be of type `Register`.")
+
+    if not isinstance(info, _Info):
+        raise TypeError("`info` must be an instance of a concrete subclass of `_Info`.")
+
+    if txn is not None and not is_transaction(txn):
+        raise TypeError("`txn` must be of type `lmdb.Transaction`.")
+
+    if txn is None:
+
+        txn = reg._db.begin()
+        commit = True
+
+    else:
+        commit = False
+
+    try:
+
+        encoder = _RelationalInfoJsonEncoder(reg, txn,
+            ensure_ascii = True,
+            allow_nan = True,
+            indent = None,
+            separators = (',', ':')
+        )
+        info.set_encoder(encoder)
+        return info.to_json().encode("ASCII")
+
+    finally:
+
+        if commit:
+            txn.commit()
+
+
+def relational_decode_info(reg, cls, json, txn = None):
+
+    if not isinstance(reg, Register):
+        raise TypeError("`reg` must be of type `Register`.")
+
+    if not issubclass(cls, _Info):
+        raise TypeError("`cls` must be a subclass of `_Info`.")
+
+    if not isinstance(json, bytes):
+        raise TypeError("`json` must of of type `bytes`.")
+
+    if txn is not None and not is_transaction(txn):
+        raise TypeError("`txn` must be of type `lmdb.Transaction`.")
+
+    if txn is None:
+
+        commit = True
+        txn = reg._db.begin()
+
+    else:
+        commit = False
+
+    try:
+
+        decoder = _RelationalInfoJsonDecoder(reg, txn)
+        return cls.from_json(json.decode("ASCII"), decoder)
+
+    finally:
+
+        if commit:
+            txn.commit()
```

### Comparing `cornifer-0.5.1/lib/cornifer/regloader.py` & `cornifer-0.6/lib/cornifer/regloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,80 +15,80 @@
 
 import re
 import warnings
 from pathlib import Path
 
 from .errors import RegisterError
 from .registers import Register
-from .regfilestructure import LOCAL_DIR_CHARS, checkRegStructure
-from ._utilities import resolvePath
+from .regfilestructure import LOCAL_DIR_CHARS, check_reg_structure
+from ._utilities import resolve_path
 from .version import CURRENT_VERSION, COMPATIBLE_VERSIONS
 
 _ARGS_TYPES = {
-    "regLimit" : int,
+    "reg_limit" : int,
 
-    "printApri" : bool,
-    "apriLimit" : int,
+    "print_apri" : bool,
+    "apri_limit" : int,
 
-    "printIntervals" : bool,
-    "printIntervalMode" : str,
-    "intervalLimit" : int,
+    "print_intervals" : bool,
+    "print_interval_mode" : str,
+    "interval_limit" : int,
 
-    "printIncompatibleRegs" : bool,
+    "print_incompatible_regs" : bool,
 
-    "keyExactMatch" : bool,
+    "key_exact_match" : bool,
 
-    "tupleExactMatch" : bool,
+    "tuple_exact_match" : bool,
 
-    "dictExactMatch" : bool,
+    "dict_exact_match" : bool,
 
-    "strExactMatch" : bool,
+    "str_exact_match" : bool,
 
 }
 
 _args = {
-    "regLimit" : 10,
+    "reg_limit" : 10,
 
-    "printApri" : True,
-    "apriLimit" : 5,
+    "print_apri" : True,
+    "apri_limit" : 5,
 
-    "printIntervals" : True,
-    "printIntervalMode" : "combined", # combined, uncombined
-    "intervalLimit" : 5,
+    "print_intervals" : True,
+    "print_interval_mode" : "combined", # combined, uncombined
+    "interval_limit" : 5,
 
     "print_warnings_" : True,
     "warnings_limit" : 10,
 
-    "printIncompatibleRegs" : False,
+    "print_incompatible_regs" : False,
 
-    "keyExactMatch" : False,
+    "key_exact_match" : False,
 
-    "tupleExactMatch" : False,
+    "tuple_exact_match" : False,
 
-    "dictExactMatch" : False,
+    "dict_exact_match" : False,
 
-    "strExactMatch" : False
+    "str_exact_match" : False
 }
 
-def setSearchArgs(**kwargs):
+def set_search_args(**kwargs):
     """This function changes the output of the `search` function."""
 
     for key,val in kwargs:
 
         if key not in _ARGS_TYPES.keys():
             raise KeyError(f"Unrecognized `search_arg` key: {key}")
 
         elif not isinstance(val, _ARGS_TYPES[key]):
             raise TypeError(f"Expected type for key \"{key}\" value : {_ARGS_TYPES[key].__name__}")
 
         elif _ARGS_TYPES[key] == int and val <= 0:
             raise ValueError(f"Value for key \"{key}\" must be a positive integer.")
 
-        elif key == "printIntervals_mode" and val not in ["combined", "uncombined"]:
-            raise ValueError('Value for key "printIntervals_mode" can be either "combined" or "uncombined".')
+        elif key == "print_intervals_mode" and val not in ["combined", "uncombined"]:
+            raise ValueError('Value for key "print_intervals_mode" can be either "combined" or "uncombined".')
 
         _args[key] = val
 
 def load(identifier):
 
     if not isinstance(identifier, (str, Path)):
         raise TypeError("`ident` must be a string or a `pathlib.Path`.")
@@ -104,19 +104,19 @@
     if "(" in resolved.name or ")" in resolved.name:
         raise ValueError("You don't need to include the parentheses for the `ident` when you call `load`.")
 
     bad_symbs = [symb for symb in resolved.name if symb not in LOCAL_DIR_CHARS]
     if len(bad_symbs) > 0:
         raise ValueError("An ident cannot contain any of the following symbols: " + "".join(bad_symbs))
 
-    reg = Register._fromLocalDir(resolved)
+    reg = Register._from_local_dir(resolved)
 
-    if not reg._hasCompatibleVersion():
+    if not reg._has_compatible_version():
         warnings.warn(
-            f"The register at `{reg._localDir}` has an incompatible version.\n"
+            f"The register at `{reg._local_dir}` has an incompatible version.\n"
             f"Current Cornifer version: {CURRENT_VERSION}\n"
             f"Compatible versions:      {str(COMPATIBLE_VERSIONS)}\n"
             f"Loaded register version:  {reg._version}"
         )
 
     return reg
 
@@ -125,29 +125,29 @@
     # Search happens in 3 phases:
     # 1. Test to make sure parameters have the correct types.
     # 2. Iterate over all `Register`s located in `savesDir` and do each of the following three subphases on each
     #    `Register`:
     #    2a. Load the `Register` and check that it has a compatible version.
     #    2b. Create two dictionaries `combined` and `uncombined`, whose keys are tuples of all registers and their
     #    corresponding apris. The values of `combined` are the return values of
-    #    `reg.get_all_intervals(apri, combine = True)` and those of `uncombined` are the return values of
-    #    `reg.get_disk_block_intervals(apri)`.
+    #    `reg.get_all_intervals(info, combine = True)` and those of `uncombined` are the return values of
+    #    `reg.get_disk_block_intervals(info)`.
     #    2c. Apply the search parameters to obtain a `list` of `relevant` registers and apris.
     # 3. Print out descriptions of registers, apris, and blocks matching search criteria.
 
     ####################
     #     PHASE 1      #
 
     if saves_directory is None:
         saves_directory = Path.cwd()
 
     elif not isinstance(saves_directory, (Path, str)):
         raise TypeError("`savesDir` must be either a string or of type `pathlib.Path`.")
 
-    saves_directory = resolvePath(Path(saves_directory))
+    saves_directory = resolve_path(Path(saves_directory))
 
     # test that kwargs are hashable
     for key, val in kwargs.items():
 
         try:
             hash(val)
 
@@ -166,38 +166,38 @@
     combined = {}
     uncombined = {}
     warnings_ = []
     relevant = []
     for local_dir in saves_directory.iterdir():
 
         try:
-            checkRegStructure(local_dir)
+            check_reg_structure(local_dir)
 
         except FileNotFoundError:
             is_register = False
 
         else:
             is_register = True
 
         if is_register:
 
             ####################
             #     PHASE 2a     #
 
             # load register
             try:
-                reg = Register._fromLocalDir(local_dir)
+                reg = Register._from_local_dir(local_dir)
 
             except (RegisterError, TypeError) as m:
                 warnings_.append(f"`Register` at `{str(local_dir)}` not loaded. Error text: {str(m)}")
                 continue
 
             # test if compatible register
-            if not reg._hasCompatibleVersion():
-                if _args["printIncompatibleRegs"]:
+            if not reg._has_compatible_version():
+                if _args["print_incompatible_regs"]:
                     warnings_.append(f"`Register` at `{str(local_dir)}` has an incompatible version.")
                 else:
                     continue
 
 
             ####################
             #     PHASE 2b     #
@@ -213,15 +213,15 @@
                     uncombined[reg, _apri] = reg.get_disk_block_intervals(_apri)
                     combined[reg, _apri] = reg.get_all_intervals(_apri, True, False)
 
             if encountered_error:
                 continue
 
 
-                # mode = _args["printIntervalMode"]
+                # mode = _args["print_interval_mode"]
 
                 # if mode == "disjoint_intervals":
                 #     pass
                 #
                 # elif mode == "block_intervals":
                 #     pass
                 #
@@ -234,44 +234,44 @@
                 # else:
                 #     raise ValueError(f"unrecognized search argument: print_block_mode : {mode}")
 
             ####################
             #     PHASE 2c     #
 
             if apri is not None and apri in apris:
-                # if the passed `apri` matches ANY of `apris`
+                # if the passed `info` matches ANY of `apris`
                 relevant.append((reg, apri))
 
             elif len(kwargs) > 0:
 
                 for _apri in apris:
                     # find all `_apri` matching ALL the search criteria
                     for (key, val), key_re in zip(kwargs.items(), key_res):
                         # iterate over user's search critera
                         for _key, _val in _apri.__dict__:
                             # iterate over `_apri` data
                             if (
-                                _key not in _apri._reservedKws and (
-                                    (key == _key and _args["keyExactMatch"]) or
-                                    (key_re.match(_key) is not None and not _args["keyExactMatch"])
+                                _key not in _apri._reserved_kws and (
+                                    (key == _key and _args["key_exact_match"]) or
+                                    (key_re.match(_key) is not None and not _args["key_exact_match"])
                                 ) and
                                 _val_match(val, _val)
                             ):
                                 # found match, move on to next search criteria
                                 break
                         else:
                             # if search criteria does not match `_apri`, then move on to next `_apri`
                             break
 
                     else:
                         # append iff the `else: break` clause is missed
                         relevant.append((reg, _apri))
 
             elif apri is None and len(kwargs) == 0:
-                # if no search criteria given, then append all apri
+                # if no search criteria given, then append all info
                 for _apri in apris:
                     relevant.append((reg, _apri))
 
     ####################
     #     PHASE 3      #
 
     prnt = ""
@@ -286,59 +286,59 @@
                 prnt += f"... and {len(warnings_) - i} more.\n"
                 break
 
             prnt += f"({i}) {w}\n"
 
         prnt += "\n"
 
-    relevant = sorted(relevant, key = lambda t: t[0]._localDir)
+    relevant = sorted(relevant, key = lambda t: t[0]._local_dir)
     current_reg = None
     reg_index = 0
     apri_index = 0
-    hit_apriLimit = False
+    hit_apri_limit = False
 
     prnt += "REGISTERS:\n"
     for reg,apri in relevant:
 
         if current_reg is None or current_reg != reg:
 
             current_reg = reg
-            prnt += f"({reg._localDir.name}) \"{str(reg)}\"\n"
-            hit_apriLimit = False
+            prnt += f"({reg._local_dir.name}) \"{str(reg)}\"\n"
+            hit_apri_limit = False
             apri_index = 0
 
             if current_reg is not None:
                 reg_index += 1
 
             else:
                 reg_index = 0
 
-        if reg_index >= _args["regLimit"]:
+        if reg_index >= _args["reg_limit"]:
 
             num_regs = len(set(_reg for _reg, _ in relevant))
             prnt += f"... and {num_regs - reg_index} more.\n"
             break
 
-        if _args["printApri"] and not hit_apriLimit:
+        if _args["print_apri"] and not hit_apri_limit:
 
-            if apri_index >= _args["apriLimit"]:
+            if apri_index >= _args["apri_limit"]:
 
-                hit_apriLimit = True
+                hit_apri_limit = True
                 num_apri = len(set(_apri for _reg,_apri in relevant if _reg == reg))
                 prnt += f"... and {num_apri - apri_index} more.\n"
 
             else:
 
                 prnt += f"\t{repr(apri)}\n"
 
-                if _args["printIntervals"]:
+                if _args["print_intervals"]:
 
-                    lim = _args["intervalLimit"]
+                    lim = _args["interval_limit"]
 
-                    if _args["printIntervalMode"] == "combined":
+                    if _args["print_interval_mode"] == "combined":
                         ints = combined[reg, apri]
 
                     else:
                         ints = uncombined[reg, apri]
 
                     if len(ints) > 0:
                         prnt += f"\t\t{str(ints[:lim])[1:-1]}"
@@ -355,29 +355,29 @@
 
 def _val_match(search_val, apri_val):
 
     if type(search_val) != type(apri_val):
         return False
 
     if isinstance(search_val, str):
-        if _args["strExactMatch"]:
+        if _args["str_exact_match"]:
             search_val = re.compile(search_val)
         else:
             return search_val == apri_val
 
     if isinstance(search_val, re.Pattern):
         return search_val.match(apri_val) is not None
 
     elif isinstance(search_val, dict):
-        if _args["dictExactMatch"]:
+        if _args["dict_exact_match"]:
             return search_val == apri_val
         else:
             return all(val == apri_val[key] for key, val in search_val.items())
 
     elif isinstance(search_val, tuple):
-        if _args["tupleExactMatch"]:
+        if _args["tuple_exact_match"]:
             return search_val == apri_val
         else:
             return search_val in apri_val
     else:
         return search_val == apri_val
```

### Comparing `cornifer-0.5.1/lib/cornifer/version.py` & `cornifer-0.6/lib/cornifer/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,10 +9,11 @@
 
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 """
 
-CURRENT_VERSION          = "0.5.1"
-COMPATIBLE_VERSIONS      = ["0.5", "0.5.1"]
+CURRENT_VERSION          = "0.6"
+COMPATIBLE_VERSIONS      = ["0.6"]
+
```

### Comparing `cornifer-0.5.1/setup.py` & `cornifer-0.6/setup.py`

 * *Files identical despite different names*

