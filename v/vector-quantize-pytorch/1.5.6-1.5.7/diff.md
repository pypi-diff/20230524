# Comparing `tmp/vector_quantize_pytorch-1.5.6.tar.gz` & `tmp/vector_quantize_pytorch-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.5.6.tar", last modified: Wed May 24 13:58:59 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.5.7.tar", last modified: Wed May 24 14:18:41 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.5.6.tar` & `vector_quantize_pytorch-1.5.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:58:59.952580 vector_quantize_pytorch-1.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-24 13:58:50.000000 vector_quantize_pytorch-1.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-24 13:58:59.948580 vector_quantize_pytorch-1.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15061 2023-05-24 13:58:50.000000 vector_quantize_pytorch-1.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 13:58:59.952580 vector_quantize_pytorch-1.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-24 13:58:50.000000 vector_quantize_pytorch-1.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:58:59.948580 vector_quantize_pytorch-1.5.6/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-24 13:58:50.000000 vector_quantize_pytorch-1.5.6/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-24 13:58:50.000000 vector_quantize_pytorch-1.5.6/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-24 13:58:50.000000 vector_quantize_pytorch-1.5.6/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (123)    23866 2023-05-24 13:58:50.000000 vector_quantize_pytorch-1.5.6/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:58:59.948580 vector_quantize_pytorch-1.5.6/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-24 13:58:59.000000 vector_quantize_pytorch-1.5.6/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-24 13:58:59.000000 vector_quantize_pytorch-1.5.6/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:58:59.000000 vector_quantize_pytorch-1.5.6/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-24 13:58:59.000000 vector_quantize_pytorch-1.5.6/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-24 13:58:59.000000 vector_quantize_pytorch-1.5.6/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:18:41.417297 vector_quantize_pytorch-1.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-24 14:18:26.000000 vector_quantize_pytorch-1.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-24 14:18:41.417297 vector_quantize_pytorch-1.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15061 2023-05-24 14:18:26.000000 vector_quantize_pytorch-1.5.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 14:18:41.417297 vector_quantize_pytorch-1.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-24 14:18:26.000000 vector_quantize_pytorch-1.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:18:41.417297 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-24 14:18:26.000000 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-24 14:18:26.000000 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-24 14:18:26.000000 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24348 2023-05-24 14:18:26.000000 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:18:41.417297 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-24 14:18:41.000000 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-24 14:18:41.000000 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:18:41.000000 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-24 14:18:41.000000 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-24 14:18:41.000000 vector_quantize_pytorch-1.5.7/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.5.6/LICENSE` & `vector_quantize_pytorch-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.6/PKG-INFO` & `vector_quantize_pytorch-1.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.5.6
+Version: 1.5.7
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.5.6/README.md` & `vector_quantize_pytorch-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.6/setup.py` & `vector_quantize_pytorch-1.5.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vector_quantize_pytorch',
   packages = find_packages(),
-  version = '1.5.6',
+  version = '1.5.7',
   license='MIT',
   description = 'Vector Quantization - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vector-quantizer-pytorch',
   keywords = [
```

### Comparing `vector_quantize_pytorch-1.5.6/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.5.7/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.6/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.5.7/vector_quantize_pytorch/residual_vq.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.6/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.5.7/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -575,29 +575,42 @@
         if only_one:
             x = rearrange(x, 'b d -> b 1 d')
 
         shape, device, heads, is_multiheaded, codebook_size, return_loss = x.shape, x.device, self.heads, self.heads > 1, self.codebook_size, exists(indices)
 
         need_transpose = not self.channel_last and not self.accept_image_fmap
 
+        # rearrange inputs
+
         if self.accept_image_fmap:
             height, width = x.shape[-2:]
             x = rearrange(x, 'b c h w -> b (h w) c')
 
         if need_transpose:
             x = rearrange(x, 'b d n -> b n d')
 
+        # project input
+
         x = self.project_in(x)
 
+        # l2norm for cosine sim, otherwise identity
+
         x = self._codebook.transform_input(x)
 
+        # handle multi-headed separate codebooks
+
         if is_multiheaded:
             ein_rhs_eq = 'h b n d' if self.separate_codebook_per_head else '1 (b h) n d'
             x = rearrange(x, f'b n (h d) -> {ein_rhs_eq}', h = heads)
 
+            if exists(mask):
+                mask = repeat(mask, 'b n -> h b n', h = heads)
+
+        # quantize
+
         quantize, embed_ind, distances = self._codebook(x)
 
         if self.training:
             quantize = x + (quantize - x).detach()
 
         # function for calculating cross entropy loss to distance matrix
         # used for (1) naturalspeech2 training residual vq latents to be close to the correct codes and (2) cross-entropy based commitment loss
@@ -614,33 +627,47 @@
                 rearrange(distances, dist_einops_eq, b = shape[0]),
                 codes,
                 ignore_index = -1
             )
 
             return ce_loss
 
