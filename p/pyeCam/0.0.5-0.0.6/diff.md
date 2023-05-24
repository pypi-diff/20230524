# Comparing `tmp/pyeCam-0.0.5.tar.gz` & `tmp/pyeCam-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeCam-0.0.5.tar", last modified: Wed May 24 09:13:18 2023, max compression
+gzip compressed data, was "pyeCam-0.0.6.tar", last modified: Wed May 24 09:26:43 2023, max compression
```

## Comparing `pyeCam-0.0.5.tar` & `pyeCam-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:18.782615 pyeCam-0.0.5/
--rw-rw-rw-   0        0        0      151 2023-05-24 09:13:18.782615 pyeCam-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    15289 2023-05-24 09:12:52.000000 pyeCam-0.0.5/pyeCam.cpp
-drwxrwxrwx   0        0        0        0 2023-05-24 09:13:18.782615 pyeCam-0.0.5/pyeCam.egg-info/
--rw-rw-rw-   0        0        0      151 2023-05-24 09:13:18.000000 pyeCam-0.0.5/pyeCam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-05-24 09:13:18.000000 pyeCam-0.0.5/pyeCam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 09:13:18.000000 pyeCam-0.0.5/pyeCam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-24 09:13:18.000000 pyeCam-0.0.5/pyeCam.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-05-24 09:13:18.000000 pyeCam-0.0.5/pyeCam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 09:13:18.782615 pyeCam-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1973 2023-05-24 09:09:56.000000 pyeCam-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:26:43.795782 pyeCam-0.0.6/
+-rw-rw-rw-   0        0        0      151 2023-05-24 09:26:43.794711 pyeCam-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    15664 2023-05-24 09:26:16.000000 pyeCam-0.0.6/pyeCam.cpp
+drwxrwxrwx   0        0        0        0 2023-05-24 09:26:43.794711 pyeCam-0.0.6/pyeCam.egg-info/
+-rw-rw-rw-   0        0        0      151 2023-05-24 09:26:43.000000 pyeCam-0.0.6/pyeCam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-05-24 09:26:43.000000 pyeCam-0.0.6/pyeCam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 09:26:43.000000 pyeCam-0.0.6/pyeCam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-24 09:26:43.000000 pyeCam-0.0.6/pyeCam.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-05-24 09:26:43.000000 pyeCam-0.0.6/pyeCam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 09:26:43.795782 pyeCam-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1973 2023-05-24 09:25:35.000000 pyeCam-0.0.6/setup.py
```

### Comparing `pyeCam-0.0.5/pyeCam.cpp` & `pyeCam-0.0.6/pyeCam.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 #include <windows.h>
 #include <objbase.h>
 #include <dshow.h>
 #include <tchar.h>
 #include <uuids.h>
 #include <WinError.h>
 #include <OleAuto.h>
+#include <iostream>
+#include <exception>
+
 
 #define	DB_LOW						0x01
 #define TOF_VID L"2560"
 #define TOF_PID L"C0D6"
 
 namespace py = pybind11;
 
@@ -56,19 +59,27 @@
 	bool isValidIndex(uint32_t deviceIndex) 
 	{
 		printf("isValidIndex - is inside a method");
 		pybind11::object py_deviceCount;
 		py_deviceCount.attr("value") = 0;
 uint32_t device_count;
 printf("isValidIndex - is inside a method - Before if method");
+try
+{
 	if (getDeviceCount(py_deviceCount) == false)
 	{ 
 printf("if valid index failed");
 		return false;
 	}
+}
+catch (const std::exception& ex) 
+{
+    std::cout << "Exception caught: " << ex.what() << std::endl;
+}
+	
 printf("Before py_deviceCount.cast<uint32_t>()");
 device_count = py_deviceCount.cast<uint32_t>();
 printf("Device count %d\n", device_count);
 device_count = pybind11::int_(py_deviceCount.attr("value").cast<int>()) ;
 
 		printf("Device count After attr  %d\n",device_count);
 		
@@ -166,16 +177,20 @@
 							pid_substr = wcsstr(wcsupr(devicePath), TEXT("PID_"));
 
 							if (pid_substr != NULL)
 							{
 								wcsncpy_s(extrctd_pid, pid_substr + 4, 4);
 								extrctd_pid[5] = '\0';
 							}
+							  if ((wcscmp(wcsupr(extrctd_vid), TOF_VID) == 0) && (wcscmp(wcsupr(extrctd_pid), TOF_PID) == 0))
+					  {
+
 								indexList |= (1 << Count);
 								Count++;
+					  }
 						}
 						SysFreeString(var.bstrVal);
 					}
 					pM->AddRef();
 				}
 				else
 				{
@@ -191,15 +206,17 @@
 	  return false;
   	}
 	return true;
   }
   
 	bool getDeviceCount(pybind11::object& gDeviceCount) 
 	{
+		printf(" getDeviceCount called");
 	  initialize();
+	  printf(" getDeviceCount initialize()");
 	  int list = indexList;
 	  gDeviceCount.attr("value") = 0;
 	  if (!indexList) 
 	  {
 		printf(" getDeviceCount Device count failed");
 		 return false;
 	  }
```

### Comparing `pyeCam-0.0.5/setup.py` & `pyeCam-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             ext.extra_compile_args = extra_compile_args
             ext.extra_link_args = extra_link_args
         build_ext.build_extensions(self)
 
 # Setup configuration
 setup(
     name='pyeCam',
-    version='0.0.5',
+    version='0.0.6',
     description='Example project using pybind11',
     author='Your Name',
     author_email='your_email@example.com',
     ext_modules=[ext_module],
     cmdclass={'build_ext': BuildExt},
     zip_safe=False
 )
```

