# Comparing `tmp/versions-1.5.0.tar.gz` & `tmp/versions-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "versions-1.5.0.tar", max compression
+gzip compressed data, was "versions-1.6.0.tar", max compression
```

## Comparing `versions-1.5.0.tar` & `versions-1.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1092 2023-05-21 12:51:48.266841 versions-1.5.0/LICENSE
--rw-r--r--   0        0        0     5452 2023-05-21 12:51:48.266841 versions-1.5.0/README.md
--rw-r--r--   0        0        0     3468 2023-05-21 12:51:48.266841 versions-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     3488 2023-05-21 12:51:48.266841 versions-1.5.0/versions/__init__.py
--rw-r--r--   0        0        0      107 2023-05-21 12:51:48.266841 versions-1.5.0/versions/__main__.py
--rw-r--r--   0        0        0     2715 2023-05-21 12:51:48.266841 versions-1.5.0/versions/constants.py
--rw-r--r--   0        0        0      607 2023-05-21 12:51:48.266841 versions-1.5.0/versions/converters.py
--rw-r--r--   0        0        0     3473 2023-05-21 12:51:48.266841 versions-1.5.0/versions/converters_modern.py
--rw-r--r--   0        0        0     3466 2023-05-21 12:51:48.266841 versions-1.5.0/versions/converters_normal.py
--rw-r--r--   0        0        0     2267 2023-05-21 12:51:48.266841 versions-1.5.0/versions/converters_utils.py
--rw-r--r--   0        0        0      520 2023-05-21 12:51:48.266841 versions-1.5.0/versions/errors.py
--rw-r--r--   0        0        0     1934 2023-05-21 12:51:48.266841 versions-1.5.0/versions/functions.py
--rw-r--r--   0        0        0      709 2023-05-21 12:51:48.266841 versions-1.5.0/versions/main.py
--rw-r--r--   0        0        0     1032 2023-05-21 12:51:48.266841 versions-1.5.0/versions/meta.py
--rw-r--r--   0        0        0    28283 2023-05-21 12:51:48.266841 versions-1.5.0/versions/operators.py
--rw-r--r--   0        0        0     7989 2023-05-21 12:51:48.266841 versions-1.5.0/versions/parsers.py
--rw-r--r--   0        0        0     7816 2023-05-21 12:51:48.266841 versions-1.5.0/versions/patterns.py
--rw-r--r--   0        0        0     2602 2023-05-21 12:51:48.266841 versions-1.5.0/versions/phases.py
--rw-r--r--   0        0        0        0 2023-05-21 12:51:48.266841 versions-1.5.0/versions/py.typed
--rw-r--r--   0        0        0      429 2023-05-21 12:51:48.266841 versions-1.5.0/versions/representation.py
--rw-r--r--   0        0        0    21914 2023-05-21 12:51:48.266841 versions-1.5.0/versions/segments.py
--rw-r--r--   0        0        0     1025 2023-05-21 12:51:48.266841 versions-1.5.0/versions/specification.py
--rw-r--r--   0        0        0     7560 2023-05-21 12:51:48.266841 versions-1.5.0/versions/specifiers.py
--rw-r--r--   0        0        0     3650 2023-05-21 12:51:48.266841 versions-1.5.0/versions/string.py
--rw-r--r--   0        0        0     3076 2023-05-21 12:51:48.266841 versions-1.5.0/versions/types.py
--rw-r--r--   0        0        0     1288 2023-05-21 12:51:48.266841 versions-1.5.0/versions/utils.py
--rw-r--r--   0        0        0    27967 2023-05-21 12:51:48.270841 versions-1.5.0/versions/version.py
--rw-r--r--   0        0        0    40692 2023-05-21 12:51:48.270841 versions-1.5.0/versions/version_sets.py
--rw-r--r--   0        0        0     2654 2023-05-21 12:51:48.270841 versions-1.5.0/versions/versioned.py
--rw-r--r--   0        0        0     6828 1970-01-01 00:00:00.000000 versions-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-23 22:01:03.177240 versions-1.6.0/LICENSE
+-rw-r--r--   0        0        0     5452 2023-05-23 22:01:03.177240 versions-1.6.0/README.md
+-rw-r--r--   0        0        0     3468 2023-05-23 22:01:03.181240 versions-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3460 2023-05-23 22:01:03.181240 versions-1.6.0/versions/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-23 22:01:03.181240 versions-1.6.0/versions/__main__.py
+-rw-r--r--   0        0        0     2715 2023-05-23 22:01:03.181240 versions-1.6.0/versions/constants.py
+-rw-r--r--   0        0        0      607 2023-05-23 22:01:03.181240 versions-1.6.0/versions/converters.py
+-rw-r--r--   0        0        0     3473 2023-05-23 22:01:03.181240 versions-1.6.0/versions/converters_modern.py
+-rw-r--r--   0        0        0     3466 2023-05-23 22:01:03.181240 versions-1.6.0/versions/converters_normal.py
+-rw-r--r--   0        0        0     2267 2023-05-23 22:01:03.181240 versions-1.6.0/versions/converters_utils.py
+-rw-r--r--   0        0        0      520 2023-05-23 22:01:03.181240 versions-1.6.0/versions/errors.py
+-rw-r--r--   0        0        0     1934 2023-05-23 22:01:03.181240 versions-1.6.0/versions/functions.py
+-rw-r--r--   0        0        0      709 2023-05-23 22:01:03.181240 versions-1.6.0/versions/main.py
+-rw-r--r--   0        0        0     1017 2023-05-23 22:01:03.181240 versions-1.6.0/versions/meta.py
+-rw-r--r--   0        0        0    28283 2023-05-23 22:01:03.181240 versions-1.6.0/versions/operators.py
+-rw-r--r--   0        0        0     7989 2023-05-23 22:01:03.181240 versions-1.6.0/versions/parsers.py
+-rw-r--r--   0        0        0     7816 2023-05-23 22:01:03.181240 versions-1.6.0/versions/patterns.py
+-rw-r--r--   0        0        0     2602 2023-05-23 22:01:03.181240 versions-1.6.0/versions/phases.py
+-rw-r--r--   0        0        0        0 2023-05-23 22:01:03.181240 versions-1.6.0/versions/py.typed
+-rw-r--r--   0        0        0      429 2023-05-23 22:01:03.181240 versions-1.6.0/versions/representation.py
+-rw-r--r--   0        0        0    21914 2023-05-23 22:01:03.181240 versions-1.6.0/versions/segments.py
+-rw-r--r--   0        0        0     1025 2023-05-23 22:01:03.181240 versions-1.6.0/versions/specification.py
+-rw-r--r--   0        0        0     7560 2023-05-23 22:01:03.181240 versions-1.6.0/versions/specifiers.py
+-rw-r--r--   0        0        0     3650 2023-05-23 22:01:03.181240 versions-1.6.0/versions/string.py
+-rw-r--r--   0        0        0     3076 2023-05-23 22:01:03.181240 versions-1.6.0/versions/types.py
+-rw-r--r--   0        0        0     1288 2023-05-23 22:01:03.181240 versions-1.6.0/versions/utils.py
+-rw-r--r--   0        0        0    27967 2023-05-23 22:01:03.181240 versions-1.6.0/versions/version.py
+-rw-r--r--   0        0        0    40692 2023-05-23 22:01:03.185240 versions-1.6.0/versions/version_sets.py
+-rw-r--r--   0        0        0     1903 2023-05-23 22:01:03.185240 versions-1.6.0/versions/versioned.py
+-rw-r--r--   0        0        0     6828 1970-01-01 00:00:00.000000 versions-1.6.0/PKG-INFO
```

### Comparing `versions-1.5.0/LICENSE` & `versions-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `versions-1.5.0/README.md` & `versions-1.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add versions
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-versions = "^1.5.0"
+versions = "^1.6.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.versions]
 git = "https://github.com/nekitdev/versions.git"
@@ -148,15 +148,15 @@
 
 `versions` allows users to access versions of items that have the `__version__` attribute:
 
 ```python
 >>> from versions import get_version
 >>> import versions
 >>> get_version(versions)
