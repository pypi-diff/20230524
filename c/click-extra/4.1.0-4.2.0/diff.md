# Comparing `tmp/click_extra-4.1.0.tar.gz` & `tmp/click_extra-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_extra-4.1.0.tar", max compression
+gzip compressed data, was "click_extra-4.2.0.tar", max compression
```

## Comparing `click_extra-4.1.0.tar` & `click_extra-4.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     5362 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/__init__.py
--rw-r--r--   0        0        0    22995 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/colorize.py
--rw-r--r--   0        0        0    14955 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/commands.py
--rw-r--r--   0        0        0    29599 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/config.py
--rw-r--r--   0        0        0     3973 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/decorators.py
--rw-r--r--   0        0        0     6380 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/docs_update.py
--rw-r--r--   0        0        0    11543 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/logging.py
--rw-r--r--   0        0        0     5259 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/parameters.py
--rw-r--r--   0        0        0    14729 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/platforms.py
--rw-r--r--   0        0        0        0 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/py.typed
--rw-r--r--   0        0        0     7754 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/pygments.py
--rw-r--r--   0        0        0     4139 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/run.py
--rw-r--r--   0        0        0     5658 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/sphinx.py
--rw-r--r--   0        0        0     5718 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tabulate.py
--rw-r--r--   0        0        0     2534 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/telemetry.py
--rw-r--r--   0        0        0      770 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/__init__.py
--rw-r--r--   0        0        0    14614 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/conftest.py
--rw-r--r--   0        0        0    17445 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_colorize.py
--rw-r--r--   0        0        0    14025 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_commands.py
--rw-r--r--   0        0        0    21404 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_config.py
--rw-r--r--   0        0        0     7256 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_logging.py
--rw-r--r--   0        0        0     7814 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_parameters.py
--rw-r--r--   0        0        0     9733 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_platforms.py
--rw-r--r--   0        0        0     8047 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_pygments.py
--rw-r--r--   0        0        0     7062 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_run.py
--rw-r--r--   0        0        0    14284 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_tabulate.py
--rw-r--r--   0        0        0     3153 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_telemetry.py
--rw-r--r--   0        0        0     3531 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_timer.py
--rw-r--r--   0        0        0     4585 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_version.py
--rw-r--r--   0        0        0     2385 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/timer.py
--rw-r--r--   0        0        0     7098 2023-05-12 06:28:38.575971 click_extra-4.1.0/click_extra/version.py
--rw-r--r--   0        0        0     6924 2023-05-12 06:28:38.579972 click_extra-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     6637 2023-05-12 06:28:38.579972 click_extra-4.1.0/readme.md
--rw-r--r--   0        0        0     9732 1970-01-01 00:00:00.000000 click_extra-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6030 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/__init__.py
+-rw-r--r--   0        0        0    27870 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/colorize.py
+-rw-r--r--   0        0        0    14955 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/commands.py
+-rw-r--r--   0        0        0    29591 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/config.py
+-rw-r--r--   0        0        0     3973 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/decorators.py
+-rw-r--r--   0        0        0     6380 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/docs_update.py
+-rw-r--r--   0        0        0    11543 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/logging.py
+-rw-r--r--   0        0        0     8515 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/parameters.py
+-rw-r--r--   0        0        0    14061 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/platforms.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/py.typed
+-rw-r--r--   0        0        0     7672 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/pygments.py
+-rw-r--r--   0        0        0     4139 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/run.py
+-rw-r--r--   0        0        0     6094 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/sphinx.py
+-rw-r--r--   0        0        0     5718 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tabulate.py
+-rw-r--r--   0        0        0     2534 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/telemetry.py
+-rw-r--r--   0        0        0      770 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/__init__.py
+-rw-r--r--   0        0        0    14766 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/conftest.py
+-rw-r--r--   0        0        0    17759 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_colorize.py
+-rw-r--r--   0        0        0    14048 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_commands.py
+-rw-r--r--   0        0        0    21404 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_config.py
+-rw-r--r--   0        0        0     7259 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_logging.py
+-rw-r--r--   0        0        0     7814 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_parameters.py
+-rw-r--r--   0        0        0     9733 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_platforms.py
+-rw-r--r--   0        0        0     8377 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_pygments.py
+-rw-r--r--   0        0        0     7062 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_run.py
+-rw-r--r--   0        0        0    14284 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_tabulate.py
+-rw-r--r--   0        0        0     3153 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_telemetry.py
+-rw-r--r--   0        0        0     3531 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_timer.py
+-rw-r--r--   0        0        0     4585 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_version.py
+-rw-r--r--   0        0        0     2385 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/timer.py
+-rw-r--r--   0        0        0     7098 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/version.py
+-rw-r--r--   0        0        0     6950 2023-05-24 07:54:57.921645 click_extra-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6637 2023-05-24 07:54:57.921645 click_extra-4.2.0/readme.md
+-rw-r--r--   0        0        0     9681 1970-01-01 00:00:00.000000 click_extra-4.2.0/PKG-INFO
```

### Comparing `click_extra-4.1.0/click_extra/__init__.py` & `click_extra-4.2.0/click_extra/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,47 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Expose package-wide elements."""
 
-__version__ = "4.1.0"
+import sys
+
+__version__ = "4.2.0"
 """Examples of valid version strings according :pep:`440#version-scheme`:
 
 .. code-block:: python
 
     __version__ = "1.2.3.dev1"  # Development release 1
     __version__ = "1.2.3a1"  # Alpha Release 1
     __version__ = "1.2.3b1"  # Beta Release 1
     __version__ = "1.2.3rc1"  # RC Release 1
     __version__ = "1.2.3"  # Final Release
     __version__ = "1.2.3.post1"  # Post Release 1
 """
 
+if sys.version_info >= (3, 9):
+    from functools import cache
+else:
+    from functools import lru_cache
+
+    def cache(user_function):
+        """Simple lightweight unbounded cache. Sometimes called "memoize".
+
+        .. important::
+
+            This is a straight `copy of the functools.cache implementation
+            <https://github.com/python/cpython/blob/55a26de/Lib/functools.py#L647-L653>`_,
+            which is only `available in the standard library starting with Python v3.9
+            <https://docs.python.org/3/library/functools.html?highlight=caching#functools.cache>`.
+        """
+        return lru_cache(maxsize=None)(user_function)
+
+
 # Import all click's module-level content to allow for drop-in replacement.
 # XXX Star import is really badly supported by mypy for now and leads to lots of
 # "Module 'XXX' has no attribute 'YYY'". See: https://github.com/python/mypy/issues/4930
 # Overrides click helpers with cloup's.
 from click import *  # noqa: E402, F403
 from click.core import ParameterSource  # noqa: E402, F401
 from cloup import *  # type: ignore[no-redef] # noqa: E402, F403
```

### Comparing `click_extra-4.1.0/click_extra/colorize.py` & `click_extra-4.2.0/click_extra/colorize.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,90 +18,127 @@
 from __future__ import annotations
 
 import os
 import re
 from configparser import RawConfigParser
 from gettext import gettext as _
 from operator import getitem
-from typing import NamedTuple, Sequence
+from typing import NamedTuple, Sequence, cast, Optional
 
 import regex as re3
 from boltons.strutils import complement_int_list, int_ranges_from_int_list
 from cloup._util import identity
-from cloup.styling import IStyle
+from cloup.styling import IStyle, Color
+from cloup.typing import MISSING, Possibly
+import click
 
 from . import (
     Choice,
     Context,
     HelpFormatter,
     Parameter,
     ParameterSource,
     Style,
     echo,
     get_current_context,
+    cache,
 )
 from .parameters import ExtraOption
 
 
 class HelpExtraTheme(NamedTuple):
-    """Extends ``cloup.HelpTheme`` with Click Extra's specific properties and
-    ``logging.levels``.
+    """Extends ``cloup.HelpTheme`` with extra properties and ``logging.levels``.
 
-    We had to redefined all fields and couldn't extend ``cloup.HelpTheme`` as there is
-    no way to cleanly do it because of mypy. See:
-    https://github.com/python/typing/issues/427
-    https://mypy.readthedocs.io/en/stable/runtime_troubles.html#future-annotations-import-pep-563
+    .. caution::
+        We had to redefined all fields and couldn't extend ``cloup.HelpTheme`` as there
+        is no way to cleanly do it with MyPy.
+
+        See:
+        - https://github.com/python/typing/issues/427
+        - https://mypy.readthedocs.io/en/stable/runtime_troubles.html#future-annotations-import-pep-563
     """
 
-    # Hard-copy from cloup.HelpTheme.
     invoked_command: IStyle = identity
     command_help: IStyle = identity
     heading: IStyle = identity
     constraint: IStyle = identity
     section_help: IStyle = identity
     col1: IStyle = identity
     col2: IStyle = identity
+    alias: IStyle = identity
+    alias_secondary: Optional[IStyle] = None
     epilog: IStyle = identity
+    """Set of properties inherited from ``cloup.HelpTheme``.
+
+    See: https://cloup.readthedocs.io/en/stable/autoapi/cloup/index.html#cloup.HelpTheme.invoked_command
+    """
 
