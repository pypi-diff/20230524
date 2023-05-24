# Comparing `tmp/aroma-0.0.0a3.tar.gz` & `tmp/aroma-0.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aroma-0.0.0a3.tar", max compression
+gzip compressed data, was "aroma-0.0.0a7.tar", max compression
```

## Comparing `aroma-0.0.0a3.tar` & `aroma-0.0.0a7.tar`

### file list

```diff
@@ -1,10 +1,14 @@
--rw-r--r--   0        0        0     1501 2023-05-22 04:51:41.380201 aroma-0.0.0a3/LICENSE
--rw-r--r--   0        0        0     2077 2023-05-22 04:51:41.380201 aroma-0.0.0a3/README.md
--rw-r--r--   0        0        0     4447 2023-05-22 04:51:41.380201 aroma-0.0.0a3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-22 04:51:41.380201 aroma-0.0.0a3/src/aroma/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 04:51:41.380201 aroma-0.0.0a3/src/aroma/datasets/__init__.py
--rw-r--r--   0        0        0    19502 2023-05-22 04:51:41.384201 aroma-0.0.0a3/src/aroma/datasets/breakfast.py
--rw-r--r--   0        0        0        0 2023-05-22 04:51:41.384201 aroma-0.0.0a3/src/aroma/utils/__init__.py
--rw-r--r--   0        0        0      745 2023-05-22 04:51:41.384201 aroma-0.0.0a3/src/aroma/utils/imports.py
--rw-r--r--   0        0        0    11816 2023-05-22 04:51:41.384201 aroma-0.0.0a3/src/aroma/utils/vocab.py
--rw-r--r--   0        0        0     3425 1970-01-01 00:00:00.000000 aroma-0.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-05-24 05:51:32.230117 aroma-0.0.0a7/LICENSE
+-rw-r--r--   0        0        0     2077 2023-05-24 05:51:32.230117 aroma-0.0.0a7/README.md
+-rw-r--r--   0        0        0     4563 2023-05-24 05:51:32.230117 aroma-0.0.0a7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 05:51:32.230117 aroma-0.0.0a7/src/aroma/__init__.py
+-rw-r--r--   0        0        0      115 2023-05-24 05:51:32.230117 aroma-0.0.0a7/src/aroma/datasets/__init__.py
+-rw-r--r--   0        0        0    19662 2023-05-24 05:51:32.230117 aroma-0.0.0a7/src/aroma/datasets/breakfast.py
+-rw-r--r--   0        0        0      136 2023-05-24 05:51:32.230117 aroma-0.0.0a7/src/aroma/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3773 2023-05-24 05:51:32.230117 aroma-0.0.0a7/src/aroma/preprocessing/intertimes.py
+-rw-r--r--   0        0        0      265 2023-05-24 05:51:32.230117 aroma-0.0.0a7/src/aroma/testing.py
+-rw-r--r--   0        0        0        0 2023-05-24 05:51:32.230117 aroma-0.0.0a7/src/aroma/utils/__init__.py
+-rw-r--r--   0        0        0     1360 2023-05-24 05:51:32.230117 aroma-0.0.0a7/src/aroma/utils/download.py
+-rw-r--r--   0        0        0     1398 2023-05-24 05:51:32.230117 aroma-0.0.0a7/src/aroma/utils/imports.py
+-rw-r--r--   0        0        0    11816 2023-05-24 05:51:32.230117 aroma-0.0.0a7/src/aroma/utils/vocab.py
+-rw-r--r--   0        0        0     3476 1970-01-01 00:00:00.000000 aroma-0.0.0a7/PKG-INFO
```

### Comparing `aroma-0.0.0a3/LICENSE` & `aroma-0.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `aroma-0.0.0a3/README.md` & `aroma-0.0.0a7/README.md`

 * *Files identical despite different names*

### Comparing `aroma-0.0.0a3/pyproject.toml` & `aroma-0.0.0a7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aroma"
-version = "0.0.0a3"
+version = "0.0.0a7"
 description = "A library to prepare asynchronous time series datasets"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/aroma"
 repository = "https://github.com/durandtibo/aroma"
 keywords = ["dataset", "TPP", "asynchronous time series"]
 license = "BSD-3-Clause"
@@ -32,24 +32,28 @@
 # Core dependencies
 coola = "^0.0,>=0.0.7"
 gravitorch = "^0.0,>=0.0.11"
 numpy = "^1.24"
 python = "^3.9"
 redcat = "^0.0,>=0.0.3"
 torch = "^2.0"
+
+gdown = { version = "^4.7", optional = true }
 polars = { version = "^0.17", optional = true }
 
 [tool.poetry.extras]
 all = [
+    "gdown",
     "polars",
 ]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3"
 coverage = { extras = ["toml"], version = "^7.2" }
