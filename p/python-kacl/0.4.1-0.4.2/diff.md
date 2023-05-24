# Comparing `tmp/python-kacl-0.4.1.tar.gz` & `tmp/python-kacl-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-kacl-0.4.1.tar", last modified: Sun May 21 18:27:45 2023, max compression
+gzip compressed data, was "python-kacl-0.4.2.tar", last modified: Tue May 23 21:39:02 2023, max compression
```

## Comparing `python-kacl-0.4.1.tar` & `python-kacl-0.4.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:27:45.474114 python-kacl-0.4.1/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-21 18:27:36.000000 python-kacl-0.4.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-21 18:27:36.000000 python-kacl-0.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    17898 2023-05-21 18:27:45.474114 python-kacl-0.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    17249 2023-05-21 18:27:36.000000 python-kacl-0.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:27:45.472114 python-kacl-0.4.1/kacl/
--rw-rw-rw-   0 root         (0) root         (0)      644 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      661 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/changes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:27:45.472114 python-kacl-0.4.1/kacl/config/
--rw-rw-rw-   0 root         (0) root         (0)      991 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/config/kacl-default.yml
--rw-rw-rw-   0 root         (0) root         (0)     2792 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/config.py
--rw-rw-rw-   0 root         (0) root         (0)    23133 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/document.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/element.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/exception.py
--rwxrwxrwx   0 root         (0) root         (0)    14244 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/kacl_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1654 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/link_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     2330 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2008 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/validation.py
--rw-rw-rw-   0 root         (0) root         (0)     2943 2023-05-21 18:27:36.000000 python-kacl-0.4.1/kacl/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:27:45.473114 python-kacl-0.4.1/python_kacl.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17898 2023-05-21 18:27:45.000000 python-kacl-0.4.1/python_kacl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      603 2023-05-21 18:27:45.000000 python-kacl-0.4.1/python_kacl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 18:27:45.000000 python-kacl-0.4.1/python_kacl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-21 18:27:45.000000 python-kacl-0.4.1/python_kacl.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 18:27:45.000000 python-kacl-0.4.1/python_kacl.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-21 18:27:45.000000 python-kacl-0.4.1/python_kacl.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-21 18:27:45.000000 python-kacl-0.4.1/python_kacl.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 18:27:45.475114 python-kacl-0.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1601 2023-05-21 18:27:36.000000 python-kacl-0.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:27:45.474114 python-kacl-0.4.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-05-21 18:27:36.000000 python-kacl-0.4.1/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1264 2023-05-21 18:27:36.000000 python-kacl-0.4.1/tests/snapshot_directory.py
--rw-rw-rw-   0 root         (0) root         (0)     5411 2023-05-21 18:27:36.000000 python-kacl-0.4.1/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    11806 2023-05-21 18:27:36.000000 python-kacl-0.4.1/tests/test_kacl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 21:39:02.801901 python-kacl-0.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-23 21:38:54.000000 python-kacl-0.4.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-23 21:38:54.000000 python-kacl-0.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    17898 2023-05-23 21:39:02.801901 python-kacl-0.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    17249 2023-05-23 21:38:54.000000 python-kacl-0.4.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 21:39:02.799901 python-kacl-0.4.2/kacl/
+-rw-rw-rw-   0 root         (0) root         (0)      644 2023-05-23 21:38:54.000000 python-kacl-0.4.2/kacl/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-05-23 21:38:54.000000 python-kacl-0.4.2/kacl/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      661 2023-05-23 21:38:54.000000 python-kacl-0.4.2/kacl/changes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 21:39:02.799901 python-kacl-0.4.2/kacl/config/
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-05-23 21:38:54.000000 python-kacl-0.4.2/kacl/config/kacl-default.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2792 2023-05-23 21:38:54.000000 python-kacl-0.4.2/kacl/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    18740 2023-05-23 21:38:54.000000 python-kacl-0.4.2/kacl/document.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2023-05-23 21:38:54.000000 python-kacl-0.4.2/kacl/element.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-05-23 21:38:54.000000 python-kacl-0.4.2/kacl/exception.py
+-rwxrwxrwx   0 root         (0) root         (0)    14252 2023-05-23 21:38:54.000000 python-kacl-0.4.2/kacl/kacl_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1654 2023-05-23 21:38:54.000000 python-kacl-0.4.2/kacl/link_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     2338 2023-05-23 21:38:54.000000 python-kacl-0.4.2/kacl/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-05-23 21:38:54.000000 python-kacl-0.4.2/kacl/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2023-05-23 21:38:54.000000 python-kacl-0.4.2/kacl/validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     9139 2023-05-23 21:38:54.000000 python-kacl-0.4.2/kacl/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 21:39:02.800901 python-kacl-0.4.2/python_kacl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17898 2023-05-23 21:39:02.000000 python-kacl-0.4.2/python_kacl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      620 2023-05-23 21:39:02.000000 python-kacl-0.4.2/python_kacl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 21:39:02.000000 python-kacl-0.4.2/python_kacl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-23 21:39:02.000000 python-kacl-0.4.2/python_kacl.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 21:39:02.000000 python-kacl-0.4.2/python_kacl.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-23 21:39:02.000000 python-kacl-0.4.2/python_kacl.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-23 21:39:02.000000 python-kacl-0.4.2/python_kacl.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 21:39:02.801901 python-kacl-0.4.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1601 2023-05-23 21:38:54.000000 python-kacl-0.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 21:39:02.801901 python-kacl-0.4.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-05-23 21:38:54.000000 python-kacl-0.4.2/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1264 2023-05-23 21:38:54.000000 python-kacl-0.4.2/tests/snapshot_directory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5619 2023-05-23 21:38:54.000000 python-kacl-0.4.2/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    11806 2023-05-23 21:38:54.000000 python-kacl-0.4.2/tests/test_kacl.py
```

### Comparing `python-kacl-0.4.1/LICENSE` & `python-kacl-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.1/PKG-INFO` & `python-kacl-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: python-kacl
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python module and CLI tool for validating and modifying Changelogs in "keep-a-changelog" format"
 Home-page: https://gitlab.com/schmieder.matthias/python-kacl.git
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Version Control
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-kacl
 
 [![Build Status](https://gitlab.com/schmieder.matthias/python-kacl/badges/main/pipeline.svg?ignore_skipped=true](https://gitlab.com/schmieder.matthias/python-kacl)
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=schmieder.matthias_python-kacl&metric=coverage)](https://sonarcloud.io/summary/new_code?id=schmieder.matthias_python-kacl)
```

### Comparing `python-kacl-0.4.1/README.md` & `python-kacl-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.1/kacl/__init__.py` & `python-kacl-0.4.2/kacl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Version of the python-kacl package
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 from kacl.document import KACLDocument
 from kacl.serializer import KACLMarkdownSerializer
 
 
 def load(file):
     """
```

### Comparing `python-kacl-0.4.1/kacl/changes.py` & `python-kacl-0.4.2/kacl/changes.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.1/kacl/config/kacl-default.yml` & `python-kacl-0.4.2/kacl/config/kacl-default.yml`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.1/kacl/config.py` & `python-kacl-0.4.2/kacl/config.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.1/kacl/document.py` & `python-kacl-0.4.2/kacl/document.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import datetime
 import os
-import re
 
 import git
 import semver
 
 from kacl.config import KACLConfig
 from kacl.element import KACLElement
 from kacl.exception import KACLException
@@ -103,35 +102,17 @@
         #         line_number=None,
         #         error_message="'Unreleased' section is missing from the Changelog"
         #     )
 
         # 3. assert versions in valid format
         versions = self.versions()
         for v in versions:
-            if "Unreleased" != v.version():
-                raw = v.raw()
-                regex = KACLParser.semver_regex
-                regex_error = r"#\s+(.*)\s+"
-                if v.link():
-                    regex = f"#\\s+\\[{KACLParser.semver_regex}\\]"
-                    regex_error = r"#\s+\[(.*)\]"
-                if not KACLParser.parse_sem_ver(raw, regex):
-                    start_pos = 0
-                    end_pos = 0
-                    m = re.match(regex_error, raw)
-                    if m:
-                        start_pos = raw.find(m.group(1))
-                        end_pos = start_pos + len(m.group(1))
-                    validation.add_error(
-                        line=raw,
-                        line_number=v.line_number(),
-                        error_message="Version is not a valid semantic version.",
-                        start_character_pos=start_pos,
-                        end_character_pos=end_pos,
-                    )
+            validation_errors = v.validate(self.config)
+            for e in validation_errors:
+                validation.add(e)
 
         # 3.1 assert versions in descending order
         for i in range(len(versions) - 1):
             try:
                 v0 = versions[i]
                 v1 = versions[i + 1]
                 if semver.VersionInfo.compare(v0.version(), v1.version()) < 1:
@@ -141,88 +122,19 @@
                         error_message="Versions are not in descending order.",
                         start_character_pos=0,
                         end_character_pos=len(v1.raw()),
                     )
             except Exception:
                 pass
 
-        # 3.2 assert versions have a valid date
-        for v in versions:
-            if "Unreleased" != v.version():
-                if not v.date() or len(v.date()) < 1:
-                    validation.add_error(
-                        line=v.raw(),
-                        line_number=v.line_number(),
-                        error_message="Versions need to be decorated with a release date in the following format 'YYYY-MM-DD'",
-                        start_character_pos=0,
-                        end_character_pos=len(v.raw()),
-                    )
-                if v.date() and not re.match(r"\d\d\d\d-[0-1][\d]-[0-3][\d]", v.date()):
-                    start_pos = v.raw().find(v.date())
-                    end_pos = start_pos + len(v.date())
-                    validation.add_error(
-                        line=v.raw(),
-                        line_number=v.line_number(),
-                        error_message="Date does not match format 'YYYY-MM-DD'",
-                        start_character_pos=start_pos,
-                        end_character_pos=end_pos,
-                    )
-
-            # 3.3 check that only allowed sections are in the version
-            sections = v.sections()
-            for title, element in sections.items():
-                if title not in self.config.allowed_version_sections:
-                    start_pos = element.raw().find(title)
-                    end_pos = start_pos + len(title)
-                    validation.add_error(
-                        line=element.raw(),
-                        line_number=element.line_number(),
-                        error_message=f'"{title}" is not a valid section for a version. Options are [{",".join( self.config.allowed_version_sections)}]',
-                        start_character_pos=start_pos,
-                        end_character_pos=end_pos,
-                    )
-                # 3.4 check that only list elements are in the sections
-                # 3.4.1 bring everything into a single line
-                body = element.body()
-                body_clean = re.sub(r"\n\s+", "", body)
-                lines = body_clean.split("\n\n")
-                non_list_lines = [
-                    x
-                    for x in lines
-                    if not x.strip().startswith("-") and len(x.strip()) > 0
-                ]
-                if len(non_list_lines) > 0:
-                    validation.add_error(
-                        line=body.strip(),
-                        line_number=element.line_number(),
-                        error_message="Section does contain more than only listings.",
-                    )
-            # 3.5 make sure that every version that has content has it's content in a section
-            if len(v.sections()) == 0 and len(v.body().strip()) != 0:
-                validation.add_error(
-                    line=v.raw(),
-                    line_number=v.line_number(),
-                    error_message=f'Version "{v.version()}" has change elements outside of a change section.',
-                )
-
-            # 3.6 Check that a link exists for linked versions
-            if "[" in v.raw() and "]" in v.raw() and not v.has_link_reference():
-                validation.add_error(
-                    line=v.raw(),
-                    line_number=v.line_number(),
-                    error_message=f'Version "{v.version()}" is linked, but no link reference found in changelog file.',
-                    start_character_pos=v.raw().find("["),
-                    end_character_pos=v.raw().find("]"),
-                )
-
         # 4 link references
         # 4.1 check that there are only linked references
-        version_strings = [v.version() for v in versions]
+        version_strings = [v.version().lower() for v in versions]
         for v, link in self.__link_references.items():
-            if v not in version_strings:
+            if v.lower() not in version_strings:
                 validation.add_error(
                     line=link.raw(),
                     line_number=link.line_number(),
                     error_message="Link not referenced anywhere in the document",
                     start_character_pos=0,
                     end_character_pos=len(link.raw()),
                 )
@@ -541,15 +453,15 @@
 
         # read versions
         versions = KACLParser.parse_header(changelog_body, 2, 2)
         versions = [KACLVersion(element=x) for x in versions]
 
         # set link references into versions if available
         for v in versions:
-            v.set_link(link_references.get(v.version(), None))
+            v.set_link(link_references.get(v.version().lower(), None))
 
         return KACLDocument(
             data=data,
             headers=headers,
             versions=versions,
             link_references=link_references,
         )
```

### Comparing `python-kacl-0.4.1/kacl/kacl_cli.py` & `python-kacl-0.4.2/kacl/kacl_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,16 +229,17 @@
     Exit code is the number of identified errors.
     """
     kacl_changelog = load_changelog(ctx)
     kacl_changelog_filepath = os.path.basename(
         kacl_changelog.config.changelog_file_path
     )
 
-    valid = kacl_changelog.is_valid()
     validation = kacl_changelog.validate()
+    valid = len(validation.errors()) < 1
+
     if as_json:
         validation_map = validation.convert_to_dict()
         click.echo(json.dumps(validation_map, sort_keys=True, indent=4))
     else:
         for error in validation.errors():
             start_char_pos, end_char_pos = error.position()
 
@@ -508,9 +509,9 @@
         click.secho(str(e), fg="red")
         sys.exit(1)
     except Exception:
         click.echo(traceback.format_exc())
         sys.exit(1)
 
 
-if __name__ == "__main__":
-    start()
+# if __name__ == "__main__":
+#     start()
```

### Comparing `python-kacl-0.4.1/kacl/link_provider.py` & `python-kacl-0.4.2/kacl/link_provider.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.1/kacl/parser.py` & `python-kacl-0.4.2/kacl/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         reg_expr = r"\n\[(.*)\]:(.*)"
         for match in re.finditer(reg_expr, text):
             if begin is None:
                 begin = match.start()
             version = match.group(1).strip()
             link = match.group(2).strip()
             line_number = text[: match.start()].count("\n") + 1
-            link_references[version] = KACLElement(
+            link_references[version.lower()] = KACLElement(
                 raw=match.group().strip(),
                 title=version,
                 body=link,
                 line_number=line_number,
             )
 
         return begin, link_references
```

### Comparing `python-kacl-0.4.1/kacl/serializer.py` & `python-kacl-0.4.2/kacl/serializer.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.1/kacl/validation.py` & `python-kacl-0.4.2/kacl/validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 
     def is_valid(self):
         return len(self.__validation_errors) == 0
 
     def errors(self):
         return self.__validation_errors
 
+    def add(self, validation_error: KACLValidationError):
+        self.__validation_errors.append(validation_error)
+
     def add_error(
         self,
         line,
         line_number,
         error_message,
         start_character_pos=None,
         end_character_pos=None,
```

### Comparing `python-kacl-0.4.1/python_kacl.egg-info/PKG-INFO` & `python-kacl-0.4.2/python_kacl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: python-kacl
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python module and CLI tool for validating and modifying Changelogs in "keep-a-changelog" format"
 Home-page: https://gitlab.com/schmieder.matthias/python-kacl.git
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Version Control
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-kacl
 
 [![Build Status](https://gitlab.com/schmieder.matthias/python-kacl/badges/main/pipeline.svg?ignore_skipped=true](https://gitlab.com/schmieder.matthias/python-kacl)
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=schmieder.matthias_python-kacl&metric=coverage)](https://sonarcloud.io/summary/new_code?id=schmieder.matthias_python-kacl)
```

### Comparing `python-kacl-0.4.1/python_kacl.egg-info/SOURCES.txt` & `python-kacl-0.4.2/python_kacl.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 kacl/__init__.py
+kacl/__main__.py
 kacl/changes.py
 kacl/config.py
 kacl/document.py
 kacl/element.py
 kacl/exception.py
 kacl/kacl_cli.py
 kacl/link_provider.py
```

### Comparing `python-kacl-0.4.1/setup.py` & `python-kacl-0.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "0.4.1"
+version = "0.4.2"
 
 version = f"{version}{os.environ.get('PIP_VERSION_POSTFIX','')}"
 
 # read the requirements from requirements.txt
 requirements = []
 with pathlib.Path("requirements.txt").open() as requirements_txt:
     requirements = [
@@ -33,18 +33,18 @@
     url="https://gitlab.com/schmieder.matthias/python-kacl.git",
     author="Matthias Schmieder",
     author_email="schmieder.matthias@gmail.com",
     entry_points={"console_scripts": ["kacl-cli = kacl.kacl_cli:start"]},
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=requirements,
     zip_safe=False,
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Version Control",
     ],
 )
```

### Comparing `python-kacl-0.4.1/tests/snapshot_directory.py` & `python-kacl-0.4.2/tests/snapshot_directory.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.1/tests/test_cli.py` & `python-kacl-0.4.2/tests/test_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,22 @@
     assert result.exit_code == 0
     assert result.output == "Success\n"
 
     result = runner.invoke(cli, ["-f", "tests/data/CHANGELOG_invalid.md", "verify"])
     assert result.exit_code == 10  # spawns 8 errors
 
 
+def test_verify_invalid_duplicates():
+    runner = CliRunner()
+    result = runner.invoke(
+        cli, ["-f", "tests/data/CHANGELOG_invalid_duplicates.md", "verify"]
+    )
+    assert result.exit_code == 2
+
+
 def test_verify_with_json_output():
     runner = CliRunner()
     result = runner.invoke(
         cli, ["-f", "tests/data/CHANGELOG_invalid.md", "verify", "--json"]
     )
     validation_result = json.loads(result.output)
```

### Comparing `python-kacl-0.4.1/tests/test_kacl.py` & `python-kacl-0.4.2/tests/test_kacl.py`

 * *Files identical despite different names*

