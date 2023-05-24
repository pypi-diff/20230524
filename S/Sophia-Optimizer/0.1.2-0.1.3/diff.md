# Comparing `tmp/Sophia-Optimizer-0.1.2.tar.gz` & `tmp/Sophia-Optimizer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sophia-Optimizer-0.1.2.tar", last modified: Wed May 24 20:18:29 2023, max compression
+gzip compressed data, was "Sophia-Optimizer-0.1.3.tar", last modified: Wed May 24 21:32:54 2023, max compression
```

## Comparing `Sophia-Optimizer-0.1.2.tar` & `Sophia-Optimizer-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:18:29.695143 Sophia-Optimizer-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 20:18:18.000000 Sophia-Optimizer-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-24 20:18:29.695143 Sophia-Optimizer-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-05-24 20:18:18.000000 Sophia-Optimizer-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:18:29.695143 Sophia-Optimizer-0.1.2/Sophia/
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-24 20:18:18.000000 Sophia-Optimizer-0.1.2/Sophia/Sophia.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-24 20:18:18.000000 Sophia-Optimizer-0.1.2/Sophia/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:18:29.695143 Sophia-Optimizer-0.1.2/Sophia_Optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-24 20:18:29.000000 Sophia-Optimizer-0.1.2/Sophia_Optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-24 20:18:29.000000 Sophia-Optimizer-0.1.2/Sophia_Optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:18:29.000000 Sophia-Optimizer-0.1.2/Sophia_Optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 20:18:29.000000 Sophia-Optimizer-0.1.2/Sophia_Optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 20:18:29.000000 Sophia-Optimizer-0.1.2/Sophia_Optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 20:18:29.695143 Sophia-Optimizer-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-24 20:18:18.000000 Sophia-Optimizer-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:32:54.880949 Sophia-Optimizer-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 21:32:41.000000 Sophia-Optimizer-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-24 21:32:54.880949 Sophia-Optimizer-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13213 2023-05-24 21:32:41.000000 Sophia-Optimizer-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:32:54.876949 Sophia-Optimizer-0.1.3/Sophia/
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-24 21:32:41.000000 Sophia-Optimizer-0.1.3/Sophia/Sophia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-24 21:32:41.000000 Sophia-Optimizer-0.1.3/Sophia/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:32:54.880949 Sophia-Optimizer-0.1.3/Sophia_Optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-24 21:32:54.000000 Sophia-Optimizer-0.1.3/Sophia_Optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-24 21:32:54.000000 Sophia-Optimizer-0.1.3/Sophia_Optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 21:32:54.000000 Sophia-Optimizer-0.1.3/Sophia_Optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 21:32:54.000000 Sophia-Optimizer-0.1.3/Sophia_Optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 21:32:54.000000 Sophia-Optimizer-0.1.3/Sophia_Optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 21:32:54.880949 Sophia-Optimizer-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-24 21:32:41.000000 Sophia-Optimizer-0.1.3/setup.py
```

### Comparing `Sophia-Optimizer-0.1.2/LICENSE` & `Sophia-Optimizer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Sophia-Optimizer-0.1.2/PKG-INFO` & `Sophia-Optimizer-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sophia-Optimizer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Sophia Optimizer ULTRA FAST
 Home-page: https://github.com/kyegomez/Sophia
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: APACHE
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Sophia-Optimizer-0.1.2/README.md` & `Sophia-Optimizer-0.1.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Sophia Optimizer
 
 Cut Model Training Cost by 50%? with this all-new simple plug in and play Optimizer: Sophia
 
 [Sophia: A Scalable Stochastic Second-order Optimizer for
 Language Model Pre-training](https://arxiv.org/pdf/2305.14342.pdf)
 
+Now with training file ready in experiments folder! 🔥🔥🔥
+
 Sophia is an second order clipped stochastic optimization algorithm that uses an inexpensive stochastic estimate of the diagonal of the Hessian as an pre-conditioner and a clipping mechanism to control the worst case update size. It achieves better performance than adam in terms of validation pre-traing loss, total compute, and wall-clock time. By cutting model training cost in half, Sophia can help save millions if not billions of dollars in computational resources.
 
 
 ## Benefits
 
 Sophia achievs the same validation pre training loss with 50% fewer number of steps than Adam
 
@@ -34,15 +36,19 @@
 
 [Join our discord and write your mark on the history books](https://discord.gg/qUtxnK2NMf)
 
 
 
 # Usage
 
-Download with pip ```pip install Sophia-Optimizer```
+Download with pip ```pip install Sophia-Optimizer``` 
+
+or 
+
+download with git ```git clone https://github.com/kyegomez/Sophia.git ```
 
 ```python 
 import torch 
 from torch import nn
 from Sophia import Sophia
 
 #or decoupled
@@ -81,14 +87,32 @@
         optimizer.zero_grad()
         output = model(batch)
         loss = loss_function(output, target)
         loss.backward()
         optimizer.step()
 ```
 
+## Training:
+To run training use git clone method and navigate to experiments folder and if not then do the following:
+
+```python
+from Sophia import DecoupledSophia, trainer
+
+
+#train model
+trainer.train()
+
+
+#eval the model
+eval_results = trainer.evaluate()
+print(f"Perplexity: {torch.exp(torch.tensor(eval_results['eval_loss']))}")
+
+```
+
+
 # Algorithmic pseudocode:
 
 ```
 
 Initialize parameters: θ1, learning rate {ηt}, hyperparameters λ, β1, β2, ϵ, and estimator choice Estimator ∈ {Hutchinson, Gauss-Newton-Bartlett}
 Set m0 = 0, v0 = 0, h1−k = 0
 For t = 1 to T do
@@ -222,8 +246,92 @@
 
 Ease of experimentation: With a decoupled architecture, researchers and practitioners can develop and test new Hessian estimators independently from the optimizer. This can lead to faster innovation and the discovery of more efficient Hessian estimation methods, which can further accelerate training speed.
 
 Customization: Users can create custom Hessian estimators tailored to their specific use cases or model architectures. This customization can potentially lead to better optimization performance and faster training times.
 
 Improved maintainability: Separating the Hessian estimation from the optimizer makes the codebase easier to maintain and understand. This can lead to faster bug fixes and improvements in the optimizer's performance.
 
-By offering these benefits, DecoupledSophia can help users accelerate training speed and improve the overall optimization process. The modular design allows for easy experimentation with different Hessian estimators, which can lead to the discovery of more efficient techniques and ultimately faster training times.
+By offering these benefits, DecoupledSophia can help users accelerate training speed and improve the overall optimization process. The modular design allows for easy experimentation with different Hessian estimators, which can lead to the discovery of more efficient techniques and ultimately faster training times.
+
+
+# Epoch - 2
+Implement the training strategy as closely as possible with transformers library!
+
+# Load and preprocess the OpenWebText dataset
+class CFG:
+    SEQ_LEN: int = 1024
+    NUM_CPU: int = multiprocessing.cpu_count()
+    TOKENIZER: str = "gpt2"
+
+tokenizer = AutoTokenizer.from_pretrained(CFG.TOKENIZER)
+dataset = load_dataset("openwebtext")
+
+def tokenize_function(example):
+    return tokenizer(example["text"] + tokenizer.eos_token)
+
+tokenized_dataset = dataset.map(
+    tokenize_function,
+    batched=True,
+    num_proc=CFG.NUM_CPU,
+    remove_columns=["text"],
+)
+
+block_size = CFG.SEQ_LEN
+
+def group_texts(examples):
+    concatenated_examples = {k: list(chain(*examples[k])) for k in examples.keys()}
+    total_length = len(concatenated_examples[list(examples.keys())[0]])
+    if total_length >= block_size:
+        total_length = (total_length // block_size) * block_size
+    result = {
+        k: [t[i : i + block_size] for i in range(0, total_length, block_size)]
+        for k, t in concatenated_examples.items()
+    }
+    return result
+
+train_dataset = tokenized_dataset.map(
+    group_texts,
+    batched=True,
+    num_proc=CFG.NUM_CPU,
+)
+
+# Initialize the GPT-2 model and tokenizer
+config = GPT2Config.from_pretrained("gpt2", n_ctx=1024)
+model = GPT2LMHeadModel.from_pretrained("gpt2", config=config)
+
+# Choose a Hessian estimator
+hessian_estimator = HutchinsonEstimator()
+
+# Initialize the DecoupledSophia optimizer
+optimizer = DecoupledSophia(model.parameters(), hessian_estimator, lr=1e-3)
+
+# Set up the training arguments
+training_args = TrainingArguments(
+    output_dir="output",
+    overwrite_output_dir=True,
+    num_train_epochs=3,
+    per_device_train_batch_size=480,
+    save_steps=10_000,
+    save_total_limit=2,
+    prediction_loss_only=True,
+    gradient_accumulation_steps=1,
+    gradient_clipping=1.0,
+    learning_rate_scheduler_type="cosine",
+    warmup_steps=2000,
+    report_to="none",
+)
+
+# Create the Trainer
+trainer = Trainer(
+    model=model,
+    args=training_args,
+    data_collator=DataCollatorForLanguageModeling(tokenizer=tokenizer, mlm=False),
+    train_dataset=train_dataset,
+    optimizers=(optimizer, None),
+)
+
+# Train the model
+trainer.train()
+
+# Evaluate the model
+eval_results = trainer.evaluate()
+print(f"Perplexity: {torch.exp(torch.tensor(eval_results['eval_loss']))}")
```

### Comparing `Sophia-Optimizer-0.1.2/Sophia/Sophia.py` & `Sophia-Optimizer-0.1.3/Sophia/Sophia.py`

 * *Files identical despite different names*

### Comparing `Sophia-Optimizer-0.1.2/Sophia_Optimizer.egg-info/PKG-INFO` & `Sophia-Optimizer-0.1.3/Sophia_Optimizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sophia-Optimizer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Sophia Optimizer ULTRA FAST
 Home-page: https://github.com/kyegomez/Sophia
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: APACHE
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Sophia-Optimizer-0.1.2/setup.py` & `Sophia-Optimizer-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'Sophia-Optimizer',
   packages = find_packages(exclude=[]),
-  version = '0.1.2',
+  version = '0.1.3',
   license='APACHE',
   description = 'Sophia Optimizer ULTRA FAST',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/Sophia',
   keywords = [
```

