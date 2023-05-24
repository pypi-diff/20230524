# Comparing `tmp/bose-1.5.3.tar.gz` & `tmp/bose-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bose-1.5.3.tar", last modified: Wed May 24 16:21:10 2023, max compression
+gzip compressed data, was "bose-1.5.4.tar", last modified: Wed May 24 16:31:14 2023, max compression
```

## Comparing `bose-1.5.3.tar` & `bose-1.5.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 16:21:10.757282 bose-1.5.3/
--rw-rw-rw-   0        0        0     1346 2023-05-24 16:21:10.757282 bose-1.5.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-24 16:21:10.756284 bose-1.5.3/bose/
--rw-rw-rw-   0        0        0      340 2023-05-13 11:28:45.126433 bose-1.5.3/bose/__init__.py
--rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-1.5.3/bose/base_data.py
--rw-rw-rw-   0        0        0     4990 2023-05-18 07:22:46.924306 bose-1.5.3/bose/base_task.py
--rw-rw-rw-   0        0        0     9039 2023-05-22 11:25:15.734584 bose-1.5.3/bose/boss_driver.py
--rw-rw-rw-   0        0        0     9051 2023-05-22 11:25:15.732590 bose-1.5.3/bose/boss_undetected_driver.py
--rw-rw-rw-   0        0        0     7295 2023-05-13 11:28:17.686088 bose-1.5.3/bose/create_driver.py
--rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-1.5.3/bose/download_driver.py
--rw-rw-rw-   0        0        0     3185 2023-05-18 07:50:25.651854 bose-1.5.3/bose/local_storage.py
--rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-1.5.3/bose/local_storage_driver.py
--rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-1.5.3/bose/opponent.py
--rw-rw-rw-   0        0        0     3187 2023-05-15 09:11:34.318135 bose-1.5.3/bose/output.py
--rw-rw-rw-   0        0        0     1650 2023-05-13 11:28:17.687091 bose-1.5.3/bose/task_info.py
--rw-rw-rw-   0        0        0     3977 2023-05-13 13:31:08.141431 bose-1.5.3/bose/temp_mail.py
--rw-rw-rw-   0        0        0     7361 2023-05-10 09:24:37.900794 bose-1.5.3/bose/user_agent.py
--rw-rw-rw-   0        0        0     6050 2023-05-10 10:34:20.625623 bose-1.5.3/bose/utils.py
--rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-1.5.3/bose/wait.py
--rw-rw-rw-   0        0        0     1203 2023-05-09 07:09:28.075948 bose-1.5.3/bose/window_size.py
--rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0     2452 2023-05-24 16:20:28.885271 bose-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 16:31:14.621986 bose-1.5.4/
+-rw-rw-rw-   0        0        0    15140 2023-05-24 16:31:14.623981 bose-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11113 2023-05-24 16:30:55.456359 bose-1.5.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-24 16:31:14.621986 bose-1.5.4/bose/
+-rw-rw-rw-   0        0        0      340 2023-05-13 11:28:45.126433 bose-1.5.4/bose/__init__.py
+-rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-1.5.4/bose/base_data.py
+-rw-rw-rw-   0        0        0     4990 2023-05-18 07:22:46.924306 bose-1.5.4/bose/base_task.py
+-rw-rw-rw-   0        0        0     9039 2023-05-22 11:25:15.734584 bose-1.5.4/bose/boss_driver.py
+-rw-rw-rw-   0        0        0     9051 2023-05-22 11:25:15.732590 bose-1.5.4/bose/boss_undetected_driver.py
+-rw-rw-rw-   0        0        0     7295 2023-05-13 11:28:17.686088 bose-1.5.4/bose/create_driver.py
+-rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-1.5.4/bose/download_driver.py
+-rw-rw-rw-   0        0        0     3185 2023-05-18 07:50:25.651854 bose-1.5.4/bose/local_storage.py
+-rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-1.5.4/bose/local_storage_driver.py
+-rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-1.5.4/bose/opponent.py
+-rw-rw-rw-   0        0        0     3187 2023-05-15 09:11:34.318135 bose-1.5.4/bose/output.py
+-rw-rw-rw-   0        0        0     1650 2023-05-13 11:28:17.687091 bose-1.5.4/bose/task_info.py
+-rw-rw-rw-   0        0        0     3977 2023-05-13 13:31:08.141431 bose-1.5.4/bose/temp_mail.py
+-rw-rw-rw-   0        0        0     7361 2023-05-10 09:24:37.900794 bose-1.5.4/bose/user_agent.py
+-rw-rw-rw-   0        0        0     6050 2023-05-10 10:34:20.625623 bose-1.5.4/bose/utils.py
+-rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-1.5.4/bose/wait.py
+-rw-rw-rw-   0        0        0     1203 2023-05-09 07:09:28.075948 bose-1.5.4/bose/window_size.py
+-rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     2524 2023-05-24 16:24:59.957564 bose-1.5.4/setup.py
```

### Comparing `bose-1.5.3/bose/base_data.py` & `bose-1.5.4/bose/base_data.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.3/bose/base_task.py` & `bose-1.5.4/bose/base_task.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.3/bose/boss_driver.py` & `bose-1.5.4/bose/boss_driver.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.3/bose/boss_undetected_driver.py` & `bose-1.5.4/bose/boss_undetected_driver.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.3/bose/create_driver.py` & `bose-1.5.4/bose/create_driver.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.3/bose/download_driver.py` & `bose-1.5.4/bose/download_driver.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.3/bose/local_storage.py` & `bose-1.5.4/bose/local_storage.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.3/bose/local_storage_driver.py` & `bose-1.5.4/bose/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.3/bose/output.py` & `bose-1.5.4/bose/output.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.3/bose/task_info.py` & `bose-1.5.4/bose/task_info.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.3/bose/temp_mail.py` & `bose-1.5.4/bose/temp_mail.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.3/bose/user_agent.py` & `bose-1.5.4/bose/user_agent.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.3/bose/utils.py` & `bose-1.5.4/bose/utils.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.3/bose/window_size.py` & `bose-1.5.4/bose/window_size.py`

 * *Files identical despite different names*

### Comparing `bose-1.5.3/setup.py` & `bose-1.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,27 +13,29 @@
 extras_require = {}
 cpython_dependencies = [
     "PyDispatcher>=2.0.5",
 ]
 
 def get_description():
     try:
-      import pypandoc
-      long_description = pypandoc.convert_file('README.md', 'rst')
-      return long_description
+    #   import pypandoc
+    #   long_description = pypandoc.convert_file('README.md', 'rst')
+    #   print(long_description)
+    #   return long_description
 
-      return open("README.md", encoding="utf-8").read()
-    except:
+      return open("README.rst", encoding="utf-8").read()
+    except Exception as e:
+    #   raise e
       return None
     
 
 setup(
     name='bose',
     packages=['bose'],
-    version='1.5.3',
+    version='1.5.4',
     license='MIT',
     project_urls={
         "Documentation": "https://omkar.cloud/bose/docs/",
         "Source": "https://github.com/omkarcloud/boss",
         "Tracker": "https://github.com/omkarcloud/boss/issues",
     },
```

