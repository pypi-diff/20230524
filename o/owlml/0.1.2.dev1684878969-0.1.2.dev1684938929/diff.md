# Comparing `tmp/owlml-0.1.2.dev1684878969.tar.gz` & `tmp/owlml-0.1.2.dev1684938929.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owlml-0.1.2.dev1684878969.tar", last modified: Tue May 23 21:56:20 2023, max compression
+gzip compressed data, was "owlml-0.1.2.dev1684938929.tar", last modified: Wed May 24 14:35:42 2023, max compression
```

## Comparing `owlml-0.1.2.dev1684878969.tar` & `owlml-0.1.2.dev1684938929.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:56:20.608841 owlml-0.1.2.dev1684878969/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-23 21:55:39.000000 owlml-0.1.2.dev1684878969/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-23 21:56:20.608841 owlml-0.1.2.dev1684878969/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-23 21:55:39.000000 owlml-0.1.2.dev1684878969/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:56:20.608841 owlml-0.1.2.dev1684878969/owlml/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-23 21:55:39.000000 owlml-0.1.2.dev1684878969/owlml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-23 21:55:39.000000 owlml-0.1.2.dev1684878969/owlml/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-23 21:55:39.000000 owlml-0.1.2.dev1684878969/owlml/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 21:55:39.000000 owlml-0.1.2.dev1684878969/owlml/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-23 21:55:39.000000 owlml-0.1.2.dev1684878969/owlml/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-23 21:55:39.000000 owlml-0.1.2.dev1684878969/owlml/images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:56:20.608841 owlml-0.1.2.dev1684878969/owlml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-23 21:56:20.000000 owlml-0.1.2.dev1684878969/owlml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-23 21:56:20.000000 owlml-0.1.2.dev1684878969/owlml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:56:20.000000 owlml-0.1.2.dev1684878969/owlml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 21:56:20.000000 owlml-0.1.2.dev1684878969/owlml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 21:56:20.000000 owlml-0.1.2.dev1684878969/owlml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 21:56:20.000000 owlml-0.1.2.dev1684878969/owlml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-23 21:56:20.608841 owlml-0.1.2.dev1684878969/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 21:55:39.000000 owlml-0.1.2.dev1684878969/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:35:42.125939 owlml-0.1.2.dev1684938929/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-24 14:35:42.125939 owlml-0.1.2.dev1684938929/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:35:42.125939 owlml-0.1.2.dev1684938929/owlml/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/owlml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/owlml/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/owlml/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/owlml/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/owlml/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/owlml/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/owlml/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/owlml/images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:35:42.125939 owlml-0.1.2.dev1684938929/owlml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-24 14:35:42.000000 owlml-0.1.2.dev1684938929/owlml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-24 14:35:42.000000 owlml-0.1.2.dev1684938929/owlml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:35:42.000000 owlml-0.1.2.dev1684938929/owlml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-24 14:35:42.000000 owlml-0.1.2.dev1684938929/owlml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-24 14:35:42.000000 owlml-0.1.2.dev1684938929/owlml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 14:35:42.000000 owlml-0.1.2.dev1684938929/owlml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-24 14:35:42.129940 owlml-0.1.2.dev1684938929/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 14:34:01.000000 owlml-0.1.2.dev1684938929/setup.py
```

### Comparing `owlml-0.1.2.dev1684878969/LICENSE` & `owlml-0.1.2.dev1684938929/LICENSE`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684878969/README.md` & `owlml-0.1.2.dev1684938929/README.md`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684878969/owlml/api.py` & `owlml-0.1.2.dev1684938929/owlml/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,26 +22,27 @@
             f"{error}\nResponse body: {response.text}"
         ) from error
 
 
 class OwlMLAPI:
     """API class for OwlML."""
 
-    base_url: str = os.path.join(_get_required_env_var("OWLML_URL"), "api")
+    base_url: str = _get_required_env_var("OWLML_URL")
+    api_url: str = os.path.join(base_url, "api")
 
     @classmethod
     def get(cls, route: str) -> dict[str, Any]:
         """Make a GET request to the OwlML API."""
-        response = requests.get(os.path.join(cls.base_url, route))
+        response = requests.get(os.path.join(cls.api_url, route))
         raise_for_status(response)
         if response.status_code == 204:
             return {}
         return response.json()
 
     @classmethod
     def post(cls, route: str, payload: dict[str, Any] = dict()) -> dict[str, Any]:
         """Make a POST request to the OwlML API."""
-        response = requests.post(os.path.join(cls.base_url, route), json=payload)
+        response = requests.post(os.path.join(cls.api_url, route), json=payload)
         raise_for_status(response)
         if response.status_code == 204:
             return {}
         return response.json()
