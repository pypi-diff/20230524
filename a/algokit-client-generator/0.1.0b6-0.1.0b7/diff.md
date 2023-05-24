# Comparing `tmp/algokit_client_generator-0.1.0b6-py3-none-any.whl.zip` & `tmp/algokit_client_generator-0.1.0b7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 15669 bytes, number of entries: 14
--rw-r--r--  2.0 unx      179 b- defN 80-Jan-01 00:00 algokit_client_generator/__init__.py
+Zip file size: 16361 bytes, number of entries: 14
+-rw-r--r--  2.0 unx       91 b- defN 80-Jan-01 00:00 algokit_client_generator/__init__.py
 -rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 algokit_client_generator/__main__.py
--rw-r--r--  2.0 unx     2132 b- defN 80-Jan-01 00:00 algokit_client_generator/cli.py
+-rw-r--r--  2.0 unx     2550 b- defN 80-Jan-01 00:00 algokit_client_generator/cli.py
 -rw-r--r--  2.0 unx     3199 b- defN 80-Jan-01 00:00 algokit_client_generator/document.py
--rw-r--r--  2.0 unx    23029 b- defN 80-Jan-01 00:00 algokit_client_generator/generator.py
+-rw-r--r--  2.0 unx    26188 b- defN 80-Jan-01 00:00 algokit_client_generator/generator.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_client_generator/py.typed
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_client_generator/spec.py
 -rw-r--r--  2.0 unx     4303 b- defN 80-Jan-01 00:00 algokit_client_generator/utils.py
--rw-r--r--  2.0 unx      890 b- defN 80-Jan-01 00:00 algokit_client_generator/writer.py
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b6.dist-info/LICENSE
--rw-r--r--  2.0 unx     4585 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b6.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b6.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b6.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1299 b- defN 16-Jan-01 00:00 algokit_client_generator-0.1.0b6.dist-info/RECORD
-14 files, 48367 bytes uncompressed, 13453 bytes compressed:  72.2%
+-rw-r--r--  2.0 unx      995 b- defN 80-Jan-01 00:00 algokit_client_generator/writer.py
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4585 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b7.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b7.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1298 b- defN 16-Jan-01 00:00 algokit_client_generator-0.1.0b7.dist-info/RECORD
+14 files, 51960 bytes uncompressed, 14145 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: algokit_client_generator/utils.py
 Comment: 
 
 Filename: algokit_client_generator/writer.py
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b6.dist-info/LICENSE
+Filename: algokit_client_generator-0.1.0b7.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b6.dist-info/METADATA
+Filename: algokit_client_generator-0.1.0b7.dist-info/METADATA
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b6.dist-info/WHEEL
+Filename: algokit_client_generator-0.1.0b7.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b6.dist-info/entry_points.txt
+Filename: algokit_client_generator-0.1.0b7.dist-info/entry_points.txt
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b6.dist-info/RECORD
+Filename: algokit_client_generator-0.1.0b7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_client_generator/__init__.py

```diff
@@ -1,4 +1,3 @@
-from algokit_client_generator.generator import GenerationSettings
 from algokit_client_generator.writer import generate_client
 
-__all__ = ["generate_client", "GenerationSettings"]
+__all__ = ["generate_client"]
```

## algokit_client_generator/cli.py

