# Comparing `tmp/classparse-0.1.3.tar.gz` & `tmp/classparse-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classparse-0.1.3.tar", last modified: Mon May 15 23:43:28 2023, max compression
+gzip compressed data, was "classparse-0.1.4.tar", last modified: Wed May 24 06:14:53 2023, max compression
```

## Comparing `classparse-0.1.3.tar` & `classparse-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-05-15 23:43:28.732604 classparse-0.1.3/
--rw-rw-r--   0 liran     (1000) liran     (1000)     5224 2023-05-09 12:28:19.000000 classparse-0.1.3/CODE_OF_CONDUCT.md
--rw-rw-r--   0 liran     (1000) liran     (1000)     1501 2023-05-15 23:42:57.000000 classparse-0.1.3/LICENSE
--rw-rw-r--   0 liran     (1000) liran     (1000)       78 2023-05-09 12:28:19.000000 classparse-0.1.3/MANIFEST.in
--rw-rw-r--   0 liran     (1000) liran     (1000)    16331 2023-05-15 23:43:28.732604 classparse-0.1.3/PKG-INFO
--rwxrwxr-x   0 liran     (1000) liran     (1000)    15664 2023-05-15 23:42:57.000000 classparse-0.1.3/README.md
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-05-15 23:43:28.732604 classparse-0.1.3/classparse/
--rw-rw-r--   0 liran     (1000) liran     (1000)    12692 2023-05-15 23:42:57.000000 classparse-0.1.3/classparse/__init__.py
--rw-rw-r--   0 liran     (1000) liran     (1000)     3140 2023-05-15 23:42:57.000000 classparse-0.1.3/classparse/docs.py
--rw-rw-r--   0 liran     (1000) liran     (1000)     9238 2023-05-15 23:42:57.000000 classparse-0.1.3/classparse/types.py
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-05-15 23:43:28.732604 classparse-0.1.3/classparse.egg-info/
--rw-rw-r--   0 liran     (1000) liran     (1000)    16331 2023-05-15 23:43:28.000000 classparse-0.1.3/classparse.egg-info/PKG-INFO
--rw-rw-r--   0 liran     (1000) liran     (1000)      294 2023-05-15 23:43:28.000000 classparse-0.1.3/classparse.egg-info/SOURCES.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)        1 2023-05-15 23:43:28.000000 classparse-0.1.3/classparse.egg-info/dependency_links.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)       73 2023-05-15 23:43:28.000000 classparse-0.1.3/classparse.egg-info/requires.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)       11 2023-05-15 23:43:28.000000 classparse-0.1.3/classparse.egg-info/top_level.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)     3134 2023-05-15 23:42:57.000000 classparse-0.1.3/pyproject.toml
--rw-rw-r--   0 liran     (1000) liran     (1000)       38 2023-05-15 23:43:28.732604 classparse-0.1.3/setup.cfg
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-05-24 06:14:53.293611 classparse-0.1.4/
+-rw-rw-r--   0 liran     (1000) liran     (1000)     5224 2023-05-09 12:28:19.000000 classparse-0.1.4/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1501 2023-05-24 06:08:35.000000 classparse-0.1.4/LICENSE
+-rw-rw-r--   0 liran     (1000) liran     (1000)       78 2023-05-09 12:28:19.000000 classparse-0.1.4/MANIFEST.in
+-rw-rw-r--   0 liran     (1000) liran     (1000)    16341 2023-05-24 06:14:53.293611 classparse-0.1.4/PKG-INFO
+-rwxrwxr-x   0 liran     (1000) liran     (1000)    15674 2023-05-24 06:08:35.000000 classparse-0.1.4/README.md
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-05-24 06:14:53.293611 classparse-0.1.4/classparse/
+-rw-rw-r--   0 liran     (1000) liran     (1000)    14505 2023-05-24 06:08:35.000000 classparse-0.1.4/classparse/__init__.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)     3140 2023-05-24 06:08:35.000000 classparse-0.1.4/classparse/docs.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)     9238 2023-05-24 06:08:35.000000 classparse-0.1.4/classparse/types.py
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-05-24 06:14:53.293611 classparse-0.1.4/classparse.egg-info/
+-rw-rw-r--   0 liran     (1000) liran     (1000)    16341 2023-05-24 06:14:53.000000 classparse-0.1.4/classparse.egg-info/PKG-INFO
+-rw-rw-r--   0 liran     (1000) liran     (1000)      294 2023-05-24 06:14:53.000000 classparse-0.1.4/classparse.egg-info/SOURCES.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)        1 2023-05-24 06:14:53.000000 classparse-0.1.4/classparse.egg-info/dependency_links.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)       79 2023-05-24 06:14:53.000000 classparse-0.1.4/classparse.egg-info/requires.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)       11 2023-05-24 06:14:53.000000 classparse-0.1.4/classparse.egg-info/top_level.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)     3188 2023-05-24 06:14:28.000000 classparse-0.1.4/pyproject.toml
+-rw-rw-r--   0 liran     (1000) liran     (1000)       38 2023-05-24 06:14:53.293611 classparse-0.1.4/setup.cfg
```

### Comparing `classparse-0.1.3/CODE_OF_CONDUCT.md` & `classparse-0.1.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `classparse-0.1.3/LICENSE` & `classparse-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `classparse-0.1.3/PKG-INFO` & `classparse-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classparse
-Version: 0.1.3
+Version: 0.1.4
 Summary: Declarative `ArgumentParser` definition with `dataclass` notation.
 Author-email: Liran Funaro <liran.funaro@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/liran-funaro/classparse
 Keywords: argparse,dataclass
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -50,27 +50,28 @@
 
 Declarative `ArgumentParser` definition with `dataclass` notation.
  - No `ArgumentParser` boilerplate code
  - IDE autocompletion and type hints
 
 # Install
 ```bash
-pip install classparse==0.1.3
+pip install classparse==0.1.4
 ```
 
 # Simple Example
 This is a simple example of the most basic usage of this library.
 <!-- embed: examples/simple.py -->