-    # Log levels from Python's logging module.
     critical: IStyle = identity
     error: IStyle = identity
     warning: IStyle = identity
     info: IStyle = identity
     debug: IStyle = identity
+    """Log levels from Python's logging module."""
 
-    # Click Extra new coloring properties.
-    subheading: IStyle = identity
     option: IStyle = identity
+    subcommand: IStyle = identity
     choice: IStyle = identity
     metavar: IStyle = identity
+    bracket: IStyle = identity
+    envvar: IStyle = identity
+    default: IStyle = identity
+    deprecated: IStyle = identity
     search: IStyle = identity
     success: IStyle = identity
+    """Click Extra new coloring properties."""
+
+    subheading: IStyle = identity
+    """Non-canonical Click Extra properties.
+
+    .. note::
+        Subheading is used for sub-sections, like `in the help of mail-deduplicate
+        <https://github.com/kdeldycke/mail-deduplicate/blob/0764287/mail_deduplicate/deduplicate.py#L445>`_.
+
+    .. todo::
+        Maybe this shouln't be in Click Extra because it is a legacy inheritance from
+        one of my other project.
+    """
 
     def with_(
         self,
+        ### Cloup properties.
         invoked_command: IStyle | None = None,
         command_help: IStyle | None = None,
         heading: IStyle | None = None,
         constraint: IStyle | None = None,
         section_help: IStyle | None = None,
         col1: IStyle | None = None,
         col2: IStyle | None = None,
+        alias: IStyle | None = None,
+        alias_secondary: Possibly[Optional[IStyle]] = MISSING,
         epilog: IStyle | None = None,
+        ### Log levels.
         critical: IStyle | None = None,
         error: IStyle | None = None,
         warning: IStyle | None = None,
         info: IStyle | None = None,
         debug: IStyle | None = None,
-        subheading: IStyle | None = None,
+        ### Click Extra properties.
         option: IStyle | None = None,
+        subcommand: IStyle | None = None,
         choice: IStyle | None = None,
         metavar: IStyle | None = None,
+        bracket: IStyle | None = None,
+        envvar: IStyle | None = None,
+        default: IStyle | None = None,
+        deprecated: IStyle | None = None,
         search: IStyle | None = None,
         success: IStyle | None = None,
+        ### Non-canonical Click Extra properties.
+        subheading: IStyle | None = None,
     ) -> HelpExtraTheme:
         """Copy of ``cloup.HelpTheme.with_``."""
         kwargs = {key: val for key, val in locals().items() if val is not None}
         kwargs.pop("self")
         if kwargs:
             return self._replace(**kwargs)
         return self
@@ -125,35 +162,45 @@
             Implement default light theme.
         """
         raise NotImplementedError
 
 
 # Populate our global theme with all default styles.
 default_theme = HelpExtraTheme(
-    # Cloup properties.
-    invoked_command=Style(fg="bright_white"),
-    heading=Style(fg="bright_blue", bold=True),
-    constraint=Style(fg="magenta"),
+    ### Cloup styles.
+    invoked_command=Style(fg=Color.bright_white),
+    heading=Style(fg=Color.bright_blue, bold=True, underline=True),
+    constraint=Style(fg=Color.magenta),
     # Neutralize Cloup's col1, as it interfers with our finer option styling
     # which takes care of separators.
     col1=identity,
-    # Log levels.
-    critical=Style(fg="red"),
-    error=Style(fg="red"),
-    warning=Style(fg="yellow"),
-    # INFO log level is the default, so no style applied.
-    info=identity,
-    debug=Style(fg="blue"),
-    # Click Extra properties.
-    subheading=Style(fg="blue"),
-    option=Style(fg="cyan"),
-    choice=Style(fg="magenta"),
-    metavar=Style(fg="bright_black"),
-    search=Style(fg="green", bold=True),
-    success=Style(fg="green"),
+    # Style aliases like options and subcommands.
+    alias=Style(fg=Color.cyan),
+    # Style aliases punctuation like options, but dimmed.
+    alias_secondary=Style(fg=Color.cyan, dim=True),
+    ### Log styles.
+    critical=Style(fg=Color.red, bold=True),
+    error=Style(fg=Color.red),
+    warning=Style(fg=Color.yellow),
+    info=identity,  # INFO level is the default, so no style applied.
+    debug=Style(fg=Color.blue),
+    ### Click Extra styles.
+    option=Style(fg=Color.cyan),
+    # Style subcommands like options and aliases.
+    subcommand=Style(fg=Color.cyan),
+    choice=Style(fg=Color.magenta),
+    metavar=Style(fg=Color.cyan, dim=True),
+    bracket=Style(dim=True),
+    envvar=Style(fg=Color.yellow, dim=True),
+    default=Style(fg=Color.green, dim=True, italic=True),
+    deprecated=Style(fg=Color.bright_yellow, bold=True),
+    search=Style(fg=Color.green, bold=True),
+    success=Style(fg=Color.green),
+    ### Non-canonical Click Extra styles.
+    subheading=Style(fg=Color.blue),
 )
 
 
 # No color theme.
 nocolor_theme = HelpExtraTheme()
 
 
@@ -321,14 +368,16 @@
         subcommands: set[str] = set()
         command_aliases: set[str] = set()
         options: set[str] = set()
         long_options: set[str] = set()
         short_options: set[str] = set()
         choices: set[str] = set()
         metavars: set[str] = set()
+        envvars: set[str] = set()
+        defaults: set[str] = set()
 
         # Includes CLI base name and its commands.
         cli_names.add(ctx.command_path)
         command = ctx.command
 
         # Will fetch command's metavar (i.e. the "[OPTIONS]" after the CLI name in
         # "Usage:") and dig into subcommands to get subcommand_metavar:
@@ -341,24 +390,31 @@
             for sub_id in subcommands:
                 sub_cmd = command.get_command(ctx, sub_id)
                 command_aliases.update(getattr(sub_cmd, "aliases", []))
 
         # Add user defined help options.
         options.update(ctx.help_option_names)
 
-        # Collect all option names and choice keywords.
+        # Collect all options, choices, metavars, envvars and default values.
         for param in command.params:
             options.update(param.opts)
             options.update(param.secondary_opts)
 
             if isinstance(param.type, Choice):
                 choices.update(param.type.choices)
 
             metavars.add(param.make_metavar())
 
+            envvars.update(param.envvar)
+
+            if isinstance(param, click.Option):
+                default_string = ExtraOption.get_help_default(param, ctx)
+                if default_string:
+                    defaults.add(default_string)
+
         # Split between shorts and long options
         for option_name in options:
             # Short options are no longer than 2 characters like "-D", "/d", "/?",
             # "+w", "-w", "f_", "_f", ...
             # XXX We cannot reuse the _short_opts and _long_opts attributes from
             # https://github.com/pallets/click/blob/b0538df/src/click/parser.py#L173-L182
             # because their values are not passed when the context is updated like
@@ -376,14 +432,16 @@
             cli_names,
             subcommands,
             command_aliases,
             long_options,
             short_options,
             choices,
             metavars,
+            envvars,
+            defaults,
         )
 
     def get_help(self, ctx):
         """Replace default formatter by our own."""
         ctx.formatter_class = HelpExtraFormatter
         return super().get_help(ctx)
 
@@ -393,14 +451,16 @@
             formatter.cli_names,
             formatter.subcommands,
             formatter.command_aliases,
             formatter.long_options,
             formatter.short_options,
             formatter.choices,
             formatter.metavars,
+            formatter.envvars,
+            formatter.defaults,
         ) = self.collect_keywords(ctx)
         return super().format_help(ctx, formatter)
 
 
 def escape_for_help_sceen(text: str) -> str:
     """Escape a text to be used in a regural expression to match help screen.
 
@@ -439,118 +499,173 @@
     cli_names: set[str] = set()
     subcommands: set[str] = set()
     command_aliases: set[str] = set()
     long_options: set[str] = set()
     short_options: set[str] = set()
     choices: set[str] = set()
     metavars: set[str] = set()
-    # TODO
-    default_values: set[str] = set()
+    envvars: set[str] = set()
+    defaults: set[str] = set()
 
     # TODO: Hihglight extra keywords <stdout> or <stderr>
 
