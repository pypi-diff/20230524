# Comparing `tmp/heksher-0.2.1.tar.gz` & `tmp/heksher-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heksher-0.2.1.tar", max compression
+gzip compressed data, was "heksher-0.2.2.tar", max compression
```

## Comparing `heksher-0.2.1.tar` & `heksher-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1088 2022-04-25 07:31:11.964611 heksher-0.2.1/LICENSE
--rw-r--r--   0        0        0     1511 2022-04-25 07:31:11.964611 heksher-0.2.1/README.md
--rw-r--r--   0        0        0      543 2022-04-25 07:31:11.964611 heksher-0.2.1/heksher/__init__.py
--rw-r--r--   0        0        0       22 2022-04-25 07:31:11.964611 heksher-0.2.1/heksher/_version.py
--rw-r--r--   0        0        0        0 2022-04-25 07:31:11.964611 heksher-0.2.1/heksher/clients/__init__.py
--rw-r--r--   0        0        0    10318 2022-04-25 07:31:11.964611 heksher-0.2.1/heksher/clients/async_client.py
--rw-r--r--   0        0        0     4080 2022-04-25 07:31:11.964611 heksher-0.2.1/heksher/clients/stub.py
--rw-r--r--   0        0        0    15725 2022-04-25 07:31:11.964611 heksher-0.2.1/heksher/clients/subclasses.py
--rw-r--r--   0        0        0     7826 2022-04-25 07:31:11.964611 heksher-0.2.1/heksher/clients/thread_client.py
--rw-r--r--   0        0        0     4185 2022-04-25 07:31:11.964611 heksher-0.2.1/heksher/clients/util.py
--rw-r--r--   0        0        0      178 2022-04-25 07:31:11.964611 heksher-0.2.1/heksher/exceptions.py
--rw-r--r--   0        0        0     1761 2022-04-25 07:31:11.964611 heksher-0.2.1/heksher/heksher_client.py
--rw-r--r--   0        0        0      326 2022-04-25 07:31:11.964611 heksher-0.2.1/heksher/main_client.py
--rw-r--r--   0        0        0     9332 2022-04-25 07:31:11.964611 heksher-0.2.1/heksher/setting.py
--rw-r--r--   0        0        0     7266 2022-04-25 07:31:11.964611 heksher-0.2.1/heksher/setting_type.py
--rw-r--r--   0        0        0     2273 2022-04-25 07:31:11.964611 heksher-0.2.1/heksher/util.py
--rw-r--r--   0        0        0      907 2022-04-25 07:31:11.964611 heksher-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2447 2022-04-25 07:31:29.735864 heksher-0.2.1/setup.py
--rw-r--r--   0        0        0     2426 2022-04-25 07:31:29.736312 heksher-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-24 13:52:35.602808 heksher-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1511 2023-05-24 13:52:35.602808 heksher-0.2.2/README.md
+-rw-r--r--   0        0        0      543 2023-05-24 13:52:35.602808 heksher-0.2.2/heksher/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-24 13:52:35.602808 heksher-0.2.2/heksher/_version.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:52:35.602808 heksher-0.2.2/heksher/clients/__init__.py
+-rw-r--r--   0        0        0    10754 2023-05-24 13:52:35.602808 heksher-0.2.2/heksher/clients/async_client.py
+-rw-r--r--   0        0        0     4080 2023-05-24 13:52:35.602808 heksher-0.2.2/heksher/clients/stub.py
+-rw-r--r--   0        0        0    15725 2023-05-24 13:52:35.602808 heksher-0.2.2/heksher/clients/subclasses.py
+-rw-r--r--   0        0        0     7826 2023-05-24 13:52:35.602808 heksher-0.2.2/heksher/clients/thread_client.py
+-rw-r--r--   0        0        0     4185 2023-05-24 13:52:35.602808 heksher-0.2.2/heksher/clients/util.py
+-rw-r--r--   0        0        0      178 2023-05-24 13:52:35.602808 heksher-0.2.2/heksher/exceptions.py
+-rw-r--r--   0        0        0     1761 2023-05-24 13:52:35.602808 heksher-0.2.2/heksher/heksher_client.py
+-rw-r--r--   0        0        0      326 2023-05-24 13:52:35.602808 heksher-0.2.2/heksher/main_client.py
+-rw-r--r--   0        0        0     9375 2023-05-24 13:52:35.602808 heksher-0.2.2/heksher/setting.py
+-rw-r--r--   0        0        0     8082 2023-05-24 13:52:35.602808 heksher-0.2.2/heksher/setting_type.py
+-rw-r--r--   0        0        0     2273 2023-05-24 13:52:35.602808 heksher-0.2.2/heksher/util.py
+-rw-r--r--   0        0        0      905 2023-05-24 13:52:35.602808 heksher-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2471 1970-01-01 00:00:00.000000 heksher-0.2.2/PKG-INFO
```

### Comparing `heksher-0.2.1/LICENSE` & `heksher-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `heksher-0.2.1/README.md` & `heksher-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `heksher-0.2.1/heksher/__init__.py` & `heksher-0.2.2/heksher/__init__.py`

 * *Files identical despite different names*

### Comparing `heksher-0.2.1/heksher/clients/async_client.py` & `heksher-0.2.2/heksher/clients/async_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     wait, wait_for
 )
 from contextvars import ContextVar
 from logging import getLogger
 from typing import Any, Awaitable, Dict, NoReturn, Optional, Sequence, TypeVar, Union
 
 import orjson