```diff
@@ -1,63 +1,81 @@
 import argparse
+import logging
 import sys
 from pathlib import Path
 
-from algokit_client_generator.generator import GenerationSettings
 from algokit_client_generator.writer import generate_client
 
-parser = argparse.ArgumentParser(
-    description="Generates typed python clients from an Algorand ARC-0032 specification file."
-)
-
-parser.add_argument(
-    "-a",
-    "--app_spec",
-    default=".",
-    type=Path,
-    help="The path to an application.json or a directory if using --walk. Defaults to current directory",
-)
-parser.add_argument(
-    "-o", "--output", default="client_generated.py", type=Path, help="The output filename for the generated client"
-)
-parser.add_argument(
-    "-w",
-    "--walk",
-    action="store_true",
-    help="Walk the input path recursively, generating a client for each application.json found",
-)
-args = parser.parse_args()
+logger = logging.getLogger(__name__)
 
-DEFAULT_CLIENT = "client_generated.py"
 
+class ArgumentError(Exception):
+    def __init__(self, message: str):
+        self.message = message
+
+
+def get_args_parser() -> argparse.ArgumentParser:
+    parser = argparse.ArgumentParser(
+        description="Generates typed python clients from an Algorand ARC-0032 specification file."
+    )
+
+    parser.add_argument(
+        "-a",
+        "--app_spec",
+        default=".",
+        type=Path,
+        help="The path to an application.json or a directory if using --walk. Defaults to current directory",
+    )
+    parser.add_argument(
+        "-o", "--output", default="client_generated.py", type=Path, help="The output filename for the generated client"
+    )
+    parser.add_argument(
+        "-w",
+        "--walk",
+        action="store_true",
+        help="Walk the input path recursively, generating a client for each application.json found",
+    )
+    return parser
 
-def walk_dir(path: Path, output: Path, settings: GenerationSettings) -> None:
+
+def configure_logging() -> None:
+    logging.basicConfig(level=logging.INFO, format="%(message)s")
+
+
+def walk_dir(path: Path, output: Path) -> None:
     for child in path.iterdir():
         if child.is_dir():
-            walk_dir(child, output, settings)
+            walk_dir(child, output)
         elif child.name.lower() == "application.json":
-            generate_client(child, child.parent / output, settings)
+            generate_client(child, child.parent / output)
 
 
-def main() -> None:
-    settings = GenerationSettings(max_line_length=120)
+def process(parser: argparse.ArgumentParser) -> None:
+    args = parser.parse_args()
     app_spec: Path = args.app_spec
     output: Path = args.output
     if not app_spec.exists():
-        print(f"{app_spec} not found", file=sys.stderr)
-        return
+        raise ArgumentError(f"Application Specification not found: {app_spec}")
 
     if args.walk:
         if not app_spec.is_dir():
-            print(f"{app_spec} must be a path to a directory, when using the --walk option", file=sys.stderr)
-            return
+            raise ArgumentError(
+                f"Application specification must be a path to a directory, when using the --walk option: {app_spec}"
+            )
         if output.is_absolute():
-            print(f"{output} must be a relative path, when using the --walk option", file=sys.stderr)
-            return
-        walk_dir(args.app_spec, args.output, settings)
+            raise ArgumentError(f"Output must be a relative path when using the --walk option: {output}")
+        walk_dir(args.app_spec, args.output)
     elif len(sys.argv) == 1:  # if user invokes with no arguments display help
         parser.print_usage()
     else:
         if not app_spec.is_file():
-            print(f"{app_spec} must be a path to an application.json", file=sys.stderr)
-            return
-        generate_client(app_spec, output, settings)
+            raise ArgumentError(f"Application Specification must be a path to an application.json: {app_spec}")
+        generate_client(app_spec, output)
+
+
+def main() -> None:
+    configure_logging()
+    parser = get_args_parser()
+    try:
+        process(parser)
+    except ArgumentError as ex:
+        logger.error(ex.message)
```

## algokit_client_generator/generator.py

