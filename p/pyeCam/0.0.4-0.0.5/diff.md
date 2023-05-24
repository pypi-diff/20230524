# Comparing `tmp/pyeCam-0.0.4.tar.gz` & `tmp/pyeCam-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeCam-0.0.4.tar", last modified: Wed May 24 08:08:38 2023, max compression
+gzip compressed data, was "pyeCam-0.0.5.tar", last modified: Wed May 24 09:13:18 2023, max compression
```

## Comparing `pyeCam-0.0.4.tar` & `pyeCam-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 08:08:38.341253 pyeCam-0.0.4/
--rw-rw-rw-   0        0        0      151 2023-05-24 08:08:38.341253 pyeCam-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    14877 2023-05-24 08:06:40.000000 pyeCam-0.0.4/pyeCam.cpp
-drwxrwxrwx   0        0        0        0 2023-05-24 08:08:38.340333 pyeCam-0.0.4/pyeCam.egg-info/
--rw-rw-rw-   0        0        0      151 2023-05-24 08:08:38.000000 pyeCam-0.0.4/pyeCam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-05-24 08:08:38.000000 pyeCam-0.0.4/pyeCam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 08:08:38.000000 pyeCam-0.0.4/pyeCam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-24 08:08:38.000000 pyeCam-0.0.4/pyeCam.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-05-24 08:08:38.000000 pyeCam-0.0.4/pyeCam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 08:08:38.342251 pyeCam-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1973 2023-05-24 08:08:00.000000 pyeCam-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:13:18.782615 pyeCam-0.0.5/
+-rw-rw-rw-   0        0        0      151 2023-05-24 09:13:18.782615 pyeCam-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    15289 2023-05-24 09:12:52.000000 pyeCam-0.0.5/pyeCam.cpp
+drwxrwxrwx   0        0        0        0 2023-05-24 09:13:18.782615 pyeCam-0.0.5/pyeCam.egg-info/
+-rw-rw-rw-   0        0        0      151 2023-05-24 09:13:18.000000 pyeCam-0.0.5/pyeCam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-05-24 09:13:18.000000 pyeCam-0.0.5/pyeCam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 09:13:18.000000 pyeCam-0.0.5/pyeCam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-24 09:13:18.000000 pyeCam-0.0.5/pyeCam.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-05-24 09:13:18.000000 pyeCam-0.0.5/pyeCam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 09:13:18.782615 pyeCam-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1973 2023-05-24 09:09:56.000000 pyeCam-0.0.5/setup.py
```

### Comparing `pyeCam-0.0.4/pyeCam.cpp` & `pyeCam-0.0.5/pyeCam.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -51,26 +51,30 @@
 
 			OutputDebugString(szBuffer);
 		}
 	}
 	 
 	bool isValidIndex(uint32_t deviceIndex) 
 	{
+		printf("isValidIndex - is inside a method");
 		pybind11::object py_deviceCount;
+		py_deviceCount.attr("value") = 0;
 uint32_t device_count;
-
+printf("isValidIndex - is inside a method - Before if method");
 	if (getDeviceCount(py_deviceCount) == false)
 	{ 
 printf("if valid index failed");
 		return false;
 	}
-
+printf("Before py_deviceCount.cast<uint32_t>()");
 device_count = py_deviceCount.cast<uint32_t>();
+printf("Device count %d\n", device_count);
+device_count = pybind11::int_(py_deviceCount.attr("value").cast<int>()) ;
 
-		printf("Device count %d\n", device_count);
+		printf("Device count After attr  %d\n",device_count);
 		
 		if (deviceIndex > device_count || deviceIndex < 0)
 		{
 			return false;
 		}
 	  
 	  return true;
@@ -223,14 +227,15 @@
   }
   
 	bool getDeviceInfo(uint32_t deviceIndex,DeviceInfo* gDevice) 
 	{
 	  printf("getDeviceInfo");
 	  try
 	  {
+		  printf("getDeviceInfo - inside printf");
 		  TCHAR devicePath[MAX_PATH] = _T("");
 		  TCHAR deviceName[MAX_PATH] = _T("");
 		  TCHAR extrctd_vid[10] = _T("");
 		  TCHAR extrctd_pid[10] = _T("");
 		  TCHAR* vid_substr;
 		  TCHAR* pid_substr;
 		  TCHAR device_name[MAX_PATH] = _T("");
@@ -239,15 +244,15 @@
 		  std::string str;
 		  HRESULT hr;
 		  ULONG cFetched;
 		  IMoniker* pM;
 		  ICreateDevEnum* pCreateDevEnum = 0;
 		  IEnumMoniker* pEm = 0;
 		  UINT8 Count = 0;
-		  
+		  printf("getDeviceInfo - isValidIndex");
 		  //if (isValidIndex(deviceIndex) < 0) 
 		  if (!isValidIndex(deviceIndex)) 
 		  {
 			  printf("InvalidDeviceIndex");
 			  return false;
 			 // return DEPTHVISTAError::setErrno(Result::InvalidDeviceIndex);
 		  }
```

### Comparing `pyeCam-0.0.4/setup.py` & `pyeCam-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             ext.extra_compile_args = extra_compile_args
             ext.extra_link_args = extra_link_args
         build_ext.build_extensions(self)
 
 # Setup configuration
 setup(
     name='pyeCam',
-    version='0.0.4',
+    version='0.0.5',
     description='Example project using pybind11',
     author='Your Name',
     author_email='your_email@example.com',
     ext_modules=[ext_module],
     cmdclass={'build_ext': BuildExt},
     zip_safe=False
 )
```

