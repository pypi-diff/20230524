# Comparing `tmp/csv-embeddings-creator-1.0.5.tar.gz` & `tmp/csv-embeddings-creator-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv-embeddings-creator-1.0.5.tar", last modified: Sun May 21 18:52:52 2023, max compression
+gzip compressed data, was "csv-embeddings-creator-1.0.6.tar", last modified: Wed May 24 06:48:07 2023, max compression
```

## Comparing `csv-embeddings-creator-1.0.5.tar` & `csv-embeddings-creator-1.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 18:52:52.322108 csv-embeddings-creator-1.0.5/
--rw-r--r--   0 chiubowen   (501) staff       (20)     3136 2023-05-21 18:52:52.321991 csv-embeddings-creator-1.0.5/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     2956 2023-05-21 18:52:52.000000 csv-embeddings-creator-1.0.5/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 18:52:52.321823 csv-embeddings-creator-1.0.5/csv_embeddings_creator.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     3136 2023-05-21 18:52:52.000000 csv-embeddings-creator-1.0.5/csv_embeddings_creator.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      322 2023-05-21 18:52:52.000000 csv-embeddings-creator-1.0.5/csv_embeddings_creator.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-21 18:52:52.000000 csv-embeddings-creator-1.0.5/csv_embeddings_creator.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       72 2023-05-21 18:52:52.000000 csv-embeddings-creator-1.0.5/csv_embeddings_creator.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       37 2023-05-21 18:52:52.000000 csv-embeddings-creator-1.0.5/csv_embeddings_creator.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       23 2023-05-21 18:52:52.000000 csv-embeddings-creator-1.0.5/csv_embeddings_creator.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     3074 2023-05-21 18:52:52.000000 csv-embeddings-creator-1.0.5/csv_embeddings_creator.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-21 18:52:52.322143 csv-embeddings-creator-1.0.5/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      552 2023-05-21 18:52:52.000000 csv-embeddings-creator-1.0.5/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-24 06:48:07.161478 csv-embeddings-creator-1.0.6/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3136 2023-05-24 06:48:07.161357 csv-embeddings-creator-1.0.6/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2956 2023-05-24 06:48:07.000000 csv-embeddings-creator-1.0.6/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-24 06:48:07.161180 csv-embeddings-creator-1.0.6/csv_embeddings_creator.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3136 2023-05-24 06:48:07.000000 csv-embeddings-creator-1.0.6/csv_embeddings_creator.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      322 2023-05-24 06:48:07.000000 csv-embeddings-creator-1.0.6/csv_embeddings_creator.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-24 06:48:07.000000 csv-embeddings-creator-1.0.6/csv_embeddings_creator.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       72 2023-05-24 06:48:07.000000 csv-embeddings-creator-1.0.6/csv_embeddings_creator.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       37 2023-05-24 06:48:07.000000 csv-embeddings-creator-1.0.6/csv_embeddings_creator.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       23 2023-05-24 06:48:07.000000 csv-embeddings-creator-1.0.6/csv_embeddings_creator.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     3058 2023-05-24 06:48:07.000000 csv-embeddings-creator-1.0.6/csv_embeddings_creator.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-24 06:48:07.161518 csv-embeddings-creator-1.0.6/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      552 2023-05-24 06:48:07.000000 csv-embeddings-creator-1.0.6/setup.py
```

### Comparing `csv-embeddings-creator-1.0.5/PKG-INFO` & `csv-embeddings-creator-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv-embeddings-creator
-Version: 1.0.5
+Version: 1.0.6
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # csv_embeddings_creator v1.0.4 by Bowen Chiu
```

### Comparing `csv-embeddings-creator-1.0.5/README.md` & `csv-embeddings-creator-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `csv-embeddings-creator-1.0.5/csv_embeddings_creator.egg-info/PKG-INFO` & `csv-embeddings-creator-1.0.6/csv_embeddings_creator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv-embeddings-creator
-Version: 1.0.5
+Version: 1.0.6
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # csv_embeddings_creator v1.0.4 by Bowen Chiu
```

### Comparing `csv-embeddings-creator-1.0.5/csv_embeddings_creator.py` & `csv-embeddings-creator-1.0.6/csv_embeddings_creator.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 
     csv_files = glob.glob(os.path.join(input_folder, '**/*.csv'), recursive=True)
     embedding_files = glob.glob(os.path.join(output_embeddings_folder, '**/*.pt'), recursive=True)
 
     # 跳過已經做完的
     dic_doc_id = {}
     for path in embedding_files:
-        doc_id = re.findall('doc-id_(.*?)_spreadsheet', path)[0]
+        doc_id = re.findall('doc-id_(.*?)_sha', path)[0]
         dic_doc_id[doc_id] = True
 
     i = 0
     for csv_file in csv_files:
-        doc_id = re.findall('doc-id_(.*?)_spreadsheet', csv_file)[0]
+        doc_id = re.findall('doc-id_(.*?)_sha', csv_file)[0]
         if doc_id in dic_doc_id:
             continue
 
         file_base_name = os.path.splitext(os.path.basename(csv_file))[0]
         existing_txt_files = glob.glob(os.path.join(output_txt_folder, f"{file_base_name}_*.txt"))
 
         if not force and existing_txt_files:
```

### Comparing `csv-embeddings-creator-1.0.5/setup.py` & `csv-embeddings-creator-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="csv-embeddings-creator",
-    version="1.0.5",
+    version="1.0.6",
     packages=find_packages(),
     py_modules=['csv_embeddings_creator'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'csv_embeddings_creator = csv_embeddings_creator:main',
         ],
```

