# Comparing `tmp/scikit-llm-0.1.0b2.tar.gz` & `tmp/scikit-llm-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-llm-0.1.0b2.tar", last modified: Fri May 19 20:03:18 2023, max compression
+gzip compressed data, was "scikit-llm-0.1.0b3.tar", last modified: Wed May 24 20:41:20 2023, max compression
```

## Comparing `scikit-llm-0.1.0b2.tar` & `scikit-llm-0.1.0b3.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-19 20:03:18.733873 scikit-llm-0.1.0b2/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1077 2023-05-12 18:41:11.000000 scikit-llm-0.1.0b2/LICENSE
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     5943 2023-05-19 20:03:18.733554 scikit-llm-0.1.0b2/PKG-INFO
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     5410 2023-05-19 20:00:45.000000 scikit-llm-0.1.0b2/README.md
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      780 2023-05-19 20:02:19.000000 scikit-llm-0.1.0b2/pyproject.toml
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-19 20:03:18.729107 scikit-llm-0.1.0b2/scikit_llm.egg-info/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     5943 2023-05-19 20:03:18.000000 scikit-llm-0.1.0b2/scikit_llm.egg-info/PKG-INFO
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      566 2023-05-19 20:03:18.000000 scikit-llm-0.1.0b2/scikit_llm.egg-info/SOURCES.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)        1 2023-05-19 20:03:18.000000 scikit-llm-0.1.0b2/scikit_llm.egg-info/dependency_links.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)       62 2023-05-19 20:03:18.000000 scikit-llm-0.1.0b2/scikit_llm.egg-info/requires.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)        6 2023-05-19 20:03:18.000000 scikit-llm-0.1.0b2/scikit_llm.egg-info/top_level.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)       38 2023-05-19 20:03:18.733980 scikit-llm-0.1.0b2/setup.cfg
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-19 20:03:18.729967 scikit-llm-0.1.0b2/skllm/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)       97 2023-05-12 18:41:11.000000 scikit-llm-0.1.0b2/skllm/__init__.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      592 2023-05-13 17:42:03.000000 scikit-llm-0.1.0b2/skllm/config.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-19 20:03:18.730926 scikit-llm-0.1.0b2/skllm/datasets/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      142 2023-05-13 15:03:57.000000 scikit-llm-0.1.0b2/skllm/datasets/__init__.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     5870 2023-05-13 15:02:46.000000 scikit-llm-0.1.0b2/skllm/datasets/multi_class.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1438 2023-05-13 15:03:34.000000 scikit-llm-0.1.0b2/skllm/datasets/multi_label.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-19 20:03:18.731222 scikit-llm-0.1.0b2/skllm/models/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     5070 2023-05-19 19:12:30.000000 scikit-llm-0.1.0b2/skllm/models/gpt_zero_shot_clf.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-19 20:03:18.732631 scikit-llm-0.1.0b2/skllm/openai/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      901 2023-05-19 19:00:05.000000 scikit-llm-0.1.0b2/skllm/openai/chatgpt.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      111 2023-05-19 18:59:36.000000 scikit-llm-0.1.0b2/skllm/openai/credentials.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      820 2023-05-19 19:02:41.000000 scikit-llm-0.1.0b2/skllm/openai/embeddings.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      730 2023-05-19 19:11:38.000000 scikit-llm-0.1.0b2/skllm/openai/mixin.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     2186 2023-05-12 18:41:11.000000 scikit-llm-0.1.0b2/skllm/openai/prompts.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-19 20:03:18.733205 scikit-llm-0.1.0b2/skllm/preprocessing/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)       60 2023-05-19 18:51:50.000000 scikit-llm-0.1.0b2/skllm/preprocessing/__init__.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1394 2023-05-19 19:23:03.000000 scikit-llm-0.1.0b2/skllm/preprocessing/gpt_vectorizer.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      244 2023-05-19 18:51:39.000000 scikit-llm-0.1.0b2/skllm/utils.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-24 20:41:20.193965 scikit-llm-0.1.0b3/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1077 2023-05-12 18:41:11.000000 scikit-llm-0.1.0b3/LICENSE
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     7102 2023-05-24 20:41:20.193643 scikit-llm-0.1.0b3/PKG-INFO
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     6569 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/README.md
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      780 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/pyproject.toml
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-24 20:41:20.185584 scikit-llm-0.1.0b3/scikit_llm.egg-info/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     7102 2023-05-24 20:41:20.000000 scikit-llm-0.1.0b3/scikit_llm.egg-info/PKG-INFO
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      661 2023-05-24 20:41:20.000000 scikit-llm-0.1.0b3/scikit_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)        1 2023-05-24 20:41:20.000000 scikit-llm-0.1.0b3/scikit_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)       62 2023-05-24 20:41:20.000000 scikit-llm-0.1.0b3/scikit_llm.egg-info/requires.txt
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)        6 2023-05-24 20:41:20.000000 scikit-llm-0.1.0b3/scikit_llm.egg-info/top_level.txt
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)       38 2023-05-24 20:41:20.194186 scikit-llm-0.1.0b3/setup.cfg
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-24 20:41:20.186932 scikit-llm-0.1.0b3/skllm/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)       97 2023-05-12 18:41:11.000000 scikit-llm-0.1.0b3/skllm/__init__.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      592 2023-05-13 17:42:03.000000 scikit-llm-0.1.0b3/skllm/config.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-24 20:41:20.188471 scikit-llm-0.1.0b3/skllm/datasets/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      209 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/skllm/datasets/__init__.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     5870 2023-05-13 15:02:46.000000 scikit-llm-0.1.0b3/skllm/datasets/multi_class.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1438 2023-05-13 15:03:34.000000 scikit-llm-0.1.0b3/skllm/datasets/multi_label.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     2729 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/skllm/datasets/summarization.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-24 20:41:20.188818 scikit-llm-0.1.0b3/skllm/models/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     5070 2023-05-19 19:12:30.000000 scikit-llm-0.1.0b3/skllm/models/gpt_zero_shot_clf.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-24 20:41:20.191778 scikit-llm-0.1.0b3/skllm/openai/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1822 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/skllm/openai/base_gpt.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1151 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/skllm/openai/chatgpt.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      111 2023-05-19 18:59:36.000000 scikit-llm-0.1.0b3/skllm/openai/credentials.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      894 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/skllm/openai/embeddings.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      730 2023-05-19 19:11:38.000000 scikit-llm-0.1.0b3/skllm/openai/mixin.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     2554 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/skllm/openai/prompts.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-24 20:41:20.192870 scikit-llm-0.1.0b3/skllm/preprocessing/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      121 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/skllm/preprocessing/__init__.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      694 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/skllm/preprocessing/gpt_summarizer.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1394 2023-05-19 19:23:03.000000 scikit-llm-0.1.0b3/skllm/preprocessing/gpt_vectorizer.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      296 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/skllm/utils.py
```

### Comparing `scikit-llm-0.1.0b2/LICENSE` & `scikit-llm-0.1.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.0b2/PKG-INFO` & `scikit-llm-0.1.0b3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: scikit-llm
-Version: 0.1.0b2
-Summary: Scikit-LLM: Seamlessly integrate powerful language models like ChatGPT into scikit-learn for enhanced text analysis tasks.
-Author-email: Oleg Kostromin <kostromin97@gmail.com>, Iryna Kondrashchenko <iryna230520@gmail.com>
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
   <img src="https://github.com/iryna-kondr/scikit-llm/blob/main/logo.png?raw=true" max-height="200"/>
 </p>
 
 # Scikit-LLM: Sklearn Meets Large Language Models
 
 Seamlessly integrate powerful language models like ChatGPT into scikit-learn for enhanced text analysis tasks.
