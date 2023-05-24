# Comparing `tmp/ansible-anonymizer-1.2.2.tar.gz` & `tmp/ansible-anonymizer-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-anonymizer-1.2.2.tar", last modified: Fri May  5 20:19:47 2023, max compression
+gzip compressed data, was "ansible-anonymizer-1.3.0.tar", last modified: Wed May 24 20:28:16 2023, max compression
```

## Comparing `ansible-anonymizer-1.2.2.tar` & `ansible-anonymizer-1.3.0.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 20:19:47.128850 ansible-anonymizer-1.2.2/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      292 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.2/.editorconfig
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 20:19:47.126850 ansible-anonymizer-1.2.2/.github/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      321 2023-03-23 15:13:37.000000 ansible-anonymizer-1.2.2/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 20:19:47.126850 ansible-anonymizer-1.2.2/.github/workflows/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      551 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.2/.github/workflows/tox.yml
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1204 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.2/.gitignore
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1138 2023-04-05 13:57:02.000000 ansible-anonymizer-1.2.2/.pre-commit-config.yaml
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1486 2023-05-05 20:19:19.000000 ansible-anonymizer-1.2.2/CHANGELOG.rst
--rw-r--r--   0 goneri    (1002) goneri    (1002)     2478 2023-03-23 15:13:37.000000 ansible-anonymizer-1.2.2/CONTRIBUTING.rst
--rw-r--r--   0 goneri    (1002) goneri    (1002)       63 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.2/HISTORY.rst
--rw-r--r--   0 goneri    (1002) goneri    (1002)      588 2023-03-22 17:41:29.000000 ansible-anonymizer-1.2.2/LICENSE
--rw-r--r--   0 goneri    (1002) goneri    (1002)      168 2023-04-05 18:22:37.000000 ansible-anonymizer-1.2.2/MANIFEST.in
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1671 2023-05-05 20:19:47.128850 ansible-anonymizer-1.2.2/PKG-INFO
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1227 2023-05-05 17:28:31.000000 ansible-anonymizer-1.2.2/README.rst
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 20:19:47.127850 ansible-anonymizer-1.2.2/ansible_anonymizer/
--rw-r--r--   0 goneri    (1002) goneri    (1002)       90 2023-05-05 20:19:19.000000 ansible-anonymizer-1.2.2/ansible_anonymizer/__init__.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     9368 2023-05-05 20:11:23.000000 ansible-anonymizer-1.2.2/ansible_anonymizer/anonymizer.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)      716 2023-05-05 20:11:23.000000 ansible-anonymizer-1.2.2/ansible_anonymizer/cli.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1914 2023-05-05 20:19:14.000000 ansible-anonymizer-1.2.2/ansible_anonymizer/field_checks.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)      294 2023-05-05 20:19:14.000000 ansible-anonymizer-1.2.2/ansible_anonymizer/jinja2.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)    11471 2023-05-05 20:19:19.000000 ansible-anonymizer-1.2.2/ansible_anonymizer/parser.py
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 20:19:47.128850 ansible-anonymizer-1.2.2/ansible_anonymizer.egg-info/
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1671 2023-05-05 20:19:47.000000 ansible-anonymizer-1.2.2/ansible_anonymizer.egg-info/PKG-INFO
--rw-r--r--   0 goneri    (1002) goneri    (1002)      659 2023-05-05 20:19:47.000000 ansible-anonymizer-1.2.2/ansible_anonymizer.egg-info/SOURCES.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)        1 2023-05-05 20:19:47.000000 ansible-anonymizer-1.2.2/ansible_anonymizer.egg-info/dependency_links.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       67 2023-05-05 20:19:47.000000 ansible-anonymizer-1.2.2/ansible_anonymizer.egg-info/entry_points.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       12 2023-05-05 20:19:47.000000 ansible-anonymizer-1.2.2/ansible_anonymizer.egg-info/requires.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       19 2023-05-05 20:19:47.000000 ansible-anonymizer-1.2.2/ansible_anonymizer.egg-info/top_level.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1551 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.2/pyproject.toml
--rw-r--r--   0 goneri    (1002) goneri    (1002)       38 2023-05-05 20:19:47.128850 ansible-anonymizer-1.2.2/setup.cfg
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 20:19:47.128850 ansible-anonymizer-1.2.2/tests/
--rw-r--r--   0 goneri    (1002) goneri    (1002)    17930 2023-05-05 20:19:19.000000 ansible-anonymizer-1.2.2/tests/test_anonymizer.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1286 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.2/tox.ini
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-24 20:28:16.838947 ansible-anonymizer-1.3.0/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      292 2023-03-10 14:59:31.000000 ansible-anonymizer-1.3.0/.editorconfig
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-24 20:28:16.836947 ansible-anonymizer-1.3.0/.github/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      321 2023-03-23 15:13:37.000000 ansible-anonymizer-1.3.0/.github/ISSUE_TEMPLATE.md
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-24 20:28:16.836947 ansible-anonymizer-1.3.0/.github/workflows/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      551 2023-03-10 14:59:31.000000 ansible-anonymizer-1.3.0/.github/workflows/tox.yml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1204 2023-03-10 14:59:31.000000 ansible-anonymizer-1.3.0/.gitignore
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      142 2023-05-24 20:00:02.000000 ansible-anonymizer-1.3.0/.gitleaks.toml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1208 2023-05-24 17:40:23.000000 ansible-anonymizer-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     2075 2023-05-24 20:00:16.000000 ansible-anonymizer-1.3.0/CHANGELOG.rst
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     2478 2023-03-23 15:13:37.000000 ansible-anonymizer-1.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       63 2023-03-10 14:59:31.000000 ansible-anonymizer-1.3.0/HISTORY.rst
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      588 2023-03-22 17:41:29.000000 ansible-anonymizer-1.3.0/LICENSE
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      168 2023-04-05 18:22:37.000000 ansible-anonymizer-1.3.0/MANIFEST.in
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1671 2023-05-24 20:28:16.838947 ansible-anonymizer-1.3.0/PKG-INFO
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1227 2023-05-05 17:28:31.000000 ansible-anonymizer-1.3.0/README.rst
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-24 20:28:16.836947 ansible-anonymizer-1.3.0/ansible_anonymizer/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       90 2023-05-24 20:00:16.000000 ansible-anonymizer-1.3.0/ansible_anonymizer/__init__.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     9368 2023-05-24 17:40:09.000000 ansible-anonymizer-1.3.0/ansible_anonymizer/anonymizer.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      724 2023-05-24 17:21:14.000000 ansible-anonymizer-1.3.0/ansible_anonymizer/cli.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     2071 2023-05-24 17:21:14.000000 ansible-anonymizer-1.3.0/ansible_anonymizer/field_checks.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      327 2023-05-24 17:21:14.000000 ansible-anonymizer-1.3.0/ansible_anonymizer/jinja2.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    13085 2023-05-24 20:02:45.000000 ansible-anonymizer-1.3.0/ansible_anonymizer/parser.py
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-24 20:28:16.837947 ansible-anonymizer-1.3.0/ansible_anonymizer.egg-info/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1671 2023-05-24 20:28:16.000000 ansible-anonymizer-1.3.0/ansible_anonymizer.egg-info/PKG-INFO
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      743 2023-05-24 20:28:16.000000 ansible-anonymizer-1.3.0/ansible_anonymizer.egg-info/SOURCES.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)        1 2023-05-24 20:28:16.000000 ansible-anonymizer-1.3.0/ansible_anonymizer.egg-info/dependency_links.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       67 2023-05-24 20:28:16.000000 ansible-anonymizer-1.3.0/ansible_anonymizer.egg-info/entry_points.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       12 2023-05-24 20:28:16.000000 ansible-anonymizer-1.3.0/ansible_anonymizer.egg-info/requires.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       19 2023-05-24 20:28:16.000000 ansible-anonymizer-1.3.0/ansible_anonymizer.egg-info/top_level.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1683 2023-05-24 20:00:02.000000 ansible-anonymizer-1.3.0/pyproject.toml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       38 2023-05-24 20:28:16.838947 ansible-anonymizer-1.3.0/setup.cfg
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-24 20:28:16.837947 ansible-anonymizer-1.3.0/tests/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    11265 2023-05-24 20:00:02.000000 ansible-anonymizer-1.3.0/tests/test_anonymizer.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1648 2023-05-24 20:00:02.000000 ansible-anonymizer-1.3.0/tests/test_field_checks.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      294 2023-05-24 20:00:02.000000 ansible-anonymizer-1.3.0/tests/test_jinja2.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     9281 2023-05-24 20:21:16.000000 ansible-anonymizer-1.3.0/tests/test_parser.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1430 2023-05-24 20:00:16.000000 ansible-anonymizer-1.3.0/tox.ini
```

### Comparing `ansible-anonymizer-1.2.2/.github/workflows/tox.yml` & `ansible-anonymizer-1.3.0/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.2/.gitignore` & `ansible-anonymizer-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.2/.pre-commit-config.yaml` & `ansible-anonymizer-1.3.0/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 repos:
-- repo: https://github.com/asottile/reorder_python_imports
-  rev: v3.9.0
+- repo: https://github.com/astral-sh/ruff-pre-commit
+  # Ruff version.
+  rev: v0.0.269
   hooks:
-  - id: reorder-python-imports
-    language_version: python3
+    - id: ruff
+      args: [--fix, --exit-non-zero-on-fix]
 - repo: https://github.com/ambv/black
   rev: 23.1.0
   hooks:
   - id: black
     args: [--safe, --quiet, --line-length, "100"]
     language_version: python3
     require_serial: true
@@ -35,16 +36,18 @@
 - repo: local
   hooks:
     - id: pylint
       name: pylint
       entry: pylint
       language: python
       types: [python]
+      args: ["ansible_anonymizer"]
 - repo: local
   hooks:
     - id: mypy
       name: mypy
       entry: mypy
       language: python
       types: [python]
       additional_dependencies:
         - mypy
+        - types-PyYAML
```

### Comparing `ansible-anonymizer-1.2.2/CHANGELOG.rst` & `ansible-anonymizer-1.3.0/CHANGELOG.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,31 @@
 Changelog
 =========
 
+Version 1.3.0 (2023-05-24)
+-------------
+
+- tests: split up test_anonymizer.py
+- pre-commit: only check ansible_anonymizer
+- pre-commit: mypy needs types-PyYAML
+- pylint: various fixes to get pylint to pass
+- pre-commmit: replace reorder_python_imports with ruff
+- tests: don't redefine dedent
+- cli: don't had an extra \n
+- parser: remove an uncessary ParserError exception
+- handle : or = in password field
+- better handling of unquoted password
+- extra tests
+- test: cover Node.get_secret()
+- properly handle series of spaces before password
+- add a .gitleaks.toml file
+
+
 Version 1.2.2 (2023-05-05)
