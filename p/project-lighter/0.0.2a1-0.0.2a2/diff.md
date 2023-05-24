# Comparing `tmp/project_lighter-0.0.2a1.tar.gz` & `tmp/project_lighter-0.0.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project_lighter-0.0.2a1.tar", max compression
+gzip compressed data, was "project_lighter-0.0.2a2.tar", max compression
```

## Comparing `project_lighter-0.0.2a1.tar` & `project_lighter-0.0.2a2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1080 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/LICENSE
--rw-r--r--   0        0        0      485 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/README.md
--rw-r--r--   0        0        0       67 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/__init__.py
--rw-r--r--   0        0        0      125 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/callbacks/__init__.py
--rw-r--r--   0        0        0    13987 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/callbacks/logger.py
--rw-r--r--   0        0        0     5784 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/callbacks/utils.py
--rw-r--r--   0        0        0        0 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/callbacks/writer/__init__.py
--rw-r--r--   0        0        0     7593 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/callbacks/writer/base.py
--rw-r--r--   0        0        0     2662 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/callbacks/writer/file.py
--rw-r--r--   0        0        0     2427 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/callbacks/writer/table.py
--rw-r--r--   0        0        0    21386 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/system.py
--rw-r--r--   0        0        0       36 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/utils/__init__.py
--rw-r--r--   0        0        0     3510 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/utils/cli.py
--rw-r--r--   0        0        0     2352 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/utils/collate.py
--rw-r--r--   0        0        0     1424 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/utils/dynamic_imports.py
--rw-r--r--   0        0        0     3431 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/utils/freezer.py
--rw-r--r--   0        0        0     2618 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/utils/misc.py
--rw-r--r--   0        0        0     5881 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/utils/model.py
--rw-r--r--   0        0        0       24 2023-05-07 04:43:34.398168 project_lighter-0.0.2a1/lighter/version.py
--rw-r--r--   0        0        0     4399 2023-05-07 04:43:34.346168 project_lighter-0.0.2a1/pyproject.toml
--rw-r--r--   0        0        0     2104 1970-01-01 00:00:00.000000 project_lighter-0.0.2a1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/LICENSE
+-rw-r--r--   0        0        0      485 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/README.md
+-rw-r--r--   0        0        0       67 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/__init__.py
+-rw-r--r--   0        0        0      125 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/callbacks/__init__.py
+-rw-r--r--   0        0        0    14196 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/callbacks/logger.py
+-rw-r--r--   0        0        0     6508 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/callbacks/utils.py
+-rw-r--r--   0        0        0        0 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/callbacks/writer/__init__.py
+-rw-r--r--   0        0        0     7593 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/callbacks/writer/base.py
+-rw-r--r--   0        0        0     2662 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/callbacks/writer/file.py
+-rw-r--r--   0        0        0     2427 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/callbacks/writer/table.py
+-rw-r--r--   0        0        0    19790 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/system.py
+-rw-r--r--   0        0        0       36 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/utils/__init__.py
+-rw-r--r--   0        0        0      627 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/utils/cli.py
+-rw-r--r--   0        0        0     2566 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/utils/collate.py
+-rw-r--r--   0        0        0     1547 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/utils/dynamic_imports.py
+-rw-r--r--   0        0        0     3431 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/utils/freezer.py
+-rw-r--r--   0        0        0     2278 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/utils/misc.py
+-rw-r--r--   0        0        0     5881 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/utils/model.py
+-rw-r--r--   0        0        0     2483 2023-05-24 14:42:41.920801 project_lighter-0.0.2a2/lighter/utils/runner.py
+-rw-r--r--   0        0        0       24 2023-05-24 14:43:03.884755 project_lighter-0.0.2a2/lighter/version.py
+-rw-r--r--   0        0        0     4399 2023-05-24 14:43:03.832755 project_lighter-0.0.2a2/pyproject.toml
+-rw-r--r--   0        0        0     1854 1970-01-01 00:00:00.000000 project_lighter-0.0.2a2/PKG-INFO
```

### Comparing `project_lighter-0.0.2a1/LICENSE` & `project_lighter-0.0.2a2/LICENSE`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a1/lighter/callbacks/logger.py` & `project_lighter-0.0.2a2/lighter/callbacks/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import Any, Dict, Union
 
 import sys
 from datetime import datetime
 from pathlib import Path
 
 import torch
+import yaml
 from loguru import logger
+from monai.bundle.config_parser import ConfigParser
 from monai.utils.module import optional_import
 from pytorch_lightning import Callback, Trainer
 
 from lighter import LighterSystem
 from lighter.callbacks.utils import get_lighter_mode, is_data_type_supported, parse_data, preprocess_image
 from lighter.utils.dynamic_imports import OPTIONAL_IMPORTS
 
@@ -41,14 +43,17 @@
         self.loss = {"train": 0, "val": 0}
         # Epoch steps. Resets at each epoch. No `test` mode step counter as loss is not calculated for it.
         self.epoch_step_counter = {"train": 0, "val": 0}
         # Global steps. Replaces `Trainer.global_step` because it counts optimizer steps
         # instead of batch steps, which can be problematic when using gradient accumulation.
         self.global_step_counter = {"train": 0, "val": 0, "test": 0}
 
+        # Initialized from runner module
+        self.config = None
+
     def setup(self, trainer: Trainer, pl_module: LighterSystem, stage: str) -> None:
         """
         Initialize logging for the LighterSystem.
         TODO: improve this docstring.
 
         Args:
             trainer (Trainer): Trainer, passed automatically by PyTorch Lightning.
@@ -59,40 +64,38 @@
             logger.error("When using LighterLogger, set Trainer(logger=None).")
             sys.exit()
 
         if not trainer.is_global_zero:
             return
 
         self.log_dir.mkdir(parents=True)
-
-        # Load the dumped config file to log it to the loggers.
-        # config = yaml.safe_load(open(self.log_dir / "config.yaml"))
+        logger.info(f"Logging to {self.log_dir}")
 
         # Loguru log file.
-        # logger.add(sink=self.log_dir / f"{stage}.log")
+        logger.add(sink=self.log_dir / f"{stage}.log")
 
         # Tensorboard initialization.
         if self.tensorboard:
             # Tensorboard is a part of PyTorch, no need to check if it is not available.
             OPTIONAL_IMPORTS["tensorboard"], _ = optional_import("torch.utils.tensorboard")
             tensorboard_dir = self.log_dir / "tensorboard"
             tensorboard_dir.mkdir()
             self.tensorboard = OPTIONAL_IMPORTS["tensorboard"].SummaryWriter(log_dir=tensorboard_dir)
-            # self.tensorboard.add_hparams(config)
+            # self.tensorboard.add_hparams(config, {}) # TODO: Tensorboard asks for a metric dict along with hparam dict
+            # https://pytorch.org/docs/stable/tensorboard.html#torch.utils.tensorboard.writer.SummaryWriter.add_hparams
 
         # Wandb initialization.
         if self.wandb:
             OPTIONAL_IMPORTS["wandb"], wandb_available = optional_import("wandb")
             if not wandb_available:
                 logger.error("Weights & Biases not installed. To install it, run `pip install wandb`. Exiting.")
                 sys.exit()
             wandb_dir = self.log_dir / "wandb"
             wandb_dir.mkdir()
-            self.wandb = OPTIONAL_IMPORTS["wandb"].init(project=self.project, dir=wandb_dir)
-            # self.wandb.config.update(config)
+            self.wandb = OPTIONAL_IMPORTS["wandb"].init(project=self.project, dir=wandb_dir, config=self.config)
 
     def teardown(self, trainer: Trainer, pl_module: LighterSystem, stage: str) -> None:
         if not trainer.is_global_zero:
             return
         if self.tensorboard:
             self.tensorboard.close()
```

