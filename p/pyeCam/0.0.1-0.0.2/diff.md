# Comparing `tmp/pyeCam-0.0.1.tar.gz` & `tmp/pyeCam-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeCam-0.0.1.tar", last modified: Tue May 23 09:49:09 2023, max compression
+gzip compressed data, was "pyeCam-0.0.2.tar", last modified: Wed May 24 07:36:47 2023, max compression
```

## Comparing `pyeCam-0.0.1.tar` & `pyeCam-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 09:49:09.944285 pyeCam-0.0.1/
--rw-rw-rw-   0        0        0      151 2023-05-23 09:49:09.928545 pyeCam-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    13321 2023-05-23 09:29:46.000000 pyeCam-0.0.1/pyeCam.cpp
-drwxrwxrwx   0        0        0        0 2023-05-23 09:49:09.928545 pyeCam-0.0.1/pyeCam.egg-info/
--rw-rw-rw-   0        0        0      151 2023-05-23 09:49:09.000000 pyeCam-0.0.1/pyeCam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-05-23 09:49:09.000000 pyeCam-0.0.1/pyeCam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 09:49:09.000000 pyeCam-0.0.1/pyeCam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-23 09:49:09.000000 pyeCam-0.0.1/pyeCam.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-05-23 09:49:09.000000 pyeCam-0.0.1/pyeCam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 09:49:09.944285 pyeCam-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1973 2023-05-23 09:48:12.000000 pyeCam-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:36:47.917885 pyeCam-0.0.2/
+-rw-rw-rw-   0        0        0      151 2023-05-24 07:36:47.917885 pyeCam-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10525 2023-05-24 07:34:36.000000 pyeCam-0.0.2/pyeCam.cpp
+drwxrwxrwx   0        0        0        0 2023-05-24 07:36:47.917885 pyeCam-0.0.2/pyeCam.egg-info/
+-rw-rw-rw-   0        0        0      151 2023-05-24 07:36:47.000000 pyeCam-0.0.2/pyeCam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-05-24 07:36:47.000000 pyeCam-0.0.2/pyeCam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 07:36:47.000000 pyeCam-0.0.2/pyeCam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-24 07:36:47.000000 pyeCam-0.0.2/pyeCam.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-05-24 07:36:47.000000 pyeCam-0.0.2/pyeCam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 07:36:47.917885 pyeCam-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1973 2023-05-23 10:19:41.000000 pyeCam-0.0.2/setup.py
```

### Comparing `pyeCam-0.0.1/pyeCam.cpp` & `pyeCam-0.0.2/pyeCam.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 #include <objbase.h>
 #include <dshow.h>
 #include <tchar.h>
 #include <uuids.h>
 #include <WinError.h>
 #include <OleAuto.h>
 
+#define	DB_LOW						0x01
 #define TOF_VID L"2560"
 #define TOF_PID L"C0D6"
-#define	DB_LOW						0x01
 
 namespace py = pybind11;
 
 int32_t indexList = -1;
 
 typedef struct
 {
     char deviceName[50];
     char vid[5];
     char pid[5];
     char devicePath[500];
     char serialNo[50];
 }DeviceInfo;
 
