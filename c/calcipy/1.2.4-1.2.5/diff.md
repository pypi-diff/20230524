# Comparing `tmp/calcipy-1.2.4.tar.gz` & `tmp/calcipy-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calcipy-1.2.4.tar", max compression
+gzip compressed data, was "calcipy-1.2.5.tar", max compression
```

## Comparing `calcipy-1.2.4.tar` & `calcipy-1.2.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1066 2023-05-13 11:22:49.916008 calcipy-1.2.4/LICENSE
--rw-r--r--   0        0        0      167 2023-05-16 23:29:56.121283 calcipy-1.2.4/calcipy/__init__.py
--rw-r--r--   0        0        0     1241 2023-05-13 10:55:19.213121 calcipy-1.2.4/calcipy/can_skip.py
--rw-r--r--   0        0        0      175 2023-03-02 02:58:57.029784 calcipy-1.2.4/calcipy/check_for_stale_packages/__init__.py
--rw-r--r--   0        0        0     8262 2023-05-13 00:16:53.654649 calcipy-1.2.4/calcipy/check_for_stale_packages/_check_for_stale_packages.py
--rw-r--r--   0        0        0     6422 2023-05-13 10:55:55.582130 calcipy-1.2.4/calcipy/cli.py
--rw-r--r--   0        0        0      154 2023-03-02 02:58:57.946199 calcipy-1.2.4/calcipy/code_tag_collector/__init__.py
--rw-r--r--   0        0        0    10840 2023-05-13 11:22:33.621932 calcipy-1.2.4/calcipy/code_tag_collector/_collector.py
--rw-r--r--   0        0        0      140 2023-03-02 02:58:58.498973 calcipy-1.2.4/calcipy/dot_dict/__init__.py
--rw-r--r--   0        0        0      803 2023-02-25 23:58:05.004832 calcipy-1.2.4/calcipy/dot_dict/_dot_dict.py
--rw-r--r--   0        0        0        0 2023-04-05 02:28:27.975837 calcipy-1.2.4/calcipy/experiments/__init__.py
--rw-r--r--   0        0        0     1988 2023-05-13 11:16:09.447581 calcipy-1.2.4/calcipy/experiments/check_duplicate_test_names.py
--rw-r--r--   0        0        0     3271 2023-02-23 02:19:12.613926 calcipy-1.2.4/calcipy/file_search.py
--rw-r--r--   0        0        0     1814 2023-04-07 21:04:03.754244 calcipy-1.2.4/calcipy/invoke_helpers.py
--rw-r--r--   0        0        0      162 2023-03-02 02:58:58.973806 calcipy-1.2.4/calcipy/md_writer/__init__.py
--rw-r--r--   0        0        0     7833 2023-04-22 15:51:43.990661 calcipy-1.2.4/calcipy/md_writer/_writer.py
--rw-r--r--   0        0        0      162 2023-03-02 02:58:59.584964 calcipy-1.2.4/calcipy/noxfile/__init__.py
--rw-r--r--   0        0        0     6546 2023-04-22 15:10:18.113523 calcipy-1.2.4/calcipy/noxfile/_noxfile.py
--rw-r--r--   0        0        0     1193 2023-04-22 15:05:58.225355 calcipy-1.2.4/calcipy/scripts.py
--rw-r--r--   0        0        0        0 2023-02-21 03:18:10.928974 calcipy-1.2.4/calcipy/tasks/__init__.py
--rw-r--r--   0        0        0     3120 2023-04-08 22:31:05.741542 calcipy-1.2.4/calcipy/tasks/all_tasks.py
--rw-r--r--   0        0        0     1876 2023-04-06 12:55:27.782578 calcipy-1.2.4/calcipy/tasks/cl.py
--rw-r--r--   0        0        0     1132 2023-02-23 02:54:45.453854 calcipy-1.2.4/calcipy/tasks/defaults.py
--rw-r--r--   0        0        0     3609 2023-04-22 14:59:14.141730 calcipy-1.2.4/calcipy/tasks/doc.py
--rw-r--r--   0        0        0     3869 2023-04-07 23:08:02.132045 calcipy-1.2.4/calcipy/tasks/lint.py
--rw-r--r--   0        0        0      454 2023-02-23 02:19:12.617085 calcipy-1.2.4/calcipy/tasks/nox.py
--rw-r--r--   0        0        0     1659 2023-05-16 23:12:39.188499 calcipy-1.2.4/calcipy/tasks/pack.py
--rw-r--r--   0        0        0      557 2023-02-23 02:19:12.617596 calcipy-1.2.4/calcipy/tasks/stale.py
--rw-r--r--   0        0        0     1498 2023-02-23 02:19:12.617900 calcipy-1.2.4/calcipy/tasks/tags.py
--rw-r--r--   0        0        0     3659 2023-04-18 23:50:20.411698 calcipy-1.2.4/calcipy/tasks/test.py
--rw-r--r--   0        0        0      634 2023-02-23 02:19:12.618406 calcipy-1.2.4/calcipy/tasks/types.py
--rw-r--r--   0        0        0     6651 2023-05-16 23:30:13.497030 calcipy-1.2.4/docs/README.md
--rw-r--r--   0        0        0     6547 2023-05-16 23:29:56.158760 calcipy-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     9989 1970-01-01 00:00:00.000000 calcipy-1.2.4/setup.py
--rw-r--r--   0        0        0    11420 1970-01-01 00:00:00.000000 calcipy-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-13 11:22:49.916008 calcipy-1.2.5/LICENSE
+-rw-r--r--   0        0        0      167 2023-05-23 22:23:44.941141 calcipy-1.2.5/calcipy/__init__.py
+-rw-r--r--   0        0        0     1241 2023-05-13 10:55:19.213121 calcipy-1.2.5/calcipy/can_skip.py
+-rw-r--r--   0        0        0      175 2023-03-02 02:58:57.029784 calcipy-1.2.5/calcipy/check_for_stale_packages/__init__.py
+-rw-r--r--   0        0        0     8262 2023-05-13 00:16:53.654649 calcipy-1.2.5/calcipy/check_for_stale_packages/_check_for_stale_packages.py
+-rw-r--r--   0        0        0     6436 2023-05-17 11:02:50.475557 calcipy-1.2.5/calcipy/cli.py
+-rw-r--r--   0        0        0      154 2023-03-02 02:58:57.946199 calcipy-1.2.5/calcipy/code_tag_collector/__init__.py
+-rw-r--r--   0        0        0    10840 2023-05-13 11:22:33.621932 calcipy-1.2.5/calcipy/code_tag_collector/_collector.py
+-rw-r--r--   0        0        0      140 2023-03-02 02:58:58.498973 calcipy-1.2.5/calcipy/dot_dict/__init__.py
+-rw-r--r--   0        0        0      803 2023-02-25 23:58:05.004832 calcipy-1.2.5/calcipy/dot_dict/_dot_dict.py
+-rw-r--r--   0        0        0        0 2023-04-05 02:28:27.975837 calcipy-1.2.5/calcipy/experiments/__init__.py
+-rw-r--r--   0        0        0     1988 2023-05-13 11:16:09.447581 calcipy-1.2.5/calcipy/experiments/check_duplicate_test_names.py
+-rw-r--r--   0        0        0     3271 2023-02-23 02:19:12.613926 calcipy-1.2.5/calcipy/file_search.py
+-rw-r--r--   0        0        0     1942 2023-05-17 11:00:03.480459 calcipy-1.2.5/calcipy/invoke_helpers.py
+-rw-r--r--   0        0        0      162 2023-03-02 02:58:58.973806 calcipy-1.2.5/calcipy/md_writer/__init__.py
+-rw-r--r--   0        0        0     7833 2023-04-22 15:51:43.990661 calcipy-1.2.5/calcipy/md_writer/_writer.py
+-rw-r--r--   0        0        0      162 2023-03-02 02:58:59.584964 calcipy-1.2.5/calcipy/noxfile/__init__.py
+-rw-r--r--   0        0        0     6546 2023-04-22 15:10:18.113523 calcipy-1.2.5/calcipy/noxfile/_noxfile.py
+-rw-r--r--   0        0        0     1258 2023-05-17 10:59:02.930491 calcipy-1.2.5/calcipy/scripts.py
+-rw-r--r--   0        0        0        0 2023-02-21 03:18:10.928974 calcipy-1.2.5/calcipy/tasks/__init__.py
+-rw-r--r--   0        0        0     3488 2023-05-17 11:01:15.749443 calcipy-1.2.5/calcipy/tasks/all_tasks.py
+-rw-r--r--   0        0        0     1884 2023-05-16 23:59:46.273109 calcipy-1.2.5/calcipy/tasks/cl.py
+-rw-r--r--   0        0        0     1169 2023-05-17 10:45:25.212981 calcipy-1.2.5/calcipy/tasks/defaults.py
+-rw-r--r--   0        0        0     3617 2023-05-16 23:59:46.277097 calcipy-1.2.5/calcipy/tasks/doc.py
+-rw-r--r--   0        0        0     3893 2023-05-17 00:35:52.385145 calcipy-1.2.5/calcipy/tasks/lint.py
+-rw-r--r--   0        0        0      462 2023-05-16 23:59:46.283536 calcipy-1.2.5/calcipy/tasks/nox.py
+-rw-r--r--   0        0        0     1667 2023-05-17 10:56:42.232544 calcipy-1.2.5/calcipy/tasks/pack.py
+-rw-r--r--   0        0        0      565 2023-05-16 23:59:46.291723 calcipy-1.2.5/calcipy/tasks/stale.py
+-rw-r--r--   0        0        0     1506 2023-05-16 23:59:46.294332 calcipy-1.2.5/calcipy/tasks/tags.py
+-rw-r--r--   0        0        0     3667 2023-05-16 23:59:46.301475 calcipy-1.2.5/calcipy/tasks/test.py
+-rw-r--r--   0        0        0      642 2023-05-16 23:59:46.303934 calcipy-1.2.5/calcipy/tasks/types.py
+-rw-r--r--   0        0        0     6651 2023-05-23 22:23:51.404030 calcipy-1.2.5/docs/README.md
+-rw-r--r--   0        0        0     6547 2023-05-23 22:23:44.978905 calcipy-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0     9989 1970-01-01 00:00:00.000000 calcipy-1.2.5/setup.py
+-rw-r--r--   0        0        0    11420 1970-01-01 00:00:00.000000 calcipy-1.2.5/PKG-INFO
```

### Comparing `calcipy-1.2.4/LICENSE` & `calcipy-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.4/calcipy/can_skip.py` & `calcipy-1.2.5/calcipy/can_skip.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.4/calcipy/check_for_stale_packages/_check_for_stale_packages.py` & `calcipy-1.2.5/calcipy/check_for_stale_packages/_check_for_stale_packages.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.4/calcipy/cli.py` & `calcipy-1.2.5/calcipy/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 from functools import wraps
 from pathlib import Path
 from types import ModuleType
 
 from beartype import beartype
 from beartype.typing import Any, Callable, Dict, List, Optional
 from corallium.log import configure_logger, logger
