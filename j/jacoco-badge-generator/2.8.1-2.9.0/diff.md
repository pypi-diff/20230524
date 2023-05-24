# Comparing `tmp/jacoco_badge_generator-2.8.1.tar.gz` & `tmp/jacoco_badge_generator-2.9.0.tar.gz`

## Comparing `jacoco_badge_generator-2.8.1.tar` & `jacoco_badge_generator-2.9.0.tar`

### file list

```diff
@@ -1,68 +1,10 @@
--rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/CHANGELOG.md
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/src/jacoco_badge_generator/__init__.py
--rw-r--r--   0        0        0    10948 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/src/jacoco_badge_generator/__main__.py
--rwxr-xr-x   0        0        0    26885 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/src/jacoco_badge_generator/coverage_badges.py
--rw-r--r--   0        0        0   131380 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/src/jacoco_badge_generator/text_length.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/0.json
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/0.svg
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/0b.json
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/100.json
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/100.svg
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/100b.json
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/599.json
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/599.svg
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/599b.json
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/60.json
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/60.svg
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/60b.json
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/70.json
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/70.svg
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/70b.json
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/78.json
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/78.svg
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/78b.json
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/80.json
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/80.svg
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/80b.json
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/87.json
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/87b.json
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/87b.svg
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/899.json
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/899.svg
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/899b.json
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/90.json
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/90.svg
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/90b.json
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/90b.svg
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/99.json
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/99.svg
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/999.json
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/999.svg
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/999b.json
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/999b.svg
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/99b.json
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/branches100.csv
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/branches90.csv
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/branches901.csv
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/branchesDivZero.csv
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/custom1.json
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/custom1.svg
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/custom2.json
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/custom2.svg
--rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/integration.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/jacoco.csv
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/jacoco100.csv
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/jacoco90.csv
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/jacoco901.csv
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/jacocoDivZero.csv
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/multi1.csv
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/multi2.csv
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/reportTest.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/reportTestFail.json
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/summaryReportTest.csv
--rw-r--r--   0        0        0    41751 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/tests/tests.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/LICENSE
--rw-r--r--   0        0        0    55012 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/README.md
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/pyproject.toml
--rw-r--r--   0        0        0    56100 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.8.1/PKG-INFO
+-rw-r--r--   0        0        0    10769 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.9.0/src/jacoco_badge_generator/__init__.py
+-rw-r--r--   0        0        0    10953 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.9.0/src/jacoco_badge_generator/__main__.py
+-rwxr-xr-x   0        0        0    27127 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.9.0/src/jacoco_badge_generator/coverage_badges.py
+-rw-r--r--   0        0        0   131380 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.9.0/src/jacoco_badge_generator/text_length.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.9.0/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.9.0/LICENSE
+-rw-r--r--   0        0        0    58216 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.9.0/README.md
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0    59304 2020-02-02 00:00:00.000000 jacoco_badge_generator-2.9.0/PKG-INFO
```

### Comparing `jacoco_badge_generator-2.8.1/CHANGELOG.md` & `jacoco_badge_generator-2.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [Unreleased] - 2022-10-24
+## [Unreleased] - 2023-05-24
 
 ### Added
 
 ### Changed
 
 ### Deprecated
 
@@ -17,14 +17,26 @@
 ### Fixed
 
 ### Dependencies
 
 ### CI/CD
 
 
+## [2.9.0] - 2023-05-24
+
+### Added
+* Support for glob patterns in GitHub Actions mode for specifying multiple JaCoCo reports for multi-module projects (note: CLI mode already supported this indirectly since the shell expands globs automatically).
+
+### Dependencies
+* Bump cicirello/pyaction from 4.11.1 to 4.19.0, including upgrading Python within the Docker container to 3.11.
+
+### CI/CD
+* Bump Python to 3.11 in CI/CD workflows.
+
+
 ## [2.8.1] - 2022-10-24
 
 ### Fixed
 * The replacement for GitHub Action's deprecated `set-output` is not available yet for all self-hosted users. This patch
   handles that by using the new `$GITHUB_OUTPUT` environment file if it exists, and otherwise falling back to `set-output`.
 
 ### Dependencies
```

### Comparing `jacoco_badge_generator-2.8.1/src/jacoco_badge_generator/__init__.py` & `jacoco_badge_generator-2.9.0/src/jacoco_badge_generator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # jacoco-badge-generator: Coverage badges, and pull request coverage checks,
 # from JaCoCo reports in GitHub Actions.
 # 
-# Copyright (c) 2020-2022 Vincent A Cicirello
+# Copyright (c) 2020-2023 Vincent A Cicirello
 # https://www.cicirello.org/
 #
 # MIT License
 # 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
