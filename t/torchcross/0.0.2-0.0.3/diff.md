# Comparing `tmp/torchcross-0.0.2.tar.gz` & `tmp/torchcross-0.0.3.tar.gz`

## Comparing `torchcross-0.0.2.tar` & `torchcross-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,52 @@
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 torchcross-0.0.2/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/cd/__init__.py
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/cd/losses.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/cd/heads/__init__.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/cd/heads/classification.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/cd/metrics/__init__.py
--rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/cd/metrics/classification.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/data/__init__.py
--rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/data/base.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/data/task.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/data/meta/__init__.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/data/meta/base.py
--rw-r--r--   0        0        0    25445 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/data/meta/few_shot.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/data/meta/few_shot_dummies.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/models/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/models/lightning/__init__.py
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/models/lightning/classifier.py
--rw-r--r--   0        0        0     9005 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/models/lightning/cross_domain_classifier.py
--rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/models/lightning/diverse_maml.py
--rw-r--r--   0        0        0     7338 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/models/lightning/diverse_transfer.py
--rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/models/lightning/episodic_model.py
--rw-r--r--   0        0        0     8104 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/models/lightning/few_shot_adapter.py
--rw-r--r--   0        0        0     6661 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/models/lightning/maml.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/utils/__init__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 torchcross-0.0.2/torchcross/utils/collate_fn.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 torchcross-0.0.2/.gitignore
--rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 torchcross-0.0.2/LICENSE
--rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 torchcross-0.0.2/LICENSE.LESSER
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 torchcross-0.0.2/README.md
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 torchcross-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 torchcross-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 torchcross-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/test_task_source.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/.pytest_cache/README.md
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/meta_dataset/test_base.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/meta_dataset/test_collection.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/meta_dataset/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/meta_dataset/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/meta_dataset/.pytest_cache/README.md
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/meta_dataset/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/meta_dataset/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 torchcross-0.0.3/tests/data/meta_dataset/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/cd/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/cd/activations.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/cd/losses.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/cd/heads/__init__.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/cd/heads/classification.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/cd/metrics/__init__.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/cd/metrics/classification.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/data/__init__.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/data/task.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/data/task_source.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/data/metadataset/__init__.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/data/metadataset/base.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/data/metadataset/collection.py
+-rw-r--r--   0        0        0    16946 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/data/metadataset/few_shot.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/data/metadataset/few_shot_dummies.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/__init__.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/cross_domain.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/episodic.py
+-rw-r--r--   0        0        0     9720 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/maml.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/protonet.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/lightning/__init__.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/lightning/cross_domain.py
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/lightning/cross_domain_classifier.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/lightning/episodic.py
+-rw-r--r--   0        0        0     6927 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/lightning/maml.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/models/lightning/mixins.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/utils/__init__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/utils/collate_fn.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 torchcross-0.0.3/torchcross/utils/layers.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 torchcross-0.0.3/.gitignore
+-rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 torchcross-0.0.3/LICENSE
+-rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 torchcross-0.0.3/LICENSE.LESSER
+-rw-r--r--   0        0        0     7234 2020-02-02 00:00:00.000000 torchcross-0.0.3/README.md
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 torchcross-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 torchcross-0.0.3/PKG-INFO
```

### Comparing `torchcross-0.0.2/torchcross/cd/losses.py` & `torchcross-0.0.3/torchcross/cd/losses.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 from typing import Callable
 
 import torch
 import torch.nn.functional as F
 
 from torchcross.data.task import TaskTarget
 
+__all__ = ["get_loss_func"]
 
 def get_loss_func(
     task_target: TaskTarget, classes: dict[int, str], device: torch.device = None
 ) -> Callable[[torch.Tensor, torch.Tensor], torch.Tensor]:
