# Comparing `tmp/devstats-0.1rc0.tar.gz` & `tmp/devstats-0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devstats-0.1rc0.tar", last modified: Mon May 22 23:49:37 2023, max compression
+gzip compressed data, was "devstats-0.1rc1.tar", last modified: Wed May 24 17:35:32 2023, max compression
```

## Comparing `devstats-0.1rc0.tar` & `devstats-0.1rc1.tar`

### file list

```diff
@@ -1,15 +1,23 @@
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-22 23:49:37.615142 devstats-0.1rc0/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1504 2023-05-22 22:53:17.000000 devstats-0.1rc0/LICENSE
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2147 2023-05-22 23:49:37.615142 devstats-0.1rc0/PKG-INFO
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)       11 2023-05-22 23:43:36.000000 devstats-0.1rc0/README.md
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-22 23:49:37.613142 devstats-0.1rc0/devstats/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     7011 2023-05-22 23:43:36.000000 devstats-0.1rc0/devstats/__init__.py
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-22 23:49:37.615142 devstats-0.1rc0/devstats.egg-info/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2147 2023-05-22 23:49:37.000000 devstats-0.1rc0/devstats.egg-info/PKG-INFO
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      247 2023-05-22 23:49:37.000000 devstats-0.1rc0/devstats.egg-info/SOURCES.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)        1 2023-05-22 23:49:37.000000 devstats-0.1rc0/devstats.egg-info/dependency_links.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)       52 2023-05-22 23:49:37.000000 devstats-0.1rc0/devstats.egg-info/entry_points.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)       73 2023-05-22 23:49:37.000000 devstats-0.1rc0/devstats.egg-info/requires.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)        9 2023-05-22 23:49:37.000000 devstats-0.1rc0/devstats.egg-info/top_level.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      793 2023-05-22 23:44:14.000000 devstats-0.1rc0/pyproject.toml
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)       38 2023-05-22 23:49:37.615142 devstats-0.1rc0/setup.cfg
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-24 17:35:32.632254 devstats-0.1rc1/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1504 2023-05-22 22:53:17.000000 devstats-0.1rc1/LICENSE
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2147 2023-05-24 17:35:32.632254 devstats-0.1rc1/PKG-INFO
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1203 2023-05-23 20:04:35.000000 devstats-0.1rc1/README.md
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-24 17:35:32.630254 devstats-0.1rc1/devstats/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)        0 2023-05-24 00:27:42.000000 devstats-0.1rc1/devstats/__init__.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1764 2023-05-24 17:33:45.000000 devstats-0.1rc1/devstats/__main__.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      494 2023-05-24 17:33:45.000000 devstats-0.1rc1/devstats/publish.py
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-24 17:35:32.631254 devstats-0.1rc1/devstats/queries/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1453 2023-05-24 00:22:14.000000 devstats-0.1rc1/devstats/queries/issue_activity_since_date.gql
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      582 2023-05-24 00:22:14.000000 devstats-0.1rc1/devstats/queries/pr_data_query.gql
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     6364 2023-05-24 16:58:50.000000 devstats-0.1rc1/devstats/query.py
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-24 17:35:32.631254 devstats-0.1rc1/devstats/reports/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    17738 2023-05-24 17:33:45.000000 devstats-0.1rc1/devstats/reports/analysis_template.md
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-24 17:35:32.631254 devstats-0.1rc1/devstats.egg-info/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2147 2023-05-24 17:35:32.000000 devstats-0.1rc1/devstats.egg-info/PKG-INFO
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      426 2023-05-24 17:35:32.000000 devstats-0.1rc1/devstats.egg-info/SOURCES.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)        1 2023-05-24 17:35:32.000000 devstats-0.1rc1/devstats.egg-info/dependency_links.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       51 2023-05-24 17:35:32.000000 devstats-0.1rc1/devstats.egg-info/entry_points.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       73 2023-05-24 17:35:32.000000 devstats-0.1rc1/devstats.egg-info/requires.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)        9 2023-05-24 17:35:32.000000 devstats-0.1rc1/devstats.egg-info/top_level.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      848 2023-05-24 17:33:52.000000 devstats-0.1rc1/pyproject.toml
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       38 2023-05-24 17:35:32.632254 devstats-0.1rc1/setup.cfg
```

### Comparing `devstats-0.1rc0/LICENSE` & `devstats-0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `devstats-0.1rc0/PKG-INFO` & `devstats-0.1rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devstats
-Version: 0.1rc0
+Version: 0.1rc1
 Summary: Developer tool for scientific Python libraries
 Maintainer-email: Scientific Python <devstats@discuss.scientific-python.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Scientific Python
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `devstats-0.1rc0/devstats/__init__.py` & `devstats-0.1rc1/devstats/query.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,16 @@
+import json
 import os
