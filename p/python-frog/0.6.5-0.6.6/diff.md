# Comparing `tmp/python-frog-0.6.5.tar.gz` & `tmp/python-frog-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-frog-0.6.5.tar", last modified: Wed Feb 22 14:09:51 2023, max compression
+gzip compressed data, was "python-frog-0.6.6.tar", last modified: Wed May 24 13:42:57 2023, max compression
```

## Comparing `python-frog-0.6.5.tar` & `python-frog-0.6.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-02-22 14:09:51.304506 python-frog-0.6.5/
--rw-r--r--   0 proycon   (1000) users      (100)    35147 2019-10-30 11:03:12.000000 python-frog-0.6.5/LICENSE
--rw-r--r--   0 proycon   (1000) users      (100)      910 2023-02-22 14:09:51.304506 python-frog-0.6.5/PKG-INFO
--rw-r--r--   0 proycon   (1000) users      (100)     6899 2022-12-21 12:31:48.000000 python-frog-0.6.5/README.rst
--rw-r--r--   0 proycon   (1000) users      (100)     1770 2021-04-22 11:44:31.000000 python-frog-0.6.5/frog_classes.pxd
--rw-r--r--   0 proycon   (1000) users      (100)   553976 2023-02-22 14:09:51.000000 python-frog-0.6.5/frog_wrapper.cpp
--rw-r--r--   0 proycon   (1000) users      (100)    12536 2022-07-22 10:47:23.000000 python-frog-0.6.5/frog_wrapper.pyx
--rw-r--r--   0 proycon   (1000) users      (100)     2854 2016-03-13 14:45:13.000000 python-frog-0.6.5/libfolia_classes.pxd
--rw-r--r--   0 proycon   (1000) users      (100)      119 2022-11-30 17:18:33.000000 python-frog-0.6.5/pyproject.toml
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-02-22 14:09:51.304506 python-frog-0.6.5/python_frog.egg-info/
--rw-r--r--   0 proycon   (1000) users      (100)      910 2023-02-22 14:09:51.000000 python-frog-0.6.5/python_frog.egg-info/PKG-INFO
--rw-r--r--   0 proycon   (1000) users      (100)      298 2023-02-22 14:09:51.000000 python-frog-0.6.5/python_frog.egg-info/SOURCES.txt
--rw-r--r--   0 proycon   (1000) users      (100)        1 2023-02-22 14:09:51.000000 python-frog-0.6.5/python_frog.egg-info/dependency_links.txt
--rw-r--r--   0 proycon   (1000) users      (100)        7 2023-02-22 14:09:51.000000 python-frog-0.6.5/python_frog.egg-info/requires.txt
--rw-r--r--   0 proycon   (1000) users      (100)        5 2023-02-22 14:09:51.000000 python-frog-0.6.5/python_frog.egg-info/top_level.txt
--rw-r--r--   0 proycon   (1000) users      (100)       61 2023-02-22 14:09:51.304506 python-frog-0.6.5/setup.cfg
--rwxr-xr-x   0 proycon   (1000) users      (100)     3572 2023-02-22 11:50:18.000000 python-frog-0.6.5/setup.py
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-24 13:42:57.852463 python-frog-0.6.6/
+-rw-r--r--   0 proycon   (1000) users      (100)    35147 2019-10-30 11:03:12.000000 python-frog-0.6.6/LICENSE
+-rw-r--r--   0 proycon   (1000) users      (100)      910 2023-05-24 13:42:57.852463 python-frog-0.6.6/PKG-INFO
+-rw-r--r--   0 proycon   (1000) users      (100)     6899 2022-12-21 12:31:48.000000 python-frog-0.6.6/README.rst
+-rw-r--r--   0 proycon   (1000) users      (100)     1770 2021-04-22 11:44:31.000000 python-frog-0.6.6/frog_classes.pxd
+-rw-r--r--   0 proycon   (1000) users      (100)   577891 2023-05-24 13:42:57.000000 python-frog-0.6.6/frog_wrapper.cpp
+-rw-r--r--   0 proycon   (1000) users      (100)    13122 2023-02-23 17:28:44.000000 python-frog-0.6.6/frog_wrapper.pyx
+-rw-r--r--   0 proycon   (1000) users      (100)     2854 2016-03-13 14:45:13.000000 python-frog-0.6.6/libfolia_classes.pxd
+-rw-r--r--   0 proycon   (1000) users      (100)      119 2022-11-30 17:18:33.000000 python-frog-0.6.6/pyproject.toml
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-24 13:42:57.852463 python-frog-0.6.6/python_frog.egg-info/
+-rw-r--r--   0 proycon   (1000) users      (100)      910 2023-05-24 13:42:57.000000 python-frog-0.6.6/python_frog.egg-info/PKG-INFO
+-rw-r--r--   0 proycon   (1000) users      (100)      298 2023-05-24 13:42:57.000000 python-frog-0.6.6/python_frog.egg-info/SOURCES.txt
+-rw-r--r--   0 proycon   (1000) users      (100)        1 2023-05-24 13:42:57.000000 python-frog-0.6.6/python_frog.egg-info/dependency_links.txt
+-rw-r--r--   0 proycon   (1000) users      (100)        7 2023-05-24 13:42:57.000000 python-frog-0.6.6/python_frog.egg-info/requires.txt
+-rw-r--r--   0 proycon   (1000) users      (100)        5 2023-05-24 13:42:57.000000 python-frog-0.6.6/python_frog.egg-info/top_level.txt
+-rw-r--r--   0 proycon   (1000) users      (100)       61 2023-05-24 13:42:57.852463 python-frog-0.6.6/setup.cfg
+-rwxr-xr-x   0 proycon   (1000) users      (100)     3572 2023-05-24 12:24:24.000000 python-frog-0.6.6/setup.py
```

### Comparing `python-frog-0.6.5/LICENSE` & `python-frog-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python-frog-0.6.5/PKG-INFO` & `python-frog-0.6.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: python-frog
-Version: 0.6.5
+Version: 0.6.6
 Summary: Python binding to Frog, an NLP suite for Dutch doing part-of-speech tagging, lemmatisation, morphological analysis, named-entity recognition, shallow parsing, and dependency parsing.
 Home-page: https://github.com/proycon/python-frog
 Author: Maarten van Gompel
 Author-email: proycon@anaproy.nl
 License: GPLv3
 Keywords: nlp computational_linguistics dutch pos lemmatizer
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires: frog (>=0.27)
-Requires: ucto (>=0.28)
+Requires: frog (>=0.30)
+Requires: ucto (>=0.29)
 License-File: LICENSE
