# Comparing `tmp/lightning-graphcore-0.1.0rc1.tar.gz` & `tmp/lightning-graphcore-0.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-graphcore-0.1.0rc1.tar", last modified: Tue May 23 13:36:27 2023, max compression
+gzip compressed data, was "lightning-graphcore-0.1.0rc2.tar", last modified: Tue May 23 21:22:33 2023, max compression
```

## Comparing `lightning-graphcore-0.1.0rc1.tar` & `lightning-graphcore-0.1.0rc2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:27.532030 lightning-graphcore-0.1.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-23 13:36:27.532030 lightning-graphcore-0.1.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:36:27.532030 lightning-graphcore-0.1.0rc1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4162 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:27.528030 lightning-graphcore-0.1.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:27.532030 lightning-graphcore-0.1.0rc1/src/lightning_graphcore/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)    18186 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:27.532030 lightning-graphcore-0.1.0rc1/src/lightning_graphcore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-23 13:36:27.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-23 13:36:27.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:36:27.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:36:27.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-23 13:36:27.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 13:36:27.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:22:33.558302 lightning-graphcore-0.1.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-23 21:22:20.000000 lightning-graphcore-0.1.0rc2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-05-23 21:22:20.000000 lightning-graphcore-0.1.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-23 21:22:20.000000 lightning-graphcore-0.1.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-23 21:22:33.558302 lightning-graphcore-0.1.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-23 21:22:20.000000 lightning-graphcore-0.1.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 21:22:20.000000 lightning-graphcore-0.1.0rc2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 21:22:33.558302 lightning-graphcore-0.1.0rc2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4162 2023-05-23 21:22:20.000000 lightning-graphcore-0.1.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:22:33.554302 lightning-graphcore-0.1.0rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:22:33.558302 lightning-graphcore-0.1.0rc2/src/lightning_graphcore/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-23 21:22:20.000000 lightning-graphcore-0.1.0rc2/src/lightning_graphcore/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-23 21:22:20.000000 lightning-graphcore-0.1.0rc2/src/lightning_graphcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-23 21:22:20.000000 lightning-graphcore-0.1.0rc2/src/lightning_graphcore/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-23 21:22:20.000000 lightning-graphcore-0.1.0rc2/src/lightning_graphcore/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18186 2023-05-23 21:22:20.000000 lightning-graphcore-0.1.0rc2/src/lightning_graphcore/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-23 21:22:20.000000 lightning-graphcore-0.1.0rc2/src/lightning_graphcore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:22:33.558302 lightning-graphcore-0.1.0rc2/src/lightning_graphcore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-23 21:22:33.000000 lightning-graphcore-0.1.0rc2/src/lightning_graphcore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-23 21:22:33.000000 lightning-graphcore-0.1.0rc2/src/lightning_graphcore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:22:33.000000 lightning-graphcore-0.1.0rc2/src/lightning_graphcore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:22:33.000000 lightning-graphcore-0.1.0rc2/src/lightning_graphcore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-23 21:22:33.000000 lightning-graphcore-0.1.0rc2/src/lightning_graphcore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 21:22:33.000000 lightning-graphcore-0.1.0rc2/src/lightning_graphcore.egg-info/top_level.txt
```

### Comparing `lightning-graphcore-0.1.0rc1/LICENSE` & `lightning-graphcore-0.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0rc1/MANIFEST.in` & `lightning-graphcore-0.1.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0rc1/PKG-INFO` & `lightning-graphcore-0.1.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-graphcore
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: Lightning support for GraphCore accelerators
 Home-page: https://github.com/Lightning-AI/lightning-graphcore
 Download-URL: https://github.com/Lightning-AI/lightning-graphcore
 Author: Lightning-AI et al.
 Author-email: name@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning-graphcore/issues
```

### Comparing `lightning-graphcore-0.1.0rc1/README.md` & `lightning-graphcore-0.1.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0rc1/setup.py` & `lightning-graphcore-0.1.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0rc1/src/lightning_graphcore/accelerator.py` & `lightning-graphcore-0.1.0rc2/src/lightning_graphcore/accelerator.py`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0rc1/src/lightning_graphcore/precision.py` & `lightning-graphcore-0.1.0rc2/src/lightning_graphcore/precision.py`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0rc1/src/lightning_graphcore/strategy.py` & `lightning-graphcore-0.1.0rc2/src/lightning_graphcore/strategy.py`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0rc1/src/lightning_graphcore/utils.py` & `lightning-graphcore-0.1.0rc2/src/lightning_graphcore/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,49 +9,50 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Union
 
-import lightning.pytorch as pl
 import torch
 from lightning_utilities.core.imports import package_available
 
 if package_available("lightning"):
     from lightning.fabric.utilities.device_dtype_mixin import _DeviceDtypeModuleMixin
+    from lightning.pytorch import LightningModule
     from lightning.pytorch.overrides.base import _LightningPrecisionModuleWrapperBase
 elif package_available("pytorch_lightning"):
+    from pytorch_lightning import LightningModule
     from pytorch_lightning.fabric.utilities.device_dtype_mixin import _DeviceDtypeModuleMixin
     from pytorch_lightning.overrides.base import _LightningPrecisionModuleWrapperBase
 
 
 class _LightningModuleWrapperBase(_DeviceDtypeModuleMixin, torch.nn.Module):
-    def __init__(self, forward_module: Union["pl.LightningModule", _LightningPrecisionModuleWrapperBase]) -> None:
+    def __init__(self, forward_module: Union[LightningModule, _LightningPrecisionModuleWrapperBase]) -> None:
         """Wrap the user's LightningModule and redirect the forward call to the appropriate `*_step()` methods.
 
         Inheriting classes may also modify the inputs or outputs of forward.
 
         Args:
             forward_module: The module to wrap. If it's not a LightningModule, it must have an attribute ``.module``
                 pointing to a LightningModule reference.
         """
         super().__init__()
-        if not isinstance(forward_module, pl.LightningModule) and (
-            not isinstance(getattr(forward_module, "module", None), pl.LightningModule)
+        if not isinstance(forward_module, LightningModule) and (
+            not isinstance(getattr(forward_module, "module", None), LightningModule)
         ):
             raise ValueError(
                 "`forward_module` must be a `LightningModule` instance or have an attribute `.module` pointing to one,"
                 f" got: {forward_module.__class__.__qualname__}"
             )
         self._forward_module = forward_module
 
     @property
-    def lightning_module(self) -> "pl.LightningModule":
-        if isinstance(self._forward_module, pl.LightningModule):
+    def lightning_module(self) -> LightningModule:
+        if isinstance(self._forward_module, LightningModule):
             return self._forward_module
         return self._forward_module.module
 
     def forward(self, *inputs: Any, **kwargs: Any) -> Any:
         pl_module = self.lightning_module
         trainer = pl_module._trainer
```

### Comparing `lightning-graphcore-0.1.0rc1/src/lightning_graphcore.egg-info/PKG-INFO` & `lightning-graphcore-0.1.0rc2/src/lightning_graphcore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-graphcore
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: Lightning support for GraphCore accelerators
 Home-page: https://github.com/Lightning-AI/lightning-graphcore
 Download-URL: https://github.com/Lightning-AI/lightning-graphcore
 Author: Lightning-AI et al.
 Author-email: name@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning-graphcore/issues
```

### Comparing `lightning-graphcore-0.1.0rc1/src/lightning_graphcore.egg-info/SOURCES.txt` & `lightning-graphcore-0.1.0rc2/src/lightning_graphcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

