# Comparing `tmp/YMS-0.82.tar.gz` & `tmp/YMS-0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YMS-0.82.tar", last modified: Wed May 24 14:16:45 2023, max compression
+gzip compressed data, was "YMS-0.83.tar", last modified: Wed May 24 14:31:09 2023, max compression
```

## Comparing `YMS-0.82.tar` & `YMS-0.83.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-24 14:16:45.688357 YMS-0.82/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-24 14:16:45.688357 YMS-0.82/PKG-INFO
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     2003 2023-04-02 09:28:26.000000 YMS-0.82/README.md
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-24 14:16:45.688357 YMS-0.82/YMS.egg-info/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-24 14:16:45.000000 YMS-0.82/YMS.egg-info/PKG-INFO
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      317 2023-05-24 14:16:45.000000 YMS-0.82/YMS.egg-info/SOURCES.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        1 2023-05-24 14:16:45.000000 YMS-0.82/YMS.egg-info/dependency_links.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       37 2023-05-24 14:16:45.000000 YMS-0.82/YMS.egg-info/entry_points.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       15 2023-05-24 14:16:45.000000 YMS-0.82/YMS.egg-info/requires.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        6 2023-05-24 14:16:45.000000 YMS-0.82/YMS.egg-info/top_level.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       38 2023-05-24 14:16:45.688357 YMS-0.82/setup.cfg
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      476 2023-05-24 14:15:17.000000 YMS-0.82/setup.py
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-24 14:16:45.688357 YMS-0.82/yamas/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1942 2023-05-09 16:55:03.000000 YMS-0.82/yamas/__init__.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       30 2023-03-26 09:25:23.000000 YMS-0.82/yamas/config.json
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)    11410 2023-05-24 14:15:17.000000 YMS-0.82/yamas/create_visualization.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1015 2023-05-09 16:55:03.000000 YMS-0.82/yamas/dataset_downloading.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9100 2023-04-02 11:41:02.000000 YMS-0.82/yamas/export_data.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1183 2023-03-09 09:50:30.000000 YMS-0.82/yamas/utilities.py
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-24 14:31:09.120385 YMS-0.83/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-24 14:31:09.120385 YMS-0.83/PKG-INFO
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     2003 2023-04-02 09:28:26.000000 YMS-0.83/README.md
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-24 14:31:09.120385 YMS-0.83/YMS.egg-info/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-24 14:31:09.000000 YMS-0.83/YMS.egg-info/PKG-INFO
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      317 2023-05-24 14:31:09.000000 YMS-0.83/YMS.egg-info/SOURCES.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        1 2023-05-24 14:31:09.000000 YMS-0.83/YMS.egg-info/dependency_links.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       37 2023-05-24 14:31:09.000000 YMS-0.83/YMS.egg-info/entry_points.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       15 2023-05-24 14:31:09.000000 YMS-0.83/YMS.egg-info/requires.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        6 2023-05-24 14:31:09.000000 YMS-0.83/YMS.egg-info/top_level.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       38 2023-05-24 14:31:09.120385 YMS-0.83/setup.cfg
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      476 2023-05-24 14:30:53.000000 YMS-0.83/setup.py
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-24 14:31:09.120385 YMS-0.83/yamas/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1942 2023-05-09 16:55:03.000000 YMS-0.83/yamas/__init__.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       30 2023-03-26 09:25:23.000000 YMS-0.83/yamas/config.json
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)    11409 2023-05-24 14:30:45.000000 YMS-0.83/yamas/create_visualization.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1015 2023-05-09 16:55:03.000000 YMS-0.83/yamas/dataset_downloading.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9100 2023-04-02 11:41:02.000000 YMS-0.83/yamas/export_data.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1183 2023-03-09 09:50:30.000000 YMS-0.83/yamas/utilities.py
```

### Comparing `YMS-0.82/README.md` & `YMS-0.83/README.md`

 * *Files identical despite different names*

### Comparing `YMS-0.82/yamas/__init__.py` & `YMS-0.83/yamas/__init__.py`

 * *Files identical despite different names*

### Comparing `YMS-0.82/yamas/create_visualization.py` & `YMS-0.83/yamas/create_visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     run_cmd([f"mkdir {export_path}"])
     final_output_path = os.path.join(export_path, f'{dataset_id}_final.txt')
     run_cmd([f"touch {final_output_path}"])
     fastq_files = [a for a in os.listdir(fastq_path) if a.split(".")[-1] == "fastq"]
     args = []
     if paired:
         print("paired")
-        for i in tqdm(0, range(len(fastq_files),2)):
+        for i in tqdm(range(0,len(fastq_files),2)):
             fastq_1 = os.path.join(fastq_path, fastq_files[i])
             fastq_2 = os.path.join(fastq_path, fastq_files[i+1])
             output = f"{fastq_files[i].split('_')[0]}.bowtie2.bz2"
             command = [f"metaphlan {fastq_1},{fastq_2} --input_type fastq --bowtie2out {output} --nproc 24"]
             run_cmd(command)
             args.append(os.path.join(fastq_path, output))
     else:
```

### Comparing `YMS-0.82/yamas/dataset_downloading.py` & `YMS-0.83/yamas/dataset_downloading.py`

 * *Files identical despite different names*

### Comparing `YMS-0.82/yamas/export_data.py` & `YMS-0.83/yamas/export_data.py`

 * *Files identical despite different names*

### Comparing `YMS-0.82/yamas/utilities.py` & `YMS-0.83/yamas/utilities.py`

 * *Files identical despite different names*

