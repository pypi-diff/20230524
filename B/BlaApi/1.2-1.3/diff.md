# Comparing `tmp/BlaApi-1.2.tar.gz` & `tmp/BlaApi-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlaApi-1.2.tar", last modified: Sun Apr 16 17:07:41 2023, max compression
+gzip compressed data, was "BlaApi-1.3.tar", last modified: Wed May 24 21:54:38 2023, max compression
```

## Comparing `BlaApi-1.2.tar` & `BlaApi-1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 17:07:41.855654 BlaApi-1.2/
-drwxrwxrwx   0        0        0        0 2023-04-16 17:07:41.842660 BlaApi-1.2/BlaApi/
--rw-rw-rw-   0        0        0        0 2023-04-16 12:18:24.000000 BlaApi-1.2/BlaApi/__init__.py
--rw-rw-rw-   0        0        0     3568 2023-04-16 15:55:24.000000 BlaApi-1.2/BlaApi/client.py
--rw-rw-rw-   0        0        0     3923 2023-04-16 16:19:00.000000 BlaApi-1.2/BlaApi/diary.py
-drwxrwxrwx   0        0        0        0 2023-04-16 17:07:41.852657 BlaApi-1.2/BlaApi.egg-info/
--rw-rw-rw-   0        0        0     5890 2023-04-16 17:07:41.000000 BlaApi-1.2/BlaApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-04-16 17:07:41.000000 BlaApi-1.2/BlaApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 17:07:41.000000 BlaApi-1.2/BlaApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-16 17:07:41.000000 BlaApi-1.2/BlaApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-16 17:07:41.000000 BlaApi-1.2/BlaApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-04-16 12:18:24.000000 BlaApi-1.2/LICENSE
--rw-rw-rw-   0        0        0     5890 2023-04-16 17:07:41.854655 BlaApi-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5239 2023-04-16 17:06:18.000000 BlaApi-1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-16 17:07:41.855654 BlaApi-1.2/setup.cfg
--rw-rw-rw-   0        0        0     3706 2023-04-16 17:07:17.000000 BlaApi-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 21:54:38.733148 BlaApi-1.3/
+drwxrwxrwx   0        0        0        0 2023-05-24 21:54:38.723631 BlaApi-1.3/BlaApi/
+-rw-rw-rw-   0        0        0        0 2023-04-16 12:18:24.000000 BlaApi-1.3/BlaApi/__init__.py
+-rw-rw-rw-   0        0        0     4012 2023-05-24 21:45:48.000000 BlaApi-1.3/BlaApi/client.py
+-rw-rw-rw-   0        0        0     3857 2023-05-24 21:48:54.000000 BlaApi-1.3/BlaApi/diary.py
+drwxrwxrwx   0        0        0        0 2023-05-24 21:54:38.731130 BlaApi-1.3/BlaApi.egg-info/
+-rw-rw-rw-   0        0        0     6155 2023-05-24 21:54:38.000000 BlaApi-1.3/BlaApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-24 21:54:38.000000 BlaApi-1.3/BlaApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 21:54:38.000000 BlaApi-1.3/BlaApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-05-24 21:54:38.000000 BlaApi-1.3/BlaApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-24 21:54:38.000000 BlaApi-1.3/BlaApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-04-16 12:18:24.000000 BlaApi-1.3/LICENSE
+-rw-rw-rw-   0        0        0     6155 2023-05-24 21:54:38.733148 BlaApi-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5504 2023-05-24 21:49:00.000000 BlaApi-1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-24 21:54:38.734152 BlaApi-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     3712 2023-05-24 21:54:24.000000 BlaApi-1.3/setup.py
```

### Comparing `BlaApi-1.2/BlaApi/client.py` & `BlaApi-1.3/BlaApi/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,24 +17,25 @@
     def login(self):
         # Construct API endpoint URL
         endpoint = "login"
         api_url = f"https://beaconlightacademy.edu.pk/app/restapi.php?endpoint={endpoint}&rnd=1667581678739&username={self.username}&password={self.password}"
         
         # Send POST request to API endpoint with headers
         response = self.client.post(api_url, headers=self.headers)
+        
         #! Raise an error if POST fails
         response.raise_for_status()
         
-        # Parse JSON response
+        # error handling
+        if json.loads(response.content).get('success') == False:
+            raise ValueError(json.loads(response.content).get('error'))
+        
         data = json.loads(response.content)['data']