-    def style_group(self, str_to_style: str, group_id: str):
-        style_alias = {
-            "default_start": self.theme.metavar,
-            "default_end": self.theme.metavar,
-            "default_value": self.theme.choice,
-            "subcommand": self.theme.option,
-            "command_aliases": self.theme.option,
-            "long_option": self.theme.option,
-            "short_option": self.theme.option,
-        }
-        # Get the style directly named by the group ID. Else inspect the
-        # style_alias above.
-        group_style = getattr(self.theme, group_id, None)
-        if not group_style:
-            group_style = style_alias[group_id]
-        return group_style(str_to_style)
+    # TODO: add collection of regexps as pre-compiled constants, so we can
+    # inspect them and get some performances improvements.
+
+    style_aliases = {
+        # Layout elements of the square brackets trailing each option.
+        "bracket_1": "bracket",
+        "bracket_2": "bracket",
+        "label_sep": "bracket",
+        "envvar_label": "bracket",
+        "default_label": "bracket",
+        # Long and short options are options.
+        "long_option": "option",
+        "short_option": "option",
+    }
+    """Map regex's group IDs to styles.
+
+    Most of the time, the style name is the same as the group ID. But some regular
+    expression implementations requires us to work around group IDs limitations, like
+    ``bracket_1`` and ``bracket_2``. In which case we use this mapping to apply back
+    the canonical style to that regex-specific group ID.
+    """
+
+    @cache
+    def get_style_id(self, group_id: str) -> str:
+        """Get the style ID to apply to a group.
+
+        Return the style which has the same ID as the group, unless it is defined in
+        the ``style_aliases`` mapping above.
+        """
+        return self.style_aliases.get(group_id, group_id)
+
+    @cache
+    def colorize_group(self, str_to_style: str, group_id: str) -> str:
+        """Colorize a string according to the style of the group ID."""
+        style = cast("IStyle", getattr(self.theme, self.get_style_id(group_id)))
+        return style(str_to_style)
 
     def colorize(self, match: re.Match) -> str:
-        """Recreate the matching string by concatenating all groups, but only colorize
-        named groups with using the function provided in ``style_map``."""
-        # Invert the group dictionnary to we can get the group ID of a match.
-        match_group = {v: k for k, v in match.groupdict().items()}
-        assert len(match_group) == len(match.groupdict())
+        """Colorize all groups with IDs in the provided matching result.
+
+        All groups without IDs are left as-is.
+
+        All groups are proccessed in the order they appear in the ``match`` object.
+        Then all groups are concatenated to form the final string that is returned.
+
+        .. caution::
+            Implementation is a bit funky here because there is no way to iterate over
+            both unnamed and named groups, in the order they appear in the regex, while
+            keeping track of the group ID.
+
+            So we have to iterate over the list of matching strings and pick up the
+            corresponding group ID along the way, from the ``match.groupdict()``
+            dictionnary. This also means we assume that the ``match.groupdict()`` is
+            returning an ordered dictionnary. Which is supposed to be true as of Python
+            3.7.
+        """
+        # Get a snapshot of all named groups.
+        named_matches = list(match.groupdict().items())
 
         txt = ""
-        for group in match.groups():
-            if group in match_group:
-                group_id = match_group[group]
-                txt += self.style_group(group, group_id)
+        # Iterate over all groups, named or not.
+        for group_string in match.groups():
+            # Is the next available named group is matching current group string?
+            if named_matches and group_string == named_matches[0][1]:
+                # We just found a named group. Consume it from the list of named groups
+                # to prevent it from being processed twice.
+                group_id, group_string = named_matches.pop(0)
+                if group_string is not None:
+                    # Colorize the group with a style matching its ID.
+                    txt += self.colorize_group(group_string, group_id)
             else:
-                txt += group
+                # No named group matching this string. Leave it as-is.
+                txt += group_string
+
+        # Double-check we processed all named groups.
+        if len(named_matches) != 0:
+            raise ValueError(
+                "The matching result contains named groups that were not processed. "
+                "There is an edge-case in the design of regular expressions."
+            )
+
         return txt
 
     def highlight_extra_keywords(self, help_text):
         """Highlight extra keywords in help screens based on the theme.
 
         It is based on regular expressions. While this is not a bullet-proof method, it
         is good enough. After all, help screens are not consumed by machine but are
         designed for humans.
+
+        .. danger::
+            All the regular expressions below are designed to match its original string
+            into a sequence of contiguous groups.
+
+            This means each part of the matching result must be encapsulated in a group.
+            And subgroups are not allowed (unless their are explicitly set as
+            non-matching with ``(?:...)`` prefix).
+
+            Groups with a name must have a corresponding style.
         """
-        # Highlight " (Deprecated)" or " (DEPRECATED)" labels, as set by either:
-        # https://github.com/pallets/click/blob/ef11be6e49e19a055fe7e5a89f0f1f4062c68dba/tests/test_commands.py#L345
-        # https://github.com/janluke/cloup/blob/c29fa051ed405856ed8bc2dbd733f9df2c8e6418/cloup/formatting/_formatter.py#L188
+        # Highlight " (Deprecated)" label, as set by either Click or Cloup:
+        # https://github.com/pallets/click/blob/8.0.0rc1/tests/test_commands.py#L322
+        # https://github.com/janluke/cloup/blob/v2.1.0/cloup/formatting/_formatter.py#L190
         help_text = re.sub(
             rf"""
-            (\s)                                      # Any blank char.
-            (?P<warning>{re.escape("(DEPRECATED)")})  # The flag string.
+            (\s)                                         # Any blank char.
+            (?P<deprecated>{re.escape("(Deprecated)")})  # The flag string.
             """,
             self.colorize,
             help_text,
-            flags=re.VERBOSE | re.IGNORECASE,
+            flags=re.VERBOSE,
         )
 
-        # Highligh subcommands' aliases.
-        for alias in self.command_aliases:
-            help_text = re.sub(
-                rf"""
-                (
-                    \ \                       # 2 spaces (i.e. section indention).
-                    \S+                       # Any subcommand.
-                    \                         # A space.
-                    \(                        # An opening parenthesis.
-                    .*                        # Any string.
-                )
-                (?P<command_aliases>{re.escape(alias)})  # The alias.
-                (
-                    .*                        # Any string.
-                    \)                        # A closing parenthesis.
-                )
-                """,
-                self.colorize,
-                help_text,
-                flags=re.VERBOSE,
-            )
-
         # Highligh subcommands.
         for subcommand in self.subcommands:
             help_text = re.sub(
                 rf"""
                 (\ \ )                        # 2 spaces (i.e. section indention).
                 (?P<subcommand>{re.escape(subcommand)})
                 (\s)                          # Any blank char.
                 """,
                 self.colorize,
                 help_text,
                 flags=re.VERBOSE,
             )
 
-        # Highligh defaults.
+        # Highligh environment variables and defaults in trailing square brackets.
         help_text = re.sub(
             r"""
             (\ \ )                  # 2 spaces (column spacing or description spacing).
-            (?P<default_start>
-                \[                  # Square brackets opening.
-                default:            # Starting content within the brackets.
+            (?P<bracket_1>\[)                  # Square brackets opening.
+
+            (?:                         # Non-capturing group.
+                (?P<envvar_label>
+                    env\s+var:            # Starting content within the brackets.
+                    \s+                 # Any number of blank chars.
+                )
+                (?P<envvar>.+?)  # Greedy-matching of any string and line returns.
+            )?                  # The envvar group is optional.
+
+            (?P<label_sep>
+                ;               # Separator between labels.
                 \s+                 # Any number of blank chars.
-            )
-            (?P<default_value>.+?)  # Greedy-matching of any string and line returns.
-            (?P<default_end>\])     # Square brackets closing.
+            )?
+
+            (?:                         # Non-capturing group.
+                (?P<default_label>
+                    default:            # Starting content within the brackets.
+                    \s+                 # Any number of blank chars.
+                )
+                (?P<default>.+?)  # Greedy-matching of any string and line returns.
+            )?                      # The default group is optional.
+
+            (?P<bracket_2>\])     # Square brackets closing.
             """,
             self.colorize,
             help_text,
             flags=re.VERBOSE | re.DOTALL,
         )
 
         # Highlight CLI names and commands.