```

### Comparing `python-frog-0.6.5/README.rst` & `python-frog-0.6.6/README.rst`

 * *Files identical despite different names*

### Comparing `python-frog-0.6.5/frog_classes.pxd` & `python-frog-0.6.6/frog_classes.pxd`

 * *Files identical despite different names*

### Comparing `python-frog-0.6.5/frog_wrapper.cpp` & `python-frog-0.6.6/frog_wrapper.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
-        "depends": [
-            "/usr/include/libfolia/folia.h",
-            "/usr/include/ticcutils/CommandLine.h",
-            "/usr/include/ticcutils/Configuration.h",
-            "/usr/include/ticcutils/LogStream.h"
-        ],
+        "depends": [],
         "extra_compile_args": [
             "--std=c++0x",
             "-D U_USING_ICU_NAMESPACE=1"
         ],
         "include_dirs": [
+            "/home/proycon/work/python-frog/env/include",
             "/usr/include/",
             "/usr/include/libxml2",
             "/usr/local/include/"
         ],
         "language": "c++",
         "libraries": [
             "frog",
             "ucto",
             "folia"
         ],
         "library_dirs": [
+            "/home/proycon/work/python-frog/env/lib",
             "/usr/lib",
             "/usr/local/lib"
         ],
         "name": "frog",
         "sources": [
             "frog_wrapper.pyx",
             "libfolia_classes.pxd",
@@ -44,16 +41,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -238,15 +235,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -277,15 +274,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1514,14 +1511,64 @@
         PyObject* obj, Py_ssize_t cstart, Py_ssize_t cstop,
         PyObject** py_start, PyObject** py_stop, PyObject** py_slice,
         int has_cstart, int has_cstop, int wraparound);
 
 /* PyIntCompare.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_NeObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
 
+/* PyObjectLookupSpecial.proto */
+#if CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject* __Pyx_PyObject_LookupSpecial(PyObject* obj, PyObject* attr_name) {
+    PyObject *res;
+    PyTypeObject *tp = Py_TYPE(obj);
+#if PY_MAJOR_VERSION < 3
+    if (unlikely(PyInstance_Check(obj)))
+        return __Pyx_PyObject_GetAttrStr(obj, attr_name);
+#endif
+    res = _PyType_Lookup(tp, attr_name);
+    if (likely(res)) {
+        descrgetfunc f = Py_TYPE(res)->tp_descr_get;
+        if (!f) {
+            Py_INCREF(res);
+        } else {
+            res = f(res, obj, (PyObject *)tp);
+        }
+    } else {
+        PyErr_SetObject(PyExc_AttributeError, attr_name);
+    }
+    return res;
+}
+#else
+#define __Pyx_PyObject_LookupSpecial(o,n) __Pyx_PyObject_GetAttrStr(o,n)
+#endif
+
+/* GetTopmostException.proto */
+#if CYTHON_USE_EXC_INFO_STACK
+static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+#endif
+
+/* SaveResetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+#else
+#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
+#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
+#endif
+
+/* GetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+#endif
+
 /* PyObject_GenericGetAttrNoDict.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
 #endif
 
@@ -1548,38 +1595,14 @@
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
-/* GetTopmostException.proto */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
-#endif
-
-/* SaveResetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-#else
-#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
-#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
-#endif
-
-/* GetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
-#endif
-
 /* CalculateMetaclass.proto */
 static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases);
 
 /* Py3ClassCreate.proto */
 static PyObject *__Pyx_Py3MetaclassPrepare(PyObject *metaclass, PyObject *bases, PyObject *name, PyObject *qualname,
                                            PyObject *mkw, PyObject *modname, PyObject *doc);
 static PyObject *__Pyx_Py3ClassCreate(PyObject *metaclass, PyObject *name, PyObject *bases, PyObject *dict,
@@ -1684,24 +1707,28 @@
 /* Implementation of 'frog' */
 static PyObject *__pyx_builtin_ImportError;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_KeyError;
 static PyObject *__pyx_builtin_enumerate;
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_print;
+static PyObject *__pyx_builtin_open;
 static const char __pyx_k_1[] = "1";
 static const char __pyx_k_3[] = "3";
 static const char __pyx_k_X[] = "X";
 static const char __pyx_k_a[] = "a";
 static const char __pyx_k_c[] = "c";
+static const char __pyx_k_f[] = "f";
 static const char __pyx_k_l[] = "l";
 static const char __pyx_k_m[] = "m";
 static const char __pyx_k_n[] = "n";
 static const char __pyx_k_p[] = "p";
+static const char __pyx_k_r[] = "r";
 static const char __pyx_k_t[] = "t";
+static const char __pyx_k_w[] = "w";
 static const char __pyx_k_x[] = "x";
 static const char __pyx_k__3[] = "_";
 static const char __pyx_k__4[] = "-";
 static const char __pyx_k__6[] = "";
 static const char __pyx_k__9[] = "=";
 static const char __pyx_k_cd[] = "cd ";
 static const char __pyx_k_id[] = "id";
@@ -1722,43 +1749,49 @@
 static const char __pyx_k_pos[] = "pos";
 static const char __pyx_k_sys[] = "sys";
 static const char __pyx_k_tmp[] = "/tmp";
 static const char __pyx_k_tok[] = "tok";
 static const char __pyx_k_0_21[] = "0.21";
 static const char __pyx_k_Frog[] = "Frog";
 static const char __pyx_k_HOME[] = "HOME";
+static const char __pyx_k_data[] = "data";
+static const char __pyx_k_exit[] = "__exit__";
 static const char __pyx_k_file[] = "file";
 static const char __pyx_k_frog[] = "frog";
 static const char __pyx_k_item[] = "item";
 static const char __pyx_k_join[] = "join";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "name";
+static const char __pyx_k_open[] = "open";
 static const char __pyx_k_path[] = "path";
+static const char __pyx_k_read[] = "read";
 static const char __pyx_k_skip[] = "skip";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_text[] = "text";
 static const char __pyx_k_ucto[] = "ucto";
 static const char __pyx_k_0_9_1[] = "0.9.1";
 static const char __pyx_k_debug[] = "debug";
 static const char __pyx_k_docid[] = "docid";
 static const char __pyx_k_doiob[] = "doiob";
 static const char __pyx_k_domwu[] = "domwu";
 static const char __pyx_k_doner[] = "doner";
 static const char __pyx_k_dotok[] = "dotok";
+static const char __pyx_k_enter[] = "__enter__";
 static const char __pyx_k_index[] = "index";
 static const char __pyx_k_isdir[] = "isdir";
 static const char __pyx_k_items[] = "items";
 static const char __pyx_k_lemma[] = "lemma";
 static const char __pyx_k_lower[] = "lower";
 static const char __pyx_k_morph[] = "morph";
 static const char __pyx_k_parse[] = "parse";
 static const char __pyx_k_print[] = "print";
 static const char __pyx_k_split[] = "split";
 static const char __pyx_k_strip[] = "strip";
 static const char __pyx_k_utf_8[] = "utf-8";
+static const char __pyx_k_write[] = "write";
 static const char __pyx_k_xmlin[] = "xmlin";
 static const char __pyx_k_TMPDIR[] = "TMPDIR";
 static const char __pyx_k_config[] = "config";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_exists[] = "exists";
 static const char __pyx_k_finish[] = "finish";
 static const char __pyx_k_import[] = "__import__";
@@ -1794,14 +1827,15 @@
 static const char __pyx_k_chunking[] = "chunking";
 static const char __pyx_k_complete[] = " complete";
 static const char __pyx_k_compound[] = "compound";
 static const char __pyx_k_config_2[] = ".config";
 static const char __pyx_k_depindex[] = "depindex";
 static const char __pyx_k_doparser[] = "doparser";
 static const char __pyx_k_doxmlout[] = "doxmlout";
+static const char __pyx_k_encoding[] = "encoding";
 static const char __pyx_k_foliaout[] = "foliaout";
 static const char __pyx_k_frogdata[] = "/frogdata-";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_override[] = "override";
 static const char __pyx_k_qualname[] = "__qualname__";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_uctodata[] = "/uctodata-";
@@ -1820,20 +1854,23 @@
 static const char __pyx_k_dochunking[] = "dochunking";
 static const char __pyx_k_folia_main[] = "folia.main";
 static const char __pyx_k_numthreads[] = "numthreads";
 static const char __pyx_k_startswith[] = "startswith";
 static const char __pyx_k_FrogOptions[] = "FrogOptions";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_No_such_key[] = "No such key: ";
+static const char __pyx_k_TEXTCATPATH[] = "TEXTCATPATH";
 static const char __pyx_k_daringmorph[] = "daringmorph";
 static const char __pyx_k_doDeepMorph[] = "doDeepMorph";
 static const char __pyx_k_dodeepmorph[] = "dodeepmorph";
 static const char __pyx_k_encode_text[] = "_encode_text";
 static const char __pyx_k_installdata[] = "installdata";
 static const char __pyx_k_process_raw[] = "process_raw";
+static const char __pyx_k_textcat_cfg[] = "/textcat.cfg";
+static const char __pyx_k_textcatpath[] = "textcatpath";
 static const char __pyx_k_FROGDATAPATH[] = "FROGDATAPATH";
 static const char __pyx_k_parsecolumns[] = "parsecolumns";
 static const char __pyx_k_dodaringmorph[] = "dodaringmorph";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_does_not_exist[] = " does not exist!";
 static const char __pyx_k_shallowparsing[] = "shallowparsing";
 static const char __pyx_k_xdg_config_dir[] = "xdg_config_dir";
@@ -1868,15 +1905,15 @@
 static const char __pyx_k_does_not_exist_Try_running_frog[] = " does not exist! Try running frog.installdata() first";
 static const char __pyx_k_refusing_to_overwrite_please_re[] = ", refusing to overwrite, please remove it first if you want to install the data anew.";
 static const char __pyx_k_wget_O_frogdata_tar_gz_https_gi[] = " && wget -O frogdata.tar.gz https://github.com/LanguageMachines/frogdata/releases/download/v";
 static const char __pyx_k_wget_O_textcat_cfg_https_raw_gi[] = " && wget -O textcat.cfg https://raw.githubusercontent.com/LanguageMachines/ucto/master/config/textcat.cfg";
 static const char __pyx_k_wget_O_uctodata_tar_gz_https_gi[] = " && wget -O uctodata.tar.gz https://github.com/LanguageMachines/uctodata/releases/download/v";
 static const char __pyx_k_Frogdata_configuration_directory[] = "Frogdata configuration directory already exists: ";
 static const char __pyx_k_Installation_of_textcat_cfg_fail[] = "Installation of textcat.cfg failed.";
-static const char __pyx_k_Language_detection_will_not_be_a[] = "Language detection will not be available unless you install libexttextcat and rerun installdata()";
+static const char __pyx_k_Language_detection_will_not_be_a[] = "Language detection will not be available unless you install libexttextcat and rerun installdata(). Libexttextcat was not found. If it is in a non-standard location, set environment variable TEXTCATPATH (defaults to /usr/share/libexttextcat) prior to calling installdata()";
 static const char __pyx_k_Text_should_be_a_string_or_FoLiA[] = "Text should be a string or FoLiA Document instance";
 static const char __pyx_k_Uctodata_configuration_directory[] = "Uctodata configuration directory already exists: ";
 static const char __pyx_k_Unable_to_return_a_FoLiA_Documen[] = "Unable to return a FoLiA Document. FoLiAPy was not installed. Use process_raw() instead if you just want the XML output as string";
 static const char __pyx_k_self_capi_cannot_be_converted_to[] = "self.capi cannot be converted to a Python object for pickling";
 static const char __pyx_k_self_capi_self_debuglogstream_se[] = "self.capi,self.debuglogstream,self.logstream cannot be converted to a Python object for pickling";
 static PyObject *__pyx_kp_u_0_21;
 static PyObject *__pyx_kp_u_0_9_1;
@@ -1902,14 +1939,15 @@
 static PyObject *__pyx_kp_u_Installation_of_uctodata_failed;
 static PyObject *__pyx_n_s_KeyError;
 static PyObject *__pyx_kp_u_Language_detection_will_not_be_a;
 static PyObject *__pyx_kp_u_No_data_returned;
 static PyObject *__pyx_kp_u_No_such_key;
 static PyObject *__pyx_kp_u_Returned_data_is_not_XML_got;
 static PyObject *__pyx_kp_u_Specified_configuration_file;
+static PyObject *__pyx_n_u_TEXTCATPATH;
 static PyObject *__pyx_n_u_TMPDIR;
 static PyObject *__pyx_kp_u_Text_should_be_a_string_or_FoLiA;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_n_s_UCTODATAVERSION;
 static PyObject *__pyx_kp_u_Uctodata_configuration_directory;
 static PyObject *__pyx_kp_u_Unable_to_return_a_FoLiA_Documen;
 static PyObject *__pyx_n_s_ValueError;
@@ -1934,14 +1972,15 @@
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_kp_u_complete;
 static PyObject *__pyx_n_u_compound;
 static PyObject *__pyx_n_b_config;
 static PyObject *__pyx_kp_u_config_2;
 static PyObject *__pyx_n_s_configurationfile;
 static PyObject *__pyx_n_u_daringmorph;
+static PyObject *__pyx_n_s_data;
 static PyObject *__pyx_n_u_debug;
 static PyObject *__pyx_n_u_debugflag;
 static PyObject *__pyx_n_b_deepmorph;
 static PyObject *__pyx_n_u_deepmorph;
 static PyObject *__pyx_n_s_default;
 static PyObject *__pyx_n_u_dep;
 static PyObject *__pyx_n_u_depindex;
@@ -1961,18 +2000,22 @@
 static PyObject *__pyx_n_u_doparse;
 static PyObject *__pyx_n_u_doparser;
 static PyObject *__pyx_n_u_dotok;
 static PyObject *__pyx_n_u_doxmlin;
 static PyObject *__pyx_n_u_doxmlout;
 static PyObject *__pyx_n_s_encode;
 static PyObject *__pyx_n_s_encode_text;
+static PyObject *__pyx_n_s_encoding;
+static PyObject *__pyx_n_s_enter;
 static PyObject *__pyx_n_s_enumerate;
 static PyObject *__pyx_n_s_environ;
 static PyObject *__pyx_n_u_eos;
 static PyObject *__pyx_n_s_exists;
+static PyObject *__pyx_n_s_exit;
+static PyObject *__pyx_n_s_f;
 static PyObject *__pyx_n_s_file;
 static PyObject *__pyx_n_s_finish;
 static PyObject *__pyx_n_s_folia_main;
 static PyObject *__pyx_n_u_foliain;
 static PyObject *__pyx_n_u_foliaout;
 static PyObject *__pyx_n_s_frog;
 static PyObject *__pyx_n_u_frog;
@@ -2007,14 +2050,15 @@
 static PyObject *__pyx_n_u_mwu;
 static PyObject *__pyx_n_u_n;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_name_2;
 static PyObject *__pyx_n_u_ner;
 static PyObject *__pyx_n_b_nld;
 static PyObject *__pyx_n_u_numthreads;
+static PyObject *__pyx_n_s_open;
 static PyObject *__pyx_n_s_options;
 static PyObject *__pyx_n_s_os;
 static PyObject *__pyx_n_b_override;
 static PyObject *__pyx_n_s_overrides;
 static PyObject *__pyx_n_u_p;
 static PyObject *__pyx_n_u_parse;
 static PyObject *__pyx_n_s_parsecolumns;
@@ -2023,14 +2067,16 @@
 static PyObject *__pyx_n_u_pos;
 static PyObject *__pyx_n_u_posprob;
 static PyObject *__pyx_n_s_prepare;
 static PyObject *__pyx_n_s_print;
 static PyObject *__pyx_n_s_process_raw;
 static PyObject *__pyx_n_s_pynlpl_formats_folia;
 static PyObject *__pyx_n_s_qualname;
+static PyObject *__pyx_n_u_r;
+static PyObject *__pyx_n_s_read;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_kp_u_refusing_to_overwrite_please_re;
 static PyObject *__pyx_n_s_remove;
 static PyObject *__pyx_n_s_replace;
 static PyObject *__pyx_kp_u_rm_Rf_frogdata_tar_gz;
@@ -2050,29 +2096,33 @@
 static PyObject *__pyx_n_s_system;
 static PyObject *__pyx_n_u_t;
 static PyObject *__pyx_kp_u_tar_gz_tar_xzf_frogdata_tar_gz;
 static PyObject *__pyx_kp_u_tar_gz_tar_xzf_uctodata_tar_gz;
 static PyObject *__pyx_n_s_targetdir;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_u_text;
+static PyObject *__pyx_kp_u_textcat_cfg;
+static PyObject *__pyx_n_s_textcatpath;
 static PyObject *__pyx_n_b_threads;
 static PyObject *__pyx_n_u_threads;
 static PyObject *__pyx_kp_u_tmp;
 static PyObject *__pyx_n_s_tmpdir;
 static PyObject *__pyx_n_u_tok;
 static PyObject *__pyx_n_u_ucto;
 static PyObject *__pyx_kp_u_uctodata;
 static PyObject *__pyx_n_s_uctodataversion;
 static PyObject *__pyx_n_s_uctodir;
 static PyObject *__pyx_kp_u_usr_share_libexttextcat;
 static PyObject *__pyx_kp_u_utf_8;
 static PyObject *__pyx_n_s_version;
+static PyObject *__pyx_n_u_w;
 static PyObject *__pyx_kp_u_wget_O_frogdata_tar_gz_https_gi;
 static PyObject *__pyx_kp_u_wget_O_textcat_cfg_https_raw_gi;
 static PyObject *__pyx_kp_u_wget_O_uctodata_tar_gz_https_gi;
+static PyObject *__pyx_n_s_write;
 static PyObject *__pyx_n_u_x;
 static PyObject *__pyx_n_s_xdg_config_dir;
 static PyObject *__pyx_n_u_xmlin;
 static PyObject *__pyx_n_u_xmlout;
 static PyObject *__pyx_pf_4frog_8Document___reduce_cython__(CYTHON_UNUSED struct __pyx_obj_4frog_Document *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_4frog_8Document_2__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_4frog_Document *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_4frog_11FrogOptions___init__(struct __pyx_obj_4frog_FrogOptions *__pyx_v_self, PyObject *__pyx_v_kwargs); /* proto */
@@ -2093,39 +2143,43 @@
 static PyObject *__pyx_pf_4frog_2installdata(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_targetdir, PyObject *__pyx_v_frogdataversion, PyObject *__pyx_v_uctodataversion); /* proto */
 static PyObject *__pyx_tp_new_4frog_Document(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_4frog_FrogOptions(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_4frog_Frog(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_25;
+static PyObject *__pyx_int_neg_1;
 static PyObject *__pyx_k__23;
 static PyObject *__pyx_k__24;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_slice__18;
+static PyObject *__pyx_slice__30;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__15;
 static PyObject *__pyx_tuple__16;
 static PyObject *__pyx_tuple__19;
 static PyObject *__pyx_tuple__20;
 static PyObject *__pyx_tuple__21;
 static PyObject *__pyx_tuple__22;
 static PyObject *__pyx_tuple__25;
 static PyObject *__pyx_tuple__26;
 static PyObject *__pyx_tuple__27;
 static PyObject *__pyx_tuple__28;
 static PyObject *__pyx_tuple__29;
-static PyObject *__pyx_tuple__30;
+static PyObject *__pyx_tuple__31;
 static PyObject *__pyx_tuple__32;
-static PyObject *__pyx_codeobj__31;
-static PyObject *__pyx_codeobj__33;
+static PyObject *__pyx_tuple__33;
+static PyObject *__pyx_tuple__35;
+static PyObject *__pyx_codeobj__34;
+static PyObject *__pyx_codeobj__36;
 /* Late includes */
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("self.capi cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  */
@@ -6445,25 +6499,35 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_4frog_2installdata(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_targetdir, PyObject *__pyx_v_frogdataversion, PyObject *__pyx_v_uctodataversion) {
   PyObject *__pyx_v_uctodir = NULL;
   PyObject *__pyx_v_tmpdir = NULL;
   PyObject *__pyx_v_frogdir = NULL;
+  PyObject *__pyx_v_textcatpath = NULL;
+  PyObject *__pyx_v_data = NULL;
+  PyObject *__pyx_v_f = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   Py_ssize_t __pyx_t_8;
   Py_UCS4 __pyx_t_9;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
+  PyObject *__pyx_t_12 = NULL;
+  PyObject *__pyx_t_13 = NULL;
+  PyObject *__pyx_t_14 = NULL;
+  PyObject *__pyx_t_15 = NULL;
+  PyObject *__pyx_t_16 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("installdata", 0);
 
   /* "frog_wrapper.pyx":234
  * 
@@ -7265,15 +7329,15 @@
     }
 
     /* "frog_wrapper.pyx":256
  *         if os.system(f"cd {tmpdir} && mkdir -p {frogdir} && wget -O frogdata.tar.gz https://github.com/LanguageMachines/frogdata/releases/download/v{frogdataversion}/frogdata-{frogdataversion}.tar.gz && tar -xzf frogdata.tar.gz && cd frogdata-{frogdataversion} && mv config/[inserted by cython to avoid comment start]* {frogdir}/ && cd .. && rm -Rf frogdata-{frogdataversion} && rm -Rf frogdata.tar.gz") != 0:
  *             raise Exception("Installation of frogdata failed")
  *         print(f"Installation of frogdata {frogdataversion} complete", file=sys.stderr)             # <<<<<<<<<<<<<<
  * 
- *     if os.path.isdir("/usr/share/libexttextcat"):
+ *     textcatpath = os.environ.get("TEXTCATPATH","/usr/share/libexttextcat")
  */
     __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 256, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_8 = 0;
     __pyx_t_9 = 127;
     __Pyx_INCREF(__pyx_kp_u_Installation_of_frogdata);
     __pyx_t_8 += 25;
@@ -7314,155 +7378,480 @@
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_L7:;
 
   /* "frog_wrapper.pyx":258
  *         print(f"Installation of frogdata {frogdataversion} complete", file=sys.stderr)
  * 
- *     if os.path.isdir("/usr/share/libexttextcat"):             # <<<<<<<<<<<<<<
+ *     textcatpath = os.environ.get("TEXTCATPATH","/usr/share/libexttextcat")             # <<<<<<<<<<<<<<
+ *     if os.path.isdir(textcatpath):
  *         if os.system(f"cd {uctodir} && wget -O textcat.cfg https://raw.githubusercontent.com/LanguageMachines/ucto/master/config/textcat.cfg") != 0:
- *             raise Exception("Installation of textcat.cfg failed.")
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_os); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 258, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 258, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_environ); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_path); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 258, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 258, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_isdir); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 258, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_textcatpath = __pyx_t_4;
+  __pyx_t_4 = 0;
+
+  /* "frog_wrapper.pyx":259
+ * 
+ *     textcatpath = os.environ.get("TEXTCATPATH","/usr/share/libexttextcat")
+ *     if os.path.isdir(textcatpath):             # <<<<<<<<<<<<<<
+ *         if os.system(f"cd {uctodir} && wget -O textcat.cfg https://raw.githubusercontent.com/LanguageMachines/ucto/master/config/textcat.cfg") != 0:
+ *             raise Exception("Installation of textcat.cfg failed.")
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_path); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_isdir); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_4, function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u_usr_share_libexttextcat) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_usr_share_libexttextcat);
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_v_textcatpath) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_textcatpath);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 258, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 258, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_1) {
 
-    /* "frog_wrapper.pyx":259
- * 
- *     if os.path.isdir("/usr/share/libexttextcat"):
+    /* "frog_wrapper.pyx":260
+ *     textcatpath = os.environ.get("TEXTCATPATH","/usr/share/libexttextcat")
+ *     if os.path.isdir(textcatpath):
  *         if os.system(f"cd {uctodir} && wget -O textcat.cfg https://raw.githubusercontent.com/LanguageMachines/ucto/master/config/textcat.cfg") != 0:             # <<<<<<<<<<<<<<
  *             raise Exception("Installation of textcat.cfg failed.")
- *     else:
+ *         if textcatpath[-1] == '/': textcatpath = textcatpath[:-1]
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_os); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 259, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_system); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 260, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_system); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 260, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 259, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 260, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_8 = 0;
     __pyx_t_9 = 127;
     __Pyx_INCREF(__pyx_kp_u_cd);
     __pyx_t_8 += 3;
     __Pyx_GIVEREF(__pyx_kp_u_cd);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u_cd);
-    __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_v_uctodir, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 259, __pyx_L1_error)
+    PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_cd);
+    __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_v_uctodir, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 260, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_9 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_9) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_9;
     __pyx_t_8 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
-    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
+    PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_kp_u_wget_O_textcat_cfg_https_raw_gi);
     __pyx_t_8 += 105;
     __Pyx_GIVEREF(__pyx_kp_u_wget_O_textcat_cfg_https_raw_gi);
-    PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_kp_u_wget_O_textcat_cfg_https_raw_gi);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_8, __pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 259, __pyx_L1_error)
+    PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u_wget_O_textcat_cfg_https_raw_gi);
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_8, __pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 260, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = NULL;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
-      if (likely(__pyx_t_4)) {
+      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-        __Pyx_INCREF(__pyx_t_4);
+        __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_4, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_7);
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_7);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 259, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 260, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyInt_NeObjC(__pyx_t_3, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_NeObjC(__pyx_t_4, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 260, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 260, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (unlikely(__pyx_t_1)) {
 
-      /* "frog_wrapper.pyx":260
- *     if os.path.isdir("/usr/share/libexttextcat"):
+      /* "frog_wrapper.pyx":261
+ *     if os.path.isdir(textcatpath):
  *         if os.system(f"cd {uctodir} && wget -O textcat.cfg https://raw.githubusercontent.com/LanguageMachines/ucto/master/config/textcat.cfg") != 0:
  *             raise Exception("Installation of textcat.cfg failed.")             # <<<<<<<<<<<<<<
- *     else:
- *         print("Language detection will not be available unless you install libexttextcat and rerun installdata()", file=sys.stderr)
+ *         if textcatpath[-1] == '/': textcatpath = textcatpath[:-1]
+ *         if textcatpath != "/usr/share/libexttextcat":
  */
-      __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 260, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 261, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __PYX_ERR(0, 260, __pyx_L1_error)
+      __PYX_ERR(0, 261, __pyx_L1_error)
 
-      /* "frog_wrapper.pyx":259
- * 
- *     if os.path.isdir("/usr/share/libexttextcat"):
+      /* "frog_wrapper.pyx":260
+ *     textcatpath = os.environ.get("TEXTCATPATH","/usr/share/libexttextcat")
+ *     if os.path.isdir(textcatpath):
  *         if os.system(f"cd {uctodir} && wget -O textcat.cfg https://raw.githubusercontent.com/LanguageMachines/ucto/master/config/textcat.cfg") != 0:             # <<<<<<<<<<<<<<
  *             raise Exception("Installation of textcat.cfg failed.")
+ *         if textcatpath[-1] == '/': textcatpath = textcatpath[:-1]
+ */
+    }
+
+    /* "frog_wrapper.pyx":262
+ *         if os.system(f"cd {uctodir} && wget -O textcat.cfg https://raw.githubusercontent.com/LanguageMachines/ucto/master/config/textcat.cfg") != 0:
+ *             raise Exception("Installation of textcat.cfg failed.")
+ *         if textcatpath[-1] == '/': textcatpath = textcatpath[:-1]             # <<<<<<<<<<<<<<
+ *         if textcatpath != "/usr/share/libexttextcat":
+ *             data = open(f"{uctodir}/textcat.cfg",'r',encoding='utf-8').read()
+ */
+    __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_textcatpath, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 262, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_t_5, __pyx_kp_u__10, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 262, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (__pyx_t_1) {
+      __pyx_t_5 = __Pyx_PyObject_GetSlice(__pyx_v_textcatpath, 0, -1L, NULL, NULL, &__pyx_slice__30, 0, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 262, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF_SET(__pyx_v_textcatpath, __pyx_t_5);
+      __pyx_t_5 = 0;
+    }
+
+    /* "frog_wrapper.pyx":263
+ *             raise Exception("Installation of textcat.cfg failed.")
+ *         if textcatpath[-1] == '/': textcatpath = textcatpath[:-1]
+ *         if textcatpath != "/usr/share/libexttextcat":             # <<<<<<<<<<<<<<
+ *             data = open(f"{uctodir}/textcat.cfg",'r',encoding='utf-8').read()
+ *             with open(f"{uctodir}/textcat.cfg",'w',encoding='utf-8') as f:
+ */
+    __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_textcatpath, __pyx_kp_u_usr_share_libexttextcat, Py_NE)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 263, __pyx_L1_error)
+    if (__pyx_t_1) {
+
+      /* "frog_wrapper.pyx":264
+ *         if textcatpath[-1] == '/': textcatpath = textcatpath[:-1]
+ *         if textcatpath != "/usr/share/libexttextcat":
+ *             data = open(f"{uctodir}/textcat.cfg",'r',encoding='utf-8').read()             # <<<<<<<<<<<<<<
+ *             with open(f"{uctodir}/textcat.cfg",'w',encoding='utf-8') as f:
+ *                 f.write(data.replace("/usr/share/libexttextcat", textcatpath))
+ */
+      __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_v_uctodir, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 264, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_7 = __Pyx_PyUnicode_Concat(__pyx_t_4, __pyx_kp_u_textcat_cfg); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 264, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 264, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_GIVEREF(__pyx_t_7);
+      PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_7);
+      __Pyx_INCREF(__pyx_n_u_r);
+      __Pyx_GIVEREF(__pyx_n_u_r);
+      PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_n_u_r);
+      __pyx_t_7 = 0;
+      __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 264, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_encoding, __pyx_kp_u_utf_8) < 0) __PYX_ERR(0, 264, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_4, __pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 264, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_read); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 264, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_3 = NULL;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
+        __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_7);
+        if (likely(__pyx_t_3)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+          __Pyx_INCREF(__pyx_t_3);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_7, function);
+        }
+      }
+      __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
+      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 264, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __pyx_v_data = __pyx_t_5;
+      __pyx_t_5 = 0;
+
+      /* "frog_wrapper.pyx":265
+ *         if textcatpath != "/usr/share/libexttextcat":
+ *             data = open(f"{uctodir}/textcat.cfg",'r',encoding='utf-8').read()
+ *             with open(f"{uctodir}/textcat.cfg",'w',encoding='utf-8') as f:             # <<<<<<<<<<<<<<
+ *                 f.write(data.replace("/usr/share/libexttextcat", textcatpath))
+ *     else:
+ */
+      /*with:*/ {
+        __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_uctodir, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 265, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __pyx_t_7 = __Pyx_PyUnicode_Concat(__pyx_t_5, __pyx_kp_u_textcat_cfg); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 265, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_7);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 265, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __Pyx_GIVEREF(__pyx_t_7);
+        PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_7);
+        __Pyx_INCREF(__pyx_n_u_w);
+        __Pyx_GIVEREF(__pyx_n_u_w);
+        PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_n_u_w);
+        __pyx_t_7 = 0;
+        __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 265, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_7);
+        if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_encoding, __pyx_kp_u_utf_8) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_5, __pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 265, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+        __pyx_t_10 = __Pyx_PyObject_LookupSpecial(__pyx_t_3, __pyx_n_s_exit); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 265, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        __pyx_t_5 = __Pyx_PyObject_LookupSpecial(__pyx_t_3, __pyx_n_s_enter); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 265, __pyx_L13_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __pyx_t_4 = NULL;
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+          __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
+          if (likely(__pyx_t_4)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+            __Pyx_INCREF(__pyx_t_4);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_5, function);
+          }
+        }
+        __pyx_t_7 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
+        __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 265, __pyx_L13_error)
+        __Pyx_GOTREF(__pyx_t_7);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __pyx_t_5 = __pyx_t_7;
+        __pyx_t_7 = 0;
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        /*try:*/ {
+          {
+            __Pyx_PyThreadState_declare
+            __Pyx_PyThreadState_assign
+            __Pyx_ExceptionSave(&__pyx_t_11, &__pyx_t_12, &__pyx_t_13);
+            __Pyx_XGOTREF(__pyx_t_11);
+            __Pyx_XGOTREF(__pyx_t_12);
+            __Pyx_XGOTREF(__pyx_t_13);
+            /*try:*/ {
+              __pyx_v_f = __pyx_t_5;
+              __pyx_t_5 = 0;
+
+              /* "frog_wrapper.pyx":266
+ *             data = open(f"{uctodir}/textcat.cfg",'r',encoding='utf-8').read()
+ *             with open(f"{uctodir}/textcat.cfg",'w',encoding='utf-8') as f:
+ *                 f.write(data.replace("/usr/share/libexttextcat", textcatpath))             # <<<<<<<<<<<<<<
  *     else:
+ *         print("Language detection will not be available unless you install libexttextcat and rerun installdata(). Libexttextcat was not found. If it is in a non-standard location, set environment variable TEXTCATPATH (defaults to /usr/share/libexttextcat) prior to calling installdata()", file=sys.stderr)
+ */
+              __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_f, __pyx_n_s_write); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 266, __pyx_L17_error)
+              __Pyx_GOTREF(__pyx_t_3);
+              __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_replace); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 266, __pyx_L17_error)
+              __Pyx_GOTREF(__pyx_t_4);
+              __pyx_t_14 = NULL;
+              __pyx_t_6 = 0;
+              if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+                __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_4);
+                if (likely(__pyx_t_14)) {
+                  PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+                  __Pyx_INCREF(__pyx_t_14);
+                  __Pyx_INCREF(function);
+                  __Pyx_DECREF_SET(__pyx_t_4, function);
+                  __pyx_t_6 = 1;
+                }
+              }
+              #if CYTHON_FAST_PYCALL
+              if (PyFunction_Check(__pyx_t_4)) {
+                PyObject *__pyx_temp[3] = {__pyx_t_14, __pyx_kp_u_usr_share_libexttextcat, __pyx_v_textcatpath};
+                __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 266, __pyx_L17_error)
+                __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
+                __Pyx_GOTREF(__pyx_t_7);
+              } else
+              #endif
+              #if CYTHON_FAST_PYCCALL
+              if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
+                PyObject *__pyx_temp[3] = {__pyx_t_14, __pyx_kp_u_usr_share_libexttextcat, __pyx_v_textcatpath};
+                __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 266, __pyx_L17_error)
+                __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
+                __Pyx_GOTREF(__pyx_t_7);
+              } else
+              #endif
+              {
+                __pyx_t_15 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 266, __pyx_L17_error)
+                __Pyx_GOTREF(__pyx_t_15);
+                if (__pyx_t_14) {
+                  __Pyx_GIVEREF(__pyx_t_14); PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_t_14); __pyx_t_14 = NULL;
+                }
+                __Pyx_INCREF(__pyx_kp_u_usr_share_libexttextcat);
+                __Pyx_GIVEREF(__pyx_kp_u_usr_share_libexttextcat);
+                PyTuple_SET_ITEM(__pyx_t_15, 0+__pyx_t_6, __pyx_kp_u_usr_share_libexttextcat);
+                __Pyx_INCREF(__pyx_v_textcatpath);
+                __Pyx_GIVEREF(__pyx_v_textcatpath);
+                PyTuple_SET_ITEM(__pyx_t_15, 1+__pyx_t_6, __pyx_v_textcatpath);
+                __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_15, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 266, __pyx_L17_error)
+                __Pyx_GOTREF(__pyx_t_7);
+                __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
+              }
+              __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+              __pyx_t_4 = NULL;
+              if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+                __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+                if (likely(__pyx_t_4)) {
+                  PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+                  __Pyx_INCREF(__pyx_t_4);
+                  __Pyx_INCREF(function);
+                  __Pyx_DECREF_SET(__pyx_t_3, function);
+                }
+              }
+              __pyx_t_5 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_7);
+              __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+              __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+              if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 266, __pyx_L17_error)
+              __Pyx_GOTREF(__pyx_t_5);
+              __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+              __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+              /* "frog_wrapper.pyx":265
+ *         if textcatpath != "/usr/share/libexttextcat":
+ *             data = open(f"{uctodir}/textcat.cfg",'r',encoding='utf-8').read()
+ *             with open(f"{uctodir}/textcat.cfg",'w',encoding='utf-8') as f:             # <<<<<<<<<<<<<<
+ *                 f.write(data.replace("/usr/share/libexttextcat", textcatpath))
+ *     else:
+ */
+            }
+            __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+            __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+            __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+            goto __pyx_L22_try_end;
+            __pyx_L17_error:;
+            __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
+            __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
+            __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+            __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+            __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+            __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+            /*except:*/ {
+              __Pyx_AddTraceback("frog.installdata", __pyx_clineno, __pyx_lineno, __pyx_filename);
+              if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_3, &__pyx_t_7) < 0) __PYX_ERR(0, 265, __pyx_L19_except_error)
+              __Pyx_GOTREF(__pyx_t_5);
+              __Pyx_GOTREF(__pyx_t_3);
+              __Pyx_GOTREF(__pyx_t_7);
+              __pyx_t_4 = PyTuple_Pack(3, __pyx_t_5, __pyx_t_3, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 265, __pyx_L19_except_error)
+              __Pyx_GOTREF(__pyx_t_4);
+              __pyx_t_16 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_4, NULL);
+              __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+              __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+              if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 265, __pyx_L19_except_error)
+              __Pyx_GOTREF(__pyx_t_16);
+              __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_16);
+              __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
+              if (__pyx_t_1 < 0) __PYX_ERR(0, 265, __pyx_L19_except_error)
+              __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
+              if (__pyx_t_2) {
+                __Pyx_GIVEREF(__pyx_t_5);
+                __Pyx_GIVEREF(__pyx_t_3);
+                __Pyx_XGIVEREF(__pyx_t_7);
+                __Pyx_ErrRestoreWithState(__pyx_t_5, __pyx_t_3, __pyx_t_7);
+                __pyx_t_5 = 0; __pyx_t_3 = 0; __pyx_t_7 = 0; 
+                __PYX_ERR(0, 265, __pyx_L19_except_error)
+              }
+              __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+              __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+              __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+              goto __pyx_L18_exception_handled;
+            }
+            __pyx_L19_except_error:;
+            __Pyx_XGIVEREF(__pyx_t_11);
+            __Pyx_XGIVEREF(__pyx_t_12);
+            __Pyx_XGIVEREF(__pyx_t_13);
+            __Pyx_ExceptionReset(__pyx_t_11, __pyx_t_12, __pyx_t_13);
+            goto __pyx_L1_error;
+            __pyx_L18_exception_handled:;
+            __Pyx_XGIVEREF(__pyx_t_11);
+            __Pyx_XGIVEREF(__pyx_t_12);
+            __Pyx_XGIVEREF(__pyx_t_13);
+            __Pyx_ExceptionReset(__pyx_t_11, __pyx_t_12, __pyx_t_13);
+            __pyx_L22_try_end:;
+          }
+        }
+        /*finally:*/ {
+          /*normal exit:*/{
+            if (__pyx_t_10) {
+              __pyx_t_13 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_tuple__31, NULL);
+              __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+              if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 265, __pyx_L1_error)
+              __Pyx_GOTREF(__pyx_t_13);
+              __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+            }
+            goto __pyx_L16;
+          }
+          __pyx_L16:;
+        }
+        goto __pyx_L26;
+        __pyx_L13_error:;
+        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+        goto __pyx_L1_error;
+        __pyx_L26:;
+      }
+
+      /* "frog_wrapper.pyx":263
+ *             raise Exception("Installation of textcat.cfg failed.")
+ *         if textcatpath[-1] == '/': textcatpath = textcatpath[:-1]
+ *         if textcatpath != "/usr/share/libexttextcat":             # <<<<<<<<<<<<<<
+ *             data = open(f"{uctodir}/textcat.cfg",'r',encoding='utf-8').read()
+ *             with open(f"{uctodir}/textcat.cfg",'w',encoding='utf-8') as f:
  */
     }
 