```

### Comparing `jacoco_badge_generator-2.8.1/src/jacoco_badge_generator/__main__.py` & `jacoco_badge_generator-2.9.0/src/jacoco_badge_generator/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # jacoco-badge-generator: Coverage badges, and pull request coverage checks,
 # from JaCoCo reports in GitHub Actions.
 # 
-# Copyright (c) 2020-2022 Vincent A Cicirello
+# Copyright (c) 2020-2023 Vincent A Cicirello
 # https://www.cicirello.org/
 #
 # MIT License
 # 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
@@ -38,15 +38,15 @@
     # such as via a build script, locally (and not via
     # GitHub Actions). The source code for the entry
     # point for GitHub Actions is found at src/entrypoint.py,
     # although please see the project README.md for detailed
     # usage within an GitHub Actions workflow.
 
     print("jacoco-badge-generator: Generate coverage badges from JaCoCo coverage reports")
-    print("Copyright (C) 2022 Vincent A. Cicirello (https://www.cicirello.org/)")
+    print("Copyright (C) 2022-2023 Vincent A. Cicirello (https://www.cicirello.org/)")
     print("MIT License: https://github.com/cicirello/jacoco-badge-generator/blob/main/LICENSE")
     print()
 
     parser = argparse.ArgumentParser(
         prog="jacoco-badge-generator",
         description="Generate coverage badges from JaCoCo coverage reports. All parameters are optional, provided that the defaults meet your use-case."
     )
```

### Comparing `jacoco_badge_generator-2.8.1/src/jacoco_badge_generator/coverage_badges.py` & `jacoco_badge_generator-2.9.0/src/jacoco_badge_generator/coverage_badges.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # jacoco-badge-generator: Coverage badges, and pull request coverage checks,
 # from JaCoCo reports in GitHub Actions.
 # 
-# Copyright (c) 2020-2022 Vincent A Cicirello
+# Copyright (c) 2020-2023 Vincent A Cicirello
 # https://www.cicirello.org/
 #
 # MIT License
 # 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
@@ -29,14 +29,15 @@
 import sys
 import math
 import pathlib
 import os
 import os.path
 import json
 from .text_length import calculateTextLength110
+from glob import glob
 
 badgeTemplate = '<svg xmlns="http://www.w3.org/2000/svg" width="{6}" \
 height="20" role="img" aria-label="{3}: {0}">\
 <linearGradient id="s" x2="0" y2="100%">\
 <stop offset="0" stop-color="#bbb" stop-opacity=".1"/>\
 <stop offset="1" stop-opacity=".1"/></linearGradient><clipPath id="r">\
 <rect width="{6}" height="20" rx="3" fill="#fff"/></clipPath>\
@@ -246,36 +247,40 @@
     elif directory[-1] == "/" :
         return directory + filename
     else :
         return directory + "/" + filename
 
 def filterMissingReports(jacocoFileList, failIfMissing=False) :
     """Validates report file existence, and returns a list
-    containing a subset of the report files that exist. Logs
-    files that don't exist to the console as warnings.
+    containing a subset of the report files that exist and a boolean
+    flag that will be True if any reports were missing or False
+    otherwise. Logs files that don't exist to the console as warnings.
 
     Keyword arguments:
-    jacocoFileList - A list of jacoco.csv files.
+    jacocoFileList - A list of jacoco.csv files or glob patterns specifying such files.
     failIfMissing - If true and if any of the jacoco.csv files
     don't exist, then it will exit with a non-zero exit code causing
     workflow to fail.
     """
     goodReports = []
+    isMissing = False
     for f in jacocoFileList :
-        if os.path.exists(f) :
-            goodReports.append(f)
-        else :
-            print("WARNING: Report file", f, "does not exist.")
+        files = glob(f, recursive=True)
+        for report in files:
+            goodReports.append(report)
+        if len(files) == 0:
+            isMissing = True
+            print("WARNING: Report file", f, "does not exist or glob", f, "is empty.")
     if len(goodReports) == 0 :
         print("WARNING: No JaCoCo csv reports found.")
         if failIfMissing :
             sys.exit(1)
-    if failIfMissing and len(goodReports) != len(jacocoFileList) :
+    if failIfMissing and isMissing :
         sys.exit(1)