```diff
@@ -1,12 +1,13 @@
 import dataclasses
+import typing
 from collections.abc import Iterable
 from typing import Literal
 
-from algokit_utils import ApplicationSpecification, OnCompleteActionName
+import algokit_utils
 
 from algokit_client_generator import utils
 from algokit_client_generator.document import DocumentParts, Part
 from algokit_client_generator.spec import ABIContractMethod, ABIStruct, ContractMethod, get_contract_methods
 
 ESCAPED_QUOTE = r"\""
 
@@ -18,15 +19,15 @@
 
     @property
     def indent_length(self) -> int:
         return len(self.indent)
 
 
 class GenerateContext:
-    def __init__(self, app_spec: ApplicationSpecification):
+    def __init__(self, app_spec: algokit_utils.ApplicationSpecification):
         self.app_spec = app_spec
         # TODO: track these as they are emitted?
         self.used_module_symbols = {
             "_APP_SPEC_JSON",
             "APP_SPEC",
             "_TArgs",
             "_TArgsHolder",
@@ -58,15 +59,14 @@
             "get_local_state",
         }
         self.client_name = utils.get_unique_symbol_by_incrementing(
             self.used_module_symbols, utils.get_class_name(self.app_spec.contract.name, "client")
         )
         self.methods = get_contract_methods(app_spec, self.used_module_symbols, self.used_client_symbols)
         self.disable_linting = True
-        self.settings = GenerationSettings()
 
 
 def generated_comment(context: GenerateContext) -> DocumentParts:
     yield "# This file was automatically generated by algokit-client-generator."
     yield "# DO NOT MODIFY IT BY HAND."
 
 
@@ -284,18 +284,25 @@
         if desc:
             yield utils.docstring(desc)
     yield Part.DecIndent
     yield Part.DecIndent
     yield Part.Gap2
 
 
+def _get_declared_schema(
+    app_spec: algokit_utils.ApplicationSpecification, schema_name: Literal["global", "local"]
+) -> dict[str, dict[str, typing.Any]]:
+    schema = app_spec.schema.get(schema_name) or {}
+    return schema.get("declared") or {}
+
+
 def state_types(context: GenerateContext) -> DocumentParts:
     app_spec = context.app_spec
-    global_schema = app_spec.schema.get("global", {}).get("declared", {})
-    local_schema = app_spec.schema.get("local", {}).get("declared", {})
+    global_schema = _get_declared_schema(app_spec, "global")
+    local_schema = _get_declared_schema(app_spec, "local")
     has_bytes = any(i.get("type") == "bytes" for i in [*global_schema.values(), *local_schema.values()])
     if has_bytes:
         yield utils.indented(
             """
 class ByteReader:
     def __init__(self, data: bytes):
         self._data = data
@@ -386,18 +393,20 @@
             app_name=app_name,
         )"""
     )
     yield Part.Gap1
     yield Part.IncIndent
     yield forwarded_client_properties(context)
     yield Part.Gap1
-    yield get_global_state_method(context)
-    yield Part.Gap1
-    yield get_local_state_method(context)
-    yield Part.Gap1
+    if _get_declared_schema(context.app_spec, "global"):
+        yield get_global_state_method(context)
+        yield Part.Gap1
+    if _get_declared_schema(context.app_spec, "local"):
+        yield get_local_state_method(context)
+        yield Part.Gap1
     yield methods_by_side_effect(context, "none", context.methods.no_op)
     yield Part.Gap1
     yield methods_by_side_effect(context, "create", context.methods.create)
     yield Part.Gap1
     yield methods_by_side_effect(context, "update", context.methods.update_application)
     yield Part.Gap1
     yield methods_by_side_effect(context, "delete", context.methods.delete_application)
@@ -461,14 +470,66 @@
     yield '_APP_SPEC_JSON = r"""'
     yield context.app_spec.to_json()
     yield '"""'
     yield Part.RestoreLineMode
     yield "APP_SPEC = algokit_utils.ApplicationSpecification.from_json(_APP_SPEC_JSON)"
 
 
+def create_method_doc_string(method: ContractMethod) -> Iterable[str]:
+    if method.abi:
+        if method.abi.method.desc:
+            yield method.abi.method.desc
+            yield ""
+        yield f"Calls `{method.abi.method.get_signature()}` ABI method"
+        yield ""
+        for arg in method.abi.args:
+            desc = f":param {arg.python_type} {arg.name}: "
+            desc += "(optional) " if arg.has_default else ""
+            desc += arg.desc or f"The `{arg.name}` ABI parameter"
+            yield desc
+        if method.call_config == "create":
+            on_completes = method.on_complete
+            yield f":param typing.Literal[{', '.join(on_completes)}] on_complete: On completion type to use"
+            yield (
+                ":param algokit_utils.CreateTransactionParameters transaction_parameters: "
+                "(optional) Additional transaction parameters"
+            )
+        else:
+            yield (
+                ":param algokit_utils.TransactionParameters transaction_parameters: "
+                "(optional) Additional transaction parameters"
+            )
+        yield (
+            f":returns algokit_utils.ABITransactionResponse[{method.abi.python_type}]: "
+            f"{method.abi.method.returns.desc or 'The result of the transaction'}"
+        )
+    else:
+        if method.call_config == "create":
+            if len(method.on_complete) > 1:
+                yield f"Creates an application using one of the {', '.join(method.on_complete)} bare methods"
+            else:
+                yield f"Creates an application using the {method.on_complete[0]} bare method"
+            yield ""
+            on_completes = method.on_complete
+            yield f":param typing.Literal[{', '.join(on_completes)}] on_complete: On completion type to use"
+            yield (
+                ":param algokit_utils.CreateTransactionParameters transaction_parameters: "
+                "(optional) Additional transaction parameters"
+            )
+        else:
+            yield f"Calls the {method.on_complete[0]} bare method"
+            yield ""
+            yield (
+                ":param algokit_utils.TransactionParameters transaction_parameters: "
+                "(optional) Additional transaction parameters"
+            )
+
+        yield ":returns algokit_utils.TransactionResponse: The result of the transaction"
+
+
 def signature(context: GenerateContext, name: str, method: ContractMethod) -> DocumentParts:
     yield f"def {name}("
     yield Part.IncIndent
     yield "self,"
     yield "*,"
     abi = method.abi
     if abi:
@@ -483,15 +544,18 @@
     else:
         yield "transaction_parameters: algokit_utils.TransactionParameters | None = None,"
     yield Part.DecIndent
     if abi:
         yield f") -> algokit_utils.ABITransactionResponse[{abi.python_type}]:"
     else:
         yield ") -> algokit_utils.TransactionResponse:"
-    # TODO: docstring
+    yield Part.IncIndent
+    yield utils.docstring("\n".join(create_method_doc_string(method)))
+    yield Part.DecIndent
+    yield Part.Gap1
 
 
 def instantiate_args(contract_method: ABIContractMethod | None) -> DocumentParts:
     if contract_method and not contract_method.args:
         yield f"args = {contract_method.args_class_name}()"
     elif contract_method:
         yield f"args = {contract_method.args_class_name}(", Part.IncIndent
@@ -523,15 +587,15 @@
     if contract_method.abi and contract_method.abi.result_struct:
         yield 'elements = self.app_spec.hints[args.method()].structs["output"]["elements"]'
         yield "result_dict = {element[0]: value for element, value in zip(elements, result.return_value)}"
         yield f"result.return_value = {contract_method.abi.python_type}(**result_dict)"
     yield "return result"
 
 
-def on_complete_literals(on_completes: Iterable[OnCompleteActionName]) -> DocumentParts:
+def on_complete_literals(on_completes: Iterable[algokit_utils.OnCompleteActionName]) -> DocumentParts:
     yield Part.InlineMode
     yield 'on_complete: typing.Literal["'
     yield utils.join('", "', on_completes)
     yield '"]'
     if "no_op" in on_completes:
         yield ' = "no_op"'
     yield ","
@@ -638,24 +702,34 @@
 
 
 def get_global_state_method(context: GenerateContext) -> DocumentParts:
     if not context.app_spec.schema.get("global", {}).get("declared", {}):
         return
     yield "def get_global_state(self) -> GlobalState:"
     yield Part.IncIndent
+    yield utils.docstring(
+        "Returns the application's global state wrapped in a strongly typed class"
+        " with options to format the stored value"
+    )
+    yield Part.Gap1
     yield "state = typing.cast(dict[bytes, bytes | int], self.app_client.get_global_state(raw=True))"
     yield "return GlobalState(state)"
     yield Part.DecIndent
 
 
 def get_local_state_method(context: GenerateContext) -> DocumentParts:
     if not context.app_spec.schema.get("local", {}).get("declared", {}):
         return
     yield "def get_local_state(self, account: str | None = None) -> LocalState:"
     yield Part.IncIndent
+    yield utils.docstring(
+        "Returns the application's local state wrapped in a strongly typed class"
+        " with options to format the stored value"
+    )
+    yield Part.Gap1
     yield "state = typing.cast(dict[bytes, bytes | int], self.app_client.get_local_state(account, raw=True))"
     yield "return LocalState(state)"
     yield Part.DecIndent
 
 
 def generate(context: GenerateContext) -> DocumentParts:
     if context.disable_linting:
```