-    /* "frog_wrapper.pyx":258
- *         print(f"Installation of frogdata {frogdataversion} complete", file=sys.stderr)
+    /* "frog_wrapper.pyx":259
  * 
- *     if os.path.isdir("/usr/share/libexttextcat"):             # <<<<<<<<<<<<<<
+ *     textcatpath = os.environ.get("TEXTCATPATH","/usr/share/libexttextcat")
+ *     if os.path.isdir(textcatpath):             # <<<<<<<<<<<<<<
  *         if os.system(f"cd {uctodir} && wget -O textcat.cfg https://raw.githubusercontent.com/LanguageMachines/ucto/master/config/textcat.cfg") != 0:
  *             raise Exception("Installation of textcat.cfg failed.")
  */
     goto __pyx_L9;
   }
 
-  /* "frog_wrapper.pyx":262
- *             raise Exception("Installation of textcat.cfg failed.")
+  /* "frog_wrapper.pyx":268
+ *                 f.write(data.replace("/usr/share/libexttextcat", textcatpath))
  *     else:
- *         print("Language detection will not be available unless you install libexttextcat and rerun installdata()", file=sys.stderr)             # <<<<<<<<<<<<<<
+ *         print("Language detection will not be available unless you install libexttextcat and rerun installdata(). Libexttextcat was not found. If it is in a non-standard location, set environment variable TEXTCATPATH (defaults to /usr/share/libexttextcat) prior to calling installdata()", file=sys.stderr)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
-    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 262, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_sys); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 262, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_stderr); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 262, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 268, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_sys); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 268, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_stderr); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 268, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_file, __pyx_t_7) < 0) __PYX_ERR(0, 262, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__29, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 262, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_file, __pyx_t_5) < 0) __PYX_ERR(0, 268, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__32, __pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 268, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __pyx_L9:;
 
   /* "frog_wrapper.pyx":233
  *     return os.environ.get("FROGDATAPATH", os.path.join(xdg_config_dir,name) )
  * 
  * def installdata(targetdir=None, frogdataversion=FROGDATAVERSION, uctodataversion=UCTODATAVERSION):             # <<<<<<<<<<<<<<
@@ -7474,20 +7863,25 @@
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_14);
+  __Pyx_XDECREF(__pyx_t_15);
   __Pyx_AddTraceback("frog.installdata", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_uctodir);
   __Pyx_XDECREF(__pyx_v_tmpdir);
   __Pyx_XDECREF(__pyx_v_frogdir);
+  __Pyx_XDECREF(__pyx_v_textcatpath);
+  __Pyx_XDECREF(__pyx_v_data);
+  __Pyx_XDECREF(__pyx_v_f);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "string.from_py":13
  * 
@@ -8277,14 +8671,15 @@
   {&__pyx_kp_u_Installation_of_uctodata_failed, __pyx_k_Installation_of_uctodata_failed, sizeof(__pyx_k_Installation_of_uctodata_failed), 0, 1, 0, 0},
   {&__pyx_n_s_KeyError, __pyx_k_KeyError, sizeof(__pyx_k_KeyError), 0, 0, 1, 1},
   {&__pyx_kp_u_Language_detection_will_not_be_a, __pyx_k_Language_detection_will_not_be_a, sizeof(__pyx_k_Language_detection_will_not_be_a), 0, 1, 0, 0},
   {&__pyx_kp_u_No_data_returned, __pyx_k_No_data_returned, sizeof(__pyx_k_No_data_returned), 0, 1, 0, 0},
   {&__pyx_kp_u_No_such_key, __pyx_k_No_such_key, sizeof(__pyx_k_No_such_key), 0, 1, 0, 0},
   {&__pyx_kp_u_Returned_data_is_not_XML_got, __pyx_k_Returned_data_is_not_XML_got, sizeof(__pyx_k_Returned_data_is_not_XML_got), 0, 1, 0, 0},
   {&__pyx_kp_u_Specified_configuration_file, __pyx_k_Specified_configuration_file, sizeof(__pyx_k_Specified_configuration_file), 0, 1, 0, 0},
+  {&__pyx_n_u_TEXTCATPATH, __pyx_k_TEXTCATPATH, sizeof(__pyx_k_TEXTCATPATH), 0, 1, 0, 1},
   {&__pyx_n_u_TMPDIR, __pyx_k_TMPDIR, sizeof(__pyx_k_TMPDIR), 0, 1, 0, 1},
   {&__pyx_kp_u_Text_should_be_a_string_or_FoLiA, __pyx_k_Text_should_be_a_string_or_FoLiA, sizeof(__pyx_k_Text_should_be_a_string_or_FoLiA), 0, 1, 0, 0},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_n_s_UCTODATAVERSION, __pyx_k_UCTODATAVERSION, sizeof(__pyx_k_UCTODATAVERSION), 0, 0, 1, 1},
   {&__pyx_kp_u_Uctodata_configuration_directory, __pyx_k_Uctodata_configuration_directory, sizeof(__pyx_k_Uctodata_configuration_directory), 0, 1, 0, 0},
   {&__pyx_kp_u_Unable_to_return_a_FoLiA_Documen, __pyx_k_Unable_to_return_a_FoLiA_Documen, sizeof(__pyx_k_Unable_to_return_a_FoLiA_Documen), 0, 1, 0, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
@@ -8309,14 +8704,15 @@
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_kp_u_complete, __pyx_k_complete, sizeof(__pyx_k_complete), 0, 1, 0, 0},
   {&__pyx_n_u_compound, __pyx_k_compound, sizeof(__pyx_k_compound), 0, 1, 0, 1},
   {&__pyx_n_b_config, __pyx_k_config, sizeof(__pyx_k_config), 0, 0, 0, 1},
   {&__pyx_kp_u_config_2, __pyx_k_config_2, sizeof(__pyx_k_config_2), 0, 1, 0, 0},
   {&__pyx_n_s_configurationfile, __pyx_k_configurationfile, sizeof(__pyx_k_configurationfile), 0, 0, 1, 1},
   {&__pyx_n_u_daringmorph, __pyx_k_daringmorph, sizeof(__pyx_k_daringmorph), 0, 1, 0, 1},
+  {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
   {&__pyx_n_u_debug, __pyx_k_debug, sizeof(__pyx_k_debug), 0, 1, 0, 1},
   {&__pyx_n_u_debugflag, __pyx_k_debugflag, sizeof(__pyx_k_debugflag), 0, 1, 0, 1},
   {&__pyx_n_b_deepmorph, __pyx_k_deepmorph, sizeof(__pyx_k_deepmorph), 0, 0, 0, 1},
   {&__pyx_n_u_deepmorph, __pyx_k_deepmorph, sizeof(__pyx_k_deepmorph), 0, 1, 0, 1},
   {&__pyx_n_s_default, __pyx_k_default, sizeof(__pyx_k_default), 0, 0, 1, 1},
   {&__pyx_n_u_dep, __pyx_k_dep, sizeof(__pyx_k_dep), 0, 1, 0, 1},
   {&__pyx_n_u_depindex, __pyx_k_depindex, sizeof(__pyx_k_depindex), 0, 1, 0, 1},
@@ -8336,18 +8732,22 @@
   {&__pyx_n_u_doparse, __pyx_k_doparse, sizeof(__pyx_k_doparse), 0, 1, 0, 1},
   {&__pyx_n_u_doparser, __pyx_k_doparser, sizeof(__pyx_k_doparser), 0, 1, 0, 1},
   {&__pyx_n_u_dotok, __pyx_k_dotok, sizeof(__pyx_k_dotok), 0, 1, 0, 1},
   {&__pyx_n_u_doxmlin, __pyx_k_doxmlin, sizeof(__pyx_k_doxmlin), 0, 1, 0, 1},
   {&__pyx_n_u_doxmlout, __pyx_k_doxmlout, sizeof(__pyx_k_doxmlout), 0, 1, 0, 1},
   {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
   {&__pyx_n_s_encode_text, __pyx_k_encode_text, sizeof(__pyx_k_encode_text), 0, 0, 1, 1},
+  {&__pyx_n_s_encoding, __pyx_k_encoding, sizeof(__pyx_k_encoding), 0, 0, 1, 1},
+  {&__pyx_n_s_enter, __pyx_k_enter, sizeof(__pyx_k_enter), 0, 0, 1, 1},
   {&__pyx_n_s_enumerate, __pyx_k_enumerate, sizeof(__pyx_k_enumerate), 0, 0, 1, 1},
   {&__pyx_n_s_environ, __pyx_k_environ, sizeof(__pyx_k_environ), 0, 0, 1, 1},
   {&__pyx_n_u_eos, __pyx_k_eos, sizeof(__pyx_k_eos), 0, 1, 0, 1},
   {&__pyx_n_s_exists, __pyx_k_exists, sizeof(__pyx_k_exists), 0, 0, 1, 1},
+  {&__pyx_n_s_exit, __pyx_k_exit, sizeof(__pyx_k_exit), 0, 0, 1, 1},
+  {&__pyx_n_s_f, __pyx_k_f, sizeof(__pyx_k_f), 0, 0, 1, 1},
   {&__pyx_n_s_file, __pyx_k_file, sizeof(__pyx_k_file), 0, 0, 1, 1},
   {&__pyx_n_s_finish, __pyx_k_finish, sizeof(__pyx_k_finish), 0, 0, 1, 1},
   {&__pyx_n_s_folia_main, __pyx_k_folia_main, sizeof(__pyx_k_folia_main), 0, 0, 1, 1},
   {&__pyx_n_u_foliain, __pyx_k_foliain, sizeof(__pyx_k_foliain), 0, 1, 0, 1},
   {&__pyx_n_u_foliaout, __pyx_k_foliaout, sizeof(__pyx_k_foliaout), 0, 1, 0, 1},
   {&__pyx_n_s_frog, __pyx_k_frog, sizeof(__pyx_k_frog), 0, 0, 1, 1},
   {&__pyx_n_u_frog, __pyx_k_frog, sizeof(__pyx_k_frog), 0, 1, 0, 1},
@@ -8382,14 +8782,15 @@
   {&__pyx_n_u_mwu, __pyx_k_mwu, sizeof(__pyx_k_mwu), 0, 1, 0, 1},
   {&__pyx_n_u_n, __pyx_k_n, sizeof(__pyx_k_n), 0, 1, 0, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
   {&__pyx_n_u_ner, __pyx_k_ner, sizeof(__pyx_k_ner), 0, 1, 0, 1},
   {&__pyx_n_b_nld, __pyx_k_nld, sizeof(__pyx_k_nld), 0, 0, 0, 1},
   {&__pyx_n_u_numthreads, __pyx_k_numthreads, sizeof(__pyx_k_numthreads), 0, 1, 0, 1},
+  {&__pyx_n_s_open, __pyx_k_open, sizeof(__pyx_k_open), 0, 0, 1, 1},
   {&__pyx_n_s_options, __pyx_k_options, sizeof(__pyx_k_options), 0, 0, 1, 1},
   {&__pyx_n_s_os, __pyx_k_os, sizeof(__pyx_k_os), 0, 0, 1, 1},
   {&__pyx_n_b_override, __pyx_k_override, sizeof(__pyx_k_override), 0, 0, 0, 1},
   {&__pyx_n_s_overrides, __pyx_k_overrides, sizeof(__pyx_k_overrides), 0, 0, 1, 1},
   {&__pyx_n_u_p, __pyx_k_p, sizeof(__pyx_k_p), 0, 1, 0, 1},
   {&__pyx_n_u_parse, __pyx_k_parse, sizeof(__pyx_k_parse), 0, 1, 0, 1},
   {&__pyx_n_s_parsecolumns, __pyx_k_parsecolumns, sizeof(__pyx_k_parsecolumns), 0, 0, 1, 1},
@@ -8398,14 +8799,16 @@
   {&__pyx_n_u_pos, __pyx_k_pos, sizeof(__pyx_k_pos), 0, 1, 0, 1},
   {&__pyx_n_u_posprob, __pyx_k_posprob, sizeof(__pyx_k_posprob), 0, 1, 0, 1},
   {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
   {&__pyx_n_s_print, __pyx_k_print, sizeof(__pyx_k_print), 0, 0, 1, 1},
   {&__pyx_n_s_process_raw, __pyx_k_process_raw, sizeof(__pyx_k_process_raw), 0, 0, 1, 1},
   {&__pyx_n_s_pynlpl_formats_folia, __pyx_k_pynlpl_formats_folia, sizeof(__pyx_k_pynlpl_formats_folia), 0, 0, 1, 1},
   {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
+  {&__pyx_n_u_r, __pyx_k_r, sizeof(__pyx_k_r), 0, 1, 0, 1},
+  {&__pyx_n_s_read, __pyx_k_read, sizeof(__pyx_k_read), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_kp_u_refusing_to_overwrite_please_re, __pyx_k_refusing_to_overwrite_please_re, sizeof(__pyx_k_refusing_to_overwrite_please_re), 0, 1, 0, 0},
   {&__pyx_n_s_remove, __pyx_k_remove, sizeof(__pyx_k_remove), 0, 0, 1, 1},
   {&__pyx_n_s_replace, __pyx_k_replace, sizeof(__pyx_k_replace), 0, 0, 1, 1},
   {&__pyx_kp_u_rm_Rf_frogdata_tar_gz, __pyx_k_rm_Rf_frogdata_tar_gz, sizeof(__pyx_k_rm_Rf_frogdata_tar_gz), 0, 1, 0, 0},
@@ -8425,42 +8828,47 @@
   {&__pyx_n_s_system, __pyx_k_system, sizeof(__pyx_k_system), 0, 0, 1, 1},
   {&__pyx_n_u_t, __pyx_k_t, sizeof(__pyx_k_t), 0, 1, 0, 1},
   {&__pyx_kp_u_tar_gz_tar_xzf_frogdata_tar_gz, __pyx_k_tar_gz_tar_xzf_frogdata_tar_gz, sizeof(__pyx_k_tar_gz_tar_xzf_frogdata_tar_gz), 0, 1, 0, 0},
   {&__pyx_kp_u_tar_gz_tar_xzf_uctodata_tar_gz, __pyx_k_tar_gz_tar_xzf_uctodata_tar_gz, sizeof(__pyx_k_tar_gz_tar_xzf_uctodata_tar_gz), 0, 1, 0, 0},
   {&__pyx_n_s_targetdir, __pyx_k_targetdir, sizeof(__pyx_k_targetdir), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_u_text, __pyx_k_text, sizeof(__pyx_k_text), 0, 1, 0, 1},
+  {&__pyx_kp_u_textcat_cfg, __pyx_k_textcat_cfg, sizeof(__pyx_k_textcat_cfg), 0, 1, 0, 0},
+  {&__pyx_n_s_textcatpath, __pyx_k_textcatpath, sizeof(__pyx_k_textcatpath), 0, 0, 1, 1},
   {&__pyx_n_b_threads, __pyx_k_threads, sizeof(__pyx_k_threads), 0, 0, 0, 1},
   {&__pyx_n_u_threads, __pyx_k_threads, sizeof(__pyx_k_threads), 0, 1, 0, 1},
   {&__pyx_kp_u_tmp, __pyx_k_tmp, sizeof(__pyx_k_tmp), 0, 1, 0, 0},
   {&__pyx_n_s_tmpdir, __pyx_k_tmpdir, sizeof(__pyx_k_tmpdir), 0, 0, 1, 1},
   {&__pyx_n_u_tok, __pyx_k_tok, sizeof(__pyx_k_tok), 0, 1, 0, 1},
   {&__pyx_n_u_ucto, __pyx_k_ucto, sizeof(__pyx_k_ucto), 0, 1, 0, 1},
   {&__pyx_kp_u_uctodata, __pyx_k_uctodata, sizeof(__pyx_k_uctodata), 0, 1, 0, 0},
   {&__pyx_n_s_uctodataversion, __pyx_k_uctodataversion, sizeof(__pyx_k_uctodataversion), 0, 0, 1, 1},
   {&__pyx_n_s_uctodir, __pyx_k_uctodir, sizeof(__pyx_k_uctodir), 0, 0, 1, 1},
   {&__pyx_kp_u_usr_share_libexttextcat, __pyx_k_usr_share_libexttextcat, sizeof(__pyx_k_usr_share_libexttextcat), 0, 1, 0, 0},
   {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
   {&__pyx_n_s_version, __pyx_k_version, sizeof(__pyx_k_version), 0, 0, 1, 1},
+  {&__pyx_n_u_w, __pyx_k_w, sizeof(__pyx_k_w), 0, 1, 0, 1},
   {&__pyx_kp_u_wget_O_frogdata_tar_gz_https_gi, __pyx_k_wget_O_frogdata_tar_gz_https_gi, sizeof(__pyx_k_wget_O_frogdata_tar_gz_https_gi), 0, 1, 0, 0},
   {&__pyx_kp_u_wget_O_textcat_cfg_https_raw_gi, __pyx_k_wget_O_textcat_cfg_https_raw_gi, sizeof(__pyx_k_wget_O_textcat_cfg_https_raw_gi), 0, 1, 0, 0},
   {&__pyx_kp_u_wget_O_uctodata_tar_gz_https_gi, __pyx_k_wget_O_uctodata_tar_gz_https_gi, sizeof(__pyx_k_wget_O_uctodata_tar_gz_https_gi), 0, 1, 0, 0},
+  {&__pyx_n_s_write, __pyx_k_write, sizeof(__pyx_k_write), 0, 0, 1, 1},
   {&__pyx_n_u_x, __pyx_k_x, sizeof(__pyx_k_x), 0, 1, 0, 1},
   {&__pyx_n_s_xdg_config_dir, __pyx_k_xdg_config_dir, sizeof(__pyx_k_xdg_config_dir), 0, 0, 1, 1},
   {&__pyx_n_u_xmlin, __pyx_k_xmlin, sizeof(__pyx_k_xmlin), 0, 1, 0, 1},
   {&__pyx_n_u_xmlout, __pyx_k_xmlout, sizeof(__pyx_k_xmlout), 0, 1, 0, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(0, 33, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 87, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 194, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 209, __pyx_L1_error)
   __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 264, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -8640,71 +9048,105 @@
  *         print(f"Installation of frogdata {frogdataversion} complete", file=sys.stderr)
  * 
  */
   __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_u_Installation_of_frogdata_failed); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__27);
   __Pyx_GIVEREF(__pyx_tuple__27);
 
