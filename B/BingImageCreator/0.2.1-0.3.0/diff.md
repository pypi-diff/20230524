# Comparing `tmp/BingImageCreator-0.2.1.tar.gz` & `tmp/BingImageCreator-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BingImageCreator-0.2.1.tar", last modified: Sun May 21 10:53:55 2023, max compression
+gzip compressed data, was "BingImageCreator-0.3.0.tar", last modified: Wed May 24 10:02:53 2023, max compression
```

## Comparing `BingImageCreator-0.2.1.tar` & `BingImageCreator-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:53:55.302250 BingImageCreator-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-21 10:53:33.000000 BingImageCreator-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-21 10:53:55.302250 BingImageCreator-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-21 10:53:33.000000 BingImageCreator-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 10:53:55.302250 BingImageCreator-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-21 10:53:33.000000 BingImageCreator-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:53:55.302250 BingImageCreator-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:53:55.302250 BingImageCreator-0.2.1/src/BingImageCreator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-21 10:53:55.000000 BingImageCreator-0.2.1/src/BingImageCreator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-21 10:53:55.000000 BingImageCreator-0.2.1/src/BingImageCreator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 10:53:55.000000 BingImageCreator-0.2.1/src/BingImageCreator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-21 10:53:55.000000 BingImageCreator-0.2.1/src/BingImageCreator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-21 10:53:55.000000 BingImageCreator-0.2.1/src/BingImageCreator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14630 2023-05-21 10:53:33.000000 BingImageCreator-0.2.1/src/BingImageCreator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:53:55.302250 BingImageCreator-0.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-21 10:53:33.000000 BingImageCreator-0.2.1/test/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:02:53.969367 BingImageCreator-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-24 10:02:24.000000 BingImageCreator-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-24 10:02:53.969367 BingImageCreator-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-24 10:02:24.000000 BingImageCreator-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-24 10:02:53.969367 BingImageCreator-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-24 10:02:24.000000 BingImageCreator-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:02:53.965367 BingImageCreator-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:02:53.965367 BingImageCreator-0.3.0/src/BingImageCreator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-24 10:02:53.000000 BingImageCreator-0.3.0/src/BingImageCreator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-24 10:02:53.000000 BingImageCreator-0.3.0/src/BingImageCreator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 10:02:53.000000 BingImageCreator-0.3.0/src/BingImageCreator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 10:02:53.000000 BingImageCreator-0.3.0/src/BingImageCreator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-24 10:02:53.000000 BingImageCreator-0.3.0/src/BingImageCreator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-05-24 10:02:24.000000 BingImageCreator-0.3.0/src/BingImageCreator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:02:53.965367 BingImageCreator-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-24 10:02:24.000000 BingImageCreator-0.3.0/test/test_example.py
```

### Comparing `BingImageCreator-0.2.1/LICENSE` & `BingImageCreator-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.2.1/PKG-INFO` & `BingImageCreator-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.2.1
+Version: 0.3.0
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.2.1/README.md` & `BingImageCreator-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.2.1/setup.py` & `BingImageCreator-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="BingImageCreator",
-    version="0.2.1",
+    version="0.3.0",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="High quality image generation by Microsoft. Reverse engineered API.",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/BingImageCreator",
```

### Comparing `BingImageCreator-0.2.1/src/BingImageCreator.egg-info/PKG-INFO` & `BingImageCreator-0.3.0/src/BingImageCreator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.2.1
+Version: 0.3.0
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.2.1/src/BingImageCreator.py` & `BingImageCreator-0.3.0/src/BingImageCreator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import argparse
 import asyncio
-from functools import partial
 import contextlib
 import json
 import os
 import random
 import sys
 import time
+from functools import partial
+from typing import Dict
+from typing import List
+from typing import Union
+
 import aiohttp
 import pkg_resources
 import regex
 import requests
