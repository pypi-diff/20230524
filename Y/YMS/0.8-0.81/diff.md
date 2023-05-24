# Comparing `tmp/YMS-0.8.tar.gz` & `tmp/YMS-0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YMS-0.8.tar", last modified: Mon May 22 15:53:18 2023, max compression
+gzip compressed data, was "YMS-0.81.tar", last modified: Wed May 24 13:44:45 2023, max compression
```

## Comparing `YMS-0.8.tar` & `YMS-0.81.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-22 15:53:18.795513 YMS-0.8/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      155 2023-05-22 15:53:18.795513 YMS-0.8/PKG-INFO
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     2003 2023-04-02 09:28:26.000000 YMS-0.8/README.md
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-22 15:53:18.795513 YMS-0.8/YMS.egg-info/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      155 2023-05-22 15:53:18.000000 YMS-0.8/YMS.egg-info/PKG-INFO
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      317 2023-05-22 15:53:18.000000 YMS-0.8/YMS.egg-info/SOURCES.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        1 2023-05-22 15:53:18.000000 YMS-0.8/YMS.egg-info/dependency_links.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       37 2023-05-22 15:53:18.000000 YMS-0.8/YMS.egg-info/entry_points.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       15 2023-05-22 15:53:18.000000 YMS-0.8/YMS.egg-info/requires.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        6 2023-05-22 15:53:18.000000 YMS-0.8/YMS.egg-info/top_level.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       38 2023-05-22 15:53:18.795513 YMS-0.8/setup.cfg
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      475 2023-05-22 15:53:02.000000 YMS-0.8/setup.py
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-22 15:53:18.795513 YMS-0.8/yamas/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1942 2023-05-09 16:55:03.000000 YMS-0.8/yamas/__init__.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       30 2023-03-26 09:25:23.000000 YMS-0.8/yamas/config.json
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)    11618 2023-05-22 15:52:53.000000 YMS-0.8/yamas/create_visualization.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1015 2023-05-09 16:55:03.000000 YMS-0.8/yamas/dataset_downloading.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9100 2023-04-02 11:41:02.000000 YMS-0.8/yamas/export_data.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1183 2023-03-09 09:50:30.000000 YMS-0.8/yamas/utilities.py
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-24 13:44:45.864295 YMS-0.81/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-24 13:44:45.864295 YMS-0.81/PKG-INFO
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     2003 2023-04-02 09:28:26.000000 YMS-0.81/README.md
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-24 13:44:45.864295 YMS-0.81/YMS.egg-info/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-24 13:44:45.000000 YMS-0.81/YMS.egg-info/PKG-INFO
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      317 2023-05-24 13:44:45.000000 YMS-0.81/YMS.egg-info/SOURCES.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        1 2023-05-24 13:44:45.000000 YMS-0.81/YMS.egg-info/dependency_links.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       37 2023-05-24 13:44:45.000000 YMS-0.81/YMS.egg-info/entry_points.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       15 2023-05-24 13:44:45.000000 YMS-0.81/YMS.egg-info/requires.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        6 2023-05-24 13:44:45.000000 YMS-0.81/YMS.egg-info/top_level.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       38 2023-05-24 13:44:45.864295 YMS-0.81/setup.cfg
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      476 2023-05-24 13:42:14.000000 YMS-0.81/setup.py
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-24 13:44:45.864295 YMS-0.81/yamas/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1942 2023-05-09 16:55:03.000000 YMS-0.81/yamas/__init__.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       30 2023-03-26 09:25:23.000000 YMS-0.81/yamas/config.json
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)    11412 2023-05-24 13:41:48.000000 YMS-0.81/yamas/create_visualization.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1015 2023-05-09 16:55:03.000000 YMS-0.81/yamas/dataset_downloading.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9100 2023-04-02 11:41:02.000000 YMS-0.81/yamas/export_data.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1183 2023-03-09 09:50:30.000000 YMS-0.81/yamas/utilities.py
```

### Comparing `YMS-0.8/README.md` & `YMS-0.81/README.md`

 * *Files identical despite different names*

### Comparing `YMS-0.8/yamas/__init__.py` & `YMS-0.81/yamas/__init__.py`

 * *Files identical despite different names*

### Comparing `YMS-0.8/yamas/create_visualization.py` & `YMS-0.81/yamas/create_visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,35 +128,34 @@
     run_cmd(command)
     return vis_file_path
 
 def metaphlan_extraction(reads_data, dataset_id):
     paired = reads_data.rev and reads_data.fwd
     fastq_path = os.path.join(reads_data.dir_path, "fastq")
     export_path = os.path.join(reads_data.dir_path, "export")
