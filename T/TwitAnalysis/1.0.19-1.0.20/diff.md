# Comparing `tmp/TwitAnalysis-1.0.19.tar.gz` & `tmp/TwitAnalysis-1.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TwitAnalysis-1.0.19.tar", last modified: Thu Dec  8 22:59:46 2022, max compression
+gzip compressed data, was "TwitAnalysis-1.0.20.tar", last modified: Wed May 24 13:35:26 2023, max compression
```

## Comparing `TwitAnalysis-1.0.19.tar` & `TwitAnalysis-1.0.20.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:59:46.353294 TwitAnalysis-1.0.19/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2022-12-08 22:59:34.000000 TwitAnalysis-1.0.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2022-12-08 22:59:46.353294 TwitAnalysis-1.0.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2022-12-08 22:59:34.000000 TwitAnalysis-1.0.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:59:46.353294 TwitAnalysis-1.0.19/TwitAnalysis/
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2022-12-08 22:59:34.000000 TwitAnalysis-1.0.19/TwitAnalysis/TwitAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2022-12-08 22:59:34.000000 TwitAnalysis-1.0.19/TwitAnalysis/TwitLive.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2022-12-08 22:59:34.000000 TwitAnalysis-1.0.19/TwitAnalysis/TwitProcess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2022-12-08 22:59:34.000000 TwitAnalysis-1.0.19/TwitAnalysis/TwitStream.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2022-12-08 22:59:34.000000 TwitAnalysis-1.0.19/TwitAnalysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:59:46.353294 TwitAnalysis-1.0.19/TwitAnalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2022-12-08 22:59:46.000000 TwitAnalysis-1.0.19/TwitAnalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2022-12-08 22:59:46.000000 TwitAnalysis-1.0.19/TwitAnalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 22:59:46.000000 TwitAnalysis-1.0.19/TwitAnalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-08 22:59:46.000000 TwitAnalysis-1.0.19/TwitAnalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-08 22:59:46.000000 TwitAnalysis-1.0.19/TwitAnalysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-08 22:59:46.353294 TwitAnalysis-1.0.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      821 2022-12-08 22:59:34.000000 TwitAnalysis-1.0.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:35:26.241569 TwitAnalysis-1.0.20/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-24 13:35:10.000000 TwitAnalysis-1.0.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-24 13:35:26.241569 TwitAnalysis-1.0.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-24 13:35:10.000000 TwitAnalysis-1.0.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:35:26.241569 TwitAnalysis-1.0.20/TwitAnalysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-05-24 13:35:10.000000 TwitAnalysis-1.0.20/TwitAnalysis/TwitAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-05-24 13:35:10.000000 TwitAnalysis-1.0.20/TwitAnalysis/TwitLive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-24 13:35:10.000000 TwitAnalysis-1.0.20/TwitAnalysis/TwitProcess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-24 13:35:10.000000 TwitAnalysis-1.0.20/TwitAnalysis/TwitStream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-24 13:35:10.000000 TwitAnalysis-1.0.20/TwitAnalysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:35:26.241569 TwitAnalysis-1.0.20/TwitAnalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-24 13:35:26.000000 TwitAnalysis-1.0.20/TwitAnalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-24 13:35:26.000000 TwitAnalysis-1.0.20/TwitAnalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:35:26.000000 TwitAnalysis-1.0.20/TwitAnalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-24 13:35:26.000000 TwitAnalysis-1.0.20/TwitAnalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 13:35:26.000000 TwitAnalysis-1.0.20/TwitAnalysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 13:35:26.241569 TwitAnalysis-1.0.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-24 13:35:10.000000 TwitAnalysis-1.0.20/setup.py
```

### Comparing `TwitAnalysis-1.0.19/LICENSE` & `TwitAnalysis-1.0.20/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,21 @@
-Copyright 2022 Michael Mondoro
+MIT License
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Copyright (c) 2023 Michael Mondoro
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `TwitAnalysis-1.0.19/PKG-INFO` & `TwitAnalysis-1.0.20/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,73 @@
-Metadata-Version: 2.1
-Name: TwitAnalysis
-Version: 1.0.19
-Summary: Package for analyzing Twitter data
-Home-page: https://github.com/michaelMondoro/TwitAnalysis
-Author: Michael Mondoro
-Author-email: michaelmondoro@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Generic badge](https://img.shields.io/badge/Licence-MIT-blue.svg)](https://shields.io/)
 [![Generic badge](https://img.shields.io/badge/Maintained-yes-green.svg)](https://shields.io/)
 [![Generic badge](https://img.shields.io/badge/Python-3.10.6-yellow.svg)](https://shields.io/)
-[![Generic badge](https://img.shields.io/badge/TwitAnalysis-1.0.19-red.svg)](https://test.pypi.org/project/TwitAnalysis/)
+[![Generic badge](https://img.shields.io/badge/TwitAnalysis-1.0.20-red.svg)](https://pypi.org/project/TwitAnalysis/)
 
 ## Purpose
 Every individual user on Twitter has a customized, personal experience and only views a tiny portion of the actual conversations, content and opinions that are put out on the platform. The purpose of this project is to provide tools to allow people to use Twitter data to obtain a more holistic perspective of the social network landscape. The TwitAnalysis modules allow for the live processing of Tweet streams as well as processing mass amounts of posted content related to certain topics, trends or users. This allows for analysis of a much larger sample size of Twitter data, allowing us to estimate the impact/reach of Twitter content. Basically, this means that we can go beyond just seeing what our friends are thinking/saying on the platform, and see the opinions of Twitter at large.
 
 ## Scope
 The scope of the project is limited by a number of different factors which we will attempt to document to allow for transparency. While not necessarily all inclusive, hopefully this can serve as a foundation for Twitter analysis, and a starting point for more targeted projects in the future.
 
 ## Functionality
 Currently the project is split into two main modules. The `TwitLive` module is used for streaming/processing live Twitter data. The `TwitProcess` module is used for processing bulk Twitter data.
 
-
+**TwitLive** Example
 ```python
