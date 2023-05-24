# Comparing `tmp/git-build-branch-0.1.14.tar.gz` & `tmp/git-build-branch-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-build-branch-0.1.14.tar", last modified: Thu Aug 25 15:02:08 2022, max compression
+gzip compressed data, was "dist/git-build-branch-0.1.9.tar", last modified: Fri Sep  4 08:03:24 2020, max compression
```

## Comparing `git-build-branch-0.1.14.tar` & `git-build-branch-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 grahamherceg   (501) staff       (20)        0 2022-08-25 15:02:08.071039 git-build-branch-0.1.14/
--rw-r--r--   0 grahamherceg   (501) staff       (20)      694 2022-08-18 02:52:42.000000 git-build-branch-0.1.14/CONTRIBUTING.rst
--rw-r--r--   0 grahamherceg   (501) staff       (20)     1503 2022-08-18 02:52:42.000000 git-build-branch-0.1.14/LICENSE
--rw-r--r--   0 grahamherceg   (501) staff       (20)      156 2022-08-18 02:52:42.000000 git-build-branch-0.1.14/MANIFEST.in
--rw-r--r--   0 grahamherceg   (501) staff       (20)     3719 2022-08-25 15:02:08.071194 git-build-branch-0.1.14/PKG-INFO
--rw-r--r--   0 grahamherceg   (501) staff       (20)     2867 2022-08-18 02:52:42.000000 git-build-branch-0.1.14/README.rst
-drwxr-xr-x   0 grahamherceg   (501) staff       (20)        0 2022-08-25 15:02:08.068433 git-build-branch-0.1.14/git_build_branch/
--rw-r--r--   0 grahamherceg   (501) staff       (20)      125 2022-08-25 15:01:41.000000 git-build-branch-0.1.14/git_build_branch/__init__.py
--rw-r--r--   0 grahamherceg   (501) staff       (20)    12301 2022-08-18 19:48:55.000000 git-build-branch-0.1.14/git_build_branch/branch_builder.py
--rw-r--r--   0 grahamherceg   (501) staff       (20)      703 2022-08-18 02:52:42.000000 git-build-branch-0.1.14/git_build_branch/checkyaml.py
--rw-r--r--   0 grahamherceg   (501) staff       (20)     7231 2022-08-18 02:52:42.000000 git-build-branch-0.1.14/git_build_branch/gitutils.py
--rw-r--r--   0 grahamherceg   (501) staff       (20)     2443 2022-08-18 02:52:42.000000 git-build-branch-0.1.14/git_build_branch/safe_commit_files.py
--rw-r--r--   0 grahamherceg   (501) staff       (20)     1413 2022-08-18 02:52:42.000000 git-build-branch-0.1.14/git_build_branch/sh_verbose.py
-drwxr-xr-x   0 grahamherceg   (501) staff       (20)        0 2022-08-25 15:02:08.070791 git-build-branch-0.1.14/git_build_branch.egg-info/
--rw-r--r--   0 grahamherceg   (501) staff       (20)     3719 2022-08-25 15:02:07.000000 git-build-branch-0.1.14/git_build_branch.egg-info/PKG-INFO
--rw-r--r--   0 grahamherceg   (501) staff       (20)      539 2022-08-25 15:02:08.000000 git-build-branch-0.1.14/git_build_branch.egg-info/SOURCES.txt
--rw-r--r--   0 grahamherceg   (501) staff       (20)        1 2022-08-25 15:02:07.000000 git-build-branch-0.1.14/git_build_branch.egg-info/dependency_links.txt
--rw-r--r--   0 grahamherceg   (501) staff       (20)      134 2022-08-25 15:02:07.000000 git-build-branch-0.1.14/git_build_branch.egg-info/entry_points.txt
--rw-r--r--   0 grahamherceg   (501) staff       (20)        1 2022-08-25 15:02:07.000000 git-build-branch-0.1.14/git_build_branch.egg-info/not-zip-safe
--rw-r--r--   0 grahamherceg   (501) staff       (20)       84 2022-08-25 15:02:07.000000 git-build-branch-0.1.14/git_build_branch.egg-info/requires.txt
--rw-r--r--   0 grahamherceg   (501) staff       (20)       17 2022-08-25 15:02:07.000000 git-build-branch-0.1.14/git_build_branch.egg-info/top_level.txt
--rw-r--r--   0 grahamherceg   (501) staff       (20)      573 2022-08-25 15:02:08.071805 git-build-branch-0.1.14/setup.cfg
--rw-r--r--   0 grahamherceg   (501) staff       (20)     1672 2022-08-25 15:01:41.000000 git-build-branch-0.1.14/setup.py
+drwxrwxr-x   0 skelly    (1000) skelly    (1000)        0 2020-09-04 08:03:24.000000 git-build-branch-0.1.9/
+-rw-rw-r--   0 skelly    (1000) skelly    (1000)     1503 2020-09-01 14:13:46.000000 git-build-branch-0.1.9/LICENSE
+-rw-rw-r--   0 skelly    (1000) skelly    (1000)     1671 2020-09-04 08:03:19.000000 git-build-branch-0.1.9/setup.py
+-rw-rw-r--   0 skelly    (1000) skelly    (1000)     4405 2020-09-04 08:03:24.000000 git-build-branch-0.1.9/PKG-INFO
+drwxrwxr-x   0 skelly    (1000) skelly    (1000)        0 2020-09-04 08:03:24.000000 git-build-branch-0.1.9/git_build_branch/
+-rw-rw-r--   0 skelly    (1000) skelly    (1000)     2453 2020-09-03 13:53:10.000000 git-build-branch-0.1.9/git_build_branch/safe_commit_files.py
+-rw-rw-r--   0 skelly    (1000) skelly    (1000)    13734 2020-09-03 14:21:14.000000 git-build-branch-0.1.9/git_build_branch/branch_builder.py
+-rw-rw-r--   0 skelly    (1000) skelly    (1000)     1413 2020-09-03 14:20:18.000000 git-build-branch-0.1.9/git_build_branch/sh_verbose.py
+-rw-rw-r--   0 skelly    (1000) skelly    (1000)     5918 2020-09-03 13:40:11.000000 git-build-branch-0.1.9/git_build_branch/gitutils.py
+-rw-rw-r--   0 skelly    (1000) skelly    (1000)      124 2020-09-04 08:03:19.000000 git-build-branch-0.1.9/git_build_branch/__init__.py
+-rw-rw-r--   0 skelly    (1000) skelly    (1000)      703 2020-09-03 13:40:49.000000 git-build-branch-0.1.9/git_build_branch/checkyaml.py
+-rw-rw-r--   0 skelly    (1000) skelly    (1000)     2721 2020-09-04 08:02:20.000000 git-build-branch-0.1.9/README.rst
+drwxrwxr-x   0 skelly    (1000) skelly    (1000)        0 2020-09-04 08:03:24.000000 git-build-branch-0.1.9/git_build_branch.egg-info/
+-rw-rw-r--   0 skelly    (1000) skelly    (1000)       17 2020-09-04 08:03:24.000000 git-build-branch-0.1.9/git_build_branch.egg-info/top_level.txt
+-rw-rw-r--   0 skelly    (1000) skelly    (1000)     4405 2020-09-04 08:03:24.000000 git-build-branch-0.1.9/git_build_branch.egg-info/PKG-INFO
+-rw-rw-r--   0 skelly    (1000) skelly    (1000)      135 2020-09-04 08:03:24.000000 git-build-branch-0.1.9/git_build_branch.egg-info/entry_points.txt
+-rw-rw-r--   0 skelly    (1000) skelly    (1000)        1 2020-09-04 08:03:24.000000 git-build-branch-0.1.9/git_build_branch.egg-info/dependency_links.txt
+-rw-rw-r--   0 skelly    (1000) skelly    (1000)      539 2020-09-04 08:03:24.000000 git-build-branch-0.1.9/git_build_branch.egg-info/SOURCES.txt
+-rw-rw-r--   0 skelly    (1000) skelly    (1000)        1 2020-09-04 08:03:24.000000 git-build-branch-0.1.9/git_build_branch.egg-info/not-zip-safe
+-rw-rw-r--   0 skelly    (1000) skelly    (1000)       84 2020-09-04 08:03:24.000000 git-build-branch-0.1.9/git_build_branch.egg-info/requires.txt
+-rw-rw-r--   0 skelly    (1000) skelly    (1000)      572 2020-09-04 08:03:24.000000 git-build-branch-0.1.9/setup.cfg
+-rw-rw-r--   0 skelly    (1000) skelly    (1000)      615 2020-09-04 08:00:41.000000 git-build-branch-0.1.9/CONTRIBUTING.rst
+-rw-rw-r--   0 skelly    (1000) skelly    (1000)      156 2020-09-02 11:44:34.000000 git-build-branch-0.1.9/MANIFEST.in
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `git-build-branch-0.1.14/CONTRIBUTING.rst` & `git-build-branch-0.1.9/CONTRIBUTING.rst`

 * *Files 26% similar despite different names*

