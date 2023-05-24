# Comparing `tmp/unitlab-1.8.5.tar.gz` & `tmp/unitlab-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitlab-1.8.5.tar", last modified: Tue May 23 13:15:54 2023, max compression
+gzip compressed data, was "unitlab-1.8.6.tar", last modified: Tue May 23 13:44:13 2023, max compression
```

## Comparing `unitlab-1.8.5.tar` & `unitlab-1.8.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-23 13:15:54.121113 unitlab-1.8.5/
--rw-rw-r--   0 me        (1000) me        (1000)     1060 2022-11-07 13:04:44.000000 unitlab-1.8.5/LICENSE.md
--rw-rw-r--   0 me        (1000) me        (1000)       84 2023-02-15 09:26:00.000000 unitlab-1.8.5/MANIFEST.in
--rw-rw-r--   0 me        (1000) me        (1000)      654 2023-05-23 13:15:54.121113 unitlab-1.8.5/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)     1439 2023-05-23 07:41:41.000000 unitlab-1.8.5/README.md
--rw-rw-r--   0 me        (1000) me        (1000)      106 2023-05-23 13:15:54.125113 unitlab-1.8.5/setup.cfg
--rw-rw-r--   0 me        (1000) me        (1000)     1108 2023-05-23 13:04:53.000000 unitlab-1.8.5/setup.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-23 13:15:54.121113 unitlab-1.8.5/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-23 13:15:54.121113 unitlab-1.8.5/src/unitlab/
--rw-rw-r--   0 me        (1000) me        (1000)      214 2023-05-23 13:05:07.000000 unitlab-1.8.5/src/unitlab/__init__.py
--rw-rw-r--   0 me        (1000) me        (1000)     2084 2023-05-23 11:11:24.000000 unitlab-1.8.5/src/unitlab/cli.py
--rw-rw-r--   0 me        (1000) me        (1000)    10963 2023-05-23 13:05:44.000000 unitlab-1.8.5/src/unitlab/client.py
--rw-rw-r--   0 me        (1000) me        (1000)      656 2023-05-23 07:35:04.000000 unitlab-1.8.5/src/unitlab/exceptions.py
--rw-rw-r--   0 me        (1000) me        (1000)     1785 2023-05-23 13:06:10.000000 unitlab-1.8.5/src/unitlab/run.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-23 13:15:54.121113 unitlab-1.8.5/src/unitlab.egg-info/
--rw-rw-r--   0 me        (1000) me        (1000)      654 2023-05-23 13:15:54.000000 unitlab-1.8.5/src/unitlab.egg-info/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)      373 2023-05-23 13:15:54.000000 unitlab-1.8.5/src/unitlab.egg-info/SOURCES.txt
--rw-rw-r--   0 me        (1000) me        (1000)        1 2023-05-23 13:15:54.000000 unitlab-1.8.5/src/unitlab.egg-info/dependency_links.txt
--rw-rw-r--   0 me        (1000) me        (1000)       44 2023-05-23 13:15:54.000000 unitlab-1.8.5/src/unitlab.egg-info/entry_points.txt
--rw-rw-r--   0 me        (1000) me        (1000)       55 2023-05-23 13:15:54.000000 unitlab-1.8.5/src/unitlab.egg-info/requires.txt
--rw-rw-r--   0 me        (1000) me        (1000)        8 2023-05-23 13:15:54.000000 unitlab-1.8.5/src/unitlab.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-23 13:44:13.497238 unitlab-1.8.6/
+-rw-rw-r--   0 me        (1000) me        (1000)     1060 2022-11-07 13:04:44.000000 unitlab-1.8.6/LICENSE.md
+-rw-rw-r--   0 me        (1000) me        (1000)       84 2023-02-15 09:26:00.000000 unitlab-1.8.6/MANIFEST.in
+-rw-rw-r--   0 me        (1000) me        (1000)      654 2023-05-23 13:44:13.497238 unitlab-1.8.6/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)     1439 2023-05-23 07:41:41.000000 unitlab-1.8.6/README.md
+-rw-rw-r--   0 me        (1000) me        (1000)      106 2023-05-23 13:44:13.497238 unitlab-1.8.6/setup.cfg
+-rw-rw-r--   0 me        (1000) me        (1000)     1108 2023-05-23 13:43:53.000000 unitlab-1.8.6/setup.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-23 13:44:13.497238 unitlab-1.8.6/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-23 13:44:13.497238 unitlab-1.8.6/src/unitlab/
+-rw-rw-r--   0 me        (1000) me        (1000)      214 2023-05-23 13:05:07.000000 unitlab-1.8.6/src/unitlab/__init__.py
+-rw-rw-r--   0 me        (1000) me        (1000)     2084 2023-05-23 11:11:24.000000 unitlab-1.8.6/src/unitlab/cli.py
+-rw-rw-r--   0 me        (1000) me        (1000)    11483 2023-05-23 13:43:21.000000 unitlab-1.8.6/src/unitlab/client.py
+-rw-rw-r--   0 me        (1000) me        (1000)      656 2023-05-23 07:35:04.000000 unitlab-1.8.6/src/unitlab/exceptions.py
+-rw-rw-r--   0 me        (1000) me        (1000)     1785 2023-05-23 13:06:10.000000 unitlab-1.8.6/src/unitlab/run.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-23 13:44:13.497238 unitlab-1.8.6/src/unitlab.egg-info/
+-rw-rw-r--   0 me        (1000) me        (1000)      654 2023-05-23 13:44:13.000000 unitlab-1.8.6/src/unitlab.egg-info/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)      373 2023-05-23 13:44:13.000000 unitlab-1.8.6/src/unitlab.egg-info/SOURCES.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        1 2023-05-23 13:44:13.000000 unitlab-1.8.6/src/unitlab.egg-info/dependency_links.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       44 2023-05-23 13:44:13.000000 unitlab-1.8.6/src/unitlab.egg-info/entry_points.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       55 2023-05-23 13:44:13.000000 unitlab-1.8.6/src/unitlab.egg-info/requires.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        8 2023-05-23 13:44:13.000000 unitlab-1.8.6/src/unitlab.egg-info/top_level.txt
```

### Comparing `unitlab-1.8.5/LICENSE.md` & `unitlab-1.8.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.5/PKG-INFO` & `unitlab-1.8.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 1.8.5
+Version: 1.8.6
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `unitlab-1.8.5/README.md` & `unitlab-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.5/setup.py` & `unitlab-1.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="unitlab",
-    version="1.8.5",
+    version="1.8.6",
     license="MIT",
     author="Unitlab Inc.",
     author_email="team@unitlab.ai",
     packages=find_packages("src"),
     include_package_data=True,
     package_data={"static": ["*"], "Potato": ["*.so"]},
     classifiers=[
```

