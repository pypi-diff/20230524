# Comparing `tmp/libyang-2.7.0.tar.gz` & `tmp/libyang-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libyang-2.7.0.tar", last modified: Tue Mar 14 08:52:09 2023, max compression
+gzip compressed data, was "libyang-2.7.1.tar", last modified: Wed May 24 13:03:57 2023, max compression
```

## Comparing `libyang-2.7.0.tar` & `libyang-2.7.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:52:09.704025 libyang-2.7.0/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-03-14 08:51:49.000000 libyang-2.7.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      205 2023-03-14 08:51:49.000000 libyang-2.7.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9350 2023-03-14 08:52:09.704025 libyang-2.7.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8769 2023-03-14 08:51:49.000000 libyang-2.7.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:52:09.704025 libyang-2.7.0/cffi/
--rw-r--r--   0 root         (0) root         (0)     1142 2023-03-14 08:51:49.000000 libyang-2.7.0/cffi/build.py
--rw-r--r--   0 root         (0) root         (0)    26589 2023-03-14 08:51:49.000000 libyang-2.7.0/cffi/cdefs.h
--rw-r--r--   0 root         (0) root         (0)      314 2023-03-14 08:51:49.000000 libyang-2.7.0/cffi/source.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:52:09.708025 libyang-2.7.0/libyang/
--rw-r--r--   0 root         (0) root         (0)        6 2023-03-14 08:52:09.708025 libyang-2.7.0/libyang/VERSION
--rw-r--r--   0 root         (0) root         (0)     3183 2023-03-14 08:51:49.000000 libyang-2.7.0/libyang/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14358 2023-03-14 08:51:49.000000 libyang-2.7.0/libyang/context.py
--rw-r--r--   0 root         (0) root         (0)    42242 2023-03-14 08:51:49.000000 libyang-2.7.0/libyang/data.py
--rw-r--r--   0 root         (0) root         (0)    13409 2023-03-14 08:51:49.000000 libyang-2.7.0/libyang/diff.py
--rw-r--r--   0 root         (0) root         (0)     5722 2023-03-14 08:51:49.000000 libyang-2.7.0/libyang/keyed_list.py
--rw-r--r--   0 root         (0) root         (0)     1941 2023-03-14 08:51:49.000000 libyang-2.7.0/libyang/log.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-14 08:51:49.000000 libyang-2.7.0/libyang/py.typed
--rw-r--r--   0 root         (0) root         (0)    44040 2023-03-14 08:51:49.000000 libyang-2.7.0/libyang/schema.py
--rw-r--r--   0 root         (0) root         (0)     3640 2023-03-14 08:51:49.000000 libyang-2.7.0/libyang/util.py
--rw-r--r--   0 root         (0) root         (0)    18831 2023-03-14 08:51:49.000000 libyang-2.7.0/libyang/xpath.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:52:09.704025 libyang-2.7.0/libyang.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9350 2023-03-14 08:52:09.000000 libyang-2.7.0/libyang.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      590 2023-03-14 08:52:09.000000 libyang-2.7.0/libyang.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-14 08:52:09.000000 libyang-2.7.0/libyang.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-14 08:52:09.000000 libyang-2.7.0/libyang.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       50 2023-03-14 08:52:09.000000 libyang-2.7.0/libyang.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-03-14 08:52:09.000000 libyang-2.7.0/libyang.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      289 2023-03-14 08:51:49.000000 libyang-2.7.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      713 2023-03-14 08:52:09.708025 libyang-2.7.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     5815 2023-03-14 08:51:49.000000 libyang-2.7.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:52:09.704025 libyang-2.7.0/tests/
--rw-r--r--   0 root         (0) root         (0)     3722 2023-03-14 08:51:49.000000 libyang-2.7.0/tests/test_context.py
--rw-r--r--   0 root         (0) root         (0)    24778 2023-03-14 08:51:49.000000 libyang-2.7.0/tests/test_data.py
--rw-r--r--   0 root         (0) root         (0)     3935 2023-03-14 08:51:49.000000 libyang-2.7.0/tests/test_diff.py
--rw-r--r--   0 root         (0) root         (0)     3547 2023-03-14 08:51:49.000000 libyang-2.7.0/tests/test_keyedlist.py
--rw-r--r--   0 root         (0) root         (0)    16192 2023-03-14 08:51:49.000000 libyang-2.7.0/tests/test_schema.py
--rw-r--r--   0 root         (0) root         (0)    15307 2023-03-14 08:51:49.000000 libyang-2.7.0/tests/test_xpath.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:03:57.407830 libyang-2.7.1/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-05-24 13:03:32.000000 libyang-2.7.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      205 2023-05-24 13:03:32.000000 libyang-2.7.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9337 2023-05-24 13:03:57.407830 libyang-2.7.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8756 2023-05-24 13:03:32.000000 libyang-2.7.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:03:57.407830 libyang-2.7.1/cffi/
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-05-24 13:03:32.000000 libyang-2.7.1/cffi/build.py
+-rw-r--r--   0 root         (0) root         (0)    26553 2023-05-24 13:03:32.000000 libyang-2.7.1/cffi/cdefs.h
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-24 13:03:32.000000 libyang-2.7.1/cffi/source.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:03:57.411830 libyang-2.7.1/libyang/
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-24 13:03:57.411830 libyang-2.7.1/libyang/VERSION
+-rw-r--r--   0 root         (0) root         (0)     3183 2023-05-24 13:03:32.000000 libyang-2.7.1/libyang/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14358 2023-05-24 13:03:32.000000 libyang-2.7.1/libyang/context.py
+-rw-r--r--   0 root         (0) root         (0)    42242 2023-05-24 13:03:32.000000 libyang-2.7.1/libyang/data.py
+-rw-r--r--   0 root         (0) root         (0)    13409 2023-05-24 13:03:32.000000 libyang-2.7.1/libyang/diff.py
+-rw-r--r--   0 root         (0) root         (0)     5722 2023-05-24 13:03:32.000000 libyang-2.7.1/libyang/keyed_list.py
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-05-24 13:03:32.000000 libyang-2.7.1/libyang/log.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 13:03:32.000000 libyang-2.7.1/libyang/py.typed
+-rw-r--r--   0 root         (0) root         (0)    44040 2023-05-24 13:03:32.000000 libyang-2.7.1/libyang/schema.py
+-rw-r--r--   0 root         (0) root         (0)     3640 2023-05-24 13:03:32.000000 libyang-2.7.1/libyang/util.py
+-rw-r--r--   0 root         (0) root         (0)    18831 2023-05-24 13:03:32.000000 libyang-2.7.1/libyang/xpath.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:03:57.407830 libyang-2.7.1/libyang.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9337 2023-05-24 13:03:57.000000 libyang-2.7.1/libyang.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      590 2023-05-24 13:03:57.000000 libyang-2.7.1/libyang.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 13:03:57.000000 libyang-2.7.1/libyang.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 13:03:57.000000 libyang-2.7.1/libyang.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       50 2023-05-24 13:03:57.000000 libyang-2.7.1/libyang.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-24 13:03:57.000000 libyang-2.7.1/libyang.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      289 2023-05-24 13:03:32.000000 libyang-2.7.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      713 2023-05-24 13:03:57.411830 libyang-2.7.1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     5815 2023-05-24 13:03:32.000000 libyang-2.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:03:57.407830 libyang-2.7.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     3722 2023-05-24 13:03:32.000000 libyang-2.7.1/tests/test_context.py
+-rw-r--r--   0 root         (0) root         (0)    24778 2023-05-24 13:03:32.000000 libyang-2.7.1/tests/test_data.py
+-rw-r--r--   0 root         (0) root         (0)     3935 2023-05-24 13:03:32.000000 libyang-2.7.1/tests/test_diff.py
+-rw-r--r--   0 root         (0) root         (0)     3547 2023-05-24 13:03:32.000000 libyang-2.7.1/tests/test_keyedlist.py
+-rw-r--r--   0 root         (0) root         (0)    16192 2023-05-24 13:03:32.000000 libyang-2.7.1/tests/test_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15307 2023-05-24 13:03:32.000000 libyang-2.7.1/tests/test_xpath.py
```

### Comparing `libyang-2.7.0/LICENSE` & `libyang-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libyang-2.7.0/PKG-INFO` & `libyang-2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libyang
-Version: 2.7.0
+Version: 2.7.1
 Summary: CFFI bindings to libyang
 Home-page: https://github.com/CESNET/libyang-python
 Author: Robin Jarry
 Author-email: robin@jarry.cc
 License: MIT
 Keywords: libyang,cffi
 Classifier: Development Status :: 4 - Beta