-<Version (1.5.0)>
+<Version (1.6.0)>
 ```
 
 ## Documentation
 
 You can find the documentation [here][Documentation].
 
 ## Support
```

### Comparing `versions-1.5.0/pyproject.toml` & `versions-1.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "versions"
-version = "1.5.0"
+version = "1.6.0"
 description = "Parsing, inspecting and specifying versions."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/versions"
@@ -30,15 +30,15 @@
 include = "versions"
 
 [tool.poetry.dependencies]
 python = ">= 3.7"
 
 attrs = ">= 23.1.0"
 
-typing-aliases = ">= 1.1.1"
+typing-aliases = ">= 1.1.2"
 typing-extensions = ">= 4.5.0"
 
 click = ">= 8.1.3"
 
 orderings = ">= 1.1.0"
 solus = ">= 1.1.0"
 entrypoint = ">= 1.4.0"
@@ -147,15 +147,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "versions"
-version = "1.5.0"
+version = "1.6.0"
 url = "https://github.com/nekitdev/versions"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `versions-1.5.0/versions/__init__.py` & `versions-1.6.0/versions/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 __description__ = "Parsing, inspecting and specifying versions."
 __url__ = "https://github.com/nekitdev/versions"
 
 __title__ = "versions"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "1.5.0"
+__version__ = "1.6.0"
 
 from versions.converters import (
     simplify,
     specifier_from_version_set,
     specifier_to_version_set,
     version_set_from_specifier,
     version_set_to_specifier,
@@ -69,17 +69,17 @@
     is_version_item,
     is_version_point,
     is_version_range,
     is_version_set,
     is_version_union,
 )
 from versions.versioned import (
+    VERSION,
     Versioned,
     get_version,
-    get_version_unchecked,
     has_version,
     is_versioned,
 )
 
 __all__ = (
     # versions
     "Version",
@@ -142,13 +142,13 @@
     "parse_specifier",
     "parse_version",
     "parse_version_set",
     # meta
     "version_info",
     "python_version_info",
     # versioned
+    "VERSION",
     "Versioned",
-    "is_versioned",
-    "has_version",
     "get_version",
-    "get_version_unchecked",
+    "has_version",
+    "is_versioned",
 )
```

