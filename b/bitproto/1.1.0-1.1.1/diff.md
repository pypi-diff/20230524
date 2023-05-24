# Comparing `tmp/bitproto-1.1.0.tar.gz` & `tmp/bitproto-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitproto-1.1.0.tar", last modified: Mon Jan  2 14:13:14 2023, max compression
+gzip compressed data, was "bitproto-1.1.1.tar", last modified: Wed May 24 15:39:55 2023, max compression
```

## Comparing `bitproto-1.1.0.tar` & `bitproto-1.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-01-02 14:13:14.853390 bitproto-1.1.0/
--rw-r--r--   0 hit9       (501) staff       (20)      262 2021-07-23 03:17:35.000000 bitproto-1.1.0/MANIFEST.in
--rw-r--r--   0 hit9       (501) staff       (20)     1443 2023-01-02 14:13:14.852934 bitproto-1.1.0/PKG-INFO
-drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-01-02 14:13:14.836675 bitproto-1.1.0/bitproto/
--rw-r--r--   0 hit9       (501) staff       (20)      200 2023-01-02 14:12:08.000000 bitproto-1.1.0/bitproto/__init__.py
--rw-r--r--   0 hit9       (501) staff       (20)    30841 2022-12-27 14:27:49.000000 bitproto-1.1.0/bitproto/_ast.py
--rw-r--r--   0 hit9       (501) staff       (20)     4925 2022-12-27 14:27:49.000000 bitproto-1.1.0/bitproto/_main.py
--rw-r--r--   0 hit9       (501) staff       (20)     8721 2022-12-27 14:27:49.000000 bitproto-1.1.0/bitproto/errors.py
--rw-r--r--   0 hit9       (501) staff       (20)     5971 2022-10-03 09:14:09.000000 bitproto-1.1.0/bitproto/grammars.py
--rw-r--r--   0 hit9       (501) staff       (20)     5644 2022-12-26 12:00:41.000000 bitproto-1.1.0/bitproto/lexer.py
--rw-r--r--   0 hit9       (501) staff       (20)     7416 2022-12-27 14:27:49.000000 bitproto-1.1.0/bitproto/linter.py
--rw-r--r--   0 hit9       (501) staff       (20)     1411 2022-12-27 14:27:49.000000 bitproto-1.1.0/bitproto/options.py
--rw-r--r--   0 hit9       (501) staff       (20)    25028 2022-12-13 15:00:12.000000 bitproto-1.1.0/bitproto/parser.py
-drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-01-02 14:13:14.840115 bitproto-1.1.0/bitproto/renderer/
--rw-r--r--   0 hit9       (501) staff       (20)      982 2022-12-13 15:00:12.000000 bitproto-1.1.0/bitproto/renderer/__init__.py
--rw-r--r--   0 hit9       (501) staff       (20)    16560 2022-12-13 15:00:12.000000 bitproto-1.1.0/bitproto/renderer/block.py
--rw-r--r--   0 hit9       (501) staff       (20)    27712 2022-12-13 15:00:12.000000 bitproto-1.1.0/bitproto/renderer/formatter.py
-drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-01-02 14:13:14.841720 bitproto-1.1.0/bitproto/renderer/impls/
--rw-r--r--   0 hit9       (501) staff       (20)      373 2022-12-13 15:00:12.000000 bitproto-1.1.0/bitproto/renderer/impls/__init__.py
-drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-01-02 14:13:14.848143 bitproto-1.1.0/bitproto/renderer/impls/c/
--rw-r--r--   0 hit9       (501) staff       (20)      118 2022-12-13 15:00:12.000000 bitproto-1.1.0/bitproto/renderer/impls/c/__init__.py
--rw-r--r--   0 hit9       (501) staff       (20)    14249 2023-01-02 14:12:08.000000 bitproto-1.1.0/bitproto/renderer/impls/c/formatter.py
--rw-r--r--   0 hit9       (501) staff       (20)    15739 2022-12-13 15:00:12.000000 bitproto-1.1.0/bitproto/renderer/impls/c/renderer_c.py
--rw-r--r--   0 hit9       (501) staff       (20)    16509 2022-12-13 15:00:12.000000 bitproto-1.1.0/bitproto/renderer/impls/c/renderer_h.py
-drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-01-02 14:13:14.850171 bitproto-1.1.0/bitproto/renderer/impls/go/
--rw-r--r--   0 hit9       (501) staff       (20)       60 2022-12-13 15:00:12.000000 bitproto-1.1.0/bitproto/renderer/impls/go/__init__.py
--rw-r--r--   0 hit9       (501) staff       (20)     8549 2022-12-13 15:00:12.000000 bitproto-1.1.0/bitproto/renderer/impls/go/formatter.py
--rw-r--r--   0 hit9       (501) staff       (20)    29070 2022-12-13 15:00:12.000000 bitproto-1.1.0/bitproto/renderer/impls/go/renderer.py
-drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-01-02 14:13:14.851817 bitproto-1.1.0/bitproto/renderer/impls/py/
--rw-r--r--   0 hit9       (501) staff       (20)       60 2022-12-13 15:00:12.000000 bitproto-1.1.0/bitproto/renderer/impls/py/__init__.py
--rw-r--r--   0 hit9       (501) staff       (20)     9205 2022-10-03 09:14:09.000000 bitproto-1.1.0/bitproto/renderer/impls/py/formatter.py
--rw-r--r--   0 hit9       (501) staff       (20)    29359 2023-01-02 14:12:08.000000 bitproto-1.1.0/bitproto/renderer/impls/py/renderer.py
--rw-r--r--   0 hit9       (501) staff       (20)     4008 2022-12-13 15:00:12.000000 bitproto-1.1.0/bitproto/renderer/renderer.py
--rw-r--r--   0 hit9       (501) staff       (20)    10654 2022-12-27 14:27:49.000000 bitproto-1.1.0/bitproto/utils.py
-drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-01-02 14:13:14.852394 bitproto-1.1.0/bitproto.egg-info/
--rw-r--r--   0 hit9       (501) staff       (20)      789 2023-01-02 14:13:14.000000 bitproto-1.1.0/bitproto.egg-info/SOURCES.txt
--rw-r--r--   0 hit9       (501) staff       (20)       57 2022-12-13 15:00:12.000000 bitproto-1.1.0/pyproject.toml
--rw-r--r--   0 hit9       (501) staff       (20)       35 2021-01-28 05:09:09.000000 bitproto-1.1.0/requirements.txt
--rw-r--r--   0 hit9       (501) staff       (20)       38 2023-01-02 14:13:14.853535 bitproto-1.1.0/setup.cfg
--rw-r--r--   0 hit9       (501) staff       (20)     2019 2022-12-27 14:27:49.000000 bitproto-1.1.0/setup.py
+drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-05-24 15:39:55.518050 bitproto-1.1.1/
+-rw-r--r--   0 hit9       (501) staff       (20)      262 2021-07-23 03:17:35.000000 bitproto-1.1.1/MANIFEST.in
+-rw-r--r--   0 hit9       (501) staff       (20)     1442 2023-05-24 15:39:55.517695 bitproto-1.1.1/PKG-INFO
+drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-05-24 15:39:55.506541 bitproto-1.1.1/bitproto/
+-rw-r--r--   0 hit9       (501) staff       (20)      200 2023-05-24 15:34:03.000000 bitproto-1.1.1/bitproto/__init__.py
+-rw-r--r--   0 hit9       (501) staff       (20)    30840 2023-05-23 02:36:38.000000 bitproto-1.1.1/bitproto/_ast.py
+-rw-r--r--   0 hit9       (501) staff       (20)     4925 2022-12-27 14:27:49.000000 bitproto-1.1.1/bitproto/_main.py
+-rw-r--r--   0 hit9       (501) staff       (20)     8721 2022-12-27 14:27:49.000000 bitproto-1.1.1/bitproto/errors.py
+-rw-r--r--   0 hit9       (501) staff       (20)     5971 2022-10-03 09:14:09.000000 bitproto-1.1.1/bitproto/grammars.py
+-rw-r--r--   0 hit9       (501) staff       (20)     5644 2022-12-26 12:00:41.000000 bitproto-1.1.1/bitproto/lexer.py
+-rw-r--r--   0 hit9       (501) staff       (20)     7415 2023-05-24 15:34:03.000000 bitproto-1.1.1/bitproto/linter.py
+-rw-r--r--   0 hit9       (501) staff       (20)     1411 2022-12-27 14:27:49.000000 bitproto-1.1.1/bitproto/options.py
+-rw-r--r--   0 hit9       (501) staff       (20)    25028 2022-12-13 15:00:12.000000 bitproto-1.1.1/bitproto/parser.py
+drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-05-24 15:39:55.508513 bitproto-1.1.1/bitproto/renderer/
+-rw-r--r--   0 hit9       (501) staff       (20)      982 2022-12-13 15:00:12.000000 bitproto-1.1.1/bitproto/renderer/__init__.py
+-rw-r--r--   0 hit9       (501) staff       (20)    16560 2022-12-13 15:00:12.000000 bitproto-1.1.1/bitproto/renderer/block.py
+-rw-r--r--   0 hit9       (501) staff       (20)    27843 2023-05-24 15:34:03.000000 bitproto-1.1.1/bitproto/renderer/formatter.py
+drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-05-24 15:39:55.508965 bitproto-1.1.1/bitproto/renderer/impls/
+-rw-r--r--   0 hit9       (501) staff       (20)      373 2022-12-13 15:00:12.000000 bitproto-1.1.1/bitproto/renderer/impls/__init__.py
+drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-05-24 15:39:55.511162 bitproto-1.1.1/bitproto/renderer/impls/c/
+-rw-r--r--   0 hit9       (501) staff       (20)      118 2022-12-13 15:00:12.000000 bitproto-1.1.1/bitproto/renderer/impls/c/__init__.py
+-rw-r--r--   0 hit9       (501) staff       (20)    14249 2023-01-02 14:12:08.000000 bitproto-1.1.1/bitproto/renderer/impls/c/formatter.py
+-rw-r--r--   0 hit9       (501) staff       (20)    15739 2022-12-13 15:00:12.000000 bitproto-1.1.1/bitproto/renderer/impls/c/renderer_c.py
+-rw-r--r--   0 hit9       (501) staff       (20)    16509 2022-12-13 15:00:12.000000 bitproto-1.1.1/bitproto/renderer/impls/c/renderer_h.py
+drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-05-24 15:39:55.512669 bitproto-1.1.1/bitproto/renderer/impls/go/
+-rw-r--r--   0 hit9       (501) staff       (20)       60 2022-12-13 15:00:12.000000 bitproto-1.1.1/bitproto/renderer/impls/go/__init__.py
+-rw-r--r--   0 hit9       (501) staff       (20)     8549 2022-12-13 15:00:12.000000 bitproto-1.1.1/bitproto/renderer/impls/go/formatter.py
+-rw-r--r--   0 hit9       (501) staff       (20)    29183 2023-05-24 15:34:03.000000 bitproto-1.1.1/bitproto/renderer/impls/go/renderer.py
+drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-05-24 15:39:55.516536 bitproto-1.1.1/bitproto/renderer/impls/py/
+-rw-r--r--   0 hit9       (501) staff       (20)       60 2022-12-13 15:00:12.000000 bitproto-1.1.1/bitproto/renderer/impls/py/__init__.py
+-rw-r--r--   0 hit9       (501) staff       (20)     9205 2022-10-03 09:14:09.000000 bitproto-1.1.1/bitproto/renderer/impls/py/formatter.py
+-rw-r--r--   0 hit9       (501) staff       (20)    29359 2023-05-22 13:19:23.000000 bitproto-1.1.1/bitproto/renderer/impls/py/renderer.py
+-rw-r--r--   0 hit9       (501) staff       (20)     4008 2022-12-13 15:00:12.000000 bitproto-1.1.1/bitproto/renderer/renderer.py
+-rw-r--r--   0 hit9       (501) staff       (20)    10653 2023-05-24 15:34:03.000000 bitproto-1.1.1/bitproto/utils.py
+drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-05-24 15:39:55.517202 bitproto-1.1.1/bitproto.egg-info/
+-rw-r--r--   0 hit9       (501) staff       (20)      789 2023-05-24 15:39:55.000000 bitproto-1.1.1/bitproto.egg-info/SOURCES.txt
+-rw-r--r--   0 hit9       (501) staff       (20)       57 2022-12-13 15:00:12.000000 bitproto-1.1.1/pyproject.toml
+-rw-r--r--   0 hit9       (501) staff       (20)       35 2021-01-28 05:09:09.000000 bitproto-1.1.1/requirements.txt
+-rw-r--r--   0 hit9       (501) staff       (20)       38 2023-05-24 15:39:55.518185 bitproto-1.1.1/setup.cfg
+-rw-r--r--   0 hit9       (501) staff       (20)     2018 2023-05-23 02:36:38.000000 bitproto-1.1.1/setup.py
```

### Comparing `bitproto-1.1.0/PKG-INFO` & `bitproto-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitproto
-Version: 1.1.0
+Version: 1.1.1
 Summary: bit level data interchange format.
 Home-page: https://github.com/hit9/bitproto
 Author: Chao Wang
 Author-email: hit9@icloud.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -25,15 +25,15 @@
 Bitproto is a fast, lightweight and easy-to-use bit level data
 interchange format for serializing data structures.
 
 Features
 ---------
 
 - Supports bit level data serialization.
