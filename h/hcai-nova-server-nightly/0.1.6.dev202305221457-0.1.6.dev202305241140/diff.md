# Comparing `tmp/hcai-nova-server-nightly-0.1.6.dev202305221457.tar.gz` & `tmp/hcai-nova-server-nightly-0.1.6.dev202305241140.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-server-nightly-0.1.6.dev202305221457.tar", last modified: Mon May 22 14:57:07 2023, max compression
+gzip compressed data, was "hcai-nova-server-nightly-0.1.6.dev202305241140.tar", last modified: Wed May 24 11:40:16 2023, max compression
```

## Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457.tar` & `hcai-nova-server-nightly-0.1.6.dev202305241140.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:57:07.361990 hcai-nova-server-nightly-0.1.6.dev202305221457/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-05-22 14:57:07.361990 hcai-nova-server-nightly-0.1.6.dev202305221457/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:57:07.361990 hcai-nova-server-nightly-0.1.6.dev202305221457/hcai_nova_server_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-05-22 14:57:07.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/hcai_nova_server_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-05-22 14:57:07.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/hcai_nova_server_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 14:57:07.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/hcai_nova_server_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-22 14:57:07.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/hcai_nova_server_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-22 14:57:07.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/hcai_nova_server_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:57:07.361990 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2568 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/nova_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:57:07.361990 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/cancel.py
--rw-r--r--   0 runner    (1001) docker     (122)    13062 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)     9891 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/train.py
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:57:07.361990 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:57:07.361990 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12151 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/explain_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      447 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/img_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/key_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/thread_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 14:57:07.361990 hcai-nova-server-nightly-0.1.6.dev202305221457/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-05-22 14:56:55.000000 hcai-nova-server-nightly-0.1.6.dev202305221457/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 11:40:16.158735 hcai-nova-server-nightly-0.1.6.dev202305241140/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-05-24 11:40:16.158735 hcai-nova-server-nightly-0.1.6.dev202305241140/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 11:40:16.154735 hcai-nova-server-nightly-0.1.6.dev202305241140/hcai_nova_server_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-05-24 11:40:16.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/hcai_nova_server_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      913 2023-05-24 11:40:16.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/hcai_nova_server_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 11:40:16.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/hcai_nova_server_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-24 11:40:16.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/hcai_nova_server_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-24 11:40:16.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/hcai_nova_server_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 11:40:16.154735 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2568 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/nova_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 11:40:16.158735 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/route/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/route/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13652 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/route/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9891 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/route/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/route/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/route/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/route/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/route/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/route/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 11:40:16.158735 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 11:40:16.158735 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12139 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/utils/explain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/utils/key_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/utils/thread_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-24 11:40:16.158735 hcai-nova-server-nightly-0.1.6.dev202305241140/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-05-24 11:40:01.000000 hcai-nova-server-nightly-0.1.6.dev202305241140/setup.py
```

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457/PKG-INFO` & `hcai-nova-server-nightly-0.1.6.dev202305241140/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.6.dev202305221457
+Version: 0.1.6.dev202305241140
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457/README.md` & `hcai-nova-server-nightly-0.1.6.dev202305241140/README.md`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457/hcai_nova_server_nightly.egg-info/PKG-INFO` & `hcai-nova-server-nightly-0.1.6.dev202305241140/hcai_nova_server_nightly.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.6.dev202305221457
+Version: 0.1.6.dev202305241140
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457/hcai_nova_server_nightly.egg-info/SOURCES.txt` & `hcai-nova-server-nightly-0.1.6.dev202305241140/hcai_nova_server_nightly.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,13 +19,12 @@
 nova_server/route/train.py
 nova_server/route/ui.py
 nova_server/templates/__init__.py
 nova_server/utils/__init__.py
 nova_server/utils/dataset_utils.py
 nova_server/utils/db_utils.py
 nova_server/utils/explain_utils.py
-nova_server/utils/img_utils.py
 nova_server/utils/import_utils.py
 nova_server/utils/key_utils.py
 nova_server/utils/log_utils.py
 nova_server/utils/status_utils.py
 nova_server/utils/thread_utils.py
```

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/nova_backend.py` & `hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/nova_backend.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/cancel.py` & `hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/route/cancel.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/explain.py` & `hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/route/explain.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,330 +1,330 @@
-import tensorflow as tf
-import io
-import numpy as np
-import io as inputoutput
-import base64
-import json
-import pickle
-import warnings
-import site as s
-from tensorflow.keras.models import load_model
-from PIL import Image
-from PIL import Image as pilimage
-from flask import Blueprint, Response, request
-from lime import lime_image
-from lime import lime_tabular
-from skimage.segmentation import mark_boundaries
-
-from nova_server.utils import explain_utils, img_utils
-
-# Initialization
-s.getusersitepackages()
-warnings.simplefilter("ignore")
-graph = tf.compat.v1.get_default_graph()
-explain = Blueprint("explain", __name__)
-
-
-@explain.route("/tfexplain", methods=["POST"])
-def explain_tfexplain():
-    global graph
-    data = {"success": "failed"}
-    #      # ensure an image was properly uploaded to our endpoint
-    if request.method == "POST":
-        if request.form.get("image"):
-
-            explainer = request.args.get("explainer")
-            # with graph.as_default():
-            model_path = request.form.get("model_path")
-            model = load_model(model_path)
-
-            # read the image in PIL format
-            image64 = request.form.get("image")
-            image = base64.b64decode(image64)
-            image = Image.open(io.BytesIO(image))
-            image = img_utils.prepare_image(image, target=(224, 224))
-            image = image * (1.0 / 255)
-            # img = tf.keras.preprocessing.image.img_to_array(image)
-            prediction = model.predict(image)
-            topClass = explain_utils.getTopXpredictions(prediction, 1)
-            print(topClass[0])
-            image = np.squeeze(image)
-
-            if explainer == "GRADCAM":
-                im = ([image], None)
-                from tf_explain.core.grad_cam import GradCAM
-
-                exp = GradCAM()
-                imgFinal = exp.explain(im, model, class_index=topClass[0][0])
-                # exp.save(imgFinal, ".", "grad_cam.png")
-
-            elif explainer == "OCCLUSIONSENSITIVITY":
-                im = ([image], None)
-                from tf_explain.core.occlusion_sensitivity import OcclusionSensitivity
-
-                exp = OcclusionSensitivity()
-                imgFinal = exp.explain(
-                    im, model, class_index=topClass[0][0], patch_size=10
-                )
-                # exp.save(imgFinal, ".", "grad_cam.png")
-
-            elif explainer == "GRADIENTSINPUTS":
-                im = (np.array([image]), None)
-                from tf_explain.core.gradients_inputs import GradientsInputs
-
-                exp = GradientsInputs()
-                imgFinal = exp.explain(im, model, class_index=topClass[0][0])
-                # exp.save(imgFinal, ".", "gradients_inputs.png")
-
-            elif explainer == "VANILLAGRADIENTS":
-                im = (np.array([image]), None)
-                from tf_explain.core.vanilla_gradients import VanillaGradients
-
-                exp = VanillaGradients()
-                imgFinal = exp.explain(im, model, class_index=topClass[0][0])
-                # exp.save(imgFinal, ".", "gradients_inputs.png")
-
-            elif explainer == "SMOOTHGRAD":
-                im = (np.array([image]), None)
-                from tf_explain.core.smoothgrad import SmoothGrad
-
-                exp = SmoothGrad()
-                imgFinal = exp.explain(im, model, class_index=topClass[0][0])
-                # exp.save(imgFinal, ".", "gradients_inputs.png")
-
-            elif explainer == "INTEGRATEDGRADIENTS":
-                im = (np.array([image]), None)
-                from tf_explain.core.integrated_gradients import IntegratedGradients
-
-                exp = IntegratedGradients()
-                imgFinal = exp.explain(im, model, class_index=topClass[0][0])
-                # exp.save(imgFinal, ".", "gradients_inputs.png")
-
-            elif explainer == "ACTIVATIONVISUALIZATION":
-                # need some solution to find out and submit layers name
-                im = (np.array([image]), None)
-                from tf_explain.core.activations import ExtractActivations
-
-                exp = ExtractActivations()
-                imgFinal = exp.explain(im, model, layers_name=["activation_1"])
-                # exp.save(imgFinal, ".", "gradients_inputs.png")
-
-            img = pilimage.fromarray(imgFinal)
-            imgByteArr = inputoutput.BytesIO()
-            img.save(imgByteArr, format="JPEG")
-            imgByteArr = imgByteArr.getvalue()
-
-            img64 = base64.b64encode(imgByteArr)
-            img64_string = img64.decode("utf-8")
-
-            data["explanation"] = img64_string
-            data["prediction"] = str(topClass[0][0])
-            data["prediction_score"] = str(topClass[0][1])
-            data["success"] = "success"
-
-    return Response(json.dumps(data), mimetype="text/plain")
-
-
-@explain.route("/innvestigate", methods=["POST"])
-def explain_innvestigate():
-    global graph
-    data = {"success": "failed"}
-    # ensure an image was properly uploaded to our endpoint
-    if request.method == "POST":
-        if request.form.get("image"):
-
-            postprocess = request.args.get("postprocess")
-            explainer = request.args.get("explainer")
-            lrpalpha = float(request.args.get("lrpalpha"))
-            lrpbeta = float(request.args.get("lrpbeta"))
-
-            with graph.as_default():
-                model_path = request.form.get("model_path")
-                model = load_model(model_path)
-
-                # read the image in PIL format
-                image64 = request.form.get("image")
-                image = base64.b64decode(image64)
-                image = Image.open(io.BytesIO(image))
-
-                # preprocess the image and prepare it for classification
-                image = img_utils.prepare_image(image, target=(224, 224))
-                image = image * (1.0 / 255)
-
-                # print(model.summary())
-                model_wo_sm = iutils.keras.graph.model_wo_softmax(model)
-
-                prediction = model.predict(image)
-                topClass = explain_utils.getTopXpredictions(prediction, 1)
-
-                model_wo_sm = iutils.keras.graph.model_wo_softmax(model)
-
-                analyzer = []
-
-                if explainer == "GUIDEDBACKPROP":
-                    analyzer = innvestigate.analyzer.GuidedBackprop(model_wo_sm)
-                elif explainer == "GRADIENT":
-                    analyzer = innvestigate.analyzer.Gradient(model_wo_sm)
-                elif explainer == "DECONVNET":
-                    analyzer = innvestigate.analyzer.Deconvnet(model_wo_sm)
-                elif explainer == "LRPEPSILON":
-                    analyzer = innvestigate.analyzer.LRPEpsilon(model_wo_sm)
-                elif explainer == "LRPZ":
-                    analyzer = innvestigate.analyzer.LRPZ(model_wo_sm)
-                elif explainer == "LRPALPHABETA":
-                    analyzer = innvestigate.analyzer.LRPAlphaBeta(
-                        model_wo_sm, alpha=lrpalpha, beta=lrpbeta
-                    )
-                elif explainer == "DEEPTAYLOR":
-                    analyzer = innvestigate.analyzer.DeepTaylor(model_wo_sm)
-
-                # Applying the analyzer
-                analysis = analyzer.analyze(image)
-
-                imgFinal = []
-
-                if postprocess == "GRAYMAP":
-                    imgFinal = explain_utils.graymap(analysis)[0]
-                elif postprocess == "HEATMAP":
-                    imgFinal = explain_utils.heatmap(analysis)[0]
-                elif postprocess == "BK_PROJ":
-                    imgFinal = explain_utils.bk_proj(analysis)[0]
-                elif postprocess == "GNUPLOT2":
-                    imgFinal = explain_utils.heatmapgnuplot2(analysis)[0]
-                elif postprocess == "CMRMAP":
-                    imgFinal = explain_utils.heatmapCMRmap(analysis)[0]
-                elif postprocess == "NIPY_SPECTRAL":
-                    imgFinal = explain_utils.heatmapnipy_spectral(analysis)[0]
-                elif postprocess == "RAINBOW":
-                    imgFinal = explain_utils.heatmap_rainbow(analysis)[0]
-                elif postprocess == "INFERNO":
-                    imgFinal = explain_utils.heatmap_inferno(analysis)[0]
-                elif postprocess == "GIST_HEAT":
-                    imgFinal = explain_utils.heatmap_gist_heat(analysis)[0]
-                elif postprocess == "VIRIDIS":
-                    imgFinal = explain_utils.heatmap_viridis(analysis)[0]
-
-                imgFinal = np.uint8(imgFinal * 255)
-
-                img = pilimage.fromarray(imgFinal)
-                imgByteArr = inputoutput.BytesIO()
-                img.save(imgByteArr, format="JPEG")
-                imgByteArr = imgByteArr.getvalue()
-
-                img64 = base64.b64encode(imgByteArr)
-                img64_string = img64.decode("utf-8")
-                data["explanation"] = img64_string
-                data["prediction"] = str(topClass[0][0])
-                data["prediction_score"] = str(topClass[0][1])
-                data["success"] = "success"
-
-    return Response(json.dumps(data), mimetype="text/plain")
-
-
-@explain.route("/lime", methods=["POST"])
-def explain_lime():
-    global graph
-    data = {"success": "failed"}
-
-    if request.method == "POST":
-        if request.form.get("image"):
-
-            top_labels = int(request.args.get("toplabels"))
-            hide_color = str(request.args.get("hidecolor"))
-            num_samples = int(request.args.get("numsamples"))
-            positive_only = str(request.args.get("positiveonly"))
-            num_features = int(request.args.get("numfeatures"))
-            hide_rest = str(request.args.get("hiderest"))
-
-            # read the image in PIL format
-            image64 = request.form.get("image")
-            image = base64.b64decode(image64)
-            image = Image.open(io.BytesIO(image))
-
-            with graph.as_default():
-
-                model_path = request.form.get("model_path")
-                model = load_model(model_path)
-
-                img = img_utils.prepare_image(image, (224, 224))
-                img = img * (1.0 / 255)
-                prediction = model.predict(img)
-                explainer = lime_image.LimeImageExplainer()
-                img = np.squeeze(img).astype("double")
-                explanation = explainer.explain_instance(
-                    img,
-                    model.predict,
-                    top_labels=top_labels,
-                    hide_color=hide_color == "True",
-                    num_samples=num_samples,
-                )
-
-                top_classes = explain_utils.getTopXpredictions(prediction, top_labels)
-
-                explanations = []
-
-                for cl in top_classes:
-                    temp, mask = explanation.get_image_and_mask(
-                        cl[0],
-                        positive_only=positive_only == "True",
-                        num_features=num_features,
-                        hide_rest=hide_rest == "True",
-                    )
-                    img_explained = mark_boundaries(temp, mask)
-                    img = Image.fromarray(np.uint8(img_explained * 255))
-                    img_byteArr = io.BytesIO()
-                    img.save(img_byteArr, format="JPEG")
-                    img_byteArr = img_byteArr.getvalue()
-                    img64 = base64.b64encode(img_byteArr)
-                    img64_string = img64.decode("utf-8")
-
-                    explanations.append((str(cl[0]), str(cl[1]), img64_string))
-
-                data["explanations"] = explanations
-                data["success"] = "success"
-
-    return Response(json.dumps(data), mimetype="text/plain")
-
-
-@explain.route("/tabular", methods=["POST"])
-def explain_tabular():
-    data = {"success": "failed"}
-
-    # TODO send sample to be explained
-
-    if request.method == "POST":
-
-        if request.form:
-
-            # data_dict = ast.literal_eval(json.loads(flask.request.data))
-
-            print("try open model")
-            with open(request.form.get("model_path"), "rb") as f:
-                model = pickle.load(f)
-
-            train_data = json.loads(request.form.get("data"))
-            dim = json.loads(request.form.get("dim"))
-            train_data = np.asarray(train_data)
-            train_data = train_data.reshape(((int)(train_data.size / dim), dim))
-            sample = json.loads(request.form.get("sample"))
-
-            num_features = int(request.args.get("numfeatures"))
-
-            explainer = lime_tabular.LimeTabularExplainer(
-                train_data, mode="classification", discretize_continuous=True
-            )
-            exp = explainer.explain_instance(
-                np.asarray(sample),
-                model.predict_proba,
-                num_features=num_features,
-                top_labels=1,
-            )
-
-            explanation_dictionary = {}
-
-            for entry in exp.as_list():
-                explanation_dictionary.update({entry[0]: entry[1]})
-
-            data["explanation"] = explanation_dictionary
-            data["success"] = "success"
-
-    return Response(json.dumps(data), mimetype="text/plain")
+# import tensorflow as tf
+# import io
+# import numpy as np
+# import io as inputoutput
+# import base64
+# import json
+# import pickle
+# import warnings
+# import site as s
+# from tensorflow.keras.models import load_model
+# from PIL import Image
+# from PIL import Image as pilimage
+# from flask import Blueprint, Response, request
+# from lime import lime_image
+# from lime import lime_tabular
+# from skimage.segmentation import mark_boundaries
+#
+# from nova_server.utils import explain_utils, img_utils
+#
+# # Initialization
+# s.getusersitepackages()
+# warnings.simplefilter("ignore")
+# graph = tf.compat.v1.get_default_graph()
+# explain = Blueprint("explain", __name__)
+#
+#
+# @explain.route("/tfexplain", methods=["POST"])
+# def explain_tfexplain():
+#     global graph
+#     data = {"success": "failed"}
+#     #      # ensure an image was properly uploaded to our endpoint
+#     if request.method == "POST":
+#         if request.form.get("image"):
+#
+#             explainer = request.args.get("explainer")
+#             # with graph.as_default():
+#             model_path = request.form.get("model_path")
+#             model = load_model(model_path)
+#
+#             # read the image in PIL format
+#             image64 = request.form.get("image")
+#             image = base64.b64decode(image64)
+#             image = Image.open(io.BytesIO(image))
+#             image = img_utils.prepare_image(image, target=(224, 224))
+#             image = image * (1.0 / 255)
+#             # img = tf.keras.preprocessing.image.img_to_array(image)
+#             prediction = model.predict(image)
+#             topClass = explain_utils.getTopXpredictions(prediction, 1)
+#             print(topClass[0])
+#             image = np.squeeze(image)
+#
+#             if explainer == "GRADCAM":
+#                 im = ([image], None)
+#                 from tf_explain.core.grad_cam import GradCAM
+#
+#                 exp = GradCAM()
+#                 imgFinal = exp.explain(im, model, class_index=topClass[0][0])
+#                 # exp.save(imgFinal, ".", "grad_cam.png")
+#
+#             elif explainer == "OCCLUSIONSENSITIVITY":
+#                 im = ([image], None)
+#                 from tf_explain.core.occlusion_sensitivity import OcclusionSensitivity
+#
+#                 exp = OcclusionSensitivity()
+#                 imgFinal = exp.explain(
+#                     im, model, class_index=topClass[0][0], patch_size=10
+#                 )
+#                 # exp.save(imgFinal, ".", "grad_cam.png")
+#
+#             elif explainer == "GRADIENTSINPUTS":
+#                 im = (np.array([image]), None)
+#                 from tf_explain.core.gradients_inputs import GradientsInputs
+#
+#                 exp = GradientsInputs()
+#                 imgFinal = exp.explain(im, model, class_index=topClass[0][0])
+#                 # exp.save(imgFinal, ".", "gradients_inputs.png")
+#
+#             elif explainer == "VANILLAGRADIENTS":
+#                 im = (np.array([image]), None)
+#                 from tf_explain.core.vanilla_gradients import VanillaGradients
+#
+#                 exp = VanillaGradients()
+#                 imgFinal = exp.explain(im, model, class_index=topClass[0][0])
+#                 # exp.save(imgFinal, ".", "gradients_inputs.png")
+#
+#             elif explainer == "SMOOTHGRAD":
+#                 im = (np.array([image]), None)
+#                 from tf_explain.core.smoothgrad import SmoothGrad
+#
+#                 exp = SmoothGrad()
+#                 imgFinal = exp.explain(im, model, class_index=topClass[0][0])
+#                 # exp.save(imgFinal, ".", "gradients_inputs.png")
+#
+#             elif explainer == "INTEGRATEDGRADIENTS":
+#                 im = (np.array([image]), None)
+#                 from tf_explain.core.integrated_gradients import IntegratedGradients
+#
+#                 exp = IntegratedGradients()
+#                 imgFinal = exp.explain(im, model, class_index=topClass[0][0])
+#                 # exp.save(imgFinal, ".", "gradients_inputs.png")
+#
+#             elif explainer == "ACTIVATIONVISUALIZATION":
+#                 # need some solution to find out and submit layers name
+#                 im = (np.array([image]), None)
+#                 from tf_explain.core.activations import ExtractActivations
+#
+#                 exp = ExtractActivations()
+#                 imgFinal = exp.explain(im, model, layers_name=["activation_1"])
+#                 # exp.save(imgFinal, ".", "gradients_inputs.png")
+#
+#             img = pilimage.fromarray(imgFinal)
+#             imgByteArr = inputoutput.BytesIO()
+#             img.save(imgByteArr, format="JPEG")
+#             imgByteArr = imgByteArr.getvalue()
+#
+#             img64 = base64.b64encode(imgByteArr)
+#             img64_string = img64.decode("utf-8")
+#
+#             data["explanation"] = img64_string
+#             data["prediction"] = str(topClass[0][0])
+#             data["prediction_score"] = str(topClass[0][1])
+#             data["success"] = "success"
+#
+#     return Response(json.dumps(data), mimetype="text/plain")
+#
+#
+# @explain.route("/innvestigate", methods=["POST"])
+# def explain_innvestigate():
+#     global graph
+#     data = {"success": "failed"}
+#     # ensure an image was properly uploaded to our endpoint
+#     if request.method == "POST":
+#         if request.form.get("image"):
+#
+#             postprocess = request.args.get("postprocess")
+#             explainer = request.args.get("explainer")
+#             lrpalpha = float(request.args.get("lrpalpha"))
+#             lrpbeta = float(request.args.get("lrpbeta"))
+#
+#             with graph.as_default():
+#                 model_path = request.form.get("model_path")
+#                 model = load_model(model_path)
+#
+#                 # read the image in PIL format
+#                 image64 = request.form.get("image")
+#                 image = base64.b64decode(image64)
+#                 image = Image.open(io.BytesIO(image))
+#
+#                 # preprocess the image and prepare it for classification
+#                 image = img_utils.prepare_image(image, target=(224, 224))
+#                 image = image * (1.0 / 255)
+#
+#                 # print(model.summary())
+#                 model_wo_sm = iutils.keras.graph.model_wo_softmax(model)
+#
+#                 prediction = model.predict(image)
+#                 topClass = explain_utils.getTopXpredictions(prediction, 1)
+#
+#                 model_wo_sm = iutils.keras.graph.model_wo_softmax(model)
+#
+#                 analyzer = []
+#
+#                 if explainer == "GUIDEDBACKPROP":
+#                     analyzer = innvestigate.analyzer.GuidedBackprop(model_wo_sm)
+#                 elif explainer == "GRADIENT":
+#                     analyzer = innvestigate.analyzer.Gradient(model_wo_sm)
+#                 elif explainer == "DECONVNET":
+#                     analyzer = innvestigate.analyzer.Deconvnet(model_wo_sm)
+#                 elif explainer == "LRPEPSILON":
+#                     analyzer = innvestigate.analyzer.LRPEpsilon(model_wo_sm)
+#                 elif explainer == "LRPZ":
+#                     analyzer = innvestigate.analyzer.LRPZ(model_wo_sm)
+#                 elif explainer == "LRPALPHABETA":
+#                     analyzer = innvestigate.analyzer.LRPAlphaBeta(
+#                         model_wo_sm, alpha=lrpalpha, beta=lrpbeta
+#                     )
+#                 elif explainer == "DEEPTAYLOR":
+#                     analyzer = innvestigate.analyzer.DeepTaylor(model_wo_sm)
+#
+#                 # Applying the analyzer
+#                 analysis = analyzer.analyze(image)
+#
+#                 imgFinal = []
+#
+#                 if postprocess == "GRAYMAP":
+#                     imgFinal = explain_utils.graymap(analysis)[0]
+#                 elif postprocess == "HEATMAP":
+#                     imgFinal = explain_utils.heatmap(analysis)[0]
+#                 elif postprocess == "BK_PROJ":
+#                     imgFinal = explain_utils.bk_proj(analysis)[0]
+#                 elif postprocess == "GNUPLOT2":
+#                     imgFinal = explain_utils.heatmapgnuplot2(analysis)[0]
+#                 elif postprocess == "CMRMAP":
+#                     imgFinal = explain_utils.heatmapCMRmap(analysis)[0]
+#                 elif postprocess == "NIPY_SPECTRAL":
+#                     imgFinal = explain_utils.heatmapnipy_spectral(analysis)[0]
+#                 elif postprocess == "RAINBOW":
+#                     imgFinal = explain_utils.heatmap_rainbow(analysis)[0]
+#                 elif postprocess == "INFERNO":
+#                     imgFinal = explain_utils.heatmap_inferno(analysis)[0]
+#                 elif postprocess == "GIST_HEAT":
+#                     imgFinal = explain_utils.heatmap_gist_heat(analysis)[0]
+#                 elif postprocess == "VIRIDIS":
+#                     imgFinal = explain_utils.heatmap_viridis(analysis)[0]
+#
+#                 imgFinal = np.uint8(imgFinal * 255)
+#
+#                 img = pilimage.fromarray(imgFinal)
+#                 imgByteArr = inputoutput.BytesIO()
+#                 img.save(imgByteArr, format="JPEG")
+#                 imgByteArr = imgByteArr.getvalue()
+#
+#                 img64 = base64.b64encode(imgByteArr)
+#                 img64_string = img64.decode("utf-8")
+#                 data["explanation"] = img64_string
+#                 data["prediction"] = str(topClass[0][0])
+#                 data["prediction_score"] = str(topClass[0][1])
+#                 data["success"] = "success"
+#
+#     return Response(json.dumps(data), mimetype="text/plain")
+#
+#
+# @explain.route("/lime", methods=["POST"])
+# def explain_lime():
+#     global graph
+#     data = {"success": "failed"}
+#
+#     if request.method == "POST":
+#         if request.form.get("image"):
+#
+#             top_labels = int(request.args.get("toplabels"))
+#             hide_color = str(request.args.get("hidecolor"))
+#             num_samples = int(request.args.get("numsamples"))
+#             positive_only = str(request.args.get("positiveonly"))
+#             num_features = int(request.args.get("numfeatures"))
+#             hide_rest = str(request.args.get("hiderest"))
+#
+#             # read the image in PIL format
+#             image64 = request.form.get("image")
+#             image = base64.b64decode(image64)
+#             image = Image.open(io.BytesIO(image))
+#
+#             with graph.as_default():
+#
+#                 model_path = request.form.get("model_path")
+#                 model = load_model(model_path)
+#
+#                 img = img_utils.prepare_image(image, (224, 224))
+#                 img = img * (1.0 / 255)
+#                 prediction = model.predict(img)
+#                 explainer = lime_image.LimeImageExplainer()
+#                 img = np.squeeze(img).astype("double")
+#                 explanation = explainer.explain_instance(
+#                     img,
+#                     model.predict,
+#                     top_labels=top_labels,
+#                     hide_color=hide_color == "True",
+#                     num_samples=num_samples,
+#                 )
+#
+#                 top_classes = explain_utils.getTopXpredictions(prediction, top_labels)
+#
+#                 explanations = []
+#
+#                 for cl in top_classes:
+#                     temp, mask = explanation.get_image_and_mask(
+#                         cl[0],
+#                         positive_only=positive_only == "True",
+#                         num_features=num_features,
+#                         hide_rest=hide_rest == "True",
+#                     )
+#                     img_explained = mark_boundaries(temp, mask)
+#                     img = Image.fromarray(np.uint8(img_explained * 255))
+#                     img_byteArr = io.BytesIO()
+#                     img.save(img_byteArr, format="JPEG")
+#                     img_byteArr = img_byteArr.getvalue()
+#                     img64 = base64.b64encode(img_byteArr)
+#                     img64_string = img64.decode("utf-8")
+#
+#                     explanations.append((str(cl[0]), str(cl[1]), img64_string))
+#
+#                 data["explanations"] = explanations
+#                 data["success"] = "success"
+#
+#     return Response(json.dumps(data), mimetype="text/plain")
+#
+#
+# @explain.route("/tabular", methods=["POST"])
+# def explain_tabular():
+#     data = {"success": "failed"}
+#
+#     # TODO send sample to be explained
+#
+#     if request.method == "POST":
+#
+#         if request.form:
+#
+#             # data_dict = ast.literal_eval(json.loads(flask.request.data))
+#
+#             print("try open model")
+#             with open(request.form.get("model_path"), "rb") as f:
+#                 model = pickle.load(f)
+#
+#             train_data = json.loads(request.form.get("data"))
+#             dim = json.loads(request.form.get("dim"))
+#             train_data = np.asarray(train_data)
+#             train_data = train_data.reshape(((int)(train_data.size / dim), dim))
+#             sample = json.loads(request.form.get("sample"))
+#
+#             num_features = int(request.args.get("numfeatures"))
+#
+#             explainer = lime_tabular.LimeTabularExplainer(
+#                 train_data, mode="classification", discretize_continuous=True
+#             )
+#             exp = explainer.explain_instance(
+#                 np.asarray(sample),
+#                 model.predict_proba,
+#                 num_features=num_features,
+#                 top_labels=1,
+#             )
+#
+#             explanation_dictionary = {}
+#
+#             for entry in exp.as_list():
+#                 explanation_dictionary.update({entry[0]: entry[1]})
+#
+#             data["explanation"] = explanation_dictionary
+#             data["success"] = "success"
+#
+#     return Response(json.dumps(data), mimetype="text/plain")
```

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/extract.py` & `hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/route/extract.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/log.py` & `hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/route/log.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/predict.py` & `hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/route/predict.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/status.py` & `hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/route/status.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/route/train.py` & `hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/route/train.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/dataset_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/db_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/utils/db_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,19 +108,19 @@
                     'name': <text>, 'conf': <confidence>
                 }
             }
         }
         db_handler ():
         logger ():
 
-    Returns:
-
     """
+
     annotations = {}
     """Temp fix"""
+
     results.pop("values", None)
     results.pop("confidences", None)
 
     for frame, results in results.items():
         frame_info = frame.split("_")
         frame_from = float(frame_info[-2])
         frame_to = float(frame_info[-1])
```

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/explain_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/utils/explain_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/import_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/key_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/utils/key_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/log_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/status_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457/nova_server/utils/thread_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305241140/nova_server/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305221457/setup.py` & `hcai-nova-server-nightly-0.1.6.dev202305241140/setup.py`

 * *Files identical despite different names*

