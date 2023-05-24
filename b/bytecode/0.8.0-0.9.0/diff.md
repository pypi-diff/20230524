# Comparing `tmp/bytecode-0.8.0.tar.gz` & `tmp/bytecode-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bytecode-0.8.0.tar", last modified: Mon Feb 18 23:56:41 2019, max compression
+gzip compressed data, was "dist/bytecode-0.9.0.tar", last modified: Sun Dec  1 17:08:25 2019, max compression
```

## Comparing `bytecode-0.8.0.tar` & `bytecode-0.9.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 mdartiailh   (501) staff       (20)        0 2019-02-18 23:56:41.000000 bytecode-0.8.0/
--rw-r--r--   0 mdartiailh   (501) staff       (20)     2379 2019-02-18 23:56:41.000000 bytecode-0.8.0/PKG-INFO
--rw-r--r--   0 mdartiailh   (501) staff       (20)      136 2018-07-31 11:08:10.000000 bytecode-0.8.0/MANIFEST.in
--rw-r--r--   0 mdartiailh   (501) staff       (20)     1074 2018-07-31 11:08:10.000000 bytecode-0.8.0/COPYING
--rw-r--r--   0 mdartiailh   (501) staff       (20)     1884 2019-02-18 23:48:39.000000 bytecode-0.8.0/setup.py
--rw-r--r--   0 mdartiailh   (501) staff       (20)      496 2019-02-18 23:47:50.000000 bytecode-0.8.0/tox.ini
-drwxr-xr-x   0 mdartiailh   (501) staff       (20)        0 2019-02-18 23:56:41.000000 bytecode-0.8.0/bytecode.egg-info/
--rw-r--r--   0 mdartiailh   (501) staff       (20)     2379 2019-02-18 23:56:40.000000 bytecode-0.8.0/bytecode.egg-info/PKG-INFO
--rw-r--r--   0 mdartiailh   (501) staff       (20)      785 2019-02-18 23:56:41.000000 bytecode-0.8.0/bytecode.egg-info/SOURCES.txt
--rw-r--r--   0 mdartiailh   (501) staff       (20)       38 2019-02-18 23:56:40.000000 bytecode-0.8.0/bytecode.egg-info/requires.txt
--rw-r--r--   0 mdartiailh   (501) staff       (20)        9 2019-02-18 23:56:40.000000 bytecode-0.8.0/bytecode.egg-info/top_level.txt
--rw-r--r--   0 mdartiailh   (501) staff       (20)        1 2019-02-18 23:56:40.000000 bytecode-0.8.0/bytecode.egg-info/dependency_links.txt
-drwxr-xr-x   0 mdartiailh   (501) staff       (20)        0 2019-02-18 23:56:41.000000 bytecode-0.8.0/bytecode/
--rw-r--r--   0 mdartiailh   (501) staff       (20)    10025 2018-07-31 11:08:10.000000 bytecode-0.8.0/bytecode/cfg.py
--rw-r--r--   0 mdartiailh   (501) staff       (20)    18832 2018-09-06 01:54:29.000000 bytecode-0.8.0/bytecode/concrete.py
--rw-r--r--   0 mdartiailh   (501) staff       (20)     3449 2019-02-18 23:47:50.000000 bytecode-0.8.0/bytecode/flags.py
-drwxr-xr-x   0 mdartiailh   (501) staff       (20)        0 2019-02-18 23:56:41.000000 bytecode-0.8.0/bytecode/tests/
--rw-r--r--   0 mdartiailh   (501) staff       (20)    34707 2018-09-06 01:32:28.000000 bytecode-0.8.0/bytecode/tests/test_concrete.py
--rw-r--r--   0 mdartiailh   (501) staff       (20)     8442 2019-02-18 23:47:50.000000 bytecode-0.8.0/bytecode/tests/test_instr.py
--rw-r--r--   0 mdartiailh   (501) staff       (20)     6942 2018-07-31 11:08:10.000000 bytecode-0.8.0/bytecode/tests/test_misc.py
--rw-r--r--   0 mdartiailh   (501) staff       (20)    33875 2019-02-18 23:47:50.000000 bytecode-0.8.0/bytecode/tests/test_peephole_opt.py
--rw-r--r--   0 mdartiailh   (501) staff       (20)     1482 2018-07-31 11:08:10.000000 bytecode-0.8.0/bytecode/tests/test_code.py
--rw-r--r--   0 mdartiailh   (501) staff       (20)    25968 2019-02-18 23:47:50.000000 bytecode-0.8.0/bytecode/tests/test_cfg.py
--rw-r--r--   0 mdartiailh   (501) staff       (20)     4754 2018-07-31 11:08:10.000000 bytecode-0.8.0/bytecode/tests/__init__.py
--rw-r--r--   0 mdartiailh   (501) staff       (20)     4432 2018-07-31 11:08:10.000000 bytecode-0.8.0/bytecode/tests/test_bytecode.py
--rw-r--r--   0 mdartiailh   (501) staff       (20)     2702 2018-07-31 11:08:10.000000 bytecode-0.8.0/bytecode/tests/test_flags.py
--rw-r--r--   0 mdartiailh   (501) staff       (20)     3857 2019-02-18 23:48:51.000000 bytecode-0.8.0/bytecode/__init__.py
--rw-r--r--   0 mdartiailh   (501) staff       (20)    10931 2019-02-18 23:47:50.000000 bytecode-0.8.0/bytecode/instr.py
--rw-r--r--   0 mdartiailh   (501) staff       (20)    15748 2018-07-31 11:08:10.000000 bytecode-0.8.0/bytecode/peephole_opt.py
--rw-r--r--   0 mdartiailh   (501) staff       (20)     4763 2018-07-31 11:08:10.000000 bytecode-0.8.0/bytecode/bytecode.py
-drwxr-xr-x   0 mdartiailh   (501) staff       (20)        0 2019-02-18 23:56:41.000000 bytecode-0.8.0/doc/
--rw-r--r--   0 mdartiailh   (501) staff       (20)      946 2018-07-31 11:08:10.000000 bytecode-0.8.0/doc/index.rst
--rw-r--r--   0 mdartiailh   (501) staff       (20)     4287 2018-07-31 11:08:10.000000 bytecode-0.8.0/doc/byteplay_codetransformer.rst
--rw-r--r--   0 mdartiailh   (501) staff       (20)     1154 2018-07-31 11:08:10.000000 bytecode-0.8.0/doc/todo.rst
--rw-r--r--   0 mdartiailh   (501) staff       (20)     6769 2018-07-31 11:08:10.000000 bytecode-0.8.0/doc/Makefile
--rw-r--r--   0 mdartiailh   (501) staff       (20)     8159 2019-02-18 23:49:06.000000 bytecode-0.8.0/doc/conf.py
--rw-r--r--   0 mdartiailh   (501) staff       (20)     4121 2018-07-31 11:08:10.000000 bytecode-0.8.0/doc/peephole.rst
--rw-r--r--   0 mdartiailh   (501) staff       (20)     4197 2018-07-31 11:08:10.000000 bytecode-0.8.0/doc/usage.rst
--rw-r--r--   0 mdartiailh   (501) staff       (20)     6704 2018-07-31 11:08:10.000000 bytecode-0.8.0/doc/make.bat
--rw-r--r--   0 mdartiailh   (501) staff       (20)     6028 2019-02-18 23:49:35.000000 bytecode-0.8.0/doc/changelog.rst
--rw-r--r--   0 mdartiailh   (501) staff       (20)     7071 2018-07-31 11:08:10.000000 bytecode-0.8.0/doc/cfg.rst
--rw-r--r--   0 mdartiailh   (501) staff       (20)    18798 2018-07-31 11:08:10.000000 bytecode-0.8.0/doc/api.rst
--rw-r--r--   0 mdartiailh   (501) staff       (20)       38 2019-02-18 23:56:41.000000 bytecode-0.8.0/setup.cfg
--rw-r--r--   0 mdartiailh   (501) staff       (20)     1436 2019-02-18 23:47:50.000000 bytecode-0.8.0/README.rst
+drwxr-xr-x   0 mdartiailh   (501) staff       (20)        0 2019-12-01 17:08:25.000000 bytecode-0.9.0/
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     1074 2018-07-31 11:08:10.000000 bytecode-0.9.0/COPYING
+-rw-r--r--   0 mdartiailh   (501) staff       (20)      136 2018-07-31 11:08:10.000000 bytecode-0.9.0/MANIFEST.in
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     2379 2019-12-01 17:08:25.000000 bytecode-0.9.0/PKG-INFO
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     1436 2019-02-18 23:47:50.000000 bytecode-0.9.0/README.rst
+drwxr-xr-x   0 mdartiailh   (501) staff       (20)        0 2019-12-01 17:08:25.000000 bytecode-0.9.0/bytecode/
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     3857 2019-12-01 16:57:07.000000 bytecode-0.9.0/bytecode/__init__.py
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     5076 2019-10-23 23:16:58.000000 bytecode-0.9.0/bytecode/bytecode.py
+-rw-r--r--   0 mdartiailh   (501) staff       (20)    10025 2018-07-31 11:08:10.000000 bytecode-0.9.0/bytecode/cfg.py
+-rw-r--r--   0 mdartiailh   (501) staff       (20)    19938 2019-10-23 23:16:58.000000 bytecode-0.9.0/bytecode/concrete.py
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     3445 2019-10-23 23:16:58.000000 bytecode-0.9.0/bytecode/flags.py
+-rw-r--r--   0 mdartiailh   (501) staff       (20)    10931 2019-02-18 23:47:50.000000 bytecode-0.9.0/bytecode/instr.py
+-rw-r--r--   0 mdartiailh   (501) staff       (20)    15748 2018-07-31 11:08:10.000000 bytecode-0.9.0/bytecode/peephole_opt.py
+drwxr-xr-x   0 mdartiailh   (501) staff       (20)        0 2019-12-01 17:08:25.000000 bytecode-0.9.0/bytecode/tests/
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     4930 2019-10-23 23:16:58.000000 bytecode-0.9.0/bytecode/tests/__init__.py
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     4432 2019-08-22 02:14:56.000000 bytecode-0.9.0/bytecode/tests/test_bytecode.py
+-rw-r--r--   0 mdartiailh   (501) staff       (20)    26234 2019-10-23 23:16:58.000000 bytecode-0.9.0/bytecode/tests/test_cfg.py
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     1482 2018-07-31 11:08:10.000000 bytecode-0.9.0/bytecode/tests/test_code.py
+-rw-r--r--   0 mdartiailh   (501) staff       (20)    34662 2019-10-23 23:16:58.000000 bytecode-0.9.0/bytecode/tests/test_concrete.py
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     2702 2019-10-23 23:16:58.000000 bytecode-0.9.0/bytecode/tests/test_flags.py
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     8442 2019-02-18 23:47:50.000000 bytecode-0.9.0/bytecode/tests/test_instr.py
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     6942 2018-07-31 11:08:10.000000 bytecode-0.9.0/bytecode/tests/test_misc.py
+-rw-r--r--   0 mdartiailh   (501) staff       (20)    33875 2019-02-18 23:47:50.000000 bytecode-0.9.0/bytecode/tests/test_peephole_opt.py
+drwxr-xr-x   0 mdartiailh   (501) staff       (20)        0 2019-12-01 17:08:25.000000 bytecode-0.9.0/bytecode.egg-info/
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     2379 2019-12-01 17:08:25.000000 bytecode-0.9.0/bytecode.egg-info/PKG-INFO
+-rw-r--r--   0 mdartiailh   (501) staff       (20)      785 2019-12-01 17:08:25.000000 bytecode-0.9.0/bytecode.egg-info/SOURCES.txt
+-rw-r--r--   0 mdartiailh   (501) staff       (20)        1 2019-12-01 17:08:25.000000 bytecode-0.9.0/bytecode.egg-info/dependency_links.txt
+-rw-r--r--   0 mdartiailh   (501) staff       (20)       38 2019-12-01 17:08:25.000000 bytecode-0.9.0/bytecode.egg-info/requires.txt
+-rw-r--r--   0 mdartiailh   (501) staff       (20)        9 2019-12-01 17:08:25.000000 bytecode-0.9.0/bytecode.egg-info/top_level.txt
+drwxr-xr-x   0 mdartiailh   (501) staff       (20)        0 2019-12-01 17:08:25.000000 bytecode-0.9.0/doc/
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     6769 2018-07-31 11:08:10.000000 bytecode-0.9.0/doc/Makefile
+-rw-r--r--   0 mdartiailh   (501) staff       (20)    18923 2019-11-03 00:39:35.000000 bytecode-0.9.0/doc/api.rst
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     4287 2019-11-03 00:39:35.000000 bytecode-0.9.0/doc/byteplay_codetransformer.rst
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     7071 2019-11-03 00:39:35.000000 bytecode-0.9.0/doc/cfg.rst
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     6173 2019-12-01 17:00:06.000000 bytecode-0.9.0/doc/changelog.rst
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     8177 2019-12-01 16:57:29.000000 bytecode-0.9.0/doc/conf.py
+-rw-r--r--   0 mdartiailh   (501) staff       (20)      946 2019-11-03 00:39:35.000000 bytecode-0.9.0/doc/index.rst
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     6704 2018-07-31 11:08:10.000000 bytecode-0.9.0/doc/make.bat
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     4121 2019-11-03 00:39:35.000000 bytecode-0.9.0/doc/peephole.rst
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     1154 2019-11-03 00:39:35.000000 bytecode-0.9.0/doc/todo.rst
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     5700 2019-12-01 16:56:08.000000 bytecode-0.9.0/doc/usage.rst
+-rw-r--r--   0 mdartiailh   (501) staff       (20)       38 2019-12-01 17:08:25.000000 bytecode-0.9.0/setup.cfg
+-rw-r--r--   0 mdartiailh   (501) staff       (20)     1884 2019-12-01 16:57:42.000000 bytecode-0.9.0/setup.py
+-rw-r--r--   0 mdartiailh   (501) staff       (20)      502 2019-10-23 23:16:58.000000 bytecode-0.9.0/tox.ini
```

### Comparing `bytecode-0.8.0/PKG-INFO` & `bytecode-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bytecode
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python module to generate and modify bytecode
 Home-page: https://github.com/vstinner/bytecode
 Author: Victor Stinner
 Author-email: victor.stinner@gmail.com
 License: MIT license
 Description: ********
         bytecode