## algokit_client_generator/writer.py

```diff
@@ -1,22 +1,28 @@
+import logging
 from pathlib import Path
 
 from algokit_utils import ApplicationSpecification
 
 from algokit_client_generator.document import DocumentParts, RenderContext, convert_part
-from algokit_client_generator.generator import GenerateContext, GenerationSettings, generate
+from algokit_client_generator.generator import GenerateContext, generate
 
+logger = logging.getLogger(__name__)
 
-def generate_client(input_path: Path, output_path: Path, settings: GenerationSettings | None = None) -> None:
+
+def generate_client(input_path: Path, output_path: Path) -> None:
+    """Given a path to an ARC-32 application.json, output a typed python client
+
+    :param Path input_path: Path to an ARC-32 application.json
+    :param Path output_path: Path to write a typed python client to
+    """
     app_spec = ApplicationSpecification.from_json(input_path.read_text())
 
     context = GenerateContext(app_spec)
-    if settings:
-        context.settings = settings
-    output = render(generate(context), context.settings)
+    output = render(generate(context))
     output_path.write_text(output)
-    print(f"Output typed client for {app_spec.contract.name} to {output_path}")
+    logger.info(f"Output typed client for {app_spec.contract.name} to {output_path}")
 
 
-def render(parts: DocumentParts, settings: GenerationSettings) -> str:
-    context = RenderContext(indent_inc=settings.indent)
+def render(parts: DocumentParts) -> str:
+    context = RenderContext(indent_inc="    ")
     return "".join(convert_part(parts, context))
```