-from httpx import AsyncClient, HTTPError
+from httpx import AsyncClient, HTTPError, HTTPStatusError
 
 from heksher.clients.subclasses import AsyncContextManagerMixin, ContextFeaturesMixin, V1APIClient
 from heksher.clients.util import SettingsOutput
 from heksher.setting import Setting
 
 logger = getLogger(__name__)
 
@@ -125,15 +125,18 @@
         while True:
             try:
                 await update()
             except CancelledError:
                 # in 3.7, cancelled is a normal exception
                 raise
             except Exception as e:
-                logger.exception('error during heksher update')
+                log_extras = {}
+                if isinstance(e, HTTPStatusError):
+                    log_extras['response_content'] = e.response.content
+                logger.exception('error during heksher update', extra=log_extras)
                 if self._update_error is not None:
                     self._update_error.set_exception(e)
                 self.on_update_error(e)
             finally:
                 self._update_event.set()
                 self.on_update_ok()
 
@@ -186,15 +189,17 @@
                 logger.warning('context feature mismatch', extra={
                     'features_in_service': features_in_service,
                     'features_in_client': self._context_features
                 })
 
         try:
             self._declaration_task = create_task(self._declaration_loop())
-            await wait_with_err_sentinel(self._undeclared.join(), self._wait_for_declaration_error())
+            undeclared_task = create_task(self._undeclared.join())
+            wait_for_update_error_task = create_task(self._wait_for_update_error())
+            await wait_with_err_sentinel(undeclared_task, wait_for_update_error_task)
             # important to only start the update thread once all pending settings are declared, otherwise we may have
             # stale settings
             self._update_task = create_task(self._update_loop())
             await self.reload()
         except Exception:
             await self.aclose()
             raise
@@ -202,15 +207,17 @@
     async def reload(self):
         """
         Block until all the tracked settings are up to date
         """
         await self._undeclared.join()
         self._update_event.clear()
         self._manual_update.set()
-        await wait_with_err_sentinel(self._update_event.wait(), self._wait_for_update_error())
+        update_event_task = create_task(self._update_event.wait())
+        wait_for_update_error_task = create_task(self._wait_for_update_error())
+        await wait_with_err_sentinel(update_event_task, wait_for_update_error_task)
 
     async def aclose(self):
         await super().aclose()
         if self._update_task:
             self._update_task.cancel()
             try:
                 await wait_for(self._update_task, 0.01)
@@ -243,16 +250,15 @@
         response = await self._http_client.get('/api/health')
         response.raise_for_status()
 
     async def get_settings(self) -> Dict:
         """
         List all the settings in the service
         """
-        response = await self._http_client.get('/api/v1/settings', params=orjson.dumps(
-            {'include_additional_data': True}))
+        response = await self._http_client.get('/api/v1/settings', params={'include_additional_data': 'True'})
         response.raise_for_status()
         settings = SettingsOutput.parse_obj(response.json()).to_settings_data()
         return settings
 
     def on_update_error(self, exc):
         # override this method to handle update errors
         pass