```diff
@@ -7,23 +7,21 @@
 Here's how to set up `git-build-branch` for local development.
 
 1. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up
 for local development::
 
     $ mkvirtualenv git-build-branch
     $ cd git-build-branch/  # cloned repo
-    $ pip install -r requirements_dev.txt (or requirements_dev_py2.txt for python2)
+    $ pip install -r requirements_dev.txt
 
 
-See ``make`` output for common tools.
-
-Releasing
+Deploying
 ---------
 
-A reminder for the maintainers on how to make a release.
+A reminder for the maintainers on how to deploy.
 Make sure all your changes are committed.
 Then run::
 
 $ bump2version patch # possible: major / minor / patch
+$ git push
 $ git push --tags
 $ make clean release
-
```

### Comparing `git-build-branch-0.1.14/LICENSE` & `git-build-branch-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `git-build-branch-0.1.14/PKG-INFO` & `git-build-branch-0.1.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,129 +1,125 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: git-build-branch
-Version: 0.1.14
+Version: 0.1.9
 Summary: Utility tool for building Git branches my merging multiple other branches together.
 Home-page: https://github.com/dimagi/git-build-branch
 Author: Dimagi
 Author-email: dev@dimagi.com
 License: BSD license
+Description: ==================
+        git-build-branch
+        ==================
+        
+        
+        .. image:: https://img.shields.io/pypi/v/git-build-branch.svg
+                :target: https://pypi.python.org/pypi/git-build-branch
+        
+        
+        Utility tool for building Git branches my merging multiple other branches together.
+        
+        
+        * Free software: BSD license
+        
+        
+        Documentation
+        -------------
+        In some cases it may be desirable to have full control over what code is deployed. This can
+        be accomplished by creating a YAML configuration file to describe what should be included in your branch.
+        
+        The format of the file is as follows:
+        
+        .. code-block:: yaml
+        
+            trunk: master
+            name: autostaging  # name of the branch to build
+            branches:  # list of branches to merge into final branch
+              - feature1
+              - feature2
+              - forkowner:feature3 # branch from fork of repository
+            submodules:
+              submodules/module1:
+                branches:
+                  - feature1
+                  - forkowner:feature2 # branch from fork of repository
+              submodules/module2:
+                trunk: develop
+                branches:
+                  - feature2
+        
+        To add some safety around this file you should use the `safe-commit-files` utility:
+        
+        .. code-block:: shell
+        
+            safe-commit-files --push /path/to/branch_config.yml
+        
+        Building the branch
+        ~~~~~~~~~~~~~~~~~~~
+        This configuration file can be used to build a deploy branch:
+        
+        .. code-block:: bash
+        
+            git checkout master
+            git-build-branch path/to/branch_config.yml
+        
+        Conflict Resolution
+        ~~~~~~~~~~~~~~~~~~~
+        
+        First, determine where the conflict lies.
+        
+        a). branch `foo` conflicts with `master`
+        
+        .. code-block:: shell
+        
+            git checkout -b foo origin/foo
+            git pull origin master
+        
+            # try to resolve conflict
+        
+            git push origin foo
+        
+        b). branch `foo` conflicts with branch `bar`
+        
+        You can't just merge foo into bar or vice versa, otherwise the PR
+        for foo will contain commits from bar.  Instead make a third,
+        conflict-resolution branch:
+        
+        .. code-block:: shell
+        
+            git checkout -b foo+bar --no-track origin/foo
+            git pull origin bar
+        
+            # try to resolve conflict
+        
+            git push origin foo+bar
+        
+        Now add the branch `foo+bar` to `branch_config.yml` and move branches foo and
+        bar to right below it.
+        
+        Later on branch B gets merged into master and removed from `branch_config.yml`.
+        
+        Perhaps the person who removes it also notices the A+B and does the
+        following. Otherwise anyone who comes along and sees A+B but not both
+        branches can feel free to assume the following need to be done.
+        
+        * Merge A+B into A. Since B is now gone, you want to merge the
+          resolution into A, otherwise A will conflict with master.
+        
+        * Remove A+B from `branch_config.yml`. It's no longer necessary since it's
+          now a subset of A.
+        
+        If you are unsure of how to resolve a conflict, notify the branch owner.
+        
+        
 Keywords: git-build-branch
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-License-File: LICENSE
-
-==================
-git-build-branch
-==================
-
-
-.. image:: https://img.shields.io/pypi/v/git-build-branch.svg
-        :target: https://pypi.python.org/pypi/git-build-branch
-
-
-Utility tool for building Git branches by merging multiple other branches together.
-
-
-* Free software: BSD license
-
-For guidelines on contributing to the project please read the CONTRIBUTING_ documentation.
-
-.. _CONTRIBUTING: CONTRIBUTING.rst
-
-
-Documentation
--------------
-In some cases it may be desirable to have full control over what code is deployed. This can
-be accomplished by creating a YAML configuration file to describe what should be included in your branch.
-
-The format of the file is as follows:
-
-.. code-block:: yaml
-
-    trunk: master
-    name: autostaging  # name of the branch to build
-    branches:  # list of branches to merge into final branch
-      - feature1
-      - feature2
-      - forkowner:feature3 # branch from fork of repository
-    submodules:
-      submodules/module1:
-        branches:
-          - feature1
-          - forkowner:feature2 # branch from fork of repository
-      submodules/module2:
-        trunk: develop
-        branches:
-          - feature2
-
-To add some safety around this file you should use the ``safe-commit-files`` utility:
-
-.. code-block:: shell
-
-    safe-commit-files --push /path/to/branch_config.yml
-
-Building the branch
-~~~~~~~~~~~~~~~~~~~
-This configuration file can be used to build a deploy branch:
-
-.. code-block:: bash
-
-    git checkout master
-    git-build-branch path/to/branch_config.yml
-
-Conflict Resolution
-~~~~~~~~~~~~~~~~~~~
-
-First, determine where the conflict lies.
-
-a). branch ``foo`` conflicts with ``master``
-
-.. code-block:: shell
-
-    git checkout -b foo origin/foo
-    git pull origin master
-
-    # try to resolve conflict
-
-    git push origin foo
-
-b). branch ``foo`` conflicts with branch ``bar``
-
-You can't just merge foo into bar or vice versa, otherwise the PR
-for foo will contain commits from bar.  Instead make a third,
-conflict-resolution branch:
-
-.. code-block:: shell
-
-    git checkout -b foo+bar --no-track origin/foo
-    git pull origin bar
-
-    # try to resolve conflict
-
-    git push origin foo+bar
-
-Now add the branch ``foo+bar`` to ``branch_config.yml`` and move branches foo and
-bar to right below it.
-
-Later on branch B gets merged into master and removed from ``branch_config.yml``.
-
-Perhaps the person who removes it also notices the A+B and does the
-following. Otherwise anyone who comes along and sees A+B but not both
-branches can feel free to assume the following need to be done.
-
-* Merge A+B into A. Since B is now gone, you want to merge the
-  resolution into A, otherwise A will conflict with master.
-
-* Remove A+B from ``branch_config.yml``. It's no longer necessary since it's
-  now a subset of A.
-
-If you are unsure of how to resolve a conflict, notify the branch owner.
-
```

### Comparing `git-build-branch-0.1.14/README.rst` & `git-build-branch-0.1.9/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -3,23 +3,19 @@
 ==================
 
 
 .. image:: https://img.shields.io/pypi/v/git-build-branch.svg
         :target: https://pypi.python.org/pypi/git-build-branch
 
 
