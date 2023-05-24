# Comparing `tmp/finetuner-0.7.6.tar.gz` & `tmp/finetuner-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finetuner-0.7.6.tar", last modified: Tue Apr 18 15:27:57 2023, max compression
+gzip compressed data, was "finetuner-0.7.7.tar", last modified: Wed May 24 07:37:52 2023, max compression
```

## Comparing `finetuner-0.7.6.tar` & `finetuner-0.7.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:27:57.118135 finetuner-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-04-18 15:27:27.000000 finetuner-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 15:27:27.000000 finetuner-0.7.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-04-18 15:27:57.118135 finetuner-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-04-18 15:27:27.000000 finetuner-0.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:27:57.118135 finetuner-0.7.6/finetuner/
--rw-r--r--   0 runner    (1001) docker     (123)    23608 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:27:57.118135 finetuner-0.7.6/finetuner/client/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/client/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/excepts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/finetuner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/hubble.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:27:57.118135 finetuner-0.7.6/finetuner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-04-18 15:27:55.000000 finetuner-0.7.6/finetuner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-18 15:27:57.000000 finetuner-0.7.6/finetuner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:27:55.000000 finetuner-0.7.6/finetuner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:27:55.000000 finetuner-0.7.6/finetuner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-18 15:27:55.000000 finetuner-0.7.6/finetuner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 15:27:55.000000 finetuner-0.7.6/finetuner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-18 15:27:27.000000 finetuner-0.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-18 15:27:57.118135 finetuner-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-18 15:27:27.000000 finetuner-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:37:52.469937 finetuner-0.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-05-24 07:37:44.000000 finetuner-0.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-24 07:37:44.000000 finetuner-0.7.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-05-24 07:37:52.469937 finetuner-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-05-24 07:37:44.000000 finetuner-0.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:37:52.465937 finetuner-0.7.7/finetuner/
+-rw-r--r--   0 runner    (1001) docker     (123)    26507 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:37:52.469937 finetuner-0.7.7/finetuner/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15422 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/excepts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14355 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/finetuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/hubble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:37:52.465937 finetuner-0.7.7/finetuner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-05-24 07:37:52.000000 finetuner-0.7.7/finetuner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-24 07:37:52.000000 finetuner-0.7.7/finetuner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:37:52.000000 finetuner-0.7.7/finetuner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:37:52.000000 finetuner-0.7.7/finetuner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-24 07:37:52.000000 finetuner-0.7.7/finetuner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 07:37:52.000000 finetuner-0.7.7/finetuner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-24 07:37:44.000000 finetuner-0.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-24 07:37:52.469937 finetuner-0.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-24 07:37:44.000000 finetuner-0.7.7/setup.py
```

### Comparing `finetuner-0.7.6/LICENSE` & `finetuner-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.6/PKG-INFO` & `finetuner-0.7.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetuner
-Version: 0.7.6
+Version: 0.7.7
 Summary: Task-oriented finetuning for better embeddings on neural search.
 Home-page: https://github.com/jina-ai/finetuner/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai
@@ -21,15 +21,15 @@
         <b>Task-oriented finetuning for better embeddings on neural search</b>
         </p>
         
         <p align=center>
         <a href="https://pypi.org/project/finetuner/"><img alt="PyPI" src="https://img.shields.io/pypi/v/finetuner?label=Release&style=flat-square"></a>
         <a href="https://codecov.io/gh/jina-ai/finetuner"><img alt="Codecov branch" src="https://img.shields.io/codecov/c/github/jina-ai/finetuner/main?logo=Codecov&logoColor=white&style=flat-square"></a>
         <a href="https://pypistats.org/packages/finetuner"><img alt="PyPI - Downloads from official pypistats" src="https://img.shields.io/pypi/dm/finetuner?style=flat-square"></a>
