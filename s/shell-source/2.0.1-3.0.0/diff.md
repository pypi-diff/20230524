# Comparing `tmp/shell_source-2.0.1.tar.gz` & `tmp/shell_source-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_source-2.0.1.tar", max compression
+gzip compressed data, was "shell_source-3.0.0.tar", max compression
```

## Comparing `shell_source-2.0.1.tar` & `shell_source-3.0.0.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-05-22 15:05:45.726556 shell_source-2.0.1/LICENSE
--rw-r--r--   0        0        0     2929 2023-05-22 15:05:45.730556 shell_source-2.0.1/README.md
--rw-r--r--   0        0        0      741 2023-05-22 15:05:45.730556 shell_source-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      513 2023-05-22 15:05:45.730556 shell_source-2.0.1/shell_source/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 15:05:45.730556 shell_source-2.0.1/shell_source/py.typed
--rw-r--r--   0        0        0     1129 2023-05-22 15:05:45.730556 shell_source-2.0.1/shell_source/shell_config.py
--rw-r--r--   0        0        0     4372 2023-05-22 15:05:45.730556 shell_source-2.0.1/shell_source/source.py
--rw-r--r--   0        0        0     3919 1970-01-01 00:00:00.000000 shell_source-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-24 17:12:11.545665 shell_source-3.0.0/LICENSE
+-rw-r--r--   0        0        0     2967 2023-05-24 17:12:11.545665 shell_source-3.0.0/README.md
+-rw-r--r--   0        0        0      741 2023-05-24 17:12:11.545665 shell_source-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      498 2023-05-24 17:12:11.545665 shell_source-3.0.0/shell_source/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 17:12:11.545665 shell_source-3.0.0/shell_source/py.typed
+-rw-r--r--   0        0        0      562 2023-05-24 17:12:11.545665 shell_source-3.0.0/shell_source/scripters/__init__.py
+-rw-r--r--   0        0        0     1147 2023-05-24 17:12:11.545665 shell_source-3.0.0/shell_source/scripters/csh_scripter.py
+-rw-r--r--   0        0        0      256 2023-05-24 17:12:11.545665 shell_source-3.0.0/shell_source/scripters/fish_scripter.py
+-rw-r--r--   0        0        0     4645 2023-05-24 17:12:11.545665 shell_source-3.0.0/shell_source/scripters/scripter.py
+-rw-r--r--   0        0        0     3311 2023-05-24 17:12:11.545665 shell_source-3.0.0/shell_source/source.py
+-rw-r--r--   0        0        0     3957 1970-01-01 00:00:00.000000 shell_source-3.0.0/PKG-INFO
```

### Comparing `shell_source-2.0.1/LICENSE` & `shell_source-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_source-2.0.1/README.md` & `shell_source-3.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -33,30 +33,42 @@
 ```
 
 ### Requesting Specific Variables
 
 If you specify the argument `variables`, then only those variables you passed will be present as keys in the returned dictionary.
 
 ```py
->>> source("path/to/script.sh", "csh", variables=("foo", "bar", "biz"))
+>>> source("path/to/script.sh", "zsh", variables=("foo", "bar", "biz"))
 {"foo": ..., "bar": ..., "biz", ...}
 ```
 
 ### Ignoring Local Variables
 
 If you don't want to obtain any local variables set by the script, but only want the environment variables, you can pass `ignore_locals=True`.
 
+### Passing Arguments to the shell
+
+If you want to pass arguments to the shell, for example `-x` or `-e`, you can pass it directly in the `shell` argument.
+
+```py
+>>> source("path/to/script.sh", "bash -x")
+```
+
+### Passing Arguments to the script
+
+If you want to pass arguments to the script being sourced, you can pass them in the `args` argument.
+
+```py
+>>> source("path/to/script.sh", "bash", args=("foo", "bar"))
+```
+
 ### Supporting Different Shells
 
-This module has been tested to work with `bash`, `zsh`, `tcsh`, and `ksh`. You can use any other shell that's somewhat posix compliant and supports the keyword "source", but it it doesn't work, you may use the `ShellConfig` class to indicate to `source` how to interact with your shell.
+This module has been tested to work with `bash`, `zsh`, and `ksh` out of the box. You can use any other shell that's somewhat posix compliant, but it it doesn't work, you may have to create a class derived from the `Scripter` class to indicate to `source` how to interact with the shell you want to use.
 
-The class `ShellConfig` contains several string templates which are used to run the necessary commands with the shell. If the shell you want to use doesn't support any of the commands set by default in that class, you can pass an instance of `ShellConfig` to `source` to override the default templates.
+Some specialized implementations of `Scripter` are provided in `shell_source.scripters` for shells that are not posix compliant, such as `csh`, `tcsh` and `fish`.
 
-For example, `csh` and `fish` are not supported by default, (specifically because they don't have the variable `$?` to get the exit status of the last command,) but we can source a script for one of these shells anyways by passing a `ShellConfig` instance which will declare how to get the exit code of the previous command.
+For example, to use `tcsh` to source a script, you can use the `CshScripter` class like so:
 
 ```py