+
 ```python
 # examples/simple.py
 from dataclasses import dataclass
 
-from classparse import as_parser
+from classparse import classparser
 
-@as_parser
+@classparser
 @dataclass
 class SimpleArgs:
     """My simple program's arguments"""
 
     retries: int = 5  # number of retries
     eps: float = 1e-3  # epsilon
 
@@ -96,33 +97,34 @@
 $ python examples/simple.py --retries 10 --eps 1e-6
 SimpleArgs(retries=10, eps=1e-06)
 ```
 
 # Exhaustive Usage Example
 This example demonstrates all the usage scenarios of this library.
 <!-- embed: examples/usage.py -->
+
 ```python
 # examples/usage.py
 import dataclasses
 from dataclasses import dataclass
 from enum import Enum, auto
 from pathlib import Path
 from typing import List, Literal, Optional, Tuple, Union
 
-from classparse import arg, as_parser, no_arg, pos_arg, to_arg_name, to_var_name
+from classparse import arg, classparser, no_arg, pos_arg, to_arg_name, to_var_name
 
 class Action(Enum):
     Initialize = "init"
     Execute = "exec"
 
 class Animal(Enum):
     Cat = auto()
     Dog = auto()
 
-@as_parser(
+@classparser(
     prog="my_program.py",  # Keyword arguments are passed to the parser init.
     default_argument_args=dict(help="(type: %(type)s)"),  # Set default arguments for each call of add_argument().
 )
 @dataclass(frozen=True)
 class AllOptions:
     """
     Class doc string ==> parser description.
```

### Comparing `classparse-0.1.3/README.md` & `classparse-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,27 +32,28 @@
 
 Declarative `ArgumentParser` definition with `dataclass` notation.
  - No `ArgumentParser` boilerplate code
  - IDE autocompletion and type hints
 
 # Install
 ```bash
-pip install classparse==0.1.3
+pip install classparse==0.1.4
 ```
 
 # Simple Example
 This is a simple example of the most basic usage of this library.
 <!-- embed: examples/simple.py -->
+
 ```python
 # examples/simple.py
 from dataclasses import dataclass
 
-from classparse import as_parser
+from classparse import classparser
 
-@as_parser
+@classparser
 @dataclass
 class SimpleArgs:
     """My simple program's arguments"""
 
     retries: int = 5  # number of retries
     eps: float = 1e-3  # epsilon
 
@@ -78,33 +79,34 @@
 $ python examples/simple.py --retries 10 --eps 1e-6
 SimpleArgs(retries=10, eps=1e-06)
 ```
 
 # Exhaustive Usage Example
 This example demonstrates all the usage scenarios of this library.
 <!-- embed: examples/usage.py -->