### Comparing `versions-1.5.0/versions/constants.py` & `versions-1.6.0/versions/constants.py`

 * *Files identical despite different names*

### Comparing `versions-1.5.0/versions/converters.py` & `versions-1.6.0/versions/converters.py`

 * *Files identical despite different names*

### Comparing `versions-1.5.0/versions/converters_modern.py` & `versions-1.6.0/versions/converters_modern.py`

 * *Files identical despite different names*

### Comparing `versions-1.5.0/versions/converters_normal.py` & `versions-1.6.0/versions/converters_normal.py`

 * *Files identical despite different names*

### Comparing `versions-1.5.0/versions/converters_utils.py` & `versions-1.6.0/versions/converters_utils.py`

 * *Files identical despite different names*

### Comparing `versions-1.5.0/versions/errors.py` & `versions-1.6.0/versions/errors.py`

 * *Files identical despite different names*

### Comparing `versions-1.5.0/versions/functions.py` & `versions-1.6.0/versions/functions.py`

 * *Files identical despite different names*

### Comparing `versions-1.5.0/versions/main.py` & `versions-1.6.0/versions/main.py`

 * *Files identical despite different names*

### Comparing `versions-1.5.0/versions/meta.py` & `versions-1.6.0/versions/meta.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from sys import version_info as python_version_tuple
 
 from typing_extensions import Final
 
-from versions import __version__ as version
-from versions.functions import parse_version
+import versions
 from versions.segments import PreTag
 from versions.version import Version
+from versions.versioned import get_version
 
 __all__ = ("version_info", "python_version_info")
 
-version_info = parse_version(version)
+version_info = get_version(versions)  # type: ignore
 """The library version represented as a [`Version`][versions.version.Version]."""
 
 FINAL: Final[str] = "final"
 
 python_major, python_minor, python_micro, python_phase, python_value = python_version_tuple
 
 if python_phase == FINAL:  # pragma: no cover
```

### Comparing `versions-1.5.0/versions/operators.py` & `versions-1.6.0/versions/operators.py`

 * *Files identical despite different names*

### Comparing `versions-1.5.0/versions/parsers.py` & `versions-1.6.0/versions/parsers.py`

 * *Files identical despite different names*

### Comparing `versions-1.5.0/versions/patterns.py` & `versions-1.6.0/versions/patterns.py`

 * *Files identical despite different names*

### Comparing `versions-1.5.0/versions/phases.py` & `versions-1.6.0/versions/phases.py`

 * *Files identical despite different names*

### Comparing `versions-1.5.0/versions/segments.py` & `versions-1.6.0/versions/segments.py`

 * *Files identical despite different names*

### Comparing `versions-1.5.0/versions/specification.py` & `versions-1.6.0/versions/specification.py`

 * *Files identical despite different names*

### Comparing `versions-1.5.0/versions/specifiers.py` & `versions-1.6.0/versions/specifiers.py`

 * *Files identical despite different names*

### Comparing `versions-1.5.0/versions/string.py` & `versions-1.6.0/versions/string.py`

 * *Files identical despite different names*

### Comparing `versions-1.5.0/versions/types.py` & `versions-1.6.0/versions/types.py`

 * *Files identical despite different names*

### Comparing `versions-1.5.0/versions/utils.py` & `versions-1.6.0/versions/utils.py`

 * *Files identical despite different names*

### Comparing `versions-1.5.0/versions/version.py` & `versions-1.6.0/versions/version.py`

 * *Files identical despite different names*

### Comparing `versions-1.5.0/versions/version_sets.py` & `versions-1.6.0/versions/version_sets.py`

 * *Files identical despite different names*

### Comparing `versions-1.5.0/versions/versioned.py` & `versions-1.6.0/versions/versioned.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 
 from versions.functions import parse_version
 from versions.version import Version
 
 __all__ = (
     "VERSION",
     "Versioned",
-    "is_versioned",
-    "has_version",
     "get_version",
-    "get_version_unchecked",
+    "has_version",
+    "is_versioned",
 )
 
 VERSION = "__version__"
 
 
 @runtime_checkable
 class Versioned(Protocol):
