# Comparing `tmp/simple-alto-parser-0.0.4.tar.gz` & `tmp/simple-alto-parser-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-alto-parser-0.0.4.tar", last modified: Wed May 17 09:09:16 2023, max compression
+gzip compressed data, was "simple-alto-parser-0.0.5.tar", last modified: Wed May 24 14:10:37 2023, max compression
```

## Comparing `simple-alto-parser-0.0.4.tar` & `simple-alto-parser-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:09:16.070344 simple-alto-parser-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 09:08:59.000000 simple-alto-parser-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 09:08:59.000000 simple-alto-parser-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-17 09:09:16.070344 simple-alto-parser-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-17 09:08:59.000000 simple-alto-parser-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-17 09:08:59.000000 simple-alto-parser-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-17 09:08:59.000000 simple-alto-parser-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-17 09:09:16.070344 simple-alto-parser-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-17 09:08:59.000000 simple-alto-parser-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:09:16.070344 simple-alto-parser-0.0.4/simple_alto_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 09:08:59.000000 simple-alto-parser-0.0.4/simple_alto_parser/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-17 09:08:59.000000 simple-alto-parser-0.0.4/simple_alto_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-05-17 09:08:59.000000 simple-alto-parser-0.0.4/simple_alto_parser/alto_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-17 09:08:59.000000 simple-alto-parser-0.0.4/simple_alto_parser/alto_file_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-05-17 09:08:59.000000 simple-alto-parser-0.0.4/simple_alto_parser/alto_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-17 09:08:59.000000 simple-alto-parser-0.0.4/simple_alto_parser/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-17 09:08:59.000000 simple-alto-parser-0.0.4/simple_alto_parser/dictionary_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-17 09:08:59.000000 simple-alto-parser-0.0.4/simple_alto_parser/dictionary_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-17 09:08:59.000000 simple-alto-parser-0.0.4/simple_alto_parser/nlp_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-17 09:08:59.000000 simple-alto-parser-0.0.4/simple_alto_parser/pattern_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:09:16.070344 simple-alto-parser-0.0.4/simple_alto_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-17 09:09:16.000000 simple-alto-parser-0.0.4/simple_alto_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-17 09:09:16.000000 simple-alto-parser-0.0.4/simple_alto_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:09:16.000000 simple-alto-parser-0.0.4/simple_alto_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-17 09:09:16.000000 simple-alto-parser-0.0.4/simple_alto_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 09:09:16.000000 simple-alto-parser-0.0.4/simple_alto_parser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:10:37.382781 simple-alto-parser-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-24 14:10:37.382781 simple-alto-parser-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-24 14:10:37.382781 simple-alto-parser-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:10:37.382781 simple-alto-parser-0.0.5/simple_alto_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/simple_alto_parser/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/simple_alto_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/simple_alto_parser/alto_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/simple_alto_parser/alto_file_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/simple_alto_parser/alto_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/simple_alto_parser/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/simple_alto_parser/dictionary_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/simple_alto_parser/dictionary_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/simple_alto_parser/nlp_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/simple_alto_parser/pattern_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:10:37.382781 simple-alto-parser-0.0.5/simple_alto_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-24 14:10:37.000000 simple-alto-parser-0.0.5/simple_alto_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-24 14:10:37.000000 simple-alto-parser-0.0.5/simple_alto_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:10:37.000000 simple-alto-parser-0.0.5/simple_alto_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-24 14:10:37.000000 simple-alto-parser-0.0.5/simple_alto_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-24 14:10:37.000000 simple-alto-parser-0.0.5/simple_alto_parser.egg-info/top_level.txt
```

### Comparing `simple-alto-parser-0.0.4/LICENSE` & `simple-alto-parser-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.4/PKG-INFO` & `simple-alto-parser-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-alto-parser
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python module to read and parse ALTO files
 Home-page: https://simple-alto-parser.readthedocs.io/en/latest/
 Author: Sorin Marti, Lea Kasper
 Author-email: sorin.marti@gmail.com, lea.kasper@unibas.ch
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
```

### Comparing `simple-alto-parser-0.0.4/README.md` & `simple-alto-parser-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.4/setup.cfg` & `simple-alto-parser-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.4/simple_alto_parser/alto_file.py` & `simple-alto-parser-0.0.5/simple_alto_parser/alto_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         return csv_title_line
 
     def get_csv_lines(self, add_header=True):
 
         header = self.get_csv_header()
         if add_header:
-            csv_lines = [header[0], ]
+            csv_lines = [header, ]
         else:
             csv_lines = []
 
         lines = self.get_text_lines()
 
         if len(lines) == 0:
             raise ValueError("No lines have been found in the file.")
@@ -100,15 +100,15 @@
                 csv_line.append(self.file_path)
 
             if print_attributes:
                 for key, value in line.element_data.items():
                     csv_line.append(value)
 
             if print_parser_results:
-                for parser_val in header[1]:
+                for parser_val in self.get_parser_result_keys():
                     csv_line.append(line.parser_data.get(parser_val, ''))
 
             if print_file_meta_data:
                 for key, value in self.file_meta_data.items():
                     csv_line.append(value)
             csv_lines.append(csv_line)
```

### Comparing `simple-alto-parser-0.0.4/simple_alto_parser/alto_file_exporter.py` & `simple-alto-parser-0.0.5/simple_alto_parser/alto_file_exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,17 @@
         self.file_parser = alto_file_parser
         self.files = alto_file_parser.get_alto_files()
 
     def get_combined_csv_header(self):
         total_header = []
         for file in self.files:
             f_header = file.get_csv_header()
-            for header in f_header[0]:
+            for header in f_header:
                 if header not in total_header:
                     total_header.append(header)
-            print(f_header[0][3+len(f_header[1]):])
         return total_header
 
     def save_csv(self, file_name, **kwargs):
         self.assure_is_file(file_name)
 
         file_idx = 0
         csv_lines = [self.get_combined_csv_header(), ]
```

### Comparing `simple-alto-parser-0.0.4/simple_alto_parser/alto_file_parser.py` & `simple-alto-parser-0.0.5/simple_alto_parser/alto_file_parser.py`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.4/simple_alto_parser/base_parser.py` & `simple-alto-parser-0.0.5/simple_alto_parser/base_parser.py`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.4/simple_alto_parser/dictionary_creator.py` & `simple-alto-parser-0.0.5/simple_alto_parser/dictionary_creator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import csv
+import json
+
 
 def from_geonames(csv_file_path):
     # Open Tsv
     with open(csv_file_path, encoding='utf-8') as f:
         csv_reader = csv.reader(f, delimiter='\t')
         row_id = 0
         for row in csv_reader:
@@ -31,8 +33,25 @@
 
 
             row_id += 1
             if row_id > 20:
                 break
 
 
-from_geonames('../assets/dicts/CH.tsv')
+#from_geonames('../assets/dicts/CH.tsv')
+
+def from_file(filename, type='undefined'):
+    with open(filename, encoding='utf-8') as f:
+        entries = []
+        for line in f:
+            entry = {
+                "label": line.strip(),
+                "variants": [line.strip()],
+                "type": type
+            }
+            entries.append(entry)
+
+    with open(filename + '.json', 'w', encoding='utf-8') as f:
+        f.write(json.dumps(entries, indent=4, sort_keys=True))
+
+from_file('../assets/dicts/titles.csv', type="title")
+
```

### Comparing `simple-alto-parser-0.0.4/simple_alto_parser/dictionary_parser.py` & `simple-alto-parser-0.0.5/simple_alto_parser/dictionary_parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,34 +11,55 @@
 
     def __init__(self, parser):
         """The constructor of the class. It initializes the list of files.
         The lines are a list of AltoXMLElement objects."""
         super().__init__(parser)
 
     def load(self, dictionary_file):