### Comparing `unitlab-1.8.5/src/unitlab/cli.py` & `unitlab-1.8.6/src/unitlab/cli.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.5/src/unitlab/client.py` & `unitlab-1.8.6/src/unitlab/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import aiohttp
 import requests
 import tqdm
 
 from .exceptions import AuthenticationError
 
-BASE_URL = "https://api.unitlab.ai/api/cli/"
+BASE_URL = os.environ.get("UNITLAB_BASE_URL", "https://api.unitlab.ai")
 SDK_URL = BASE_URL + "/api/sdk/"
 
 
 SDK_ENPOINTS = {
     "ai_models": SDK_URL + "ai-models/",
     "ai_model": SDK_URL + "ai-model/{}/",
     "tasks": SDK_URL + "tasks/",
@@ -198,14 +198,15 @@
             with open(image, "rb") as img:
                 try:
                     response = await session.request(
                         "POST",
                         url=SDK_ENPOINTS["upload_data"],
                         data=aiohttp.FormData(fields={"task": task_id, "image": img}),
                     )
+                    response.raise_for_status()
                     return 1 if response.status == 201 else 0
                 except Exception as e:
                     logging.error(f"Error uploading image {image} - {e}")
                     return 0
 
         async def batch_upload(
             session: aiohttp.ClientSession, batch: list, task_id: str, pbar: tqdm.tqdm
@@ -217,30 +218,40 @@
                 pbar.update(await f)
 
         async def main():
             images = [
                 image
                 for images_list in (
                     glob.glob(os.path.join(directory, "") + extension)
-                    for extension in ["*jpg", "*png"]
+                    for extension in ["*jpg", "*png", "*jpeg", "*webp"]
                 )
                 for image in images_list
             ]
-            num_images = len(images)
+            filtered_images = []
+            for image in images:
+                file_size = os.path.getsize(image) / 1024 / 1024
+                if file_size > 6:
+                    logging.warning(
+                        f"Image {image} is too large ({file_size:.4f} megabytes) skipping, max size is 6 MB"
+                    )
+                    continue
+                filtered_images.append(image)
+
+            num_images = len(filtered_images)
             num_batches = (num_images + batch_size - 1) // batch_size
 
             logging.info(f"Uploading {num_images} images to task {task_id}")
             with tqdm.tqdm(total=num_images, ncols=80) as pbar:
                 async with aiohttp.ClientSession(
                     headers=self._get_headers()
                 ) as session:
                     for i in range(num_batches):
                         await batch_upload(
                             session,
-                            images[
+                            filtered_images[
                                 i * batch_size : min((i + 1) * batch_size, num_images)
                             ],
                             task_id,
                             pbar,
                         )
 
         asyncio.run(main())
```

### Comparing `unitlab-1.8.5/src/unitlab/exceptions.py` & `unitlab-1.8.6/src/unitlab/exceptions.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.5/src/unitlab/run.py` & `unitlab-1.8.6/src/unitlab/run.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.5/src/unitlab.egg-info/PKG-INFO` & `unitlab-1.8.6/src/unitlab.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 1.8.5
+Version: 1.8.6
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

