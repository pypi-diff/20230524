# Comparing `tmp/conjuring-0.5.0.tar.gz` & `tmp/conjuring-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conjuring-0.5.0.tar", max compression
+gzip compressed data, was "conjuring-0.6.0.tar", max compression
```

## Comparing `conjuring-0.5.0.tar` & `conjuring-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     1455 2023-05-22 01:07:03.669380 conjuring-0.5.0/docs/README.md
--rw-r--r--   0        0        0     9175 2023-05-22 01:07:03.669380 conjuring-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4393 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/__init__.py
--rw-r--r--   0        0        0      541 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/colors.py
--rw-r--r--   0        0        0      398 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/constants.py
--rw-r--r--   0        0        0    10397 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/grimoire.py
--rw-r--r--   0        0        0        0 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/__init__.py
--rw-r--r--   0        0        0     2191 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/aws.py
--rw-r--r--   0        0        0     3018 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/blanket.py
--rw-r--r--   0        0        0     2058 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/conjuring.py
--rw-r--r--   0        0        0     1240 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/docker.py
--rw-r--r--   0        0        0     1725 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/duplicity.py
--rw-r--r--   0        0        0     1018 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/fork.py
--rw-r--r--   0        0        0    14779 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/git.py
--rw-r--r--   0        0        0     1008 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/jrnl.py
--rw-r--r--   0        0        0     2967 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/k8s.py
--rw-r--r--   0        0        0     7050 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/media.py
--rw-r--r--   0        0        0      777 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/mkdocs.py
--rw-r--r--   0        0        0     2647 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/mr.py
--rw-r--r--   0        0        0      824 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/onedrive.py
--rw-r--r--   0        0        0    11612 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/paperless.py
--rw-r--r--   0        0        0     2724 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/pre_commit.py
--rw-r--r--   0        0        0     9187 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/py.py
--rw-r--r--   0        0        0     1081 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/shell.py
--rw-r--r--   0        0        0     1928 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/visibility.py
--rw-r--r--   0        0        0     2573 1970-01-01 00:00:00.000000 conjuring-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1629 2023-05-24 21:03:33.289764 conjuring-0.6.0/docs/README.md
+-rw-r--r--   0        0        0     3002 2023-05-24 21:03:33.289764 conjuring-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4393 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/__init__.py
+-rw-r--r--   0        0        0      564 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/colors.py
+-rw-r--r--   0        0        0      605 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/constants.py
+-rw-r--r--   0        0        0    11407 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/grimoire.py
+-rw-r--r--   0        0        0       50 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/__init__.py
+-rw-r--r--   0        0        0     2392 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/aws.py
+-rw-r--r--   0        0        0     2089 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/conjuring.py
+-rw-r--r--   0        0        0     1319 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/direnv.py
+-rw-r--r--   0        0        0     1366 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/docker.py
+-rw-r--r--   0        0        0     1928 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/duplicity.py
+-rw-r--r--   0        0        0     1126 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/fork.py
+-rw-r--r--   0        0        0     3277 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/generic.py
+-rw-r--r--   0        0        0    15370 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/git.py
+-rw-r--r--   0        0        0     1288 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/jrnl.py
+-rw-r--r--   0        0        0     3289 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/k8s.py
+-rw-r--r--   0        0        0     7568 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/media.py
+-rw-r--r--   0        0        0      949 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/mkdocs.py
+-rw-r--r--   0        0        0     2807 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/mr.py
+-rw-r--r--   0        0        0      966 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/onedrive.py
+-rw-r--r--   0        0        0    12527 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/paperless.py
+-rw-r--r--   0        0        0     2946 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/pre_commit.py
+-rw-r--r--   0        0        0     9810 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/py.py
+-rw-r--r--   0        0        0     1151 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/shell.py
+-rw-r--r--   0        0        0     2690 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/visibility.py
+-rw-r--r--   0        0        0     2768 1970-01-01 00:00:00.000000 conjuring-0.6.0/PKG-INFO
```

### Comparing `conjuring-0.5.0/docs/README.md` & `conjuring-0.6.0/docs/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+<!-- markdownlint-disable-file MD031 -->
+
+[//]: # "It breaks numbered lists on Mkdocs"
+[//]: # "MD031/blanks-around-fences Fenced code blocks should be surrounded by blank lines"
+
 # Conjuring
 
 Reusable global [Invoke](https://github.com/pyinvoke/invoke) tasks that can be
 merged with local project tasks.
 
 ## Features
 
@@ -21,25 +26,19 @@
 
 Each module under [the `conjuring/spells` directory](https://github.com/andreoliwa/conjuring/tree/master/src/conjuring/spells)
 is a collection of Invoke tasks.
 
 ## Quick setup
 
 1. Install Conjuring in an isolated virtualenv with [pipx](https://github.com/pypa/pipx):
-
    ```shell
    pipx install --include-deps conjuring
    ```
-
    The `--include-deps` flag is needed to install Invoke's apps (`invoke` and `inv`).
-
 2. Create a `tasks.py` file on your home dir:
-
    ```shell
    echo -e "from conjuring import *\n\nnamespace = cast_all_spells()" > ~/tasks.py
    ```
-
 3. You should see the list of Conjuring tasks from any directory where you type this:
-
    ```shell
    invoke --list
    ```
```

### Comparing `conjuring-0.5.0/src/conjuring/__init__.py` & `conjuring-0.6.0/src/conjuring/__init__.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.5.0/src/conjuring/colors.py` & `conjuring-0.6.0/src/conjuring/colors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-00000000: 434f 4c4f 525f 4e4f 4e45 203d 2022 5c30  COLOR_NONE = "\0
-00000010: 3333 5b30 6d22 0a43 4f4c 4f52 5f42 4c41  33[0m".COLOR_BLA
-00000020: 434b 203d 2022 5c30 3333 5b33 306d 220a  CK = "\033[30m".
-00000030: 434f 4c4f 525f 5245 4420 3d20 225c 3033  COLOR_RED = "\03
-00000040: 335b 3331 6d22 0a43 4f4c 4f52 5f47 5245  3[31m".COLOR_GRE
-00000050: 454e 203d 2022 5c30 3333 5b33 326d 220a  EN = "\033[32m".
-00000060: 434f 4c4f 525f 5945 4c4c 4f57 203d 2022  COLOR_YELLOW = "
-00000070: 5c30 3333 5b33 336d 220a 434f 4c4f 525f  \033[33m".COLOR_
-00000080: 424c 5545 203d 2022 5c30 3333 5b33 346d  BLUE = "\033[34m
-00000090: 220a 434f 4c4f 525f 5055 5250 4c45 203d  ".COLOR_PURPLE =
-000000a0: 2022 5c30 3333 5b33 356d 220a 434f 4c4f   "\033[35m".COLO
-000000b0: 525f 4359 414e 203d 2022 5c30 3333 5b33  R_CYAN = "\033[3
-000000c0: 366d 220a 434f 4c4f 525f 5748 4954 4520  6m".COLOR_WHITE 
-000000d0: 3d20 225c 3033 335b 3337 6d22 0a0a 434f  = "\033[37m"..CO
-000000e0: 4c4f 525f 4c49 4748 545f 4752 4545 4e20  LOR_LIGHT_GREEN 
-000000f0: 3d20 225c 3033 335b 313b 3332 6d22 0a43  = "\033[1;32m".C
-00000100: 4f4c 4f52 5f4c 4947 4854 5f52 4544 203d  OLOR_LIGHT_RED =
-00000110: 2022 5c30 3333 5b31 3b33 316d 220a 0a43   "\033[1;31m"..C
-00000120: 4f4c 4f52 5f42 4f4c 445f 424c 4143 4b20  OLOR_BOLD_BLACK 
-00000130: 3d20 225c 3033 335b 313b 3330 6d22 0a43  = "\033[1;30m".C
-00000140: 4f4c 4f52 5f42 4f4c 445f 5245 4420 3d20  OLOR_BOLD_RED = 
-00000150: 225c 3033 335b 313b 3331 6d22 0a43 4f4c  "\033[1;31m".COL
-00000160: 4f52 5f42 4f4c 445f 4752 4545 4e20 3d20  OR_BOLD_GREEN = 
-00000170: 225c 3033 335b 313b 3332 6d22 0a43 4f4c  "\033[1;32m".COL
-00000180: 4f52 5f42 4f4c 445f 5945 4c4c 4f57 203d  OR_BOLD_YELLOW =
-00000190: 2022 5c30 3333 5b31 3b33 336d 220a 434f   "\033[1;33m".CO
-000001a0: 4c4f 525f 424f 4c44 5f42 4c55 4520 3d20  LOR_BOLD_BLUE = 
-000001b0: 225c 3033 335b 313b 3334 6d22 0a43 4f4c  "\033[1;34m".COL
-000001c0: 4f52 5f42 4f4c 445f 5055 5250 4c45 203d  OR_BOLD_PURPLE =
-000001d0: 2022 5c30 3333 5b31 3b33 356d 220a 434f   "\033[1;35m".CO
-000001e0: 4c4f 525f 424f 4c44 5f43 5941 4e20 3d20  LOR_BOLD_CYAN = 
-000001f0: 225c 3033 335b 313b 3336 6d22 0a43 4f4c  "\033[1;36m".COL
-00000200: 4f52 5f42 4f4c 445f 5748 4954 4520 3d20  OR_BOLD_WHITE = 
-00000210: 225c 3033 335b 313b 3337 6d22 0a         "\033[1;37m".
+00000000: 2222 2243 6f6c 6f72 2063 6f6e 7374 616e  """Color constan
+00000010: 7473 2e22 2222 0a43 4f4c 4f52 5f4e 4f4e  ts.""".COLOR_NON
+00000020: 4520 3d20 225c 3033 335b 306d 220a 434f  E = "\033[0m".CO
+00000030: 4c4f 525f 424c 4143 4b20 3d20 225c 3033  LOR_BLACK = "\03
+00000040: 335b 3330 6d22 0a43 4f4c 4f52 5f52 4544  3[30m".COLOR_RED
+00000050: 203d 2022 5c30 3333 5b33 316d 220a 434f   = "\033[31m".CO
+00000060: 4c4f 525f 4752 4545 4e20 3d20 225c 3033  LOR_GREEN = "\03
+00000070: 335b 3332 6d22 0a43 4f4c 4f52 5f59 454c  3[32m".COLOR_YEL
+00000080: 4c4f 5720 3d20 225c 3033 335b 3333 6d22  LOW = "\033[33m"
+00000090: 0a43 4f4c 4f52 5f42 4c55 4520 3d20 225c  .COLOR_BLUE = "\
+000000a0: 3033 335b 3334 6d22 0a43 4f4c 4f52 5f50  033[34m".COLOR_P
+000000b0: 5552 504c 4520 3d20 225c 3033 335b 3335  URPLE = "\033[35
+000000c0: 6d22 0a43 4f4c 4f52 5f43 5941 4e20 3d20  m".COLOR_CYAN = 
+000000d0: 225c 3033 335b 3336 6d22 0a43 4f4c 4f52  "\033[36m".COLOR
+000000e0: 5f57 4849 5445 203d 2022 5c30 3333 5b33  _WHITE = "\033[3
+000000f0: 376d 220a 0a43 4f4c 4f52 5f4c 4947 4854  7m"..COLOR_LIGHT
+00000100: 5f47 5245 454e 203d 2022 5c30 3333 5b31  _GREEN = "\033[1
+00000110: 3b33 326d 220a 434f 4c4f 525f 4c49 4748  ;32m".COLOR_LIGH
+00000120: 545f 5245 4420 3d20 225c 3033 335b 313b  T_RED = "\033[1;
+00000130: 3331 6d22 0a0a 434f 4c4f 525f 424f 4c44  31m"..COLOR_BOLD
+00000140: 5f42 4c41 434b 203d 2022 5c30 3333 5b31  _BLACK = "\033[1
+00000150: 3b33 306d 220a 434f 4c4f 525f 424f 4c44  ;30m".COLOR_BOLD
+00000160: 5f52 4544 203d 2022 5c30 3333 5b31 3b33  _RED = "\033[1;3
+00000170: 316d 220a 434f 4c4f 525f 424f 4c44 5f47  1m".COLOR_BOLD_G
+00000180: 5245 454e 203d 2022 5c30 3333 5b31 3b33  REEN = "\033[1;3
+00000190: 326d 220a 434f 4c4f 525f 424f 4c44 5f59  2m".COLOR_BOLD_Y
+000001a0: 454c 4c4f 5720 3d20 225c 3033 335b 313b  ELLOW = "\033[1;
+000001b0: 3333 6d22 0a43 4f4c 4f52 5f42 4f4c 445f  33m".COLOR_BOLD_
+000001c0: 424c 5545 203d 2022 5c30 3333 5b31 3b33  BLUE = "\033[1;3
+000001d0: 346d 220a 434f 4c4f 525f 424f 4c44 5f50  4m".COLOR_BOLD_P
+000001e0: 5552 504c 4520 3d20 225c 3033 335b 313b  URPLE = "\033[1;
+000001f0: 3335 6d22 0a43 4f4c 4f52 5f42 4f4c 445f  35m".COLOR_BOLD_
+00000200: 4359 414e 203d 2022 5c30 3333 5b31 3b33  CYAN = "\033[1;3
+00000210: 366d 220a 434f 4c4f 525f 424f 4c44 5f57  6m".COLOR_BOLD_W
+00000220: 4849 5445 203d 2022 5c30 3333 5b31 3b33  HITE = "\033[1;3
+00000230: 376d 220a                                7m".
```

### Comparing `conjuring-0.5.0/src/conjuring/grimoire.py` & `conjuring-0.6.0/src/conjuring/grimoire.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,105 +1,120 @@
+"""Helper functions used in other modules."""
 from __future__ import annotations
 
 import fnmatch
 import os
 import sys
 import time
-import types
 from collections import defaultdict
-from collections.abc import Sequence
 from dataclasses import dataclass
 from importlib import import_module
 from pathlib import Path
 from shlex import quote
-from typing import Callable
+from shutil import which
+from typing import TYPE_CHECKING, Callable
 
+import typer
 from invoke import Collection, Context, Result, Task
 
 from conjuring.colors import COLOR_BOLD_WHITE, COLOR_LIGHT_GREEN, COLOR_LIGHT_RED, COLOR_NONE, COLOR_YELLOW
 from conjuring.visibility import display_task
 
+if TYPE_CHECKING:
+    import types
+    from collections.abc import Sequence
+
 CONJURING_IGNORE_MODULES = os.environ.get("CONJURING_IGNORE_MODULES", "").split(",")
 
 
 def join_pieces(*pieces: str) -> str:
     """Join pieces, ignoring empty strings."""
     return " ".join(str(piece) for piece in pieces if str(piece).strip())
 
 
-def run_command(c: Context, *pieces: str, dry: bool | None = None, **kwargs) -> Result:
+def run_command(c: Context, *pieces: str, dry: bool | None = None, **kwargs: str | bool) -> Result:
     """Build command from pieces, ignoring empty strings."""
     if dry is not None:
         kwargs.setdefault("dry", dry)
     kwargs.setdefault("warn", False)
     kwargs.setdefault("hide", False)
     return c.run(join_pieces(*pieces), **kwargs)
 
 
-def run_stdout(c: Context, *pieces: str, **kwargs) -> str:
+def run_stdout(c: Context, *pieces: str, **kwargs: str | bool) -> str:
     """Run a (hidden) command and return the stripped stdout."""
     kwargs.setdefault("warn", False)
     kwargs.setdefault("hide", True)
     kwargs.setdefault("pty", False)
     return c.run(join_pieces(*pieces), **kwargs).stdout.strip()
 
 
-def run_lines(c: Context, *pieces: str, **kwargs) -> list[str]:
+def run_lines(c: Context, *pieces: str, **kwargs: str | bool) -> list[str]:
     """Run a (hidden) command and return the result as lines."""
     return run_stdout(c, *pieces, **kwargs).splitlines()
 
 
-def run_multiple(c: Context, *commands: str, **kwargs) -> None:
+def run_multiple(c: Context, *commands: str, **kwargs: str | bool) -> None:
     """Run multiple commands from a list, ignoring empty ones."""
     for cmd in [c for c in commands if str(c).strip()]:
         c.run(cmd, **kwargs)
 
 
-def print_color(*message: str, color=COLOR_NONE, nl=False):
+def print_color(*message: str, color: str = COLOR_NONE, nl: bool = False) -> None:
     """Print a colored message."""
     all_messages = ("\n" if nl else " ").join(message)
-    print(f"{color}{all_messages}{COLOR_NONE}")
+    typer.echo(f"{color}{all_messages}{COLOR_NONE}")
 
 
-def print_success(*message: str, nl=False):
+def print_success(*message: str, nl: bool = False) -> None:
     """Print a success message."""
     print_color(*message, color=COLOR_LIGHT_GREEN, nl=nl)
 
 
-def print_error(*message: str, nl=False):
+def print_error(*message: str, nl: bool = False) -> None:
     """Print an error message."""
     print_color(*message, color=COLOR_LIGHT_RED, nl=nl)
 
 
-def print_warning(*message: str, nl=False):
+def print_warning(*message: str, nl: bool = False) -> None:
     """Print a warning message."""
     print_color(*message, color=COLOR_YELLOW, nl=nl)
 
 
 def ask_user_prompt(*message: str, color: str = COLOR_BOLD_WHITE, allowed_keys: str = "") -> str:
     """Display a prompt with a message. Wait a little before, so stdout is flushed before the input message."""
     lowercase_key_list = [char.lower() for char in allowed_keys] if allowed_keys else []
     options = "/".join(allowed_keys) if allowed_keys else None
     prefix = f"Type {options} +" if allowed_keys else "Press"
 
     while True:
-        print()
+        typer.echo()
         print_color(*message, color=color)
         time.sleep(0.2)
 
         typed_input = input(f"{prefix} ENTER to continue or Ctrl-C to abort: ")
         if not allowed_keys:
             return typed_input
 
         lowercase_key = typed_input.lower()
         if lowercase_key in lowercase_key_list:
             return lowercase_key
 
 
-def run_with_fzf(c: Context, *pieces: str, query="", header="", multi=False, options="", preview="", **kwargs) -> str:
+# TODO: Use iterfzf or create Fzf class with multi() and single() methods (with different return types
+def run_with_fzf(  # noqa: PLR0913
+    c: Context,
+    *pieces: str,
+    query: str = "",
+    header: str = "",
+    multi: bool = False,
+    options: str = "",
+    preview: str = "",
+    **kwargs: str | bool,
+) -> str:
     """Run a command with fzf and return the chosen entry."""
     fzf_pieces = ["| fzf --reverse --select-1 --height 40% --cycle"]
     if query:
         fzf_pieces.append(f"-q '{query}'")
     if header:
         fzf_pieces.append(f"--header='{header}'")
     if multi:
@@ -118,60 +133,65 @@
 
 def ignore_module(module_name: str) -> bool:
     """Ignore a module by its name."""
     return any(ignore_str and ignore_str in module_name for ignore_str in CONJURING_IGNORE_MODULES)
 
 
 def resolve_module_str(module_or_str: types.ModuleType | str) -> types.ModuleType | None:
+    """Resolve a module from a string or return it if it's already a module."""
     if isinstance(module_or_str, str):
         module = import_module(module_or_str)
         if ignore_module(module_or_str):
             return None
     else:
         module = module_or_str
         if ignore_module(module.__name__):
             return None
     return module
 
 
 def slugify(name: str) -> str:
+    """Slugify a name."""
     return name.replace(".", "_")
 
 
 def guess_full_task_name(prefix: str | None, name: str) -> str:
     """Guess how Invoke will name this task.
 
     NOTE: this is unstable and may break because Invoke has no public API to get the final task name.
     """
     formatted_task_name = slugify(name).replace("_", "-")
     return f"{prefix}.{formatted_task_name}" if prefix else formatted_task_name
 
 
 @dataclass
 class SpellBook:
+    """A collection of Invoke tasks from a module, with a prefix."""
+
     prefix: str
     module: types.ModuleType
     display_all_tasks: bool
 
 
 def _is_task_present(name: str, list_: Sequence[str] | None) -> bool:
     if not list_:
         return True
     return any(fnmatch.fnmatch(name, element) for element in list_)
 
 
-def add_single_task_to(
+def add_single_task_to(  # noqa: PLR0913
     collection: Collection,
     task: Task,
     include: Sequence[str] | None,
     exclude: Sequence[str] | None,
     *,
     prefix: str | None,
     task_name: str | None,
 ) -> bool:
+    """Add a single task to the collection if it matches the include/exclude filters."""
     guessed_name = guess_full_task_name(prefix, task.name)
     should_include = not include or _is_task_present(guessed_name, include)
     should_exclude = exclude and _is_task_present(guessed_name, exclude)
     if should_include and not should_exclude:
         if task_name:
             collection.add_task(task, task_name)
         else:
@@ -237,19 +257,19 @@
                 if "this collection has a task name" in str(err):
                     to_collection.add_collection(spell_book.module, prefix + "_" + slugify(spell_book.module.__name__))
                     continue
                 raise
 
 
 def collection_from_python_files(
-    current_module,
+    current_module: types.ModuleType | str,
     *py_glob_patterns: str,
     include: Sequence[str] | None = None,
     exclude: Sequence[str] | None = None,
-):
+) -> Collection:
     """Create a custom collection by adding tasks from multiple files.
 
     Search directories for glob patterns:
     1. Root dir.
     2. Current dir.
 
     If the current dir is the root, tasks won't be duplicated.
@@ -277,10 +297,16 @@
     return main_colllection
 
 
 def lazy_env_variable(variable: str, description: str) -> str:
     """Fetch environment variable. On error, display a message with its description."""
     try:
         return os.environ[variable]
-    except KeyError:
+    except KeyError as err:
         print_error(f"Set the {variable!r} environment variable with the {description}.")
-        raise SystemExit
+        raise SystemExit from err
+
+
+def bat(c: Context, *pieces: str) -> Result:
+    """Display files with "bat" if it's installed. Otherwise, fallback to "cat"."""
+    tool = "bat" if which("bat") else "cat"
+    return run_command(c, tool, *pieces)
```

### Comparing `conjuring-0.5.0/src/conjuring/spells/aws.py` & `conjuring-0.6.0/src/conjuring/spells/aws.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,68 +1,70 @@
+"""AWS: ECR login, ..."""
 import os
 from typing import Optional
 from urllib.parse import urlparse
 
-from invoke import Context, task
+import typer
+from invoke import Context, Result, task
 
+from conjuring.constants import AWS_CONFIG
 from conjuring.grimoire import run_command, run_lines, run_with_fzf
 
-AWS_CONFIG = "~/.aws/config"
-
 LIST_AWS_PROFILES_COMMAND = rf"rg -o '\[profile[^\]]+' {AWS_CONFIG} | cut -d ' ' -f 2"
 
 SHOULD_PREFIX = True
 
 
 def list_aws_profiles(c: Context) -> list[str]:
     """List AWS profiles from the config file."""
     return run_lines(c, LIST_AWS_PROFILES_COMMAND)
 
 
-def fzf_aws_profile(c, partial_name: Optional[str] = None) -> str:
+def fzf_aws_profile(c: Context, partial_name: Optional[str] = None) -> str:
     """Select an AWS profile from a partial profile name using fzf."""
     if not partial_name and (aws_profile := os.environ.get("AWS_PROFILE")) and aws_profile:
-        print(f"Using env variable AWS_PROFILE (set to '{aws_profile}')")
+        typer.echo(f"Using env variable AWS_PROFILE (set to '{aws_profile}')")
         return aws_profile
 
-    return run_with_fzf(c, LIST_AWS_PROFILES_COMMAND, query=partial_name)
+    return run_with_fzf(c, LIST_AWS_PROFILES_COMMAND, query=partial_name or "")
 
 
-def fzf_aws_account(c) -> str:
+def fzf_aws_account(c: Context) -> str:
     """Select an AWS account from the config file."""
     return run_with_fzf(c, f"rg -o 'aws:iam::[^:]+' {AWS_CONFIG} | cut -d ':' -f 4 | sort -u")
 
 
-def fzf_aws_region(c) -> str:
+def fzf_aws_region(c: Context) -> str:
     """Select an AWS region from the config file."""
     return run_with_fzf(c, f"rg -o '^region.+' {AWS_CONFIG} | tr -d ' ' | cut -d'=' -f 2 | sort -u")
 
 
-def run_aws_vault(c, *pieces, profile: Optional[str] = None):
+def run_aws_vault(c: Context, *pieces: str, profile: Optional[str] = None) -> Result:
     """Run AWS vault commands in a subshell, or open a subshell if no commands were provided."""
-    run_command(c, "aws-vault exec", fzf_aws_profile(c, profile), "--", *pieces, pty=False)
+    return run_command(c, "aws-vault exec", fzf_aws_profile(c, profile), "--", *pieces, pty=False)
 
 
-def clean_aws_url(c, url: Optional[str] = None):
+def clean_ecr_url(c: Context, url: Optional[str] = None) -> str:
+    """Clean an AWS ECR URL."""
     if not url:
         account = fzf_aws_account(c)
         region = fzf_aws_region(c)
         return f"{account}.dkr.ecr.{region}.amazonaws.com"
     return urlparse(url).netloc
 
 
 @task
-def ecr_login(c, url=""):
+def ecr_login(c: Context, url: str = "") -> None:
     """Log in to AWS ECR.
 
     Using Amazon ECR with the AWS CLI - Amazon ECR:
     https://docs.aws.amazon.com/AmazonECR/latest/userguide/getting-started-cli.html#cli-authenticate-registry
     """
     profile = fzf_aws_profile(c)
-    url = clean_aws_url(c, url)
+    url = clean_ecr_url(c, url)
     run_command(
         c,
         "aws ecr get-login-password --profile",
         profile,
         "| docker login --username AWS --password-stdin",
         url,
     )
```

### Comparing `conjuring-0.5.0/src/conjuring/spells/blanket.py` & `conjuring-0.6.0/src/conjuring/spells/generic.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,77 +1,89 @@
-"""Generic spells that don't have a prefix and don't fit other modules."""
+"""Generic spells: list to-do items in files, ..."""
 from __future__ import annotations
 
 from collections import defaultdict
 from dataclasses import dataclass
 from shlex import quote
 
-from invoke import task
+import typer
+from invoke import Context, task
 
 from conjuring.grimoire import print_error, print_success, run_command, run_lines
 
 # Split the strings to prevent this method from detecting them as tasks when running on this own project
-FIX_ME = "FIX" + "ME"
-TO_DO = "TO" + "DO"
+FIX_ME = "FIX" + "ME"  # noqa: ISC003
+TO_DO = "TO" + "DO"  # noqa: ISC003
 
 
 @dataclass(frozen=True)
-class Task:
+class ToDoItem:
+    """A to-do item."""
+
     which: str
     description: str
 
     @property
-    def sort_key(self):
+    def sort_key(self) -> str:
         """Key to sort the instance.
 
         String concatenation works.
         Checking both fields separately with ``and`` conditions didn't work: sort order was not as expected
         (meaning fix-me tasks first, then to-do tasks).
         """
         return f"{self.which}-{self.description.lower()}"
 
-    def __lt__(self, other: Task) -> bool:
+    def __lt__(self, other: ToDoItem) -> bool:
         return self.sort_key < other.sort_key
 
 
 @dataclass
 class Location:
+    """Location of a to-do item in a file."""
+
     file: str
     line: int
     comment: str
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         self.line = int(self.line)
         self.comment = self.comment.strip()
 
 
 @task(
     help={
         "cz": "Run commitizen (cz check) to validate the description of the to-do item as a commit message",
         "valid": "When using cz check, print valid to-do items",
         "invalid": "When using cz check, print invalid to-do items",
         "short": "Short format: only the description, without the lines of code where to-do items were found",
         "priority": f"Show only higher priority tasks ({FIX_ME})",
     },
 )
-def todo(c, cz=False, valid=True, invalid=True, short=False, priority=False):
+def todo(  # noqa: PLR0913
+    c: Context,
+    cz: bool = False,
+    valid: bool = True,
+    invalid: bool = True,
+    short: bool = False,
+    priority: bool = False,
+) -> None:
     """List to-dos and fix-mes in code. Optionally check if the description follows Conventional Commits (cz check)."""
-    all_todos: dict[Task, list[Location]] = defaultdict(list)
-    all_keys: list[Task] = []
+    all_todos: dict[ToDoItem, list[Location]] = defaultdict(list)
+    all_keys: list[ToDoItem] = []
 
     for which in (FIX_ME,) if priority else (FIX_ME, TO_DO):
         # This command freezes if pty=False
         for line in run_lines(c, f"rg --color=never --no-heading {which}", warn=True, pty=True):
             before, after = line.split(which, maxsplit=1)  # type: str,str
-            key = Task(which, after.strip(": "))
+            key = ToDoItem(which, after.strip(": "))
             all_keys.append(key)
-            location = Location(*before.strip("/# ").split(":", maxsplit=2))  # type: ignore
+            location = Location(*before.strip("/# ").split(":", maxsplit=2))  # type: ignore[arg-type]
             all_todos[key].append(location)
 
-    for item, locations in sorted(all_todos.items()):  # type: Task, list[Location]
+    for item, locations in sorted(all_todos.items()):  # type: ToDoItem, list[Location]
         func = print_success
         if cz:
             result = run_command(c, "cz check -m", quote(item.description), hide=True, warn=True)
             if result.ok:
                 if not valid:
                     continue
             else:
@@ -80,8 +92,8 @@
                 func = print_error
 
         func(f"{item.which}: {item.description}")
 
         if short:
             continue
         for loc in locations:  # type: Location
-            print(f"   {loc.file}:{loc.line} {loc.comment}")
+            typer.echo(f"   {loc.file}:{loc.line} {loc.comment}")
```

### Comparing `conjuring-0.5.0/src/conjuring/spells/conjuring.py` & `conjuring-0.6.0/src/conjuring/spells/conjuring.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,51 @@
+"""Init Invoke configuration files for Conjuring."""
 from pathlib import Path
 
-from invoke import task
+import typer
+from invoke import Context, task
 
-from conjuring.constants import CONJURING_INIT, INVOKE_YAML
+from conjuring.constants import CONJURING_INIT, ROOT_INVOKE_YAML
 from conjuring.grimoire import print_success, print_warning, run_command, run_stdout
 
 SHOULD_PREFIX = True
 
 
 @task(
     help={
         "edit": "Open the config file with $EDITOR",
         "revert": "Revert the changes and go back to using tasks.py as the default tasks file",
     },
 )
-def init(c, edit=False, revert=False):
+def init(c: Context, edit: bool = False, revert: bool = False) -> None:
     """Init Conjuring on your home dir to merge any local `tasks.py` file with global Conjuring tasks."""
-    config_file = INVOKE_YAML
+    config_file = ROOT_INVOKE_YAML
 
     json_config = f"""'{{"tasks":{{"collection_name":"{CONJURING_INIT}"}}'"""
     if config_file.exists():
         current_collection_name = run_stdout(c, f"yq e '.tasks.collection_name' {config_file}")
         if current_collection_name == CONJURING_INIT:
             print_success(f"Configuration file is already set to {CONJURING_INIT!r}")
             run_command(c, f"cat {config_file}")
         else:
             message = "Remove this from" if revert else "Add this to"
-            print(f"The {config_file} configuration file already exists! {message} the file:")
+            typer.echo(f"The {config_file} configuration file already exists! {message} the file:")
             run_command(c, "yq eval -n", json_config)
             if edit:
                 run_command(c, "$EDITOR", str(config_file))
-    else:
-        if not revert:
-            c.run(f"touch {config_file}")
-            run_command(c, "yq eval -i", json_config, str(config_file))
-            c.run(f"cat {config_file}")
+    elif not revert:
+        c.run(f"touch {config_file}")
+        run_command(c, "yq eval -i", json_config, str(config_file))
+        c.run(f"cat {config_file}")
 
     default_tasks = Path("~/tasks.py").expanduser()
     conjuring_init = Path(f"~/{CONJURING_INIT}.py").expanduser()
     if revert:
         if conjuring_init.exists():
             conjuring_init.rename(default_tasks)
+    elif default_tasks.exists():
+        default_tasks.rename(conjuring_init)
+    elif conjuring_init.exists():
+        print_success("Global tasks file already exists.")
+        run_command(c, f"cat {conjuring_init}")
     else:
-        if default_tasks.exists():
-            default_tasks.rename(conjuring_init)
-        else:
-            if conjuring_init.exists():
-                print_success("Global tasks file already exists.")
-                run_command(c, f"cat {conjuring_init}")
-            else:
-                print_warning(f"Nothing to do: file {default_tasks} does not exist!")
+        print_warning(f"Nothing to do: file {default_tasks} does not exist!")
```

### Comparing `conjuring-0.5.0/src/conjuring/spells/docker.py` & `conjuring-0.6.0/src/conjuring/spells/docker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from invoke import task
+"""Docker: remove containers, volumes and more.."""
+from invoke import Context, task
 
 from conjuring.grimoire import print_error, run_command
 
 SHOULD_PREFIX = True
 
 
 @task(
     help={
         "container": "Container name to remove (regexp)",
         "all_": "All containers",
         "exited": "Exited containers",
     },
 )
-def rm_containers(c, container="", all_=False, exited=False):
+def rm_containers(c: Context, container: str = "", all_: bool = False, exited: bool = False) -> None:
     """Remove Docker containers."""
     cmd = []
     if all_:
         cmd = ["docker ps -a"]
     elif exited:
         cmd = ["docker ps -a -f status=exited"]
     elif container:
@@ -27,15 +28,15 @@
 
     run_command(c, *cmd, dry=False)
     run_command(c, *cmd, "| tail +2 | awk '{print $1}' | xargs docker rm -f")
     run_command(c, *cmd)
 
 
 @task(help=({"dangling": "Dangling volumes"}))
-def rm_volumes(c, dangling=False):
+def rm_volumes(c: Context, dangling: bool = False) -> None:
     """Remove Docker volumes."""
     cmd = ""
     if dangling:
         cmd = 'docker volume ls -f "dangling=true"'
     if not cmd:
         print_error("Choose one argument. Run with --help to see available argument")
         return
```

### Comparing `conjuring-0.5.0/src/conjuring/spells/duplicity.py` & `conjuring-0.6.0/src/conjuring/spells/duplicity.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,39 @@
+"""Backup and restore with Duplicity https://duplicity.us/."""
 from pathlib import Path
 from string import Template
 from tempfile import NamedTemporaryFile
 
-from invoke import task
+import typer
+from invoke import Context, task
 
 from conjuring.grimoire import run_command, run_with_fzf
 
 SHOULD_PREFIX = True
 BACKUP_DIR = Path("~/OneDrive/Backup").expanduser()
 
 
-def print_hostname(c):
+def print_hostname(c: Context) -> str:
+    """Print the hostname of the current machine."""
     host = c.run("hostname | sed 's/.local//'").stdout.strip()
-    print(f"Host: {host}")
+    typer.echo(f"Host: {host}")
     return host
 
 
 @task
-def backup(c):
+def backup(c: Context) -> None:
     """Backup files with Duplicity."""
     host = print_hostname(c)
     backup_dir = f"file://{BACKUP_DIR}/{host}/duplicity/"
     # To back up directly on OneDrive:
     # backup_dir = f"onedrive://Backup/{host}/duplicity/"
-    print(f"Backup dir: {backup_dir}")
+    typer.echo(f"Backup dir: {backup_dir}")
 
     template_file = Path("~/dotfiles/duplicity-template.cfg").expanduser()
-    print(f"Template file: {template_file}")
+    typer.echo(f"Template file: {template_file}")
 
     template_contents = template_file.read_text()
     duplicity_config = Template(template_contents).substitute({"HOME": Path.home()})
 
     with NamedTemporaryFile("r+", delete=False) as temp_file:
         temp_file.write(duplicity_config)
         temp_file.flush()
@@ -42,15 +45,15 @@
             f"--include-filelist={temp_file.name}",
             "--exclude='**' $HOME/",
             backup_dir,
         )
 
 
 @task
-def restore(c):
+def restore(c: Context) -> None:
     """Restore files with Duplicity. You will be prompted to choose the source dir. Restore dir is ~/Downloads."""
     print_hostname(c)
     chosen_dir = run_with_fzf(c, f"fd -d 2 -t d duplicity {BACKUP_DIR}")
     if not chosen_dir:
         return
 
     source_computer = Path(chosen_dir).parent.name
```

### Comparing `conjuring-0.5.0/src/conjuring/spells/fork.py` & `conjuring-0.6.0/src/conjuring/spells/fork.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from invoke import Exit, task
+"""GitHub forks: configure remote, sync..."""
+from invoke import Context, Exit, task
 
 from conjuring.spells.git import Git
 
 SHOULD_PREFIX = True
 
 
 @task
-def remote(c, username, remote=""):
+def remote(c: Context, username: str, remote: str = "") -> None:
     """Configure a remote for a fork.
 
     https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/configuring-a-remote-for-a-fork
     """
     if username.startswith("-"):
         msg = "Arguments should be: username [--remote]"
         raise Exit(msg)
@@ -19,15 +20,15 @@
 
     project = c.run(r"git remote -v | rg origin | head -1 | rg -o '/(.+)\.git' -r '$1'", pty=False).stdout.strip()
     c.run(f"git remote add {remote} https://github.com/{username}/{project}.git", warn=True)
     c.run("git remote -v")
 
 
 @task
-def sync(c, remote="upstream"):
+def sync(c: Context, remote: str = "upstream") -> None:
     """Sync a fork.
 
     https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/syncing-a-fork
     """
     c.run(f"git fetch {remote}")
     existing_branch = Git(c).checkout("master", "main")
     c.run(f"git merge {remote}/{existing_branch}")
```

### Comparing `conjuring-0.5.0/src/conjuring/spells/git.py` & `conjuring-0.6.0/src/conjuring/spells/git.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+"""Git: update all, extract subtree, rewrite history, ..."""
 import re
 from configparser import ConfigParser
 from dataclasses import dataclass
 from functools import lru_cache
 from pathlib import Path
 
+import typer
 from invoke import Context, Exit, UnexpectedExit, task
 
 from conjuring.colors import COLOR_LIGHT_RED, COLOR_NONE
 from conjuring.grimoire import (
     print_error,
     print_success,
     run_command,
@@ -52,54 +54,58 @@
         )
 
     def checkout(self, *branches: str) -> str:
         """Try checking out the specified branches in order."""
         for branch in branches:
             try:
                 self.context.run(f"git checkout {branch}")
-                return branch
             except UnexpectedExit:
                 pass
+            else:
+                return branch
         return ""
 
     @property
     def github_username(self) -> str:
         """The GitHub username configured in the global settings."""
         return global_config()["github"]["user"]
 
     def choose_local_branch(self, branch: str) -> str:
+        """Choose a local branch."""
         return run_with_fzf(self.context, "git branch --list | rg -v develop | cut -b 3-", query=branch)
 
 
 @dataclass(frozen=True)
 class PrefixBranch:
+    """Tuple of prefix and branch name."""
+
     prefix: str
     branch: str
 
 
 @task(klass=MagicTask)
-def update_all(c, group=""):
+def update_all(c: Context, group: str = "") -> None:
     """Run gita super to update and clean branches."""
     parts = ["gita", "super"]
     if group:
         parts.append(group)
     gita_super = " ".join(parts)
     c.run(f"{gita_super} up && {gita_super} delete-merged-branches")
 
 
 @task
-def switch_url_to(c, remote="origin", https=False):
+def switch_url_to(c: Context, remote: str = "origin", https: bool = False) -> None:
     """Set an SSH or HTTPS URL for a remote."""
     regex = r"'git@(.+\.com):(.+/.+)\.git\s'" if https else r"'/([^/]+\.com)/([^/]+/.+)\s\('"
     replace = "'$1/$2'" if https else "'$1:$2'"
 
     result = c.run(f"git remote -v | rg {remote} | head -1 | rg -o {regex} -r {replace}", warn=True, pty=False)
     match = result.stdout.strip()
     if not match:
-        print(f"{COLOR_LIGHT_RED}Match not found{COLOR_NONE}")
+        typer.echo(f"{COLOR_LIGHT_RED}Match not found{COLOR_NONE}")
     else:
         repo = f"https://{match}" if https else f"git@{match}"
         if not repo.endswith(".git"):
             repo += ".git"
         c.run(f"git remote set-url {remote} {repo}")
 
     c.run("git remote -v")
@@ -108,15 +114,15 @@
 @task(
     help={
         "new_project_dir": "Dir of the project to be created. The dir might exist or not",
         "reset": "Remove the new dir and start over",
         "keep": "Keep branches and remote after the extracting is done",
     },
 )
-def extract_subtree(c, new_project_dir, reset=False, keep=False):
+def extract_subtree(c: Context, new_project_dir: str, reset: bool = False, keep: bool = False) -> None:
     """Extract files from subdirectories of the current Git repo to another repo, using git subtree.
 
     The files will be moved to the root of the new repo.
 
     Solutions adapted from:
     - https://serebrov.github.io/html/2021-09-13-git-move-history-to-another-repository.html
     - https://stackoverflow.com/questions/25574407/git-subtree-split-two-directories/58253979#58253979
@@ -212,15 +218,15 @@
     help={
         "full": "Display all info: files, authors, dates",
         "files": "Display all files in Git history, even the ones that were deleted and don't exist anymore",
         "author": "Display authors",
         "dates": "Display committer and author dates in different colors",
     },
 )
-def history(c, full=False, files=False, author=False, dates=False):
+def history(c: Context, full: bool = False, files: bool = False, author: bool = False, dates: bool = False) -> None:
     """Grep the whole Git log and display information."""
     option_chosen = False
     if full:
         option_chosen = True
         files = author = dates = True
     if files:
         option_chosen = True
@@ -231,15 +237,15 @@
     if dates:
         option_chosen = True
         header = True
         for line in run_lines(c, 'git log --format="%H|%cI|%aI|%GK|%s"', hide=False):
             if header:
                 print_success("Green = dates are equal")
                 print_error("Red = dates are different")
-                print(
+                typer.echo(
                     "Commit                                   Committer Date            "
                     "Author Date               GPG key          Subject",
                 )
                 header = False
 
             fields = line.split("|")
             committer_date = fields[1]
@@ -254,15 +260,15 @@
 @task(
     help={
         "commit": "Base commit to be used for the range (default: --root)",
         "gpg": "Sign the commit (default: True)",
         "author": "Set the current author (from 'git config') on the commit range",
     },
 )
-def rewrite(c, commit="--root", gpg=True, author=True):
+def rewrite(c: Context, commit: str = "--root", gpg: bool = True, author: bool = True) -> None:
     """Rewrite a range of commits, signing with GPG and setting the author.
 
     https://git-scm.com/docs/git-commit
     https://git-scm.com/docs/git-rebase
     """
     gpg_flag = " --gpg-sign" if gpg else " --no-gpg-sign"
 
@@ -275,21 +281,21 @@
     c.run(f'git log --format="%H %cI %aI %s" {commit} > $TMPDIR/rebase_sign_hashlist')
     c.run(
         "git rebase --committer-date-is-author-date --exec 'GIT_COMMITTER_DATE="
         '$(fgrep -m 1 "$(git log -1 --format="%aI %s" $GIT_COMMIT)" $TMPDIR/rebase_sign_hashlist'
         f' | cut -d" " -f3) git commit --amend --no-edit -n{author_flag}{gpg_flag}\' -i {commit}',
     )
     history(c, dates=True)
-    print()
-    print("NOTE: If commits were modified during the rebase above, their committer date will be the current date")
-    print("Rebase again with this command, without changing any commit, and all dates should be green")
+    typer.echo()
+    typer.echo("NOTE: If commits were modified during the rebase above, their committer date will be the current date")
+    typer.echo("Rebase again with this command, without changing any commit, and all dates should be green")
 
 
 @task
-def tidy_up(c):
+def tidy_up(c: Context) -> None:
     """Prune remotes, update all branches of the repo, delete merged/squashed branches."""
     c.run("gitup .")
     c.run("git delete-merged-branches")
 
     # warn=True is needed; apparently, this command fails when there is no branch, and execution is stopped
     c.run("git delete-squashed-branches", warn=True)
 
@@ -301,28 +307,34 @@
     help={
         "remote": "List remote branches (default: False)",
         "update": "Update the repo before merging (default: True)",
         "push": "Push the merge to the remote (default: True)",
         "rebase": "Rebase the default branch before merging (default: False)",
     },
 )
-def merge_default(c, remote=False, update=True, push=True, rebase=False):
+def merge_default(
+    c: Context,
+    remote: bool = False,
+    update: bool = True,
+    push: bool = True,
+    rebase: bool = False,
+) -> None:
     """Merge the default branch of the repo. Also set it with "git config", if not already set."""
     default_branch = set_default_branch(c, remote)
 
     if update:
         tidy_up(c)
     which_verb = "rebase" if rebase else "merge"
     run_command(c, f"git {which_verb}", f"origin/{default_branch}")
     if push:
         force_option = "--force-with-lease" if rebase else ""
         run_command(c, "git push", force_option)
 
 
-def set_default_branch(c: Context, remote=False):
+def set_default_branch(c: Context, remote: bool = False) -> str:
     """Set the default branch config on the repo, if not configured yet."""
     cmd_read_default_branch = "git config git-extras.default-branch"
     default_branch = run_stdout(c, cmd_read_default_branch, warn=True, dry=False)
     if not default_branch:
         default_branch = run_with_fzf(
             c,
             "git branch --list",
@@ -335,31 +347,32 @@
     return default_branch
 
 
 @task(
     help={
         "tag": "Name of the tag to compare to (default: last created tag)",
         "files": "Display files instead of commits (default: false)",
-        "verbose": "Files: display changes/insertions/deletion. Commits: display the full commit message, author... (default: False)",
+        "verbose": "Files: display changes/insertions/deletion."
+        " Commits: display the full commit message, author... (default: False)",
     },
 )
-def changes_since_tag(c, tag="", files=False, verbose=False):
+def changes_since_tag(c: Context, tag: str = "", files: bool = False, verbose: bool = False) -> None:
     """Display changes (commits or files) since the last tag (or a chosen tag)."""
     which_tag = tag or run_stdout(c, "git tag --list --sort -creatordate | head -1", hide=False, dry=False)
     default_branch = set_default_branch(c)
     if files:
         option = "" if verbose else " --name-only"
         c.run(f"git diff --stat {which_tag} origin/{default_branch}{option}")
     else:
         option = "" if verbose else " --oneline"
         c.run(f"git log {which_tag}..origin/{default_branch}{option}")
 
 
 @task()
-def watch(c):
+def watch(c: Context) -> None:
     """Watch a build on GitHub Actions, then open a pull request or repo after the build is over."""
     current_branch = Git(c).current_branch()
     print_success(f"Current branch = {current_branch}")
 
     c.run("gh run watch", warn=True)
     out = c.run(f"gh pr view {current_branch} --web", warn=True).stdout.strip()
     if "no pull requests found for branch" in out:
@@ -368,15 +381,15 @@
 
 @task(
     help={
         "prefix": "Keep the Conventional Commits prefix",
         "sort": "Sort bullets",
     },
 )
-def body(c, prefix=True, sort=True):
+def body(c: Context, prefix: bool = True, sort: bool = True) -> None:
     """Prepare a commit body to be used on pull requests and squashed commits."""
     default_branch = set_default_branch(c)
     bullets = []
     for line in run_lines(c, f"git log {default_branch}..", "--format=%s%n%b"):
         clean = line.strip(" -")
         if "Merge branch" in clean or "Revert " in clean or "This reverts" in clean or not clean:
             continue
@@ -387,8 +400,8 @@
 
         # Remove Jira ticket with regex
         clean = re.sub(r"\[?\D+-\d+[\]:]", "", clean).strip(" -")
 
         bullets.append(f"- {clean}")
 
     results = sorted(set(bullets)) if sort else bullets
-    print("\n".join(results))
+    typer.echo("\n".join(results))
```

### Comparing `conjuring-0.5.0/src/conjuring/spells/k8s.py` & `conjuring-0.6.0/src/conjuring/spells/k8s.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Kubernetes."""
+"""Kubernetes: get pods, show variables from config maps, validate score and more."""
 from dataclasses import dataclass
 from typing import Optional, cast
 
 from invoke import Context, Result, task
 
 from conjuring.grimoire import run_command, run_lines, run_with_fzf
 
@@ -11,22 +11,22 @@
 
 @dataclass
 class Kubectl:
     """Kubectl commands."""
 
     context: Context
 
-    def choose_apps(self, partial_app_name: Optional[str] = None, *, multi=False) -> list[str]:
+    def choose_apps(self, partial_app_name: Optional[str] = None, *, multi: bool = False) -> list[str]:
         """Select apps from Kubernetes deployments, using a partial app name and fzf."""
         return cast(
             list[str],
             run_with_fzf(
                 self.context,
                 """kubectl get deployments.apps -o jsonpath='{range .items[*]}{.metadata.name}{"\\n"}{end}'""",
-                query=partial_app_name,
+                query=partial_app_name or "",
                 multi=multi,
             ),
         )
 
     @staticmethod
     def _app_selector(apps: list[str]) -> str:
         """Return the app selector for one or more apps."""
@@ -42,44 +42,48 @@
 
     def run_get(self, resource: str, apps: list[str]) -> Result:
         """Run the kubectl get command for one or more apps."""
         return run_command(self.context, self.cmd_get(resource, apps))
 
 
 @task()
-def validate_score(c):
+def validate_score(c: Context) -> None:
     """Validate and score files that were changed from the master branch."""
     # TODO: handle branches named "main"
     # Continue even if there are errors
     c.run("git diff master.. --name-only | xargs kubeval", warn=True)
     c.run("git diff master.. --name-only | xargs kubectl score")
 
 
 @task(help={"rg": "Filter results with rg"})
-def config_map(c, app, rg=""):
+def config_map(c: Context, app: str, rg: str = "") -> None:
     """Show the config map for an app."""
     chosen_app = Kubectl(c).choose_apps(app)
     run_command(
         c,
         f"kubectl get deployment/{chosen_app} -o json",
         "| jq -r .spec.template.spec.containers[].envFrom[].configMapRef.name",
         "| rg -v null | xargs -I % kubectl get configmap/% -o json | jq -r .data",
         f"| rg {rg}" if rg else "",
     )
 
 
 @task(help={"replica_set": "Show the replica sets for an app"})
-def pods(c, app, replica_set=False):
+def pods(c: Context, app: str, replica_set: bool = False) -> None:
     """Show the pods and replica sets for an app."""
     kubectl = Kubectl(c)
     chosen_apps = kubectl.choose_apps(app, multi=True)
     kubectl.run_get("pods", chosen_apps)
 
     if replica_set:
         replica_set_names = run_lines(
             c,
             kubectl.cmd_get("pods", chosen_apps),
             """-o jsonpath='{range .items[*]}{.metadata.ownerReferences[0].name}{"\\n"}{end}'""",
             "| sort -u",
         )
         for name in replica_set_names:
             run_command(c, f"kubectl get replicaset {name}")
+
+
+# TODO: You can verify the containers running in a given pod with the following command
+#  > kubectl get pods <pod name> -o jsonpath='{.spec.containers[*].name}'
```

### Comparing `conjuring-0.5.0/src/conjuring/spells/media.py` & `conjuring-0.6.0/src/conjuring/spells/media.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,26 @@
+"""Media files: remove empty dirs, clean up picture dirs, download YouTube videos, transcribe audio, ..."""
+from __future__ import annotations
+
 import os
-from datetime import date
+from datetime import datetime, timezone
 from itertools import chain
 from pathlib import Path
 
-from invoke import task
+import typer
+from invoke import Context, task
 
-from conjuring.constants import DESKTOP_DIR, DOT_DS_STORE, DOT_NO_MEDIA, DOWNLOADS_DIR, ONE_DRIVE_DIR, PICTURES_DIR
+from conjuring.constants import (
+    DESKTOP_DIR,
+    DOT_DS_STORE,
+    DOT_NOMEDIA,
+    DOWNLOADS_DIR,
+    ONEDRIVE_DIR,
+    ONEDRIVE_PICTURES_DIR,
+)
 from conjuring.grimoire import print_warning, run_command, run_stdout
 
 SHOULD_PREFIX = True
 
 AUDIO_EXTENSIONS = {"mp3", "m4a", "wav", "aiff", "flac", "ogg", "wma"}
 
 
@@ -17,43 +28,43 @@
     help={
         "dir": "Directory to clean up. Default: current dir",
         "fd": "Use https://github.com/sharkdp/fd instead of 'find'",
         "force": "Delete the actual files (dotfiles are always deleted). Default: False",
     },
     iterable=["dir_"],
 )
-def rm_empty_dirs(c, dir_, force=False, fd=True):
+def rm_empty_dirs(c: Context, dir_: list[str | Path], force: bool = False, fd: bool = True) -> None:
     """Remove some hidden files first, then remove empty dirs.
 
     The ending slash is needed to search OneDrive, now that its behaviour changed in macOS Monterey.
     """
     if not dir_:
         dir_ = [Path.cwd()]
 
     dirs = list({str(Path(d).expanduser().absolute()) for d in dir_})
     xargs = "xargs -0 -n 1 rm -v"
-    for hidden_file in [DOT_DS_STORE, DOT_NO_MEDIA]:
+    for hidden_file in [DOT_DS_STORE, DOT_NOMEDIA]:
         if fd:
             c.run(f"fd -uu -0 -tf -i {hidden_file} {'/ '.join(dirs)}/ | {xargs}")
         else:
             for one_dir in dirs:
                 c.run(f"find {one_dir}/ -type f -iname {hidden_file} -print0 | {xargs}")
 
     f_option = " ".join([f"-f {d}/" for d in dirs[:-1]])
     delete_flag = "-delete" if force else ""
     run_command(c, "find", f_option, f"{dirs[-1]}/ -mindepth 1 -type d -empty -print", delete_flag)
     if not force:
         print_warning("[DRY RUN] Run with --force to actually delete the files")
 
 
 @task
-def cleanup(c, browse=False):
+def cleanup(c: Context, browse: bool = False) -> None:
     """Cleanup pictures."""
     c.run(f"fd -H -0 -tf -i {DOT_DS_STORE} | xargs -0 rm -v")
-    c.run(f"fd -H -0 -tf -i {DOT_NO_MEDIA} | xargs -0 rm -v")
+    c.run(f"fd -H -0 -tf -i {DOT_NOMEDIA} | xargs -0 rm -v")
     c.run("find . -mindepth 1 -type d -empty -print -delete")
 
     # Unhide Picasa originals dir
     for line in c.run("fd -H -t d .picasaoriginals", pty=False).stdout.splitlines():
         original_dir = Path(line)
         c.run(f"mv {original_dir} {original_dir.parent}/Picasa_Originals")
 
@@ -61,66 +72,71 @@
     for line in c.run("fd -t d originals", pty=False).stdout.splitlines():
         original_dir = Path(line)
         c.run(f"mv {original_dir} {original_dir.parent}_Temp")
         c.run(f"mv {original_dir.parent} {original_dir.parent}_Copy")
         c.run(f"mv {original_dir.parent}_Temp {original_dir.parent}")
 
     # Merge the copy dir with the main one
-    for line in run_command(c, "fd -a -uu -t d --color never _copy", str(PICTURES_DIR)).stdout.splitlines():
+    for line in run_command(c, "fd -a -uu -t d --color never _copy", str(ONEDRIVE_PICTURES_DIR)).stdout.splitlines():
         copy_dir = Path(line)
         original_dir = Path(line.replace("_Copy", ""))
         if original_dir.exists():
             if browse:
                 c.run(f"open '{original_dir}'")
             c.run(f"merge-dirs '{original_dir}' '{copy_dir}'")
         else:
             c.run(f"mv '{copy_dir}' '{original_dir}'")
 
     # List dirs with _Copy files
     copy_dirs = set()
-    for line in run_command(c, "fd -H -t f --color never _copy", str(PICTURES_DIR), hide=True).stdout.splitlines():
+    for line in run_command(
+        c,
+        "fd -H -t f --color never _copy",
+        str(ONEDRIVE_PICTURES_DIR),
+        hide=True,
+    ).stdout.splitlines():
         copy_dirs.add(Path(line).parent)
 
     for dir_ in sorted(copy_dirs):
-        print(dir_)
+        typer.echo(dir_)
 
 
 @task(
     help={
         "organize": "Call 'organize run' before categorizing",
         "browse": "Open dir on Finder",
         "empty": "Check dirs that are not empty but should be",
     },
 )
-def categorize(c, organize=True, browse=True, empty=True):
+def categorize(c: Context, organize: bool = True, browse: bool = True, empty: bool = True) -> None:
     """Open directories with files/photos that have to be categorized/moved/renamed."""
     if organize:
         c.run("invoke organize")
 
     empty_dirs = (
         [
             Path(str(d)).expanduser()
             for d in [
                 DOWNLOADS_DIR,
                 DESKTOP_DIR,
                 "~/Documents/Shared_Downloads",
-                PICTURES_DIR / "Telegram",
-                PICTURES_DIR / "Samsung_Gallery/Pictures/Telegram",
-                ONE_DRIVE_DIR / "Documents/Mayan_Staging/Portugues",
-                ONE_DRIVE_DIR / "Documents/Mayan_Staging/English",
-                ONE_DRIVE_DIR / "Documents/Mayan_Staging/Deutsch",
+                ONEDRIVE_PICTURES_DIR / "Telegram",
+                ONEDRIVE_PICTURES_DIR / "Samsung_Gallery/Pictures/Telegram",
+                ONEDRIVE_DIR / "Documents/Mayan_Staging/Portugues",
+                ONEDRIVE_DIR / "Documents/Mayan_Staging/English",
+                ONEDRIVE_DIR / "Documents/Mayan_Staging/Deutsch",
             ]
         ]
         if empty
         else []
     )
 
-    current_year = date.today().year
+    current_year = datetime.now(tz=timezone.utc).date().year
     picture_dirs = [
-        Path(PICTURES_DIR) / f"Camera_New/{sub}" for sub in chain([current_year], range(2008, current_year))
+        Path(ONEDRIVE_PICTURES_DIR) / f"Camera_New/{sub}" for sub in chain([current_year], range(2008, current_year))
     ]
 
     for path in chain(empty_dirs, picture_dirs):  # type: Path
         if not path.exists():
             continue
         has_files = False
         for file in path.glob("*"):
@@ -136,20 +152,20 @@
                 "fd . -t f --color never",
                 str(path),
                 "| sort -ru",
                 "| head -1",
             )
             run_command(c, f"open -R {last_file!r}")
             break
-        else:
-            print(str(path))
+
+        typer.echo(str(path))
 
 
 @task
-def youtube_dl(c, url, min_height=240, download_archive_path=""):
+def youtube_dl(c: Context, url: str, min_height: int = 240, download_archive_path: str = "") -> None:
     """Download video URLs, try different low-res formats until it finds one."""
     download_archive_path = download_archive_path or os.environ.get("YOUTUBE_DL_DOWNLOAD_ARCHIVE_PATH", "")
     archive_option = f"--download-archive {download_archive_path!r}" if download_archive_path else ""
 
     all_heights = [h for h in [240, 360, 480, 0] if h >= min_height or h == 0]
     for height in all_heights:
         # https://github.com/ytdl-org/youtube-dl#format-selection-examples
@@ -168,22 +184,22 @@
             warn=True,
         )
         if result.ok or "Unsupported URL:" in result.stdout:
             break
 
 
 @task
-def slideshow(c, start_at=""):
+def slideshow(c: Context, start_at: str = "") -> None:
     """Show pictures in the current dir with feh."""
     start_at_option = f"--start-at {start_at}" if start_at else ""
     run_command(c, "feh -r -. -g 1790x1070 -B black --caption-path .", start_at_option)
 
 
 @task(help={"dir_": "Directory with audios to transcribe"})
-def whisper(c, dir_):
+def whisper(c: Context, dir_: str | Path) -> None:
     """Transcribe multiple audio file that haven't been transcribed yet, using whisper."""
     dir_ = Path(dir_).expanduser()
     audios: list[Path] = []
     for extension in AUDIO_EXTENSIONS:
         audios.extend(dir_.glob(f"*.{extension}"))
     for file in audios:
         transcript_file = file.with_suffix(".txt")
```

### Comparing `conjuring-0.5.0/src/conjuring/spells/mr.py` & `conjuring-0.6.0/src/conjuring/spells/mr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-"""Tasks to interact with https://myrepos.branchable.com/."""
+"""Spells to interact with myrepos repository management tool https://myrepos.branchable.com/."""
 from dataclasses import dataclass
 from itertools import chain
 from pathlib import Path
 from typing import Optional
 
+import typer
 from invoke import Context, task
 
 from conjuring.grimoire import run_stdout, run_with_fzf
 
 MRCONFIG_FILE = ".mrconfig"
 
 SHOULD_PREFIX = True
 
 
 @dataclass
 class MyRepos:
+    """Find and interact with myrepos config files."""
+
     context: Context
 
-    def find_configs(self, partial_name: str, echo=False) -> list[Path]:
+    def find_configs(self, partial_name: str, echo: bool = False) -> list[Path]:
         """Find config files in the current dir or dirs above."""
         lower_partial_name = partial_name.lower()
         glob_pattern = MRCONFIG_FILE if not lower_partial_name else f"{MRCONFIG_FILE}*{lower_partial_name}*"
         config_dir = self._find_dir_with_mrconfigs(glob_pattern)
         if not config_dir:
             msg = f"No {MRCONFIG_FILE}* file was found in {Path.cwd()} or its parents"
             raise FileNotFoundError(msg)
@@ -38,29 +41,29 @@
                 multi=True,
                 echo=echo,
                 hide=not echo,
             )
         return sorted({config_dir / c for c in chosen})
 
     @staticmethod
-    def _find_dir_with_mrconfigs(glob_pattern) -> Optional[Path]:
+    def _find_dir_with_mrconfigs(glob_pattern: str) -> Optional[Path]:
         for dir_ in chain([Path.cwd()], Path.cwd().parents):
             for _ in dir_.glob(glob_pattern):
                 # Exit loop on the first file found; fzf will handle the rest
                 return dir_
         return None
 
 
 @task(
     help={
         "config": f"Specific config file to use. Use fzf if multiple are found. Default: {MRCONFIG_FILE}",
         "echo": "Echo the commands being executed, for debugging purposes. Default: False",
     },
 )
-def grep(c, search_text, config="", echo=False):
+def grep(c: Context, search_text: str, config: str = "", echo: bool = False) -> None:
     """Grep mr repositories with a search text and print the directories in which the text was found.
 
     Needs mr to be preconfigured with files starting with the ".mrconfig" prefix.
     """
     for chosen in MyRepos(c).find_configs(config, echo=echo):
         # For some reason, using run_command() prints a "\r" char at the end of each line;
         # the solution is to get output as a string and use print().
@@ -69,8 +72,8 @@
             "mr -c",
             str(chosen),
             "-m grep",
             search_text,
             "| rg --color=never 'mr grep: (.+)$' --replace '$1'",
             echo=echo,
         )
-        print(output_without_linefeed)
+        typer.echo(output_without_linefeed)
```

### Comparing `conjuring-0.5.0/src/conjuring/spells/onedrive.py` & `conjuring-0.6.0/src/conjuring/spells/onedrive.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,30 @@
+"""OneDrive: list files with conflicts, ..."""
+from __future__ import annotations
+
 from pathlib import Path
 
-from invoke import task
+import typer
+from invoke import Context, task
 
 from conjuring.grimoire import run_lines, run_stdout
 
 SHOULD_PREFIX = True
 
 
 @task(
     help={"dir": "Directory; can be used multiple times. Default: current dir"},
     iterable=["dir_"],
 )
-def conflicts(c, dir_):
-    """Display files with conflicts."""
+def conflicts(c: Context, dir_: list[str | Path]) -> None:
+    """List files with conflicts."""
     if not dir_:
         dir_ = [Path.cwd()]
 
     hostname = run_stdout(c, "hostname -s").strip()
     suffix = f"-{hostname}"
     for one_dir in list({str(Path(d).expanduser().absolute()) for d in dir_}):
         for line in run_lines(c, f"fd -t f {hostname} {one_dir} | sort"):
             duplicated = Path(line)
             original_name = duplicated.stem[: -len(suffix)]
             original = duplicated.with_stem(original_name)
-            print(run_stdout(c, f"diff {duplicated} {original}", warn=True).strip())
+            typer.echo(run_stdout(c, f"diff {duplicated} {original}", warn=True).strip())
```

### Comparing `conjuring-0.5.0/src/conjuring/spells/paperless.py` & `conjuring-0.6.0/src/conjuring/spells/paperless.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,89 +1,108 @@
-"""Wrapper tasks for papaerless commands https://github.com/paperless-ngx/paperless-ngx."""
+"""Paperless: maintenance, renamer, sanity check, delete failed duplicates https://github.com/paperless-ngx/paperless-ngx."""
 from __future__ import annotations
 
 import re
 import shutil
 from collections import defaultdict
-from collections.abc import Sequence
 from dataclasses import dataclass, field
+from http import HTTPStatus
 from pathlib import Path
+from typing import TYPE_CHECKING
 
 import requests
-from invoke import task
+import typer
+from invoke import Context, task
 
 from conjuring.constants import DOT_DS_STORE, DOWNLOADS_DIR
 from conjuring.grimoire import lazy_env_variable, print_error, print_success, print_warning, run_lines
 
+if TYPE_CHECKING:
+    from collections.abc import Sequence
+
+COUNT_PARTS = 4
+
+STARTING_YEAR = 1900
+
+COUNT_PAIR = 2
+
 SHOULD_PREFIX = True
 
 USR_SRC_DOCUMENTS = "/usr/src/paperless/media/documents/"
 ORPHAN_ARCHIVE = "archive"
 ORPHAN_ORIGINALS = "originals"
 ORPHAN_THUMBNAILS = "thumbnails"
 DOWNLOAD_DESTINATION_DIR = DOWNLOADS_DIR / __name__.rsplit(".")[-1]
 DUPLICATE_OF = " It is a duplicate of "
 REGEX_TITLE_WITH_ID = re.compile(r"(?P<name>.*) ?\(#(?P<id>\d+)\)")
 
 
 def paperless_cmd() -> str:
+    """Command to run Paperless with Docker."""
     yaml_file = lazy_env_variable("PAPERLESS_COMPOSE_YAML", "path to the Paperless Docker compose YAML file")
     return f"docker compose -f {yaml_file} exec webserver"
 
 
 def paperless_documents_dir() -> Path:
+    """Directory where Paperless stores documents."""
     documents_dir = lazy_env_variable("PAPERLESS_MEDIA_DOCUMENTS_DIR", "directory where Paperless stores documents")
     return Path(documents_dir).expanduser()
 
 
 def paperless_url() -> str:
+    """URL where Paperless is running."""
     return lazy_env_variable("PAPERLESS_URL", "URL where Paperless is running")
 
 
 def paperless_token() -> str:
+    """Auth token to access Paperless API."""
     return lazy_env_variable("PAPERLESS_TOKEN", "auth token to access Paperless API")
 
 
 @task
-def maintenance(c, reindex=True, optimize=True, thumbnails=True):
+def maintenance(c: Context, reindex: bool = True, optimize: bool = True, thumbnails: bool = True) -> None:
     """Reindex all docs and optionally optimize them.
 
     https://docs.paperless-ngx.com/administration/#index
     https://docs.paperless-ngx.com/administration/#thumbnails
     """
     if reindex:
         c.run(f"{paperless_cmd()} document_index reindex")
     if optimize:
         c.run(f"{paperless_cmd()} document_index optimize")
     if thumbnails:
         c.run(f"{paperless_cmd()} document_thumbnails")
 
 
 @task
-def rename(c):
+def rename(c: Context) -> None:
     """Rename files.
 
     https://docs.paperless-ngx.com/administration/#renamer
     """
     c.run(f"{paperless_cmd()} document_renamer")
 
 
 @dataclass
 class Document:
+    """A paperless document."""
+
     document_id: int
     title: str
     errors: list = field(default_factory=list, init=False)
 
 
 @dataclass
 class OrphanFile:
+    """A paperless orphan file."""
+
     source: Path
     destination: Path
 
-    def __lt__(self, other: OrphanFile):
+    def __lt__(self, other: OrphanFile) -> bool:
         return self.source < other.source
 
 
 @task(
     help={
         "hide": "Hide progress bar of sanity command",
         "orphans": "Show orphan files",
@@ -91,25 +110,25 @@
         "documents": "Show documents with issues",
         "unknown": "Show unknown lines from the log",
         "together": f"Keep {ORPHAN_ORIGINALS} and {ORPHAN_ARCHIVE} in the same output directory",
         "fix": "Fix broken files by copying them to the downloads dir",
         "move": "Move files instead of copying",
     },
 )
-def sanity(
-    c,
-    hide=True,
-    orphans=False,
-    thumbnails=False,
-    documents=False,
-    unknown=True,
-    together=False,
-    fix=False,
-    move=False,
-):
+def sanity(  # noqa: PLR0913
+    c: Context,
+    hide: bool = True,
+    orphans: bool = False,
+    thumbnails: bool = False,
+    documents: bool = False,
+    unknown: bool = True,
+    together: bool = False,
+    fix: bool = False,
+    move: bool = False,
+) -> None:
     """Sanity checker. Optionally fix orphan files (copies or movies them to the download dir).
 
     https://docs.paperless-ngx.com/administration/#sanity-checker
     """
     # Fail fast if the env var is not set
     documents_dir = paperless_documents_dir() if fix else None
     if documents_dir and not documents_dir.exists():
@@ -161,15 +180,21 @@
     _handle_items(False, move, orphans, "Orphan files", orphan_files)
     # TODO: feat(paperless): move thumbnail files to downloads dir
     _handle_items(fix, move, thumbnails, "Thumbnail files", thumbnail_files)
     _handle_items(False, move, documents, "Documents with issues", documents_with_issues)
     _handle_items(False, move, unknown, "Unknown lines", unknown_lines)
 
 
-def _process_orphans(partial_path, documents_dir, original_or_archive_files, orphan_files, thumbnail_files):
+def _process_orphans(
+    partial_path: Path,
+    documents_dir: Path | None,
+    original_or_archive_files: dict[str, list[OrphanFile]],
+    orphan_files: list[str],
+    thumbnail_files: list[str],
+) -> None:
     if partial_path.name == DOT_DS_STORE:
         return
 
     first_part = partial_path.parts[0]
     if first_part == ORPHAN_THUMBNAILS:
         thumbnail_files.append(str(partial_path))
         return
@@ -181,28 +206,33 @@
     orphan_files.append(str(partial_path))
 
 
 def _split_original_archive(
     original_or_archive_files: dict[str, list[OrphanFile]],
     partial_path: Path,
     documents_dir: Path | None = None,
-):
+) -> None:
     file_key = str(Path("/".join(partial_path.parts[1:])).with_suffix(""))
     expanded_parts = []
     for part in partial_path.parts[:-1]:
         if "," in part:
             expanded_parts.extend(sorted(part.split(",")))
         else:
             expanded_parts.append(part)
 
     # Skip directories with a year when the file name starts with it
     filtered_parts = [
         part
         for part in expanded_parts
-        if not (part.isnumeric() and len(part) == 4 and int(part) > 1900 and partial_path.stem.startswith(part))
+        if not (
+            part.isnumeric()
+            and len(part) == COUNT_PARTS
+            and int(part) > STARTING_YEAR
+            and partial_path.stem.startswith(part)
+        )
     ]
 
     file_name = partial_path.parts[-1]
     filtered_parts.append(file_name)
 
     orphan_dir = documents_dir or Path()
     orphan = OrphanFile(source=orphan_dir / partial_path, destination=Path("/".join(filtered_parts)))
@@ -210,17 +240,17 @@
 
 
 def _split_matched_unmatched(
     original_or_archive_files: dict[str, list[OrphanFile]],
     matched_files: list[OrphanFile],
     unmatched_files: list[OrphanFile],
     together: bool,
-):
+) -> None:
     for single_or_pair in original_or_archive_files.values():
-        if len(single_or_pair) == 2:
+        if len(single_or_pair) == COUNT_PAIR:
             originals_first = sorted(single_or_pair, reverse=True)
             if together:
                 for orphan_file in originals_first:
                     match_path = orphan_file.destination
                     file_without_first_part = Path("/".join(match_path.parts[1:]))
                     if str(match_path).startswith(ORPHAN_ARCHIVE):
                         # Append ORPHAN_ARCHIVE to the file stem
@@ -238,32 +268,32 @@
 
 def _handle_items(
     fix: bool,
     move: bool,
     show_details: bool,
     title: str,
     collection: Sequence[str | OrphanFile | Document],
-):
+) -> None:
     length = len(collection)
     which_function = print_error if length else print_success
     which_function(f"{title} (count: {length})")
     if not show_details:
         return
 
     # https://docs.python.org/3/library/shutil.html#shutil.copy2
     msg = "Moving" if move else "Copying"
 
     dest_dir = DOWNLOAD_DESTINATION_DIR / title
     for item in collection:
         if not isinstance(item, OrphanFile):
-            print(str(item))
+            typer.echo(str(item))
             continue
 
         if not fix:
-            print(str(item.source))
+            typer.echo(str(item.source))
             continue
 
         if not item.source.exists():
             print_error(f"Not found: {item.source}")
             continue
 
         dest_file = dest_dir / item.destination
@@ -273,15 +303,15 @@
         if move:
             shutil.move(item.source, dest_file)
         else:
             shutil.copy2(item.source, dest_file)
 
 
 @task
-def delete_failed_duplicates(c, max_delete=100):
+def delete_failed_duplicates(c: Context, max_delete: int = 100) -> None:
     """Delete records marked as duplicate but that cannot be downloaded. So the PDF files can be reimported."""
     session = requests.Session()
     session.headers.update({"authorization": f"token {paperless_token()}"})
 
     delete_count = 0
     req_tasks = session.get(f"{paperless_url()}/api/tasks/?format=json")
     for obj in req_tasks.json():
@@ -305,25 +335,25 @@
         data = match.groupdict()
         document_id = data["id"]
 
         api_document_url = f"{paperless_url()}/api/documents/{document_id}/"
         document_url = f"{paperless_url()}/documents/{document_id}"
         url = f"{api_document_url}download/"
         req_download = session.head(url)
-        if req_download.status_code != 404:
+        if req_download.status_code != HTTPStatus.NOT_FOUND:
             print_success(document_url, f"Document exists {req_download.status_code=}", clean_line)
             continue
 
         req_document = session.head(api_document_url)
-        if req_document.status_code == 404:
+        if req_document.status_code == HTTPStatus.NOT_FOUND:
             print_warning(document_url, "Document already deleted before", clean_line)
             continue
 
         req_delete = session.delete(api_document_url)
-        if req_delete.status_code == 204:
+        if req_delete.status_code == HTTPStatus.NO_CONTENT:
             print_success(document_url, f"Document deleted #{delete_count}", clean_line)
             delete_count += 1
             if delete_count >= max_delete:
                 raise SystemExit
             continue
 
         print_error(document_url, clean_line, f"Something wrong: {req_delete.status_code=}")
```

### Comparing `conjuring-0.5.0/src/conjuring/spells/pre_commit.py` & `conjuring-0.6.0/src/conjuring/spells/pre_commit.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,59 @@
+"""pre-commit: install, uninstall, run/autoupdate selected hooks."""
 from typing import Optional
 
-from invoke import task
+from invoke import Context, task
 
 from conjuring.grimoire import run_command, run_stdout, run_with_fzf
 from conjuring.visibility import ShouldDisplayTasks, has_pre_commit_config_yaml
 
 SHOULD_PREFIX = True
 should_display_tasks: ShouldDisplayTasks = has_pre_commit_config_yaml
 
 
-def _run_garbage_collector(c):
+def _run_garbage_collector(c: Context) -> None:
     c.run("pre-commit gc")
 
 
-def get_hook_types(commit_msg: bool, desired_hooks: Optional[list[str]] = None):
+def get_hook_types(commit_msg: bool, desired_hooks: Optional[list[str]] = None) -> str:
     """Prepare a list of hook types to install/uninstall."""
     hooks = ["pre-commit"]
     if desired_hooks:
         hooks.extend(desired_hooks)
     if commit_msg:
         hooks.append("commit-msg")
         hooks.append("prepare-commit-msg")
     return " ".join([f"--hook-type {h}" for h in hooks])
 
 
 @task(help={"gc": "Run the garbage collector to remove unused venvs", "commit_msg": "Install commit message hooks"})
-def install(c, gc=False, commit_msg=True):
+def install(c: Context, gc: bool = False, commit_msg: bool = True) -> None:
     """Pre-commit install hooks."""
     if gc:
         _run_garbage_collector(c)
     c.run(f"pre-commit install {get_hook_types(commit_msg)} --install-hooks")
 
 
 @task(help={"gc": "Run the garbage collector to remove unused venvs", "commit_msg": "Uninstall commit message hooks"})
-def uninstall(c, gc=False, commit_msg=True):
+def uninstall(c: Context, gc: bool = False, commit_msg: bool = True) -> None:
     """Pre-commit uninstall ALL hooks."""
     if gc:
         _run_garbage_collector(c)
 
     installed_hooks = [hook for hook in run_stdout(c, "ls .git/hooks", dry=False).splitlines() if ".sample" not in hook]
     c.run(f"pre-commit uninstall {get_hook_types(commit_msg, installed_hooks)}")
 
 
 @task(
     help={
         "hooks": "Comma-separated list of partial hook IDs (fzf will be used to match them)."
         " Use 'all', '.' or '-' to run all hooks.",
     },
 )
-def run(c, hooks):
+def run(c: Context, hooks: str) -> None:
     """Pre-commit run all hooks or a specific one. Don't stop on failures. Needs fzf and yq."""
     split_hooks = hooks.split(",")
     chosen_hooks = []
     for special in ("all", ".", "-"):
         if special in split_hooks:
             chosen_hooks.append("")
             break
@@ -63,14 +64,14 @@
             )
 
     for chosen_hook in chosen_hooks:
         run_command(c, "pre-commit run --all-files", chosen_hook, warn=True)
 
 
 @task()
