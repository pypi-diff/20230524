# Comparing `tmp/ard-0.0.8.tar.gz` & `tmp/ard-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ard-0.0.8.tar", last modified: Thu May  6 18:02:33 2021, max compression
+gzip compressed data, was "ard-0.0.9.tar", last modified: Thu May  6 23:14:24 2021, max compression
```

## Comparing `ard-0.0.8.tar` & `ard-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 emblemparade  (1000) emblemparade  (1000)        0 2021-05-06 18:02:33.161369 ard-0.0.8/
--rw-rw-r--   0 emblemparade  (1000) emblemparade  (1000)    11357 2021-04-29 19:11:09.000000 ard-0.0.8/LICENSE
--rw-rw-r--   0 emblemparade  (1000) emblemparade  (1000)     2077 2021-05-06 18:02:33.161369 ard-0.0.8/PKG-INFO
--rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)     1342 2021-05-05 19:29:04.000000 ard-0.0.8/README.md
-drwxrwxr-x   0 emblemparade  (1000) emblemparade  (1000)        0 2021-05-06 18:02:33.160369 ard-0.0.8/ard/
--rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)      272 2021-05-06 16:34:49.000000 ard-0.0.8/ard/__init__.py
--rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)     1653 2021-05-06 17:51:01.000000 ard-0.0.8/ard/cbor.py
--rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)     5361 2021-05-05 17:00:31.000000 ard-0.0.8/ard/cjson.py
--rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)      972 2021-05-05 18:58:16.000000 ard-0.0.8/ard/decode.py
--rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)     1366 2021-05-05 18:58:19.000000 ard-0.0.8/ard/encode.py
--rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)      201 2021-05-05 19:12:00.000000 ard-0.0.8/ard/exceptions.py
--rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)      396 2021-05-05 18:43:20.000000 ard-0.0.8/ard/json.py
--rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)     1593 2021-05-05 19:14:34.000000 ard-0.0.8/ard/read.py
--rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)     7321 2021-05-05 17:24:01.000000 ard-0.0.8/ard/types.py
--rw-rw-r--   0 emblemparade  (1000) emblemparade  (1000)       22 2021-05-06 18:02:29.000000 ard-0.0.8/ard/version.py
--rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)     2054 2021-05-05 19:15:12.000000 ard-0.0.8/ard/write.py
--rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)     1186 2021-05-03 18:50:22.000000 ard-0.0.8/ard/yaml.py
-drwxrwxr-x   0 emblemparade  (1000) emblemparade  (1000)        0 2021-05-06 18:02:33.161369 ard-0.0.8/ard.egg-info/
--rw-rw-r--   0 emblemparade  (1000) emblemparade  (1000)     2077 2021-05-06 18:02:33.000000 ard-0.0.8/ard.egg-info/PKG-INFO
--rw-rw-r--   0 emblemparade  (1000) emblemparade  (1000)      332 2021-05-06 18:02:33.000000 ard-0.0.8/ard.egg-info/SOURCES.txt
--rw-rw-r--   0 emblemparade  (1000) emblemparade  (1000)        1 2021-05-06 18:02:33.000000 ard-0.0.8/ard.egg-info/dependency_links.txt
--rw-rw-r--   0 emblemparade  (1000) emblemparade  (1000)       18 2021-05-06 18:02:33.000000 ard-0.0.8/ard.egg-info/requires.txt
--rw-rw-r--   0 emblemparade  (1000) emblemparade  (1000)        4 2021-05-06 18:02:33.000000 ard-0.0.8/ard.egg-info/top_level.txt
--rwxr-xr-x   0 emblemparade  (1000) emblemparade  (1000)     1709 2021-05-06 17:58:54.000000 ard-0.0.8/ardconv
--rw-rw-r--   0 emblemparade  (1000) emblemparade  (1000)       38 2021-05-06 18:02:33.161369 ard-0.0.8/setup.cfg
--rwxrwxr-x   0 emblemparade  (1000) emblemparade  (1000)      967 2021-05-06 17:40:51.000000 ard-0.0.8/setup.py
+drwxrwxr-x   0 emblemparade  (1000) emblemparade  (1000)        0 2021-05-06 23:14:24.979969 ard-0.0.9/
+-rw-rw-r--   0 emblemparade  (1000) emblemparade  (1000)    11357 2021-04-29 19:11:09.000000 ard-0.0.9/LICENSE
+-rw-rw-r--   0 emblemparade  (1000) emblemparade  (1000)     2077 2021-05-06 23:14:24.979969 ard-0.0.9/PKG-INFO
+-rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)     1342 2021-05-05 19:29:04.000000 ard-0.0.9/README.md
+drwxrwxr-x   0 emblemparade  (1000) emblemparade  (1000)        0 2021-05-06 23:14:24.978969 ard-0.0.9/ard/
+-rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)      272 2021-05-06 16:34:49.000000 ard-0.0.9/ard/__init__.py
+-rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)     1653 2021-05-06 17:51:01.000000 ard-0.0.9/ard/cbor.py
+-rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)     5361 2021-05-05 17:00:31.000000 ard-0.0.9/ard/cjson.py
+-rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)      972 2021-05-05 18:58:16.000000 ard-0.0.9/ard/decode.py
+-rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)     1366 2021-05-05 18:58:19.000000 ard-0.0.9/ard/encode.py
+-rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)      201 2021-05-05 19:12:00.000000 ard-0.0.9/ard/exceptions.py
+-rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)      396 2021-05-05 18:43:20.000000 ard-0.0.9/ard/json.py
+-rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)     1598 2021-05-06 23:06:12.000000 ard-0.0.9/ard/read.py
+-rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)     7321 2021-05-05 17:24:01.000000 ard-0.0.9/ard/types.py
+-rw-rw-r--   0 emblemparade  (1000) emblemparade  (1000)       22 2021-05-06 23:14:21.000000 ard-0.0.9/ard/version.py
+-rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)     2059 2021-05-06 23:06:07.000000 ard-0.0.9/ard/write.py
+-rw-r--r--   0 emblemparade  (1000) emblemparade  (1000)     1186 2021-05-03 18:50:22.000000 ard-0.0.9/ard/yaml.py
+drwxrwxr-x   0 emblemparade  (1000) emblemparade  (1000)        0 2021-05-06 23:14:24.978969 ard-0.0.9/ard.egg-info/
+-rw-rw-r--   0 emblemparade  (1000) emblemparade  (1000)     2077 2021-05-06 23:14:24.000000 ard-0.0.9/ard.egg-info/PKG-INFO
+-rw-rw-r--   0 emblemparade  (1000) emblemparade  (1000)      332 2021-05-06 23:14:24.000000 ard-0.0.9/ard.egg-info/SOURCES.txt
+-rw-rw-r--   0 emblemparade  (1000) emblemparade  (1000)        1 2021-05-06 23:14:24.000000 ard-0.0.9/ard.egg-info/dependency_links.txt
+-rw-rw-r--   0 emblemparade  (1000) emblemparade  (1000)       18 2021-05-06 23:14:24.000000 ard-0.0.9/ard.egg-info/requires.txt
+-rw-rw-r--   0 emblemparade  (1000) emblemparade  (1000)        4 2021-05-06 23:14:24.000000 ard-0.0.9/ard.egg-info/top_level.txt
+-rwxr-xr-x   0 emblemparade  (1000) emblemparade  (1000)     2215 2021-05-06 23:11:19.000000 ard-0.0.9/ardconv
+-rw-rw-r--   0 emblemparade  (1000) emblemparade  (1000)       38 2021-05-06 23:14:24.979969 ard-0.0.9/setup.cfg
+-rwxrwxr-x   0 emblemparade  (1000) emblemparade  (1000)      967 2021-05-06 17:40:51.000000 ard-0.0.9/setup.py
```

### Comparing `ard-0.0.8/LICENSE` & `ard-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ard-0.0.8/PKG-INFO` & `ard-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ard
-Version: 0.0.8
+Version: 0.0.9
 Summary: Agnostic Raw Data for Python
 Home-page: https://github.com/tliron/python-ard
 Author: Tal Liron
 Author-email: tal.liron@gmail.com
 License: Apache License 2.0
 Download-URL: https://github.com/tliron/python-ard/releases
 Description: Agnostic Raw Data for Python
