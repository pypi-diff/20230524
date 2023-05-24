# Comparing `tmp/imagen-pytorch-1.9.6.tar.gz` & `tmp/imagen-pytorch-1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imagen-pytorch-1.9.6.tar", last modified: Sun Aug 21 16:14:45 2022, max compression
+gzip compressed data, was "imagen-pytorch-1.9.7.tar", last modified: Mon Aug 22 17:29:39 2022, max compression
```

## Comparing `imagen-pytorch-1.9.6.tar` & `imagen-pytorch-1.9.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 16:14:45.933760 imagen-pytorch-1.9.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-08-21 16:14:36.000000 imagen-pytorch-1.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-08-21 16:14:45.933760 imagen-pytorch-1.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    31342 2022-08-21 16:14:36.000000 imagen-pytorch-1.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 16:14:45.929759 imagen-pytorch-1.9.6/imagen_pytorch/
--rw-r--r--   0 runner    (1001) docker     (121)      685 2022-08-21 16:14:36.000000 imagen-pytorch-1.9.6/imagen_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-08-21 16:14:36.000000 imagen-pytorch-1.9.6/imagen_pytorch/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     6154 2022-08-21 16:14:36.000000 imagen-pytorch-1.9.6/imagen_pytorch/configs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1733 2022-08-21 16:14:36.000000 imagen-pytorch-1.9.6/imagen_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (121)    30653 2022-08-21 16:14:36.000000 imagen-pytorch-1.9.6/imagen_pytorch/elucidated_imagen.py
--rw-r--r--   0 runner    (1001) docker     (121)    86979 2022-08-21 16:14:36.000000 imagen-pytorch-1.9.6/imagen_pytorch/imagen_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 16:14:45.933760 imagen-pytorch-1.9.6/imagen_pytorch/imagen_video/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-08-21 16:14:36.000000 imagen-pytorch-1.9.6/imagen_pytorch/imagen_video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    53995 2022-08-21 16:14:36.000000 imagen-pytorch-1.9.6/imagen_pytorch/imagen_video/imagen_video.py
--rw-r--r--   0 runner    (1001) docker     (121)     3053 2022-08-21 16:14:36.000000 imagen-pytorch-1.9.6/imagen_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (121)    32280 2022-08-21 16:14:36.000000 imagen-pytorch-1.9.6/imagen_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-08-21 16:14:36.000000 imagen-pytorch-1.9.6/imagen_pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-21 16:14:36.000000 imagen-pytorch-1.9.6/imagen_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 16:14:45.933760 imagen-pytorch-1.9.6/imagen_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-08-21 16:14:45.000000 imagen-pytorch-1.9.6/imagen_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-08-21 16:14:45.000000 imagen-pytorch-1.9.6/imagen_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-21 16:14:45.000000 imagen-pytorch-1.9.6/imagen_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-21 16:14:45.000000 imagen-pytorch-1.9.6/imagen_pytorch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-08-21 16:14:45.000000 imagen-pytorch-1.9.6/imagen_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-21 16:14:45.000000 imagen-pytorch-1.9.6/imagen_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-21 16:14:45.933760 imagen-pytorch-1.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-08-21 16:14:36.000000 imagen-pytorch-1.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 17:29:39.349363 imagen-pytorch-1.9.7/
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2022-08-22 17:29:39.349363 imagen-pytorch-1.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    31342 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 17:29:39.349363 imagen-pytorch-1.9.7/imagen_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (121)      685 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6154 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/configs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1733 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30653 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/elucidated_imagen.py
+-rw-r--r--   0 runner    (1001) docker     (121)    87117 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/imagen_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 17:29:39.349363 imagen-pytorch-1.9.7/imagen_pytorch/imagen_video/
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/imagen_video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    53995 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/imagen_video/imagen_video.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3053 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32674 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/imagen_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 17:29:39.349363 imagen-pytorch-1.9.7/imagen_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2022-08-22 17:29:39.000000 imagen-pytorch-1.9.7/imagen_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2022-08-22 17:29:39.000000 imagen-pytorch-1.9.7/imagen_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 17:29:39.000000 imagen-pytorch-1.9.7/imagen_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-22 17:29:39.000000 imagen-pytorch-1.9.7/imagen_pytorch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      194 2022-08-22 17:29:39.000000 imagen-pytorch-1.9.7/imagen_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-22 17:29:39.000000 imagen-pytorch-1.9.7/imagen_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 17:29:39.349363 imagen-pytorch-1.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-08-22 17:29:29.000000 imagen-pytorch-1.9.7/setup.py
```

### Comparing `imagen-pytorch-1.9.6/LICENSE` & `imagen-pytorch-1.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `imagen-pytorch-1.9.6/PKG-INFO` & `imagen-pytorch-1.9.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imagen-pytorch
-Version: 1.9.6
+Version: 1.9.7
 Summary: Imagen - unprecedented photorealism × deep level of language understanding
 Home-page: https://github.com/lucidrains/imagen-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,text-to-image,denoising-diffusion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `imagen-pytorch-1.9.6/README.md` & `imagen-pytorch-1.9.7/README.md`

 * *Files identical despite different names*

### Comparing `imagen-pytorch-1.9.6/imagen_pytorch/__init__.py` & `imagen-pytorch-1.9.7/imagen_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `imagen-pytorch-1.9.6/imagen_pytorch/cli.py` & `imagen-pytorch-1.9.7/imagen_pytorch/cli.py`

 * *Files identical despite different names*