```

### Comparing `heksher-0.2.1/heksher/clients/stub.py` & `heksher-0.2.2/heksher/clients/stub.py`

 * *Files identical despite different names*

### Comparing `heksher-0.2.1/heksher/clients/subclasses.py` & `heksher-0.2.2/heksher/clients/subclasses.py`

 * *Files identical despite different names*

### Comparing `heksher-0.2.1/heksher/clients/thread_client.py` & `heksher-0.2.2/heksher/clients/thread_client.py`

 * *Files identical despite different names*

### Comparing `heksher-0.2.1/heksher/clients/util.py` & `heksher-0.2.2/heksher/clients/util.py`

 * *Files identical despite different names*

### Comparing `heksher-0.2.1/heksher/heksher_client.py` & `heksher-0.2.2/heksher/heksher_client.py`

 * *Files identical despite different names*

### Comparing `heksher-0.2.1/heksher/setting.py` & `heksher-0.2.2/heksher/setting.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
         self._validators: List[Validator[T]] = []
         self.server_default_value: Optional[T] = None
 
         heksher.main_client.Main.add_settings((self,))
 
     def convert_server_value(self, raw_value: Any, rule: Optional[QueriedRule]) -> Conversion[T]:
-        convert = self.type.convert(raw_value)
+        convert = self.type.convert_from_heksher(raw_value)
         if convert.coercions:
             value = self.on_coerce(convert.value, raw_value, convert.coercions, rule, self)
         else:
             value = convert.value
         for validator in self._validators:
             value = validator(value, rule, self)
         return Conversion(value, convert.coercions)
@@ -158,15 +158,15 @@
         """
         return {
             'name': self.name,
             'configurable_features': list(self.configurable_features),
             'type': self.type.heksher_string(),
             'metadata': self.metadata,
             'alias': self.alias,
-            'default_value': self.default_value,
+            'default_value': self.type.convert_to_heksher(self.default_value),
             'version': self.version_str,
         }
 
 
 @dataclass(frozen=True)
 class RuleMatch(Generic[T]):
     """
```

### Comparing `heksher-0.2.1/heksher/setting_type.py` & `heksher-0.2.2/heksher/setting_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,27 +45,38 @@
     def heksher_string(self) -> str:
         """
         Returns: The type as string, as specified by the Heksher specs
         """
         pass
 
     @abstractmethod
-    def convert(self, x) -> Conversion[T]:
+    def convert_from_heksher(self, x) -> Conversion[T]:
         """
         Args:
             x: JSON-parsed value, retrieved from http api
 
         Returns:
             x, converted to an immutable pythonic value
 
         Notes:
             convert must return an immutable value
         """
         pass
 
+    @abstractmethod
+    def convert_to_heksher(self, x: T) -> Any:
+        """
+        Args:
+            x: immutable pythonic value
+
+        Returns:
+            x, JSON-parsed value
+        """
+        pass
+
     def __eq__(self, other):
         return isinstance(other, SettingType) and self.heksher_string() == other.heksher_string()
 
 
 class SimpleSettingType(SettingType[T]):
     """
     A setting type for immutable primitives
@@ -74,19 +85,22 @@
     def __init__(self, name, acceptable_types: Tuple[type, ...]):
         self.name = name
         self.type = acceptable_types
 
     def heksher_string(self) -> str:
         return self.name
 
-    def convert(self, x):
+    def convert_from_heksher(self, x):
         if not isinstance(x, self.type):
             raise TypeError(f'value is not of type {self.type}')
         return Conversion(x)
 
+    def convert_to_heksher(self, x: T) -> Any:
+        return x
+
 
 F = TypeVar('F', bound=IntFlag)
 
 
 class HeksherFlags(SettingType[F]):
     """
     A setting type for flags, reflecting a flags of strings in heksher service.
@@ -101,28 +115,31 @@
             flags_type: The IntFlags subclass to use as a type
         """
         self.type_ = flags_type
 
     def heksher_string(self) -> str:
         return 'Flags[' + ','.join(sorted(str(orjson.dumps(x), 'utf-8') for x in self.type_.__members__)) + ']'
 
-    def convert(self, x) -> Conversion[F]:
+    def convert_from_heksher(self, x) -> Conversion[F]:
         ret = self.type_(0)
         coercions = []
         for i in x:
             if not isinstance(i, str):
                 raise TypeError(f'expected string in flags, got {type(i).__name__}')
             try:
                 member = self.type_[i]
             except KeyError:
                 coercions.append(f'server sent a flag value not found in the python type ({i})')
             else:
                 ret |= member
         return Conversion(ret, coercions)
 
+    def convert_to_heksher(self, x: F) -> Any:
+        return [flag.name for flag in self.type_ if x & flag]
+
 
 E = TypeVar('E', bound=Enum)
 
 
 class HeksherEnum(SettingType[E]):
     """
     A setting type for an enum of primitive values