-def auto(c, repo="", bleed=False):
+def auto(c: Context, repo: str = "", bleed: bool = False) -> None:
     """Autoupdate a Git hook or all hooks with the latest tag. Needs fzf and yq."""
     command = ""
     if repo:
         chosen = run_with_fzf(c, "yq e '.repos[].repo' .pre-commit-config.yaml", query=repo, dry=False)
         command = f"--repo {chosen}"
     run_command(c, "pre-commit autoupdate", "--bleeding-edge" if bleed else "", command)
```

### Comparing `conjuring-0.5.0/src/conjuring/spells/py.py` & `conjuring-0.6.0/src/conjuring/spells/py.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,76 +1,83 @@
+"""Python and Poetry: install venvs, run tests and coverage, install debug tools, generate Ruff config."""
 import re
 from collections import defaultdict
 from pathlib import Path
 from textwrap import dedent
 from typing import Optional
 
-from invoke import Context, task
+import typer
+from invoke import Context, Result, task
 
+from conjuring.constants import PYPROJECT_TOML
 from conjuring.grimoire import print_error, run_command, run_lines, run_with_fzf
 from conjuring.visibility import MagicTask, ShouldDisplayTasks, is_poetry_project
 
 SHOULD_PREFIX = True
 should_display_tasks: ShouldDisplayTasks = is_poetry_project
 