-Utility tool for building Git branches by merging multiple other branches together.
+Utility tool for building Git branches my merging multiple other branches together.
 
 
 * Free software: BSD license
 
-For guidelines on contributing to the project please read the CONTRIBUTING_ documentation.
-
-.. _CONTRIBUTING: CONTRIBUTING.rst
-
 
 Documentation
 -------------
 In some cases it may be desirable to have full control over what code is deployed. This can
 be accomplished by creating a YAML configuration file to describe what should be included in your branch.
 
 The format of the file is as follows:
@@ -38,15 +34,15 @@
           - feature1
           - forkowner:feature2 # branch from fork of repository
       submodules/module2:
         trunk: develop
         branches:
           - feature2
 
-To add some safety around this file you should use the ``safe-commit-files`` utility:
+To add some safety around this file you should use the `safe-commit-files` utility:
 
 .. code-block:: shell
 
     safe-commit-files --push /path/to/branch_config.yml
 
 Building the branch
 ~~~~~~~~~~~~~~~~~~~
@@ -58,50 +54,50 @@
     git-build-branch path/to/branch_config.yml
 
 Conflict Resolution
 ~~~~~~~~~~~~~~~~~~~
 
 First, determine where the conflict lies.
 
-a). branch ``foo`` conflicts with ``master``
+a). branch `foo` conflicts with `master`
 
 .. code-block:: shell
 
     git checkout -b foo origin/foo
     git pull origin master
 
     # try to resolve conflict
 
     git push origin foo
 