@@ -137,20 +154,23 @@
         for member in self.type_:
             if type(member.value) not in (int, str, float, bool):
                 raise TypeError(f'enum member {member} has a non-primitive value of type')
 
     def heksher_string(self) -> str:
         return 'Enum[' + ','.join(sorted(str(orjson.dumps(x.value), 'utf-8') for x in self.type_)) + ']'
 
-    def convert(self, x) -> Conversion[E]:
+    def convert_from_heksher(self, x) -> Conversion[E]:
         try:
             return Conversion(self.type_(x))
         except ValueError as ve:
             raise TypeError('value is not a valid enum member') from ve
 
+    def convert_to_heksher(self, x: E) -> Any:
+        return x.value
+
 
 class HeksherSequence(SettingType[Sequence[T]]):
     """
     A setting type for a sequence type
     """
 
     def __init__(self, inner: SettingType[T]):
@@ -159,27 +179,30 @@
             inner: the inner setting type of each member
         """
         self.inner = setting_type(inner)
 
     def heksher_string(self) -> str:
         return f'Sequence<{self.inner.heksher_string()}>'
 
-    def convert(self, x) -> Conversion[Sequence[T]]:
+    def convert_from_heksher(self, x) -> Conversion[Sequence[T]]:
         values = []
         coercions = []
         for i, v in enumerate(x):
             try:
-                conversion = self.inner.convert(v)
+                conversion = self.inner.convert_from_heksher(v)
             except TypeError as e:
                 coercions.append(f'failed to convert element {i}: {e!r}')
             else:
                 values.append(conversion.value)
                 coercions.extend(f'element {i}: {c}' for c in conversion.coercions)
         return Conversion(tuple(values), coercions)
 
+    def convert_to_heksher(self, x: Sequence[T]) -> Any:
+        return [self.inner.convert_to_heksher(v) for v in x]
+
 
 class HeksherMapping(SettingType[Mapping[str, T]]):
     """
     A setting type for a mapping type with string keys
     """
 
     def __init__(self, inner: SettingType[T]):
@@ -188,27 +211,30 @@
             inner: the inner setting type of each value in the
         """
         self.inner = setting_type(inner)
 
     def heksher_string(self) -> str:
         return f'Mapping<{self.inner.heksher_string()}>'
 
-    def convert(self, x) -> Conversion[Mapping[str, T]]:
+    def convert_from_heksher(self, x) -> Conversion[Mapping[str, T]]:
         values = {}
         coercions = []
         for k, v in x.items():
             try:
-                conversion = self.inner.convert(v)
+                conversion = self.inner.convert_from_heksher(v)
             except TypeError as e:
                 coercions.append(f'failed to convert value for key {k}: {e!r}')
             else:
                 values[k] = conversion.value
                 coercions.extend(f'{k}: {c}' for c in conversion.coercions)
         return Conversion(MappingProxyType(values), coercions)
 
+    def convert_to_heksher(self, x: Mapping[str, T]) -> Any:
+        return {k: self.inner.convert_to_heksher(v) for k, v in x.items()}
+
 
 _simples: Mapping[type, SettingType] = {
     int: SimpleSettingType('int', (int,)),
     float: SimpleSettingType('float', (int, float)),
     str: SimpleSettingType('str', (str,)),
     bool: SimpleSettingType('bool', (bool,)),
 }
