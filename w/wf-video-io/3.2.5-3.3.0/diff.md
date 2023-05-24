# Comparing `tmp/wf_video_io-3.2.5.tar.gz` & `tmp/wf_video_io-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf_video_io-3.2.5.tar", max compression
+gzip compressed data, was "wf_video_io-3.3.0.tar", max compression
```

## Comparing `wf_video_io-3.2.5.tar` & `wf_video_io-3.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0     1088 2022-07-13 02:25:51.284383 wf_video_io-3.2.5/LICENSE
--rwxr-xr-x   0        0        0      278 2023-01-27 16:56:30.309581 wf_video_io-3.2.5/README.md
--rw-r--r--   0        0        0     1162 2023-05-23 17:28:06.039351 wf_video_io-3.2.5/pyproject.toml
--rwxr-xr-x   0        0        0       28 2022-07-13 02:25:51.323025 wf_video_io-3.2.5/video_io/__init__.py
--rw-r--r--   0        0        0       37 2022-10-13 19:42:09.408938 wf_video_io-3.2.5/video_io/client/__init__.py
--rwxr-xr-x   0        0        0    15027 2023-05-23 16:51:13.034649 wf_video_io-3.2.5/video_io/client/core.py
--rw-r--r--   0        0        0      265 2023-05-15 17:34:04.808749 wf_video_io-3.2.5/video_io/client/errors.py
--rw-r--r--   0        0        0     3415 2023-05-23 17:27:25.989322 wf_video_io-3.2.5/video_io/client/utils.py
--rw-r--r--   0        0        0     1742 2023-05-15 17:34:04.821553 wf_video_io-3.2.5/video_io/config.py
--rwxr-xr-x   0        0        0    47659 2023-05-15 17:34:04.959430 wf_video_io-3.2.5/video_io/core.py
--rw-r--r--   0        0        0      382 2023-05-15 17:34:04.811182 wf_video_io-3.2.5/video_io/log_retry.py
--rw-r--r--   0        0        0    10067 2023-05-15 17:34:04.860739 wf_video_io-3.2.5/video_io/utils.py
--rw-r--r--   0        0        0      585 2023-01-27 16:56:30.326420 wf_video_io-3.2.5/video_io/video_reader.py
--rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 wf_video_io-3.2.5/setup.py
--rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 wf_video_io-3.2.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1088 2022-07-13 02:25:51.284383 wf_video_io-3.3.0/LICENSE
+-rwxr-xr-x   0        0        0      278 2023-01-27 16:56:30.309581 wf_video_io-3.3.0/README.md
+-rw-r--r--   0        0        0     1162 2023-05-24 18:48:33.803582 wf_video_io-3.3.0/pyproject.toml
+-rwxr-xr-x   0        0        0       28 2022-07-13 02:25:51.323025 wf_video_io-3.3.0/video_io/__init__.py
+-rw-r--r--   0        0        0       37 2022-10-13 19:42:09.408938 wf_video_io-3.3.0/video_io/client/__init__.py
+-rwxr-xr-x   0        0        0    15566 2023-05-24 18:27:45.399757 wf_video_io-3.3.0/video_io/client/core.py
+-rw-r--r--   0        0        0      265 2023-05-15 17:34:04.808749 wf_video_io-3.3.0/video_io/client/errors.py
+-rw-r--r--   0        0        0     3385 2023-05-24 18:36:26.987342 wf_video_io-3.3.0/video_io/client/utils.py
+-rw-r--r--   0        0        0     1742 2023-05-15 17:34:04.821553 wf_video_io-3.3.0/video_io/config.py
+-rwxr-xr-x   0        0        0    47659 2023-05-15 17:34:04.959430 wf_video_io-3.3.0/video_io/core.py
+-rw-r--r--   0        0        0      382 2023-05-15 17:34:04.811182 wf_video_io-3.3.0/video_io/log_retry.py
+-rw-r--r--   0        0        0    10067 2023-05-15 17:34:04.860739 wf_video_io-3.3.0/video_io/utils.py
+-rw-r--r--   0        0        0      585 2023-01-27 16:56:30.326420 wf_video_io-3.3.0/video_io/video_reader.py
+-rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 wf_video_io-3.3.0/setup.py
+-rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 wf_video_io-3.3.0/PKG-INFO
```

### Comparing `wf_video_io-3.2.5/LICENSE` & `wf_video_io-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.2.5/pyproject.toml` & `wf_video_io-3.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "wf-video-io"
 dynamic = ["version"]
 
 [tool.poetry]
 name = "wf-video-io"
