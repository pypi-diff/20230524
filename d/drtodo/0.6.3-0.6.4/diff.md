# Comparing `tmp/drtodo-0.6.3.tar.gz` & `tmp/drtodo-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drtodo-0.6.3.tar", max compression
+gzip compressed data, was "drtodo-0.6.4.tar", max compression
```

## Comparing `drtodo-0.6.3.tar` & `drtodo-0.6.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1064 2023-05-23 02:51:22.787598 drtodo-0.6.3/LICENSE
--rw-r--r--   0        0        0     9777 2023-05-23 02:51:22.787598 drtodo-0.6.3/drtodo/README.md
--rw-r--r--   0        0        0      224 2023-05-23 02:51:22.791598 drtodo-0.6.3/drtodo/__init__.py
--rw-r--r--   0        0        0       44 2023-05-23 02:51:22.791598 drtodo-0.6.3/drtodo/__main__.py
--rw-r--r--   0        0        0    11844 2023-05-23 02:51:22.791598 drtodo-0.6.3/drtodo/main.py
--rw-r--r--   0        0        0     4703 2023-05-23 02:51:22.791598 drtodo-0.6.3/drtodo/man_command.py
--rw-r--r--   0        0        0     4784 2023-05-23 02:51:22.791598 drtodo-0.6.3/drtodo/mdparser.py
--rw-r--r--   0        0        0     1406 2023-05-23 02:51:22.791598 drtodo-0.6.3/drtodo/mistuneplugin.py
--rw-r--r--   0        0        0      618 2023-05-23 02:51:22.791598 drtodo-0.6.3/drtodo/rich_display.py
--rw-r--r--   0        0        0     7052 2023-05-23 02:51:22.791598 drtodo-0.6.3/drtodo/settings.py
--rw-r--r--   0        0        0       11 2023-05-23 02:51:22.791598 drtodo-0.6.3/drtodo/util.py
--rw-r--r--   0        0        0      807 2023-05-23 02:51:34.295809 drtodo-0.6.3/pyproject.toml
--rw-r--r--   0        0        0    10671 1970-01-01 00:00:00.000000 drtodo-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-24 00:54:19.171030 drtodo-0.6.4/LICENSE
+-rw-r--r--   0        0        0     9777 2023-05-24 00:54:19.171030 drtodo-0.6.4/drtodo/README.md
+-rw-r--r--   0        0        0      224 2023-05-24 00:54:19.171030 drtodo-0.6.4/drtodo/__init__.py
+-rw-r--r--   0        0        0       46 2023-05-24 00:54:19.171030 drtodo-0.6.4/drtodo/__main__.py
+-rw-r--r--   0        0        0    15460 2023-05-24 00:54:19.171030 drtodo-0.6.4/drtodo/main.py
+-rw-r--r--   0        0        0     4703 2023-05-24 00:54:19.171030 drtodo-0.6.4/drtodo/man_command.py
+-rw-r--r--   0        0        0     4784 2023-05-24 00:54:19.171030 drtodo-0.6.4/drtodo/mdparser.py
+-rw-r--r--   0        0        0     1406 2023-05-24 00:54:19.171030 drtodo-0.6.4/drtodo/mistuneplugin.py
+-rw-r--r--   0        0        0      618 2023-05-24 00:54:19.171030 drtodo-0.6.4/drtodo/rich_display.py
+-rw-r--r--   0        0        0     7061 2023-05-24 00:54:19.171030 drtodo-0.6.4/drtodo/settings.py
+-rw-r--r--   0        0        0       11 2023-05-24 00:54:19.171030 drtodo-0.6.4/drtodo/util.py
+-rw-r--r--   0        0        0      808 2023-05-24 00:54:33.283104 drtodo-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0    10671 1970-01-01 00:00:00.000000 drtodo-0.6.4/PKG-INFO
```

### Comparing `drtodo-0.6.3/LICENSE` & `drtodo-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.3/drtodo/README.md` & `drtodo-0.6.4/drtodo/README.md`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.3/drtodo/main.py` & `drtodo-0.6.4/drtodo/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+import inspect
 import re
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Callable
 
 import rich.markdown
 import typer
-from git import Repo
+from git.repo import Repo
 from rich import print
 
 from .man_command import manapp
 from .mdparser import TaskListTraverser, TodoListParser
 from .rich_display import console
-from .settings import constants, globals, settings
+from .settings import constants, globals, settings, Style
 
 app = typer.Typer(
     no_args_is_help=True,
     rich_markup_mode="markdown",
     help=f"**{constants.appname}, MD**: *a straightforward todo list manager for markdown files in git repos.*",
     epilog=f"DrTodo can manage items in a global todo list ({globals.global_todofile_pretty})"
     f" and in a local todo list ({globals.local_todofile_pretty or 'if the current folder is under a git repo'})."
@@ -46,14 +47,15 @@
     ensure_appdir(may_create=True)
 
 
 def print_todo_item(item: dict):
     # print a green large checkmark if checked is True or a blank empty box if checked is False
     # and properly render the markdown text with rich
     # trim trailing whitespace too
+    assert isinstance(settings.style, Style)
     checked_bullet = settings.style.checked
     unchecked_bullet = settings.style.unchecked
 
     strike = ""
     dim = ""
     if item['checked']:
         if settings.style.dim_done:
@@ -73,16 +75,17 @@
 
 
 def print_todo_items(items: list):
     for item in items:
         print_todo_item(item)
 
 
-@app.command()
-def list():
+@app.command(name="list")
+@app.command(name="ls", hidden=True)
+def list_command():
     """
     List todo items in the list
     """
     if globals.global_todofile and globals.global_todofile.exists():
         console().print(f"[header]{globals.global_todofile_pretty}[text]")
         todo = TodoListParser()
         todo.parse(globals.global_todofile)
@@ -90,16 +93,17 @@
     if globals.local_todofile and globals.local_todofile.exists():
         console().print(f"[header]{globals.local_todofile_pretty}[text]")
         todo = TodoListParser()
         todo.parse(globals.local_todofile)
         print_todo_items(todo.items)
 
 
-@app.command()
-def debug():
+@app.command(name="debug")
+@app.command(name="dbg", hidden=True)
+def debug_command():
     """
     List configuration, settings, version and other debug info.
     """
     console().print(f"{version_string()}", highlight=False)
 
     d = constants.__dict__ | dict(settings) | globals.__dict__
     console().print(d)
@@ -109,15 +113,16 @@
     if todofile_path and todofile_path.exists():
         todo = TodoListParser()
         todo.parse(todofile_path)
         # TODO: need to append in the MD file in the right place (once we support sections, etc.)
         todo.add_item_after(add=todo_item, after=todo.items[-1])
         save_todo_backups(todofile_path, todo)
     else:
-        raise typer.Exit(f"Cannot add item to {todofile_path} because it does not exist")
+        print(f"Cannot add item to {todofile_path} because it does not exist")
+        raise typer.Exit(2)
 
 
 # add [--priority <priority>] [--due <due>] [--owner <owner>] [--done] <item description>
 @app.command()
 def add(
     description: str,
     priority: int = typer.Option(None, "--priority", "-p"),
@@ -135,14 +140,15 @@
     prioritystr = f" P{priority}" if priority else ""
     itemstr = f"{prioritystr}{ownerstr}{duestr} {description}".strip()
     todo_item = TaskListTraverser.create_item(itemstr, index=0, checked=done)
     if not global_todo and globals.local_todofile and globals.local_todofile.exists():
         console().print(f"[header]{globals.local_todofile_pretty}[text]")
         _add_item(todo_item, globals.local_todofile)
     else:
+        assert globals.global_todofile
         console().print(f"[header]{globals.global_todofile_pretty}[text]")
         _add_item(todo_item, globals.global_todofile)
     print_todo_item(todo_item)
 
 
 def save_todo_backups(pathname: Path, todo):
     def make_backup_path(i: int) -> Path:
@@ -278,23 +284,93 @@
 
 panel_GLOBAL = "Global Options"
 panel_FILESELECTION = "File Selection Options"
 
 
 # Typer callback handles global options like --mdfile and --verbose
 @app.callback()
-def main(
+def main_callback(
     settings: Optional[Path] = typer.Option(constants.appdir, "--settings", "-s", help="Settings file to use",
                                             rich_help_panel=panel_GLOBAL),
     verbose: Optional[bool] = typer.Option(False, "--verbose", "-v", help="Verbose output",
                                            rich_help_panel=panel_GLOBAL),
     mdfile: Optional[Path] = typer.Option(settings.mdfile, help="Markdown file to use for todo list",
                                           rich_help_panel=panel_FILESELECTION),
     version: Optional[bool] = typer.Option(False, "--version", "-V", help="Show version and exit",
                                            callback=_version_callback, is_eager=True, rich_help_panel=panel_GLOBAL),
 ):
     # BUG: this is called even when the command is init, so it prints a warning about the appdir not existing
     ensure_appdir()
 
 
+# this is fairly generic code that can be used to add aliases to any typer app
+# TODO: move this to a separate package and create decorators for it
+# @app.command_alias(name = 'ls') on the command function
+# @typer_aliases(app=app) on the main() function or maybe @app.typer_aliases()
+def typer_aliases(*, app: typer.Typer,
+                  alias_help_formatter: Optional[Callable[[str], str]] = None,
+                  aliases_help_formatter: Optional[Callable[[str, list[str]], str]] = None) -> None:
+    """
+    Initializes typer aliases for all hidden commands and properly sets the help text for them.
+    Parameters:
+        app: the typer app to modify
+        alias_help_formatter: formats a help string for an aliased command like f"Alias of {command name}"
+        aliases_help_formatter: formats a help string for a command with aliases like f"Aliases: {alias1}, {alias2}"
+    """
+
+    def get_command_name(command_info) -> str:
+        # borrowed from Typer.main.get_command_from_info()
+        name = command_info.name or typer.main.get_command_name(command_info.callback.__name__)
+        return name
+
+    def get_command_help(command_info) -> Optional[str]:
+        # borrowed from Typer.main.get_command_from_info()
+        use_help = command_info.help
+        if use_help is None:
+            use_help = inspect.getdoc(command_info.callback)
+        else:
+            use_help = inspect.cleandoc(use_help)
+        return use_help
+
+    def format_alias_help(aliased_name: str) -> str:
+        if app.rich_markup_mode == "markdown":
+            return f"Alias of `{aliased_name}`"
+        elif app.rich_markup_mode == "rich":
+            return f"Alias of [bold]{aliased_name}[/bold]"
+        else:
+            return f"Alias of {aliased_name}"
+
+    def format_aliases_help(base_help: str, aliases: list[str]) -> str:
+        if app.rich_markup_mode == "markdown":
+            return f"{base_help} *[or {', '.join([f'`{alias}`' for alias in aliases])}]*"
+        elif app.rich_markup_mode == "rich":
+            return f"{base_help} [italics][or {', '.join([f'[bold]{alias}[/bold]' for alias in aliases])}][/italics]"
+        else:
+            return f"{base_help} [or {', '.join(aliases)}]"
+
+    alias_help_formatter = alias_help_formatter or format_alias_help
+    aliases_help_formatter = aliases_help_formatter or format_aliases_help
+
+    aliased_commands = set()
+    # for each command that is not hidden, find any hidden command with the same callback
+    for visible_command in [cmd for cmd in app.registered_commands if not cmd.hidden]:
+        for hidden_command in [cmd for cmd in app.registered_commands if cmd.hidden]:
+            if visible_command.callback == hidden_command.callback:
+                if not hidden_command.help:
+                    hidden_command.help = alias_help_formatter(get_command_name(visible_command))
+                setattr(visible_command, 'aliases', getattr(visible_command, 'aliases', []) + [hidden_command])
+                aliased_commands.add(visible_command)
+
+    # adjust help text for aliased commands
+    for cmd in aliased_commands:
+        basehelp = get_command_help(cmd)
+        if basehelp:
+            cmd.help =  aliases_help_formatter(basehelp, [get_command_name(alias) for alias in cmd.aliases])
+
+
+def main(*args, **kwargs):
+    typer_aliases(app=app)
+    app(*args, **kwargs)
+
+
 if __name__ == "__main__":
-    app()
+    main()
```

