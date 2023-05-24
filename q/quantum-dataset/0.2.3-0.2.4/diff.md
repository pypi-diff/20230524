# Comparing `tmp/quantum_dataset-0.2.3.tar.gz` & `tmp/quantum_dataset-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantum_dataset-0.2.3.tar", last modified: Tue Mar  8 23:24:06 2022, max compression
+gzip compressed data, was "quantum_dataset-0.2.4.tar", last modified: Wed May 24 08:56:16 2023, max compression
```

## Comparing `quantum_dataset-0.2.3.tar` & `quantum_dataset-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-03-08 23:24:06.178361 quantum_dataset-0.2.3/
--rw-rw-rw-   0        0        0     1545 2022-03-08 23:24:06.179363 quantum_dataset-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      623 2021-02-19 13:13:56.000000 quantum_dataset-0.2.3/README.md
--rw-rw-rw-   0        0        0      127 2022-03-08 18:46:20.000000 quantum_dataset-0.2.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2022-03-08 23:24:06.161360 quantum_dataset-0.2.3/quantum_dataset.egg-info/
--rw-rw-rw-   0        0        0     1545 2022-03-08 23:24:05.000000 quantum_dataset-0.2.3/quantum_dataset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      507 2022-03-08 23:24:05.000000 quantum_dataset-0.2.3/quantum_dataset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-08 23:24:05.000000 quantum_dataset-0.2.3/quantum_dataset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-03-11 15:57:43.000000 quantum_dataset-0.2.3/quantum_dataset.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       62 2022-03-08 23:24:05.000000 quantum_dataset-0.2.3/quantum_dataset.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-03-08 23:24:05.000000 quantum_dataset-0.2.3/quantum_dataset.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-03-08 23:24:06.174364 quantum_dataset-0.2.3/quantumdataset/
--rw-rw-rw-   0        0        0       70 2022-03-08 18:46:20.000000 quantum_dataset-0.2.3/quantumdataset/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-08 23:24:06.177359 quantum_dataset-0.2.3/quantumdataset/externals/
--rw-rw-rw-   0        0        0        0 2022-03-08 23:21:00.000000 quantum_dataset-0.2.3/quantumdataset/externals/__init__.py
--rw-rw-rw-   0        0        0    10655 2022-03-08 18:46:20.000000 quantum_dataset-0.2.3/quantumdataset/externals/serialization.py
--rw-rw-rw-   0        0        0    17678 2022-03-08 23:21:00.000000 quantum_dataset-0.2.3/quantumdataset/quantum_dataset.py
--rw-rw-rw-   0        0        0        0 2022-03-03 12:08:38.000000 quantum_dataset-0.2.3/quantumdataset/quantum_dataset2.py
--rw-rw-rw-   0        0        0       23 2022-03-08 23:21:21.000000 quantum_dataset-0.2.3/quantumdataset/version.py
--rw-rw-rw-   0        0        0     6806 2022-03-08 18:46:20.000000 quantum_dataset-0.2.3/quantumdataset/xarray_utils.py
--rw-rw-rw-   0        0        0      306 2022-03-08 23:24:06.188408 quantum_dataset-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1564 2022-03-08 23:21:27.000000 quantum_dataset-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 08:56:16.188442 quantum_dataset-0.2.4/
+-rw-rw-rw-   0        0        0     1257 2023-05-24 08:56:16.189468 quantum_dataset-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2022-03-11 22:34:39.000000 quantum_dataset-0.2.4/README.md
+-rw-rw-rw-   0        0        0      501 2023-05-24 08:29:46.000000 quantum_dataset-0.2.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-24 08:56:16.166736 quantum_dataset-0.2.4/quantum_dataset.egg-info/
+-rw-rw-rw-   0        0        0     1257 2023-05-24 08:56:15.000000 quantum_dataset-0.2.4/quantum_dataset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      542 2023-05-24 08:56:16.000000 quantum_dataset-0.2.4/quantum_dataset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 08:56:15.000000 quantum_dataset-0.2.4/quantum_dataset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-03-11 15:57:43.000000 quantum_dataset-0.2.4/quantum_dataset.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-05-24 08:56:15.000000 quantum_dataset-0.2.4/quantum_dataset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-24 08:56:15.000000 quantum_dataset-0.2.4/quantum_dataset.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 08:56:16.179277 quantum_dataset-0.2.4/quantumdataset/
+-rw-rw-rw-   0        0        0       80 2022-03-11 22:34:36.000000 quantum_dataset-0.2.4/quantumdataset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 08:56:16.184357 quantum_dataset-0.2.4/quantumdataset/externals/
+-rw-rw-rw-   0        0        0        0 2022-03-11 22:34:36.000000 quantum_dataset-0.2.4/quantumdataset/externals/__init__.py
+-rw-rw-rw-   0        0        0    21350 2023-05-24 08:46:49.000000 quantum_dataset-0.2.4/quantumdataset/externals/markup.py
+-rw-rw-rw-   0        0        0    10655 2022-03-11 22:34:36.000000 quantum_dataset-0.2.4/quantumdataset/externals/serialization.py
+-rw-rw-rw-   0        0        0    17568 2023-05-24 08:50:55.000000 quantum_dataset-0.2.4/quantumdataset/quantum_dataset.py
+-rw-rw-rw-   0        0        0        0 2022-03-03 12:08:38.000000 quantum_dataset-0.2.4/quantumdataset/quantum_dataset2.py
+-rw-rw-rw-   0        0        0       23 2023-05-24 08:55:06.000000 quantum_dataset-0.2.4/quantumdataset/version.py
+-rw-rw-rw-   0        0        0     6806 2022-03-11 22:34:36.000000 quantum_dataset-0.2.4/quantumdataset/xarray_utils.py
+-rw-rw-rw-   0        0        0      306 2023-05-24 08:56:16.199009 quantum_dataset-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2023-05-24 08:32:08.000000 quantum_dataset-0.2.4/setup.py
```

### Comparing `quantum_dataset-0.2.3/PKG-INFO` & `quantum_dataset-0.2.4/quantum_dataset.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 Metadata-Version: 2.1
-Name: quantum_dataset
-Version: 0.2.3
+Name: quantum-dataset
+Version: 0.2.4
 Summary: Collection of measurements on quantum devices
 Home-page: https://github.com/QuTech-Delft/quantum_dataset/
 Author: Pieter Eendebak
 Author-email: pieter.eendebak@tno.nl
 Maintainer: Pieter Eendebak
 Maintainer-email: pieter.eendebak@tno.nl
 License: MIT