-version = "3.2.5"
+version = "3.3.0"
 description = "Library for working with video files and interacting with the wildflower video-service"
 authors = ["Paul J DeCoursey <paul@decoursey.net>", "Theodore Quinn <ted.quinn@wildflowerschools.org>"]
 maintainers = ["Paul J DeCoursey <paul@decoursey.net>", "Theodore Quinn <ted.quinn@wildflowerschools.org>", "Benjamin Jaffe-Talberg <ben.talberg@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "video_io"}]
```

### Comparing `wf_video_io-3.2.5/video_io/client/core.py` & `wf_video_io-3.3.0/video_io/client/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,15 @@
         p = Path(destination) / path
         if not p.is_file() or overwrite:
             logger.info("Downloading video file %s", path)
             request = {
                 "method": "GET",
                 "url": f"{self.URL}/video/{path}/data",
                 "headers": self.headers,
+                "timeout": 45
             }
             try:
                 response = self.request_session.request(**request)
                 response.raise_for_status()
 
                 pp = p.parent
                 if not pp.exists():
@@ -217,28 +218,38 @@
                 environment_id,
                 start_date,
                 end_date,
                 e,
             )
             raise e
 
-    async def upload_video(self, path, local_cache_directory=None):
+    async def upload_video(self, path: str, local_cache_directory: str = None):
+        response = await self.upload_videos(path=[path], local_cache_directory=local_cache_directory)
+        return response[0]
+
+    async def upload_videos(self, paths: list[str], local_cache_directory: str = None):
         if local_cache_directory is None:
             local_cache_directory = self.CACHE_DIRECTORY