```

### Comparing `click_extra-4.1.0/click_extra/commands.py` & `click_extra-4.2.0/click_extra/commands.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.1.0/click_extra/config.py` & `click_extra-4.2.0/click_extra/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -618,15 +618,15 @@
 
     def load_conf(self, ctx, param, path_pattern):
         """Fetch parameters values from configuration file and merge them with the
         defaults.
 
         User configuration is
         `merged to the context default_map as Click does <https://click.palletsprojects.com/en/8.1.x/commands/#context-defaults>`_.
-        
+
         This allow user's config to only overrides defaults. Values sets from direct
         command line parameters, environment variables or interactive prompts, takes
         precedence over any values from the config file.
         """
         logger = logging.getLogger("click_extra")
 
         explicit_conf = ctx.get_parameter_source("config") in (
```

### Comparing `click_extra-4.1.0/click_extra/decorators.py` & `click_extra-4.2.0/click_extra/decorators.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.1.0/click_extra/docs_update.py` & `click_extra-4.2.0/click_extra/docs_update.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.1.0/click_extra/logging.py` & `click_extra-4.2.0/click_extra/logging.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.1.0/click_extra/platforms.py` & `click_extra-4.2.0/click_extra/platforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,31 +29,15 @@
 from __future__ import annotations
 
 import platform
 import sys
 from dataclasses import dataclass, field
 from typing import Iterable
 
-if sys.version_info >= (3, 9):
-    from functools import cache
-else:
-    from functools import lru_cache
-
-    def cache(user_function):
-        """Simple lightweight unbounded cache. Sometimes called "memoize".
-
-        .. important::
-
-            This is a straight `copy of the functools.cache implementation
-            <https://github.com/python/cpython/blob/55a26de6ba938962dc23f2495723cf0f4f3ab7c6/Lib/functools.py#L647-L653>`_,
-            which is only `available in the standard library starting with Python v3.9
-            <https://docs.python.org/3/library/functools.html?highlight=caching#functools.cache>`.
-        """
-        return lru_cache(maxsize=None)(user_function)
-
+from . import cache
 
 """ Below is the collection of heuristics used to identify each platform.
 
 All these heuristics can be hard-cached as the underlying system is not suppose to
 change between code execution.
 """
```

### Comparing `click_extra-4.1.0/click_extra/pygments.py` & `click_extra-4.2.0/click_extra/pygments.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,90 +9,44 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
-"""Helpers and utilities to allow Pygments to parse and render ANSI codes.
-
-.. warning::
-
-    Styling has been hard-coded to match the default style of the `Furo Sphinx theme
-    <https://github.com/pradyunsg/furo>`_.
-
-    We will revisit this in the future to make it more flexible for new users with
-    different needs.
-"""
+"""Helpers and utilities to allow Pygments to parse and render ANSI codes."""
 
 from __future__ import annotations
 
-from configparser import ConfigParser
-
-import furo
 from pygments import lexers
 from pygments.filter import Filter
 from pygments.filters import TokenMergeFilter
 from pygments.formatters import HtmlFormatter
+from pygments.formatter import _lookup_style  # type: ignore[attr-defined]
 from pygments.lexer import Lexer, LexerMeta
 from pygments.lexers.algebra import GAPConsoleLexer
 from pygments.lexers.dylan import DylanConsoleLexer
 from pygments.lexers.erlang import ElixirConsoleLexer, ErlangShellLexer
 from pygments.lexers.julia import JuliaConsoleLexer
 from pygments.lexers.matlab import MatlabSessionLexer
 from pygments.lexers.php import PsyshConsoleLexer
 from pygments.lexers.python import PythonConsoleLexer
 from pygments.lexers.r import RConsoleLexer
 from pygments.lexers.ruby import RubyConsoleLexer
 from pygments.lexers.shell import ShellSessionBaseLexer
 from pygments.lexers.special import OutputLexer
 from pygments.lexers.sql import PostgresConsoleLexer, SqliteConsoleLexer
 from pygments.style import StyleMeta
-from pygments.styles import get_style_by_name
 from pygments.token import Generic, string_to_tokentype
 from pygments_ansi_color import (
     AnsiColorLexer,
     ExtendedColorHtmlFormatterMixin,
     color_tokens,
 )
 
-fg_colors = bg_colors = {
-    "Black": "#000000",
-    "Red": "#EF2929",
-    "Green": "#8AE234",
-    "Yellow": "#FCE94F",
-    "Blue": "#3465A4",
-    "Magenta": "#c509c5",
-    "Cyan": "#34E2E2",
-    "White": "#ffffff",
-}
-"""Hard-coded default style for ANSI code rendering.
-
-.. todo::
-
-    Make this more configurable.
-"""
-
-
-# Extract the name of furo's default pygment style, as defined in:
-# https://github.com/pradyunsg/furo/blob/8eba6499b812d7aeab2a99fcdf33e8bcb07b05fc/src/furo/theme/furo/theme.conf#L4
-furo_conf = furo.THEME_PATH / "theme.conf"
-ini_config = ConfigParser()
-ini_config.read_string(furo_conf.read_text())
-furo_style_name = ini_config.get("theme", "pygments_style")
-
-
-# Base our new custom style in furo's.
-style_base: StyleMeta = get_style_by_name(furo_style_name)
-
-
-class AnsiClickExtraFuroStyle(style_base):  # type: ignore
-    styles = dict(style_base.styles)
-    styles.update(color_tokens(fg_colors, bg_colors, enable_256color=True))
-
 
 DEFAULT_TOKEN_TYPE = Generic.Output
 """Default Pygments' token type to render with ANSI support.
 
 We defaults to ``Generic.Output`` tokens, as this is the token type used by all REPL-
 like and terminal lexers.
 """
@@ -160,17 +114,17 @@
         """
         super().__init__(*args, **kwargs)
         self.filters.append(TokenMergeFilter())
         self.filters.append(AnsiFilter())
 
 
 def collect_session_lexers():
-    """Retrieve among default Pygments lexers those producing shell-like sessions.
+    """Retrieve all lexers producing shell-like sessions in Pygments.
 
-    This function contain a anually-maintained list of lexers, to which we dynamiccaly
+    This function contain a manually-maintained list of lexers, to which we dynamiccaly
     adds lexers inheriting from ``ShellSessionBaseLexer``.
 
     .. hint::
 
         To help maintain this list, there is `a test that will fail
         <https://github.com/kdeldycke/click-extra/blob/main/click_extra/tests/test_pygments.py>`_
         if a new REPL/terminal-like lexer is added to Pygments but not referenced here.
@@ -213,7 +167,34 @@
 
     `Adds support for ANSI 256 colors
     <https://github.com/chriskuehl/pygments-ansi-color#optional-enable-256-color-support>`_.
     """
 
     name = "ANSI HTML"
     aliases = ["ansi-html"]
+
+    def __init__(self, **kwargs):
+        """Intercept the ``style`` argument to augment it with ANSI colors support.
+
+        Creates a new style instance that inherits from the one provided by the user,
+        but updates its ``styles`` attribute to add ANSI colors support from
+        ``pygments_ansi_color``.
+        """
+        # XXX Same default style as in Pygments' HtmlFormatter, which is... `default`:
+        # https://github.com/pygments/pygments/blob/1d83928/pygments/formatter.py#LL89C33-L89C33
+        base_style_id = kwargs.setdefault("style", "default")
+
+        # Fetch user-provided style.
+        base_style = _lookup_style(base_style_id)
+
+        # Augment the style with ANSI colors support.
+        augmented_styles = dict(base_style.styles)
+        augmented_styles.update(color_tokens(enable_256color=True))
+
+        # Prefix the style name with `Ansi` to avoid name collision with the original
+        # and ease debugging.
+        new_name = f"Ansi{base_style.__name__}"
+        new_lexer = StyleMeta(new_name, (base_style,), {"styles": augmented_styles})
+
+        kwargs["style"] = new_lexer
+
+        super().__init__(**kwargs)
```

### Comparing `click_extra-4.1.0/click_extra/run.py` & `click_extra-4.2.0/click_extra/run.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.1.0/click_extra/sphinx.py` & `click_extra-4.2.0/click_extra/sphinx.py`

 * *Files 20% similar despite different names*

```diff
@@ -75,33 +75,28 @@
 Emulates:
     .. code-block:: python
 
         import click._compat
 
         click._compat.text_type = str
 
+.. hint::
+    A fix has been proposed upstream at
+    `pallets-sphinx-themes#69 <https://github.com/pallets/pallets-sphinx-themes/pull/69>`_
+    and is waiting for a merge.
+
 .. seealso::
     - `similar hack in click 8.x's docs/conf.py
       <https://github.com/pallets/click/commit/00883dd3d0a29f68f375cab5e21cef0669941aba#diff-85933aa74a2d66c3e4dcdf7a9ad8397f5a7971080d34ef1108296a7c6b69e7e3>`_
 
     - `incriminating import in pallets_sphinx_themes
       <https://github.com/pallets/pallets-sphinx-themes/blob/7b69241/src/pallets_sphinx_themes/themes/click/domain.py#L9>`_
-
-.. tip::
-    A fix has been proposed upstream at
-    `pallets-sphinx-themes#69 <https://github.com/pallets/pallets-sphinx-themes/pull/69>`_.
 """
 
 
-def setup_ansi_pygment_styles(app):
-    """Add support for ANSI Shell Session syntax highlighting."""
-    app.config.pygments_style = "ansi-click-extra-furo-style"
-    PygmentsBridge.html_formatter = AnsiHtmlFormatter
-
-
 class PatchedViewList(ViewList):
     """Force the rendering of ANSI shell session.
 
     Replaces the ``.. sourcecode:: shell-session`` code block produced by
     ``.. click:run::`` directive with an ANSI Shell Session:
     ``.. code-block:: ansi-shell-session``.
 
@@ -124,16 +119,30 @@
 
 def setup(app):
     """Register new directives, augmented with ANSI coloring.
 
     New directives:
         - ``.. click:example::``
         - ``.. click:run::``
+
+    .. danger::
+        This function activates lots of monkey-patches:
+
+        - ``sphinx.highlighting.PygmentsBridge`` is updated to set its default HTML
+        formatter to an ANSI capable one for the whole Sphinx app.
+
+        - ``click_compat_hack`` to `bypass old Python 2.x in pallets-sphinx-themes
+        <#click_extra.sphinx.click_compat_hack>`.
+
+        - ``pallets_sphinx_themes.themes.click.domain.ViewList`` is
+        `patched to force an ANSI lexer on the rST code block
+        <#click_extra.sphinx.PatchedViewList>`_.
     """
-    setup_ansi_pygment_styles(app)
+    # Set Sphinx's default HTML formatter to an ANSI capable one.
+    PygmentsBridge.html_formatter = AnsiHtmlFormatter
 
     with click_compat_hack:
         from pallets_sphinx_themes.themes.click import domain
 
         domain.ViewList = PatchedViewList
 
         ####################################
```

### Comparing `click_extra-4.1.0/click_extra/tabulate.py` & `click_extra-4.2.0/click_extra/tabulate.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.1.0/click_extra/telemetry.py` & `click_extra-4.2.0/click_extra/telemetry.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.1.0/click_extra/tests/__init__.py` & `click_extra-4.2.0/click_extra/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.1.0/click_extra/tests/conftest.py` & `click_extra-4.2.0/click_extra/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -156,17 +156,17 @@
 
         # Extra parameters passed to the invoked command's ``main()`` constructor.
         extra = {}
         if color == "forced":
             extra["color"] = True
 
         with monkeypatch.context() as patch:
-            # Monkeypatch the original command's ``main()`` call to pass extra parameter
-            # for Context initialization. Because we cannot simply add ``color`` to
-            # ``**extra``.
+            # Monkeypatch the original command's ``main()`` call to pass extra
+            # parameter for Context initialization. Because we cannot simply add
+            # ``color`` to ``**extra``.
             patch.setattr(cli, "main", partial(cli.main, **extra))
 
             result = runner.invoke(cli=cli, args=args, env=env, color=bool(color))
 
         # Force stripping of all colors from results.
         if color is False:
             result.stdout_bytes = strip_ansi(result.stdout_bytes)
@@ -344,37 +344,41 @@
     r"  --version                 Show the version and exit.\n"
     r"  -h, --help                Show this message and exit.\n"
 )
 
 
 default_options_colored_help = (
     r"  \x1b\[36m--time\x1b\[0m / \x1b\[36m--no-time\x1b\[0m"
-    r"        Measure and print elapsed execution time.  \x1b\[90m\[default:\n"
-    r"                            \x1b\[0m\x1b\[35mno-time\x1b\[0m\x1b\[90m\]\x1b\[0m\n"
+    r"        Measure and print elapsed execution time."
+    r"  \x1b\[2m\[\x1b\[0m\x1b\[2mdefault:\n"
+    r"                            "
+    r"\x1b\[0m\x1b\[32m\x1b\[2m\x1b\[3mno-time\x1b\[0m\x1b\[2m\]\x1b\[0m\n"
     r"  \x1b\[36m--color\x1b\[0m, \x1b\[36m--ansi\x1b\[0m /"
     r" \x1b\[36m--no-color\x1b\[0m, \x1b\[36m--no-ansi\x1b\[0m\n"
     r"                            Strip out all colors and all ANSI codes from"
     r" output.\n"
-    r"                            \x1b\[90m\[default:"
-    r" \x1b\[0m\x1b\[35mcolor\x1b\[0m\x1b\[90m\]\x1b\[0m\n"
-    r"  \x1b\[36m-C\x1b\[0m, \x1b\[36m--config\x1b\[0m \x1b\[90mCONFIG_PATH\x1b\[0m"
+    r"                            \x1b\[2m\[\x1b\[0m\x1b\[2mdefault:"
+    r" \x1b\[0m\x1b\[32m\x1b\[2m\x1b\[3mcolor\x1b\[0m\x1b\[2m\]\x1b\[0m\n"
+    r"  \x1b\[36m-C\x1b\[0m, \x1b\[36m--config\x1b\[0m"
+    r" \x1b\[36m\x1b\[2mCONFIG_PATH\x1b\[0m"
     r"  Location of the configuration file. Supports glob\n"
     r"                            pattern of local path and remote URL."
-    r"  \x1b\[90m\[default:( \S+)?\n"
+    r"  \x1b\[2m\[\x1b\[0m\x1b\[2mdefault:( \S+)?\n"
     r"(                            .+\n)*"
     r"                            "
-    r"\S+\.{toml,yaml,yml,json,ini,xml}\x1b\[0m\x1b\[90m\]\x1b\[0m\n"
+    r"\S+\.{toml,yaml,yml,json,ini,xml}\x1b\[0m\x1b\[2m\]\x1b\[0m\n"
     r"  \x1b\[36m--show-params\x1b\[0m"
     r"             Show all CLI parameters, their provenance, defaults\n"
     r"                            and value, then exit.\n"
-    r"  \x1b\[36m-v\x1b\[0m, \x1b\[36m--verbosity\x1b\[0m \x1b\[90mLEVEL\x1b\[0m"
+    r"  \x1b\[36m-v\x1b\[0m, \x1b\[36m--verbosity\x1b\[0m"
+    r" \x1b\[36m\x1b\[2mLEVEL\x1b\[0m"
     r"     Either \x1b\[35mCRITICAL\x1b\[0m, \x1b\[35mERROR\x1b\[0m, "
     r"\x1b\[35mWARNING\x1b\[0m, \x1b\[35mINFO\x1b\[0m, \x1b\[35mDEBUG\x1b\[0m.\n"
-    r"                            \x1b\[90m\[default: "
-    r"\x1b\[0m\x1b\[35mWARNING\x1b\[0m\x1b\[90m\]\x1b\[0m\n"
+    r"                            \x1b\[2m\[\x1b\[0m\x1b\[2mdefault: "
+    r"\x1b\[0m\x1b\[32m\x1b\[2m\x1b\[3mWARNING\x1b\[0m\x1b\[2m\]\x1b\[0m\n"
     r"  \x1b\[36m--version\x1b\[0m                 Show the version and exit.\n"
     r"  \x1b\[36m-h\x1b\[0m, \x1b\[36m--help\x1b\[0m"
     r"                Show this message and exit.\n"
 )
 
 
 default_debug_uncolored_log_start = (
```

### Comparing `click_extra-4.1.0/click_extra/tests/test_colorize.py` & `click_extra-4.2.0/click_extra/tests/test_colorize.py`

 * *Files 8% similar despite different names*

```diff
@@ -155,42 +155,46 @@
     def command4():
         echo("Run click-extra command #4...")
 
     color_cli1.section("Subcommand group 1", command1, command2)
     color_cli1.section("Extra commands", command3, command4)
 
     help_screen = (
-        r"\x1b\[94m\x1b\[1mUsage: \x1b\[0m\x1b\[97mcolor-cli1\x1b\[0m "
-        r"\x1b\[90m\[OPTIONS\]\x1b\[0m \x1b\[90mCOMMAND \[ARGS\]...\x1b\[0m\n\n"
-        r"\x1b\[94m\x1b\[1mGroup 1:\x1b\[0m\n"
-        r"  \x1b\[36m-a\x1b\[0m, \x1b\[36m--o1\x1b\[0m \x1b\[90mTEXT\x1b\[0m\n"
-        r"  \x1b\[36m-b\x1b\[0m, \x1b\[36m--o2\x1b\[0m \x1b\[90mTEXT\x1b\[0m\n\n"
-        r"\x1b\[94m\x1b\[1mGroup 2:\x1b\[0m\n"
-        r"  \x1b\[36m--o3\x1b\[0m \x1b\[90mMY_VAR\x1b\[0m\n"
-        r"  \x1b\[36m--o4\x1b\[0m \x1b\[90mTEXT\x1b\[0m\n\n"
-        r"\x1b\[94m\x1b\[1mOther options:\x1b\[0m\n"
-        r"  \x1b\[36m--test\x1b\[0m \x1b\[90mTEXT\x1b\[0m\n"
+        r"\x1b\[94m\x1b\[1m\x1b\[4mUsage: \x1b\[0m\x1b\[97mcolor-cli1\x1b\[0m "
+        r"\x1b\[36m\x1b\[2m\[OPTIONS\]\x1b\[0m"
+        r" \x1b\[36m\x1b\[2mCOMMAND \[ARGS\]...\x1b\[0m\n\n"
+        r"\x1b\[94m\x1b\[1m\x1b\[4mGroup 1:\x1b\[0m\n"
+        r"  \x1b\[36m-a\x1b\[0m, \x1b\[36m--o1\x1b\[0m \x1b\[36m\x1b\[2mTEXT\x1b\[0m\n"
+        r"  \x1b\[36m-b\x1b\[0m, \x1b\[36m--o2\x1b\[0m \x1b\[36m\x1b\[2mTEXT\x1b\[0m\n"
+        r"\n"
+        r"\x1b\[94m\x1b\[1m\x1b\[4mGroup 2:\x1b\[0m\n"
+        r"  \x1b\[36m--o3\x1b\[0m \x1b\[36m\x1b\[2mMY_VAR\x1b\[0m\n"
+        r"  \x1b\[36m--o4\x1b\[0m \x1b\[36m\x1b\[2mTEXT\x1b\[0m\n\n"
+        r"\x1b\[94m\x1b\[1m\x1b\[4mOther options:\x1b\[0m\n"
+        r"  \x1b\[36m--test\x1b\[0m \x1b\[36m\x1b\[2mTEXT\x1b\[0m\n"
         r"  \x1b\[36m-b\x1b\[0m, \x1b\[36m--boolean\x1b\[0m / \x1b\[36m\+B\x1b\[0m,"
         r" \x1b\[36m--no-boolean\x1b\[0m\n"
         r"                            "
-        r"\x1b\[90m\[default: \x1b\[0m\x1b\[35mno-boolean\x1b\[0m\x1b\[90m\]\x1b\[0m\n"
+        r"\x1b\[2m\[\x1b\[0m\x1b\[2mdefault: "
+        r"\x1b\[0m\x1b\[32m\x1b\[2m\x1b\[3mno-boolean\x1b\[0m\x1b\[2m\]\x1b\[0m\n"
         r"  \x1b\[36m/debug\x1b\[0m; \x1b\[36m/no-debug\x1b\[0m"
-        r"         \x1b\[90m\[default:"
-        r" \x1b\[0m\x1b\[35mno-debug\x1b\[0m\x1b\[90m\]\x1b\[0m\n"
+        r"         \x1b\[2m\[\x1b\[0m\x1b\[2mdefault:"
+        r" \x1b\[0m\x1b\[32m\x1b\[2m\x1b\[3mno-debug\x1b\[0m\x1b\[2m\]\x1b\[0m\n"
         r"  \x1b\[36m--shout\x1b\[0m / \x1b\[36m-S\x1b\[0m, \x1b\[36m--no-shout\x1b\[0m"
-        r"  \x1b\[90m\[default: \x1b\[0m\x1b\[35mno-shout\x1b\[0m\x1b\[90m\]\x1b\[0m\n"
+        r"  \x1b\[2m\[\x1b\[0m\x1b\[2mdefault: "
+        r"\x1b\[0m\x1b\[32m\x1b\[2m\x1b\[3mno-shout\x1b\[0m\x1b\[2m\]\x1b\[0m\n"
         rf"{default_options_colored_help}"
         r"\n"
-        r"\x1b\[94m\x1b\[1mSubcommand group 1:\x1b\[0m\n"
+        r"\x1b\[94m\x1b\[1m\x1b\[4mSubcommand group 1:\x1b\[0m\n"
         r"  \x1b\[36mcommand1\x1b\[0m  CLI description with extra"
-        r" \x1b\[90mMY_VAR\x1b\[0m reference.\n"
+        r" \x1b\[36m\x1b\[2mMY_VAR\x1b\[0m reference.\n"
         r"  \x1b\[36mcommand2\x1b\[0m\n\n"
-        r"\x1b\[94m\x1b\[1mExtra commands:\x1b\[0m\n"
+        r"\x1b\[94m\x1b\[1m\x1b\[4mExtra commands:\x1b\[0m\n"
         r"  \x1b\[36mcommand3\x1b\[0m\n"
-        r"  \x1b\[36mcommand4\x1b\[0m  \x1b\[33m\(Deprecated\)\x1b\[0m\n"
+        r"  \x1b\[36mcommand4\x1b\[0m  \x1b\[93m\x1b\[1m\(Deprecated\)\x1b\[0m\n"
     )
 
     result = invoke(color_cli1, "--help", color=True)
     assert result.exit_code == 0
     assert re.fullmatch(help_screen, result.output)
     assert not result.stderr
 
@@ -200,40 +204,40 @@
     assert not result.stderr
 
     # CLI main group is invoked before sub-command.
     result = invoke(color_cli1, "command1", "--help", color=True)
     assert result.exit_code == 0
     assert result.output == (
         "It works!\n"
-        "\x1b[94m\x1b[1mUsage: \x1b[0m\x1b[97mcolor-cli1 command1\x1b[0m"
-        " \x1b[90m[OPTIONS]\x1b[0m [\x1b[36mMY_ARG\x1b[0m]...\n"
+        "\x1b[94m\x1b[1m\x1b[4mUsage: \x1b[0m\x1b[97mcolor-cli1 command1\x1b[0m"
+        " \x1b[36m\x1b[2m[OPTIONS]\x1b[0m [\x1b[36mMY_ARG\x1b[0m]...\n"
         "\n"
         "  CLI description with extra MY_VAR reference.\n"
         "\n"
-        "\x1b[94m\x1b[1mPositional arguments:\x1b[0m\n"
+        "\x1b[94m\x1b[1m\x1b[4mPositional arguments:\x1b[0m\n"
         "  [\x1b[36mMY_ARG\x1b[0m]...  Argument supports help.\n"
         "\n"
-        "\x1b[94m\x1b[1mOptions:\x1b[0m\n"
+        "\x1b[94m\x1b[1m\x1b[4mOptions:\x1b[0m\n"
         "  \x1b[36m-h\x1b[0m, \x1b[36m--help\x1b[0m  Show this message and exit.\n"
     )
     assert not result.stderr
 
     # Standalone call to command: CLI main group is skipped.
     result = invoke(command1, "--help", color=True)
     assert result.exit_code == 0
     assert result.output == (
-        "\x1b[94m\x1b[1mUsage: \x1b[0m\x1b[97mcommand1\x1b[0m"
-        " \x1b[90m[OPTIONS]\x1b[0m [\x1b[36mMY_ARG\x1b[0m]...\n"
+        "\x1b[94m\x1b[1m\x1b[4mUsage: \x1b[0m\x1b[97mcommand1\x1b[0m"
+        " \x1b[36m\x1b[2m[OPTIONS]\x1b[0m [\x1b[36mMY_ARG\x1b[0m]...\n"
         "\n"
         "  CLI description with extra MY_VAR reference.\n"
         "\n"
-        "\x1b[94m\x1b[1mPositional arguments:\x1b[0m\n"
+        "\x1b[94m\x1b[1m\x1b[4mPositional arguments:\x1b[0m\n"
         "  [\x1b[36mMY_ARG\x1b[0m]...  Argument supports help.\n"
         "\n"
-        "\x1b[94m\x1b[1mOptions:\x1b[0m\n"
+        "\x1b[94m\x1b[1m\x1b[4mOptions:\x1b[0m\n"
         "  \x1b[36m-h\x1b[0m, \x1b[36m--help\x1b[0m  Show this message and exit.\n"
     )
     assert not result.stderr
 
     # Non-click-extra commands are not colorized nor have extra options.
     for cmd_id in ("command2", "command3"):
         result = invoke(color_cli1, cmd_id, "--help", color=True)
```

### Comparing `click_extra-4.1.0/click_extra/tests/test_commands.py` & `click_extra-4.2.0/click_extra/tests/test_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,19 +196,19 @@
 def test_subcommand_help(invoke, all_command_cli, cmd_id, param):
     result = invoke(all_command_cli, f"{cmd_id}-subcommand", param)
     assert result.exit_code == 0
     assert not result.stderr
 
     colored_help_header = (
         r"It works!\n"
-        rf"\x1b\[94m\x1b\[1mUsage: "
+        r"\x1b\[94m\x1b\[1m\x1b\[4mUsage: "
         rf"\x1b\[0m\x1b\[97mcommand-cli1 {cmd_id}-subcommand\x1b\[0m"
-        r" \x1b\[90m\[OPTIONS\]\x1b\[0m\n"
+        r" \x1b\[36m\x1b\[2m\[OPTIONS\]\x1b\[0m\n"
         r"\n"
-        r"\x1b\[94m\x1b\[1mOptions:\x1b\[0m\n"
+        r"\x1b\[94m\x1b\[1m\x1b\[4mOptions:\x1b\[0m\n"
     )
 
     # Extra sucommands are colored and include all extra options.
     if cmd_id == "click-extra":
         assert re.fullmatch(
             rf"{colored_help_header}{default_options_colored_help}",
             result.stdout,
```

### Comparing `click_extra-4.1.0/click_extra/tests/test_config.py` & `click_extra-4.2.0/click_extra/tests/test_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -476,15 +476,15 @@
             "dummy_flag = True\nmy_list = ('pip', 'npm', 'gem')\nint_parameter = 3\n"
         )
 
         # Debug level has been activated by configuration file.
         debug_log = rf"Load configuration matching {re.escape(str(conf_path))}\n"
         if is_url:
             debug_log += (
-                r'info: 127\.0\.0\.1 - - \[\S+ \S+\] '
+                r"info: 127\.0\.0\.1 - - \[\S+ \S+\] "
                 rf'"GET /{re.escape(conf_name)} HTTP/1\.1" 200 -\n'
             )
         debug_log += (
             r"debug: Set <Logger click_extra \(DEBUG\)> to DEBUG.\n"
             r"debug: Set <RootLogger root \(DEBUG\)> to DEBUG.\n"
             r"debug: \S+, version \S+\n"
             r"debug: {.*}\n"
```

### Comparing `click_extra-4.1.0/click_extra/tests/test_logging.py` & `click_extra-4.2.0/click_extra/tests/test_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             r"\x1b\[34mdebug\x1b\[0m: Set <RootLogger root \(DEBUG\)> to DEBUG.\n"
             r"\x1b\[34mdebug\x1b\[0m: my random message.\n"
             r"\x1b\[34mdebug\x1b\[0m: my debug message.\n"
         ),
         r"info: my info message.\n",
         r"\x1b\[33mwarning\x1b\[0m: my warning message.\n",
         r"\x1b\[31merror\x1b\[0m: my error message.\n",
-        r"\x1b\[31mcritical\x1b\[0m: my critical message.\n",
+        r"\x1b\[31m\x1b\[1mcritical\x1b\[0m: my critical message.\n",
     )
     level_index = {index: level for level, index in enumerate(LOG_LEVELS)}[level]
     log_records = r"".join(messages[-level_index - 1 :])
 
     if level == "DEBUG":
         log_records += default_debug_colored_log_end
     assert re.fullmatch(log_records, result.stderr)
