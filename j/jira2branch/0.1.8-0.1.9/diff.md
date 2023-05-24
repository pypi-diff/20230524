# Comparing `tmp/jira2branch-0.1.8.tar.gz` & `tmp/jira2branch-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jira2branch-0.1.8.tar", last modified: Thu Sep 23 11:14:02 2021, max compression
+gzip compressed data, was "jira2branch-0.1.9.tar", last modified: Thu Sep 23 13:35:39 2021, max compression
```

## Comparing `jira2branch-0.1.8.tar` & `jira2branch-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tiagoafpereira  (1000) tiagoafpereira  (1000)        0 2021-09-23 11:14:02.184682 jira2branch-0.1.8/
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)     1833 2021-09-23 11:14:02.184682 jira2branch-0.1.8/PKG-INFO
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)     1418 2021-09-23 11:13:26.000000 jira2branch-0.1.8/README.md
-drwxr-xr-x   0 tiagoafpereira  (1000) tiagoafpereira  (1000)        0 2021-09-23 11:14:02.184682 jira2branch-0.1.8/jira2branch/
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)       74 2021-09-23 11:11:15.000000 jira2branch-0.1.8/jira2branch/__init__.py
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)     9918 2021-09-23 11:12:58.000000 jira2branch-0.1.8/jira2branch/__main__.py
-drwxr-xr-x   0 tiagoafpereira  (1000) tiagoafpereira  (1000)        0 2021-09-23 11:14:02.184682 jira2branch-0.1.8/jira2branch/tests/
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)        0 2021-09-09 15:20:22.000000 jira2branch-0.1.8/jira2branch/tests/__init__.py
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)      838 2021-09-09 15:18:35.000000 jira2branch-0.1.8/jira2branch/tests/test_main.py
-drwxr-xr-x   0 tiagoafpereira  (1000) tiagoafpereira  (1000)        0 2021-09-23 11:14:02.184682 jira2branch-0.1.8/jira2branch.egg-info/
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)     1833 2021-09-23 11:14:02.000000 jira2branch-0.1.8/jira2branch.egg-info/PKG-INFO
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)      339 2021-09-23 11:14:02.000000 jira2branch-0.1.8/jira2branch.egg-info/SOURCES.txt
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)        1 2021-09-23 11:14:02.000000 jira2branch-0.1.8/jira2branch.egg-info/dependency_links.txt
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)       58 2021-09-23 11:14:02.000000 jira2branch-0.1.8/jira2branch.egg-info/entry_points.txt
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)       36 2021-09-23 11:14:02.000000 jira2branch-0.1.8/jira2branch.egg-info/requires.txt
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)       12 2021-09-23 11:14:02.000000 jira2branch-0.1.8/jira2branch.egg-info/top_level.txt
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)       38 2021-09-23 11:14:02.184682 jira2branch-0.1.8/setup.cfg
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)     1052 2021-09-23 11:11:15.000000 jira2branch-0.1.8/setup.py
+drwxr-xr-x   0 tiagoafpereira  (1000) tiagoafpereira  (1000)        0 2021-09-23 13:35:39.155202 jira2branch-0.1.9/
+-rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)     1833 2021-09-23 13:35:39.155202 jira2branch-0.1.9/PKG-INFO
+-rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)     1418 2021-09-23 11:13:26.000000 jira2branch-0.1.9/README.md
+drwxr-xr-x   0 tiagoafpereira  (1000) tiagoafpereira  (1000)        0 2021-09-23 13:35:39.155202 jira2branch-0.1.9/jira2branch/
+-rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)       74 2021-09-23 13:10:10.000000 jira2branch-0.1.9/jira2branch/__init__.py
+-rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)    10236 2021-09-23 13:35:22.000000 jira2branch-0.1.9/jira2branch/__main__.py
+drwxr-xr-x   0 tiagoafpereira  (1000) tiagoafpereira  (1000)        0 2021-09-23 13:35:39.155202 jira2branch-0.1.9/jira2branch/tests/
+-rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)        0 2021-09-09 15:20:22.000000 jira2branch-0.1.9/jira2branch/tests/__init__.py
+-rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)      838 2021-09-09 15:18:35.000000 jira2branch-0.1.9/jira2branch/tests/test_main.py
+drwxr-xr-x   0 tiagoafpereira  (1000) tiagoafpereira  (1000)        0 2021-09-23 13:35:39.155202 jira2branch-0.1.9/jira2branch.egg-info/
+-rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)     1833 2021-09-23 13:35:39.000000 jira2branch-0.1.9/jira2branch.egg-info/PKG-INFO
+-rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)      339 2021-09-23 13:35:39.000000 jira2branch-0.1.9/jira2branch.egg-info/SOURCES.txt
+-rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)        1 2021-09-23 13:35:39.000000 jira2branch-0.1.9/jira2branch.egg-info/dependency_links.txt
+-rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)       58 2021-09-23 13:35:39.000000 jira2branch-0.1.9/jira2branch.egg-info/entry_points.txt
+-rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)       36 2021-09-23 13:35:39.000000 jira2branch-0.1.9/jira2branch.egg-info/requires.txt
+-rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)       12 2021-09-23 13:35:39.000000 jira2branch-0.1.9/jira2branch.egg-info/top_level.txt
+-rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)       38 2021-09-23 13:35:39.155202 jira2branch-0.1.9/setup.cfg
+-rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)     1052 2021-09-23 13:10:10.000000 jira2branch-0.1.9/setup.py
```

### Comparing `jira2branch-0.1.8/PKG-INFO` & `jira2branch-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jira2branch
-Version: 0.1.8
+Version: 0.1.9
 Summary: Takes a JIRA issue and creates a git branch
 Home-page: UNKNOWN
 Author: Tiago Pereira
 Author-email: tiago.pereira@infraspeak.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jira2branch-0.1.8/README.md` & `jira2branch-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `jira2branch-0.1.8/jira2branch/__main__.py` & `jira2branch-0.1.9/jira2branch/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,19 +127,25 @@
     try:
         repo = Repo(target)
         #  check if dirty
         if repo.is_dirty():
             click.secho("Current working dir not clean, please commit or stash your changes first", fg='red')
             exit(1)
 
-        # check if develop exists otherwise switch to master (otherwise switch to main)
+        # check if develop exists otherwise switch to master otherwise switch to main
         for branch in [source_branch, 'master', 'main']:
+            spinner = Halo(text=f'Checking if source branch {branch} exists...', spinner='dots')
+            spinner.start()
             if check_if_branch_exists(repo, branch):
                 source_branch = branch
+                click.secho(f'YES', fg='red')
+                spinner.stop()
                 break
+            else:
+                click.secho(f'NO', fg='red')
 
         #  check if a branch by this name already exists locally
         click.secho('Checking if branch already exists on local repository...')
         if check_if_branch_is_local(repo, branch_name):
             click.secho('Local branch already exists, switching to it', fg='blue')
             switch_to_branch(repo, branch_name)
             exit()
@@ -162,18 +168,19 @@
             repo.git.execute(['git', 'fetch', '--all'])
             spinner.stop()
             click.secho('Fetched all remote branches', fg='green')
         except Exception as err:
             print(err)
             spinner.stop()
         try:
-            source = f'origin/{source_branch}'
-            spinner = Halo(text=f'Creating local branch {branch_name} from {source}', spinner='dots')
+            spinner = Halo(text=f'Creating local branch {branch_name} from {source_branch}', spinner='dots')
             spinner.start()
-            repo.git.execute(['git', 'checkout', '-b', branch_name, source])
+            repo.git.execute(['git', 'checkout', source_branch])
+            repo.git.execute(['git', 'pull'])
+            repo.git.execute(['git', 'branch', branch_name])
             spinner.stop()
             click.secho(f'Created local branch {branch_name}', fg='green')
             switch_to_branch(repo, branch_name)
         except Exception as err:
             click.secho('Failed to create local branch...')
             print(err)
             spinner.stop()
```

### Comparing `jira2branch-0.1.8/jira2branch/tests/test_main.py` & `jira2branch-0.1.9/jira2branch/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `jira2branch-0.1.8/jira2branch.egg-info/PKG-INFO` & `jira2branch-0.1.9/jira2branch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jira2branch
-Version: 0.1.8
+Version: 0.1.9
 Summary: Takes a JIRA issue and creates a git branch
 Home-page: UNKNOWN
 Author: Tiago Pereira
 Author-email: tiago.pereira@infraspeak.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jira2branch-0.1.8/setup.py` & `jira2branch-0.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="jira2branch",
-    version="0.1.8",
+    version="0.1.9",
     description="Takes a JIRA issue and creates a git branch",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Tiago Pereira",
     author_email="tiago.pereira@infraspeak.com",
     license="MIT",
     classifiers=[
```