-from TwitLive import TwitLive
+from TwitAnalysis import *
+from time import sleep
+
+live = TwitLive()
 
-# Make sure to have your keys/tokens defined in your '.config' file. See example file for details
-live = TwitLive(a)
-live.TrendAnalysis("United States", 3, False)
+# Process and display trend analysis
+live.TopTrendAnalysis("United States",2,False, 30)
+live.trends_summary()
+
+# Stream tweets based on search
+stream = live.SearchAnalysis("healthcare",False)
+sleep(10)
+stream.disconnect()
+
+live.search_summary(stream)
 
 ```
 
-![tweets](https://user-images.githubusercontent.com/38412172/197245058-916f99d9-5c0d-437d-80e3-158a8e3af039.png)
+![tweets](https://user-images.githubusercontent.com/38412172/210646662-c83fcbfc-68e6-422e-a47e-a81fa1227d3a.png)
 
+**TwitProcess** Example
+```python
+from TwitAnalysis import *
+
+# Initialize new process object with a specific query
+p = TwitProcess("Python Programming")
+# Search/Process Tweets
+p.bulk_analysis(700)
+
+# Display stats for search results
+print("Stats for query: 'Python Programming'")
+print(f"Sentiment: {p.overall_sentiment()}")
+print(f"Retweets: {p.retweets}")
+print(f"Tweets: {p.reg_tweets}")
+print(f"Impact: {p.impact}")
+
+```
+```
+#==== OUTPUT ====#
+Stats for query: 'Python Programming'
+Sentiment: -0.366
+Retweets: 485
+Tweets: 282
+Impact: 6,228,425
+```
 
-**TODO**:
-  - [x] Calculate *Impact* (How many people are being reached or impacted by this topic/trend)
-  - [x] Stream Tweet trend data
-  - [x] Determine Tweet sentiment
-  - [ ] Calculate *Sentiment* (General sentiment surrounding topic/trend)
-  - [ ] Test/Verify Sentiment model
-  - [ ] Stream based on location
-  - [ ] Process search data
 
 -----
 
-**Documentation**
+**Twitter Documentation**
 
 https://developer.twitter.com/en/docs/tutorials/building-high-quality-filters
 
 **Research**
 
 https://www.sciencedirect.com/science/article/pii/S0268401218306005
 https://epjdatascience.springeropen.com/articles/10.1140/epjds/s13688-018-0178-0
```

### Comparing `TwitAnalysis-1.0.19/TwitAnalysis.egg-info/PKG-INFO` & `TwitAnalysis-1.0.20/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,87 @@
 Metadata-Version: 2.1
 Name: TwitAnalysis