+    """Get the loss function for a given task target and classes.
+
+    Args:
+        task_target: The task target.
+        classes: The classes for the task.
+        device: The device to create tensors needed for the loss function
+            on.
+
+    Returns:
+        A loss function that takes logits and labels and returns a loss
+        tensor.
+    """
     match task_target:
         case TaskTarget.MULTICLASS_CLASSIFICATION:
             return F.cross_entropy
         case TaskTarget.MULTILABEL_CLASSIFICATION | TaskTarget.BINARY_CLASSIFICATION:
             return lambda p, y: F.binary_cross_entropy_with_logits(p, y.float())
         case TaskTarget.ORDINAL_REGRESSION:
             class_to_idx = torch.full(
```

### Comparing `torchcross-0.0.2/torchcross/cd/metrics/classification.py` & `torchcross-0.0.3/torchcross/cd/metrics/classification.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,22 +6,26 @@
 
 from torchcross.data.task import TaskTarget
 
 
 def get_accuracy_func(
     task_target: TaskTarget, classes: dict[int, str], device: torch.device = None
 ) -> Callable[[torch.Tensor, torch.Tensor], torch.Tensor]:
-    """
-    Get the accuracy metric function for a given task target.
-    :param task_target: the task target
-    :param classes: a dictionary mapping class indices to class names
-    :param device: a torch device (needed for ordinal regression metric)
-    :return: a function expecting two tensors, the first being the
-    predictions and the second being the ground truth, and returning
-    the accuracy
+    """Get the accuracy function for a given task target and classes.
+
+    Args:
+        task_target: The task target.
+        classes: The classes for the task.
+        device: The device to create tensors needed for the accuracy
+            function on.
+
+    Returns:
+        A torchmetrics functional metric or a function wrapping a
+        torchmetrics functional metric for the given task target and
+        classes.
     """
     match task_target:
         case TaskTarget.MULTICLASS_CLASSIFICATION:
             return partial(
                 torchmetrics.functional.classification.multiclass_accuracy,
                 num_classes=len(classes),
             )
@@ -49,23 +53,27 @@
         case target:
             raise NotImplementedError(f"Unsupported task target: {target}")
 
 
 def get_auroc_func(
     task_target: TaskTarget, classes: dict[int, str], device: torch.device = None
 ) -> Callable[[torch.Tensor, torch.Tensor], torch.Tensor]:
-    """
-    Get the area under the ROC curve metric function for a given task
-    target.
-    :param task_target: the task target
-    :param classes: a dictionary mapping class indices to class names
-    :param device: a torch device (needed for ordinal regression metric)
-    :return: a function expecting two tensors, the first being the
-    predictions and the second being the ground truth, and returning
-    the area under the ROC curve
+    """Get the area under the ROC curve metric function for a given task
+    target and classes.
+
+    Args:
+        task_target: The task target.
+        classes: The classes for the task.
+        device: The device to create tensors needed for the metric
+            function on.
+
+    Returns:
+        A torchmetrics functional metric or a function wrapping a
+        torchmetrics functional metric for the given task target and
+        classes.
     """
     match task_target:
         case TaskTarget.MULTICLASS_CLASSIFICATION:
             return partial(
                 torchmetrics.functional.classification.multiclass_auroc,
                 num_classes=len(classes),
             )
```

### Comparing `torchcross-0.0.2/torchcross/data/base.py` & `torchcross-0.0.3/torchcross/data/task_source.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import bisect
 import random
 from abc import ABC
-import bisect
-from collections.abc import Sequence
+from collections.abc import Callable, Sequence
 
 import numpy as np
 import torch
 from torch.utils.data import (
     Dataset,
     ConcatDataset,
     BatchSampler,
@@ -13,64 +13,116 @@
     SequentialSampler,
     IterableDataset,
 )
 
 from torchcross.utils.collate_fn import identity
 from .task import TaskTarget, TaskDescription
 
+__all__ = [
+    "TaskSource",
+    "WrapTaskSource",
+    "BatchedTaskSource",
+    "RandomChainTaskSource",
+    "ConcatTaskSource",
+]
+
+from ..utils import to_numpy
+
 
 class TaskSource(Dataset, ABC):
+    """A dataset that can be used as a source to generate tasks."""
+
     task_target: TaskTarget
     labels: np.ndarray | torch.Tensor | Sequence
-    classes: dict[int, str] = None
+    classes: dict[int, str]
     task_identifier: str = ""
 
 
+class WrapTaskSource(TaskSource):
+    """Wraps a dataset as a task source."""
+
+    def __init__(
+        self,
+        dataset: Dataset,
+        task_target: TaskTarget,
+        classes: dict[int, str],
+        label_fn: Callable[[Dataset], np.ndarray | torch.Tensor | Sequence] = None,
+        task_identifier: str = "",
+    ):
+        self.dataset = dataset
+        self.task_target = task_target
+        self.classes = classes
+        self.task_identifier = task_identifier
+
+        def default_label_fn(ds: Dataset):
+            return np.stack([to_numpy(item[1]) for item in ds])
+
+        label_fn = label_fn if label_fn else default_label_fn
+        self.labels = label_fn(self.dataset)
+
+    def __getitem__(self, index):
+        return self.dataset[index]
+
+    def __len__(self):
+        return len(self.dataset)
+
+
 class BatchedTaskSource(TaskSource, IterableDataset):
     def __init__(
         self,
         task_source: TaskSource,
         batch_size: int,
         shuffle: bool = True,
         drop_last: bool = False,
         collate_fn=None,
+        with_task_description: bool = False,
     ):
         self.task_source = task_source
         self.task_target = task_source.task_target
         self.classes = task_source.classes
         self.task_identifier = task_source.task_identifier
+        self.with_task_description = with_task_description
+        if self.with_task_description:
+            self.task_description = TaskDescription(
+                self.task_target, self.classes, self.task_identifier
+            )
 
         sampler = (
             RandomSampler(self.task_source)
             if shuffle
             else SequentialSampler(self.task_source)
         )
         self.batch_sampler = BatchSampler(sampler, batch_size, drop_last)
         self.collate_fn = collate_fn if collate_fn else identity
 
     def __iter__(self):
         for batch in self.batch_sampler:
-            yield self.collate_fn([self.task_source[i] for i in batch])
+            if self.with_task_description:
+                yield (
+                    self.collate_fn([self.task_source[i] for i in batch]),
+                    self.task_description,
+                )
+            else:
+                yield self.collate_fn([self.task_source[i] for i in batch])
 
     def __len__(self):
         return len(self.batch_sampler)
 
 
 class RandomChainTaskSource(TaskSource, IterableDataset):
     def __init__(self, task_sources: list[BatchedTaskSource]):
         self.task_sources = task_sources
 
     def __iter__(self):
         iterators = [iter(ts) for ts in self.task_sources]
         # Calculate the weights of each iterator based on the batched task source length
         weights = [len(ts) for ts in self.task_sources]
         task_descriptions = [
-            TaskDescription(
-                ts.task_target, ts.classes, ts.task_identifier
-            ) for ts in self.task_sources
+            TaskDescription(ts.task_target, ts.classes, ts.task_identifier)
+            for ts in self.task_sources
         ]
         while iterators:
             # Randomly select an iterator with a probability proportional to its weight
             i = random.choices(range(len(self.task_sources)), weights=weights)[0]
             selected_iterator = iterators[i]
             try:
                 # Return one element from the selected iterator
@@ -102,7 +154,26 @@
             self.datasets[dataset_idx][sample_idx],
             TaskDescription(
                 self.datasets[dataset_idx].task_target,
                 self.datasets[dataset_idx].classes,
                 self.datasets[dataset_idx].task_identifier,
             ),
         )