## Comparing `algokit_client_generator-0.1.0b6.dist-info/LICENSE` & `algokit_client_generator-0.1.0b7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_client_generator-0.1.0b6.dist-info/METADATA` & `algokit_client_generator-0.1.0b7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-client-generator
-Version: 0.1.0b6
+Version: 0.1.0b7
 Summary: Algorand typed client Generator
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_client_generator-0.1.0b6.dist-info/RECORD` & `algokit_client_generator-0.1.0b7.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-algokit_client_generator/__init__.py,sha256=KHVr3rMTN2T146gjOpaF3fc5cqoLoVs01ueXn-p9QHI,179
+algokit_client_generator/__init__.py,sha256=ikLxrMdPVjpmrVYDdHbunvzUwiXqrCdvp8Qi5x0gC0c,91
 algokit_client_generator/__main__.py,sha256=MlkUdDAWa2XH1QDdjvayVR_WaZEGkA9voNutHzWEfFo,54
-algokit_client_generator/cli.py,sha256=S9YxyLIpzDvSGLbxP7QJz8b-otpzX-lgHRJzvEzFC6Q,2132
+algokit_client_generator/cli.py,sha256=XwuLZUhym9ntuHRIayPZsfv2-vTSbEykt3evF7EdVq4,2550
 algokit_client_generator/document.py,sha256=X4xMvu_LfDcaosEy3AtjRoXpiLZoXRVCIoPNo8b-h08,3199
-algokit_client_generator/generator.py,sha256=WlnxNObfumcp2R3cu0FqrBHQNfC1TiGwDLTBxNPfv7w,23029
+algokit_client_generator/generator.py,sha256=IIoCVPQmAwdq4CDoEdRQVN6Zp4QmpB3DHOFJWCKuGNI,26188
 algokit_client_generator/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 algokit_client_generator/spec.py,sha256=apgef1qcRbm2akT1ogF23d6HnSncPwnLdrqaVzJAKmo,7466
 algokit_client_generator/utils.py,sha256=LQ3wXw_1IlnkKKNzDetIbAIBqEgYrRRjI6Bu_42Yzpc,4303
-algokit_client_generator/writer.py,sha256=MF46CQ8q1nW-K66RcKcXYE1uArrNRKHWF-uKQT8eziU,890
-algokit_client_generator-0.1.0b6.dist-info/LICENSE,sha256=fkgfhUgPPyK1aS4tK9QOFRl5fWtuFEtkKx4zPQNT1bQ,1076
-algokit_client_generator-0.1.0b6.dist-info/METADATA,sha256=DHw5TK0OeJjk4NTPcqNpsm9BPJD4vw_b1nY4LL0toWA,4585
-algokit_client_generator-0.1.0b6.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
-algokit_client_generator-0.1.0b6.dist-info/entry_points.txt,sha256=RnsJToDSJC_LyXvGqv7LNpgkqipw1C7eQsc0bke--A0,67
-algokit_client_generator-0.1.0b6.dist-info/RECORD,,
+algokit_client_generator/writer.py,sha256=CynBYWnHlO1E4Ubcpjvzq8kRcgfYCpnO3nEAslBEr-s,995
+algokit_client_generator-0.1.0b7.dist-info/LICENSE,sha256=fkgfhUgPPyK1aS4tK9QOFRl5fWtuFEtkKx4zPQNT1bQ,1076
+algokit_client_generator-0.1.0b7.dist-info/METADATA,sha256=cYlTVKkvu77UHYj3EXl50bCrrXrzQkzT6-pOvPxcLNs,4585
+algokit_client_generator-0.1.0b7.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+algokit_client_generator-0.1.0b7.dist-info/entry_points.txt,sha256=RnsJToDSJC_LyXvGqv7LNpgkqipw1C7eQsc0bke--A0,67
+algokit_client_generator-0.1.0b7.dist-info/RECORD,,
```

