# Comparing `tmp/pyeCam-0.0.2.tar.gz` & `tmp/pyeCam-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeCam-0.0.2.tar", last modified: Wed May 24 07:36:47 2023, max compression
+gzip compressed data, was "pyeCam-0.0.3.tar", last modified: Wed May 24 07:58:30 2023, max compression
```

## Comparing `pyeCam-0.0.2.tar` & `pyeCam-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 07:36:47.917885 pyeCam-0.0.2/
--rw-rw-rw-   0        0        0      151 2023-05-24 07:36:47.917885 pyeCam-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    10525 2023-05-24 07:34:36.000000 pyeCam-0.0.2/pyeCam.cpp
-drwxrwxrwx   0        0        0        0 2023-05-24 07:36:47.917885 pyeCam-0.0.2/pyeCam.egg-info/
--rw-rw-rw-   0        0        0      151 2023-05-24 07:36:47.000000 pyeCam-0.0.2/pyeCam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-05-24 07:36:47.000000 pyeCam-0.0.2/pyeCam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 07:36:47.000000 pyeCam-0.0.2/pyeCam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-24 07:36:47.000000 pyeCam-0.0.2/pyeCam.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-05-24 07:36:47.000000 pyeCam-0.0.2/pyeCam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 07:36:47.917885 pyeCam-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1973 2023-05-23 10:19:41.000000 pyeCam-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:58:30.612330 pyeCam-0.0.3/
+-rw-rw-rw-   0        0        0      151 2023-05-24 07:58:30.611248 pyeCam-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11231 2023-05-24 07:55:55.000000 pyeCam-0.0.3/pyeCam.cpp
+drwxrwxrwx   0        0        0        0 2023-05-24 07:58:30.611248 pyeCam-0.0.3/pyeCam.egg-info/
+-rw-rw-rw-   0        0        0      151 2023-05-24 07:58:30.000000 pyeCam-0.0.3/pyeCam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-05-24 07:58:30.000000 pyeCam-0.0.3/pyeCam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 07:58:30.000000 pyeCam-0.0.3/pyeCam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-24 07:58:30.000000 pyeCam-0.0.3/pyeCam.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-05-24 07:58:30.000000 pyeCam-0.0.3/pyeCam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 07:58:30.612330 pyeCam-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1973 2023-05-24 07:57:41.000000 pyeCam-0.0.3/setup.py
```

### Comparing `pyeCam-0.0.2/pyeCam.cpp` & `pyeCam-0.0.3/pyeCam.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -55,15 +55,16 @@
 	 
 	bool isValidIndex(uint32_t deviceIndex) 
 	{
 		pybind11::object py_deviceCount;
 uint32_t device_count;
 
 	if (getDeviceCount(py_deviceCount) == false)
-	{
+	{ 
+printf("if valid index failed");
 		return false;
 	}
 
 device_count = py_deviceCount.cast<uint32_t>();
 
 		printf("Device count %d\n", device_count);
 		
@@ -191,14 +192,15 @@
 	bool getDeviceCount(pybind11::object& gDeviceCount) 
 	{
 	  initialize();
 	  int list = indexList;
 	  gDeviceCount.attr("value") = 0;
 	  if (!indexList) 
 	  {
+		printf(" getDeviceCount Device count failed");
 		 return false;
 	  }
 	  while (list)
 	  {
 		  list &= (list - 1);
 		  gDeviceCount.attr("value") = pybind11::int_(gDeviceCount.attr("value").cast<int>() + 1);
 	  }
@@ -218,14 +220,15 @@
 		  DebugMessage(DB_LOW, L"Device Name is : %s\n", (gDevicesList + index)->deviceName);
 	  }
 	 return true;
   }
   
 	bool getDeviceInfo(uint32_t deviceIndex,DeviceInfo* gDevice) 
 	{
+	  printf("getDeviceInfo");
 	  try
 	  {
 		  TCHAR devicePath[MAX_PATH] = _T("");
 		  TCHAR deviceName[MAX_PATH] = _T("");
 		  TCHAR extrctd_vid[10] = _T("");
 		  TCHAR extrctd_pid[10] = _T("");
 		  TCHAR* vid_substr;
@@ -236,33 +239,40 @@
 		  std::string str;
 		  HRESULT hr;
 		  ULONG cFetched;
 		  IMoniker* pM;
 		  ICreateDevEnum* pCreateDevEnum = 0;
 		  IEnumMoniker* pEm = 0;
 		  UINT8 Count = 0;
+		  
+		  //if (isValidIndex(deviceIndex) < 0) 
 		  if (!isValidIndex(deviceIndex)) 
 		  {
+			  printf("InvalidDeviceIndex");
 			  return false;
+			 // return DEPTHVISTAError::setErrno(Result::InvalidDeviceIndex);
 		  }
 		  getDevNodeNumber(&deviceIndex);
 		  hr = CoCreateInstance(CLSID_SystemDeviceEnum, NULL, CLSCTX_INPROC_SERVER,
 			  IID_ICreateDevEnum, (void**)&pCreateDevEnum);
 		  if (hr != NO_ERROR)
 		  {
 			  SetLastError(0);
+			   printf("NotInitialized");
 			  return false;
+			 // return DEPTHVISTAError::setErrno(Result::NotInitialized);
 		  }
 
 		  hr = pCreateDevEnum->CreateClassEnumerator(CLSID_VideoInputDeviceCategory, &pEm, 0);
 		  if (hr != NOERROR)
 		  {
+			   printf("NotInitialized");
 			  return false;
+			 // return DEPTHVISTAError::setErrno(Result::NotInitialized);
 		  }
-		  
 		  pEm->Reset();
 
 		  while (hr = pEm->Next(1, &pM, &cFetched), hr == S_OK)
 		  {
 			  IPropertyBag* pBag = 0;
 			  hr = pM->BindToStorage(0, 0, IID_IPropertyBag, (void**)&pBag);
 
@@ -315,29 +325,33 @@
 				  }
 				  pM->AddRef();
 
 			  }
 			  else
 			  {
 				  pEm->Release();
+				  printf("NotInitialized");
 				  return false;
+				 // return DEPTHVISTAError::setErrno(Result::NotInitialized);
 			  }
 			  pM->Release();
 		  }
 		  pEm->Release();
+		 // return DEPTHVISTAError::setErrno(Result::Ok);
 		 return true;
 	  }
 	  catch (...)
 	  {
 		  DebugMessage(DB_LOW, L"Exception EnumerateVideoDevices....\r\n");
-		  return false;
+		  //return DEPTHVISTAError::setErrno(Result::NotInitialized);
+		  printf("NotInitialized");
+			  return false;
 	  }
   }
-  
-  
+	
 	PYBIND11_MODULE(pyeCam, m)
 	{
     	m.def("getDeviceInfo", &getDeviceInfo, "getDeviceInfo");
 		m.def("getDeviceListInfo", &getDeviceListInfo, "getDeviceListInfo");
 		m.def("getDeviceCount", &getDeviceCount, R"pbdoc(Get device count)pbdoc");
 		 
 		py::class_<DeviceInfo>(m, "DeviceInfo")
```

### Comparing `pyeCam-0.0.2/setup.py` & `pyeCam-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             ext.extra_compile_args = extra_compile_args
             ext.extra_link_args = extra_link_args
         build_ext.build_extensions(self)
 
 # Setup configuration
 setup(
     name='pyeCam',
-    version='0.0.2',
+    version='0.0.3',
     description='Example project using pybind11',
     author='Your Name',
     author_email='your_email@example.com',
     ext_modules=[ext_module],
     cmdclass={'build_ext': BuildExt},
     zip_safe=False
 )
```