-- Supports protocol extensiblity, for backward-compatibility.
+- Supports protocol extensiblity, for forward-compatibility.
 - Very easy to start
 
   - Protocol syntax is similar to the well-known protobuf.
   - Generating code with very simple serialization api.
 
 - Supports the following languages
```

### Comparing `bitproto-1.1.0/bitproto/_ast.py` & `bitproto-1.1.1/bitproto/_ast.py`

 * *Files 0% similar despite different names*

```diff
@@ -732,15 +732,15 @@
 
     def __repr__(self) -> str:
         return "<type int{0}>".format(self.cap)
 
 
 @dataclass
 class ExtensibleType(Type):
-    """ExtensibleType is the type able to extend its size for backward-compatiable
+    """ExtensibleType is the type able to extend its size for forward-compatiable
     concern. When setting the `extensible` parameter to True, a micro buffer that
     indicates the type size will be inserted at the head of encoded buffer.
     In bitproto, array, enum and message are extensible types.
     """
 
     extensible: bool = False
```

### Comparing `bitproto-1.1.0/bitproto/_main.py` & `bitproto-1.1.1/bitproto/_main.py`

 * *Files identical despite different names*

### Comparing `bitproto-1.1.0/bitproto/errors.py` & `bitproto-1.1.1/bitproto/errors.py`

 * *Files identical despite different names*

### Comparing `bitproto-1.1.0/bitproto/grammars.py` & `bitproto-1.1.1/bitproto/grammars.py`

 * *Files identical despite different names*

### Comparing `bitproto-1.1.0/bitproto/lexer.py` & `bitproto-1.1.1/bitproto/lexer.py`

 * *Files identical despite different names*

### Comparing `bitproto-1.1.0/bitproto/linter.py` & `bitproto-1.1.1/bitproto/linter.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,14 @@
 
     def lint(self, proto: Proto) -> int:
         """Run lint rules for definitions bound to this proto.
         Returns number of warning reported.
         """
         warning_count: int = 0
         for definition_type in SUPPORTED_TYPES:
-
             items: List[Tuple[str, Definition]]
             if definition_type is Proto:  # proto is not a member of itself.
                 items = [(proto.name, proto)]
             else:
                 items = proto.filter(definition_type, recursive=True, bound=proto)
 
             rules = self.filter_rules(definition_type)
```

### Comparing `bitproto-1.1.0/bitproto/options.py` & `bitproto-1.1.1/bitproto/options.py`

 * *Files identical despite different names*

### Comparing `bitproto-1.1.0/bitproto/parser.py` & `bitproto-1.1.1/bitproto/parser.py`

 * *Files identical despite different names*

### Comparing `bitproto-1.1.0/bitproto/renderer/__init__.py` & `bitproto-1.1.1/bitproto/renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `bitproto-1.1.0/bitproto/renderer/block.py` & `bitproto-1.1.1/bitproto/renderer/block.py`

 * *Files identical despite different names*

### Comparing `bitproto-1.1.0/bitproto/renderer/formatter.py` & `bitproto-1.1.1/bitproto/renderer/formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 
 # Dict[DefinitionType => One or tuple of CaseStyle name OR CaseStyleConverter]
 CaseStyleMapping = Dict[T[Definition], Union[str, Tuple[str, ...], CaseStyleConverter]]
 
 
 @unique
 class CaseStyle(Enum_):
-
     KEEP = 0
     SNAKE = 1
     UPPER = 2
     PASCAL = 3
 
     def converter(self) -> CaseStyleConverter:
         """Returns the case converter function."""
@@ -397,25 +396,31 @@
     def format_definition_name(
         self, d: Definition, class_: Optional[T[Definition]] = None
     ) -> str:
         """Formats the declaration name for given definition in target language.
         Joins a with a dot delimer if given definition is a definition imported.
         """
         definition_name = self.format_definition_name_inner_proto(d, class_)
-        protos = [scope for scope in d.scope_stack if isinstance(scope, Proto)]
 
-        if len(protos) <= 1:
+        parent = d.scope_stack[-1]
+
+        if not isinstance(parent, Proto):
+            # Member of Non-Proto scopes: message, enum etc.
             return definition_name
 
         if not self.support_import_as_member():
             return definition_name
 
-        proto = protos[-1]  # Last is the imported parent.
-        items = [self._get_definition_name(proto), definition_name]
-        return self.delimer_cross_proto().join(items)
+        if not parent.scope_stack:
+            # `parent` is the top proto.
+            return definition_name
+        # `parent` is imported in another proto.
+        return self.delimer_cross_proto().join(
+            [self._get_definition_name(parent), definition_name]
+        )
 
     @final
     def format_name_related_to_definition(
         self, d: Definition, fmt: str, class_: Optional[T[Definition]] = None
     ) -> str:
         """Format a name related to given definition d from given formatter fmt.
         Example fmt: 'XXX{definition_name}'.
