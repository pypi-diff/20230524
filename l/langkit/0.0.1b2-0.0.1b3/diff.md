# Comparing `tmp/langkit-0.0.1b2.tar.gz` & `tmp/langkit-0.0.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langkit-0.0.1b2.tar", max compression
+gzip compressed data, was "langkit-0.0.1b3.tar", max compression
```

## Comparing `langkit-0.0.1b2.tar` & `langkit-0.0.1b3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2259 2023-05-20 01:38:15.592537 langkit-0.0.1b2/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.1b2/LICENSE
--rw-r--r--   0        0        0      706 2023-05-19 23:22:41.142537 langkit-0.0.1b2/langkit/__init__.py
--rw-r--r--   0        0        0    16284 2023-05-20 01:39:38.002537 langkit-0.0.1b2/langkit/examples/GPT_Intro_to_LangKit.ipynb
--rw-r--r--   0        0        0     1119 2023-05-20 01:19:57.252537 langkit-0.0.1b2/langkit/input_output.py
--rw-r--r--   0        0        0      778 2023-05-19 23:17:27.872537 langkit-0.0.1b2/langkit/pattern_groups.json
--rw-r--r--   0        0        0     2505 2023-05-19 23:24:38.182537 langkit-0.0.1b2/langkit/regexes.py
--rw-r--r--   0        0        0      451 2023-05-19 23:17:27.872537 langkit-0.0.1b2/langkit/sentiment.py
--rw-r--r--   0        0        0      714 2023-05-19 23:17:27.872537 langkit-0.0.1b2/langkit/tests/conftest.py
--rw-r--r--   0        0        0     2201 2023-05-19 23:17:27.872537 langkit-0.0.1b2/langkit/tests/test_input_output.py
--rw-r--r--   0        0        0     2170 2023-05-19 23:26:15.952537 langkit-0.0.1b2/langkit/tests/test_patterns.py
--rw-r--r--   0        0        0     2273 2023-05-19 23:17:27.872537 langkit-0.0.1b2/langkit/tests/test_themes.py
--rw-r--r--   0        0        0     2289 2023-05-19 23:17:27.872537 langkit-0.0.1b2/langkit/textstat.py
--rw-r--r--   0        0        0     8896 2023-05-19 23:17:27.872537 langkit-0.0.1b2/langkit/themes.json
--rw-r--r--   0        0        0      261 2023-05-19 23:17:27.872537 langkit-0.0.1b2/langkit/themes.json.txt
--rw-r--r--   0        0        0     2869 2023-05-19 23:17:27.872537 langkit-0.0.1b2/langkit/themes.py
--rw-r--r--   0        0        0      728 2023-05-19 23:17:27.872537 langkit-0.0.1b2/langkit/toxicity.py
--rw-r--r--   0        0        0      144 2023-05-19 23:17:27.872537 langkit-0.0.1b2/langkit/transformer.py
--rw-r--r--   0        0        0      733 2023-05-22 14:55:45.182537 langkit-0.0.1b2/pyproject.toml
--rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 langkit-0.0.1b2/PKG-INFO
+-rw-r--r--   0        0        0     2259 2023-05-20 01:38:15.592537 langkit-0.0.1b3/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.1b3/LICENSE
+-rw-r--r--   0        0        0      706 2023-05-19 23:22:41.142537 langkit-0.0.1b3/langkit/__init__.py
+-rw-r--r--   0        0        0    16284 2023-05-20 01:39:38.002537 langkit-0.0.1b3/langkit/examples/GPT_Intro_to_LangKit.ipynb
+-rw-r--r--   0        0        0     1119 2023-05-20 01:19:57.252537 langkit-0.0.1b3/langkit/input_output.py
+-rw-r--r--   0        0        0      778 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/pattern_groups.json
+-rw-r--r--   0        0        0     2505 2023-05-19 23:24:38.182537 langkit-0.0.1b3/langkit/regexes.py
+-rw-r--r--   0        0        0      451 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/sentiment.py
+-rw-r--r--   0        0        0      714 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/tests/conftest.py
+-rw-r--r--   0        0        0     2201 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/tests/test_input_output.py
+-rw-r--r--   0        0        0     2170 2023-05-19 23:26:15.952537 langkit-0.0.1b3/langkit/tests/test_patterns.py
+-rw-r--r--   0        0        0     2273 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/tests/test_themes.py
+-rw-r--r--   0        0        0     2289 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/textstat.py
+-rw-r--r--   0        0        0     8896 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/themes.json
+-rw-r--r--   0        0        0      261 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/themes.json.txt
+-rw-r--r--   0        0        0     2869 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/themes.py
+-rw-r--r--   0        0        0      728 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/toxicity.py
+-rw-r--r--   0        0        0      144 2023-05-19 23:17:27.872537 langkit-0.0.1b3/langkit/transformer.py
+-rw-r--r--   0        0        0      749 2023-05-23 22:38:43.492537 langkit-0.0.1b3/pyproject.toml
+-rw-r--r--   0        0        0     3166 1970-01-01 00:00:00.000000 langkit-0.0.1b3/PKG-INFO
```

### Comparing `langkit-0.0.1b2/DESCRIPTION.md` & `langkit-0.0.1b3/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b2/LICENSE` & `langkit-0.0.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b2/langkit/__init__.py` & `langkit-0.0.1b3/langkit/__init__.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b2/langkit/examples/GPT_Intro_to_LangKit.ipynb` & `langkit-0.0.1b3/langkit/examples/GPT_Intro_to_LangKit.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b2/langkit/input_output.py` & `langkit-0.0.1b3/langkit/input_output.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b2/langkit/pattern_groups.json` & `langkit-0.0.1b3/langkit/pattern_groups.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b2/langkit/regexes.py` & `langkit-0.0.1b3/langkit/regexes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b2/langkit/tests/conftest.py` & `langkit-0.0.1b3/langkit/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b2/langkit/tests/test_input_output.py` & `langkit-0.0.1b3/langkit/tests/test_input_output.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b2/langkit/tests/test_patterns.py` & `langkit-0.0.1b3/langkit/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b2/langkit/tests/test_themes.py` & `langkit-0.0.1b3/langkit/tests/test_themes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b2/langkit/textstat.py` & `langkit-0.0.1b3/langkit/textstat.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b2/langkit/themes.json` & `langkit-0.0.1b3/langkit/themes.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b2/langkit/themes.py` & `langkit-0.0.1b3/langkit/themes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b2/langkit/toxicity.py` & `langkit-0.0.1b3/langkit/toxicity.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b2/PKG-INFO` & `langkit-0.0.1b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langkit
-Version: 0.0.1b2
+Version: 0.0.1b3
 Summary: A collection of text metric udfs for whylogs profiling and monitoring in WhyLabs
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: langkit@whylabs.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 Requires-Dist: datasets
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: openai
 Requires-Dist: pandas
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: textstat (>=0.7.3,<0.8.0)
 Requires-Dist: torch ; extra == "io"
-Requires-Dist: whylogs (>=1.1.42.dev3,<2.0.0)
+Requires-Dist: whylogs (>=1.1.42.dev3,<=1.1.42.dev4)
 Description-Content-Type: text/markdown
 
 # LangKit
 
 **LangKit** is an open-source text metrics toolkit for monitoring language models. It offers an array of methods for extracting relevant signals from the input and/or output text, which are compatible with the open-source data logging library [whylogs](https://whylogs.readthedocs.io/en/latest).
 
 The generated profiles can be visualized and monitored in the [WhyLabs platform](https://whylabs.ai/) or they can be further analyzed by the user on their own accord.
```