-  /* "frog_wrapper.pyx":260
- *     if os.path.isdir("/usr/share/libexttextcat"):
+  /* "frog_wrapper.pyx":258
+ *         print(f"Installation of frogdata {frogdataversion} complete", file=sys.stderr)
+ * 
+ *     textcatpath = os.environ.get("TEXTCATPATH","/usr/share/libexttextcat")             # <<<<<<<<<<<<<<
+ *     if os.path.isdir(textcatpath):
  *         if os.system(f"cd {uctodir} && wget -O textcat.cfg https://raw.githubusercontent.com/LanguageMachines/ucto/master/config/textcat.cfg") != 0:
- *             raise Exception("Installation of textcat.cfg failed.")             # <<<<<<<<<<<<<<
- *     else:
- *         print("Language detection will not be available unless you install libexttextcat and rerun installdata()", file=sys.stderr)
  */
-  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_u_Installation_of_textcat_cfg_fail); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(2, __pyx_n_u_TEXTCATPATH, __pyx_kp_u_usr_share_libexttextcat); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
 
+  /* "frog_wrapper.pyx":261
+ *     if os.path.isdir(textcatpath):
+ *         if os.system(f"cd {uctodir} && wget -O textcat.cfg https://raw.githubusercontent.com/LanguageMachines/ucto/master/config/textcat.cfg") != 0:
+ *             raise Exception("Installation of textcat.cfg failed.")             # <<<<<<<<<<<<<<
+ *         if textcatpath[-1] == '/': textcatpath = textcatpath[:-1]
+ *         if textcatpath != "/usr/share/libexttextcat":
+ */
+  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_u_Installation_of_textcat_cfg_fail); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 261, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__29);
+  __Pyx_GIVEREF(__pyx_tuple__29);
+
   /* "frog_wrapper.pyx":262
+ *         if os.system(f"cd {uctodir} && wget -O textcat.cfg https://raw.githubusercontent.com/LanguageMachines/ucto/master/config/textcat.cfg") != 0:
  *             raise Exception("Installation of textcat.cfg failed.")
+ *         if textcatpath[-1] == '/': textcatpath = textcatpath[:-1]             # <<<<<<<<<<<<<<
+ *         if textcatpath != "/usr/share/libexttextcat":
+ *             data = open(f"{uctodir}/textcat.cfg",'r',encoding='utf-8').read()
+ */
+  __pyx_slice__30 = PySlice_New(Py_None, __pyx_int_neg_1, Py_None); if (unlikely(!__pyx_slice__30)) __PYX_ERR(0, 262, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__30);
+  __Pyx_GIVEREF(__pyx_slice__30);
+
+  /* "frog_wrapper.pyx":265
+ *         if textcatpath != "/usr/share/libexttextcat":
+ *             data = open(f"{uctodir}/textcat.cfg",'r',encoding='utf-8').read()
+ *             with open(f"{uctodir}/textcat.cfg",'w',encoding='utf-8') as f:             # <<<<<<<<<<<<<<
+ *                 f.write(data.replace("/usr/share/libexttextcat", textcatpath))
+ *     else:
+ */
+  __pyx_tuple__31 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__31);
+  __Pyx_GIVEREF(__pyx_tuple__31);
+
+  /* "frog_wrapper.pyx":268
+ *                 f.write(data.replace("/usr/share/libexttextcat", textcatpath))
  *     else:
- *         print("Language detection will not be available unless you install libexttextcat and rerun installdata()", file=sys.stderr)             # <<<<<<<<<<<<<<
+ *         print("Language detection will not be available unless you install libexttextcat and rerun installdata(). Libexttextcat was not found. If it is in a non-standard location, set environment variable TEXTCATPATH (defaults to /usr/share/libexttextcat) prior to calling installdata()", file=sys.stderr)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_u_Language_detection_will_not_be_a); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 262, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__29);
-  __Pyx_GIVEREF(__pyx_tuple__29);
+  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_kp_u_Language_detection_will_not_be_a); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 268, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__32);
+  __Pyx_GIVEREF(__pyx_tuple__32);
 
   /* "frog_wrapper.pyx":229
  *         return text #already was bytes or python2 str
  * 
  * def localpath(name="frog"):             # <<<<<<<<<<<<<<
  *     xdg_config_dir = os.environ.get("XDG_CONFIG_HOME", os.path.join(os.environ.get("HOME",""), ".config"))
  *     return os.environ.get("FROGDATAPATH", os.path.join(xdg_config_dir,name) )
  */