```

### Comparing `bitproto-1.1.0/bitproto/renderer/impls/c/formatter.py` & `bitproto-1.1.1/bitproto/renderer/impls/c/formatter.py`

 * *Files identical despite different names*

### Comparing `bitproto-1.1.0/bitproto/renderer/impls/c/renderer_c.py` & `bitproto-1.1.1/bitproto/renderer/impls/c/renderer_c.py`

 * *Files identical despite different names*

### Comparing `bitproto-1.1.0/bitproto/renderer/impls/c/renderer_h.py` & `bitproto-1.1.1/bitproto/renderer/impls/c/renderer_h.py`

 * *Files identical despite different names*

### Comparing `bitproto-1.1.0/bitproto/renderer/impls/go/formatter.py` & `bitproto-1.1.1/bitproto/renderer/impls/go/formatter.py`

 * *Files identical despite different names*

### Comparing `bitproto-1.1.0/bitproto/renderer/impls/go/renderer.py` & `bitproto-1.1.1/bitproto/renderer/impls/go/renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,21 +50,14 @@
         self.push(f"import (")
         self.push(f'"strconv"', indent=1)
         self.push(f'"encoding/json"', indent=1)
         self.push_empty_line()
         self.push(f'bp "{GO_LIB_IMPORT_PATH}"', indent=1)
         self.push(f")")
 