-bool getDeviceCount(uint32_t *gDeviceCount) ;
-bool getDeviceListInfo(uint32_t deviceCount,DeviceInfo* gDevicesList);
-bool getDeviceInfo(uint32_t deviceIndex,DeviceInfo* gDevice) ;
+	bool getDeviceCount(pybind11::object& gDeviceCount);
+	bool getDeviceListInfo(uint32_t deviceCount,DeviceInfo* gDevicesList);
+	bool getDeviceInfo(uint32_t deviceIndex,DeviceInfo* gDevice);
 
 	void DebugMessage(BOOL bEnable, LPTSTR szFormat, ...)
 	{
 		if (bEnable)
 		{
 			static TCHAR szBuffer[2048] = { 0 };
 			const size_t NUMCHARS = sizeof(szBuffer) / sizeof(szBuffer[0]);
@@ -51,24 +51,30 @@
 
 			OutputDebugString(szBuffer);
 		}
 	}
 	 
 	bool isValidIndex(uint32_t deviceIndex) 
 	{
-	  uint32_t device_count;
-	  
-	  if (getDeviceCount(&device_count)==false)
-	  {
-		 return false;
-	  }
-	  if (deviceIndex > device_count || deviceIndex < 0)
-	  {
-		  return false;
-	  }
+		pybind11::object py_deviceCount;
+uint32_t device_count;
+
+	if (getDeviceCount(py_deviceCount) == false)
+	{
+		return false;
+	}
+
+device_count = py_deviceCount.cast<uint32_t>();
+
+		printf("Device count %d\n", device_count);
+		
+		if (deviceIndex > device_count || deviceIndex < 0)
+		{
+			return false;
+		}
 	  
 	  return true;
 	}
 	
 	void getDevNodeNumber(uint32_t *nodeNo) 
 	{
 	  uint32_t auto_index = 0, count = 0;
@@ -94,15 +100,14 @@
 	  indexList = -1;
 	}
   
 	bool initialize() 
 	{
 		try
 		{
-	  		printf("initialize is statred\n");
 	  		CoInitializeEx(NULL, COINIT_APARTMENTTHREADED);
 	  		TCHAR devicePath[MAX_PATH] = _T("");
 	  		TCHAR extrctd_vid[10] = _T("");
 	  		TCHAR extrctd_pid[10] = _T("");
 	  		TCHAR* vid_substr;
 	  		TCHAR* pid_substr;
 	  		HRESULT hr;
@@ -116,70 +121,56 @@
 	  		indexList = 0;
 	  
 	  		hr = CoCreateInstance(CLSID_SystemDeviceEnum, NULL, CLSCTX_INPROC_SERVER,
 		  	IID_ICreateDevEnum, (void**)&pCreateDevEnum);
 	  		if (hr != NO_ERROR)
 	  		{
 		 		SetLastError(0);
-		  		printf("NotInitialized Error\n");
 		  		return false;
-		  		//return DEPTHVISTAError::setErrno(Result::NotInitialized);
 	  		}
 
 			hr = pCreateDevEnum->CreateClassEnumerator(CLSID_VideoInputDeviceCategory, &pEm, 0);
 			if (hr != NOERROR)
 			{
-				printf("NotInitialized Error\n");
 				return false;
 			}
 			pEm->Reset();
-			printf("Before While loop\n");
 			while (hr = pEm->Next(1, &pM, &cFetched), hr == S_OK)
 			{
-				printf("Entered a While loop\n");
 				IPropertyBag* pBag = 0;
 				hr = pM->BindToStorage(0, 0, IID_IPropertyBag, (void**)&pBag);
 
 				if (SUCCEEDED(hr))
 				{
-					printf(" While loop hr successed\n");
 					VARIANT var;
 					var.vt = VT_BSTR;
 					hr = pBag->Read(L"DevicePath", &var, 0);
 					if (hr == S_OK)
 					{
-						printf(" While loop hr S_OK successed\n");
 						StringCbPrintf(devicePath, MAX_PATH, L"%s", var.bstrVal);
 
 						if (devicePath != NULL)
 						{
-							printf(" While loop hr devicePath != NULL successed\n");
 							vid_substr = wcsstr(wcsupr(devicePath), TEXT("VID_"));
 
 							if (vid_substr != NULL)
 							{
 								wcsncpy_s(extrctd_vid, vid_substr + 4, 4);
 								extrctd_vid[5] = '\0';
-								printf(" While loop hr wcsncpy_s(extrctd_vid, vid_substr + 4, 4) successed\n");
 							}
 
 							pid_substr = wcsstr(wcsupr(devicePath), TEXT("PID_"));
 
 							if (pid_substr != NULL)
 							{
 								wcsncpy_s(extrctd_pid, pid_substr + 4, 4);
 								extrctd_pid[5] = '\0';
-								printf("While loop - pid_substr != NULL - wcsncpy_s(extrctd_pid, pid_substr + 4, 4);\n");
 							}
-						
-							if ((wcscmp(wcsupr(extrctd_vid), TOF_VID) == 0) && (wcscmp(wcsupr(extrctd_pid), TOF_PID) == 0))
-							{
 								indexList |= (1 << Count);
 								Count++;
-					        }
 						}
 						SysFreeString(var.bstrVal);
 					}
 					pM->AddRef();
 				}
 				else
 				{
@@ -188,70 +179,44 @@
 				pM->Release();
 			}
 			pEm->Release();
 			return true;
 		}
   	catch (...)
   	{
-	  printf("NotInitialized Error");
 	  return false;
   	}
 	return true;
   }
   
-	bool getDeviceCount1(pybind11::object& gDeviceCount) 
+	bool getDeviceCount(pybind11::object& gDeviceCount) 
 	{
 	  initialize();
 	  int list = indexList;
 	  gDeviceCount.attr("value") = 0;
 	  if (!indexList) 
 	  {
-		 printf("Device is not connected");
 		 return false;
 	  }
 	  while (list)
 	  {
-		  printf("Before list =  %d\n",list);
 		  list &= (list - 1);
-		  printf("After list =  %d\n",list);
 		  gDeviceCount.attr("value") = pybind11::int_(gDeviceCount.attr("value").cast<int>() + 1);
 	  }
 	  return true;
   }
   
-	bool getDeviceCount(uint32_t* gDeviceCount) 
-	{
-	  initialize();
-	  int list = indexList;
-	  *gDeviceCount = 0;
-	  if (!indexList) 
-	  {
-		 printf("Device is not connected");
-		 return false;
-	  }
-	  while (list)
-	  {
-		  printf("Before list =  %d\n",list);
-		  list &= (list - 1);
-		  printf("After list =  %d\n",list);
-		  printf("Before gdevice list =  %d\n",*gDeviceCount);
-		  *gDeviceCount += 1;
-		  printf("After gdevice list =  %d\n",*gDeviceCount);
-	  }
-	  return true;
-  }
   
 	bool getDeviceListInfo(uint32_t deviceCount,DeviceInfo* gDevicesList) 
 	{
 	  for (uint32_t index = 0; index < deviceCount; index++) 
 	  {
 		  DebugMessage(DB_LOW, L"Device index is : %d\n", index);
 			if (getDeviceInfo(index, (gDevicesList + index))== false) 
 			{
-			  printf("other issue");
 			  return false;
 			}
 		  DebugMessage(DB_LOW, L"Device Name is : %s\n", (gDevicesList + index)->deviceName);
 	  }
 	 return true;
   }
   
@@ -350,15 +315,14 @@
 				  }
 				  pM->AddRef();
 
 			  }
 			  else
 			  {
 				  pEm->Release();
-				  printf("NotInitialized");
 				  return false;
 			  }
 			  pM->Release();
 		  }
 		  pEm->Release();
 		 return true;
 	  }