-        dictionary = json.load(open(dictionary_file))
+        dictionary = json.load(open(dictionary_file, encoding='utf-8'))
+        for entry in dictionary:
+            if 'label' in entry:
+                if 'variants' not in entry:
+                    entry['variants'] = [entry['label']]
+                if 'type' not in entry:
+                    entry['type'] = 'undefined'
+
+                entry['variants'] = [v.strip() for v in entry['variants']]
+                entry['variants'] = sorted(entry['variants'], key=len, reverse=True)
+                print(entry['variants'])
+            else:
+                raise Exception('The dictionary entry does not contain a label.')
+
         self.dictionaries.append(dictionary)
 
-    def find(self, strict=True):
+    def find(self, strict=True, restrict_to=None):
         """Find a pattern in the text lines."""
         self.clear()
         file_id = 0
         for file in self.parser.get_alto_files():
             line_id = 0
             for line in file.get_text_lines():
                 for dictionary in self.dictionaries:
                     for entry in dictionary:
-                        if strict:
-                            match = entry['entry'].strip('.').lower() == line.get_text().strip().strip('.').lower()
+                        if restrict_to is not None and entry['type'] == restrict_to:
+                            match = None
+                            if strict:
+                                for v in entry['variants']:
+                                    match = v.strip('.').lower() == line.get_text().strip().strip('.').lower()
+                                    if match:
+                                        match = v
+                                        break
+                            else:
+                                for v in entry['variants']:
+                                    match = re.search(re.escape(v), line.get_text().strip())
+                                    if match:
+                                        break
+
                             if match:
-                                match = entry['entry']
-                        else:
-                            match = re.search(entry['entry'], line.get_text().strip())
-                        if match:
-                            self.matches.append(DictionaryMatch(file_id, line_id, match, entry))
+                                self.matches.append(DictionaryMatch(file_id, line_id, match, entry))
                 line_id += 1
             file_id += 1
         return self
 
     def categorize(self):
         """Add the given category to all matches."""
         for match in self.matches:
@@ -52,17 +73,15 @@
 
     def remove(self, replacement=''):
         """Remove all matched patterns from matching lines."""
         for match in self.matches:
             if type(match.match) == str:
                 new_text = self.parser.get_alto_files()[match.file_id].get_text_lines()[match.line_id].get_text().replace(match.match, replacement)
             else:
-                new_text = re.sub(match.match,
-                                  replacement,
-                                  self.parser.get_alto_files()[match.fidx].get_text_lines()[match.lidx].get_text())
+                new_text = self.parser.get_alto_files()[match.file_id].get_text_lines()[match.line_id].get_text().replace(match.match.group(0), replacement)
 
             self.parser.get_alto_files()[match.file_id].get_text_lines()[match.line_id].set_text(new_text)
         return self
 
     def replace(self, replacement):
         self.remove(replacement)
         return self
```

### Comparing `simple-alto-parser-0.0.4/simple_alto_parser/nlp_parser.py` & `simple-alto-parser-0.0.5/simple_alto_parser/nlp_parser.py`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.4/simple_alto_parser/pattern_parser.py` & `simple-alto-parser-0.0.5/simple_alto_parser/pattern_parser.py`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.4/simple_alto_parser.egg-info/PKG-INFO` & `simple-alto-parser-0.0.5/simple_alto_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-alto-parser
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python module to read and parse ALTO files
 Home-page: https://simple-alto-parser.readthedocs.io/en/latest/
 Author: Sorin Marti, Lea Kasper
 Author-email: sorin.marti@gmail.com, lea.kasper@unibas.ch
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
```

### Comparing `simple-alto-parser-0.0.4/simple_alto_parser.egg-info/SOURCES.txt` & `simple-alto-parser-0.0.5/simple_alto_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

