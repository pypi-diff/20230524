# Comparing `tmp/giscemultitools-1.0.2.tar.gz` & `tmp/giscemultitools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giscemultitools-1.0.2.tar", last modified: Thu Apr 27 09:36:05 2023, max compression
+gzip compressed data, was "giscemultitools-1.1.0.tar", last modified: Wed May 24 06:27:18 2023, max compression
```

## Comparing `giscemultitools-1.0.2.tar` & `giscemultitools-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:36:05.695651 giscemultitools-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-27 09:36:05.695651 giscemultitools-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:36:05.691651 giscemultitools-1.0.2/giscemultitools/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/giscemultitools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:36:05.691651 giscemultitools-1.0.2/giscemultitools/githubutils/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/giscemultitools/githubutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/giscemultitools/githubutils/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:36:05.695651 giscemultitools-1.0.2/giscemultitools/githubutils/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/giscemultitools/githubutils/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/giscemultitools/githubutils/scripts/github_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/giscemultitools/githubutils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:36:05.695651 giscemultitools-1.0.2/giscemultitools/slackutils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/giscemultitools/slackutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:36:05.695651 giscemultitools-1.0.2/giscemultitools/slackutils/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/giscemultitools/slackutils/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/giscemultitools/slackutils/scripts/slack_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/giscemultitools/slackutils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:36:05.691651 giscemultitools-1.0.2/giscemultitools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-27 09:36:05.000000 giscemultitools-1.0.2/giscemultitools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-27 09:36:05.000000 giscemultitools-1.0.2/giscemultitools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:36:05.000000 giscemultitools-1.0.2/giscemultitools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 09:36:05.000000 giscemultitools-1.0.2/giscemultitools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 09:36:05.000000 giscemultitools-1.0.2/giscemultitools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 09:36:05.000000 giscemultitools-1.0.2/giscemultitools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 09:36:05.695651 giscemultitools-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:27:18.879965 giscemultitools-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-24 06:27:18.879965 giscemultitools-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 06:27:16.000000 giscemultitools-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:27:18.879965 giscemultitools-1.1.0/giscemultitools/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-24 06:27:16.000000 giscemultitools-1.1.0/giscemultitools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:27:18.879965 giscemultitools-1.1.0/giscemultitools/githubutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-24 06:27:16.000000 giscemultitools-1.1.0/giscemultitools/githubutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-24 06:27:16.000000 giscemultitools-1.1.0/giscemultitools/githubutils/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:27:18.879965 giscemultitools-1.1.0/giscemultitools/githubutils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-24 06:27:16.000000 giscemultitools-1.1.0/giscemultitools/githubutils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-24 06:27:16.000000 giscemultitools-1.1.0/giscemultitools/githubutils/scripts/github_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-05-24 06:27:16.000000 giscemultitools-1.1.0/giscemultitools/githubutils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:27:18.879965 giscemultitools-1.1.0/giscemultitools/slackutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-24 06:27:16.000000 giscemultitools-1.1.0/giscemultitools/slackutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:27:18.879965 giscemultitools-1.1.0/giscemultitools/slackutils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-24 06:27:16.000000 giscemultitools-1.1.0/giscemultitools/slackutils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-24 06:27:16.000000 giscemultitools-1.1.0/giscemultitools/slackutils/scripts/slack_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-24 06:27:16.000000 giscemultitools-1.1.0/giscemultitools/slackutils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:27:18.879965 giscemultitools-1.1.0/giscemultitools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-24 06:27:18.000000 giscemultitools-1.1.0/giscemultitools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-24 06:27:18.000000 giscemultitools-1.1.0/giscemultitools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 06:27:18.000000 giscemultitools-1.1.0/giscemultitools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 06:27:18.000000 giscemultitools-1.1.0/giscemultitools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 06:27:18.000000 giscemultitools-1.1.0/giscemultitools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 06:27:18.000000 giscemultitools-1.1.0/giscemultitools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 06:27:18.879965 giscemultitools-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-24 06:27:16.000000 giscemultitools-1.1.0/setup.py
```

### Comparing `giscemultitools-1.0.2/giscemultitools/githubutils/objects.py` & `giscemultitools-1.1.0/giscemultitools/githubutils/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,17 @@
                 repository(owner: "%s", name: "%s") {
                     pullRequest(number: %s) {
                         baseRefName
                         number
                         state
                         url
                         title
+                        mergedAt
+                        createdAt
+
                         milestone {
                           title
                         }
 
                         mergeCommit {
                             oid
                         }
```

### Comparing `giscemultitools-1.0.2/giscemultitools/githubutils/scripts/github_cli.py` & `giscemultitools-1.1.0/giscemultitools/githubutils/scripts/github_cli.py`

 * *Files identical despite different names*

### Comparing `giscemultitools-1.0.2/giscemultitools/githubutils/utils.py` & `giscemultitools-1.1.0/giscemultitools/githubutils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
             'pullRequest': {
                 'number': response['data']['repository']['pullRequest']['number'],
                 'state': response['data']['repository']['pullRequest']['state'],
                 'milestone': response['data']['repository']['pullRequest']['milestone'] and response['data']['repository']['pullRequest']['milestone']['title'] or '',
                 'url': response['data']['repository']['pullRequest']['url'],
                 'title': response['data']['repository']['pullRequest']['title'],
                 'baseRefName': response['data']['repository']['pullRequest']['baseRefName'],
+                'mergedAt': response['data']['repository']['pullRequest']['mergedAt'],
+                'createdAt': response['data']['repository']['pullRequest']['createdAt'],
                 'labels': response['data']['repository']['pullRequest']['labels']['nodes']
             },
             'projectItems': []
         }
         for card in response['data']['repository']['pullRequest']['projectItems']['nodes']:
             pos_status = 0
             for i, node in enumerate(card['fieldValues']['nodes']):
```

### Comparing `giscemultitools-1.0.2/giscemultitools/slackutils/scripts/slack_cli.py` & `giscemultitools-1.1.0/giscemultitools/slackutils/scripts/slack_cli.py`

 * *Files identical despite different names*

### Comparing `giscemultitools-1.0.2/giscemultitools/slackutils/utils.py` & `giscemultitools-1.1.0/giscemultitools/slackutils/utils.py`

 * *Files identical despite different names*

### Comparing `giscemultitools-1.0.2/giscemultitools.egg-info/SOURCES.txt` & `giscemultitools-1.1.0/giscemultitools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `giscemultitools-1.0.2/setup.py` & `giscemultitools-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 setup(
     name='giscemultitools',
     description='Llibreria d\'utilitats',
     author='GISCE',
     author_email='devel@gisce.net',
     url='http://www.gisce.net',
-    version='1.0.2',
+    version='1.1.0',
     license='General Public Licence 2',
     long_description='''Long description''',
     provides=['giscemultitools'],
     install_requires=[
         "requests",
         "click"
     ],
```