-    qza_path = os.path.join(reads_data.dir_path, "qza")
     run_cmd([f"mkdir {export_path}"])
     final_output_path = os.path.join(export_path, f'{dataset_id}_final.txt')
     run_cmd([f"touch {final_output_path}"])
     fastq_files = [a for a in os.listdir(fastq_path) if a.split(".")[-1] == "fastq"]
     args = []
     if paired:
         print("paired")
-        for i, j in tqdm(zip(fastq_files[::2], fastq_files[1::2])):
+        for i in tqdm(0, range(len(fastq_files),2)):
             fastq_1 = os.path.join(fastq_path, fastq_files[i])
-            fastq_2 = os.path.join(fastq_path, fastq_files[j])
-            output = os.path.join(qza_path, "{fastq_1.split('_')[0]}.bowtie2.bz2")
+            fastq_2 = os.path.join(fastq_path, fastq_files[i+1])
+            output = f"{fastq_files[i].split('_')[0]}.bowtie2.bz2"
             command = [f"metaphlan {fastq_1},{fastq_2} --input_type fastq --bowtie2out {output} --nproc 24"]
             run_cmd(command)
             args.append(os.path.join(fastq_path, output))
     else:
         print("not paired")
         for fastq in tqdm(fastq_files):
             output = os.path.join(os.path.join(reads_data.dir_path, 'qza'), f'{fastq}_profile.txt')
             fastq = os.path.join(fastq_path,fastq)
-            command = [f"metaphlan {fastq} --input_type fastq --nproc 16 > {output}"]
+            command = [f"metaphlan {fastq} --input_type fastq --nproc 24 > {output}"]
             run_cmd(command)
             args.append(output)
     merge(args, open(final_output_path, 'w'), gtdb=False)
 
 def metaphlan_txt_csv(reads_data, dataset_id):
     export_path = os.path.join(reads_data.dir_path, "export")
     input_file = os.path.join(export_path,f"{dataset_id}_final.txt")
@@ -196,31 +195,31 @@
     verbose_print("Checking inputs:")
     check_input(acc_list)
 
     verbose_print("\n")
     verbose_print("Creating a new directory for this dataset import:'", dir_name, "'")
     dir_path = create_dir(dir_name,specific_location)
     verbose_print("Find ALL NEW data in:", dir_path)
-    stages_length = 5 if data_type=='16S' else 3
 
     verbose_print("\n")
-    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start prefetch (1/{stages_length})")
+    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start prefetch (1/5)")
     download_data_from_sra(dir_path, acc_list)
-    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish prefetch (1/{stages_length})")
+    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish prefetch (1/5)")
 
     verbose_print("\n")
-    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start conversion (2/{stages_length})")
+    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start conversion (2/5)")
     reads_data = sra_to_fastq(dir_path)
-    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish conversion (2/{stages_length})")
+    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish conversion (2/5)")
+
+    verbose_print("\n")
+    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start creating manifest (3/5)")
+    create_manifest(reads_data)
+    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish creating manifest (3/5)")
 
     if data_type == '16S':
-        verbose_print("\n")
-        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start creating manifest (3/5)")
-        create_manifest(reads_data)
-        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish creating manifest (3/5)")
 
         verbose_print("\n")
         verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start 'qiime import' (4/5)")
         qza_file_path = qiime_import(reads_data)
         verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish 'qiime import' (4/5)")
 
         verbose_print("\n")
@@ -242,17 +241,17 @@
             print(f"Note: The data has only a forward read.\n"
                   f"Therefore, you must give the parameters 'trim' and 'trunc' of export() "
                   f"exactly one integers value which is related to the forward read.")
 
         return reads_data.dir_path
     else:
         verbose_print("\n")
-        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start metaphlan extraction (3/4)")
+        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start metaphlan extraction (4/5)")
         metaphlan_extraction(reads_data, dataset_id)
-        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish metaphlan extraction (3/4)")
+        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish metaphlan extraction (4/5)")
         verbose_print("\n")
-        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start metaphlan extraction (4/4)")
+        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start metaphlan extraction (5/5)")
         metaphlan_txt_csv(reads_data, dataset_id)
-        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish metaphlan extraction (4/4)")
+        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish metaphlan extraction (5/5)")
         verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finished downloading.\n")
```

### Comparing `YMS-0.8/yamas/dataset_downloading.py` & `YMS-0.81/yamas/dataset_downloading.py`

 * *Files identical despite different names*

### Comparing `YMS-0.8/yamas/export_data.py` & `YMS-0.81/yamas/export_data.py`

 * *Files identical despite different names*

### Comparing `YMS-0.8/yamas/utilities.py` & `YMS-0.81/yamas/utilities.py`

 * *Files identical despite different names*