@@ -154,16 +154,15 @@
 
 
 @pytest.mark.parametrize(
     "logger_param", (logging.getLogger("awesome_app"), "awesome_app")
 )
 @pytest.mark.parametrize("params", (("--verbosity", "DEBUG"), None))
 def test_custom_logger_param(invoke, logger_param, params):
-    """Passing a logger instance or name to the ``default_logger`` parameter works.
-    """
+    """Passing a logger instance or name to the ``default_logger`` parameter works."""
 
     @click.command
     @verbosity_option(default_logger=logger_param)
     def awesome_app():
         echo("Starting Awesome App...")
         logging.getLogger("awesome_app").debug("Awesome App has started.")
```

### Comparing `click_extra-4.1.0/click_extra/tests/test_parameters.py` & `click_extra-4.2.0/click_extra/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.1.0/click_extra/tests/test_platforms.py` & `click_extra-4.2.0/click_extra/tests/test_platforms.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.1.0/click_extra/tests/test_pygments.py` & `click_extra-4.2.0/click_extra/tests/test_pygments.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,17 +21,19 @@
 from operator import itemgetter
 from pathlib import Path
 from importlib import metadata
 
 from boltons.strutils import camel2under
 from boltons.typeutils import issubclass
 from pygments.filter import Filter
+from pygments.filters import get_filter_by_name
 from pygments.formatter import Formatter
