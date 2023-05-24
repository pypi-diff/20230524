# Comparing `tmp/DBnomics-1.2.3.tar.gz` & `tmp/dbnomics-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DBnomics-1.2.3.tar", last modified: Wed May 25 15:09:46 2022, max compression
+gzip compressed data, was "dbnomics-1.2.4.tar", last modified: Wed May 24 15:27:22 2023, max compression
```

## Comparing `DBnomics-1.2.3.tar` & `dbnomics-1.2.4.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 15:09:46.631118 DBnomics-1.2.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 15:09:46.631118 DBnomics-1.2.3/DBnomics.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3054 2022-05-25 15:09:46.000000 DBnomics-1.2.3/DBnomics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      231 2022-05-25 15:09:46.000000 DBnomics-1.2.3/DBnomics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-25 15:09:46.000000 DBnomics-1.2.3/DBnomics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-05-25 15:09:46.000000 DBnomics-1.2.3/DBnomics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-05-25 15:09:46.000000 DBnomics-1.2.3/DBnomics.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    34461 2022-05-25 15:02:47.000000 DBnomics-1.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3054 2022-05-25 15:09:46.631118 DBnomics-1.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2331 2022-05-25 15:02:47.000000 DBnomics-1.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 15:09:46.631118 DBnomics-1.2.3/dbnomics/
--rw-rw-rw-   0 root         (0) root         (0)    22402 2022-05-25 15:02:47.000000 DBnomics-1.2.3/dbnomics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       31 2022-05-25 15:02:47.000000 DBnomics-1.2.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      506 2022-05-25 15:09:46.631118 DBnomics-1.2.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2788 2022-05-25 15:02:47.000000 DBnomics-1.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:27:22.196650 dbnomics-1.2.4/
+-rw-rw-rw-   0 root         (0) root         (0)    34461 2023-05-24 14:07:48.000000 dbnomics-1.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    42252 2023-05-24 15:27:22.196650 dbnomics-1.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1880 2023-05-24 14:07:48.000000 dbnomics-1.2.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2084 2023-05-24 14:07:48.000000 dbnomics-1.2.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-05-24 15:27:22.196650 dbnomics-1.2.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:27:22.192650 dbnomics-1.2.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:27:22.192650 dbnomics-1.2.4/src/dbnomics/
+-rw-rw-rw-   0 root         (0) root         (0)    22733 2023-05-24 14:07:48.000000 dbnomics-1.2.4/src/dbnomics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:27:22.196650 dbnomics-1.2.4/src/dbnomics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    42252 2023-05-24 15:27:22.000000 dbnomics-1.2.4/src/dbnomics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      267 2023-05-24 15:27:22.000000 dbnomics-1.2.4/src/dbnomics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 15:27:22.000000 dbnomics-1.2.4/src/dbnomics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-24 15:27:22.000000 dbnomics-1.2.4/src/dbnomics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-24 15:27:22.000000 dbnomics-1.2.4/src/dbnomics.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:27:22.196650 dbnomics-1.2.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2271 2023-05-24 14:07:48.000000 dbnomics-1.2.4/tests/test_client.py
```

### Comparing `DBnomics-1.2.3/LICENSE` & `dbnomics-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `DBnomics-1.2.3/README.md` & `dbnomics-1.2.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,80 @@
 # DBnomics Python client
 
-Access DBnomics time series from Python.
+Download time series from DBnomics and access it as a [Pandas](https://pandas.pydata.org/) DataFrame.
 
-This project relies on [Python Pandas](https://pandas.pydata.org/).
+This package is compatible with Python >= 3.8. (TODO vermin)
 
-## Tutorial
+## Documentation
 
-A tutorial is available as a [Jupyter notebook](./index.ipynb).
+### Quick start
 
-### Use with a proxy
+### Tutorial
 
-This Python package uses [requests](https://requests.readthedocs.io/), which is able to work with a proxy (HTTP/HTTPS, SOCKS). For more information, please check [its documentation](https://requests.readthedocs.io/en/master/user/advanced/#proxies).
+A tutorial showing how to download series as a DataFrame and plot them is available as a [notebook](https://git.nomics.world/dbnomics/dbnomics-python-client/-/blob/master/index.ipynb).
 
 ## Install
 
 ```bash
 pip install dbnomics
 ```
 
-See also: https://pypi.org/project/DBnomics/
+See also: <https://pypi.org/project/DBnomics/>
 
-## Development
+## Configuration
 
-To work on dbnomics-python-client source code:
+### Use with a proxy
 
-```bash
-git clone https://git.nomics.world/dbnomics/dbnomics-python-client.git
-cd dbnomics-python-client
-pip install -r requirements.txt
-pip install -r requirements-dev.txt
-pip install -e .
-```
+This Python package uses [requests](https://requests.readthedocs.io/), which is able to work with a proxy (HTTP/HTTPS, SOCKS). For more information, please check [its documentation](https://requests.readthedocs.io/en/master/user/advanced/#proxies).
+
+### Customize the API base URL
 
 If you plan to use a local Web API, running on the port 5000, you'll need to use the `api_base_url` parameter of the `fetch_*` functions, like this:
 
 ```python