-Description: # Quantum Dataset
-        
-        A collection of measurements on quantum devices.
-        
-        The data for the QuantumDataset is attached to the github releases. By default it retrieves the dataset from
-        
-        https://github.com/QuTech-Delft/quantum_dataset/releases/tag/Test
-        
-        ## Example usage
-        
-        ```
-        import qtt
-        from quantumdataset import QuantumDataset
-        quantum_dataset=QuantumDataset(datadir=r'd:\data\tmp\qd' )
-        quantum_dataset.list_tags()
-        
-        dataset = quantum_dataset.load_dataset('allxy', 0)
-        qtt.data.plot_dataset(dataset, fig = 1)
-        
-        
-        quantum_dataset.generate_overview_page(qtt.utilities.tools.mkdirc(r'd:\data\tmp\qd-overview'))
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
+
+# Quantum Dataset
+
+A collection of measurements on quantum devices.
+
+The data for the QuantumDataset is attached to the github release named `Test`, see
+https://github.com/QuTech-Delft/quantum_dataset/releases/tag/Test
+
+## Example usage
+
+```
+from quantumdataset import QuantumDataset
+quantum_dataset=QuantumDataset(data_directory=None)
+quantum_dataset.list_tags()
+
+dataset = quantum_dataset.load_dataset('allxy', 0)
+quantum_dataset.plot_dataset(dataset)
+
+quantum_dataset.generate_overview_page(quantum_dataset.data_directory / 'overview')
+```
+
+![](docs/anti_crossing.png)
```

### Comparing `quantum_dataset-0.2.3/quantumdataset/externals/serialization.py` & `quantum_dataset-0.2.4/quantumdataset/externals/serialization.py`

 * *Files identical despite different names*

### Comparing `quantum_dataset-0.2.3/quantumdataset/quantum_dataset.py` & `quantum_dataset-0.2.4/quantumdataset/quantum_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,33 +10,33 @@
 import json
 import logging
 import os
 import tempfile
 import uuid
 from io import BytesIO
 from pathlib import Path
-from typing import Any, Callable, List, Optional, Tuple, Union
+from typing import Any, Callable
 from urllib.request import urlopen
 from zipfile import ZipFile
 
 import matplotlib.pyplot as plt
+from matplotlib.backends.backend_svg import FigureCanvasSVG
+from matplotlib.figure import Figure
 import numpy as np
 import xarray as xr
-from MarkupPy import markup
-from MarkupPy.markup import oneliner as oneliner
+from quantumdataset.externals.markup import oneliner
+from quantumdataset.externals import markup
 
 try:
     import qcodes
 except ImportError:
     qcodes = None  # type: ignore
 from dataclasses import dataclass, field
 
 from dataclasses_json import dataclass_json
