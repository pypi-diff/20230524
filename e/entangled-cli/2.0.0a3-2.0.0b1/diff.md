# Comparing `tmp/entangled_cli-2.0.0a3.tar.gz` & `tmp/entangled_cli-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entangled_cli-2.0.0a3.tar", max compression
+gzip compressed data, was "entangled_cli-2.0.0b1.tar", max compression
```

## Comparing `entangled_cli-2.0.0a3.tar` & `entangled_cli-2.0.0b1.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0    11357 2023-05-20 22:45:38.703760 entangled_cli-2.0.0a3/LICENSE
--rw-r--r--   0        0        0     3636 2023-05-20 22:45:38.703760 entangled_cli-2.0.0a3/README.md
--rw-r--r--   0        0        0        1 2023-05-20 22:45:38.703760 entangled_cli-2.0.0a3/entangled/__init__.py
--rw-r--r--   0        0        0     2366 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/code_reader.py
--rw-r--r--   0        0        0      152 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/commands/init.py
--rw-r--r--   0        0        0     1828 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/commands/stitch.py
--rw-r--r--   0        0        0     1184 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/commands/sync.py
--rw-r--r--   0        0        0     1775 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/commands/tangle.py
--rw-r--r--   0        0        0     1292 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/commands/watch.py
--rw-r--r--   0        0        0     2586 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/config/__init__.py
--rw-r--r--   0        0        0     1327 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/config/language.py
--rw-r--r--   0        0        0      606 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/config/version.py
--rw-r--r--   0        0        0     1775 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/construct.py
--rw-r--r--   0        0        0        1 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/data/defaults.toml
--rw-r--r--   0        0        0     3731 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/document.py
--rw-r--r--   0        0        0      828 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/error.py
--rw-r--r--   0        0        0     5186 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/filedb.py
--rw-r--r--   0        0        0      652 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/hooks/__init__.py
--rw-r--r--   0        0        0      653 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/hooks/base.py
--rw-r--r--   0        0        0     1494 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/hooks/build.py
--rw-r--r--   0        0        0     1455 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/main.py
--rw-r--r--   0        0        0     4560 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/markdown_reader.py
--rw-r--r--   0        0        0     5507 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/parsing.py
--rw-r--r--   0        0        0     2440 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/properties.py
--rw-r--r--   0        0        0        0 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/py.typed
--rw-r--r--   0        0        0     1067 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/tangle.py
--rw-r--r--   0        0        0     5460 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/transaction.py
--rw-r--r--   0        0        0      834 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/utility.py
--rw-r--r--   0        0        0       30 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/entangled/version.py
--rw-r--r--   0        0        0     1170 2023-05-20 22:45:38.707760 entangled_cli-2.0.0a3/pyproject.toml
--rw-r--r--   0        0        0     4300 1970-01-01 00:00:00.000000 entangled_cli-2.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/LICENSE
+-rw-r--r--   0        0        0     3636 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/README.md
+-rw-r--r--   0        0        0        1 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/__init__.py
+-rw-r--r--   0        0        0     2306 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/code_reader.py
+-rw-r--r--   0        0        0      152 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/commands/init.py
+-rw-r--r--   0        0        0     2003 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/commands/stitch.py
+-rw-r--r--   0        0        0     1184 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/commands/sync.py
+-rw-r--r--   0        0        0     1737 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/commands/tangle.py
+-rw-r--r--   0        0        0     1692 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/commands/watch.py
+-rw-r--r--   0        0        0     2586 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/config/__init__.py
+-rw-r--r--   0        0        0     1402 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/config/language.py
+-rw-r--r--   0        0        0      606 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/config/version.py
+-rw-r--r--   0        0        0     1775 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/construct.py
+-rw-r--r--   0        0        0        1 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/data/defaults.toml
+-rw-r--r--   0        0        0     3819 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/document.py
+-rw-r--r--   0        0        0        0 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/errors/__init__.py
+-rw-r--r--   0        0        0      561 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/errors/internal.py
+-rw-r--r--   0        0        0      736 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/errors/user.py
+-rw-r--r--   0        0        0     5189 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/filedb.py
+-rw-r--r--   0        0        0      652 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/hooks/__init__.py
+-rw-r--r--   0        0        0      653 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/hooks/base.py
+-rw-r--r--   0        0        0     1494 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/entangled/hooks/build.py
+-rw-r--r--   0        0        0     1744 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/entangled/main.py
+-rw-r--r--   0        0        0     4630 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/entangled/markdown_reader.py
+-rw-r--r--   0        0        0     5450 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/entangled/parsing.py
+-rw-r--r--   0        0        0     2449 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/entangled/properties.py
+-rw-r--r--   0        0        0        0 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/entangled/py.typed
+-rw-r--r--   0        0        0     1697 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/entangled/tangle.py
+-rw-r--r--   0        0        0     5470 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/entangled/transaction.py
+-rw-r--r--   0        0        0      834 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/entangled/utility.py
+-rw-r--r--   0        0        0       85 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/entangled/version.py
+-rw-r--r--   0        0        0     1169 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     4300 1970-01-01 00:00:00.000000 entangled_cli-2.0.0b1/PKG-INFO
```

### Comparing `entangled_cli-2.0.0a3/LICENSE` & `entangled_cli-2.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0a3/README.md` & `entangled_cli-2.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0a3/entangled/code_reader.py` & `entangled_cli-2.0.0b1/entangled/code_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,15 @@
-from typing import Optional
 from dataclasses import dataclass, field
 from pathlib import Path
 
 import mawk
 import re