-b). branch ``foo`` conflicts with branch ``bar``
+b). branch `foo` conflicts with branch `bar`
 
 You can't just merge foo into bar or vice versa, otherwise the PR
 for foo will contain commits from bar.  Instead make a third,
 conflict-resolution branch:
 
 .. code-block:: shell
 
     git checkout -b foo+bar --no-track origin/foo
     git pull origin bar
 
     # try to resolve conflict
 
     git push origin foo+bar
 
-Now add the branch ``foo+bar`` to ``branch_config.yml`` and move branches foo and
+Now add the branch `foo+bar` to `branch_config.yml` and move branches foo and
 bar to right below it.
 
-Later on branch B gets merged into master and removed from ``branch_config.yml``.
+Later on branch B gets merged into master and removed from `branch_config.yml`.
 
 Perhaps the person who removes it also notices the A+B and does the
 following. Otherwise anyone who comes along and sees A+B but not both
 branches can feel free to assume the following need to be done.
 
 * Merge A+B into A. Since B is now gone, you want to merge the
   resolution into A, otherwise A will conflict with master.
 
-* Remove A+B from ``branch_config.yml``. It's no longer necessary since it's
+* Remove A+B from `branch_config.yml`. It's no longer necessary since it's
   now a subset of A.
 
 If you are unsure of how to resolve a conflict, notify the branch owner.
