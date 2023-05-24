# Comparing `tmp/mysmallutils-2.0.4.tar.gz` & `tmp/mysmallutils-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysmallutils-2.0.4.tar", last modified: Tue May 23 11:37:14 2023, max compression
+gzip compressed data, was "mysmallutils-2.0.5.tar", last modified: Wed May 24 12:30:21 2023, max compression
```

## Comparing `mysmallutils-2.0.4.tar` & `mysmallutils-2.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 11:37:14.033808 mysmallutils-2.0.4/
--rw-rw-rw-   0        0        0    58702 2023-05-23 11:37:14.032805 mysmallutils-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    58220 2023-05-23 11:31:29.000000 mysmallutils-2.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 11:37:13.998338 mysmallutils-2.0.4/mysmallutils.egg-info/
--rw-rw-rw-   0        0        0    58702 2023-05-23 11:37:13.000000 mysmallutils-2.0.4/mysmallutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-05-23 11:37:13.000000 mysmallutils-2.0.4/mysmallutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 11:37:13.000000 mysmallutils-2.0.4/mysmallutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 11:37:13.000000 mysmallutils-2.0.4/mysmallutils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-23 11:37:14.030804 mysmallutils-2.0.4/mysutils/
--rw-rw-rw-   0        0        0        0 2023-02-06 15:28:27.000000 mysmallutils-2.0.4/mysutils/__init__.py
--rw-rw-rw-   0        0        0    22982 2023-02-07 14:39:08.000000 mysmallutils-2.0.4/mysutils/collections.py
--rw-rw-rw-   0        0        0     1533 2023-02-06 15:28:27.000000 mysmallutils-2.0.4/mysutils/command.py
--rw-rw-rw-   0        0        0     1753 2023-02-06 15:28:27.000000 mysmallutils-2.0.4/mysutils/config.py
--rw-rw-rw-   0        0        0     8540 2023-02-06 15:28:27.000000 mysmallutils-2.0.4/mysutils/fastapi.py
--rw-rw-rw-   0        0        0    25877 2023-02-13 14:44:23.000000 mysmallutils-2.0.4/mysutils/file.py
--rw-rw-rw-   0        0        0     2649 2023-02-06 15:28:27.000000 mysmallutils-2.0.4/mysutils/logging.py
--rw-rw-rw-   0        0        0      639 2023-02-06 15:28:27.000000 mysmallutils-2.0.4/mysutils/method.py
--rw-rw-rw-   0        0        0      467 2023-02-06 15:28:27.000000 mysmallutils-2.0.4/mysutils/misc.py
--rw-rw-rw-   0        0        0      820 2023-02-06 15:28:27.000000 mysmallutils-2.0.4/mysutils/request.py
--rw-rw-rw-   0        0        0     1861 2023-02-06 15:28:27.000000 mysmallutils-2.0.4/mysutils/service.py
--rw-rw-rw-   0        0        0    12420 2023-02-10 08:55:00.000000 mysmallutils-2.0.4/mysutils/tar.py
--rw-rw-rw-   0        0        0     8592 2023-05-23 11:22:26.000000 mysmallutils-2.0.4/mysutils/text.py
--rw-rw-rw-   0        0        0     6479 2023-02-10 13:25:04.000000 mysmallutils-2.0.4/mysutils/tmp.py
--rw-rw-rw-   0        0        0     1974 2023-02-06 15:28:27.000000 mysmallutils-2.0.4/mysutils/unittest.py
--rw-rw-rw-   0        0        0     1175 2023-02-06 15:28:27.000000 mysmallutils-2.0.4/mysutils/web.py
--rw-rw-rw-   0        0        0     3082 2023-02-07 14:39:08.000000 mysmallutils-2.0.4/mysutils/yaml.py
--rw-rw-rw-   0        0        0       42 2023-05-23 11:37:14.033808 mysmallutils-2.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1711 2023-05-23 11:35:18.000000 mysmallutils-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:30:21.254543 mysmallutils-2.0.5/
+-rw-rw-rw-   0        0        0    59126 2023-05-24 12:30:21.251538 mysmallutils-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    58644 2023-05-24 12:29:20.000000 mysmallutils-2.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 12:30:21.020679 mysmallutils-2.0.5/mysmallutils.egg-info/
+-rw-rw-rw-   0        0        0    59126 2023-05-24 12:30:20.000000 mysmallutils-2.0.5/mysmallutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-05-24 12:30:20.000000 mysmallutils-2.0.5/mysmallutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 12:30:20.000000 mysmallutils-2.0.5/mysmallutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-24 12:30:20.000000 mysmallutils-2.0.5/mysmallutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 12:30:21.246390 mysmallutils-2.0.5/mysutils/
+-rw-rw-rw-   0        0        0        0 2023-02-06 15:28:27.000000 mysmallutils-2.0.5/mysutils/__init__.py
+-rw-rw-rw-   0        0        0    22982 2023-02-07 14:39:08.000000 mysmallutils-2.0.5/mysutils/collections.py
+-rw-rw-rw-   0        0        0     1533 2023-02-06 15:28:27.000000 mysmallutils-2.0.5/mysutils/command.py
+-rw-rw-rw-   0        0        0     1753 2023-02-06 15:28:27.000000 mysmallutils-2.0.5/mysutils/config.py
+-rw-rw-rw-   0        0        0     8540 2023-02-06 15:28:27.000000 mysmallutils-2.0.5/mysutils/fastapi.py
+-rw-rw-rw-   0        0        0    25877 2023-02-13 14:44:23.000000 mysmallutils-2.0.5/mysutils/file.py
+-rw-rw-rw-   0        0        0     2649 2023-02-06 15:28:27.000000 mysmallutils-2.0.5/mysutils/logging.py
+-rw-rw-rw-   0        0        0      639 2023-02-06 15:28:27.000000 mysmallutils-2.0.5/mysutils/method.py
+-rw-rw-rw-   0        0        0      467 2023-02-06 15:28:27.000000 mysmallutils-2.0.5/mysutils/misc.py
+-rw-rw-rw-   0        0        0      820 2023-02-06 15:28:27.000000 mysmallutils-2.0.5/mysutils/request.py
+-rw-rw-rw-   0        0        0     1861 2023-02-06 15:28:27.000000 mysmallutils-2.0.5/mysutils/service.py
+-rw-rw-rw-   0        0        0    12420 2023-02-10 08:55:00.000000 mysmallutils-2.0.5/mysutils/tar.py
+-rw-rw-rw-   0        0        0     9257 2023-05-24 12:17:24.000000 mysmallutils-2.0.5/mysutils/text.py
+-rw-rw-rw-   0        0        0     6479 2023-02-10 13:25:04.000000 mysmallutils-2.0.5/mysutils/tmp.py
+-rw-rw-rw-   0        0        0     1974 2023-02-06 15:28:27.000000 mysmallutils-2.0.5/mysutils/unittest.py
+-rw-rw-rw-   0        0        0     1175 2023-02-06 15:28:27.000000 mysmallutils-2.0.5/mysutils/web.py
+-rw-rw-rw-   0        0        0     3082 2023-02-07 14:39:08.000000 mysmallutils-2.0.5/mysutils/yaml.py
+-rw-rw-rw-   0        0        0       42 2023-05-24 12:30:21.254543 mysmallutils-2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1711 2023-05-24 09:51:44.000000 mysmallutils-2.0.5/setup.py
```

### Comparing `mysmallutils-2.0.4/PKG-INFO` & `mysmallutils-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysmallutils
-Version: 2.0.4
+Version: 2.0.5
 Summary: Small Python utils to do life easier.
 Home-page: https://github.com/jmgomezsoriano/mysmallutils
 Author: José Manuel Gómez Soriano
 Author-email: jmgomez.soriano@gmail.com
 License: LGPL2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -31,14 +31,15 @@
   * [Tuples](#tuples)
   * [OrderedSet](#orderedset)
 * [Text](#text)
   * [Find URLs](#find-urls)
   * [Get URLs](#get-urls)
   * [Remove URLs](#remove-urls)
   * [Replace URLs](#replace-urls)
+  * [Check URLs in a text](#check-urls-in-a-text)
   * [Clean text](#clean-text)
   * [Text markup](#text-markup)
 * [File access, load and save files](#file-access-load-and-save-files)
   * [Open files](#open-files)
   * [Read file](#read-file)
   * [Write in a file](#write-in-a-file)
   * [Load and save json files](#load-and-save-json-files)
@@ -729,14 +730,29 @@
 # Replace only the url with the path /my_space/user
 replace_urls(text, 'https://hello.com', r'my_space/user')
 # Result:
 # 'This is a test!\n
 #      Clean punctuation symbols and urls like this: https://hello.com https://example.com/your_space')
 ```
 
+## Check URLs in a text<a id="check-urls-in-a-text" name="check-urls-in-a-text"></a>
+Check if a text is a URL or contain one.
+
+```python
+from mysutils.text import is_url, has_url
+
+text = '...'
+# Check if a text is a URL
+if is_url(text):
+  print('It is a URL!')
+# Check if a text contains a URL
+if has_url(text):
+  print('It contains, at least, a URL!')
+```
+
 ## Clean text<a id="clean-text" name="clean-text"></a>
 Remove punctuation symbols, urls and convert to lower.
 
 ```python
 from mysutils.text import clean_text
 
 text = 'This is a test!\n     Clean punctuation symbols and urls like this: ' \
```

### Comparing `mysmallutils-2.0.4/README.md` & `mysmallutils-2.0.5/mysmallutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: mysmallutils
+Version: 2.0.5
+Summary: Small Python utils to do life easier.
+Home-page: https://github.com/jmgomezsoriano/mysmallutils
+Author: José Manuel Gómez Soriano
+Author-email: jmgomez.soriano@gmail.com
+License: LGPL2
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10,<4
+Description-Content-Type: text/markdown
+
 # MySmallUtils
 Small Python utils to do life easier.
 
 This includes tools to execute external commands, compress files,
 manage configuration files, open different types of files (JSON, YAML and Pickle) compressed or not,
 configure logging, obtain metrics, download files, etc.
 
@@ -17,14 +31,15 @@
   * [Tuples](#tuples)
   * [OrderedSet](#orderedset)
 * [Text](#text)
   * [Find URLs](#find-urls)
   * [Get URLs](#get-urls)
   * [Remove URLs](#remove-urls)
   * [Replace URLs](#replace-urls)
+  * [Check URLs in a text](#check-urls-in-a-text)
   * [Clean text](#clean-text)
   * [Text markup](#text-markup)
 * [File access, load and save files](#file-access-load-and-save-files)
   * [Open files](#open-files)
   * [Read file](#read-file)
   * [Write in a file](#write-in-a-file)
   * [Load and save json files](#load-and-save-json-files)
@@ -715,14 +730,29 @@
 # Replace only the url with the path /my_space/user
 replace_urls(text, 'https://hello.com', r'my_space/user')
 # Result:
 # 'This is a test!\n
 #      Clean punctuation symbols and urls like this: https://hello.com https://example.com/your_space')
 ```
 
+## Check URLs in a text<a id="check-urls-in-a-text" name="check-urls-in-a-text"></a>
+Check if a text is a URL or contain one.
+
+```python
+from mysutils.text import is_url, has_url
+
+text = '...'
+# Check if a text is a URL
+if is_url(text):
+  print('It is a URL!')
+# Check if a text contains a URL
+if has_url(text):
+  print('It contains, at least, a URL!')
+```
+
 ## Clean text<a id="clean-text" name="clean-text"></a>
 Remove punctuation symbols, urls and convert to lower.
 
 ```python
 from mysutils.text import clean_text
 
 text = 'This is a test!\n     Clean punctuation symbols and urls like this: ' \
@@ -1741,8 +1771,8 @@
 
 # You can do
 conditional(my_func, a > b, 1, 'apple', c='Lucas')
 ```
 
 # How to collaborate
 
-I you want to collaborate with this project, please, <a href="mailto:jmgomez.soriano@gmail.com">contact with me</a>.
+I you want to collaborate with this project, please, <a href="mailto:jmgomez.soriano@gmail.com">contact with me</a>.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mysmallutils-2.0.4/mysmallutils.egg-info/PKG-INFO` & `mysmallutils-2.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: mysmallutils
-Version: 2.0.4
-Summary: Small Python utils to do life easier.
-Home-page: https://github.com/jmgomezsoriano/mysmallutils
-Author: José Manuel Gómez Soriano
-Author-email: jmgomez.soriano@gmail.com
-License: LGPL2
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10,<4
-Description-Content-Type: text/markdown
-
 # MySmallUtils
 Small Python utils to do life easier.
 
 This includes tools to execute external commands, compress files,
 manage configuration files, open different types of files (JSON, YAML and Pickle) compressed or not,
 configure logging, obtain metrics, download files, etc.
 
@@ -31,14 +17,15 @@
   * [Tuples](#tuples)
   * [OrderedSet](#orderedset)
 * [Text](#text)
   * [Find URLs](#find-urls)
   * [Get URLs](#get-urls)
   * [Remove URLs](#remove-urls)
   * [Replace URLs](#replace-urls)
+  * [Check URLs in a text](#check-urls-in-a-text)
   * [Clean text](#clean-text)
   * [Text markup](#text-markup)
 * [File access, load and save files](#file-access-load-and-save-files)
   * [Open files](#open-files)
   * [Read file](#read-file)
   * [Write in a file](#write-in-a-file)
   * [Load and save json files](#load-and-save-json-files)
@@ -729,14 +716,29 @@
 # Replace only the url with the path /my_space/user
 replace_urls(text, 'https://hello.com', r'my_space/user')
 # Result:
 # 'This is a test!\n
 #      Clean punctuation symbols and urls like this: https://hello.com https://example.com/your_space')
 ```
 
+## Check URLs in a text<a id="check-urls-in-a-text" name="check-urls-in-a-text"></a>
+Check if a text is a URL or contain one.
+
+```python
+from mysutils.text import is_url, has_url
+
+text = '...'
+# Check if a text is a URL
+if is_url(text):
+  print('It is a URL!')
+# Check if a text contains a URL
+if has_url(text):
+  print('It contains, at least, a URL!')
+```
+
 ## Clean text<a id="clean-text" name="clean-text"></a>
 Remove punctuation symbols, urls and convert to lower.
 
 ```python
 from mysutils.text import clean_text
 
 text = 'This is a test!\n     Clean punctuation symbols and urls like this: ' \
@@ -1755,8 +1757,8 @@
 
 # You can do
 conditional(my_func, a > b, 1, 'apple', c='Lucas')
 ```
 
 # How to collaborate
 
-I you want to collaborate with this project, please, <a href="mailto:jmgomez.soriano@gmail.com">contact with me</a>.
+I you want to collaborate with this project, please, <a href="mailto:jmgomez.soriano@gmail.com">contact with me</a>.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mysmallutils-2.0.4/mysutils/collections.py` & `mysmallutils-2.0.5/mysutils/collections.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.4/mysutils/command.py` & `mysmallutils-2.0.5/mysutils/command.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.4/mysutils/config.py` & `mysmallutils-2.0.5/mysutils/config.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.4/mysutils/fastapi.py` & `mysmallutils-2.0.5/mysutils/fastapi.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.4/mysutils/file.py` & `mysmallutils-2.0.5/mysutils/file.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.4/mysutils/logging.py` & `mysmallutils-2.0.5/mysutils/logging.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.4/mysutils/method.py` & `mysmallutils-2.0.5/mysutils/method.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.4/mysutils/request.py` & `mysmallutils-2.0.5/mysutils/request.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.4/mysutils/service.py` & `mysmallutils-2.0.5/mysutils/service.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.4/mysutils/tar.py` & `mysmallutils-2.0.5/mysutils/tar.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.4/mysutils/text.py` & `mysmallutils-2.0.5/mysutils/text.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,46 @@
 import re
 from enum import Enum, unique
 from re import Match
 from typing import Union, Iterator, List
 
-URL_PATTERN = r'[A-Za-z0-9]+://[A-Za-z0-9%-_]+(/[A-Za-z0-9%-_])*(#|\\?)[A-Za-z0-9%-_&=]*'
+PROTOCOL_PATTERN = r'([\w\+]+://)?'
+DOMAIN_PATTERN = r'\w[\w%@:\-_]+(\.\w[\w%@:\-_]*)+/?'
+PATH_PATTERN = r'([\w%@\.\-_]+/?)*'
+QUERY_PATTERN = r'(\?[\w%\-_&=]*)?'
+HASH_PATTERN = r'(#[\w%\-_&=]*)*'
+URL_PATTERN = PROTOCOL_PATTERN + DOMAIN_PATTERN + PATH_PATTERN + QUERY_PATTERN + HASH_PATTERN
 
 
 def find_urls(text: str, end_with: str = '') -> Iterator[Match[str]]:
     """ Find all the urls in the text.
     :param text: The text to search in.
     :param end_with: If set, only remove the URLs that finish with that regular expression.
         By default, all the URLs are matched.
     :return: An iterator over the url matches.
     """
     return re.finditer(URL_PATTERN + end_with, text)
 
 
+def is_url(text: str) -> bool:
+    """ Check if the text is a URL.
+    :param text: The text to check.
+    :return: True if the text is a URL, False otherwise.
+    """
+    return bool(re.match(URL_PATTERN, text))
+
+
+def has_url(text: str) -> bool:
+    """ Check if the text contains a URL.
+    :param text: The text to check.
+    :return: True if the text contains a URL, False otherwise.
+    """
+    return bool(re.search(URL_PATTERN, text))
+
+
 def get_urls(text: str, end_with: str = '') -> List[str]:
     """ Get all the urls in the text.
     :param text: The text to search in.
     :param end_with: If set, only remove the URLs that finish with that regular expression.
         By default, all the URLs are returned.
     """
     return [text[match.span()[0]:match.span()[1]] for match in find_urls(text, end_with)]
```

### Comparing `mysmallutils-2.0.4/mysutils/tmp.py` & `mysmallutils-2.0.5/mysutils/tmp.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.4/mysutils/unittest.py` & `mysmallutils-2.0.5/mysutils/unittest.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.4/mysutils/web.py` & `mysmallutils-2.0.5/mysutils/web.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.4/mysutils/yaml.py` & `mysmallutils-2.0.5/mysutils/yaml.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.4/setup.py` & `mysmallutils-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 setuptools.setup(
     cmdclass={
         'clean': CleanCommand,
         'prepublish': PrepublishCommand,
     },
     name='mysmallutils',
-    version='2.0.4',
+    version='2.0.5',
     url='https://github.com/jmgomezsoriano/mysmallutils',
     license='LGPL2',
     author='José Manuel Gómez Soriano',
     author_email='jmgomez.soriano@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     description='Small Python utils to do life easier.',
```