+
 ```python
 # examples/usage.py
 import dataclasses
 from dataclasses import dataclass
 from enum import Enum, auto
 from pathlib import Path
 from typing import List, Literal, Optional, Tuple, Union
 
-from classparse import arg, as_parser, no_arg, pos_arg, to_arg_name, to_var_name
+from classparse import arg, classparser, no_arg, pos_arg, to_arg_name, to_var_name
 
 class Action(Enum):
     Initialize = "init"
     Execute = "exec"
 
 class Animal(Enum):
     Cat = auto()
     Dog = auto()
 
-@as_parser(
+@classparser(
     prog="my_program.py",  # Keyword arguments are passed to the parser init.
     default_argument_args=dict(help="(type: %(type)s)"),  # Set default arguments for each call of add_argument().
 )
 @dataclass(frozen=True)
 class AllOptions:
     """
     Class doc string ==> parser description.
```

### Comparing `classparse-0.1.3/classparse/__init__.py` & `classparse-0.1.4/classparse/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,37 +25,41 @@
 CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 POSSIBILITY OF SUCH DAMAGE.
 """
-import yaml
 import argparse
 import dataclasses
 import functools
 import typing
-from dataclasses import dataclass
 from types import MethodType
 from typing import (
     Any,
+    Callable,
     Dict,
+    Generic,
     Iterable,
     List,
     Optional,
+    Protocol,
     Sequence,
     Tuple,
     Type,
+    TypeVar,
     Union,
 )
 
+import yaml
+
 from classparse import docs
-from classparse.types import _update_field_type, _obj_to_yaml_dict, _yaml_dict_to_obj
+from classparse.types import _obj_to_yaml_dict, _update_field_type, _yaml_dict_to_obj
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 NO_ARG = "__no_arg__"
 POS_ARG = "__pos_arg__"
 
 
 def arg(flag=None, default=None, **metadata):
     """
     Allow adding parameters to a named argument.
@@ -95,33 +99,39 @@
     arg_name = to_arg_name(arg_name)
     if positional:
         assert flag is None, "Flag is not supported for positional argument"
         return [arg_name]
     return filter(None, [flag, f"--{arg_name}"])
 
 
-class DataclassParser(typing.Protocol):  # pragma: no cover
+T = TypeVar("T")
+
+
+class DataclassParser(Protocol[T]):  # pragma: no cover
+    def __new__(cls) -> Union["DataclassParser[T]", T]:
+        ...
+
     @classmethod
     def get_vars(cls) -> Dict[str, Any]:
         ...
 
     @classmethod
     def asdict(cls) -> Dict[str, Any]:
         ...
 
     @classmethod
-    def from_dict(cls, namespace: Dict[str, Any]) -> "DataclassParser":
+    def from_dict(cls, namespace: Dict[str, Any]) -> Union["DataclassParser[T]", T]:
         ...
 
     @classmethod
-    def dump_yaml(cls, stream=None, **kwargs) -> str:
+    def dump_yaml(cls, stream=None, **kwargs) -> Optional[str]:
         ...
 
     @classmethod
-    def load_yaml(cls, stream) -> "DataclassParser":
+    def load_yaml(cls, stream) -> Union["DataclassParser[T]", T]:
         ...
 
     @classmethod
     def get_parser(cls) -> argparse.ArgumentParser:
         ...
 
     @classmethod
@@ -137,51 +147,56 @@
         ...
 
     @classmethod
     def print_usage(cls, file=None):
         ...
 
     @classmethod
-    def parse_args(cls, args: Optional[Sequence[str]] = None) -> "DataclassParser":
+    def parse_args(cls, args: Optional[Sequence[str]] = None) -> Union["DataclassParser[T]", T]:
         ...
 
     @classmethod
-    def parse_intermixed_args(cls, args: Optional[Sequence[str]] = None) -> "DataclassParser":
+    def parse_intermixed_args(cls, args: Optional[Sequence[str]] = None) -> Union["DataclassParser[T]", T]:
         ...
 
     @classmethod
