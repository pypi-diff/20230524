# Comparing `tmp/apply_pr-2.8.2.tar.gz` & `tmp/apply_pr-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apply_pr-2.8.2.tar", last modified: Wed Jul 15 11:40:58 2020, max compression
+gzip compressed data, was "dist/apply_pr-2.9.0.tar", last modified: Fri Jul 17 07:18:06 2020, max compression
```

## Comparing `apply_pr-2.8.2.tar` & `apply_pr-2.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-15 11:40:58.000000 apply_pr-2.8.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)       26 2020-07-15 11:40:36.000000 apply_pr-2.8.2/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)       63 2020-07-15 11:40:36.000000 apply_pr-2.8.2/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      243 2020-07-15 11:40:58.000000 apply_pr-2.8.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4438 2020-07-15 11:40:36.000000 apply_pr-2.8.2/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-15 11:40:58.000000 apply_pr-2.8.2/apply_pr.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      243 2020-07-15 11:40:58.000000 apply_pr-2.8.2/apply_pr.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-15 11:40:58.000000 apply_pr-2.8.2/apply_pr.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2020-07-15 11:40:58.000000 apply_pr-2.8.2/apply_pr.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      318 2020-07-15 11:40:58.000000 apply_pr-2.8.2/apply_pr.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       63 2020-07-15 11:40:58.000000 apply_pr-2.8.2/apply_pr.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      107 2020-07-15 11:40:58.000000 apply_pr-2.8.2/apply_pr.egg-info/entry_points.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-15 11:40:58.000000 apply_pr-2.8.2/apply_pr/
--rw-rw-r--   0 travis    (2000) travis    (2000)    36130 2020-07-15 11:40:36.000000 apply_pr-2.8.2/apply_pr/fabfile.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8072 2020-07-15 11:40:36.000000 apply_pr-2.8.2/apply_pr/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      658 2020-07-15 11:40:36.000000 apply_pr-2.8.2/apply_pr/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      148 2020-07-15 11:40:36.000000 apply_pr-2.8.2/apply_pr/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-07-15 11:40:58.000000 apply_pr-2.8.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      555 2020-07-15 11:40:36.000000 apply_pr-2.8.2/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-17 07:18:06.000000 apply_pr-2.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       26 2020-07-17 07:17:48.000000 apply_pr-2.9.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)       63 2020-07-17 07:17:48.000000 apply_pr-2.9.0/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      243 2020-07-17 07:18:06.000000 apply_pr-2.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4438 2020-07-17 07:17:48.000000 apply_pr-2.9.0/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-17 07:18:06.000000 apply_pr-2.9.0/apply_pr.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      243 2020-07-17 07:18:06.000000 apply_pr-2.9.0/apply_pr.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-17 07:18:06.000000 apply_pr-2.9.0/apply_pr.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2020-07-17 07:18:06.000000 apply_pr-2.9.0/apply_pr.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      318 2020-07-17 07:18:06.000000 apply_pr-2.9.0/apply_pr.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       63 2020-07-17 07:18:06.000000 apply_pr-2.9.0/apply_pr.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      107 2020-07-17 07:18:06.000000 apply_pr-2.9.0/apply_pr.egg-info/entry_points.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-17 07:18:06.000000 apply_pr-2.9.0/apply_pr/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36130 2020-07-17 07:17:48.000000 apply_pr-2.9.0/apply_pr/fabfile.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8748 2020-07-17 07:17:48.000000 apply_pr-2.9.0/apply_pr/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      658 2020-07-17 07:17:48.000000 apply_pr-2.9.0/apply_pr/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      148 2020-07-17 07:17:48.000000 apply_pr-2.9.0/apply_pr/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-07-17 07:18:06.000000 apply_pr-2.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      555 2020-07-17 07:17:48.000000 apply_pr-2.9.0/setup.py
```

### Comparing `apply_pr-2.8.2/README.md` & `apply_pr-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `apply_pr-2.8.2/apply_pr/fabfile.py` & `apply_pr-2.9.0/apply_pr/fabfile.py`

 * *Files identical despite different names*

### Comparing `apply_pr-2.8.2/apply_pr/cli.py` & `apply_pr-2.9.0/apply_pr/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,19 @@
         help='Milestone to get the issues from (version)'),
     click.option('--issues/--no-issues', default=False, show_default=True,
         help='Also get the data on the issues'),
     click.option('--changelog_path', default='/tmp', show_default=True,
         help='Path to drop the changelog file in'),
 ]
 
+mark_deployed_options = github_options + [
+    click.option("--pr", help="Pull request to apply", required=True),
+    click.option("--force-hostname", help="Force hostname",  default=False),
+]
+
 def add_options(options):
     def _add_options(func):
         for option in reversed(options):
             func = option(func)
         return func
     return _add_options
 
@@ -181,14 +186,28 @@
 @sastre.command(name='status')
 @add_options(status_options)
 def status(**kwargs):
     """Update the status of a deploy into GitHub"""
     status_pr(**kwargs)
 
 
+@sastre.command(name='mark_deployed')
+@add_options(mark_deployed_options)
+def mark_deployed(pr, force_hostname=False, owner='gisce', repository='erp'):
+    from apply_pr import fabfile
+
+    configure_logging()
+
+    mark_deployed_task = WrappedCallableTask(fabfile.mark_deployed)
+    execute(mark_deployed_task, pr, hostname=force_hostname, owner=owner, repository=repository)
+    click.echo(colors.green(u"Marking PR#{} as deployed success! \U0001F680".format(
+        pr
+    )))
+
+
 def check_prs_status(prs, separator, version, owner, repository):
     """Check the status of the PRs for a set of PRs"""
     from apply_pr import fabfile
 
     log_level = getattr(logging, os.environ.get('LOG_LEVEL', 'INFO').upper())
     logging.basicConfig(level=log_level)
```

### Comparing `apply_pr-2.8.2/apply_pr/version.py` & `apply_pr-2.9.0/apply_pr/version.py`

 * *Files identical despite different names*

### Comparing `apply_pr-2.8.2/setup.py` & `apply_pr-2.9.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt', 'r') as f:
     INSTALL_REQUIRES = f.readlines()
 
 setup(
     name='apply_pr',
-    version='2.8.2',
+    version='2.9.0',
     packages=find_packages(),
     url='https://github.com/gisce/apply_pr',
     license='MIT',
     author='GISCE-TI, S.L.',
     author_email='devel@gisce.net',
     description='Apply Pull Requests from GitHub',
     entry_points='''
```