-PYPROJECT_TOML = "pyproject.toml"
 REGEX_RUFF_LINE = re.compile(r"^(?P<filename>.*?):\d+:\d+: (?P<code>.*?)(?P<message> .*)$")
 REGEX_RUFF_MESSAGE = re.compile(r"`[^`]+`")
 
 
 class PyEnv:
+    """pyenv-related tasks."""
+
     def __init__(self, context: Context) -> None:
         self.context = context
 
     def has_local(self) -> bool:
         """Check if a local Python version is set."""
         output = self.context.run("pyenv local", warn=True).stdout.strip()
         return output and "no local version" not in output
 
-    def set_local(self, python_version: str):
+    def set_local(self, python_version: str) -> Result:
         """Set the local pyenv version."""
         latest = self.list_versions(python_version)[-1]
-        self.context.run(f"pyenv local {latest}")
+        return self.context.run(f"pyenv local {latest}")
 
-    def list_versions(self, python_version: Optional[str] = None):
+    def list_versions(self, python_version: Optional[str] = None) -> list[str]:
         """List all installed Python versions, or only the ones matching the desired version."""
         all_versions = run_lines(self.context, "pyenv versions --bare")
         if not python_version:
             return all_versions
 
-        selected_versions = [version for version in all_versions if version.startswith(python_version)]
-        return selected_versions
+        return [version for version in all_versions if version.startswith(python_version)]
 
 
 class Poetry:
+    """Poetry-related tasks."""
+
     def __init__(self, context: Context) -> None:
         self.context = context
 
-    def used_in_project(self, display_error=True) -> bool:
+    def used_in_project(self, display_error: bool = True) -> bool:
         """Check if Poetry is being used."""
         used = int(
             run_command(
                 self.context,
                 f"grep tool.poetry {PYPROJECT_TOML} 2>/dev/null | wc -c",
                 hide=True,
                 warn=True,
             ).stdout.strip(),
         )
         if not used and display_error:
             print_error("This task only works with Poetry projects (so far).")
         return bool(used)
 
-    def parse_python_version(self, venv: str):
+    @staticmethod
+    def parse_python_version(venv: str) -> str:
         """For now, assuming we only have Poetry venvs."""
         return venv.split(" ")[0].split("-py")[1]
 
-    def remove_venv(self, python_version: str):
-        self.context.run(f"poetry env remove python{python_version}")
+    def remove_venv(self, python_version: str) -> Result:
+        """Remove a Poetry venv."""
+        return self.context.run(f"poetry env remove python{python_version}")
 
-    def guess_python_version(self):
+    def guess_python_version(self) -> str:
         """Guess Python version from pyproject.toml."""
         # TODO: rewrite this hack and use a TOML package to read the values directly
         pyproject_lines = run_lines(
             self.context,
             f"rg --no-line-number -e '^python ' -e python_version {PYPROJECT_TOML}",
         )
         versions: set[str] = set()
