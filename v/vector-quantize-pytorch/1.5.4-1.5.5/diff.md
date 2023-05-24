# Comparing `tmp/vector_quantize_pytorch-1.5.4.tar.gz` & `tmp/vector_quantize_pytorch-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.5.4.tar", last modified: Tue May 23 20:27:28 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.5.5.tar", last modified: Tue May 23 20:47:12 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.5.4.tar` & `vector_quantize_pytorch-1.5.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:27:28.290620 vector_quantize_pytorch-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 20:27:14.000000 vector_quantize_pytorch-1.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-23 20:27:28.290620 vector_quantize_pytorch-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15061 2023-05-23 20:27:14.000000 vector_quantize_pytorch-1.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 20:27:28.290620 vector_quantize_pytorch-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-23 20:27:14.000000 vector_quantize_pytorch-1.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:27:28.290620 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-23 20:27:14.000000 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-23 20:27:14.000000 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-23 20:27:14.000000 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (123)    23042 2023-05-23 20:27:14.000000 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:27:28.290620 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-23 20:27:28.000000 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-23 20:27:28.000000 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:27:28.000000 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 20:27:28.000000 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-23 20:27:28.000000 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:47:12.654228 vector_quantize_pytorch-1.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 20:46:55.000000 vector_quantize_pytorch-1.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-23 20:47:12.654228 vector_quantize_pytorch-1.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15061 2023-05-23 20:46:55.000000 vector_quantize_pytorch-1.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 20:47:12.654228 vector_quantize_pytorch-1.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-23 20:46:55.000000 vector_quantize_pytorch-1.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:47:12.654228 vector_quantize_pytorch-1.5.5/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-23 20:46:55.000000 vector_quantize_pytorch-1.5.5/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-23 20:46:55.000000 vector_quantize_pytorch-1.5.5/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-23 20:46:55.000000 vector_quantize_pytorch-1.5.5/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-05-23 20:46:55.000000 vector_quantize_pytorch-1.5.5/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:47:12.654228 vector_quantize_pytorch-1.5.5/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-23 20:47:12.000000 vector_quantize_pytorch-1.5.5/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-23 20:47:12.000000 vector_quantize_pytorch-1.5.5/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:47:12.000000 vector_quantize_pytorch-1.5.5/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 20:47:12.000000 vector_quantize_pytorch-1.5.5/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-23 20:47:12.000000 vector_quantize_pytorch-1.5.5/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.5.4/LICENSE` & `vector_quantize_pytorch-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.4/PKG-INFO` & `vector_quantize_pytorch-1.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.5.4
+Version: 1.5.5
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.5.4/README.md` & `vector_quantize_pytorch-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.4/setup.py` & `vector_quantize_pytorch-1.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vector_quantize_pytorch',
   packages = find_packages(),
-  version = '1.5.4',
+  version = '1.5.5',
   license='MIT',
   description = 'Vector Quantization - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vector-quantizer-pytorch',
   keywords = [
```

### Comparing `vector_quantize_pytorch-1.5.4/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.5.5/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.4/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.5.5/vector_quantize_pytorch/residual_vq.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.4/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.5.5/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,14 +308,17 @@
 
             embed_normalized = self.embed_avg / rearrange(cluster_size, '... -> ... 1')
             self.embed.data.copy_(embed_normalized)
             self.expire_codes_(x)
 
         quantize = batched_embedding(embed_ind, self.embed)
 
+        if self.training:
+            quantize = x + (quantize - x).detach()
+
         if needs_codebook_dim:
             quantize, embed_ind = map(lambda t: rearrange(t, '1 ... -> ...'), (quantize, embed_ind))
 
         dist = unpack_one(dist, ps, 'h * d')
 
         return quantize, embed_ind, dist
 
@@ -452,14 +455,18 @@
             embed_normalized = l2norm(embed_normalized)
 
             self.embed.data.copy_(l2norm(embed_normalized))
             self.expire_codes_(x)
 
         quantize = batched_embedding(embed_ind, self.embed)
 
+        if self.training:
+            l2norm_x = l2norm(x)
+            quantize = l2norm_x + (quantize - l2norm_x).detach()
+
         if needs_codebook_dim:
             quantize, embed_ind = map(lambda t: rearrange(t, '1 ... -> ...'), (quantize, embed_ind))
 
         dist = unpack_one(dist, ps, 'h * d')
         return quantize, embed_ind, dist
 
 # main class
@@ -583,17 +590,14 @@
 
         if is_multiheaded:
             ein_rhs_eq = 'h b n d' if self.separate_codebook_per_head else '1 (b h) n d'
             x = rearrange(x, f'b n (h d) -> {ein_rhs_eq}', h = heads)
 
         quantize, embed_ind, distances = self._codebook(x)
 
-        if self.training:
-            quantize = x + (quantize - x).detach()
-
         if return_loss:
             if not is_multiheaded:
                 dist_einops_eq = '1 b n l -> b l n'
             elif self.separate_codebook_per_head:
                 dist_einops_eq = 'c b n l -> b l n c'
             else:
                 dist_einops_eq = '1 (b h) n l -> b l n h'
```

### Comparing `vector_quantize_pytorch-1.5.4/vector_quantize_pytorch.egg-info/PKG-INFO` & `vector_quantize_pytorch-1.5.5/vector_quantize_pytorch.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-quantize-pytorch
-Version: 1.5.4
+Version: 1.5.5
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