-from matplotlib.backends.backend_svg import FigureCanvasSVG
-from matplotlib.figure import Figure
 
 from quantumdataset.externals.serialization import Serializer
 from quantumdataset.xarray_utils import plot_xarray_dataset
 
 
 def print_dataset_non_gui(dataset: xr.Dataset, filename: str):
     """Plot a dataset and write to disk"""
@@ -44,45 +44,48 @@
     _ = FigureCanvasSVG(figure)
     ax = figure.subplots()
     plot_xarray_dataset(dataset, fig=ax)
     figure.canvas.print_figure(filename)
     return figure
 
 
-#%%
+# %%
 def install_quantum_dataset(location: str, version: str, overwrite: bool = False):
     """Install data on the specified location"""
     qdfile = os.path.join(location, "quantumdataset.txt")
     if os.path.exists(qdfile) and not overwrite:
-
         raise Exception(f"file {qdfile} exists, not overwriting dataset")
 
     zipurl = f"https://github.com/QuTech-Delft/quantum_dataset/releases/download/Test/QuantumDataset-{version}.zip"
 
     print(f"downloading Quantum Dataset from {zipurl} to {location}")
     with urlopen(zipurl) as zipresp:
         with ZipFile(BytesIO(zipresp.read())) as zfile:
             print("   extracting data...")
             zfile.extractall(location)
 
 
+def gen_uid() -> str:
+    return str(uuid.uuid4())
+
+
 @dataclass_json
 @dataclass
 class Metadata:
     tag: str
     name: str
-    uid: str
-    extra: dict = field(default_factory=dict)
+    uid: str = field(default_factory=gen_uid)
+    extra: dict[str, Any] = field(default_factory=dict)
 
 
 QUANTUM_DATASET_LOCATION = "QUANTUM_DATASET_LOCATION"
 
 
 class QuantumDataset:
-    def __init__(self, data_directory: Optional[str]):
+    def __init__(self, data_directory: str | None):
         """Create object to load and store quantum datasets
 
         Args:
             data_directory: directory with stored results. If None, then retrieve location from environment variable QUANTUM_DATASET_LOCATION
 
         """
         if data_directory is None:
@@ -99,21 +102,21 @@
         assert data_directory is not None
         self._header_css = '<style type="text/css">\n  body { font-family: Verdana, Geneva, sans-serif; }\n</style>\n'
         if self.check_quantum_dataset_installation(data_directory) is None:
             install_quantum_dataset(location=data_directory, version=str(self._version))
             if self.check_quantum_dataset_installation(location=data_directory) is None:
                 raise Exception(f"failed to install dataset at {data_directory}")
 
-    def database_metadata(self) -> List[Metadata]:
+    def database_metadata(self) -> list[Metadata]:
         """Return database metadata structure"""
         self._metadata = self.load_database_metadata()
         return self._metadata
 
     @staticmethod
-    def check_quantum_dataset_installation(location: str) -> Optional[str]:
+    def check_quantum_dataset_installation(location: str) -> str | None:
         """Return version of the Quantum DataSet installed
 
         Returns None if no data is installed
         """
         qdfile = os.path.join(location, "metadata.json")
         if not os.path.exists(qdfile):
             logging.info(f"could not find {qdfile}")
@@ -133,24 +136,24 @@
 
     def show_data(self):
         """List all data in the database"""
         for tag in self.list_tags():
             ll = self.list_subtags(tag)
             print("tag %s: %d results" % (tag, len(ll)))
 
-    def list_subtags(self, tag: str) -> List[str]:
+    def list_subtags(self, tag: str) -> list[str]:
         """List all subtags for the specified tag"""
         return sorted({m.name for m in self.database_metadata() if m.tag == tag})
 
     def plot_dataset(self, dataset, fig: int = 100):
         """Plot a dataset into a matplotlib figure window"""
         dataset = self.convert_dataset_to_xarray(dataset)
         plot_xarray_dataset(dataset, fig=fig)
 
-    def show(self, tag: str, fig: Union[int, plt.Figure]):
+    def show(self, tag: str, fig: int | plt.Figure):
         """Show all datasets for a specific tag"""
 
         names = self.list_subtags(tag)
         print("tag %s: %d result(s)" % (tag, len(names)))
 
         nx = int(np.ceil(np.sqrt(len(names))))
         ny = int(np.ceil(len(names) / nx))
