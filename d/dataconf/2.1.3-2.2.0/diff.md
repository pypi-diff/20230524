# Comparing `tmp/dataconf-2.1.3.tar.gz` & `tmp/dataconf-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataconf-2.1.3.tar", max compression
+gzip compressed data, was "dataconf-2.2.0.tar", max compression
```

## Comparing `dataconf-2.1.3.tar` & `dataconf-2.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    16724 2022-12-05 15:59:49.677131 dataconf-2.1.3/LICENSE
--rw-r--r--   0        0        0     4933 2022-12-05 15:59:49.677131 dataconf-2.1.3/README.md
--rw-r--r--   0        0        0      685 2022-12-05 15:59:49.677131 dataconf-2.1.3/dataconf/__init__.py
--rw-r--r--   0        0        0      871 2022-12-05 15:59:49.677131 dataconf-2.1.3/dataconf/cli.py
--rw-r--r--   0        0        0      691 2022-12-05 15:59:49.677131 dataconf-2.1.3/dataconf/exceptions.py
--rw-r--r--   0        0        0     4310 2022-12-05 15:59:49.677131 dataconf-2.1.3/dataconf/main.py
--rw-r--r--   0        0        0       44 2022-12-05 15:59:49.677131 dataconf-2.1.3/dataconf/py.typed
--rw-r--r--   0        0        0    11164 2022-12-05 15:59:49.677131 dataconf-2.1.3/dataconf/utils.py
--rw-r--r--   0        0        0       22 2022-12-05 15:59:49.677131 dataconf-2.1.3/dataconf/version.py
--rw-r--r--   0        0        0     1199 2022-12-05 15:59:49.677131 dataconf-2.1.3/pyproject.toml
--rw-r--r--   0        0        0     6090 1970-01-01 00:00:00.000000 dataconf-2.1.3/setup.py
--rw-r--r--   0        0        0     5922 1970-01-01 00:00:00.000000 dataconf-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0    16724 2023-05-23 22:08:58.125449 dataconf-2.2.0/LICENSE
+-rw-r--r--   0        0        0     4933 2023-05-23 22:08:58.125449 dataconf-2.2.0/README.md
+-rw-r--r--   0        0        0      685 2023-05-23 22:08:58.125449 dataconf-2.2.0/dataconf/__init__.py
+-rw-r--r--   0        0        0      871 2023-05-23 22:08:58.125449 dataconf-2.2.0/dataconf/cli.py
+-rw-r--r--   0        0        0      691 2023-05-23 22:08:58.125449 dataconf-2.2.0/dataconf/exceptions.py
+-rw-r--r--   0        0        0     4412 2023-05-23 22:08:58.125449 dataconf-2.2.0/dataconf/main.py
+-rw-r--r--   0        0        0       44 2023-05-23 22:08:58.125449 dataconf-2.2.0/dataconf/py.typed
+-rw-r--r--   0        0        0    11159 2023-05-23 22:08:58.125449 dataconf-2.2.0/dataconf/utils.py
+-rw-r--r--   0        0        0       22 2023-05-23 22:08:58.125449 dataconf-2.2.0/dataconf/version.py
+-rw-r--r--   0        0        0     1244 2023-05-23 22:08:58.125449 dataconf-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6083 1970-01-01 00:00:00.000000 dataconf-2.2.0/setup.py
+-rw-r--r--   0        0        0     5953 1970-01-01 00:00:00.000000 dataconf-2.2.0/PKG-INFO
```

### Comparing `dataconf-2.1.3/LICENSE` & `dataconf-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataconf-2.1.3/README.md` & `dataconf-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dataconf-2.1.3/dataconf/__init__.py` & `dataconf-2.2.0/dataconf/__init__.py`

 * *Files identical despite different names*

### Comparing `dataconf-2.1.3/dataconf/cli.py` & `dataconf-2.2.0/dataconf/cli.py`

 * *Files identical despite different names*

### Comparing `dataconf-2.1.3/dataconf/exceptions.py` & `dataconf-2.2.0/dataconf/exceptions.py`

 * *Files identical despite different names*

### Comparing `dataconf-2.1.3/dataconf/main.py` & `dataconf-2.2.0/dataconf/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import contextlib
 import os