### Comparing `project_lighter-0.0.2a1/lighter/callbacks/utils.py` & `project_lighter-0.0.2a2/lighter/callbacks/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,25 +13,27 @@
     Returns:
         str: name of the Lighter mode.
     """
     lightning_to_lighter = {"train": "train", "validate": "val", "test": "test"}
     return lightning_to_lighter[lightning_stage]
 
 
-def is_data_type_supported(data: Any) -> bool:
-    """Check the input data for its type. Valid data types are:
+def is_data_type_supported(data: Union[Any, List[Any], Dict[str, Union[Any, List[Any], Tuple[Any]]]]) -> bool:
+    """
+    Check the input data recursively for its type. Valid data types are:
         - torch.Tensor
         - List[torch.Tensor]
         - Tuple[torch.Tensor]
         - Dict[str, torch.Tensor]
         - Dict[str, List[torch.Tensor]]
         - Dict[str, Tuple[torch.Tensor]]
+        - Nested combinations of the above
 
     Args:
-        data (Any): input data to check
+        data (Union[Any, List[Any], Dict[str, Union[Any, List[Any], Tuple[Any]]]]): Input data to check.
 
     Returns:
         bool: True if the data type is supported, False otherwise.
     """
     if isinstance(data, dict):
         is_valid = all(is_data_type_supported(elem) for elem in data.values())
     elif isinstance(data, (list, tuple)):
