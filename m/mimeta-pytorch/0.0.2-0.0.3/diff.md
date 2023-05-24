# Comparing `tmp/mimeta_pytorch-0.0.2.tar.gz` & `tmp/mimeta_pytorch-0.0.3.tar.gz`

## Comparing `mimeta_pytorch-0.0.2.tar` & `mimeta_pytorch-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.2/.python-version
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.2/requirements.txt
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.2/mimeta/__init__.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.2/mimeta/batches.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.2/mimeta/logger.py
--rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.2/mimeta/mimeta.py
--rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.2/mimeta/task_presampling.py
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.2/mimeta/tasks.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.2/.gitignore
--rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.2/LICENSE
--rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.2/LICENSE.LESSER
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.2/README.md
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/examples/cross_domain_maml.py
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/examples/cross_domain_pretraining.py
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/examples/imagenet-pretrained.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/mimeta/__init__.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/mimeta/batches.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/mimeta/logger.py
+-rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/mimeta/mimeta.py
+-rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/mimeta/task_presampling.py
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/mimeta/tasks.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/.gitignore
+-rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/LICENSE
+-rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/LICENSE.LESSER
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/README.md
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 mimeta_pytorch-0.0.3/PKG-INFO
```

### Comparing `mimeta_pytorch-0.0.2/mimeta/batches.py` & `mimeta_pytorch-0.0.3/mimeta/batches.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, Callable
 