+        # if returning cross entropy loss on codes that were passed in
+
         if return_loss:
             return quantize, calculate_ce_loss(indices)
 
+        # transform embedding indices
+
+        if is_multiheaded:
+            if self.separate_codebook_per_head:
+                embed_ind = rearrange(embed_ind, 'h b n -> b n h', h = heads)
+            else:
+                embed_ind = rearrange(embed_ind, '1 (b h) n -> b n h', h = heads)
+
+        if self.accept_image_fmap:
+            embed_ind = rearrange(embed_ind, 'b (h w) ... -> b h w ...', h = height, w = width)
+
+        if only_one:
+            embed_ind = rearrange(embed_ind, 'b 1 -> b')
+
+        # aggregate loss
+
         loss = torch.tensor([0.], device = device, requires_grad = self.training)
 
         if self.training:
             if self.commitment_weight > 0:
                 if self.commitment_use_cross_entropy_loss:
-                    commit_loss = calculate_ce_loss(distances, embed_ind)
+                    commit_loss = calculate_ce_loss(embed_ind)
                 else:
                     detached_quantize = quantize.detach()
 
                     if exists(mask):
                         # with variable lengthed sequences
                         commit_loss = F.mse_loss(detached_quantize, x, reduction = 'none')
-
-                        if is_multiheaded:
-                            mask = repeat(mask, 'b n -> c (b h) n', c = commit_loss.shape[0], h = commit_loss.shape[1] // mask.shape[0])
-
                         commit_loss = commit_loss[mask].mean()
                     else:
                         commit_loss = F.mse_loss(detached_quantize, x)
 
                 loss = loss + commit_loss * self.commitment_weight
 
             if self.orthogonal_reg_weight > 0:
@@ -658,29 +685,31 @@
                 if exists(self.orthogonal_reg_max_codes) and num_codes > self.orthogonal_reg_max_codes:
                     rand_ids = torch.randperm(num_codes, device = device)[:self.orthogonal_reg_max_codes]
                     codebook = codebook[:, rand_ids]
 
                 orthogonal_reg_loss = orthogonal_loss_fn(codebook)
                 loss = loss + orthogonal_reg_loss * self.orthogonal_reg_weight
 
+        # handle multi-headed quantized embeddings
+
         if is_multiheaded:
             if self.separate_codebook_per_head:
                 quantize = rearrange(quantize, 'h b n d -> b n (h d)', h = heads)
-                embed_ind = rearrange(embed_ind, 'h b n -> b n h', h = heads)
             else:
                 quantize = rearrange(quantize, '1 (b h) n d -> b n (h d)', h = heads)
-                embed_ind = rearrange(embed_ind, '1 (b h) n -> b n h', h = heads)
+
+        # project out
 
         quantize = self.project_out(quantize)
 
+        # rearrange quantized embeddings
+
         if need_transpose:
             quantize = rearrange(quantize, 'b n d -> b d n')
 
         if self.accept_image_fmap:
             quantize = rearrange(quantize, 'b (h w) c -> b c h w', h = height, w = width)
-            embed_ind = rearrange(embed_ind, 'b (h w) ... -> b h w ...', h = height, w = width)
 
         if only_one:
             quantize = rearrange(quantize, 'b 1 d -> b d')
-            embed_ind = rearrange(embed_ind, 'b 1 -> b')
 
         return quantize, embed_ind, loss
```

### Comparing `vector_quantize_pytorch-1.5.6/vector_quantize_pytorch.egg-info/PKG-INFO` & `vector_quantize_pytorch-1.5.7/vector_quantize_pytorch.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-quantize-pytorch
-Version: 1.5.6
+Version: 1.5.7
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