-  __pyx_tuple__30 = PyTuple_Pack(2, __pyx_n_s_name, __pyx_n_s_xdg_config_dir); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 229, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
-  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_frog_wrapper_pyx, __pyx_n_s_localpath, 229, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(2, __pyx_n_s_name, __pyx_n_s_xdg_config_dir); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__33);
+  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_frog_wrapper_pyx, __pyx_n_s_localpath, 229, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 229, __pyx_L1_error)
 
   /* "frog_wrapper.pyx":233
  *     return os.environ.get("FROGDATAPATH", os.path.join(xdg_config_dir,name) )
  * 
  * def installdata(targetdir=None, frogdataversion=FROGDATAVERSION, uctodataversion=UCTODATAVERSION):             # <<<<<<<<<<<<<<
  *     if targetdir is None:
  *         uctodir = localpath("ucto")
  */
-  __pyx_tuple__32 = PyTuple_Pack(6, __pyx_n_s_targetdir, __pyx_n_s_frogdataversion, __pyx_n_s_uctodataversion, __pyx_n_s_uctodir, __pyx_n_s_tmpdir, __pyx_n_s_frogdir); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 233, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__32);
-  __Pyx_GIVEREF(__pyx_tuple__32);
-  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(3, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_frog_wrapper_pyx, __pyx_n_s_installdata, 233, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_tuple__35 = PyTuple_Pack(9, __pyx_n_s_targetdir, __pyx_n_s_frogdataversion, __pyx_n_s_uctodataversion, __pyx_n_s_uctodir, __pyx_n_s_tmpdir, __pyx_n_s_frogdir, __pyx_n_s_textcatpath, __pyx_n_s_data, __pyx_n_s_f); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__35);
+  __Pyx_GIVEREF(__pyx_tuple__35);
+  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(3, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_frog_wrapper_pyx, __pyx_n_s_installdata, 233, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 233, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_25 = PyInt_FromLong(25); if (unlikely(!__pyx_int_25)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -9608,28 +10050,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -11164,14 +11606,144 @@
         double a = PyFloat_AS_DOUBLE(op1);
         if ((double)a != (double)b) Py_RETURN_TRUE; else Py_RETURN_FALSE;
     }
     return (
         PyObject_RichCompare(op1, op2, Py_NE));
 }
 