-        <a href="https://slack.jina.ai"><img src="https://img.shields.io/badge/Slack-3.6k-blueviolet?logo=slack&amp;logoColor=white&style=flat-square"></a>
+        <a href="https://discord.jina.ai"><img src="https://img.shields.io/discord/1106542220112302130?logo=discord&logoColor=white&style=flat-square"></a>
         </p>
         
         <!-- start elevator-pitch -->
         
         Fine-tuning is an effective way to improve performance on [neural search](https://jina.ai/news/what-is-neural-search-and-learn-to-build-a-neural-search-engine/) tasks.
         However, setting up and performing fine-tuning can be very time-consuming and resource-intensive.
         
@@ -157,15 +157,15 @@
         
         Make sure you have Python 3.8+ installed. Finetuner can be installed via `pip` by executing:
         
         ```bash
         pip install -U finetuner
         ```
         
-        If you want to encode `docarray.DocumentArray` objects with the `finetuner.encode` function, you need to install 
+        If you want to encode local data with the `finetuner.encode` function, you need to install 
         `"finetuner[full]"`. This includes a number of additional dependencies, which are necessary for encoding: Torch, 
         Torchvision and OpenCLIP:
         
         ```bash
         pip install "finetuner[full]"
         ```
         
@@ -187,15 +187,15 @@
         <!-- end finetuner-articles -->
         
         <!-- start support-pitch -->
         ## Support
         
         - Use [Discussions](https://github.com/jina-ai/finetuner/discussions) to talk about your use cases, questions, and
           support queries.
-        - Join our [Slack community](https://slack.jina.ai) and chat with other Jina AI community members about ideas.
+        - Join our [Discord community](https://discord.jina.ai) and chat with other community members about ideas.
         - Join our [Engineering All Hands](https://youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to discuss your use case and learn Jina AI new features.
             - **When?** The second Tuesday of every month
             - **Where?**
               Zoom ([see our public events calendar](https://calendar.google.com/calendar/embed?src=c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com&ctz=Europe%2FBerlin)/[.ical](https://calendar.google.com/calendar/ical/c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com/public/basic.ics))
               and [live stream on YouTube](https://youtube.com/c/jina-ai)
         - Subscribe to the latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: finetuner Version: 0.7.6 Summary: Task-oriented
+Metadata-Version: 2.1 Name: finetuner Version: 0.7.7 Summary: Task-oriented
 finetuning for better embeddings on neural search. Home-page: https://
 github.com/jina-ai/finetuner/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai Project-URL: Source,
 https://github.com/jina-ai/finetuner/ Project-URL: Tracker, https://github.com/
 jina-ai/finetuner/issues Description:
 
 [Finetuner logo: Finetuner helps you to create experiments in order to improve
   embeddings on search tasks. It accompanies you to deliver the last mile of
               performance-tuning for neural search applications.]
         Task-oriented finetuning for better embeddings on neural search
  [PyPI] [Codecov_branch] [PyPI_-_Downloads_from_official_pypistats] [https://
-                       img.shields.io/badge/Slack-3.6k-
-         blueviolet?logo=slack&amp;logoColor=white&style=flat-square]
+                            img.shields.io/discord/
+      1106542220112302130?logo=discord&logoColor=white&style=flat-square]
  Fine-tuning is an effective way to improve performance on [neural search]
 (https://jina.ai/news/what-is-neural-search-and-learn-to-build-a-neural-search-
 engine/) tasks. However, setting up and performing fine-tuning can be very
 time-consuming and resource-intensive. Jina AI's Finetuner makes fine-tuning
 easier and faster by streamlining the workflow and handling all the complexity
 and infrastructure in the cloud. With Finetuner, you can easily enhance the
 performance of pre-trained models, making them production-ready [without
@@ -51,40 +51,39 @@
            (German)
 PointNet++ ModelNet40 3D   mRR    0.791      0.891     12.7%  [Open_In_Colab]
            Mesh Search     Recall 0.154      0.242     57.1%
 All metrics were evaluated for k@20 after training for 5 epochs using the Adam
 optimizer with learning rates of 1e-4 for ResNet, 1e-7 for CLIP and 1e-5 for
 the BERT models, 5e-4 for PointNet++  ## Install Make sure you have Python 3.8+
 installed. Finetuner can be installed via `pip` by executing: ```bash pip
-install -U finetuner ``` If you want to encode `docarray.DocumentArray` objects
-with the `finetuner.encode` function, you need to install `"finetuner[full]"`.
-This includes a number of additional dependencies, which are necessary for
-encoding: Torch, Torchvision and OpenCLIP: ```bash pip install "finetuner
-[full]" ```  > â ï¸ Starting with version 0.5.0, Finetuner computing is
-performed on Jina AI Cloud. The last local version is `0.4.1`. > This version
-is still available for installation via `pip`. See [Finetuner git tags and
-releases](https://github.com/jina-ai/finetuner/releases).  ## Articles about
-Finetuner Check out our published blogposts and tutorials to see Finetuner in
-action! - [Fine-tuning with Low Budget and High Expectations](https://jina.ai/
-news/fine-tuning-with-low-budget-and-high-expectations/) - [Hype and Hybrids:
-Search is more than Keywords and Vectors](https://jina.ai/news/hype-and-
-hybrids-multimodal-search-means-more-than-keywords-and-vectors-2/) - [Improving
-Search Quality for Non-English Queries with Fine-tuned Multilingual CLIP
-Models](https://jina.ai/news/improving-search-quality-non-english-queries-fine-
-tuned-multilingual-clip-models/) - [How Much Do We Get by Finetuning CLIP?]
-(https://jina.ai/news/applying-jina-ai-finetuner-to-clip-less-data-smaller-
-models-higher-performance/)   ## Support - Use [Discussions](https://
-github.com/jina-ai/finetuner/discussions) to talk about your use cases,
-questions, and support queries. - Join our [Slack community](https://
-slack.jina.ai) and chat with other Jina AI community members about ideas. -
-Join our [Engineering All Hands](https://youtube.com/
-playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to discuss your use
-case and learn Jina AI new features. - **When?** The second Tuesday of every
-month - **Where?** Zoom ([see our public events calendar](https://
-calendar.google.com/calendar/
+install -U finetuner ``` If you want to encode local data with the
+`finetuner.encode` function, you need to install `"finetuner[full]"`. This
+includes a number of additional dependencies, which are necessary for encoding:
+Torch, Torchvision and OpenCLIP: ```bash pip install "finetuner[full]" ```  >
+â ï¸ Starting with version 0.5.0, Finetuner computing is performed on Jina AI
+Cloud. The last local version is `0.4.1`. > This version is still available for
+installation via `pip`. See [Finetuner git tags and releases](https://
+github.com/jina-ai/finetuner/releases).  ## Articles about Finetuner Check out
+our published blogposts and tutorials to see Finetuner in action! - [Fine-
+tuning with Low Budget and High Expectations](https://jina.ai/news/fine-tuning-
+with-low-budget-and-high-expectations/) - [Hype and Hybrids: Search is more
+than Keywords and Vectors](https://jina.ai/news/hype-and-hybrids-multimodal-
+search-means-more-than-keywords-and-vectors-2/) - [Improving Search Quality for
+Non-English Queries with Fine-tuned Multilingual CLIP Models](https://jina.ai/
+news/improving-search-quality-non-english-queries-fine-tuned-multilingual-clip-
+models/) - [How Much Do We Get by Finetuning CLIP?](https://jina.ai/news/
+applying-jina-ai-finetuner-to-clip-less-data-smaller-models-higher-performance/
+)   ## Support - Use [Discussions](https://github.com/jina-ai/finetuner/
+discussions) to talk about your use cases, questions, and support queries. -
+Join our [Discord community](https://discord.jina.ai) and chat with other
+community members about ideas. - Join our [Engineering All Hands](https://
+youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to
+discuss your use case and learn Jina AI new features. - **When?** The second
+Tuesday of every month - **Where?** Zoom ([see our public events calendar]
+(https://calendar.google.com/calendar/
 embed?src=c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com&ctz=Europe%2FBerlin)/
 [.ical](https://calendar.google.com/calendar/ical/
 c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com/public/basic.ics)) and
 [live stream on YouTube](https://youtube.com/c/jina-ai) - Subscribe to the
 latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
 ## Join Us Finetuner is backed by [Jina AI](https://jina.ai) and licensed under
 [Apache-2.0](./LICENSE). [We are actively hiring](https://jobs.jina.ai) AI
```

### Comparing `finetuner-0.7.6/README.md` & `finetuner-0.7.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 <b>Task-oriented finetuning for better embeddings on neural search</b>
 </p>
 
 <p align=center>
 <a href="https://pypi.org/project/finetuner/"><img alt="PyPI" src="https://img.shields.io/pypi/v/finetuner?label=Release&style=flat-square"></a>
 <a href="https://codecov.io/gh/jina-ai/finetuner"><img alt="Codecov branch" src="https://img.shields.io/codecov/c/github/jina-ai/finetuner/main?logo=Codecov&logoColor=white&style=flat-square"></a>
 <a href="https://pypistats.org/packages/finetuner"><img alt="PyPI - Downloads from official pypistats" src="https://img.shields.io/pypi/dm/finetuner?style=flat-square"></a>
-<a href="https://slack.jina.ai"><img src="https://img.shields.io/badge/Slack-3.6k-blueviolet?logo=slack&amp;logoColor=white&style=flat-square"></a>
+<a href="https://discord.jina.ai"><img src="https://img.shields.io/discord/1106542220112302130?logo=discord&logoColor=white&style=flat-square"></a>
 </p>
 
 <!-- start elevator-pitch -->
 
 Fine-tuning is an effective way to improve performance on [neural search](https://jina.ai/news/what-is-neural-search-and-learn-to-build-a-neural-search-engine/) tasks.
 However, setting up and performing fine-tuning can be very time-consuming and resource-intensive.
 
@@ -145,15 +145,15 @@
 
 Make sure you have Python 3.8+ installed. Finetuner can be installed via `pip` by executing:
 
 ```bash
 pip install -U finetuner
 ```
 
-If you want to encode `docarray.DocumentArray` objects with the `finetuner.encode` function, you need to install 
+If you want to encode local data with the `finetuner.encode` function, you need to install 
 `"finetuner[full]"`. This includes a number of additional dependencies, which are necessary for encoding: Torch, 
 Torchvision and OpenCLIP:
 
 ```bash
 pip install "finetuner[full]"
 ```
 
@@ -175,15 +175,15 @@
 <!-- end finetuner-articles -->
 
 <!-- start support-pitch -->
 ## Support
 
 - Use [Discussions](https://github.com/jina-ai/finetuner/discussions) to talk about your use cases, questions, and
   support queries.
-- Join our [Slack community](https://slack.jina.ai) and chat with other Jina AI community members about ideas.
+- Join our [Discord community](https://discord.jina.ai) and chat with other community members about ideas.
 - Join our [Engineering All Hands](https://youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to discuss your use case and learn Jina AI new features.
     - **When?** The second Tuesday of every month
     - **Where?**
       Zoom ([see our public events calendar](https://calendar.google.com/calendar/embed?src=c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com&ctz=Europe%2FBerlin)/[.ical](https://calendar.google.com/calendar/ical/c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com/public/basic.ics))
       and [live stream on YouTube](https://youtube.com/c/jina-ai)
 - Subscribe to the latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 
 
 [Finetuner logo: Finetuner helps you to create experiments in order to improve
   embeddings on search tasks. It accompanies you to deliver the last mile of
               performance-tuning for neural search applications.]
         Task-oriented finetuning for better embeddings on neural search
  [PyPI] [Codecov_branch] [PyPI_-_Downloads_from_official_pypistats] [https://
-                       img.shields.io/badge/Slack-3.6k-
-         blueviolet?logo=slack&amp;logoColor=white&style=flat-square]
+                            img.shields.io/discord/
+      1106542220112302130?logo=discord&logoColor=white&style=flat-square]
  Fine-tuning is an effective way to improve performance on [neural search]
 (https://jina.ai/news/what-is-neural-search-and-learn-to-build-a-neural-search-
 engine/) tasks. However, setting up and performing fine-tuning can be very
 time-consuming and resource-intensive. Jina AI's Finetuner makes fine-tuning
 easier and faster by streamlining the workflow and handling all the complexity
 and infrastructure in the cloud. With Finetuner, you can easily enhance the
 performance of pre-trained models, making them production-ready [without
@@ -45,40 +45,39 @@
            (German)
 PointNet++ ModelNet40 3D   mRR    0.791      0.891     12.7%  [Open_In_Colab]
            Mesh Search     Recall 0.154      0.242     57.1%
 All metrics were evaluated for k@20 after training for 5 epochs using the Adam
 optimizer with learning rates of 1e-4 for ResNet, 1e-7 for CLIP and 1e-5 for
 the BERT models, 5e-4 for PointNet++  ## Install Make sure you have Python 3.8+
 installed. Finetuner can be installed via `pip` by executing: ```bash pip
-install -U finetuner ``` If you want to encode `docarray.DocumentArray` objects
-with the `finetuner.encode` function, you need to install `"finetuner[full]"`.
-This includes a number of additional dependencies, which are necessary for
-encoding: Torch, Torchvision and OpenCLIP: ```bash pip install "finetuner
-[full]" ```  > â ï¸ Starting with version 0.5.0, Finetuner computing is
-performed on Jina AI Cloud. The last local version is `0.4.1`. > This version
-is still available for installation via `pip`. See [Finetuner git tags and
-releases](https://github.com/jina-ai/finetuner/releases).  ## Articles about
-Finetuner Check out our published blogposts and tutorials to see Finetuner in
-action! - [Fine-tuning with Low Budget and High Expectations](https://jina.ai/
-news/fine-tuning-with-low-budget-and-high-expectations/) - [Hype and Hybrids:
-Search is more than Keywords and Vectors](https://jina.ai/news/hype-and-
-hybrids-multimodal-search-means-more-than-keywords-and-vectors-2/) - [Improving
-Search Quality for Non-English Queries with Fine-tuned Multilingual CLIP
-Models](https://jina.ai/news/improving-search-quality-non-english-queries-fine-
-tuned-multilingual-clip-models/) - [How Much Do We Get by Finetuning CLIP?]
-(https://jina.ai/news/applying-jina-ai-finetuner-to-clip-less-data-smaller-
-models-higher-performance/)   ## Support - Use [Discussions](https://
-github.com/jina-ai/finetuner/discussions) to talk about your use cases,
-questions, and support queries. - Join our [Slack community](https://
-slack.jina.ai) and chat with other Jina AI community members about ideas. -
-Join our [Engineering All Hands](https://youtube.com/
-playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to discuss your use
-case and learn Jina AI new features. - **When?** The second Tuesday of every
-month - **Where?** Zoom ([see our public events calendar](https://
-calendar.google.com/calendar/
+install -U finetuner ``` If you want to encode local data with the
+`finetuner.encode` function, you need to install `"finetuner[full]"`. This
+includes a number of additional dependencies, which are necessary for encoding:
+Torch, Torchvision and OpenCLIP: ```bash pip install "finetuner[full]" ```  >
+â ï¸ Starting with version 0.5.0, Finetuner computing is performed on Jina AI
+Cloud. The last local version is `0.4.1`. > This version is still available for
+installation via `pip`. See [Finetuner git tags and releases](https://
+github.com/jina-ai/finetuner/releases).  ## Articles about Finetuner Check out
+our published blogposts and tutorials to see Finetuner in action! - [Fine-
+tuning with Low Budget and High Expectations](https://jina.ai/news/fine-tuning-
+with-low-budget-and-high-expectations/) - [Hype and Hybrids: Search is more
+than Keywords and Vectors](https://jina.ai/news/hype-and-hybrids-multimodal-
+search-means-more-than-keywords-and-vectors-2/) - [Improving Search Quality for
+Non-English Queries with Fine-tuned Multilingual CLIP Models](https://jina.ai/
+news/improving-search-quality-non-english-queries-fine-tuned-multilingual-clip-
+models/) - [How Much Do We Get by Finetuning CLIP?](https://jina.ai/news/
+applying-jina-ai-finetuner-to-clip-less-data-smaller-models-higher-performance/
+)   ## Support - Use [Discussions](https://github.com/jina-ai/finetuner/
+discussions) to talk about your use cases, questions, and support queries. -
+Join our [Discord community](https://discord.jina.ai) and chat with other
+community members about ideas. - Join our [Engineering All Hands](https://
+youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to
+discuss your use case and learn Jina AI new features. - **When?** The second
+Tuesday of every month - **Where?** Zoom ([see our public events calendar]
+(https://calendar.google.com/calendar/
 embed?src=c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com&ctz=Europe%2FBerlin)/
 [.ical](https://calendar.google.com/calendar/ical/
 c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com/public/basic.ics)) and
 [live stream on YouTube](https://youtube.com/c/jina-ai) - Subscribe to the
 latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
 ## Join Us Finetuner is backed by [Jina AI](https://jina.ai) and licensed under
 [Apache-2.0](./LICENSE). [We are actively hiring](https://jobs.jina.ai) AI
```

### Comparing `finetuner-0.7.6/finetuner/__init__.py` & `finetuner-0.7.7/finetuner/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import inspect
 import os
 import warnings
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, TextIO, Union
 
 from _finetuner.runner.stubs import model as model_stub
-from docarray import DocumentArray
+from docarray import Document, DocumentArray  # noqa F401
 
 from finetuner.constants import (
     DEFAULT_FINETUNER_HOST,
     DEFAULT_HUBBLE_REGISTRY,
     HOST,
     HUBBLE_REGISTRY,
 )
 from finetuner.data import CSVOptions
+from finetuner.model import SynthesisModels
 from finetuner.run import Run
 from hubble import login_required
 
 if HOST not in os.environ:
     os.environ[HOST] = DEFAULT_FINETUNER_HOST
 
 if HUBBLE_REGISTRY not in os.environ:
@@ -63,35 +64,35 @@
         if name != 'MLPStub' and not name.startswith('_') and type(stub) != type:
             rv[stub.name] = stub
     return rv
 
 
 def list_models() -> List[str]:
     """List available models."""
-    return [name for name in list_model_classes()]
+    return [_model_class.display_name for _model_class in list_model_classes().values()]
 
 
 def list_model_options() -> Dict[str, List[Dict[str, Any]]]:
     """List available options per model."""
     return {
-        name: [
+        _model_class.display_name: [
             {
                 'name': parameter.name,
                 'type': parameter.annotation,
                 'required': parameter.default == parameter.empty,
                 'default': (
                     parameter.default if parameter.default != parameter.empty else None
                 ),
             }
             for parameter in inspect.signature(
                 _model_class.__init__
             ).parameters.values()
             if parameter.name != 'self'
         ]
-        for name, _model_class in list_model_classes().items()
+        for _model_class in list_model_classes().values()
     }
 
 
 def describe_models(task: Optional[str] = None) -> None:
     """Print model information, such as name, task, output dimension, architecture
     and description as a table.
 
@@ -133,16 +134,16 @@
     csv_options: Optional[CSVOptions] = None,
     public: bool = False,
     num_items_per_class: int = 4,
     sampler: str = 'auto',
     loss_optimizer: Optional[str] = None,
     loss_optimizer_options: Optional[Dict[str, Any]] = None,
 ) -> Run:
-    """Create a Finetuner :class:`Run`, calling this function will submit a fine-tuning
-    job to the Jina AI Cloud.
+    """Create a Finetuner training :class:`Run`, calling this function will submit a
+    fine-tuning job to the Jina AI Cloud.
 
     :param model: The name of model to be fine-tuned. Run `finetuner.list_models()` or
         `finetuner.describe_models()` to see the available model names.
     :param train_data: Either a `DocumentArray` for training data, a name of the
         `DocumentArray` that is pushed on Jina AI Cloud or a path to a CSV file.
     :param eval_data: Either a `DocumentArray` for evaluation data, a name of the
         `DocumentArray` that is pushed on Jina AI Cloud or a path to a CSV file.
@@ -236,15 +237,15 @@
         <https://pytorch.org/docs/stable/optim.html>`_.
 
     .. note::
        Unless necessary, please stick with `device="cuda"`, `cpu` training could be
        extremely slow and inefficient.
     """
 
-    return ft.create_run(
+    return ft.create_training_run(
         model=model,
         train_data=train_data,
         eval_data=eval_data,
         val_split=val_split,
         model_artifact=model_artifact,
         run_name=run_name,
         description=description,
@@ -271,17 +272,81 @@
         num_items_per_class=num_items_per_class,
         sampler=sampler,
         loss_optimizer=loss_optimizer,
         loss_optimizer_options=loss_optimizer_options,
     )
 
 
-# `create_run` and `fit` do the same
+@login_required
+def synthesize(
+    query_data: Union[str, List[str], DocumentArray],
+    corpus_data: Union[str, List[str], DocumentArray],
+    models: SynthesisModels,
+    num_relations: int = 3,
+    run_name: Optional[str] = None,
+    description: Optional[str] = None,
+    experiment_name: Optional[str] = None,
+    device: str = 'cuda',
+    num_workers: int = 4,
+    csv_options: Optional[CSVOptions] = None,
+    public: bool = False,
+) -> Run:
+    """Create a Finetuner synthesis :class:`Run`, calling this function will submit a
+    data synthesis job to the Jina AI Cloud.
+
+    :param query_data: Either a :class:`DocumentArray` for example queries, name of a
+        `DocumentArray` that is pushed on Jina AI Cloud, the dataset itself as
+        a list of strings or a path to a CSV file.
+    :param corpus_data: Either a :class:`DocumentArray` for corpus data, a name of a
+        `DocumentArray` that is pushed on Jina AI Cloud, the dataset itself as a
+        list of strings or a path to a CSV file.
+    :param models: A :class:`SynthesisModels` object containing the names of
+        the models used for relation mining and cross encoding.
+        You can pass `finetuner.data.DATA_SYNTHESIS_EN` for the recommended models for
+        synthesis based on english data.
+    :param num_relations: The number of relations to mine per query.
+    :param run_name: Name of the run.
+    :param: description: Run Description.
+    :param experiment_name: Name of the experiment.
+    :param device: Whether to use the CPU, if set to `cuda`, a Nvidia GPU will be used.
+        otherwise use `cpu` to run a cpu job.
+    :param num_workers: Number of CPU workers. If `cpu: False` this is the number of
+        workers used by the dataloader.
+    :param csv_options: A :class:`CSVOptions` object containing options used for
+        reading in training and evaluation data from a CSV file, if they are
+        provided as such.
+    :param public: A boolean value indicates if the artifact is public. It should be
+        set to `True` if you would like to share your synthesized data with others.
+
+    .. note::
+       Unless necessary, please stick with `device="cuda"`, `cpu` training could be
+       extremely slow and inefficient.
+    """
+    return ft.create_synthesis_run(
+        query_data=query_data,
+        corpus_data=corpus_data,
+        models=models,
+        num_relations=num_relations,
+        run_name=run_name,
+        description=description,
+        experiment_name=experiment_name,
+        device=device,
+        num_workers=num_workers,
+        csv_options=csv_options,
+        public=public,
+    )
+
+
+# `create_run`, `create_training_run` and `fit` do the same
+create_training_run = fit
 create_run = fit
 
+# `create_synthesis_run` and `synthesize` do the same
+create_synthesis_run = synthesize
+
 
 def get_run(run_name: str, experiment_name: Optional[str] = None) -> Run:
     """Get a :class:`Run` by its name and (optional) :class:`Experiment` name.
 
     If an experiment name is not specified, we'll look for the run in the default
     experiment.
```

### Comparing `finetuner-0.7.6/finetuner/client/base.py` & `finetuner-0.7.7/finetuner/client/base.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.6/finetuner/client/client.py` & `finetuner-0.7.7/finetuner/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     LOGS,
     LOGSTREAM,
     METRICS,
     NAME,
     POST,
     RUNS,
     STATUS,
+    TASK,
 )
 
 _finetuner_core_version = pkg_resources.get_distribution('finetuner-stubs').version
 
 
 class FinetunerV1Client(_BaseClient):
     """
@@ -263,14 +264,15 @@
         return self._handle_request(url=url, method=GET)
 
     def create_run(
         self,
         experiment_name: str,
         run_name: str,
         run_config: dict,
+        task: str,
         device: str,
         cpus: int,
         gpus: int,
     ) -> dict:
         """Create a run inside a given experiment.
 
         For optional parameters please visit our documentation (link).
@@ -287,13 +289,14 @@
         )
         return self._handle_request(
             url=url,
             method=POST,
             json_data={
                 NAME: run_name,
                 CONFIG: run_config,
+                TASK: task,
                 FINETUNER_VERSION: _finetuner_core_version,
                 DEVICE: device,
                 CPUS: cpus,
                 GPUS: gpus,
             },
         )
```

### Comparing `finetuner-0.7.6/finetuner/client/session.py` & `finetuner-0.7.7/finetuner/client/session.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.6/finetuner/console.py` & `finetuner-0.7.7/finetuner/console.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.6/finetuner/constants.py` & `finetuner-0.7.7/finetuner/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -77,7 +77,20 @@
 QUERY_DATA = 'query_data'
 INDEX_DATA = 'index_data'
 DA_PREFIX = 'finetuner-dastorage'
 ONNX = 'to_onnx'
 PUBLIC = 'public'
 NUM_ITEMS_PER_CLASS = 'num_items_per_class'
 VAL_SPLIT = 'val_split'
+TASK = 'task'
+TRAINING_TASK = 'training'
+SYNTHESIS_TASK = 'generation'
+# Synthesis job
+RAW_DATA_CONFIG = 'data'
+RELATION_MINING = 'relation_mining'
+CROSS_ENCODER = 'cross_encoder'
+QUERIES = 'queries'
+CORPUS = 'corpus'
+MODELS = 'models'
+NUM_RELATIONS = 'num_relations'
+TRAIN_DATA = 'train_data'
+MAX_NUM_DOCS = 'max_num_docs'
```

### Comparing `finetuner-0.7.6/finetuner/data.py` & `finetuner-0.7.7/finetuner/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from abc import ABC
 from contextlib import nullcontext
 from dataclasses import dataclass
 from io import StringIO
 from typing import TYPE_CHECKING, List, Optional, TextIO, Tuple, Union
 
 from _finetuner.runner.stubs.model import get_stub
-from docarray import Document, DocumentArray
 from docarray.document.generators import _subsample
 from docarray.document.mixins.helper import _is_uri
 from genericpath import isfile
 
+from finetuner import Document, DocumentArray
 from finetuner.constants import DEFAULT_TAG_KEY, DEFAULT_TAG_SCORE_KEY
 
 if TYPE_CHECKING:
     from _finetuner.models.inference import InferenceEngine
 
 
 @dataclass
@@ -218,41 +218,72 @@
                     self._options.convert_to_blob,
                     self._options.create_point_clouds,
                     point_cloud_size=self._options.point_cloud_size,
                 )
                 yield Document(chunks=[doc1, doc2], tags={DEFAULT_TAG_SCORE_KEY: col3})
 
 
+class DataSynthesisParser(_CSVParser):
+    """
+    CSV has either one column or one row, each item in the CSV represents a single
+    document so the structure of the CSV file is not important.
+    """
+
+    def __init__(
+        self,
+        file: Union[str, TextIO, StringIO],
+        task: str,
+        options: Optional[CSVOptions] = None,
+    ):
+        super().__init__(file, task, options)
+
+    def parse(self):
+        with self._file_ctx as fp:
+            lines = csv.reader(fp, dialect=self._options.dialect)
+
+            for columns in _subsample(
+                lines, self._options.size, self._options.sampling_rate
+            ):
+                for column in columns:
+                    yield Document(text=column)
+
+
 class CSVContext:
     """
     A CSV context switch class with conditions to parse CSVs into DocumentArray.
 
     :param model: The model being used, to get model stub and associated task.
-    :param options: an instance of :class`CSVOptions`.
+    :param options: An instance of :class`CSVOptions`.
     """
 
     def __init__(
         self,
-        model: str,
+        model: Optional[str] = None,
         options: Optional[CSVOptions] = None,
     ):
         self._model = model
         self._options = options or CSVOptions()
-        if model == 'mlp':
+        if not model:
+            self._task = 'synthesis'
+        elif model == 'mlp':
             self._task = 'image-to-image'
         else:
             model_stub = get_stub(
                 model,
                 select_model='clip-text',
             )
             # for clip select_model is mandatory, though any model will get us the task
             self._task = model_stub.task
 
     def _get_csv_parser(self, data: Union[str, TextIO]):
-        if self._options.is_labeled:
+        if self._task == 'synthesis':
+            return DataSynthesisParser(
+                file=data, task=self._task, options=self._options
+            )
+        elif self._options.is_labeled:
             return LabeledCSVParser(file=data, task=self._task, options=self._options)
         else:
             _, num_columns = get_csv_file_dialect_columns(
                 file=data, encoding=self._options.encoding
             )
             if num_columns == 2:
                 return QueryDocumentRelationsParser(
```

### Comparing `finetuner-0.7.6/finetuner/experiment.py` & `finetuner-0.7.7/finetuner/experiment.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import json
 from dataclasses import fields
 from typing import Any, Dict, List, Optional, TextIO, Union
 
 from _finetuner.runner.stubs import config
-from docarray import DocumentArray
 
+from finetuner import Document, DocumentArray
 from finetuner.callback import EvaluationCallback
 from finetuner.client import FinetunerV1Client
 from finetuner.constants import (
     BATCH_SIZE,
     CALLBACKS,
     CONFIG,
     CREATED_AT,
@@ -31,18 +32,23 @@
     OPTIMIZER,
     OPTIMIZER_OPTIONS,
     OUTPUT_DIM,
     PUBLIC,
     SAMPLER,
     SCHEDULER,
     SCHEDULER_OPTIONS,
+    SYNTHESIS_TASK,
+    TASK,
+    TRAIN_DATA,
+    TRAINING_TASK,
     VAL_SPLIT,
 )
-from finetuner.data import CSVContext
-from finetuner.hubble import push_data
+from finetuner.data import CSVContext, CSVOptions
+from finetuner.hubble import push_synthesis_data, push_training_data
+from finetuner.model import SynthesisModels
 from finetuner.names import get_random_name
 from finetuner.run import Run
 
 
 class Experiment:
     """Class for an experiment.
 
@@ -82,19 +88,23 @@
 
         :param name: Name of the run.
         :return: A `Run` object.
         """
         run = self._client.get_run(experiment_name=self._name, run_name=name)
         run = Run(
             name=run[NAME],
-            config=run[CONFIG],
+            config=json.loads(run[CONFIG])
+            if isinstance(run[CONFIG], str)
+            else run[CONFIG],
             created_at=run[CREATED_AT],
             description=run[DESCRIPTION],
             experiment_name=self._name,
             client=self._client,
+            task=run.get(TASK, TRAINING_TASK),
+            train_data=run.get(TRAIN_DATA, None),
         )
         return run
 
     def list_runs(self, page: int = 50, size: int = 50) -> List[Run]:
         """List all :class:`Run`.
 
         :param page: The page index.
@@ -112,14 +122,16 @@
             Run(
                 name=run[NAME],
                 config=run[CONFIG],
                 created_at=run[CREATED_AT],
                 description=run[DESCRIPTION],
                 experiment_name=self._name,
                 client=self._client,
+                task=run.get(TASK, TRAINING_TASK),
+                train_data=run.get(TRAIN_DATA, None),
             )
             for run in runs
         ]
 
     def delete_run(self, name: str):
         """Delete a :class:`Run` by its name.
 
@@ -127,24 +139,26 @@
         """
         self._client.delete_run(experiment_name=self._name, run_name=name)
 
     def delete_runs(self):
         """Delete all :class:`Run` inside the :class:`Experiment`."""
         self._client.delete_runs(experiment_name=self._name)
 
-    def create_run(
+    def create_training_run(
         self,
         model: str,
         train_data: Union[str, TextIO, DocumentArray],
         run_name: Optional[str] = None,
         eval_data: Optional[Union[str, TextIO, DocumentArray]] = None,
-        csv_options: Optional[Dict[str, Any]] = None,
+        csv_options: Optional[CSVOptions] = None,
         **kwargs,
     ) -> Run:
-        """Create a :class:`Run` inside the :class:`Experiment`."""
+        """Create a :class:`Run` inside the :class:`Experiment` with the
+        task of 'training'.
+        """
         if not run_name:
             run_name = get_random_name()
 
         eval_callback = None
         callbacks = kwargs[CALLBACKS] if kwargs.get(CALLBACKS) else []
         for callback in callbacks:
             if isinstance(callback, EvaluationCallback):
@@ -159,15 +173,15 @@
             eval_callback.query_data = csv_context.build_dataset(
                 data=eval_callback.query_data,
             )
             eval_callback.index_data = csv_context.build_dataset(
                 eval_callback.index_data
             )
 
-        train_data, eval_data, query_data, index_data = push_data(
+        train_data, eval_data, query_data, index_data = push_training_data(
             experiment_name=self._name,
             run_name=run_name,
             train_data=train_data,
             eval_data=eval_data,
             query_data=eval_callback.query_data if eval_callback else None,
             index_data=eval_callback.index_data if eval_callback else None,
         )
@@ -190,37 +204,108 @@
             device = 'gpu'
 
         num_workers = kwargs.get(NUM_WORKERS, 4)
         run = self._client.create_run(
             run_name=run_name,
             experiment_name=self._name,
             run_config=config,
+            task=TRAINING_TASK,
             device=device,
             cpus=num_workers,
             gpus=1,
         )
         run = Run(
             client=self._client,
             name=run[NAME],
             experiment_name=self._name,
             config=run[CONFIG],
             created_at=run[CREATED_AT],
             description=run[DESCRIPTION],
+            task=TRAINING_TASK,
+        )
+        return run
+
+    def create_synthesis_run(
+        self,
+        query_data: Union[str, List[str], DocumentArray],
+        corpus_data: Union[str, List[str], DocumentArray],
+        models: SynthesisModels,
+        num_relations: int = 3,
+        run_name: Optional[str] = None,
+        csv_options: Optional[CSVOptions] = None,
+        **kwargs,
+    ) -> Run:
+        """Create a :class:`Run` inside the :class:`Experiment` with the
+        task of 'generation' (data synthesis).
+        """
+        if not run_name:
+            run_name = get_random_name()
+
+        csv_context = CSVContext(None, options=csv_options)
+        query_data = (
+            csv_context.build_dataset(data=query_data)
+            if isinstance(query_data, str)
+            else DocumentArray([Document(text=data) for data in query_data])
+        )
+        corpus_data = (
+            csv_context.build_dataset(data=corpus_data)
+            if isinstance(query_data, str)
+            else DocumentArray([Document(text=data) for data in corpus_data])
+        )
+        query_data, corpus_data = push_synthesis_data(
+            experiment_name=self._name,
+            run_name=run_name,
+            query_data=query_data,
+            corpus_data=corpus_data,
+        )
+
+        config = self._create_synthesis_config(
+            query_data=query_data,
+            corpus_data=corpus_data,
+            models=models,
+            num_relations=num_relations,
+            experiment_name=self._name,
+            run_name=run_name,
+            **kwargs,
+        )
+
+        device = kwargs.get(DEVICE, 'cuda')
+        if device == 'cuda':
+            device = 'gpu'
+
+        num_workers = kwargs.get(NUM_WORKERS, 4)
+        run = self._client.create_run(
+            run_name=run_name,
+            experiment_name=self._name,
+            run_config=config,
+            task=SYNTHESIS_TASK,
+            device=device,
+            cpus=num_workers,
+            gpus=1,
+        )
+        run = Run(
+            client=self._client,
+            name=run[NAME],
+            experiment_name=self._name,
+            config=run[CONFIG],
+            created_at=run[CREATED_AT],
+            description=run[DESCRIPTION],
+            task=SYNTHESIS_TASK,
         )
         return run
 
     @staticmethod
     def _create_finetuning_config(
         model: str,
         train_data: str,
         experiment_name: str,
         run_name: str,
         **kwargs,
     ) -> Dict[str, Any]:
-        """Create config for a :class:`Run`.
+        """Create finetuning config for a :class:`Run`.
 
         :param model: Name of the model to be fine-tuned.
         :param train_data: Either a `DocumentArray` for training data or a
             name of the `DocumentArray` that is pushed on Hubble.
         :param experiment_name: Name of the experiment.
         :param run_name: Name of the run.
         :param kwargs: Optional keyword arguments for the run config.
@@ -294,7 +379,51 @@
             hyper_parameters=hyper_parameters,
             public=public,
             experiment_name=experiment_name,
             run_name=run_name,
         )
 
         return finetuning_config.dict()
+
+    @staticmethod
+    def _create_synthesis_config(
+        query_data: str,
+        corpus_data: str,
+        models: SynthesisModels,
+        num_relations: int,
+        experiment_name: str,
+        run_name: str,
+        **kwargs,
+    ) -> Dict[str, Any]:
+        """Create a synthesis config for a :class:`Run`.
+
+        :param query_data: Name of the :class:`DocumentArray` containing the query data
+            used during training.
+        :param corpus_data: Name of the :class:`DocumentArray` containing the corpus
+            data used during training.
+        :param models: A :class:`SynthesisModels` object containing the names of
+            the models used for relation mining and cross encoding.
+        :param num_relations: Number of relations to mine per query.
+        :param experiment_name: Name of the experiment.
+        :param run_name: Name of the run.
+        :return: Run parameters wrapped up as a config dict.
+        """
+        public = kwargs[PUBLIC] if kwargs.get(PUBLIC) else False
+        data = config.RawDataConfig(
+            queries=query_data,
+            corpus=corpus_data,
+        )
+        relation_mining = config.RelationMiningConfig(
+            models=models.relation_miner
+            if isinstance(models.relation_miner, list)
+            else [models.relation_miner],
+            num_relations=num_relations,
+        )
+        generation_config = config.DataGenerationConfig(
+            data=data,
+            relation_mining=relation_mining,
+            cross_encoder=models.cross_encoder,
+            public=public,
+            experiment_name=experiment_name,
+            run_name=run_name,
+        )
+        return generation_config.dict()
```

### Comparing `finetuner-0.7.6/finetuner/finetuner.py` & `finetuner-0.7.7/finetuner/finetuner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Any, Dict, List, Optional, Union
 
-from docarray import DocumentArray
-
 import hubble
+from finetuner import DocumentArray
 from finetuner.client import FinetunerV1Client
 from finetuner.constants import CREATED_AT, DESCRIPTION, NAME, STATUS
 from finetuner.data import CSVOptions
 from finetuner.excepts import FinetunerServerError
 from finetuner.experiment import Experiment
+from finetuner.model import SynthesisModels
 from finetuner.run import Run
 from hubble import login_required
 
 
 class Finetuner:
     """Finetuner class."""
 
@@ -136,15 +136,15 @@
                 created_at=experiment[CREATED_AT],
                 description=experiment[DESCRIPTION],
             )
             for experiment in experiments
         ]
 
     @login_required
-    def create_run(
+    def create_training_run(
         self,
         model: str,
         train_data: Union[str, DocumentArray],
         eval_data: Optional[Union[str, DocumentArray]] = None,
         val_split: float = 0.0,
         model_artifact: Optional[str] = None,
         run_name: Optional[str] = None,
@@ -170,15 +170,15 @@
         csv_options: Optional[CSVOptions] = None,
         public: bool = False,
         num_items_per_class: int = 4,
         sampler: str = 'auto',
         loss_optimizer: Optional[str] = None,
         loss_optimizer_options: Optional[Dict[str, Any]] = None,
     ) -> Run:
-        """Create a run.
+        """Create a training run.
 
         If an experiment name is not specified, the run will be created in the default
         experiment.
 
         :return: A `Run` object.
         """
         if not experiment_name:
@@ -188,15 +188,15 @@
         if not experiment:
             raise ValueError(
                 (
                     'Unable to start finetuning run as experiment is `None`. '
                     'Make sure you have logged in using `finetuner.login(force=True)`.'
                 )
             )
-        return experiment.create_run(
+        return experiment.create_training_run(
             model=model,
             train_data=train_data,
             eval_data=eval_data,
             val_split=val_split,
             model_artifact=model_artifact,
             run_name=run_name,
             description=description,
@@ -222,14 +222,60 @@
             num_items_per_class=num_items_per_class,
             sampler=sampler,
             loss_optimizer=loss_optimizer,
             loss_optimizer_options=loss_optimizer_options,
         )
 
     @login_required
+    def create_synthesis_run(
+        self,
+        query_data: Union[str, List[str], DocumentArray],
+        corpus_data: Union[str, List[str], DocumentArray],
+        models: SynthesisModels,
+        num_relations: int = 3,
+        run_name: Optional[str] = None,
+        description: Optional[str] = None,
+        experiment_name: Optional[str] = None,
+        device: str = 'cuda',
+        num_workers: int = 4,
+        csv_options: Optional[CSVOptions] = None,
+        public: bool = False,
+    ) -> Run:
+        """Create a synthesis run.
+
+        If an experiment name is not specified, the run will be created in the default
+        experiment.
+
+        :return: A `Run` object.
+        """
+        if not experiment_name:
+            experiment = self._default_experiment
+        else:
+            experiment = self.get_experiment(name=experiment_name)
+        if not experiment:
+            raise ValueError(
+                (
+                    'Unable to start finetuning run as experiment is `None`. '
+                    'Make sure you have logged in using `finetuner.login(force=True)`.'
+                )
+            )
+        return experiment.create_synthesis_run(
+            query_data=query_data,
+            corpus_data=corpus_data,
+            models=models,
+            num_relations=num_relations,
+            run_name=run_name,
+            description=description,
+            device=device,
+            num_workers=num_workers,
+            csv_options=csv_options,
+            public=public,
+        )
+
+    @login_required
     def get_run(self, run_name: str, experiment_name: Optional[str] = None) -> Run:
         """Get run by its name and (optional) experiment.
 
         If an experiment name is not specified, we'll look for the run in the default
         experiment.
 
         :param run_name: Name of the run.
```

### Comparing `finetuner-0.7.6/finetuner/hubble.py` & `finetuner-0.7.7/finetuner/hubble.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,114 @@
 import os
 from typing import Dict, Optional, Tuple, Union
 
-from docarray import DocumentArray
-
+from finetuner import DocumentArray
 from finetuner.constants import ARTIFACTS_DIR, DA_PREFIX
 
 
-def push_data(
+def push_docarray(
+    data: Union[None, str, DocumentArray],
+    name: str,
+    ids2names: Optional[Dict[int, str]] = None,
+) -> Optional[str]:
+    """Upload a DocumentArray to Jina AI Cloud and return its name."""
+    if isinstance(data, DocumentArray):
+        _id = id(data)  # get the reference id
+        if ids2names is not None and _id in ids2names:
+            return ids2names[_id]
+        print(f'Pushing a DocumentArray to Jina AI Cloud under the name {name} ...')
+        data.push(name=name, show_progress=True, public=False)
+        if ids2names is not None:
+            ids2names[id(data)] = name
+        return name
+    return data
+
+
+def push_training_data(
     experiment_name: str,
     run_name: str,
     train_data: Union[str, DocumentArray],
     eval_data: Union[None, str, DocumentArray] = None,
     query_data: Union[None, str, DocumentArray] = None,
     index_data: Union[None, str, DocumentArray] = None,
 ) -> Tuple[Optional[str], ...]:
-    """Upload data to Hubble and returns their names.
+    """Upload data to Jina AI Cloud and returns their names.
 
     Uploads all data needed for fine-tuning - training data,
     evaluation data and query/index data for `EvaluationCallback`.
 
     Data is given either as a `DocumentArray` or
-    a name of the `DocumentArray` that is already pushed to Hubble.
+    a name of the `DocumentArray` that is already pushed to Jina AI Cloud.
 
     Checks not to upload same dataset twice.
 
     :param experiment_name: Name of the experiment.
     :param run_name: Name of the run.
     :param train_data: Training data.
     :param eval_data: Evaluation data.
     :param query_data: Query data for `EvaluationCallback`.
     :param index_data: Index data for `EvaluationCallback`.
     :return: Name(s) of the uploaded data.
     """
-
-    def _push_docarray(
-        data: Union[None, str, DocumentArray], name: str, ids2names: Dict[int, str]
-    ) -> Optional[str]:
-        if isinstance(data, DocumentArray):
-            _id = id(data)  # get the reference id
-            if _id in ids2names:
-                return ids2names[_id]
-            print(f'Pushing a DocumentArray to Hubble under the name {name} ...')
-            data.push(name=name, show_progress=True, public=False)
-            ids2names[id(data)] = name
-            return name
-        return data
-
     _ids2names = dict()
     return (
-        _push_docarray(
+        push_docarray(
             train_data, f'{DA_PREFIX}-{experiment_name}-{run_name}-train', _ids2names
         ),
-        _push_docarray(
+        push_docarray(
             eval_data, f'{DA_PREFIX}-{experiment_name}-{run_name}-eval', _ids2names
         ),
-        _push_docarray(
+        push_docarray(
             query_data, f'{DA_PREFIX}-{experiment_name}-{run_name}-query', _ids2names
         ),
-        _push_docarray(
+        push_docarray(
             index_data, f'{DA_PREFIX}-{experiment_name}-{run_name}-index', _ids2names
         ),
     )
 
 
+def push_synthesis_data(
+    experiment_name: str,
+    run_name: str,
+    query_data: Union[str, DocumentArray],
+    corpus_data: Union[str, DocumentArray],
+) -> Tuple[Optional[str], Optional[str]]:
+    """Upload data to Jina AI Cloud and returns their names.
+
+    Uploads all data needed for data synthesis - query data and corpus data.
+
+    Data is given either as a `DocumentArray` or
+    a name of the `DocumentArray` that is already pushed to Jina AI Cloud.
+
+    Checks not to upload same dataset twice.
+
+    :param experiment_name: Name of the experiment.
+    :param run_name: Name of the run.
+    :param query_data: Query data.
+    :param corpus_data: Corpus data.
+    :return: Names of the uploaded query and corpus data.
+    """
+    _ids2names = dict()
+    return (
+        push_docarray(
+            query_data, f'{DA_PREFIX}-{experiment_name}-{run_name}-query', _ids2names
+        ),
+        push_docarray(
+            corpus_data, f'{DA_PREFIX}-{experiment_name}-{run_name}-corpus', _ids2names
+        ),
+    )
+
+
 def download_artifact(
     client, artifact_id: str, run_name: str, directory: str = ARTIFACTS_DIR
 ) -> str:
-    """Download artifact from Hubble by its ID.
+    """Download artifact from Jina AI Cloud by its ID.
 
     :param client: Hubble client instance.
-    :param artifact_id: The artifact id stored in the Hubble.
+    :param artifact_id: The artifact id stored in the Jina AI Cloud.
     :param run_name: The name of the run as artifact name to store locally.
     :param directory: Directory where the artifact will be stored.
     :returns: A string that indicates the download path.
     """
     os.makedirs(directory, exist_ok=True)
 
     path = os.path.join(directory, f'{run_name}.zip')
```

### Comparing `finetuner-0.7.6/finetuner/names.py` & `finetuner-0.7.7/finetuner/names.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.6/finetuner.egg-info/PKG-INFO` & `finetuner-0.7.7/finetuner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetuner
-Version: 0.7.6
+Version: 0.7.7
 Summary: Task-oriented finetuning for better embeddings on neural search.
 Home-page: https://github.com/jina-ai/finetuner/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai
@@ -21,15 +21,15 @@
         <b>Task-oriented finetuning for better embeddings on neural search</b>
         </p>
         
         <p align=center>
         <a href="https://pypi.org/project/finetuner/"><img alt="PyPI" src="https://img.shields.io/pypi/v/finetuner?label=Release&style=flat-square"></a>
         <a href="https://codecov.io/gh/jina-ai/finetuner"><img alt="Codecov branch" src="https://img.shields.io/codecov/c/github/jina-ai/finetuner/main?logo=Codecov&logoColor=white&style=flat-square"></a>
         <a href="https://pypistats.org/packages/finetuner"><img alt="PyPI - Downloads from official pypistats" src="https://img.shields.io/pypi/dm/finetuner?style=flat-square"></a>
-        <a href="https://slack.jina.ai"><img src="https://img.shields.io/badge/Slack-3.6k-blueviolet?logo=slack&amp;logoColor=white&style=flat-square"></a>
+        <a href="https://discord.jina.ai"><img src="https://img.shields.io/discord/1106542220112302130?logo=discord&logoColor=white&style=flat-square"></a>
         </p>
         
         <!-- start elevator-pitch -->
         
         Fine-tuning is an effective way to improve performance on [neural search](https://jina.ai/news/what-is-neural-search-and-learn-to-build-a-neural-search-engine/) tasks.
         However, setting up and performing fine-tuning can be very time-consuming and resource-intensive.
         
@@ -157,15 +157,15 @@
         
         Make sure you have Python 3.8+ installed. Finetuner can be installed via `pip` by executing:
         
         ```bash
         pip install -U finetuner
         ```
         
-        If you want to encode `docarray.DocumentArray` objects with the `finetuner.encode` function, you need to install 
+        If you want to encode local data with the `finetuner.encode` function, you need to install 
         `"finetuner[full]"`. This includes a number of additional dependencies, which are necessary for encoding: Torch, 
         Torchvision and OpenCLIP:
         
         ```bash
         pip install "finetuner[full]"
         ```
         
@@ -187,15 +187,15 @@
         <!-- end finetuner-articles -->
         
         <!-- start support-pitch -->
         ## Support
         
         - Use [Discussions](https://github.com/jina-ai/finetuner/discussions) to talk about your use cases, questions, and
           support queries.
-        - Join our [Slack community](https://slack.jina.ai) and chat with other Jina AI community members about ideas.
+        - Join our [Discord community](https://discord.jina.ai) and chat with other community members about ideas.
         - Join our [Engineering All Hands](https://youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to discuss your use case and learn Jina AI new features.
             - **When?** The second Tuesday of every month
             - **Where?**
               Zoom ([see our public events calendar](https://calendar.google.com/calendar/embed?src=c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com&ctz=Europe%2FBerlin)/[.ical](https://calendar.google.com/calendar/ical/c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com/public/basic.ics))
               and [live stream on YouTube](https://youtube.com/c/jina-ai)
         - Subscribe to the latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: finetuner Version: 0.7.6 Summary: Task-oriented
+Metadata-Version: 2.1 Name: finetuner Version: 0.7.7 Summary: Task-oriented
 finetuning for better embeddings on neural search. Home-page: https://
 github.com/jina-ai/finetuner/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai Project-URL: Source,
 https://github.com/jina-ai/finetuner/ Project-URL: Tracker, https://github.com/
 jina-ai/finetuner/issues Description:
 
 [Finetuner logo: Finetuner helps you to create experiments in order to improve
   embeddings on search tasks. It accompanies you to deliver the last mile of
               performance-tuning for neural search applications.]
         Task-oriented finetuning for better embeddings on neural search
  [PyPI] [Codecov_branch] [PyPI_-_Downloads_from_official_pypistats] [https://
-                       img.shields.io/badge/Slack-3.6k-
-         blueviolet?logo=slack&amp;logoColor=white&style=flat-square]
+                            img.shields.io/discord/
+      1106542220112302130?logo=discord&logoColor=white&style=flat-square]
  Fine-tuning is an effective way to improve performance on [neural search]
 (https://jina.ai/news/what-is-neural-search-and-learn-to-build-a-neural-search-
 engine/) tasks. However, setting up and performing fine-tuning can be very
 time-consuming and resource-intensive. Jina AI's Finetuner makes fine-tuning
 easier and faster by streamlining the workflow and handling all the complexity
 and infrastructure in the cloud. With Finetuner, you can easily enhance the
 performance of pre-trained models, making them production-ready [without
@@ -51,40 +51,39 @@
            (German)
 PointNet++ ModelNet40 3D   mRR    0.791      0.891     12.7%  [Open_In_Colab]
            Mesh Search     Recall 0.154      0.242     57.1%
 All metrics were evaluated for k@20 after training for 5 epochs using the Adam
 optimizer with learning rates of 1e-4 for ResNet, 1e-7 for CLIP and 1e-5 for
 the BERT models, 5e-4 for PointNet++  ## Install Make sure you have Python 3.8+
 installed. Finetuner can be installed via `pip` by executing: ```bash pip
-install -U finetuner ``` If you want to encode `docarray.DocumentArray` objects
-with the `finetuner.encode` function, you need to install `"finetuner[full]"`.
-This includes a number of additional dependencies, which are necessary for
-encoding: Torch, Torchvision and OpenCLIP: ```bash pip install "finetuner
-[full]" ```  > â ï¸ Starting with version 0.5.0, Finetuner computing is
-performed on Jina AI Cloud. The last local version is `0.4.1`. > This version
-is still available for installation via `pip`. See [Finetuner git tags and
-releases](https://github.com/jina-ai/finetuner/releases).  ## Articles about
-Finetuner Check out our published blogposts and tutorials to see Finetuner in
-action! - [Fine-tuning with Low Budget and High Expectations](https://jina.ai/
-news/fine-tuning-with-low-budget-and-high-expectations/) - [Hype and Hybrids:
-Search is more than Keywords and Vectors](https://jina.ai/news/hype-and-
-hybrids-multimodal-search-means-more-than-keywords-and-vectors-2/) - [Improving
-Search Quality for Non-English Queries with Fine-tuned Multilingual CLIP
-Models](https://jina.ai/news/improving-search-quality-non-english-queries-fine-
-tuned-multilingual-clip-models/) - [How Much Do We Get by Finetuning CLIP?]
-(https://jina.ai/news/applying-jina-ai-finetuner-to-clip-less-data-smaller-
-models-higher-performance/)   ## Support - Use [Discussions](https://
-github.com/jina-ai/finetuner/discussions) to talk about your use cases,
-questions, and support queries. - Join our [Slack community](https://
-slack.jina.ai) and chat with other Jina AI community members about ideas. -
-Join our [Engineering All Hands](https://youtube.com/
-playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to discuss your use
-case and learn Jina AI new features. - **When?** The second Tuesday of every
-month - **Where?** Zoom ([see our public events calendar](https://
-calendar.google.com/calendar/
+install -U finetuner ``` If you want to encode local data with the
+`finetuner.encode` function, you need to install `"finetuner[full]"`. This
+includes a number of additional dependencies, which are necessary for encoding:
+Torch, Torchvision and OpenCLIP: ```bash pip install "finetuner[full]" ```  >
+â ï¸ Starting with version 0.5.0, Finetuner computing is performed on Jina AI
+Cloud. The last local version is `0.4.1`. > This version is still available for
+installation via `pip`. See [Finetuner git tags and releases](https://
+github.com/jina-ai/finetuner/releases).  ## Articles about Finetuner Check out
+our published blogposts and tutorials to see Finetuner in action! - [Fine-
+tuning with Low Budget and High Expectations](https://jina.ai/news/fine-tuning-
+with-low-budget-and-high-expectations/) - [Hype and Hybrids: Search is more
+than Keywords and Vectors](https://jina.ai/news/hype-and-hybrids-multimodal-
+search-means-more-than-keywords-and-vectors-2/) - [Improving Search Quality for
+Non-English Queries with Fine-tuned Multilingual CLIP Models](https://jina.ai/
+news/improving-search-quality-non-english-queries-fine-tuned-multilingual-clip-
+models/) - [How Much Do We Get by Finetuning CLIP?](https://jina.ai/news/
+applying-jina-ai-finetuner-to-clip-less-data-smaller-models-higher-performance/
+)   ## Support - Use [Discussions](https://github.com/jina-ai/finetuner/
+discussions) to talk about your use cases, questions, and support queries. -
+Join our [Discord community](https://discord.jina.ai) and chat with other
+community members about ideas. - Join our [Engineering All Hands](https://
+youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to
+discuss your use case and learn Jina AI new features. - **When?** The second
+Tuesday of every month - **Where?** Zoom ([see our public events calendar]
+(https://calendar.google.com/calendar/
 embed?src=c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com&ctz=Europe%2FBerlin)/
 [.ical](https://calendar.google.com/calendar/ical/
 c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com/public/basic.ics)) and
 [live stream on YouTube](https://youtube.com/c/jina-ai) - Subscribe to the
 latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
 ## Join Us Finetuner is backed by [Jina AI](https://jina.ai) and licensed under
 [Apache-2.0](./LICENSE). [We are actively hiring](https://jobs.jina.ai) AI
```

### Comparing `finetuner-0.7.6/finetuner.egg-info/SOURCES.txt` & `finetuner-0.7.7/finetuner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.6/setup.py` & `finetuner-0.7.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,20 +25,20 @@
         long_description=_long_description,
         long_description_content_type='text/markdown',
         zip_safe=False,
         setup_requires=['setuptools>=18.0', 'wheel'],
         install_requires=[
             'docarray[common]<0.30.0',
             'trimesh==3.16.4',
-            'finetuner-stubs==0.13.4',
+            'finetuner-stubs==0.13.6',
             'jina-hubble-sdk==0.33.1',
         ],
         extras_require={
             'full': [
-                'finetuner-commons==0.13.4',
+                'finetuner-commons==0.13.6',
             ],
             'test': [
                 'black==22.3.0',
                 'flake8==5.0.4',
                 'isort==5.10.1',
                 'pytest==7.0.0',
                 'pytest-cov==3.0.0',
```