@@ -40,44 +42,59 @@
         is_valid = True
     else:
         is_valid = False
     return is_valid
 
 
 def parse_data(
-    data: Union[Any, List[Any], Dict[str, Any], Dict[str, List[Any]], Dict[str, Tuple[Any]]]
+    data: Union[Any, List[Any], Dict[str, Union[Any, List[Any], Tuple[Any]]]], prefix: Optional[str] = None
 ) -> Dict[Optional[str], Any]:
-    """Parse the input data as follows:
-        - If dict, go over all keys and values, unpacking list and tuples, and assigning them all
-          a unique identifier based on the original key and their position if they were a list/tuple.
-        - If list/tuple, enumerate them and use their position as key for each value of the list/tuple.
-        - If any other type, return it as-is with the key set to 'None'. A 'None' key indicates that no
-          identifier is needed because no parsing ocurred.
+    """
+    Parse the input data recursively, handling nested dictionaries, lists, and tuples.
+
+    This function will recursively parse the input data, unpacking nested dictionaries, lists, and tuples. The result
+    will be a dictionary where each key is a unique identifier reflecting the data's original structure (dict keys
+    or list/tuple positions) and each value is a non-container data type from the input data.
 
     Args:
-        data (Any, List[Any], Dict[str, Any], Dict[str, List[Any]], Dict[str, Tuple[Any]):
-            input data to parse.
+        data (Union[Any, List[Any], Dict[str, Union[Any, List[Any], Tuple[Any]]]]): Input data to parse.
+        prefix (Optional[str]): Current prefix for keys in the result dictionary. Defaults to None.
 
     Returns:
-        Dict[Optional[str], Any]: a dict where key is either a string
-            identifier or `None`, and value the parsed output.
+        Dict[Optional[str], Any]: A dictionary where key is either a string identifier or `None`, and value is the parsed output.
+
+    Example:
+        input_data = {
+            "a": [1, 2],
+            "b": {"c": (3, 4), "d": 5}
+        }
+        output_data = parse_data(input_data)
+        # Output:
+        # {
+        #     'a_0': 1,
+        #     'a_1': 2,
+        #     'b_c_0': 3,
+        #     'b_c_1': 4,
+        #     'b_d': 5
+        # }
     """
     result = {}
     if isinstance(data, dict):
         for key, value in data.items():
-            if isinstance(value, (list, tuple)):
-                for idx, element in enumerate(value):
-                    result[f"{key}_{idx}" if len(value) > 1 else key] = element
-            else:
-                result[key] = value
+            # Recursively parse the value with an updated prefix
+            sub_result = parse_data(value, prefix=f"{prefix}_{key}" if prefix else key)
+            result.update(sub_result)
     elif isinstance(data, (list, tuple)):
         for idx, element in enumerate(data):
-            result[str(idx)] = element
+            # Recursively parse the element with an updated prefix
+            sub_result = parse_data(element, prefix=f"{prefix}_{idx}" if prefix else str(idx))
+            result.update(sub_result)
     else:
-        result[None] = data
+        # Assign the value to the result dictionary using the current prefix as its key
+        result[prefix] = data
     return result
 
 
 def gather_tensors(
     inputs: Union[List[Union[torch.Tensor, List, Tuple, Dict]], Tuple[Union[torch.Tensor, List, Tuple, Dict]]]
 ) -> Union[List, Dict]:
     """Recursively gather tensors. Tensors can be standalone or inside of other data structures (list/tuple/dict).
```

### Comparing `project_lighter-0.0.2a1/lighter/callbacks/writer/base.py` & `project_lighter-0.0.2a2/lighter/callbacks/writer/base.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a1/lighter/callbacks/writer/file.py` & `project_lighter-0.0.2a2/lighter/callbacks/writer/file.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a1/lighter/callbacks/writer/table.py` & `project_lighter-0.0.2a2/lighter/callbacks/writer/table.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a1/lighter/system.py` & `project_lighter-0.0.2a2/lighter/system.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import torch
 from loguru import logger
 from torch.nn import Module
 from torch.optim import Optimizer
 from torch.utils.data import DataLoader, Dataset, Sampler
 from torchmetrics import Metric, MetricCollection
 
-from lighter.utils.collate import collate_fn_replace_corrupted
-from lighter.utils.misc import countargs, ensure_list, get_name, hasarg
+from lighter.utils.collate import collate_replace_corrupted
+from lighter.utils.misc import ensure_list, get_name, hasarg
 from lighter.utils.model import reshape_pred_if_single_value_prediction
 
 
 class LighterSystem(pl.LightningModule):
     """_summary_
 
     Args:
@@ -161,41 +161,28 @@
 
         Args:
             input (torch.Tensor, List[torch.Tensor], Tuple[torch.Tensor], Dict[str, torch.Tensor]): input to the model.
 
         Returns:
             Any: output of the model.
         """
+        # Freeze the layers if specified so.
+        if self.freezer is not None:
+            self.freezer(self.model, self.global_step, self.current_epoch)
+
         # Keyword arguments to pass to the forward method
         kwargs = {}
         if hasarg(self.model.forward, "epoch"):
             # Add `epoch` argument if forward accepts it
             kwargs["epoch"] = self.current_epoch
         if hasarg(self.model.forward, "step"):
             # Add `step` argument if forward accepts it
             kwargs["step"] = self.global_step
 
-        # Type not supported.
-        if not isinstance(input, (torch.Tensor, tuple, list, dict)):
-            logger.error(f"Input type '{type(input)}' not supported.")
-            sys.exit()
-
-        # Freeze the layers if specified so.
-        if self.freezer is not None:
-            self.freezer(self.model, self.global_step, self.current_epoch)
-
-        # Unpack Tuple or List. Only if num of args passed is less than or equal to num of args accepted.
-        if isinstance(input, (tuple, list)) and (len(input) + len(kwargs)) <= countargs(self.model):
-            return self.model(*input, **kwargs)
-        # Unpack Dict. Only if dict's keys match criterion's keyword arguments.
-        elif isinstance(input, dict) and all(hasarg(self.model, name) for name in input):
-            return self.model(**input, **kwargs)
-        # Tensor, Tuple, List, or Dict, as-is, not unpacked.
-        else:
-            return self.model(input, **kwargs)
+        return self.model(input, **kwargs)
 
     def _base_step(self, batch: Union[List, Tuple], batch_idx: int, mode: str) -> Union[Dict[str, Any], Any]:
         """Base step for all modes ("train", "val", "test", "predict")
 
         Args:
             batch (List, Tuple):
                 output of the DataLoader and input to the model.
@@ -205,16 +192,35 @@
         Returns:
             Union[Dict[str, Any], Any]: For the training, validation and test step, it returns
                 a dict containing loss, metrics, input, target, and pred. Loss will be `None`
                 for the test step. Metrics will be `None` if no metrics are specified.
 
                 For predict step, it returns pred only.
         """
-        # Split the batch into input and target. Target will be `None` if not provided.
-        input, target = self._split_batch(batch)
+        # Ensure that the batch is a list, a tuple, or a dict.
+        if not isinstance(batch, (list, tuple, dict)):
+            raise TypeError(
+                "A batch must be a list, a tuple, or a dict."
+                "A batch dict must have 'input' and 'target' as keys."
+                "A batch list or a tuple must have 2 elements - input and target."
+                "If target does not exist, return `None` as target."
+            )
+        # Ensure that a dict batch has input and target keys exclusively.
+        if isinstance(batch, dict) and set(batch.keys()) != {"input", "target"}:
+            raise ValueError("A batch must be a dict with 'input' and 'target' as keys.")
+        # Ensure that a list/tuple batch has 2 elements (input and target).
+        if len(batch) == 1:
+            raise ValueError(
+                "A batch must consist of 2 elements - input and target. If target does not exist, return `None` as target."
+            )
+        if len(batch) > 2:
+            raise ValueError(f"A batch must consist of 2 elements - input and target, but found {len(batch)} elements.")
+
+        # Split the batch into input and target.
+        input, target = batch if not isinstance(batch, dict) else (batch["input"], batch["target"])
 
         # Forward
         if self.inferer and mode in ["val", "test", "predict"]:
             pred = self.inferer(input, self)
         else:
             pred = self(input)
 
@@ -254,43 +260,29 @@
 
         Returns:
             torch.Tensor: the calculated loss.
         """
         # Keyword arguments to pass to the loss/criterion function
         kwargs = {}
         if hasarg(self.criterion.forward, "target"):
-            # Add `target` argument if forward accepts it. Casting performed if specified.
-            kwargs["target"] = target.to(self._cast_target_dtype_to)
+            # Add `target` argument if forward accepts it. Cast it if it is a tensor and if the target type is specified.
+            kwargs["target"] = target if not isinstance(target, torch.Tensor) else target.to(self._cast_target_dtype_to)
         else:
             if not self._target_not_used_reported and not self.trainer.sanity_checking:
                 self._target_not_used_reported = True
                 logger.info(
                     f"The criterion `{get_name(self.criterion, True)}` "
                     "has no `target` argument. In such cases, the LighterSystem "
                     "passes only the predicted values to the criterion. "
                     "This is intended as a support for self-supervised "
                     "losses where target is not used. If this is not the "
                     "behavior you expected, redefine your criterion "
                     "so that it has a `target` argument."
                 )
-
-        # Type not supported.
-        if not isinstance(pred, (torch.Tensor, tuple, list, dict)):
-            logger.error(f"Pred type '{type(pred)}' not supported.")
-            sys.exit()
-
-        # Unpack Tuple or List. Only if num of args passed is less than or equal to num of args accepted.
-        if isinstance(pred, (tuple, list)) and (len(pred) + len(kwargs)) <= countargs(self.criterion):
-            return self.criterion(*pred, **kwargs)
-        # Unpack Dict. Only if dict's keys match criterion's keyword arguments' names.
-        elif isinstance(pred, dict) and all(hasarg(self.criterion, name) for name in pred):
-            return self.criterion(**pred, **kwargs)
-        # Tensor, Tuple, List, or Dict, as-is, not unpacked.
-        else:
-            return self.criterion(pred, **kwargs)
+        return self.criterion(pred, **kwargs)
 
     def _base_dataloader(self, mode: str) -> DataLoader:
         """Instantiate the dataloader for a mode (train/val/test/predict).
         Includes a collate function that enables the DataLoader to replace
         None's (alias for corrupted examples) in the batch with valid examples.
         To make use of it, write a try-except in your Dataset that handles
         corrupted data by returning None instead.
@@ -315,15 +307,15 @@
         batch_size = self.batch_size
         if self.inferer is not None and mode in ["val", "test", "predict"]:
             logger.info(f"Setting the '{mode}' mode dataloader to batch size of 1 because an inferer is provided.")
             batch_size = 1
 
         # A dataset can return None when a corrupted example occurs. This collate
         # function replaces None's with valid examples from the dataset.
-        collate_fn = partial(collate_fn_replace_corrupted, dataset=dataset, default_collate_fn=collate_fn)
+        collate_fn = partial(collate_replace_corrupted, dataset=dataset, default_collate_fn=collate_fn)
         return DataLoader(
             dataset,
             sampler=sampler,
             shuffle=(mode == "train" and sampler is None),
             batch_size=batch_size,
             drop_last=self.drop_last_batch,
             num_workers=self.num_workers,
@@ -391,42 +383,14 @@
             self.test_step = partial(self._base_step, mode="test")
 
         # Predict methods.
         if stage == "predict":
             self.predict_dataloader = partial(self._base_dataloader, mode="predict")
             self.predict_step = partial(self._base_step, mode="predict")
 
-    def _split_batch(self, batch) -> Tuple[torch.Tensor, Optional[Any]]:
-        """Split the batch into input and target. Target will be `None` if not provided.
-
-        Args:
-            batch (List, Tuple): output of the DataLoader and input to the model.
-
-        Returns:
-            Tuple(torch.Tensor, Optional[Any]): input and target.
-        """
-        # Check if the batch format is correct.
-        if len(batch) > 2:
-            raise ValueError(
-                "Found more than 2 items in the batch. `LighterSystem` requires the dataloader to return either "
-                "input tensor(s) only, or a two-element tuple/list consisting of input tensor(s) and target(s)."
-            )
-
-        # Report the batch split type. Only on the first call.
-        if not self._batch_type_reported:
-            self._batch_type_reported = True
-            if len(batch) == 1:
-                logger.info("Target not provided. Using `None` as target. Ignore if intended.")
-            else:
-                logger.info("Using the first item as input and the second item as target.")
-
-        # Split the batch into input and target. Target will be `None` if not provided.
-        input, target = (batch, None) if len(batch) == 1 else batch
-        return input, target
-
     def _init_placeholders_for_dataloader_and_step_methods(self) -> None:
         """`LighterSystem` dynamically defines the `..._dataloader()`and `..._step()` methods
         in the `self.setup()` method. However, `LightningModule` excepts them to be defined at
         the initialization. To prevent it from throwing an error, the `..._dataloader()` and
         `..._step()` are initially defined as `lambda: None`, before `self.setup()` is called.
         """
         self.train_dataloader = self.training_step = lambda: None
```

### Comparing `project_lighter-0.0.2a1/lighter/utils/collate.py` & `project_lighter-0.0.2a2/lighter/utils/collate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 from typing import Any, Callable, List
 
 import random
 
 import torch
 from torch.utils.data import DataLoader
+from torch.utils.data._utils.collate import collate_str_fn, default_collate_fn_map
 from torch.utils.data.dataloader import default_collate
 
+# Collate support for None. Just as a string, None is not collated. Allows elements of the batch to be None.
+default_collate_fn_map.update({type(None): collate_str_fn})
 
-def collate_fn_replace_corrupted(batch: List[Any], dataset: DataLoader, default_collate_fn: Callable = None) -> torch.Tensor:
+
+def collate_replace_corrupted(batch: Any, dataset: DataLoader, default_collate_fn: Callable = None) -> Any:
     """Collate function that allows to replace corrupted examples in the batch.
     The dataloader should return `None` when that occurs.
     The `None`s in the batch are replaced with other, randomly-selected, examples.
 
     Args:
-        batch (List[Any]): batch from the DataLoader.
+        batch (Any): batch from the DataLoader.
         dataset (Dataset): dataset that the DataLoader is passing through. Needs to be fixed
             in place with functools.partial before passing it to DataLoader's 'collate_fn' option
             as 'collate_fn' should only have a single argument - batch. Example:
                 ```
-                collate_fn = functools.partial(collate_fn_replace_corrupted, dataset=dataset)`
+                collate_fn = functools.partial(collate_replace_corrupted, dataset=dataset)`
                 loader = DataLoader(dataset, ..., collate_fn=collate_fn).
                 ```
         default_collate_fn (Callable): the collate function to call once the batch has no corrupted examples.
             If `None`, `torch.utils.data.dataloader.default_collate` is called. Defaults to None.
     Returns:
-        torch.Tensor: batch with new examples instead of corrupted ones.
+        Any: batch with new examples instead of corrupted ones.
     """
     # Use `torch.utils.data.dataloader.default_collate` if no other default collate function is specified.
     default_collate_fn = default_collate_fn if default_collate_fn is not None else default_collate
     # Idea from https://stackoverflow.com/a/57882783
     original_batch_len = len(batch)
     # Filter out all the Nones (corrupted examples).
     batch = list(filter(lambda x: x is not None, batch))
     filtered_batch_len = len(batch)
     # Num of corrupted examples.
     num_corrupted = original_batch_len - filtered_batch_len
     if num_corrupted > 0:
         # Replace a corrupted example with another randomly selected example.
         batch.extend([dataset[random.randint(0, len(dataset) - 1)] for _ in range(num_corrupted)])
         # Recursive call to replace the replacements if they are corrupted.
-        return collate_fn_replace_corrupted(batch, dataset)
+        return collate_replace_corrupted(batch, dataset)
     # Finally, when the whole batch is fine, apply the default collate function.
     return default_collate_fn(batch)
```

### Comparing `project_lighter-0.0.2a1/lighter/utils/dynamic_imports.py` & `project_lighter-0.0.2a2/lighter/utils/dynamic_imports.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,16 +13,20 @@
     """Given the path to a module, import it, and name it as specified.
 
     Args:
         module_name (str): what to name the imported module.
         module_path (str): path to the module to load.
     """
     # Based on https://stackoverflow.com/a/41595552.
+
+    if module_name in sys.modules:
+        logger.error(f"{module_path} has already been imported as module: {module_name}")
+        sys.exit()
+
     module_path = Path(module_path).resolve() / "__init__.py"
-    print(module_path)
     if not module_path.is_file():
         logger.error(f"No `__init__.py` in `{module_path}`. Exiting.")
         sys.exit()
     spec = importlib.util.spec_from_file_location(module_name, str(module_path))
     module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(module)
     sys.modules[module_name] = module
```

### Comparing `project_lighter-0.0.2a1/lighter/utils/freezer.py` & `project_lighter-0.0.2a2/lighter/utils/freezer.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a1/lighter/utils/misc.py` & `project_lighter-0.0.2a2/lighter/utils/misc.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,26 +54,14 @@
         bool: `True` if the argument if the specified name exists.
     """
 
     args = inspect.signature(_callable).parameters.keys()
     return arg_name in args
 
 
-def countargs(_callable: Callable) -> bool:
-    """Count the number of arguments that a function, class, or method accepts.
-
-    Args:
-        callable (Callable): function, class, or method to inspect.
-
-    Returns:
-        int: number of arguments that it accepts.
-    """
-    return len(inspect.signature(_callable).parameters.keys())
-
-
 def get_name(_callable: Callable, include_module_name: bool = False) -> str:
     """Get the name of an object, class or function.
 
     Args:
         _callable (Callable): object, class or function.
         include_module_name (bool, optional): whether to include the name of the module from
             which it comes. Defaults to False.
```

### Comparing `project_lighter-0.0.2a1/lighter/utils/model.py` & `project_lighter-0.0.2a2/lighter/utils/model.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a1/pyproject.toml` & `project_lighter-0.0.2a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 lighter = "lighter.utils.cli:interface"
 
 [tool.poetry]
 name = "project-lighter"
-version = "0.0.2a1"
+version = "0.0.2a2"
 description = "YAML-based automated rapid prototyping framework for deep learning experiments"
 readme = "README.md"
 authors = ["Ibrahim Hadzic <ibrahimhadzic45@gmail.com>" ,
             "Suraj Pai <b.pai@maastrichtuniversity.nl>", 
             "Keno Bressem <kbressem@bwh.harvard.edu>"]
 license = "MIT"
 repository = "https://github.com/lighter/lighter"
```

### Comparing `project_lighter-0.0.2a1/PKG-INFO` & `project_lighter-0.0.2a2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project-lighter
-Version: 0.0.2a1
+Version: 0.0.2a2
 Summary: YAML-based automated rapid prototyping framework for deep learning experiments
 Home-page: https://github.com/lighter/lighter
 License: MIT
 Author: Ibrahim Hadzic
 Author-email: ibrahimhadzic45@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -12,19 +12,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: lightly (>=1.2.43,<2.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: monai-weekly (>=1.2.dev2305,<2.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: py (>=1.11.0,<2.0.0)
```