@@ -80,20 +87,21 @@
             clean_version = value_only.replace("^", "").replace("~", "").strip('" ')
             versions.add(clean_version)
         if len(versions) > 1:
             print_error(f"Multiple Python versions found in {PYPROJECT_TOML}: {versions=}")
             raise SystemExit
         return list(versions)[0]
 
-    def use_venv(self, python_version: str):
-        self.context.run(f"poetry env use python{python_version}")
+    def use_venv(self, python_version: str) -> Result:
+        """Use a Poetry venv."""
+        return self.context.run(f"poetry env use python{python_version}")
 
 
 @task(help={"inject": "Pipx repo to inject this project into"})
-def editable(c, inject=""):
+def editable(c: Context, inject: str = "") -> None:
     """Hack to install a Poetry package as editable until Poetry supports PEP660 hooks.
 
     It won't be needed anymore when https://github.com/python-poetry/poetry-core/pull/182 is merged.
     """
     if not Poetry(c).used_in_project():
         return
 
@@ -116,15 +124,15 @@
     c.run(f"mv {PYPROJECT_TOML} _{PYPROJECT_TOML}")
     run_command(c, "pipx inject -e", chosen_repo, ".")
     c.run(f"mv _{PYPROJECT_TOML} {PYPROJECT_TOML}")
     c.run("rm setup.py")
 
 
 @task(help={"version": "Python version", "force": "Recreate the environment", "delete_all": "Delete all environments"})