-from torchcross.data.base import RandomChainTaskSource, BatchedTaskSource
+from torchcross.data import RandomChainTaskSource, BatchedTaskSource
 from .logger import logger
 from .mimeta import MIMeta
 
 
 class MultiMIMetaBatchTaskSource(RandomChainTaskSource):
     def __init__(
         self,
```

### Comparing `mimeta_pytorch-0.0.2/mimeta/mimeta.py` & `mimeta_pytorch-0.0.3/mimeta/mimeta.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import h5py
 import numpy as np
 import torch
 import yaml
 from PIL import Image
 from torchvision import transforms
 
-from torchcross.data.base import TaskSource
-from torchcross.data.task import TaskTarget
+from torchcross.data import TaskSource
+from torchcross.data import TaskTarget
 from .logger import logger
 
 
 def default_transform(input_size):
     return transforms.Compose(
         [
             transforms.Resize(input_size[1:]),
@@ -20,14 +20,15 @@
             transforms.Normalize((0.5,) * input_size[0], (0.5,) * input_size[0]),
         ]
     )
 
 
 class MIMeta(TaskSource):
     _data_path: str = None
+    _infos: dict[str, dict] = None
     _dataset_dir_mapping: dict[str, str] = None
     _available_tasks: dict[str, list[str]] = None
 
     def __init__(
         self,
         data_path,
         dataset_name,
@@ -55,24 +56,24 @@
 
         dataset_subdir = self._dataset_dir_mapping[dataset_name]
 
         # load info.yaml file and parse task information
         info_file = os.path.join(data_path, dataset_subdir, "info.yaml")
         with open(info_file, "r") as f:
             info = yaml.load(f, Loader=yaml.FullLoader)
-            task_info = next(
-                (t for t in info["tasks"] if t["task_name"] == task_name), None
+        task_info = next(
+            (t for t in info["tasks"] if t["task_name"] == task_name), None
+        )
+        if task_info is None:
+            raise ValueError(
+                f"No task with name '{task_name}' found for dataset '{dataset_name}'"
             )
-            if task_info is None:
-                raise ValueError(
-                    f"No task with name '{task_name}' found for dataset '{dataset_name}'"
-                )
-            self.classes = task_info["labels"]
-            self.task_target = TaskTarget[task_info["task_target"]]
-            self.input_size = info["input_size"]
+        self.classes = task_info["labels"]
+        self.task_target = TaskTarget[task_info["task_target"]]
+        self.input_size = info["input_size"]
 
         # set number of channels based on input size
         self.num_channels = self.input_size[0]
 
         # set transform to default if none is provided
         if self.transform is None:
             self.transform = default_transform(self.input_size)
@@ -92,15 +93,17 @@
             self.hdf5_images = h5py.File(self.hdf5_path, "r")["images"]
 
         if self.original_split is not None:
             split_file = os.path.join(
                 data_path, dataset_subdir, "original_splits", f"{original_split}.txt"
             )
             if not os.path.exists(split_file):
-                available_splits = [k for k, v in info["num_samples"].items() if v > 0]
+                available_splits = [
+                    k for k, v in info["original_splits_num_samples"].items() if v > 0
+                ]
                 raise ValueError(
                     f"Split '{original_split}' not found for dataset {dataset_name}. "
                     f"Available splits: {available_splits}"
                 )
             with open(split_file, "r") as f:
                 split_paths = [x.strip() for x in f.readlines()]
             self.split_indices = [
@@ -142,24 +145,37 @@
     @classmethod
     def get_available_tasks(cls, data_path: str) -> dict[str, list[str]]:
         if cls._available_tasks is None or cls._data_path != data_path:
             cls._read_dataset_info(data_path)
         return cls._available_tasks
 
     @classmethod
+    def get_info_dict(cls, data_path: str, dataset_name: str) -> dict:
+        if cls._dataset_dir_mapping is None or cls._data_path != data_path:
+            cls._read_dataset_info(data_path)
+        if dataset_name not in cls._infos:
+            raise ValueError(
+                f"Dataset '{dataset_name}' not found. "
+                f"Available datasets: {list(cls._infos.keys())}"
+            )
+        return cls._infos[dataset_name]
+
+    @classmethod
     def _read_dataset_info(cls, data_path: str):
         cls._dataset_dir_mapping = {}
         cls._available_tasks = {}
+        cls._infos = {}
         for subdir in os.listdir(data_path):
             subdir_path = os.path.join(data_path, subdir)
             if not os.path.isdir(subdir_path):
                 continue
             info_path = os.path.join(subdir_path, "info.yaml")
             if not os.path.isfile(info_path):
                 continue
             with open(info_path, "r") as f:
                 info = yaml.load(f, Loader=yaml.FullLoader)
+                cls._infos[info["name"]] = info
                 cls._dataset_dir_mapping[info["name"]] = subdir
                 cls._available_tasks[info["name"]] = [
                     t["task_name"] for t in info["tasks"]
                 ]
         cls._data_path = data_path
```

### Comparing `mimeta_pytorch-0.0.2/mimeta/task_presampling.py` & `mimeta_pytorch-0.0.3/mimeta/task_presampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import pickle as pkl
 
-from torchcross.data.meta import FewShotMetaDataset, SubTaskRandomFewShotMetaDataset
-from mimeta.mimeta import MIMeta
+from mimeta import MIMeta
+from torchcross.data.metadataset import FewShotMetaDataset, SubTaskRandomFewShotMetaDataset
 from torchcross.data.task import Task
 
-
 overwrite = False
 
 
 def available_tasks(data_path) -> list[tuple[str, str]]:
     task_dict = MIMeta.get_available_tasks(data_path)
     return [(dataset, task) for dataset, tasks in task_dict.items() for task in tasks]
 
@@ -66,16 +65,16 @@
         print("Length: None")
     task_list = [t for t in few_shot]
     print("Total: ", len(task_list))
     return task_list
 
 
 def save_few_shot_tasks(data_path, save_path=None):
-    n_query = 20
-    length = 400
+    n_query = 10
+    length = 100
     os.makedirs(save_path, exist_ok=True)
     # create few-shot instances for all tasks and all nshot values
     # and save them to pkl files
     for dataset, task in available_tasks(data_path):
         for n_support in [1, 2, 3, 5, 7, 10, 15, 20, 25, 30]:
             few_shot_tasks = create_few_shot_tasks(
                 data_path, dataset, task, n_support, n_query, length
@@ -89,15 +88,15 @@
                 )
             with open(os.path.join(save_path, file_name), "wb") as f:
                 pkl.dump(few_shot_tasks, f)
 
 
 def save_random_few_shot_tasks(data_path, save_path=None):
     n_query = 10
-    length = 20000
+    length = 1000
     n_support_min = 1
     n_support_max = 10
     os.makedirs(save_path, exist_ok=True)
     for dataset, task in available_tasks(data_path):
         few_shot_tasks = create_random_few_shot_tasks(
             data_path, dataset, task, n_support_min, n_support_max, n_query, length
         )
@@ -122,13 +121,13 @@
     parser.add_argument("--save_path", type=str, default="data/MIMeta_presampled")
     args = parser.parse_args()
     data_path = args.data_path
     save_path = args.save_path
 
     print("Available tasks:")
     print(available_tasks(data_path))
-    save_few_shot_tasks(data_path, save_path)
+    #save_few_shot_tasks(data_path, save_path)
     save_random_few_shot_tasks(data_path, save_path)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `mimeta_pytorch-0.0.2/mimeta/tasks.py` & `mimeta_pytorch-0.0.3/mimeta/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import pickle as pkl
 from typing import Optional, Callable
 
-from torchcross.data.meta import MetaDataset
+from torchcross.data.metadataset import MetaDataset
 from torchcross.data.task import Task
 from torchcross.utils.collate_fn import identity
 from .logger import logger
 from .mimeta import MIMeta
 
 
 class PickledMIMetaTaskDataset(MetaDataset):
```

### Comparing `mimeta_pytorch-0.0.2/LICENSE` & `mimeta_pytorch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mimeta_pytorch-0.0.2/LICENSE.LESSER` & `mimeta_pytorch-0.0.3/LICENSE.LESSER`

 * *Files identical despite different names*

### Comparing `mimeta_pytorch-0.0.2/pyproject.toml` & `mimeta_pytorch-0.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mimeta-pytorch"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="Stefano Woerner", email="stefano@woerner.eu" },
 ]
 description = "Library for using the MIMeta dataset"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
     "h5py~=3.8.0",
     "numpy~=1.24.3",
     "torch~=2.0.0",
     "PyYAML~=6.0",
     "Pillow~=9.5.0",
     "torchvision~=0.15.1",
-    "torchcross~=0.0.2",
+    "torchcross~=0.0.3",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/StefanoWoerner/mimeta-pytorch"
 "Issue Tracker" = "https://github.com/StefanoWoerner/mimeta-pytorch/issues"
```

### Comparing `mimeta_pytorch-0.0.2/PKG-INFO` & `mimeta_pytorch-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: mimeta-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library for using the MIMeta dataset
 Project-URL: Homepage, https://github.com/StefanoWoerner/mimeta-pytorch
 Project-URL: Issue Tracker, https://github.com/StefanoWoerner/mimeta-pytorch/issues
 Author-email: Stefano Woerner <stefano@woerner.eu>
 License-File: LICENSE
 License-File: LICENSE.LESSER
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.10
 Requires-Dist: h5py~=3.8.0
 Requires-Dist: numpy~=1.24.3
 Requires-Dist: pillow~=9.5.0
 Requires-Dist: pyyaml~=6.0
-Requires-Dist: torchcross~=0.0.2
+Requires-Dist: torchcross~=0.0.3
 Requires-Dist: torchvision~=0.15.1
 Requires-Dist: torch~=2.0.0
 Description-Content-Type: text/markdown
 
 # MIMeta for PyTorch
 
 ## Medical Imaging Meta Dataset
@@ -58,15 +59,15 @@
 is welcome.**
 
 ## Installation
 
 The toolbox can be installed via pip:
 
 ```bash
-pip install mimeta
+pip install mimeta-pytorch
 ```
 
 ## Basic Usage
 
 The MIMeta dataset can be accessed via the `mimeta.MIMeta` class, which extends the 
 `torch.utils.data.Dataset` class. See the basic example below:
 
@@ -99,8 +100,18 @@
 MIMeta can be used in conjunction with TorchCross to easily create cross-domain learning
 or few-shot learning experiments. To this end, MIMeta provides two convenience classes
 for generating batches from multiple MIMeta tasks and for generating few-shot insttances
 of multiple MIMeta tasks.
 
 ### Examples
 
-Coming soon.
+See the [examples](examples) directory for examples on how to use MIMeta in conjunction
+with TorchCross.
+- [`imagenet_pretrained.py`](examples/imagenet_pretraining.py) shows how you can test
+  pre-trained models on a few-shot instance of a MIMeta task.
+- [`cross_domain_pretraining.py`](examples/cross_domain_pretraining.py) shows how you
+  can perform cross-domain pre-training on different MIMeta tasks and then test the
+  pre-trained model on a few-shot instance of a MIMeta task.
+- [`cross_domain_maml.py`](examples/cross_domain_maml.py) shows how you can perform
+  cross-domain meta-learning with [MAML](https://arxiv.org/abs/1703.03400) on different
+  MIMeta tasks and then test the meta-learned model on multiple few-shot instances of a
+  MIMeta task.
```