+/* GetTopmostException */
+#if CYTHON_USE_EXC_INFO_STACK
+static _PyErr_StackItem *
+__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
+{
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
+           exc_info->previous_item != NULL)
+    {
+        exc_info = exc_info->previous_item;
+    }
+    return exc_info;
+}
+#endif
+
+/* SaveResetException */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    *type = exc_info->exc_type;
+    *value = exc_info->exc_value;
+    *tb = exc_info->exc_traceback;
+    #else
+    *type = tstate->exc_type;
+    *value = tstate->exc_value;
+    *tb = tstate->exc_traceback;
+    #endif
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+}
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_type = exc_info->exc_type;
+    tmp_value = exc_info->exc_value;
+    tmp_tb = exc_info->exc_traceback;
+    exc_info->exc_type = type;
+    exc_info->exc_value = value;
+    exc_info->exc_traceback = tb;
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = type;
+    tstate->exc_value = value;
+    tstate->exc_traceback = tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+}
+#endif
+
+/* GetException */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+#endif
+{
+    PyObject *local_type, *local_value, *local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    local_type = tstate->curexc_type;
+    local_value = tstate->curexc_value;
+    local_tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+#else
+    PyErr_Fetch(&local_type, &local_value, &local_tb);
+#endif
+    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
+#if CYTHON_FAST_THREAD_STATE
+    if (unlikely(tstate->curexc_type))
+#else
+    if (unlikely(PyErr_Occurred()))
+#endif
+        goto bad;
+    #if PY_MAJOR_VERSION >= 3
+    if (local_tb) {
+        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
+            goto bad;
+    }
+    #endif
+    Py_XINCREF(local_tb);
+    Py_XINCREF(local_type);
+    Py_XINCREF(local_value);
+    *type = local_type;
+    *value = local_value;
+    *tb = local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    #if CYTHON_USE_EXC_INFO_STACK
+    {
+        _PyErr_StackItem *exc_info = tstate->exc_info;
+        tmp_type = exc_info->exc_type;
+        tmp_value = exc_info->exc_value;
+        tmp_tb = exc_info->exc_traceback;
+        exc_info->exc_type = local_type;
+        exc_info->exc_value = local_value;
+        exc_info->exc_traceback = local_tb;
+    }
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = local_type;
+    tstate->exc_value = local_value;
+    tstate->exc_traceback = local_tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#else
+    PyErr_SetExcInfo(local_type, local_value, local_tb);
+#endif
+    return 0;
+bad:
+    *type = 0;
+    *value = 0;
+    *tb = 0;
+    Py_XDECREF(local_type);
+    Py_XDECREF(local_value);
+    Py_XDECREF(local_tb);
+    return -1;
+}
+
 /* PyObject_GenericGetAttrNoDict */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
     PyErr_Format(PyExc_AttributeError,
 #if PY_MAJOR_VERSION >= 3
                  "'%.50s' object has no attribute '%U'",
                  tp->tp_name, attr_name);
