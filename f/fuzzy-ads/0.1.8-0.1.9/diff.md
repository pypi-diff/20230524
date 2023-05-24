# Comparing `tmp/fuzzy-ads-0.1.8.tar.gz` & `tmp/fuzzy-ads-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzy-ads-0.1.8.tar", max compression
+gzip compressed data, was "fuzzy-ads-0.1.9.tar", max compression
```

## Comparing `fuzzy-ads-0.1.8.tar` & `fuzzy-ads-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2022-03-07 23:16:36.253500 fuzzy-ads-0.1.8/LICENSE
--rw-r--r--   0        0        0       22 2022-04-05 14:31:51.461244 fuzzy-ads-0.1.8/fuzzy_ads/__init__.py
--rw-r--r--   0        0        0     1714 2022-03-12 11:06:49.984556 fuzzy-ads-0.1.8/fuzzy_ads/cli.py
--rw-r--r--   0        0        0     8447 2022-04-05 14:28:58.944311 fuzzy-ads-0.1.8/fuzzy_ads/query.py
--rw-r--r--   0        0        0      655 2022-04-05 14:31:45.341211 fuzzy-ads-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      867 2022-04-05 14:32:09.722541 fuzzy-ads-0.1.8/setup.py
--rw-r--r--   0        0        0      753 2022-04-05 14:32:09.723133 fuzzy-ads-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-03-07 23:16:36.253500 fuzzy-ads-0.1.9/LICENSE
+-rw-r--r--   0        0        0       22 2022-04-05 14:31:51.461244 fuzzy-ads-0.1.9/fuzzy_ads/__init__.py
+-rw-r--r--   0        0        0     1714 2022-03-12 11:06:49.984556 fuzzy-ads-0.1.9/fuzzy_ads/cli.py
+-rw-r--r--   0        0        0     8670 2022-05-16 09:30:24.215072 fuzzy-ads-0.1.9/fuzzy_ads/query.py
+-rw-r--r--   0        0        0      655 2022-05-16 09:32:03.507716 fuzzy-ads-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      867 2022-05-16 09:34:06.374096 fuzzy-ads-0.1.9/setup.py
+-rw-r--r--   0        0        0      753 2022-05-16 09:34:06.374663 fuzzy-ads-0.1.9/PKG-INFO
```

### Comparing `fuzzy-ads-0.1.8/LICENSE` & `fuzzy-ads-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fuzzy-ads-0.1.8/fuzzy_ads/cli.py` & `fuzzy-ads-0.1.9/fuzzy_ads/cli.py`

 * *Files identical despite different names*

### Comparing `fuzzy-ads-0.1.8/fuzzy_ads/query.py` & `fuzzy-ads-0.1.9/fuzzy_ads/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                 " " * shutil.get_terminal_size()[0],
                 paper.title[0] if paper.title is not None else "-",
             ]
         )
 
         # Flush article line to fzf choices
         LINE = (
-            f"{PREFIX}{FZF_LINE_FORMAT(paper)}{POSTFIX}{HIDDEN_TITLE}".encode(
+            f"{PREFIX}{paper.bibcode}:{_format_authors(paper)}{POSTFIX}{HIDDEN_TITLE}".encode(
                 sys.getdefaultencoding()
             )
             + b"\n"
         )
 
         if "REFEREED" in paper.property:
             refereed.append(LINE)
@@ -197,14 +197,28 @@
         for data in response.iter_content(chunk_size=1024):
             size = file.write(data)
             bar.update(task, advance=size)
 
 
 # ------
 # Settings
+def _format_authors(paper):
+    """Format the first three authors of a paper, append 'et al.' in case there is more than 3."""
+
+    if paper.author is not None:
+
+        author = " & ".join(paper.author[:3])
+
+        if len(paper.author) > 3:
+            author = author + ", et al."
+    else:
+        author = "-"
+
+    return author
+
 
 # Tempfiles for fzf input
 FILE_ALL = Path(tempfile.gettempdir()) / "ads_all.input"
 FILE_NONREFEREED = Path(tempfile.gettempdir()) / "ads_nonrefereed.input"
 FILE_REFEREED = Path(tempfile.gettempdir()) / "ads_refereed.input"
 
 
@@ -216,17 +230,14 @@
     "--preview-window",
     "up,1",
     "--bind",
     f"ctrl-a:reload(cat {FILE_ALL}),ctrl-f:reload(cat {FILE_NONREFEREED}),ctrl-r:reload(cat {FILE_REFEREED})",
     "--header",
     "ctrl-a: all entries  | ctrl-f: non-refereed only | ctrl-r: refereed only",
 ]
-FZF_LINE_FORMAT = (
-    lambda paper: f"{paper.bibcode}: {' & '.join(paper.author[:3]) if paper.author is not None else '-'}"
-)
 
 # Colours for fzf lines
 COLOUR_NO_OPENACCESS = "\033[2m"
 COLOUR_RESET = "\033[0m"
 
 # Article fields to query from ADS
 QUERY_FIELDS = ["author", "bibcode", "year", "title", "property", "esources", "doi"]
```

### Comparing `fuzzy-ads-0.1.8/pyproject.toml` & `fuzzy-ads-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fuzzy-ads"
-version = "0.1.8"
+version = "0.1.9"
 description = "Unofficial Command Line Interface the SAO/NASA Astrophysics Data System"
 authors = ["Max Mahlke <max.mahlke@oca.eu>"]
 homepage = "https://github.com/maxmahlke/fuzzy-ads"
 documentation = "https://github.com/maxmahlke/fuzzy-ads"
 repository = "https://github.com/maxmahlke/fuzzy-ads.git"
 
 [tool.poetry.dependencies]
```

### Comparing `fuzzy-ads-0.1.8/setup.py` & `fuzzy-ads-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'rich>=11.2.0,<12.0.0']
 
 entry_points = \
 {'console_scripts': ['ads = fuzzy_ads.cli:cli']}
 
 setup_kwargs = {
     'name': 'fuzzy-ads',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Unofficial Command Line Interface the SAO/NASA Astrophysics Data System',
     'long_description': None,
     'author': 'Max Mahlke',
     'author_email': 'max.mahlke@oca.eu',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/maxmahlke/fuzzy-ads',
```

### Comparing `fuzzy-ads-0.1.8/PKG-INFO` & `fuzzy-ads-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzy-ads
-Version: 0.1.8
+Version: 0.1.9
 Summary: Unofficial Command Line Interface the SAO/NASA Astrophysics Data System
 Home-page: https://github.com/maxmahlke/fuzzy-ads
 Author: Max Mahlke
 Author-email: max.mahlke@oca.eu
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