-    def parse_known_args(cls, args: Optional[Sequence[str]] = None) -> Tuple["DataclassParser", List[str]]:
+    def parse_known_args(cls, args: Optional[Sequence[str]] = None) -> Tuple[Union["DataclassParser[T]", T], List[str]]:
         ...
 
     @classmethod
-    def parse_known_intermixed_args(cls, args: Optional[Sequence[str]] = None) -> Tuple["DataclassParser", List[str]]:
+    def parse_known_intermixed_args(
+        cls, args: Optional[Sequence[str]] = None
+    ) -> Tuple[Union["DataclassParser[T]", T], List[str]]:
         ...
 
 
-class DataclassParserMaker:
-    def __init__(self, cls: dataclass, default_argument_args=None, **parser_args):
-        if not dataclasses.is_dataclass(cls):
-            raise TypeError("Cannot operate on a non-dataclass object.")
+DataClass = TypeVar("DataClass")
 
-        if not isinstance(cls, type):
-            cls = type(cls)
 
-        self.cls = cls
+class DataclassParserMaker(Generic[DataClass]):
+    def __init__(self, instance_or_cls: Union[Type[DataClass], DataClass], default_argument_args=None, **parser_args):
+        if not dataclasses.is_dataclass(instance_or_cls):
+            raise TypeError("Cannot operate on a non-dataclass object.")
+
+        if isinstance(instance_or_cls, type):
+            self.cls = instance_or_cls
+        else:
+            self.cls = type(instance_or_cls)
 
         if default_argument_args is None:
             default_argument_args = {}
         self.default_argument_args = default_argument_args
 
-        parser_args.setdefault("description", cls.__doc__)
+        parser_args.setdefault("description", self.cls.__doc__)
         self.parser_args = parser_args
 
-        self.docs = docs.get_argument_docs(cls)
+        self.docs = docs.get_argument_docs(self.cls)
         self.args = []
 
-        for field in dataclasses.fields(cls):
+        for field in dataclasses.fields(self.cls):
             self._add_argument_from_field(field)
 
         self.all_types = self._get_all_kwarg("type")
         self.all_defaults = self._get_all_kwarg("default")
         self.main_parser = self.make()
 
     def _get_all_kwarg(self, arg_name):
@@ -214,115 +229,126 @@
             kwargs["default"] = field.default
 
         # Fix field type to match work well with argparse
         _update_field_type(kwargs)
 
         self.args.append((field.name, args, kwargs))
 
-    def make(self, default_values: Union[dataclass, Dict[str, Any], None] = None):
+    def make(self, default_values: Optional[DataClass] = None) -> argparse.ArgumentParser:
         parser = argparse.ArgumentParser(**self.parser_args)
         if dataclasses.is_dataclass(default_values):
             default_values = dataclasses.asdict(default_values)
-        if isinstance(default_values, dict):
-            default_values = {to_var_name(k): v for k, v in default_values.items()}
-        if default_values is None:
+        else:
+            assert default_values is None
             default_values = {}
 
         for name, args, kwargs in self.args:
             if name in default_values:
                 kwargs = dict(kwargs, default=default_values[name])
             parser.add_argument(*args, **kwargs)
 
         return parser
 
-    def cast_to_class(self, namespace) -> dataclass:
+    def cast_to_class(self, namespace) -> Union[DataclassParser[DataClass], DataClass]:
         if not isinstance(namespace, dict):
             namespace = vars(namespace)
         return self.cls(**{to_var_name(k): v for k, v in namespace.items()})
 
-    def get_vars(self, instance_or_cls) -> Dict[str, Any]:
+    def get_vars(self, instance_or_cls: Union[Type[DataClass], DataClass]) -> Dict[str, Any]:
         if isinstance(instance_or_cls, type):
             return dict(self.all_defaults)
         else:
             return dataclasses.asdict(instance_or_cls)
 
-    def asdict(self, instance_or_cls) -> Dict[str, Any]:
+    def asdict(self, instance_or_cls: Union[Type[DataClass], DataClass]) -> Dict[str, Any]:
         return {to_arg_name(k): v for k, v in self.get_vars(instance_or_cls).items()}
 