```

### Comparing `owlml-0.1.2.dev1684878969/owlml/auth.py` & `owlml-0.1.2.dev1684938929/owlml/auth.py`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684878969/owlml/datasets.py` & `owlml-0.1.2.dev1684938929/owlml/images.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,89 @@
-"""OwlML datasets API."""
-import json
-import time
+"""OwlML images API."""
+import hashlib
+import os
 from pathlib import Path
 from typing import Any, Optional, Union
 
 import requests
+from PIL import Image
 from tqdm import tqdm
 
 from .api import OwlMLAPI, raise_for_status
 
 
 def _complete_batch(batch: str) -> dict[str, Any]:
     """Complete a batch."""
     return OwlMLAPI.post(f"batches/{batch}/complete")
 
 
+def _complete_image(image_id: str) -> dict[str, Any]:
+    """Complete an image."""
+    return OwlMLAPI.post(f"images/{image_id}/complete")
+
+
 def _create_batch(dataset: str, batch: Optional[str] = None) -> dict[str, Any]:
     """Create a batch."""
     payload = dict(dataset=dataset)
     if batch is not None:
         payload["slug"] = batch
     return OwlMLAPI.post("batches", payload)
 
 
-def create_dataset(org: str, slug: str, labels: list[str]) -> dict[str, Any]:
-    """Create a dataset."""
-    payload = dict(org=org, slug=slug, labels=labels)
-    return OwlMLAPI.post("datasets", payload)
-
-
-def download_dataset(
-    dataset: str,
-    version_slug: Optional[str] = None,
-    output_path: Union[str, Path] = "./",
+def _create_image(
+    dataset: str, batch: str, image_path: Union[str, Path]
 ) -> dict[str, Any]:
-    """Download dataset version."""
-    output_path = Path(output_path)
-    if version_slug is None:
-        version = version_dataset(dataset)
-        version_slug = version["slug"]
-    version = OwlMLAPI.get(f"dataset-versions/{version_slug}")
-    if len(version["images"]) == 0:
-        raise ValueError(f"No images in dataset version {version_slug}.")
-    image = next(iter(version["images"]))
-    image_path = output_path / Path(image["image_id"] + image["extension"])
-    dataset_path = image_path.parent.parent.parent
-    annotations_path = dataset_path / "annotations" / f"{version_slug}.json"
-    annotations_path.parent.mkdir(parents=True, exist_ok=True)
-    with open(annotations_path, "w") as f:
-        f.write(json.dumps(version["annotations"]))
-    for image in tqdm(version["images"]):
-        image_path = output_path / Path(image["image_id"] + image["extension"])
-        image_path.parent.mkdir(parents=True, exist_ok=True)
-        response = requests.get(image["presigned_get"])
-        raise_for_status(response)
-        with open(image_path, "wb") as f:
-            f.write(response.content)
+    image = Image.open(image_path)
+    width, height = image.size
+    with open(image_path, "rb") as f:
+        checksum = hashlib.md5(f.read()).hexdigest()
+    payload = dict(
+        dataset=dataset,
+        batch=batch,
+        filename=image_path.name,
+        checksum=checksum,
+        width=width,
+        height=height,
+    )
+    return OwlMLAPI.post("images", payload)
+
+
+def _download_image(presigned_get: str, image_path: Union[str, Path]) -> None:
+    """Download an image."""
+    response = requests.get(presigned_get)
+    raise_for_status(response)
+    with open(image_path, "wb") as f:
+        f.write(response.content)
+
+
+def _upload_image(presigned_post: dict[str, Any], image_path: Union[str, Path]) -> None:
+    """Upload an image."""
+    files = {"file": open(image_path, "rb")}
+    response = requests.post(
+        presigned_post["url"], data=presigned_post["fields"], files=files
+    )
+    raise_for_status(response)
+
+
+def generate_image_id(image_path: Union[str, Path]) -> str:
+    """Generate an image ID."""
+    org, dataset, batch, _, filename = str(image_path).split("/")[-5:]
+    slug = Path(filename).stem
+    return os.path.join(org, dataset, batch, "images", slug)
+
+
+def list_local_images(data_directory: Union[str, Path]) -> list[Path]:
+    """List local images."""
+    return sorted(Path(data_directory).glob("**/images/*"))
 
 
-def version_dataset(dataset: str, slug: Optional[str] = None) -> dict[str, Any]:
-    """Version a dataset."""
-    payload = dict(dataset=dataset)
-    if slug is not None:
-        payload["slug"] = slug
-    version = OwlMLAPI.post("dataset-versions", payload)
-    while version == {}:
-        time.sleep(0.25)
-        version = OwlMLAPI.post("dataset-versions", payload)
-    return version
+def upload_images(
+    dataset: str, image_directory: Union[str, Path], batch: Optional[str] = None
+) -> dict[str, Any]:
+    """Upload images to a dataset."""
+    batch_response = _create_batch(dataset, batch)
+    images = list(Path(image_directory).glob("*"))
+    for image_path in tqdm(images):
+        image_response = _create_image(dataset, batch_response["slug"], image_path)
+        _upload_image(image_response["presigned_post"], image_path)
+        _complete_image(image_response["id"])
+    return _complete_batch(batch_response["slug"])
```