-import requests
+import re
 import sys
-import json
-import click
+from glob import glob
 
-try:
-    token = os.environ["GRAPH_API_KEY"]
-except KeyError:
-    print("You need to set GRAPH_API_KEY")
-    print("But you shouldn't use this yet.")
-    sys.exit()
+import requests
 
 endpoint = r"https://api.github.com/graphql"
-headers = {"Authorization": f"bearer {token}"}
 
 
 def load_query_from_file(fname, repo_owner="numpy", repo_name="numpy"):
     """
     Load an 'issue' query from file and set the target repository, where
     the target repository has the format:
 
@@ -47,28 +41,30 @@
         query = fh.read()
         # Set target repo from template
         query = query.replace("_REPO_OWNER_", repo_owner)
         query = query.replace("_REPO_NAME_", repo_name)
     return query
 
 
-def send_query(query, query_type, cursor=None):
+def send_query(query, query_type, headers, cursor=None):
     """
     Send a GraphQL query via requests.post
 
     No validation is done on the query before sending. GitHub GraphQL is
     supported with the `cursor` argument.
 
     Parameters
     ----------
     query : str
         The GraphQL query to be sent
     query_type : {"issues", "pullRequests"}
         The object being queried according to the GitHub GraphQL schema.
         Currently only issues and pullRequests are supported
+    headers : dict
+        Contains authorization token
     cursor : str, optional
         If given, then the cursor is injected into the query to support
         GitHub's GraphQL pagination.
 
     Returns
     -------
     dict
@@ -93,29 +89,34 @@
         query = query[:cursor_ind] + f'after:"{cursor}", ' + query[cursor_ind:]
     # Build request payload
     payload = {"query": "".join(query.split("\n"))}
     response = requests.post(endpoint, json=payload, headers=headers)
     return json.loads(response.content)
 
 
-def get_all_responses(query, query_type):
+def get_all_responses(query, query_type, headers):
     """
     Helper function to bypass GitHub GraphQL API node limit.
     """
     # Get data from a single response
-    initial_data = send_query(query, query_type)
+    print(f"Retrieving first page...", end="", flush=True)
+    initial_data = send_query(query, query_type, headers)
     data, last_cursor, total_count = parse_single_query(initial_data, query_type)
-    print(f"Retrieving {len(data)} out of {total_count} values...")
+
     # Continue requesting data (with pagination) until all are acquired
     while len(data) < total_count:
-        rdata = send_query(query, query_type, cursor=last_cursor)
+        rdata = send_query(query, query_type, headers, cursor=last_cursor)
         pdata, last_cursor, _ = parse_single_query(rdata, query_type)
         data.extend(pdata)
