# Comparing `tmp/witness-etl-0.0.5.tar.gz` & `tmp/witness-etl-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "witness-etl-0.0.5.tar", last modified: Thu May 18 16:04:14 2023, max compression
+gzip compressed data, was "witness-etl-0.0.6.tar", last modified: Wed May 24 02:31:14 2023, max compression
```

## Comparing `witness-etl-0.0.5.tar` & `witness-etl-0.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 16:04:14.616954 witness-etl-0.0.5/
--rw-rw-rw-   0        0        0    11558 2022-10-24 01:46:22.000000 witness-etl-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1179 2023-05-18 16:04:14.618392 witness-etl-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      641 2023-05-11 16:29:07.000000 witness-etl-0.0.5/README.md
--rw-rw-rw-   0        0        0      217 2022-10-24 01:46:22.000000 witness-etl-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0     1013 2023-05-18 16:04:14.622405 witness-etl-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-18 16:04:14.426718 witness-etl-0.0.5/tests/
--rw-rw-rw-   0        0        0     1204 2023-05-11 15:36:54.000000 witness-etl-0.0.5/tests/test_batch.py
--rw-rw-rw-   0        0        0     1916 2023-05-11 16:04:37.000000 witness-etl-0.0.5/tests/test_dump.py
--rw-rw-rw-   0        0        0     2415 2023-05-11 11:47:54.000000 witness-etl-0.0.5/tests/test_http_extractors.py
-drwxrwxrwx   0        0        0        0 2023-05-18 16:04:14.447478 witness-etl-0.0.5/witness/
--rw-rw-rw-   0        0        0      959 2023-05-11 09:39:22.000000 witness-etl-0.0.5/witness/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 16:04:14.491371 witness-etl-0.0.5/witness/core/
--rw-rw-rw-   0        0        0      712 2023-05-11 09:39:22.000000 witness-etl-0.0.5/witness/core/__init__.py
--rw-rw-rw-   0        0        0     4046 2023-05-11 11:19:15.000000 witness-etl-0.0.5/witness/core/abstract.py
--rw-rw-rw-   0        0        0     4304 2023-05-11 16:00:54.000000 witness-etl-0.0.5/witness/core/batch.py
--rw-rw-rw-   0        0        0     1810 2023-05-11 16:27:43.000000 witness-etl-0.0.5/witness/core/meta.py
-drwxrwxrwx   0        0        0        0 2023-05-18 16:04:14.529668 witness-etl-0.0.5/witness/extractors/
--rw-rw-rw-   0        0        0      632 2022-10-24 01:46:22.000000 witness-etl-0.0.5/witness/extractors/__init__.py
--rw-rw-rw-   0        0        0     2359 2022-11-24 13:54:30.000000 witness-etl-0.0.5/witness/extractors/database.py
--rw-rw-rw-   0        0        0      861 2023-05-15 09:26:02.000000 witness-etl-0.0.5/witness/extractors/file.py
--rw-rw-rw-   0        0        0     1251 2023-05-11 11:19:15.000000 witness-etl-0.0.5/witness/extractors/http.py
-drwxrwxrwx   0        0        0        0 2023-05-18 16:04:14.532330 witness-etl-0.0.5/witness/loaders/
--rw-rw-rw-   0        0        0      632 2022-10-24 01:46:22.000000 witness-etl-0.0.5/witness/loaders/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 16:04:14.533743 witness-etl-0.0.5/witness/providers/
--rw-rw-rw-   0        0        0        0 2022-11-01 04:30:23.000000 witness-etl-0.0.5/witness/providers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 16:04:14.555180 witness-etl-0.0.5/witness/providers/pandas/
--rw-rw-rw-   0        0        0      630 2023-01-09 04:38:56.000000 witness-etl-0.0.5/witness/providers/pandas/__init__.py
--rw-rw-rw-   0        0        0     3300 2023-05-18 15:51:50.000000 witness-etl-0.0.5/witness/providers/pandas/core.py
--rw-rw-rw-   0        0        0     1500 2023-05-18 15:31:12.000000 witness-etl-0.0.5/witness/providers/pandas/extractors.py
--rw-rw-rw-   0        0        0     2922 2023-05-18 15:51:50.000000 witness-etl-0.0.5/witness/providers/pandas/loaders.py
-drwxrwxrwx   0        0        0        0 2023-05-18 16:04:14.569709 witness-etl-0.0.5/witness/serializers/
--rw-rw-rw-   0        0        0        0 2023-01-09 04:29:12.000000 witness-etl-0.0.5/witness/serializers/__init__.py
--rw-rw-rw-   0        0        0      953 2023-01-12 11:39:38.000000 witness-etl-0.0.5/witness/serializers/http.py
--rw-rw-rw-   0        0        0      997 2022-11-22 11:45:30.000000 witness-etl-0.0.5/witness/version.py
-drwxrwxrwx   0        0        0        0 2023-05-18 16:04:14.615955 witness-etl-0.0.5/witness_etl.egg-info/
--rw-rw-rw-   0        0        0     1179 2023-05-18 16:04:14.000000 witness-etl-0.0.5/witness_etl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      796 2023-05-18 16:04:14.000000 witness-etl-0.0.5/witness_etl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 16:04:14.000000 witness-etl-0.0.5/witness_etl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      145 2023-05-18 16:04:14.000000 witness-etl-0.0.5/witness_etl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-18 16:04:14.000000 witness-etl-0.0.5/witness_etl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 02:31:14.705363 witness-etl-0.0.6/
+-rw-rw-rw-   0        0        0    11558 2022-10-24 01:46:22.000000 witness-etl-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1179 2023-05-24 02:31:14.705363 witness-etl-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2023-05-11 16:29:07.000000 witness-etl-0.0.6/README.md
+-rw-rw-rw-   0        0        0      217 2022-10-24 01:46:22.000000 witness-etl-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1013 2023-05-24 02:31:14.707366 witness-etl-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 02:31:14.518426 witness-etl-0.0.6/tests/
+-rw-rw-rw-   0        0        0     1440 2023-05-24 02:22:58.000000 witness-etl-0.0.6/tests/test_batch.py
+-rw-rw-rw-   0        0        0     1916 2023-05-11 16:04:37.000000 witness-etl-0.0.6/tests/test_dump.py
+-rw-rw-rw-   0        0        0     2418 2023-05-22 03:56:40.000000 witness-etl-0.0.6/tests/test_http_extractors.py
+drwxrwxrwx   0        0        0        0 2023-05-24 02:31:14.524436 witness-etl-0.0.6/witness/
+-rw-rw-rw-   0        0        0      976 2023-05-24 02:22:07.000000 witness-etl-0.0.6/witness/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 02:31:14.545751 witness-etl-0.0.6/witness/core/
+-rw-rw-rw-   0        0        0      712 2023-05-11 09:39:22.000000 witness-etl-0.0.6/witness/core/__init__.py
+-rw-rw-rw-   0        0        0     4045 2023-05-22 03:55:03.000000 witness-etl-0.0.6/witness/core/abstract.py
+-rw-rw-rw-   0        0        0     4415 2023-05-22 03:55:03.000000 witness-etl-0.0.6/witness/core/batch.py
+-rw-rw-rw-   0        0        0     2685 2023-05-24 02:22:07.000000 witness-etl-0.0.6/witness/core/meta.py
+drwxrwxrwx   0        0        0        0 2023-05-24 02:31:14.612938 witness-etl-0.0.6/witness/extractors/
+-rw-rw-rw-   0        0        0      632 2022-10-24 01:46:22.000000 witness-etl-0.0.6/witness/extractors/__init__.py
+-rw-rw-rw-   0        0        0     2358 2023-05-22 03:55:03.000000 witness-etl-0.0.6/witness/extractors/database.py
+-rw-rw-rw-   0        0        0      860 2023-05-22 03:55:03.000000 witness-etl-0.0.6/witness/extractors/file.py
+-rw-rw-rw-   0        0        0     1250 2023-05-22 03:55:03.000000 witness-etl-0.0.6/witness/extractors/http.py
+drwxrwxrwx   0        0        0        0 2023-05-24 02:31:14.624122 witness-etl-0.0.6/witness/loaders/
+-rw-rw-rw-   0        0        0      632 2022-10-24 01:46:22.000000 witness-etl-0.0.6/witness/loaders/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 02:31:14.625603 witness-etl-0.0.6/witness/providers/
+-rw-rw-rw-   0        0        0        0 2022-11-01 04:30:23.000000 witness-etl-0.0.6/witness/providers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 02:31:14.669468 witness-etl-0.0.6/witness/providers/pandas/
+-rw-rw-rw-   0        0        0      630 2023-01-09 04:38:56.000000 witness-etl-0.0.6/witness/providers/pandas/__init__.py
+-rw-rw-rw-   0        0        0     3299 2023-05-22 03:55:03.000000 witness-etl-0.0.6/witness/providers/pandas/core.py
+-rw-rw-rw-   0        0        0     1500 2023-05-18 15:31:12.000000 witness-etl-0.0.6/witness/providers/pandas/extractors.py
+-rw-rw-rw-   0        0        0     2922 2023-05-18 15:51:50.000000 witness-etl-0.0.6/witness/providers/pandas/loaders.py
+drwxrwxrwx   0        0        0        0 2023-05-24 02:31:14.680033 witness-etl-0.0.6/witness/serializers/
+-rw-rw-rw-   0        0        0        0 2023-01-09 04:29:12.000000 witness-etl-0.0.6/witness/serializers/__init__.py
+-rw-rw-rw-   0        0        0      953 2023-01-12 11:39:38.000000 witness-etl-0.0.6/witness/serializers/http.py
+-rw-rw-rw-   0        0        0      997 2023-05-24 02:27:39.000000 witness-etl-0.0.6/witness/version.py
+drwxrwxrwx   0        0        0        0 2023-05-24 02:31:14.704365 witness-etl-0.0.6/witness_etl.egg-info/
+-rw-rw-rw-   0        0        0     1179 2023-05-24 02:31:14.000000 witness-etl-0.0.6/witness_etl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      796 2023-05-24 02:31:14.000000 witness-etl-0.0.6/witness_etl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 02:31:14.000000 witness-etl-0.0.6/witness_etl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      145 2023-05-24 02:31:14.000000 witness-etl-0.0.6/witness_etl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-24 02:31:14.000000 witness-etl-0.0.6/witness_etl.egg-info/top_level.txt
```

### Comparing `witness-etl-0.0.5/LICENSE` & `witness-etl-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.5/PKG-INFO` & `witness-etl-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: witness-etl
-Version: 0.0.5
+Version: 0.0.6
 Summary: A minimal ETL library.
 Author: Eugene Popov
 Author-email: evgeniypalych@gmail.com
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/eppv/witness
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `witness-etl-0.0.5/README.md` & `witness-etl-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.5/setup.cfg` & `witness-etl-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6974 6e65 7373 2d65 746c 0d0a   = witness-etl..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 350d  version = 0.0.5.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 360d  version = 0.0.6.
 00000030: 0a61 7574 686f 7220 3d20 4575 6765 6e65  .author = Eugene
 00000040: 2050 6f70 6f76 0d0a 6175 7468 6f72 5f65   Popov..author_e
 00000050: 6d61 696c 203d 2065 7667 656e 6979 7061  mail = evgeniypa
 00000060: 6c79 6368 4067 6d61 696c 2e63 6f6d 0d0a  lych@gmail.com..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 4120  description = A 
 00000080: 6d69 6e69 6d61 6c20 4554 4c20 6c69 6272  minimal ETL libr
 00000090: 6172 792e 0d0a 6c6f 6e67 5f64 6573 6372  ary...long_descr
```