@@ -200,15 +200,15 @@
    ...     'data': {
    ...         'hostname': 'foobar',
    ...         'interface': [
    ...             {'name': 'eth0', 'address': '1.2.3.4/24'},
    ...             {'name': 'lo', 'address': '127.0.0.1'},
    ...         ],
    ...     },
-   ... }, config=True)
+   ... })
    >>> print(node.print_mem('xml', pretty=True))
    <data xmlns="urn:example">
      <interface>
        <name>eth0</name>
        <address>1.2.3.4/24</address>
      </interface>
      <interface>
```

### Comparing `libyang-2.7.0/README.rst` & `libyang-2.7.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
    ...     'data': {
    ...         'hostname': 'foobar',
    ...         'interface': [
    ...             {'name': 'eth0', 'address': '1.2.3.4/24'},
    ...             {'name': 'lo', 'address': '127.0.0.1'},
    ...         ],
    ...     },
-   ... }, config=True)
+   ... })
    >>> print(node.print_mem('xml', pretty=True))
    <data xmlns="urn:example">
      <interface>
        <name>eth0</name>
        <address>1.2.3.4/24</address>
      </interface>
      <interface>
```

### Comparing `libyang-2.7.0/cffi/build.py` & `libyang-2.7.1/cffi/build.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.0/cffi/cdefs.h` & `libyang-2.7.1/cffi/cdefs.h`

 * *Files 1% similar despite different names*

```diff
@@ -715,15 +715,14 @@
             struct lyd_node *next;
             struct lyd_node *prev;
             struct lyd_meta *meta;
             void *priv;
         };
     };
     struct lyd_node *child;