@@ -11444,144 +12016,14 @@
         #else
             "cannot import name %S", name);
         #endif
     }
     return value;
 }
 
-/* GetTopmostException */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem *
-__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
-{
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
-           exc_info->previous_item != NULL)
-    {
-        exc_info = exc_info->previous_item;
-    }
-    return exc_info;
-}
-#endif
-
-/* SaveResetException */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
-    *type = exc_info->exc_type;
-    *value = exc_info->exc_value;
-    *tb = exc_info->exc_traceback;
-    #else
-    *type = tstate->exc_type;
-    *value = tstate->exc_value;
-    *tb = tstate->exc_traceback;
-    #endif
-    Py_XINCREF(*type);
-    Py_XINCREF(*value);
-    Py_XINCREF(*tb);
-}
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    tmp_type = exc_info->exc_type;
-    tmp_value = exc_info->exc_value;
-    tmp_tb = exc_info->exc_traceback;
-    exc_info->exc_type = type;
-    exc_info->exc_value = value;
-    exc_info->exc_traceback = tb;
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = type;
-    tstate->exc_value = value;
-    tstate->exc_traceback = tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-#endif
-
-/* GetException */
-#if CYTHON_FAST_THREAD_STATE
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
-#endif
-{
-    PyObject *local_type, *local_value, *local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    local_type = tstate->curexc_type;
-    local_value = tstate->curexc_value;
-    local_tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-#else
-    PyErr_Fetch(&local_type, &local_value, &local_tb);
-#endif
-    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
-#if CYTHON_FAST_THREAD_STATE
-    if (unlikely(tstate->curexc_type))
-#else
-    if (unlikely(PyErr_Occurred()))
-#endif
-        goto bad;
-    #if PY_MAJOR_VERSION >= 3
-    if (local_tb) {
-        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
-            goto bad;
-    }
-    #endif
-    Py_XINCREF(local_tb);
-    Py_XINCREF(local_type);
-    Py_XINCREF(local_value);
-    *type = local_type;
-    *value = local_value;
-    *tb = local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    #if CYTHON_USE_EXC_INFO_STACK
-    {
-        _PyErr_StackItem *exc_info = tstate->exc_info;
-        tmp_type = exc_info->exc_type;
-        tmp_value = exc_info->exc_value;
-        tmp_tb = exc_info->exc_traceback;
-        exc_info->exc_type = local_type;
-        exc_info->exc_value = local_value;
-        exc_info->exc_traceback = local_tb;
-    }
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = local_type;
-    tstate->exc_value = local_value;
-    tstate->exc_traceback = local_tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-#else
-    PyErr_SetExcInfo(local_type, local_value, local_tb);
-#endif
-    return 0;
-bad:
-    *type = 0;
-    *value = 0;
-    *tb = 0;
-    Py_XDECREF(local_type);
-    Py_XDECREF(local_value);
-    Py_XDECREF(local_tb);
-    return -1;
-}
-
 /* CalculateMetaclass */
 static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases) {
     Py_ssize_t i, nbases = PyTuple_GET_SIZE(bases);
     for (i=0; i < nbases; i++) {
         PyTypeObject *tmptype;
         PyObject *tmp = PyTuple_GET_ITEM(bases, i);
         tmptype = Py_TYPE(tmp);
```

### Comparing `python-frog-0.6.5/frog_wrapper.pyx` & `python-frog-0.6.6/frog_wrapper.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -251,15 +251,21 @@
         print(f"Frogdata configuration directory already exists: {frogdir}, refusing to overwrite, please remove it first if you want to install the data anew.", file=sys.stderr)
     else:
         tmpdir=os.environ.get("TMPDIR","/tmp")
         if os.system(f"cd {tmpdir} && mkdir -p {frogdir} && wget -O frogdata.tar.gz https://github.com/LanguageMachines/frogdata/releases/download/v{frogdataversion}/frogdata-{frogdataversion}.tar.gz && tar -xzf frogdata.tar.gz && cd frogdata-{frogdataversion} && mv config/* {frogdir}/ && cd .. && rm -Rf frogdata-{frogdataversion} && rm -Rf frogdata.tar.gz") != 0:
             raise Exception("Installation of frogdata failed")
         print(f"Installation of frogdata {frogdataversion} complete", file=sys.stderr)
 
-    if os.path.isdir("/usr/share/libexttextcat"):
+    textcatpath = os.environ.get("TEXTCATPATH","/usr/share/libexttextcat")
+    if os.path.isdir(textcatpath):
         if os.system(f"cd {uctodir} && wget -O textcat.cfg https://raw.githubusercontent.com/LanguageMachines/ucto/master/config/textcat.cfg") != 0:
             raise Exception("Installation of textcat.cfg failed.")
+        if textcatpath[-1] == '/': textcatpath = textcatpath[:-1]
+        if textcatpath != "/usr/share/libexttextcat":
+            data = open(f"{uctodir}/textcat.cfg",'r',encoding='utf-8').read()
+            with open(f"{uctodir}/textcat.cfg",'w',encoding='utf-8') as f:
+                f.write(data.replace("/usr/share/libexttextcat", textcatpath))
     else:
-        print("Language detection will not be available unless you install libexttextcat and rerun installdata()", file=sys.stderr)
+        print("Language detection will not be available unless you install libexttextcat and rerun installdata(). Libexttextcat was not found. If it is in a non-standard location, set environment variable TEXTCATPATH (defaults to /usr/share/libexttextcat) prior to calling installdata()", file=sys.stderr)
```

### Comparing `python-frog-0.6.5/libfolia_classes.pxd` & `python-frog-0.6.6/libfolia_classes.pxd`

 * *Files identical despite different names*

### Comparing `python-frog-0.6.5/python_frog.egg-info/PKG-INFO` & `python-frog-0.6.6/python_frog.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: python-frog
-Version: 0.6.5
+Version: 0.6.6
 Summary: Python binding to Frog, an NLP suite for Dutch doing part-of-speech tagging, lemmatisation, morphological analysis, named-entity recognition, shallow parsing, and dependency parsing.
 Home-page: https://github.com/proycon/python-frog
 Author: Maarten van Gompel
 Author-email: proycon@anaproy.nl
 License: GPLv3
 Keywords: nlp computational_linguistics dutch pos lemmatizer
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires: frog (>=0.27)
-Requires: ucto (>=0.28)
+Requires: frog (>=0.30)
+Requires: ucto (>=0.29)
 License-File: LICENSE
```

### Comparing `python-frog-0.6.5/setup.py` & `python-frog-0.6.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,24 +53,24 @@
                        ],
                 compiler_directives={"language_level": "3"}
                 )
 
 
 setup(
     name = 'python-frog',
-    version = '0.6.5', #also ensure UCTODATAVERSION and FROGDATAVERSION are good in frog_wrapper.pyx
+    version = '0.6.6', #also ensure UCTODATAVERSION and FROGDATAVERSION are good in frog_wrapper.pyx
     author = "Maarten van Gompel",
     author_email = "proycon@anaproy.nl",
     description = ("Python binding to Frog, an NLP suite for Dutch doing part-of-speech tagging, lemmatisation, morphological analysis, named-entity recognition, shallow parsing, and dependency parsing."),
     license = "GPLv3",
     keywords = "nlp computational_linguistics dutch pos lemmatizer",
     url = "https://github.com/proycon/python-frog",
     ext_modules = extensions,
     cmdclass = {'build_ext': build_ext},
-    requires = ['frog (>=0.27)','ucto (>=0.28)'],
+    requires = ['frog (>=0.30)','ucto (>=0.29)'],
     install_requires=['Cython'],
     data_files = [("sources",["frog_wrapper.pyx"])],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Topic :: Text Processing :: Linguistic",
         "Programming Language :: Cython",
         "Programming Language :: Python :: 3",
```