-import logging
 
 from .document import ReferenceId, TextLocation, ReferenceMap
-
-
-@dataclass
-class IndentationError(Exception):
-    location: TextLocation
-
-    def __str__(self):
-        return f"indentation error at `{self.location}`"
+from .errors.user import IndentationError
 
 
 @dataclass
 class StitchError(Exception):
     path: Path
     msg: str
 
@@ -74,11 +65,14 @@
             raise IndentationError(self.location)
         self.refs[self.current.ref].source = "\n".join(self.current.content)
         self.stack.pop()
         return []
 
     @mawk.always
     def otherwise(self, line: str):
+        if line.strip() == "":
+            self.current.content.append("")
+            return []
         if not line.startswith(self.current.indent):
             raise IndentationError(self.location)
         self.current.content.append(line.removeprefix(self.current.indent))
         return []
```

### Comparing `entangled_cli-2.0.0a3/entangled/commands/stitch.py` & `entangled_cli-2.0.0b1/entangled/commands/stitch.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import argh  # type: ignore
 
 from ..config import config
 from ..code_reader import CodeReader
 from ..markdown_reader import MarkdownReader
 from ..document import ReferenceMap, Content, PlainText, ReferenceId
 from ..transaction import transaction, TransactionMode
+from ..errors.user import UserError
 
 
 def stitch_markdown(reference_map: ReferenceMap, content: list[Content]) -> str:
     def get(item: Content):
         match item:
             case PlainText(s):
                 return s
@@ -34,23 +35,27 @@
     elif force:
         mode = TransactionMode.FORCE
     else:
         mode = TransactionMode.FAIL
 
     refs = ReferenceMap()
     content: dict[Path, list[Content]] = {}
-    for path in input_file_list:
-        logging.debug("reading `%s`", path)
-        with open(path, "r") as f:
-            mr = MarkdownReader(str(path), refs)
-            mr.run(f.read())
-            content[path] = mr.content
-
-    with transaction(mode) as t:
-        for path in t.db.managed:
+    try:
+        for path in input_file_list:
             logging.debug("reading `%s`", path)
-            t.db.update(path)
             with open(path, "r") as f:
-                CodeReader(str(path), refs).run(f.read())
-
-        for path in input_file_list:
-            t.write(path, stitch_markdown(refs, content[path]), [])
+                mr = MarkdownReader(str(path), refs)
+                mr.run(f.read())
+                content[path] = mr.content
+
+        with transaction(mode) as t:
+            for path in t.db.managed:
+                logging.debug("reading `%s`", path)
+                t.db.update(path)
+                with open(path, "r") as f:
+                    CodeReader(str(path), refs).run(f.read())
+
+            for path in input_file_list:
+                t.write(path, stitch_markdown(refs, content[path]), [])
+                
+    except UserError as e:
+        logging.error(str(e))
```

### Comparing `entangled_cli-2.0.0a3/entangled/commands/sync.py` & `entangled_cli-2.0.0b1/entangled/commands/sync.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0a3/entangled/commands/tangle.py` & `entangled_cli-2.0.0b1/entangled/commands/tangle.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,42 +7,42 @@
 
 from ..document import ReferenceMap
 from ..config import config, AnnotationMethod
 from ..markdown_reader import MarkdownReader
 from ..transaction import transaction, TransactionMode
 from ..tangle import tangle_ref
 from ..hooks import get_hooks
-from ..error import UserError
+from ..errors.user import UserError
 
 
 @argh.arg(
     "-a",
     "--annotate",
     choices=[m.name.lower() for m in AnnotationMethod],
     help="annotation method",
 )
 @argh.arg("--force", help="force overwrite on conflict")
 @argh.arg("-s", "--show", help="only show, don't act")
 def tangle(*, annotate: Optional[str] = None, force: bool = False, show: bool = False):
     """Tangle codes from Markdown"""
-    try:
-        if annotate is not None:
-            config.annotation = AnnotationMethod[annotate.upper()]
+    if annotate is not None:
+        config.annotation = AnnotationMethod[annotate.upper()]
 
-        input_file_list = chain.from_iterable(map(Path(".").glob, config.watch_list))
-        refs = ReferenceMap()
-        hooks = get_hooks()
-
-        if show:
-            mode = TransactionMode.SHOW
-        elif force:
-            mode = TransactionMode.FORCE
-        else:
-            mode = TransactionMode.FAIL
+    input_file_list = chain.from_iterable(map(Path(".").glob, config.watch_list))
+    refs = ReferenceMap()
+    hooks = get_hooks()
+
+    if show:
+        mode = TransactionMode.SHOW
+    elif force:
+        mode = TransactionMode.FORCE
+    else:
+        mode = TransactionMode.FAIL
 
+    try:
         with transaction(mode) as t:
             for path in input_file_list:
                 logging.debug("reading `%s`", path)
                 t.db.update(path)
                 with open(path, "r") as f:
                     MarkdownReader(str(path), refs, hooks).run(f.read())
```

### Comparing `entangled_cli-2.0.0a3/entangled/commands/watch.py` & `entangled_cli-2.0.0b1/entangled/commands/watch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from typing import Optional
 from pathlib import Path
 from itertools import chain
 import logging
+from threading import Event
 
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler, FileSystemEvent
 
 from .sync import sync
 from ..config import config
 from ..filedb import file_db
@@ -24,22 +26,33 @@
         path = Path(event.src_path)
         if path.is_relative_to(Path("./.entangled")):
             return
         if any(path.is_relative_to(p) for p in self.watched):
             sync()
 
 
-def watch():
-    """Keep a loop running, watching for changes."""
+def _watch(_stop_event: Optional[Event] = None):
+    """Keep a loop running, watching for changes. This interface is separated
+    from the CLI one, so that it can be tested using threading instead of
+    subprocess."""
+
+    def stop() -> bool:
+        return _stop_event is not None and _stop_event.is_set()
+    
     sync()
 
     event_handler = EventHandler()
     observer = Observer()
     observer.schedule(event_handler, ".", recursive=True)
     observer.start()
 
     try:
-        while observer.is_alive():
-            observer.join(1.0)
+        while observer.is_alive() and not stop():
+            observer.join(0.1)
     finally:
         observer.stop()
         observer.join()