@@ -26,30 +13,33 @@
 ```
 
 ## Support us 🤝
 
 You can support the project in the following ways:
 
 - ⭐ Star Scikit-LLM on GitHub (click the star button in the top right corner)
+- 🐦 Check out our related project - [Falcon AutoML](https://github.com/OKUA1/falcon)
 - 💡 Provide your feedback or propose ideas in the [issues](https://github.com/iryna-kondr/scikit-llm/issues) section
 - 🔗 Post about Scikit-LLM on LinkedIn or other platforms
-- 🪶 Check out our related project - [Falcon AutoML](https://github.com/OKUA1/falcon)
-
 
 ## Documentation 📚
 
 ### Configuring OpenAI API Key
 At the moment Scikit-LLM is only compatible with some of the OpenAI models. Hence, a user-provided OpenAI API key is required.
 
 ```python
 from skllm.config import SKLLMConfig
 SKLLMConfig.set_openai_key("<YOUR_KEY>")
 SKLLMConfig.set_openai_org("<YOUR_ORGANISATION>")
 ```
 
+**Important notice:** 
+- If you have a free trial OpenAI account, the [rate limits](https://platform.openai.com/docs/guides/rate-limits/overview) are not sufficient (specifically 3 requests per minute). Please switch to the "pay as you go" plan first.
+- When calling `SKLLMConfig.set_openai_org`, you have to provide your organization ID and **NOT** the name. You can find your ID [here](https://platform.openai.com/account/org-settings).
+
 ### Zero-Shot Text Classification
 
 One of the powerful ChatGPT features is the ability to perform text classification without being re-trained. For that, the only requirement is that the labels must be descriptive.
 
 We provide a class `ZeroShotGPTClassifier` that allows to create such a model as a regular scikit-learn classifier.
 
 Example 1: Training as a regular classifier
@@ -153,18 +143,34 @@
 
 steps = [('GPT', GPTVectorizer()), ('Clf', XGBClassifier())]
 clf = Pipeline(steps)
 clf.fit(X_train, y_train_encoded)
 yh = clf.predict(X_test)
 ```
 