```

### Comparing `ard-0.0.8/README.md` & `ard-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ard-0.0.8/ard/cbor.py` & `ard-0.0.9/ard/cbor.py`

 * *Files identical despite different names*

### Comparing `ard-0.0.8/ard/cjson.py` & `ard-0.0.9/ard/cjson.py`

 * *Files identical despite different names*

### Comparing `ard-0.0.8/ard/decode.py` & `ard-0.0.9/ard/decode.py`

 * *Files identical despite different names*

### Comparing `ard-0.0.8/ard/encode.py` & `ard-0.0.9/ard/encode.py`

 * *Files identical despite different names*

### Comparing `ard-0.0.8/ard/read.py` & `ard-0.0.9/ard/read.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,52 +11,52 @@
     'read_yaml',
     'read_json',
     'read_cjson',
     'read_xml',
     'read_cbor')
 
 
-def read(reader, format='yaml'):
+def read(stream, format='yaml'):
     if (format == 'yaml') or (format == ''):
-        return read_yaml(reader)
+        return read_yaml(stream)
     elif format == 'json':
-        return read_json(reader)
+        return read_json(stream)
     elif format == 'cjson':
-        return read_cjson(reader)
+        return read_cjson(stream)
     elif format == 'xml':
-        return read_xml(reader)
+        return read_xml(stream)
     elif format == 'cbor':
-        return read_cbor(reader)
+        return read_cbor(stream)
     else:
         raise ARDException('unsupported format: ' + format)
 
-def read_yaml(reader):
+def read_yaml(stream):
     try:
         yaml=ruamel.yaml.YAML(typ='safe')
         yaml.Constructor = YAMLSafeConstructor
-        return yaml.load(reader)
+        return yaml.load(stream)
     except Exception as e:
         raise DecodeError('yaml') from e
 
-def read_json(reader):
+def read_json(stream):
     try:
-        return json.load(reader)
+        return json.load(stream)
     except Exception as e:
         raise DecodeError('json') from e
 
-def read_cjson(reader):
-    cjson = read_json(reader)
+def read_cjson(stream):
+    cjson = read_json(stream)
     try:
         return convert_from_cjson(cjson)
     except Exception as e:
         raise DecodeError('cjson') from e
 
-def read_xml(reader):
+def read_xml(stream):
     # TODO
-    raise NotImplementedError()
+    raise NotImplementedError('xml')
 
-def read_cbor(reader):
+def read_cbor(stream):
     try:
-        decoder = cbor2.CBORDecoder(reader)
+        decoder = cbor2.CBORDecoder(stream)
         return convert_frozendicts_to_maps(decoder.decode())
     except Exception as e:
         raise DecodeError('cbor') from e
```

### Comparing `ard-0.0.8/ard/types.py` & `ard-0.0.9/ard/types.py`

 * *Files identical despite different names*

### Comparing `ard-0.0.8/ard/write.py` & `ard-0.0.9/ard/write.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         value = convert_to_cjson(value)
     except Exception as e:
         raise EncodeError('cjson') from e
     write_json(value, writer, indent)
 
 def write_xml(value, writer, indent=''):
     # TODO
-    raise NotImplementedError()
+    raise NotImplementedError('xml')
 
 def write_cbor(value, writer):
     try:
         encoder = cbor2.CBOREncoder(writer, default=cbor_encoder_default)
         encoder.encode(value)
     except Exception as e:
         raise EncodeError('cbor') from e
```

### Comparing `ard-0.0.8/ard/yaml.py` & `ard-0.0.9/ard/yaml.py`

 * *Files identical despite different names*

### Comparing `ard-0.0.8/ard.egg-info/PKG-INFO` & `ard-0.0.9/ard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ard
-Version: 0.0.8
+Version: 0.0.9
 Summary: Agnostic Raw Data for Python
 Home-page: https://github.com/tliron/python-ard
 Author: Tal Liron
 Author-email: tal.liron@gmail.com
 License: Apache License 2.0
 Download-URL: https://github.com/tliron/python-ard/releases
 Description: Agnostic Raw Data for Python
```

### Comparing `ard-0.0.8/ardconv` & `ard-0.0.9/ardconv`

 * *Files 9% similar despite different names*

```diff
@@ -7,44 +7,61 @@
     parser = argparse.ArgumentParser(description='Convert ARD between transmission formats')
     parser.add_argument('--version', '-V', action='store_true', help='show version')
     parser.add_argument('input', type=str, nargs='?', help='input file (stdin if not provided)')
     parser.add_argument('output', type=str, nargs='?', help='output file (stdout if not provided)')
     parser.add_argument('--input', '-i', dest='input_format', type=str, choices=('yaml', 'json', 'cjson', 'xml', 'cbor'), default='yaml', help='input format')
     parser.add_argument('--output', '-o', dest='output_format', type=str, choices=('yaml', 'json', 'cjson', 'xml', 'cbor'), default='yaml', help='output format')
     parser.add_argument('--indent', '-n', type=int, default=2, help='output indentation size')
+    parser.add_argument('--verbose', '-v', action='store_true', help='verbose errors')
     args = parser.parse_args()
 
     if args.version:
         print(ard.__version__)
         sys.exit(0)
 
-    if args.input is not None:
-        input = open(args.input, 'r')
-    else:
-        if args.input_format == 'cbor':
-            input = sys.stdin.buffer
-        else:
-            input = sys.stdin
-
     try:
-        value = ard.read(input, args.input_format)
-    finally:
-        if args.input is not None:
-            input.close()
 
-    if args.output is not None:
-        output = open(args.output, 'w')
-    else:
-        if args.output_format == 'cbor':
-            output = sys.stdout.buffer
+        if args.input is not None:
+            input = open(args.input, 'r')
         else:
-            output = sys.stdout
+            if args.input_format == 'cbor':
+                input = sys.stdin.buffer
+            else:
+                input = sys.stdin
+
+        try:
+            value = ard.read(input, args.input_format)
+        finally:
+            if args.input is not None:
+                input.close()
 
-    try:
-        ard.write(value, output, args.output_format, indent=' ' * args.indent)
-    finally:
         if args.output is not None:
-            output.close()
+            output = open(args.output, 'w')
+        else:
+            if args.output_format == 'cbor':
+                output = sys.stdout.buffer
+            else:
+                output = sys.stdout
+
+        try:
+            ard.write(value, output, args.output_format, indent=' ' * args.indent)
+        finally:
+            if args.output is not None:
+                output.close()
+
+    except KeyboardInterrupt:
+        sys.exit(130)
+
+    except BaseException as e:
+        if args.verbose:
+            raise e
+        else:
+            m = str(e)
+            if m:
+                m = ': ' + m
+            m = type(e).__name__ + m
+            print(m, file=sys.stderr)
+            sys.exit(1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ard-0.0.8/setup.py` & `ard-0.0.9/setup.py`

 * *Files identical despite different names*