+
+
+def watch():
+    """Keep a loop running, watching for changes."""
+    _watch()
```

### Comparing `entangled_cli-2.0.0a3/entangled/config/__init__.py` & `entangled_cli-2.0.0b1/entangled/config/__init__.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0a3/entangled/config/language.py` & `entangled_cli-2.0.0b1/entangled/config/language.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,12 +31,13 @@
     Language("Rust", ["rust"], Comment("//")),
     Language("Haskell", ["haskell"], Comment("--")),
     Language(
         "Lisp", ["scheme", "r5rs", "r6rs", "r7rs", "racket", "clojure"], Comment(";")
     ),
     Language("Julia", ["julia"], Comment("#")),
     Language("Java", ["java"], Comment("//")),
+    Language("PureScritp", ["pure", "purs", "purescript"], Comment("--")),
     Language("CSS", ["css"], Comment("/*", "*/")),
     Language("Lua", ["lua"], Comment("--")),
     Language("Make", ["make", "makefile"], Comment("#")),
     Language("Gnuplot", ["gnuplot"], Comment("#"))
 ]
```

### Comparing `entangled_cli-2.0.0a3/entangled/config/version.py` & `entangled_cli-2.0.0b1/entangled/config/version.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0a3/entangled/construct.py` & `entangled_cli-2.0.0b1/entangled/construct.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0a3/entangled/document.py` & `entangled_cli-2.0.0b1/entangled/document.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-from typing import Union, Optional, Iterable, Any
+from typing import Union, Iterable, Any
 from dataclasses import dataclass, field
 from collections import defaultdict
 from functools import singledispatchmethod
 from itertools import chain
-from pathlib import Path
-import mawk
 
 from .config import Language, AnnotationMethod, config
 from .properties import Property, get_attribute
-from .error import InternalError, CyclicReference
+from .errors.internal import InternalError
 
 
 def length(iter: Iterable[Any]) -> int:
     return sum(1 for _ in iter)
 
 
 @dataclass
@@ -34,14 +32,17 @@
 
 
 @dataclass
 class TextLocation:
     filename: str
     line_number: int = 0
 
+    def __str__(self):
+        return f"{self.filename}:{self.line_number}"
+
 
 @dataclass
 class CodeBlock:
     language: Language
     properties: list[Property]
     indent: str
     source: str
@@ -85,26 +86,26 @@
         return self.by_name(key)
 
     @singledispatchmethod
     def get_decorated(self, ref):
         raise NotImplementedError(f"Invalid key: {type(ref)}")
 
     @get_decorated.register
-    def _(self, ref: ReferenceId) -> list[str]:
+    def _(self, ref: ReferenceId, annotation=config.annotation) -> list[str]:
         init = ref == self.index[ref.name][0]
         count = "init" if init else str(ref.ref_count)
         cb = self.map[ref]
         close_comment = (
             "" if cb.language.comment.close is None else f" {cb.language.comment.close}"
         )
         start = (
             f"{cb.language.comment.open} ~/~ begin <<{ref.file}#{ref.name}>>[{count}]"
         )
         end = f"{cb.language.comment.open} ~/~ end{close_comment}"
-        match config.annotation:
+        match annotation:
             case AnnotationMethod.STANDARD:
                 return [start + close_comment, cb.source, end]
             case AnnotationMethod.NAKED:
                 return [cb.source]
             case AnnotationMethod.SUPPLEMENTED:
                 if config.annotation_format is None:
                     return [start + close_comment, cb.source, end]
@@ -116,11 +117,11 @@
                     start + " " + supplement + close_comment,
                     cb.source,
                     end,
                 ]
         raise InternalError("End of exhaustive match reached")
     
     @get_decorated.register