-source(
-	"path/to/script.csh",
-	"csh",
-	shell_config=ShellConfig(prev_exit_code="$status")
-)
+>>> source("path/to/script.csh", "tcsh", scripter=CshScripter())
 ```
```

### Comparing `shell_source-2.0.1/pyproject.toml` & `shell_source-3.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shell-source"
-version = "2.0.1"
+version = "3.0.0"
 description = "A python module for sourcing variables from shell scripts"
 authors = ["Abraham Murciano <abrahammurciano@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/abrahammurciano/python-shell-source"
 documentation = "https://abrahammurciano.github.io/python-shell-source/shell_source/"
 keywords = ["shell", "source", "environment"]
```

### Comparing `shell_source-2.0.1/shell_source/source.py` & `shell_source-3.0.0/shell_source/source.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 import logging
 import re
 import shlex
 import subprocess
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import Collection, Dict, Iterable, Mapping, Optional, Sequence, Union
+from typing import Collection, Dict, Iterable, Sequence, Union
 
-from .shell_config import ShellConfig
+from .scripters import Scripter
 
 logger = logging.getLogger(__name__)
 
 
 def source(
     script: Union[str, Path],
     shell: str = "sh",
     *,
+    args: Iterable[str] = (),
     variables: Collection[str] = (),
     ignore_locals: bool = False,
-    shell_config: ShellConfig = ShellConfig(),
+    scripter: Scripter = Scripter(),
     **subprocess_kwargs,
 ) -> Dict[str, str]:
     """Run a shell script and return its variables as a dictionary.
 
     > NOTE: If the script defines variables with newlines in their values it is undefined behaviour, though it will not raise an exception.
 
     Args:
         script: The shell script to source. It may contain arguments, file redirections, etc so long as it is supported by the shell you give.
         shell: The shell to use. If the shell you give is in the path it's name suffices, otherwise give the path to it. You may also pass flags, such as -x or -e. Default is "sh".
+        args: Any extra arguments to pass to the sourced script. Default is no arguments.
         variables: The names of the variables set in the script to return. By default, all variables are returned.
         ignore_locals: If True, no local variables set by the script are returned. Default is False.
-        shell_config: An instance of ShellConfig that specifies how to interact with the given shell. If your shell is (somewhat) posix-compliant the default should work.
+        scripter: An instance of Scripter that knows how to interact with the given shell. If your shell is (somewhat) posix-compliant the default should work. `csh` and `tcsh` must use `CshScripter`.
         subprocess_kwargs: Any other keyword arguments are passed to subprocess.run. By default, check=True is passed. Also, args, input and text are not allowed.
     """
-    check = subprocess_kwargs.pop("check", True)
+    subprocess_kwargs.setdefault("check", True)
     disallowed_kwargs = {"args", "input", "text"}
     if disallowed_kwargs & subprocess_kwargs.keys():
         raise TypeError(
             f"Illegal arguments to source(): {', '.join(disallowed_kwargs & subprocess_kwargs.keys())}"
         )
     with TemporaryDirectory() as tmpdir:
         vars_file = Path(tmpdir) / "vars"
-        stdin = _get_cmds(
-            script=script,
-            vars_file=vars_file,
-            check=check,
+        stdin = scripter.script(
+            script,
+            vars_file,
+            args=args,
             variables=variables,
             ignore_locals=ignore_locals,
-            shell_config=shell_config,
         )
         subprocess.run(
             shlex.split(shell),
             input=stdin,
             text=True,
-            check=check,
             **subprocess_kwargs,
         )
         return _parse_vars(vars_file.read_text())
 
 
 _SPLIT_PATTERN = re.compile(r"[\t= ]")
 
@@ -80,41 +80,7 @@
             try:
                 result[-1] += line
             except IndexError:
                 logger.warning(
                     f"Expected a line matching '.*[\t=].*' but instead found '{line}'. Ignoring this line."
                 )
     return result
-
-
-def _get_cmds(
-    *,
-    script: Union[str, Path],
-    vars_file: Path,
-    check: bool,
-    variables: Collection[str],
-    ignore_locals: bool,
-    shell_config: ShellConfig,
-) -> str:
-    """Get a string to be sent to the stdin of the shell."""
-    source_cmd = shell_config.source_cmd.format(script=script)
-    exit_or_true = (
-        shell_config.exit_cmd.format(code=shell_config.prev_exit_code)
-        if check
-        else "true"
-    )
-    full_source_cmd = shell_config.boolean_or.format(cmd1=source_cmd, cmd2=exit_or_true)
-    get_vars_cmds = (
-        shell_config.redirect_stdout.format(cmd=cmd, file=vars_file)
-        for cmd in _get_vars_cmds(variables, ignore_locals, shell_config)
-    )
-    return " ;\n".join((full_source_cmd, *get_vars_cmds))
-
-
-def _get_vars_cmds(
-    variables: Collection[str], ignore_locals: bool, shell_config: ShellConfig
-) -> Iterable[str]:
-    if variables:
-        return (
-            f"echo {var}={shell_config.get_var.format(var=var)}" for var in variables
-        )
-    return [*(() if ignore_locals else (shell_config.get_all_locals,)), "env"]
```

### Comparing `shell_source-2.0.1/PKG-INFO` & `shell_source-3.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-source
-Version: 2.0.1
+Version: 3.0.0
 Summary: A python module for sourcing variables from shell scripts
 Home-page: https://github.com/abrahammurciano/python-shell-source
 License: MIT
 Keywords: shell,source,environment
 Author: Abraham Murciano
 Author-email: abrahammurciano@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -56,31 +56,43 @@
 ```
 
 ### Requesting Specific Variables
 
 If you specify the argument `variables`, then only those variables you passed will be present as keys in the returned dictionary.
 
 ```py
->>> source("path/to/script.sh", "csh", variables=("foo", "bar", "biz"))
+>>> source("path/to/script.sh", "zsh", variables=("foo", "bar", "biz"))
 {"foo": ..., "bar": ..., "biz", ...}
 ```
 
 ### Ignoring Local Variables
 
 If you don't want to obtain any local variables set by the script, but only want the environment variables, you can pass `ignore_locals=True`.
 
+### Passing Arguments to the shell
+
+If you want to pass arguments to the shell, for example `-x` or `-e`, you can pass it directly in the `shell` argument.
+
+```py
+>>> source("path/to/script.sh", "bash -x")
+```
+
+### Passing Arguments to the script
+
+If you want to pass arguments to the script being sourced, you can pass them in the `args` argument.
+
+```py
+>>> source("path/to/script.sh", "bash", args=("foo", "bar"))
+```
+
 ### Supporting Different Shells
 
-This module has been tested to work with `bash`, `zsh`, `tcsh`, and `ksh`. You can use any other shell that's somewhat posix compliant and supports the keyword "source", but it it doesn't work, you may use the `ShellConfig` class to indicate to `source` how to interact with your shell.
+This module has been tested to work with `bash`, `zsh`, and `ksh` out of the box. You can use any other shell that's somewhat posix compliant, but it it doesn't work, you may have to create a class derived from the `Scripter` class to indicate to `source` how to interact with the shell you want to use.
 
-The class `ShellConfig` contains several string templates which are used to run the necessary commands with the shell. If the shell you want to use doesn't support any of the commands set by default in that class, you can pass an instance of `ShellConfig` to `source` to override the default templates.
+Some specialized implementations of `Scripter` are provided in `shell_source.scripters` for shells that are not posix compliant, such as `csh`, `tcsh` and `fish`.
 
-For example, `csh` and `fish` are not supported by default, (specifically because they don't have the variable `$?` to get the exit status of the last command,) but we can source a script for one of these shells anyways by passing a `ShellConfig` instance which will declare how to get the exit code of the previous command.
+For example, to use `tcsh` to source a script, you can use the `CshScripter` class like so:
 
 ```py
-source(
-	"path/to/script.csh",
-	"csh",
-	shell_config=ShellConfig(prev_exit_code="$status")
-)
+>>> source("path/to/script.csh", "tcsh", scripter=CshScripter())
 ```
```

