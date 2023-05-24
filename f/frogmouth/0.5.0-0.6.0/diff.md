# Comparing `tmp/frogmouth-0.5.0.tar.gz` & `tmp/frogmouth-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frogmouth-0.5.0.tar", max compression
+gzip compressed data, was "frogmouth-0.6.0.tar", max compression
```

## Comparing `frogmouth-0.5.0.tar` & `frogmouth-0.6.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1072 2023-04-27 14:46:52.801782 frogmouth-0.5.0/LICENSE
--rw-r--r--   0        0        0     2752 2023-04-30 07:26:36.700670 frogmouth-0.5.0/README.md
--rw-r--r--   0        0        0      283 2023-05-09 08:04:58.867459 frogmouth-0.5.0/frogmouth/__init__.py
--rw-r--r--   0        0        0      112 2023-04-27 14:46:52.802125 frogmouth-0.5.0/frogmouth/__main__.py
--rw-r--r--   0        0        0       74 2023-04-27 14:46:52.802222 frogmouth-0.5.0/frogmouth/app/__init__.py
--rw-r--r--   0        0        0     2070 2023-04-30 11:10:42.375933 frogmouth-0.5.0/frogmouth/app/app.py
--rw-r--r--   0        0        0      395 2023-04-27 14:46:52.802403 frogmouth-0.5.0/frogmouth/data/__init__.py
--rw-r--r--   0        0        0     1639 2023-04-27 14:46:52.802497 frogmouth-0.5.0/frogmouth/data/bookmarks.py
--rw-r--r--   0        0        0     2270 2023-05-09 08:04:58.867587 frogmouth-0.5.0/frogmouth/data/config.py
--rw-r--r--   0        0        0      582 2023-04-27 14:46:52.802650 frogmouth-0.5.0/frogmouth/data/data_directory.py
--rw-r--r--   0        0        0     1370 2023-04-27 14:46:52.802714 frogmouth-0.5.0/frogmouth/data/history.py
--rw-r--r--   0        0        0      354 2023-04-27 14:46:52.802828 frogmouth-0.5.0/frogmouth/dialogs/__init__.py
--rw-r--r--   0        0        0      565 2023-04-28 13:52:42.406602 frogmouth-0.5.0/frogmouth/dialogs/error.py
--rw-r--r--   0        0        0     4539 2023-05-09 08:04:58.868315 frogmouth-0.5.0/frogmouth/dialogs/help_dialog.py
--rw-r--r--   0        0        0      269 2023-04-27 14:55:30.387330 frogmouth-0.5.0/frogmouth/dialogs/information.py
--rw-r--r--   0        0        0     2544 2023-05-09 08:04:58.868437 frogmouth-0.5.0/frogmouth/dialogs/input_dialog.py
--rw-r--r--   0        0        0     2168 2023-04-29 20:35:07.295162 frogmouth-0.5.0/frogmouth/dialogs/text_dialog.py
--rw-r--r--   0        0        0     3602 2023-05-03 09:31:33.036152 frogmouth-0.5.0/frogmouth/dialogs/yes_no_dialog.py
--rw-r--r--   0        0        0       83 2023-04-27 14:46:52.803485 frogmouth-0.5.0/frogmouth/screens/__init__.py
--rw-r--r--   0        0        0    18617 2023-05-09 08:04:58.868627 frogmouth-0.5.0/frogmouth/screens/main.py
--rw-r--r--   0        0        0      327 2023-04-27 14:46:52.803762 frogmouth-0.5.0/frogmouth/utility/__init__.py
--rw-r--r--   0        0        0      894 2023-04-28 13:00:47.734733 frogmouth-0.5.0/frogmouth/utility/advertising.py
--rw-r--r--   0        0        0     4237 2023-04-27 14:46:52.803923 frogmouth-0.5.0/frogmouth/utility/forge.py
--rw-r--r--   0        0        0     1206 2023-05-09 08:04:58.868785 frogmouth-0.5.0/frogmouth/utility/type_tests.py
--rw-r--r--   0        0        0      184 2023-04-27 14:46:52.804110 frogmouth-0.5.0/frogmouth/widgets/__init__.py
--rw-r--r--   0        0        0     6015 2023-05-09 08:04:58.868929 frogmouth-0.5.0/frogmouth/widgets/navigation.py
--rw-r--r--   0        0        0      298 2023-04-27 14:46:52.804311 frogmouth-0.5.0/frogmouth/widgets/navigation_panes/__init__.py
--rw-r--r--   0        0        0     5633 2023-05-03 09:31:33.037203 frogmouth-0.5.0/frogmouth/widgets/navigation_panes/bookmarks.py
--rw-r--r--   0        0        0     5685 2023-05-09 08:04:58.869061 frogmouth-0.5.0/frogmouth/widgets/navigation_panes/history.py
--rw-r--r--   0        0        0     3071 2023-05-09 08:04:58.869180 frogmouth-0.5.0/frogmouth/widgets/navigation_panes/local_files.py
--rw-r--r--   0        0        0      665 2023-05-03 09:31:33.037312 frogmouth-0.5.0/frogmouth/widgets/navigation_panes/navigation_pane.py
--rw-r--r--   0        0        0     2341 2023-05-09 08:04:58.869286 frogmouth-0.5.0/frogmouth/widgets/navigation_panes/table_of_contents.py
--rw-r--r--   0        0        0    11931 2023-05-09 08:04:58.869453 frogmouth-0.5.0/frogmouth/widgets/omnibox.py
--rw-r--r--   0        0        0    10750 2023-05-09 08:04:58.872361 frogmouth-0.5.0/frogmouth/widgets/viewer.py
--rw-r--r--   0        0        0     1468 2023-05-09 08:04:58.873191 frogmouth-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4331 1970-01-01 00:00:00.000000 frogmouth-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-27 14:46:52.801782 frogmouth-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2752 2023-04-30 07:26:36.700670 frogmouth-0.6.0/README.md
+-rw-r--r--   0        0        0      283 2023-05-24 09:22:14.385143 frogmouth-0.6.0/frogmouth/__init__.py
+-rw-r--r--   0        0        0      112 2023-04-27 14:46:52.802125 frogmouth-0.6.0/frogmouth/__main__.py
+-rw-r--r--   0        0        0       74 2023-04-27 14:46:52.802222 frogmouth-0.6.0/frogmouth/app/__init__.py
+-rw-r--r--   0        0        0     2070 2023-04-30 11:10:42.375933 frogmouth-0.6.0/frogmouth/app/app.py
+-rw-r--r--   0        0        0      395 2023-04-27 14:46:52.802403 frogmouth-0.6.0/frogmouth/data/__init__.py
+-rw-r--r--   0        0        0     1639 2023-04-27 14:46:52.802497 frogmouth-0.6.0/frogmouth/data/bookmarks.py
+-rw-r--r--   0        0        0     2270 2023-05-09 08:04:58.867587 frogmouth-0.6.0/frogmouth/data/config.py
+-rw-r--r--   0        0        0      582 2023-04-27 14:46:52.802650 frogmouth-0.6.0/frogmouth/data/data_directory.py
+-rw-r--r--   0        0        0     1370 2023-04-27 14:46:52.802714 frogmouth-0.6.0/frogmouth/data/history.py
+-rw-r--r--   0        0        0      354 2023-04-27 14:46:52.802828 frogmouth-0.6.0/frogmouth/dialogs/__init__.py
+-rw-r--r--   0        0        0      565 2023-04-28 13:52:42.406602 frogmouth-0.6.0/frogmouth/dialogs/error.py
+-rw-r--r--   0        0        0     4616 2023-05-18 13:41:34.483482 frogmouth-0.6.0/frogmouth/dialogs/help_dialog.py
+-rw-r--r--   0        0        0      269 2023-04-27 14:55:30.387330 frogmouth-0.6.0/frogmouth/dialogs/information.py
+-rw-r--r--   0        0        0     2544 2023-05-09 08:04:58.868437 frogmouth-0.6.0/frogmouth/dialogs/input_dialog.py
+-rw-r--r--   0        0        0     2168 2023-04-29 20:35:07.295162 frogmouth-0.6.0/frogmouth/dialogs/text_dialog.py
+-rw-r--r--   0        0        0     3602 2023-05-03 09:31:33.036152 frogmouth-0.6.0/frogmouth/dialogs/yes_no_dialog.py
+-rw-r--r--   0        0        0       83 2023-04-27 14:46:52.803485 frogmouth-0.6.0/frogmouth/screens/__init__.py
+-rw-r--r--   0        0        0    18949 2023-05-18 13:41:34.483651 frogmouth-0.6.0/frogmouth/screens/main.py
+-rw-r--r--   0        0        0      402 2023-05-18 13:41:34.484301 frogmouth-0.6.0/frogmouth/utility/__init__.py
+-rw-r--r--   0        0        0      894 2023-04-28 13:00:47.734733 frogmouth-0.6.0/frogmouth/utility/advertising.py
+-rw-r--r--   0        0        0     5135 2023-05-18 13:41:34.484397 frogmouth-0.6.0/frogmouth/utility/forge.py
+-rw-r--r--   0        0        0     1206 2023-05-09 08:04:58.868785 frogmouth-0.6.0/frogmouth/utility/type_tests.py
+-rw-r--r--   0        0        0      184 2023-04-27 14:46:52.804110 frogmouth-0.6.0/frogmouth/widgets/__init__.py
+-rw-r--r--   0        0        0     6015 2023-05-09 08:04:58.868929 frogmouth-0.6.0/frogmouth/widgets/navigation.py
+-rw-r--r--   0        0        0      298 2023-04-27 14:46:52.804311 frogmouth-0.6.0/frogmouth/widgets/navigation_panes/__init__.py
+-rw-r--r--   0        0        0     5633 2023-05-03 09:31:33.037203 frogmouth-0.6.0/frogmouth/widgets/navigation_panes/bookmarks.py
+-rw-r--r--   0        0        0     5685 2023-05-09 08:04:58.869061 frogmouth-0.6.0/frogmouth/widgets/navigation_panes/history.py
+-rw-r--r--   0        0        0     3071 2023-05-09 08:04:58.869180 frogmouth-0.6.0/frogmouth/widgets/navigation_panes/local_files.py
+-rw-r--r--   0        0        0      665 2023-05-03 09:31:33.037312 frogmouth-0.6.0/frogmouth/widgets/navigation_panes/navigation_pane.py
+-rw-r--r--   0        0        0     2341 2023-05-09 08:04:58.869286 frogmouth-0.6.0/frogmouth/widgets/navigation_panes/table_of_contents.py
+-rw-r--r--   0        0        0    12260 2023-05-18 13:41:34.484532 frogmouth-0.6.0/frogmouth/widgets/omnibox.py
+-rw-r--r--   0        0        0    10750 2023-05-09 08:04:58.872361 frogmouth-0.6.0/frogmouth/widgets/viewer.py
+-rw-r--r--   0        0        0     1470 2023-05-24 09:22:14.385940 frogmouth-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 frogmouth-0.6.0/PKG-INFO
```

### Comparing `frogmouth-0.5.0/LICENSE` & `frogmouth-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frogmouth-0.5.0/README.md` & `frogmouth-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `frogmouth-0.5.0/frogmouth/app/app.py` & `frogmouth-0.6.0/frogmouth/app/app.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.5.0/frogmouth/data/bookmarks.py` & `frogmouth-0.6.0/frogmouth/data/bookmarks.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.5.0/frogmouth/data/config.py` & `frogmouth-0.6.0/frogmouth/data/config.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.5.0/frogmouth/data/data_directory.py` & `frogmouth-0.6.0/frogmouth/data/data_directory.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.5.0/frogmouth/data/history.py` & `frogmouth-0.6.0/frogmouth/data/history.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.5.0/frogmouth/dialogs/error.py` & `frogmouth-0.6.0/frogmouth/dialogs/error.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.5.0/frogmouth/dialogs/help_dialog.py` & `frogmouth-0.6.0/frogmouth/dialogs/help_dialog.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 Press `/` or click the address bar, then enter any of the following commands:
 
 | Command | Aliases | Arguments | Command |
 | -- | -- | -- | -- |
 | `about` | `a` | | Show details about the application |
 | `bookmarks` | `b`, `bm` | | Show the bookmarks list |
 | `bitbucket` | `bb` | `<repo-info>` | View a file on BitBucket (see below) |
+| `codeberg` | `cb` | `<repo-info>` | View a file on Codceberg (see below) |
 | `changelog` | `cl` | | View the Frogmouth ChangeLog |
 | `chdir` | `cd` | `<dir>` | Switch the local file browser to a new directory |
 | `contents` | `c`, `toc` | | Show the table of contents for the document |
 | `discord` | | | Visit the Textualize Discord server |
 | `github` | `gh` | `<repo-info>` | View a file on GitHub (see below) |
 | `gitlab` | `gl` | `<repo-info>` | View a file on GitLab (see below) |
 | `help` | `?` | | Show this document |
```