-        full_path = local_cache_directory / path
-        ptype, file_details = parse_path(path)
-        if ptype == "file":
-            file_details["ptype"] = ptype
-            file_details["path"] = full_path
-            file_details["filepath"] = path
-            resp = await self.upload_videos([file_details])
-            return resp[0]
-        return {
-            "error": "invalid path. doesn't match pattern [environment_id]/[camera_id]/[year]/[month]/[day]/[hour]/[min]-[second].mp4"
-        }
+
+        all_results: list[None, dict] = [None] * len(paths)
+        all_file_details: list[dict] = []
+        for ii, path in enumerate(paths):
+            full_path = local_cache_directory / path
+            ptype, file_details = parse_path(path)
+            if ptype == "file":
+                file_details["ptype"] = ptype
+                file_details["path"] = full_path
+                file_details["filepath"] = path
+                all_file_details.append(file_details)
+            else:
+                all_results[ii] = {
+                    "error": f"Invalid path. '{path}' doesn't match pattern [environment_id]/[camera_id]/[year]/[month]/[day]/[hour]/[min]-[second].mp4"
+                }
+
+        return await self._upload_videos(all_file_details)
 
     def prepare_video(self, file_details: Dict) -> (Dict, BytesIO):
         path = file_details["path"]
         video_properties = get_video_file_details(path)
         if file_details["ptype"] == "file":
             ts = f"{file_details['year']}-{file_details['month']}-{file_details['day']}T{file_details['hour']}:{file_details['file'][0:2]}:{file_details['file'][3:5]}.0000"
             meta = {
@@ -261,58 +272,61 @@
             with p.open("r", encoding="utf8") as fp:
                 meta = yaml.safe_load(fp.read())
         return (
             meta,
             open(path, "rb"),  # pylint: disable=R1732
         )
 
-    async def upload_videos(self, file_details: List[Dict]):
+    async def _upload_videos(self, file_details: List[Dict]):
         request = {
             "method": "POST",
             "url": f"{self.URL}/videos",
             "headers": self.headers,
         }
+
         files = []
         videos = []
         for details in file_details:
             meta, fileio = self.prepare_video(details)
             files.append(
                 (
                     "files",
                     fileio,
                 )
             )
             videos.append(meta)
+
         results = []
         request["files"] = files
         request["data"] = {"videos": json.dumps(videos)}
         try:
             request = requests.Request(**request)
             r = request.prepare()
             response = self.request_session.send(r)
             response.raise_for_status()
 
-            for i, vr in enumerate(response.json()):
+            for ii, vr in enumerate(response.json()):
                 results.append(
                     {
-                        "path": videos[i]["meta"]["path"],
+                        "path": videos[ii]["meta"]["path"],
                         "uploaded": True,
                         "id": vr["id"],
                         "disposition": "ok"
                         if "disposition" not in vr
                         else vr["disposition"],
                     }
                 )
             return results
         except JSONDecodeError as je:
             logger.error(
                 "Unusual response from video-service for %s: %s",
                 file_details,
-                response.text,
+                je.msg,
             )
+            raise je
         except requests.exceptions.HTTPError as e:
             logger.error(
                 "Failing uploading videos %s with HTTP error code %s",
                 file_details,
                 e.response.status_code,
             )
             raise e
@@ -395,15 +409,15 @@
             details["files_uploaded"] = 0
             details["details"] = []
             logger.debug("found %s files to be uploaded", len(files_found))
             with concurrent.futures.ThreadPoolExecutor(
                 max_workers=max_workers
             ) as executor:
                 results = executor.map(
-                    self.upload_videos, chunks(files_found, batch_size)
+                    self._upload_videos, chunks(files_found, batch_size)
                 )
                 logger.debug(results)
                 for result in await asyncio.gather(*results):
                     logger.debug(result)
                     for data in result:
                         if data["uploaded"]:
                             details["files_uploaded"] += 1
```

### Comparing `wf_video_io-3.2.5/video_io/client/utils.py` & `wf_video_io-3.3.0/video_io/client/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import json
 import re
-import subprocess
 
 import ffmpeg
 from tenacity import retry, wait_random, stop_after_attempt
 from auth0.v3.authentication import GetToken
 from cachetools.func import ttl_cache
 import jmespath
```

### Comparing `wf_video_io-3.2.5/video_io/config.py` & `wf_video_io-3.3.0/video_io/config.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.2.5/video_io/core.py` & `wf_video_io-3.3.0/video_io/core.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.2.5/video_io/utils.py` & `wf_video_io-3.3.0/video_io/utils.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.2.5/video_io/video_reader.py` & `wf_video_io-3.3.0/video_io/video_reader.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.2.5/setup.py` & `wf_video_io-3.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'wf-cv-utils>=3.4.0',
  'wf-fastapi-auth0>=1.0',
  'wf-gqlpycgen>=0.7.4,<0.8.0',
  'wf-honeycomb-io>=2.0.0']
 
 setup_kwargs = {
     'name': 'wf-video-io',
-    'version': '3.2.5',
+    'version': '3.3.0',
     'description': 'Library for working with video files and interacting with the wildflower video-service',
     'long_description': '# video_io\n\nTools for accessing Wildflower video data\n\n## Test\n\nTests are written with *behave* and *pytest*. As of 11/10/2022, *behave* tests are not functional.\n\n__Run pytest tests__\n\n```pytest```\n\n## Task list\n* ~~Add ability to request concatenation of videos~~ (11/7/2022)\n',
     'author': 'Paul J DeCoursey',
     'author_email': 'paul@decoursey.net',
     'maintainer': 'Paul J DeCoursey',
     'maintainer_email': 'paul@decoursey.net',
     'url': 'None',
```

### Comparing `wf_video_io-3.2.5/PKG-INFO` & `wf_video_io-3.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-video-io
-Version: 3.2.5
+Version: 3.3.0
 Summary: Library for working with video files and interacting with the wildflower video-service
 License: MIT
 Author: Paul J DeCoursey
 Author-email: paul@decoursey.net
 Maintainer: Paul J DeCoursey
 Maintainer-email: paul@decoursey.net
 Requires-Python: >=3.8,<3.12
```