-def install(c, version="", force=False, delete_all=False):
+def install(c: Context, version: str = "", force: bool = False, delete_all: bool = False) -> None:
     """Install a Python virtual environment. For now, only works with Poetry."""
     venv_list = run_lines(c, "poetry env list", hide=False)
     poetry = Poetry(c)
     if not poetry.used_in_project():
         return
 
     if delete_all:
@@ -141,25 +149,25 @@
         poetry.remove_venv(version)
     poetry.use_venv(version)
 
     c.run("poetry lock --check && poetry install")
 
 
 @task(help={"watch": "Watch for changes and re-run affected tests. Install pytest-watch and pytest-testmon first."})
-def test(c, watch=False):
+def test(c: Context, watch: bool = False) -> None:
     """Run tests with pytest."""
     if not Poetry(c).used_in_project():
         return
 
     command = 'ptw --runner "pytest --testmon"' if watch else "pytest -v"
     run_command(c, "poetry run", command)
 
 
 @task(help={"show_all": "Show all lines, even if they are covered"})
-def coverage(c, show_all=False):
+def coverage(c: Context, show_all: bool = False) -> None:
     """Run tests with pytest and coverage."""
     if not Poetry(c).used_in_project():
         return
 
     options = [f"--cov={source}" for source in ["src", Path.cwd().name, "app"] if Path(source).exists()]
 
     skip_option = "" if show_all else ":skip-covered"
