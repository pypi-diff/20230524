# Comparing `tmp/srrcomp-0.1.1.tar.gz` & `tmp/srrcomp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srrcomp-0.1.1.tar", last modified: Mon Dec 26 14:12:10 2022, max compression
+gzip compressed data, was "srrcomp-0.1.2.tar", last modified: Wed May 24 07:56:00 2023, max compression
```

## Comparing `srrcomp-0.1.1.tar` & `srrcomp-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 14:12:10.070901 srrcomp-0.1.1/
--rw-rw-r--   0 root         (0) root         (0)     1749 2022-12-26 14:10:57.000000 srrcomp-0.1.1/LICENSE.txt
--rw-rw-r--   0 root         (0) root         (0)      490 2022-12-26 14:10:57.000000 srrcomp-0.1.1/NOTICE.txt
--rw-r--r--   0 root         (0) root         (0)     3798 2022-12-26 14:12:10.070901 srrcomp-0.1.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3386 2022-12-26 14:10:57.000000 srrcomp-0.1.1/README.md
--rw-rw-r--   0 root         (0) root         (0)      125 2022-12-26 14:10:57.000000 srrcomp-0.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-26 14:12:10.070901 srrcomp-0.1.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1605 2022-12-26 14:10:57.000000 srrcomp-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 14:12:10.066901 srrcomp-0.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 14:12:10.066901 srrcomp-0.1.1/src/srrcomp/
--rw-rw-r--   0 root         (0) root         (0)       96 2022-12-26 14:10:57.000000 srrcomp-0.1.1/src/srrcomp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 14:12:10.066901 srrcomp-0.1.1/src/srrcomp/eden_utils/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 14:12:10.070901 srrcomp-0.1.1/src/srrcomp/eden_utils/csrc/
--rw-rw-r--   0 root         (0) root         (0)     9053 2022-12-26 14:10:57.000000 srrcomp-0.1.1/src/srrcomp/eden_utils/csrc/cuda_hadamard.cu
--rw-rw-r--   0 root         (0) root         (0)      273 2022-12-26 14:10:57.000000 srrcomp-0.1.1/src/srrcomp/eden_utils/csrc/cuda_hadamard.h
--rw-rw-r--   0 root         (0) root         (0)     3229 2022-12-26 14:10:57.000000 srrcomp-0.1.1/src/srrcomp/eden_utils/csrc/cuda_packing.cu
--rw-rw-r--   0 root         (0) root         (0)      323 2022-12-26 14:10:57.000000 srrcomp-0.1.1/src/srrcomp/eden_utils/csrc/cuda_packing.h
--rw-rw-r--   0 root         (0) root         (0)      752 2022-12-26 14:10:57.000000 srrcomp-0.1.1/src/srrcomp/eden_utils/csrc/defs.h
--rw-rw-r--   0 root         (0) root         (0)     2929 2022-12-26 14:10:57.000000 srrcomp-0.1.1/src/srrcomp/eden_utils/eden_utils.cpp
--rw-rw-r--   0 root         (0) root         (0)    19638 2022-12-26 14:10:57.000000 srrcomp-0.1.1/src/srrcomp/srrcomp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 14:12:10.066901 srrcomp-0.1.1/src/srrcomp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3798 2022-12-26 14:12:10.000000 srrcomp-0.1.1/src/srrcomp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      526 2022-12-26 14:12:10.000000 srrcomp-0.1.1/src/srrcomp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-26 14:12:10.000000 srrcomp-0.1.1/src/srrcomp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-12-26 14:12:10.000000 srrcomp-0.1.1/src/srrcomp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-12-26 14:12:10.000000 srrcomp-0.1.1/src/srrcomp.egg-info/top_level.txt
+drwxrwxr-x   0 ybi       (1001) ybi       (1001)        0 2023-05-24 07:56:00.057044 srrcomp-0.1.2/
+-rw-rw-r--   0 ybi       (1001) ybi       (1001)     1749 2023-05-24 07:49:40.000000 srrcomp-0.1.2/LICENSE.txt
+-rw-rw-r--   0 ybi       (1001) ybi       (1001)      490 2023-05-24 07:49:40.000000 srrcomp-0.1.2/NOTICE.txt
+-rw-rw-r--   0 ybi       (1001) ybi       (1001)     3799 2023-05-24 07:56:00.057044 srrcomp-0.1.2/PKG-INFO
+-rw-rw-r--   0 ybi       (1001) ybi       (1001)     3387 2023-05-24 07:49:40.000000 srrcomp-0.1.2/README.md
+-rw-rw-r--   0 ybi       (1001) ybi       (1001)      125 2023-05-24 07:49:40.000000 srrcomp-0.1.2/pyproject.toml
+-rw-rw-r--   0 ybi       (1001) ybi       (1001)       38 2023-05-24 07:56:00.057044 srrcomp-0.1.2/setup.cfg
+-rw-rw-r--   0 ybi       (1001) ybi       (1001)     1605 2023-05-24 07:49:40.000000 srrcomp-0.1.2/setup.py
+drwxrwxr-x   0 ybi       (1001) ybi       (1001)        0 2023-05-24 07:56:00.053044 srrcomp-0.1.2/src/
+drwxrwxr-x   0 ybi       (1001) ybi       (1001)        0 2023-05-24 07:56:00.057044 srrcomp-0.1.2/src/srrcomp/
+-rw-rw-r--   0 ybi       (1001) ybi       (1001)       96 2023-05-24 07:49:40.000000 srrcomp-0.1.2/src/srrcomp/__init__.py
+drwxrwxr-x   0 ybi       (1001) ybi       (1001)        0 2023-05-24 07:56:00.057044 srrcomp-0.1.2/src/srrcomp/eden_utils/
+drwxrwxr-x   0 ybi       (1001) ybi       (1001)        0 2023-05-24 07:56:00.057044 srrcomp-0.1.2/src/srrcomp/eden_utils/csrc/
+-rw-rw-r--   0 ybi       (1001) ybi       (1001)     9297 2023-05-24 07:49:40.000000 srrcomp-0.1.2/src/srrcomp/eden_utils/csrc/cuda_hadamard.cu
+-rw-rw-r--   0 ybi       (1001) ybi       (1001)      273 2023-05-24 07:49:40.000000 srrcomp-0.1.2/src/srrcomp/eden_utils/csrc/cuda_hadamard.h
+-rw-rw-r--   0 ybi       (1001) ybi       (1001)     3229 2023-05-24 07:49:40.000000 srrcomp-0.1.2/src/srrcomp/eden_utils/csrc/cuda_packing.cu
+-rw-rw-r--   0 ybi       (1001) ybi       (1001)      323 2023-05-24 07:49:40.000000 srrcomp-0.1.2/src/srrcomp/eden_utils/csrc/cuda_packing.h
+-rw-rw-r--   0 ybi       (1001) ybi       (1001)      752 2023-05-24 07:49:40.000000 srrcomp-0.1.2/src/srrcomp/eden_utils/csrc/defs.h
+-rw-rw-r--   0 ybi       (1001) ybi       (1001)     2929 2023-05-24 07:49:40.000000 srrcomp-0.1.2/src/srrcomp/eden_utils/eden_utils.cpp
+-rw-rw-r--   0 ybi       (1001) ybi       (1001)    19638 2023-05-24 07:49:40.000000 srrcomp-0.1.2/src/srrcomp/srrcomp.py
+drwxrwxr-x   0 ybi       (1001) ybi       (1001)        0 2023-05-24 07:56:00.057044 srrcomp-0.1.2/src/srrcomp.egg-info/
+-rw-rw-r--   0 ybi       (1001) ybi       (1001)     3799 2023-05-24 07:56:00.000000 srrcomp-0.1.2/src/srrcomp.egg-info/PKG-INFO
+-rw-rw-r--   0 ybi       (1001) ybi       (1001)      526 2023-05-24 07:56:00.000000 srrcomp-0.1.2/src/srrcomp.egg-info/SOURCES.txt
+-rw-rw-r--   0 ybi       (1001) ybi       (1001)        1 2023-05-24 07:56:00.000000 srrcomp-0.1.2/src/srrcomp.egg-info/dependency_links.txt
+-rw-rw-r--   0 ybi       (1001) ybi       (1001)       12 2023-05-24 07:56:00.000000 srrcomp-0.1.2/src/srrcomp.egg-info/requires.txt
+-rw-rw-r--   0 ybi       (1001) ybi       (1001)       19 2023-05-24 07:56:00.000000 srrcomp-0.1.2/src/srrcomp.egg-info/top_level.txt
```

### Comparing `srrcomp-0.1.1/LICENSE.txt` & `srrcomp-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srrcomp-0.1.1/PKG-INFO` & `srrcomp-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srrcomp
-Version: 0.1.1
+Version: 0.1.2
 Summary: Structured random rotation (srr) based compression tools
 Home-page: https://github.com/shayvar/structured-random-rotation-based-compression
 Author: Shay Vargaftik and Yaniv Ben-Itzhak
 Author-email: shayv@vmware.com, ybenitzhak@vmware.com
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -59,15 +59,15 @@
 
 Windows: `$ pip install srrcomp --extra-index-url https://download.pytorch.org/whl/ --no-cache`
 
 If the message *"Faster CUDA implementation for Hadamard and bit packing is not available. Using torch implementation instead."* appears when importing srrcomp on a GPU machine, try installing `srrcomp` from source.
 
 ### Install from source
 