@@ -373,98 +337,65 @@
 	PYBIND11_MODULE(pyeCam, m)
 	{
     	m.def("getDeviceInfo", &getDeviceInfo, "getDeviceInfo");
 		m.def("getDeviceListInfo", &getDeviceListInfo, "getDeviceListInfo");
 		m.def("getDeviceCount", &getDeviceCount, R"pbdoc(Get device count)pbdoc");
 		 
 		py::class_<DeviceInfo>(m, "DeviceInfo")
-        .def(py::init<>())
-        .def_property("deviceName",
-            [](const DeviceInfo& info) {
-                return py::array(py::buffer_info(
-                    const_cast<char*>(info.deviceName),
-                    sizeof(char),
-                    py::format_descriptor<char>::format(),
-                    1,
-                    {50},
-                    {sizeof(char)}
-                ));
-            },
-            [](DeviceInfo& info, const py::array_t<char>& arr) {
-                auto buf = arr.request();
-                if (buf.size != 50)
-                    throw std::runtime_error("Invalid array size");
-                std::memcpy(info.deviceName, buf.ptr, buf.size * sizeof(char));
-            }
-        )
-        .def_property("vid",
-            [](const DeviceInfo& info) {
-                return py::array(py::buffer_info(
-                    const_cast<char*>(info.vid),
-                    sizeof(char),
-                    py::format_descriptor<char>::format(),
-                    1,
-                    {5},
-                    {sizeof(char)}
-                ));
-            },
-            [](DeviceInfo& info, const py::array_t<char>& arr) {
-                auto buf = arr.request();
-                if (buf.size != 5)
-                    throw std::runtime_error("Invalid array size");
-                std::memcpy(info.vid, buf.ptr, buf.size * sizeof(char));
-            }
-        )
-        .def_property("pid",
-            [](const DeviceInfo& info) {
-                return py::array(py::buffer_info(
-                    const_cast<char*>(info.pid),
-                    sizeof(char),
-                    py::format_descriptor<char>::format(),
-                    1,
-                    {5},
-                    {sizeof(char)}
-                ));
-            },
-            [](DeviceInfo& info, const py::array_t<char>& arr) {
-                auto buf = arr.request();
-                if (buf.size != 5)
-                    throw std::runtime_error("Invalid array size");
-                std::memcpy(info.pid, buf.ptr, buf.size * sizeof(char));
-            }
-        )
-        .def_property("devicePath",
-            [](const DeviceInfo& info) {
-                return py::array(py::buffer_info(
-                    const_cast<char*>(info.devicePath),
-                    sizeof(char),
-                    py::format_descriptor<char>::format(),
-                    1,
-                    {500},
-                    {sizeof(char)}
-                ));
-            },
-            [](DeviceInfo& info, const py::array_t<char>& arr) {
-                auto buf = arr.request();
-                if (buf.size != 500)
-                    throw std::runtime_error("Invalid array size");
-                std::memcpy(info.devicePath, buf.ptr, buf.size * sizeof(char));
-            }
-        )
-        .def_property("serialNo",
-            [](const DeviceInfo& info) {
-                return py::array(py::buffer_info(
-                    const_cast<char*>(info.serialNo),
-                    sizeof(char),
-                    py::format_descriptor<char>::format(),
-                    1,
-                    {50},
-                    {sizeof(char)}
-                ));
-            },
-            [](DeviceInfo& info, const py::array_t<char>& arr) {
-                auto buf = arr.request();
-                if (buf.size != 50)
-                    throw std::runtime_error("Invalid array size");
-               std::memcpy(info.serialNo, buf.ptr, buf.size * sizeof(char));}
-);
+    .def(py::init<>())
+    .def_property("deviceName",
+        [](const DeviceInfo& info) {
+            return std::string(info.deviceName);
+        },
+        [](DeviceInfo& info, const std::string& value) {
+            if (value.size() >= 50)
+                throw std::runtime_error("Invalid string size");
+            std::memcpy(info.deviceName, value.c_str(), value.size());
+            info.deviceName[value.size()] = '\0';
+        }
+    )
+    .def_property("vid",
+        [](const DeviceInfo& info) {
+            return std::string(info.vid);
+        },
+        [](DeviceInfo& info, const std::string& value) {
+            if (value.size() >= 5)
+                throw std::runtime_error("Invalid string size");
+            std::memcpy(info.vid, value.c_str(), value.size());
+            info.vid[value.size()] = '\0';
+        }
+    )
+    .def_property("pid",
+        [](const DeviceInfo& info) {
+            return std::string(info.pid);
+        },
+        [](DeviceInfo& info, const std::string& value) {
+            if (value.size() >= 5)
+                throw std::runtime_error("Invalid string size");
+            std::memcpy(info.pid, value.c_str(), value.size());
+            info.pid[value.size()] = '\0';
+        }
+    )
+    .def_property("devicePath",
+        [](const DeviceInfo& info) {
+            return std::string(info.devicePath);
+        },
+        [](DeviceInfo& info, const std::string& value) {
+            if (value.size() >= 500)
+                throw std::runtime_error("Invalid string size");
+            std::memcpy(info.devicePath, value.c_str(), value.size());
+            info.devicePath[value.size()] = '\0';
+        }
+    )
+    .def_property("serialNo",
+        [](const DeviceInfo& info) {
+            return std::string(info.serialNo);
+        },
+        [](DeviceInfo& info, const std::string& value) {
+            if (value.size() >= 50)
+                throw std::runtime_error("Invalid string size");
+            std::memcpy(info.serialNo, value.c_str(), value.size());
+            info.serialNo[value.size()] = '\0';
+        }
+    );
+
 	}
```

### Comparing `pyeCam-0.0.1/setup.py` & `pyeCam-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             ext.extra_compile_args = extra_compile_args
             ext.extra_link_args = extra_link_args
         build_ext.build_extensions(self)
 
 # Setup configuration
 setup(
     name='pyeCam',
-    version='0.0.1',
+    version='0.0.2',
     description='Example project using pybind11',
     author='Your Name',
     author_email='your_email@example.com',
     ext_modules=[ext_module],
     cmdclass={'build_ext': BuildExt},
     zip_safe=False
 )
```