-    def _(self, ref_name: str) -> Iterable[str]:
+    def _(self, ref_name: str, annotation=config.annotation) -> Iterable[str]:
         return chain.from_iterable(
-            self.get_decorated(ref) for ref in self.index[ref_name]
+            self.get_decorated(ref, annotation) for ref in self.index[ref_name]
         )
```

### Comparing `entangled_cli-2.0.0a3/entangled/error.py` & `entangled_cli-2.0.0b1/entangled/errors/internal.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,20 @@
 from typing import Any
 from dataclasses import dataclass, field
 from textwrap import wrap
+import logging
 
 
 @dataclass
 class InternalError(Exception):
     msg: str
     irritants: list[Any] = field(default_factory=list)
 
     def __str__(self):
         return f"Internal error: {self.msg}"
 
 
-class UserError(Exception):
-    def __str__(self):
-        return "Unknown user error."
-
-
-@dataclass
-class CyclicReference(UserError):
-    ref_name: str
-
-    def __str__(self):
-        return f"Cyclic reference in <<{self.ref_name}>>"
-
-
 def bug_contact():
-    print(
-        wrap(
-            "This error is due to an internal bug in Entangled. "
-            "Please file an issue including the above stack trace "
-            "and example content to reproduce the exception "
-            "at https://github.com/entangled/entangled.py/."
-        )
-    )
+    logging.error(
+        "This error is due to an internal bug in Entangled. Please file an "
+        "issue including the above stack trace " "and example content to "
+        "reproduce the exception at https://github.com/entangled/entangled.py/.")
```

### Comparing `entangled_cli-2.0.0a3/entangled/filedb.py` & `entangled_cli-2.0.0b1/entangled/filedb.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
     @staticmethod
     def initialize() -> FileDB:
         if FileDB.path().exists():
             db = FileDB.read()
             undead = list(filter(lambda p: not p.exists(), db.files))
             for path in undead:
-                logging.warn(
+                logging.warning(
                     "File `%s` in DB doesn't exist. Removing entry from DB.", path
                 )
                 del db[path]
             return db
 
         FileDB.path().parent.mkdir(parents=True, exist_ok=True)
         data = {"version": __version__, "files": [], "source": [], "target": []}
```

### Comparing `entangled_cli-2.0.0a3/entangled/hooks/__init__.py` & `entangled_cli-2.0.0b1/entangled/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0a3/entangled/hooks/base.py` & `entangled_cli-2.0.0b1/entangled/hooks/base.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0a3/entangled/hooks/build.py` & `entangled_cli-2.0.0b1/entangled/hooks/build.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0a3/entangled/main.py` & `entangled_cli-2.0.0b1/entangled/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
     WITH_RICH = True
 except ImportError:
     WITH_RICH = False
 
 
 from .commands import tangle, stitch, sync, watch
+from .errors.internal import bug_contact
+from .errors.user import UserError
+from .version import __version__
 
 
 if WITH_RICH:
 
     class BackTickHighlighter(RegexHighlighter):
         highlights = [r"`(?P<bold>[^`]*)`"]
 
@@ -36,15 +39,15 @@
             handlers=[RichHandler(show_path=debug, highlighter=BackTickHighlighter())],
         )
         logging.debug("Rich logging enabled")
     else:
         logging.basicConfig(level=level)
         logging.debug("Plain logging enabled")
 
-    logging.info("Welcome to Entangled (https://entangled.github.io/)")
+    logging.info(f"Entangled {__version__} (https://entangled.github.io/)")
 
 
 def cli():
     import argparse
 
     try:
         parser = argparse.ArgumentParser()
@@ -54,12 +57,19 @@
         argh.add_commands(parser, [tangle, stitch, sync, watch])
         args = parser.parse_args()
         configure(args.debug)
         argh.dispatch(parser)
     except KeyboardInterrupt:
         logging.info("Goodbye")
         sys.exit(0)
+    except UserError as e:
+        logging.info(str(e))
+        sys.exit(0)
+    except Exception as e:
+        logging.error(str(e))
+        bug_contact(e)
+        sys.exit(1)
 
 
 if __name__ == "__main__":
         cli()