-        self.push_empty_line()
-
-        self.push_comment("Avoid possible golang import not used error")
-        self.push(f"var formatInt = strconv.FormatInt")
-        self.push(f"var jsonMarshal = json.Marshal")
-        self.push(f"var _ = bp.Useless")
-
 
 class BlockImportChildProto(BlockBindProto[F]):
     @override(Block)
     def render(self) -> None:
         self.push(self.formatter.format_import_statement(self.d, as_name=self.name))
 
 
@@ -77,14 +70,23 @@
         ]
 
     @override(BlockComposition)
     def separator(self) -> str:
         return "\n"
 
 
+class BlockAvoidGeneralImportsNotUsed(Block):
+    @override(Block)
+    def render(self) -> None:
+        self.push_comment("Avoid possible golang import not used error")
+        self.push(f"var formatInt = strconv.FormatInt")
+        self.push(f"var jsonMarshal = json.Marshal")
+        self.push(f"var _ = bp.Useless")
+
+
 class BlockAliasMethodBase(BlockBindAlias[F]):
     @cached_property
     def method_receiver(self) -> str:
         if isinstance(self.d.type, Message):
             return f"*{self.alias_name}"
         return f"{self.alias_name}"
 
@@ -746,14 +748,15 @@
     @override(BlockComposition)
     def blocks(self) -> List[Block[F]]:
         return [
             BlockAheadNotice(),
             BlockPackageName(self.bound),
             BlockGeneralImports(),
             BlockImportChildProtoList(),
+            BlockAvoidGeneralImportsNotUsed(),
             BlockBoundDefinitionList(),
         ]
 
 
 class BlockGeneralImportsOpMode(Block):
     @override(Block)
     def render(self) -> None:
```

### Comparing `bitproto-1.1.0/bitproto/renderer/impls/py/formatter.py` & `bitproto-1.1.1/bitproto/renderer/impls/py/formatter.py`

 * *Files identical despite different names*

### Comparing `bitproto-1.1.0/bitproto/renderer/impls/py/renderer.py` & `bitproto-1.1.1/bitproto/renderer/impls/py/renderer.py`

 * *Files identical despite different names*

### Comparing `bitproto-1.1.0/bitproto/renderer/renderer.py` & `bitproto-1.1.1/bitproto/renderer/renderer.py`

 * *Files identical despite different names*

### Comparing `bitproto-1.1.0/bitproto/utils.py` & `bitproto-1.1.1/bitproto/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,14 @@
 
         setattr(class_, "__frozen__", False)
         setattr(class_, "freeze", freeze)
         setattr(class_, "__setattr__", __setattr__)
         setattr(class_, "__delattr__", __delattr__)
 
         if post_init:
-
             init_func = getattr(class_, "__init__")
 
             def decorate_init(func):
                 @wraps(func)
                 def decorated(class_self, *args, **kwds):
                     ret = func(class_self, *args, **kwds)
                     class_self.freeze()
```

### Comparing `bitproto-1.1.0/bitproto.egg-info/SOURCES.txt` & `bitproto-1.1.1/bitproto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bitproto-1.1.0/setup.py` & `bitproto-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 Bitproto is a fast, lightweight and easy-to-use bit level data
 interchange format for serializing data structures.
 
 Features
 ---------
 
 - Supports bit level data serialization.
-- Supports protocol extensiblity, for backward-compatibility.
+- Supports protocol extensiblity, for forward-compatibility.
 - Very easy to start
 
   - Protocol syntax is similar to the well-known protobuf.
   - Generating code with very simple serialization api.
 
 - Supports the following languages
```

