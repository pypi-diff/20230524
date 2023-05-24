# Comparing `tmp/pygments_git-1.3.0.tar.gz` & `tmp/pygments_git-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygments_git-1.3.0.tar", last modified: Mon Apr 17 21:00:58 2023, max compression
+gzip compressed data, was "pygments_git-1.4.0.tar", last modified: Wed May 24 10:37:39 2023, max compression
```

## Comparing `pygments_git-1.3.0.tar` & `pygments_git-1.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-17 21:00:58.778544 pygments_git-1.3.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      463 2023-04-17 21:00:56.000000 pygments_git-1.3.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2023-04-01 11:07:54.000000 pygments_git-1.3.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-04-01 11:04:32.000000 pygments_git-1.3.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4594 2023-04-17 21:00:58.778603 pygments_git-1.3.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3444 2023-04-10 17:30:19.000000 pygments_git-1.3.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-04-01 13:54:14.000000 pygments_git-1.3.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1809 2023-04-17 21:00:58.778910 pygments_git-1.3.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-17 21:00:58.776178 pygments_git-1.3.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-17 21:00:58.777387 pygments_git-1.3.0/src/pygments_git/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    13092 2023-04-17 21:00:53.000000 pygments_git-1.3.0/src/pygments_git/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-04-01 11:04:33.000000 pygments_git-1.3.0/src/pygments_git/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-17 21:00:58.778314 pygments_git-1.3.0/src/pygments_git.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4594 2023-04-17 21:00:58.000000 pygments_git-1.3.0/src/pygments_git.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      432 2023-04-17 21:00:58.000000 pygments_git-1.3.0/src/pygments_git.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-04-17 21:00:58.000000 pygments_git-1.3.0/src/pygments_git.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)      322 2023-04-17 21:00:58.000000 pygments_git-1.3.0/src/pygments_git.egg-info/entry_points.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-04-17 21:00:58.000000 pygments_git-1.3.0/src/pygments_git.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)        9 2023-04-17 21:00:58.000000 pygments_git-1.3.0/src/pygments_git.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       13 2023-04-17 21:00:58.000000 pygments_git-1.3.0/src/pygments_git.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-17 21:00:58.778432 pygments_git-1.3.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     9332 2023-04-17 21:00:53.000000 pygments_git-1.3.0/tests/test_pygments_git.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-24 10:37:39.409635 pygments_git-1.4.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      635 2023-05-24 10:37:37.000000 pygments_git-1.4.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2023-04-01 11:07:54.000000 pygments_git-1.4.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-04-01 11:04:32.000000 pygments_git-1.4.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4594 2023-05-24 10:37:39.409699 pygments_git-1.4.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3444 2023-04-10 17:30:19.000000 pygments_git-1.4.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-04-01 13:54:14.000000 pygments_git-1.4.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1809 2023-05-24 10:37:39.410003 pygments_git-1.4.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-24 10:37:39.407634 pygments_git-1.4.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-24 10:37:39.408620 pygments_git-1.4.0/src/pygments_git/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    13568 2023-05-24 10:36:44.000000 pygments_git-1.4.0/src/pygments_git/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-04-01 11:04:33.000000 pygments_git-1.4.0/src/pygments_git/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-24 10:37:39.409406 pygments_git-1.4.0/src/pygments_git.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4594 2023-05-24 10:37:39.000000 pygments_git-1.4.0/src/pygments_git.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      432 2023-05-24 10:37:39.000000 pygments_git-1.4.0/src/pygments_git.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-05-24 10:37:39.000000 pygments_git-1.4.0/src/pygments_git.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      322 2023-05-24 10:37:39.000000 pygments_git-1.4.0/src/pygments_git.egg-info/entry_points.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-05-24 10:37:39.000000 pygments_git-1.4.0/src/pygments_git.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        9 2023-05-24 10:37:39.000000 pygments_git-1.4.0/src/pygments_git.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       13 2023-05-24 10:37:39.000000 pygments_git-1.4.0/src/pygments_git.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-24 10:37:39.409525 pygments_git-1.4.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    10328 2023-05-24 10:36:44.000000 pygments_git-1.4.0/tests/test_pygments_git.py
```

### Comparing `pygments_git-1.3.0/LICENSE` & `pygments_git-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygments_git-1.3.0/PKG-INFO` & `pygments_git-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygments_git
-Version: 1.3.0
+Version: 1.4.0
 Summary: Pygments lexers for Git output and files.
 Home-page: https://github.com/adamchainz/pygments-git
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/pygments-git/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
```

### Comparing `pygments_git-1.3.0/README.rst` & `pygments_git-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `pygments_git-1.3.0/setup.cfg` & `pygments_git-1.4.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pygments_git
-version = 1.3.0
+version = 1.4.0
 description = Pygments lexers for Git output and files.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/pygments-git
 author = Adam Johnson
 author_email = me@adamj.eu
 license = MIT
```

