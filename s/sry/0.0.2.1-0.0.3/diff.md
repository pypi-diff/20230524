# Comparing `tmp/sry-0.0.2.1-py3-none-any.whl.zip` & `tmp/sry-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1848 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     2359 b- defN 23-May-07 11:18 sry.py
--rw-rw-rw-  2.0 fat       74 b- defN 23-May-08 08:40 sry-0.0.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-08 08:40 sry-0.0.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-May-08 08:40 sry-0.0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      350 b- defN 23-May-08 08:40 sry-0.0.2.1.dist-info/RECORD
-5 files, 2876 bytes uncompressed, 1194 bytes compressed:  58.5%
+Zip file size: 2057 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     2998 b- defN 23-May-08 09:42 sry.py
+-rw-rw-rw-  2.0 fat       72 b- defN 23-May-08 09:43 sry-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-08 09:43 sry-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 23-May-08 09:43 sry-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      342 b- defN 23-May-08 09:43 sry-0.0.3.dist-info/RECORD
+5 files, 3505 bytes uncompressed, 1419 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: sry.py
 Comment: 
 
-Filename: sry-0.0.2.1.dist-info/METADATA
+Filename: sry-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: sry-0.0.2.1.dist-info/WHEEL
+Filename: sry-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: sry-0.0.2.1.dist-info/top_level.txt
+Filename: sry-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: sry-0.0.2.1.dist-info/RECORD
+Filename: sry-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sry.py

```diff
@@ -1,10 +1,11 @@
 import os
 import requests
 from tqdm import tqdm
+import datetime
 
 
 class File:
 	class Size:
 		def find_file_size(self, path="C:\\", max_or_min="max"):
 			size_path, size_list = self.__get_all_size(path)
 			if max_or_min == "max":
@@ -21,15 +22,15 @@
 				for file_name in files:
 					size_path.append([os.path.getsize(os.path.join(path, file_name)), os.path.join(path, file_name)])
 				for dir in file_dir:
 					size_path.append([os.path.getsize(os.path.join(path, dir)), os.path.join(path, dir)])
 			size_list = []
 			for i in range(len(size_path)):
 				size_list.append(size_path[i][0])
-			return size_path, size_list
+			return [size_path, size_list]
 
 		def __size_small(self, fsize, size_path, size_list):
 			if fsize < 1024:
 				return [str(round(fsize, 2)) + 'B', size_path[size_list.index(max(size_list))][1]]
 			else:
 				KBX = fsize / 1024
 				if KBX < 1024:
@@ -47,14 +48,30 @@
 
 		def all_file_size(self, path="C:\\"):
 			size_path, size_list = self.__get_all_size(path)
 			for i in range(len(size_path)):
 				size_path[i][0] = str(self.__size_small(int(size_path[i][0]), size_path, size_list)[0])
 			return size_path
 
+	def big_and_not_be_used(self,path="C:\\"):
+		size_path = self.__get_all_size(path)[0]
+		path_list = [i[1] for i in size_path]
+		filelist = []
+		path_with_time = []
+		for i in range(0, len(path_list)):
+			filelist.append(path_list[i])
+
+		for i in range(0, len(filelist)):
+			a_path = path_list[i]
+			timestamp = os.path.getmtime(a_path)
+			date = datetime.datetime.fromtimestamp(timestamp)
+			path_with_time.append(["\\".join([item for item in filelist[i].split("\\") if not item in path.split("\\")]), date.strftime('%Y-%m-%d %H:%M:%S')])
+		return path_with_time
+
+
 class Download:
 	def Download_with_progress_bar(self,url,fname):
 		resp = requests.get(url, stream=True)
 		total = int(resp.headers.get('content-length', 0))
 		with open(fname, 'wb') as file, tqdm(
 				desc=fname,
 				total=total,
@@ -65,8 +82,9 @@
 			for data in resp.iter_content(chunk_size=1024):
 				size = file.write(data)
 				bar.update(size)
 
 
 file = File
 size = file.Size()
-download = Download()
+download = Download()
+size.big_and_not_be_used("C:\\Users\\sunhui\\Desktop")
```