```

### Comparing `entangled_cli-2.0.0a3/entangled/markdown_reader.py` & `entangled_cli-2.0.0b1/entangled/markdown_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 from typing import Optional
-from dataclasses import dataclass
 from copy import copy
 from pathlib import Path
 
 import re
 import mawk
 import logging
 
 from .config import config
 from .utility import first
 from .document import TextLocation, CodeBlock, ReferenceMap, Content, PlainText
 from .properties import read_properties, get_attribute, get_classes, get_id
 from .hooks.base import HookBase
-
-
-@dataclass
-class MarkdownError(Exception):
-    location: TextLocation
-    what: str
-
-    def __str__(self):
-        return self.what
+from .errors.user import ParseError
+from . import parsing
 
 
 class MarkdownReader(mawk.RuleSet):
     """Reads a Markdown file, and splits it up into code blocks and other
     content. The contents of the code blocks get stored in `reference_map`.
     """
 
@@ -60,29 +52,33 @@
     def on_open_codeblock(self, m: re.Match) -> Optional[list[str]]:
         if self.ignore:
             return None
         if self.inside_codeblock:
             return None
         self.current_codeblock_indent = m["indent"]
         self.current_codeblock_location = copy(self.location)
-        self.current_codeblock_properties = read_properties(m["properties"])
         self.current_content.append(m[0])
-        self.flush_plain_text()
-        self.inside_codeblock = True
+        try:
+            self.current_codeblock_properties = read_properties(m["properties"])
+            self.flush_plain_text()
+            self.inside_codeblock = True
+        except parsing.Failure as f:
+            logging.error("Parsing error at %s: %s", self.location, f)
+            logging.error("Continuing parsing rest of document.")
         return []
 
     @mawk.on_match(config.markers.close)
     def on_close_codeblock(self, m: re.Match):
         if self.ignore:
             return
         if not self.inside_codeblock:
             return
         
         if len(m["indent"]) < len(self.current_codeblock_indent):
-            raise MarkdownError(self.location, "indentation error")
+            raise IndentationError(self.location)
 
         if m["indent"] != self.current_codeblock_indent:
             return  # treat this as code-block content
 
         # add block to reference-map
         language_class = first(get_classes(self.current_codeblock_properties))
         block_id = get_id(self.current_codeblock_properties)