### Comparing `pygments_git-1.3.0/src/pygments_git/__init__.py` & `pygments_git-1.4.0/src/pygments_git/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -211,20 +211,19 @@
                     Generic.Output,
                     Name.Label,
                     Generic.Output,
                 ),
             ),
             # git log
             (
-                r"^(commit)( )([0-9a-f]{40})( )(\(.*?\))?$",
+                r"^(commit)( )([0-9a-f]{40})( \(.*?\))?$",
                 bygroups(  # type: ignore [no-untyped-call]
                     Generic.Subheading,
                     Generic.Output,
                     Number.Hex,
-                    Generic.Output,
                     Name.Label,
                 ),
             ),
             (
                 r"""(?x)
                     ^
                     ((?:Author|AuthorDate|Commit|CommitDate|Date):)
@@ -235,14 +234,28 @@
                 bygroups(  # type: ignore [no-untyped-call]
                     Keyword.Declaration,
                     Generic.Output,
                     String.Symbol,
                 ),
             ),
             (
+                r"""(?x)
+                    ^
+                    (Merge:)
+                    (\ +)
+                    (.*)
+                    $
+                """,
+                bygroups(  # type: ignore [no-untyped-call]
+                    Keyword.Declaration,
+                    Generic.Output,
+                    Number.Hex,
+                ),
+            ),
+            (
                 r"""(?xi)
                     ^
                     (\ *)
                     ((?:co-authored|signed-off)-by:)
                     (\ +)
                     (.*)
                     $
@@ -260,14 +273,17 @@
                 bygroups(  # type: ignore [no-untyped-call]
                     Name.Label,
                     Number.Hex,
                     Name.Label,
                     Generic.Output,
                 ),
             ),
+            # hints and errors
+            (r"^hint:.*$", Comment.Single),
+            (r"^(error|fatal):.*$", Generic.Error),
             # Any SHA to be highlighted as such
             (r"\b([0-9a-f]{40}|[0-9a-f]{7})\b", Number.Hex),
             # Diff lines
             (r"^diff --git.*$", Generic.Heading),
             (
                 r"""(?x)^
                     (index\ )
```

### Comparing `pygments_git-1.3.0/src/pygments_git.egg-info/PKG-INFO` & `pygments_git-1.4.0/src/pygments_git.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygments-git
-Version: 1.3.0
+Version: 1.4.0
 Summary: Pygments lexers for Git output and files.
 Home-page: https://github.com/adamchainz/pygments-git
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/pygments-git/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
```

### Comparing `pygments_git-1.3.0/tests/test_pygments_git.py` & `pygments_git-1.4.0/tests/test_pygments_git.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,16 +44,17 @@
                 lexer=get_lexer_by_name(lexer, stripnl=False),
                 formatter=formatter,
             )
             result = str(BeautifulSoup(result, "html.parser")).strip()
             self.cases[testid] = (lexer, given, result)
             if not save and testid in loaded_cases:  # pragma: no branch
                 loaded_lexer, loaded_given, loaded_result = loaded_cases[testid]
-                if lexer == loaded_lexer and given == loaded_given:  # pragma: no branch
-                    assert result == loaded_result
+                assert loaded_lexer == lexer
+                assert loaded_given == given
+                assert result == loaded_result
 
     checker = Checker()
 
     yield checker
 
     if save:  # pragma: no cover
         lines = [
@@ -237,16 +238,39 @@
         index 3eb29f0..ed3581b 100644
         --- it.txt
         +++ it.txt
         @@ -1 +1 @@
         -twisted
         +bopped
 
+        $ git show 362fdb8
+        commit 362fdb88072ca0259e9f6e0251b47af4d75e141c
+        Merge: 8456fa3 722568d
+        Author: A Hacker <hacker9001@funmail.example>
+        Date:   ...
+
+            Merge branch 'jig'
+
         $ git commit -m "Spin it"
         [main 0bcdb8f] Spin it
+
+        $ git pull
+        hint: You have divergent branches and need to specify how to reconcile them.
+        hint: You can do so by running one of the following commands sometime before
+        hint: your next pull:
+        hint:
+        hint:   git config pull.rebase false  # merge
+        hint:   git config pull.rebase true   # rebase
+        hint:   git config pull.ff only       # fast-forward only
+        hint:
+        hint: You can replace "git config" with "git config --global" to set a default
+        hint: preference for all repositories. You can also pass --rebase, --no-rebase,
+        hint: or --ff-only on the command line to override the configured default per
+        hint: invocation.
+        fatal: Need to specify how to reconcile divergent branches.
         """,
     )
 
 
 def test_git_ignore(golden_file):
     golden_file.check(
         "test_git_ignore",
```

