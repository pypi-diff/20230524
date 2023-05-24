# Comparing `tmp/tenforce-0.1.3.tar.gz` & `tmp/tenforce-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenforce-0.1.3.tar", last modified: Tue May 23 16:21:36 2023, max compression
+gzip compressed data, was "tenforce-0.1.4.tar", last modified: Wed May 24 20:04:18 2023, max compression
```

## Comparing `tenforce-0.1.3.tar` & `tenforce-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,30 @@
-drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2023-05-23 16:21:36.140056 tenforce-0.1.3/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     1071 2023-05-23 13:05:06.000000 tenforce-0.1.3/LICENSE.md
--rw-rw-r--   0 hunter    (1000) hunter    (1000)       29 2023-05-22 17:02:22.000000 tenforce-0.1.3/MANIFEST.in
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     3681 2023-05-23 16:21:36.140056 tenforce-0.1.3/PKG-INFO
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     2261 2023-05-23 15:10:19.000000 tenforce-0.1.3/README.md
--rw-rw-r--   0 hunter    (1000) hunter    (1000)      363 2023-05-23 15:34:43.000000 tenforce-0.1.3/pyproject.toml
--rw-rw-r--   0 hunter    (1000) hunter    (1000)       38 2023-05-23 16:21:36.140056 tenforce-0.1.3/setup.cfg
--rw-rw-r--   0 hunter    (1000) hunter    (1000)      227 2023-05-23 16:20:42.000000 tenforce-0.1.3/setup.py
-drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2023-05-23 16:21:36.140056 tenforce-0.1.3/tenforce/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        0 2023-05-22 17:02:22.000000 tenforce-0.1.3/tenforce/__init__.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)   390904 2023-05-23 16:21:35.000000 tenforce-0.1.3/tenforce/enforcer.c
--rw-rw-r--   0 hunter    (1000) hunter    (1000)      259 2023-05-23 16:18:13.000000 tenforce-0.1.3/tenforce/enforcer.pyi
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     6323 2023-05-23 16:15:17.000000 tenforce-0.1.3/tenforce/enforcer.pyx
--rw-rw-r--   0 hunter    (1000) hunter    (1000)      551 2023-05-23 13:05:06.000000 tenforce-0.1.3/tenforce/exceptions.py
-drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2023-05-23 16:21:36.140056 tenforce-0.1.3/tenforce.egg-info/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     3681 2023-05-23 16:21:36.000000 tenforce-0.1.3/tenforce.egg-info/PKG-INFO
--rw-rw-r--   0 hunter    (1000) hunter    (1000)      306 2023-05-23 16:21:36.000000 tenforce-0.1.3/tenforce.egg-info/SOURCES.txt
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        1 2023-05-23 16:21:36.000000 tenforce-0.1.3/tenforce.egg-info/dependency_links.txt
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        9 2023-05-23 16:21:36.000000 tenforce-0.1.3/tenforce.egg-info/top_level.txt
-drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2023-05-23 16:21:36.140056 tenforce-0.1.3/tests/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     2088 2023-05-23 15:16:54.000000 tenforce-0.1.3/tests/test.py
+drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2023-05-24 20:04:18.950206 tenforce-0.1.4/
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     1071 2023-05-23 13:05:06.000000 tenforce-0.1.4/LICENSE.md
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)       49 2023-05-24 20:02:30.000000 tenforce-0.1.4/MANIFEST.in
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     3794 2023-05-24 20:04:18.950206 tenforce-0.1.4/PKG-INFO
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     2261 2023-05-23 15:10:19.000000 tenforce-0.1.4/README.md
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)      529 2023-05-24 20:03:52.000000 tenforce-0.1.4/pyproject.toml
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)       38 2023-05-24 20:04:18.950206 tenforce-0.1.4/setup.cfg
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)      320 2023-05-24 19:58:53.000000 tenforce-0.1.4/setup.py
+drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2023-05-24 20:04:18.946205 tenforce-0.1.4/tenforce/
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)        0 2023-05-22 17:02:22.000000 tenforce-0.1.4/tenforce/__init__.pyx
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)   201727 2023-05-24 20:04:18.000000 tenforce-0.1.4/tenforce/enforcer.c
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)      318 2023-05-23 20:19:38.000000 tenforce-0.1.4/tenforce/enforcer.pyi
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     2241 2023-05-24 19:56:06.000000 tenforce-0.1.4/tenforce/enforcer.pyx
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)      580 2023-05-24 18:37:55.000000 tenforce-0.1.4/tenforce/exceptions.py
+drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2023-05-24 20:04:18.950206 tenforce-0.1.4/tenforce/lib/
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)        0 2023-05-24 19:38:01.000000 tenforce-0.1.4/tenforce/lib/__init__.py
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)        0 2023-05-24 18:43:39.000000 tenforce-0.1.4/tenforce/lib/__init__.pyx
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)   156414 2023-05-24 20:04:18.000000 tenforce-0.1.4/tenforce/lib/autocast.c
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)      836 2023-05-24 18:37:55.000000 tenforce-0.1.4/tenforce/lib/autocast.pyx
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)   354384 2023-05-24 20:04:18.000000 tenforce-0.1.4/tenforce/lib/members.c
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     2204 2023-05-24 19:48:24.000000 tenforce-0.1.4/tenforce/lib/members.pyx
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)   220630 2023-05-24 20:04:18.000000 tenforce-0.1.4/tenforce/lib/parser.c
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     3298 2023-05-24 19:27:08.000000 tenforce-0.1.4/tenforce/lib/parser.pyx
+drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2023-05-24 20:04:18.946205 tenforce-0.1.4/tenforce.egg-info/
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     3794 2023-05-24 20:04:18.000000 tenforce-0.1.4/tenforce.egg-info/PKG-INFO
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)      502 2023-05-24 20:04:18.000000 tenforce-0.1.4/tenforce.egg-info/SOURCES.txt
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)        1 2023-05-24 20:04:18.000000 tenforce-0.1.4/tenforce.egg-info/dependency_links.txt
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)        9 2023-05-24 20:04:18.000000 tenforce-0.1.4/tenforce.egg-info/top_level.txt
+drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2023-05-24 20:04:18.950206 tenforce-0.1.4/tests/
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     3632 2023-05-24 18:37:55.000000 tenforce-0.1.4/tests/test.py
```

### Comparing `tenforce-0.1.3/LICENSE.md` & `tenforce-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tenforce-0.1.3/PKG-INFO` & `tenforce-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: tenforce
-Version: 0.1.3
+Version: 0.1.4
 Summary: Type enforcement for Python
+Author-email: Hunter LaFaille <hunterlafaille@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hunter LaFaille
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -19,14 +20,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+Keywords: type enforcement,validation,fast,types,cython
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Tenforce
 
 **T**ype **enforce**ment for Python.