```

### Comparing `bytecode-0.8.0/COPYING` & `bytecode-0.9.0/COPYING`

 * *Files identical despite different names*

### Comparing `bytecode-0.8.0/setup.py` & `bytecode-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 #
 # After the release:
 #
 #  - set version to n+1
 #  - git commit -a -m "post-release"
 #  - git push
 
-VERSION = '0.8.0'
+VERSION = '0.9.0'
 
 DESCRIPTION = 'Python module to generate and modify bytecode'
 CLASSIFIERS = [
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Natural Language :: English',
```

### Comparing `bytecode-0.8.0/bytecode.egg-info/PKG-INFO` & `bytecode-0.9.0/bytecode.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bytecode
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python module to generate and modify bytecode
 Home-page: https://github.com/vstinner/bytecode
 Author: Victor Stinner
 Author-email: victor.stinner@gmail.com
 License: MIT license
 Description: ********
         bytecode
```

### Comparing `bytecode-0.8.0/bytecode.egg-info/SOURCES.txt` & `bytecode-0.9.0/bytecode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bytecode-0.8.0/bytecode/cfg.py` & `bytecode-0.9.0/bytecode/cfg.py`

 * *Files identical despite different names*

### Comparing `bytecode-0.8.0/bytecode/concrete.py` & `bytecode-0.9.0/bytecode/concrete.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,14 +236,16 @@
                 raise ValueError("EXTENDED_ARG at the end of the code")
 
         bytecode = ConcreteBytecode()
         bytecode.name = code.co_name
         bytecode.filename = code.co_filename
         bytecode.flags = code.co_flags
         bytecode.argcount = code.co_argcount
+        if sys.version_info >= (3, 8):
+            bytecode.posonlyargcount = code.co_posonlyargcount
         bytecode.kwonlyargcount = code.co_kwonlyargcount
         bytecode.first_lineno = code.co_firstlineno
         bytecode.names = list(code.co_names)
         bytecode.consts = list(code.co_consts)
         bytecode.varnames = list(code.co_varnames)
         bytecode.freevars = list(code.co_freevars)
         bytecode.cellvars = list(code.co_cellvars)
@@ -318,29 +320,48 @@
 
     def to_code(self, stacksize=None):
         code_str, linenos = self._assemble_code()
         lnotab = self._assemble_lnotab(self.first_lineno, linenos)
         nlocals = len(self.varnames)
         if stacksize is None:
             stacksize = self.compute_stacksize()
-        return types.CodeType(self.argcount,
-                              self.kwonlyargcount,
-                              nlocals,
-                              stacksize,
-                              int(self.flags),
-                              code_str,
-                              tuple(self.consts),
-                              tuple(self.names),
-                              tuple(self.varnames),
-                              self.filename,
-                              self.name,
-                              self.first_lineno,
-                              lnotab,
-                              tuple(self.freevars),
-                              tuple(self.cellvars))
+
+        if sys.version_info < (3, 8):
+            return types.CodeType(self.argcount,
+                                  self.kwonlyargcount,
+                                  nlocals,
+                                  stacksize,
+                                  int(self.flags),
+                                  code_str,
+                                  tuple(self.consts),
+                                  tuple(self.names),
+                                  tuple(self.varnames),
+                                  self.filename,
+                                  self.name,
+                                  self.first_lineno,
+                                  lnotab,
+                                  tuple(self.freevars),
+                                  tuple(self.cellvars))
+        else:
+            return types.CodeType(self.argcount,
+                                  self.posonlyargcount,
+                                  self.kwonlyargcount,
+                                  nlocals,
+                                  stacksize,
+                                  int(self.flags),
+                                  code_str,
+                                  tuple(self.consts),
+                                  tuple(self.names),
+                                  tuple(self.varnames),
+                                  self.filename,
+                                  self.name,
+                                  self.first_lineno,
+                                  lnotab,
+                                  tuple(self.freevars),
+                                  tuple(self.cellvars))
 
     def to_bytecode(self):
         # find jump targets
         jump_targets = set()
         offset = 0
         for instr in self:
             if isinstance(instr, SetLineno):
@@ -401,14 +422,16 @@
             label = labels[jump_target]
             instructions[index] = Instr(instr.name, label, lineno=instr.lineno)
 
         bytecode = _bytecode.Bytecode()
         bytecode._copy_attr_from(self)
 
         nargs = bytecode.argcount + bytecode.kwonlyargcount
+        if sys.version_info > (3, 8):
+            nargs += bytecode.posonlyargcount
         if bytecode.flags & inspect.CO_VARARGS:
             nargs += 1
         if bytecode.flags & inspect.CO_VARKEYWORDS:
             nargs += 1
         bytecode.argnames = self.varnames[:nargs]
         _set_docstring(bytecode, self.consts)
```

### Comparing `bytecode-0.8.0/bytecode/flags.py` & `bytecode-0.9.0/bytecode/flags.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,34 +48,34 @@
     instr_names = {i.name for i in instructions
                    if not isinstance(i, (_bytecode.SetLineno,
                                          _bytecode.Label))}
 
     if not (instr_names & {'STORE_NAME', 'LOAD_NAME', 'DELETE_NAME'}):
         flags |= CompilerFlags.OPTIMIZED
 
-    flags |= bytecode.flags & (CompilerFlags.NEWLOCALS |
-                               CompilerFlags.VARARGS |
-                               CompilerFlags.VARKEYWORDS |
-                               CompilerFlags.NESTED)
+    flags |= bytecode.flags & (CompilerFlags.NEWLOCALS
+                               | CompilerFlags.VARARGS
+                               | CompilerFlags.VARKEYWORDS
+                               | CompilerFlags.NESTED)
 
     if instr_names & {'YIELD_VALUE', 'YIELD_FROM'}:
         if not is_async and not bytecode.flags & CompilerFlags.ASYNC_GENERATOR:
             flags |= CompilerFlags.GENERATOR
         else:
             flags |= CompilerFlags.ASYNC_GENERATOR
 
     if not (instr_names & {'LOAD_CLOSURE', 'LOAD_DEREF', 'STORE_DEREF',
                            'DELETE_DEREF', 'LOAD_CLASSDEREF'}):
         flags |= CompilerFlags.NOFREE
 
-    if (not (bytecode.flags & CompilerFlags.ITERABLE_COROUTINE or
-             flags & CompilerFlags.ASYNC_GENERATOR) and
-            (instr_names & {'GET_AWAITABLE', 'GET_AITER', 'GET_ANEXT',
-                            'BEFORE_ASYNC_WITH', 'SETUP_ASYNC_WITH'} or
-             bytecode.flags & CompilerFlags.COROUTINE)):
+    if (not (bytecode.flags & CompilerFlags.ITERABLE_COROUTINE
+             or flags & CompilerFlags.ASYNC_GENERATOR)
+        and (instr_names & {'GET_AWAITABLE', 'GET_AITER', 'GET_ANEXT',
+                            'BEFORE_ASYNC_WITH', 'SETUP_ASYNC_WITH'}
+             or bytecode.flags & CompilerFlags.COROUTINE)):
         flags |= CompilerFlags.COROUTINE
 
     flags |= bytecode.flags & CompilerFlags.ITERABLE_COROUTINE
 
     flags |= bytecode.flags & CompilerFlags.FUTURE_GENERATOR_STOP
 
     if ([bool(flags & getattr(CompilerFlags, k))
```

### Comparing `bytecode-0.8.0/bytecode/tests/test_concrete.py` & `bytecode-0.9.0/bytecode/tests/test_concrete.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,29 +383,33 @@
 class ConcreteFromCodeTests(TestCase):
 
     def test_extended_arg(self):
         # Create a code object from arbitrary bytecode
         co_code = (b'\x90\x12\x904\x90\xabd\xcd' if WORDCODE else
                    b'\x904\x12d\xcd\xab')
         code = get_code('x=1')
-        code = types.CodeType(code.co_argcount,
-                              code.co_kwonlyargcount,
-                              code.co_nlocals,
-                              code.co_stacksize,
-                              code.co_flags,
-                              co_code,
-                              code.co_consts,
-                              code.co_names,
-                              code.co_varnames,
-                              code.co_filename,
-                              code.co_name,
-                              code.co_firstlineno,
-                              code.co_lnotab,
-                              code.co_freevars,
-                              code.co_cellvars)
+        args = ((code.co_argcount,)
+                if sys.version_info < (3, 8) else
+                (code.co_argcount, code.co_posonlyargcount))
+        args += (code.co_kwonlyargcount,
+                 code.co_nlocals,
+                 code.co_stacksize,
+                 code.co_flags,
+                 co_code,
+                 code.co_consts,
+                 code.co_names,
+                 code.co_varnames,
+                 code.co_filename,
+                 code.co_name,
+                 code.co_firstlineno,
+                 code.co_lnotab,
+                 code.co_freevars,
+                 code.co_cellvars)
+
+        code = types.CodeType(*args)
 
         # without EXTENDED_ARG opcode
         bytecode = ConcreteBytecode.from_code(code)
         self.assertListEqual(list(bytecode),
                              [ConcreteInstr("LOAD_CONST", 0x1234abcd,
                                             lineno=1)])
```

### Comparing `bytecode-0.8.0/bytecode/tests/test_instr.py` & `bytecode-0.9.0/bytecode/tests/test_instr.py`

 * *Files identical despite different names*

### Comparing `bytecode-0.8.0/bytecode/tests/test_misc.py` & `bytecode-0.9.0/bytecode/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `bytecode-0.8.0/bytecode/tests/test_peephole_opt.py` & `bytecode-0.9.0/bytecode/tests/test_peephole_opt.py`

 * *Files identical despite different names*

### Comparing `bytecode-0.8.0/bytecode/tests/test_code.py` & `bytecode-0.9.0/bytecode/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `bytecode-0.8.0/bytecode/tests/test_cfg.py` & `bytecode-0.9.0/bytecode/tests/test_cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,16 @@
                 y = 2
                 return arg1
         """
         code = disassemble(source, filename="hello.py", function=True)
         self.assertEqual(code.argcount, 2)
         self.assertEqual(code.filename, "hello.py")
         self.assertEqual(code.first_lineno, 3)
+        if sys.version_info > (3, 8):
+            self.assertEqual(code.posonlyargcount, 0)
         self.assertEqual(code.kwonlyargcount, 1)
         self.assertEqual(code.name, "func")
         self.assertEqual(code.cellvars, [])
 
         code.name = "name"
         code.filename = "filename"
         code.flags = 123
@@ -409,14 +411,16 @@
             code.split_block(code[0], 3)
 
     def test_to_code(self):
         # test resolution of jump labels
         bytecode = ControlFlowGraph()
         bytecode.first_lineno = 3
         bytecode.argcount = 3
+        if sys.version_info > (3, 8):
+            bytecode.posonlyargcount = 0
         bytecode.kwonlyargcount = 2
         bytecode.name = 'func'
         bytecode.filename = 'hello.py'
         bytecode.flags = 0x43
         bytecode.argnames = ('arg', 'arg2', 'arg3', 'kwonly', 'kwonly2')
         bytecode.docstring = None
         block0 = bytecode[0]
@@ -449,14 +453,16 @@
                         b'}\x05\x00'
                         b'|\x05\x00'
                         b'S')
 
         code = bytecode.to_code()
         self.assertEqual(code.co_consts, (None, 3))
         self.assertEqual(code.co_argcount, 3)
+        if sys.version_info > (3, 8):
+            self.assertEqual(code.co_posonlyargcount, 0)
         self.assertEqual(code.co_kwonlyargcount, 2)
         self.assertEqual(code.co_nlocals, 6)
         self.assertEqual(code.co_stacksize, 1)
         # FIXME: don't use hardcoded constants
         self.assertEqual(code.co_flags, 0x43)
         self.assertEqual(code.co_code, expected)
         self.assertEqual(code.co_names, ())
```

### Comparing `bytecode-0.8.0/bytecode/tests/__init__.py` & `bytecode-0.9.0/bytecode/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,19 @@
                 labels[instr] = name
 
         if is_concrete:
             name = 'ConcreteBytecode'
             print(indent + 'code = %s()' % name)
             if code.argcount:
                 print(indent + 'code.argcount = %s' % code.argcount)
+            if sys.version_info > (3, 8):
+                if code.posonlyargcount:
+                    print(indent + 'code.posonlyargcount = %s' % code.posonlyargcount)
             if code.kwonlyargcount:
-                print(indent + 'code.argcount = %s' % code.kwonlyargcount)
+                print(indent + 'code.kwargonlycount = %s' % code.kwonlyargcount)
             print(indent + 'code.flags = %#x' % code.flags)
             if code.consts:
                 print(indent + 'code.consts = %r' % code.consts)
             if code.names:
                 print(indent + 'code.names = %r' % code.names)
             if code.varnames:
                 print(indent + 'code.varnames = %r' % code.varnames)
```

### Comparing `bytecode-0.8.0/bytecode/tests/test_bytecode.py` & `bytecode-0.9.0/bytecode/tests/test_bytecode.py`

 * *Files identical despite different names*

### Comparing `bytecode-0.8.0/bytecode/tests/test_flags.py` & `bytecode-0.9.0/bytecode/tests/test_flags.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 class FlagsTests(unittest.TestCase):
 
     def test_flag_inference(self):
 
         # Check no loss of non-infered flags
         code = ControlFlowGraph()
-        code.flags |= (CompilerFlags.NEWLOCALS | CompilerFlags.VARARGS |
-                       CompilerFlags.VARKEYWORDS | CompilerFlags.NESTED |
-                       CompilerFlags.FUTURE_GENERATOR_STOP)
+        code.flags |= (CompilerFlags.NEWLOCALS | CompilerFlags.VARARGS
+                       | CompilerFlags.VARKEYWORDS | CompilerFlags.NESTED
+                       | CompilerFlags.FUTURE_GENERATOR_STOP)
         code.update_flags()
         for f in (CompilerFlags.NEWLOCALS, CompilerFlags.VARARGS,
                   CompilerFlags.VARKEYWORDS, CompilerFlags.NESTED,
                   CompilerFlags.NOFREE, CompilerFlags.OPTIMIZED,
                   CompilerFlags.FUTURE_GENERATOR_STOP):
             self.assertTrue(bool(code.flags & f))
 
@@ -49,15 +49,15 @@
         for f, expected in ((CompilerFlags(0), True), (iter_flags, False)):
             code.flags = f
             self.assertEqual(bool(infer_flags(code) & CompilerFlags.COROUTINE),
                              expected)
 
         # Test check flag sanity
         code.append(ConcreteInstr('YIELD_VALUE'))
-        code.flags = CompilerFlags(CompilerFlags.GENERATOR |
-                                   CompilerFlags.COROUTINE)
+        code.flags = CompilerFlags(CompilerFlags.GENERATOR
+                                   | CompilerFlags.COROUTINE)
         infer_flags(code, is_async=True)  # Just want to be sure it pases
         with self.assertRaises(ValueError):
             code.update_flags()
 
         with self.assertRaises(ValueError):
             infer_flags(None)
```

### Comparing `bytecode-0.8.0/bytecode/__init__.py` & `bytecode-0.9.0/bytecode/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 
 __all__ = ['Label', 'Instr', 'SetLineno', 'Bytecode',
            'ConcreteInstr', 'ConcreteBytecode',
            'ControlFlowGraph', 'CompilerFlags']
 
 from bytecode.flags import CompilerFlags
 from bytecode.instr import (UNSET, Label, SetLineno, Instr, CellVar, FreeVar,   # noqa
```

### Comparing `bytecode-0.8.0/bytecode/instr.py` & `bytecode-0.9.0/bytecode/instr.py`

 * *Files identical despite different names*

### Comparing `bytecode-0.8.0/bytecode/peephole_opt.py` & `bytecode-0.9.0/bytecode/peephole_opt.py`

 * *Files identical despite different names*

### Comparing `bytecode-0.8.0/bytecode/bytecode.py` & `bytecode-0.9.0/bytecode/bytecode.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 # alias to keep the 'bytecode' variable free
+import sys
 import bytecode as _bytecode
 from bytecode.instr import UNSET, Label, SetLineno, Instr
 from bytecode.flags import infer_flags
 
 
 class BaseBytecode:
 
     def __init__(self):
         self.argcount = 0
+        if sys.version_info > (3, 8):
+            self.posonlyargcount = 0
         self.kwonlyargcount = 0
         self.first_lineno = 1
         self.name = '<module>'
         self.filename = '<string>'
         self.docstring = UNSET
         self.cellvars = []
         # we cannot recreate freevars from instructions because of super()
         # special-case
         self.freevars = []
         self._flags = _bytecode.CompilerFlags(0)
 
     def _copy_attr_from(self, bytecode):
         self.argcount = bytecode.argcount
+        if sys.version_info > (3, 8):
+            self.posonlyargcount = bytecode.posonlyargcount
         self.kwonlyargcount = bytecode.kwonlyargcount
         self.flags = bytecode.flags
         self.first_lineno = bytecode.first_lineno
         self.name = bytecode.name
         self.filename = bytecode.filename
         self.docstring = bytecode.docstring
         self.cellvars = list(bytecode.cellvars)
@@ -32,14 +37,17 @@
 
     def __eq__(self, other):
         if type(self) != type(other):
             return False
 
         if self.argcount != other.argcount:
             return False
+        if sys.version_info > (3, 8):
+            if self.posonlyargcount != other.posonlyargcount:
+                return False
         if self.kwonlyargcount != other.kwonlyargcount:
             return False
         if self.compute_stacksize() != other.compute_stacksize():
             return False
         if self.flags != other.flags:
             return False
         if self.first_lineno != other.first_lineno:
```

### Comparing `bytecode-0.8.0/doc/index.rst` & `bytecode-0.9.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `bytecode-0.8.0/doc/byteplay_codetransformer.rst` & `bytecode-0.9.0/doc/byteplay_codetransformer.rst`

 * *Files identical despite different names*

### Comparing `bytecode-0.8.0/doc/todo.rst` & `bytecode-0.9.0/doc/todo.rst`

 * *Files identical despite different names*

### Comparing `bytecode-0.8.0/doc/Makefile` & `bytecode-0.9.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `bytecode-0.8.0/doc/conf.py` & `bytecode-0.9.0/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = []
+extensions = ['sphinx_tabs.tabs']
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
 
@@ -48,15 +48,15 @@
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 # The full version, including alpha/beta/rc tags.
-version = release = '0.8.0'
+version = release = '0.9.0'
 
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
```

### Comparing `bytecode-0.8.0/doc/peephole.rst` & `bytecode-0.9.0/doc/peephole.rst`

 * *Files identical despite different names*

### Comparing `bytecode-0.8.0/doc/make.bat` & `bytecode-0.9.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `bytecode-0.8.0/doc/changelog.rst` & `bytecode-0.9.0/doc/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 ChangeLog
 =========
 
+2019-12-01: Version 0.9.0
+-------------------------
+
+New features:
+
+- Add support for released version of Python 3.8 and update documentation.
+
+
 2019-02-18: Version 0.8.0
 -------------------------
 
 New features:
 
 - Add support for Python 3.7 PR #29
 - Add preliminary support for Python 3.8-dev PR #41
```

### Comparing `bytecode-0.8.0/doc/cfg.rst` & `bytecode-0.9.0/doc/cfg.rst`

 * *Files identical despite different names*

### Comparing `bytecode-0.8.0/doc/api.rst` & `bytecode-0.9.0/doc/api.rst`

 * *Files 1% similar despite different names*

```diff
@@ -309,14 +309,20 @@
 
       Flags (``int``).
 
    .. attribute:: freevars
 
       List of free variable names (``list`` of ``str``), default: empty list.
 
+   .. attribute:: posonlyargcount
+
+      Positional-only argument count (``int``), default: ``0``.
+
+      New in Python 3.8
+
    .. attribute:: kwonlyargcount
 
       Keyword-only argument count (``int``), default: ``0``.
 
    .. attribute:: name
 
       Code name (``str``), default: ``'<module>'``.
```

### Comparing `bytecode-0.8.0/README.rst` & `bytecode-0.9.0/README.rst`

 * *Files identical despite different names*