@@ -173,17 +176,17 @@
                 plt.draw()
             except Exception as ex:
                 print(f"failed to plot {subtag} ({ex})")
 
     def generate_results_page(
         self,
         tag: str,
-        htmldir: Union[Path, str],
-        filename: Union[Path, str],
-        plot_function: Optional[Callable] = None,
+        htmldir: Path | str,
+        filename: Path | str,
+        plot_function: Callable | None = None,
         verbose: int = 1,
     ):
         """Generate a result page for a particular tag"""
 
         image_extension = "png"
         htmldir = Path(htmldir)
         assert isinstance(htmldir, Path)
@@ -247,34 +250,34 @@
             print_dataset_non_gui(dataset, str(imagefile))
             page.a(name="dataset%d" % ii)
             page.h3("Dataset: %s" % oneliner.a(meta.name, href=dataset_filename))
             page.a.close()
             page.img(src=imagefile0)
 
         if filename is not None:
-            with open(filename, "wt") as fid:
+            with open(filename, "w") as fid:
                 fid.write(str(page))
 
         return page
 
-    def generate_overview_page(self, htmldir: str, plot_functions: Optional[dict] = None) -> str:
+    def generate_overview_page(self, htmldir: str, plot_functions: dict | None = None) -> str:
         """Generate HTML page with overview of data in the database"""
         htmlpath = Path(htmldir)
         if plot_functions is None:
             plot_functions = {}
         for tag in self.list_tags():
             page_filename = htmlpath / f"qdataset-{tag}.html"
 
             plot_function = plot_functions.get(tag, None)
             page = self.generate_results_page(tag, htmlpath, page_filename, plot_function=plot_function)
 
         filename, page = self._generate_main_page(htmldir)
         return filename
 