```

### Comparing `tenforce-0.1.3/README.md` & `tenforce-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tenforce-0.1.3/tenforce/enforcer.c` & `tenforce-0.1.4/tenforce/lib/members.c`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
-        "name": "tenforce.enforcer",
+        "name": "tenforce.lib.members",
         "sources": [
-            "tenforce/enforcer.pyx"
+            "tenforce/lib/members.pyx"
         ]
     },
-    "module_name": "tenforce.enforcer"
+    "module_name": "tenforce.lib.members"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
 #define CYTHON_ABI "0_29_34"
 #define CYTHON_HEX_VERSION 0x001D22F0
-#define CYTHON_FUTURE_DIVISION 1
+#define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
     #define __stdcall
@@ -746,16 +746,16 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__tenforce__enforcer
-#define __PYX_HAVE_API__tenforce__enforcer
+#define __PYX_HAVE__tenforce__lib__members
+#define __PYX_HAVE_API__tenforce__lib__members
 /* Early includes */
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
@@ -958,123 +958,115 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "tenforce/enforcer.pyx",
+  "tenforce/lib/members.pyx",
   "stringsource",
 };
 
 /*--- Type declarations ---*/
-struct __pyx_obj_8tenforce_8enforcer_ParsedMember;
-struct __pyx_obj_8tenforce_8enforcer_ParsedListMember;
-struct __pyx_opt_args_8tenforce_8enforcer__parse_generic_alias_member;
-struct __pyx_opt_args_8tenforce_8enforcer__parse_member;
-struct __pyx_opt_args_8tenforce_8enforcer_check;
+struct __pyx_obj_8tenforce_3lib_7members_ParsedMember;
+struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember;
+struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember;
 
-/* "tenforce/enforcer.pyx":79
- *     return obj
- * 
- * cpdef ParsedListMember _parse_generic_alias_member(str class_name, str member_name, object generic_alias, object obj, bint auto_cast = False):             # <<<<<<<<<<<<<<
- *     """
- *     Parses a member of a class that has a GenericAlias type annotation (ex: list[str])
- */
-struct __pyx_opt_args_8tenforce_8enforcer__parse_generic_alias_member {
-  int __pyx_n;
-  int auto_cast;
-};
-
-/* "tenforce/enforcer.pyx":114
- *     return plm
- * 
- * cpdef ParsedMember _parse_member(str class_name, str member_name, type annotation, object obj, bint auto_cast = False):             # <<<<<<<<<<<<<<
- *     """
- *     Parses a standard member of a class
- */
-struct __pyx_opt_args_8tenforce_8enforcer__parse_member {
-  int __pyx_n;
-  int auto_cast;
-};
-
-/* "tenforce/enforcer.pyx":142
- * 
- * 
- * cpdef check(object obj, bint auto_cast = False):             # <<<<<<<<<<<<<<
- *     """
- *     Checks the class variables of an object & enforces its type hints
- */
-struct __pyx_opt_args_8tenforce_8enforcer_check {
-  int __pyx_n;
-  int auto_cast;
-};
-
-/* "tenforce/enforcer.pyx":7
- * from tenforce.exceptions import TypeEnforcementError, AutoCastError
- * 
+/* "tenforce/lib/members.pxd":1
  * cdef class ParsedMember:             # <<<<<<<<<<<<<<
  *     cdef type annotated_type
  *     cdef type actual_type
  */
-struct __pyx_obj_8tenforce_8enforcer_ParsedMember {
+struct __pyx_obj_8tenforce_3lib_7members_ParsedMember {
   PyObject_HEAD
-  struct __pyx_vtabstruct_8tenforce_8enforcer_ParsedMember *__pyx_vtab;
+  struct __pyx_vtabstruct_8tenforce_3lib_7members_ParsedMember *__pyx_vtab;
   PyTypeObject *annotated_type;
   PyTypeObject *actual_type;
   PyObject *obj;
   PyObject *member_name;
   PyObject *class_name;
 };
 
 
-/* "tenforce/enforcer.pyx":31
- * 
+/* "tenforce/lib/members.pxd":9
+ *     cpdef enforce(self)
  * 
  * cdef class ParsedListMember:             # <<<<<<<<<<<<<<
  *     cdef type base_annotated_type
  *     cdef list list_
  */
-struct __pyx_obj_8tenforce_8enforcer_ParsedListMember {
+struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember {
   PyObject_HEAD
-  struct __pyx_vtabstruct_8tenforce_8enforcer_ParsedListMember *__pyx_vtab;
+  struct __pyx_vtabstruct_8tenforce_3lib_7members_ParsedListMember *__pyx_vtab;
   PyTypeObject *base_annotated_type;
   PyObject *list_;
   PyObject *member_name;
   PyObject *class_name;
 };
 
 
+/* "tenforce/lib/members.pxd":16
+ *     cpdef enforce(self)
+ * 
+ * cdef class ParsedUnionMember:             # <<<<<<<<<<<<<<
+ *     cdef tuple allowed_types
+ *     cdef type actual_type
+ */
+struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember {
+  PyObject_HEAD
+  struct __pyx_vtabstruct_8tenforce_3lib_7members_ParsedUnionMember *__pyx_vtab;
+  PyObject *allowed_types;
+  PyTypeObject *actual_type;
+  PyObject *obj;
+  PyObject *member_name;
+  PyObject *class_name;
+};
+
+
 
-/* "tenforce/enforcer.pyx":7
- * from tenforce.exceptions import TypeEnforcementError, AutoCastError
+/* "tenforce/lib/members.pyx":3
+ * from tenforce.exceptions import TypeEnforcementError
  * 
  * cdef class ParsedMember:             # <<<<<<<<<<<<<<
- *     cdef type annotated_type
- *     cdef type actual_type
+ *     cpdef enforce(self):
+ *         """
  */
 
-struct __pyx_vtabstruct_8tenforce_8enforcer_ParsedMember {
-  PyObject *(*enforce)(struct __pyx_obj_8tenforce_8enforcer_ParsedMember *, int __pyx_skip_dispatch);
+struct __pyx_vtabstruct_8tenforce_3lib_7members_ParsedMember {
+  PyObject *(*enforce)(struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *, int __pyx_skip_dispatch);
 };
-static struct __pyx_vtabstruct_8tenforce_8enforcer_ParsedMember *__pyx_vtabptr_8tenforce_8enforcer_ParsedMember;
+static struct __pyx_vtabstruct_8tenforce_3lib_7members_ParsedMember *__pyx_vtabptr_8tenforce_3lib_7members_ParsedMember;
 
 
-/* "tenforce/enforcer.pyx":31
+/* "tenforce/lib/members.pyx":20
  * 
  * 
  * cdef class ParsedListMember:             # <<<<<<<<<<<<<<
- *     cdef type base_annotated_type
- *     cdef list list_
+ *     cpdef enforce(self):
+ *         """
+ */
+
+struct __pyx_vtabstruct_8tenforce_3lib_7members_ParsedListMember {
+  PyObject *(*enforce)(struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *, int __pyx_skip_dispatch);
+};
+static struct __pyx_vtabstruct_8tenforce_3lib_7members_ParsedListMember *__pyx_vtabptr_8tenforce_3lib_7members_ParsedListMember;
+
+
+/* "tenforce/lib/members.pyx":41
+ * 
+ * 
+ * cdef class ParsedUnionMember:             # <<<<<<<<<<<<<<
+ *     cpdef enforce(self):
+ *         """
  */
 
-struct __pyx_vtabstruct_8tenforce_8enforcer_ParsedListMember {
-  PyObject *(*enforce)(struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *, int __pyx_skip_dispatch);
+struct __pyx_vtabstruct_8tenforce_3lib_7members_ParsedUnionMember {
+  PyObject *(*enforce)(struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *, int __pyx_skip_dispatch);
 };
-static struct __pyx_vtabstruct_8tenforce_8enforcer_ParsedListMember *__pyx_vtabptr_8tenforce_8enforcer_ParsedListMember;
+static struct __pyx_vtabstruct_8tenforce_3lib_7members_ParsedUnionMember *__pyx_vtabptr_8tenforce_3lib_7members_ParsedUnionMember;
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
@@ -1324,36 +1316,14 @@
     (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
                                                               int wraparound, int boundscheck);
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
                                                      int is_list, int wraparound, int boundscheck);
 
-/* PyUnicode_Unicode.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyUnicode_Unicode(PyObject *obj);
-
-/* GCCDiagnostics.proto */
-#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
-#define __Pyx_HAS_GCC_DIAGNOSTIC
-#endif
-
-/* BuildPyUnicode.proto */
-static PyObject* __Pyx_PyUnicode_BuildFromAscii(Py_ssize_t ulength, char* chars, int clength,
-                                                int prepend_sign, char padding_char);
-
-/* IncludeStringH.proto */
-#include <string.h>
-
-/* CIntToPyUnicode.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_int(int value, Py_ssize_t width, char padding_char, char format_char);
-
-/* JoinPyUnicode.proto */
-static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
-                                      Py_UCS4 max_char);
-
 /* PyObjectFormatSimple.proto */
 #if CYTHON_COMPILING_IN_PYPY
     #define __Pyx_PyObject_FormatSimple(s, f) (\
         likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
         PyObject_Format(s, f))
 #elif PY_MAJOR_VERSION < 3
     #define __Pyx_PyObject_FormatSimple(s, f) (\
@@ -1368,155 +1338,60 @@
         PyObject_Format(s, f))
 #else
     #define __Pyx_PyObject_FormatSimple(s, f) (\
         likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
         PyObject_Format(s, f))
 #endif
 
-/* PyObjectCall2Args.proto */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
+/* GCCDiagnostics.proto */
+#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#define __Pyx_HAS_GCC_DIAGNOSTIC
+#endif
+
+/* BuildPyUnicode.proto */
+static PyObject* __Pyx_PyUnicode_BuildFromAscii(Py_ssize_t ulength, char* chars, int clength,
+                                                int prepend_sign, char padding_char);
+
+/* IncludeStringH.proto */
+#include <string.h>
+
+/* CIntToPyUnicode.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_int(int value, Py_ssize_t width, char padding_char, char format_char);
+
+/* JoinPyUnicode.proto */
+static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
+                                      Py_UCS4 max_char);
 
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
 /* RaiseDoubleKeywords.proto */
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
 /* ParseKeywords.proto */
 static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
     const char* function_name);
 
-/* ArgTypeTest.proto */
-#define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
-    ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
-        __Pyx__ArgTypeTest(obj, type, name, exact))
-static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
-
-/* SetItemInt.proto */
-#define __Pyx_SetItemInt(o, i, v, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_SetItemInt_Fast(o, (Py_ssize_t)i, v, is_list, wraparound, boundscheck) :\
-    (is_list ? (PyErr_SetString(PyExc_IndexError, "list assignment index out of range"), -1) :\
-               __Pyx_SetItemInt_Generic(o, to_py_func(i), v)))
-static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v);
-static CYTHON_INLINE int __Pyx_SetItemInt_Fast(PyObject *o, Py_ssize_t i, PyObject *v,
-                                               int is_list, int wraparound, int boundscheck);
-
-/* IterFinish.proto */
-static CYTHON_INLINE int __Pyx_IterFinish(void);
-
-/* PyObjectGetMethod.proto */
-static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
-
-/* PyObjectCallMethod0.proto */
-static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name);
-
-/* RaiseNeedMoreValuesToUnpack.proto */
-static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index);
-
-/* RaiseTooManyValuesToUnpack.proto */
-static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected);
-
-/* UnpackItemEndCheck.proto */
-static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected);
-
-/* RaiseNoneIterError.proto */
-static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void);
-
-/* UnpackTupleError.proto */
-static void __Pyx_UnpackTupleError(PyObject *, Py_ssize_t index);
-
-/* UnpackTuple2.proto */
-#define __Pyx_unpack_tuple2(tuple, value1, value2, is_tuple, has_known_size, decref_tuple)\
-    (likely(is_tuple || PyTuple_Check(tuple)) ?\
-        (likely(has_known_size || PyTuple_GET_SIZE(tuple) == 2) ?\
-            __Pyx_unpack_tuple2_exact(tuple, value1, value2, decref_tuple) :\
-            (__Pyx_UnpackTupleError(tuple, 2), -1)) :\
-        __Pyx_unpack_tuple2_generic(tuple, value1, value2, has_known_size, decref_tuple))
-static CYTHON_INLINE int __Pyx_unpack_tuple2_exact(
-    PyObject* tuple, PyObject** value1, PyObject** value2, int decref_tuple);
-static int __Pyx_unpack_tuple2_generic(
-    PyObject* tuple, PyObject** value1, PyObject** value2, int has_known_size, int decref_tuple);
-
-/* dict_iter.proto */
-static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* dict, int is_dict, PyObject* method_name,
-                                                   Py_ssize_t* p_orig_length, int* p_is_dict);
-static CYTHON_INLINE int __Pyx_dict_iter_next(PyObject* dict_or_iter, Py_ssize_t orig_length, Py_ssize_t* ppos,
-                                              PyObject** pkey, PyObject** pvalue, PyObject** pitem, int is_dict);
-
-/* DictGetItem.proto */
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
-#define __Pyx_PyObject_Dict_GetItem(obj, name)\
-    (likely(PyDict_CheckExact(obj)) ?\
-     __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
-#else
-#define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
-#define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
-#endif
-
-/* dict_getitem_default.proto */
-static PyObject* __Pyx_PyDict_GetItemDefault(PyObject* d, PyObject* key, PyObject* default_value);
-
-/* UnpackUnboundCMethod.proto */
-typedef struct {
-    PyObject *type;
-    PyObject **method_name;
-    PyCFunction func;
-    PyObject *method;
-    int flag;
-} __Pyx_CachedCFunction;
-
-/* CallUnboundCMethod1.proto */
-static PyObject* __Pyx__CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg);
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg);
-#else
-#define __Pyx_CallUnboundCMethod1(cfunc, self, arg)  __Pyx__CallUnboundCMethod1(cfunc, self, arg)
-#endif
-
-/* CallUnboundCMethod2.proto */
-static PyObject* __Pyx__CallUnboundCMethod2(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg1, PyObject* arg2);
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030600B1
-static CYTHON_INLINE PyObject *__Pyx_CallUnboundCMethod2(__Pyx_CachedCFunction *cfunc, PyObject *self, PyObject *arg1, PyObject *arg2);
-#else
-#define __Pyx_CallUnboundCMethod2(cfunc, self, arg1, arg2)  __Pyx__CallUnboundCMethod2(cfunc, self, arg1, arg2)
-#endif
-
-/* ListAppend.proto */
-#if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
-static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
-    PyListObject* L = (PyListObject*) list;
-    Py_ssize_t len = Py_SIZE(list);
-    if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
-        Py_INCREF(x);
-        PyList_SET_ITEM(list, len, x);
-        __Pyx_SET_SIZE(list, len + 1);
-        return 0;
-    }
-    return PyList_Append(list, x);
-}
-#else
-#define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
-#endif
-
 /* PySequenceContains.proto */
 static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
     int result = PySequence_Contains(seq, item);
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
 }
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
+/* PyObjectCall2Args.proto */
+static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
+
 /* HasAttr.proto */
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
 
 /* PyObject_GenericGetAttrNoDict.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
@@ -1592,194 +1467,164 @@
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
-static PyObject *__pyx_f_8tenforce_8enforcer_12ParsedMember_enforce(struct __pyx_obj_8tenforce_8enforcer_ParsedMember *__pyx_v_self, int __pyx_skip_dispatch); /* proto*/
-static PyObject *__pyx_f_8tenforce_8enforcer_16ParsedListMember_enforce(struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *__pyx_v_self, int __pyx_skip_dispatch); /* proto*/
+static PyObject *__pyx_f_8tenforce_3lib_7members_12ParsedMember_enforce(struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *__pyx_v_self, int __pyx_skip_dispatch); /* proto*/
+static PyObject *__pyx_f_8tenforce_3lib_7members_16ParsedListMember_enforce(struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *__pyx_v_self, int __pyx_skip_dispatch); /* proto*/
+static PyObject *__pyx_f_8tenforce_3lib_7members_17ParsedUnionMember_enforce(struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *__pyx_v_self, int __pyx_skip_dispatch); /* proto*/
+
+/* Module declarations from 'tenforce.lib.members' */
+static PyTypeObject *__pyx_ptype_8tenforce_3lib_7members_ParsedMember = 0;
+static PyTypeObject *__pyx_ptype_8tenforce_3lib_7members_ParsedListMember = 0;
+static PyTypeObject *__pyx_ptype_8tenforce_3lib_7members_ParsedUnionMember = 0;
+static PyObject *__pyx_f_8tenforce_3lib_7members___pyx_unpickle_ParsedMember__set_state(struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *, PyObject *); /*proto*/
+static PyObject *__pyx_f_8tenforce_3lib_7members___pyx_unpickle_ParsedListMember__set_state(struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *, PyObject *); /*proto*/
+static PyObject *__pyx_f_8tenforce_3lib_7members___pyx_unpickle_ParsedUnionMember__set_state(struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *, PyObject *); /*proto*/
+#define __Pyx_MODULE_NAME "tenforce.lib.members"
+extern int __pyx_module_is_main_tenforce__lib__members;
+int __pyx_module_is_main_tenforce__lib__members = 0;
 
-/* Module declarations from 'tenforce.enforcer' */
-static PyTypeObject *__pyx_ptype_8tenforce_8enforcer_ParsedMember = 0;
-static PyTypeObject *__pyx_ptype_8tenforce_8enforcer_ParsedListMember = 0;
-static PyObject *__pyx_f_8tenforce_8enforcer__auto_cast(PyObject *, PyTypeObject *, int __pyx_skip_dispatch); /*proto*/
-static struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *__pyx_f_8tenforce_8enforcer__parse_generic_alias_member(PyObject *, PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch, struct __pyx_opt_args_8tenforce_8enforcer__parse_generic_alias_member *__pyx_optional_args); /*proto*/
-static struct __pyx_obj_8tenforce_8enforcer_ParsedMember *__pyx_f_8tenforce_8enforcer__parse_member(PyObject *, PyObject *, PyTypeObject *, PyObject *, int __pyx_skip_dispatch, struct __pyx_opt_args_8tenforce_8enforcer__parse_member *__pyx_optional_args); /*proto*/
-static PyObject *__pyx_f_8tenforce_8enforcer_check(PyObject *, int __pyx_skip_dispatch, struct __pyx_opt_args_8tenforce_8enforcer_check *__pyx_optional_args); /*proto*/
-static PyObject *__pyx_f_8tenforce_8enforcer___pyx_unpickle_ParsedMember__set_state(struct __pyx_obj_8tenforce_8enforcer_ParsedMember *, PyObject *); /*proto*/
-static PyObject *__pyx_f_8tenforce_8enforcer___pyx_unpickle_ParsedListMember__set_state(struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *, PyObject *); /*proto*/
-#define __Pyx_MODULE_NAME "tenforce.enforcer"
-extern int __pyx_module_is_main_tenforce__enforcer;
-int __pyx_module_is_main_tenforce__enforcer = 0;
-
-/* Implementation of 'tenforce.enforcer' */
+/* Implementation of 'tenforce.lib.members' */
 static PyObject *__pyx_builtin_range;
-static PyObject *__pyx_builtin_ValueError;
 static const char __pyx_k_[] = "[";
 static const char __pyx_k__2[] = "]";
-static const char __pyx_k__3[] = "'";
-static const char __pyx_k_get[] = "get";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
-static const char __pyx_k_None[] = "None";
 static const char __pyx_k_dict[] = "__dict__";
-static const char __pyx_k_keys[] = "keys";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_test[] = "__test__";
-static const char __pyx_k_class[] = "__class__";
 static const char __pyx_k_range[] = "range";
-static const char __pyx_k_types[] = "types";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reduce[] = "__reduce__";
-static const char __pyx_k_typing[] = "typing";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_enforce[] = "enforce";
-static const char __pyx_k_get_args[] = "get_args";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_var_name[] = "var_name";
-static const char __pyx_k_auto_cast[] = "auto_cast";
-static const char __pyx_k_isnumeric[] = "isnumeric";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
-static const char __pyx_k_ValueError[] = "ValueError";
-static const char __pyx_k_annotation[] = "annotation";
 static const char __pyx_k_class_name[] = "class_name";
-static const char __pyx_k_get_origin[] = "get_origin";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_actual_type[] = "actual_type";
-static const char __pyx_k_annotations[] = "__annotations__";
-static const char __pyx_k_member_name[] = "member_name";
-static const char __pyx_k_GenericAlias[] = "GenericAlias";
 static const char __pyx_k_ParsedMember[] = "ParsedMember";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "stringsource";
-static const char __pyx_k_AutoCastError[] = "AutoCastError";
-static const char __pyx_k_generic_alias[] = "generic_alias";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
-static const char __pyx_k_requested_type[] = "requested_type";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
+static const char __pyx_k_requested_types[] = "requested_types";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_ParsedListMember[] = "ParsedListMember";
-static const char __pyx_k_failed_to_cast_to[] = " failed to cast to ";
-static const char __pyx_k_tenforce_enforcer[] = "tenforce.enforcer";
+static const char __pyx_k_ParsedUnionMember[] = "ParsedUnionMember";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_tenforce_exceptions[] = "tenforce.exceptions";
 static const char __pyx_k_TypeEnforcementError[] = "TypeEnforcementError";
+static const char __pyx_k_tenforce_lib_members[] = "tenforce.lib.members";
 static const char __pyx_k_pyx_unpickle_ParsedMember[] = "__pyx_unpickle_ParsedMember";
 static const char __pyx_k_pyx_unpickle_ParsedListMember[] = "__pyx_unpickle_ParsedListMember";
+static const char __pyx_k_pyx_unpickle_ParsedUnionMember[] = "__pyx_unpickle_ParsedUnionMember";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x2b52d43, 0x2bacb3c, 0xa433fcf) = (actual_type, annotated_type, class_name, member_name, obj))";
-static const char __pyx_k_Unsupported_Generic_Alias_origin[] = "Unsupported Generic Alias origin type '";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_2[] = "Incompatible checksums (0x%x vs (0xd0ed7c0, 0xb986991, 0x5dd79c2) = (base_annotated_type, class_name, list_, member_name))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_3[] = "Incompatible checksums (0x%x vs (0x997196e, 0x521cf66, 0xa47b3e8) = (actual_type, allowed_types, class_name, member_name, obj))";
 static PyObject *__pyx_kp_u_;
-static PyObject *__pyx_n_s_AutoCastError;
-static PyObject *__pyx_n_s_GenericAlias;
 static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
 static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2;
-static PyObject *__pyx_kp_u_None;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_3;
 static PyObject *__pyx_n_s_ParsedListMember;
 static PyObject *__pyx_n_s_ParsedMember;
+static PyObject *__pyx_n_s_ParsedUnionMember;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_TypeEnforcementError;
-static PyObject *__pyx_kp_u_Unsupported_Generic_Alias_origin;
-static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_kp_u__2;
-static PyObject *__pyx_kp_u__3;
 static PyObject *__pyx_n_s_actual_type;
-static PyObject *__pyx_n_s_annotation;
-static PyObject *__pyx_n_s_annotations;
-static PyObject *__pyx_n_s_auto_cast;
-static PyObject *__pyx_n_s_class;
 static PyObject *__pyx_n_s_class_name;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_enforce;
-static PyObject *__pyx_kp_u_failed_to_cast_to;
-static PyObject *__pyx_n_s_generic_alias;
-static PyObject *__pyx_n_s_get;
-static PyObject *__pyx_n_s_get_args;
-static PyObject *__pyx_n_s_get_origin;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_n_s_import;
-static PyObject *__pyx_n_s_isnumeric;
-static PyObject *__pyx_n_s_keys;
 static PyObject *__pyx_n_s_main;
-static PyObject *__pyx_n_s_member_name;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_new;
 static PyObject *__pyx_n_s_obj;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_result;
 static PyObject *__pyx_n_s_pyx_state;
 static PyObject *__pyx_n_s_pyx_type;
 static PyObject *__pyx_n_s_pyx_unpickle_ParsedListMember;
 static PyObject *__pyx_n_s_pyx_unpickle_ParsedMember;
+static PyObject *__pyx_n_s_pyx_unpickle_ParsedUnionMember;
 static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
-static PyObject *__pyx_n_s_requested_type;
+static PyObject *__pyx_n_s_requested_types;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_kp_s_stringsource;
-static PyObject *__pyx_n_s_tenforce_enforcer;
 static PyObject *__pyx_n_s_tenforce_exceptions;
+static PyObject *__pyx_n_s_tenforce_lib_members;
 static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_n_s_types;
-static PyObject *__pyx_n_s_typing;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_var_name;
-static PyObject *__pyx_pf_8tenforce_8enforcer_12ParsedMember_enforce(struct __pyx_obj_8tenforce_8enforcer_ParsedMember *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_8tenforce_8enforcer_12ParsedMember_2__reduce_cython__(struct __pyx_obj_8tenforce_8enforcer_ParsedMember *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_8tenforce_8enforcer_12ParsedMember_4__setstate_cython__(struct __pyx_obj_8tenforce_8enforcer_ParsedMember *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_8tenforce_8enforcer_16ParsedListMember_enforce(struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_8tenforce_8enforcer_16ParsedListMember_2__reduce_cython__(struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_8tenforce_8enforcer_16ParsedListMember_4__setstate_cython__(struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_8tenforce_8enforcer__auto_cast(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_obj, PyTypeObject *__pyx_v_annotation); /* proto */
-static PyObject *__pyx_pf_8tenforce_8enforcer_2_parse_generic_alias_member(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_class_name, PyObject *__pyx_v_member_name, PyObject *__pyx_v_generic_alias, PyObject *__pyx_v_obj, int __pyx_v_auto_cast); /* proto */
-static PyObject *__pyx_pf_8tenforce_8enforcer_4_parse_member(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_class_name, PyObject *__pyx_v_member_name, PyTypeObject *__pyx_v_annotation, PyObject *__pyx_v_obj, int __pyx_v_auto_cast); /* proto */
-static PyObject *__pyx_pf_8tenforce_8enforcer_6check(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_obj, int __pyx_v_auto_cast); /* proto */
-static PyObject *__pyx_pf_8tenforce_8enforcer_8__pyx_unpickle_ParsedMember(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_8tenforce_8enforcer_10__pyx_unpickle_ParsedListMember(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_tp_new_8tenforce_8enforcer_ParsedMember(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_8tenforce_8enforcer_ParsedListMember(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_get = {0, &__pyx_n_s_get, 0, 0, 0};
+static PyObject *__pyx_pf_8tenforce_3lib_7members_12ParsedMember_enforce(struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_8tenforce_3lib_7members_12ParsedMember_2__reduce_cython__(struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_8tenforce_3lib_7members_12ParsedMember_4__setstate_cython__(struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_8tenforce_3lib_7members_16ParsedListMember_enforce(struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_8tenforce_3lib_7members_16ParsedListMember_2__reduce_cython__(struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_8tenforce_3lib_7members_16ParsedListMember_4__setstate_cython__(struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_8tenforce_3lib_7members_17ParsedUnionMember_enforce(struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_8tenforce_3lib_7members_17ParsedUnionMember_2__reduce_cython__(struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_8tenforce_3lib_7members_17ParsedUnionMember_4__setstate_cython__(struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_8tenforce_3lib_7members___pyx_unpickle_ParsedMember(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_8tenforce_3lib_7members_2__pyx_unpickle_ParsedListMember(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_8tenforce_3lib_7members_4__pyx_unpickle_ParsedUnionMember(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_tp_new_8tenforce_3lib_7members_ParsedMember(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_8tenforce_3lib_7members_ParsedListMember(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_8tenforce_3lib_7members_ParsedUnionMember(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_45428035;
 static PyObject *__pyx_int_45796156;
+static PyObject *__pyx_int_86101862;
 static PyObject *__pyx_int_98400706;
+static PyObject *__pyx_int_160897390;
 static PyObject *__pyx_int_172179407;
+static PyObject *__pyx_int_172471272;
 static PyObject *__pyx_int_194537873;
 static PyObject *__pyx_int_219076544;
+static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__8;
+static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_codeobj__7;
 static PyObject *__pyx_codeobj__9;
+static PyObject *__pyx_codeobj__11;
 /* Late includes */
 
-/* "tenforce/enforcer.pyx":14
- *     cdef str class_name
+/* "tenforce/lib/members.pyx":4
  * 
+ * cdef class ParsedMember:
  *     cpdef enforce(self):             # <<<<<<<<<<<<<<
  *         """
  *         Enforces the type for this ParsedMember
  */
 
-static PyObject *__pyx_pw_8tenforce_8enforcer_12ParsedMember_1enforce(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_f_8tenforce_8enforcer_12ParsedMember_enforce(struct __pyx_obj_8tenforce_8enforcer_ParsedMember *__pyx_v_self, int __pyx_skip_dispatch) {
+static PyObject *__pyx_pw_8tenforce_3lib_7members_12ParsedMember_1enforce(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_f_8tenforce_3lib_7members_12ParsedMember_enforce(struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *__pyx_v_self, int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
@@ -1793,32 +1638,32 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_enforce); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_enforce); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_8tenforce_8enforcer_12ParsedMember_1enforce)) {
+      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_8tenforce_3lib_7members_12ParsedMember_1enforce)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -1831,190 +1676,196 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "tenforce/enforcer.pyx":21
+  /* "tenforce/lib/members.pyx":10
+ *         :return: None
  *         """
- *         #print(f"{self.class_name}.{self.member_name}: {self.annotated_type} | {self.actual_type} = {self.obj}")
  *         if self.actual_type is not self.annotated_type:             # <<<<<<<<<<<<<<
  *             raise TypeEnforcementError(
  *                 class_name=self.class_name,
  */
   __pyx_t_5 = (__pyx_v_self->actual_type != __pyx_v_self->annotated_type);
   __pyx_t_6 = (__pyx_t_5 != 0);
   if (unlikely(__pyx_t_6)) {
 
-    /* "tenforce/enforcer.pyx":22
- *         #print(f"{self.class_name}.{self.member_name}: {self.annotated_type} | {self.actual_type} = {self.obj}")
+    /* "tenforce/lib/members.pyx":11
+ *         """
  *         if self.actual_type is not self.annotated_type:
  *             raise TypeEnforcementError(             # <<<<<<<<<<<<<<
  *                 class_name=self.class_name,
  *                 var_name=self.member_name,
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_TypeEnforcementError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 22, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_TypeEnforcementError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
 
-    /* "tenforce/enforcer.pyx":23
+    /* "tenforce/lib/members.pyx":12
  *         if self.actual_type is not self.annotated_type:
  *             raise TypeEnforcementError(
  *                 class_name=self.class_name,             # <<<<<<<<<<<<<<
  *                 var_name=self.member_name,
- *                 requested_type=self.annotated_type,
+ *                 requested_types=[self.annotated_type],
  */
-    __pyx_t_2 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 23, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_class_name, __pyx_v_self->class_name) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_class_name, __pyx_v_self->class_name) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
 
-    /* "tenforce/enforcer.pyx":24
+    /* "tenforce/lib/members.pyx":13
  *             raise TypeEnforcementError(
  *                 class_name=self.class_name,
  *                 var_name=self.member_name,             # <<<<<<<<<<<<<<
- *                 requested_type=self.annotated_type,
+ *                 requested_types=[self.annotated_type],
  *                 actual_type=self.actual_type,
  */
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_var_name, __pyx_v_self->member_name) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_var_name, __pyx_v_self->member_name) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
 
-    /* "tenforce/enforcer.pyx":25
+    /* "tenforce/lib/members.pyx":14
  *                 class_name=self.class_name,
  *                 var_name=self.member_name,
- *                 requested_type=self.annotated_type,             # <<<<<<<<<<<<<<
+ *                 requested_types=[self.annotated_type],             # <<<<<<<<<<<<<<
  *                 actual_type=self.actual_type,
  *                 obj=self.obj
  */
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_requested_type, ((PyObject *)__pyx_v_self->annotated_type)) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_INCREF(((PyObject *)__pyx_v_self->annotated_type));
+    __Pyx_GIVEREF(((PyObject *)__pyx_v_self->annotated_type));
+    PyList_SET_ITEM(__pyx_t_3, 0, ((PyObject *)__pyx_v_self->annotated_type));
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_requested_types, __pyx_t_3) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "tenforce/enforcer.pyx":26
+    /* "tenforce/lib/members.pyx":15
  *                 var_name=self.member_name,
- *                 requested_type=self.annotated_type,
+ *                 requested_types=[self.annotated_type],
  *                 actual_type=self.actual_type,             # <<<<<<<<<<<<<<
  *                 obj=self.obj
  *             )
  */
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_actual_type, ((PyObject *)__pyx_v_self->actual_type)) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_actual_type, ((PyObject *)__pyx_v_self->actual_type)) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
 
-    /* "tenforce/enforcer.pyx":27
- *                 requested_type=self.annotated_type,
+    /* "tenforce/lib/members.pyx":16
+ *                 requested_types=[self.annotated_type],
  *                 actual_type=self.actual_type,
  *                 obj=self.obj             # <<<<<<<<<<<<<<
  *             )
  * 
  */
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_obj, __pyx_v_self->obj) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_obj, __pyx_v_self->obj) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
 
-    /* "tenforce/enforcer.pyx":22
- *         #print(f"{self.class_name}.{self.member_name}: {self.annotated_type} | {self.actual_type} = {self.obj}")
+    /* "tenforce/lib/members.pyx":11
+ *         """
  *         if self.actual_type is not self.annotated_type:
  *             raise TypeEnforcementError(             # <<<<<<<<<<<<<<
  *                 class_name=self.class_name,
  *                 var_name=self.member_name,
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 11, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 22, __pyx_L1_error)
+    __PYX_ERR(0, 11, __pyx_L1_error)
 
-    /* "tenforce/enforcer.pyx":21
+    /* "tenforce/lib/members.pyx":10
+ *         :return: None
  *         """
- *         #print(f"{self.class_name}.{self.member_name}: {self.annotated_type} | {self.actual_type} = {self.obj}")
  *         if self.actual_type is not self.annotated_type:             # <<<<<<<<<<<<<<
  *             raise TypeEnforcementError(
  *                 class_name=self.class_name,
  */
   }
 
-  /* "tenforce/enforcer.pyx":14
- *     cdef str class_name
+  /* "tenforce/lib/members.pyx":4
  * 
+ * cdef class ParsedMember:
  *     cpdef enforce(self):             # <<<<<<<<<<<<<<
  *         """
  *         Enforces the type for this ParsedMember
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("tenforce.enforcer.ParsedMember.enforce", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("tenforce.lib.members.ParsedMember.enforce", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8tenforce_8enforcer_12ParsedMember_1enforce(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_8tenforce_8enforcer_12ParsedMember_enforce[] = "\n        Enforces the type for this ParsedMember\n        :raises TypeEnforcementError: if there is a mismatched type\n        :return: None\n        ";
-static PyObject *__pyx_pw_8tenforce_8enforcer_12ParsedMember_1enforce(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_8tenforce_3lib_7members_12ParsedMember_1enforce(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_8tenforce_3lib_7members_12ParsedMember_enforce[] = "\n        Enforces the type for this ParsedMember\n        :raises TypeEnforcementError: if there is a mismatched type\n        :return: None\n        ";
+static PyObject *__pyx_pw_8tenforce_3lib_7members_12ParsedMember_1enforce(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("enforce (wrapper)", 0);
-  __pyx_r = __pyx_pf_8tenforce_8enforcer_12ParsedMember_enforce(((struct __pyx_obj_8tenforce_8enforcer_ParsedMember *)__pyx_v_self));
+  __pyx_r = __pyx_pf_8tenforce_3lib_7members_12ParsedMember_enforce(((struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8tenforce_8enforcer_12ParsedMember_enforce(struct __pyx_obj_8tenforce_8enforcer_ParsedMember *__pyx_v_self) {
+static PyObject *__pyx_pf_8tenforce_3lib_7members_12ParsedMember_enforce(struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("enforce", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8tenforce_8enforcer_12ParsedMember_enforce(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8tenforce_3lib_7members_12ParsedMember_enforce(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("tenforce.enforcer.ParsedMember.enforce", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("tenforce.lib.members.ParsedMember.enforce", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8tenforce_8enforcer_12ParsedMember_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_8tenforce_8enforcer_12ParsedMember_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_8tenforce_3lib_7members_12ParsedMember_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_8tenforce_3lib_7members_12ParsedMember_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_8tenforce_8enforcer_12ParsedMember_2__reduce_cython__(((struct __pyx_obj_8tenforce_8enforcer_ParsedMember *)__pyx_v_self));
+  __pyx_r = __pyx_pf_8tenforce_3lib_7members_12ParsedMember_2__reduce_cython__(((struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8tenforce_8enforcer_12ParsedMember_2__reduce_cython__(struct __pyx_obj_8tenforce_8enforcer_ParsedMember *__pyx_v_self) {
+static PyObject *__pyx_pf_8tenforce_3lib_7members_12ParsedMember_2__reduce_cython__(struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
@@ -2255,15 +2106,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("tenforce.enforcer.ParsedMember.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("tenforce.lib.members.ParsedMember.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_state);
   __Pyx_XDECREF(__pyx_v__dict);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -2273,42 +2124,42 @@
  *     else:
  *         return __pyx_unpickle_ParsedMember, (type(self), 0x2b52d43, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_ParsedMember__set_state(self, __pyx_state)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8tenforce_8enforcer_12ParsedMember_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_8tenforce_8enforcer_12ParsedMember_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_8tenforce_3lib_7members_12ParsedMember_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_8tenforce_3lib_7members_12ParsedMember_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_8tenforce_8enforcer_12ParsedMember_4__setstate_cython__(((struct __pyx_obj_8tenforce_8enforcer_ParsedMember *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_8tenforce_3lib_7members_12ParsedMember_4__setstate_cython__(((struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8tenforce_8enforcer_12ParsedMember_4__setstate_cython__(struct __pyx_obj_8tenforce_8enforcer_ParsedMember *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_8tenforce_3lib_7members_12ParsedMember_4__setstate_cython__(struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_ParsedMember, (type(self), 0x2b52d43, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_ParsedMember__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
   if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
-  __pyx_t_1 = __pyx_f_8tenforce_8enforcer___pyx_unpickle_ParsedMember__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8tenforce_3lib_7members___pyx_unpickle_ParsedMember__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_ParsedMember, (type(self), 0x2b52d43, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
@@ -2316,32 +2167,32 @@
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("tenforce.enforcer.ParsedMember.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("tenforce.lib.members.ParsedMember.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "tenforce/enforcer.pyx":38
- *     # we don't have an actual_type field, since a list can have more than one type!
+/* "tenforce/lib/members.pyx":21
  * 
+ * cdef class ParsedListMember:
  *     cpdef enforce(self):             # <<<<<<<<<<<<<<
  *         """
  *         Enforces the type annotated_type for list_
  */
 
-static PyObject *__pyx_pw_8tenforce_8enforcer_16ParsedListMember_1enforce(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_f_8tenforce_8enforcer_16ParsedListMember_enforce(struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *__pyx_v_self, int __pyx_skip_dispatch) {
+static PyObject *__pyx_pw_8tenforce_3lib_7members_16ParsedListMember_1enforce(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_f_8tenforce_3lib_7members_16ParsedListMember_enforce(struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *__pyx_v_self, int __pyx_skip_dispatch) {
   int __pyx_v_x;
   PyTypeObject *__pyx_v_current_elem_type = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -2362,32 +2213,32 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_enforce); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_enforce); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_8tenforce_8enforcer_16ParsedListMember_1enforce)) {
+      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_8tenforce_3lib_7members_16ParsedListMember_1enforce)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -2400,264 +2251,270 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "tenforce/enforcer.pyx":46
+  /* "tenforce/lib/members.pyx":29
  *         cdef int x
  *         cdef type current_elem_type
  *         for x in range(len(self.list_)):             # <<<<<<<<<<<<<<
  *             current_elem_type = type(self.list_[x])
  *             if current_elem_type is not self.base_annotated_type:
  */
   __pyx_t_1 = __pyx_v_self->list_;
   __Pyx_INCREF(__pyx_t_1);
   if (unlikely(__pyx_t_1 == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 46, __pyx_L1_error)
+    __PYX_ERR(0, 29, __pyx_L1_error)
   }
-  __pyx_t_5 = PyList_GET_SIZE(__pyx_t_1); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_5 = PyList_GET_SIZE(__pyx_t_1); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_6 = __pyx_t_5;
   for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
     __pyx_v_x = __pyx_t_7;
 
-    /* "tenforce/enforcer.pyx":47
+    /* "tenforce/lib/members.pyx":30
  *         cdef type current_elem_type
  *         for x in range(len(self.list_)):
  *             current_elem_type = type(self.list_[x])             # <<<<<<<<<<<<<<
  *             if current_elem_type is not self.base_annotated_type:
  *                 raise TypeEnforcementError(
  */
     if (unlikely(__pyx_v_self->list_ == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 47, __pyx_L1_error)
+      __PYX_ERR(0, 30, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_self->list_, __pyx_v_x, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_self->list_, __pyx_v_x, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(((PyObject *)Py_TYPE(__pyx_t_1)));
     __Pyx_XDECREF_SET(__pyx_v_current_elem_type, ((PyTypeObject*)((PyObject *)Py_TYPE(__pyx_t_1))));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "tenforce/enforcer.pyx":48
+    /* "tenforce/lib/members.pyx":31
  *         for x in range(len(self.list_)):
  *             current_elem_type = type(self.list_[x])
  *             if current_elem_type is not self.base_annotated_type:             # <<<<<<<<<<<<<<
  *                 raise TypeEnforcementError(
  *                     class_name=self.class_name,
  */
     __pyx_t_8 = (__pyx_v_current_elem_type != __pyx_v_self->base_annotated_type);
     __pyx_t_9 = (__pyx_t_8 != 0);
     if (unlikely(__pyx_t_9)) {
 
-      /* "tenforce/enforcer.pyx":49
+      /* "tenforce/lib/members.pyx":32
  *             current_elem_type = type(self.list_[x])
  *             if current_elem_type is not self.base_annotated_type:
  *                 raise TypeEnforcementError(             # <<<<<<<<<<<<<<
  *                     class_name=self.class_name,
  *                     var_name=f"{self.member_name}[{x}]",
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_TypeEnforcementError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_TypeEnforcementError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
 
-      /* "tenforce/enforcer.pyx":50
+      /* "tenforce/lib/members.pyx":33
  *             if current_elem_type is not self.base_annotated_type:
  *                 raise TypeEnforcementError(
  *                     class_name=self.class_name,             # <<<<<<<<<<<<<<
  *                     var_name=f"{self.member_name}[{x}]",
- *                     requested_type=self.base_annotated_type,
+ *                     requested_types=[self.base_annotated_type],
  */
-      __pyx_t_2 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_class_name, __pyx_v_self->class_name) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_class_name, __pyx_v_self->class_name) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
 
-      /* "tenforce/enforcer.pyx":51
+      /* "tenforce/lib/members.pyx":34
  *                 raise TypeEnforcementError(
  *                     class_name=self.class_name,
  *                     var_name=f"{self.member_name}[{x}]",             # <<<<<<<<<<<<<<
- *                     requested_type=self.base_annotated_type,
+ *                     requested_types=[self.base_annotated_type],
  *                     actual_type=current_elem_type,
  */
-      __pyx_t_3 = PyTuple_New(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
+      __pyx_t_3 = PyTuple_New(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 34, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_10 = 0;
       __pyx_t_11 = 127;
-      __pyx_t_4 = __Pyx_PyUnicode_Unicode(__pyx_v_self->member_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 51, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_v_self->member_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 34, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_11 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) > __pyx_t_11) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) : __pyx_t_11;
       __pyx_t_10 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
       __pyx_t_4 = 0;
       __Pyx_INCREF(__pyx_kp_u_);
       __pyx_t_10 += 1;
       __Pyx_GIVEREF(__pyx_kp_u_);
       PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_kp_u_);
-      __pyx_t_4 = __Pyx_PyUnicode_From_int(__pyx_v_x, 0, ' ', 'd'); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 51, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyUnicode_From_int(__pyx_v_x, 0, ' ', 'd'); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 34, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_10 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_4);
       __pyx_t_4 = 0;
       __Pyx_INCREF(__pyx_kp_u__2);
       __pyx_t_10 += 1;
       __Pyx_GIVEREF(__pyx_kp_u__2);
       PyTuple_SET_ITEM(__pyx_t_3, 3, __pyx_kp_u__2);
-      __pyx_t_4 = __Pyx_PyUnicode_Join(__pyx_t_3, 4, __pyx_t_10, __pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 51, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyUnicode_Join(__pyx_t_3, 4, __pyx_t_10, __pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 34, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_var_name, __pyx_t_4) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_var_name, __pyx_t_4) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "tenforce/enforcer.pyx":52
+      /* "tenforce/lib/members.pyx":35
  *                     class_name=self.class_name,
  *                     var_name=f"{self.member_name}[{x}]",
- *                     requested_type=self.base_annotated_type,             # <<<<<<<<<<<<<<
+ *                     requested_types=[self.base_annotated_type],             # <<<<<<<<<<<<<<
  *                     actual_type=current_elem_type,
  *                     obj=self.list_[x]
  */
-      if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_requested_type, ((PyObject *)__pyx_v_self->base_annotated_type)) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
+      __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 35, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_INCREF(((PyObject *)__pyx_v_self->base_annotated_type));
+      __Pyx_GIVEREF(((PyObject *)__pyx_v_self->base_annotated_type));
+      PyList_SET_ITEM(__pyx_t_4, 0, ((PyObject *)__pyx_v_self->base_annotated_type));
+      if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_requested_types, __pyx_t_4) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "tenforce/enforcer.pyx":53
+      /* "tenforce/lib/members.pyx":36
  *                     var_name=f"{self.member_name}[{x}]",
- *                     requested_type=self.base_annotated_type,
+ *                     requested_types=[self.base_annotated_type],
  *                     actual_type=current_elem_type,             # <<<<<<<<<<<<<<
  *                     obj=self.list_[x]
  *                 )
  */
-      if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_actual_type, ((PyObject *)__pyx_v_current_elem_type)) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_actual_type, ((PyObject *)__pyx_v_current_elem_type)) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
 
-      /* "tenforce/enforcer.pyx":54
- *                     requested_type=self.base_annotated_type,
+      /* "tenforce/lib/members.pyx":37
+ *                     requested_types=[self.base_annotated_type],
  *                     actual_type=current_elem_type,
  *                     obj=self.list_[x]             # <<<<<<<<<<<<<<
  *                 )
  * 
  */
       if (unlikely(__pyx_v_self->list_ == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 54, __pyx_L1_error)
+        __PYX_ERR(0, 37, __pyx_L1_error)
       }
-      __pyx_t_4 = __Pyx_GetItemInt_List(__pyx_v_self->list_, __pyx_v_x, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 54, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt_List(__pyx_v_self->list_, __pyx_v_x, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 37, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_obj, __pyx_t_4) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_obj, __pyx_t_4) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "tenforce/enforcer.pyx":49
+      /* "tenforce/lib/members.pyx":32
  *             current_elem_type = type(self.list_[x])
  *             if current_elem_type is not self.base_annotated_type:
  *                 raise TypeEnforcementError(             # <<<<<<<<<<<<<<
  *                     class_name=self.class_name,
  *                     var_name=f"{self.member_name}[{x}]",
  */
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 49, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_Raise(__pyx_t_4, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __PYX_ERR(0, 49, __pyx_L1_error)
+      __PYX_ERR(0, 32, __pyx_L1_error)
 
-      /* "tenforce/enforcer.pyx":48
+      /* "tenforce/lib/members.pyx":31
  *         for x in range(len(self.list_)):
  *             current_elem_type = type(self.list_[x])
  *             if current_elem_type is not self.base_annotated_type:             # <<<<<<<<<<<<<<
  *                 raise TypeEnforcementError(
  *                     class_name=self.class_name,
  */
     }
   }
 
-  /* "tenforce/enforcer.pyx":38
- *     # we don't have an actual_type field, since a list can have more than one type!
+  /* "tenforce/lib/members.pyx":21
  * 
+ * cdef class ParsedListMember:
  *     cpdef enforce(self):             # <<<<<<<<<<<<<<
  *         """
  *         Enforces the type annotated_type for list_
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("tenforce.enforcer.ParsedListMember.enforce", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("tenforce.lib.members.ParsedListMember.enforce", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_current_elem_type);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8tenforce_8enforcer_16ParsedListMember_1enforce(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_8tenforce_8enforcer_16ParsedListMember_enforce[] = "\n        Enforces the type annotated_type for list_\n        :raises TypeEnforcementError: if there is a mismatched type\n        :return: \n        ";
-static PyObject *__pyx_pw_8tenforce_8enforcer_16ParsedListMember_1enforce(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_8tenforce_3lib_7members_16ParsedListMember_1enforce(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_8tenforce_3lib_7members_16ParsedListMember_enforce[] = "\n        Enforces the type annotated_type for list_\n        :raises TypeEnforcementError: if there is a mismatched type\n        :return: \n        ";
+static PyObject *__pyx_pw_8tenforce_3lib_7members_16ParsedListMember_1enforce(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("enforce (wrapper)", 0);
-  __pyx_r = __pyx_pf_8tenforce_8enforcer_16ParsedListMember_enforce(((struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *)__pyx_v_self));
+  __pyx_r = __pyx_pf_8tenforce_3lib_7members_16ParsedListMember_enforce(((struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8tenforce_8enforcer_16ParsedListMember_enforce(struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *__pyx_v_self) {
+static PyObject *__pyx_pf_8tenforce_3lib_7members_16ParsedListMember_enforce(struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("enforce", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8tenforce_8enforcer_16ParsedListMember_enforce(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8tenforce_3lib_7members_16ParsedListMember_enforce(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("tenforce.enforcer.ParsedListMember.enforce", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("tenforce.lib.members.ParsedListMember.enforce", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8tenforce_8enforcer_16ParsedListMember_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_8tenforce_8enforcer_16ParsedListMember_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_8tenforce_3lib_7members_16ParsedListMember_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_8tenforce_3lib_7members_16ParsedListMember_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_8tenforce_8enforcer_16ParsedListMember_2__reduce_cython__(((struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *)__pyx_v_self));
+  __pyx_r = __pyx_pf_8tenforce_3lib_7members_16ParsedListMember_2__reduce_cython__(((struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8tenforce_8enforcer_16ParsedListMember_2__reduce_cython__(struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *__pyx_v_self) {
+static PyObject *__pyx_pf_8tenforce_3lib_7members_16ParsedListMember_2__reduce_cython__(struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
@@ -2888,15 +2745,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("tenforce.enforcer.ParsedListMember.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("tenforce.lib.members.ParsedListMember.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_state);
   __Pyx_XDECREF(__pyx_v__dict);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -2906,42 +2763,42 @@
  *     else:
  *         return __pyx_unpickle_ParsedListMember, (type(self), 0xd0ed7c0, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_ParsedListMember__set_state(self, __pyx_state)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8tenforce_8enforcer_16ParsedListMember_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_8tenforce_8enforcer_16ParsedListMember_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_8tenforce_3lib_7members_16ParsedListMember_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_8tenforce_3lib_7members_16ParsedListMember_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_8tenforce_8enforcer_16ParsedListMember_4__setstate_cython__(((struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_8tenforce_3lib_7members_16ParsedListMember_4__setstate_cython__(((struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8tenforce_8enforcer_16ParsedListMember_4__setstate_cython__(struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_8tenforce_3lib_7members_16ParsedListMember_4__setstate_cython__(struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_ParsedListMember, (type(self), 0xd0ed7c0, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_ParsedListMember__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
   if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
-  __pyx_t_1 = __pyx_f_8tenforce_8enforcer___pyx_unpickle_ParsedListMember__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8tenforce_3lib_7members___pyx_unpickle_ParsedListMember__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_ParsedListMember, (type(self), 0xd0ed7c0, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
@@ -2949,1557 +2806,672 @@
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("tenforce.enforcer.ParsedListMember.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("tenforce.lib.members.ParsedListMember.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "tenforce/enforcer.pyx":57
- *                 )
+/* "tenforce/lib/members.pyx":42
  * 
- * cpdef object _auto_cast(object obj, type annotation):             # <<<<<<<<<<<<<<
- *     """
- *     Cast an object to its annotated type
+ * cdef class ParsedUnionMember:
+ *     cpdef enforce(self):             # <<<<<<<<<<<<<<
+ *         """
+ *         Enforces the type for this ParsedMember
  */
 
-static PyObject *__pyx_pw_8tenforce_8enforcer_1_auto_cast(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_f_8tenforce_8enforcer__auto_cast(PyObject *__pyx_v_obj, PyTypeObject *__pyx_v_annotation, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static PyObject *__pyx_pw_8tenforce_3lib_7members_17ParsedUnionMember_1enforce(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_f_8tenforce_3lib_7members_17ParsedUnionMember_enforce(struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *__pyx_v_self, int __pyx_skip_dispatch) {
+  int __pyx_v_x;
+  int __pyx_v_match_found;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  int __pyx_t_2;
-  int __pyx_t_3;
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  Py_ssize_t __pyx_t_7;
-  Py_UCS4 __pyx_t_8;
-  PyObject *__pyx_t_9 = NULL;
+  Py_ssize_t __pyx_t_5;
+  Py_ssize_t __pyx_t_6;
+  int __pyx_t_7;
+  int __pyx_t_8;
+  int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_auto_cast", 0);
-  __Pyx_INCREF(__pyx_v_obj);
-
-  /* "tenforce/enforcer.pyx":66
- *     """
- *     # if the value provided is a numeric string, try and cast it to an int
- *     if type(obj) is str and annotation is int and obj.isnumeric():             # <<<<<<<<<<<<<<
- *         obj = int(obj)
- * 
- */
-  __pyx_t_2 = (((PyObject *)Py_TYPE(__pyx_v_obj)) == ((PyObject *)(&PyUnicode_Type)));
-  __pyx_t_3 = (__pyx_t_2 != 0);
-  if (__pyx_t_3) {
-  } else {
-    __pyx_t_1 = __pyx_t_3;
-    goto __pyx_L4_bool_binop_done;
-  }
-  __pyx_t_3 = (__pyx_v_annotation == (&PyInt_Type));
-  __pyx_t_2 = (__pyx_t_3 != 0);
-  if (__pyx_t_2) {
-  } else {
-    __pyx_t_1 = __pyx_t_2;
-    goto __pyx_L4_bool_binop_done;
-  }
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_obj, __pyx_n_s_isnumeric); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 66, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
-    if (likely(__pyx_t_6)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-      __Pyx_INCREF(__pyx_t_6);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_5, function);
+  __Pyx_RefNannySetupContext("enforce", 0);
+  /* Check if called by wrapper */
+  if (unlikely(__pyx_skip_dispatch)) ;
+  /* Check if overridden in Python */
+  else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
+    #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
+    static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
+    if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
+      PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
+      #endif
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_enforce); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_8tenforce_3lib_7members_17ParsedUnionMember_1enforce)) {
+        __Pyx_XDECREF(__pyx_r);
+        __Pyx_INCREF(__pyx_t_1);
+        __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
+        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+          __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+          if (likely(__pyx_t_4)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+            __Pyx_INCREF(__pyx_t_4);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_3, function);
+          }
+        }
+        __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
+        __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __pyx_r = __pyx_t_2;
+        __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        goto __pyx_L0;
+      }
+      #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
+      __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
+      __pyx_obj_dict_version = __Pyx_get_object_dict_version(((PyObject *)__pyx_v_self));
+      if (unlikely(__pyx_type_dict_guard != __pyx_tp_dict_version)) {
+        __pyx_tp_dict_version = __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
+      }
+      #endif
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
-  }
-  __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 66, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_1 = __pyx_t_2;
-  __pyx_L4_bool_binop_done:;
-  if (__pyx_t_1) {
-
-    /* "tenforce/enforcer.pyx":67
- *     # if the value provided is a numeric string, try and cast it to an int
- *     if type(obj) is str and annotation is int and obj.isnumeric():
- *         obj = int(obj)             # <<<<<<<<<<<<<<
- * 
- *     # if the value provided is an int and the annotation requires a float, try and cast it to a float
- */
-    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_obj); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 67, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF_SET(__pyx_v_obj, __pyx_t_4);
-    __pyx_t_4 = 0;
-
-    /* "tenforce/enforcer.pyx":66
- *     """
- *     # if the value provided is a numeric string, try and cast it to an int
- *     if type(obj) is str and annotation is int and obj.isnumeric():             # <<<<<<<<<<<<<<
- *         obj = int(obj)
- * 
- */
+    #endif
   }
 
-  /* "tenforce/enforcer.pyx":70
- * 
- *     # if the value provided is an int and the annotation requires a float, try and cast it to a float
- *     if type(obj) is int and annotation is float:             # <<<<<<<<<<<<<<
- *         obj = float(obj)
- * 
- */
-  __pyx_t_2 = (((PyObject *)Py_TYPE(__pyx_v_obj)) == ((PyObject *)(&PyInt_Type)));
-  __pyx_t_3 = (__pyx_t_2 != 0);
-  if (__pyx_t_3) {
-  } else {
-    __pyx_t_1 = __pyx_t_3;
-    goto __pyx_L8_bool_binop_done;
-  }
-  __pyx_t_3 = (__pyx_v_annotation == (&PyFloat_Type));
-  __pyx_t_2 = (__pyx_t_3 != 0);
-  __pyx_t_1 = __pyx_t_2;
-  __pyx_L8_bool_binop_done:;
-  if (__pyx_t_1) {
-
-    /* "tenforce/enforcer.pyx":71
- *     # if the value provided is an int and the annotation requires a float, try and cast it to a float
- *     if type(obj) is int and annotation is float:
- *         obj = float(obj)             # <<<<<<<<<<<<<<
- * 
- *     # if we couldn't cast obj
+  /* "tenforce/lib/members.pyx":50
+ *         # try to find a matching type in the union
+ *         cdef int x
+ *         cdef bint match_found = False             # <<<<<<<<<<<<<<
+ *         for x in range(len(self.allowed_types)):
+ *             if self.actual_type is self.allowed_types[x]:
  */
-    __pyx_t_4 = __Pyx_PyNumber_Float(__pyx_v_obj); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 71, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF_SET(__pyx_v_obj, __pyx_t_4);
-    __pyx_t_4 = 0;
+  __pyx_v_match_found = 0;
 
-    /* "tenforce/enforcer.pyx":70
- * 
- *     # if the value provided is an int and the annotation requires a float, try and cast it to a float
- *     if type(obj) is int and annotation is float:             # <<<<<<<<<<<<<<
- *         obj = float(obj)
- * 
+  /* "tenforce/lib/members.pyx":51
+ *         cdef int x
+ *         cdef bint match_found = False
+ *         for x in range(len(self.allowed_types)):             # <<<<<<<<<<<<<<
+ *             if self.actual_type is self.allowed_types[x]:
+ *                 match_found = True
  */
+  __pyx_t_1 = __pyx_v_self->allowed_types;
+  __Pyx_INCREF(__pyx_t_1);
+  if (unlikely(__pyx_t_1 == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+    __PYX_ERR(0, 51, __pyx_L1_error)
   }
+  __pyx_t_5 = PyTuple_GET_SIZE(__pyx_t_1); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_6 = __pyx_t_5;
+  for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
+    __pyx_v_x = __pyx_t_7;
 
-  /* "tenforce/enforcer.pyx":74
- * 
- *     # if we couldn't cast obj
- *     if type(obj) is not annotation:             # <<<<<<<<<<<<<<
- *         raise AutoCastError(f"{obj} failed to cast to {annotation}")
- * 
- */
-  __pyx_t_1 = (((PyObject *)Py_TYPE(__pyx_v_obj)) != ((PyObject *)__pyx_v_annotation));
-  __pyx_t_2 = (__pyx_t_1 != 0);
-  if (unlikely(__pyx_t_2)) {
-
-    /* "tenforce/enforcer.pyx":75
- *     # if we couldn't cast obj
- *     if type(obj) is not annotation:
- *         raise AutoCastError(f"{obj} failed to cast to {annotation}")             # <<<<<<<<<<<<<<
- * 
- *     return obj
+    /* "tenforce/lib/members.pyx":52
+ *         cdef bint match_found = False
+ *         for x in range(len(self.allowed_types)):
+ *             if self.actual_type is self.allowed_types[x]:             # <<<<<<<<<<<<<<
+ *                 match_found = True
+ *                 break
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_AutoCastError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 75, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 75, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = 0;
-    __pyx_t_8 = 127;
-    __pyx_t_9 = __Pyx_PyObject_FormatSimple(__pyx_v_obj, __pyx_empty_unicode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 75, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_8 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_9) > __pyx_t_8) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_9) : __pyx_t_8;
-    __pyx_t_7 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_9);
-    __Pyx_GIVEREF(__pyx_t_9);
-    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_9);
-    __pyx_t_9 = 0;
-    __Pyx_INCREF(__pyx_kp_u_failed_to_cast_to);
-    __pyx_t_7 += 19;
-    __Pyx_GIVEREF(__pyx_kp_u_failed_to_cast_to);
-    PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_kp_u_failed_to_cast_to);
-    __pyx_t_9 = __Pyx_PyObject_FormatSimple(((PyObject *)__pyx_v_annotation), __pyx_empty_unicode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 75, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_8 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_9) > __pyx_t_8) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_9) : __pyx_t_8;
-    __pyx_t_7 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_9);
-    __Pyx_GIVEREF(__pyx_t_9);
-    PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_9);
-    __pyx_t_9 = 0;
-    __pyx_t_9 = __Pyx_PyUnicode_Join(__pyx_t_6, 3, __pyx_t_7, __pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 75, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
-      if (likely(__pyx_t_6)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-        __Pyx_INCREF(__pyx_t_6);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_5, function);
-      }
+    if (unlikely(__pyx_v_self->allowed_types == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+      __PYX_ERR(0, 52, __pyx_L1_error)
     }
-    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_t_9) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_9);
-    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 75, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 75, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v_self->allowed_types, __pyx_v_x, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_8 = (__pyx_v_self->actual_type == ((PyTypeObject*)__pyx_t_1));
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_9 = (__pyx_t_8 != 0);
+    if (__pyx_t_9) {
 
-    /* "tenforce/enforcer.pyx":74
- * 
- *     # if we couldn't cast obj
- *     if type(obj) is not annotation:             # <<<<<<<<<<<<<<
- *         raise AutoCastError(f"{obj} failed to cast to {annotation}")
+      /* "tenforce/lib/members.pyx":53
+ *         for x in range(len(self.allowed_types)):
+ *             if self.actual_type is self.allowed_types[x]:
+ *                 match_found = True             # <<<<<<<<<<<<<<
+ *                 break
  * 
  */
-  }
+      __pyx_v_match_found = 1;
 
-  /* "tenforce/enforcer.pyx":77
- *         raise AutoCastError(f"{obj} failed to cast to {annotation}")
- * 
- *     return obj             # <<<<<<<<<<<<<<
+      /* "tenforce/lib/members.pyx":54
+ *             if self.actual_type is self.allowed_types[x]:
+ *                 match_found = True
+ *                 break             # <<<<<<<<<<<<<<
  * 
- * cpdef ParsedListMember _parse_generic_alias_member(str class_name, str member_name, object generic_alias, object obj, bint auto_cast = False):
+ *         # if there was no matching type found in the union, raise error
  */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_obj);
-  __pyx_r = __pyx_v_obj;
-  goto __pyx_L0;
+      goto __pyx_L4_break;
 
-  /* "tenforce/enforcer.pyx":57
- *                 )
- * 
- * cpdef object _auto_cast(object obj, type annotation):             # <<<<<<<<<<<<<<
- *     """
- *     Cast an object to its annotated type
+      /* "tenforce/lib/members.pyx":52
+ *         cdef bint match_found = False
+ *         for x in range(len(self.allowed_types)):
+ *             if self.actual_type is self.allowed_types[x]:             # <<<<<<<<<<<<<<
+ *                 match_found = True
+ *                 break
  */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_AddTraceback("tenforce.enforcer._auto_cast", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_obj);
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* Python wrapper */
-static PyObject *__pyx_pw_8tenforce_8enforcer_1_auto_cast(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8tenforce_8enforcer__auto_cast[] = "\n    Cast an object to its annotated type\n    :param obj: Object to cast\n    :param annotation: Type annotation\n    :raise AutoCastError: if it was impossible to cast obj to its type annotation\n    :return: Casted object\n    ";
-static PyObject *__pyx_pw_8tenforce_8enforcer_1_auto_cast(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  PyObject *__pyx_v_obj = 0;
-  PyTypeObject *__pyx_v_annotation = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("_auto_cast (wrapper)", 0);
-  {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_obj,&__pyx_n_s_annotation,0};
-    PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
-      Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
-        case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_obj)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_annotation)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("_auto_cast", 1, 2, 2, 1); __PYX_ERR(0, 57, __pyx_L3_error)
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_auto_cast") < 0)) __PYX_ERR(0, 57, __pyx_L3_error)
-      }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_obj = values[0];
-    __pyx_v_annotation = ((PyTypeObject*)values[1]);
   }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_auto_cast", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 57, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("tenforce.enforcer._auto_cast", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_annotation), (&PyType_Type), 1, "annotation", 1))) __PYX_ERR(0, 57, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8tenforce_8enforcer__auto_cast(__pyx_self, __pyx_v_obj, __pyx_v_annotation);
+  __pyx_L4_break:;
 
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_8tenforce_8enforcer__auto_cast(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_obj, PyTypeObject *__pyx_v_annotation) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_auto_cast", 0);
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8tenforce_8enforcer__auto_cast(__pyx_v_obj, __pyx_v_annotation, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("tenforce.enforcer._auto_cast", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "tenforce/enforcer.pyx":79
- *     return obj
- * 
- * cpdef ParsedListMember _parse_generic_alias_member(str class_name, str member_name, object generic_alias, object obj, bint auto_cast = False):             # <<<<<<<<<<<<<<
- *     """
- *     Parses a member of a class that has a GenericAlias type annotation (ex: list[str])
- */
-
-static PyObject *__pyx_pw_8tenforce_8enforcer_3_parse_generic_alias_member(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *__pyx_f_8tenforce_8enforcer__parse_generic_alias_member(PyObject *__pyx_v_class_name, PyObject *__pyx_v_member_name, PyObject *__pyx_v_generic_alias, PyObject *__pyx_v_obj, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_8tenforce_8enforcer__parse_generic_alias_member *__pyx_optional_args) {
-  int __pyx_v_auto_cast = ((int)0);
-  PyTypeObject *__pyx_v_origin = 0;
-  PyTypeObject *__pyx_v_annotation = 0;
-  int __pyx_v_x;
-  struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *__pyx_v_plm = 0;
-  struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  int __pyx_t_5;
-  Py_ssize_t __pyx_t_6;
-  Py_UCS4 __pyx_t_7;
-  Py_ssize_t __pyx_t_8;
-  int __pyx_t_9;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_parse_generic_alias_member", 0);
-  if (__pyx_optional_args) {
-    if (__pyx_optional_args->__pyx_n > 0) {
-      __pyx_v_auto_cast = __pyx_optional_args->auto_cast;
-    }
-  }
-
-  /* "tenforce/enforcer.pyx":90
- *     """
- *     # get what kind of generic alias this is
- *     cpdef type origin = typing.get_origin(generic_alias)             # <<<<<<<<<<<<<<
- *     if origin is not list:
- *         raise ValueError(f"Unsupported Generic Alias origin type '{origin}'")
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_typing); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get_origin); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_2);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_v_generic_alias) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_generic_alias);
-  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(PyType_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "type", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 90, __pyx_L1_error)
-  __pyx_v_origin = ((PyTypeObject*)__pyx_t_1);
-  __pyx_t_1 = 0;
-
-  /* "tenforce/enforcer.pyx":91
- *     # get what kind of generic alias this is
- *     cpdef type origin = typing.get_origin(generic_alias)
- *     if origin is not list:             # <<<<<<<<<<<<<<
- *         raise ValueError(f"Unsupported Generic Alias origin type '{origin}'")
+  /* "tenforce/lib/members.pyx":57
  * 
+ *         # if there was no matching type found in the union, raise error
+ *         if not match_found:             # <<<<<<<<<<<<<<
+ *             raise TypeEnforcementError(
+ *                 class_name=self.class_name,
  */
-  __pyx_t_4 = (__pyx_v_origin != (&PyList_Type));
-  __pyx_t_5 = (__pyx_t_4 != 0);
-  if (unlikely(__pyx_t_5)) {
+  __pyx_t_9 = ((!(__pyx_v_match_found != 0)) != 0);
+  if (unlikely(__pyx_t_9)) {
 
-    /* "tenforce/enforcer.pyx":92
- *     cpdef type origin = typing.get_origin(generic_alias)
- *     if origin is not list:
- *         raise ValueError(f"Unsupported Generic Alias origin type '{origin}'")             # <<<<<<<<<<<<<<
- * 
- *     # get out base annotation arg (ex: list[ -> str <- ])
+    /* "tenforce/lib/members.pyx":58
+ *         # if there was no matching type found in the union, raise error
+ *         if not match_found:
+ *             raise TypeEnforcementError(             # <<<<<<<<<<<<<<
+ *                 class_name=self.class_name,
+ *                 var_name=self.member_name,
  */
-    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = 0;
-    __pyx_t_7 = 127;
-    __Pyx_INCREF(__pyx_kp_u_Unsupported_Generic_Alias_origin);
-    __pyx_t_6 += 39;
-    __Pyx_GIVEREF(__pyx_kp_u_Unsupported_Generic_Alias_origin);
-    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Unsupported_Generic_Alias_origin);
-    __pyx_t_3 = __Pyx_PyObject_FormatSimple(((PyObject *)__pyx_v_origin), __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) : __pyx_t_7;
-    __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
-    __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_3);
-    __pyx_t_3 = 0;
-    __Pyx_INCREF(__pyx_kp_u__3);
-    __pyx_t_6 += 1;
-    __Pyx_GIVEREF(__pyx_kp_u__3);
-    PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u__3);
-    __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_TypeEnforcementError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_Raise(__pyx_t_1, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 92, __pyx_L1_error)
 
-    /* "tenforce/enforcer.pyx":91
- *     # get what kind of generic alias this is
- *     cpdef type origin = typing.get_origin(generic_alias)
- *     if origin is not list:             # <<<<<<<<<<<<<<
- *         raise ValueError(f"Unsupported Generic Alias origin type '{origin}'")
- * 
- */
-  }
-
-  /* "tenforce/enforcer.pyx":95
- * 
- *     # get out base annotation arg (ex: list[ -> str <- ])
- *     cdef type annotation = typing.get_args(generic_alias)[0]             # <<<<<<<<<<<<<<
- * 
- *     # if auto cast is true, auto cast the value
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_typing); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get_args); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_generic_alias) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_generic_alias);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(PyType_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "type", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(0, 95, __pyx_L1_error)
-  __pyx_v_annotation = ((PyTypeObject*)__pyx_t_2);
-  __pyx_t_2 = 0;
-
-  /* "tenforce/enforcer.pyx":99
- *     # if auto cast is true, auto cast the value
- *     cdef int x
- *     if auto_cast is True:             # <<<<<<<<<<<<<<
- *         for x in range(len(obj)):
- *             obj[x] = _auto_cast(obj[x], annotation)
- */
-  __pyx_t_5 = ((__pyx_v_auto_cast == 1) != 0);
-  if (__pyx_t_5) {
-
-    /* "tenforce/enforcer.pyx":100
- *     cdef int x
- *     if auto_cast is True:
- *         for x in range(len(obj)):             # <<<<<<<<<<<<<<
- *             obj[x] = _auto_cast(obj[x], annotation)
- * 
- */
-    __pyx_t_6 = PyObject_Length(__pyx_v_obj); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 100, __pyx_L1_error)
-    __pyx_t_8 = __pyx_t_6;
-    for (__pyx_t_9 = 0; __pyx_t_9 < __pyx_t_8; __pyx_t_9+=1) {
-      __pyx_v_x = __pyx_t_9;
-
-      /* "tenforce/enforcer.pyx":101
- *     if auto_cast is True:
- *         for x in range(len(obj)):
- *             obj[x] = _auto_cast(obj[x], annotation)             # <<<<<<<<<<<<<<
- * 
- *     # create a parsed list member
+    /* "tenforce/lib/members.pyx":59
+ *         if not match_found:
+ *             raise TypeEnforcementError(
+ *                 class_name=self.class_name,             # <<<<<<<<<<<<<<
+ *                 var_name=self.member_name,
+ *                 requested_types=self.allowed_types,
  */
-      __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_obj, __pyx_v_x, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_1 = __pyx_f_8tenforce_8enforcer__auto_cast(__pyx_t_2, __pyx_v_annotation, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(__Pyx_SetItemInt(__pyx_v_obj, __pyx_v_x, __pyx_t_1, int, 1, __Pyx_PyInt_From_int, 0, 1, 1) < 0)) __PYX_ERR(0, 101, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    }
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 59, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_class_name, __pyx_v_self->class_name) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
 
-    /* "tenforce/enforcer.pyx":99
- *     # if auto cast is true, auto cast the value
- *     cdef int x
- *     if auto_cast is True:             # <<<<<<<<<<<<<<
- *         for x in range(len(obj)):
- *             obj[x] = _auto_cast(obj[x], annotation)
+    /* "tenforce/lib/members.pyx":60
+ *             raise TypeEnforcementError(
+ *                 class_name=self.class_name,
+ *                 var_name=self.member_name,             # <<<<<<<<<<<<<<
+ *                 requested_types=self.allowed_types,
+ *                 actual_type=self.actual_type,
  */
-  }
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_var_name, __pyx_v_self->member_name) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
 
-  /* "tenforce/enforcer.pyx":104
- * 
- *     # create a parsed list member
- *     cdef ParsedListMember plm = ParsedListMember()             # <<<<<<<<<<<<<<
- *     plm.class_name = class_name
- *     plm.member_name = member_name
+    /* "tenforce/lib/members.pyx":61
+ *                 class_name=self.class_name,
+ *                 var_name=self.member_name,
+ *                 requested_types=self.allowed_types,             # <<<<<<<<<<<<<<
+ *                 actual_type=self.actual_type,
+ *                 obj=self.obj
  */
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8tenforce_8enforcer_ParsedListMember)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_v_plm = ((struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *)__pyx_t_1);
-  __pyx_t_1 = 0;
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_requested_types, __pyx_v_self->allowed_types) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
 
-  /* "tenforce/enforcer.pyx":105
- *     # create a parsed list member
- *     cdef ParsedListMember plm = ParsedListMember()
- *     plm.class_name = class_name             # <<<<<<<<<<<<<<
- *     plm.member_name = member_name
- *     plm.list_ = obj
- */
-  __Pyx_INCREF(__pyx_v_class_name);
-  __Pyx_GIVEREF(__pyx_v_class_name);
-  __Pyx_GOTREF(__pyx_v_plm->class_name);
-  __Pyx_DECREF(__pyx_v_plm->class_name);
-  __pyx_v_plm->class_name = __pyx_v_class_name;
-
-  /* "tenforce/enforcer.pyx":106
- *     cdef ParsedListMember plm = ParsedListMember()
- *     plm.class_name = class_name
- *     plm.member_name = member_name             # <<<<<<<<<<<<<<
- *     plm.list_ = obj
- *     plm.base_annotated_type = annotation
- */
-  __Pyx_INCREF(__pyx_v_member_name);
-  __Pyx_GIVEREF(__pyx_v_member_name);
-  __Pyx_GOTREF(__pyx_v_plm->member_name);
-  __Pyx_DECREF(__pyx_v_plm->member_name);
-  __pyx_v_plm->member_name = __pyx_v_member_name;
-
-  /* "tenforce/enforcer.pyx":107
- *     plm.class_name = class_name
- *     plm.member_name = member_name
- *     plm.list_ = obj             # <<<<<<<<<<<<<<
- *     plm.base_annotated_type = annotation
- * 
+    /* "tenforce/lib/members.pyx":62
+ *                 var_name=self.member_name,
+ *                 requested_types=self.allowed_types,
+ *                 actual_type=self.actual_type,             # <<<<<<<<<<<<<<
+ *                 obj=self.obj
+ *             )
  */
-  if (!(likely(PyList_CheckExact(__pyx_v_obj))||((__pyx_v_obj) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_v_obj)->tp_name), 0))) __PYX_ERR(0, 107, __pyx_L1_error)
-  __pyx_t_1 = __pyx_v_obj;
-  __Pyx_INCREF(__pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_1);
-  __Pyx_GOTREF(__pyx_v_plm->list_);
-  __Pyx_DECREF(__pyx_v_plm->list_);
-  __pyx_v_plm->list_ = ((PyObject*)__pyx_t_1);
-  __pyx_t_1 = 0;
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_actual_type, ((PyObject *)__pyx_v_self->actual_type)) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
 
-  /* "tenforce/enforcer.pyx":108
- *     plm.member_name = member_name
- *     plm.list_ = obj
- *     plm.base_annotated_type = annotation             # <<<<<<<<<<<<<<
- * 
- *     # run the enforce now, we want to not bother enforcing more if we have a validation error
+    /* "tenforce/lib/members.pyx":63
+ *                 requested_types=self.allowed_types,
+ *                 actual_type=self.actual_type,
+ *                 obj=self.obj             # <<<<<<<<<<<<<<
+ *             )
  */
-  __Pyx_INCREF(((PyObject *)__pyx_v_annotation));
-  __Pyx_GIVEREF(((PyObject *)__pyx_v_annotation));
-  __Pyx_GOTREF(__pyx_v_plm->base_annotated_type);
-  __Pyx_DECREF(((PyObject *)__pyx_v_plm->base_annotated_type));
-  __pyx_v_plm->base_annotated_type = __pyx_v_annotation;
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_obj, __pyx_v_self->obj) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
 
-  /* "tenforce/enforcer.pyx":111
- * 
- *     # run the enforce now, we want to not bother enforcing more if we have a validation error
- *     plm.enforce()             # <<<<<<<<<<<<<<
- *     return plm
- * 
+    /* "tenforce/lib/members.pyx":58
+ *         # if there was no matching type found in the union, raise error
+ *         if not match_found:
+ *             raise TypeEnforcementError(             # <<<<<<<<<<<<<<
+ *                 class_name=self.class_name,
+ *                 var_name=self.member_name,
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_8tenforce_8enforcer_ParsedListMember *)__pyx_v_plm->__pyx_vtab)->enforce(__pyx_v_plm, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 58, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __PYX_ERR(0, 58, __pyx_L1_error)
 
-  /* "tenforce/enforcer.pyx":112
- *     # run the enforce now, we want to not bother enforcing more if we have a validation error
- *     plm.enforce()
- *     return plm             # <<<<<<<<<<<<<<
+    /* "tenforce/lib/members.pyx":57
  * 
- * cpdef ParsedMember _parse_member(str class_name, str member_name, type annotation, object obj, bint auto_cast = False):
+ *         # if there was no matching type found in the union, raise error
+ *         if not match_found:             # <<<<<<<<<<<<<<
+ *             raise TypeEnforcementError(
+ *                 class_name=self.class_name,
  */
-  __Pyx_XDECREF(((PyObject *)__pyx_r));
-  __Pyx_INCREF(((PyObject *)__pyx_v_plm));
-  __pyx_r = __pyx_v_plm;
-  goto __pyx_L0;
+  }
 
-  /* "tenforce/enforcer.pyx":79
- *     return obj
+  /* "tenforce/lib/members.pyx":42
  * 
- * cpdef ParsedListMember _parse_generic_alias_member(str class_name, str member_name, object generic_alias, object obj, bint auto_cast = False):             # <<<<<<<<<<<<<<
- *     """
- *     Parses a member of a class that has a GenericAlias type annotation (ex: list[str])
+ * cdef class ParsedUnionMember:
+ *     cpdef enforce(self):             # <<<<<<<<<<<<<<
+ *         """
+ *         Enforces the type for this ParsedMember
  */
 
   /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("tenforce.enforcer._parse_generic_alias_member", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("tenforce.lib.members.ParsedUnionMember.enforce", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_origin);
-  __Pyx_XDECREF(__pyx_v_annotation);
-  __Pyx_XDECREF((PyObject *)__pyx_v_plm);
-  __Pyx_XGIVEREF((PyObject *)__pyx_r);
+  __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8tenforce_8enforcer_3_parse_generic_alias_member(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8tenforce_8enforcer_2_parse_generic_alias_member[] = "\n    Parses a member of a class that has a GenericAlias type annotation (ex: list[str])\n    :param class_name: \n    :param member_name: \n    :param obj: \n    :param generic_alias: GenericAlias instance\n    :param auto_cast: \n    :return: ParsedListMember\n    ";
-static PyObject *__pyx_pw_8tenforce_8enforcer_3_parse_generic_alias_member(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  PyObject *__pyx_v_class_name = 0;
-  PyObject *__pyx_v_member_name = 0;
-  PyObject *__pyx_v_generic_alias = 0;
-  PyObject *__pyx_v_obj = 0;
-  int __pyx_v_auto_cast;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
+static PyObject *__pyx_pw_8tenforce_3lib_7members_17ParsedUnionMember_1enforce(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_8tenforce_3lib_7members_17ParsedUnionMember_enforce[] = "\n        Enforces the type for this ParsedMember\n        :raises TypeEnforcementError: if there is a mismatched type\n        :return: None\n        ";
+static PyObject *__pyx_pw_8tenforce_3lib_7members_17ParsedUnionMember_1enforce(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("_parse_generic_alias_member (wrapper)", 0);
-  {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_class_name,&__pyx_n_s_member_name,&__pyx_n_s_generic_alias,&__pyx_n_s_obj,&__pyx_n_s_auto_cast,0};
-    PyObject* values[5] = {0,0,0,0,0};
-    if (unlikely(__pyx_kwds)) {
-      Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
-        CYTHON_FALLTHROUGH;
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-        CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
-        case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_class_name)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_member_name)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("_parse_generic_alias_member", 0, 4, 5, 1); __PYX_ERR(0, 79, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_generic_alias)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("_parse_generic_alias_member", 0, 4, 5, 2); __PYX_ERR(0, 79, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  3:
-        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_obj)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("_parse_generic_alias_member", 0, 4, 5, 3); __PYX_ERR(0, 79, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  4:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_auto_cast);
-          if (value) { values[4] = value; kw_args--; }
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_parse_generic_alias_member") < 0)) __PYX_ERR(0, 79, __pyx_L3_error)
-      }
-    } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
-        CYTHON_FALLTHROUGH;
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-        values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-    }
-    __pyx_v_class_name = ((PyObject*)values[0]);
-    __pyx_v_member_name = ((PyObject*)values[1]);
-    __pyx_v_generic_alias = values[2];
-    __pyx_v_obj = values[3];
-    if (values[4]) {
-      __pyx_v_auto_cast = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_auto_cast == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 79, __pyx_L3_error)
-    } else {
-      __pyx_v_auto_cast = ((int)0);
-    }
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_parse_generic_alias_member", 0, 4, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 79, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("tenforce.enforcer._parse_generic_alias_member", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_class_name), (&PyUnicode_Type), 1, "class_name", 1))) __PYX_ERR(0, 79, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_member_name), (&PyUnicode_Type), 1, "member_name", 1))) __PYX_ERR(0, 79, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8tenforce_8enforcer_2_parse_generic_alias_member(__pyx_self, __pyx_v_class_name, __pyx_v_member_name, __pyx_v_generic_alias, __pyx_v_obj, __pyx_v_auto_cast);
+  __Pyx_RefNannySetupContext("enforce (wrapper)", 0);
+  __pyx_r = __pyx_pf_8tenforce_3lib_7members_17ParsedUnionMember_enforce(((struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *)__pyx_v_self));
 
   /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8tenforce_8enforcer_2_parse_generic_alias_member(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_class_name, PyObject *__pyx_v_member_name, PyObject *__pyx_v_generic_alias, PyObject *__pyx_v_obj, int __pyx_v_auto_cast) {
+static PyObject *__pyx_pf_8tenforce_3lib_7members_17ParsedUnionMember_enforce(struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  struct __pyx_opt_args_8tenforce_8enforcer__parse_generic_alias_member __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_parse_generic_alias_member", 0);
+  __Pyx_RefNannySetupContext("enforce", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2.__pyx_n = 1;
-  __pyx_t_2.auto_cast = __pyx_v_auto_cast;
-  __pyx_t_1 = ((PyObject *)__pyx_f_8tenforce_8enforcer__parse_generic_alias_member(__pyx_v_class_name, __pyx_v_member_name, __pyx_v_generic_alias, __pyx_v_obj, 0, &__pyx_t_2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8tenforce_3lib_7members_17ParsedUnionMember_enforce(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("tenforce.enforcer._parse_generic_alias_member", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("tenforce.lib.members.ParsedUnionMember.enforce", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "tenforce/enforcer.pyx":114
- *     return plm
- * 
- * cpdef ParsedMember _parse_member(str class_name, str member_name, type annotation, object obj, bint auto_cast = False):             # <<<<<<<<<<<<<<
- *     """
- *     Parses a standard member of a class
- */
-
-static PyObject *__pyx_pw_8tenforce_8enforcer_5_parse_member(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static struct __pyx_obj_8tenforce_8enforcer_ParsedMember *__pyx_f_8tenforce_8enforcer__parse_member(PyObject *__pyx_v_class_name, PyObject *__pyx_v_member_name, PyTypeObject *__pyx_v_annotation, PyObject *__pyx_v_obj, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_8tenforce_8enforcer__parse_member *__pyx_optional_args) {
-  int __pyx_v_auto_cast = ((int)0);
-  struct __pyx_obj_8tenforce_8enforcer_ParsedMember *__pyx_v_parsed_member = 0;
-  struct __pyx_obj_8tenforce_8enforcer_ParsedMember *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_parse_member", 0);
-  if (__pyx_optional_args) {
-    if (__pyx_optional_args->__pyx_n > 0) {
-      __pyx_v_auto_cast = __pyx_optional_args->auto_cast;
-    }
-  }
-  __Pyx_INCREF(__pyx_v_obj);
-
-  /* "tenforce/enforcer.pyx":125
- *     """
- *     # if auto cast is true, auto cast the value
- *     if auto_cast is True:             # <<<<<<<<<<<<<<
- *         obj = _auto_cast(obj, annotation)
- * 
- */
-  __pyx_t_1 = ((__pyx_v_auto_cast == 1) != 0);
-  if (__pyx_t_1) {
-
-    /* "tenforce/enforcer.pyx":126
- *     # if auto cast is true, auto cast the value
- *     if auto_cast is True:
- *         obj = _auto_cast(obj, annotation)             # <<<<<<<<<<<<<<
- * 
- *     # create a ParsedMember
- */
-    __pyx_t_2 = __pyx_f_8tenforce_8enforcer__auto_cast(__pyx_v_obj, __pyx_v_annotation, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF_SET(__pyx_v_obj, __pyx_t_2);
-    __pyx_t_2 = 0;
-
-    /* "tenforce/enforcer.pyx":125
- *     """
- *     # if auto cast is true, auto cast the value
- *     if auto_cast is True:             # <<<<<<<<<<<<<<
- *         obj = _auto_cast(obj, annotation)
- * 
- */
-  }
-
-  /* "tenforce/enforcer.pyx":129
- * 
- *     # create a ParsedMember
- *     cpdef ParsedMember parsed_member = ParsedMember()             # <<<<<<<<<<<<<<
- *     parsed_member.annotated_type = annotation
- *     parsed_member.actual_type = type(obj)
- */
-  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8tenforce_8enforcer_ParsedMember)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 129, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_v_parsed_member = ((struct __pyx_obj_8tenforce_8enforcer_ParsedMember *)__pyx_t_2);
-  __pyx_t_2 = 0;
-
-  /* "tenforce/enforcer.pyx":130
- *     # create a ParsedMember
- *     cpdef ParsedMember parsed_member = ParsedMember()
- *     parsed_member.annotated_type = annotation             # <<<<<<<<<<<<<<
- *     parsed_member.actual_type = type(obj)
- *     parsed_member.obj = obj
- */
-  __Pyx_INCREF(((PyObject *)__pyx_v_annotation));
-  __Pyx_GIVEREF(((PyObject *)__pyx_v_annotation));
-  __Pyx_GOTREF(__pyx_v_parsed_member->annotated_type);
-  __Pyx_DECREF(((PyObject *)__pyx_v_parsed_member->annotated_type));
-  __pyx_v_parsed_member->annotated_type = __pyx_v_annotation;
-
-  /* "tenforce/enforcer.pyx":131
- *     cpdef ParsedMember parsed_member = ParsedMember()
- *     parsed_member.annotated_type = annotation
- *     parsed_member.actual_type = type(obj)             # <<<<<<<<<<<<<<
- *     parsed_member.obj = obj
- *     parsed_member.member_name = member_name
- */
-  __Pyx_INCREF(((PyObject *)Py_TYPE(__pyx_v_obj)));
-  __Pyx_GIVEREF(((PyObject *)Py_TYPE(__pyx_v_obj)));
-  __Pyx_GOTREF(__pyx_v_parsed_member->actual_type);
-  __Pyx_DECREF(((PyObject *)__pyx_v_parsed_member->actual_type));
-  __pyx_v_parsed_member->actual_type = ((PyTypeObject*)((PyObject *)Py_TYPE(__pyx_v_obj)));
-
-  /* "tenforce/enforcer.pyx":132
- *     parsed_member.annotated_type = annotation
- *     parsed_member.actual_type = type(obj)
- *     parsed_member.obj = obj             # <<<<<<<<<<<<<<
- *     parsed_member.member_name = member_name
- *     parsed_member.class_name = class_name
- */
-  __Pyx_INCREF(__pyx_v_obj);
-  __Pyx_GIVEREF(__pyx_v_obj);
-  __Pyx_GOTREF(__pyx_v_parsed_member->obj);
-  __Pyx_DECREF(__pyx_v_parsed_member->obj);
-  __pyx_v_parsed_member->obj = __pyx_v_obj;
-
-  /* "tenforce/enforcer.pyx":133
- *     parsed_member.actual_type = type(obj)
- *     parsed_member.obj = obj
- *     parsed_member.member_name = member_name             # <<<<<<<<<<<<<<
- *     parsed_member.class_name = class_name
- * 
- */
-  __Pyx_INCREF(__pyx_v_member_name);
-  __Pyx_GIVEREF(__pyx_v_member_name);
-  __Pyx_GOTREF(__pyx_v_parsed_member->member_name);
-  __Pyx_DECREF(__pyx_v_parsed_member->member_name);
-  __pyx_v_parsed_member->member_name = __pyx_v_member_name;
-
-  /* "tenforce/enforcer.pyx":134
- *     parsed_member.obj = obj
- *     parsed_member.member_name = member_name
- *     parsed_member.class_name = class_name             # <<<<<<<<<<<<<<
- * 
- *     # run the enforce now, we want to not bother enforcing more if we have a validation error
- */
-  __Pyx_INCREF(__pyx_v_class_name);
-  __Pyx_GIVEREF(__pyx_v_class_name);
-  __Pyx_GOTREF(__pyx_v_parsed_member->class_name);
-  __Pyx_DECREF(__pyx_v_parsed_member->class_name);
-  __pyx_v_parsed_member->class_name = __pyx_v_class_name;
-
-  /* "tenforce/enforcer.pyx":138
- *     # run the enforce now, we want to not bother enforcing more if we have a validation error
- * 
- *     parsed_member.enforce()             # <<<<<<<<<<<<<<
- *     return parsed_member
- * 
- */
-  __pyx_t_2 = ((struct __pyx_vtabstruct_8tenforce_8enforcer_ParsedMember *)__pyx_v_parsed_member->__pyx_vtab)->enforce(__pyx_v_parsed_member, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "tenforce/enforcer.pyx":139
- * 
- *     parsed_member.enforce()
- *     return parsed_member             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __Pyx_XDECREF(((PyObject *)__pyx_r));
-  __Pyx_INCREF(((PyObject *)__pyx_v_parsed_member));
-  __pyx_r = __pyx_v_parsed_member;
-  goto __pyx_L0;
-
-  /* "tenforce/enforcer.pyx":114
- *     return plm
- * 
- * cpdef ParsedMember _parse_member(str class_name, str member_name, type annotation, object obj, bint auto_cast = False):             # <<<<<<<<<<<<<<
- *     """
- *     Parses a standard member of a class
+/* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     cdef tuple state
+ *     cdef object _dict
  */
 
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("tenforce.enforcer._parse_member", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_parsed_member);
-  __Pyx_XDECREF(__pyx_v_obj);
-  __Pyx_XGIVEREF((PyObject *)__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
 /* Python wrapper */
-static PyObject *__pyx_pw_8tenforce_8enforcer_5_parse_member(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8tenforce_8enforcer_4_parse_member[] = "\n    Parses a standard member of a class\n    :param class_name: Class name\n    :param member_name: Member name\n    :param obj: Object to parse\n    :param annotation: Type annotation of obj\n    :param auto_cast: Automatically cast compatible types\n    :return: ParsedMember object\n    ";
-static PyObject *__pyx_pw_8tenforce_8enforcer_5_parse_member(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  PyObject *__pyx_v_class_name = 0;
-  PyObject *__pyx_v_member_name = 0;
-  PyTypeObject *__pyx_v_annotation = 0;
-  PyObject *__pyx_v_obj = 0;
-  int __pyx_v_auto_cast;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
+static PyObject *__pyx_pw_8tenforce_3lib_7members_17ParsedUnionMember_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_8tenforce_3lib_7members_17ParsedUnionMember_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("_parse_member (wrapper)", 0);
-  {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_class_name,&__pyx_n_s_member_name,&__pyx_n_s_annotation,&__pyx_n_s_obj,&__pyx_n_s_auto_cast,0};
-    PyObject* values[5] = {0,0,0,0,0};
-    if (unlikely(__pyx_kwds)) {
-      Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
-        CYTHON_FALLTHROUGH;
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-        CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
-        case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_class_name)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_member_name)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("_parse_member", 0, 4, 5, 1); __PYX_ERR(0, 114, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_annotation)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("_parse_member", 0, 4, 5, 2); __PYX_ERR(0, 114, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  3:
-        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_obj)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("_parse_member", 0, 4, 5, 3); __PYX_ERR(0, 114, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  4:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_auto_cast);
-          if (value) { values[4] = value; kw_args--; }
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_parse_member") < 0)) __PYX_ERR(0, 114, __pyx_L3_error)
-      }
-    } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
-        CYTHON_FALLTHROUGH;
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-        values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-    }
-    __pyx_v_class_name = ((PyObject*)values[0]);
-    __pyx_v_member_name = ((PyObject*)values[1]);
-    __pyx_v_annotation = ((PyTypeObject*)values[2]);
-    __pyx_v_obj = values[3];
-    if (values[4]) {
-      __pyx_v_auto_cast = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_auto_cast == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 114, __pyx_L3_error)
-    } else {
-      __pyx_v_auto_cast = ((int)0);
-    }
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_parse_member", 0, 4, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 114, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("tenforce.enforcer._parse_member", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_class_name), (&PyUnicode_Type), 1, "class_name", 1))) __PYX_ERR(0, 114, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_member_name), (&PyUnicode_Type), 1, "member_name", 1))) __PYX_ERR(0, 114, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_annotation), (&PyType_Type), 1, "annotation", 1))) __PYX_ERR(0, 114, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8tenforce_8enforcer_4_parse_member(__pyx_self, __pyx_v_class_name, __pyx_v_member_name, __pyx_v_annotation, __pyx_v_obj, __pyx_v_auto_cast);
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_8tenforce_8enforcer_4_parse_member(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_class_name, PyObject *__pyx_v_member_name, PyTypeObject *__pyx_v_annotation, PyObject *__pyx_v_obj, int __pyx_v_auto_cast) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  struct __pyx_opt_args_8tenforce_8enforcer__parse_member __pyx_t_2;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_parse_member", 0);
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2.__pyx_n = 1;
-  __pyx_t_2.auto_cast = __pyx_v_auto_cast;
-  __pyx_t_1 = ((PyObject *)__pyx_f_8tenforce_8enforcer__parse_member(__pyx_v_class_name, __pyx_v_member_name, __pyx_v_annotation, __pyx_v_obj, 0, &__pyx_t_2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 114, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
+  __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_8tenforce_3lib_7members_17ParsedUnionMember_2__reduce_cython__(((struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *)__pyx_v_self));
 
   /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("tenforce.enforcer._parse_member", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "tenforce/enforcer.pyx":142
- * 
- * 
- * cpdef check(object obj, bint auto_cast = False):             # <<<<<<<<<<<<<<
- *     """
- *     Checks the class variables of an object & enforces its type hints
- */
-
-static PyObject *__pyx_pw_8tenforce_8enforcer_7check(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_f_8tenforce_8enforcer_check(PyObject *__pyx_v_obj, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_8tenforce_8enforcer_check *__pyx_optional_args) {
-  int __pyx_v_auto_cast = ((int)0);
-  PyObject *__pyx_v_class_name = 0;
-  PyObject *__pyx_v_annotations = 0;
-  PyObject *__pyx_v_values = 0;
-  PyObject *__pyx_v_parsed_members = 0;
-  struct __pyx_obj_8tenforce_8enforcer_ParsedMember *__pyx_v_parsed_member = 0;
-  CYTHON_UNUSED PyObject *__pyx_v_parsed_generic_alias_member = 0;
-  PyObject *__pyx_v_member_name = 0;
-  CYTHON_UNUSED struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *__pyx_v_plm = NULL;
+static PyObject *__pyx_pf_8tenforce_3lib_7members_17ParsedUnionMember_2__reduce_cython__(struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *__pyx_v_self) {
+  PyObject *__pyx_v_state = 0;
+  PyObject *__pyx_v__dict = 0;
+  int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  Py_ssize_t __pyx_t_3;
-  Py_ssize_t __pyx_t_4;
+  int __pyx_t_2;
+  int __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
-  int __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
-  int __pyx_t_8;
-  int __pyx_t_9;
-  PyObject *__pyx_t_10 = NULL;
-  struct __pyx_opt_args_8tenforce_8enforcer__parse_generic_alias_member __pyx_t_11;
-  struct __pyx_opt_args_8tenforce_8enforcer__parse_member __pyx_t_12;
-  int __pyx_t_13;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("check", 0);
-  if (__pyx_optional_args) {
-    if (__pyx_optional_args->__pyx_n > 0) {
-      __pyx_v_auto_cast = __pyx_optional_args->auto_cast;
-    }
-  }
+  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
-  /* "tenforce/enforcer.pyx":151
- * 
- *     # define the annotations and values
- *     cdef str class_name = obj.__class__.__name__             # <<<<<<<<<<<<<<
- *     cdef dict annotations = obj.__annotations__
- *     cdef dict values = obj.__dict__
+  /* "(tree fragment)":5
+ *     cdef object _dict
+ *     cdef bint use_setstate
+ *     state = (self.actual_type, self.allowed_types, self.class_name, self.member_name, self.obj)             # <<<<<<<<<<<<<<
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_obj, __pyx_n_s_class); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 151, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 151, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(0, 151, __pyx_L1_error)
-  __pyx_v_class_name = ((PyObject*)__pyx_t_2);
-  __pyx_t_2 = 0;
-
-  /* "tenforce/enforcer.pyx":152
- *     # define the annotations and values
- *     cdef str class_name = obj.__class__.__name__
- *     cdef dict annotations = obj.__annotations__             # <<<<<<<<<<<<<<
- *     cdef dict values = obj.__dict__
- * 
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_obj, __pyx_n_s_annotations); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (!(likely(PyDict_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(0, 152, __pyx_L1_error)
-  __pyx_v_annotations = ((PyObject*)__pyx_t_2);
-  __pyx_t_2 = 0;
-
-  /* "tenforce/enforcer.pyx":153
- *     cdef str class_name = obj.__class__.__name__
- *     cdef dict annotations = obj.__annotations__
- *     cdef dict values = obj.__dict__             # <<<<<<<<<<<<<<
- * 
- *     # create the ParsedMember instance and a list to hold them
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_obj, __pyx_n_s_dict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (!(likely(PyDict_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(0, 153, __pyx_L1_error)
-  __pyx_v_values = ((PyObject*)__pyx_t_2);
-  __pyx_t_2 = 0;
-
-  /* "tenforce/enforcer.pyx":156
- * 
- *     # create the ParsedMember instance and a list to hold them
- *     cdef list parsed_members = []             # <<<<<<<<<<<<<<
- *     cdef ParsedMember parsed_member
- * 
- */
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_v_parsed_members = ((PyObject*)__pyx_t_2);
-  __pyx_t_2 = 0;
+  __Pyx_INCREF(((PyObject *)__pyx_v_self->actual_type));
+  __Pyx_GIVEREF(((PyObject *)__pyx_v_self->actual_type));
+  PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_v_self->actual_type));
+  __Pyx_INCREF(__pyx_v_self->allowed_types);
+  __Pyx_GIVEREF(__pyx_v_self->allowed_types);
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_self->allowed_types);
+  __Pyx_INCREF(__pyx_v_self->class_name);
+  __Pyx_GIVEREF(__pyx_v_self->class_name);
+  PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_v_self->class_name);
+  __Pyx_INCREF(__pyx_v_self->member_name);
+  __Pyx_GIVEREF(__pyx_v_self->member_name);
+  PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_v_self->member_name);
+  __Pyx_INCREF(__pyx_v_self->obj);
+  __Pyx_GIVEREF(__pyx_v_self->obj);
+  PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_v_self->obj);
+  __pyx_v_state = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
 
-  /* "tenforce/enforcer.pyx":159
- *     cdef ParsedMember parsed_member
- * 
- *     cdef list parsed_generic_alias_member = []             # <<<<<<<<<<<<<<
- *     cdef ParsedListMember parsed_list_member
- * 
+  /* "(tree fragment)":6
+ *     cdef bint use_setstate
+ *     state = (self.actual_type, self.allowed_types, self.class_name, self.member_name, self.obj)
+ *     _dict = getattr(self, '__dict__', None)             # <<<<<<<<<<<<<<
+ *     if _dict is not None:
+ *         state += (_dict,)
  */
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 159, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_v_parsed_generic_alias_member = ((PyObject*)__pyx_t_2);
-  __pyx_t_2 = 0;
-
-  /* "tenforce/enforcer.pyx":164
- *     # iterate over the annotations and create ParsedMember objects
- *     cdef str member_name
- *     for member_name in annotations.keys():             # <<<<<<<<<<<<<<
- *         if type(annotations[member_name]) is GenericAlias:
- *             plm = _parse_generic_alias_member(
- */
-  __pyx_t_3 = 0;
-  if (unlikely(__pyx_v_annotations == Py_None)) {
-    PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "keys");
-    __PYX_ERR(0, 164, __pyx_L1_error)
-  }
-  __pyx_t_1 = __Pyx_dict_iterator(__pyx_v_annotations, 1, __pyx_n_s_keys, (&__pyx_t_4), (&__pyx_t_5)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_s_dict, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __pyx_t_2 = __pyx_t_1;
+  __pyx_v__dict = __pyx_t_1;
   __pyx_t_1 = 0;
-  while (1) {
-    __pyx_t_6 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_4, &__pyx_t_3, &__pyx_t_1, NULL, NULL, __pyx_t_5);
-    if (unlikely(__pyx_t_6 == 0)) break;
-    if (unlikely(__pyx_t_6 == -1)) __PYX_ERR(0, 164, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 164, __pyx_L1_error)
-    __Pyx_XDECREF_SET(__pyx_v_member_name, ((PyObject*)__pyx_t_1));
-    __pyx_t_1 = 0;
 
-    /* "tenforce/enforcer.pyx":165
- *     cdef str member_name
- *     for member_name in annotations.keys():
- *         if type(annotations[member_name]) is GenericAlias:             # <<<<<<<<<<<<<<
- *             plm = _parse_generic_alias_member(
- *                 class_name=class_name,
+  /* "(tree fragment)":7
+ *     state = (self.actual_type, self.allowed_types, self.class_name, self.member_name, self.obj)
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:             # <<<<<<<<<<<<<<
+ *         state += (_dict,)
+ *         use_setstate = True
  */
-    if (unlikely(__pyx_v_annotations == Py_None)) {
-      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 165, __pyx_L1_error)
-    }
-    __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_annotations, __pyx_v_member_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __pyx_t_2 = (__pyx_v__dict != Py_None);
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
+
+    /* "(tree fragment)":8
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:
+ *         state += (_dict,)             # <<<<<<<<<<<<<<
+ *         use_setstate = True
+ *     else:
+ */
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 8, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_GenericAlias); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 165, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = (((PyObject *)Py_TYPE(__pyx_t_1)) == __pyx_t_7);
+    __Pyx_INCREF(__pyx_v__dict);
+    __Pyx_GIVEREF(__pyx_v__dict);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v__dict);
+    __pyx_t_4 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_9 = (__pyx_t_8 != 0);
-    if (__pyx_t_9) {
+    __Pyx_DECREF_SET(__pyx_v_state, ((PyObject*)__pyx_t_4));
+    __pyx_t_4 = 0;
 
-      /* "tenforce/enforcer.pyx":169
- *                 class_name=class_name,
- *                 member_name=member_name,
- *                 generic_alias=annotations[member_name],             # <<<<<<<<<<<<<<
- *                 obj=values.get(member_name),
- *                 auto_cast=auto_cast
+    /* "(tree fragment)":9
+ *     if _dict is not None:
+ *         state += (_dict,)
+ *         use_setstate = True             # <<<<<<<<<<<<<<
+ *     else:
+ *         use_setstate = self.actual_type is not None or self.allowed_types is not None or self.class_name is not None or self.member_name is not None or self.obj is not None
  */
-      if (unlikely(__pyx_v_annotations == Py_None)) {
-        PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 169, __pyx_L1_error)
-      }
-      __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_v_annotations, __pyx_v_member_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 169, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
+    __pyx_v_use_setstate = 1;
 
-      /* "tenforce/enforcer.pyx":170
- *                 member_name=member_name,
- *                 generic_alias=annotations[member_name],
- *                 obj=values.get(member_name),             # <<<<<<<<<<<<<<
- *                 auto_cast=auto_cast
- *             )
+    /* "(tree fragment)":7
+ *     state = (self.actual_type, self.allowed_types, self.class_name, self.member_name, self.obj)
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:             # <<<<<<<<<<<<<<
+ *         state += (_dict,)
+ *         use_setstate = True
  */
-      if (unlikely(__pyx_v_values == Py_None)) {
-        PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "get");
-        __PYX_ERR(0, 170, __pyx_L1_error)
-      }
-      __pyx_t_1 = __Pyx_PyDict_GetItemDefault(__pyx_v_values, __pyx_v_member_name, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 170, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-
-      /* "tenforce/enforcer.pyx":166
- *     for member_name in annotations.keys():
- *         if type(annotations[member_name]) is GenericAlias:
- *             plm = _parse_generic_alias_member(             # <<<<<<<<<<<<<<
- *                 class_name=class_name,
- *                 member_name=member_name,
- */
-      __pyx_t_11.__pyx_n = 1;
-      __pyx_t_11.auto_cast = __pyx_v_auto_cast;
-      __pyx_t_10 = ((PyObject *)__pyx_f_8tenforce_8enforcer__parse_generic_alias_member(__pyx_v_class_name, __pyx_v_member_name, __pyx_t_7, __pyx_t_1, 0, &__pyx_t_11)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 166, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_10);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_XDECREF_SET(__pyx_v_plm, ((struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *)__pyx_t_10));
-      __pyx_t_10 = 0;
+    goto __pyx_L3;
+  }
 
-      /* "tenforce/enforcer.pyx":165
- *     cdef str member_name
- *     for member_name in annotations.keys():
- *         if type(annotations[member_name]) is GenericAlias:             # <<<<<<<<<<<<<<
- *             plm = _parse_generic_alias_member(
- *                 class_name=class_name,
+  /* "(tree fragment)":11
+ *         use_setstate = True
+ *     else:
+ *         use_setstate = self.actual_type is not None or self.allowed_types is not None or self.class_name is not None or self.member_name is not None or self.obj is not None             # <<<<<<<<<<<<<<
+ *     if use_setstate:
+ *         return __pyx_unpickle_ParsedUnionMember, (type(self), 0x997196e, None), state
  */
-      goto __pyx_L5;
+  /*else*/ {
+    __pyx_t_2 = (__pyx_v_self->actual_type != ((PyTypeObject*)Py_None));
+    __pyx_t_5 = (__pyx_t_2 != 0);
+    if (!__pyx_t_5) {
+    } else {
+      __pyx_t_3 = __pyx_t_5;
+      goto __pyx_L4_bool_binop_done;
     }
+    __pyx_t_5 = (__pyx_v_self->allowed_types != ((PyObject*)Py_None));
+    __pyx_t_2 = (__pyx_t_5 != 0);
+    if (!__pyx_t_2) {
+    } else {
+      __pyx_t_3 = __pyx_t_2;
+      goto __pyx_L4_bool_binop_done;
+    }
+    __pyx_t_2 = (__pyx_v_self->class_name != ((PyObject*)Py_None));
+    __pyx_t_5 = (__pyx_t_2 != 0);
+    if (!__pyx_t_5) {
+    } else {
+      __pyx_t_3 = __pyx_t_5;
+      goto __pyx_L4_bool_binop_done;
+    }
+    __pyx_t_5 = (__pyx_v_self->member_name != ((PyObject*)Py_None));
+    __pyx_t_2 = (__pyx_t_5 != 0);
+    if (!__pyx_t_2) {
+    } else {
+      __pyx_t_3 = __pyx_t_2;
+      goto __pyx_L4_bool_binop_done;
+    }
+    __pyx_t_2 = (__pyx_v_self->obj != Py_None);
+    __pyx_t_5 = (__pyx_t_2 != 0);
+    __pyx_t_3 = __pyx_t_5;
+    __pyx_L4_bool_binop_done:;
+    __pyx_v_use_setstate = __pyx_t_3;
+  }
+  __pyx_L3:;
 
-    /* "tenforce/enforcer.pyx":174
- *             )
- *         else:
- *             parsed_member = _parse_member(             # <<<<<<<<<<<<<<
- *                 class_name=class_name,
- *                 member_name=member_name,
- */
-    /*else*/ {
-
-      /* "tenforce/enforcer.pyx":177
- *                 class_name=class_name,
- *                 member_name=member_name,
- *                 annotation=annotations[member_name],             # <<<<<<<<<<<<<<
- *                 obj=values.get(member_name),
- *                 auto_cast=auto_cast
+  /* "(tree fragment)":12
+ *     else:
+ *         use_setstate = self.actual_type is not None or self.allowed_types is not None or self.class_name is not None or self.member_name is not None or self.obj is not None
+ *     if use_setstate:             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_ParsedUnionMember, (type(self), 0x997196e, None), state
+ *     else:
  */
-      if (unlikely(__pyx_v_annotations == Py_None)) {
-        PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 177, __pyx_L1_error)
-      }
-      __pyx_t_10 = __Pyx_PyDict_GetItem(__pyx_v_annotations, __pyx_v_member_name); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 177, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_10);
-      if (!(likely(PyType_CheckExact(__pyx_t_10))||((__pyx_t_10) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "type", Py_TYPE(__pyx_t_10)->tp_name), 0))) __PYX_ERR(0, 177, __pyx_L1_error)
-
-      /* "tenforce/enforcer.pyx":178
- *                 member_name=member_name,
- *                 annotation=annotations[member_name],
- *                 obj=values.get(member_name),             # <<<<<<<<<<<<<<
- *                 auto_cast=auto_cast
- *             )
+  __pyx_t_3 = (__pyx_v_use_setstate != 0);
+  if (__pyx_t_3) {
+
+    /* "(tree fragment)":13
+ *         use_setstate = self.actual_type is not None or self.allowed_types is not None or self.class_name is not None or self.member_name is not None or self.obj is not None
+ *     if use_setstate:
+ *         return __pyx_unpickle_ParsedUnionMember, (type(self), 0x997196e, None), state             # <<<<<<<<<<<<<<
+ *     else:
+ *         return __pyx_unpickle_ParsedUnionMember, (type(self), 0x997196e, state)
  */
-      if (unlikely(__pyx_v_values == Py_None)) {
-        PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "get");
-        __PYX_ERR(0, 178, __pyx_L1_error)
-      }
-      __pyx_t_1 = __Pyx_PyDict_GetItemDefault(__pyx_v_values, __pyx_v_member_name, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pyx_unpickle_ParsedUnionMember); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_INCREF(__pyx_int_160897390);
+    __Pyx_GIVEREF(__pyx_int_160897390);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_160897390);
+    __Pyx_INCREF(Py_None);
+    __Pyx_GIVEREF(Py_None);
+    PyTuple_SET_ITEM(__pyx_t_1, 2, Py_None);
+    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_1);
+    __Pyx_INCREF(__pyx_v_state);
+    __Pyx_GIVEREF(__pyx_v_state);
+    PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_v_state);
+    __pyx_t_4 = 0;
+    __pyx_t_1 = 0;
+    __pyx_r = __pyx_t_6;
+    __pyx_t_6 = 0;
+    goto __pyx_L0;
 
-      /* "tenforce/enforcer.pyx":174
- *             )
- *         else:
- *             parsed_member = _parse_member(             # <<<<<<<<<<<<<<
- *                 class_name=class_name,
- *                 member_name=member_name,
- */
-      __pyx_t_12.__pyx_n = 1;
-      __pyx_t_12.auto_cast = __pyx_v_auto_cast;
-      __pyx_t_7 = ((PyObject *)__pyx_f_8tenforce_8enforcer__parse_member(__pyx_v_class_name, __pyx_v_member_name, ((PyTypeObject*)__pyx_t_10), __pyx_t_1, 0, &__pyx_t_12)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 174, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_XDECREF_SET(__pyx_v_parsed_member, ((struct __pyx_obj_8tenforce_8enforcer_ParsedMember *)__pyx_t_7));
-      __pyx_t_7 = 0;
+    /* "(tree fragment)":12
+ *     else:
+ *         use_setstate = self.actual_type is not None or self.allowed_types is not None or self.class_name is not None or self.member_name is not None or self.obj is not None
+ *     if use_setstate:             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_ParsedUnionMember, (type(self), 0x997196e, None), state
+ *     else:
+ */
+  }
 
-      /* "tenforce/enforcer.pyx":181
- *                 auto_cast=auto_cast
- *             )
- *             parsed_members.append(parsed_member)             # <<<<<<<<<<<<<<
+  /* "(tree fragment)":15
+ *         return __pyx_unpickle_ParsedUnionMember, (type(self), 0x997196e, None), state
+ *     else:
+ *         return __pyx_unpickle_ParsedUnionMember, (type(self), 0x997196e, state)             # <<<<<<<<<<<<<<
+ * def __setstate_cython__(self, __pyx_state):
+ *     __pyx_unpickle_ParsedUnionMember__set_state(self, __pyx_state)
  */
-      __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_parsed_members, ((PyObject *)__pyx_v_parsed_member)); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 181, __pyx_L1_error)
-    }
-    __pyx_L5:;
+  /*else*/ {
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_pyx_unpickle_ParsedUnionMember); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_INCREF(__pyx_int_160897390);
+    __Pyx_GIVEREF(__pyx_int_160897390);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_160897390);
+    __Pyx_INCREF(__pyx_v_state);
+    __Pyx_GIVEREF(__pyx_v_state);
+    PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_v_state);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_GIVEREF(__pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_6 = 0;
+    __pyx_t_1 = 0;
+    __pyx_r = __pyx_t_4;
+    __pyx_t_4 = 0;
+    goto __pyx_L0;
   }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "tenforce/enforcer.pyx":142
- * 
- * 
- * cpdef check(object obj, bint auto_cast = False):             # <<<<<<<<<<<<<<
- *     """
- *     Checks the class variables of an object & enforces its type hints
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     cdef tuple state
+ *     cdef object _dict
  */
 
   /* function exit code */
-  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-  goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_AddTraceback("tenforce.enforcer.check", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("tenforce.lib.members.ParsedUnionMember.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_class_name);
-  __Pyx_XDECREF(__pyx_v_annotations);
-  __Pyx_XDECREF(__pyx_v_values);
-  __Pyx_XDECREF(__pyx_v_parsed_members);
-  __Pyx_XDECREF((PyObject *)__pyx_v_parsed_member);
-  __Pyx_XDECREF(__pyx_v_parsed_generic_alias_member);
-  __Pyx_XDECREF(__pyx_v_member_name);
-  __Pyx_XDECREF((PyObject *)__pyx_v_plm);
+  __Pyx_XDECREF(__pyx_v_state);
+  __Pyx_XDECREF(__pyx_v__dict);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "(tree fragment)":16
+ *     else:
+ *         return __pyx_unpickle_ParsedUnionMember, (type(self), 0x997196e, state)
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_unpickle_ParsedUnionMember__set_state(self, __pyx_state)
+ */
+
 /* Python wrapper */
-static PyObject *__pyx_pw_8tenforce_8enforcer_7check(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_8tenforce_8enforcer_6check[] = "\n    Checks the class variables of an object & enforces its type hints\n    :param obj: Instance of a class\n    :param auto_cast: Optional, automatically cast things like \n    :return: None\n    ";
-static PyObject *__pyx_pw_8tenforce_8enforcer_7check(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  PyObject *__pyx_v_obj = 0;
-  int __pyx_v_auto_cast;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
+static PyObject *__pyx_pw_8tenforce_3lib_7members_17ParsedUnionMember_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_8tenforce_3lib_7members_17ParsedUnionMember_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("check (wrapper)", 0);
-  {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_obj,&__pyx_n_s_auto_cast,0};
-    PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
-      Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
-        case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_obj)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_auto_cast);
-          if (value) { values[1] = value; kw_args--; }
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "check") < 0)) __PYX_ERR(0, 142, __pyx_L3_error)
-      }
-    } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-    }
-    __pyx_v_obj = values[0];
-    if (values[1]) {
-      __pyx_v_auto_cast = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_auto_cast == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 142, __pyx_L3_error)
-    } else {
-      __pyx_v_auto_cast = ((int)0);
-    }
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("check", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 142, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("tenforce.enforcer.check", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8tenforce_8enforcer_6check(__pyx_self, __pyx_v_obj, __pyx_v_auto_cast);
+  __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_8tenforce_3lib_7members_17ParsedUnionMember_4__setstate_cython__(((struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8tenforce_8enforcer_6check(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_obj, int __pyx_v_auto_cast) {
+static PyObject *__pyx_pf_8tenforce_3lib_7members_17ParsedUnionMember_4__setstate_cython__(struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  struct __pyx_opt_args_8tenforce_8enforcer_check __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("check", 0);
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2.__pyx_n = 1;
-  __pyx_t_2.auto_cast = __pyx_v_auto_cast;
-  __pyx_t_1 = __pyx_f_8tenforce_8enforcer_check(__pyx_v_obj, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+
+  /* "(tree fragment)":17
+ *         return __pyx_unpickle_ParsedUnionMember, (type(self), 0x997196e, state)
+ * def __setstate_cython__(self, __pyx_state):
+ *     __pyx_unpickle_ParsedUnionMember__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
+ */
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8tenforce_3lib_7members___pyx_unpickle_ParsedUnionMember__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "(tree fragment)":16
+ *     else:
+ *         return __pyx_unpickle_ParsedUnionMember, (type(self), 0x997196e, state)
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_unpickle_ParsedUnionMember__set_state(self, __pyx_state)
+ */
 
   /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("tenforce.enforcer.check", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("tenforce.lib.members.ParsedUnionMember.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __pyx_unpickle_ParsedMember(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8tenforce_8enforcer_9__pyx_unpickle_ParsedMember(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_8tenforce_8enforcer_9__pyx_unpickle_ParsedMember = {"__pyx_unpickle_ParsedMember", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8tenforce_8enforcer_9__pyx_unpickle_ParsedMember, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8tenforce_8enforcer_9__pyx_unpickle_ParsedMember(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_8tenforce_3lib_7members_1__pyx_unpickle_ParsedMember(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_8tenforce_3lib_7members_1__pyx_unpickle_ParsedMember = {"__pyx_unpickle_ParsedMember", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8tenforce_3lib_7members_1__pyx_unpickle_ParsedMember, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8tenforce_3lib_7members_1__pyx_unpickle_ParsedMember(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -4553,26 +3525,26 @@
     __pyx_v___pyx_checksum = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v___pyx_checksum == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
     __pyx_v___pyx_state = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_ParsedMember", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("tenforce.enforcer.__pyx_unpickle_ParsedMember", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("tenforce.lib.members.__pyx_unpickle_ParsedMember", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8tenforce_8enforcer_8__pyx_unpickle_ParsedMember(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_8tenforce_3lib_7members___pyx_unpickle_ParsedMember(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8tenforce_8enforcer_8__pyx_unpickle_ParsedMember(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_8tenforce_3lib_7members___pyx_unpickle_ParsedMember(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
@@ -4589,15 +3561,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x2b52d43, 0x2bacb3c, 0xa433fcf):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x2b52d43, 0x2bacb3c, 0xa433fcf) = (actual_type, annotated_type, class_name, member_name, obj))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__4, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__3, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x2b52d43, 0x2bacb3c, 0xa433fcf):
@@ -4606,15 +3578,15 @@
  *     __pyx_result = ParsedMember.__new__(__pyx_type)
  */
     __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
     PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
-    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_t_1);
     __pyx_v___pyx_PickleError = __pyx_t_1;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -4665,15 +3637,15 @@
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x2b52d43, 0x2bacb3c, 0xa433fcf) = (actual_type, annotated_type, class_name, member_name, obj))" % __pyx_checksum)
  *     __pyx_result = ParsedMember.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_ParsedMember__set_state(<ParsedMember> __pyx_result, __pyx_state)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_8tenforce_8enforcer_ParsedMember), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_8tenforce_3lib_7members_ParsedMember), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_5);
@@ -4704,15 +3676,15 @@
  *     __pyx_result = ParsedMember.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_ParsedMember__set_state(<ParsedMember> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_ParsedMember__set_state(ParsedMember __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_4 = __pyx_f_8tenforce_8enforcer___pyx_unpickle_ParsedMember__set_state(((struct __pyx_obj_8tenforce_8enforcer_ParsedMember *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_8tenforce_3lib_7members___pyx_unpickle_ParsedMember__set_state(((struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x2b52d43, 0x2bacb3c, 0xa433fcf) = (actual_type, annotated_type, class_name, member_name, obj))" % __pyx_checksum)
  *     __pyx_result = ParsedMember.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
@@ -4741,15 +3713,15 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("tenforce.enforcer.__pyx_unpickle_ParsedMember", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("tenforce.lib.members.__pyx_unpickle_ParsedMember", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -4759,15 +3731,15 @@
  *         __pyx_unpickle_ParsedMember__set_state(<ParsedMember> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_ParsedMember__set_state(ParsedMember __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.actual_type = __pyx_state[0]; __pyx_result.annotated_type = __pyx_state[1]; __pyx_result.class_name = __pyx_state[2]; __pyx_result.member_name = __pyx_state[3]; __pyx_result.obj = __pyx_state[4]
  *     if len(__pyx_state) > 5 and hasattr(__pyx_result, '__dict__'):
  */
 
-static PyObject *__pyx_f_8tenforce_8enforcer___pyx_unpickle_ParsedMember__set_state(struct __pyx_obj_8tenforce_8enforcer_ParsedMember *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_f_8tenforce_3lib_7members___pyx_unpickle_ParsedMember__set_state(struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
@@ -4812,27 +3784,27 @@
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
+  if (!(likely(PyString_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "str", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v___pyx_result->class_name);
   __Pyx_DECREF(__pyx_v___pyx_result->class_name);
   __pyx_v___pyx_result->class_name = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 3, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
+  if (!(likely(PyString_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "str", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v___pyx_result->member_name);
   __Pyx_DECREF(__pyx_v___pyx_result->member_name);
   __pyx_v___pyx_result->member_name = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
@@ -4923,32 +3895,32 @@
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("tenforce.enforcer.__pyx_unpickle_ParsedMember__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("tenforce.lib.members.__pyx_unpickle_ParsedMember__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __pyx_unpickle_ParsedListMember(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8tenforce_8enforcer_11__pyx_unpickle_ParsedListMember(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_8tenforce_8enforcer_11__pyx_unpickle_ParsedListMember = {"__pyx_unpickle_ParsedListMember", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8tenforce_8enforcer_11__pyx_unpickle_ParsedListMember, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8tenforce_8enforcer_11__pyx_unpickle_ParsedListMember(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_8tenforce_3lib_7members_3__pyx_unpickle_ParsedListMember(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_8tenforce_3lib_7members_3__pyx_unpickle_ParsedListMember = {"__pyx_unpickle_ParsedListMember", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8tenforce_3lib_7members_3__pyx_unpickle_ParsedListMember, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8tenforce_3lib_7members_3__pyx_unpickle_ParsedListMember(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -5002,26 +3974,26 @@
     __pyx_v___pyx_checksum = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v___pyx_checksum == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
     __pyx_v___pyx_state = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_ParsedListMember", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("tenforce.enforcer.__pyx_unpickle_ParsedListMember", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("tenforce.lib.members.__pyx_unpickle_ParsedListMember", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8tenforce_8enforcer_10__pyx_unpickle_ParsedListMember(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_8tenforce_3lib_7members_2__pyx_unpickle_ParsedListMember(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8tenforce_8enforcer_10__pyx_unpickle_ParsedListMember(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_8tenforce_3lib_7members_2__pyx_unpickle_ParsedListMember(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
@@ -5038,15 +4010,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xd0ed7c0, 0xb986991, 0x5dd79c2):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd0ed7c0, 0xb986991, 0x5dd79c2) = (base_annotated_type, class_name, list_, member_name))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__5, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__4, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xd0ed7c0, 0xb986991, 0x5dd79c2):
@@ -5055,15 +4027,15 @@
  *     __pyx_result = ParsedListMember.__new__(__pyx_type)
  */
     __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
     PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
-    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_t_1);
     __pyx_v___pyx_PickleError = __pyx_t_1;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -5114,15 +4086,15 @@
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd0ed7c0, 0xb986991, 0x5dd79c2) = (base_annotated_type, class_name, list_, member_name))" % __pyx_checksum)
  *     __pyx_result = ParsedListMember.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_ParsedListMember__set_state(<ParsedListMember> __pyx_result, __pyx_state)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_8tenforce_8enforcer_ParsedListMember), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_8tenforce_3lib_7members_ParsedListMember), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_5);
@@ -5153,15 +4125,15 @@
  *     __pyx_result = ParsedListMember.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_ParsedListMember__set_state(<ParsedListMember> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_ParsedListMember__set_state(ParsedListMember __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_4 = __pyx_f_8tenforce_8enforcer___pyx_unpickle_ParsedListMember__set_state(((struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_8tenforce_3lib_7members___pyx_unpickle_ParsedListMember__set_state(((struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd0ed7c0, 0xb986991, 0x5dd79c2) = (base_annotated_type, class_name, list_, member_name))" % __pyx_checksum)
  *     __pyx_result = ParsedListMember.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
@@ -5190,15 +4162,15 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("tenforce.enforcer.__pyx_unpickle_ParsedListMember", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("tenforce.lib.members.__pyx_unpickle_ParsedListMember", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -5208,15 +4180,15 @@
  *         __pyx_unpickle_ParsedListMember__set_state(<ParsedListMember> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_ParsedListMember__set_state(ParsedListMember __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.base_annotated_type = __pyx_state[0]; __pyx_result.class_name = __pyx_state[1]; __pyx_result.list_ = __pyx_state[2]; __pyx_result.member_name = __pyx_state[3]
  *     if len(__pyx_state) > 4 and hasattr(__pyx_result, '__dict__'):
  */
 
-static PyObject *__pyx_f_8tenforce_8enforcer___pyx_unpickle_ParsedListMember__set_state(struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_f_8tenforce_3lib_7members___pyx_unpickle_ParsedListMember__set_state(struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
@@ -5249,15 +4221,15 @@
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
+  if (!(likely(PyString_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "str", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v___pyx_result->class_name);
   __Pyx_DECREF(__pyx_v___pyx_result->class_name);
   __pyx_v___pyx_result->class_name = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
@@ -5273,15 +4245,15 @@
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 3, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
+  if (!(likely(PyString_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "str", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v___pyx_result->member_name);
   __Pyx_DECREF(__pyx_v___pyx_result->member_name);
   __pyx_v___pyx_result->member_name = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "(tree fragment)":13
@@ -5361,101 +4333,550 @@
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("tenforce.enforcer.__pyx_unpickle_ParsedListMember__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("tenforce.lib.members.__pyx_unpickle_ParsedListMember__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static struct __pyx_vtabstruct_8tenforce_8enforcer_ParsedMember __pyx_vtable_8tenforce_8enforcer_ParsedMember;
 
-static PyObject *__pyx_tp_new_8tenforce_8enforcer_ParsedMember(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
-  struct __pyx_obj_8tenforce_8enforcer_ParsedMember *p;
+/* "(tree fragment)":1
+ * def __pyx_unpickle_ParsedUnionMember(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_8tenforce_3lib_7members_5__pyx_unpickle_ParsedUnionMember(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_8tenforce_3lib_7members_5__pyx_unpickle_ParsedUnionMember = {"__pyx_unpickle_ParsedUnionMember", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8tenforce_3lib_7members_5__pyx_unpickle_ParsedUnionMember, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8tenforce_3lib_7members_5__pyx_unpickle_ParsedUnionMember(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v___pyx_type = 0;
+  long __pyx_v___pyx_checksum;
+  PyObject *__pyx_v___pyx_state = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__pyx_unpickle_ParsedUnionMember (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_type,&__pyx_n_s_pyx_checksum,&__pyx_n_s_pyx_state,0};
+    PyObject* values[3] = {0,0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_type)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_checksum)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_ParsedUnionMember", 1, 3, 3, 1); __PYX_ERR(1, 1, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_state)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_ParsedUnionMember", 1, 3, 3, 2); __PYX_ERR(1, 1, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_unpickle_ParsedUnionMember") < 0)) __PYX_ERR(1, 1, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+    }
+    __pyx_v___pyx_type = values[0];
+    __pyx_v___pyx_checksum = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v___pyx_checksum == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
+    __pyx_v___pyx_state = values[2];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_ParsedUnionMember", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("tenforce.lib.members.__pyx_unpickle_ParsedUnionMember", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_8tenforce_3lib_7members_4__pyx_unpickle_ParsedUnionMember(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_8tenforce_3lib_7members_4__pyx_unpickle_ParsedUnionMember(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_v___pyx_PickleError = 0;
+  PyObject *__pyx_v___pyx_result = 0;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_unpickle_ParsedUnionMember", 0);
+
+  /* "(tree fragment)":4
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0x997196e, 0x521cf66, 0xa47b3e8):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x997196e, 0x521cf66, 0xa47b3e8) = (actual_type, allowed_types, class_name, member_name, obj))" % __pyx_checksum)
+ */
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__5, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
+
+    /* "(tree fragment)":5
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0x997196e, 0x521cf66, 0xa47b3e8):
+ *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x997196e, 0x521cf66, 0xa47b3e8) = (actual_type, allowed_types, class_name, member_name, obj))" % __pyx_checksum)
+ *     __pyx_result = ParsedUnionMember.__new__(__pyx_type)
+ */
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_n_s_PickleError);
+    __Pyx_GIVEREF(__pyx_n_s_PickleError);
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, -1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+    /* "(tree fragment)":6
+ *     if __pyx_checksum not in (0x997196e, 0x521cf66, 0xa47b3e8):
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x997196e, 0x521cf66, 0xa47b3e8) = (actual_type, allowed_types, class_name, member_name, obj))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *     __pyx_result = ParsedUnionMember.__new__(__pyx_type)
+ *     if __pyx_state is not None:
+ */
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_INCREF(__pyx_v___pyx_PickleError);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
+      }
+    }
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __PYX_ERR(1, 6, __pyx_L1_error)
+
+    /* "(tree fragment)":4
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0x997196e, 0x521cf66, 0xa47b3e8):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x997196e, 0x521cf66, 0xa47b3e8) = (actual_type, allowed_types, class_name, member_name, obj))" % __pyx_checksum)
+ */
+  }
+
+  /* "(tree fragment)":7
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x997196e, 0x521cf66, 0xa47b3e8) = (actual_type, allowed_types, class_name, member_name, obj))" % __pyx_checksum)
+ *     __pyx_result = ParsedUnionMember.__new__(__pyx_type)             # <<<<<<<<<<<<<<
+ *     if __pyx_state is not None:
+ *         __pyx_unpickle_ParsedUnionMember__set_state(<ParsedUnionMember> __pyx_result, __pyx_state)
+ */
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_8tenforce_3lib_7members_ParsedUnionMember), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
+    }
+  }
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
+
+  /* "(tree fragment)":8
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x997196e, 0x521cf66, 0xa47b3e8) = (actual_type, allowed_types, class_name, member_name, obj))" % __pyx_checksum)
+ *     __pyx_result = ParsedUnionMember.__new__(__pyx_type)
+ *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
+ *         __pyx_unpickle_ParsedUnionMember__set_state(<ParsedUnionMember> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ */
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
+
+    /* "(tree fragment)":9
+ *     __pyx_result = ParsedUnionMember.__new__(__pyx_type)
+ *     if __pyx_state is not None:
+ *         __pyx_unpickle_ParsedUnionMember__set_state(<ParsedUnionMember> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
+ *     return __pyx_result
+ * cdef __pyx_unpickle_ParsedUnionMember__set_state(ParsedUnionMember __pyx_result, tuple __pyx_state):
+ */
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_8tenforce_3lib_7members___pyx_unpickle_ParsedUnionMember__set_state(((struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+    /* "(tree fragment)":8
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x997196e, 0x521cf66, 0xa47b3e8) = (actual_type, allowed_types, class_name, member_name, obj))" % __pyx_checksum)
+ *     __pyx_result = ParsedUnionMember.__new__(__pyx_type)
+ *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
+ *         __pyx_unpickle_ParsedUnionMember__set_state(<ParsedUnionMember> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ */
+  }
+
+  /* "(tree fragment)":10
+ *     if __pyx_state is not None:
+ *         __pyx_unpickle_ParsedUnionMember__set_state(<ParsedUnionMember> __pyx_result, __pyx_state)
+ *     return __pyx_result             # <<<<<<<<<<<<<<
+ * cdef __pyx_unpickle_ParsedUnionMember__set_state(ParsedUnionMember __pyx_result, tuple __pyx_state):
+ *     __pyx_result.actual_type = __pyx_state[0]; __pyx_result.allowed_types = __pyx_state[1]; __pyx_result.class_name = __pyx_state[2]; __pyx_result.member_name = __pyx_state[3]; __pyx_result.obj = __pyx_state[4]
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v___pyx_result);
+  __pyx_r = __pyx_v___pyx_result;
+  goto __pyx_L0;
+
+  /* "(tree fragment)":1
+ * def __pyx_unpickle_ParsedUnionMember(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("tenforce.lib.members.__pyx_unpickle_ParsedUnionMember", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v___pyx_PickleError);
+  __Pyx_XDECREF(__pyx_v___pyx_result);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "(tree fragment)":11
+ *         __pyx_unpickle_ParsedUnionMember__set_state(<ParsedUnionMember> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ * cdef __pyx_unpickle_ParsedUnionMember__set_state(ParsedUnionMember __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_result.actual_type = __pyx_state[0]; __pyx_result.allowed_types = __pyx_state[1]; __pyx_result.class_name = __pyx_state[2]; __pyx_result.member_name = __pyx_state[3]; __pyx_result.obj = __pyx_state[4]
+ *     if len(__pyx_state) > 5 and hasattr(__pyx_result, '__dict__'):
+ */
+
+static PyObject *__pyx_f_8tenforce_3lib_7members___pyx_unpickle_ParsedUnionMember__set_state(struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  Py_ssize_t __pyx_t_3;
+  int __pyx_t_4;
+  int __pyx_t_5;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_unpickle_ParsedUnionMember__set_state", 0);
+
+  /* "(tree fragment)":12
+ *     return __pyx_result
+ * cdef __pyx_unpickle_ParsedUnionMember__set_state(ParsedUnionMember __pyx_result, tuple __pyx_state):
+ *     __pyx_result.actual_type = __pyx_state[0]; __pyx_result.allowed_types = __pyx_state[1]; __pyx_result.class_name = __pyx_state[2]; __pyx_result.member_name = __pyx_state[3]; __pyx_result.obj = __pyx_state[4]             # <<<<<<<<<<<<<<
+ *     if len(__pyx_state) > 5 and hasattr(__pyx_result, '__dict__'):
+ *         __pyx_result.__dict__.update(__pyx_state[5])
+ */
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (!(likely(PyType_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "type", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->actual_type);
+  __Pyx_DECREF(((PyObject *)__pyx_v___pyx_result->actual_type));
+  __pyx_v___pyx_result->actual_type = ((PyTypeObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (!(likely(PyTuple_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->allowed_types);
+  __Pyx_DECREF(__pyx_v___pyx_result->allowed_types);
+  __pyx_v___pyx_result->allowed_types = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (!(likely(PyString_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "str", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->class_name);
+  __Pyx_DECREF(__pyx_v___pyx_result->class_name);
+  __pyx_v___pyx_result->class_name = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 3, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (!(likely(PyString_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "str", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->member_name);
+  __Pyx_DECREF(__pyx_v___pyx_result->member_name);
+  __pyx_v___pyx_result->member_name = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 4, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->obj);
+  __Pyx_DECREF(__pyx_v___pyx_result->obj);
+  __pyx_v___pyx_result->obj = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "(tree fragment)":13
+ * cdef __pyx_unpickle_ParsedUnionMember__set_state(ParsedUnionMember __pyx_result, tuple __pyx_state):
+ *     __pyx_result.actual_type = __pyx_state[0]; __pyx_result.allowed_types = __pyx_state[1]; __pyx_result.class_name = __pyx_state[2]; __pyx_result.member_name = __pyx_state[3]; __pyx_result.obj = __pyx_state[4]
+ *     if len(__pyx_state) > 5 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
+ *         __pyx_result.__dict__.update(__pyx_state[5])
+ */
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+    __PYX_ERR(1, 13, __pyx_L1_error)
+  }
+  __pyx_t_3 = PyTuple_GET_SIZE(__pyx_v___pyx_state); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
+  __pyx_t_4 = ((__pyx_t_3 > 5) != 0);
+  if (__pyx_t_4) {
+  } else {
+    __pyx_t_2 = __pyx_t_4;
+    goto __pyx_L4_bool_binop_done;
+  }
+  __pyx_t_4 = __Pyx_HasAttr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
+  __pyx_t_5 = (__pyx_t_4 != 0);
+  __pyx_t_2 = __pyx_t_5;
+  __pyx_L4_bool_binop_done:;
+  if (__pyx_t_2) {
+
+    /* "(tree fragment)":14
+ *     __pyx_result.actual_type = __pyx_state[0]; __pyx_result.allowed_types = __pyx_state[1]; __pyx_result.class_name = __pyx_state[2]; __pyx_result.member_name = __pyx_state[3]; __pyx_result.obj = __pyx_state[4]
+ *     if len(__pyx_state) > 5 and hasattr(__pyx_result, '__dict__'):
+ *         __pyx_result.__dict__.update(__pyx_state[5])             # <<<<<<<<<<<<<<
+ */
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_update); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (unlikely(__pyx_v___pyx_state == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+      __PYX_ERR(1, 14, __pyx_L1_error)
+    }
+    __pyx_t_6 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 5, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_8 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
+      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
+      if (likely(__pyx_t_8)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+        __Pyx_INCREF(__pyx_t_8);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_7, function);
+      }
+    }
+    __pyx_t_1 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_6);
+    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "(tree fragment)":13
+ * cdef __pyx_unpickle_ParsedUnionMember__set_state(ParsedUnionMember __pyx_result, tuple __pyx_state):
+ *     __pyx_result.actual_type = __pyx_state[0]; __pyx_result.allowed_types = __pyx_state[1]; __pyx_result.class_name = __pyx_state[2]; __pyx_result.member_name = __pyx_state[3]; __pyx_result.obj = __pyx_state[4]
+ *     if len(__pyx_state) > 5 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
+ *         __pyx_result.__dict__.update(__pyx_state[5])
+ */
+  }
+
+  /* "(tree fragment)":11
+ *         __pyx_unpickle_ParsedUnionMember__set_state(<ParsedUnionMember> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ * cdef __pyx_unpickle_ParsedUnionMember__set_state(ParsedUnionMember __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_result.actual_type = __pyx_state[0]; __pyx_result.allowed_types = __pyx_state[1]; __pyx_result.class_name = __pyx_state[2]; __pyx_result.member_name = __pyx_state[3]; __pyx_result.obj = __pyx_state[4]
+ *     if len(__pyx_state) > 5 and hasattr(__pyx_result, '__dict__'):
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("tenforce.lib.members.__pyx_unpickle_ParsedUnionMember__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+static struct __pyx_vtabstruct_8tenforce_3lib_7members_ParsedMember __pyx_vtable_8tenforce_3lib_7members_ParsedMember;
+
+static PyObject *__pyx_tp_new_8tenforce_3lib_7members_ParsedMember(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+  struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
-  p = ((struct __pyx_obj_8tenforce_8enforcer_ParsedMember *)o);
-  p->__pyx_vtab = __pyx_vtabptr_8tenforce_8enforcer_ParsedMember;
+  p = ((struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *)o);
+  p->__pyx_vtab = __pyx_vtabptr_8tenforce_3lib_7members_ParsedMember;
   p->annotated_type = ((PyTypeObject*)Py_None); Py_INCREF(Py_None);
   p->actual_type = ((PyTypeObject*)Py_None); Py_INCREF(Py_None);
   p->obj = Py_None; Py_INCREF(Py_None);
   p->member_name = ((PyObject*)Py_None); Py_INCREF(Py_None);
   p->class_name = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
-static void __pyx_tp_dealloc_8tenforce_8enforcer_ParsedMember(PyObject *o) {
-  struct __pyx_obj_8tenforce_8enforcer_ParsedMember *p = (struct __pyx_obj_8tenforce_8enforcer_ParsedMember *)o;
+static void __pyx_tp_dealloc_8tenforce_3lib_7members_ParsedMember(PyObject *o) {
+  struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *p = (struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *)o;
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->annotated_type);
   Py_CLEAR(p->actual_type);
   Py_CLEAR(p->obj);
   Py_CLEAR(p->member_name);
   Py_CLEAR(p->class_name);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
-static int __pyx_tp_traverse_8tenforce_8enforcer_ParsedMember(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_8tenforce_3lib_7members_ParsedMember(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_8tenforce_8enforcer_ParsedMember *p = (struct __pyx_obj_8tenforce_8enforcer_ParsedMember *)o;
+  struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *p = (struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *)o;
   if (p->annotated_type) {
     e = (*v)(((PyObject *)p->annotated_type), a); if (e) return e;
   }
   if (p->actual_type) {
     e = (*v)(((PyObject *)p->actual_type), a); if (e) return e;
   }
   if (p->obj) {
     e = (*v)(p->obj, a); if (e) return e;
   }
   return 0;
 }
 
-static int __pyx_tp_clear_8tenforce_8enforcer_ParsedMember(PyObject *o) {
+static int __pyx_tp_clear_8tenforce_3lib_7members_ParsedMember(PyObject *o) {
   PyObject* tmp;
-  struct __pyx_obj_8tenforce_8enforcer_ParsedMember *p = (struct __pyx_obj_8tenforce_8enforcer_ParsedMember *)o;
+  struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *p = (struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *)o;
   tmp = ((PyObject*)p->annotated_type);
   p->annotated_type = ((PyTypeObject*)Py_None); Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->actual_type);
   p->actual_type = ((PyTypeObject*)Py_None); Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->obj);
   p->obj = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
-static PyMethodDef __pyx_methods_8tenforce_8enforcer_ParsedMember[] = {
-  {"enforce", (PyCFunction)__pyx_pw_8tenforce_8enforcer_12ParsedMember_1enforce, METH_NOARGS, __pyx_doc_8tenforce_8enforcer_12ParsedMember_enforce},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_8tenforce_8enforcer_12ParsedMember_3__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_8tenforce_8enforcer_12ParsedMember_5__setstate_cython__, METH_O, 0},
+static PyMethodDef __pyx_methods_8tenforce_3lib_7members_ParsedMember[] = {
+  {"enforce", (PyCFunction)__pyx_pw_8tenforce_3lib_7members_12ParsedMember_1enforce, METH_NOARGS, __pyx_doc_8tenforce_3lib_7members_12ParsedMember_enforce},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_8tenforce_3lib_7members_12ParsedMember_3__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_8tenforce_3lib_7members_12ParsedMember_5__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
-static PyTypeObject __pyx_type_8tenforce_8enforcer_ParsedMember = {
+static PyTypeObject __pyx_type_8tenforce_3lib_7members_ParsedMember = {
   PyVarObject_HEAD_INIT(0, 0)
-  "tenforce.enforcer.ParsedMember", /*tp_name*/
-  sizeof(struct __pyx_obj_8tenforce_8enforcer_ParsedMember), /*tp_basicsize*/
+  "tenforce.lib.members.ParsedMember", /*tp_name*/
+  sizeof(struct __pyx_obj_8tenforce_3lib_7members_ParsedMember), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_8tenforce_8enforcer_ParsedMember, /*tp_dealloc*/
+  __pyx_tp_dealloc_8tenforce_3lib_7members_ParsedMember, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -5474,31 +4895,31 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   0, /*tp_doc*/
-  __pyx_tp_traverse_8tenforce_8enforcer_ParsedMember, /*tp_traverse*/
-  __pyx_tp_clear_8tenforce_8enforcer_ParsedMember, /*tp_clear*/
+  __pyx_tp_traverse_8tenforce_3lib_7members_ParsedMember, /*tp_traverse*/
+  __pyx_tp_clear_8tenforce_3lib_7members_ParsedMember, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_8tenforce_8enforcer_ParsedMember, /*tp_methods*/
+  __pyx_methods_8tenforce_3lib_7members_ParsedMember, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_8tenforce_8enforcer_ParsedMember, /*tp_new*/
+  __pyx_tp_new_8tenforce_3lib_7members_ParsedMember, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -5513,86 +4934,86 @@
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
-static struct __pyx_vtabstruct_8tenforce_8enforcer_ParsedListMember __pyx_vtable_8tenforce_8enforcer_ParsedListMember;
+static struct __pyx_vtabstruct_8tenforce_3lib_7members_ParsedListMember __pyx_vtable_8tenforce_3lib_7members_ParsedListMember;
 
-static PyObject *__pyx_tp_new_8tenforce_8enforcer_ParsedListMember(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
-  struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *p;
+static PyObject *__pyx_tp_new_8tenforce_3lib_7members_ParsedListMember(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+  struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
-  p = ((struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *)o);
-  p->__pyx_vtab = __pyx_vtabptr_8tenforce_8enforcer_ParsedListMember;
+  p = ((struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *)o);
+  p->__pyx_vtab = __pyx_vtabptr_8tenforce_3lib_7members_ParsedListMember;
   p->base_annotated_type = ((PyTypeObject*)Py_None); Py_INCREF(Py_None);
   p->list_ = ((PyObject*)Py_None); Py_INCREF(Py_None);
   p->member_name = ((PyObject*)Py_None); Py_INCREF(Py_None);
   p->class_name = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
-static void __pyx_tp_dealloc_8tenforce_8enforcer_ParsedListMember(PyObject *o) {
-  struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *p = (struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *)o;
+static void __pyx_tp_dealloc_8tenforce_3lib_7members_ParsedListMember(PyObject *o) {
+  struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *p = (struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *)o;
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->base_annotated_type);
   Py_CLEAR(p->list_);
   Py_CLEAR(p->member_name);
   Py_CLEAR(p->class_name);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
-static int __pyx_tp_traverse_8tenforce_8enforcer_ParsedListMember(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_8tenforce_3lib_7members_ParsedListMember(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *p = (struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *)o;
+  struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *p = (struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *)o;
   if (p->base_annotated_type) {
     e = (*v)(((PyObject *)p->base_annotated_type), a); if (e) return e;
   }
   if (p->list_) {
     e = (*v)(p->list_, a); if (e) return e;
   }
   return 0;
 }
 
-static int __pyx_tp_clear_8tenforce_8enforcer_ParsedListMember(PyObject *o) {
+static int __pyx_tp_clear_8tenforce_3lib_7members_ParsedListMember(PyObject *o) {
   PyObject* tmp;
-  struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *p = (struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *)o;
+  struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *p = (struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *)o;
   tmp = ((PyObject*)p->base_annotated_type);
   p->base_annotated_type = ((PyTypeObject*)Py_None); Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->list_);
   p->list_ = ((PyObject*)Py_None); Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
-static PyMethodDef __pyx_methods_8tenforce_8enforcer_ParsedListMember[] = {
-  {"enforce", (PyCFunction)__pyx_pw_8tenforce_8enforcer_16ParsedListMember_1enforce, METH_NOARGS, __pyx_doc_8tenforce_8enforcer_16ParsedListMember_enforce},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_8tenforce_8enforcer_16ParsedListMember_3__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_8tenforce_8enforcer_16ParsedListMember_5__setstate_cython__, METH_O, 0},
+static PyMethodDef __pyx_methods_8tenforce_3lib_7members_ParsedListMember[] = {
+  {"enforce", (PyCFunction)__pyx_pw_8tenforce_3lib_7members_16ParsedListMember_1enforce, METH_NOARGS, __pyx_doc_8tenforce_3lib_7members_16ParsedListMember_enforce},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_8tenforce_3lib_7members_16ParsedListMember_3__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_8tenforce_3lib_7members_16ParsedListMember_5__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
-static PyTypeObject __pyx_type_8tenforce_8enforcer_ParsedListMember = {
+static PyTypeObject __pyx_type_8tenforce_3lib_7members_ParsedListMember = {
   PyVarObject_HEAD_INIT(0, 0)
-  "tenforce.enforcer.ParsedListMember", /*tp_name*/
-  sizeof(struct __pyx_obj_8tenforce_8enforcer_ParsedListMember), /*tp_basicsize*/
+  "tenforce.lib.members.ParsedListMember", /*tp_name*/
+  sizeof(struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_8tenforce_8enforcer_ParsedListMember, /*tp_dealloc*/
+  __pyx_tp_dealloc_8tenforce_3lib_7members_ParsedListMember, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -5611,31 +5032,176 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   0, /*tp_doc*/
-  __pyx_tp_traverse_8tenforce_8enforcer_ParsedListMember, /*tp_traverse*/
-  __pyx_tp_clear_8tenforce_8enforcer_ParsedListMember, /*tp_clear*/
+  __pyx_tp_traverse_8tenforce_3lib_7members_ParsedListMember, /*tp_traverse*/
+  __pyx_tp_clear_8tenforce_3lib_7members_ParsedListMember, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_8tenforce_8enforcer_ParsedListMember, /*tp_methods*/
+  __pyx_methods_8tenforce_3lib_7members_ParsedListMember, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_8tenforce_8enforcer_ParsedListMember, /*tp_new*/
+  __pyx_tp_new_8tenforce_3lib_7members_ParsedListMember, /*tp_new*/
+  0, /*tp_free*/
+  0, /*tp_is_gc*/
+  0, /*tp_bases*/
+  0, /*tp_mro*/
+  0, /*tp_cache*/
+  0, /*tp_subclasses*/
+  0, /*tp_weaklist*/
+  0, /*tp_del*/
+  0, /*tp_version_tag*/
+  #if PY_VERSION_HEX >= 0x030400a1
+  0, /*tp_finalize*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+  0, /*tp_vectorcall*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  0, /*tp_print*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  0, /*tp_pypy_flags*/
+  #endif
+};
+static struct __pyx_vtabstruct_8tenforce_3lib_7members_ParsedUnionMember __pyx_vtable_8tenforce_3lib_7members_ParsedUnionMember;
+
+static PyObject *__pyx_tp_new_8tenforce_3lib_7members_ParsedUnionMember(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+  struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *p;
+  PyObject *o;
+  if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
+    o = (*t->tp_alloc)(t, 0);
+  } else {
+    o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
+  }
+  if (unlikely(!o)) return 0;
+  p = ((struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *)o);
+  p->__pyx_vtab = __pyx_vtabptr_8tenforce_3lib_7members_ParsedUnionMember;
+  p->allowed_types = ((PyObject*)Py_None); Py_INCREF(Py_None);
+  p->actual_type = ((PyTypeObject*)Py_None); Py_INCREF(Py_None);
+  p->obj = Py_None; Py_INCREF(Py_None);
+  p->member_name = ((PyObject*)Py_None); Py_INCREF(Py_None);
+  p->class_name = ((PyObject*)Py_None); Py_INCREF(Py_None);
+  return o;
+}
+
+static void __pyx_tp_dealloc_8tenforce_3lib_7members_ParsedUnionMember(PyObject *o) {
+  struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *p = (struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *)o;
+  #if CYTHON_USE_TP_FINALIZE
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+    if (PyObject_CallFinalizerFromDealloc(o)) return;
+  }
+  #endif
+  PyObject_GC_UnTrack(o);
+  Py_CLEAR(p->allowed_types);
+  Py_CLEAR(p->actual_type);
+  Py_CLEAR(p->obj);
+  Py_CLEAR(p->member_name);
+  Py_CLEAR(p->class_name);
+  (*Py_TYPE(o)->tp_free)(o);
+}
+
+static int __pyx_tp_traverse_8tenforce_3lib_7members_ParsedUnionMember(PyObject *o, visitproc v, void *a) {
+  int e;
+  struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *p = (struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *)o;
+  if (p->allowed_types) {
+    e = (*v)(p->allowed_types, a); if (e) return e;
+  }
+  if (p->actual_type) {
+    e = (*v)(((PyObject *)p->actual_type), a); if (e) return e;
+  }
+  if (p->obj) {
+    e = (*v)(p->obj, a); if (e) return e;
+  }
+  return 0;
+}
+
+static int __pyx_tp_clear_8tenforce_3lib_7members_ParsedUnionMember(PyObject *o) {
+  PyObject* tmp;
+  struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *p = (struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *)o;
+  tmp = ((PyObject*)p->allowed_types);
+  p->allowed_types = ((PyObject*)Py_None); Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
+  tmp = ((PyObject*)p->actual_type);
+  p->actual_type = ((PyTypeObject*)Py_None); Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
+  tmp = ((PyObject*)p->obj);
+  p->obj = Py_None; Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
+  return 0;
+}
+
+static PyMethodDef __pyx_methods_8tenforce_3lib_7members_ParsedUnionMember[] = {
+  {"enforce", (PyCFunction)__pyx_pw_8tenforce_3lib_7members_17ParsedUnionMember_1enforce, METH_NOARGS, __pyx_doc_8tenforce_3lib_7members_17ParsedUnionMember_enforce},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_8tenforce_3lib_7members_17ParsedUnionMember_3__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_8tenforce_3lib_7members_17ParsedUnionMember_5__setstate_cython__, METH_O, 0},
+  {0, 0, 0, 0}
+};
+
+static PyTypeObject __pyx_type_8tenforce_3lib_7members_ParsedUnionMember = {
+  PyVarObject_HEAD_INIT(0, 0)
+  "tenforce.lib.members.ParsedUnionMember", /*tp_name*/
+  sizeof(struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember), /*tp_basicsize*/
+  0, /*tp_itemsize*/
+  __pyx_tp_dealloc_8tenforce_3lib_7members_ParsedUnionMember, /*tp_dealloc*/
+  #if PY_VERSION_HEX < 0x030800b4
+  0, /*tp_print*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4
+  0, /*tp_vectorcall_offset*/
+  #endif
+  0, /*tp_getattr*/
+  0, /*tp_setattr*/
+  #if PY_MAJOR_VERSION < 3
+  0, /*tp_compare*/
+  #endif
+  #if PY_MAJOR_VERSION >= 3
+  0, /*tp_as_async*/
+  #endif
+  0, /*tp_repr*/
+  0, /*tp_as_number*/
+  0, /*tp_as_sequence*/
+  0, /*tp_as_mapping*/
+  0, /*tp_hash*/
+  0, /*tp_call*/
+  0, /*tp_str*/
+  0, /*tp_getattro*/
+  0, /*tp_setattro*/
+  0, /*tp_as_buffer*/
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
+  0, /*tp_doc*/
+  __pyx_tp_traverse_8tenforce_3lib_7members_ParsedUnionMember, /*tp_traverse*/
+  __pyx_tp_clear_8tenforce_3lib_7members_ParsedUnionMember, /*tp_clear*/
+  0, /*tp_richcompare*/
+  0, /*tp_weaklistoffset*/
+  0, /*tp_iter*/
+  0, /*tp_iternext*/
+  __pyx_methods_8tenforce_3lib_7members_ParsedUnionMember, /*tp_methods*/
+  0, /*tp_members*/
+  0, /*tp_getset*/
+  0, /*tp_base*/
+  0, /*tp_dict*/
+  0, /*tp_descr_get*/
+  0, /*tp_descr_set*/
+  0, /*tp_dictoffset*/
+  0, /*tp_init*/
+  0, /*tp_alloc*/
+  __pyx_tp_new_8tenforce_3lib_7members_ParsedUnionMember, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -5652,35 +5218,31 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
-  {"_auto_cast", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8tenforce_8enforcer_1_auto_cast, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8tenforce_8enforcer__auto_cast},
-  {"_parse_generic_alias_member", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8tenforce_8enforcer_3_parse_generic_alias_member, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8tenforce_8enforcer_2_parse_generic_alias_member},
-  {"_parse_member", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8tenforce_8enforcer_5_parse_member, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8tenforce_8enforcer_4_parse_member},
-  {"check", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8tenforce_8enforcer_7check, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8tenforce_8enforcer_6check},
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec_enforcer(PyObject* module); /*proto*/
+static int __pyx_pymod_exec_members(PyObject* module); /*proto*/
 static PyModuleDef_Slot __pyx_moduledef_slots[] = {
   {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec_enforcer},
+  {Py_mod_exec, (void*)__pyx_pymod_exec_members},
   {0, NULL}
 };
 #endif
 
 static struct PyModuleDef __pyx_moduledef = {
     PyModuleDef_HEAD_INIT,
-    "enforcer",
+    "members",
     0, /* m_doc */
   #if CYTHON_PEP489_MULTI_PHASE_INIT
     0, /* m_size */
   #else
     -1, /* m_size */
   #endif
     __pyx_methods /* m_methods */,
@@ -5702,79 +5264,61 @@
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_kp_u_, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 0},
-  {&__pyx_n_s_AutoCastError, __pyx_k_AutoCastError, sizeof(__pyx_k_AutoCastError), 0, 0, 1, 1},
-  {&__pyx_n_s_GenericAlias, __pyx_k_GenericAlias, sizeof(__pyx_k_GenericAlias), 0, 0, 1, 1},
   {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
   {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2, __pyx_k_Incompatible_checksums_0x_x_vs_0_2, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_2), 0, 0, 1, 0},
-  {&__pyx_kp_u_None, __pyx_k_None, sizeof(__pyx_k_None), 0, 1, 0, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_3, __pyx_k_Incompatible_checksums_0x_x_vs_0_3, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_3), 0, 0, 1, 0},
   {&__pyx_n_s_ParsedListMember, __pyx_k_ParsedListMember, sizeof(__pyx_k_ParsedListMember), 0, 0, 1, 1},
   {&__pyx_n_s_ParsedMember, __pyx_k_ParsedMember, sizeof(__pyx_k_ParsedMember), 0, 0, 1, 1},
+  {&__pyx_n_s_ParsedUnionMember, __pyx_k_ParsedUnionMember, sizeof(__pyx_k_ParsedUnionMember), 0, 0, 1, 1},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_TypeEnforcementError, __pyx_k_TypeEnforcementError, sizeof(__pyx_k_TypeEnforcementError), 0, 0, 1, 1},
-  {&__pyx_kp_u_Unsupported_Generic_Alias_origin, __pyx_k_Unsupported_Generic_Alias_origin, sizeof(__pyx_k_Unsupported_Generic_Alias_origin), 0, 1, 0, 0},
-  {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
-  {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
   {&__pyx_n_s_actual_type, __pyx_k_actual_type, sizeof(__pyx_k_actual_type), 0, 0, 1, 1},
-  {&__pyx_n_s_annotation, __pyx_k_annotation, sizeof(__pyx_k_annotation), 0, 0, 1, 1},
-  {&__pyx_n_s_annotations, __pyx_k_annotations, sizeof(__pyx_k_annotations), 0, 0, 1, 1},
-  {&__pyx_n_s_auto_cast, __pyx_k_auto_cast, sizeof(__pyx_k_auto_cast), 0, 0, 1, 1},
-  {&__pyx_n_s_class, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
   {&__pyx_n_s_class_name, __pyx_k_class_name, sizeof(__pyx_k_class_name), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_enforce, __pyx_k_enforce, sizeof(__pyx_k_enforce), 0, 0, 1, 1},
-  {&__pyx_kp_u_failed_to_cast_to, __pyx_k_failed_to_cast_to, sizeof(__pyx_k_failed_to_cast_to), 0, 1, 0, 0},
-  {&__pyx_n_s_generic_alias, __pyx_k_generic_alias, sizeof(__pyx_k_generic_alias), 0, 0, 1, 1},
-  {&__pyx_n_s_get, __pyx_k_get, sizeof(__pyx_k_get), 0, 0, 1, 1},
-  {&__pyx_n_s_get_args, __pyx_k_get_args, sizeof(__pyx_k_get_args), 0, 0, 1, 1},
-  {&__pyx_n_s_get_origin, __pyx_k_get_origin, sizeof(__pyx_k_get_origin), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-  {&__pyx_n_s_isnumeric, __pyx_k_isnumeric, sizeof(__pyx_k_isnumeric), 0, 0, 1, 1},
-  {&__pyx_n_s_keys, __pyx_k_keys, sizeof(__pyx_k_keys), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-  {&__pyx_n_s_member_name, __pyx_k_member_name, sizeof(__pyx_k_member_name), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
   {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_ParsedListMember, __pyx_k_pyx_unpickle_ParsedListMember, sizeof(__pyx_k_pyx_unpickle_ParsedListMember), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_ParsedMember, __pyx_k_pyx_unpickle_ParsedMember, sizeof(__pyx_k_pyx_unpickle_ParsedMember), 0, 0, 1, 1},
+  {&__pyx_n_s_pyx_unpickle_ParsedUnionMember, __pyx_k_pyx_unpickle_ParsedUnionMember, sizeof(__pyx_k_pyx_unpickle_ParsedUnionMember), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
-  {&__pyx_n_s_requested_type, __pyx_k_requested_type, sizeof(__pyx_k_requested_type), 0, 0, 1, 1},
+  {&__pyx_n_s_requested_types, __pyx_k_requested_types, sizeof(__pyx_k_requested_types), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
-  {&__pyx_n_s_tenforce_enforcer, __pyx_k_tenforce_enforcer, sizeof(__pyx_k_tenforce_enforcer), 0, 0, 1, 1},
   {&__pyx_n_s_tenforce_exceptions, __pyx_k_tenforce_exceptions, sizeof(__pyx_k_tenforce_exceptions), 0, 0, 1, 1},
+  {&__pyx_n_s_tenforce_lib_members, __pyx_k_tenforce_lib_members, sizeof(__pyx_k_tenforce_lib_members), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-  {&__pyx_n_s_types, __pyx_k_types, sizeof(__pyx_k_types), 0, 0, 1, 1},
-  {&__pyx_n_s_typing, __pyx_k_typing, sizeof(__pyx_k_typing), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_var_name, __pyx_k_var_name, sizeof(__pyx_k_var_name), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 46, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 29, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -5783,18 +5327,21 @@
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x2b52d43, 0x2bacb3c, 0xa433fcf):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x2b52d43, 0x2bacb3c, 0xa433fcf) = (actual_type, annotated_type, class_name, member_name, obj))" % __pyx_checksum)
  */
-  __pyx_tuple__4 = PyTuple_Pack(3, __pyx_int_45428035, __pyx_int_45796156, __pyx_int_172179407); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(3, __pyx_int_45428035, __pyx_int_45796156, __pyx_int_172179407); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_tuple__4 = PyTuple_Pack(3, __pyx_int_219076544, __pyx_int_194537873, __pyx_int_98400706); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_tuple__5 = PyTuple_Pack(3, __pyx_int_219076544, __pyx_int_194537873, __pyx_int_98400706); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(3, __pyx_int_160897390, __pyx_int_86101862, __pyx_int_172471272); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_ParsedMember(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
@@ -5803,28 +5350,34 @@
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
   __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_ParsedMember, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__8 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
   __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_ParsedListMember, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_ParsedUnionMember, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  __pyx_umethod_PyDict_Type_get.type = (PyObject*)&PyDict_Type;
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_45428035 = PyInt_FromLong(45428035L); if (unlikely(!__pyx_int_45428035)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_45796156 = PyInt_FromLong(45796156L); if (unlikely(!__pyx_int_45796156)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_86101862 = PyInt_FromLong(86101862L); if (unlikely(!__pyx_int_86101862)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_98400706 = PyInt_FromLong(98400706L); if (unlikely(!__pyx_int_98400706)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_160897390 = PyInt_FromLong(160897390L); if (unlikely(!__pyx_int_160897390)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_172179407 = PyInt_FromLong(172179407L); if (unlikely(!__pyx_int_172179407)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_172471272 = PyInt_FromLong(172471272L); if (unlikely(!__pyx_int_172471272)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_194537873 = PyInt_FromLong(194537873L); if (unlikely(!__pyx_int_194537873)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_219076544 = PyInt_FromLong(219076544L); if (unlikely(!__pyx_int_219076544)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
@@ -5863,40 +5416,53 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  __pyx_vtabptr_8tenforce_8enforcer_ParsedMember = &__pyx_vtable_8tenforce_8enforcer_ParsedMember;
-  __pyx_vtable_8tenforce_8enforcer_ParsedMember.enforce = (PyObject *(*)(struct __pyx_obj_8tenforce_8enforcer_ParsedMember *, int __pyx_skip_dispatch))__pyx_f_8tenforce_8enforcer_12ParsedMember_enforce;
-  if (PyType_Ready(&__pyx_type_8tenforce_8enforcer_ParsedMember) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  __pyx_vtabptr_8tenforce_3lib_7members_ParsedMember = &__pyx_vtable_8tenforce_3lib_7members_ParsedMember;
+  __pyx_vtable_8tenforce_3lib_7members_ParsedMember.enforce = (PyObject *(*)(struct __pyx_obj_8tenforce_3lib_7members_ParsedMember *, int __pyx_skip_dispatch))__pyx_f_8tenforce_3lib_7members_12ParsedMember_enforce;
+  if (PyType_Ready(&__pyx_type_8tenforce_3lib_7members_ParsedMember) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_8tenforce_8enforcer_ParsedMember.tp_print = 0;
+  __pyx_type_8tenforce_3lib_7members_ParsedMember.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8tenforce_8enforcer_ParsedMember.tp_dictoffset && __pyx_type_8tenforce_8enforcer_ParsedMember.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_8tenforce_8enforcer_ParsedMember.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8tenforce_3lib_7members_ParsedMember.tp_dictoffset && __pyx_type_8tenforce_3lib_7members_ParsedMember.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_8tenforce_3lib_7members_ParsedMember.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_8tenforce_8enforcer_ParsedMember.tp_dict, __pyx_vtabptr_8tenforce_8enforcer_ParsedMember) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ParsedMember, (PyObject *)&__pyx_type_8tenforce_8enforcer_ParsedMember) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8tenforce_8enforcer_ParsedMember) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
-  __pyx_ptype_8tenforce_8enforcer_ParsedMember = &__pyx_type_8tenforce_8enforcer_ParsedMember;
-  __pyx_vtabptr_8tenforce_8enforcer_ParsedListMember = &__pyx_vtable_8tenforce_8enforcer_ParsedListMember;
-  __pyx_vtable_8tenforce_8enforcer_ParsedListMember.enforce = (PyObject *(*)(struct __pyx_obj_8tenforce_8enforcer_ParsedListMember *, int __pyx_skip_dispatch))__pyx_f_8tenforce_8enforcer_16ParsedListMember_enforce;
-  if (PyType_Ready(&__pyx_type_8tenforce_8enforcer_ParsedListMember) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_8tenforce_3lib_7members_ParsedMember.tp_dict, __pyx_vtabptr_8tenforce_3lib_7members_ParsedMember) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ParsedMember, (PyObject *)&__pyx_type_8tenforce_3lib_7members_ParsedMember) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8tenforce_3lib_7members_ParsedMember) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_ptype_8tenforce_3lib_7members_ParsedMember = &__pyx_type_8tenforce_3lib_7members_ParsedMember;
+  __pyx_vtabptr_8tenforce_3lib_7members_ParsedListMember = &__pyx_vtable_8tenforce_3lib_7members_ParsedListMember;
+  __pyx_vtable_8tenforce_3lib_7members_ParsedListMember.enforce = (PyObject *(*)(struct __pyx_obj_8tenforce_3lib_7members_ParsedListMember *, int __pyx_skip_dispatch))__pyx_f_8tenforce_3lib_7members_16ParsedListMember_enforce;
+  if (PyType_Ready(&__pyx_type_8tenforce_3lib_7members_ParsedListMember) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_8tenforce_8enforcer_ParsedListMember.tp_print = 0;
+  __pyx_type_8tenforce_3lib_7members_ParsedListMember.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8tenforce_8enforcer_ParsedListMember.tp_dictoffset && __pyx_type_8tenforce_8enforcer_ParsedListMember.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_8tenforce_8enforcer_ParsedListMember.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8tenforce_3lib_7members_ParsedListMember.tp_dictoffset && __pyx_type_8tenforce_3lib_7members_ParsedListMember.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_8tenforce_3lib_7members_ParsedListMember.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_8tenforce_8enforcer_ParsedListMember.tp_dict, __pyx_vtabptr_8tenforce_8enforcer_ParsedListMember) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ParsedListMember, (PyObject *)&__pyx_type_8tenforce_8enforcer_ParsedListMember) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8tenforce_8enforcer_ParsedListMember) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
-  __pyx_ptype_8tenforce_8enforcer_ParsedListMember = &__pyx_type_8tenforce_8enforcer_ParsedListMember;
+  if (__Pyx_SetVtable(__pyx_type_8tenforce_3lib_7members_ParsedListMember.tp_dict, __pyx_vtabptr_8tenforce_3lib_7members_ParsedListMember) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ParsedListMember, (PyObject *)&__pyx_type_8tenforce_3lib_7members_ParsedListMember) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8tenforce_3lib_7members_ParsedListMember) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_ptype_8tenforce_3lib_7members_ParsedListMember = &__pyx_type_8tenforce_3lib_7members_ParsedListMember;
+  __pyx_vtabptr_8tenforce_3lib_7members_ParsedUnionMember = &__pyx_vtable_8tenforce_3lib_7members_ParsedUnionMember;
+  __pyx_vtable_8tenforce_3lib_7members_ParsedUnionMember.enforce = (PyObject *(*)(struct __pyx_obj_8tenforce_3lib_7members_ParsedUnionMember *, int __pyx_skip_dispatch))__pyx_f_8tenforce_3lib_7members_17ParsedUnionMember_enforce;
+  if (PyType_Ready(&__pyx_type_8tenforce_3lib_7members_ParsedUnionMember) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
+  #if PY_VERSION_HEX < 0x030800B1
+  __pyx_type_8tenforce_3lib_7members_ParsedUnionMember.tp_print = 0;
+  #endif
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8tenforce_3lib_7members_ParsedUnionMember.tp_dictoffset && __pyx_type_8tenforce_3lib_7members_ParsedUnionMember.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_8tenforce_3lib_7members_ParsedUnionMember.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  }
+  if (__Pyx_SetVtable(__pyx_type_8tenforce_3lib_7members_ParsedUnionMember.tp_dict, __pyx_vtabptr_8tenforce_3lib_7members_ParsedUnionMember) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ParsedUnionMember, (PyObject *)&__pyx_type_8tenforce_3lib_7members_ParsedUnionMember) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8tenforce_3lib_7members_ParsedUnionMember) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_ptype_8tenforce_3lib_7members_ParsedUnionMember = &__pyx_type_8tenforce_3lib_7members_ParsedUnionMember;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -5939,19 +5505,19 @@
 #else
 #define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
-__Pyx_PyMODINIT_FUNC initenforcer(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC initenforcer(void)
+__Pyx_PyMODINIT_FUNC initmembers(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC initmembers(void)
 #else
-__Pyx_PyMODINIT_FUNC PyInit_enforcer(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC PyInit_enforcer(void)
+__Pyx_PyMODINIT_FUNC PyInit_members(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC PyInit_members(void)
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 {
   return PyModuleDef_Init(&__pyx_moduledef);
 }
 static CYTHON_SMALL_CODE int __Pyx_check_single_interpreter(void) {
     #if PY_VERSION_HEX >= 0x030700A1
     static PY_INT64_T main_interpreter_id = -1;
@@ -6010,43 +5576,43 @@
     return module;
 bad:
     Py_XDECREF(module);
     return NULL;
 }
 
 
-static CYTHON_SMALL_CODE int __pyx_pymod_exec_enforcer(PyObject *__pyx_pyinit_module)
+static CYTHON_SMALL_CODE int __pyx_pymod_exec_members(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
-    PyErr_SetString(PyExc_RuntimeError, "Module 'enforcer' has already been imported. Re-initialisation is not supported.");
+    PyErr_SetString(PyExc_RuntimeError, "Module 'members' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
-  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_enforcer(void)", 0);
+  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_members(void)", 0);
   if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -6075,15 +5641,15 @@
   #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("enforcer", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  __pyx_m = Py_InitModule4("members", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   #endif
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
@@ -6093,22 +5659,22 @@
   Py_INCREF(__pyx_cython_runtime);
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_tenforce__enforcer) {
+  if (__pyx_module_is_main_tenforce__lib__members) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "tenforce.enforcer")) {
-      if (unlikely(PyDict_SetItemString(modules, "tenforce.enforcer", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "tenforce.lib.members")) {
+      if (unlikely(PyDict_SetItemString(modules, "tenforce.lib.members", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -6121,119 +5687,88 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "tenforce/enforcer.pyx":2
- * #cython: language_level=3
- * import typing             # <<<<<<<<<<<<<<
- * from types import GenericAlias
- * 
- */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_typing, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_typing, __pyx_t_1) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "tenforce/enforcer.pyx":3
- * #cython: language_level=3
- * import typing
- * from types import GenericAlias             # <<<<<<<<<<<<<<
+  /* "tenforce/lib/members.pyx":1
+ * from tenforce.exceptions import TypeEnforcementError             # <<<<<<<<<<<<<<
  * 
- * from tenforce.exceptions import TypeEnforcementError, AutoCastError
+ * cdef class ParsedMember:
  */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_INCREF(__pyx_n_s_GenericAlias);
-  __Pyx_GIVEREF(__pyx_n_s_GenericAlias);
-  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_GenericAlias);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_types, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __Pyx_INCREF(__pyx_n_s_TypeEnforcementError);
+  __Pyx_GIVEREF(__pyx_n_s_TypeEnforcementError);
+  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_TypeEnforcementError);
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_tenforce_exceptions, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_GenericAlias); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_TypeEnforcementError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_GenericAlias, __pyx_t_1) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_TypeEnforcementError, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "tenforce/enforcer.pyx":5
- * from types import GenericAlias
- * 
- * from tenforce.exceptions import TypeEnforcementError, AutoCastError             # <<<<<<<<<<<<<<
- * 
- * cdef class ParsedMember:
- */
-  __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(__pyx_n_s_TypeEnforcementError);
-  __Pyx_GIVEREF(__pyx_n_s_TypeEnforcementError);
-  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_TypeEnforcementError);
-  __Pyx_INCREF(__pyx_n_s_AutoCastError);
-  __Pyx_GIVEREF(__pyx_n_s_AutoCastError);
-  PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_AutoCastError);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_tenforce_exceptions, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_TypeEnforcementError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_TypeEnforcementError, __pyx_t_2) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_AutoCastError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_AutoCastError, __pyx_t_2) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
   /* "(tree fragment)":1
  * def __pyx_unpickle_ParsedMember(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8tenforce_8enforcer_9__pyx_unpickle_ParsedMember, NULL, __pyx_n_s_tenforce_enforcer); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_ParsedMember, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_8tenforce_3lib_7members_1__pyx_unpickle_ParsedMember, NULL, __pyx_n_s_tenforce_lib_members); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_ParsedMember, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_ParsedMember__set_state(<ParsedMember> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_ParsedMember__set_state(ParsedMember __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.actual_type = __pyx_state[0]; __pyx_result.annotated_type = __pyx_state[1]; __pyx_result.class_name = __pyx_state[2]; __pyx_result.member_name = __pyx_state[3]; __pyx_result.obj = __pyx_state[4]
  *     if len(__pyx_state) > 5 and hasattr(__pyx_result, '__dict__'):
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8tenforce_8enforcer_11__pyx_unpickle_ParsedListMember, NULL, __pyx_n_s_tenforce_enforcer); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_ParsedListMember, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_8tenforce_3lib_7members_3__pyx_unpickle_ParsedListMember, NULL, __pyx_n_s_tenforce_lib_members); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_ParsedListMember, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "tenforce/enforcer.pyx":1
- * #cython: language_level=3             # <<<<<<<<<<<<<<
- * import typing
- * from types import GenericAlias
+  /* "(tree fragment)":1
+ * def __pyx_unpickle_ParsedUnionMember(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_8tenforce_3lib_7members_5__pyx_unpickle_ParsedUnionMember, NULL, __pyx_n_s_tenforce_lib_members); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_ParsedUnionMember, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "tenforce/lib/members.pyx":1
+ * from tenforce.exceptions import TypeEnforcementError             # <<<<<<<<<<<<<<
+ * 
+ * cdef class ParsedMember:
+ */
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   if (__pyx_m) {
     if (__pyx_d) {
-      __Pyx_AddTraceback("init tenforce.enforcer", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init tenforce.lib.members", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init tenforce.enforcer");
+    PyErr_SetString(PyExc_ImportError, "init tenforce.lib.members");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
@@ -6912,21 +6447,14 @@
     if (is_list || PySequence_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
-/* PyUnicode_Unicode */
-static CYTHON_INLINE PyObject* __Pyx_PyUnicode_Unicode(PyObject *obj) {
-    if (unlikely(obj == Py_None))
-        obj = __pyx_kp_u_None;
-    return __Pyx_NewRef(obj);
-}
-
 /* CIntToDigits */
 static const char DIGIT_PAIRS_10[2*10*10+1] = {
     "00010203040506070809"
     "10111213141516171819"
     "20212223242526272829"
     "30313233343536373839"
     "40414243444546474849"
@@ -7158,43 +6686,14 @@
 #else
     result_ulength++;
     value_count++;
     return PyUnicode_Join(__pyx_empty_unicode, value_tuple);
 #endif
 }
 
-/* PyObjectCall2Args */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
-    PyObject *args, *result = NULL;
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyFunction_FastCall(function, args, 2);
-    }
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyCFunction_FastCall(function, args, 2);
-    }
-    #endif
-    args = PyTuple_New(2);
-    if (unlikely(!args)) goto done;
-    Py_INCREF(arg1);
-    PyTuple_SET_ITEM(args, 0, arg1);
-    Py_INCREF(arg2);
-    PyTuple_SET_ITEM(args, 1, arg2);
-    Py_INCREF(function);
-    result = __Pyx_PyObject_Call(function, args, NULL);
-    Py_DECREF(args);
-    Py_DECREF(function);
-done:
-    return result;
-}
-
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
     Py_ssize_t num_found)
@@ -7329,617 +6828,14 @@
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
-/* ArgTypeTest */
-static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
-{
-    if (unlikely(!type)) {
-        PyErr_SetString(PyExc_SystemError, "Missing type object");
-        return 0;
-    }
-    else if (exact) {
-        #if PY_MAJOR_VERSION == 2
-        if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
-        #endif
-    }
-    else {
-        if (likely(__Pyx_TypeCheck(obj, type))) return 1;
-    }
-    PyErr_Format(PyExc_TypeError,
-        "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
-        name, type->tp_name, Py_TYPE(obj)->tp_name);
-    return 0;
-}
-
-/* SetItemInt */
-static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v) {
-    int r;
-    if (!j) return -1;
-    r = PyObject_SetItem(o, j, v);
-    Py_DECREF(j);
-    return r;
-}
-static CYTHON_INLINE int __Pyx_SetItemInt_Fast(PyObject *o, Py_ssize_t i, PyObject *v, int is_list,
-                                               CYTHON_NCP_UNUSED int wraparound, CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
-    if (is_list || PyList_CheckExact(o)) {
-        Py_ssize_t n = (!wraparound) ? i : ((likely(i >= 0)) ? i : i + PyList_GET_SIZE(o));
-        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o)))) {
-            PyObject* old = PyList_GET_ITEM(o, n);
-            Py_INCREF(v);
-            PyList_SET_ITEM(o, n, v);
-            Py_DECREF(old);
-            return 1;
-        }
-    } else {
-        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
-        if (likely(m && m->sq_ass_item)) {
-            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
-                Py_ssize_t l = m->sq_length(o);
-                if (likely(l >= 0)) {
-                    i += l;
-                } else {
-                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
-                        return -1;
-                    PyErr_Clear();
-                }
-            }
-            return m->sq_ass_item(o, i, v);
-        }
-    }
-#else
-#if CYTHON_COMPILING_IN_PYPY
-    if (is_list || (PySequence_Check(o) && !PyDict_Check(o)))
-#else
-    if (is_list || PySequence_Check(o))
-#endif
-    {
-        return PySequence_SetItem(o, i, v);
-    }
-#endif
-    return __Pyx_SetItemInt_Generic(o, PyInt_FromSsize_t(i), v);
-}
-
-/* IterFinish */
-static CYTHON_INLINE int __Pyx_IterFinish(void) {
-#if CYTHON_FAST_THREAD_STATE
-    PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject* exc_type = tstate->curexc_type;
-    if (unlikely(exc_type)) {
-        if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) {
-            PyObject *exc_value, *exc_tb;
-            exc_value = tstate->curexc_value;
-            exc_tb = tstate->curexc_traceback;
-            tstate->curexc_type = 0;
-            tstate->curexc_value = 0;
-            tstate->curexc_traceback = 0;
-            Py_DECREF(exc_type);
-            Py_XDECREF(exc_value);
-            Py_XDECREF(exc_tb);
-            return 0;
-        } else {
-            return -1;
-        }
-    }
-    return 0;
-#else
-    if (unlikely(PyErr_Occurred())) {
-        if (likely(PyErr_ExceptionMatches(PyExc_StopIteration))) {
-            PyErr_Clear();
-            return 0;
-        } else {
-            return -1;
-        }
-    }
-    return 0;
-#endif
-}
-
-/* PyObjectGetMethod */
-static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
-    PyObject *attr;
-#if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
-    PyTypeObject *tp = Py_TYPE(obj);
-    PyObject *descr;
-    descrgetfunc f = NULL;
-    PyObject **dictptr, *dict;
-    int meth_found = 0;
-    assert (*method == NULL);
-    if (unlikely(tp->tp_getattro != PyObject_GenericGetAttr)) {
-        attr = __Pyx_PyObject_GetAttrStr(obj, name);
-        goto try_unpack;
-    }
-    if (unlikely(tp->tp_dict == NULL) && unlikely(PyType_Ready(tp) < 0)) {
-        return 0;
-    }
-    descr = _PyType_Lookup(tp, name);
-    if (likely(descr != NULL)) {
-        Py_INCREF(descr);
-#if PY_MAJOR_VERSION >= 3
-        #ifdef __Pyx_CyFunction_USED
-        if (likely(PyFunction_Check(descr) || (Py_TYPE(descr) == &PyMethodDescr_Type) || __Pyx_CyFunction_Check(descr)))
-        #else
-        if (likely(PyFunction_Check(descr) || (Py_TYPE(descr) == &PyMethodDescr_Type)))
-        #endif
-#else
-        #ifdef __Pyx_CyFunction_USED
-        if (likely(PyFunction_Check(descr) || __Pyx_CyFunction_Check(descr)))
-        #else
-        if (likely(PyFunction_Check(descr)))
-        #endif
-#endif
-        {
-            meth_found = 1;
-        } else {
-            f = Py_TYPE(descr)->tp_descr_get;
-            if (f != NULL && PyDescr_IsData(descr)) {
-                attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
-                Py_DECREF(descr);
-                goto try_unpack;
-            }
-        }
-    }
-    dictptr = _PyObject_GetDictPtr(obj);
-    if (dictptr != NULL && (dict = *dictptr) != NULL) {
-        Py_INCREF(dict);
-        attr = __Pyx_PyDict_GetItemStr(dict, name);
-        if (attr != NULL) {
-            Py_INCREF(attr);
-            Py_DECREF(dict);
-            Py_XDECREF(descr);
-            goto try_unpack;
-        }
-        Py_DECREF(dict);
-    }
-    if (meth_found) {
-        *method = descr;
-        return 1;
-    }
-    if (f != NULL) {
-        attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
-        Py_DECREF(descr);
-        goto try_unpack;
-    }
-    if (descr != NULL) {
-        *method = descr;
-        return 0;
-    }
-    PyErr_Format(PyExc_AttributeError,
-#if PY_MAJOR_VERSION >= 3
-                 "'%.50s' object has no attribute '%U'",
-                 tp->tp_name, name);
-#else
-                 "'%.50s' object has no attribute '%.400s'",
-                 tp->tp_name, PyString_AS_STRING(name));
-#endif
-    return 0;
-#else
-    attr = __Pyx_PyObject_GetAttrStr(obj, name);
-    goto try_unpack;
-#endif
-try_unpack:
-#if CYTHON_UNPACK_METHODS
-    if (likely(attr) && PyMethod_Check(attr) && likely(PyMethod_GET_SELF(attr) == obj)) {
-        PyObject *function = PyMethod_GET_FUNCTION(attr);
-        Py_INCREF(function);
-        Py_DECREF(attr);
-        *method = function;
-        return 1;
-    }
-#endif
-    *method = attr;
-    return 0;
-}
-
-/* PyObjectCallMethod0 */
-static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name) {
-    PyObject *method = NULL, *result = NULL;
-    int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
-    if (likely(is_method)) {
-        result = __Pyx_PyObject_CallOneArg(method, obj);
-        Py_DECREF(method);
-        return result;
-    }
-    if (unlikely(!method)) goto bad;
-    result = __Pyx_PyObject_CallNoArg(method);
-    Py_DECREF(method);
-bad:
-    return result;
-}
-
-/* RaiseNeedMoreValuesToUnpack */
-static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index) {
-    PyErr_Format(PyExc_ValueError,
-                 "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
-                 index, (index == 1) ? "" : "s");
-}
-
-/* RaiseTooManyValuesToUnpack */
-static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
-    PyErr_Format(PyExc_ValueError,
-                 "too many values to unpack (expected %" CYTHON_FORMAT_SSIZE_T "d)", expected);
-}
-
-/* UnpackItemEndCheck */
-static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
-    if (unlikely(retval)) {
-        Py_DECREF(retval);
-        __Pyx_RaiseTooManyValuesError(expected);
-        return -1;
-    }
-    return __Pyx_IterFinish();
-}
-
-/* RaiseNoneIterError */
-static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-}
-
-/* UnpackTupleError */
-static void __Pyx_UnpackTupleError(PyObject *t, Py_ssize_t index) {
-    if (t == Py_None) {
-      __Pyx_RaiseNoneNotIterableError();
-    } else if (PyTuple_GET_SIZE(t) < index) {
-      __Pyx_RaiseNeedMoreValuesError(PyTuple_GET_SIZE(t));
-    } else {
-      __Pyx_RaiseTooManyValuesError(index);
-    }
-}
-
-/* UnpackTuple2 */
-static CYTHON_INLINE int __Pyx_unpack_tuple2_exact(
-        PyObject* tuple, PyObject** pvalue1, PyObject** pvalue2, int decref_tuple) {
-    PyObject *value1 = NULL, *value2 = NULL;
-#if CYTHON_COMPILING_IN_PYPY
-    value1 = PySequence_ITEM(tuple, 0);  if (unlikely(!value1)) goto bad;
-    value2 = PySequence_ITEM(tuple, 1);  if (unlikely(!value2)) goto bad;
-#else
-    value1 = PyTuple_GET_ITEM(tuple, 0);  Py_INCREF(value1);
-    value2 = PyTuple_GET_ITEM(tuple, 1);  Py_INCREF(value2);
-#endif
-    if (decref_tuple) {
-        Py_DECREF(tuple);
-    }
-    *pvalue1 = value1;
-    *pvalue2 = value2;
-    return 0;
-#if CYTHON_COMPILING_IN_PYPY
-bad:
-    Py_XDECREF(value1);
-    Py_XDECREF(value2);
-    if (decref_tuple) { Py_XDECREF(tuple); }
-    return -1;
-#endif
-}
-static int __Pyx_unpack_tuple2_generic(PyObject* tuple, PyObject** pvalue1, PyObject** pvalue2,
-                                       int has_known_size, int decref_tuple) {
-    Py_ssize_t index;
-    PyObject *value1 = NULL, *value2 = NULL, *iter = NULL;
-    iternextfunc iternext;
-    iter = PyObject_GetIter(tuple);
-    if (unlikely(!iter)) goto bad;
-    if (decref_tuple) { Py_DECREF(tuple); tuple = NULL; }
-    iternext = Py_TYPE(iter)->tp_iternext;
-    value1 = iternext(iter); if (unlikely(!value1)) { index = 0; goto unpacking_failed; }
-    value2 = iternext(iter); if (unlikely(!value2)) { index = 1; goto unpacking_failed; }
-    if (!has_known_size && unlikely(__Pyx_IternextUnpackEndCheck(iternext(iter), 2))) goto bad;
-    Py_DECREF(iter);
-    *pvalue1 = value1;
-    *pvalue2 = value2;
-    return 0;
-unpacking_failed:
-    if (!has_known_size && __Pyx_IterFinish() == 0)
-        __Pyx_RaiseNeedMoreValuesError(index);
-bad:
-    Py_XDECREF(iter);
-    Py_XDECREF(value1);
-    Py_XDECREF(value2);
-    if (decref_tuple) { Py_XDECREF(tuple); }
-    return -1;
-}
-
-/* dict_iter */
-static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* iterable, int is_dict, PyObject* method_name,
-                                                   Py_ssize_t* p_orig_length, int* p_source_is_dict) {
-    is_dict = is_dict || likely(PyDict_CheckExact(iterable));
-    *p_source_is_dict = is_dict;
-    if (is_dict) {
-#if !CYTHON_COMPILING_IN_PYPY
-        *p_orig_length = PyDict_Size(iterable);
-        Py_INCREF(iterable);
-        return iterable;
-#elif PY_MAJOR_VERSION >= 3
-        static PyObject *py_items = NULL, *py_keys = NULL, *py_values = NULL;
-        PyObject **pp = NULL;
-        if (method_name) {
-            const char *name = PyUnicode_AsUTF8(method_name);
-            if (strcmp(name, "iteritems") == 0) pp = &py_items;
-            else if (strcmp(name, "iterkeys") == 0) pp = &py_keys;
-            else if (strcmp(name, "itervalues") == 0) pp = &py_values;
-            if (pp) {
-                if (!*pp) {
-                    *pp = PyUnicode_FromString(name + 4);
-                    if (!*pp)
-                        return NULL;
-                }
-                method_name = *pp;
-            }
-        }
-#endif
-    }
-    *p_orig_length = 0;
-    if (method_name) {
-        PyObject* iter;
-        iterable = __Pyx_PyObject_CallMethod0(iterable, method_name);
-        if (!iterable)
-            return NULL;
-#if !CYTHON_COMPILING_IN_PYPY
-        if (PyTuple_CheckExact(iterable) || PyList_CheckExact(iterable))
-            return iterable;
-#endif
-        iter = PyObject_GetIter(iterable);
-        Py_DECREF(iterable);
-        return iter;
-    }
-    return PyObject_GetIter(iterable);
-}
-static CYTHON_INLINE int __Pyx_dict_iter_next(
-        PyObject* iter_obj, CYTHON_NCP_UNUSED Py_ssize_t orig_length, CYTHON_NCP_UNUSED Py_ssize_t* ppos,
-        PyObject** pkey, PyObject** pvalue, PyObject** pitem, int source_is_dict) {
-    PyObject* next_item;
-#if !CYTHON_COMPILING_IN_PYPY
-    if (source_is_dict) {
-        PyObject *key, *value;
-        if (unlikely(orig_length != PyDict_Size(iter_obj))) {
-            PyErr_SetString(PyExc_RuntimeError, "dictionary changed size during iteration");
-            return -1;
-        }
-        if (unlikely(!PyDict_Next(iter_obj, ppos, &key, &value))) {
-            return 0;
-        }
-        if (pitem) {
-            PyObject* tuple = PyTuple_New(2);
-            if (unlikely(!tuple)) {
-                return -1;
-            }
-            Py_INCREF(key);
-            Py_INCREF(value);
-            PyTuple_SET_ITEM(tuple, 0, key);
-            PyTuple_SET_ITEM(tuple, 1, value);
-            *pitem = tuple;
-        } else {
-            if (pkey) {
-                Py_INCREF(key);
-                *pkey = key;
-            }
-            if (pvalue) {
-                Py_INCREF(value);
-                *pvalue = value;
-            }
-        }
-        return 1;
-    } else if (PyTuple_CheckExact(iter_obj)) {
-        Py_ssize_t pos = *ppos;
-        if (unlikely(pos >= PyTuple_GET_SIZE(iter_obj))) return 0;
-        *ppos = pos + 1;
-        next_item = PyTuple_GET_ITEM(iter_obj, pos);
-        Py_INCREF(next_item);
-    } else if (PyList_CheckExact(iter_obj)) {
-        Py_ssize_t pos = *ppos;
-        if (unlikely(pos >= PyList_GET_SIZE(iter_obj))) return 0;
-        *ppos = pos + 1;
-        next_item = PyList_GET_ITEM(iter_obj, pos);
-        Py_INCREF(next_item);
-    } else
-#endif
-    {
-        next_item = PyIter_Next(iter_obj);
-        if (unlikely(!next_item)) {
-            return __Pyx_IterFinish();
-        }
-    }
-    if (pitem) {
-        *pitem = next_item;
-    } else if (pkey && pvalue) {
-        if (__Pyx_unpack_tuple2(next_item, pkey, pvalue, source_is_dict, source_is_dict, 1))
-            return -1;
-    } else if (pkey) {
-        *pkey = next_item;
-    } else {
-        *pvalue = next_item;
-    }
-    return 1;
-}
-
-/* DictGetItem */
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
-    PyObject *value;
-    value = PyDict_GetItemWithError(d, key);
-    if (unlikely(!value)) {
-        if (!PyErr_Occurred()) {
-            if (unlikely(PyTuple_Check(key))) {
-                PyObject* args = PyTuple_Pack(1, key);
-                if (likely(args)) {
-                    PyErr_SetObject(PyExc_KeyError, args);
-                    Py_DECREF(args);
-                }
-            } else {
-                PyErr_SetObject(PyExc_KeyError, key);
-            }
-        }
-        return NULL;
-    }
-    Py_INCREF(value);
-    return value;
-}
-#endif
-
-/* UnpackUnboundCMethod */
-static int __Pyx_TryUnpackUnboundCMethod(__Pyx_CachedCFunction* target) {
-    PyObject *method;
-    method = __Pyx_PyObject_GetAttrStr(target->type, *target->method_name);
-    if (unlikely(!method))
-        return -1;
-    target->method = method;
-#if CYTHON_COMPILING_IN_CPYTHON
-    #if PY_MAJOR_VERSION >= 3
-    if (likely(__Pyx_TypeCheck(method, &PyMethodDescr_Type)))
-    #endif
-    {
-        PyMethodDescrObject *descr = (PyMethodDescrObject*) method;
-        target->func = descr->d_method->ml_meth;
-        target->flag = descr->d_method->ml_flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_STACKLESS);
-    }
-#endif
-    return 0;
-}
-
-/* CallUnboundCMethod1 */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg) {
-    if (likely(cfunc->func)) {
-        int flag = cfunc->flag;
-        if (flag == METH_O) {
-            return (*(cfunc->func))(self, arg);
-        } else if (PY_VERSION_HEX >= 0x030600B1 && flag == METH_FASTCALL) {
-            #if PY_VERSION_HEX >= 0x030700A0
-                return (*(__Pyx_PyCFunctionFast)(void*)(PyCFunction)cfunc->func)(self, &arg, 1);
-            #else
-                return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
-            #endif
-        } else if (PY_VERSION_HEX >= 0x030700A0 && flag == (METH_FASTCALL | METH_KEYWORDS)) {
-            return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
-        }
-    }
-    return __Pyx__CallUnboundCMethod1(cfunc, self, arg);
-}
-#endif
-static PyObject* __Pyx__CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg){
-    PyObject *args, *result = NULL;
-    if (unlikely(!cfunc->func && !cfunc->method) && unlikely(__Pyx_TryUnpackUnboundCMethod(cfunc) < 0)) return NULL;
-#if CYTHON_COMPILING_IN_CPYTHON
-    if (cfunc->func && (cfunc->flag & METH_VARARGS)) {
-        args = PyTuple_New(1);
-        if (unlikely(!args)) goto bad;
-        Py_INCREF(arg);
-        PyTuple_SET_ITEM(args, 0, arg);
-        if (cfunc->flag & METH_KEYWORDS)
-            result = (*(PyCFunctionWithKeywords)(void*)(PyCFunction)cfunc->func)(self, args, NULL);
-        else
-            result = (*cfunc->func)(self, args);
-    } else {
-        args = PyTuple_New(2);
-        if (unlikely(!args)) goto bad;
-        Py_INCREF(self);
-        PyTuple_SET_ITEM(args, 0, self);
-        Py_INCREF(arg);
-        PyTuple_SET_ITEM(args, 1, arg);
-        result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
-    }
-#else
-    args = PyTuple_Pack(2, self, arg);
-    if (unlikely(!args)) goto bad;
-    result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
-#endif
-bad:
-    Py_XDECREF(args);
-    return result;
-}
-
-/* CallUnboundCMethod2 */
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030600B1
-static CYTHON_INLINE PyObject *__Pyx_CallUnboundCMethod2(__Pyx_CachedCFunction *cfunc, PyObject *self, PyObject *arg1, PyObject *arg2) {
-    if (likely(cfunc->func)) {
-        PyObject *args[2] = {arg1, arg2};
-        if (cfunc->flag == METH_FASTCALL) {
-            #if PY_VERSION_HEX >= 0x030700A0
-            return (*(__Pyx_PyCFunctionFast)(void*)(PyCFunction)cfunc->func)(self, args, 2);
-            #else
-            return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, args, 2, NULL);
-            #endif
-        }
-        #if PY_VERSION_HEX >= 0x030700A0
-        if (cfunc->flag == (METH_FASTCALL | METH_KEYWORDS))
-            return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, args, 2, NULL);
-        #endif
-    }
-    return __Pyx__CallUnboundCMethod2(cfunc, self, arg1, arg2);
-}
-#endif
-static PyObject* __Pyx__CallUnboundCMethod2(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg1, PyObject* arg2){
-    PyObject *args, *result = NULL;
-    if (unlikely(!cfunc->func && !cfunc->method) && unlikely(__Pyx_TryUnpackUnboundCMethod(cfunc) < 0)) return NULL;
-#if CYTHON_COMPILING_IN_CPYTHON
-    if (cfunc->func && (cfunc->flag & METH_VARARGS)) {
-        args = PyTuple_New(2);
-        if (unlikely(!args)) goto bad;
-        Py_INCREF(arg1);
-        PyTuple_SET_ITEM(args, 0, arg1);
-        Py_INCREF(arg2);
-        PyTuple_SET_ITEM(args, 1, arg2);
-        if (cfunc->flag & METH_KEYWORDS)
-            result = (*(PyCFunctionWithKeywords)(void*)(PyCFunction)cfunc->func)(self, args, NULL);
-        else
-            result = (*cfunc->func)(self, args);
-    } else {
-        args = PyTuple_New(3);
-        if (unlikely(!args)) goto bad;
-        Py_INCREF(self);
-        PyTuple_SET_ITEM(args, 0, self);
-        Py_INCREF(arg1);
-        PyTuple_SET_ITEM(args, 1, arg1);
-        Py_INCREF(arg2);
-        PyTuple_SET_ITEM(args, 2, arg2);
-        result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
-    }
-#else
-    args = PyTuple_Pack(3, self, arg1, arg2);
-    if (unlikely(!args)) goto bad;
-    result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
-#endif
-bad:
-    Py_XDECREF(args);
-    return result;
-}
-
-/* dict_getitem_default */
-static PyObject* __Pyx_PyDict_GetItemDefault(PyObject* d, PyObject* key, PyObject* default_value) {
-    PyObject* value;
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-    value = PyDict_GetItemWithError(d, key);
-    if (unlikely(!value)) {
-        if (unlikely(PyErr_Occurred()))
-            return NULL;
-        value = default_value;
-    }
-    Py_INCREF(value);
-    if ((1));
-#else
-    if (PyString_CheckExact(key) || PyUnicode_CheckExact(key) || PyInt_CheckExact(key)) {
-        value = PyDict_GetItem(d, key);
-        if (unlikely(!value)) {
-            value = default_value;
-        }
-        Py_INCREF(value);
-    }
-#endif
-    else {
-        if (default_value == Py_None)
-            value = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyDict_Type_get, d, key);
-        else
-            value = __Pyx_CallUnboundCMethod2(&__pyx_umethod_PyDict_Type_get, d, key, default_value);
-    }
-    return value;
-}
-
 /* Import */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
     PyObject *empty_list = 0;
     PyObject *module = 0;
     PyObject *global_dict = 0;
     PyObject *empty_dict = 0;
     PyObject *list;
@@ -8011,14 +6907,43 @@
         #else
             "cannot import name %S", name);
         #endif
     }
     return value;
 }
 
+/* PyObjectCall2Args */
+static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
+    PyObject *args, *result = NULL;
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(function)) {
+        PyObject *args[2] = {arg1, arg2};
+        return __Pyx_PyFunction_FastCall(function, args, 2);
+    }
+    #endif
+    #if CYTHON_FAST_PYCCALL
+    if (__Pyx_PyFastCFunction_Check(function)) {
+        PyObject *args[2] = {arg1, arg2};
+        return __Pyx_PyCFunction_FastCall(function, args, 2);
+    }
+    #endif
+    args = PyTuple_New(2);
+    if (unlikely(!args)) goto done;
+    Py_INCREF(arg1);
+    PyTuple_SET_ITEM(args, 0, arg1);
+    Py_INCREF(arg2);
+    PyTuple_SET_ITEM(args, 1, arg2);
+    Py_INCREF(function);
+    result = __Pyx_PyObject_Call(function, args, NULL);
+    Py_DECREF(args);
+    Py_DECREF(function);
+done:
+    return result;
+}
+
 /* HasAttr */
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
     PyObject *r;
     if (unlikely(!__Pyx_PyBaseString_Check(n))) {
         PyErr_SetString(PyExc_TypeError,
                         "hasattr(): attribute name must be string");
         return -1;
```