-from pygments.lexers import find_lexer_class_by_name
-from pygments.style import Style
+from pygments.formatters import get_formatter_by_name
+from pygments.lexer import Lexer
+from pygments.lexers import find_lexer_class_by_name, get_lexer_by_name
 import requests
 
 if sys.version_info >= (3, 11):
     import tomllib
 else:
     import tomli as tomllib  # type: ignore[import]
 
@@ -139,14 +141,24 @@
     assert lexer_candidates
     lexer_classes = {find_lexer_class_by_name(alias) for alias in lexer_candidates}
     # We cannot test for strict equality yet, as some ANSI-ready lexers do not
     # have any test artifacts producing ``Generic.Output`` tokens.
     assert lexer_classes.issubset(collect_session_lexers())
 
 
+def collect_classes(klass, prefix="Ansi"):
+    """Returns all classes defined in ``click_extra.pygments`` that are a
+    subclass of ``klass``, and whose name starts with the provided ``prefix``."""
+    klasses = {}
+    for name, var in extra_pygments.__dict__.items():
+        if issubclass(var, klass) and name.startswith(prefix):
+            klasses[name] = var
+    return klasses
+
+
 def get_pyproject_section(*section_path: str) -> dict[str, str]:
     """Descends into the TOML tree of ``pyproject.toml`` to reach the value specified by
     ``section_path``."""
     toml_path = PROJECT_ROOT.joinpath("pyproject.toml").resolve()
     section: dict = tomllib.loads(toml_path.read_text(encoding="utf-8"))
     for section_id in section_path:
         section = section[section_id]
