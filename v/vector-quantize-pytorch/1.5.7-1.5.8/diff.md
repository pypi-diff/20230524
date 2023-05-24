# Comparing `tmp/vector_quantize_pytorch-1.5.7.tar.gz` & `tmp/vector_quantize_pytorch-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.5.7.tar", last modified: Wed May 24 14:18:41 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.5.8.tar", last modified: Wed May 24 14:28:34 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.5.7.tar` & `vector_quantize_pytorch-1.5.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:18:41.417297 vector_quantize_pytorch-1.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-24 14:18:26.000000 vector_quantize_pytorch-1.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-24 14:18:41.417297 vector_quantize_pytorch-1.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15061 2023-05-24 14:18:26.000000 vector_quantize_pytorch-1.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 14:18:41.417297 vector_quantize_pytorch-1.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-24 14:18:26.000000 vector_quantize_pytorch-1.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:18:41.417297 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-24 14:18:26.000000 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-24 14:18:26.000000 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-24 14:18:26.000000 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (123)    24348 2023-05-24 14:18:26.000000 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:18:41.417297 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-24 14:18:41.000000 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-24 14:18:41.000000 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:18:41.000000 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-24 14:18:41.000000 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-24 14:18:41.000000 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:28:34.000207 vector_quantize_pytorch-1.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-24 14:28:20.000000 vector_quantize_pytorch-1.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-24 14:28:34.000207 vector_quantize_pytorch-1.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15061 2023-05-24 14:28:20.000000 vector_quantize_pytorch-1.5.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 14:28:34.000207 vector_quantize_pytorch-1.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-24 14:28:20.000000 vector_quantize_pytorch-1.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:28:34.000207 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-24 14:28:20.000000 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-24 14:28:20.000000 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-24 14:28:20.000000 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24652 2023-05-24 14:28:20.000000 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:28:34.000207 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-24 14:28:33.000000 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-24 14:28:33.000000 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:28:33.000000 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-24 14:28:33.000000 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-24 14:28:33.000000 vector_quantize_pytorch-1.5.8/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.5.7/LICENSE` & `vector_quantize_pytorch-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.7/PKG-INFO` & `vector_quantize_pytorch-1.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.5.7
+Version: 1.5.8
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.5.7/README.md` & `vector_quantize_pytorch-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.7/setup.py` & `vector_quantize_pytorch-1.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vector_quantize_pytorch',
   packages = find_packages(),
-  version = '1.5.7',
+  version = '1.5.8',
   license='MIT',
   description = 'Vector Quantization - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vector-quantizer-pytorch',
   keywords = [
```

### Comparing `vector_quantize_pytorch-1.5.7/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.5.8/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.7/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.5.8/vector_quantize_pytorch/residual_vq.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.7/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.5.8/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -598,17 +598,14 @@
 
         # handle multi-headed separate codebooks
 
         if is_multiheaded:
             ein_rhs_eq = 'h b n d' if self.separate_codebook_per_head else '1 (b h) n d'
             x = rearrange(x, f'b n (h d) -> {ein_rhs_eq}', h = heads)
 
-            if exists(mask):
-                mask = repeat(mask, 'b n -> h b n', h = heads)
-
         # quantize
 
         quantize, embed_ind, distances = self._codebook(x)
 
         if self.training:
             quantize = x + (quantize - x).detach()
 
@@ -653,21 +650,31 @@
         # aggregate loss
 
         loss = torch.tensor([0.], device = device, requires_grad = self.training)
 
         if self.training:
             if self.commitment_weight > 0:
                 if self.commitment_use_cross_entropy_loss:
+                    if exists(mask):
+                        if is_multiheaded:
+                            mask = repeat(mask, 'b n -> b n h', h = heads)
+
+                        embed_ind.masked_fill_(~mask, -1)
+
                     commit_loss = calculate_ce_loss(embed_ind)
                 else:
                     detached_quantize = quantize.detach()
 
                     if exists(mask):
                         # with variable lengthed sequences
                         commit_loss = F.mse_loss(detached_quantize, x, reduction = 'none')
+
+                        if is_multiheaded:
+                            mask = repeat(mask, 'b n -> c (b h) n', c = commit_loss.shape[0], h = commit_loss.shape[1] // mask.shape[0])
+
                         commit_loss = commit_loss[mask].mean()
                     else:
                         commit_loss = F.mse_loss(detached_quantize, x)
 
                 loss = loss + commit_loss * self.commitment_weight
 
             if self.orthogonal_reg_weight > 0:
```

### Comparing `vector_quantize_pytorch-1.5.7/vector_quantize_pytorch.egg-info/PKG-INFO` & `vector_quantize_pytorch-1.5.8/vector_quantize_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-quantize-pytorch
-Version: 1.5.7
+Version: 1.5.8
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