### Comparing `tenforce-0.1.3/tenforce/exceptions.py` & `tenforce-0.1.4/tenforce/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 class TypeEnforcementError(Exception):
-    def __init__(self, class_name: str, var_name: str, requested_type: type, actual_type: type, obj: object):
+    def __init__(self, class_name: str, var_name: str, requested_types: list[type], actual_type: type, obj: object):
         self.class_name = class_name
         self.var_name = var_name
-        self.requested_type = requested_type
+        self.requested_types = requested_types
         self.actual_type = actual_type
         self.obj = obj
 
     def __str__(self):
-        return f"'{self.class_name}.{self.var_name}' is type '{self.actual_type.__name__}', needs type '{self.requested_type.__name__}'. Value is: {self.obj}"
+        return f"'{self.class_name}.{self.var_name}' is type '{self.actual_type.__name__}' & accepts type(s) {[x.__name__ for x in self.requested_types]}. Value is: '{self.obj}'"
 
 
 class AutoCastError(Exception):
     pass
```

### Comparing `tenforce-0.1.3/tenforce.egg-info/PKG-INFO` & `tenforce-0.1.4/tenforce.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: tenforce
-Version: 0.1.3
+Version: 0.1.4
 Summary: Type enforcement for Python
+Author-email: Hunter LaFaille <hunterlafaille@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hunter LaFaille
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -19,14 +20,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+Keywords: type enforcement,validation,fast,types,cython
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Tenforce
 
 **T**ype **enforce**ment for Python.