@@ -155,15 +167,15 @@
 
 def check_entry_points(entry_points: dict[str, str], *section_path: str) -> None:
     entry_points = dict(sorted(entry_points.items(), key=itemgetter(0)))
     project_entry_points = get_pyproject_section(*section_path)
     assert project_entry_points == entry_points
 
 
-def test_registered_lexers():
+def test_lexer_entry_points():
     entry_points = {}
     for lexer in collect_session_lexers():
         # Check an ANSI lexer variant is available for import from Click Extra.
         ansi_lexer_id = f"Ansi{lexer.__name__}"
         assert ansi_lexer_id in extra_pygments.__dict__
 
         # Transform ANSI lexer class ID into entry point ID.
@@ -174,46 +186,47 @@
         # Generate the lexer entry point.
         class_path = f"click_extra.pygments:{ansi_lexer_id}"
         entry_points[entry_id] = class_path
 
     check_entry_points(entry_points, "tool", "poetry", "plugins", "pygments.lexers")
 
 
-def collect_class_names(klass, prefix="Ansi"):
-    """Returns the name of all classes defined in ``click_extra.pygments`` that are a
-    subclass of ``klass``, and whose name starts with the provided ``prefix``."""
-    for name, var in extra_pygments.__dict__.items():
-        if issubclass(var, klass) and name.startswith(prefix):
-            yield name
-
-
-def test_registered_filters():
+def test_filter_entry_points():
     entry_points = {}
-    for name in collect_class_names(Filter):
+    for name in collect_classes(Filter):
         entry_id = camel2under(name).replace("_", "-")
         entry_points[entry_id] = f"click_extra.pygments:{name}"
 
     check_entry_points(entry_points, "tool", "poetry", "plugins", "pygments.filters")
 
 
-def test_registered_formatters():
+def test_formatter_entry_points():
     entry_points = {}
-    for name in collect_class_names(Formatter):
+    for name in collect_classes(Formatter):
         entry_id = camel2under(name).replace("_", "-")
         entry_points[entry_id] = f"click_extra.pygments:{name}"
 
     check_entry_points(entry_points, "tool", "poetry", "plugins", "pygments.formatters")
 
 
-def test_registered_styles():
-    entry_points = {}
-    for name in collect_class_names(Style):
+def test_registered_lexers():
+    for klass in collect_classes(Lexer).values():
+        for alias in klass.aliases:
+            get_lexer_by_name(alias)
+
+
+def test_registered_filters():
+    for name in collect_classes(Filter):
         entry_id = camel2under(name).replace("_", "-")
-        entry_points[entry_id] = f"click_extra.pygments:{name}"
+        get_filter_by_name(entry_id)
 
-    check_entry_points(entry_points, "tool", "poetry", "plugins", "pygments.styles")
+
+def test_registered_formatters():
+    for klass in collect_classes(Formatter).values():
+        for alias in klass.aliases:
+            get_formatter_by_name(alias)
 
 
 def test_ansi_lexers_doc():
     doc_content = PROJECT_ROOT.joinpath("docs/pygments.md").read_text()
     for lexer in collect_session_lexers():
         assert lexer.__name__ in doc_content
```

### Comparing `click_extra-4.1.0/click_extra/tests/test_run.py` & `click_extra-4.2.0/click_extra/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.1.0/click_extra/tests/test_tabulate.py` & `click_extra-4.2.0/click_extra/tests/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.1.0/click_extra/tests/test_telemetry.py` & `click_extra-4.2.0/click_extra/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.1.0/click_extra/tests/test_timer.py` & `click_extra-4.2.0/click_extra/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.1.0/click_extra/tests/test_version.py` & `click_extra-4.2.0/click_extra/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.1.0/click_extra/timer.py` & `click_extra-4.2.0/click_extra/timer.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.1.0/click_extra/version.py` & `click_extra-4.2.0/click_extra/version.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.1.0/pyproject.toml` & `click_extra-4.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 # Docs: https://python-poetry.org/docs/pyproject/
 name = "click-extra"
-version = "4.1.0"
+version = "4.2.0"
 description = "🌈 Extra colorization and configuration loading for Click."
 license = 'GPL-2.0-or-later'
 authors = ["Kevin Deldycke <kevin@deldycke.com>"]
 readme = "readme.md"
 homepage = 'https://github.com/kdeldycke/click-extra'
 repository = 'https://github.com/kdeldycke/click-extra'
 documentation = 'https://kdeldycke.github.io/click-extra'
@@ -70,23 +70,24 @@
 python = "^3.8"
 # XXX boltons.ecoutils 23.0.0 breaks PDB interactive sessions in pytest.
 # Investigation of the root cause is being discussed upstream at:
 # https://github.com/mahmoud/boltons/issues/334
 boltons = "^23.0.0"
 # Click 8.1 is the first version to support ``params=`` in ``@command``.
 click = "^8.1"
-cloup = "^2.0.0.post1"
+# Cloup 2.1.0 introduced colorization of subcommand aliases.
+cloup = "^2.1.0"
 commentjson = "^0.9.0"
-furo = "^2023.03.27"
 mergedeep = "^1.3.4"
 # Pallets-Sphinx-Themes 2.1.0 is the first version rendering ``.. sourcecode:: shell-session`` code-blocks.
 Pallets-Sphinx-Themes = "^2.1.0"
 # Pygments 2.14.0 is the first version with ``lexers.algebra.GAPConsoleLexer`` that is referenced in our code.
 pygments = "^2.14"
-pygments-ansi-color = "^0.2.0"
+# pygments-ansi-color 0.3.0 is the first version to set the default theme of ANSI colors.
+pygments-ansi-color = "^0.3.0"
 pyyaml = "^6.0.0"
 # regex is required for case-insensitive matches in Unicode.
 # v2023.3.22 is the first to drop Python 3.7.
 regex = "^2023.3.22"
 # requests 2.28.2 is the first version to support charset_normalizer 3.x.
 requests = "^2.28.2"
 # Sphinx 6 is the first version to drop Python 3.7.