@@ -46,48 +45,24 @@
 """An alias of [`is_versioned`][versions.versioned.is_versioned]."""
 
 
 V = TypeVar("V", bound=Version)
 
 
 @overload
-def get_version(item: Any) -> Optional[Version]:
-    ...
-
-
-@overload
-def get_version(item: Any, version_type: Type[V]) -> Optional[V]:
-    ...
-
-
-def get_version(item: Any, version_type: Type[Version] = Version) -> Optional[Version]:
-    """Parses the version of the `item` if [`has_version(item)`][versions.versioned.has_version],
-    otherwise this function returns [`None`][None].
-
-    Parameters:
-        item: The item to fetch the version from.
-        version_type: The type of the version to parse.
-
-    Returns:
-        The version of `version_type` of the `item`, if one is present, otherwise [`None`][None].
-    """
-    return get_version_unchecked(item, version_type) if has_version(item) else None
-
-
-@overload
-def get_version_unchecked(item: Versioned) -> Version:
+def get_version(item: Versioned) -> Optional[Version]:
     ...
 
 
 @overload
-def get_version_unchecked(item: Versioned, version_type: Type[V]) -> V:
+def get_version(item: Versioned, version_type: Type[V]) -> Optional[V]:
     ...
 
 
-def get_version_unchecked(item: Versioned, version_type: Type[Version] = Version) -> Version:
+def get_version(item: Versioned, version_type: Type[Version] = Version) -> Optional[Version]:
     """Fetches the `__version__` attribute of the `item`,
     parsing it into the version of `version_type`, without checking whether the attribute exists.
 
     Parameters:
         item: The item to fetch the version from.
         version_type: The type of the version to parse.
```

### Comparing `versions-1.5.0/PKG-INFO` & `versions-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: versions
-Version: 1.5.0
+Version: 1.6.0
 Summary: Parsing, inspecting and specifying versions.
 Home-page: https://github.com/nekitdev/versions
 License: MIT
 Keywords: python,semver,version
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,15 +20,15 @@
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: attrs (>=23.1.0)
 Requires-Dist: click (>=8.1.3)
 Requires-Dist: entrypoint (>=1.4.0)
 Requires-Dist: orderings (>=1.1.0)
 Requires-Dist: solus (>=1.1.0)
-Requires-Dist: typing-aliases (>=1.1.1)
+Requires-Dist: typing-aliases (>=1.1.2)
 Requires-Dist: typing-extensions (>=4.5.0)
 Project-URL: Documentation, https://nekitdev.github.io/versions
 Project-URL: Discord, https://nekit.dev/discord
 Project-URL: Funding, https://patreon.com/nekitdev
 Project-URL: Issues, https://github.com/nekitdev/versions/issues
 Project-URL: Repository, https://github.com/nekitdev/versions
 Description-Content-Type: text/markdown
@@ -75,15 +75,15 @@
 $ poetry add versions
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-versions = "^1.5.0"
+versions = "^1.6.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.versions]
 git = "https://github.com/nekitdev/versions.git"
@@ -183,15 +183,15 @@
 
 `versions` allows users to access versions of items that have the `__version__` attribute:
 
 ```python
 >>> from versions import get_version
 >>> import versions
 >>> get_version(versions)
-<Version (1.5.0)>
+<Version (1.6.0)>
 ```
 
 ## Documentation
 
 You can find the documentation [here][Documentation].
 
 ## Support
```