```

### Comparing `tenforce-0.1.3/tests/test.py` & `tenforce-0.1.4/tests/test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,78 @@
+import gc
 import unittest
+from typing import Any
+
 from pydantic import BaseModel
 
 from tenforce.enforcer import check
 from tenforce.exceptions import TypeEnforcementError
 
 
 class TestClass:
     sku: int
     mfg_part_number: str
     description: str
     image_urls: list[str]
 
 
+class OtherTestClass:
+    sku: int
+    mfg_part_number: str
+    description: str
+
+
+class OtherOtherTestClass:
+    sku: int | None
+    mfg_part_number: str
+    description: str
+
+
 class TestClassPd(BaseModel):
     sku: int
     mfg_part_number: str
     description: str
     image_urls: list[str]
 
 
-class TestValidator(unittest.TestCase):
-    def test_one_billion_tenforce(self):
+class OtherTestClassPd(BaseModel):
+    sku: int
+    mfg_part_number: str
+    description: str
+
+
+class OtherOtherTestClassPd(BaseModel):
+    sku: int | None
+    mfg_part_number: str
+    description: str
+
+
+class TestEnforcer(unittest.TestCase):
+    def test_one_million_tenforce(self):
         """
-        Tests 1 Billion successful validations on TestClass using Tenforce
+        Tests one million successful validations on TestClass using Tenforce
         """