-dataframe = fetch_series(
+df = fetch_series(
     api_base_url='http://localhost:5000',
     provider_code='AMECO',
     dataset_code='ZUTN',
 )
 ```
 
 Or globally change the default API URL used by the `dbnomics` module, like this:
 
 ```python
 import dbnomics
 dbnomics.default_api_base_url = "http://localhost:5000"
 ```
 
+## Development
+
+To work on dbnomics-python-client source code:
+
+```bash
+git clone https://git.nomics.world/dbnomics/dbnomics-python-client.git
+cd dbnomics-python-client
+pip install -r requirements.txt
+pip install -r requirements-dev.txt
+pip install -e .
+```
+
 ### Open the demo notebook
 
 Install jupyter if not already done, in a virtualenv:
 
 ```bash
 pip install jupyter
 jupyter notebook index.ipynb
 ```
 
 ## Tests
 
-Run tests:
-
 ```bash
-# Only once
 pip install -r requirements.txt
 pip install -r requirements-test.txt
 pip install -e .
 
 pytest
 
-# Specify an alterate API URL
+# Specify an alternate API URL
 API_URL=http://localhost:5000 pytest
 ```
-
-## Release
-
-To release a version on PyPI:
-
-- merge one or many feature branches into master (no need to do a release for every feature...)
-- update `setup.py` incrementing the package version (we use Semantic Versioning so determine if it's a major, minor or patch increment)
-- ensure the changelog is up to date
-- `git commit setup.py CHANGELOG.md -m "Release"`
-- create a Git tag with a `v` before version number and push it (`git tag v1.2.0; git push; git push --tags`)
-- the [CI](./.gitlab-ci.yml) will run a job to publish the package on PyPI at https://pypi.org/project/DBnomics/
-
-It's advised to do `pip install -e .` to let your virtualenv know about the new version number.
```

### Comparing `DBnomics-1.2.3/dbnomics/__init__.py` & `dbnomics-1.2.4/src/dbnomics/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,34 @@
-# dbnomics-python-client -- Access DBnomics time series from Python
-# By: Christophe Benz <christophe.benz@cepremap.org>
-#
-# Copyright (C) 2017-2019 Cepremap
-# https://git.nomics.world/dbnomics/dbnomics-python-client
-#
-# dbnomics-python-client is free software; you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# dbnomics-python-client is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-
-"""Access DBnomics time series from Python."""
-
+from __future__ import annotations
 
 import itertools
 import json
 import logging
 import os
 import urllib
 from collections import defaultdict
 from urllib.parse import urljoin
 
+import httpx
 import pandas as pd
-import requests
+from tenacity import RetryError, TryAgain, after_log, retry, stop_after_attempt, wait_random_exponential
 
 default_api_base_url = os.environ.get("API_URL") or "https://api.db.nomics.world/v22/"
 default_max_nb_series = 50
-
 default_editor_api_base_url = os.environ.get("EDITOR_API_URL") or "https://editor.nomics.world/api/v1/"
 editor_apply_endpoint_nb_series_per_post = 100
 
+default_timeout = 60
+
+
 log = logging.getLogger(__name__)
 
 
 class TooManySeries(Exception):
-    def __init__(self, num_found, max_nb_series):
+    def __init__(self, num_found, max_nb_series) -> None:
         self.num_found = num_found
         self.max_nb_series = max_nb_series
         message = (
             "DBnomics Web API found {num_found} series matching your request, "
             + (
                 "but you passed the argument 'max_nb_series={max_nb_series}'."
                 if max_nb_series is not None
@@ -68,14 +50,15 @@
     series_code=None,
     dimensions=None,
     series_ids=None,
     max_nb_series=None,
     api_base_url=None,
     editor_api_base_url=default_editor_api_base_url,
     filters=None,
+    timeout=None,
 ):
     """Download time series from DBnomics. Filter series by different ways according to the given parameters.
 
     If not `None`, `dimensions` parameter must be a `dict` of dimensions (`list` of `str`), like so:
     `{"freq": ["A", "M"], "country": ["FR"]}`.
 
     If not `None`, `series_code` must be a `str`. It can be a series code (one series), or a "mask" (many series):
@@ -91,16 +74,16 @@
     If `max_nb_series` is `None`, a default value of 50 series will be used.
 
     If `filters` is not `None`, apply those filters using the Time Series Editor API
     (Cf https://editor.nomics.world/filters)
 
     Return a Python Pandas `DataFrame`.
 
-    Examples:
-
+    Examples
+    --------
     - fetch one series:
       fetch_series("AMECO/ZUTN/EA19.1.0.0.0.ZUTN")
 
     - fetch all the series of a dataset:
       fetch_series("AMECO", "ZUTN")
 
     - fetch many series from different datasets:
@@ -117,110 +100,126 @@
     - fetch one series and apply interpolation filter:
       fetch_series(
           'AMECO/ZUTN/EA19.1.0.0.0.ZUTN',
           filters=[{"code": "interpolate", "parameters": {"frequency": "monthly", "method": "spline"}}],
       )
     """
     # Parameters validation
-    global default_api_base_url
     if api_base_url is None:
         api_base_url = default_api_base_url
     if not api_base_url.endswith("/"):
         api_base_url += "/"
     if dataset_code is None:
         if isinstance(provider_code, list):
             series_ids = provider_code
             provider_code = None
         elif isinstance(provider_code, str):
             series_ids = [provider_code]
             provider_code = None
 
     if provider_code is not None and not isinstance(provider_code, str):
-        raise ValueError("`provider_code` parameter must be a string")
+        msg = "`provider_code` parameter must be a string"
+        raise ValueError(msg)
     if dataset_code is not None and not isinstance(dataset_code, str):
-        raise ValueError("`dataset_code` parameter must be a string")
+        msg = "`dataset_code` parameter must be a string"
+        raise ValueError(msg)
     if dimensions is not None and not isinstance(dimensions, dict):
-        raise ValueError("`dimensions` parameter must be a dict")
+        msg = "`dimensions` parameter must be a dict"
+        raise ValueError(msg)
     if series_code is not None and not isinstance(series_code, str):
-        raise ValueError("`series_code` parameter must be a string")
+        msg = "`series_code` parameter must be a string"
+        raise ValueError(msg)
     if series_ids is not None and (
         not isinstance(series_ids, list) or any(not isinstance(series_id, str) for series_id in series_ids)
     ):
-        raise ValueError("`series_ids` parameter must be a list of strings")
+        msg = "`series_ids` parameter must be a list of strings"
+        raise ValueError(msg)
     if api_base_url is not None and not isinstance(api_base_url, str):
-        raise ValueError("`api_base_url` parameter must be a string")
+        msg = "`api_base_url` parameter must be a string"
+        raise ValueError(msg)
 
     series_base_url = urljoin(api_base_url, "series")
 
     if dimensions is None and series_code is None and series_ids is None:
         if not provider_code or not dataset_code:
-            raise ValueError("When you don't use `dimensions`, you must specifiy `provider_code` and `dataset_code`.")
-        api_link = series_base_url + "/{}/{}?observations=1".format(provider_code, dataset_code)
+            msg = "When you don't use `dimensions`, you must specifiy `provider_code` and `dataset_code`."
+            raise ValueError(msg)
+        api_link = series_base_url + f"/{provider_code}/{dataset_code}?observations=1"
         return fetch_series_by_api_link(
             api_link,
             filters=filters,
             max_nb_series=max_nb_series,
             editor_api_base_url=editor_api_base_url,
+            timeout=timeout,
         )
 
     if dimensions is not None:
         if not provider_code or not dataset_code:
-            raise ValueError("When you use `dimensions`, you must specifiy `provider_code` and `dataset_code`.")
+            msg = "When you use `dimensions`, you must specifiy `provider_code` and `dataset_code`."
+            raise ValueError(msg)
         api_link = series_base_url + "/{}/{}?observations=1&dimensions={}".format(
             provider_code, dataset_code, json.dumps(dimensions)
         )
         return fetch_series_by_api_link(
             api_link,
             filters=filters,
             max_nb_series=max_nb_series,
             editor_api_base_url=editor_api_base_url,
+            timeout=timeout,
         )
 
     if series_code is not None:
         if not provider_code or not dataset_code:
-            raise ValueError("When you use `series_code`, you must specifiy `provider_code` and `dataset_code`.")
-        api_link = series_base_url + "/{}/{}/{}?observations=1".format(provider_code, dataset_code, series_code)
+            msg = "When you use `series_code`, you must specifiy `provider_code` and `dataset_code`."
+            raise ValueError(msg)
+        api_link = series_base_url + f"/{provider_code}/{dataset_code}/{series_code}?observations=1"
         return fetch_series_by_api_link(
             api_link,
             filters=filters,
             max_nb_series=max_nb_series,
             editor_api_base_url=editor_api_base_url,
+            timeout=timeout,
         )
 
     if series_ids is not None:
         if provider_code or dataset_code:
-            raise ValueError("When you use `series_ids`, you must not specifiy `provider_code` nor `dataset_code`.")
+            msg = "When you use `series_ids`, you must not specifiy `provider_code` nor `dataset_code`."
+            raise ValueError(msg)
         api_link = series_base_url + "?observations=1&series_ids={}".format(
             ",".join(map(urllib.parse.quote, series_ids))
         )
         return fetch_series_by_api_link(
             api_link,
             filters=filters,
             max_nb_series=max_nb_series,
             editor_api_base_url=editor_api_base_url,
+            timeout=timeout,
         )
 
-    raise ValueError("Invalid combination of function arguments")
+    msg = "Invalid combination of function arguments"
+    raise ValueError(msg)
 
 
 def fetch_series_by_api_link(
     api_link,
     max_nb_series=None,
     editor_api_base_url=default_editor_api_base_url,
     filters=None,
+    timeout=None,
 ):
     """Fetch series given an "API link" URL.
 
     "API link" URLs can be found on DBnomics web site (https://db.nomics.world/) on dataset or series pages
     using "Download" buttons.
 
     If `filters` is not `None`, apply those filters using the Time Series Editor API
     (Cf https://editor.nomics.world/filters)
 
     Example:
+    -------
       fetch_series(api_link="https://api.db.nomics.world/v22/series?provider_code=AMECO&dataset_code=ZUTN")
     """
     # Call API via `iter_series_infos`, add dimensions labels and store result in `series_list`.
     # Fill `datasets_dimensions`
     datasets_dimensions = None
     series_dims_by_dataset_code = defaultdict(dict)
     # series_dims_by_dataset_code example:
@@ -229,15 +228,15 @@
     #            'EA19.1.0.0.0.ZUTN': { 'freq':'a', 'geo':'ea19', 'unit':'percentage-of-active-population'},
     #            'EA20.1.0.0.0.ZUTN': { 'freq':'a', 'geo':'ea20', 'unit':'percentage-of-active-population'},
     #            ...
     #        },
     #        ...
     #    }
     series_list = []
-    for series_infos in iter_series_infos(api_link, max_nb_series=max_nb_series):
+    for series_infos in iter_series_infos(api_link, max_nb_series=max_nb_series, timeout=timeout):
         complete_dataset_code = (
             series_infos["series"]["provider_code"] + "/" + series_infos["series"]["dataset_code"]
         )  # ex 'AMECO/ZUTN'
         if datasets_dimensions is None:
             # Let see if there's only one dataset returned by API, or many datasets
             datasets_dimensions = (
                 series_infos["datasets_dimensions"]
@@ -277,15 +276,15 @@
         # Add dimensions labels to flat_series
         complete_dataset_code = flat_series["provider_code"] + "/" + flat_series["dataset_code"]  # ex: "AMECO/ZUTN"
         dataset_dimensions = datasets_dimensions[complete_dataset_code]
         if "dimensions_labels" in dataset_dimensions:
             dataset_dimensions_labels = dataset_dimensions["dimensions_labels"]
         else:
             dataset_dimensions_labels = {
-                dim_code: "{} (label)".format(dim_code) for dim_code in dataset_dimensions["dimensions_codes_order"]
+                dim_code: f"{dim_code} (label)" for dim_code in dataset_dimensions["dimensions_codes_order"]
             }
         # Add dimensions values labels to current series
         if "dimensions_values_labels" in dataset_dimensions:
             for dimension_code in series.get("dimensions", {}):
                 dimension_label = dataset_dimensions_labels[dimension_code]
                 dimension_value_code = series_dims_by_dataset_code[complete_dataset_code][series["series_code"]][
                     dimension_code
@@ -301,102 +300,110 @@
         common_columns.append("filtered")
         filtered_series_list = [
             {**series, "filtered": True}
             for series in filter_series(
                 series_list=series_list,
                 filters=filters,
                 editor_api_base_url=editor_api_base_url,
+                timeout=timeout,
             )
         ]
         flat_series_list = [{**series, "filtered": False} for series in flat_series_list] + filtered_series_list
 
     # Compute dimensions_labels_columns_names and dimensions_codes_columns_names
     dimensions_labels_columns_names = []
     dimensions_codes_columns_names = []
-    for complete_dataset_code in datasets_dimensions.keys():
+    for complete_dataset_code in datasets_dimensions:
         for dimension_code in datasets_dimensions[complete_dataset_code]["dimensions_codes_order"]:
             dimensions_codes_columns_names.append(dimension_code)
             # We only add dimensions labels column if this information is present
             if "dimensions_labels" in dataset_dimensions and "dimensions_values_labels" in dataset_dimensions:
                 dimensions_labels_columns_names.append(
                     datasets_dimensions[complete_dataset_code]["dimensions_labels"][dimension_code]
                 )
             else:
-                if "dimensions_values_labels" in dataset_dimensions:
+                if "dimensions_values_labels" in dataset_dimensions:  # noqa: PLR5501
                     # No dimensions labels but dimensions_values_labels -> we add " (label)" to the end
                     # of dimension code
-                    dimensions_labels_columns_names.append("{} (label)".format(dimension_code))
+                    dimensions_labels_columns_names.append(f"{dimension_code} (label)")
                 # In the case there's no dimension_label nor dimensions_values_labels, we do not add any column
 
     # In the DataFrame we want to display the dimension columns at the right so we reorder them.
     ordered_columns_names = common_columns + dimensions_codes_columns_names + dimensions_labels_columns_names
 
     # Build dataframe
     dataframes = (pd.DataFrame(data=series, columns=ordered_columns_names) for series in flat_series_list)
     return pd.concat(objs=dataframes, sort=False)
 
 
-def fetch_series_page(series_endpoint_url, offset):
+def fetch_series_page(series_endpoint_url, offset, timeout=None):
     series_page_url = "{}{}offset={}".format(
         series_endpoint_url,
         "&" if "?" in series_endpoint_url else "?",
         offset,
     )
 
-    response = requests.get(series_page_url)
+    try:
+        response = _fetch_response(series_page_url, timeout=timeout)
+    except RetryError as exc:
+        raise FetchError(url=series_page_url) from exc
+
     response_json = response.json()
-    if not response.ok:
-        message = response_json.get("message")
-        raise ValueError("Could not fetch data from URL {!r} because: {}".format(series_page_url, message))
 
     series_page = response_json.get("series")
     if series_page is not None:
         assert series_page["offset"] == offset, (series_page["offset"], offset)
 
     return response_json
 
 
-def filter_series(series_list, filters, editor_api_base_url=default_editor_api_base_url):
+def filter_series(series_list, filters, editor_api_base_url=default_editor_api_base_url, timeout=None):
     if not editor_api_base_url.endswith("/"):
         editor_api_base_url += "/"
     apply_endpoint_url = urljoin(editor_api_base_url, "apply")
-    return list(iter_filtered_series(series_list, filters, apply_endpoint_url))
+    return list(iter_filtered_series(series_list, filters, apply_endpoint_url, timeout=timeout))
+
 
+def iter_filtered_series(series_list, filters, apply_endpoint_url, timeout=None):
+    if timeout is None:
+        timeout = default_timeout
 
-def iter_filtered_series(series_list, filters, apply_endpoint_url):
     for series_group in grouper(editor_apply_endpoint_nb_series_per_post, series_list):
         # Keep only keys required by the editor API.
         posted_series_list = [
             {
                 "frequency": series["@frequency"],
                 "period_start_day": series["period_start_day"],
                 "value": series["value"],
             }
             for series in series_group
         ]
-        response = requests.post(apply_endpoint_url, json={"filters": filters, "series": posted_series_list})
+        response = httpx.post(
+            apply_endpoint_url, json={"filters": filters, "series": posted_series_list}, timeout=timeout
+        )
         try:
             response_json = response.json()
         except ValueError:
-            log.error("Invalid response from Time Series Editor (JSON expected)")
+            log.error("Invalid response from Time Series Editor (JSON expected)")  # noqa: TRY400
             continue
-        if not response.ok:
+        if not response.is_success:
             log.error("Error with series filters: %s", json.dumps(response_json, indent=2))
             continue
 
         filter_results = response_json.get("filter_results")
         if not filter_results:
             continue
 
         for dbnomics_series, filter_result in zip(series_group, filter_results):
             yield flatten_editor_series(series=filter_result["series"], dbnomics_series=dbnomics_series)
 
 
-def iter_series_infos(api_link, max_nb_series=None):
-    """Iterate through series.docs returned by API
+def iter_series_infos(api_link, max_nb_series=None, timeout=None):
+    """Iterate through series.docs returned by API.
+
     Returns dicts of dataset(s) dimensions and series.
     The answer can have a key 'dataset_dimensions' if only one dataset is returned by API, or 'datasets_dimensions' if
     more than one dataset is returned.
      - datasets_dimensions or dataset_dimensions don't change between calls
      - series is the current series
     Example:
     {
@@ -410,37 +417,37 @@
            "CEPII/CHELEM-TRADE-GTAP": {
                "code": "CHELEM-TRADE-GTAP",
                "converted_at": "2019-01-29T15:53:30Z",
                "dimensions_codes_order": ["exporter", "importer", "secgroup", ...],
                ...
            },
       'series':
-    }
+    }.
     """
 
     def yield_series(series, response_json):
-        """Handle the cases of one-dataset and multi-datasets answer from API"""
+        """Handle the cases of one-dataset and multi-datasets answer from API."""
         assert "datasets" in response_json or "dataset" in response_json
         if "datasets" in response_json:
             # Multi-datasets answer
             datasets_dimensions_dict = {"datasets_dimensions": response_json["datasets"]}
         else:
             # Mono-dataset answer
             datasets_dimensions_dict = {"dataset_dimensions": response_json["dataset"]}
         yield {"series": series, **datasets_dimensions_dict}
 
     total_nb_series = 0
 
     while True:
-        response_json = fetch_series_page(api_link, offset=total_nb_series)
+        response_json = fetch_series_page(api_link, offset=total_nb_series, timeout=timeout)
 
         errors = response_json.get("errors")
         if errors:
             for error in errors:
-                log.error("{}: {}".format(error["message"], error))
+                log.error("%s: %s", error["message"], error)
 
         series_page = response_json["series"]
 
         num_found = series_page["num_found"]
         if max_nb_series is None and num_found > default_max_nb_series:
             raise TooManySeries(num_found, max_nb_series)
 
@@ -510,32 +517,32 @@
         "dataset_code": dbnomics_series["dataset_code"],
         "dataset_name": dbnomics_series.get("dataset_name"),
         "series_code": "{}_filtered".format(dbnomics_series["series_code"]),
     }
 
     series_name = dbnomics_series.get("series_name")
     if series_name:
-        series["series_name"] = "{} (filtered)".format(series_name)
+        series["series_name"] = f"{series_name} (filtered)"
 
     return series
 
 
 def normalize_period(series):
-    """Keep original period and convert str to datetime. Modifies `series`"""
+    """Keep original period and convert str to datetime. Modifies `series`."""
     period = series.get("period") or []
     period_start_day = series.get("period_start_day") or []
     return {
         **without_keys(series, keys={"period_start_day"}),
         "original_period": period,
         "period": list(map(pd.to_datetime, period_start_day)),
     }
 
 
 def normalize_value(series):
-    """Keep original value and convert "NA" to None (or user specified value). Modifies `series`"""
+    """Keep original value and convert "NA" to None (or user specified value). Modifies `series`."""
     value = series.get("value") or []
     return {
         **series,
         "original_value": value,
         "value": [
             # None will be replaced by np.NaN in DataFrame construction.
             None if v == "NA" else v
@@ -543,16 +550,42 @@
         ],
     }
 
 
 # UTILS
 
 
+class FetchError(Exception):
+    def __init__(self, *, url: str) -> None:
+        msg = f"Could not fetch data from URL {url!r}"
+        super().__init__(msg)
+        self.url = url
+
+
+@retry(
+    after=after_log(log, logging.ERROR),
+    stop=stop_after_attempt(3),
+    wait=wait_random_exponential(max=60),
+)
+def _fetch_response(url, timeout=None):
+    if timeout is None:
+        timeout = default_timeout
+
+    response = httpx.get(url, timeout=timeout)
+
+    if response.status_code in {429, 500, 502, 503, 504}:
+        raise TryAgain
+
+    response.raise_for_status()
+
+    return response
+
+
 def grouper(n, iterable):
-    """From https://stackoverflow.com/a/31185097/3548266
+    """From https://stackoverflow.com/a/31185097/3548266.
 
     >>> list(grouper(3, 'ABCDEFG'))
     [['A', 'B', 'C'], ['D', 'E', 'F'], ['G']]
     """
     iterable = iter(iterable)
     return iter(lambda: list(itertools.islice(iterable, n)), [])
```