+### Text Summarization
+
+GPT excels at performing summarization tasks. Therefore, we provide `GPTSummarizer` that can be used both as stand-alone estimator, or as a preprocessor (in this case we can make an analogy with a dimensionality reduction preprocessor).
+
+Example:
+```python
+from skllm.preprocessing import GPTSummarizer
+from skllm.datasets import get_summarization_dataset
+
+X = get_summarization_dataset()
+s = GPTSummarizer(openai_model = 'gpt-3.5-turbo', max_words = 15)
+summaries = s.fit_transform(X)
+```
+
+Please be aware that the `max_words` hyperparameter sets a soft limit, which is not strictly enforced outside of the prompt. Therefore, in some cases, the actual number of words might be slightly higher.
+
 ## Roadmap 🧭
 
 - [x] Zero-Shot Classification with OpenAI GPT 3/4
     - [x] Multiclass classification
     - [x] Multi-label classification
     - [x] ChatGPT models
     - [ ] InstructGPT models
 - [ ] Few shot classifier
 - [x] GPT Vectorizer
 - [ ] GPT Fine-tuning (optional)
-- [ ] Integration of other LLMs
+- [ ] Integration of other LLMs
```

### Comparing `scikit-llm-0.1.0b2/pyproject.toml` & `scikit-llm-0.1.0b3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 dependencies = [
 "scikit-learn>=1.1.0",
 "pandas>=1.5.0",
 "openai>=0.27.0",
 "tqdm>=4.60.0",
 ]
 name = "scikit-llm"
-version = "0.1.0b2"
+version = "0.1.0b3"
 authors = [
   { name="Oleg Kostromin", email="kostromin97@gmail.com" },
   { name="Iryna Kondrashchenko", email="iryna230520@gmail.com" },
 ]
 description = "Scikit-LLM: Seamlessly integrate powerful language models like ChatGPT into scikit-learn for enhanced text analysis tasks."
 readme = "README.md"
 license = {text = "MIT"}