-
         # Retrieve access token & student info from JSON response
         token = data.get('accessToken')
-        if token is None:
-            raise ValueError("Access token not found in response.")
         student_info = data.get('students')
 
         # Return student ids and student names as lists
         student_ids = [] #Initialize
         student_names = [] #Initialize
 
         for s in student_info:
@@ -59,15 +60,19 @@
     def get_diary_list(self):
         # Construct API endpoint URL
         endpoint = "diaryList"
         api_url = f"https://beaconlightacademy.edu.pk/app/restapi.php?endpoint={endpoint}&accessToken={self.token}&year=1"
         
         # Send POST request to API endpoint with headers
         response = self.client.post(api_url, headers=self.headers)
-
+        
+        # error handling
+        if json.loads(response.content).get('success') == False:
+            raise ValueError(json.loads(response.content).get('error'))
+        
         #! Raise an error if POST fails
         response.raise_for_status()
         
         # Retreive diary list from JSON response
         data = json.loads(response.content)['data']
         
         return data
@@ -86,12 +91,17 @@
             
             # Send POST request to API endpoint with headers
             response = self.client.post(api_url, headers=self.headers)
             
             #! Raise an error if POST fails
             response.raise_for_status()
             
+            
+            # error handling
+            if json.loads(response.content).get('success') == False:
+                raise ValueError(json.loads(response.content).get('error'))
+            
             # Retrieve diary data from JSON response
             data = json.loads(response.content)['data']
             output.append(data)
 
         return output
```

### Comparing `BlaApi-1.2/BlaApi/diary.py` & `BlaApi-1.3/BlaApi/diary.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,17 +33,16 @@
         if not passthru:
             for d in diary:
                 if d['studentId'] == student_id:  
                     output.append(d['id'])
         if output:
             return output
         else:
-            print("EXCEPTION: No entries for provided student id.")
-            return None
-
+            raise LookupError('No entries for provided student id.')
+        
     def get_current_date(self):
         
         # Retreive current date in a format that the api requires. 
         #! EXAMPLE: "Tue, 9/11/2001"
 
         # Get current date and day of week
         current_date = datetime.datetime.today()
@@ -83,16 +82,15 @@
         if not passthru:
             for d in diary:
                 if d['date'] == date:
                     output.append(d['id'])
         if output:
             return output
         else:
-            print("EXCEPTION: No matching entries for the specified date.")
-            return None
+            raise LookupError('No matching entries for the specified date.')
 
 
     def search_been_read(self, been_read=True, passthru=None):
 
         diary = self.client.get_diary_list()
 
         # parse output from diary list function
@@ -116,9 +114,8 @@
         else:
             for d in diary:
                 if d['bRead'] == been_read:
                     output.append(d['id'])
         if output:
             return output
         else:
-            print("EXCEPTION: No unread/read diaries found.")
-            return None
+            raise LookupError('No unread/read diaries found.')
```

### Comparing `BlaApi-1.2/BlaApi.egg-info/PKG-INFO` & `BlaApi-1.3/BlaApi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlaApi
-Version: 1.2
+Version: 1.3
 Summary: A wrapper for the beacon light api.
 Home-page: https://github.com/me/myproject
 Author: Omer-Farooqui
 Author-email: deaddogfuneral@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -17,22 +17,33 @@
 License-File: LICENSE
 
 
 # BLA-API-Wrapper.
 
 ## Description
 
-##### A light weight python library to interact with my school's homework app.
+##### A light weight python library to interact with [Beacon Light Academy's Homework App.](https://beaconlightacademy.edu.pk/app/)
 
 ### Table of Contents
 
