# Comparing `tmp/Sophia-Optimizer-0.1.1.tar.gz` & `tmp/Sophia-Optimizer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sophia-Optimizer-0.1.1.tar", last modified: Wed May 24 18:41:05 2023, max compression
+gzip compressed data, was "Sophia-Optimizer-0.1.2.tar", last modified: Wed May 24 20:18:29 2023, max compression
```

## Comparing `Sophia-Optimizer-0.1.1.tar` & `Sophia-Optimizer-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:41:05.773739 Sophia-Optimizer-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 18:40:49.000000 Sophia-Optimizer-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-24 18:41:05.773739 Sophia-Optimizer-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-24 18:40:49.000000 Sophia-Optimizer-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:41:05.773739 Sophia-Optimizer-0.1.1/Sophia/
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-24 18:40:49.000000 Sophia-Optimizer-0.1.1/Sophia/Sophia.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-24 18:40:49.000000 Sophia-Optimizer-0.1.1/Sophia/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:41:05.773739 Sophia-Optimizer-0.1.1/Sophia_Optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-24 18:41:05.000000 Sophia-Optimizer-0.1.1/Sophia_Optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-24 18:41:05.000000 Sophia-Optimizer-0.1.1/Sophia_Optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:41:05.000000 Sophia-Optimizer-0.1.1/Sophia_Optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 18:41:05.000000 Sophia-Optimizer-0.1.1/Sophia_Optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 18:41:05.000000 Sophia-Optimizer-0.1.1/Sophia_Optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 18:41:05.773739 Sophia-Optimizer-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-24 18:40:49.000000 Sophia-Optimizer-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:18:29.695143 Sophia-Optimizer-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 20:18:18.000000 Sophia-Optimizer-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-24 20:18:29.695143 Sophia-Optimizer-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-05-24 20:18:18.000000 Sophia-Optimizer-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:18:29.695143 Sophia-Optimizer-0.1.2/Sophia/
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-24 20:18:18.000000 Sophia-Optimizer-0.1.2/Sophia/Sophia.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-24 20:18:18.000000 Sophia-Optimizer-0.1.2/Sophia/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:18:29.695143 Sophia-Optimizer-0.1.2/Sophia_Optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-24 20:18:29.000000 Sophia-Optimizer-0.1.2/Sophia_Optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-24 20:18:29.000000 Sophia-Optimizer-0.1.2/Sophia_Optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:18:29.000000 Sophia-Optimizer-0.1.2/Sophia_Optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 20:18:29.000000 Sophia-Optimizer-0.1.2/Sophia_Optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 20:18:29.000000 Sophia-Optimizer-0.1.2/Sophia_Optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 20:18:29.695143 Sophia-Optimizer-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-24 20:18:18.000000 Sophia-Optimizer-0.1.2/setup.py
```

### Comparing `Sophia-Optimizer-0.1.1/LICENSE` & `Sophia-Optimizer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Sophia-Optimizer-0.1.1/PKG-INFO` & `Sophia-Optimizer-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sophia-Optimizer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Sophia Optimizer ULTRA FAST
 Home-page: https://github.com/kyegomez/Sophia
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: APACHE
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Sophia-Optimizer-0.1.1/README.md` & `Sophia-Optimizer-0.1.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,57 @@
 # Sophia Optimizer
 
-Cut Model Training Cost by 50% with this simple plug in Optimizer
+Cut Model Training Cost by 50%? with this all-new simple plug in and play Optimizer: Sophia
 