-Version: 1.0.19
+Version: 1.0.20
 Summary: Package for analyzing Twitter data
 Home-page: https://github.com/michaelMondoro/TwitAnalysis
 Author: Michael Mondoro
 Author-email: michaelmondoro@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Generic badge](https://img.shields.io/badge/Licence-MIT-blue.svg)](https://shields.io/)
 [![Generic badge](https://img.shields.io/badge/Maintained-yes-green.svg)](https://shields.io/)
 [![Generic badge](https://img.shields.io/badge/Python-3.10.6-yellow.svg)](https://shields.io/)
-[![Generic badge](https://img.shields.io/badge/TwitAnalysis-1.0.19-red.svg)](https://test.pypi.org/project/TwitAnalysis/)
+[![Generic badge](https://img.shields.io/badge/TwitAnalysis-1.0.20-red.svg)](https://pypi.org/project/TwitAnalysis/)
 
 ## Purpose
 Every individual user on Twitter has a customized, personal experience and only views a tiny portion of the actual conversations, content and opinions that are put out on the platform. The purpose of this project is to provide tools to allow people to use Twitter data to obtain a more holistic perspective of the social network landscape. The TwitAnalysis modules allow for the live processing of Tweet streams as well as processing mass amounts of posted content related to certain topics, trends or users. This allows for analysis of a much larger sample size of Twitter data, allowing us to estimate the impact/reach of Twitter content. Basically, this means that we can go beyond just seeing what our friends are thinking/saying on the platform, and see the opinions of Twitter at large.
 
 ## Scope
 The scope of the project is limited by a number of different factors which we will attempt to document to allow for transparency. While not necessarily all inclusive, hopefully this can serve as a foundation for Twitter analysis, and a starting point for more targeted projects in the future.
 
 ## Functionality
 Currently the project is split into two main modules. The `TwitLive` module is used for streaming/processing live Twitter data. The `TwitProcess` module is used for processing bulk Twitter data.
 
-
+**TwitLive** Example
 ```python
-from TwitLive import TwitLive
+from TwitAnalysis import *
+from time import sleep
+
+live = TwitLive()
+
+# Process and display trend analysis
+live.TopTrendAnalysis("United States",2,False, 30)
+live.trends_summary()
 
-# Make sure to have your keys/tokens defined in your '.config' file. See example file for details
-live = TwitLive(a)
-live.TrendAnalysis("United States", 3, False)
+# Stream tweets based on search
+stream = live.SearchAnalysis("healthcare",False)
+sleep(10)
+stream.disconnect()
+
+live.search_summary(stream)
 
 ```
 
-![tweets](https://user-images.githubusercontent.com/38412172/197245058-916f99d9-5c0d-437d-80e3-158a8e3af039.png)
+![tweets](https://user-images.githubusercontent.com/38412172/210646662-c83fcbfc-68e6-422e-a47e-a81fa1227d3a.png)
+
+**TwitProcess** Example
+```python
+from TwitAnalysis import *
+
+# Initialize new process object with a specific query
+p = TwitProcess("Python Programming")
+# Search/Process Tweets
+p.bulk_analysis(700)
+
+# Display stats for search results
+print("Stats for query: 'Python Programming'")
+print(f"Sentiment: {p.overall_sentiment()}")
+print(f"Retweets: {p.retweets}")
+print(f"Tweets: {p.reg_tweets}")
+print(f"Impact: {p.impact}")
 
+```
+```
+#==== OUTPUT ====#
+Stats for query: 'Python Programming'
+Sentiment: -0.366
+Retweets: 485
+Tweets: 282
+Impact: 6,228,425
+```
 
-**TODO**:
-  - [x] Calculate *Impact* (How many people are being reached or impacted by this topic/trend)
-  - [x] Stream Tweet trend data
-  - [x] Determine Tweet sentiment
-  - [ ] Calculate *Sentiment* (General sentiment surrounding topic/trend)
-  - [ ] Test/Verify Sentiment model
-  - [ ] Stream based on location
-  - [ ] Process search data
 
 -----
 
-**Documentation**
+**Twitter Documentation**
 
 https://developer.twitter.com/en/docs/tutorials/building-high-quality-filters
 
 **Research**
 
 https://www.sciencedirect.com/science/article/pii/S0268401218306005
 https://epjdatascience.springeropen.com/articles/10.1140/epjds/s13688-018-0178-0
```

### Comparing `TwitAnalysis-1.0.19/setup.py` & `TwitAnalysis-1.0.20/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="TwitAnalysis",
-    version="1.0.19",
+    version="1.0.20",
     author="Michael Mondoro",
     author_email="michaelmondoro@gmail.com",
     description="Package for analyzing Twitter data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/michaelMondoro/TwitAnalysis",
     packages=setuptools.find_packages(),
```

