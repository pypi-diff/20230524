# Comparing `tmp/dapla_toolbelt_pseudo-0.2.3.tar.gz` & `tmp/dapla_toolbelt_pseudo-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_toolbelt_pseudo-0.2.3.tar", max compression
+gzip compressed data, was "dapla_toolbelt_pseudo-0.2.4.tar", max compression
```

## Comparing `dapla_toolbelt_pseudo-0.2.3.tar` & `dapla_toolbelt_pseudo-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1077 2023-03-22 21:55:01.981546 dapla_toolbelt_pseudo-0.2.3/LICENSE
--rw-r--r--   0        0        0     4899 2023-03-22 21:55:01.981546 dapla_toolbelt_pseudo-0.2.3/README.md
--rw-r--r--   0        0        0     2396 2023-03-22 21:55:14.393862 dapla_toolbelt_pseudo-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      947 2023-03-22 21:55:01.985547 dapla_toolbelt_pseudo-0.2.3/src/dapla_pseudo/__init__.py
--rw-r--r--   0        0        0      683 2023-03-22 21:55:01.985547 dapla_toolbelt_pseudo-0.2.3/src/dapla_pseudo/constants.py
--rw-r--r--   0        0        0      833 2023-03-22 21:55:01.985547 dapla_toolbelt_pseudo-0.2.3/src/dapla_pseudo/models.py
--rw-r--r--   0        0        0        0 2023-03-22 21:55:01.985547 dapla_toolbelt_pseudo-0.2.3/src/dapla_pseudo/py.typed
--rw-r--r--   0        0        0      404 2023-03-22 21:55:01.985547 dapla_toolbelt_pseudo-0.2.3/src/dapla_pseudo/types.py
--rw-r--r--   0        0        0      888 2023-03-22 21:55:01.985547 dapla_toolbelt_pseudo-0.2.3/src/dapla_pseudo/utils.py
--rw-r--r--   0        0        0      316 2023-03-22 21:55:01.985547 dapla_toolbelt_pseudo-0.2.3/src/dapla_pseudo/v1/__init__.py
--rw-r--r--   0        0        0    11182 2023-03-22 21:55:01.985547 dapla_toolbelt_pseudo-0.2.3/src/dapla_pseudo/v1/client.py
--rw-r--r--   0        0        0     4756 2023-03-22 21:55:01.985547 dapla_toolbelt_pseudo-0.2.3/src/dapla_pseudo/v1/models.py
--rw-r--r--   0        0        0    11269 2023-03-22 21:55:01.985547 dapla_toolbelt_pseudo-0.2.3/src/dapla_pseudo/v1/ops.py
--rw-r--r--   0        0        0     6007 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-0.2.3/setup.py
--rw-r--r--   0        0        0     6040 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-24 13:07:01.913619 dapla_toolbelt_pseudo-0.2.4/LICENSE
+-rw-r--r--   0        0        0     4899 2023-05-24 13:07:01.913619 dapla_toolbelt_pseudo-0.2.4/README.md
+-rw-r--r--   0        0        0     2417 2023-05-24 13:07:12.897626 dapla_toolbelt_pseudo-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1147 2023-05-24 13:07:12.897626 dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/__init__.py
+-rw-r--r--   0        0        0      657 2023-05-24 13:07:01.917619 dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/constants.py
+-rw-r--r--   0        0        0      833 2023-05-24 13:07:01.917619 dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/models.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:07:01.917619 dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/py.typed
+-rw-r--r--   0        0        0      407 2023-05-24 13:07:01.917619 dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/types.py
+-rw-r--r--   0        0        0      888 2023-05-24 13:07:01.917619 dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/utils.py
+-rw-r--r--   0        0        0      316 2023-05-24 13:07:01.917619 dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/v1/__init__.py
+-rw-r--r--   0        0        0    11182 2023-05-24 13:07:01.917619 dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/v1/client.py
+-rw-r--r--   0        0        0     4756 2023-05-24 13:07:01.917619 dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/v1/models.py
+-rw-r--r--   0        0        0    12294 2023-05-24 13:07:01.917619 dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/v1/ops.py
+-rw-r--r--   0        0        0     6007 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-0.2.4/setup.py
+-rw-r--r--   0        0        0     6040 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-0.2.4/PKG-INFO
```

### Comparing `dapla_toolbelt_pseudo-0.2.3/LICENSE` & `dapla_toolbelt_pseudo-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.3/README.md` & `dapla_toolbelt_pseudo-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.3/pyproject.toml` & `dapla_toolbelt_pseudo-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-toolbelt-pseudo"
-version = "0.2.3"
+version = "0.2.4"
 description = "Pseudonymization extensions for Dapla Toolbelt"
 authors = ["Team Skyinfrastruktur <dapla@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 repository = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 documentation = "https://statisticsnorway.github.io/dapla-toolbelt-pseudo"
@@ -38,15 +38,15 @@
 flake8-bandit = ">=2.1.2"
 flake8-bugbear = ">=21.9.2"
 flake8-docstrings = ">=1.6.0"
 flake8-rst-docstrings = ">=0.2.5"
 furo = ">=2021.11.12"
 isort = ">=5.10.1"
 mock = "^4.0.3"
-mypy = "^0.991"
+mypy = ">=1.1.1"
 myst-parser = {version = ">=0.16.1"}
 pep8-naming = ">=0.12.1"
 pre-commit = ">=2.16.0"
 pre-commit-hooks = ">=4.1.0"
 pytest = ">=6.2.5"
 pyupgrade = ">=2.29.1"
 responses = "^0.22.0"
@@ -57,14 +57,15 @@
 sqlalchemy = ">=2.0.0rc1"
 typeguard = ">=2.13.3"
 types-mock = "^4.0.15.2"
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
 ipykernel = "^6.21.3"
 pandas-stubs = "^1.5.3.230304"
 nbstripout = "^0.6.1"
+ipython = "^8.11.0"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
 branch = true
```

### Comparing `dapla_toolbelt_pseudo-0.2.3/src/dapla_pseudo/__init__.py` & `dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,21 @@
 from dapla_pseudo import pseudonymize
 (which would resolve to the default implementation)
 
 Alternatively, lock the implementation to a specific version, like so:
 from dapla_pseudo.v1 import pseudonymize
 (which would always resolve to the v1 implementation)
 """
-__version__ = "0.0.1"
+
+import importlib
+
+
+# Avoid having to define the version multiple places.
+# Ref: https://github.com/python-poetry/poetry/issues/144#issuecomment-1488038660
+__version__ = importlib.metadata.version("dapla_toolbelt_pseudo")
 
 from .v1 import PseudoClient
 from .v1 import depseudonymize
 from .v1 import pseudonymize
 from .v1 import repseudonymize
```

### Comparing `dapla_toolbelt_pseudo-0.2.3/src/dapla_pseudo/constants.py` & `dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """This module defines constants that is referenced throughout the codebase."""
 from typing import Final
 
 from pydantic import BaseModel
 
 
-class Env(BaseModel, frozen=True):
+class Env(BaseModel):
     """Environment variables."""
 
     PSEUDO_SERVICE_URL: Final[str] = "PSEUDO_SERVICE_URL"
     PSEUDO_SERVICE_AUTH_TOKEN: Final[str] = "PSEUDO_SERVICE_AUTH_TOKEN"
 
 
-class PredefinedKeys(BaseModel, frozen=True):
+class PredefinedKeys(BaseModel):
     """Names of 'global keys' that the Dapla Pseudo Service is familiar with."""
 
     SSB_COMMON_KEY_1: Final[str] = "ssb-common-key-1"
     SSB_COMMON_KEY_2: Final[str] = "ssb-common-key-2"
     PAPIS_COMMON_KEY_1: Final[str] = "papis-common-key-1"
```

### Comparing `dapla_toolbelt_pseudo-0.2.3/src/dapla_pseudo/models.py` & `dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/models.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.3/src/dapla_pseudo/utils.py` & `dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/utils.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.3/src/dapla_pseudo/v1/client.py` & `dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/v1/client.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.3/src/dapla_pseudo/v1/models.py` & `dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/v1/models.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.3/src/dapla_pseudo/v1/ops.py` & `dapla_toolbelt_pseudo-0.2.4/src/dapla_pseudo/v1/ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,48 +20,58 @@
 import pandas as pd
 import requests
 
 from dapla_pseudo.constants import env
 from dapla_pseudo.constants import predefined_keys
 
 from ..types import _BinaryFileDecl
-from ..types import _DataDecl
+from ..types import _DatasetDecl
 from ..types import _FieldDecl
 from .client import PseudoClient
 from .models import DepseudonymizeFileRequest
 from .models import Field
 from .models import KeyWrapper
 from .models import Mimetypes
 from .models import PseudoConfig
 from .models import PseudoKeyset
 from .models import PseudonymizeFileRequest
 from .models import PseudoRule
 from .models import RepseudonymizeFileRequest
 
 
 def pseudonymize(
-    data: _DataDecl,
-    fields: t.List[_FieldDecl],
+    dataset: _DatasetDecl,
+    fields: t.Optional[t.List[_FieldDecl]] = None,
     sid_fields: t.Optional[t.List[str]] = None,
     key: t.Union[str, PseudoKeyset] = predefined_keys.SSB_COMMON_KEY_1,
     stream: bool = True,
 ) -> requests.Response:
-    """Pseudonymize specified fields of a local file.
+    """Pseudonymize specified fields of a dataset.
 
-    Supported file formats: json
+    The dataset may be supplied as:
+        - A local file on disk (string or Path)
+        - A file handle (io.BufferedReader)
+        - A Pandas dataframe
 
-    The ``fields`` list specifies what to pseudonymize. This can either be a plain vanilla list of field names (e.g.
-    ``["some_field1", "another_field2"]``, or you can apply ninja-style techniques, such as using wildcard characters
-    (e.g. *Name) or slashes to target hierarchical fields (e.g. **/path/to/hierarchicalStuff).
+    Supported file formats: json, csv
 
-    Pseudonymize uses the tink-daead crypto function underneath the hood. It requires a key.
+    The ``fields`` and ``sid_fields`` lists specify what to pseudonymize. At least one of these fields must be specified.
+    The list contents can either be plain field names (e.g. ``["some_field1", "another_field2"]``, or you can apply
+    more advanced techniques, such as using wildcard characters (e.g. *Name) or slashes to target hierarchical fields
+    (e.g. **/path/to/hierarchicalStuff).
+
+    For ``fields``, the ``daead`` pseudonymization function is used. It requires a key.
     You can choose to specify one of the predefined ("globally available") keys ("ssb-common-key-1" or
     "ssb-common-key-2") or provide your own custom keyset. If you don't specify a key, the predefined "ssb-common-key-1"
     will be used as default.
 
+    For ``sid_fields``, the ``map-sid`` pseudonymization function is used. This maps a fødselsnummer to a "stabil ID" and
+    subsequently pseudonymizes the stabil ID using an FPE algorithm. Pseudonyms produced by this function are guaranteed to be
+    compatible with those produced by the PAPIS project.
+
     It is possible to operate on the file in a streaming manner, e.g. like so:
 
     .. code-block:: python
 
         with pseudonymize("./data/personer.json", fields=["fnr", "fornavn", "etternavn"], stream=True) as res:
             with open("./data/personer.json", 'wb') as f:
                 shutil.copyfileobj(res.raw, f)
@@ -69,40 +79,52 @@
     :param data: path to file, file handle or dataframe
     :param fields: list of fields that should be pseudonymized
     :param sid_fields: list of fields that should be mapped to stabil ID and pseudonymized
     :param key: either named reference to a "global" key or a keyset json
     :param stream: true if the results should be chunked into pieces (use for large data)
     :return: pseudonymized data
     """
+    if not fields and not sid_fields:
+        raise ValueError("At least one of fields and sid_fields must be specified.")
+
+    # Avoid later type errors by making sure we have lists
+    if fields is None:
+        fields = []
+    if sid_fields is None:
+        sid_fields = []
+
     file_handle: t.Optional[_BinaryFileDecl] = None
-    match data:
+    match dataset:
         case str() | Path():
             # File path
-            content_type = Mimetypes(magic.from_file(data, mime=True))
+            content_type = Mimetypes(magic.from_file(dataset, mime=True))
         case pd.DataFrame():
             # Dataframe
             content_type = Mimetypes.JSON
-            file_handle = _dataframe_to_json(data, fields, sid_fields)
+            file_handle = _dataframe_to_json(dataset, fields, sid_fields)
         case io.BufferedReader():
             # File handle
-            content_type = Mimetypes(magic.from_buffer(data.read(2048), mime=True))
-            data.seek(0)
-            file_handle = data
+            content_type = Mimetypes(magic.from_buffer(dataset.read(2048), mime=True))
+            dataset.seek(0)
+            file_handle = dataset
         case _:
-            raise ValueError(f"Unsupported data type: {type(data)}. Supported types are {_DataDecl}")
+            raise ValueError(f"Unsupported data type: {type(dataset)}. Supported types are {_DatasetDecl}")
     k = KeyWrapper(key)
     rules = _rules_of(fields=fields, sid_fields=sid_fields or [], key=k.key_id)
     pseudonymize_request = PseudonymizeFileRequest(
-        pseudo_config=PseudoConfig(rules=rules, keysets=k.keyset_list()), target_content_type=content_type
+        pseudo_config=PseudoConfig(rules=rules, keysets=k.keyset_list()),
+        target_content_type=content_type,
+        target_uri=None,
+        compression=None,
     )
 
     if file_handle is not None:
         return _client().pseudonymize(pseudonymize_request, file_handle, stream=stream)
     else:
-        return _client()._process_file("pseudonymize", pseudonymize_request, str(data), stream=stream)
+        return _client()._process_file("pseudonymize", pseudonymize_request, str(dataset), stream=stream)
 
 
 def depseudonymize(
     file_path: str,
     fields: t.List[_FieldDecl],
     key: t.Union[str, PseudoKeyset] = predefined_keys.SSB_COMMON_KEY_1,
     stream: bool = True,
@@ -142,14 +164,16 @@
     """
     content_type = mimetypes.MimeTypes().guess_type(file_path)[0]
     k = KeyWrapper(key)
     rules = _rules_of(fields=fields, sid_fields=[], key=k.key_id)
     req = DepseudonymizeFileRequest(
         pseudo_config=PseudoConfig(rules=rules, keysets=k.keyset_list()),
         target_content_type=content_type,
+        target_uri=None,
+        compression=None,
     )
 
     return _client().depseudonymize_file(req, file_path, stream=stream)
 
 
 def repseudonymize(
     file_path: str,
@@ -197,14 +221,16 @@
     target_key_wrapper = KeyWrapper(target_key)
     source_rules = _rules_of(fields=fields, sid_fields=[], key=source_key_wrapper.key_id)
     target_rules = _rules_of(fields=fields, sid_fields=[], key=target_key_wrapper.key_id)
     req = RepseudonymizeFileRequest(
         source_pseudo_config=PseudoConfig(rules=source_rules, keysets=source_key_wrapper.keyset_list()),
         target_pseudo_config=PseudoConfig(rules=target_rules, keysets=target_key_wrapper.keyset_list()),
         target_content_type=content_type,
+        target_uri=None,
+        compression=None,
     )
 
     return _client().repseudonymize_file(req, file_path, stream=stream)
 
 
 def _client() -> PseudoClient:
     return PseudoClient(
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dapla_toolbelt_pseudo-0.2.3/setup.py` & `dapla_toolbelt_pseudo-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'pyhumps>=3.8.0,<4.0.0',
  'pylibmagic>=0.2.2,<0.3.0',
  'python-magic>=0.4.27,<0.5.0',
  'types-requests>=2.28.11,<3.0.0']
 
 setup_kwargs = {
     'name': 'dapla-toolbelt-pseudo',
-    'version': '0.2.3',
+    'version': '0.2.4',
     'description': 'Pseudonymization extensions for Dapla Toolbelt',
     'long_description': '# Pseudonymization extensions for Dapla Toolbelt\n\n[![PyPI](https://img.shields.io/pypi/v/dapla-toolbelt-pseudo.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/dapla-toolbelt-pseudo.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/dapla-toolbelt-pseudo)][python version]\n[![License](https://img.shields.io/pypi/l/dapla-toolbelt-pseudo)][license]\n\n[![Tests](https://github.com/statisticsnorway/dapla-toolbelt-pseudo/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/statisticsnorway/dapla-toolbelt-pseudo/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/dapla-toolbelt-pseudo/\n[status]: https://pypi.org/project/dapla-toolbelt-pseudo/\n[python version]: https://pypi.org/project/dapla-toolbelt-pseudo\n[tests]: https://github.com/statisticsnorway/dapla-toolbelt-pseudo/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/statisticsnorway/dapla-toolbelt-pseudo\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\nPseudonymize, repseudonymize and depseudonymize data on Dapla.\n\n## Usage\n\nSee the [command-line reference] for details.\n\n### Pseudonymize\n\n```python\nfrom dapla_pseudo import pseudonymize\n\n# Pseudonymize fields in a local file using the default key:\npseudonymize(file_path="./data/personer.json", fields=["fnr", "fornavn"])\n\n# Pseudonymize fields in a local file, explicitly denoting the key to use:\npseudonymize(file_path="./data/personer.json", fields=["fnr", "fornavn"], key="ssb-common-key-1")\n\n# Pseudonymize a local file using a custom key:\nimport json\ncustom_keyset = json.dumps(    {\n    "encryptedKeyset": "CiQAp91NBhLdknX3j9jF6vwhdyURaqcT9/M/iczV7fLn...8XYFKwxiwMtCzDT6QGzCCCM=",\n    "keysetInfo": {\n        "primaryKeyId": 1234567890,\n        "keyInfo": [\n            {\n                "typeUrl": "type.googleapis.com/google.crypto.tink.AesSivKey",\n                "status": "ENABLED",\n                "keyId": 1234567890,\n                "outputPrefixType": "TINK",\n            }\n        ],\n    },\n    "kekUri": "gcp-kms://projects/some-project-id/locations/europe-north1/keyRings/some-keyring/cryptoKeys/some-kek-1",\n})\npseudonymize(file_path="./data/personer.json", fields=["fnr", "fornavn"], key=custom_keyset)\n\n# Operate on data in a streaming manner:\nimport shutil\nwith pseudonymize("./data/personer.json", fields=["fnr", "fornavn", "etternavn"], stream=True) as res:\n    with open("./data/personer_deid.json", \'wb\') as f:\n        res.raw.decode_content = True\n        shutil.copyfileobj(res.raw, f)\n\n# Map certain fields to stabil ID\npseudonymize(file_path="./data/personer.json", fields=["fornavn"], sid_fields=["fnr"])\n```\n\n### Repseudonymize\n\n```python\nfrom dapla_pseudo import repseudonymize\n\n# Repseudonymize fields in a local file, denoting source and target keys to use:\nrepseudonymize(file_path="./data/personer_deid.json", fields=["fnr", "fornavn"], source_key="ssb-common-key-1", target_key="ssb-common-key-2")\n```\n\n### Depseudonymize\n\n```python\nfrom dapla_pseudo import depseudonymize\n\n# Depseudonymize fields in a local file using the default key:\ndepseudonymize(file_path="./data/personer_deid.json", fields=["fnr", "fornavn"])\n\n# Depseudonymize fields in a local file, explicitly denoting the key to use:\ndepseudonymize(file_path="./data/personer_deid.json", fields=["fnr", "fornavn"], key="ssb-common-key-1")\n```\n\n_Note that depseudonymization requires elevated access privileges._\n\n## Requirements\n\n- [Dapla Toolbelt](https://github.com/statisticsnorway/dapla-toolbelt)\n\n## Installation\n\nYou can install _dapla-toolbelt-pseudo_ via [pip] from [PyPI]:\n\n```console\npip install dapla-toolbelt-pseudo\n```\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Pseudonymization extensions for Dapla Toolbelt_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]\'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/statisticsnorway/dapla-toolbelt-pseudo/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/statisticsnorway/dapla-toolbelt-pseudo/blob/main/LICENSE\n[contributor guide]: https://github.com/statisticsnorway/dapla-toolbelt-pseudo/blob/main/CONTRIBUTING.md\n[command-line reference]: https://statisticsnorway.github.io/dapla-toolbelt-pseudo\n',
     'author': 'Team Skyinfrastruktur',
     'author_email': 'dapla@ssb.no',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/statisticsnorway/dapla-toolbelt-pseudo',
```

### Comparing `dapla_toolbelt_pseudo-0.2.3/PKG-INFO` & `dapla_toolbelt_pseudo-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapla-toolbelt-pseudo
-Version: 0.2.3
+Version: 0.2.4
 Summary: Pseudonymization extensions for Dapla Toolbelt
 Home-page: https://github.com/statisticsnorway/dapla-toolbelt-pseudo
 License: MIT
 Author: Team Skyinfrastruktur
 Author-email: dapla@ssb.no
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 4 - Beta
```