### Comparing `imagen-pytorch-1.9.6/imagen_pytorch/configs.py` & `imagen-pytorch-1.9.7/imagen_pytorch/configs.py`

 * *Files identical despite different names*

### Comparing `imagen-pytorch-1.9.6/imagen_pytorch/data.py` & `imagen-pytorch-1.9.7/imagen_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `imagen-pytorch-1.9.6/imagen_pytorch/elucidated_imagen.py` & `imagen-pytorch-1.9.7/imagen_pytorch/elucidated_imagen.py`

 * *Files identical despite different names*

### Comparing `imagen-pytorch-1.9.6/imagen_pytorch/imagen_pytorch.py` & `imagen-pytorch-1.9.7/imagen_pytorch/imagen_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,22 +233,25 @@
 
         # following (eq. 33)
         posterior_variance = (sigma_next ** 2) * c
         posterior_log_variance_clipped = log(posterior_variance, eps = 1e-20)
         return posterior_mean, posterior_variance, posterior_log_variance_clipped
 
     def q_sample(self, x_start, t, noise = None):
+        dtype = x_start.dtype
+
         if isinstance(t, float):
             batch = x_start.shape[0]
-            t = torch.full((batch,), t, device = x_start.device, dtype = x_start.dtype)
+            t = torch.full((batch,), t, device = x_start.device, dtype = dtype)
 
         noise = default(noise, lambda: torch.randn_like(x_start))
-        log_snr = self.log_snr(t)
+        log_snr = self.log_snr(t).type(dtype)
         log_snr_padded_dim = right_pad_dims_to(x_start, log_snr)
         alpha, sigma =  log_snr_to_alpha_sigma(log_snr_padded_dim)
+
         return alpha * x_start + sigma * noise, log_snr
 
     def q_sample_from_to(self, x_from, from_t, to_t, noise = None):
         shape, device, dtype = x_from.shape, x_from.device, x_from.dtype
         batch = shape[0]
 
         if isinstance(from_t, float):
@@ -280,36 +283,43 @@
 class LayerNorm(nn.Module):
     def __init__(self, dim, stable = False):
         super().__init__()
         self.stable = stable
         self.g = nn.Parameter(torch.ones(dim))
 
     def forward(self, x):
+        dtype = x.dtype
+
         if self.stable:
             x = x / x.amax(dim = -1, keepdim = True).detach()
 
         eps = 1e-5 if x.dtype == torch.float32 else 1e-3
         var = torch.var(x, dim = -1, unbiased = False, keepdim = True)
         mean = torch.mean(x, dim = -1, keepdim = True)
-        return (x - mean) * (var + eps).rsqrt() * self.g
+
+        return (x - mean) * (var + eps).rsqrt().type(dtype) * self.g.type(dtype)
+
 
 class ChanLayerNorm(nn.Module):
     def __init__(self, dim, stable = False):
         super().__init__()
         self.stable = stable
         self.g = nn.Parameter(torch.ones(1, dim, 1, 1))
 
     def forward(self, x):
+        dtype = x.dtype
+
         if self.stable:
             x = x / x.amax(dim = 1, keepdim = True).detach()
 
         eps = 1e-5 if x.dtype == torch.float32 else 1e-3
         var = torch.var(x, dim = 1, unbiased = False, keepdim = True)
         mean = torch.mean(x, dim = 1, keepdim = True)
-        return (x - mean) * (var + eps).rsqrt() * self.g
+
+        return (x - mean) * (var + eps).rsqrt().type(dtype) * self.g.type(dtype)
 
 class Always():
     def __init__(self, val):
         self.val = val
 
     def __call__(self, *args, **kwargs):
         return self.val