### Comparing `witness-etl-0.0.5/tests/test_batch.py` & `witness-etl-0.0.6/witness/serializers/http.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,30 @@
-#  Copyright (c) 2022.  Eugene Popov.
+
+#  Copyright (c) 2023.  Eugene Popov.
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #     you may not use this file except in compliance with the License.
 #     You may obtain a copy of the License at
 #
 #         http://www.apache.org/licenses/LICENSE-2.0
 #
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
-from witness import MetaData
-from tests import conftest
-
-calibration_meta = conftest.batch_meta
-calibration_data = conftest.batch_data
-
-def test_info(fxtr_batch):
-    print(fxtr_batch.info())
 
+from witness.core.abstract import AbstractSerializer
+import json
 
-def test_construct_meta(fxtr_batch):
-    constructed_meta = MetaData(**calibration_meta)
-    assert fxtr_batch.meta == constructed_meta
 
+class JsonSerializer(AbstractSerializer):
 
-def test_manual_add_to_meta(fxtr_batch):
-    manual_constructed_meta = MetaData()
-    for k,v in calibration_meta.items():
-        manual_constructed_meta[k] = v
-    assert manual_constructed_meta == fxtr_batch.meta
+    def to_batch(self, raw, *args, **kwargs):
+        data = raw.json()
+        return data
 