-## 👥 Share With Your Friends
-If you find Sophia useful, please share this GitHub repository with your friends and colleagues. Let's cut the cost of AI training together!
-
-[Share on Twitter](https://twitter.com/intent/tweet?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FSophia&text=Check%20out%20Sophia%20Optimizer%20-%20a%20second-order%20clipped%20stochastic%20optimization%20algorithm%20that%20cuts%20model%20training%20cost%20in%20half!%20%23DeepLearning%20%23AI%20%23Optimization)
-
-[Share on Linkedin](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FSophia&title=Sophia%20Optimizer&summary=Check%20out%20Sophia%20Optimizer%20-%20a%20second-order%20clipped%20stochastic%20optimization%20algorithm%20that%20cuts%20model%20training%20cost%20in%20half!%20%23DeepLearning%20%23AI%20%23Optimization)
-
-# 🌐 Agora: AI Researchers Advancing Humanity
-Sophia is backed by Agora, a community of AI researchers dedicated to advancing humanity and solving some of the world's biggest problems. Join us in making a difference!
-
-[Join our discord and write your mark on the history books](https://discord.gg/qUtxnK2NMf)
+[Sophia: A Scalable Stochastic Second-order Optimizer for
+Language Model Pre-training](https://arxiv.org/pdf/2305.14342.pdf)
 
 Sophia is an second order clipped stochastic optimization algorithm that uses an inexpensive stochastic estimate of the diagonal of the Hessian as an pre-conditioner and a clipping mechanism to control the worst case update size. It achieves better performance than adam in terms of validation pre-traing loss, total compute, and wall-clock time. By cutting model training cost in half, Sophia can help save millions if not billions of dollars in computational resources.
 
+
 ## Benefits
 
 Sophia achievs the same validation pre training loss with 50% fewer number of steps than Adam
 
 50% less total compute and 50% less wall-clock time
 
 Seamless integration into existing training pipelines -- plug in and play!
 
 No special requirments on model architecture or computing infrastructure
 
 Supports both Hutchinson and Gauss-Newton-Bartlett Hessian Estimators
 
+
+
+## 👥 Share With Your Friends
+If you find Sophia useful, please share this GitHub repository with your friends and colleagues. Let's cut the cost of AI training together!
+
+[Share on Twitter](https://twitter.com/intent/tweet?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FSophia&text=Check%20out%20Sophia%20Optimizer%20-%20a%20second-order%20clipped%20stochastic%20optimization%20algorithm%20that%20cuts%20model%20training%20cost%20in%20half!%20%23DeepLearning%20%23AI%20%23Optimization)
+
+[Share on Linkedin](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FSophia&title=Sophia%20Optimizer&summary=Check%20out%20Sophia%20Optimizer%20-%20a%20second-order%20clipped%20stochastic%20optimization%20algorithm%20that%20cuts%20model%20training%20cost%20in%20half!%20%23DeepLearning%20%23AI%20%23Optimization)
+
+# 🌐 Agora: AI Researchers Advancing Humanity
+Sophia is backed by Agora, a community of AI researchers dedicated to advancing humanity and solving some of the world's biggest problems. Join us in making a difference!
+
+[Join our discord and write your mark on the history books](https://discord.gg/qUtxnK2NMf)
+
+
+
 # Usage
 
 Download with pip ```pip install Sophia-Optimizer```
 
-
 ```python 
 import torch 
 from torch import nn
 from Sophia import Sophia
-from Nebula import Nebula
+
+#or decoupled
+#from Sophia import DecoupledSophia #plug in and play, personalize, improved maintainability
+
 
 #define your model
 
 class MyModel(nn.Module):
     def __init__(self):
         super(MyModel, self).__init__()
         self.fc1 = nn.Linear(784, 128)
@@ -51,20 +61,23 @@
         x = torch.relu(self.fc1(x))
         x = self.fc2(x)
         return x
 
 
 #init model loss function and input data
 model = MyModel()
-loss_function = Nebula()
+loss_function = nn.CrossEntropy()
 input_data = ... #input data
 
 #init the optimizer
 optimizer = Sophia(model, input_data, model.parameters(), lr=1e-3, estimator="Hutchinson")
 
+#decoupled
+#optimizer = DecoupledSophia(model.parameters(), hessian_estimator, lr=1e-3)
+
 
 #training loop
 for epoch in range(epochs):
     for batch in data_loader:
         optimizer.zero_grad()
         output = model(batch)
         loss = loss_function(output, target)
@@ -165,7 +178,52 @@
         y_hats = [torch.softmax(logit, dim=0) for logit in logits]
         g_hat = torch.autograd.grad(sum([self.loss_function(logit, y_hat) for logit, y_hat in zip(logits, y_hats)]) / B, p, retain_graph=True)[0]
         return B * g_hat * g_hat
     
         
 ```
 
+# Roadmap
+The following roadmap outlines the future development plans for the Sophia optimizer. The roadmap is divided into three stages: short-term, mid-term, and long-term goals.
+
+
+## Short-term Goals
+
+Ready to train plug in and play file with your own model or Andromeda
+
+Performance improvements: Investigate and implement potential performance improvements to further reduce training time and computational resources -> Decoupled Sophia + heavy metric logging + Implement in Triton and or Jax?
+
+Additional Hessian estimators: Research and implement other Hessian estimators to provide more options for users.
+
+Hyperparameter tuning: Develop a set of recommended hyperparameters for various use cases and model architectures.
+
+# Mid-term Goals
+Integration with Andromeda model: Train the Andromeda model using the Sophia optimizer and compare its performance with other optimizers.
+
+Sophia optimizer variants: Explore and develop variants of the Sophia optimizer tailored for specific tasks, such as computer vision, multi-modality AI, and natural language processing, and reinforcement learning.
+
+Distributed training: Implement support for distributed training to enable users to train large-scale models using Sophia across multiple devices and nodes.
+
+Automatic hyperparameter tuning: Develop an automatic hyperparameter tuning module to help users find the best hyperparameters for their specific use case.
+
+# Long-term Goals
+Training multiple models in parallel: Develop a framework for training multiple models concurrently with different optimizers, allowing users to test and compare the performance of various optimizers, including Sophia, on their specific tasks.
+
+Sophia optimizer for other domains: Adapt the Sophia optimizer for other domains, such as optimization in reinforcement learning, Bayesian optimization, and evolutionary algorithms.
+
+
+By following this roadmap, we aim to make the Sophia optimizer a powerful and versatile tool for the deep learning community, enabling users to train their models more efficiently and effectively.
+
+
+# Epoch 1 - Decoupled Sophia
+
+The DecoupledSophia optimizer offers several benefits that can help accelerate training speed and improve the flexibility of the optimization process:
+
+Modularity: Decoupling the Hessian estimation from the main optimizer allows users to easily plug in different Hessian estimators without modifying the core optimizer code. This modularity makes it easier to experiment with various Hessian estimation techniques and find the best one for a specific task.
+
+Ease of experimentation: With a decoupled architecture, researchers and practitioners can develop and test new Hessian estimators independently from the optimizer. This can lead to faster innovation and the discovery of more efficient Hessian estimation methods, which can further accelerate training speed.
+
+Customization: Users can create custom Hessian estimators tailored to their specific use cases or model architectures. This customization can potentially lead to better optimization performance and faster training times.
+
+Improved maintainability: Separating the Hessian estimation from the optimizer makes the codebase easier to maintain and understand. This can lead to faster bug fixes and improvements in the optimizer's performance.
+
+By offering these benefits, DecoupledSophia can help users accelerate training speed and improve the overall optimization process. The modular design allows for easy experimentation with different Hessian estimators, which can lead to the discovery of more efficient techniques and ultimately faster training times.
```

### Comparing `Sophia-Optimizer-0.1.1/Sophia/Sophia.py` & `Sophia-Optimizer-0.1.2/Sophia/Sophia.py`

 * *Files identical despite different names*

### Comparing `Sophia-Optimizer-0.1.1/Sophia_Optimizer.egg-info/PKG-INFO` & `Sophia-Optimizer-0.1.2/Sophia_Optimizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sophia-Optimizer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Sophia Optimizer ULTRA FAST
 Home-page: https://github.com/kyegomez/Sophia
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: APACHE
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Sophia-Optimizer-0.1.1/setup.py` & `Sophia-Optimizer-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'Sophia-Optimizer',
   packages = find_packages(exclude=[]),
-  version = '0.1.1',
+  version = '0.1.2',
   license='APACHE',
   description = 'Sophia Optimizer ULTRA FAST',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/Sophia',
   keywords = [
```