@@ -488,14 +498,15 @@
             LayerNorm(dim)
         )
 
     def forward(self, x, context = None, mask = None, attn_bias = None):
         b, n, device = *x.shape[:2], x.device
 
         x = self.norm(x)
+
         q, k, v = (self.to_q(x), *self.to_kv(x).chunk(2, dim = -1))
 
         q = rearrange(q, 'b n (h d) -> b h n d', h = self.heads)
         q = q * self.scale
 
         # add null key / value for classifier free guidance in prior net
```

### Comparing `imagen-pytorch-1.9.6/imagen_pytorch/imagen_video/imagen_video.py` & `imagen-pytorch-1.9.7/imagen_pytorch/imagen_video/imagen_video.py`

 * *Files identical despite different names*

### Comparing `imagen-pytorch-1.9.6/imagen_pytorch/t5.py` & `imagen-pytorch-1.9.7/imagen_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `imagen-pytorch-1.9.6/imagen_pytorch/trainer.py` & `imagen-pytorch-1.9.7/imagen_pytorch/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,28 +106,33 @@
         was_training = model.training
         model.eval()
         out = fn(model, *args, **kwargs)
         model.train(was_training)
         return out
     return inner
 
-def cast_torch_tensor(fn):
+def cast_torch_tensor(fn, cast_fp16 = False):
     @wraps(fn)
     def inner(model, *args, **kwargs):
         device = kwargs.pop('_device', model.device)
         cast_device = kwargs.pop('_cast_device', True)
 
+        should_cast_fp16 = cast_fp16 and model.cast_half_at_training
+
         kwargs_keys = kwargs.keys()
         all_args = (*args, *kwargs.values())
         split_kwargs_index = len(all_args) - len(kwargs_keys)
         all_args = tuple(map(lambda t: torch.from_numpy(t) if exists(t) and isinstance(t, np.ndarray) else t, all_args))
 
         if cast_device:
             all_args = tuple(map(lambda t: t.to(device) if exists(t) and isinstance(t, torch.Tensor) else t, all_args))
 
+        if should_cast_fp16:
+            all_args = tuple(map(lambda t: t.half() if exists(t) and isinstance(t, torch.Tensor) else t, all_args))
+
         args, kwargs_values = all_args[:split_kwargs_index], all_args[split_kwargs_index:]
         kwargs = dict(tuple(zip(kwargs_keys, kwargs_values)))
 
         out = fn(model, *args, **kwargs)
         return out
     return inner
 
@@ -280,14 +285,18 @@
             'split_batches': split_batches,
             'mixed_precision': accelerator_mixed_precision,
             'kwargs_handlers': [DistributedDataParallelKwargs(find_unused_parameters = True)]
         , **accelerate_kwargs})
 
         ImagenTrainer.locked = self.is_distributed
 
+        # cast data to fp16 at training time if needed
+
+        self.cast_half_at_training = accelerator_mixed_precision == 'fp16'
+
         # grad scaler must be managed outside of accelerator
 
         grad_scaler_enabled = fp16
 
         # imagen, unets and ema unets
 
         self.imagen = imagen
@@ -924,15 +933,15 @@
         self.print_untrained_unets()        
 
         with context():
             output = self.imagen.sample(*args, device = self.device, use_tqdm = self.is_main, **kwargs)
 
         return output
 
-    @cast_torch_tensor
+    @partial(cast_torch_tensor, cast_fp16 = True)
     def forward(
         self,
         *args,
         unet_number = None,
         max_batch_size = None,
         **kwargs
     ):
```

### Comparing `imagen-pytorch-1.9.6/imagen_pytorch/utils.py` & `imagen-pytorch-1.9.7/imagen_pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `imagen-pytorch-1.9.6/imagen_pytorch.egg-info/PKG-INFO` & `imagen-pytorch-1.9.7/imagen_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imagen-pytorch
-Version: 1.9.6
+Version: 1.9.7
 Summary: Imagen - unprecedented photorealism × deep level of language understanding
 Home-page: https://github.com/lucidrains/imagen-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,text-to-image,denoising-diffusion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `imagen-pytorch-1.9.6/imagen_pytorch.egg-info/SOURCES.txt` & `imagen-pytorch-1.9.7/imagen_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imagen-pytorch-1.9.6/setup.py` & `imagen-pytorch-1.9.7/setup.py`

 * *Files identical despite different names*