-    def from_dict(self, instance_or_cls, namespace: Union[Any, Dict[str, Any]]) -> DataclassParser:
+    def from_dict(
+        self, instance_or_cls: Union[Type[DataClass], DataClass], namespace: Union[Any, Dict[str, Any]]
+    ) -> Union[DataclassParser[DataClass], DataClass]:
         if not isinstance(namespace, dict):
             namespace = vars(namespace)
 
         defaults = self.get_vars(instance_or_cls)
         iter_namespace = ((to_var_name(k), v) for k, v in namespace.items())
         defaults.update({k: v for k, v in iter_namespace if k in defaults})
         return self.cast_to_class(defaults)
 
-    def dump_yaml(self, instance_or_cls, stream=None, **kwargs) -> str:
+    def dump_yaml(self, instance_or_cls: Union[Type[DataClass], DataClass], stream=None, **kwargs) -> str:
         cur_vars = self.get_vars(instance_or_cls)
         cur_vars = _obj_to_yaml_dict(cur_vars)
         return yaml.safe_dump(cur_vars, stream=stream, **kwargs)
 
-    def load_yaml(self, instance_or_cls, stream) -> DataclassParser:
+    def load_yaml(
+        self, instance_or_cls: Union[Type[DataClass], DataClass], stream
+    ) -> Union[DataclassParser[DataClass], DataClass]:
         cur_vars = self.get_vars(instance_or_cls)
         loaded_vars = yaml.safe_load(stream)
         loaded_vars = _yaml_dict_to_obj(loaded_vars, self.all_types)
         cur_vars.update(loaded_vars)
         return self.cls(**cur_vars)
 
-    def _get_parser(self, instance_or_cls) -> argparse.ArgumentParser:
+    def _get_parser(self, instance_or_cls: Union[Type[DataClass], DataClass]) -> argparse.ArgumentParser:
         if isinstance(instance_or_cls, type):
             return self.main_parser
         else:
             return self.make(instance_or_cls)
 
-    def get_parser(self, instance_or_cls) -> argparse.ArgumentParser:
+    def get_parser(self, instance_or_cls: Union[Type[DataClass], DataClass]) -> argparse.ArgumentParser:
         return self.make(instance_or_cls if not isinstance(instance_or_cls, type) else None)
 
-    def format_help(self, instance_or_cls) -> str:
+    def format_help(self, instance_or_cls: Union[Type[DataClass], DataClass]) -> str:
         return self._get_parser(instance_or_cls).format_help()
 
-    def format_usage(self, instance_or_cls) -> str:
+    def format_usage(self, instance_or_cls: Union[Type[DataClass], DataClass]) -> str:
         return self._get_parser(instance_or_cls).format_usage()
 
-    def print_help(self, instance_or_cls, file=None):
+    def print_help(self, instance_or_cls: Union[Type[DataClass], DataClass], file=None):
         return self._get_parser(instance_or_cls).print_help(file)
 
-    def print_usage(self, instance_or_cls, file=None):
+    def print_usage(self, instance_or_cls: Union[Type[DataClass], DataClass], file=None):
         return self._get_parser(instance_or_cls).print_usage(file)
 
-    def parse_args(self, instance_or_cls, args: Optional[Sequence[str]] = None) -> DataclassParser:
+    def parse_args(
+        self, instance_or_cls: Union[Type[DataClass], DataClass], args: Optional[Sequence[str]] = None
+    ) -> Union[DataclassParser[DataClass], DataClass]:
         namespace = self._get_parser(instance_or_cls).parse_args(args=args)
         return self.cast_to_class(namespace)
 