-    return goodReports
+    return goodReports, isMissing
 
 def stringToPercentage(s) :
     """Converts a string describing a percentage to
     a float. The string s can be of any of the following
     forms: 60.2%, 60.2, or 0.602. All three of these will
     be treated the same. Without the percent sign, it is
     treated the same as with the percent sign if the value
@@ -573,17 +578,17 @@
         badgesDirectory = badgesDirectory[2:]
     if len(badgesDirectory) > 0 and badgesDirectory[0] == "/" :
         badgesDirectory = badgesDirectory[1:]
     if badgesDirectory == "." :
         badgesDirectory = ""
 
     jacocoFileList = jacocoCsvFile.split()
-    filteredFileList = filterMissingReports(jacocoFileList, onMissingReport=="fail")
+    filteredFileList, isMissing = filterMissingReports(jacocoFileList, onMissingReport=="fail")
     
-    noReportsMissing = len(jacocoFileList)==len(filteredFileList)
+    noReportsMissing = not isMissing
 
     if len(filteredFileList) > 0 and (noReportsMissing or onMissingReport!="quiet") :  
 
         cov, branches = computeCoverage(filteredFileList)
 
         if coverageIsFailing(cov, branches, minCoverage, minBranches) :
             print("Failing the workflow run.")
```

### Comparing `jacoco_badge_generator-2.8.1/src/jacoco_badge_generator/text_length.py` & `jacoco_badge_generator-2.9.0/src/jacoco_badge_generator/text_length.py`

 * *Files identical despite different names*

### Comparing `jacoco_badge_generator-2.8.1/LICENSE` & `jacoco_badge_generator-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jacoco_badge_generator-2.8.1/README.md` & `jacoco_badge_generator-2.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![cicirello/jacoco-badge-generator - Coverage badges, and pull request coverage checks, from JaCoCo reports in GitHub Actions](https://actions.cicirello.org/images/jacoco-badge-generator640.png)](#jacoco-badge-generator)
 
 Check out all of our GitHub Actions: https://actions.cicirello.org/
 
 ## About
 
-| __GitHub Actions__ | [![GitHub release (latest by date)](https://img.shields.io/github/v/release/cicirello/jacoco-badge-generator?label=Marketplace&logo=GitHub)](https://github.com/marketplace/actions/jacoco-badge-generator) [![Count of Action Users](https://badgen.net/github/dependents-repo/cicirello/jacoco-badge-generator?icon=github&label=used%20by)](https://github.com/cicirello/jacoco-badge-generator/network/dependents) |
+| __GitHub Actions__ | [![GitHub release (latest by date)](https://img.shields.io/github/v/release/cicirello/jacoco-badge-generator?label=Marketplace&logo=GitHub)](https://github.com/marketplace/actions/jacoco-badge-generator) [![Count of Action Users](https://img.shields.io/badge/used%20by-repo%20list-informational?logo=github)](https://github.com/cicirello/jacoco-badge-generator/network/dependents?package_id=UGFja2FnZS0yOTQ0NTMxNTI3) |
 | :--- | :--- |
 | __Command-Line Utility__ | [![PyPI](https://img.shields.io/pypi/v/jacoco-badge-generator?logo=pypi)](https://pypi.org/project/jacoco-badge-generator/) [![PyPI Downloads/month](https://static.pepy.tech/personalized-badge/jacoco-badge-generator?period=month&units=international_system&left_color=grey&right_color=blue&left_text=pypi%20downloads/month)](https://pepy.tech/project/jacoco-badge-generator) [![PyPI Downloads/week](https://static.pepy.tech/personalized-badge/jacoco-badge-generator?period=week&units=international_system&left_color=grey&right_color=blue&left_text=pypi%20downloads/week)](https://pepy.tech/project/jacoco-badge-generator) |
 | __Build Status__ | [![build](https://github.com/cicirello/jacoco-badge-generator/actions/workflows/build.yml/badge.svg)](https://github.com/cicirello/jacoco-badge-generator/actions/workflows/build.yml) [![CodeQL](https://github.com/cicirello/jacoco-badge-generator/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/cicirello/jacoco-badge-generator/actions/workflows/codeql-analysis.yml) |
 | __Security__ | [![Snyk security score](https://snyk-widget.herokuapp.com/badge/pip/jacoco-badge-generator/badge.svg)](https://snyk.io/vuln/pip%3Ajacoco-badge-generator) |
 | __Source Info__ | [![License](https://img.shields.io/github/license/cicirello/jacoco-badge-generator)](https://github.com/cicirello/jacoco-badge-generator/blob/main/LICENSE) ![GitHub top language](https://img.shields.io/github/languages/top/cicirello/jacoco-badge-generator) |
 | __Support__ | [![GitHub Sponsors](https://img.shields.io/badge/sponsor-30363D?logo=GitHub-Sponsors&logoColor=#EA4AAA)](https://github.com/sponsors/cicirello) [![Liberapay](https://img.shields.io/badge/Liberapay-F6C915?logo=liberapay&logoColor=black)](https://liberapay.com/cicirello) [![Ko-Fi](https://img.shields.io/badge/Ko--fi-F16061?logo=ko-fi&logoColor=white)](https://ko-fi.com/cicirello) | 
 
@@ -272,14 +272,25 @@
 
 If you have a multi-module project, you can pass the paths (including filenames)
 to all of the `jacoco.csv` files for all of the sub-projects. Separate these by spaces,
 and in particular see the [Multi-Module Example Workflows](#multi-module-example-workflows)
 for an example of how to do this. Multi-module support is limited to cases where
 each module has its own test coverage report, and where those reports don't overlap.
 
+You can also use a glob pattern to specify the set of JaCoCo reports for your modules.
+For example, `jacoco-csv-file: "**/jacoco.csv"` will match all `jacoco.csv` files found
+across all directories within your project. Or for example `jacoco-csv-file: "**/*.csv"`
+will match all `csv` files found within your project, but be careful with such a pattern
+if your project has other `csv` files that are not JaCoCo reports. Or as another example,
+maybe all of your JaCoCo reports are in the same directory, but with names with numbers.
+The pattern `jacoco-csv-file: "target/site/jacoco/module*.csv"` will match all `csv` files
+in the directory `target/site/jacoco/` whose name begins with `module`. Note that in all of 
+these examples you need the quotes around the glob pattern or else GitHub Actions will 
+give you an error that your workflow file is invalid.
+
 The action assumes that all reports passed via this input are 
 independent of each other. If you are using matrix testing, such that 
 each group of tests produces a report, and where the groups overlap in what
 they are testing (e.g., one group tests a portion of a class or method, 
 and another group tests another portion, etc), then the coverage computed by 
 this action will not be correct. The csv reports don't contain enough information
 to properly merge such overlapping reports. If this applies to your use-case, then
@@ -552,15 +563,15 @@
 
 ```XML
 <build>
   <plugins>
     <plugin>
       <groupId>org.jacoco</groupId>
       <artifactId>jacoco-maven-plugin</artifactId>
-      <version>0.8.8</version>
+      <version>0.8.10</version>
       <executions>
         <execution>
           <goals>
             <goal>prepare-agent</goal>
           </goals>
         </execution>
         <execution>
@@ -574,15 +585,15 @@
       </plugin>
   </plugins>
 </build>
 ```
 
 Note that the jacoco-badge-generator action has been tested with
 the `jacoco.csv` files generated by `jacoco-maven-plugin` versions
-0.8.6 through 0.8.8, and has not been tested with earlier versions
+0.8.6 through 0.8.10, and has not been tested with earlier versions
 of JaCoCo.
 
 ##### Running JaCoCo via Gradle
 
 If you use gradle as your build tool, then you can configure JaCoCo
 in `build.gradle.kts` with:
 
@@ -644,15 +655,15 @@
           jacoco-csv-file: build/reports/jacoco/test/jacocoTestReport.csv
 ```
 
 You can also use a specific release with:
 
 ```yml
     - name: Generate JaCoCo Badge
-      uses: cicirello/jacoco-badge-generator@v2.8.0
+      uses: cicirello/jacoco-badge-generator@v2.9.0
       with:
         generate-branches-badge: true
 ```
 
 #### All Possible Action Inputs
 
 This shows a workflow step that uses all of the
@@ -724,15 +735,15 @@
 
     steps:
     - uses: actions/checkout@v2
 
     - name: Set up the Java JDK
       uses: actions/setup-java@v2
       with:
-        java-version: '11'
+        java-version: '17'
         distribution: 'adopt'
 
     - name: Build with Maven
       run: mvn -B test
 
     - name: Generate JaCoCo Badge
       id: jacoco
@@ -782,15 +793,15 @@
 
     steps:
     - uses: actions/checkout@v2
 
     - name: Set up the Java JDK
       uses: actions/setup-java@v2
       with:
-        java-version: '11'
+        java-version: '17'
         distribution: 'adopt'
 
     - name: Build with Maven
       run: mvn -B test
 
     - name: Generate JaCoCo Badge
       id: jacoco
@@ -842,15 +853,15 @@
 
     steps:
     - uses: actions/checkout@v2
 
     - name: Set up the Java JDK
       uses: actions/setup-java@v2
       with:
-        java-version: '11'
+        java-version: '17'
         distribution: 'adopt'
 
     - name: Build with Maven
       run: mvn -B test
 
     - name: Generate JaCoCo Badge
       id: jacoco
@@ -874,15 +885,70 @@
           git config --global user.email 'YOUR-GITHUB-USERID@users.noreply.github.com'
           git add -A
           git commit -m "Autogenerated JaCoCo coverage badge"
           git push
         fi
 ```
 
-#### Example Workflow 4: Multi-Module Project with Separate Badges for Each Module.
+#### Example Workflow 4: Glob Pattern to Specify Reports of a Multi-Module Project.
+
+This example workflow uses a glob pattern to specify the reports of a multi-module project,
+and generates both badges (instructions coverage percentage and branches coverage percentage). 
+The badges that are generated are computed over all modules. In this example, all of the JaCoCo
+reports are named `jacoco.csv` but reside in different directories. You can match all of them
+with `jacoco-csv-file: "**/jacoco.csv"`. The quotes around the glob are required to avoid an
+invalid workflow error from GitHub Actions.
+
+```yml
+name: build
+
+on:
+  push:
+    branches: [ main ]
+
+jobs:
+  build:
+    runs-on: ubuntu-latest
+
+    steps:
+    - uses: actions/checkout@v2
+
+    - name: Set up the Java JDK
+      uses: actions/setup-java@v2
+      with:
+        java-version: '17'
+        distribution: 'adopt'
+
+    - name: Build with Maven
+      run: mvn -B test
+
+    - name: Generate JaCoCo Badge
+      id: jacoco
+      uses: cicirello/jacoco-badge-generator@v2
+      with:
+        generate-branches-badge: true
+        jacoco-csv-file: "**/jacoco.csv"
+
+    - name: Log coverage percentage
+      run: |
+        echo "coverage = ${{ steps.jacoco.outputs.coverage }}"
+        echo "branch coverage = ${{ steps.jacoco.outputs.branches }}"
+
+    - name: Commit the badge (if it changed)
+      run: |
+        if [[ `git status --porcelain` ]]; then
+          git config --global user.name 'YOUR NAME HERE'
+          git config --global user.email 'YOUR-GITHUB-USERID@users.noreply.github.com'
+          git add -A
+          git commit -m "Autogenerated JaCoCo coverage badge"
+          git push
+        fi
+```
+
+#### Example Workflow 5: Multi-Module Project with Separate Badges for Each Module.
 
 If you would prefer to generate separate coverage badges for each of the
 modules of a multi-module project, then just include multiple steps of the
 `jacoco-badge-generator` in your workflow, such as in this example. Be sure to use
 the inputs to specify names for the badge files, otherwise with the defaults
 the subsequent steps will overwrite the previous. This example assumes that there
 are two modules. You also will likely want to use the `coverage-label` and `branches-label`
@@ -903,15 +969,15 @@
 
     steps:
     - uses: actions/checkout@v2
 
     - name: Set up the Java JDK
       uses: actions/setup-java@v2
       with:
-        java-version: '11'
+        java-version: '17'
         distribution: 'adopt'
 
     - name: Build with Maven
       run: mvn -B test
 
     - name: Generate JaCoCo Badges for Module 1
       id: jacocoMod1
@@ -1107,14 +1173,26 @@
 they are independent), then you can specify the locations and names of all of the report files with
 something like:
 
 ```Shell
 python3 -m jacoco_badge_generator --jacoco-csv-file reports/report1.csv reports/report2.csv
 ```
 
+In CLI mode, glob patterns will be handled by your shell. You can accomplish the above with:
+
+```Shell
+python3 -m jacoco_badge_generator --jacoco-csv-file reports/report*.csv
+```
+
+Or perhaps all of your reports are named `jacoco.csv` but in different directories, then you can
+match all of them with:
+
+```Shell
+python3 -m jacoco_badge_generator --jacoco-csv-file **/jacoco.csv
+```
 
 ## Summary of Input Defaults
 
 The following table summarizes the default values of all inputs for both the GitHub Actions
 usage as well as the CLI usage. If your use-case requires the defaults as specified below, then
 you do not need to include them.
 
@@ -1141,14 +1219,15 @@
 | `fail-if-branches-less-than: 0` | `--fail-if-branches-less-than 0` |
 | `fail-on-coverage-decrease: false` | `--fail-on-coverage-decrease false` |
 | `fail-on-branches-decrease: false` | `--fail-on-branches-decrease false` |
 
 ## Blog Posts
 
 Here is a selection of blog posts about the jacoco-badge-generator on DEV.to:
+* [Using GitHub Actions to Build a Java Project With Pull Request Coverage Commenting and Coverage Badges](https://dev.to/cicirello/using-github-actions-to-build-a-java-project-with-pull-request-coverage-commenting-and-coverage-badges-50a2), posted on DEV on November 9, 2022.
 * [The jacoco-badge-generator GitHub Action is now also available as a CLI tool from PyPI](https://dev.to/cicirello/the-jacoco-badge-generator-github-action-is-now-also-available-as-a-cli-tool-from-pypi-3ma0), posted on DEV on July 8, 2022.
 * [JaCoCo coverage badges, PR coverage checks, and PR coverage comments, from GitHub Actions](https://dev.to/cicirello/jacoco-coverage-badges-pr-coverage-checks-and-pr-coverage-comments-from-github-actions-4a8f), posted on DEV on November 29, 2021.
 
 ## Support the Project
 
 You can support the project in a number of ways:
 * __Starring__: If you find the `jacoco-badge-generator` action
```

### Comparing `jacoco_badge_generator-2.8.1/pyproject.toml` & `jacoco_badge_generator-2.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jacoco-badge-generator"
-version = "2.8.1"
+version = "2.9.0"
 authors = [
   { name="Vincent A. Cicirello", email="development@cicirello.org" },
 ]
 description = "JaCoCo coverage badges (SVG format), and coverage checks (e.g., decreasing coverage and minimum coverage)"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -42,11 +42,12 @@
 "Changelog" = "https://github.com/cicirello/jacoco-badge-generator/blob/main/CHANGELOG.md"
 
 [tool.hatch.build]
 exclude = [
     "/.github",
     "/images",
     "/src/entrypoint.py",
+    "/tests",
     "/.dockerignore",
     "/action.yml",
     "/Dockerfile",
 ]
```

### Comparing `jacoco_badge_generator-2.8.1/PKG-INFO` & `jacoco_badge_generator-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jacoco-badge-generator
-Version: 2.8.1
+Version: 2.9.0
 Summary: JaCoCo coverage badges (SVG format), and coverage checks (e.g., decreasing coverage and minimum coverage)
 Project-URL: Information Page, https://actions.cicirello.org/jacoco-badge-generator/
 Project-URL: GitHub Repository, https://github.com/cicirello/jacoco-badge-generator
 Project-URL: Bug Tracker, https://github.com/cicirello/jacoco-badge-generator/issues
 Project-URL: Changelog, https://github.com/cicirello/jacoco-badge-generator/blob/main/CHANGELOG.md
 Author-email: "Vincent A. Cicirello" <development@cicirello.org>
 License-File: LICENSE
@@ -21,15 +21,15 @@
 
 [![cicirello/jacoco-badge-generator - Coverage badges, and pull request coverage checks, from JaCoCo reports in GitHub Actions](https://actions.cicirello.org/images/jacoco-badge-generator640.png)](#jacoco-badge-generator)
 
 Check out all of our GitHub Actions: https://actions.cicirello.org/
 
 ## About
 
-| __GitHub Actions__ | [![GitHub release (latest by date)](https://img.shields.io/github/v/release/cicirello/jacoco-badge-generator?label=Marketplace&logo=GitHub)](https://github.com/marketplace/actions/jacoco-badge-generator) [![Count of Action Users](https://badgen.net/github/dependents-repo/cicirello/jacoco-badge-generator?icon=github&label=used%20by)](https://github.com/cicirello/jacoco-badge-generator/network/dependents) |
+| __GitHub Actions__ | [![GitHub release (latest by date)](https://img.shields.io/github/v/release/cicirello/jacoco-badge-generator?label=Marketplace&logo=GitHub)](https://github.com/marketplace/actions/jacoco-badge-generator) [![Count of Action Users](https://img.shields.io/badge/used%20by-repo%20list-informational?logo=github)](https://github.com/cicirello/jacoco-badge-generator/network/dependents?package_id=UGFja2FnZS0yOTQ0NTMxNTI3) |
 | :--- | :--- |
 | __Command-Line Utility__ | [![PyPI](https://img.shields.io/pypi/v/jacoco-badge-generator?logo=pypi)](https://pypi.org/project/jacoco-badge-generator/) [![PyPI Downloads/month](https://static.pepy.tech/personalized-badge/jacoco-badge-generator?period=month&units=international_system&left_color=grey&right_color=blue&left_text=pypi%20downloads/month)](https://pepy.tech/project/jacoco-badge-generator) [![PyPI Downloads/week](https://static.pepy.tech/personalized-badge/jacoco-badge-generator?period=week&units=international_system&left_color=grey&right_color=blue&left_text=pypi%20downloads/week)](https://pepy.tech/project/jacoco-badge-generator) |
 | __Build Status__ | [![build](https://github.com/cicirello/jacoco-badge-generator/actions/workflows/build.yml/badge.svg)](https://github.com/cicirello/jacoco-badge-generator/actions/workflows/build.yml) [![CodeQL](https://github.com/cicirello/jacoco-badge-generator/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/cicirello/jacoco-badge-generator/actions/workflows/codeql-analysis.yml) |
 | __Security__ | [![Snyk security score](https://snyk-widget.herokuapp.com/badge/pip/jacoco-badge-generator/badge.svg)](https://snyk.io/vuln/pip%3Ajacoco-badge-generator) |
 | __Source Info__ | [![License](https://img.shields.io/github/license/cicirello/jacoco-badge-generator)](https://github.com/cicirello/jacoco-badge-generator/blob/main/LICENSE) ![GitHub top language](https://img.shields.io/github/languages/top/cicirello/jacoco-badge-generator) |
 | __Support__ | [![GitHub Sponsors](https://img.shields.io/badge/sponsor-30363D?logo=GitHub-Sponsors&logoColor=#EA4AAA)](https://github.com/sponsors/cicirello) [![Liberapay](https://img.shields.io/badge/Liberapay-F6C915?logo=liberapay&logoColor=black)](https://liberapay.com/cicirello) [![Ko-Fi](https://img.shields.io/badge/Ko--fi-F16061?logo=ko-fi&logoColor=white)](https://ko-fi.com/cicirello) | 
 
@@ -291,14 +291,25 @@
 
 If you have a multi-module project, you can pass the paths (including filenames)
 to all of the `jacoco.csv` files for all of the sub-projects. Separate these by spaces,
 and in particular see the [Multi-Module Example Workflows](#multi-module-example-workflows)
 for an example of how to do this. Multi-module support is limited to cases where
 each module has its own test coverage report, and where those reports don't overlap.
 
+You can also use a glob pattern to specify the set of JaCoCo reports for your modules.
+For example, `jacoco-csv-file: "**/jacoco.csv"` will match all `jacoco.csv` files found
+across all directories within your project. Or for example `jacoco-csv-file: "**/*.csv"`
+will match all `csv` files found within your project, but be careful with such a pattern
+if your project has other `csv` files that are not JaCoCo reports. Or as another example,
+maybe all of your JaCoCo reports are in the same directory, but with names with numbers.
+The pattern `jacoco-csv-file: "target/site/jacoco/module*.csv"` will match all `csv` files
+in the directory `target/site/jacoco/` whose name begins with `module`. Note that in all of 
+these examples you need the quotes around the glob pattern or else GitHub Actions will 
+give you an error that your workflow file is invalid.
+
 The action assumes that all reports passed via this input are 
 independent of each other. If you are using matrix testing, such that 
 each group of tests produces a report, and where the groups overlap in what
 they are testing (e.g., one group tests a portion of a class or method, 
 and another group tests another portion, etc), then the coverage computed by 
 this action will not be correct. The csv reports don't contain enough information
 to properly merge such overlapping reports. If this applies to your use-case, then
@@ -571,15 +582,15 @@
 
 ```XML
 <build>
   <plugins>
     <plugin>
       <groupId>org.jacoco</groupId>
       <artifactId>jacoco-maven-plugin</artifactId>
-      <version>0.8.8</version>
+      <version>0.8.10</version>
       <executions>
         <execution>
           <goals>
             <goal>prepare-agent</goal>
           </goals>
         </execution>
         <execution>
@@ -593,15 +604,15 @@
       </plugin>
   </plugins>
 </build>
 ```
 
 Note that the jacoco-badge-generator action has been tested with
 the `jacoco.csv` files generated by `jacoco-maven-plugin` versions
-0.8.6 through 0.8.8, and has not been tested with earlier versions
+0.8.6 through 0.8.10, and has not been tested with earlier versions
 of JaCoCo.
 
 ##### Running JaCoCo via Gradle
 
 If you use gradle as your build tool, then you can configure JaCoCo
 in `build.gradle.kts` with:
 
@@ -663,15 +674,15 @@
           jacoco-csv-file: build/reports/jacoco/test/jacocoTestReport.csv
 ```
 
 You can also use a specific release with:
 
 ```yml
     - name: Generate JaCoCo Badge
-      uses: cicirello/jacoco-badge-generator@v2.8.0
+      uses: cicirello/jacoco-badge-generator@v2.9.0
       with:
         generate-branches-badge: true
 ```
 
 #### All Possible Action Inputs
 
 This shows a workflow step that uses all of the
@@ -743,15 +754,15 @@
 
     steps:
     - uses: actions/checkout@v2
 
     - name: Set up the Java JDK
       uses: actions/setup-java@v2
       with:
-        java-version: '11'
+        java-version: '17'
         distribution: 'adopt'
 
     - name: Build with Maven
       run: mvn -B test
 
     - name: Generate JaCoCo Badge
       id: jacoco
@@ -801,15 +812,15 @@
 
     steps:
     - uses: actions/checkout@v2
 
     - name: Set up the Java JDK
       uses: actions/setup-java@v2
       with:
-        java-version: '11'
+        java-version: '17'
         distribution: 'adopt'
 
     - name: Build with Maven
       run: mvn -B test
 
     - name: Generate JaCoCo Badge
       id: jacoco
@@ -861,15 +872,15 @@
 
     steps:
     - uses: actions/checkout@v2
 
     - name: Set up the Java JDK
       uses: actions/setup-java@v2
       with:
-        java-version: '11'
+        java-version: '17'
         distribution: 'adopt'
 
     - name: Build with Maven
       run: mvn -B test
 
     - name: Generate JaCoCo Badge
       id: jacoco
@@ -893,15 +904,70 @@
           git config --global user.email 'YOUR-GITHUB-USERID@users.noreply.github.com'
           git add -A
           git commit -m "Autogenerated JaCoCo coverage badge"
           git push
         fi
 ```
 
-#### Example Workflow 4: Multi-Module Project with Separate Badges for Each Module.
+#### Example Workflow 4: Glob Pattern to Specify Reports of a Multi-Module Project.
+
+This example workflow uses a glob pattern to specify the reports of a multi-module project,
+and generates both badges (instructions coverage percentage and branches coverage percentage). 
+The badges that are generated are computed over all modules. In this example, all of the JaCoCo
+reports are named `jacoco.csv` but reside in different directories. You can match all of them
+with `jacoco-csv-file: "**/jacoco.csv"`. The quotes around the glob are required to avoid an
+invalid workflow error from GitHub Actions.
+
+```yml
+name: build
+
+on:
+  push:
+    branches: [ main ]
+
+jobs:
+  build:
+    runs-on: ubuntu-latest
+
+    steps:
+    - uses: actions/checkout@v2
+
+    - name: Set up the Java JDK
+      uses: actions/setup-java@v2
+      with:
+        java-version: '17'
+        distribution: 'adopt'
+
+    - name: Build with Maven
+      run: mvn -B test
+
+    - name: Generate JaCoCo Badge
+      id: jacoco
+      uses: cicirello/jacoco-badge-generator@v2
+      with:
+        generate-branches-badge: true
+        jacoco-csv-file: "**/jacoco.csv"
+
+    - name: Log coverage percentage
+      run: |
+        echo "coverage = ${{ steps.jacoco.outputs.coverage }}"
+        echo "branch coverage = ${{ steps.jacoco.outputs.branches }}"
+
+    - name: Commit the badge (if it changed)
+      run: |
+        if [[ `git status --porcelain` ]]; then
+          git config --global user.name 'YOUR NAME HERE'
+          git config --global user.email 'YOUR-GITHUB-USERID@users.noreply.github.com'
+          git add -A
+          git commit -m "Autogenerated JaCoCo coverage badge"
+          git push
+        fi
+```
+
+#### Example Workflow 5: Multi-Module Project with Separate Badges for Each Module.
 
 If you would prefer to generate separate coverage badges for each of the
 modules of a multi-module project, then just include multiple steps of the
 `jacoco-badge-generator` in your workflow, such as in this example. Be sure to use
 the inputs to specify names for the badge files, otherwise with the defaults
 the subsequent steps will overwrite the previous. This example assumes that there
 are two modules. You also will likely want to use the `coverage-label` and `branches-label`
@@ -922,15 +988,15 @@
 
     steps:
     - uses: actions/checkout@v2
 
     - name: Set up the Java JDK
       uses: actions/setup-java@v2
       with:
-        java-version: '11'
+        java-version: '17'
         distribution: 'adopt'
 
     - name: Build with Maven
       run: mvn -B test
 
     - name: Generate JaCoCo Badges for Module 1
       id: jacocoMod1
@@ -1126,14 +1192,26 @@
 they are independent), then you can specify the locations and names of all of the report files with
 something like:
 
 ```Shell
 python3 -m jacoco_badge_generator --jacoco-csv-file reports/report1.csv reports/report2.csv
 ```
 
+In CLI mode, glob patterns will be handled by your shell. You can accomplish the above with:
+
+```Shell
+python3 -m jacoco_badge_generator --jacoco-csv-file reports/report*.csv
+```
+
+Or perhaps all of your reports are named `jacoco.csv` but in different directories, then you can
+match all of them with:
+
+```Shell
+python3 -m jacoco_badge_generator --jacoco-csv-file **/jacoco.csv
+```
 
 ## Summary of Input Defaults
 
 The following table summarizes the default values of all inputs for both the GitHub Actions
 usage as well as the CLI usage. If your use-case requires the defaults as specified below, then
 you do not need to include them.
 
@@ -1160,14 +1238,15 @@
 | `fail-if-branches-less-than: 0` | `--fail-if-branches-less-than 0` |
 | `fail-on-coverage-decrease: false` | `--fail-on-coverage-decrease false` |
 | `fail-on-branches-decrease: false` | `--fail-on-branches-decrease false` |
 
 ## Blog Posts
 
 Here is a selection of blog posts about the jacoco-badge-generator on DEV.to:
+* [Using GitHub Actions to Build a Java Project With Pull Request Coverage Commenting and Coverage Badges](https://dev.to/cicirello/using-github-actions-to-build-a-java-project-with-pull-request-coverage-commenting-and-coverage-badges-50a2), posted on DEV on November 9, 2022.
 * [The jacoco-badge-generator GitHub Action is now also available as a CLI tool from PyPI](https://dev.to/cicirello/the-jacoco-badge-generator-github-action-is-now-also-available-as-a-cli-tool-from-pypi-3ma0), posted on DEV on July 8, 2022.
 * [JaCoCo coverage badges, PR coverage checks, and PR coverage comments, from GitHub Actions](https://dev.to/cicirello/jacoco-coverage-badges-pr-coverage-checks-and-pr-coverage-comments-from-github-actions-4a8f), posted on DEV on November 29, 2021.
 
 ## Support the Project
 
 You can support the project in a number of ways:
 * __Starring__: If you find the `jacoco-badge-generator` action
```