@@ -174,15 +182,23 @@
         "ipython": "Install https://pypi.org/project/ipython/",
         "ipdb": "Install https://pypi.org/project/ipdb/",
         "pudb": "Install https://pypi.org/project/pudb/",
         "icecream": "Install https://pypi.org/project/icecream/",
         "devtools": "Install https://pypi.org/project/devtools/",
     },
 )
-def debug_tools(c, all_=False, ipython=False, ipdb=False, pudb=False, icecream=False, devtools=False):
+def debug_tools(  # noqa: PLR0913
+    c: Context,
+    all_: bool = False,
+    ipython: bool = False,
+    ipdb: bool = False,
+    pudb: bool = False,
+    icecream: bool = False,
+    devtools: bool = False,
+) -> None:
     """Install debug tools."""
     if not Poetry(c).used_in_project():
         return
 
     tools = [
         "pip",
         "ipython" if ipython or all_ else "",
@@ -191,63 +207,63 @@
         "icecream" if icecream or all_ else "",
         "devtools[pygments]" if devtools or all_ else "",
     ]
     run_command(c, "poetry run pip install --upgrade", *tools)
 
 
 @task(klass=MagicTask)
-def ruff_config(c):
+def ruff_config(c: Context) -> None:
     """Generate ruff configuration from existing warnings."""
     # TODO: feat: check if the global ruff is installed and use it if it is
     ignore: dict[str, set[str]] = defaultdict(set)
     per_file_ignores: dict[str, set[str]] = defaultdict(set)
     for line in run_lines(c, "pre-commit run --all-files ruff", warn=True):
         if line.startswith("warning:"):