+- [Installation](#Installation)
+
+
+
 - [Quick-Start](#Quick-Start)
 
+
+
 - [Documentation](#Documentation)
 
+
+
+- [Examples](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/tree/master/examples)
+
+
 - Useful Links:
   
   - [PyPI](https://pypi.org/project/BlaApi/)
   
   - [Github Repo](https://github.com/Omer-Farooqui/BLA-Api-Wrapper)
 
 ## Installation
@@ -149,8 +160,12 @@
   - [ ] Attachments
 
 - [ ] Make better doccumentation
 
 ### My motivation to create this
 
 Simply put, I found my school's app to be subpar, so I'm attempting to create a better one. *(It's also an excuse to learn new skills)*
-Feel free to open an issue if you have any questions, and star my [repo](https://github.com/Omer-Farooqui/BLA-Api-Wrapper) if you want 👉👈.
+
+
+
+
+Feel free to open an [issue](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/issues) if you want to send hate comments, and star my [repo](https://github.com/Omer-Farooqui/BLA-Api-Wrapper) if you don't 👉👈.
```

### Comparing `BlaApi-1.2/LICENSE` & `BlaApi-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `BlaApi-1.2/PKG-INFO` & `BlaApi-1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlaApi
-Version: 1.2
+Version: 1.3
 Summary: A wrapper for the beacon light api.
 Home-page: https://github.com/me/myproject
 Author: Omer-Farooqui
 Author-email: deaddogfuneral@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -17,22 +17,33 @@
 License-File: LICENSE
 
 
 # BLA-API-Wrapper.
 
 ## Description
 
-##### A light weight python library to interact with my school's homework app.
+##### A light weight python library to interact with [Beacon Light Academy's Homework App.](https://beaconlightacademy.edu.pk/app/)
 
 ### Table of Contents
 
+- [Installation](#Installation)
+
+
+
 - [Quick-Start](#Quick-Start)
 
+
+
 - [Documentation](#Documentation)
 
+
+
+- [Examples](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/tree/master/examples)
+
+
 - Useful Links:
   
   - [PyPI](https://pypi.org/project/BlaApi/)
   
   - [Github Repo](https://github.com/Omer-Farooqui/BLA-Api-Wrapper)
 
 ## Installation
@@ -149,8 +160,12 @@
   - [ ] Attachments
 
 - [ ] Make better doccumentation
 
 ### My motivation to create this
 
 Simply put, I found my school's app to be subpar, so I'm attempting to create a better one. *(It's also an excuse to learn new skills)*
-Feel free to open an issue if you have any questions, and star my [repo](https://github.com/Omer-Farooqui/BLA-Api-Wrapper) if you want 👉👈.
+
+
+
+
+Feel free to open an [issue](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/issues) if you want to send hate comments, and star my [repo](https://github.com/Omer-Farooqui/BLA-Api-Wrapper) if you don't 👉👈.
```

### Comparing `BlaApi-1.2/README.md` & `BlaApi-1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 # BLA-API-Wrapper.
 
 ## Description
 
-##### A light weight python library to interact with my school's homework app.
+##### A light weight python library to interact with [Beacon Light Academy's Homework App.](https://beaconlightacademy.edu.pk/app/)
 
 ### Table of Contents
 
+- [Installation](#Installation)
+
+
+
 - [Quick-Start](#Quick-Start)
 
+
+
 - [Documentation](#Documentation)
 
+
+
+- [Examples](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/tree/master/examples)
+
+
 - Useful Links:
   
   - [PyPI](https://pypi.org/project/BlaApi/)
   
   - [Github Repo](https://github.com/Omer-Farooqui/BLA-Api-Wrapper)
 
 ## Installation
@@ -130,8 +141,12 @@
   - [ ] Attachments
 
 - [ ] Make better doccumentation
 
 ### My motivation to create this
 
 Simply put, I found my school's app to be subpar, so I'm attempting to create a better one. *(It's also an excuse to learn new skills)*
-Feel free to open an issue if you have any questions, and star my [repo](https://github.com/Omer-Farooqui/BLA-Api-Wrapper) if you want 👉👈.
+
+
+
+
+Feel free to open an [issue](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/issues) if you want to send hate comments, and star my [repo](https://github.com/Omer-Farooqui/BLA-Api-Wrapper) if you don't 👉👈.
```

### Comparing `BlaApi-1.2/setup.py` & `BlaApi-1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Package meta-data.
 NAME = 'BlaApi'
 DESCRIPTION = 'A wrapper for the beacon light api.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'deaddogfuneral@gmail.com'
 AUTHOR = 'Omer-Farooqui'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '1.2'
+VERSION = '1.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
      'httpx', 'fake_useragent',
 ]
 
 # What packages are optional?
@@ -73,15 +73,15 @@
         except OSError:
             pass
 
         self.status('Building Source and Wheel (universal) distribution…')
         os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
 
         self.status('Uploading the package to PyPI via Twine…')
-        os.system('twine upload dist/*')
+        os.system('py -m twine upload dist/*')
 
         self.status('Pushing git tags…')
         os.system('git tag v{0}'.format(about['__version__']))
         os.system('git push --tags')
 
         sys.exit()
```