+
+    def __len__(self):
+        return sum(len(d) for d in self.datasets)
+
+
+class SubsetTaskSource(TaskSource):
+    def __init__(self, task_source: TaskSource, indices: Sequence[int]):
+        self.task_source = task_source
+        self.indices = indices
+        self.task_target = task_source.task_target
+        self.classes = task_source.classes
+        self.task_identifier = task_source.task_identifier
+        self.labels = task_source.labels[indices]
+
+    def __getitem__(self, idx):
+        return self.task_source[self.indices[idx]]
+
+    def __len__(self):
+        return len(self.indices)
```

### Comparing `torchcross-0.0.2/torchcross/data/meta/base.py` & `torchcross-0.0.3/torchcross/data/metadataset/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 from collections.abc import Iterable, Iterator
 from typing import Any
 
 from torch.utils.data import Dataset, IterableDataset, ChainDataset
 
-from ..base import TaskSource
+from ..task_source import TaskSource
 from ..task import Task
 
 
 class MetaDataset(Dataset[Task], ABC):
     task_source: TaskSource
 
     @abstractmethod
```

### Comparing `torchcross-0.0.2/torchcross/data/meta/few_shot_dummies.py` & `torchcross-0.0.3/torchcross/data/metadataset/few_shot_dummies.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 
 from torchcross.utils.collate_fn import identity
 from . import MetaDataset
-from ..base import TaskSource
+from ..task_source import TaskSource
 from ..task import TaskTarget, Task
 
 
 class TakeFirstFewShotMetaDataset(MetaDataset):
     def __init__(
         self,
         dataset: TaskSource,
```

### Comparing `torchcross-0.0.2/LICENSE` & `torchcross-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.2/LICENSE.LESSER` & `torchcross-0.0.3/LICENSE.LESSER`

 * *Files identical despite different names*

### Comparing `torchcross-0.0.2/pyproject.toml` & `torchcross-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "torchcross"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="Stefano Woerner", email="stefano@woerner.eu" },
 ]
 description = "Easy-to-use PyTorch library for cross-domain learning, few-shot learning and meta-learning"
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
-    "h5py~=3.8.0",
     "numpy~=1.24.3",
     "torch~=2.0.0",
-    "PyYAML~=6.0",
-    "Pillow~=9.5.0",
-    "torchvision~=0.15.1",
+    "lightning~=2.0.2",
+    "torchmetrics~=0.11.4",
+    "omegaconf~=2.3.0",
+    "torchopt~=0.7.1",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/StefanoWoerner/torchcross"
 "Issue Tracker" = "https://github.com/StefanoWoerner/torchcross/issues"
```