-        for x in range(0, 9_999_999):
+        for x in range(0, 1_000_000):
             test_class = TestClass()
             test_class.sku = 12345
             test_class.mfg_part_number = "ABC"
             test_class.description = "Test Description"
             test_class.image_urls = ["a", "b"]
             check(test_class)
 
-    def test_one_billion_pydantic(self):
+    def test_one_million_pydantic(self):
         """
-        Tests 1 Billion successful validations on TestClasPd using Pydantic
+        Tests one million validations on TestClasPd using Pydantic
         """
-        for x in range(0, 9_999_999):
+        for x in range(0, 1_000_000):
             test_class = TestClassPd(
                 sku=12345,
                 mfg_part_number="ABC",
                 description="Test Description",
-                image_urls=[]
+                image_urls=["a", "b"]
             )
 
     def test_fail(self):
         """
         Try to force a TypeEnforcementError
         """
         try:
@@ -68,7 +95,39 @@
         test_class = TestClass()
         test_class.sku = "12345"
         test_class.mfg_part_number = "ABC"
         test_class.description = "Test Description"
         test_class.image_urls = ["a", "b"]
         check(test_class, auto_cast=True)
 
+    def test_one_million_no_generic_alias_tenforce(self):
+        """
+        Tests one billion successful validations on OtherTestClass using Tenforce
+        """
+        for x in range(0, 1_000_000):
+            test_class = OtherTestClass()
+            test_class.sku = 12345
+            test_class.mfg_part_number = "ABC"
+            test_class.description = "Test Description"
+            check(test_class)
+
+    def test_one_million_no_generic_alias_pydantic(self):
+        """
+        Tests one billion successful validations on OtherTestClassPd using Pydantic
+        """
+        for x in range(0, 1_000_000):
+            test_class = OtherTestClassPd(
+                sku=12345,
+                mfg_part_number="ABC",
+                description="Test Description"
+            )
+
+    def test_optional_field(self):
+        """
+        Tests an optional field
+        """
+        test_class = OtherOtherTestClass()
+        test_class.sku = "ABC"
+        test_class.mfg_part_number = "ABC"
+        test_class.description = "Test Description"
+        test_class.image_urls = [1, 2]
+        check(test_class, auto_cast=True)
```

