# Comparing `tmp/python-datauri-1.1.0.tar.gz` & `tmp/python_datauri-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-datauri-1.1.0.tar", last modified: Mon Dec 13 18:09:34 2021, max compression
+gzip compressed data, was "python_datauri-1.2.0.tar", max compression
```

## Comparing `python-datauri-1.1.0.tar` & `python_datauri-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,7 @@
-drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2021-12-13 18:09:34.000000 python-datauri-1.1.0/
--rw-r--r--   0 flavio.curella   (502) staff       (20)     1211 2020-07-31 14:49:13.000000 python-datauri-1.1.0/LICENSE
--rw-r--r--   0 flavio.curella   (502) staff       (20)       25 2020-07-31 14:49:13.000000 python-datauri-1.1.0/MANIFEST.in
--rw-r--r--   0 flavio.curella   (502) staff       (20)     3506 2021-12-13 18:09:34.000000 python-datauri-1.1.0/PKG-INFO
--rw-r--r--   0 flavio.curella   (502) staff       (20)     2067 2021-01-19 18:04:00.000000 python-datauri-1.1.0/README.rst
-drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2021-12-13 18:09:34.000000 python-datauri-1.1.0/datauri/
--rw-r--r--   0 flavio.curella   (502) staff       (20)     3555 2021-12-13 17:54:03.000000 python-datauri-1.1.0/datauri/__init__.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)      134 2020-07-31 14:49:13.000000 python-datauri-1.1.0/datauri/exceptions.py
-drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2021-12-13 18:09:34.000000 python-datauri-1.1.0/python_datauri.egg-info/
--rw-r--r--   0 flavio.curella   (502) staff       (20)     3506 2021-12-13 18:09:34.000000 python-datauri-1.1.0/python_datauri.egg-info/PKG-INFO
--rw-r--r--   0 flavio.curella   (502) staff       (20)      355 2021-12-13 18:09:34.000000 python-datauri-1.1.0/python_datauri.egg-info/SOURCES.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)        1 2021-12-13 18:09:34.000000 python-datauri-1.1.0/python_datauri.egg-info/dependency_links.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)       14 2021-12-13 18:09:34.000000 python-datauri-1.1.0/python_datauri.egg-info/top_level.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)      140 2021-12-13 18:09:34.000000 python-datauri-1.1.0/setup.cfg
--rw-r--r--   0 flavio.curella   (502) staff       (20)     1209 2021-12-13 18:07:16.000000 python-datauri-1.1.0/setup.py
-drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2021-12-13 18:09:34.000000 python-datauri-1.1.0/tests/
--rw-r--r--   0 flavio.curella   (502) staff       (20)        0 2020-07-31 14:49:13.000000 python-datauri-1.1.0/tests/__init__.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)       19 2020-07-31 14:49:13.000000 python-datauri-1.1.0/tests/test_file.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)       19 2020-07-31 14:49:13.000000 python-datauri-1.1.0/tests/test_file_ebcdic.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)     3324 2020-07-31 14:49:13.000000 python-datauri-1.1.0/tests/test_long_file.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)     6108 2021-01-19 17:35:00.000000 python-datauri-1.1.0/tests/test_parsing.py
+-rw-r--r--   0        0        0     1211 2020-07-31 14:49:13.887654 python_datauri-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2067 2021-01-19 18:04:00.594309 python_datauri-1.2.0/README.rst
+-rw-r--r--   0        0        0     4770 2023-05-24 21:43:12.696296 python_datauri-1.2.0/datauri/__init__.py
+-rw-r--r--   0        0        0      134 2020-07-31 14:49:13.888532 python_datauri-1.2.0/datauri/exceptions.py
+-rw-r--r--   0        0        0      655 2023-05-24 21:45:50.898950 python_datauri-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2795 1970-01-01 00:00:00.000000 python_datauri-1.2.0/setup.py
+-rw-r--r--   0        0        0     2717 1970-01-01 00:00:00.000000 python_datauri-1.2.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python-datauri-1.1.0/LICENSE` & `python_datauri-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-datauri-1.1.0/README.rst` & `python_datauri-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-datauri-1.1.0/datauri/__init__.py` & `python_datauri-1.2.0/datauri/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import mimetypes
 import re
 import textwrap
-
 from base64 import b64decode as decode64
 from base64 import b64encode as encode64
-
 from urllib.parse import quote, unquote
 
 from .exceptions import InvalidCharset, InvalidDataURI, InvalidMimeType
 
 MIMETYPE_REGEX = r"[\w]+\/[\w\-\+\.]+"
 _MIMETYPE_RE = re.compile("^{}$".format(MIMETYPE_REGEX))
 
@@ -61,15 +59,18 @@
 
     def __new__(cls, *args, **kwargs):
         uri = super(DataURI, cls).__new__(cls, *args, **kwargs)
         uri._parse  # Trigger any ValueErrors on instantiation.
         return uri
 
     def __repr__(self):
-        return "DataURI(%s)" % (super(DataURI, self).__repr__(),)
+        truncated = str(self)
+        if len(truncated) > 80:
+            truncated = truncated[:79] + "…"
+        return "DataURI(%s)" % (truncated,)
 
     def wrap(self, width=76):
         return "\n".join(textwrap.wrap(self, width, break_on_hyphens=False))
 
     @property
     def mimetype(self):
         return self._parse[0]
@@ -97,23 +98,59 @@
     def text(self):
         if self.charset is None:
             raise InvalidCharset("DataURI has no encoding set.")
 
         return self.data.decode(self.charset)
 
     @property
-    def _parse(self):
+    def is_valid(self):
         match = _DATA_URI_RE.match(self)
         if not match:
+            return False
+        return True
+
+    @property
+    def _parse(self):
+        if self.is_valid is False:
             raise InvalidDataURI("Not a valid data URI: %r" % self)
+        match = _DATA_URI_RE.match(self)
         mimetype = match.group("mimetype") or None
         name = match.group("name") or None
         charset = match.group("charset") or None
 
         if match.group("base64"):
             _charset = charset or "utf-8"
             _data = bytes(match.group("data"), _charset)
             data = decode64(_data)
         else:
             data = unquote(match.group("data"))
 
         return mimetype, name, charset, bool(match.group("base64")), data
+
+    # Pydantic methods
+    @classmethod
+    def __get_validators__(cls):
+        # one or more validators may be yielded which will be called in the
+        # order to validate the input, each validator will receive as an input
+        # the value returned from the previous validator
+        yield cls.validate
+
+    @classmethod
+    def validate(cls, v):
+        if not isinstance(v, str):
+            raise TypeError("string required")
+
+        m = cls(v)
+        if not m.is_valid:
+            raise ValueError("invalid data-uri format")
+        return m
+
+    @classmethod
+    def __modify_schema__(cls, field_schema):
+        # __modify_schema__ should mutate the dict it receives in place,
+        # the returned value will be ignored
+        field_schema.update(
+            pattern=DATA_URI_REGEX,
+            examples=[
+                "data:text/plain;charset=utf-8;base64,VGhlIHF1aWNrIGJyb3duIGZveCBqdW1wZWQgb3ZlciB0aGUgbGF6eSBkb2cu"
+            ],
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