-            print(line)
+            typer.echo(line)
             continue
 
         match = REGEX_RUFF_LINE.match(line)
         if not match:
             continue
 
         filename = match.group("filename")
         code = match.group("code")
         message = match.group("message")
         clean_message = REGEX_RUFF_MESSAGE.sub("?", message)
 
         ignore[code].add(clean_message.strip())
         per_file_ignores[filename].add(code)
 
-    def _print_ruff_codes(ignore_section: bool):
+    def _print_ruff_codes(ignore_section: bool) -> None:
         for _code, messages in sorted(ignore.items()):
             joined_messages = ",".join(sorted(messages))
             if ignore_section:
-                print(f'    "{_code}", # {joined_messages}', end="")
+                typer.echo(f'    "{_code}", # {joined_messages}', nl=False)
             else:
-                print(f"# {_code} {joined_messages}", end="")
-            print(f" https://beta.ruff.rs/docs/rules/?q={_code}")
+                typer.echo(f"# {_code} {joined_messages}", nl=False)
+            typer.echo(f" https://beta.ruff.rs/docs/rules/?q={_code}")
 
     # TODO: edit pyproject.toml existing config for both sections,
     #  skipping existing lines and adding new codes at the bottom
     if ignore:
         header = """
             # https://beta.ruff.rs/docs/settings/#ignore
             ignore = [
                 # Ignores to keep
                 # TODO: Ignores to fix
         """
-        print(dedent(header).strip())
+        typer.echo(dedent(header).strip())
         _print_ruff_codes(True)
-        print("]\n")
+        typer.echo("]\n")
 
     if per_file_ignores:
         header = """
             # https://beta.ruff.rs/docs/settings/#per-file-ignores
             [tool.ruff.per-file-ignores]
             # Ignores to keep
             # TODO: Ignores to fix
         """
-        print(dedent(header).strip())
+        typer.echo(dedent(header).strip())
         _print_ruff_codes(False)
         for file, codes in sorted(per_file_ignores.items()):
             sorted_codes = '", "'.join(sorted(codes))
-            print(f'"{file}" = ["{sorted_codes}"]')
+            typer.echo(f'"{file}" = ["{sorted_codes}"]')
```

### Comparing `conjuring-0.5.0/src/conjuring/spells/shell.py` & `conjuring-0.6.0/src/conjuring/spells/shell.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """Shell tasks."""
-from invoke import task
+from invoke import Context, task
 
 SHOULD_PREFIX = True
 
 COMPAT_DIR = "$BASH_COMPLETION_COMPAT_DIR/"
 USER_DIR = "$BASH_COMPLETION_USER_DIR/completions/"
 COMPLETION_DIRS = (COMPAT_DIR, USER_DIR)
 
 
 @task
-def completion_list(c):
+def completion_list(c: Context) -> None:
     """List existing shell completions."""
     for var in COMPLETION_DIRS:
         c.run(f"exa -l {var}")
 
 
 @task
-def completion_install(c, app):
+def completion_install(c: Context, app: str) -> None:
     """Install shell completion. For now, only for the Bash shell, and only for Click projects.
 
     See:
     - https://click.palletsprojects.com/en/8.0.x/shell-completion/
     - https://github.com/click-contrib/click-completion
     """
     completion_file = f"{COMPAT_DIR}{app}.bash-completion"
     c.run(f"_{app.upper()}_COMPLETE=bash_source {app} > {completion_file}")
     c.run(f"exa -l {completion_file}")
     c.run(f"bat {completion_file}")
 
 
 @task
-def completion_uninstall(c, app):
+def completion_uninstall(c: Context, app: str) -> None:
     """Uninstall shell completion from both completion dirs."""
     for completion_dir in COMPLETION_DIRS:
         with c.cd(completion_dir):
             c.run(f"rm -v {app}*", warn=True)
     completion_list(c)
```

### Comparing `conjuring-0.5.0/src/conjuring/visibility.py` & `conjuring-0.6.0/src/conjuring/visibility.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,74 @@
-import re
+"""Visibility predicates and a custom Invoke task that can be hidden."""
+from collections.abc import Iterable
 from pathlib import Path
-from typing import Callable
+from typing import Any, Callable, Optional, Union
 
 from invoke import Task
 
-POETRY_LINE = re.compile(r"\[tool\..*poetry\]")
+from conjuring.constants import PRE_COMMIT_CONFIG_YAML, PYPROJECT_TOML
+
+TOOL_POETRY_SECTION = "[tool.poetry]"
 ShouldDisplayTasks = Callable[[], bool]
 
 
-def always_visible():
+def always_visible() -> bool:
+    """Predicate that always returns True."""
     return True
 
 
 def has_pre_commit_config_yaml() -> bool:
-    return Path(".pre-commit-config.yaml").exists()
+    """Return True if the current dir has a .pre-commit-config.yaml file."""
+    return Path(PRE_COMMIT_CONFIG_YAML).exists()
 
 
 def is_home_dir() -> bool:
+    """Return True if the current dir is the user's home dir."""
     return Path.cwd() == Path.home()
 
 
 def is_git_repo() -> bool:
     """Only display tasks if the current dir is a Git repo."""
     return Path(".git").exists()
 
 
 def is_poetry_project() -> bool:
-    fpath = Path("pyproject.toml")
-    return fpath.exists() and _has_poetry_line(fpath)
-
-
-def _has_poetry_line(fpath: Path) -> bool:
-    return any(re.search(POETRY_LINE, line) for line in fpath.open(encoding="utf-8"))
+    """Return True if the current dir is a Poetry project."""
+    pyproject_toml = Path(PYPROJECT_TOML)
+    return pyproject_toml.exists() and TOOL_POETRY_SECTION in pyproject_toml.read_text(encoding="utf-8")
 
 
 def display_task(task: Task, module_flag: bool) -> bool:  # TODO: refactor: rename to should_display_task
+    """Return True if the task should be displayed."""
     if isinstance(task, MagicTask):
         # This is our custom task, let's check its visibility before the module
         return task.should_display()
 
     # This is a regular Invoke Task; let's check if the module should be visible or not
     return module_flag
 
 
 class MagicTask(Task):
-    def __init__(
+    """An Invoke task that can be hidden."""
+
+    def __init__(  # noqa: PLR0913
         self,
-        body,
-        name=None,
-        aliases=(),
-        positional=None,
-        optional=(),
-        default=False,
-        auto_shortflags=True,
-        help=None,
-        pre=None,
-        post=None,
-        autoprint=False,
-        iterable=None,
-        incrementable=None,
+        body: Callable,
+        name: Optional[str] = None,
+        aliases: Iterable[str] = (),
+        positional: Optional[Iterable[str]] = None,
+        optional: Iterable[str] = (),
+        default: bool = False,
+        auto_shortflags: bool = True,
+        help: Optional[dict[str, Any]] = None,  # noqa: A002
+        pre: Optional[Union[list[str], str]] = None,
+        post: Optional[Union[list[str], str]] = None,
+        autoprint: bool = False,
+        iterable: Optional[Iterable[str]] = None,
+        incrementable: Optional[Iterable[str]] = None,
         should_display: ShouldDisplayTasks = always_visible,
     ) -> None:
         self.should_display: ShouldDisplayTasks = should_display
         super().__init__(
             body,
             name,
             aliases,
```

### Comparing `conjuring-0.5.0/PKG-INFO` & `conjuring-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conjuring
-Version: 0.5.0
+Version: 0.6.0
 Summary: 🐍🤖 Reusable global Invoke tasks that can be merged with local project tasks
 Home-page: https://github.com/andreoliwa/conjuring
 License: MIT
 Keywords: invoke,tasks,automation,cli,python
 Author: W. Augusto Andreoli
 Author-email: andreoliwa@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -18,18 +18,24 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Requires-Dist: invoke
 Requires-Dist: requests
+Requires-Dist: typer
 Project-URL: Documentation, https://andreoliwa.github.io/conjuring/
 Project-URL: Repository, https://github.com/andreoliwa/conjuring
 Description-Content-Type: text/markdown
 
+<!-- markdownlint-disable-file MD031 -->
+
+[//]: # "It breaks numbered lists on Mkdocs"
+[//]: # "MD031/blanks-around-fences Fenced code blocks should be surrounded by blank lines"
+
 # Conjuring
 
 Reusable global [Invoke](https://github.com/pyinvoke/invoke) tasks that can be
 merged with local project tasks.
 
 ## Features
 
@@ -49,26 +55,20 @@
 
 Each module under [the `conjuring/spells` directory](https://github.com/andreoliwa/conjuring/tree/master/src/conjuring/spells)
 is a collection of Invoke tasks.
 
 ## Quick setup
 
 1. Install Conjuring in an isolated virtualenv with [pipx](https://github.com/pypa/pipx):
-
    ```shell
    pipx install --include-deps conjuring
    ```
-
    The `--include-deps` flag is needed to install Invoke's apps (`invoke` and `inv`).
-
 2. Create a `tasks.py` file on your home dir:
-
    ```shell
    echo -e "from conjuring import *\n\nnamespace = cast_all_spells()" > ~/tasks.py
    ```
-
 3. You should see the list of Conjuring tasks from any directory where you type this:
-
    ```shell
    invoke --list
    ```
```