+-------------
 
 - adjustment to handle aws/credentials
 
 Version 1.2.1 (2023-05-05)
 -------------
 
 - clean up some debug traces
```

### Comparing `ansible-anonymizer-1.2.2/CONTRIBUTING.rst` & `ansible-anonymizer-1.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.2/LICENSE` & `ansible-anonymizer-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.2/PKG-INFO` & `ansible-anonymizer-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-anonymizer
-Version: 1.2.2
+Version: 1.3.0
 Summary: Ansible Anonymizer
 Author-email: Gonéri Le Bouder <goneri@lebouder.net>
 Project-URL: Homepage, https://github.com/ansible/anonymizer
 Keywords: pii,anonymize
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `ansible-anonymizer-1.2.2/README.rst` & `ansible-anonymizer-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.2/ansible_anonymizer/anonymizer.py` & `ansible-anonymizer-1.3.0/ansible_anonymizer/anonymizer.py`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.2/ansible_anonymizer/cli.py` & `ansible-anonymizer-1.3.0/ansible_anonymizer/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 def main() -> None:
     parser = argparse.ArgumentParser()
     parser.add_argument("file_path", type=pathlib.Path)
     parser.add_argument("--format", choices=["text", "yaml"], type=str, default="text")
     args = parser.parse_args()
 
     if args.format == "text":