```

### Comparing `entangled_cli-2.0.0a3/entangled/parsing.py` & `entangled_cli-2.0.0b1/entangled/parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Monadic recursive descent parser combinator. This is used to custom 
 light weight parsing within Entangled, mainly parsing the class, id and
 attribute properties of code blocks in markdown."""
 
 from __future__ import annotations
 
-from abc import ABC, abstractclassmethod, abstractmethod
 from dataclasses import dataclass
 from typing import (
     TypeVar,
     TypeVarTuple,
     Generic,
     Callable,
     Union,
```

### Comparing `entangled_cli-2.0.0a3/entangled/properties.py` & `entangled_cli-2.0.0b1/entangled/properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from __future__ import annotations
 
 from typing import Optional, Union, ClassVar, Iterable
 from dataclasses import dataclass
 import re
 
-from .parsing import Parser, many, choice, tokenize, matching, Parsable, starmap
+from .parsing import Parser, many, choice, tokenize, matching, Parsable, starmap, Failure
 
 
 @dataclass
 class Id(Parsable):
     value: str
     _pattern: ClassVar[Parser] = matching(r"#([a-zA-Z]\S*)")
```

### Comparing `entangled_cli-2.0.0a3/entangled/tangle.py` & `entangled_cli-2.0.0b1/entangled/tangle.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,59 @@
-from typing import Optional, TypeVar
-from dataclasses import dataclass
+from typing import Optional, TypeVar, Generic
+from dataclasses import dataclass, field
 from textwrap import indent
+from contextlib import contextmanager
 
 import re
 import mawk
 
-from .document import ReferenceMap
-from .error import CyclicReference
+from .document import ReferenceMap, AnnotationMethod
+from .errors.user import CyclicReference
+from .config import config
 
 
 T = TypeVar("T")
 
 
 @dataclass
+class Visitor(Generic[T]):
+    _visited: dict[T, int] = field(default_factory=dict)
+
+    def in_order(self) -> list[T]:
+        return [k for k, v in sorted(self._visited.items(), key=lambda kv: kv[1])]
+    
+    @contextmanager
+    def visit(self, x: T):
+        if x in self._visited:
+            raise CyclicReference(str(x), list(map(str, self.in_order())))
+        self._visited[x] = len(self._visited)
+        yield
+        del self._visited[x]
+
+
+@dataclass
 class Tangler(mawk.RuleSet):
     reference_map: ReferenceMap
-    visited: set[str]
+    visited: Visitor[str]
     deps: set[str]
+    annotation: AnnotationMethod
 
     @mawk.on_match(r"^(?P<indent>\s*)<<(?P<refname>[\w-]+)>>\s*$")
     def on_noweb(self, m: re.Match):
-        if m["refname"] in self.visited:
-            raise CyclicReference(m["refname"])
-        result, deps = tangle_ref(self.reference_map, m["refname"], self.visited)
+        result, deps = tangle_ref(self.reference_map, m["refname"], self.annotation, self.visited)
         self.deps.update(deps)
         return [indent(result, m["indent"])]
 
 
 def tangle_ref(
-    refs: ReferenceMap, ref_name: str, _visited: Optional[set[str]] = None
+    refs: ReferenceMap, ref_name: str, 
+    annotation: AnnotationMethod = config.annotation,
+    _visited: Optional[Visitor[str]] = None
 ) -> tuple[str, set[str]]:
-    visited = _visited or set()
-    visited.add(ref_name)
-    deps = set(cb.origin.filename for cb in refs.by_name(ref_name))
-    source = "\n".join(refs.get_decorated(ref_name))
-    t = Tangler(refs, visited, deps)
-    result = t.run(source)
+    v = _visited or Visitor()
+    with v.visit(ref_name):
+        deps = set(cb.origin.filename for cb in refs.by_name(ref_name))
+        source = "\n".join(refs.get_decorated(ref_name, annotation))
+        t = Tangler(refs, v, deps, annotation)
+        result = t.run(source)
     return result, deps
```

### Comparing `entangled_cli-2.0.0a3/entangled/transaction.py` & `entangled_cli-2.0.0b1/entangled/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     WITH_RICH = True
 except ImportError:
     WITH_RICH = False
 
 from .utility import cat_maybes
 from .filedb import FileDB, stat, file_db
-from .error import InternalError
+from .errors.internal import InternalError
 
 
 @dataclass
 class Action:
     target: Path
 
     def conflict(self, _: FileDB) -> Optional[str]:
```

### Comparing `entangled_cli-2.0.0a3/entangled/utility.py` & `entangled_cli-2.0.0b1/entangled/utility.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0a3/pyproject.toml` & `entangled_cli-2.0.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "entangled-cli"
-version = "2.0.0-alpha-3"
+version = "2.0.0-beta-1"
 description = "Literate Programming toolbox"
 repository = "https://github.com/entangled/entangled.py"
 homepage = "https://entangled.github.io/"
 authors = ["Johan Hidding <j.hidding@esciencecenter.nl>"]
 license = "Apache 2"
 readme = "README.md"
 packages = [
```

### Comparing `entangled_cli-2.0.0a3/PKG-INFO` & `entangled_cli-2.0.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entangled-cli
-Version: 2.0.0a3
+Version: 2.0.0b1
 Summary: Literate Programming toolbox
 Home-page: https://entangled.github.io/
 License: Apache 2
 Author: Johan Hidding
 Author-email: j.hidding@esciencecenter.nl
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
```