-    struct hash_table *children_ht;
     ...;
 };
 
 LY_ERR lyd_validate_all(struct lyd_node **, const struct ly_ctx *, uint32_t, struct lyd_node **);
 LY_ERR lyd_validate_op(struct lyd_node *, const struct lyd_node *, enum lyd_type, struct lyd_node **);
 struct lyd_node* lyd_child_no_keys(const struct lyd_node *);
```

### Comparing `libyang-2.7.0/libyang/__init__.py` & `libyang-2.7.1/libyang/__init__.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.0/libyang/context.py` & `libyang-2.7.1/libyang/context.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.0/libyang/data.py` & `libyang-2.7.1/libyang/data.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.0/libyang/diff.py` & `libyang-2.7.1/libyang/diff.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.0/libyang/keyed_list.py` & `libyang-2.7.1/libyang/keyed_list.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.0/libyang/log.py` & `libyang-2.7.1/libyang/log.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.0/libyang/schema.py` & `libyang-2.7.1/libyang/schema.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.0/libyang/util.py` & `libyang-2.7.1/libyang/util.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.0/libyang/xpath.py` & `libyang-2.7.1/libyang/xpath.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.0/libyang.egg-info/PKG-INFO` & `libyang-2.7.1/libyang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libyang
-Version: 2.7.0
+Version: 2.7.1
 Summary: CFFI bindings to libyang
 Home-page: https://github.com/CESNET/libyang-python
 Author: Robin Jarry
 Author-email: robin@jarry.cc
 License: MIT
 Keywords: libyang,cffi
 Classifier: Development Status :: 4 - Beta
@@ -200,15 +200,15 @@
    ...     'data': {
    ...         'hostname': 'foobar',
    ...         'interface': [
    ...             {'name': 'eth0', 'address': '1.2.3.4/24'},
    ...             {'name': 'lo', 'address': '127.0.0.1'},
    ...         ],
    ...     },
-   ... }, config=True)
+   ... })
    >>> print(node.print_mem('xml', pretty=True))
    <data xmlns="urn:example">
      <interface>
        <name>eth0</name>
        <address>1.2.3.4/24</address>
      </interface>
      <interface>
```

### Comparing `libyang-2.7.0/libyang.egg-info/SOURCES.txt` & `libyang-2.7.1/libyang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libyang-2.7.0/setup.cfg` & `libyang-2.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `libyang-2.7.0/setup.py` & `libyang-2.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.0/tests/test_context.py` & `libyang-2.7.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.0/tests/test_data.py` & `libyang-2.7.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.0/tests/test_diff.py` & `libyang-2.7.1/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.0/tests/test_keyedlist.py` & `libyang-2.7.1/tests/test_keyedlist.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.0/tests/test_schema.py` & `libyang-2.7.1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `libyang-2.7.0/tests/test_xpath.py` & `libyang-2.7.1/tests/test_xpath.py`

 * *Files identical despite different names*