+docformatter = { extras = ["tomli"], version = "^1.7" }
 pre-commit = "^3.3"
 pylint = "^2.17"
 pytest = "^7.3"
 pytest-cov = "^4.0"
 pytest-timeout = "^2.1"
 ruff = "^0.0.269"
```

### Comparing `aroma-0.0.0a3/src/aroma/datasets/breakfast.py` & `aroma-0.0.0a7/src/aroma/datasets/breakfast.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,17 +23,17 @@
     "COOKING_ACTIVITIES",
     "DATASET_SPLITS",
     "DuplicateExampleRemoverIterDataPipe",
     "TxtAnnotationReaderIterDataPipe",
     "create_action_vocabulary",
     "filter_batch_by_dataset_split",
     "filter_examples_by_dataset_split",
-    "get_action_annotation_from_txt_file",
-    "get_event_data",
-    "get_event_examples",
+    "load_action_annotation",
+    "load_event_data",
+    "load_event_examples",
     "parse_action_annotation_lines",
     "remove_duplicate_examples",
 ]
 
 import logging
 from collections import Counter
 from collections.abc import Iterable, Iterator, Sequence
@@ -117,16 +117,16 @@
     "train1": sorted(PART2 + PART3 + PART4),
     "train2": sorted(PART1 + PART3 + PART4),
     "train3": sorted(PART1 + PART2 + PART4),
     "train4": sorted(PART1 + PART2 + PART3),
 }
 
 
-def get_event_data(path: Path, remove_duplicate: bool = True) -> tuple[BatchDict, dict]:
-    r"""Gets the event data and metadata for Breakfast.
+def load_event_data(path: Path, remove_duplicate: bool = True) -> tuple[BatchDict, dict]:
+    r"""Loads the event data and metadata for Breakfast.
 
     Args:
         path (``pathlib.Path``): Specifies the directory where the
             dataset annotations are stored.
         remove_duplicate (bool, optional): If ``True``, the duplicate
             examples are removed.
 
@@ -134,46 +134,46 @@
         tuple: A tuple with the data and metadata.
 
     Example usage:
 
     .. code-block:: python
 
         >>> from pathlib import Path
-        >>> from aroma.datasets.breakfast import get_event_data
+        >>> from aroma.datasets.breakfast import load_event_data
         # Dataset built with coarse annotations and without duplicate sequence events.
-        >>> data, metadata = get_event_data(Path('/path/to/data/breakfast/segmentation_coarse/'))
+        >>> data, metadata = load_event_data(Path('/path/to/data/breakfast/segmentation_coarse/'))
         >>> data.keys()
         dict_keys(['action_index', 'cooking_activity', 'end_time', 'person_id', 'start_time'])
         >>> data.batch_size
         508
         >>> metadata
         {'action_vocab': Vocabulary(
           counter=Counter({'SIL': 1016, 'pour_milk': 199, 'cut_fruit': 176, ..., 'stir_tea': 2}),
           index_to_token=('SIL', 'pour_milk', 'cut_fruit',..., 'stir_tea'),
           token_to_index={'SIL': 0, 'pour_milk': 1, 'cut_fruit': 2, ..., 'stir_tea': 47},
         )}
         # Dataset built with coarse annotations and with duplicate sequence events.