-        print(anonymize_text_block(args.file_path.read_text()))
+        print(anonymize_text_block(args.file_path.read_text()), end="")
     elif args.format == "yaml":
         print(anonymize_struct(yaml.safe_load(args.file_path.read_text())))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ansible-anonymizer-1.2.2/ansible_anonymizer/field_checks.py` & `ansible-anonymizer-1.3.0/ansible_anonymizer/field_checks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-
+"""Functions used to identify the field types."""
 import re
 
 # Denylist regex to TC of secrets filter
 # From detect_secrets.plugins (Apache v2 License)
 DENYLIST = (
     "api_?key",
     "auth_?key",
@@ -40,14 +40,15 @@
     # Valid field found in sudo configuration
     if field_name == "NOPASSWD":
         return True
     return False
 
 
 def is_password_field_name(name: str) -> bool:
+    """Return True if name looks like a password field name."""
     flags = re.MULTILINE | re.IGNORECASE
     if is_allowed_password_field(name):
         return False
     return re.search(DENYLIST_REGEX_WITH_PREFIX, name, flags=flags) is not None
 
 
 def is_jinja2_expression(value: str) -> bool:
@@ -67,12 +68,13 @@
     ):
         return True
 
     return False
 
 
 def is_path(content: str) -> bool:
+    """Return True if content is a path."""
     # Rather conservative on purpose to avoid a false
     # positive
     if "/" not in content:
         return False
     return bool(re.match(r"^(|~)[a-z0-9_/\.-]+$", content, flags=re.IGNORECASE))
```

### Comparing `ansible-anonymizer-1.2.2/ansible_anonymizer/parser.py` & `ansible-anonymizer-1.3.0/ansible_anonymizer/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 #!/usr/bin/env python3
-
+"""Parser for YAML-like structure that is error tolerant."""
 from collections.abc import Generator
 from enum import Enum
-from typing import Literal, Optional, Union
+from typing import Optional, Union
 
 from ansible_anonymizer.field_checks import is_password_field_name
 from ansible_anonymizer.jinja2 import str_jinja2_variable_name
 
-"""Parser for YAML-like structure that tolerate error."""
-
-quote_t = Literal['"', "'"]
-
 
 class NodeType(Enum):
     """The different type of Node returned by the parser."""
 
+    # pylint: disable=invalid-name
+
     unknown = 0
     field = 1
     separator = 2
     quoted_string_holder = 3
     quoted_string_closing = 4
     new_line = 5
     space = 6
@@ -28,14 +26,15 @@
 
 
 class ParserError(Exception):
     """Unexpected behaviour."""
 
 
 class Node:
+    # pylint: disable=too-many-instance-attributes
     """A element returned by the parser."""
 
     def __init__(self, begin_at: int) -> None:
         self.previous: Optional["Node"] = None
         self.next: Optional["Node"] = None
         self.begin_at: int = begin_at
         self.end_at: int
@@ -66,63 +65,77 @@
         """Identify the secret Node associated with the current Node."""
         candidate = self.next
         has_separator = False
         while candidate:
             if candidate.type is NodeType.space:
                 pass
             elif candidate.type is NodeType.quoted_string_closing:
-                if candidate.holder is not self.holder:
-                    raise ParserError()
+                pass
             elif has_separator:
                 if candidate.type is NodeType.securized:
                     # We should not come back on the same node
                     raise ParserError