+    def from_batch(self, data, *args, **kwargs):
+        raw = json.dumps(data)
+        return raw
```

### Comparing `witness-etl-0.0.5/tests/test_dump.py` & `witness-etl-0.0.6/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.5/tests/test_http_extractors.py` & `witness-etl-0.0.6/tests/test_http_extractors.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,9 +62,9 @@
     full_extractor.unify()
     assert full_extractor.output is not None
     print(full_extractor.output)
     batch = Batch()
     batch.fill(extractor=full_extractor)
     assert batch.data == full_extractor.output['data']
     assert full_extractor.output['meta'] in batch.meta
-    assert 'extraction_timestamp' in batch.meta.keys()
+    assert batch.meta['extraction_timestamp'] is not None
```

### Comparing `witness-etl-0.0.5/witness/__init__.py` & `witness-etl-0.0.6/witness/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
 from .core.batch import Batch
-from .core.meta import MetaData
+from .core.meta import MetaData, MetaJSONEncoder
 from . import version
 
 # Meta
 __version__ = version.version
 __author__ = 'Eugene Popov'
```

### Comparing `witness-etl-0.0.5/witness/core/__init__.py` & `witness-etl-0.0.6/witness/core/__init__.py`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.5/witness/core/abstract.py` & `witness-etl-0.0.6/witness/core/abstract.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
         self.uri = uri
         self.output = None
         self.extraction_timestamp: Optional[pendulum.DateTime] = None
         self.serializer: Optional[AbstractSerializer] = None
         self.is_unified = False
 
-    def _set_extraction_timestamp(self):
+    def set_extraction_timestamp(self):
         setattr(self, 'extraction_timestamp', pendulum.now())
 
     def _set_unified_true(self):
         setattr(self, 'is_unified', True)
 
     @abstractmethod
     def extract(self):
```