```

### Comparing `scikit-llm-0.1.0b2/scikit_llm.egg-info/PKG-INFO` & `scikit-llm-0.1.0b3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-llm
-Version: 0.1.0b2
+Version: 0.1.0b3
 Summary: Scikit-LLM: Seamlessly integrate powerful language models like ChatGPT into scikit-learn for enhanced text analysis tasks.
 Author-email: Oleg Kostromin <kostromin97@gmail.com>, Iryna Kondrashchenko <iryna230520@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -26,30 +26,33 @@
 ```
 
 ## Support us 🤝
 
 You can support the project in the following ways:
 
 - ⭐ Star Scikit-LLM on GitHub (click the star button in the top right corner)
+- 🐦 Check out our related project - [Falcon AutoML](https://github.com/OKUA1/falcon)
 - 💡 Provide your feedback or propose ideas in the [issues](https://github.com/iryna-kondr/scikit-llm/issues) section
 - 🔗 Post about Scikit-LLM on LinkedIn or other platforms
-- 🪶 Check out our related project - [Falcon AutoML](https://github.com/OKUA1/falcon)
-
 
 ## Documentation 📚
 
 ### Configuring OpenAI API Key
 At the moment Scikit-LLM is only compatible with some of the OpenAI models. Hence, a user-provided OpenAI API key is required.
 
 ```python
 from skllm.config import SKLLMConfig
 SKLLMConfig.set_openai_key("<YOUR_KEY>")
 SKLLMConfig.set_openai_org("<YOUR_ORGANISATION>")
 ```
 
+**Important notice:** 
+- If you have a free trial OpenAI account, the [rate limits](https://platform.openai.com/docs/guides/rate-limits/overview) are not sufficient (specifically 3 requests per minute). Please switch to the "pay as you go" plan first.
+- When calling `SKLLMConfig.set_openai_org`, you have to provide your organization ID and **NOT** the name. You can find your ID [here](https://platform.openai.com/account/org-settings).
+
 ### Zero-Shot Text Classification
 
 One of the powerful ChatGPT features is the ability to perform text classification without being re-trained. For that, the only requirement is that the labels must be descriptive.
 
 We provide a class `ZeroShotGPTClassifier` that allows to create such a model as a regular scikit-learn classifier.
 
 Example 1: Training as a regular classifier
@@ -153,14 +156,30 @@
 
 steps = [('GPT', GPTVectorizer()), ('Clf', XGBClassifier())]
 clf = Pipeline(steps)
 clf.fit(X_train, y_train_encoded)
 yh = clf.predict(X_test)
 ```
 
+### Text Summarization
+
+GPT excels at performing summarization tasks. Therefore, we provide `GPTSummarizer` that can be used both as stand-alone estimator, or as a preprocessor (in this case we can make an analogy with a dimensionality reduction preprocessor).
+
+Example:
+```python
+from skllm.preprocessing import GPTSummarizer
+from skllm.datasets import get_summarization_dataset
+
+X = get_summarization_dataset()
+s = GPTSummarizer(openai_model = 'gpt-3.5-turbo', max_words = 15)
+summaries = s.fit_transform(X)
+```
+
+Please be aware that the `max_words` hyperparameter sets a soft limit, which is not strictly enforced outside of the prompt. Therefore, in some cases, the actual number of words might be slightly higher.
+
 ## Roadmap 🧭
 
 - [x] Zero-Shot Classification with OpenAI GPT 3/4
     - [x] Multiclass classification
     - [x] Multi-label classification
     - [x] ChatGPT models
     - [ ] InstructGPT models
```

### Comparing `scikit-llm-0.1.0b2/scikit_llm.egg-info/SOURCES.txt` & `scikit-llm-0.1.0b3/scikit_llm.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 scikit_llm.egg-info/top_level.txt
 skllm/__init__.py
 skllm/config.py
 skllm/utils.py
 skllm/datasets/__init__.py
 skllm/datasets/multi_class.py
 skllm/datasets/multi_label.py
+skllm/datasets/summarization.py
 skllm/models/gpt_zero_shot_clf.py
+skllm/openai/base_gpt.py
 skllm/openai/chatgpt.py
 skllm/openai/credentials.py
 skllm/openai/embeddings.py
 skllm/openai/mixin.py
 skllm/openai/prompts.py
 skllm/preprocessing/__init__.py
+skllm/preprocessing/gpt_summarizer.py
 skllm/preprocessing/gpt_vectorizer.py