-from invoke import Collection, Config, Context, Program, Task
-from invoke import task as invoke_task  # noqa: TID251
-from invoke.config import merge_dicts
+from invoke.collection import Collection
+from invoke.config import Config, merge_dicts
+from invoke.context import Context
+from invoke.program import Program
+from invoke.tasks import task as invoke_task  # noqa: TID251
 from pydantic import BaseModel, Field, PositiveInt
 
 from .invoke_helpers import use_pty
 
 
 class GlobalTaskOptions(BaseModel):
     """Global Task Options."""
@@ -30,15 +32,15 @@
     verbose: PositiveInt = Field(default=0, lte=3)
     """Verbosity level."""
 
     keep_going: bool = False
     """Continue task execution regardless of failure."""
 
 
-class _CalcipyProgram(Program):  # type: ignore[misc]
+class _CalcipyProgram(Program):
     """Customized version of Invoke's `Program`."""
 
     def print_help(self) -> None:  # pragma: no cover
         """Extend print_help with calcipy-specific global configuration.
 
         https://github.com/pyinvoke/invoke/blob/0bcee75e4a26ad33b13831719c00340ca12af2f0/invoke/program.py#L657-L667
 
@@ -51,29 +53,29 @@
             ('--keep-going', 'Continue running tasks even on failure'),
             ('--working_dir=STRING', 'Set the cwd for the program. Example: "../run --working-dir .. lint test"'),
             ('-v,-vv,-vvv', 'Globally configure logger verbosity (-vvv for most verbose)'),
         ])
         print('')  # noqa: T201
 
 
-class CalcipyConfig(Config):  # type: ignore[misc]
+class CalcipyConfig(Config):
     """Opinionated Config with better defaults."""
 
     @staticmethod
     def global_defaults() -> Dict:  # type: ignore[type-arg]  # pragma: no cover
         """Override the global defaults."""
         invoke_defaults = Config.global_defaults()
         calcipy_defaults = {
             'run': {
                 'echo': True,
                 'echo_format': '\033[2;3;37mRunning: {command}\033[0m',
                 'pty': use_pty(),
             },
         }
-        return merge_dicts(invoke_defaults, calcipy_defaults)  # type: ignore[no-any-return]
+        return merge_dicts(invoke_defaults, calcipy_defaults)
 
 
 @beartype
 def start_program(  # pragma: no cover
     pkg_name: str,
     pkg_version: str,
     module: Optional[ModuleType] = None,
@@ -164,21 +166,22 @@
     except Exception:
         if not ctx.config.gto.keep_going:
             raise
         logger.exception('Task Failed', func=str(func), args=args, kwargs=kwargs)
     return None
 
 
+# TODO: Can I type this function with fewer Any's?
 @beartype
-def task(*task_args: Any, show_task_info: bool = True, **task_kwargs: Any) -> Callable[[Any], Task]:
+def task(*task_args: Any, show_task_info: bool = True, **task_kwargs: Any) -> Callable[[Any], Any]:
     """Wrapper to accept arguments for an invoke task."""
     @beartype
-    def wrapper(func: Any) -> Task:  # noqa: ANN001
+    def wrapper(func: Any) -> Any:  # noqa: ANN001
         """Wraps the decorated task."""
-        @invoke_task(*task_args, **task_kwargs)  # type: ignore[misc]
+        @invoke_task(*task_args, **task_kwargs)
         @beartype
         @wraps(func)
-        def inner(ctx: Context, *args: Any, **kwargs: Any) -> Task:
+        def inner(ctx: Context, *args: Any, **kwargs: Any) -> Any:
             """Wrap the task with settings configured in `gto` for working_dir and logging."""
             return _inner_runner(func=func, ctx=ctx, show_task_info=show_task_info, args=args, kwargs=kwargs)
         return inner
     return wrapper
```

### Comparing `calcipy-1.2.4/calcipy/code_tag_collector/_collector.py` & `calcipy-1.2.5/calcipy/code_tag_collector/_collector.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.4/calcipy/dot_dict/_dot_dict.py` & `calcipy-1.2.5/calcipy/dot_dict/_dot_dict.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.4/calcipy/experiments/check_duplicate_test_names.py` & `calcipy-1.2.5/calcipy/experiments/check_duplicate_test_names.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.4/calcipy/file_search.py` & `calcipy-1.2.5/calcipy/file_search.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.4/calcipy/invoke_helpers.py` & `calcipy-1.2.5/calcipy/invoke_helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from functools import lru_cache
 from os import environ
 from pathlib import Path
 
 from beartype import beartype
 from beartype.typing import Any, Optional
 from corallium.file_helpers import COPIER_ANSWERS, read_yaml_file
-from invoke import Context, Result
+from invoke.context import Context
+from invoke.runners import Result
 
 # ----------------------------------------------------------------------------------------------------------------------
 # General Invoke
 
 
 @lru_cache(maxsize=1)
 @beartype
@@ -28,15 +29,18 @@
 def run(ctx: Context, *run_args: Any, **run_kwargs: Any) -> Result:
     """Wrap invoke.run to run within the `working_dir`."""
     working_dir = '.'
     with suppress(AttributeError):
         working_dir = ctx.config.gto.working_dir
 
     with ctx.cd(working_dir):
-        return ctx.run(*run_args, **run_kwargs)
+        res = ctx.run(*run_args, **run_kwargs)
+    if not res:
+        raise NotImplementedError('No response from `ctx.run`')
+    return res
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 # Invoke Task Helpers
 
 
 @lru_cache(maxsize=1)
```

### Comparing `calcipy-1.2.4/calcipy/md_writer/_writer.py` & `calcipy-1.2.5/calcipy/md_writer/_writer.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.4/calcipy/noxfile/_noxfile.py` & `calcipy-1.2.5/calcipy/noxfile/_noxfile.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.4/calcipy/scripts.py` & `calcipy-1.2.5/calcipy/scripts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Start the command line program."""
 
 from types import ModuleType
 
 from beartype import beartype
 from beartype.typing import List