### Comparing `frogmouth-0.5.0/frogmouth/dialogs/input_dialog.py` & `frogmouth-0.6.0/frogmouth/dialogs/input_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.5.0/frogmouth/dialogs/text_dialog.py` & `frogmouth-0.6.0/frogmouth/dialogs/text_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.5.0/frogmouth/dialogs/yes_no_dialog.py` & `frogmouth-0.6.0/frogmouth/dialogs/yes_no_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.5.0/frogmouth/screens/main.py` & `frogmouth-0.6.0/frogmouth/screens/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from textual.widgets import Footer, Markdown
 
 from .. import __version__
 from ..data import load_config, load_history, save_config, save_history
 from ..dialogs import ErrorDialog, HelpDialog, InformationDialog, InputDialog
 from ..utility import (
     build_raw_bitbucket_url,
+    build_raw_codeberg_url,
     build_raw_github_url,
     build_raw_gitlab_url,
     is_likely_url,
     maybe_markdown,
 )
 from ..utility.advertising import (
     APPLICATION_TITLE,
@@ -271,14 +272,22 @@
         """Handle a BitBucket shortcut command.
 
         Args:
             event: The BitBucket shortcut command event to handle.
         """
         await self._from_forge("BitBucket", event, build_raw_bitbucket_url)
 
+    async def on_omnibox_codeberg_command(self, event: Omnibox.CodebergCommand) -> None:
+        """Handle a Codeberg shortcut command.
+
+        Args:
+            event: The Codeberg shortcut command event to handle.
+        """
+        await self._from_forge("Codeberg", event, build_raw_codeberg_url)
+
     def on_omnibox_about_command(self) -> None:
         """Handle being asked to show the about dialog."""
         self.action_about()
 
     def on_omnibox_help_command(self) -> None:
         """Handle being asked to show the help document."""
         self.action_help()
```

### Comparing `frogmouth-0.5.0/frogmouth/utility/advertising.py` & `frogmouth-0.6.0/frogmouth/utility/advertising.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.5.0/frogmouth/utility/forge.py` & `frogmouth-0.6.0/frogmouth/utility/forge.py`

 * *Files 8% similar despite different names*

```diff
@@ -139,7 +139,38 @@
     return await build_raw_forge_url(
         "https://bitbucket.org/{owner}/{repository}/raw/{branch}/{file}",
         owner,
         repository,
         branch,
         desired_file,
     )
+
+
+async def build_raw_codeberg_url(
+    owner: str,
+    repository: str,
+    branch: str | None = None,
+    desired_file: str | None = None,
+) -> URL | None:
+    """Attempt to get the Codeberg raw URL for the given file.
+
+    Args:
+        owner: The owner of the repository to look in.
+        repository: The repository to look in.
+        branch: The optional branch to look in.
+        desired_file: Optional name of the file to go looking for.
+
+    Returns:
+        The URL for the file, or `None` if none could be guessed.
+
+    If the branch isn't supplied then `main` and `master` will be tested.
+
+    If the target file isn't supplied it's assumed that `README.md` is the
+    target.
+    """
+    return await build_raw_forge_url(
+        "https://codeberg.org/{owner}/{repository}/raw//branch/{branch}/{file}",
+        owner,
+        repository,
+        branch,
+        desired_file,
+    )
```

### Comparing `frogmouth-0.5.0/frogmouth/utility/type_tests.py` & `frogmouth-0.6.0/frogmouth/utility/type_tests.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.5.0/frogmouth/widgets/navigation.py` & `frogmouth-0.6.0/frogmouth/widgets/navigation.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.5.0/frogmouth/widgets/navigation_panes/bookmarks.py` & `frogmouth-0.6.0/frogmouth/widgets/navigation_panes/bookmarks.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.5.0/frogmouth/widgets/navigation_panes/history.py` & `frogmouth-0.6.0/frogmouth/widgets/navigation_panes/history.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.5.0/frogmouth/widgets/navigation_panes/local_files.py` & `frogmouth-0.6.0/frogmouth/widgets/navigation_panes/local_files.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.5.0/frogmouth/widgets/navigation_panes/navigation_pane.py` & `frogmouth-0.6.0/frogmouth/widgets/navigation_panes/navigation_pane.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.5.0/frogmouth/widgets/navigation_panes/table_of_contents.py` & `frogmouth-0.6.0/frogmouth/widgets/navigation_panes/table_of_contents.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.5.0/frogmouth/widgets/omnibox.py` & `frogmouth-0.6.0/frogmouth/widgets/omnibox.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
     _ALIASES: dict[str, str] = {
         "a": "about",
         "b": "bookmarks",
         "bm": "bookmarks",
         "bb": "bitbucket",
         "c": "contents",
+        "cb": "codeberg",
         "cd": "chdir",
         "cl": "changelog",
         "gh": "github",
         "gl": "gitlab",
         "h": "history",
         "l": "local",
         "obs": "obsidian",
@@ -328,14 +329,25 @@
         """The BitBucket command.
 
         Args:
             tail: The tail of the command.
         """
         self._forge_quick_look(self.BitBucketCommand, tail)
 
+    class CodebergCommand(ForgeCommand):
+        """The Codeberg quick load command."""
+
+    def command_codeberg(self, tail: str) -> None:
+        """The Codeberg command.
+
+        Args:
+            tail: The tail of the command.
+        """
+        self._forge_quick_look(self.CodebergCommand, tail)
+
     def command_discord(self, _: str) -> None:
         """The command to visit the Textualize discord server."""
         open_url(DISCORD)
 
     def command_changelog(self, _: str) -> None:
         """The command to show the application's own ChangeLog"""
         self.command_github(f"{ORGANISATION_NAME}/{PACKAGE_NAME} ChangeLog.md")
```

### Comparing `frogmouth-0.5.0/frogmouth/widgets/viewer.py` & `frogmouth-0.6.0/frogmouth/widgets/viewer.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.5.0/pyproject.toml` & `frogmouth-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "frogmouth"
 homepage = "https://github.com/Textualize/frogmouth"
-version = "0.5.0"
+version = "0.6.0"
 description = "A Markdown document viewer for the terminal"
 authors = ["Dave Pearson <dave@textualize.io>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "frogmouth"}]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -24,22 +24,22 @@
     "Programming Language :: Python :: 3.9",
     "Topic :: Software Development :: Documentation",
     "Topic :: Text Processing :: Markup :: Markdown",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-textual = {version = "^0.24.0"}
+textual = {version = ">=0.24.0"}
 typing-extensions = "^4.5.0"
 httpx = "^0.23.3"
 xdg = "^6.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
-textual = {extras = ["dev"], version = "^0.24.0"}
+textual = {extras = ["dev"], version = ">=0.24.0"}
 mypy = "^1.1.1"
 pylint = "^2.17.1"
 pre-commit = "^3.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `frogmouth-0.5.0/PKG-INFO` & `frogmouth-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frogmouth
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Markdown document viewer for the terminal
 Home-page: https://github.com/Textualize/frogmouth
 License: MIT
 Author: Dave Pearson
 Author-email: dave@textualize.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -26,15 +26,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
-Requires-Dist: textual (>=0.24.0,<0.25.0)
+Requires-Dist: textual (>=0.24.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Requires-Dist: xdg (>=6.0.0,<7.0.0)
 Description-Content-Type: text/markdown
 
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/554369/234892488-856f9da7-7b82-4429-ac35-0d0545bf0d24.png"  width="300" align="center"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: frogmouth Version: 0.5.0 Summary: A Markdown
+Metadata-Version: 2.1 Name: frogmouth Version: 0.6.0 Summary: A Markdown
 document viewer for the terminal Home-page: https://github.com/Textualize/
 frogmouth License: MIT Author: Dave Pearson Author-email: dave@textualize.io
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: Other
 Audience Classifier: License :: OSI Approved :: MIT License Classifier:
@@ -13,16 +13,16 @@
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Software
 Development :: Documentation Classifier: Topic :: Text Processing :: Markup ::
 Markdown Requires-Dist: httpx (>=0.23.3,<0.24.0) Requires-Dist: textual
-(>=0.24.0,<0.25.0) Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) Requires-
-Dist: xdg (>=6.0.0,<7.0.0) Description-Content-Type: text/markdown
+(>=0.24.0) Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) Requires-Dist: xdg
+(>=6.0.0,<7.0.0) Description-Content-Type: text/markdown
 [https://user-images.githubusercontent.com/554369/234892488-856f9da7-7b82-4429-
                             ac35-0d0545bf0d24.png]
 [![Discord](https://img.shields.io/discord/1026214085173461072)](https://
 discord.gg/Enf6Z3qhVr) # Frogmouth Frogmouth is a Markdown viewer / browser for
 your terminal, built with [Textual](https://github.com/Textualize/textual).
 Frogmouth can open `*.md` files locally or via a URL. There is a familiar
 browser-like navigation stack, history, bookmarks, and table of contents.
```