### Comparing `drtodo-0.6.3/drtodo/man_command.py` & `drtodo-0.6.4/drtodo/man_command.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.3/drtodo/mdparser.py` & `drtodo-0.6.4/drtodo/mdparser.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.3/drtodo/mistuneplugin.py` & `drtodo-0.6.4/drtodo/mistuneplugin.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.3/drtodo/rich_display.py` & `drtodo-0.6.4/drtodo/rich_display.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.3/drtodo/settings.py` & `drtodo-0.6.4/drtodo/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     import tomllib as toml
 except ImportError:
     import tomli as toml
 from git import Repo
 
 from . import __version__
 
-__all__ = ["constants", "settings", "globals", "initialize", "make_pretty_path"]
+__all__ = ["constants", "settings", "globals", "initialize", "make_pretty_path", "Style"]
 
 
 @dataclass(frozen=True)
 class Constants:
     appname: str = "DrTodo"
     appdir: Path = Path(typer.get_app_dir(appname, force_posix=True))
     version: str = __version__
```

### Comparing `drtodo-0.6.3/PKG-INFO` & `drtodo-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drtodo
-Version: 0.6.3
+Version: 0.6.4
 Summary: DrTodo, MD: todo list manager using markdown files and git
 Home-page: https://github.com/exilium-com/DrTodo
 License: MIT
 Keywords: utilities,todo,markdown
 Author: exilium
 Author-email: info@exilium.com
 Requires-Python: >=3.9,<4.0
```