-    def parse_intermixed_args(self, instance_or_cls, args: Optional[Sequence[str]] = None) -> DataclassParser:
+    def parse_intermixed_args(
+        self, instance_or_cls: Union[Type[DataClass], DataClass], args: Optional[Sequence[str]] = None
+    ) -> Union[DataclassParser[DataClass], DataClass]:
         namespace = self._get_parser(instance_or_cls).parse_intermixed_args(args=args)
         return self.cast_to_class(namespace)
 
     def parse_known_args(
-        self, instance_or_cls, args: Optional[Sequence[str]] = None
-    ) -> Tuple[DataclassParser, List[str]]:
+        self, instance_or_cls: Union[Type[DataClass], DataClass], args: Optional[Sequence[str]] = None
+    ) -> Tuple[Union[DataclassParser[DataClass], DataClass], List[str]]:
         namespace, args = self._get_parser(instance_or_cls).parse_known_args(args=args)
         return self.cast_to_class(namespace), args
 
     def parse_known_intermixed_args(
-        self, instance_or_cls, args: Optional[Sequence[str]] = None
-    ) -> Tuple[DataclassParser, List[str]]:
+        self, instance_or_cls: Union[Type[DataClass], DataClass], args: Optional[Sequence[str]] = None
+    ) -> Tuple[Union[DataclassParser[DataClass], DataClass], List[str]]:
         namespace, args = self._get_parser(instance_or_cls).parse_known_intermixed_args(args=args)
         return self.cast_to_class(namespace), args
 
 
-def make_parser(cls: dataclass, default_argument_args=None, **parser_args) -> argparse.ArgumentParser:
-    return DataclassParserMaker(cls, default_argument_args, **parser_args).main_parser
+def make_parser(
+    instance_or_cls: Union[Type[DataClass], DataClass], default_argument_args=None, **parser_args
+) -> argparse.ArgumentParser:
+    return DataclassParserMaker(instance_or_cls, default_argument_args, **parser_args).main_parser
 
 
-def parse_to(cls: dataclass, args=None, default_argument_args: dict = None, **parser_args) -> dataclass:
+def parse_to(
+    instance_or_cls: Union[Type[DataClass], DataClass], args=None, default_argument_args: dict = None, **parser_args
+) -> Union[DataclassParser[DataClass], DataClass]:
     """Parse arguments to a dataclass"""
-    parser_maker = DataclassParserMaker(cls, default_argument_args=default_argument_args, **parser_args)
-    return parser_maker.parse_args(cls, args=args)
+    parser_maker = DataclassParserMaker(instance_or_cls, default_argument_args=default_argument_args, **parser_args)
+    return parser_maker.parse_args(instance_or_cls, args=args)
 
 
 class ClassOrInstanceMethod:
     def __init__(self, f):
         self.f = f
         functools.update_wrapper(self, f)
 
@@ -335,24 +361,41 @@
 
 
 _dataclass_parser_methods: Tuple[str] = tuple(
     method_name for method_name in dir(DataclassParser) if not method_name.startswith("_")
 )
 
 
-def _wrap_dataclass(cls: dataclass, kwargs: Dict[str, Any]) -> Type[DataclassParser]:
+def _transform_dataclass_parser(
+    cls: Type[DataClass], /, kwargs: Dict[str, Any] = None
+) -> Union[Type[DataclassParser[DataClass]], Type[DataClass]]:
+    """Decorator that adds `DataclassParser` methods to the dataclass"""
+    kwargs = kwargs or {}
     parser_maker = DataclassParserMaker(cls, **kwargs)
     for method_name in _dataclass_parser_methods:
         setattr(cls, method_name, ClassOrInstanceMethod(getattr(parser_maker, method_name)))
     return cls
 
 
-def as_parser(cls=None, /, **kwargs):
+K = TypeVar("K")
+
+
+@typing.overload
+def classparser(**kwargs) -> Callable[[Type[K]], Union[Type[DataclassParser[K]], Type[K]]]:
+    ...  # pragma: no cover
+
+
+@typing.overload
+def classparser(cls: Type[DataClass]) -> Union[Type[DataclassParser[DataClass]], Type[DataClass]]:
+    ...  # pragma: no cover
+
+
+def classparser(cls=None, /, **kwargs):
     """Decorator that adds `DataclassParser` methods to the dataclass"""
-    if cls is not None:
-        return _wrap_dataclass(cls, kwargs)
-    else:
 
-        def decorator(container_class):
-            return _wrap_dataclass(container_class, kwargs)
+    # See if we're being called as @dataclass_parser or @dataclass_parser().
+    if cls is None:
+        # We're called with parens.
+        return functools.partial(_transform_dataclass_parser, kwargs=kwargs)
 