-from typing import Union
 
 if os.environ.get("BING_URL") == None:
     BING_URL = "https://www.bing.com"
 else:
     BING_URL = os.environ.get("BING_URL")
 # Generate random IP between range 13.104.0.0/14
 FORWARDED_IP = (
@@ -62,15 +65,15 @@
     """
 
     def __init__(
         self,
         auth_cookie: str,
         debug_file: Union[str, None] = None,
         quiet: bool = False,
-        all_cookies: list[dict] = None,
+        all_cookies: List[Dict] = None,
     ) -> None:
         self.session: requests.Session = requests.Session()
         self.session.headers = HEADERS
         self.session.cookies.set("_U", auth_cookie)
         if all_cookies:
             for cookie in all_cookies:
                 self.session.cookies.set(cookie["name"], cookie["value"])
@@ -90,15 +93,18 @@
         if self.debug_file:
             self.debug(sending_message)
         url_encoded_prompt = requests.utils.quote(prompt)
         payload = f"q={url_encoded_prompt}&qs=ds"
         # https://www.bing.com/images/create?q=<PROMPT>&rt=3&FORM=GENCRE
         url = f"{BING_URL}/images/create?q={url_encoded_prompt}&rt=4&FORM=GENCRE"
         response = self.session.post(
-            url, allow_redirects=False, data=payload, timeout=200
+            url,
+            allow_redirects=False,
+            data=payload,
+            timeout=200,
         )
         # check for content waring message
         if "this prompt has been blocked" in response.text.lower():
             if self.debug_file:
                 self.debug(f"ERROR: {error_blocked_prompt}")
             raise Exception(
                 error_blocked_prompt,
@@ -180,22 +186,23 @@
         with contextlib.suppress(FileExistsError):
             os.mkdir(output_dir)
         try:
             fn = f"{file_name}_" if file_name else ""
             jpeg_index = 0
             for link in links:
                 while os.path.exists(
-                    os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg")
+                    os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg"),
                 ):
                     jpeg_index += 1
                 with self.session.get(link, stream=True) as response:
                     # save response to file
                     response.raise_for_status()
                     with open(
-                        os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg"), "wb"
+                        os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg"),
+                        "wb",
                     ) as output_file:
                         for chunk in response.iter_content(chunk_size=8192):
                             output_file.write(chunk)
         except requests.exceptions.MissingSchema as url_exception:
             raise Exception(
                 "Inappropriate contents found in the generated images. Please try again or try another prompt.",
             ) from url_exception
@@ -204,21 +211,39 @@
 class ImageGenAsync:
     """
     Image generation by Microsoft Bing
     Parameters:
         auth_cookie: str
     """
 
-    def __init__(self, auth_cookie: str, quiet: bool = False) -> None:
+    def __init__(
+        self,
+        auth_cookie: str = None,
+        debug_file: Union[str, None] = None,
+        quiet: bool = False,
+        all_cookies: List[Dict] = None,
+    ) -> None:
+        if auth_cookie is None and not all_cookies:
+            raise Exception("No auth cookie provided")
         self.session = aiohttp.ClientSession(
             headers=HEADERS,
             cookies={"_U": auth_cookie},
             trust_env=True,
         )
+        if all_cookies:
+            for cookie in all_cookies:
+                self.session.cookie_jar.update_cookies(
+                    {cookie["name"]: cookie["value"]},
+                )
+        if auth_cookie:
+            self.session.cookie_jar.update_cookies({"_U": auth_cookie})
         self.quiet = quiet
+        self.debug_file = debug_file
+        if self.debug_file:
+            self.debug = partial(debug, self.debug_file)
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, *excinfo) -> None:
         await self.session.close()
 
@@ -231,15 +256,17 @@
         if not self.quiet:
             print("Sending request...")
         url_encoded_prompt = requests.utils.quote(prompt)
         # https://www.bing.com/images/create?q=<PROMPT>&rt=3&FORM=GENCRE
         url = f"{BING_URL}/images/create?q={url_encoded_prompt}&rt=4&FORM=GENCRE"
         payload = f"q={url_encoded_prompt}&qs=ds"
         async with self.session.post(
-            url, allow_redirects=False, data=payload
+            url,
+            allow_redirects=False,
+            data=payload,
         ) as response:
             content = await response.text()
             if "this prompt has been blocked" in content.lower():
                 raise Exception(
                     "Your prompt has been blocked by Bing. Try to change any bad words and try again.",
                 )
             if response.status != 302:
@@ -294,44 +321,67 @@
             if im in bad_images:
                 raise Exception("Bad images")
         # No images
         if not normal_image_links:
             raise Exception("No images")
         return normal_image_links
 
-    async def save_images(self, links: list, output_dir: str) -> None:
+    async def save_images(
+        self,
+        links: list,
+        output_dir: str,
+        file_name: str = None,
+    ) -> None:
         """
         Saves images to output directory
         """
+        if self.debug_file:
+            self.debug(download_message)
         if not self.quiet:
-            print("\nDownloading images...")
+            print(download_message)
         with contextlib.suppress(FileExistsError):
             os.mkdir(output_dir)
         try:
+            fn = f"{file_name}_" if file_name else ""
             jpeg_index = 0
             for link in links:
-                while os.path.exists(os.path.join(output_dir, f"{jpeg_index}.jpeg")):
+                while os.path.exists(
+                    os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg"),
+                ):
                     jpeg_index += 1
                 async with self.session.get(link, raise_for_status=True) as response:
                     # save response to file
                     with open(
-                        os.path.join(output_dir, f"{jpeg_index}.jpeg"), "wb"
+                        os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg"),
+                        "wb",
                     ) as output_file:
                         async for chunk in response.content.iter_chunked(8192):
                             output_file.write(chunk)
         except aiohttp.client_exceptions.InvalidURL as url_exception:
             raise Exception(
                 "Inappropriate contents found in the generated images. Please try again or try another prompt.",
             ) from url_exception
 
 
-async def async_image_gen(args) -> None:
-    async with ImageGenAsync(args.U, args.quiet) as image_generator:
-        images = await image_generator.get_images(args.prompt)
-        await image_generator.save_images(images, output_dir=args.output_dir)
+async def async_image_gen(
+    prompt: str,
+    output_dir: str,
+    u_cookie=None,
+    debug_file=None,
+    quiet=False,
+    all_cookies=None,
+):
+    async with ImageGenAsync(
+        u_cookie,
+        debug_file=debug_file,
+        quiet=quiet,
+        all_cookies=all_cookies,
+    ) as image_generator:
+        images = await image_generator.get_images(prompt)
+        await image_generator.save_images(images, output_dir=output_dir)
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("-U", help="Auth cookie from browser", type=str)
     parser.add_argument("--cookie-file", help="File containing auth cookie", type=str)
     parser.add_argument(
@@ -385,19 +435,31 @@
 
     if args.U is None and args.cookie_file is None:
         raise Exception("Could not find auth cookie")
 
     if not args.asyncio:
         # Create image generator
         image_generator = ImageGen(
-            args.U, args.debug_file, args.quiet, all_cookies=cookie_json
+            args.U,
+            args.debug_file,
+            args.quiet,
+            all_cookies=cookie_json,
         )
         image_generator.save_images(
             image_generator.get_images(args.prompt),
             output_dir=args.output_dir,
         )
     else:
-        asyncio.run(async_image_gen(args))
+        asyncio.run(
+            async_image_gen(
+                args.prompt,
+                args.output_dir,
+                args.U,
+                args.debug_file,
+                args.quiet,
+                all_cookies=cookie_json,
+            ),
+        )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `BingImageCreator-0.2.1/test/test_example.py` & `BingImageCreator-0.3.0/test/test_example.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-import os,shutil
+import os
+import shutil
+
 from src.BingImageCreator import ImageGen
+
+
 def test_save_images():
     # create a temporary output directory for testing purposes
     test_output_dir = "test_output"
     os.mkdir(test_output_dir)
     # download a test image
     test_image_url = "https://picsum.photos/200"
-    gen = ImageGen(auth_cookie='')
-    gen.save_images([test_image_url], test_output_dir, )
+    gen = ImageGen(auth_cookie="")
+    gen.save_images([test_image_url], test_output_dir)
     gen.save_images([test_image_url], test_output_dir, file_name="test_image")
     # check if the image was downloaded and saved correctly
     assert os.path.exists(os.path.join(test_output_dir, "test_image_0.jpeg"))
     assert os.path.exists(os.path.join(test_output_dir, "0.jpeg"))
     # remove the temporary output directory
     shutil.rmtree(test_output_dir)
```