```

### Comparing `scikit-llm-0.1.0b2/skllm/config.py` & `scikit-llm-0.1.0b3/skllm/config.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.0b2/skllm/datasets/multi_class.py` & `scikit-llm-0.1.0b3/skllm/datasets/multi_class.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.0b2/skllm/datasets/multi_label.py` & `scikit-llm-0.1.0b3/skllm/datasets/multi_label.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.0b2/skllm/models/gpt_zero_shot_clf.py` & `scikit-llm-0.1.0b3/skllm/models/gpt_zero_shot_clf.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.0b2/skllm/openai/embeddings.py` & `scikit-llm-0.1.0b3/skllm/openai/embeddings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import openai
+from time import sleep
 from skllm.openai.credentials import set_credentials
 
 def get_embedding(
     text, key: str, org: str, model="text-embedding-ada-002", max_retries=3
 ):
     set_credentials(key, org)
     text = text.replace("\n", " ")
     error_msg = None
+    error_type = None
     for _ in range(max_retries):
         try:
             emb = openai.Embedding.create(input=[text], model=model)["data"][0][
                 "embedding"
             ]
             if not isinstance(emb, list):
                 raise ValueError(f"Encountered unknown embedding format. Expected list, got {type(emb)}")
             return emb
         except Exception as e:
             error_msg = str(e)
-            continue
+            error_type =  type(e).__name__
+            sleep(3)
     raise RuntimeError(
-        f"Could not obtain the embedding after retrying {max_retries} times. \nLast captured error: `{error_msg}`"
+        f"Could not obtain the embedding after {max_retries} retries: `{error_type} :: {error_msg}`"
     )
```

### Comparing `scikit-llm-0.1.0b2/skllm/openai/mixin.py` & `scikit-llm-0.1.0b3/skllm/openai/mixin.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.0b2/skllm/openai/prompts.py` & `scikit-llm-0.1.0b3/skllm/openai/prompts.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
         "2. List of categories the text sample can be assigned to. The list is delimited with square brackets. The categories in the list are enclosed in the single quotes and comma separated.",
         "",
         "Perform the following tasks:",
         "1. Identify to which category the provided text belongs to with the highest probability.",
         "2. Assign the provided text to that category.",
         "3. Provide your response in a JSON format containing a single key `label` and a value corresponding to the assigned category. Do not provide any additional information except the JSON.",
         "\n", 
-        f"List of categories: {repr(labels)}"
+        f"List of categories: {repr(labels)}",
         "\n",
         f"Text sample: ```{x}```",
         "\n",
         "Your JSON response: "
     ]
     prompt = "\n".join(lines)
     return prompt
@@ -23,17 +23,28 @@
         "You will be provided with the following information:",
         "1. An arbitrary text sample. The sample is delimited with triple backticks.",
         f"2. List of categories the text sample can be assigned to. The list is delimited with square brackets. The categories in the list are enclosed in the single quotes and comma separated. The text sample belongs to at least one category but cannot exceed {max_cats}.",
         "",
         "Perform the following tasks:",
         "1. Identify to which categories the provided text belongs to with the highest probability.",
         f"2. Assign the text sample to at least 1 but up to {max_cats} categories based on the probabilities.",
-        "3. Provide your response in a JSON format containing a single key `label` and a value corresponding to the list of assigned categories. Do not provide any additional information except the JSON."
+        "3. Provide your response in a JSON format containing a single key `label` and a value corresponding to the list of assigned categories. Do not provide any additional information except the JSON.",
         "\n", 
-        f"List of categories: {repr(labels)}"
+        f"List of categories: {repr(labels)}",
         "\n",
         f"Text sample: ```{x}```",
         "\n",
         "Your JSON response: "
     ]
     prompt = "\n".join(lines)
+    return prompt
+
+def get_summary_prompt(x, max_words):
+    lines = [
+        "Your task is to generate a summary of the text sample.",
+        f"Summarize the text sample provided below, delimited by triple backticks, in at most {max_words} words.",
+        "\n",
+        f"Text sample: ```{x}```",
+        f"Summarized text:"
+    ]
+    prompt = "\n".join(lines)
     return prompt
```

### Comparing `scikit-llm-0.1.0b2/skllm/preprocessing/gpt_vectorizer.py` & `scikit-llm-0.1.0b3/skllm/preprocessing/gpt_vectorizer.py`

 * *Files identical despite different names*