-from typing import Any
+from typing import Any, Optional
 from typing import Dict
 from typing import List
 from typing import Type
 from urllib.parse import urlparse
 from urllib.request import urlopen
 
 from dataconf import utils
@@ -50,15 +50,14 @@
         return self.dict(data, **kwargs)
 
     def dict(self, obj: Dict[str, Any], **kwargs) -> "Multi":
         conf = ConfigFactory.from_dict(obj)
         return Multi(self.confs + [conf], self.strict, **kwargs)
 
     def string(self, s: str, loader: str = HOCON, **kwargs) -> "Multi":
-
         if loader == YAML:
             data = safe_load(s)
             return self.dict(data, **kwargs)
 
         conf = ConfigFactory.parse_string(s)
         return Multi(self.confs + [conf], self.strict, **kwargs)
 
@@ -68,16 +67,18 @@
             with contextlib.closing(urlopen(uri, timeout=timeout)) as fd:
                 s = fd.read().decode("utf-8")
             return self.string(s, loader=YAML, **kwargs)
 
         conf = ConfigFactory.parse_URL(uri, timeout=timeout, required=True)
         return Multi(self.confs + [conf], self.strict, **kwargs)
 
-    def file(self, path: str, **kwargs) -> "Multi":
-        if path.endswith(".yaml") or path.endswith(".yml"):
+    def file(self, path: str, loader: Optional[str] = None, **kwargs) -> "Multi":
+        if loader == YAML or (
+            loader is None and (path.endswith(".yaml") or path.endswith(".yml"))
+        ):
             with open(path, "r") as f:
                 data = safe_load(f)
             return self.dict(data, **kwargs)
 
         conf = ConfigFactory.parse_file(path)
         return Multi(self.confs + [conf], self.strict, **kwargs)
```

### Comparing `dataconf-2.1.3/dataconf/utils.py` & `dataconf-2.2.0/dataconf/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -45,25 +45,23 @@
 def is_optional(type: Type):
     # Optional = Union[T, NoneType]
     return get_origin(type) is Union and NoneType in get_args(type)
 
 
 def __parse(value: any, clazz: Type, path: str, strict: bool, ignore_unexpected: bool):
     if is_dataclass(clazz):
-
         if not isinstance(value, ConfigTree):
             raise TypeConfigException(
                 f"expected type {clazz} at {path}, got {type(value)}"
             )
 
         fs = {}
         renamings = dict()
 
         for f in fields(clazz):
-
             if f.name in value:
                 val = value[f.name]
             elif f.name.replace("_", "-") in value:
                 renamings[f.name] = f.name.replace("_", "-")
                 val = value[f.name.replace("_", "-")]
             else:
                 if callable(f.default_factory):
@@ -95,29 +93,33 @@
 
     origin = get_origin(clazz)
     args = get_args(clazz)
 
     if origin is list:
         if len(args) != 1:
             raise MissingTypeException("expected list with type information: List[?]")
+
         if value is not None:
+            parse_candidate = args[0]
             return [
-                __parse(v, args[0], f"{path}[]", strict, ignore_unexpected)
+                __parse(v, parse_candidate, f"{path}[]", strict, ignore_unexpected)
                 for v in value
             ]
         return None
 
     if origin is dict:
         if len(args) != 2:
             raise MissingTypeException(
                 "expected dict with type information: Dict[?, ?]"
             )
         if value is not None:
+            # ignore key type
+            parse_candidate = args[1]
             return {
-                k: __parse(v, args[1], f"{path}.{k}", strict, ignore_unexpected)
+                k: __parse(v, parse_candidate, f"{path}.{k}", strict, ignore_unexpected)
                 for k, v in value.items()
             }
         return None
 
     if is_optional(clazz):
         left, right = args
         try:
@@ -129,25 +131,23 @@
                 ignore_unexpected,
             )
         except TypeConfigException:
             # cannot parse Optional
             return None
 
     if origin is Union:
-        left, right = args
-
-        try:
-            return __parse(value, left, path, strict, ignore_unexpected)
-        except TypeConfigException as left_failure:
+        for parse_candidate in args:
             try:
-                return __parse(value, right, path, strict, ignore_unexpected)
-            except TypeConfigException as right_failure:
-                raise TypeConfigException(
-                    f"expected type {clazz} at {path}, failed both:\n- {left_failure}\n- {right_failure}"
-                )
+                return __parse(value, parse_candidate, path, strict, ignore_unexpected)
+            except TypeConfigException:
+                continue
+
+        raise TypeConfigException(
+            f"expected one of {', '.join(map(str, args))} at {path}, got {type(value)}"
+        )
 
     if clazz is bool:
         if not strict:
             try:
                 value = bool(value)
             except ValueError:
                 pass
@@ -179,20 +179,20 @@
             return dict(value)
 
         return value
 
     if isclass(clazz) and (issubclass(clazz, Enum) or issubclass(clazz, IntEnum)):
         if isinstance(value, int):
             return clazz.__call__(value)
+        elif issubclass(clazz, str):
+            return clazz(value)
         elif isinstance(value, str):
             return clazz.__getattr__(value)
-        else:
-            raise TypeConfigException(
-                f"expected str or int at {path}, got {type(value)}"
-            )
+
+        raise TypeConfigException(f"expected str or int at {path}, got {type(value)}")
 
     if clazz is datetime:
         dt = __parse_type(value, clazz, path, isinstance(value, str))
         try:
             return isoparse(dt)
         except ValueError as e:
             raise ParseException(
@@ -240,15 +240,14 @@
             f"expected type {clazz} at {path}, failed subclasses:\n- {failures}"
         )
 
     raise TypeConfigException(f"expected type {clazz} at {path}, got {type(value)}")
 
 
 def __generate(value: object, path: str):
-
     if is_dataclass(value):
         tree = {k: __generate(v, f"{path}.{k}") for k, v in asdict(value).items()}
         return ConfigTree(tree)
 
     if isinstance(value, dict):
         tree = {k: __generate(v, f"{path}.{k}") for k, v in value.items()}
         return ConfigTree(tree)
@@ -264,45 +263,42 @@
     return value
 
 
 def __env_vars_parse(prefix: str, obj: Dict[str, Any]):
     ret = {}
 
     def set_lens(p, focus, v):
-
         # value
         if len(p) == 1:
             # []x
             if isinstance(focus, list):
                 if p[0] != len(focus):
                     raise EnvListOrderException
                 focus.append(v)
             # {}x
             else:
                 focus[p[0]] = v
             return
 
         # dict
         if p[1] == "":
-
             if p[0] not in focus:
                 # []{x}
                 if isinstance(focus, list):
                     if p[0] != len(focus):
                         raise EnvListOrderException
                     focus.append({})
                 # {}{x}
                 else:
                     focus[p[0]] = {}
 
             return set_lens(p[2:], focus[p[0]], v)
 
         # list (only if the focus/value is already a list or if it starts with element 0)
         if isinstance(p[1], int) and (p[1] == 0 or isinstance(focus[p[0]], list)):
-
             if p[0] not in focus:
                 # [][x]
                 if isinstance(focus, list):
                     if p[1] != len(focus):
                         raise EnvListOrderException
                     focus.append([])
                 # {}[x]
```

### Comparing `dataconf-2.1.3/setup.py` & `dataconf-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 packages = \
 ['dataconf']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['PyYAML>=6.0,<7.0', 'pyhocon>=0.3.59,<0.4.0', 'python-dateutil>=2.8.2,<3.0.0']