@@ -96,14 +97,15 @@
 tomli = { version = "^2.0.1", python = "< 3.11" }
 wcmatch = "^8.4.1"
 xmltodict = "^0.13.0"
 
 [tool.poetry.group.dev.dependencies]
 bump2version = "^1.0.1"
 coverage = { extras = ["toml"], version = "^7.2.3" }
+furo = "^2023.05.20"
 mypy = "^1.2.0"
 myst-parser = "^1.0.0"
 pytest = "^7.3.1"
 # More pytest plugins at: https://docs.pytest.org/en/latest/reference/plugin_list.html
 pytest-cases = "^3.6.14"
 pytest-cov = "^4.0.0"
 pytest-httpserver = "^1.0.6"
@@ -118,15 +120,15 @@
 types-PyYAML = "^6.0.12.9"
 types-regex = "^2023.3.23.1"
 types-requests = "^2.28.11.17"
 types-tabulate = "^0.9.0.2"
 types-xmltodict = "^0.13.0.2"
 
 [tool.poetry.plugins."pygments.lexers"]
-# The name of the entrypoint values doesn’t really matter, Pygments extracts required metadata from the class definition.
+# The name of the entrypoint value doesn’t really matter, Pygments extracts required metadata from the class definition.
 # Source: https://pygments.org/docs/plugins/#defining-plugins-through-entrypoints
 ansi-bash-session = "click_extra.pygments:AnsiBashSessionLexer"
 ansi-dylan-console = "click_extra.pygments:AnsiDylanConsoleLexer"
 ansi-elixir-console = "click_extra.pygments:AnsiElixirConsoleLexer"
 ansi-erlang-shell = "click_extra.pygments:AnsiErlangShellLexer"
 ansi-gap-console = "click_extra.pygments:AnsiGAPConsoleLexer"
 ansi-julia-console = "click_extra.pygments:AnsiJuliaConsoleLexer"
@@ -144,17 +146,14 @@
 
 [tool.poetry.plugins."pygments.filters"]
 ansi-filter = "click_extra.pygments:AnsiFilter"
 
 [tool.poetry.plugins."pygments.formatters"]
 ansi-html-formatter = "click_extra.pygments:AnsiHtmlFormatter"
 
-[tool.poetry.plugins."pygments.styles"]
-ansi-click-extra-furo-style = "click_extra.pygments:AnsiClickExtraFuroStyle"
-
 [tool.mypy]
 warn_unused_configs = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_return_any = true
 warn_unreachable = true
 pretty = true
```

### Comparing `click_extra-4.1.0/readme.md` & `click_extra-4.2.0/readme.md`

 * *Files identical despite different names*

### Comparing `click_extra-4.1.0/PKG-INFO` & `click_extra-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-extra
-Version: 4.1.0
+Version: 4.2.0
 Summary: 🌈 Extra colorization and configuration loading for Click.
 Home-page: https://github.com/kdeldycke/click-extra
 License: GPL-2.0-or-later
 Keywords: ansi-colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-tabulate,sphinx,terminal,toml,xml,yaml
 Author: Kevin Deldycke
 Author-email: kevin@deldycke.com
 Requires-Python: >=3.8,<4.0
@@ -38,20 +38,19 @@
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: Topic :: Text Processing :: Markup :: reStructuredText
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: Pallets-Sphinx-Themes (>=2.1.0,<3.0.0)
 Requires-Dist: boltons (>=23.0.0,<24.0.0)
 Requires-Dist: click (>=8.1,<9.0)
-Requires-Dist: cloup (>=2.0.0.post1,<3.0.0)
+Requires-Dist: cloup (>=2.1.0,<3.0.0)
 Requires-Dist: commentjson (>=0.9.0,<0.10.0)
-Requires-Dist: furo (>=2023.03.27,<2024.0.0)
 Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
 Requires-Dist: pygments (>=2.14,<3.0)
-Requires-Dist: pygments-ansi-color (>=0.2.0,<0.3.0)
+Requires-Dist: pygments-ansi-color (>=0.3.0,<0.4.0)
 Requires-Dist: pyyaml (>=6.0.0,<7.0.0)
 Requires-Dist: regex (>=2023.3.22,<2024.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: sphinx (>=6,<7)
 Requires-Dist: tabulate[widechars] (>=0.9,<0.10)
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
 Requires-Dist: wcmatch (>=8.4.1,<9.0.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: click-extra Version: 4.1.0 Summary: ð Extra
+Metadata-Version: 2.1 Name: click-extra Version: 4.2.0 Summary: ð Extra
 colorization and configuration loading for Click. Home-page: https://
 github.com/kdeldycke/click-extra License: GPL-2.0-or-later Keywords: ansi-
 colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-
 tabulate,sphinx,terminal,toml,xml,yaml Author: Kevin Deldycke Author-email:
 kevin@deldycke.com Requires-Python: >=3.8,<4.0 Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Environment :: Plugins Classifier: Framework :: Pytest Classifier: Framework ::
@@ -21,28 +21,27 @@
 Classifier: Topic :: System :: Shells Classifier: Topic :: Terminals
 Classifier: Topic :: Text Processing :: Filters Classifier: Topic :: Text
 Processing :: Markup :: HTML Classifier: Topic :: Text Processing :: Markup ::
 Markdown Classifier: Topic :: Text Processing :: Markup :: XML Classifier:
 Topic :: Text Processing :: Markup :: reStructuredText Classifier: Topic ::
 Utilities Classifier: Typing :: Typed Requires-Dist: Pallets-Sphinx-Themes
 (>=2.1.0,<3.0.0) Requires-Dist: boltons (>=23.0.0,<24.0.0) Requires-Dist: click
-(>=8.1,<9.0) Requires-Dist: cloup (>=2.0.0.post1,<3.0.0) Requires-Dist:
-commentjson (>=0.9.0,<0.10.0) Requires-Dist: furo (>=2023.03.27,<2024.0.0)
-Requires-Dist: mergedeep (>=1.3.4,<2.0.0) Requires-Dist: pygments (>=2.14,<3.0)
-Requires-Dist: pygments-ansi-color (>=0.2.0,<0.3.0) Requires-Dist: pyyaml
-(>=6.0.0,<7.0.0) Requires-Dist: regex (>=2023.3.22,<2024.0.0) Requires-Dist:
-requests (>=2.28.2,<3.0.0) Requires-Dist: sphinx (>=6,<7) Requires-Dist:
-tabulate[widechars] (>=0.9,<0.10) Requires-Dist: tomli (>=2.0.1,<3.0.0) ;
-python_version < "3.11" Requires-Dist: wcmatch (>=8.4.1,<9.0.0) Requires-Dist:
-xmltodict (>=0.13.0,<0.14.0) Project-URL: Changelog, https://
-kdeldycke.github.io/click-extra/changelog.html Project-URL: Documentation,
-https://kdeldycke.github.io/click-extra Project-URL: Funding, https://
-github.com/sponsors/kdeldycke Project-URL: Issues, https://github.com/
-kdeldycke/click-extra/issues Project-URL: Repository, https://github.com/
-kdeldycke/click-extra Description-Content-Type: text/markdown
+(>=8.1,<9.0) Requires-Dist: cloup (>=2.1.0,<3.0.0) Requires-Dist: commentjson
+(>=0.9.0,<0.10.0) Requires-Dist: mergedeep (>=1.3.4,<2.0.0) Requires-Dist:
+pygments (>=2.14,<3.0) Requires-Dist: pygments-ansi-color (>=0.3.0,<0.4.0)
+Requires-Dist: pyyaml (>=6.0.0,<7.0.0) Requires-Dist: regex
+(>=2023.3.22,<2024.0.0) Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-
+Dist: sphinx (>=6,<7) Requires-Dist: tabulate[widechars] (>=0.9,<0.10)
+Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11" Requires-Dist:
+wcmatch (>=8.4.1,<9.0.0) Requires-Dist: xmltodict (>=0.13.0,<0.14.0) Project-
+URL: Changelog, https://kdeldycke.github.io/click-extra/changelog.html Project-
+URL: Documentation, https://kdeldycke.github.io/click-extra Project-URL:
+Funding, https://github.com/sponsors/kdeldycke Project-URL: Issues, https://
+github.com/kdeldycke/click-extra/issues Project-URL: Repository, https://
+github.com/kdeldycke/click-extra Description-Content-Type: text/markdown
                                  [Click_Extra]
 [![Last release](https://img.shields.io/pypi/v/click-extra.svg)](https://
 pypi.python.org/pypi/click-extra) [![Python versions](https://img.shields.io/
 pypi/pyversions/click-extra.svg)](https://pypi.python.org/pypi/click-extra) [!
 [Unittests status](https://github.com/kdeldycke/click-extra/actions/workflows/
 tests.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/click-extra/
 actions/workflows/tests.yaml?query=branch%3Amain) [![Documentation status]
```