-                if candidate.type is NodeType.field:
-                    return candidate
-                if candidate.type is NodeType.unknown:
-                    return candidate
-                if candidate.type is NodeType.quoted_string_holder:
+                if candidate.type in [
+                    NodeType.field,
+                    NodeType.unknown,
+                    NodeType.quoted_string_holder,
+                ]:
                     return candidate
-                else:
-                    return None
+                return None
             elif candidate.type is NodeType.separator:
                 has_separator = True
             else:
                 return None
             candidate = candidate.next
         return None
 
+    def merge_with_next(self) -> None:
+        """Merge the current node with the next one."""
+        self.type = NodeType.unknown
+        assert self.next  # for mypy # noqa: S101
+        self.text += self.next.text
+        self.next.type = NodeType.deleted
+        self.next.text = "KILLED"
+        self.next = self.next.next
+        if self.next:
+            self.next.previous = self
+
     def is_password_field_name(self) -> bool:
         """Return True if the field name matches the DENYLIST_REGEX regex."""
         return is_password_field_name(self.text)
 
     def __str__(self) -> str:
         """Expose the Node as a string."""
         return f"TEXT={self.text}, BEGIN_AT={self.begin_at}, TYPE={self.type}"
 
 
-def is_valid_first_character_for_a_variable(c: str) -> bool:
+def is_valid_first_character_for_a_variable(char: str) -> bool:
     """Assuming variable names cannot start with a digit."""
-    return c.isascii() and (c.isalpha() or c in ["-", "_"])
+    return char.isascii() and (char.isalpha() or char in ["-", "_"])
 
 
-def is_valid_variable_character(c: str) -> bool:
+def is_valid_variable_character(char: str) -> bool:
+    """Return True if the character can be part of an Ansible variable name."""
     # note: isnumeric accepts a wider range than just the 0-9
-    return c.isascii() and (c.isalpha() or c.isnumeric() or c in ["-", "_"])
+    return char.isascii() and (char.isalpha() or char.isnumeric() or char in ["-", "_"])
 
 
-def is_field_value_sep(c: str) -> bool:
-    return c in [":", "="]
+def is_field_value_sep(char: str) -> bool:
+    """Return True if the character is : or =."""
+    return char in [":", "="]
 
 
 def parser(block: str) -> Node:
+    # pylint: disable=too-many-branches
+    # pylint: disable=too-many-statements
+    """Digest a text block an return a list of Nodes that will be simplified later."""
     root_node = Node(0)
     root_node.type = NodeType.quoted_string_holder
     current_node = root_node
-    for pos, c in enumerate(block):
+    for pos, c in enumerate(block):  # pylint: disable=invalid-name
         if c == "\\":
             new_node = Node(pos)
             new_node.attach(previous=current_node)
             new_node.type = NodeType.backslash
             current_node = new_node
         elif c in ["'", '"']:
             is_protected = current_node.type is NodeType.backslash
@@ -186,21 +199,19 @@
                 current_node = new_node
 
         current_node.text += c
     return root_node
 
 
 def hide_secrets(block: str) -> str:
+    """Return block without any potential secrets."""
     root_node = parser(block)
     close_quotes(root_node)
     handle_backslashes(root_node)
-    # Group substring with unknown and field types
-    # combinate_fields(root_node)
     combinate_value_fields(root_node)
-
     hide_secret_fields(root_node)
 
     output = ""
     for node in flatten(root_node):
         output += node.text
     return output
 
@@ -239,93 +250,119 @@
             current_node = current_node.next
         else:
             current_node.type = NodeType.unknown
         current_node = current_node.next
 
 
 def combinate_value_fields(root_node: Node) -> None:
-    """
-    Merge the unquoted value fields.
+    """Combinate the unquoted value strings."""
+    mergable_types = [NodeType.space, NodeType.field, NodeType.unknown, NodeType.space]
+
+    def _is_a_new_key_value(node: Node) -> bool:
+        """Check if the current node is actually the beginning of a new secret key/value."""
+        if not node.next:
+            return False
+
+        current = node.next
+        if current.type is not NodeType.space:
+            return False
+
+        while current.type == NodeType.space:
+            if current.next is None:
+                return False
+            current = current.next
+
+        # if we've got a separator after the field, we prefer to preserve
+        # it. e.g: secret1: foo secret2: bar, secret1 and secret2 are two distinct seecrets.
+        if current and current.type is NodeType.field and current.next and current.next.text == ":":
+            return True
+        return False
+
+    def _find_separator_node(node: Node) -> Union[None, Node]:
+        while node and node.next:
+            if node.next.type is NodeType.space:
+                node = node.next
+            elif node.next and node.next.type is NodeType.separator:
+                return node.next
+            else:
+                return None
+        return None
 
-    In YAML or INI, a value can be an unprotected string with spaces.
-    Internally     the parser represent such series of spaces and fields
-    as different Node objects. Since all these objects are actually one
-    single value, we merge them together.
-    """
     current_node = root_node
-    mergable_types = [NodeType.space, NodeType.field, NodeType.unknown]
-    post_sep = False
-    while current_node:
-        if post_sep:
-            # We ignore the first space after the : sign
-            if current_node.type is NodeType.space and current_node.next:
-                current_node = current_node.next
-
-            while (
-                current_node.type in mergable_types
-                and not current_node.is_password_field_name()
-                and current_node.next
-                and current_node.next.type in mergable_types
-                and not current_node.next.is_password_field_name()
-            ):
-                current_node.type = NodeType.unknown
-                current_node.text += current_node.next.text
-                current_node.next.type = NodeType.deleted
-                current_node.next.text = "KILLED"
-                current_node.next = current_node.next.next
-                if current_node.next:
-                    current_node.next.previous = current_node
-
-        elif current_node.type is NodeType.separator:
-            post_sep = True
-        if current_node.next is None:
-            break
+    while current_node and current_node.next:
         current_node = current_node.next
+        if current_node.type is not NodeType.field:
+            continue
+        if not current_node.is_password_field_name():
+            continue
 
-
-def print_node(root_node: Node) -> None:
-    for node in flatten(root_node):
-        print(node, end="")
+        secret_content_ptr = current_node.get_secret()
+        if not secret_content_ptr:
+            continue
+        separator = _find_separator_node(current_node)
+        if not separator:
+            continue
+        if secret_content_ptr.type is NodeType.quoted_string_holder:
+            assert secret_content_ptr.closed_by  # for mypy # noqa: S101
+            current_node = secret_content_ptr.closed_by
+            continue
+        while (
+            secret_content_ptr.next
+            and (
+                (secret_content_ptr.next.type in mergable_types)
+                or (
+                    secret_content_ptr.next.type is NodeType.separator
+                    and secret_content_ptr.next.text != separator.text
+                )
+            )
+            and not _is_a_new_key_value(secret_content_ptr)
+        ):
+            secret_content_ptr.merge_with_next()
 
 
 def flatten(node: Node) -> Generator[Node, None, None]:
-    n = node
-    while n:
-        yield n
-        if not n.next:
+    """Iterator that go through each nodes and follow the original text order."""
+    current = node
+    while current:
+        yield current
+        if not current.next:
             break
-        n = n.next
+        current = current.next
 
 
 def hide_secret_fields(root_node: Node) -> None:
+    """Remove the secret fields from a series of nodes."""
+
     def hide_quoted_string(node: Node, secret_node: Node) -> None:
         assert secret_node.closed_by  # for mypy # noqa: S101
         secret_node.next = secret_node.closed_by.next
         secret_node.type = NodeType.securized
         secret_node.text = (
             f"{secret_node.text}{{{{ {str_jinja2_variable_name(node.text)} }}}}{secret_node.text}"
         )
         if secret_node.next:
-            return hide_secret_fields(secret_node.next)
+            hide_secret_fields(secret_node.next)
 
     def hide_regular_field(node: Node, secret_node: Node) -> None:
         secret_node.type = NodeType.securized
         assert secret_node.holder  # for mypy # noqa: S101
         quote = "" if secret_node.holder.text else '"'
         secret_node.text = f"{quote}{{{{ {str_jinja2_variable_name(node.text)} }}}}{quote}"
         if secret_node.next:
-            return hide_secret_fields(secret_node.next)
+            hide_secret_fields(secret_node.next)
 
     for node in flatten(root_node):
         if node.type is not NodeType.field:
             continue
         if not node.is_password_field_name():
             continue
 
         secret_node = node.get_secret()
         if not secret_node:
             continue
 
+        # pylint: disable=inconsistent-return-statements
+        # pylint: disable=no-else-return
         if secret_node.type is NodeType.quoted_string_holder:
             return hide_quoted_string(node, secret_node)
         else:
             return hide_regular_field(node, secret_node)
```

### Comparing `ansible-anonymizer-1.2.2/ansible_anonymizer.egg-info/PKG-INFO` & `ansible-anonymizer-1.3.0/ansible_anonymizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-anonymizer
-Version: 1.2.2
+Version: 1.3.0
 Summary: Ansible Anonymizer
 Author-email: Gonéri Le Bouder <goneri@lebouder.net>
 Project-URL: Homepage, https://github.com/ansible/anonymizer
 Keywords: pii,anonymize
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `ansible-anonymizer-1.2.2/ansible_anonymizer.egg-info/SOURCES.txt` & `ansible-anonymizer-1.3.0/ansible_anonymizer.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .editorconfig
 .gitignore
+.gitleaks.toml
 .pre-commit-config.yaml
 CHANGELOG.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
@@ -19,8 +20,11 @@
 ansible_anonymizer/parser.py
 ansible_anonymizer.egg-info/PKG-INFO
 ansible_anonymizer.egg-info/SOURCES.txt
 ansible_anonymizer.egg-info/dependency_links.txt
 ansible_anonymizer.egg-info/entry_points.txt
 ansible_anonymizer.egg-info/requires.txt
 ansible_anonymizer.egg-info/top_level.txt
-tests/test_anonymizer.py
+tests/test_anonymizer.py
+tests/test_field_checks.py
+tests/test_jinja2.py
+tests/test_parser.py
```

### Comparing `ansible-anonymizer-1.2.2/pyproject.toml` & `ansible-anonymizer-1.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -64,7 +64,10 @@
     "W",  # Warning
     "YTT", # flake8-2020
 ]
 ignore = ["D107", "D203", "D212", "D100", "D103", "PGH003", "D401", "SIM114", "ISC003"]
 
 [tool.ruff.per-file-ignores]
 "tests/test_anonymizer.py" = ["S101", "S105"]
+"tests/test_field_checks.py" = ["S101", "S105"]
+"tests/test_jinja2.py" = ["S101", "S105"]
+"tests/test_parser.py" = ["S101", "S105"]
```

### Comparing `ansible-anonymizer-1.2.2/tox.ini` & `ansible-anonymizer-1.3.0/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tox]
-envlist = py39, py310, py311, flake8, mypy, black, ruff
+envlist = py39, py310, py311, flake8, mypy, black, ruff, pylint
 
 [gh-actions]
 python =
     3.9: py39
     3.10: py310
-    3.11: py311, flake8, mypy, black, ruff
+    3.11: py311, flake8, mypy, black, ruff, pylint
 
 [testenv:flake8]
 basepython = python
 deps = flake8
 commands = flake8 ansible_anonymizer tests
 
 [testenv]
@@ -68,7 +68,15 @@
 
 [testenv:ruff]
 basepython = python3.11
 skip_install = true
 deps =
     ruff
 commands = ruff .
+
+[testenv:pylint]
+basepython = python3.11
+skip_install = true
+deps =
+    PyYAML
+    pylint
+commands = pylint ansible_anonymizer
```