```

### Comparing `heksher-0.2.1/heksher/util.py` & `heksher-0.2.2/heksher/util.py`

 * *Files identical despite different names*

### Comparing `heksher-0.2.1/pyproject.toml` & `heksher-0.2.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 [tool.poetry]
 name = "heksher"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["Biocatch LTD <serverteam@biocatch.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/biocatchltd/heksher-py"
 packages = [
     {include="heksher"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-orjson = "^3.0.0"
+orjson = ">=3.0.0"
 httpx = "*"
 mock = {version="^4.0.0", markers = "python_version < '3.8'"}
 ordered-set = "^4.0.0"
 pydantic = "^1.0.0"
 sortedcontainers = "^2.4.0"
 Deprecated = ">=1.2.13"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytest-asyncio = "*"
-flake8 = { version = "*", allow-prereleases = true }
+flake8 = "^4.0.1"
 isort = "^5.9.1"
-mypy = "^0.902"
+mypy = "^0.950"
 types-mock = "^0.1.3"
 types-orjson = "^0.1.1"
-pytest-cov = "*"
-yellowbox = {version="^0.6.0", extras=["webserver"]}
+coverage = "^6.4.4"
+yellowbox = {version="^0.7.0", extras=["webserver"]}
+yellowbox-heksher = "^0.2.0"
 Sphinx = "^4.3.1"
 sphinx-rtd-theme = "^1.0.0"
 types-Deprecated = "^1.2.6"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `heksher-0.2.1/setup.py` & `heksher-0.2.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,66 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['heksher', 'heksher.clients']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Deprecated>=1.2.13',
- 'httpx',
- 'ordered-set>=4.0.0,<5.0.0',
- 'orjson>=3.0.0,<4.0.0',
- 'pydantic>=1.0.0,<2.0.0',
- 'sortedcontainers>=2.4.0,<3.0.0']
-
-extras_require = \
-{':python_version < "3.8"': ['mock>=4.0.0,<5.0.0']}
-
-setup_kwargs = {
-    'name': 'heksher',
-    'version': '0.2.1',
-    'description': '',
-    'long_description': '# heksher SDK for python\nThis is a library for using a [heksher](https://github.com/biocatchltd/Heksher) server from within python.\nCompatible with python 3.7, 3.8, and 3.9. The library contains both an asynchronous client, as well as a thread-based\nclient. Also included are stub clients to make testing without a service simple.\n\n## Example usage\n```python\n# main.py\nfrom contextvars import ContextVar\nfrom heksher import AsyncHeksherClient, Setting\n\nuser = ContextVar(\'user\', default=\'guest\')\n\nclass App:\n    ...\n    \n    async def startup(self):\n        ...\n        \n        # initialize the client, and set it as the process\' main client\n        self.heksher_client = AsyncHeksherClient(\'http://heksher.service.url\',\n                                            update_interval=60, \n                                            context_features=[\'user\', \'trust\', \'theme\'])\n        # set certain context features to be retrieved either from string constants or\n        # context variables \n        self.heksher_client.set_defaults(user = user, theme="light")\n        await self.heksher_client.set_as_main()\n    \n    async def shutdown(self):\n        await self.heksher_client.close()        \n        ...\n\ncache_size_setting = Setting(\'cache_size\', type=int, configurable_features=[\'user\', \'trust\'], default_value=10)\ndef foo(trust: str):\n    ...\n    # should be run after App.startup is completed\n    cache_size = cache_size_setting.get(trust=trust)\n    ...\n```\nThread-based client usage is nearly identical. ',
-    'author': 'Biocatch LTD',
-    'author_email': 'serverteam@biocatch.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/biocatchltd/heksher-py',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: heksher
+Version: 0.2.2
+Summary: 
+Home-page: https://github.com/biocatchltd/heksher-py
+License: MIT
+Author: Biocatch LTD
+Author-email: serverteam@biocatch.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Deprecated (>=1.2.13)
+Requires-Dist: httpx
+Requires-Dist: mock (>=4.0.0,<5.0.0) ; python_version < "3.8"
+Requires-Dist: ordered-set (>=4.0.0,<5.0.0)
+Requires-Dist: orjson (>=3.0.0)
+Requires-Dist: pydantic (>=1.0.0,<2.0.0)
+Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0)
+Project-URL: Repository, https://github.com/biocatchltd/heksher-py
+Description-Content-Type: text/markdown
+
+# heksher SDK for python
+This is a library for using a [heksher](https://github.com/biocatchltd/Heksher) server from within python.
+Compatible with python 3.7, 3.8, and 3.9. The library contains both an asynchronous client, as well as a thread-based
+client. Also included are stub clients to make testing without a service simple.
+
+## Example usage
+```python
+# main.py
+from contextvars import ContextVar
+from heksher import AsyncHeksherClient, Setting
+
+user = ContextVar('user', default='guest')
+
+class App:
+    ...
+    
+    async def startup(self):
+        ...
+        
+        # initialize the client, and set it as the process' main client
+        self.heksher_client = AsyncHeksherClient('http://heksher.service.url',
+                                            update_interval=60, 
+                                            context_features=['user', 'trust', 'theme'])
+        # set certain context features to be retrieved either from string constants or
+        # context variables 
+        self.heksher_client.set_defaults(user = user, theme="light")
+        await self.heksher_client.set_as_main()
+    
+    async def shutdown(self):
+        await self.heksher_client.close()        
+        ...
+
+cache_size_setting = Setting('cache_size', type=int, configurable_features=['user', 'trust'], default_value=10)
+def foo(trust: str):
+    ...
+    # should be run after App.startup is completed
+    cache_size = cache_size_setting.get(trust=trust)
+    ...
+```
+Thread-based client usage is nearly identical.
```