```

### Comparing `git-build-branch-0.1.14/git_build_branch/branch_builder.py` & `git-build-branch-0.1.9/git_build_branch/branch_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,25 +9,21 @@
 import jsonobject  # noqa E402
 import os  # noqa E402
 import re  # noqa E402
 import sh  # noqa E402
 import yaml  # noqa E402
 from contextlib2 import ExitStack  # noqa E402
 
-from .gitutils import (  # noqa E402
-    MissingRemote,
+from .gitutils import (
     OriginalBranch,
     get_git,
-    get_local_ref,
     git_recent_tags,
-    has_local,
     has_merge_conflict,
-    origin,
     print_merge_details,
-)
+)  # noqa E402
 
 from .sh_verbose import ShVerbose  # noqa E402
 
 
 class BranchConfig(jsonobject.JsonObject):
     trunk = jsonobject.StringProperty()
     name = jsonobject.StringProperty()
@@ -90,14 +86,40 @@
 
 def remote_url(git, remote, original="origin"):
     origin_url = sh.grep(git.remote("-v"), original).split()[1]
     repo_name = origin_url.rsplit("/", 1)[1]
     return "https://github.com/{}/{}".format(remote, repo_name)
 
 
+def has_ref(git, ref):
+    """Return true if the named branch exists"""
+    try:
+        out = git("show-ref", "--verify", "--quiet", ref)
+    except sh.ErrorReturnCode:
+        return False
+    return out.exit_code == 0
+
+
+def has_local(git, branch):
+    """Return true if the named local branch exists"""
+    return has_ref(git, "refs/heads/{}".format(branch))
+
+
+def has_remote(git, ref):
+    """Return true if the named remote branch exists
+
+    :param ref: Remote ref (example: origin/branch-name)
+    """
+    return has_ref(git, "refs/remotes/{}".format(ref))
+
+
+def origin(branch):
+    return "origin/{}".format(branch)
+
+
 def sync_local_copies(config, path, push=True):
     base_config = config
     unpushed_branches = []
 
     def _count_commits(compare_spec):
         return int(sh.wc(git.log(compare_spec, '--oneline', _piped=True), '-l'))
 
@@ -147,20 +169,28 @@
         for path, config in all_configs:
             git = get_git(path)
             try:
                 git.checkout('-B', config.name, origin(config.trunk), '--no-track')
             except Exception:
                 git.checkout('-B', config.name, config.trunk, '--no-track')
             for branch in config.branches:
-                try:
-                    branch = get_local_ref(git, branch)
-                except MissingRemote:
-                    not_found.append((path, branch))
-                    print(f"  [{format_cwd(path)}] {branch} NOT FOUND")
-                    continue
+                remote = ":" in branch
+                if remote or not has_local(git, branch):
+                    if remote:
+                        remote_branch = branch.replace(":", "/", 1)
+                    else:
+                        remote_branch = origin(branch)
+                    if not has_remote(git, remote_branch):
+                        not_found.append((path, branch))
+                        print("  [{cwd}] {branch} NOT FOUND".format(
+                            cwd=format_cwd(path),
+                            branch=branch,
+                        ))
+                        continue
+                    branch = remote_branch
                 print("  [{cwd}] Merging {branch} into {name}".format(
                     cwd=path,
                     branch=branch,
                     name=config.name
                 ), end=' ')
                 try:
                     git.merge(branch, '--no-edit')
@@ -205,18 +235,18 @@
                     name=config.name,
                 ))
                 force_push(get_git(path), config.name)
 
     if not_found:
         print("You must remove the following branches before rebuilding:")
         for cwd, branch in not_found:
-            print(red("  [{cwd}] {branch}".format(
+            print("  [{cwd}] {branch}".format(
                 cwd=format_cwd(cwd),
                 branch=branch,
-            )))
+            ))
     if merge_conflicts:
         print("You must fix the following merge conflicts before rebuilding:")
         for cwd, branch, config in merge_conflicts:
             print("\n[{cwd}] {branch} => {name}".format(
                 cwd=format_cwd(cwd),
                 branch=branch,
                 name=config.name,
@@ -244,17 +274,27 @@
         print_merge_details(branch, config.name, git,
                             known_branches=config.branches)
 
 
 def force_push(git, branch):
     try:
         git.push('origin', branch, '--force')
-    except sh.ErrorReturnCode_128:
-        print(red("Failed to force push to origin. Please check your remote URL and ensure it accepts writes."))
-        raise
+    except sh.ErrorReturnCode_128 as e:
+        # oops we're using a read-only URL, so change to the suggested url
+        try:
+            line = sh.grep(git.remote("-v"),
+                           '-E', r'^origin.(https|git)://github\.com/.*\(push\)$')
+        except sh.ErrorReturnCode_1:
+            raise e
+        old_url = line.strip().split()[1]
+        prefix = "git" if old_url.startswith("git:") else "https"
+        new_url = old_url.replace(prefix + "://github.com/", "git@github.com:")
+        print("    {} -> {}".format(old_url, new_url))
+        git.remote('set-url', 'origin', new_url)
+        git.push('origin', branch, '--force')
 
 
 def format_cwd(cwd):
     return os.path.join(cwd) if cwd else '.'
 
 
 class DisableGitHooks(object):
```

### Comparing `git-build-branch-0.1.14/git_build_branch/checkyaml.py` & `git-build-branch-0.1.9/git_build_branch/checkyaml.py`

 * *Files identical despite different names*

### Comparing `git-build-branch-0.1.14/git_build_branch/gitutils.py` & `git-build-branch-0.1.9/git_build_branch/gitutils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import re
 
 import sh
 
 from .sh_verbose import ShVerbose
 
 
@@ -54,73 +53,23 @@
     submodules = []
     for line in git.submodule().split('\n')[:-1]:
         path = line[1:].split()[1]
         submodules.append(path)
     return submodules
 
 
-def get_local_ref(git, branch):
-    remote = ":" in branch
-    if isinstance(branch, LocalRef) or not remote and has_local(git, branch):
-        return branch
-    if remote:
-        remote_branch = branch.replace(":", "/", 1)
-    else:
-        remote_branch = origin(branch)
-    if not has_remote(git, remote_branch):
-        path = git._partial_call_args.get("cwd") or os.getcwd()
-        raise MissingRemote(f"git ref '{remote_branch}' not found in {path}")
-    return LocalRef(remote_branch)
-
-
-def origin(branch):
-    return "origin/{}".format(branch)
-
-
-def has_local(git, branch):
-    """Return true if the named local branch exists"""
-    return has_ref(git, "refs/heads/{}".format(branch))
-
-
-def has_remote(git, ref):
-    """Return true if the named remote branch exists
-
-    :param ref: Remote ref (example: origin/branch-name)
-    """
-    return has_ref(git, "refs/remotes/{}".format(ref))
-
-
-def has_ref(git, ref):
-    """Return true if the named branch exists"""
-    try:
-        out = git("show-ref", "--verify", "--quiet", ref)
-    except sh.ErrorReturnCode:
-        return False
-    return out.exit_code == 0
-
-
-class LocalRef(str):
-    pass
-
-
-class MissingRemote(Exception):
-    pass
-
-
 def git_check_merge(branch1, branch2, git=None):
     """
     returns True if branch1 would auto-merge cleanly into branch2,
     False if the merge requires human assistance
 
     Thanks to http://stackoverflow.com/a/501461/240553
 
     """
     git = git or get_git()
-    branch1 = get_local_ref(git, branch1)
-    branch2 = get_local_ref(git, branch2)
     with ShVerbose(False):
         orig_branch = git_current_branch(git)
         git.checkout(branch2)
         is_behind = git.log('{0}..{1}'.format(branch2, branch1),
                             max_count=1).strip()
         clean_merge = True
         if is_behind:
@@ -131,18 +80,15 @@
                 clean_merge = False
             git.merge('--abort')
         git.checkout(orig_branch)
         return clean_merge
 
 
 def has_merge_conflict(branch1, branch2, git):
-    try:
-        return not git_check_merge(branch1, branch2, git=git)
-    except MissingRemote:
-        return False
+    return not git_check_merge(branch1, branch2, git=git)
 
 
 def git_bisect_merge_conflict(branch1, branch2, git=None):
     """
     return the branch2 commit that prevents branch1 from being merged in
 
     """
@@ -222,12 +168,13 @@
         option = args.pop(0)
     except IndexError:
         option = None
     if option == 'show-conflict':
         if len(args) == 2:
             print_merge_details(*args, git=get_git())
         else:
-            print('usage: python gitutils.py show-conflict <branch1> <branch2>')
+            print ('usage: python scripts/gitutils.py '
+                   'show-conflict <branch1> <branch2>')
     else:
-        print('usage: python gitutils.py <command> [args...]\n')
+        print('usage: python scripts/gitutils.py <command> [args...]\n')
         print('Available commands:')
         print(_left_pad('   ', '\n'.join(options)))
```

### Comparing `git-build-branch-0.1.14/git_build_branch/safe_commit_files.py` & `git-build-branch-0.1.9/git_build_branch/safe_commit_files.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,26 +34,26 @@
         if branch != "master":
             print("You may only commit a deploy branch config file to master. '{}'".format(branch))
             exit(1)
 
         git.add(*files)
         try:
             staged = sh.grep(git.diff("--staged", "--stat"), "|")
-        except ErrorReturnCode:
+        except ErrorReturnCode as e:
             print("You have no changes to commit.")
             exit(1)
 
         staged_files = filter(None, [line.split("|")[0].strip() for line in staged.split("\n")])
         if not staged_files:
             print("You have no changes to commit.")
             exit(1)
 
         basenames = {os.path.basename(filename) for filename in files}
         staged_basenames = {os.path.basename(filename) for filename in staged_files}
-        if basenames != staged_basenames:
+        if  basenames != staged_basenames:
             print("Unexpected files staged: {}".format(", ".join(staged_files)))
             exit(1)
 
         for filename in files:
             if os.path.splitext(filename)[1].lower() in ('yaml', 'yml'):
                 try:
                     checkyaml(filename)
@@ -62,16 +62,16 @@
                     print(e)
                     exit(1)
 
         git.fetch()
         if git.log("--max-count=1", "origin/{0}..{0}".format(branch)).strip():
             print("Your local '{0}' is ahead of 'origin/{0}'.".format(branch))
 
-        message = "updating files: {}".format(", ".join(files))
-        git.commit("--message", message, "--message", "[ci skip]")
+        message = "'updating files: {}'".format(", ".join(files))
+        git.commit("--message", message, "--message", "'[ci skip]'")
 
         if args.push:
             git.push("origin", branch)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `git-build-branch-0.1.14/git_build_branch/sh_verbose.py` & `git-build-branch-0.1.9/git_build_branch/sh_verbose.py`

 * *Files identical despite different names*

### Comparing `git-build-branch-0.1.14/git_build_branch.egg-info/PKG-INFO` & `git-build-branch-0.1.9/git_build_branch.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,129 +1,125 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: git-build-branch
-Version: 0.1.14
+Version: 0.1.9
 Summary: Utility tool for building Git branches my merging multiple other branches together.
 Home-page: https://github.com/dimagi/git-build-branch
 Author: Dimagi
 Author-email: dev@dimagi.com
 License: BSD license
+Description: ==================
+        git-build-branch
+        ==================
+        
+        
+        .. image:: https://img.shields.io/pypi/v/git-build-branch.svg
+                :target: https://pypi.python.org/pypi/git-build-branch
+        
+        
+        Utility tool for building Git branches my merging multiple other branches together.
+        
+        
+        * Free software: BSD license
+        
+        
+        Documentation
+        -------------
+        In some cases it may be desirable to have full control over what code is deployed. This can
+        be accomplished by creating a YAML configuration file to describe what should be included in your branch.
+        
+        The format of the file is as follows:
+        
+        .. code-block:: yaml
+        
+            trunk: master
+            name: autostaging  # name of the branch to build
+            branches:  # list of branches to merge into final branch
+              - feature1
+              - feature2
+              - forkowner:feature3 # branch from fork of repository
+            submodules:
+              submodules/module1:
+                branches:
+                  - feature1
+                  - forkowner:feature2 # branch from fork of repository
+              submodules/module2:
+                trunk: develop
+                branches:
+                  - feature2
+        
+        To add some safety around this file you should use the `safe-commit-files` utility:
+        
+        .. code-block:: shell
+        
+            safe-commit-files --push /path/to/branch_config.yml
+        
+        Building the branch
+        ~~~~~~~~~~~~~~~~~~~
+        This configuration file can be used to build a deploy branch:
+        
+        .. code-block:: bash
+        
+            git checkout master
+            git-build-branch path/to/branch_config.yml
+        
+        Conflict Resolution
+        ~~~~~~~~~~~~~~~~~~~
+        
+        First, determine where the conflict lies.
+        
+        a). branch `foo` conflicts with `master`
+        
+        .. code-block:: shell
+        
+            git checkout -b foo origin/foo
+            git pull origin master
+        
+            # try to resolve conflict
+        
+            git push origin foo
+        
+        b). branch `foo` conflicts with branch `bar`
+        
+        You can't just merge foo into bar or vice versa, otherwise the PR
+        for foo will contain commits from bar.  Instead make a third,
+        conflict-resolution branch:
+        
+        .. code-block:: shell
+        
+            git checkout -b foo+bar --no-track origin/foo
+            git pull origin bar
+        
+            # try to resolve conflict
+        
+            git push origin foo+bar
+        
+        Now add the branch `foo+bar` to `branch_config.yml` and move branches foo and
+        bar to right below it.
+        
+        Later on branch B gets merged into master and removed from `branch_config.yml`.
+        
+        Perhaps the person who removes it also notices the A+B and does the
+        following. Otherwise anyone who comes along and sees A+B but not both
+        branches can feel free to assume the following need to be done.
+        
+        * Merge A+B into A. Since B is now gone, you want to merge the
+          resolution into A, otherwise A will conflict with master.
+        
+        * Remove A+B from `branch_config.yml`. It's no longer necessary since it's
+          now a subset of A.
+        
+        If you are unsure of how to resolve a conflict, notify the branch owner.
+        
+        
 Keywords: git-build-branch
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-License-File: LICENSE
-
-==================
-git-build-branch
-==================
-
-
-.. image:: https://img.shields.io/pypi/v/git-build-branch.svg
-        :target: https://pypi.python.org/pypi/git-build-branch
-
-
-Utility tool for building Git branches by merging multiple other branches together.
-
-
-* Free software: BSD license
-
-For guidelines on contributing to the project please read the CONTRIBUTING_ documentation.
-
-.. _CONTRIBUTING: CONTRIBUTING.rst
-
-
-Documentation
--------------
-In some cases it may be desirable to have full control over what code is deployed. This can
-be accomplished by creating a YAML configuration file to describe what should be included in your branch.
-
-The format of the file is as follows:
-
-.. code-block:: yaml
-
-    trunk: master
-    name: autostaging  # name of the branch to build
-    branches:  # list of branches to merge into final branch
-      - feature1
-      - feature2
-      - forkowner:feature3 # branch from fork of repository
-    submodules:
-      submodules/module1:
-        branches:
-          - feature1
-          - forkowner:feature2 # branch from fork of repository
-      submodules/module2:
-        trunk: develop
-        branches:
-          - feature2
-
-To add some safety around this file you should use the ``safe-commit-files`` utility:
-
-.. code-block:: shell
-
-    safe-commit-files --push /path/to/branch_config.yml
-
-Building the branch
-~~~~~~~~~~~~~~~~~~~
-This configuration file can be used to build a deploy branch:
-
-.. code-block:: bash
-
-    git checkout master
-    git-build-branch path/to/branch_config.yml
-
-Conflict Resolution
-~~~~~~~~~~~~~~~~~~~
-
-First, determine where the conflict lies.
-
-a). branch ``foo`` conflicts with ``master``
-
-.. code-block:: shell
-
-    git checkout -b foo origin/foo
-    git pull origin master
-
-    # try to resolve conflict
-
-    git push origin foo
-
-b). branch ``foo`` conflicts with branch ``bar``
-
-You can't just merge foo into bar or vice versa, otherwise the PR
-for foo will contain commits from bar.  Instead make a third,
-conflict-resolution branch:
-
-.. code-block:: shell
-
-    git checkout -b foo+bar --no-track origin/foo
-    git pull origin bar
-
-    # try to resolve conflict
-
-    git push origin foo+bar
-
-Now add the branch ``foo+bar`` to ``branch_config.yml`` and move branches foo and
-bar to right below it.
-
-Later on branch B gets merged into master and removed from ``branch_config.yml``.
-
-Perhaps the person who removes it also notices the A+B and does the
-following. Otherwise anyone who comes along and sees A+B but not both
-branches can feel free to assume the following need to be done.
-
-* Merge A+B into A. Since B is now gone, you want to merge the
-  resolution into A, otherwise A will conflict with master.
-
-* Remove A+B from ``branch_config.yml``. It's no longer necessary since it's
-  now a subset of A.
-
-If you are unsure of how to resolve a conflict, notify the branch owner.
-
```

### Comparing `git-build-branch-0.1.14/git_build_branch.egg-info/SOURCES.txt` & `git-build-branch-0.1.9/git_build_branch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `git-build-branch-0.1.14/setup.cfg` & `git-build-branch-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.14
+current_version = 0.1.9
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `git-build-branch-0.1.14/setup.py` & `git-build-branch-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,10 +46,10 @@
     long_description=readme,
     include_package_data=True,
     keywords='git-build-branch',
     name='git-build-branch',
     packages=find_packages(include=['git_build_branch', 'git_build_branch.*']),
     setup_requires=setup_requirements,
     url='https://github.com/dimagi/git-build-branch',
-    version='0.1.14',
+    version='0.1.9',
     zip_safe=False,
 )
```