+from invoke.collection import Collection
 
 from . import __pkg_name__, __version__
 from .cli import start_program
 
 
 @beartype
 def start() -> None:  # pragma: no cover
@@ -19,15 +20,15 @@
 @beartype
 def _start_subset(modules: List[ModuleType]) -> None:  # pragma: no cover
     """Run the specified subset."""
     from .tasks.defaults import new_collection
 
     ns = new_collection()
     for module in modules:
-        ns.add_collection(module)
+        ns.add_collection(Collection.from_module(module))
 
     start_program(__pkg_name__, __version__, collection=ns)
 
 
 @beartype
 def start_lint() -> None:  # pragma: no cover
     """Run CLI with only the lint namespace."""
```

### Comparing `calcipy-1.2.4/calcipy/tasks/cl.py` & `calcipy-1.2.5/calcipy/tasks/cl.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Changelog CLI."""
 
 from beartype import beartype
 from beartype.typing import Literal, Optional
-from invoke import Context
+from invoke.context import Context
 
 from ..cli import task
 from ..invoke_helpers import get_doc_subdir, get_project_path, run
 
 SuffixT = Optional[Literal['alpha', 'beta', 'rc']]
 """Prerelease Suffix Type."""
```

### Comparing `calcipy-1.2.4/calcipy/tasks/defaults.py` & `calcipy-1.2.5/calcipy/tasks/defaults.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Calcipy-Invoke Defaults."""
 
 import json
 from contextlib import suppress
 from pathlib import Path
 
 from beartype import beartype