+['PyYAML>=6.0,<7.0', 'pyhocon==0.3.60', 'python-dateutil>=2.8.2,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['dataconf = dataconf.cli:run']}
 
 setup_kwargs = {
     'name': 'dataconf',
-    'version': '2.1.3',
+    'version': '2.2.0',
     'description': 'Simple dataclasses configuration management for Python with hocon/json/yaml/properties/env-vars/dict support.',
     'long_description': '# Dataconf\n\n[![Actions Status](https://github.com/zifeo/dataconf/workflows/CI/badge.svg)](https://github.com/zifeo/dataconf/actions)\n[![PyPI version](https://badge.fury.io/py/dataconf.svg)](https://badge.fury.io/py/dataconf)\n\nSimple dataclasses configuration management for Python with\nhocon/json/yaml/properties/env-vars/dict/cli support.\n\n## Getting started\n\nRequires at least Python 3.8.\n\n```bash\n# pypi\npip install dataconf\npoetry add dataconf\n\n# remote master\npip install --upgrade git+https://github.com/zifeo/dataconf.git\npoetry add git+https://github.com/zifeo/dataconf.git\n\n# local repo/dev\npoetry install\npre-commit install\n```\n\n## Usage\n\n```python\nimport os\nfrom dataclasses import dataclass, field\nfrom typing import List, Dict, Text, Union\nfrom dateutil.relativedelta import relativedelta\nfrom datetime import datetime\nimport dataconf\n\nconf = """\nstr_name = test\nstr_name = ${?HOME}\ndash-to-underscore = true\nfloat_num = 2.2\niso_datetime = "2000-01-01T20:00:00"\n# this is a comment\nlist_data = [\n    a\n    b\n]\nnested {\n    a = test\n    b : 1\n}\nnested_list = [\n    {\n        a = test1\n        b : 2.5\n    }\n]\nduration = 2s\nunion = 1\npeople {\n    name = Thailand\n}\nzone {\n    area_code = 42\n}\n"""\n\nclass AbstractBaseClass:\n    pass\n    \n@dataclass\nclass Person(AbstractBaseClass):\n    name: Text\n        \n@dataclass\nclass Zone(AbstractBaseClass):\n    area_code: int\n\n@dataclass\nclass Nested:\n    a: Text\n    b: float\n\n@dataclass\nclass Config:\n    str_name: Text\n    dash_to_underscore: bool\n    float_num: float\n    iso_datetime: datetime\n    list_data: List[Text]\n    nested: Nested\n    nested_list: List[Nested]\n    duration: relativedelta\n    union: Union[Text, int]\n    people: AbstractBaseClass\n    zone: AbstractBaseClass\n    default: Text = \'hello\'\n    default_factory: Dict[Text, Text] = field(default_factory=dict)\n\nprint(dataconf.string(conf, Config))\n# Config(\n#   str_name=\'/users/root\',\n#   dash_to_underscore=True,\n#   float_num=2.2,\n#   list_data=[\'a\', \'b\'],\n#   nested=Nested(a=\'test\'),\n#   nested_list=[Nested(a=\'test1\', b=2.5)],\n#   duration=relativedelta(seconds=+2), \n#   union=1, \n#   people=Person(name=\'Thailand\'), \n#   zone=Zone(area_code=42),\n#   default=\'hello\', \n#   default_factory={}\n# )\n\n@dataclass\nclass Example:\n    hello: str\n    world: str\n    foo: List[str]\n\nos.environ[\'DC_WORLD\'] = \'monde\'\n\nprint(\n    dataconf\n    .multi\n    .url(\'https://raw.githubusercontent.com/zifeo/dataconf/main/confs/simple.hocon\')\n    .env(\'DC\')\n    .on(Example)\n)\n# Example(hello=\'bonjour\',world=\'monde\')\n```\n\n## API\n\n```python\nimport dataconf\n\nconf = dataconf.string(\'{ name: Test }\', Config)\nconf = dataconf.string(\'name:\\n\\tvalue: Test\', Config, loader=dataconf.YAML)  # dataconf.HOCON by default\nconf = dataconf.env(\'PREFIX_\', Config)\nconf = dataconf.dict({\'name\': \'Test\'}, Config)\nconf = dataconf.url(\'https://raw.githubusercontent.com/zifeo/dataconf/master/confs/test.hocon\', Config)  # hocon, json, yaml, properties\nconf = dataconf.file(\'confs/test.hocon\', Config)  # hocon, json, yaml, properties\nconf = dataconf.cli(sys.argv, Config)\n\n# Aggregation\nconf = dataconf.multi.string(...).env(...).url(...).file(...).dict(...).cli(...).on(Config)\n\n# Same api as Python json/yaml packages (e.g. `load`, `loads`, `dump`, `dumps`)\nconf = dataconf.load(\'confs/test.hocon\', Config)  # hocon, json, yaml, properties\nconf = dataconf.load(\'confs/test.yaml\', Config, loader=dataconf.YAML)  # dataconf.HOCON by default\ndataconf.dump(\'confs/test.hocon\', conf, out=\'hocon\')\ndataconf.dump(\'confs/test.json\', conf, out=\'json\')\ndataconf.dump(\'confs/test.yaml\', conf, out=\'yaml\')\ndataconf.dump(\'confs/test.properties\', conf, out=\'properties\')\n```\n\nFor full HOCON capabilities see\n[here](https://github.com/chimpler/pyhocon/#example-of-hocon-file).\n\n## Parse env vars\n\n```bash\nPREFIX_VAR=a\nPREFIX_VAR_NAME=b\nPREFIX_TEST__NAME=c\nPREFIX_LS_0=d\nPREFIX_LS_1=e\nPREFIX_LSLS_0_0=f\nPREFIX_LSOB_0__NAME=g\nPREFIX_NESTED_="{ name: Test }"\nPREFIX_SUB_="{ value: ${PREFIX_VAR} }"\n```\n\nis equivalent to\n\n```\n{\n    var = a\n    var_name = b\n    test {\n        name = c\n    }\n    ls = [\n        d\n        e\n    ]\n    lsls = [\n        [\n            f\n        ]\n    ]\n    lsob = [\n        {\n            name = g\n        }\n    ]\n    nested {\n        # parse nested config by suffixing env var with `_`\n        name: Test\n    }\n    sub {\n        # will have value "a" at parsing, useful for aliases\n        value = ${PREFIX_VAR}\n    }\n}\n```\n\nNote that when using `.env` source, the strict mode is disabled and value might\nbe casted.\n\n## Parse CLI arguments\n\nSame as env vars parse (dashes are converted to underscore, e.g. `TEST_A` →\n`--test-a`).\n\n## CLI usage\n\nCan be used for validation or converting between supported file formats (`-o`).\n\n```shell\ndataconf -c confs/test.hocon -m tests.configs -d TestConf -o hocon\n# dataconf.exceptions.TypeConfigException: expected type <class \'datetime.timedelta\'> at .duration, got <class \'int\'>\n```\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/zifeo/dataconf',
```

### Comparing `dataconf-2.1.3/PKG-INFO` & `dataconf-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: dataconf
-Version: 2.1.3
+Version: 2.2.0
 Summary: Simple dataclasses configuration management for Python with hocon/json/yaml/properties/env-vars/dict support.
 Home-page: https://github.com/zifeo/dataconf
-License: Apache2
+License: MPL-2.0
 Keywords: configuration,dataclasses,yaml,hocon,json,properties,cli,environment variables
 Requires-Python: >=3.8,<4.0
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: pyhocon (>=0.3.59,<0.4.0)
+Requires-Dist: pyhocon (==0.3.60)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Project-URL: Repository, https://github.com/zifeo/dataconf
 Description-Content-Type: text/markdown
 
 # Dataconf
 
 [![Actions Status](https://github.com/zifeo/dataconf/workflows/CI/badge.svg)](https://github.com/zifeo/dataconf/actions)
```