### Comparing `witness-etl-0.0.5/witness/core/batch.py` & `witness-etl-0.0.6/witness/core/batch.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,21 +59,21 @@
         return message
 
     def fill(self, extractor):
         """
         Fills batch internal datastructures using
         the extractor passed in.
         """
-        if extractor.output is None:
-            extractor.extract()
 
-        if extractor.is_unified:
-            output = extractor.output
+        if extractor.output is not None:
+            if extractor.extraction_timestamp is None:
+                extractor.set_extraction_timestamp()
+            output = extractor.output if extractor.is_unified else extractor.unify().output
         else:
-            output = extractor.unify().output
+            output = extractor.extract().unify().output
         setattr(self, 'data', output['data'])
         setattr(self, 'meta', MetaData(**output['meta']))
         return self
 
     def push(self, loader, meta_elements: Optional[list[str]] = None):
         """
         Pushes data, with the appropriate meta attached,
```

### Comparing `witness-etl-0.0.5/witness/extractors/__init__.py` & `witness-etl-0.0.6/witness/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.5/witness/extractors/database.py` & `witness-etl-0.0.6/witness/extractors/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class DatabaseExtractor(AbstractExtractor):
 
     def __init__(self, uri):
         super().__init__(uri)
 
     def extract(self):
-        self._set_extraction_timestamp()
+        self.set_extraction_timestamp()
 
     def unify(self):
         raise NotImplementedError
 
 
 class ODBCExtractor(DatabaseExtractor):
```

### Comparing `witness-etl-0.0.5/witness/extractors/file.py` & `witness-etl-0.0.6/witness/extractors/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,12 +15,12 @@
 
 from witness.core.abstract import AbstractExtractor
 
 
 class FileExtractor(AbstractExtractor):
 
     def extract(self):
-        self._set_extraction_timestamp()
+        self.set_extraction_timestamp()
 
     def unify(self):
         raise NotImplementedError
```

### Comparing `witness-etl-0.0.5/witness/extractors/http.py` & `witness-etl-0.0.6/witness/extractors/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def extract(self):
 
         response = requests.get(url=self.uri, params=self.params, auth=self.auth)
         response.raise_for_status()
 
         setattr(self, 'output', response)
-        self._set_extraction_timestamp()
+        self.set_extraction_timestamp()
 
         return self
 
     def unify(self):
         meta = {'extraction_timestamp': self.extraction_timestamp,
                 'record_source': self.uri}
         data = self.serializer.to_batch(self.output)
```

### Comparing `witness-etl-0.0.5/witness/loaders/__init__.py` & `witness-etl-0.0.6/witness/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.5/witness/providers/pandas/__init__.py` & `witness-etl-0.0.6/witness/providers/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.5/witness/providers/pandas/core.py` & `witness-etl-0.0.6/witness/providers/pandas/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     def __init__(self, uri, serializer: Optional[AbstractSerializer] = PandasSerializer()):
         super().__init__(uri)
         self.serializer = PandasSerializer()
 
     output: pd.DataFrame
 
     def extract(self):
-        self._set_extraction_timestamp()
+        self.set_extraction_timestamp()
         return self
 
     def unify(self):
         data = self.serializer.to_batch(self.output)
         meta = {
             "extraction_timestamp": self.extraction_timestamp,
             "record_source": self.uri,
```

### Comparing `witness-etl-0.0.5/witness/providers/pandas/extractors.py` & `witness-etl-0.0.6/witness/providers/pandas/extractors.py`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.5/witness/providers/pandas/loaders.py` & `witness-etl-0.0.6/witness/providers/pandas/loaders.py`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.5/witness/version.py` & `witness-etl-0.0.6/witness/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,14 @@
 except ImportError:
     from importlib import metadata  # type: ignore[no-redef]
 
 try:
     version = metadata.version('witness-etl')
 except metadata.PackageNotFoundError:
     import logging
-    version = '0.0.5'
+    version = '0.0.6'
 
 
 del metadata
 
 if __name__ == '__main__':
     print(version)
```

### Comparing `witness-etl-0.0.5/witness_etl.egg-info/PKG-INFO` & `witness-etl-0.0.6/witness_etl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: witness-etl
-Version: 0.0.5
+Version: 0.0.6
 Summary: A minimal ETL library.
 Author: Eugene Popov
 Author-email: evgeniypalych@gmail.com
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/eppv/witness
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `witness-etl-0.0.5/witness_etl.egg-info/SOURCES.txt` & `witness-etl-0.0.6/witness_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

