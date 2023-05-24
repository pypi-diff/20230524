# Comparing `tmp/open_gpt_torch-0.0.2.tar.gz` & `tmp/open_gpt_torch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_gpt_torch-0.0.2.tar", max compression
+gzip compressed data, was "open_gpt_torch-0.0.3.tar", max compression
```

## Comparing `open_gpt_torch-0.0.2.tar` & `open_gpt_torch-0.0.3.tar`

### file list

```diff
@@ -1,47 +1,48 @@
--rw-r--r--   0        0        0    10825 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/LICENSE
--rw-r--r--   0        0        0     6092 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/README.md
--rw-r--r--   0        0        0      853 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/__init__.py
--rw-r--r--   0        0        0      107 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/__main__.py
--rw-r--r--   0        0        0        0 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/cli/__init__.py
--rw-r--r--   0        0        0     1057 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/cli/application.py
--rw-r--r--   0        0        0      508 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/cli/command_loader.py
--rw-r--r--   0        0        0        0 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/cli/commands/__init__.py
--rw-r--r--   0        0        0      567 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/cli/commands/about.py
--rw-r--r--   0        0        0      953 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/cli/commands/playground.py
--rw-r--r--   0        0        0     1229 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/cli/commands/serve.py
--rw-r--r--   0        0        0     3771 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/factory.py
--rw-r--r--   0        0        0     2509 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/helper.py
--rw-r--r--   0        0        0      498 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/logging.py
--rw-r--r--   0        0        0        0 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/flamingo/__init__.py
--rw-r--r--   0        0        0     6038 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/flamingo/flamingo_lm.py
--rw-r--r--   0        0        0     9043 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/flamingo/flamingo_model.py
--rw-r--r--   0        0        0     5644 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/flamingo/loading.py
--rw-r--r--   0        0        0     2511 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/flamingo/modeling.py
--rw-r--r--   0        0        0     3782 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/generation.py
--rw-r--r--   0        0        0        0 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/llama/__init__.py
--rw-r--r--   0        0        0     1407 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/llama/modeling.py
--rw-r--r--   0        0        0     2501 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/loading.py
--rw-r--r--   0        0        0     2101 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/modeling.py
--rw-r--r--   0        0        0        0 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/moss/__init__.py
--rw-r--r--   0        0        0     3549 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/moss/modeling.py
--rw-r--r--   0        0        0        0 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/pythia/__init__.py
--rw-r--r--   0        0        0      814 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/pythia/modeling.py
--rw-r--r--   0        0        0        0 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/stablelm/__init__.py
--rw-r--r--   0        0        0     2740 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/stablelm/modeling.py
--rw-r--r--   0        0        0        0 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/vicuna/__init__.py
--rw-r--r--   0        0        0     3372 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/vicuna/loading.py
--rw-r--r--   0        0        0     1534 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/vicuna/modeling.py
--rw-r--r--   0        0        0     2905 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/profile.py
--rw-r--r--   0        0        0        0 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/serve/__init__.py
--rw-r--r--   0        0        0       36 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/serve/executors/__init__.py
--rw-r--r--   0        0        0     1778 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/serve/executors/base.py
--rw-r--r--   0        0        0     2132 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/serve/executors/flamingo.py
--rw-r--r--   0        0        0      171 2023-05-16 05:18:44.866036 open_gpt_torch-0.0.2/open_gpt/serve/executors/utils.py
--rw-r--r--   0        0        0      931 2023-05-16 05:18:44.866036 open_gpt_torch-0.0.2/open_gpt/serve/gateway.py
--rw-r--r--   0        0        0        0 2023-05-16 05:18:44.866036 open_gpt_torch-0.0.2/open_gpt/serve/playground/__init__.py
--rw-r--r--   0        0        0     4689 2023-05-16 05:18:44.866036 open_gpt_torch-0.0.2/open_gpt/serve/playground/gradio.py
--rw-r--r--   0        0        0     7396 2023-05-16 05:18:44.866036 open_gpt_torch-0.0.2/open_gpt/serve/playground/gradio_chatbot.py
--rw-r--r--   0        0        0     2714 2023-05-16 05:18:44.866036 open_gpt_torch-0.0.2/open_gpt/serve/playground/gradio_css.py
--rw-r--r--   0        0        0     3097 2023-05-16 05:18:44.866036 open_gpt_torch-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    19264 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    10825 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/LICENSE
+-rw-r--r--   0        0        0     7611 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/README.md
+-rw-r--r--   0        0        0      929 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/cli/__init__.py
+-rw-r--r--   0        0        0     1057 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/cli/application.py
+-rw-r--r--   0        0        0      508 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/cli/command_loader.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/cli/commands/__init__.py
+-rw-r--r--   0        0        0      567 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/cli/commands/about.py
+-rw-r--r--   0        0        0      953 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/cli/commands/playground.py
+-rw-r--r--   0        0        0     2031 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/cli/commands/serve.py
+-rw-r--r--   0        0        0     4103 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/factory.py
+-rw-r--r--   0        0        0     2469 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/helper.py
+-rw-r--r--   0        0        0      498 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/logging.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/models/flamingo/__init__.py
+-rw-r--r--   0        0        0     6038 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/models/flamingo/flamingo_lm.py
+-rw-r--r--   0        0        0     9043 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/models/flamingo/flamingo_model.py
+-rw-r--r--   0        0        0     5650 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/models/flamingo/loading.py
+-rw-r--r--   0        0        0     2511 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/models/flamingo/modeling.py
+-rw-r--r--   0        0        0     3590 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/models/generation.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/models/llama/__init__.py
+-rw-r--r--   0        0        0     2288 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/models/llama/loading.py
+-rw-r--r--   0        0        0      815 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/models/llama/modeling.py
+-rw-r--r--   0        0        0     2960 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/models/loading.py
+-rw-r--r--   0        0        0     1945 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/models/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/models/moss/__init__.py
+-rw-r--r--   0        0        0     3549 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/models/moss/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/models/pythia/__init__.py
+-rw-r--r--   0        0        0      814 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/models/pythia/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/models/stablelm/__init__.py
+-rw-r--r--   0        0        0     2740 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/models/stablelm/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/models/vicuna/__init__.py
+-rw-r--r--   0        0        0     2064 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/models/vicuna/loading.py
+-rw-r--r--   0        0        0     1573 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/models/vicuna/modeling.py
+-rw-r--r--   0        0        0     3527 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/profile.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/serve/__init__.py
+-rw-r--r--   0        0        0       36 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/serve/executors/__init__.py
+-rw-r--r--   0        0        0     1778 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/serve/executors/base.py
+-rw-r--r--   0        0        0     2376 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/serve/executors/flamingo.py
+-rw-r--r--   0        0        0      171 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/serve/executors/utils.py
+-rw-r--r--   0        0        0     3429 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/serve/gateway.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/serve/playground/__init__.py
+-rw-r--r--   0        0        0     4689 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/serve/playground/gradio.py
+-rw-r--r--   0        0        0     7396 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/serve/playground/gradio_chatbot.py
+-rw-r--r--   0        0        0     2714 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/open_gpt/serve/playground/gradio_css.py
+-rw-r--r--   0        0        0     3073 2023-05-24 07:24:53.202915 open_gpt_torch-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    20671 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.3/PKG-INFO
```

### Comparing `open_gpt_torch-0.0.2/LICENSE` & `open_gpt_torch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.2/README.md` & `open_gpt_torch-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 ![](https://img.shields.io/badge/Made%20with-JinaAI-blueviolet?style=flat)
 [![PyPI](https://img.shields.io/pypi/v/open_gpt_torch)](https://pypi.org/project/open_gpt_torch/)
 [![PyPI - License](https://img.shields.io/pypi/l/open_gpt_torch)](https://pypi.org/project/open_gpt_torch/)
 
 **OpenGPT** is an open-source _cloud-native_ large-scale **_multimodal models_** (LMMs) serving framework. 
 It is designed to simplify the deployment and management of large language models, on a distributed cluster of GPUs.
+We aim to make it a one-stop solution for a centralized and accessible place to gather techniques for optimizing large-scale multimodal models and make them easy to use for everyone.
+
 
 ## Table of contents
 
 - [Features](#features)
 - [Supported models](#supported-models)
 - [Get started](#get-started)
 - [Build a model serving in one line](#build-a-model-serving-in-one-line)
@@ -80,15 +82,17 @@
 ```
 
 ### Quickstart
 
 ```python
 import open_gpt
 
-model = open_gpt.create_model('facebook/llama-7b', device='cuda', precision='fp16')
+model = open_gpt.create_model(
+    'stabilityai/stablelm-tuned-alpha-3b', device='cuda', precision='fp16'
+)
 
 prompt = "The quick brown fox jumps over the lazy dog."
 
 output = model.generate(
     prompt,
     max_length=100,
     temperature=0.9,
@@ -96,42 +100,59 @@
     top_p=0.95,
     repetition_penalty=1.2,
     do_sample=True,
     num_return_sequences=1,
 )
 ```
 
+We use the [stabilityai/stablelm-tuned-alpha-3b](https://huggingface.co/stabilityai/stablelm-tuned-alpha-3b) as the open example model as it is relatively small and fast to download.
+
 > **Warning**
 > In the above example, we use `precision='fp16'` to reduce the memory usage and speed up the inference with some loss in accuracy on text generation tasks. 
 > You can also use `precision='fp32'` instead as you like for better performance. 
 
 > **Note**
 > It usually takes a while (several minutes) for the first time to download and load the model into the memory.
 
 
 In most cases of large model serving, the model cannot fit into a single GPU. To solve this problem, we also provide a `device_map` option (supported by `accecleate` package) to automatically partition the model and distribute it across multiple GPUs:
 
 ```python
 model = open_gpt.create_model(
-    'facebook/llama-7b', precision='fp16', device_map='balanced'
+    'stabilityai/stablelm-tuned-alpha-3b', precision='fp16', device_map='balanced'
 )
 ```
 
-See [examples on how to use opengpt with different models.](./examples)
+In the above example, `device_map="balanced"` evenly split the model on all available GPUs, making it possible for you to serve large models.
+
+> **Note**
+> The `device_map` option is supported by the [accelerate](https://github.com/huggingface/accelerate) package. 
+
+
+See [examples on how to use opengpt with different models.](./examples) 🔥
 
 
 ## Build a model serving in one line
 
 To do so, you can use the `serve` command:
 
 ```bash
-opengpt serve facebook/llama-7b --precision fp16 --port 51000
+opengpt serve stabilityai/stablelm-tuned-alpha-3b --precision fp16 --device_map balanced
 ```
 
-This will start a server on port `51000`. You can then send requests to the server:
+💡 **Tip**: you can inspect the available options with `opengpt serve --help`.
+
+This will start a gRPC and HTTP server listening on port `51000` and `52000` respectively. 
+Once the server is ready, as shown below:
+<details>
+<summary>Click to expand</summary>
+<img src="https://github.com/jina-ai/opengpt/blob/main/.github/images/serve_ready.png" width="600px">
+</details>
+
+You can then send requests to the server:
 
 ```python
 import requests
 
 prompt = "The quick brown fox jumps over the lazy dog."
 
 response = requests.post(
@@ -145,25 +166,49 @@
         "repetition_penalty": 1.2,
         "do_sample": True,
         "num_return_sequences": 1,
     },
 )
 ```
 
-Note that the server will only accept requests from the same machine. If you want to accept requests from other machines, you can use the `--host` flag to specify the host to bind to.
+What's more, we also provide a [Python client](https://github.com/jina-ai/inference-client/) (`inference-client`) for you to easily interact with the server:
+
+```python
+from open_gpt import Client
+
+client = Client()
+
+# connect to the model server
+model = client.get_model(endpoint='grpc://0.0.0.0:51000')
+
+prompt = "The quick brown fox jumps over the lazy dog."
+
+output = model.generate(
+    prompt,
+    max_length=100,
+    temperature=0.9,
+    top_k=50,
+    top_p=0.95,
+    repetition_penalty=1.2,
+    do_sample=True,
+    num_return_sequences=1,
+)
+```
+
+💡 **Tip**: To display the list of available commands, please use the `list` command.
 
 ## Cloud-native deployment
 
 You can also deploy the server to a cloud provider like Jina Cloud or AWS.
 To do so, you can use `deploy` command:
 
 - Jina Cloud
 
 ```bash
-opengpt deploy facebook/llama-7b --device cuda --precision fp16 --provider jina --name opengpt --replicas 2
+opengpt deploy stabilityai/stablelm-tuned-alpha-3b --device cuda --precision fp16 --provider jina --name opengpt --replicas 2
 ```
 
 **TBD ...**
 
 
 ## Contributing
```

#### html2text {}

```diff
@@ -7,71 +7,90 @@
 (https://promptperfect.jina.ai/) & [Stable Diffusion X](https://clipdrop.co/
 stable-diffusion) ![](https://img.shields.io/badge/Made%20with-JinaAI-
 blueviolet?style=flat) [![PyPI](https://img.shields.io/pypi/v/open_gpt_torch)]
 (https://pypi.org/project/open_gpt_torch/) [![PyPI - License](https://
 img.shields.io/pypi/l/open_gpt_torch)](https://pypi.org/project/open_gpt_torch/
 ) **OpenGPT** is an open-source _cloud-native_ large-scale **_multimodal
 models_** (LMMs) serving framework. It is designed to simplify the deployment
-and management of large language models, on a distributed cluster of GPUs. ##
-Table of contents - [Features](#features) - [Supported models](#supported-
-models) - [Get started](#get-started) - [Build a model serving in one line]
-(#build-a-model-serving-in-one-line) - [Cloud-native deployment](#cloud-native-
-deployment) - [Roadmap](#roadmap) ## Features OpenGPT provides the following
-features to make it easy to deploy and serve **large multi-modal models**
-(LMMs) at scale: - Support for multi-modal models on top of large language
-models - Scalable architecture for handling high traffic loads - Optimized for
-low-latency inference - Automatic model partitioning and distribution across
-multiple GPUs - Centralized model management and monitoring - REST API for easy
-integration with existing applications ## Updates - **2023-05-12**: ðWe have
-released the first version `v0.0.1` of OpenGPT. You can install it with `pip
-install open_gpt_torch`. ## Supported Models  OpenGPT supports the following
-models out of the box: - LLM (Large Language Model) - [LLaMA](https://
-ai.facebook.com/blog/large-language-model-llama-meta-ai/): open and efficient
-foundation language models by Meta - [Pythia](https://github.com/EleutherAI/
-pythia): a collection of models developed to facilitate interpretability
-research by EleutherAI - [StableLM](https://github.com/Stability-AI/StableLM):
-series of large language models by Stability AI - [Vicuna](https://
-vicuna.lmsys.org/): a chat assistant fine-tuned from LLaMA on user-shared
-conversations by LMSYS - [MOSS](https://txsun1997.github.io/blogs/moss.html):
-conversational language model from Fudan University - LMM (Large Multi-modal
-Model) - [OpenFlamingo](https://github.com/mlfoundations/open_flamingo): an
-open source version of DeepMind's [Flamingo](https://www.deepmind.com/blog/
-tackling-multiple-tasks-with-a-single-visual-language-model) model - [MiniGPT-
-4](https://minigpt-4.github.io/): aligns a frozen visual encoder with a frozen
-LLM, Vicuna, using just one projection layer. For more details about the
-supported models, please see the [Model Zoo](./MODEL_ZOO.md).  ## Roadmap You
-can view our roadmap with features that are planned, started, and completed on
-the [Roadmap discussion](https://github.com/jina-ai/opengpt/discussions/
-categories/roadmap) category. ## Get Started ### Installation Install the
-package with `pip`: ```bash pip install open_gpt_torch ``` ### Quickstart
-```python import open_gpt model = open_gpt.create_model('facebook/llama-7b',
-device='cuda', precision='fp16') prompt = "The quick brown fox jumps over the
-lazy dog." output = model.generate( prompt, max_length=100, temperature=0.9,
-top_k=50, top_p=0.95, repetition_penalty=1.2, do_sample=True,
-num_return_sequences=1, ) ``` > **Warning** > In the above example, we use
+and management of large language models, on a distributed cluster of GPUs. We
+aim to make it a one-stop solution for a centralized and accessible place to
+gather techniques for optimizing large-scale multimodal models and make them
+easy to use for everyone. ## Table of contents - [Features](#features) -
+[Supported models](#supported-models) - [Get started](#get-started) - [Build a
+model serving in one line](#build-a-model-serving-in-one-line) - [Cloud-native
+deployment](#cloud-native-deployment) - [Roadmap](#roadmap) ## Features OpenGPT
+provides the following features to make it easy to deploy and serve **large
+multi-modal models** (LMMs) at scale: - Support for multi-modal models on top
+of large language models - Scalable architecture for handling high traffic
+loads - Optimized for low-latency inference - Automatic model partitioning and
+distribution across multiple GPUs - Centralized model management and monitoring
+- REST API for easy integration with existing applications ## Updates - **2023-
+05-12**: ðWe have released the first version `v0.0.1` of OpenGPT. You can
+install it with `pip install open_gpt_torch`. ## Supported Models  OpenGPT
+supports the following models out of the box: - LLM (Large Language Model) -
+[LLaMA](https://ai.facebook.com/blog/large-language-model-llama-meta-ai/): open
+and efficient foundation language models by Meta - [Pythia](https://github.com/
+EleutherAI/pythia): a collection of models developed to facilitate
+interpretability research by EleutherAI - [StableLM](https://github.com/
+Stability-AI/StableLM): series of large language models by Stability AI -
+[Vicuna](https://vicuna.lmsys.org/): a chat assistant fine-tuned from LLaMA on
+user-shared conversations by LMSYS - [MOSS](https://txsun1997.github.io/blogs/
+moss.html): conversational language model from Fudan University - LMM (Large
+Multi-modal Model) - [OpenFlamingo](https://github.com/mlfoundations/
+open_flamingo): an open source version of DeepMind's [Flamingo](https://
+www.deepmind.com/blog/tackling-multiple-tasks-with-a-single-visual-language-
+model) model - [MiniGPT-4](https://minigpt-4.github.io/): aligns a frozen
+visual encoder with a frozen LLM, Vicuna, using just one projection layer. For
+more details about the supported models, please see the [Model Zoo](./
+MODEL_ZOO.md).  ## Roadmap You can view our roadmap with features that are
+planned, started, and completed on the [Roadmap discussion](https://github.com/
+jina-ai/opengpt/discussions/categories/roadmap) category. ## Get Started ###
+Installation Install the package with `pip`: ```bash pip install open_gpt_torch
+``` ### Quickstart ```python import open_gpt model = open_gpt.create_model
+( 'stabilityai/stablelm-tuned-alpha-3b', device='cuda', precision='fp16' )
+prompt = "The quick brown fox jumps over the lazy dog." output = model.generate
+( prompt, max_length=100, temperature=0.9, top_k=50, top_p=0.95,
+repetition_penalty=1.2, do_sample=True, num_return_sequences=1, ) ``` We use
+the [stabilityai/stablelm-tuned-alpha-3b](https://huggingface.co/stabilityai/
+stablelm-tuned-alpha-3b) as the open example model as it is relatively small
+and fast to download. > **Warning** > In the above example, we use
 `precision='fp16'` to reduce the memory usage and speed up the inference with
 some loss in accuracy on text generation tasks. > You can also use
 `precision='fp32'` instead as you like for better performance. > **Note** > It
 usually takes a while (several minutes) for the first time to download and load
 the model into the memory. In most cases of large model serving, the model
 cannot fit into a single GPU. To solve this problem, we also provide a
 `device_map` option (supported by `accecleate` package) to automatically
 partition the model and distribute it across multiple GPUs: ```python model =
-open_gpt.create_model( 'facebook/llama-7b', precision='fp16',
-device_map='balanced' ) ``` See [examples on how to use opengpt with different
-models.](./examples) ## Build a model serving in one line To do so, you can use
-the `serve` command: ```bash opengpt serve facebook/llama-7b --precision fp16 -
--port 51000 ``` This will start a server on port `51000`. You can then send
-requests to the server: ```python import requests prompt = "The quick brown fox
-jumps over the lazy dog." response = requests.post( "http://localhost:51000/
-generate", json={ "prompt": prompt, "max_length": 100, "temperature": 0.9,
-"top_k": 50, "top_p": 0.95, "repetition_penalty": 1.2, "do_sample": True,
-"num_return_sequences": 1, }, ) ``` Note that the server will only accept
-requests from the same machine. If you want to accept requests from other
-machines, you can use the `--host` flag to specify the host to bind to. ##
-Cloud-native deployment You can also deploy the server to a cloud provider like
-Jina Cloud or AWS. To do so, you can use `deploy` command: - Jina Cloud ```bash
-opengpt deploy facebook/llama-7b --device cuda --precision fp16 --provider jina
---name opengpt --replicas 2 ``` **TBD ...** ## Contributing We welcome
-contributions from the community! To contribute, please submit a pull request
-following our contributing guidelines. ## License OpenGPT is licensed under the
-Apache License, Version 2.0. See LICENSE for the full license text.
+open_gpt.create_model( 'stabilityai/stablelm-tuned-alpha-3b', precision='fp16',
+device_map='balanced' ) ``` In the above example, `device_map="balanced"`
+evenly split the model on all available GPUs, making it possible for you to
+serve large models. > **Note** > The `device_map` option is supported by the
+[accelerate](https://github.com/huggingface/accelerate) package. See [examples
+on how to use opengpt with different models.](./examples) ð¥ ## Build a model
+serving in one line To do so, you can use the `serve` command: ```bash opengpt
+serve stabilityai/stablelm-tuned-alpha-3b --precision fp16 --device_map
+balanced ``` ð¡ **Tip**: you can inspect the available options with `opengpt
+serve --help`. This will start a gRPC and HTTP server listening on port `51000`
+and `52000` respectively. Once the server is ready, as shown below:  Click to
+expand [https://github.com/jina-ai/opengpt/blob/main/.github/images/
+serve_ready.png]  You can then send requests to the server: ```python import
+requests prompt = "The quick brown fox jumps over the lazy dog." response =
+requests.post( "http://localhost:51000/generate", json={ "prompt": prompt,
+"max_length": 100, "temperature": 0.9, "top_k": 50, "top_p": 0.95,
+"repetition_penalty": 1.2, "do_sample": True, "num_return_sequences": 1, }, )
+``` What's more, we also provide a [Python client](https://github.com/jina-ai/
+inference-client/) (`inference-client`) for you to easily interact with the
+server: ```python from open_gpt import Client client = Client() # connect to
+the model server model = client.get_model(endpoint='grpc://0.0.0.0:51000')
+prompt = "The quick brown fox jumps over the lazy dog." output = model.generate
+( prompt, max_length=100, temperature=0.9, top_k=50, top_p=0.95,
+repetition_penalty=1.2, do_sample=True, num_return_sequences=1, ) ``` ð¡
+**Tip**: To display the list of available commands, please use the `list`
+command. ## Cloud-native deployment You can also deploy the server to a cloud
+provider like Jina Cloud or AWS. To do so, you can use `deploy` command: - Jina
+Cloud ```bash opengpt deploy stabilityai/stablelm-tuned-alpha-3b --device cuda
+--precision fp16 --provider jina --name opengpt --replicas 2 ``` **TBD ...** ##
+Contributing We welcome contributions from the community! To contribute, please
+submit a pull request following our contributing guidelines. ## License OpenGPT
+is licensed under the Apache License, Version 2.0. See LICENSE for the full
+license text.
```

### Comparing `open_gpt_torch-0.0.2/open_gpt/__init__.py` & `open_gpt_torch-0.0.3/open_gpt/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,8 +30,12 @@
     :return: The version number.
     """
     return importlib_metadata.version(__package__ + '_torch')
 
 
 __version__ = get_version()
 
+_os.environ['NO_VERSION_CHECK'] = '1'
+
+from inference_client import Client
+
 from .factory import create_model
```

### Comparing `open_gpt_torch-0.0.2/open_gpt/cli/application.py` & `open_gpt_torch-0.0.3/open_gpt/cli/application.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.2/open_gpt/cli/commands/about.py` & `open_gpt_torch-0.0.3/open_gpt/cli/commands/about.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.2/open_gpt/cli/commands/playground.py` & `open_gpt_torch-0.0.3/open_gpt/cli/commands/playground.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.2/open_gpt/factory.py` & `open_gpt_torch-0.0.3/open_gpt/factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from typing import List, Optional, Union
 
 import torch
 
 
 def create_model(
     model_name: str,
-    precision: Optional[str] = None,
+    precision: str = 'fp32',
     device: Optional[Union[str, torch.device]] = None,
     device_map: Optional[Union[str, List[int]]] = None,
     **kwargs,
 ):
     """Create a model.
 
     :param model_name: The name of the model to create.
-    :param precision: The precision to use. Can be one of ``"float16"``, ``"float32"``, ``"float64"``, ``"bfloat16"``, ``"mixed"`` or ``None``.
+    :param precision: The precision to use for the model. Can be one of ``"fp16"``, ``"fp32"`` or ``"int8"``. Defaults to ``"fp32"``.
     :param device: The device to use. Can be one of ``"cpu"``, ``"cuda"``, ``"cuda:X"`` or ``None``.
     :param device_map: The device map to use. Can be one of ``"balanced"``, ``"single"`` or a list of device IDs.
     :param kwargs: Additional keyword arguments to pass to the model.
     """
 
     if model_name.startswith('facebook/llama') or model_name.startswith(
         'decapoda-research/llama'
@@ -96,27 +96,45 @@
             precision=precision,
             device_map=device_map,
             **kwargs,
         )
 
 
 def create_flow(
-    model_name_or_path: str, protocol='http', port=51000, replicas: int = 1
+    model_name_or_path: str,
+    grpc_port: int = 51001,
+    http_port: int = 51002,
+    cors: bool = False,
+    uses_with: Optional[dict] = {},
+    replicas: int = 1,
 ):
     from jina import Flow
 
     if 'flamingo' in model_name_or_path:
         from .serve.executors.flamingo import FlamingoExecutor as Executor
     else:
-        from serve.executors import CausualLMExecutor as Executor
+        from .serve.executors import CausualLMExecutor as Executor
+
+    from .serve.gateway import Gateway
 
     # normalize the model name to be used as flow executor name
     norm_name = model_name_or_path.split('/')[-1]
-    norm_name = norm_name.replace('-', '_').lower()
+    norm_name = norm_name.replace('-', '_').replace('.', '_').lower()
+
+    uses_with['model_name_or_path'] = model_name_or_path
 
-    return Flow(protocol=protocol, port=port, cors=True).add(
-        uses=Executor,
-        uses_with={'model_name_or_path': model_name_or_path},
-        name=f'{norm_name}_executor',
-        replicas=replicas,
-        timeout_ready=-1,
+    return (
+        Flow()
+        .config_gateway(
+            uses=Gateway,
+            port=[grpc_port, http_port],
+            protocol=['grpc', 'http'],
+            cors=cors,
+        )
+        .add(
+            uses=Executor,
+            uses_with=uses_with,
+            name=f'{norm_name}_executor',
+            replicas=replicas,
+            timeout_ready=-1,
+        )
     )
```

### Comparing `open_gpt_torch-0.0.2/open_gpt/helper.py` & `open_gpt_torch-0.0.3/open_gpt/helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,34 +6,33 @@
 import torch
 import torch.backends.cudnn as cudnn
 import torch.distributed as dist
 
 _PRECISION_TO_DTYPE = {
     'fp16': torch.float16,
     'fp32': torch.float32,
-    'int8': torch.int8,
-    'torch.float32': torch.float32,
-    'torch.float16': torch.float16,
-    'torch.int8': torch.int8,
+    'int8': torch.float16,
+    'float32': torch.float32,
+    'float16': torch.float16,
 }
 
 _DEFAULT_DTYPE = torch.float32
 
 
 def cast_torch_dtype(precision: Union[str, 'torch.dtype']):
     assert precision is not None
     if isinstance(precision, str):
-        return _PRECISION_TO_DTYPE.get(precision, precision)
+        return _PRECISION_TO_DTYPE.get(precision)
     elif isinstance(precision, torch.dtype):
         return precision
     else:
         return ValueError(f'Invalid precision: {precision}')
 
 
-def cast_precision(dtype: Optional[Union[str, 'torch.dtype']]):
+def cast_to_precision(dtype: Optional[Union[str, 'torch.dtype']]) -> str:
     if isinstance(dtype, str):
         return dtype
     elif dtype == torch.float32:
         return 'fp32'
     elif dtype == torch.float16:
         return 'fp16'
     elif dtype == torch.int8:
```

### Comparing `open_gpt_torch-0.0.2/open_gpt/models/flamingo/flamingo_lm.py` & `open_gpt_torch-0.0.3/open_gpt/models/flamingo/flamingo_lm.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.2/open_gpt/models/flamingo/flamingo_model.py` & `open_gpt_torch-0.0.3/open_gpt/models/flamingo/flamingo_model.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.2/open_gpt/models/flamingo/loading.py` & `open_gpt_torch-0.0.3/open_gpt/models/flamingo/loading.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,25 +26,25 @@
     :param lang_model_name_or_path: The name or path of the language model to use.
     :param tokenizer_name_or_path: The name or path of the tokenizer to use. If not specified, the tokenizer associated with the model will be used.
     :param decoder_layers_attr_name: The name of the attribute that specifies the decoder layers.
     :param device: The device to load the model on.
     :param dtype: The dtype to load the model with.
     """
 
-    from ...helper import cast_precision
+    from ...helper import cast_to_precision
     from ..loading import load_model_and_tokenizer as load_llama_model_and_tokenizer
     from .flamingo_lm import FlamingoLMMixin
     from .flamingo_model import FlamingoLMModel
 
     assert (
         device_map is None
     ), f"`device_map={device_map}` is not supported for Flamingo models"
 
     # load the vision model
-    precision = cast_precision(dtype)
+    precision = cast_to_precision(dtype)
     model_name, *pretrained = vision_model_name_or_path.split("::")
     pretrained = pretrained[0] if len(pretrained) == 1 else 'openai'
     clip_model, _, image_processor = open_clip.create_model_and_transforms(
         model_name, pretrained=pretrained, device=device, precision=precision
     )
     # set the vision encoder to output the visual features
     clip_model.visual.output_tokens = True
```

### Comparing `open_gpt_torch-0.0.2/open_gpt/models/flamingo/modeling.py` & `open_gpt_torch-0.0.3/open_gpt/models/flamingo/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.2/open_gpt/models/generation.py` & `open_gpt_torch-0.0.3/open_gpt/models/generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import dataclasses
 from typing import TYPE_CHECKING, List, Optional, Union, overload
 
 import torch
-from transformers import GenerationConfig
 
 if TYPE_CHECKING:
     from transformers import AutoModelForCausalLM, AutoTokenizer
 
 
 class GenerationMixin:
     """Mixin for generation methods."""
@@ -50,22 +49,17 @@
         :param no_repeat_ngram_size: If set to int > 0, all ngrams of that size can only occur once.
         """
         ...
 
     def generate(self, prompts: Union[str, List[str]], **kwargs):
         inputs = self.tokenizer(
             [prompts] if isinstance(prompts, str) else prompts,
-            padding=True,
+            padding='longest',
             return_tensors="pt",
-        )
-
-        # Move inputs to the correct device
-        for k, v in inputs.items():
-            if isinstance(v, torch.Tensor):
-                inputs[k] = v.to(self._device)
+        ).to(self._device)
 
         # overwrite default values with kwargs
         clean_up_tokenization_spaces = kwargs.pop('clean_up_tokenization_spaces', True)
         skip_special_tokens = kwargs.pop("skip_special_tokens", True)
 
         with torch.inference_mode():
             outputs = self.model.generate(**inputs, **kwargs)
```

### Comparing `open_gpt_torch-0.0.2/open_gpt/models/loading.py` & `open_gpt_torch-0.0.3/open_gpt/models/llama/loading.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,72 +1,69 @@
 from typing import List, Optional, Union
 
 import torch
-from loguru import logger
 
-from open_gpt.helper import auto_dtype_and_device
+from open_gpt.logging import logger
 
 
 def load_model_and_tokenizer(
     model_name_or_path: str,
     tokenizer_name_or_path: Optional[str] = None,
     device: Optional[torch.device] = None,
-    dtype: Optional[Union[str, torch.dtype]] = None,
+    precision: Optional[str] = None,
+    dtype: Optional[torch.dtype] = None,
     device_map: Optional[Union[str, List[int]]] = None,
     no_split_module_classes: Optional[List[str]] = None,
     **kwargs,
 ):
     """Load a model and tokenizer from HuggingFace."""
     import os
 
-    from transformers import AutoConfig, AutoModelForCausalLM, AutoTokenizer
+    from transformers import AutoConfig, AutoModelForCausalLM
+    from transformers.models.llama.tokenization_llama import LlamaTokenizer
 
-    dtype, device = auto_dtype_and_device(dtype, device)
-
-    tokenizer = AutoTokenizer.from_pretrained(
-        tokenizer_name_or_path or model_name_or_path, trust_remote_code=True
+    tokenizer = LlamaTokenizer.from_pretrained(
+        model_name_or_path or tokenizer_name_or_path
     )
 
     if tokenizer.pad_token is None:
         # Issue: GPT models don't have a pad token
         # tokenizer.add_special_tokens({"pad_token": "<PAD>"})
-        tokenizer.pad_token = tokenizer.eos_token
-        tokenizer.pad_token_id = tokenizer.eos_token_id
+        tokenizer.pad_token = tokenizer.unk_token
+        tokenizer.pad_token_id = tokenizer.unk_token_id
 
     # For generation padding tokens should be on the left
     tokenizer.padding_side = "left"
 
+    logger.info(f"Loading llama base model from {model_name_or_path}")
     if device_map:
         import huggingface_hub
         from accelerate import init_empty_weights, load_checkpoint_and_dispatch
 
         if not os.path.exists(model_name_or_path):
             model_path = huggingface_hub.snapshot_download(model_name_or_path)
         else:
             model_path = model_name_or_path
 
-        config = AutoConfig.from_pretrained(model_name_or_path, trust_remote_code=True)
         with init_empty_weights():
+            config = AutoConfig.from_pretrained(model_path, trust_remote_code=True)
             model = AutoModelForCausalLM.from_config(
                 config, torch_dtype=dtype, trust_remote_code=True
             )
-            # make sure token embedding weights are still tied if needed
-            model.tie_weights()
 
-            model = load_checkpoint_and_dispatch(
-                model,
-                model_path,
-                device_map=device_map,
-                no_split_module_classes=no_split_module_classes,
-                dtype=dtype,
-            )
+        # make sure token embedding weights are still tied if needed
+        model.tie_weights()
+
+        model = load_checkpoint_and_dispatch(
+            model,
+            model_path,
+            device_map=device_map,
+            no_split_module_classes=no_split_module_classes,
+            dtype=dtype,
+        )
     else:
         model = AutoModelForCausalLM.from_pretrained(
             model_name_or_path, torch_dtype=dtype, trust_remote_code=True
         )
         model.to(device)
 
-    if hasattr(model, 'generation_config'):
-        # set pad_token_id to eos_token_id because GPT does not have a PAD token
-        model.generation_config.pad_token_id = model.generation_config.eos_token_id
-
     return model, tokenizer
```

### Comparing `open_gpt_torch-0.0.2/open_gpt/models/modeling.py` & `open_gpt_torch-0.0.3/open_gpt/models/modeling.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import TYPE_CHECKING, List, Optional, Union
 
 import torch
 from torch import nn
 
 from ..helper import auto_dtype_and_device
-from ..logging import logger
 from .generation import GenerationMixin
 
 if TYPE_CHECKING:
     from transformers import AutoModelForCausalLM, AutoTokenizer
 
 
 class BaseModel(nn.Module, GenerationMixin):
@@ -16,33 +15,30 @@
     tokenizer: 'AutoTokenizer'
     no_split_module_classes: List[str] = None
 
     def __init__(
         self,
         model_name_or_path: str,
         tokenizer_name_or_path: Optional[str] = None,
-        dtype: Optional[Union[str, torch.dtype]] = None,
+        precision: str = 'fp32',
         device: Optional[torch.device] = None,
         device_map: Optional[Union[str, List[int]]] = None,
         eval_mode: bool = True,
         **kwargs,
     ):
         """Create a model of the given name."""
 
         super().__init__()
 
         self._model_name_or_path = model_name_or_path
 
-        self._dtype, self._device = auto_dtype_and_device(dtype, device)
+        self._precision = precision
+        self._dtype, self._device = auto_dtype_and_device(precision, device)
 
         self._device_map = device_map
-        if not self._device_map:
-            logger.warning(
-                f'To turn on tensor parallelism, set `device_map` to a list of GPU ids rather than `None`'
-            )
 
         self._eval_mode = eval_mode
 
         self.load_model_and_transforms(
             model_name_or_path, tokenizer_name_or_path=tokenizer_name_or_path
         )
 
@@ -52,14 +48,15 @@
         self, model_name_or_path: str, tokenizer_name_or_path: Optional[str] = None
     ):
         from .loading import load_model_and_tokenizer
 
         self.model, self.tokenizer = load_model_and_tokenizer(
             model_name_or_path,
             tokenizer_name_or_path=tokenizer_name_or_path,
+            precision=self._precision,
             dtype=self._dtype,
             device=self._device,
             device_map=self._device_map,
             no_split_module_classes=self.no_split_module_classes,
         )
 
         # turn the eval mode off `eval_mode=False` in training
```

### Comparing `open_gpt_torch-0.0.2/open_gpt/models/moss/modeling.py` & `open_gpt_torch-0.0.3/open_gpt/models/moss/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.2/open_gpt/models/pythia/modeling.py` & `open_gpt_torch-0.0.3/open_gpt/models/pythia/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.2/open_gpt/models/stablelm/modeling.py` & `open_gpt_torch-0.0.3/open_gpt/models/stablelm/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.2/open_gpt/models/vicuna/loading.py` & `open_gpt_torch-0.0.3/open_gpt/models/loading.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,95 +1,87 @@
 from typing import List, Optional, Union
 
 import torch
-from tqdm import tqdm
 
-from open_gpt.helper import auto_dtype_and_device
-from open_gpt.logging import logger
+from ..logging import logger
 
 
 def load_model_and_tokenizer(
     model_name_or_path: str,
     tokenizer_name_or_path: Optional[str] = None,
     device: Optional[torch.device] = None,
-    dtype: Optional[Union[str, torch.dtype]] = None,
+    precision: Optional[str] = None,
+    dtype: Optional[torch.dtype] = None,
     device_map: Optional[Union[str, List[int]]] = None,
     no_split_module_classes: Optional[List[str]] = None,
     **kwargs,
 ):
     """Load a model and tokenizer from HuggingFace."""
     import os
 
     from transformers import AutoConfig, AutoModelForCausalLM, AutoTokenizer
 
-    dtype, device = auto_dtype_and_device(dtype, device)
-
-    model_size = model_name_or_path.split('-')[-3]
-
-    facebook_llama_model_name_or_path = f"facebook/llama-{model_size}"
-    if os.path.exists(facebook_llama_model_name_or_path):
-        llama_model_name_or_path = facebook_llama_model_name_or_path
-    else:
-        llama_model_name_or_path = f"decapoda-research/llama-{model_size}-hf"
-
     tokenizer = AutoTokenizer.from_pretrained(
-        model_name_or_path or tokenizer_name_or_path, trust_remote_code=True
+        tokenizer_name_or_path or model_name_or_path, trust_remote_code=True
     )
 
     if tokenizer.pad_token is None:
         # Issue: GPT models don't have a pad token
-        # tokenizer.add_special_tokens({"pad_token": "<PAD>"})
-        tokenizer.pad_token = tokenizer.eos_token
-        tokenizer.pad_token_id = tokenizer.eos_token_id
+        tokenizer.pad_token = tokenizer.unk_token
+        tokenizer.pad_token_id = tokenizer.unk_token_id
 
     # For generation padding tokens should be on the left
     tokenizer.padding_side = "left"
 
-    logger.info(
-        f"Loading llama-{model_size} base model from {llama_model_name_or_path}"
-    )
     if device_map:
         import huggingface_hub
         from accelerate import init_empty_weights, load_checkpoint_and_dispatch
 
-        if not os.path.exists(llama_model_name_or_path):
-            model_path = huggingface_hub.snapshot_download(llama_model_name_or_path)
+        if not os.path.exists(model_name_or_path):
+            model_path = huggingface_hub.snapshot_download(model_name_or_path)
         else:
-            model_path = llama_model_name_or_path
+            model_path = model_name_or_path
 
+        config = AutoConfig.from_pretrained(model_name_or_path, trust_remote_code=True)
         with init_empty_weights():
-            config = AutoConfig.from_pretrained(
-                llama_model_name_or_path, trust_remote_code=True
-            )
             model = AutoModelForCausalLM.from_config(
                 config, torch_dtype=dtype, trust_remote_code=True
             )
             # make sure token embedding weights are still tied if needed
             model.tie_weights()
 
-            model = load_checkpoint_and_dispatch(
-                model,
-                model_path,
-                device_map=device_map,
-                no_split_module_classes=no_split_module_classes,
-                dtype=dtype,
+        if precision == 'bit8':
+            from jina.importer import ImportExtensions
+
+            with ImportExtensions(required=True):
+                import bitsandbytes as bnb
+
+            from transformers.utils.bitsandbytes import replace_8bit_linear
+
+            model = replace_8bit_linear(
+                model, threshold=6.0, modules_to_not_convert=["lm_head", "embed_out"]
             )
+
+            # For some reason replace_8bit_linear creates parameters with requires_grad=True but it's irrelevant rn
+            for p in model.parameters():
+                p.requires_grad = False
+
+        model = load_checkpoint_and_dispatch(
+            model,
+            model_path,
+            device_map=device_map,
+            no_split_module_classes=no_split_module_classes,
+            dtype=dtype if precision != 'bit8' else None,
+        )
     else:
+        logger.warning(
+            f'To turn on tensor parallelism, set `device_map` to a list of GPU ids rather than `None`'
+        )
         model = AutoModelForCausalLM.from_pretrained(
-            llama_model_name_or_path, torch_dtype=dtype, trust_remote_code=True
+            model_name_or_path,
+            torch_dtype=dtype,
+            load_in_8bit=precision == 'bit8',
+            trust_remote_code=True,
         )
         model.to(device)
 
-    logger.info(f"Loading model weights delta from {model_name_or_path}")
-    delta = AutoModelForCausalLM.from_pretrained(
-        model_name_or_path, torch_dtype=torch.float16, low_cpu_mem_usage=True
-    )
-    # adapted from `fastchat.model.apply_delta`
-    for name, param in tqdm(model.state_dict().items(), desc="Applying delta"):
-        assert name in delta.state_dict()
-        param.data += delta.state_dict()[name].to(param.dtype).to(param.device)
-
-    # clean up delta to save memory
-    delta = None
-    torch.cuda.empty_cache()
-
     return model, tokenizer
```

### Comparing `open_gpt_torch-0.0.2/open_gpt/models/vicuna/modeling.py` & `open_gpt_torch-0.0.3/open_gpt/models/vicuna/modeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,13 +43,14 @@
 
         from .loading import load_model_and_tokenizer
 
         self.model, self.tokenizer = load_model_and_tokenizer(
             model_name_or_path,
             tokenizer_name_or_path=tokenizer_name_or_path,
             dtype=self._dtype,
+            precision=self._precision,
             device=self._device,
             device_map=self._device_map,
             no_split_module_classes=self.no_split_module_classes,
         )
 
         self.model.eval()
```

### Comparing `open_gpt_torch-0.0.2/open_gpt/profile.py` & `open_gpt_torch-0.0.3/open_gpt/profile.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,14 +15,37 @@
 
 KB = 1 << 10
 MB = 1 << 20
 GB = 1 << 30
 T = 1e12
 
 
+def cpu_mem_stats():
+    objects = gc.get_objects()
+    tensors = [obj for obj in objects if torch.is_tensor(obj) and not obj.is_cuda]
+
+    total_numel = 0
+    total_mem = 0
+    visited_data = set()
+    for tensor in tensors:
+        # a data_ptr indicates a memory block allocated
+        data_ptr = tensor.storage().data_ptr()
+        if data_ptr in visited_data:
+            continue
+        visited_data.add(data_ptr)
+
+        numel = tensor.numel()
+        total_numel += numel
+        element_size = tensor.storage().element_size()
+        mem = numel * element_size
+        total_mem += mem
+
+    return total_mem
+
+
 def compute_module_sizes(model):
     return _compute_module_sizes(model)
 
 
 class PeakCPUMemory:
     def __init__(self):
         self.process = psutil.Process()
```

### Comparing `open_gpt_torch-0.0.2/open_gpt/serve/executors/base.py` & `open_gpt_torch-0.0.3/open_gpt/serve/executors/base.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.2/open_gpt/serve/executors/flamingo.py` & `open_gpt_torch-0.0.3/open_gpt/serve/executors/flamingo.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,16 +27,23 @@
             model_name_or_path
         ), '`model_name_or_path` must be provided to initialize the model and tokenizer.'
 
         self._model_name_or_path = model_name_or_path
         self._minibatch_size = minibatch_size
         self._thread_pool = ThreadPool(processes=num_workers)
 
+        # IMPORTANT: flamingo does not allow device_map to be set
+        # self._device_map = device_map
+        if device_map:
+            logger.warning(
+                '`device_map` is not supported in FlamingoExecutor. Ignored.'
+            )
+
         self.model = open_gpt.create_model(
-            model_name_or_path, precision=precision, device_map=device_map, **kwargs
+            model_name_or_path, precision=precision, device_map=None, **kwargs
         )
 
         # warmup the model to avoid the first-time slowness
         # self.model.generate(['Hello world!'])
 
     @requests(on='/generate')
     def generate(self, docs: 'DocumentArray', parameters: Dict = {}, **kwargs):
```

### Comparing `open_gpt_torch-0.0.2/open_gpt/serve/playground/gradio.py` & `open_gpt_torch-0.0.3/open_gpt/serve/playground/gradio.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.2/open_gpt/serve/playground/gradio_chatbot.py` & `open_gpt_torch-0.0.3/open_gpt/serve/playground/gradio_chatbot.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.2/open_gpt/serve/playground/gradio_css.py` & `open_gpt_torch-0.0.3/open_gpt/serve/playground/gradio_css.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.2/pyproject.toml` & `open_gpt_torch-0.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "open_gpt_torch"
-version = "0.0.2"
+version = "0.0.3"
 description = "An open-source cloud-native of large multi-modal models (LMMs) serving framework."
 
 license = "Apache-2.0"
 
 authors = [
     "Jina AI <hello@jina.ai>"
 ]
@@ -42,24 +42,26 @@
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 # Compatible Python versions
 python = ">=3.8,<4.0"
-# torch = {version = "<2.0.0+cu116", source="torch_cuda"} # a meta device requires torch >= 1.9.0
 jina = "^3.15.0"
 docarray = "^0.21.0"
+inference-client = "^0.0.4"
+pydantic = "^1.10.0"
 loguru = "^0.5"
 cleo = "^2.0.0"
 click = "^8.1.3"
 numpy = "^1.21.2"
 einops = "^0.6.0"
 transformers = "^4.28.0"
 open_clip_torch = "^2.16"
+bitsandbytes = "^0.38.0"
 accelerate = "^0.18.0"
 tqdm = "^4.62.3"
 
 # A list of all of the optional dependencies, some of which are included in the
 # below `extras`. They can be opted into by apps.
 open-flamingo = { version = "^0.0", optional = true }
 gradio = { version = "^3.30.0", optional = true }
```

### Comparing `open_gpt_torch-0.0.2/PKG-INFO` & `open_gpt_torch-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-gpt-torch
-Version: 0.0.2
+Version: 0.0.3
 Summary: An open-source cloud-native of large multi-modal models (LMMs) serving framework.
 Home-page: https://github.com/jina-ai/opengpt
 License: Apache-2.0
 Keywords: Pytorch,LMM,GPT,LLM,multi-modality,cloud-native,model-serving,model-inference,llama,vicuna,stabellm
 Author: Jina AI
 Author-email: hello@jina.ai
 Requires-Python: >=3.8,<4.0
@@ -14,40 +14,38 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: flamingo
 Provides-Extra: playground
 Requires-Dist: accelerate (>=0.18.0,<0.19.0)
+Requires-Dist: bitsandbytes (>=0.38.0,<0.39.0)
 Requires-Dist: cleo (>=2.0.0,<3.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: docarray (>=0.21.0,<0.22.0)
 Requires-Dist: einops (>=0.6.0,<0.7.0)
 Requires-Dist: gradio (>=3.30.0,<4.0.0) ; extra == "playground"
+Requires-Dist: inference-client (>=0.0.4,<0.0.5)
 Requires-Dist: jina (>=3.15.0,<4.0.0)
 Requires-Dist: loguru (>=0.5,<0.6)
 Requires-Dist: markdown2 (>=2.4.0,<3.0.0) ; extra == "playground"
 Requires-Dist: mdtex2html (>=1.2.0,<2.0.0) ; extra == "playground"
 Requires-Dist: numpy (>=1.21.2,<2.0.0)
 Requires-Dist: open-flamingo (>=0.0,<0.1) ; extra == "flamingo"
 Requires-Dist: open_clip_torch (>=2.16,<3.0)
+Requires-Dist: pydantic (>=1.10.0,<2.0.0)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Requires-Dist: transformers (>=4.28.0,<5.0.0)
 Project-URL: Repository, https://github.com/jina-ai/opengpt
 Description-Content-Type: text/markdown
 
 # ☄️ OpenGPT
 
@@ -63,14 +61,16 @@
 
 ![](https://img.shields.io/badge/Made%20with-JinaAI-blueviolet?style=flat)
 [![PyPI](https://img.shields.io/pypi/v/open_gpt_torch)](https://pypi.org/project/open_gpt_torch/)
 [![PyPI - License](https://img.shields.io/pypi/l/open_gpt_torch)](https://pypi.org/project/open_gpt_torch/)
 
 **OpenGPT** is an open-source _cloud-native_ large-scale **_multimodal models_** (LMMs) serving framework. 
 It is designed to simplify the deployment and management of large language models, on a distributed cluster of GPUs.
+We aim to make it a one-stop solution for a centralized and accessible place to gather techniques for optimizing large-scale multimodal models and make them easy to use for everyone.
+
 
 ## Table of contents
 
 - [Features](#features)
 - [Supported models](#supported-models)
 - [Get started](#get-started)
 - [Build a model serving in one line](#build-a-model-serving-in-one-line)
@@ -131,15 +131,17 @@
 ```
 
 ### Quickstart
 
 ```python
 import open_gpt
 
-model = open_gpt.create_model('facebook/llama-7b', device='cuda', precision='fp16')
+model = open_gpt.create_model(
+    'stabilityai/stablelm-tuned-alpha-3b', device='cuda', precision='fp16'
+)
 
 prompt = "The quick brown fox jumps over the lazy dog."
 
 output = model.generate(
     prompt,
     max_length=100,
     temperature=0.9,
@@ -147,42 +149,59 @@
     top_p=0.95,
     repetition_penalty=1.2,
     do_sample=True,
     num_return_sequences=1,
 )
 ```
 
+We use the [stabilityai/stablelm-tuned-alpha-3b](https://huggingface.co/stabilityai/stablelm-tuned-alpha-3b) as the open example model as it is relatively small and fast to download.
+
 > **Warning**
 > In the above example, we use `precision='fp16'` to reduce the memory usage and speed up the inference with some loss in accuracy on text generation tasks. 
 > You can also use `precision='fp32'` instead as you like for better performance. 
 
 > **Note**
 > It usually takes a while (several minutes) for the first time to download and load the model into the memory.
 
 
 In most cases of large model serving, the model cannot fit into a single GPU. To solve this problem, we also provide a `device_map` option (supported by `accecleate` package) to automatically partition the model and distribute it across multiple GPUs:
 
 ```python
 model = open_gpt.create_model(
-    'facebook/llama-7b', precision='fp16', device_map='balanced'
+    'stabilityai/stablelm-tuned-alpha-3b', precision='fp16', device_map='balanced'
 )
 ```
 
-See [examples on how to use opengpt with different models.](./examples)
+In the above example, `device_map="balanced"` evenly split the model on all available GPUs, making it possible for you to serve large models.
+
+> **Note**
+> The `device_map` option is supported by the [accelerate](https://github.com/huggingface/accelerate) package. 
+
+
+See [examples on how to use opengpt with different models.](./examples) 🔥
 
 
 ## Build a model serving in one line
 
 To do so, you can use the `serve` command:
 
 ```bash
-opengpt serve facebook/llama-7b --precision fp16 --port 51000
+opengpt serve stabilityai/stablelm-tuned-alpha-3b --precision fp16 --device_map balanced
 ```
 
-This will start a server on port `51000`. You can then send requests to the server:
+💡 **Tip**: you can inspect the available options with `opengpt serve --help`.
+
+This will start a gRPC and HTTP server listening on port `51000` and `52000` respectively. 
+Once the server is ready, as shown below:
+<details>
+<summary>Click to expand</summary>
+<img src="https://github.com/jina-ai/opengpt/blob/main/.github/images/serve_ready.png" width="600px">
+</details>
+
+You can then send requests to the server:
 
 ```python
 import requests
 
 prompt = "The quick brown fox jumps over the lazy dog."
 
 response = requests.post(
@@ -196,25 +215,49 @@
         "repetition_penalty": 1.2,
         "do_sample": True,
         "num_return_sequences": 1,
     },
 )
 ```
 
-Note that the server will only accept requests from the same machine. If you want to accept requests from other machines, you can use the `--host` flag to specify the host to bind to.
+What's more, we also provide a [Python client](https://github.com/jina-ai/inference-client/) (`inference-client`) for you to easily interact with the server:
+
+```python
+from open_gpt import Client
+
+client = Client()
+
+# connect to the model server
+model = client.get_model(endpoint='grpc://0.0.0.0:51000')
+
+prompt = "The quick brown fox jumps over the lazy dog."
+
+output = model.generate(
+    prompt,
+    max_length=100,
+    temperature=0.9,
+    top_k=50,
+    top_p=0.95,
+    repetition_penalty=1.2,
+    do_sample=True,
+    num_return_sequences=1,
+)
+```
+
+💡 **Tip**: To display the list of available commands, please use the `list` command.
 
 ## Cloud-native deployment
 
 You can also deploy the server to a cloud provider like Jina Cloud or AWS.
 To do so, you can use `deploy` command:
 
 - Jina Cloud
 
 ```bash
-opengpt deploy facebook/llama-7b --device cuda --precision fp16 --provider jina --name opengpt --replicas 2
+opengpt deploy stabilityai/stablelm-tuned-alpha-3b --device cuda --precision fp16 --provider jina --name opengpt --replicas 2
 ```
 
 **TBD ...**
 
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,235 +1,251 @@
-Metadata-Version: 2.1 Name: open-gpt-torch Version: 0.0.2 Summary: An open-
+Metadata-Version: 2.1 Name: open-gpt-torch Version: 0.0.3 Summary: An open-
 source cloud-native of large multi-modal models (LMMs) serving framework. Home-
 page: https://github.com/jina-ai/opengpt License: Apache-2.0 Keywords:
 Pytorch,LMM,GPT,LLM,multi-modality,cloud-native,model-serving,model-
 inference,llama,vicuna,stabellm Author: Jina AI Author-email: hello@jina.ai
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
-Scientific/Engineering :: Mathematics Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Provides-Extra: flamingo
-Provides-Extra: playground Requires-Dist: accelerate (>=0.18.0,<0.19.0)
-Requires-Dist: cleo (>=2.0.0,<3.0.0) Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: docarray (>=0.21.0,<0.22.0) Requires-Dist: einops
-(>=0.6.0,<0.7.0) Requires-Dist: gradio (>=3.30.0,<4.0.0) ; extra ==
-"playground" Requires-Dist: jina (>=3.15.0,<4.0.0) Requires-Dist: loguru
-(>=0.5,<0.6) Requires-Dist: markdown2 (>=2.4.0,<3.0.0) ; extra == "playground"
-Requires-Dist: mdtex2html (>=1.2.0,<2.0.0) ; extra == "playground" Requires-
-Dist: numpy (>=1.21.2,<2.0.0) Requires-Dist: open-flamingo (>=0.0,<0.1) ; extra
-== "flamingo" Requires-Dist: open_clip_torch (>=2.16,<3.0) Requires-Dist: tqdm
-(>=4.62.3,<5.0.0) Requires-Dist: transformers (>=4.28.0,<5.0.0) Project-URL:
-Repository, https://github.com/jina-ai/opengpt Description-Content-Type: text/
-markdown # âï¸ OpenGPT
+Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Scientific/Engineering ::
+Mathematics Classifier: Topic :: Software Development Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Provides-Extra: flamingo Provides-Extra: playground
+Requires-Dist: accelerate (>=0.18.0,<0.19.0) Requires-Dist: bitsandbytes
+(>=0.38.0,<0.39.0) Requires-Dist: cleo (>=2.0.0,<3.0.0) Requires-Dist: click
+(>=8.1.3,<9.0.0) Requires-Dist: docarray (>=0.21.0,<0.22.0) Requires-Dist:
+einops (>=0.6.0,<0.7.0) Requires-Dist: gradio (>=3.30.0,<4.0.0) ; extra ==
+"playground" Requires-Dist: inference-client (>=0.0.4,<0.0.5) Requires-Dist:
+jina (>=3.15.0,<4.0.0) Requires-Dist: loguru (>=0.5,<0.6) Requires-Dist:
+markdown2 (>=2.4.0,<3.0.0) ; extra == "playground" Requires-Dist: mdtex2html
+(>=1.2.0,<2.0.0) ; extra == "playground" Requires-Dist: numpy (>=1.21.2,<2.0.0)
+Requires-Dist: open-flamingo (>=0.0,<0.1) ; extra == "flamingo" Requires-Dist:
+open_clip_torch (>=2.16,<3.0) Requires-Dist: pydantic (>=1.10.0,<2.0.0)
+Requires-Dist: tqdm (>=4.62.3,<5.0.0) Requires-Dist: transformers
+(>=4.28.0,<5.0.0) Project-URL: Repository, https://github.com/jina-ai/opengpt
+Description-Content-Type: text/markdown # âï¸ OpenGPT
   [OpenGPT:_An_open-source_cloud-native_large-scale_multimodal_model_serving
                                   framework]
 > "A playful and whimsical vector art of a Stochastic Tigger, wearing a t-shirt
 with a "GPT" text printed logo, surrounded by colorful geometric shapes. âar
 1:1 âupbeta" > > â Prompts and logo art was produced with [PromptPerfect]
 (https://promptperfect.jina.ai/) & [Stable Diffusion X](https://clipdrop.co/
 stable-diffusion) ![](https://img.shields.io/badge/Made%20with-JinaAI-
 blueviolet?style=flat) [![PyPI](https://img.shields.io/pypi/v/open_gpt_torch)]
 (https://pypi.org/project/open_gpt_torch/) [![PyPI - License](https://
 img.shields.io/pypi/l/open_gpt_torch)](https://pypi.org/project/open_gpt_torch/
 ) **OpenGPT** is an open-source _cloud-native_ large-scale **_multimodal
 models_** (LMMs) serving framework. It is designed to simplify the deployment
-and management of large language models, on a distributed cluster of GPUs. ##
-Table of contents - [Features](#features) - [Supported models](#supported-
-models) - [Get started](#get-started) - [Build a model serving in one line]
-(#build-a-model-serving-in-one-line) - [Cloud-native deployment](#cloud-native-
-deployment) - [Roadmap](#roadmap) ## Features OpenGPT provides the following
-features to make it easy to deploy and serve **large multi-modal models**
-(LMMs) at scale: - Support for multi-modal models on top of large language
-models - Scalable architecture for handling high traffic loads - Optimized for
-low-latency inference - Automatic model partitioning and distribution across
-multiple GPUs - Centralized model management and monitoring - REST API for easy
-integration with existing applications ## Updates - **2023-05-12**: ðWe have
-released the first version `v0.0.1` of OpenGPT. You can install it with `pip
-install open_gpt_torch`. ## Supported Models  OpenGPT supports the following
-models out of the box: - LLM (Large Language Model) - [LLaMA](https://
-ai.facebook.com/blog/large-language-model-llama-meta-ai/): open and efficient
-foundation language models by Meta - [Pythia](https://github.com/EleutherAI/
-pythia): a collection of models developed to facilitate interpretability
-research by EleutherAI - [StableLM](https://github.com/Stability-AI/StableLM):
-series of large language models by Stability AI - [Vicuna](https://
-vicuna.lmsys.org/): a chat assistant fine-tuned from LLaMA on user-shared
-conversations by LMSYS - [MOSS](https://txsun1997.github.io/blogs/moss.html):
-conversational language model from Fudan University - LMM (Large Multi-modal
-Model) - [OpenFlamingo](https://github.com/mlfoundations/open_flamingo): an
-open source version of DeepMind's [Flamingo](https://www.deepmind.com/blog/
-tackling-multiple-tasks-with-a-single-visual-language-model) model - [MiniGPT-
-4](https://minigpt-4.github.io/): aligns a frozen visual encoder with a frozen
-LLM, Vicuna, using just one projection layer. For more details about the
-supported models, please see the [Model Zoo](./MODEL_ZOO.md).  ## Roadmap You
-can view our roadmap with features that are planned, started, and completed on
-the [Roadmap discussion](https://github.com/jina-ai/opengpt/discussions/
-categories/roadmap) category. ## Get Started ### Installation Install the
-package with `pip`: ```bash pip install open_gpt_torch ``` ### Quickstart
-```python import open_gpt model = open_gpt.create_model('facebook/llama-7b',
-device='cuda', precision='fp16') prompt = "The quick brown fox jumps over the
-lazy dog." output = model.generate( prompt, max_length=100, temperature=0.9,
-top_k=50, top_p=0.95, repetition_penalty=1.2, do_sample=True,
-num_return_sequences=1, ) ``` > **Warning** > In the above example, we use
+and management of large language models, on a distributed cluster of GPUs. We
+aim to make it a one-stop solution for a centralized and accessible place to
+gather techniques for optimizing large-scale multimodal models and make them
+easy to use for everyone. ## Table of contents - [Features](#features) -
+[Supported models](#supported-models) - [Get started](#get-started) - [Build a
+model serving in one line](#build-a-model-serving-in-one-line) - [Cloud-native
+deployment](#cloud-native-deployment) - [Roadmap](#roadmap) ## Features OpenGPT
+provides the following features to make it easy to deploy and serve **large
+multi-modal models** (LMMs) at scale: - Support for multi-modal models on top
+of large language models - Scalable architecture for handling high traffic
+loads - Optimized for low-latency inference - Automatic model partitioning and
+distribution across multiple GPUs - Centralized model management and monitoring
+- REST API for easy integration with existing applications ## Updates - **2023-
+05-12**: ðWe have released the first version `v0.0.1` of OpenGPT. You can
+install it with `pip install open_gpt_torch`. ## Supported Models  OpenGPT
+supports the following models out of the box: - LLM (Large Language Model) -
+[LLaMA](https://ai.facebook.com/blog/large-language-model-llama-meta-ai/): open
+and efficient foundation language models by Meta - [Pythia](https://github.com/
+EleutherAI/pythia): a collection of models developed to facilitate
+interpretability research by EleutherAI - [StableLM](https://github.com/
+Stability-AI/StableLM): series of large language models by Stability AI -
+[Vicuna](https://vicuna.lmsys.org/): a chat assistant fine-tuned from LLaMA on
+user-shared conversations by LMSYS - [MOSS](https://txsun1997.github.io/blogs/
+moss.html): conversational language model from Fudan University - LMM (Large
+Multi-modal Model) - [OpenFlamingo](https://github.com/mlfoundations/
+open_flamingo): an open source version of DeepMind's [Flamingo](https://
+www.deepmind.com/blog/tackling-multiple-tasks-with-a-single-visual-language-
+model) model - [MiniGPT-4](https://minigpt-4.github.io/): aligns a frozen
+visual encoder with a frozen LLM, Vicuna, using just one projection layer. For
+more details about the supported models, please see the [Model Zoo](./
+MODEL_ZOO.md).  ## Roadmap You can view our roadmap with features that are
+planned, started, and completed on the [Roadmap discussion](https://github.com/
+jina-ai/opengpt/discussions/categories/roadmap) category. ## Get Started ###
+Installation Install the package with `pip`: ```bash pip install open_gpt_torch
+``` ### Quickstart ```python import open_gpt model = open_gpt.create_model
+( 'stabilityai/stablelm-tuned-alpha-3b', device='cuda', precision='fp16' )
+prompt = "The quick brown fox jumps over the lazy dog." output = model.generate
+( prompt, max_length=100, temperature=0.9, top_k=50, top_p=0.95,
+repetition_penalty=1.2, do_sample=True, num_return_sequences=1, ) ``` We use
+the [stabilityai/stablelm-tuned-alpha-3b](https://huggingface.co/stabilityai/
+stablelm-tuned-alpha-3b) as the open example model as it is relatively small
+and fast to download. > **Warning** > In the above example, we use
 `precision='fp16'` to reduce the memory usage and speed up the inference with
 some loss in accuracy on text generation tasks. > You can also use
 `precision='fp32'` instead as you like for better performance. > **Note** > It
 usually takes a while (several minutes) for the first time to download and load
 the model into the memory. In most cases of large model serving, the model
 cannot fit into a single GPU. To solve this problem, we also provide a
 `device_map` option (supported by `accecleate` package) to automatically
 partition the model and distribute it across multiple GPUs: ```python model =
-open_gpt.create_model( 'facebook/llama-7b', precision='fp16',
-device_map='balanced' ) ``` See [examples on how to use opengpt with different
-models.](./examples) ## Build a model serving in one line To do so, you can use
-the `serve` command: ```bash opengpt serve facebook/llama-7b --precision fp16 -
--port 51000 ``` This will start a server on port `51000`. You can then send
-requests to the server: ```python import requests prompt = "The quick brown fox
-jumps over the lazy dog." response = requests.post( "http://localhost:51000/
-generate", json={ "prompt": prompt, "max_length": 100, "temperature": 0.9,
-"top_k": 50, "top_p": 0.95, "repetition_penalty": 1.2, "do_sample": True,
-"num_return_sequences": 1, }, ) ``` Note that the server will only accept
-requests from the same machine. If you want to accept requests from other
-machines, you can use the `--host` flag to specify the host to bind to. ##
-Cloud-native deployment You can also deploy the server to a cloud provider like
-Jina Cloud or AWS. To do so, you can use `deploy` command: - Jina Cloud ```bash
-opengpt deploy facebook/llama-7b --device cuda --precision fp16 --provider jina
---name opengpt --replicas 2 ``` **TBD ...** ## Contributing We welcome
-contributions from the community! To contribute, please submit a pull request
-following our contributing guidelines. ## License OpenGPT is licensed under the
-Apache License, Version 2.0. See LICENSE for the full license text. Copyright
-2020-2022 Jina AI Limited. All rights reserved. Apache License Version 2.0,
-January 2004 http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE,
-REPRODUCTION, AND DISTRIBUTION 1. Definitions. "License" shall mean the terms
-and conditions for use, reproduction, and distribution as defined by Sections 1
-through 9 of this document. "Licensor" shall mean the copyright owner or entity
-authorized by the copyright owner that is granting the License. "Legal Entity"
-shall mean the union of the acting entity and all other entities that control,
-are controlled by, or are under common control with that entity. For the
-purposes of this definition, "control" means (i) the power, direct or indirect,
-to cause the direction or management of such entity, whether by contract or
-otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding
-shares, or (iii) beneficial ownership of such entity. "You" (or "Your") shall
-mean an individual or Legal Entity exercising permissions granted by this
-License. "Source" form shall mean the preferred form for making modifications,
-including but not limited to software source code, documentation source, and
-configuration files. "Object" form shall mean any form resulting from
-mechanical transformation or translation of a Source form, including but not
-limited to compiled object code, generated documentation, and conversions to
-other media types. "Work" shall mean the work of authorship, whether in Source
-or Object form, made available under the License, as indicated by a copyright
-notice that is included in or attached to the work (an example is provided in
-the Appendix below). "Derivative Works" shall mean any work, whether in Source
-or Object form, that is based on (or derived from) the Work and for which the
-editorial revisions, annotations, elaborations, or other modifications
-represent, as a whole, an original work of authorship. For the purposes of this
-License, Derivative Works shall not include works that remain separable from,
-or merely link (or bind by name) to the interfaces of, the Work and Derivative
-Works thereof. "Contribution" shall mean any work of authorship, including the
-original version of the Work and any modifications or additions to that Work or
-Derivative Works thereof, that is intentionally submitted to Licensor for
-inclusion in the Work by the copyright owner or by an individual or Legal
-Entity authorized to submit on behalf of the copyright owner. For the purposes
-of this definition, "submitted" means any form of electronic, verbal, or
-written communication sent to the Licensor or its representatives, including
-but not limited to communication on electronic mailing lists, source code
-control systems, and issue tracking systems that are managed by, or on behalf
-of, the Licensor for the purpose of discussing and improving the Work, but
-excluding communication that is conspicuously marked or otherwise designated in
-writing by the copyright owner as "Not a Contribution." "Contributor" shall
-mean Licensor and any individual or Legal Entity on behalf of whom a
-Contribution has been received by Licensor and subsequently incorporated within
-the Work. 2. Grant of Copyright License. Subject to the terms and conditions of
-this License, each Contributor hereby grants to You a perpetual, worldwide,
-non-exclusive, no-charge, royalty-free, irrevocable copyright license to
-reproduce, prepare Derivative Works of, publicly display, publicly perform,
-sublicense, and distribute the Work and such Derivative Works in Source or
-Object form. 3. Grant of Patent License. Subject to the terms and conditions of
-this License, each Contributor hereby grants to You a perpetual, worldwide,
-non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this
-section) patent license to make, have made, use, offer to sell, sell, import,
-and otherwise transfer the Work, where such license applies only to those
-patent claims licensable by such Contributor that are necessarily infringed by
-their Contribution(s) alone or by combination of their Contribution(s) with the
-Work to which such Contribution(s) was submitted. If You institute patent
-litigation against any entity (including a cross-claim or counterclaim in a
-lawsuit) alleging that the Work or a Contribution incorporated within the Work
-constitutes direct or contributory patent infringement, then any patent
-licenses granted to You under this License for that Work shall terminate as of
-the date such litigation is filed. 4. Redistribution. You may reproduce and
-distribute copies of the Work or Derivative Works thereof in any medium, with
-or without modifications, and in Source or Object form, provided that You meet
-the following conditions: (a) You must give any other recipients of the Work or
-Derivative Works a copy of this License; and (b) You must cause any modified
-files to carry prominent notices stating that You changed the files; and (c)
-You must retain, in the Source form of any Derivative Works that You
-distribute, all copyright, patent, trademark, and attribution notices from the
-Source form of the Work, excluding those notices that do not pertain to any
-part of the Derivative Works; and (d) If the Work includes a "NOTICE" text file
-as part of its distribution, then any Derivative Works that You distribute must
-include a readable copy of the attribution notices contained within such NOTICE
-file, excluding those notices that do not pertain to any part of the Derivative
-Works, in at least one of the following places: within a NOTICE text file
-distributed as part of the Derivative Works; within the Source form or
-documentation, if provided along with the Derivative Works; or, within a
-display generated by the Derivative Works, if and wherever such third-party
-notices normally appear. The contents of the NOTICE file are for informational
-purposes only and do not modify the License. You may add Your own attribution
-notices within Derivative Works that You distribute, alongside or as an
-addendum to the NOTICE text from the Work, provided that such additional
-attribution notices cannot be construed as modifying the License. You may add
-Your own copyright statement to Your modifications and may provide additional
-or different license terms and conditions for use, reproduction, or
-distribution of Your modifications, or for any such Derivative Works as a
-whole, provided Your use, reproduction, and distribution of the Work otherwise
-complies with the conditions stated in this License. 5. Submission of
-Contributions. Unless You explicitly state otherwise, any Contribution
-intentionally submitted for inclusion in the Work by You to the Licensor shall
-be under the terms and conditions of this License, without any additional terms
-or conditions. Notwithstanding the above, nothing herein shall supersede or
-modify the terms of any separate license agreement you may have executed with
-Licensor regarding such Contributions. 6. Trademarks. This License does not
-grant permission to use the trade names, trademarks, service marks, or product
-names of the Licensor, except as required for reasonable and customary use in
-describing the origin of the Work and reproducing the content of the NOTICE
-file. 7. Disclaimer of Warranty. Unless required by applicable law or agreed to
-in writing, Licensor provides the Work (and each Contributor provides its
-Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-KIND, either express or implied, including, without limitation, any warranties
-or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-PARTICULAR PURPOSE. You are solely responsible for determining the
-appropriateness of using or redistributing the Work and assume any risks
-associated with Your exercise of permissions under this License. 8. Limitation
-of Liability. In no event and under no legal theory, whether in tort (including
-negligence), contract, or otherwise, unless required by applicable law (such as
-deliberate and grossly negligent acts) or agreed to in writing, shall any
-Contributor be liable to You for damages, including any direct, indirect,
-special, incidental, or consequential damages of any character arising as a
-result of this License or out of the use or inability to use the Work
-(including but not limited to damages for loss of goodwill, work stoppage,
-computer failure or malfunction, or any and all other commercial damages or
-losses), even if such Contributor has been advised of the possibility of such
-damages. 9. Accepting Warranty or Additional Liability. While redistributing
-the Work or Derivative Works thereof, You may choose to offer, and charge a fee
-for, acceptance of support, warranty, indemnity, or other liability obligations
-and/or rights consistent with this License. However, in accepting such
-obligations, You may act only on Your own behalf and on Your sole
-responsibility, not on behalf of any other Contributor, and only if You agree
-to indemnify, defend, and hold each Contributor harmless for any liability
-incurred by, or claims asserted against, such Contributor by reason of your
-accepting any such warranty or additional liability. END OF TERMS AND
+open_gpt.create_model( 'stabilityai/stablelm-tuned-alpha-3b', precision='fp16',
+device_map='balanced' ) ``` In the above example, `device_map="balanced"`
+evenly split the model on all available GPUs, making it possible for you to
+serve large models. > **Note** > The `device_map` option is supported by the
+[accelerate](https://github.com/huggingface/accelerate) package. See [examples
+on how to use opengpt with different models.](./examples) ð¥ ## Build a model
+serving in one line To do so, you can use the `serve` command: ```bash opengpt
+serve stabilityai/stablelm-tuned-alpha-3b --precision fp16 --device_map
+balanced ``` ð¡ **Tip**: you can inspect the available options with `opengpt
+serve --help`. This will start a gRPC and HTTP server listening on port `51000`
+and `52000` respectively. Once the server is ready, as shown below:  Click to
+expand [https://github.com/jina-ai/opengpt/blob/main/.github/images/
+serve_ready.png]  You can then send requests to the server: ```python import
+requests prompt = "The quick brown fox jumps over the lazy dog." response =
+requests.post( "http://localhost:51000/generate", json={ "prompt": prompt,
+"max_length": 100, "temperature": 0.9, "top_k": 50, "top_p": 0.95,
+"repetition_penalty": 1.2, "do_sample": True, "num_return_sequences": 1, }, )
+``` What's more, we also provide a [Python client](https://github.com/jina-ai/
+inference-client/) (`inference-client`) for you to easily interact with the
+server: ```python from open_gpt import Client client = Client() # connect to
+the model server model = client.get_model(endpoint='grpc://0.0.0.0:51000')
+prompt = "The quick brown fox jumps over the lazy dog." output = model.generate
+( prompt, max_length=100, temperature=0.9, top_k=50, top_p=0.95,
+repetition_penalty=1.2, do_sample=True, num_return_sequences=1, ) ``` ð¡
+**Tip**: To display the list of available commands, please use the `list`
+command. ## Cloud-native deployment You can also deploy the server to a cloud
+provider like Jina Cloud or AWS. To do so, you can use `deploy` command: - Jina
+Cloud ```bash opengpt deploy stabilityai/stablelm-tuned-alpha-3b --device cuda
+--precision fp16 --provider jina --name opengpt --replicas 2 ``` **TBD ...** ##
+Contributing We welcome contributions from the community! To contribute, please
+submit a pull request following our contributing guidelines. ## License OpenGPT
+is licensed under the Apache License, Version 2.0. See LICENSE for the full
+license text. Copyright 2020-2022 Jina AI Limited. All rights reserved. Apache
+License Version 2.0, January 2004 http://www.apache.org/licenses/ TERMS AND
+CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION 1. Definitions. "License"
+shall mean the terms and conditions for use, reproduction, and distribution as
+defined by Sections 1 through 9 of this document. "Licensor" shall mean the
+copyright owner or entity authorized by the copyright owner that is granting
+the License. "Legal Entity" shall mean the union of the acting entity and all
+other entities that control, are controlled by, or are under common control
+with that entity. For the purposes of this definition, "control" means (i) the
+power, direct or indirect, to cause the direction or management of such entity,
+whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or
+more of the outstanding shares, or (iii) beneficial ownership of such entity.
+"You" (or "Your") shall mean an individual or Legal Entity exercising
+permissions granted by this License. "Source" form shall mean the preferred
+form for making modifications, including but not limited to software source
+code, documentation source, and configuration files. "Object" form shall mean
+any form resulting from mechanical transformation or translation of a Source
+form, including but not limited to compiled object code, generated
+documentation, and conversions to other media types. "Work" shall mean the work
+of authorship, whether in Source or Object form, made available under the
+License, as indicated by a copyright notice that is included in or attached to
+the work (an example is provided in the Appendix below). "Derivative Works"
+shall mean any work, whether in Source or Object form, that is based on (or
+derived from) the Work and for which the editorial revisions, annotations,
+elaborations, or other modifications represent, as a whole, an original work of
+authorship. For the purposes of this License, Derivative Works shall not
+include works that remain separable from, or merely link (or bind by name) to
+the interfaces of, the Work and Derivative Works thereof. "Contribution" shall
+mean any work of authorship, including the original version of the Work and any
+modifications or additions to that Work or Derivative Works thereof, that is
+intentionally submitted to Licensor for inclusion in the Work by the copyright
+owner or by an individual or Legal Entity authorized to submit on behalf of the
+copyright owner. For the purposes of this definition, "submitted" means any
+form of electronic, verbal, or written communication sent to the Licensor or
+its representatives, including but not limited to communication on electronic
+mailing lists, source code control systems, and issue tracking systems that are
+managed by, or on behalf of, the Licensor for the purpose of discussing and
+improving the Work, but excluding communication that is conspicuously marked or
+otherwise designated in writing by the copyright owner as "Not a Contribution."
+"Contributor" shall mean Licensor and any individual or Legal Entity on behalf
+of whom a Contribution has been received by Licensor and subsequently
+incorporated within the Work. 2. Grant of Copyright License. Subject to the
+terms and conditions of this License, each Contributor hereby grants to You a
+perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+copyright license to reproduce, prepare Derivative Works of, publicly display,
+publicly perform, sublicense, and distribute the Work and such Derivative Works
+in Source or Object form. 3. Grant of Patent License. Subject to the terms and
+conditions of this License, each Contributor hereby grants to You a perpetual,
+worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as
+stated in this section) patent license to make, have made, use, offer to sell,
+sell, import, and otherwise transfer the Work, where such license applies only
+to those patent claims licensable by such Contributor that are necessarily
+infringed by their Contribution(s) alone or by combination of their
+Contribution(s) with the Work to which such Contribution(s) was submitted. If
+You institute patent litigation against any entity (including a cross-claim or
+counterclaim in a lawsuit) alleging that the Work or a Contribution
+incorporated within the Work constitutes direct or contributory patent
+infringement, then any patent licenses granted to You under this License for
+that Work shall terminate as of the date such litigation is filed. 4.
+Redistribution. You may reproduce and distribute copies of the Work or
+Derivative Works thereof in any medium, with or without modifications, and in
+Source or Object form, provided that You meet the following conditions: (a) You
+must give any other recipients of the Work or Derivative Works a copy of this
+License; and (b) You must cause any modified files to carry prominent notices
+stating that You changed the files; and (c) You must retain, in the Source form
+of any Derivative Works that You distribute, all copyright, patent, trademark,
+and attribution notices from the Source form of the Work, excluding those
+notices that do not pertain to any part of the Derivative Works; and (d) If the
+Work includes a "NOTICE" text file as part of its distribution, then any
+Derivative Works that You distribute must include a readable copy of the
+attribution notices contained within such NOTICE file, excluding those notices
+that do not pertain to any part of the Derivative Works, in at least one of the
+following places: within a NOTICE text file distributed as part of the
+Derivative Works; within the Source form or documentation, if provided along
+with the Derivative Works; or, within a display generated by the Derivative
+Works, if and wherever such third-party notices normally appear. The contents
+of the NOTICE file are for informational purposes only and do not modify the
+License. You may add Your own attribution notices within Derivative Works that
+You distribute, alongside or as an addendum to the NOTICE text from the Work,
+provided that such additional attribution notices cannot be construed as
+modifying the License. You may add Your own copyright statement to Your
+modifications and may provide additional or different license terms and
+conditions for use, reproduction, or distribution of Your modifications, or for
+any such Derivative Works as a whole, provided Your use, reproduction, and
+distribution of the Work otherwise complies with the conditions stated in this
+License. 5. Submission of Contributions. Unless You explicitly state otherwise,
+any Contribution intentionally submitted for inclusion in the Work by You to
+the Licensor shall be under the terms and conditions of this License, without
+any additional terms or conditions. Notwithstanding the above, nothing herein
+shall supersede or modify the terms of any separate license agreement you may
+have executed with Licensor regarding such Contributions. 6. Trademarks. This
+License does not grant permission to use the trade names, trademarks, service
+marks, or product names of the Licensor, except as required for reasonable and
+customary use in describing the origin of the Work and reproducing the content
+of the NOTICE file. 7. Disclaimer of Warranty. Unless required by applicable
+law or agreed to in writing, Licensor provides the Work (and each Contributor
+provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR
+CONDITIONS OF ANY KIND, either express or implied, including, without
+limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT,
+MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely
+responsible for determining the appropriateness of using or redistributing the
+Work and assume any risks associated with Your exercise of permissions under
+this License. 8. Limitation of Liability. In no event and under no legal
+theory, whether in tort (including negligence), contract, or otherwise, unless
+required by applicable law (such as deliberate and grossly negligent acts) or
+agreed to in writing, shall any Contributor be liable to You for damages,
+including any direct, indirect, special, incidental, or consequential damages
+of any character arising as a result of this License or out of the use or
+inability to use the Work (including but not limited to damages for loss of
+goodwill, work stoppage, computer failure or malfunction, or any and all other
+commercial damages or losses), even if such Contributor has been advised of the
+possibility of such damages. 9. Accepting Warranty or Additional Liability.
+While redistributing the Work or Derivative Works thereof, You may choose to
+offer, and charge a fee for, acceptance of support, warranty, indemnity, or
+other liability obligations and/or rights consistent with this License.
+However, in accepting such obligations, You may act only on Your own behalf and
+on Your sole responsibility, not on behalf of any other Contributor, and only
+if You agree to indemnify, defend, and hold each Contributor harmless for any
+liability incurred by, or claims asserted against, such Contributor by reason
+of your accepting any such warranty or additional liability. END OF TERMS AND
 CONDITIONS Copyright 2020-2022 Jina AI Limited Licensed under the Apache
 License, Version 2.0 (the "License"); you may not use this file except in
 compliance with the License. You may obtain a copy of the License at http://
 www.apache.org/licenses/LICENSE-2.0 Unless required by applicable law or agreed
 to in writing, software distributed under the License is distributed on an "AS
 IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
 implied. See the License for the specific language governing permissions and
```