-        print(f"Retrieving {len(data)} out of {total_count} values...")
-    print("Done.")
+        print(
+            f"OK\nRetrieving {len(data)} out of {total_count} values...",
+            end="",
+            flush=True,
+        )
+    print("OK")
     return data
 
 
 def parse_single_query(data, query_type):
     """
     Parse the data returned by `send_query`
 
@@ -136,15 +137,17 @@
 
 
 class GithubGrabber:
     """
     Pull down data via the GitHub APIv.4 given a valid GraphQL query.
     """
 
-    def __init__(self, query_fname, query_type, repo_owner="numpy", repo_name="numpy"):
+    def __init__(
+        self, query_fname, query_type, headers, repo_owner="numpy", repo_name="numpy"
+    ):
         """
         Create an object to send/recv queries related to the issue tracker
         for the given repository via the GitHub API v.4.
 
         The repository to query against is given by:
         https://github.com/<repo_owner>/<repo_name>
 
@@ -159,61 +162,34 @@
         repo_owner : str
             Repository owner. Default is "numpy"
         repo_name : str
             Repository name. Default is "numpy"
         """
         self.query_fname = query_fname
         self.query_type = query_type  # TODO: Parse this directly from query
+        self.headers = headers
         self.repo_owner = repo_owner
         self.repo_name = repo_name
         self.raw_data = None
         self.load_query()
 
     def load_query(self):
         self.query = load_query_from_file(
             self.query_fname, self.repo_owner, self.repo_name
         )
 
     def get(self):
         """
         Get JSON-formatted raw data from the query.
         """
-        self.raw_data = get_all_responses(self.query, self.query_type)
+        self.raw_data = get_all_responses(self.query, self.query_type, self.headers)
 
     def dump(self, outfile):
         """
         Dump raw json to `outfile`.
         """
         if not self.raw_data:
             raise ValueError("raw_data is currently empty, nothing to dump")
 
         with open(outfile, "w") as outf:
+            print(f"Writing [{outfile}]")
             json.dump(self.raw_data, outf)
-
-
-@click.command()
-@click.argument("repo_owner")
-@click.argument("repo_name")
-def main(repo_owner, repo_name):
-    """Download and save issue and pr data for `repo_owner`/`repo_name`."""
-    # Download issue data
-    issues = GithubGrabber(
-        "query_examples/issue_activity_since_date.gql",
-        "issues",
-        repo_owner=repo_owner,
-        repo_name=repo_name,
-    )
-    issues.get()
-    issues.dump(f"{repo_name}_issues.json")
-    # Download PR data
-    prs = GithubGrabber(
-        "query_examples/pr_data_query.gql",
-        "pullRequests",
-        repo_owner=repo_owner,
-        repo_name=repo_name,
-    )
-    prs.get()
-    prs.dump(f"{repo_name}_prs.json")
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `devstats-0.1rc0/devstats.egg-info/PKG-INFO` & `devstats-0.1rc1/devstats.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devstats
-Version: 0.1rc0
+Version: 0.1rc1
 Summary: Developer tool for scientific Python libraries
 Maintainer-email: Scientific Python <devstats@discuss.scientific-python.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Scientific Python
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `devstats-0.1rc0/pyproject.toml` & `devstats-0.1rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "devstats"
-version = "0.1rc0"
+version = "0.1rc1"
 requires-python = ">=3.10"
 description = "Developer tool for scientific Python libraries"
 license = {file = "LICENSE"}
 maintainers = [
   {name = "Scientific Python", email = "devstats@discuss.scientific-python.org"}
 ]
 classifiers = [
@@ -21,17 +21,20 @@
   "jupyter",
   "notebook",
   "numpy",
   "networkx",
 ]
 
 [project.scripts]
-devstats = "devstats.__main__:main"
+devstats = "devstats.__main__:cli"
 
 [project.optional-dependencies]
-lint = ["pre-commit >= 3.r32"]
+lint = ["pre-commit >= 3.3.2"]
 
 [project.urls]
 homepage = "https://github.com/scientific-python/devstats"
 
 [tool.setuptools.packages.find]
 include = ["devstats*"]
+
+[tool.setuptools.package-data]
+"*" = ["*.gql", "*.md"]
```