-    def _generate_main_page(self, htmldir: str) -> Tuple[str, markup.page]:
+    def _generate_main_page(self, htmldir: str) -> tuple[str, markup.page]:
         """Generate overview page with results"""
 
         page = markup.page()
         page.init(
             title="Quantum Dataset",
             lang="en",
             header="<!-- Start of page -->\n" + self._header_css,
@@ -301,20 +304,20 @@
             link = oneliner.a("%s" % tag, href=link)
             subtags = self.list_subtags(tag)
             page.li(link + f": {len(subtags)} datasets")
         page.ol.close()
 
         if htmldir is not None:
             filename = os.path.join(htmldir, "index.html")
-            with (open(filename, "wt")) as fid:
+            with open(filename, "w") as fid:
                 fid.write(str(page))
 
         return filename, page
 
-    def convert_dataset_to_xarray(self, dataset: Union[xr.Dataset, dict]) -> xr.Dataset:
+    def convert_dataset_to_xarray(self, dataset: xr.Dataset | dict) -> xr.Dataset:
         """Convert dataset to internal dictionary format"""
         if isinstance(dataset, xr.Dataset):
             return dataset
 
         if qcodes is not None:
             from qcodes.data.data_set import DataSet
 
@@ -328,35 +331,34 @@
 
         else:
             raise TypeError(f"dataset is of type {type(dataset)}")
 
         assert isinstance(dataset, xr.Dataset)
         return dataset
 
-    def convert_dataset_to_dictionary(self, dataset: Union[xr.Dataset, dict]) -> dict:
+    def convert_dataset_to_dictionary(self, dataset: xr.Dataset | dict) -> dict:
         """Convert dataset to internal dictionary format"""
         return self.convert_dataset_to_xarray(dataset).to_dict()
 
     def get_metadata(self, *, uid=None, tag=None, subtag=None) -> Metadata:
-
         metadata = self.database_metadata()
         if uid is not None:
             uids = [m.uid for m in metadata]
             idx = uids.index(uid)
             return metadata[idx]
 
         data = [m for m in metadata if m.tag == tag and m.name == subtag]
         assert len(data) == 1
         return data[0]
 
-    def load_dataset(self, tag: Optional[str] = None, subtag: Union[str, int] = None) -> xr.Dataset:
+    def load_dataset(self, tag: str | None = None, subtag: str | int | None = None) -> xr.Dataset:
         """Load a dataset from the database"""
         if isinstance(subtag, int) and isinstance(tag, str):
             subtag = self.list_subtags(tag)[subtag]
-        assert isinstance(subtag, str)
+            assert isinstance(subtag, str)
 
         meta = self.get_metadata(tag=tag, subtag=subtag)
         filename = self._generate_dataset_filename(meta)
 
         with open(filename) as fid:
             encoded_data = json.load(fid)
 
@@ -375,40 +377,39 @@
         dataset = self.convert_dataset_to_xarray(dataset)
         dataset_dictionary = dataset.to_dict()
 
         filename = self._generate_dataset_filename(metadata)
 
         encoded_data = self.serializer.encode_data(dataset_dictionary)
 
-        with open(filename, "wt") as fid:
+        with open(filename, "w") as fid:
             json.dump(encoded_data, fid)
 
         mm = self.database_metadata()
         mm = mm + [metadata]
         self.save_database_metadata(mm)
         return filename
 
-    def list_tags(self) -> List[str]:
+    def list_tags(self) -> list[str]:
         """List all the tags currently in the database"""
         return sorted({m.tag for m in self.database_metadata()})
 
-    def load_database_metadata(self) -> List[Metadata]:
+    def load_database_metadata(self) -> list[Metadata]:
         with open(self.data_directory / "metadata.json") as fid:
             metadata = json.load(fid)
             return [Metadata.from_dict(m) for m in metadata]  # type: ignore
 
-    def save_database_metadata(self, metadata: List[Metadata]):
-        with open(self.data_directory / "metadata.json", "wt") as fid:
+    def save_database_metadata(self, metadata: list[Metadata]):
+        with open(self.data_directory / "metadata.json", "w") as fid:
             json.dump([m.to_dict() for m in metadata], fid)  # type: ignore
 
 
 if __name__ == "__main__":
     import xarray as xr
     from qtt.utilities.tools import measure_time
-    from sqt.utils.profiling import profile_expression
 
     from quantumdataset import QuantumDataset
 
     if 0:
         q = QuantumDataset(r"C:\data\QuantumDatasetOld")
         data = []
         for tag in q.list_tags():
@@ -428,16 +429,16 @@
             print(f"convert {d}")
             ds = q.load_dataset(*d)  # , output_format='Dataset')
             ds = ds.to_xarray()
             ds.attrs.pop("qcodes_location", None)
             ds.attrs.pop("metadata", None)
             # m = q.load_dataset(*d, output_format='dict')
 
-            # uid = gen_uid()
-            uid = str(uuid.uuid4())
+            uid = gen_uid()
+
             name = d[1].replace("\\", "_")
             m = Metadata(**{"tag": d[0], "name": name, "extra": {}, "uid": uid})
             # ds.attrs['tuid']=m.uid
             filename = q2.save_dataset(ds, m)
             metadata.append(m)
             if 0:
                 m = q.load_dataset(*d)
@@ -454,46 +455,43 @@
     q2.plot_dataset(ds, fig=1)
 
     from rich import print as rprint
 
     rprint(q2.database_metadata()[:3])
 
     if 1:
-
         tag = q2.list_tags()[0]
 
         q2.show(tag, fig=2)
 
         htmldir = q2.data_directory / "html"
         # htmldir.mkdir(exist_ok=True)
         with measure_time():
             filename = q2.generate_overview_page(str(htmldir))
 
         import webbrowser
 
         webbrowser.open(filename)
 
-#%% Resample a dataset
+# %% Resample a dataset
 if 0:
     d = ("elzerman_detuning_scan", "2019-09-07_21-58-05_qtt_vstack.json")
     # d=data[9]
 
     meta = q2.get_metadata(uid="4269d0d4-2ac4-4bb9-ac03-ce00be90fdae")
     d = (meta.tag, meta.name)
     # m = q2.load_dataset(meta.tag, meta.name)
     m = q.load_dataset(*d)
 
-    from qtt.dataset_processing import resample_dataset
-
-    #%%
+    # %%
     m2 = m.coarsen({"time": 4}).mean()
     # m2=resample_dataset(m, (2,))
     m2
     # q.save_dataset(m2, *d, overwrite=True)
     # q2.save_dataset(m2, meta, overwrite=True)
 
-    #%%
+    # %%
     from sqt.utils.plotting import plot_dataset
 
     plot_dataset(m2, fig=1)
 
     tag = "anticrossing"
```

### Comparing `quantum_dataset-0.2.3/quantumdataset/xarray_utils.py` & `quantum_dataset-0.2.4/quantumdataset/xarray_utils.py`

 * *Files identical despite different names*

### Comparing `quantum_dataset-0.2.3/setup.py` & `quantum_dataset-0.2.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,18 +34,17 @@
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/QuTech-Delft/quantum_dataset/",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering",
     ],
     license="MIT",
     packages=find_packages(),
-    install_requires=["numpy", "xarray", "matplotlib", "MarkupPy", "dataclasses", "dataclasses_json"],
+    install_requires=["numpy", "xarray", "matplotlib", "dataclasses_json"],
     tests_require=["pytest"],
     zip_safe=False,
 )
```