-        return decorator
+    # We're called as @dataclass_parser without parens.
+    return _transform_dataclass_parser(cls, kwargs)
```

### Comparing `classparse-0.1.3/classparse/docs.py` & `classparse-0.1.4/classparse/docs.py`

 * *Files identical despite different names*

### Comparing `classparse-0.1.3/classparse/types.py` & `classparse-0.1.4/classparse/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 POSSIBILITY OF SUCH DAMAGE.
 """
 import argparse
 import enum
 import functools
 import itertools
 import typing
-from typing import Any, Dict, List, Literal, Optional, Tuple, Type, Union, Callable
+from typing import Any, Callable, Dict, List, Literal, Optional, Tuple, Type, Union
 
 _TYPE_RECURSION_LIMIT = 1024
 
 
 @functools.wraps(bool)
 def __parse_bool(x):
     _x = str(x).lower().strip()
```

### Comparing `classparse-0.1.3/classparse.egg-info/PKG-INFO` & `classparse-0.1.4/classparse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classparse
-Version: 0.1.3
+Version: 0.1.4
 Summary: Declarative `ArgumentParser` definition with `dataclass` notation.
 Author-email: Liran Funaro <liran.funaro@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/liran-funaro/classparse
 Keywords: argparse,dataclass
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -50,27 +50,28 @@
 
 Declarative `ArgumentParser` definition with `dataclass` notation.
  - No `ArgumentParser` boilerplate code
  - IDE autocompletion and type hints
 
 # Install
 ```bash
-pip install classparse==0.1.3
+pip install classparse==0.1.4
 ```
 
 # Simple Example
 This is a simple example of the most basic usage of this library.
 <!-- embed: examples/simple.py -->
+
 ```python
 # examples/simple.py
 from dataclasses import dataclass
 
-from classparse import as_parser
+from classparse import classparser
 
-@as_parser
+@classparser
 @dataclass
 class SimpleArgs:
     """My simple program's arguments"""
 
     retries: int = 5  # number of retries
     eps: float = 1e-3  # epsilon
 
@@ -96,33 +97,34 @@
 $ python examples/simple.py --retries 10 --eps 1e-6
 SimpleArgs(retries=10, eps=1e-06)
 ```
 
 # Exhaustive Usage Example
 This example demonstrates all the usage scenarios of this library.
 <!-- embed: examples/usage.py -->
+
 ```python
 # examples/usage.py
 import dataclasses
 from dataclasses import dataclass
 from enum import Enum, auto
 from pathlib import Path
 from typing import List, Literal, Optional, Tuple, Union
 
-from classparse import arg, as_parser, no_arg, pos_arg, to_arg_name, to_var_name
+from classparse import arg, classparser, no_arg, pos_arg, to_arg_name, to_var_name
 
 class Action(Enum):
     Initialize = "init"
     Execute = "exec"
 
 class Animal(Enum):
     Cat = auto()
     Dog = auto()
 
-@as_parser(
+@classparser(
     prog="my_program.py",  # Keyword arguments are passed to the parser init.
     default_argument_args=dict(help="(type: %(type)s)"),  # Set default arguments for each call of add_argument().
 )
 @dataclass(frozen=True)
 class AllOptions:
     """
     Class doc string ==> parser description.
```

### Comparing `classparse-0.1.3/pyproject.toml` & `classparse-0.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -26,17 +26,20 @@
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools]
+packages = ["classparse"]
+
 [project]
 name = "classparse"
-version = "0.1.3"
+version = "0.1.4"
 description = "Declarative `ArgumentParser` definition with `dataclass` notation."
 readme = "README.md"
 authors = [{ name = "Liran Funaro", email = "liran.funaro@gmail.com" }]
 license = { text = "BSD-3-Clause" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -45,21 +48,21 @@
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 keywords = ["argparse", "dataclass"]
 dependencies = ["PyYAML"]
 requires-python = ">=3.8"
 
 [project.optional-dependencies]
-dev = ["bumpver", "black", "flake8", "pip-tools", "pytest", "pytest-cov", "coveralls"]
+dev = ["bumpver", "black", "isort", "flake8", "pip-tools", "pytest", "pytest-cov", "coveralls"]
 
 [project.urls]
 Homepage = "https://github.com/liran-funaro/classparse"
 
 [tool.bumpver]
-current_version = "0.1.3"
+current_version = "0.1.4"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