-For Windows and Ubuntu versions earlier than 22.04, dowload source from [the official repository](https://github.com/shayvar/structured-random-rotation-based-compression) and run `$ python setup.py install`
+For Windows and Ubuntu versions earlier than 22.04, download source from [the official repository](https://github.com/shayvar/structured-random-rotation-based-compression) and run `$ python setup.py install`
 
 For Ubuntu 22.04 use build and pip and other standards-based tools to build and install from source.
 
 ## Testing
 
 ### Basic
```

### Comparing `srrcomp-0.1.1/README.md` & `srrcomp-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 Windows: `$ pip install srrcomp --extra-index-url https://download.pytorch.org/whl/ --no-cache`
 
 If the message *"Faster CUDA implementation for Hadamard and bit packing is not available. Using torch implementation instead."* appears when importing srrcomp on a GPU machine, try installing `srrcomp` from source.
 
 ### Install from source
 
-For Windows and Ubuntu versions earlier than 22.04, dowload source from [the official repository](https://github.com/shayvar/structured-random-rotation-based-compression) and run `$ python setup.py install`
+For Windows and Ubuntu versions earlier than 22.04, download source from [the official repository](https://github.com/shayvar/structured-random-rotation-based-compression) and run `$ python setup.py install`
 
 For Ubuntu 22.04 use build and pip and other standards-based tools to build and install from source.
 
 ## Testing
 
 ### Basic
```

### Comparing `srrcomp-0.1.1/setup.py` & `srrcomp-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='srrcomp',
-    version='0.1.1',
+    version='0.1.2',
     description='Structured random rotation (srr) based compression tools',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Shay Vargaftik and Yaniv Ben-Itzhak',
     author_email='shayv@vmware.com, ybenitzhak@vmware.com',
     url='https://github.com/shayvar/structured-random-rotation-based-compression',
     license='BSD-3-Clause',
```

### Comparing `srrcomp-0.1.1/src/srrcomp/eden_utils/csrc/cuda_hadamard.cu` & `srrcomp-0.1.2/src/srrcomp/eden_utils/csrc/cuda_hadamard.cu`

 * *Files 12% similar despite different names*

```diff
@@ -227,20 +227,22 @@
 	
 	cudaError_t cudaStatus = cudaSetDevice(device);
 	if (cudaStatus != cudaSuccess) 
 	{
 		fprintf(stderr, "\n*** (CPP) HadamardWithCudaNoSharedMemory failed. %s ***\n", cudaGetErrorString(cudaStatus));
 	}
 	
-	struct cudaDeviceProp prop;
-	cudaGetDeviceProperties(&prop, device);
+	int maxThreadsPerBlock;
 
-	int radix2_num_threads = (n >> 1) < prop.maxThreadsPerBlock ? (n >> 1) : prop.maxThreadsPerBlock;
-	int radix4_num_threads = (n >> 2) < prop.maxThreadsPerBlock ? (n >> 2) : prop.maxThreadsPerBlock;
-	int radix8_num_threads = (n >> 3) < prop.maxThreadsPerBlock ? (n >> 3) : prop.maxThreadsPerBlock;
+	// read the following attribute from the cuda device
+	cudaDeviceGetAttribute(&maxThreadsPerBlock, cudaDevAttrMaxThreadsPerBlock, device);
+
+	int radix2_num_threads = (n >> 1) < maxThreadsPerBlock ? (n >> 1) : maxThreadsPerBlock;
+	int radix4_num_threads = (n >> 2) < maxThreadsPerBlock ? (n >> 2) : maxThreadsPerBlock;
+	int radix8_num_threads = (n >> 3) < maxThreadsPerBlock ? (n >> 3) : maxThreadsPerBlock;
 
 	int log2n = (int)log2(n);
 	int len = 1;
 
 	if ((log2n % 3) % 2 != 0) 
 	{
 		HadamardRadix2Iteration <<< (n >> 1) / radix2_num_threads, radix2_num_threads >>> (vec, len);
@@ -276,21 +278,25 @@
 	
 	cudaError_t cudaStatus = cudaSetDevice(device);
 	if (cudaStatus != cudaSuccess) 
 	{
 		fprintf(stderr, "\n*** (CPP) HadamardWithCuda failed. %s ***\n", cudaGetErrorString(cudaStatus));
 	}
 
-	struct cudaDeviceProp prop;
-	cudaGetDeviceProperties(&prop, device);
+	int maxThreadsPerBlock;
+	int sharedMemPerBlock;
+
+	// read the following attributes from the cuda device
+	cudaDeviceGetAttribute(&maxThreadsPerBlock, cudaDevAttrMaxThreadsPerBlock, device);
+	cudaDeviceGetAttribute(&sharedMemPerBlock, cudaDevAttrMaxSharedMemoryPerBlock, device);
 
 	int log2n = (int)log2(n);
 
 	// constraint on block's shared memory size
-	int sharedMemPerBlockfFloats = (int)prop.sharedMemPerBlock / sizeof(float);
+	int sharedMemPerBlockfFloats = sharedMemPerBlock / sizeof(float);
 	int log2nSharedMemPerBlockfFloats = (int)log2(sharedMemPerBlockfFloats);
 	int sharedMemIters = log2nSharedMemPerBlockfFloats > log2n ? log2n : log2nSharedMemPerBlockfFloats;
 
 	// must ensure that only radix8 iterations remain after shared memory iterations
 	if ((log2n - sharedMemIters) % 3 == 2) 
 	{
 		sharedMemIters -= 1;
@@ -311,20 +317,20 @@
 
 	if (sharedMemSize == 2) 
 	{
 		num_threads = 1;
 	}
 	else 
 	{
-		num_threads = (sharedMemSize >> 2) < prop.maxThreadsPerBlock ? (sharedMemSize >> 2) : prop.maxThreadsPerBlock;
+		num_threads = (sharedMemSize >> 2) < maxThreadsPerBlock ? (sharedMemSize >> 2) : maxThreadsPerBlock;
 	}
 
 	HadamardSharedMemoryIterations <<< num_blocks, num_threads, sharedMemSize * sizeof(float) >>> (vec, sharedMemIters);
 
-	int radix8_num_threads = (n >> 3) < prop.maxThreadsPerBlock ? (n >> 3) : prop.maxThreadsPerBlock;
+	int radix8_num_threads = (n >> 3) < maxThreadsPerBlock ? (n >> 3) : maxThreadsPerBlock;
 
 	// complete the transform	
 	for (int len = sharedMemSize; len < n; len <<= 3) 
 	{
 		HadamardRadix8Iteration <<< (n >> 3) / radix8_num_threads, radix8_num_threads >>> (vec, len);
 	}
```

### Comparing `srrcomp-0.1.1/src/srrcomp/eden_utils/csrc/cuda_packing.cu` & `srrcomp-0.1.2/src/srrcomp/eden_utils/csrc/cuda_packing.cu`

 * *Files identical despite different names*

### Comparing `srrcomp-0.1.1/src/srrcomp/eden_utils/csrc/defs.h` & `srrcomp-0.1.2/src/srrcomp/eden_utils/csrc/defs.h`

 * *Files identical despite different names*

### Comparing `srrcomp-0.1.1/src/srrcomp/eden_utils/eden_utils.cpp` & `srrcomp-0.1.2/src/srrcomp/eden_utils/eden_utils.cpp`

 * *Files identical despite different names*

### Comparing `srrcomp-0.1.1/src/srrcomp/srrcomp.py` & `srrcomp-0.1.2/src/srrcomp/srrcomp.py`

 * *Files identical despite different names*

### Comparing `srrcomp-0.1.1/src/srrcomp.egg-info/PKG-INFO` & `srrcomp-0.1.2/src/srrcomp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srrcomp
-Version: 0.1.1
+Version: 0.1.2
 Summary: Structured random rotation (srr) based compression tools
 Home-page: https://github.com/shayvar/structured-random-rotation-based-compression
 Author: Shay Vargaftik and Yaniv Ben-Itzhak
 Author-email: shayv@vmware.com, ybenitzhak@vmware.com
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -59,15 +59,15 @@
 
 Windows: `$ pip install srrcomp --extra-index-url https://download.pytorch.org/whl/ --no-cache`
 
 If the message *"Faster CUDA implementation for Hadamard and bit packing is not available. Using torch implementation instead."* appears when importing srrcomp on a GPU machine, try installing `srrcomp` from source.
 
 ### Install from source
 
-For Windows and Ubuntu versions earlier than 22.04, dowload source from [the official repository](https://github.com/shayvar/structured-random-rotation-based-compression) and run `$ python setup.py install`
+For Windows and Ubuntu versions earlier than 22.04, download source from [the official repository](https://github.com/shayvar/structured-random-rotation-based-compression) and run `$ python setup.py install`
 
 For Ubuntu 22.04 use build and pip and other standards-based tools to build and install from source.
 
 ## Testing
 
 ### Basic
```

### Comparing `srrcomp-0.1.1/src/srrcomp.egg-info/SOURCES.txt` & `srrcomp-0.1.2/src/srrcomp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