-from invoke import Collection, Context
+from invoke.collection import Collection
+from invoke.context import Context
 
 DEFAULTS = {
     'tags': {
         'filename': 'CODE_TAG_SUMMARY.md',
     },
     'test': {
         'min_cover': '0',
```

### Comparing `calcipy-1.2.4/calcipy/tasks/doc.py` & `calcipy-1.2.5/calcipy/tasks/doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     delete_dir,
     ensure_dir,
     open_in_browser,
     read_package_name,
     read_yaml_file,
     trim_trailing_whitespace,
 )
-from invoke import Context
+from invoke.context import Context
 from invoke.exceptions import UnexpectedExit
 
 from ..cli import task
 from ..invoke_helpers import get_doc_subdir, get_project_path, run
 from ..md_writer import write_autoformatted_md_sections
```

### Comparing `calcipy-1.2.4/calcipy/tasks/lint.py` & `calcipy-1.2.5/calcipy/tasks/lint.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from contextlib import suppress
 
 from beartype import beartype
 from beartype.typing import Optional
 from corallium.file_helpers import read_package_name
 from corallium.log import logger
-from invoke import Context
+from invoke.context import Context
 
 from ..cli import task
 from ..invoke_helpers import run
 
 # ==============================================================================
 # Ruff
 
@@ -92,15 +92,15 @@
     pkg_name = read_package_name()
     run(ctx, f'poetry run bandit --recursive {pkg_name} -s B101')
 
     # See additional semgrep rules at:
     #   https://semgrep.dev/explore
     #   https://github.com/returntocorp/semgrep-rules/tree/develop/python
     #   https://awesomeopensource.com/project/returntocorp/semgrep-rules?categorypage=45
-    semgrep_configs = ' '.join([
+    semgrep_configs = ' '.join([  # noqa: FLY002
         '--config=p/ci',
         '--config=p/default',
         '--config=p/security-audit',
         '--config=r/bash',
         '--config=r/contrib',
         '--config=r/fingerprints',
         '--config=r/generic',
```

### Comparing `calcipy-1.2.4/calcipy/tasks/pack.py` & `calcipy-1.2.5/calcipy/tasks/pack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Packaging CLI."""
 
 from corallium import file_helpers  # Required for mocking read_pyproject
 from corallium.file_helpers import LOCK, PROJECT_TOML
 from corallium.log import logger
-from invoke import Context
+from invoke.context import Context
 
 from .. import can_skip  # Required for mocking can_skip.can_skip
 from ..cli import task
 from ..invoke_helpers import run
 from ..noxfile._noxfile import BASE_NOX_COMMAND
```

### Comparing `calcipy-1.2.4/calcipy/tasks/stale.py` & `calcipy-1.2.5/calcipy/tasks/stale.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Stale Packages CLI."""
 
-from invoke import Context
+from invoke.context import Context
 
 from ..check_for_stale_packages import check_for_stale_packages as cfsp
 from ..cli import task
 from ..invoke_helpers import run
 
 
 @task(
```

### Comparing `calcipy-1.2.4/calcipy/tasks/tags.py` & `calcipy-1.2.5/calcipy/tasks/tags.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code Tag Collector CLI."""
 
 from pathlib import Path
 
 from beartype.typing import Optional
-from invoke import Context
+from invoke.context import Context
 
 from ..cli import task
 from ..code_tag_collector import write_code_tag_file
 from ..file_search import find_project_files
 from ..invoke_helpers import get_doc_subdir
 from .defaults import from_ctx
```

### Comparing `calcipy-1.2.4/calcipy/tasks/test.py` & `calcipy-1.2.5/calcipy/tasks/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Test CLI."""
 
 from pathlib import Path
 
 from beartype import beartype
 from beartype.typing import Optional
 from corallium.file_helpers import open_in_browser, read_package_name
-from invoke import Context
+from invoke.context import Context
 
 from ..cli import task
 from ..experiments import check_duplicate_test_names
 from ..invoke_helpers import run
 from .defaults import from_ctx
 
 _STEPWISE_ARGS = ' --failed-first --new-first --exitfirst -vv --no-cov'
```

### Comparing `calcipy-1.2.4/calcipy/tasks/types.py` & `calcipy-1.2.5/calcipy/tasks/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Types CLI."""
 
 from beartype import beartype
 from corallium.file_helpers import read_package_name
-from invoke import Context
+from invoke.context import Context
 
 from ..cli import task
 from ..invoke_helpers import run
 
 
 @beartype
 def _inner_task(ctx: Context, *, cli_args: str, command: str) -> None:
```

### Comparing `calcipy-1.2.4/docs/README.md` & `calcipy-1.2.5/docs/README.md`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.4/pyproject.toml` & `calcipy-1.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "1.2.4"
+version = "1.2.5"
 version_files = ["calcipy/__init__.py:^__version", "pyproject.toml:^version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
@@ -26,25 +26,25 @@
 include = ["LICENSE"]
 keywords = ["nox", "python-poetry"]
 license = "MIT"
 maintainers = []
 name = "calcipy"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/calcipy"
-version = "1.2.4"
+version = "1.2.5"
 
 [tool.poetry.dependencies]
 python = "^3.8.12"
 arrow = {optional = true, version = ">=1.2.3"} # tags
 autopep8 = {optional = true, version = ">=2.0.1"} # flake8
 bandit = {optional = true, version = ">=1.7.4"} # lint
 beartype = ">=0.12.0"
 bidict = {optional = true, version = ">=0.22.1"} # stale
 commitizen = {optional = true, version = ">=2.42.0"} # doc
-corallium = ">=0.2.1"
+corallium = ">=0.2.2"
 dlint = {optional = true, version = ">=0.14.0"} # flake8
 flake8 = {optional = true, version = ">=6.0.0"} # flake8
 flake8-adjustable-complexity = {optional = true, version = ">=0.0.6"} # flake8
 flake8-annotations-complexity = {optional = true, version = ">=0.0.7"} # flake8
 flake8-executable = {optional = true, version = ">=2.1.3"} # flake8
 flake8-expression-complexity = {optional = true, version = ">=0.0.11"} # flake8
 flake8-functions = {optional = true, version = ">=0.0.7"} # flake8
@@ -56,15 +56,15 @@
 flake8-sql = {optional = true, version = ">=0.4.1"} # flake8
 flake8-string-format = {optional = true, version = ">=0.3.0"} # flake8
 flake8-super = {optional = true, version = ">=0.1.3"} # flake8
 flake8-tuple = {optional = true, version = ">=0.4.1"} # flake8
 flake8-typing-imports = {optional = true, version = ">=1.14.0"} # flake8
 flake8-use-pathlib = {optional = true, version = ">=0.3.0"} # flake8
 flake8-variables-names = {optional = true, version = ">=0.0.5"} # flake8
-invoke = ">=2.1.0"
+invoke = ">=2.1.2"
 mkdocs = {optional = true, version = ">=1.4.1"} # doc
 mkdocs-build-plantuml-plugin = {optional = true, version = ">=1.7.4"} # doc
 mkdocs-gen-files = {optional = true, version = ">=0.4.0"} # doc
 mkdocs-git-revision-date-localized-plugin = {optional = true, version = ">=1.0.1"} # doc
 mkdocs-include-markdown-plugin = {markers = "python_version < '3.12'", optional = true, version = ">=4.0.3"} # doc
 mkdocs-literate-nav = {optional = true, version = ">=0.5.0"} # doc
 mkdocs-material = {optional = true, version = ">=8.2.16"} # doc
@@ -80,15 +80,15 @@
 pyrate_limiter = {optional = true, version = ">=2.4"} # stale
 pytest = {optional = true, version = ">=7.2.1"} # test
 pytest-cov = {optional = true, version = ">=4.0.0"} # test
 pytest-randomly = {optional = true, version = ">=3.12.0"} # test
 pytest-watcher = {optional = true, version = ">=0.2.6"} # test
 python-box = {optional = true, version = ">=6.0.2"} # ddict
 pyyaml = {optional = true, version = ">=5.2"} # doc,tags
-requests = {optional = true, version = ">=2.28.1"} # stale
+requests = {optional = true, version = ">=2.31.0"} # stale
 ruff = {optional = true, version = ">=0.0.253"} # lint
 semgrep = {optional = true, version = ">=1.12.1"} # lint
 tabulate = {optional = true, version = ">=0.9.0"} # tags: Required for pandas to markdown
 transitions = {optional = true, version = ">=0.9.0"} # tags: docs
 
 [tool.poetry.extras]
 ddict = ["python-box"]
```

### Comparing `calcipy-1.2.4/setup.py` & `calcipy-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
  'calcipy.noxfile',
  'calcipy.tasks']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['beartype>=0.12.0', 'corallium>=0.2.1', 'invoke>=2.1.0', 'pydantic>=1.10.5']
+['beartype>=0.12.0', 'corallium>=0.2.2', 'invoke>=2.1.2', 'pydantic>=1.10.5']
 
 extras_require = \
 {'ddict': ['python-box>=6.0.2'],
  'doc': ['commitizen>=2.42.0',
          'mkdocs>=1.4.1',
          'mkdocs-build-plantuml-plugin>=1.7.4',
          'mkdocs-gen-files>=0.4.0',
@@ -59,15 +59,15 @@
           'ruff>=0.0.253',
           'semgrep>=1.12.1'],
  'nox': ['nox-poetry>=1.0.2'],
  'pylint': ['pylint>=2.16.2'],
  'stale': ['arrow>=1.2.3',
            'bidict>=0.22.1',
            'pyrate_limiter>=2.4',
-           'requests>=2.28.1'],
+           'requests>=2.31.0'],
  'tags': ['arrow>=1.2.3', 'pandas>=1.5.3', 'pyyaml>=5.2', 'tabulate>=0.9.0'],
  'test': ['pytest>=7.2.1',
           'pytest-cov>=4.0.0',
           'pytest-randomly>=3.12.0',
           'pytest-watcher>=0.2.6'],
  'types': ['mypy>=1.0.0']}
 
@@ -75,15 +75,15 @@
 {'console_scripts': ['calcipy = calcipy.scripts:start',
                      'calcipy_lint = calcipy.scripts:start_lint',
                      'calcipy_tags = calcipy.scripts:start_tags',
                      'calcipy_types = calcipy.scripts:start_types']}
 
 setup_kwargs = {
     'name': 'calcipy',
-    'version': '1.2.4',
+    'version': '1.2.5',
     'description': 'Python package to simplify development',
     'long_description': '# calcipy\n\n![./calcipy-banner-wide.svg](https://raw.githubusercontent.com/KyleKing/calcipy/main/docs/calcipy-banner-wide.svg)\n\n`calcipy` is a Python package that implements best practices such as code style (linting, auto-fixes), documentation, CI/CD, and logging. Like the calcium carbonate in hard coral, packages can be built on the `calcipy` foundation.\n\n`calcipy` has some configurability, but is tailored for my particular use cases. If you want the same sort of functionality, there are a number of alternatives to consider:\n\n- [pyscaffold](https://github.com/pyscaffold/pyscaffold) is a much more mature project that aims for the same goals, but with a slightly different approach and tech stack (tox vs. nox, cookiecutter vs. copier, etc.)\n- [tidypy](https://github.com/jayclassless/tidypy#features), [pylama](https://github.com/klen/pylama), and [codecheck](https://pypi.org/project/codecheck/) offer similar functionality of bundling and running static checkers, but makes far fewer assumptions\n- [pytoil](https://github.com/FollowTheProcess/pytoil) is a general CLI tool for developer automation\n- And many more such as [pyta](https://github.com/pyta-uoft/pyta), [prospector](https://github.com/PyCQA/prospector), [wemake-python-styleguide](https://github.com/wemake-services/wemake-python-styleguide) / [cjolowicz/cookiecutter-hypermodern-python](https://github.com/cjolowicz/cookiecutter-hypermodern-python), [formate](https://github.com/python-formate/formate), [johnthagen/python-blueprint](https://github.com/johnthagen/python-blueprint), [oxsecurity/megalinter](https://github.com/oxsecurity/megalinter), etc.\n\n## Installation\n\nCalcipy needs a few static files managed using copier and a template project: [kyleking/calcipy_template](https://github.com/KyleKing/calcipy_template/)\n\nYou can quickly use the template to create a new project or add calcipy to an existing one:\n\n```sh\n# Install copier. pipx is recommended\npipx install copier\n\n# To create a new project\ncopier copy gh:KyleKing/calcipy_template new_project\ncd new_project\n\n# Or convert/update an existing one\ncd my_project\ncopier copy gh:KyleKing/calcipy_template .\ncopier update\n```\n\nSee [./Advanced_Configuration.md](./Advanced_Configuration.md) for documentation on the configurable aspects of `calcipy`\n\n### Calcipy CLI\n\nAdditionally, `calcipy` can be run as a CLI application without adding the package as a dependency.\n\nQuick Start:\n\n```sh\npipx install calcipy\n\n# Use \'tags\' to create a CODE_TAG_SUMMARY of the specified directory\ncalcipy tags --help\ncalcipy tags --base-dir=~/path/to/my_project\n\n# See additional documentation from the CLI help\n> calcipy\n\nSubcommands:\n\nmain                                     Main task pipeline.\nother                                    Run tasks that are otherwise not exercised in main.\nrelease                                  Release pipeline.\ncl.bump                                  Bumps project version based on commits & settings in pyproject.toml.\ncl.write                                 Write a Changelog file with the raw Git history.\ndoc.build                                Build documentation with mkdocs.\ndoc.deploy                               Deploy docs to the Github `gh-pages` branch.\ndoc.watch                                Serve local documentation for local editing.\nlint.autopep8                            Run autopep8.\nlint.check (lint)                        Run ruff as check-only.\nlint.fix                                 Run ruff and apply fixes.\nlint.flake8                              Run ruff and apply fixes.\nlint.pre-commit                          Run pre-commit.\nlint.pylint                              Run ruff and apply fixes.\nlint.security                            Attempt to identify possible security vulnerabilities.\nlint.watch                               Run ruff as check-only.\nnox.noxfile (nox)                        Run nox from the local noxfile.\npack.check-licenses                      Check licenses for compatibility with `licensecheck`.\npack.lock                                Ensure poetry.lock is  up-to-date.\npack.publish                             Build the distributed format(s) and publish.\nstale.check-for-stale-packages (stale)   Identify stale dependencies.\ntags.collect-code-tags (tags)            Create a `CODE_TAG_SUMMARY.md` with a table for TODO- and FIXME-style code comments.\ntest.coverage                            Generate useful coverage outputs after running pytest.\ntest.pytest (test)                       Run pytest with default arguments.\ntest.step                                Run pytest optimized to stop on first error.\ntest.watch                               Run pytest with polling and optimized to stop on first error.\ntypes.mypy                               Run mypy.\ntypes.pyright                            Run pyright.\n\nGlobal Task Options:\n\nworking_dir   Set the cwd for the program. Example: "../run --working-dir .. lint test"\n*file_args    List of Paths available globally to all tasks. Will resolve paths with working_dir\nverbose       Globally configure logger verbosity (-vvv for most verbose)\n```\n\n### Calcipy Pre-Commit\n\n`calcipy` can also be used as a `pre-commit` task by adding the below snippet to your `pre-commit` file:\n\n```yaml\nrepos:\n  - repo: https://github.com/KyleKing/calcipy\n    rev: main\n    hooks:\n      - id: tags\n      - id: lint-fix\n      - id: types\n```\n\n## Project Status\n\nSee the `Open Issues` and/or the [CODE_TAG_SUMMARY]. For release history, see the [CHANGELOG].\n\n## Contributing\n\nWe welcome pull requests! For your pull request to be accepted smoothly, we suggest that you first open a GitHub issue to discuss your idea. For resources on getting started with the code base, see the below documentation:\n\n- [DEVELOPER_GUIDE]\n- [STYLE_GUIDE]\n\n## Code of Conduct\n\nWe follow the [Contributor Covenant Code of Conduct][contributor-covenant].\n\n### Open Source Status\n\nWe try to reasonably meet most aspects of the "OpenSSF scorecard" from [Open Source Insights](https://deps.dev/pypi/calcipy)\n\n## Responsible Disclosure\n\nIf you have any security issue to report, please contact the project maintainers privately. You can reach us at [dev.act.kyle@gmail.com](mailto:dev.act.kyle@gmail.com).\n\n## License\n\n[LICENSE]\n\n[changelog]: https://calcipy.kyleking.me/docs/CHANGELOG\n[code_tag_summary]: https://calcipy.kyleking.me/docs/CODE_TAG_SUMMARY\n[contributor-covenant]: https://www.contributor-covenant.org\n[developer_guide]: https://calcipy.kyleking.me/docs/DEVELOPER_GUIDE\n[license]: https://github.com/kyleking/calcipy/blob/main/LICENSE\n[style_guide]: https://calcipy.kyleking.me/docs/STYLE_GUIDE\n',
     'author': 'Kyle King',
     'author_email': 'dev.act.kyle@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyleking/calcipy',
```

### Comparing `calcipy-1.2.4/PKG-INFO` & `calcipy-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcipy
-Version: 1.2.4
+Version: 1.2.5
 Summary: Python package to simplify development
 Home-page: https://github.com/kyleking/calcipy
 License: MIT
 Keywords: nox,python-poetry
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
 Requires-Python: >=3.8.12,<4.0.0
@@ -35,15 +35,15 @@
 Provides-Extra: types
 Requires-Dist: arrow (>=1.2.3) ; extra == "stale" or extra == "tags"
 Requires-Dist: autopep8 (>=2.0.1) ; extra == "lint"
 Requires-Dist: bandit (>=1.7.4) ; extra == "lint"
 Requires-Dist: beartype (>=0.12.0)
 Requires-Dist: bidict (>=0.22.1) ; extra == "stale"
 Requires-Dist: commitizen (>=2.42.0) ; extra == "doc"
-Requires-Dist: corallium (>=0.2.1)
+Requires-Dist: corallium (>=0.2.2)
 Requires-Dist: dlint (>=0.14.0) ; extra == "flake8"
 Requires-Dist: flake8 (>=6.0.0) ; extra == "flake8"
 Requires-Dist: flake8-adjustable-complexity (>=0.0.6) ; extra == "flake8"
 Requires-Dist: flake8-annotations-complexity (>=0.0.7) ; extra == "flake8"
 Requires-Dist: flake8-executable (>=2.1.3) ; extra == "flake8"
 Requires-Dist: flake8-expression-complexity (>=0.0.11) ; extra == "flake8"
 Requires-Dist: flake8-functions (>=0.0.7) ; extra == "flake8"
@@ -55,15 +55,15 @@
 Requires-Dist: flake8-sql (>=0.4.1) ; extra == "flake8"
 Requires-Dist: flake8-string-format (>=0.3.0) ; extra == "flake8"
 Requires-Dist: flake8-super (>=0.1.3) ; extra == "flake8"
 Requires-Dist: flake8-tuple (>=0.4.1) ; extra == "flake8"
 Requires-Dist: flake8-typing-imports (>=1.14.0) ; extra == "flake8"
 Requires-Dist: flake8-use-pathlib (>=0.3.0) ; extra == "flake8"
 Requires-Dist: flake8-variables-names (>=0.0.5) ; extra == "flake8"
-Requires-Dist: invoke (>=2.1.0)
+Requires-Dist: invoke (>=2.1.2)
 Requires-Dist: mkdocs (>=1.4.1) ; extra == "doc"
 Requires-Dist: mkdocs-build-plantuml-plugin (>=1.7.4) ; extra == "doc"
 Requires-Dist: mkdocs-gen-files (>=0.4.0) ; extra == "doc"
 Requires-Dist: mkdocs-git-revision-date-localized-plugin (>=1.0.1) ; extra == "doc"
 Requires-Dist: mkdocs-include-markdown-plugin (>=4.0.3) ; (python_version < "3.12") and (extra == "doc")
 Requires-Dist: mkdocs-literate-nav (>=0.5.0) ; extra == "doc"
 Requires-Dist: mkdocs-material (>=8.2.16) ; extra == "doc"
@@ -79,15 +79,15 @@
 Requires-Dist: pyrate_limiter (>=2.4) ; extra == "stale"
 Requires-Dist: pytest (>=7.2.1) ; extra == "test"
 Requires-Dist: pytest-cov (>=4.0.0) ; extra == "test"
 Requires-Dist: pytest-randomly (>=3.12.0) ; extra == "test"
 Requires-Dist: pytest-watcher (>=0.2.6) ; extra == "test"
 Requires-Dist: python-box (>=6.0.2) ; extra == "ddict"
 Requires-Dist: pyyaml (>=5.2) ; extra == "doc" or extra == "tags"
-Requires-Dist: requests (>=2.28.1) ; extra == "stale"
+Requires-Dist: requests (>=2.31.0) ; extra == "stale"
 Requires-Dist: ruff (>=0.0.253) ; extra == "lint"
 Requires-Dist: semgrep (>=1.12.1) ; extra == "lint"
 Requires-Dist: tabulate (>=0.9.0) ; extra == "tags"
 Requires-Dist: transitions (>=0.9.0) ; extra == "doc"
 Project-URL: Bug Tracker, https://github.com/kyleking/calcipy/issues
 Project-URL: Changelog, https://github.com/kyleking/calcipy/blob/main/docs/docs/CHANGELOG.md
 Project-URL: Documentation, https://calcipy.kyleking.me
```