-        >>> data, metadata = get_event_data(
+        >>> data, metadata = load_event_data(
         ...     Path('/path/to/data/breakfast/segmentation_coarse/'),
         ...     remove_duplicate=False,
         ... )
         >>> data.batch_size
         1712
         # Dataset built with coarse annotations and without duplicate sequence events.
-        >>> data, metadata = get_event_data(Path('/path/to/data/breakfast/segmentation_fine/'))
+        >>> data, metadata = load_event_data(Path('/path/to/data/breakfast/segmentation_fine/'))
         >>> data.batch_size
         257
         >>> metadata
         {'action_vocab': Vocabulary(
           counter=Counter({'garbage': 774, 'move': 649, ..., 'carry_capSalt': 3}),
           index_to_token=('garbage', 'move', 'carry_knife', ..., 'carry_capSalt'),
           token_to_index={'garbage': 0, 'move': 1, 'carry_knife': 2, ..., 'carry_capSalt': 177},
         )}
     """
-    examples = get_event_examples(path=path, remove_duplicate=remove_duplicate)
+    examples = load_event_examples(path=path, remove_duplicate=remove_duplicate)
     action_vocab = create_action_vocabulary(examples)
     batch = convert_to_dict_of_lists(
         tuple(ActionIndexAdderIterDataPipe(SourceWrapper(examples), action_vocab))
     )
     return (
         BatchDict(
             {
@@ -190,16 +190,16 @@
                 ),
             }
         ),
         {Annotation.ACTION_VOCAB: action_vocab},
     )
 
 
-def get_event_examples(path: Path, remove_duplicate: bool = True) -> tuple[dict, ...]:
-    r"""Gets all the event-based examples.
+def load_event_examples(path: Path, remove_duplicate: bool = True) -> tuple[dict, ...]:
+    r"""Loads all the event-based examples.
 
     Args:
         path (``pathlib.Path``): Specifies the path where the
             annotations files are.
         remove_duplicate (bool, optional): If ``True``, the duplicate
             examples are removed.
 
@@ -209,16 +209,16 @@
             ``'end_time'``, ``'person_id'``, ``'start_time'``.
 
     Example usage:
 
     .. code-block:: python
 
         >>> from pathlib import Path
-        >>> from aroma.datasets.breakfast import get_event_examples
-        >>> examples = get_event_examples(Path("/path/to/data/breakfast/segmentation_coarse"))
+        >>> from aroma.datasets.breakfast import load_event_examples
+        >>> examples = load_event_examples(Path("/path/to/data/breakfast/segmentation_coarse"))
         >>> len(examples)
         508
         >>> examples[0]
         {'action': ('SIL',
           'take_bowl',
           'pour_cereals',
           'pour_milk',
@@ -235,21 +235,21 @@
                  [428.],
                  [575.],
                  [705.],
                  [836.]]),
          'person_id': 'P03',
          'cooking_activity': 'cereals'}
         # To keep duplicate examples
-        >>> examples = get_event_examples(
+        >>> examples = load_event_examples(
         ...     Path("/path/to/data/breakfast/segmentation_coarse"),
         ...     remove_duplicate=False,
         ... )
         >>> len(examples)
         1712
-        >>> examples = get_event_examples(Path("/path/to/data/breakfast/segmentation_fine"))
+        >>> examples = load_event_examples(Path("/path/to/data/breakfast/segmentation_fine"))
         >>> len(examples)
         257
         >>> examples[0]
         {'action': ('garbage',
           'reach_cabinet',
           'open_cabinet',
           'reach_bowl',
@@ -367,17 +367,17 @@
     Example usage:
 
     .. code-block:: python
 
         >>> from pathlib import Path
         >>> from aroma.datasets.breakfast import (
         ...     filter_batch_by_dataset_split,
-        ...     get_event_data,
+        ...     load_event_data,
         ... )
-        >>> data, metadata = get_event_data(Path('/path/to/data/breakfast/segmentation_coarse/'))
+        >>> data, metadata = load_event_data(Path('/path/to/data/breakfast/segmentation_coarse/'))
         >>> filter_batch_by_dataset_split(data, 'train1').batch_size
         386
         >>> filter_batch_by_dataset_split(data, 'test1').batch_size
         122
     """
     indices = []
     valid_person_ids = set(DATASET_SPLITS[split])
@@ -409,16 +409,16 @@
     for example in examples:
         if example[person_id_key] in valid_person_ids:
             filtered_examples.append(example)
     logger.info(f"Found {len(filtered_examples):,} examples for split `{split}`")
     return filtered_examples
 
 
-def get_action_annotation_from_txt_file(path: Path) -> dict:
-    r"""Gets action annotations from a text file.
+def load_action_annotation(path: Path) -> dict:
+    r"""Loads action annotations from a text file.
 
     Args:
         path (``pathlib.Path``): Specifies the file with the annotations.
 
     Returns:
         dict: A dictionary with the sequence of actions, the start
             time and end time of each action.
@@ -538,15 +538,15 @@
     """
 
     def __init__(self, datapipe: IterDataPipe[Path]) -> None:
         self._datapipe = datapipe
 
     def __iter__(self) -> Iterator[dict]:
         for path in self._datapipe:
-            yield get_action_annotation_from_txt_file(path)
+            yield load_action_annotation(path)
 
     def __len__(self) -> int:
         return len(self._datapipe)
 
     def __str__(self) -> str:
         return f"{self.__class__.__qualname__}(\n" f"  datapipe={str_indent(self._datapipe)},\n)"
 
@@ -599,10 +599,15 @@
 
 
 # if __name__ == "__main__":
 #     logging.basicConfig(level=logging.DEBUG)
 #
 #     annotation_path = Path("/Users/thibaut/Downloads/segmentation_coarse")
 #     # annotation_path = Path("/Users/thibaut/Downloads/segmentation_fine")
-#     batch, metadata = get_event_data(annotation_path)
+#     batch, metadata = load_event_data(annotation_path)
 #     print(batch)
 #     print(metadata)
+#
+#     from aroma.preprocessing import add_inter_times_
+#
+#     add_inter_times_(batch, time_key=Annotation.START_TIME, inter_times_key=Annotation.INTER_TIMES)
+#     print(batch)
```

### Comparing `aroma-0.0.0a3/src/aroma/utils/imports.py` & `aroma-0.0.0a7/src/aroma/utils/imports.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,7 +24,35 @@
 
 def is_polars_available() -> bool:
     r"""Indicates if the ``polars`` package is installed or not.
 
     https://www.pola.rs/
     """
     return find_spec("polars") is not None
+
+
+#################
+#     gdown
+##################
+
+
+def check_gdown() -> None:
+    r"""Checks if the ``gdown`` package is installed.
+
+    Raises
+    ------
+        RuntimeError if the ``gdown`` package is not installed.
+    """
+    if not is_gdown_available():
+        raise RuntimeError(
+            "`gdown` package is required but not installed. "
+            "You can install `gdown` package with the command:\n\n"
+            "pip install gdown\n"
+        )
+
+
+def is_gdown_available() -> bool:
+    r"""Indicates if the ``gdown`` package is installed or not.
+
+    https://github.com/wkentaro/gdown
+    """
+    return find_spec("gdown") is not None
```

### Comparing `aroma-0.0.0a3/src/aroma/utils/vocab.py` & `aroma-0.0.0a7/src/aroma/utils/vocab.py`

 * *Files identical despite different names*

### Comparing `aroma-0.0.0a3/PKG-INFO` & `aroma-0.0.0a7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aroma
-Version: 0.0.0a3
+Version: 0.0.0a7
 Summary: A library to prepare asynchronous time series datasets
 Home-page: https://github.com/durandtibo/aroma
 License: BSD-3-Clause
 Keywords: dataset,TPP,asynchronous time series
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: all
 Requires-Dist: coola (>=0.0.7,<0.1)
+Requires-Dist: gdown (>=4.7,<5.0) ; extra == "all"
 Requires-Dist: gravitorch (>=0.0.11,<0.1)
 Requires-Dist: numpy (>=1.24,<2.0)
 Requires-Dist: polars (>=0.17,<0.18) ; extra == "all"
 Requires-Dist: redcat (>=0.0.3,<0.1)
 Requires-Dist: torch (>=2.0,<3.0)
 Project-URL: Repository, https://github.com/durandtibo/aroma
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: aroma Version: 0.0.0a3 Summary: A library to
+Metadata-Version: 2.1 Name: aroma Version: 0.0.0a7 Summary: A library to
 prepare asynchronous time series datasets Home-page: https://github.com/
 durandtibo/aroma License: BSD-3-Clause Keywords: dataset,TPP,asynchronous time
 series Author: Thibaut Durand Author-email: durand.tibo+gh@gmail.com Requires-
 Python: >=3.9,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Information
 Technology Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
 Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Software Development :: Libraries
-Provides-Extra: all Requires-Dist: coola (>=0.0.7,<0.1) Requires-Dist:
-gravitorch (>=0.0.11,<0.1) Requires-Dist: numpy (>=1.24,<2.0) Requires-Dist:
-polars (>=0.17,<0.18) ; extra == "all" Requires-Dist: redcat (>=0.0.3,<0.1)
-Requires-Dist: torch (>=2.0,<3.0) Project-URL: Repository, https://github.com/
-durandtibo/aroma Description-Content-Type: text/markdown # aroma
+Provides-Extra: all Requires-Dist: coola (>=0.0.7,<0.1) Requires-Dist: gdown
+(>=4.7,<5.0) ; extra == "all" Requires-Dist: gravitorch (>=0.0.11,<0.1)
+Requires-Dist: numpy (>=1.24,<2.0) Requires-Dist: polars (>=0.17,<0.18) ; extra
+== "all" Requires-Dist: redcat (>=0.0.3,<0.1) Requires-Dist: torch (>=2.0,<3.0)
+Project-URL: Repository, https://github.com/durandtibo/aroma Description-
+Content-Type: text/markdown # aroma
           [CI] [CI] [Codecov] [https://api.codeclimate.com/v1/badges/
  14fed84cba9e0c2ad206/maintainability] [https://api.codeclimate.com/v1/badges/
                      14fed84cba9e0c2ad206/test_coverage]
 [PYPI_version] [Python] [BSD-3-Clause] [Code_style:_black] [Doc_style:_google]
                        [Downloads] [Monthly_downloads]
 ## Overview A python library to prepare asynchronous time series datasets
```

